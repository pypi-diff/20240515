# Comparing `tmp/grasp_planning-0.5.1.tar.gz` & `tmp/grasp_planning-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.5.1.tar", max compression
+gzip compressed data, was "grasp_planning-0.5.2.tar", max compression
```

## Comparing `grasp_planning-0.5.1.tar` & `grasp_planning-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1711 2024-05-14 12:21:39.645718 grasp_planning-0.5.1/README.md
--rw-r--r--   0        0        0      123 2024-05-07 16:34:01.834623 grasp_planning-0.5.1/grasp_planning/__init__.py
--rw-r--r--   0        0        0     1335 2024-05-13 14:27:59.161140 grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/collision_constraint.cpython-38.pyc
--rw-r--r--   0        0        0      799 2024-05-13 12:55:10.134092 grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/constraint_template.cpython-38.pyc
--rw-r--r--   0        0        0      411 2024-05-08 08:43:17.328729 grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/constraints.cpython-38.pyc
--rw-r--r--   0        0        0     1331 2024-05-13 12:55:10.134092 grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/grasp_pos_constraint.cpython-38.pyc
--rw-r--r--   0        0        0     1528 2024-05-13 13:10:01.879282 grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/grasp_rot_constraint.cpython-38.pyc
--rw-r--r--   0        0        0     1557 2024-05-09 15:57:33.554280 grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/manipulation_constraint.cpython-38.pyc
--rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884832 grasp_planning-0.5.1/grasp_planning/constraints/collision_constraint.py
--rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.1/grasp_planning/constraints/constraint_template.py
--rw-r--r--   0        0        0      252 2024-05-08 08:42:32.500427 grasp_planning-0.5.1/grasp_planning/constraints/constraints.py
--rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452309 grasp_planning-0.5.1/grasp_planning/constraints/grasp_pos_constraint.py
--rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.1/grasp_planning/constraints/grasp_rot_constraint.py
--rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.1/grasp_planning/constraints/manipulation_constraint.py
--rw-r--r--   0        0        0      219 2024-05-07 16:34:48.974947 grasp_planning-0.5.1/grasp_planning/cost/__pycache__/costs.cpython-38.pyc
--rw-r--r--   0        0        0     1344 2024-05-13 08:32:20.007123 grasp_planning-0.5.1/grasp_planning/cost/__pycache__/squared_acc_cost.cpython-38.pyc
--rw-r--r--   0        0        0       65 2024-05-07 16:34:01.834623 grasp_planning-0.5.1/grasp_planning/cost/costs.py
--rw-r--r--   0        0        0        0 2024-05-02 12:00:02.772313 grasp_planning-0.5.1/grasp_planning/cost/dist_to_home.py
--rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.1/grasp_planning/cost/squared_acc_cost.py
--rw-r--r--   0        0        0     5969 2024-05-14 13:19:55.752368 grasp_planning-0.5.1/grasp_planning/solver/__pycache__/gomp_planner.cpython-38.pyc
--rw-r--r--   0        0        0     2203 2024-05-13 13:26:57.783698 grasp_planning-0.5.1/grasp_planning/solver/__pycache__/robot_model.cpython-38.pyc
--rw-r--r--   0        0        0     7650 2024-05-14 13:19:53.464393 grasp_planning-0.5.1/grasp_planning/solver/gomp_planner.py
--rw-r--r--   0        0        0     1875 2024-05-13 13:26:55.591679 grasp_planning-0.5.1/grasp_planning/solver/robot_model.py
--rw-r--r--   0        0        0      450 2024-05-14 13:21:33.811293 grasp_planning-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 grasp_planning-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1711 2024-05-14 12:21:39.645718 grasp_planning-0.5.2/README.md
+-rw-r--r--   0        0        0      123 2024-05-07 16:34:01.834623 grasp_planning-0.5.2/grasp_planning/__init__.py
+-rw-r--r--   0        0        0     1335 2024-05-13 14:27:59.161140 grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/collision_constraint.cpython-38.pyc
+-rw-r--r--   0        0        0      799 2024-05-13 12:55:10.134092 grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/constraint_template.cpython-38.pyc
+-rw-r--r--   0        0        0      411 2024-05-08 08:43:17.328729 grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/constraints.cpython-38.pyc
+-rw-r--r--   0        0        0     1331 2024-05-13 12:55:10.134092 grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/grasp_pos_constraint.cpython-38.pyc
+-rw-r--r--   0        0        0     1528 2024-05-13 13:10:01.879282 grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/grasp_rot_constraint.cpython-38.pyc
+-rw-r--r--   0        0        0     1557 2024-05-09 15:57:33.554280 grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/manipulation_constraint.cpython-38.pyc
+-rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884832 grasp_planning-0.5.2/grasp_planning/constraints/collision_constraint.py
+-rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.2/grasp_planning/constraints/constraint_template.py
+-rw-r--r--   0        0        0      252 2024-05-08 08:42:32.500427 grasp_planning-0.5.2/grasp_planning/constraints/constraints.py
+-rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452309 grasp_planning-0.5.2/grasp_planning/constraints/grasp_pos_constraint.py
+-rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.2/grasp_planning/constraints/grasp_rot_constraint.py
+-rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.2/grasp_planning/constraints/manipulation_constraint.py
+-rw-r--r--   0        0        0      219 2024-05-07 16:34:48.974947 grasp_planning-0.5.2/grasp_planning/cost/__pycache__/costs.cpython-38.pyc
+-rw-r--r--   0        0        0     1344 2024-05-13 08:32:20.007123 grasp_planning-0.5.2/grasp_planning/cost/__pycache__/squared_acc_cost.cpython-38.pyc
+-rw-r--r--   0        0        0       65 2024-05-07 16:34:01.834623 grasp_planning-0.5.2/grasp_planning/cost/costs.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:00:02.772313 grasp_planning-0.5.2/grasp_planning/cost/dist_to_home.py
+-rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.2/grasp_planning/cost/squared_acc_cost.py
+-rw-r--r--   0        0        0     5881 2024-05-14 14:48:45.786607 grasp_planning-0.5.2/grasp_planning/solver/__pycache__/gomp_planner.cpython-38.pyc
+-rw-r--r--   0        0        0     2207 2024-05-14 14:05:14.682867 grasp_planning-0.5.2/grasp_planning/solver/__pycache__/robot_model.cpython-38.pyc
+-rw-r--r--   0        0        0     7594 2024-05-14 14:48:28.822517 grasp_planning-0.5.2/grasp_planning/solver/gomp_planner.py
+-rw-r--r--   0        0        0     1915 2024-05-14 14:04:42.954341 grasp_planning-0.5.2/grasp_planning/solver/robot_model.py
+-rw-r--r--   0        0        0      450 2024-05-14 14:55:59.628741 grasp_planning-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 grasp_planning-0.5.2/PKG-INFO
```

### Comparing `grasp_planning-0.5.1/README.md` & `grasp_planning-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/collision_constraint.cpython-38.pyc` & `grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/collision_constraint.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/constraint_template.cpython-38.pyc` & `grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/constraint_template.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/grasp_pos_constraint.cpython-38.pyc` & `grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/grasp_pos_constraint.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/grasp_rot_constraint.cpython-38.pyc` & `grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/grasp_rot_constraint.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/manipulation_constraint.cpython-38.pyc` & `grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/manipulation_constraint.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.1/grasp_planning/constraints/collision_constraint.py` & `grasp_planning-0.5.2/grasp_planning/constraints/collision_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.1/grasp_planning/constraints/grasp_pos_constraint.py` & `grasp_planning-0.5.2/grasp_planning/constraints/grasp_pos_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.1/grasp_planning/constraints/grasp_rot_constraint.py` & `grasp_planning-0.5.2/grasp_planning/constraints/grasp_rot_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.1/grasp_planning/constraints/manipulation_constraint.py` & `grasp_planning-0.5.2/grasp_planning/constraints/manipulation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.1/grasp_planning/cost/__pycache__/squared_acc_cost.cpython-38.pyc` & `grasp_planning-0.5.2/grasp_planning/cost/__pycache__/squared_acc_cost.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.1/grasp_planning/cost/squared_acc_cost.py` & `grasp_planning-0.5.2/grasp_planning/cost/squared_acc_cost.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.1/grasp_planning/solver/__pycache__/gomp_planner.cpython-38.pyc` & `grasp_planning-0.5.2/grasp_planning/solver/__pycache__/gomp_planner.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue May 14 13:19:53 2024 UTC, .py size: 7650 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 f964 4366 e21d 0000  U........dCf....
+00000000: 550d 0d0a 0000 0000 bc79 4366 aa1d 0000  U........yCf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c04 5a05 6400 6402 6c06 6d07 5a08  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c0b 6d0c 5a0c 0100 6400 6405 6c0d  d.l.m.Z...d.d.l.
 00000070: 5400 4700 6406 6407 8400 6407 8302 5a0e  T.G.d.d...d...Z.
@@ -71,304 +71,298 @@
 00000460: 7665 722f 676f 6d70 5f70 6c61 6e6e 6572  ver/gomp_planner
 00000470: 2e70 79da 085f 5f69 6e69 745f 5f0a 0000  .py..__init__...
 00000480: 0073 2600 0000 0002 0601 0601 1003 0e01  .s&.............
 00000490: 0a01 0601 0801 0601 0603 1601 0602 0601  ................
 000004a0: 0c01 0602 1201 1201 0601 0a01 7a0d 474f  ............z.GO
 000004b0: 4d50 2e5f 5f69 6e69 745f 5f54 2902 7218  MP.__init__T).r.
 000004c0: 0000 0072 0900 0000 6303 0000 0000 0000  ...r....c.......
-000004d0: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
-000004e0: 0073 9600 0000 7400 6a01 6401 7402 6402  .s....t.j.d.t.d.
-000004f0: 8d02 7c00 5f03 7c02 7244 7404 6a05 6403  ..|._.|.rDt.j.d.
-00000500: 6404 6405 7c01 6703 6406 6407 8d03 a006  d.d.|.g.d.d.....
-00000510: a100 7d03 7400 a007 7400 a008 7c01 a101  ..}.t...t...|...
-00000520: 6408 a102 7c00 5f09 6e2a 7404 6a05 6403  d...|._.n*t.j.d.
-00000530: 7400 6a0a 6405 7c01 6703 6409 6407 8d03  t.j.d.|.g.d.d...
-00000540: a006 a100 7d03 7400 a007 7c01 6408 a102  ....}.t...|.d...
-00000550: 7c00 5f09 7c03 7c00 6a03 640a 640b 8502  |._.|.|.j.d.d...
-00000560: 640a 640b 8502 6602 3c00 7c00 6a0b 7c00  d.d...f.<.|.j.|.
-00000570: 6a03 1000 7c00 5f0c 640a 5300 290c 7a48  j...|._.d.S.).zH
-00000580: 0a20 2020 2020 2020 204f 626a 6563 7420  .        Object 
-00000590: 6861 7320 746f 2068 6176 6520 7a2d 6178  has to have z-ax
-000005a0: 6973 2061 6c69 676e 6564 2077 6974 6820  is aligned with 
-000005b0: 7468 6520 776f 726c 6420 6672 616d 650a  the world frame.
-000005c0: 2020 2020 2020 2020 7207 0000 0072 0a00          r....r..
-000005d0: 0000 da03 7879 7ae9 b400 0000 7201 0000  ....xyz.....r...
-000005e0: 0054 2901 da07 6465 6772 6565 73e9 0200  .T)...degrees...
-000005f0: 0000 464e e903 0000 0029 0d72 1000 0000  ..FN.....).r....
-00000600: 7211 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00000610: 0152 5a0a 6672 6f6d 5f65 756c 6572 5a09  .RZ.from_eulerZ.
-00000620: 6173 5f6d 6174 7269 78da 0572 6f75 6e64  as_matrix..round
-00000630: 5a07 6465 6732 7261 6472 1800 0000 da02  Z.deg2radr......
-00000640: 7069 720f 0000 0072 0e00 0000 2904 7224  pir....r....).r$
-00000650: 0000 0072 1800 0000 722a 0000 005a 0b52  ...r....r*...Z.R
-00000660: 5f4f 626a 5f47 7261 7370 7225 0000 0072  _Obj_Graspr%...r
-00000670: 2500 0000 7226 0000 00da 1075 7064 6174  %...r&.....updat
-00000680: 655f 6772 6173 705f 444f 4627 0000 0073  e_grasp_DOF'...s
-00000690: 1000 0000 0004 1001 0401 1a01 1602 1c01  ................
-000006a0: 0e01 1601 7a15 474f 4d50 2e75 7064 6174  ....z.GOMP.updat
-000006b0: 655f 6772 6173 705f 444f 4629 0272 0f00  e_grasp_DOF).r..
-000006c0: 0000 7209 0000 0063 0200 0000 0000 0000  ..r....c........
-000006d0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-000006e0: 730a 0000 007c 017c 005f 0064 0153 0029  s....|.|._.d.S.)
-000006f0: 027a 2f0a 2020 2020 2020 2020 5570 6461  .z/.        Upda
-00000700: 7465 206f 626a 6563 7420 616e 6420 6772  te object and gr
-00000710: 6173 7020 706f 7365 730a 2020 2020 2020  asp poses.      
-00000720: 2020 4e29 0172 0f00 0000 2902 7224 0000    N).r....).r$..
-00000730: 0072 0f00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
-00000740: 7226 0000 00da 1275 7064 6174 655f 6f62  r&.....update_ob
-00000750: 6a65 6374 5f70 6f73 6535 0000 0073 0200  ject_pose5...s..
-00000760: 0000 0004 7a17 474f 4d50 2e75 7064 6174  ....z.GOMP.updat
-00000770: 655f 6f62 6a65 6374 5f70 6f73 6563 0100  e_object_posec..
-00000780: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-00000790: 0000 4300 0000 7354 0000 0074 006a 01a0  ..C...sT...t.j..
-000007a0: 027c 006a 0364 0164 0285 0264 0164 0285  .|.j.d.d...d.d..
-000007b0: 0266 0219 00a1 01a0 0464 03a1 017d 0174  .f.......d...}.t
-000007c0: 05a0 067c 006a 0364 0164 0285 0264 0266  ...|.j.d.d...d.f
-000007d0: 0219 0064 0164 0185 0264 0166 0219 007c  ...d.d...d.f...|
-000007e0: 0166 02a1 017c 005f 077c 006a 0753 0029  .f...|._.|.j.S.)
-000007f0: 047a 360a 2020 2020 2020 2020 436f 6e76  .z6.        Conv
-00000800: 6572 7420 545f 575f 4772 6173 7020 696e  ert T_W_Grasp in
-00000810: 746f 205b 782c 792c 7a2c 722c 702c 795d  to [x,y,z,r,p,y]
-00000820: 0a20 2020 2020 2020 204e 722c 0000 0072  .        Nr,...r
-00000830: 2800 0000 2908 da02 7363 7202 0000 005a  (...)...scr....Z
-00000840: 0b66 726f 6d5f 6d61 7472 6978 720e 0000  .from_matrixr...
-00000850: 005a 0861 735f 6575 6c65 7272 1000 0000  .Z.as_eulerr....
-00000860: 5a06 7673 7461 636b 5a0d 545f 575f 4772  Z.vstackZ.T_W_Gr
-00000870: 6173 705f 7270 7929 0272 2400 0000 5a0d  asp_rpy).r$...Z.
-00000880: 525f 575f 4772 6173 705f 7270 7972 2500  R_W_Grasp_rpyr%.
-00000890: 0000 7225 0000 0072 2600 0000 da0a 5f67  ..r%...r&....._g
-000008a0: 7261 7370 3272 7079 3b00 0000 7306 0000  rasp2rpy;...s...
-000008b0: 0000 0424 012a 017a 0f47 4f4d 502e 5f67  ...$.*.z.GOMP._g
-000008c0: 7261 7370 3272 7079 6302 0000 0000 0000  rasp2rpyc.......
-000008d0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-000008e0: 0073 1400 0000 7400 a001 7c01 7c00 6a02  .s....t...|.|.j.
-000008f0: a102 7c00 5f03 6400 5300 a901 4e29 0472  ..|._.d.S...N).r
-00000900: 1000 0000 5a04 7469 6c65 7217 0000 0072  ....Z.tiler....r
-00000910: 1a00 0000 2902 7224 0000 00da 0171 7225  ....).r$.....qr%
-00000920: 0000 0072 2500 0000 7226 0000 00da 0e73  ...r%...r&.....s
-00000930: 6574 5f69 6e69 745f 6775 6573 7344 0000  et_init_guessD..
-00000940: 0073 0200 0000 0001 7a13 474f 4d50 2e73  .s......z.GOMP.s
-00000950: 6574 5f69 6e69 745f 6775 6573 7363 0300  et_init_guessc..
-00000960: 0000 0000 0000 0000 0000 0500 0000 0500  ................
-00000970: 0000 4300 0000 7302 0100 007c 006a 0064  ..C...s....|.j.d
-00000980: 006b 0873 147c 006a 0164 006b 0872 ca74  .k.s.|.j.d.k.r.t
-00000990: 02a0 037c 006a 047c 006a 0566 0264 01a1  ...|.j.|.j.f.d..
-000009a0: 027c 005f 0074 02a0 037c 006a 047c 006a  .|._.t...|.j.|.j
-000009b0: 0566 0264 02a1 027c 005f 017c 006a 06a0  .f.d...|._.|.j..
-000009c0: 07a1 007d 0374 087c 006a 0583 0144 005d  ...}.t.|.j...D.]
-000009d0: 747d 047c 0364 0064 0085 0264 0366 0219  t}.|.d.d...d.f..
-000009e0: 007c 006a 0064 007c 006a 0985 027c 0466  .|.j.d.|.j...|.f
-000009f0: 023c 007c 0364 0064 0085 0264 0466 0219  .<.|.d.d...d.f..
-00000a00: 007c 006a 0164 007c 006a 0985 027c 0466  .|.j.d.|.j...|.f
-00000a10: 023c 0064 0574 026a 0a14 007c 006a 0064  .<.d.t.j...|.j.d
-00000a20: 0664 0085 027c 0466 023c 0064 0774 026a  .d...|.f.<.d.t.j
-00000a30: 0a14 007c 006a 0164 0664 0085 027c 0466  ...|.j.d.d...|.f
-00000a40: 023c 0071 547c 017c 006a 0064 0064 0085  .<.qT|.|.j.d.d..
-00000a50: 0264 0366 023c 007c 017c 006a 0164 0064  .d.f.<.|.|.j.d.d
-00000a60: 0085 0264 0366 023c 007c 0264 006b 0372  ...d.f.<.|.d.k.r
-00000a70: fe74 0b64 0883 0101 0064 0053 0029 094e  .t.d.....d.S.).N
-00000a80: 6700 0000 0000 0059 c067 0000 0000 0000  g......Y.g......
-00000a90: 5940 7201 0000 00e9 0100 0000 e9fe ffff  Y@r.............
-00000aa0: ffe9 fdff ffff 722b 0000 007a 2c46 696e  ......r+...z,Fin
-00000ab0: 616c 2062 6f75 6e64 6172 7920 636f 6e64  al boundary cond
-00000ac0: 6974 696f 6e20 6973 206e 6f74 2069 6d70  ition is not imp
-00000ad0: 6c65 6d65 6e74 6564 2e29 0c72 1b00 0000  lemented.).r....
-00000ae0: 721c 0000 0072 1000 0000 5a04 6675 6c6c  r....r....Z.full
-00000af0: 7216 0000 0072 1700 0000 7214 0000 005a  r....r....r....Z
-00000b00: 1467 6574 5f6a 6f69 6e74 5f70 6f73 5f6c  .get_joint_pos_l
-00000b10: 696d 6974 73da 0572 616e 6765 7215 0000  imits..ranger...
-00000b20: 0072 2f00 0000 da05 7072 696e 7429 0572  .r/.....print).r
-00000b30: 2400 0000 da07 715f 7374 6172 745a 0571  $.....q_startZ.q
-00000b40: 5f65 6e64 5a0c 6a6f 696e 745f 6c69 6d69  _endZ.joint_limi
-00000b50: 7473 da01 7472 2500 0000 7225 0000 0072  ts..tr%...r%...r
-00000b60: 2600 0000 da17 7365 745f 626f 756e 6461  &.....set_bounda
-00000b70: 7279 5f63 6f6e 6469 7469 6f6e 7347 0000  ry_conditionsG..
-00000b80: 0073 1a00 0000 0001 1402 1601 1603 0a01  .s..............
-00000b90: 0e01 2001 2001 1801 1a04 1201 1202 0801  .. . ...........
-00000ba0: 7a1c 474f 4d50 2e73 6574 5f62 6f75 6e64  z.GOMP.set_bound
-00000bb0: 6172 795f 636f 6e64 6974 696f 6e73 4663  ary_conditionsFc
-00000bc0: 0200 0000 0000 0000 0000 0000 0c00 0000  ................
-00000bd0: 0900 0000 4300 0000 7324 0100 007c 006a  ....C...s$...|.j
-00000be0: 00a0 0164 01a1 017d 0274 027c 006a 037c  ...d...}.t.|.j.|
-00000bf0: 006a 0464 0264 038d 037d 037c 03a0 057c  .j.d.d...}.|...|
-00000c00: 02a1 017d 0474 06a0 07a1 0074 06a0 07a1  ...}.t.....t....
-00000c10: 0074 06a0 07a1 0003 0002 007d 057c 005f  .t.........}.|._
-00000c20: 087c 005f 097c 006a 0a44 005d 3e7d 067c  .|._.|.j.D.]>}.|
-00000c30: 06a0 0ba1 005c 037d 077d 087d 0974 06a0  .....\.}.}.}.t..
-00000c40: 077c 057c 07a1 027d 0574 06a0 077c 006a  .|.|...}.t...|.j
-00000c50: 087c 08a1 027c 005f 0874 06a0 077c 006a  .|...|._.t...|.j
-00000c60: 097c 09a1 027c 005f 0971 4e7c 006a 0c72  .|...|._.qN|.j.r
-00000c70: a27c 006a 0da0 0e7c 006a 0fa1 0101 0074  .|.j...|.j.....t
-00000c80: 06a0 077c 006a 0d64 0419 00a1 017c 005f  ...|.j.d.....|._
-00000c90: 1074 1164 0574 127c 006a 0d83 0183 0244  .t.d.t.|.j.....D
-00000ca0: 005d 1a7d 0a74 06a0 077c 006a 107c 006a  .].}.t...|.j.|.j
-00000cb0: 0d7c 0a19 00a1 027c 005f 1071 c469 007d  .|.....|._.q.i.}
-00000cc0: 0b64 067c 0b64 073c 007c 0190 0173 0264  .d.|.d.<.|...s.d
-00000cd0: 047c 0b64 083c 0064 047c 0b64 093c 0074  .|.d.<.d.|.d.<.t
-00000ce0: 06a0 1364 0a64 0b7c 027c 047c 057c 006a  ...d.d.|.|.|.|.j
-00000cf0: 1064 0c9c 047c 0ba1 047c 005f 1464 0053  .d...|...|._.d.S
-00000d00: 0029 0d4e a902 e9ff ffff ff72 3700 0000  .).N.......r7...
-00000d10: 5429 015a 0b6d 616e 6970 5f66 7261 6d65  T).Z.manip_frame
-00000d20: 7201 0000 0072 3700 0000 67fc a9f1 d24d  r....r7...g....M
-00000d30: 6250 3f7a 1469 706f 7074 2e61 6363 6570  bP?z.ipopt.accep
-00000d40: 7461 626c 655f 746f 6c7a 1169 706f 7074  table_tolz.ipopt
-00000d50: 2e70 7269 6e74 5f6c 6576 656c 5a0a 7072  .print_levelZ.pr
-00000d60: 696e 745f 7469 6d65 da06 736f 6c76 6572  int_time..solver
-00000d70: 5a05 6970 6f70 7429 0472 0d00 0000 da01  Z.ipopt).r......
-00000d80: 66da 0167 da01 7029 1572 0d00 0000 da07  f..g..p).r......
-00000d90: 7265 7368 6170 6572 0400 0000 7217 0000  reshaper....r...
-00000da0: 0072 1600 0000 5a09 6576 616c 5f63 6f73  .r....Z.eval_cos
-00000db0: 7472 1900 0000 7221 0000 00da 0467 5f6c  tr....r!.....g_l
-00000dc0: 62da 0467 5f75 6272 1d00 0000 5a0e 6765  b..g_ubr....Z.ge
-00000dd0: 745f 636f 6e73 7472 6169 6e74 7220 0000  t_constraintr ..
-00000de0: 0072 2300 0000 da06 6170 7065 6e64 721f  .r#.....appendr.
-00000df0: 0000 0072 2200 0000 723a 0000 00da 036c  ...r"...r:.....l
-00000e00: 656e 5a06 6e6c 7073 6f6c 7241 0000 0029  enZ.nlpsolrA...)
-00000e10: 0c72 2400 0000 da07 7665 7262 6f73 655a  .r$.....verboseZ
-00000e20: 0c78 5f63 615f 666c 6174 7465 6e5a 0463  .x_ca_flattenZ.c
-00000e30: 6f73 745a 096f 626a 6563 7469 7665 7243  ostZ.objectiverC
-00000e40: 0000 005a 0667 5f74 6572 6dda 0267 7472  ...Z.g_term..gtr
-00000e50: 4600 0000 7247 0000 00da 0169 da07 6f70  F...rG.....i..op
-00000e60: 7469 6f6e 7372 2500 0000 7225 0000 0072  tionsr%...r%...r
-00000e70: 2600 0000 da0d 7365 7475 705f 7072 6f62  &.....setup_prob
-00000e80: 6c65 6d5f 0000 0073 2800 0000 0004 0c05  lem_...s(.......
-00000e90: 1201 0a02 2001 0a01 0e01 0c01 1001 1202  .... ...........
-00000ea0: 0601 0e03 1201 1401 1802 0401 0801 0601  ................
-00000eb0: 0801 0802 7a12 474f 4d50 2e73 6574 7570  ....z.GOMP.setup
-00000ec0: 5f70 726f 626c 656d 6301 0000 0000 0000  _problemc.......
-00000ed0: 0000 0000 0004 0000 0009 0000 0043 0000  .............C..
-00000ee0: 0073 6e00 0000 7c00 6a00 7c00 6a01 7c00  .sn...|.j.|.j.|.
-00000ef0: 6a02 7c00 6a03 7c00 6a04 6a05 6401 6402  j.|.j.|.j.j.d.d.
-00000f00: 6403 8d02 7c00 6a06 6a05 6401 6402 6403  d...|.j.j.d.d.d.
-00000f10: 8d02 7c00 6a07 6404 8d06 7d01 7c00 6a00  ..|.j.d...}.|.j.
-00000f20: a008 a100 6405 1900 7d02 7c00 6a00 a008  ....d...}.|.j...
-00000f30: a100 6406 1900 7d03 7409 a005 7c01 6407  ..d...}.t...|.d.
-00000f40: 1900 7c00 6a0a 7c00 6a0b 6602 a102 7c02  ..|.j.|.j.f...|.
-00000f50: 6602 5300 2908 4e72 3f00 0000 da01 4629  f.S.).Nr?.....F)
-00000f60: 01da 056f 7264 6572 2906 5a02 7830 5a03  ...order).Z.x0Z.
-00000f70: 6c62 675a 0375 6267 5a03 6c62 785a 0375  lbgZ.ubgZ.lbxZ.u
-00000f80: 6278 7244 0000 005a 0773 7563 6365 7373  bxrD...Z.success
-00000f90: 5a0d 7265 7475 726e 5f73 7461 7475 7372  Z.return_statusr
-00000fa0: 0d00 0000 290c 7241 0000 0072 1a00 0000  ....).rA...r....
-00000fb0: 7246 0000 0072 4700 0000 721b 0000 0072  rF...rG...r....r
-00000fc0: 4500 0000 721c 0000 00da 1070 6172 616d  E...r......param
-00000fd0: 735f 6f70 7469 6d5f 6e75 6d5a 0573 7461  s_optim_numZ.sta
-00000fe0: 7473 7210 0000 0072 1500 0000 7217 0000  tsr....r....r...
-00000ff0: 0029 0472 2400 0000 da06 7265 7375 6c74  .).r$.....result
-00001000: 5a0c 7375 6363 6573 735f 666c 6167 5a0b  Z.success_flagZ.
-00001010: 7375 6363 6573 735f 6d73 6772 2500 0000  success_msgr%...
-00001020: 7225 0000 0072 2600 0000 da05 736f 6c76  r%...r&.....solv
-00001030: 6584 0000 0073 1400 0000 0001 0801 0401  e....s..........
-00001040: 0401 0e01 0e01 04fb 0607 0e01 0e01 7a0a  ..............z.
-00001050: 474f 4d50 2e73 6f6c 7665 e700 0000 0000  GOMP.solve......
-00001060: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00001070: 0300 0000 0800 0000 4300 0000 7322 0000  ........C...s"..
-00001080: 007c 006a 00a0 0174 027c 006a 037c 006a  .|.j...t.|.j.|.j
-00001090: 047c 017c 006a 057c 0283 05a1 0101 0064  .|.|.j.|.......d
-000010a0: 0053 0072 3400 0000 2906 721d 0000 0072  .S.r4...).r....r
-000010b0: 4800 0000 5a12 4772 6173 7050 6f73 436f  H...Z.GraspPosCo
-000010c0: 6e73 7472 6169 6e74 7214 0000 0072 0d00  nstraintr....r..
-000010d0: 0000 721e 0000 00a9 0372 2400 0000 da0b  ..r......r$.....
-000010e0: 7761 7970 6f69 6e74 5f49 44da 0974 6f6c  waypoint_ID..tol
-000010f0: 6572 616e 6365 7225 0000 0072 2500 0000  erancer%...r%...
-00001100: 7226 0000 00da 195f 6164 645f 6772 6173  r&....._add_gras
-00001110: 705f 706f 735f 636f 6e73 7472 6169 6e74  p_pos_constraint
-00001120: 9000 0000 730c 0000 0000 010c 0104 0102  ....s...........
-00001130: 0104 0102 fc7a 1e47 4f4d 502e 5f61 6464  .....z.GOMP._add
-00001140: 5f67 7261 7370 5f70 6f73 5f63 6f6e 7374  _grasp_pos_const
-00001150: 7261 696e 74e7 9a99 9999 9999 b93f 6303  raint........?c.
-00001160: 0000 0000 0000 0000 0000 0003 0000 0009  ................
-00001170: 0000 0043 0000 0073 2600 0000 7c00 6a00  ...C...s&...|.j.
-00001180: a001 7402 7c00 6a03 7c00 6a04 7c01 7c00  ..t.|.j.|.j.|.|.
-00001190: 6a05 7c00 6a06 7c02 8306 a101 0100 6400  j.|.j.|.......d.
-000011a0: 5300 7234 0000 0029 0772 1d00 0000 7248  S.r4...).r....rH
-000011b0: 0000 005a 1247 7261 7370 526f 7443 6f6e  ...Z.GraspRotCon
-000011c0: 7374 7261 696e 7472 1400 0000 720d 0000  straintr....r...
-000011d0: 0072 1e00 0000 7218 0000 0072 5500 0000  .r....r....rU...
-000011e0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-000011f0: 195f 6164 645f 6772 6173 705f 726f 745f  ._add_grasp_rot_
-00001200: 636f 6e73 7472 6169 6e74 9700 0000 730e  constraint....s.
-00001210: 0000 0000 010c 0104 0102 0104 0104 0102  ................
-00001220: fb7a 1e47 4f4d 502e 5f61 6464 5f67 7261  .z.GOMP._add_gra
-00001230: 7370 5f72 6f74 5f63 6f6e 7374 7261 696e  sp_rot_constrain
-00001240: 7463 0300 0000 0000 0000 0000 0000 0300  tc..............
-00001250: 0000 0400 0000 4300 0000 732a 0000 007c  ......C...s*...|
-00001260: 00a0 007c 017c 02a1 0201 007c 00a0 017c  ...|.|.....|...|
-00001270: 017c 02a1 0201 007c 006a 02a0 037c 006a  .|.....|.j...|.j
-00001280: 04a1 0101 0064 0053 0072 3400 0000 2905  .....d.S.r4...).
-00001290: 7258 0000 0072 5a00 0000 7223 0000 0072  rX...rZ...r#...r
-000012a0: 4800 0000 721e 0000 0072 5500 0000 7225  H...r....rU...r%
-000012b0: 0000 0072 2500 0000 7226 0000 00da 1461  ...r%...r&.....a
-000012c0: 6464 5f67 7261 7370 5f63 6f6e 7374 7261  dd_grasp_constra
-000012d0: 696e 749f 0000 0073 0600 0000 0001 0c01  int....s........
-000012e0: 0c01 7a19 474f 4d50 2e61 6464 5f67 7261  ..z.GOMP.add_gra
-000012f0: 7370 5f63 6f6e 7374 7261 696e 74e7 0000  sp_constraint...
-00001300: 0000 0000 e03f e79a 9999 9999 99c9 3fe7  .....?........?.
-00001310: 7b14 ae47 e17a 843f 6306 0000 0000 0000  {..G.z.?c.......
-00001320: 0000 0000 0006 0000 000c 0000 0043 0000  .............C..
-00001330: 0073 3000 0000 6401 7c00 5f00 7c00 6a01  .s0...d.|._.|.j.
-00001340: a002 7403 7c00 6a04 7c00 6a05 7c01 7c00  ..t.|.j.|.j.|.|.
-00001350: 6a06 7c02 7c03 7c04 7c05 6402 8d08 a101  j.|.|.|.|.d.....
-00001360: 0100 6400 5300 2903 4e54 2908 5a05 726f  ..d.S.).NT).Z.ro
-00001370: 626f 745a 0471 5f63 6172 5600 0000 721f  botZ.q_carV...r.
-00001380: 0000 005a 096c 696e 6b5f 6e61 6d65 da06  ...Z.link_name..
-00001390: 725f 6c69 6e6b da06 725f 6f62 7374 7257  r_link..r_obstrW
-000013a0: 0000 0029 0772 2000 0000 721d 0000 0072  ...).r ...r....r
-000013b0: 4800 0000 5a13 436f 6c6c 6973 696f 6e43  H...Z.CollisionC
-000013c0: 6f6e 7374 7261 696e 7472 1400 0000 720d  onstraintr....r.
-000013d0: 0000 0072 1f00 0000 2906 7224 0000 0072  ...r....).r$...r
-000013e0: 5600 0000 da0a 6368 696c 645f 6c69 6e6b  V.....child_link
-000013f0: 725f 0000 0072 6000 0000 7257 0000 0072  r_...r`...rW...r
-00001400: 2500 0000 7225 0000 0072 2600 0000 da18  %...r%...r&.....
-00001410: 6164 645f 636f 6c6c 6973 696f 6e5f 636f  add_collision_co
-00001420: 6e73 7472 6169 6e74 a400 0000 7314 0000  nstraint....s...
-00001430: 0000 0106 010c 0104 0102 0104 0102 0102  ................
-00001440: 0102 0102 f97a 1d47 4f4d 502e 6164 645f  .....z.GOMP.add_
-00001450: 636f 6c6c 6973 696f 6e5f 636f 6e73 7472  collision_constr
-00001460: 6169 6e74 6303 0000 0000 0000 0000 0000  aintc...........
-00001470: 0003 0000 0004 0000 0043 0000 0073 3a00  .........C...s:.
-00001480: 0000 7c00 a000 7c01 a101 0100 7c00 6a01  ..|...|.....|.j.
-00001490: 7c00 6a02 6401 6402 8d02 0100 7c00 6a03  |.j.d.d.....|.j.
-000014a0: 7230 7404 a005 7c01 7c02 a102 7c00 5f06  r0t...|.|...|._.
-000014b0: 6e06 7c01 7c00 5f06 6400 5300 2903 4e46  n.|.|._.d.S.).NF
-000014c0: 2902 7218 0000 0072 2a00 0000 2907 7231  ).r....r*...).r1
-000014d0: 0000 0072 3000 0000 7218 0000 0072 2000  ...r0...r....r .
-000014e0: 0000 7219 0000 0072 2100 0000 7251 0000  ..r....r!...rQ..
-000014f0: 0029 0372 2400 0000 720f 0000 00da 0854  .).r$...r......T
-00001500: 5f57 5f4f 6273 7472 2500 0000 7225 0000  _W_Obstr%...r%..
-00001510: 0072 2600 0000 da19 7570 6461 7465 5f63  .r&.....update_c
-00001520: 6f6e 7374 7261 696e 7473 5f70 6172 616d  onstraints_param
-00001530: 73af 0000 0073 0a00 0000 0001 0a01 1002  s....s..........
-00001540: 0601 1002 7a1e 474f 4d50 2e75 7064 6174  ....z.GOMP.updat
-00001550: 655f 636f 6e73 7472 6169 6e74 735f 7061  e_constraints_pa
-00001560: 7261 6d73 2901 5429 014e 2901 4629 0172  rams).T).N).F).r
-00001570: 5400 0000 2901 7259 0000 0029 0172 5400  T...).rY...).rT.
-00001580: 0000 2903 725c 0000 0072 5d00 0000 725e  ..).r\...r]...r^
-00001590: 0000 0029 014e 2914 da08 5f5f 6e61 6d65  ...).N)...__name
-000015a0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-000015b0: 5f5f 7175 616c 6e61 6d65 5f5f 7210 0000  __qualname__r...
-000015c0: 0072 2f00 0000 7227 0000 0072 1200 0000  .r/...r'...r....
-000015d0: 7230 0000 00da 0561 7272 6179 7231 0000  r0.....arrayr1..
-000015e0: 0072 3300 0000 7236 0000 0072 3e00 0000  .r3...r6...r>...
-000015f0: 724e 0000 0072 5300 0000 7258 0000 0072  rN...rS...rX...r
-00001600: 5a00 0000 725b 0000 0072 6200 0000 7264  Z...r[...rb...rd
-00001610: 0000 0072 2500 0000 7225 0000 0072 2500  ...r%...r%...r%.
-00001620: 0000 7226 0000 0072 0600 0000 0900 0000  ..r&...r........
-00001630: 731a 0000 0008 011c 1d12 0e12 0608 0908  s...............
-00001640: 030a 180a 2508 0c0a 070a 080a 050a 0b72  ....%..........r
-00001650: 0600 0000 290f da05 6e75 6d70 7972 1000  ....)...numpyr..
-00001660: 0000 5a06 6361 7361 6469 7219 0000 005a  ..Z.casadir....Z
-00001670: 0e73 7061 7469 616c 5f63 6173 6164 6972  .spatial_casadir
-00001680: 3200 0000 5a17 7363 6970 792e 7370 6174  2...Z.scipy.spat
-00001690: 6961 6c2e 7472 616e 7366 6f72 6d72 0200  ial.transformr..
-000016a0: 0000 722d 0000 005a 2167 7261 7370 5f70  ..r-...Z!grasp_p
-000016b0: 6c61 6e6e 696e 672e 736f 6c76 6572 2e72  lanning.solver.r
-000016c0: 6f62 6f74 5f6d 6f64 656c 7203 0000 005a  obot_modelr....Z
-000016d0: 1967 7261 7370 5f70 6c61 6e6e 696e 672e  .grasp_planning.
-000016e0: 636f 7374 2e63 6f73 7473 7204 0000 005a  cost.costsr....Z
-000016f0: 2667 7261 7370 5f70 6c61 6e6e 696e 672e  &grasp_planning.
-00001700: 636f 6e73 7472 6169 6e74 732e 636f 6e73  constraints.cons
-00001710: 7472 6169 6e74 7372 0600 0000 7225 0000  traintsr....r%..
-00001720: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00001730: da08 3c6d 6f64 756c 653e 0100 0000 730e  ..<module>....s.
-00001740: 0000 0008 0108 0108 010c 010c 010c 0108  ................
-00001750: 02                                       .
+000004d0: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
+000004e0: 0073 9000 0000 7400 6a01 6401 7402 6402  .s....t.j.d.t.d.
+000004f0: 8d02 7c00 5f03 7c02 7240 7400 a004 7c01  ..|._.|.r@t...|.
+00000500: a101 7c00 5f05 7406 6a07 6403 6404 6405  ..|._.t.j.d.d.d.
+00000510: 7c00 6a05 6703 6406 6407 8d03 a008 a100  |.j.g.d.d.......
+00000520: 7c00 5f09 6e26 7c01 7c00 5f05 7406 6a07  |._.n&|.|._.t.j.
+00000530: 6403 7400 6a0a 6405 7c00 6a05 6703 6408  d.t.j.d.|.j.g.d.
+00000540: 6407 8d03 a008 a100 7c00 5f09 7c00 6a09  d.......|._.|.j.
+00000550: 7c00 6a03 6409 640a 8502 6409 640a 8502  |.j.d.d...d.d...
+00000560: 6602 3c00 7c00 6a0b 7c00 6a03 1000 7c00  f.<.|.j.|.j...|.
+00000570: 5f0c 6409 5300 290b 7a48 0a20 2020 2020  _.d.S.).zH.     
+00000580: 2020 204f 626a 6563 7420 6861 7320 746f     Object has to
+00000590: 2068 6176 6520 7a2d 6178 6973 2061 6c69   have z-axis ali
+000005a0: 676e 6564 2077 6974 6820 7468 6520 776f  gned with the wo
+000005b0: 726c 6420 6672 616d 650a 2020 2020 2020  rld frame.      
+000005c0: 2020 7207 0000 0072 0a00 0000 da03 7879    r....r......xy
+000005d0: 7ae9 b400 0000 7201 0000 0054 2901 da07  z.....r....T)...
+000005e0: 6465 6772 6565 7346 4ee9 0300 0000 290d  degreesFN.....).
+000005f0: 7210 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00000600: 1300 0000 5a07 6465 6732 7261 6472 1800  ....Z.deg2radr..
+00000610: 0000 da01 525a 0a66 726f 6d5f 6575 6c65  ....RZ.from_eule
+00000620: 725a 0961 735f 6d61 7472 6978 5a0b 525f  rZ.as_matrixZ.R_
+00000630: 4f62 6a5f 4772 6173 70da 0270 6972 0f00  Obj_Grasp..pir..
+00000640: 0000 720e 0000 0029 0372 2400 0000 7218  ..r....).r$...r.
+00000650: 0000 0072 2a00 0000 7225 0000 0072 2500  ...r*...r%...r%.
+00000660: 0000 7226 0000 00da 1075 7064 6174 655f  ..r&.....update_
+00000670: 6772 6173 705f 444f 4627 0000 0073 1000  grasp_DOF'...s..
+00000680: 0000 0004 1001 0401 0c01 2002 0601 2001  .......... ... .
+00000690: 1801 7a15 474f 4d50 2e75 7064 6174 655f  ..z.GOMP.update_
+000006a0: 6772 6173 705f 444f 4629 0272 0f00 0000  grasp_DOF).r....
+000006b0: 7209 0000 0063 0200 0000 0000 0000 0000  r....c..........
+000006c0: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
+000006d0: 0000 007c 017c 005f 0064 0153 0029 027a  ...|.|._.d.S.).z
+000006e0: 2f0a 2020 2020 2020 2020 5570 6461 7465  /.        Update
+000006f0: 206f 626a 6563 7420 616e 6420 6772 6173   object and gras
+00000700: 7020 706f 7365 730a 2020 2020 2020 2020  p poses.        
+00000710: 4e29 0172 0f00 0000 2902 7224 0000 0072  N).r....).r$...r
+00000720: 0f00 0000 7225 0000 0072 2500 0000 7226  ....r%...r%...r&
+00000730: 0000 00da 1275 7064 6174 655f 6f62 6a65  .....update_obje
+00000740: 6374 5f70 6f73 6538 0000 0073 0200 0000  ct_pose8...s....
+00000750: 0004 7a17 474f 4d50 2e75 7064 6174 655f  ..z.GOMP.update_
+00000760: 6f62 6a65 6374 5f70 6f73 6563 0100 0000  object_posec....
+00000770: 0000 0000 0000 0000 0200 0000 0600 0000  ................
+00000780: 4300 0000 7354 0000 0074 006a 01a0 027c  C...sT...t.j...|
+00000790: 006a 0364 0164 0285 0264 0164 0285 0266  .j.d.d...d.d...f
+000007a0: 0219 00a1 01a0 0464 03a1 017d 0174 05a0  .......d...}.t..
+000007b0: 067c 006a 0364 0164 0285 0264 0266 0219  .|.j.d.d...d.f..
+000007c0: 0064 0164 0185 0264 0166 0219 007c 0166  .d.d...d.f...|.f
+000007d0: 02a1 017c 005f 077c 006a 0753 0029 047a  ...|._.|.j.S.).z
+000007e0: 360a 2020 2020 2020 2020 436f 6e76 6572  6.        Conver
+000007f0: 7420 545f 575f 4772 6173 7020 696e 746f  t T_W_Grasp into
+00000800: 205b 782c 792c 7a2c 722c 702c 795d 0a20   [x,y,z,r,p,y]. 
+00000810: 2020 2020 2020 204e 722b 0000 0072 2800         Nr+...r(.
+00000820: 0000 2908 da02 7363 7202 0000 005a 0b66  ..)...scr....Z.f
+00000830: 726f 6d5f 6d61 7472 6978 720e 0000 005a  rom_matrixr....Z
+00000840: 0861 735f 6575 6c65 7272 1000 0000 5a06  .as_eulerr....Z.
+00000850: 7673 7461 636b 5a0d 545f 575f 4772 6173  vstackZ.T_W_Gras
+00000860: 705f 7270 7929 0272 2400 0000 5a0d 525f  p_rpy).r$...Z.R_
+00000870: 575f 4772 6173 705f 7270 7972 2500 0000  W_Grasp_rpyr%...
+00000880: 7225 0000 0072 2600 0000 da0a 5f67 7261  r%...r&....._gra
+00000890: 7370 3272 7079 3e00 0000 7306 0000 0000  sp2rpy>...s.....
+000008a0: 0424 012a 017a 0f47 4f4d 502e 5f67 7261  .$.*.z.GOMP._gra
+000008b0: 7370 3272 7079 6302 0000 0000 0000 0000  sp2rpyc.........
+000008c0: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+000008d0: 1400 0000 7400 a001 7c01 7c00 6a02 a102  ....t...|.|.j...
+000008e0: 7c00 5f03 6400 5300 a901 4e29 0472 1000  |._.d.S...N).r..
+000008f0: 0000 5a04 7469 6c65 7217 0000 0072 1a00  ..Z.tiler....r..
+00000900: 0000 2902 7224 0000 00da 0171 7225 0000  ..).r$.....qr%..
+00000910: 0072 2500 0000 7226 0000 00da 0e73 6574  .r%...r&.....set
+00000920: 5f69 6e69 745f 6775 6573 7347 0000 0073  _init_guessG...s
+00000930: 0200 0000 0001 7a13 474f 4d50 2e73 6574  ......z.GOMP.set
+00000940: 5f69 6e69 745f 6775 6573 7363 0300 0000  _init_guessc....
+00000950: 0000 0000 0000 0000 0500 0000 0500 0000  ................
+00000960: 4300 0000 73d2 0000 007c 006a 0064 006b  C...s....|.j.d.k
+00000970: 0873 147c 006a 0164 006b 0872 9a74 02a0  .s.|.j.d.k.r.t..
+00000980: 037c 006a 047c 006a 0566 0264 01a1 027c  .|.j.|.j.f.d...|
+00000990: 005f 0074 02a0 037c 006a 047c 006a 0566  ._.t...|.j.|.j.f
+000009a0: 0264 02a1 027c 005f 017c 006a 06a0 07a1  .d...|._.|.j....
+000009b0: 007d 0374 087c 006a 0583 0144 005d 447d  .}.t.|.j...D.]D}
+000009c0: 047c 0364 0064 0085 0264 0366 0219 007c  .|.d.d...d.f...|
+000009d0: 006a 0064 007c 006a 0985 027c 0466 023c  .j.d.|.j...|.f.<
+000009e0: 007c 0364 0064 0085 0264 0466 0219 007c  .|.d.d...d.f...|
+000009f0: 006a 0164 007c 006a 0985 027c 0466 023c  .j.d.|.j...|.f.<
+00000a00: 0071 547c 017c 006a 0064 0064 0085 0264  .qT|.|.j.d.d...d
+00000a10: 0366 023c 007c 017c 006a 0164 0064 0085  .f.<.|.|.j.d.d..
+00000a20: 0264 0366 023c 007c 0264 006b 0372 ce74  .d.f.<.|.d.k.r.t
+00000a30: 0a64 0583 0101 0064 0053 0029 064e 6700  .d.....d.S.).Ng.
+00000a40: 0000 0000 0059 c067 0000 0000 0000 5940  .....Y.g......Y@
+00000a50: 7201 0000 00e9 0100 0000 7a2c 4669 6e61  r.........z,Fina
+00000a60: 6c20 626f 756e 6461 7279 2063 6f6e 6469  l boundary condi
+00000a70: 7469 6f6e 2069 7320 6e6f 7420 696d 706c  tion is not impl
+00000a80: 656d 656e 7465 642e 290b 721b 0000 0072  emented.).r....r
+00000a90: 1c00 0000 7210 0000 005a 0466 756c 6c72  ....r....Z.fullr
+00000aa0: 1600 0000 7217 0000 0072 1400 0000 5a14  ....r....r....Z.
+00000ab0: 6765 745f 6a6f 696e 745f 706f 735f 6c69  get_joint_pos_li
+00000ac0: 6d69 7473 da05 7261 6e67 6572 1500 0000  mits..ranger....
+00000ad0: da05 7072 696e 7429 0572 2400 0000 da07  ..print).r$.....
+00000ae0: 715f 7374 6172 745a 0571 5f65 6e64 5a0c  q_startZ.q_endZ.
+00000af0: 6a6f 696e 745f 6c69 6d69 7473 da01 7472  joint_limits..tr
+00000b00: 2500 0000 7225 0000 0072 2600 0000 da17  %...r%...r&.....
+00000b10: 7365 745f 626f 756e 6461 7279 5f63 6f6e  set_boundary_con
+00000b20: 6469 7469 6f6e 734a 0000 0073 1600 0000  ditionsJ...s....
+00000b30: 0001 1402 1601 1603 0a01 0e01 2001 2205  ............ .".
+00000b40: 1201 1202 0801 7a1c 474f 4d50 2e73 6574  ......z.GOMP.set
+00000b50: 5f62 6f75 6e64 6172 795f 636f 6e64 6974  _boundary_condit
+00000b60: 696f 6e73 4663 0200 0000 0000 0000 0000  ionsFc..........
+00000b70: 0000 0c00 0000 0900 0000 4300 0000 7324  ..........C...s$
+00000b80: 0100 007c 006a 00a0 0164 01a1 017d 0274  ...|.j...d...}.t
+00000b90: 027c 006a 037c 006a 0464 0264 038d 037d  .|.j.|.j.d.d...}
+00000ba0: 037c 03a0 057c 02a1 017d 0474 06a0 07a1  .|...|...}.t....
+00000bb0: 0074 06a0 07a1 0074 06a0 07a1 0003 0002  .t.....t........
+00000bc0: 007d 057c 005f 087c 005f 097c 006a 0a44  .}.|._.|._.|.j.D
+00000bd0: 005d 3e7d 067c 06a0 0ba1 005c 037d 077d  .]>}.|.....\.}.}
+00000be0: 087d 0974 06a0 077c 057c 07a1 027d 0574  .}.t...|.|...}.t
+00000bf0: 06a0 077c 006a 087c 08a1 027c 005f 0874  ...|.j.|...|._.t
+00000c00: 06a0 077c 006a 097c 09a1 027c 005f 0971  ...|.j.|...|._.q
+00000c10: 4e7c 006a 0c72 a27c 006a 0da0 0e7c 006a  N|.j.r.|.j...|.j
+00000c20: 0fa1 0101 0074 06a0 077c 006a 0d64 0419  .....t...|.j.d..
+00000c30: 00a1 017c 005f 1074 1164 0574 127c 006a  ...|._.t.d.t.|.j
+00000c40: 0d83 0183 0244 005d 1a7d 0a74 06a0 077c  .....D.].}.t...|
+00000c50: 006a 107c 006a 0d7c 0a19 00a1 027c 005f  .j.|.j.|.....|._
+00000c60: 1071 c469 007d 0b64 067c 0b64 073c 007c  .q.i.}.d.|.d.<.|
+00000c70: 0190 0173 0264 047c 0b64 083c 0064 047c  ...s.d.|.d.<.d.|
+00000c80: 0b64 093c 0074 06a0 1364 0a64 0b7c 027c  .d.<.t...d.d.|.|
+00000c90: 047c 057c 006a 1064 0c9c 047c 0ba1 047c  .|.|.j.d...|...|
+00000ca0: 005f 1464 0053 0029 0d4e a902 e9ff ffff  ._.d.S.).N......
+00000cb0: ff72 3500 0000 5429 015a 0b6d 616e 6970  .r5...T).Z.manip
+00000cc0: 5f66 7261 6d65 7201 0000 0072 3500 0000  _framer....r5...
+00000cd0: 67fc a9f1 d24d 6250 3f7a 1469 706f 7074  g....MbP?z.ipopt
+00000ce0: 2e61 6363 6570 7461 626c 655f 746f 6c7a  .acceptable_tolz
+00000cf0: 1169 706f 7074 2e70 7269 6e74 5f6c 6576  .ipopt.print_lev
+00000d00: 656c 5a0a 7072 696e 745f 7469 6d65 da06  elZ.print_time..
+00000d10: 736f 6c76 6572 5a05 6970 6f70 7429 0472  solverZ.ipopt).r
+00000d20: 0d00 0000 da01 66da 0167 da01 7029 1572  ......f..g..p).r
+00000d30: 0d00 0000 da07 7265 7368 6170 6572 0400  ......reshaper..
+00000d40: 0000 7217 0000 0072 1600 0000 5a09 6576  ..r....r....Z.ev
+00000d50: 616c 5f63 6f73 7472 1900 0000 7221 0000  al_costr....r!..
+00000d60: 00da 0467 5f6c 62da 0467 5f75 6272 1d00  ...g_lb..g_ubr..
+00000d70: 0000 5a0e 6765 745f 636f 6e73 7472 6169  ..Z.get_constrai
+00000d80: 6e74 7220 0000 0072 2300 0000 da06 6170  ntr ...r#.....ap
+00000d90: 7065 6e64 721f 0000 0072 2200 0000 7236  pendr....r"...r6
+00000da0: 0000 00da 036c 656e 5a06 6e6c 7073 6f6c  .....lenZ.nlpsol
+00000db0: 723d 0000 0029 0c72 2400 0000 da07 7665  r=...).r$.....ve
+00000dc0: 7262 6f73 655a 0c78 5f63 615f 666c 6174  rboseZ.x_ca_flat
+00000dd0: 7465 6e5a 0463 6f73 745a 096f 626a 6563  tenZ.costZ.objec
+00000de0: 7469 7665 723f 0000 005a 0667 5f74 6572  tiver?...Z.g_ter
+00000df0: 6dda 0267 7472 4200 0000 7243 0000 00da  m..gtrB...rC....
+00000e00: 0169 da07 6f70 7469 6f6e 7372 2500 0000  .i..optionsr%...
+00000e10: 7225 0000 0072 2600 0000 da0d 7365 7475  r%...r&.....setu
+00000e20: 705f 7072 6f62 6c65 6d61 0000 0073 2800  p_problema...s(.
+00000e30: 0000 0004 0c05 1201 0a02 2001 0a01 0e01  .......... .....
+00000e40: 0c01 1001 1202 0601 0e03 1201 1401 1802  ................
+00000e50: 0401 0801 0601 0801 0802 7a12 474f 4d50  ..........z.GOMP
+00000e60: 2e73 6574 7570 5f70 726f 626c 656d 6301  .setup_problemc.
+00000e70: 0000 0000 0000 0000 0000 0004 0000 0009  ................
+00000e80: 0000 0043 0000 0073 6c00 0000 7c00 6a00  ...C...sl...|.j.
+00000e90: 7c00 6a01 7c00 6a02 7c00 6a03 7c00 6a04  |.j.|.j.|.j.|.j.
+00000ea0: 6a05 6401 6402 6403 8d02 7c00 6a06 6a05  j.d.d.d...|.j.j.
+00000eb0: 6401 6402 6403 8d02 7c00 6a07 6404 8d06  d.d.d...|.j.d...
+00000ec0: 7d01 7c00 6a00 a008 a100 6405 1900 7d02  }.|.j.....d...}.
+00000ed0: 7c00 6a00 a008 a100 6406 1900 7d03 7c01  |.j.....d...}.|.
+00000ee0: 6407 1900 a005 7c00 6a09 7c00 6a0a 6602  d.....|.j.|.j.f.
+00000ef0: a101 7c02 6602 5300 2908 4e72 3b00 0000  ..|.f.S.).Nr;...
+00000f00: da01 4629 01da 056f 7264 6572 2906 5a02  ..F)...order).Z.
+00000f10: 7830 5a03 6c62 675a 0375 6267 5a03 6c62  x0Z.lbgZ.ubgZ.lb
+00000f20: 785a 0375 6278 7240 0000 005a 0773 7563  xZ.ubxr@...Z.suc
+00000f30: 6365 7373 5a0d 7265 7475 726e 5f73 7461  cessZ.return_sta
+00000f40: 7475 7372 0d00 0000 290b 723d 0000 0072  tusr....).r=...r
+00000f50: 1a00 0000 7242 0000 0072 4300 0000 721b  ....rB...rC...r.
+00000f60: 0000 0072 4100 0000 721c 0000 0072 0e00  ...rA...r....r..
+00000f70: 0000 5a05 7374 6174 7372 1500 0000 7217  ..Z.statsr....r.
+00000f80: 0000 0029 0472 2400 0000 da06 7265 7375  ...).r$.....resu
+00000f90: 6c74 5a0c 7375 6363 6573 735f 666c 6167  ltZ.success_flag
+00000fa0: 5a0b 7375 6363 6573 735f 6d73 6772 2500  Z.success_msgr%.
+00000fb0: 0000 7225 0000 0072 2600 0000 da05 736f  ..r%...r&.....so
+00000fc0: 6c76 6586 0000 0073 1400 0000 0001 0801  lve....s........
+00000fd0: 0401 0401 0e01 0e01 04fb 0607 0e01 0e01  ................
+00000fe0: 7a0a 474f 4d50 2e73 6f6c 7665 e700 0000  z.GOMP.solve....
+00000ff0: 0000 0000 0063 0300 0000 0000 0000 0000  .....c..........
+00001000: 0000 0300 0000 0800 0000 4300 0000 7322  ..........C...s"
+00001010: 0000 007c 006a 00a0 0174 027c 006a 037c  ...|.j...t.|.j.|
+00001020: 006a 047c 017c 006a 057c 0283 05a1 0101  .j.|.|.j.|......
+00001030: 0064 0053 0072 3200 0000 2906 721d 0000  .d.S.r2...).r...
+00001040: 0072 4400 0000 5a12 4772 6173 7050 6f73  .rD...Z.GraspPos
+00001050: 436f 6e73 7472 6169 6e74 7214 0000 0072  Constraintr....r
+00001060: 0d00 0000 721e 0000 00a9 0372 2400 0000  ....r......r$...
+00001070: da0b 7761 7970 6f69 6e74 5f49 44da 0974  ..waypoint_ID..t
+00001080: 6f6c 6572 616e 6365 7225 0000 0072 2500  olerancer%...r%.
+00001090: 0000 7226 0000 00da 195f 6164 645f 6772  ..r&....._add_gr
+000010a0: 6173 705f 706f 735f 636f 6e73 7472 6169  asp_pos_constrai
+000010b0: 6e74 9200 0000 730c 0000 0000 010c 0104  nt....s.........
+000010c0: 0102 0104 0102 fc7a 1e47 4f4d 502e 5f61  .......z.GOMP._a
+000010d0: 6464 5f67 7261 7370 5f70 6f73 5f63 6f6e  dd_grasp_pos_con
+000010e0: 7374 7261 696e 74e7 9a99 9999 9999 b93f  straint........?
+000010f0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00001100: 0009 0000 0043 0000 0073 2600 0000 7c00  .....C...s&...|.
+00001110: 6a00 a001 7402 7c00 6a03 7c00 6a04 7c01  j...t.|.j.|.j.|.
+00001120: 7c00 6a05 7c00 6a06 7c02 8306 a101 0100  |.j.|.j.|.......
+00001130: 6400 5300 7232 0000 0029 0772 1d00 0000  d.S.r2...).r....
+00001140: 7244 0000 005a 1247 7261 7370 526f 7443  rD...Z.GraspRotC
+00001150: 6f6e 7374 7261 696e 7472 1400 0000 720d  onstraintr....r.
+00001160: 0000 0072 1e00 0000 7218 0000 0072 5000  ...r....r....rP.
+00001170: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
+00001180: 00da 195f 6164 645f 6772 6173 705f 726f  ..._add_grasp_ro
+00001190: 745f 636f 6e73 7472 6169 6e74 9900 0000  t_constraint....
+000011a0: 730e 0000 0000 010c 0104 0102 0104 0104  s...............
+000011b0: 0102 fb7a 1e47 4f4d 502e 5f61 6464 5f67  ...z.GOMP._add_g
+000011c0: 7261 7370 5f72 6f74 5f63 6f6e 7374 7261  rasp_rot_constra
+000011d0: 696e 7463 0300 0000 0000 0000 0000 0000  intc............
+000011e0: 0300 0000 0400 0000 4300 0000 732a 0000  ........C...s*..
+000011f0: 007c 00a0 007c 017c 02a1 0201 007c 00a0  .|...|.|.....|..
+00001200: 017c 017c 02a1 0201 007c 006a 02a0 037c  .|.|.....|.j...|
+00001210: 006a 04a1 0101 0064 0053 0072 3200 0000  .j.....d.S.r2...
+00001220: 2905 7253 0000 0072 5500 0000 7223 0000  ).rS...rU...r#..
+00001230: 0072 4400 0000 721e 0000 0072 5000 0000  .rD...r....rP...
+00001240: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
+00001250: 1461 6464 5f67 7261 7370 5f63 6f6e 7374  .add_grasp_const
+00001260: 7261 696e 74a1 0000 0073 0600 0000 0001  raint....s......
+00001270: 0c01 0c01 7a19 474f 4d50 2e61 6464 5f67  ....z.GOMP.add_g
+00001280: 7261 7370 5f63 6f6e 7374 7261 696e 74e7  rasp_constraint.
+00001290: 0000 0000 0000 e03f e79a 9999 9999 99c9  .......?........
+000012a0: 3fe7 7b14 ae47 e17a 843f 6306 0000 0000  ?.{..G.z.?c.....
+000012b0: 0000 0000 0000 0006 0000 000c 0000 0043  ...............C
+000012c0: 0000 0073 3000 0000 6401 7c00 5f00 7c00  ...s0...d.|._.|.
+000012d0: 6a01 a002 7403 7c00 6a04 7c00 6a05 7c01  j...t.|.j.|.j.|.
+000012e0: 7c00 6a06 7c02 7c03 7c04 7c05 6402 8d08  |.j.|.|.|.|.d...
+000012f0: a101 0100 6400 5300 2903 4e54 2908 5a05  ....d.S.).NT).Z.
+00001300: 726f 626f 745a 0471 5f63 6172 5100 0000  robotZ.q_carQ...
+00001310: 721f 0000 005a 096c 696e 6b5f 6e61 6d65  r....Z.link_name
+00001320: da06 725f 6c69 6e6b da06 725f 6f62 7374  ..r_link..r_obst
+00001330: 7252 0000 0029 0772 2000 0000 721d 0000  rR...).r ...r...
+00001340: 0072 4400 0000 5a13 436f 6c6c 6973 696f  .rD...Z.Collisio
+00001350: 6e43 6f6e 7374 7261 696e 7472 1400 0000  nConstraintr....
+00001360: 720d 0000 0072 1f00 0000 2906 7224 0000  r....r....).r$..
+00001370: 0072 5100 0000 5a0a 6368 696c 645f 6c69  .rQ...Z.child_li
+00001380: 6e6b 725a 0000 0072 5b00 0000 7252 0000  nkrZ...r[...rR..
+00001390: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+000013a0: da18 6164 645f 636f 6c6c 6973 696f 6e5f  ..add_collision_
+000013b0: 636f 6e73 7472 6169 6e74 a600 0000 7314  constraint....s.
+000013c0: 0000 0000 0106 010c 0104 0102 0104 0102  ................
+000013d0: 0102 0102 0102 f97a 1d47 4f4d 502e 6164  .......z.GOMP.ad
+000013e0: 645f 636f 6c6c 6973 696f 6e5f 636f 6e73  d_collision_cons
+000013f0: 7472 6169 6e74 6303 0000 0000 0000 0000  traintc.........
+00001400: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+00001410: 3e00 0000 7c00 a000 7c01 a101 0100 7c00  >...|...|.....|.
+00001420: 6a01 7c00 6a02 6401 6402 8d02 0100 7c00  j.|.j.d.d.....|.
+00001430: 6a03 7232 7404 a005 7c00 6a06 7c02 a102  j.r2t...|.j.|...
+00001440: 7c00 5f07 6e08 7c00 6a06 7c00 5f07 6400  |._.n.|.j.|._.d.
+00001450: 5300 2903 4e46 2902 7218 0000 0072 2a00  S.).NF).r....r*.
+00001460: 0000 2908 722f 0000 0072 2e00 0000 7218  ..).r/...r....r.
+00001470: 0000 0072 2000 0000 7219 0000 0072 2100  ...r ...r....r!.
+00001480: 0000 720e 0000 005a 1070 6172 616d 735f  ..r....Z.params_
+00001490: 6f70 7469 6d5f 6e75 6d29 0372 2400 0000  optim_num).r$...
+000014a0: 720f 0000 00da 0854 5f57 5f4f 6273 7472  r......T_W_Obstr
+000014b0: 2500 0000 7225 0000 0072 2600 0000 da19  %...r%...r&.....
+000014c0: 7570 6461 7465 5f63 6f6e 7374 7261 696e  update_constrain
+000014d0: 7473 5f70 6172 616d 73b1 0000 0073 0a00  ts_params....s..
+000014e0: 0000 0001 0a01 1002 0601 1202 7a1e 474f  ............z.GO
+000014f0: 4d50 2e75 7064 6174 655f 636f 6e73 7472  MP.update_constr
+00001500: 6169 6e74 735f 7061 7261 6d73 2901 5429  aints_params).T)
+00001510: 014e 2901 4629 0172 4f00 0000 2901 7254  .N).F).rO...).rT
+00001520: 0000 0029 0172 4f00 0000 2903 7257 0000  ...).rO...).rW..
+00001530: 0072 5800 0000 7259 0000 0029 014e 2914  .rX...rY...).N).
+00001540: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00001550: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00001560: 6d65 5f5f 7210 0000 0072 2d00 0000 7227  me__r....r-...r'
+00001570: 0000 0072 1200 0000 722e 0000 00da 0561  ...r....r......a
+00001580: 7272 6179 722f 0000 0072 3100 0000 7234  rrayr/...r1...r4
+00001590: 0000 0072 3a00 0000 724a 0000 0072 4e00  ...r:...rJ...rN.
+000015a0: 0000 7253 0000 0072 5500 0000 7256 0000  ..rS...rU...rV..
+000015b0: 0072 5c00 0000 725e 0000 0072 2500 0000  .r\...r^...r%...
+000015c0: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
+000015d0: 0600 0000 0900 0000 731a 0000 0008 011c  ........s.......
+000015e0: 1d12 1112 0608 0908 030a 170a 2508 0c0a  ............%...
+000015f0: 070a 080a 050a 0b72 0600 0000 290f da05  .......r....)...
+00001600: 6e75 6d70 7972 1000 0000 5a06 6361 7361  numpyr....Z.casa
+00001610: 6469 7219 0000 005a 0e73 7061 7469 616c  dir....Z.spatial
+00001620: 5f63 6173 6164 6972 3000 0000 5a17 7363  _casadir0...Z.sc
+00001630: 6970 792e 7370 6174 6961 6c2e 7472 616e  ipy.spatial.tran
+00001640: 7366 6f72 6d72 0200 0000 722c 0000 005a  sformr....r,...Z
+00001650: 2167 7261 7370 5f70 6c61 6e6e 696e 672e  !grasp_planning.
+00001660: 736f 6c76 6572 2e72 6f62 6f74 5f6d 6f64  solver.robot_mod
+00001670: 656c 7203 0000 005a 1967 7261 7370 5f70  elr....Z.grasp_p
+00001680: 6c61 6e6e 696e 672e 636f 7374 2e63 6f73  lanning.cost.cos
+00001690: 7473 7204 0000 005a 2667 7261 7370 5f70  tsr....Z&grasp_p
+000016a0: 6c61 6e6e 696e 672e 636f 6e73 7472 6169  lanning.constrai
+000016b0: 6e74 732e 636f 6e73 7472 6169 6e74 7372  nts.constraintsr
+000016c0: 0600 0000 7225 0000 0072 2500 0000 7225  ....r%...r%...r%
+000016d0: 0000 0072 2600 0000 da08 3c6d 6f64 756c  ...r&.....<modul
+000016e0: 653e 0100 0000 730e 0000 0008 0108 0108  e>....s.........
+000016f0: 010c 010c 010c 0108 02                   .........
```

### Comparing `grasp_planning-0.5.1/grasp_planning/solver/__pycache__/robot_model.cpython-38.pyc` & `grasp_planning-0.5.2/grasp_planning/solver/__pycache__/robot_model.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 13 13:26:55 2024 UTC, .py size: 1875 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1f15 4266 5307 0000  U.........BfS...
+00000000: 550d 0d0a 0000 0000 7a6f 4366 7b07 0000  U.......zoCf{...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c04 5a05 6400 6402 6c06 6d07 5a08  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6404 6405 8400 6405 8302 5a0b 6401 5300  d.d...d...Z.d.S.
 00000070: 2906 e900 0000 004e 2901 da08 526f 7461  )......N)...Rota
@@ -12,127 +12,127 @@
 000000b0: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
 000000c0: 005a 0364 0e64 0464 0584 015a 0464 0664  .Z.d.d.d...Z.d.d
 000000d0: 0784 005a 0564 0864 0984 005a 0664 0a64  ...Z.d.d...Z.d.d
 000000e0: 0b84 005a 0764 0c64 0d84 005a 0864 0353  ...Z.d.d...Z.d.S
 000000f0: 0029 0fda 1352 6f62 6f74 4b69 6e65 6d61  .)...RobotKinema
 00000100: 7469 634d 6f64 656c 6304 0000 0000 0000  ticModelc.......
 00000110: 0000 0000 0005 0000 0009 0000 0043 0000  .............C..
-00000120: 0073 6800 0000 7400 7c01 6401 8302 8f10  .sh...t.|.d.....
+00000120: 0073 6e00 0000 7400 7c01 6401 8302 8f10  .sn...t.|.d.....
 00000130: 7d04 7c04 a001 a100 7c00 5f02 5700 3500  }.|.....|._.W.5.
 00000140: 5100 5200 5800 7403 7c00 6a02 7c02 7c03  Q.R.X.t.|.j.|.|.
-00000150: 6402 8d03 7c00 5f04 7c03 7c00 5f05 7c00  d...|._.|.|._.|.
-00000160: 6a04 a006 a100 7c00 5f07 6700 7c00 5f08  j.....|._.g.|._.
-00000170: 7409 a00a 7c00 6a07 6403 6602 a101 7c00  t...|.j.d.f...|.
-00000180: 5f0b 7c00 a00c a100 0100 6400 5300 2904  _.|.......d.S.).
-00000190: 4eda 0172 2902 da09 726f 6f74 5f6c 696e  N..r)...root_lin
-000001a0: 6b5a 0965 6e64 5f6c 696e 6b73 e902 0000  kZ.end_links....
-000001b0: 0029 0dda 046f 7065 6eda 0472 6561 64da  .)...open..read.
-000001c0: 0475 7264 6672 0300 0000 da08 726f 626f  .urdfr......robo
-000001d0: 745f 666b da08 656e 645f 6c69 6e6b da01  t_fk..end_link..
-000001e0: 6eda 066e 5f64 6f66 73da 0b6a 6f69 6e74  n..n_dofs..joint
-000001f0: 5f6e 616d 6573 da02 6e70 da05 7a65 726f  _names..np..zero
-00000200: 73da 106a 6f69 6e74 5f70 6f73 5f6c 696d  s..joint_pos_lim
-00000210: 6974 73da 165f 7265 6164 5f6a 6f69 6e74  its.._read_joint
-00000220: 5f70 6f73 5f6c 696d 6974 7329 05da 0473  _pos_limits)...s
-00000230: 656c 665a 0975 7264 665f 6669 6c65 7206  elfZ.urdf_filer.
-00000240: 0000 0072 0c00 0000 da04 6669 6c65 a900  ...r......file..
-00000250: 7216 0000 00fa 472f 686f 6d65 2f74 6f6d  r.....G/home/tom
-00000260: 6173 2f44 6573 6b74 6f70 2f67 7261 7370  as/Desktop/grasp
-00000270: 5f70 6c61 6e6e 696e 672f 6772 6173 705f  _planning/grasp_
-00000280: 706c 616e 6e69 6e67 2f73 6f6c 7665 722f  planning/solver/
-00000290: 726f 626f 745f 6d6f 6465 6c2e 7079 da08  robot_model.py..
-000002a0: 5f5f 696e 6974 5f5f 0800 0000 7318 0000  __init__....s...
-000002b0: 0000 010c 0114 0202 0104 0102 0102 fd08  ................
-000002c0: 0506 010c 0106 0112 017a 1c52 6f62 6f74  .........z.Robot
-000002d0: 4b69 6e65 6d61 7469 634d 6f64 656c 2e5f  KinematicModel._
-000002e0: 5f69 6e69 745f 5f4e 6303 0000 0000 0000  _init__Nc.......
-000002f0: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
-00000300: 0073 3200 0000 7c02 6400 6b02 721c 7c00  .s2...|.d.k.r.|.
-00000310: 6a00 6a01 7c01 7c00 6a02 6401 6402 8d03  j.j.|.|.j.d.d...
-00000320: 5300 7c00 6a00 6a01 7c01 7c02 6401 6403  S.|.j.j.|.|.d.d.
-00000330: 8d03 5300 6400 5300 2904 4e46 a901 da0d  ..S.d.S.).NF....
-00000340: 706f 7369 7469 6f6e 5f6f 6e6c 7929 025a  position_only).Z
-00000350: 0a63 6869 6c64 5f6c 696e 6b72 1a00 0000  .child_linkr....
-00000360: 2903 720b 0000 00da 0663 6173 6164 6972  ).r......casadir
-00000370: 0c00 0000 2903 7214 0000 00da 0471 5f63  ....).r......q_c
-00000380: 6172 0c00 0000 7216 0000 0072 1600 0000  ar....r....r....
-00000390: 7217 0000 00da 0d63 6f6d 7075 7465 5f66  r......compute_f
-000003a0: 6b5f 6361 1700 0000 7306 0000 0000 0108  k_ca....s.......
-000003b0: 0114 027a 2152 6f62 6f74 4b69 6e65 6d61  ...z!RobotKinema
-000003c0: 7469 634d 6f64 656c 2e63 6f6d 7075 7465  ticModel.compute
-000003d0: 5f66 6b5f 6361 6302 0000 0000 0000 0000  _fk_cac.........
-000003e0: 0000 0004 0000 0006 0000 0043 0000 0073  ...........C...s
-000003f0: 4400 0000 7c00 a000 7c01 a101 7d02 7401  D...|...|...}.t.
-00000400: 6a02 a003 7c02 6400 6401 8502 6400 6401  j...|.d.d...d.d.
-00000410: 8502 6602 1900 a101 a004 6402 a101 7d03  ..f.......d...}.
-00000420: 7405 a006 7c02 6400 6401 8502 6401 6602  t...|.d.d...d.f.
-00000430: 1900 7c03 a102 5300 2903 4ee9 0300 0000  ..|...S.).N.....
-00000440: da03 7879 7a29 0772 1d00 0000 da02 7363  ..xyz).r......sc
-00000450: 7202 0000 00da 0b66 726f 6d5f 6d61 7472  r......from_matr
-00000460: 6978 da08 6173 5f65 756c 6572 da02 6361  ix..as_euler..ca
-00000470: da07 7665 7274 6361 7429 0472 1400 0000  ..vertcat).r....
-00000480: 721c 0000 005a 0566 6b5f 6361 5a08 525f  r....Z.fk_caZ.R_
-00000490: 6361 5f72 7079 7216 0000 0072 1600 0000  ca_rpyr....r....
-000004a0: 7217 0000 00da 1163 6f6d 7075 7465 5f66  r......compute_f
-000004b0: 6b5f 7270 795f 6361 1e00 0000 7306 0000  k_rpy_ca....s...
-000004c0: 0000 010a 0122 017a 2552 6f62 6f74 4b69  .....".z%RobotKi
-000004d0: 6e65 6d61 7469 634d 6f64 656c 2e63 6f6d  nematicModel.com
-000004e0: 7075 7465 5f66 6b5f 7270 795f 6361 6302  pute_fk_rpy_cac.
-000004f0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-00000500: 0000 0043 0000 0073 1400 0000 7c00 6a00  ...C...s....|.j.
-00000510: 6a01 7c01 7c00 6a02 6401 6402 8d03 5300  j.|.|.j.d.d...S.
-00000520: 2903 4e46 7219 0000 0029 0372 0b00 0000  ).NFr....).r....
-00000530: da05 6e75 6d70 7972 0c00 0000 2902 7214  ..numpyr....).r.
-00000540: 0000 00da 0171 7216 0000 0072 1600 0000  .....qr....r....
-00000550: 7217 0000 00da 0765 7661 6c5f 666b 2300  r......eval_fk#.
-00000560: 0000 7302 0000 0000 017a 1b52 6f62 6f74  ..s......z.Robot
-00000570: 4b69 6e65 6d61 7469 634d 6f64 656c 2e65  KinematicModel.e
-00000580: 7661 6c5f 666b 6301 0000 0000 0000 0000  val_fkc.........
-00000590: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
-000005a0: 5800 0000 7c00 6a00 6a01 a002 6401 6402  X...|.j.j...d.d.
-000005b0: a102 7d01 6403 7d02 7c01 4400 5d3a 7d03  ..}.d.}.|.D.]:}.
-000005c0: 7c03 6a03 6404 6b06 7218 7c00 6a04 a005  |.j.d.k.r.|.j...
-000005d0: 7c03 6a06 a101 0100 7c03 6a07 6a08 7c03  |.j.....|.j.j.|.
-000005e0: 6a07 6a09 6702 7c00 6a0a 7c02 3c00 7c02  j.j.g.|.j.|.<.|.
-000005f0: 6405 3700 7d02 7118 6400 5300 2906 4eda  d.7.}.q.d.S.).N.
-00000600: 0577 6f72 6c64 da0e 6172 6d5f 746f 6f6c  .world..arm_tool
-00000610: 5f66 7261 6d65 7201 0000 0029 025a 0872  _framer....).Z.r
-00000620: 6576 6f6c 7574 655a 0970 7269 736d 6174  evoluteZ.prismat
-00000630: 6963 e901 0000 0029 0b72 0b00 0000 5a05  ic.....).r....Z.
-00000640: 726f 626f 745a 0e67 6574 5f6a 6f69 6e74  robotZ.get_joint
-00000650: 5f69 6e66 6fda 0474 7970 6572 0f00 0000  _info..typer....
-00000660: da06 6170 7065 6e64 da04 6e61 6d65 da05  ..append..name..
-00000670: 6c69 6d69 74da 056c 6f77 6572 da05 7570  limit..lower..up
-00000680: 7065 7272 1200 0000 2904 7214 0000 005a  perr....).r....Z
-00000690: 066a 6f69 6e74 73da 0169 5a05 6a6f 696e  .joints..iZ.join
-000006a0: 7472 1600 0000 7216 0000 0072 1700 0000  tr....r....r....
-000006b0: 7213 0000 0026 0000 0073 0e00 0000 0001  r....&...s......
-000006c0: 1001 0401 0801 0a01 0e02 1601 7a2a 526f  ............z*Ro
-000006d0: 626f 744b 696e 656d 6174 6963 4d6f 6465  botKinematicMode
-000006e0: 6c2e 5f72 6561 645f 6a6f 696e 745f 706f  l._read_joint_po
-000006f0: 735f 6c69 6d69 7473 6301 0000 0000 0000  s_limitsc.......
-00000700: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00000710: 0073 0600 0000 7c00 6a00 5300 2901 4e29  .s....|.j.S.).N)
-00000720: 0172 1200 0000 2901 7214 0000 0072 1600  .r....).r....r..
-00000730: 0000 7216 0000 0072 1700 0000 da14 6765  ..r....r......ge
-00000740: 745f 6a6f 696e 745f 706f 735f 6c69 6d69  t_joint_pos_limi
-00000750: 7473 3100 0000 7302 0000 0000 017a 2852  ts1...s......z(R
-00000760: 6f62 6f74 4b69 6e65 6d61 7469 634d 6f64  obotKinematicMod
-00000770: 656c 2e67 6574 5f6a 6f69 6e74 5f70 6f73  el.get_joint_pos
-00000780: 5f6c 696d 6974 7329 014e 2909 da08 5f5f  _limits).N)...__
-00000790: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000007a0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000007b0: 7218 0000 0072 1d00 0000 7225 0000 0072  r....r....r%...r
-000007c0: 2800 0000 7213 0000 0072 3300 0000 7216  (...r....r3...r.
-000007d0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-000007e0: 0000 7204 0000 0007 0000 0073 0c00 0000  ..r........s....
-000007f0: 0801 080f 0a07 0805 0803 080b 7204 0000  ............r...
-00000800: 0029 0c72 2600 0000 7210 0000 0072 1b00  .).r&...r....r..
-00000810: 0000 7223 0000 00da 0e73 7061 7469 616c  ..r#.....spatial
-00000820: 5f63 6173 6164 6972 2000 0000 da17 7363  _casadir .....sc
-00000830: 6970 792e 7370 6174 6961 6c2e 7472 616e  ipy.spatial.tran
-00000840: 7366 6f72 6d72 0200 0000 da01 525a 1166  sformr......RZ.f
-00000850: 6f72 7761 7264 6b69 6e65 6d61 7469 6373  orwardkinematics
-00000860: 7203 0000 0072 0400 0000 7216 0000 0072  r....r....r....r
-00000870: 1600 0000 7216 0000 0072 1700 0000 da08  ....r....r......
-00000880: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
-00000890: 0008 0108 0108 010c 010c 02              ...........
+00000150: 6402 8d03 7c00 5f04 7c02 7c00 5f05 7c03  d...|._.|.|._.|.
+00000160: 7c00 5f06 7c00 6a04 a007 a100 7c00 5f08  |._.|.j.....|._.
+00000170: 6700 7c00 5f09 740a a00b 7c00 6a08 6403  g.|._.t...|.j.d.
+00000180: 6602 a101 7c00 5f0c 7c00 a00d a100 0100  f...|._.|.......
+00000190: 6400 5300 2904 4eda 0172 2902 da09 726f  d.S.).N..r)...ro
+000001a0: 6f74 5f6c 696e 6b5a 0965 6e64 5f6c 696e  ot_linkZ.end_lin
+000001b0: 6b73 e902 0000 0029 0eda 046f 7065 6eda  ks.....)...open.
+000001c0: 0472 6561 64da 0475 7264 6672 0300 0000  .read..urdfr....
+000001d0: da08 726f 626f 745f 666b 7206 0000 00da  ..robot_fkr.....
+000001e0: 0865 6e64 5f6c 696e 6bda 016e da06 6e5f  .end_link..n..n_
+000001f0: 646f 6673 da0b 6a6f 696e 745f 6e61 6d65  dofs..joint_name
+00000200: 73da 026e 70da 057a 6572 6f73 da10 6a6f  s..np..zeros..jo
+00000210: 696e 745f 706f 735f 6c69 6d69 7473 da16  int_pos_limits..
+00000220: 5f72 6561 645f 6a6f 696e 745f 706f 735f  _read_joint_pos_
+00000230: 6c69 6d69 7473 2905 da04 7365 6c66 5a09  limits)...selfZ.
+00000240: 7572 6466 5f66 696c 6572 0600 0000 720c  urdf_filer....r.
+00000250: 0000 00da 0466 696c 65a9 0072 1600 0000  .....file..r....
+00000260: fa47 2f68 6f6d 652f 746f 6d61 732f 4465  .G/home/tomas/De
+00000270: 736b 746f 702f 6772 6173 705f 706c 616e  sktop/grasp_plan
+00000280: 6e69 6e67 2f67 7261 7370 5f70 6c61 6e6e  ning/grasp_plann
+00000290: 696e 672f 736f 6c76 6572 2f72 6f62 6f74  ing/solver/robot
+000002a0: 5f6d 6f64 656c 2e70 79da 085f 5f69 6e69  _model.py..__ini
+000002b0: 745f 5f08 0000 0073 1a00 0000 0001 0c01  t__....s........
+000002c0: 1402 0201 0401 0201 02fd 0805 0601 0601  ................
+000002d0: 0c01 0601 1201 7a1c 526f 626f 744b 696e  ......z.RobotKin
+000002e0: 656d 6174 6963 4d6f 6465 6c2e 5f5f 696e  ematicModel.__in
+000002f0: 6974 5f5f 4e63 0300 0000 0000 0000 0000  it__Nc..........
+00000300: 0000 0300 0000 0500 0000 4300 0000 7332  ..........C...s2
+00000310: 0000 007c 0264 006b 0272 1c7c 006a 006a  ...|.d.k.r.|.j.j
+00000320: 017c 017c 006a 0264 0164 028d 0353 007c  .|.|.j.d.d...S.|
+00000330: 006a 006a 017c 017c 0264 0164 038d 0353  .j.j.|.|.d.d...S
+00000340: 0064 0053 0029 044e 46a9 01da 0d70 6f73  .d.S.).NF....pos
+00000350: 6974 696f 6e5f 6f6e 6c79 2902 da0a 6368  ition_only)...ch
+00000360: 696c 645f 6c69 6e6b 721a 0000 0029 0372  ild_linkr....).r
+00000370: 0b00 0000 da06 6361 7361 6469 720c 0000  ......casadir...
+00000380: 0029 0372 1400 0000 da04 715f 6361 720c  .).r......q_car.
+00000390: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+000003a0: 0000 da0d 636f 6d70 7574 655f 666b 5f63  ....compute_fk_c
+000003b0: 6118 0000 0073 0600 0000 0001 0801 1402  a....s..........
+000003c0: 7a21 526f 626f 744b 696e 656d 6174 6963  z!RobotKinematic
+000003d0: 4d6f 6465 6c2e 636f 6d70 7574 655f 666b  Model.compute_fk
+000003e0: 5f63 6163 0200 0000 0000 0000 0000 0000  _cac............
+000003f0: 0400 0000 0600 0000 4300 0000 7344 0000  ........C...sD..
+00000400: 007c 00a0 007c 01a1 017d 0274 016a 02a0  .|...|...}.t.j..
+00000410: 037c 0264 0064 0185 0264 0064 0185 0266  .|.d.d...d.d...f
+00000420: 0219 00a1 01a0 0464 02a1 017d 0374 05a0  .......d...}.t..
+00000430: 067c 0264 0064 0185 0264 0166 0219 007c  .|.d.d...d.f...|
+00000440: 03a1 0253 0029 034e e903 0000 00da 0378  ...S.).N.......x
+00000450: 797a 2907 721e 0000 00da 0273 6372 0200  yz).r......scr..
+00000460: 0000 da0b 6672 6f6d 5f6d 6174 7269 78da  ....from_matrix.
+00000470: 0861 735f 6575 6c65 72da 0263 61da 0776  .as_euler..ca..v
+00000480: 6572 7463 6174 2904 7214 0000 0072 1d00  ertcat).r....r..
+00000490: 0000 5a05 666b 5f63 615a 0852 5f63 615f  ..Z.fk_caZ.R_ca_
+000004a0: 7270 7972 1600 0000 7216 0000 0072 1700  rpyr....r....r..
+000004b0: 0000 da11 636f 6d70 7574 655f 666b 5f72  ....compute_fk_r
+000004c0: 7079 5f63 611f 0000 0073 0600 0000 0001  py_ca....s......
+000004d0: 0a01 2201 7a25 526f 626f 744b 696e 656d  ..".z%RobotKinem
+000004e0: 6174 6963 4d6f 6465 6c2e 636f 6d70 7574  aticModel.comput
+000004f0: 655f 666b 5f72 7079 5f63 6163 0200 0000  e_fk_rpy_cac....
+00000500: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00000510: 4300 0000 7314 0000 007c 006a 006a 017c  C...s....|.j.j.|
+00000520: 017c 006a 0264 0164 028d 0353 0029 034e  .|.j.d.d...S.).N
+00000530: 4672 1900 0000 2903 720b 0000 00da 056e  Fr....).r......n
+00000540: 756d 7079 720c 0000 0029 0272 1400 0000  umpyr....).r....
+00000550: da01 7172 1600 0000 7216 0000 0072 1700  ..qr....r....r..
+00000560: 0000 da07 6576 616c 5f66 6b24 0000 0073  ....eval_fk$...s
+00000570: 0200 0000 0001 7a1b 526f 626f 744b 696e  ......z.RobotKin
+00000580: 656d 6174 6963 4d6f 6465 6c2e 6576 616c  ematicModel.eval
+00000590: 5f66 6b63 0100 0000 0000 0000 0000 0000  _fkc............
+000005a0: 0400 0000 0400 0000 4300 0000 735c 0000  ........C...s\..
+000005b0: 007c 006a 006a 01a0 027c 006a 037c 006a  .|.j.j...|.j.|.j
+000005c0: 04a1 027d 0164 017d 027c 0144 005d 3a7d  ...}.d.}.|.D.]:}
+000005d0: 037c 036a 0564 026b 0672 1c7c 006a 06a0  .|.j.d.k.r.|.j..
+000005e0: 077c 036a 08a1 0101 007c 036a 096a 0a7c  .|.j.....|.j.j.|
+000005f0: 036a 096a 0b67 027c 006a 0c7c 023c 007c  .j.j.g.|.j.|.<.|
+00000600: 0264 0337 007d 0271 1c64 0053 0029 044e  .d.7.}.q.d.S.).N
+00000610: 7201 0000 0029 025a 0872 6576 6f6c 7574  r....).Z.revolut
+00000620: 655a 0970 7269 736d 6174 6963 e901 0000  eZ.prismatic....
+00000630: 0029 0d72 0b00 0000 da05 726f 626f 745a  .).r......robotZ
+00000640: 0e67 6574 5f6a 6f69 6e74 5f69 6e66 6f72  .get_joint_infor
+00000650: 0600 0000 720c 0000 00da 0474 7970 6572  ....r......typer
+00000660: 0f00 0000 da06 6170 7065 6e64 da04 6e61  ......append..na
+00000670: 6d65 da05 6c69 6d69 74da 056c 6f77 6572  me..limit..lower
+00000680: da05 7570 7065 7272 1200 0000 2904 7214  ..upperr....).r.
+00000690: 0000 005a 066a 6f69 6e74 73da 0169 5a05  ...Z.joints..iZ.
+000006a0: 6a6f 696e 7472 1600 0000 7216 0000 0072  jointr....r....r
+000006b0: 1700 0000 7213 0000 0027 0000 0073 0e00  ....r....'...s..
+000006c0: 0000 0001 1401 0401 0801 0a01 0e02 1601  ................
+000006d0: 7a2a 526f 626f 744b 696e 656d 6174 6963  z*RobotKinematic
+000006e0: 4d6f 6465 6c2e 5f72 6561 645f 6a6f 696e  Model._read_join
+000006f0: 745f 706f 735f 6c69 6d69 7473 6301 0000  t_pos_limitsc...
+00000700: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00000710: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
+00000720: 2901 4e29 0172 1200 0000 2901 7214 0000  ).N).r....).r...
+00000730: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000740: da14 6765 745f 6a6f 696e 745f 706f 735f  ..get_joint_pos_
+00000750: 6c69 6d69 7473 3200 0000 7302 0000 0000  limits2...s.....
+00000760: 017a 2852 6f62 6f74 4b69 6e65 6d61 7469  .z(RobotKinemati
+00000770: 634d 6f64 656c 2e67 6574 5f6a 6f69 6e74  cModel.get_joint
+00000780: 5f70 6f73 5f6c 696d 6974 7329 014e 2909  _pos_limits).N).
+00000790: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000007a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+000007b0: 6d65 5f5f 7218 0000 0072 1e00 0000 7226  me__r....r....r&
+000007c0: 0000 0072 2900 0000 7213 0000 0072 3300  ...r)...r....r3.
+000007d0: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
+000007e0: 0072 1700 0000 7204 0000 0007 0000 0073  .r....r........s
+000007f0: 0c00 0000 0801 0810 0a07 0805 0803 080b  ................
+00000800: 7204 0000 0029 0c72 2700 0000 7210 0000  r....).r'...r...
+00000810: 0072 1c00 0000 7224 0000 00da 0e73 7061  .r....r$.....spa
+00000820: 7469 616c 5f63 6173 6164 6972 2100 0000  tial_casadir!...
+00000830: da17 7363 6970 792e 7370 6174 6961 6c2e  ..scipy.spatial.
+00000840: 7472 616e 7366 6f72 6d72 0200 0000 da01  transformr......
+00000850: 525a 1166 6f72 7761 7264 6b69 6e65 6d61  RZ.forwardkinema
+00000860: 7469 6373 7203 0000 0072 0400 0000 7216  ticsr....r....r.
+00000870: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00000880: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000890: 730a 0000 0008 0108 0108 010c 010c 02    s..............
```

### Comparing `grasp_planning-0.5.1/grasp_planning/solver/gomp_planner.py` & `grasp_planning-0.5.2/grasp_planning/solver/gomp_planner.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,21 +38,24 @@
 
     def update_grasp_DOF(self, theta: float, degrees=True) -> None:
         """
         Object has to have z-axis aligned with the world frame
         """
         self.T_Obj_Grasp = np.eye(4, dtype=float)
         if degrees:
-            R_Obj_Grasp = R.from_euler('xyz', [180, 0, theta], degrees=True).as_matrix()
-            self.theta = np.round(np.deg2rad(theta), 2)
+            self.theta = np.deg2rad(theta)
+            self.R_Obj_Grasp = R.from_euler('xyz', [180, 0, self.theta], degrees=True).as_matrix()
         else:
-            R_Obj_Grasp = R.from_euler('xyz', [np.pi, 0, theta], degrees=False).as_matrix()
-            self.theta = np.round(theta, 2)
-        self.T_Obj_Grasp[:3,:3] = R_Obj_Grasp
+            self.theta = theta
+            self.R_Obj_Grasp = R.from_euler('xyz', [np.pi, 0, self.theta], degrees=False).as_matrix()
+        self.T_Obj_Grasp[:3,:3] = self.R_Obj_Grasp
         self.T_W_Grasp = self.T_W_Obj @ self.T_Obj_Grasp
+        
+        # print("T_W_Grasp\n", self.T_W_Grasp)
+
 
     def update_object_pose(self, T_W_Obj: np.array) -> None:
         """
         Update object and grasp poses
         """
         self.T_W_Obj = T_W_Obj
 
@@ -75,16 +78,15 @@
             self.u_joint_limits = np.full((self.x_dim, self.n_waypoints), 100.0)
 
             # get joint limits
             joint_limits = self._robot_model.get_joint_pos_limits()
             for t in range(self.n_waypoints):
                 self.l_joint_limits[:self.n_dofs, t] = joint_limits[:,0]
                 self.u_joint_limits[:self.n_dofs, t] = joint_limits[:,1]
-                self.l_joint_limits[-3:, t] = -2*np.pi
-                self.u_joint_limits[-3:, t] = 2*np.pi
+ 
 
         
         # init boundary
         self.l_joint_limits[:,0] = q_start
         self.u_joint_limits[:,0] = q_start
 
         if q_end != None:
@@ -131,19 +133,19 @@
         
     def solve(self):
         result = self.solver(x0=self.x_init,
                              lbg=self.g_lb,
                              ubg=self.g_ub,
                              lbx=self.l_joint_limits.reshape((-1,1), order='F'),
                              ubx=self.u_joint_limits.reshape((-1,1), order='F'),
-                             p=self.params_optim_num)
-        
+                             p=self.T_W_Grasp)
+
         success_flag = self.solver.stats()["success"]
         success_msg = self.solver.stats()["return_status"]
-        return  np.reshape(result['x'], (self.n_dofs, self.n_waypoints)), success_flag
+        return  result['x'].reshape((self.n_dofs, self.n_waypoints)), success_flag
 
     def _add_grasp_pos_constraint(self, waypoint_ID, tolerance=0.0):
         self.g_list.append(GraspPosConstraint(self._robot_model, 
                                               self.x, 
                                               waypoint_ID, 
                                               self.param_grasp_ca, 
                                               tolerance))
@@ -173,10 +175,10 @@
                                                 tolerance=tolerance))
 
     def update_constraints_params(self, T_W_Obj, T_W_Obst=None):
         self.update_object_pose(T_W_Obj)
         self.update_grasp_DOF(theta=self.theta, degrees=False)
 
         if self._collision_flag:
-            self.params_optim_num = ca.vertcat(T_W_Obj, T_W_Obst)
+            self.params_optim_num = ca.vertcat(self.T_W_Grasp, T_W_Obst)
         else:
-            self.params_optim_num = T_W_Obj
+            self.params_optim_num = self.T_W_Grasp
```

### Comparing `grasp_planning-0.5.1/grasp_planning/solver/robot_model.py` & `grasp_planning-0.5.2/grasp_planning/solver/robot_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
             self.urdf = file.read()
 
         self.robot_fk = GenericURDFFk(
                             self.urdf,
                             root_link = root_link,
                             end_links= end_link
                         )
+        self.root_link = root_link
         self.end_link = end_link
         self.n_dofs = self.robot_fk.n()
         self.joint_names = []
         self.joint_pos_limits = np.zeros((self.n_dofs, 2))
         self._read_joint_pos_limits()
 
     def compute_fk_ca(self, q_ca, end_link=None):
@@ -32,15 +33,15 @@
         R_ca_rpy = sc.Rotation.from_matrix(fk_ca[:3,:3]).as_euler("xyz") #convert rotation part of FK into rpy
         return ca.vertcat(fk_ca[:3,3], R_ca_rpy)
 
     def eval_fk(self, q):
         return self.robot_fk.numpy(q, self.end_link, position_only=False)
 
     def _read_joint_pos_limits(self):
-        joints = self.robot_fk.robot.get_joint_info('world', 'arm_tool_frame')
+        joints = self.robot_fk.robot.get_joint_info(self.root_link, self.end_link )
         i = 0
         for joint in joints:
             if joint.type in ["revolute", "prismatic"]:
                 self.joint_names.append(joint.name)
                 # self.joint_pos_limits.append([joint.limit.lower, joint.limit.upper])
                 self.joint_pos_limits[i] = [joint.limit.lower, joint.limit.upper]
                 i += 1
```

### Comparing `grasp_planning-0.5.1/PKG-INFO` & `grasp_planning-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grasp_planning
-Version: 0.5.1
+Version: 0.5.2
 Summary: "Grasp and Motion Planning Python Package."
 License: MIT
 Author: Tomas Merva
 Author-email: tmerva7@gmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

