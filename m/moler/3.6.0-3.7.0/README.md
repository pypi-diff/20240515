# Comparing `tmp/moler-3.6.0.tar.gz` & `tmp/moler-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moler-3.6.0.tar", last modified: Tue May  7 12:42:27 2024, max compression
+gzip compressed data, was "moler-3.7.0.tar", last modified: Wed May 15 13:33:43 2024, max compression
```

## Comparing `moler-3.6.0.tar` & `moler-3.7.0.tar`

### file list

```diff
@@ -1,344 +1,344 @@
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.454288 moler-3.6.0/
--rw-r--r--   0 ute       (1000) ute       (1000)     1505 2024-02-06 08:16:12.000000 moler-3.6.0/LICENSE
--rw-r--r--   0 ute       (1000) ute       (1000)    26591 2024-05-07 12:42:27.454288 moler-3.6.0/PKG-INFO
--rw-r--r--   0 ute       (1000) ute       (1000)    24908 2024-05-07 12:40:55.000000 moler-3.6.0/README.md
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.278288 moler-3.6.0/moler/
--rw-r--r--   0 ute       (1000) ute       (1000)      143 2024-02-06 08:16:12.000000 moler-3.6.0/moler/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10606 2024-02-19 07:54:48.000000 moler-3.6.0/moler/abstract_moler_connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)    49062 2024-02-19 07:54:48.000000 moler-3.6.0/moler/asyncio_runner.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.294288 moler-3.6.0/moler/cmd/
--rw-r--r--   0 ute       (1000) ute       (1000)     4140 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.298288 moler-3.6.0/moler/cmd/adb/
--rw-r--r--   0 ute       (1000) ute       (1000)      191 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/adb/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5686 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/adb/adb_shell.py
--rw-r--r--   0 ute       (1000) ute       (1000)      331 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/adb/generic_adb_command.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.322288 moler-3.6.0/moler/cmd/at/
--rw-r--r--   0 ute       (1000) ute       (1000)      369 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1588 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/at.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1553 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/attach.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1826 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/create_pdu_session.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3604 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/cu.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1526 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/detach.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1878 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/enable_echo.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2808 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/exit_serial_proxy.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3786 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/genericat.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5005 2024-02-06 14:47:26.000000 moler-3.6.0/moler/cmd/at/get_apns.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3062 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/get_attach_state.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4770 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/get_cell_id.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9134 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/get_cell_id_gprs.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8605 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/get_cell_id_lte.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6797 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/get_cell_id_nr.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2792 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/get_functionality_level.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5945 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/get_imei.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2654 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/get_imsi.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3226 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/get_ip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3125 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/get_manufacturer_id.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5128 2024-02-06 14:47:26.000000 moler-3.6.0/moler/cmd/at/get_product_info.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3294 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/get_revision_id.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3555 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/plink_serial.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2361 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/quectel_lock_nr_earfcn.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2459 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/quectel_network_preferences.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1828 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/at/release_pdu_session.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4632 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/run_script.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2570 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/set_apn.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2454 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/set_cell_id.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3066 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/set_cell_id_gprs.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3056 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/set_cell_id_lte.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2741 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/set_cell_id_nr.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3367 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/set_functionality_level.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2231 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/at/set_mode.py
--rw-r--r--   0 ute       (1000) ute       (1000)    13384 2024-05-07 12:40:55.000000 moler-3.6.0/moler/cmd/commandchangingprompt.py
--rw-r--r--   0 ute       (1000) ute       (1000)    28640 2024-04-24 13:39:02.000000 moler-3.6.0/moler/cmd/commandtextualgeneric.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.322288 moler-3.6.0/moler/cmd/juniper/
--rw-r--r--   0 ute       (1000) ute       (1000)      195 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/juniper/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.322288 moler-3.6.0/moler/cmd/juniper/cli/
--rw-r--r--   0 ute       (1000) ute       (1000)      199 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/juniper/cli/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2571 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/juniper/cli/configure.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.322288 moler-3.6.0/moler/cmd/juniper/configure/
--rw-r--r--   0 ute       (1000) ute       (1000)      205 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/juniper/configure/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2616 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/juniper/configure/exit_configure.py
--rw-r--r--   0 ute       (1000) ute       (1000)      993 2024-02-06 14:47:26.000000 moler-3.6.0/moler/cmd/juniper/genericjuniper.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.326288 moler-3.6.0/moler/cmd/juniper_ex/
--rw-r--r--   0 ute       (1000) ute       (1000)      197 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/juniper_ex/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.326288 moler-3.6.0/moler/cmd/juniper_ex/cli/
--rw-r--r--   0 ute       (1000) ute       (1000)      201 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/juniper_ex/cli/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.326288 moler-3.6.0/moler/cmd/juniper_ex/configure/
--rw-r--r--   0 ute       (1000) ute       (1000)      207 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/juniper_ex/configure/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      404 2024-02-06 14:47:26.000000 moler-3.6.0/moler/cmd/juniper_ex/genericjuniperex.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.326288 moler-3.6.0/moler/cmd/pdu_aten/
--rw-r--r--   0 ute       (1000) ute       (1000)      192 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/pdu_aten/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      904 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/pdu_aten/generic_pdu_aten.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.326288 moler-3.6.0/moler/cmd/pdu_aten/pdu/
--rw-r--r--   0 ute       (1000) ute       (1000)      205 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/pdu_aten/pdu/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      415 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/pdu_aten/pdu/exit_telnet.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1193 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/pdu_aten/pdu/generic_pdu.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1589 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/pdu_aten/pdu/quit.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2895 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/pdu_aten/pdu/read_meter.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2948 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/pdu_aten/pdu/read_status.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1870 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/pdu_aten/pdu/sw.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.330288 moler-3.6.0/moler/cmd/scpi/
--rw-r--r--   0 ute       (1000) ute       (1000)      188 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/scpi/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      370 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/scpi/genricscpi.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.330288 moler-3.6.0/moler/cmd/scpi/scpi/
--rw-r--r--   0 ute       (1000) ute       (1000)      202 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/scpi/scpi/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      415 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/scpi/scpi/exit_telnet.py
--rw-r--r--   0 ute       (1000) ute       (1000)      969 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/scpi/scpi/genericscpistate.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1378 2024-02-06 14:47:26.000000 moler-3.6.0/moler/cmd/scpi/scpi/idn.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1598 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/scpi/scpi/read.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1921 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/scpi/scpi/run_command.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.374288 moler-3.6.0/moler/cmd/unix/
--rw-r--r--   0 ute       (1000) ute       (1000)      194 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/unix/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4744 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/adb_devices.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1957 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/adb_forward.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1465 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/adb_root.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1201 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/unix/bash.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6135 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/cat.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3342 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/cd.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2004 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/chgrp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2158 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/chmod.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2507 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/chown.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1650 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/cp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2807 2024-03-11 13:43:51.000000 moler-3.6.0/moler/cmd/unix/ctrl_c.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2459 2024-03-11 13:46:32.000000 moler-3.6.0/moler/cmd/unix/ctrl_z.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3554 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/cut.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5302 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/date.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3635 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/devmem.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6395 2024-02-06 14:47:26.000000 moler-3.6.0/moler/cmd/unix/df.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4384 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/dmesg.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4325 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/du.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4189 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/echo.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1077 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/unix/enter.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6135 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/unix/env.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10518 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ethtool.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1799 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/unix/exit.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3769 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/unix/exit_telnet.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6520 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/export.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8513 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/find.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12697 2024-04-09 06:59:25.000000 moler-3.6.0/moler/cmd/unix/generictelnetssh.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6381 2024-04-11 12:09:37.000000 moler-3.6.0/moler/cmd/unix/genericunix.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9240 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/grep.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6109 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/gunzip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4691 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/gzip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7087 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/hciconfig.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4606 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/head.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4428 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/hexdump.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2527 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/unix/history.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1417 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/hostname.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4940 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/id.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20386 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ifconfig.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6319 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ip_addr.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6423 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ip_link.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6554 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ip_neigh.py
--rw-r--r--   0 ute       (1000) ute       (1000)    19050 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ip_route.py
--rw-r--r--   0 ute       (1000) ute       (1000)    40999 2024-03-01 08:45:11.000000 moler-3.6.0/moler/cmd/unix/iperf.py
--rw-r--r--   0 ute       (1000) ute       (1000)    96255 2024-03-01 08:01:14.000000 moler-3.6.0/moler/cmd/unix/iperf2.py
--rw-r--r--   0 ute       (1000) ute       (1000)   184934 2024-04-15 07:32:05.000000 moler-3.6.0/moler/cmd/unix/iperf3.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17415 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ipsec.py
--rw-r--r--   0 ute       (1000) ute       (1000)    60585 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/iptables.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2096 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/kill.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2642 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/killall.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1545 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ln.py
--rw-r--r--   0 ute       (1000) ute       (1000)      432 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/unix/logout.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17144 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ls.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8656 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/lsof.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6108 2024-04-15 07:32:05.000000 moler-3.6.0/moler/cmd/unix/lxc_attach.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7388 2024-04-15 07:32:05.000000 moler-3.6.0/moler/cmd/unix/lxc_info.py
--rw-r--r--   0 ute       (1000) ute       (1000)    19814 2024-04-15 07:32:05.000000 moler-3.6.0/moler/cmd/unix/lxc_ls.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1677 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/md5sum.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1854 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/mkdir.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5082 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/mount.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5753 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/mpstat.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1986 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/mv.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20213 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/netstat.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7517 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/nft.py
--rw-r--r--   0 ute       (1000) ute       (1000)    39366 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/nmap.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12330 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/nping.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5168 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ntpq.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3907 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/openssl_s_client.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8259 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/openssl_x509_text_in.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9153 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/passwd.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17005 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ping.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1352 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/pkill.py
--rw-r--r--   0 ute       (1000) ute       (1000)    18616 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ps.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2609 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/pwd.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3048 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/unix/reboot.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1706 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/rm.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7861 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/route.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4494 2024-03-18 09:44:23.000000 moler-3.6.0/moler/cmd/unix/run_script.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3743 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/run_serial_proxy.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12696 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/scp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4191 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/sed.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8652 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/service.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10793 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/sftp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4883 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/shasum.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6854 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/socat.py
--rw-r--r--   0 ute       (1000) ute       (1000)    13026 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/ss.py
--rw-r--r--   0 ute       (1000) ute       (1000)    45119 2024-05-07 12:40:55.000000 moler-3.6.0/moler/cmd/unix/ssh.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4910 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/sshkeygen.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7152 2024-05-07 12:40:55.000000 moler-3.6.0/moler/cmd/unix/su.py
--rw-r--r--   0 ute       (1000) ute       (1000)    21553 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/sudo.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1139 2024-02-06 08:16:12.000000 moler-3.6.0/moler/cmd/unix/sync.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3488 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/sysctl.py
--rw-r--r--   0 ute       (1000) ute       (1000)    16285 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/systemctl.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2509 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/tail.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5810 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/tail_latest_file.py
--rw-r--r--   0 ute       (1000) ute       (1000)      927 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/tar.py
--rw-r--r--   0 ute       (1000) ute       (1000)    25812 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/tcpdump.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3071 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/tee.py
--rw-r--r--   0 ute       (1000) ute       (1000)    19398 2024-05-07 12:40:55.000000 moler-3.6.0/moler/cmd/unix/telnet.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17342 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/top.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1686 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/touch.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7982 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/traceroute.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10992 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/tshark.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2890 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/uname.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1788 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/unxz.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10632 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/unzip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7243 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/uptime.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2946 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/useradd.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3577 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/userdel.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9935 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/w.py
--rw-r--r--   0 ute       (1000) ute       (1000)    40990 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/wget.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3125 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/which.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1215 2024-02-15 14:32:06.000000 moler-3.6.0/moler/cmd/unix/whoami.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1907 2024-02-19 07:54:48.000000 moler-3.6.0/moler/cmd/unix/zip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2785 2024-02-19 07:54:48.000000 moler-3.6.0/moler/command.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9032 2024-02-19 07:54:48.000000 moler-3.6.0/moler/command_scheduler.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.394288 moler-3.6.0/moler/config/
--rw-r--r--   0 ute       (1000) ute       (1000)    12409 2024-03-06 09:25:24.000000 moler-3.6.0/moler/config/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)    11652 2024-02-19 07:54:48.000000 moler-3.6.0/moler/config/connections.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1534 2024-02-06 14:47:26.000000 moler-3.6.0/moler/config/devices.py
--rw-r--r--   0 ute       (1000) ute       (1000)    34448 2024-05-07 07:25:07.000000 moler-3.6.0/moler/config/loggers.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1589 2024-02-06 14:47:26.000000 moler-3.6.0/moler/config/runners.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1594 2024-02-06 08:16:12.000000 moler-3.6.0/moler/connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8517 2024-02-19 07:54:48.000000 moler-3.6.0/moler/connection_factory.py
--rw-r--r--   0 ute       (1000) ute       (1000)    21922 2024-03-11 12:51:33.000000 moler-3.6.0/moler/connection_observer.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.414288 moler-3.6.0/moler/device/
--rw-r--r--   0 ute       (1000) ute       (1000)      425 2024-02-06 08:16:12.000000 moler-3.6.0/moler/device/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7195 2024-04-15 07:32:05.000000 moler-3.6.0/moler/device/abstract_device.py
--rw-r--r--   0 ute       (1000) ute       (1000)    16037 2024-04-15 07:32:05.000000 moler-3.6.0/moler/device/adbremote.py
--rw-r--r--   0 ute       (1000) ute       (1000)    22496 2024-04-15 07:32:05.000000 moler-3.6.0/moler/device/adbremote2.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10575 2024-04-15 07:32:05.000000 moler-3.6.0/moler/device/atremote.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20904 2024-02-19 07:54:48.000000 moler-3.6.0/moler/device/device.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1663 2024-04-15 07:32:05.000000 moler-3.6.0/moler/device/juniper_ex.py
--rw-r--r--   0 ute       (1000) ute       (1000)    14312 2024-02-06 08:16:12.000000 moler-3.6.0/moler/device/junipergeneric.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12333 2024-04-15 07:32:05.000000 moler-3.6.0/moler/device/pdu_aten.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10797 2024-02-06 08:16:12.000000 moler-3.6.0/moler/device/proxy_pc.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20245 2024-04-15 07:32:05.000000 moler-3.6.0/moler/device/proxy_pc2.py
--rw-r--r--   0 ute       (1000) ute       (1000)    11991 2024-04-15 07:32:05.000000 moler-3.6.0/moler/device/scpi.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2339 2024-04-24 13:48:30.000000 moler-3.6.0/moler/device/state_machine.py
--rw-r--r--   0 ute       (1000) ute       (1000)    46387 2024-05-07 12:40:55.000000 moler-3.6.0/moler/device/textualdevice.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10092 2024-05-07 12:40:55.000000 moler-3.6.0/moler/device/unixlocal.py
--rw-r--r--   0 ute       (1000) ute       (1000)    19845 2024-04-15 07:32:05.000000 moler-3.6.0/moler/device/unixremote.py
--rw-r--r--   0 ute       (1000) ute       (1000)    25983 2024-04-15 07:32:05.000000 moler-3.6.0/moler/device/unixremote2.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6418 2024-04-16 11:44:52.000000 moler-3.6.0/moler/event.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5038 2024-04-15 07:32:05.000000 moler-3.6.0/moler/event_awaiter.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.414288 moler-3.6.0/moler/events/
--rw-r--r--   0 ute       (1000) ute       (1000)      134 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.414288 moler-3.6.0/moler/events/juniper/
--rw-r--r--   0 ute       (1000) ute       (1000)      193 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/juniper/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      898 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/juniper/genericshared_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      324 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/juniper/genericshared_textualevent.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.426288 moler-3.6.0/moler/events/juniper_ex/
--rw-r--r--   0 ute       (1000) ute       (1000)      195 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/juniper_ex/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      903 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/juniper_ex/genericjuniper_ex_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      336 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/juniper_ex/genericjuniper_ex_textualevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7401 2024-02-19 07:54:48.000000 moler-3.6.0/moler/events/lineevent.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.426288 moler-3.6.0/moler/events/pdu_aten/
--rw-r--r--   0 ute       (1000) ute       (1000)      190 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/pdu_aten/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.426288 moler-3.6.0/moler/events/scpi/
--rw-r--r--   0 ute       (1000) ute       (1000)      186 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/scpi/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      892 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/scpi/genericscpi_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      325 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/scpi/genericscpi_textualevent.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.430288 moler-3.6.0/moler/events/shared/
--rw-r--r--   0 ute       (1000) ute       (1000)      180 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/shared/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1241 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/shared/genericshared_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      673 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/shared/genericshared_textualevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2227 2024-02-06 14:47:26.000000 moler-3.6.0/moler/events/shared/password_prompt.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5516 2024-02-06 14:47:26.000000 moler-3.6.0/moler/events/shared/wait4.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5819 2024-04-15 10:55:18.000000 moler-3.6.0/moler/events/textualevent.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.434288 moler-3.6.0/moler/events/unix/
--rw-r--r--   0 ute       (1000) ute       (1000)      188 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/unix/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2185 2024-02-06 14:47:26.000000 moler-3.6.0/moler/events/unix/advise_to_change_your_password.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2236 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/unix/failed_login_counter.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1243 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/unix/genericunix_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      675 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/unix/genericunix_textualevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      997 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/unix/last_failed_login.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2968 2024-02-19 07:54:48.000000 moler-3.6.0/moler/events/unix/last_login.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4734 2024-02-06 14:47:26.000000 moler-3.6.0/moler/events/unix/ping_no_response.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2302 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/unix/ping_response.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3599 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/unix/private_system.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1317 2024-02-06 14:47:26.000000 moler-3.6.0/moler/events/unix/shutdown.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4641 2024-04-15 07:32:05.000000 moler-3.6.0/moler/events/unix/u_boot_crtm.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1463 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/unix/wait4prompt.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4289 2024-02-19 07:54:48.000000 moler-3.6.0/moler/events/unix/wait4prompts.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1756 2024-02-06 08:16:12.000000 moler-3.6.0/moler/events/unix/warning_default_password.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5760 2024-02-19 07:54:48.000000 moler-3.6.0/moler/exceptions.py
--rw-r--r--   0 ute       (1000) ute       (1000)    18298 2024-04-11 12:09:37.000000 moler-3.6.0/moler/helpers.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3176 2024-02-19 07:54:48.000000 moler-3.6.0/moler/instance_loader.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.434288 moler-3.6.0/moler/io/
--rw-r--r--   0 ute       (1000) ute       (1000)      499 2024-02-06 08:16:12.000000 moler-3.6.0/moler/io/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.434288 moler-3.6.0/moler/io/asyncio/
--rw-r--r--   0 ute       (1000) ute       (1000)      536 2024-02-06 14:47:26.000000 moler-3.6.0/moler/io/asyncio/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5954 2024-02-19 07:54:48.000000 moler-3.6.0/moler/io/asyncio/tcp.py
--rw-r--r--   0 ute       (1000) ute       (1000)    14931 2024-02-19 07:54:48.000000 moler-3.6.0/moler/io/asyncio/terminal.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7222 2024-02-19 07:54:48.000000 moler-3.6.0/moler/io/io_connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2156 2024-02-19 07:54:48.000000 moler-3.6.0/moler/io/io_exceptions.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.438288 moler-3.6.0/moler/io/raw/
--rw-r--r--   0 ute       (1000) ute       (1000)     1320 2024-02-19 07:54:48.000000 moler-3.6.0/moler/io/raw/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9652 2024-02-19 07:54:48.000000 moler-3.6.0/moler/io/raw/memory.py
--rw-r--r--   0 ute       (1000) ute       (1000)    22609 2024-02-19 07:54:48.000000 moler-3.6.0/moler/io/raw/sshshell.py
--rw-r--r--   0 ute       (1000) ute       (1000)      741 2024-02-06 14:47:26.000000 moler-3.6.0/moler/io/raw/subprocess.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7554 2024-02-19 07:54:48.000000 moler-3.6.0/moler/io/raw/tcp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9922 2024-02-19 07:54:48.000000 moler-3.6.0/moler/io/raw/tcpserverpiped.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7325 2024-02-19 07:54:48.000000 moler-3.6.0/moler/io/raw/terminal.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5679 2024-02-06 14:47:26.000000 moler-3.6.0/moler/moler_connection_for_single_thread_runner.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1672 2024-02-06 08:16:12.000000 moler-3.6.0/moler/observable_connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4597 2024-02-19 07:54:48.000000 moler-3.6.0/moler/observer_thread_wrapper.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.438288 moler-3.6.0/moler/parser/
--rw-r--r--   0 ute       (1000) ute       (1000)      141 2024-02-06 08:16:12.000000 moler-3.6.0/moler/parser/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)    18616 2024-04-15 07:32:05.000000 moler-3.6.0/moler/parser/table_text.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5503 2024-02-06 14:47:26.000000 moler-3.6.0/moler/publisher.py
--rw-r--r--   0 ute       (1000) ute       (1000)    37230 2024-03-06 09:47:05.000000 moler-3.6.0/moler/runner.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3910 2024-02-19 07:54:48.000000 moler-3.6.0/moler/runner_factory.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20412 2024-02-19 07:54:48.000000 moler-3.6.0/moler/runner_single_thread.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6890 2024-04-15 07:32:05.000000 moler-3.6.0/moler/scheduler.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8824 2024-02-19 07:54:48.000000 moler-3.6.0/moler/threaded_moler_connection.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.442288 moler-3.6.0/moler/util/
--rw-r--r--   0 ute       (1000) ute       (1000)      138 2024-02-06 08:16:12.000000 moler-3.6.0/moler/util/__init__.py
--rwxr-xr-x   0 ute       (1000) ute       (1000)    13467 2024-05-07 12:40:55.000000 moler-3.6.0/moler/util/cmds_events_doc.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2581 2024-02-19 07:54:48.000000 moler-3.6.0/moler/util/compressed_rotating_file_handler.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1405 2024-02-19 07:54:48.000000 moler-3.6.0/moler/util/compressed_timed_rotating_file_handler.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1255 2024-02-19 07:54:48.000000 moler-3.6.0/moler/util/connection_observer.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3436 2024-02-14 14:53:24.000000 moler-3.6.0/moler/util/connection_observer_life_status.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4520 2024-02-19 07:54:48.000000 moler-3.6.0/moler/util/converterhelper.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12577 2024-04-25 12:15:39.000000 moler-3.6.0/moler/util/devices_SM.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2987 2024-02-06 14:47:26.000000 moler-3.6.0/moler/util/loghelper.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9386 2024-02-19 07:54:48.000000 moler-3.6.0/moler/util/moler_serial_proxy.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10038 2024-04-15 07:32:05.000000 moler-3.6.0/moler/util/moler_test.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1973 2024-02-19 07:54:48.000000 moler-3.6.0/moler/util/tracked_thread.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.454288 moler-3.6.0/moler.egg-info/
--rw-r--r--   0 ute       (1000) ute       (1000)    26591 2024-05-07 12:42:27.000000 moler-3.6.0/moler.egg-info/PKG-INFO
--rw-r--r--   0 ute       (1000) ute       (1000)     8786 2024-05-07 12:42:27.000000 moler-3.6.0/moler.egg-info/SOURCES.txt
--rw-r--r--   0 ute       (1000) ute       (1000)        1 2024-05-07 12:42:27.000000 moler-3.6.0/moler.egg-info/dependency_links.txt
--rw-r--r--   0 ute       (1000) ute       (1000)      157 2024-05-07 12:42:27.000000 moler-3.6.0/moler.egg-info/requires.txt
--rw-r--r--   0 ute       (1000) ute       (1000)        6 2024-05-07 12:42:27.000000 moler-3.6.0/moler.egg-info/top_level.txt
--rw-r--r--   0 ute       (1000) ute       (1000)      165 2024-05-07 12:42:27.454288 moler-3.6.0/setup.cfg
--rw-r--r--   0 ute       (1000) ute       (1000)     1966 2024-05-07 12:40:55.000000 moler-3.6.0/setup.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-07 12:42:27.450288 moler-3.6.0/test/
--rw-r--r--   0 ute       (1000) ute       (1000)    10233 2024-02-06 08:16:12.000000 moler-3.6.0/test/test_cmds_events_doc.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10694 2024-02-19 07:54:48.000000 moler-3.6.0/test/test_command.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20821 2024-02-19 07:54:48.000000 moler-3.6.0/test/test_connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8679 2024-02-06 08:16:12.000000 moler-3.6.0/test/test_connection_configuration.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5284 2024-02-06 08:16:12.000000 moler-3.6.0/test/test_connection_factory.py
--rw-r--r--   0 ute       (1000) ute       (1000)    24667 2024-02-19 07:54:48.000000 moler-3.6.0/test/test_connection_observer.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8313 2024-02-19 07:54:48.000000 moler-3.6.0/test/test_event.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4828 2024-03-06 09:25:24.000000 moler-3.6.0/test/test_event_awaiter.py
--rw-r--r--   0 ute       (1000) ute       (1000)    13445 2024-02-19 07:54:48.000000 moler-3.6.0/test/test_helpers.py
--rw-r--r--   0 ute       (1000) ute       (1000)    15345 2024-02-19 07:54:48.000000 moler-3.6.0/test/test_loggers.py
--rw-r--r--   0 ute       (1000) ute       (1000)      474 2024-02-06 08:16:12.000000 moler-3.6.0/test/test_moler_sleep.py
--rw-r--r--   0 ute       (1000) ute       (1000)    18464 2024-02-06 08:16:12.000000 moler-3.6.0/test/test_moler_test.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9533 2024-02-06 08:16:12.000000 moler-3.6.0/test/test_publisher.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8171 2024-02-19 07:54:48.000000 moler-3.6.0/test/test_runner.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3908 2024-03-01 08:45:11.000000 moler-3.6.0/test/test_scheduler.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2845 2024-02-06 08:16:12.000000 moler-3.6.0/test/test_table_read_parser.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4260 2024-02-06 08:16:12.000000 moler-3.6.0/test/test_util_loghelper.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.736000 moler-3.7.0/
+-rw-r--r--   0 ute       (1000) ute       (1000)     1505 2024-05-15 12:51:33.000000 moler-3.7.0/LICENSE
+-rw-r--r--   0 ute       (1000) ute       (1000)    26591 2024-05-15 13:33:43.736000 moler-3.7.0/PKG-INFO
+-rw-r--r--   0 ute       (1000) ute       (1000)    24908 2024-05-15 13:33:25.000000 moler-3.7.0/README.md
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.680000 moler-3.7.0/moler/
+-rw-r--r--   0 ute       (1000) ute       (1000)      143 2024-05-15 12:51:33.000000 moler-3.7.0/moler/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10606 2024-05-15 12:51:33.000000 moler-3.7.0/moler/abstract_moler_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    49062 2024-05-15 12:51:33.000000 moler-3.7.0/moler/asyncio_runner.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.684000 moler-3.7.0/moler/cmd/
+-rw-r--r--   0 ute       (1000) ute       (1000)     4140 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.688000 moler-3.7.0/moler/cmd/adb/
+-rw-r--r--   0 ute       (1000) ute       (1000)      191 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/adb/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5686 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/adb/adb_shell.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      331 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/adb/generic_adb_command.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.700000 moler-3.7.0/moler/cmd/at/
+-rw-r--r--   0 ute       (1000) ute       (1000)      369 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1588 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/at.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1553 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/attach.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1826 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/create_pdu_session.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3604 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/cu.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1526 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/detach.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1878 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/enable_echo.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2808 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/exit_serial_proxy.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3786 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/genericat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5005 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_apns.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3062 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_attach_state.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4770 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_cell_id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9134 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_cell_id_gprs.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8605 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_cell_id_lte.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6797 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_cell_id_nr.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2792 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_functionality_level.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5945 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_imei.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2654 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_imsi.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3226 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_ip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3125 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_manufacturer_id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5128 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_product_info.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3294 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/get_revision_id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3555 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/plink_serial.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2361 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/quectel_lock_nr_earfcn.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2459 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/quectel_network_preferences.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1828 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/release_pdu_session.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4632 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/run_script.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2570 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/set_apn.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2454 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/set_cell_id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3066 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/set_cell_id_gprs.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3056 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/set_cell_id_lte.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2741 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/set_cell_id_nr.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3367 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/set_functionality_level.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2231 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/at/set_mode.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    13384 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/commandchangingprompt.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    28640 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/commandtextualgeneric.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.700000 moler-3.7.0/moler/cmd/juniper/
+-rw-r--r--   0 ute       (1000) ute       (1000)      195 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/juniper/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.700000 moler-3.7.0/moler/cmd/juniper/cli/
+-rw-r--r--   0 ute       (1000) ute       (1000)      199 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/juniper/cli/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2571 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/juniper/cli/configure.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.700000 moler-3.7.0/moler/cmd/juniper/configure/
+-rw-r--r--   0 ute       (1000) ute       (1000)      205 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/juniper/configure/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2616 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/juniper/configure/exit_configure.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      993 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/juniper/genericjuniper.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.700000 moler-3.7.0/moler/cmd/juniper_ex/
+-rw-r--r--   0 ute       (1000) ute       (1000)      197 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/juniper_ex/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.700000 moler-3.7.0/moler/cmd/juniper_ex/cli/
+-rw-r--r--   0 ute       (1000) ute       (1000)      201 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/juniper_ex/cli/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.700000 moler-3.7.0/moler/cmd/juniper_ex/configure/
+-rw-r--r--   0 ute       (1000) ute       (1000)      207 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/juniper_ex/configure/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      404 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/juniper_ex/genericjuniperex.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.700000 moler-3.7.0/moler/cmd/pdu_aten/
+-rw-r--r--   0 ute       (1000) ute       (1000)      192 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/pdu_aten/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      904 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/pdu_aten/generic_pdu_aten.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.700000 moler-3.7.0/moler/cmd/pdu_aten/pdu/
+-rw-r--r--   0 ute       (1000) ute       (1000)      205 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/pdu_aten/pdu/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      415 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/pdu_aten/pdu/exit_telnet.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1193 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/pdu_aten/pdu/generic_pdu.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1589 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/pdu_aten/pdu/quit.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2895 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/pdu_aten/pdu/read_meter.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2948 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/pdu_aten/pdu/read_status.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1870 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/pdu_aten/pdu/sw.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.700000 moler-3.7.0/moler/cmd/scpi/
+-rw-r--r--   0 ute       (1000) ute       (1000)      188 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/scpi/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      370 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/scpi/genricscpi.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.704000 moler-3.7.0/moler/cmd/scpi/scpi/
+-rw-r--r--   0 ute       (1000) ute       (1000)      202 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/scpi/scpi/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      415 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/scpi/scpi/exit_telnet.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      969 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/scpi/scpi/genericscpistate.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1378 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/scpi/scpi/idn.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1598 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/scpi/scpi/read.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1921 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/scpi/scpi/run_command.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.724000 moler-3.7.0/moler/cmd/unix/
+-rw-r--r--   0 ute       (1000) ute       (1000)      194 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4744 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/adb_devices.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1957 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/adb_forward.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1465 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/adb_root.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1201 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/bash.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6135 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/cat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3342 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/cd.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2004 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/chgrp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2158 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/chmod.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2507 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/chown.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1650 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/cp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2807 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ctrl_c.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2459 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ctrl_z.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3554 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/cut.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5302 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/date.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3635 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/devmem.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6395 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/df.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4384 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/dmesg.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4325 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/du.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4189 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/echo.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1077 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/enter.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6135 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/env.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10518 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ethtool.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1799 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/exit.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3769 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/exit_telnet.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6520 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/export.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8513 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/find.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12697 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/generictelnetssh.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6381 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/genericunix.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9240 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/grep.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6109 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/gunzip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4691 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/gzip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7087 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/hciconfig.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4606 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/head.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4428 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/hexdump.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2527 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/history.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1417 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/hostname.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4940 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20386 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ifconfig.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6319 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ip_addr.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6423 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ip_link.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6554 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ip_neigh.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    19050 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ip_route.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    40999 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/iperf.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    96255 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/iperf2.py
+-rw-r--r--   0 ute       (1000) ute       (1000)   185020 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/iperf3.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17415 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ipsec.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    60585 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/iptables.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2096 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/kill.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2642 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/killall.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1545 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ln.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      432 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/logout.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17144 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ls.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8656 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/lsof.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6108 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/lxc_attach.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7388 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/lxc_info.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    19814 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/lxc_ls.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1677 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/md5sum.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1854 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/mkdir.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5082 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/mount.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5753 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/mpstat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1986 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/mv.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20213 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/netstat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7517 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/nft.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    39366 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/nmap.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12330 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/nping.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5168 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ntpq.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3907 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/openssl_s_client.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8259 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/openssl_x509_text_in.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9153 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/passwd.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17005 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ping.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1352 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/pkill.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    18616 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ps.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2609 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/pwd.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3048 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/reboot.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1706 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/rm.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7861 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/route.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4494 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/run_script.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3743 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/run_serial_proxy.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12696 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/scp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4191 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/sed.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8652 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/service.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10793 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/sftp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4883 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/shasum.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6854 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/socat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    13026 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ss.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    45119 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/ssh.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4910 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/sshkeygen.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7152 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/su.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    21553 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/sudo.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1139 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/sync.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3488 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/sysctl.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    16285 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/systemctl.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2509 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/tail.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5810 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/tail_latest_file.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      927 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/tar.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    25812 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/tcpdump.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3071 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/tee.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    19398 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/telnet.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17342 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/top.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1686 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/touch.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7982 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/traceroute.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10992 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/tshark.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2890 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/uname.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1788 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/unxz.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10632 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/unzip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7243 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/uptime.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2946 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/useradd.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3577 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/userdel.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9935 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/w.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    40990 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/wget.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3125 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/which.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1215 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/whoami.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1907 2024-05-15 12:51:33.000000 moler-3.7.0/moler/cmd/unix/zip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2785 2024-05-15 12:51:33.000000 moler-3.7.0/moler/command.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9032 2024-05-15 12:51:33.000000 moler-3.7.0/moler/command_scheduler.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.724000 moler-3.7.0/moler/config/
+-rw-r--r--   0 ute       (1000) ute       (1000)    12409 2024-05-15 12:51:33.000000 moler-3.7.0/moler/config/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    11652 2024-05-15 12:51:33.000000 moler-3.7.0/moler/config/connections.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1534 2024-05-15 12:51:33.000000 moler-3.7.0/moler/config/devices.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    34448 2024-05-15 12:51:33.000000 moler-3.7.0/moler/config/loggers.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1589 2024-05-15 12:51:33.000000 moler-3.7.0/moler/config/runners.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1594 2024-05-15 12:51:33.000000 moler-3.7.0/moler/connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8517 2024-05-15 12:51:33.000000 moler-3.7.0/moler/connection_factory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    21922 2024-05-15 12:51:33.000000 moler-3.7.0/moler/connection_observer.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.728000 moler-3.7.0/moler/device/
+-rw-r--r--   0 ute       (1000) ute       (1000)      425 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7195 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/abstract_device.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    16037 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/adbremote.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    22496 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/adbremote2.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10575 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/atremote.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20904 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/device.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1663 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/juniper_ex.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    14312 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/junipergeneric.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12333 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/pdu_aten.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10797 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/proxy_pc.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20245 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/proxy_pc2.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    11991 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/scpi.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2339 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/state_machine.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    46387 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/textualdevice.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10092 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/unixlocal.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    19845 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/unixremote.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    25983 2024-05-15 12:51:33.000000 moler-3.7.0/moler/device/unixremote2.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6418 2024-05-15 12:51:33.000000 moler-3.7.0/moler/event.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5038 2024-05-15 12:51:33.000000 moler-3.7.0/moler/event_awaiter.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.728000 moler-3.7.0/moler/events/
+-rw-r--r--   0 ute       (1000) ute       (1000)      134 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.728000 moler-3.7.0/moler/events/juniper/
+-rw-r--r--   0 ute       (1000) ute       (1000)      193 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/juniper/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      898 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/juniper/genericshared_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      324 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/juniper/genericshared_textualevent.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.728000 moler-3.7.0/moler/events/juniper_ex/
+-rw-r--r--   0 ute       (1000) ute       (1000)      195 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/juniper_ex/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      903 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/juniper_ex/genericjuniper_ex_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      336 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/juniper_ex/genericjuniper_ex_textualevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7401 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/lineevent.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.728000 moler-3.7.0/moler/events/pdu_aten/
+-rw-r--r--   0 ute       (1000) ute       (1000)      190 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/pdu_aten/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.728000 moler-3.7.0/moler/events/scpi/
+-rw-r--r--   0 ute       (1000) ute       (1000)      186 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/scpi/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      892 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/scpi/genericscpi_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      325 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/scpi/genericscpi_textualevent.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.728000 moler-3.7.0/moler/events/shared/
+-rw-r--r--   0 ute       (1000) ute       (1000)      180 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/shared/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1241 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/shared/genericshared_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      673 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/shared/genericshared_textualevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2227 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/shared/password_prompt.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5516 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/shared/wait4.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5819 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/textualevent.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.732000 moler-3.7.0/moler/events/unix/
+-rw-r--r--   0 ute       (1000) ute       (1000)      188 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2185 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/advise_to_change_your_password.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2236 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/failed_login_counter.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1243 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/genericunix_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      675 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/genericunix_textualevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      997 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/last_failed_login.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2968 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/last_login.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4734 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/ping_no_response.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2302 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/ping_response.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3599 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/private_system.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1317 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/shutdown.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4641 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/u_boot_crtm.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1463 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/wait4prompt.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4289 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/wait4prompts.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1756 2024-05-15 12:51:33.000000 moler-3.7.0/moler/events/unix/warning_default_password.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5760 2024-05-15 12:51:33.000000 moler-3.7.0/moler/exceptions.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    18298 2024-05-15 12:51:33.000000 moler-3.7.0/moler/helpers.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3176 2024-05-15 12:51:33.000000 moler-3.7.0/moler/instance_loader.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.732000 moler-3.7.0/moler/io/
+-rw-r--r--   0 ute       (1000) ute       (1000)      499 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.732000 moler-3.7.0/moler/io/asyncio/
+-rw-r--r--   0 ute       (1000) ute       (1000)      536 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/asyncio/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5954 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/asyncio/tcp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    14931 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/asyncio/terminal.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7222 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/io_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2156 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/io_exceptions.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.732000 moler-3.7.0/moler/io/raw/
+-rw-r--r--   0 ute       (1000) ute       (1000)     1320 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/raw/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9652 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/raw/memory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    22609 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/raw/sshshell.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      741 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/raw/subprocess.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7554 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/raw/tcp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9922 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/raw/tcpserverpiped.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7325 2024-05-15 12:51:33.000000 moler-3.7.0/moler/io/raw/terminal.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5679 2024-05-15 12:51:33.000000 moler-3.7.0/moler/moler_connection_for_single_thread_runner.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1672 2024-05-15 12:51:33.000000 moler-3.7.0/moler/observable_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4597 2024-05-15 12:51:33.000000 moler-3.7.0/moler/observer_thread_wrapper.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.732000 moler-3.7.0/moler/parser/
+-rw-r--r--   0 ute       (1000) ute       (1000)      141 2024-05-15 12:51:33.000000 moler-3.7.0/moler/parser/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    18616 2024-05-15 12:51:33.000000 moler-3.7.0/moler/parser/table_text.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5503 2024-05-15 12:51:33.000000 moler-3.7.0/moler/publisher.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    37230 2024-05-15 12:51:33.000000 moler-3.7.0/moler/runner.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3910 2024-05-15 12:51:33.000000 moler-3.7.0/moler/runner_factory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20412 2024-05-15 12:51:33.000000 moler-3.7.0/moler/runner_single_thread.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6890 2024-05-15 12:51:33.000000 moler-3.7.0/moler/scheduler.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8824 2024-05-15 12:51:33.000000 moler-3.7.0/moler/threaded_moler_connection.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.736000 moler-3.7.0/moler/util/
+-rw-r--r--   0 ute       (1000) ute       (1000)      138 2024-05-15 12:51:33.000000 moler-3.7.0/moler/util/__init__.py
+-rwxr-xr-x   0 ute       (1000) ute       (1000)    13467 2024-05-15 12:51:33.000000 moler-3.7.0/moler/util/cmds_events_doc.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2581 2024-05-15 12:51:33.000000 moler-3.7.0/moler/util/compressed_rotating_file_handler.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1405 2024-05-15 12:51:33.000000 moler-3.7.0/moler/util/compressed_timed_rotating_file_handler.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1255 2024-05-15 12:51:33.000000 moler-3.7.0/moler/util/connection_observer.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3436 2024-05-15 12:51:33.000000 moler-3.7.0/moler/util/connection_observer_life_status.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4520 2024-05-15 12:51:33.000000 moler-3.7.0/moler/util/converterhelper.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12577 2024-05-15 12:51:33.000000 moler-3.7.0/moler/util/devices_SM.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2987 2024-05-15 12:51:33.000000 moler-3.7.0/moler/util/loghelper.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9386 2024-05-15 12:51:33.000000 moler-3.7.0/moler/util/moler_serial_proxy.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10038 2024-05-15 12:51:33.000000 moler-3.7.0/moler/util/moler_test.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1973 2024-05-15 12:51:33.000000 moler-3.7.0/moler/util/tracked_thread.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.736000 moler-3.7.0/moler.egg-info/
+-rw-r--r--   0 ute       (1000) ute       (1000)    26591 2024-05-15 13:33:43.000000 moler-3.7.0/moler.egg-info/PKG-INFO
+-rw-r--r--   0 ute       (1000) ute       (1000)     8786 2024-05-15 13:33:43.000000 moler-3.7.0/moler.egg-info/SOURCES.txt
+-rw-r--r--   0 ute       (1000) ute       (1000)        1 2024-05-15 13:33:43.000000 moler-3.7.0/moler.egg-info/dependency_links.txt
+-rw-r--r--   0 ute       (1000) ute       (1000)      157 2024-05-15 13:33:43.000000 moler-3.7.0/moler.egg-info/requires.txt
+-rw-r--r--   0 ute       (1000) ute       (1000)        6 2024-05-15 13:33:43.000000 moler-3.7.0/moler.egg-info/top_level.txt
+-rw-r--r--   0 ute       (1000) ute       (1000)      165 2024-05-15 13:33:43.740000 moler-3.7.0/setup.cfg
+-rw-r--r--   0 ute       (1000) ute       (1000)     1966 2024-05-15 12:51:33.000000 moler-3.7.0/setup.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-05-15 13:33:43.736000 moler-3.7.0/test/
+-rw-r--r--   0 ute       (1000) ute       (1000)    10233 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_cmds_events_doc.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10694 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_command.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20821 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8679 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_connection_configuration.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5284 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_connection_factory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    24667 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_connection_observer.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8313 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_event.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4828 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_event_awaiter.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    13445 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_helpers.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    15345 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_loggers.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      474 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_moler_sleep.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    18464 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_moler_test.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9533 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_publisher.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8171 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_runner.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3908 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_scheduler.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2845 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_table_read_parser.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4260 2024-05-15 12:51:33.000000 moler-3.7.0/test/test_util_loghelper.py
```

### Comparing `moler-3.6.0/LICENSE` & `moler-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/PKG-INFO` & `moler-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moler
-Version: 3.6.0
+Version: 3.7.0
 Summary: Moler is a library for working with terminals, mainly for automated tests
 Home-page: https://github.com/nokia/moler
 Author: Nokia
 License: BSD 3-Clause
 Project-URL: Bug Reports, https://github.com/nokia/moler/issues
 Project-URL: Source, https://github.com/nokia/moler
 Keywords: testing development
@@ -38,15 +38,15 @@
 Requires-Dist: psutil
 Requires-Dist: python-dateutil
 Requires-Dist: pyserial
 Requires-Dist: cryptography
 Requires-Dist: paramiko
 Requires-Dist: importlib-metadata
 
-[![image](https://img.shields.io/badge/pypi-v3.6.0-blue.svg)](https://pypi.org/project/moler/)
+[![image](https://img.shields.io/badge/pypi-v3.7.0-blue.svg)](https://pypi.org/project/moler/)
 [![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/moler/)
 [![Build Status](https://github.com/nokia/moler/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/nokia/moler/actions)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](./LICENSE)
 
 # Table of Contents
 1. [Changelog](#changelog)
 2. [Moler info](#moler)
```

### Comparing `moler-3.6.0/README.md` & `moler-3.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![image](https://img.shields.io/badge/pypi-v3.6.0-blue.svg)](https://pypi.org/project/moler/)
+[![image](https://img.shields.io/badge/pypi-v3.7.0-blue.svg)](https://pypi.org/project/moler/)
 [![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/moler/)
 [![Build Status](https://github.com/nokia/moler/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/nokia/moler/actions)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](./LICENSE)
 
 # Table of Contents
 1. [Changelog](#changelog)
 2. [Moler info](#moler)
```

### Comparing `moler-3.6.0/moler/abstract_moler_connection.py` & `moler-3.7.0/moler/abstract_moler_connection.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/asyncio_runner.py` & `moler-3.7.0/moler/asyncio_runner.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/__init__.py` & `moler-3.7.0/moler/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/adb/adb_shell.py` & `moler-3.7.0/moler/cmd/adb/adb_shell.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/at.py` & `moler-3.7.0/moler/cmd/at/at.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/attach.py` & `moler-3.7.0/moler/cmd/at/attach.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/create_pdu_session.py` & `moler-3.7.0/moler/cmd/at/create_pdu_session.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/cu.py` & `moler-3.7.0/moler/cmd/at/cu.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/detach.py` & `moler-3.7.0/moler/cmd/at/detach.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/enable_echo.py` & `moler-3.7.0/moler/cmd/at/enable_echo.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/exit_serial_proxy.py` & `moler-3.7.0/moler/cmd/at/exit_serial_proxy.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/genericat.py` & `moler-3.7.0/moler/cmd/at/genericat.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_apns.py` & `moler-3.7.0/moler/cmd/at/get_apns.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_attach_state.py` & `moler-3.7.0/moler/cmd/at/get_attach_state.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_cell_id.py` & `moler-3.7.0/moler/cmd/at/get_cell_id.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_cell_id_gprs.py` & `moler-3.7.0/moler/cmd/at/get_cell_id_gprs.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_cell_id_lte.py` & `moler-3.7.0/moler/cmd/at/get_cell_id_lte.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_cell_id_nr.py` & `moler-3.7.0/moler/cmd/at/get_cell_id_nr.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_functionality_level.py` & `moler-3.7.0/moler/cmd/at/get_functionality_level.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_imei.py` & `moler-3.7.0/moler/cmd/at/get_imei.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_imsi.py` & `moler-3.7.0/moler/cmd/at/get_imsi.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_ip.py` & `moler-3.7.0/moler/cmd/at/get_ip.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_manufacturer_id.py` & `moler-3.7.0/moler/cmd/at/get_manufacturer_id.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_product_info.py` & `moler-3.7.0/moler/cmd/at/get_product_info.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/get_revision_id.py` & `moler-3.7.0/moler/cmd/at/get_revision_id.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/plink_serial.py` & `moler-3.7.0/moler/cmd/at/plink_serial.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/quectel_lock_nr_earfcn.py` & `moler-3.7.0/moler/cmd/at/quectel_lock_nr_earfcn.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/quectel_network_preferences.py` & `moler-3.7.0/moler/cmd/at/quectel_network_preferences.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/release_pdu_session.py` & `moler-3.7.0/moler/cmd/at/release_pdu_session.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/run_script.py` & `moler-3.7.0/moler/cmd/at/run_script.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/set_apn.py` & `moler-3.7.0/moler/cmd/at/set_apn.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/set_cell_id.py` & `moler-3.7.0/moler/cmd/at/set_cell_id.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/set_cell_id_gprs.py` & `moler-3.7.0/moler/cmd/at/set_cell_id_gprs.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/set_cell_id_lte.py` & `moler-3.7.0/moler/cmd/at/set_cell_id_lte.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/set_cell_id_nr.py` & `moler-3.7.0/moler/cmd/at/set_cell_id_nr.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/set_functionality_level.py` & `moler-3.7.0/moler/cmd/at/set_functionality_level.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/at/set_mode.py` & `moler-3.7.0/moler/cmd/at/set_mode.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/commandchangingprompt.py` & `moler-3.7.0/moler/cmd/commandchangingprompt.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/commandtextualgeneric.py` & `moler-3.7.0/moler/cmd/commandtextualgeneric.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/juniper/cli/configure.py` & `moler-3.7.0/moler/cmd/juniper/cli/configure.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/juniper/configure/exit_configure.py` & `moler-3.7.0/moler/cmd/juniper/configure/exit_configure.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/juniper/genericjuniper.py` & `moler-3.7.0/moler/cmd/juniper/genericjuniper.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/pdu_aten/generic_pdu_aten.py` & `moler-3.7.0/moler/cmd/pdu_aten/generic_pdu_aten.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/pdu_aten/pdu/generic_pdu.py` & `moler-3.7.0/moler/cmd/pdu_aten/pdu/generic_pdu.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/pdu_aten/pdu/quit.py` & `moler-3.7.0/moler/cmd/pdu_aten/pdu/quit.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/pdu_aten/pdu/read_meter.py` & `moler-3.7.0/moler/cmd/pdu_aten/pdu/read_meter.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/pdu_aten/pdu/read_status.py` & `moler-3.7.0/moler/cmd/pdu_aten/pdu/read_status.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/pdu_aten/pdu/sw.py` & `moler-3.7.0/moler/cmd/pdu_aten/pdu/sw.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/scpi/scpi/genericscpistate.py` & `moler-3.7.0/moler/cmd/scpi/scpi/genericscpistate.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/scpi/scpi/idn.py` & `moler-3.7.0/moler/cmd/scpi/scpi/idn.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/scpi/scpi/read.py` & `moler-3.7.0/moler/cmd/scpi/scpi/read.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/scpi/scpi/run_command.py` & `moler-3.7.0/moler/cmd/scpi/scpi/run_command.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/adb_devices.py` & `moler-3.7.0/moler/cmd/unix/adb_devices.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/adb_forward.py` & `moler-3.7.0/moler/cmd/unix/adb_forward.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/adb_root.py` & `moler-3.7.0/moler/cmd/unix/adb_root.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/bash.py` & `moler-3.7.0/moler/cmd/unix/bash.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/cat.py` & `moler-3.7.0/moler/cmd/unix/cat.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/cd.py` & `moler-3.7.0/moler/cmd/unix/cd.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/chgrp.py` & `moler-3.7.0/moler/cmd/unix/chgrp.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/chmod.py` & `moler-3.7.0/moler/cmd/unix/chmod.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/chown.py` & `moler-3.7.0/moler/cmd/unix/chown.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/cp.py` & `moler-3.7.0/moler/cmd/unix/cp.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ctrl_c.py` & `moler-3.7.0/moler/cmd/unix/ctrl_c.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ctrl_z.py` & `moler-3.7.0/moler/cmd/unix/ctrl_z.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/cut.py` & `moler-3.7.0/moler/cmd/unix/cut.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/date.py` & `moler-3.7.0/moler/cmd/unix/date.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/devmem.py` & `moler-3.7.0/moler/cmd/unix/devmem.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/df.py` & `moler-3.7.0/moler/cmd/unix/df.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/dmesg.py` & `moler-3.7.0/moler/cmd/unix/dmesg.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/du.py` & `moler-3.7.0/moler/cmd/unix/du.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/echo.py` & `moler-3.7.0/moler/cmd/unix/echo.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/enter.py` & `moler-3.7.0/moler/cmd/unix/enter.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/env.py` & `moler-3.7.0/moler/cmd/unix/env.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ethtool.py` & `moler-3.7.0/moler/cmd/unix/ethtool.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/exit.py` & `moler-3.7.0/moler/cmd/unix/exit.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/exit_telnet.py` & `moler-3.7.0/moler/cmd/unix/exit_telnet.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/export.py` & `moler-3.7.0/moler/cmd/unix/export.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/find.py` & `moler-3.7.0/moler/cmd/unix/find.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/generictelnetssh.py` & `moler-3.7.0/moler/cmd/unix/generictelnetssh.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/genericunix.py` & `moler-3.7.0/moler/cmd/unix/genericunix.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/grep.py` & `moler-3.7.0/moler/cmd/unix/grep.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/gunzip.py` & `moler-3.7.0/moler/cmd/unix/gunzip.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/gzip.py` & `moler-3.7.0/moler/cmd/unix/gzip.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/hciconfig.py` & `moler-3.7.0/moler/cmd/unix/hciconfig.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/head.py` & `moler-3.7.0/moler/cmd/unix/head.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/hexdump.py` & `moler-3.7.0/moler/cmd/unix/hexdump.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/history.py` & `moler-3.7.0/moler/cmd/unix/history.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/hostname.py` & `moler-3.7.0/moler/cmd/unix/hostname.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/id.py` & `moler-3.7.0/moler/cmd/unix/id.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ifconfig.py` & `moler-3.7.0/moler/cmd/unix/ifconfig.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ip_addr.py` & `moler-3.7.0/moler/cmd/unix/ip_addr.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ip_link.py` & `moler-3.7.0/moler/cmd/unix/ip_link.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ip_neigh.py` & `moler-3.7.0/moler/cmd/unix/ip_neigh.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ip_route.py` & `moler-3.7.0/moler/cmd/unix/ip_route.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/iperf.py` & `moler-3.7.0/moler/cmd/unix/iperf.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/iperf2.py` & `moler-3.7.0/moler/cmd/unix/iperf2.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/iperf3.py` & `moler-3.7.0/moler/cmd/unix/iperf3.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,16 @@
 
     # iperf3 output for: udp server
     # [ ID] Interval      Transfer      Bitrate      Jitter      Lost/Total Datagrams
 
     # iperf3 output for: udp client
     # [ ID] Interval      Transfer      Bitrate      Total Datagrams
 
-    _re_headers = re.compile(r"\[\s+ID\]\s+Interval\s+Transfer\s+Bitrate")
+    # for iperf3 versions <= 3.1.7 the Bitrate column was named Bandwidth
+    _re_headers = re.compile(r"\[\s+ID\]\s+Interval\s+Transfer\s+(Bitrate|Bandwidth)")
 
     def _parse_headers(self, line):
         if self._regex_helper.search_compiled(Iperf3._re_headers, line):
             if self.parallel_client:
                 client, server = list(self._connection_dict.values())[0]
                 # pylint: disable-next=unused-variable
                 (
```

### Comparing `moler-3.6.0/moler/cmd/unix/ipsec.py` & `moler-3.7.0/moler/cmd/unix/ipsec.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/iptables.py` & `moler-3.7.0/moler/cmd/unix/iptables.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/kill.py` & `moler-3.7.0/moler/cmd/unix/kill.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/killall.py` & `moler-3.7.0/moler/cmd/unix/killall.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ln.py` & `moler-3.7.0/moler/cmd/unix/ln.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ls.py` & `moler-3.7.0/moler/cmd/unix/ls.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/lsof.py` & `moler-3.7.0/moler/cmd/unix/lsof.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/lxc_attach.py` & `moler-3.7.0/moler/cmd/unix/lxc_attach.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/lxc_info.py` & `moler-3.7.0/moler/cmd/unix/lxc_info.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/lxc_ls.py` & `moler-3.7.0/moler/cmd/unix/lxc_ls.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/md5sum.py` & `moler-3.7.0/moler/cmd/unix/md5sum.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/mkdir.py` & `moler-3.7.0/moler/cmd/unix/mkdir.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/mount.py` & `moler-3.7.0/moler/cmd/unix/mount.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/mpstat.py` & `moler-3.7.0/moler/cmd/unix/mpstat.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/mv.py` & `moler-3.7.0/moler/cmd/unix/mv.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/netstat.py` & `moler-3.7.0/moler/cmd/unix/netstat.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/nft.py` & `moler-3.7.0/moler/cmd/unix/nft.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/nmap.py` & `moler-3.7.0/moler/cmd/unix/nmap.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/nping.py` & `moler-3.7.0/moler/cmd/unix/nping.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ntpq.py` & `moler-3.7.0/moler/cmd/unix/ntpq.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/openssl_s_client.py` & `moler-3.7.0/moler/cmd/unix/openssl_s_client.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/openssl_x509_text_in.py` & `moler-3.7.0/moler/cmd/unix/openssl_x509_text_in.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/passwd.py` & `moler-3.7.0/moler/cmd/unix/passwd.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ping.py` & `moler-3.7.0/moler/cmd/unix/ping.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/pkill.py` & `moler-3.7.0/moler/cmd/unix/pkill.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ps.py` & `moler-3.7.0/moler/cmd/unix/ps.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/pwd.py` & `moler-3.7.0/moler/cmd/unix/pwd.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/reboot.py` & `moler-3.7.0/moler/cmd/unix/reboot.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/rm.py` & `moler-3.7.0/moler/cmd/unix/rm.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/route.py` & `moler-3.7.0/moler/cmd/unix/route.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/run_script.py` & `moler-3.7.0/moler/cmd/unix/run_script.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/run_serial_proxy.py` & `moler-3.7.0/moler/cmd/unix/run_serial_proxy.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/scp.py` & `moler-3.7.0/moler/cmd/unix/scp.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/sed.py` & `moler-3.7.0/moler/cmd/unix/sed.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/service.py` & `moler-3.7.0/moler/cmd/unix/service.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/sftp.py` & `moler-3.7.0/moler/cmd/unix/sftp.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/shasum.py` & `moler-3.7.0/moler/cmd/unix/shasum.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/socat.py` & `moler-3.7.0/moler/cmd/unix/socat.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ss.py` & `moler-3.7.0/moler/cmd/unix/ss.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/ssh.py` & `moler-3.7.0/moler/cmd/unix/ssh.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/sshkeygen.py` & `moler-3.7.0/moler/cmd/unix/sshkeygen.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/su.py` & `moler-3.7.0/moler/cmd/unix/su.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/sudo.py` & `moler-3.7.0/moler/cmd/unix/sudo.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/sync.py` & `moler-3.7.0/moler/cmd/unix/sync.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/sysctl.py` & `moler-3.7.0/moler/cmd/unix/sysctl.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/systemctl.py` & `moler-3.7.0/moler/cmd/unix/systemctl.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/tail.py` & `moler-3.7.0/moler/cmd/unix/tail.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/tail_latest_file.py` & `moler-3.7.0/moler/cmd/unix/tail_latest_file.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/tar.py` & `moler-3.7.0/moler/cmd/unix/tar.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/tcpdump.py` & `moler-3.7.0/moler/cmd/unix/tcpdump.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/tee.py` & `moler-3.7.0/moler/cmd/unix/tee.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/telnet.py` & `moler-3.7.0/moler/cmd/unix/telnet.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/top.py` & `moler-3.7.0/moler/cmd/unix/top.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/touch.py` & `moler-3.7.0/moler/cmd/unix/touch.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/traceroute.py` & `moler-3.7.0/moler/cmd/unix/traceroute.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/tshark.py` & `moler-3.7.0/moler/cmd/unix/tshark.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/uname.py` & `moler-3.7.0/moler/cmd/unix/uname.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/unxz.py` & `moler-3.7.0/moler/cmd/unix/unxz.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/unzip.py` & `moler-3.7.0/moler/cmd/unix/unzip.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/uptime.py` & `moler-3.7.0/moler/cmd/unix/uptime.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/useradd.py` & `moler-3.7.0/moler/cmd/unix/useradd.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/userdel.py` & `moler-3.7.0/moler/cmd/unix/userdel.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/w.py` & `moler-3.7.0/moler/cmd/unix/w.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/wget.py` & `moler-3.7.0/moler/cmd/unix/wget.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/which.py` & `moler-3.7.0/moler/cmd/unix/which.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/whoami.py` & `moler-3.7.0/moler/cmd/unix/whoami.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/cmd/unix/zip.py` & `moler-3.7.0/moler/cmd/unix/zip.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/command.py` & `moler-3.7.0/moler/command.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/command_scheduler.py` & `moler-3.7.0/moler/command_scheduler.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/config/__init__.py` & `moler-3.7.0/moler/config/__init__.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/config/connections.py` & `moler-3.7.0/moler/config/connections.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/config/devices.py` & `moler-3.7.0/moler/config/devices.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/config/loggers.py` & `moler-3.7.0/moler/config/loggers.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/config/runners.py` & `moler-3.7.0/moler/config/runners.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/connection.py` & `moler-3.7.0/moler/connection.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/connection_factory.py` & `moler-3.7.0/moler/connection_factory.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/connection_observer.py` & `moler-3.7.0/moler/connection_observer.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/abstract_device.py` & `moler-3.7.0/moler/device/abstract_device.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/adbremote.py` & `moler-3.7.0/moler/device/adbremote.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/adbremote2.py` & `moler-3.7.0/moler/device/adbremote2.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/atremote.py` & `moler-3.7.0/moler/device/atremote.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/device.py` & `moler-3.7.0/moler/device/device.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/juniper_ex.py` & `moler-3.7.0/moler/device/juniper_ex.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/junipergeneric.py` & `moler-3.7.0/moler/device/junipergeneric.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/pdu_aten.py` & `moler-3.7.0/moler/device/pdu_aten.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/proxy_pc.py` & `moler-3.7.0/moler/device/proxy_pc.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/proxy_pc2.py` & `moler-3.7.0/moler/device/proxy_pc2.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/scpi.py` & `moler-3.7.0/moler/device/scpi.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/state_machine.py` & `moler-3.7.0/moler/device/state_machine.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/textualdevice.py` & `moler-3.7.0/moler/device/textualdevice.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/unixlocal.py` & `moler-3.7.0/moler/device/unixlocal.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/unixremote.py` & `moler-3.7.0/moler/device/unixremote.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/device/unixremote2.py` & `moler-3.7.0/moler/device/unixremote2.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/event.py` & `moler-3.7.0/moler/event.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/event_awaiter.py` & `moler-3.7.0/moler/event_awaiter.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/juniper/genericshared_lineevent.py` & `moler-3.7.0/moler/events/juniper/genericshared_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/juniper_ex/genericjuniper_ex_lineevent.py` & `moler-3.7.0/moler/events/juniper_ex/genericjuniper_ex_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/lineevent.py` & `moler-3.7.0/moler/events/lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/scpi/genericscpi_lineevent.py` & `moler-3.7.0/moler/events/scpi/genericscpi_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/shared/genericshared_lineevent.py` & `moler-3.7.0/moler/events/shared/genericshared_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/shared/genericshared_textualevent.py` & `moler-3.7.0/moler/events/shared/genericshared_textualevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/shared/password_prompt.py` & `moler-3.7.0/moler/events/shared/password_prompt.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/shared/wait4.py` & `moler-3.7.0/moler/events/shared/wait4.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/textualevent.py` & `moler-3.7.0/moler/events/textualevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/advise_to_change_your_password.py` & `moler-3.7.0/moler/events/unix/advise_to_change_your_password.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/failed_login_counter.py` & `moler-3.7.0/moler/events/unix/failed_login_counter.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/genericunix_lineevent.py` & `moler-3.7.0/moler/events/unix/genericunix_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/genericunix_textualevent.py` & `moler-3.7.0/moler/events/unix/genericunix_textualevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/last_failed_login.py` & `moler-3.7.0/moler/events/unix/last_failed_login.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/last_login.py` & `moler-3.7.0/moler/events/unix/last_login.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/ping_no_response.py` & `moler-3.7.0/moler/events/unix/ping_no_response.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/ping_response.py` & `moler-3.7.0/moler/events/unix/ping_response.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/private_system.py` & `moler-3.7.0/moler/events/unix/private_system.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/shutdown.py` & `moler-3.7.0/moler/events/unix/shutdown.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/u_boot_crtm.py` & `moler-3.7.0/moler/events/unix/u_boot_crtm.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/wait4prompt.py` & `moler-3.7.0/moler/events/unix/wait4prompt.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/wait4prompts.py` & `moler-3.7.0/moler/events/unix/wait4prompts.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/events/unix/warning_default_password.py` & `moler-3.7.0/moler/events/unix/warning_default_password.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/exceptions.py` & `moler-3.7.0/moler/exceptions.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/helpers.py` & `moler-3.7.0/moler/helpers.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/instance_loader.py` & `moler-3.7.0/moler/instance_loader.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/io/asyncio/__init__.py` & `moler-3.7.0/moler/io/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/io/asyncio/tcp.py` & `moler-3.7.0/moler/io/asyncio/tcp.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/io/asyncio/terminal.py` & `moler-3.7.0/moler/io/asyncio/terminal.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/io/io_connection.py` & `moler-3.7.0/moler/io/io_connection.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/io/io_exceptions.py` & `moler-3.7.0/moler/io/io_exceptions.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/io/raw/__init__.py` & `moler-3.7.0/moler/io/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/io/raw/memory.py` & `moler-3.7.0/moler/io/raw/memory.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/io/raw/sshshell.py` & `moler-3.7.0/moler/io/raw/sshshell.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/io/raw/subprocess.py` & `moler-3.7.0/moler/io/raw/subprocess.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/io/raw/tcp.py` & `moler-3.7.0/moler/io/raw/tcp.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/io/raw/tcpserverpiped.py` & `moler-3.7.0/moler/io/raw/tcpserverpiped.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/io/raw/terminal.py` & `moler-3.7.0/moler/io/raw/terminal.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/moler_connection_for_single_thread_runner.py` & `moler-3.7.0/moler/moler_connection_for_single_thread_runner.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/observable_connection.py` & `moler-3.7.0/moler/observable_connection.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/observer_thread_wrapper.py` & `moler-3.7.0/moler/observer_thread_wrapper.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/parser/table_text.py` & `moler-3.7.0/moler/parser/table_text.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/publisher.py` & `moler-3.7.0/moler/publisher.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/runner.py` & `moler-3.7.0/moler/runner.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/runner_factory.py` & `moler-3.7.0/moler/runner_factory.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/runner_single_thread.py` & `moler-3.7.0/moler/runner_single_thread.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/scheduler.py` & `moler-3.7.0/moler/scheduler.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/threaded_moler_connection.py` & `moler-3.7.0/moler/threaded_moler_connection.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/util/cmds_events_doc.py` & `moler-3.7.0/moler/util/cmds_events_doc.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/util/compressed_rotating_file_handler.py` & `moler-3.7.0/moler/util/compressed_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/util/compressed_timed_rotating_file_handler.py` & `moler-3.7.0/moler/util/compressed_timed_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/util/connection_observer.py` & `moler-3.7.0/moler/util/connection_observer.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/util/connection_observer_life_status.py` & `moler-3.7.0/moler/util/connection_observer_life_status.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/util/converterhelper.py` & `moler-3.7.0/moler/util/converterhelper.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/util/devices_SM.py` & `moler-3.7.0/moler/util/devices_SM.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/util/loghelper.py` & `moler-3.7.0/moler/util/loghelper.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/util/moler_serial_proxy.py` & `moler-3.7.0/moler/util/moler_serial_proxy.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/util/moler_test.py` & `moler-3.7.0/moler/util/moler_test.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler/util/tracked_thread.py` & `moler-3.7.0/moler/util/tracked_thread.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/moler.egg-info/PKG-INFO` & `moler-3.7.0/moler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moler
-Version: 3.6.0
+Version: 3.7.0
 Summary: Moler is a library for working with terminals, mainly for automated tests
 Home-page: https://github.com/nokia/moler
 Author: Nokia
 License: BSD 3-Clause
 Project-URL: Bug Reports, https://github.com/nokia/moler/issues
 Project-URL: Source, https://github.com/nokia/moler
 Keywords: testing development
@@ -38,15 +38,15 @@
 Requires-Dist: psutil
 Requires-Dist: python-dateutil
 Requires-Dist: pyserial
 Requires-Dist: cryptography
 Requires-Dist: paramiko
 Requires-Dist: importlib-metadata
 
-[![image](https://img.shields.io/badge/pypi-v3.6.0-blue.svg)](https://pypi.org/project/moler/)
+[![image](https://img.shields.io/badge/pypi-v3.7.0-blue.svg)](https://pypi.org/project/moler/)
 [![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/moler/)
 [![Build Status](https://github.com/nokia/moler/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/nokia/moler/actions)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](./LICENSE)
 
 # Table of Contents
 1. [Changelog](#changelog)
 2. [Moler info](#moler)
```

### Comparing `moler-3.6.0/moler.egg-info/SOURCES.txt` & `moler-3.7.0/moler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/setup.py` & `moler-3.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = f.read()
 
 with io.open(join(getcwd(), 'requirements', 'base.txt'), encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='moler',
-    version='3.6.0',
+    version='3.7.0',
     description='Moler is a library for working with terminals, mainly for automated tests',  # Required
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nokia/moler',
     author='Nokia',
     license='BSD 3-Clause',
     classifiers=[
```

### Comparing `moler-3.6.0/test/test_cmds_events_doc.py` & `moler-3.7.0/test/test_cmds_events_doc.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_command.py` & `moler-3.7.0/test/test_command.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_connection.py` & `moler-3.7.0/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_connection_configuration.py` & `moler-3.7.0/test/test_connection_configuration.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_connection_factory.py` & `moler-3.7.0/test/test_connection_factory.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_connection_observer.py` & `moler-3.7.0/test/test_connection_observer.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_event.py` & `moler-3.7.0/test/test_event.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_event_awaiter.py` & `moler-3.7.0/test/test_event_awaiter.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_helpers.py` & `moler-3.7.0/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_loggers.py` & `moler-3.7.0/test/test_loggers.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_moler_test.py` & `moler-3.7.0/test/test_moler_test.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_publisher.py` & `moler-3.7.0/test/test_publisher.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_runner.py` & `moler-3.7.0/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_scheduler.py` & `moler-3.7.0/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_table_read_parser.py` & `moler-3.7.0/test/test_table_read_parser.py`

 * *Files identical despite different names*

### Comparing `moler-3.6.0/test/test_util_loghelper.py` & `moler-3.7.0/test/test_util_loghelper.py`

 * *Files identical despite different names*

