# Comparing `tmp/sambacc-0.4.tar.gz` & `tmp/sambacc-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sambacc-0.4.tar", last modified: Mon Nov 27 18:28:29 2023, max compression
+gzip compressed data, was "sambacc-0.5.tar", last modified: Wed May 15 16:47:40 2024, max compression
```

## Comparing `sambacc-0.4.tar` & `sambacc-0.5.tar`

### file list

```diff
@@ -1,106 +1,108 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.959629 sambacc-0.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.935629 sambacc-0.4/.copr/
--rw-r--r--   0 root         (0) root         (0)      600 2023-08-09 14:48:32.000000 sambacc-0.4/.copr/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.935629 sambacc-0.4/.github/
--rw-r--r--   0 root         (0) root         (0)     3151 2023-09-19 20:10:00.000000 sambacc-0.4/.github/mergify.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.935629 sambacc-0.4/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1971 2023-09-19 18:53:58.000000 sambacc-0.4/.github/workflows/ci.yml
--rw-r--r--   0 root         (0) root         (0)       92 2023-07-07 14:51:46.000000 sambacc-0.4/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4615 2023-08-09 14:48:32.000000 sambacc-0.4/.gitlint
--rw-r--r--   0 root         (0) root         (0)      122 2023-07-07 14:51:46.000000 sambacc-0.4/.hgignore
--rw-r--r--   0 root         (0) root         (0)    35149 2023-07-07 14:51:46.000000 sambacc-0.4/COPYING
--rw-r--r--   0 root         (0) root         (0)      100 2023-08-09 14:48:32.000000 sambacc-0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7291 2023-11-27 18:28:29.959629 sambacc-0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6709 2023-09-15 13:41:12.000000 sambacc-0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.936629 sambacc-0.4/docs/
--rw-r--r--   0 root         (0) root         (0)    11915 2023-11-15 15:05:41.000000 sambacc-0.4/docs/configuration.md
--rw-r--r--   0 root         (0) root         (0)     4018 2023-11-27 17:42:32.000000 sambacc-0.4/docs/release-process.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.936629 sambacc-0.4/examples/
--rw-r--r--   0 root         (0) root         (0)     2972 2023-08-10 21:11:00.000000 sambacc-0.4/examples/addc.json
--rw-r--r--   0 root         (0) root         (0)      906 2023-07-07 14:51:46.000000 sambacc-0.4/examples/ctdb.json
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-07 14:51:46.000000 sambacc-0.4/examples/example1.json
--rw-r--r--   0 root         (0) root         (0)      842 2023-07-07 14:51:46.000000 sambacc-0.4/examples/minimal.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.937629 sambacc-0.4/extras/
--rw-r--r--   0 root         (0) root         (0)     2179 2023-11-15 15:05:41.000000 sambacc-0.4/extras/python-sambacc.spec
--rw-r--r--   0 root         (0) root         (0)      819 2023-08-09 14:48:32.000000 sambacc-0.4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.940629 sambacc-0.4/sambacc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 14:51:46.000000 sambacc-0.4/sambacc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       90 2023-11-27 18:28:29.000000 sambacc-0.4/sambacc/_version.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-07-07 14:51:46.000000 sambacc-0.4/sambacc/_xattr.py
--rw-r--r--   0 root         (0) root         (0)     5314 2023-08-23 17:28:34.000000 sambacc-0.4/sambacc/addc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.944629 sambacc-0.4/sambacc/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 14:51:46.000000 sambacc-0.4/sambacc/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5936 2023-08-23 17:28:34.000000 sambacc-0.4/sambacc/commands/addc.py
--rw-r--r--   0 root         (0) root         (0)     1391 2023-07-07 14:51:46.000000 sambacc-0.4/sambacc/commands/check.py
--rw-r--r--   0 root         (0) root         (0)     6019 2023-11-15 15:05:41.000000 sambacc-0.4/sambacc/commands/cli.py
--rw-r--r--   0 root         (0) root         (0)     5348 2023-09-26 21:21:14.000000 sambacc-0.4/sambacc/commands/config.py
--rw-r--r--   0 root         (0) root         (0)     8412 2023-09-26 21:21:14.000000 sambacc-0.4/sambacc/commands/ctdb.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/commands/dcmain.py
--rw-r--r--   0 root         (0) root         (0)     3447 2023-09-26 21:21:14.000000 sambacc-0.4/sambacc/commands/dns.py
--rw-r--r--   0 root         (0) root         (0)     3802 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/commands/initialize.py
--rw-r--r--   0 root         (0) root         (0)     4709 2023-11-15 15:05:41.000000 sambacc-0.4/sambacc/commands/join.py
--rw-r--r--   0 root         (0) root         (0)     8248 2023-11-15 15:05:41.000000 sambacc-0.4/sambacc/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     3248 2023-07-07 14:51:46.000000 sambacc-0.4/sambacc/commands/run.py
--rw-r--r--   0 root         (0) root         (0)     1976 2023-07-07 14:51:46.000000 sambacc-0.4/sambacc/commands/users.py
--rw-r--r--   0 root         (0) root         (0)    17978 2023-11-15 15:05:41.000000 sambacc-0.4/sambacc/config.py
--rw-r--r--   0 root         (0) root         (0)     4255 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/container_dns.py
--rw-r--r--   0 root         (0) root         (0)    17972 2023-09-15 19:52:31.000000 sambacc-0.4/sambacc/ctdb.py
--rw-r--r--   0 root         (0) root         (0)     3154 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/inotify_waiter.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/jfile.py
--rw-r--r--   0 root         (0) root         (0)     7738 2023-11-15 15:05:41.000000 sambacc-0.4/sambacc/join.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-11-15 15:05:41.000000 sambacc-0.4/sambacc/leader.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/netcmd_loader.py
--rw-r--r--   0 root         (0) root         (0)     2347 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/nsswitch_loader.py
--rw-r--r--   0 root         (0) root         (0)     1890 2023-11-15 15:05:41.000000 sambacc-0.4/sambacc/opener.py
--rw-r--r--   0 root         (0) root         (0)     2897 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/passdb_loader.py
--rw-r--r--   0 root         (0) root         (0)     2928 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/passwd_loader.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-07-07 14:51:46.000000 sambacc-0.4/sambacc/paths.py
--rw-r--r--   0 root         (0) root         (0)     5147 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/permissions.py
--rw-r--r--   0 root         (0) root         (0)     5295 2023-11-15 15:05:41.000000 sambacc-0.4/sambacc/rados_opener.py
--rw-r--r--   0 root         (0) root         (0)     5230 2023-09-15 19:52:31.000000 sambacc-0.4/sambacc/samba_cmds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.947629 sambacc-0.4/sambacc/schema/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9823 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/schema/conf-v0.schema.json
--rw-r--r--   0 root         (0) root         (0)     9783 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/schema/conf-v0.schema.yaml
--rw-r--r--   0 root         (0) root         (0)    12292 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/schema/conf_v0_schema.py
--rw-r--r--   0 root         (0) root         (0)     4906 2023-08-09 14:48:32.000000 sambacc-0.4/sambacc/schema/tool.py
--rw-r--r--   0 root         (0) root         (0)     3016 2023-11-15 15:05:41.000000 sambacc-0.4/sambacc/simple_waiter.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-09-26 21:21:14.000000 sambacc-0.4/sambacc/smbconf_api.py
--rw-r--r--   0 root         (0) root         (0)     5232 2023-08-23 17:30:10.000000 sambacc-0.4/sambacc/smbconf_samba.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-07-07 14:51:46.000000 sambacc-0.4/sambacc/textfile.py
--rw-r--r--   0 root         (0) root         (0)     1006 2023-09-16 14:40:49.000000 sambacc-0.4/sambacc/typelets.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-11-15 15:05:41.000000 sambacc-0.4/sambacc/url_opener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.958629 sambacc-0.4/sambacc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7291 2023-11-27 18:28:29.000000 sambacc-0.4/sambacc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2104 2023-11-27 18:28:29.000000 sambacc-0.4/sambacc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-27 18:28:29.000000 sambacc-0.4/sambacc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-11-27 18:28:29.000000 sambacc-0.4/sambacc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-11-27 18:28:29.000000 sambacc-0.4/sambacc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-11-27 18:28:29.000000 sambacc-0.4/sambacc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      862 2023-11-27 18:28:29.960629 sambacc-0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.958629 sambacc-0.4/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 14:51:46.000000 sambacc-0.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 18:28:29.958629 sambacc-0.4/tests/container/
--rw-r--r--   0 root         (0) root         (0)      626 2023-08-23 17:28:34.000000 sambacc-0.4/tests/container/Containerfile
--rwxr-xr-x   0 root         (0) root         (0)     7060 2023-09-19 18:06:53.000000 sambacc-0.4/tests/container/build.sh
--rw-r--r--   0 root         (0) root         (0)     4883 2023-08-23 17:28:34.000000 sambacc-0.4/tests/test_addc.py
--rw-r--r--   0 root         (0) root         (0)     7957 2023-08-09 14:48:32.000000 sambacc-0.4/tests/test_commands_config.py
--rw-r--r--   0 root         (0) root         (0)    30082 2023-11-15 15:05:41.000000 sambacc-0.4/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-08-09 14:48:32.000000 sambacc-0.4/tests/test_container_dns.py
--rw-r--r--   0 root         (0) root         (0)    18241 2023-09-26 21:21:14.000000 sambacc-0.4/tests/test_ctdb.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-07-07 14:51:46.000000 sambacc-0.4/tests/test_inotify_waiter.py
--rw-r--r--   0 root         (0) root         (0)     2537 2023-07-07 14:51:46.000000 sambacc-0.4/tests/test_jfile.py
--rw-r--r--   0 root         (0) root         (0)     8420 2023-11-15 15:05:41.000000 sambacc-0.4/tests/test_join.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-07-07 14:51:46.000000 sambacc-0.4/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-07-07 14:51:46.000000 sambacc-0.4/tests/test_netcmd_loader.py
--rw-r--r--   0 root         (0) root         (0)     3435 2023-07-07 14:51:46.000000 sambacc-0.4/tests/test_passdb_loader.py
--rw-r--r--   0 root         (0) root         (0)     3653 2023-07-07 14:51:46.000000 sambacc-0.4/tests/test_passwd_loader.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-07-07 14:51:46.000000 sambacc-0.4/tests/test_paths.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-07-07 14:51:46.000000 sambacc-0.4/tests/test_permissions.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-11-15 15:05:41.000000 sambacc-0.4/tests/test_rados_opener.py
--rw-r--r--   0 root         (0) root         (0)     4826 2023-07-07 14:51:46.000000 sambacc-0.4/tests/test_samba_cmds.py
--rw-r--r--   0 root         (0) root         (0)     1761 2023-09-15 13:41:12.000000 sambacc-0.4/tests/test_simple_waiter.py
--rw-r--r--   0 root         (0) root         (0)     2717 2023-08-23 17:28:34.000000 sambacc-0.4/tests/test_smbconf_api.py
--rw-r--r--   0 root         (0) root         (0)     5531 2023-08-23 17:30:15.000000 sambacc-0.4/tests/test_smbconf_samba.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-11-15 15:05:41.000000 sambacc-0.4/tests/test_url_opener.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-09-26 21:06:17.000000 sambacc-0.4/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.067079 sambacc-0.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.042079 sambacc-0.5/.copr/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-09 14:48:32.000000 sambacc-0.5/.copr/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.042079 sambacc-0.5/.github/
+-rw-r--r--   0 root         (0) root         (0)     3151 2024-05-15 16:34:19.000000 sambacc-0.5/.github/mergify.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.042079 sambacc-0.5/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-05-15 16:34:19.000000 sambacc-0.5/.github/workflows/ci.yml
+-rw-r--r--   0 root         (0) root         (0)       92 2023-07-07 14:51:46.000000 sambacc-0.5/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4615 2023-08-09 14:48:32.000000 sambacc-0.5/.gitlint
+-rw-r--r--   0 root         (0) root         (0)      122 2023-07-07 14:51:46.000000 sambacc-0.5/.hgignore
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-07-07 14:51:46.000000 sambacc-0.5/COPYING
+-rw-r--r--   0 root         (0) root         (0)      100 2023-08-09 14:48:32.000000 sambacc-0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7291 2024-05-15 16:47:40.067079 sambacc-0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6709 2023-09-15 13:41:12.000000 sambacc-0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.043079 sambacc-0.5/docs/
+-rw-r--r--   0 root         (0) root         (0)    13451 2024-03-04 15:52:27.000000 sambacc-0.5/docs/configuration.md
+-rw-r--r--   0 root         (0) root         (0)     4018 2023-11-27 17:42:32.000000 sambacc-0.5/docs/release-process.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.044079 sambacc-0.5/examples/
+-rw-r--r--   0 root         (0) root         (0)     2972 2023-08-10 21:11:00.000000 sambacc-0.5/examples/addc.json
+-rw-r--r--   0 root         (0) root         (0)     3210 2024-02-26 16:00:14.000000 sambacc-0.5/examples/addc_ou.json
+-rw-r--r--   0 root         (0) root         (0)     3067 2024-03-02 22:04:44.000000 sambacc-0.5/examples/addc_x.json
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-07 14:51:46.000000 sambacc-0.5/examples/ctdb.json
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-07 14:51:46.000000 sambacc-0.5/examples/example1.json
+-rw-r--r--   0 root         (0) root         (0)      842 2023-07-07 14:51:46.000000 sambacc-0.5/examples/minimal.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.044079 sambacc-0.5/extras/
+-rw-r--r--   0 root         (0) root         (0)     2320 2024-02-26 15:18:47.000000 sambacc-0.5/extras/python-sambacc.spec
+-rw-r--r--   0 root         (0) root         (0)      819 2023-08-09 14:48:32.000000 sambacc-0.5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.056079 sambacc-0.5/sambacc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 14:51:46.000000 sambacc-0.5/sambacc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-15 16:47:39.000000 sambacc-0.5/sambacc/_version.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-07-07 14:51:46.000000 sambacc-0.5/sambacc/_xattr.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2024-03-04 15:52:27.000000 sambacc-0.5/sambacc/addc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.061079 sambacc-0.5/sambacc/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 14:51:46.000000 sambacc-0.5/sambacc/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6627 2024-03-04 15:52:27.000000 sambacc-0.5/sambacc/commands/addc.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-07-07 14:51:46.000000 sambacc-0.5/sambacc/commands/check.py
+-rw-r--r--   0 root         (0) root         (0)     6019 2024-01-03 20:12:04.000000 sambacc-0.5/sambacc/commands/cli.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2024-02-26 15:18:47.000000 sambacc-0.5/sambacc/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)     8402 2024-02-26 15:18:47.000000 sambacc-0.5/sambacc/commands/ctdb.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-08-09 14:48:32.000000 sambacc-0.5/sambacc/commands/dcmain.py
+-rw-r--r--   0 root         (0) root         (0)     3441 2024-02-26 15:18:47.000000 sambacc-0.5/sambacc/commands/dns.py
+-rw-r--r--   0 root         (0) root         (0)     3802 2023-08-09 14:48:32.000000 sambacc-0.5/sambacc/commands/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     4709 2023-11-15 15:05:41.000000 sambacc-0.5/sambacc/commands/join.py
+-rw-r--r--   0 root         (0) root         (0)    10975 2024-02-26 15:18:47.000000 sambacc-0.5/sambacc/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     3248 2023-07-07 14:51:46.000000 sambacc-0.5/sambacc/commands/run.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-07-07 14:51:46.000000 sambacc-0.5/sambacc/commands/users.py
+-rw-r--r--   0 root         (0) root         (0)    19190 2024-03-04 15:52:27.000000 sambacc-0.5/sambacc/config.py
+-rw-r--r--   0 root         (0) root         (0)     4255 2023-08-09 14:48:32.000000 sambacc-0.5/sambacc/container_dns.py
+-rw-r--r--   0 root         (0) root         (0)    17972 2024-01-03 20:04:00.000000 sambacc-0.5/sambacc/ctdb.py
+-rw-r--r--   0 root         (0) root         (0)     3154 2023-08-09 14:48:32.000000 sambacc-0.5/sambacc/inotify_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-08-09 14:48:32.000000 sambacc-0.5/sambacc/jfile.py
+-rw-r--r--   0 root         (0) root         (0)     7738 2023-11-15 15:05:41.000000 sambacc-0.5/sambacc/join.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-01-03 20:12:04.000000 sambacc-0.5/sambacc/leader.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-08-09 14:48:32.000000 sambacc-0.5/sambacc/netcmd_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-08-09 14:48:32.000000 sambacc-0.5/sambacc/nsswitch_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-01-03 20:12:04.000000 sambacc-0.5/sambacc/opener.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-08-09 14:48:32.000000 sambacc-0.5/sambacc/passdb_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-08-09 14:48:32.000000 sambacc-0.5/sambacc/passwd_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-07-07 14:51:46.000000 sambacc-0.5/sambacc/paths.py
+-rw-r--r--   0 root         (0) root         (0)     5147 2023-08-09 14:48:32.000000 sambacc-0.5/sambacc/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     7130 2024-01-03 20:04:00.000000 sambacc-0.5/sambacc/rados_opener.py
+-rw-r--r--   0 root         (0) root         (0)     5259 2024-02-26 16:00:14.000000 sambacc-0.5/sambacc/samba_cmds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.062079 sambacc-0.5/sambacc/schema/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 14:48:32.000000 sambacc-0.5/sambacc/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11588 2024-03-04 20:50:58.000000 sambacc-0.5/sambacc/schema/conf-v0.schema.json
+-rw-r--r--   0 root         (0) root         (0)    11452 2024-03-04 20:50:58.000000 sambacc-0.5/sambacc/schema/conf-v0.schema.yaml
+-rw-r--r--   0 root         (0) root         (0)    14962 2024-03-04 20:50:58.000000 sambacc-0.5/sambacc/schema/conf_v0_schema.py
+-rw-r--r--   0 root         (0) root         (0)     4906 2023-08-09 14:48:32.000000 sambacc-0.5/sambacc/schema/tool.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2024-01-03 20:12:04.000000 sambacc-0.5/sambacc/simple_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-01-03 20:12:04.000000 sambacc-0.5/sambacc/smbconf_api.py
+-rw-r--r--   0 root         (0) root         (0)     5232 2023-08-23 17:30:10.000000 sambacc-0.5/sambacc/smbconf_samba.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-07-07 14:51:46.000000 sambacc-0.5/sambacc/textfile.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-09-16 14:40:49.000000 sambacc-0.5/sambacc/typelets.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-11-15 15:05:41.000000 sambacc-0.5/sambacc/url_opener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.066079 sambacc-0.5/sambacc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7291 2024-05-15 16:47:39.000000 sambacc-0.5/sambacc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-05-15 16:47:40.000000 sambacc-0.5/sambacc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:47:39.000000 sambacc-0.5/sambacc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2024-05-15 16:47:40.000000 sambacc-0.5/sambacc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2024-05-15 16:47:40.000000 sambacc-0.5/sambacc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-15 16:47:40.000000 sambacc-0.5/sambacc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      862 2024-05-15 16:47:40.068079 sambacc-0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.066079 sambacc-0.5/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 14:51:46.000000 sambacc-0.5/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:40.066079 sambacc-0.5/tests/container/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-12-07 19:47:28.000000 sambacc-0.5/tests/container/Containerfile
+-rwxr-xr-x   0 root         (0) root         (0)     7060 2023-09-19 18:06:53.000000 sambacc-0.5/tests/container/build.sh
+-rw-r--r--   0 root         (0) root         (0)     6706 2024-03-04 15:52:27.000000 sambacc-0.5/tests/test_addc.py
+-rw-r--r--   0 root         (0) root         (0)     8084 2023-12-07 19:47:28.000000 sambacc-0.5/tests/test_commands_config.py
+-rw-r--r--   0 root         (0) root         (0)    30534 2024-02-26 16:00:14.000000 sambacc-0.5/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-08-09 14:48:32.000000 sambacc-0.5/tests/test_container_dns.py
+-rw-r--r--   0 root         (0) root         (0)    18241 2024-01-03 20:12:04.000000 sambacc-0.5/tests/test_ctdb.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-07-07 14:51:46.000000 sambacc-0.5/tests/test_inotify_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-07-07 14:51:46.000000 sambacc-0.5/tests/test_jfile.py
+-rw-r--r--   0 root         (0) root         (0)     8420 2023-11-15 15:05:41.000000 sambacc-0.5/tests/test_join.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-07-07 14:51:46.000000 sambacc-0.5/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2023-07-07 14:51:46.000000 sambacc-0.5/tests/test_netcmd_loader.py
+-rw-r--r--   0 root         (0) root         (0)     3435 2023-07-07 14:51:46.000000 sambacc-0.5/tests/test_passdb_loader.py
+-rw-r--r--   0 root         (0) root         (0)     3653 2023-07-07 14:51:46.000000 sambacc-0.5/tests/test_passwd_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-07-07 14:51:46.000000 sambacc-0.5/tests/test_paths.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-07-07 14:51:46.000000 sambacc-0.5/tests/test_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     7513 2024-01-03 15:06:45.000000 sambacc-0.5/tests/test_rados_opener.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-07-07 14:51:46.000000 sambacc-0.5/tests/test_samba_cmds.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2023-09-15 13:41:12.000000 sambacc-0.5/tests/test_simple_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-08-23 17:28:34.000000 sambacc-0.5/tests/test_smbconf_api.py
+-rw-r--r--   0 root         (0) root         (0)     5531 2023-08-23 17:30:15.000000 sambacc-0.5/tests/test_smbconf_samba.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-11-15 15:05:41.000000 sambacc-0.5/tests/test_url_opener.py
+-rw-r--r--   0 root         (0) root         (0)     2167 2024-03-02 22:12:40.000000 sambacc-0.5/tox.ini
```

### Comparing `sambacc-0.4/.copr/Makefile` & `sambacc-0.5/.copr/Makefile`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/.github/mergify.yml` & `sambacc-0.5/.github/mergify.yml`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # https://docs.mergify.io/conditions.html#validating-all-status-check
 # TODO: Use mergify's recently added 'shared configuration support'
 # to dedup some of the check-x=y repetition in the future.
 queue_rules:
   - name: default
     conditions:
       - check-success=check-commits
-      - check-success=test (fedora-37)
-      - check-success=test (fedora-38)
+      - check-success=test (fedora-39)
+      - check-success=test (fedora-40)
       - check-success=test (centos-stream9)
       - check-success=dpulls
 
 
 pull_request_rules:
   # Clearing approvals after content changes
   - name: Remove outdated approvals
@@ -30,16 +30,16 @@
       dismiss_reviews:
         approved: true
         changes_requested: false
   # Perform automatic merge on conditions
   - name: Automatic merge on approval
     conditions:
       - check-success=check-commits
-      - check-success=test (fedora-37)
-      - check-success=test (fedora-38)
+      - check-success=test (fedora-39)
+      - check-success=test (fedora-40)
       - check-success=test (centos-stream9)
       - check-success=dpulls
       - "-draft"
       # Contributors should set the 'do-not-merge' label if they don't want
       # the PR to be (auto)merged for some reason.
       - "label!=do-not-merge"
       # A reviewer should set a label starting with 'review-in-progress' (and
```

### Comparing `sambacc-0.4/.github/workflows/ci.yml` & `sambacc-0.5/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -10,49 +10,50 @@
     - cron: 1 1 * * *
 
 jobs:
   check-commits:
     runs-on: ubuntu-latest
     if: github.event_name == 'pull_request'
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
           ref: ${{ github.event.pull_request.head.sha }}
       - uses: actions/setup-python@v4
       - name: Install tox
         run: python -m pip install tox
       - name: Run gitlint
         run: tox -e gitlint
   test:
     runs-on: ubuntu-latest
     strategy:
+      fail-fast: false
       matrix:
-        test_distro: ["fedora-37", "fedora-38", "centos-stream9"]
+        test_distro: ["fedora-40", "fedora-39", "centos-stream9"]
         include:
-          - test_distro: "fedora-37"
-            base_image: "registry.fedoraproject.org/fedora:37"
-          - test_distro: "fedora-38"
-            base_image: "registry.fedoraproject.org/fedora:38"
+          - test_distro: "fedora-40"
+            base_image: "registry.fedoraproject.org/fedora:40"
+          - test_distro: "fedora-39"
+            base_image: "registry.fedoraproject.org/fedora:39"
           - test_distro: "centos-stream9"
             base_image: "quay.io/centos/centos:stream9"
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Build test container
         run: docker build -t sambacc:ci-${{ matrix.test_distro }} --build-arg=SAMBACC_BASE_IMAGE=${{ matrix.base_image }}  tests/container/ -f tests/container/Containerfile
       - name: Run test container
         run: docker run -v $PWD:/var/tmp/build/sambacc sambacc:ci-${{ matrix.test_distro }}
 
   push:
     needs: [test]
     runs-on: ubuntu-latest
     if: (github.event_name == 'push' || github.event_name == 'schedule') && github.repository == 'samba-in-kubernetes/sambacc'
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: log in to quay.io
         run: docker login -u "${{ secrets.QUAY_USER }}" -p "${{ secrets.QUAY_PASS }}" quay.io
       - name: build container image
         run: docker build -t quay.io/samba.org/sambacc:latest tests/container -f tests/container/Containerfile
       - name: publish container image
         run: docker push quay.io/samba.org/sambacc:latest
```

### Comparing `sambacc-0.4/.gitlint` & `sambacc-0.5/.gitlint`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/COPYING` & `sambacc-0.5/COPYING`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/PKG-INFO` & `sambacc-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sambacc
-Version: 0.4
+Version: 0.5
 Summary: Samba Container Configurator
 Home-page: https://github.com/samba-in-kubernetes/sambacc
 Author: John Mulligan
 Author-email: phlogistonjohn@asynchrono.us
 License: GPL3
 Description-Content-Type: text/markdown
 License-File: COPYING
```

### Comparing `sambacc-0.4/README.md` & `sambacc-0.5/README.md`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/docs/configuration.md` & `sambacc-0.5/docs/configuration.md`

 * *Files 13% similar despite different names*

```diff
@@ -255,14 +255,43 @@
 instances. The `domain_settings` section contains a mapping of domain
 settings names to a domain-settings configuration block.
 
 Each domain configuration section is as follows:
 * `realm` - Name of the domain in kerberos realm form.
 * `short_domain` - Optional. The short (nt-style) name of the domain.
 * `admin_password` - The default password for the administrator user.
+* `interfaces` - An optional subsection for dynamically configuring the network
+  interfaces the domain controller will use. See below.
+
+#### Interfaces Section
+
+The interfaces section enables the sambacc tool to dynamically configure what
+network interfaces will be enabled when the domain is provisioned.  On some
+systems and in some environments there may be "bogus" network interfaces that
+one does not want to enable the domain controller for. Examples include
+interfaces related to virtualization or container engines that would cause the
+DC to include a private or otherwise inaccessable IP to be included in the DNS
+record(s) for the domain & domain controller.
+
+The loopback device ("lo") is always enabled.
+
+* `include_pattern` - Optional string. A regular expression that must match
+  the name of an interface for that interface to be included.
+  Example: `^eno[0-9]+$`
+* `exclude_pattern` - Optional string. A regular expression that must not
+  match the name of an interface for that interface to be included.
+  The `exclude_pattern` option takes precedence over the `include_pattern`
+  option.
+  Example: `^(docker|virbr)[0-9]+$`
+
+These options are intended to automate the act of examining a host's interfaces
+prior to deployment and creating a list of suitable interfaces prior to setting
+the "interfaces" and "bind interfaces only" parameters.  See the [Samba
+Wiki page](https://wiki.samba.org/index.php/Setting_up_Samba_as_an_Active_Directory_Domain_Controller#Parameter_Reference)
+for more details on this operation.
 
 
 ## Domain Groups Section
 
 The `domain_groups` section defines initial groups that will be
 automatically added to a newly provisioned domain. This section
 is a mapping of the domain settings name to a list of domain group
```

### Comparing `sambacc-0.4/docs/release-process.md` & `sambacc-0.5/docs/release-process.md`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/examples/addc.json` & `sambacc-0.5/examples/addc.json`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/examples/ctdb.json` & `sambacc-0.5/examples/ctdb.json`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/examples/example1.json` & `sambacc-0.5/examples/example1.json`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/examples/minimal.json` & `sambacc-0.5/examples/minimal.json`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/extras/python-sambacc.spec` & `sambacc-0.5/extras/python-sambacc.spec`

 * *Files 17% similar despite different names*

```diff
@@ -36,20 +36,24 @@
 %description %_description
 
 %package -n python3-%{bname}
 Summary: %{summary}
 # Distro requires that are technically optional for the lib
 Requires: python3-samba
 Requires: python3-pyxattr
-%if 0%{?fedora} >= 37
+%if 0%{?fedora} >= 37 || 0%{?rhel} >= 9
+# Enable extras other than validation as the dependency needed
+# is too old on centos/rhel 9.
 Recommends: %{name}+toml
-Recommends: %{name}+validation
 Recommends: %{name}+yaml
 Recommends: %{name}+rados
 %endif
+%if 0%{?fedora} >= 37
+Recommends: %{name}+validation
+%endif
 
 %description -n python3-%{bname}  %_description
 
 
 %prep
 %autosetup -n %{bname}-%{pversion}
```

### Comparing `sambacc-0.4/pyproject.toml` & `sambacc-0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/_xattr.py` & `sambacc-0.5/sambacc/_xattr.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/addc.py` & `sambacc-0.5/sambacc/addc.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 #
 
 import logging
+import re
 import subprocess
 import typing
 
+from sambacc import config
 from sambacc import samba_cmds
 
 _logger = logging.getLogger(__name__)
 
 
 def provision(
     realm: str,
@@ -71,26 +73,33 @@
 
 
 def create_user(
     name: str,
     password: str,
     surname: typing.Optional[str],
     given_name: typing.Optional[str],
+    ou: typing.Optional[str] = None,
 ) -> None:
-    cmd = _user_create_cmd(name, password, surname, given_name)
+    cmd = _user_create_cmd(name, password, surname, given_name, ou)
     _logger.info("Creating user: %r", name)
     subprocess.check_call(cmd)
 
 
-def create_group(name: str) -> None:
-    cmd = _group_add_cmd(name)
+def create_group(name: str, ou: typing.Optional[str] = None) -> None:
+    cmd = _group_add_cmd(name, ou)
     _logger.info("Creating group: %r", name)
     subprocess.check_call(cmd)
 
 
+def create_ou(name: str) -> None:
+    cmd = _ou_add_cmd(name)
+    _logger.info("Creating organizational unit: %r", name)
+    subprocess.check_call(cmd)
+
+
 def add_group_members(group_name: str, members: list[str]) -> None:
     cmd = _group_add_members_cmd(group_name, members)
     _logger.info("Adding group members: %r", cmd)
     subprocess.check_call(cmd)
 
 
 def _filter_opts(
@@ -159,38 +168,73 @@
 
 
 def _user_create_cmd(
     name: str,
     password: str,
     surname: typing.Optional[str],
     given_name: typing.Optional[str],
+    ou: typing.Optional[str],
 ) -> list[str]:
     cmd = samba_cmds.sambatool[
         "user",
         "create",
         name,
         password,
     ].argv()
     if surname:
         cmd.append(f"--surname={surname}")
     if given_name:
         cmd.append(f"--given-name={given_name}")
+    if ou:
+        cmd.append(f"--userou=OU={ou}")
     return cmd
 
 
-def _group_add_cmd(name: str) -> list[str]:
+def _group_add_cmd(name: str, ou: typing.Optional[str]) -> list[str]:
     cmd = samba_cmds.sambatool[
         "group",
         "add",
         name,
     ].argv()
+    if ou:
+        cmd.append(f"--groupou=OU={ou}")
+    return cmd
+
+
+def _ou_add_cmd(name: str) -> list[str]:
+    cmd = samba_cmds.sambatool[
+        "ou",
+        "add",
+        f"OU={name}",
+    ].argv()
     return cmd
 
 
 def _group_add_members_cmd(group_name: str, members: list[str]) -> list[str]:
     cmd = samba_cmds.sambatool[
         "group",
         "addmembers",
         group_name,
         ",".join(members),
     ].argv()
     return cmd
+
+
+def _ifnames() -> list[str]:
+    import socket
+
+    return [iface for _, iface in socket.if_nameindex()]
+
+
+def filtered_interfaces(
+    ic: config.DCInterfaceConfig, ifnames: typing.Optional[list[str]] = None
+) -> list[str]:
+    _include = re.compile(ic.include_pattern or "^.*$")
+    _exclude = re.compile(ic.exclude_pattern or "^$")
+    if ifnames is None:
+        ifnames = _ifnames()
+    return [
+        name
+        for name in ifnames
+        if (name == "lo")
+        or (_include.match(name) and not _exclude.match(name))
+    ]
```

### Comparing `sambacc-0.4/sambacc/commands/addc.py` & `sambacc-0.5/sambacc/commands/addc.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,20 +80,30 @@
     if os.path.exists(_provisioned):
         _logger.info("Domain already provisioned")
         return
     domconfig = ctx.instance_config.domain()
     _logger.info(f"Provisioning domain: {domconfig.realm}")
 
     dcname = ctx.cli.name or domconfig.dcname
+    prov_opts = list(ctx.instance_config.global_options())
+    explicit_ifaces = "interfaces" in dict(prov_opts)
+    if domconfig.interface_config.configured and not explicit_ifaces:
+        # dynamically select interfaces from the system to pass to the
+        # provisioning command
+        _logger.info("Dynamic interface selection enabled")
+        ifaces = addc.filtered_interfaces(domconfig.interface_config)
+        _logger.info("Selected interfaces: %s", ifaces)
+        prov_opts.append(("interfaces", " ".join(ifaces)))
+        prov_opts.append(("bind interfaces only", "yes"))
     addc.provision(
         realm=domconfig.realm,
         domain=domconfig.short_domain,
         dcname=dcname,
         admin_password=domconfig.admin_password,
-        options=ctx.instance_config.global_options(),
+        options=prov_opts,
     )
     _merge_config(_provisioned, ctx.instance_config.global_options())
 
 
 def _prep_join(ctx: Context) -> None:
     if os.path.exists(_provisioned):
         _logger.info("Already configured. Not joining")
@@ -151,23 +161,27 @@
 
 def _prep_populate(ctx: Context) -> None:
     if os.path.exists(_populated):
         _logger.info("populated marker exists")
         return
     _logger.info("Populating domain with default entries")
 
+    for ou in ctx.instance_config.organizational_units():
+        addc.create_ou(ou.ou_name)
+
     for dgroup in ctx.instance_config.domain_groups():
-        addc.create_group(dgroup.groupname)
+        addc.create_group(dgroup.groupname, dgroup.ou)
 
     for duser in ctx.instance_config.domain_users():
         addc.create_user(
             name=duser.username,
             password=duser.plaintext_passwd,
             surname=duser.surname,
             given_name=duser.given_name,
+            ou=duser.ou,
         )
         # TODO: probably should improve this to avoid extra calls / loops
         for gname in duser.member_of:
             addc.add_group_members(group_name=gname, members=[duser.username])
 
     # "touch" the populated marker
     with open(_populated, "w"):
```

### Comparing `sambacc-0.4/sambacc/commands/check.py` & `sambacc-0.5/sambacc/commands/check.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/commands/cli.py` & `sambacc-0.5/sambacc/commands/cli.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/commands/config.py` & `sambacc-0.5/sambacc/commands/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,22 +62,24 @@
     loader.import_config(ctx.instance_config)
 
 
 def _update_config_args(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "--watch",
         action="store_true",
-        help=("If set, watch the source for changes and update config."),
+        help="If set, watch the source for changes and update config.",
     )
 
 
 def _read_config(ctx: Context) -> config.InstanceConfig:
     cfgs = ctx.cli.config or []
     return config.read_config_files(
-        cfgs, require_validation=ctx.require_validation
+        cfgs,
+        require_validation=ctx.require_validation,
+        opener=ctx.opener,
     ).get(ctx.cli.identity)
 
 
 def _update_config(
     current: config.InstanceConfig,
     previous: typing.Optional[config.InstanceConfig],
     ensure_paths: bool = True,
```

### Comparing `sambacc-0.4/sambacc/commands/ctdb.py` & `sambacc-0.5/sambacc/commands/ctdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,50 +53,50 @@
     raise Fail(gate)
 
 
 def _ctdb_migrate_args(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "--dest-dir",
         default=ctdb.DB_DIR,
-        help=("Specify where CTDB database files will be written."),
+        help="Specify where CTDB database files will be written.",
     )
 
 
 def _ctdb_general_node_args(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "--hostname",
-        help=("Specify the host name for the CTDB node"),
+        help="Specify the host name for the CTDB node",
     )
     parser.add_argument(
         "--node-number",
         type=int,
-        help=("Expected node number"),
+        help="Expected node number",
     )
     # This is a choice with a single acceptable param, rather than an on/off
     # bool, # in the case that other container orchs have a similar but not
     # quite the same issue and we want to support a different scheme someday.
     parser.add_argument(
         "--take-node-number-from-hostname",
         choices=(_AFTER_LAST_DASH,),
         help=(
             "Take the node number from the given host name following"
             " the specified policy."
         ),
     )
     parser.add_argument(
         "--persistent-path",
-        help=("Path to a persistent path for storing nodes file"),
+        help="Path to a persistent path for storing nodes file",
     )
 
 
 def _ctdb_set_node_args(parser: argparse.ArgumentParser) -> None:
     _ctdb_general_node_args(parser)
     parser.add_argument(
         "--ip",
-        help=("Specify node by IP"),
+        help="Specify node by IP",
     )
 
 
 class NodeParams:
     _ctx: Context
     node_number: typing.Optional[int] = None
     hostname: typing.Optional[str] = None
```

### Comparing `sambacc-0.4/sambacc/commands/dcmain.py` & `sambacc-0.5/sambacc/commands/dcmain.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/commands/dns.py` & `sambacc-0.5/sambacc/commands/dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,26 @@
 _logger = logging.getLogger(__name__)
 
 
 def _dns_register_args(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "--watch",
         action="store_true",
-        help=("If set, watch the source for changes and update DNS."),
+        help="If set, watch the source for changes and update DNS.",
     )
     parser.add_argument(
         "--domain",
         default="",
-        help=("Manually specify parent domain for DNS entries."),
+        help="Manually specify parent domain for DNS entries.",
     )
     parser.add_argument(
         "--target",
         default=container_dns.EXTERNAL,
         choices=[container_dns.EXTERNAL, container_dns.INTERNAL],
-        help=("Register IPs that fulfill the given access target."),
+        help="Register IPs that fulfill the given access target.",
     )
     parser.add_argument("source", help="Path to source JSON file.")
 
 
 @commands.command(name="dns-register", arg_func=_dns_register_args)
 def dns_register(ctx: Context) -> None:
     """Register container & container orchestration IPs with AD DNS."""
```

### Comparing `sambacc-0.4/sambacc/commands/initialize.py` & `sambacc-0.5/sambacc/commands/initialize.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/commands/join.py` & `sambacc-0.5/sambacc/commands/join.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/commands/main.py` & `sambacc-0.5/sambacc/commands/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -97,23 +97,85 @@
     parser.add_argument(
         "--samba-command-prefix",
         help="Wrap samba commands within a supplied command prefix",
     )
     parser.add_argument(
         "--skip-if-file",
         action="append",
-        help=("Perform no action if the specified path exists."),
+        help="Perform no action if the specified path exists.",
     )
     parser.add_argument(
         "--validate-config",
         choices=("auto", "required", "true", "false"),
-        help=("Perform schema based validation of configuration."),
+        help="Perform schema based validation of configuration.",
+    )
+    parser.add_argument(
+        "--ceph-id",
+        type=_ceph_id,
+        help=(
+            "Specify a user/client ID to ceph libraries"
+            "(can also be set in the environment by SAMBACC_CEPH_ID."
+            " Ignored if Ceph RADOS libraries are not present or unused."
+            " Pass `?` for more details)."
+        ),
+    )
+    parser.add_argument(
+        "--debug",
+        action="store_true",
+        help="Enable debug level logging of sambacc.",
     )
 
 
+def _ceph_id(
+    value: typing.Union[str, dict[str, typing.Any]]
+) -> dict[str, typing.Any]:
+    if not isinstance(value, str):
+        return value
+    if value == "?":
+        # A hack to avoid putting tons of ceph specific info in the normal
+        # help output. There's probably a better way to do this but it
+        # gets the job done for now.
+        raise argparse.ArgumentTypeError(
+            "requested help:"
+            " Specify names in the form"
+            " --ceph-id=[key=value][,key=value][,...]."
+            ' Valid keys include "name" to set the exact name and "rados_id"'
+            ' to specify a name that lacks the "client." prefix (that will'
+            "automatically get added)."
+            " Alternatively, specify just the name to allow the system to"
+            " guess if the name is prefixed already or not."
+        )
+    result: dict[str, typing.Any] = {}
+    # complex mode
+    if "=" in value:
+        for part in value.split(","):
+            if "=" not in part:
+                raise argparse.ArgumentTypeError(
+                    f"unexpected value for ceph-id: {value!r}"
+                )
+            key, val = part.split("=", 1)
+            if key == "name":
+                result["client_name"] = val
+                result["full_name"] = True
+            elif key == "rados_id":
+                result["client_name"] = val
+                result["full_name"] = False
+            else:
+                b = f"unexpected key {key!r} in value for ceph-id: {value!r}"
+                raise argparse.ArgumentTypeError(b)
+    else:
+        # this shorthand is meant mainly for lazy humans (me) when running test
+        # images manually. The key-value form above is meant for automation.
+        result["client_name"] = value
+        # assume that if the name starts with client. it's the full name and
+        # avoid having the ceph library double up an create client.client.x.
+        result["full_name"] = value.startswith("client.")
+    return result
+
+
 def from_env(
     ns: typing.Any,
     var: str,
     ename: str,
     default: typing.Any = None,
     convert_env: typing.Optional[typing.Callable] = None,
     convert_value: typing.Optional[typing.Callable] = str,
@@ -169,14 +231,15 @@
         convert_value=None,
     )
     from_env(cli, "identity", "SAMBA_CONTAINER_ID")
     from_env(cli, "username", "JOIN_USERNAME")
     from_env(cli, "password", "INSECURE_JOIN_PASSWORD")
     from_env(cli, "samba_debug_level", "SAMBA_DEBUG_LEVEL")
     from_env(cli, "validate_config", "SAMBACC_VALIDATE_CONFIG")
+    from_env(cli, "ceph_id", "SAMBACC_CEPH_ID", convert_value=_ceph_id)
 
 
 class CommandContext:
     """CLI Context for standard samba-container commands."""
 
     def __init__(self, cli_args: argparse.Namespace):
         self._cli = cli_args
@@ -223,25 +286,30 @@
     if cli.samba_debug_level:
         samba_cmds.set_global_debug(cli.samba_debug_level)
     if cli.samba_command_prefix:
         samba_cmds.set_global_prefix([cli.samba_command_prefix])
 
     # should there be an option to force {en,dis}able openers?
     # Right now we just always try to enable rados when possible.
-    rados_opener.enable_rados_url_opener(url_opener.URLOpener)
+    rados_opener.enable_rados_url_opener(
+        url_opener.URLOpener,
+        client_name=cli.ceph_id.get("client_name", ""),
+        full_name=cli.ceph_id.get("full_name", False),
+    )
 
 
 def enable_logging(cli: typing.Any) -> None:
+    level = logging.DEBUG if cli.debug else logging.INFO
     logger = logging.getLogger()
-    logger.setLevel(logging.INFO)
+    logger.setLevel(level)
     handler = logging.StreamHandler()
     handler.setFormatter(
         logging.Formatter("{asctime}: {levelname}: {message}", style="{")
     )
-    handler.setLevel(logging.INFO)
+    handler.setLevel(level)
     logger.addHandler(handler)
 
 
 def action_filter(cli: typing.Any) -> typing.Optional[str]:
     for path in cli.skip_if_file or []:
         if os.path.exists(path):
             return f"skip-if-file: {path} exists"
```

### Comparing `sambacc-0.4/sambacc/commands/run.py` & `sambacc-0.5/sambacc/commands/run.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/commands/users.py` & `sambacc-0.5/sambacc/commands/users.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/config.py` & `sambacc-0.5/sambacc/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -333,14 +333,24 @@
         if not self.with_addc:
             raise ValueError("ad dc not supported by configuration")
         ds_name: str = self.iconfig["domain_settings"]
         dgroups = self.gconfig.data.get("domain_groups", {}).get(ds_name, [])
         for n, entry in enumerate(dgroups):
             yield DomainGroupEntry(self, entry, n)
 
+    def organizational_units(self) -> typing.Iterable[OrganizationalUnitEntry]:
+        if not self.with_addc:
+            raise ValueError("ad dc not supported by configuration")
+        ds_name: str = self.iconfig["domain_settings"]
+        o_units = self.gconfig.data.get("organizational_units", {}).get(
+            ds_name, []
+        )
+        for n, entry in enumerate(o_units):
+            yield OrganizationalUnitEntry(self, entry, n)
+
     def __eq__(self, other: typing.Any) -> bool:
         if isinstance(other, InstanceConfig) and self.iconfig == other.iconfig:
             self_shares = _shares_data(self.gconfig, self.iconfig)
             other_shares = _shares_data(other.gconfig, other.iconfig)
             self_globals = _globals_data(self.gconfig, self.iconfig)
             other_globals = _globals_data(other.gconfig, other.iconfig)
             return (
@@ -472,14 +482,15 @@
 
 class GroupEntry:
     def __init__(self, iconf: InstanceConfig, grec: dict, num: int):
         self.iconfig = iconf
         self.groupname = grec["name"]
         self.entry_num = num
         self._gid = grec.get("gid")
+        self.ou = grec.get("ou")
         if self._gid is not None:
             if not isinstance(self._gid, int):
                 raise ValueError("invalid gid value")
 
     @property
     def gid(self) -> int:
         if self._gid:
@@ -492,31 +503,51 @@
 
 
 class DomainConfig:
     def __init__(self, drec: dict, instance_name: str):
         self.realm = drec["realm"]
         self.short_domain = drec.get("short_domain", "")
         self.admin_password = drec.get("admin_password", "")
+        self.interface_config = DCInterfaceConfig(drec.get("interfaces", {}))
         self.dcname = instance_name
 
 
+class DCInterfaceConfig:
+    def __init__(self, iface_config: dict) -> None:
+        self.include_pattern: str = iface_config.get("include_pattern", "")
+        self.exclude_pattern: str = iface_config.get("exclude_pattern", "")
+
+    @property
+    def configured(self) -> bool:
+        """Return true if at least one interface property has been set."""
+        return bool(self.include_pattern) or bool(self.exclude_pattern)
+
+
 class DomainUserEntry(UserEntry):
     def __init__(self, iconf: InstanceConfig, urec: dict, num: int):
         super().__init__(iconf, urec, num)
         self.surname = urec.get("surname")
         self.given_name = urec.get("given_name")
         self.member_of = urec.get("member_of", [])
+        self.ou = urec.get("ou")
         if not isinstance(self.member_of, list):
             raise ValueError("member_of should contain a list of group names")
 
 
 class DomainGroupEntry(GroupEntry):
     pass
 
 
+class OrganizationalUnitEntry:
+    def __init__(self, iconf: InstanceConfig, urec: dict, num: int):
+        self.iconfig = iconf
+        self.ou_name = urec["name"]
+        self.entry_num = num
+
+
 class PermissionsConfig:
     _method_key: str = "method"
     _status_xattr_key: str = "status_xattr"
     _default_method: str = "none"
     _default_status_xattr: str = "user.share-perms-status"
 
     def __init__(self, pconf: dict[str, str]) -> None:
```

### Comparing `sambacc-0.4/sambacc/container_dns.py` & `sambacc-0.5/sambacc/container_dns.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/ctdb.py` & `sambacc-0.5/sambacc/ctdb.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/inotify_waiter.py` & `sambacc-0.5/sambacc/inotify_waiter.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/jfile.py` & `sambacc-0.5/sambacc/jfile.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/join.py` & `sambacc-0.5/sambacc/join.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/leader.py` & `sambacc-0.5/sambacc/leader.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/netcmd_loader.py` & `sambacc-0.5/sambacc/netcmd_loader.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/nsswitch_loader.py` & `sambacc-0.5/sambacc/nsswitch_loader.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/opener.py` & `sambacc-0.5/sambacc/opener.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/passdb_loader.py` & `sambacc-0.5/sambacc/passdb_loader.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/passwd_loader.py` & `sambacc-0.5/sambacc/passwd_loader.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/paths.py` & `sambacc-0.5/sambacc/paths.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/permissions.py` & `sambacc-0.5/sambacc/permissions.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/rados_opener.py` & `sambacc-0.5/sambacc/rados_opener.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,62 +14,90 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 #
 
 from __future__ import annotations
 
+import io
+import json
+import logging
 import typing
 import urllib.request
 
 from . import url_opener
 from .typelets import ExcType, ExcValue, ExcTraceback
 
 _RADOSModule = typing.Any
+_RADOSObject = typing.Any
 
 _CHUNK_SIZE = 4 * 1024
 
+_logger = logging.getLogger(__name__)
+
 
 class RADOSUnsupported(Exception):
     pass
 
 
+class _RADOSInterface:
+    api: _RADOSModule
+    client_name: str
+    full_name: bool
+
+    def Rados(self) -> _RADOSObject:
+        name = rados_id = ""
+        if self.full_name:
+            name = self.client_name
+        else:
+            rados_id = self.client_name
+        _logger.debug("Creating RADOS connection")
+        return self.api.Rados(
+            name=name,
+            rados_id=rados_id,
+            conffile=self.api.Rados.DEFAULT_CONF_FILES,
+        )
+
+
 class _RADOSHandler(urllib.request.BaseHandler):
-    _rados_api: typing.Optional[_RADOSModule] = None
+    _interface: typing.Optional[_RADOSInterface] = None
 
     def rados_open(self, req: urllib.request.Request) -> typing.IO:
-        if self._rados_api is None:
+        if self._interface is None:
             raise RADOSUnsupported()
+        if req.selector.startswith("mon-config-key:"):
+            return _get_mon_config_key(
+                self._interface, req.selector.split(":", 1)[1]
+            )
         sel = req.selector.lstrip("/")
         if req.host:
             pool = req.host
             ns, key = sel.split("/", 1)
         else:
             pool, ns, key = sel.split("/", 2)
-        return _RADOSResponse(self._rados_api, pool, ns, key)
+        return _RADOSResponse(self._interface, pool, ns, key)
 
 
 # it's quite annoying to have a read-only typing.IO we're forced to
 # have so many stub methods. Go's much more granular io interfaces for
 # readers/writers is much nicer for this.
 class _RADOSResponse(typing.IO):
     def __init__(
-        self, rados_api: _RADOSModule, pool: str, ns: str, key: str
+        self, interface: _RADOSInterface, pool: str, ns: str, key: str
     ) -> None:
         self._pool = pool
         self._ns = ns
         self._key = key
 
-        self._open(rados_api)
+        self._open(interface)
         self._test()
 
-    def _open(self, rados_api: _RADOSModule) -> None:
+    def _open(self, interface: _RADOSInterface) -> None:
         # TODO: connection caching
-        self._conn = rados_api.Rados()
-        self._conn.conf_read_file()
+        self._conn = interface.Rados()
         self._conn.connect()
         self._connected = True
         self._ioctx = self._conn.open_ioctx(self._pool)
         self._ioctx.set_namespace(self._ns)
         self._closed = False
         self._offset = 0
 
@@ -167,24 +195,58 @@
     def write(self, s: typing.Any) -> int:
         raise NotImplementedError()
 
     def writelines(self, ls: typing.Iterable[typing.Any]) -> None:
         raise NotImplementedError()
 
 
-def enable_rados_url_opener(cls: typing.Type[url_opener.URLOpener]) -> None:
+def _get_mon_config_key(interface: _RADOSInterface, key: str) -> io.BytesIO:
+    mcmd = json.dumps(
+        {
+            "prefix": "config-key get",
+            "key": str(key),
+        }
+    )
+    with interface.Rados() as rc:
+        ret, out, err = rc.mon_command(mcmd, b"")
+        if ret == 0:
+            # We need to return a file like object. Since we are handed just
+            # bytes from this api, use BytesIO to adapt it to something valid.
+            return io.BytesIO(out)
+        # ensure ceph didn't send us a negative errno
+        ret = ret if ret > 0 else -ret
+        msg = f"failed to get mon config key: {key!r}: {err}"
+        raise OSError(ret, msg)
+
+
+def enable_rados_url_opener(
+    cls: typing.Type[url_opener.URLOpener],
+    *,
+    client_name: str = "",
+    full_name: bool = False,
+) -> None:
     """Extend the URLOpener type to support pseudo-URLs for rados
     object storage. If rados libraries are not found the function
     does nothing.
 
     If rados libraries are found than URLOpener can be used like:
     >>> uo = url_opener.URLOpener()
     >>> res = uo.open("rados://my_pool/namepace/obj_key")
     >>> res.read()
     """
     try:
         import rados  # type: ignore[import]
     except ImportError:
+        _logger.debug("Failed to import ceph 'rados' module")
         return
 
-    _RADOSHandler._rados_api = rados
+    _logger.debug(
+        "Enabling ceph rados support with"
+        f" client_name={client_name!r}, full_name={full_name}"
+    )
+    rados_interface = _RADOSInterface()
+    rados_interface.api = rados
+    rados_interface.client_name = client_name
+    rados_interface.full_name = full_name
+
+    _RADOSHandler._interface = rados_interface
     cls._handlers.append(_RADOSHandler)
```

### Comparing `sambacc-0.4/sambacc/samba_cmds.py` & `sambacc-0.5/sambacc/samba_cmds.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         if self.debug:
             return [dlvl.format(self.debug)]
         if _GLOBAL_DEBUG:
             return [dlvl.format(_GLOBAL_DEBUG)]
         return []
 
     def raw_args(self) -> list[str]:
-        return [self._name] + self._debug_args() + self.args
+        return [self._name] + self.args + self._debug_args()
 
     def __repr__(self) -> str:
         return "SambaCommand({!r}, {!r}, {!r})".format(
             self._name, self.args, self.debug
         )
 
 
@@ -168,15 +168,15 @@
 def winbindd_foreground() -> SambaCommand:
     return winbindd[
         "--foreground", _daemon_stdout_opt("winbindd"), "--no-process-group"
     ]
 
 
 def samba_dc_foreground() -> SambaCommand:
-    return samba_dc["--foreground"]
+    return samba_dc["--foreground", _daemon_stdout_opt("samba")]
 
 
 ctdbd = SambaCommand("/usr/sbin/ctdbd")
 
 ctdbd_foreground = ctdbd["--interactive"]
 
 ltdbtool = CommandArgs("ltdbtool")
```

### Comparing `sambacc-0.4/sambacc/schema/conf-v0.schema.json` & `sambacc-0.5/sambacc/schema/conf-v0.schema.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874088980078565%*

 * *Differences: {"'$defs'": "{'user_entry': {'description': 'A user that will be instantiated in the local "*

 * *            "container environment to\\nin order to provide access to smb shares.\\n'}, "*

 * *            "'group_entry': {'description': 'A group that will be instantiated in the local "*

 * *            "container environment to\\nin order to provide access to smb shares.\\n'}, "*

 * *            "'domain_user_entry': {'properties': {'ou': OrderedDict([('description', 'A "*

 * *            "organizational unit that the user should b […]*

```diff
@@ -6,14 +6,18 @@
             "properties": {
                 "gid": {
                     "type": "integer"
                 },
                 "name": {
                     "description": "The group name",
                     "type": "string"
+                },
+                "ou": {
+                    "description": "A organizational unit that the user should belong to",
+                    "type": "string"
                 }
             },
             "required": [
                 "name"
             ],
             "type": "object"
         },
@@ -38,14 +42,18 @@
                 "name": {
                     "description": "The user's name",
                     "type": "string"
                 },
                 "nt_hash": {
                     "type": "string"
                 },
+                "ou": {
+                    "description": "A organizational unit that the user should belong to",
+                    "type": "string"
+                },
                 "password": {
                     "description": "A plain-text password",
                     "type": "string"
                 },
                 "surname": {
                     "description": "A surname for the user",
                     "type": "string"
@@ -67,15 +75,15 @@
                     "ctdb"
                 ]
             },
             "type": "array"
         },
         "group_entry": {
             "additionalProperties": false,
-            "description": "A group that will be instantiated in the local contianer environment to\nin order to provide access to smb shares.\n",
+            "description": "A group that will be instantiated in the local container environment to\nin order to provide access to smb shares.\n",
             "properties": {
                 "gid": {
                     "description": "The Unix GID the group should have",
                     "type": "integer"
                 },
                 "name": {
                     "description": "The group name",
@@ -83,14 +91,28 @@
                 }
             },
             "required": [
                 "name"
             ],
             "type": "object"
         },
+        "organizational_unit_entry": {
+            "additionalProperties": false,
+            "description": "A organizational unit that will be created in the specified AD domain. These\ngroups are populated in the directory after the domain is provisioned.\n",
+            "properties": {
+                "name": {
+                    "description": "The organizational unit name",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "name"
+            ],
+            "type": "object"
+        },
         "permissions_config": {
             "additionalProperties": {
                 "type": "string"
             },
             "description": "Settings that enable and manage sambacc's permissions management support.\n",
             "properties": {
                 "method": {
@@ -116,15 +138,15 @@
             "items": {
                 "type": "string"
             },
             "type": "array"
         },
         "user_entry": {
             "additionalProperties": false,
-            "description": "A user that will be instantiated in the local contianer environment to\nin order to provide access to smb shares.\n",
+            "description": "A user that will be instantiated in the local container environment to\nin order to provide access to smb shares.\n",
             "properties": {
                 "gid": {
                     "description": "The Unix GID the user should have",
                     "type": "integer"
                 },
                 "name": {
                     "description": "The user's name",
@@ -180,15 +202,15 @@
                     },
                     "shares": {
                         "$ref": "#/$defs/section_choices"
                     }
                 },
                 "type": "object"
             },
-            "description": "A mapping of named configurations (instances) to top-level configuration\nblocks. A useable configuration file must have at least one configuration,\nbut more than one is supported.\n",
+            "description": "A mapping of named configurations (instances) to top-level configuration\nblocks. A usable configuration file must have at least one configuration,\nbut more than one is supported.\n",
             "title": "Container Configurations",
             "type": "object"
         },
         "ctdb": {
             "additionalProperties": {
                 "type": "string"
             },
@@ -207,14 +229,27 @@
         "domain_settings": {
             "additionalProperties": {
                 "additionalProperties": false,
                 "properties": {
                     "admin_password": {
                         "type": "string"
                     },
+                    "interfaces": {
+                        "properties": {
+                            "exclude_pattern": {
+                                "description": "A regular expression that must not match for a network interface\nto be included in the AD DC interfaces list.\n",
+                                "type": "string"
+                            },
+                            "include_pattern": {
+                                "description": "A regular expression that must match for a network interface\nto be included in the AD DC interfaces list.\n",
+                                "type": "string"
+                            }
+                        },
+                        "type": "object"
+                    },
                     "realm": {
                         "type": "string"
                     },
                     "short_domain": {
                         "type": "string"
                     }
                 },
@@ -242,32 +277,42 @@
                 "properties": {
                     "options": {
                         "$ref": "#/$defs/samba_options"
                     }
                 },
                 "type": "object"
             },
-            "description": "A mapping of samba global configuation blocks. The global section names\nare not passed to Samba. All sections selected by a configuration are\nmerged together before passing to Samba.\n",
+            "description": "A mapping of samba global configuration blocks. The global section names\nare not passed to Samba. All sections selected by a configuration are\nmerged together before passing to Samba.\n",
             "type": "object"
         },
         "groups": {
-            "description": "Groups to add to the container environment in order to provide\nShare access-control wihout becoming a domain member server.\n",
+            "description": "Groups to add to the container environment in order to provide\nShare access-control without becoming a domain member server.\n",
             "properties": {
                 "all_entries": {
                     "items": {
                         "$ref": "#/$defs/group_entry"
                     },
                     "type": "array"
                 }
             },
             "type": "object"
         },
+        "organizational_units": {
+            "additionalProperties": {
+                "items": {
+                    "$ref": "#/$defs/organizational_unit_entry"
+                },
+                "type": "array"
+            },
+            "description": "The organizational_unit section defines initial organizational unit that will be\nautomatically added to a newly provisioned domain. This section is\na mapping of the domain settings name to a list of domain group entries.\n",
+            "type": "object"
+        },
         "samba-container-config": {
             "description": "A short version string that assists in allowing the configuration\nformat to (some day) support incompatible version changes.\n(It is unique to the configuration and is not the version of sambacc)\n",
-            "title": "Cofiguration Format Version",
+            "title": "Configuration Format Version",
             "type": "string"
         },
         "shares": {
             "additionalProperties": {
                 "additionalProperties": false,
                 "properties": {
                     "options": {
@@ -279,15 +324,15 @@
                 },
                 "type": "object"
             },
             "description": "A mapping of share name to share specific configuration. A share can\nhave \"options\" that are passed to Samba. Shares can have an optional\n\"permissions\" section for managing permissions/acls in sambacc.\n",
             "type": "object"
         },
         "users": {
-            "description": "Users to add to the container environment in order to provide\nShare access-control wihout becoming a domain member server.\n",
+            "description": "Users to add to the container environment in order to provide\nShare access-control without becoming a domain member server.\n",
             "properties": {
                 "all_entries": {
                     "items": {
                         "$ref": "#/$defs/user_entry"
                     },
                     "type": "array"
                 }
```

### Comparing `sambacc-0.4/sambacc/schema/conf-v0.schema.yaml` & `sambacc-0.5/sambacc/schema/conf-v0.schema.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ---
 # EDIT THIS FILE
 # When you are done editing this YAML representation, convert it into
 # a matching <name>.json file in the same directory. That file exists
-# for jsonschema implmenations that can't read directly from YAML.
+# for jsonschema implementations that can't read directly from YAML.
 #
-# After edting this file, generated files need to be updated.
+# After editing this file, generated files need to be updated.
 # Run: python -m sambacc.schema.tool --update
 #
 $schema:  "http://json-schema.org/draft-07/schema#"
 $id: "mailto:phlogistonjohn+sambacc-v0@asynchrono.us"
 title: "sambacc configuration"
 description: |
   The configuration for the sambacc tool. sambacc configures Samba and the container
@@ -41,15 +41,15 @@
     description: |
       A mapping of values that will be passed into the smb.conf (or equivalent)
       to directly configure Samba.
     type: object
     additionalProperties:
       type: string
   # permissions backend configurations
-  # each backend may have it's own set of additional properties
+  # each backend may have its own set of additional properties
   permissions_config:
     description: |
       Settings that enable and manage sambacc's permissions management support.
     type: object
     properties:
       method:
         description: Backend method for controlling permissions on shares
@@ -58,15 +58,15 @@
         description: xattr name used to store permissions state
         type: string
     additionalProperties:
       type: string
   # file server user entries
   user_entry:
     description: |
-      A user that will be instantiated in the local contianer environment to
+      A user that will be instantiated in the local container environment to
       in order to provide access to smb shares.
     type: object
     properties:
       name:
         description: The user's name
         type: string
       uid:
@@ -83,15 +83,15 @@
         type: string
     required:
       - name
     additionalProperties: false
   # file server group entries
   group_entry:
     description: |
-      A group that will be instantiated in the local contianer environment to
+      A group that will be instantiated in the local container environment to
       in order to provide access to smb shares.
     type: object
     properties:
       name:
         description: The group name
         type: string
       gid:
@@ -121,14 +121,17 @@
       gid:
         type: integer
       nt_hash:
         type: string
       password:
         description: A plain-text password
         type: string
+      ou:
+        description: A organizational unit that the user should belong to
+        type: string
       member_of:
         description: A list of group names that the user should belong to
         type: array
         items:
           type: string
     required:
       - name
@@ -141,34 +144,50 @@
     type: object
     properties:
       name:
         description: The group name
         type: string
       gid:
         type: integer
+      ou:
+        description: A organizational unit that the user should belong to
+        type: string
+    required:
+      - name
+    additionalProperties: false
+  # domain controller organizational unit entries
+  organizational_unit_entry:
+    description: |
+      A organizational unit that will be created in the specified AD domain. These
+      groups are populated in the directory after the domain is provisioned.
+    type: object
+    properties:
+      name:
+        description: The organizational unit name
+        type: string
     required:
       - name
     additionalProperties: false
 properties:
   samba-container-config:
     type: "string"
-    title: "Cofiguration Format Version"
+    title: "Configuration Format Version"
     description: |
       A short version string that assists in allowing the configuration
       format to (some day) support incompatible version changes.
       (It is unique to the configuration and is not the version of sambacc)
   # top-level configuration section. each subsection is an "instance" -
   # a single server or a group of servers acting as one unit.
   # You can store multiple instance configurations in a single config and
   # use the sambacc --identity/SAMBA_CONTAINER_ID to select between them.
   configs:
     title: "Container Configurations"
     description: |
       A mapping of named configurations (instances) to top-level configuration
-      blocks. A useable configuration file must have at least one configuration,
+      blocks. A usable configuration file must have at least one configuration,
       but more than one is supported.
     type: object
     additionalProperties:
       type: object
       properties:
         shares:
           $ref: "#/$defs/section_choices"
@@ -183,33 +202,33 @@
             A name that will be set for the server instance.
           type: string
         domain_settings:
           description: |
             The name of the domain settings. Only used with 'ADDC' feature flag.
           type: string
       additionalProperties: false
-  # share defintions.
+  # share definitions.
   shares:
     description: |
       A mapping of share name to share specific configuration. A share can
       have "options" that are passed to Samba. Shares can have an optional
       "permissions" section for managing permissions/acls in sambacc.
     type: object
     additionalProperties:
       type: object
       properties:
         options:
           $ref: "#/$defs/samba_options"
         permissions:
           $ref: "#/$defs/permissions_config"
       additionalProperties: false
-  # globals defintions.
+  # globals definitions.
   globals:
     description: |
-      A mapping of samba global configuation blocks. The global section names
+      A mapping of samba global configuration blocks. The global section names
       are not passed to Samba. All sections selected by a configuration are
       merged together before passing to Samba.
     type: object
     additionalProperties:
       type: object
       properties:
         options:
@@ -226,35 +245,48 @@
       properties:
         realm:
           type: string
         short_domain:
           type: string
         admin_password:
           type: string
+        interfaces:
+          type: object
+          properties:
+            include_pattern:
+              type: string
+              description: |
+                A regular expression that must match for a network interface
+                to be included in the AD DC interfaces list.
+            exclude_pattern:
+              type: string
+              description: |
+                A regular expression that must not match for a network interface
+                to be included in the AD DC interfaces list.
       required:
         - realm
       additionalProperties: false
   # users to be set up in the container environment prior to starting
   # a samba fileserver
   users:
     description: |
       Users to add to the container environment in order to provide
-      Share access-control wihout becoming a domain member server.
+      Share access-control without becoming a domain member server.
     type: object
     properties:
       all_entries:
         type: array
         items:
           $ref: "#/$defs/user_entry"
   # groups to be set up in the container environment prior to starting
   # a samba fileserver
   groups:
     description: |
       Groups to add to the container environment in order to provide
-      Share access-control wihout becoming a domain member server.
+      Share access-control without becoming a domain member server.
     type: object
     properties:
       all_entries:
         type: array
         items:
           $ref: "#/$defs/group_entry"
   # domain_users are users that will be initialized for a new AD DC instance
@@ -275,14 +307,25 @@
       automatically added to a newly provisioned domain. This section is
       a mapping of the domain settings name to a list of domain group entries.
     type: object
     additionalProperties:
       type: array
       items:
         $ref: "#/$defs/domain_group_entry"
+  # organizational_unit are organizational unit that will be initialized for a new AD DC instance
+  organizational_units:
+    description: |
+      The organizational_unit section defines initial organizational unit that will be
+      automatically added to a newly provisioned domain. This section is
+      a mapping of the domain settings name to a list of domain group entries.
+    type: object
+    additionalProperties:
+      type: array
+      items:
+        $ref: "#/$defs/organizational_unit_entry"
   # ctdb customization settings
   # generally for developers/expert users only. these ctdb specific overrides
   # live outside the smb.conf and have their own section
   ctdb:
     type: object
     additionalProperties:
       type: string
```

### Comparing `sambacc-0.4/sambacc/schema/conf_v0_schema.py` & `sambacc-0.5/sambacc/schema/conf_v0_schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                     "type": "string",
                 },
             },
             "additionalProperties": {"type": "string"},
         },
         "user_entry": {
             "description": (
-                "A user that will be instantiated in the local contianer"
+                "A user that will be instantiated in the local container"
                 " environment to\nin order to provide access to smb shares.\n"
             ),
             "type": "object",
             "properties": {
                 "name": {"description": "The user's name", "type": "string"},
                 "uid": {
                     "description": "The Unix UID the user should have",
@@ -89,15 +89,15 @@
                 },
             },
             "required": ["name"],
             "additionalProperties": False,
         },
         "group_entry": {
             "description": (
-                "A group that will be instantiated in the local contianer"
+                "A group that will be instantiated in the local container"
                 " environment to\nin order to provide access to smb shares.\n"
             ),
             "type": "object",
             "properties": {
                 "name": {"description": "The group name", "type": "string"},
                 "gid": {
                     "description": "The Unix GID the group should have",
@@ -127,14 +127,20 @@
                 "uid": {"type": "integer"},
                 "gid": {"type": "integer"},
                 "nt_hash": {"type": "string"},
                 "password": {
                     "description": "A plain-text password",
                     "type": "string",
                 },
+                "ou": {
+                    "description": (
+                        "A organizational unit that the user should belong to"
+                    ),
+                    "type": "string",
+                },
                 "member_of": {
                     "description": (
                         "A list of group names that the user should belong to"
                     ),
                     "type": "array",
                     "items": {"type": "string"},
                 },
@@ -148,35 +154,57 @@
                 " These\ngroups are populated in the directory after the"
                 " domain is provisioned.\n"
             ),
             "type": "object",
             "properties": {
                 "name": {"description": "The group name", "type": "string"},
                 "gid": {"type": "integer"},
+                "ou": {
+                    "description": (
+                        "A organizational unit that the user should belong to"
+                    ),
+                    "type": "string",
+                },
+            },
+            "required": ["name"],
+            "additionalProperties": False,
+        },
+        "organizational_unit_entry": {
+            "description": (
+                "A organizational unit that will be created in the specified"
+                " AD domain. These\ngroups are populated in the directory"
+                " after the domain is provisioned.\n"
+            ),
+            "type": "object",
+            "properties": {
+                "name": {
+                    "description": "The organizational unit name",
+                    "type": "string",
+                }
             },
             "required": ["name"],
             "additionalProperties": False,
         },
     },
     "properties": {
         "samba-container-config": {
             "type": "string",
-            "title": "Cofiguration Format Version",
+            "title": "Configuration Format Version",
             "description": (
                 "A short version string that assists in allowing the"
                 " configuration\nformat to (some day) support incompatible"
                 " version changes.\n(It is unique to the configuration and is"
                 " not the version of sambacc)\n"
             ),
         },
         "configs": {
             "title": "Container Configurations",
             "description": (
                 "A mapping of named configurations (instances) to top-level"
-                " configuration\nblocks. A useable configuration file must"
+                " configuration\nblocks. A usable configuration file must"
                 " have at least one configuration,\nbut more than one is"
                 " supported.\n"
             ),
             "type": "object",
             "additionalProperties": {
                 "type": "object",
                 "properties": {
@@ -217,15 +245,15 @@
                     "permissions": {"$ref": "#/$defs/permissions_config"},
                 },
                 "additionalProperties": False,
             },
         },
         "globals": {
             "description": (
-                "A mapping of samba global configuation blocks. The global"
+                "A mapping of samba global configuration blocks. The global"
                 " section names\nare not passed to Samba. All sections"
                 " selected by a configuration are\nmerged together before"
                 " passing to Samba.\n"
             ),
             "type": "object",
             "additionalProperties": {
                 "type": "object",
@@ -242,37 +270,58 @@
             "type": "object",
             "additionalProperties": {
                 "type": "object",
                 "properties": {
                     "realm": {"type": "string"},
                     "short_domain": {"type": "string"},
                     "admin_password": {"type": "string"},
+                    "interfaces": {
+                        "type": "object",
+                        "properties": {
+                            "include_pattern": {
+                                "type": "string",
+                                "description": (
+                                    "A regular expression that must match for"
+                                    " a network interface\nto be included in"
+                                    " the AD DC interfaces list.\n"
+                                ),
+                            },
+                            "exclude_pattern": {
+                                "type": "string",
+                                "description": (
+                                    "A regular expression that must not match"
+                                    " for a network interface\nto be included"
+                                    " in the AD DC interfaces list.\n"
+                                ),
+                            },
+                        },
+                    },
                 },
                 "required": ["realm"],
                 "additionalProperties": False,
             },
         },
         "users": {
             "description": (
                 "Users to add to the container environment in order to"
-                " provide\nShare access-control wihout becoming a domain"
+                " provide\nShare access-control without becoming a domain"
                 " member server.\n"
             ),
             "type": "object",
             "properties": {
                 "all_entries": {
                     "type": "array",
                     "items": {"$ref": "#/$defs/user_entry"},
                 }
             },
         },
         "groups": {
             "description": (
                 "Groups to add to the container environment in order to"
-                " provide\nShare access-control wihout becoming a domain"
+                " provide\nShare access-control without becoming a domain"
                 " member server.\n"
             ),
             "type": "object",
             "properties": {
                 "all_entries": {
                     "type": "array",
                     "items": {"$ref": "#/$defs/group_entry"},
@@ -301,14 +350,27 @@
             ),
             "type": "object",
             "additionalProperties": {
                 "type": "array",
                 "items": {"$ref": "#/$defs/domain_group_entry"},
             },
         },
+        "organizational_units": {
+            "description": (
+                "The organizational_unit section defines initial"
+                " organizational unit that will be\nautomatically added to a"
+                " newly provisioned domain. This section is\na mapping of the"
+                " domain settings name to a list of domain group entries.\n"
+            ),
+            "type": "object",
+            "additionalProperties": {
+                "type": "array",
+                "items": {"$ref": "#/$defs/organizational_unit_entry"},
+            },
+        },
         "ctdb": {
             "type": "object",
             "additionalProperties": {"type": "string"},
         },
     },
     "additionalProperties": False,
     "required": ["samba-container-config"],
```

### Comparing `sambacc-0.4/sambacc/schema/tool.py` & `sambacc-0.5/sambacc/schema/tool.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/simple_waiter.py` & `sambacc-0.5/sambacc/simple_waiter.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/smbconf_api.py` & `sambacc-0.5/sambacc/smbconf_api.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/smbconf_samba.py` & `sambacc-0.5/sambacc/smbconf_samba.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/textfile.py` & `sambacc-0.5/sambacc/textfile.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/typelets.py` & `sambacc-0.5/sambacc/typelets.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc/url_opener.py` & `sambacc-0.5/sambacc/url_opener.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/sambacc.egg-info/PKG-INFO` & `sambacc-0.5/sambacc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sambacc
-Version: 0.4
+Version: 0.5
 Summary: Samba Container Configurator
 Home-page: https://github.com/samba-in-kubernetes/sambacc
 Author: John Mulligan
 Author-email: phlogistonjohn@asynchrono.us
 License: GPL3
 Description-Content-Type: text/markdown
 License-File: COPYING
```

### Comparing `sambacc-0.4/sambacc.egg-info/SOURCES.txt` & `sambacc-0.5/sambacc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 tox.ini
 .copr/Makefile
 .github/mergify.yml
 .github/workflows/ci.yml
 docs/configuration.md
 docs/release-process.md
 examples/addc.json
+examples/addc_ou.json
+examples/addc_x.json
 examples/ctdb.json
 examples/example1.json
 examples/minimal.json
 extras/python-sambacc.spec
 sambacc/__init__.py
 sambacc/_version.py
 sambacc/_xattr.py
```

### Comparing `sambacc-0.4/setup.cfg` & `sambacc-0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/container/Containerfile` & `sambacc-0.5/tests/container/Containerfile`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ARG SAMBACC_BASE_IMAGE='registry.fedoraproject.org/fedora:37'
+ARG SAMBACC_BASE_IMAGE='registry.fedoraproject.org/fedora:39'
 FROM $SAMBACC_BASE_IMAGE
 
 
 COPY build.sh /usr/local/bin/build.sh
 
 # Set SAMBACC_MINIMAL to yes to build a container that only contains the
 # build.sh script on top of the base image. When called, build.sh will
```

### Comparing `sambacc-0.4/tests/container/build.sh` & `sambacc-0.5/tests/container/build.sh`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_addc.py` & `sambacc-0.5/tests/test_samba_cmds.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 # sambacc: a samba container configuration tool
-# Copyright (C) 2022  John Mulligan
+# Copyright (C) 2021  John Mulligan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,136 +12,154 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 #
 
-import os
+import sambacc.samba_cmds
 
-import pytest
 
-
-import sambacc.addc
-
-
-def _fake_samba_tool(path):
-    fake_samba_tool = path / "fake_samba_tool.sh"
-    with open(fake_samba_tool, "w") as fh:
-        fh.write("#!/bin/sh\n")
-        fh.write(f"[ -e {path}/fail ] && exit 1\n")
-        fh.write(f'echo "$@" > {path}/args.out\n')
-        fh.write("exit 0")
-    os.chmod(fake_samba_tool, 0o700)
-    return fake_samba_tool
-
-
-def test_provision(tmp_path, monkeypatch):
-    monkeypatch.setattr(
-        sambacc.samba_cmds, "_GLOBAL_PREFIX", [_fake_samba_tool(tmp_path)]
-    )
-
-    sambacc.addc.provision("FOOBAR.TEST", "quux", "h4ckm3")
-    with open(tmp_path / "args.out") as fh:
-        result = fh.read()
-    assert "--realm=FOOBAR.TEST" in result
-    assert "--option=netbios name=quux" in result
-    assert "--dns-backend=SAMBA_INTERNAL" in result
-
-    sambacc.addc.provision(
-        "BARFOO.TEST",
-        "quux",
-        "h4ckm3",
-        options=[
-            ("ldap server require strong auth", "no"),
-            ("dns zone scavenging", "yes"),
-            ("ldap machine suffix", "ou=Machines"),
-            ("netbios name", "flipper"),
-        ],
-    )
-    with open(tmp_path / "args.out") as fh:
-        result = fh.read()
-    assert "--realm=BARFOO.TEST" in result
-    assert "--option=netbios name=quux" in result
-    assert "--dns-backend=SAMBA_INTERNAL" in result
-    assert "--option=ldap server require strong auth=no" in result
-    assert "--option=dns zone scavenging=yes" in result
-    assert "--option=ldap machine suffix=ou=Machines" in result
-    assert "--option=netbios name=flipper" not in result
-
-    open(tmp_path / "fail", "w").close()
-    with pytest.raises(Exception):
-        sambacc.addc.provision("FOOBAR.TEST", "quux", "h4ckm3")
-
-
-def test_join(tmp_path, monkeypatch):
-    monkeypatch.setattr(
-        sambacc.samba_cmds, "_GLOBAL_PREFIX", [_fake_samba_tool(tmp_path)]
-    )
-
-    sambacc.addc.join("FOOBAR.TEST", "quux", "h4ckm3")
-    with open(tmp_path / "args.out") as fh:
-        result = fh.read()
-    assert "FOOBAR.TEST" in result
-    assert "--option=netbios name=quux" in result
-    assert "--dns-backend=SAMBA_INTERNAL" in result
-
-    sambacc.addc.join(
-        "BARFOO.TEST",
-        "quux",
-        "h4ckm3",
-        options=[
-            ("ldap server require strong auth", "no"),
-            ("dns zone scavenging", "yes"),
-            ("ldap machine suffix", "ou=Machines"),
-            ("netbios name", "flipper"),
-        ],
-    )
-    with open(tmp_path / "args.out") as fh:
-        result = fh.read()
-    with open(tmp_path / "args.out") as fh:
-        result = fh.read()
-    assert "BARFOO.TEST" in result
-    assert "--option=netbios name=quux" in result
-    assert "--dns-backend=SAMBA_INTERNAL" in result
-    assert "--option=ldap server require strong auth=no" in result
-    assert "--option=dns zone scavenging=yes" in result
-    assert "--option=ldap machine suffix=ou=Machines" in result
-    assert "--option=netbios name=flipper" not in result
-
-
-def test_create_user(tmp_path, monkeypatch):
-    monkeypatch.setattr(
-        sambacc.samba_cmds, "_GLOBAL_PREFIX", [_fake_samba_tool(tmp_path)]
-    )
-
-    sambacc.addc.create_user("fflintstone", "b3dr0ck", "Flintstone", "Fred")
-    with open(tmp_path / "args.out") as fh:
-        result = fh.read()
-    assert "user create fflintstone" in result
-    assert "--surname=Flintstone" in result
-    assert "--given-name=Fred" in result
-
-
-def test_create_group(tmp_path, monkeypatch):
-    monkeypatch.setattr(
-        sambacc.samba_cmds, "_GLOBAL_PREFIX", [_fake_samba_tool(tmp_path)]
-    )
-
-    sambacc.addc.create_group("quarry_workers")
-    with open(tmp_path / "args.out") as fh:
-        result = fh.read()
-    assert "group add quarry_workers" in result
-
-
-def test_add_group_members(tmp_path, monkeypatch):
-    monkeypatch.setattr(
-        sambacc.samba_cmds, "_GLOBAL_PREFIX", [_fake_samba_tool(tmp_path)]
-    )
-
-    sambacc.addc.add_group_members(
-        "quarry_workers", ["fflintstone", "brubble"]
-    )
-    with open(tmp_path / "args.out") as fh:
-        result = fh.read()
-    assert "group addmembers quarry_workers" in result
-    assert "fflintstone,brubble" in result
+def test_create_samba_command():
+    cmd = sambacc.samba_cmds.SambaCommand("hello")
+    assert cmd.name == "hello"
+    cmd2 = cmd["world"]
+    assert cmd.name == "hello"
+    assert list(cmd) == ["hello"]
+    assert list(cmd2) == ["hello", "world"]
+
+
+def test_debug_command():
+    cmd = sambacc.samba_cmds.SambaCommand("beep", debug="5")
+    assert list(cmd) == ["beep", "--debuglevel=5"]
+
+
+def test_global_debug():
+    sambacc.samba_cmds.set_global_debug("7")
+    try:
+        cmd = sambacc.samba_cmds.SambaCommand("cheep")
+        assert list(cmd) == ["cheep", "--debuglevel=7"]
+    finally:
+        sambacc.samba_cmds.set_global_debug("")
+
+
+def test_global_prefix():
+    # enabled
+    sambacc.samba_cmds.set_global_prefix(["bob"])
+    try:
+        cmd = sambacc.samba_cmds.SambaCommand("deep")
+        assert list(cmd) == ["bob", "deep"]
+        assert cmd.name == "bob"
+    finally:
+        sambacc.samba_cmds.set_global_prefix([])
+
+    # disabled
+    cmd = sambacc.samba_cmds.SambaCommand("deep")
+    assert list(cmd) == ["deep"]
+    assert cmd.name == "deep"
+
+
+def test_global_prefix_extended():
+    # enabled
+    sambacc.samba_cmds.set_global_prefix(["frank"])
+    try:
+        cmd = sambacc.samba_cmds.SambaCommand("deep")[
+            "13", "--future=not-too-distant"
+        ]
+        assert list(cmd) == ["frank", "deep", "13", "--future=not-too-distant"]
+        assert cmd.name == "frank"
+    finally:
+        sambacc.samba_cmds.set_global_prefix([])
+
+    # disabled, must not "inherit" the prefix
+    cmd2 = cmd["--scheme", "evil"]
+    assert list(cmd2) == [
+        "deep",
+        "13",
+        "--future=not-too-distant",
+        "--scheme",
+        "evil",
+    ]
+    assert cmd2.name == "deep"
+
+
+def test_command_repr():
+    cmd = sambacc.samba_cmds.SambaCommand("doop")
+    cr = repr(cmd)
+    assert cr.startswith("SambaCommand")
+    assert "doop" in cr
+
+
+def test_encode_none():
+    res = sambacc.samba_cmds.encode(None)
+    assert res == b""
+
+
+def test_execute():
+    import os
+
+    cmd = sambacc.samba_cmds.SambaCommand("true")
+    pid = os.fork()
+    if pid == 0:
+        sambacc.samba_cmds.execute(cmd)
+    else:
+        _, status = os.waitpid(pid, 0)
+        assert status == 0
+
+
+def test_create_command_args():
+    # this is the simpler base class for SambaCommand. It lacks
+    # the samba debug level option.
+    cmd = sambacc.samba_cmds.CommandArgs("something")
+    assert cmd.name == "something"
+    cmd2 = cmd["nice"]
+    assert cmd.name == "something"
+    assert list(cmd) == ["something"]
+    assert list(cmd2) == ["something", "nice"]
+
+
+def test_command_args_repr():
+    r = str(sambacc.samba_cmds.CommandArgs("something", ["nice"]))
+    assert r.startswith("CommandArgs")
+    assert "something" in r
+    assert "nice" in r
+
+
+def test_get_samba_specifics(monkeypatch):
+    monkeypatch.setenv("SAMBA_SPECIFICS", "")
+    ss = sambacc.samba_cmds.get_samba_specifics()
+    assert not ss
+
+    monkeypatch.setenv("SAMBA_SPECIFICS", "wibble,quux")
+    ss = sambacc.samba_cmds.get_samba_specifics()
+    assert ss
+    assert len(ss) == 2
+    assert "wibble" in ss
+    assert "quux" in ss
+
+
+def test_smbd_foreground(monkeypatch):
+    monkeypatch.setenv("SAMBA_SPECIFICS", "")
+    sf = sambacc.samba_cmds.smbd_foreground()
+    assert "smbd" in sf.name
+    assert "--log-stdout" in sf.argv()
+    assert "--debug-stdout" not in sf.argv()
+
+    monkeypatch.setenv("SAMBA_SPECIFICS", "daemon_cli_debug_output")
+    sf = sambacc.samba_cmds.smbd_foreground()
+    assert "smbd" in sf.name
+    assert "--log-stdout" not in sf.argv()
+    assert "--debug-stdout" in sf.argv()
+
+
+def test_winbindd_foreground(monkeypatch):
+    monkeypatch.setenv("SAMBA_SPECIFICS", "")
+    wf = sambacc.samba_cmds.winbindd_foreground()
+    assert "winbindd" in wf.name
+    assert "--stdout" in wf.argv()
+    assert "--debug-stdout" not in wf.argv()
+
+    monkeypatch.setenv("SAMBA_SPECIFICS", "daemon_cli_debug_output")
+    wf = sambacc.samba_cmds.winbindd_foreground()
+    assert "winbindd" in wf.name
+    assert "--stdout" not in wf.argv()
+    assert "--debug-stdout" in wf.argv()
```

### Comparing `sambacc-0.4/tests/test_commands_config.py` & `sambacc-0.5/tests/test_commands_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #
 
 import argparse
 import functools
 import os
 
 import sambacc.config
+import sambacc.opener
 import sambacc.paths
 
 import sambacc.commands.config
 
 
 config1 = """
 {
@@ -109,14 +110,18 @@
                 "config": config,
                 "identity": identity,
             },
             sambacc.config.read_config_files(config).get(identity),
         )
         return ctx
 
+    @property
+    def opener(self) -> sambacc.opener.Opener:
+        return sambacc.opener.FileOpener()
+
 
 class FakeWaiter:
     def __init__(self, attempts=None):
         self.count = 0
         self.on_count = {}
         self.attempts = attempts
```

### Comparing `sambacc-0.4/tests/test_config.py` & `sambacc-0.5/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 #
 
 import io
 import os
-import pytest
 import unittest
 
+import pytest
+
 import sambacc.config
 import sambacc.opener
 
 config1 = """
 {
     "samba-container-config": "v0",
     "configs": {
@@ -161,15 +162,14 @@
         {"name": "bobs", "gid": 2000},
         {"name": "alii", "gid": 2001}
       ]
   }
 }
 """
 
-
 ctdb_config1 = """
 {
   "samba-container-config": "v0",
   "configs": {
     "ctdb1": {
       "shares": [
         "demo"
@@ -251,14 +251,68 @@
         "member_of": ["friends"]
       }
     ]
   }
 }
 """
 
+addc_config2 = """
+{
+  "samba-container-config": "v0",
+  "configs": {
+    "demo": {
+      "instance_features": ["addc"],
+      "domain_settings": "sink",
+      "instance_name": "dc1"
+    }
+  },
+  "domain_settings": {
+    "sink": {
+      "realm": "DOMAIN1.SINK.TEST",
+      "short_domain": "DOMAIN1",
+      "admin_password": "Passw0rd"
+    }
+  },
+  "organizational_units": {
+    "sink": [
+      {"name": "friends"}
+    ]
+  },
+  "domain_groups": {
+    "sink": [
+      {
+        "name": "friends",
+        "ou": "friends"
+      },
+      {"name": "gothamites"}
+    ]
+  },
+  "domain_users": {
+    "sink": [
+      {
+        "name": "bwayne",
+        "password": "1115Rose.",
+        "given_name": "Bruce",
+        "surname": "Wayne",
+        "member_of": ["friends", "gothamites"],
+        "ou": "friends"
+      },
+      {
+        "name": "ckent",
+        "password": "1115Rose.",
+        "given_name": "Clark",
+        "surname": "Kent",
+        "member_of": ["friends"],
+        "ou": "friends"
+      }
+    ]
+  }
+}
+"""
+
 
 class TestConfig(unittest.TestCase):
     def test_non_json(self):
         with self.assertRaises(Exception):
             with open(os.devnull) as fh:
                 sambacc.config.GlobalConfig(fh)
 
@@ -511,69 +565,48 @@
     assert dgroups[0].groupname == "friends"
 
     dusers = sorted(i1.domain_users(), key=lambda v: v.username)
     assert len(dusers) == 2
     assert dusers[0].username == "bwayne"
 
 
+def test_ad_dc_ou_config_demo():
+    c1 = sambacc.config.GlobalConfig(io.StringIO(addc_config2))
+    i1 = c1.get("demo")
+    assert i1.with_addc
+
+    domou = sorted(i1.organizational_units(), key=lambda v: v.ou_name)
+    assert len(domou) == 1
+    assert domou[0].ou_name == "friends"
+
+    dgroups = sorted(i1.domain_groups(), key=lambda v: v.groupname)
+    assert len(dgroups) == 2
+    assert dgroups[0].ou == "friends"
+
+    dusers = sorted(i1.domain_users(), key=lambda v: v.username)
+    assert len(dusers) == 2
+    assert dusers[0].ou == "friends"
+
+
 def test_ad_dc_invalid():
     c1 = sambacc.config.GlobalConfig(io.StringIO(config1))
     i1 = c1.get("foobar")
     assert not i1.with_addc
 
     with pytest.raises(ValueError):
         i1.domain()
 
     with pytest.raises(ValueError):
         list(i1.domain_users())
 
     with pytest.raises(ValueError):
         list(i1.domain_groups())
 
-
-def test_ad_dc_bad_member_of():
-    jdata = {
-        "samba-container-config": "v0",
-        "configs": {
-            "demo": {
-                "instance_features": ["addc"],
-                "domain_settings": "sink",
-                "instance_name": "dc1",
-            }
-        },
-        "domain_settings": {
-            "sink": {
-                "realm": "DOMAIN1.SINK.TEST",
-                "short_domain": "DOMAIN1",
-                "admin_password": "Passw0rd",
-            }
-        },
-        "domain_groups": {"sink": [{"name": "friends"}]},
-        "domain_users": {
-            "sink": [
-                {
-                    "name": "ckent",
-                    "password": "1115Rose.",
-                    "given_name": "Clark",
-                    "surname": "Kent",
-                    "member_of": "friends",
-                }
-            ]
-        },
-    }
-    c1 = sambacc.config.GlobalConfig(initial_data=jdata)
-    i1 = c1.get("demo")
-    assert i1.with_addc
-
-    dgroups = sorted(i1.domain_groups(), key=lambda v: v.groupname)
-    assert len(dgroups) == 1
-    assert dgroups[0].groupname == "friends"
-
     with pytest.raises(ValueError):
-        list(i1.domain_users())
+        list(i1.organizational_units())
 
 
 def test_share_config_no_path():
     j = """{
     "samba-container-config": "v0",
     "configs": {
         "foobar":{
```

### Comparing `sambacc-0.4/tests/test_container_dns.py` & `sambacc-0.5/tests/test_container_dns.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_ctdb.py` & `sambacc-0.5/tests/test_ctdb.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_inotify_waiter.py` & `sambacc-0.5/tests/test_inotify_waiter.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_jfile.py` & `sambacc-0.5/tests/test_jfile.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_join.py` & `sambacc-0.5/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_main.py` & `sambacc-0.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_netcmd_loader.py` & `sambacc-0.5/tests/test_netcmd_loader.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_passdb_loader.py` & `sambacc-0.5/tests/test_passdb_loader.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_passwd_loader.py` & `sambacc-0.5/tests/test_passwd_loader.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_paths.py` & `sambacc-0.5/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_permissions.py` & `sambacc-0.5/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_rados_opener.py` & `sambacc-0.5/tests/test_rados_opener.py`

 * *Files 27% similar despite different names*

```diff
@@ -41,14 +41,62 @@
 
 def test_enable_rados_url_opener_fail(monkeypatch):
     cls_mock = unittest.mock.MagicMock()
     sambacc.rados_opener.enable_rados_url_opener(cls_mock)
     assert not cls_mock._handlers.append.called
 
 
+def test_enable_rados_url_opener_with_args(monkeypatch):
+    mock = unittest.mock.MagicMock()
+    monkeypatch.setitem(sys.modules, "rados", mock)
+
+    cls_mock = unittest.mock.MagicMock()
+    cls_mock._handlers = []
+    sambacc.rados_opener.enable_rados_url_opener(cls_mock, client_name="user1")
+    assert len(cls_mock._handlers) == 1
+    assert isinstance(
+        cls_mock._handlers[0]._interface, sambacc.rados_opener._RADOSInterface
+    )
+    assert cls_mock._handlers[0]._interface.api is mock
+    assert cls_mock._handlers[0]._interface.client_name == "user1"
+    assert not cls_mock._handlers[0]._interface.full_name
+    ri = cls_mock._handlers[0]._interface
+    ri.Rados()
+    assert ri.api.Rados.call_args[1]["rados_id"] == "user1"
+    assert ri.api.Rados.call_args[1]["name"] == ""
+    assert (
+        ri.api.Rados.call_args[1]["conffile"] == mock.Rados.DEFAULT_CONF_FILES
+    )
+
+
+def test_enable_rados_url_opener_with_args2(monkeypatch):
+    mock = unittest.mock.MagicMock()
+    monkeypatch.setitem(sys.modules, "rados", mock)
+
+    cls_mock = unittest.mock.MagicMock()
+    cls_mock._handlers = []
+    sambacc.rados_opener.enable_rados_url_opener(
+        cls_mock, client_name="client.user1", full_name=True
+    )
+    assert len(cls_mock._handlers) == 1
+    assert isinstance(
+        cls_mock._handlers[0]._interface, sambacc.rados_opener._RADOSInterface
+    )
+    assert cls_mock._handlers[0]._interface.api is mock
+    assert cls_mock._handlers[0]._interface.client_name == "client.user1"
+    assert cls_mock._handlers[0]._interface.full_name
+    ri = cls_mock._handlers[0]._interface
+    ri.Rados()
+    assert ri.api.Rados.call_args[1]["rados_id"] == ""
+    assert ri.api.Rados.call_args[1]["name"] == "client.user1"
+    assert (
+        ri.api.Rados.call_args[1]["conffile"] == mock.Rados.DEFAULT_CONF_FILES
+    )
+
+
 def test_rados_handler_parse():
     class RH(sambacc.rados_opener._RADOSHandler):
         _rados_api = unittest.mock.MagicMock()
 
     rh = RH()
     rq = urllib.request.Request("rados://foo/bar/baz")
     rr = rh.rados_open(rq)
@@ -63,15 +111,15 @@
     assert rr._key == "baz1"
 
 
 def test_rados_handler_norados():
     # Generally, this shouldn't happen because the rados handler shouldn't
     # be added to the URLOpener if rados module was unavailable.
     class RH(sambacc.rados_opener._RADOSHandler):
-        _rados_api = None
+        _interface = None
 
     rh = RH()
     rq = urllib.request.Request("rados://foo/bar/baz")
     with pytest.raises(sambacc.rados_opener.RADOSUnsupported):
         rh.rados_open(rq)
 
 
@@ -152,7 +200,33 @@
         rr.readlines()
     with pytest.raises(NotImplementedError):
         rr.truncate()
     with pytest.raises(NotImplementedError):
         rr.write(b"zzzzz")
     with pytest.raises(NotImplementedError):
         rr.writelines([b"zzzzz"])
+
+
+def test_rados_handler_config_key():
+    class RH(sambacc.rados_opener._RADOSHandler):
+        _interface = unittest.mock.MagicMock()
+
+    mc = RH._interface.Rados.return_value.__enter__.return_value.mon_command
+    mc.return_value = (0, b"rubber baby buggy bumpers", "")
+
+    rh = RH()
+    rq = urllib.request.Request("rados:mon-config-key:aa/bb/cc")
+    rr = rh.rados_open(rq)
+    assert isinstance(rr, io.BytesIO)
+    assert rr.read() == b"rubber baby buggy bumpers"
+    assert mc.called
+    assert "aa/bb/cc" in mc.call_args[0][0]
+
+    mc.reset_mock()
+    mc.return_value = (2, b"", "no passing")
+    rh = RH()
+    rq = urllib.request.Request("rados:mon-config-key:xx/yy/zz")
+    with pytest.raises(OSError) as pe:
+        rh.rados_open(rq)
+    assert getattr(pe.value, "errno", None) == 2
+    assert mc.called
+    assert "xx/yy/zz" in mc.call_args[0][0]
```

### Comparing `sambacc-0.4/tests/test_simple_waiter.py` & `sambacc-0.5/tests/test_simple_waiter.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_smbconf_api.py` & `sambacc-0.5/tests/test_smbconf_api.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_smbconf_samba.py` & `sambacc-0.5/tests/test_smbconf_samba.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.4/tests/test_url_opener.py` & `sambacc-0.5/tests/test_url_opener.py`

 * *Files identical despite different names*

