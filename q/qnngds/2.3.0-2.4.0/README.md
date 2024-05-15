# Comparing `tmp/qnngds-2.3.0.tar.gz` & `tmp/qnngds-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnngds-2.3.0.tar", last modified: Mon Apr 29 20:32:55 2024, max compression
+gzip compressed data, was "qnngds-2.4.0.tar", last modified: Tue May 14 21:12:34 2024, max compression
```

## Comparing `qnngds-2.3.0.tar` & `qnngds-2.4.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1081 2024-04-29 20:32:53.220975 qnngds-2.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1129 2024-04-29 20:32:53.220975 qnngds-2.3.0/README.md
--rw-r--r--   0        0        0     1161 2024-04-29 20:32:55.984981 qnngds-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      536 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/__init__.py
--rw-r--r--   0        0        0      290 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/_default_param.py
--rw-r--r--   0        0        0    28436 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/cells.py
--rw-r--r--   0        0        0    10495 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/circuits.py
--rw-r--r--   0        0        0    30532 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/design.py
--rw-r--r--   0        0        0      158 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/devices/__init__.py
--rw-r--r--   0        0        0      231 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/devices/htron.py
--rw-r--r--   0        0        0     1214 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/devices/nanowire.py
--rw-r--r--   0        0        0     4526 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/devices/ntron.py
--rw-r--r--   0        0        0     5935 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/devices/resistor.py
--rw-r--r--   0        0        0     2548 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/devices/snspd.py
--rw-r--r--   0        0        0     1237 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/geometries.py
--rw-r--r--   0        0        0     8009 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/tests.py
--rw-r--r--   0        0        0    28616 2024-04-29 20:32:53.236975 qnngds-2.3.0/src/qnngds/utilities.py
--rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-05-14 21:12:29.966925 qnngds-2.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2024-05-14 21:12:29.966925 qnngds-2.4.0/README.md
+-rw-r--r--   0        0        0     1161 2024-05-14 21:12:34.642913 qnngds-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      543 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/_default_param.py
+-rw-r--r--   0        0        0    28759 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/cells.py
+-rw-r--r--   0        0        0    10385 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/circuits.py
+-rw-r--r--   0        0        0    30526 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/design.py
+-rw-r--r--   0        0        0      158 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/devices/__init__.py
+-rw-r--r--   0        0        0      231 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/devices/htron.py
+-rw-r--r--   0        0        0     1313 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/devices/nanowire.py
+-rw-r--r--   0        0        0     3136 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/devices/ntron.py
+-rw-r--r--   0        0        0     6365 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/devices/resistor.py
+-rw-r--r--   0        0        0     4561 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/devices/snspd.py
+-rw-r--r--   0        0        0     1300 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/geometries.py
+-rw-r--r--   0        0        0     8683 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/tests.py
+-rw-r--r--   0        0        0    28662 2024-05-14 21:12:29.982925 qnngds-2.4.0/src/qnngds/utilities.py
+-rw-r--r--   0        0        0     3331 2024-05-14 21:12:29.982925 qnngds-2.4.0/tests/all_dev_on_gds.py
+-rw-r--r--   0        0        0      922 2024-05-14 21:12:29.982925 qnngds-2.4.0/tests/single_dev_on_gds.py
+-rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.4.0/PKG-INFO
```

### Comparing `qnngds-2.3.0/LICENSE.txt` & `qnngds-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qnngds-2.3.0/README.md` & `qnngds-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `qnngds-2.3.0/pyproject.toml` & `qnngds-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "qnngds"
-version = "2.3.0"
+version = "2.4.0"
 authors = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
     { name = "A. Jacquillat", email = "audrey.jacquillat@gmail.com" },
     { name = "R. Foster", email = "reedf@mit.edu" },
 ]
 maintainers = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
```

### Comparing `qnngds-2.3.0/src/qnngds/__init__.py` & `qnngds-2.4.0/src/qnngds/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import devices, circuits, design, geometries, tests, utilities
+from . import devices, circuits, cells, design, geometries, tests, utilities
 
 
 def help():
     """Provides links to documentation."""
 
     print(
         "Need help? Check qnngds documentation: https://qnngds.readthedocs.io/en/latest/ \n"
```

### Comparing `qnngds-2.3.0/src/qnngds/cells.py` & `qnngds-2.4.0/src/qnngds/cells.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     """Creates alignment marks in an integer number of unit cells.
 
     Parameters:
         die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
         layers_to_align (list of int): Layers to align.
         outline_die (int or float): The width of the die's outline.
         die_layer (int): The layer where the die is placed.
-        text (str): Text to be displayed.
+        text (str, optional): If None, the text is f"lay={layers_to_align}".
 
     Returns:
         DIE_ALIGN (Device): A device that centers the alignment marks in an n*m unit cell.
     """
 
     if text is None:
-        text = ""
-    DIE = Device(f"DIE ALIGN {text} ")
+        text = f"lay={layers_to_align}"
+    DIE = Device(f"CELL.ALIGN({text})")
 
     ALIGN = test.alignment_mark(layers_to_align)
 
     n = math.ceil((ALIGN.xsize) / die_w)
     m = math.ceil((ALIGN.ysize) / die_w)
 
     BORDER = utility.die_cell(
@@ -79,26 +79,26 @@
         die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
         pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
         layers_to_probe (list of int): The layers on which to place the VDP structure.
         layers_to_outline (list of int): Among the VDP layers, the ones for which structure must not be filled but outlined.
         outline (int or float): The width of the VDP and die's outline.
         die_layer (int or tuple of int): The layer where the die is placed.
         pad_layer (int or tuple of int): The layer where the pads are placed.
-        text (str, optional): If None, the text is f"VDP \n{layers_to_probe}".
+        text (str, optional): If None, the text is f"lay={layers_to_probe}".
     Returns:
         DIE_VANDP (Device): The created device.
     """
     # Initialize parameters left to default (=None)
 
     if text is None:
-        text = str(layers_to_probe)
+        text = f"lay={layers_to_probe}"
     if layers_to_outline is None:
         layers_to_outline = [die_layer]  # default layer to outline if None is given
 
-    DIE_VANDP = Device(f"DIE VAN DER PAUW {text} ")
+    DIE_VANDP = Device(f"CELL.VDP({text})")
 
     device_max_w = die_w - 2 * (
         pad_size[1] + 2 * outline
     )  # width of max device size for this cell
     contact_w = device_max_w / 10  # choosing a contact width 10 times smaller
     device_w = (
         device_max_w - 2 * contact_w
@@ -108,21 +108,21 @@
 
     DIE = utility.die_cell(
         die_size=(die_w, die_w),
         device_max_size=(device_max_w, device_max_w),
         ports={},
         ports_gnd=[],
         isolation=outline,
-        text=text,
+        text=f"VDP \n{text}",
         layer=die_layer,
         pad_layer=pad_layer,
         invert=True,
         fill_pad_layer=False,
     )
-    DIE_VANDP << DIE
+    DIE_VANDP << DIE.flatten()
 
     # Creates the vdp structure, add pads and route
 
     VDP = Device()
 
     ## VDP probed area
     AREA = test.vdp(device_w, contact_w)
@@ -151,20 +151,21 @@
     ROUTES = utility.route_to_dev(PADS.get_ports(), AREA.ports)
     VDP << ROUTES
 
     VDP.flatten(0)
 
     # Outline the vdp structure for layers that need to be outlined
 
-    DEVICE = Device("VAN DER PAUW")
+    DEVICE = Device(f"VDP(lay={layers_to_probe})")
 
     for layer in layers_to_probe:
         TEST_LAY = pg.deepcopy(VDP)
         if layer in layers_to_outline:
             TEST_LAY = pg.outline(TEST_LAY, outline)
+        TEST_LAY.name = f"VDP(lay={layer})"
         DEVICE << TEST_LAY.flatten(single_layer=layer)
 
     DIE_VANDP << DEVICE
 
     # Add pads if they are not in already present
     if pad_layer not in layers_to_probe:
         PADS = pg.union(PADS, layer=pad_layer)
@@ -189,25 +190,25 @@
 
     Parameters:
         die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
         layers_to_etch (list of list of int): Each element of the list corresponds to one test point, to put on the list of layers specified.
                                                Example: [[1, 2], [1], [2]]
         outline_die (int or float): The width of the die's outline.
         die_layer (int): The layer where the die is placed.
-        text (str): Text to be displayed.
+        text (str, optional): If None, the text is f"lay={layers_to_etch}".
 
     Returns:
         DIE_ETCH_TEST (Device): A device (with size n*m of unit cells) with etch tests in its center.
     """
 
     if text is None:
-        text = f"{layers_to_etch}"
-    DIE_ETCH_TEST = Device(f"DIE ETCH TEST {text} ")
+        text = f"lay={layers_to_etch}"
+    DIE_ETCH_TEST = Device(f"CELL.ETCH_TEST({text})")
 
-    TEST = Device()
+    TEST = Device(f"ETCH_TEST({text})")
 
     ## Create the probing areas
 
     margin = 0.12 * die_w
     rect = pg.rectangle((die_w - 2 * margin, die_w - 2 * margin))
     for i, layer_to_etch in enumerate(layers_to_etch):
         probe = Device()
@@ -227,15 +228,15 @@
         isolation=outline_die,
         layer=die_layer,
         invert=True,
     )
 
     BORDER.move(TEST.center)
     DIE_ETCH_TEST << BORDER.flatten()
-    DIE_ETCH_TEST << TEST
+    DIE_ETCH_TEST << TEST.flatten()
     DIE_ETCH_TEST.move(DIE_ETCH_TEST.center, (0, 0))
 
     return DIE_ETCH_TEST
 
 
 def resolution_test(
     die_w: Union[int, float] = dflt.die_w,
@@ -259,26 +260,26 @@
 
     Parameters:
         die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
         layer_to_resolve (int): The layer to put the resolution test on.
         resolutions_to_test (list of float): The resolutions to test in µm.
         outline (int or float): The width of the VDP and die's outline.
         die_layer (int or tuple of int): The layer where the die is placed.
-        text (str, optional): If None, the text is f"RES TEST \n{layer_to_resolve}".
+        text (str, optional): If None, the text is f"lay={layer_to_resolve}".
 
     Returns:
         DIE_RES_TEST (Device): The created device.
     """
 
     if text is None:
-        text = layer_to_resolve
-    DIE_RES_TEST = Device(f"DIE RESOLUTION TEST {text} ")
+        text = f"lay={layer_to_resolve}"
+    DIE_RES_TEST = Device(f"CELL.RESOLUTION_TEST({text})")
 
     ## Create the test structure
-    TEST_RES = Device(f"RESOLUTION TEST {text} ")
+    TEST_RES = Device(f"RESOLUTION_TEST({text})")
     test_res = TEST_RES << test.resolution_test(
         resolutions=resolutions_to_test, inverted=False, layer=layer_to_resolve
     )
     test_res_invert = TEST_RES << test.resolution_test(
         resolutions=resolutions_to_test,
         inverted=resolutions_to_test[-1],
         layer=layer_to_resolve,
@@ -292,22 +293,21 @@
     ## Create the die
     n = math.ceil((TEST_RES.xsize) / die_w)
     m = math.ceil((TEST_RES.ysize) / die_w)
     BORDER = utility.die_cell(
         die_size=(n * die_w, m * die_w),
         ports={},
         ports_gnd=[],
-        text=f"RES TEST \n{text} ",
+        text=f"RES TEST \n{text}",
         isolation=outline,
         layer=die_layer,
         invert=True,
     )
 
     DIE_RES_TEST << BORDER.flatten()
-
     return DIE_RES_TEST
 
 
 ## devices:
 
 
 def nanowires(
@@ -337,34 +337,36 @@
             ports to assure alignment with the device (useful for ebeam
             lithography).
         outline_die (int or float): The width of the pads outline.
         outline_dev (int or float): The width of the device's outline.
         device_layer (int or tuple of int): The layer where the device is placed.
         die_layer (int or tuple of int): The layer where the die is placed.
         pad_layer (int or tuple of int): The layer where the pads are placed.
-        text (str, optional): If None, the text is "NWIRES".
+        text (str, optional): If None, the text is f"w={channels_w}".
         fill_pad_layer (bool): If True, the space reserved for pads in the
             die_cell in filled in pad's layer.
 
     Returns:
         Device: A device (of size n*m unit cells) containing the nanowires, the
         border of the die (created with die_cell function), and the connections
         between the nanowires and pads.
     """
 
     if text is None:
-        text = ""
+        channels_w = [item[0] for item in channels_sources_w]
+        text = f"w={channels_w}"
+    cell_text = text.replace(" \n", ", ")
 
-    NANOWIRES_DIE = Device(f"DIE NWIRES {text} ")
+    NANOWIRES_DIE = Device(f"CELL.NWIRES({cell_text})")
 
-    DEVICE = Device(f"NWIRES {text} ")
+    DEVICE = Device(f"NWIRES({cell_text})")
 
     ## Create the NANOWIRES
 
-    NANOWIRES = Device()
+    NANOWIRES = Device(f"NWIRES({cell_text})")
     nanowires_ref = []
     for i, channel_source_w in enumerate(channels_sources_w):
         nanowire_ref = NANOWIRES << device.nanowire.spot(
             channel_source_w[0], channel_source_w[1]
         )
         nanowires_ref.append(nanowire_ref)
     DEVICE << NANOWIRES
@@ -385,15 +387,15 @@
         device_max_size=dev_max_size,
         pad_size=pad_size,
         contact_w=die_contact_w,
         contact_l=overlap_w,
         ports={"N": n, "S": n},
         ports_gnd=["S"],
         isolation=outline_die,
-        text=f"NWIRES {text}",
+        text=f"NWIRES\n{text}",
         layer=die_layer,
         pad_layer=pad_layer,
         invert=True,
         fill_pad_layer=fill_pad_layer,
     )
 
     ## Place the nanowires
@@ -413,23 +415,22 @@
     DEVICE << HT
 
     # routes from nanowires to hyper tapers
     ROUTES = utility.route_to_dev(HT.get_ports(), NANOWIRES.ports)
     DEVICE << ROUTES
 
     DEVICE.ports = dev_ports.ports
-    DEVICE = pg.outline(DEVICE, outline_dev, open_ports=2 * outline_dev)
-    DEVICE = pg.union(DEVICE, layer=device_layer)
-    DEVICE.name = f"NWIRES {text} "
+    DEVICE = pg.outline(
+        DEVICE, outline_dev, open_ports=2 * outline_dev, layer=device_layer
+    )
+    DEVICE.name = f"NWIRES({cell_text})"
 
     NANOWIRES_DIE << DEVICE
     NANOWIRES_DIE << BORDER
 
-    NANOWIRES_DIE = pg.union(NANOWIRES_DIE, by_layer=True)
-    NANOWIRES_DIE.name = f"DIE NWIRES {text} "
     return NANOWIRES_DIE
 
 
 def ntron(
     die_w: Union[int, float] = dflt.die_w,
     pad_size: Tuple[float, float] = dflt.pad_size,
     choke_w: Union[int, float] = 0.1,
@@ -443,15 +444,15 @@
     outline_dev: Union[None, int, float] = dflt.device_outline,
     device_layer: int = dflt.layers["device"],
     die_layer: int = dflt.layers["die"],
     pad_layer: int = dflt.layers["pad"],
     text: Union[None, str] = dflt.text,
     fill_pad_layer: bool = False,
 ) -> Device:
-    """Creates a standardized cell specifically for a single ntron.
+    r"""Creates a standardized cell specifically for a single ntron.
 
     Unless specified, scales the ntron parameters as:
     gate_w = drain_w = source_w = 3 * channel_w
     choke_shift = -3 * channel_w
 
     Parameters:
         die_w (int or float): Width of a unit die/cell in the design (the output
@@ -467,15 +468,15 @@
             ports to assure alignment with the device (useful for ebeam
             lithography).
         outline_die (int or float): The width of the pads outline.
         outline_dev (int or float): The width of the device's outline.
         device_layer (int or array-like[2]): The layer where the device is placed.
         die_layer (int or array-like[2]): The layer where the die is placed.
         pad_layer (int or array-like[2]): The layer where the pads are placed.
-        text (string, optional): If None, the text is the ntron's choke and channel widths.
+        text (string, optional): If None, the text is f"chk: {choke_w} \\nchnl: {channel_w}".
         fill_pad_layer (bool): If True, the space reserved for pads in the
             die_cell in filled in pad's layer.
 
     Returns:
         Device: A device containing the ntron, the border of the die (created with die_cell function),
         and the connections between the ports.
     """
@@ -490,23 +491,24 @@
     else:
         drain_w = source_w
     if gate_w is None:
         gate_w = source_w
     if choke_shift is None:
         choke_shift = -3 * channel_w
 
-    NTRON = device.ntron.smooth_compassPorts(
+    NTRON = device.ntron.smooth(
         choke_w, gate_w, channel_w, source_w, drain_w, choke_shift, device_layer
     )
-
+    NTRON = utility.rename_ports_to_compass(NTRON)
     if text is None:
         text = f"chk: {choke_w} \nchnl: {channel_w}"
-    DIE_NTRON = Device(f"DIE NTRON {text} ")
+    cell_text = text.replace(" \n", ", ")
+    DIE_NTRON = Device(f"CELL.NTRON({cell_text})")
 
-    DEVICE = Device(f"NTRON {text} ")
+    DEVICE = Device(f"NTRON({cell_text})")
     DEVICE << NTRON
 
     ## Create the DIE
 
     # die parameters, checkup conditions
     die_contact_w = NTRON.ports["N1"].width + overlap_w
     routes_margin = 2 * die_contact_w
@@ -520,15 +522,15 @@
         die_size=(die_w, die_w),
         device_max_size=(device_max_w, device_max_w),
         pad_size=pad_size,
         contact_w=die_contact_w,
         contact_l=overlap_w,
         ports={"N": 1, "W": 1, "S": 1},
         ports_gnd=["S"],
-        text=text,
+        text=f"NTRON \n{text}",
         isolation=outline_die,
         layer=die_layer,
         pad_layer=pad_layer,
         invert=True,
         fill_pad_layer=fill_pad_layer,
     )
 
@@ -546,21 +548,19 @@
     DEVICE.ports = device_ports.ports
     # routes
     ROUTES = utility.route_to_dev(HT.get_ports(), NTRON.ports, device_layer)
     DEVICE << ROUTES
 
     DEVICE = pg.outline(DEVICE, outline_dev, precision=0.000001, open_ports=outline_dev)
     DEVICE = pg.union(DEVICE, layer=device_layer)
-    DEVICE.name = f"NTRON {text} "
+    DEVICE.name = f"NTRON({cell_text})"
 
     DIE_NTRON << DEVICE
     DIE_NTRON << BORDER
 
-    DIE_NTRON = pg.union(DIE_NTRON, by_layer=True)
-    DIE_NTRON.name = f"DIE NTRON {text} "
     return DIE_NTRON
 
 
 def snspd(
     die_w: Union[int, float] = dflt.die_w,
     pad_size: Tuple[float] = dflt.pad_size,
     snspd_width: float = 0.2,
@@ -594,26 +594,27 @@
             ports to assure alignment with the device (useful for ebeam
             lithography).
         outline_die (int or float): The width of the pads outline.
         outline_dev (int or float): The width of the device's outline.
         device_layer (int or array-like[2]): The layer where the device is placed.
         die_layer (int or array-like[2]): The layer where the die is placed.
         pad_layer (int or array-like[2]): The layer where the pads are placed.
-        text (string, optional): If None, text = f'SNSPD {w_choke}'.
+        text (string, optional): If None, the text is f"w={snspd_width}".
         fill_pad_layer (bool): If True, the space reserved for pads in the
             die_cell in filled in pad's layer.
 
     Returns:
         Device: A cell (of size n*m unit die_cells) containing the SNSPD.
     """
     if text is None:
-        text = f"{snspd_width}"
+        text = f"w={snspd_width}"
+    cell_text = text.replace(" \n", ", ")
 
-    SNSPD_CELL = Device(f"CELL SNSPD {text} ")
-    DEVICE = Device(f"SNSPD {text} ")
+    SNSPD_CELL = Device(f"CELL.SNSPD({cell_text})")
+    DEVICE = Device(f"SNSPD({cell_text})")
 
     # create SNSPD, make its ports compass, add safe optimal step
     SNSPD = device.snspd.vertical(
         wire_width=snspd_width,
         wire_pitch=snspd_pitch,
         size=snspd_size,
         num_squares=snspd_num_squares,
@@ -637,15 +638,15 @@
         die_size=(n * die_w, m * die_w),
         device_max_size=device_max_size,
         pad_size=pad_size,
         contact_w=die_contact_w,
         contact_l=overlap_w,
         ports={"N": 1, "S": 1},
         ports_gnd=["S"],
-        text=f"SNSPD {text}",
+        text=f"SNSPD \n{text}",
         isolation=outline_die,
         layer=die_layer,
         pad_layer=pad_layer,
         invert=True,
         fill_pad_layer=fill_pad_layer,
     )
 
@@ -662,15 +663,15 @@
         HT.get_ports(), SNSPD.ports
     )  # absolutly no need to route, but will be useful when ports are no longer aligned with pads
     DEVICE << ROUTES
 
     DEVICE = pg.outline(
         DEVICE, outline_dev, open_ports=2 * outline_dev, layer=device_layer
     )
-    DEVICE.name = f"SNSPD {text} "
+    DEVICE.name = f"SNSPD({cell_text})"
 
     SNSPD_CELL << DEVICE
     SNSPD_CELL << BORDER
     return SNSPD_CELL
 
 
 def snspd_ntron(
@@ -698,31 +699,33 @@
         overlap_w (int or float): Extra length of the routes above the die's ports to assure alignment with the device
                                              (useful for ebeam lithography).
         outline_die (int or float): The width of the pads outline.
         outline_dev (int or float): The width of the device's outline.
         device_layer (int or array-like[2]): The layer where the device is placed.
         die_layer (int or array-like[2]): The layer where the die is placed.
         pad_layer (int or array-like[2]): The layer where the pads are placed.
-        text (string, optional): If None, text = f'SNSPD {w_choke}'.
+        text (string, optional): If None, the text is f"w={w_snspd}, {w_choke}".
         fill_pad_layer (bool): If True, the space reserved for pads in the
             die_cell in filled in pad's layer.
 
     Returns:
         Device: A cell containing a die in die_layer, pads in pad layer,
         and an SNSPD-NTRON properly routed in the device layer.
     """
 
     # Create SNSPD-NTRON
     if w_snspd is None:
         w_snspd = 5 * w_choke
 
     if text is None:
-        text = f"SNSPD \n{w_snspd} {w_choke} "
-    DIE_SNSPD_NTRON = Device(f"DIE {text} ")
-    DEVICE = Device(f"{text} ")
+        text = f"w={w_snspd}, {w_choke}"
+    cell_text = text.replace(" \n", ", ")
+
+    DIE_SNSPD_NTRON = Device(f"CELL.SNSPD-NTRON({cell_text})")
+    DEVICE = Device(f"SNSPD-NTRON({cell_text})")
 
     SNSPD_NTRON = circuit.snspd_ntron(
         w_snspd=w_snspd,
         pitch_snspd=3 * w_snspd,
         size_snspd=(30 * w_snspd, 30 * w_snspd),
         w_inductor=3 * w_snspd,
         pitch_inductor=6 * w_snspd,
@@ -764,15 +767,15 @@
         die_size=(n * die_w, m * die_w),
         device_max_size=device_max_size,
         pad_size=pad_size,
         contact_w=die_contact_w,
         contact_l=overlap_w,
         ports={"N": 3, "E": 1, "W": 1, "S": 2},
         ports_gnd=["S"],
-        text=text,
+        text=f"SNSPD-NTRON\n{text}",
         isolation=outline_die,
         layer=die_layer,
         pad_layer=pad_layer,
         invert=True,
         fill_pad_layer=fill_pad_layer,
     )
 
@@ -788,16 +791,13 @@
 
     # routes
     ROUTES = utility.route_to_dev(HT.get_ports(), SNSPD_NTRON.ports, device_layer)
     DEVICE << ROUTES
 
     DEVICE = pg.outline(DEVICE, outline_dev, precision=0.000001, open_ports=outline_dev)
     DEVICE = pg.union(DEVICE, layer=device_layer)
-    DEVICE.name = f"DIE {text} "
+    DEVICE.name = f"SNSPD-NTRON({cell_text})"
 
     DIE_SNSPD_NTRON << DEVICE
     DIE_SNSPD_NTRON << BORDER
 
-    DIE_SNSPD_NTRON = pg.union(DIE_SNSPD_NTRON, by_layer=True)
-    DIE_SNSPD_NTRON.name = f"SNSPD \n{w_snspd} {w_choke} "
-
     return DIE_SNSPD_NTRON
```

### Comparing `qnngds-2.3.0/src/qnngds/circuits.py` & `qnngds-2.4.0/src/qnngds/circuits.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ntron, logic gates etc.)"""
 
 from phidl import Device
 import phidl.geometry as pg
 from typing import Tuple, Union
 import math
 
-import qnngds.devices as qd
+import qnngds.devices as device
 
 
 def snspd_ntron(
     w_snspd: float = 0.1,
     pitch_snspd: float = 0.3,
     size_snspd: Tuple[Union[int, float]] = (3, 3),
     w_inductor: float = 0.3,
@@ -115,176 +115,171 @@
         D.add_port(port=first_tee.ports[3], name="E")
 
         D.flatten()
         return D
 
     def create_snspd():
         ## SNSPD
-        SNSPD = SNSPD_NTRON << pg.snspd(
+        SNSPD = SNSPD_NTRON << device.snspd.basic(
             wire_width=w_snspd,
             wire_pitch=pitch_snspd,
             size=size_snspd,
             num_squares=None,
             turn_ratio=4,
             terminals_same_side=False,
             layer=layer,
         )
         SNSPD.rotate(90)
         # port 1 connected to gnd
-        route = SNSPD_NTRON << pg.optimal_step(
-            SNSPD.ports[1].width, w_pad, symmetric=True
-        )
+        route = ROUTES << pg.optimal_step(SNSPD.ports[1].width, w_pad, symmetric=True)
         route.connect(route.ports[1], SNSPD.ports[1])
         SNSPD_NTRON.add_port(port=route.ports[2], name="S1")
         # port 2 connected to crossA south
-        route_step = SNSPD_NTRON << pg.optimal_step(
+        route_step = ROUTES << pg.optimal_step(
             SNSPD.ports[2].width, CROSSA.ports["S"].width, symmetric=True
         )
         route_step.connect(route_step.ports[1], SNSPD.ports[2])
-        route = SNSPD_NTRON << pg.compass((w_inductor, w_pad / 2))
+        route = ROUTES << pg.compass((w_inductor, w_pad / 2))
         route.connect(route.ports["S"], route_step.ports[2])
         CROSSA.connect(CROSSA.ports["S"], route.ports["N"])
 
     def create_inductor1():
         ## INDUCTOR1
-        INDUCTOR1 = SNSPD_NTRON << pg.snspd(
+        INDUCTOR1 = SNSPD_NTRON << device.snspd.basic(
             wire_width=w_inductor,
             wire_pitch=pitch_inductor,
             size=size_inductor13,
             num_squares=None,
             terminals_same_side=False,
             layer=layer,
         )
         INDUCTOR1.rotate(90).mirror()
         # port 1 connected to crossA north
-        route = SNSPD_NTRON << pg.compass((w_inductor, w_pad / 2))
+        route = ROUTES << pg.compass((w_inductor, w_pad / 2))
         route.connect(route.ports["S"], CROSSA.ports["N"])
         INDUCTOR1.connect(INDUCTOR1.ports[1], route.ports["N"])
         # port 2 connected to pad
-        route = SNSPD_NTRON << pg.optimal_step(
+        route = ROUTES << pg.optimal_step(
             INDUCTOR1.ports[2].width, w_pad, symmetric=True
         )
         route.connect(route.ports[1], INDUCTOR1.ports[2])
         SNSPD_NTRON.add_port(port=route.ports[2], name="N1")
 
     def create_inductor2():
         ## INDUCTOR2
-        INDUCTOR2 = Device()
-        inductor2 = INDUCTOR2 << pg.snspd(
+        INDUCTOR2 = SNSPD_NTRON << device.snspd.basic(
             wire_width=w_inductor,
             wire_pitch=pitch_inductor,
             size=size_inductor2,
             num_squares=None,
             terminals_same_side=True,
             layer=layer,
         )
-        arcleft = INDUCTOR2 << pg.arc(radius=2 * w_inductor, width=w_inductor, theta=90)
-        arcright = INDUCTOR2 << pg.arc(
-            radius=2 * w_inductor, width=w_inductor, theta=90
-        )
-        arcleft.connect(arcleft.ports[2], inductor2.ports[1])
-        arcright.connect(arcright.ports[1], inductor2.ports[2])
-        INDUCTOR2.add_port(port=arcleft.ports[1])
-        INDUCTOR2.add_port(port=arcright.ports[2])
-        INDUCTOR2 = SNSPD_NTRON << INDUCTOR2
-        # port 1 connected to crossA east
-        INDUCTOR2.connect(INDUCTOR2.ports[1], CROSSA.ports["E"])
-        # port 2 connected to crossB west
-        route = SNSPD_NTRON << pg.compass((w_pad / 2, w_inductor))
-        route.connect(route.ports["W"], INDUCTOR2.ports[2])
+        arcleft = ROUTES << pg.arc(radius=2 * w_inductor, width=w_inductor, theta=90)
+        arcright = ROUTES << pg.arc(radius=2 * w_inductor, width=w_inductor, theta=90)
+        # connect arcleft to crossA east
+        arcleft.mirror()
+        arcleft.connect(arcleft.ports[2], CROSSA.ports["E"])
+        # connect INDUCTOR2 to arcleft
+        INDUCTOR2.connect(INDUCTOR2.ports[1], arcleft.ports[1])
+        # connect arcright to INDUCTOR2
+        arcright.connect(arcright.ports[1], INDUCTOR2.ports[2])
+        # arcright's port 2 connected to crossB west
+        route = ROUTES << pg.compass((w_pad / 2, w_inductor))
+        route.connect(route.ports["W"], arcright.ports[2])
         CROSSB.connect(CROSSB.ports["W"], route.ports["E"])
 
     def create_ntron():
         ## NTRON
-        NTRON = SNSPD_NTRON << qd.ntron.smooth(
+        NTRON = SNSPD_NTRON << device.ntron.smooth(
             choke_w=w_choke,
             gate_w=w_inductor,
             channel_w=w_channel,
             source_w=w_inductor,
             drain_w=w_inductor,
             choke_shift=-3 * w_channel,
             layer=layer,
         )
         # port 3 connected to crossB east
-        route = SNSPD_NTRON << pg.compass((w_pad / 2, w_inductor))
+        route = ROUTES << pg.compass((w_pad / 2, w_inductor))
         route.connect(route.ports["W"], CROSSB.ports["E"])
         NTRON.connect(NTRON.ports[3], route.ports["E"])
         # port 1 connected to crossC south
-        route = SNSPD_NTRON << pg.compass((w_inductor, w_pad / 2))
+        route = ROUTES << pg.compass((w_inductor, w_pad / 2))
         route.connect(route.ports["S"], NTRON.ports[1])
         CROSSC.connect(CROSSC.ports["S"], route.ports["N"])
         # port 2 connected to gnd
-        route = SNSPD_NTRON << pg.optimal_step(
-            NTRON.ports[2].width, w_pad, symmetric=True
-        )
+        route = ROUTES << pg.optimal_step(NTRON.ports[2].width, w_pad, symmetric=True)
         route.connect(route.ports[1], NTRON.ports[2])
         SNSPD_NTRON.add_port(port=route.ports[2], name="S2")
 
     def create_inductor3():
         ## INDUCTOR3
-        INDUCTOR3 = SNSPD_NTRON << pg.snspd(
+        INDUCTOR3 = SNSPD_NTRON << device.snspd.basic(
             wire_width=w_inductor,
             wire_pitch=pitch_inductor,
             size=size_inductor13,
             num_squares=None,
             terminals_same_side=False,
             layer=layer,
         )
         INDUCTOR3.rotate(90)
         # port 1 connected to crossC north
-        route = SNSPD_NTRON << pg.compass((w_inductor, w_pad / 2))
+        route = ROUTES << pg.compass((w_inductor, w_pad / 2))
         route.connect(route.ports["S"], CROSSC.ports["N"])
         INDUCTOR3.connect(INDUCTOR3.ports[1], route.ports["N"])
         # port 2 connected to pad
-        route = SNSPD_NTRON << pg.optimal_step(
+        route = ROUTES << pg.optimal_step(
             INDUCTOR3.ports[2].width, w_pad, symmetric=True
         )
         route.connect(route.ports[1], INDUCTOR3.ports[2])
         SNSPD_NTRON.add_port(port=route.ports[2], name="N3")
 
     def create_probing_routes():
         ## SNSPD PROBING PAD
-        step = SNSPD_NTRON << pg.optimal_step(w_inductor, w_pad, symmetric=True)
+        step = ROUTES << pg.optimal_step(w_inductor, w_pad, symmetric=True)
         step.connect(step.ports[1], CROSSA.ports["W"])
-        route = SNSPD_NTRON << pg.compass((abs(SNSPD_NTRON.xmin - step.xmin), w_pad))
+        route = ROUTES << pg.compass((abs(SNSPD_NTRON.xmin - step.xmin), w_pad))
         route.connect(route.ports["E"], step.ports[2])
         SNSPD_NTRON.add_port(port=route.ports["W"], name="W1")
 
         ## NTRON IN PROBING PAD
-        step = SNSPD_NTRON << pg.optimal_step(w_inductor, w_pad, symmetric=True)
+        step = ROUTES << pg.optimal_step(w_inductor, w_pad, symmetric=True)
         step.connect(step.ports[1], CROSSB.ports["N"])
-        route = SNSPD_NTRON << pg.compass((w_pad, abs(SNSPD_NTRON.ymax - step.ymax)))
+        route = ROUTES << pg.compass((w_pad, abs(SNSPD_NTRON.ymax - step.ymax)))
         route.connect(route.ports["S"], step.ports[2])
         SNSPD_NTRON.add_port(port=route.ports["N"], name="N2")
 
         ## NTRON OUT PROBING PAD
-        step = SNSPD_NTRON << pg.optimal_step(w_inductor, w_pad, symmetric=True)
+        step = ROUTES << pg.optimal_step(w_inductor, w_pad, symmetric=True)
         step.connect(step.ports[1], CROSSC.ports["E"])
-        route = SNSPD_NTRON << pg.compass((abs(SNSPD_NTRON.xmax - step.xmax), w_pad))
+        route = ROUTES << pg.compass((abs(SNSPD_NTRON.xmax - step.xmax), w_pad))
         route.connect(route.ports["W"], step.ports[2])
         SNSPD_NTRON.add_port(port=route.ports["E"], name="E1")
 
     SNSPD_NTRON = Device(f"SNSPD NTRON {w_snspd} {w_choke} ")
+    ROUTES = Device("ROUTES")
 
     size_inductor13, size_inductor2 = scale_inductors_to_snspd()
 
-    CROSSA = SNSPD_NTRON << crossA()
-    CROSSB = SNSPD_NTRON << crossB()
-    CROSSC = SNSPD_NTRON << crossC()
+    CROSSA = ROUTES << crossA()
+    CROSSB = ROUTES << crossB()
+    CROSSC = ROUTES << crossC()
 
     create_snspd()
     create_inductor1()
     create_inductor2()
     create_ntron()
     create_inductor3()
     create_probing_routes()
 
-    SNSPD_NTRON.flatten()
+    SNSPD_NTRON << ROUTES.flatten()
+    # SNSPD_NTRON.flatten()
 
-    ports = SNSPD_NTRON.get_ports()
-    SNSPD_NTRON = pg.union(SNSPD_NTRON, layer=layer)
-    for port in ports:
-        SNSPD_NTRON.add_port(port)
+    # ports = SNSPD_NTRON.get_ports()
+    # SNSPD_NTRON = pg.union(SNSPD_NTRON, layer=layer)
+    # for port in ports:
+    #     SNSPD_NTRON.add_port(port)
 
     SNSPD_NTRON.move(SNSPD_NTRON.center, (0, 0))
     SNSPD_NTRON.name = f"SNSPD NTRON {w_snspd} {w_choke} "
     return SNSPD_NTRON
```

### Comparing `qnngds-2.3.0/src/qnngds/design.py` & `qnngds-2.4.0/src/qnngds/design.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,16 +166,16 @@
                     f"Error, Device {cell_name} "
                     + f"falls out of the chip map ({coordinates[1]+m}, {coordinates[0]+n})"
                 )
                 return False
 
     # move the cell
     cell_bottom_left = (
-        -(n_cell - 1 + (n_cell % 2) * 0.5) * die_w,
-        -(m_cell - 1 + (m_cell % 2) * 0.5) * die_w,
+        -n_cell * 0.5 * die_w,
+        -m_cell * 0.5 * die_w,
     )
     cell.move(cell_bottom_left, ((coordinates[0]) * die_w, (coordinates[1]) * die_w))
 
     # write the cell's place on the devices map text file
     if devices_map_txt is not None:
         with open(f"{devices_map_txt}.txt", "a") as file:
             try:
@@ -498,26 +498,26 @@
                 If None, the name of the Design will be used.
 
         Returns:
             str or None: The filename of the written GDS file, or None if no file was written.
         """
         if text is None:
             text = self.name
-        return self.CHIP.write_gds(filename=f"{text}.gds")
+        return self.CHIP.write_gds(filename=f"{text}.gds", max_cellname_length=32000)
 
     # basics:
 
     def alignment_cell(
         self, layers_to_align: List[int], text: Union[None, str] = dflt.text
     ) -> Device:
         """Creates alignment marks in an integer number of unit cells.
 
         Parameters:
             layers_to_align (List[int]): Layers to align.
-            text (str): The text of the cell is f"ALIGN {text}".
+            text (str, optional): If None, the text is f"lay={layers_to_align}".
 
         Returns:
             Device: A device that centers the alignment marks in an n*m unit cell.
         """
         return cell.alignment(
             die_w=self.die_w,
             layers_to_align=layers_to_align,
@@ -534,15 +534,15 @@
     ) -> Device:
         r"""Creates a cell containing a Van Der Pauw structure between 4 contact
         pads.
 
         Parameters:
             layers_to_probe (List[int]): The layers on which to place the VDP structure.
             layers_to_outline (List[int]): Among the VDP layers, the ones for which structure must not be filled but outlined.
-            text (str, optional): If None, the text is f"VDP \n{layers_to_probe}". Otherwise, f"VDP \n{text}".
+            text (str, optional): If None, the text is f"lay={layers_to_probe}".
 
         Returns:
             Device: The created device.
         """
 
         return cell.vdp(
             die_w=self.die_w,
@@ -562,15 +562,15 @@
 
         These test structures are thought to be used by probing on pads (with a simple multimeter)
         that should be isolated one from another if the etching is complete.
 
         Parameters:
             layers_to_etch (List[List[int]]): Each element of the list corresponds to one test point,
                 to put on the list of layers specified. Example: [[1, 2], [1], [2]].
-            text (str, optional): If None, the cell text is f"ETCH TEST {layers_to_etch}".
+            text (str, optional): If None, the text is f"lay={layers_to_etch}".
 
         Returns:
             Device: A device (with size n*m of unit cells) with etch tests in its center.
         """
 
         return cell.etch_test(
             die_w=self.die_w,
@@ -597,15 +597,15 @@
         text: Union[None, str] = dflt.text,
     ) -> Device:
         r"""Creates a cell containing a resolution test.
 
         Parameters:
             layer_to_resolve (int): The layer to put the resolution test on.
             resolutions_to_test (List[float]): The resolutions to test in µm.
-            text (str, optional): If None, the text is f"RES TEST \n{layer_to_resolve}".
+            text (str, optional): If None, the text is f"lay={layer_to_resolve}".
 
         Returns:
             Device: The created device.
         """
 
         return cell.resolution_test(
             die_w=self.die_w,
@@ -625,15 +625,15 @@
     ) -> Device:
         """Creates a cell containing several nanowires of given channel and
         source.
 
         Parameters:
             channels_sources_w (List[Tuple[float, float]]): The list of
                 (channel_w, source_w) of the nanowires to create.
-            text (str, optional): If None, the text is "NWIRES".
+            text (str, optional): If None, the text is f"w={channels_w}".
 
         Returns:
             Device: A device containing the nanowires, the border of the die
             (created with die_cell function), and the connections between the
             nanowires and pads.
         """
 
@@ -670,15 +670,15 @@
         Parameters:
             choke_w (int or float): The width of the ntron's choke in µm.
             channel_w (int or float): The width of the ntron's channel in µm.
             gate_w (int or float, optional): If None, gate width is 3 times the channel width.
             source_w (int or float, optional): If None, source width is 3 times the channel width.
             drain_w (int or float, optional): If None, drain width is 3 times the channel width.
             choke_shift (int or float, optional): If None, choke shift is -3 times the channel width.
-            text (str, optional): If None, the text is f"chk: {choke_w} /n chnl: {channel_w}".
+            text (str, optional): If None, the text is f"chk: {choke_w} \\nchnl: {channel_w}".
 
         Returns:
             Device: A device containing the ntron, the border of the die (created with die_cell function),
             and the connections between the ports.
         """
 
         return cell.ntron(
@@ -712,27 +712,27 @@
         single-photon detector (SNSPD).
 
         Parameters:
             snspd_width (float): Width of the nanowire.
             snspd_pitch (float): Pitch of the nanowire.
             snspd_size (tuple of int or float): Size of the detector in squares (width, height).
             snspd_num_squares (Optional[int]): Number of squares in the detector.
-            text (string, optional): If None, text = f'SNSPD {w_choke}'.
+            text (string, optional): If None, the text is f"w={snspd_width}".
 
         Returns:
             Device: A cell (of size n*m unit die_cells) containing the SNSPD.
         """
 
         return cell.snspd(
             die_w=self.die_w,
             pad_size=self.pad_size,
             snspd_width=snspd_width,
             snspd_pitch=snspd_pitch,
-            size=snspd_size,
-            num_squares=snspd_num_squares,
+            snspd_size=snspd_size,
+            snspd_num_squares=snspd_num_squares,
             overlap_w=self.ebeam_overlap,
             outline_die=self.die_outline,
             outline_dev=self.device_outline,
             device_layer=self.layers["device"],
             die_layer=self.layers["die"],
             pad_layer=self.layers["pad"],
             text=text,
@@ -748,15 +748,15 @@
         """Creates a cell that contains an SNSPD coupled to an NTRON. The
         device's parameters are sized according to the SNSPD's width and the
         NTRON's choke.
 
         Parameters:
             w_choke (int or float): The width of the NTRON choke in µm.
             w_snspd (int or float, optional): The width of the SNSPD nanowire in µm. If None, scaled to 5*w_choke.
-            text (str, optional): If None, text = f'SNSPD {w_choke}'.
+            text (string, optional): If None, the text is f"w={w_snspd}, {w_choke}".
 
         Returns:
             Device: A cell containing a die in die_layer, pads in pad layer, and an SNSPD-NTRON properly routed in the device layer.
         """
 
         return cell.snspd_ntron(
             die_w=self.die_w,
```

### Comparing `qnngds-2.3.0/src/qnngds/devices/nanowire.py` & `qnngds-2.4.0/src/qnngds/devices/nanowire.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 """Single nanowire constriction."""
 
 from phidl import Device
 
 import phidl.geometry as pg
 from typing import Tuple, Optional
+import qnngds._default_param as dflt
 
 
 def spot(
-    channel_w: float = 0.1, source_w: float = 0.3, layer: int = 0, num_pts: int = 100
+    channel_w: float = 0.1,
+    source_w: float = 0.3,
+    layer: int = dflt.layers["device"],
+    num_pts: int = 100,
 ) -> Device:
-    """Creates a single wire, with the same appearance as an NTRON but without
-    the gate.
+    """Creates a single wire, made of two optimal steps from channel_w to
+    source_w.
 
     Args:
         channel_w (int or float): The width of the channel (at the hot-spot location).
         source_w (int or float): The width of the nanowire's "source".
         layer (int): The layer where to put the device.
         num_pts (int): The number of points comprising the optimal_steps geometries.
 
     Returns:
         Device: A device containing 2 optimal steps joined at their channel_w end.
     """
 
-    NANOWIRE = Device(f"NANOWIRE {channel_w} ")
+    NANOWIRE = Device()
     wire = pg.optimal_step(channel_w, source_w, symmetric=True, num_pts=num_pts)
     source = NANOWIRE << wire
     gnd = NANOWIRE << wire
     source.connect(source.ports[1], gnd.ports[1])
 
-    NANOWIRE.flatten(single_layer=layer)
+    NANOWIRE = pg.union(NANOWIRE, layer=layer)
     NANOWIRE.add_port(name=1, port=source.ports[2])
     NANOWIRE.add_port(name=2, port=gnd.ports[2])
     NANOWIRE.rotate(-90)
     NANOWIRE.move(NANOWIRE.center, (0, 0))
+    NANOWIRE.name = f"NANOWIRE.SPOT(w={channel_w})"
 
     return NANOWIRE
```

### Comparing `qnngds-2.3.0/src/qnngds/devices/ntron.py` & `qnngds-2.4.0/src/qnngds/devices/ntron.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Nanocryotron `[1] <https://doi.org/10.1021/nl502629x>`_ variants."""
 
 from phidl import Device
 
 import phidl.geometry as pg
 from typing import Tuple, Optional
+import qnngds._default_param as dflt
 
 
 def smooth(
     choke_w: float = 0.03,
     gate_w: float = 0.2,
     channel_w: float = 0.1,
     source_w: float = 0.3,
     drain_w: float = 0.3,
     choke_shift: float = -0.3,
-    layer: int = 0,
+    layer: int = dflt.layers["device"],
 ) -> Device:
     """Creates a ntron device.
 
     Args:
         choke_w (float): Width of the choke region.
         gate_w (float): Width of the gate region.
         channel_w (float): Width of the channel region.
@@ -50,83 +51,28 @@
     k.movey(choke_shift)
 
     D = pg.union(D)
     D.flatten(single_layer=layer)
     D.add_port(name=3, port=k.ports[1])
     D.add_port(name=1, port=d.ports[1])
     D.add_port(name=2, port=s.ports[2])
-    D.name = f"NTRON {choke_w} {channel_w} "
-    D.info = locals()
-
-    return D
-
-
-def smooth_compassPorts(
-    choke_w: float = 0.03,
-    gate_w: float = 0.2,
-    channel_w: float = 0.1,
-    source_w: float = 0.3,
-    drain_w: float = 0.3,
-    choke_shift: float = -0.3,
-    layer: int = 0,
-) -> Device:
-    """Creates a ntron device with compass ports (i.e. N1, W1, S1 for drain,
-    gate, source respectively).
-
-    Args:
-        choke_w (float): Width of the choke region.
-        gate_w (float): Width of the gate region.
-        channel_w (float): Width of the channel region.
-        source_w (float): Width of the source region.
-        drain_w (float): Width of the drain region.
-        choke_shift (float): Shift of the choke region.
-        layer (int): Layer for the device to be created on.
-
-    Returns:
-        Device: The ntron device.
-    """
-
-    D = Device()
-
-    choke = pg.optimal_step(gate_w, choke_w, symmetric=True, num_pts=100)
-    k = D << choke
-
-    channel = pg.compass(size=(channel_w, choke_w))
-    c = D << channel
-    c.connect(channel.ports["W"], choke.ports[2])
-
-    drain = pg.optimal_step(drain_w, channel_w)
-    d = D << drain
-    d.connect(drain.ports[2], c.ports["N"])
-
-    source = pg.optimal_step(channel_w, source_w)
-    s = D << source
-    s.connect(source.ports[1], c.ports["S"])
-
-    k.movey(choke_shift)
-
-    D = pg.union(D)
-    D.flatten(single_layer=layer)
-    D.add_port(name="N1", port=d.ports[1])
-    D.add_port(name="S1", port=s.ports[2])
-    D.add_port(name="W1", port=k.ports[1])
-    D.name = f"NTRON {choke_w} {channel_w} "
+    D.name = f"NTRON.SMOOTH(choke_w={choke_w}, channel_w={channel_w})"
     D.info = locals()
 
     return D
 
 
 def sharp(
     choke_w: float = 0.03,
     choke_l: float = 0.5,
     gate_w: float = 0.2,
     channel_w: float = 0.1,
     source_w: float = 0.3,
     drain_w: float = 0.3,
-    layer: int = 0,
+    layer: int = dflt.layers["device"],
 ) -> Device:
     """Creates a sharp ntron device.
 
     Args:
         choke_w (float): Width of the choke region.
         choke_l (float): Length of the choke region.
         gate_w (float): Width of the gate region.
@@ -135,15 +81,15 @@
         drain_w (float): Width of the drain region.
         layer (int): Layer for the device to be created on.
 
     Returns:
         Device: The sharp ntron device.
     """
 
-    D = Device("nTron")
+    D = Device()
 
     choke = pg.taper(choke_l, gate_w, choke_w)
     k = D << choke
 
     channel = pg.compass(size=(channel_w, choke_w / 10))
     c = D << channel
     c.connect(channel.ports["W"], choke.ports[2])
@@ -157,10 +103,10 @@
     s.connect(source.ports[1], c.ports["S"])
 
     D = pg.union(D)
     D.flatten(single_layer=layer)
     D.add_port(name="g", port=k.ports[1])
     D.add_port(name="d", port=d.ports[1])
     D.add_port(name="s", port=s.ports[2])
-    D.name = "nTron"
+    D.name = f"NTRON.SHARP(choke_w={choke_w}, channel_w={channel_w})"
     D.info = locals()
     return D
```

### Comparing `qnngds-2.3.0/src/qnngds/devices/resistor.py` & `qnngds-2.4.0/src/qnngds/devices/resistor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Layouts for resistors and resistors with superconducting contacts."""
 
 from phidl import Device
 
 import phidl.geometry as pg
 from typing import Tuple, Optional
+import qnngds._default_param as dflt
 
 
 def meander(
     width: float = 2,
     pitch: float = 4,
     squares: float = 100,
     max_length: float = 20,
     aspect_ratio: float = 1,
-    layer: int = 1,
+    layer: int = dflt.layers["device"],
 ) -> Device:
     """Create resistor meander with specified number of squares.
 
     If squares*width > max_length, meander the resistor, otherwise just return a straight line
 
     Args:
         width (float): width in microns
@@ -100,29 +101,31 @@
             stub_top.connect(stub_top.ports[1], hp_i.ports[2])
         hp_prev = hp_i
     stub_bot = D << stub(180 * (n_turn % 2))
     stub_bot.connect(stub_bot.ports[1], hp_prev.ports[2 - (n_turn % 2)])
     D = pg.union(D, by_layer=True, precision=0.01)
     D.add_port(name=1, port=stub_top.ports[2])
     D.add_port(name=2, port=stub_bot.ports[2])
+
+    D.name = f"RESISTOR.MEANDER (w={width}, pitch={pitch})"
     D.info = locals()
     return D
 
 
-def sc_contacts(
+def meander_sc_contacts(
     width: float = 1,
     squares: float = 60,
     max_length: float = 10,
     meander_pitch: float = 2,
     contact_width: float = 8,
     contact_height: float = 2,
     outline_sc: float = 1,
     width_routing: float = 1,
-    layer_res: int = 2,
-    layer_sc: int = 1,
+    layer_res: int = dflt.layers["pad"],
+    layer_sc: int = dflt.layers["device"],
 ) -> Device:
     """Create resistor meander with superconducting contacts.
 
     If squares*width > max_length, meander the resistor.
 
     Args:
         width (float): width of resistor
@@ -135,17 +138,21 @@
         width_routing (float): width of routing connections on superconducting layer
         layer_res (int): GDS layer for resistor
         layer_sc (int): GDS layer for superconductor
 
     Returns:
         D (Device): the resistor meander
     """
-    D = Device("resistor_negtone")
+    MEAN_SC_CONT = Device(
+        f"RESISTOR.MEANDER_SC_CONTACTS (w={width}, pitch={meander_pitch})"
+    )
+    CONTACTS = Device("CONTACTS")
+
     aspect_ratio = (contact_width + 2 * outline_sc) / max_length * 1.5
-    res = D << meander(
+    res = MEAN_SC_CONT << meander(
         layer=layer_res,
         width=width,
         pitch=max(meander_pitch, width + 1),
         squares=squares,
         max_length=max_length,
         aspect_ratio=aspect_ratio,
     )
@@ -154,21 +161,25 @@
     contact_sc = pg.straight(
         size=(contact_width + 2 * outline_sc, contact_height + 2 * outline_sc),
         layer=layer_sc,
     )
     rout = pg.straight(size=(width_routing, 2 * width_routing), layer=layer_sc)
     ports = []
     for p, port in res.ports.items():
-        s = D << stub
+        s = CONTACTS << stub
         s.connect(s.ports[1], port)
-        c = D << contact
+        c = CONTACTS << contact
         c.connect(c.ports[1], s.ports[2])
-        c_sc = D << contact_sc
+        c_sc = CONTACTS << contact_sc
         c_sc.center = c.center
-        r = D << rout
+        r = CONTACTS << rout
         r.connect(r.ports[1], c_sc.ports[2 - (p % 2)])
         ports.append(r.ports[2])
-    D = pg.union(D, by_layer=True)
-    D.add_port(port=ports[0], name=1)
-    D.add_port(port=ports[1], name=2)
-    D.info = locals()
-    return D
+
+    CONTACTS = pg.union(CONTACTS, by_layer=True)
+    CONTACTS.name = "CONTACTS"
+    MEAN_SC_CONT << CONTACTS
+
+    MEAN_SC_CONT.add_port(port=ports[0], name=1)
+    MEAN_SC_CONT.add_port(port=ports[1], name=2)
+    MEAN_SC_CONT.info = locals()
+    return MEAN_SC_CONT
```

### Comparing `qnngds-2.3.0/src/qnngds/geometries.py` & `qnngds-2.4.0/src/qnngds/geometries.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Geometries contains useful shapes/tools that are not available in phidl's
 geometry library."""
 
 from phidl import Device
 import numpy as np
+import qnngds._default_param as dflt
 
 
-def hyper_taper(length=10, wide_section=50, narrow_section=5, layer=0):
+def hyper_taper(
+    length=10, wide_section=50, narrow_section=5, layer=dflt.layers["device"]
+):
     """Hyperbolic taper (solid). Designed by colang.
 
     Args:
         length (float): Length of taper.
         wide_section (float): Wide width dimension.
         narrow_section (float): Narrow width dimension.
         layer (int): Layer for device to be created on.
```

### Comparing `qnngds-2.3.0/src/qnngds/tests.py` & `qnngds-2.4.0/src/qnngds/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests contains common test structures for following/characterizing a
 fabrication process and its effect on the materials."""
 
 from phidl import Device
 import phidl.geometry as pg
 from typing import List, Union
-import math
+import qnngds._default_param as dflt
 
 
 def alignment_mark(layers: List[int] = [1, 2, 3, 4]) -> Device:
     """Creates an alignment mark for each photolithography.
 
     Args:
         layers (List[int]): An array of layers.
@@ -19,18 +19,20 @@
 
     def create_marker(layer1, layer2):
 
         MARK = Device()
 
         # central part with cross
 
-        cross = MARK << pg.cross(length=190, width=20, layer=layer1)
+        CROSS = Device("CROSS")
+        cross = CROSS << pg.union(pg.cross(length=190, width=20), layer=layer1)
         rect = pg.rectangle((65, 65), layer=layer2)
-        window = MARK.add_array(rect, 2, 2, (125, 125))
+        window = CROSS.add_array(rect, 2, 2, (125, 125))
         window.move(window.center, cross.center)
+        MARK << CROSS.flatten()
 
         # combs
         def create_comb(pitch1=500, pitch2=100, layer1=1, layer2=2):
 
             COMB = Device()
 
             # middle comb (made of layer1), pitch = 10
@@ -61,65 +63,72 @@
 
             rect1b = pg.rectangle((5, 10), layer=layer1)
             marksb = COMB.add_array(rect1b, 2, 2, spacing=(100, 100))
             marksb.move(marksb.center, middle_comb.center)
 
             return COMB
 
+        VERNIER = Device("VERNIER(500, 200, 100, 50)")
         comb51 = create_comb(pitch1=500, pitch2=100, layer1=layer1, layer2=layer2)
 
-        top = MARK.add_ref(comb51)
+        top = VERNIER.add_ref(comb51)
         top.move((0, 0), (0, 200))
 
-        left = MARK.add_ref(comb51)
+        left = VERNIER.add_ref(comb51)
         left.rotate(90)
         left.move((0, 0), (-200, 0))
 
         comb205 = create_comb(pitch1=200, pitch2=50, layer1=layer1, layer2=layer2)
 
-        bottom = MARK.add_ref(comb205)
+        bottom = VERNIER.add_ref(comb205)
         bottom.rotate(180)
         bottom.move((0, 0), (0, -200))
 
-        right = MARK.add_ref(comb205)
+        right = VERNIER.add_ref(comb205)
         right.rotate(-90)
         right.move((0, 0), (200, 0))
+        MARK << VERNIER.flatten()
 
         MARK.move(MARK.center, (0, 0))
 
         # text
-        text1 = MARK << pg.text(str(layer2), size=50, layer={layer1, layer2})
+        TEXT = Device(f"TEXT({layer2} ON {layer1})")
+        text1 = TEXT << pg.text(str(layer2), size=50, layer={layer1, layer2})
         text1.move(text1.center, (220, 200))
-        text2 = MARK << pg.text(f"{layer2} ON {layer1}", size=10, layer=layer2)
+        text2 = TEXT << pg.text(f"{layer2} ON {layer1}", size=10, layer=layer2)
         text2.move(text2.center, (220, 240))
+        MARK << TEXT.flatten()
 
+        MARK.name = f"ALIGN {layer2} ON {layer1}"
         return MARK
 
     ALIGN = Device("ALIGN ")
     markers_pitch = 600
     for i, layer1 in enumerate(layers):
         n = len(layers) - i - 1
         if n != 0:
             for j, layer2 in enumerate(layers[-n:]):
                 MARK = create_marker(layer1, layer2)
                 MARK.move((j * markers_pitch, i * markers_pitch))
                 ALIGN << MARK
-            text = ALIGN << pg.text(str(layer1), size=160, layer=layer1)
+            text = pg.text(str(layer1), size=160, layer=layer1)
+            text.name = f"TEXT({str(layer1)})"
             text.move(text.center, (-340, i * markers_pitch))
+            ALIGN << text
 
     num_layers = len(layers)
     offset = -(num_layers - 2) * markers_pitch / 2
     ALIGN.move((0, 0), (offset, offset))
     return ALIGN
 
 
 def resolution_test(
     resolutions: List[float] = [0.8, 1, 1.2, 1.4, 1.6, 1.8, 2.0],
     inverted: Union[bool, float] = False,
-    layer: int = 0,
+    layer: int = dflt.layers["device"],
 ) -> Device:
     """Creates test structures for determining a process resolution.
 
     Args:
         resolutions (List[float]): List of resolutions (in µm) to be tested.
         inverted (Union[bool, float]): If True, invert the device. If float, outline the device by this width.
         layer (int): Layer to put the device on.
@@ -145,23 +154,26 @@
 
             L.align("all", "xmin")
             L.move((L.xmin, L.ymin), (0, 0))
             return L
 
         grid_spacing = (13 * res, 13 * res)
 
-        for i, percent in enumerate([0.8, 1, 1.2]):
+        space = [0.8, 1, 1.2]
+        for i, percent in enumerate(space):
             lll = LLL << create_L(percent * res, 2 * res)
             lll.move([i * space for space in grid_spacing])
 
         text = LLL << pg.text(str(res), size=20)
         text.move(
             text.get_bounding_box()[0], [(i + 1) * space for space in grid_spacing]
         )
 
+        LLL.flatten(single_layer=layer)
+        LLL.name = f"3L({space} x {res})"
         return LLL
 
     def create_waffle(res=1):
 
         WAFFLE = Device()
         W = pg.rectangle(size=(res * 80, res * 80))
 
@@ -180,53 +192,57 @@
         WAFFLE << W2
         text = WAFFLE << pg.text(str(res), size=20)
         text.move(
             (text.get_bounding_box()[0][0], text.get_bounding_box()[1][1]),
             (2 * res, -2 * res),
         )
 
+        WAFFLE.flatten(single_layer=layer)
+        WAFFLE.name = f"WAFFLE({res})"
         return WAFFLE
 
-    RES_TEST = Device("RESOLUTION TEST ")
-
     RES_TEST1 = pg.gridsweep(
         function=create_3L,
         param_x={"res": resolutions},
         param_y={},
         spacing=10,
         align_y="ymin",
+        label_layer=None,
     )
+    RES_TEST1.name = "3Ls"
     RES_TEST2 = pg.gridsweep(
         function=create_waffle,
         param_x={"res": resolutions},
         param_y={},
         spacing=10,
         align_y="ymax",
+        label_layer=None,
     )
-
-    RES_TEST << pg.grid(
-        device_list=[[RES_TEST1], [RES_TEST2]], spacing=20, align_x="xmin"
+    RES_TEST2.name = "WAFFLES"
+    RES_TEST = pg.grid(
+        device_list=[[RES_TEST1], [RES_TEST2]],
+        spacing=20,
+        align_x="xmin",
     )
 
     if inverted:
         if inverted == True:
             RES_TEST = pg.invert(RES_TEST, border=5, precision=0.0000001, layer=layer)
         else:
-            RES_TEST = pg.outline(RES_TEST, inverted)
+            RES_TEST = pg.outline(RES_TEST, inverted, layer=layer)
         res_test_name = "RESOLUTION TEST INVERTED "
     else:
         res_test_name = "RESOLUTION TEST "
 
-    RES_TEST = pg.union(RES_TEST, layer=layer)
     RES_TEST.move(RES_TEST.center, (0, 0))
     RES_TEST.name = res_test_name
     return RES_TEST
 
 
-def vdp(l: float = 400, w: float = 40, layer: int = 1) -> Device:
+def vdp(l: float = 400, w: float = 40, layer: int = dflt.layers["device"]) -> Device:
     """Creates a Van der Pauw (VDP) device with specified dimensions.
 
     Args:
         l (float): Length of the VDP device, overall maximum dimension, in µm.
         w (float): Width of the contact points (width of the ports), in µm.
         layer (int): Layer to put the device on.
```

### Comparing `qnngds-2.3.0/src/qnngds/utilities.py` & `qnngds-2.4.0/src/qnngds/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,16 @@
         elif port_name == "S":
             overlap_port.midpoint[1] += contact_l
         elif port_name == "W":
             overlap_port.midpoint[0] += contact_l
         elif port_name == "E":
             overlap_port.midpoint[0] += -contact_l
 
-    DIE = Device(f"DIE {text} ")
+    die_name = text.replace("\n", "")
+    DIE = Device(f"DIE {die_name} ")
 
     border = pg.rectangle(die_size)
     border.move(border.center, (0, 0))
 
     borderOut = Device()
 
     ## Make the routes and pads
@@ -187,15 +188,15 @@
         PADS.remove_layers([layer])
         PADS.name = "pads"
         DIE = pg.invert(DIE, border=0, layer=layer)
         DIE << PADS
     for port in ports:
         DIE.add_port(port)
 
-    DIE.name = f"DIE {text}"
+    DIE.name = f"DIE {die_name}"
     return DIE
 
 
 def calculate_available_space_for_dev(
     die_size: Tuple[Union[int, float], Union[int, float]] = (dflt.die_w, dflt.die_w),
     pad_size: Tuple[Union[int, float], Union[int, float]] = dflt.pad_size,
     contact_l: Union[int, float] = dflt.ebeam_overlap,
```

### Comparing `qnngds-2.3.0/PKG-INFO` & `qnngds-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnngds
-Version: 2.3.0
+Version: 2.4.0
 Summary: The QNN library for creating gds files
 Keywords: phidl,nanowire_electronics,nanofabrication,gds
 Author-Email: "A. Jacquillat" <audrey01@mit.edu>, "A. Jacquillat" <audrey.jacquillat@gmail.com>, "R. Foster" <reedf@mit.edu>
 Maintainer-Email: "A. Jacquillat" <audrey01@mit.edu>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

