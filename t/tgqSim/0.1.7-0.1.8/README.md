# Comparing `tmp/tgqSim-0.1.7.tar.gz` & `tmp/tgqSim-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgqSim-0.1.7.tar", last modified: Tue May 14 03:32:09 2024, max compression
+gzip compressed data, was "tgqSim-0.1.8.tar", last modified: Tue May 14 05:41:47 2024, max compression
```

## Comparing `tgqSim-0.1.7.tar` & `tgqSim-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 03:32:09.865350 tgqSim-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-14 03:32:07.000000 tgqSim-0.1.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-14 03:32:07.000000 tgqSim-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2024-05-14 03:32:09.865350 tgqSim-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-14 03:32:07.000000 tgqSim-0.1.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 03:32:09.865350 tgqSim-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-14 03:32:08.000000 tgqSim-0.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 03:32:09.864350 tgqSim-0.1.7/tgqSim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 03:32:09.864350 tgqSim-0.1.7/tgqSim/GateSimulation/
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/GateSimulation/DoubleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/GateSimulation/SingleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/GateSimulation/TripleGate.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/GateSimulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22122 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/QuantumCircuit.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-14 03:32:08.000000 tgqSim-0.1.7/tgqSim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/draw_circuit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 03:32:09.865350 tgqSim-0.1.7/tgqSim/lib/
--rw-rw-rw-   0 root         (0) root         (0)    61896 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/lib/cuda_11-8_tgq_simulator.so
--rw-rw-rw-   0 root         (0) root         (0)    73456 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/lib/cuda_12-4_tgq_simulator.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 03:32:09.864350 tgqSim-0.1.7/tgqSim.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2024-05-14 03:32:09.000000 tgqSim-0.1.7/tgqSim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-14 03:32:09.000000 tgqSim-0.1.7/tgqSim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 03:32:09.000000 tgqSim-0.1.7/tgqSim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-14 03:32:09.000000 tgqSim-0.1.7/tgqSim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-14 03:32:09.000000 tgqSim-0.1.7/tgqSim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:41:47.874247 tgqSim-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-14 05:41:46.000000 tgqSim-0.1.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-14 05:41:46.000000 tgqSim-0.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2024-05-14 05:41:47.873247 tgqSim-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-14 05:41:46.000000 tgqSim-0.1.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 05:41:47.874247 tgqSim-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-14 05:41:46.000000 tgqSim-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:41:47.872247 tgqSim-0.1.8/tgqSim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:41:47.873247 tgqSim-0.1.8/tgqSim/GateSimulation/
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/GateSimulation/DoubleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/GateSimulation/SingleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/GateSimulation/TripleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/GateSimulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22122 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/QuantumCircuit.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/draw_circuit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:41:47.873247 tgqSim-0.1.8/tgqSim/lib/
+-rw-rw-rw-   0 root         (0) root         (0)    61952 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/lib/cuda_11-8_tgq_simulator.so
+-rw-rw-rw-   0 root         (0) root         (0)    73456 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/lib/cuda_12-4_tgq_simulator.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:41:47.872247 tgqSim-0.1.8/tgqSim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2024-05-14 05:41:47.000000 tgqSim-0.1.8/tgqSim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-14 05:41:47.000000 tgqSim-0.1.8/tgqSim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 05:41:47.000000 tgqSim-0.1.8/tgqSim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-14 05:41:47.000000 tgqSim-0.1.8/tgqSim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-14 05:41:47.000000 tgqSim-0.1.8/tgqSim.egg-info/top_level.txt
```

### Comparing `tgqSim-0.1.7/LICENSE` & `tgqSim-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.7/PKG-INFO` & `tgqSim-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.7
+Version: 0.1.8
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `tgqSim-0.1.7/setup.py` & `tgqSim-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tgqSim',
-    version='0.1.7',
+    version='0.1.8',
     description='TGQ量子模拟器',  # 包描述
     long_description="Python for quantum simulation http://www.tiangongqs.com",  # 详细描述
     long_description_content_type='text/markdown',
     author='tiangongqs',  # 作者姓名
     license='MIT',  # 许可证
     package=find_packages(),
     include_package_data=True,
```

### Comparing `tgqSim-0.1.7/tgqSim/GateSimulation/DoubleGate.py` & `tgqSim-0.1.8/tgqSim/GateSimulation/DoubleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.7/tgqSim/GateSimulation/SingleGate.py` & `tgqSim-0.1.8/tgqSim/GateSimulation/SingleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.7/tgqSim/GateSimulation/TripleGate.py` & `tgqSim-0.1.8/tgqSim/GateSimulation/TripleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.7/tgqSim/QuantumCircuit.py` & `tgqSim-0.1.8/tgqSim/QuantumCircuit.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.7/tgqSim/draw_circuit_tools.py` & `tgqSim-0.1.8/tgqSim/draw_circuit_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.7/tgqSim/lib/cuda_11-8_tgq_simulator.so` & `tgqSim-0.1.8/tgqSim/lib/cuda_11-8_tgq_simulator.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 4% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -4,17 +4,17 @@
   Data:                              2's complement, little endian
   Version:                           1 (current)
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
-  Entry point address:               0x2830
+  Entry point address:               0x2850
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          59848 (bytes into file)
+  Start of section headers:          59904 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         11
   Size of section headers:           64 (bytes)
   Number of section headers:         32
   Section header string table index: 31
```

#### readelf --wide --program-header {}

```diff
@@ -1,23 +1,23 @@
 
 Elf file type is DYN (Shared object file)
-Entry point 0x2830
+Entry point 0x2850
 There are 11 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x001b18 0x001b18 R   0x1000
-  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x0034b1 0x0034b1 R E 0x1000
-  LOAD           0x006000 0x0000000000006000 0x0000000000006000 0x006af0 0x006af0 R   0x1000
-  LOAD           0x00cdb0 0x000000000000ddb0 0x000000000000ddb0 0x000478 0x000488 RW  0x1000
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x001b78 0x001b78 R   0x1000
+  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x003501 0x003501 R E 0x1000
+  LOAD           0x006000 0x0000000000006000 0x0000000000006000 0x006b20 0x006b20 R   0x1000
+  LOAD           0x00cdb0 0x000000000000ddb0 0x000000000000ddb0 0x000480 0x000490 RW  0x1000
   DYNAMIC        0x00cdc8 0x000000000000ddc8 0x000000000000ddc8 0x0001e0 0x0001e0 RW  0x8
   NOTE           0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
   NOTE           0x0002c8 0x00000000000002c8 0x00000000000002c8 0x000024 0x000024 R   0x4
   GNU_PROPERTY   0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
-  GNU_EH_FRAME   0x00c2c0 0x000000000000c2c0 0x000000000000c2c0 0x0001bc 0x0001bc R   0x4
+  GNU_EH_FRAME   0x00c2f0 0x000000000000c2f0 0x000000000000c2f0 0x0001bc 0x0001bc R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
   GNU_RELRO      0x00cdb0 0x000000000000ddb0 0x000000000000ddb0 0x000250 0x000250 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     .note.gnu.property .note.gnu.build-id .gnu.hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt 
    01     .init .plt .plt.got .plt.sec .text .fini
```

#### readelf --wide --sections {}

```diff
@@ -1,41 +1,41 @@
-There are 32 section headers, starting at offset 0xe9c8:
+There are 32 section headers, starting at offset 0xea00:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .note.gnu.property NOTE            00000000000002a8 0002a8 000020 00   A  0   0  8
   [ 2] .note.gnu.build-id NOTE            00000000000002c8 0002c8 000024 00   A  0   0  4
   [ 3] .gnu.hash         GNU_HASH        00000000000002f0 0002f0 0001a4 00   A  4   0  8
-  [ 4] .dynsym           DYNSYM          0000000000000498 000498 000750 18   A  5   1  8
-  [ 5] .dynstr           STRTAB          0000000000000be8 000be8 0006d2 00   A  0   0  1
-  [ 6] .gnu.version      VERSYM          00000000000012ba 0012ba 00009c 02   A  4   0  2
-  [ 7] .gnu.version_r    VERNEED         0000000000001358 001358 000070 00   A  5   3  8
-  [ 8] .rela.dyn         RELA            00000000000013c8 0013c8 000180 18   A  4   0  8
-  [ 9] .rela.plt         RELA            0000000000001548 001548 0005d0 18  AI  4  24  8
+  [ 4] .dynsym           DYNSYM          0000000000000498 000498 000768 18   A  5   1  8
+  [ 5] .dynstr           STRTAB          0000000000000c00 000c00 0006eb 00   A  0   0  1
+  [ 6] .gnu.version      VERSYM          00000000000012ec 0012ec 00009e 02   A  4   0  2
+  [ 7] .gnu.version_r    VERNEED         0000000000001390 001390 000080 00   A  5   3  8
+  [ 8] .rela.dyn         RELA            0000000000001410 001410 000180 18   A  4   0  8
+  [ 9] .rela.plt         RELA            0000000000001590 001590 0005e8 18  AI  4  24  8
   [10] .init             PROGBITS        0000000000002000 002000 00001b 00  AX  0   0  4
-  [11] .plt              PROGBITS        0000000000002020 002020 0003f0 10  AX  0   0 16
-  [12] .plt.got          PROGBITS        0000000000002410 002410 000040 10  AX  0   0 16
-  [13] .plt.sec          PROGBITS        0000000000002450 002450 0003e0 10  AX  0   0 16
-  [14] .text             PROGBITS        0000000000002830 002830 002c72 00  AX  0   0 16
-  [15] .fini             PROGBITS        00000000000054a4 0054a4 00000d 00  AX  0   0  4
-  [16] .rodata           PROGBITS        0000000000006000 006000 000300 00   A  0   0 16
-  [17] .nv_fatbin        PROGBITS        0000000000006300 006300 005fc0 00   A  0   0  8
-  [18] .eh_frame_hdr     PROGBITS        000000000000c2c0 00c2c0 0001bc 00   A  0   0  4
-  [19] .eh_frame         PROGBITS        000000000000c480 00c480 000670 00   A  0   0  8
+  [11] .plt              PROGBITS        0000000000002020 002020 000400 10  AX  0   0 16
+  [12] .plt.got          PROGBITS        0000000000002420 002420 000040 10  AX  0   0 16
+  [13] .plt.sec          PROGBITS        0000000000002460 002460 0003f0 10  AX  0   0 16
+  [14] .text             PROGBITS        0000000000002850 002850 002ca2 00  AX  0   0 16
+  [15] .fini             PROGBITS        00000000000054f4 0054f4 00000d 00  AX  0   0  4
+  [16] .rodata           PROGBITS        0000000000006000 006000 000330 00   A  0   0 16
+  [17] .nv_fatbin        PROGBITS        0000000000006330 006330 005fc0 00   A  0   0  8
+  [18] .eh_frame_hdr     PROGBITS        000000000000c2f0 00c2f0 0001bc 00   A  0   0  4
+  [19] .eh_frame         PROGBITS        000000000000c4b0 00c4b0 000670 00   A  0   0  8
   [20] .init_array       INIT_ARRAY      000000000000ddb0 00cdb0 000010 08  WA  0   0  8
   [21] .fini_array       FINI_ARRAY      000000000000ddc0 00cdc0 000008 08  WA  0   0  8
   [22] .dynamic          DYNAMIC         000000000000ddc8 00cdc8 0001e0 10  WA  5   0  8
   [23] .got              PROGBITS        000000000000dfa8 00cfa8 000058 08  WA  0   0  8
-  [24] .got.plt          PROGBITS        000000000000e000 00d000 000208 08  WA  0   0  8
-  [25] .data             PROGBITS        000000000000e208 00d208 000008 00  WA  0   0  8
-  [26] .nvFatBinSegment  PROGBITS        000000000000e210 00d210 000018 00  WA  0   0  8
-  [27] .bss              NOBITS          000000000000e228 00d228 000010 00  WA  0   0  8
-  [28] .comment          PROGBITS        0000000000000000 00d228 00002b 01  MS  0   0  1
-  [29] .symtab           SYMTAB          0000000000000000 00d258 000c78 18     30  56  8
-  [30] .strtab           STRTAB          0000000000000000 00ded0 0009cd 00      0   0  1
-  [31] .shstrtab         STRTAB          0000000000000000 00e89d 000129 00      0   0  1
+  [24] .got.plt          PROGBITS        000000000000e000 00d000 000210 08  WA  0   0  8
+  [25] .data             PROGBITS        000000000000e210 00d210 000008 00  WA  0   0  8
+  [26] .nvFatBinSegment  PROGBITS        000000000000e218 00d218 000018 00  WA  0   0  8
+  [27] .bss              NOBITS          000000000000e230 00d230 000010 00  WA  0   0  8
+  [28] .comment          PROGBITS        0000000000000000 00d230 00002b 01  MS  0   0  1
+  [29] .symtab           SYMTAB          0000000000000000 00d260 000c90 18     30  56  8
+  [30] .strtab           STRTAB          0000000000000000 00def0 0009e7 00      0   0  1
+  [31] .shstrtab         STRTAB          0000000000000000 00e8d7 000129 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -1,9 +1,9 @@
 
-Symbol table '.dynsym' contains 78 entries:
+Symbol table '.dynsym' contains 79 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sincosf@GLIBC_2.2.5 (2)
      2: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5 (3)
      3: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaUnregisterFatBinary@libcudart.so.11.0 (4)
      4: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
      5: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinary@libcudart.so.11.0 (4)
@@ -18,200 +18,202 @@
     14: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaDeviceSynchronize@libcudart.so.11.0 (4)
     15: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
     16: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND time@GLIBC_2.2.5 (3)
     17: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sqrtf@GLIBC_2.2.5 (2)
     18: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5 (3)
     19: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMalloc@libcudart.so.11.0 (4)
     20: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaLaunchKernel@libcudart.so.11.0 (4)
-    21: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaSetDevice@libcudart.so.11.0 (4)
-    22: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@GLIBC_2.2.5 (3)
-    23: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@GLIBC_2.2.5 (3)
-    24: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-    25: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPushCallConfiguration@libcudart.so.11.0 (4)
-    26: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinaryEnd@libcudart.so.11.0 (4)
-    27: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (3)
-    28: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND rand@GLIBC_2.2.5 (3)
-    29: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPopCallConfiguration@libcudart.so.11.0 (4)
-    30: 0000000000003d00    82 FUNC    GLOBAL DEFAULT   14 _Z9isInArrayPPKcPci
-    31: 0000000000004930   251 FUNC    GLOBAL DEFAULT   14 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm
-    32: 0000000000002d80    55 FUNC    GLOBAL DEFAULT   14 _Z9swap_gateP6float2
-    33: 0000000000002e10   109 FUNC    GLOBAL DEFAULT   14 _Z11cphase_gateP6float2f
-    34: 0000000000003930   418 FUNC    GLOBAL DEFAULT   14 _Z23fred_gate_control_smallP6float2
-    35: 0000000000002f00    62 FUNC    GLOBAL DEFAULT   14 _Z7cz_gateP6float2
-    36: 0000000000002a10    27 FUNC    GLOBAL DEFAULT   14 _Z6z_gateP6float2
-    37: 0000000000003280   404 FUNC    GLOBAL DEFAULT   14 _Z20toff_gate_target_midP6float2
-    38: 0000000000005030  1110 FUNC    GLOBAL DEFAULT   14 tripleGateAction
-    39: 0000000000003ba0   294 FUNC    GLOBAL DEFAULT   14 _Z7getprobP6float2Pfm
-    40: 0000000000002dc0    69 FUNC    GLOBAL DEFAULT   14 _Z10iswap_gateP6float2
-    41: 0000000000004370     9 FUNC    GLOBAL DEFAULT   14 _Z19actionOnSingleQubitP6float2S0_mPm
-    42: 0000000000004380  1444 FUNC    GLOBAL DEFAULT   14 singleGateAction
-    43: 0000000000002a50    27 FUNC    GLOBAL DEFAULT   14 _Z8sdg_gateP6float2
-    44: 0000000000004a40  1243 FUNC    GLOBAL DEFAULT   14 doubleGateAction
-    45: 0000000000002d10   102 FUNC    GLOBAL DEFAULT   14 _Z7ad_gateP6float2f
-    46: 0000000000002ca0   105 FUNC    GLOBAL DEFAULT   14 _Z7pd_gateP6float2f
-    47: 0000000000003d90   526 FUNC    GLOBAL DEFAULT   14 _Z13normalizationP6float2i
-    48: 0000000000002ad0   101 FUNC    GLOBAL DEFAULT   14 _Z7rx_gateP6float2f
-    49: 00000000000030e0   198 FUNC    GLOBAL DEFAULT   14 _Z8rzz_gateP6float2f
-    50: 0000000000003d60    33 FUNC    GLOBAL DEFAULT   14 _Z14getArrayLengthPi
-    51: 0000000000003780   418 FUNC    GLOBAL DEFAULT   14 _Z21fred_gate_control_midP6float2
-    52: 0000000000003b50    69 FUNC    GLOBAL DEFAULT   14 _Z20generate_binary_dataf
-    53: 0000000000002a90    27 FUNC    GLOBAL DEFAULT   14 _Z8tdg_gateP6float2
-    54: 0000000000005020     9 FUNC    GLOBAL DEFAULT   14 _Z18actionOnTripleGateP6float2S0_mPm
-    55: 0000000000002ab0    26 FUNC    GLOBAL DEFAULT   14 _Z6h_gateP6float2
-    56: 0000000000002bb0    98 FUNC    GLOBAL DEFAULT   14 _Z7rz_gateP6float2f
-    57: 0000000000003420   418 FUNC    GLOBAL DEFAULT   14 _Z20toff_gate_target_bigP6float2
-    58: 0000000000002e80    55 FUNC    GLOBAL DEFAULT   14 _Z21cnot_gate_control_bigP6float2
-    59: 0000000000003200   115 FUNC    GLOBAL DEFAULT   14 _Z22toff_gate_target_smallP6float2
-    60: 0000000000003010   204 FUNC    GLOBAL DEFAULT   14 _Z8ryy_gateP6float2f
-    61: 0000000000003cd0    47 FUNC    GLOBAL DEFAULT   14 _Z4hashPKc
-    62: 00000000000029b0     9 FUNC    GLOBAL DEFAULT   14 _Z7comparePKvS0_
-    63: 00000000000031b0    69 FUNC    GLOBAL DEFAULT   14 _Z8syc_gateP6float2
-    64: 0000000000003fa0   707 FUNC    GLOBAL DEFAULT   14 execute_circuit
-    65: 0000000000003ae0   105 FUNC    GLOBAL DEFAULT   14 _Z11identityMatP6float2i
-    66: 00000000000035d0   418 FUNC    GLOBAL DEFAULT   14 _Z21fred_gate_control_bigP6float2
-    67: 0000000000002a30    27 FUNC    GLOBAL DEFAULT   14 _Z6s_gateP6float2
-    68: 0000000000004f20   251 FUNC    GLOBAL DEFAULT   14 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
-    69: 0000000000002b40   110 FUNC    GLOBAL DEFAULT   14 _Z7ry_gateP6float2f
-    70: 00000000000029d0    27 FUNC    GLOBAL DEFAULT   14 _Z6x_gateP6float2
-    71: 0000000000002a70    27 FUNC    GLOBAL DEFAULT   14 _Z6t_gateP6float2
-    72: 0000000000002ec0    55 FUNC    GLOBAL DEFAULT   14 _Z23cnot_gate_control_smallP6float2
-    73: 0000000000002f40   201 FUNC    GLOBAL DEFAULT   14 _Z8rxx_gateP6float2f
-    74: 0000000000004a30     9 FUNC    GLOBAL DEFAULT   14 _Z19actionOnDoubleQubitP6float2S0_mPm
-    75: 00000000000029f0    26 FUNC    GLOBAL DEFAULT   14 _Z6y_gateP6float2
-    76: 0000000000004270   251 FUNC    GLOBAL DEFAULT   14 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
-    77: 0000000000002c20   116 FUNC    GLOBAL DEFAULT   14 _Z11damp_i_gateP6float2f
+    21: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __printf_chk@GLIBC_2.3.4 (6)
+    22: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaSetDevice@libcudart.so.11.0 (4)
+    23: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@GLIBC_2.2.5 (3)
+    24: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@GLIBC_2.2.5 (3)
+    25: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+    26: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPushCallConfiguration@libcudart.so.11.0 (4)
+    27: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinaryEnd@libcudart.so.11.0 (4)
+    28: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (3)
+    29: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND rand@GLIBC_2.2.5 (3)
+    30: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPopCallConfiguration@libcudart.so.11.0 (4)
+    31: 0000000000003d20    82 FUNC    GLOBAL DEFAULT   14 _Z9isInArrayPPKcPci
+    32: 0000000000004960   251 FUNC    GLOBAL DEFAULT   14 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm
+    33: 0000000000002da0    55 FUNC    GLOBAL DEFAULT   14 _Z9swap_gateP6float2
+    34: 0000000000002e30   109 FUNC    GLOBAL DEFAULT   14 _Z11cphase_gateP6float2f
+    35: 0000000000003950   418 FUNC    GLOBAL DEFAULT   14 _Z23fred_gate_control_smallP6float2
+    36: 0000000000002f20    62 FUNC    GLOBAL DEFAULT   14 _Z7cz_gateP6float2
+    37: 0000000000002a30    27 FUNC    GLOBAL DEFAULT   14 _Z6z_gateP6float2
+    38: 00000000000032a0   404 FUNC    GLOBAL DEFAULT   14 _Z20toff_gate_target_midP6float2
+    39: 0000000000005080  1110 FUNC    GLOBAL DEFAULT   14 tripleGateAction
+    40: 0000000000003bc0   294 FUNC    GLOBAL DEFAULT   14 _Z7getprobP6float2Pfm
+    41: 0000000000002de0    69 FUNC    GLOBAL DEFAULT   14 _Z10iswap_gateP6float2
+    42: 00000000000043a0     9 FUNC    GLOBAL DEFAULT   14 _Z19actionOnSingleQubitP6float2S0_mPm
+    43: 00000000000043b0  1444 FUNC    GLOBAL DEFAULT   14 singleGateAction
+    44: 0000000000002a70    27 FUNC    GLOBAL DEFAULT   14 _Z8sdg_gateP6float2
+    45: 0000000000004a70  1269 FUNC    GLOBAL DEFAULT   14 doubleGateAction
+    46: 0000000000002d30   102 FUNC    GLOBAL DEFAULT   14 _Z7ad_gateP6float2f
+    47: 0000000000002cc0   105 FUNC    GLOBAL DEFAULT   14 _Z7pd_gateP6float2f
+    48: 0000000000003db0   526 FUNC    GLOBAL DEFAULT   14 _Z13normalizationP6float2i
+    49: 0000000000002af0   101 FUNC    GLOBAL DEFAULT   14 _Z7rx_gateP6float2f
+    50: 0000000000003100   198 FUNC    GLOBAL DEFAULT   14 _Z8rzz_gateP6float2f
+    51: 0000000000003d80    33 FUNC    GLOBAL DEFAULT   14 _Z14getArrayLengthPi
+    52: 00000000000037a0   418 FUNC    GLOBAL DEFAULT   14 _Z21fred_gate_control_midP6float2
+    53: 0000000000003b70    69 FUNC    GLOBAL DEFAULT   14 _Z20generate_binary_dataf
+    54: 0000000000002ab0    27 FUNC    GLOBAL DEFAULT   14 _Z8tdg_gateP6float2
+    55: 0000000000005070     9 FUNC    GLOBAL DEFAULT   14 _Z18actionOnTripleGateP6float2S0_mPm
+    56: 0000000000002ad0    26 FUNC    GLOBAL DEFAULT   14 _Z6h_gateP6float2
+    57: 0000000000002bd0    98 FUNC    GLOBAL DEFAULT   14 _Z7rz_gateP6float2f
+    58: 0000000000003440   418 FUNC    GLOBAL DEFAULT   14 _Z20toff_gate_target_bigP6float2
+    59: 0000000000002ea0    55 FUNC    GLOBAL DEFAULT   14 _Z21cnot_gate_control_bigP6float2
+    60: 0000000000003220   115 FUNC    GLOBAL DEFAULT   14 _Z22toff_gate_target_smallP6float2
+    61: 0000000000003030   204 FUNC    GLOBAL DEFAULT   14 _Z8ryy_gateP6float2f
+    62: 0000000000003cf0    47 FUNC    GLOBAL DEFAULT   14 _Z4hashPKc
+    63: 00000000000029d0     9 FUNC    GLOBAL DEFAULT   14 _Z7comparePKvS0_
+    64: 00000000000031d0    69 FUNC    GLOBAL DEFAULT   14 _Z8syc_gateP6float2
+    65: 0000000000003fc0   731 FUNC    GLOBAL DEFAULT   14 execute_circuit
+    66: 0000000000003b00   105 FUNC    GLOBAL DEFAULT   14 _Z11identityMatP6float2i
+    67: 00000000000035f0   418 FUNC    GLOBAL DEFAULT   14 _Z21fred_gate_control_bigP6float2
+    68: 0000000000002a50    27 FUNC    GLOBAL DEFAULT   14 _Z6s_gateP6float2
+    69: 0000000000004f70   251 FUNC    GLOBAL DEFAULT   14 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
+    70: 0000000000002b60   110 FUNC    GLOBAL DEFAULT   14 _Z7ry_gateP6float2f
+    71: 00000000000029f0    27 FUNC    GLOBAL DEFAULT   14 _Z6x_gateP6float2
+    72: 0000000000002a90    27 FUNC    GLOBAL DEFAULT   14 _Z6t_gateP6float2
+    73: 0000000000002ee0    55 FUNC    GLOBAL DEFAULT   14 _Z23cnot_gate_control_smallP6float2
+    74: 0000000000002f60   201 FUNC    GLOBAL DEFAULT   14 _Z8rxx_gateP6float2f
+    75: 0000000000004a60     9 FUNC    GLOBAL DEFAULT   14 _Z19actionOnDoubleQubitP6float2S0_mPm
+    76: 0000000000002a10    26 FUNC    GLOBAL DEFAULT   14 _Z6y_gateP6float2
+    77: 00000000000042a0   251 FUNC    GLOBAL DEFAULT   14 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
+    78: 0000000000002c40   116 FUNC    GLOBAL DEFAULT   14 _Z11damp_i_gateP6float2f
 
-Symbol table '.symtab' contains 133 entries:
+Symbol table '.symtab' contains 134 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 00000000000002a8     0 SECTION LOCAL  DEFAULT    1 .note.gnu.property
      2: 00000000000002c8     0 SECTION LOCAL  DEFAULT    2 .note.gnu.build-id
      3: 00000000000002f0     0 SECTION LOCAL  DEFAULT    3 .gnu.hash
      4: 0000000000000498     0 SECTION LOCAL  DEFAULT    4 .dynsym
-     5: 0000000000000be8     0 SECTION LOCAL  DEFAULT    5 .dynstr
-     6: 00000000000012ba     0 SECTION LOCAL  DEFAULT    6 .gnu.version
-     7: 0000000000001358     0 SECTION LOCAL  DEFAULT    7 .gnu.version_r
-     8: 00000000000013c8     0 SECTION LOCAL  DEFAULT    8 .rela.dyn
-     9: 0000000000001548     0 SECTION LOCAL  DEFAULT    9 .rela.plt
+     5: 0000000000000c00     0 SECTION LOCAL  DEFAULT    5 .dynstr
+     6: 00000000000012ec     0 SECTION LOCAL  DEFAULT    6 .gnu.version
+     7: 0000000000001390     0 SECTION LOCAL  DEFAULT    7 .gnu.version_r
+     8: 0000000000001410     0 SECTION LOCAL  DEFAULT    8 .rela.dyn
+     9: 0000000000001590     0 SECTION LOCAL  DEFAULT    9 .rela.plt
     10: 0000000000002000     0 SECTION LOCAL  DEFAULT   10 .init
     11: 0000000000002020     0 SECTION LOCAL  DEFAULT   11 .plt
-    12: 0000000000002410     0 SECTION LOCAL  DEFAULT   12 .plt.got
-    13: 0000000000002450     0 SECTION LOCAL  DEFAULT   13 .plt.sec
-    14: 0000000000002830     0 SECTION LOCAL  DEFAULT   14 .text
-    15: 00000000000054a4     0 SECTION LOCAL  DEFAULT   15 .fini
+    12: 0000000000002420     0 SECTION LOCAL  DEFAULT   12 .plt.got
+    13: 0000000000002460     0 SECTION LOCAL  DEFAULT   13 .plt.sec
+    14: 0000000000002850     0 SECTION LOCAL  DEFAULT   14 .text
+    15: 00000000000054f4     0 SECTION LOCAL  DEFAULT   15 .fini
     16: 0000000000006000     0 SECTION LOCAL  DEFAULT   16 .rodata
-    17: 0000000000006300     0 SECTION LOCAL  DEFAULT   17 .nv_fatbin
-    18: 000000000000c2c0     0 SECTION LOCAL  DEFAULT   18 .eh_frame_hdr
-    19: 000000000000c480     0 SECTION LOCAL  DEFAULT   19 .eh_frame
+    17: 0000000000006330     0 SECTION LOCAL  DEFAULT   17 .nv_fatbin
+    18: 000000000000c2f0     0 SECTION LOCAL  DEFAULT   18 .eh_frame_hdr
+    19: 000000000000c4b0     0 SECTION LOCAL  DEFAULT   19 .eh_frame
     20: 000000000000ddb0     0 SECTION LOCAL  DEFAULT   20 .init_array
     21: 000000000000ddc0     0 SECTION LOCAL  DEFAULT   21 .fini_array
     22: 000000000000ddc8     0 SECTION LOCAL  DEFAULT   22 .dynamic
     23: 000000000000dfa8     0 SECTION LOCAL  DEFAULT   23 .got
     24: 000000000000e000     0 SECTION LOCAL  DEFAULT   24 .got.plt
-    25: 000000000000e208     0 SECTION LOCAL  DEFAULT   25 .data
-    26: 000000000000e210     0 SECTION LOCAL  DEFAULT   26 .nvFatBinSegment
-    27: 000000000000e228     0 SECTION LOCAL  DEFAULT   27 .bss
+    25: 000000000000e210     0 SECTION LOCAL  DEFAULT   25 .data
+    26: 000000000000e218     0 SECTION LOCAL  DEFAULT   26 .nvFatBinSegment
+    27: 000000000000e230     0 SECTION LOCAL  DEFAULT   27 .bss
     28: 0000000000000000     0 SECTION LOCAL  DEFAULT   28 .comment
-    29: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00000258_00000000-6_tgq_simulator.cudafe1.cpp
-    30: 0000000000006780     0 NOTYPE  LOCAL  DEFAULT   17 fatbinData
-    31: 00000000000029c0    16 FUNC    LOCAL  DEFAULT   14 _ZL26__cudaUnregisterBinaryUtilv
-    32: 000000000000e230     8 OBJECT  LOCAL  DEFAULT   27 _ZL20__cudaFatCubinHandle
-    33: 0000000000002830   190 FUNC    LOCAL  DEFAULT   14 _ZL24__sti____cudaRegisterAllv
-    34: 000000000000e210    24 OBJECT  LOCAL  DEFAULT   26 _ZL15__fatDeviceText
+    29: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00000239_00000000-6_tgq_simulator.cudafe1.cpp
+    30: 00000000000067b0     0 NOTYPE  LOCAL  DEFAULT   17 fatbinData
+    31: 00000000000029e0    16 FUNC    LOCAL  DEFAULT   14 _ZL26__cudaUnregisterBinaryUtilv
+    32: 000000000000e238     8 OBJECT  LOCAL  DEFAULT   27 _ZL20__cudaFatCubinHandle
+    33: 0000000000002850   190 FUNC    LOCAL  DEFAULT   14 _ZL24__sti____cudaRegisterAllv
+    34: 000000000000e218    24 OBJECT  LOCAL  DEFAULT   26 _ZL15__fatDeviceText
     35: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    36: 00000000000028f0     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
-    37: 0000000000002920     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
-    38: 0000000000002960     0 FUNC    LOCAL  DEFAULT   14 __do_global_dtors_aux
-    39: 000000000000e228     1 OBJECT  LOCAL  DEFAULT   27 completed.0
+    36: 0000000000002910     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
+    37: 0000000000002940     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
+    38: 0000000000002980     0 FUNC    LOCAL  DEFAULT   14 __do_global_dtors_aux
+    39: 000000000000e230     1 OBJECT  LOCAL  DEFAULT   27 completed.0
     40: 000000000000ddc0     0 OBJECT  LOCAL  DEFAULT   21 __do_global_dtors_aux_fini_array_entry
-    41: 00000000000029a0     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
+    41: 00000000000029c0     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
     42: 000000000000ddb0     0 OBJECT  LOCAL  DEFAULT   20 __frame_dummy_init_array_entry
     43: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS link.stub
-    44: 0000000000006300     0 NOTYPE  LOCAL  DEFAULT   17 fatbinData
+    44: 0000000000006330     0 NOTYPE  LOCAL  DEFAULT   17 fatbinData
     45: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    46: 000000000000caec     0 OBJECT  LOCAL  DEFAULT   19 __FRAME_END__
+    46: 000000000000cb1c     0 OBJECT  LOCAL  DEFAULT   19 __FRAME_END__
     47: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
-    48: 0000000000005490    18 FUNC    LOCAL  DEFAULT   14 atexit
-    49: 00000000000054a4     0 FUNC    LOCAL  DEFAULT   15 _fini
-    50: 000000000000e208     0 OBJECT  LOCAL  DEFAULT   25 __dso_handle
+    48: 00000000000054e0    18 FUNC    LOCAL  DEFAULT   14 atexit
+    49: 00000000000054f4     0 FUNC    LOCAL  DEFAULT   15 _fini
+    50: 000000000000e210     0 OBJECT  LOCAL  DEFAULT   25 __dso_handle
     51: 000000000000ddc8     0 OBJECT  LOCAL  DEFAULT   22 _DYNAMIC
-    52: 000000000000c2c0     0 NOTYPE  LOCAL  DEFAULT   18 __GNU_EH_FRAME_HDR
-    53: 000000000000e210     0 OBJECT  LOCAL  DEFAULT   26 __TMC_END__
+    52: 000000000000c2f0     0 NOTYPE  LOCAL  DEFAULT   18 __GNU_EH_FRAME_HDR
+    53: 000000000000e218     0 OBJECT  LOCAL  DEFAULT   26 __TMC_END__
     54: 000000000000e000     0 OBJECT  LOCAL  DEFAULT   24 _GLOBAL_OFFSET_TABLE_
     55: 0000000000002000     0 FUNC    LOCAL  DEFAULT   10 _init
-    56: 0000000000002f40   201 FUNC    GLOBAL DEFAULT   14 _Z8rxx_gateP6float2f
+    56: 0000000000002f60   201 FUNC    GLOBAL DEFAULT   14 _Z8rxx_gateP6float2f
     57: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sincosf@@GLIBC_2.2.5
-    58: 0000000000002b40   110 FUNC    GLOBAL DEFAULT   14 _Z7ry_gateP6float2f
+    58: 0000000000002b60   110 FUNC    GLOBAL DEFAULT   14 _Z7ry_gateP6float2f
     59: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@@GLIBC_2.2.5
     60: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaUnregisterFatBinary@@libcudart.so.11.0
-    61: 0000000000003930   418 FUNC    GLOBAL DEFAULT   14 _Z23fred_gate_control_smallP6float2
+    61: 0000000000003950   418 FUNC    GLOBAL DEFAULT   14 _Z23fred_gate_control_smallP6float2
     62: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-    63: 0000000000002a70    27 FUNC    GLOBAL DEFAULT   14 _Z6t_gateP6float2
+    63: 0000000000002a90    27 FUNC    GLOBAL DEFAULT   14 _Z6t_gateP6float2
     64: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinary@@libcudart.so.11.0
-    65: 0000000000002ca0   105 FUNC    GLOBAL DEFAULT   14 _Z7pd_gateP6float2f
+    65: 0000000000002cc0   105 FUNC    GLOBAL DEFAULT   14 _Z7pd_gateP6float2f
     66: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND puts@@GLIBC_2.2.5
     67: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND qsort@@GLIBC_2.2.5
-    68: 0000000000005030  1110 FUNC    GLOBAL DEFAULT   14 tripleGateAction
-    69: 0000000000002ec0    55 FUNC    GLOBAL DEFAULT   14 _Z23cnot_gate_control_smallP6float2
-    70: 0000000000003010   204 FUNC    GLOBAL DEFAULT   14 _Z8ryy_gateP6float2f
-    71: 0000000000003d00    82 FUNC    GLOBAL DEFAULT   14 _Z9isInArrayPPKcPci
-    72: 0000000000003ba0   294 FUNC    GLOBAL DEFAULT   14 _Z7getprobP6float2Pfm
-    73: 00000000000030e0   198 FUNC    GLOBAL DEFAULT   14 _Z8rzz_gateP6float2f
+    68: 0000000000005080  1110 FUNC    GLOBAL DEFAULT   14 tripleGateAction
+    69: 0000000000002ee0    55 FUNC    GLOBAL DEFAULT   14 _Z23cnot_gate_control_smallP6float2
+    70: 0000000000003030   204 FUNC    GLOBAL DEFAULT   14 _Z8ryy_gateP6float2f
+    71: 0000000000003d20    82 FUNC    GLOBAL DEFAULT   14 _Z9isInArrayPPKcPci
+    72: 0000000000003bc0   294 FUNC    GLOBAL DEFAULT   14 _Z7getprobP6float2Pfm
+    73: 0000000000003100   198 FUNC    GLOBAL DEFAULT   14 _Z8rzz_gateP6float2f
     74: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@@GLIBC_2.4
-    75: 0000000000003b50    69 FUNC    GLOBAL DEFAULT   14 _Z20generate_binary_dataf
-    76: 0000000000002a10    27 FUNC    GLOBAL DEFAULT   14 _Z6z_gateP6float2
-    77: 0000000000004270   251 FUNC    GLOBAL DEFAULT   14 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
-    78: 0000000000002ab0    26 FUNC    GLOBAL DEFAULT   14 _Z6h_gateP6float2
-    79: 0000000000004380  1444 FUNC    GLOBAL DEFAULT   14 singleGateAction
+    75: 0000000000003b70    69 FUNC    GLOBAL DEFAULT   14 _Z20generate_binary_dataf
+    76: 0000000000002a30    27 FUNC    GLOBAL DEFAULT   14 _Z6z_gateP6float2
+    77: 00000000000042a0   251 FUNC    GLOBAL DEFAULT   14 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
+    78: 0000000000002ad0    26 FUNC    GLOBAL DEFAULT   14 _Z6h_gateP6float2
+    79: 00000000000043b0  1444 FUNC    GLOBAL DEFAULT   14 singleGateAction
     80: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaFree@@libcudart.so.11.0
-    81: 0000000000004930   251 FUNC    GLOBAL DEFAULT   14 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm
+    81: 0000000000004960   251 FUNC    GLOBAL DEFAULT   14 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm
     82: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMemcpy@@libcudart.so.11.0
-    83: 0000000000004a40  1243 FUNC    GLOBAL DEFAULT   14 doubleGateAction
+    83: 0000000000004a70  1269 FUNC    GLOBAL DEFAULT   14 doubleGateAction
     84: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND srand@@GLIBC_2.2.5
-    85: 0000000000003200   115 FUNC    GLOBAL DEFAULT   14 _Z22toff_gate_target_smallP6float2
+    85: 0000000000003220   115 FUNC    GLOBAL DEFAULT   14 _Z22toff_gate_target_smallP6float2
     86: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFunction@@libcudart.so.11.0
     87: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strcmp@@GLIBC_2.2.5
-    88: 00000000000035d0   418 FUNC    GLOBAL DEFAULT   14 _Z21fred_gate_control_bigP6float2
+    88: 00000000000035f0   418 FUNC    GLOBAL DEFAULT   14 _Z21fred_gate_control_bigP6float2
     89: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaDeviceSynchronize@@libcudart.so.11.0
-    90: 0000000000004a30     9 FUNC    GLOBAL DEFAULT   14 _Z19actionOnDoubleQubitP6float2S0_mPm
+    90: 0000000000004a60     9 FUNC    GLOBAL DEFAULT   14 _Z19actionOnDoubleQubitP6float2S0_mPm
     91: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-    92: 0000000000003420   418 FUNC    GLOBAL DEFAULT   14 _Z20toff_gate_target_bigP6float2
+    92: 0000000000003440   418 FUNC    GLOBAL DEFAULT   14 _Z20toff_gate_target_bigP6float2
     93: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND time@@GLIBC_2.2.5
-    94: 0000000000002c20   116 FUNC    GLOBAL DEFAULT   14 _Z11damp_i_gateP6float2f
+    94: 0000000000002c40   116 FUNC    GLOBAL DEFAULT   14 _Z11damp_i_gateP6float2f
     95: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sqrtf@@GLIBC_2.2.5
-    96: 0000000000002dc0    69 FUNC    GLOBAL DEFAULT   14 _Z10iswap_gateP6float2
-    97: 0000000000002e80    55 FUNC    GLOBAL DEFAULT   14 _Z21cnot_gate_control_bigP6float2
-    98: 0000000000002bb0    98 FUNC    GLOBAL DEFAULT   14 _Z7rz_gateP6float2f
-    99: 0000000000002a90    27 FUNC    GLOBAL DEFAULT   14 _Z8tdg_gateP6float2
-   100: 0000000000002d80    55 FUNC    GLOBAL DEFAULT   14 _Z9swap_gateP6float2
+    96: 0000000000002de0    69 FUNC    GLOBAL DEFAULT   14 _Z10iswap_gateP6float2
+    97: 0000000000002ea0    55 FUNC    GLOBAL DEFAULT   14 _Z21cnot_gate_control_bigP6float2
+    98: 0000000000002bd0    98 FUNC    GLOBAL DEFAULT   14 _Z7rz_gateP6float2f
+    99: 0000000000002ab0    27 FUNC    GLOBAL DEFAULT   14 _Z8tdg_gateP6float2
+   100: 0000000000002da0    55 FUNC    GLOBAL DEFAULT   14 _Z9swap_gateP6float2
    101: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@@GLIBC_2.2.5
-   102: 0000000000003d90   526 FUNC    GLOBAL DEFAULT   14 _Z13normalizationP6float2i
-   103: 0000000000002a30    27 FUNC    GLOBAL DEFAULT   14 _Z6s_gateP6float2
+   102: 0000000000003db0   526 FUNC    GLOBAL DEFAULT   14 _Z13normalizationP6float2i
+   103: 0000000000002a50    27 FUNC    GLOBAL DEFAULT   14 _Z6s_gateP6float2
    104: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMalloc@@libcudart.so.11.0
-   105: 0000000000003fa0   707 FUNC    GLOBAL DEFAULT   14 execute_circuit
-   106: 0000000000003d60    33 FUNC    GLOBAL DEFAULT   14 _Z14getArrayLengthPi
+   105: 0000000000003fc0   731 FUNC    GLOBAL DEFAULT   14 execute_circuit
+   106: 0000000000003d80    33 FUNC    GLOBAL DEFAULT   14 _Z14getArrayLengthPi
    107: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaLaunchKernel@@libcudart.so.11.0
-   108: 0000000000003ae0   105 FUNC    GLOBAL DEFAULT   14 _Z11identityMatP6float2i
-   109: 0000000000005020     9 FUNC    GLOBAL DEFAULT   14 _Z18actionOnTripleGateP6float2S0_mPm
-   110: 0000000000002a50    27 FUNC    GLOBAL DEFAULT   14 _Z8sdg_gateP6float2
-   111: 0000000000003280   404 FUNC    GLOBAL DEFAULT   14 _Z20toff_gate_target_midP6float2
-   112: 00000000000029f0    26 FUNC    GLOBAL DEFAULT   14 _Z6y_gateP6float2
-   113: 0000000000002ad0   101 FUNC    GLOBAL DEFAULT   14 _Z7rx_gateP6float2f
-   114: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaSetDevice@@libcudart.so.11.0
-   115: 0000000000002f00    62 FUNC    GLOBAL DEFAULT   14 _Z7cz_gateP6float2
-   116: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@@GLIBC_2.2.5
-   117: 0000000000003780   418 FUNC    GLOBAL DEFAULT   14 _Z21fred_gate_control_midP6float2
-   118: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@@GLIBC_2.2.5
-   119: 0000000000003cd0    47 FUNC    GLOBAL DEFAULT   14 _Z4hashPKc
-   120: 00000000000031b0    69 FUNC    GLOBAL DEFAULT   14 _Z8syc_gateP6float2
-   121: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-   122: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPushCallConfiguration@@libcudart.so.11.0
-   123: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinaryEnd@@libcudart.so.11.0
-   124: 00000000000029b0     9 FUNC    GLOBAL DEFAULT   14 _Z7comparePKvS0_
-   125: 0000000000002e10   109 FUNC    GLOBAL DEFAULT   14 _Z11cphase_gateP6float2f
-   126: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@@GLIBC_2.2.5
-   127: 0000000000002d10   102 FUNC    GLOBAL DEFAULT   14 _Z7ad_gateP6float2f
-   128: 0000000000004370     9 FUNC    GLOBAL DEFAULT   14 _Z19actionOnSingleQubitP6float2S0_mPm
-   129: 0000000000004f20   251 FUNC    GLOBAL DEFAULT   14 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
-   130: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND rand@@GLIBC_2.2.5
-   131: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPopCallConfiguration@@libcudart.so.11.0
-   132: 00000000000029d0    27 FUNC    GLOBAL DEFAULT   14 _Z6x_gateP6float2
+   108: 0000000000003b00   105 FUNC    GLOBAL DEFAULT   14 _Z11identityMatP6float2i
+   109: 0000000000005070     9 FUNC    GLOBAL DEFAULT   14 _Z18actionOnTripleGateP6float2S0_mPm
+   110: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __printf_chk@@GLIBC_2.3.4
+   111: 0000000000002a70    27 FUNC    GLOBAL DEFAULT   14 _Z8sdg_gateP6float2
+   112: 00000000000032a0   404 FUNC    GLOBAL DEFAULT   14 _Z20toff_gate_target_midP6float2
+   113: 0000000000002a10    26 FUNC    GLOBAL DEFAULT   14 _Z6y_gateP6float2
+   114: 0000000000002af0   101 FUNC    GLOBAL DEFAULT   14 _Z7rx_gateP6float2f
+   115: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaSetDevice@@libcudart.so.11.0
+   116: 0000000000002f20    62 FUNC    GLOBAL DEFAULT   14 _Z7cz_gateP6float2
+   117: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@@GLIBC_2.2.5
+   118: 00000000000037a0   418 FUNC    GLOBAL DEFAULT   14 _Z21fred_gate_control_midP6float2
+   119: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@@GLIBC_2.2.5
+   120: 0000000000003cf0    47 FUNC    GLOBAL DEFAULT   14 _Z4hashPKc
+   121: 00000000000031d0    69 FUNC    GLOBAL DEFAULT   14 _Z8syc_gateP6float2
+   122: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+   123: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPushCallConfiguration@@libcudart.so.11.0
+   124: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinaryEnd@@libcudart.so.11.0
+   125: 00000000000029d0     9 FUNC    GLOBAL DEFAULT   14 _Z7comparePKvS0_
+   126: 0000000000002e30   109 FUNC    GLOBAL DEFAULT   14 _Z11cphase_gateP6float2f
+   127: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@@GLIBC_2.2.5
+   128: 0000000000002d30   102 FUNC    GLOBAL DEFAULT   14 _Z7ad_gateP6float2f
+   129: 00000000000043a0     9 FUNC    GLOBAL DEFAULT   14 _Z19actionOnSingleQubitP6float2S0_mPm
+   130: 0000000000004f70   251 FUNC    GLOBAL DEFAULT   14 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
+   131: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND rand@@GLIBC_2.2.5
+   132: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPopCallConfiguration@@libcudart.so.11.0
+   133: 00000000000029f0    27 FUNC    GLOBAL DEFAULT   14 _Z6x_gateP6float2
```

#### readelf --wide --relocs {}

```diff
@@ -1,84 +1,85 @@
 
-Relocation section '.rela.dyn' at offset 0x13c8 contains 16 entries:
+Relocation section '.rela.dyn' at offset 0x1410 contains 16 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-000000000000ddb0  0000000000000008 R_X86_64_RELATIVE                         29a0
-000000000000ddb8  0000000000000008 R_X86_64_RELATIVE                         2830
-000000000000ddc0  0000000000000008 R_X86_64_RELATIVE                         2960
-000000000000e208  0000000000000008 R_X86_64_RELATIVE                         e208
-000000000000e218  0000000000000008 R_X86_64_RELATIVE                         6780
+000000000000ddb0  0000000000000008 R_X86_64_RELATIVE                         29c0
+000000000000ddb8  0000000000000008 R_X86_64_RELATIVE                         2850
+000000000000ddc0  0000000000000008 R_X86_64_RELATIVE                         2980
+000000000000e210  0000000000000008 R_X86_64_RELATIVE                         e210
+000000000000e220  0000000000000008 R_X86_64_RELATIVE                         67b0
 000000000000dfa8  0000000400000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
-000000000000dfb0  0000002600000006 R_X86_64_GLOB_DAT      0000000000005030 tripleGateAction + 0
-000000000000dfb8  0000002a00000006 R_X86_64_GLOB_DAT      0000000000004380 singleGateAction + 0
-000000000000dfc0  0000002c00000006 R_X86_64_GLOB_DAT      0000000000004a40 doubleGateAction + 0
-000000000000dfc8  0000004a00000006 R_X86_64_GLOB_DAT      0000000000004a30 _Z19actionOnDoubleQubitP6float2S0_mPm + 0
+000000000000dfb0  0000002700000006 R_X86_64_GLOB_DAT      0000000000005080 tripleGateAction + 0
+000000000000dfb8  0000002b00000006 R_X86_64_GLOB_DAT      00000000000043b0 singleGateAction + 0
+000000000000dfc0  0000002d00000006 R_X86_64_GLOB_DAT      0000000000004a70 doubleGateAction + 0
+000000000000dfc8  0000004b00000006 R_X86_64_GLOB_DAT      0000000000004a60 _Z19actionOnDoubleQubitP6float2S0_mPm + 0
 000000000000dfd0  0000000f00000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
-000000000000dfd8  0000003600000006 R_X86_64_GLOB_DAT      0000000000005020 _Z18actionOnTripleGateP6float2S0_mPm + 0
-000000000000dfe0  0000001800000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
-000000000000dfe8  0000003e00000006 R_X86_64_GLOB_DAT      00000000000029b0 _Z7comparePKvS0_ + 0
-000000000000dff0  0000001b00000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
-000000000000dff8  0000002900000006 R_X86_64_GLOB_DAT      0000000000004370 _Z19actionOnSingleQubitP6float2S0_mPm + 0
+000000000000dfd8  0000003700000006 R_X86_64_GLOB_DAT      0000000000005070 _Z18actionOnTripleGateP6float2S0_mPm + 0
+000000000000dfe0  0000001900000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
+000000000000dfe8  0000003f00000006 R_X86_64_GLOB_DAT      00000000000029d0 _Z7comparePKvS0_ + 0
+000000000000dff0  0000001c00000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
+000000000000dff8  0000002a00000006 R_X86_64_GLOB_DAT      00000000000043a0 _Z19actionOnSingleQubitP6float2S0_mPm + 0
 
-Relocation section '.rela.plt' at offset 0x1548 contains 62 entries:
+Relocation section '.rela.plt' at offset 0x1590 contains 63 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-000000000000e018  0000004900000007 R_X86_64_JUMP_SLOT     0000000000002f40 _Z8rxx_gateP6float2f + 0
+000000000000e018  0000004a00000007 R_X86_64_JUMP_SLOT     0000000000002f60 _Z8rxx_gateP6float2f + 0
 000000000000e020  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 sincosf@GLIBC_2.2.5 + 0
-000000000000e028  0000004500000007 R_X86_64_JUMP_SLOT     0000000000002b40 _Z7ry_gateP6float2f + 0
+000000000000e028  0000004600000007 R_X86_64_JUMP_SLOT     0000000000002b60 _Z7ry_gateP6float2f + 0
 000000000000e030  0000000200000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
 000000000000e038  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaUnregisterFatBinary@libcudart.so.11.0 + 0
-000000000000e040  0000002200000007 R_X86_64_JUMP_SLOT     0000000000003930 _Z23fred_gate_control_smallP6float2 + 0
-000000000000e048  0000004700000007 R_X86_64_JUMP_SLOT     0000000000002a70 _Z6t_gateP6float2 + 0
+000000000000e040  0000002300000007 R_X86_64_JUMP_SLOT     0000000000003950 _Z23fred_gate_control_smallP6float2 + 0
+000000000000e048  0000004800000007 R_X86_64_JUMP_SLOT     0000000000002a90 _Z6t_gateP6float2 + 0
 000000000000e050  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinary@libcudart.so.11.0 + 0
-000000000000e058  0000002e00000007 R_X86_64_JUMP_SLOT     0000000000002ca0 _Z7pd_gateP6float2f + 0
+000000000000e058  0000002f00000007 R_X86_64_JUMP_SLOT     0000000000002cc0 _Z7pd_gateP6float2f + 0
 000000000000e060  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 puts@GLIBC_2.2.5 + 0
 000000000000e068  0000000700000007 R_X86_64_JUMP_SLOT     0000000000000000 qsort@GLIBC_2.2.5 + 0
-000000000000e070  0000004800000007 R_X86_64_JUMP_SLOT     0000000000002ec0 _Z23cnot_gate_control_smallP6float2 + 0
-000000000000e078  0000003c00000007 R_X86_64_JUMP_SLOT     0000000000003010 _Z8ryy_gateP6float2f + 0
-000000000000e080  0000001e00000007 R_X86_64_JUMP_SLOT     0000000000003d00 _Z9isInArrayPPKcPci + 0
-000000000000e088  0000003100000007 R_X86_64_JUMP_SLOT     00000000000030e0 _Z8rzz_gateP6float2f + 0
+000000000000e070  0000004900000007 R_X86_64_JUMP_SLOT     0000000000002ee0 _Z23cnot_gate_control_smallP6float2 + 0
+000000000000e078  0000003d00000007 R_X86_64_JUMP_SLOT     0000000000003030 _Z8ryy_gateP6float2f + 0
+000000000000e080  0000001f00000007 R_X86_64_JUMP_SLOT     0000000000003d20 _Z9isInArrayPPKcPci + 0
+000000000000e088  0000003200000007 R_X86_64_JUMP_SLOT     0000000000003100 _Z8rzz_gateP6float2f + 0
 000000000000e090  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 __stack_chk_fail@GLIBC_2.4 + 0
-000000000000e098  0000002400000007 R_X86_64_JUMP_SLOT     0000000000002a10 _Z6z_gateP6float2 + 0
-000000000000e0a0  0000004c00000007 R_X86_64_JUMP_SLOT     0000000000004270 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm + 0
-000000000000e0a8  0000003700000007 R_X86_64_JUMP_SLOT     0000000000002ab0 _Z6h_gateP6float2 + 0
+000000000000e098  0000002500000007 R_X86_64_JUMP_SLOT     0000000000002a30 _Z6z_gateP6float2 + 0
+000000000000e0a0  0000004d00000007 R_X86_64_JUMP_SLOT     00000000000042a0 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm + 0
+000000000000e0a8  0000003800000007 R_X86_64_JUMP_SLOT     0000000000002ad0 _Z6h_gateP6float2 + 0
 000000000000e0b0  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaFree@libcudart.so.11.0 + 0
-000000000000e0b8  0000001f00000007 R_X86_64_JUMP_SLOT     0000000000004930 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm + 0
+000000000000e0b8  0000002000000007 R_X86_64_JUMP_SLOT     0000000000004960 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm + 0
 000000000000e0c0  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaMemcpy@libcudart.so.11.0 + 0
 000000000000e0c8  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000000000 srand@GLIBC_2.2.5 + 0
-000000000000e0d0  0000003b00000007 R_X86_64_JUMP_SLOT     0000000000003200 _Z22toff_gate_target_smallP6float2 + 0
+000000000000e0d0  0000003c00000007 R_X86_64_JUMP_SLOT     0000000000003220 _Z22toff_gate_target_smallP6float2 + 0
 000000000000e0d8  0000000c00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFunction@libcudart.so.11.0 + 0
 000000000000e0e0  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000000000 strcmp@GLIBC_2.2.5 + 0
-000000000000e0e8  0000004200000007 R_X86_64_JUMP_SLOT     00000000000035d0 _Z21fred_gate_control_bigP6float2 + 0
+000000000000e0e8  0000004300000007 R_X86_64_JUMP_SLOT     00000000000035f0 _Z21fred_gate_control_bigP6float2 + 0
 000000000000e0f0  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaDeviceSynchronize@libcudart.so.11.0 + 0
-000000000000e0f8  0000003900000007 R_X86_64_JUMP_SLOT     0000000000003420 _Z20toff_gate_target_bigP6float2 + 0
+000000000000e0f8  0000003a00000007 R_X86_64_JUMP_SLOT     0000000000003440 _Z20toff_gate_target_bigP6float2 + 0
 000000000000e100  0000001000000007 R_X86_64_JUMP_SLOT     0000000000000000 time@GLIBC_2.2.5 + 0
-000000000000e108  0000004d00000007 R_X86_64_JUMP_SLOT     0000000000002c20 _Z11damp_i_gateP6float2f + 0
+000000000000e108  0000004e00000007 R_X86_64_JUMP_SLOT     0000000000002c40 _Z11damp_i_gateP6float2f + 0
 000000000000e110  0000001100000007 R_X86_64_JUMP_SLOT     0000000000000000 sqrtf@GLIBC_2.2.5 + 0
-000000000000e118  0000002800000007 R_X86_64_JUMP_SLOT     0000000000002dc0 _Z10iswap_gateP6float2 + 0
-000000000000e120  0000003a00000007 R_X86_64_JUMP_SLOT     0000000000002e80 _Z21cnot_gate_control_bigP6float2 + 0
-000000000000e128  0000003800000007 R_X86_64_JUMP_SLOT     0000000000002bb0 _Z7rz_gateP6float2f + 0
-000000000000e130  0000003500000007 R_X86_64_JUMP_SLOT     0000000000002a90 _Z8tdg_gateP6float2 + 0
-000000000000e138  0000002000000007 R_X86_64_JUMP_SLOT     0000000000002d80 _Z9swap_gateP6float2 + 0
+000000000000e118  0000002900000007 R_X86_64_JUMP_SLOT     0000000000002de0 _Z10iswap_gateP6float2 + 0
+000000000000e120  0000003b00000007 R_X86_64_JUMP_SLOT     0000000000002ea0 _Z21cnot_gate_control_bigP6float2 + 0
+000000000000e128  0000003900000007 R_X86_64_JUMP_SLOT     0000000000002bd0 _Z7rz_gateP6float2f + 0
+000000000000e130  0000003600000007 R_X86_64_JUMP_SLOT     0000000000002ab0 _Z8tdg_gateP6float2 + 0
+000000000000e138  0000002100000007 R_X86_64_JUMP_SLOT     0000000000002da0 _Z9swap_gateP6float2 + 0
 000000000000e140  0000001200000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
-000000000000e148  0000002f00000007 R_X86_64_JUMP_SLOT     0000000000003d90 _Z13normalizationP6float2i + 0
-000000000000e150  0000004300000007 R_X86_64_JUMP_SLOT     0000000000002a30 _Z6s_gateP6float2 + 0
+000000000000e148  0000003000000007 R_X86_64_JUMP_SLOT     0000000000003db0 _Z13normalizationP6float2i + 0
+000000000000e150  0000004400000007 R_X86_64_JUMP_SLOT     0000000000002a50 _Z6s_gateP6float2 + 0
 000000000000e158  0000001300000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaMalloc@libcudart.so.11.0 + 0
-000000000000e160  0000003200000007 R_X86_64_JUMP_SLOT     0000000000003d60 _Z14getArrayLengthPi + 0
+000000000000e160  0000003300000007 R_X86_64_JUMP_SLOT     0000000000003d80 _Z14getArrayLengthPi + 0
 000000000000e168  0000001400000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaLaunchKernel@libcudart.so.11.0 + 0
-000000000000e170  0000002b00000007 R_X86_64_JUMP_SLOT     0000000000002a50 _Z8sdg_gateP6float2 + 0
-000000000000e178  0000002500000007 R_X86_64_JUMP_SLOT     0000000000003280 _Z20toff_gate_target_midP6float2 + 0
-000000000000e180  0000004b00000007 R_X86_64_JUMP_SLOT     00000000000029f0 _Z6y_gateP6float2 + 0
-000000000000e188  0000003000000007 R_X86_64_JUMP_SLOT     0000000000002ad0 _Z7rx_gateP6float2f + 0
-000000000000e190  0000001500000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaSetDevice@libcudart.so.11.0 + 0
-000000000000e198  0000002300000007 R_X86_64_JUMP_SLOT     0000000000002f00 _Z7cz_gateP6float2 + 0
-000000000000e1a0  0000001600000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_atexit@GLIBC_2.2.5 + 0
-000000000000e1a8  0000003300000007 R_X86_64_JUMP_SLOT     0000000000003780 _Z21fred_gate_control_midP6float2 + 0
-000000000000e1b0  0000001700000007 R_X86_64_JUMP_SLOT     0000000000000000 exit@GLIBC_2.2.5 + 0
-000000000000e1b8  0000003d00000007 R_X86_64_JUMP_SLOT     0000000000003cd0 _Z4hashPKc + 0
-000000000000e1c0  0000003f00000007 R_X86_64_JUMP_SLOT     00000000000031b0 _Z8syc_gateP6float2 + 0
-000000000000e1c8  0000001900000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPushCallConfiguration@libcudart.so.11.0 + 0
-000000000000e1d0  0000001a00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinaryEnd@libcudart.so.11.0 + 0
-000000000000e1d8  0000002100000007 R_X86_64_JUMP_SLOT     0000000000002e10 _Z11cphase_gateP6float2f + 0
-000000000000e1e0  0000002d00000007 R_X86_64_JUMP_SLOT     0000000000002d10 _Z7ad_gateP6float2f + 0
-000000000000e1e8  0000004400000007 R_X86_64_JUMP_SLOT     0000000000004f20 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm + 0
-000000000000e1f0  0000001c00000007 R_X86_64_JUMP_SLOT     0000000000000000 rand@GLIBC_2.2.5 + 0
-000000000000e1f8  0000001d00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPopCallConfiguration@libcudart.so.11.0 + 0
-000000000000e200  0000004600000007 R_X86_64_JUMP_SLOT     00000000000029d0 _Z6x_gateP6float2 + 0
+000000000000e170  0000001500000007 R_X86_64_JUMP_SLOT     0000000000000000 __printf_chk@GLIBC_2.3.4 + 0
+000000000000e178  0000002c00000007 R_X86_64_JUMP_SLOT     0000000000002a70 _Z8sdg_gateP6float2 + 0
+000000000000e180  0000002600000007 R_X86_64_JUMP_SLOT     00000000000032a0 _Z20toff_gate_target_midP6float2 + 0
+000000000000e188  0000004c00000007 R_X86_64_JUMP_SLOT     0000000000002a10 _Z6y_gateP6float2 + 0
+000000000000e190  0000003100000007 R_X86_64_JUMP_SLOT     0000000000002af0 _Z7rx_gateP6float2f + 0
+000000000000e198  0000001600000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaSetDevice@libcudart.so.11.0 + 0
+000000000000e1a0  0000002400000007 R_X86_64_JUMP_SLOT     0000000000002f20 _Z7cz_gateP6float2 + 0
+000000000000e1a8  0000001700000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_atexit@GLIBC_2.2.5 + 0
+000000000000e1b0  0000003400000007 R_X86_64_JUMP_SLOT     00000000000037a0 _Z21fred_gate_control_midP6float2 + 0
+000000000000e1b8  0000001800000007 R_X86_64_JUMP_SLOT     0000000000000000 exit@GLIBC_2.2.5 + 0
+000000000000e1c0  0000003e00000007 R_X86_64_JUMP_SLOT     0000000000003cf0 _Z4hashPKc + 0
+000000000000e1c8  0000004000000007 R_X86_64_JUMP_SLOT     00000000000031d0 _Z8syc_gateP6float2 + 0
+000000000000e1d0  0000001a00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPushCallConfiguration@libcudart.so.11.0 + 0
+000000000000e1d8  0000001b00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinaryEnd@libcudart.so.11.0 + 0
+000000000000e1e0  0000002200000007 R_X86_64_JUMP_SLOT     0000000000002e30 _Z11cphase_gateP6float2f + 0
+000000000000e1e8  0000002e00000007 R_X86_64_JUMP_SLOT     0000000000002d30 _Z7ad_gateP6float2f + 0
+000000000000e1f0  0000004500000007 R_X86_64_JUMP_SLOT     0000000000004f70 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm + 0
+000000000000e1f8  0000001d00000007 R_X86_64_JUMP_SLOT     0000000000000000 rand@GLIBC_2.2.5 + 0
+000000000000e200  0000001e00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPopCallConfiguration@libcudart.so.11.0 + 0
+000000000000e208  0000004700000007 R_X86_64_JUMP_SLOT     00000000000029f0 _Z6x_gateP6float2 + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -1,29 +1,29 @@
 
 Dynamic section at offset 0xcdc8 contains 26 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libcudart.so.11.0]
  0x0000000000000001 (NEEDED)             Shared library: [libm.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x000000000000000c (INIT)               0x2000
- 0x000000000000000d (FINI)               0x54a4
+ 0x000000000000000d (FINI)               0x54f4
  0x0000000000000019 (INIT_ARRAY)         0xddb0
  0x000000000000001b (INIT_ARRAYSZ)       16 (bytes)
  0x000000000000001a (FINI_ARRAY)         0xddc0
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x2f0
- 0x0000000000000005 (STRTAB)             0xbe8
+ 0x0000000000000005 (STRTAB)             0xc00
  0x0000000000000006 (SYMTAB)             0x498
- 0x000000000000000a (STRSZ)              1746 (bytes)
+ 0x000000000000000a (STRSZ)              1771 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
  0x0000000000000003 (PLTGOT)             0xe000
- 0x0000000000000002 (PLTRELSZ)           1488 (bytes)
+ 0x0000000000000002 (PLTRELSZ)           1512 (bytes)
  0x0000000000000014 (PLTREL)             RELA
- 0x0000000000000017 (JMPREL)             0x1548
- 0x0000000000000007 (RELA)               0x13c8
+ 0x0000000000000017 (JMPREL)             0x1590
+ 0x0000000000000007 (RELA)               0x1410
  0x0000000000000008 (RELASZ)             384 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
- 0x000000006ffffffe (VERNEED)            0x1358
+ 0x000000006ffffffe (VERNEED)            0x1390
  0x000000006fffffff (VERNEEDNUM)         3
- 0x000000006ffffff0 (VERSYM)             0x12ba
+ 0x000000006ffffff0 (VERSYM)             0x12ec
  0x000000006ffffff9 (RELACOUNT)          5
  0x0000000000000000 (NULL)               0x0
```

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 95b9732f33b40c9bf16d8d593e640b8fe93e51cc
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: bd357528ec3539952ec3b115a22654dc70d3cb32
```

#### readelf --wide --version-info {}

```diff
@@ -1,33 +1,34 @@
 
-Version symbols section '.gnu.version' contains 78 entries:
- Addr: 0x00000000000012ba  Offset: 0x000012ba  Link: 4 (.dynsym)
+Version symbols section '.gnu.version' contains 79 entries:
+ Addr: 0x00000000000012ec  Offset: 0x000012ec  Link: 4 (.dynsym)
   000:   0 (*local*)       2 (GLIBC_2.2.5)   3 (GLIBC_2.2.5)   4 (libcudart.so.11.0)    
   004:   0 (*local*)       4 (libcudart.so.11.0)       3 (GLIBC_2.2.5)   3 (GLIBC_2.2.5)
   008:   5 (GLIBC_2.4)     4 (libcudart.so.11.0)       4 (libcudart.so.11.0)       3 (GLIBC_2.2.5)
   00c:   4 (libcudart.so.11.0)       3 (GLIBC_2.2.5)   4 (libcudart.so.11.0)       0 (*local*)    
   010:   3 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)   3 (GLIBC_2.2.5)   4 (libcudart.so.11.0)    
-  014:   4 (libcudart.so.11.0)       4 (libcudart.so.11.0)       3 (GLIBC_2.2.5)   3 (GLIBC_2.2.5)
-  018:   0 (*local*)       4 (libcudart.so.11.0)       4 (libcudart.so.11.0)       3 (GLIBC_2.2.5)
-  01c:   3 (GLIBC_2.2.5)   4 (libcudart.so.11.0)       1 (*global*)      1 (*global*)   
+  014:   4 (libcudart.so.11.0)       6 (GLIBC_2.3.4)   4 (libcudart.so.11.0)       3 (GLIBC_2.2.5)
+  018:   3 (GLIBC_2.2.5)   0 (*local*)       4 (libcudart.so.11.0)       4 (libcudart.so.11.0)    
+  01c:   3 (GLIBC_2.2.5)   3 (GLIBC_2.2.5)   4 (libcudart.so.11.0)       1 (*global*)   
   020:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   024:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   028:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   02c:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   030:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   034:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   038:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   03c:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   040:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   044:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   048:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
-  04c:   1 (*global*)      1 (*global*)   
+  04c:   1 (*global*)      1 (*global*)      1 (*global*)   
 
 Version needs section '.gnu.version_r' contains 3 entries:
- Addr: 0x0000000000001358  Offset: 0x00001358  Link: 5 (.dynstr)
+ Addr: 0x0000000000001390  Offset: 0x00001390  Link: 5 (.dynstr)
   000000: Version: 1  File: libcudart.so.11.0  Cnt: 1
   0x0010:   Name: libcudart.so.11.0  Flags: none  Version: 4
-  0x0020: Version: 1  File: libc.so.6  Cnt: 2
-  0x0030:   Name: GLIBC_2.4  Flags: none  Version: 5
-  0x0040:   Name: GLIBC_2.2.5  Flags: none  Version: 3
-  0x0050: Version: 1  File: libm.so.6  Cnt: 1
-  0x0060:   Name: GLIBC_2.2.5  Flags: none  Version: 2
+  0x0020: Version: 1  File: libc.so.6  Cnt: 3
+  0x0030:   Name: GLIBC_2.3.4  Flags: none  Version: 6
+  0x0040:   Name: GLIBC_2.4  Flags: none  Version: 5
+  0x0050:   Name: GLIBC_2.2.5  Flags: none  Version: 3
+  0x0060: Version: 1  File: libm.so.6  Cnt: 1
+  0x0070:   Name: GLIBC_2.2.5  Flags: none  Version: 2
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -9,596 +9,596 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000024 0000001c FDE cie=00000000 pc=0000000000002020..0000000000002410
+00000018 0000000000000024 0000001c FDE cie=00000000 pc=0000000000002020..0000000000002420
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 6 to 0000000000002026
   DW_CFA_def_cfa_offset: 24
   DW_CFA_advance_loc: 10 to 0000000000002030
   DW_CFA_def_cfa_expression (DW_OP_breg7 (rsp): 8; DW_OP_breg16 (rip): 0; DW_OP_lit15; DW_OP_and; DW_OP_lit10; DW_OP_ge; DW_OP_lit3; DW_OP_shl; DW_OP_plus)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000040 0000000000000014 00000044 FDE cie=00000000 pc=0000000000002410..0000000000002450
+00000040 0000000000000014 00000044 FDE cie=00000000 pc=0000000000002420..0000000000002460
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000058 0000000000000014 0000005c FDE cie=00000000 pc=0000000000002450..0000000000002830
+00000058 0000000000000014 0000005c FDE cie=00000000 pc=0000000000002460..0000000000002850
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000070 0000000000000010 00000074 FDE cie=00000000 pc=00000000000029b0..00000000000029b9
+00000070 0000000000000010 00000074 FDE cie=00000000 pc=00000000000029d0..00000000000029d9
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000084 0000000000000010 00000088 FDE cie=00000000 pc=00000000000029c0..00000000000029d0
+00000084 0000000000000010 00000088 FDE cie=00000000 pc=00000000000029e0..00000000000029f0
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000098 0000000000000010 0000009c FDE cie=00000000 pc=00000000000029d0..00000000000029eb
+00000098 0000000000000010 0000009c FDE cie=00000000 pc=00000000000029f0..0000000000002a0b
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000ac 0000000000000010 000000b0 FDE cie=00000000 pc=00000000000029f0..0000000000002a0a
+000000ac 0000000000000010 000000b0 FDE cie=00000000 pc=0000000000002a10..0000000000002a2a
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000c0 0000000000000010 000000c4 FDE cie=00000000 pc=0000000000002a10..0000000000002a2b
+000000c0 0000000000000010 000000c4 FDE cie=00000000 pc=0000000000002a30..0000000000002a4b
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000d4 0000000000000010 000000d8 FDE cie=00000000 pc=0000000000002a30..0000000000002a4b
+000000d4 0000000000000010 000000d8 FDE cie=00000000 pc=0000000000002a50..0000000000002a6b
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000e8 0000000000000010 000000ec FDE cie=00000000 pc=0000000000002a50..0000000000002a6b
+000000e8 0000000000000010 000000ec FDE cie=00000000 pc=0000000000002a70..0000000000002a8b
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000fc 0000000000000010 00000100 FDE cie=00000000 pc=0000000000002a70..0000000000002a8b
+000000fc 0000000000000010 00000100 FDE cie=00000000 pc=0000000000002a90..0000000000002aab
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000110 0000000000000010 00000114 FDE cie=00000000 pc=0000000000002a90..0000000000002aab
+00000110 0000000000000010 00000114 FDE cie=00000000 pc=0000000000002ab0..0000000000002acb
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000124 0000000000000010 00000128 FDE cie=00000000 pc=0000000000002ab0..0000000000002aca
+00000124 0000000000000010 00000128 FDE cie=00000000 pc=0000000000002ad0..0000000000002aea
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000138 000000000000001c 0000013c FDE cie=00000000 pc=0000000000002ad0..0000000000002b35
-  DW_CFA_advance_loc: 5 to 0000000000002ad5
+00000138 000000000000001c 0000013c FDE cie=00000000 pc=0000000000002af0..0000000000002b55
+  DW_CFA_advance_loc: 5 to 0000000000002af5
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 0000000000002adc
+  DW_CFA_advance_loc: 7 to 0000000000002afc
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 87 to 0000000000002b33
+  DW_CFA_advance_loc1: 87 to 0000000000002b53
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000002b34
+  DW_CFA_advance_loc: 1 to 0000000000002b54
   DW_CFA_def_cfa_offset: 8
 
-00000158 000000000000001c 0000015c FDE cie=00000000 pc=0000000000002b40..0000000000002bae
-  DW_CFA_advance_loc: 5 to 0000000000002b45
+00000158 000000000000001c 0000015c FDE cie=00000000 pc=0000000000002b60..0000000000002bce
+  DW_CFA_advance_loc: 5 to 0000000000002b65
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 0000000000002b4c
+  DW_CFA_advance_loc: 7 to 0000000000002b6c
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 96 to 0000000000002bac
+  DW_CFA_advance_loc1: 96 to 0000000000002bcc
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000002bad
+  DW_CFA_advance_loc: 1 to 0000000000002bcd
   DW_CFA_def_cfa_offset: 8
 
-00000178 000000000000001c 0000017c FDE cie=00000000 pc=0000000000002bb0..0000000000002c12
-  DW_CFA_advance_loc: 5 to 0000000000002bb5
+00000178 000000000000001c 0000017c FDE cie=00000000 pc=0000000000002bd0..0000000000002c32
+  DW_CFA_advance_loc: 5 to 0000000000002bd5
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 0000000000002bbc
+  DW_CFA_advance_loc: 7 to 0000000000002bdc
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 84 to 0000000000002c10
+  DW_CFA_advance_loc1: 84 to 0000000000002c30
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000002c11
+  DW_CFA_advance_loc: 1 to 0000000000002c31
   DW_CFA_def_cfa_offset: 8
 
-00000198 0000000000000014 0000019c FDE cie=00000000 pc=0000000000002c20..0000000000002c94
-  DW_CFA_advance_loc1: 81 to 0000000000002c71
+00000198 0000000000000014 0000019c FDE cie=00000000 pc=0000000000002c40..0000000000002cb4
+  DW_CFA_advance_loc1: 81 to 0000000000002c91
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 34 to 0000000000002c93
+  DW_CFA_advance_loc: 34 to 0000000000002cb3
   DW_CFA_def_cfa_offset: 8
 
-000001b0 0000000000000014 000001b4 FDE cie=00000000 pc=0000000000002ca0..0000000000002d09
-  DW_CFA_advance_loc1: 73 to 0000000000002ce9
+000001b0 0000000000000014 000001b4 FDE cie=00000000 pc=0000000000002cc0..0000000000002d29
+  DW_CFA_advance_loc1: 73 to 0000000000002d09
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 31 to 0000000000002d08
+  DW_CFA_advance_loc: 31 to 0000000000002d28
   DW_CFA_def_cfa_offset: 8
 
-000001c8 0000000000000018 000001cc FDE cie=00000000 pc=0000000000002d10..0000000000002d76
-  DW_CFA_advance_loc: 36 to 0000000000002d34
+000001c8 0000000000000018 000001cc FDE cie=00000000 pc=0000000000002d30..0000000000002d96
+  DW_CFA_advance_loc: 36 to 0000000000002d54
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 48 to 0000000000002d64
+  DW_CFA_advance_loc: 48 to 0000000000002d84
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000002d65
+  DW_CFA_advance_loc: 1 to 0000000000002d85
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
 
-000001e4 0000000000000010 000001e8 FDE cie=00000000 pc=0000000000002d80..0000000000002db7
+000001e4 0000000000000010 000001e8 FDE cie=00000000 pc=0000000000002da0..0000000000002dd7
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001f8 0000000000000010 000001fc FDE cie=00000000 pc=0000000000002dc0..0000000000002e05
+000001f8 0000000000000010 000001fc FDE cie=00000000 pc=0000000000002de0..0000000000002e25
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000020c 000000000000001c 00000210 FDE cie=00000000 pc=0000000000002e10..0000000000002e7d
-  DW_CFA_advance_loc: 5 to 0000000000002e15
+0000020c 000000000000001c 00000210 FDE cie=00000000 pc=0000000000002e30..0000000000002e9d
+  DW_CFA_advance_loc: 5 to 0000000000002e35
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 0000000000002e1c
+  DW_CFA_advance_loc: 7 to 0000000000002e3c
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 95 to 0000000000002e7b
+  DW_CFA_advance_loc1: 95 to 0000000000002e9b
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000002e7c
+  DW_CFA_advance_loc: 1 to 0000000000002e9c
   DW_CFA_def_cfa_offset: 8
 
-0000022c 0000000000000010 00000230 FDE cie=00000000 pc=0000000000002e80..0000000000002eb7
+0000022c 0000000000000010 00000230 FDE cie=00000000 pc=0000000000002ea0..0000000000002ed7
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000240 0000000000000010 00000244 FDE cie=00000000 pc=0000000000002ec0..0000000000002ef7
+00000240 0000000000000010 00000244 FDE cie=00000000 pc=0000000000002ee0..0000000000002f17
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000254 0000000000000010 00000258 FDE cie=00000000 pc=0000000000002f00..0000000000002f3e
+00000254 0000000000000010 00000258 FDE cie=00000000 pc=0000000000002f20..0000000000002f5e
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000268 000000000000001c 0000026c FDE cie=00000000 pc=0000000000002f40..0000000000003009
-  DW_CFA_advance_loc: 5 to 0000000000002f45
+00000268 000000000000001c 0000026c FDE cie=00000000 pc=0000000000002f60..0000000000003029
+  DW_CFA_advance_loc: 5 to 0000000000002f65
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 0000000000002f4c
+  DW_CFA_advance_loc: 7 to 0000000000002f6c
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 187 to 0000000000003007
+  DW_CFA_advance_loc1: 187 to 0000000000003027
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000003008
+  DW_CFA_advance_loc: 1 to 0000000000003028
   DW_CFA_def_cfa_offset: 8
 
-00000288 000000000000001c 0000028c FDE cie=00000000 pc=0000000000003010..00000000000030dc
-  DW_CFA_advance_loc: 5 to 0000000000003015
+00000288 000000000000001c 0000028c FDE cie=00000000 pc=0000000000003030..00000000000030fc
+  DW_CFA_advance_loc: 5 to 0000000000003035
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 000000000000301c
+  DW_CFA_advance_loc: 7 to 000000000000303c
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 190 to 00000000000030da
+  DW_CFA_advance_loc1: 190 to 00000000000030fa
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000000000030db
+  DW_CFA_advance_loc: 1 to 00000000000030fb
   DW_CFA_def_cfa_offset: 8
 
-000002a8 000000000000001c 000002ac FDE cie=00000000 pc=00000000000030e0..00000000000031a6
-  DW_CFA_advance_loc: 5 to 00000000000030e5
+000002a8 000000000000001c 000002ac FDE cie=00000000 pc=0000000000003100..00000000000031c6
+  DW_CFA_advance_loc: 5 to 0000000000003105
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 00000000000030ec
+  DW_CFA_advance_loc: 7 to 000000000000310c
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 184 to 00000000000031a4
+  DW_CFA_advance_loc1: 184 to 00000000000031c4
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000000000031a5
+  DW_CFA_advance_loc: 1 to 00000000000031c5
   DW_CFA_def_cfa_offset: 8
 
-000002c8 0000000000000010 000002cc FDE cie=00000000 pc=00000000000031b0..00000000000031f5
+000002c8 0000000000000010 000002cc FDE cie=00000000 pc=00000000000031d0..0000000000003215
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000002dc 0000000000000010 000002e0 FDE cie=00000000 pc=0000000000003200..0000000000003273
+000002dc 0000000000000010 000002e0 FDE cie=00000000 pc=0000000000003220..0000000000003293
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000002f0 0000000000000010 000002f4 FDE cie=00000000 pc=0000000000003280..0000000000003414
+000002f0 0000000000000010 000002f4 FDE cie=00000000 pc=00000000000032a0..0000000000003434
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000304 0000000000000010 00000308 FDE cie=00000000 pc=0000000000003420..00000000000035c2
+00000304 0000000000000010 00000308 FDE cie=00000000 pc=0000000000003440..00000000000035e2
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000318 0000000000000010 0000031c FDE cie=00000000 pc=00000000000035d0..0000000000003772
+00000318 0000000000000010 0000031c FDE cie=00000000 pc=00000000000035f0..0000000000003792
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000032c 0000000000000010 00000330 FDE cie=00000000 pc=0000000000003780..0000000000003922
+0000032c 0000000000000010 00000330 FDE cie=00000000 pc=00000000000037a0..0000000000003942
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000340 0000000000000010 00000344 FDE cie=00000000 pc=0000000000003930..0000000000003ad2
+00000340 0000000000000010 00000344 FDE cie=00000000 pc=0000000000003950..0000000000003af2
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000354 0000000000000010 00000358 FDE cie=00000000 pc=0000000000003ae0..0000000000003b49
+00000354 0000000000000010 00000358 FDE cie=00000000 pc=0000000000003b00..0000000000003b69
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000368 0000000000000014 0000036c FDE cie=00000000 pc=0000000000003b50..0000000000003b95
-  DW_CFA_advance_loc: 8 to 0000000000003b58
+00000368 0000000000000014 0000036c FDE cie=00000000 pc=0000000000003b70..0000000000003bb5
+  DW_CFA_advance_loc: 8 to 0000000000003b78
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 60 to 0000000000003b94
+  DW_CFA_advance_loc: 60 to 0000000000003bb4
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
 
-00000380 0000000000000010 00000384 FDE cie=00000000 pc=0000000000003ba0..0000000000003cc6
+00000380 0000000000000010 00000384 FDE cie=00000000 pc=0000000000003bc0..0000000000003ce6
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000394 0000000000000010 00000398 FDE cie=00000000 pc=0000000000003cd0..0000000000003cff
+00000394 0000000000000010 00000398 FDE cie=00000000 pc=0000000000003cf0..0000000000003d1f
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000003a8 0000000000000038 000003ac FDE cie=00000000 pc=0000000000003d00..0000000000003d52
-  DW_CFA_advance_loc: 13 to 0000000000003d0d
+000003a8 0000000000000038 000003ac FDE cie=00000000 pc=0000000000003d20..0000000000003d72
+  DW_CFA_advance_loc: 13 to 0000000000003d2d
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r12 (r12) at cfa-16
-  DW_CFA_advance_loc: 6 to 0000000000003d13
+  DW_CFA_advance_loc: 6 to 0000000000003d33
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r6 (rbp) at cfa-24
-  DW_CFA_advance_loc: 4 to 0000000000003d17
+  DW_CFA_advance_loc: 4 to 0000000000003d37
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r3 (rbx) at cfa-32
-  DW_CFA_advance_loc: 34 to 0000000000003d39
+  DW_CFA_advance_loc: 34 to 0000000000003d59
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 6 to 0000000000003d3f
+  DW_CFA_advance_loc: 6 to 0000000000003d5f
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000003d41
+  DW_CFA_advance_loc: 2 to 0000000000003d61
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 0000000000003d48
+  DW_CFA_advance_loc: 7 to 0000000000003d68
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 1 to 0000000000003d49
+  DW_CFA_advance_loc: 1 to 0000000000003d69
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 3 to 0000000000003d4c
+  DW_CFA_advance_loc: 3 to 0000000000003d6c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000003d4e
+  DW_CFA_advance_loc: 2 to 0000000000003d6e
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000003d4f
+  DW_CFA_advance_loc: 1 to 0000000000003d6f
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000003e4 0000000000000010 000003e8 FDE cie=00000000 pc=0000000000003d60..0000000000003d81
+000003e4 0000000000000010 000003e8 FDE cie=00000000 pc=0000000000003d80..0000000000003da1
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000003f8 0000000000000010 000003fc FDE cie=00000000 pc=0000000000003d90..0000000000003f9e
+000003f8 0000000000000010 000003fc FDE cie=00000000 pc=0000000000003db0..0000000000003fbe
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000040c 000000000000004c 00000410 FDE cie=00000000 pc=0000000000003fa0..0000000000004263
-  DW_CFA_advance_loc: 6 to 0000000000003fa6
+0000040c 000000000000004c 00000410 FDE cie=00000000 pc=0000000000003fc0..000000000000429b
+  DW_CFA_advance_loc: 6 to 0000000000003fc6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 12 to 0000000000003fb2
+  DW_CFA_advance_loc: 12 to 0000000000003fd2
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 14 to 0000000000003fc0
+  DW_CFA_advance_loc: 2 to 0000000000003fd4
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000003fc2
+  DW_CFA_advance_loc: 2 to 0000000000003fd6
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 11 to 0000000000003fcd
+  DW_CFA_advance_loc: 11 to 0000000000003fe1
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 11 to 0000000000003fd8
+  DW_CFA_advance_loc: 16 to 0000000000003ff1
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 0000000000003fdf
+  DW_CFA_advance_loc: 14 to 0000000000003fff
   DW_CFA_def_cfa_offset: 304
-  DW_CFA_advance_loc2: 587 to 000000000000422a
+  DW_CFA_advance_loc2: 611 to 0000000000004262
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 000000000000422b
+  DW_CFA_advance_loc: 1 to 0000000000004263
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000422c
+  DW_CFA_advance_loc: 1 to 0000000000004264
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000422e
+  DW_CFA_advance_loc: 2 to 0000000000004266
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000004230
+  DW_CFA_advance_loc: 2 to 0000000000004268
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000004232
+  DW_CFA_advance_loc: 2 to 000000000000426a
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000004234
+  DW_CFA_advance_loc: 2 to 000000000000426c
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 4 to 0000000000004238
+  DW_CFA_advance_loc: 4 to 0000000000004270
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000045c 0000000000000028 00000460 FDE cie=00000000 pc=0000000000004270..000000000000436b
-  DW_CFA_advance_loc: 11 to 000000000000427b
+0000045c 0000000000000028 00000460 FDE cie=00000000 pc=00000000000042a0..000000000000439b
+  DW_CFA_advance_loc: 11 to 00000000000042ab
   DW_CFA_def_cfa_offset: 176
-  DW_CFA_advance_loc1: 163 to 000000000000431e
+  DW_CFA_advance_loc1: 163 to 000000000000434e
   DW_CFA_def_cfa_offset: 184
-  DW_CFA_advance_loc: 11 to 0000000000004329
+  DW_CFA_advance_loc: 11 to 0000000000004359
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc: 33 to 000000000000434a
+  DW_CFA_advance_loc: 33 to 000000000000437a
   DW_CFA_def_cfa_offset: 184
-  DW_CFA_advance_loc: 1 to 000000000000434b
+  DW_CFA_advance_loc: 1 to 000000000000437b
   DW_CFA_def_cfa_offset: 176
-  DW_CFA_advance_loc: 26 to 0000000000004365
+  DW_CFA_advance_loc: 26 to 0000000000004395
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000004366
+  DW_CFA_advance_loc: 1 to 0000000000004396
   DW_CFA_restore_state
 
-00000488 0000000000000010 0000048c FDE cie=00000000 pc=0000000000004370..0000000000004379
+00000488 0000000000000010 0000048c FDE cie=00000000 pc=00000000000043a0..00000000000043a9
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000049c 000000000000004c 000004a0 FDE cie=00000000 pc=0000000000004380..0000000000004924
-  DW_CFA_advance_loc: 6 to 0000000000004386
+0000049c 000000000000004c 000004a0 FDE cie=00000000 pc=00000000000043b0..0000000000004954
+  DW_CFA_advance_loc: 6 to 00000000000043b6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000004388
+  DW_CFA_advance_loc: 2 to 00000000000043b8
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 8 to 0000000000004390
+  DW_CFA_advance_loc: 8 to 00000000000043c0
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 12 to 000000000000439c
+  DW_CFA_advance_loc: 12 to 00000000000043cc
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000439d
+  DW_CFA_advance_loc: 1 to 00000000000043cd
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 00000000000043a1
+  DW_CFA_advance_loc: 4 to 00000000000043d1
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 14 to 00000000000043af
+  DW_CFA_advance_loc: 14 to 00000000000043df
   DW_CFA_def_cfa_offset: 272
-  DW_CFA_advance_loc2: 831 to 00000000000046ee
+  DW_CFA_advance_loc2: 831 to 000000000000471e
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 00000000000046f2
+  DW_CFA_advance_loc: 4 to 0000000000004722
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000046f3
+  DW_CFA_advance_loc: 1 to 0000000000004723
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000046f5
+  DW_CFA_advance_loc: 2 to 0000000000004725
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000046f7
+  DW_CFA_advance_loc: 2 to 0000000000004727
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000046f9
+  DW_CFA_advance_loc: 2 to 0000000000004729
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000046fb
+  DW_CFA_advance_loc: 2 to 000000000000472b
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 5 to 0000000000004700
+  DW_CFA_advance_loc: 5 to 0000000000004730
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000004ec 0000000000000028 000004f0 FDE cie=00000000 pc=0000000000004930..0000000000004a2b
-  DW_CFA_advance_loc: 11 to 000000000000493b
+000004ec 0000000000000028 000004f0 FDE cie=00000000 pc=0000000000004960..0000000000004a5b
+  DW_CFA_advance_loc: 11 to 000000000000496b
   DW_CFA_def_cfa_offset: 176
-  DW_CFA_advance_loc1: 163 to 00000000000049de
+  DW_CFA_advance_loc1: 163 to 0000000000004a0e
   DW_CFA_def_cfa_offset: 184
-  DW_CFA_advance_loc: 11 to 00000000000049e9
+  DW_CFA_advance_loc: 11 to 0000000000004a19
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc: 33 to 0000000000004a0a
+  DW_CFA_advance_loc: 33 to 0000000000004a3a
   DW_CFA_def_cfa_offset: 184
-  DW_CFA_advance_loc: 1 to 0000000000004a0b
+  DW_CFA_advance_loc: 1 to 0000000000004a3b
   DW_CFA_def_cfa_offset: 176
-  DW_CFA_advance_loc: 26 to 0000000000004a25
+  DW_CFA_advance_loc: 26 to 0000000000004a55
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000004a26
+  DW_CFA_advance_loc: 1 to 0000000000004a56
   DW_CFA_restore_state
 
-00000518 0000000000000010 0000051c FDE cie=00000000 pc=0000000000004a30..0000000000004a39
+00000518 0000000000000010 0000051c FDE cie=00000000 pc=0000000000004a60..0000000000004a69
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000052c 000000000000004c 00000530 FDE cie=00000000 pc=0000000000004a40..0000000000004f1b
-  DW_CFA_advance_loc: 6 to 0000000000004a46
+0000052c 000000000000004c 00000530 FDE cie=00000000 pc=0000000000004a70..0000000000004f65
+  DW_CFA_advance_loc: 6 to 0000000000004a76
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000004a48
+  DW_CFA_advance_loc: 2 to 0000000000004a78
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 8 to 0000000000004a50
+  DW_CFA_advance_loc: 8 to 0000000000004a80
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 0000000000004a55
+  DW_CFA_advance_loc: 5 to 0000000000004a85
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000004a56
+  DW_CFA_advance_loc: 4 to 0000000000004a89
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 0000000000004a5a
+  DW_CFA_advance_loc: 1 to 0000000000004a8a
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 10 to 0000000000004a64
+  DW_CFA_advance_loc: 10 to 0000000000004a94
   DW_CFA_def_cfa_offset: 224
-  DW_CFA_advance_loc2: 771 to 0000000000004d67
+  DW_CFA_advance_loc2: 795 to 0000000000004daf
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 0000000000004d6b
+  DW_CFA_advance_loc: 4 to 0000000000004db3
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000004d6c
+  DW_CFA_advance_loc: 1 to 0000000000004db4
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000004d6e
+  DW_CFA_advance_loc: 2 to 0000000000004db6
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000004d70
+  DW_CFA_advance_loc: 2 to 0000000000004db8
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000004d72
+  DW_CFA_advance_loc: 2 to 0000000000004dba
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000004d74
+  DW_CFA_advance_loc: 2 to 0000000000004dbc
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 12 to 0000000000004d80
+  DW_CFA_advance_loc: 12 to 0000000000004dc8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000057c 0000000000000028 00000580 FDE cie=00000000 pc=0000000000004f20..000000000000501b
-  DW_CFA_advance_loc: 11 to 0000000000004f2b
+0000057c 0000000000000028 00000580 FDE cie=00000000 pc=0000000000004f70..000000000000506b
+  DW_CFA_advance_loc: 11 to 0000000000004f7b
   DW_CFA_def_cfa_offset: 176
-  DW_CFA_advance_loc1: 163 to 0000000000004fce
+  DW_CFA_advance_loc1: 163 to 000000000000501e
   DW_CFA_def_cfa_offset: 184
-  DW_CFA_advance_loc: 11 to 0000000000004fd9
+  DW_CFA_advance_loc: 11 to 0000000000005029
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc: 33 to 0000000000004ffa
+  DW_CFA_advance_loc: 33 to 000000000000504a
   DW_CFA_def_cfa_offset: 184
-  DW_CFA_advance_loc: 1 to 0000000000004ffb
+  DW_CFA_advance_loc: 1 to 000000000000504b
   DW_CFA_def_cfa_offset: 176
-  DW_CFA_advance_loc: 26 to 0000000000005015
+  DW_CFA_advance_loc: 26 to 0000000000005065
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000005016
+  DW_CFA_advance_loc: 1 to 0000000000005066
   DW_CFA_restore_state
 
-000005a8 0000000000000010 000005ac FDE cie=00000000 pc=0000000000005020..0000000000005029
+000005a8 0000000000000010 000005ac FDE cie=00000000 pc=0000000000005070..0000000000005079
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000005bc 000000000000004c 000005c0 FDE cie=00000000 pc=0000000000005030..0000000000005486
-  DW_CFA_advance_loc: 6 to 0000000000005036
+000005bc 000000000000004c 000005c0 FDE cie=00000000 pc=0000000000005080..00000000000054d6
+  DW_CFA_advance_loc: 6 to 0000000000005086
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000005038
+  DW_CFA_advance_loc: 2 to 0000000000005088
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 12 to 0000000000005044
+  DW_CFA_advance_loc: 12 to 0000000000005094
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 10 to 000000000000504e
+  DW_CFA_advance_loc: 10 to 000000000000509e
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000504f
+  DW_CFA_advance_loc: 1 to 000000000000509f
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 0000000000005053
+  DW_CFA_advance_loc: 4 to 00000000000050a3
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 000000000000505a
+  DW_CFA_advance_loc: 7 to 00000000000050aa
   DW_CFA_def_cfa_offset: 176
-  DW_CFA_advance_loc2: 636 to 00000000000052d6
+  DW_CFA_advance_loc2: 636 to 0000000000005326
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 00000000000052da
+  DW_CFA_advance_loc: 4 to 000000000000532a
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000052db
+  DW_CFA_advance_loc: 1 to 000000000000532b
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000052dd
+  DW_CFA_advance_loc: 2 to 000000000000532d
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000052df
+  DW_CFA_advance_loc: 2 to 000000000000532f
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000052e1
+  DW_CFA_advance_loc: 2 to 0000000000005331
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000052e3
+  DW_CFA_advance_loc: 2 to 0000000000005333
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 13 to 00000000000052f0
+  DW_CFA_advance_loc: 13 to 0000000000005340
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000060c 0000000000000048 00000610 FDE cie=00000000 pc=0000000000002830..00000000000028ee
-  DW_CFA_advance_loc: 5 to 0000000000002835
+0000060c 0000000000000048 00000610 FDE cie=00000000 pc=0000000000002850..000000000000290e
+  DW_CFA_advance_loc: 5 to 0000000000002855
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 14 to 0000000000002843
+  DW_CFA_advance_loc: 14 to 0000000000002863
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 11 to 000000000000284e
+  DW_CFA_advance_loc: 11 to 000000000000286e
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 15 to 000000000000285d
+  DW_CFA_advance_loc: 15 to 000000000000287d
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 12 to 0000000000002869
+  DW_CFA_advance_loc: 12 to 0000000000002889
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 16 to 0000000000002879
+  DW_CFA_advance_loc: 16 to 0000000000002899
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 8 to 0000000000002881
+  DW_CFA_advance_loc: 8 to 00000000000028a1
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 22 to 0000000000002897
+  DW_CFA_advance_loc: 22 to 00000000000028b7
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 5 to 000000000000289c
+  DW_CFA_advance_loc: 5 to 00000000000028bc
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000289e
+  DW_CFA_advance_loc: 2 to 00000000000028be
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 9 to 00000000000028a7
+  DW_CFA_advance_loc: 9 to 00000000000028c7
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 8 to 00000000000028af
+  DW_CFA_advance_loc: 8 to 00000000000028cf
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 22 to 00000000000028c5
+  DW_CFA_advance_loc: 22 to 00000000000028e5
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 5 to 00000000000028ca
+  DW_CFA_advance_loc: 5 to 00000000000028ea
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000028cc
+  DW_CFA_advance_loc: 2 to 00000000000028ec
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 16 to 00000000000028dc
+  DW_CFA_advance_loc: 16 to 00000000000028fc
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 13 to 00000000000028e9
+  DW_CFA_advance_loc: 13 to 0000000000002909
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000658 0000000000000010 0000065c FDE cie=00000000 pc=0000000000005490..00000000000054a2
+00000658 0000000000000010 0000065c FDE cie=00000000 pc=00000000000054e0..00000000000054f2
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
 0000066c ZERO terminator
```

#### strings --all --bytes=8 {}

```diff
@@ -39,14 +39,15 @@
 _Z7getprobP6float2Pfm
 _Z4hashPKc
 _Z9isInArrayPPKcPci
 _Z14getArrayLengthPi
 _Z13normalizationP6float2i
 execute_circuit
 singleGateAction
+__printf_chk
 doubleGateAction
 tripleGateAction
 __stack_chk_fail
 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
 __cudaPopCallConfiguration
 _Z19actionOnSingleQubitP6float2S0_mPm
 cudaLaunchKernel
@@ -63,21 +64,24 @@
 __cudaRegisterFatBinary
 __cudaRegisterFunction
 __cudaRegisterFatBinaryEnd
 libcudart.so.11.0
 libm.so.6
 libc.so.6
 __cxa_atexit
+GLIBC_2.3.4
 GLIBC_2.4
 GLIBC_2.2.5
 []A\A]A^A_
 []A\A]A^A_
 []A\A]A^A_
 []A\A]A^A_
-Must be have two action position!
+gateName: %s
+pos_array_size = %d
+Must be have two action position!, gateName: %s
 action position must be different!
 Must be have three action position!
 _Z18actionOnTripleGateP6float2S0_mPm
 _Z19actionOnDoubleQubitP6float2S0_mPm
 _Z19actionOnSingleQubitP6float2S0_mPm
 .shstrtab
 .symtab_shndx
@@ -145,15 +149,15 @@
 qad.lo.s
 cvta.to.global
 setp.ge`
 @%p5 bra $L__BB0_2;
 TripleGate
 -60@Y8603E
 GCC: (Ubuntu 10.3.0-1ubuntu1~20.04) 10.3.0
-tmpxft_00000258_00000000-6_tgq_simulator.cudafe1.cpp
+tmpxft_00000239_00000000-6_tgq_simulator.cudafe1.cpp
 fatbinData
 _ZL26__cudaUnregisterBinaryUtilv
 _ZL20__cudaFatCubinHandle
 _ZL24__sti____cudaRegisterAllv
 _ZL15__fatDeviceText
 crtstuff.c
 deregister_tm_clones
@@ -219,14 +223,15 @@
 _Z6s_gateP6float2
 cudaMalloc@@libcudart.so.11.0
 execute_circuit
 _Z14getArrayLengthPi
 cudaLaunchKernel@@libcudart.so.11.0
 _Z11identityMatP6float2i
 _Z18actionOnTripleGateP6float2S0_mPm
+__printf_chk@@GLIBC_2.3.4
 _Z8sdg_gateP6float2
 _Z20toff_gate_target_midP6float2
 _Z6y_gateP6float2
 _Z7rx_gateP6float2f
 cudaSetDevice@@libcudart.so.11.0
 _Z7cz_gateP6float2
 __cxa_atexit@@GLIBC_2.2.5
```

#### readelf --wide --decompress --hex-dump=.gnu.hash {}

```diff
@@ -1,23 +1,23 @@
 
 Hex dump of section '.gnu.hash':
-  0x000002f0 25000000 1e000000 08000000 09000000 %...............
+  0x000002f0 25000000 1f000000 08000000 09000000 %...............
   0x00000300 00400000 30884000 081524c4 163010a2 .@..0.@...$..0..
   0x00000310 01000811 41420d02 65002092 89400848 ....AB..e. ..@.H
   0x00000320 21805322 00100018 00840000 00103000 !.S"..........0.
   0x00000330 000444a4 0000b100 01800010 02005c60 ..D...........\`
-  0x00000340 1e000000 21000000 22000000 24000000 ....!..."...$...
-  0x00000350 26000000 28000000 2a000000 2c000000 &...(...*...,...
-  0x00000360 00000000 2e000000 30000000 31000000 ........0...1...
-  0x00000370 33000000 00000000 34000000 36000000 3.......4...6...
-  0x00000380 00000000 37000000 38000000 39000000 ....7...8...9...
-  0x00000390 3b000000 3c000000 00000000 3e000000 ;...<.......>...
-  0x000003a0 00000000 3f000000 40000000 00000000 ....?...@.......
-  0x000003b0 42000000 45000000 47000000 49000000 B...E...G...I...
-  0x000003c0 00000000 00000000 4c000000 00000000 ........L.......
+  0x00000340 1f000000 22000000 23000000 25000000 ...."...#...%...
+  0x00000350 27000000 29000000 2b000000 2d000000 '...)...+...-...
+  0x00000360 00000000 2f000000 31000000 32000000 ..../...1...2...
+  0x00000370 34000000 00000000 35000000 37000000 4.......5...7...
+  0x00000380 00000000 38000000 39000000 3a000000 ....8...9...:...
+  0x00000390 3c000000 3d000000 00000000 3f000000 <...=.......?...
+  0x000003a0 00000000 40000000 41000000 00000000 ....@...A.......
+  0x000003b0 43000000 46000000 48000000 4a000000 C...F...H...J...
+  0x000003c0 00000000 00000000 4d000000 00000000 ........M.......
   0x000003d0 00000000 928053d0 00a11a24 a1b02886 ......S....$..(.
   0x000003e0 49aa77ff 4a24a498 e1047ad9 dcb2ce6d I.w.J$....z....m
   0x000003f0 dd819875 b4ef5d94 793cce5b 1033342d ...u..].y<.[.34-
   0x00000400 254a303d a6b88f28 63d80942 de760557 %J0=...(c..B.v.W
   0x00000410 efe62ce8 1c1f4a9f c18abb63 f3fd4879 ..,...J....c..Hy
   0x00000420 b069491b 7db44aa1 a9e4abfe aee000b1 .iI.}.J.........
   0x00000430 43fe3e4e 6d3eb49e 8ba54a43 75d9d7bf C.>Nm>....JCu...
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1,113 +1,114 @@
 
 Hex dump of section '.dynstr':
-  0x00000be8 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
-  0x00000bf8 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
-  0x00000c08 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
-  0x00000c18 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
-  0x00000c28 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
-  0x00000c38 6c697a65 005f5a37 636f6d70 61726550 lize._Z7compareP
-  0x00000c48 4b765330 5f005f5f 63756461 556e7265 KvS0_.__cudaUnre
-  0x00000c58 67697374 65724661 7442696e 61727900 gisterFatBinary.
-  0x00000c68 5f5a3678 5f676174 65503666 6c6f6174 _Z6x_gateP6float
-  0x00000c78 32005f5a 36795f67 61746550 36666c6f 2._Z6y_gateP6flo
-  0x00000c88 61743200 5f5a367a 5f676174 65503666 at2._Z6z_gateP6f
-  0x00000c98 6c6f6174 32005f5a 36735f67 61746550 loat2._Z6s_gateP
-  0x00000ca8 36666c6f 61743200 5f5a3873 64675f67 6float2._Z8sdg_g
-  0x00000cb8 61746550 36666c6f 61743200 5f5a3674 ateP6float2._Z6t
-  0x00000cc8 5f676174 65503666 6c6f6174 32005f5a _gateP6float2._Z
-  0x00000cd8 38746467 5f676174 65503666 6c6f6174 8tdg_gateP6float
-  0x00000ce8 32005f5a 36685f67 61746550 36666c6f 2._Z6h_gateP6flo
-  0x00000cf8 61743200 5f5a3772 785f6761 74655036 at2._Z7rx_gateP6
-  0x00000d08 666c6f61 74326600 73696e63 6f736600 float2f.sincosf.
-  0x00000d18 5f5a3772 795f6761 74655036 666c6f61 _Z7ry_gateP6floa
-  0x00000d28 74326600 5f5a3772 7a5f6761 74655036 t2f._Z7rz_gateP6
-  0x00000d38 666c6f61 74326600 5f5a3131 64616d70 float2f._Z11damp
-  0x00000d48 5f695f67 61746550 36666c6f 61743266 _i_gateP6float2f
-  0x00000d58 00737172 7466005f 5a377064 5f676174 .sqrtf._Z7pd_gat
-  0x00000d68 65503666 6c6f6174 3266005f 5a376164 eP6float2f._Z7ad
-  0x00000d78 5f676174 65503666 6c6f6174 3266005f _gateP6float2f._
-  0x00000d88 5a397377 61705f67 61746550 36666c6f Z9swap_gateP6flo
-  0x00000d98 61743200 5f5a3130 69737761 705f6761 at2._Z10iswap_ga
-  0x00000da8 74655036 666c6f61 7432005f 5a313163 teP6float2._Z11c
-  0x00000db8 70686173 655f6761 74655036 666c6f61 phase_gateP6floa
-  0x00000dc8 74326600 5f5a3231 636e6f74 5f676174 t2f._Z21cnot_gat
-  0x00000dd8 655f636f 6e74726f 6c5f6269 67503666 e_control_bigP6f
-  0x00000de8 6c6f6174 32005f5a 3233636e 6f745f67 loat2._Z23cnot_g
-  0x00000df8 6174655f 636f6e74 726f6c5f 736d616c ate_control_smal
-  0x00000e08 6c503666 6c6f6174 32005f5a 37637a5f lP6float2._Z7cz_
-  0x00000e18 67617465 5036666c 6f617432 005f5a38 gateP6float2._Z8
-  0x00000e28 7278785f 67617465 5036666c 6f617432 rxx_gateP6float2
-  0x00000e38 66005f5a 38727979 5f676174 65503666 f._Z8ryy_gateP6f
-  0x00000e48 6c6f6174 3266005f 5a38727a 7a5f6761 loat2f._Z8rzz_ga
-  0x00000e58 74655036 666c6f61 74326600 5f5a3873 teP6float2f._Z8s
-  0x00000e68 79635f67 61746550 36666c6f 61743200 yc_gateP6float2.
-  0x00000e78 5f5a3232 746f6666 5f676174 655f7461 _Z22toff_gate_ta
-  0x00000e88 72676574 5f736d61 6c6c5036 666c6f61 rget_smallP6floa
-  0x00000e98 7432005f 5a323074 6f66665f 67617465 t2._Z20toff_gate
-  0x00000ea8 5f746172 6765745f 6d696450 36666c6f _target_midP6flo
-  0x00000eb8 61743200 5f5a3230 746f6666 5f676174 at2._Z20toff_gat
-  0x00000ec8 655f7461 72676574 5f626967 5036666c e_target_bigP6fl
-  0x00000ed8 6f617432 005f5a32 31667265 645f6761 oat2._Z21fred_ga
-  0x00000ee8 74655f63 6f6e7472 6f6c5f62 69675036 te_control_bigP6
-  0x00000ef8 666c6f61 7432005f 5a323166 7265645f float2._Z21fred_
-  0x00000f08 67617465 5f636f6e 74726f6c 5f6d6964 gate_control_mid
-  0x00000f18 5036666c 6f617432 005f5a32 33667265 P6float2._Z23fre
-  0x00000f28 645f6761 74655f63 6f6e7472 6f6c5f73 d_gate_control_s
-  0x00000f38 6d616c6c 5036666c 6f617432 005f5a31 mallP6float2._Z1
-  0x00000f48 31696465 6e746974 794d6174 5036666c 1identityMatP6fl
-  0x00000f58 6f617432 69005f5a 32306765 6e657261 oat2i._Z20genera
-  0x00000f68 74655f62 696e6172 795f6461 74616600 te_binary_dataf.
-  0x00000f78 74696d65 00737261 6e64005f 5a376765 time.srand._Z7ge
-  0x00000f88 7470726f 62503666 6c6f6174 3250666d tprobP6float2Pfm
-  0x00000f98 005f5a34 68617368 504b6300 5f5a3969 ._Z4hashPKc._Z9i
-  0x00000fa8 73496e41 72726179 50504b63 50636900 sInArrayPPKcPci.
-  0x00000fb8 73747263 6d70005f 5a313467 65744172 strcmp._Z14getAr
-  0x00000fc8 7261794c 656e6774 68506900 5f5a3133 rayLengthPi._Z13
-  0x00000fd8 6e6f726d 616c697a 6174696f 6e503666 normalizationP6f
-  0x00000fe8 6c6f6174 32690065 78656375 74655f63 loat2i.execute_c
-  0x00000ff8 69726375 69740073 696e676c 65476174 ircuit.singleGat
-  0x00001008 65416374 696f6e00 646f7562 6c654761 eAction.doubleGa
-  0x00001018 74654163 74696f6e 00747269 706c6547 teAction.tripleG
-  0x00001028 61746541 6374696f 6e005f5f 73746163 ateAction.__stac
-  0x00001038 6b5f6368 6b5f6661 696c005f 5a35315f k_chk_fail._Z51_
-  0x00001048 5f646576 6963655f 73747562 5f5f5a31 _device_stub__Z1
-  0x00001058 39616374 696f6e4f 6e53696e 676c6551 9actionOnSingleQ
-  0x00001068 75626974 5036666c 6f617432 53305f6d ubitP6float2S0_m
-  0x00001078 506d5036 666c6f61 74325330 5f6d506d PmP6float2S0_mPm
-  0x00001088 005f5f63 75646150 6f704361 6c6c436f .__cudaPopCallCo
-  0x00001098 6e666967 75726174 696f6e00 5f5a3139 nfiguration._Z19
-  0x000010a8 61637469 6f6e4f6e 53696e67 6c655175 actionOnSingleQu
-  0x000010b8 62697450 36666c6f 61743253 305f6d50 bitP6float2S0_mP
-  0x000010c8 6d006375 64614c61 756e6368 4b65726e m.cudaLaunchKern
-  0x000010d8 656c0063 75646153 65744465 76696365 el.cudaSetDevice
-  0x000010e8 006d616c 6c6f6300 63756461 4d616c6c .malloc.cudaMall
-  0x000010f8 6f630063 7564614d 656d6370 79005f5f oc.cudaMemcpy.__
-  0x00001108 63756461 50757368 43616c6c 436f6e66 cudaPushCallConf
-  0x00001118 69677572 6174696f 6e006375 64614465 iguration.cudaDe
-  0x00001128 76696365 53796e63 68726f6e 697a6500 viceSynchronize.
-  0x00001138 63756461 46726565 00667265 65005f5a cudaFree.free._Z
-  0x00001148 35315f5f 64657669 63655f73 7475625f 51__device_stub_
-  0x00001158 5f5a3139 61637469 6f6e4f6e 446f7562 _Z19actionOnDoub
-  0x00001168 6c655175 62697450 36666c6f 61743253 leQubitP6float2S
-  0x00001178 305f6d50 6d503666 6c6f6174 3253305f 0_mPmP6float2S0_
-  0x00001188 6d506d00 5f5a3139 61637469 6f6e4f6e mPm._Z19actionOn
-  0x00001198 446f7562 6c655175 62697450 36666c6f DoubleQubitP6flo
-  0x000011a8 61743253 305f6d50 6d007173 6f727400 at2S0_mPm.qsort.
-  0x000011b8 70757473 005f5a35 305f5f64 65766963 puts._Z50__devic
-  0x000011c8 655f7374 75625f5f 5a313861 6374696f e_stub__Z18actio
-  0x000011d8 6e4f6e54 7269706c 65476174 65503666 nOnTripleGateP6f
-  0x000011e8 6c6f6174 3253305f 6d506d50 36666c6f loat2S0_mPmP6flo
-  0x000011f8 61743253 305f6d50 6d005f5a 31386163 at2S0_mPm._Z18ac
-  0x00001208 74696f6e 4f6e5472 69706c65 47617465 tionOnTripleGate
-  0x00001218 5036666c 6f617432 53305f6d 506d005f P6float2S0_mPm._
-  0x00001228 5f637564 61526567 69737465 72466174 _cudaRegisterFat
-  0x00001238 42696e61 7279005f 5f637564 61526567 Binary.__cudaReg
-  0x00001248 69737465 7246756e 6374696f 6e005f5f isterFunction.__
-  0x00001258 63756461 52656769 73746572 46617442 cudaRegisterFatB
-  0x00001268 696e6172 79456e64 006c6962 63756461 inaryEnd.libcuda
-  0x00001278 72742e73 6f2e3131 2e30006c 69626d2e rt.so.11.0.libm.
-  0x00001288 736f2e36 006c6962 632e736f 2e36005f so.6.libc.so.6._
-  0x00001298 5f637861 5f617465 78697400 474c4942 _cxa_atexit.GLIB
-  0x000012a8 435f322e 3400474c 4942435f 322e322e C_2.4.GLIBC_2.2.
-  0x000012b8 3500                                5.
+  0x00000c00 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
+  0x00000c10 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
+  0x00000c20 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
+  0x00000c30 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
+  0x00000c40 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
+  0x00000c50 6c697a65 005f5a37 636f6d70 61726550 lize._Z7compareP
+  0x00000c60 4b765330 5f005f5f 63756461 556e7265 KvS0_.__cudaUnre
+  0x00000c70 67697374 65724661 7442696e 61727900 gisterFatBinary.
+  0x00000c80 5f5a3678 5f676174 65503666 6c6f6174 _Z6x_gateP6float
+  0x00000c90 32005f5a 36795f67 61746550 36666c6f 2._Z6y_gateP6flo
+  0x00000ca0 61743200 5f5a367a 5f676174 65503666 at2._Z6z_gateP6f
+  0x00000cb0 6c6f6174 32005f5a 36735f67 61746550 loat2._Z6s_gateP
+  0x00000cc0 36666c6f 61743200 5f5a3873 64675f67 6float2._Z8sdg_g
+  0x00000cd0 61746550 36666c6f 61743200 5f5a3674 ateP6float2._Z6t
+  0x00000ce0 5f676174 65503666 6c6f6174 32005f5a _gateP6float2._Z
+  0x00000cf0 38746467 5f676174 65503666 6c6f6174 8tdg_gateP6float
+  0x00000d00 32005f5a 36685f67 61746550 36666c6f 2._Z6h_gateP6flo
+  0x00000d10 61743200 5f5a3772 785f6761 74655036 at2._Z7rx_gateP6
+  0x00000d20 666c6f61 74326600 73696e63 6f736600 float2f.sincosf.
+  0x00000d30 5f5a3772 795f6761 74655036 666c6f61 _Z7ry_gateP6floa
+  0x00000d40 74326600 5f5a3772 7a5f6761 74655036 t2f._Z7rz_gateP6
+  0x00000d50 666c6f61 74326600 5f5a3131 64616d70 float2f._Z11damp
+  0x00000d60 5f695f67 61746550 36666c6f 61743266 _i_gateP6float2f
+  0x00000d70 00737172 7466005f 5a377064 5f676174 .sqrtf._Z7pd_gat
+  0x00000d80 65503666 6c6f6174 3266005f 5a376164 eP6float2f._Z7ad
+  0x00000d90 5f676174 65503666 6c6f6174 3266005f _gateP6float2f._
+  0x00000da0 5a397377 61705f67 61746550 36666c6f Z9swap_gateP6flo
+  0x00000db0 61743200 5f5a3130 69737761 705f6761 at2._Z10iswap_ga
+  0x00000dc0 74655036 666c6f61 7432005f 5a313163 teP6float2._Z11c
+  0x00000dd0 70686173 655f6761 74655036 666c6f61 phase_gateP6floa
+  0x00000de0 74326600 5f5a3231 636e6f74 5f676174 t2f._Z21cnot_gat
+  0x00000df0 655f636f 6e74726f 6c5f6269 67503666 e_control_bigP6f
+  0x00000e00 6c6f6174 32005f5a 3233636e 6f745f67 loat2._Z23cnot_g
+  0x00000e10 6174655f 636f6e74 726f6c5f 736d616c ate_control_smal
+  0x00000e20 6c503666 6c6f6174 32005f5a 37637a5f lP6float2._Z7cz_
+  0x00000e30 67617465 5036666c 6f617432 005f5a38 gateP6float2._Z8
+  0x00000e40 7278785f 67617465 5036666c 6f617432 rxx_gateP6float2
+  0x00000e50 66005f5a 38727979 5f676174 65503666 f._Z8ryy_gateP6f
+  0x00000e60 6c6f6174 3266005f 5a38727a 7a5f6761 loat2f._Z8rzz_ga
+  0x00000e70 74655036 666c6f61 74326600 5f5a3873 teP6float2f._Z8s
+  0x00000e80 79635f67 61746550 36666c6f 61743200 yc_gateP6float2.
+  0x00000e90 5f5a3232 746f6666 5f676174 655f7461 _Z22toff_gate_ta
+  0x00000ea0 72676574 5f736d61 6c6c5036 666c6f61 rget_smallP6floa
+  0x00000eb0 7432005f 5a323074 6f66665f 67617465 t2._Z20toff_gate
+  0x00000ec0 5f746172 6765745f 6d696450 36666c6f _target_midP6flo
+  0x00000ed0 61743200 5f5a3230 746f6666 5f676174 at2._Z20toff_gat
+  0x00000ee0 655f7461 72676574 5f626967 5036666c e_target_bigP6fl
+  0x00000ef0 6f617432 005f5a32 31667265 645f6761 oat2._Z21fred_ga
+  0x00000f00 74655f63 6f6e7472 6f6c5f62 69675036 te_control_bigP6
+  0x00000f10 666c6f61 7432005f 5a323166 7265645f float2._Z21fred_
+  0x00000f20 67617465 5f636f6e 74726f6c 5f6d6964 gate_control_mid
+  0x00000f30 5036666c 6f617432 005f5a32 33667265 P6float2._Z23fre
+  0x00000f40 645f6761 74655f63 6f6e7472 6f6c5f73 d_gate_control_s
+  0x00000f50 6d616c6c 5036666c 6f617432 005f5a31 mallP6float2._Z1
+  0x00000f60 31696465 6e746974 794d6174 5036666c 1identityMatP6fl
+  0x00000f70 6f617432 69005f5a 32306765 6e657261 oat2i._Z20genera
+  0x00000f80 74655f62 696e6172 795f6461 74616600 te_binary_dataf.
+  0x00000f90 74696d65 00737261 6e64005f 5a376765 time.srand._Z7ge
+  0x00000fa0 7470726f 62503666 6c6f6174 3250666d tprobP6float2Pfm
+  0x00000fb0 005f5a34 68617368 504b6300 5f5a3969 ._Z4hashPKc._Z9i
+  0x00000fc0 73496e41 72726179 50504b63 50636900 sInArrayPPKcPci.
+  0x00000fd0 73747263 6d70005f 5a313467 65744172 strcmp._Z14getAr
+  0x00000fe0 7261794c 656e6774 68506900 5f5a3133 rayLengthPi._Z13
+  0x00000ff0 6e6f726d 616c697a 6174696f 6e503666 normalizationP6f
+  0x00001000 6c6f6174 32690065 78656375 74655f63 loat2i.execute_c
+  0x00001010 69726375 69740073 696e676c 65476174 ircuit.singleGat
+  0x00001020 65416374 696f6e00 5f5f7072 696e7466 eAction.__printf
+  0x00001030 5f63686b 00646f75 626c6547 61746541 _chk.doubleGateA
+  0x00001040 6374696f 6e007472 69706c65 47617465 ction.tripleGate
+  0x00001050 41637469 6f6e005f 5f737461 636b5f63 Action.__stack_c
+  0x00001060 686b5f66 61696c00 5f5a3531 5f5f6465 hk_fail._Z51__de
+  0x00001070 76696365 5f737475 625f5f5a 31396163 vice_stub__Z19ac
+  0x00001080 74696f6e 4f6e5369 6e676c65 51756269 tionOnSingleQubi
+  0x00001090 74503666 6c6f6174 3253305f 6d506d50 tP6float2S0_mPmP
+  0x000010a0 36666c6f 61743253 305f6d50 6d005f5f 6float2S0_mPm.__
+  0x000010b0 63756461 506f7043 616c6c43 6f6e6669 cudaPopCallConfi
+  0x000010c0 67757261 74696f6e 005f5a31 39616374 guration._Z19act
+  0x000010d0 696f6e4f 6e53696e 676c6551 75626974 ionOnSingleQubit
+  0x000010e0 5036666c 6f617432 53305f6d 506d0063 P6float2S0_mPm.c
+  0x000010f0 7564614c 61756e63 684b6572 6e656c00 udaLaunchKernel.
+  0x00001100 63756461 53657444 65766963 65006d61 cudaSetDevice.ma
+  0x00001110 6c6c6f63 00637564 614d616c 6c6f6300 lloc.cudaMalloc.
+  0x00001120 63756461 4d656d63 7079005f 5f637564 cudaMemcpy.__cud
+  0x00001130 61507573 6843616c 6c436f6e 66696775 aPushCallConfigu
+  0x00001140 72617469 6f6e0063 75646144 65766963 ration.cudaDevic
+  0x00001150 6553796e 6368726f 6e697a65 00637564 eSynchronize.cud
+  0x00001160 61467265 65006672 6565005f 5a35315f aFree.free._Z51_
+  0x00001170 5f646576 6963655f 73747562 5f5f5a31 _device_stub__Z1
+  0x00001180 39616374 696f6e4f 6e446f75 626c6551 9actionOnDoubleQ
+  0x00001190 75626974 5036666c 6f617432 53305f6d ubitP6float2S0_m
+  0x000011a0 506d5036 666c6f61 74325330 5f6d506d PmP6float2S0_mPm
+  0x000011b0 005f5a31 39616374 696f6e4f 6e446f75 ._Z19actionOnDou
+  0x000011c0 626c6551 75626974 5036666c 6f617432 bleQubitP6float2
+  0x000011d0 53305f6d 506d0071 736f7274 00707574 S0_mPm.qsort.put
+  0x000011e0 73005f5a 35305f5f 64657669 63655f73 s._Z50__device_s
+  0x000011f0 7475625f 5f5a3138 61637469 6f6e4f6e tub__Z18actionOn
+  0x00001200 54726970 6c654761 74655036 666c6f61 TripleGateP6floa
+  0x00001210 74325330 5f6d506d 5036666c 6f617432 t2S0_mPmP6float2
+  0x00001220 53305f6d 506d005f 5a313861 6374696f S0_mPm._Z18actio
+  0x00001230 6e4f6e54 7269706c 65476174 65503666 nOnTripleGateP6f
+  0x00001240 6c6f6174 3253305f 6d506d00 5f5f6375 loat2S0_mPm.__cu
+  0x00001250 64615265 67697374 65724661 7442696e daRegisterFatBin
+  0x00001260 61727900 5f5f6375 64615265 67697374 ary.__cudaRegist
+  0x00001270 65724675 6e637469 6f6e005f 5f637564 erFunction.__cud
+  0x00001280 61526567 69737465 72466174 42696e61 aRegisterFatBina
+  0x00001290 7279456e 64006c69 62637564 6172742e ryEnd.libcudart.
+  0x000012a0 736f2e31 312e3000 6c69626d 2e736f2e so.11.0.libm.so.
+  0x000012b0 36006c69 62632e73 6f2e3600 5f5f6378 6.libc.so.6.__cx
+  0x000012c0 615f6174 65786974 00474c49 42435f32 a_atexit.GLIBC_2
+  0x000012d0 2e332e34 00474c49 42435f32 2e340047 .3.4.GLIBC_2.4.G
+  0x000012e0 4c494243 5f322e32 2e3500            LIBC_2.2.5.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -251,7 +251,11 @@
 	push   $0x3c
 	bnd jmp 2020 <.plt>
 	nop
 	endbr64
 	push   $0x3d
 	bnd jmp 2020 <.plt>
 	nop
+	endbr64
+	push   $0x3e
+	bnd jmp 2020 <.plt>
+	nop
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.got {}

```diff
@@ -1,24 +1,24 @@
 
 
 
 Disassembly of section .plt.got:
 
-0000000000002410 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>:
+0000000000002420 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>:
 	endbr64
-	bnd jmp *0xbbad(%rip)        
+	bnd jmp *0xbb9d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002420 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)@plt>:
+0000000000002430 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)@plt>:
 	endbr64
-	bnd jmp *0xbbad(%rip)        
+	bnd jmp *0xbb9d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002430 <__cxa_finalize@plt>:
+0000000000002440 <__cxa_finalize@plt>:
 	endbr64
-	bnd jmp *0xbbb5(%rip)        
+	bnd jmp *0xbba5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002440 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>:
+0000000000002450 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>:
 	endbr64
-	bnd jmp *0xbbad(%rip)        
+	bnd jmp *0xbb9d(%rip)        
 	nopl   0x0(%rax,%rax,1)
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.sec {}

```diff
@@ -1,314 +1,319 @@
 
 
 
 Disassembly of section .plt.sec:
 
-0000000000002450 <rxx_gate(float2*, float)@plt>:
-	endbr64
-	bnd jmp *0xbbbd(%rip)        
-	nopl   0x0(%rax,%rax,1)
-
-0000000000002460 <sincosf@plt>:
-	endbr64
-	bnd jmp *0xbbb5(%rip)        
-	nopl   0x0(%rax,%rax,1)
-
-0000000000002470 <ry_gate(float2*, float)@plt>:
+0000000000002460 <rxx_gate(float2*, float)@plt>:
 	endbr64
 	bnd jmp *0xbbad(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002480 <free@plt>:
+0000000000002470 <sincosf@plt>:
 	endbr64
 	bnd jmp *0xbba5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002490 <__cudaUnregisterFatBinary@plt>:
+0000000000002480 <ry_gate(float2*, float)@plt>:
 	endbr64
 	bnd jmp *0xbb9d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000024a0 <fred_gate_control_small(float2*)@plt>:
+0000000000002490 <free@plt>:
 	endbr64
 	bnd jmp *0xbb95(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000024b0 <t_gate(float2*)@plt>:
+00000000000024a0 <__cudaUnregisterFatBinary@plt>:
 	endbr64
 	bnd jmp *0xbb8d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000024c0 <__cudaRegisterFatBinary@plt>:
+00000000000024b0 <fred_gate_control_small(float2*)@plt>:
 	endbr64
 	bnd jmp *0xbb85(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000024d0 <pd_gate(float2*, float)@plt>:
+00000000000024c0 <t_gate(float2*)@plt>:
 	endbr64
 	bnd jmp *0xbb7d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000024e0 <puts@plt>:
+00000000000024d0 <__cudaRegisterFatBinary@plt>:
 	endbr64
 	bnd jmp *0xbb75(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000024f0 <qsort@plt>:
+00000000000024e0 <pd_gate(float2*, float)@plt>:
 	endbr64
 	bnd jmp *0xbb6d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002500 <cnot_gate_control_small(float2*)@plt>:
+00000000000024f0 <puts@plt>:
 	endbr64
 	bnd jmp *0xbb65(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002510 <ryy_gate(float2*, float)@plt>:
+0000000000002500 <qsort@plt>:
 	endbr64
 	bnd jmp *0xbb5d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002520 <isInArray(char const**, char*, int)@plt>:
+0000000000002510 <cnot_gate_control_small(float2*)@plt>:
 	endbr64
 	bnd jmp *0xbb55(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002530 <rzz_gate(float2*, float)@plt>:
+0000000000002520 <ryy_gate(float2*, float)@plt>:
 	endbr64
 	bnd jmp *0xbb4d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002540 <__stack_chk_fail@plt>:
+0000000000002530 <isInArray(char const**, char*, int)@plt>:
 	endbr64
 	bnd jmp *0xbb45(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002550 <z_gate(float2*)@plt>:
+0000000000002540 <rzz_gate(float2*, float)@plt>:
 	endbr64
 	bnd jmp *0xbb3d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002560 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>:
+0000000000002550 <__stack_chk_fail@plt>:
 	endbr64
 	bnd jmp *0xbb35(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002570 <h_gate(float2*)@plt>:
+0000000000002560 <z_gate(float2*)@plt>:
 	endbr64
 	bnd jmp *0xbb2d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002580 <cudaFree@plt>:
+0000000000002570 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>:
 	endbr64
 	bnd jmp *0xbb25(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002590 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>:
+0000000000002580 <h_gate(float2*)@plt>:
 	endbr64
 	bnd jmp *0xbb1d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000025a0 <cudaMemcpy@plt>:
+0000000000002590 <cudaFree@plt>:
 	endbr64
 	bnd jmp *0xbb15(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000025b0 <srand@plt>:
+00000000000025a0 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>:
 	endbr64
 	bnd jmp *0xbb0d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000025c0 <toff_gate_target_small(float2*)@plt>:
+00000000000025b0 <cudaMemcpy@plt>:
 	endbr64
 	bnd jmp *0xbb05(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000025d0 <__cudaRegisterFunction@plt>:
+00000000000025c0 <srand@plt>:
 	endbr64
 	bnd jmp *0xbafd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000025e0 <strcmp@plt>:
+00000000000025d0 <toff_gate_target_small(float2*)@plt>:
 	endbr64
 	bnd jmp *0xbaf5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000025f0 <fred_gate_control_big(float2*)@plt>:
+00000000000025e0 <__cudaRegisterFunction@plt>:
 	endbr64
 	bnd jmp *0xbaed(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002600 <cudaDeviceSynchronize@plt>:
+00000000000025f0 <strcmp@plt>:
 	endbr64
 	bnd jmp *0xbae5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002610 <toff_gate_target_big(float2*)@plt>:
+0000000000002600 <fred_gate_control_big(float2*)@plt>:
 	endbr64
 	bnd jmp *0xbadd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002620 <time@plt>:
+0000000000002610 <cudaDeviceSynchronize@plt>:
 	endbr64
 	bnd jmp *0xbad5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002630 <damp_i_gate(float2*, float)@plt>:
+0000000000002620 <toff_gate_target_big(float2*)@plt>:
 	endbr64
 	bnd jmp *0xbacd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002640 <sqrtf@plt>:
+0000000000002630 <time@plt>:
 	endbr64
 	bnd jmp *0xbac5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002650 <iswap_gate(float2*)@plt>:
+0000000000002640 <damp_i_gate(float2*, float)@plt>:
 	endbr64
 	bnd jmp *0xbabd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002660 <cnot_gate_control_big(float2*)@plt>:
+0000000000002650 <sqrtf@plt>:
 	endbr64
 	bnd jmp *0xbab5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002670 <rz_gate(float2*, float)@plt>:
+0000000000002660 <iswap_gate(float2*)@plt>:
 	endbr64
 	bnd jmp *0xbaad(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002680 <tdg_gate(float2*)@plt>:
+0000000000002670 <cnot_gate_control_big(float2*)@plt>:
 	endbr64
 	bnd jmp *0xbaa5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002690 <swap_gate(float2*)@plt>:
+0000000000002680 <rz_gate(float2*, float)@plt>:
 	endbr64
 	bnd jmp *0xba9d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000026a0 <malloc@plt>:
+0000000000002690 <tdg_gate(float2*)@plt>:
 	endbr64
 	bnd jmp *0xba95(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000026b0 <normalization(float2*, int)@plt>:
+00000000000026a0 <swap_gate(float2*)@plt>:
 	endbr64
 	bnd jmp *0xba8d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000026c0 <s_gate(float2*)@plt>:
+00000000000026b0 <malloc@plt>:
 	endbr64
 	bnd jmp *0xba85(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000026d0 <cudaMalloc@plt>:
+00000000000026c0 <normalization(float2*, int)@plt>:
 	endbr64
 	bnd jmp *0xba7d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000026e0 <getArrayLength(int*)@plt>:
+00000000000026d0 <s_gate(float2*)@plt>:
 	endbr64
 	bnd jmp *0xba75(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000026f0 <cudaLaunchKernel@plt>:
+00000000000026e0 <cudaMalloc@plt>:
 	endbr64
 	bnd jmp *0xba6d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002700 <sdg_gate(float2*)@plt>:
+00000000000026f0 <getArrayLength(int*)@plt>:
 	endbr64
 	bnd jmp *0xba65(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002710 <toff_gate_target_mid(float2*)@plt>:
+0000000000002700 <cudaLaunchKernel@plt>:
 	endbr64
 	bnd jmp *0xba5d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002720 <y_gate(float2*)@plt>:
+0000000000002710 <__printf_chk@plt>:
 	endbr64
 	bnd jmp *0xba55(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002730 <rx_gate(float2*, float)@plt>:
+0000000000002720 <sdg_gate(float2*)@plt>:
 	endbr64
 	bnd jmp *0xba4d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002740 <cudaSetDevice@plt>:
+0000000000002730 <toff_gate_target_mid(float2*)@plt>:
 	endbr64
 	bnd jmp *0xba45(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002750 <cz_gate(float2*)@plt>:
+0000000000002740 <y_gate(float2*)@plt>:
 	endbr64
 	bnd jmp *0xba3d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002760 <__cxa_atexit@plt>:
+0000000000002750 <rx_gate(float2*, float)@plt>:
 	endbr64
 	bnd jmp *0xba35(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002770 <fred_gate_control_mid(float2*)@plt>:
+0000000000002760 <cudaSetDevice@plt>:
 	endbr64
 	bnd jmp *0xba2d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002780 <exit@plt>:
+0000000000002770 <cz_gate(float2*)@plt>:
 	endbr64
 	bnd jmp *0xba25(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002790 <hash(char const*)@plt>:
+0000000000002780 <__cxa_atexit@plt>:
 	endbr64
 	bnd jmp *0xba1d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000027a0 <syc_gate(float2*)@plt>:
+0000000000002790 <fred_gate_control_mid(float2*)@plt>:
 	endbr64
 	bnd jmp *0xba15(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000027b0 <__cudaPushCallConfiguration@plt>:
+00000000000027a0 <exit@plt>:
 	endbr64
 	bnd jmp *0xba0d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000027c0 <__cudaRegisterFatBinaryEnd@plt>:
+00000000000027b0 <hash(char const*)@plt>:
 	endbr64
 	bnd jmp *0xba05(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000027d0 <cphase_gate(float2*, float)@plt>:
+00000000000027c0 <syc_gate(float2*)@plt>:
 	endbr64
 	bnd jmp *0xb9fd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000027e0 <ad_gate(float2*, float)@plt>:
+00000000000027d0 <__cudaPushCallConfiguration@plt>:
 	endbr64
 	bnd jmp *0xb9f5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000027f0 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>:
+00000000000027e0 <__cudaRegisterFatBinaryEnd@plt>:
 	endbr64
 	bnd jmp *0xb9ed(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002800 <rand@plt>:
+00000000000027f0 <cphase_gate(float2*, float)@plt>:
 	endbr64
 	bnd jmp *0xb9e5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002810 <__cudaPopCallConfiguration@plt>:
+0000000000002800 <ad_gate(float2*, float)@plt>:
 	endbr64
 	bnd jmp *0xb9dd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002820 <x_gate(float2*)@plt>:
+0000000000002810 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>:
 	endbr64
 	bnd jmp *0xb9d5(%rip)        
 	nopl   0x0(%rax,%rax,1)
+
+0000000000002820 <rand@plt>:
+	endbr64
+	bnd jmp *0xb9cd(%rip)        
+	nopl   0x0(%rax,%rax,1)
+
+0000000000002830 <__cudaPopCallConfiguration@plt>:
+	endbr64
+	bnd jmp *0xb9c5(%rip)        
+	nopl   0x0(%rax,%rax,1)
+
+0000000000002840 <x_gate(float2*)@plt>:
+	endbr64
+	bnd jmp *0xb9bd(%rip)        
+	nopl   0x0(%rax,%rax,1)
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1,432 +1,432 @@
 
 
 
 Disassembly of section .text:
 
-0000000000002830 <__sti____cudaRegisterAll()>:
+0000000000002850 <__sti____cudaRegisterAll()>:
 __sti____cudaRegisterAll():
 	endbr64
 	push   %rbp
-	lea    0xb9d4(%rip),%rdi        
-	call   24c0 <__cudaRegisterFatBinary@plt>
+	lea    0xb9bc(%rip),%rdi        
+	call   24d0 <__cudaRegisterFatBinary@plt>
 	push   $0x0
 	xor    %r9d,%r9d
 	mov    $0xffffffff,%r8d
 	push   $0x0
-	lea    0x38c3(%rip),%rcx        
+	lea    0x38d3(%rip),%rcx        
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	push   $0x0
-	mov    0xb774(%rip),%rsi        
+	mov    0xb754(%rip),%rsi        
 	mov    %rcx,%rdx
 	push   $0x0
-	mov    %rax,0xb9c0(%rip)        
-	call   25d0 <__cudaRegisterFunction@plt>
+	mov    %rax,0xb9a8(%rip)        
+	call   25e0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
-	lea    0x38b8(%rip),%rcx        
-	mov    0xb739(%rip),%rsi        
+	lea    0x38c8(%rip),%rcx        
+	mov    0xb719(%rip),%rsi        
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
-	call   25d0 <__cudaRegisterFunction@plt>
+	call   25e0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
-	lea    0x38b2(%rip),%rcx        
-	mov    0xb73b(%rip),%rsi        
+	lea    0x38c2(%rip),%rcx        
+	mov    0xb71b(%rip),%rsi        
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
-	call   25d0 <__cudaRegisterFunction@plt>
-	mov    0xb958(%rip),%rdi        
+	call   25e0 <__cudaRegisterFunction@plt>
+	mov    0xb940(%rip),%rdi        
 	add    $0x20,%rsp
-	call   27c0 <__cudaRegisterFatBinaryEnd@plt>
+	call   27e0 <__cudaRegisterFatBinaryEnd@plt>
 	lea    0xd8(%rip),%rdi        
 	pop    %rbp
-	jmp    5490 <atexit>
+	jmp    54e0 <atexit>
 	xchg   %ax,%ax
 
-00000000000028f0 <deregister_tm_clones>:
+0000000000002910 <deregister_tm_clones>:
 deregister_tm_clones():
-	lea    0xb919(%rip),%rdi        
-	lea    0xb912(%rip),%rax        
+	lea    0xb901(%rip),%rdi        
+	lea    0xb8fa(%rip),%rax        
 	cmp    %rdi,%rax
-	je     2918 <deregister_tm_clones+0x28>
-	mov    0xb69e(%rip),%rax        
+	je     2938 <deregister_tm_clones+0x28>
+	mov    0xb67e(%rip),%rax        
 	test   %rax,%rax
-	je     2918 <deregister_tm_clones+0x28>
+	je     2938 <deregister_tm_clones+0x28>
 	jmp    *%rax
 	nopl   0x0(%rax)
 	ret
 	nopl   0x0(%rax)
 
-0000000000002920 <register_tm_clones>:
+0000000000002940 <register_tm_clones>:
 register_tm_clones():
-	lea    0xb8e9(%rip),%rdi        
-	lea    0xb8e2(%rip),%rsi        
+	lea    0xb8d1(%rip),%rdi        
+	lea    0xb8ca(%rip),%rsi        
 	sub    %rdi,%rsi
 	mov    %rsi,%rax
 	shr    $0x3f,%rsi
 	sar    $0x3,%rax
 	add    %rax,%rsi
 	sar    $1,%rsi
-	je     2958 <register_tm_clones+0x38>
-	mov    0xb695(%rip),%rax        
+	je     2978 <register_tm_clones+0x38>
+	mov    0xb675(%rip),%rax        
 	test   %rax,%rax
-	je     2958 <register_tm_clones+0x38>
+	je     2978 <register_tm_clones+0x38>
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
 	ret
 	nopl   0x0(%rax)
 
-0000000000002960 <__do_global_dtors_aux>:
+0000000000002980 <__do_global_dtors_aux>:
 __do_global_dtors_aux():
 	endbr64
-	cmpb   $0x0,0xb8bd(%rip)        
-	jne    2998 <__do_global_dtors_aux+0x38>
+	cmpb   $0x0,0xb8a5(%rip)        
+	jne    29b8 <__do_global_dtors_aux+0x38>
 	push   %rbp
-	cmpq   $0x0,0xb67a(%rip)        
+	cmpq   $0x0,0xb65a(%rip)        
 	mov    %rsp,%rbp
-	je     2987 <__do_global_dtors_aux+0x27>
-	mov    0xb886(%rip),%rdi        
-	call   2430 <__cxa_finalize@plt>
-	call   28f0 <deregister_tm_clones>
-	movb   $0x1,0xb895(%rip)        
+	je     29a7 <__do_global_dtors_aux+0x27>
+	mov    0xb86e(%rip),%rdi        
+	call   2440 <__cxa_finalize@plt>
+	call   2910 <deregister_tm_clones>
+	movb   $0x1,0xb87d(%rip)        
 	pop    %rbp
 	ret
 	nopl   (%rax)
 	ret
 	nopl   0x0(%rax)
 
-00000000000029a0 <frame_dummy>:
+00000000000029c0 <frame_dummy>:
 frame_dummy():
 	endbr64
-	jmp    2920 <register_tm_clones>
+	jmp    2940 <register_tm_clones>
 	nopl   0x0(%rax)
 
-00000000000029b0 <compare(void const*, void const*)>:
+00000000000029d0 <compare(void const*, void const*)>:
 compare(void const*, void const*):
 	endbr64
 	mov    (%rdi),%eax
 	sub    (%rsi),%eax
 	ret
 	nopl   0x0(%rax)
 
-00000000000029c0 <__cudaUnregisterBinaryUtil()>:
+00000000000029e0 <__cudaUnregisterBinaryUtil()>:
 __cudaUnregisterBinaryUtil():
 	endbr64
-	mov    0xb865(%rip),%rdi        
-	jmp    2490 <__cudaUnregisterFatBinary@plt>
+	mov    0xb84d(%rip),%rdi        
+	jmp    24a0 <__cudaUnregisterFatBinary@plt>
 
-00000000000029d0 <x_gate(float2*)>:
+00000000000029f0 <x_gate(float2*)>:
 x_gate(float2*):
 	endbr64
-	movaps 0x37b5(%rip),%xmm0        
+	movaps 0x37c5(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movss  0x37ba(%rip),%xmm0        
+	movss  0x37ca(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-00000000000029f0 <y_gate(float2*)>:
+0000000000002a10 <y_gate(float2*)>:
 y_gate(float2*):
 	endbr64
-	movaps 0x37b5(%rip),%xmm0        
+	movaps 0x37c5(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x37bb(%rip),%xmm0        
+	movaps 0x37cb(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-0000000000002a10 <z_gate(float2*)>:
+0000000000002a30 <z_gate(float2*)>:
 z_gate(float2*):
 	endbr64
-	movss  0x3784(%rip),%xmm0        
+	movss  0x3794(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x37aa(%rip),%xmm0        
+	movaps 0x37ba(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002a30 <s_gate(float2*)>:
+0000000000002a50 <s_gate(float2*)>:
 s_gate(float2*):
 	endbr64
-	movss  0x3764(%rip),%xmm0        
+	movss  0x3774(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x379a(%rip),%xmm0        
+	movaps 0x37aa(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002a50 <sdg_gate(float2*)>:
+0000000000002a70 <sdg_gate(float2*)>:
 sdg_gate(float2*):
 	endbr64
-	movss  0x3744(%rip),%xmm0        
+	movss  0x3754(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x374a(%rip),%xmm0        
+	movaps 0x375a(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002a70 <t_gate(float2*)>:
+0000000000002a90 <t_gate(float2*)>:
 t_gate(float2*):
 	endbr64
-	movss  0x3724(%rip),%xmm0        
+	movss  0x3734(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x376a(%rip),%xmm0        
+	movaps 0x377a(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002a90 <tdg_gate(float2*)>:
+0000000000002ab0 <tdg_gate(float2*)>:
 tdg_gate(float2*):
 	endbr64
-	movss  0x3704(%rip),%xmm0        
+	movss  0x3714(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x375a(%rip),%xmm0        
+	movaps 0x376a(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002ab0 <h_gate(float2*)>:
+0000000000002ad0 <h_gate(float2*)>:
 h_gate(float2*):
 	endbr64
-	movaps 0x3755(%rip),%xmm0        
+	movaps 0x3765(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x375b(%rip),%xmm0        
+	movaps 0x376b(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-0000000000002ad0 <rx_gate(float2*, float)>:
+0000000000002af0 <rx_gate(float2*, float)>:
 rx_gate(float2*, float):
 	endbr64
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x37fc(%rip),%xmm0        
+	mulss  0x380c(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   2460 <sincosf@plt>
+	call   2470 <sincosf@plt>
 	movss  0x8(%rsp),%xmm1
 	movss  0xc(%rsp),%xmm0
 	movq   $0x0,0x4(%rbx)
-	xorps  0x3722(%rip),%xmm0        
+	xorps  0x3732(%rip),%xmm0        
 	movl   $0x0,0x10(%rbx)
 	movl   $0x0,0x1c(%rbx)
 	movss  %xmm1,(%rbx)
 	movss  %xmm0,0xc(%rbx)
 	movss  %xmm0,0x14(%rbx)
 	movss  %xmm1,0x18(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-0000000000002b40 <ry_gate(float2*, float)>:
+0000000000002b60 <ry_gate(float2*, float)>:
 ry_gate(float2*, float):
 	endbr64
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x378c(%rip),%xmm0        
+	mulss  0x379c(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   2460 <sincosf@plt>
+	call   2470 <sincosf@plt>
 	movss  0xc(%rsp),%xmm1
 	movss  0x8(%rsp),%xmm0
 	movl   $0x0,0x4(%rbx)
 	movl   $0x0,0xc(%rbx)
 	movaps %xmm1,%xmm2
-	xorps  0x36a9(%rip),%xmm2        
+	xorps  0x36b9(%rip),%xmm2        
 	movl   $0x0,0x14(%rbx)
 	movl   $0x0,0x1c(%rbx)
 	movss  %xmm0,(%rbx)
 	movss  %xmm2,0x8(%rbx)
 	movss  %xmm1,0x10(%rbx)
 	movss  %xmm0,0x18(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	xchg   %ax,%ax
 
-0000000000002bb0 <rz_gate(float2*, float)>:
+0000000000002bd0 <rz_gate(float2*, float)>:
 rz_gate(float2*, float):
 	endbr64
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x371c(%rip),%xmm0        
+	mulss  0x372c(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   2460 <sincosf@plt>
+	call   2470 <sincosf@plt>
 	movss  0xc(%rsp),%xmm0
 	movss  0x8(%rsp),%xmm1
 	movq   $0x0,0x8(%rbx)
 	movq   $0x0,0x10(%rbx)
 	movaps %xmm0,%xmm2
-	xorps  0x3637(%rip),%xmm2        
+	xorps  0x3647(%rip),%xmm2        
 	movss  %xmm1,(%rbx)
 	movss  %xmm1,0x18(%rbx)
 	movss  %xmm2,0x4(%rbx)
 	movss  %xmm0,0x1c(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000002c20 <damp_i_gate(float2*, float)>:
+0000000000002c40 <damp_i_gate(float2*, float)>:
 damp_i_gate(float2*, float):
 	endbr64
 	pxor   %xmm3,%xmm3
 	comiss %xmm3,%xmm0
-	jbe    2c3a <damp_i_gate(float2*, float)+0x1a>
-	movss  0x36af(%rip),%xmm1        
+	jbe    2c5a <damp_i_gate(float2*, float)+0x1a>
+	movss  0x36bf(%rip),%xmm1        
 	comiss %xmm0,%xmm1
-	ja     2c40 <damp_i_gate(float2*, float)+0x20>
+	ja     2c60 <damp_i_gate(float2*, float)+0x20>
 	ret
 	nopl   0x0(%rax,%rax,1)
 	subss  %xmm0,%xmm1
-	movss  0x3554(%rip),%xmm2        
+	movss  0x3564(%rip),%xmm2        
 	movq   $0x0,0x10(%rdi)
 	movups %xmm2,(%rdi)
 	ucomiss %xmm1,%xmm3
-	ja     2c6d <damp_i_gate(float2*, float)+0x4d>
+	ja     2c8d <damp_i_gate(float2*, float)+0x4d>
 	sqrtss %xmm1,%xmm1
 	movl   $0x0,0x1c(%rdi)
 	movss  %xmm1,0x18(%rdi)
 	ret
 	sub    $0x18,%rsp
 	movaps %xmm1,%xmm0
 	mov    %rdi,0x8(%rsp)
-	call   2640 <sqrtf@plt>
+	call   2650 <sqrtf@plt>
 	mov    0x8(%rsp),%rdi
 	movl   $0x0,0x1c(%rdi)
 	movss  %xmm0,0x18(%rdi)
 	add    $0x18,%rsp
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nop
 
-0000000000002ca0 <pd_gate(float2*, float)>:
+0000000000002cc0 <pd_gate(float2*, float)>:
 pd_gate(float2*, float):
 	endbr64
 	pxor   %xmm2,%xmm2
 	comiss %xmm2,%xmm0
-	jbe    2cba <pd_gate(float2*, float)+0x1a>
-	movss  0x362f(%rip),%xmm1        
+	jbe    2cda <pd_gate(float2*, float)+0x1a>
+	movss  0x363f(%rip),%xmm1        
 	comiss %xmm0,%xmm1
-	ja     2cc0 <pd_gate(float2*, float)+0x20>
+	ja     2ce0 <pd_gate(float2*, float)+0x20>
 	ret
 	nopl   0x0(%rax,%rax,1)
 	ucomiss %xmm0,%xmm2
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x10(%rdi)
 	movups %xmm1,(%rdi)
-	ja     2ce5 <pd_gate(float2*, float)+0x45>
+	ja     2d05 <pd_gate(float2*, float)+0x45>
 	sqrtss %xmm0,%xmm0
 	movl   $0x0,0x1c(%rdi)
 	movss  %xmm0,0x18(%rdi)
 	ret
 	sub    $0x18,%rsp
 	mov    %rdi,0x8(%rsp)
-	call   2640 <sqrtf@plt>
+	call   2650 <sqrtf@plt>
 	mov    0x8(%rsp),%rdi
 	movl   $0x0,0x1c(%rdi)
 	movss  %xmm0,0x18(%rdi)
 	add    $0x18,%rsp
 	ret
 	nopl   0x0(%rax)
 
-0000000000002d10 <ad_gate(float2*, float)>:
+0000000000002d30 <ad_gate(float2*, float)>:
 ad_gate(float2*, float):
 	endbr64
 	pxor   %xmm2,%xmm2
 	comiss %xmm2,%xmm0
-	jbe    2d2a <ad_gate(float2*, float)+0x1a>
-	movss  0x35bf(%rip),%xmm1        
+	jbe    2d4a <ad_gate(float2*, float)+0x1a>
+	movss  0x35cf(%rip),%xmm1        
 	comiss %xmm0,%xmm1
-	ja     2d30 <ad_gate(float2*, float)+0x20>
+	ja     2d50 <ad_gate(float2*, float)+0x20>
 	ret
 	nopl   0x0(%rax,%rax,1)
 	sub    $0x18,%rsp
 	ucomiss %xmm0,%xmm2
 	movq   $0x0,(%rdi)
-	ja     2d65 <ad_gate(float2*, float)+0x55>
+	ja     2d85 <ad_gate(float2*, float)+0x55>
 	sqrtss %xmm0,%xmm0
 	movl   $0x0,0xc(%rdi)
 	movq   $0x0,0x10(%rdi)
 	movq   $0x0,0x18(%rdi)
 	movss  %xmm0,0x8(%rdi)
 	add    $0x18,%rsp
 	ret
 	mov    %rdi,0x8(%rsp)
-	call   2640 <sqrtf@plt>
+	call   2650 <sqrtf@plt>
 	mov    0x8(%rsp),%rdi
-	jmp    2d44 <ad_gate(float2*, float)+0x34>
+	jmp    2d64 <ad_gate(float2*, float)+0x34>
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000002d80 <swap_gate(float2*)>:
+0000000000002da0 <swap_gate(float2*)>:
 swap_gate(float2*):
 	endbr64
-	movss  0x3414(%rip),%xmm1        
+	movss  0x3424(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
 	movups %xmm1,(%rdi)
 	movups %xmm1,0x30(%rdi)
-	movaps 0x33f2(%rip),%xmm1        
+	movaps 0x3402(%rip),%xmm1        
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x20(%rdi)
 	movups %xmm1,0x40(%rdi)
 	movups %xmm0,0x50(%rdi)
 	movups %xmm0,0x60(%rdi)
 	movups %xmm1,0x70(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-0000000000002dc0 <iswap_gate(float2*)>:
+0000000000002de0 <iswap_gate(float2*)>:
 iswap_gate(float2*):
 	endbr64
-	movaps 0x33f5(%rip),%xmm1        
-	movss  0x33cd(%rip),%xmm0        
+	movaps 0x3405(%rip),%xmm1        
+	movss  0x33dd(%rip),%xmm0        
 	movups %xmm0,(%rdi)
 	pxor   %xmm0,%xmm0
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x20(%rdi)
 	movups %xmm1,0x30(%rdi)
-	movaps 0x33f3(%rip),%xmm1        
+	movaps 0x3403(%rip),%xmm1        
 	movups %xmm0,0x50(%rdi)
 	movups %xmm0,0x60(%rdi)
-	movaps 0x3394(%rip),%xmm0        
+	movaps 0x33a4(%rip),%xmm0        
 	movups %xmm1,0x40(%rdi)
 	movups %xmm0,0x70(%rdi)
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-0000000000002e10 <cphase_gate(float2*, float)>:
+0000000000002e30 <cphase_gate(float2*, float)>:
 cphase_gate(float2*, float):
 	endbr64
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   2460 <sincosf@plt>
+	call   2470 <sincosf@plt>
 	pxor   %xmm0,%xmm0
-	movaps 0x335a(%rip),%xmm2        
-	movss  0x3362(%rip),%xmm1        
+	movaps 0x336a(%rip),%xmm2        
+	movss  0x3372(%rip),%xmm1        
 	movups %xmm0,0x10(%rbx)
 	movups %xmm0,0x30(%rbx)
 	movups %xmm0,0x40(%rbx)
 	movups %xmm0,0x60(%rbx)
 	movss  0x8(%rsp),%xmm0
 	movq   $0x0,0x70(%rbx)
 	movss  %xmm0,0x78(%rbx)
@@ -436,80 +436,80 @@
 	movups %xmm1,0x50(%rbx)
 	movss  %xmm0,0x7c(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	nopl   (%rax)
 
-0000000000002e80 <cnot_gate_control_big(float2*)>:
+0000000000002ea0 <cnot_gate_control_big(float2*)>:
 cnot_gate_control_big(float2*):
 	endbr64
-	movaps 0x3305(%rip),%xmm2        
+	movaps 0x3315(%rip),%xmm2        
 	pxor   %xmm0,%xmm0
-	movss  0x3309(%rip),%xmm1        
+	movss  0x3319(%rip),%xmm1        
 	movups %xmm1,(%rdi)
 	movups %xmm0,0x10(%rdi)
 	movups %xmm2,0x20(%rdi)
 	movups %xmm0,0x30(%rdi)
 	movups %xmm0,0x40(%rdi)
 	movups %xmm2,0x50(%rdi)
 	movups %xmm0,0x60(%rdi)
 	movups %xmm1,0x70(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-0000000000002ec0 <cnot_gate_control_small(float2*)>:
+0000000000002ee0 <cnot_gate_control_small(float2*)>:
 cnot_gate_control_small(float2*):
 	endbr64
-	movaps 0x32c5(%rip),%xmm1        
+	movaps 0x32d5(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
-	movss  0x32c9(%rip),%xmm2        
+	movss  0x32d9(%rip),%xmm2        
 	movups %xmm2,(%rdi)
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x20(%rdi)
 	movups %xmm1,0x30(%rdi)
 	movups %xmm0,0x40(%rdi)
 	movups %xmm2,0x50(%rdi)
 	movups %xmm1,0x60(%rdi)
 	movups %xmm0,0x70(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-0000000000002f00 <cz_gate(float2*)>:
+0000000000002f20 <cz_gate(float2*)>:
 cz_gate(float2*):
 	endbr64
 	pxor   %xmm0,%xmm0
-	movaps 0x3281(%rip),%xmm2        
-	movss  0x3289(%rip),%xmm1        
+	movaps 0x3291(%rip),%xmm2        
+	movss  0x3299(%rip),%xmm1        
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x30(%rdi)
 	movups %xmm0,0x40(%rdi)
 	movups %xmm0,0x60(%rdi)
-	movaps 0x32a2(%rip),%xmm0        
+	movaps 0x32b2(%rip),%xmm0        
 	movups %xmm1,(%rdi)
 	movups %xmm2,0x20(%rdi)
 	movups %xmm1,0x50(%rdi)
 	movups %xmm0,0x70(%rdi)
 	ret
 	xchg   %ax,%ax
 
-0000000000002f40 <rxx_gate(float2*, float)>:
+0000000000002f60 <rxx_gate(float2*, float)>:
 rxx_gate(float2*, float):
 	endbr64
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x338c(%rip),%xmm0        
+	mulss  0x339c(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   2460 <sincosf@plt>
+	call   2470 <sincosf@plt>
 	movss  0x8(%rsp),%xmm1
 	movss  0xc(%rsp),%xmm0
 	movq   $0x0,0x4(%rbx)
-	xorps  0x32b2(%rip),%xmm0        
+	xorps  0x32c2(%rip),%xmm0        
 	movq   $0x0,0xc(%rbx)
 	movq   $0x0,0x14(%rbx)
 	movq   $0x0,0x20(%rbx)
 	movq   $0x0,0x2c(%rbx)
 	movq   $0x0,0x38(%rbx)
 	movq   $0x0,0x40(%rbx)
 	movl   $0x0,0x48(%rbx)
@@ -527,30 +527,30 @@
 	movss  %xmm0,0x64(%rbx)
 	movss  %xmm1,0x78(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	nopl   0x0(%rax)
 
-0000000000003010 <ryy_gate(float2*, float)>:
+0000000000003030 <ryy_gate(float2*, float)>:
 ryy_gate(float2*, float):
 	endbr64
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x32bc(%rip),%xmm0        
+	mulss  0x32cc(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   2460 <sincosf@plt>
+	call   2470 <sincosf@plt>
 	movss  0xc(%rsp),%xmm1
 	movss  0x8(%rsp),%xmm0
 	movq   $0x0,0x4(%rbx)
 	movq   $0x0,0xc(%rbx)
 	movaps %xmm1,%xmm2
-	xorps  0x31d7(%rip),%xmm2        
+	xorps  0x31e7(%rip),%xmm2        
 	movq   $0x0,0x14(%rbx)
 	movq   $0x0,0x20(%rbx)
 	movq   $0x0,0x2c(%rbx)
 	movq   $0x0,0x38(%rbx)
 	movq   $0x0,0x40(%rbx)
 	movl   $0x0,0x48(%rbx)
 	movq   $0x0,0x54(%rbx)
@@ -567,30 +567,30 @@
 	movss  %xmm1,0x64(%rbx)
 	movss  %xmm0,0x78(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	nopl   0x0(%rax)
 
-00000000000030e0 <rzz_gate(float2*, float)>:
+0000000000003100 <rzz_gate(float2*, float)>:
 rzz_gate(float2*, float):
 	endbr64
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x31ec(%rip),%xmm0        
+	mulss  0x31fc(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   2460 <sincosf@plt>
+	call   2470 <sincosf@plt>
 	movss  0xc(%rsp),%xmm1
 	movss  0x8(%rsp),%xmm0
 	movq   $0x0,0x8(%rbx)
 	movq   $0x0,0x10(%rbx)
 	movaps %xmm1,%xmm2
-	xorps  0x3107(%rip),%xmm2        
+	xorps  0x3117(%rip),%xmm2        
 	movq   $0x0,0x18(%rbx)
 	movq   $0x0,0x20(%rbx)
 	movq   $0x0,0x30(%rbx)
 	movq   $0x0,0x38(%rbx)
 	movq   $0x0,0x40(%rbx)
 	movq   $0x0,0x48(%rbx)
 	movq   $0x0,0x58(%rbx)
@@ -606,79 +606,79 @@
 	movss  %xmm0,0x78(%rbx)
 	movss  %xmm2,0x7c(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 
-00000000000031b0 <syc_gate(float2*)>:
+00000000000031d0 <syc_gate(float2*)>:
 syc_gate(float2*):
 	endbr64
-	movaps 0x3085(%rip),%xmm1        
-	movss  0x2fdd(%rip),%xmm0        
+	movaps 0x3095(%rip),%xmm1        
+	movss  0x2fed(%rip),%xmm0        
 	movups %xmm0,(%rdi)
 	pxor   %xmm0,%xmm0
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x20(%rdi)
 	movups %xmm1,0x30(%rdi)
-	movaps 0x2fd3(%rip),%xmm1        
+	movaps 0x2fe3(%rip),%xmm1        
 	movups %xmm0,0x50(%rdi)
 	movups %xmm0,0x60(%rdi)
-	movaps 0x3064(%rip),%xmm0        
+	movaps 0x3074(%rip),%xmm0        
 	movups %xmm1,0x40(%rdi)
 	movups %xmm0,0x70(%rdi)
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-0000000000003200 <toff_gate_target_small(float2*)>:
+0000000000003220 <toff_gate_target_small(float2*)>:
 toff_gate_target_small(float2*):
 	endbr64
-	movss  0x30d8(%rip),%xmm0        
+	movss  0x30e8(%rip),%xmm0        
 	mov    %rdi,%rdx
 	xor    %eax,%eax
-	jmp    3229 <toff_gate_target_small(float2*)+0x29>
+	jmp    3249 <toff_gate_target_small(float2*)+0x29>
 	nopl   0x0(%rax,%rax,1)
 	movss  %xmm0,(%rdx)
 	movl   $0x0,0x4(%rdx)
 	add    $0x8,%rdx
 	mov    %ecx,%eax
 	lea    0x1(%rax),%ecx
 	cmp    $0x2f,%eax
-	ja     3250 <toff_gate_target_small(float2*)+0x50>
+	ja     3270 <toff_gate_target_small(float2*)+0x50>
 	imul   $0x38e38e39,%eax,%eax
 	cmp    $0x1c71c71c,%eax
-	jbe    3218 <toff_gate_target_small(float2*)+0x18>
+	jbe    3238 <toff_gate_target_small(float2*)+0x18>
 	movl   $0x0,(%rdx)
-	jmp    321c <toff_gate_target_small(float2*)+0x1c>
+	jmp    323c <toff_gate_target_small(float2*)+0x1c>
 	cs nopw 0x0(%rax,%rax,1)
 	movl   $0x0,(%rdx)
 	movl   $0x0,0x4(%rdx)
 	cmp    $0x40,%ecx
-	jne    3223 <toff_gate_target_small(float2*)+0x23>
+	jne    3243 <toff_gate_target_small(float2*)+0x23>
 	movss  %xmm0,0x1b8(%rdi)
 	movss  %xmm0,0x1f0(%rdi)
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	xchg   %ax,%ax
 
-0000000000003280 <toff_gate_target_mid(float2*)>:
+00000000000032a0 <toff_gate_target_mid(float2*)>:
 toff_gate_target_mid(float2*):
 	endbr64
-	movdqa 0x3014(%rip),%xmm4        
+	movdqa 0x3024(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x2fc5(%rip),%xmm5        
+	movdqa 0x2fd5(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x2fc1(%rip),%xmm11        
-	movdqa 0x2fc8(%rip),%xmm10        
+	movdqa 0x2fd1(%rip),%xmm11        
+	movdqa 0x2fd8(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x2fec(%rip),%xmm8        
+	movaps 0x2ffc(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x2fbf(%rip),%xmm9        
+	movdqa 0x2fcf(%rip),%xmm9        
 	nopl   0x0(%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -729,39 +729,39 @@
 	andnps %xmm0,%xmm1
 	movaps %xmm1,%xmm0
 	unpckhps %xmm6,%xmm1
 	unpcklps %xmm6,%xmm0
 	movups %xmm1,-0x10(%rax)
 	movups %xmm0,-0x20(%rax)
 	cmp    %rax,%rdx
-	jne    32d8 <toff_gate_target_mid(float2*)+0x58>
+	jne    32f8 <toff_gate_target_mid(float2*)+0x58>
 	movl   $0x3f800000,0x1a8(%rdi)
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x3f800000,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x0,0x1f8(%rdi)
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nop
 
-0000000000003420 <toff_gate_target_big(float2*)>:
+0000000000003440 <toff_gate_target_big(float2*)>:
 toff_gate_target_big(float2*):
 	endbr64
-	movdqa 0x2e74(%rip),%xmm4        
+	movdqa 0x2e84(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x2e25(%rip),%xmm5        
+	movdqa 0x2e35(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x2e21(%rip),%xmm11        
-	movdqa 0x2e68(%rip),%xmm10        
+	movdqa 0x2e31(%rip),%xmm11        
+	movdqa 0x2e78(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x2e4c(%rip),%xmm8        
+	movaps 0x2e5c(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x2e1f(%rip),%xmm9        
+	movdqa 0x2e2f(%rip),%xmm9        
 	nopl   0x0(%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -812,41 +812,41 @@
 	andnps %xmm0,%xmm1
 	movaps %xmm1,%xmm0
 	unpckhps %xmm6,%xmm1
 	unpcklps %xmm6,%xmm0
 	movups %xmm1,-0x10(%rax)
 	movups %xmm0,-0x20(%rax)
 	cmp    %rax,%rdx
-	jne    3478 <toff_gate_target_big(float2*)+0x58>
-	movss  0x2d5f(%rip),%xmm0        
+	jne    3498 <toff_gate_target_big(float2*)+0x58>
+	movss  0x2d6f(%rip),%xmm0        
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x0,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x0,0x1f8(%rdi)
 	movss  %xmm0,0xf8(%rdi)
 	movss  %xmm0,0x1d8(%rdi)
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-00000000000035d0 <fred_gate_control_big(float2*)>:
+00000000000035f0 <fred_gate_control_big(float2*)>:
 fred_gate_control_big(float2*):
 	endbr64
-	movdqa 0x2cc4(%rip),%xmm4        
+	movdqa 0x2cd4(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x2c75(%rip),%xmm5        
+	movdqa 0x2c85(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x2c71(%rip),%xmm11        
-	movdqa 0x2c78(%rip),%xmm10        
+	movdqa 0x2c81(%rip),%xmm11        
+	movdqa 0x2c88(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x2c9c(%rip),%xmm8        
+	movaps 0x2cac(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x2caf(%rip),%xmm9        
+	movdqa 0x2cbf(%rip),%xmm9        
 	nopl   0x0(%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -897,41 +897,41 @@
 	andnps %xmm0,%xmm1
 	movaps %xmm1,%xmm0
 	unpckhps %xmm6,%xmm1
 	unpcklps %xmm6,%xmm0
 	movups %xmm1,-0x10(%rax)
 	movups %xmm0,-0x20(%rax)
 	cmp    %rax,%rdx
-	jne    3628 <fred_gate_control_big(float2*)+0x58>
-	movss  0x2baf(%rip),%xmm0        
+	jne    3648 <fred_gate_control_big(float2*)+0x58>
+	movss  0x2bbf(%rip),%xmm0        
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x0,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x3f800000,0x1f8(%rdi)
 	movss  %xmm0,0x170(%rdi)
 	movss  %xmm0,0x1a8(%rdi)
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000003780 <fred_gate_control_mid(float2*)>:
+00000000000037a0 <fred_gate_control_mid(float2*)>:
 fred_gate_control_mid(float2*):
 	endbr64
-	movdqa 0x2b14(%rip),%xmm4        
+	movdqa 0x2b24(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x2ac5(%rip),%xmm5        
+	movdqa 0x2ad5(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x2ac1(%rip),%xmm11        
-	movdqa 0x2b08(%rip),%xmm10        
+	movdqa 0x2ad1(%rip),%xmm11        
+	movdqa 0x2b18(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x2aec(%rip),%xmm8        
+	movaps 0x2afc(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x2aff(%rip),%xmm9        
+	movdqa 0x2b0f(%rip),%xmm9        
 	nopl   0x0(%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -982,41 +982,41 @@
 	andnps %xmm0,%xmm1
 	movaps %xmm1,%xmm0
 	unpckhps %xmm6,%xmm1
 	unpcklps %xmm6,%xmm0
 	movups %xmm1,-0x10(%rax)
 	movups %xmm0,-0x20(%rax)
 	cmp    %rax,%rdx
-	jne    37d8 <fred_gate_control_mid(float2*)+0x58>
-	movss  0x29ff(%rip),%xmm0        
+	jne    37f8 <fred_gate_control_mid(float2*)+0x58>
+	movss  0x2a0f(%rip),%xmm0        
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x0,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x3f800000,0x1f8(%rdi)
 	movss  %xmm0,0xf0(%rdi)
 	movss  %xmm0,0x198(%rdi)
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000003930 <fred_gate_control_small(float2*)>:
+0000000000003950 <fred_gate_control_small(float2*)>:
 fred_gate_control_small(float2*):
 	endbr64
-	movdqa 0x2964(%rip),%xmm4        
+	movdqa 0x2974(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x2915(%rip),%xmm5        
+	movdqa 0x2925(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x2911(%rip),%xmm11        
-	movdqa 0x2958(%rip),%xmm10        
+	movdqa 0x2921(%rip),%xmm11        
+	movdqa 0x2968(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x293c(%rip),%xmm8        
+	movaps 0x294c(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x28ff(%rip),%xmm9        
+	movdqa 0x290f(%rip),%xmm9        
 	nopl   0x0(%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -1067,98 +1067,98 @@
 	andnps %xmm0,%xmm1
 	movaps %xmm1,%xmm0
 	unpckhps %xmm6,%xmm1
 	unpcklps %xmm6,%xmm0
 	movups %xmm1,-0x10(%rax)
 	movups %xmm0,-0x20(%rax)
 	cmp    %rax,%rdx
-	jne    3988 <fred_gate_control_small(float2*)+0x58>
-	movss  0x284f(%rip),%xmm0        
+	jne    39a8 <fred_gate_control_small(float2*)+0x58>
+	movss  0x285f(%rip),%xmm0        
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x0,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x3f800000,0x1f8(%rdi)
 	movss  %xmm0,0xe8(%rdi)
 	movss  %xmm0,0x158(%rdi)
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000003ae0 <identityMat(float2*, int)>:
+0000000000003b00 <identityMat(float2*, int)>:
 identityMat(float2*, int):
 	endbr64
 	lea    (%rsi,%rsi,1),%ecx
 	mov    %esi,%eax
 	mov    $0x1,%esi
-	movss  0x27ee(%rip),%xmm0        
+	movss  0x27fe(%rip),%xmm0        
 	mov    %esi,%edx
 	shl    %cl,%edx
 	lea    0x1(%rax),%ecx
 	shl    %cl,%esi
 	movslq %edx,%r8
 	xor    %ecx,%ecx
 	test   %edx,%edx
-	jle    3b48 <identityMat(float2*, int)+0x68>
+	jle    3b68 <identityMat(float2*, int)+0x68>
 	nopl   0x0(%rax,%rax,1)
 	mov    %ecx,%eax
 	cltd
 	idiv   %esi
 	test   %edx,%edx
-	jne    3b30 <identityMat(float2*, int)+0x50>
+	jne    3b50 <identityMat(float2*, int)+0x50>
 	movl   $0x0,0x4(%rdi,%rcx,8)
 	movss  %xmm0,(%rdi,%rcx,8)
 	add    $0x1,%rcx
 	cmp    %r8,%rcx
-	jne    3b10 <identityMat(float2*, int)+0x30>
+	jne    3b30 <identityMat(float2*, int)+0x30>
 	ret
 	movl   $0x0,(%rdi,%rcx,8)
 	movl   $0x0,0x4(%rdi,%rcx,8)
 	add    $0x1,%rcx
 	cmp    %r8,%rcx
-	jne    3b10 <identityMat(float2*, int)+0x30>
+	jne    3b30 <identityMat(float2*, int)+0x30>
 	ret
 	nopl   0x0(%rax)
 
-0000000000003b50 <generate_binary_data(float)>:
+0000000000003b70 <generate_binary_data(float)>:
 generate_binary_data(float):
 	endbr64
 	sub    $0x18,%rsp
 	xor    %edi,%edi
 	movss  %xmm0,0xc(%rsp)
-	call   2620 <time@plt>
+	call   2630 <time@plt>
 	mov    %rax,%rdi
-	call   25b0 <srand@plt>
-	call   2800 <rand@plt>
+	call   25c0 <srand@plt>
+	call   2820 <rand@plt>
 	pxor   %xmm0,%xmm0
 	movss  0xc(%rsp),%xmm1
 	cvtsi2ss %eax,%xmm0
-	mulss  0x2760(%rip),%xmm0        
+	mulss  0x2770(%rip),%xmm0        
 	xor    %eax,%eax
 	comiss %xmm0,%xmm1
 	seta   %al
 	add    $0x18,%rsp
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-0000000000003ba0 <getprob(float2*, float*, unsigned long)>:
+0000000000003bc0 <getprob(float2*, float*, unsigned long)>:
 getprob(float2*, float*, unsigned long):
 	endbr64
 	test   %rdx,%rdx
-	je     3cc5 <getprob(float2*, float*, unsigned long)+0x125>
+	je     3ce5 <getprob(float2*, float*, unsigned long)+0x125>
 	lea    (%rsi,%rdx,4),%rax
 	cmp    %rax,%rdi
 	lea    (%rdi,%rdx,8),%rax
 	setae  %cl
 	cmp    %rax,%rsi
 	setae  %al
 	or     %al,%cl
-	je     3c98 <getprob(float2*, float*, unsigned long)+0xf8>
+	je     3cb8 <getprob(float2*, float*, unsigned long)+0xf8>
 	lea    -0x1(%rdx),%rax
 	cmp    $0x2,%rax
-	jbe    3c98 <getprob(float2*, float*, unsigned long)+0xf8>
+	jbe    3cb8 <getprob(float2*, float*, unsigned long)+0xf8>
 	mov    %rdx,%rcx
 	xor    %eax,%eax
 	shr    $0x2,%rcx
 	shl    $0x4,%rcx
 	nopl   0x0(%rax)
 	movups (%rdi,%rax,2),%xmm0
 	movups 0x10(%rdi,%rax,2),%xmm2
@@ -1167,41 +1167,41 @@
 	shufps $0x88,%xmm2,%xmm1
 	mulps  %xmm0,%xmm0
 	mulps  %xmm1,%xmm1
 	addps  %xmm1,%xmm0
 	movups %xmm0,(%rsi,%rax,1)
 	add    $0x10,%rax
 	cmp    %rcx,%rax
-	jne    3be8 <getprob(float2*, float*, unsigned long)+0x48>
+	jne    3c08 <getprob(float2*, float*, unsigned long)+0x48>
 	mov    %rdx,%rax
 	and    $0xfffffffffffffffc,%rax
 	test   $0x3,%dl
-	je     3cc5 <getprob(float2*, float*, unsigned long)+0x125>
+	je     3ce5 <getprob(float2*, float*, unsigned long)+0x125>
 	lea    (%rdi,%rax,8),%rcx
 	movss  (%rcx),%xmm0
 	movss  0x4(%rcx),%xmm1
 	lea    0x1(%rax),%ecx
 	movslq %ecx,%rcx
 	mulss  %xmm0,%xmm0
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	movss  %xmm0,(%rsi,%rax,4)
 	cmp    %rcx,%rdx
-	jbe    3cc5 <getprob(float2*, float*, unsigned long)+0x125>
+	jbe    3ce5 <getprob(float2*, float*, unsigned long)+0x125>
 	lea    (%rdi,%rcx,8),%r8
 	add    $0x2,%eax
 	movss  (%r8),%xmm0
 	movss  0x4(%r8),%xmm1
 	cltq
 	mulss  %xmm0,%xmm0
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	movss  %xmm0,(%rsi,%rcx,4)
 	cmp    %rax,%rdx
-	jbe    3cc5 <getprob(float2*, float*, unsigned long)+0x125>
+	jbe    3ce5 <getprob(float2*, float*, unsigned long)+0x125>
 	lea    (%rdi,%rax,8),%rdx
 	movss  (%rdx),%xmm0
 	movss  0x4(%rdx),%xmm1
 	mulss  %xmm0,%xmm0
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	movss  %xmm0,(%rsi,%rax,4)
@@ -1213,59 +1213,59 @@
 	movss  0x4(%rdi,%rax,8),%xmm0
 	mulss  %xmm1,%xmm1
 	mulss  %xmm0,%xmm0
 	addss  %xmm1,%xmm0
 	movss  %xmm0,(%rsi,%rax,4)
 	add    $0x1,%rax
 	cmp    %rax,%rdx
-	jne    3ca0 <getprob(float2*, float*, unsigned long)+0x100>
+	jne    3cc0 <getprob(float2*, float*, unsigned long)+0x100>
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000003cd0 <hash(char const*)>:
+0000000000003cf0 <hash(char const*)>:
 hash(char const*):
 	endbr64
 	movsbl (%rdi),%eax
 	lea    0x1(%rdi),%rdx
 	mov    $0x1,%r8d
 	test   %al,%al
-	je     3cfb <hash(char const*)+0x2b>
+	je     3d1b <hash(char const*)+0x2b>
 	nopl   (%rax)
 	lea    (%rax,%r8,2),%eax
 	add    $0x1,%rdx
 	add    %eax,%r8d
 	movsbl -0x1(%rdx),%eax
 	test   %al,%al
-	jne    3ce8 <hash(char const*)+0x18>
+	jne    3d08 <hash(char const*)+0x18>
 	mov    %r8d,%eax
 	ret
 	nop
 
-0000000000003d00 <isInArray(char const**, char*, int)>:
+0000000000003d20 <isInArray(char const**, char*, int)>:
 isInArray(char const**, char*, int):
 	endbr64
 	test   %edx,%edx
-	jle    3d4f <isInArray(char const**, char*, int)+0x4f>
+	jle    3d6f <isInArray(char const**, char*, int)+0x4f>
 	lea    -0x1(%rdx),%eax
 	push   %r12
 	lea    0x8(%rdi,%rax,8),%r12
 	push   %rbp
 	mov    %rsi,%rbp
 	push   %rbx
 	mov    %rdi,%rbx
-	jmp    3d29 <isInArray(char const**, char*, int)+0x29>
+	jmp    3d49 <isInArray(char const**, char*, int)+0x29>
 	nopl   0x0(%rax)
 	add    $0x8,%rbx
 	cmp    %r12,%rbx
-	je     3d48 <isInArray(char const**, char*, int)+0x48>
+	je     3d68 <isInArray(char const**, char*, int)+0x48>
 	mov    (%rbx),%rdi
 	mov    %rbp,%rsi
-	call   25e0 <strcmp@plt>
+	call   25f0 <strcmp@plt>
 	test   %eax,%eax
-	jne    3d20 <isInArray(char const**, char*, int)+0x20>
+	jne    3d40 <isInArray(char const**, char*, int)+0x20>
 	pop    %rbx
 	mov    $0x1,%eax
 	pop    %rbp
 	pop    %r12
 	ret
 	nopw   0x0(%rax,%rax,1)
 	pop    %rbx
@@ -1274,42 +1274,42 @@
 	pop    %r12
 	ret
 	xor    %eax,%eax
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000003d60 <getArrayLength(int*)>:
+0000000000003d80 <getArrayLength(int*)>:
 getArrayLength(int*):
 	endbr64
 	xor    %eax,%eax
 	cmpl   $0xffffffff,(%rdi)
-	je     3d80 <getArrayLength(int*)+0x20>
+	je     3da0 <getArrayLength(int*)+0x20>
 	nopl   0x0(%rax,%rax,1)
 	add    $0x4,%rdi
 	add    $0x1,%eax
 	cmpl   $0xffffffff,(%rdi)
-	jne    3d70 <getArrayLength(int*)+0x10>
+	jne    3d90 <getArrayLength(int*)+0x10>
 	ret
 	nopl   (%rax)
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-0000000000003d90 <normalization(float2*, int)>:
+0000000000003db0 <normalization(float2*, int)>:
 normalization(float2*, int):
 	endbr64
 	mov    %esi,%ecx
 	mov    $0x1,%edx
 	shl    %cl,%edx
 	test   %edx,%edx
-	jle    3f10 <normalization(float2*, int)+0x180>
+	jle    3f30 <normalization(float2*, int)+0x180>
 	lea    -0x1(%rdx),%r8d
 	cmp    $0x2,%r8d
-	jbe    3f93 <normalization(float2*, int)+0x203>
+	jbe    3fb3 <normalization(float2*, int)+0x203>
 	mov    %edx,%esi
 	mov    %rdi,%rax
 	pxor   %xmm3,%xmm3
 	shr    $0x2,%esi
 	shl    $0x5,%rsi
 	add    %rdi,%rsi
 	cs nopw 0x0(%rax,%rax,1)
@@ -1330,274 +1330,278 @@
 	movaps %xmm0,%xmm2
 	unpckhps %xmm0,%xmm2
 	shufps $0xff,%xmm0,%xmm0
 	addss  %xmm2,%xmm1
 	movaps %xmm1,%xmm3
 	addss  %xmm0,%xmm3
 	cmp    %rsi,%rax
-	jne    3dd0 <normalization(float2*, int)+0x40>
+	jne    3df0 <normalization(float2*, int)+0x40>
 	mov    %edx,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%dl
-	je     3e96 <normalization(float2*, int)+0x106>
+	je     3eb6 <normalization(float2*, int)+0x106>
 	movslq %eax,%rsi
 	lea    (%rdi,%rsi,8),%rsi
 	movss  (%rsi),%xmm0
 	movss  0x4(%rsi),%xmm1
 	lea    0x1(%rax),%esi
 	mulss  %xmm0,%xmm0
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	addss  %xmm0,%xmm3
 	cmp    %edx,%esi
-	jge    3f70 <normalization(float2*, int)+0x1e0>
+	jge    3f90 <normalization(float2*, int)+0x1e0>
 	movslq %esi,%rsi
 	add    $0x2,%eax
 	lea    (%rdi,%rsi,8),%rcx
 	movss  (%rcx),%xmm1
 	movss  0x4(%rcx),%xmm0
 	mulss  %xmm1,%xmm1
 	mulss  %xmm0,%xmm0
 	addss  %xmm1,%xmm0
 	addss  %xmm0,%xmm3
 	cmp    %eax,%edx
-	jle    3e96 <normalization(float2*, int)+0x106>
+	jle    3eb6 <normalization(float2*, int)+0x106>
 	cltq
 	lea    (%rdi,%rax,8),%rax
 	movss  (%rax),%xmm0
 	movss  0x4(%rax),%xmm1
 	mulss  %xmm0,%xmm0
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	addss  %xmm0,%xmm3
-	movsd  0x2452(%rip),%xmm1        
+	movsd  0x2462(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
 	cvtss2sd %xmm3,%xmm0
 	comisd %xmm0,%xmm1
-	ja     3f18 <normalization(float2*, int)+0x188>
+	ja     3f38 <normalization(float2*, int)+0x188>
 	mov    %edx,%ecx
 	movaps %xmm3,%xmm1
 	mov    %rdi,%rax
 	shr    $1,%ecx
 	shufps $0x0,%xmm1,%xmm1
 	shl    $0x4,%rcx
 	add    %rdi,%rcx
 	nopl   0x0(%rax)
 	movups (%rax),%xmm0
 	add    $0x10,%rax
 	divps  %xmm1,%xmm0
 	movups %xmm0,-0x10(%rax)
 	cmp    %rcx,%rax
-	jne    3ec8 <normalization(float2*, int)+0x138>
+	jne    3ee8 <normalization(float2*, int)+0x138>
 	mov    %edx,%ecx
 	and    $0xfffffffe,%ecx
 	and    $0x1,%edx
-	je     3f10 <normalization(float2*, int)+0x180>
+	je     3f30 <normalization(float2*, int)+0x180>
 	movslq %ecx,%rcx
 	lea    (%rdi,%rcx,8),%rax
 	movss  (%rax),%xmm0
 	divss  %xmm3,%xmm0
 	movss  %xmm0,(%rax)
 	movss  0x4(%rax),%xmm0
 	divss  %xmm3,%xmm0
 	movss  %xmm0,0x4(%rax)
 	ret
 	nopw   0x0(%rax,%rax,1)
 	ret
 	nopl   0x0(%rax)
-	movss  0x23c4(%rip),%xmm0        
+	movss  0x23d4(%rip),%xmm0        
 	mov    %r8d,%r8d
 	mov    %edx,%edx
 	xor    %eax,%eax
-	jmp    3f40 <normalization(float2*, int)+0x1b0>
+	jmp    3f60 <normalization(float2*, int)+0x1b0>
 	nopl   0x0(%rax)
 	movl   $0x0,(%rdi,%rax,8)
 	add    $0x1,%rax
 	cmp    %rdx,%rax
-	je     3f52 <normalization(float2*, int)+0x1c2>
+	je     3f72 <normalization(float2*, int)+0x1c2>
 	test   %rax,%rax
-	jne    3f30 <normalization(float2*, int)+0x1a0>
+	jne    3f50 <normalization(float2*, int)+0x1a0>
 	add    $0x1,%rax
 	movss  %xmm0,(%rdi)
 	cmp    %rdx,%rax
-	jne    3f40 <normalization(float2*, int)+0x1b0>
+	jne    3f60 <normalization(float2*, int)+0x1b0>
 	lea    0x4(%rdi),%rax
 	lea    0xc(%rdi,%r8,8),%rdx
 	nopl   0x0(%rax,%rax,1)
 	movl   $0x0,(%rax)
 	add    $0x8,%rax
 	cmp    %rdx,%rax
-	jne    3f60 <normalization(float2*, int)+0x1d0>
+	jne    3f80 <normalization(float2*, int)+0x1d0>
 	ret
-	movsd  0x2378(%rip),%xmm1        
+	movsd  0x2388(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
 	cvtss2sd %xmm3,%xmm0
 	comisd %xmm0,%xmm1
-	ja     3f18 <normalization(float2*, int)+0x188>
+	ja     3f38 <normalization(float2*, int)+0x188>
 	test   %ecx,%ecx
-	je     3ee5 <normalization(float2*, int)+0x155>
-	jmp    3eac <normalization(float2*, int)+0x11c>
+	je     3f05 <normalization(float2*, int)+0x155>
+	jmp    3ecc <normalization(float2*, int)+0x11c>
 	xor    %eax,%eax
 	pxor   %xmm3,%xmm3
-	jmp    3e25 <normalization(float2*, int)+0x95>
+	jmp    3e45 <normalization(float2*, int)+0x95>
 	xchg   %ax,%ax
 
-0000000000003fa0 <execute_circuit>:
+0000000000003fc0 <execute_circuit>:
 execute_circuit():
 	endbr64
 	push   %r15
 	mov    %rsi,%r9
-	lea    0x209c(%rip),%rsi        
+	lea    0x2032(%rip),%rsi        
 	push   %r14
-	movq   %rsi,%xmm0
-	lea    0x2044(%rip),%rsi        
 	push   %r13
 	push   %r12
 	mov    %ecx,%r12d
-	lea    0x2048(%rip),%rcx        
+	lea    0x2062(%rip),%rcx        
 	push   %rbp
+	movq   %rcx,%xmm0
+	lea    0x2041(%rip),%rcx        
 	mov    %rdi,%rbp
-	lea    0x2057(%rip),%rdi        
 	push   %rbx
+	lea    0x2016(%rip),%rdi        
 	sub    $0xf8,%rsp
 	mov    %fs:0x28,%rax
 	mov    %rax,0xe8(%rsp)
-	lea    0x201b(%rip),%rax        
+	lea    0x1ffb(%rip),%rax        
 	movq   %rax,%xmm1
-	lea    0x1ffd(%rip),%rax        
+	lea    0x1fdd(%rip),%rax        
 	punpcklqdq %xmm1,%xmm0
 	movq   %rax,%xmm2
-	lea    0x1ff3(%rip),%rax        
+	lea    0x1fd3(%rip),%rax        
 	movaps %xmm0,0x70(%rsp)
-	movq   %rdi,%xmm0
+	movq   %rcx,%xmm0
 	movq   %rax,%xmm3
-	lea    0x1fdf(%rip),%rdi        
+	lea    0x1fbf(%rip),%rcx        
 	punpcklqdq %xmm2,%xmm0
-	lea    0x1fd8(%rip),%rax        
+	lea    0x1fb8(%rip),%rax        
 	movaps %xmm0,0x80(%rsp)
 	movq   %rsi,%xmm0
 	movq   %rax,%xmm4
-	lea    0x1fc1(%rip),%rsi        
+	lea    0x1fa4(%rip),%rax        
 	punpcklqdq %xmm3,%xmm0
-	lea    0x1fb9(%rip),%rax        
-	movaps %xmm0,0x90(%rsp)
-	movq   %rdi,%xmm0
 	movq   %rax,%xmm5
-	lea    0x1fa6(%rip),%rax        
+	lea    0x1f97(%rip),%rsi        
+	movaps %xmm0,0x90(%rsp)
+	movq   %rcx,%xmm0
+	lea    0x1f86(%rip),%rax        
+	lea    0x1f86(%rip),%rcx        
 	punpcklqdq %xmm4,%xmm0
 	movq   %rax,%xmm6
-	lea    0x1f9d(%rip),%rdi        
+	lea    0x1f79(%rip),%rax        
 	movaps %xmm0,0xa0(%rsp)
-	movq   %rsi,%xmm0
-	lea    0x1f8c(%rip),%rax        
-	lea    0x1fa9(%rip),%rsi        
-	punpcklqdq %xmm5,%xmm0
+	movq   %rdi,%xmm0
 	movq   %rax,%xmm7
-	lea    0x1f78(%rip),%rax        
+	lea    0x1f84(%rip),%rdi        
+	punpcklqdq %xmm5,%xmm0
+	lea    0x1f58(%rip),%rax        
 	movaps %xmm0,0xb0(%rsp)
-	movq   %rcx,%xmm0
+	movq   %rsi,%xmm0
 	movq   %rax,%xmm1
-	lea    0x1f65(%rip),%rcx        
+	lea    0x1f45(%rip),%rsi        
 	punpcklqdq %xmm6,%xmm0
-	lea    0x1f7b(%rip),%rax        
+	lea    0x1f51(%rip),%rax        
 	movaps %xmm0,0xc0(%rsp)
-	movq   %rdi,%xmm0
+	movq   %rcx,%xmm0
 	movq   %rax,%xmm2
-	lea    0x1f44(%rip),%rdi        
+	lea    0x1f24(%rip),%rcx        
 	punpcklqdq %xmm7,%xmm0
-	lea    0x1f3c(%rip),%rax        
+	lea    0x1f1c(%rip),%rax        
 	movaps %xmm0,0xd0(%rsp)
-	movq   %rsi,%xmm0
+	movq   %rdi,%xmm0
 	movq   %rax,%xmm3
-	lea    0x1f27(%rip),%rsi        
+	lea    0x1f07(%rip),%rdi        
 	punpcklqdq %xmm1,%xmm0
-	lea    0x1f20(%rip),%rax        
+	lea    0x1f00(%rip),%rax        
 	movaps %xmm0,0x20(%rsp)
-	movq   %rcx,%xmm0
+	movq   %rsi,%xmm0
 	movq   %rax,%xmm4
-	lea    0x1f0e(%rip),%rax        
+	lea    0x1eee(%rip),%rax        
 	punpcklqdq %xmm2,%xmm0
 	mov    %rax,0x60(%rsp)
-	lea    0x1f02(%rip),%rcx        
-	lea    0x1eff(%rip),%rax        
+	lea    0x1ee2(%rip),%rsi        
+	lea    0x1edf(%rip),%rax        
 	movaps %xmm0,0x30(%rsp)
-	movq   %rdi,%xmm0
+	movq   %rcx,%xmm0
 	movq   %rax,%xmm5
 	punpcklqdq %xmm3,%xmm0
 	movaps %xmm0,0x40(%rsp)
-	movq   %rsi,%xmm0
+	movq   %rdi,%xmm0
 	punpcklqdq %xmm4,%xmm0
 	movaps %xmm0,0x50(%rsp)
-	movq   %rcx,%xmm0
+	movq   %rsi,%xmm0
 	punpcklqdq %xmm5,%xmm0
 	movaps %xmm0,0x10(%rsp)
 	test   %edx,%edx
-	jle    4210 <execute_circuit+0x270>
+	jle    4248 <execute_circuit+0x288>
 	lea    -0x1(%rdx),%eax
 	mov    %r8d,%r13d
 	lea    0x70(%rsp),%r14
 	mov    %r9,%r15
 	lea    (%rax,%rax,2),%rax
 	lea    0x18(%r9,%rax,8),%rax
 	mov    %rax,(%rsp)
 	lea    0x20(%rsp),%rax
 	mov    %rax,0x8(%rsp)
-	jmp    41d9 <execute_circuit+0x239>
+	jmp    41f9 <execute_circuit+0x239>
 	nopl   0x0(%rax,%rax,1)
-	mov    0x9e01(%rip),%rbx        
+	mov    0x9de1(%rip),%rbx        
 	movss  0x10(%r15),%xmm0
 	mov    0x8(%r15),%rcx
 	mov    %r13d,%r8d
 	mov    %r12d,%edx
 	mov    (%r15),%rdi
 	mov    %rbp,%rsi
 	add    $0x18,%r15
 	call   *%rbx
 	cmp    %r15,(%rsp)
-	je     4210 <execute_circuit+0x270>
+	je     4248 <execute_circuit+0x288>
+	mov    (%r15),%rdx
+	lea    0x1e47(%rip),%rsi        
+	mov    $0x1,%edi
+	xor    %eax,%eax
+	call   2710 <__printf_chk@plt>
 	mov    (%r15),%rsi
 	mov    $0xe,%edx
 	mov    %r14,%rdi
-	call   2520 <isInArray(char const**, char*, int)@plt>
+	call   2530 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	jne    41b0 <execute_circuit+0x210>
+	jne    41d0 <execute_circuit+0x210>
 	mov    (%r15),%rsi
 	mov    0x8(%rsp),%rdi
 	mov    $0x9,%edx
-	call   2520 <isInArray(char const**, char*, int)@plt>
+	call   2530 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     4238 <execute_circuit+0x298>
-	mov    0x9db6(%rip),%rbx        
-	jmp    41b7 <execute_circuit+0x217>
-	nopl   0x0(%rax)
+	je     4270 <execute_circuit+0x2b0>
+	mov    0x9d80(%rip),%rbx        
+	jmp    41d7 <execute_circuit+0x217>
+	nopw   0x0(%rax,%rax,1)
 	mov    0xe8(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    425e <execute_circuit+0x2be>
+	jne    4296 <execute_circuit+0x2d6>
 	add    $0xf8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   (%rax)
 	mov    (%r15),%rsi
 	lea    0x10(%rsp),%rdi
 	mov    $0x2,%edx
-	call   2520 <isInArray(char const**, char*, int)@plt>
+	call   2530 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     41b7 <execute_circuit+0x217>
-	mov    0x9d57(%rip),%rbx        
-	jmp    41b7 <execute_circuit+0x217>
-	call   2540 <__stack_chk_fail@plt>
-	data16 cs nopw 0x0(%rax,%rax,1)
-	xchg   %ax,%ax
+	je     41d7 <execute_circuit+0x217>
+	mov    0x9d1f(%rip),%rbx        
+	jmp    41d7 <execute_circuit+0x217>
+	call   2550 <__stack_chk_fail@plt>
+	nopl   0x0(%rax,%rax,1)
 
-0000000000004270 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
+00000000000042a0 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
 __device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*):
 	endbr64
 	sub    $0xa8,%rsp
 	mov    %rdi,0x18(%rsp)
 	lea    0x38(%rsp),%rdi
 	mov    %rsi,0x10(%rsp)
 	lea    0x48(%rsp),%rsi
@@ -1621,147 +1625,147 @@
 	mov    %rsp,%rax
 	movq   %rax,%xmm2
 	mov    0x1ffd(%rip),%rax        
 	punpcklqdq %xmm2,%xmm0
 	mov    %rax,0x38(%rsp)
 	mov    %rax,0x48(%rsp)
 	movaps %xmm0,0x80(%rsp)
-	call   2810 <__cudaPopCallConfiguration@plt>
+	call   2830 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
-	jne    434b <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xdb>
+	jne    437b <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xdb>
 	push   0x30(%rsp)
-	mov    0x9cd3(%rip),%rdi        
+	mov    0x9ca3(%rip),%rdi        
 	push   0x30(%rsp)
 	mov    0x58(%rsp),%rcx
 	mov    0x60(%rsp),%r8d
 	mov    0x48(%rsp),%rsi
 	mov    0x50(%rsp),%edx
 	lea    0x80(%rsp),%r9
-	call   26f0 <cudaLaunchKernel@plt>
+	call   2700 <cudaLaunchKernel@plt>
 	pop    %rax
 	pop    %rdx
 	mov    0x98(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    4366 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xf6>
+	jne    4396 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xf6>
 	add    $0xa8,%rsp
 	ret
-	call   2540 <__stack_chk_fail@plt>
+	call   2550 <__stack_chk_fail@plt>
 	nopl   0x0(%rax,%rax,1)
 
-0000000000004370 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)>:
+00000000000043a0 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)>:
 actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*):
 	endbr64
-	jmp    2560 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    2570 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
 	nopl   0x0(%rax)
 
-0000000000004380 <singleGateAction>:
+00000000000043b0 <singleGateAction>:
 singleGateAction():
 	endbr64
 	push   %r15
 	push   %r14
 	mov    %rdi,%r14
 	mov    %rcx,%rdi
 	push   %r13
 	mov    %rsi,%r13
-	lea    0x1c7a(%rip),%rsi        
+	lea    0x1c4a(%rip),%rsi        
 	push   %r12
 	push   %rbp
 	mov    %r8d,%ebp
 	push   %rbx
-	lea    0x1ca4(%rip),%rbx        
+	lea    0x1c6a(%rip),%rbx        
 	sub    $0xd8,%rsp
 	mov    %edx,0x4(%rsp)
-	lea    0x1c4e(%rip),%rdx        
+	lea    0x1c1e(%rip),%rdx        
 	mov    %rcx,0x10(%rsp)
 	movss  %xmm0,0x1c(%rsp)
 	movq   %rbx,%xmm0
-	lea    0x1c5d(%rip),%rbx        
+	lea    0x1c2d(%rip),%rbx        
 	mov    %fs:0x28,%rax
 	mov    %rax,0xc8(%rsp)
-	lea    0x1c29(%rip),%rax        
+	lea    0x1bf9(%rip),%rax        
 	movq   %rax,%xmm1
-	lea    0x1c0b(%rip),%rax        
+	lea    0x1bdb(%rip),%rax        
 	punpcklqdq %xmm1,%xmm0
 	movq   %rax,%xmm2
-	lea    0x1c01(%rip),%rax        
+	lea    0x1bd1(%rip),%rax        
 	movaps %xmm0,0x50(%rsp)
 	movq   %rbx,%xmm0
 	movq   %rax,%xmm3
-	lea    0x1be7(%rip),%rbx        
+	lea    0x1bb7(%rip),%rbx        
 	punpcklqdq %xmm2,%xmm0
-	lea    0x1be6(%rip),%rax        
+	lea    0x1bb6(%rip),%rax        
 	movaps %xmm0,0x60(%rsp)
 	movq   %rbx,%xmm0
 	movq   %rax,%xmm4
-	lea    0x1bd2(%rip),%rbx        
+	lea    0x1ba2(%rip),%rbx        
 	punpcklqdq %xmm3,%xmm0
-	lea    0x1bca(%rip),%rax        
+	lea    0x1b9a(%rip),%rax        
 	movaps %xmm0,0x70(%rsp)
 	movq   %rdx,%xmm0
 	movq   %rax,%xmm5
-	lea    0x1bba(%rip),%rax        
+	lea    0x1b8a(%rip),%rax        
 	punpcklqdq %xmm4,%xmm0
 	movq   %rax,%xmm6
-	lea    0x1bb1(%rip),%rdx        
+	lea    0x1b81(%rip),%rdx        
 	movaps %xmm0,0x80(%rsp)
 	movq   %rbx,%xmm0
-	lea    0x1ba0(%rip),%rax        
+	lea    0x1b70(%rip),%rax        
 	punpcklqdq %xmm5,%xmm0
 	movq   %rax,%xmm7
 	movaps %xmm0,0x90(%rsp)
 	movq   %rsi,%xmm0
 	punpcklqdq %xmm6,%xmm0
 	movaps %xmm0,0xa0(%rsp)
 	movq   %rdx,%xmm0
 	punpcklqdq %xmm7,%xmm0
 	movaps %xmm0,0xb0(%rsp)
-	call   26e0 <getArrayLength(int*)@plt>
+	call   26f0 <getArrayLength(int*)@plt>
 	cmp    $0x1,%eax
-	jne    491a <singleGateAction+0x59a>
+	jne    494a <singleGateAction+0x59a>
 	mov    %ebp,%edi
 	mov    %eax,%ebx
-	call   2740 <cudaSetDevice@plt>
+	call   2760 <cudaSetDevice@plt>
 	mov    $0x20,%edi
-	call   26a0 <malloc@plt>
+	call   26b0 <malloc@plt>
 	mov    $0x8,%edi
 	mov    %rax,%r12
-	call   26a0 <malloc@plt>
+	call   26b0 <malloc@plt>
 	movzbl 0x4(%rsp),%ecx
 	lea    0x20(%rsp),%rdi
 	mov    $0x20,%esi
 	movq   $0x0,0x20(%rsp)
 	mov    %rax,%rbp
 	mov    %ebx,%eax
 	movq   $0x0,0x28(%rsp)
 	shl    %cl,%eax
 	movq   $0x0,0x30(%rsp)
 	cltq
 	lea    0x0(,%rax,8),%r15
 	mov    %rax,0x8(%rsp)
-	call   26d0 <cudaMalloc@plt>
+	call   26e0 <cudaMalloc@plt>
 	lea    0x28(%rsp),%rdi
 	mov    %r15,%rsi
-	call   26d0 <cudaMalloc@plt>
+	call   26e0 <cudaMalloc@plt>
 	lea    0x30(%rsp),%rdi
 	mov    $0x8,%esi
-	call   26d0 <cudaMalloc@plt>
+	call   26e0 <cudaMalloc@plt>
 	mov    0x28(%rsp),%rdi
 	mov    %r15,%rdx
 	mov    %r13,%rsi
 	mov    $0x1,%ecx
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    %r14,%rdi
-	call   2790 <hash(char const*)@plt>
+	call   27b0 <hash(char const*)@plt>
 	lea    0x50(%rsp),%rdi
 	mov    $0xe,%edx
 	mov    %r14,%rsi
 	mov    %eax,0x18(%rsp)
-	call   2520 <isInArray(char const**, char*, int)@plt>
+	call   2530 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     48e2 <singleGateAction+0x562>
+	je     4912 <singleGateAction+0x562>
 	mov    0x10(%rsp),%rsi
 	mov    0x30(%rsp),%rdi
 	mov    (%rsi),%ecx
 	mov    %ebx,%esi
 	shl    %cl,%esi
 	add    $0x1,%ecx
 	movslq %esi,%rax
@@ -1778,201 +1782,201 @@
 	div    %rcx
 	mov    $0x1,%ecx
 	mov    $0x8,%edx
 	add    $0x1,%eax
 	mov    %eax,0x44(%rsp)
 	movabs $0x100000001,%rax
 	mov    %rax,0x48(%rsp)
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    0x18(%rsp),%r8d
 	cmp    $0x1bd,%r8d
-	je     4890 <singleGateAction+0x510>
-	ja     4790 <singleGateAction+0x410>
+	je     48c0 <singleGateAction+0x510>
+	ja     47c0 <singleGateAction+0x410>
 	cmp    $0x7d,%r8d
-	ja     4700 <singleGateAction+0x380>
+	ja     4730 <singleGateAction+0x380>
 	cmp    $0x6a,%r8d
-	jbe    4650 <singleGateAction+0x2d0>
+	jbe    4680 <singleGateAction+0x2d0>
 	sub    $0x6b,%r8d
 	cmp    $0x12,%r8d
-	ja     4650 <singleGateAction+0x2d0>
-	lea    0x1a37(%rip),%rdx        
+	ja     4680 <singleGateAction+0x2d0>
+	lea    0x1a27(%rip),%rdx        
 	movslq (%rdx,%r8,4),%rax
 	add    %rdx,%rax
 	notrack jmp *%rax
 	nopl   0x0(%rax,%rax,1)
 	cmp    $0x1d8,%r8d
-	je     48b8 <singleGateAction+0x538>
+	je     48e8 <singleGateAction+0x538>
 	cmp    $0x1d9,%r8d
-	jne    47d0 <singleGateAction+0x450>
+	jne    4800 <singleGateAction+0x450>
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   2670 <rz_gate(float2*, float)@plt>
+	call   2680 <rz_gate(float2*, float)@plt>
 	mov    0x20(%rsp),%rdi
 	mov    $0x1,%ecx
 	mov    $0x20,%edx
 	mov    %r12,%rsi
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    %ebx,0x38(%rsp)
 	mov    0x40(%rsp),%ecx
 	xor    %r9d,%r9d
 	mov    0x38(%rsp),%rdx
 	mov    0x44(%rsp),%rdi
 	xor    %r8d,%r8d
 	mov    0x4c(%rsp),%esi
-	call   27b0 <__cudaPushCallConfiguration@plt>
+	call   27d0 <__cudaPushCallConfiguration@plt>
 	test   %eax,%eax
-	je     47f0 <singleGateAction+0x470>
-	call   2600 <cudaDeviceSynchronize@plt>
+	je     4820 <singleGateAction+0x470>
+	call   2610 <cudaDeviceSynchronize@plt>
 	mov    0x28(%rsp),%rsi
 	mov    %r15,%rdx
 	mov    %r13,%rdi
 	mov    $0x2,%ecx
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    0x20(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    %r12,%rdi
-	call   2480 <free@plt>
+	call   2490 <free@plt>
 	mov    0xc8(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    48dd <singleGateAction+0x55d>
+	jne    490d <singleGateAction+0x55d>
 	add    $0xd8,%rsp
 	mov    %rbp,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
-	jmp    2480 <free@plt>
+	jmp    2490 <free@plt>
 	cmp    $0x190,%r8d
-	jne    4650 <singleGateAction+0x2d0>
+	jne    4680 <singleGateAction+0x2d0>
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   27e0 <ad_gate(float2*, float)@plt>
+	call   2800 <ad_gate(float2*, float)@plt>
 	mov    0x20(%rsp),%rdi
 	mov    $0x1,%ecx
 	mov    $0x20,%edx
 	mov    %r12,%rsi
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    %ebx,0x38(%rsp)
 	mov    0x40(%rsp),%ecx
 	xor    %r9d,%r9d
 	mov    0x38(%rsp),%rdx
 	mov    0x44(%rsp),%rdi
 	xor    %r8d,%r8d
 	mov    0x4c(%rsp),%esi
-	call   27b0 <__cudaPushCallConfiguration@plt>
+	call   27d0 <__cudaPushCallConfiguration@plt>
 	test   %eax,%eax
-	je     4810 <singleGateAction+0x490>
-	call   2600 <cudaDeviceSynchronize@plt>
+	je     4840 <singleGateAction+0x490>
+	call   2610 <cudaDeviceSynchronize@plt>
 	mov    0x28(%rsp),%rsi
 	mov    %r13,%rdi
 	mov    %r15,%rdx
 	mov    $0x2,%ecx
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    0x4(%rsp),%esi
 	mov    %r13,%rdi
-	call   26b0 <normalization(float2*, int)@plt>
-	jmp    46aa <singleGateAction+0x32a>
+	call   26c0 <normalization(float2*, int)@plt>
+	jmp    46da <singleGateAction+0x32a>
 	cs nopw 0x0(%rax,%rax,1)
 	cmp    $0x5b9,%r8d
-	je     48d0 <singleGateAction+0x550>
-	jbe    4628 <singleGateAction+0x2a8>
+	je     4900 <singleGateAction+0x550>
+	jbe    4658 <singleGateAction+0x2a8>
 	cmp    $0x5c2,%r8d
-	je     48a8 <singleGateAction+0x528>
+	je     48d8 <singleGateAction+0x528>
 	cmp    $0x914b,%r8d
-	jne    4650 <singleGateAction+0x2d0>
+	jne    4680 <singleGateAction+0x2d0>
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   2630 <damp_i_gate(float2*, float)@plt>
-	jmp    471b <singleGateAction+0x39b>
+	call   2640 <damp_i_gate(float2*, float)@plt>
+	jmp    474b <singleGateAction+0x39b>
 	cmp    $0x1d7,%r8d
-	jne    4650 <singleGateAction+0x2d0>
+	jne    4680 <singleGateAction+0x2d0>
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   2730 <rx_gate(float2*, float)@plt>
-	jmp    4650 <singleGateAction+0x2d0>
+	call   2750 <rx_gate(float2*, float)@plt>
+	jmp    4680 <singleGateAction+0x2d0>
 	mov    0x30(%rsp),%rcx
 	mov    0x8(%rsp),%rdx
 	mov    0x20(%rsp),%rsi
 	mov    0x28(%rsp),%rdi
-	call   2440 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
-	jmp    4690 <singleGateAction+0x310>
+	call   2450 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    46c0 <singleGateAction+0x310>
 	xchg   %ax,%ax
 	mov    0x30(%rsp),%rcx
 	mov    0x8(%rsp),%rdx
 	mov    0x20(%rsp),%rsi
 	mov    0x28(%rsp),%rdi
-	call   2440 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
-	jmp    475b <singleGateAction+0x3db>
+	call   2450 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    478b <singleGateAction+0x3db>
 	xchg   %ax,%ax
 	mov    %r12,%rdi
-	call   2550 <z_gate(float2*)@plt>
-	jmp    4650 <singleGateAction+0x2d0>
+	call   2560 <z_gate(float2*)@plt>
+	jmp    4680 <singleGateAction+0x2d0>
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   2820 <x_gate(float2*)@plt>
-	jmp    4650 <singleGateAction+0x2d0>
+	call   2840 <x_gate(float2*)@plt>
+	jmp    4680 <singleGateAction+0x2d0>
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   2720 <y_gate(float2*)@plt>
-	jmp    4650 <singleGateAction+0x2d0>
+	call   2740 <y_gate(float2*)@plt>
+	jmp    4680 <singleGateAction+0x2d0>
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   2570 <h_gate(float2*)@plt>
-	jmp    4650 <singleGateAction+0x2d0>
+	call   2580 <h_gate(float2*)@plt>
+	jmp    4680 <singleGateAction+0x2d0>
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   26c0 <s_gate(float2*)@plt>
-	jmp    4650 <singleGateAction+0x2d0>
+	call   26d0 <s_gate(float2*)@plt>
+	jmp    4680 <singleGateAction+0x2d0>
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   24b0 <t_gate(float2*)@plt>
-	jmp    4650 <singleGateAction+0x2d0>
+	call   24c0 <t_gate(float2*)@plt>
+	jmp    4680 <singleGateAction+0x2d0>
 	nopl   (%rax)
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   24d0 <pd_gate(float2*, float)@plt>
-	jmp    471b <singleGateAction+0x39b>
+	call   24e0 <pd_gate(float2*, float)@plt>
+	jmp    474b <singleGateAction+0x39b>
 	nopl   0x0(%rax,%rax,1)
 	mov    %r12,%rdi
-	call   2680 <tdg_gate(float2*)@plt>
-	jmp    4650 <singleGateAction+0x2d0>
+	call   2690 <tdg_gate(float2*)@plt>
+	jmp    4680 <singleGateAction+0x2d0>
 	nopl   (%rax)
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   2470 <ry_gate(float2*, float)@plt>
-	jmp    4650 <singleGateAction+0x2d0>
+	call   2480 <ry_gate(float2*, float)@plt>
+	jmp    4680 <singleGateAction+0x2d0>
 	nopl   0x0(%rax,%rax,1)
 	mov    %r12,%rdi
-	call   2700 <sdg_gate(float2*)@plt>
-	jmp    4650 <singleGateAction+0x2d0>
-	call   2540 <__stack_chk_fail@plt>
+	call   2720 <sdg_gate(float2*)@plt>
+	jmp    4680 <singleGateAction+0x2d0>
+	call   2550 <__stack_chk_fail@plt>
 	mov    0x20(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    %r12,%rdi
-	call   2480 <free@plt>
+	call   2490 <free@plt>
 	mov    %rbp,%rdi
-	call   2480 <free@plt>
+	call   2490 <free@plt>
 	mov    $0x3,%edi
-	call   2780 <exit@plt>
+	call   27a0 <exit@plt>
 	mov    $0x1,%edi
-	call   2780 <exit@plt>
+	call   27a0 <exit@plt>
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nop
 
-0000000000004930 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000004960 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
 __device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*):
 	endbr64
 	sub    $0xa8,%rsp
 	mov    %rdi,0x18(%rsp)
 	lea    0x38(%rsp),%rdi
 	mov    %rsi,0x10(%rsp)
 	lea    0x48(%rsp),%rsi
@@ -1996,158 +2000,164 @@
 	mov    %rsp,%rax
 	movq   %rax,%xmm2
 	mov    0x193d(%rip),%rax        
 	punpcklqdq %xmm2,%xmm0
 	mov    %rax,0x38(%rsp)
 	mov    %rax,0x48(%rsp)
 	movaps %xmm0,0x80(%rsp)
-	call   2810 <__cudaPopCallConfiguration@plt>
+	call   2830 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
-	jne    4a0b <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xdb>
+	jne    4a3b <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xdb>
 	push   0x30(%rsp)
-	mov    0x95e3(%rip),%rdi        
+	mov    0x95b3(%rip),%rdi        
 	push   0x30(%rsp)
 	mov    0x58(%rsp),%rcx
 	mov    0x60(%rsp),%r8d
 	mov    0x48(%rsp),%rsi
 	mov    0x50(%rsp),%edx
 	lea    0x80(%rsp),%r9
-	call   26f0 <cudaLaunchKernel@plt>
+	call   2700 <cudaLaunchKernel@plt>
 	pop    %rax
 	pop    %rdx
 	mov    0x98(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    4a26 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xf6>
+	jne    4a56 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xf6>
 	add    $0xa8,%rsp
 	ret
-	call   2540 <__stack_chk_fail@plt>
+	call   2550 <__stack_chk_fail@plt>
 	nopl   0x0(%rax,%rax,1)
 
-0000000000004a30 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000004a60 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)>:
 actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*):
 	endbr64
-	jmp    2590 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    25a0 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
 	nopl   0x0(%rax)
 
-0000000000004a40 <doubleGateAction>:
+0000000000004a70 <doubleGateAction>:
 doubleGateAction():
 	endbr64
 	push   %r15
 	push   %r14
 	mov    %rdi,%r14
 	mov    %rcx,%rdi
 	push   %r13
 	mov    %edx,%r13d
 	push   %r12
+	mov    %r8d,%r12d
 	push   %rbp
-	mov    %r8d,%ebp
 	push   %rbx
 	mov    %rcx,%rbx
 	sub    $0xa8,%rsp
 	mov    %rsi,(%rsp)
-	lea    0x15d6(%rip),%rsi        
+	lea    0x15a6(%rip),%rsi        
 	movss  %xmm0,0x14(%rsp)
 	movq   %rsi,%xmm0
-	lea    0x15a9(%rip),%rsi        
+	lea    0x1579(%rip),%rsi        
 	mov    %fs:0x28,%rax
 	mov    %rax,0x98(%rsp)
-	lea    0x158b(%rip),%rax        
+	lea    0x155b(%rip),%rax        
 	movq   %rax,%xmm1
-	lea    0x15a6(%rip),%rax        
+	lea    0x156c(%rip),%rax        
 	punpcklqdq %xmm1,%xmm0
 	movq   %rax,%xmm2
-	lea    0x157b(%rip),%rax        
+	lea    0x154b(%rip),%rax        
 	movaps %xmm0,0x50(%rsp)
 	movq   %rsi,%xmm0
 	movq   %rax,%xmm3
-	lea    0x1562(%rip),%rsi        
+	lea    0x1532(%rip),%rsi        
 	punpcklqdq %xmm2,%xmm0
-	lea    0x1562(%rip),%rax        
+	lea    0x1532(%rip),%rax        
 	movaps %xmm0,0x60(%rsp)
 	movq   %rsi,%xmm0
 	movq   %rax,%xmm4
-	lea    0x1548(%rip),%rsi        
+	lea    0x1518(%rip),%rsi        
 	punpcklqdq %xmm3,%xmm0
-	lea    0x1545(%rip),%rax        
+	lea    0x1515(%rip),%rax        
 	movaps %xmm0,0x70(%rsp)
 	movq   %rsi,%xmm0
 	punpcklqdq %xmm4,%xmm0
 	mov    %rax,0x90(%rsp)
 	movaps %xmm0,0x80(%rsp)
-	call   26e0 <getArrayLength(int*)@plt>
-	cmp    $0x2,%eax
-	jne    4eb7 <doubleGateAction+0x477>
+	call   26f0 <getArrayLength(int*)@plt>
+	lea    0x1507(%rip),%rsi        
+	mov    $0x1,%edi
+	mov    %eax,%ebp
+	mov    %eax,%edx
+	xor    %eax,%eax
+	call   2710 <__printf_chk@plt>
+	cmp    $0x2,%ebp
+	jne    4ef7 <doubleGateAction+0x487>
 	mov    0x4(%rbx),%eax
 	cmp    %eax,(%rbx)
-	je     4f05 <doubleGateAction+0x4c5>
-	mov    %ebp,%edi
-	call   2740 <cudaSetDevice@plt>
+	je     4f4f <doubleGateAction+0x4df>
+	mov    %r12d,%edi
+	call   2760 <cudaSetDevice@plt>
 	mov    $0x80,%edi
-	call   26a0 <malloc@plt>
+	call   26b0 <malloc@plt>
 	mov    $0x10,%edi
 	mov    %rax,%r12
-	call   26a0 <malloc@plt>
+	call   26b0 <malloc@plt>
 	mov    $0x1,%r10d
 	mov    %r13d,%ecx
 	lea    0x20(%rsp),%rdi
 	mov    %rax,%rbp
 	mov    %r10d,%eax
 	mov    $0x80,%esi
 	movq   $0x0,0x20(%rsp)
 	movq   $0x0,0x28(%rsp)
 	shl    %cl,%eax
 	movq   $0x0,0x30(%rsp)
 	cltq
 	lea    0x0(,%rax,8),%r15
 	mov    %rax,0x8(%rsp)
-	call   26d0 <cudaMalloc@plt>
+	call   26e0 <cudaMalloc@plt>
 	lea    0x28(%rsp),%rdi
 	mov    %r15,%rsi
-	call   26d0 <cudaMalloc@plt>
+	call   26e0 <cudaMalloc@plt>
 	lea    0x30(%rsp),%rdi
 	mov    $0x10,%esi
-	call   26d0 <cudaMalloc@plt>
+	call   26e0 <cudaMalloc@plt>
 	mov    (%rsp),%rsi
 	mov    0x28(%rsp),%rdi
 	mov    %r15,%rdx
 	mov    $0x1,%ecx
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    %r14,%rdi
-	call   2790 <hash(char const*)@plt>
+	call   27b0 <hash(char const*)@plt>
 	mov    (%rbx),%ecx
 	mov    0x4(%rbx),%esi
 	mov    $0x4,%edx
 	mov    %rbx,%rdi
 	mov    %eax,%r13d
 	mov    %ecx,0x18(%rsp)
-	mov    0x93fd(%rip),%rcx        
+	mov    0x93b5(%rip),%rcx        
 	mov    %esi,0x1c(%rsp)
 	mov    $0x2,%esi
-	call   24f0 <qsort@plt>
+	call   2500 <qsort@plt>
 	lea    0x50(%rsp),%rdi
 	mov    $0x9,%edx
 	mov    %r14,%rsi
-	call   2520 <isInArray(char const**, char*, int)@plt>
+	call   2530 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     4ecd <doubleGateAction+0x48d>
+	je     4f17 <doubleGateAction+0x4a7>
 	mov    (%rbx),%eax
 	mov    $0x1,%r10d
 	mov    0x30(%rsp),%rdi
 	mov    %rbp,%rsi
 	mov    %r10d,%edx
 	mov    %eax,%ecx
 	shl    %cl,%edx
 	mov    0x4(%rbx),%ecx
 	mov    %r10d,%ebx
 	movslq %edx,%rdx
 	mov    %rdx,0x0(%rbp)
 	mov    %r10d,%edx
 	shl    %cl,%edx
 	lea    0x1(%rax),%ecx
-	mov    0x16b2(%rip),%rax        
+	mov    0x169a(%rip),%rax        
 	shl    %cl,%ebx
 	movslq %edx,%rdx
 	mov    %rax,0x3c(%rsp)
 	mov    0x8(%rsp),%rax
 	mov    %ebx,%ecx
 	mov    %rdx,0x8(%rbp)
 	movslq %ebx,%rdx
@@ -2156,153 +2166,156 @@
 	div    %rcx
 	mov    $0x1,%ecx
 	mov    $0x10,%edx
 	add    $0x1,%eax
 	mov    %eax,0x44(%rsp)
 	movabs $0x100000001,%rax
 	mov    %rax,0x48(%rsp)
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	cmp    $0x5fd,%r13d
-	je     4e80 <doubleGateAction+0x440>
-	jbe    4d80 <doubleGateAction+0x340>
+	je     4ec0 <doubleGateAction+0x450>
+	jbe    4dc8 <doubleGateAction+0x358>
 	cmp    $0x1234,%r13d
-	je     4e40 <doubleGateAction+0x400>
-	jbe    4db0 <doubleGateAction+0x370>
+	je     4e80 <doubleGateAction+0x410>
+	jbe    4df8 <doubleGateAction+0x388>
 	cmp    $0x340f,%r13d
-	jne    4cc8 <doubleGateAction+0x288>
+	jne    4d10 <doubleGateAction+0x2a0>
 	mov    %r12,%rdi
-	call   2650 <iswap_gate(float2*)@plt>
+	call   2660 <iswap_gate(float2*)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x20(%rsp),%rdi
 	mov    $0x1,%ecx
 	mov    $0x80,%edx
 	mov    %r12,%rsi
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    %ebx,0x38(%rsp)
 	mov    0x40(%rsp),%ecx
 	xor    %r9d,%r9d
 	mov    0x38(%rsp),%rdx
 	mov    0x44(%rsp),%rdi
 	xor    %r8d,%r8d
 	mov    0x4c(%rsp),%esi
-	call   27b0 <__cudaPushCallConfiguration@plt>
+	call   27d0 <__cudaPushCallConfiguration@plt>
 	test   %eax,%eax
-	je     4e18 <doubleGateAction+0x3d8>
-	call   2600 <cudaDeviceSynchronize@plt>
+	je     4e60 <doubleGateAction+0x3f0>
+	call   2610 <cudaDeviceSynchronize@plt>
 	mov    0x28(%rsp),%rsi
 	mov    (%rsp),%rdi
 	mov    %r15,%rdx
 	mov    $0x2,%ecx
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    0x20(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    %r12,%rdi
-	call   2480 <free@plt>
+	call   2490 <free@plt>
 	mov    0x98(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    4eb2 <doubleGateAction+0x472>
+	jne    4ef2 <doubleGateAction+0x482>
 	add    $0xa8,%rsp
 	mov    %rbp,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
-	jmp    2480 <free@plt>
+	jmp    2490 <free@plt>
 	nopl   0x0(%rax)
 	cmp    $0x1ac,%r13d
-	je     4e98 <doubleGateAction+0x458>
-	jbe    4de0 <doubleGateAction+0x3a0>
+	je     4ed8 <doubleGateAction+0x468>
+	jbe    4e28 <doubleGateAction+0x3b8>
 	cmp    $0x5f4,%r13d
-	jne    4cc8 <doubleGateAction+0x288>
+	jne    4d10 <doubleGateAction+0x2a0>
 	mov    %r12,%rdi
-	call   27a0 <syc_gate(float2*)@plt>
-	jmp    4cc8 <doubleGateAction+0x288>
+	call   27c0 <syc_gate(float2*)@plt>
+	jmp    4d10 <doubleGateAction+0x2a0>
 	nopl   0x0(%rax)
 	cmp    $0x601,%r13d
-	je     4e50 <doubleGateAction+0x410>
+	je     4e90 <doubleGateAction+0x420>
 	cmp    $0x605,%r13d
-	jne    4cc8 <doubleGateAction+0x288>
+	jne    4d10 <doubleGateAction+0x2a0>
 	movss  0x14(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   2530 <rzz_gate(float2*, float)@plt>
-	jmp    4cc8 <doubleGateAction+0x288>
+	call   2540 <rzz_gate(float2*, float)@plt>
+	jmp    4d10 <doubleGateAction+0x2a0>
 	nopl   (%rax)
 	cmp    $0x1a2,%r13d
-	je     4e68 <doubleGateAction+0x428>
+	je     4ea8 <doubleGateAction+0x438>
 	cmp    $0x1aa,%r13d
-	jne    4cc8 <doubleGateAction+0x288>
+	jne    4d10 <doubleGateAction+0x2a0>
 	mov    0x1c(%rsp),%ecx
 	mov    %r12,%rdi
 	cmp    %ecx,0x18(%rsp)
-	jle    4ea8 <doubleGateAction+0x468>
-	call   2660 <cnot_gate_control_big(float2*)@plt>
-	jmp    4cc8 <doubleGateAction+0x288>
+	jle    4ee8 <doubleGateAction+0x478>
+	call   2670 <cnot_gate_control_big(float2*)@plt>
+	jmp    4d10 <doubleGateAction+0x2a0>
 	nopl   0x0(%rax)
 	mov    0x30(%rsp),%rcx
 	mov    0x8(%rsp),%rdx
 	mov    0x20(%rsp),%rsi
 	mov    0x28(%rsp),%rdi
-	call   2410 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
-	jmp    4d08 <doubleGateAction+0x2c8>
-	cs nopw 0x0(%rax,%rax,1)
+	call   2420 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    4d50 <doubleGateAction+0x2e0>
+	xchg   %ax,%ax
 	mov    %r12,%rdi
-	call   2690 <swap_gate(float2*)@plt>
-	jmp    4cc8 <doubleGateAction+0x288>
+	call   26a0 <swap_gate(float2*)@plt>
+	jmp    4d10 <doubleGateAction+0x2a0>
 	nopl   (%rax)
 	movss  0x14(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   2510 <ryy_gate(float2*, float)@plt>
-	jmp    4cc8 <doubleGateAction+0x288>
+	call   2520 <ryy_gate(float2*, float)@plt>
+	jmp    4d10 <doubleGateAction+0x2a0>
 	nopl   0x0(%rax,%rax,1)
 	movss  0x14(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   27d0 <cphase_gate(float2*, float)@plt>
-	jmp    4cc8 <doubleGateAction+0x288>
+	call   27f0 <cphase_gate(float2*, float)@plt>
+	jmp    4d10 <doubleGateAction+0x2a0>
 	nopl   0x0(%rax,%rax,1)
 	movss  0x14(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   2450 <rxx_gate(float2*, float)@plt>
-	jmp    4cc8 <doubleGateAction+0x288>
+	call   2460 <rxx_gate(float2*, float)@plt>
+	jmp    4d10 <doubleGateAction+0x2a0>
 	nopl   0x0(%rax,%rax,1)
 	mov    %r12,%rdi
-	call   2750 <cz_gate(float2*)@plt>
-	jmp    4cc8 <doubleGateAction+0x288>
+	call   2770 <cz_gate(float2*)@plt>
+	jmp    4d10 <doubleGateAction+0x2a0>
 	nopl   (%rax)
-	call   2500 <cnot_gate_control_small(float2*)@plt>
-	jmp    4cc8 <doubleGateAction+0x288>
-	call   2540 <__stack_chk_fail@plt>
-	lea    0x11e2(%rip),%rdi        
-	call   24e0 <puts@plt>
+	call   2510 <cnot_gate_control_small(float2*)@plt>
+	jmp    4d10 <doubleGateAction+0x2a0>
+	call   2550 <__stack_chk_fail@plt>
+	mov    $0x1,%edi
+	mov    %r14,%rdx
+	lea    0x11ba(%rip),%rsi        
+	xor    %eax,%eax
+	call   2710 <__printf_chk@plt>
 	mov    $0x1,%edi
-	call   2780 <exit@plt>
+	call   27a0 <exit@plt>
 	mov    0x20(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    %r12,%rdi
-	call   2480 <free@plt>
+	call   2490 <free@plt>
 	mov    %rbp,%rdi
-	call   2480 <free@plt>
+	call   2490 <free@plt>
 	mov    $0x3,%edi
-	call   2780 <exit@plt>
-	lea    0x11bc(%rip),%rdi        
-	call   24e0 <puts@plt>
+	call   27a0 <exit@plt>
+	lea    0x11a2(%rip),%rdi        
+	call   24f0 <puts@plt>
 	mov    $0x2,%edi
-	call   2780 <exit@plt>
-	nopl   0x0(%rax,%rax,1)
+	call   27a0 <exit@plt>
+	data16 cs nopw 0x0(%rax,%rax,1)
 
-0000000000004f20 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000004f70 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
 __device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*):
 	endbr64
 	sub    $0xa8,%rsp
 	mov    %rdi,0x18(%rsp)
 	lea    0x38(%rsp),%rdi
 	mov    %rsi,0x10(%rsp)
 	lea    0x48(%rsp),%rsi
@@ -2321,134 +2334,134 @@
 	movq   %rax,%xmm1
 	lea    0x8(%rsp),%rax
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x70(%rsp)
 	movq   %rax,%xmm0
 	mov    %rsp,%rax
 	movq   %rax,%xmm2
-	mov    0x134d(%rip),%rax        
+	mov    0x132d(%rip),%rax        
 	punpcklqdq %xmm2,%xmm0
 	mov    %rax,0x38(%rsp)
 	mov    %rax,0x48(%rsp)
 	movaps %xmm0,0x80(%rsp)
-	call   2810 <__cudaPopCallConfiguration@plt>
+	call   2830 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
-	jne    4ffb <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xdb>
+	jne    504b <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xdb>
 	push   0x30(%rsp)
-	mov    0x9003(%rip),%rdi        
+	mov    0x8fb3(%rip),%rdi        
 	push   0x30(%rsp)
 	mov    0x58(%rsp),%rcx
 	mov    0x60(%rsp),%r8d
 	mov    0x48(%rsp),%rsi
 	mov    0x50(%rsp),%edx
 	lea    0x80(%rsp),%r9
-	call   26f0 <cudaLaunchKernel@plt>
+	call   2700 <cudaLaunchKernel@plt>
 	pop    %rax
 	pop    %rdx
 	mov    0x98(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    5016 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xf6>
+	jne    5066 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xf6>
 	add    $0xa8,%rsp
 	ret
-	call   2540 <__stack_chk_fail@plt>
+	call   2550 <__stack_chk_fail@plt>
 	nopl   0x0(%rax,%rax,1)
 
-0000000000005020 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000005070 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)>:
 actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*):
 	endbr64
-	jmp    27f0 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    2810 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
 	nopl   0x0(%rax)
 
-0000000000005030 <tripleGateAction>:
+0000000000005080 <tripleGateAction>:
 tripleGateAction():
 	endbr64
 	push   %r15
 	push   %r14
 	mov    %rsi,%r14
-	lea    0x1008(%rip),%rsi        
+	lea    0xfae(%rip),%rsi        
 	push   %r13
 	movq   %rsi,%xmm0
 	mov    %edx,%r13d
 	push   %r12
 	push   %rbp
 	mov    %r8d,%ebp
 	push   %rbx
 	mov    %rcx,%rbx
 	sub    $0x78,%rsp
 	mov    %rdi,0x8(%rsp)
 	mov    %rcx,%rdi
 	mov    %fs:0x28,%rax
 	mov    %rax,0x68(%rsp)
-	lea    0xfcd(%rip),%rax        
+	lea    0xf7d(%rip),%rax        
 	movq   %rax,%xmm1
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x50(%rsp)
-	call   26e0 <getArrayLength(int*)@plt>
+	call   26f0 <getArrayLength(int*)@plt>
 	cmp    $0x3,%eax
-	jne    5470 <tripleGateAction+0x440>
+	jne    54c0 <tripleGateAction+0x440>
 	mov    (%rbx),%ecx
 	mov    0x4(%rbx),%eax
 	cmp    %eax,%ecx
-	je     541d <tripleGateAction+0x3ed>
+	je     546d <tripleGateAction+0x3ed>
 	mov    0x8(%rbx),%edx
 	cmp    %edx,%eax
-	je     541d <tripleGateAction+0x3ed>
+	je     546d <tripleGateAction+0x3ed>
 	cmp    %edx,%ecx
-	je     541d <tripleGateAction+0x3ed>
+	je     546d <tripleGateAction+0x3ed>
 	mov    %ebp,%edi
-	call   2740 <cudaSetDevice@plt>
+	call   2760 <cudaSetDevice@plt>
 	mov    $0x200,%edi
-	call   26a0 <malloc@plt>
+	call   26b0 <malloc@plt>
 	mov    $0x18,%edi
 	mov    %rax,%r12
-	call   26a0 <malloc@plt>
+	call   26b0 <malloc@plt>
 	mov    $0x1,%r8d
 	mov    %r13d,%ecx
 	lea    0x20(%rsp),%rdi
 	mov    %rax,%rbp
 	mov    %r8d,%eax
 	mov    $0x200,%esi
 	movq   $0x0,0x20(%rsp)
 	movq   $0x0,0x28(%rsp)
 	shl    %cl,%eax
 	movq   $0x0,0x30(%rsp)
 	movslq %eax,%r13
-	call   26d0 <cudaMalloc@plt>
+	call   26e0 <cudaMalloc@plt>
 	lea    0x0(,%r13,8),%r15
 	lea    0x28(%rsp),%rdi
 	mov    %r15,%rsi
-	call   26d0 <cudaMalloc@plt>
+	call   26e0 <cudaMalloc@plt>
 	lea    0x30(%rsp),%rdi
 	mov    $0x18,%esi
-	call   26d0 <cudaMalloc@plt>
+	call   26e0 <cudaMalloc@plt>
 	mov    0x28(%rsp),%rdi
 	mov    %r15,%rdx
 	mov    %r14,%rsi
 	mov    $0x1,%ecx
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    0x8(%rsp),%rdi
-	call   2790 <hash(char const*)@plt>
+	call   27b0 <hash(char const*)@plt>
 	mov    (%rbx),%ecx
 	mov    $0x4,%edx
 	mov    %rbx,%rdi
 	mov    $0x3,%esi
 	mov    %eax,0x1c(%rsp)
 	mov    %ecx,0x10(%rsp)
 	mov    0x4(%rbx),%ecx
 	mov    %ecx,0x18(%rsp)
 	mov    0x8(%rbx),%ecx
 	mov    %ecx,0x14(%rsp)
-	mov    0x8e6a(%rip),%rcx        
-	call   24f0 <qsort@plt>
+	mov    0x8e1a(%rip),%rcx        
+	call   2500 <qsort@plt>
 	mov    0x8(%rsp),%rsi
 	lea    0x50(%rsp),%rdi
 	mov    $0x2,%edx
-	call   2520 <isInArray(char const**, char*, int)@plt>
+	call   2530 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     5433 <tripleGateAction+0x403>
+	je     5483 <tripleGateAction+0x403>
 	mov    (%rbx),%eax
 	mov    $0x1,%r8d
 	mov    0x30(%rsp),%rdi
 	movabs $0x100000001,%rsi
 	mov    %r8d,%edx
 	mov    %rsi,0x48(%rsp)
 	mov    %rbp,%rsi
@@ -2462,175 +2475,175 @@
 	mov    0x8(%rbx),%ecx
 	mov    %r8d,%ebx
 	movslq %edx,%rdx
 	mov    %rdx,0x8(%rbp)
 	mov    %r8d,%edx
 	shl    %cl,%edx
 	lea    0x1(%rax),%ecx
-	mov    0x1108(%rip),%rax        
+	mov    0x10e8(%rip),%rax        
 	movslq %edx,%rdx
 	shl    %cl,%ebx
 	mov    %rdx,0x10(%rbp)
 	movslq %ebx,%rdx
 	mov    %ebx,%ecx
 	mov    %rax,0x3c(%rsp)
 	mov    %r13,%rax
 	sub    %rdx,%rax
 	xor    %edx,%edx
 	div    %rcx
 	mov    $0x1,%ecx
 	mov    $0x18,%edx
 	add    $0x1,%eax
 	mov    %eax,0x44(%rsp)
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    0x1c(%rsp),%eax
 	cmp    $0x537,%eax
-	je     5360 <tripleGateAction+0x330>
+	je     53b0 <tripleGateAction+0x330>
 	cmp    $0x3229,%eax
-	je     52f0 <tripleGateAction+0x2c0>
+	je     5340 <tripleGateAction+0x2c0>
 	mov    0x20(%rsp),%rdi
 	mov    $0x1,%ecx
 	mov    $0x200,%edx
 	mov    %r12,%rsi
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    %ebx,0x38(%rsp)
 	mov    0x40(%rsp),%ecx
 	xor    %r9d,%r9d
 	mov    0x38(%rsp),%rdx
 	mov    0x44(%rsp),%rdi
 	xor    %r8d,%r8d
 	mov    0x4c(%rsp),%esi
-	call   27b0 <__cudaPushCallConfiguration@plt>
+	call   27d0 <__cudaPushCallConfiguration@plt>
 	test   %eax,%eax
-	je     53c0 <tripleGateAction+0x390>
-	call   2600 <cudaDeviceSynchronize@plt>
+	je     5410 <tripleGateAction+0x390>
+	call   2610 <cudaDeviceSynchronize@plt>
 	mov    0x28(%rsp),%rsi
 	mov    %r15,%rdx
 	mov    %r14,%rdi
 	mov    $0x2,%ecx
-	call   25a0 <cudaMemcpy@plt>
+	call   25b0 <cudaMemcpy@plt>
 	mov    0x20(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    %r12,%rdi
-	call   2480 <free@plt>
+	call   2490 <free@plt>
 	mov    0x68(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    546b <tripleGateAction+0x43b>
+	jne    54bb <tripleGateAction+0x43b>
 	add    $0x78,%rsp
 	mov    %rbp,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
-	jmp    2480 <free@plt>
+	jmp    2490 <free@plt>
 	nopl   0x0(%rax,%rax,1)
 	mov    0x18(%rsp),%esi
 	mov    0x14(%rsp),%eax
 	cmp    %eax,%esi
 	cmovle %esi,%eax
 	cmp    0x10(%rsp),%eax
-	jg     5410 <tripleGateAction+0x3e0>
+	jg     5460 <tripleGateAction+0x3e0>
 	mov    0x14(%rsp),%eax
 	cmp    %eax,%esi
 	cmovge %esi,%eax
 	cmp    0x10(%rsp),%eax
-	jl     53f0 <tripleGateAction+0x3c0>
+	jl     5440 <tripleGateAction+0x3c0>
 	mov    0x10(%rsp),%eax
 	mov    0x14(%rsp),%esi
 	cmp    %esi,%eax
-	jge    532e <tripleGateAction+0x2fe>
+	jge    537e <tripleGateAction+0x2fe>
 	mov    0x18(%rsp),%esi
 	cmp    %esi,%eax
-	jg     534a <tripleGateAction+0x31a>
+	jg     539a <tripleGateAction+0x31a>
 	mov    0x10(%rsp),%eax
 	mov    0x18(%rsp),%esi
 	cmp    %esi,%eax
-	jge    523e <tripleGateAction+0x20e>
+	jge    528e <tripleGateAction+0x20e>
 	mov    0x14(%rsp),%esi
 	cmp    %esi,%eax
-	jle    523e <tripleGateAction+0x20e>
+	jle    528e <tripleGateAction+0x20e>
 	mov    %r12,%rdi
-	call   2770 <fred_gate_control_mid(float2*)@plt>
-	jmp    523e <tripleGateAction+0x20e>
+	call   2790 <fred_gate_control_mid(float2*)@plt>
+	jmp    528e <tripleGateAction+0x20e>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x10(%rsp),%esi
 	mov    0x18(%rsp),%eax
 	cmp    %eax,%esi
 	cmovge %esi,%eax
 	cmp    0x14(%rsp),%eax
-	jl     5400 <tripleGateAction+0x3d0>
+	jl     5450 <tripleGateAction+0x3d0>
 	mov    0x18(%rsp),%eax
 	cmp    %eax,%esi
 	cmovle %esi,%eax
 	cmp    0x14(%rsp),%eax
-	jg     53e0 <tripleGateAction+0x3b0>
+	jg     5430 <tripleGateAction+0x3b0>
 	mov    0x14(%rsp),%eax
 	cmp    %eax,0x10(%rsp)
-	jge    5396 <tripleGateAction+0x366>
+	jge    53e6 <tripleGateAction+0x366>
 	cmp    %eax,0x18(%rsp)
-	jg     53ae <tripleGateAction+0x37e>
+	jg     53fe <tripleGateAction+0x37e>
 	mov    0x14(%rsp),%eax
 	cmp    %eax,0x18(%rsp)
-	jge    523e <tripleGateAction+0x20e>
+	jge    528e <tripleGateAction+0x20e>
 	cmp    %eax,0x10(%rsp)
-	jle    523e <tripleGateAction+0x20e>
+	jle    528e <tripleGateAction+0x20e>
 	mov    %r12,%rdi
-	call   2710 <toff_gate_target_mid(float2*)@plt>
-	jmp    523e <tripleGateAction+0x20e>
+	call   2730 <toff_gate_target_mid(float2*)@plt>
+	jmp    528e <tripleGateAction+0x20e>
 	nopl   0x0(%rax,%rax,1)
 	mov    0x30(%rsp),%rcx
 	mov    0x20(%rsp),%rsi
 	mov    %r13,%rdx
 	mov    0x28(%rsp),%rdi
-	call   2420 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)@plt>
-	jmp    527e <tripleGateAction+0x24e>
+	call   2430 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    52ce <tripleGateAction+0x24e>
 	nopl   0x0(%rax)
 	mov    %r12,%rdi
-	call   25c0 <toff_gate_target_small(float2*)@plt>
-	jmp    523e <tripleGateAction+0x20e>
+	call   25d0 <toff_gate_target_small(float2*)@plt>
+	jmp    528e <tripleGateAction+0x20e>
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   25f0 <fred_gate_control_big(float2*)@plt>
-	jmp    523e <tripleGateAction+0x20e>
+	call   2600 <fred_gate_control_big(float2*)@plt>
+	jmp    528e <tripleGateAction+0x20e>
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   2610 <toff_gate_target_big(float2*)@plt>
-	jmp    523e <tripleGateAction+0x20e>
+	call   2620 <toff_gate_target_big(float2*)@plt>
+	jmp    528e <tripleGateAction+0x20e>
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   24a0 <fred_gate_control_small(float2*)@plt>
-	jmp    523e <tripleGateAction+0x20e>
-	lea    0xca4(%rip),%rdi        
-	call   24e0 <puts@plt>
+	call   24b0 <fred_gate_control_small(float2*)@plt>
+	jmp    528e <tripleGateAction+0x20e>
+	lea    0xc84(%rip),%rdi        
+	call   24f0 <puts@plt>
 	mov    $0x2,%edi
-	call   2780 <exit@plt>
+	call   27a0 <exit@plt>
 	mov    0x20(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
-	call   2580 <cudaFree@plt>
+	call   2590 <cudaFree@plt>
 	mov    %r12,%rdi
-	call   2480 <free@plt>
+	call   2490 <free@plt>
 	mov    %rbp,%rdi
-	call   2480 <free@plt>
+	call   2490 <free@plt>
 	mov    $0x3,%edi
-	call   2780 <exit@plt>
-	call   2540 <__stack_chk_fail@plt>
-	lea    0xc79(%rip),%rdi        
-	call   24e0 <puts@plt>
+	call   27a0 <exit@plt>
+	call   2550 <__stack_chk_fail@plt>
+	lea    0xc59(%rip),%rdi        
+	call   24f0 <puts@plt>
 	mov    $0x1,%edi
-	call   2780 <exit@plt>
+	call   27a0 <exit@plt>
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000005490 <atexit>:
+00000000000054e0 <atexit>:
 atexit():
 	endbr64
-	mov    0x8d6d(%rip),%rdx        
+	mov    0x8d25(%rip),%rdx        
 	xor    %esi,%esi
-	jmp    2760 <__cxa_atexit@plt>
+	jmp    2780 <__cxa_atexit@plt>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,11 +1,11 @@
 
 
 
 Disassembly of section .fini:
 
-00000000000054a4 <_fini>:
+00000000000054f4 <_fini>:
 _fini():
 	endbr64
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,51 +1,54 @@
 
 Hex dump of section '.rodata':
   0x00006000 73007364 67007400 74646700 68007278 s.sdg.t.tdg.h.rx
   0x00006010 00727900 727a0064 616d705f 49007064 .ry.rz.damp_I.pd
   0x00006020 00616400 69737761 70006370 00637a00 .ad.iswap.cp.cz.
   0x00006030 72787800 72797900 727a7a00 73796300 rxx.ryy.rzz.syc.
-  0x00006040 63787800 63737761 70006363 78000000 cxx.cswap.ccx...
-  0x00006050 10e8ffff 00e6ffff 00e6ffff 00e6ffff ................
-  0x00006060 00e6ffff 00e6ffff 00e6ffff 00e6ffff ................
-  0x00006070 00e6ffff 00e6ffff 00e6ffff 20e8ffff ............ ...
-  0x00006080 30e8ffff 00e6ffff 00e6ffff 00e6ffff 0...............
-  0x00006090 f0e7ffff 00e8ffff e0e7ffff 00000000 ................
-  0x000060a0 4d757374 20626520 68617665 2074776f Must be have two
-  0x000060b0 20616374 696f6e20 706f7369 74696f6e  action position
-  0x000060c0 21000000 00000000 61637469 6f6e2070 !.......action p
-  0x000060d0 6f736974 696f6e20 6d757374 20626520 osition must be 
-  0x000060e0 64696666 6572656e 74210000 00000000 different!......
-  0x000060f0 4d757374 20626520 68617665 20746872 Must be have thr
-  0x00006100 65652061 6374696f 6e20706f 73697469 ee action positi
-  0x00006110 6f6e2100 00000000 5f5a3138 61637469 on!....._Z18acti
-  0x00006120 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
-  0x00006130 666c6f61 74325330 5f6d506d 00000000 float2S0_mPm....
-  0x00006140 5f5a3139 61637469 6f6e4f6e 446f7562 _Z19actionOnDoub
-  0x00006150 6c655175 62697450 36666c6f 61743253 leQubitP6float2S
-  0x00006160 305f6d50 6d000000 5f5a3139 61637469 0_mPm..._Z19acti
-  0x00006170 6f6e4f6e 53696e67 6c655175 62697450 onOnSingleQubitP
-  0x00006180 36666c6f 61743253 305f6d50 6d000000 6float2S0_mPm...
-  0x00006190 00000000 00000000 0000803f 00000000 ...........?....
-  0x000061a0 0000803f 00000000 00000000 00000000 ...?............
-  0x000061b0 00000000 00000000 00000000 000080bf ................
-  0x000061c0 00000000 0000803f 00000000 00000000 .......?........
-  0x000061d0 00000000 00000000 000080bf 00000000 ................
-  0x000061e0 00000000 00000000 00000000 0000803f ...............?
-  0x000061f0 00000000 00000000 f304353f f304353f ..........5?..5?
-  0x00006200 00000000 00000000 f304353f f30435bf ..........5?..5.
-  0x00006210 f304353f 00000000 f304353f 00000000 ..5?......5?....
-  0x00006220 f304353f 00000000 f30435bf 00000000 ..5?......5.....
-  0x00006230 00000080 00000000 00000000 00000000 ................
-  0x00006240 00000000 000080bf 00000000 00000000 ................
-  0x00006250 00000000 00000000 d7b35d3f 000000bf ..........]?....
-  0x00006260 00000000 01000000 02000000 03000000 ................
-  0x00006270 04000000 04000000 04000000 04000000 ................
-  0x00006280 2d000000 2d000000 2d000000 2d000000 -...-...-...-...
-  0x00006290 3f000000 3f000000 3f000000 3f000000 ?...?...?...?...
-  0x000062a0 398ee338 398ee338 398ee338 398ee338 9..89..89..89..8
-  0x000062b0 0000803f 0000803f 0000803f 0000803f ...?...?...?...?
-  0x000062c0 1b000000 1b000000 1b000000 1b000000 ................
-  0x000062d0 36000000 36000000 36000000 36000000 6...6...6...6...
-  0x000062e0 0000003f 0000803f 00000030 00000000 ...?...?...0....
-  0x000062f0 8dedb5a0 f7c6b03e 01000000 01000000 .......>........
+  0x00006040 63637800 63737761 70006761 74654e61 ccx.cswap.gateNa
+  0x00006050 6d653a20 25730a00 706f735f 61727261 me: %s..pos_arra
+  0x00006060 795f7369 7a65203d 2025640a 00000000 y_size = %d.....
+  0x00006070 20e8ffff 10e6ffff 10e6ffff 10e6ffff  ...............
+  0x00006080 10e6ffff 10e6ffff 10e6ffff 10e6ffff ................
+  0x00006090 10e6ffff 10e6ffff 10e6ffff 30e8ffff ............0...
+  0x000060a0 40e8ffff 10e6ffff 10e6ffff 10e6ffff @...............
+  0x000060b0 00e8ffff 10e8ffff f0e7ffff 00000000 ................
+  0x000060c0 4d757374 20626520 68617665 2074776f Must be have two
+  0x000060d0 20616374 696f6e20 706f7369 74696f6e  action position
+  0x000060e0 212c2067 6174654e 616d653a 2025730a !, gateName: %s.
+  0x000060f0 00000000 00000000 61637469 6f6e2070 ........action p
+  0x00006100 6f736974 696f6e20 6d757374 20626520 osition must be 
+  0x00006110 64696666 6572656e 74210000 00000000 different!......
+  0x00006120 4d757374 20626520 68617665 20746872 Must be have thr
+  0x00006130 65652061 6374696f 6e20706f 73697469 ee action positi
+  0x00006140 6f6e2100 00000000 5f5a3138 61637469 on!....._Z18acti
+  0x00006150 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
+  0x00006160 666c6f61 74325330 5f6d506d 00000000 float2S0_mPm....
+  0x00006170 5f5a3139 61637469 6f6e4f6e 446f7562 _Z19actionOnDoub
+  0x00006180 6c655175 62697450 36666c6f 61743253 leQubitP6float2S
+  0x00006190 305f6d50 6d000000 5f5a3139 61637469 0_mPm..._Z19acti
+  0x000061a0 6f6e4f6e 53696e67 6c655175 62697450 onOnSingleQubitP
+  0x000061b0 36666c6f 61743253 305f6d50 6d000000 6float2S0_mPm...
+  0x000061c0 00000000 00000000 0000803f 00000000 ...........?....
+  0x000061d0 0000803f 00000000 00000000 00000000 ...?............
+  0x000061e0 00000000 00000000 00000000 000080bf ................
+  0x000061f0 00000000 0000803f 00000000 00000000 .......?........
+  0x00006200 00000000 00000000 000080bf 00000000 ................
+  0x00006210 00000000 00000000 00000000 0000803f ...............?
+  0x00006220 00000000 00000000 f304353f f304353f ..........5?..5?
+  0x00006230 00000000 00000000 f304353f f30435bf ..........5?..5.
+  0x00006240 f304353f 00000000 f304353f 00000000 ..5?......5?....
+  0x00006250 f304353f 00000000 f30435bf 00000000 ..5?......5.....
+  0x00006260 00000080 00000000 00000000 00000000 ................
+  0x00006270 00000000 000080bf 00000000 00000000 ................
+  0x00006280 00000000 00000000 d7b35d3f 000000bf ..........]?....
+  0x00006290 00000000 01000000 02000000 03000000 ................
+  0x000062a0 04000000 04000000 04000000 04000000 ................
+  0x000062b0 2d000000 2d000000 2d000000 2d000000 -...-...-...-...
+  0x000062c0 3f000000 3f000000 3f000000 3f000000 ?...?...?...?...
+  0x000062d0 398ee338 398ee338 398ee338 398ee338 9..89..89..89..8
+  0x000062e0 0000803f 0000803f 0000803f 0000803f ...?...?...?...?
+  0x000062f0 1b000000 1b000000 1b000000 1b000000 ................
+  0x00006300 36000000 36000000 36000000 36000000 6...6...6...6...
+  0x00006310 0000003f 0000803f 00000030 00000000 ...?...?...0....
+  0x00006320 8dedb5a0 f7c6b03e 01000000 01000000 .......>........
```

#### readelf --wide --decompress --hex-dump=.nv_fatbin {}

```diff
@@ -1,272 +1,269 @@
 
 Hex dump of section '.nv_fatbin':
-  0x00006300 50ed55ba 01001000 70040000 00000000 P.U.....p.......
-  0x00006310 02000101 40000000 30040000 00000000 ....@...0.......
-  0x00006320 00000000 00000000 07000100 50000000 ............P...
-  0x00006330 00000000 00000000 11000000 00000000 ................
-  0x00006340 00000000 00000000 00000000 00000000 ................
-  0x00006350 7f454c46 02010133 07000000 00000000 .ELF...3........
-  0x00006360 0200be00 76000000 00000000 00000000 ....v...........
-  0x00006370 c0030000 00000000 40020000 00000000 ........@.......
-  0x00006380 50055000 40003800 02004000 06000100 P.P.@.8...@.....
-  0x00006390 002e7368 73747274 6162002e 73747274 ..shstrtab..strt
-  0x000063a0 6162002e 73796d74 6162002e 73796d74 ab..symtab..symt
-  0x000063b0 61625f73 686e6478 002e6e76 2e696e66 ab_shndx..nv.inf
-  0x000063c0 6f002e6e 762e6361 6c6c6772 61706800 o..nv.callgraph.
-  0x000063d0 2e6e762e 70726f74 6f747970 65002e6e .nv.prototype..n
-  0x000063e0 762e7265 6c2e6163 74696f6e 00002e73 v.rel.action...s
-  0x000063f0 68737472 74616200 2e737472 74616200 hstrtab..strtab.
-  0x00006400 2e73796d 74616200 2e73796d 7461625f .symtab..symtab_
-  0x00006410 73686e64 78002e6e 762e696e 666f002e shndx..nv.info..
-  0x00006420 6e762e63 616c6c67 72617068 002e6e76 nv.callgraph..nv
-  0x00006430 2e70726f 746f7479 7065002e 6e762e72 .prototype..nv.r
-  0x00006440 656c2e61 6374696f 6e000000 00000000 el.action.......
-  0x00006450 00000000 00000000 00000000 00000000 ................
-  0x00006460 00000000 00000000 32000000 03000400 ........2.......
-  0x00006470 00000000 00000000 00000000 00000000 ................
-  0x00006480 4e000000 03000500 00000000 00000000 N...............
-  0x00006490 00000000 00000000 00000000 ffffffff ................
-  0x000064a0 00000000 feffffff 00000000 fdffffff ................
-  0x000064b0 4b000000 00000000 00020208 100a2f22 K............./"
-  0x000064c0 00000008 00000000 00000808 00000000 ................
-  0x000064d0 00001008 00000000 00001808 00000000 ................
-  0x000064e0 00002008 00000000 00002808 00000000 .. .......(.....
-  0x000064f0 00003008 00000000 00003808 00000000 ..0.......8.....
-  0x00006500 01000008 00000000 01000808 00000000 ................
-  0x00006510 01001008 00000000 01001808 00000000 ................
-  0x00006520 01002008 00000000 01002808 00000000 .. .......(.....
-  0x00006530 01003008 00000000 01003808 00000000 ..0.......8.....
-  0x00006540 02000008 00000000 02000808 00000000 ................
-  0x00006550 02001008 00000000 02001808 00000000 ................
-  0x00006560 02002008 00000000 02002808 00000000 .. .......(.....
-  0x00006570 02003008 00000000 02003808 00000000 ..0.......8.....
-  0x00006580 00000014 2c000000 0300000c 00000000 ....,...........
-  0x00006590 00000000 00000000 00000000 00000000 ................
-  0x000065a0 00000000 00000000 00000000 00000000 ................
-  0x000065b0 00000000 00000000 00000000 00000000 ................
+  0x00006330 50ed55ba 01001000 70040000 00000000 P.U.....p.......
+  0x00006340 02000101 40000000 30040000 00000000 ....@...0.......
+  0x00006350 00000000 00000000 07000100 50000000 ............P...
+  0x00006360 00000000 00000000 11000000 00000000 ................
+  0x00006370 00000000 00000000 00000000 00000000 ................
+  0x00006380 7f454c46 02010133 07000000 00000000 .ELF...3........
+  0x00006390 0200be00 76000000 00000000 00000000 ....v...........
+  0x000063a0 c0030000 00000000 40020000 00000000 ........@.......
+  0x000063b0 50055000 40003800 02004000 06000100 P.P.@.8...@.....
+  0x000063c0 002e7368 73747274 6162002e 73747274 ..shstrtab..strt
+  0x000063d0 6162002e 73796d74 6162002e 73796d74 ab..symtab..symt
+  0x000063e0 61625f73 686e6478 002e6e76 2e696e66 ab_shndx..nv.inf
+  0x000063f0 6f002e6e 762e6361 6c6c6772 61706800 o..nv.callgraph.
+  0x00006400 2e6e762e 70726f74 6f747970 65002e6e .nv.prototype..n
+  0x00006410 762e7265 6c2e6163 74696f6e 00002e73 v.rel.action...s
+  0x00006420 68737472 74616200 2e737472 74616200 hstrtab..strtab.
+  0x00006430 2e73796d 74616200 2e73796d 7461625f .symtab..symtab_
+  0x00006440 73686e64 78002e6e 762e696e 666f002e shndx..nv.info..
+  0x00006450 6e762e63 616c6c67 72617068 002e6e76 nv.callgraph..nv
+  0x00006460 2e70726f 746f7479 7065002e 6e762e72 .prototype..nv.r
+  0x00006470 656c2e61 6374696f 6e000000 00000000 el.action.......
+  0x00006480 00000000 00000000 00000000 00000000 ................
+  0x00006490 00000000 00000000 32000000 03000400 ........2.......
+  0x000064a0 00000000 00000000 00000000 00000000 ................
+  0x000064b0 4e000000 03000500 00000000 00000000 N...............
+  0x000064c0 00000000 00000000 00000000 ffffffff ................
+  0x000064d0 00000000 feffffff 00000000 fdffffff ................
+  0x000064e0 4b000000 00000000 00020208 100a2f22 K............./"
+  0x000064f0 00000008 00000000 00000808 00000000 ................
+  0x00006500 00001008 00000000 00001808 00000000 ................
+  0x00006510 00002008 00000000 00002808 00000000 .. .......(.....
+  0x00006520 00003008 00000000 00003808 00000000 ..0.......8.....
+  0x00006530 01000008 00000000 01000808 00000000 ................
+  0x00006540 01001008 00000000 01001808 00000000 ................
+  0x00006550 01002008 00000000 01002808 00000000 .. .......(.....
+  0x00006560 01003008 00000000 01003808 00000000 ..0.......8.....
+  0x00006570 02000008 00000000 02000808 00000000 ................
+  0x00006580 02001008 00000000 02001808 00000000 ................
+  0x00006590 02002008 00000000 02002808 00000000 .. .......(.....
+  0x000065a0 02003008 00000000 02003808 00000000 ..0.......8.....
+  0x000065b0 00000014 2c000000 0300000c 00000000 ....,...........
   0x000065c0 00000000 00000000 00000000 00000000 ................
-  0x000065d0 01000000 03000000 00000000 00000000 ................
-  0x000065e0 00000000 00000000 40000000 00000000 ........@.......
-  0x000065f0 5d000000 00000000 00000000 00000000 ]...............
-  0x00006600 01000000 00000000 00000000 00000000 ................
-  0x00006610 0b000000 03000000 00000000 00000000 ................
-  0x00006620 00000000 00000000 9d000000 00000000 ................
-  0x00006630 5d000000 00000000 00000000 00000000 ]...............
-  0x00006640 01000000 00000000 00000000 00000000 ................
-  0x00006650 13000000 02000000 00000000 00000000 ................
-  0x00006660 00000000 00000000 00010000 00000000 ................
-  0x00006670 48000000 00000000 02000000 03000000 H...............
-  0x00006680 08000000 00000000 18000000 00000000 ................
-  0x00006690 32000000 01000070 00000000 00000000 2......p........
-  0x000066a0 00000000 00000000 48010000 00000000 ........H.......
-  0x000066b0 18000000 00000000 03000000 00000000 ................
-  0x000066c0 04000000 00000000 08000000 00000000 ................
-  0x000066d0 4e000000 0b000070 00000000 00000000 N......p........
-  0x000066e0 00000000 00000000 60010000 00000000 ........`.......
-  0x000066f0 e0000000 00000000 00000000 00000000 ................
-  0x00006700 08000000 00000000 08000000 00000000 ................
-  0x00006710 06000000 05000000 c0030000 00000000 ................
-  0x00006720 00000000 00000000 00000000 00000000 ................
-  0x00006730 70000000 00000000 70000000 00000000 p.......p.......
-  0x00006740 08000000 00000000 01000000 05000000 ................
-  0x00006750 c0030000 00000000 00000000 00000000 ................
-  0x00006760 00000000 00000000 70000000 00000000 ........p.......
-  0x00006770 70000000 00000000 08000000 00000000 p...............
-  0x00006780 50ed55ba 01001000 305b0000 00000000 P.U.....0[......
-  0x00006790 02000101 40000000 683b0000 00000000 ....@...h;......
-  0x000067a0 00000000 00000000 07000100 50000000 ............P...
-  0x000067b0 00000000 00000000 11000000 00000000 ................
-  0x000067c0 00000000 00000000 00000000 00000000 ................
-  0x000067d0 7f454c46 02010133 07000000 00000000 .ELF...3........
-  0x000067e0 0200be00 76000000 00000000 00000000 ....v...........
-  0x000067f0 c03a0000 00000000 80360000 00000000 .:.......6......
-  0x00006800 50055000 40003800 03004000 11000100 P.P.@.8...@.....
-  0x00006810 002e7368 73747274 6162002e 73747274 ..shstrtab..strt
-  0x00006820 6162002e 73796d74 6162002e 73796d74 ab..symtab..symt
-  0x00006830 61625f73 686e6478 002e6e76 2e696e66 ab_shndx..nv.inf
-  0x00006840 6f002e74 6578742e 5f5a3138 61637469 o..text._Z18acti
-  0x00006850 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
-  0x00006860 666c6f61 74325330 5f6d506d 002e6e76 float2S0_mPm..nv
-  0x00006870 2e696e66 6f2e5f5a 31386163 74696f6e .info._Z18action
-  0x00006880 4f6e5472 69706c65 47617465 5036666c OnTripleGateP6fl
-  0x00006890 6f617432 53305f6d 506d002e 6e762e73 oat2S0_mPm..nv.s
-  0x000068a0 68617265 642e5f5a 31386163 74696f6e hared._Z18action
+  0x000065d0 00000000 00000000 00000000 00000000 ................
+  0x000065e0 00000000 00000000 00000000 00000000 ................
+  0x000065f0 00000000 00000000 00000000 00000000 ................
+  0x00006600 01000000 03000000 00000000 00000000 ................
+  0x00006610 00000000 00000000 40000000 00000000 ........@.......
+  0x00006620 5d000000 00000000 00000000 00000000 ]...............
+  0x00006630 01000000 00000000 00000000 00000000 ................
+  0x00006640 0b000000 03000000 00000000 00000000 ................
+  0x00006650 00000000 00000000 9d000000 00000000 ................
+  0x00006660 5d000000 00000000 00000000 00000000 ]...............
+  0x00006670 01000000 00000000 00000000 00000000 ................
+  0x00006680 13000000 02000000 00000000 00000000 ................
+  0x00006690 00000000 00000000 00010000 00000000 ................
+  0x000066a0 48000000 00000000 02000000 03000000 H...............
+  0x000066b0 08000000 00000000 18000000 00000000 ................
+  0x000066c0 32000000 01000070 00000000 00000000 2......p........
+  0x000066d0 00000000 00000000 48010000 00000000 ........H.......
+  0x000066e0 18000000 00000000 03000000 00000000 ................
+  0x000066f0 04000000 00000000 08000000 00000000 ................
+  0x00006700 4e000000 0b000070 00000000 00000000 N......p........
+  0x00006710 00000000 00000000 60010000 00000000 ........`.......
+  0x00006720 e0000000 00000000 00000000 00000000 ................
+  0x00006730 08000000 00000000 08000000 00000000 ................
+  0x00006740 06000000 05000000 c0030000 00000000 ................
+  0x00006750 00000000 00000000 00000000 00000000 ................
+  0x00006760 70000000 00000000 70000000 00000000 p.......p.......
+  0x00006770 08000000 00000000 01000000 05000000 ................
+  0x00006780 c0030000 00000000 00000000 00000000 ................
+  0x00006790 00000000 00000000 70000000 00000000 ........p.......
+  0x000067a0 70000000 00000000 08000000 00000000 p...............
+  0x000067b0 50ed55ba 01001000 305b0000 00000000 P.U.....0[......
+  0x000067c0 02000101 40000000 683b0000 00000000 ....@...h;......
+  0x000067d0 00000000 00000000 07000100 50000000 ............P...
+  0x000067e0 00000000 00000000 11000000 00000000 ................
+  0x000067f0 00000000 00000000 00000000 00000000 ................
+  0x00006800 7f454c46 02010133 07000000 00000000 .ELF...3........
+  0x00006810 0200be00 76000000 00000000 00000000 ....v...........
+  0x00006820 c03a0000 00000000 80360000 00000000 .:.......6......
+  0x00006830 50055000 40003800 03004000 11000100 P.P.@.8...@.....
+  0x00006840 002e7368 73747274 6162002e 73747274 ..shstrtab..strt
+  0x00006850 6162002e 73796d74 6162002e 73796d74 ab..symtab..symt
+  0x00006860 61625f73 686e6478 002e6e76 2e696e66 ab_shndx..nv.inf
+  0x00006870 6f002e74 6578742e 5f5a3138 61637469 o..text._Z18acti
+  0x00006880 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
+  0x00006890 666c6f61 74325330 5f6d506d 002e6e76 float2S0_mPm..nv
+  0x000068a0 2e696e66 6f2e5f5a 31386163 74696f6e .info._Z18action
   0x000068b0 4f6e5472 69706c65 47617465 5036666c OnTripleGateP6fl
-  0x000068c0 6f617432 53305f6d 506d002e 6e762e63 oat2S0_mPm..nv.c
-  0x000068d0 6f6e7374 616e7430 2e5f5a31 38616374 onstant0._Z18act
-  0x000068e0 696f6e4f 6e547269 706c6547 61746550 ionOnTripleGateP
-  0x000068f0 36666c6f 61743253 305f6d50 6d002e74 6float2S0_mPm..t
-  0x00006900 6578742e 5f5a3139 61637469 6f6e4f6e ext._Z19actionOn
-  0x00006910 446f7562 6c655175 62697450 36666c6f DoubleQubitP6flo
-  0x00006920 61743253 305f6d50 6d002e6e 762e696e at2S0_mPm..nv.in
-  0x00006930 666f2e5f 5a313961 6374696f 6e4f6e44 fo._Z19actionOnD
-  0x00006940 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x00006950 74325330 5f6d506d 002e6e76 2e736861 t2S0_mPm..nv.sha
-  0x00006960 7265642e 5f5a3139 61637469 6f6e4f6e red._Z19actionOn
-  0x00006970 446f7562 6c655175 62697450 36666c6f DoubleQubitP6flo
-  0x00006980 61743253 305f6d50 6d002e6e 762e636f at2S0_mPm..nv.co
-  0x00006990 6e737461 6e74302e 5f5a3139 61637469 nstant0._Z19acti
-  0x000069a0 6f6e4f6e 446f7562 6c655175 62697450 onOnDoubleQubitP
-  0x000069b0 36666c6f 61743253 305f6d50 6d002e74 6float2S0_mPm..t
-  0x000069c0 6578742e 5f5a3139 61637469 6f6e4f6e ext._Z19actionOn
-  0x000069d0 53696e67 6c655175 62697450 36666c6f SingleQubitP6flo
-  0x000069e0 61743253 305f6d50 6d002e6e 762e696e at2S0_mPm..nv.in
-  0x000069f0 666f2e5f 5a313961 6374696f 6e4f6e53 fo._Z19actionOnS
-  0x00006a00 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
-  0x00006a10 74325330 5f6d506d 002e6e76 2e736861 t2S0_mPm..nv.sha
-  0x00006a20 7265642e 5f5a3139 61637469 6f6e4f6e red._Z19actionOn
-  0x00006a30 53696e67 6c655175 62697450 36666c6f SingleQubitP6flo
-  0x00006a40 61743253 305f6d50 6d002e6e 762e636f at2S0_mPm..nv.co
-  0x00006a50 6e737461 6e74302e 5f5a3139 61637469 nstant0._Z19acti
-  0x00006a60 6f6e4f6e 53696e67 6c655175 62697450 onOnSingleQubitP
-  0x00006a70 36666c6f 61743253 305f6d50 6d002e64 6float2S0_mPm..d
-  0x00006a80 65627567 5f667261 6d65002e 72656c2e ebug_frame..rel.
-  0x00006a90 64656275 675f6672 616d6500 2e72656c debug_frame..rel
-  0x00006aa0 612e6465 6275675f 6672616d 65002e6e a.debug_frame..n
-  0x00006ab0 762e7265 6c2e6163 74696f6e 00002e73 v.rel.action...s
-  0x00006ac0 68737472 74616200 2e737472 74616200 hstrtab..strtab.
-  0x00006ad0 2e73796d 74616200 2e73796d 7461625f .symtab..symtab_
-  0x00006ae0 73686e64 78002e6e 762e696e 666f005f shndx..nv.info._
-  0x00006af0 5a313861 6374696f 6e4f6e54 7269706c Z18actionOnTripl
-  0x00006b00 65476174 65503666 6c6f6174 3253305f eGateP6float2S0_
-  0x00006b10 6d506d00 2e746578 742e5f5a 31386163 mPm..text._Z18ac
-  0x00006b20 74696f6e 4f6e5472 69706c65 47617465 tionOnTripleGate
-  0x00006b30 5036666c 6f617432 53305f6d 506d002e P6float2S0_mPm..
-  0x00006b40 6e762e69 6e666f2e 5f5a3138 61637469 nv.info._Z18acti
-  0x00006b50 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
-  0x00006b60 666c6f61 74325330 5f6d506d 002e6e76 float2S0_mPm..nv
-  0x00006b70 2e736861 7265642e 5f5a3138 61637469 .shared._Z18acti
+  0x000068c0 6f617432 53305f6d 506d002e 6e762e73 oat2S0_mPm..nv.s
+  0x000068d0 68617265 642e5f5a 31386163 74696f6e hared._Z18action
+  0x000068e0 4f6e5472 69706c65 47617465 5036666c OnTripleGateP6fl
+  0x000068f0 6f617432 53305f6d 506d002e 6e762e63 oat2S0_mPm..nv.c
+  0x00006900 6f6e7374 616e7430 2e5f5a31 38616374 onstant0._Z18act
+  0x00006910 696f6e4f 6e547269 706c6547 61746550 ionOnTripleGateP
+  0x00006920 36666c6f 61743253 305f6d50 6d002e74 6float2S0_mPm..t
+  0x00006930 6578742e 5f5a3139 61637469 6f6e4f6e ext._Z19actionOn
+  0x00006940 446f7562 6c655175 62697450 36666c6f DoubleQubitP6flo
+  0x00006950 61743253 305f6d50 6d002e6e 762e696e at2S0_mPm..nv.in
+  0x00006960 666f2e5f 5a313961 6374696f 6e4f6e44 fo._Z19actionOnD
+  0x00006970 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
+  0x00006980 74325330 5f6d506d 002e6e76 2e736861 t2S0_mPm..nv.sha
+  0x00006990 7265642e 5f5a3139 61637469 6f6e4f6e red._Z19actionOn
+  0x000069a0 446f7562 6c655175 62697450 36666c6f DoubleQubitP6flo
+  0x000069b0 61743253 305f6d50 6d002e6e 762e636f at2S0_mPm..nv.co
+  0x000069c0 6e737461 6e74302e 5f5a3139 61637469 nstant0._Z19acti
+  0x000069d0 6f6e4f6e 446f7562 6c655175 62697450 onOnDoubleQubitP
+  0x000069e0 36666c6f 61743253 305f6d50 6d002e74 6float2S0_mPm..t
+  0x000069f0 6578742e 5f5a3139 61637469 6f6e4f6e ext._Z19actionOn
+  0x00006a00 53696e67 6c655175 62697450 36666c6f SingleQubitP6flo
+  0x00006a10 61743253 305f6d50 6d002e6e 762e696e at2S0_mPm..nv.in
+  0x00006a20 666f2e5f 5a313961 6374696f 6e4f6e53 fo._Z19actionOnS
+  0x00006a30 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
+  0x00006a40 74325330 5f6d506d 002e6e76 2e736861 t2S0_mPm..nv.sha
+  0x00006a50 7265642e 5f5a3139 61637469 6f6e4f6e red._Z19actionOn
+  0x00006a60 53696e67 6c655175 62697450 36666c6f SingleQubitP6flo
+  0x00006a70 61743253 305f6d50 6d002e6e 762e636f at2S0_mPm..nv.co
+  0x00006a80 6e737461 6e74302e 5f5a3139 61637469 nstant0._Z19acti
+  0x00006a90 6f6e4f6e 53696e67 6c655175 62697450 onOnSingleQubitP
+  0x00006aa0 36666c6f 61743253 305f6d50 6d002e64 6float2S0_mPm..d
+  0x00006ab0 65627567 5f667261 6d65002e 72656c2e ebug_frame..rel.
+  0x00006ac0 64656275 675f6672 616d6500 2e72656c debug_frame..rel
+  0x00006ad0 612e6465 6275675f 6672616d 65002e6e a.debug_frame..n
+  0x00006ae0 762e7265 6c2e6163 74696f6e 00002e73 v.rel.action...s
+  0x00006af0 68737472 74616200 2e737472 74616200 hstrtab..strtab.
+  0x00006b00 2e73796d 74616200 2e73796d 7461625f .symtab..symtab_
+  0x00006b10 73686e64 78002e6e 762e696e 666f005f shndx..nv.info._
+  0x00006b20 5a313861 6374696f 6e4f6e54 7269706c Z18actionOnTripl
+  0x00006b30 65476174 65503666 6c6f6174 3253305f eGateP6float2S0_
+  0x00006b40 6d506d00 2e746578 742e5f5a 31386163 mPm..text._Z18ac
+  0x00006b50 74696f6e 4f6e5472 69706c65 47617465 tionOnTripleGate
+  0x00006b60 5036666c 6f617432 53305f6d 506d002e P6float2S0_mPm..
+  0x00006b70 6e762e69 6e666f2e 5f5a3138 61637469 nv.info._Z18acti
   0x00006b80 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
   0x00006b90 666c6f61 74325330 5f6d506d 002e6e76 float2S0_mPm..nv
-  0x00006ba0 2e636f6e 7374616e 74302e5f 5a313861 .constant0._Z18a
-  0x00006bb0 6374696f 6e4f6e54 7269706c 65476174 ctionOnTripleGat
-  0x00006bc0 65503666 6c6f6174 3253305f 6d506d00 eP6float2S0_mPm.
-  0x00006bd0 5f706172 616d005f 5a313961 6374696f _param._Z19actio
-  0x00006be0 6e4f6e44 6f75626c 65517562 69745036 nOnDoubleQubitP6
-  0x00006bf0 666c6f61 74325330 5f6d506d 002e7465 float2S0_mPm..te
-  0x00006c00 78742e5f 5a313961 6374696f 6e4f6e44 xt._Z19actionOnD
-  0x00006c10 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x00006c20 74325330 5f6d506d 002e6e76 2e696e66 t2S0_mPm..nv.inf
-  0x00006c30 6f2e5f5a 31396163 74696f6e 4f6e446f o._Z19actionOnDo
-  0x00006c40 75626c65 51756269 74503666 6c6f6174 ubleQubitP6float
-  0x00006c50 3253305f 6d506d00 2e6e762e 73686172 2S0_mPm..nv.shar
-  0x00006c60 65642e5f 5a313961 6374696f 6e4f6e44 ed._Z19actionOnD
-  0x00006c70 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x00006c80 74325330 5f6d506d 002e6e76 2e636f6e t2S0_mPm..nv.con
-  0x00006c90 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
-  0x00006ca0 6e4f6e44 6f75626c 65517562 69745036 nOnDoubleQubitP6
-  0x00006cb0 666c6f61 74325330 5f6d506d 005f5a31 float2S0_mPm._Z1
-  0x00006cc0 39616374 696f6e4f 6e53696e 676c6551 9actionOnSingleQ
-  0x00006cd0 75626974 5036666c 6f617432 53305f6d ubitP6float2S0_m
-  0x00006ce0 506d002e 74657874 2e5f5a31 39616374 Pm..text._Z19act
-  0x00006cf0 696f6e4f 6e53696e 676c6551 75626974 ionOnSingleQubit
-  0x00006d00 5036666c 6f617432 53305f6d 506d002e P6float2S0_mPm..
-  0x00006d10 6e762e69 6e666f2e 5f5a3139 61637469 nv.info._Z19acti
-  0x00006d20 6f6e4f6e 53696e67 6c655175 62697450 onOnSingleQubitP
-  0x00006d30 36666c6f 61743253 305f6d50 6d002e6e 6float2S0_mPm..n
-  0x00006d40 762e7368 61726564 2e5f5a31 39616374 v.shared._Z19act
-  0x00006d50 696f6e4f 6e53696e 676c6551 75626974 ionOnSingleQubit
-  0x00006d60 5036666c 6f617432 53305f6d 506d002e P6float2S0_mPm..
-  0x00006d70 6e762e63 6f6e7374 616e7430 2e5f5a31 nv.constant0._Z1
-  0x00006d80 39616374 696f6e4f 6e53696e 676c6551 9actionOnSingleQ
-  0x00006d90 75626974 5036666c 6f617432 53305f6d ubitP6float2S0_m
-  0x00006da0 506d002e 64656275 675f6672 616d6500 Pm..debug_frame.
-  0x00006db0 2e72656c 2e646562 75675f66 72616d65 .rel.debug_frame
-  0x00006dc0 002e7265 6c612e64 65627567 5f667261 ..rela.debug_fra
-  0x00006dd0 6d65002e 6e762e72 656c2e61 6374696f me..nv.rel.actio
-  0x00006de0 6e000000 00000000 00000000 00000000 n...............
-  0x00006df0 00000000 00000000 00000000 00000000 ................
-  0x00006e00 57000000 03000e00 00000000 00000000 W...............
-  0x00006e10 00000000 00000000 e0000000 03000b00 ................
+  0x00006ba0 2e736861 7265642e 5f5a3138 61637469 .shared._Z18acti
+  0x00006bb0 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
+  0x00006bc0 666c6f61 74325330 5f6d506d 002e6e76 float2S0_mPm..nv
+  0x00006bd0 2e636f6e 7374616e 74302e5f 5a313861 .constant0._Z18a
+  0x00006be0 6374696f 6e4f6e54 7269706c 65476174 ctionOnTripleGat
+  0x00006bf0 65503666 6c6f6174 3253305f 6d506d00 eP6float2S0_mPm.
+  0x00006c00 5f706172 616d005f 5a313961 6374696f _param._Z19actio
+  0x00006c10 6e4f6e44 6f75626c 65517562 69745036 nOnDoubleQubitP6
+  0x00006c20 666c6f61 74325330 5f6d506d 002e7465 float2S0_mPm..te
+  0x00006c30 78742e5f 5a313961 6374696f 6e4f6e44 xt._Z19actionOnD
+  0x00006c40 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
+  0x00006c50 74325330 5f6d506d 002e6e76 2e696e66 t2S0_mPm..nv.inf
+  0x00006c60 6f2e5f5a 31396163 74696f6e 4f6e446f o._Z19actionOnDo
+  0x00006c70 75626c65 51756269 74503666 6c6f6174 ubleQubitP6float
+  0x00006c80 3253305f 6d506d00 2e6e762e 73686172 2S0_mPm..nv.shar
+  0x00006c90 65642e5f 5a313961 6374696f 6e4f6e44 ed._Z19actionOnD
+  0x00006ca0 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
+  0x00006cb0 74325330 5f6d506d 002e6e76 2e636f6e t2S0_mPm..nv.con
+  0x00006cc0 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
+  0x00006cd0 6e4f6e44 6f75626c 65517562 69745036 nOnDoubleQubitP6
+  0x00006ce0 666c6f61 74325330 5f6d506d 005f5a31 float2S0_mPm._Z1
+  0x00006cf0 39616374 696f6e4f 6e53696e 676c6551 9actionOnSingleQ
+  0x00006d00 75626974 5036666c 6f617432 53305f6d ubitP6float2S0_m
+  0x00006d10 506d002e 74657874 2e5f5a31 39616374 Pm..text._Z19act
+  0x00006d20 696f6e4f 6e53696e 676c6551 75626974 ionOnSingleQubit
+  0x00006d30 5036666c 6f617432 53305f6d 506d002e P6float2S0_mPm..
+  0x00006d40 6e762e69 6e666f2e 5f5a3139 61637469 nv.info._Z19acti
+  0x00006d50 6f6e4f6e 53696e67 6c655175 62697450 onOnSingleQubitP
+  0x00006d60 36666c6f 61743253 305f6d50 6d002e6e 6float2S0_mPm..n
+  0x00006d70 762e7368 61726564 2e5f5a31 39616374 v.shared._Z19act
+  0x00006d80 696f6e4f 6e53696e 676c6551 75626974 ionOnSingleQubit
+  0x00006d90 5036666c 6f617432 53305f6d 506d002e P6float2S0_mPm..
+  0x00006da0 6e762e63 6f6e7374 616e7430 2e5f5a31 nv.constant0._Z1
+  0x00006db0 39616374 696f6e4f 6e53696e 676c6551 9actionOnSingleQ
+  0x00006dc0 75626974 5036666c 6f617432 53305f6d ubitP6float2S0_m
+  0x00006dd0 506d002e 64656275 675f6672 616d6500 Pm..debug_frame.
+  0x00006de0 2e72656c 2e646562 75675f66 72616d65 .rel.debug_frame
+  0x00006df0 002e7265 6c612e64 65627567 5f667261 ..rela.debug_fra
+  0x00006e00 6d65002e 6e762e72 656c2e61 6374696f me..nv.rel.actio
+  0x00006e10 6e000000 00000000 00000000 00000000 n...............
   0x00006e20 00000000 00000000 00000000 00000000 ................
-  0x00006e30 40010000 03000f00 00000000 00000000 @...............
-  0x00006e40 00000000 00000000 cc010000 03000c00 ................
+  0x00006e30 57000000 03000e00 00000000 00000000 W...............
+  0x00006e40 00000000 00000000 e0000000 03000b00 ................
   0x00006e50 00000000 00000000 00000000 00000000 ................
-  0x00006e60 26020000 03001000 00000000 00000000 &...............
-  0x00006e70 00000000 00000000 b2020000 03000d00 ................
+  0x00006e60 40010000 03000f00 00000000 00000000 @...............
+  0x00006e70 00000000 00000000 cc010000 03000c00 ................
   0x00006e80 00000000 00000000 00000000 00000000 ................
-  0x00006e90 e6020000 03000400 00000000 00000000 ................
-  0x00006ea0 00000000 00000000 16030000 03000900 ................
+  0x00006e90 26020000 03001000 00000000 00000000 &...............
+  0x00006ea0 00000000 00000000 b2020000 03000d00 ................
   0x00006eb0 00000000 00000000 00000000 00000000 ................
-  0x00006ec0 32000000 12100e00 00000000 00000000 2...............
-  0x00006ed0 001a0000 00000000 1a010000 12100f00 ................
-  0x00006ee0 00000000 00000000 80080000 00000000 ................
-  0x00006ef0 00020000 12101000 00000000 00000000 ................
-  0x00006f00 00040000 00000000 ffffffff 24000000 ............$...
-  0x00006f10 00000000 ffffffff ffffffff 0300047c ...............|
-  0x00006f20 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
-  0x00006f30 08818080 28000000 ffffffff 34000000 ....(.......4...
-  0x00006f40 00000000 00000000 00000000 00000000 ................
-  0x00006f50 00000000 001a0000 00000000 04040000 ................
-  0x00006f60 0004e000 00000c81 80802800 046c0500 ..........(..l..
-  0x00006f70 00000000 00000000 ffffffff 24000000 ............$...
-  0x00006f80 00000000 ffffffff ffffffff 0300047c ...............|
-  0x00006f90 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
-  0x00006fa0 08818080 28000000 ffffffff 34000000 ....(.......4...
-  0x00006fb0 00000000 70000000 00000000 00000000 ....p...........
-  0x00006fc0 00000000 80080000 00000000 04040000 ................
-  0x00006fd0 00046800 00000c81 80802800 04800100 ..h.......(.....
-  0x00006fe0 00000000 00000000 ffffffff 24000000 ............$...
-  0x00006ff0 00000000 ffffffff ffffffff 0300047c ...............|
-  0x00007000 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
-  0x00007010 08818080 28000000 ffffffff 34000000 ....(.......4...
-  0x00007020 00000000 e0000000 00000000 00000000 ................
-  0x00007030 00000000 00040000 00000000 04040000 ................
-  0x00007040 00044000 00000c81 80802800 04780000 ..@.......(..x..
-  0x00007050 00000000 00000000 042f0800 0b000000 ........./......
-  0x00007060 18000000 04230800 0b000000 00000000 .....#..........
-  0x00007070 04120800 0b000000 00000000 04110800 ................
-  0x00007080 0b000000 00000000 042f0800 0a000000 ........./......
-  0x00007090 22000000 04230800 0a000000 00000000 "....#..........
-  0x000070a0 04120800 0a000000 00000000 04110800 ................
-  0x000070b0 0a000000 00000000 042f0800 09000000 ........./......
-  0x000070c0 34000000 04230800 09000000 00000000 4....#..........
-  0x000070d0 04120800 09000000 00000000 04110800 ................
-  0x000070e0 09000000 00000000 04370400 76000000 .........7..v...
-  0x000070f0 01350000 040a0800 02000000 60012000 .5..........`. .
-  0x00007100 03192000 04170c00 00000000 03001800 .. .............
-  0x00007110 00f02100 04170c00 00000000 02001000 ..!.............
-  0x00007120 00f02100 04170c00 00000000 01000800 ..!.............
-  0x00007130 00f02100 04170c00 00000000 00000000 ..!.............
-  0x00007140 00f02100 031bff00 041c0800 80030000 ..!.............
-  0x00007150 40190000 04370400 76000000 01350000 @....7..v....5..
-  0x00007160 040a0800 04000000 60012000 03192000 ........`. ... .
-  0x00007170 04170c00 00000000 03001800 00f02100 ..............!.
-  0x00007180 04170c00 00000000 02001000 00f02100 ..............!.
-  0x00007190 04170c00 00000000 01000800 00f02100 ..............!.
-  0x000071a0 04170c00 00000000 00000000 00f02100 ..............!.
-  0x000071b0 031bff00 041c0800 a0010000 b0070000 ................
-  0x000071c0 04370400 76000000 01350000 040a0800 .7..v....5......
-  0x000071d0 06000000 60012000 03192000 04170c00 ....`. ... .....
-  0x000071e0 00000000 03001800 00f02100 04170c00 ..........!.....
-  0x000071f0 00000000 02001000 00f02100 04170c00 ..........!.....
-  0x00007200 00000000 01000800 00f02100 04170c00 ..........!.....
-  0x00007210 00000000 00000000 00f02100 031bff00 ..........!.....
-  0x00007220 041c0800 00010000 f0020000 00000000 ................
-  0x00007230 4b000000 00000000 00020208 100a2f22 K............./"
-  0x00007240 00000008 00000000 00000808 00000000 ................
-  0x00007250 00001008 00000000 00001808 00000000 ................
-  0x00007260 00002008 00000000 00002808 00000000 .. .......(.....
-  0x00007270 00003008 00000000 00003808 00000000 ..0.......8.....
-  0x00007280 01000008 00000000 01000808 00000000 ................
-  0x00007290 01001008 00000000 01001808 00000000 ................
-  0x000072a0 01002008 00000000 01002808 00000000 .. .......(.....
-  0x000072b0 01003008 00000000 01003808 00000000 ..0.......8.....
-  0x000072c0 02000008 00000000 02000808 00000000 ................
-  0x000072d0 02001008 00000000 02001808 00000000 ................
-  0x000072e0 02002008 00000000 02002808 00000000 .. .......(.....
-  0x000072f0 02003008 00000000 02003808 00000000 ..0.......8.....
-  0x00007300 00000014 2c000000 0300000c 00000000 ....,...........
-  0x00007310 24010000 00000000 02000000 0b000000 $...............
-  0x00007320 b4000000 00000000 02000000 0a000000 ................
-  0x00007330 44000000 00000000 02000000 09000000 D...............
-  0x00007340 00000000 00000000 00000000 00000000 ................
-  0x00007350 00000000 00000000 00000000 00000000 ................
-  0x00007360 00000000 00000000 00000000 00000000 ................
+  0x00006ec0 e6020000 03000400 00000000 00000000 ................
+  0x00006ed0 00000000 00000000 16030000 03000900 ................
+  0x00006ee0 00000000 00000000 00000000 00000000 ................
+  0x00006ef0 32000000 12100e00 00000000 00000000 2...............
+  0x00006f00 001a0000 00000000 1a010000 12100f00 ................
+  0x00006f10 00000000 00000000 80080000 00000000 ................
+  0x00006f20 00020000 12101000 00000000 00000000 ................
+  0x00006f30 00040000 00000000 ffffffff 24000000 ............$...
+  0x00006f40 00000000 ffffffff ffffffff 0300047c ...............|
+  0x00006f50 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
+  0x00006f60 08818080 28000000 ffffffff 34000000 ....(.......4...
+  0x00006f70 00000000 00000000 00000000 00000000 ................
+  0x00006f80 00000000 001a0000 00000000 04040000 ................
+  0x00006f90 0004e000 00000c81 80802800 046c0500 ..........(..l..
+  0x00006fa0 00000000 00000000 ffffffff 24000000 ............$...
+  0x00006fb0 00000000 ffffffff ffffffff 0300047c ...............|
+  0x00006fc0 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
+  0x00006fd0 08818080 28000000 ffffffff 34000000 ....(.......4...
+  0x00006fe0 00000000 70000000 00000000 00000000 ....p...........
+  0x00006ff0 00000000 80080000 00000000 04040000 ................
+  0x00007000 00046800 00000c81 80802800 04800100 ..h.......(.....
+  0x00007010 00000000 00000000 ffffffff 24000000 ............$...
+  0x00007020 00000000 ffffffff ffffffff 0300047c ...............|
+  0x00007030 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
+  0x00007040 08818080 28000000 ffffffff 34000000 ....(.......4...
+  0x00007050 00000000 e0000000 00000000 00000000 ................
+  0x00007060 00000000 00040000 00000000 04040000 ................
+  0x00007070 00044000 00000c81 80802800 04780000 ..@.......(..x..
+  0x00007080 00000000 00000000 042f0800 0b000000 ........./......
+  0x00007090 18000000 04230800 0b000000 00000000 .....#..........
+  0x000070a0 04120800 0b000000 00000000 04110800 ................
+  0x000070b0 0b000000 00000000 042f0800 0a000000 ........./......
+  0x000070c0 22000000 04230800 0a000000 00000000 "....#..........
+  0x000070d0 04120800 0a000000 00000000 04110800 ................
+  0x000070e0 0a000000 00000000 042f0800 09000000 ........./......
+  0x000070f0 34000000 04230800 09000000 00000000 4....#..........
+  0x00007100 04120800 09000000 00000000 04110800 ................
+  0x00007110 09000000 00000000 04370400 76000000 .........7..v...
+  0x00007120 01350000 040a0800 02000000 60012000 .5..........`. .
+  0x00007130 03192000 04170c00 00000000 03001800 .. .............
+  0x00007140 00f02100 04170c00 00000000 02001000 ..!.............
+  0x00007150 00f02100 04170c00 00000000 01000800 ..!.............
+  0x00007160 00f02100 04170c00 00000000 00000000 ..!.............
+  0x00007170 00f02100 031bff00 041c0800 80030000 ..!.............
+  0x00007180 40190000 04370400 76000000 01350000 @....7..v....5..
+  0x00007190 040a0800 04000000 60012000 03192000 ........`. ... .
+  0x000071a0 04170c00 00000000 03001800 00f02100 ..............!.
+  0x000071b0 04170c00 00000000 02001000 00f02100 ..............!.
+  0x000071c0 04170c00 00000000 01000800 00f02100 ..............!.
+  0x000071d0 04170c00 00000000 00000000 00f02100 ..............!.
+  0x000071e0 031bff00 041c0800 a0010000 b0070000 ................
+  0x000071f0 04370400 76000000 01350000 040a0800 .7..v....5......
+  0x00007200 06000000 60012000 03192000 04170c00 ....`. ... .....
+  0x00007210 00000000 03001800 00f02100 04170c00 ..........!.....
+  0x00007220 00000000 02001000 00f02100 04170c00 ..........!.....
+  0x00007230 00000000 01000800 00f02100 04170c00 ..........!.....
+  0x00007240 00000000 00000000 00f02100 031bff00 ..........!.....
+  0x00007250 041c0800 00010000 f0020000 00000000 ................
+  0x00007260 4b000000 00000000 00020208 100a2f22 K............./"
+  0x00007270 00000008 00000000 00000808 00000000 ................
+  0x00007280 00001008 00000000 00001808 00000000 ................
+  0x00007290 00002008 00000000 00002808 00000000 .. .......(.....
+  0x000072a0 00003008 00000000 00003808 00000000 ..0.......8.....
+  0x000072b0 01000008 00000000 01000808 00000000 ................
+  0x000072c0 01001008 00000000 01001808 00000000 ................
+  0x000072d0 01002008 00000000 01002808 00000000 .. .......(.....
+  0x000072e0 01003008 00000000 01003808 00000000 ..0.......8.....
+  0x000072f0 02000008 00000000 02000808 00000000 ................
+  0x00007300 02001008 00000000 02001808 00000000 ................
+  0x00007310 02002008 00000000 02002808 00000000 .. .......(.....
+  0x00007320 02003008 00000000 02003808 00000000 ..0.......8.....
+  0x00007330 00000014 2c000000 0300000c 00000000 ....,...........
+  0x00007340 24010000 00000000 02000000 0b000000 $...............
+  0x00007350 b4000000 00000000 02000000 0a000000 ................
+  0x00007360 44000000 00000000 02000000 09000000 D...............
   0x00007370 00000000 00000000 00000000 00000000 ................
   0x00007380 00000000 00000000 00000000 00000000 ................
   0x00007390 00000000 00000000 00000000 00000000 ................
   0x000073a0 00000000 00000000 00000000 00000000 ................
   0x000073b0 00000000 00000000 00000000 00000000 ................
   0x000073c0 00000000 00000000 00000000 00000000 ................
   0x000073d0 00000000 00000000 00000000 00000000 ................
@@ -329,1207 +326,1210 @@
   0x00007760 00000000 00000000 00000000 00000000 ................
   0x00007770 00000000 00000000 00000000 00000000 ................
   0x00007780 00000000 00000000 00000000 00000000 ................
   0x00007790 00000000 00000000 00000000 00000000 ................
   0x000077a0 00000000 00000000 00000000 00000000 ................
   0x000077b0 00000000 00000000 00000000 00000000 ................
   0x000077c0 00000000 00000000 00000000 00000000 ................
-  0x000077d0 027a0100 000a0000 000f0000 00c40f00 .z..............
-  0x000077e0 027a0400 005e0000 000f0000 00e20f00 .z...^..........
-  0x000077f0 b97a0600 00460000 000a0000 00e20f00 .z...F..........
-  0x00007800 027a0500 005f0000 000f0000 00ca0f00 .z..._..........
-  0x00007810 81790304 06080000 00191e0c 00a80e00 .y..............
-  0x00007820 81790604 06000000 00191e0c 00e80e00 .y..............
-  0x00007830 81790804 06100000 00191e0c 00220f00 .y..........."..
-  0x00007840 b97a0400 00000000 00080000 00e40f00 .z..............
-  0x00007850 9978043f 01000000 04160108 00e20f00 .x.?............
-  0x00007860 19790b00 00000000 00250000 00280e00 .y.......%...(..
-  0x00007870 19790a00 00000000 00210000 00240e00 .y.......!...$..
-  0x00007880 247a0b0b 00000000 0a028e07 00ca1f00 $z..............
-  0x00007890 1272020b 03000000 fffc8e07 00e44f0c .r............O.
-  0x000078a0 1272100b 06000000 fffc8e07 00e48f04 .r..............
-  0x000078b0 10720006 03000000 ffe0ff07 00e40f00 .r..............
-  0x000078c0 0c72000b 02000000 7052f003 00e40f04 .r......pR......
-  0x000078d0 1272070b 00000000 fffc8e07 00e40f04 .r..............
-  0x000078e0 0c72000b 10000000 70527000 00c40f00 .r......pRp.....
-  0x000078f0 10720c06 08000000 ffe0ff07 00e40f09 .r..............
-  0x00007900 1272000b 08000000 fffc8e07 00e40f0c .r..............
-  0x00007910 0c72000b 07000000 70527000 00e40f00 .r......pRp.....
-  0x00007920 10720303 08000000 ffe0ff07 00e40f00 .r..............
-  0x00007930 1272080b 0c000000 fffc8e07 00e40f04 .r..............
-  0x00007940 0c72000b 00000000 70527000 00c40f00 .r......pRp.....
-  0x00007950 10720606 03000000 ffe0ff07 00e40f08 .r..............
-  0x00007960 1272040b 03000000 fffc8e07 00e40f04 .r..............
-  0x00007970 0c72000b 08000000 70527000 00e40f04 .r......pRp.....
-  0x00007980 1272050b 06000000 fffc8e07 00e40f04 .r..............
-  0x00007990 0c72000b 04000000 70527000 00e40f00 .r......pRp.....
-  0x000079a0 197803ff 1f000000 0b140100 00c40f00 .x..............
-  0x000079b0 0c72000b 05000000 70527000 00c80f00 .r......pRp.....
-  0x000079c0 0c720010 02000000 70527000 00c80f00 .r......pRp.....
-  0x000079d0 0c720010 07000000 70527000 00c80f00 .r......pRp.....
-  0x000079e0 0c720010 00000000 70527000 00c80f00 .r......pRp.....
-  0x000079f0 0c720010 08000000 70527000 00c80f00 .r......pRp.....
-  0x00007a00 0c720010 04000000 70527000 00c80f00 .r......pRp.....
-  0x00007a10 0c720010 05000000 70527000 00c80f00 .r......pRp.....
-  0x00007a20 0c720002 07000000 70527000 00c80f00 .r......pRp.....
-  0x00007a30 0c720002 00000000 70527000 00c80f00 .r......pRp.....
-  0x00007a40 0c720002 08000000 70527000 00c80f00 .r......pRp.....
-  0x00007a50 0c720002 04000000 70527000 00c80f00 .r......pRp.....
-  0x00007a60 0c720002 05000000 70527000 00c80f00 .r......pRp.....
-  0x00007a70 0c720007 00000000 70527000 00c80f00 .r......pRp.....
-  0x00007a80 0c720007 08000000 70527000 00c80f00 .r......pRp.....
-  0x00007a90 0c720007 04000000 70527000 00c80f00 .r......pRp.....
-  0x00007aa0 0c720007 05000000 70527000 00c80f00 .r......pRp.....
-  0x00007ab0 0c720000 08000000 70527000 00c80f00 .r......pRp.....
-  0x00007ac0 0c720000 04000000 70527000 00c80f00 .r......pRp.....
-  0x00007ad0 0c720000 05000000 70527200 00e40f08 .r......pRr.....
-  0x00007ae0 0c7a000b 005c0000 7060f003 00e40f00 .z...\..p`......
-  0x00007af0 0c720008 04000000 7052f200 00e40f04 .r......pR......
-  0x00007b00 0c7a0003 005d0000 0061f003 00e40f00 .z...]...a......
-  0x00007b10 0c720008 05000000 7052f200 00e40f00 .r......pR......
-  0x00007b20 0c7c000a 04000000 7010700c 00c40f00 .|......p.p.....
-  0x00007b30 0c720004 05000000 7052f200 00c80f00 .r......pR......
-  0x00007b40 1c780000 00000000 70307000 00da0f00 .x......p0p.....
-  0x00007b50 4d890000 00000000 00008003 00ea0f00 M...............
-  0x00007b60 357403ff 08000000 ff010000 00e20f00 5t..............
-  0x00007b70 027a2800 005a0000 000f0000 00e40f00 .z(..Z..........
-  0x00007b80 027a2900 005b0000 000f0000 00ca0f00 .z)..[..........
-  0x00007b90 81792428 06400000 001b1e0c 00a40e00 .y$(.@..........
-  0x00007ba0 25760a0b 00580000 03028e07 00e40f08 %v...X..........
-  0x00007bb0 81792228 06800000 001b1e0c 00e80e00 .y"(............
-  0x00007bc0 81791e0a 06000000 001b1e0c 00a80e00 .y..............
-  0x00007bd0 81791228 06c00000 001b1e0c 00280f00 .y.(.........(..
-  0x00007be0 81791a28 06000100 001b1e0c 00680f00 .y.(.........h..
-  0x00007bf0 81790c28 06400100 001b1e0c 00280f00 .y.(.@.......(..
-  0x00007c00 81792628 06000000 001b1e0c 00280f00 .y&(.........(..
-  0x00007c10 81792028 06c00100 001b1e0c 00680f00 .y (.........h..
-  0x00007c20 81791628 06800100 001b1e0c 00620f00 .y.(.........b..
-  0x00007c30 25761010 00580000 03028e07 00c60f00 %v...X..........
-  0x00007c40 81791828 06080000 001b1e0c 00680f00 .y.(.........h..
-  0x00007c50 81790e10 06000000 001b1e0c 00680f00 .y...........h..
-  0x00007c60 81791428 06880000 001b1e0c 00680f00 .y.(.........h..
-  0x00007c70 81791c28 06480000 001b1e0c 00620f00 .y.(.H.......b..
-  0x00007c80 2072091f 25000000 00004000 00c44f00  r..%.....@...O.
-  0x00007c90 2072061e 25000000 00004000 00e40f04  r..%.....@.....
-  0x00007ca0 2372091e 24000000 09080000 00e40f0c #r..$...........
-  0x00007cb0 2372061f 24000000 06000000 00e40f04 #r..$...........
-  0x00007cc0 2072251f 23000000 00004000 00e48f08  r%.#.....@.....
-  0x00007cd0 2072241e 23000000 00004000 00e40f04  r$.#.....@.....
-  0x00007ce0 2372231e 22000000 25080000 00c40f00 #r#."...%.......
-  0x00007cf0 2372221f 22000000 24000000 00e40f04 #r"."...$.......
-  0x00007d00 2072251f 13000000 00004000 00e40f0d  r%.......@.....
-  0x00007d10 2072241e 13000000 00004000 00e40f04  r$.......@.....
-  0x00007d20 2372131e 12000000 25080000 00e40f08 #r......%.......
-  0x00007d30 2372121f 12000000 24000000 00e40f04 #r......$.......
-  0x00007d40 2072251f 1b000000 00004000 00c40f02  r%.......@.....
-  0x00007d50 2072241e 1b000000 00004000 00e40f04  r$.......@.....
-  0x00007d60 23721b1e 1a000000 25080000 00e40f0c #r......%.......
-  0x00007d70 23721a1f 1a000000 24000000 00e40f04 #r......$.......
-  0x00007d80 2072251f 0d000000 00004000 00e40f08  r%.......@.....
-  0x00007d90 2072241e 0d000000 00004000 00e40f00  r$.......@.....
-  0x00007da0 20722b27 1f000000 00004000 00c40f00  r+'......@.....
-  0x00007db0 20722a27 1e000000 00004000 00e40f00  r*'......@.....
-  0x00007dc0 2372251e 0c000000 25080000 00e40f0c #r%.....%.......
-  0x00007dd0 2372241f 0c000000 24000000 00e40f04 #r$.....$.......
-  0x00007de0 20720d1f 21000000 00004000 00e40f08  r..!.....@.....
-  0x00007df0 20720c1e 21000000 00004000 00e40f00  r..!.....@.....
-  0x00007e00 23722b26 1e000000 2b080000 00c40f00 #r+&....+.......
-  0x00007e10 23722a26 1f000000 2a000000 00e40f00 #r*&....*.......
-  0x00007e20 2072271f 17000000 00004000 00e40f0c  r'.......@.....
-  0x00007e30 2072261e 17000000 00004000 00e40f04  r&.......@.....
-  0x00007e40 2372211e 20000000 0d080000 00e40f0c #r!. ...........
-  0x00007e50 2372201f 20000000 0c000000 00e40f04 #r . ...........
-  0x00007e60 2372271e 16000000 27080000 00e20f08 #r'.....'.......
-  0x00007e70 81790c28 06c80000 001b1e0c 00a20e00 .y.(............
-  0x00007e80 2372261f 16000000 26000000 00c60f00 #r&.....&.......
-  0x00007e90 81791628 06080100 001b1e0c 00e20e00 .y.(............
-  0x00007ea0 23721e18 0e000000 2b000000 00e40f0c #r......+.......
-  0x00007eb0 23722b18 0f000000 2a000000 00e40f08 #r+.....*.......
-  0x00007ec0 23722a19 0f000000 1e010000 00e40f04 #r*.............
-  0x00007ed0 23722b19 0e000000 2b000000 00e20f00 #r+.....+.......
-  0x00007ee0 81791e28 06880100 001b1e0c 00280f00 .y.(.........(..
-  0x00007ef0 81791828 06480100 001b1e0c 00620f00 .y.(.H.......b..
-  0x00007f00 23722e0e 14000000 23000000 00c40f00 #r......#.......
-  0x00007f10 23722c0e 1c000000 09000000 00e40f08 #r,.............
-  0x00007f20 23721c0f 1c000000 06000000 00e40f04 #r..............
-  0x00007f30 2372220f 14000000 22000000 00e40f04 #r".....".......
-  0x00007f40 2372090f 15000080 2e000000 00e40f00 #r..............
-  0x00007f50 25762e02 00580000 03028e07 00c80f00 %v...X..........
-  0x00007f60 2372060f 1d000080 2c000000 00e40f0c #r......,.......
-  0x00007f70 23722c0e 1d000000 1c000000 00e40f04 #r,.............
-  0x00007f80 81791c28 06c80100 001b1e0c 00220f00 .y.(........."..
-  0x00007f90 2372220e 15000000 22000000 00e40f04 #r".....".......
-  0x00007fa0 2372140e 0c000000 13000000 00e44f0c #r............O.
-  0x00007fb0 2372120f 0c000000 12000000 00e40f00 #r..............
-  0x00007fc0 23720c0e 16000000 1b000000 00c48f00 #r..............
-  0x00007fd0 2372160f 16000000 1a000000 00e40f04 #r..............
-  0x00007fe0 23721b0f 0d000080 14000000 00e40f0c #r..............
-  0x00007ff0 23721a0e 0d000000 12000000 00e20f00 #r..............
-  0x00008000 81791428 06500000 001b1e0c 00a20e00 .y.(.P..........
-  0x00008010 2372230f 17000080 0c000000 00c60f00 #r#.............
-  0x00008020 81790c28 06100000 001b1e0c 00e80e00 .y.(............
-  0x00008030 8179122e 06000000 001b1e0c 00e20e00 .y..............
-  0x00008040 2372020e 17000000 16000000 00e40f04 #r..............
-  0x00008050 2372160e 18000000 25000000 00e40f0e #r......%.......
-  0x00008060 2372240f 18000000 24000000 00e40f00 #r$.....$.......
-  0x00008070 2372180e 1e000000 27000000 00c40f01 #r......'.......
-  0x00008080 2372260f 1e000000 26000000 00e40f04 #r&.....&.......
-  0x00008090 2372250f 19000080 16000000 00e40f0c #r%.............
-  0x000080a0 23721e0e 19000000 24000000 00e20f00 #r......$.......
-  0x000080b0 81791628 06900000 001b1e0c 00220f00 .y.(........."..
-  0x000080c0 2372270f 1f000080 18000000 00c60f00 #r'.............
-  0x000080d0 81791828 06d00000 001b1e0c 00620f00 .y.(.........b..
-  0x000080e0 2372240e 1c000000 21000000 00e40f0c #r$.....!.......
-  0x000080f0 2372200f 1c000000 20000000 00e40f04 #r ..... .......
-  0x00008100 2372210f 1d000080 24000000 00e40f08 #r!.....$.......
-  0x00008110 23721d0e 1d000000 20000000 00e40f04 #r...... .......
-  0x00008120 23721f0e 1f000000 26000000 00e40f00 #r......&.......
-  0x00008130 81790e28 06500100 001b1e0c 00620f00 .y.(.P.......b..
-  0x00008140 23721c0c 12000000 2a000000 00c48f00 #r......*.......
-  0x00008150 23722b0c 13000000 2b000000 00e40f08 #r+.....+.......
-  0x00008160 23721c0d 13000000 1c010000 00e40f04 #r..............
-  0x00008170 2372200d 12000000 2b000000 00e40f00 #r .....+.......
-  0x00008180 81790c28 06100100 001b1e0c 00e20e00 .y.(............
-  0x00008190 23720612 14000000 06000000 00e44f08 #r............O.
-  0x000081a0 23722413 14000000 2c000000 00e40f04 #r$.....,.......
-  0x000081b0 23720613 15000080 06000000 00c40f00 #r..............
-  0x000081c0 23722412 15000000 24000000 00e40f04 #r$.....$.......
-  0x000081d0 81791428 06900100 001b1e0c 00a20e00 .y.(............
-  0x000081e0 23722612 16000000 09000000 00e40f0d #r&.............
-  0x000081f0 23722213 16000000 22000000 00e40f04 #r".....".......
-  0x00008200 23721612 18000000 1b000000 00e40f0a #r..............
-  0x00008210 23721813 18000000 1a000000 00e40f04 #r..............
-  0x00008220 81791a28 06d00100 001b1e0c 00220f00 .y.(........."..
-  0x00008230 23720913 17000080 26000000 00c40f00 #r......&.......
-  0x00008240 23721712 17000000 22000000 00e40f04 #r......".......
-  0x00008250 23722212 19000000 18000000 00e40f00 #r".............
-  0x00008260 23721e13 0e000000 1e000000 00e40f00 #r..............
-  0x00008270 25762c07 00580000 03028e07 00c80f00 %v,..X..........
-  0x00008280 23722612 0f000000 1e000000 00e40f04 #r&.............
-  0x00008290 23721613 19000080 16000000 00e40f04 #r..............
-  0x000082a0 23721812 0c000000 23000000 00e48f0c #r......#.......
-  0x000082b0 23720213 0c000000 02000000 00e40f04 #r..............
-  0x000082c0 23720c12 0e000000 25000000 00e40f00 #r......%.......
-  0x000082d0 23722313 0d000080 18000000 00c40f00 #r#.............
-  0x000082e0 23720212 0d000000 02000000 00e40f04 #r..............
-  0x000082f0 23720713 0f000080 0c000000 00e40f04 #r..............
-  0x00008300 23721812 14000000 27000000 00e24f08 #r......'.....O.
-  0x00008310 81790c28 06180000 001b1e0c 00a20e00 .y.(............
-  0x00008320 23721f13 14000000 1f000000 00c60f00 #r..............
-  0x00008330 81790e2c 06000000 001b1e0c 00a20e00 .y.,............
-  0x00008340 23722513 15000080 18000000 00e40f0c #r%.............
-  0x00008350 23722a12 15000000 1f000000 00e20f04 #r*.............
-  0x00008360 81791828 06980000 001b1e0c 00e80e00 .y.(............
-  0x00008370 81791428 06580000 001b1e0c 00620f00 .y.(.X.......b..
-  0x00008380 23721e12 1a000000 21000000 00e40f09 #r......!.......
-  0x00008390 23721a13 1a000000 1d000000 00c40f00 #r..............
-  0x000083a0 23721d13 1b000080 1e000000 00e40f08 #r..............
-  0x000083b0 81791e28 06d80000 001b1e0c 00220f00 .y.(........."..
-  0x000083c0 23721b12 1b000000 1a000000 00e40f00 #r..............
-  0x000083d0 23721c0c 0e000000 1c000000 00e44f0c #r............O.
-  0x000083e0 2372200c 0f000000 20000000 00e40f08 #r ..... .......
-  0x000083f0 23721a0d 0f000000 1c010000 00e40f04 #r..............
-  0x00008400 23721c0d 0e000000 20000000 00c40f00 #r...... .......
-  0x00008410 2372120e 18000000 09000000 00e28f04 #r..............
-  0x00008420 81790c28 06180100 001b1e0c 00a20e00 .y.(............
-  0x00008430 2372060e 14000000 06000000 00e40f0e #r..............
-  0x00008440 2372240f 14000000 24000000 00e40f04 #r$.....$.......
-  0x00008450 2372170f 18000000 17000000 00e40f04 #r..............
-  0x00008460 2372180f 19000080 12000000 00e40f04 #r..............
-  0x00008470 2372060f 15000080 06000000 00e20f08 #r..............
-  0x00008480 81791228 06580100 001b1e0c 00e20e00 .y.(.X..........
-  0x00008490 2372090e 15000000 24000000 00c60f00 #r......$.......
-  0x000084a0 81791428 06980100 001b1e0c 00620f00 .y.(.........b..
-  0x000084b0 2372190e 19000000 17000000 00e40f04 #r..............
-  0x000084c0 2372200e 1e000000 16000000 00e40f0d #r .............
-  0x000084d0 81791628 06d80100 001b1e0c 00220f00 .y.(........."..
-  0x000084e0 2372220f 1e000000 22000000 00e40f04 #r".....".......
-  0x000084f0 23721e0e 0c000000 23000000 00e44f08 #r......#.....O.
-  0x00008500 2372210f 0c000000 02000000 00c40f00 #r!.............
-  0x00008510 23720c0f 0d000080 1e000000 00e40f04 #r..............
-  0x00008520 2372020f 1f000080 20000000 00e40f04 #r...... .......
-  0x00008530 23721e0e 12000000 07000000 00e48f0c #r..............
-  0x00008540 2372240f 12000000 26000000 00e40f04 #r$.....&.......
-  0x00008550 2372120e 14000000 25000000 00e40f0a #r......%.......
-  0x00008560 2372140f 14000000 2a000000 00c40f00 #r......*.......
-  0x00008570 25762a00 00580000 03028e07 00c80f00 %v*..X..........
-  0x00008580 2372200e 1f000000 22000000 00e40f04 #r .....".......
-  0x00008590 2372220e 0d000000 21000000 00e40f04 #r".....!.......
-  0x000085a0 2372070f 13000080 1e000000 00e40f0c #r..............
-  0x000085b0 2372240e 13000000 24000000 00e20f04 #r$.....$.......
-  0x000085c0 81791e28 06600000 001b1e0c 00a20e00 .y.(.`..........
-  0x000085d0 23720d0f 15000080 12000000 00e40f08 #r..............
-  0x000085e0 2372000e 15000000 14000000 00e20f04 #r..............
-  0x000085f0 8179122a 06000000 001b1e0c 00e20e00 .y.*............
-  0x00008600 2372260e 16000000 1d000000 00c40f01 #r&.............
-  0x00008610 2372160f 16000000 1b000000 00e20f04 #r..............
-  0x00008620 81791428 06200000 001b1e0c 00e20e00 .y.(. ..........
-  0x00008630 23721b0f 17000080 26000000 00e40f08 #r......&.......
-  0x00008640 2372260e 17000000 16000000 00e40f00 #r&.............
-  0x00008650 81790e28 06a00000 001b1e0c 00280f00 .y.(.........(..
-  0x00008660 81791628 06e00000 001b1e0c 00620f00 .y.(.........b..
-  0x00008670 23721a14 12000000 1a000000 00c48f00 #r..............
-  0x00008680 23721c14 13000000 1c000000 00e40f08 #r..............
-  0x00008690 23721412 1e000000 06000000 00e44f0c #r............O.
-  0x000086a0 23721e13 1e000000 09000000 00e40f00 #r..............
-  0x000086b0 23720915 12000000 1c000000 00e40f04 #r..............
-  0x000086c0 23720615 13000000 1a010000 00e40f00 #r..............
-  0x000086d0 23721c12 0e000000 18000000 00c40f01 #r..............
-  0x000086e0 23721a13 1f000080 14000000 00e40f0c #r..............
-  0x000086f0 23720e13 0e000000 19000000 00e20f04 #r..............
-  0x00008700 81791428 06200100 001b1e0c 00a20e00 .y.(. ..........
-  0x00008710 23721f12 1f000000 1e000000 00e40f04 #r..............
-  0x00008720 23721e12 16000000 02000000 00e20f0a #r..............
-  0x00008730 81791828 06600100 001b1e0c 00e20e00 .y.(.`..........
-  0x00008740 23722013 16000000 20000000 00e40f04 #r ..... .......
-  0x00008750 23720213 0f000080 1c000000 00c40f00 #r..............
-  0x00008760 23721c12 0f000000 0e000000 00e40f04 #r..............
-  0x00008770 81790e28 06a00100 001b1e0c 00220f00 .y.(........."..
-  0x00008780 23721d13 17000080 1e000000 00e40f0c #r..............
-  0x00008790 23721e12 17000000 20000000 00e40f04 #r...... .......
-  0x000087a0 81791628 06e00100 001b1e0c 00620f00 .y.(.........b..
-  0x000087b0 23720c12 14000000 0c000000 00e44f08 #r............O.
-  0x000087c0 23722213 14000000 22000000 00c40f00 #r".....".......
-  0x000087d0 23721412 18000000 07000000 00e48f08 #r..............
-  0x000087e0 23720713 15000080 0c000000 00e40f04 #r..............
-  0x000087f0 23722013 18000000 24000000 00e40f00 #r .....$.......
-  0x00008800 25762408 00580000 03028e07 00c80f00 %v$..X..........
-  0x00008810 23720c12 0e000000 0d000000 00e40f0d #r..............
-  0x00008820 23720013 0e000000 00000000 00e40f04 #r..............
-  0x00008830 23721812 15000000 22000000 00e40f04 #r......".......
-  0x00008840 23720812 16000000 1b000000 00e40f0a #r..............
-  0x00008850 23722213 16000000 26000000 00e40f04 #r".....&.......
-  0x00008860 23722113 19000080 14000000 00c40f00 #r!.............
-  0x00008870 23722012 19000000 20000000 00e20f04 #r ..... .......
-  0x00008880 81791428 06680000 001b1e0c 00a20e00 .y.(.h..........
-  0x00008890 23721913 0f000080 0c000000 00e40f0c #r..............
-  0x000088a0 23720012 0f000000 00000000 00e20f04 #r..............
-  0x000088b0 81790c24 06000000 001b1e0c 00a20e00 .y.$............
-  0x000088c0 23721b13 17000080 08000000 00e40f08 #r..............
-  0x000088d0 23722212 17000000 22000000 00e20f00 #r".....".......
-  0x000088e0 81790e28 06280000 001b1e0c 00e80e00 .y.(.(..........
-  0x000088f0 81791228 06a80000 001b1e0c 00280f00 .y.(.........(..
-  0x00008900 81791628 06e80000 001b1e0c 00620f00 .y.(.........b..
-  0x00008910 2372230d 14000000 1f000000 00c44f00 #r#...........O.
-  0x00008920 2372090e 0d000000 09000000 00e48f04 #r..............
-  0x00008930 2372060e 0c000000 06000000 00e40f00 #r..............
-  0x00008940 2372020c 12000000 02000000 00e40f0d #r..............
-  0x00008950 23721c0d 12000000 1c000000 00e40f00 #r..............
-  0x00008960 23721f0f 0c000000 09000000 00e40f00 #r..............
-  0x00008970 23721a0c 14000000 1a000000 00e20f00 #r..............
-  0x00008980 81790828 06280100 001b1e0c 00a20e00 .y.(.(..........
-  0x00008990 2372020d 13000080 02000000 00c40f00 #r..............
-  0x000089a0 23721c0c 13000000 1c000000 00e40f04 #r..............
-  0x000089b0 2372060f 0d000000 06010000 00e20f00 #r..............
-  0x000089c0 81791228 06680100 001b1e0c 00e20e00 .y.(.h..........
-  0x000089d0 2372140c 16000000 1d000000 00c60f02 #r..............
-  0x000089e0 81790e28 06a80100 001b1e0c 00220f00 .y.(........."..
-  0x000089f0 23721e0d 16000000 1e000000 00e40f04 #r..............
-  0x00008a00 23721a0d 15000080 1a000000 00e40f0c #r..............
-  0x00008a10 2372230c 15000000 23000000 00e40f04 #r#.....#.......
-  0x00008a20 2372160d 17000080 14000000 00e40f08 #r..............
-  0x00008a30 81791428 06e80100 001b1e0c 00620f00 .y.(.........b..
-  0x00008a40 2372170c 17000000 1e000000 00c40f00 #r..............
-  0x00008a50 25762604 00580000 03028e07 00c80f00 %v&..X..........
-  0x00008a60 23721e0c 08000000 07000000 00e44f0c #r............O.
-  0x00008a70 2372180d 08000000 18000000 00e40f04 #r..............
-  0x00008a80 2372080c 12000000 21000000 00e48f0c #r......!.......
-  0x00008a90 2372200d 12000000 20000000 00e40f04 #r ..... .......
-  0x00008aa0 2372120c 0e000000 19000000 00e40f01 #r..............
-  0x00008ab0 2372070d 09000080 1e000000 00c40f00 #r..............
-  0x00008ac0 23720e0d 0e000000 00000000 00e40f04 #r..............
-  0x00008ad0 23721d0d 0f000080 12000000 00e40f04 #r..............
-  0x00008ae0 2372120c 14000000 1b000000 00e40f0e #r..............
-  0x00008af0 23721e0d 14000000 22000000 00e40f04 #r......".......
-  0x00008b00 2372180c 09000000 18000000 00e40f00 #r..............
-  0x00008b10 2372190d 13000080 08000000 00c40f00 #r..............
-  0x00008b20 2372000c 13000000 20000000 00e20f04 #r...... .......
-  0x00008b30 81790828 06300000 001b1e0c 00a20e00 .y.(.0..........
-  0x00008b40 2372040c 0f000000 0e000000 00e40f04 #r..............
-  0x00008b50 23721b0d 15000080 12000000 00e20f08 #r..............
-  0x00008b60 81790e26 06000000 001b1e0c 00a20e00 .y.&............
-  0x00008b70 23721e0c 15000000 1e000000 00c60f00 #r..............
-  0x00008b80 81790c28 06700000 001b1e0c 00e80e00 .y.(.p..........
-  0x00008b90 81791228 06b00000 001b1e0c 00280f00 .y.(.........(..
-  0x00008ba0 81791428 06f00000 001b1e0c 00620f00 .y.(.........b..
-  0x00008bb0 23720608 0e000000 06000000 00e44f04 #r............O.
-  0x00008bc0 23721f08 0f000000 1f000000 00c40f00 #r..............
-  0x00008bd0 23721a0e 0c000000 1a000000 00e48f0c #r..............
-  0x00008be0 2372230f 0c000000 23000000 00e40f04 #r#.....#.......
-  0x00008bf0 2372080e 12000000 02000000 00e40f0d #r..............
-  0x00008c00 2372020f 0d000080 1a000000 00e40f0c #r..............
-  0x00008c10 2372200f 12000000 1c000000 00e40f00 #r .............
-  0x00008c20 23721a0e 0d000000 23000000 00c40f00 #r......#.......
-  0x00008c30 23720609 0f000000 06010000 00e20f04 #r..............
-  0x00008c40 81790c28 06300100 001b1e0c 00a20e00 .y.(.0..........
-  0x00008c50 23721f09 0e000000 1f000000 00e40f00 #r..............
-  0x00008c60 23721c0f 13000080 08000000 00e40f0c #r..............
-  0x00008c70 81790828 06700100 001b1e0c 00e20e00 .y.(.p..........
-  0x00008c80 2372160e 14000000 16000000 00e40f0e #r..............
-  0x00008c90 2372170f 14000000 17000000 00e40f00 #r..............
-  0x00008ca0 2372200e 13000000 20000000 00c40f00 #r ..... .......
-  0x00008cb0 2372160f 15000080 16000000 00e20f08 #r..............
-  0x00008cc0 81791228 06b00100 001b1e0c 00220f00 .y.(........."..
-  0x00008cd0 2372170e 15000000 17000000 00c60f00 #r..............
-  0x00008ce0 81791428 06f00100 001b1e0c 00620f00 .y.(.........b..
-  0x00008cf0 25763005 00580000 03028e07 00c80f00 %v0..X..........
-  0x00008d00 2372220e 0c000000 07000000 00e44f0c #r"...........O.
-  0x00008d10 2372180f 0c000000 18000000 00e40f04 #r..............
-  0x00008d20 23720c0e 08000000 19000000 00e48f08 #r..............
-  0x00008d30 2372080f 08000000 00000000 00e40f04 #r..............
-  0x00008d40 2372000f 0d000080 22000000 00e40f04 #r......".......
-  0x00008d50 2372070f 09000080 0c000000 00c40f00 #r..............
-  0x00008d60 2372220e 09000000 08000000 00e40f04 #r".............
-  0x00008d70 2372080e 12000000 1d000000 00e40f0d #r..............
-  0x00008d80 2372040f 12000000 04000000 00e40f04 #r..............
-  0x00008d90 23720c0e 14000000 1b000000 00e40f0e #r..............
-  0x00008da0 23721e0f 14000000 1e000000 00e40f00 #r..............
-  0x00008db0 2372180e 0d000000 18000000 00c40f00 #r..............
-  0x00008dc0 2372190f 13000080 08000000 00e40f0c #r..............
-  0x00008dd0 2372140e 13000000 04000000 00e20f00 #r..............
-  0x00008de0 81790830 06000000 001b1e0c 00a20e00 .y.0............
-  0x00008df0 2372210f 15000080 0c000000 00c60f00 #r!.............
-  0x00008e00 81790428 06380000 001b1e0c 00a80e00 .y.(.8..........
-  0x00008e10 81790c28 06780000 001b1e0c 00e20e00 .y.(.x..........
-  0x00008e20 2372150e 15000000 1e000000 00c60f00 #r..............
-  0x00008e30 81790e28 06b80000 001b1e0c 00280f00 .y.(.........(..
-  0x00008e40 81791228 06f80000 001b1e0c 00620f00 .y.(.........b..
-  0x00008e50 23720304 09000000 1f000000 00e44f04 #r............O.
-  0x00008e60 23720604 08000000 06000000 00e40f00 #r..............
-  0x00008e70 23721a09 0c000000 1a000000 00e48f08 #r..............
-  0x00008e80 23720408 0c000000 02000000 00c40f00 #r..............
-  0x00008e90 23720305 08000000 03000000 00e40f04 #r..............
-  0x00008ea0 23720205 09000000 06010000 00e40f00 #r..............
-  0x00008eb0 23720508 0d000000 1a000000 00e40f0c #r..............
-  0x00008ec0 23720608 0e000000 1c000000 00e20f0d #r..............
-  0x00008ed0 81791a28 06380100 001b1e0c 00a20e00 .y.(.8..........
-  0x00008ee0 23722009 0e000000 20000000 00e40f04 #r ..... .......
-  0x00008ef0 23720e08 12000000 16000000 00e20f02 #r..............
-  0x00008f00 81791c28 06f80100 001b1e0c 00e20e00 .y.(............
-  0x00008f10 23720409 0d000080 04000000 00c40f00 #r..............
-  0x00008f20 23721209 12000000 17000000 00e20f04 #r..............
-  0x00008f30 81790c28 06b80100 001b1e0c 00280f00 .y.(.........(..
-  0x00008f40 81791628 06780100 001b1e0c 00620f00 .y.(.x.......b..
-  0x00008f50 23720609 0f000080 06000000 00e40f04 #r..............
-  0x00008f60 23720e09 13000080 0e000000 00e20f00 #r..............
-  0x00008f70 8679000a 02000000 061b100c 00e80f00 .y..............
-  0x00008f80 86790010 04000000 061b100c 00e20f00 .y..............
-  0x00008f90 23720008 1a000000 00000000 00c44f00 #r............O.
-  0x00008fa0 23721a09 1a000000 18000000 00e40f04 #r..............
-  0x00008fb0 23721509 1c000000 15000000 00e48f0c #r..............
-  0x00008fc0 23721c08 1c000000 21000000 00e40f04 #r......!.......
-  0x00008fd0 23721409 0c000000 14000000 00e40f09 #r..............
-  0x00008fe0 23720c08 0c000000 19000000 00e40f04 #r..............
-  0x00008ff0 23721808 16000000 07000000 00c40f02 #r..............
-  0x00009000 23722209 16000000 22000000 00e40f04 #r".....".......
-  0x00009010 23720708 0f000000 20000000 00e40f04 #r...... .......
-  0x00009020 23720f08 13000000 12000000 00e40f04 #r..............
-  0x00009030 23721308 1b000000 1a000000 00e40f0c #r..............
-  0x00009040 23721209 1b000080 00000000 00e40f00 #r..............
-  0x00009050 23721b08 17000000 22000000 00c40f00 #r......".......
-  0x00009060 23721a09 17000080 18000000 00e20f04 #r..............
-  0x00009070 8679002e 06000000 061b100c 00e20f00 .y..............
-  0x00009080 23721708 0d000000 14000000 00e40f0c #r..............
-  0x00009090 23721609 0d000080 0c000000 00e20f04 #r..............
-  0x000090a0 8679002c 0e000000 061b100c 00e20f00 .y.,............
-  0x000090b0 23721508 1d000000 15000000 00e40f08 #r..............
-  0x000090c0 23721409 1d000080 1c000000 00e20f00 #r..............
-  0x000090d0 8679002a 12000000 061b100c 00e80f00 .y.*............
-  0x000090e0 86790024 1a000000 061b100c 00e80f00 .y.$............
-  0x000090f0 86790026 16000000 061b100c 00e80f00 .y.&............
-  0x00009100 86790030 14000000 061b100c 00e20f00 .y.0............
-  0x00009110 4d790000 00000000 00008003 00ea0f00 My..............
-  0x00009120 47790000 f0ffffff ffff8303 00c00f00 Gy..............
-  0x00009130 18790000 00000000 00000000 00c00f00 .y..............
-  0x00009140 18790000 00000000 00000000 00c00f00 .y..............
-  0x00009150 18790000 00000000 00000000 00c00f00 .y..............
+  0x000077d0 00000000 00000000 00000000 00000000 ................
+  0x000077e0 00000000 00000000 00000000 00000000 ................
+  0x000077f0 00000000 00000000 00000000 00000000 ................
+  0x00007800 027a0100 000a0000 000f0000 00c40f00 .z..............
+  0x00007810 027a0400 005e0000 000f0000 00e20f00 .z...^..........
+  0x00007820 b97a0600 00460000 000a0000 00e20f00 .z...F..........
+  0x00007830 027a0500 005f0000 000f0000 00ca0f00 .z..._..........
+  0x00007840 81790304 06080000 00191e0c 00a80e00 .y..............
+  0x00007850 81790604 06000000 00191e0c 00e80e00 .y..............
+  0x00007860 81790804 06100000 00191e0c 00220f00 .y..........."..
+  0x00007870 b97a0400 00000000 00080000 00e40f00 .z..............
+  0x00007880 9978043f 01000000 04160108 00e20f00 .x.?............
+  0x00007890 19790b00 00000000 00250000 00280e00 .y.......%...(..
+  0x000078a0 19790a00 00000000 00210000 00240e00 .y.......!...$..
+  0x000078b0 247a0b0b 00000000 0a028e07 00ca1f00 $z..............
+  0x000078c0 1272020b 03000000 fffc8e07 00e44f0c .r............O.
+  0x000078d0 1272100b 06000000 fffc8e07 00e48f04 .r..............
+  0x000078e0 10720006 03000000 ffe0ff07 00e40f00 .r..............
+  0x000078f0 0c72000b 02000000 7052f003 00e40f04 .r......pR......
+  0x00007900 1272070b 00000000 fffc8e07 00e40f04 .r..............
+  0x00007910 0c72000b 10000000 70527000 00c40f00 .r......pRp.....
+  0x00007920 10720c06 08000000 ffe0ff07 00e40f09 .r..............
+  0x00007930 1272000b 08000000 fffc8e07 00e40f0c .r..............
+  0x00007940 0c72000b 07000000 70527000 00e40f00 .r......pRp.....
+  0x00007950 10720303 08000000 ffe0ff07 00e40f00 .r..............
+  0x00007960 1272080b 0c000000 fffc8e07 00e40f04 .r..............
+  0x00007970 0c72000b 00000000 70527000 00c40f00 .r......pRp.....
+  0x00007980 10720606 03000000 ffe0ff07 00e40f08 .r..............
+  0x00007990 1272040b 03000000 fffc8e07 00e40f04 .r..............
+  0x000079a0 0c72000b 08000000 70527000 00e40f04 .r......pRp.....
+  0x000079b0 1272050b 06000000 fffc8e07 00e40f04 .r..............
+  0x000079c0 0c72000b 04000000 70527000 00e40f00 .r......pRp.....
+  0x000079d0 197803ff 1f000000 0b140100 00c40f00 .x..............
+  0x000079e0 0c72000b 05000000 70527000 00c80f00 .r......pRp.....
+  0x000079f0 0c720010 02000000 70527000 00c80f00 .r......pRp.....
+  0x00007a00 0c720010 07000000 70527000 00c80f00 .r......pRp.....
+  0x00007a10 0c720010 00000000 70527000 00c80f00 .r......pRp.....
+  0x00007a20 0c720010 08000000 70527000 00c80f00 .r......pRp.....
+  0x00007a30 0c720010 04000000 70527000 00c80f00 .r......pRp.....
+  0x00007a40 0c720010 05000000 70527000 00c80f00 .r......pRp.....
+  0x00007a50 0c720002 07000000 70527000 00c80f00 .r......pRp.....
+  0x00007a60 0c720002 00000000 70527000 00c80f00 .r......pRp.....
+  0x00007a70 0c720002 08000000 70527000 00c80f00 .r......pRp.....
+  0x00007a80 0c720002 04000000 70527000 00c80f00 .r......pRp.....
+  0x00007a90 0c720002 05000000 70527000 00c80f00 .r......pRp.....
+  0x00007aa0 0c720007 00000000 70527000 00c80f00 .r......pRp.....
+  0x00007ab0 0c720007 08000000 70527000 00c80f00 .r......pRp.....
+  0x00007ac0 0c720007 04000000 70527000 00c80f00 .r......pRp.....
+  0x00007ad0 0c720007 05000000 70527000 00c80f00 .r......pRp.....
+  0x00007ae0 0c720000 08000000 70527000 00c80f00 .r......pRp.....
+  0x00007af0 0c720000 04000000 70527000 00c80f00 .r......pRp.....
+  0x00007b00 0c720000 05000000 70527200 00e40f08 .r......pRr.....
+  0x00007b10 0c7a000b 005c0000 7060f003 00e40f00 .z...\..p`......
+  0x00007b20 0c720008 04000000 7052f200 00e40f04 .r......pR......
+  0x00007b30 0c7a0003 005d0000 0061f003 00e40f00 .z...]...a......
+  0x00007b40 0c720008 05000000 7052f200 00e40f00 .r......pR......
+  0x00007b50 0c7c000a 04000000 7010700c 00c40f00 .|......p.p.....
+  0x00007b60 0c720004 05000000 7052f200 00c80f00 .r......pR......
+  0x00007b70 1c780000 00000000 70307000 00da0f00 .x......p0p.....
+  0x00007b80 4d890000 00000000 00008003 00ea0f00 M...............
+  0x00007b90 357403ff 08000000 ff010000 00e20f00 5t..............
+  0x00007ba0 027a2800 005a0000 000f0000 00e40f00 .z(..Z..........
+  0x00007bb0 027a2900 005b0000 000f0000 00ca0f00 .z)..[..........
+  0x00007bc0 81792428 06400000 001b1e0c 00a40e00 .y$(.@..........
+  0x00007bd0 25760a0b 00580000 03028e07 00e40f08 %v...X..........
+  0x00007be0 81792228 06800000 001b1e0c 00e80e00 .y"(............
+  0x00007bf0 81791e0a 06000000 001b1e0c 00a80e00 .y..............
+  0x00007c00 81791228 06c00000 001b1e0c 00280f00 .y.(.........(..
+  0x00007c10 81791a28 06000100 001b1e0c 00680f00 .y.(.........h..
+  0x00007c20 81790c28 06400100 001b1e0c 00280f00 .y.(.@.......(..
+  0x00007c30 81792628 06000000 001b1e0c 00280f00 .y&(.........(..
+  0x00007c40 81792028 06c00100 001b1e0c 00680f00 .y (.........h..
+  0x00007c50 81791628 06800100 001b1e0c 00620f00 .y.(.........b..
+  0x00007c60 25761010 00580000 03028e07 00c60f00 %v...X..........
+  0x00007c70 81791828 06080000 001b1e0c 00680f00 .y.(.........h..
+  0x00007c80 81790e10 06000000 001b1e0c 00680f00 .y...........h..
+  0x00007c90 81791428 06880000 001b1e0c 00680f00 .y.(.........h..
+  0x00007ca0 81791c28 06480000 001b1e0c 00620f00 .y.(.H.......b..
+  0x00007cb0 2072091f 25000000 00004000 00c44f00  r..%.....@...O.
+  0x00007cc0 2072061e 25000000 00004000 00e40f04  r..%.....@.....
+  0x00007cd0 2372091e 24000000 09080000 00e40f0c #r..$...........
+  0x00007ce0 2372061f 24000000 06000000 00e40f04 #r..$...........
+  0x00007cf0 2072251f 23000000 00004000 00e48f08  r%.#.....@.....
+  0x00007d00 2072241e 23000000 00004000 00e40f04  r$.#.....@.....
+  0x00007d10 2372231e 22000000 25080000 00c40f00 #r#."...%.......
+  0x00007d20 2372221f 22000000 24000000 00e40f04 #r"."...$.......
+  0x00007d30 2072251f 13000000 00004000 00e40f0d  r%.......@.....
+  0x00007d40 2072241e 13000000 00004000 00e40f04  r$.......@.....
+  0x00007d50 2372131e 12000000 25080000 00e40f08 #r......%.......
+  0x00007d60 2372121f 12000000 24000000 00e40f04 #r......$.......
+  0x00007d70 2072251f 1b000000 00004000 00c40f02  r%.......@.....
+  0x00007d80 2072241e 1b000000 00004000 00e40f04  r$.......@.....
+  0x00007d90 23721b1e 1a000000 25080000 00e40f0c #r......%.......
+  0x00007da0 23721a1f 1a000000 24000000 00e40f04 #r......$.......
+  0x00007db0 2072251f 0d000000 00004000 00e40f08  r%.......@.....
+  0x00007dc0 2072241e 0d000000 00004000 00e40f00  r$.......@.....
+  0x00007dd0 20722b27 1f000000 00004000 00c40f00  r+'......@.....
+  0x00007de0 20722a27 1e000000 00004000 00e40f00  r*'......@.....
+  0x00007df0 2372251e 0c000000 25080000 00e40f0c #r%.....%.......
+  0x00007e00 2372241f 0c000000 24000000 00e40f04 #r$.....$.......
+  0x00007e10 20720d1f 21000000 00004000 00e40f08  r..!.....@.....
+  0x00007e20 20720c1e 21000000 00004000 00e40f00  r..!.....@.....
+  0x00007e30 23722b26 1e000000 2b080000 00c40f00 #r+&....+.......
+  0x00007e40 23722a26 1f000000 2a000000 00e40f00 #r*&....*.......
+  0x00007e50 2072271f 17000000 00004000 00e40f0c  r'.......@.....
+  0x00007e60 2072261e 17000000 00004000 00e40f04  r&.......@.....
+  0x00007e70 2372211e 20000000 0d080000 00e40f0c #r!. ...........
+  0x00007e80 2372201f 20000000 0c000000 00e40f04 #r . ...........
+  0x00007e90 2372271e 16000000 27080000 00e20f08 #r'.....'.......
+  0x00007ea0 81790c28 06c80000 001b1e0c 00a20e00 .y.(............
+  0x00007eb0 2372261f 16000000 26000000 00c60f00 #r&.....&.......
+  0x00007ec0 81791628 06080100 001b1e0c 00e20e00 .y.(............
+  0x00007ed0 23721e18 0e000000 2b000000 00e40f0c #r......+.......
+  0x00007ee0 23722b18 0f000000 2a000000 00e40f08 #r+.....*.......
+  0x00007ef0 23722a19 0f000000 1e010000 00e40f04 #r*.............
+  0x00007f00 23722b19 0e000000 2b000000 00e20f00 #r+.....+.......
+  0x00007f10 81791e28 06880100 001b1e0c 00280f00 .y.(.........(..
+  0x00007f20 81791828 06480100 001b1e0c 00620f00 .y.(.H.......b..
+  0x00007f30 23722e0e 14000000 23000000 00c40f00 #r......#.......
+  0x00007f40 23722c0e 1c000000 09000000 00e40f08 #r,.............
+  0x00007f50 23721c0f 1c000000 06000000 00e40f04 #r..............
+  0x00007f60 2372220f 14000000 22000000 00e40f04 #r".....".......
+  0x00007f70 2372090f 15000080 2e000000 00e40f00 #r..............
+  0x00007f80 25762e02 00580000 03028e07 00c80f00 %v...X..........
+  0x00007f90 2372060f 1d000080 2c000000 00e40f0c #r......,.......
+  0x00007fa0 23722c0e 1d000000 1c000000 00e40f04 #r,.............
+  0x00007fb0 81791c28 06c80100 001b1e0c 00220f00 .y.(........."..
+  0x00007fc0 2372220e 15000000 22000000 00e40f04 #r".....".......
+  0x00007fd0 2372140e 0c000000 13000000 00e44f0c #r............O.
+  0x00007fe0 2372120f 0c000000 12000000 00e40f00 #r..............
+  0x00007ff0 23720c0e 16000000 1b000000 00c48f00 #r..............
+  0x00008000 2372160f 16000000 1a000000 00e40f04 #r..............
+  0x00008010 23721b0f 0d000080 14000000 00e40f0c #r..............
+  0x00008020 23721a0e 0d000000 12000000 00e20f00 #r..............
+  0x00008030 81791428 06500000 001b1e0c 00a20e00 .y.(.P..........
+  0x00008040 2372230f 17000080 0c000000 00c60f00 #r#.............
+  0x00008050 81790c28 06100000 001b1e0c 00e80e00 .y.(............
+  0x00008060 8179122e 06000000 001b1e0c 00e20e00 .y..............
+  0x00008070 2372020e 17000000 16000000 00e40f04 #r..............
+  0x00008080 2372160e 18000000 25000000 00e40f0e #r......%.......
+  0x00008090 2372240f 18000000 24000000 00e40f00 #r$.....$.......
+  0x000080a0 2372180e 1e000000 27000000 00c40f01 #r......'.......
+  0x000080b0 2372260f 1e000000 26000000 00e40f04 #r&.....&.......
+  0x000080c0 2372250f 19000080 16000000 00e40f0c #r%.............
+  0x000080d0 23721e0e 19000000 24000000 00e20f00 #r......$.......
+  0x000080e0 81791628 06900000 001b1e0c 00220f00 .y.(........."..
+  0x000080f0 2372270f 1f000080 18000000 00c60f00 #r'.............
+  0x00008100 81791828 06d00000 001b1e0c 00620f00 .y.(.........b..
+  0x00008110 2372240e 1c000000 21000000 00e40f0c #r$.....!.......
+  0x00008120 2372200f 1c000000 20000000 00e40f04 #r ..... .......
+  0x00008130 2372210f 1d000080 24000000 00e40f08 #r!.....$.......
+  0x00008140 23721d0e 1d000000 20000000 00e40f04 #r...... .......
+  0x00008150 23721f0e 1f000000 26000000 00e40f00 #r......&.......
+  0x00008160 81790e28 06500100 001b1e0c 00620f00 .y.(.P.......b..
+  0x00008170 23721c0c 12000000 2a000000 00c48f00 #r......*.......
+  0x00008180 23722b0c 13000000 2b000000 00e40f08 #r+.....+.......
+  0x00008190 23721c0d 13000000 1c010000 00e40f04 #r..............
+  0x000081a0 2372200d 12000000 2b000000 00e40f00 #r .....+.......
+  0x000081b0 81790c28 06100100 001b1e0c 00e20e00 .y.(............
+  0x000081c0 23720612 14000000 06000000 00e44f08 #r............O.
+  0x000081d0 23722413 14000000 2c000000 00e40f04 #r$.....,.......
+  0x000081e0 23720613 15000080 06000000 00c40f00 #r..............
+  0x000081f0 23722412 15000000 24000000 00e40f04 #r$.....$.......
+  0x00008200 81791428 06900100 001b1e0c 00a20e00 .y.(............
+  0x00008210 23722612 16000000 09000000 00e40f0d #r&.............
+  0x00008220 23722213 16000000 22000000 00e40f04 #r".....".......
+  0x00008230 23721612 18000000 1b000000 00e40f0a #r..............
+  0x00008240 23721813 18000000 1a000000 00e40f04 #r..............
+  0x00008250 81791a28 06d00100 001b1e0c 00220f00 .y.(........."..
+  0x00008260 23720913 17000080 26000000 00c40f00 #r......&.......
+  0x00008270 23721712 17000000 22000000 00e40f04 #r......".......
+  0x00008280 23722212 19000000 18000000 00e40f00 #r".............
+  0x00008290 23721e13 0e000000 1e000000 00e40f00 #r..............
+  0x000082a0 25762c07 00580000 03028e07 00c80f00 %v,..X..........
+  0x000082b0 23722612 0f000000 1e000000 00e40f04 #r&.............
+  0x000082c0 23721613 19000080 16000000 00e40f04 #r..............
+  0x000082d0 23721812 0c000000 23000000 00e48f0c #r......#.......
+  0x000082e0 23720213 0c000000 02000000 00e40f04 #r..............
+  0x000082f0 23720c12 0e000000 25000000 00e40f00 #r......%.......
+  0x00008300 23722313 0d000080 18000000 00c40f00 #r#.............
+  0x00008310 23720212 0d000000 02000000 00e40f04 #r..............
+  0x00008320 23720713 0f000080 0c000000 00e40f04 #r..............
+  0x00008330 23721812 14000000 27000000 00e24f08 #r......'.....O.
+  0x00008340 81790c28 06180000 001b1e0c 00a20e00 .y.(............
+  0x00008350 23721f13 14000000 1f000000 00c60f00 #r..............
+  0x00008360 81790e2c 06000000 001b1e0c 00a20e00 .y.,............
+  0x00008370 23722513 15000080 18000000 00e40f0c #r%.............
+  0x00008380 23722a12 15000000 1f000000 00e20f04 #r*.............
+  0x00008390 81791828 06980000 001b1e0c 00e80e00 .y.(............
+  0x000083a0 81791428 06580000 001b1e0c 00620f00 .y.(.X.......b..
+  0x000083b0 23721e12 1a000000 21000000 00e40f09 #r......!.......
+  0x000083c0 23721a13 1a000000 1d000000 00c40f00 #r..............
+  0x000083d0 23721d13 1b000080 1e000000 00e40f08 #r..............
+  0x000083e0 81791e28 06d80000 001b1e0c 00220f00 .y.(........."..
+  0x000083f0 23721b12 1b000000 1a000000 00e40f00 #r..............
+  0x00008400 23721c0c 0e000000 1c000000 00e44f0c #r............O.
+  0x00008410 2372200c 0f000000 20000000 00e40f08 #r ..... .......
+  0x00008420 23721a0d 0f000000 1c010000 00e40f04 #r..............
+  0x00008430 23721c0d 0e000000 20000000 00c40f00 #r...... .......
+  0x00008440 2372120e 18000000 09000000 00e28f04 #r..............
+  0x00008450 81790c28 06180100 001b1e0c 00a20e00 .y.(............
+  0x00008460 2372060e 14000000 06000000 00e40f0e #r..............
+  0x00008470 2372240f 14000000 24000000 00e40f04 #r$.....$.......
+  0x00008480 2372170f 18000000 17000000 00e40f04 #r..............
+  0x00008490 2372180f 19000080 12000000 00e40f04 #r..............
+  0x000084a0 2372060f 15000080 06000000 00e20f08 #r..............
+  0x000084b0 81791228 06580100 001b1e0c 00e20e00 .y.(.X..........
+  0x000084c0 2372090e 15000000 24000000 00c60f00 #r......$.......
+  0x000084d0 81791428 06980100 001b1e0c 00620f00 .y.(.........b..
+  0x000084e0 2372190e 19000000 17000000 00e40f04 #r..............
+  0x000084f0 2372200e 1e000000 16000000 00e40f0d #r .............
+  0x00008500 81791628 06d80100 001b1e0c 00220f00 .y.(........."..
+  0x00008510 2372220f 1e000000 22000000 00e40f04 #r".....".......
+  0x00008520 23721e0e 0c000000 23000000 00e44f08 #r......#.....O.
+  0x00008530 2372210f 0c000000 02000000 00c40f00 #r!.............
+  0x00008540 23720c0f 0d000080 1e000000 00e40f04 #r..............
+  0x00008550 2372020f 1f000080 20000000 00e40f04 #r...... .......
+  0x00008560 23721e0e 12000000 07000000 00e48f0c #r..............
+  0x00008570 2372240f 12000000 26000000 00e40f04 #r$.....&.......
+  0x00008580 2372120e 14000000 25000000 00e40f0a #r......%.......
+  0x00008590 2372140f 14000000 2a000000 00c40f00 #r......*.......
+  0x000085a0 25762a00 00580000 03028e07 00c80f00 %v*..X..........
+  0x000085b0 2372200e 1f000000 22000000 00e40f04 #r .....".......
+  0x000085c0 2372220e 0d000000 21000000 00e40f04 #r".....!.......
+  0x000085d0 2372070f 13000080 1e000000 00e40f0c #r..............
+  0x000085e0 2372240e 13000000 24000000 00e20f04 #r$.....$.......
+  0x000085f0 81791e28 06600000 001b1e0c 00a20e00 .y.(.`..........
+  0x00008600 23720d0f 15000080 12000000 00e40f08 #r..............
+  0x00008610 2372000e 15000000 14000000 00e20f04 #r..............
+  0x00008620 8179122a 06000000 001b1e0c 00e20e00 .y.*............
+  0x00008630 2372260e 16000000 1d000000 00c40f01 #r&.............
+  0x00008640 2372160f 16000000 1b000000 00e20f04 #r..............
+  0x00008650 81791428 06200000 001b1e0c 00e20e00 .y.(. ..........
+  0x00008660 23721b0f 17000080 26000000 00e40f08 #r......&.......
+  0x00008670 2372260e 17000000 16000000 00e40f00 #r&.............
+  0x00008680 81790e28 06a00000 001b1e0c 00280f00 .y.(.........(..
+  0x00008690 81791628 06e00000 001b1e0c 00620f00 .y.(.........b..
+  0x000086a0 23721a14 12000000 1a000000 00c48f00 #r..............
+  0x000086b0 23721c14 13000000 1c000000 00e40f08 #r..............
+  0x000086c0 23721412 1e000000 06000000 00e44f0c #r............O.
+  0x000086d0 23721e13 1e000000 09000000 00e40f00 #r..............
+  0x000086e0 23720915 12000000 1c000000 00e40f04 #r..............
+  0x000086f0 23720615 13000000 1a010000 00e40f00 #r..............
+  0x00008700 23721c12 0e000000 18000000 00c40f01 #r..............
+  0x00008710 23721a13 1f000080 14000000 00e40f0c #r..............
+  0x00008720 23720e13 0e000000 19000000 00e20f04 #r..............
+  0x00008730 81791428 06200100 001b1e0c 00a20e00 .y.(. ..........
+  0x00008740 23721f12 1f000000 1e000000 00e40f04 #r..............
+  0x00008750 23721e12 16000000 02000000 00e20f0a #r..............
+  0x00008760 81791828 06600100 001b1e0c 00e20e00 .y.(.`..........
+  0x00008770 23722013 16000000 20000000 00e40f04 #r ..... .......
+  0x00008780 23720213 0f000080 1c000000 00c40f00 #r..............
+  0x00008790 23721c12 0f000000 0e000000 00e40f04 #r..............
+  0x000087a0 81790e28 06a00100 001b1e0c 00220f00 .y.(........."..
+  0x000087b0 23721d13 17000080 1e000000 00e40f0c #r..............
+  0x000087c0 23721e12 17000000 20000000 00e40f04 #r...... .......
+  0x000087d0 81791628 06e00100 001b1e0c 00620f00 .y.(.........b..
+  0x000087e0 23720c12 14000000 0c000000 00e44f08 #r............O.
+  0x000087f0 23722213 14000000 22000000 00c40f00 #r".....".......
+  0x00008800 23721412 18000000 07000000 00e48f08 #r..............
+  0x00008810 23720713 15000080 0c000000 00e40f04 #r..............
+  0x00008820 23722013 18000000 24000000 00e40f00 #r .....$.......
+  0x00008830 25762408 00580000 03028e07 00c80f00 %v$..X..........
+  0x00008840 23720c12 0e000000 0d000000 00e40f0d #r..............
+  0x00008850 23720013 0e000000 00000000 00e40f04 #r..............
+  0x00008860 23721812 15000000 22000000 00e40f04 #r......".......
+  0x00008870 23720812 16000000 1b000000 00e40f0a #r..............
+  0x00008880 23722213 16000000 26000000 00e40f04 #r".....&.......
+  0x00008890 23722113 19000080 14000000 00c40f00 #r!.............
+  0x000088a0 23722012 19000000 20000000 00e20f04 #r ..... .......
+  0x000088b0 81791428 06680000 001b1e0c 00a20e00 .y.(.h..........
+  0x000088c0 23721913 0f000080 0c000000 00e40f0c #r..............
+  0x000088d0 23720012 0f000000 00000000 00e20f04 #r..............
+  0x000088e0 81790c24 06000000 001b1e0c 00a20e00 .y.$............
+  0x000088f0 23721b13 17000080 08000000 00e40f08 #r..............
+  0x00008900 23722212 17000000 22000000 00e20f00 #r".....".......
+  0x00008910 81790e28 06280000 001b1e0c 00e80e00 .y.(.(..........
+  0x00008920 81791228 06a80000 001b1e0c 00280f00 .y.(.........(..
+  0x00008930 81791628 06e80000 001b1e0c 00620f00 .y.(.........b..
+  0x00008940 2372230d 14000000 1f000000 00c44f00 #r#...........O.
+  0x00008950 2372090e 0d000000 09000000 00e48f04 #r..............
+  0x00008960 2372060e 0c000000 06000000 00e40f00 #r..............
+  0x00008970 2372020c 12000000 02000000 00e40f0d #r..............
+  0x00008980 23721c0d 12000000 1c000000 00e40f00 #r..............
+  0x00008990 23721f0f 0c000000 09000000 00e40f00 #r..............
+  0x000089a0 23721a0c 14000000 1a000000 00e20f00 #r..............
+  0x000089b0 81790828 06280100 001b1e0c 00a20e00 .y.(.(..........
+  0x000089c0 2372020d 13000080 02000000 00c40f00 #r..............
+  0x000089d0 23721c0c 13000000 1c000000 00e40f04 #r..............
+  0x000089e0 2372060f 0d000000 06010000 00e20f00 #r..............
+  0x000089f0 81791228 06680100 001b1e0c 00e20e00 .y.(.h..........
+  0x00008a00 2372140c 16000000 1d000000 00c60f02 #r..............
+  0x00008a10 81790e28 06a80100 001b1e0c 00220f00 .y.(........."..
+  0x00008a20 23721e0d 16000000 1e000000 00e40f04 #r..............
+  0x00008a30 23721a0d 15000080 1a000000 00e40f0c #r..............
+  0x00008a40 2372230c 15000000 23000000 00e40f04 #r#.....#.......
+  0x00008a50 2372160d 17000080 14000000 00e40f08 #r..............
+  0x00008a60 81791428 06e80100 001b1e0c 00620f00 .y.(.........b..
+  0x00008a70 2372170c 17000000 1e000000 00c40f00 #r..............
+  0x00008a80 25762604 00580000 03028e07 00c80f00 %v&..X..........
+  0x00008a90 23721e0c 08000000 07000000 00e44f0c #r............O.
+  0x00008aa0 2372180d 08000000 18000000 00e40f04 #r..............
+  0x00008ab0 2372080c 12000000 21000000 00e48f0c #r......!.......
+  0x00008ac0 2372200d 12000000 20000000 00e40f04 #r ..... .......
+  0x00008ad0 2372120c 0e000000 19000000 00e40f01 #r..............
+  0x00008ae0 2372070d 09000080 1e000000 00c40f00 #r..............
+  0x00008af0 23720e0d 0e000000 00000000 00e40f04 #r..............
+  0x00008b00 23721d0d 0f000080 12000000 00e40f04 #r..............
+  0x00008b10 2372120c 14000000 1b000000 00e40f0e #r..............
+  0x00008b20 23721e0d 14000000 22000000 00e40f04 #r......".......
+  0x00008b30 2372180c 09000000 18000000 00e40f00 #r..............
+  0x00008b40 2372190d 13000080 08000000 00c40f00 #r..............
+  0x00008b50 2372000c 13000000 20000000 00e20f04 #r...... .......
+  0x00008b60 81790828 06300000 001b1e0c 00a20e00 .y.(.0..........
+  0x00008b70 2372040c 0f000000 0e000000 00e40f04 #r..............
+  0x00008b80 23721b0d 15000080 12000000 00e20f08 #r..............
+  0x00008b90 81790e26 06000000 001b1e0c 00a20e00 .y.&............
+  0x00008ba0 23721e0c 15000000 1e000000 00c60f00 #r..............
+  0x00008bb0 81790c28 06700000 001b1e0c 00e80e00 .y.(.p..........
+  0x00008bc0 81791228 06b00000 001b1e0c 00280f00 .y.(.........(..
+  0x00008bd0 81791428 06f00000 001b1e0c 00620f00 .y.(.........b..
+  0x00008be0 23720608 0e000000 06000000 00e44f04 #r............O.
+  0x00008bf0 23721f08 0f000000 1f000000 00c40f00 #r..............
+  0x00008c00 23721a0e 0c000000 1a000000 00e48f0c #r..............
+  0x00008c10 2372230f 0c000000 23000000 00e40f04 #r#.....#.......
+  0x00008c20 2372080e 12000000 02000000 00e40f0d #r..............
+  0x00008c30 2372020f 0d000080 1a000000 00e40f0c #r..............
+  0x00008c40 2372200f 12000000 1c000000 00e40f00 #r .............
+  0x00008c50 23721a0e 0d000000 23000000 00c40f00 #r......#.......
+  0x00008c60 23720609 0f000000 06010000 00e20f04 #r..............
+  0x00008c70 81790c28 06300100 001b1e0c 00a20e00 .y.(.0..........
+  0x00008c80 23721f09 0e000000 1f000000 00e40f00 #r..............
+  0x00008c90 23721c0f 13000080 08000000 00e40f0c #r..............
+  0x00008ca0 81790828 06700100 001b1e0c 00e20e00 .y.(.p..........
+  0x00008cb0 2372160e 14000000 16000000 00e40f0e #r..............
+  0x00008cc0 2372170f 14000000 17000000 00e40f00 #r..............
+  0x00008cd0 2372200e 13000000 20000000 00c40f00 #r ..... .......
+  0x00008ce0 2372160f 15000080 16000000 00e20f08 #r..............
+  0x00008cf0 81791228 06b00100 001b1e0c 00220f00 .y.(........."..
+  0x00008d00 2372170e 15000000 17000000 00c60f00 #r..............
+  0x00008d10 81791428 06f00100 001b1e0c 00620f00 .y.(.........b..
+  0x00008d20 25763005 00580000 03028e07 00c80f00 %v0..X..........
+  0x00008d30 2372220e 0c000000 07000000 00e44f0c #r"...........O.
+  0x00008d40 2372180f 0c000000 18000000 00e40f04 #r..............
+  0x00008d50 23720c0e 08000000 19000000 00e48f08 #r..............
+  0x00008d60 2372080f 08000000 00000000 00e40f04 #r..............
+  0x00008d70 2372000f 0d000080 22000000 00e40f04 #r......".......
+  0x00008d80 2372070f 09000080 0c000000 00c40f00 #r..............
+  0x00008d90 2372220e 09000000 08000000 00e40f04 #r".............
+  0x00008da0 2372080e 12000000 1d000000 00e40f0d #r..............
+  0x00008db0 2372040f 12000000 04000000 00e40f04 #r..............
+  0x00008dc0 23720c0e 14000000 1b000000 00e40f0e #r..............
+  0x00008dd0 23721e0f 14000000 1e000000 00e40f00 #r..............
+  0x00008de0 2372180e 0d000000 18000000 00c40f00 #r..............
+  0x00008df0 2372190f 13000080 08000000 00e40f0c #r..............
+  0x00008e00 2372140e 13000000 04000000 00e20f00 #r..............
+  0x00008e10 81790830 06000000 001b1e0c 00a20e00 .y.0............
+  0x00008e20 2372210f 15000080 0c000000 00c60f00 #r!.............
+  0x00008e30 81790428 06380000 001b1e0c 00a80e00 .y.(.8..........
+  0x00008e40 81790c28 06780000 001b1e0c 00e20e00 .y.(.x..........
+  0x00008e50 2372150e 15000000 1e000000 00c60f00 #r..............
+  0x00008e60 81790e28 06b80000 001b1e0c 00280f00 .y.(.........(..
+  0x00008e70 81791228 06f80000 001b1e0c 00620f00 .y.(.........b..
+  0x00008e80 23720304 09000000 1f000000 00e44f04 #r............O.
+  0x00008e90 23720604 08000000 06000000 00e40f00 #r..............
+  0x00008ea0 23721a09 0c000000 1a000000 00e48f08 #r..............
+  0x00008eb0 23720408 0c000000 02000000 00c40f00 #r..............
+  0x00008ec0 23720305 08000000 03000000 00e40f04 #r..............
+  0x00008ed0 23720205 09000000 06010000 00e40f00 #r..............
+  0x00008ee0 23720508 0d000000 1a000000 00e40f0c #r..............
+  0x00008ef0 23720608 0e000000 1c000000 00e20f0d #r..............
+  0x00008f00 81791a28 06380100 001b1e0c 00a20e00 .y.(.8..........
+  0x00008f10 23722009 0e000000 20000000 00e40f04 #r ..... .......
+  0x00008f20 23720e08 12000000 16000000 00e20f02 #r..............
+  0x00008f30 81791c28 06f80100 001b1e0c 00e20e00 .y.(............
+  0x00008f40 23720409 0d000080 04000000 00c40f00 #r..............
+  0x00008f50 23721209 12000000 17000000 00e20f04 #r..............
+  0x00008f60 81790c28 06b80100 001b1e0c 00280f00 .y.(.........(..
+  0x00008f70 81791628 06780100 001b1e0c 00620f00 .y.(.x.......b..
+  0x00008f80 23720609 0f000080 06000000 00e40f04 #r..............
+  0x00008f90 23720e09 13000080 0e000000 00e20f00 #r..............
+  0x00008fa0 8679000a 02000000 061b100c 00e80f00 .y..............
+  0x00008fb0 86790010 04000000 061b100c 00e20f00 .y..............
+  0x00008fc0 23720008 1a000000 00000000 00c44f00 #r............O.
+  0x00008fd0 23721a09 1a000000 18000000 00e40f04 #r..............
+  0x00008fe0 23721509 1c000000 15000000 00e48f0c #r..............
+  0x00008ff0 23721c08 1c000000 21000000 00e40f04 #r......!.......
+  0x00009000 23721409 0c000000 14000000 00e40f09 #r..............
+  0x00009010 23720c08 0c000000 19000000 00e40f04 #r..............
+  0x00009020 23721808 16000000 07000000 00c40f02 #r..............
+  0x00009030 23722209 16000000 22000000 00e40f04 #r".....".......
+  0x00009040 23720708 0f000000 20000000 00e40f04 #r...... .......
+  0x00009050 23720f08 13000000 12000000 00e40f04 #r..............
+  0x00009060 23721308 1b000000 1a000000 00e40f0c #r..............
+  0x00009070 23721209 1b000080 00000000 00e40f00 #r..............
+  0x00009080 23721b08 17000000 22000000 00c40f00 #r......".......
+  0x00009090 23721a09 17000080 18000000 00e20f04 #r..............
+  0x000090a0 8679002e 06000000 061b100c 00e20f00 .y..............
+  0x000090b0 23721708 0d000000 14000000 00e40f0c #r..............
+  0x000090c0 23721609 0d000080 0c000000 00e20f04 #r..............
+  0x000090d0 8679002c 0e000000 061b100c 00e20f00 .y.,............
+  0x000090e0 23721508 1d000000 15000000 00e40f08 #r..............
+  0x000090f0 23721409 1d000080 1c000000 00e20f00 #r..............
+  0x00009100 8679002a 12000000 061b100c 00e80f00 .y.*............
+  0x00009110 86790024 1a000000 061b100c 00e80f00 .y.$............
+  0x00009120 86790026 16000000 061b100c 00e80f00 .y.&............
+  0x00009130 86790030 14000000 061b100c 00e20f00 .y.0............
+  0x00009140 4d790000 00000000 00008003 00ea0f00 My..............
+  0x00009150 47790000 f0ffffff ffff8303 00c00f00 Gy..............
   0x00009160 18790000 00000000 00000000 00c00f00 .y..............
   0x00009170 18790000 00000000 00000000 00c00f00 .y..............
   0x00009180 18790000 00000000 00000000 00c00f00 .y..............
   0x00009190 18790000 00000000 00000000 00c00f00 .y..............
   0x000091a0 18790000 00000000 00000000 00c00f00 .y..............
   0x000091b0 18790000 00000000 00000000 00c00f00 .y..............
   0x000091c0 18790000 00000000 00000000 00c00f00 .y..............
-  0x000091d0 027a0100 000a0000 000f0000 00c40f00 .z..............
-  0x000091e0 027a0200 005e0000 000f0000 00e20f00 .z...^..........
-  0x000091f0 b97a0600 00460000 000a0000 00e20f00 .z...F..........
-  0x00009200 027a0300 005f0000 000f0000 00ca0f00 .z..._..........
-  0x00009210 81790402 06080000 00191e0c 00a80000 .y..............
-  0x00009220 81790502 06000000 00191e0c 00e20000 .y..............
-  0x00009230 b97a0400 00000000 00080000 00e40f00 .z..............
-  0x00009240 9978043f 01000000 04160108 00e20f00 .x.?............
-  0x00009250 19790000 00000000 00250000 00680e00 .y.......%...h..
-  0x00009260 19790900 00000000 00210000 00640e00 .y.......!...d..
-  0x00009270 247a0000 00000000 09028e07 00ca2f00 $z............/.
-  0x00009280 197803ff 1f000000 00140100 00e41f00 .x..............
-  0x00009290 12720700 04000000 fffc8e07 00e44f0c .r............O.
-  0x000092a0 10720b05 04000000 ffe0ff07 00e48f00 .r..............
-  0x000092b0 12720500 05000000 fffc8e07 00e40f04 .r..............
-  0x000092c0 0c720000 07000000 7052f003 00e40f04 .r......pR......
-  0x000092d0 12720600 0b000000 fffc8e07 00c40f00 .r..............
-  0x000092e0 0c720000 05000000 70527000 00c80f00 .r......pRp.....
-  0x000092f0 0c720000 06000000 70527200 00e40f0c .r......pRr.....
-  0x00009300 0c7a0000 005c0000 7060f003 00e40f00 .z...\..p`......
-  0x00009310 0c720005 07000000 7052f200 00e40f00 .r......pR......
-  0x00009320 0c7a0003 005d0000 0061f003 00e40f00 .z...]...a......
-  0x00009330 0c720005 06000000 7052f200 00e40f00 .r......pR......
-  0x00009340 0c7c0009 04000000 7010700c 00c40f00 .|......p.p.....
-  0x00009350 0c720007 06000000 7052f200 00c80f00 .r......pR......
-  0x00009360 1c780000 00000000 70307000 00da0f00 .x......p0p.....
-  0x00009370 4d890000 00000000 00008003 00ea0f00 M...............
-  0x00009380 117a0800 00580000 ff188007 00e40f04 .z...X..........
-  0x00009390 027a0e00 005a0000 000f0000 00e40f00 .z...Z..........
-  0x000093a0 027a0f00 005b0000 000f0000 00e40f00 .z...[..........
-  0x000093b0 117a0900 00590000 031c0f00 00c60f00 .z...Y..........
-  0x000093c0 8179020e 06000000 001b1e0c 00a80e00 .y..............
-  0x000093d0 81791408 06000000 001b1e0c 00a80e00 .y..............
-  0x000093e0 8179100e 06200000 001b1e0c 00e80e00 .y... ..........
-  0x000093f0 81790a0e 06400000 001b1e0c 00280f00 .y...@.......(..
-  0x00009400 8179160e 06600000 001b1e0c 00620f00 .y...`.......b..
-  0x00009410 357400ff 08000000 ff010000 00c60f00 5t..............
-  0x00009420 8179120e 06280000 001b1e0c 006e0f00 .y...(.......n..
-  0x00009430 25760c05 00580000 00028e07 00c80f00 %v...X..........
-  0x00009440 20721903 15000000 00004000 00e44f04  r........@...O.
-  0x00009450 20720403 14000000 00004000 00e40f00  r........@.....
-  0x00009460 20720315 11000000 00004000 00e48f0c  r........@.....
-  0x00009470 20720514 11000000 00004000 00e40f04  r........@.....
-  0x00009480 20721115 0b000000 00004000 00e40f09  r........@.....
-  0x00009490 20721814 0b000000 00004000 00c40f00  r........@.....
-  0x000094a0 23721902 14000000 19080000 00e40f04 #r..............
-  0x000094b0 23720402 15000000 04000000 00e40f00 #r..............
-  0x000094c0 23720214 10000000 03080000 00e40f0c #r..............
-  0x000094d0 23720515 10000000 05000000 00e40f04 #r..............
-  0x000094e0 23720314 0a000000 11080000 00e40f08 #r..............
-  0x000094f0 23721815 0a000000 18000000 00e20f04 #r..............
-  0x00009500 8179100c 06000000 001b1e0c 00a20e00 .y..............
-  0x00009510 20721b15 17000000 00004000 00c60f02  r........@.....
-  0x00009520 81790a0e 06080000 001b1e0c 00a20e00 .y..............
-  0x00009530 20721a14 17000000 00004000 00e40f04  r........@.....
-  0x00009540 23721b14 16000000 1b080000 00e40f08 #r..............
-  0x00009550 23721a15 16000000 1a000000 00e40f00 #r..............
-  0x00009560 8179140e 06480000 001b1e0c 00e80e00 .y...H..........
-  0x00009570 8179160e 06680000 001b1e0c 00220f00 .y...h......."..
-  0x00009580 23721c0a 10000000 19000000 00c44f00 #r............O.
-  0x00009590 2372040a 11000000 04000000 00e40f08 #r..............
-  0x000095a0 23720a10 12000000 02000000 00e40f00 #r..............
-  0x000095b0 2372020b 11000000 1c010000 00e40f04 #r..............
-  0x000095c0 23720b0b 10000000 04000000 00e40f00 #r..............
-  0x000095d0 23720411 13000080 0a000000 00e40f04 #r..............
-  0x000095e0 23720511 12000000 05000000 00c40f00 #r..............
-  0x000095f0 23720a10 14000000 03000000 00e48f0c #r..............
-  0x00009600 23721310 13000000 05000000 00e40f00 #r..............
-  0x00009610 23720311 15000080 0a000000 00e40f04 #r..............
-  0x00009620 23720511 14000000 18000000 00e40f00 #r..............
-  0x00009630 25761c07 00580000 00028e07 00c80f00 %v...X..........
-  0x00009640 23721210 16000000 1b000000 00e20f0d #r..............
-  0x00009650 8179181c 06000000 001b1e0c 00a20e00 .y..............
-  0x00009660 23720a11 16000000 1a000000 00e40f04 #r..............
-  0x00009670 23720510 15000000 05000000 00e20f04 #r..............
-  0x00009680 81791a0e 06300000 001b1e0c 00a20e00 .y...0..........
-  0x00009690 23720711 17000080 12000000 00e40f08 #r..............
-  0x000096a0 23720a10 17000000 0a000000 00e20f00 #r..............
-  0x000096b0 8179140e 06100000 001b1e0c 00e80e00 .y..............
-  0x000096c0 8179100e 06500000 001b1e0c 00280f00 .y...P.......(..
-  0x000096d0 8179160e 06700000 001b1e0c 00620f00 .y...p.......b..
-  0x000096e0 25761e06 00580000 00028e07 00c80f00 %v...X..........
-  0x000096f0 23720418 1a000000 04000000 00e44f08 #r............O.
-  0x00009700 23721319 1a000000 13000000 00e40f04 #r..............
-  0x00009710 23720214 18000000 02000000 00e48f04 #r..............
-  0x00009720 23720b14 19000000 0b000000 00e40f00 #r..............
-  0x00009730 23721218 10000000 03000000 00e40f09 #r..............
-  0x00009740 23720519 10000000 05000000 00c40f00 #r..............
-  0x00009750 23720018 16000000 07000000 00e40f0e #r..............
-  0x00009760 23721619 16000000 0a000000 00e20f04 #r..............
-  0x00009770 8179060e 06180000 001b1e0c 00a20e00 .y..............
-  0x00009780 23720319 11000080 12000000 00e40f00 #r..............
-  0x00009790 23720215 19000000 02010000 00e40f04 #r..............
-  0x000097a0 23721118 11000000 05000000 00e40f00 #r..............
-  0x000097b0 23721515 18000000 0b000000 00c40f00 #r..............
-  0x000097c0 23720419 1b000080 04000000 00e20f04 #r..............
-  0x000097d0 81790a1e 06000000 001b1e0c 00a20e00 .y..............
-  0x000097e0 23720519 17000080 00000000 00e40f00 #r..............
-  0x000097f0 23721b18 1b000000 13000000 00e40f04 #r..............
-  0x00009800 23720018 17000000 16000000 00e20f00 #r..............
-  0x00009810 8179120e 06380000 001b1e0c 00e80e00 .y...8..........
-  0x00009820 8179160e 06580000 001b1e0c 00280f00 .y...X.......(..
-  0x00009830 8179180e 06780000 001b1e0c 00620f00 .y...x.......b..
-  0x00009840 23721506 0b000000 15000000 00c44f00 #r............O.
-  0x00009850 23720206 0a000000 02000000 00e40f00 #r..............
-  0x00009860 23721b0b 12000000 1b000000 00e48f0c #r..............
-  0x00009870 2372040a 12000000 04000000 00e40f04 #r..............
-  0x00009880 2372110b 16000000 11000000 00e40f0d #r..............
-  0x00009890 2372160a 16000000 03000000 00e40f00 #r..............
-  0x000098a0 2372000b 18000000 00000000 00c40f02 #r..............
-  0x000098b0 2372180a 18000000 05000000 00e40f04 #r..............
-  0x000098c0 23721507 0a000000 15000000 00e40f04 #r..............
-  0x000098d0 23721407 0b000000 02010000 00e40f00 #r..............
-  0x000098e0 2372070a 13000000 1b000000 00e40f0c #r..............
-  0x000098f0 2372060b 13000080 04000000 00e40f00 #r..............
-  0x00009900 2372110a 17000000 11000000 00c40f00 #r..............
-  0x00009910 2372100b 17000080 16000000 00e40f04 #r..............
-  0x00009920 2372030a 19000000 00000000 00e40f08 #r..............
-  0x00009930 2372020b 19000080 18000000 00e20f00 #r..............
-  0x00009940 86790008 14000000 061b100c 00e80f00 .y..............
-  0x00009950 8679000c 06000000 061b100c 00e80f00 .y..............
-  0x00009960 8679001c 10000000 061b100c 00e80f00 .y..............
-  0x00009970 8679001e 02000000 061b100c 00e20f00 .y..............
-  0x00009980 4d790000 00000000 00008003 00ea0f00 My..............
-  0x00009990 47790000 f0ffffff ffff8303 00c00f00 Gy..............
-  0x000099a0 18790000 00000000 00000000 00c00f00 .y..............
-  0x000099b0 18790000 00000000 00000000 00c00f00 .y..............
-  0x000099c0 18790000 00000000 00000000 00c00f00 .y..............
+  0x000091d0 18790000 00000000 00000000 00c00f00 .y..............
+  0x000091e0 18790000 00000000 00000000 00c00f00 .y..............
+  0x000091f0 18790000 00000000 00000000 00c00f00 .y..............
+  0x00009200 027a0100 000a0000 000f0000 00c40f00 .z..............
+  0x00009210 027a0200 005e0000 000f0000 00e20f00 .z...^..........
+  0x00009220 b97a0600 00460000 000a0000 00e20f00 .z...F..........
+  0x00009230 027a0300 005f0000 000f0000 00ca0f00 .z..._..........
+  0x00009240 81790402 06080000 00191e0c 00a80000 .y..............
+  0x00009250 81790502 06000000 00191e0c 00e20000 .y..............
+  0x00009260 b97a0400 00000000 00080000 00e40f00 .z..............
+  0x00009270 9978043f 01000000 04160108 00e20f00 .x.?............
+  0x00009280 19790000 00000000 00250000 00680e00 .y.......%...h..
+  0x00009290 19790900 00000000 00210000 00640e00 .y.......!...d..
+  0x000092a0 247a0000 00000000 09028e07 00ca2f00 $z............/.
+  0x000092b0 197803ff 1f000000 00140100 00e41f00 .x..............
+  0x000092c0 12720700 04000000 fffc8e07 00e44f0c .r............O.
+  0x000092d0 10720b05 04000000 ffe0ff07 00e48f00 .r..............
+  0x000092e0 12720500 05000000 fffc8e07 00e40f04 .r..............
+  0x000092f0 0c720000 07000000 7052f003 00e40f04 .r......pR......
+  0x00009300 12720600 0b000000 fffc8e07 00c40f00 .r..............
+  0x00009310 0c720000 05000000 70527000 00c80f00 .r......pRp.....
+  0x00009320 0c720000 06000000 70527200 00e40f0c .r......pRr.....
+  0x00009330 0c7a0000 005c0000 7060f003 00e40f00 .z...\..p`......
+  0x00009340 0c720005 07000000 7052f200 00e40f00 .r......pR......
+  0x00009350 0c7a0003 005d0000 0061f003 00e40f00 .z...]...a......
+  0x00009360 0c720005 06000000 7052f200 00e40f00 .r......pR......
+  0x00009370 0c7c0009 04000000 7010700c 00c40f00 .|......p.p.....
+  0x00009380 0c720007 06000000 7052f200 00c80f00 .r......pR......
+  0x00009390 1c780000 00000000 70307000 00da0f00 .x......p0p.....
+  0x000093a0 4d890000 00000000 00008003 00ea0f00 M...............
+  0x000093b0 117a0800 00580000 ff188007 00e40f04 .z...X..........
+  0x000093c0 027a0e00 005a0000 000f0000 00e40f00 .z...Z..........
+  0x000093d0 027a0f00 005b0000 000f0000 00e40f00 .z...[..........
+  0x000093e0 117a0900 00590000 031c0f00 00c60f00 .z...Y..........
+  0x000093f0 8179020e 06000000 001b1e0c 00a80e00 .y..............
+  0x00009400 81791408 06000000 001b1e0c 00a80e00 .y..............
+  0x00009410 8179100e 06200000 001b1e0c 00e80e00 .y... ..........
+  0x00009420 81790a0e 06400000 001b1e0c 00280f00 .y...@.......(..
+  0x00009430 8179160e 06600000 001b1e0c 00620f00 .y...`.......b..
+  0x00009440 357400ff 08000000 ff010000 00c60f00 5t..............
+  0x00009450 8179120e 06280000 001b1e0c 006e0f00 .y...(.......n..
+  0x00009460 25760c05 00580000 00028e07 00c80f00 %v...X..........
+  0x00009470 20721903 15000000 00004000 00e44f04  r........@...O.
+  0x00009480 20720403 14000000 00004000 00e40f00  r........@.....
+  0x00009490 20720315 11000000 00004000 00e48f0c  r........@.....
+  0x000094a0 20720514 11000000 00004000 00e40f04  r........@.....
+  0x000094b0 20721115 0b000000 00004000 00e40f09  r........@.....
+  0x000094c0 20721814 0b000000 00004000 00c40f00  r........@.....
+  0x000094d0 23721902 14000000 19080000 00e40f04 #r..............
+  0x000094e0 23720402 15000000 04000000 00e40f00 #r..............
+  0x000094f0 23720214 10000000 03080000 00e40f0c #r..............
+  0x00009500 23720515 10000000 05000000 00e40f04 #r..............
+  0x00009510 23720314 0a000000 11080000 00e40f08 #r..............
+  0x00009520 23721815 0a000000 18000000 00e20f04 #r..............
+  0x00009530 8179100c 06000000 001b1e0c 00a20e00 .y..............
+  0x00009540 20721b15 17000000 00004000 00c60f02  r........@.....
+  0x00009550 81790a0e 06080000 001b1e0c 00a20e00 .y..............
+  0x00009560 20721a14 17000000 00004000 00e40f04  r........@.....
+  0x00009570 23721b14 16000000 1b080000 00e40f08 #r..............
+  0x00009580 23721a15 16000000 1a000000 00e40f00 #r..............
+  0x00009590 8179140e 06480000 001b1e0c 00e80e00 .y...H..........
+  0x000095a0 8179160e 06680000 001b1e0c 00220f00 .y...h......."..
+  0x000095b0 23721c0a 10000000 19000000 00c44f00 #r............O.
+  0x000095c0 2372040a 11000000 04000000 00e40f08 #r..............
+  0x000095d0 23720a10 12000000 02000000 00e40f00 #r..............
+  0x000095e0 2372020b 11000000 1c010000 00e40f04 #r..............
+  0x000095f0 23720b0b 10000000 04000000 00e40f00 #r..............
+  0x00009600 23720411 13000080 0a000000 00e40f04 #r..............
+  0x00009610 23720511 12000000 05000000 00c40f00 #r..............
+  0x00009620 23720a10 14000000 03000000 00e48f0c #r..............
+  0x00009630 23721310 13000000 05000000 00e40f00 #r..............
+  0x00009640 23720311 15000080 0a000000 00e40f04 #r..............
+  0x00009650 23720511 14000000 18000000 00e40f00 #r..............
+  0x00009660 25761c07 00580000 00028e07 00c80f00 %v...X..........
+  0x00009670 23721210 16000000 1b000000 00e20f0d #r..............
+  0x00009680 8179181c 06000000 001b1e0c 00a20e00 .y..............
+  0x00009690 23720a11 16000000 1a000000 00e40f04 #r..............
+  0x000096a0 23720510 15000000 05000000 00e20f04 #r..............
+  0x000096b0 81791a0e 06300000 001b1e0c 00a20e00 .y...0..........
+  0x000096c0 23720711 17000080 12000000 00e40f08 #r..............
+  0x000096d0 23720a10 17000000 0a000000 00e20f00 #r..............
+  0x000096e0 8179140e 06100000 001b1e0c 00e80e00 .y..............
+  0x000096f0 8179100e 06500000 001b1e0c 00280f00 .y...P.......(..
+  0x00009700 8179160e 06700000 001b1e0c 00620f00 .y...p.......b..
+  0x00009710 25761e06 00580000 00028e07 00c80f00 %v...X..........
+  0x00009720 23720418 1a000000 04000000 00e44f08 #r............O.
+  0x00009730 23721319 1a000000 13000000 00e40f04 #r..............
+  0x00009740 23720214 18000000 02000000 00e48f04 #r..............
+  0x00009750 23720b14 19000000 0b000000 00e40f00 #r..............
+  0x00009760 23721218 10000000 03000000 00e40f09 #r..............
+  0x00009770 23720519 10000000 05000000 00c40f00 #r..............
+  0x00009780 23720018 16000000 07000000 00e40f0e #r..............
+  0x00009790 23721619 16000000 0a000000 00e20f04 #r..............
+  0x000097a0 8179060e 06180000 001b1e0c 00a20e00 .y..............
+  0x000097b0 23720319 11000080 12000000 00e40f00 #r..............
+  0x000097c0 23720215 19000000 02010000 00e40f04 #r..............
+  0x000097d0 23721118 11000000 05000000 00e40f00 #r..............
+  0x000097e0 23721515 18000000 0b000000 00c40f00 #r..............
+  0x000097f0 23720419 1b000080 04000000 00e20f04 #r..............
+  0x00009800 81790a1e 06000000 001b1e0c 00a20e00 .y..............
+  0x00009810 23720519 17000080 00000000 00e40f00 #r..............
+  0x00009820 23721b18 1b000000 13000000 00e40f04 #r..............
+  0x00009830 23720018 17000000 16000000 00e20f00 #r..............
+  0x00009840 8179120e 06380000 001b1e0c 00e80e00 .y...8..........
+  0x00009850 8179160e 06580000 001b1e0c 00280f00 .y...X.......(..
+  0x00009860 8179180e 06780000 001b1e0c 00620f00 .y...x.......b..
+  0x00009870 23721506 0b000000 15000000 00c44f00 #r............O.
+  0x00009880 23720206 0a000000 02000000 00e40f00 #r..............
+  0x00009890 23721b0b 12000000 1b000000 00e48f0c #r..............
+  0x000098a0 2372040a 12000000 04000000 00e40f04 #r..............
+  0x000098b0 2372110b 16000000 11000000 00e40f0d #r..............
+  0x000098c0 2372160a 16000000 03000000 00e40f00 #r..............
+  0x000098d0 2372000b 18000000 00000000 00c40f02 #r..............
+  0x000098e0 2372180a 18000000 05000000 00e40f04 #r..............
+  0x000098f0 23721507 0a000000 15000000 00e40f04 #r..............
+  0x00009900 23721407 0b000000 02010000 00e40f00 #r..............
+  0x00009910 2372070a 13000000 1b000000 00e40f0c #r..............
+  0x00009920 2372060b 13000080 04000000 00e40f00 #r..............
+  0x00009930 2372110a 17000000 11000000 00c40f00 #r..............
+  0x00009940 2372100b 17000080 16000000 00e40f04 #r..............
+  0x00009950 2372030a 19000000 00000000 00e40f08 #r..............
+  0x00009960 2372020b 19000080 18000000 00e20f00 #r..............
+  0x00009970 86790008 14000000 061b100c 00e80f00 .y..............
+  0x00009980 8679000c 06000000 061b100c 00e80f00 .y..............
+  0x00009990 8679001c 10000000 061b100c 00e80f00 .y..............
+  0x000099a0 8679001e 02000000 061b100c 00e20f00 .y..............
+  0x000099b0 4d790000 00000000 00008003 00ea0f00 My..............
+  0x000099c0 47790000 f0ffffff ffff8303 00c00f00 Gy..............
   0x000099d0 18790000 00000000 00000000 00c00f00 .y..............
   0x000099e0 18790000 00000000 00000000 00c00f00 .y..............
   0x000099f0 18790000 00000000 00000000 00c00f00 .y..............
   0x00009a00 18790000 00000000 00000000 00c00f00 .y..............
   0x00009a10 18790000 00000000 00000000 00c00f00 .y..............
   0x00009a20 18790000 00000000 00000000 00c00f00 .y..............
   0x00009a30 18790000 00000000 00000000 00c00f00 .y..............
   0x00009a40 18790000 00000000 00000000 00c00f00 .y..............
-  0x00009a50 027a0100 000a0000 000f0000 00c40f00 .z..............
-  0x00009a60 027a0300 005f0000 000f0000 00e20f00 .z..._..........
-  0x00009a70 b97a0600 00460000 000a0000 00e20f00 .z...F..........
-  0x00009a80 027a0200 005e0000 000f0000 00ca0f00 .z...^..........
-  0x00009a90 81790302 06000000 00191e0c 00a20e00 .y..............
-  0x00009aa0 b97a0400 00000000 00080000 00e40f00 .z..............
-  0x00009ab0 9978043f 01000000 04160108 00e20f00 .x.?............
-  0x00009ac0 19790000 00000000 00250000 00280e00 .y.......%...(..
-  0x00009ad0 19790700 00000000 00210000 00240e00 .y.......!...$..
-  0x00009ae0 247a0000 00000000 07028e07 00ca1f00 $z..............
-  0x00009af0 0c7a0000 005c0000 7060f003 00e40f00 .z...\..p`......
-  0x00009b00 197809ff 1f000000 00140100 00c80f00 .x..............
-  0x00009b10 0c7a0009 005d0000 0061f003 00c80f00 .z...]...a......
-  0x00009b20 0c7c0007 04000000 70647008 00e40f00 .|......pdp.....
-  0x00009b30 12720500 03000000 fffc8e07 00c84f00 .r............O.
-  0x00009b40 0c720000 05000000 70267000 00da0f00 .r......p&p.....
-  0x00009b50 4d090000 00000000 00008003 00ea0f00 M...............
-  0x00009b60 117a0200 00580000 ff188007 00e20f04 .z...X..........
-  0x00009b70 357404ff 08000000 ff010000 00e20f00 5t..............
-  0x00009b80 027a1200 005a0000 000f0000 00e40f00 .z...Z..........
-  0x00009b90 027a1300 005b0000 000f0000 00e40f00 .z...[..........
-  0x00009ba0 117a0300 00590000 091c0f00 00c60f00 .z...Y..........
-  0x00009bb0 81791012 06000000 001b1e0c 00a80e00 .y..............
-  0x00009bc0 81790e02 06000000 001b1e0c 00a20e00 .y..............
-  0x00009bd0 25760405 00580000 04028e07 00c60f00 %v...X..........
-  0x00009be0 81790c12 06100000 001b1e0c 00e80e00 .y..............
-  0x00009bf0 81790812 06080000 001b1e0c 00280f00 .y...........(..
-  0x00009c00 81790604 06000000 001b1e0c 00280f00 .y...........(..
-  0x00009c10 81790a12 06180000 001b1e0c 00620f00 .y...........b..
-  0x00009c20 20720010 0f000000 00004000 00c44f00  r........@...O.
-  0x00009c30 20721511 0f000000 00004000 00e40f00  r........@.....
-  0x00009c40 2072140e 0d000000 00004000 00e48f08  r........@.....
-  0x00009c50 20720d0f 0d000000 00004000 00e40f00  r........@.....
-  0x00009c60 23720011 0e000000 00000000 00e40f08 #r..............
-  0x00009c70 23721510 0e000000 15080000 00e40f00 #r..............
-  0x00009c80 2372140f 0c000000 14000000 00c40f00 #r..............
-  0x00009c90 23720d0e 0c000000 0d080000 00e40f00 #r..............
-  0x00009ca0 23720c09 06000000 00000000 00e40f09 #r..............
-  0x00009cb0 23720008 06000000 15000000 00e40f00 #r..............
-  0x00009cc0 23721407 0a000000 14000000 00e40f0a #r..............
-  0x00009cd0 23720a06 0a000000 0d000000 00e40f00 #r..............
-  0x00009ce0 23720d08 07000000 0c000000 00c40f00 #r..............
-  0x00009cf0 23720c09 07000000 00010000 00e40f00 #r..............
-  0x00009d00 23720906 0b000000 14000000 00e40f08 #r..............
-  0x00009d10 23720807 0b000080 0a000000 00e20f00 #r..............
-  0x00009d20 86790002 0c000000 061b100c 00e80f00 .y..............
-  0x00009d30 86790004 08000000 061b100c 00e20f00 .y..............
-  0x00009d40 4d790000 00000000 00008003 00ea0f00 My..............
-  0x00009d50 47790000 f0ffffff ffff8303 00c00f00 Gy..............
-  0x00009d60 18790000 00000000 00000000 00c00f00 .y..............
-  0x00009d70 18790000 00000000 00000000 00c00f00 .y..............
-  0x00009d80 18790000 00000000 00000000 00c00f00 .y..............
+  0x00009a50 18790000 00000000 00000000 00c00f00 .y..............
+  0x00009a60 18790000 00000000 00000000 00c00f00 .y..............
+  0x00009a70 18790000 00000000 00000000 00c00f00 .y..............
+  0x00009a80 027a0100 000a0000 000f0000 00c40f00 .z..............
+  0x00009a90 027a0300 005f0000 000f0000 00e20f00 .z..._..........
+  0x00009aa0 b97a0600 00460000 000a0000 00e20f00 .z...F..........
+  0x00009ab0 027a0200 005e0000 000f0000 00ca0f00 .z...^..........
+  0x00009ac0 81790302 06000000 00191e0c 00a20e00 .y..............
+  0x00009ad0 b97a0400 00000000 00080000 00e40f00 .z..............
+  0x00009ae0 9978043f 01000000 04160108 00e20f00 .x.?............
+  0x00009af0 19790000 00000000 00250000 00280e00 .y.......%...(..
+  0x00009b00 19790700 00000000 00210000 00240e00 .y.......!...$..
+  0x00009b10 247a0000 00000000 07028e07 00ca1f00 $z..............
+  0x00009b20 0c7a0000 005c0000 7060f003 00e40f00 .z...\..p`......
+  0x00009b30 197809ff 1f000000 00140100 00c80f00 .x..............
+  0x00009b40 0c7a0009 005d0000 0061f003 00c80f00 .z...]...a......
+  0x00009b50 0c7c0007 04000000 70647008 00e40f00 .|......pdp.....
+  0x00009b60 12720500 03000000 fffc8e07 00c84f00 .r............O.
+  0x00009b70 0c720000 05000000 70267000 00da0f00 .r......p&p.....
+  0x00009b80 4d090000 00000000 00008003 00ea0f00 M...............
+  0x00009b90 117a0200 00580000 ff188007 00e20f04 .z...X..........
+  0x00009ba0 357404ff 08000000 ff010000 00e20f00 5t..............
+  0x00009bb0 027a1200 005a0000 000f0000 00e40f00 .z...Z..........
+  0x00009bc0 027a1300 005b0000 000f0000 00e40f00 .z...[..........
+  0x00009bd0 117a0300 00590000 091c0f00 00c60f00 .z...Y..........
+  0x00009be0 81791012 06000000 001b1e0c 00a80e00 .y..............
+  0x00009bf0 81790e02 06000000 001b1e0c 00a20e00 .y..............
+  0x00009c00 25760405 00580000 04028e07 00c60f00 %v...X..........
+  0x00009c10 81790c12 06100000 001b1e0c 00e80e00 .y..............
+  0x00009c20 81790812 06080000 001b1e0c 00280f00 .y...........(..
+  0x00009c30 81790604 06000000 001b1e0c 00280f00 .y...........(..
+  0x00009c40 81790a12 06180000 001b1e0c 00620f00 .y...........b..
+  0x00009c50 20720010 0f000000 00004000 00c44f00  r........@...O.
+  0x00009c60 20721511 0f000000 00004000 00e40f00  r........@.....
+  0x00009c70 2072140e 0d000000 00004000 00e48f08  r........@.....
+  0x00009c80 20720d0f 0d000000 00004000 00e40f00  r........@.....
+  0x00009c90 23720011 0e000000 00000000 00e40f08 #r..............
+  0x00009ca0 23721510 0e000000 15080000 00e40f00 #r..............
+  0x00009cb0 2372140f 0c000000 14000000 00c40f00 #r..............
+  0x00009cc0 23720d0e 0c000000 0d080000 00e40f00 #r..............
+  0x00009cd0 23720c09 06000000 00000000 00e40f09 #r..............
+  0x00009ce0 23720008 06000000 15000000 00e40f00 #r..............
+  0x00009cf0 23721407 0a000000 14000000 00e40f0a #r..............
+  0x00009d00 23720a06 0a000000 0d000000 00e40f00 #r..............
+  0x00009d10 23720d08 07000000 0c000000 00c40f00 #r..............
+  0x00009d20 23720c09 07000000 00010000 00e40f00 #r..............
+  0x00009d30 23720906 0b000000 14000000 00e40f08 #r..............
+  0x00009d40 23720807 0b000080 0a000000 00e20f00 #r..............
+  0x00009d50 86790002 0c000000 061b100c 00e80f00 .y..............
+  0x00009d60 86790004 08000000 061b100c 00e20f00 .y..............
+  0x00009d70 4d790000 00000000 00008003 00ea0f00 My..............
+  0x00009d80 47790000 f0ffffff ffff8303 00c00f00 Gy..............
   0x00009d90 18790000 00000000 00000000 00c00f00 .y..............
   0x00009da0 18790000 00000000 00000000 00c00f00 .y..............
   0x00009db0 18790000 00000000 00000000 00c00f00 .y..............
   0x00009dc0 18790000 00000000 00000000 00c00f00 .y..............
   0x00009dd0 18790000 00000000 00000000 00c00f00 .y..............
   0x00009de0 18790000 00000000 00000000 00c00f00 .y..............
   0x00009df0 18790000 00000000 00000000 00c00f00 .y..............
   0x00009e00 18790000 00000000 00000000 00c00f00 .y..............
   0x00009e10 18790000 00000000 00000000 00c00f00 .y..............
   0x00009e20 18790000 00000000 00000000 00c00f00 .y..............
   0x00009e30 18790000 00000000 00000000 00c00f00 .y..............
   0x00009e40 18790000 00000000 00000000 00c00f00 .y..............
-  0x00009e50 00000000 00000000 00000000 00000000 ................
-  0x00009e60 00000000 00000000 00000000 00000000 ................
-  0x00009e70 00000000 00000000 00000000 00000000 ................
+  0x00009e50 18790000 00000000 00000000 00c00f00 .y..............
+  0x00009e60 18790000 00000000 00000000 00c00f00 .y..............
+  0x00009e70 18790000 00000000 00000000 00c00f00 .y..............
   0x00009e80 00000000 00000000 00000000 00000000 ................
-  0x00009e90 01000000 03000000 00000000 00000000 ................
-  0x00009ea0 00000000 00000000 40000000 00000000 ........@.......
-  0x00009eb0 ad020000 00000000 00000000 00000000 ................
-  0x00009ec0 01000000 00000000 00000000 00000000 ................
-  0x00009ed0 0b000000 03000000 00000000 00000000 ................
-  0x00009ee0 00000000 00000000 ed020000 00000000 ................
-  0x00009ef0 25030000 00000000 00000000 00000000 %...............
-  0x00009f00 01000000 00000000 00000000 00000000 ................
-  0x00009f10 13000000 02000000 00000000 00000000 ................
-  0x00009f20 00000000 00000000 18060000 00000000 ................
-  0x00009f30 20010000 00000000 02000000 09000000  ...............
-  0x00009f40 08000000 00000000 18000000 00000000 ................
-  0x00009f50 6e020000 01000000 00000000 00000000 n...............
-  0x00009f60 00000000 00000000 38070000 00000000 ........8.......
-  0x00009f70 50010000 00000000 00000000 00000000 P...............
-  0x00009f80 01000000 00000000 00000000 00000000 ................
-  0x00009f90 29000000 00000070 00000000 00000000 )......p........
-  0x00009fa0 00000000 00000000 88080000 00000000 ................
-  0x00009fb0 90000000 00000000 03000000 00000000 ................
-  0x00009fc0 04000000 00000000 00000000 00000000 ................
-  0x00009fd0 5d000000 00000070 00000000 00000000 ]......p........
-  0x00009fe0 00000000 00000000 18090000 00000000 ................
-  0x00009ff0 6c000000 00000000 03000000 0e000000 l...............
-  0x0000a000 04000000 00000000 00000000 00000000 ................
-  0x0000a010 1a010000 00000070 00000000 00000000 .......p........
-  0x0000a020 00000000 00000000 84090000 00000000 ................
-  0x0000a030 6c000000 00000000 03000000 0f000000 l...............
-  0x0000a040 04000000 00000000 00000000 00000000 ................
-  0x0000a050 da010000 00000070 00000000 00000000 .......p........
-  0x0000a060 00000000 00000000 f0090000 00000000 ................
-  0x0000a070 6c000000 00000000 03000000 10000000 l...............
-  0x0000a080 04000000 00000000 00000000 00000000 ................
-  0x0000a090 9e020000 0b000070 00000000 00000000 .......p........
-  0x0000a0a0 00000000 00000000 600a0000 00000000 ........`.......
-  0x0000a0b0 e0000000 00000000 00000000 00000000 ................
-  0x0000a0c0 08000000 00000000 08000000 00000000 ................
-  0x0000a0d0 7b020000 09000000 00000000 00000000 {...............
-  0x0000a0e0 00000000 00000000 400b0000 00000000 ........@.......
-  0x0000a0f0 30000000 00000000 03000000 04000000 0...............
-  0x0000a100 08000000 00000000 10000000 00000000 ................
-  0x0000a110 bb000000 01000000 02000000 00000000 ................
-  0x0000a120 00000000 00000000 700b0000 00000000 ........p.......
-  0x0000a130 80010000 00000000 00000000 0e000000 ................
-  0x0000a140 04000000 00000000 00000000 00000000 ................
-  0x0000a150 7a010000 01000000 02000000 00000000 z...............
-  0x0000a160 00000000 00000000 f00c0000 00000000 ................
-  0x0000a170 80010000 00000000 00000000 0f000000 ................
-  0x0000a180 04000000 00000000 00000000 00000000 ................
-  0x0000a190 3a020000 01000000 02000000 00000000 :...............
-  0x0000a1a0 00000000 00000000 700e0000 00000000 ........p.......
-  0x0000a1b0 80010000 00000000 00000000 10000000 ................
-  0x0000a1c0 04000000 00000000 00000000 00000000 ................
-  0x0000a1d0 32000000 01000000 06000000 00000000 2...............
-  0x0000a1e0 00000000 00000000 00100000 00000000 ................
-  0x0000a1f0 001a0000 00000000 03000000 09000034 ...............4
-  0x0000a200 80000000 00000000 00000000 00000000 ................
-  0x0000a210 ee000000 01000000 06000000 00000000 ................
-  0x0000a220 00000000 00000000 002a0000 00000000 .........*......
-  0x0000a230 80080000 00000000 03000000 0a000022 ..............."
-  0x0000a240 80000000 00000000 00000000 00000000 ................
-  0x0000a250 ae010000 01000000 06000000 00000000 ................
-  0x0000a260 00000000 00000000 80320000 00000000 .........2......
-  0x0000a270 00040000 00000000 03000000 0b000018 ................
-  0x0000a280 80000000 00000000 00000000 00000000 ................
-  0x0000a290 06000000 05000000 c03a0000 00000000 .........:......
-  0x0000a2a0 00000000 00000000 00000000 00000000 ................
-  0x0000a2b0 a8000000 00000000 a8000000 00000000 ................
-  0x0000a2c0 08000000 00000000 01000000 05000000 ................
-  0x0000a2d0 700b0000 00000000 00000000 00000000 p...............
-  0x0000a2e0 00000000 00000000 102b0000 00000000 .........+......
-  0x0000a2f0 102b0000 00000000 08000000 00000000 .+..............
-  0x0000a300 01000000 05000000 c03a0000 00000000 .........:......
-  0x0000a310 00000000 00000000 00000000 00000000 ................
-  0x0000a320 a8000000 00000000 a8000000 00000000 ................
-  0x0000a330 08000000 00000000 01000101 48000000 ............H...
-  0x0000a340 401f0000 00000000 3d1f0000 40000000 @.......=...@...
-  0x0000a350 08000700 50000000 00000000 00000000 ....P...........
-  0x0000a360 11200000 00000000 00000000 00000000 . ..............
-  0x0000a370 8c620000 00000000 00000000 00000000 .b..............
-  0x0000a380 130a0100 f21c2e76 65727369 6f6e2037 .......version 7
-  0x0000a390 2e380a2e 74617267 65742073 6d5f3830 .8..target sm_80
-  0x0000a3a0 0a2e6164 64726573 735f7369 7a652036 ..address_size 6
-  0x0000a3b0 342f00ff 31697369 626c6520 2e656e74 4/..1isible .ent
-  0x0000a3c0 7279205f 5a313961 6374696f 6e4f6e53 ry _Z19actionOnS
-  0x0000a3d0 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
-  0x0000a3e0 74325330 5f6d506d 280a2e70 6172616d t2S0_mPm(..param
-  0x0000a3f0 202e7536 34330013 115f3100 3f5f302c  .u643..._1.?_0,
-  0x0000a400 3b00261f 313b0027 1f323b00 27f30833 ;.&.1;.'.2;.'..3
-  0x0000a410 0a290a7b 0a2e7265 67202e70 72656420 .).{..reg .pred 
-  0x0000a420 25703c36 3e3b1200 95663332 2025663c %p<6>;...f32 %f<
-  0x0000a430 34351200 10621200 36723c38 1100f201 45...b..6r<8....
-  0x0000a440 36342025 72643c31 333e3b0a 0a0a6c64 64 %rd<13>;...ld
-  0x0000a450 8a00222e 7518004f 322c205b 9000193d ..".u..O2, [...=
-  0x0000a460 305d3b44 001f3344 001c1f31 4400001f 0];D..3D...1D...
-  0x0000a470 3444001c 1f324400 001f3544 001c9133 4D...2D...5D...3
-  0x0000a480 5d3b0a6d 6f762e75 3401a832 2c20256e ];.mov.u4..2, %n
-  0x0000a490 7469642e 7816007c 332c2025 63746117 tid.x..|3, %cta.
-  0x0000a4a0 0044342c 20252c00 7161642e 6c6f2e73 .D4, %,.qad.lo.s
-  0x0000a4b0 18002335 2c340001 4f00f403 72343b0a ..#5,4..O...r4;.
-  0x0000a4c0 63767461 2e746f2e 676c6f62 616cab00 cvta.to.global..
-  0x0000a4d0 21362cb1 0001c400 041a0001 41004036 !6,.........A.@6
-  0x0000a4e0 2c205b20 00535d3b 0a6f72ce 0124312c , [ .S];.or..$1,
-  0x0000a4f0 5a001136 5000432e 73363470 0012641c Z..6P.C.s64p..d.
-  0x0000a500 00923b0a 73657470 2e676560 00357031 ..;.setp.ge`.5p1
-  0x0000a510 2c1c0073 64343b0a 7368725f 0013379b ,..sd4;.shr_..7.
-  0x0000a520 00173132 00001900 3370322c d6002172 ..12....3p2,..!r
-  0x0000a530 377a0003 6c022333 2c1c0014 70320022 7z..l.#3,...p2."
-  0x0000a540 65717b00 25703496 00183132 0024352c eq{.%p4...12.$5,
-  0x0000a550 3700ff08 343b0a40 25703520 62726120 7...4;.@%p5 bra 
-  0x0000a560 244c5f5f 4242305f 323b0a12 0104019a $L__BB0_2;......
-  0x0000a570 002f6432 31010511 381f0018 33310121 ./d21...8...31.!
-  0x0000a580 76320003 307b2566 e9003266 327d3b01 v2..0{%f..2f2};.
-  0x0000a590 20385df1 00146cf9 0214390b 0182333b  8]...l...9...3;
-  0x0000a5a0 0a616464 2e731700 3631302c 76001f39 .add.s..610,v..9
-  0x0000a5b0 57000300 cb002366 36570010 31fa0233 W.....#f6W..1..3
-  0x0000a5c0 6d756c74 03005700 02780018 35170001 mult..W..x..5...
-  0x0000a5d0 57002166 32390054 3b0a7375 62180025 W.!f29.T;.sub..%
-  0x0000a5e0 312c3500 1f30c500 04013600 243133c7 1,5..0....6.$13.
-  0x0000a5f0 00232b38 71004577 696465ef 0122312c .#+8q.Ewide.."1,
-  0x0000a600 11021a38 ce00003c 0004ce00 2f313161 ...8...<..../11a
-  0x0000a610 00041136 61001437 d1000043 0363666d ...6a..7...C.cfm
-  0x0000a620 612e726e a5001132 bd000388 00022d00 a.rn...2......-.
-  0x0000a630 1831dd00 223231a2 00010600 19371a00 .1.."21......7..
-  0x0000a640 15320f01 1c365500 15331201 0150012c .2...6U..3...P.,
-  0x0000a650 32322100 17345600 0176001f 32e70104 22!..4V..v..2...
-  0x0000a660 12324100 15362201 3931365d 86000160 .2A..6".916]...`
-  0x0000a670 012d3235 96011233 96011d36 97013533 .-25...3...6..53
-  0x0000a680 312c3800 1f339801 041133bc 00163398 1,8..3....3...3.
-  0x0000a690 012c3234 39011133 5a002633 32c30019 .,249..3Z.&32...
-  0x0000a6a0 33390121 33371400 0f390100 2633389a 39.!37...9..&38.
-  0x0000a6b0 001c3556 0007cf00 0255001b 38220027 ..5V.....U..8".'
-  0x0000a6c0 34307800 0264001c 39230017 31d40101 40x..d..9#..1...
-  0x0000a6d0 23002832 34020135 34322cfa 011032e4 #.(24..542,...2.
-  0x0000a6e0 031b7402 0103fc02 342c207b 2d003c34 ..t.....4, {-.<4
-  0x0000a6f0 317d6500 1733e000 01ab0029 34306500 1}e..3.....)40e.
-  0x0000a700 26342c26 011f3765 00051332 6500012d &4,&..7e...2e..-
-  0x0000a710 00653433 7d3b0a0a 37049f3a 0a726574 .e43};..7..:.ret
-  0x0000a720 3b0a0a7d 32080b4f 446f7562 32081c0e ;..}2..ODoub2...
-  0x0000a730 33000e32 080f3b00 241f313b 00271f32 3..2..;.$.1;.'.2
-  0x0000a740 3b00270f 3208012c 31373308 3c313631 ;.'.2..,173.<161
-  0x0000a750 34082d31 3235082f 32303508 060e9300 4.-125./205.....
-  0x0000a760 0f35082b 0e44000f 35081f0e 44000f35 .5.+.D..5...D..5
-  0x0000a770 081f0e44 000f3508 091f341f 08031f35 ...D..5...4....5
-  0x0000a780 4c08021f 36350804 15374a07 1634e507 L...65...7J..4..
-  0x0000a790 0f350814 233634f9 05043608 30637674 .5..#64...6.0cvt
-  0x0000a7a0 6f00031a 00023707 1c374d08 0172001f o.....7..7M..r..
-  0x0000a7b0 38490000 13384900 2d2b384b 0021392c 8I...8I.-+8K.!9,
-  0x0000a7c0 2100074b 0015324b 0019398e 0617398d !..K..2K..9...9.
-  0x0000a7d0 061c3847 00037907 17394800 15334800 ..8G..y..9H..3H.
-  0x0000a7e0 23313066 08136ef2 06267031 1c000c1b #10f..n..&p1....
-  0x0000a7f0 00067f00 69323b0a 616e64b4 081131b9 ....i2;.and...1.
-  0x0000a800 080c3300 15343300 19333300 09b5080a ..3..43..33.....
-  0x0000a810 33002436 2c35010a 66002337 2c1d002c 3.$6,5..f.#7,..,
-  0x0000a820 70353300 15383300 0a660023 392c1d00 p53..83..f.#9,..
-  0x0000a830 2c703733 00021601 1e323400 01f10702 ,p73.....24.....
-  0x0000a840 1f002f70 39fe0903 044d0022 6c746301 ../p9....M."ltc.
-  0x0000a850 1170ee05 031d000a ff09023f 08163500 .p.........?..5.
-  0x0000a860 0a226c74 1a001170 800701a2 023a7231 ."lt...p.....:r1
-  0x0000a870 31820024 342c2000 2a703104 01363135 1..$4, .*p1..615
-  0x0000a880 2c210065 313b0a6e 6f741b00 11361500 ,!.e1;.not...6..
-  0x0000a890 1135040a 27313605 0a1f3105 0a082f31 .5..'16...1.../1
-  0x0000a8a0 30060a0b 2f313107 0a162a31 31080a2f 0.../11...*11../
-  0x0000a8b0 3132090a 0427332c 7a002f31 320b0a11 12...'3,z./12...
-  0x0000a8c0 2f335d0b 0a5a2f31 310c0a03 1f340c0a /3]..Z/11....4..
-  0x0000a8d0 0328352c d1001f34 6300041a 360d0a1f .(5,...4c...6...
-  0x0000a8e0 350d0a2d 06e10002 0d0a0653 080f7f00 5..-.......S....
-  0x0000a8f0 0103160a 1634e200 2f3136e3 00011336 .....4../16....6
-  0x0000a900 17030be3 0001c303 05e3001f 36640004 ............6d..
-  0x0000a910 11376400 14386400 1d37b709 01c30003 .7d..8d..7......
-  0x0000a920 8b001437 9d0a06e3 00025909 02a00a28 ...7......Y....(
-  0x0000a930 3238e300 02eb0802 40001f33 33020411 28......@..33...
-  0x0000a940 33380026 3335e300 2f3234e3 00011338 38.&35../24....8
-  0x0000a950 330e0be3 0028392c e3001f38 64000411 3....(9,...8d...
-  0x0000a960 38640014 3964001c 39e30002 b209038b 8d..9d..9.......
-  0x0000a970 00022d00 1833e300 03ba0914 353c0a07 ..-..3......5<..
-  0x0000a980 1a001634 b80b0b99 0a253435 f2020119 ...4.....%45....
-  0x0000a990 022c3434 21001c36 750a1d34 44001737 .,44!..6u..4D..7
-  0x0000a9a0 3f020246 000c3a0c 2734389f 01010c00 ?..F..:.'48.....
-  0x0000a9b0 2c343723 001739a2 01026900 0c240b27 ,47#..9...i..$.'
-  0x0000a9c0 35300201 012f001f 34ef0d05 01d20016 50.../..4.......
-  0x0000a9d0 35410448 2b33325d 13011135 f8001e35 5A.H+32]...5...5
-  0x0000a9e0 eb032235 363a000d ec033635 372c3800 .."56:....657,8.
-  0x0000a9f0 0fa70204 1135db00 26353977 003b3430 .....5..&59w.;40
-  0x0000aa00 5dc50011 365b0026 35382e01 1935470c ]...6[.&58...5G.
-  0x0000aa10 22363344 000e8d03 3536342c 40001f36 "63D....564,@..6
-  0x0000aa20 38050411 36a00027 36368200 1d388200 8...6..'66...8..
-  0x0000aa30 015c0026 36356a01 28363482 00223730 .\.&65j.(64.."70
-  0x0000aa40 44000e2c 03353731 2c40001f 37f10404 D..,.571,@..7...
-  0x0000aa50 1137a000 1737f104 2c353682 0011375c .7...7..,56...7\
-  0x0000aa60 00022a00 02cb0219 37910422 37374400 ..*.....7.."77D.
-  0x0000aa70 0ecb0226 37389f01 0ccc0226 3739d401 ...&78.....&79..
-  0x0000aa80 0261000c 41022738 307c0102 64000c65 .a..A.'80|..d..e
-  0x0000aa90 0d273831 7f010146 002c3830 23001732 .'81...F.,80#..2
-  0x0000aaa0 4001014c 002c3831 23001733 43010169 @..L.,81#..3C..i
-  0x0000aab0 001c382c 0f273834 0401016f 001f38d4 ..8,.'84...o..8.
-  0x0000aac0 01041138 6a001738 d4013836 345d1501 ...8j..8..864]..
-  0x0000aad0 12383f00 01270009 cd022239 303a000d .8?..'...."90:..
-  0x0000aae0 cd023539 312c3800 1f39c901 0411399b ..591,8..9....9.
-  0x0000aaf0 001739c9 013b3732 5dc50011 395b0026 ..9..;72]...9[.&
-  0x0000ab00 39322e01 1939c901 22393744 000ecd02 92...9.."97D....
-  0x0000ab10 3639382c 40001f37 82000403 5a071630 698,@..7....Z..0
-  0x0000ab20 83001d38 50032131 305e0026 39396c01 ...8P.!10^.&99l.
-  0x0000ab30 28393884 00213130 6a013e31 3030d102 (98..!10j.>100..
-  0x0000ab40 46313035 2c44002f 31306207 05223036 F105,D./10b.."06
-  0x0000ab50 20001737 8a000d58 031131e2 05042d00  ..7...X..1...-.
-  0x0000ab60 02d80229 31309101 12313208 3e313037 ...)10...12.>107
-  0x0000ab70 db023631 3132ae01 0cdc0236 313133e4 ..6112.....6113.
-  0x0000ab80 0122362c 2f000d24 0017348e 01123725 ."6,/..$..4...7%
-  0x0000ab90 001d3325 00173593 01034a00 1d342500 ..3%..5...J..4%.
-  0x0000aba0 17365401 02c9002d 31352500 18375801 .6T....-15%..7X.
-  0x0000abb0 0370001d 36260018 38150112 3926000f .p..6&..8...9&..
-  0x0000abc0 f1010422 31312000 1732f201 3939365d ..."11 ..2..996]
-  0x0000abd0 26010245 06032a00 1a351b00 13343e00 &..E..*..5...4>.
-  0x0000abe0 0df00212 317b1104 3d001f32 e8010502 ....1{..=..2....
-  0x0000abf0 be112731 32e8014c 3130345d d4000285 ..'12..L104]....
-  0x0000ac00 12042e00 0334000a 8c000251 083e3132 .....4.....Q.>12
-  0x0000ac10 37fb0213 31e61103 46002f33 318d0004 7...1...F./31...
-  0x0000ac20 03851118 335a090e ea131231 9212032e ....3Z.....1....
-  0x0000ac30 00038701 2a33328d 0013384a 000f0203 ....*32...8J....
-  0x0000ac40 00039301 0446000f 9e080412 31a01237 .....F......1..7
-  0x0000ac50 3134318d 001e328d 03026b08 032e0003 141...2...k.....
-  0x0000ac60 03030be7 02037308 2f343103 0300046e ......s./41....n
-  0x0000ac70 081f3004 03022734 37fb0102 2a000d6a ..0...'47...*..j
-  0x0000ac80 0812316b 08049c01 0206030d 6d081231 ..1k........m..1
-  0x0000ac90 6e08049f 0102c201 0d700812 31710804 n........p..1q..
-  0x0000aca0 5b010208 032d3439 26001831 5e010252 [....-49&..1^..R
-  0x0000acb0 002d3530 26001832 1a01027f 002d3531 .-50&..2.....-51
-  0x0000acc0 260008c5 09017100 293530af 01353534 &.....q.)50..554
-  0x0000acd0 2c0c0a2f 34338013 05123380 13032e00 ,../43....3.....
-  0x0000ace0 4d313533 7d690017 35630701 69002a38 M153}i..5c..i.*8
-  0x0000acf0 34690026 362caa07 0fe91306 14356900 4i.&6,.......5i.
-  0x0000ad00 22362c56 000e6900 1837f204 1238c201 "6,V..i..7...8..
-  0x0000ad10 0a830203 9107033f 052f3131 6d000514 .......?./11m...
-  0x0000ad20 376d0002 30002e35 376d0018 395c0203 7m..0..57m..9\..
-  0x0000ad30 27001932 6d003836 302ca902 1f356d00 '..2m.860,...5m.
-  0x0000ad40 0513396d 00033000 263539c5 141f31c5 ..9m..0.&59...1.
-  0x0000ad50 140d1438 8212af54 7269706c 65476174 ...8...TripleGat
-  0x0000ad60 65c41408 0f320012 0ec3140f 3a001c1f e....2......:...
-  0x0000ad70 313a0026 1f323a00 260ff21c 021c31c0 1:.&.2:.&.....1.
-  0x0000ad80 14363630 39ae1402 c0142d32 34c0142f .6609.....-24../
-  0x0000ad90 3332c014 021231f4 130f4001 160f3714 32....1...@...7.
-  0x0000ada0 001f3243 001b1f31 0215010f 43001b1f ..2C...1....C...
-  0x0000adb0 32430000 1f344300 1b2f335d 59110523 2C...4C../3]Y..#
-  0x0000adc0 352c2c12 06ae141f 38c41402 1f39f114 5,,.....8....9..
-  0x0000add0 032f3130 dc140401 bc080136 00247238 ./10.......6.$r8
-  0x0000ade0 e2132e6c 64d91400 3f032d35 5d2d1421 ...ld...?.-5]-.!
-  0x0000adf0 322c2000 072d1425 312c5600 2f31320b 2, ..-.%1,V./12.
-  0x0000ae00 15071f35 c2140001 0f090a0e 1517324e ...5..........2N
-  0x0000ae10 000a1812 23382c9a 00023200 0b4a001d ....#8,...2..J..
-  0x0000ae20 340d1517 334a001f 34980000 14399800 4...3J..4....9..
-  0x0000ae30 2e313699 001d3514 1517344f 001a351a .16...5...4O..5.
-  0x0000ae40 1017309a 001d394b 00133638 10074c00 ..0...9K..68..L.
-  0x0000ae50 17354c00 1a364c00 1731ab15 0e4c0002 .5L..6L..1...L..
-  0x0000ae60 18002731 314c0017 364c001f 37841c01 ..'11L..6L..7...
-  0x0000ae70 0353001d 364d0015 38611305 4d001737 .S..6M..8a..M..7
-  0x0000ae80 4d001f38 fa15022f 3131fb15 072f3131 M..8.../11.../11
-  0x0000ae90 fc151f2f 3131fd15 201331cb 1f0ffe15 .../11.. .1.....
-  0x0000aea0 1904981f 0cff1501 39001f38 ff150302 ........9..8....
-  0x0000aeb0 35001936 35000114 00023b00 2d313037 5..65.....;.-107
-  0x0000aec0 00070801 1a373700 26332c3d 160d0b01 .....77.&3,=....
-  0x0000aed0 053a142f 2572d115 081d3337 00020f01 .:./%r....37....
-  0x0000aee0 0e420101 2902021f 0001f315 0b370002 .B..)........7..
-  0x0000aef0 12010e45 01019409 021f003c 70313737 ...E.......<p177
-  0x0000af00 0001d009 1f724801 00017a14 021f003d .....rH...z....=
-  0x0000af10 70313937 00021401 0e4a0101 c70b021f p197.....J......
-  0x0000af20 003d7032 31370006 13010a4a 0101050c .=p217.....J....
-  0x0000af30 021f003d 70323337 00011301 1e321301 ...=p237.....2..
-  0x0000af40 01d30902 1f003d70 32353700 15383700 ......=p257..87.
-  0x0000af50 0a130101 8b1e021f 002d7032 13012533 .........-p2..%3
-  0x0000af60 3037000a 13010139 0c021f00 2d703213 07.....9....-p2.
-  0x0000af70 01253332 37000a13 0101a40a 021f003d .%327..........=
-  0x0000af80 70333137 00153437 000a1301 016a0a02 p317..47.....j..
-  0x0000af90 1f003d70 33333700 0113011e 33dc0001 ..=p337.....3...
-  0x0000afa0 2e0c021f 002d7033 13012533 3837000b .....-p3..%387..
-  0x0000afb0 dc002439 2c1f003c 70333737 00253430 ..$9,..<p377.%40
-  0x0000afc0 37000adc 0001cf09 021f003d 70333937 7..........=p397
-  0x0000afd0 00153237 000adc00 01111502 1f002d70 ..27..........-p
-  0x0000afe0 34130101 010a2e72 34a50001 a00c021f 4......r4.......
-  0x0000aff0 003d7034 33370015 3637000b a5002437 .=p437..67....$7
-  0x0000b000 2c1f003d 70343537 00153837 000ba500 ,..=p457..87....
-  0x0000b010 24392c1f 003c7034 37370001 810c2e72 $9,..<p477.....r
-  0x0000b020 356e0001 740c021f 003d7034 39370015 5n..t....=p497..
-  0x0000b030 3237000a 6e00015f 0c021f00 3d703531 27..n.._....=p51
-  0x0000b040 370002d7 000f3700 0024352c 1f003e70 7.....7..$5,..>p
-  0x0000b050 3533bb1a 14336c1a 0abd1a01 150c041f 53...3l.........
-  0x0000b060 00296433 be1a0447 080dbe1a 01300c03 .)d3...G.....0..
-  0x0000b070 5b1c2a31 39870024 382c2100 3a703536 [.*19..$8,!.:p56
-  0x0000b080 1b002639 2c210019 35bf1a01 c10b3170 ..&9,!..5.....1p
-  0x0000b090 3539bf1a 273630bf 1a1f32bf 1a091434 59..'60...2....4
-  0x0000b0a0 bf1a2f6c 640f0f00 099f1a00 21100f46 ../ld.......!..F
-  0x0000b0b0 00040184 012f6431 0f19052f 31311019 ...../d1.../11..
-  0x0000b0c0 051e3510 190fc41a 062f375d c41a5b3f ..5....../7]..[?
-  0x0000b0d0 342b38fe 18061f31 fe18051f 35fe180a 4+8....1....5...
-  0x0000b0e0 010f0107 c41a0dfe 18012406 048a0002 ..........$.....
-  0x0000b0f0 b00f0fc4 1a481f34 c41a0323 32304705 .....H.4...#20G.
-  0x0000b100 0ae30001 7c0005e3 001f3246 0104021a ....|.....2F....
-  0x0000b110 1005c41a 2c3231e3 00273331 25190fc4 ....,21..'31%...
-  0x0000b120 1a4e1f34 c41a0314 324e050b e3000062 .N.4....2N.....b
-  0x0000b130 0006e300 0f640005 1938c41a 2f3233c4 .....d...8../23.
-  0x0000b140 1a2d06e3 0002c41a 06f8100f 7f000102 .-..............
-  0x0000b150 5a122634 36e3002f 3332e300 0113348c Z.&46../32....4.
-  0x0000b160 050be300 003e0006 e3000f23 14040239 .....>.....#...9
-  0x0000b170 121435a1 141d326d 1d02c211 038b0001 ..5...2m........
-  0x0000b180 2d002834 34e30001 46050357 1b0adc11 -.(44...F..W....
-  0x0000b190 02931102 40001f35 7f000413 35321a06 ....@..5....52..
-  0x0000b1a0 e3002f34 30e30001 13360106 0be30000 ../40....6......
-  0x0000b1b0 560206e3 000f5d04 0402f210 1436ea13 V.....]......6..
-  0x0000b1c0 1d326d1d 02891a02 8b00022d 00283535 .2m........-.(55
-  0x0000b1d0 e300021b 1901a805 38663631 e3000212 ........8f61....
-  0x0000b1e0 19024000 2f36357f 00040238 001738e3 ..@./65....8..8.
-  0x0000b1f0 000f6f04 01027809 1d36e300 00730106 ..o...x..6...s..
-  0x0000b200 e3000f6f 040402c9 1a1437c2 051d326f ...o......7...2o
-  0x0000b210 041137c3 00028b00 03f61a18 36e30002 ..7.........6...
-  0x0000b220 c21a2236 38470008 e30003bc 1a014000 .."68G........@.
-  0x0000b230 1f376201 0402c61a 263739e3 002f3536 .7b.....&79../56
-  0x0000b240 e3000002 240a1c37 e30001e8 0305e300 ....$..7........
-  0x0000b250 0fec2805 02a61a14 38b5051d 336f0402 ..(.....8...3o..
-  0x0000b260 6918028b 00243832 e71306e3 00353837 i....$82.....587
-  0x0000b270 2c551b29 38331a00 1f38501e 0616387e ,U.)83...8P...8~
-  0x0000b280 06015f00 1c385415 1839c805 1237861a .._..8T..9...7..
-  0x0000b290 0c230008 cb051436 a31a0a23 0017322b .#.....6...#..2+
-  0x0000b2a0 05143878 1a0a2300 1c33501e 1c393119 ..8x..#..3P..91.
-  0x0000b2b0 2739348e 04123917 190c2300 01c80126 '94...9...#....&
-  0x0000b2c0 3335b104 2f393404 1b0202f1 03019109 35../94.........
-  0x0000b2d0 2c663916 01263937 f4030214 041c39b8 ,f9..&97......9.
-  0x0000b2e0 16273938 54031431 161b0a23 00173957 .'98T..1...#..9W
-  0x0000b2f0 031430e9 1a092300 038d1903 b8021232 ..0...#........2
-  0x0000b300 c5190d24 001731bc 0222312c 37000d25 ...$..1.."1,7..%
-  0x0000b310 0017321e 02123325 000fa918 05053e1b ..2...3%......>.
-  0x0000b320 06d0020b a21c03ff 15032a00 0b980826 ..........*....&
-  0x0000b330 382ca61b 0a9b0838 30392c3d 000f3c08 8,.....809,=..<.
-  0x0000b340 0502db08 36313131 80000eab 1c031e1b ....6111........
-  0x0000b350 042d0002 43081a30 7f180153 03004900 .-..C..0...S..I.
-  0x0000b360 0e460803 131b0546 000fbd04 0404151b .F.....F........
-  0x0000b370 1731bf04 0fb41c00 03ae0826 31379e02 .1.........&17..
-  0x0000b380 013b1b07 8c0002b7 08033f1b 0aef0705 .;........?.....
-  0x0000b390 c71a0246 000f8e07 0505101b 07f4070f ...F............
-  0x0000b3a0 b61c0002 40032731 3295073a 3132338c ....@.'12..:123.
-  0x0000b3b0 00133949 000e9807 050c1b03 46000f91 ..9I........F...
-  0x0000b3c0 21040410 1b163335 0b02da1b 0a8c0002 !.....35........
-  0x0000b3d0 6903032d 00022a03 39313330 8c000175 i..-..*.9130...u
-  0x0000b3e0 0e04441b 0b1d1904 0b1b0346 000f7e05 ..D........F..~.
-  0x0000b3f0 04050f1b 0780050f e61b0102 6d08032e ............m...
-  0x0000b400 00027103 39313337 8d0002b0 0803441b ..q.9137......D.
-  0x0000b410 0aeb0605 62180246 000fb408 05050f1b ....b..F........
-  0x0000b420 07b6080e e61b05b1 1a273435 b6030a59 .........'45...Y
-  0x0000b430 0804ae1a 2e343695 0604a41a 0346002f .....46......F./
-  0x0000b440 35308d00 04243532 301a068d 000fe61b 50...$520.......
-  0x0000b450 0002a704 032e0002 3c0601cc 1a088d00 ........<.......
-  0x0000b460 02f7192e 35333f06 283135f2 030c4206 ....53?.(15...B.
-  0x0000b470 04c41902 2b040369 000de804 283630cd ....+..i....(60.
-  0x0000b480 03036c00 0dea0402 490504d0 0302f303 ..l.....I.......
-  0x0000b490 1d36eb04 02522304 8d0302e6 1b2d3631 .6...R#......-61
-  0x0000b4a0 26001833 90030272 001d3683 1f02db08 &..3...r..6.....
-  0x0000b4b0 27313254 063d3136 33260018 35500303 '12T.=163&..5P..
-  0x0000b4c0 72000d85 1f022d09 030d0302 5a063d31 r.....-.....Z.=1
-  0x0000b4d0 36352600 17371003 03e0012d 36362600 65&..7.....-66&.
-  0x0000b4e0 1838cc02 0310010d 161d02da 2304cf02 .8..........#...
-  0x0000b4f0 02f2021d 367c0128 37308b02 023d011d ....6|.(70...=..
-  0x0000b500 367c0128 37318e02 020d002d 37302600 6|.(71.....-70&.
-  0x0000b510 18324a02 0263012f 37319e02 04133720 .2J..c./71....7 
-  0x0000b520 0008a70d 3932385d 5c02027f 092f3137 ....928]\..../17
-  0x0000b530 69060002 cd062f31 37690600 02e60805 i...../17i......
-  0x0000b540 3d000f69 06050240 24273138 69062e31 =..i...@$'18i..1
-  0x0000b550 33c60402 db232831 386a061a 376a0602 3....#(18j..7j..
-  0x0000b560 c9211231 6e240b6a 06029909 0546000f .!.1n$.j.....F..
-  0x0000b570 6a060502 a0092731 386a062e 3134c604 j.....'18j..14..
-  0x0000b580 034e0927 3837b802 1a386b06 0332221f .N.'87...8k..2".
-  0x0000b590 386b0601 03292203 46002f39 328d0004 8k...)".F./92...
-  0x0000b5a0 024b0927 31396b06 2e3135c6 0402e608 .K.'19k..15.....
-  0x0000b5b0 2831396c 062a3933 8d001339 4a000e6c (19l.*93...9J..l
-  0x0000b5c0 061232de 08054600 0f6c0604 1232e108 ..2...F..l...2..
-  0x0000b5d0 38323032 cf0f0dc6 041232fc 23273230 8202......2.#'20
-  0x0000b5e0 6d063832 30308d00 1232b622 2f32306d m.8200...2."/20m
-  0x0000b5f0 06001232 96080546 000f6d06 041232df ...2...F..m...2.
-  0x0000b600 08283230 6d061d36 86071232 120b032e .(20m..6...2....
-  0x0000b610 00027b03 2932306d 06123212 0b2f3230 ..{.)20m..2../20
-  0x0000b620 6d060012 32970804 46002f31 338d0004 m...2...F./13...
-  0x0000b630 02e10828 32316d06 1d37c102 1132b411 ...(21m..7...2..
-  0x0000b640 042e0002 bc033932 31348d00 0450110f ......9214...P..
-  0x0000b650 6d060012 32980804 46000f10 110602e2 m...2...F.......
-  0x0000b660 08283232 6d061d38 c1021132 cc0e042e .(22m..8...2....
-  0x0000b670 00026d06 3a323231 8d001337 4a000e6d ..m.:221...7J..m
-  0x0000b680 06283232 f6030c6d 06373232 392f0403 .(22...m.7229/..
-  0x0000b690 69000cf1 04383233 30d00303 6c001d39 i....8230...l..9
-  0x0000b6a0 26001831 d303024c 002d3330 26001832 &..1...L.-30&..2
-  0x0000b6b0 8f031238 26001d31 26001833 9203022c ...8&..1&..3...,
-  0x0000b6c0 002d3332 26001834 4e03026e 012d3333 .-32&..4N..n.-33
-  0x0000b6d0 26001835 51030372 001d3426 0017360d &..5Q..r..4&..6.
-  0x0000b6e0 03026d06 3d323335 26001737 10030333 ..m.=235&..7...3
-  0x0000b6f0 032d3336 26001838 cc021231 26001d37 .-36&..8...1&..7
-  0x0000b700 26001839 cf020372 000d7c01 2834308b &..9...r..|.(40.
-  0x0000b710 02123226 000d7c01 2834318e 02020d00 ..2&..|.(41.....
-  0x0000b720 2d343026 0018324a 02123326 000f6d06 -40&..2J..3&..m.
-  0x0000b730 04233234 2000086d 06393932 5d5c0202 .#24 ..m.992]\..
-  0x0000b740 91242e32 346d0632 3234381b 000e6d06 .$.24m.2248...m.
-  0x0000b750 13323801 043d000f 6d060413 32850117 .28..=..m...2...
-  0x0000b760 356d062e 3230c604 02501203 2e000377 5m..20...P.....w
-  0x0000b770 02293439 8c000259 122f3235 6d060012 .)49...Y./25m...
-  0x0000b780 32cb0905 46000f6d 06041232 cf093832 2...F..m...2..82
-  0x0000b790 35388d00 0ec60403 ed012735 37b80229 58........'57..)
-  0x0000b7a0 35368d00 026e092f 32356d06 00123264 56...n./25m...2d
-  0x0000b7b0 09044600 2f36328d 00040265 09273236 ..F./62....e.'26
-  0x0000b7c0 6d063e32 31368d00 02630027 3634f902 m.>216...c.'64..
-  0x0000b7d0 2a36338d 0013394a 000f6d06 0002e708 *63...9J..m.....
-  0x0000b7e0 0546000f 6d060503 6e022737 328d002d .F..m...n.'72..-
-  0x0000b7f0 32348d00 02111228 32376d06 2937308d 24.....(27m.)70.
-  0x0000b800 00025412 2f32376d 0601029a 08054600 ..T./27m......F.
-  0x0000b810 0f6d0605 02e30818 325a123d 3233328d .m......2Z.=232.
-  0x0000b820 00034605 2737387b 030afd11 13321f03 ..F.'78{.....2..
-  0x0000b830 1f376d06 01029a08 0446002f 38338d00 .7m......F./83..
-  0x0000b840 0402e408 37323836 8d000e10 2f123233 ....7286..../.23
-  0x0000b850 12283238 6d062938 348d0002 35122f32 .(28m.)84...5./2
-  0x0000b860 386d0601 029a0804 46000fcd 2c051332 8m......F...,..2
-  0x0000b870 32122839 338d000e c10202cd 11283239 2.(93........(29
-  0x0000b880 6d060ad3 2c1232cd 112f3239 6d060102 m...,.2../29m...
-  0x0000b890 9a082f32 346d0603 02db0827 32346d06 ../24m.....'24m.
-  0x0000b8a0 0dc21112 33e40828 32356d06 0dc41112 ....3..(25m.....
-  0x0000b8b0 33a80527 32356d06 1d33c511 1233a805 3..'25m..3...3..
-  0x0000b8c0 2732356d 063d3330 31260018 33920312 '25m.=301&..3...
-  0x0000b8d0 3726001d 32260018 344e0312 3926001d 7&..2&..4N..9&..
-  0x0000b8e0 33260018 35510303 72001d34 26001736 3&..5Q..r..4&..6
-  0x0000b8f0 0d0302ea 003d3330 35260017 37100302 .....=305&..7...
-  0x0000b900 33033d33 30362600 1838cc02 12312600 3.=306&..8...1&.
-  0x0000b910 1d372600 1839cf02 0372000d 7c01024f .7&..9...r..|..O
-  0x0000b920 0e273238 6d063d33 30392600 18318e02 .'28m.=309&..1..
-  0x0000b930 0272002d 31302600 18324a02 12332600 .r.-10&..2J..3&.
-  0x0000b940 0f6d0604 23333120 00076d06 15321316 .m..#31 ..m..2..
-  0x0000b950 025c0212 330c022e 33316d06 1233950e .\..3...31m..3..
-  0x0000b960 2e33316d 06123385 09053d00 0f6d0604 .31m..3...=..m..
-  0x0000b970 1233cf09 2833326d 0601c413 0ad50003 .3..(32m........
-  0x0000b980 d80e2732 30770229 31398c00 03d50e1f ..'20w.)19......
-  0x0000b990 326d0600 1233cb09 0546000f 6d060413 2m...3...F..m...
-  0x0000b9a0 33840227 32388d00 0ed11312 33710903 3..'28......3q..
-  0x0000b9b0 2e000434 00096d06 12336e09 2f33326d ...4..m..3n./32m
-  0x0000b9c0 06001333 351b0346 000f371b 06031f16 ...35..F..7.....
-  0x0000b9d0 09391b0e d2131333 ec022733 34f9020a .9.....3..'34...
-  0x0000b9e0 dc1a1333 35031f33 6d060012 33e70805 ...35..3m...3...
-  0x0000b9f0 46000f6d 06041233 e8082833 346d060e F..m...3..(34m..
-  0x0000ba00 d3131233 9b0f032e 00033a03 2934308d ...3......:.)40.
-  0x0000ba10 0002980f 2f33346d 06001233 9a080546 ..../34m...3...F
-  0x0000ba20 000f6d06 041233e3 08283334 6d060ed4 ..m...3..(34m...
-  0x0000ba30 131233dc 0f032e00 037b0329 34378d00 ..3......{.)47..
-  0x0000ba40 0226122f 33346d06 0012339a 08044600 .&./34m...3...F.
-  0x0000ba50 2f35338d 000402e4 08273335 6d061e33 /53......'35m..3
-  0x0000ba60 d4131233 5d12032e 0003bc03 2935348d ...3].......)54.
-  0x0000ba70 0003a300 1f356d06 00133360 04034600 .....5m...3`..F.
-  0x0000ba80 2f36308d 000402e4 08273336 6d061e33 /60......'36m..3
-  0x0000ba90 d4131233 e1112733 366d063a 3336318d ...3..'36m.:361.
-  0x0000baa0 0013374a 000e6d06 12339a08 2f33316d ..7J..m..3../31m
-  0x0000bab0 06021233 db082633 316d061d 33cb1112 ...3..&31m..3...
-  0x0000bac0 33e40827 33326d06 1d33cb11 38333731 3..'32m..3..8371
-  0x0000bad0 d303024c 000dcb11 38333732 8f03029c ...L....8372....
-  0x0000bae0 002d3731 26001833 92030272 002d3732 .-71&..3...r.-72
-  0x0000baf0 26001834 4e0302ca 001d376d 06020e09 &..4N.....7m....
-  0x0000bb00 2833336d 061d376d 06025709 2833346d (33m..7m..W.(34m
-  0x0000bb10 061d372f 01026109 2833346d 062d3736 ..7/..a.(34m.-76
-  0x0000bb20 26001838 cc021231 26000d6d 06026606 &..8...1&..m..f.
-  0x0000bb30 2833346d 060d8c36 38333830 8b02023d (34m...68380...=
-  0x0000bb40 012d3739 26001831 8e02020d 000d9236 .-79&..1.......6
-  0x0000bb50 38333832 4a020263 012f3831 9e020404 8382J..c./81....
-  0x0000bb60 20001834 281f2930 5d5c0202 a00e2f33  ..4(.)0]\..../3
-  0x0000bb70 386d0600 02950e2f 33386d06 00028509 8m...../38m.....
-  0x0000bb80 053d000f 6d060502 cf093833 39318100 .=..m.....8391..
-  0x0000bb90 0ec60404 d80e1730 77022938 398c0004 .......0w.)89...
-  0x0000bba0 26120f6d 060102cb 09054600 0f6d0605 &..m......F..m..
-  0x0000bbb0 02cf0927 33396d06 1e33d413 12347109 ...'39m..3...4q.
-  0x0000bbc0 032e0003 b8022839 368d0012 346e092f ......(96...4n./
-  0x0000bbd0 33396d06 00123464 09034600 3f343032 39m...4d..F.?402
-  0x0000bbe0 8d000312 34650927 34306d06 1e33d413 ....4e.'40m..3..
-  0x0000bbf0 1234f408 032e0013 330d0009 1d041234 .4......3......4
-  0x0000bc00 f1081234 90090a6d 061234e7 08054600 ...4...m..4...F.
-  0x0000bc10 0f6d0604 1234e808 2734316d 061e33d4 .m...4..'41m..3.
-  0x0000bc20 1312349b 0f273431 6d063934 31308d00 ..4..'41m.9410..
-  0x0000bc30 02bd012f 34316d06 00123476 04054600 .../41m...4v..F.
-  0x0000bc40 0f6d0604 1234e308 2734316d 061e33d4 .m...4..'41m..3.
-  0x0000bc50 131234dc 0f032e00 027b0339 3431378d ..4......{.9417.
-  0x0000bc60 00022612 2f34316d 06001234 9a080446 ..&./41m...4...F
-  0x0000bc70 002f3233 8d000402 e4083834 32368d00 ./23......8426..
-  0x0000bc80 0dc10212 345d1227 34326d06 39343234 ....4].'42m.9424
-  0x0000bc90 8d00025b 122f3432 6d060012 349a0804 ...[./42m...4...
-  0x0000bca0 46002f33 308d0004 02e40837 3433338d F./30......7433.
-  0x0000bcb0 000ed413 1234e111 2734336d 063a3433 .....4..'43m.:43
-  0x0000bcc0 318d0013 374a000e 6d062834 33f6030c 1...7J..m.(43...
-  0x0000bcd0 6d063734 33392f04 0369000c f1043834 m.7439/..i....84
-  0x0000bce0 3430d003 036c001d 39260018 31d30302 40...l..9&..1...
-  0x0000bcf0 4c000dcb 111234a8 05273339 6d063d34 L.....4..'39m.=4
-  0x0000bd00 34312600 18339203 0272002d 34322600 41&..3...r.-42&.
-  0x0000bd10 18344e03 026e012d 34332600 18355103 .4N..n.-43&..5Q.
-  0x0000bd20 0372001d 34260017 360d0302 6d063d34 .r..4&..6...m.=4
-  0x0000bd30 34352600 17371003 0333030d ca361234 45&..7...3...6.4
-  0x0000bd40 66062734 316d063d 34343726 001839cf f.'41m.=447&..9.
-  0x0000bd50 02037200 0d7c0128 35308b02 0278002d ..r..|.(50...x.-
-  0x0000bd60 34392600 18318e02 020d002d 35302600 49&..1.....-50&.
-  0x0000bd70 18324a02 12332600 0f6d0604 23343520 .2J..3&..m..#45 
-  0x0000bd80 00086d06 01e51507 5c0202a0 0e2e3435 ..m.....\.....45
-  0x0000bd90 6d061234 950e2e34 356d0612 34850905 m..4...45m..4...
-  0x0000bda0 3d000f6d 06041334 13012736 31810001 =..m...4..'61...
-  0x0000bdb0 c8130ad5 0002d80e 032e0003 77022935 ............w.)5
-  0x0000bdc0 398c0002 d50e2f34 366d0600 1234cb09 9...../46m...4..
-  0x0000bdd0 0546000f 6d060412 34cf0919 34dd240e .F..m...4...4.$.
-  0x0000bde0 d4131334 7b012736 37b8020a 80241334 ...4{.'67....$.4
-  0x0000bdf0 c4011f36 6d060102 64090446 002f3732 ...6m...d..F./72
-  0x0000be00 8d000402 65093834 37358d00 0ec60402 ....e.8475......
-  0x0000be10 f408032e 0003f902 2a37338d 0013394a ........*73...9J
-  0x0000be20 000f6d06 0002e708 0546000f 6d060502 ..m......F..m...
-  0x0000be30 e8082734 386d061e 34d41312 349b0f28 ..'48m..4...4..(
-  0x0000be40 34386d06 2938308d 0002980f 2f34386d 48m.)80...../48m
-  0x0000be50 0601029a 08054600 0f6d0605 02e30827 ......F..m.....'
-  0x0000be60 34386d06 1e34d413 1234dc0f 032e0003 48m..4...4......
-  0x0000be70 7b031a38 6d060226 122f3438 6d060102 {..8m..&./48m...
-  0x0000be80 9a080446 002f3933 8d000402 e4082734 ...F./93......'4
-  0x0000be90 396d061e 34d41312 345d1228 34396d06 9m..4...4].(49m.
-  0x0000bea0 2839348d 0012355b 122f3439 6d060013 (94...5[./49m...
-  0x0000beb0 359a0802 46003f35 30308d00 031235e4 5...F.?500....5.
-  0x0000bec0 08273530 6d061e34 d4131235 e1112735 .'50m..4...5..'5
-  0x0000bed0 306d063a 3530318d 00123716 000f6d06 0m.:501...7...m.
-  0x0000bee0 00283530 f6030c6d 06373530 392f0403 .(50...m.7509/..
-  0x0000bef0 69000cf1 04383531 30d00303 6c001d39 i....8510...l..9
-  0x0000bf00 26001831 d303024c 000dcb11 38353132 &..1...L....8512
-  0x0000bf10 8f031238 26001d31 26001833 92030272 ...8&..1&..3...r
-  0x0000bf20 002d3132 26001834 4e03026e 012d3133 .-12&..4N..n.-13
-  0x0000bf30 26001835 51030372 001d3426 0017360d &..5Q..r..4&..6.
-  0x0000bf40 0302e205 3d353135 26001737 10030233 ....=515&..7...3
-  0x0000bf50 033d3531 36260018 38cc0202 52002d31 .=516&..8...R.-1
-  0x0000bf60 37260018 39cf0203 72000d7c 01024f0e 7&..9...r..|..O.
-  0x0000bf70 2734396d 063d3531 39260018 318e0202 '49m.=519&..1...
-  0x0000bf80 72002d32 30260018 324a0212 3326000f r.-20&..2J..3&..
-  0x0000bf90 6d060423 35322000 18349e02 29385d5c m..#52 ..4..)8]\
-  0x0000bfa0 02039a01 1e326d06 1335db01 1e326d06 .....2m..5...2m.
-  0x0000bfb0 12358509 053d000f 6d060412 35cf0927 .5...=..m...5..'
-  0x0000bfc0 35336d06 1134c813 0ad50002 d80e032e 53m..4..........
-  0x0000bfd0 00037702 2932398c 0002d50e 2f35336d ..w.)29...../53m
-  0x0000bfe0 06001235 cb090546 000f6d06 041235cf ...5...F..m...5.
-  0x0000bff0 09283533 6d060ed4 13133519 0f273337 .(53m.....5..'37
-  0x0000c000 b8022933 368d0002 6e092f35 336d0600 ..)36...n./53m..
-  0x0000c010 12356409 0446002f 34328d00 04031317 .5d..F./42......
-  0x0000c020 18346d06 0ed41312 35f40803 2e0003f9 .4m.....5.......
-  0x0000c030 022a3433 8d001339 4a000e6d 06133505 .*43...9J..m..5.
-  0x0000c040 03044600 0f6d0604 1235e808 37353532 ..F..m...5..7552
-  0x0000c050 8d000ed4 1312359b 0f032e00 03770029 ......5......w.)
-  0x0000c060 35308d00 02980f2f 35356d06 0012359a 50...../55m...5.
-  0x0000c070 08054600 0f6d0604 1235e308 38353539 ..F..m...5..8559
-  0x0000c080 8d000d87 071235dc 0f032e00 037b030a ......5......{..
-  0x0000c090 3a481235 26122f35 356d0600 12359a08 :H.5&./55m...5..
-  0x0000c0a0 0446002f 36338d00 0402e408 37353636 .F./63......7566
-  0x0000c0b0 8d000ed4 1312355d 12032e00 03bc030a ......5]........
-  0x0000c0c0 45481235 5b122f35 366d0601 04320002 EH.5[./56m...2..
-  0x0000c0d0 46002f37 308d0004 033b0406 4c483e34 F./70....;..LH>4
-  0x0000c0e0 2b35d413 1235e111 2835376d 062a3731 +5...5..(57m.*71
-  0x0000c0f0 8d001337 4a000f6d 0600029a 082f3532 ...7J..m...../52
-  0x0000c100 6d060302 db082735 326d060d cb111235 m.....'52m.....5
-  0x0000c110 e4082835 336d060d cb113835 3831d303 ..(53m....8581..
-  0x0000c120 024c000d cb113835 38328f03 029c000d .L....8582......
-  0x0000c130 60483835 38339203 0272000d 63483835 `H8583...r..cH85
-  0x0000c140 38344e03 02ca002d 38332600 18355103 84N....-83&..5Q.
-  0x0000c150 0372000d 6d060257 09030d03 0368032d .r..m..W.....h.-
-  0x0000c160 38352600 17371003 0333032d 38362600 85&..7...3.-86&.
-  0x0000c170 1838cc02 0252002d 38372600 1839cf02 .8...R.-87&..9..
-  0x0000c180 0372000d 7c012839 308b0202 3d010d53 .r..|.(90...=..S
-  0x0000c190 2e383539 318e0202 0d000d56 2e12358b .8591......V..5.
-  0x0000c1a0 09283537 6d060d59 2e373539 33192f12 .(57m..Y.7593./.
-  0x0000c1b0 32ad280a e0022639 34ca472f 3837cf42 2.(...&94.G/87.B
-  0x0000c1c0 0c032e00 2d3539a5 43123542 07044529 ....-59.C.5B..E)
-  0x0000c1d0 026b000b 4b03023f 07059229 1f37cf42 .k..K..?...).7.B
-  0x0000c1e0 0c033000 2d3539a9 43293539 45231232 ..0.-59.C)59E#.2
-  0x0000c1f0 ab1c0b6d 0028382c 92230f6d 00052432 ...m.(8,.#.m..$2
-  0x0000c200 316d0022 382c5a00 0e6d0018 39451d12 1m."8,Z..m..9E..
-  0x0000c210 32ab1609 6d001336 091d0492 1d0f6d00 2...m..6......m.
-  0x0000c220 0603ec44 0330003c 3539396d 001236dc ...D.0.<599m..6.
-  0x0000c230 0a283336 6d001b38 6d002832 2c92170f .(36m..8m.(2,...
-  0x0000c240 6d000603 f0440330 002d3630 40593836 m....D.0.-60@Y86
-  0x0000c250 30334511 1232ab0a 0b6d0028 342c9211 03E..2...m.(4,..
-  0x0000c260 0f6d0006 03210203 30002d36 30210212 .m...!..0.-60!..
-  0x0000c270 368e1027 35306d00 2b35326d 0028362c 6..'50m.+52m.(6,
-  0x0000c280 920b0f6d 00060321 02033000 2d363021 ...m...!..0.-60!
-  0x0000c290 02293630 4505026d 001b396d 0028382c .)60E..m..9m.(8,
-  0x0000c2a0 92050f6d 00051333 21020330 00363630 ...m...3!..0.660
-  0x0000c2b0 375d4515 325d4550 0a7d0a0a 00000000 7]E.2]EP.}......
+  0x00009e90 00000000 00000000 00000000 00000000 ................
+  0x00009ea0 00000000 00000000 00000000 00000000 ................
+  0x00009eb0 00000000 00000000 00000000 00000000 ................
+  0x00009ec0 01000000 03000000 00000000 00000000 ................
+  0x00009ed0 00000000 00000000 40000000 00000000 ........@.......
+  0x00009ee0 ad020000 00000000 00000000 00000000 ................
+  0x00009ef0 01000000 00000000 00000000 00000000 ................
+  0x00009f00 0b000000 03000000 00000000 00000000 ................
+  0x00009f10 00000000 00000000 ed020000 00000000 ................
+  0x00009f20 25030000 00000000 00000000 00000000 %...............
+  0x00009f30 01000000 00000000 00000000 00000000 ................
+  0x00009f40 13000000 02000000 00000000 00000000 ................
+  0x00009f50 00000000 00000000 18060000 00000000 ................
+  0x00009f60 20010000 00000000 02000000 09000000  ...............
+  0x00009f70 08000000 00000000 18000000 00000000 ................
+  0x00009f80 6e020000 01000000 00000000 00000000 n...............
+  0x00009f90 00000000 00000000 38070000 00000000 ........8.......
+  0x00009fa0 50010000 00000000 00000000 00000000 P...............
+  0x00009fb0 01000000 00000000 00000000 00000000 ................
+  0x00009fc0 29000000 00000070 00000000 00000000 )......p........
+  0x00009fd0 00000000 00000000 88080000 00000000 ................
+  0x00009fe0 90000000 00000000 03000000 00000000 ................
+  0x00009ff0 04000000 00000000 00000000 00000000 ................
+  0x0000a000 5d000000 00000070 00000000 00000000 ]......p........
+  0x0000a010 00000000 00000000 18090000 00000000 ................
+  0x0000a020 6c000000 00000000 03000000 0e000000 l...............
+  0x0000a030 04000000 00000000 00000000 00000000 ................
+  0x0000a040 1a010000 00000070 00000000 00000000 .......p........
+  0x0000a050 00000000 00000000 84090000 00000000 ................
+  0x0000a060 6c000000 00000000 03000000 0f000000 l...............
+  0x0000a070 04000000 00000000 00000000 00000000 ................
+  0x0000a080 da010000 00000070 00000000 00000000 .......p........
+  0x0000a090 00000000 00000000 f0090000 00000000 ................
+  0x0000a0a0 6c000000 00000000 03000000 10000000 l...............
+  0x0000a0b0 04000000 00000000 00000000 00000000 ................
+  0x0000a0c0 9e020000 0b000070 00000000 00000000 .......p........
+  0x0000a0d0 00000000 00000000 600a0000 00000000 ........`.......
+  0x0000a0e0 e0000000 00000000 00000000 00000000 ................
+  0x0000a0f0 08000000 00000000 08000000 00000000 ................
+  0x0000a100 7b020000 09000000 00000000 00000000 {...............
+  0x0000a110 00000000 00000000 400b0000 00000000 ........@.......
+  0x0000a120 30000000 00000000 03000000 04000000 0...............
+  0x0000a130 08000000 00000000 10000000 00000000 ................
+  0x0000a140 bb000000 01000000 02000000 00000000 ................
+  0x0000a150 00000000 00000000 700b0000 00000000 ........p.......
+  0x0000a160 80010000 00000000 00000000 0e000000 ................
+  0x0000a170 04000000 00000000 00000000 00000000 ................
+  0x0000a180 7a010000 01000000 02000000 00000000 z...............
+  0x0000a190 00000000 00000000 f00c0000 00000000 ................
+  0x0000a1a0 80010000 00000000 00000000 0f000000 ................
+  0x0000a1b0 04000000 00000000 00000000 00000000 ................
+  0x0000a1c0 3a020000 01000000 02000000 00000000 :...............
+  0x0000a1d0 00000000 00000000 700e0000 00000000 ........p.......
+  0x0000a1e0 80010000 00000000 00000000 10000000 ................
+  0x0000a1f0 04000000 00000000 00000000 00000000 ................
+  0x0000a200 32000000 01000000 06000000 00000000 2...............
+  0x0000a210 00000000 00000000 00100000 00000000 ................
+  0x0000a220 001a0000 00000000 03000000 09000034 ...............4
+  0x0000a230 80000000 00000000 00000000 00000000 ................
+  0x0000a240 ee000000 01000000 06000000 00000000 ................
+  0x0000a250 00000000 00000000 002a0000 00000000 .........*......
+  0x0000a260 80080000 00000000 03000000 0a000022 ..............."
+  0x0000a270 80000000 00000000 00000000 00000000 ................
+  0x0000a280 ae010000 01000000 06000000 00000000 ................
+  0x0000a290 00000000 00000000 80320000 00000000 .........2......
+  0x0000a2a0 00040000 00000000 03000000 0b000018 ................
+  0x0000a2b0 80000000 00000000 00000000 00000000 ................
+  0x0000a2c0 06000000 05000000 c03a0000 00000000 .........:......
+  0x0000a2d0 00000000 00000000 00000000 00000000 ................
+  0x0000a2e0 a8000000 00000000 a8000000 00000000 ................
+  0x0000a2f0 08000000 00000000 01000000 05000000 ................
+  0x0000a300 700b0000 00000000 00000000 00000000 p...............
+  0x0000a310 00000000 00000000 102b0000 00000000 .........+......
+  0x0000a320 102b0000 00000000 08000000 00000000 .+..............
+  0x0000a330 01000000 05000000 c03a0000 00000000 .........:......
+  0x0000a340 00000000 00000000 00000000 00000000 ................
+  0x0000a350 a8000000 00000000 a8000000 00000000 ................
+  0x0000a360 08000000 00000000 01000101 48000000 ............H...
+  0x0000a370 401f0000 00000000 3d1f0000 40000000 @.......=...@...
+  0x0000a380 08000700 50000000 00000000 00000000 ....P...........
+  0x0000a390 11200000 00000000 00000000 00000000 . ..............
+  0x0000a3a0 8c620000 00000000 00000000 00000000 .b..............
+  0x0000a3b0 130a0100 f21c2e76 65727369 6f6e2037 .......version 7
+  0x0000a3c0 2e380a2e 74617267 65742073 6d5f3830 .8..target sm_80
+  0x0000a3d0 0a2e6164 64726573 735f7369 7a652036 ..address_size 6
+  0x0000a3e0 342f00ff 31697369 626c6520 2e656e74 4/..1isible .ent
+  0x0000a3f0 7279205f 5a313961 6374696f 6e4f6e53 ry _Z19actionOnS
+  0x0000a400 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
+  0x0000a410 74325330 5f6d506d 280a2e70 6172616d t2S0_mPm(..param
+  0x0000a420 202e7536 34330013 115f3100 3f5f302c  .u643..._1.?_0,
+  0x0000a430 3b00261f 313b0027 1f323b00 27f30833 ;.&.1;.'.2;.'..3
+  0x0000a440 0a290a7b 0a2e7265 67202e70 72656420 .).{..reg .pred 
+  0x0000a450 25703c36 3e3b1200 95663332 2025663c %p<6>;...f32 %f<
+  0x0000a460 34351200 10621200 36723c38 1100f201 45...b..6r<8....
+  0x0000a470 36342025 72643c31 333e3b0a 0a0a6c64 64 %rd<13>;...ld
+  0x0000a480 8a00222e 7518004f 322c205b 9000193d ..".u..O2, [...=
+  0x0000a490 305d3b44 001f3344 001c1f31 4400001f 0];D..3D...1D...
+  0x0000a4a0 3444001c 1f324400 001f3544 001c9133 4D...2D...5D...3
+  0x0000a4b0 5d3b0a6d 6f762e75 3401a832 2c20256e ];.mov.u4..2, %n
+  0x0000a4c0 7469642e 7816007c 332c2025 63746117 tid.x..|3, %cta.
+  0x0000a4d0 0044342c 20252c00 7161642e 6c6f2e73 .D4, %,.qad.lo.s
+  0x0000a4e0 18002335 2c340001 4f00f403 72343b0a ..#5,4..O...r4;.
+  0x0000a4f0 63767461 2e746f2e 676c6f62 616cab00 cvta.to.global..
+  0x0000a500 21362cb1 0001c400 041a0001 41004036 !6,.........A.@6
+  0x0000a510 2c205b20 00535d3b 0a6f72ce 0124312c , [ .S];.or..$1,
+  0x0000a520 5a001136 5000432e 73363470 0012641c Z..6P.C.s64p..d.
+  0x0000a530 00923b0a 73657470 2e676560 00357031 ..;.setp.ge`.5p1
+  0x0000a540 2c1c0073 64343b0a 7368725f 0013379b ,..sd4;.shr_..7.
+  0x0000a550 00173132 00001900 3370322c d6002172 ..12....3p2,..!r
+  0x0000a560 377a0003 6c022333 2c1c0014 70320022 7z..l.#3,...p2."
+  0x0000a570 65717b00 25703496 00183132 0024352c eq{.%p4...12.$5,
+  0x0000a580 3700ff08 343b0a40 25703520 62726120 7...4;.@%p5 bra 
+  0x0000a590 244c5f5f 4242305f 323b0a12 0104019a $L__BB0_2;......
+  0x0000a5a0 002f6432 31010511 381f0018 33310121 ./d21...8...31.!
+  0x0000a5b0 76320003 307b2566 e9003266 327d3b01 v2..0{%f..2f2};.
+  0x0000a5c0 20385df1 00146cf9 0214390b 0182333b  8]...l...9...3;
+  0x0000a5d0 0a616464 2e731700 3631302c 76001f39 .add.s..610,v..9
+  0x0000a5e0 57000300 cb002366 36570010 31fa0233 W.....#f6W..1..3
+  0x0000a5f0 6d756c74 03005700 02780018 35170001 mult..W..x..5...
+  0x0000a600 57002166 32390054 3b0a7375 62180025 W.!f29.T;.sub..%
+  0x0000a610 312c3500 1f30c500 04013600 243133c7 1,5..0....6.$13.
+  0x0000a620 00232b38 71004577 696465ef 0122312c .#+8q.Ewide.."1,
+  0x0000a630 11021a38 ce00003c 0004ce00 2f313161 ...8...<..../11a
+  0x0000a640 00041136 61001437 d1000043 0363666d ...6a..7...C.cfm
+  0x0000a650 612e726e a5001132 bd000388 00022d00 a.rn...2......-.
+  0x0000a660 1831dd00 223231a2 00010600 19371a00 .1.."21......7..
+  0x0000a670 15320f01 1c365500 15331201 0150012c .2...6U..3...P.,
+  0x0000a680 32322100 17345600 0176001f 32e70104 22!..4V..v..2...
+  0x0000a690 12324100 15362201 3931365d 86000160 .2A..6".916]...`
+  0x0000a6a0 012d3235 96011233 96011d36 97013533 .-25...3...6..53
+  0x0000a6b0 312c3800 1f339801 041133bc 00163398 1,8..3....3...3.
+  0x0000a6c0 012c3234 39011133 5a002633 32c30019 .,249..3Z.&32...
+  0x0000a6d0 33390121 33371400 0f390100 2633389a 39.!37...9..&38.
+  0x0000a6e0 001c3556 0007cf00 0255001b 38220027 ..5V.....U..8".'
+  0x0000a6f0 34307800 0264001c 39230017 31d40101 40x..d..9#..1...
+  0x0000a700 23002832 34020135 34322cfa 011032e4 #.(24..542,...2.
+  0x0000a710 031b7402 0103fc02 342c207b 2d003c34 ..t.....4, {-.<4
+  0x0000a720 317d6500 1733e000 01ab0029 34306500 1}e..3.....)40e.
+  0x0000a730 26342c26 011f3765 00051332 6500012d &4,&..7e...2e..-
+  0x0000a740 00653433 7d3b0a0a 37049f3a 0a726574 .e43};..7..:.ret
+  0x0000a750 3b0a0a7d 32080b4f 446f7562 32081c0e ;..}2..ODoub2...
+  0x0000a760 33000e32 080f3b00 241f313b 00271f32 3..2..;.$.1;.'.2
+  0x0000a770 3b00270f 3208012c 31373308 3c313631 ;.'.2..,173.<161
+  0x0000a780 34082d31 3235082f 32303508 060e9300 4.-125./205.....
+  0x0000a790 0f35082b 0e44000f 35081f0e 44000f35 .5.+.D..5...D..5
+  0x0000a7a0 081f0e44 000f3508 091f341f 08031f35 ...D..5...4....5
+  0x0000a7b0 4c08021f 36350804 15374a07 1634e507 L...65...7J..4..
+  0x0000a7c0 0f350814 233634f9 05043608 30637674 .5..#64...6.0cvt
+  0x0000a7d0 6f00031a 00023707 1c374d08 0172001f o.....7..7M..r..
+  0x0000a7e0 38490000 13384900 2d2b384b 0021392c 8I...8I.-+8K.!9,
+  0x0000a7f0 2100074b 0015324b 0019398e 0617398d !..K..2K..9...9.
+  0x0000a800 061c3847 00037907 17394800 15334800 ..8G..y..9H..3H.
+  0x0000a810 23313066 08136ef2 06267031 1c000c1b #10f..n..&p1....
+  0x0000a820 00067f00 69323b0a 616e64b4 081131b9 ....i2;.and...1.
+  0x0000a830 080c3300 15343300 19333300 09b5080a ..3..43..33.....
+  0x0000a840 33002436 2c35010a 66002337 2c1d002c 3.$6,5..f.#7,..,
+  0x0000a850 70353300 15383300 0a660023 392c1d00 p53..83..f.#9,..
+  0x0000a860 2c703733 00021601 1e323400 01f10702 ,p73.....24.....
+  0x0000a870 1f002f70 39fe0903 044d0022 6c746301 ../p9....M."ltc.
+  0x0000a880 1170ee05 031d000a ff09023f 08163500 .p.........?..5.
+  0x0000a890 0a226c74 1a001170 800701a2 023a7231 ."lt...p.....:r1
+  0x0000a8a0 31820024 342c2000 2a703104 01363135 1..$4, .*p1..615
+  0x0000a8b0 2c210065 313b0a6e 6f741b00 11361500 ,!.e1;.not...6..
+  0x0000a8c0 1135040a 27313605 0a1f3105 0a082f31 .5..'16...1.../1
+  0x0000a8d0 30060a0b 2f313107 0a162a31 31080a2f 0.../11...*11../
+  0x0000a8e0 3132090a 0427332c 7a002f31 320b0a11 12...'3,z./12...
+  0x0000a8f0 2f335d0b 0a5a2f31 310c0a03 1f340c0a /3]..Z/11....4..
+  0x0000a900 0328352c d1001f34 6300041a 360d0a1f .(5,...4c...6...
+  0x0000a910 350d0a2d 06e10002 0d0a0653 080f7f00 5..-.......S....
+  0x0000a920 0103160a 1634e200 2f3136e3 00011336 .....4../16....6
+  0x0000a930 17030be3 0001c303 05e3001f 36640004 ............6d..
+  0x0000a940 11376400 14386400 1d37b709 01c30003 .7d..8d..7......
+  0x0000a950 8b001437 9d0a06e3 00025909 02a00a28 ...7......Y....(
+  0x0000a960 3238e300 02eb0802 40001f33 33020411 28......@..33...
+  0x0000a970 33380026 3335e300 2f3234e3 00011338 38.&35../24....8
+  0x0000a980 330e0be3 0028392c e3001f38 64000411 3....(9,...8d...
+  0x0000a990 38640014 3964001c 39e30002 b209038b 8d..9d..9.......
+  0x0000a9a0 00022d00 1833e300 03ba0914 353c0a07 ..-..3......5<..
+  0x0000a9b0 1a001634 b80b0b99 0a253435 f2020119 ...4.....%45....
+  0x0000a9c0 022c3434 21001c36 750a1d34 44001737 .,44!..6u..4D..7
+  0x0000a9d0 3f020246 000c3a0c 2734389f 01010c00 ?..F..:.'48.....
+  0x0000a9e0 2c343723 001739a2 01026900 0c240b27 ,47#..9...i..$.'
+  0x0000a9f0 35300201 012f001f 34ef0d05 01d20016 50.../..4.......
+  0x0000aa00 35410448 2b33325d 13011135 f8001e35 5A.H+32]...5...5
+  0x0000aa10 eb032235 363a000d ec033635 372c3800 .."56:....657,8.
+  0x0000aa20 0fa70204 1135db00 26353977 003b3430 .....5..&59w.;40
+  0x0000aa30 5dc50011 365b0026 35382e01 1935470c ]...6[.&58...5G.
+  0x0000aa40 22363344 000e8d03 3536342c 40001f36 "63D....564,@..6
+  0x0000aa50 38050411 36a00027 36368200 1d388200 8...6..'66...8..
+  0x0000aa60 015c0026 36356a01 28363482 00223730 .\.&65j.(64.."70
+  0x0000aa70 44000e2c 03353731 2c40001f 37f10404 D..,.571,@..7...
+  0x0000aa80 1137a000 1737f104 2c353682 0011375c .7...7..,56...7\
+  0x0000aa90 00022a00 02cb0219 37910422 37374400 ..*.....7.."77D.
+  0x0000aaa0 0ecb0226 37389f01 0ccc0226 3739d401 ...&78.....&79..
+  0x0000aab0 0261000c 41022738 307c0102 64000c65 .a..A.'80|..d..e
+  0x0000aac0 0d273831 7f010146 002c3830 23001732 .'81...F.,80#..2
+  0x0000aad0 4001014c 002c3831 23001733 43010169 @..L.,81#..3C..i
+  0x0000aae0 001c382c 0f273834 0401016f 001f38d4 ..8,.'84...o..8.
+  0x0000aaf0 01041138 6a001738 d4013836 345d1501 ...8j..8..864]..
+  0x0000ab00 12383f00 01270009 cd022239 303a000d .8?..'...."90:..
+  0x0000ab10 cd023539 312c3800 1f39c901 0411399b ..591,8..9....9.
+  0x0000ab20 001739c9 013b3732 5dc50011 395b0026 ..9..;72]...9[.&
+  0x0000ab30 39322e01 1939c901 22393744 000ecd02 92...9.."97D....
+  0x0000ab40 3639382c 40001f37 82000403 5a071630 698,@..7....Z..0
+  0x0000ab50 83001d38 50032131 305e0026 39396c01 ...8P.!10^.&99l.
+  0x0000ab60 28393884 00213130 6a013e31 3030d102 (98..!10j.>100..
+  0x0000ab70 46313035 2c44002f 31306207 05223036 F105,D./10b.."06
+  0x0000ab80 20001737 8a000d58 031131e2 05042d00  ..7...X..1...-.
+  0x0000ab90 02d80229 31309101 12313208 3e313037 ...)10...12.>107
+  0x0000aba0 db023631 3132ae01 0cdc0236 313133e4 ..6112.....6113.
+  0x0000abb0 0122362c 2f000d24 0017348e 01123725 ."6,/..$..4...7%
+  0x0000abc0 001d3325 00173593 01034a00 1d342500 ..3%..5...J..4%.
+  0x0000abd0 17365401 02c9002d 31352500 18375801 .6T....-15%..7X.
+  0x0000abe0 0370001d 36260018 38150112 3926000f .p..6&..8...9&..
+  0x0000abf0 f1010422 31312000 1732f201 3939365d ..."11 ..2..996]
+  0x0000ac00 26010245 06032a00 1a351b00 13343e00 &..E..*..5...4>.
+  0x0000ac10 0df00212 317b1104 3d001f32 e8010502 ....1{..=..2....
+  0x0000ac20 be112731 32e8014c 3130345d d4000285 ..'12..L104]....
+  0x0000ac30 12042e00 0334000a 8c000251 083e3132 .....4.....Q.>12
+  0x0000ac40 37fb0213 31e61103 46002f33 318d0004 7...1...F./31...
+  0x0000ac50 03851118 335a090e ea131231 9212032e ....3Z.....1....
+  0x0000ac60 00038701 2a33328d 0013384a 000f0203 ....*32...8J....
+  0x0000ac70 00039301 0446000f 9e080412 31a01237 .....F......1..7
+  0x0000ac80 3134318d 001e328d 03026b08 032e0003 141...2...k.....
+  0x0000ac90 03030be7 02037308 2f343103 0300046e ......s./41....n
+  0x0000aca0 081f3004 03022734 37fb0102 2a000d6a ..0...'47...*..j
+  0x0000acb0 0812316b 08049c01 0206030d 6d081231 ..1k........m..1
+  0x0000acc0 6e08049f 0102c201 0d700812 31710804 n........p..1q..
+  0x0000acd0 5b010208 032d3439 26001831 5e010252 [....-49&..1^..R
+  0x0000ace0 002d3530 26001832 1a01027f 002d3531 .-50&..2.....-51
+  0x0000acf0 260008c5 09017100 293530af 01353534 &.....q.)50..554
+  0x0000ad00 2c0c0a2f 34338013 05123380 13032e00 ,../43....3.....
+  0x0000ad10 4d313533 7d690017 35630701 69002a38 M153}i..5c..i.*8
+  0x0000ad20 34690026 362caa07 0fe91306 14356900 4i.&6,.......5i.
+  0x0000ad30 22362c56 000e6900 1837f204 1238c201 "6,V..i..7...8..
+  0x0000ad40 0a830203 9107033f 052f3131 6d000514 .......?./11m...
+  0x0000ad50 376d0002 30002e35 376d0018 395c0203 7m..0..57m..9\..
+  0x0000ad60 27001932 6d003836 302ca902 1f356d00 '..2m.860,...5m.
+  0x0000ad70 0513396d 00033000 263539c5 141f31c5 ..9m..0.&59...1.
+  0x0000ad80 140d1438 8212af54 7269706c 65476174 ...8...TripleGat
+  0x0000ad90 65c41408 0f320012 0ec3140f 3a001c1f e....2......:...
+  0x0000ada0 313a0026 1f323a00 260ff21c 021c31c0 1:.&.2:.&.....1.
+  0x0000adb0 14363630 39ae1402 c0142d32 34c0142f .6609.....-24../
+  0x0000adc0 3332c014 021231f4 130f4001 160f3714 32....1...@...7.
+  0x0000add0 001f3243 001b1f31 0215010f 43001b1f ..2C...1....C...
+  0x0000ade0 32430000 1f344300 1b2f335d 59110523 2C...4C../3]Y..#
+  0x0000adf0 352c2c12 06ae141f 38c41402 1f39f114 5,,.....8....9..
+  0x0000ae00 032f3130 dc140401 bc080136 00247238 ./10.......6.$r8
+  0x0000ae10 e2132e6c 64d91400 3f032d35 5d2d1421 ...ld...?.-5]-.!
+  0x0000ae20 322c2000 072d1425 312c5600 2f31320b 2, ..-.%1,V./12.
+  0x0000ae30 15071f35 c2140001 0f090a0e 1517324e ...5..........2N
+  0x0000ae40 000a1812 23382c9a 00023200 0b4a001d ....#8,...2..J..
+  0x0000ae50 340d1517 334a001f 34980000 14399800 4...3J..4....9..
+  0x0000ae60 2e313699 001d3514 1517344f 001a351a .16...5...4O..5.
+  0x0000ae70 1017309a 001d394b 00133638 10074c00 ..0...9K..68..L.
+  0x0000ae80 17354c00 1a364c00 1731ab15 0e4c0002 .5L..6L..1...L..
+  0x0000ae90 18002731 314c0017 364c001f 37841c01 ..'11L..6L..7...
+  0x0000aea0 0353001d 364d0015 38611305 4d001737 .S..6M..8a..M..7
+  0x0000aeb0 4d001f38 fa15022f 3131fb15 072f3131 M..8.../11.../11
+  0x0000aec0 fc151f2f 3131fd15 201331cb 1f0ffe15 .../11.. .1.....
+  0x0000aed0 1904981f 0cff1501 39001f38 ff150302 ........9..8....
+  0x0000aee0 35001936 35000114 00023b00 2d313037 5..65.....;.-107
+  0x0000aef0 00070801 1a373700 26332c3d 160d0b01 .....77.&3,=....
+  0x0000af00 053a142f 2572d115 081d3337 00020f01 .:./%r....37....
+  0x0000af10 0e420101 2902021f 0001f315 0b370002 .B..)........7..
+  0x0000af20 12010e45 01019409 021f003c 70313737 ...E.......<p177
+  0x0000af30 0001d009 1f724801 00017a14 021f003d .....rH...z....=
+  0x0000af40 70313937 00021401 0e4a0101 c70b021f p197.....J......
+  0x0000af50 003d7032 31370006 13010a4a 0101050c .=p217.....J....
+  0x0000af60 021f003d 70323337 00011301 1e321301 ...=p237.....2..
+  0x0000af70 01d30902 1f003d70 32353700 15383700 ......=p257..87.
+  0x0000af80 0a130101 8b1e021f 002d7032 13012533 .........-p2..%3
+  0x0000af90 3037000a 13010139 0c021f00 2d703213 07.....9....-p2.
+  0x0000afa0 01253332 37000a13 0101a40a 021f003d .%327..........=
+  0x0000afb0 70333137 00153437 000a1301 016a0a02 p317..47.....j..
+  0x0000afc0 1f003d70 33333700 0113011e 33dc0001 ..=p337.....3...
+  0x0000afd0 2e0c021f 002d7033 13012533 3837000b .....-p3..%387..
+  0x0000afe0 dc002439 2c1f003c 70333737 00253430 ..$9,..<p377.%40
+  0x0000aff0 37000adc 0001cf09 021f003d 70333937 7..........=p397
+  0x0000b000 00153237 000adc00 01111502 1f002d70 ..27..........-p
+  0x0000b010 34130101 010a2e72 34a50001 a00c021f 4......r4.......
+  0x0000b020 003d7034 33370015 3637000b a5002437 .=p437..67....$7
+  0x0000b030 2c1f003d 70343537 00153837 000ba500 ,..=p457..87....
+  0x0000b040 24392c1f 003c7034 37370001 810c2e72 $9,..<p477.....r
+  0x0000b050 356e0001 740c021f 003d7034 39370015 5n..t....=p497..
+  0x0000b060 3237000a 6e00015f 0c021f00 3d703531 27..n.._....=p51
+  0x0000b070 370002d7 000f3700 0024352c 1f003e70 7.....7..$5,..>p
+  0x0000b080 3533bb1a 14336c1a 0abd1a01 150c041f 53...3l.........
+  0x0000b090 00296433 be1a0447 080dbe1a 01300c03 .)d3...G.....0..
+  0x0000b0a0 5b1c2a31 39870024 382c2100 3a703536 [.*19..$8,!.:p56
+  0x0000b0b0 1b002639 2c210019 35bf1a01 c10b3170 ..&9,!..5.....1p
+  0x0000b0c0 3539bf1a 273630bf 1a1f32bf 1a091434 59..'60...2....4
+  0x0000b0d0 bf1a2f6c 640f0f00 099f1a00 21100f46 ../ld.......!..F
+  0x0000b0e0 00040184 012f6431 0f19052f 31311019 ...../d1.../11..
+  0x0000b0f0 051e3510 190fc41a 062f375d c41a5b3f ..5....../7]..[?
+  0x0000b100 342b38fe 18061f31 fe18051f 35fe180a 4+8....1....5...
+  0x0000b110 010f0107 c41a0dfe 18012406 048a0002 ..........$.....
+  0x0000b120 b00f0fc4 1a481f34 c41a0323 32304705 .....H.4...#20G.
+  0x0000b130 0ae30001 7c0005e3 001f3246 0104021a ....|.....2F....
+  0x0000b140 1005c41a 2c3231e3 00273331 25190fc4 ....,21..'31%...
+  0x0000b150 1a4e1f34 c41a0314 324e050b e3000062 .N.4....2N.....b
+  0x0000b160 0006e300 0f640005 1938c41a 2f3233c4 .....d...8../23.
+  0x0000b170 1a2d06e3 0002c41a 06f8100f 7f000102 .-..............
+  0x0000b180 5a122634 36e3002f 3332e300 0113348c Z.&46../32....4.
+  0x0000b190 050be300 003e0006 e3000f23 14040239 .....>.....#...9
+  0x0000b1a0 121435a1 141d326d 1d02c211 038b0001 ..5...2m........
+  0x0000b1b0 2d002834 34e30001 46050357 1b0adc11 -.(44...F..W....
+  0x0000b1c0 02931102 40001f35 7f000413 35321a06 ....@..5....52..
+  0x0000b1d0 e3002f34 30e30001 13360106 0be30000 ../40....6......
+  0x0000b1e0 560206e3 000f5d04 0402f210 1436ea13 V.....]......6..
+  0x0000b1f0 1d326d1d 02891a02 8b00022d 00283535 .2m........-.(55
+  0x0000b200 e300021b 1901a805 38663631 e3000212 ........8f61....
+  0x0000b210 19024000 2f36357f 00040238 001738e3 ..@./65....8..8.
+  0x0000b220 000f6f04 01027809 1d36e300 00730106 ..o...x..6...s..
+  0x0000b230 e3000f6f 040402c9 1a1437c2 051d326f ...o......7...2o
+  0x0000b240 041137c3 00028b00 03f61a18 36e30002 ..7.........6...
+  0x0000b250 c21a2236 38470008 e30003bc 1a014000 .."68G........@.
+  0x0000b260 1f376201 0402c61a 263739e3 002f3536 .7b.....&79../56
+  0x0000b270 e3000002 240a1c37 e30001e8 0305e300 ....$..7........
+  0x0000b280 0fec2805 02a61a14 38b5051d 336f0402 ..(.....8...3o..
+  0x0000b290 6918028b 00243832 e71306e3 00353837 i....$82.....587
+  0x0000b2a0 2c551b29 38331a00 1f38501e 0616387e ,U.)83...8P...8~
+  0x0000b2b0 06015f00 1c385415 1839c805 1237861a .._..8T..9...7..
+  0x0000b2c0 0c230008 cb051436 a31a0a23 0017322b .#.....6...#..2+
+  0x0000b2d0 05143878 1a0a2300 1c33501e 1c393119 ..8x..#..3P..91.
+  0x0000b2e0 2739348e 04123917 190c2300 01c80126 '94...9...#....&
+  0x0000b2f0 3335b104 2f393404 1b0202f1 03019109 35../94.........
+  0x0000b300 2c663916 01263937 f4030214 041c39b8 ,f9..&97......9.
+  0x0000b310 16273938 54031431 161b0a23 00173957 .'98T..1...#..9W
+  0x0000b320 031430e9 1a092300 038d1903 b8021232 ..0...#........2
+  0x0000b330 c5190d24 001731bc 0222312c 37000d25 ...$..1.."1,7..%
+  0x0000b340 0017321e 02123325 000fa918 05053e1b ..2...3%......>.
+  0x0000b350 06d0020b a21c03ff 15032a00 0b980826 ..........*....&
+  0x0000b360 382ca61b 0a9b0838 30392c3d 000f3c08 8,.....809,=..<.
+  0x0000b370 0502db08 36313131 80000eab 1c031e1b ....6111........
+  0x0000b380 042d0002 43081a30 7f180153 03004900 .-..C..0...S..I.
+  0x0000b390 0e460803 131b0546 000fbd04 0404151b .F.....F........
+  0x0000b3a0 1731bf04 0fb41c00 03ae0826 31379e02 .1.........&17..
+  0x0000b3b0 013b1b07 8c0002b7 08033f1b 0aef0705 .;........?.....
+  0x0000b3c0 c71a0246 000f8e07 0505101b 07f4070f ...F............
+  0x0000b3d0 b61c0002 40032731 3295073a 3132338c ....@.'12..:123.
+  0x0000b3e0 00133949 000e9807 050c1b03 46000f91 ..9I........F...
+  0x0000b3f0 21040410 1b163335 0b02da1b 0a8c0002 !.....35........
+  0x0000b400 6903032d 00022a03 39313330 8c000175 i..-..*.9130...u
+  0x0000b410 0e04441b 0b1d1904 0b1b0346 000f7e05 ..D........F..~.
+  0x0000b420 04050f1b 0780050f e61b0102 6d08032e ............m...
+  0x0000b430 00027103 39313337 8d0002b0 0803441b ..q.9137......D.
+  0x0000b440 0aeb0605 62180246 000fb408 05050f1b ....b..F........
+  0x0000b450 07b6080e e61b05b1 1a273435 b6030a59 .........'45...Y
+  0x0000b460 0804ae1a 2e343695 0604a41a 0346002f .....46......F./
+  0x0000b470 35308d00 04243532 301a068d 000fe61b 50...$520.......
+  0x0000b480 0002a704 032e0002 3c0601cc 1a088d00 ........<.......
+  0x0000b490 02f7192e 35333f06 283135f2 030c4206 ....53?.(15...B.
+  0x0000b4a0 04c41902 2b040369 000de804 283630cd ....+..i....(60.
+  0x0000b4b0 03036c00 0dea0402 490504d0 0302f303 ..l.....I.......
+  0x0000b4c0 1d36eb04 02522304 8d0302e6 1b2d3631 .6...R#......-61
+  0x0000b4d0 26001833 90030272 001d3683 1f02db08 &..3...r..6.....
+  0x0000b4e0 27313254 063d3136 33260018 35500303 '12T.=163&..5P..
+  0x0000b4f0 72000d85 1f022d09 030d0302 5a063d31 r.....-.....Z.=1
+  0x0000b500 36352600 17371003 03e0012d 36362600 65&..7.....-66&.
+  0x0000b510 1838cc02 0310010d 161d02da 2304cf02 .8..........#...
+  0x0000b520 02f2021d 367c0128 37308b02 023d011d ....6|.(70...=..
+  0x0000b530 367c0128 37318e02 020d002d 37302600 6|.(71.....-70&.
+  0x0000b540 18324a02 0263012f 37319e02 04133720 .2J..c./71....7 
+  0x0000b550 0008a70d 3932385d 5c02027f 092f3137 ....928]\..../17
+  0x0000b560 69060002 cd062f31 37690600 02e60805 i...../17i......
+  0x0000b570 3d000f69 06050240 24273138 69062e31 =..i...@$'18i..1
+  0x0000b580 33c60402 db232831 386a061a 376a0602 3....#(18j..7j..
+  0x0000b590 c9211231 6e240b6a 06029909 0546000f .!.1n$.j.....F..
+  0x0000b5a0 6a060502 a0092731 386a062e 3134c604 j.....'18j..14..
+  0x0000b5b0 034e0927 3837b802 1a386b06 0332221f .N.'87...8k..2".
+  0x0000b5c0 386b0601 03292203 46002f39 328d0004 8k...)".F./92...
+  0x0000b5d0 024b0927 31396b06 2e3135c6 0402e608 .K.'19k..15.....
+  0x0000b5e0 2831396c 062a3933 8d001339 4a000e6c (19l.*93...9J..l
+  0x0000b5f0 061232de 08054600 0f6c0604 1232e108 ..2...F..l...2..
+  0x0000b600 38323032 cf0f0dc6 041232fc 23273230 8202......2.#'20
+  0x0000b610 6d063832 30308d00 1232b622 2f32306d m.8200...2."/20m
+  0x0000b620 06001232 96080546 000f6d06 041232df ...2...F..m...2.
+  0x0000b630 08283230 6d061d36 86071232 120b032e .(20m..6...2....
+  0x0000b640 00027b03 2932306d 06123212 0b2f3230 ..{.)20m..2../20
+  0x0000b650 6d060012 32970804 46002f31 338d0004 m...2...F./13...
+  0x0000b660 02e10828 32316d06 1d37c102 1132b411 ...(21m..7...2..
+  0x0000b670 042e0002 bc033932 31348d00 0450110f ......9214...P..
+  0x0000b680 6d060012 32980804 46000f10 110602e2 m...2...F.......
+  0x0000b690 08283232 6d061d38 c1021132 cc0e042e .(22m..8...2....
+  0x0000b6a0 00026d06 3a323231 8d001337 4a000e6d ..m.:221...7J..m
+  0x0000b6b0 06283232 f6030c6d 06373232 392f0403 .(22...m.7229/..
+  0x0000b6c0 69000cf1 04383233 30d00303 6c001d39 i....8230...l..9
+  0x0000b6d0 26001831 d303024c 002d3330 26001832 &..1...L.-30&..2
+  0x0000b6e0 8f031238 26001d31 26001833 9203022c ...8&..1&..3...,
+  0x0000b6f0 002d3332 26001834 4e03026e 012d3333 .-32&..4N..n.-33
+  0x0000b700 26001835 51030372 001d3426 0017360d &..5Q..r..4&..6.
+  0x0000b710 03026d06 3d323335 26001737 10030333 ..m.=235&..7...3
+  0x0000b720 032d3336 26001838 cc021231 26001d37 .-36&..8...1&..7
+  0x0000b730 26001839 cf020372 000d7c01 2834308b &..9...r..|.(40.
+  0x0000b740 02123226 000d7c01 2834318e 02020d00 ..2&..|.(41.....
+  0x0000b750 2d343026 0018324a 02123326 000f6d06 -40&..2J..3&..m.
+  0x0000b760 04233234 2000086d 06393932 5d5c0202 .#24 ..m.992]\..
+  0x0000b770 91242e32 346d0632 3234381b 000e6d06 .$.24m.2248...m.
+  0x0000b780 13323801 043d000f 6d060413 32850117 .28..=..m...2...
+  0x0000b790 356d062e 3230c604 02501203 2e000377 5m..20...P.....w
+  0x0000b7a0 02293439 8c000259 122f3235 6d060012 .)49...Y./25m...
+  0x0000b7b0 32cb0905 46000f6d 06041232 cf093832 2...F..m...2..82
+  0x0000b7c0 35388d00 0ec60403 ed012735 37b80229 58........'57..)
+  0x0000b7d0 35368d00 026e092f 32356d06 00123264 56...n./25m...2d
+  0x0000b7e0 09044600 2f36328d 00040265 09273236 ..F./62....e.'26
+  0x0000b7f0 6d063e32 31368d00 02630027 3634f902 m.>216...c.'64..
+  0x0000b800 2a36338d 0013394a 000f6d06 0002e708 *63...9J..m.....
+  0x0000b810 0546000f 6d060503 6e022737 328d002d .F..m...n.'72..-
+  0x0000b820 32348d00 02111228 32376d06 2937308d 24.....(27m.)70.
+  0x0000b830 00025412 2f32376d 0601029a 08054600 ..T./27m......F.
+  0x0000b840 0f6d0605 02e30818 325a123d 3233328d .m......2Z.=232.
+  0x0000b850 00034605 2737387b 030afd11 13321f03 ..F.'78{.....2..
+  0x0000b860 1f376d06 01029a08 0446002f 38338d00 .7m......F./83..
+  0x0000b870 0402e408 37323836 8d000e10 2f123233 ....7286..../.23
+  0x0000b880 12283238 6d062938 348d0002 35122f32 .(28m.)84...5./2
+  0x0000b890 386d0601 029a0804 46000fcd 2c051332 8m......F...,..2
+  0x0000b8a0 32122839 338d000e c10202cd 11283239 2.(93........(29
+  0x0000b8b0 6d060ad3 2c1232cd 112f3239 6d060102 m...,.2../29m...
+  0x0000b8c0 9a082f32 346d0603 02db0827 32346d06 ../24m.....'24m.
+  0x0000b8d0 0dc21112 33e40828 32356d06 0dc41112 ....3..(25m.....
+  0x0000b8e0 33a80527 32356d06 1d33c511 1233a805 3..'25m..3...3..
+  0x0000b8f0 2732356d 063d3330 31260018 33920312 '25m.=301&..3...
+  0x0000b900 3726001d 32260018 344e0312 3926001d 7&..2&..4N..9&..
+  0x0000b910 33260018 35510303 72001d34 26001736 3&..5Q..r..4&..6
+  0x0000b920 0d0302ea 003d3330 35260017 37100302 .....=305&..7...
+  0x0000b930 33033d33 30362600 1838cc02 12312600 3.=306&..8...1&.
+  0x0000b940 1d372600 1839cf02 0372000d 7c01024f .7&..9...r..|..O
+  0x0000b950 0e273238 6d063d33 30392600 18318e02 .'28m.=309&..1..
+  0x0000b960 0272002d 31302600 18324a02 12332600 .r.-10&..2J..3&.
+  0x0000b970 0f6d0604 23333120 00076d06 15321316 .m..#31 ..m..2..
+  0x0000b980 025c0212 330c022e 33316d06 1233950e .\..3...31m..3..
+  0x0000b990 2e33316d 06123385 09053d00 0f6d0604 .31m..3...=..m..
+  0x0000b9a0 1233cf09 2833326d 0601c413 0ad50003 .3..(32m........
+  0x0000b9b0 d80e2732 30770229 31398c00 03d50e1f ..'20w.)19......
+  0x0000b9c0 326d0600 1233cb09 0546000f 6d060413 2m...3...F..m...
+  0x0000b9d0 33840227 32388d00 0ed11312 33710903 3..'28......3q..
+  0x0000b9e0 2e000434 00096d06 12336e09 2f33326d ...4..m..3n./32m
+  0x0000b9f0 06001333 351b0346 000f371b 06031f16 ...35..F..7.....
+  0x0000ba00 09391b0e d2131333 ec022733 34f9020a .9.....3..'34...
+  0x0000ba10 dc1a1333 35031f33 6d060012 33e70805 ...35..3m...3...
+  0x0000ba20 46000f6d 06041233 e8082833 346d060e F..m...3..(34m..
+  0x0000ba30 d3131233 9b0f032e 00033a03 2934308d ...3......:.)40.
+  0x0000ba40 0002980f 2f33346d 06001233 9a080546 ..../34m...3...F
+  0x0000ba50 000f6d06 041233e3 08283334 6d060ed4 ..m...3..(34m...
+  0x0000ba60 131233dc 0f032e00 037b0329 34378d00 ..3......{.)47..
+  0x0000ba70 0226122f 33346d06 0012339a 08044600 .&./34m...3...F.
+  0x0000ba80 2f35338d 000402e4 08273335 6d061e33 /53......'35m..3
+  0x0000ba90 d4131233 5d12032e 0003bc03 2935348d ...3].......)54.
+  0x0000baa0 0003a300 1f356d06 00133360 04034600 .....5m...3`..F.
+  0x0000bab0 2f36308d 000402e4 08273336 6d061e33 /60......'36m..3
+  0x0000bac0 d4131233 e1112733 366d063a 3336318d ...3..'36m.:361.
+  0x0000bad0 0013374a 000e6d06 12339a08 2f33316d ..7J..m..3../31m
+  0x0000bae0 06021233 db082633 316d061d 33cb1112 ...3..&31m..3...
+  0x0000baf0 33e40827 33326d06 1d33cb11 38333731 3..'32m..3..8371
+  0x0000bb00 d303024c 000dcb11 38333732 8f03029c ...L....8372....
+  0x0000bb10 002d3731 26001833 92030272 002d3732 .-71&..3...r.-72
+  0x0000bb20 26001834 4e0302ca 001d376d 06020e09 &..4N.....7m....
+  0x0000bb30 2833336d 061d376d 06025709 2833346d (33m..7m..W.(34m
+  0x0000bb40 061d372f 01026109 2833346d 062d3736 ..7/..a.(34m.-76
+  0x0000bb50 26001838 cc021231 26000d6d 06026606 &..8...1&..m..f.
+  0x0000bb60 2833346d 060d8c36 38333830 8b02023d (34m...68380...=
+  0x0000bb70 012d3739 26001831 8e02020d 000d9236 .-79&..1.......6
+  0x0000bb80 38333832 4a020263 012f3831 9e020404 8382J..c./81....
+  0x0000bb90 20001834 281f2930 5d5c0202 a00e2f33  ..4(.)0]\..../3
+  0x0000bba0 386d0600 02950e2f 33386d06 00028509 8m...../38m.....
+  0x0000bbb0 053d000f 6d060502 cf093833 39318100 .=..m.....8391..
+  0x0000bbc0 0ec60404 d80e1730 77022938 398c0004 .......0w.)89...
+  0x0000bbd0 26120f6d 060102cb 09054600 0f6d0605 &..m......F..m..
+  0x0000bbe0 02cf0927 33396d06 1e33d413 12347109 ...'39m..3...4q.
+  0x0000bbf0 032e0003 b8022839 368d0012 346e092f ......(96...4n./
+  0x0000bc00 33396d06 00123464 09034600 3f343032 39m...4d..F.?402
+  0x0000bc10 8d000312 34650927 34306d06 1e33d413 ....4e.'40m..3..
+  0x0000bc20 1234f408 032e0013 330d0009 1d041234 .4......3......4
+  0x0000bc30 f1081234 90090a6d 061234e7 08054600 ...4...m..4...F.
+  0x0000bc40 0f6d0604 1234e808 2734316d 061e33d4 .m...4..'41m..3.
+  0x0000bc50 1312349b 0f273431 6d063934 31308d00 ..4..'41m.9410..
+  0x0000bc60 02bd012f 34316d06 00123476 04054600 .../41m...4v..F.
+  0x0000bc70 0f6d0604 1234e308 2734316d 061e33d4 .m...4..'41m..3.
+  0x0000bc80 131234dc 0f032e00 027b0339 3431378d ..4......{.9417.
+  0x0000bc90 00022612 2f34316d 06001234 9a080446 ..&./41m...4...F
+  0x0000bca0 002f3233 8d000402 e4083834 32368d00 ./23......8426..
+  0x0000bcb0 0dc10212 345d1227 34326d06 39343234 ....4].'42m.9424
+  0x0000bcc0 8d00025b 122f3432 6d060012 349a0804 ...[./42m...4...
+  0x0000bcd0 46002f33 308d0004 02e40837 3433338d F./30......7433.
+  0x0000bce0 000ed413 1234e111 2734336d 063a3433 .....4..'43m.:43
+  0x0000bcf0 318d0013 374a000e 6d062834 33f6030c 1...7J..m.(43...
+  0x0000bd00 6d063734 33392f04 0369000c f1043834 m.7439/..i....84
+  0x0000bd10 3430d003 036c001d 39260018 31d30302 40...l..9&..1...
+  0x0000bd20 4c000dcb 111234a8 05273339 6d063d34 L.....4..'39m.=4
+  0x0000bd30 34312600 18339203 0272002d 34322600 41&..3...r.-42&.
+  0x0000bd40 18344e03 026e012d 34332600 18355103 .4N..n.-43&..5Q.
+  0x0000bd50 0372001d 34260017 360d0302 6d063d34 .r..4&..6...m.=4
+  0x0000bd60 34352600 17371003 0333030d ca361234 45&..7...3...6.4
+  0x0000bd70 66062734 316d063d 34343726 001839cf f.'41m.=447&..9.
+  0x0000bd80 02037200 0d7c0128 35308b02 0278002d ..r..|.(50...x.-
+  0x0000bd90 34392600 18318e02 020d002d 35302600 49&..1.....-50&.
+  0x0000bda0 18324a02 12332600 0f6d0604 23343520 .2J..3&..m..#45 
+  0x0000bdb0 00086d06 01e51507 5c0202a0 0e2e3435 ..m.....\.....45
+  0x0000bdc0 6d061234 950e2e34 356d0612 34850905 m..4...45m..4...
+  0x0000bdd0 3d000f6d 06041334 13012736 31810001 =..m...4..'61...
+  0x0000bde0 c8130ad5 0002d80e 032e0003 77022935 ............w.)5
+  0x0000bdf0 398c0002 d50e2f34 366d0600 1234cb09 9...../46m...4..
+  0x0000be00 0546000f 6d060412 34cf0919 34dd240e .F..m...4...4.$.
+  0x0000be10 d4131334 7b012736 37b8020a 80241334 ...4{.'67....$.4
+  0x0000be20 c4011f36 6d060102 64090446 002f3732 ...6m...d..F./72
+  0x0000be30 8d000402 65093834 37358d00 0ec60402 ....e.8475......
+  0x0000be40 f408032e 0003f902 2a37338d 0013394a ........*73...9J
+  0x0000be50 000f6d06 0002e708 0546000f 6d060502 ..m......F..m...
+  0x0000be60 e8082734 386d061e 34d41312 349b0f28 ..'48m..4...4..(
+  0x0000be70 34386d06 2938308d 0002980f 2f34386d 48m.)80...../48m
+  0x0000be80 0601029a 08054600 0f6d0605 02e30827 ......F..m.....'
+  0x0000be90 34386d06 1e34d413 1234dc0f 032e0003 48m..4...4......
+  0x0000bea0 7b031a38 6d060226 122f3438 6d060102 {..8m..&./48m...
+  0x0000beb0 9a080446 002f3933 8d000402 e4082734 ...F./93......'4
+  0x0000bec0 396d061e 34d41312 345d1228 34396d06 9m..4...4].(49m.
+  0x0000bed0 2839348d 0012355b 122f3439 6d060013 (94...5[./49m...
+  0x0000bee0 359a0802 46003f35 30308d00 031235e4 5...F.?500....5.
+  0x0000bef0 08273530 6d061e34 d4131235 e1112735 .'50m..4...5..'5
+  0x0000bf00 306d063a 3530318d 00123716 000f6d06 0m.:501...7...m.
+  0x0000bf10 00283530 f6030c6d 06373530 392f0403 .(50...m.7509/..
+  0x0000bf20 69000cf1 04383531 30d00303 6c001d39 i....8510...l..9
+  0x0000bf30 26001831 d303024c 000dcb11 38353132 &..1...L....8512
+  0x0000bf40 8f031238 26001d31 26001833 92030272 ...8&..1&..3...r
+  0x0000bf50 002d3132 26001834 4e03026e 012d3133 .-12&..4N..n.-13
+  0x0000bf60 26001835 51030372 001d3426 0017360d &..5Q..r..4&..6.
+  0x0000bf70 0302e205 3d353135 26001737 10030233 ....=515&..7...3
+  0x0000bf80 033d3531 36260018 38cc0202 52002d31 .=516&..8...R.-1
+  0x0000bf90 37260018 39cf0203 72000d7c 01024f0e 7&..9...r..|..O.
+  0x0000bfa0 2734396d 063d3531 39260018 318e0202 '49m.=519&..1...
+  0x0000bfb0 72002d32 30260018 324a0212 3326000f r.-20&..2J..3&..
+  0x0000bfc0 6d060423 35322000 18349e02 29385d5c m..#52 ..4..)8]\
+  0x0000bfd0 02039a01 1e326d06 1335db01 1e326d06 .....2m..5...2m.
+  0x0000bfe0 12358509 053d000f 6d060412 35cf0927 .5...=..m...5..'
+  0x0000bff0 35336d06 1134c813 0ad50002 d80e032e 53m..4..........
+  0x0000c000 00037702 2932398c 0002d50e 2f35336d ..w.)29...../53m
+  0x0000c010 06001235 cb090546 000f6d06 041235cf ...5...F..m...5.
+  0x0000c020 09283533 6d060ed4 13133519 0f273337 .(53m.....5..'37
+  0x0000c030 b8022933 368d0002 6e092f35 336d0600 ..)36...n./53m..
+  0x0000c040 12356409 0446002f 34328d00 04031317 .5d..F./42......
+  0x0000c050 18346d06 0ed41312 35f40803 2e0003f9 .4m.....5.......
+  0x0000c060 022a3433 8d001339 4a000e6d 06133505 .*43...9J..m..5.
+  0x0000c070 03044600 0f6d0604 1235e808 37353532 ..F..m...5..7552
+  0x0000c080 8d000ed4 1312359b 0f032e00 03770029 ......5......w.)
+  0x0000c090 35308d00 02980f2f 35356d06 0012359a 50...../55m...5.
+  0x0000c0a0 08054600 0f6d0604 1235e308 38353539 ..F..m...5..8559
+  0x0000c0b0 8d000d87 071235dc 0f032e00 037b030a ......5......{..
+  0x0000c0c0 3a481235 26122f35 356d0600 12359a08 :H.5&./55m...5..
+  0x0000c0d0 0446002f 36338d00 0402e408 37353636 .F./63......7566
+  0x0000c0e0 8d000ed4 1312355d 12032e00 03bc030a ......5]........
+  0x0000c0f0 45481235 5b122f35 366d0601 04320002 EH.5[./56m...2..
+  0x0000c100 46002f37 308d0004 033b0406 4c483e34 F./70....;..LH>4
+  0x0000c110 2b35d413 1235e111 2835376d 062a3731 +5...5..(57m.*71
+  0x0000c120 8d001337 4a000f6d 0600029a 082f3532 ...7J..m...../52
+  0x0000c130 6d060302 db082735 326d060d cb111235 m.....'52m.....5
+  0x0000c140 e4082835 336d060d cb113835 3831d303 ..(53m....8581..
+  0x0000c150 024c000d cb113835 38328f03 029c000d .L....8582......
+  0x0000c160 60483835 38339203 0272000d 63483835 `H8583...r..cH85
+  0x0000c170 38344e03 02ca002d 38332600 18355103 84N....-83&..5Q.
+  0x0000c180 0372000d 6d060257 09030d03 0368032d .r..m..W.....h.-
+  0x0000c190 38352600 17371003 0333032d 38362600 85&..7...3.-86&.
+  0x0000c1a0 1838cc02 0252002d 38372600 1839cf02 .8...R.-87&..9..
+  0x0000c1b0 0372000d 7c012839 308b0202 3d010d53 .r..|.(90...=..S
+  0x0000c1c0 2e383539 318e0202 0d000d56 2e12358b .8591......V..5.
+  0x0000c1d0 09283537 6d060d59 2e373539 33192f12 .(57m..Y.7593./.
+  0x0000c1e0 32ad280a e0022639 34ca472f 3837cf42 2.(...&94.G/87.B
+  0x0000c1f0 0c032e00 2d3539a5 43123542 07044529 ....-59.C.5B..E)
+  0x0000c200 026b000b 4b03023f 07059229 1f37cf42 .k..K..?...).7.B
+  0x0000c210 0c033000 2d3539a9 43293539 45231232 ..0.-59.C)59E#.2
+  0x0000c220 ab1c0b6d 0028382c 92230f6d 00052432 ...m.(8,.#.m..$2
+  0x0000c230 316d0022 382c5a00 0e6d0018 39451d12 1m."8,Z..m..9E..
+  0x0000c240 32ab1609 6d001336 091d0492 1d0f6d00 2...m..6......m.
+  0x0000c250 0603ec44 0330003c 3539396d 001236dc ...D.0.<599m..6.
+  0x0000c260 0a283336 6d001b38 6d002832 2c92170f .(36m..8m.(2,...
+  0x0000c270 6d000603 f0440330 002d3630 40593836 m....D.0.-60@Y86
+  0x0000c280 30334511 1232ab0a 0b6d0028 342c9211 03E..2...m.(4,..
+  0x0000c290 0f6d0006 03210203 30002d36 30210212 .m...!..0.-60!..
+  0x0000c2a0 368e1027 35306d00 2b35326d 0028362c 6..'50m.+52m.(6,
+  0x0000c2b0 920b0f6d 00060321 02033000 2d363021 ...m...!..0.-60!
+  0x0000c2c0 02293630 4505026d 001b396d 0028382c .)60E..m..9m.(8,
+  0x0000c2d0 92050f6d 00051333 21020330 00363630 ...m...3!..0.660
+  0x0000c2e0 375d4515 325d4550 0a7d0a0a 00000000 7]E.2]EP.}......
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,31 +1,31 @@
 
 Hex dump of section '.eh_frame_hdr':
-  0x0000c2c0 011b033b bc010000 36000000 605dffff ...;....6...`]..
-  0x0000c2d0 d8010000 5061ffff 00020000 9061ffff ....Pa.......a..
-  0x0000c2e0 18020000 7065ffff cc070000 f066ffff ....pe.......f..
-  0x0000c2f0 30020000 0067ffff 44020000 1067ffff 0....g..D....g..
-  0x0000c300 58020000 3067ffff 6c020000 5067ffff X...0g..l...Pg..
-  0x0000c310 80020000 7067ffff 94020000 9067ffff ....pg.......g..
-  0x0000c320 a8020000 b067ffff bc020000 d067ffff .....g.......g..
-  0x0000c330 d0020000 f067ffff e4020000 1068ffff .....g.......h..
-  0x0000c340 f8020000 8068ffff 18030000 f068ffff .....h.......h..
-  0x0000c350 38030000 6069ffff 58030000 e069ffff 8...`i..X....i..
-  0x0000c360 70030000 506affff 88030000 c06affff p...Pj.......j..
-  0x0000c370 a4030000 006bffff b8030000 506bffff .....k......Pk..
-  0x0000c380 cc030000 c06bffff ec030000 006cffff .....k.......l..
-  0x0000c390 00040000 406cffff 14040000 806cffff ....@l.......l..
-  0x0000c3a0 28040000 506dffff 48040000 206effff (...Pm..H... n..
-  0x0000c3b0 68040000 f06effff 88040000 406fffff h....n......@o..
-  0x0000c3c0 9c040000 c06fffff b0040000 6071ffff .....o......`q..
-  0x0000c3d0 c4040000 1073ffff d8040000 c074ffff .....s.......t..
-  0x0000c3e0 ec040000 7076ffff 00050000 2078ffff ....pv...... x..
-  0x0000c3f0 14050000 9078ffff 28050000 e078ffff .....x..(....x..
-  0x0000c400 40050000 107affff 54050000 407affff @....z..T...@z..
-  0x0000c410 68050000 a07affff a4050000 d07affff h....z.......z..
-  0x0000c420 b8050000 e07cffff cc050000 b07fffff .....|..........
-  0x0000c430 1c060000 b080ffff 48060000 c080ffff ........H.......
-  0x0000c440 5c060000 7086ffff ac060000 7087ffff \...p.......p...
-  0x0000c450 d8060000 8087ffff ec060000 608cffff ............`...
-  0x0000c460 3c070000 608dffff 68070000 708dffff <...`...h...p...
-  0x0000c470 7c070000 d091ffff 18080000          |...........
+  0x0000c2f0 011b033b bc010000 36000000 305dffff ...;....6...0]..
+  0x0000c300 d8010000 3061ffff 00020000 7061ffff ....0a......pa..
+  0x0000c310 18020000 6065ffff cc070000 e066ffff ....`e.......f..
+  0x0000c320 30020000 f066ffff 44020000 0067ffff 0....f..D....g..
+  0x0000c330 58020000 2067ffff 6c020000 4067ffff X... g..l...@g..
+  0x0000c340 80020000 6067ffff 94020000 8067ffff ....`g.......g..
+  0x0000c350 a8020000 a067ffff bc020000 c067ffff .....g.......g..
+  0x0000c360 d0020000 e067ffff e4020000 0068ffff .....g.......h..
+  0x0000c370 f8020000 7068ffff 18030000 e068ffff ....ph.......h..
+  0x0000c380 38030000 5069ffff 58030000 d069ffff 8...Pi..X....i..
+  0x0000c390 70030000 406affff 88030000 b06affff p...@j.......j..
+  0x0000c3a0 a4030000 f06affff b8030000 406bffff .....j......@k..
+  0x0000c3b0 cc030000 b06bffff ec030000 f06bffff .....k.......k..
+  0x0000c3c0 00040000 306cffff 14040000 706cffff ....0l......pl..
+  0x0000c3d0 28040000 406dffff 48040000 106effff (...@m..H....n..
+  0x0000c3e0 68040000 e06effff 88040000 306fffff h....n......0o..
+  0x0000c3f0 9c040000 b06fffff b0040000 5071ffff .....o......Pq..
+  0x0000c400 c4040000 0073ffff d8040000 b074ffff .....s.......t..
+  0x0000c410 ec040000 6076ffff 00050000 1078ffff ....`v.......x..
+  0x0000c420 14050000 8078ffff 28050000 d078ffff .....x..(....x..
+  0x0000c430 40050000 007affff 54050000 307affff @....z..T...0z..
+  0x0000c440 68050000 907affff a4050000 c07affff h....z.......z..
+  0x0000c450 b8050000 d07cffff cc050000 b07fffff .....|..........
+  0x0000c460 1c060000 b080ffff 48060000 c080ffff ........H.......
+  0x0000c470 5c060000 7086ffff ac060000 7087ffff \...p.......p...
+  0x0000c480 d8060000 8087ffff ec060000 808cffff ................
+  0x0000c490 3c070000 808dffff 68070000 908dffff <.......h.......
+  0x0000c4a0 7c070000 f091ffff 18080000          |...........
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,106 +1,106 @@
 
 Hex dump of section '.eh_frame':
-  0x0000c480 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x0000c490 1b0c0708 90010000 24000000 1c000000 ........$.......
-  0x0000c4a0 805bffff f0030000 000e1046 0e184a0f .[.........F..J.
-  0x0000c4b0 0b770880 003f1a3a 2a332422 00000000 .w...?.:*3$"....
-  0x0000c4c0 14000000 44000000 485fffff 40000000 ....D...H_..@...
-  0x0000c4d0 00000000 00000000 14000000 5c000000 ............\...
-  0x0000c4e0 705fffff e0030000 00000000 00000000 p_..............
-  0x0000c4f0 10000000 74000000 b864ffff 09000000 ....t....d......
-  0x0000c500 00000000 10000000 88000000 b464ffff .............d..
-  0x0000c510 10000000 00000000 10000000 9c000000 ................
-  0x0000c520 b064ffff 1b000000 00000000 10000000 .d..............
-  0x0000c530 b0000000 bc64ffff 1a000000 00000000 .....d..........
-  0x0000c540 10000000 c4000000 c864ffff 1b000000 .........d......
-  0x0000c550 00000000 10000000 d8000000 d464ffff .............d..
-  0x0000c560 1b000000 00000000 10000000 ec000000 ................
-  0x0000c570 e064ffff 1b000000 00000000 10000000 .d..............
-  0x0000c580 00010000 ec64ffff 1b000000 00000000 .....d..........
-  0x0000c590 10000000 14010000 f864ffff 1b000000 .........d......
-  0x0000c5a0 00000000 10000000 28010000 0465ffff ........(....e..
-  0x0000c5b0 1a000000 00000000 1c000000 3c010000 ............<...
-  0x0000c5c0 1065ffff 65000000 00450e10 8302470e .e..e....E....G.
-  0x0000c5d0 2002570e 10410e08 1c000000 5c010000  .W..A......\...
-  0x0000c5e0 6065ffff 6e000000 00450e10 8302470e `e..n....E....G.
-  0x0000c5f0 2002600e 10410e08 1c000000 7c010000  .`..A......|...
-  0x0000c600 b065ffff 62000000 00450e10 8302470e .e..b....E....G.
-  0x0000c610 2002540e 10410e08 14000000 9c010000  .T..A..........
-  0x0000c620 0066ffff 74000000 0002510e 20620e08 .f..t.....Q. b..
-  0x0000c630 14000000 b4010000 6866ffff 69000000 ........hf..i...
-  0x0000c640 0002490e 205f0e08 18000000 cc010000 ..I. _..........
-  0x0000c650 c066ffff 66000000 00640e20 700a0e08 .f..f....d. p...
-  0x0000c660 410b0000 10000000 e8010000 1467ffff A............g..
-  0x0000c670 37000000 00000000 10000000 fc010000 7...............
-  0x0000c680 4067ffff 45000000 00000000 1c000000 @g..E...........
-  0x0000c690 10020000 7c67ffff 6d000000 00450e10 ....|g..m....E..
-  0x0000c6a0 8302470e 20025f0e 10410e08 10000000 ..G. ._..A......
-  0x0000c6b0 30020000 cc67ffff 37000000 00000000 0....g..7.......
-  0x0000c6c0 10000000 44020000 f867ffff 37000000 ....D....g..7...
-  0x0000c6d0 00000000 10000000 58020000 2468ffff ........X...$h..
-  0x0000c6e0 3e000000 00000000 1c000000 6c020000 >...........l...
-  0x0000c6f0 5068ffff c9000000 00450e10 8302470e Ph.......E....G.
-  0x0000c700 2002bb0e 10410e08 1c000000 8c020000  ....A..........
-  0x0000c710 0069ffff cc000000 00450e10 8302470e .i.......E....G.
-  0x0000c720 2002be0e 10410e08 1c000000 ac020000  ....A..........
-  0x0000c730 b069ffff c6000000 00450e10 8302470e .i.......E....G.
-  0x0000c740 2002b80e 10410e08 10000000 cc020000  ....A..........
-  0x0000c750 606affff 45000000 00000000 10000000 `j..E...........
-  0x0000c760 e0020000 9c6affff 73000000 00000000 .....j..s.......
-  0x0000c770 10000000 f4020000 086bffff 94010000 .........k......
-  0x0000c780 00000000 10000000 08030000 946cffff .............l..
-  0x0000c790 a2010000 00000000 10000000 1c030000 ................
-  0x0000c7a0 306effff a2010000 00000000 10000000 0n..............
-  0x0000c7b0 30030000 cc6fffff a2010000 00000000 0....o..........
-  0x0000c7c0 10000000 44030000 6871ffff a2010000 ....D...hq......
-  0x0000c7d0 00000000 10000000 58030000 0473ffff ........X....s..
-  0x0000c7e0 69000000 00000000 14000000 6c030000 i...........l...
-  0x0000c7f0 6073ffff 45000000 00480e20 7c0e0800 `s..E....H. |...
-  0x0000c800 10000000 84030000 9873ffff 26010000 .........s..&...
-  0x0000c810 00000000 10000000 98030000 b474ffff .............t..
-  0x0000c820 2f000000 00000000 38000000 ac030000 /.......8.......
-  0x0000c830 d074ffff 52000000 004d0e10 8c02460e .t..R....M....F.
-  0x0000c840 18860344 0e208304 620a0e18 460e1042 ...D. ..b...F..B
-  0x0000c850 0e08470b 410e1843 0e10420e 0841c3c6 ..G.A..C..B..A..
-  0x0000c860 cc000000 10000000 e8030000 f474ffff .............t..
-  0x0000c870 21000000 00000000 10000000 fc030000 !...............
-  0x0000c880 1075ffff 0e020000 00000000 4c000000 .u..........L...
-  0x0000c890 10040000 0c77ffff c3020000 00460e10 .....w.......F..
-  0x0000c8a0 8f024c0e 188e034e 0e208d04 420e288c ..L....N. ..B.(.
-  0x0000c8b0 054b0e30 86064b0e 38830747 0eb00203 .K.0..K.8..G....
-  0x0000c8c0 4b020a0e 38410e30 410e2842 0e20420e K...8A.0A.(B. B.
-  0x0000c8d0 18420e10 420e0844 0b000000 28000000 .B..B..D....(...
-  0x0000c8e0 60040000 8c79ffff fb000000 004b0eb0 `....y.......K..
-  0x0000c8f0 0102a30e b8014b0e c001610e b801410e ......K...a...A.
-  0x0000c900 b0015a0a 0e08410b 10000000 8c040000 ..Z...A.........
-  0x0000c910 607affff 09000000 00000000 4c000000 `z..........L...
-  0x0000c920 a0040000 5c7affff a4050000 00460e10 ....\z.......F..
-  0x0000c930 8f02420e 188e0348 0e208d04 4c0e288c ..B....H. ..L.(.
-  0x0000c940 05410e30 8606440e 3883074e 0e900203 .A.0..D.8..N....
-  0x0000c950 3f030a0e 38440e30 410e2842 0e20420e ?...8D.0A.(B. B.
-  0x0000c960 18420e10 420e0845 0b000000 28000000 .B..B..E....(...
-  0x0000c970 f0040000 bc7fffff fb000000 004b0eb0 .............K..
-  0x0000c980 0102a30e b8014b0e c001610e b801410e ......K...a...A.
-  0x0000c990 b0015a0a 0e08410b 10000000 1c050000 ..Z...A.........
-  0x0000c9a0 9080ffff 09000000 00000000 4c000000 ............L...
-  0x0000c9b0 30050000 8c80ffff db040000 00460e10 0............F..
-  0x0000c9c0 8f02420e 188e0348 0e208d04 450e288c ..B....H. ..E.(.
-  0x0000c9d0 05410e30 8606440e 3883074a 0ee00103 .A.0..D.8..J....
-  0x0000c9e0 03030a0e 38440e30 410e2842 0e20420e ....8D.0A.(B. B.
-  0x0000c9f0 18420e10 420e084c 0b000000 28000000 .B..B..L....(...
-  0x0000ca00 80050000 1c85ffff fb000000 004b0eb0 .............K..
-  0x0000ca10 0102a30e b8014b0e c001610e b801410e ......K...a...A.
-  0x0000ca20 b0015a0a 0e08410b 10000000 ac050000 ..Z...A.........
-  0x0000ca30 f085ffff 09000000 00000000 4c000000 ............L...
-  0x0000ca40 c0050000 ec85ffff 56040000 00460e10 ........V....F..
-  0x0000ca50 8f02420e 188e034c 0e208d04 4a0e288c ..B....L. ..J.(.
-  0x0000ca60 05410e30 8606440e 38830747 0eb00103 .A.0..D.8..G....
-  0x0000ca70 7c020a0e 38440e30 410e2842 0e20420e |...8D.0A.(B. B.
-  0x0000ca80 18420e10 420e084d 0b000000 48000000 .B..B..M....H...
-  0x0000ca90 10060000 9c5dffff be000000 00450e10 .....].......E..
-  0x0000caa0 86024e0e 184b0e20 4f0e284c 0e30500e ..N..K. O.(L.0P.
-  0x0000cab0 10480e18 560e2045 0e28420e 30490e10 .H..V. E.(B.0I..
-  0x0000cac0 480e1856 0e20450e 28420e30 500e104d H..V. E.(B.0P..M
-  0x0000cad0 0e080000 00000000 10000000 5c060000 ............\...
-  0x0000cae0 b089ffff 12000000 00000000 00000000 ................
+  0x0000c4b0 14000000 00000000 017a5200 01781001 .........zR..x..
+  0x0000c4c0 1b0c0708 90010000 24000000 1c000000 ........$.......
+  0x0000c4d0 505bffff 00040000 000e1046 0e184a0f P[.........F..J.
+  0x0000c4e0 0b770880 003f1a3a 2a332422 00000000 .w...?.:*3$"....
+  0x0000c4f0 14000000 44000000 285fffff 40000000 ....D...(_..@...
+  0x0000c500 00000000 00000000 14000000 5c000000 ............\...
+  0x0000c510 505fffff f0030000 00000000 00000000 P_..............
+  0x0000c520 10000000 74000000 a864ffff 09000000 ....t....d......
+  0x0000c530 00000000 10000000 88000000 a464ffff .............d..
+  0x0000c540 10000000 00000000 10000000 9c000000 ................
+  0x0000c550 a064ffff 1b000000 00000000 10000000 .d..............
+  0x0000c560 b0000000 ac64ffff 1a000000 00000000 .....d..........
+  0x0000c570 10000000 c4000000 b864ffff 1b000000 .........d......
+  0x0000c580 00000000 10000000 d8000000 c464ffff .............d..
+  0x0000c590 1b000000 00000000 10000000 ec000000 ................
+  0x0000c5a0 d064ffff 1b000000 00000000 10000000 .d..............
+  0x0000c5b0 00010000 dc64ffff 1b000000 00000000 .....d..........
+  0x0000c5c0 10000000 14010000 e864ffff 1b000000 .........d......
+  0x0000c5d0 00000000 10000000 28010000 f464ffff ........(....d..
+  0x0000c5e0 1a000000 00000000 1c000000 3c010000 ............<...
+  0x0000c5f0 0065ffff 65000000 00450e10 8302470e .e..e....E....G.
+  0x0000c600 2002570e 10410e08 1c000000 5c010000  .W..A......\...
+  0x0000c610 5065ffff 6e000000 00450e10 8302470e Pe..n....E....G.
+  0x0000c620 2002600e 10410e08 1c000000 7c010000  .`..A......|...
+  0x0000c630 a065ffff 62000000 00450e10 8302470e .e..b....E....G.
+  0x0000c640 2002540e 10410e08 14000000 9c010000  .T..A..........
+  0x0000c650 f065ffff 74000000 0002510e 20620e08 .e..t.....Q. b..
+  0x0000c660 14000000 b4010000 5866ffff 69000000 ........Xf..i...
+  0x0000c670 0002490e 205f0e08 18000000 cc010000 ..I. _..........
+  0x0000c680 b066ffff 66000000 00640e20 700a0e08 .f..f....d. p...
+  0x0000c690 410b0000 10000000 e8010000 0467ffff A............g..
+  0x0000c6a0 37000000 00000000 10000000 fc010000 7...............
+  0x0000c6b0 3067ffff 45000000 00000000 1c000000 0g..E...........
+  0x0000c6c0 10020000 6c67ffff 6d000000 00450e10 ....lg..m....E..
+  0x0000c6d0 8302470e 20025f0e 10410e08 10000000 ..G. ._..A......
+  0x0000c6e0 30020000 bc67ffff 37000000 00000000 0....g..7.......
+  0x0000c6f0 10000000 44020000 e867ffff 37000000 ....D....g..7...
+  0x0000c700 00000000 10000000 58020000 1468ffff ........X....h..
+  0x0000c710 3e000000 00000000 1c000000 6c020000 >...........l...
+  0x0000c720 4068ffff c9000000 00450e10 8302470e @h.......E....G.
+  0x0000c730 2002bb0e 10410e08 1c000000 8c020000  ....A..........
+  0x0000c740 f068ffff cc000000 00450e10 8302470e .h.......E....G.
+  0x0000c750 2002be0e 10410e08 1c000000 ac020000  ....A..........
+  0x0000c760 a069ffff c6000000 00450e10 8302470e .i.......E....G.
+  0x0000c770 2002b80e 10410e08 10000000 cc020000  ....A..........
+  0x0000c780 506affff 45000000 00000000 10000000 Pj..E...........
+  0x0000c790 e0020000 8c6affff 73000000 00000000 .....j..s.......
+  0x0000c7a0 10000000 f4020000 f86affff 94010000 .........j......
+  0x0000c7b0 00000000 10000000 08030000 846cffff .............l..
+  0x0000c7c0 a2010000 00000000 10000000 1c030000 ................
+  0x0000c7d0 206effff a2010000 00000000 10000000  n..............
+  0x0000c7e0 30030000 bc6fffff a2010000 00000000 0....o..........
+  0x0000c7f0 10000000 44030000 5871ffff a2010000 ....D...Xq......
+  0x0000c800 00000000 10000000 58030000 f472ffff ........X....r..
+  0x0000c810 69000000 00000000 14000000 6c030000 i...........l...
+  0x0000c820 5073ffff 45000000 00480e20 7c0e0800 Ps..E....H. |...
+  0x0000c830 10000000 84030000 8873ffff 26010000 .........s..&...
+  0x0000c840 00000000 10000000 98030000 a474ffff .............t..
+  0x0000c850 2f000000 00000000 38000000 ac030000 /.......8.......
+  0x0000c860 c074ffff 52000000 004d0e10 8c02460e .t..R....M....F.
+  0x0000c870 18860344 0e208304 620a0e18 460e1042 ...D. ..b...F..B
+  0x0000c880 0e08470b 410e1843 0e10420e 0841c3c6 ..G.A..C..B..A..
+  0x0000c890 cc000000 10000000 e8030000 e474ffff .............t..
+  0x0000c8a0 21000000 00000000 10000000 fc030000 !...............
+  0x0000c8b0 0075ffff 0e020000 00000000 4c000000 .u..........L...
+  0x0000c8c0 10040000 fc76ffff db020000 00460e10 .....v.......F..
+  0x0000c8d0 8f024c0e 188e0342 0e208d04 420e288c ..L....B. ..B.(.
+  0x0000c8e0 054b0e30 8606500e 3883074e 0eb00203 .K.0..P.8..N....
+  0x0000c8f0 63020a0e 38410e30 410e2842 0e20420e c...8A.0A.(B. B.
+  0x0000c900 18420e10 420e0844 0b000000 28000000 .B..B..D....(...
+  0x0000c910 60040000 8c79ffff fb000000 004b0eb0 `....y.......K..
+  0x0000c920 0102a30e b8014b0e c001610e b801410e ......K...a...A.
+  0x0000c930 b0015a0a 0e08410b 10000000 8c040000 ..Z...A.........
+  0x0000c940 607affff 09000000 00000000 4c000000 `z..........L...
+  0x0000c950 a0040000 5c7affff a4050000 00460e10 ....\z.......F..
+  0x0000c960 8f02420e 188e0348 0e208d04 4c0e288c ..B....H. ..L.(.
+  0x0000c970 05410e30 8606440e 3883074e 0e900203 .A.0..D.8..N....
+  0x0000c980 3f030a0e 38440e30 410e2842 0e20420e ?...8D.0A.(B. B.
+  0x0000c990 18420e10 420e0845 0b000000 28000000 .B..B..E....(...
+  0x0000c9a0 f0040000 bc7fffff fb000000 004b0eb0 .............K..
+  0x0000c9b0 0102a30e b8014b0e c001610e b801410e ......K...a...A.
+  0x0000c9c0 b0015a0a 0e08410b 10000000 1c050000 ..Z...A.........
+  0x0000c9d0 9080ffff 09000000 00000000 4c000000 ............L...
+  0x0000c9e0 30050000 8c80ffff f5040000 00460e10 0............F..
+  0x0000c9f0 8f02420e 188e0348 0e208d04 450e288c ..B....H. ..E.(.
+  0x0000ca00 05440e30 8606410e 3883074a 0ee00103 .D.0..A.8..J....
+  0x0000ca10 1b030a0e 38440e30 410e2842 0e20420e ....8D.0A.(B. B.
+  0x0000ca20 18420e10 420e084c 0b000000 28000000 .B..B..L....(...
+  0x0000ca30 80050000 3c85ffff fb000000 004b0eb0 ....<........K..
+  0x0000ca40 0102a30e b8014b0e c001610e b801410e ......K...a...A.
+  0x0000ca50 b0015a0a 0e08410b 10000000 ac050000 ..Z...A.........
+  0x0000ca60 1086ffff 09000000 00000000 4c000000 ............L...
+  0x0000ca70 c0050000 0c86ffff 56040000 00460e10 ........V....F..
+  0x0000ca80 8f02420e 188e034c 0e208d04 4a0e288c ..B....L. ..J.(.
+  0x0000ca90 05410e30 8606440e 38830747 0eb00103 .A.0..D.8..G....
+  0x0000caa0 7c020a0e 38440e30 410e2842 0e20420e |...8D.0A.(B. B.
+  0x0000cab0 18420e10 420e084d 0b000000 48000000 .B..B..M....H...
+  0x0000cac0 10060000 8c5dffff be000000 00450e10 .....].......E..
+  0x0000cad0 86024e0e 184b0e20 4f0e284c 0e30500e ..N..K. O.(L.0P.
+  0x0000cae0 10480e18 560e2045 0e28420e 30490e10 .H..V. E.(B.0I..
+  0x0000caf0 480e1856 0e20450e 28420e30 500e104d H..V. E.(B.0P..M
+  0x0000cb00 0e080000 00000000 10000000 5c060000 ............\...
+  0x0000cb10 d089ffff 12000000 00000000 00000000 ................
```

#### readelf --wide --decompress --hex-dump=.init_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.init_array':
-  0x0000ddb0 a0290000 00000000 30280000 00000000 .)......0(......
+  0x0000ddb0 c0290000 00000000 50280000 00000000 .)......P(......
```

#### readelf --wide --decompress --hex-dump=.fini_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.fini_array':
-  0x0000ddc0 60290000 00000000                   `)......
+  0x0000ddc0 80290000 00000000                   .)......
```

#### readelf --wide --decompress --hex-dump=.got.plt {}

```diff
@@ -29,9 +29,9 @@
   0x0000e190 20230000 00000000 30230000 00000000  #......0#......
   0x0000e1a0 40230000 00000000 50230000 00000000 @#......P#......
   0x0000e1b0 60230000 00000000 70230000 00000000 `#......p#......
   0x0000e1c0 80230000 00000000 90230000 00000000 .#.......#......
   0x0000e1d0 a0230000 00000000 b0230000 00000000 .#.......#......
   0x0000e1e0 c0230000 00000000 d0230000 00000000 .#.......#......
   0x0000e1f0 e0230000 00000000 f0230000 00000000 .#.......#......
-  0x0000e200 00240000 00000000                   .$......
+  0x0000e200 00240000 00000000 10240000 00000000 .$.......$......
```

#### readelf --wide --decompress --hex-dump=.data {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.data':
-  0x0000e208 08e20000 00000000                   ........
+  0x0000e210 10e20000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.nvFatBinSegment {}

```diff
@@ -1,5 +1,5 @@
 
 Hex dump of section '.nvFatBinSegment':
-  0x0000e210 b1436246 01000000 80670000 00000000 .CbF.....g......
-  0x0000e220 00000000 00000000                   ........
+  0x0000e218 b1436246 01000000 b0670000 00000000 .CbF.....g......
+  0x0000e228 00000000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.strtab':
-  0x00000000 00746d70 7866745f 30303030 30323538 .tmpxft_00000258
+  0x00000000 00746d70 7866745f 30303030 30323339 .tmpxft_00000239
   0x00000010 5f303030 30303030 302d365f 7467715f _00000000-6_tgq_
   0x00000020 73696d75 6c61746f 722e6375 64616665 simulator.cudafe
   0x00000030 312e6370 70006661 7462696e 44617461 1.cpp.fatbinData
   0x00000040 005f5a4c 32365f5f 63756461 556e7265 ._ZL26__cudaUnre
   0x00000050 67697374 65724269 6e617279 5574696c gisterBinaryUtil
   0x00000060 76005f5a 4c32305f 5f637564 61466174 v._ZL20__cudaFat
   0x00000070 43756269 6e48616e 646c6500 5f5a4c32 CubinHandle._ZL2
@@ -114,47 +114,49 @@
   0x000006f0 5f5a3134 67657441 72726179 4c656e67 _Z14getArrayLeng
   0x00000700 74685069 00637564 614c6175 6e63684b thPi.cudaLaunchK
   0x00000710 65726e65 6c40406c 69626375 64617274 ernel@@libcudart
   0x00000720 2e736f2e 31312e30 005f5a31 31696465 .so.11.0._Z11ide
   0x00000730 6e746974 794d6174 5036666c 6f617432 ntityMatP6float2
   0x00000740 69005f5a 31386163 74696f6e 4f6e5472 i._Z18actionOnTr
   0x00000750 69706c65 47617465 5036666c 6f617432 ipleGateP6float2
-  0x00000760 53305f6d 506d005f 5a387364 675f6761 S0_mPm._Z8sdg_ga
-  0x00000770 74655036 666c6f61 7432005f 5a323074 teP6float2._Z20t
-  0x00000780 6f66665f 67617465 5f746172 6765745f off_gate_target_
-  0x00000790 6d696450 36666c6f 61743200 5f5a3679 midP6float2._Z6y
-  0x000007a0 5f676174 65503666 6c6f6174 32005f5a _gateP6float2._Z
-  0x000007b0 3772785f 67617465 5036666c 6f617432 7rx_gateP6float2
-  0x000007c0 66006375 64615365 74446576 69636540 f.cudaSetDevice@
-  0x000007d0 406c6962 63756461 72742e73 6f2e3131 @libcudart.so.11
-  0x000007e0 2e30005f 5a37637a 5f676174 65503666 .0._Z7cz_gateP6f
-  0x000007f0 6c6f6174 32005f5f 6378615f 61746578 loat2.__cxa_atex
-  0x00000800 69744040 474c4942 435f322e 322e3500 it@@GLIBC_2.2.5.
-  0x00000810 5f5a3231 66726564 5f676174 655f636f _Z21fred_gate_co
-  0x00000820 6e74726f 6c5f6d69 64503666 6c6f6174 ntrol_midP6float
-  0x00000830 32005f5a 34686173 68504b63 005f5a38 2._Z4hashPKc._Z8
-  0x00000840 7379635f 67617465 5036666c 6f617432 syc_gateP6float2
-  0x00000850 005f4954 4d5f7265 67697374 6572544d ._ITM_registerTM
-  0x00000860 436c6f6e 65546162 6c65005f 5f637564 CloneTable.__cud
-  0x00000870 61507573 6843616c 6c436f6e 66696775 aPushCallConfigu
-  0x00000880 72617469 6f6e4040 6c696263 75646172 ration@@libcudar
-  0x00000890 742e736f 2e31312e 30005f5f 63756461 t.so.11.0.__cuda
-  0x000008a0 52656769 73746572 46617442 696e6172 RegisterFatBinar
-  0x000008b0 79456e64 40406c69 62637564 6172742e yEnd@@libcudart.
-  0x000008c0 736f2e31 312e3000 5f5a3763 6f6d7061 so.11.0._Z7compa
-  0x000008d0 7265504b 7653305f 005f5a31 31637068 rePKvS0_._Z11cph
-  0x000008e0 6173655f 67617465 5036666c 6f617432 ase_gateP6float2
-  0x000008f0 66005f5f 6378615f 66696e61 6c697a65 f.__cxa_finalize
-  0x00000900 4040474c 4942435f 322e322e 35005f5a @@GLIBC_2.2.5._Z
-  0x00000910 3761645f 67617465 5036666c 6f617432 7ad_gateP6float2
-  0x00000920 66005f5a 31396163 74696f6e 4f6e5369 f._Z19actionOnSi
-  0x00000930 6e676c65 51756269 74503666 6c6f6174 ngleQubitP6float
-  0x00000940 3253305f 6d506d00 5f5a3530 5f5f6465 2S0_mPm._Z50__de
-  0x00000950 76696365 5f737475 625f5f5a 31386163 vice_stub__Z18ac
-  0x00000960 74696f6e 4f6e5472 69706c65 47617465 tionOnTripleGate
-  0x00000970 5036666c 6f617432 53305f6d 506d5036 P6float2S0_mPmP6
-  0x00000980 666c6f61 74325330 5f6d506d 005f5f63 float2S0_mPm.__c
-  0x00000990 75646150 6f704361 6c6c436f 6e666967 udaPopCallConfig
-  0x000009a0 75726174 696f6e40 406c6962 63756461 uration@@libcuda
-  0x000009b0 72742e73 6f2e3131 2e30005f 5a36785f rt.so.11.0._Z6x_
-  0x000009c0 67617465 5036666c 6f617432 00       gateP6float2.
+  0x00000760 53305f6d 506d005f 5f707269 6e74665f S0_mPm.__printf_
+  0x00000770 63686b40 40474c49 42435f32 2e332e34 chk@@GLIBC_2.3.4
+  0x00000780 005f5a38 7364675f 67617465 5036666c ._Z8sdg_gateP6fl
+  0x00000790 6f617432 005f5a32 30746f66 665f6761 oat2._Z20toff_ga
+  0x000007a0 74655f74 61726765 745f6d69 64503666 te_target_midP6f
+  0x000007b0 6c6f6174 32005f5a 36795f67 61746550 loat2._Z6y_gateP
+  0x000007c0 36666c6f 61743200 5f5a3772 785f6761 6float2._Z7rx_ga
+  0x000007d0 74655036 666c6f61 74326600 63756461 teP6float2f.cuda
+  0x000007e0 53657444 65766963 6540406c 69626375 SetDevice@@libcu
+  0x000007f0 64617274 2e736f2e 31312e30 005f5a37 dart.so.11.0._Z7
+  0x00000800 637a5f67 61746550 36666c6f 61743200 cz_gateP6float2.
+  0x00000810 5f5f6378 615f6174 65786974 4040474c __cxa_atexit@@GL
+  0x00000820 4942435f 322e322e 35005f5a 32316672 IBC_2.2.5._Z21fr
+  0x00000830 65645f67 6174655f 636f6e74 726f6c5f ed_gate_control_
+  0x00000840 6d696450 36666c6f 61743200 5f5a3468 midP6float2._Z4h
+  0x00000850 61736850 4b63005f 5a387379 635f6761 ashPKc._Z8syc_ga
+  0x00000860 74655036 666c6f61 7432005f 49544d5f teP6float2._ITM_
+  0x00000870 72656769 73746572 544d436c 6f6e6554 registerTMCloneT
+  0x00000880 61626c65 005f5f63 75646150 75736843 able.__cudaPushC
+  0x00000890 616c6c43 6f6e6669 67757261 74696f6e allConfiguration
+  0x000008a0 40406c69 62637564 6172742e 736f2e31 @@libcudart.so.1
+  0x000008b0 312e3000 5f5f6375 64615265 67697374 1.0.__cudaRegist
+  0x000008c0 65724661 7442696e 61727945 6e644040 erFatBinaryEnd@@
+  0x000008d0 6c696263 75646172 742e736f 2e31312e libcudart.so.11.
+  0x000008e0 30005f5a 37636f6d 70617265 504b7653 0._Z7comparePKvS
+  0x000008f0 305f005f 5a313163 70686173 655f6761 0_._Z11cphase_ga
+  0x00000900 74655036 666c6f61 74326600 5f5f6378 teP6float2f.__cx
+  0x00000910 615f6669 6e616c69 7a654040 474c4942 a_finalize@@GLIB
+  0x00000920 435f322e 322e3500 5f5a3761 645f6761 C_2.2.5._Z7ad_ga
+  0x00000930 74655036 666c6f61 74326600 5f5a3139 teP6float2f._Z19
+  0x00000940 61637469 6f6e4f6e 53696e67 6c655175 actionOnSingleQu
+  0x00000950 62697450 36666c6f 61743253 305f6d50 bitP6float2S0_mP
+  0x00000960 6d005f5a 35305f5f 64657669 63655f73 m._Z50__device_s
+  0x00000970 7475625f 5f5a3138 61637469 6f6e4f6e tub__Z18actionOn
+  0x00000980 54726970 6c654761 74655036 666c6f61 TripleGateP6floa
+  0x00000990 74325330 5f6d506d 5036666c 6f617432 t2S0_mPmP6float2
+  0x000009a0 53305f6d 506d005f 5f637564 61506f70 S0_mPm.__cudaPop
+  0x000009b0 43616c6c 436f6e66 69677572 6174696f CallConfiguratio
+  0x000009c0 6e40406c 69626375 64617274 2e736f2e n@@libcudart.so.
+  0x000009d0 31312e30 005f5a36 785f6761 74655036 11.0._Z6x_gateP6
+  0x000009e0 666c6f61 743200                     float2.
```

### Comparing `tgqSim-0.1.7/tgqSim/lib/cuda_12-4_tgq_simulator.so` & `tgqSim-0.1.8/tgqSim/lib/cuda_12-4_tgq_simulator.so`

 * *Files 3% similar despite different names*

#### readelf --wide --program-header {}

```diff
@@ -1,18 +1,18 @@
 
 Elf file type is DYN (Shared object file)
 Entry point 0x1fa0
 There are 6 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x00b664 0x00b664 R E 0x200000
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x00b684 0x00b684 R E 0x200000
   LOAD           0x00bd60 0x000000000020bd60 0x000000000020bd60 0x0004e8 0x0004f8 RW  0x200000
   DYNAMIC        0x00bd78 0x000000000020bd78 0x000000000020bd78 0x000230 0x000230 RW  0x8
-  GNU_EH_FRAME   0x00ade8 0x000000000000ade8 0x000000000000ade8 0x0001ac 0x0001ac R   0x4
+  GNU_EH_FRAME   0x00ae08 0x000000000000ae08 0x000000000000ae08 0x0001ac 0x0001ac R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
   GNU_RELRO      0x00bd60 0x000000000020bd60 0x000000000020bd60 0x0002a0 0x0002a0 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     .hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt .init .plt .text .fini .rodata .nv_fatbin .eh_frame_hdr .eh_frame 
    01     .init_array .fini_array .dynamic .got .got.plt .data .nvFatBinSegment .bss
```

#### readelf --wide --sections {}

```diff
@@ -8,20 +8,20 @@
   [ 3] .dynstr           STRTAB          0000000000000b80 000b80 000717 00   A  0   0  1
   [ 4] .gnu.version      VERSYM          0000000000001298 001298 0000a2 02   A  2   0  2
   [ 5] .gnu.version_r    VERNEED         0000000000001340 001340 000060 00   A  3   3  8
   [ 6] .rela.dyn         RELA            00000000000013a0 0013a0 000180 18   A  2   0  8
   [ 7] .rela.plt         RELA            0000000000001520 001520 000630 18  AI  2  20  8
   [ 8] .init             PROGBITS        0000000000001b50 001b50 000017 00  AX  0   0  4
   [ 9] .plt              PROGBITS        0000000000001b70 001b70 000430 10  AX  0   0 16
-  [10] .text             PROGBITS        0000000000001fa0 001fa0 002abe 00  AX  0   0 16
-  [11] .fini             PROGBITS        0000000000004a60 004a60 000009 00  AX  0   0  4
-  [12] .rodata           PROGBITS        0000000000004a70 004a70 000318 00   A  0   0 16
-  [13] .nv_fatbin        PROGBITS        0000000000004d88 004d88 006060 00   A  0   0  8
-  [14] .eh_frame_hdr     PROGBITS        000000000000ade8 00ade8 0001ac 00   A  0   0  4
-  [15] .eh_frame         PROGBITS        000000000000af98 00af98 0006cc 00   A  0   0  8
+  [10] .text             PROGBITS        0000000000001fa0 001fa0 002ace 00  AX  0   0 16
+  [11] .fini             PROGBITS        0000000000004a70 004a70 000009 00  AX  0   0  4
+  [12] .rodata           PROGBITS        0000000000004a80 004a80 000328 00   A  0   0 16
+  [13] .nv_fatbin        PROGBITS        0000000000004da8 004da8 006060 00   A  0   0  8
+  [14] .eh_frame_hdr     PROGBITS        000000000000ae08 00ae08 0001ac 00   A  0   0  4
+  [15] .eh_frame         PROGBITS        000000000000afb8 00afb8 0006cc 00   A  0   0  8
   [16] .init_array       INIT_ARRAY      000000000020bd60 00bd60 000010 08  WA  0   0  8
   [17] .fini_array       FINI_ARRAY      000000000020bd70 00bd70 000008 08  WA  0   0  8
   [18] .dynamic          DYNAMIC         000000000020bd78 00bd78 000230 10  WA  3   0  8
   [19] .got              PROGBITS        000000000020bfa8 00bfa8 000058 08  WA  0   0  8
   [20] .got.plt          PROGBITS        000000000020c000 00c000 000228 08  WA  0   0  8
   [21] .data             PROGBITS        000000000020c228 00c228 000008 00  WA  0   0  8
   [22] .nvFatBinSegment  PROGBITS        000000000020c230 00c230 000018 00  WA  0   0  8
```

#### readelf --wide --symbols {}

```diff
@@ -1,19 +1,19 @@
 
 Symbol table '.dynsym' contains 81 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 00000000000025a0   105 FUNC    GLOBAL DEFAULT   10 _Z11cphase_gateP6float2f
-     2: 00000000000036c0   662 FUNC    GLOBAL DEFAULT   10 execute_circuit
+     2: 00000000000036c0   678 FUNC    GLOBAL DEFAULT   10 execute_circuit
      3: 0000000000002490   117 FUNC    GLOBAL DEFAULT   10 _Z7ad_gateP6float2f
      4: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND printf@GLIBC_2.2.5 (2)
      5: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMalloc@libcudart.so.12 (3)
      6: 0000000000003400    47 FUNC    GLOBAL DEFAULT   10 _Z4hashPKc
      7: 0000000000002410   120 FUNC    GLOBAL DEFAULT   10 _Z7pd_gateP6float2f
-     8: 0000000000004550   201 FUNC    GLOBAL DEFAULT   10 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
+     8: 0000000000004560   201 FUNC    GLOBAL DEFAULT   10 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
      9: 0000000000002160    22 FUNC    GLOBAL DEFAULT   10 _Z6y_gateP6float2
     10: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaLaunchKernel@libcudart.so.12 (3)
     11: 0000000000002990   101 FUNC    GLOBAL DEFAULT   10 _Z22toff_gate_target_smallP6float2
     12: 0000000000002120     5 FUNC    GLOBAL DEFAULT   10 _Z7comparePKvS0_
     13: 000000000020c248     0 NOTYPE  GLOBAL DEFAULT   22 _edata
     14: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND rand@GLIBC_2.2.5 (2)
     15: 0000000000003080   416 FUNC    GLOBAL DEFAULT   10 _Z23fred_gate_control_smallP6float2
@@ -24,62 +24,62 @@
     20: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sincosf@GLIBC_2.2.5 (4)
     21: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (2)
     22: 0000000000002d40   416 FUNC    GLOBAL DEFAULT   10 _Z21fred_gate_control_bigP6float2
     23: 0000000000002940    65 FUNC    GLOBAL DEFAULT   10 _Z8syc_gateP6float2
     24: 00000000000026d0   197 FUNC    GLOBAL DEFAULT   10 _Z8rxx_gateP6float2f
     25: 0000000000002a00   402 FUNC    GLOBAL DEFAULT   10 _Z20toff_gate_target_midP6float2
     26: 0000000000002870   194 FUNC    GLOBAL DEFAULT   10 _Z8rzz_gateP6float2f
-    27: 0000000000004080  1227 FUNC    GLOBAL DEFAULT   10 doubleGateAction
+    27: 0000000000004090  1227 FUNC    GLOBAL DEFAULT   10 doubleGateAction
     28: 0000000000003430    82 FUNC    GLOBAL DEFAULT   10 _Z9isInArrayPPKcPci
     29: 0000000000002610    51 FUNC    GLOBAL DEFAULT   10 _Z21cnot_gate_control_bigP6float2
     30: 0000000000002140    23 FUNC    GLOBAL DEFAULT   10 _Z6x_gateP6float2
     31: 0000000000003290    65 FUNC    GLOBAL DEFAULT   10 _Z20generate_binary_dataf
     32: 00000000000021a0    23 FUNC    GLOBAL DEFAULT   10 _Z6s_gateP6float2
     33: 0000000000002380   131 FUNC    GLOBAL DEFAULT   10 _Z11damp_i_gateP6float2f
     34: 0000000000002550    65 FUNC    GLOBAL DEFAULT   10 _Z10iswap_gateP6float2
     35: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@GLIBC_2.2.5 (2)
     36: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinary@libcudart.so.12 (3)
     37: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND time@GLIBC_2.2.5 (2)
     38: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND srand@GLIBC_2.2.5 (2)
     39: 00000000000021e0    23 FUNC    GLOBAL DEFAULT   10 _Z6t_gateP6float2
     40: 00000000000034c0   510 FUNC    GLOBAL DEFAULT   10 _Z13normalizationP6float2i
     41: 0000000000002180    23 FUNC    GLOBAL DEFAULT   10 _Z6z_gateP6float2
-    42: 0000000000004070     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnDoubleQubitP6float2S0_mPm
-    43: 0000000000003fa0   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm
+    42: 0000000000004080     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnDoubleQubitP6float2S0_mPm
+    43: 0000000000003fb0   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm
     44: 00000000000032e0   286 FUNC    GLOBAL DEFAULT   10 _Z7getprobP6float2Pfm
     45: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5 (2)
     46: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMemcpy@libcudart.so.12 (3)
     47: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@GLIBC_2.2.5 (2)
     48: 0000000000002200    23 FUNC    GLOBAL DEFAULT   10 _Z8tdg_gateP6float2
     49: 0000000000002690    58 FUNC    GLOBAL DEFAULT   10 _Z7cz_gateP6float2
-    50: 0000000000004620     5 FUNC    GLOBAL DEFAULT   10 _Z18actionOnTripleGateP6float2S0_mPm
+    50: 0000000000004630     5 FUNC    GLOBAL DEFAULT   10 _Z18actionOnTripleGateP6float2S0_mPm
     51: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5 (2)
     52: 000000000020c258     0 NOTYPE  GLOBAL DEFAULT   23 _end
-    53: 0000000000003960   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
+    53: 0000000000003970   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
     54: 0000000000003490    33 FUNC    GLOBAL DEFAULT   10 _Z14getArrayLengthPi
     55: 00000000000021c0    23 FUNC    GLOBAL DEFAULT   10 _Z8sdg_gateP6float2
     56: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strcmp@GLIBC_2.2.5 (2)
     57: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFunction@libcudart.so.12 (3)
     58: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaFree@libcudart.so.12 (3)
     59: 0000000000002ba0   416 FUNC    GLOBAL DEFAULT   10 _Z20toff_gate_target_bigP6float2
     60: 00000000000027a0   200 FUNC    GLOBAL DEFAULT   10 _Z8ryy_gateP6float2f
     61: 000000000020c248     0 NOTYPE  GLOBAL DEFAULT   23 __bss_start
     62: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND puts@GLIBC_2.2.5 (2)
-    63: 0000000000003a40  1373 FUNC    GLOBAL DEFAULT   10 singleGateAction
-    64: 0000000000003a30     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnSingleQubitP6float2S0_mPm
+    63: 0000000000003a50  1373 FUNC    GLOBAL DEFAULT   10 singleGateAction
+    64: 0000000000003a40     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnSingleQubitP6float2S0_mPm
     65: 0000000000003220   107 FUNC    GLOBAL DEFAULT   10 _Z11identityMatP6float2i
     66: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPopCallConfiguration@libcudart.so.12 (3)
     67: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaDeviceSynchronize@libcudart.so.12 (3)
     68: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
     69: 0000000000002320    94 FUNC    GLOBAL DEFAULT   10 _Z7rz_gateP6float2f
     70: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPushCallConfiguration@libcudart.so.12 (3)
     71: 0000000000002220    22 FUNC    GLOBAL DEFAULT   10 _Z6h_gateP6float2
     72: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sqrtf@GLIBC_2.2.5 (4)
     73: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinaryEnd@libcudart.so.12 (3)
-    74: 0000000000004630  1049 FUNC    GLOBAL DEFAULT   10 tripleGateAction
+    74: 0000000000004640  1049 FUNC    GLOBAL DEFAULT   10 tripleGateAction
     75: 0000000000002510    51 FUNC    GLOBAL DEFAULT   10 _Z9swap_gateP6float2
     76: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
     77: 0000000000002240    97 FUNC    GLOBAL DEFAULT   10 _Z7rx_gateP6float2f
     78: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND qsort@GLIBC_2.2.5 (2)
     79: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
     80: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaSetDevice@libcudart.so.12 (3)
 
@@ -92,19 +92,19 @@
      4: 0000000000001298     0 SECTION LOCAL  DEFAULT    4 .gnu.version
      5: 0000000000001340     0 SECTION LOCAL  DEFAULT    5 .gnu.version_r
      6: 00000000000013a0     0 SECTION LOCAL  DEFAULT    6 .rela.dyn
      7: 0000000000001520     0 SECTION LOCAL  DEFAULT    7 .rela.plt
      8: 0000000000001b50     0 SECTION LOCAL  DEFAULT    8 .init
      9: 0000000000001b70     0 SECTION LOCAL  DEFAULT    9 .plt
     10: 0000000000001fa0     0 SECTION LOCAL  DEFAULT   10 .text
-    11: 0000000000004a60     0 SECTION LOCAL  DEFAULT   11 .fini
-    12: 0000000000004a70     0 SECTION LOCAL  DEFAULT   12 .rodata
-    13: 0000000000004d88     0 SECTION LOCAL  DEFAULT   13 .nv_fatbin
-    14: 000000000000ade8     0 SECTION LOCAL  DEFAULT   14 .eh_frame_hdr
-    15: 000000000000af98     0 SECTION LOCAL  DEFAULT   15 .eh_frame
+    11: 0000000000004a70     0 SECTION LOCAL  DEFAULT   11 .fini
+    12: 0000000000004a80     0 SECTION LOCAL  DEFAULT   12 .rodata
+    13: 0000000000004da8     0 SECTION LOCAL  DEFAULT   13 .nv_fatbin
+    14: 000000000000ae08     0 SECTION LOCAL  DEFAULT   14 .eh_frame_hdr
+    15: 000000000000afb8     0 SECTION LOCAL  DEFAULT   15 .eh_frame
     16: 000000000020bd60     0 SECTION LOCAL  DEFAULT   16 .init_array
     17: 000000000020bd70     0 SECTION LOCAL  DEFAULT   17 .fini_array
     18: 000000000020bd78     0 SECTION LOCAL  DEFAULT   18 .dynamic
     19: 000000000020bfa8     0 SECTION LOCAL  DEFAULT   19 .got
     20: 000000000020c000     0 SECTION LOCAL  DEFAULT   20 .got.plt
     21: 000000000020c228     0 SECTION LOCAL  DEFAULT   21 .data
     22: 000000000020c230     0 SECTION LOCAL  DEFAULT   22 .nvFatBinSegment
@@ -113,50 +113,50 @@
     25: 0000000000000000     0 SECTION LOCAL  DEFAULT   25 .debug_aranges
     26: 0000000000000000     0 SECTION LOCAL  DEFAULT   26 .debug_info
     27: 0000000000000000     0 SECTION LOCAL  DEFAULT   27 .debug_abbrev
     28: 0000000000000000     0 SECTION LOCAL  DEFAULT   28 .debug_line
     29: 0000000000000000     0 SECTION LOCAL  DEFAULT   29 .debug_str
     30: 0000000000000000     0 SECTION LOCAL  DEFAULT   30 .debug_loc
     31: 0000000000000000     0 SECTION LOCAL  DEFAULT   31 .debug_ranges
-    32: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00005715_00000000-6_tgq_simulator.cudafe1.cpp
-    33: 0000000000005148     0 NOTYPE  LOCAL  DEFAULT   13 fatbinData
+    32: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00005772_00000000-6_tgq_simulator.cudafe1.cpp
+    33: 0000000000005168     0 NOTYPE  LOCAL  DEFAULT   13 fatbinData
     34: 0000000000002130    12 FUNC    LOCAL  DEFAULT   10 _ZL26__cudaUnregisterBinaryUtilv
     35: 000000000020c250     8 OBJECT  LOCAL  DEFAULT   23 _ZL20__cudaFatCubinHandle
     36: 0000000000001fa0   186 FUNC    LOCAL  DEFAULT   10 _ZL24__sti____cudaRegisterAllv
     37: 000000000020c230    24 OBJECT  LOCAL  DEFAULT   22 _ZL15__fatDeviceText
     38: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
     39: 0000000000002060     0 FUNC    LOCAL  DEFAULT   10 deregister_tm_clones
     40: 0000000000002090     0 FUNC    LOCAL  DEFAULT   10 register_tm_clones
     41: 00000000000020d0     0 FUNC    LOCAL  DEFAULT   10 __do_global_dtors_aux
     42: 000000000020c248     1 OBJECT  LOCAL  DEFAULT   23 completed.7311
     43: 000000000020bd70     0 OBJECT  LOCAL  DEFAULT   17 __do_global_dtors_aux_fini_array_entry
     44: 0000000000002110     0 FUNC    LOCAL  DEFAULT   10 frame_dummy
     45: 000000000020bd60     0 OBJECT  LOCAL  DEFAULT   16 __frame_dummy_init_array_entry
     46: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS link.stub
-    47: 0000000000004d88     0 NOTYPE  LOCAL  DEFAULT   13 fatbinData
+    47: 0000000000004da8     0 NOTYPE  LOCAL  DEFAULT   13 fatbinData
     48: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS atexit.c
     49: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    50: 000000000000b660     0 OBJECT  LOCAL  DEFAULT   15 __FRAME_END__
+    50: 000000000000b680     0 OBJECT  LOCAL  DEFAULT   15 __FRAME_END__
     51: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
-    52: 000000000000ade8     0 NOTYPE  LOCAL  DEFAULT   14 __GNU_EH_FRAME_HDR
+    52: 000000000000ae08     0 NOTYPE  LOCAL  DEFAULT   14 __GNU_EH_FRAME_HDR
     53: 000000000020c228     0 OBJECT  LOCAL  DEFAULT   21 __dso_handle
-    54: 0000000000004a50    14 FUNC    LOCAL  DEFAULT   10 atexit
-    55: 0000000000004a60     0 FUNC    LOCAL  DEFAULT   11 _fini
+    54: 0000000000004a60    14 FUNC    LOCAL  DEFAULT   10 atexit
+    55: 0000000000004a70     0 FUNC    LOCAL  DEFAULT   11 _fini
     56: 0000000000001b50     0 FUNC    LOCAL  DEFAULT    8 _init
     57: 000000000020bd78     0 OBJECT  LOCAL  DEFAULT   18 _DYNAMIC
     58: 000000000020c230     0 OBJECT  LOCAL  DEFAULT   22 __TMC_END__
     59: 000000000020c000     0 OBJECT  LOCAL  DEFAULT   20 _GLOBAL_OFFSET_TABLE_
     60: 00000000000025a0   105 FUNC    GLOBAL DEFAULT   10 _Z11cphase_gateP6float2f
-    61: 00000000000036c0   662 FUNC    GLOBAL DEFAULT   10 execute_circuit
+    61: 00000000000036c0   678 FUNC    GLOBAL DEFAULT   10 execute_circuit
     62: 0000000000002490   117 FUNC    GLOBAL DEFAULT   10 _Z7ad_gateP6float2f
     63: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND printf@@GLIBC_2.2.5
     64: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMalloc@@libcudart.so.12
     65: 0000000000003400    47 FUNC    GLOBAL DEFAULT   10 _Z4hashPKc
     66: 0000000000002410   120 FUNC    GLOBAL DEFAULT   10 _Z7pd_gateP6float2f
-    67: 0000000000004550   201 FUNC    GLOBAL DEFAULT   10 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
+    67: 0000000000004560   201 FUNC    GLOBAL DEFAULT   10 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
     68: 0000000000002160    22 FUNC    GLOBAL DEFAULT   10 _Z6y_gateP6float2
     69: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaLaunchKernel@@libcudart.so.12
     70: 0000000000002990   101 FUNC    GLOBAL DEFAULT   10 _Z22toff_gate_target_smallP6float2
     71: 0000000000002120     5 FUNC    GLOBAL DEFAULT   10 _Z7comparePKvS0_
     72: 000000000020c248     0 NOTYPE  GLOBAL DEFAULT   22 _edata
     73: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND rand@@GLIBC_2.2.5
     74: 0000000000003080   416 FUNC    GLOBAL DEFAULT   10 _Z23fred_gate_control_smallP6float2
@@ -167,61 +167,61 @@
     79: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sincosf@@GLIBC_2.2.5
     80: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@@GLIBC_2.2.5
     81: 0000000000002d40   416 FUNC    GLOBAL DEFAULT   10 _Z21fred_gate_control_bigP6float2
     82: 0000000000002940    65 FUNC    GLOBAL DEFAULT   10 _Z8syc_gateP6float2
     83: 00000000000026d0   197 FUNC    GLOBAL DEFAULT   10 _Z8rxx_gateP6float2f
     84: 0000000000002a00   402 FUNC    GLOBAL DEFAULT   10 _Z20toff_gate_target_midP6float2
     85: 0000000000002870   194 FUNC    GLOBAL DEFAULT   10 _Z8rzz_gateP6float2f
-    86: 0000000000004080  1227 FUNC    GLOBAL DEFAULT   10 doubleGateAction
+    86: 0000000000004090  1227 FUNC    GLOBAL DEFAULT   10 doubleGateAction
     87: 0000000000003430    82 FUNC    GLOBAL DEFAULT   10 _Z9isInArrayPPKcPci
     88: 0000000000002610    51 FUNC    GLOBAL DEFAULT   10 _Z21cnot_gate_control_bigP6float2
     89: 0000000000002140    23 FUNC    GLOBAL DEFAULT   10 _Z6x_gateP6float2
     90: 0000000000003290    65 FUNC    GLOBAL DEFAULT   10 _Z20generate_binary_dataf
     91: 00000000000021a0    23 FUNC    GLOBAL DEFAULT   10 _Z6s_gateP6float2
     92: 0000000000002380   131 FUNC    GLOBAL DEFAULT   10 _Z11damp_i_gateP6float2f
     93: 0000000000002550    65 FUNC    GLOBAL DEFAULT   10 _Z10iswap_gateP6float2
     94: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@@GLIBC_2.2.5
     95: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinary@@libcudart.so.12
     96: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND time@@GLIBC_2.2.5
     97: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND srand@@GLIBC_2.2.5
     98: 00000000000021e0    23 FUNC    GLOBAL DEFAULT   10 _Z6t_gateP6float2
     99: 00000000000034c0   510 FUNC    GLOBAL DEFAULT   10 _Z13normalizationP6float2i
    100: 0000000000002180    23 FUNC    GLOBAL DEFAULT   10 _Z6z_gateP6float2
-   101: 0000000000004070     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnDoubleQubitP6float2S0_mPm
-   102: 0000000000003fa0   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm
+   101: 0000000000004080     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnDoubleQubitP6float2S0_mPm
+   102: 0000000000003fb0   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm
    103: 00000000000032e0   286 FUNC    GLOBAL DEFAULT   10 _Z7getprobP6float2Pfm
    104: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@@GLIBC_2.2.5
    105: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMemcpy@@libcudart.so.12
    106: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@@GLIBC_2.2.5
    107: 0000000000002200    23 FUNC    GLOBAL DEFAULT   10 _Z8tdg_gateP6float2
    108: 0000000000002690    58 FUNC    GLOBAL DEFAULT   10 _Z7cz_gateP6float2
-   109: 0000000000004620     5 FUNC    GLOBAL DEFAULT   10 _Z18actionOnTripleGateP6float2S0_mPm
+   109: 0000000000004630     5 FUNC    GLOBAL DEFAULT   10 _Z18actionOnTripleGateP6float2S0_mPm
    110: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@@GLIBC_2.2.5
    111: 000000000020c258     0 NOTYPE  GLOBAL DEFAULT   23 _end
-   112: 0000000000003960   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
+   112: 0000000000003970   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
    113: 0000000000003490    33 FUNC    GLOBAL DEFAULT   10 _Z14getArrayLengthPi
    114: 00000000000021c0    23 FUNC    GLOBAL DEFAULT   10 _Z8sdg_gateP6float2
    115: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strcmp@@GLIBC_2.2.5
    116: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFunction@@libcudart.so.12
    117: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaFree@@libcudart.so.12
    118: 0000000000002ba0   416 FUNC    GLOBAL DEFAULT   10 _Z20toff_gate_target_bigP6float2
    119: 00000000000027a0   200 FUNC    GLOBAL DEFAULT   10 _Z8ryy_gateP6float2f
    120: 000000000020c248     0 NOTYPE  GLOBAL DEFAULT   23 __bss_start
    121: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND puts@@GLIBC_2.2.5
-   122: 0000000000003a40  1373 FUNC    GLOBAL DEFAULT   10 singleGateAction
-   123: 0000000000003a30     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnSingleQubitP6float2S0_mPm
+   122: 0000000000003a50  1373 FUNC    GLOBAL DEFAULT   10 singleGateAction
+   123: 0000000000003a40     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnSingleQubitP6float2S0_mPm
    124: 0000000000003220   107 FUNC    GLOBAL DEFAULT   10 _Z11identityMatP6float2i
    125: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPopCallConfiguration@@libcudart.so.12
    126: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaDeviceSynchronize@@libcudart.so.12
    127: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
    128: 0000000000002320    94 FUNC    GLOBAL DEFAULT   10 _Z7rz_gateP6float2f
    129: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPushCallConfiguration@@libcudart.so.12
    130: 0000000000002220    22 FUNC    GLOBAL DEFAULT   10 _Z6h_gateP6float2
    131: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sqrtf@@GLIBC_2.2.5
    132: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinaryEnd@@libcudart.so.12
-   133: 0000000000004630  1049 FUNC    GLOBAL DEFAULT   10 tripleGateAction
+   133: 0000000000004640  1049 FUNC    GLOBAL DEFAULT   10 tripleGateAction
    134: 0000000000002510    51 FUNC    GLOBAL DEFAULT   10 _Z9swap_gateP6float2
    135: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
    136: 0000000000002240    97 FUNC    GLOBAL DEFAULT   10 _Z7rx_gateP6float2f
    137: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND qsort@@GLIBC_2.2.5
    138: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
    139: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaSetDevice@@libcudart.so.12
```

#### readelf --wide --relocs {}

```diff
@@ -1,36 +1,36 @@
 
 Relocation section '.rela.dyn' at offset 0x13a0 contains 16 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 000000000020bd60  0000000000000008 R_X86_64_RELATIVE                         2110
 000000000020bd68  0000000000000008 R_X86_64_RELATIVE                         1fa0
 000000000020bd70  0000000000000008 R_X86_64_RELATIVE                         20d0
 000000000020c228  0000000000000008 R_X86_64_RELATIVE                         20c228
-000000000020c238  0000000000000008 R_X86_64_RELATIVE                         5148
+000000000020c238  0000000000000008 R_X86_64_RELATIVE                         5168
 000000000020bfa8  0000000c00000006 R_X86_64_GLOB_DAT      0000000000002120 _Z7comparePKvS0_ + 0
 000000000020bfb0  0000001500000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
-000000000020bfb8  0000001b00000006 R_X86_64_GLOB_DAT      0000000000004080 doubleGateAction + 0
-000000000020bfc0  0000002a00000006 R_X86_64_GLOB_DAT      0000000000004070 _Z19actionOnDoubleQubitP6float2S0_mPm + 0
-000000000020bfc8  0000003200000006 R_X86_64_GLOB_DAT      0000000000004620 _Z18actionOnTripleGateP6float2S0_mPm + 0
-000000000020bfd0  0000003f00000006 R_X86_64_GLOB_DAT      0000000000003a40 singleGateAction + 0
-000000000020bfd8  0000004000000006 R_X86_64_GLOB_DAT      0000000000003a30 _Z19actionOnSingleQubitP6float2S0_mPm + 0
+000000000020bfb8  0000001b00000006 R_X86_64_GLOB_DAT      0000000000004090 doubleGateAction + 0
+000000000020bfc0  0000002a00000006 R_X86_64_GLOB_DAT      0000000000004080 _Z19actionOnDoubleQubitP6float2S0_mPm + 0
+000000000020bfc8  0000003200000006 R_X86_64_GLOB_DAT      0000000000004630 _Z18actionOnTripleGateP6float2S0_mPm + 0
+000000000020bfd0  0000003f00000006 R_X86_64_GLOB_DAT      0000000000003a50 singleGateAction + 0
+000000000020bfd8  0000004000000006 R_X86_64_GLOB_DAT      0000000000003a40 _Z19actionOnSingleQubitP6float2S0_mPm + 0
 000000000020bfe0  0000004400000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
-000000000020bfe8  0000004a00000006 R_X86_64_GLOB_DAT      0000000000004630 tripleGateAction + 0
+000000000020bfe8  0000004a00000006 R_X86_64_GLOB_DAT      0000000000004640 tripleGateAction + 0
 000000000020bff0  0000004c00000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
 000000000020bff8  0000004f00000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
 
 Relocation section '.rela.plt' at offset 0x1520 contains 66 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 000000000020c018  0000000100000007 R_X86_64_JUMP_SLOT     00000000000025a0 _Z11cphase_gateP6float2f + 0
 000000000020c020  0000000300000007 R_X86_64_JUMP_SLOT     0000000000002490 _Z7ad_gateP6float2f + 0
 000000000020c028  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 printf@GLIBC_2.2.5 + 0
 000000000020c030  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaMalloc@libcudart.so.12 + 0
 000000000020c038  0000000600000007 R_X86_64_JUMP_SLOT     0000000000003400 _Z4hashPKc + 0
 000000000020c040  0000000700000007 R_X86_64_JUMP_SLOT     0000000000002410 _Z7pd_gateP6float2f + 0
-000000000020c048  0000000800000007 R_X86_64_JUMP_SLOT     0000000000004550 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm + 0
+000000000020c048  0000000800000007 R_X86_64_JUMP_SLOT     0000000000004560 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm + 0
 000000000020c050  0000000900000007 R_X86_64_JUMP_SLOT     0000000000002160 _Z6y_gateP6float2 + 0
 000000000020c058  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaLaunchKernel@libcudart.so.12 + 0
 000000000020c060  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000002990 _Z22toff_gate_target_smallP6float2 + 0
 000000000020c068  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 rand@GLIBC_2.2.5 + 0
 000000000020c070  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000003080 _Z23fred_gate_control_smallP6float2 + 0
 000000000020c078  0000001000000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaUnregisterFatBinary@libcudart.so.12 + 0
 000000000020c080  0000001100000007 R_X86_64_JUMP_SLOT     0000000000002ee0 _Z21fred_gate_control_midP6float2 + 0
@@ -52,33 +52,33 @@
 000000000020c100  0000002300000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_atexit@GLIBC_2.2.5 + 0
 000000000020c108  0000002400000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinary@libcudart.so.12 + 0
 000000000020c110  0000002500000007 R_X86_64_JUMP_SLOT     0000000000000000 time@GLIBC_2.2.5 + 0
 000000000020c118  0000002600000007 R_X86_64_JUMP_SLOT     0000000000000000 srand@GLIBC_2.2.5 + 0
 000000000020c120  0000002700000007 R_X86_64_JUMP_SLOT     00000000000021e0 _Z6t_gateP6float2 + 0
 000000000020c128  0000002800000007 R_X86_64_JUMP_SLOT     00000000000034c0 _Z13normalizationP6float2i + 0
 000000000020c130  0000002900000007 R_X86_64_JUMP_SLOT     0000000000002180 _Z6z_gateP6float2 + 0
-000000000020c138  0000002a00000007 R_X86_64_JUMP_SLOT     0000000000004070 _Z19actionOnDoubleQubitP6float2S0_mPm + 0
-000000000020c140  0000002b00000007 R_X86_64_JUMP_SLOT     0000000000003fa0 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm + 0
+000000000020c138  0000002a00000007 R_X86_64_JUMP_SLOT     0000000000004080 _Z19actionOnDoubleQubitP6float2S0_mPm + 0
+000000000020c140  0000002b00000007 R_X86_64_JUMP_SLOT     0000000000003fb0 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm + 0
 000000000020c148  0000002d00000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
 000000000020c150  0000002e00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaMemcpy@libcudart.so.12 + 0
 000000000020c158  0000002f00000007 R_X86_64_JUMP_SLOT     0000000000000000 exit@GLIBC_2.2.5 + 0
 000000000020c160  0000003000000007 R_X86_64_JUMP_SLOT     0000000000002200 _Z8tdg_gateP6float2 + 0
 000000000020c168  0000003100000007 R_X86_64_JUMP_SLOT     0000000000002690 _Z7cz_gateP6float2 + 0
-000000000020c170  0000003200000007 R_X86_64_JUMP_SLOT     0000000000004620 _Z18actionOnTripleGateP6float2S0_mPm + 0
+000000000020c170  0000003200000007 R_X86_64_JUMP_SLOT     0000000000004630 _Z18actionOnTripleGateP6float2S0_mPm + 0
 000000000020c178  0000003300000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
-000000000020c180  0000003500000007 R_X86_64_JUMP_SLOT     0000000000003960 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm + 0
+000000000020c180  0000003500000007 R_X86_64_JUMP_SLOT     0000000000003970 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm + 0
 000000000020c188  0000003600000007 R_X86_64_JUMP_SLOT     0000000000003490 _Z14getArrayLengthPi + 0
 000000000020c190  0000003700000007 R_X86_64_JUMP_SLOT     00000000000021c0 _Z8sdg_gateP6float2 + 0
 000000000020c198  0000003800000007 R_X86_64_JUMP_SLOT     0000000000000000 strcmp@GLIBC_2.2.5 + 0
 000000000020c1a0  0000003900000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFunction@libcudart.so.12 + 0
 000000000020c1a8  0000003a00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaFree@libcudart.so.12 + 0
 000000000020c1b0  0000003b00000007 R_X86_64_JUMP_SLOT     0000000000002ba0 _Z20toff_gate_target_bigP6float2 + 0
 000000000020c1b8  0000003c00000007 R_X86_64_JUMP_SLOT     00000000000027a0 _Z8ryy_gateP6float2f + 0
 000000000020c1c0  0000003e00000007 R_X86_64_JUMP_SLOT     0000000000000000 puts@GLIBC_2.2.5 + 0
-000000000020c1c8  0000004000000007 R_X86_64_JUMP_SLOT     0000000000003a30 _Z19actionOnSingleQubitP6float2S0_mPm + 0
+000000000020c1c8  0000004000000007 R_X86_64_JUMP_SLOT     0000000000003a40 _Z19actionOnSingleQubitP6float2S0_mPm + 0
 000000000020c1d0  0000004200000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPopCallConfiguration@libcudart.so.12 + 0
 000000000020c1d8  0000004300000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaDeviceSynchronize@libcudart.so.12 + 0
 000000000020c1e0  0000004500000007 R_X86_64_JUMP_SLOT     0000000000002320 _Z7rz_gateP6float2f + 0
 000000000020c1e8  0000004600000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPushCallConfiguration@libcudart.so.12 + 0
 000000000020c1f0  0000004700000007 R_X86_64_JUMP_SLOT     0000000000002220 _Z6h_gateP6float2 + 0
 000000000020c1f8  0000004800000007 R_X86_64_JUMP_SLOT     0000000000000000 sqrtf@GLIBC_2.2.5 + 0
 000000000020c200  0000004900000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinaryEnd@libcudart.so.12 + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -6,15 +6,15 @@
  0x0000000000000001 (NEEDED)             Shared library: [libpthread.so.0]
  0x0000000000000001 (NEEDED)             Shared library: [libdl.so.2]
  0x0000000000000001 (NEEDED)             Shared library: [libstdc++.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [libm.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [libgcc_s.so.1]
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x000000000000000c (INIT)               0x1b50
- 0x000000000000000d (FINI)               0x4a60
+ 0x000000000000000d (FINI)               0x4a70
  0x0000000000000019 (INIT_ARRAY)         0x20bd60
  0x000000000000001b (INIT_ARRAYSZ)       16 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x20bd70
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x0000000000000004 (HASH)               0x190
  0x0000000000000005 (STRTAB)             0xb80
  0x0000000000000006 (SYMTAB)             0x3e8
```

#### readelf --wide --debug-dump=rawline {}

```diff
@@ -38,18 +38,18 @@
   [0x00000048]  Special opcode 63: advance Address by 4 to 0x1b54 and Line by 2 to 68
   [0x00000049]  Special opcode 104: advance Address by 7 to 0x1b5b and Line by 1 to 69
   [0x0000004a]  Special opcode 48: advance Address by 3 to 0x1b5e and Line by 1 to 70
   [0x0000004b]  Special opcode 34: advance Address by 2 to 0x1b60 and Line by 1 to 71
   [0x0000004c]  Advance PC by 2 to 0x1b62
   [0x0000004e]  Extended opcode 1: End of Sequence
 
-  [0x00000051]  Extended opcode 2: set Address to 0x4a60
+  [0x00000051]  Extended opcode 2: set Address to 0x4a70
   [0x0000005c]  Advance Line by 83 to 84
   [0x0000005f]  Copy
-  [0x00000060]  Advance PC by 4 to 0x4a64
+  [0x00000060]  Advance PC by 4 to 0x4a74
   [0x00000062]  Extended opcode 1: End of Sequence
 
 
   Offset:                      0x65
   Length:                      999
   DWARF Version:               2
   Prologue Length:             965
@@ -138,23 +138,23 @@
   37	13	0	0	internaltypes.h
   38	13	0	0	pthread-functions.h
   39	13	0	0	libc-lockP.h
   40	0	0	0	exit.h
 
  Line Number Statements:
   [0x00000434]  Set column to 1
-  [0x00000436]  Extended opcode 2: set Address to 0x4a50
+  [0x00000436]  Extended opcode 2: set Address to 0x4a60
   [0x00000441]  Advance Line by 44 to 45
   [0x00000443]  Copy
   [0x00000444]  Set column to 3
-  [0x00000446]  Special opcode 6: advance Address by 0 to 0x4a50 and Line by 1 to 46 (view 1)
+  [0x00000446]  Special opcode 6: advance Address by 0 to 0x4a60 and Line by 1 to 46 (view 1)
   [0x00000447]  Set column to 10
   [0x00000449]  Set is_stmt to 0
   [0x0000044a]  Copy (view 2)
-  [0x0000044b]  Advance PC by 14 to 0x4a5e
+  [0x0000044b]  Advance PC by 14 to 0x4a6e
   [0x0000044d]  Extended opcode 1: End of Sequence
 
 
   Offset:                      0x450
   Length:                      93
   DWARF Version:               2
   Prologue Length:             47
@@ -189,15 +189,15 @@
   [0x00000489]  Extended opcode 2: set Address to 0x1b62
   [0x00000494]  Advance Line by 39 to 40
   [0x00000496]  Copy
   [0x00000497]  Special opcode 62: advance Address by 4 to 0x1b66 and Line by 1 to 41
   [0x00000498]  Advance PC by 1 to 0x1b67
   [0x0000049a]  Extended opcode 1: End of Sequence
 
-  [0x0000049d]  Extended opcode 2: set Address to 0x4a64
+  [0x0000049d]  Extended opcode 2: set Address to 0x4a74
   [0x000004a8]  Advance Line by 43 to 44
   [0x000004aa]  Copy
-  [0x000004ab]  Special opcode 62: advance Address by 4 to 0x4a68 and Line by 1 to 45
-  [0x000004ac]  Advance PC by 1 to 0x4a69
+  [0x000004ab]  Special opcode 62: advance Address by 4 to 0x4a78 and Line by 1 to 45
+  [0x000004ac]  Advance PC by 1 to 0x4a79
   [0x000004ae]  Extended opcode 1: End of Sequence
```

#### readelf --wide --debug-dump=info {}

```diff
@@ -18,15 +18,15 @@
    Abbrev Offset: 0x12
    Pointer Size:  8
  <0><5a>: Abbrev Number: 1 (DW_TAG_compile_unit)
     <5b>   DW_AT_producer    : (strp) (offset: 0x987): GNU C11 9.3.0 -mtune=generic -march=x86-64 -g -O2 -std=gnu11 -fgnu89-inline -fmerge-all-constants -frounding-math -fno-stack-protector -fmath-errno -fPIC -ftls-model=initial-exec
     <5f>   DW_AT_language    : (data1) 12	(ANSI C99)
     <60>   DW_AT_name        : (strp) (offset: 0x763): atexit.c
     <64>   DW_AT_comp_dir    : (strp) (offset: 0x4b2): /opt/glibc-2.31/stdlib
-    <68>   DW_AT_low_pc      : (addr) 0x4a50
+    <68>   DW_AT_low_pc      : (addr) 0x4a60
     <70>   DW_AT_high_pc     : (data8) 0xe
     <78>   DW_AT_stmt_list   : (sec_offset) 0x65
  <1><7c>: Abbrev Number: 2 (DW_TAG_base_type)
     <7d>   DW_AT_byte_size   : (data1) 8
     <7e>   DW_AT_encoding    : (data1) 5	(signed)
     <7f>   DW_AT_name        : (strp) (offset: 0x890): long int
  <1><83>: Abbrev Number: 3 (DW_TAG_typedef)
@@ -3992,28 +3992,28 @@
     <1e4c>   DW_AT_external    : (flag_present) 1
     <1e4c>   DW_AT_name        : (strp) (offset: 0x5e8): atexit
     <1e50>   DW_AT_decl_file   : (data1) 1
     <1e51>   DW_AT_decl_line   : (data1) 44
     <1e52>   DW_AT_decl_column : (data1) 1
     <1e53>   DW_AT_prototyped  : (flag_present) 1
     <1e53>   DW_AT_type        : (ref4) <0x96>, int
-    <1e57>   DW_AT_low_pc      : (addr) 0x4a50
+    <1e57>   DW_AT_low_pc      : (addr) 0x4a60
     <1e5f>   DW_AT_high_pc     : (data8) 0xe
     <1e67>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
     <1e69>   DW_AT_GNU_all_call_sites: (flag_present) 1
     <1e69>   DW_AT_sibling     : (ref4) <0x1e98>
  <2><1e6d>: Abbrev Number: 57 (DW_TAG_formal_parameter)
     <1e6e>   DW_AT_name        : (strp) (offset: 0x29c): func
     <1e72>   DW_AT_decl_file   : (data1) 1
     <1e73>   DW_AT_decl_line   : (data1) 44
     <1e74>   DW_AT_decl_column : (data1) 16
     <1e75>   DW_AT_type        : (ref4) <0xac4>
     <1e79>   DW_AT_location    : (sec_offset) 0 (location list)
  <2><1e7d>: Abbrev Number: 58 (DW_TAG_GNU_call_site)
-    <1e7e>   DW_AT_low_pc      : (addr) 0x4a5e
+    <1e7e>   DW_AT_low_pc      : (addr) 0x4a6e
     <1e86>   DW_AT_GNU_tail_call: (flag_present) 1
     <1e86>   DW_AT_abstract_origin: (ref4) <0x1e98>
  <3><1e8a>: Abbrev Number: 59 (DW_TAG_GNU_call_site_parameter)
     <1e8b>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <1e8d>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 55 	(DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)))
  <3><1e91>: Abbrev Number: 59 (DW_TAG_GNU_call_site_parameter)
     <1e92>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
```

#### readelf --wide --debug-dump=aranges {}

```diff
@@ -4,29 +4,29 @@
   Version:                  2
   Offset into .debug_info:  0
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
     0000000000001b50 0000000000000012
-    0000000000004a60 0000000000000004
+    0000000000004a70 0000000000000004
     0000000000000000 0000000000000000
   Length:                   44
   Version:                  2
   Offset into .debug_info:  0x4f
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
-    0000000000004a50 000000000000000e
+    0000000000004a60 000000000000000e
     0000000000000000 0000000000000000
   Length:                   60
   Version:                  2
   Offset into .debug_info:  0x1ea5
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
     0000000000001b62 0000000000000005
-    0000000000004a64 0000000000000005
+    0000000000004a74 0000000000000005
     0000000000000000 0000000000000000
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -411,267 +411,267 @@
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000450 000000000000004c 00000454 FDE cie=00000000 pc=00000000000036c0..0000000000003956
+00000450 000000000000004c 00000454 FDE cie=00000000 pc=00000000000036c0..0000000000003966
   DW_CFA_advance_loc: 2 to 00000000000036c2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_advance_loc: 19 to 00000000000036d5
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 19 to 00000000000036e8
+  DW_CFA_advance_loc: 14 to 00000000000036e3
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 18 to 00000000000036fa
+  DW_CFA_advance_loc: 14 to 00000000000036f1
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 18 to 000000000000370c
+  DW_CFA_advance_loc: 16 to 0000000000003701
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 16 to 000000000000371c
+  DW_CFA_advance_loc: 16 to 0000000000003711
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 38 to 0000000000003742
+  DW_CFA_advance_loc: 49 to 0000000000003742
   DW_CFA_def_cfa_offset: 288
-  DW_CFA_advance_loc2: 477 to 000000000000391f
+  DW_CFA_advance_loc2: 493 to 000000000000392f
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000003920
+  DW_CFA_advance_loc: 1 to 0000000000003930
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000003921
+  DW_CFA_advance_loc: 1 to 0000000000003931
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000003923
+  DW_CFA_advance_loc: 2 to 0000000000003933
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000003925
+  DW_CFA_advance_loc: 2 to 0000000000003935
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000003927
+  DW_CFA_advance_loc: 2 to 0000000000003937
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000003929
+  DW_CFA_advance_loc: 2 to 0000000000003939
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 0000000000003930
+  DW_CFA_advance_loc: 7 to 0000000000003940
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000004a0 000000000000002c 000004a4 FDE cie=00000000 pc=0000000000003960..0000000000003a29
-  DW_CFA_advance_loc: 7 to 0000000000003967
+000004a0 000000000000002c 000004a4 FDE cie=00000000 pc=0000000000003970..0000000000003a39
+  DW_CFA_advance_loc: 7 to 0000000000003977
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc1: 144 to 00000000000039f7
+  DW_CFA_advance_loc1: 144 to 0000000000003a07
   DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 11 to 0000000000003a02
+  DW_CFA_advance_loc: 11 to 0000000000003a12
   DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc: 30 to 0000000000003a20
+  DW_CFA_advance_loc: 30 to 0000000000003a30
   DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 1 to 0000000000003a21
+  DW_CFA_advance_loc: 1 to 0000000000003a31
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc: 7 to 0000000000003a28
+  DW_CFA_advance_loc: 7 to 0000000000003a38
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000004d0 0000000000000014 000004d4 FDE cie=00000000 pc=0000000000003a30..0000000000003a35
+000004d0 0000000000000014 000004d4 FDE cie=00000000 pc=0000000000003a40..0000000000003a45
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000004e8 000000000000004c 000004ec FDE cie=00000000 pc=0000000000003a40..0000000000003f9d
-  DW_CFA_advance_loc: 2 to 0000000000003a42
+000004e8 000000000000004c 000004ec FDE cie=00000000 pc=0000000000003a50..0000000000003fad
+  DW_CFA_advance_loc: 2 to 0000000000003a52
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 9 to 0000000000003a4b
+  DW_CFA_advance_loc: 9 to 0000000000003a5b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 17 to 0000000000003a5c
+  DW_CFA_advance_loc: 17 to 0000000000003a6c
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 13 to 0000000000003a69
+  DW_CFA_advance_loc: 13 to 0000000000003a79
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 15 to 0000000000003a78
+  DW_CFA_advance_loc: 15 to 0000000000003a88
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 16 to 0000000000003a88
+  DW_CFA_advance_loc: 16 to 0000000000003a98
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 50 to 0000000000003aba
+  DW_CFA_advance_loc: 50 to 0000000000003aca
   DW_CFA_def_cfa_offset: 256
-  DW_CFA_advance_loc2: 709 to 0000000000003d7f
+  DW_CFA_advance_loc2: 709 to 0000000000003d8f
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 0000000000003d83
+  DW_CFA_advance_loc: 4 to 0000000000003d93
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000003d84
+  DW_CFA_advance_loc: 1 to 0000000000003d94
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000003d86
+  DW_CFA_advance_loc: 2 to 0000000000003d96
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000003d88
+  DW_CFA_advance_loc: 2 to 0000000000003d98
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000003d8a
+  DW_CFA_advance_loc: 2 to 0000000000003d9a
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000003d8c
+  DW_CFA_advance_loc: 2 to 0000000000003d9c
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 12 to 0000000000003d98
+  DW_CFA_advance_loc: 12 to 0000000000003da8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000538 000000000000002c 0000053c FDE cie=00000000 pc=0000000000003fa0..0000000000004069
-  DW_CFA_advance_loc: 7 to 0000000000003fa7
+00000538 000000000000002c 0000053c FDE cie=00000000 pc=0000000000003fb0..0000000000004079
+  DW_CFA_advance_loc: 7 to 0000000000003fb7
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc1: 144 to 0000000000004037
+  DW_CFA_advance_loc1: 144 to 0000000000004047
   DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 11 to 0000000000004042
+  DW_CFA_advance_loc: 11 to 0000000000004052
   DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc: 30 to 0000000000004060
+  DW_CFA_advance_loc: 30 to 0000000000004070
   DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 1 to 0000000000004061
+  DW_CFA_advance_loc: 1 to 0000000000004071
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc: 7 to 0000000000004068
+  DW_CFA_advance_loc: 7 to 0000000000004078
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000568 0000000000000014 0000056c FDE cie=00000000 pc=0000000000004070..0000000000004075
+00000568 0000000000000014 0000056c FDE cie=00000000 pc=0000000000004080..0000000000004085
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000580 000000000000004c 00000584 FDE cie=00000000 pc=0000000000004080..000000000000454b
-  DW_CFA_advance_loc: 2 to 0000000000004082
+00000580 000000000000004c 00000584 FDE cie=00000000 pc=0000000000004090..000000000000455b
+  DW_CFA_advance_loc: 2 to 0000000000004092
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 9 to 000000000000408b
+  DW_CFA_advance_loc: 9 to 000000000000409b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 17 to 000000000000409c
+  DW_CFA_advance_loc: 17 to 00000000000040ac
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 15 to 00000000000040ab
+  DW_CFA_advance_loc: 15 to 00000000000040bb
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 16 to 00000000000040bb
+  DW_CFA_advance_loc: 16 to 00000000000040cb
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 13 to 00000000000040c8
+  DW_CFA_advance_loc: 13 to 00000000000040d8
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 22 to 00000000000040de
+  DW_CFA_advance_loc: 22 to 00000000000040ee
   DW_CFA_def_cfa_offset: 224
-  DW_CFA_advance_loc2: 698 to 0000000000004398
+  DW_CFA_advance_loc2: 698 to 00000000000043a8
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 000000000000439c
+  DW_CFA_advance_loc: 4 to 00000000000043ac
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000439d
+  DW_CFA_advance_loc: 1 to 00000000000043ad
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000439f
+  DW_CFA_advance_loc: 2 to 00000000000043af
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000043a1
+  DW_CFA_advance_loc: 2 to 00000000000043b1
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000043a3
+  DW_CFA_advance_loc: 2 to 00000000000043b3
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000043a5
+  DW_CFA_advance_loc: 2 to 00000000000043b5
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 11 to 00000000000043b0
+  DW_CFA_advance_loc: 11 to 00000000000043c0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000005d0 000000000000002c 000005d4 FDE cie=00000000 pc=0000000000004550..0000000000004619
-  DW_CFA_advance_loc: 7 to 0000000000004557
+000005d0 000000000000002c 000005d4 FDE cie=00000000 pc=0000000000004560..0000000000004629
+  DW_CFA_advance_loc: 7 to 0000000000004567
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc1: 144 to 00000000000045e7
+  DW_CFA_advance_loc1: 144 to 00000000000045f7
   DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 11 to 00000000000045f2
+  DW_CFA_advance_loc: 11 to 0000000000004602
   DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc: 30 to 0000000000004610
+  DW_CFA_advance_loc: 30 to 0000000000004620
   DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 1 to 0000000000004611
+  DW_CFA_advance_loc: 1 to 0000000000004621
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc: 7 to 0000000000004618
+  DW_CFA_advance_loc: 7 to 0000000000004628
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000600 0000000000000014 00000604 FDE cie=00000000 pc=0000000000004620..0000000000004625
+00000600 0000000000000014 00000604 FDE cie=00000000 pc=0000000000004630..0000000000004635
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000618 000000000000004c 0000061c FDE cie=00000000 pc=0000000000004630..0000000000004a49
-  DW_CFA_advance_loc: 2 to 0000000000004632
+00000618 000000000000004c 0000061c FDE cie=00000000 pc=0000000000004640..0000000000004a59
+  DW_CFA_advance_loc: 2 to 0000000000004642
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 9 to 000000000000463b
+  DW_CFA_advance_loc: 9 to 000000000000464b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 13 to 0000000000004648
+  DW_CFA_advance_loc: 13 to 0000000000004658
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 000000000000464d
+  DW_CFA_advance_loc: 5 to 000000000000465d
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000464e
+  DW_CFA_advance_loc: 1 to 000000000000465e
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 0000000000004652
+  DW_CFA_advance_loc: 4 to 0000000000004662
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 0000000000004659
+  DW_CFA_advance_loc: 7 to 0000000000004669
   DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc2: 595 to 00000000000048ac
+  DW_CFA_advance_loc2: 595 to 00000000000048bc
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 00000000000048b0
+  DW_CFA_advance_loc: 4 to 00000000000048c0
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000048b1
+  DW_CFA_advance_loc: 1 to 00000000000048c1
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000048b3
+  DW_CFA_advance_loc: 2 to 00000000000048c3
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000048b5
+  DW_CFA_advance_loc: 2 to 00000000000048c5
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000048b7
+  DW_CFA_advance_loc: 2 to 00000000000048c7
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000048b9
+  DW_CFA_advance_loc: 2 to 00000000000048c9
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 00000000000048c0
+  DW_CFA_advance_loc: 7 to 00000000000048d0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
 00000668 0000000000000044 0000066c FDE cie=00000000 pc=0000000000001fa0..000000000000205a
   DW_CFA_advance_loc: 1 to 0000000000001fa1
@@ -708,15 +708,15 @@
   DW_CFA_advance_loc: 16 to 0000000000002048
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 13 to 0000000000002055
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
 
-000006b0 0000000000000014 000006b4 FDE cie=00000000 pc=0000000000004a50..0000000000004a5e
+000006b0 0000000000000014 000006b4 FDE cie=00000000 pc=0000000000004a60..0000000000004a6e
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
```

#### readelf --wide --debug-dump=loc {}

```diff
@@ -1,7 +1,7 @@
 Contents of the .debug_loc section:
 
     Offset   Begin            End              Expression
-    00000000 0000000000004a50 0000000000004a5d (DW_OP_reg5 (rdi))
-    00000013 0000000000004a5d 0000000000004a5e (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
+    00000000 0000000000004a60 0000000000004a6d (DW_OP_reg5 (rdi))
+    00000013 0000000000004a6d 0000000000004a6e (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
     00000029 <End of list>
```

#### readelf --wide --debug-dump=ranges {}

```diff
@@ -4,29 +4,29 @@
   Version:                  2
   Offset into .debug_info:  0
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
     0000000000001b50 0000000000000012
-    0000000000004a60 0000000000000004
+    0000000000004a70 0000000000000004
     0000000000000000 0000000000000000
   Length:                   44
   Version:                  2
   Offset into .debug_info:  0x4f
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
-    0000000000004a50 000000000000000e
+    0000000000004a60 000000000000000e
     0000000000000000 0000000000000000
   Length:                   60
   Version:                  2
   Offset into .debug_info:  0x1ea5
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
     0000000000001b62 0000000000000005
-    0000000000004a64 0000000000000005
+    0000000000004a74 0000000000000005
     0000000000000000 0000000000000000
```

#### strings --all --bytes=8 {}

```diff
@@ -73,14 +73,15 @@
 __cxa_atexit
 __bss_start
 GLIBC_2.2.5
 []A\A]A^A_
 []A\A]A^A_
 []A\A]A^A_
 []A\A]A^A_
+gateName: %s
 pos_array_size = %d
 Must be have two action position!, gateName: %s
 action position must be different!
 Must be have three action position!
 _Z18actionOnTripleGateP6float2S0_mPm
 _Z19actionOnDoubleQubitP6float2S0_mPm
 _Z19actionOnSingleQubitP6float2S0_mPm
@@ -470,15 +471,15 @@
 ptr___pthread_cond_init
 __exit_funcs
 ptr__pthread_cleanup_pop_restore
 _Unwind_Exception_Cleanup_Fn
 __routine
 __pthread_mutex_s
 __mon_yday
-tmpxft_00005715_00000000-6_tgq_simulator.cudafe1.cpp
+tmpxft_00005772_00000000-6_tgq_simulator.cudafe1.cpp
 fatbinData
 _ZL26__cudaUnregisterBinaryUtilv
 _ZL20__cudaFatCubinHandle
 _ZL24__sti____cudaRegisterAllv
 _ZL15__fatDeviceText
 crtstuff.c
 deregister_tm_clones
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -62,40 +62,40 @@
   0x00000f30 005f5a34 68617368 504b6300 5f5a3969 ._Z4hashPKc._Z9i
   0x00000f40 73496e41 72726179 50504b63 50636900 sInArrayPPKcPci.
   0x00000f50 73747263 6d70005f 5a313467 65744172 strcmp._Z14getAr
   0x00000f60 7261794c 656e6774 68506900 5f5a3133 rayLengthPi._Z13
   0x00000f70 6e6f726d 616c697a 6174696f 6e503666 normalizationP6f
   0x00000f80 6c6f6174 32690065 78656375 74655f63 loat2i.execute_c
   0x00000f90 69726375 69740073 696e676c 65476174 ircuit.singleGat
-  0x00000fa0 65416374 696f6e00 646f7562 6c654761 eAction.doubleGa
-  0x00000fb0 74654163 74696f6e 00747269 706c6547 teAction.tripleG
-  0x00000fc0 61746541 6374696f 6e005f5a 35315f5f ateAction._Z51__
-  0x00000fd0 64657669 63655f73 7475625f 5f5a3139 device_stub__Z19
-  0x00000fe0 61637469 6f6e4f6e 53696e67 6c655175 actionOnSingleQu
-  0x00000ff0 62697450 36666c6f 61743253 305f6d50 bitP6float2S0_mP
-  0x00001000 6d503666 6c6f6174 3253305f 6d506d00 mP6float2S0_mPm.
-  0x00001010 5f5f6375 6461506f 7043616c 6c436f6e __cudaPopCallCon
-  0x00001020 66696775 72617469 6f6e005f 5a313961 figuration._Z19a
-  0x00001030 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
-  0x00001040 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
-  0x00001050 00637564 614c6175 6e63684b 65726e65 .cudaLaunchKerne
-  0x00001060 6c006375 64615365 74446576 69636500 l.cudaSetDevice.
-  0x00001070 6d616c6c 6f630063 7564614d 616c6c6f malloc.cudaMallo
-  0x00001080 63006375 64614d65 6d637079 005f5f63 c.cudaMemcpy.__c
-  0x00001090 75646150 75736843 616c6c43 6f6e6669 udaPushCallConfi
-  0x000010a0 67757261 74696f6e 00637564 61446576 guration.cudaDev
-  0x000010b0 69636553 796e6368 726f6e69 7a650063 iceSynchronize.c
-  0x000010c0 75646146 72656500 66726565 005f5a35 udaFree.free._Z5
-  0x000010d0 315f5f64 65766963 655f7374 75625f5f 1__device_stub__
-  0x000010e0 5a313961 6374696f 6e4f6e44 6f75626c Z19actionOnDoubl
-  0x000010f0 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
-  0x00001100 5f6d506d 5036666c 6f617432 53305f6d _mPmP6float2S0_m
-  0x00001110 506d005f 5a313961 6374696f 6e4f6e44 Pm._Z19actionOnD
-  0x00001120 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x00001130 74325330 5f6d506d 00707269 6e746600 t2S0_mPm.printf.
+  0x00000fa0 65416374 696f6e00 7072696e 74660064 eAction.printf.d
+  0x00000fb0 6f75626c 65476174 65416374 696f6e00 oubleGateAction.
+  0x00000fc0 74726970 6c654761 74654163 74696f6e tripleGateAction
+  0x00000fd0 005f5a35 315f5f64 65766963 655f7374 ._Z51__device_st
+  0x00000fe0 75625f5f 5a313961 6374696f 6e4f6e53 ub__Z19actionOnS
+  0x00000ff0 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
+  0x00001000 74325330 5f6d506d 5036666c 6f617432 t2S0_mPmP6float2
+  0x00001010 53305f6d 506d005f 5f637564 61506f70 S0_mPm.__cudaPop
+  0x00001020 43616c6c 436f6e66 69677572 6174696f CallConfiguratio
+  0x00001030 6e005f5a 31396163 74696f6e 4f6e5369 n._Z19actionOnSi
+  0x00001040 6e676c65 51756269 74503666 6c6f6174 ngleQubitP6float
+  0x00001050 3253305f 6d506d00 63756461 4c61756e 2S0_mPm.cudaLaun
+  0x00001060 63684b65 726e656c 00637564 61536574 chKernel.cudaSet
+  0x00001070 44657669 6365006d 616c6c6f 63006375 Device.malloc.cu
+  0x00001080 64614d61 6c6c6f63 00637564 614d656d daMalloc.cudaMem
+  0x00001090 63707900 5f5f6375 64615075 73684361 cpy.__cudaPushCa
+  0x000010a0 6c6c436f 6e666967 75726174 696f6e00 llConfiguration.
+  0x000010b0 63756461 44657669 63655379 6e636872 cudaDeviceSynchr
+  0x000010c0 6f6e697a 65006375 64614672 65650066 onize.cudaFree.f
+  0x000010d0 72656500 5f5a3531 5f5f6465 76696365 ree._Z51__device
+  0x000010e0 5f737475 625f5f5a 31396163 74696f6e _stub__Z19action
+  0x000010f0 4f6e446f 75626c65 51756269 74503666 OnDoubleQubitP6f
+  0x00001100 6c6f6174 3253305f 6d506d50 36666c6f loat2S0_mPmP6flo
+  0x00001110 61743253 305f6d50 6d005f5a 31396163 at2S0_mPm._Z19ac
+  0x00001120 74696f6e 4f6e446f 75626c65 51756269 tionOnDoubleQubi
+  0x00001130 74503666 6c6f6174 3253305f 6d506d00 tP6float2S0_mPm.
   0x00001140 71736f72 74007075 7473005f 5a35305f qsort.puts._Z50_
   0x00001150 5f646576 6963655f 73747562 5f5f5a31 _device_stub__Z1
   0x00001160 38616374 696f6e4f 6e547269 706c6547 8actionOnTripleG
   0x00001170 61746550 36666c6f 61743253 305f6d50 ateP6float2S0_mP
   0x00001180 6d503666 6c6f6174 3253305f 6d506d00 mP6float2S0_mPm.
   0x00001190 5f5a3138 61637469 6f6e4f6e 54726970 _Z18actionOnTrip
   0x000011a0 6c654761 74655036 666c6f61 74325330 leGateP6float2S0
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -8,53 +8,53 @@
 	push   %rbp
 	lea    0x20a288(%rip),%rdi        
 	call   1d60 <__cudaRegisterFatBinary@plt>
 	push   $0x0
 	xor    %r9d,%r9d
 	mov    $0xffffffff,%r8d
 	push   $0x0
-	lea    0x2be7(%rip),%rcx        
+	lea    0x2c07(%rip),%rcx        
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	push   $0x0
 	mov    0x209ff8(%rip),%rsi        
 	mov    %rcx,%rdx
 	push   $0x0
 	mov    %rax,0x20a274(%rip)        
 	call   1e90 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
-	lea    0x2bdc(%rip),%rcx        
+	lea    0x2bfc(%rip),%rcx        
 	mov    0x209fc5(%rip),%rsi        
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   1e90 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
-	lea    0x2bd6(%rip),%rcx        
+	lea    0x2bf6(%rip),%rcx        
 	mov    0x209faf(%rip),%rsi        
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   1e90 <__cudaRegisterFunction@plt>
 	mov    0x20a20c(%rip),%rdi        
 	add    $0x20,%rsp
 	call   1f50 <__cudaRegisterFatBinaryEnd@plt>
 	lea    0xdc(%rip),%rdi        
 	pop    %rbp
-	jmp    4a50 <atexit>
+	jmp    4a60 <atexit>
 	nopw   0x0(%rax,%rax,1)
 
 0000000000002060 <deregister_tm_clones>:
 deregister_tm_clones():
 	lea    0x20a1c9(%rip),%rdi        
 	lea    0x20a1c2(%rip),%rax        
 	cmp    %rdi,%rax
@@ -122,97 +122,97 @@
 __cudaUnregisterBinaryUtil():
 	mov    0x20a119(%rip),%rdi        
 	jmp    1c40 <__cudaUnregisterFatBinary@plt>
 	nopl   0x0(%rax)
 
 0000000000002140 <x_gate(float2*)>:
 x_gate(float2*):
-	movaps 0x2ad9(%rip),%xmm0        
+	movaps 0x2af9(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movss  0x2ade(%rip),%xmm0        
+	movss  0x2afe(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
 0000000000002160 <y_gate(float2*)>:
 y_gate(float2*):
-	movaps 0x2ad9(%rip),%xmm0        
+	movaps 0x2af9(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2adf(%rip),%xmm0        
+	movaps 0x2aff(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000002180 <z_gate(float2*)>:
 z_gate(float2*):
-	movss  0x2aa8(%rip),%xmm0        
+	movss  0x2ac8(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2ace(%rip),%xmm0        
+	movaps 0x2aee(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
 00000000000021a0 <s_gate(float2*)>:
 s_gate(float2*):
-	movss  0x2a88(%rip),%xmm0        
+	movss  0x2aa8(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2abe(%rip),%xmm0        
+	movaps 0x2ade(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
 00000000000021c0 <sdg_gate(float2*)>:
 sdg_gate(float2*):
-	movss  0x2a68(%rip),%xmm0        
+	movss  0x2a88(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2a6e(%rip),%xmm0        
+	movaps 0x2a8e(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
 00000000000021e0 <t_gate(float2*)>:
 t_gate(float2*):
-	movss  0x2a48(%rip),%xmm0        
+	movss  0x2a68(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2a8e(%rip),%xmm0        
+	movaps 0x2aae(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
 0000000000002200 <tdg_gate(float2*)>:
 tdg_gate(float2*):
-	movss  0x2a28(%rip),%xmm0        
+	movss  0x2a48(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2a7e(%rip),%xmm0        
+	movaps 0x2a9e(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
 0000000000002220 <h_gate(float2*)>:
 h_gate(float2*):
-	movaps 0x2a79(%rip),%xmm0        
+	movaps 0x2a99(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2a7f(%rip),%xmm0        
+	movaps 0x2a9f(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000002240 <rx_gate(float2*, float)>:
 rx_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x2b20(%rip),%xmm0        
+	mulss  0x2b40(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
 	call   1c80 <sincosf@plt>
 	movss  0x8(%rsp),%xmm1
 	movss  0xc(%rsp),%xmm0
 	movq   $0x0,0x4(%rbx)
-	xorps  0x2a46(%rip),%xmm0        
+	xorps  0x2a66(%rip),%xmm0        
 	movl   $0x0,0x10(%rbx)
 	movl   $0x0,0x1c(%rbx)
 	movss  %xmm1,(%rbx)
 	movss  %xmm0,0xc(%rbx)
 	movss  %xmm0,0x14(%rbx)
 	movss  %xmm1,0x18(%rbx)
 	add    $0x10,%rsp
@@ -222,24 +222,24 @@
 	cs nopw 0x0(%rax,%rax,1)
 
 00000000000022b0 <ry_gate(float2*, float)>:
 ry_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x2ab0(%rip),%xmm0        
+	mulss  0x2ad0(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
 	call   1c80 <sincosf@plt>
 	movss  0xc(%rsp),%xmm1
 	movss  0x8(%rsp),%xmm0
 	movl   $0x0,0x4(%rbx)
 	movl   $0x0,0xc(%rbx)
 	movaps %xmm1,%xmm2
-	xorps  0x29cd(%rip),%xmm2        
+	xorps  0x29ed(%rip),%xmm2        
 	movl   $0x0,0x14(%rbx)
 	movl   $0x0,0x1c(%rbx)
 	movss  %xmm0,(%rbx)
 	movss  %xmm2,0x8(%rbx)
 	movss  %xmm1,0x10(%rbx)
 	movss  %xmm0,0x18(%rbx)
 	add    $0x10,%rsp
@@ -248,45 +248,45 @@
 	nopw   0x0(%rax,%rax,1)
 
 0000000000002320 <rz_gate(float2*, float)>:
 rz_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x2a40(%rip),%xmm0        
+	mulss  0x2a60(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
 	call   1c80 <sincosf@plt>
 	movss  0xc(%rsp),%xmm0
 	movss  0x8(%rsp),%xmm1
 	movq   $0x0,0x8(%rbx)
 	movq   $0x0,0x10(%rbx)
 	movaps %xmm0,%xmm2
-	xorps  0x295b(%rip),%xmm2        
+	xorps  0x297b(%rip),%xmm2        
 	movss  %xmm1,(%rbx)
 	movss  %xmm1,0x18(%rbx)
 	movss  %xmm2,0x4(%rbx)
 	movss  %xmm0,0x1c(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	xchg   %ax,%ax
 
 0000000000002380 <damp_i_gate(float2*, float)>:
 damp_i_gate(float2*, float):
 	pxor   %xmm3,%xmm3
 	comiss %xmm3,%xmm0
 	jbe    2396 <damp_i_gate(float2*, float)+0x16>
-	movss  0x29e3(%rip),%xmm1        
+	movss  0x2a03(%rip),%xmm1        
 	comiss %xmm0,%xmm1
 	ja     23a0 <damp_i_gate(float2*, float)+0x20>
 	ret
 	nopw   0x0(%rax,%rax,1)
 	subss  %xmm0,%xmm1
-	movss  0x2884(%rip),%xmm2        
+	movss  0x28a4(%rip),%xmm2        
 	movq   $0x0,0x10(%rdi)
 	movups %xmm2,(%rdi)
 	ucomiss %xmm1,%xmm3
 	movaps %xmm1,%xmm2
 	sqrtss %xmm2,%xmm2
 	ja     23d0 <damp_i_gate(float2*, float)+0x50>
 	movl   $0x0,0x1c(%rdi)
@@ -307,15 +307,15 @@
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000002410 <pd_gate(float2*, float)>:
 pd_gate(float2*, float):
 	pxor   %xmm2,%xmm2
 	comiss %xmm2,%xmm0
 	jbe    2426 <pd_gate(float2*, float)+0x16>
-	movss  0x2953(%rip),%xmm1        
+	movss  0x2973(%rip),%xmm1        
 	comiss %xmm0,%xmm1
 	ja     2430 <pd_gate(float2*, float)+0x20>
 	ret
 	nopw   0x0(%rax,%rax,1)
 	ucomiss %xmm0,%xmm2
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x10(%rdi)
@@ -339,15 +339,15 @@
 	nopl   0x0(%rax,%rax,1)
 
 0000000000002490 <ad_gate(float2*, float)>:
 ad_gate(float2*, float):
 	pxor   %xmm2,%xmm2
 	comiss %xmm2,%xmm0
 	jbe    24a6 <ad_gate(float2*, float)+0x16>
-	movss  0x28d3(%rip),%xmm1        
+	movss  0x28f3(%rip),%xmm1        
 	comiss %xmm0,%xmm1
 	ja     24b0 <ad_gate(float2*, float)+0x20>
 	ret
 	nopw   0x0(%rax,%rax,1)
 	sub    $0x18,%rsp
 	ucomiss %xmm0,%xmm2
 	movaps %xmm0,%xmm1
@@ -367,42 +367,42 @@
 	movss  0x4(%rsp),%xmm1
 	jmp    24c7 <ad_gate(float2*, float)+0x37>
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000002510 <swap_gate(float2*)>:
 swap_gate(float2*):
-	movss  0x2718(%rip),%xmm1        
+	movss  0x2738(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
 	movups %xmm1,(%rdi)
 	movups %xmm1,0x30(%rdi)
-	movaps 0x26f6(%rip),%xmm1        
+	movaps 0x2716(%rip),%xmm1        
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x20(%rdi)
 	movups %xmm1,0x40(%rdi)
 	movups %xmm0,0x50(%rdi)
 	movups %xmm0,0x60(%rdi)
 	movups %xmm1,0x70(%rdi)
 	ret
 	nopl   (%rax)
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000002550 <iswap_gate(float2*)>:
 iswap_gate(float2*):
-	movaps 0x26f9(%rip),%xmm1        
-	movss  0x26d1(%rip),%xmm0        
+	movaps 0x2719(%rip),%xmm1        
+	movss  0x26f1(%rip),%xmm0        
 	movups %xmm0,(%rdi)
 	pxor   %xmm0,%xmm0
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x20(%rdi)
 	movups %xmm1,0x30(%rdi)
-	movaps 0x26f7(%rip),%xmm1        
+	movaps 0x2717(%rip),%xmm1        
 	movups %xmm0,0x50(%rdi)
 	movups %xmm0,0x60(%rdi)
-	movaps 0x2698(%rip),%xmm0        
+	movaps 0x26b8(%rip),%xmm0        
 	movups %xmm1,0x40(%rdi)
 	movups %xmm0,0x70(%rdi)
 	ret
 	nopl   0x0(%rax,%rax,1)
 	cs nopw 0x0(%rax,%rax,1)
 
 00000000000025a0 <cphase_gate(float2*, float)>:
@@ -410,16 +410,16 @@
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
 	call   1c80 <sincosf@plt>
 	pxor   %xmm0,%xmm0
-	movaps 0x265e(%rip),%xmm2        
-	movss  0x2666(%rip),%xmm1        
+	movaps 0x267e(%rip),%xmm2        
+	movss  0x2686(%rip),%xmm1        
 	movups %xmm0,0x10(%rbx)
 	movups %xmm0,0x30(%rbx)
 	movups %xmm0,0x40(%rbx)
 	movups %xmm0,0x60(%rbx)
 	movss  0x8(%rsp),%xmm0
 	movq   $0x0,0x70(%rbx)
 	movss  %xmm0,0x78(%rbx)
@@ -431,34 +431,34 @@
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	nopl   0x0(%rax)
 
 0000000000002610 <cnot_gate_control_big(float2*)>:
 cnot_gate_control_big(float2*):
-	movaps 0x2609(%rip),%xmm2        
+	movaps 0x2629(%rip),%xmm2        
 	pxor   %xmm0,%xmm0
-	movss  0x260d(%rip),%xmm1        
+	movss  0x262d(%rip),%xmm1        
 	movups %xmm1,(%rdi)
 	movups %xmm0,0x10(%rdi)
 	movups %xmm2,0x20(%rdi)
 	movups %xmm0,0x30(%rdi)
 	movups %xmm0,0x40(%rdi)
 	movups %xmm2,0x50(%rdi)
 	movups %xmm0,0x60(%rdi)
 	movups %xmm1,0x70(%rdi)
 	ret
 	nopl   (%rax)
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000002650 <cnot_gate_control_small(float2*)>:
 cnot_gate_control_small(float2*):
-	movaps 0x25c9(%rip),%xmm1        
+	movaps 0x25e9(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
-	movss  0x25cd(%rip),%xmm2        
+	movss  0x25ed(%rip),%xmm2        
 	movups %xmm2,(%rdi)
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x20(%rdi)
 	movups %xmm1,0x30(%rdi)
 	movups %xmm0,0x40(%rdi)
 	movups %xmm2,0x50(%rdi)
 	movups %xmm1,0x60(%rdi)
@@ -466,41 +466,41 @@
 	ret
 	nopl   (%rax)
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000002690 <cz_gate(float2*)>:
 cz_gate(float2*):
 	pxor   %xmm0,%xmm0
-	movaps 0x2585(%rip),%xmm2        
-	movss  0x258d(%rip),%xmm1        
+	movaps 0x25a5(%rip),%xmm2        
+	movss  0x25ad(%rip),%xmm1        
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x30(%rdi)
 	movups %xmm0,0x40(%rdi)
 	movups %xmm0,0x60(%rdi)
-	movaps 0x25a6(%rip),%xmm0        
+	movaps 0x25c6(%rip),%xmm0        
 	movups %xmm1,(%rdi)
 	movups %xmm2,0x20(%rdi)
 	movups %xmm1,0x50(%rdi)
 	movups %xmm0,0x70(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
 00000000000026d0 <rxx_gate(float2*, float)>:
 rxx_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x2690(%rip),%xmm0        
+	mulss  0x26b0(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
 	call   1c80 <sincosf@plt>
 	movss  0x8(%rsp),%xmm1
 	movss  0xc(%rsp),%xmm0
 	movq   $0x0,0x4(%rbx)
-	xorps  0x25b6(%rip),%xmm0        
+	xorps  0x25d6(%rip),%xmm0        
 	movq   $0x0,0xc(%rbx)
 	movq   $0x0,0x14(%rbx)
 	movq   $0x0,0x20(%rbx)
 	movq   $0x0,0x2c(%rbx)
 	movq   $0x0,0x38(%rbx)
 	movq   $0x0,0x40(%rbx)
 	movl   $0x0,0x48(%rbx)
@@ -524,24 +524,24 @@
 	cs nopw 0x0(%rax,%rax,1)
 
 00000000000027a0 <ryy_gate(float2*, float)>:
 ryy_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x25c0(%rip),%xmm0        
+	mulss  0x25e0(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
 	call   1c80 <sincosf@plt>
 	movss  0xc(%rsp),%xmm1
 	movss  0x8(%rsp),%xmm0
 	movq   $0x0,0x4(%rbx)
 	movq   $0x0,0xc(%rbx)
 	movaps %xmm1,%xmm2
-	xorps  0x24db(%rip),%xmm2        
+	xorps  0x24fb(%rip),%xmm2        
 	movq   $0x0,0x14(%rbx)
 	movq   $0x0,0x20(%rbx)
 	movq   $0x0,0x2c(%rbx)
 	movq   $0x0,0x38(%rbx)
 	movq   $0x0,0x40(%rbx)
 	movl   $0x0,0x48(%rbx)
 	movq   $0x0,0x54(%rbx)
@@ -563,24 +563,24 @@
 	nopl   0x0(%rax,%rax,1)
 
 0000000000002870 <rzz_gate(float2*, float)>:
 rzz_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x24f0(%rip),%xmm0        
+	mulss  0x2510(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
 	call   1c80 <sincosf@plt>
 	movss  0xc(%rsp),%xmm1
 	movss  0x8(%rsp),%xmm0
 	movq   $0x0,0x8(%rbx)
 	movq   $0x0,0x10(%rbx)
 	movaps %xmm1,%xmm2
-	xorps  0x240b(%rip),%xmm2        
+	xorps  0x242b(%rip),%xmm2        
 	movq   $0x0,0x18(%rbx)
 	movq   $0x0,0x20(%rbx)
 	movq   $0x0,0x30(%rbx)
 	movq   $0x0,0x38(%rbx)
 	movq   $0x0,0x40(%rbx)
 	movq   $0x0,0x48(%rbx)
 	movq   $0x0,0x58(%rbx)
@@ -599,34 +599,34 @@
 	pop    %rbx
 	ret
 	nopl   0x0(%rax)
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000002940 <syc_gate(float2*)>:
 syc_gate(float2*):
-	movaps 0x2389(%rip),%xmm1        
-	movss  0x22e1(%rip),%xmm0        
+	movaps 0x23a9(%rip),%xmm1        
+	movss  0x2301(%rip),%xmm0        
 	movups %xmm0,(%rdi)
 	pxor   %xmm0,%xmm0
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x20(%rdi)
 	movups %xmm1,0x30(%rdi)
-	movaps 0x22d7(%rip),%xmm1        
+	movaps 0x22f7(%rip),%xmm1        
 	movups %xmm0,0x50(%rdi)
 	movups %xmm0,0x60(%rdi)
-	movaps 0x2368(%rip),%xmm0        
+	movaps 0x2388(%rip),%xmm0        
 	movups %xmm1,0x40(%rdi)
 	movups %xmm0,0x70(%rdi)
 	ret
 	nopl   0x0(%rax,%rax,1)
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000002990 <toff_gate_target_small(float2*)>:
 toff_gate_target_small(float2*):
-	movss  0x23dc(%rip),%xmm0        
+	movss  0x23fc(%rip),%xmm0        
 	xor    %eax,%eax
 	jmp    29b1 <toff_gate_target_small(float2*)+0x21>
 	nopl   0x0(%rax)
 	movss  %xmm0,(%rdi,%rax,8)
 	movl   $0x0,0x4(%rdi,%rax,8)
 	add    $0x1,%rax
 	cmp    $0x2f,%rax
@@ -645,26 +645,26 @@
 	movss  %xmm0,0x1f0(%rdi)
 	ret
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000002a00 <toff_gate_target_mid(float2*)>:
 toff_gate_target_mid(float2*):
-	movdqa 0x2328(%rip),%xmm4        
+	movdqa 0x2348(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x22d9(%rip),%xmm5        
+	movdqa 0x22f9(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x22d5(%rip),%xmm11        
-	movdqa 0x22dc(%rip),%xmm10        
+	movdqa 0x22f5(%rip),%xmm11        
+	movdqa 0x22fc(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x2300(%rip),%xmm8        
+	movaps 0x2320(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x22d3(%rip),%xmm9        
+	movdqa 0x22f3(%rip),%xmm9        
 	nopl   (%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -729,26 +729,26 @@
 	movq   $0x0,0x1f8(%rdi)
 	ret
 	nopl   0x0(%rax)
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000002ba0 <toff_gate_target_big(float2*)>:
 toff_gate_target_big(float2*):
-	movdqa 0x2188(%rip),%xmm4        
+	movdqa 0x21a8(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x2139(%rip),%xmm5        
+	movdqa 0x2159(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x2135(%rip),%xmm11        
-	movdqa 0x217c(%rip),%xmm10        
+	movdqa 0x2155(%rip),%xmm11        
+	movdqa 0x219c(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x2160(%rip),%xmm8        
+	movaps 0x2180(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x2133(%rip),%xmm9        
+	movdqa 0x2153(%rip),%xmm9        
 	nopl   (%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -802,37 +802,37 @@
 	movaps %xmm2,%xmm1
 	unpcklps %xmm6,%xmm1
 	unpckhps %xmm6,%xmm0
 	movups %xmm1,-0x20(%rax)
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
 	jne    2bf0 <toff_gate_target_big(float2*)+0x50>
-	movss  0x2071(%rip),%xmm0        
+	movss  0x2091(%rip),%xmm0        
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x0,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x0,0x1f8(%rdi)
 	movss  %xmm0,0xf8(%rdi)
 	movss  %xmm0,0x1d8(%rdi)
 	ret
 
 0000000000002d40 <fred_gate_control_big(float2*)>:
 fred_gate_control_big(float2*):
-	movdqa 0x1fe8(%rip),%xmm4        
+	movdqa 0x2008(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x1f99(%rip),%xmm5        
+	movdqa 0x1fb9(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x1f95(%rip),%xmm11        
-	movdqa 0x1f9c(%rip),%xmm10        
+	movdqa 0x1fb5(%rip),%xmm11        
+	movdqa 0x1fbc(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x1fc0(%rip),%xmm8        
+	movaps 0x1fe0(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x1fd3(%rip),%xmm9        
+	movdqa 0x1ff3(%rip),%xmm9        
 	nopl   (%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -886,37 +886,37 @@
 	movaps %xmm2,%xmm1
 	unpcklps %xmm6,%xmm1
 	unpckhps %xmm6,%xmm0
 	movups %xmm1,-0x20(%rax)
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
 	jne    2d90 <fred_gate_control_big(float2*)+0x50>
-	movss  0x1ed1(%rip),%xmm0        
+	movss  0x1ef1(%rip),%xmm0        
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x0,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x3f800000,0x1f8(%rdi)
 	movss  %xmm0,0x170(%rdi)
 	movss  %xmm0,0x1a8(%rdi)
 	ret
 
 0000000000002ee0 <fred_gate_control_mid(float2*)>:
 fred_gate_control_mid(float2*):
-	movdqa 0x1e48(%rip),%xmm4        
+	movdqa 0x1e68(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x1df9(%rip),%xmm5        
+	movdqa 0x1e19(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x1df5(%rip),%xmm11        
-	movdqa 0x1e3c(%rip),%xmm10        
+	movdqa 0x1e15(%rip),%xmm11        
+	movdqa 0x1e5c(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x1e20(%rip),%xmm8        
+	movaps 0x1e40(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x1e33(%rip),%xmm9        
+	movdqa 0x1e53(%rip),%xmm9        
 	nopl   (%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -970,37 +970,37 @@
 	movaps %xmm2,%xmm1
 	unpcklps %xmm6,%xmm1
 	unpckhps %xmm6,%xmm0
 	movups %xmm1,-0x20(%rax)
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
 	jne    2f30 <fred_gate_control_mid(float2*)+0x50>
-	movss  0x1d31(%rip),%xmm0        
+	movss  0x1d51(%rip),%xmm0        
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x0,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x3f800000,0x1f8(%rdi)
 	movss  %xmm0,0xf0(%rdi)
 	movss  %xmm0,0x198(%rdi)
 	ret
 
 0000000000003080 <fred_gate_control_small(float2*)>:
 fred_gate_control_small(float2*):
-	movdqa 0x1ca8(%rip),%xmm4        
+	movdqa 0x1cc8(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x1c59(%rip),%xmm5        
+	movdqa 0x1c79(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x1c55(%rip),%xmm11        
-	movdqa 0x1c9c(%rip),%xmm10        
+	movdqa 0x1c75(%rip),%xmm11        
+	movdqa 0x1cbc(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x1c80(%rip),%xmm8        
+	movaps 0x1ca0(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x1c43(%rip),%xmm9        
+	movdqa 0x1c63(%rip),%xmm9        
 	nopl   (%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -1054,29 +1054,29 @@
 	movaps %xmm2,%xmm1
 	unpcklps %xmm6,%xmm1
 	unpckhps %xmm6,%xmm0
 	movups %xmm1,-0x20(%rax)
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
 	jne    30d0 <fred_gate_control_small(float2*)+0x50>
-	movss  0x1b91(%rip),%xmm0        
+	movss  0x1bb1(%rip),%xmm0        
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x0,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x3f800000,0x1f8(%rdi)
 	movss  %xmm0,0xe8(%rdi)
 	movss  %xmm0,0x158(%rdi)
 	ret
 
 0000000000003220 <identityMat(float2*, int)>:
 identityMat(float2*, int):
 	lea    (%rsi,%rsi,1),%ecx
 	mov    %esi,%eax
 	mov    $0x1,%esi
-	movss  0x1b42(%rip),%xmm0        
+	movss  0x1b62(%rip),%xmm0        
 	mov    %esi,%edx
 	shl    %cl,%edx
 	lea    0x1(%rax),%ecx
 	shl    %cl,%esi
 	lea    -0x1(%rdx),%r8d
 	xor    %ecx,%ecx
 	test   %edx,%edx
@@ -1110,15 +1110,15 @@
 	call   1d70 <time@plt>
 	mov    %rax,%rdi
 	call   1d80 <srand@plt>
 	call   1c20 <rand@plt>
 	pxor   %xmm1,%xmm1
 	movss  0xc(%rsp),%xmm0
 	cvtsi2ss %eax,%xmm1
-	mulss  0x1ab4(%rip),%xmm1        
+	mulss  0x1ad4(%rip),%xmm1        
 	xor    %eax,%eax
 	comiss %xmm1,%xmm0
 	seta   %al
 	add    $0x18,%rsp
 	ret
 	nopl   0x0(%rax,%rax,1)
 	cs nopw 0x0(%rax,%rax,1)
@@ -1343,15 +1343,15 @@
 	lea    (%rdi,%rax,8),%rax
 	movss  (%rax),%xmm0
 	movss  0x4(%rax),%xmm1
 	mulss  %xmm0,%xmm0
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	addss  %xmm0,%xmm3
-	movsd  0x17b9(%rip),%xmm1        
+	movsd  0x17d9(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
 	cvtss2sd %xmm3,%xmm0
 	comisd %xmm0,%xmm1
 	ja     3638 <normalization(float2*, int)+0x178>
 	mov    %esi,%edx
 	movaps %xmm3,%xmm1
 	mov    %rdi,%rax
@@ -1378,15 +1378,15 @@
 	movss  0x4(%rax),%xmm0
 	divss  %xmm3,%xmm0
 	movss  %xmm0,0x4(%rax)
 	ret
 	nop
 	ret
 	nopl   0x0(%rax)
-	movss  0x1734(%rip),%xmm0        
+	movss  0x1754(%rip),%xmm0        
 	mov    %r8d,%ecx
 	xor    %eax,%eax
 	jmp    3663 <normalization(float2*, int)+0x1a3>
 	nopw   0x0(%rax,%rax,1)
 	movl   $0x0,(%rdi,%rax,8)
 	lea    0x1(%rax),%rdx
 	cmp    %rcx,%rax
@@ -1402,15 +1402,15 @@
 	lea    0xc(%rdi,%rax,8),%rax
 	xchg   %ax,%ax
 	movl   $0x0,(%rdx)
 	add    $0x8,%rdx
 	cmp    %rax,%rdx
 	jne    3680 <normalization(float2*, int)+0x1c0>
 	ret
-	movsd  0x16e8(%rip),%xmm1        
+	movsd  0x1708(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
 	cvtss2sd %xmm3,%xmm0
 	comisd %xmm0,%xmm1
 	ja     3638 <normalization(float2*, int)+0x178>
 	test   %ecx,%ecx
 	je     360d <normalization(float2*, int)+0x14d>
 	jmp    35d5 <normalization(float2*, int)+0x115>
@@ -1418,99 +1418,99 @@
 	pxor   %xmm3,%xmm3
 	jmp    354e <normalization(float2*, int)+0x8e>
 	xchg   %ax,%ax
 
 00000000000036c0 <execute_circuit>:
 execute_circuit():
 	push   %r15
-	lea    0x13b9(%rip),%rax        
+	lea    0x13c9(%rip),%rax        
 	mov    %rsi,%r9
-	lea    0x13df(%rip),%rsi        
+	lea    0x13af(%rip),%rsi        
 	push   %r14
 	movq   %rax,%xmm1
-	movq   %rsi,%xmm0
-	lea    0x138a(%rip),%rax        
+	lea    0x139f(%rip),%rax        
 	push   %r13
-	punpcklqdq %xmm1,%xmm0
 	movq   %rax,%xmm2
-	lea    0x137a(%rip),%rsi        
+	lea    0x1397(%rip),%rax        
 	push   %r12
-	lea    0x1375(%rip),%rax        
 	mov    %ecx,%r12d
-	lea    0x1379(%rip),%rcx        
+	lea    0x13c7(%rip),%rcx        
+	movq   %rax,%xmm3
 	push   %rbp
+	movq   %rcx,%xmm0
+	lea    0x13a1(%rip),%rcx        
 	mov    %rdi,%rbp
-	lea    0x1388(%rip),%rdi        
-	movq   %rax,%xmm3
 	push   %rbx
-	lea    0x1359(%rip),%rax        
+	punpcklqdq %xmm1,%xmm0
+	lea    0x1370(%rip),%rax        
+	lea    0x136b(%rip),%rdi        
 	movq   %rax,%xmm4
-	lea    0x1352(%rip),%rax        
+	lea    0x1362(%rip),%rax        
 	movq   %rax,%xmm5
-	lea    0x134c(%rip),%rax        
+	lea    0x135c(%rip),%rax        
 	sub    $0xe8,%rsp
 	movq   %rax,%xmm6
-	lea    0x1343(%rip),%rax        
+	lea    0x1353(%rip),%rax        
 	movaps %xmm0,0x70(%rsp)
-	movq   %rdi,%xmm0
+	movq   %rcx,%xmm0
 	movq   %rax,%xmm7
-	lea    0x1314(%rip),%rdi        
+	lea    0x1324(%rip),%rcx        
 	punpcklqdq %xmm2,%xmm0
-	lea    0x1325(%rip),%rax        
+	lea    0x1335(%rip),%rax        
 	movaps %xmm0,0x80(%rsp)
 	movq   %rsi,%xmm0
-	lea    0x12fb(%rip),%rsi        
+	lea    0x1311(%rip),%rsi        
 	movq   %rax,%xmm1
 	punpcklqdq %xmm3,%xmm0
-	lea    0x131e(%rip),%rax        
+	lea    0x132e(%rip),%rax        
 	movaps %xmm0,0x90(%rsp)
-	movq   %rdi,%xmm0
-	lea    0x12e7(%rip),%rdi        
+	movq   %rcx,%xmm0
+	lea    0x12f7(%rip),%rcx        
 	movq   %rax,%xmm2
 	punpcklqdq %xmm4,%xmm0
-	lea    0x12e9(%rip),%rax        
+	lea    0x12f9(%rip),%rax        
 	movaps %xmm0,0xa0(%rsp)
-	movq   %rsi,%xmm0
-	lea    0x12ea(%rip),%rsi        
+	movq   %rdi,%xmm0
+	lea    0x12fa(%rip),%rdi        
 	movq   %rax,%xmm3
 	punpcklqdq %xmm5,%xmm0
-	lea    0x12cd(%rip),%rax        
+	lea    0x12dd(%rip),%rax        
 	movaps %xmm0,0xb0(%rsp)
-	movq   %rcx,%xmm0
-	lea    0x12ab(%rip),%rcx        
+	movq   %rsi,%xmm0
+	lea    0x12bb(%rip),%rsi        
 	movq   %rax,%xmm4
 	punpcklqdq %xmm6,%xmm0
-	lea    0x12ad(%rip),%rax        
+	lea    0x12bd(%rip),%rax        
 	movaps %xmm0,0xc0(%rsp)
-	movq   %rdi,%xmm0
-	lea    0x128a(%rip),%rdi        
+	movq   %rcx,%xmm0
+	lea    0x129a(%rip),%rcx        
 	punpcklqdq %xmm7,%xmm0
 	mov    %rax,0x60(%rsp)
-	lea    0x1291(%rip),%rax        
+	lea    0x12a1(%rip),%rax        
 	movaps %xmm0,0xd0(%rsp)
-	movq   %rsi,%xmm0
-	lea    0x126d(%rip),%rsi        
+	movq   %rdi,%xmm0
+	lea    0x127d(%rip),%rdi        
 	movq   %rax,%xmm5
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x20(%rsp)
-	movq   %rcx,%xmm0
-	lea    0x125f(%rip),%rcx        
+	movq   %rsi,%xmm0
+	lea    0x126f(%rip),%rsi        
 	punpcklqdq %xmm2,%xmm0
 	movaps %xmm0,0x30(%rsp)
-	movq   %rdi,%xmm0
+	movq   %rcx,%xmm0
 	punpcklqdq %xmm3,%xmm0
 	movaps %xmm0,0x40(%rsp)
-	movq   %rsi,%xmm0
+	movq   %rdi,%xmm0
 	punpcklqdq %xmm4,%xmm0
 	movaps %xmm0,0x50(%rsp)
-	movq   %rcx,%xmm0
+	movq   %rsi,%xmm0
 	punpcklqdq %xmm5,%xmm0
 	movaps %xmm0,0x10(%rsp)
 	test   %edx,%edx
-	jle    3918 <execute_circuit+0x258>
+	jle    3928 <execute_circuit+0x268>
 	lea    -0x1(%rdx),%eax
 	mov    %r8d,%r13d
 	lea    0x70(%rsp),%r14
 	mov    %r9,%r15
 	lea    (%rax,%rax,2),%rax
 	lea    0x18(%r9,%rax,8),%rax
 	mov    %rax,(%rsp)
@@ -1524,30 +1524,34 @@
 	mov    %r13d,%r8d
 	mov    %r12d,%edx
 	mov    (%r15),%rdi
 	mov    %rbp,%rsi
 	add    $0x18,%r15
 	call   *%rbx
 	cmp    %r15,(%rsp)
-	je     3918 <execute_circuit+0x258>
+	je     3928 <execute_circuit+0x268>
+	mov    (%r15),%rsi
+	lea    0x11df(%rip),%rdi        
+	xor    %eax,%eax
+	call   1ba0 <printf@plt>
 	mov    (%r15),%rsi
 	mov    $0xe,%edx
 	mov    %r14,%rdi
 	call   1cf0 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
 	jne    38b8 <execute_circuit+0x1f8>
 	mov    (%r15),%rsi
 	mov    0x8(%rsp),%rdi
 	mov    $0x9,%edx
 	call   1cf0 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     3930 <execute_circuit+0x270>
-	mov    0x2086a6(%rip),%rbx        
+	je     3940 <execute_circuit+0x280>
+	mov    0x208695(%rip),%rbx        
 	jmp    38bf <execute_circuit+0x1ff>
-	nopl   0x0(%rax)
+	nopl   (%rax)
 	add    $0xe8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
@@ -1555,19 +1559,19 @@
 	nopw   0x0(%rax,%rax,1)
 	mov    (%r15),%rsi
 	lea    0x10(%rsp),%rdi
 	mov    $0x2,%edx
 	call   1cf0 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
 	je     38bf <execute_circuit+0x1ff>
-	mov    0x208697(%rip),%rbx        
+	mov    0x208687(%rip),%rbx        
 	jmp    38bf <execute_circuit+0x1ff>
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000003960 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000003970 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
 __device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*):
 	sub    $0x88,%rsp
 	lea    0x18(%rsp),%rax
 	mov    %rdi,0x18(%rsp)
 	lea    0x30(%rsp),%rdi
 	movq   %rax,%xmm0
 	lea    0x10(%rsp),%rax
@@ -1589,37 +1593,37 @@
 	punpcklqdq %xmm2,%xmm0
 	mov    %rax,0x30(%rsp)
 	mov    %rax,0x3c(%rsp)
 	movl   $0x1,0x44(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	call   1ef0 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
-	jne    3a21 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xc1>
+	jne    3a31 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xc1>
 	push   0x28(%rsp)
-	mov    0x2085da(%rip),%rdi        
+	mov    0x2085ca(%rip),%rdi        
 	push   0x28(%rsp)
 	mov    0x4c(%rsp),%rcx
 	mov    0x54(%rsp),%r8d
 	mov    0x40(%rsp),%rsi
 	mov    0x48(%rsp),%edx
 	lea    0x70(%rsp),%r9
 	call   1c00 <cudaLaunchKernel@plt>
 	pop    %rax
 	pop    %rdx
 	add    $0x88,%rsp
 	ret
 	nopl   0x0(%rax)
 
-0000000000003a30 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000003a40 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)>:
 actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*):
 	jmp    1e50 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000003a40 <singleGateAction>:
+0000000000003a50 <singleGateAction>:
 singleGateAction():
 	push   %r15
 	lea    0x1039(%rip),%rax        
 	push   %r14
 	movq   %rax,%xmm1
 	lea    0x1019(%rip),%rax        
 	mov    %rdi,%r14
@@ -1671,15 +1675,15 @@
 	punpcklqdq %xmm6,%xmm0
 	movaps %xmm0,0xa0(%rsp)
 	movq   %rsi,%xmm0
 	punpcklqdq %xmm7,%xmm0
 	movaps %xmm0,0xb0(%rsp)
 	call   1e60 <getArrayLength(int*)@plt>
 	cmp    $0x1,%eax
-	jne    3f5b <singleGateAction+0x51b>
+	jne    3f6b <singleGateAction+0x51b>
 	mov    %ebp,%edi
 	mov    %eax,%ebx
 	call   1f90 <cudaSetDevice@plt>
 	mov    $0x20,%edi
 	call   1e40 <malloc@plt>
 	mov    $0x8,%edi
 	mov    %rax,%r12
@@ -1712,15 +1716,15 @@
 	call   1bc0 <hash(char const*)@plt>
 	lea    0x50(%rsp),%rdi
 	mov    $0xe,%edx
 	mov    %r14,%rsi
 	mov    %eax,0x18(%rsp)
 	call   1cf0 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     3f65 <singleGateAction+0x525>
+	je     3f75 <singleGateAction+0x525>
 	mov    0x10(%rsp),%rsi
 	mov    0x8(%rsp),%rdx
 	mov    0x30(%rsp),%rdi
 	mov    (%rsi),%ecx
 	mov    %ebx,%esi
 	shl    %cl,%esi
 	add    $0x1,%ecx
@@ -1740,32 +1744,32 @@
 	mov    $0x8,%edx
 	mov    %rbp,%rsi
 	add    $0x1,%eax
 	mov    %eax,0x44(%rsp)
 	call   1df0 <cudaMemcpy@plt>
 	mov    0x18(%rsp),%r8d
 	cmp    $0x1bd,%r8d
-	je     3f48 <singleGateAction+0x508>
-	ja     3e20 <singleGateAction+0x3e0>
+	je     3f58 <singleGateAction+0x508>
+	ja     3e30 <singleGateAction+0x3e0>
 	cmp    $0x7d,%r8d
-	ja     3d98 <singleGateAction+0x358>
+	ja     3da8 <singleGateAction+0x358>
 	cmp    $0x6a,%r8d
-	jbe    3cf8 <singleGateAction+0x2b8>
+	jbe    3d08 <singleGateAction+0x2b8>
 	sub    $0x6b,%r8d
 	cmp    $0x12,%r8d
-	ja     3cf8 <singleGateAction+0x2b8>
-	lea    0xe10(%rip),%rdx        
+	ja     3d08 <singleGateAction+0x2b8>
+	lea    0xe20(%rip),%rdx        
 	movslq (%rdx,%r8,4),%rax
 	add    %rdx,%rax
 	jmp    *%rax
 	nopl   0x0(%rax)
 	cmp    $0x1d8,%r8d
-	je     3f30 <singleGateAction+0x4f0>
+	je     3f40 <singleGateAction+0x4f0>
 	cmp    $0x1d9,%r8d
-	jne    3e60 <singleGateAction+0x420>
+	jne    3e70 <singleGateAction+0x420>
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
 	call   1f10 <rz_gate(float2*, float)@plt>
 	mov    0x20(%rsp),%rdi
 	mov    $0x1,%ecx
 	mov    $0x20,%edx
 	mov    %r12,%rsi
@@ -1775,15 +1779,15 @@
 	xor    %r9d,%r9d
 	mov    0x38(%rsp),%rdx
 	mov    0x44(%rsp),%rdi
 	xor    %r8d,%r8d
 	mov    0x4c(%rsp),%esi
 	call   1f20 <__cudaPushCallConfiguration@plt>
 	test   %eax,%eax
-	je     3e80 <singleGateAction+0x440>
+	je     3e90 <singleGateAction+0x440>
 	call   1f00 <cudaDeviceSynchronize@plt>
 	mov    0x28(%rsp),%rsi
 	mov    %r15,%rdx
 	mov    %r13,%rdi
 	mov    $0x2,%ecx
 	call   1df0 <cudaMemcpy@plt>
 	mov    0x20(%rsp),%rdi
@@ -1801,15 +1805,15 @@
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	jmp    1de0 <free@plt>
 	nopl   0x0(%rax)
 	cmp    $0x190,%r8d
-	jne    3cf8 <singleGateAction+0x2b8>
+	jne    3d08 <singleGateAction+0x2b8>
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
 	call   1b90 <ad_gate(float2*, float)@plt>
 	mov    0x20(%rsp),%rdi
 	mov    $0x1,%ecx
 	mov    $0x20,%edx
 	mov    %r12,%rsi
@@ -1819,92 +1823,92 @@
 	xor    %r9d,%r9d
 	mov    0x38(%rsp),%rdx
 	mov    0x44(%rsp),%rdi
 	xor    %r8d,%r8d
 	mov    0x4c(%rsp),%esi
 	call   1f20 <__cudaPushCallConfiguration@plt>
 	test   %eax,%eax
-	je     3ef0 <singleGateAction+0x4b0>
+	je     3f00 <singleGateAction+0x4b0>
 	call   1f00 <cudaDeviceSynchronize@plt>
 	mov    0x28(%rsp),%rsi
 	mov    %r13,%rdi
 	mov    %r15,%rdx
 	mov    $0x2,%ecx
 	call   1df0 <cudaMemcpy@plt>
 	mov    0x4(%rsp),%esi
 	mov    %r13,%rdi
 	call   1da0 <normalization(float2*, int)@plt>
-	jmp    3d52 <singleGateAction+0x312>
+	jmp    3d62 <singleGateAction+0x312>
 	xchg   %ax,%ax
 	cmp    $0x5b9,%r8d
-	je     3f10 <singleGateAction+0x4d0>
-	jbe    3cd0 <singleGateAction+0x290>
+	je     3f20 <singleGateAction+0x4d0>
+	jbe    3ce0 <singleGateAction+0x290>
 	cmp    $0x5c2,%r8d
-	je     3f20 <singleGateAction+0x4e0>
+	je     3f30 <singleGateAction+0x4e0>
 	cmp    $0x914b,%r8d
-	jne    3cf8 <singleGateAction+0x2b8>
+	jne    3d08 <singleGateAction+0x2b8>
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
 	call   1d30 <damp_i_gate(float2*, float)@plt>
-	jmp    3db3 <singleGateAction+0x373>
+	jmp    3dc3 <singleGateAction+0x373>
 	cmp    $0x1d7,%r8d
-	jne    3cf8 <singleGateAction+0x2b8>
+	jne    3d08 <singleGateAction+0x2b8>
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
 	call   1f70 <rx_gate(float2*, float)@plt>
-	jmp    3cf8 <singleGateAction+0x2b8>
+	jmp    3d08 <singleGateAction+0x2b8>
 	mov    0x30(%rsp),%rcx
 	mov    0x8(%rsp),%rdx
 	mov    0x20(%rsp),%rsi
 	mov    0x28(%rsp),%rdi
 	call   1ee0 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
-	jmp    3d38 <singleGateAction+0x2f8>
+	jmp    3d48 <singleGateAction+0x2f8>
 	mov    %r12,%rdi
 	call   1db0 <z_gate(float2*)@plt>
-	jmp    3cf8 <singleGateAction+0x2b8>
+	jmp    3d08 <singleGateAction+0x2b8>
 	mov    %r12,%rdi
 	call   1f30 <h_gate(float2*)@plt>
-	jmp    3cf8 <singleGateAction+0x2b8>
+	jmp    3d08 <singleGateAction+0x2b8>
 	mov    %r12,%rdi
 	call   1d20 <s_gate(float2*)@plt>
-	jmp    3cf8 <singleGateAction+0x2b8>
+	jmp    3d08 <singleGateAction+0x2b8>
 	mov    %r12,%rdi
 	call   1d90 <t_gate(float2*)@plt>
-	jmp    3cf8 <singleGateAction+0x2b8>
+	jmp    3d08 <singleGateAction+0x2b8>
 	mov    %r12,%rdi
 	call   1d10 <x_gate(float2*)@plt>
-	jmp    3cf8 <singleGateAction+0x2b8>
+	jmp    3d08 <singleGateAction+0x2b8>
 	mov    %r12,%rdi
 	call   1bf0 <y_gate(float2*)@plt>
-	jmp    3cf8 <singleGateAction+0x2b8>
+	jmp    3d08 <singleGateAction+0x2b8>
 	nopl   0x0(%rax)
 	mov    0x30(%rsp),%rcx
 	mov    0x8(%rsp),%rdx
 	mov    0x20(%rsp),%rsi
 	mov    0x28(%rsp),%rdi
 	call   1ee0 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
-	jmp    3df3 <singleGateAction+0x3b3>
+	jmp    3e03 <singleGateAction+0x3b3>
 	xchg   %ax,%ax
 	mov    %r12,%rdi
 	call   1e70 <sdg_gate(float2*)@plt>
-	jmp    3cf8 <singleGateAction+0x2b8>
+	jmp    3d08 <singleGateAction+0x2b8>
 	nopl   (%rax)
 	mov    %r12,%rdi
 	call   1e10 <tdg_gate(float2*)@plt>
-	jmp    3cf8 <singleGateAction+0x2b8>
+	jmp    3d08 <singleGateAction+0x2b8>
 	nopl   (%rax)
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
 	call   1c70 <ry_gate(float2*, float)@plt>
-	jmp    3cf8 <singleGateAction+0x2b8>
+	jmp    3d08 <singleGateAction+0x2b8>
 	nopl   0x0(%rax,%rax,1)
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
 	call   1bd0 <pd_gate(float2*, float)@plt>
-	jmp    3db3 <singleGateAction+0x373>
+	jmp    3dc3 <singleGateAction+0x373>
 	mov    $0x1,%edi
 	call   1e00 <exit@plt>
 	mov    0x20(%rsp),%rdi
 	call   1ea0 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
 	call   1ea0 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
@@ -1913,15 +1917,15 @@
 	call   1de0 <free@plt>
 	mov    %rbp,%rdi
 	call   1de0 <free@plt>
 	mov    $0x3,%edi
 	call   1e00 <exit@plt>
 	nopl   (%rax)
 
-0000000000003fa0 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000003fb0 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
 __device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*):
 	sub    $0x88,%rsp
 	lea    0x18(%rsp),%rax
 	mov    %rdi,0x18(%rsp)
 	lea    0x30(%rsp),%rdi
 	movq   %rax,%xmm0
 	lea    0x10(%rsp),%rax
@@ -1943,37 +1947,37 @@
 	punpcklqdq %xmm2,%xmm0
 	mov    %rax,0x30(%rsp)
 	mov    %rax,0x3c(%rsp)
 	movl   $0x1,0x44(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	call   1ef0 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
-	jne    4061 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xc1>
+	jne    4071 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xc1>
 	push   0x28(%rsp)
-	mov    0x207f82(%rip),%rdi        
+	mov    0x207f72(%rip),%rdi        
 	push   0x28(%rsp)
 	mov    0x4c(%rsp),%rcx
 	mov    0x54(%rsp),%r8d
 	mov    0x40(%rsp),%rsi
 	mov    0x48(%rsp),%edx
 	lea    0x70(%rsp),%r9
 	call   1c00 <cudaLaunchKernel@plt>
 	pop    %rax
 	pop    %rdx
 	add    $0x88,%rsp
 	ret
 	nopl   0x0(%rax)
 
-0000000000004070 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000004080 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)>:
 actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*):
 	jmp    1dd0 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000004080 <doubleGateAction>:
+0000000000004090 <doubleGateAction>:
 doubleGateAction():
 	push   %r15
 	lea    0xa0b(%rip),%rax        
 	push   %r14
 	movq   %rax,%xmm1
 	lea    0xa1a(%rip),%rax        
 	mov    %rdi,%r14
@@ -2008,24 +2012,24 @@
 	movq   %rsi,%xmm0
 	punpcklqdq %xmm3,%xmm0
 	movaps %xmm0,0x70(%rsp)
 	movq   %rdx,%xmm0
 	punpcklqdq %xmm4,%xmm0
 	movaps %xmm0,0x80(%rsp)
 	call   1e60 <getArrayLength(int*)@plt>
-	lea    0x96e(%rip),%rdi        
+	lea    0x97c(%rip),%rdi        
 	mov    %eax,%ebp
 	mov    %eax,%esi
 	xor    %eax,%eax
 	call   1ba0 <printf@plt>
 	cmp    $0x2,%ebp
-	jne    44e2 <doubleGateAction+0x462>
+	jne    44f2 <doubleGateAction+0x462>
 	mov    0x4(%rbx),%eax
 	cmp    %eax,(%rbx)
-	je     4535 <doubleGateAction+0x4b5>
+	je     4545 <doubleGateAction+0x4b5>
 	mov    %r12d,%edi
 	call   1f90 <cudaSetDevice@plt>
 	mov    $0x80,%edi
 	call   1e40 <malloc@plt>
 	mov    $0x10,%edi
 	mov    %rax,%r12
 	call   1e40 <malloc@plt>
@@ -2058,24 +2062,24 @@
 	call   1bc0 <hash(char const*)@plt>
 	mov    0x4(%rbx),%ecx
 	mov    (%rbx),%esi
 	mov    $0x4,%edx
 	mov    %rbx,%rdi
 	mov    %eax,%r13d
 	mov    %ecx,0x1c(%rsp)
-	mov    0x207d7f(%rip),%rcx        
+	mov    0x207d6f(%rip),%rcx        
 	mov    %esi,0x18(%rsp)
 	mov    $0x2,%esi
 	call   1f80 <qsort@plt>
 	lea    0x50(%rsp),%rdi
 	mov    $0x9,%edx
 	mov    %r14,%rsi
 	call   1cf0 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     44fd <doubleGateAction+0x47d>
+	je     450d <doubleGateAction+0x47d>
 	mov    (%rbx),%edx
 	mov    $0x1,%r10d
 	mov    0x30(%rsp),%rdi
 	mov    %r10d,%esi
 	mov    %edx,%ecx
 	shl    %cl,%esi
 	mov    0x4(%rbx),%ecx
@@ -2103,21 +2107,21 @@
 	div    %rsi
 	mov    $0x10,%edx
 	mov    %rbp,%rsi
 	add    $0x1,%eax
 	mov    %eax,0x44(%rsp)
 	call   1df0 <cudaMemcpy@plt>
 	cmp    $0x5fd,%r13d
-	je     44b0 <doubleGateAction+0x430>
-	jbe    43b0 <doubleGateAction+0x330>
+	je     44c0 <doubleGateAction+0x430>
+	jbe    43c0 <doubleGateAction+0x330>
 	cmp    $0x1234,%r13d
-	je     44a0 <doubleGateAction+0x420>
-	jbe    43e0 <doubleGateAction+0x360>
+	je     44b0 <doubleGateAction+0x420>
+	jbe    43f0 <doubleGateAction+0x360>
 	cmp    $0x340f,%r13d
-	jne    4310 <doubleGateAction+0x290>
+	jne    4320 <doubleGateAction+0x290>
 	mov    %r12,%rdi
 	call   1d40 <iswap_gate(float2*)@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    0x20(%rsp),%rdi
 	mov    $0x1,%ecx
 	mov    $0x80,%edx
 	mov    %r12,%rsi
@@ -2127,15 +2131,15 @@
 	xor    %r9d,%r9d
 	mov    0x38(%rsp),%rdx
 	mov    0x44(%rsp),%rdi
 	xor    %r8d,%r8d
 	mov    0x4c(%rsp),%esi
 	call   1f20 <__cudaPushCallConfiguration@plt>
 	test   %eax,%eax
-	je     4448 <doubleGateAction+0x3c8>
+	je     4458 <doubleGateAction+0x3c8>
 	call   1f00 <cudaDeviceSynchronize@plt>
 	mov    0x28(%rsp),%rsi
 	mov    (%rsp),%rdi
 	mov    %r15,%rdx
 	mov    $0x2,%ecx
 	call   1df0 <cudaMemcpy@plt>
 	mov    0x20(%rsp),%rdi
@@ -2153,75 +2157,75 @@
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	jmp    1de0 <free@plt>
 	nopw   0x0(%rax,%rax,1)
 	cmp    $0x1ac,%r13d
-	je     44c8 <doubleGateAction+0x448>
-	jbe    4410 <doubleGateAction+0x390>
+	je     44d8 <doubleGateAction+0x448>
+	jbe    4420 <doubleGateAction+0x390>
 	cmp    $0x5f4,%r13d
-	jne    4310 <doubleGateAction+0x290>
+	jne    4320 <doubleGateAction+0x290>
 	mov    %r12,%rdi
 	call   1cb0 <syc_gate(float2*)@plt>
-	jmp    4310 <doubleGateAction+0x290>
+	jmp    4320 <doubleGateAction+0x290>
 	nopl   0x0(%rax)
 	cmp    $0x601,%r13d
-	je     4488 <doubleGateAction+0x408>
+	je     4498 <doubleGateAction+0x408>
 	cmp    $0x605,%r13d
-	jne    4310 <doubleGateAction+0x290>
+	jne    4320 <doubleGateAction+0x290>
 	movss  0x14(%rsp),%xmm0
 	mov    %r12,%rdi
 	call   1ce0 <rzz_gate(float2*, float)@plt>
-	jmp    4310 <doubleGateAction+0x290>
+	jmp    4320 <doubleGateAction+0x290>
 	nopl   (%rax)
 	cmp    $0x1a2,%r13d
-	je     4470 <doubleGateAction+0x3f0>
+	je     4480 <doubleGateAction+0x3f0>
 	cmp    $0x1aa,%r13d
-	jne    4310 <doubleGateAction+0x290>
+	jne    4320 <doubleGateAction+0x290>
 	mov    0x1c(%rsp),%edx
 	mov    %r12,%rdi
 	cmp    %edx,0x18(%rsp)
-	jle    44d8 <doubleGateAction+0x458>
+	jle    44e8 <doubleGateAction+0x458>
 	call   1d00 <cnot_gate_control_big(float2*)@plt>
-	jmp    4310 <doubleGateAction+0x290>
+	jmp    4320 <doubleGateAction+0x290>
 	nopl   0x0(%rax)
 	mov    0x30(%rsp),%rcx
 	mov    0x8(%rsp),%rdx
 	mov    0x20(%rsp),%rsi
 	mov    0x28(%rsp),%rdi
 	call   1dc0 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
-	jmp    4350 <doubleGateAction+0x2d0>
+	jmp    4360 <doubleGateAction+0x2d0>
 	cs nopw 0x0(%rax,%rax,1)
 	movss  0x14(%rsp),%xmm0
 	mov    %r12,%rdi
 	call   1b80 <cphase_gate(float2*, float)@plt>
-	jmp    4310 <doubleGateAction+0x290>
+	jmp    4320 <doubleGateAction+0x290>
 	nopl   0x0(%rax,%rax,1)
 	movss  0x14(%rsp),%xmm0
 	mov    %r12,%rdi
 	call   1ec0 <ryy_gate(float2*, float)@plt>
-	jmp    4310 <doubleGateAction+0x290>
+	jmp    4320 <doubleGateAction+0x290>
 	nopl   0x0(%rax,%rax,1)
 	mov    %r12,%rdi
 	call   1f60 <swap_gate(float2*)@plt>
-	jmp    4310 <doubleGateAction+0x290>
+	jmp    4320 <doubleGateAction+0x290>
 	nopl   (%rax)
 	movss  0x14(%rsp),%xmm0
 	mov    %r12,%rdi
 	call   1cc0 <rxx_gate(float2*, float)@plt>
-	jmp    4310 <doubleGateAction+0x290>
+	jmp    4320 <doubleGateAction+0x290>
 	nopl   0x0(%rax,%rax,1)
 	mov    %r12,%rdi
 	call   1e20 <cz_gate(float2*)@plt>
-	jmp    4310 <doubleGateAction+0x290>
+	jmp    4320 <doubleGateAction+0x290>
 	nopl   (%rax)
 	call   1c60 <cnot_gate_control_small(float2*)@plt>
-	jmp    4310 <doubleGateAction+0x290>
-	lea    0x637(%rip),%rdi        
+	jmp    4320 <doubleGateAction+0x290>
+	lea    0x647(%rip),%rdi        
 	mov    %r14,%rsi
 	xor    %eax,%eax
 	call   1ba0 <printf@plt>
 	mov    $0x1,%edi
 	call   1e00 <exit@plt>
 	mov    0x20(%rsp),%rdi
 	call   1ea0 <cudaFree@plt>
@@ -2231,21 +2235,21 @@
 	call   1ea0 <cudaFree@plt>
 	mov    %r12,%rdi
 	call   1de0 <free@plt>
 	mov    %rbp,%rdi
 	call   1de0 <free@plt>
 	mov    $0x3,%edi
 	call   1e00 <exit@plt>
-	lea    0x61c(%rip),%rdi        
+	lea    0x62c(%rip),%rdi        
 	call   1ed0 <puts@plt>
 	mov    $0x2,%edi
 	call   1e00 <exit@plt>
 	nopl   0x0(%rax,%rax,1)
 
-0000000000004550 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000004560 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
 __device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*):
 	sub    $0x88,%rsp
 	lea    0x18(%rsp),%rax
 	mov    %rdi,0x18(%rsp)
 	lea    0x30(%rsp),%rdi
 	movq   %rax,%xmm0
 	lea    0x10(%rsp),%rax
@@ -2267,37 +2271,37 @@
 	punpcklqdq %xmm2,%xmm0
 	mov    %rax,0x30(%rsp)
 	mov    %rax,0x3c(%rsp)
 	movl   $0x1,0x44(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	call   1ef0 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
-	jne    4611 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xc1>
+	jne    4621 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xc1>
 	push   0x28(%rsp)
-	mov    0x2079da(%rip),%rdi        
+	mov    0x2079ca(%rip),%rdi        
 	push   0x28(%rsp)
 	mov    0x4c(%rsp),%rcx
 	mov    0x54(%rsp),%r8d
 	mov    0x40(%rsp),%rsi
 	mov    0x48(%rsp),%edx
 	lea    0x70(%rsp),%r9
 	call   1c00 <cudaLaunchKernel@plt>
 	pop    %rax
 	pop    %rdx
 	add    $0x88,%rsp
 	ret
 	nopl   0x0(%rax)
 
-0000000000004620 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000004630 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)>:
 actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*):
 	jmp    1be0 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000004630 <tripleGateAction>:
+0000000000004640 <tripleGateAction>:
 tripleGateAction():
 	push   %r15
 	lea    0x47b(%rip),%rax        
 	push   %r14
 	movq   %rax,%xmm1
 	mov    %rdi,%r14
 	mov    %rcx,%rdi
@@ -2312,24 +2316,24 @@
 	mov    %rsi,0x8(%rsp)
 	lea    0x44b(%rip),%rsi        
 	movq   %rsi,%xmm0
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x50(%rsp)
 	call   1e60 <getArrayLength(int*)@plt>
 	cmp    $0x3,%eax
-	jne    49fb <tripleGateAction+0x3cb>
+	jne    4a0b <tripleGateAction+0x3cb>
 	mov    (%rbx),%ecx
 	mov    0x4(%rbx),%eax
 	cmp    %eax,%ecx
-	je     49e5 <tripleGateAction+0x3b5>
+	je     49f5 <tripleGateAction+0x3b5>
 	mov    0x8(%rbx),%edx
 	cmp    %edx,%eax
-	je     49e5 <tripleGateAction+0x3b5>
+	je     49f5 <tripleGateAction+0x3b5>
 	cmp    %edx,%ecx
-	je     49e5 <tripleGateAction+0x3b5>
+	je     49f5 <tripleGateAction+0x3b5>
 	mov    %ebp,%edi
 	call   1f90 <cudaSetDevice@plt>
 	mov    $0x200,%edi
 	call   1e40 <malloc@plt>
 	mov    $0x18,%edi
 	mov    %rax,%r12
 	call   1e40 <malloc@plt>
@@ -2358,29 +2362,29 @@
 	mov    $0x1,%ecx
 	call   1df0 <cudaMemcpy@plt>
 	mov    %r14,%rdi
 	call   1bc0 <hash(char const*)@plt>
 	mov    (%rbx),%esi
 	mov    $0x4,%edx
 	mov    %rbx,%rdi
-	mov    0x207857(%rip),%rcx        
+	mov    0x207847(%rip),%rcx        
 	mov    %eax,0x1c(%rsp)
 	mov    %esi,0x10(%rsp)
 	mov    0x4(%rbx),%esi
 	mov    %esi,0x18(%rsp)
 	mov    0x8(%rbx),%esi
 	mov    %esi,0x14(%rsp)
 	mov    $0x3,%esi
 	call   1f80 <qsort@plt>
 	lea    0x50(%rsp),%rdi
 	mov    $0x2,%edx
 	mov    %r14,%rsi
 	call   1cf0 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     4a11 <tripleGateAction+0x3e1>
+	je     4a21 <tripleGateAction+0x3e1>
 	mov    (%rbx),%eax
 	mov    $0x1,%r8d
 	mov    %r13,%rsi
 	mov    0x30(%rsp),%rdi
 	mov    %r8d,%edx
 	mov    %eax,%ecx
 	shl    %cl,%edx
@@ -2412,32 +2416,32 @@
 	mov    $0x18,%edx
 	mov    %rbp,%rsi
 	add    $0x1,%eax
 	mov    %eax,0x44(%rsp)
 	call   1df0 <cudaMemcpy@plt>
 	mov    0x1c(%rsp),%eax
 	cmp    $0x537,%eax
-	je     4928 <tripleGateAction+0x2f8>
+	je     4938 <tripleGateAction+0x2f8>
 	cmp    $0x3229,%eax
-	je     48c0 <tripleGateAction+0x290>
+	je     48d0 <tripleGateAction+0x290>
 	mov    0x20(%rsp),%rdi
 	mov    $0x1,%ecx
 	mov    $0x200,%edx
 	mov    %r12,%rsi
 	call   1df0 <cudaMemcpy@plt>
 	mov    %ebx,0x38(%rsp)
 	mov    0x40(%rsp),%ecx
 	xor    %r9d,%r9d
 	mov    0x38(%rsp),%rdx
 	mov    0x44(%rsp),%rdi
 	xor    %r8d,%r8d
 	mov    0x4c(%rsp),%esi
 	call   1f20 <__cudaPushCallConfiguration@plt>
 	test   %eax,%eax
-	je     4988 <tripleGateAction+0x358>
+	je     4998 <tripleGateAction+0x358>
 	call   1f00 <cudaDeviceSynchronize@plt>
 	mov    0x28(%rsp),%rsi
 	mov    0x8(%rsp),%rdi
 	mov    %r15,%rdx
 	mov    $0x2,%ecx
 	call   1df0 <cudaMemcpy@plt>
 	mov    0x20(%rsp),%rdi
@@ -2459,89 +2463,89 @@
 	jmp    1de0 <free@plt>
 	xchg   %ax,%ax
 	mov    0x18(%rsp),%ecx
 	mov    0x14(%rsp),%eax
 	cmp    %eax,%ecx
 	cmovle %ecx,%eax
 	cmp    0x10(%rsp),%eax
-	jg     49d8 <tripleGateAction+0x3a8>
+	jg     49e8 <tripleGateAction+0x3a8>
 	mov    0x14(%rsp),%eax
 	cmp    %eax,%ecx
 	cmovge %ecx,%eax
 	cmp    0x10(%rsp),%eax
-	jl     49b8 <tripleGateAction+0x388>
+	jl     49c8 <tripleGateAction+0x388>
 	mov    0x10(%rsp),%eax
 	mov    0x14(%rsp),%edi
 	cmp    %edi,%eax
-	jge    48fa <tripleGateAction+0x2ca>
+	jge    490a <tripleGateAction+0x2ca>
 	cmp    %ecx,%eax
-	jg     4916 <tripleGateAction+0x2e6>
+	jg     4926 <tripleGateAction+0x2e6>
 	mov    0x10(%rsp),%eax
 	mov    0x18(%rsp),%esi
 	cmp    %esi,%eax
-	jge    4826 <tripleGateAction+0x1f6>
+	jge    4836 <tripleGateAction+0x1f6>
 	mov    0x14(%rsp),%edi
 	cmp    %edi,%eax
-	jle    4826 <tripleGateAction+0x1f6>
+	jle    4836 <tripleGateAction+0x1f6>
 	mov    %r12,%rdi
 	call   1c50 <fred_gate_control_mid(float2*)@plt>
-	jmp    4826 <tripleGateAction+0x1f6>
+	jmp    4836 <tripleGateAction+0x1f6>
 	nopl   0x0(%rax,%rax,1)
 	mov    0x10(%rsp),%esi
 	mov    0x18(%rsp),%eax
 	cmp    %eax,%esi
 	cmovge %esi,%eax
 	cmp    0x14(%rsp),%eax
-	jl     49c8 <tripleGateAction+0x398>
+	jl     49d8 <tripleGateAction+0x398>
 	mov    0x18(%rsp),%eax
 	cmp    %eax,%esi
 	cmovle %esi,%eax
 	cmp    0x14(%rsp),%eax
-	jg     49a8 <tripleGateAction+0x378>
+	jg     49b8 <tripleGateAction+0x378>
 	mov    0x14(%rsp),%eax
 	cmp    %eax,0x10(%rsp)
-	jge    495e <tripleGateAction+0x32e>
+	jge    496e <tripleGateAction+0x32e>
 	cmp    %eax,0x18(%rsp)
-	jg     4976 <tripleGateAction+0x346>
+	jg     4986 <tripleGateAction+0x346>
 	mov    0x14(%rsp),%eax
 	cmp    %eax,0x18(%rsp)
-	jge    4826 <tripleGateAction+0x1f6>
+	jge    4836 <tripleGateAction+0x1f6>
 	cmp    %eax,0x10(%rsp)
-	jle    4826 <tripleGateAction+0x1f6>
+	jle    4836 <tripleGateAction+0x1f6>
 	mov    %r12,%rdi
 	call   1cd0 <toff_gate_target_mid(float2*)@plt>
-	jmp    4826 <tripleGateAction+0x1f6>
+	jmp    4836 <tripleGateAction+0x1f6>
 	nopl   0x0(%rax,%rax,1)
 	mov    0x30(%rsp),%rcx
 	mov    0x20(%rsp),%rsi
 	mov    %r13,%rdx
 	mov    0x28(%rsp),%rdi
 	call   1e30 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)@plt>
-	jmp    4866 <tripleGateAction+0x236>
+	jmp    4876 <tripleGateAction+0x236>
 	nopl   0x0(%rax)
 	mov    %r12,%rdi
 	call   1c10 <toff_gate_target_small(float2*)@plt>
-	jmp    4826 <tripleGateAction+0x1f6>
+	jmp    4836 <tripleGateAction+0x1f6>
 	nopl   (%rax)
 	mov    %r12,%rdi
 	call   1ca0 <fred_gate_control_big(float2*)@plt>
-	jmp    4826 <tripleGateAction+0x1f6>
+	jmp    4836 <tripleGateAction+0x1f6>
 	nopl   (%rax)
 	mov    %r12,%rdi
 	call   1eb0 <toff_gate_target_big(float2*)@plt>
-	jmp    4826 <tripleGateAction+0x1f6>
+	jmp    4836 <tripleGateAction+0x1f6>
 	nopl   (%rax)
 	mov    %r12,%rdi
 	call   1c30 <fred_gate_control_small(float2*)@plt>
-	jmp    4826 <tripleGateAction+0x1f6>
-	lea    0x16c(%rip),%rdi        
+	jmp    4836 <tripleGateAction+0x1f6>
+	lea    0x17c(%rip),%rdi        
 	call   1ed0 <puts@plt>
 	mov    $0x2,%edi
 	call   1e00 <exit@plt>
-	lea    0x17e(%rip),%rdi        
+	lea    0x18e(%rip),%rdi        
 	call   1ed0 <puts@plt>
 	mov    $0x1,%edi
 	call   1e00 <exit@plt>
 	mov    0x20(%rsp),%rdi
 	call   1ea0 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
 	call   1ea0 <cudaFree@plt>
@@ -2551,13 +2555,13 @@
 	call   1de0 <free@plt>
 	mov    %rbp,%rdi
 	call   1de0 <free@plt>
 	mov    $0x3,%edi
 	call   1e00 <exit@plt>
 	nopl   0x0(%rax)
 
-0000000000004a50 <atexit>:
+0000000000004a60 <atexit>:
 atexit():
 /opt/glibc-2.31/stdlib/atexit.c:46
-	mov    0x2077d1(%rip),%rdx        
+	mov    0x2077c1(%rip),%rdx        
 	xor    %esi,%esi
 	jmp    1d50 <__cxa_atexit@plt>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,13 +1,13 @@
 
 
 
 Disassembly of section .fini:
 
-0000000000004a60 <_fini>:
+0000000000004a70 <_fini>:
 _fini():
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crti.S:84
 	sub    $0x8,%rsp
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crtn.S:44
 	add    $0x8,%rsp
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crtn.S:45
 	ret
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,53 +1,54 @@
 
 Hex dump of section '.rodata':
-  0x00004a70 73007364 67007400 74646700 68007278 s.sdg.t.tdg.h.rx
-  0x00004a80 00727900 727a0064 616d705f 49007064 .ry.rz.damp_I.pd
-  0x00004a90 00616400 69737761 70006370 00637a00 .ad.iswap.cp.cz.
-  0x00004aa0 72787800 72797900 727a7a00 73796300 rxx.ryy.rzz.syc.
-  0x00004ab0 63637800 63737761 7000706f 735f6172 ccx.cswap.pos_ar
-  0x00004ac0 7261795f 73697a65 203d2025 640a0000 ray_size = %d...
-  0x00004ad0 dbf3ffff 28f2ffff 28f2ffff 28f2ffff ....(...(...(...
-  0x00004ae0 28f2ffff 28f2ffff 28f2ffff 28f2ffff (...(...(...(...
-  0x00004af0 28f2ffff 28f2ffff 28f2ffff e8f3ffff (...(...(.......
-  0x00004b00 f5f3ffff 28f2ffff 28f2ffff 28f2ffff ....(...(...(...
-  0x00004b10 02f4ffff 0ff4ffff cef3ffff 00000000 ................
-  0x00004b20 4d757374 20626520 68617665 2074776f Must be have two
-  0x00004b30 20616374 696f6e20 706f7369 74696f6e  action position
-  0x00004b40 212c2067 6174654e 616d653a 2025730a !, gateName: %s.
-  0x00004b50 00000000 00000000 61637469 6f6e2070 ........action p
-  0x00004b60 6f736974 696f6e20 6d757374 20626520 osition must be 
-  0x00004b70 64696666 6572656e 74210000 00000000 different!......
-  0x00004b80 4d757374 20626520 68617665 20746872 Must be have thr
-  0x00004b90 65652061 6374696f 6e20706f 73697469 ee action positi
-  0x00004ba0 6f6e2100 00000000 5f5a3138 61637469 on!....._Z18acti
-  0x00004bb0 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
-  0x00004bc0 666c6f61 74325330 5f6d506d 00000000 float2S0_mPm....
-  0x00004bd0 5f5a3139 61637469 6f6e4f6e 446f7562 _Z19actionOnDoub
-  0x00004be0 6c655175 62697450 36666c6f 61743253 leQubitP6float2S
-  0x00004bf0 305f6d50 6d000000 5f5a3139 61637469 0_mPm..._Z19acti
-  0x00004c00 6f6e4f6e 53696e67 6c655175 62697450 onOnSingleQubitP
-  0x00004c10 36666c6f 61743253 305f6d50 6d000000 6float2S0_mPm...
-  0x00004c20 00000000 00000000 0000803f 00000000 ...........?....
-  0x00004c30 0000803f 00000000 00000000 00000000 ...?............
-  0x00004c40 00000000 00000000 00000000 000080bf ................
-  0x00004c50 00000000 0000803f 00000000 00000000 .......?........
-  0x00004c60 00000000 00000000 000080bf 00000000 ................
-  0x00004c70 00000000 00000000 00000000 0000803f ...............?
-  0x00004c80 00000000 00000000 f304353f f304353f ..........5?..5?
-  0x00004c90 00000000 00000000 f304353f f30435bf ..........5?..5.
-  0x00004ca0 f304353f 00000000 f304353f 00000000 ..5?......5?....
-  0x00004cb0 f304353f 00000000 f30435bf 00000000 ..5?......5.....
-  0x00004cc0 00000080 00000000 00000000 00000000 ................
-  0x00004cd0 00000000 000080bf 00000000 00000000 ................
-  0x00004ce0 00000000 00000000 d7b35d3f 000000bf ..........]?....
-  0x00004cf0 00000000 01000000 02000000 03000000 ................
-  0x00004d00 04000000 04000000 04000000 04000000 ................
-  0x00004d10 2d000000 2d000000 2d000000 2d000000 -...-...-...-...
-  0x00004d20 3f000000 3f000000 3f000000 3f000000 ?...?...?...?...
-  0x00004d30 398ee338 398ee338 398ee338 398ee338 9..89..89..89..8
-  0x00004d40 0000803f 0000803f 0000803f 0000803f ...?...?...?...?
-  0x00004d50 1b000000 1b000000 1b000000 1b000000 ................
-  0x00004d60 36000000 36000000 36000000 36000000 6...6...6...6...
-  0x00004d70 0000003f 0000803f 00000030 00000000 ...?...?...0....
-  0x00004d80 8dedb5a0 f7c6b03e                   .......>
+  0x00004a80 73007364 67007400 74646700 68007278 s.sdg.t.tdg.h.rx
+  0x00004a90 00727900 727a0064 616d705f 49007064 .ry.rz.damp_I.pd
+  0x00004aa0 00616400 69737761 70006370 00637a00 .ad.iswap.cp.cz.
+  0x00004ab0 72787800 72797900 727a7a00 73796300 rxx.ryy.rzz.syc.
+  0x00004ac0 63637800 63737761 70006761 74654e61 ccx.cswap.gateNa
+  0x00004ad0 6d653a20 25730a00 706f735f 61727261 me: %s..pos_arra
+  0x00004ae0 795f7369 7a65203d 2025640a 00000000 y_size = %d.....
+  0x00004af0 cbf3ffff 18f2ffff 18f2ffff 18f2ffff ................
+  0x00004b00 18f2ffff 18f2ffff 18f2ffff 18f2ffff ................
+  0x00004b10 18f2ffff 18f2ffff 18f2ffff d8f3ffff ................
+  0x00004b20 e5f3ffff 18f2ffff 18f2ffff 18f2ffff ................
+  0x00004b30 f2f3ffff fff3ffff bef3ffff 00000000 ................
+  0x00004b40 4d757374 20626520 68617665 2074776f Must be have two
+  0x00004b50 20616374 696f6e20 706f7369 74696f6e  action position
+  0x00004b60 212c2067 6174654e 616d653a 2025730a !, gateName: %s.
+  0x00004b70 00000000 00000000 61637469 6f6e2070 ........action p
+  0x00004b80 6f736974 696f6e20 6d757374 20626520 osition must be 
+  0x00004b90 64696666 6572656e 74210000 00000000 different!......
+  0x00004ba0 4d757374 20626520 68617665 20746872 Must be have thr
+  0x00004bb0 65652061 6374696f 6e20706f 73697469 ee action positi
+  0x00004bc0 6f6e2100 00000000 5f5a3138 61637469 on!....._Z18acti
+  0x00004bd0 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
+  0x00004be0 666c6f61 74325330 5f6d506d 00000000 float2S0_mPm....
+  0x00004bf0 5f5a3139 61637469 6f6e4f6e 446f7562 _Z19actionOnDoub
+  0x00004c00 6c655175 62697450 36666c6f 61743253 leQubitP6float2S
+  0x00004c10 305f6d50 6d000000 5f5a3139 61637469 0_mPm..._Z19acti
+  0x00004c20 6f6e4f6e 53696e67 6c655175 62697450 onOnSingleQubitP
+  0x00004c30 36666c6f 61743253 305f6d50 6d000000 6float2S0_mPm...
+  0x00004c40 00000000 00000000 0000803f 00000000 ...........?....
+  0x00004c50 0000803f 00000000 00000000 00000000 ...?............
+  0x00004c60 00000000 00000000 00000000 000080bf ................
+  0x00004c70 00000000 0000803f 00000000 00000000 .......?........
+  0x00004c80 00000000 00000000 000080bf 00000000 ................
+  0x00004c90 00000000 00000000 00000000 0000803f ...............?
+  0x00004ca0 00000000 00000000 f304353f f304353f ..........5?..5?
+  0x00004cb0 00000000 00000000 f304353f f30435bf ..........5?..5.
+  0x00004cc0 f304353f 00000000 f304353f 00000000 ..5?......5?....
+  0x00004cd0 f304353f 00000000 f30435bf 00000000 ..5?......5.....
+  0x00004ce0 00000080 00000000 00000000 00000000 ................
+  0x00004cf0 00000000 000080bf 00000000 00000000 ................
+  0x00004d00 00000000 00000000 d7b35d3f 000000bf ..........]?....
+  0x00004d10 00000000 01000000 02000000 03000000 ................
+  0x00004d20 04000000 04000000 04000000 04000000 ................
+  0x00004d30 2d000000 2d000000 2d000000 2d000000 -...-...-...-...
+  0x00004d40 3f000000 3f000000 3f000000 3f000000 ?...?...?...?...
+  0x00004d50 398ee338 398ee338 398ee338 398ee338 9..89..89..89..8
+  0x00004d60 0000803f 0000803f 0000803f 0000803f ...?...?...?...?
+  0x00004d70 1b000000 1b000000 1b000000 1b000000 ................
+  0x00004d80 36000000 36000000 36000000 36000000 6...6...6...6...
+  0x00004d90 0000003f 0000803f 00000030 00000000 ...?...?...0....
+  0x00004da0 8dedb5a0 f7c6b03e                   .......>
```

#### readelf --wide --decompress --hex-dump=.nv_fatbin {}

```diff
@@ -1,274 +1,272 @@
 
 Hex dump of section '.nv_fatbin':
-  0x00004d88 50ed55ba 01001000 b0030000 00000000 P.U.............
-  0x00004d98 02000101 48000000 68030000 00000000 ....H...h.......
-  0x00004da8 00000000 00000000 07000100 50000000 ............P...
-  0x00004db8 00000000 00000000 11000000 00000000 ................
-  0x00004dc8 00000000 00000000 00000000 00000000 ................
-  0x00004dd8 00000000 00000000 7f454c46 02010133 .........ELF...3
-  0x00004de8 07000000 00000000 0200be00 7c000000 ............|...
-  0x00004df8 00000000 00000000 f8020000 00000000 ................
-  0x00004e08 78010000 00000000 50055000 40003800 x.......P.P.@.8.
-  0x00004e18 02004000 06000100 002e7368 73747274 ..@.......shstrt
-  0x00004e28 6162002e 73747274 6162002e 73796d74 ab..strtab..symt
-  0x00004e38 6162002e 73796d74 61625f73 686e6478 ab..symtab_shndx
-  0x00004e48 002e6e76 2e696e66 6f002e6e 762e6361 ..nv.info..nv.ca
-  0x00004e58 6c6c6772 61706800 2e6e762e 70726f74 llgraph..nv.prot
-  0x00004e68 6f747970 65002e6e 762e7265 6c2e6163 otype..nv.rel.ac
-  0x00004e78 74696f6e 00002e73 68737472 74616200 tion...shstrtab.
-  0x00004e88 2e737472 74616200 2e73796d 74616200 .strtab..symtab.
-  0x00004e98 2e73796d 7461625f 73686e64 78002e6e .symtab_shndx..n
-  0x00004ea8 762e696e 666f002e 6e762e63 616c6c67 v.info..nv.callg
-  0x00004eb8 72617068 002e6e76 2e70726f 746f7479 raph..nv.prototy
-  0x00004ec8 7065002e 6e762e72 656c2e61 6374696f pe..nv.rel.actio
-  0x00004ed8 6e000000 00000000 00000000 00000000 n...............
-  0x00004ee8 00000000 00000000 00000000 00000000 ................
-  0x00004ef8 32000000 03000400 00000000 00000000 2...............
-  0x00004f08 00000000 00000000 4e000000 03000500 ........N.......
-  0x00004f18 00000000 00000000 00000000 00000000 ................
-  0x00004f28 00000000 ffffffff 00000000 feffffff ................
-  0x00004f38 00000000 fdffffff 00000000 fcffffff ................
-  0x00004f48 73000000 00000000 00000011 25000536 s...........%..6
-  0x00004f58 00000000 00000000 00000000 00000000 ................
-  0x00004f68 00000000 00000000 00000000 00000000 ................
+  0x00004da8 50ed55ba 01001000 b0030000 00000000 P.U.............
+  0x00004db8 02000101 48000000 68030000 00000000 ....H...h.......
+  0x00004dc8 00000000 00000000 07000100 50000000 ............P...
+  0x00004dd8 00000000 00000000 11000000 00000000 ................
+  0x00004de8 00000000 00000000 00000000 00000000 ................
+  0x00004df8 00000000 00000000 7f454c46 02010133 .........ELF...3
+  0x00004e08 07000000 00000000 0200be00 7c000000 ............|...
+  0x00004e18 00000000 00000000 f8020000 00000000 ................
+  0x00004e28 78010000 00000000 50055000 40003800 x.......P.P.@.8.
+  0x00004e38 02004000 06000100 002e7368 73747274 ..@.......shstrt
+  0x00004e48 6162002e 73747274 6162002e 73796d74 ab..strtab..symt
+  0x00004e58 6162002e 73796d74 61625f73 686e6478 ab..symtab_shndx
+  0x00004e68 002e6e76 2e696e66 6f002e6e 762e6361 ..nv.info..nv.ca
+  0x00004e78 6c6c6772 61706800 2e6e762e 70726f74 llgraph..nv.prot
+  0x00004e88 6f747970 65002e6e 762e7265 6c2e6163 otype..nv.rel.ac
+  0x00004e98 74696f6e 00002e73 68737472 74616200 tion...shstrtab.
+  0x00004ea8 2e737472 74616200 2e73796d 74616200 .strtab..symtab.
+  0x00004eb8 2e73796d 7461625f 73686e64 78002e6e .symtab_shndx..n
+  0x00004ec8 762e696e 666f002e 6e762e63 616c6c67 v.info..nv.callg
+  0x00004ed8 72617068 002e6e76 2e70726f 746f7479 raph..nv.prototy
+  0x00004ee8 7065002e 6e762e72 656c2e61 6374696f pe..nv.rel.actio
+  0x00004ef8 6e000000 00000000 00000000 00000000 n...............
+  0x00004f08 00000000 00000000 00000000 00000000 ................
+  0x00004f18 32000000 03000400 00000000 00000000 2...............
+  0x00004f28 00000000 00000000 4e000000 03000500 ........N.......
+  0x00004f38 00000000 00000000 00000000 00000000 ................
+  0x00004f48 00000000 ffffffff 00000000 feffffff ................
+  0x00004f58 00000000 fdffffff 00000000 fcffffff ................
+  0x00004f68 73000000 00000000 00000011 25000536 s...........%..6
   0x00004f78 00000000 00000000 00000000 00000000 ................
   0x00004f88 00000000 00000000 00000000 00000000 ................
-  0x00004f98 01000000 03000000 00000000 00000000 ................
-  0x00004fa8 00000000 00000000 40000000 00000000 ........@.......
-  0x00004fb8 5d000000 00000000 00000000 00000000 ]...............
-  0x00004fc8 01000000 00000000 00000000 00000000 ................
-  0x00004fd8 0b000000 03000000 00000000 00000000 ................
-  0x00004fe8 00000000 00000000 9d000000 00000000 ................
-  0x00004ff8 5d000000 00000000 00000000 00000000 ]...............
-  0x00005008 01000000 00000000 00000000 00000000 ................
-  0x00005018 13000000 02000000 00000000 00000000 ................
-  0x00005028 00000000 00000000 00010000 00000000 ................
-  0x00005038 48000000 00000000 02000000 03000000 H...............
-  0x00005048 08000000 00000000 18000000 00000000 ................
-  0x00005058 32000000 01000070 00000000 00000000 2......p........
-  0x00005068 00000000 00000000 48010000 00000000 ........H.......
-  0x00005078 20000000 00000000 03000000 00000000  ...............
-  0x00005088 04000000 00000000 08000000 00000000 ................
-  0x00005098 4e000000 0b000070 00000000 00000000 N......p........
-  0x000050a8 00000000 00000000 68010000 00000000 ........h.......
-  0x000050b8 10000000 00000000 00000000 00000000 ................
-  0x000050c8 08000000 00000000 08000000 00000000 ................
-  0x000050d8 06000000 05000000 f8020000 00000000 ................
-  0x000050e8 00000000 00000000 00000000 00000000 ................
-  0x000050f8 70000000 00000000 70000000 00000000 p.......p.......
-  0x00005108 08000000 00000000 01000000 05000000 ................
-  0x00005118 f8020000 00000000 00000000 00000000 ................
-  0x00005128 00000000 00000000 70000000 00000000 ........p.......
-  0x00005138 70000000 00000000 08000000 00000000 p...............
-  0x00005148 50ed55ba 01001000 905c0000 00000000 P.U......\......
-  0x00005158 02000101 48000000 a83c0000 00000000 ....H....<......
-  0x00005168 00000000 00000000 07000100 50000000 ............P...
-  0x00005178 00000000 00000000 11000000 00000000 ................
-  0x00005188 00000000 00000000 00000000 00000000 ................
-  0x00005198 00000000 00000000 7f454c46 02010133 .........ELF...3
-  0x000051a8 07000000 00000000 0200be00 7c000000 ............|...
-  0x000051b8 00000000 00000000 003c0000 00000000 .........<......
-  0x000051c8 80370000 00000000 50055000 40003800 .7......P.P.@.8.
-  0x000051d8 03004000 12000100 002e7368 73747274 ..@.......shstrt
-  0x000051e8 6162002e 73747274 6162002e 73796d74 ab..strtab..symt
-  0x000051f8 6162002e 73796d74 61625f73 686e6478 ab..symtab_shndx
-  0x00005208 002e6e76 2e696e66 6f002e74 6578742e ..nv.info..text.
-  0x00005218 5f5a3138 61637469 6f6e4f6e 54726970 _Z18actionOnTrip
-  0x00005228 6c654761 74655036 666c6f61 74325330 leGateP6float2S0
-  0x00005238 5f6d506d 002e6e76 2e696e66 6f2e5f5a _mPm..nv.info._Z
-  0x00005248 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
-  0x00005258 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
-  0x00005268 506d002e 6e762e73 68617265 642e5f5a Pm..nv.shared._Z
-  0x00005278 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
-  0x00005288 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
-  0x00005298 506d002e 6e762e63 6f6e7374 616e7430 Pm..nv.constant0
-  0x000052a8 2e5f5a31 38616374 696f6e4f 6e547269 ._Z18actionOnTri
-  0x000052b8 706c6547 61746550 36666c6f 61743253 pleGateP6float2S
-  0x000052c8 305f6d50 6d002e72 656c2e6e 762e636f 0_mPm..rel.nv.co
-  0x000052d8 6e737461 6e74302e 5f5a3138 61637469 nstant0._Z18acti
-  0x000052e8 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
-  0x000052f8 666c6f61 74325330 5f6d506d 002e7465 float2S0_mPm..te
-  0x00005308 78742e5f 5a313961 6374696f 6e4f6e44 xt._Z19actionOnD
-  0x00005318 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x00005328 74325330 5f6d506d 002e6e76 2e696e66 t2S0_mPm..nv.inf
-  0x00005338 6f2e5f5a 31396163 74696f6e 4f6e446f o._Z19actionOnDo
-  0x00005348 75626c65 51756269 74503666 6c6f6174 ubleQubitP6float
-  0x00005358 3253305f 6d506d00 2e6e762e 73686172 2S0_mPm..nv.shar
-  0x00005368 65642e5f 5a313961 6374696f 6e4f6e44 ed._Z19actionOnD
-  0x00005378 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x00005388 74325330 5f6d506d 002e6e76 2e636f6e t2S0_mPm..nv.con
-  0x00005398 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
-  0x000053a8 6e4f6e44 6f75626c 65517562 69745036 nOnDoubleQubitP6
-  0x000053b8 666c6f61 74325330 5f6d506d 002e7265 float2S0_mPm..re
-  0x000053c8 6c2e6e76 2e636f6e 7374616e 74302e5f l.nv.constant0._
-  0x000053d8 5a313961 6374696f 6e4f6e44 6f75626c Z19actionOnDoubl
-  0x000053e8 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
-  0x000053f8 5f6d506d 002e7465 78742e5f 5a313961 _mPm..text._Z19a
-  0x00005408 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
-  0x00005418 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
-  0x00005428 002e6e76 2e696e66 6f2e5f5a 31396163 ..nv.info._Z19ac
-  0x00005438 74696f6e 4f6e5369 6e676c65 51756269 tionOnSingleQubi
-  0x00005448 74503666 6c6f6174 3253305f 6d506d00 tP6float2S0_mPm.
-  0x00005458 2e6e762e 73686172 65642e5f 5a313961 .nv.shared._Z19a
-  0x00005468 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
-  0x00005478 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
-  0x00005488 002e6e76 2e636f6e 7374616e 74302e5f ..nv.constant0._
-  0x00005498 5a313961 6374696f 6e4f6e53 696e676c Z19actionOnSingl
-  0x000054a8 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
-  0x000054b8 5f6d506d 002e7265 6c2e6e76 2e636f6e _mPm..rel.nv.con
-  0x000054c8 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
-  0x000054d8 6e4f6e53 696e676c 65517562 69745036 nOnSingleQubitP6
-  0x000054e8 666c6f61 74325330 5f6d506d 002e6465 float2S0_mPm..de
-  0x000054f8 6275675f 6672616d 65002e72 656c2e64 bug_frame..rel.d
-  0x00005508 65627567 5f667261 6d65002e 72656c61 ebug_frame..rela
-  0x00005518 2e646562 75675f66 72616d65 002e6e76 .debug_frame..nv
-  0x00005528 2e63616c 6c677261 7068002e 6e762e70 .callgraph..nv.p
-  0x00005538 726f746f 74797065 002e6e76 2e72656c rototype..nv.rel
-  0x00005548 2e616374 696f6e00 002e7368 73747274 .action...shstrt
-  0x00005558 6162002e 73747274 6162002e 73796d74 ab..strtab..symt
-  0x00005568 6162002e 73796d74 61625f73 686e6478 ab..symtab_shndx
-  0x00005578 002e6e76 2e696e66 6f002e74 6578742e ..nv.info..text.
-  0x00005588 5f5a3138 61637469 6f6e4f6e 54726970 _Z18actionOnTrip
-  0x00005598 6c654761 74655036 666c6f61 74325330 leGateP6float2S0
-  0x000055a8 5f6d506d 002e6e76 2e696e66 6f2e5f5a _mPm..nv.info._Z
-  0x000055b8 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
-  0x000055c8 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
-  0x000055d8 506d002e 6e762e73 68617265 642e5f5a Pm..nv.shared._Z
-  0x000055e8 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
-  0x000055f8 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
-  0x00005608 506d002e 72656c2e 6e762e63 6f6e7374 Pm..rel.nv.const
-  0x00005618 616e7430 2e5f5a31 38616374 696f6e4f ant0._Z18actionO
-  0x00005628 6e547269 706c6547 61746550 36666c6f nTripleGateP6flo
-  0x00005638 61743253 305f6d50 6d002e6e 762e636f at2S0_mPm..nv.co
-  0x00005648 6e737461 6e74302e 5f5a3138 61637469 nstant0._Z18acti
-  0x00005658 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
-  0x00005668 666c6f61 74325330 5f6d506d 002e7465 float2S0_mPm..te
-  0x00005678 78742e5f 5a313961 6374696f 6e4f6e44 xt._Z19actionOnD
-  0x00005688 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x00005698 74325330 5f6d506d 002e6e76 2e696e66 t2S0_mPm..nv.inf
-  0x000056a8 6f2e5f5a 31396163 74696f6e 4f6e446f o._Z19actionOnDo
-  0x000056b8 75626c65 51756269 74503666 6c6f6174 ubleQubitP6float
-  0x000056c8 3253305f 6d506d00 2e6e762e 73686172 2S0_mPm..nv.shar
-  0x000056d8 65642e5f 5a313961 6374696f 6e4f6e44 ed._Z19actionOnD
-  0x000056e8 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x000056f8 74325330 5f6d506d 002e7265 6c2e6e76 t2S0_mPm..rel.nv
-  0x00005708 2e636f6e 7374616e 74302e5f 5a313961 .constant0._Z19a
-  0x00005718 6374696f 6e4f6e44 6f75626c 65517562 ctionOnDoubleQub
-  0x00005728 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
-  0x00005738 002e6e76 2e636f6e 7374616e 74302e5f ..nv.constant0._
-  0x00005748 5a313961 6374696f 6e4f6e44 6f75626c Z19actionOnDoubl
-  0x00005758 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
-  0x00005768 5f6d506d 002e7465 78742e5f 5a313961 _mPm..text._Z19a
-  0x00005778 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
-  0x00005788 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
-  0x00005798 002e6e76 2e696e66 6f2e5f5a 31396163 ..nv.info._Z19ac
-  0x000057a8 74696f6e 4f6e5369 6e676c65 51756269 tionOnSingleQubi
-  0x000057b8 74503666 6c6f6174 3253305f 6d506d00 tP6float2S0_mPm.
-  0x000057c8 2e6e762e 73686172 65642e5f 5a313961 .nv.shared._Z19a
-  0x000057d8 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
-  0x000057e8 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
-  0x000057f8 002e7265 6c2e6e76 2e636f6e 7374616e ..rel.nv.constan
-  0x00005808 74302e5f 5a313961 6374696f 6e4f6e53 t0._Z19actionOnS
-  0x00005818 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
-  0x00005828 74325330 5f6d506d 002e6e76 2e636f6e t2S0_mPm..nv.con
-  0x00005838 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
-  0x00005848 6e4f6e53 696e676c 65517562 69745036 nOnSingleQubitP6
-  0x00005858 666c6f61 74325330 5f6d506d 002e6465 float2S0_mPm..de
-  0x00005868 6275675f 6672616d 65002e72 656c2e64 bug_frame..rel.d
-  0x00005878 65627567 5f667261 6d65002e 72656c61 ebug_frame..rela
-  0x00005888 2e646562 75675f66 72616d65 002e6e76 .debug_frame..nv
-  0x00005898 2e63616c 6c677261 7068002e 6e762e70 .callgraph..nv.p
-  0x000058a8 726f746f 74797065 002e6e76 2e72656c rototype..nv.rel
-  0x000058b8 2e616374 696f6e00 5f5a3138 61637469 .action._Z18acti
-  0x000058c8 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
-  0x000058d8 666c6f61 74325330 5f6d506d 005f5a31 float2S0_mPm._Z1
-  0x000058e8 39616374 696f6e4f 6e446f75 626c6551 9actionOnDoubleQ
-  0x000058f8 75626974 5036666c 6f617432 53305f6d ubitP6float2S0_m
-  0x00005908 506d005f 5a313961 6374696f 6e4f6e53 Pm._Z19actionOnS
-  0x00005918 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
-  0x00005928 74325330 5f6d506d 00000000 00000000 t2S0_mPm........
-  0x00005938 00000000 00000000 00000000 00000000 ................
-  0x00005948 00000000 00000000 32000000 03000f00 ........2.......
+  0x00004f98 00000000 00000000 00000000 00000000 ................
+  0x00004fa8 00000000 00000000 00000000 00000000 ................
+  0x00004fb8 01000000 03000000 00000000 00000000 ................
+  0x00004fc8 00000000 00000000 40000000 00000000 ........@.......
+  0x00004fd8 5d000000 00000000 00000000 00000000 ]...............
+  0x00004fe8 01000000 00000000 00000000 00000000 ................
+  0x00004ff8 0b000000 03000000 00000000 00000000 ................
+  0x00005008 00000000 00000000 9d000000 00000000 ................
+  0x00005018 5d000000 00000000 00000000 00000000 ]...............
+  0x00005028 01000000 00000000 00000000 00000000 ................
+  0x00005038 13000000 02000000 00000000 00000000 ................
+  0x00005048 00000000 00000000 00010000 00000000 ................
+  0x00005058 48000000 00000000 02000000 03000000 H...............
+  0x00005068 08000000 00000000 18000000 00000000 ................
+  0x00005078 32000000 01000070 00000000 00000000 2......p........
+  0x00005088 00000000 00000000 48010000 00000000 ........H.......
+  0x00005098 20000000 00000000 03000000 00000000  ...............
+  0x000050a8 04000000 00000000 08000000 00000000 ................
+  0x000050b8 4e000000 0b000070 00000000 00000000 N......p........
+  0x000050c8 00000000 00000000 68010000 00000000 ........h.......
+  0x000050d8 10000000 00000000 00000000 00000000 ................
+  0x000050e8 08000000 00000000 08000000 00000000 ................
+  0x000050f8 06000000 05000000 f8020000 00000000 ................
+  0x00005108 00000000 00000000 00000000 00000000 ................
+  0x00005118 70000000 00000000 70000000 00000000 p.......p.......
+  0x00005128 08000000 00000000 01000000 05000000 ................
+  0x00005138 f8020000 00000000 00000000 00000000 ................
+  0x00005148 00000000 00000000 70000000 00000000 ........p.......
+  0x00005158 70000000 00000000 08000000 00000000 p...............
+  0x00005168 50ed55ba 01001000 905c0000 00000000 P.U......\......
+  0x00005178 02000101 48000000 a83c0000 00000000 ....H....<......
+  0x00005188 00000000 00000000 07000100 50000000 ............P...
+  0x00005198 00000000 00000000 11000000 00000000 ................
+  0x000051a8 00000000 00000000 00000000 00000000 ................
+  0x000051b8 00000000 00000000 7f454c46 02010133 .........ELF...3
+  0x000051c8 07000000 00000000 0200be00 7c000000 ............|...
+  0x000051d8 00000000 00000000 003c0000 00000000 .........<......
+  0x000051e8 80370000 00000000 50055000 40003800 .7......P.P.@.8.
+  0x000051f8 03004000 12000100 002e7368 73747274 ..@.......shstrt
+  0x00005208 6162002e 73747274 6162002e 73796d74 ab..strtab..symt
+  0x00005218 6162002e 73796d74 61625f73 686e6478 ab..symtab_shndx
+  0x00005228 002e6e76 2e696e66 6f002e74 6578742e ..nv.info..text.
+  0x00005238 5f5a3138 61637469 6f6e4f6e 54726970 _Z18actionOnTrip
+  0x00005248 6c654761 74655036 666c6f61 74325330 leGateP6float2S0
+  0x00005258 5f6d506d 002e6e76 2e696e66 6f2e5f5a _mPm..nv.info._Z
+  0x00005268 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
+  0x00005278 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
+  0x00005288 506d002e 6e762e73 68617265 642e5f5a Pm..nv.shared._Z
+  0x00005298 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
+  0x000052a8 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
+  0x000052b8 506d002e 6e762e63 6f6e7374 616e7430 Pm..nv.constant0
+  0x000052c8 2e5f5a31 38616374 696f6e4f 6e547269 ._Z18actionOnTri
+  0x000052d8 706c6547 61746550 36666c6f 61743253 pleGateP6float2S
+  0x000052e8 305f6d50 6d002e72 656c2e6e 762e636f 0_mPm..rel.nv.co
+  0x000052f8 6e737461 6e74302e 5f5a3138 61637469 nstant0._Z18acti
+  0x00005308 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
+  0x00005318 666c6f61 74325330 5f6d506d 002e7465 float2S0_mPm..te
+  0x00005328 78742e5f 5a313961 6374696f 6e4f6e44 xt._Z19actionOnD
+  0x00005338 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
+  0x00005348 74325330 5f6d506d 002e6e76 2e696e66 t2S0_mPm..nv.inf
+  0x00005358 6f2e5f5a 31396163 74696f6e 4f6e446f o._Z19actionOnDo
+  0x00005368 75626c65 51756269 74503666 6c6f6174 ubleQubitP6float
+  0x00005378 3253305f 6d506d00 2e6e762e 73686172 2S0_mPm..nv.shar
+  0x00005388 65642e5f 5a313961 6374696f 6e4f6e44 ed._Z19actionOnD
+  0x00005398 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
+  0x000053a8 74325330 5f6d506d 002e6e76 2e636f6e t2S0_mPm..nv.con
+  0x000053b8 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
+  0x000053c8 6e4f6e44 6f75626c 65517562 69745036 nOnDoubleQubitP6
+  0x000053d8 666c6f61 74325330 5f6d506d 002e7265 float2S0_mPm..re
+  0x000053e8 6c2e6e76 2e636f6e 7374616e 74302e5f l.nv.constant0._
+  0x000053f8 5a313961 6374696f 6e4f6e44 6f75626c Z19actionOnDoubl
+  0x00005408 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
+  0x00005418 5f6d506d 002e7465 78742e5f 5a313961 _mPm..text._Z19a
+  0x00005428 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
+  0x00005438 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
+  0x00005448 002e6e76 2e696e66 6f2e5f5a 31396163 ..nv.info._Z19ac
+  0x00005458 74696f6e 4f6e5369 6e676c65 51756269 tionOnSingleQubi
+  0x00005468 74503666 6c6f6174 3253305f 6d506d00 tP6float2S0_mPm.
+  0x00005478 2e6e762e 73686172 65642e5f 5a313961 .nv.shared._Z19a
+  0x00005488 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
+  0x00005498 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
+  0x000054a8 002e6e76 2e636f6e 7374616e 74302e5f ..nv.constant0._
+  0x000054b8 5a313961 6374696f 6e4f6e53 696e676c Z19actionOnSingl
+  0x000054c8 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
+  0x000054d8 5f6d506d 002e7265 6c2e6e76 2e636f6e _mPm..rel.nv.con
+  0x000054e8 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
+  0x000054f8 6e4f6e53 696e676c 65517562 69745036 nOnSingleQubitP6
+  0x00005508 666c6f61 74325330 5f6d506d 002e6465 float2S0_mPm..de
+  0x00005518 6275675f 6672616d 65002e72 656c2e64 bug_frame..rel.d
+  0x00005528 65627567 5f667261 6d65002e 72656c61 ebug_frame..rela
+  0x00005538 2e646562 75675f66 72616d65 002e6e76 .debug_frame..nv
+  0x00005548 2e63616c 6c677261 7068002e 6e762e70 .callgraph..nv.p
+  0x00005558 726f746f 74797065 002e6e76 2e72656c rototype..nv.rel
+  0x00005568 2e616374 696f6e00 002e7368 73747274 .action...shstrt
+  0x00005578 6162002e 73747274 6162002e 73796d74 ab..strtab..symt
+  0x00005588 6162002e 73796d74 61625f73 686e6478 ab..symtab_shndx
+  0x00005598 002e6e76 2e696e66 6f002e74 6578742e ..nv.info..text.
+  0x000055a8 5f5a3138 61637469 6f6e4f6e 54726970 _Z18actionOnTrip
+  0x000055b8 6c654761 74655036 666c6f61 74325330 leGateP6float2S0
+  0x000055c8 5f6d506d 002e6e76 2e696e66 6f2e5f5a _mPm..nv.info._Z
+  0x000055d8 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
+  0x000055e8 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
+  0x000055f8 506d002e 6e762e73 68617265 642e5f5a Pm..nv.shared._Z
+  0x00005608 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
+  0x00005618 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
+  0x00005628 506d002e 72656c2e 6e762e63 6f6e7374 Pm..rel.nv.const
+  0x00005638 616e7430 2e5f5a31 38616374 696f6e4f ant0._Z18actionO
+  0x00005648 6e547269 706c6547 61746550 36666c6f nTripleGateP6flo
+  0x00005658 61743253 305f6d50 6d002e6e 762e636f at2S0_mPm..nv.co
+  0x00005668 6e737461 6e74302e 5f5a3138 61637469 nstant0._Z18acti
+  0x00005678 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
+  0x00005688 666c6f61 74325330 5f6d506d 002e7465 float2S0_mPm..te
+  0x00005698 78742e5f 5a313961 6374696f 6e4f6e44 xt._Z19actionOnD
+  0x000056a8 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
+  0x000056b8 74325330 5f6d506d 002e6e76 2e696e66 t2S0_mPm..nv.inf
+  0x000056c8 6f2e5f5a 31396163 74696f6e 4f6e446f o._Z19actionOnDo
+  0x000056d8 75626c65 51756269 74503666 6c6f6174 ubleQubitP6float
+  0x000056e8 3253305f 6d506d00 2e6e762e 73686172 2S0_mPm..nv.shar
+  0x000056f8 65642e5f 5a313961 6374696f 6e4f6e44 ed._Z19actionOnD
+  0x00005708 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
+  0x00005718 74325330 5f6d506d 002e7265 6c2e6e76 t2S0_mPm..rel.nv
+  0x00005728 2e636f6e 7374616e 74302e5f 5a313961 .constant0._Z19a
+  0x00005738 6374696f 6e4f6e44 6f75626c 65517562 ctionOnDoubleQub
+  0x00005748 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
+  0x00005758 002e6e76 2e636f6e 7374616e 74302e5f ..nv.constant0._
+  0x00005768 5a313961 6374696f 6e4f6e44 6f75626c Z19actionOnDoubl
+  0x00005778 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
+  0x00005788 5f6d506d 002e7465 78742e5f 5a313961 _mPm..text._Z19a
+  0x00005798 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
+  0x000057a8 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
+  0x000057b8 002e6e76 2e696e66 6f2e5f5a 31396163 ..nv.info._Z19ac
+  0x000057c8 74696f6e 4f6e5369 6e676c65 51756269 tionOnSingleQubi
+  0x000057d8 74503666 6c6f6174 3253305f 6d506d00 tP6float2S0_mPm.
+  0x000057e8 2e6e762e 73686172 65642e5f 5a313961 .nv.shared._Z19a
+  0x000057f8 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
+  0x00005808 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
+  0x00005818 002e7265 6c2e6e76 2e636f6e 7374616e ..rel.nv.constan
+  0x00005828 74302e5f 5a313961 6374696f 6e4f6e53 t0._Z19actionOnS
+  0x00005838 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
+  0x00005848 74325330 5f6d506d 002e6e76 2e636f6e t2S0_mPm..nv.con
+  0x00005858 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
+  0x00005868 6e4f6e53 696e676c 65517562 69745036 nOnSingleQubitP6
+  0x00005878 666c6f61 74325330 5f6d506d 002e6465 float2S0_mPm..de
+  0x00005888 6275675f 6672616d 65002e72 656c2e64 bug_frame..rel.d
+  0x00005898 65627567 5f667261 6d65002e 72656c61 ebug_frame..rela
+  0x000058a8 2e646562 75675f66 72616d65 002e6e76 .debug_frame..nv
+  0x000058b8 2e63616c 6c677261 7068002e 6e762e70 .callgraph..nv.p
+  0x000058c8 726f746f 74797065 002e6e76 2e72656c rototype..nv.rel
+  0x000058d8 2e616374 696f6e00 5f5a3138 61637469 .action._Z18acti
+  0x000058e8 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
+  0x000058f8 666c6f61 74325330 5f6d506d 005f5a31 float2S0_mPm._Z1
+  0x00005908 39616374 696f6e4f 6e446f75 626c6551 9actionOnDoubleQ
+  0x00005918 75626974 5036666c 6f617432 53305f6d ubitP6float2S0_m
+  0x00005928 506d005f 5a313961 6374696f 6e4f6e53 Pm._Z19actionOnS
+  0x00005938 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
+  0x00005948 74325330 5f6d506d 00000000 00000000 t2S0_mPm........
   0x00005958 00000000 00000000 00000000 00000000 ................
-  0x00005968 f2000000 03000c00 00000000 00000000 ................
-  0x00005978 00000000 00000000 25010000 03001000 ........%.......
-  0x00005988 00000000 00000000 00000000 00000000 ................
-  0x00005998 e9010000 03000d00 00000000 00000000 ................
-  0x000059a8 00000000 00000000 1d020000 03001100 ................
-  0x000059b8 00000000 00000000 00000000 00000000 ................
-  0x000059c8 e1020000 03000e00 00000000 00000000 ................
-  0x000059d8 00000000 00000000 15030000 03000400 ................
-  0x000059e8 00000000 00000000 00000000 00000000 ................
-  0x000059f8 45030000 03000900 00000000 00000000 E...............
-  0x00005a08 00000000 00000000 61030000 03000a00 ........a.......
-  0x00005a18 00000000 00000000 00000000 00000000 ................
-  0x00005a28 70030000 12100f00 00000000 00000000 p...............
-  0x00005a38 001a0000 00000000 95030000 12101000 ................
-  0x00005a48 00000000 00000000 80080000 00000000 ................
-  0x00005a58 bb030000 12101100 00000000 00000000 ................
-  0x00005a68 00040000 00000000 ffffffff 24000000 ............$...
-  0x00005a78 00000000 ffffffff ffffffff 0300047c ...............|
-  0x00005a88 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
-  0x00005a98 08818080 28000000 ffffffff 34000000 ....(.......4...
-  0x00005aa8 00000000 00000000 00000000 00000000 ................
-  0x00005ab8 00000000 001a0000 00000000 04040000 ................
-  0x00005ac8 0004e000 00000c81 80802800 046c0500 ..........(..l..
-  0x00005ad8 00000000 00000000 ffffffff 24000000 ............$...
-  0x00005ae8 00000000 ffffffff ffffffff 0300047c ...............|
-  0x00005af8 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
-  0x00005b08 08818080 28000000 ffffffff 34000000 ....(.......4...
-  0x00005b18 00000000 70000000 00000000 00000000 ....p...........
-  0x00005b28 00000000 80080000 00000000 04040000 ................
-  0x00005b38 00046800 00000c81 80802800 04800100 ..h.......(.....
-  0x00005b48 00000000 00000000 ffffffff 24000000 ............$...
-  0x00005b58 00000000 ffffffff ffffffff 0300047c ...............|
-  0x00005b68 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
-  0x00005b78 08818080 28000000 ffffffff 34000000 ....(.......4...
-  0x00005b88 00000000 e0000000 00000000 00000000 ................
-  0x00005b98 00000000 00040000 00000000 04040000 ................
-  0x00005ba8 00044000 00000c81 80802800 04780000 ..@.......(..x..
-  0x00005bb8 00000000 00000000 042f0800 0c000000 ........./......
-  0x00005bc8 18000000 04120800 0c000000 00000000 ................
-  0x00005bd8 04110800 0c000000 00000000 042f0800 ............./..
-  0x00005be8 0b000000 22000000 04120800 0b000000 ...."...........
-  0x00005bf8 00000000 04110800 0b000000 00000000 ................
-  0x00005c08 042f0800 0a000000 34000000 04120800 ./......4.......
-  0x00005c18 0a000000 00000000 04110800 0a000000 ................
-  0x00005c28 00000000 04120800 0a000000 00000000 ................
-  0x00005c38 04120800 0b000000 00000000 04120800 ................
-  0x00005c48 0c000000 00000000 04370400 7c000000 .........7..|...
-  0x00005c58 01350000 040a0800 02000000 60012000 .5..........`. .
-  0x00005c68 03192000 04170c00 00000000 03001800 .. .............
-  0x00005c78 00f02100 04170c00 00000000 02001000 ..!.............
-  0x00005c88 00f02100 04170c00 00000000 01000800 ..!.............
-  0x00005c98 00f02100 04170c00 00000000 00000000 ..!.............
-  0x00005ca8 00f02100 031bff00 041c0800 80030000 ..!.............
-  0x00005cb8 40190000 04370400 7c000000 01350000 @....7..|....5..
-  0x00005cc8 040a0800 04000000 60012000 03192000 ........`. ... .
-  0x00005cd8 04170c00 00000000 03001800 00f02100 ..............!.
-  0x00005ce8 04170c00 00000000 02001000 00f02100 ..............!.
-  0x00005cf8 04170c00 00000000 01000800 00f02100 ..............!.
-  0x00005d08 04170c00 00000000 00000000 00f02100 ..............!.
-  0x00005d18 031bff00 041c0800 a0010000 b0070000 ................
-  0x00005d28 04370400 7c000000 01350000 040a0800 .7..|....5......
-  0x00005d38 06000000 60012000 03192000 04170c00 ....`. ... .....
-  0x00005d48 00000000 03001800 00f02100 04170c00 ..........!.....
-  0x00005d58 00000000 02001000 00f02100 04170c00 ..........!.....
-  0x00005d68 00000000 01000800 00f02100 04170c00 ..........!.....
-  0x00005d78 00000000 00000000 00f02100 031bff00 ..........!.....
-  0x00005d88 041c0800 00010000 f0020000 00000000 ................
-  0x00005d98 ffffffff 00000000 feffffff 00000000 ................
-  0x00005da8 fdffffff 00000000 fcffffff 00000000 ................
-  0x00005db8 73000000 00000000 00000011 25000536 s...........%..6
-  0x00005dc8 24010000 00000000 02000000 0c000000 $...............
-  0x00005dd8 b4000000 00000000 02000000 0b000000 ................
-  0x00005de8 44000000 00000000 02000000 0a000000 D...............
-  0x00005df8 00000000 00000000 00000000 00000000 ................
-  0x00005e08 00000000 00000000 00000000 00000000 ................
+  0x00005968 00000000 00000000 32000000 03000f00 ........2.......
+  0x00005978 00000000 00000000 00000000 00000000 ................
+  0x00005988 f2000000 03000c00 00000000 00000000 ................
+  0x00005998 00000000 00000000 25010000 03001000 ........%.......
+  0x000059a8 00000000 00000000 00000000 00000000 ................
+  0x000059b8 e9010000 03000d00 00000000 00000000 ................
+  0x000059c8 00000000 00000000 1d020000 03001100 ................
+  0x000059d8 00000000 00000000 00000000 00000000 ................
+  0x000059e8 e1020000 03000e00 00000000 00000000 ................
+  0x000059f8 00000000 00000000 15030000 03000400 ................
+  0x00005a08 00000000 00000000 00000000 00000000 ................
+  0x00005a18 45030000 03000900 00000000 00000000 E...............
+  0x00005a28 00000000 00000000 61030000 03000a00 ........a.......
+  0x00005a38 00000000 00000000 00000000 00000000 ................
+  0x00005a48 70030000 12100f00 00000000 00000000 p...............
+  0x00005a58 001a0000 00000000 95030000 12101000 ................
+  0x00005a68 00000000 00000000 80080000 00000000 ................
+  0x00005a78 bb030000 12101100 00000000 00000000 ................
+  0x00005a88 00040000 00000000 ffffffff 24000000 ............$...
+  0x00005a98 00000000 ffffffff ffffffff 0300047c ...............|
+  0x00005aa8 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
+  0x00005ab8 08818080 28000000 ffffffff 34000000 ....(.......4...
+  0x00005ac8 00000000 00000000 00000000 00000000 ................
+  0x00005ad8 00000000 001a0000 00000000 04040000 ................
+  0x00005ae8 0004e000 00000c81 80802800 046c0500 ..........(..l..
+  0x00005af8 00000000 00000000 ffffffff 24000000 ............$...
+  0x00005b08 00000000 ffffffff ffffffff 0300047c ...............|
+  0x00005b18 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
+  0x00005b28 08818080 28000000 ffffffff 34000000 ....(.......4...
+  0x00005b38 00000000 70000000 00000000 00000000 ....p...........
+  0x00005b48 00000000 80080000 00000000 04040000 ................
+  0x00005b58 00046800 00000c81 80802800 04800100 ..h.......(.....
+  0x00005b68 00000000 00000000 ffffffff 24000000 ............$...
+  0x00005b78 00000000 ffffffff ffffffff 0300047c ...............|
+  0x00005b88 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
+  0x00005b98 08818080 28000000 ffffffff 34000000 ....(.......4...
+  0x00005ba8 00000000 e0000000 00000000 00000000 ................
+  0x00005bb8 00000000 00040000 00000000 04040000 ................
+  0x00005bc8 00044000 00000c81 80802800 04780000 ..@.......(..x..
+  0x00005bd8 00000000 00000000 042f0800 0c000000 ........./......
+  0x00005be8 18000000 04120800 0c000000 00000000 ................
+  0x00005bf8 04110800 0c000000 00000000 042f0800 ............./..
+  0x00005c08 0b000000 22000000 04120800 0b000000 ...."...........
+  0x00005c18 00000000 04110800 0b000000 00000000 ................
+  0x00005c28 042f0800 0a000000 34000000 04120800 ./......4.......
+  0x00005c38 0a000000 00000000 04110800 0a000000 ................
+  0x00005c48 00000000 04120800 0a000000 00000000 ................
+  0x00005c58 04120800 0b000000 00000000 04120800 ................
+  0x00005c68 0c000000 00000000 04370400 7c000000 .........7..|...
+  0x00005c78 01350000 040a0800 02000000 60012000 .5..........`. .
+  0x00005c88 03192000 04170c00 00000000 03001800 .. .............
+  0x00005c98 00f02100 04170c00 00000000 02001000 ..!.............
+  0x00005ca8 00f02100 04170c00 00000000 01000800 ..!.............
+  0x00005cb8 00f02100 04170c00 00000000 00000000 ..!.............
+  0x00005cc8 00f02100 031bff00 041c0800 80030000 ..!.............
+  0x00005cd8 40190000 04370400 7c000000 01350000 @....7..|....5..
+  0x00005ce8 040a0800 04000000 60012000 03192000 ........`. ... .
+  0x00005cf8 04170c00 00000000 03001800 00f02100 ..............!.
+  0x00005d08 04170c00 00000000 02001000 00f02100 ..............!.
+  0x00005d18 04170c00 00000000 01000800 00f02100 ..............!.
+  0x00005d28 04170c00 00000000 00000000 00f02100 ..............!.
+  0x00005d38 031bff00 041c0800 a0010000 b0070000 ................
+  0x00005d48 04370400 7c000000 01350000 040a0800 .7..|....5......
+  0x00005d58 06000000 60012000 03192000 04170c00 ....`. ... .....
+  0x00005d68 00000000 03001800 00f02100 04170c00 ..........!.....
+  0x00005d78 00000000 02001000 00f02100 04170c00 ..........!.....
+  0x00005d88 00000000 01000800 00f02100 04170c00 ..........!.....
+  0x00005d98 00000000 00000000 00f02100 031bff00 ..........!.....
+  0x00005da8 041c0800 00010000 f0020000 00000000 ................
+  0x00005db8 ffffffff 00000000 feffffff 00000000 ................
+  0x00005dc8 fdffffff 00000000 fcffffff 00000000 ................
+  0x00005dd8 73000000 00000000 00000011 25000536 s...........%..6
+  0x00005de8 24010000 00000000 02000000 0c000000 $...............
+  0x00005df8 b4000000 00000000 02000000 0b000000 ................
+  0x00005e08 44000000 00000000 02000000 0a000000 D...............
   0x00005e18 00000000 00000000 00000000 00000000 ................
   0x00005e28 00000000 00000000 00000000 00000000 ................
   0x00005e38 00000000 00000000 00000000 00000000 ................
   0x00005e48 00000000 00000000 00000000 00000000 ................
   0x00005e58 00000000 00000000 00000000 00000000 ................
   0x00005e68 00000000 00000000 00000000 00000000 ................
   0x00005e78 00000000 00000000 00000000 00000000 ................
@@ -333,1213 +331,1215 @@
   0x00006228 00000000 00000000 00000000 00000000 ................
   0x00006238 00000000 00000000 00000000 00000000 ................
   0x00006248 00000000 00000000 00000000 00000000 ................
   0x00006258 00000000 00000000 00000000 00000000 ................
   0x00006268 00000000 00000000 00000000 00000000 ................
   0x00006278 00000000 00000000 00000000 00000000 ................
   0x00006288 00000000 00000000 00000000 00000000 ................
-  0x00006298 00000000 00000000 027a0100 000a0000 .........z......
-  0x000062a8 000f0000 00e40f00 027a0400 005e0000 .........z...^..
-  0x000062b8 000f0000 00e20f00 b97a0600 00460000 .........z...F..
-  0x000062c8 000a0000 00e20f00 027a0500 005f0000 .........z..._..
-  0x000062d8 000f0000 00ca0f00 81790304 06080000 .........y......
-  0x000062e8 00191e0c 00a80e00 81790604 06000000 .........y......
-  0x000062f8 00191e0c 00e80e00 81790804 06100000 .........y......
-  0x00006308 00191e0c 00220f00 b97a0400 00000000 ....."...z......
-  0x00006318 00080000 00e40f00 9978043f 01000000 .........x.?....
-  0x00006328 04160108 00e20f00 19790b00 00000000 .........y......
-  0x00006338 00250000 00280e00 19790a00 00000000 .%...(...y......
-  0x00006348 00210000 00240e00 247a0b0b 00000000 .!...$..$z......
-  0x00006358 0a028e07 00ca1f00 1272020b 03000000 .........r......
-  0x00006368 fffc8e07 00e44f0c 1272100b 06000000 ......O..r......
-  0x00006378 fffc8e07 00e48f04 10720006 03000000 .........r......
-  0x00006388 ffe0ff07 00e40f00 0c72000b 02000000 .........r......
-  0x00006398 7052f003 00e40f04 1272070b 00000000 pR.......r......
-  0x000063a8 fffc8e07 00e40f04 0c72000b 10000000 .........r......
-  0x000063b8 70527000 00c40f00 10720c06 08000000 pRp......r......
-  0x000063c8 ffe0ff07 00e40f09 1272000b 08000000 .........r......
-  0x000063d8 fffc8e07 00e40f0c 0c72000b 07000000 .........r......
-  0x000063e8 70527000 00e40f00 10720303 08000000 pRp......r......
-  0x000063f8 ffe0ff07 00e40f00 1272080b 0c000000 .........r......
-  0x00006408 fffc8e07 00e40f04 0c72000b 00000000 .........r......
-  0x00006418 70527000 00c40f00 10720606 03000000 pRp......r......
-  0x00006428 ffe0ff07 00e40f08 1272040b 03000000 .........r......
-  0x00006438 fffc8e07 00e40f04 0c72000b 08000000 .........r......
-  0x00006448 70527000 00e40f04 1272050b 06000000 pRp......r......
-  0x00006458 fffc8e07 00e40f04 0c72000b 04000000 .........r......
-  0x00006468 70527000 00e40f00 197803ff 1f000000 pRp......x......
-  0x00006478 0b140100 00c40f00 0c72000b 05000000 .........r......
-  0x00006488 70527000 00c80f00 0c720010 02000000 pRp......r......
-  0x00006498 70527000 00c80f00 0c720010 07000000 pRp......r......
-  0x000064a8 70527000 00c80f00 0c720010 00000000 pRp......r......
-  0x000064b8 70527000 00c80f00 0c720010 08000000 pRp......r......
-  0x000064c8 70527000 00c80f00 0c720010 04000000 pRp......r......
-  0x000064d8 70527000 00c80f00 0c720010 05000000 pRp......r......
-  0x000064e8 70527000 00c80f00 0c720002 07000000 pRp......r......
-  0x000064f8 70527000 00c80f00 0c720002 00000000 pRp......r......
-  0x00006508 70527000 00c80f00 0c720002 08000000 pRp......r......
-  0x00006518 70527000 00c80f00 0c720002 04000000 pRp......r......
-  0x00006528 70527000 00c80f00 0c720002 05000000 pRp......r......
-  0x00006538 70527000 00c80f00 0c720007 00000000 pRp......r......
-  0x00006548 70527000 00c80f00 0c720007 08000000 pRp......r......
-  0x00006558 70527000 00c80f00 0c720007 04000000 pRp......r......
-  0x00006568 70527000 00c80f00 0c720007 05000000 pRp......r......
-  0x00006578 70527000 00c80f00 0c720000 08000000 pRp......r......
-  0x00006588 70527000 00c80f00 0c720000 04000000 pRp......r......
-  0x00006598 70527000 00c80f00 0c720000 05000000 pRp......r......
-  0x000065a8 70527200 00e40f08 0c7a000b 005c0000 pRr......z...\..
-  0x000065b8 7060f003 00e40f00 0c720008 04000000 p`.......r......
-  0x000065c8 7052f200 00e40f04 0c7a0003 005d0000 pR.......z...]..
-  0x000065d8 0061f003 00e40f00 0c720008 05000000 .a.......r......
-  0x000065e8 7052f200 00e40f00 0c7c000a 04000000 pR.......|......
-  0x000065f8 7010700c 00c40f00 0c720004 05000000 p.p......r......
-  0x00006608 7052f200 00c80f00 1c780000 00000000 pR.......x......
-  0x00006618 70307000 00da0f00 4d890000 00000000 p0p.....M.......
-  0x00006628 00008003 00ea0f00 357403ff 08000000 ........5t......
-  0x00006638 ff010000 00e20f00 027a2800 005a0000 .........z(..Z..
-  0x00006648 000f0000 00e40f00 027a2900 005b0000 .........z)..[..
-  0x00006658 000f0000 00ca0f00 81792428 06400000 .........y$(.@..
-  0x00006668 001b1e0c 00a40e00 25760a0b 00580000 ........%v...X..
-  0x00006678 03028e07 00e40f08 81792228 06800000 .........y"(....
-  0x00006688 001b1e0c 00e80e00 81791e0a 06000000 .........y......
-  0x00006698 001b1e0c 00a80e00 81791228 06c00000 .........y.(....
-  0x000066a8 001b1e0c 00280f00 81791a28 06000100 .....(...y.(....
-  0x000066b8 001b1e0c 00680f00 81790c28 06400100 .....h...y.(.@..
-  0x000066c8 001b1e0c 00280f00 81792628 06000000 .....(...y&(....
-  0x000066d8 001b1e0c 00280f00 81792028 06c00100 .....(...y (....
-  0x000066e8 001b1e0c 00680f00 81791628 06800100 .....h...y.(....
-  0x000066f8 001b1e0c 00620f00 25761010 00580000 .....b..%v...X..
-  0x00006708 03028e07 00c60f00 81791828 06080000 .........y.(....
-  0x00006718 001b1e0c 00680f00 81790e10 06000000 .....h...y......
-  0x00006728 001b1e0c 00680f00 81791428 06880000 .....h...y.(....
-  0x00006738 001b1e0c 00680f00 81791c28 06480000 .....h...y.(.H..
-  0x00006748 001b1e0c 00620f00 2072091f 25000000 .....b.. r..%...
-  0x00006758 00004000 00c44f00 2072061e 25000000 ..@...O. r..%...
-  0x00006768 00004000 00e40f04 2372091e 24000000 ..@.....#r..$...
-  0x00006778 09080000 00e40f0c 2372061f 24000000 ........#r..$...
-  0x00006788 06000000 00e40f04 2072251f 23000000 ........ r%.#...
-  0x00006798 00004000 00e48f08 2072241e 23000000 ..@..... r$.#...
-  0x000067a8 00004000 00e40f04 2372231e 22000000 ..@.....#r#."...
-  0x000067b8 25080000 00c40f00 2372221f 22000000 %.......#r"."...
-  0x000067c8 24000000 00e40f04 2072251f 13000000 $....... r%.....
-  0x000067d8 00004000 00e40f0d 2072241e 13000000 ..@..... r$.....
-  0x000067e8 00004000 00e40f04 2372131e 12000000 ..@.....#r......
-  0x000067f8 25080000 00e40f08 2372121f 12000000 %.......#r......
-  0x00006808 24000000 00e40f04 2072251f 1b000000 $....... r%.....
-  0x00006818 00004000 00c40f02 2072241e 1b000000 ..@..... r$.....
-  0x00006828 00004000 00e40f04 23721b1e 1a000000 ..@.....#r......
-  0x00006838 25080000 00e40f0c 23721a1f 1a000000 %.......#r......
-  0x00006848 24000000 00e40f04 2072251f 0d000000 $....... r%.....
-  0x00006858 00004000 00e40f08 2072241e 0d000000 ..@..... r$.....
-  0x00006868 00004000 00e40f00 20722b27 1f000000 ..@..... r+'....
-  0x00006878 00004000 00c40f00 20722a27 1e000000 ..@..... r*'....
-  0x00006888 00004000 00e40f00 2372251e 0c000000 ..@.....#r%.....
-  0x00006898 25080000 00e40f0c 2372241f 0c000000 %.......#r$.....
-  0x000068a8 24000000 00e40f04 20720d1f 21000000 $....... r..!...
-  0x000068b8 00004000 00e40f08 20720c1e 21000000 ..@..... r..!...
-  0x000068c8 00004000 00e40f00 23722b26 1e000000 ..@.....#r+&....
-  0x000068d8 2b080000 00c40f00 23722a26 1f000000 +.......#r*&....
-  0x000068e8 2a000000 00e40f00 2072271f 17000000 *....... r'.....
-  0x000068f8 00004000 00e40f0c 2072261e 17000000 ..@..... r&.....
-  0x00006908 00004000 00e40f04 2372211e 20000000 ..@.....#r!. ...
-  0x00006918 0d080000 00e40f0c 2372201f 20000000 ........#r . ...
-  0x00006928 0c000000 00e40f04 2372271e 16000000 ........#r'.....
-  0x00006938 27080000 00e20f08 81790c28 06c80000 '........y.(....
-  0x00006948 001b1e0c 00a20e00 2372261f 16000000 ........#r&.....
-  0x00006958 26000000 00c60f00 81791628 06080100 &........y.(....
-  0x00006968 001b1e0c 00e20e00 23721e18 0e000000 ........#r......
-  0x00006978 2b000000 00e40f0c 23722b18 0f000000 +.......#r+.....
-  0x00006988 2a000000 00e40f08 23722a19 0f000000 *.......#r*.....
-  0x00006998 1e010000 00e40f04 23722b19 0e000000 ........#r+.....
-  0x000069a8 2b000000 00e20f00 81791e28 06880100 +........y.(....
-  0x000069b8 001b1e0c 00280f00 81791828 06480100 .....(...y.(.H..
-  0x000069c8 001b1e0c 00620f00 23722e0e 14000000 .....b..#r......
-  0x000069d8 23000000 00c40f00 23722c0e 1c000000 #.......#r,.....
-  0x000069e8 09000000 00e40f08 23721c0f 1c000000 ........#r......
-  0x000069f8 06000000 00e40f04 2372220f 14000000 ........#r".....
-  0x00006a08 22000000 00e40f04 2372090f 15000080 ".......#r......
-  0x00006a18 2e000000 00e40f00 25762e02 00580000 ........%v...X..
-  0x00006a28 03028e07 00c80f00 2372060f 1d000080 ........#r......
-  0x00006a38 2c000000 00e40f0c 23722c0e 1d000000 ,.......#r,.....
-  0x00006a48 1c000000 00e40f04 81791c28 06c80100 .........y.(....
-  0x00006a58 001b1e0c 00220f00 2372220e 15000000 ....."..#r".....
-  0x00006a68 22000000 00e40f04 2372140e 0c000000 ".......#r......
-  0x00006a78 13000000 00e44f0c 2372120f 0c000000 ......O.#r......
-  0x00006a88 12000000 00e40f00 23720c0e 16000000 ........#r......
-  0x00006a98 1b000000 00c48f00 2372160f 16000000 ........#r......
-  0x00006aa8 1a000000 00e40f04 23721b0f 0d000080 ........#r......
-  0x00006ab8 14000000 00e40f0c 23721a0e 0d000000 ........#r......
-  0x00006ac8 12000000 00e20f00 81791428 06500000 .........y.(.P..
-  0x00006ad8 001b1e0c 00a20e00 2372230f 17000080 ........#r#.....
-  0x00006ae8 0c000000 00c60f00 81790c28 06100000 .........y.(....
-  0x00006af8 001b1e0c 00e80e00 8179122e 06000000 .........y......
-  0x00006b08 001b1e0c 00e20e00 2372020e 17000000 ........#r......
-  0x00006b18 16000000 00e40f04 2372160e 18000000 ........#r......
-  0x00006b28 25000000 00e40f0e 2372240f 18000000 %.......#r$.....
-  0x00006b38 24000000 00e40f00 2372180e 1e000000 $.......#r......
-  0x00006b48 27000000 00c40f01 2372260f 1e000000 '.......#r&.....
-  0x00006b58 26000000 00e40f04 2372250f 19000080 &.......#r%.....
-  0x00006b68 16000000 00e40f0c 23721e0e 19000000 ........#r......
-  0x00006b78 24000000 00e20f00 81791628 06900000 $........y.(....
-  0x00006b88 001b1e0c 00220f00 2372270f 1f000080 ....."..#r'.....
-  0x00006b98 18000000 00c60f00 81791828 06d00000 .........y.(....
-  0x00006ba8 001b1e0c 00620f00 2372240e 1c000000 .....b..#r$.....
-  0x00006bb8 21000000 00e40f0c 2372200f 1c000000 !.......#r .....
-  0x00006bc8 20000000 00e40f04 2372210f 1d000080  .......#r!.....
-  0x00006bd8 24000000 00e40f08 23721d0e 1d000000 $.......#r......
-  0x00006be8 20000000 00e40f04 23721f0e 1f000000  .......#r......
-  0x00006bf8 26000000 00e40f00 81790e28 06500100 &........y.(.P..
-  0x00006c08 001b1e0c 00620f00 23721c0c 12000000 .....b..#r......
-  0x00006c18 2a000000 00c48f00 23722b0c 13000000 *.......#r+.....
-  0x00006c28 2b000000 00e40f08 23721c0d 13000000 +.......#r......
-  0x00006c38 1c010000 00e40f04 2372200d 12000000 ........#r .....
-  0x00006c48 2b000000 00e40f00 81790c28 06100100 +........y.(....
-  0x00006c58 001b1e0c 00e20e00 23720612 14000000 ........#r......
-  0x00006c68 06000000 00e44f08 23722413 14000000 ......O.#r$.....
-  0x00006c78 2c000000 00e40f04 23720613 15000080 ,.......#r......
-  0x00006c88 06000000 00c40f00 23722412 15000000 ........#r$.....
-  0x00006c98 24000000 00e40f04 81791428 06900100 $........y.(....
-  0x00006ca8 001b1e0c 00a20e00 23722612 16000000 ........#r&.....
-  0x00006cb8 09000000 00e40f0d 23722213 16000000 ........#r".....
-  0x00006cc8 22000000 00e40f04 23721612 18000000 ".......#r......
-  0x00006cd8 1b000000 00e40f0a 23721813 18000000 ........#r......
-  0x00006ce8 1a000000 00e40f04 81791a28 06d00100 .........y.(....
-  0x00006cf8 001b1e0c 00220f00 23720913 17000080 ....."..#r......
-  0x00006d08 26000000 00c40f00 23721712 17000000 &.......#r......
-  0x00006d18 22000000 00e40f04 23722212 19000000 ".......#r".....
-  0x00006d28 18000000 00e40f00 23721e13 0e000000 ........#r......
-  0x00006d38 1e000000 00e40f00 25762c07 00580000 ........%v,..X..
-  0x00006d48 03028e07 00c80f00 23722612 0f000000 ........#r&.....
-  0x00006d58 1e000000 00e40f04 23721613 19000080 ........#r......
-  0x00006d68 16000000 00e40f04 23721812 0c000000 ........#r......
-  0x00006d78 23000000 00e48f0c 23720213 0c000000 #.......#r......
-  0x00006d88 02000000 00e40f04 23720c12 0e000000 ........#r......
-  0x00006d98 25000000 00e40f00 23722313 0d000080 %.......#r#.....
-  0x00006da8 18000000 00c40f00 23720212 0d000000 ........#r......
-  0x00006db8 02000000 00e40f04 23720713 0f000080 ........#r......
-  0x00006dc8 0c000000 00e40f04 23721812 14000000 ........#r......
-  0x00006dd8 27000000 00e24f08 81790c28 06180000 '.....O..y.(....
-  0x00006de8 001b1e0c 00a20e00 23721f13 14000000 ........#r......
-  0x00006df8 1f000000 00c60f00 81790e2c 06000000 .........y.,....
-  0x00006e08 001b1e0c 00a20e00 23722513 15000080 ........#r%.....
-  0x00006e18 18000000 00e40f0c 23722a12 15000000 ........#r*.....
-  0x00006e28 1f000000 00e20f04 81791828 06980000 .........y.(....
-  0x00006e38 001b1e0c 00e80e00 81791428 06580000 .........y.(.X..
-  0x00006e48 001b1e0c 00620f00 23721e12 1a000000 .....b..#r......
-  0x00006e58 21000000 00e40f09 23721a13 1a000000 !.......#r......
-  0x00006e68 1d000000 00c40f00 23721d13 1b000080 ........#r......
-  0x00006e78 1e000000 00e40f08 81791e28 06d80000 .........y.(....
-  0x00006e88 001b1e0c 00220f00 23721b12 1b000000 ....."..#r......
-  0x00006e98 1a000000 00e40f00 23721c0c 0e000000 ........#r......
-  0x00006ea8 1c000000 00e44f0c 2372200c 0f000000 ......O.#r .....
-  0x00006eb8 20000000 00e40f08 23721a0d 0f000000  .......#r......
-  0x00006ec8 1c010000 00e40f04 23721c0d 0e000000 ........#r......
-  0x00006ed8 20000000 00c40f00 2372120e 18000000  .......#r......
-  0x00006ee8 09000000 00e28f04 81790c28 06180100 .........y.(....
-  0x00006ef8 001b1e0c 00a20e00 2372060e 14000000 ........#r......
-  0x00006f08 06000000 00e40f0e 2372240f 14000000 ........#r$.....
-  0x00006f18 24000000 00e40f04 2372170f 18000000 $.......#r......
-  0x00006f28 17000000 00e40f04 2372180f 19000080 ........#r......
-  0x00006f38 12000000 00e40f04 2372060f 15000080 ........#r......
-  0x00006f48 06000000 00e20f08 81791228 06580100 .........y.(.X..
-  0x00006f58 001b1e0c 00e20e00 2372090e 15000000 ........#r......
-  0x00006f68 24000000 00c60f00 81791428 06980100 $........y.(....
-  0x00006f78 001b1e0c 00620f00 2372190e 19000000 .....b..#r......
-  0x00006f88 17000000 00e40f04 2372200e 1e000000 ........#r .....
-  0x00006f98 16000000 00e40f0d 81791628 06d80100 .........y.(....
-  0x00006fa8 001b1e0c 00220f00 2372220f 1e000000 ....."..#r".....
-  0x00006fb8 22000000 00e40f04 23721e0e 0c000000 ".......#r......
-  0x00006fc8 23000000 00e44f08 2372210f 0c000000 #.....O.#r!.....
-  0x00006fd8 02000000 00c40f00 23720c0f 0d000080 ........#r......
-  0x00006fe8 1e000000 00e40f04 2372020f 1f000080 ........#r......
-  0x00006ff8 20000000 00e40f04 23721e0e 12000000  .......#r......
-  0x00007008 07000000 00e48f0c 2372240f 12000000 ........#r$.....
-  0x00007018 26000000 00e40f04 2372120e 14000000 &.......#r......
-  0x00007028 25000000 00e40f0a 2372140f 14000000 %.......#r......
-  0x00007038 2a000000 00c40f00 25762a00 00580000 *.......%v*..X..
-  0x00007048 03028e07 00c80f00 2372200e 1f000000 ........#r .....
-  0x00007058 22000000 00e40f04 2372220e 0d000000 ".......#r".....
-  0x00007068 21000000 00e40f04 2372070f 13000080 !.......#r......
-  0x00007078 1e000000 00e40f0c 2372240e 13000000 ........#r$.....
-  0x00007088 24000000 00e20f04 81791e28 06600000 $........y.(.`..
-  0x00007098 001b1e0c 00a20e00 23720d0f 15000080 ........#r......
-  0x000070a8 12000000 00e40f08 2372000e 15000000 ........#r......
-  0x000070b8 14000000 00e20f04 8179122a 06000000 .........y.*....
-  0x000070c8 001b1e0c 00e20e00 2372260e 16000000 ........#r&.....
-  0x000070d8 1d000000 00c40f01 2372160f 16000000 ........#r......
-  0x000070e8 1b000000 00e20f04 81791428 06200000 .........y.(. ..
-  0x000070f8 001b1e0c 00e20e00 23721b0f 17000080 ........#r......
-  0x00007108 26000000 00e40f08 2372260e 17000000 &.......#r&.....
-  0x00007118 16000000 00e40f00 81790e28 06a00000 .........y.(....
-  0x00007128 001b1e0c 00280f00 81791628 06e00000 .....(...y.(....
-  0x00007138 001b1e0c 00620f00 23721a14 12000000 .....b..#r......
-  0x00007148 1a000000 00c48f00 23721c14 13000000 ........#r......
-  0x00007158 1c000000 00e40f08 23721412 1e000000 ........#r......
-  0x00007168 06000000 00e44f0c 23721e13 1e000000 ......O.#r......
-  0x00007178 09000000 00e40f00 23720915 12000000 ........#r......
-  0x00007188 1c000000 00e40f04 23720615 13000000 ........#r......
-  0x00007198 1a010000 00e40f00 23721c12 0e000000 ........#r......
-  0x000071a8 18000000 00c40f01 23721a13 1f000080 ........#r......
-  0x000071b8 14000000 00e40f0c 23720e13 0e000000 ........#r......
-  0x000071c8 19000000 00e20f04 81791428 06200100 .........y.(. ..
-  0x000071d8 001b1e0c 00a20e00 23721f12 1f000000 ........#r......
-  0x000071e8 1e000000 00e40f04 23721e12 16000000 ........#r......
-  0x000071f8 02000000 00e20f0a 81791828 06600100 .........y.(.`..
-  0x00007208 001b1e0c 00e20e00 23722013 16000000 ........#r .....
-  0x00007218 20000000 00e40f04 23720213 0f000080  .......#r......
-  0x00007228 1c000000 00c40f00 23721c12 0f000000 ........#r......
-  0x00007238 0e000000 00e40f04 81790e28 06a00100 .........y.(....
-  0x00007248 001b1e0c 00220f00 23721d13 17000080 ....."..#r......
-  0x00007258 1e000000 00e40f0c 23721e12 17000000 ........#r......
-  0x00007268 20000000 00e40f04 81791628 06e00100  ........y.(....
-  0x00007278 001b1e0c 00620f00 23720c12 14000000 .....b..#r......
-  0x00007288 0c000000 00e44f08 23722213 14000000 ......O.#r".....
-  0x00007298 22000000 00c40f00 23721412 18000000 ".......#r......
-  0x000072a8 07000000 00e48f08 23720713 15000080 ........#r......
-  0x000072b8 0c000000 00e40f04 23722013 18000000 ........#r .....
-  0x000072c8 24000000 00e40f00 25762408 00580000 $.......%v$..X..
-  0x000072d8 03028e07 00c80f00 23720c12 0e000000 ........#r......
-  0x000072e8 0d000000 00e40f0d 23720013 0e000000 ........#r......
-  0x000072f8 00000000 00e40f04 23721812 15000000 ........#r......
-  0x00007308 22000000 00e40f04 23720812 16000000 ".......#r......
-  0x00007318 1b000000 00e40f0a 23722213 16000000 ........#r".....
-  0x00007328 26000000 00e40f04 23722113 19000080 &.......#r!.....
-  0x00007338 14000000 00c40f00 23722012 19000000 ........#r .....
-  0x00007348 20000000 00e20f04 81791428 06680000  ........y.(.h..
-  0x00007358 001b1e0c 00a20e00 23721913 0f000080 ........#r......
-  0x00007368 0c000000 00e40f0c 23720012 0f000000 ........#r......
-  0x00007378 00000000 00e20f04 81790c24 06000000 .........y.$....
-  0x00007388 001b1e0c 00a20e00 23721b13 17000080 ........#r......
-  0x00007398 08000000 00e40f08 23722212 17000000 ........#r".....
-  0x000073a8 22000000 00e20f00 81790e28 06280000 "........y.(.(..
-  0x000073b8 001b1e0c 00e80e00 81791228 06a80000 .........y.(....
-  0x000073c8 001b1e0c 00280f00 81791628 06e80000 .....(...y.(....
-  0x000073d8 001b1e0c 00620f00 2372230d 14000000 .....b..#r#.....
-  0x000073e8 1f000000 00c44f00 2372090e 0d000000 ......O.#r......
-  0x000073f8 09000000 00e48f04 2372060e 0c000000 ........#r......
-  0x00007408 06000000 00e40f00 2372020c 12000000 ........#r......
-  0x00007418 02000000 00e40f0d 23721c0d 12000000 ........#r......
-  0x00007428 1c000000 00e40f00 23721f0f 0c000000 ........#r......
-  0x00007438 09000000 00e40f00 23721a0c 14000000 ........#r......
-  0x00007448 1a000000 00e20f00 81790828 06280100 .........y.(.(..
-  0x00007458 001b1e0c 00a20e00 2372020d 13000080 ........#r......
-  0x00007468 02000000 00c40f00 23721c0c 13000000 ........#r......
-  0x00007478 1c000000 00e40f04 2372060f 0d000000 ........#r......
-  0x00007488 06010000 00e20f00 81791228 06680100 .........y.(.h..
-  0x00007498 001b1e0c 00e20e00 2372140c 16000000 ........#r......
-  0x000074a8 1d000000 00c60f02 81790e28 06a80100 .........y.(....
-  0x000074b8 001b1e0c 00220f00 23721e0d 16000000 ....."..#r......
-  0x000074c8 1e000000 00e40f04 23721a0d 15000080 ........#r......
-  0x000074d8 1a000000 00e40f0c 2372230c 15000000 ........#r#.....
-  0x000074e8 23000000 00e40f04 2372160d 17000080 #.......#r......
-  0x000074f8 14000000 00e40f08 81791428 06e80100 .........y.(....
-  0x00007508 001b1e0c 00620f00 2372170c 17000000 .....b..#r......
-  0x00007518 1e000000 00c40f00 25762604 00580000 ........%v&..X..
-  0x00007528 03028e07 00c80f00 23721e0c 08000000 ........#r......
-  0x00007538 07000000 00e44f0c 2372180d 08000000 ......O.#r......
-  0x00007548 18000000 00e40f04 2372080c 12000000 ........#r......
-  0x00007558 21000000 00e48f0c 2372200d 12000000 !.......#r .....
-  0x00007568 20000000 00e40f04 2372120c 0e000000  .......#r......
-  0x00007578 19000000 00e40f01 2372070d 09000080 ........#r......
-  0x00007588 1e000000 00c40f00 23720e0d 0e000000 ........#r......
-  0x00007598 00000000 00e40f04 23721d0d 0f000080 ........#r......
-  0x000075a8 12000000 00e40f04 2372120c 14000000 ........#r......
-  0x000075b8 1b000000 00e40f0e 23721e0d 14000000 ........#r......
-  0x000075c8 22000000 00e40f04 2372180c 09000000 ".......#r......
-  0x000075d8 18000000 00e40f00 2372190d 13000080 ........#r......
-  0x000075e8 08000000 00c40f00 2372000c 13000000 ........#r......
-  0x000075f8 20000000 00e20f04 81790828 06300000  ........y.(.0..
-  0x00007608 001b1e0c 00a20e00 2372040c 0f000000 ........#r......
-  0x00007618 0e000000 00e40f04 23721b0d 15000080 ........#r......
-  0x00007628 12000000 00e20f08 81790e26 06000000 .........y.&....
-  0x00007638 001b1e0c 00a20e00 23721e0c 15000000 ........#r......
-  0x00007648 1e000000 00c60f00 81790c28 06700000 .........y.(.p..
-  0x00007658 001b1e0c 00e80e00 81791228 06b00000 .........y.(....
-  0x00007668 001b1e0c 00280f00 81791428 06f00000 .....(...y.(....
-  0x00007678 001b1e0c 00620f00 23720608 0e000000 .....b..#r......
-  0x00007688 06000000 00e44f04 23721f08 0f000000 ......O.#r......
-  0x00007698 1f000000 00c40f00 23721a0e 0c000000 ........#r......
-  0x000076a8 1a000000 00e48f0c 2372230f 0c000000 ........#r#.....
-  0x000076b8 23000000 00e40f04 2372080e 12000000 #.......#r......
-  0x000076c8 02000000 00e40f0d 2372020f 0d000080 ........#r......
-  0x000076d8 1a000000 00e40f0c 2372200f 12000000 ........#r .....
-  0x000076e8 1c000000 00e40f00 23721a0e 0d000000 ........#r......
-  0x000076f8 23000000 00c40f00 23720609 0f000000 #.......#r......
-  0x00007708 06010000 00e20f04 81790c28 06300100 .........y.(.0..
-  0x00007718 001b1e0c 00a20e00 23721f09 0e000000 ........#r......
-  0x00007728 1f000000 00e40f00 23721c0f 13000080 ........#r......
-  0x00007738 08000000 00e40f0c 81790828 06700100 .........y.(.p..
-  0x00007748 001b1e0c 00e20e00 2372160e 14000000 ........#r......
-  0x00007758 16000000 00e40f0e 2372170f 14000000 ........#r......
-  0x00007768 17000000 00e40f00 2372200e 13000000 ........#r .....
-  0x00007778 20000000 00c40f00 2372160f 15000080  .......#r......
-  0x00007788 16000000 00e20f08 81791228 06b00100 .........y.(....
-  0x00007798 001b1e0c 00220f00 2372170e 15000000 ....."..#r......
-  0x000077a8 17000000 00c60f00 81791428 06f00100 .........y.(....
-  0x000077b8 001b1e0c 00620f00 25763005 00580000 .....b..%v0..X..
-  0x000077c8 03028e07 00c80f00 2372220e 0c000000 ........#r".....
-  0x000077d8 07000000 00e44f0c 2372180f 0c000000 ......O.#r......
-  0x000077e8 18000000 00e40f04 23720c0e 08000000 ........#r......
-  0x000077f8 19000000 00e48f08 2372080f 08000000 ........#r......
-  0x00007808 00000000 00e40f04 2372000f 0d000080 ........#r......
-  0x00007818 22000000 00e40f04 2372070f 09000080 ".......#r......
-  0x00007828 0c000000 00c40f00 2372220e 09000000 ........#r".....
-  0x00007838 08000000 00e40f04 2372080e 12000000 ........#r......
-  0x00007848 1d000000 00e40f0d 2372040f 12000000 ........#r......
-  0x00007858 04000000 00e40f04 23720c0e 14000000 ........#r......
-  0x00007868 1b000000 00e40f0e 23721e0f 14000000 ........#r......
-  0x00007878 1e000000 00e40f00 2372180e 0d000000 ........#r......
-  0x00007888 18000000 00c40f00 2372190f 13000080 ........#r......
-  0x00007898 08000000 00e40f0c 2372140e 13000000 ........#r......
-  0x000078a8 04000000 00e20f00 81790830 06000000 .........y.0....
-  0x000078b8 001b1e0c 00a20e00 2372210f 15000080 ........#r!.....
-  0x000078c8 0c000000 00c60f00 81790428 06380000 .........y.(.8..
-  0x000078d8 001b1e0c 00a80e00 81790c28 06780000 .........y.(.x..
-  0x000078e8 001b1e0c 00e20e00 2372150e 15000000 ........#r......
-  0x000078f8 1e000000 00c60f00 81790e28 06b80000 .........y.(....
-  0x00007908 001b1e0c 00280f00 81791228 06f80000 .....(...y.(....
-  0x00007918 001b1e0c 00620f00 23720304 09000000 .....b..#r......
-  0x00007928 1f000000 00e44f04 23720604 08000000 ......O.#r......
-  0x00007938 06000000 00e40f00 23721a09 0c000000 ........#r......
-  0x00007948 1a000000 00e48f08 23720408 0c000000 ........#r......
-  0x00007958 02000000 00c40f00 23720305 08000000 ........#r......
-  0x00007968 03000000 00e40f04 23720205 09000000 ........#r......
-  0x00007978 06010000 00e40f00 23720508 0d000000 ........#r......
-  0x00007988 1a000000 00e40f0c 23720608 0e000000 ........#r......
-  0x00007998 1c000000 00e20f0d 81791a28 06380100 .........y.(.8..
-  0x000079a8 001b1e0c 00a20e00 23722009 0e000000 ........#r .....
-  0x000079b8 20000000 00e40f04 23720e08 12000000  .......#r......
-  0x000079c8 16000000 00e20f02 81791c28 06f80100 .........y.(....
-  0x000079d8 001b1e0c 00e20e00 23720409 0d000080 ........#r......
-  0x000079e8 04000000 00c40f00 23721209 12000000 ........#r......
-  0x000079f8 17000000 00e20f04 81790c28 06b80100 .........y.(....
-  0x00007a08 001b1e0c 00280f00 81791628 06780100 .....(...y.(.x..
-  0x00007a18 001b1e0c 00620f00 23720609 0f000080 .....b..#r......
-  0x00007a28 06000000 00e40f04 23720e09 13000080 ........#r......
-  0x00007a38 0e000000 00e20f00 8679000a 02000000 .........y......
-  0x00007a48 061b100c 00e80f00 86790010 04000000 .........y......
-  0x00007a58 061b100c 00e20f00 23720008 1a000000 ........#r......
-  0x00007a68 00000000 00c44f00 23721a09 1a000000 ......O.#r......
-  0x00007a78 18000000 00e40f04 23721509 1c000000 ........#r......
-  0x00007a88 15000000 00e48f0c 23721c08 1c000000 ........#r......
-  0x00007a98 21000000 00e40f04 23721409 0c000000 !.......#r......
-  0x00007aa8 14000000 00e40f09 23720c08 0c000000 ........#r......
-  0x00007ab8 19000000 00e40f04 23721808 16000000 ........#r......
-  0x00007ac8 07000000 00c40f02 23722209 16000000 ........#r".....
-  0x00007ad8 22000000 00e40f04 23720708 0f000000 ".......#r......
-  0x00007ae8 20000000 00e40f04 23720f08 13000000  .......#r......
-  0x00007af8 12000000 00e40f04 23721308 1b000000 ........#r......
-  0x00007b08 1a000000 00e40f0c 23721209 1b000080 ........#r......
-  0x00007b18 00000000 00e40f00 23721b08 17000000 ........#r......
-  0x00007b28 22000000 00c40f00 23721a09 17000080 ".......#r......
-  0x00007b38 18000000 00e20f04 8679002e 06000000 .........y......
-  0x00007b48 061b100c 00e20f00 23721708 0d000000 ........#r......
-  0x00007b58 14000000 00e40f0c 23721609 0d000080 ........#r......
-  0x00007b68 0c000000 00e20f04 8679002c 0e000000 .........y.,....
-  0x00007b78 061b100c 00e20f00 23721508 1d000000 ........#r......
-  0x00007b88 15000000 00e40f08 23721409 1d000080 ........#r......
-  0x00007b98 1c000000 00e20f00 8679002a 12000000 .........y.*....
-  0x00007ba8 061b100c 00e80f00 86790024 1a000000 .........y.$....
-  0x00007bb8 061b100c 00e80f00 86790026 16000000 .........y.&....
-  0x00007bc8 061b100c 00e80f00 86790030 14000000 .........y.0....
-  0x00007bd8 061b100c 00e20f00 4d790000 00000000 ........My......
-  0x00007be8 00008003 00ea0f00 47790000 f0ffffff ........Gy......
-  0x00007bf8 ffff8303 00c00f00 18790000 00000000 .........y......
-  0x00007c08 00000000 00c00f00 18790000 00000000 .........y......
-  0x00007c18 00000000 00c00f00 18790000 00000000 .........y......
+  0x00006298 00000000 00000000 00000000 00000000 ................
+  0x000062a8 00000000 00000000 00000000 00000000 ................
+  0x000062b8 00000000 00000000 027a0100 000a0000 .........z......
+  0x000062c8 000f0000 00e40f00 027a0400 005e0000 .........z...^..
+  0x000062d8 000f0000 00e20f00 b97a0600 00460000 .........z...F..
+  0x000062e8 000a0000 00e20f00 027a0500 005f0000 .........z..._..
+  0x000062f8 000f0000 00ca0f00 81790304 06080000 .........y......
+  0x00006308 00191e0c 00a80e00 81790604 06000000 .........y......
+  0x00006318 00191e0c 00e80e00 81790804 06100000 .........y......
+  0x00006328 00191e0c 00220f00 b97a0400 00000000 ....."...z......
+  0x00006338 00080000 00e40f00 9978043f 01000000 .........x.?....
+  0x00006348 04160108 00e20f00 19790b00 00000000 .........y......
+  0x00006358 00250000 00280e00 19790a00 00000000 .%...(...y......
+  0x00006368 00210000 00240e00 247a0b0b 00000000 .!...$..$z......
+  0x00006378 0a028e07 00ca1f00 1272020b 03000000 .........r......
+  0x00006388 fffc8e07 00e44f0c 1272100b 06000000 ......O..r......
+  0x00006398 fffc8e07 00e48f04 10720006 03000000 .........r......
+  0x000063a8 ffe0ff07 00e40f00 0c72000b 02000000 .........r......
+  0x000063b8 7052f003 00e40f04 1272070b 00000000 pR.......r......
+  0x000063c8 fffc8e07 00e40f04 0c72000b 10000000 .........r......
+  0x000063d8 70527000 00c40f00 10720c06 08000000 pRp......r......
+  0x000063e8 ffe0ff07 00e40f09 1272000b 08000000 .........r......
+  0x000063f8 fffc8e07 00e40f0c 0c72000b 07000000 .........r......
+  0x00006408 70527000 00e40f00 10720303 08000000 pRp......r......
+  0x00006418 ffe0ff07 00e40f00 1272080b 0c000000 .........r......
+  0x00006428 fffc8e07 00e40f04 0c72000b 00000000 .........r......
+  0x00006438 70527000 00c40f00 10720606 03000000 pRp......r......
+  0x00006448 ffe0ff07 00e40f08 1272040b 03000000 .........r......
+  0x00006458 fffc8e07 00e40f04 0c72000b 08000000 .........r......
+  0x00006468 70527000 00e40f04 1272050b 06000000 pRp......r......
+  0x00006478 fffc8e07 00e40f04 0c72000b 04000000 .........r......
+  0x00006488 70527000 00e40f00 197803ff 1f000000 pRp......x......
+  0x00006498 0b140100 00c40f00 0c72000b 05000000 .........r......
+  0x000064a8 70527000 00c80f00 0c720010 02000000 pRp......r......
+  0x000064b8 70527000 00c80f00 0c720010 07000000 pRp......r......
+  0x000064c8 70527000 00c80f00 0c720010 00000000 pRp......r......
+  0x000064d8 70527000 00c80f00 0c720010 08000000 pRp......r......
+  0x000064e8 70527000 00c80f00 0c720010 04000000 pRp......r......
+  0x000064f8 70527000 00c80f00 0c720010 05000000 pRp......r......
+  0x00006508 70527000 00c80f00 0c720002 07000000 pRp......r......
+  0x00006518 70527000 00c80f00 0c720002 00000000 pRp......r......
+  0x00006528 70527000 00c80f00 0c720002 08000000 pRp......r......
+  0x00006538 70527000 00c80f00 0c720002 04000000 pRp......r......
+  0x00006548 70527000 00c80f00 0c720002 05000000 pRp......r......
+  0x00006558 70527000 00c80f00 0c720007 00000000 pRp......r......
+  0x00006568 70527000 00c80f00 0c720007 08000000 pRp......r......
+  0x00006578 70527000 00c80f00 0c720007 04000000 pRp......r......
+  0x00006588 70527000 00c80f00 0c720007 05000000 pRp......r......
+  0x00006598 70527000 00c80f00 0c720000 08000000 pRp......r......
+  0x000065a8 70527000 00c80f00 0c720000 04000000 pRp......r......
+  0x000065b8 70527000 00c80f00 0c720000 05000000 pRp......r......
+  0x000065c8 70527200 00e40f08 0c7a000b 005c0000 pRr......z...\..
+  0x000065d8 7060f003 00e40f00 0c720008 04000000 p`.......r......
+  0x000065e8 7052f200 00e40f04 0c7a0003 005d0000 pR.......z...]..
+  0x000065f8 0061f003 00e40f00 0c720008 05000000 .a.......r......
+  0x00006608 7052f200 00e40f00 0c7c000a 04000000 pR.......|......
+  0x00006618 7010700c 00c40f00 0c720004 05000000 p.p......r......
+  0x00006628 7052f200 00c80f00 1c780000 00000000 pR.......x......
+  0x00006638 70307000 00da0f00 4d890000 00000000 p0p.....M.......
+  0x00006648 00008003 00ea0f00 357403ff 08000000 ........5t......
+  0x00006658 ff010000 00e20f00 027a2800 005a0000 .........z(..Z..
+  0x00006668 000f0000 00e40f00 027a2900 005b0000 .........z)..[..
+  0x00006678 000f0000 00ca0f00 81792428 06400000 .........y$(.@..
+  0x00006688 001b1e0c 00a40e00 25760a0b 00580000 ........%v...X..
+  0x00006698 03028e07 00e40f08 81792228 06800000 .........y"(....
+  0x000066a8 001b1e0c 00e80e00 81791e0a 06000000 .........y......
+  0x000066b8 001b1e0c 00a80e00 81791228 06c00000 .........y.(....
+  0x000066c8 001b1e0c 00280f00 81791a28 06000100 .....(...y.(....
+  0x000066d8 001b1e0c 00680f00 81790c28 06400100 .....h...y.(.@..
+  0x000066e8 001b1e0c 00280f00 81792628 06000000 .....(...y&(....
+  0x000066f8 001b1e0c 00280f00 81792028 06c00100 .....(...y (....
+  0x00006708 001b1e0c 00680f00 81791628 06800100 .....h...y.(....
+  0x00006718 001b1e0c 00620f00 25761010 00580000 .....b..%v...X..
+  0x00006728 03028e07 00c60f00 81791828 06080000 .........y.(....
+  0x00006738 001b1e0c 00680f00 81790e10 06000000 .....h...y......
+  0x00006748 001b1e0c 00680f00 81791428 06880000 .....h...y.(....
+  0x00006758 001b1e0c 00680f00 81791c28 06480000 .....h...y.(.H..
+  0x00006768 001b1e0c 00620f00 2072091f 25000000 .....b.. r..%...
+  0x00006778 00004000 00c44f00 2072061e 25000000 ..@...O. r..%...
+  0x00006788 00004000 00e40f04 2372091e 24000000 ..@.....#r..$...
+  0x00006798 09080000 00e40f0c 2372061f 24000000 ........#r..$...
+  0x000067a8 06000000 00e40f04 2072251f 23000000 ........ r%.#...
+  0x000067b8 00004000 00e48f08 2072241e 23000000 ..@..... r$.#...
+  0x000067c8 00004000 00e40f04 2372231e 22000000 ..@.....#r#."...
+  0x000067d8 25080000 00c40f00 2372221f 22000000 %.......#r"."...
+  0x000067e8 24000000 00e40f04 2072251f 13000000 $....... r%.....
+  0x000067f8 00004000 00e40f0d 2072241e 13000000 ..@..... r$.....
+  0x00006808 00004000 00e40f04 2372131e 12000000 ..@.....#r......
+  0x00006818 25080000 00e40f08 2372121f 12000000 %.......#r......
+  0x00006828 24000000 00e40f04 2072251f 1b000000 $....... r%.....
+  0x00006838 00004000 00c40f02 2072241e 1b000000 ..@..... r$.....
+  0x00006848 00004000 00e40f04 23721b1e 1a000000 ..@.....#r......
+  0x00006858 25080000 00e40f0c 23721a1f 1a000000 %.......#r......
+  0x00006868 24000000 00e40f04 2072251f 0d000000 $....... r%.....
+  0x00006878 00004000 00e40f08 2072241e 0d000000 ..@..... r$.....
+  0x00006888 00004000 00e40f00 20722b27 1f000000 ..@..... r+'....
+  0x00006898 00004000 00c40f00 20722a27 1e000000 ..@..... r*'....
+  0x000068a8 00004000 00e40f00 2372251e 0c000000 ..@.....#r%.....
+  0x000068b8 25080000 00e40f0c 2372241f 0c000000 %.......#r$.....
+  0x000068c8 24000000 00e40f04 20720d1f 21000000 $....... r..!...
+  0x000068d8 00004000 00e40f08 20720c1e 21000000 ..@..... r..!...
+  0x000068e8 00004000 00e40f00 23722b26 1e000000 ..@.....#r+&....
+  0x000068f8 2b080000 00c40f00 23722a26 1f000000 +.......#r*&....
+  0x00006908 2a000000 00e40f00 2072271f 17000000 *....... r'.....
+  0x00006918 00004000 00e40f0c 2072261e 17000000 ..@..... r&.....
+  0x00006928 00004000 00e40f04 2372211e 20000000 ..@.....#r!. ...
+  0x00006938 0d080000 00e40f0c 2372201f 20000000 ........#r . ...
+  0x00006948 0c000000 00e40f04 2372271e 16000000 ........#r'.....
+  0x00006958 27080000 00e20f08 81790c28 06c80000 '........y.(....
+  0x00006968 001b1e0c 00a20e00 2372261f 16000000 ........#r&.....
+  0x00006978 26000000 00c60f00 81791628 06080100 &........y.(....
+  0x00006988 001b1e0c 00e20e00 23721e18 0e000000 ........#r......
+  0x00006998 2b000000 00e40f0c 23722b18 0f000000 +.......#r+.....
+  0x000069a8 2a000000 00e40f08 23722a19 0f000000 *.......#r*.....
+  0x000069b8 1e010000 00e40f04 23722b19 0e000000 ........#r+.....
+  0x000069c8 2b000000 00e20f00 81791e28 06880100 +........y.(....
+  0x000069d8 001b1e0c 00280f00 81791828 06480100 .....(...y.(.H..
+  0x000069e8 001b1e0c 00620f00 23722e0e 14000000 .....b..#r......
+  0x000069f8 23000000 00c40f00 23722c0e 1c000000 #.......#r,.....
+  0x00006a08 09000000 00e40f08 23721c0f 1c000000 ........#r......
+  0x00006a18 06000000 00e40f04 2372220f 14000000 ........#r".....
+  0x00006a28 22000000 00e40f04 2372090f 15000080 ".......#r......
+  0x00006a38 2e000000 00e40f00 25762e02 00580000 ........%v...X..
+  0x00006a48 03028e07 00c80f00 2372060f 1d000080 ........#r......
+  0x00006a58 2c000000 00e40f0c 23722c0e 1d000000 ,.......#r,.....
+  0x00006a68 1c000000 00e40f04 81791c28 06c80100 .........y.(....
+  0x00006a78 001b1e0c 00220f00 2372220e 15000000 ....."..#r".....
+  0x00006a88 22000000 00e40f04 2372140e 0c000000 ".......#r......
+  0x00006a98 13000000 00e44f0c 2372120f 0c000000 ......O.#r......
+  0x00006aa8 12000000 00e40f00 23720c0e 16000000 ........#r......
+  0x00006ab8 1b000000 00c48f00 2372160f 16000000 ........#r......
+  0x00006ac8 1a000000 00e40f04 23721b0f 0d000080 ........#r......
+  0x00006ad8 14000000 00e40f0c 23721a0e 0d000000 ........#r......
+  0x00006ae8 12000000 00e20f00 81791428 06500000 .........y.(.P..
+  0x00006af8 001b1e0c 00a20e00 2372230f 17000080 ........#r#.....
+  0x00006b08 0c000000 00c60f00 81790c28 06100000 .........y.(....
+  0x00006b18 001b1e0c 00e80e00 8179122e 06000000 .........y......
+  0x00006b28 001b1e0c 00e20e00 2372020e 17000000 ........#r......
+  0x00006b38 16000000 00e40f04 2372160e 18000000 ........#r......
+  0x00006b48 25000000 00e40f0e 2372240f 18000000 %.......#r$.....
+  0x00006b58 24000000 00e40f00 2372180e 1e000000 $.......#r......
+  0x00006b68 27000000 00c40f01 2372260f 1e000000 '.......#r&.....
+  0x00006b78 26000000 00e40f04 2372250f 19000080 &.......#r%.....
+  0x00006b88 16000000 00e40f0c 23721e0e 19000000 ........#r......
+  0x00006b98 24000000 00e20f00 81791628 06900000 $........y.(....
+  0x00006ba8 001b1e0c 00220f00 2372270f 1f000080 ....."..#r'.....
+  0x00006bb8 18000000 00c60f00 81791828 06d00000 .........y.(....
+  0x00006bc8 001b1e0c 00620f00 2372240e 1c000000 .....b..#r$.....
+  0x00006bd8 21000000 00e40f0c 2372200f 1c000000 !.......#r .....
+  0x00006be8 20000000 00e40f04 2372210f 1d000080  .......#r!.....
+  0x00006bf8 24000000 00e40f08 23721d0e 1d000000 $.......#r......
+  0x00006c08 20000000 00e40f04 23721f0e 1f000000  .......#r......
+  0x00006c18 26000000 00e40f00 81790e28 06500100 &........y.(.P..
+  0x00006c28 001b1e0c 00620f00 23721c0c 12000000 .....b..#r......
+  0x00006c38 2a000000 00c48f00 23722b0c 13000000 *.......#r+.....
+  0x00006c48 2b000000 00e40f08 23721c0d 13000000 +.......#r......
+  0x00006c58 1c010000 00e40f04 2372200d 12000000 ........#r .....
+  0x00006c68 2b000000 00e40f00 81790c28 06100100 +........y.(....
+  0x00006c78 001b1e0c 00e20e00 23720612 14000000 ........#r......
+  0x00006c88 06000000 00e44f08 23722413 14000000 ......O.#r$.....
+  0x00006c98 2c000000 00e40f04 23720613 15000080 ,.......#r......
+  0x00006ca8 06000000 00c40f00 23722412 15000000 ........#r$.....
+  0x00006cb8 24000000 00e40f04 81791428 06900100 $........y.(....
+  0x00006cc8 001b1e0c 00a20e00 23722612 16000000 ........#r&.....
+  0x00006cd8 09000000 00e40f0d 23722213 16000000 ........#r".....
+  0x00006ce8 22000000 00e40f04 23721612 18000000 ".......#r......
+  0x00006cf8 1b000000 00e40f0a 23721813 18000000 ........#r......
+  0x00006d08 1a000000 00e40f04 81791a28 06d00100 .........y.(....
+  0x00006d18 001b1e0c 00220f00 23720913 17000080 ....."..#r......
+  0x00006d28 26000000 00c40f00 23721712 17000000 &.......#r......
+  0x00006d38 22000000 00e40f04 23722212 19000000 ".......#r".....
+  0x00006d48 18000000 00e40f00 23721e13 0e000000 ........#r......
+  0x00006d58 1e000000 00e40f00 25762c07 00580000 ........%v,..X..
+  0x00006d68 03028e07 00c80f00 23722612 0f000000 ........#r&.....
+  0x00006d78 1e000000 00e40f04 23721613 19000080 ........#r......
+  0x00006d88 16000000 00e40f04 23721812 0c000000 ........#r......
+  0x00006d98 23000000 00e48f0c 23720213 0c000000 #.......#r......
+  0x00006da8 02000000 00e40f04 23720c12 0e000000 ........#r......
+  0x00006db8 25000000 00e40f00 23722313 0d000080 %.......#r#.....
+  0x00006dc8 18000000 00c40f00 23720212 0d000000 ........#r......
+  0x00006dd8 02000000 00e40f04 23720713 0f000080 ........#r......
+  0x00006de8 0c000000 00e40f04 23721812 14000000 ........#r......
+  0x00006df8 27000000 00e24f08 81790c28 06180000 '.....O..y.(....
+  0x00006e08 001b1e0c 00a20e00 23721f13 14000000 ........#r......
+  0x00006e18 1f000000 00c60f00 81790e2c 06000000 .........y.,....
+  0x00006e28 001b1e0c 00a20e00 23722513 15000080 ........#r%.....
+  0x00006e38 18000000 00e40f0c 23722a12 15000000 ........#r*.....
+  0x00006e48 1f000000 00e20f04 81791828 06980000 .........y.(....
+  0x00006e58 001b1e0c 00e80e00 81791428 06580000 .........y.(.X..
+  0x00006e68 001b1e0c 00620f00 23721e12 1a000000 .....b..#r......
+  0x00006e78 21000000 00e40f09 23721a13 1a000000 !.......#r......
+  0x00006e88 1d000000 00c40f00 23721d13 1b000080 ........#r......
+  0x00006e98 1e000000 00e40f08 81791e28 06d80000 .........y.(....
+  0x00006ea8 001b1e0c 00220f00 23721b12 1b000000 ....."..#r......
+  0x00006eb8 1a000000 00e40f00 23721c0c 0e000000 ........#r......
+  0x00006ec8 1c000000 00e44f0c 2372200c 0f000000 ......O.#r .....
+  0x00006ed8 20000000 00e40f08 23721a0d 0f000000  .......#r......
+  0x00006ee8 1c010000 00e40f04 23721c0d 0e000000 ........#r......
+  0x00006ef8 20000000 00c40f00 2372120e 18000000  .......#r......
+  0x00006f08 09000000 00e28f04 81790c28 06180100 .........y.(....
+  0x00006f18 001b1e0c 00a20e00 2372060e 14000000 ........#r......
+  0x00006f28 06000000 00e40f0e 2372240f 14000000 ........#r$.....
+  0x00006f38 24000000 00e40f04 2372170f 18000000 $.......#r......
+  0x00006f48 17000000 00e40f04 2372180f 19000080 ........#r......
+  0x00006f58 12000000 00e40f04 2372060f 15000080 ........#r......
+  0x00006f68 06000000 00e20f08 81791228 06580100 .........y.(.X..
+  0x00006f78 001b1e0c 00e20e00 2372090e 15000000 ........#r......
+  0x00006f88 24000000 00c60f00 81791428 06980100 $........y.(....
+  0x00006f98 001b1e0c 00620f00 2372190e 19000000 .....b..#r......
+  0x00006fa8 17000000 00e40f04 2372200e 1e000000 ........#r .....
+  0x00006fb8 16000000 00e40f0d 81791628 06d80100 .........y.(....
+  0x00006fc8 001b1e0c 00220f00 2372220f 1e000000 ....."..#r".....
+  0x00006fd8 22000000 00e40f04 23721e0e 0c000000 ".......#r......
+  0x00006fe8 23000000 00e44f08 2372210f 0c000000 #.....O.#r!.....
+  0x00006ff8 02000000 00c40f00 23720c0f 0d000080 ........#r......
+  0x00007008 1e000000 00e40f04 2372020f 1f000080 ........#r......
+  0x00007018 20000000 00e40f04 23721e0e 12000000  .......#r......
+  0x00007028 07000000 00e48f0c 2372240f 12000000 ........#r$.....
+  0x00007038 26000000 00e40f04 2372120e 14000000 &.......#r......
+  0x00007048 25000000 00e40f0a 2372140f 14000000 %.......#r......
+  0x00007058 2a000000 00c40f00 25762a00 00580000 *.......%v*..X..
+  0x00007068 03028e07 00c80f00 2372200e 1f000000 ........#r .....
+  0x00007078 22000000 00e40f04 2372220e 0d000000 ".......#r".....
+  0x00007088 21000000 00e40f04 2372070f 13000080 !.......#r......
+  0x00007098 1e000000 00e40f0c 2372240e 13000000 ........#r$.....
+  0x000070a8 24000000 00e20f04 81791e28 06600000 $........y.(.`..
+  0x000070b8 001b1e0c 00a20e00 23720d0f 15000080 ........#r......
+  0x000070c8 12000000 00e40f08 2372000e 15000000 ........#r......
+  0x000070d8 14000000 00e20f04 8179122a 06000000 .........y.*....
+  0x000070e8 001b1e0c 00e20e00 2372260e 16000000 ........#r&.....
+  0x000070f8 1d000000 00c40f01 2372160f 16000000 ........#r......
+  0x00007108 1b000000 00e20f04 81791428 06200000 .........y.(. ..
+  0x00007118 001b1e0c 00e20e00 23721b0f 17000080 ........#r......
+  0x00007128 26000000 00e40f08 2372260e 17000000 &.......#r&.....
+  0x00007138 16000000 00e40f00 81790e28 06a00000 .........y.(....
+  0x00007148 001b1e0c 00280f00 81791628 06e00000 .....(...y.(....
+  0x00007158 001b1e0c 00620f00 23721a14 12000000 .....b..#r......
+  0x00007168 1a000000 00c48f00 23721c14 13000000 ........#r......
+  0x00007178 1c000000 00e40f08 23721412 1e000000 ........#r......
+  0x00007188 06000000 00e44f0c 23721e13 1e000000 ......O.#r......
+  0x00007198 09000000 00e40f00 23720915 12000000 ........#r......
+  0x000071a8 1c000000 00e40f04 23720615 13000000 ........#r......
+  0x000071b8 1a010000 00e40f00 23721c12 0e000000 ........#r......
+  0x000071c8 18000000 00c40f01 23721a13 1f000080 ........#r......
+  0x000071d8 14000000 00e40f0c 23720e13 0e000000 ........#r......
+  0x000071e8 19000000 00e20f04 81791428 06200100 .........y.(. ..
+  0x000071f8 001b1e0c 00a20e00 23721f12 1f000000 ........#r......
+  0x00007208 1e000000 00e40f04 23721e12 16000000 ........#r......
+  0x00007218 02000000 00e20f0a 81791828 06600100 .........y.(.`..
+  0x00007228 001b1e0c 00e20e00 23722013 16000000 ........#r .....
+  0x00007238 20000000 00e40f04 23720213 0f000080  .......#r......
+  0x00007248 1c000000 00c40f00 23721c12 0f000000 ........#r......
+  0x00007258 0e000000 00e40f04 81790e28 06a00100 .........y.(....
+  0x00007268 001b1e0c 00220f00 23721d13 17000080 ....."..#r......
+  0x00007278 1e000000 00e40f0c 23721e12 17000000 ........#r......
+  0x00007288 20000000 00e40f04 81791628 06e00100  ........y.(....
+  0x00007298 001b1e0c 00620f00 23720c12 14000000 .....b..#r......
+  0x000072a8 0c000000 00e44f08 23722213 14000000 ......O.#r".....
+  0x000072b8 22000000 00c40f00 23721412 18000000 ".......#r......
+  0x000072c8 07000000 00e48f08 23720713 15000080 ........#r......
+  0x000072d8 0c000000 00e40f04 23722013 18000000 ........#r .....
+  0x000072e8 24000000 00e40f00 25762408 00580000 $.......%v$..X..
+  0x000072f8 03028e07 00c80f00 23720c12 0e000000 ........#r......
+  0x00007308 0d000000 00e40f0d 23720013 0e000000 ........#r......
+  0x00007318 00000000 00e40f04 23721812 15000000 ........#r......
+  0x00007328 22000000 00e40f04 23720812 16000000 ".......#r......
+  0x00007338 1b000000 00e40f0a 23722213 16000000 ........#r".....
+  0x00007348 26000000 00e40f04 23722113 19000080 &.......#r!.....
+  0x00007358 14000000 00c40f00 23722012 19000000 ........#r .....
+  0x00007368 20000000 00e20f04 81791428 06680000  ........y.(.h..
+  0x00007378 001b1e0c 00a20e00 23721913 0f000080 ........#r......
+  0x00007388 0c000000 00e40f0c 23720012 0f000000 ........#r......
+  0x00007398 00000000 00e20f04 81790c24 06000000 .........y.$....
+  0x000073a8 001b1e0c 00a20e00 23721b13 17000080 ........#r......
+  0x000073b8 08000000 00e40f08 23722212 17000000 ........#r".....
+  0x000073c8 22000000 00e20f00 81790e28 06280000 "........y.(.(..
+  0x000073d8 001b1e0c 00e80e00 81791228 06a80000 .........y.(....
+  0x000073e8 001b1e0c 00280f00 81791628 06e80000 .....(...y.(....
+  0x000073f8 001b1e0c 00620f00 2372230d 14000000 .....b..#r#.....
+  0x00007408 1f000000 00c44f00 2372090e 0d000000 ......O.#r......
+  0x00007418 09000000 00e48f04 2372060e 0c000000 ........#r......
+  0x00007428 06000000 00e40f00 2372020c 12000000 ........#r......
+  0x00007438 02000000 00e40f0d 23721c0d 12000000 ........#r......
+  0x00007448 1c000000 00e40f00 23721f0f 0c000000 ........#r......
+  0x00007458 09000000 00e40f00 23721a0c 14000000 ........#r......
+  0x00007468 1a000000 00e20f00 81790828 06280100 .........y.(.(..
+  0x00007478 001b1e0c 00a20e00 2372020d 13000080 ........#r......
+  0x00007488 02000000 00c40f00 23721c0c 13000000 ........#r......
+  0x00007498 1c000000 00e40f04 2372060f 0d000000 ........#r......
+  0x000074a8 06010000 00e20f00 81791228 06680100 .........y.(.h..
+  0x000074b8 001b1e0c 00e20e00 2372140c 16000000 ........#r......
+  0x000074c8 1d000000 00c60f02 81790e28 06a80100 .........y.(....
+  0x000074d8 001b1e0c 00220f00 23721e0d 16000000 ....."..#r......
+  0x000074e8 1e000000 00e40f04 23721a0d 15000080 ........#r......
+  0x000074f8 1a000000 00e40f0c 2372230c 15000000 ........#r#.....
+  0x00007508 23000000 00e40f04 2372160d 17000080 #.......#r......
+  0x00007518 14000000 00e40f08 81791428 06e80100 .........y.(....
+  0x00007528 001b1e0c 00620f00 2372170c 17000000 .....b..#r......
+  0x00007538 1e000000 00c40f00 25762604 00580000 ........%v&..X..
+  0x00007548 03028e07 00c80f00 23721e0c 08000000 ........#r......
+  0x00007558 07000000 00e44f0c 2372180d 08000000 ......O.#r......
+  0x00007568 18000000 00e40f04 2372080c 12000000 ........#r......
+  0x00007578 21000000 00e48f0c 2372200d 12000000 !.......#r .....
+  0x00007588 20000000 00e40f04 2372120c 0e000000  .......#r......
+  0x00007598 19000000 00e40f01 2372070d 09000080 ........#r......
+  0x000075a8 1e000000 00c40f00 23720e0d 0e000000 ........#r......
+  0x000075b8 00000000 00e40f04 23721d0d 0f000080 ........#r......
+  0x000075c8 12000000 00e40f04 2372120c 14000000 ........#r......
+  0x000075d8 1b000000 00e40f0e 23721e0d 14000000 ........#r......
+  0x000075e8 22000000 00e40f04 2372180c 09000000 ".......#r......
+  0x000075f8 18000000 00e40f00 2372190d 13000080 ........#r......
+  0x00007608 08000000 00c40f00 2372000c 13000000 ........#r......
+  0x00007618 20000000 00e20f04 81790828 06300000  ........y.(.0..
+  0x00007628 001b1e0c 00a20e00 2372040c 0f000000 ........#r......
+  0x00007638 0e000000 00e40f04 23721b0d 15000080 ........#r......
+  0x00007648 12000000 00e20f08 81790e26 06000000 .........y.&....
+  0x00007658 001b1e0c 00a20e00 23721e0c 15000000 ........#r......
+  0x00007668 1e000000 00c60f00 81790c28 06700000 .........y.(.p..
+  0x00007678 001b1e0c 00e80e00 81791228 06b00000 .........y.(....
+  0x00007688 001b1e0c 00280f00 81791428 06f00000 .....(...y.(....
+  0x00007698 001b1e0c 00620f00 23720608 0e000000 .....b..#r......
+  0x000076a8 06000000 00e44f04 23721f08 0f000000 ......O.#r......
+  0x000076b8 1f000000 00c40f00 23721a0e 0c000000 ........#r......
+  0x000076c8 1a000000 00e48f0c 2372230f 0c000000 ........#r#.....
+  0x000076d8 23000000 00e40f04 2372080e 12000000 #.......#r......
+  0x000076e8 02000000 00e40f0d 2372020f 0d000080 ........#r......
+  0x000076f8 1a000000 00e40f0c 2372200f 12000000 ........#r .....
+  0x00007708 1c000000 00e40f00 23721a0e 0d000000 ........#r......
+  0x00007718 23000000 00c40f00 23720609 0f000000 #.......#r......
+  0x00007728 06010000 00e20f04 81790c28 06300100 .........y.(.0..
+  0x00007738 001b1e0c 00a20e00 23721f09 0e000000 ........#r......
+  0x00007748 1f000000 00e40f00 23721c0f 13000080 ........#r......
+  0x00007758 08000000 00e40f0c 81790828 06700100 .........y.(.p..
+  0x00007768 001b1e0c 00e20e00 2372160e 14000000 ........#r......
+  0x00007778 16000000 00e40f0e 2372170f 14000000 ........#r......
+  0x00007788 17000000 00e40f00 2372200e 13000000 ........#r .....
+  0x00007798 20000000 00c40f00 2372160f 15000080  .......#r......
+  0x000077a8 16000000 00e20f08 81791228 06b00100 .........y.(....
+  0x000077b8 001b1e0c 00220f00 2372170e 15000000 ....."..#r......
+  0x000077c8 17000000 00c60f00 81791428 06f00100 .........y.(....
+  0x000077d8 001b1e0c 00620f00 25763005 00580000 .....b..%v0..X..
+  0x000077e8 03028e07 00c80f00 2372220e 0c000000 ........#r".....
+  0x000077f8 07000000 00e44f0c 2372180f 0c000000 ......O.#r......
+  0x00007808 18000000 00e40f04 23720c0e 08000000 ........#r......
+  0x00007818 19000000 00e48f08 2372080f 08000000 ........#r......
+  0x00007828 00000000 00e40f04 2372000f 0d000080 ........#r......
+  0x00007838 22000000 00e40f04 2372070f 09000080 ".......#r......
+  0x00007848 0c000000 00c40f00 2372220e 09000000 ........#r".....
+  0x00007858 08000000 00e40f04 2372080e 12000000 ........#r......
+  0x00007868 1d000000 00e40f0d 2372040f 12000000 ........#r......
+  0x00007878 04000000 00e40f04 23720c0e 14000000 ........#r......
+  0x00007888 1b000000 00e40f0e 23721e0f 14000000 ........#r......
+  0x00007898 1e000000 00e40f00 2372180e 0d000000 ........#r......
+  0x000078a8 18000000 00c40f00 2372190f 13000080 ........#r......
+  0x000078b8 08000000 00e40f0c 2372140e 13000000 ........#r......
+  0x000078c8 04000000 00e20f00 81790830 06000000 .........y.0....
+  0x000078d8 001b1e0c 00a20e00 2372210f 15000080 ........#r!.....
+  0x000078e8 0c000000 00c60f00 81790428 06380000 .........y.(.8..
+  0x000078f8 001b1e0c 00a80e00 81790c28 06780000 .........y.(.x..
+  0x00007908 001b1e0c 00e20e00 2372150e 15000000 ........#r......
+  0x00007918 1e000000 00c60f00 81790e28 06b80000 .........y.(....
+  0x00007928 001b1e0c 00280f00 81791228 06f80000 .....(...y.(....
+  0x00007938 001b1e0c 00620f00 23720304 09000000 .....b..#r......
+  0x00007948 1f000000 00e44f04 23720604 08000000 ......O.#r......
+  0x00007958 06000000 00e40f00 23721a09 0c000000 ........#r......
+  0x00007968 1a000000 00e48f08 23720408 0c000000 ........#r......
+  0x00007978 02000000 00c40f00 23720305 08000000 ........#r......
+  0x00007988 03000000 00e40f04 23720205 09000000 ........#r......
+  0x00007998 06010000 00e40f00 23720508 0d000000 ........#r......
+  0x000079a8 1a000000 00e40f0c 23720608 0e000000 ........#r......
+  0x000079b8 1c000000 00e20f0d 81791a28 06380100 .........y.(.8..
+  0x000079c8 001b1e0c 00a20e00 23722009 0e000000 ........#r .....
+  0x000079d8 20000000 00e40f04 23720e08 12000000  .......#r......
+  0x000079e8 16000000 00e20f02 81791c28 06f80100 .........y.(....
+  0x000079f8 001b1e0c 00e20e00 23720409 0d000080 ........#r......
+  0x00007a08 04000000 00c40f00 23721209 12000000 ........#r......
+  0x00007a18 17000000 00e20f04 81790c28 06b80100 .........y.(....
+  0x00007a28 001b1e0c 00280f00 81791628 06780100 .....(...y.(.x..
+  0x00007a38 001b1e0c 00620f00 23720609 0f000080 .....b..#r......
+  0x00007a48 06000000 00e40f04 23720e09 13000080 ........#r......
+  0x00007a58 0e000000 00e20f00 8679000a 02000000 .........y......
+  0x00007a68 061b100c 00e80f00 86790010 04000000 .........y......
+  0x00007a78 061b100c 00e20f00 23720008 1a000000 ........#r......
+  0x00007a88 00000000 00c44f00 23721a09 1a000000 ......O.#r......
+  0x00007a98 18000000 00e40f04 23721509 1c000000 ........#r......
+  0x00007aa8 15000000 00e48f0c 23721c08 1c000000 ........#r......
+  0x00007ab8 21000000 00e40f04 23721409 0c000000 !.......#r......
+  0x00007ac8 14000000 00e40f09 23720c08 0c000000 ........#r......
+  0x00007ad8 19000000 00e40f04 23721808 16000000 ........#r......
+  0x00007ae8 07000000 00c40f02 23722209 16000000 ........#r".....
+  0x00007af8 22000000 00e40f04 23720708 0f000000 ".......#r......
+  0x00007b08 20000000 00e40f04 23720f08 13000000  .......#r......
+  0x00007b18 12000000 00e40f04 23721308 1b000000 ........#r......
+  0x00007b28 1a000000 00e40f0c 23721209 1b000080 ........#r......
+  0x00007b38 00000000 00e40f00 23721b08 17000000 ........#r......
+  0x00007b48 22000000 00c40f00 23721a09 17000080 ".......#r......
+  0x00007b58 18000000 00e20f04 8679002e 06000000 .........y......
+  0x00007b68 061b100c 00e20f00 23721708 0d000000 ........#r......
+  0x00007b78 14000000 00e40f0c 23721609 0d000080 ........#r......
+  0x00007b88 0c000000 00e20f04 8679002c 0e000000 .........y.,....
+  0x00007b98 061b100c 00e20f00 23721508 1d000000 ........#r......
+  0x00007ba8 15000000 00e40f08 23721409 1d000080 ........#r......
+  0x00007bb8 1c000000 00e20f00 8679002a 12000000 .........y.*....
+  0x00007bc8 061b100c 00e80f00 86790024 1a000000 .........y.$....
+  0x00007bd8 061b100c 00e80f00 86790026 16000000 .........y.&....
+  0x00007be8 061b100c 00e80f00 86790030 14000000 .........y.0....
+  0x00007bf8 061b100c 00e20f00 4d790000 00000000 ........My......
+  0x00007c08 00008003 00ea0f00 47790000 f0ffffff ........Gy......
+  0x00007c18 ffff8303 00c00f00 18790000 00000000 .........y......
   0x00007c28 00000000 00c00f00 18790000 00000000 .........y......
   0x00007c38 00000000 00c00f00 18790000 00000000 .........y......
   0x00007c48 00000000 00c00f00 18790000 00000000 .........y......
   0x00007c58 00000000 00c00f00 18790000 00000000 .........y......
   0x00007c68 00000000 00c00f00 18790000 00000000 .........y......
   0x00007c78 00000000 00c00f00 18790000 00000000 .........y......
   0x00007c88 00000000 00c00f00 18790000 00000000 .........y......
-  0x00007c98 00000000 00c00f00 027a0100 000a0000 .........z......
-  0x00007ca8 000f0000 00e40f00 027a0200 005e0000 .........z...^..
-  0x00007cb8 000f0000 00e20f00 b97a0600 00460000 .........z...F..
-  0x00007cc8 000a0000 00e20f00 027a0300 005f0000 .........z..._..
-  0x00007cd8 000f0000 00ca0f00 81790402 06080000 .........y......
-  0x00007ce8 00191e0c 00a80000 81790502 06000000 .........y......
-  0x00007cf8 00191e0c 00e20000 b97a0400 00000000 .........z......
-  0x00007d08 00080000 00e40f00 9978043f 01000000 .........x.?....
-  0x00007d18 04160108 00e20f00 19790000 00000000 .........y......
-  0x00007d28 00250000 00680e00 19790900 00000000 .%...h...y......
-  0x00007d38 00210000 00640e00 247a0000 00000000 .!...d..$z......
-  0x00007d48 09028e07 00ca2f00 197803ff 1f000000 ....../..x......
-  0x00007d58 00140100 00e41f00 12720700 04000000 .........r......
-  0x00007d68 fffc8e07 00e44f0c 10720b05 04000000 ......O..r......
-  0x00007d78 ffe0ff07 00e48f00 12720500 05000000 .........r......
-  0x00007d88 fffc8e07 00e40f04 0c720000 07000000 .........r......
-  0x00007d98 7052f003 00e40f04 12720600 0b000000 pR.......r......
-  0x00007da8 fffc8e07 00c40f00 0c720000 05000000 .........r......
-  0x00007db8 70527000 00c80f00 0c720000 06000000 pRp......r......
-  0x00007dc8 70527200 00e40f0c 0c7a0000 005c0000 pRr......z...\..
-  0x00007dd8 7060f003 00e40f00 0c720005 07000000 p`.......r......
-  0x00007de8 7052f200 00e40f00 0c7a0003 005d0000 pR.......z...]..
-  0x00007df8 0061f003 00e40f00 0c720005 06000000 .a.......r......
-  0x00007e08 7052f200 00e40f00 0c7c0009 04000000 pR.......|......
-  0x00007e18 7010700c 00c40f00 0c720007 06000000 p.p......r......
-  0x00007e28 7052f200 00c80f00 1c780000 00000000 pR.......x......
-  0x00007e38 70307000 00da0f00 4d890000 00000000 p0p.....M.......
-  0x00007e48 00008003 00ea0f00 117a0800 00580000 .........z...X..
-  0x00007e58 ff188007 00e40f04 027a0e00 005a0000 .........z...Z..
-  0x00007e68 000f0000 00e40f00 027a0f00 005b0000 .........z...[..
-  0x00007e78 000f0000 00e40f00 117a0900 00590000 .........z...Y..
-  0x00007e88 031c0f00 00c60f00 8179020e 06000000 .........y......
-  0x00007e98 001b1e0c 00a80e00 81791408 06000000 .........y......
-  0x00007ea8 001b1e0c 00a80e00 8179100e 06200000 .........y... ..
-  0x00007eb8 001b1e0c 00e80e00 81790a0e 06400000 .........y...@..
-  0x00007ec8 001b1e0c 00280f00 8179160e 06600000 .....(...y...`..
-  0x00007ed8 001b1e0c 00620f00 357400ff 08000000 .....b..5t......
-  0x00007ee8 ff010000 00c60f00 8179120e 06280000 .........y...(..
-  0x00007ef8 001b1e0c 006e0f00 25760c05 00580000 .....n..%v...X..
-  0x00007f08 00028e07 00c80f00 20721903 15000000 ........ r......
-  0x00007f18 00004000 00e44f04 20720403 14000000 ..@...O. r......
-  0x00007f28 00004000 00e40f00 20720315 11000000 ..@..... r......
-  0x00007f38 00004000 00e48f0c 20720514 11000000 ..@..... r......
-  0x00007f48 00004000 00e40f04 20721115 0b000000 ..@..... r......
-  0x00007f58 00004000 00e40f09 20721814 0b000000 ..@..... r......
-  0x00007f68 00004000 00c40f00 23721902 14000000 ..@.....#r......
-  0x00007f78 19080000 00e40f04 23720402 15000000 ........#r......
-  0x00007f88 04000000 00e40f00 23720214 10000000 ........#r......
-  0x00007f98 03080000 00e40f0c 23720515 10000000 ........#r......
-  0x00007fa8 05000000 00e40f04 23720314 0a000000 ........#r......
-  0x00007fb8 11080000 00e40f08 23721815 0a000000 ........#r......
-  0x00007fc8 18000000 00e20f04 8179100c 06000000 .........y......
-  0x00007fd8 001b1e0c 00a20e00 20721b15 17000000 ........ r......
-  0x00007fe8 00004000 00c60f02 81790a0e 06080000 ..@......y......
-  0x00007ff8 001b1e0c 00a20e00 20721a14 17000000 ........ r......
-  0x00008008 00004000 00e40f04 23721b14 16000000 ..@.....#r......
-  0x00008018 1b080000 00e40f08 23721a15 16000000 ........#r......
-  0x00008028 1a000000 00e40f00 8179140e 06480000 .........y...H..
-  0x00008038 001b1e0c 00e80e00 8179160e 06680000 .........y...h..
-  0x00008048 001b1e0c 00220f00 23721c0a 10000000 ....."..#r......
-  0x00008058 19000000 00c44f00 2372040a 11000000 ......O.#r......
-  0x00008068 04000000 00e40f08 23720a10 12000000 ........#r......
-  0x00008078 02000000 00e40f00 2372020b 11000000 ........#r......
-  0x00008088 1c010000 00e40f04 23720b0b 10000000 ........#r......
-  0x00008098 04000000 00e40f00 23720411 13000080 ........#r......
-  0x000080a8 0a000000 00e40f04 23720511 12000000 ........#r......
-  0x000080b8 05000000 00c40f00 23720a10 14000000 ........#r......
-  0x000080c8 03000000 00e48f0c 23721310 13000000 ........#r......
-  0x000080d8 05000000 00e40f00 23720311 15000080 ........#r......
-  0x000080e8 0a000000 00e40f04 23720511 14000000 ........#r......
-  0x000080f8 18000000 00e40f00 25761c07 00580000 ........%v...X..
-  0x00008108 00028e07 00c80f00 23721210 16000000 ........#r......
-  0x00008118 1b000000 00e20f0d 8179181c 06000000 .........y......
-  0x00008128 001b1e0c 00a20e00 23720a11 16000000 ........#r......
-  0x00008138 1a000000 00e40f04 23720510 15000000 ........#r......
-  0x00008148 05000000 00e20f04 81791a0e 06300000 .........y...0..
-  0x00008158 001b1e0c 00a20e00 23720711 17000080 ........#r......
-  0x00008168 12000000 00e40f08 23720a10 17000000 ........#r......
-  0x00008178 0a000000 00e20f00 8179140e 06100000 .........y......
-  0x00008188 001b1e0c 00e80e00 8179100e 06500000 .........y...P..
-  0x00008198 001b1e0c 00280f00 8179160e 06700000 .....(...y...p..
-  0x000081a8 001b1e0c 00620f00 25761e06 00580000 .....b..%v...X..
-  0x000081b8 00028e07 00c80f00 23720418 1a000000 ........#r......
-  0x000081c8 04000000 00e44f08 23721319 1a000000 ......O.#r......
-  0x000081d8 13000000 00e40f04 23720214 18000000 ........#r......
-  0x000081e8 02000000 00e48f04 23720b14 19000000 ........#r......
-  0x000081f8 0b000000 00e40f00 23721218 10000000 ........#r......
-  0x00008208 03000000 00e40f09 23720519 10000000 ........#r......
-  0x00008218 05000000 00c40f00 23720018 16000000 ........#r......
-  0x00008228 07000000 00e40f0e 23721619 16000000 ........#r......
-  0x00008238 0a000000 00e20f04 8179060e 06180000 .........y......
-  0x00008248 001b1e0c 00a20e00 23720319 11000080 ........#r......
-  0x00008258 12000000 00e40f00 23720215 19000000 ........#r......
-  0x00008268 02010000 00e40f04 23721118 11000000 ........#r......
-  0x00008278 05000000 00e40f00 23721515 18000000 ........#r......
-  0x00008288 0b000000 00c40f00 23720419 1b000080 ........#r......
-  0x00008298 04000000 00e20f04 81790a1e 06000000 .........y......
-  0x000082a8 001b1e0c 00a20e00 23720519 17000080 ........#r......
-  0x000082b8 00000000 00e40f00 23721b18 1b000000 ........#r......
-  0x000082c8 13000000 00e40f04 23720018 17000000 ........#r......
-  0x000082d8 16000000 00e20f00 8179120e 06380000 .........y...8..
-  0x000082e8 001b1e0c 00e80e00 8179160e 06580000 .........y...X..
-  0x000082f8 001b1e0c 00280f00 8179180e 06780000 .....(...y...x..
-  0x00008308 001b1e0c 00620f00 23721506 0b000000 .....b..#r......
-  0x00008318 15000000 00c44f00 23720206 0a000000 ......O.#r......
-  0x00008328 02000000 00e40f00 23721b0b 12000000 ........#r......
-  0x00008338 1b000000 00e48f0c 2372040a 12000000 ........#r......
-  0x00008348 04000000 00e40f04 2372110b 16000000 ........#r......
-  0x00008358 11000000 00e40f0d 2372160a 16000000 ........#r......
-  0x00008368 03000000 00e40f00 2372000b 18000000 ........#r......
-  0x00008378 00000000 00c40f02 2372180a 18000000 ........#r......
-  0x00008388 05000000 00e40f04 23721507 0a000000 ........#r......
-  0x00008398 15000000 00e40f04 23721407 0b000000 ........#r......
-  0x000083a8 02010000 00e40f00 2372070a 13000000 ........#r......
-  0x000083b8 1b000000 00e40f0c 2372060b 13000080 ........#r......
-  0x000083c8 04000000 00e40f00 2372110a 17000000 ........#r......
-  0x000083d8 11000000 00c40f00 2372100b 17000080 ........#r......
-  0x000083e8 16000000 00e40f04 2372030a 19000000 ........#r......
-  0x000083f8 00000000 00e40f08 2372020b 19000080 ........#r......
-  0x00008408 18000000 00e20f00 86790008 14000000 .........y......
-  0x00008418 061b100c 00e80f00 8679000c 06000000 .........y......
-  0x00008428 061b100c 00e80f00 8679001c 10000000 .........y......
-  0x00008438 061b100c 00e80f00 8679001e 02000000 .........y......
-  0x00008448 061b100c 00e20f00 4d790000 00000000 ........My......
-  0x00008458 00008003 00ea0f00 47790000 f0ffffff ........Gy......
-  0x00008468 ffff8303 00c00f00 18790000 00000000 .........y......
-  0x00008478 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008488 00000000 00c00f00 18790000 00000000 .........y......
+  0x00007c98 00000000 00c00f00 18790000 00000000 .........y......
+  0x00007ca8 00000000 00c00f00 18790000 00000000 .........y......
+  0x00007cb8 00000000 00c00f00 027a0100 000a0000 .........z......
+  0x00007cc8 000f0000 00e40f00 027a0200 005e0000 .........z...^..
+  0x00007cd8 000f0000 00e20f00 b97a0600 00460000 .........z...F..
+  0x00007ce8 000a0000 00e20f00 027a0300 005f0000 .........z..._..
+  0x00007cf8 000f0000 00ca0f00 81790402 06080000 .........y......
+  0x00007d08 00191e0c 00a80000 81790502 06000000 .........y......
+  0x00007d18 00191e0c 00e20000 b97a0400 00000000 .........z......
+  0x00007d28 00080000 00e40f00 9978043f 01000000 .........x.?....
+  0x00007d38 04160108 00e20f00 19790000 00000000 .........y......
+  0x00007d48 00250000 00680e00 19790900 00000000 .%...h...y......
+  0x00007d58 00210000 00640e00 247a0000 00000000 .!...d..$z......
+  0x00007d68 09028e07 00ca2f00 197803ff 1f000000 ....../..x......
+  0x00007d78 00140100 00e41f00 12720700 04000000 .........r......
+  0x00007d88 fffc8e07 00e44f0c 10720b05 04000000 ......O..r......
+  0x00007d98 ffe0ff07 00e48f00 12720500 05000000 .........r......
+  0x00007da8 fffc8e07 00e40f04 0c720000 07000000 .........r......
+  0x00007db8 7052f003 00e40f04 12720600 0b000000 pR.......r......
+  0x00007dc8 fffc8e07 00c40f00 0c720000 05000000 .........r......
+  0x00007dd8 70527000 00c80f00 0c720000 06000000 pRp......r......
+  0x00007de8 70527200 00e40f0c 0c7a0000 005c0000 pRr......z...\..
+  0x00007df8 7060f003 00e40f00 0c720005 07000000 p`.......r......
+  0x00007e08 7052f200 00e40f00 0c7a0003 005d0000 pR.......z...]..
+  0x00007e18 0061f003 00e40f00 0c720005 06000000 .a.......r......
+  0x00007e28 7052f200 00e40f00 0c7c0009 04000000 pR.......|......
+  0x00007e38 7010700c 00c40f00 0c720007 06000000 p.p......r......
+  0x00007e48 7052f200 00c80f00 1c780000 00000000 pR.......x......
+  0x00007e58 70307000 00da0f00 4d890000 00000000 p0p.....M.......
+  0x00007e68 00008003 00ea0f00 117a0800 00580000 .........z...X..
+  0x00007e78 ff188007 00e40f04 027a0e00 005a0000 .........z...Z..
+  0x00007e88 000f0000 00e40f00 027a0f00 005b0000 .........z...[..
+  0x00007e98 000f0000 00e40f00 117a0900 00590000 .........z...Y..
+  0x00007ea8 031c0f00 00c60f00 8179020e 06000000 .........y......
+  0x00007eb8 001b1e0c 00a80e00 81791408 06000000 .........y......
+  0x00007ec8 001b1e0c 00a80e00 8179100e 06200000 .........y... ..
+  0x00007ed8 001b1e0c 00e80e00 81790a0e 06400000 .........y...@..
+  0x00007ee8 001b1e0c 00280f00 8179160e 06600000 .....(...y...`..
+  0x00007ef8 001b1e0c 00620f00 357400ff 08000000 .....b..5t......
+  0x00007f08 ff010000 00c60f00 8179120e 06280000 .........y...(..
+  0x00007f18 001b1e0c 006e0f00 25760c05 00580000 .....n..%v...X..
+  0x00007f28 00028e07 00c80f00 20721903 15000000 ........ r......
+  0x00007f38 00004000 00e44f04 20720403 14000000 ..@...O. r......
+  0x00007f48 00004000 00e40f00 20720315 11000000 ..@..... r......
+  0x00007f58 00004000 00e48f0c 20720514 11000000 ..@..... r......
+  0x00007f68 00004000 00e40f04 20721115 0b000000 ..@..... r......
+  0x00007f78 00004000 00e40f09 20721814 0b000000 ..@..... r......
+  0x00007f88 00004000 00c40f00 23721902 14000000 ..@.....#r......
+  0x00007f98 19080000 00e40f04 23720402 15000000 ........#r......
+  0x00007fa8 04000000 00e40f00 23720214 10000000 ........#r......
+  0x00007fb8 03080000 00e40f0c 23720515 10000000 ........#r......
+  0x00007fc8 05000000 00e40f04 23720314 0a000000 ........#r......
+  0x00007fd8 11080000 00e40f08 23721815 0a000000 ........#r......
+  0x00007fe8 18000000 00e20f04 8179100c 06000000 .........y......
+  0x00007ff8 001b1e0c 00a20e00 20721b15 17000000 ........ r......
+  0x00008008 00004000 00c60f02 81790a0e 06080000 ..@......y......
+  0x00008018 001b1e0c 00a20e00 20721a14 17000000 ........ r......
+  0x00008028 00004000 00e40f04 23721b14 16000000 ..@.....#r......
+  0x00008038 1b080000 00e40f08 23721a15 16000000 ........#r......
+  0x00008048 1a000000 00e40f00 8179140e 06480000 .........y...H..
+  0x00008058 001b1e0c 00e80e00 8179160e 06680000 .........y...h..
+  0x00008068 001b1e0c 00220f00 23721c0a 10000000 ....."..#r......
+  0x00008078 19000000 00c44f00 2372040a 11000000 ......O.#r......
+  0x00008088 04000000 00e40f08 23720a10 12000000 ........#r......
+  0x00008098 02000000 00e40f00 2372020b 11000000 ........#r......
+  0x000080a8 1c010000 00e40f04 23720b0b 10000000 ........#r......
+  0x000080b8 04000000 00e40f00 23720411 13000080 ........#r......
+  0x000080c8 0a000000 00e40f04 23720511 12000000 ........#r......
+  0x000080d8 05000000 00c40f00 23720a10 14000000 ........#r......
+  0x000080e8 03000000 00e48f0c 23721310 13000000 ........#r......
+  0x000080f8 05000000 00e40f00 23720311 15000080 ........#r......
+  0x00008108 0a000000 00e40f04 23720511 14000000 ........#r......
+  0x00008118 18000000 00e40f00 25761c07 00580000 ........%v...X..
+  0x00008128 00028e07 00c80f00 23721210 16000000 ........#r......
+  0x00008138 1b000000 00e20f0d 8179181c 06000000 .........y......
+  0x00008148 001b1e0c 00a20e00 23720a11 16000000 ........#r......
+  0x00008158 1a000000 00e40f04 23720510 15000000 ........#r......
+  0x00008168 05000000 00e20f04 81791a0e 06300000 .........y...0..
+  0x00008178 001b1e0c 00a20e00 23720711 17000080 ........#r......
+  0x00008188 12000000 00e40f08 23720a10 17000000 ........#r......
+  0x00008198 0a000000 00e20f00 8179140e 06100000 .........y......
+  0x000081a8 001b1e0c 00e80e00 8179100e 06500000 .........y...P..
+  0x000081b8 001b1e0c 00280f00 8179160e 06700000 .....(...y...p..
+  0x000081c8 001b1e0c 00620f00 25761e06 00580000 .....b..%v...X..
+  0x000081d8 00028e07 00c80f00 23720418 1a000000 ........#r......
+  0x000081e8 04000000 00e44f08 23721319 1a000000 ......O.#r......
+  0x000081f8 13000000 00e40f04 23720214 18000000 ........#r......
+  0x00008208 02000000 00e48f04 23720b14 19000000 ........#r......
+  0x00008218 0b000000 00e40f00 23721218 10000000 ........#r......
+  0x00008228 03000000 00e40f09 23720519 10000000 ........#r......
+  0x00008238 05000000 00c40f00 23720018 16000000 ........#r......
+  0x00008248 07000000 00e40f0e 23721619 16000000 ........#r......
+  0x00008258 0a000000 00e20f04 8179060e 06180000 .........y......
+  0x00008268 001b1e0c 00a20e00 23720319 11000080 ........#r......
+  0x00008278 12000000 00e40f00 23720215 19000000 ........#r......
+  0x00008288 02010000 00e40f04 23721118 11000000 ........#r......
+  0x00008298 05000000 00e40f00 23721515 18000000 ........#r......
+  0x000082a8 0b000000 00c40f00 23720419 1b000080 ........#r......
+  0x000082b8 04000000 00e20f04 81790a1e 06000000 .........y......
+  0x000082c8 001b1e0c 00a20e00 23720519 17000080 ........#r......
+  0x000082d8 00000000 00e40f00 23721b18 1b000000 ........#r......
+  0x000082e8 13000000 00e40f04 23720018 17000000 ........#r......
+  0x000082f8 16000000 00e20f00 8179120e 06380000 .........y...8..
+  0x00008308 001b1e0c 00e80e00 8179160e 06580000 .........y...X..
+  0x00008318 001b1e0c 00280f00 8179180e 06780000 .....(...y...x..
+  0x00008328 001b1e0c 00620f00 23721506 0b000000 .....b..#r......
+  0x00008338 15000000 00c44f00 23720206 0a000000 ......O.#r......
+  0x00008348 02000000 00e40f00 23721b0b 12000000 ........#r......
+  0x00008358 1b000000 00e48f0c 2372040a 12000000 ........#r......
+  0x00008368 04000000 00e40f04 2372110b 16000000 ........#r......
+  0x00008378 11000000 00e40f0d 2372160a 16000000 ........#r......
+  0x00008388 03000000 00e40f00 2372000b 18000000 ........#r......
+  0x00008398 00000000 00c40f02 2372180a 18000000 ........#r......
+  0x000083a8 05000000 00e40f04 23721507 0a000000 ........#r......
+  0x000083b8 15000000 00e40f04 23721407 0b000000 ........#r......
+  0x000083c8 02010000 00e40f00 2372070a 13000000 ........#r......
+  0x000083d8 1b000000 00e40f0c 2372060b 13000080 ........#r......
+  0x000083e8 04000000 00e40f00 2372110a 17000000 ........#r......
+  0x000083f8 11000000 00c40f00 2372100b 17000080 ........#r......
+  0x00008408 16000000 00e40f04 2372030a 19000000 ........#r......
+  0x00008418 00000000 00e40f08 2372020b 19000080 ........#r......
+  0x00008428 18000000 00e20f00 86790008 14000000 .........y......
+  0x00008438 061b100c 00e80f00 8679000c 06000000 .........y......
+  0x00008448 061b100c 00e80f00 8679001c 10000000 .........y......
+  0x00008458 061b100c 00e80f00 8679001e 02000000 .........y......
+  0x00008468 061b100c 00e20f00 4d790000 00000000 ........My......
+  0x00008478 00008003 00ea0f00 47790000 f0ffffff ........Gy......
+  0x00008488 ffff8303 00c00f00 18790000 00000000 .........y......
   0x00008498 00000000 00c00f00 18790000 00000000 .........y......
   0x000084a8 00000000 00c00f00 18790000 00000000 .........y......
   0x000084b8 00000000 00c00f00 18790000 00000000 .........y......
   0x000084c8 00000000 00c00f00 18790000 00000000 .........y......
   0x000084d8 00000000 00c00f00 18790000 00000000 .........y......
   0x000084e8 00000000 00c00f00 18790000 00000000 .........y......
   0x000084f8 00000000 00c00f00 18790000 00000000 .........y......
   0x00008508 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008518 00000000 00c00f00 027a0100 000a0000 .........z......
-  0x00008528 000f0000 00e40f00 027a0300 005f0000 .........z..._..
-  0x00008538 000f0000 00e20f00 b97a0600 00460000 .........z...F..
-  0x00008548 000a0000 00e20f00 027a0200 005e0000 .........z...^..
-  0x00008558 000f0000 00ca0f00 81790302 06000000 .........y......
-  0x00008568 00191e0c 00a20e00 b97a0400 00000000 .........z......
-  0x00008578 00080000 00e40f00 9978043f 01000000 .........x.?....
-  0x00008588 04160108 00e20f00 19790000 00000000 .........y......
-  0x00008598 00250000 00280e00 19790700 00000000 .%...(...y......
-  0x000085a8 00210000 00240e00 247a0000 00000000 .!...$..$z......
-  0x000085b8 07028e07 00ca1f00 0c7a0000 005c0000 .........z...\..
-  0x000085c8 7060f003 00e40f00 197809ff 1f000000 p`.......x......
-  0x000085d8 00140100 00c80f00 0c7a0009 005d0000 .........z...]..
-  0x000085e8 0061f003 00c80f00 0c7c0007 04000000 .a.......|......
-  0x000085f8 70647008 00e40f00 12720500 03000000 pdp......r......
-  0x00008608 fffc8e07 00c84f00 0c720000 05000000 ......O..r......
-  0x00008618 70267000 00da0f00 4d090000 00000000 p&p.....M.......
-  0x00008628 00008003 00ea0f00 117a0200 00580000 .........z...X..
-  0x00008638 ff188007 00e20f04 357404ff 08000000 ........5t......
-  0x00008648 ff010000 00e20f00 027a1200 005a0000 .........z...Z..
-  0x00008658 000f0000 00e40f00 027a1300 005b0000 .........z...[..
-  0x00008668 000f0000 00e40f00 117a0300 00590000 .........z...Y..
-  0x00008678 091c0f00 00c60f00 81791012 06000000 .........y......
-  0x00008688 001b1e0c 00a80e00 81790e02 06000000 .........y......
-  0x00008698 001b1e0c 00a20e00 25760405 00580000 ........%v...X..
-  0x000086a8 04028e07 00c60f00 81790c12 06100000 .........y......
-  0x000086b8 001b1e0c 00e80e00 81790812 06080000 .........y......
-  0x000086c8 001b1e0c 00280f00 81790604 06000000 .....(...y......
-  0x000086d8 001b1e0c 00280f00 81790a12 06180000 .....(...y......
-  0x000086e8 001b1e0c 00620f00 20720010 0f000000 .....b.. r......
-  0x000086f8 00004000 00c44f00 20721511 0f000000 ..@...O. r......
-  0x00008708 00004000 00e40f00 2072140e 0d000000 ..@..... r......
-  0x00008718 00004000 00e48f08 20720d0f 0d000000 ..@..... r......
-  0x00008728 00004000 00e40f00 23720011 0e000000 ..@.....#r......
-  0x00008738 00000000 00e40f08 23721510 0e000000 ........#r......
-  0x00008748 15080000 00e40f00 2372140f 0c000000 ........#r......
-  0x00008758 14000000 00c40f00 23720d0e 0c000000 ........#r......
-  0x00008768 0d080000 00e40f00 23720c09 06000000 ........#r......
-  0x00008778 00000000 00e40f09 23720008 06000000 ........#r......
-  0x00008788 15000000 00e40f00 23721407 0a000000 ........#r......
-  0x00008798 14000000 00e40f0a 23720a06 0a000000 ........#r......
-  0x000087a8 0d000000 00e40f00 23720d08 07000000 ........#r......
-  0x000087b8 0c000000 00c40f00 23720c09 07000000 ........#r......
-  0x000087c8 00010000 00e40f00 23720906 0b000000 ........#r......
-  0x000087d8 14000000 00e40f08 23720807 0b000080 ........#r......
-  0x000087e8 0a000000 00e20f00 86790002 0c000000 .........y......
-  0x000087f8 061b100c 00e80f00 86790004 08000000 .........y......
-  0x00008808 061b100c 00e20f00 4d790000 00000000 ........My......
-  0x00008818 00008003 00ea0f00 47790000 f0ffffff ........Gy......
-  0x00008828 ffff8303 00c00f00 18790000 00000000 .........y......
-  0x00008838 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008848 00000000 00c00f00 18790000 00000000 .........y......
+  0x00008518 00000000 00c00f00 18790000 00000000 .........y......
+  0x00008528 00000000 00c00f00 18790000 00000000 .........y......
+  0x00008538 00000000 00c00f00 027a0100 000a0000 .........z......
+  0x00008548 000f0000 00e40f00 027a0300 005f0000 .........z..._..
+  0x00008558 000f0000 00e20f00 b97a0600 00460000 .........z...F..
+  0x00008568 000a0000 00e20f00 027a0200 005e0000 .........z...^..
+  0x00008578 000f0000 00ca0f00 81790302 06000000 .........y......
+  0x00008588 00191e0c 00a20e00 b97a0400 00000000 .........z......
+  0x00008598 00080000 00e40f00 9978043f 01000000 .........x.?....
+  0x000085a8 04160108 00e20f00 19790000 00000000 .........y......
+  0x000085b8 00250000 00280e00 19790700 00000000 .%...(...y......
+  0x000085c8 00210000 00240e00 247a0000 00000000 .!...$..$z......
+  0x000085d8 07028e07 00ca1f00 0c7a0000 005c0000 .........z...\..
+  0x000085e8 7060f003 00e40f00 197809ff 1f000000 p`.......x......
+  0x000085f8 00140100 00c80f00 0c7a0009 005d0000 .........z...]..
+  0x00008608 0061f003 00c80f00 0c7c0007 04000000 .a.......|......
+  0x00008618 70647008 00e40f00 12720500 03000000 pdp......r......
+  0x00008628 fffc8e07 00c84f00 0c720000 05000000 ......O..r......
+  0x00008638 70267000 00da0f00 4d090000 00000000 p&p.....M.......
+  0x00008648 00008003 00ea0f00 117a0200 00580000 .........z...X..
+  0x00008658 ff188007 00e20f04 357404ff 08000000 ........5t......
+  0x00008668 ff010000 00e20f00 027a1200 005a0000 .........z...Z..
+  0x00008678 000f0000 00e40f00 027a1300 005b0000 .........z...[..
+  0x00008688 000f0000 00e40f00 117a0300 00590000 .........z...Y..
+  0x00008698 091c0f00 00c60f00 81791012 06000000 .........y......
+  0x000086a8 001b1e0c 00a80e00 81790e02 06000000 .........y......
+  0x000086b8 001b1e0c 00a20e00 25760405 00580000 ........%v...X..
+  0x000086c8 04028e07 00c60f00 81790c12 06100000 .........y......
+  0x000086d8 001b1e0c 00e80e00 81790812 06080000 .........y......
+  0x000086e8 001b1e0c 00280f00 81790604 06000000 .....(...y......
+  0x000086f8 001b1e0c 00280f00 81790a12 06180000 .....(...y......
+  0x00008708 001b1e0c 00620f00 20720010 0f000000 .....b.. r......
+  0x00008718 00004000 00c44f00 20721511 0f000000 ..@...O. r......
+  0x00008728 00004000 00e40f00 2072140e 0d000000 ..@..... r......
+  0x00008738 00004000 00e48f08 20720d0f 0d000000 ..@..... r......
+  0x00008748 00004000 00e40f00 23720011 0e000000 ..@.....#r......
+  0x00008758 00000000 00e40f08 23721510 0e000000 ........#r......
+  0x00008768 15080000 00e40f00 2372140f 0c000000 ........#r......
+  0x00008778 14000000 00c40f00 23720d0e 0c000000 ........#r......
+  0x00008788 0d080000 00e40f00 23720c09 06000000 ........#r......
+  0x00008798 00000000 00e40f09 23720008 06000000 ........#r......
+  0x000087a8 15000000 00e40f00 23721407 0a000000 ........#r......
+  0x000087b8 14000000 00e40f0a 23720a06 0a000000 ........#r......
+  0x000087c8 0d000000 00e40f00 23720d08 07000000 ........#r......
+  0x000087d8 0c000000 00c40f00 23720c09 07000000 ........#r......
+  0x000087e8 00010000 00e40f00 23720906 0b000000 ........#r......
+  0x000087f8 14000000 00e40f08 23720807 0b000080 ........#r......
+  0x00008808 0a000000 00e20f00 86790002 0c000000 .........y......
+  0x00008818 061b100c 00e80f00 86790004 08000000 .........y......
+  0x00008828 061b100c 00e20f00 4d790000 00000000 ........My......
+  0x00008838 00008003 00ea0f00 47790000 f0ffffff ........Gy......
+  0x00008848 ffff8303 00c00f00 18790000 00000000 .........y......
   0x00008858 00000000 00c00f00 18790000 00000000 .........y......
   0x00008868 00000000 00c00f00 18790000 00000000 .........y......
   0x00008878 00000000 00c00f00 18790000 00000000 .........y......
   0x00008888 00000000 00c00f00 18790000 00000000 .........y......
   0x00008898 00000000 00c00f00 18790000 00000000 .........y......
   0x000088a8 00000000 00c00f00 18790000 00000000 .........y......
   0x000088b8 00000000 00c00f00 18790000 00000000 .........y......
   0x000088c8 00000000 00c00f00 18790000 00000000 .........y......
   0x000088d8 00000000 00c00f00 18790000 00000000 .........y......
   0x000088e8 00000000 00c00f00 18790000 00000000 .........y......
   0x000088f8 00000000 00c00f00 18790000 00000000 .........y......
   0x00008908 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008918 00000000 00c00f00 00000000 00000000 ................
-  0x00008928 00000000 00000000 00000000 00000000 ................
-  0x00008938 00000000 00000000 00000000 00000000 ................
+  0x00008918 00000000 00c00f00 18790000 00000000 .........y......
+  0x00008928 00000000 00c00f00 18790000 00000000 .........y......
+  0x00008938 00000000 00c00f00 00000000 00000000 ................
   0x00008948 00000000 00000000 00000000 00000000 ................
-  0x00008958 00000000 00000000 01000000 03000000 ................
+  0x00008958 00000000 00000000 00000000 00000000 ................
   0x00008968 00000000 00000000 00000000 00000000 ................
-  0x00008978 40000000 00000000 70030000 00000000 @.......p.......
-  0x00008988 00000000 00000000 01000000 00000000 ................
-  0x00008998 00000000 00000000 0b000000 03000000 ................
-  0x000089a8 00000000 00000000 00000000 00000000 ................
-  0x000089b8 b0030000 00000000 e1030000 00000000 ................
-  0x000089c8 00000000 00000000 01000000 00000000 ................
-  0x000089d8 00000000 00000000 13000000 02000000 ................
-  0x000089e8 00000000 00000000 00000000 00000000 ................
-  0x000089f8 98070000 00000000 38010000 00000000 ........8.......
-  0x00008a08 02000000 0a000000 08000000 00000000 ................
-  0x00008a18 18000000 00000000 15030000 01000000 ................
-  0x00008a28 00000000 00000000 00000000 00000000 ................
-  0x00008a38 d0080000 00000000 50010000 00000000 ........P.......
-  0x00008a48 00000000 00000000 01000000 00000000 ................
-  0x00008a58 00000000 00000000 29000000 00000070 ........)......p
-  0x00008a68 00000000 00000000 00000000 00000000 ................
-  0x00008a78 200a0000 00000000 90000000 00000000  ...............
-  0x00008a88 03000000 00000000 04000000 00000000 ................
-  0x00008a98 00000000 00000000 5d000000 00000070 ........]......p
-  0x00008aa8 40000000 00000000 00000000 00000000 @...............
-  0x00008ab8 b00a0000 00000000 6c000000 00000000 ........l.......
-  0x00008ac8 03000000 0f000000 04000000 00000000 ................
-  0x00008ad8 00000000 00000000 51010000 00000070 ........Q......p
-  0x00008ae8 40000000 00000000 00000000 00000000 @...............
-  0x00008af8 1c0b0000 00000000 6c000000 00000000 ........l.......
-  0x00008b08 03000000 10000000 04000000 00000000 ................
-  0x00008b18 00000000 00000000 49020000 00000070 ........I......p
-  0x00008b28 40000000 00000000 00000000 00000000 @...............
-  0x00008b38 880b0000 00000000 6c000000 00000000 ........l.......
-  0x00008b48 03000000 11000000 04000000 00000000 ................
-  0x00008b58 00000000 00000000 45030000 01000070 ........E......p
-  0x00008b68 00000000 00000000 00000000 00000000 ................
-  0x00008b78 f40b0000 00000000 20000000 00000000 ........ .......
-  0x00008b88 03000000 00000000 04000000 00000000 ................
-  0x00008b98 08000000 00000000 61030000 0b000070 ........a......p
-  0x00008ba8 00000000 00000000 00000000 00000000 ................
-  0x00008bb8 180c0000 00000000 10000000 00000000 ................
-  0x00008bc8 00000000 00000000 08000000 00000000 ................
-  0x00008bd8 08000000 00000000 22030000 09000000 ........".......
-  0x00008be8 40000000 00000000 00000000 00000000 @...............
-  0x00008bf8 280c0000 00000000 30000000 00000000 (.......0.......
-  0x00008c08 03000000 04000000 08000000 00000000 ................
-  0x00008c18 10000000 00000000 bb000000 01000000 ................
-  0x00008c28 42000000 00000000 00000000 00000000 B...............
-  0x00008c38 580c0000 00000000 80010000 00000000 X...............
-  0x00008c48 00000000 0f000000 04000000 00000000 ................
-  0x00008c58 00000000 00000000 b1010000 01000000 ................
-  0x00008c68 42000000 00000000 00000000 00000000 B...............
-  0x00008c78 d80d0000 00000000 80010000 00000000 ................
-  0x00008c88 00000000 10000000 04000000 00000000 ................
-  0x00008c98 00000000 00000000 a9020000 01000000 ................
-  0x00008ca8 42000000 00000000 00000000 00000000 B...............
-  0x00008cb8 580f0000 00000000 80010000 00000000 X...............
-  0x00008cc8 00000000 11000000 04000000 00000000 ................
-  0x00008cd8 00000000 00000000 32000000 01000000 ........2.......
-  0x00008ce8 06000000 00000000 00000000 00000000 ................
-  0x00008cf8 00110000 00000000 001a0000 00000000 ................
-  0x00008d08 03000000 0a000034 80000000 00000000 .......4........
-  0x00008d18 00000000 00000000 25010000 01000000 ........%.......
-  0x00008d28 06000000 00000000 00000000 00000000 ................
-  0x00008d38 002b0000 00000000 80080000 00000000 .+..............
-  0x00008d48 03000000 0b000022 80000000 00000000 ......."........
-  0x00008d58 00000000 00000000 1d020000 01000000 ................
-  0x00008d68 06000000 00000000 00000000 00000000 ................
-  0x00008d78 80330000 00000000 00040000 00000000 .3..............
-  0x00008d88 03000000 0c000018 80000000 00000000 ................
-  0x00008d98 00000000 00000000 06000000 05000000 ................
-  0x00008da8 003c0000 00000000 00000000 00000000 .<..............
-  0x00008db8 00000000 00000000 a8000000 00000000 ................
-  0x00008dc8 a8000000 00000000 08000000 00000000 ................
-  0x00008dd8 01000000 05000000 580c0000 00000000 ........X.......
-  0x00008de8 00000000 00000000 00000000 00000000 ................
-  0x00008df8 282b0000 00000000 282b0000 00000000 (+......(+......
-  0x00008e08 08000000 00000000 01000000 05000000 ................
-  0x00008e18 003c0000 00000000 00000000 00000000 .<..............
-  0x00008e28 00000000 00000000 a8000000 00000000 ................
-  0x00008e38 a8000000 00000000 08000000 00000000 ................
-  0x00008e48 01000101 58000000 481f0000 00000000 ....X...H.......
-  0x00008e58 451f0000 48000000 04000800 50000000 E...H.......P...
-  0x00008e68 00000000 00000000 11200000 00000000 ......... ......
-  0x00008e78 00000000 00000000 9e620000 00000000 .........b......
-  0x00008e88 00000000 00000000 50000000 00000000 ........P.......
-  0x00008e98 00000000 00000000 3c0a2f2f 0300f31e ........<.//....
-  0x00008ea8 0a2e7665 7273696f 6e20382e 340a2e74 ..version 8.4..t
-  0x00008eb8 61726765 7420736d 5f38300a 2e616464 arget sm_80..add
-  0x00008ec8 72657373 5f73697a 65203634 0a3100ff ress_size 64.1..
-  0x00008ed8 31697369 626c6520 2e656e74 7279205f 1isible .entry _
-  0x00008ee8 5a313961 6374696f 6e4f6e53 696e676c Z19actionOnSingl
-  0x00008ef8 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
-  0x00008f08 5f6d506d 280a2e70 6172616d 202e7536 _mPm(..param .u6
-  0x00008f18 34330013 115f3100 3f5f302c 3b00261f 43..._1.?_0,;.&.
-  0x00008f28 313b0027 1f323b00 27f30833 0a290a7b 1;.'.2;.'..3.).{
-  0x00008f38 0a2e7265 67202e70 72656420 25703c36 ..reg .pred %p<6
-  0x00008f48 3e3b1200 95663332 2025663c 34351200 >;...f32 %f<45..
-  0x00008f58 10621200 36723c38 1100f201 36342025 .b..6r<8....64 %
-  0x00008f68 72643c31 333e3b0a 0a0a6c64 8a00222e rd<13>;...ld..".
-  0x00008f78 7518004f 322c205b 9000193d 305d3b44 u..O2, [...=0];D
-  0x00008f88 001f3344 001c1f31 4400001f 3444001c ..3D...1D...4D..
-  0x00008f98 1f324400 001f3544 001c9133 5d3b0a6d .2D...5D...3];.m
-  0x00008fa8 6f762e75 3401a832 2c20256e 7469642e ov.u4..2, %ntid.
-  0x00008fb8 7816007c 332c2025 63746117 0044342c x..|3, %cta..D4,
-  0x00008fc8 20252c00 7161642e 6c6f2e73 18002335  %,.qad.lo.s..#5
-  0x00008fd8 2c340001 4f00f403 72343b0a 63767461 ,4..O...r4;.cvta
-  0x00008fe8 2e746f2e 676c6f62 616cab00 21362cb1 .to.global..!6,.
-  0x00008ff8 0001c400 041a0001 41004036 2c205b20 ........A.@6, [ 
-  0x00009008 00535d3b 0a6f72ce 0124312c 5a001136 .S];.or..$1,Z..6
-  0x00009018 5000432e 73363470 0012641c 00923b0a P.C.s64p..d...;.
-  0x00009028 73657470 2e676560 00357031 2c1c0073 setp.ge`.5p1,..s
-  0x00009038 64343b0a 7368725f 0013379b 00173132 d4;.shr_..7...12
-  0x00009048 00001900 3370322c d6002172 377a0003 ....3p2,..!r7z..
-  0x00009058 6c022333 2c1c0014 70320022 65717b00 l.#3,...p2."eq{.
-  0x00009068 25703496 00183132 0024352c 3700ff08 %p4...12.$5,7...
-  0x00009078 343b0a40 25703520 62726120 244c5f5f 4;.@%p5 bra $L__
-  0x00009088 4242305f 323b0a12 0104019a 002f6432 BB0_2;......./d2
-  0x00009098 31010511 381f0018 33310121 76320003 1...8...31.!v2..
-  0x000090a8 307b2566 e9003266 327d3b01 20385df1 0{%f..2f2};. 8].
-  0x000090b8 00146cf9 0214390b 0182333b 0a616464 ..l...9...3;.add
-  0x000090c8 2e731700 3631302c 76001f39 57000300 .s..610,v..9W...
-  0x000090d8 cb002366 36570010 31fa0233 6d756c74 ..#f6W..1..3mult
-  0x000090e8 03005700 02780018 35170001 57002166 ..W..x..5...W.!f
-  0x000090f8 32390054 3b0a7375 62180025 312c3500 29.T;.sub..%1,5.
-  0x00009108 1f30c500 04013600 243133c7 00232b38 .0....6.$13..#+8
-  0x00009118 71004577 696465ef 0122312c 11021a38 q.Ewide.."1,...8
-  0x00009128 ce00003c 0004ce00 2f313161 00041136 ...<..../11a...6
-  0x00009138 61001437 d1000043 0363666d 612e726e a..7...C.cfma.rn
-  0x00009148 a5001132 bd000388 00022d00 1831dd00 ...2......-..1..
-  0x00009158 223231a2 00010600 19371a00 15320f01 "21......7...2..
-  0x00009168 1c365500 15331201 0150012c 32322100 .6U..3...P.,22!.
-  0x00009178 17345600 0176001f 32e70104 12324100 .4V..v..2....2A.
-  0x00009188 15362201 3931365d 86000160 012d3235 .6".916]...`.-25
-  0x00009198 96011233 96011d36 97013533 312c3800 ...3...6..531,8.
-  0x000091a8 1f339801 041133bc 00163398 012c3234 .3....3...3..,24
-  0x000091b8 39011133 5a002633 32c30019 33390121 9..3Z.&32...39.!
-  0x000091c8 33371400 0f390100 2633389a 001c3556 37...9..&38...5V
-  0x000091d8 0007cf00 0255001b 38220027 34307800 .....U..8".'40x.
-  0x000091e8 0264001c 39230017 31d40101 23002832 .d..9#..1...#.(2
-  0x000091f8 34020135 34322cfa 011032e4 031b7402 4..542,...2...t.
-  0x00009208 0103fc02 342c207b 2d003c34 317d6500 ....4, {-.<41}e.
-  0x00009218 1733e000 01ab0029 34306500 26342c26 .3.....)40e.&4,&
-  0x00009228 011f3765 00051332 6500012d 00653433 ..7e...2e..-.e43
-  0x00009238 7d3b0a0a 3704903a 0a726574 3b0a0a7d };..7..:.ret;..}
-  0x00009248 35081f2e 3408084f 446f7562 34081c0e 5...4..ODoub4...
-  0x00009258 33000e34 080f3b00 241f313b 00271f32 3..4..;.$.1;.'.2
-  0x00009268 3b00270f 3408012c 31373508 3c313631 ;.'.4..,175.<161
-  0x00009278 36082d31 3237082f 32303708 060e9300 6.-127./207.....
-  0x00009288 0f37082b 0e44000f 37081f0e 44000f37 .7.+.D..7...D..7
-  0x00009298 081f0e44 000f3708 091f3421 08031f35 ...D..7...4!...5
-  0x000092a8 4e08021f 36370804 15374c07 1634e707 N...67...7L..4..
-  0x000092b8 0f370814 233634fb 05043808 30637674 .7..#64...8.0cvt
-  0x000092c8 6f00031a 00023907 1c374f08 0172001f o.....9..7O..r..
-  0x000092d8 38490000 13384900 2d2b384b 0021392c 8I...8I.-+8K.!9,
-  0x000092e8 2100074b 0015324b 00193990 0617398f !..K..2K..9...9.
-  0x000092f8 061c3847 00037b07 17394800 15334800 ..8G..{..9H..3H.
-  0x00009308 23313068 08136ef4 06267031 1c000c1b #10h..n..&p1....
-  0x00009318 00067f00 69323b0a 616e64b6 081131bb ....i2;.and...1.
-  0x00009328 080c3300 15343300 19333300 09b7080a ..3..43..33.....
-  0x00009338 33002436 2c35010a 66002337 2c1d002c 3.$6,5..f.#7,..,
-  0x00009348 70353300 15383300 0a660023 392c1d00 p53..83..f.#9,..
-  0x00009358 2c703733 00021601 1e323400 01f30702 ,p73.....24.....
-  0x00009368 1f002f70 39000a03 044d0022 6c746301 ../p9....M."ltc.
-  0x00009378 1170f005 031d000a 010a0241 08163502 .p.........A..5.
-  0x00009388 0a226c74 1a001170 820701a2 023a7231 ."lt...p.....:r1
-  0x00009398 31820024 342c2000 2a703104 01363135 1..$4, .*p1..615
-  0x000093a8 2c210065 313b0a6e 6f741b00 11361500 ,!.e1;.not...6..
-  0x000093b8 1135060a 27313607 0a1f3107 0a082f31 .5..'16...1.../1
-  0x000093c8 30080a0b 2f313109 0a162a31 310a0a2f 0.../11...*11../
-  0x000093d8 31320b0a 0427332c 7a002f31 320d0a11 12...'3,z./12...
-  0x000093e8 2f335d0d 0a5a2f31 310e0a03 1f340e0a /3]..Z/11....4..
-  0x000093f8 0328352c d1001f34 6300041a 360f0a1f .(5,...4c...6...
-  0x00009408 350f0a2d 06e10002 0f0a0655 080f7f00 5..-.......U....
-  0x00009418 0103180a 1634e200 2f3136e3 00011336 .....4../16....6
-  0x00009428 17030be3 0001c303 05e3001f 36640004 ............6d..
-  0x00009438 11376400 14386400 1d37b909 01c30003 .7d..8d..7......
-  0x00009448 8b001437 9f0a06e3 00025b09 02a20a28 ...7......[....(
-  0x00009458 3238e300 02ed0802 40001f33 33020411 28......@..33...
-  0x00009468 33380026 3335e300 2f3234e3 00011338 38.&35../24....8
-  0x00009478 350e0be3 0028392c e3001f38 64000411 5....(9,...8d...
-  0x00009488 38640014 3964001c 39e30002 b409038b 8d..9d..9.......
-  0x00009498 00022d00 1833e300 03bc0914 353e0a07 ..-..3......5>..
-  0x000094a8 1a001634 ba0b0b9b 0a253435 f2020119 ...4.....%45....
-  0x000094b8 022c3434 21001c36 770a1d34 44001737 .,44!..6w..4D..7
-  0x000094c8 3f020246 000c3c0c 2734389f 01010c00 ?..F..<.'48.....
-  0x000094d8 2c343723 001739a2 01026900 0c260b27 ,47#..9...i..&.'
-  0x000094e8 35300201 012f001f 34f10d05 01d20016 50.../..4.......
-  0x000094f8 35410448 2b33325d 13011135 f8001e35 5A.H+32]...5...5
-  0x00009508 eb032235 363a000d ec033635 372c3800 .."56:....657,8.
-  0x00009518 0fa70204 1135db00 26353977 003b3430 .....5..&59w.;40
-  0x00009528 5dc50011 365b0026 35382e01 1935490c ]...6[.&58...5I.
-  0x00009538 22363344 000e8d03 3536342c 40001f36 "63D....564,@..6
-  0x00009548 38050411 36a00027 36368200 1d388200 8...6..'66...8..
-  0x00009558 015c0026 36356a01 28363482 00223730 .\.&65j.(64.."70
-  0x00009568 44000e2c 03353731 2c40001f 37f10404 D..,.571,@..7...
-  0x00009578 1137a000 1737f104 2c353682 0011375c .7...7..,56...7\
-  0x00009588 00022a00 02cb0219 37910422 37374400 ..*.....7.."77D.
-  0x00009598 0ecb0226 37389f01 0ccc0226 3739d401 ...&78.....&79..
-  0x000095a8 0261000c 41022738 307c0102 64000c67 .a..A.'80|..d..g
-  0x000095b8 0d273831 7f010146 002c3830 23001732 .'81...F.,80#..2
-  0x000095c8 4001014c 002c3831 23001733 43010169 @..L.,81#..3C..i
-  0x000095d8 001c382e 0f273834 0401016f 001f38d4 ..8..'84...o..8.
-  0x000095e8 01041138 6a001738 d4013836 345d1501 ...8j..8..864]..
-  0x000095f8 12383f00 01270009 cd022239 303a000d .8?..'...."90:..
-  0x00009608 cd023539 312c3800 1f39c901 0411399b ..591,8..9....9.
-  0x00009618 001739c9 013b3732 5dc50011 395b0026 ..9..;72]...9[.&
-  0x00009628 39322e01 1939c901 22393744 000ecd02 92...9.."97D....
-  0x00009638 3639382c 40001f37 82000403 5a071630 698,@..7....Z..0
-  0x00009648 83001d38 50032131 305e0026 39396c01 ...8P.!10^.&99l.
-  0x00009658 28393884 00213130 6a013e31 3030d102 (98..!10j.>100..
-  0x00009668 46313035 2c44002f 31306207 05223036 F105,D./10b.."06
-  0x00009678 20001737 8a000d58 031131e2 05042d00  ..7...X..1...-.
-  0x00009688 02d80229 31309101 12313208 3e313037 ...)10...12.>107
-  0x00009698 db023631 3132ae01 0cdc0236 313133e4 ..6112.....6113.
-  0x000096a8 0122362c 2f000d24 0017348e 01123725 ."6,/..$..4...7%
-  0x000096b8 001d3325 00173593 01034a00 1d342500 ..3%..5...J..4%.
-  0x000096c8 17365401 02c9002d 31352500 18375801 .6T....-15%..7X.
-  0x000096d8 0370001d 36260018 38150112 3926000f .p..6&..8...9&..
-  0x000096e8 f1010422 31312000 1732f201 3939365d ..."11 ..2..996]
-  0x000096f8 26010245 06032a00 1a351b00 13343e00 &..E..*..5...4>.
-  0x00009708 0df00212 317d1104 3d001f32 e8010502 ....1}..=..2....
-  0x00009718 c0112731 32e8014c 3130345d d4000287 ..'12..L104]....
-  0x00009728 12042e00 0334000a 8c000251 083e3132 .....4.....Q.>12
-  0x00009738 37fb0213 31e81103 46002f33 318d0004 7...1...F./31...
-  0x00009748 03871118 335a090e ec131231 9412032e ....3Z.....1....
-  0x00009758 00038701 2a33328d 0013384a 000f0203 ....*32...8J....
-  0x00009768 00039301 0446000f 9e080412 31a21237 .....F......1..7
-  0x00009778 3134318d 001e328d 03026b08 032e0003 141...2...k.....
-  0x00009788 03030be7 02037308 2f343103 0300046e ......s./41....n
-  0x00009798 081f3004 03022734 37fb0102 2a000d6a ..0...'47...*..j
-  0x000097a8 0812316b 08049c01 0206030d 6d081231 ..1k........m..1
-  0x000097b8 6e08049f 0102c201 0d700812 31710804 n........p..1q..
-  0x000097c8 5b010208 032d3439 26001831 5e010252 [....-49&..1^..R
-  0x000097d8 002d3530 26001832 1a01027f 002d3531 .-50&..2.....-51
-  0x000097e8 260008c5 09017100 293530af 01353534 &.....q.)50..554
-  0x000097f8 2c0c0a2f 34338213 05123382 13032e00 ,../43....3.....
-  0x00009808 4d313533 7d690017 35630701 69002a38 M153}i..5c..i.*8
-  0x00009818 34690026 362caa07 0feb1306 14356900 4i.&6,.......5i.
-  0x00009828 22362c56 000e6900 1837f204 1238c201 "6,V..i..7...8..
-  0x00009838 0a830203 9107033f 052f3131 6d000514 .......?./11m...
-  0x00009848 376d0002 30002e35 376d0018 395c0203 7m..0..57m..9\..
-  0x00009858 27001932 6d003836 302ca902 1f356d00 '..2m.860,...5m.
-  0x00009868 0513396d 00033000 263539c7 141f31c7 ..9m..0.&59...1.
-  0x00009878 140f1438 8412af54 7269706c 65476174 ...8...TripleGat
-  0x00009888 65c61408 0f320012 0ec5140f 3a001c1f e....2......:...
-  0x00009898 313a0026 1f323a00 260ff61c 021c31c2 1:.&.2:.&.....1.
-  0x000098a8 14363630 39b01402 c2142d32 34c2142f .6609.....-24../
-  0x000098b8 3332c214 021231f6 130f4001 160f3914 32....1...@...9.
-  0x000098c8 001f3243 001b1f31 0415010f 43001b1f ..2C...1....C...
-  0x000098d8 32430000 1f344300 1b2f335d 5b110523 2C...4C../3][..#
-  0x000098e8 352c2e12 06b0141f 38c61402 1f39f314 5,......8....9..
-  0x000098f8 032f3130 de140401 be080136 00247238 ./10.......6.$r8
-  0x00009908 e4132e6c 64db1400 41032d35 5d2f1421 ...ld...A.-5]/.!
-  0x00009918 322c2000 072f1425 312c5600 2f31320d 2, ../.%1,V./12.
-  0x00009928 15071f35 c4140001 11090a10 1517324e ...5..........2N
-  0x00009938 000a1a12 23382c9a 00023200 0b4a001d ....#8,...2..J..
-  0x00009948 340f1517 334a001f 34980000 14399800 4...3J..4....9..
-  0x00009958 2e313699 001d3516 1517344f 001a351c .16...5...4O..5.
-  0x00009968 1017309a 001d394b 0013363a 10074c00 ..0...9K..6:..L.
-  0x00009978 17354c00 1a364c00 1731ad15 0e4c0002 .5L..6L..1...L..
-  0x00009988 18002731 314c0017 364c001f 37881c01 ..'11L..6L..7...
-  0x00009998 0353001d 364d0015 38631305 4d001737 .S..6M..8c..M..7
-  0x000099a8 4d001f38 fc15022f 3131fd15 072f3131 M..8.../11.../11
-  0x000099b8 fe151f2f 3131ff15 201331cf 1f0f0016 .../11.. .1.....
-  0x000099c8 19049c1f 0c011601 39001f38 01160302 ........9..8....
-  0x000099d8 35001936 35000114 00023b00 2d313037 5..65.....;.-107
-  0x000099e8 00070801 1a373700 26332c3f 160d0b01 .....77.&3,?....
-  0x000099f8 053c142f 2572d315 081d3337 00020f01 .<./%r....37....
-  0x00009a08 0e420101 2902021f 0001f515 0b370002 .B..)........7..
-  0x00009a18 12010e45 01019609 021f003c 70313737 ...E.......<p177
-  0x00009a28 0001d209 1f724801 00017c14 021f003d .....rH...|....=
-  0x00009a38 70313937 00021401 0e4a0101 c90b021f p197.....J......
-  0x00009a48 003d7032 31370006 13010a4a 0101070c .=p217.....J....
-  0x00009a58 021f003d 70323337 00011301 1e321301 ...=p237.....2..
-  0x00009a68 01d50902 1f003d70 32353700 15383700 ......=p257..87.
-  0x00009a78 0a130101 8f1e021f 002d7032 13012533 .........-p2..%3
-  0x00009a88 3037000a 1301013b 0c021f00 2d703213 07.....;....-p2.
-  0x00009a98 01253332 37000a13 0101a60a 021f003d .%327..........=
-  0x00009aa8 70333137 00153437 000a1301 016c0a02 p317..47.....l..
-  0x00009ab8 1f003d70 33333700 0113011e 33dc0001 ..=p337.....3...
-  0x00009ac8 300c021f 002d7033 13012533 3837000b 0....-p3..%387..
-  0x00009ad8 dc002439 2c1f003c 70333737 00253430 ..$9,..<p377.%40
-  0x00009ae8 37000adc 0001d109 021f003d 70333937 7..........=p397
-  0x00009af8 00153237 000adc00 01131502 1f002d70 ..27..........-p
-  0x00009b08 34130101 030a2e72 34a50001 a20c021f 4......r4.......
-  0x00009b18 003d7034 33370015 3637000b a5002437 .=p437..67....$7
-  0x00009b28 2c1f003d 70343537 00153837 000ba500 ,..=p457..87....
-  0x00009b38 24392c1f 003c7034 37370001 830c2e72 $9,..<p477.....r
-  0x00009b48 356e0001 760c021f 003d7034 39370015 5n..v....=p497..
-  0x00009b58 3237000a 6e000161 0c021f00 3d703531 27..n..a....=p51
-  0x00009b68 370002d7 000f3700 0024352c 1f003e70 7.....7..$5,..>p
-  0x00009b78 3533bd1a 14336e1a 0abf1a01 170c041f 53...3n.........
-  0x00009b88 00296433 c01a0447 080dc01a 01320c03 .)d3...G.....2..
-  0x00009b98 5d1c2a31 39870024 382c2100 3a703536 ].*19..$8,!.:p56
-  0x00009ba8 1b002639 2c210019 35c11a01 c30b3170 ..&9,!..5.....1p
-  0x00009bb8 3539c11a 273630c1 1a1f32c1 1a091434 59..'60...2....4
-  0x00009bc8 c11a2f6c 64110f00 09a11a00 23100f46 ../ld.......#..F
-  0x00009bd8 00040184 012f6431 1119052f 31311219 ...../d1.../11..
-  0x00009be8 051e3512 190fc61a 062f375d c61a5b3f ..5....../7]..[?
-  0x00009bf8 342b3800 19061f31 0019051f 3500190a 4+8....1....5...
-  0x00009c08 010f0107 c61a0d00 19012406 048a0002 ..........$.....
-  0x00009c18 b20f0fc6 1a481f34 c61a0323 32304705 .....H.4...#20G.
-  0x00009c28 0ae30001 7c0005e3 001f3246 0104021c ....|.....2F....
-  0x00009c38 1005c61a 2c3231e3 00273331 27190fc6 ....,21..'31'...
-  0x00009c48 1a4e1f34 c61a0314 324e050b e3000062 .N.4....2N.....b
-  0x00009c58 0006e300 0f640005 1938c61a 2f3233c6 .....d...8../23.
-  0x00009c68 1a2d06e3 0002c61a 06fa100f 7f000102 .-..............
-  0x00009c78 5c122634 36e3002f 3332e300 0113348c \.&46../32....4.
-  0x00009c88 050be300 003e0006 e3000f25 1404023b .....>.....%...;
-  0x00009c98 121435a3 141d326f 1d02c411 038b0001 ..5...2o........
-  0x00009ca8 2d002834 34e30001 46050359 1b0ade11 -.(44...F..Y....
-  0x00009cb8 02951102 40001f35 7f000413 35341a06 ....@..5....54..
-  0x00009cc8 e3002f34 30e30001 13360106 0be30000 ../40....6......
-  0x00009cd8 560206e3 000f5d04 0402f410 1436ec13 V.....]......6..
-  0x00009ce8 1d326f1d 028b1a02 8b00022d 00283535 .2o........-.(55
-  0x00009cf8 e300021d 1901a805 38663631 e3000214 ........8f61....
-  0x00009d08 19024000 2f36357f 00040238 001738e3 ..@./65....8..8.
-  0x00009d18 000f6f04 01027809 1d36e300 00730106 ..o...x..6...s..
-  0x00009d28 e3000f6f 040402cb 1a1437c2 051d326f ...o......7...2o
-  0x00009d38 041137c3 00028b00 03f81a18 36e30002 ..7.........6...
-  0x00009d48 c41a2236 38470008 e30003be 1a014000 .."68G........@.
-  0x00009d58 1f376201 0402c81a 263739e3 002f3536 .7b.....&79../56
-  0x00009d68 e3000002 240a1c37 e30001e8 0305e300 ....$..7........
-  0x00009d78 0ff02805 02a81a14 38b5051d 336f0402 ..(.....8...3o..
-  0x00009d88 6b18028b 00243832 e91306e3 00353837 k....$82.....587
-  0x00009d98 2c571b29 38331a00 1f38521e 0616387e ,W.)83...8R...8~
-  0x00009da8 06015f00 1c385615 1839c805 1237881a .._..8V..9...7..
-  0x00009db8 0c230008 cb051436 a51a0a23 0017322b .#.....6...#..2+
-  0x00009dc8 0514387a 1a0a2300 1c33521e 1c393319 ..8z..#..3R..93.
-  0x00009dd8 2739348e 04123919 190c2300 01c80126 '94...9...#....&
-  0x00009de8 3335b104 2f393406 1b0202f1 03019109 35../94.........
-  0x00009df8 2c663916 01263937 f4030214 041c39ba ,f9..&97......9.
-  0x00009e08 16273938 54031431 181b0a23 00173957 .'98T..1...#..9W
-  0x00009e18 031430eb 1a092300 038f1903 b8021232 ..0...#........2
-  0x00009e28 c7190d24 001731bc 0222312c 37000d25 ...$..1.."1,7..%
-  0x00009e38 0017321e 02123325 000fab18 0505401b ..2...3%......@.
-  0x00009e48 06d0020b a41c0301 16032a00 0b980826 ..........*....&
-  0x00009e58 382ca81b 0a9b0838 30392c3d 000f3c08 8,.....809,=..<.
-  0x00009e68 0502db08 36313131 80000ead 1c03201b ....6111...... .
-  0x00009e78 042d0002 43081a30 81180153 03004900 .-..C..0...S..I.
-  0x00009e88 0e460803 151b0546 000fbd04 0404171b .F.....F........
-  0x00009e98 1731bf04 0fb61c00 03ae0826 31379e02 .1.........&17..
-  0x00009ea8 013d1b07 8c0002b7 0803411b 0aef0705 .=........A.....
-  0x00009eb8 c91a0246 000f8e07 0505121b 07f4070f ...F............
-  0x00009ec8 b81c0002 40032731 3295073a 3132338c ....@.'12..:123.
-  0x00009ed8 00133949 000e9807 050e1b03 46000f93 ..9I........F...
-  0x00009ee8 21040412 1b163335 0b02dc1b 0a8c0002 !.....35........
-  0x00009ef8 6903032d 00022a03 39313330 8c000175 i..-..*.9130...u
-  0x00009f08 0e04461b 0b1f1904 0d1b0346 000f7e05 ..F........F..~.
-  0x00009f18 0405111b 0780050f e81b0102 6d08032e ............m...
-  0x00009f28 00027103 39313337 8d0002b0 0803461b ..q.9137......F.
-  0x00009f38 0aeb0605 64180246 000fb408 0505111b ....d..F........
-  0x00009f48 07b6080e e81b05b3 1a273435 b6030a59 .........'45...Y
-  0x00009f58 0804b01a 2e343695 0604a61a 0346002f .....46......F./
-  0x00009f68 35308d00 04243532 321a068d 000fe81b 50...$522.......
-  0x00009f78 0002a704 032e0002 3c0601ce 1a088d00 ........<.......
-  0x00009f88 02f9192e 35333f06 283135f2 030c4206 ....53?.(15...B.
-  0x00009f98 04c61902 2b040369 000de804 283630cd ....+..i....(60.
-  0x00009fa8 03036c00 0dea0402 490504d0 0302f303 ..l.....I.......
-  0x00009fb8 1d36eb04 02542304 8d0302e8 1b2d3631 .6...T#......-61
-  0x00009fc8 26001833 90030272 001d3685 1f02db08 &..3...r..6.....
-  0x00009fd8 27313254 063d3136 33260018 35500303 '12T.=163&..5P..
-  0x00009fe8 72000d87 1f022d09 030d0302 5a063d31 r.....-.....Z.=1
-  0x00009ff8 36352600 17371003 03e0012d 36362600 65&..7.....-66&.
-  0x0000a008 1838cc02 0310010d 181d02dc 2304cf02 .8..........#...
-  0x0000a018 02f2021d 367c0128 37308b02 023d011d ....6|.(70...=..
-  0x0000a028 367c0128 37318e02 020d002d 37302600 6|.(71.....-70&.
-  0x0000a038 18324a02 0263012f 37319e02 04133720 .2J..c./71....7 
-  0x0000a048 0008a70d 3932385d 5c02027f 092f3137 ....928]\..../17
-  0x0000a058 69060002 cd062f31 37690600 02e60805 i...../17i......
-  0x0000a068 3d000f69 06050242 24273138 69062e31 =..i...B$'18i..1
-  0x0000a078 33c60402 dd232831 386a061a 376a0602 3....#(18j..7j..
-  0x0000a088 cb211231 70240b6a 06029909 0546000f .!.1p$.j.....F..
-  0x0000a098 6a060502 a0092731 386a062e 3134c604 j.....'18j..14..
-  0x0000a0a8 034e0927 3837b802 1a386b06 0334221f .N.'87...8k..4".
-  0x0000a0b8 386b0601 032b2203 46002f39 328d0004 8k...+".F./92...
-  0x0000a0c8 024b0927 31396b06 2e3135c6 0402e608 .K.'19k..15.....
-  0x0000a0d8 2831396c 062a3933 8d001339 4a000e6c (19l.*93...9J..l
-  0x0000a0e8 061232de 08054600 0f6c0604 1232e108 ..2...F..l...2..
-  0x0000a0f8 38323032 cf0f0dc6 041232fe 23273230 8202......2.#'20
-  0x0000a108 6d063832 30308d00 1232b822 2f32306d m.8200...2."/20m
-  0x0000a118 06001232 96080546 000f6d06 041232df ...2...F..m...2.
-  0x0000a128 08283230 6d061d36 86071232 120b032e .(20m..6...2....
-  0x0000a138 00027b03 2932306d 06123212 0b2f3230 ..{.)20m..2../20
-  0x0000a148 6d060012 32970804 46002f31 338d0004 m...2...F./13...
-  0x0000a158 02e10828 32316d06 1d37c102 1132b411 ...(21m..7...2..
-  0x0000a168 042e0002 bc033932 31348d00 0450110f ......9214...P..
-  0x0000a178 6d060012 32980804 46000f10 110602e2 m...2...F.......
-  0x0000a188 08283232 6d061d38 c1021132 cc0e042e .(22m..8...2....
-  0x0000a198 00026d06 3a323231 8d001337 4a000e6d ..m.:221...7J..m
-  0x0000a1a8 06283232 f6030c6d 06373232 392f0403 .(22...m.7229/..
-  0x0000a1b8 69000cf1 04383233 30d00303 6c001d39 i....8230...l..9
-  0x0000a1c8 26001831 d303024c 002d3330 26001832 &..1...L.-30&..2
-  0x0000a1d8 8f031238 26001d31 26001833 9203022c ...8&..1&..3...,
-  0x0000a1e8 002d3332 26001834 4e03026e 012d3333 .-32&..4N..n.-33
-  0x0000a1f8 26001835 51030372 001d3426 0017360d &..5Q..r..4&..6.
-  0x0000a208 03026d06 3d323335 26001737 10030333 ..m.=235&..7...3
-  0x0000a218 032d3336 26001838 cc021231 26001d37 .-36&..8...1&..7
-  0x0000a228 26001839 cf020372 000d7c01 2834308b &..9...r..|.(40.
-  0x0000a238 02123226 000d7c01 2834318e 02020d00 ..2&..|.(41.....
-  0x0000a248 2d343026 0018324a 02123326 000f6d06 -40&..2J..3&..m.
-  0x0000a258 04233234 2000086d 06393932 5d5c0202 .#24 ..m.992]\..
-  0x0000a268 93242e32 346d0632 3234381b 000e6d06 .$.24m.2248...m.
-  0x0000a278 13323801 043d000f 6d060413 32850117 .28..=..m...2...
-  0x0000a288 356d062e 3230c604 02501203 2e000377 5m..20...P.....w
-  0x0000a298 02293439 8c000259 122f3235 6d060012 .)49...Y./25m...
-  0x0000a2a8 32cb0905 46000f6d 06041232 cf093832 2...F..m...2..82
-  0x0000a2b8 35388d00 0ec60403 ed012735 37b80229 58........'57..)
-  0x0000a2c8 35368d00 026e092f 32356d06 00123264 56...n./25m...2d
-  0x0000a2d8 09044600 2f36328d 00040265 09273236 ..F./62....e.'26
-  0x0000a2e8 6d063e32 31368d00 02630027 3634f902 m.>216...c.'64..
-  0x0000a2f8 2a36338d 0013394a 000f6d06 0002e708 *63...9J..m.....
-  0x0000a308 0546000f 6d060503 6e022737 328d002d .F..m...n.'72..-
-  0x0000a318 32348d00 02111228 32376d06 2937308d 24.....(27m.)70.
-  0x0000a328 00025412 2f32376d 0601029a 08054600 ..T./27m......F.
-  0x0000a338 0f6d0605 02e30818 325a123d 3233328d .m......2Z.=232.
-  0x0000a348 00034605 2737387b 030afd11 13321f03 ..F.'78{.....2..
-  0x0000a358 1f376d06 01029a08 0446002f 38338d00 .7m......F./83..
-  0x0000a368 0402e408 37323836 8d000e12 2f123233 ....7286..../.23
-  0x0000a378 12283238 6d062938 348d0002 35122f32 .(28m.)84...5./2
-  0x0000a388 386d0601 029a0804 46000fcf 2c051332 8m......F...,..2
-  0x0000a398 32122839 338d000e c10202cd 11283239 2.(93........(29
-  0x0000a3a8 6d060ad5 2c1232cd 112f3239 6d060102 m...,.2../29m...
-  0x0000a3b8 9a082f32 346d0603 02db0827 32346d06 ../24m.....'24m.
-  0x0000a3c8 0dc21112 33e40828 32356d06 0dc41112 ....3..(25m.....
-  0x0000a3d8 33a80527 32356d06 1d33c511 1233a805 3..'25m..3...3..
-  0x0000a3e8 2732356d 063d3330 31260018 33920312 '25m.=301&..3...
-  0x0000a3f8 3726001d 32260018 344e0312 3926001d 7&..2&..4N..9&..
-  0x0000a408 33260018 35510303 72001d34 26001736 3&..5Q..r..4&..6
-  0x0000a418 0d0302ea 003d3330 35260017 37100302 .....=305&..7...
-  0x0000a428 33033d33 30362600 1838cc02 12312600 3.=306&..8...1&.
-  0x0000a438 1d372600 1839cf02 0372000d 7c01024f .7&..9...r..|..O
-  0x0000a448 0e273238 6d063d33 30392600 18318e02 .'28m.=309&..1..
-  0x0000a458 0272002d 31302600 18324a02 12332600 .r.-10&..2J..3&.
-  0x0000a468 0f6d0604 23333120 00076d06 15321316 .m..#31 ..m..2..
-  0x0000a478 025c0212 330c022e 33316d06 1233950e .\..3...31m..3..
-  0x0000a488 2e33316d 06123385 09053d00 0f6d0604 .31m..3...=..m..
-  0x0000a498 1233cf09 2833326d 0601c413 0ad50003 .3..(32m........
-  0x0000a4a8 d80e2732 30770229 31398c00 03d50e1f ..'20w.)19......
-  0x0000a4b8 326d0600 1233cb09 0546000f 6d060413 2m...3...F..m...
-  0x0000a4c8 33840227 32388d00 0ed11312 33710903 3..'28......3q..
-  0x0000a4d8 2e000434 00096d06 12336e09 2f33326d ...4..m..3n./32m
-  0x0000a4e8 06001333 351b0346 000f371b 06031f16 ...35..F..7.....
-  0x0000a4f8 09391b0e d2131333 ec022733 34f9020a .9.....3..'34...
-  0x0000a508 dc1a1333 35031f33 6d060012 33e70805 ...35..3m...3...
-  0x0000a518 46000f6d 06041233 e8082833 346d060e F..m...3..(34m..
-  0x0000a528 d3131233 9b0f032e 00033a03 2934308d ...3......:.)40.
-  0x0000a538 0002980f 2f33346d 06001233 9a080546 ..../34m...3...F
-  0x0000a548 000f6d06 041233e3 08283334 6d060ed4 ..m...3..(34m...
-  0x0000a558 131233dc 0f032e00 037b0329 34378d00 ..3......{.)47..
-  0x0000a568 0226122f 33346d06 0012339a 08044600 .&./34m...3...F.
-  0x0000a578 2f35338d 000402e4 08273335 6d061e33 /53......'35m..3
-  0x0000a588 d4131233 5d12032e 0003bc03 2935348d ...3].......)54.
-  0x0000a598 0003a300 1f356d06 00133360 04034600 .....5m...3`..F.
-  0x0000a5a8 2f36308d 000402e4 08273336 6d061e33 /60......'36m..3
-  0x0000a5b8 d4131233 e1112733 366d063a 3336318d ...3..'36m.:361.
-  0x0000a5c8 0013374a 000e6d06 12339a08 2f33316d ..7J..m..3../31m
-  0x0000a5d8 06021233 db082633 316d061d 33cb1112 ...3..&31m..3...
-  0x0000a5e8 33e40827 33326d06 1d33cb11 38333731 3..'32m..3..8371
-  0x0000a5f8 d303024c 000dcb11 38333732 8f03029c ...L....8372....
-  0x0000a608 002d3731 26001833 92030272 002d3732 .-71&..3...r.-72
-  0x0000a618 26001834 4e0302ca 001d376d 06020e09 &..4N.....7m....
-  0x0000a628 2833336d 061d376d 06025709 2833346d (33m..7m..W.(34m
-  0x0000a638 061d372f 01026109 2833346d 062d3736 ..7/..a.(34m.-76
-  0x0000a648 26001838 cc021231 26000d6d 06026606 &..8...1&..m..f.
-  0x0000a658 2833346d 060d8e36 38333830 8b02023d (34m...68380...=
-  0x0000a668 012d3739 26001831 8e02020d 000d9436 .-79&..1.......6
-  0x0000a678 38333832 4a020263 012f3831 9e020404 8382J..c./81....
-  0x0000a688 20001834 281f2930 5d5c0202 a00e2f33  ..4(.)0]\..../3
-  0x0000a698 386d0600 02950e2f 33386d06 00028509 8m...../38m.....
-  0x0000a6a8 053d000f 6d060502 cf093833 39318100 .=..m.....8391..
-  0x0000a6b8 0ec60404 d80e1730 77022938 398c0004 .......0w.)89...
-  0x0000a6c8 26120f6d 060102cb 09054600 0f6d0605 &..m......F..m..
-  0x0000a6d8 02cf0927 33396d06 1e33d413 12347109 ...'39m..3...4q.
-  0x0000a6e8 032e0003 b8022839 368d0012 346e092f ......(96...4n./
-  0x0000a6f8 33396d06 00123464 09034600 3f343032 39m...4d..F.?402
-  0x0000a708 8d000312 34650927 34306d06 1e33d413 ....4e.'40m..3..
-  0x0000a718 1234f408 032e0013 330d0009 1d041234 .4......3......4
-  0x0000a728 f1081234 90090a6d 061234e7 08054600 ...4...m..4...F.
-  0x0000a738 0f6d0604 1234e808 2734316d 061e33d4 .m...4..'41m..3.
-  0x0000a748 1312349b 0f273431 6d063934 31308d00 ..4..'41m.9410..
-  0x0000a758 02bd012f 34316d06 00123476 04054600 .../41m...4v..F.
-  0x0000a768 0f6d0604 1234e308 2734316d 061e33d4 .m...4..'41m..3.
-  0x0000a778 131234dc 0f032e00 027b0339 3431378d ..4......{.9417.
-  0x0000a788 00022612 2f34316d 06001234 9a080446 ..&./41m...4...F
-  0x0000a798 002f3233 8d000402 e4083834 32368d00 ./23......8426..
-  0x0000a7a8 0dc10212 345d1227 34326d06 39343234 ....4].'42m.9424
-  0x0000a7b8 8d00025b 122f3432 6d060012 349a0804 ...[./42m...4...
-  0x0000a7c8 46002f33 308d0004 02e40837 3433338d F./30......7433.
-  0x0000a7d8 000ed413 1234e111 2734336d 063a3433 .....4..'43m.:43
-  0x0000a7e8 318d0013 374a000e 6d062834 33f6030c 1...7J..m.(43...
-  0x0000a7f8 6d063734 33392f04 0369000c f1043834 m.7439/..i....84
-  0x0000a808 3430d003 036c001d 39260018 31d30302 40...l..9&..1...
-  0x0000a818 4c000dcb 111234a8 05273339 6d063d34 L.....4..'39m.=4
-  0x0000a828 34312600 18339203 0272002d 34322600 41&..3...r.-42&.
-  0x0000a838 18344e03 026e012d 34332600 18355103 .4N..n.-43&..5Q.
-  0x0000a848 0372001d 34260017 360d0302 6d063d34 .r..4&..6...m.=4
-  0x0000a858 34352600 17371003 0333030d cc361234 45&..7...3...6.4
-  0x0000a868 66062734 316d063d 34343726 001839cf f.'41m.=447&..9.
-  0x0000a878 02037200 0d7c0128 35308b02 0278002d ..r..|.(50...x.-
-  0x0000a888 34392600 18318e02 020d002d 35302600 49&..1.....-50&.
-  0x0000a898 18324a02 12332600 0f6d0604 23343520 .2J..3&..m..#45 
-  0x0000a8a8 00086d06 01e51507 5c0202a0 0e2e3435 ..m.....\.....45
-  0x0000a8b8 6d061234 950e2e34 356d0612 34850905 m..4...45m..4...
-  0x0000a8c8 3d000f6d 06041334 13012736 31810001 =..m...4..'61...
-  0x0000a8d8 c8130ad5 0002d80e 032e0003 77022935 ............w.)5
-  0x0000a8e8 398c0002 d50e2f34 366d0600 1234cb09 9...../46m...4..
-  0x0000a8f8 0546000f 6d060412 34cf0919 34dd240e .F..m...4...4.$.
-  0x0000a908 d4131334 7b012736 37b8020a 80241334 ...4{.'67....$.4
-  0x0000a918 c4011f36 6d060102 64090446 002f3732 ...6m...d..F./72
-  0x0000a928 8d000402 65093834 37358d00 0ec60402 ....e.8475......
-  0x0000a938 f408032e 0003f902 2a37338d 0013394a ........*73...9J
-  0x0000a948 000f6d06 0002e708 0546000f 6d060502 ..m......F..m...
-  0x0000a958 e8082734 386d061e 34d41312 349b0f28 ..'48m..4...4..(
-  0x0000a968 34386d06 2938308d 0002980f 2f34386d 48m.)80...../48m
-  0x0000a978 0601029a 08054600 0f6d0605 02e30827 ......F..m.....'
-  0x0000a988 34386d06 1e34d413 1234dc0f 032e0003 48m..4...4......
-  0x0000a998 7b031a38 6d060226 122f3438 6d060102 {..8m..&./48m...
-  0x0000a9a8 9a080446 002f3933 8d000402 e4082734 ...F./93......'4
-  0x0000a9b8 396d061e 34d41312 345d1228 34396d06 9m..4...4].(49m.
-  0x0000a9c8 2839348d 0012355b 122f3439 6d060013 (94...5[./49m...
-  0x0000a9d8 359a0802 46003f35 30308d00 031235e4 5...F.?500....5.
-  0x0000a9e8 08273530 6d061e34 d4131235 e1112735 .'50m..4...5..'5
-  0x0000a9f8 306d063a 3530318d 00123716 000f6d06 0m.:501...7...m.
-  0x0000aa08 00283530 f6030c6d 06373530 392f0403 .(50...m.7509/..
-  0x0000aa18 69000cf1 04383531 30d00303 6c001d39 i....8510...l..9
-  0x0000aa28 26001831 d303024c 000dcb11 38353132 &..1...L....8512
-  0x0000aa38 8f031238 26001d31 26001833 92030272 ...8&..1&..3...r
-  0x0000aa48 002d3132 26001834 4e03026e 012d3133 .-12&..4N..n.-13
-  0x0000aa58 26001835 51030372 001d3426 0017360d &..5Q..r..4&..6.
-  0x0000aa68 0302e205 3d353135 26001737 10030233 ....=515&..7...3
-  0x0000aa78 033d3531 36260018 38cc0202 52002d31 .=516&..8...R.-1
-  0x0000aa88 37260018 39cf0203 72000d7c 01024f0e 7&..9...r..|..O.
-  0x0000aa98 2734396d 063d3531 39260018 318e0202 '49m.=519&..1...
-  0x0000aaa8 72002d32 30260018 324a0212 3326000f r.-20&..2J..3&..
-  0x0000aab8 6d060423 35322000 18349e02 29385d5c m..#52 ..4..)8]\
-  0x0000aac8 02039a01 1e326d06 1335db01 1e326d06 .....2m..5...2m.
-  0x0000aad8 12358509 053d000f 6d060412 35cf0927 .5...=..m...5..'
-  0x0000aae8 35336d06 1134c813 0ad50002 d80e032e 53m..4..........
-  0x0000aaf8 00037702 2932398c 0002d50e 2f35336d ..w.)29...../53m
-  0x0000ab08 06001235 cb090546 000f6d06 041235cf ...5...F..m...5.
-  0x0000ab18 09283533 6d060ed4 13133519 0f273337 .(53m.....5..'37
-  0x0000ab28 b8022933 368d0002 6e092f35 336d0600 ..)36...n./53m..
-  0x0000ab38 12356409 0446002f 34328d00 04031317 .5d..F./42......
-  0x0000ab48 18346d06 0ed41312 35f40803 2e0003f9 .4m.....5.......
-  0x0000ab58 022a3433 8d001339 4a000e6d 06133505 .*43...9J..m..5.
-  0x0000ab68 03044600 0f6d0604 1235e808 37353532 ..F..m...5..7552
-  0x0000ab78 8d000ed4 1312359b 0f032e00 03770029 ......5......w.)
-  0x0000ab88 35308d00 02980f2f 35356d06 0012359a 50...../55m...5.
-  0x0000ab98 08054600 0f6d0604 1235e308 38353539 ..F..m...5..8559
-  0x0000aba8 8d000d87 071235dc 0f032e00 037b030a ......5......{..
-  0x0000abb8 3c481235 26122f35 356d0600 12359a08 <H.5&./55m...5..
-  0x0000abc8 0446002f 36338d00 0402e408 37353636 .F./63......7566
-  0x0000abd8 8d000ed4 1312355d 12032e00 03bc030a ......5]........
-  0x0000abe8 47481235 5b122f35 366d0601 04320002 GH.5[./56m...2..
-  0x0000abf8 46002f37 308d0004 033b0406 4e483e34 F./70....;..NH>4
-  0x0000ac08 2b35d413 1235e111 2835376d 062a3731 +5...5..(57m.*71
-  0x0000ac18 8d001337 4a000f6d 0600029a 082f3532 ...7J..m...../52
-  0x0000ac28 6d060302 db082735 326d060d cb111235 m.....'52m.....5
-  0x0000ac38 e4082835 336d060d cb113835 3831d303 ..(53m....8581..
-  0x0000ac48 024c000d cb113835 38328f03 029c000d .L....8582......
-  0x0000ac58 62483835 38339203 0272000d 65483835 bH8583...r..eH85
-  0x0000ac68 38344e03 02ca002d 38332600 18355103 84N....-83&..5Q.
-  0x0000ac78 0372000d 6d060257 09030d03 0368032d .r..m..W.....h.-
-  0x0000ac88 38352600 17371003 0333032d 38362600 85&..7...3.-86&.
-  0x0000ac98 1838cc02 0252002d 38372600 1839cf02 .8...R.-87&..9..
-  0x0000aca8 0372000d 7c012839 308b0202 3d010d53 .r..|.(90...=..S
-  0x0000acb8 2e383539 318e0202 0d000d56 2e12358b .8591......V..5.
-  0x0000acc8 09283537 6d060d59 2e373539 33192f12 .(57m..Y.7593./.
-  0x0000acd8 32ad280a e0022639 34cc472f 3837d142 2.(...&94.G/87.B
-  0x0000ace8 0c032e00 2d3539a7 43123542 07044529 ....-59.C.5B..E)
-  0x0000acf8 026b000b 4b03023f 07059229 1f37d142 .k..K..?...).7.B
-  0x0000ad08 0c033000 2d3539ab 43293539 45231232 ..0.-59.C)59E#.2
-  0x0000ad18 ab1c0b6d 0028382c 92230f6d 00052432 ...m.(8,.#.m..$2
-  0x0000ad28 316d0022 382c5a00 0e6d0018 39451d12 1m."8,Z..m..9E..
-  0x0000ad38 32ab1609 6d001336 091d0492 1d0f6d00 2...m..6......m.
-  0x0000ad48 0603ee44 0330003c 3539396d 001236dc ...D.0.<599m..6.
-  0x0000ad58 0a283336 6d001b38 6d002832 2c92170f .(36m..8m.(2,...
-  0x0000ad68 6d000603 f2440330 002d3630 44593836 m....D.0.-60DY86
-  0x0000ad78 30334511 1232ab0a 0b6d0028 342c9211 03E..2...m.(4,..
-  0x0000ad88 0f6d0006 03210203 30002d36 30210212 .m...!..0.-60!..
-  0x0000ad98 368e1027 35306d00 2b35326d 0028362c 6..'50m.+52m.(6,
-  0x0000ada8 920b0f6d 00060321 02033000 2d363021 ...m...!..0.-60!
-  0x0000adb8 02293630 4505026d 001b396d 0028382c .)60E..m..9m.(8,
-  0x0000adc8 92050f6d 00051333 21020330 00363630 ...m...3!..0.660
-  0x0000add8 375f4515 325f4550 0a7d0a0a 00000000 7_E.2_EP.}......
+  0x00008978 00000000 00000000 01000000 03000000 ................
+  0x00008988 00000000 00000000 00000000 00000000 ................
+  0x00008998 40000000 00000000 70030000 00000000 @.......p.......
+  0x000089a8 00000000 00000000 01000000 00000000 ................
+  0x000089b8 00000000 00000000 0b000000 03000000 ................
+  0x000089c8 00000000 00000000 00000000 00000000 ................
+  0x000089d8 b0030000 00000000 e1030000 00000000 ................
+  0x000089e8 00000000 00000000 01000000 00000000 ................
+  0x000089f8 00000000 00000000 13000000 02000000 ................
+  0x00008a08 00000000 00000000 00000000 00000000 ................
+  0x00008a18 98070000 00000000 38010000 00000000 ........8.......
+  0x00008a28 02000000 0a000000 08000000 00000000 ................
+  0x00008a38 18000000 00000000 15030000 01000000 ................
+  0x00008a48 00000000 00000000 00000000 00000000 ................
+  0x00008a58 d0080000 00000000 50010000 00000000 ........P.......
+  0x00008a68 00000000 00000000 01000000 00000000 ................
+  0x00008a78 00000000 00000000 29000000 00000070 ........)......p
+  0x00008a88 00000000 00000000 00000000 00000000 ................
+  0x00008a98 200a0000 00000000 90000000 00000000  ...............
+  0x00008aa8 03000000 00000000 04000000 00000000 ................
+  0x00008ab8 00000000 00000000 5d000000 00000070 ........]......p
+  0x00008ac8 40000000 00000000 00000000 00000000 @...............
+  0x00008ad8 b00a0000 00000000 6c000000 00000000 ........l.......
+  0x00008ae8 03000000 0f000000 04000000 00000000 ................
+  0x00008af8 00000000 00000000 51010000 00000070 ........Q......p
+  0x00008b08 40000000 00000000 00000000 00000000 @...............
+  0x00008b18 1c0b0000 00000000 6c000000 00000000 ........l.......
+  0x00008b28 03000000 10000000 04000000 00000000 ................
+  0x00008b38 00000000 00000000 49020000 00000070 ........I......p
+  0x00008b48 40000000 00000000 00000000 00000000 @...............
+  0x00008b58 880b0000 00000000 6c000000 00000000 ........l.......
+  0x00008b68 03000000 11000000 04000000 00000000 ................
+  0x00008b78 00000000 00000000 45030000 01000070 ........E......p
+  0x00008b88 00000000 00000000 00000000 00000000 ................
+  0x00008b98 f40b0000 00000000 20000000 00000000 ........ .......
+  0x00008ba8 03000000 00000000 04000000 00000000 ................
+  0x00008bb8 08000000 00000000 61030000 0b000070 ........a......p
+  0x00008bc8 00000000 00000000 00000000 00000000 ................
+  0x00008bd8 180c0000 00000000 10000000 00000000 ................
+  0x00008be8 00000000 00000000 08000000 00000000 ................
+  0x00008bf8 08000000 00000000 22030000 09000000 ........".......
+  0x00008c08 40000000 00000000 00000000 00000000 @...............
+  0x00008c18 280c0000 00000000 30000000 00000000 (.......0.......
+  0x00008c28 03000000 04000000 08000000 00000000 ................
+  0x00008c38 10000000 00000000 bb000000 01000000 ................
+  0x00008c48 42000000 00000000 00000000 00000000 B...............
+  0x00008c58 580c0000 00000000 80010000 00000000 X...............
+  0x00008c68 00000000 0f000000 04000000 00000000 ................
+  0x00008c78 00000000 00000000 b1010000 01000000 ................
+  0x00008c88 42000000 00000000 00000000 00000000 B...............
+  0x00008c98 d80d0000 00000000 80010000 00000000 ................
+  0x00008ca8 00000000 10000000 04000000 00000000 ................
+  0x00008cb8 00000000 00000000 a9020000 01000000 ................
+  0x00008cc8 42000000 00000000 00000000 00000000 B...............
+  0x00008cd8 580f0000 00000000 80010000 00000000 X...............
+  0x00008ce8 00000000 11000000 04000000 00000000 ................
+  0x00008cf8 00000000 00000000 32000000 01000000 ........2.......
+  0x00008d08 06000000 00000000 00000000 00000000 ................
+  0x00008d18 00110000 00000000 001a0000 00000000 ................
+  0x00008d28 03000000 0a000034 80000000 00000000 .......4........
+  0x00008d38 00000000 00000000 25010000 01000000 ........%.......
+  0x00008d48 06000000 00000000 00000000 00000000 ................
+  0x00008d58 002b0000 00000000 80080000 00000000 .+..............
+  0x00008d68 03000000 0b000022 80000000 00000000 ......."........
+  0x00008d78 00000000 00000000 1d020000 01000000 ................
+  0x00008d88 06000000 00000000 00000000 00000000 ................
+  0x00008d98 80330000 00000000 00040000 00000000 .3..............
+  0x00008da8 03000000 0c000018 80000000 00000000 ................
+  0x00008db8 00000000 00000000 06000000 05000000 ................
+  0x00008dc8 003c0000 00000000 00000000 00000000 .<..............
+  0x00008dd8 00000000 00000000 a8000000 00000000 ................
+  0x00008de8 a8000000 00000000 08000000 00000000 ................
+  0x00008df8 01000000 05000000 580c0000 00000000 ........X.......
+  0x00008e08 00000000 00000000 00000000 00000000 ................
+  0x00008e18 282b0000 00000000 282b0000 00000000 (+......(+......
+  0x00008e28 08000000 00000000 01000000 05000000 ................
+  0x00008e38 003c0000 00000000 00000000 00000000 .<..............
+  0x00008e48 00000000 00000000 a8000000 00000000 ................
+  0x00008e58 a8000000 00000000 08000000 00000000 ................
+  0x00008e68 01000101 58000000 481f0000 00000000 ....X...H.......
+  0x00008e78 451f0000 48000000 04000800 50000000 E...H.......P...
+  0x00008e88 00000000 00000000 11200000 00000000 ......... ......
+  0x00008e98 00000000 00000000 9e620000 00000000 .........b......
+  0x00008ea8 00000000 00000000 50000000 00000000 ........P.......
+  0x00008eb8 00000000 00000000 3c0a2f2f 0300f31e ........<.//....
+  0x00008ec8 0a2e7665 7273696f 6e20382e 340a2e74 ..version 8.4..t
+  0x00008ed8 61726765 7420736d 5f38300a 2e616464 arget sm_80..add
+  0x00008ee8 72657373 5f73697a 65203634 0a3100ff ress_size 64.1..
+  0x00008ef8 31697369 626c6520 2e656e74 7279205f 1isible .entry _
+  0x00008f08 5a313961 6374696f 6e4f6e53 696e676c Z19actionOnSingl
+  0x00008f18 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
+  0x00008f28 5f6d506d 280a2e70 6172616d 202e7536 _mPm(..param .u6
+  0x00008f38 34330013 115f3100 3f5f302c 3b00261f 43..._1.?_0,;.&.
+  0x00008f48 313b0027 1f323b00 27f30833 0a290a7b 1;.'.2;.'..3.).{
+  0x00008f58 0a2e7265 67202e70 72656420 25703c36 ..reg .pred %p<6
+  0x00008f68 3e3b1200 95663332 2025663c 34351200 >;...f32 %f<45..
+  0x00008f78 10621200 36723c38 1100f201 36342025 .b..6r<8....64 %
+  0x00008f88 72643c31 333e3b0a 0a0a6c64 8a00222e rd<13>;...ld..".
+  0x00008f98 7518004f 322c205b 9000193d 305d3b44 u..O2, [...=0];D
+  0x00008fa8 001f3344 001c1f31 4400001f 3444001c ..3D...1D...4D..
+  0x00008fb8 1f324400 001f3544 001c9133 5d3b0a6d .2D...5D...3];.m
+  0x00008fc8 6f762e75 3401a832 2c20256e 7469642e ov.u4..2, %ntid.
+  0x00008fd8 7816007c 332c2025 63746117 0044342c x..|3, %cta..D4,
+  0x00008fe8 20252c00 7161642e 6c6f2e73 18002335  %,.qad.lo.s..#5
+  0x00008ff8 2c340001 4f00f403 72343b0a 63767461 ,4..O...r4;.cvta
+  0x00009008 2e746f2e 676c6f62 616cab00 21362cb1 .to.global..!6,.
+  0x00009018 0001c400 041a0001 41004036 2c205b20 ........A.@6, [ 
+  0x00009028 00535d3b 0a6f72ce 0124312c 5a001136 .S];.or..$1,Z..6
+  0x00009038 5000432e 73363470 0012641c 00923b0a P.C.s64p..d...;.
+  0x00009048 73657470 2e676560 00357031 2c1c0073 setp.ge`.5p1,..s
+  0x00009058 64343b0a 7368725f 0013379b 00173132 d4;.shr_..7...12
+  0x00009068 00001900 3370322c d6002172 377a0003 ....3p2,..!r7z..
+  0x00009078 6c022333 2c1c0014 70320022 65717b00 l.#3,...p2."eq{.
+  0x00009088 25703496 00183132 0024352c 3700ff08 %p4...12.$5,7...
+  0x00009098 343b0a40 25703520 62726120 244c5f5f 4;.@%p5 bra $L__
+  0x000090a8 4242305f 323b0a12 0104019a 002f6432 BB0_2;......./d2
+  0x000090b8 31010511 381f0018 33310121 76320003 1...8...31.!v2..
+  0x000090c8 307b2566 e9003266 327d3b01 20385df1 0{%f..2f2};. 8].
+  0x000090d8 00146cf9 0214390b 0182333b 0a616464 ..l...9...3;.add
+  0x000090e8 2e731700 3631302c 76001f39 57000300 .s..610,v..9W...
+  0x000090f8 cb002366 36570010 31fa0233 6d756c74 ..#f6W..1..3mult
+  0x00009108 03005700 02780018 35170001 57002166 ..W..x..5...W.!f
+  0x00009118 32390054 3b0a7375 62180025 312c3500 29.T;.sub..%1,5.
+  0x00009128 1f30c500 04013600 243133c7 00232b38 .0....6.$13..#+8
+  0x00009138 71004577 696465ef 0122312c 11021a38 q.Ewide.."1,...8
+  0x00009148 ce00003c 0004ce00 2f313161 00041136 ...<..../11a...6
+  0x00009158 61001437 d1000043 0363666d 612e726e a..7...C.cfma.rn
+  0x00009168 a5001132 bd000388 00022d00 1831dd00 ...2......-..1..
+  0x00009178 223231a2 00010600 19371a00 15320f01 "21......7...2..
+  0x00009188 1c365500 15331201 0150012c 32322100 .6U..3...P.,22!.
+  0x00009198 17345600 0176001f 32e70104 12324100 .4V..v..2....2A.
+  0x000091a8 15362201 3931365d 86000160 012d3235 .6".916]...`.-25
+  0x000091b8 96011233 96011d36 97013533 312c3800 ...3...6..531,8.
+  0x000091c8 1f339801 041133bc 00163398 012c3234 .3....3...3..,24
+  0x000091d8 39011133 5a002633 32c30019 33390121 9..3Z.&32...39.!
+  0x000091e8 33371400 0f390100 2633389a 001c3556 37...9..&38...5V
+  0x000091f8 0007cf00 0255001b 38220027 34307800 .....U..8".'40x.
+  0x00009208 0264001c 39230017 31d40101 23002832 .d..9#..1...#.(2
+  0x00009218 34020135 34322cfa 011032e4 031b7402 4..542,...2...t.
+  0x00009228 0103fc02 342c207b 2d003c34 317d6500 ....4, {-.<41}e.
+  0x00009238 1733e000 01ab0029 34306500 26342c26 .3.....)40e.&4,&
+  0x00009248 011f3765 00051332 6500012d 00653433 ..7e...2e..-.e43
+  0x00009258 7d3b0a0a 3704903a 0a726574 3b0a0a7d };..7..:.ret;..}
+  0x00009268 35081f2e 3408084f 446f7562 34081c0e 5...4..ODoub4...
+  0x00009278 33000e34 080f3b00 241f313b 00271f32 3..4..;.$.1;.'.2
+  0x00009288 3b00270f 3408012c 31373508 3c313631 ;.'.4..,175.<161
+  0x00009298 36082d31 3237082f 32303708 060e9300 6.-127./207.....
+  0x000092a8 0f37082b 0e44000f 37081f0e 44000f37 .7.+.D..7...D..7
+  0x000092b8 081f0e44 000f3708 091f3421 08031f35 ...D..7...4!...5
+  0x000092c8 4e08021f 36370804 15374c07 1634e707 N...67...7L..4..
+  0x000092d8 0f370814 233634fb 05043808 30637674 .7..#64...8.0cvt
+  0x000092e8 6f00031a 00023907 1c374f08 0172001f o.....9..7O..r..
+  0x000092f8 38490000 13384900 2d2b384b 0021392c 8I...8I.-+8K.!9,
+  0x00009308 2100074b 0015324b 00193990 0617398f !..K..2K..9...9.
+  0x00009318 061c3847 00037b07 17394800 15334800 ..8G..{..9H..3H.
+  0x00009328 23313068 08136ef4 06267031 1c000c1b #10h..n..&p1....
+  0x00009338 00067f00 69323b0a 616e64b6 081131bb ....i2;.and...1.
+  0x00009348 080c3300 15343300 19333300 09b7080a ..3..43..33.....
+  0x00009358 33002436 2c35010a 66002337 2c1d002c 3.$6,5..f.#7,..,
+  0x00009368 70353300 15383300 0a660023 392c1d00 p53..83..f.#9,..
+  0x00009378 2c703733 00021601 1e323400 01f30702 ,p73.....24.....
+  0x00009388 1f002f70 39000a03 044d0022 6c746301 ../p9....M."ltc.
+  0x00009398 1170f005 031d000a 010a0241 08163502 .p.........A..5.
+  0x000093a8 0a226c74 1a001170 820701a2 023a7231 ."lt...p.....:r1
+  0x000093b8 31820024 342c2000 2a703104 01363135 1..$4, .*p1..615
+  0x000093c8 2c210065 313b0a6e 6f741b00 11361500 ,!.e1;.not...6..
+  0x000093d8 1135060a 27313607 0a1f3107 0a082f31 .5..'16...1.../1
+  0x000093e8 30080a0b 2f313109 0a162a31 310a0a2f 0.../11...*11../
+  0x000093f8 31320b0a 0427332c 7a002f31 320d0a11 12...'3,z./12...
+  0x00009408 2f335d0d 0a5a2f31 310e0a03 1f340e0a /3]..Z/11....4..
+  0x00009418 0328352c d1001f34 6300041a 360f0a1f .(5,...4c...6...
+  0x00009428 350f0a2d 06e10002 0f0a0655 080f7f00 5..-.......U....
+  0x00009438 0103180a 1634e200 2f3136e3 00011336 .....4../16....6
+  0x00009448 17030be3 0001c303 05e3001f 36640004 ............6d..
+  0x00009458 11376400 14386400 1d37b909 01c30003 .7d..8d..7......
+  0x00009468 8b001437 9f0a06e3 00025b09 02a20a28 ...7......[....(
+  0x00009478 3238e300 02ed0802 40001f33 33020411 28......@..33...
+  0x00009488 33380026 3335e300 2f3234e3 00011338 38.&35../24....8
+  0x00009498 350e0be3 0028392c e3001f38 64000411 5....(9,...8d...
+  0x000094a8 38640014 3964001c 39e30002 b409038b 8d..9d..9.......
+  0x000094b8 00022d00 1833e300 03bc0914 353e0a07 ..-..3......5>..
+  0x000094c8 1a001634 ba0b0b9b 0a253435 f2020119 ...4.....%45....
+  0x000094d8 022c3434 21001c36 770a1d34 44001737 .,44!..6w..4D..7
+  0x000094e8 3f020246 000c3c0c 2734389f 01010c00 ?..F..<.'48.....
+  0x000094f8 2c343723 001739a2 01026900 0c260b27 ,47#..9...i..&.'
+  0x00009508 35300201 012f001f 34f10d05 01d20016 50.../..4.......
+  0x00009518 35410448 2b33325d 13011135 f8001e35 5A.H+32]...5...5
+  0x00009528 eb032235 363a000d ec033635 372c3800 .."56:....657,8.
+  0x00009538 0fa70204 1135db00 26353977 003b3430 .....5..&59w.;40
+  0x00009548 5dc50011 365b0026 35382e01 1935490c ]...6[.&58...5I.
+  0x00009558 22363344 000e8d03 3536342c 40001f36 "63D....564,@..6
+  0x00009568 38050411 36a00027 36368200 1d388200 8...6..'66...8..
+  0x00009578 015c0026 36356a01 28363482 00223730 .\.&65j.(64.."70
+  0x00009588 44000e2c 03353731 2c40001f 37f10404 D..,.571,@..7...
+  0x00009598 1137a000 1737f104 2c353682 0011375c .7...7..,56...7\
+  0x000095a8 00022a00 02cb0219 37910422 37374400 ..*.....7.."77D.
+  0x000095b8 0ecb0226 37389f01 0ccc0226 3739d401 ...&78.....&79..
+  0x000095c8 0261000c 41022738 307c0102 64000c67 .a..A.'80|..d..g
+  0x000095d8 0d273831 7f010146 002c3830 23001732 .'81...F.,80#..2
+  0x000095e8 4001014c 002c3831 23001733 43010169 @..L.,81#..3C..i
+  0x000095f8 001c382e 0f273834 0401016f 001f38d4 ..8..'84...o..8.
+  0x00009608 01041138 6a001738 d4013836 345d1501 ...8j..8..864]..
+  0x00009618 12383f00 01270009 cd022239 303a000d .8?..'...."90:..
+  0x00009628 cd023539 312c3800 1f39c901 0411399b ..591,8..9....9.
+  0x00009638 001739c9 013b3732 5dc50011 395b0026 ..9..;72]...9[.&
+  0x00009648 39322e01 1939c901 22393744 000ecd02 92...9.."97D....
+  0x00009658 3639382c 40001f37 82000403 5a071630 698,@..7....Z..0
+  0x00009668 83001d38 50032131 305e0026 39396c01 ...8P.!10^.&99l.
+  0x00009678 28393884 00213130 6a013e31 3030d102 (98..!10j.>100..
+  0x00009688 46313035 2c44002f 31306207 05223036 F105,D./10b.."06
+  0x00009698 20001737 8a000d58 031131e2 05042d00  ..7...X..1...-.
+  0x000096a8 02d80229 31309101 12313208 3e313037 ...)10...12.>107
+  0x000096b8 db023631 3132ae01 0cdc0236 313133e4 ..6112.....6113.
+  0x000096c8 0122362c 2f000d24 0017348e 01123725 ."6,/..$..4...7%
+  0x000096d8 001d3325 00173593 01034a00 1d342500 ..3%..5...J..4%.
+  0x000096e8 17365401 02c9002d 31352500 18375801 .6T....-15%..7X.
+  0x000096f8 0370001d 36260018 38150112 3926000f .p..6&..8...9&..
+  0x00009708 f1010422 31312000 1732f201 3939365d ..."11 ..2..996]
+  0x00009718 26010245 06032a00 1a351b00 13343e00 &..E..*..5...4>.
+  0x00009728 0df00212 317d1104 3d001f32 e8010502 ....1}..=..2....
+  0x00009738 c0112731 32e8014c 3130345d d4000287 ..'12..L104]....
+  0x00009748 12042e00 0334000a 8c000251 083e3132 .....4.....Q.>12
+  0x00009758 37fb0213 31e81103 46002f33 318d0004 7...1...F./31...
+  0x00009768 03871118 335a090e ec131231 9412032e ....3Z.....1....
+  0x00009778 00038701 2a33328d 0013384a 000f0203 ....*32...8J....
+  0x00009788 00039301 0446000f 9e080412 31a21237 .....F......1..7
+  0x00009798 3134318d 001e328d 03026b08 032e0003 141...2...k.....
+  0x000097a8 03030be7 02037308 2f343103 0300046e ......s./41....n
+  0x000097b8 081f3004 03022734 37fb0102 2a000d6a ..0...'47...*..j
+  0x000097c8 0812316b 08049c01 0206030d 6d081231 ..1k........m..1
+  0x000097d8 6e08049f 0102c201 0d700812 31710804 n........p..1q..
+  0x000097e8 5b010208 032d3439 26001831 5e010252 [....-49&..1^..R
+  0x000097f8 002d3530 26001832 1a01027f 002d3531 .-50&..2.....-51
+  0x00009808 260008c5 09017100 293530af 01353534 &.....q.)50..554
+  0x00009818 2c0c0a2f 34338213 05123382 13032e00 ,../43....3.....
+  0x00009828 4d313533 7d690017 35630701 69002a38 M153}i..5c..i.*8
+  0x00009838 34690026 362caa07 0feb1306 14356900 4i.&6,.......5i.
+  0x00009848 22362c56 000e6900 1837f204 1238c201 "6,V..i..7...8..
+  0x00009858 0a830203 9107033f 052f3131 6d000514 .......?./11m...
+  0x00009868 376d0002 30002e35 376d0018 395c0203 7m..0..57m..9\..
+  0x00009878 27001932 6d003836 302ca902 1f356d00 '..2m.860,...5m.
+  0x00009888 0513396d 00033000 263539c7 141f31c7 ..9m..0.&59...1.
+  0x00009898 140f1438 8412af54 7269706c 65476174 ...8...TripleGat
+  0x000098a8 65c61408 0f320012 0ec5140f 3a001c1f e....2......:...
+  0x000098b8 313a0026 1f323a00 260ff61c 021c31c2 1:.&.2:.&.....1.
+  0x000098c8 14363630 39b01402 c2142d32 34c2142f .6609.....-24../
+  0x000098d8 3332c214 021231f6 130f4001 160f3914 32....1...@...9.
+  0x000098e8 001f3243 001b1f31 0415010f 43001b1f ..2C...1....C...
+  0x000098f8 32430000 1f344300 1b2f335d 5b110523 2C...4C../3][..#
+  0x00009908 352c2e12 06b0141f 38c61402 1f39f314 5,......8....9..
+  0x00009918 032f3130 de140401 be080136 00247238 ./10.......6.$r8
+  0x00009928 e4132e6c 64db1400 41032d35 5d2f1421 ...ld...A.-5]/.!
+  0x00009938 322c2000 072f1425 312c5600 2f31320d 2, ../.%1,V./12.
+  0x00009948 15071f35 c4140001 11090a10 1517324e ...5..........2N
+  0x00009958 000a1a12 23382c9a 00023200 0b4a001d ....#8,...2..J..
+  0x00009968 340f1517 334a001f 34980000 14399800 4...3J..4....9..
+  0x00009978 2e313699 001d3516 1517344f 001a351c .16...5...4O..5.
+  0x00009988 1017309a 001d394b 0013363a 10074c00 ..0...9K..6:..L.
+  0x00009998 17354c00 1a364c00 1731ad15 0e4c0002 .5L..6L..1...L..
+  0x000099a8 18002731 314c0017 364c001f 37881c01 ..'11L..6L..7...
+  0x000099b8 0353001d 364d0015 38631305 4d001737 .S..6M..8c..M..7
+  0x000099c8 4d001f38 fc15022f 3131fd15 072f3131 M..8.../11.../11
+  0x000099d8 fe151f2f 3131ff15 201331cf 1f0f0016 .../11.. .1.....
+  0x000099e8 19049c1f 0c011601 39001f38 01160302 ........9..8....
+  0x000099f8 35001936 35000114 00023b00 2d313037 5..65.....;.-107
+  0x00009a08 00070801 1a373700 26332c3f 160d0b01 .....77.&3,?....
+  0x00009a18 053c142f 2572d315 081d3337 00020f01 .<./%r....37....
+  0x00009a28 0e420101 2902021f 0001f515 0b370002 .B..)........7..
+  0x00009a38 12010e45 01019609 021f003c 70313737 ...E.......<p177
+  0x00009a48 0001d209 1f724801 00017c14 021f003d .....rH...|....=
+  0x00009a58 70313937 00021401 0e4a0101 c90b021f p197.....J......
+  0x00009a68 003d7032 31370006 13010a4a 0101070c .=p217.....J....
+  0x00009a78 021f003d 70323337 00011301 1e321301 ...=p237.....2..
+  0x00009a88 01d50902 1f003d70 32353700 15383700 ......=p257..87.
+  0x00009a98 0a130101 8f1e021f 002d7032 13012533 .........-p2..%3
+  0x00009aa8 3037000a 1301013b 0c021f00 2d703213 07.....;....-p2.
+  0x00009ab8 01253332 37000a13 0101a60a 021f003d .%327..........=
+  0x00009ac8 70333137 00153437 000a1301 016c0a02 p317..47.....l..
+  0x00009ad8 1f003d70 33333700 0113011e 33dc0001 ..=p337.....3...
+  0x00009ae8 300c021f 002d7033 13012533 3837000b 0....-p3..%387..
+  0x00009af8 dc002439 2c1f003c 70333737 00253430 ..$9,..<p377.%40
+  0x00009b08 37000adc 0001d109 021f003d 70333937 7..........=p397
+  0x00009b18 00153237 000adc00 01131502 1f002d70 ..27..........-p
+  0x00009b28 34130101 030a2e72 34a50001 a20c021f 4......r4.......
+  0x00009b38 003d7034 33370015 3637000b a5002437 .=p437..67....$7
+  0x00009b48 2c1f003d 70343537 00153837 000ba500 ,..=p457..87....
+  0x00009b58 24392c1f 003c7034 37370001 830c2e72 $9,..<p477.....r
+  0x00009b68 356e0001 760c021f 003d7034 39370015 5n..v....=p497..
+  0x00009b78 3237000a 6e000161 0c021f00 3d703531 27..n..a....=p51
+  0x00009b88 370002d7 000f3700 0024352c 1f003e70 7.....7..$5,..>p
+  0x00009b98 3533bd1a 14336e1a 0abf1a01 170c041f 53...3n.........
+  0x00009ba8 00296433 c01a0447 080dc01a 01320c03 .)d3...G.....2..
+  0x00009bb8 5d1c2a31 39870024 382c2100 3a703536 ].*19..$8,!.:p56
+  0x00009bc8 1b002639 2c210019 35c11a01 c30b3170 ..&9,!..5.....1p
+  0x00009bd8 3539c11a 273630c1 1a1f32c1 1a091434 59..'60...2....4
+  0x00009be8 c11a2f6c 64110f00 09a11a00 23100f46 ../ld.......#..F
+  0x00009bf8 00040184 012f6431 1119052f 31311219 ...../d1.../11..
+  0x00009c08 051e3512 190fc61a 062f375d c61a5b3f ..5....../7]..[?
+  0x00009c18 342b3800 19061f31 0019051f 3500190a 4+8....1....5...
+  0x00009c28 010f0107 c61a0d00 19012406 048a0002 ..........$.....
+  0x00009c38 b20f0fc6 1a481f34 c61a0323 32304705 .....H.4...#20G.
+  0x00009c48 0ae30001 7c0005e3 001f3246 0104021c ....|.....2F....
+  0x00009c58 1005c61a 2c3231e3 00273331 27190fc6 ....,21..'31'...
+  0x00009c68 1a4e1f34 c61a0314 324e050b e3000062 .N.4....2N.....b
+  0x00009c78 0006e300 0f640005 1938c61a 2f3233c6 .....d...8../23.
+  0x00009c88 1a2d06e3 0002c61a 06fa100f 7f000102 .-..............
+  0x00009c98 5c122634 36e3002f 3332e300 0113348c \.&46../32....4.
+  0x00009ca8 050be300 003e0006 e3000f25 1404023b .....>.....%...;
+  0x00009cb8 121435a3 141d326f 1d02c411 038b0001 ..5...2o........
+  0x00009cc8 2d002834 34e30001 46050359 1b0ade11 -.(44...F..Y....
+  0x00009cd8 02951102 40001f35 7f000413 35341a06 ....@..5....54..
+  0x00009ce8 e3002f34 30e30001 13360106 0be30000 ../40....6......
+  0x00009cf8 560206e3 000f5d04 0402f410 1436ec13 V.....]......6..
+  0x00009d08 1d326f1d 028b1a02 8b00022d 00283535 .2o........-.(55
+  0x00009d18 e300021d 1901a805 38663631 e3000214 ........8f61....
+  0x00009d28 19024000 2f36357f 00040238 001738e3 ..@./65....8..8.
+  0x00009d38 000f6f04 01027809 1d36e300 00730106 ..o...x..6...s..
+  0x00009d48 e3000f6f 040402cb 1a1437c2 051d326f ...o......7...2o
+  0x00009d58 041137c3 00028b00 03f81a18 36e30002 ..7.........6...
+  0x00009d68 c41a2236 38470008 e30003be 1a014000 .."68G........@.
+  0x00009d78 1f376201 0402c81a 263739e3 002f3536 .7b.....&79../56
+  0x00009d88 e3000002 240a1c37 e30001e8 0305e300 ....$..7........
+  0x00009d98 0ff02805 02a81a14 38b5051d 336f0402 ..(.....8...3o..
+  0x00009da8 6b18028b 00243832 e91306e3 00353837 k....$82.....587
+  0x00009db8 2c571b29 38331a00 1f38521e 0616387e ,W.)83...8R...8~
+  0x00009dc8 06015f00 1c385615 1839c805 1237881a .._..8V..9...7..
+  0x00009dd8 0c230008 cb051436 a51a0a23 0017322b .#.....6...#..2+
+  0x00009de8 0514387a 1a0a2300 1c33521e 1c393319 ..8z..#..3R..93.
+  0x00009df8 2739348e 04123919 190c2300 01c80126 '94...9...#....&
+  0x00009e08 3335b104 2f393406 1b0202f1 03019109 35../94.........
+  0x00009e18 2c663916 01263937 f4030214 041c39ba ,f9..&97......9.
+  0x00009e28 16273938 54031431 181b0a23 00173957 .'98T..1...#..9W
+  0x00009e38 031430eb 1a092300 038f1903 b8021232 ..0...#........2
+  0x00009e48 c7190d24 001731bc 0222312c 37000d25 ...$..1.."1,7..%
+  0x00009e58 0017321e 02123325 000fab18 0505401b ..2...3%......@.
+  0x00009e68 06d0020b a41c0301 16032a00 0b980826 ..........*....&
+  0x00009e78 382ca81b 0a9b0838 30392c3d 000f3c08 8,.....809,=..<.
+  0x00009e88 0502db08 36313131 80000ead 1c03201b ....6111...... .
+  0x00009e98 042d0002 43081a30 81180153 03004900 .-..C..0...S..I.
+  0x00009ea8 0e460803 151b0546 000fbd04 0404171b .F.....F........
+  0x00009eb8 1731bf04 0fb61c00 03ae0826 31379e02 .1.........&17..
+  0x00009ec8 013d1b07 8c0002b7 0803411b 0aef0705 .=........A.....
+  0x00009ed8 c91a0246 000f8e07 0505121b 07f4070f ...F............
+  0x00009ee8 b81c0002 40032731 3295073a 3132338c ....@.'12..:123.
+  0x00009ef8 00133949 000e9807 050e1b03 46000f93 ..9I........F...
+  0x00009f08 21040412 1b163335 0b02dc1b 0a8c0002 !.....35........
+  0x00009f18 6903032d 00022a03 39313330 8c000175 i..-..*.9130...u
+  0x00009f28 0e04461b 0b1f1904 0d1b0346 000f7e05 ..F........F..~.
+  0x00009f38 0405111b 0780050f e81b0102 6d08032e ............m...
+  0x00009f48 00027103 39313337 8d0002b0 0803461b ..q.9137......F.
+  0x00009f58 0aeb0605 64180246 000fb408 0505111b ....d..F........
+  0x00009f68 07b6080e e81b05b3 1a273435 b6030a59 .........'45...Y
+  0x00009f78 0804b01a 2e343695 0604a61a 0346002f .....46......F./
+  0x00009f88 35308d00 04243532 321a068d 000fe81b 50...$522.......
+  0x00009f98 0002a704 032e0002 3c0601ce 1a088d00 ........<.......
+  0x00009fa8 02f9192e 35333f06 283135f2 030c4206 ....53?.(15...B.
+  0x00009fb8 04c61902 2b040369 000de804 283630cd ....+..i....(60.
+  0x00009fc8 03036c00 0dea0402 490504d0 0302f303 ..l.....I.......
+  0x00009fd8 1d36eb04 02542304 8d0302e8 1b2d3631 .6...T#......-61
+  0x00009fe8 26001833 90030272 001d3685 1f02db08 &..3...r..6.....
+  0x00009ff8 27313254 063d3136 33260018 35500303 '12T.=163&..5P..
+  0x0000a008 72000d87 1f022d09 030d0302 5a063d31 r.....-.....Z.=1
+  0x0000a018 36352600 17371003 03e0012d 36362600 65&..7.....-66&.
+  0x0000a028 1838cc02 0310010d 181d02dc 2304cf02 .8..........#...
+  0x0000a038 02f2021d 367c0128 37308b02 023d011d ....6|.(70...=..
+  0x0000a048 367c0128 37318e02 020d002d 37302600 6|.(71.....-70&.
+  0x0000a058 18324a02 0263012f 37319e02 04133720 .2J..c./71....7 
+  0x0000a068 0008a70d 3932385d 5c02027f 092f3137 ....928]\..../17
+  0x0000a078 69060002 cd062f31 37690600 02e60805 i...../17i......
+  0x0000a088 3d000f69 06050242 24273138 69062e31 =..i...B$'18i..1
+  0x0000a098 33c60402 dd232831 386a061a 376a0602 3....#(18j..7j..
+  0x0000a0a8 cb211231 70240b6a 06029909 0546000f .!.1p$.j.....F..
+  0x0000a0b8 6a060502 a0092731 386a062e 3134c604 j.....'18j..14..
+  0x0000a0c8 034e0927 3837b802 1a386b06 0334221f .N.'87...8k..4".
+  0x0000a0d8 386b0601 032b2203 46002f39 328d0004 8k...+".F./92...
+  0x0000a0e8 024b0927 31396b06 2e3135c6 0402e608 .K.'19k..15.....
+  0x0000a0f8 2831396c 062a3933 8d001339 4a000e6c (19l.*93...9J..l
+  0x0000a108 061232de 08054600 0f6c0604 1232e108 ..2...F..l...2..
+  0x0000a118 38323032 cf0f0dc6 041232fe 23273230 8202......2.#'20
+  0x0000a128 6d063832 30308d00 1232b822 2f32306d m.8200...2."/20m
+  0x0000a138 06001232 96080546 000f6d06 041232df ...2...F..m...2.
+  0x0000a148 08283230 6d061d36 86071232 120b032e .(20m..6...2....
+  0x0000a158 00027b03 2932306d 06123212 0b2f3230 ..{.)20m..2../20
+  0x0000a168 6d060012 32970804 46002f31 338d0004 m...2...F./13...
+  0x0000a178 02e10828 32316d06 1d37c102 1132b411 ...(21m..7...2..
+  0x0000a188 042e0002 bc033932 31348d00 0450110f ......9214...P..
+  0x0000a198 6d060012 32980804 46000f10 110602e2 m...2...F.......
+  0x0000a1a8 08283232 6d061d38 c1021132 cc0e042e .(22m..8...2....
+  0x0000a1b8 00026d06 3a323231 8d001337 4a000e6d ..m.:221...7J..m
+  0x0000a1c8 06283232 f6030c6d 06373232 392f0403 .(22...m.7229/..
+  0x0000a1d8 69000cf1 04383233 30d00303 6c001d39 i....8230...l..9
+  0x0000a1e8 26001831 d303024c 002d3330 26001832 &..1...L.-30&..2
+  0x0000a1f8 8f031238 26001d31 26001833 9203022c ...8&..1&..3...,
+  0x0000a208 002d3332 26001834 4e03026e 012d3333 .-32&..4N..n.-33
+  0x0000a218 26001835 51030372 001d3426 0017360d &..5Q..r..4&..6.
+  0x0000a228 03026d06 3d323335 26001737 10030333 ..m.=235&..7...3
+  0x0000a238 032d3336 26001838 cc021231 26001d37 .-36&..8...1&..7
+  0x0000a248 26001839 cf020372 000d7c01 2834308b &..9...r..|.(40.
+  0x0000a258 02123226 000d7c01 2834318e 02020d00 ..2&..|.(41.....
+  0x0000a268 2d343026 0018324a 02123326 000f6d06 -40&..2J..3&..m.
+  0x0000a278 04233234 2000086d 06393932 5d5c0202 .#24 ..m.992]\..
+  0x0000a288 93242e32 346d0632 3234381b 000e6d06 .$.24m.2248...m.
+  0x0000a298 13323801 043d000f 6d060413 32850117 .28..=..m...2...
+  0x0000a2a8 356d062e 3230c604 02501203 2e000377 5m..20...P.....w
+  0x0000a2b8 02293439 8c000259 122f3235 6d060012 .)49...Y./25m...
+  0x0000a2c8 32cb0905 46000f6d 06041232 cf093832 2...F..m...2..82
+  0x0000a2d8 35388d00 0ec60403 ed012735 37b80229 58........'57..)
+  0x0000a2e8 35368d00 026e092f 32356d06 00123264 56...n./25m...2d
+  0x0000a2f8 09044600 2f36328d 00040265 09273236 ..F./62....e.'26
+  0x0000a308 6d063e32 31368d00 02630027 3634f902 m.>216...c.'64..
+  0x0000a318 2a36338d 0013394a 000f6d06 0002e708 *63...9J..m.....
+  0x0000a328 0546000f 6d060503 6e022737 328d002d .F..m...n.'72..-
+  0x0000a338 32348d00 02111228 32376d06 2937308d 24.....(27m.)70.
+  0x0000a348 00025412 2f32376d 0601029a 08054600 ..T./27m......F.
+  0x0000a358 0f6d0605 02e30818 325a123d 3233328d .m......2Z.=232.
+  0x0000a368 00034605 2737387b 030afd11 13321f03 ..F.'78{.....2..
+  0x0000a378 1f376d06 01029a08 0446002f 38338d00 .7m......F./83..
+  0x0000a388 0402e408 37323836 8d000e12 2f123233 ....7286..../.23
+  0x0000a398 12283238 6d062938 348d0002 35122f32 .(28m.)84...5./2
+  0x0000a3a8 386d0601 029a0804 46000fcf 2c051332 8m......F...,..2
+  0x0000a3b8 32122839 338d000e c10202cd 11283239 2.(93........(29
+  0x0000a3c8 6d060ad5 2c1232cd 112f3239 6d060102 m...,.2../29m...
+  0x0000a3d8 9a082f32 346d0603 02db0827 32346d06 ../24m.....'24m.
+  0x0000a3e8 0dc21112 33e40828 32356d06 0dc41112 ....3..(25m.....
+  0x0000a3f8 33a80527 32356d06 1d33c511 1233a805 3..'25m..3...3..
+  0x0000a408 2732356d 063d3330 31260018 33920312 '25m.=301&..3...
+  0x0000a418 3726001d 32260018 344e0312 3926001d 7&..2&..4N..9&..
+  0x0000a428 33260018 35510303 72001d34 26001736 3&..5Q..r..4&..6
+  0x0000a438 0d0302ea 003d3330 35260017 37100302 .....=305&..7...
+  0x0000a448 33033d33 30362600 1838cc02 12312600 3.=306&..8...1&.
+  0x0000a458 1d372600 1839cf02 0372000d 7c01024f .7&..9...r..|..O
+  0x0000a468 0e273238 6d063d33 30392600 18318e02 .'28m.=309&..1..
+  0x0000a478 0272002d 31302600 18324a02 12332600 .r.-10&..2J..3&.
+  0x0000a488 0f6d0604 23333120 00076d06 15321316 .m..#31 ..m..2..
+  0x0000a498 025c0212 330c022e 33316d06 1233950e .\..3...31m..3..
+  0x0000a4a8 2e33316d 06123385 09053d00 0f6d0604 .31m..3...=..m..
+  0x0000a4b8 1233cf09 2833326d 0601c413 0ad50003 .3..(32m........
+  0x0000a4c8 d80e2732 30770229 31398c00 03d50e1f ..'20w.)19......
+  0x0000a4d8 326d0600 1233cb09 0546000f 6d060413 2m...3...F..m...
+  0x0000a4e8 33840227 32388d00 0ed11312 33710903 3..'28......3q..
+  0x0000a4f8 2e000434 00096d06 12336e09 2f33326d ...4..m..3n./32m
+  0x0000a508 06001333 351b0346 000f371b 06031f16 ...35..F..7.....
+  0x0000a518 09391b0e d2131333 ec022733 34f9020a .9.....3..'34...
+  0x0000a528 dc1a1333 35031f33 6d060012 33e70805 ...35..3m...3...
+  0x0000a538 46000f6d 06041233 e8082833 346d060e F..m...3..(34m..
+  0x0000a548 d3131233 9b0f032e 00033a03 2934308d ...3......:.)40.
+  0x0000a558 0002980f 2f33346d 06001233 9a080546 ..../34m...3...F
+  0x0000a568 000f6d06 041233e3 08283334 6d060ed4 ..m...3..(34m...
+  0x0000a578 131233dc 0f032e00 037b0329 34378d00 ..3......{.)47..
+  0x0000a588 0226122f 33346d06 0012339a 08044600 .&./34m...3...F.
+  0x0000a598 2f35338d 000402e4 08273335 6d061e33 /53......'35m..3
+  0x0000a5a8 d4131233 5d12032e 0003bc03 2935348d ...3].......)54.
+  0x0000a5b8 0003a300 1f356d06 00133360 04034600 .....5m...3`..F.
+  0x0000a5c8 2f36308d 000402e4 08273336 6d061e33 /60......'36m..3
+  0x0000a5d8 d4131233 e1112733 366d063a 3336318d ...3..'36m.:361.
+  0x0000a5e8 0013374a 000e6d06 12339a08 2f33316d ..7J..m..3../31m
+  0x0000a5f8 06021233 db082633 316d061d 33cb1112 ...3..&31m..3...
+  0x0000a608 33e40827 33326d06 1d33cb11 38333731 3..'32m..3..8371
+  0x0000a618 d303024c 000dcb11 38333732 8f03029c ...L....8372....
+  0x0000a628 002d3731 26001833 92030272 002d3732 .-71&..3...r.-72
+  0x0000a638 26001834 4e0302ca 001d376d 06020e09 &..4N.....7m....
+  0x0000a648 2833336d 061d376d 06025709 2833346d (33m..7m..W.(34m
+  0x0000a658 061d372f 01026109 2833346d 062d3736 ..7/..a.(34m.-76
+  0x0000a668 26001838 cc021231 26000d6d 06026606 &..8...1&..m..f.
+  0x0000a678 2833346d 060d8e36 38333830 8b02023d (34m...68380...=
+  0x0000a688 012d3739 26001831 8e02020d 000d9436 .-79&..1.......6
+  0x0000a698 38333832 4a020263 012f3831 9e020404 8382J..c./81....
+  0x0000a6a8 20001834 281f2930 5d5c0202 a00e2f33  ..4(.)0]\..../3
+  0x0000a6b8 386d0600 02950e2f 33386d06 00028509 8m...../38m.....
+  0x0000a6c8 053d000f 6d060502 cf093833 39318100 .=..m.....8391..
+  0x0000a6d8 0ec60404 d80e1730 77022938 398c0004 .......0w.)89...
+  0x0000a6e8 26120f6d 060102cb 09054600 0f6d0605 &..m......F..m..
+  0x0000a6f8 02cf0927 33396d06 1e33d413 12347109 ...'39m..3...4q.
+  0x0000a708 032e0003 b8022839 368d0012 346e092f ......(96...4n./
+  0x0000a718 33396d06 00123464 09034600 3f343032 39m...4d..F.?402
+  0x0000a728 8d000312 34650927 34306d06 1e33d413 ....4e.'40m..3..
+  0x0000a738 1234f408 032e0013 330d0009 1d041234 .4......3......4
+  0x0000a748 f1081234 90090a6d 061234e7 08054600 ...4...m..4...F.
+  0x0000a758 0f6d0604 1234e808 2734316d 061e33d4 .m...4..'41m..3.
+  0x0000a768 1312349b 0f273431 6d063934 31308d00 ..4..'41m.9410..
+  0x0000a778 02bd012f 34316d06 00123476 04054600 .../41m...4v..F.
+  0x0000a788 0f6d0604 1234e308 2734316d 061e33d4 .m...4..'41m..3.
+  0x0000a798 131234dc 0f032e00 027b0339 3431378d ..4......{.9417.
+  0x0000a7a8 00022612 2f34316d 06001234 9a080446 ..&./41m...4...F
+  0x0000a7b8 002f3233 8d000402 e4083834 32368d00 ./23......8426..
+  0x0000a7c8 0dc10212 345d1227 34326d06 39343234 ....4].'42m.9424
+  0x0000a7d8 8d00025b 122f3432 6d060012 349a0804 ...[./42m...4...
+  0x0000a7e8 46002f33 308d0004 02e40837 3433338d F./30......7433.
+  0x0000a7f8 000ed413 1234e111 2734336d 063a3433 .....4..'43m.:43
+  0x0000a808 318d0013 374a000e 6d062834 33f6030c 1...7J..m.(43...
+  0x0000a818 6d063734 33392f04 0369000c f1043834 m.7439/..i....84
+  0x0000a828 3430d003 036c001d 39260018 31d30302 40...l..9&..1...
+  0x0000a838 4c000dcb 111234a8 05273339 6d063d34 L.....4..'39m.=4
+  0x0000a848 34312600 18339203 0272002d 34322600 41&..3...r.-42&.
+  0x0000a858 18344e03 026e012d 34332600 18355103 .4N..n.-43&..5Q.
+  0x0000a868 0372001d 34260017 360d0302 6d063d34 .r..4&..6...m.=4
+  0x0000a878 34352600 17371003 0333030d cc361234 45&..7...3...6.4
+  0x0000a888 66062734 316d063d 34343726 001839cf f.'41m.=447&..9.
+  0x0000a898 02037200 0d7c0128 35308b02 0278002d ..r..|.(50...x.-
+  0x0000a8a8 34392600 18318e02 020d002d 35302600 49&..1.....-50&.
+  0x0000a8b8 18324a02 12332600 0f6d0604 23343520 .2J..3&..m..#45 
+  0x0000a8c8 00086d06 01e51507 5c0202a0 0e2e3435 ..m.....\.....45
+  0x0000a8d8 6d061234 950e2e34 356d0612 34850905 m..4...45m..4...
+  0x0000a8e8 3d000f6d 06041334 13012736 31810001 =..m...4..'61...
+  0x0000a8f8 c8130ad5 0002d80e 032e0003 77022935 ............w.)5
+  0x0000a908 398c0002 d50e2f34 366d0600 1234cb09 9...../46m...4..
+  0x0000a918 0546000f 6d060412 34cf0919 34dd240e .F..m...4...4.$.
+  0x0000a928 d4131334 7b012736 37b8020a 80241334 ...4{.'67....$.4
+  0x0000a938 c4011f36 6d060102 64090446 002f3732 ...6m...d..F./72
+  0x0000a948 8d000402 65093834 37358d00 0ec60402 ....e.8475......
+  0x0000a958 f408032e 0003f902 2a37338d 0013394a ........*73...9J
+  0x0000a968 000f6d06 0002e708 0546000f 6d060502 ..m......F..m...
+  0x0000a978 e8082734 386d061e 34d41312 349b0f28 ..'48m..4...4..(
+  0x0000a988 34386d06 2938308d 0002980f 2f34386d 48m.)80...../48m
+  0x0000a998 0601029a 08054600 0f6d0605 02e30827 ......F..m.....'
+  0x0000a9a8 34386d06 1e34d413 1234dc0f 032e0003 48m..4...4......
+  0x0000a9b8 7b031a38 6d060226 122f3438 6d060102 {..8m..&./48m...
+  0x0000a9c8 9a080446 002f3933 8d000402 e4082734 ...F./93......'4
+  0x0000a9d8 396d061e 34d41312 345d1228 34396d06 9m..4...4].(49m.
+  0x0000a9e8 2839348d 0012355b 122f3439 6d060013 (94...5[./49m...
+  0x0000a9f8 359a0802 46003f35 30308d00 031235e4 5...F.?500....5.
+  0x0000aa08 08273530 6d061e34 d4131235 e1112735 .'50m..4...5..'5
+  0x0000aa18 306d063a 3530318d 00123716 000f6d06 0m.:501...7...m.
+  0x0000aa28 00283530 f6030c6d 06373530 392f0403 .(50...m.7509/..
+  0x0000aa38 69000cf1 04383531 30d00303 6c001d39 i....8510...l..9
+  0x0000aa48 26001831 d303024c 000dcb11 38353132 &..1...L....8512
+  0x0000aa58 8f031238 26001d31 26001833 92030272 ...8&..1&..3...r
+  0x0000aa68 002d3132 26001834 4e03026e 012d3133 .-12&..4N..n.-13
+  0x0000aa78 26001835 51030372 001d3426 0017360d &..5Q..r..4&..6.
+  0x0000aa88 0302e205 3d353135 26001737 10030233 ....=515&..7...3
+  0x0000aa98 033d3531 36260018 38cc0202 52002d31 .=516&..8...R.-1
+  0x0000aaa8 37260018 39cf0203 72000d7c 01024f0e 7&..9...r..|..O.
+  0x0000aab8 2734396d 063d3531 39260018 318e0202 '49m.=519&..1...
+  0x0000aac8 72002d32 30260018 324a0212 3326000f r.-20&..2J..3&..
+  0x0000aad8 6d060423 35322000 18349e02 29385d5c m..#52 ..4..)8]\
+  0x0000aae8 02039a01 1e326d06 1335db01 1e326d06 .....2m..5...2m.
+  0x0000aaf8 12358509 053d000f 6d060412 35cf0927 .5...=..m...5..'
+  0x0000ab08 35336d06 1134c813 0ad50002 d80e032e 53m..4..........
+  0x0000ab18 00037702 2932398c 0002d50e 2f35336d ..w.)29...../53m
+  0x0000ab28 06001235 cb090546 000f6d06 041235cf ...5...F..m...5.
+  0x0000ab38 09283533 6d060ed4 13133519 0f273337 .(53m.....5..'37
+  0x0000ab48 b8022933 368d0002 6e092f35 336d0600 ..)36...n./53m..
+  0x0000ab58 12356409 0446002f 34328d00 04031317 .5d..F./42......
+  0x0000ab68 18346d06 0ed41312 35f40803 2e0003f9 .4m.....5.......
+  0x0000ab78 022a3433 8d001339 4a000e6d 06133505 .*43...9J..m..5.
+  0x0000ab88 03044600 0f6d0604 1235e808 37353532 ..F..m...5..7552
+  0x0000ab98 8d000ed4 1312359b 0f032e00 03770029 ......5......w.)
+  0x0000aba8 35308d00 02980f2f 35356d06 0012359a 50...../55m...5.
+  0x0000abb8 08054600 0f6d0604 1235e308 38353539 ..F..m...5..8559
+  0x0000abc8 8d000d87 071235dc 0f032e00 037b030a ......5......{..
+  0x0000abd8 3c481235 26122f35 356d0600 12359a08 <H.5&./55m...5..
+  0x0000abe8 0446002f 36338d00 0402e408 37353636 .F./63......7566
+  0x0000abf8 8d000ed4 1312355d 12032e00 03bc030a ......5]........
+  0x0000ac08 47481235 5b122f35 366d0601 04320002 GH.5[./56m...2..
+  0x0000ac18 46002f37 308d0004 033b0406 4e483e34 F./70....;..NH>4
+  0x0000ac28 2b35d413 1235e111 2835376d 062a3731 +5...5..(57m.*71
+  0x0000ac38 8d001337 4a000f6d 0600029a 082f3532 ...7J..m...../52
+  0x0000ac48 6d060302 db082735 326d060d cb111235 m.....'52m.....5
+  0x0000ac58 e4082835 336d060d cb113835 3831d303 ..(53m....8581..
+  0x0000ac68 024c000d cb113835 38328f03 029c000d .L....8582......
+  0x0000ac78 62483835 38339203 0272000d 65483835 bH8583...r..eH85
+  0x0000ac88 38344e03 02ca002d 38332600 18355103 84N....-83&..5Q.
+  0x0000ac98 0372000d 6d060257 09030d03 0368032d .r..m..W.....h.-
+  0x0000aca8 38352600 17371003 0333032d 38362600 85&..7...3.-86&.
+  0x0000acb8 1838cc02 0252002d 38372600 1839cf02 .8...R.-87&..9..
+  0x0000acc8 0372000d 7c012839 308b0202 3d010d53 .r..|.(90...=..S
+  0x0000acd8 2e383539 318e0202 0d000d56 2e12358b .8591......V..5.
+  0x0000ace8 09283537 6d060d59 2e373539 33192f12 .(57m..Y.7593./.
+  0x0000acf8 32ad280a e0022639 34cc472f 3837d142 2.(...&94.G/87.B
+  0x0000ad08 0c032e00 2d3539a7 43123542 07044529 ....-59.C.5B..E)
+  0x0000ad18 026b000b 4b03023f 07059229 1f37d142 .k..K..?...).7.B
+  0x0000ad28 0c033000 2d3539ab 43293539 45231232 ..0.-59.C)59E#.2
+  0x0000ad38 ab1c0b6d 0028382c 92230f6d 00052432 ...m.(8,.#.m..$2
+  0x0000ad48 316d0022 382c5a00 0e6d0018 39451d12 1m."8,Z..m..9E..
+  0x0000ad58 32ab1609 6d001336 091d0492 1d0f6d00 2...m..6......m.
+  0x0000ad68 0603ee44 0330003c 3539396d 001236dc ...D.0.<599m..6.
+  0x0000ad78 0a283336 6d001b38 6d002832 2c92170f .(36m..8m.(2,...
+  0x0000ad88 6d000603 f2440330 002d3630 44593836 m....D.0.-60DY86
+  0x0000ad98 30334511 1232ab0a 0b6d0028 342c9211 03E..2...m.(4,..
+  0x0000ada8 0f6d0006 03210203 30002d36 30210212 .m...!..0.-60!..
+  0x0000adb8 368e1027 35306d00 2b35326d 0028362c 6..'50m.+52m.(6,
+  0x0000adc8 920b0f6d 00060321 02033000 2d363021 ...m...!..0.-60!
+  0x0000add8 02293630 4505026d 001b396d 0028382c .)60E..m..9m.(8,
+  0x0000ade8 92050f6d 00051333 21020330 00363630 ...m...3!..0.660
+  0x0000adf8 375f4515 325f4550 0a7d0a0a 00000000 7_E.2_EP.}......
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,30 +1,30 @@
 
 Hex dump of section '.eh_frame_hdr':
-  0x0000ade8 011b033b ac010000 34000000 886dffff ...;....4....m..
-  0x0000adf8 c8010000 b871ffff 18080000 3873ffff .....q......8s..
-  0x0000ae08 f0010000 4873ffff 08020000 5873ffff ....Hs......Xs..
-  0x0000ae18 20020000 7873ffff 38020000 9873ffff  ...xs..8....s..
-  0x0000ae28 50020000 b873ffff 68020000 d873ffff P....s..h....s..
-  0x0000ae38 80020000 f873ffff 98020000 1874ffff .....s.......t..
-  0x0000ae48 b0020000 3874ffff c8020000 5874ffff ....8t......Xt..
-  0x0000ae58 e0020000 c874ffff 00030000 3875ffff .....t......8u..
-  0x0000ae68 20030000 9875ffff 40030000 2876ffff  ....u..@...(v..
-  0x0000ae78 58030000 a876ffff 70030000 2877ffff X....v..p...(w..
-  0x0000ae88 90030000 6877ffff a8030000 b877ffff ....hw.......w..
-  0x0000ae98 c0030000 2878ffff e0030000 6878ffff ....(x......hx..
-  0x0000aea8 f8030000 a878ffff 10040000 e878ffff .....x.......x..
-  0x0000aeb8 28040000 b879ffff 48040000 887affff (....y..H....z..
-  0x0000aec8 68040000 587bffff 88040000 a87bffff h...X{.......{..
-  0x0000aed8 a0040000 187cffff b8040000 b87dffff .....|.......}..
-  0x0000aee8 d0040000 587fffff e8040000 f880ffff ....X...........
-  0x0000aef8 00050000 9882ffff 18050000 3884ffff ............8...
-  0x0000af08 30050000 a884ffff 48050000 f884ffff 0.......H.......
-  0x0000af18 60050000 1886ffff 78050000 4886ffff `.......x...H...
-  0x0000af28 90050000 a886ffff d0050000 d886ffff ................
-  0x0000af38 e8050000 d888ffff 00060000 788bffff ............x...
-  0x0000af48 50060000 488cffff 80060000 588cffff P...H.......X...
-  0x0000af58 98060000 b891ffff e8060000 8892ffff ................
-  0x0000af68 18070000 9892ffff 30070000 6897ffff ........0...h...
-  0x0000af78 80070000 3898ffff b0070000 4898ffff ....8.......H...
-  0x0000af88 c8070000 689cffff 60080000          ....h...`...
+  0x0000ae08 011b033b ac010000 34000000 686dffff ...;....4...hm..
+  0x0000ae18 c8010000 9871ffff 18080000 1873ffff .....q.......s..
+  0x0000ae28 f0010000 2873ffff 08020000 3873ffff ....(s......8s..
+  0x0000ae38 20020000 5873ffff 38020000 7873ffff  ...Xs..8...xs..
+  0x0000ae48 50020000 9873ffff 68020000 b873ffff P....s..h....s..
+  0x0000ae58 80020000 d873ffff 98020000 f873ffff .....s.......s..
+  0x0000ae68 b0020000 1874ffff c8020000 3874ffff .....t......8t..
+  0x0000ae78 e0020000 a874ffff 00030000 1875ffff .....t.......u..
+  0x0000ae88 20030000 7875ffff 40030000 0876ffff  ...xu..@....v..
+  0x0000ae98 58030000 8876ffff 70030000 0877ffff X....v..p....w..
+  0x0000aea8 90030000 4877ffff a8030000 9877ffff ....Hw.......w..
+  0x0000aeb8 c0030000 0878ffff e0030000 4878ffff .....x......Hx..
+  0x0000aec8 f8030000 8878ffff 10040000 c878ffff .....x.......x..
+  0x0000aed8 28040000 9879ffff 48040000 687affff (....y..H...hz..
+  0x0000aee8 68040000 387bffff 88040000 887bffff h...8{.......{..
+  0x0000aef8 a0040000 f87bffff b8040000 987dffff .....{.......}..
+  0x0000af08 d0040000 387fffff e8040000 d880ffff ....8...........
+  0x0000af18 00050000 7882ffff 18050000 1884ffff ....x...........
+  0x0000af28 30050000 8884ffff 48050000 d884ffff 0.......H.......
+  0x0000af38 60050000 f885ffff 78050000 2886ffff `.......x...(...
+  0x0000af48 90050000 8886ffff d0050000 b886ffff ................
+  0x0000af58 e8050000 b888ffff 00060000 688bffff ............h...
+  0x0000af68 50060000 388cffff 80060000 488cffff P...8.......H...
+  0x0000af78 98060000 a891ffff e8060000 7892ffff ............x...
+  0x0000af88 18070000 8892ffff 30070000 5897ffff ........0...X...
+  0x0000af98 80070000 2898ffff b0070000 3898ffff ....(.......8...
+  0x0000afa8 c8070000 589cffff 60080000          ....X...`...
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,112 +1,112 @@
 
 Hex dump of section '.eh_frame':
-  0x0000af98 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x0000afa8 1b0c0708 90010000 24000000 1c000000 ........$.......
-  0x0000afb8 b86bffff 30040000 000e1046 0e184a0f .k..0......F..J.
-  0x0000afc8 0b770880 003f1a3b 2a332422 00000000 .w...?.;*3$"....
-  0x0000afd8 14000000 44000000 4071ffff 05000000 ....D...@q......
-  0x0000afe8 00000000 00000000 14000000 5c000000 ............\...
-  0x0000aff8 3871ffff 0c000000 00000000 00000000 8q..............
-  0x0000b008 14000000 74000000 3071ffff 17000000 ....t...0q......
-  0x0000b018 00000000 00000000 14000000 8c000000 ................
-  0x0000b028 3871ffff 16000000 00000000 00000000 8q..............
-  0x0000b038 14000000 a4000000 4071ffff 17000000 ........@q......
-  0x0000b048 00000000 00000000 14000000 bc000000 ................
-  0x0000b058 4871ffff 17000000 00000000 00000000 Hq..............
-  0x0000b068 14000000 d4000000 5071ffff 17000000 ........Pq......
-  0x0000b078 00000000 00000000 14000000 ec000000 ................
-  0x0000b088 5871ffff 17000000 00000000 00000000 Xq..............
-  0x0000b098 14000000 04010000 6071ffff 17000000 ........`q......
-  0x0000b0a8 00000000 00000000 14000000 1c010000 ................
-  0x0000b0b8 6871ffff 16000000 00000000 00000000 hq..............
-  0x0000b0c8 1c000000 34010000 7071ffff 61000000 ....4...pq..a...
-  0x0000b0d8 00410e10 8302470e 2002570e 10410e08 .A....G. .W..A..
-  0x0000b0e8 1c000000 54010000 c071ffff 6a000000 ....T....q..j...
-  0x0000b0f8 00410e10 8302470e 2002600e 10410e08 .A....G. .`..A..
-  0x0000b108 1c000000 74010000 1072ffff 5e000000 ....t....r..^...
-  0x0000b118 00410e10 8302470e 2002540e 10410e08 .A....G. .T..A..
-  0x0000b128 14000000 94010000 5072ffff 83000000 ........Pr......
-  0x0000b138 0002540e 206e0e08 14000000 ac010000 ..T. n..........
-  0x0000b148 c872ffff 78000000 00024c0e 206b0e08 .r..x.....L. k..
-  0x0000b158 1c000000 c4010000 3073ffff 75000000 ........0s..u...
-  0x0000b168 00640e20 730a0e08 410b0000 00000000 .d. s...A.......
-  0x0000b178 14000000 e4010000 9073ffff 33000000 .........s..3...
-  0x0000b188 00000000 00000000 14000000 fc010000 ................
-  0x0000b198 b873ffff 41000000 00000000 00000000 .s..A...........
-  0x0000b1a8 1c000000 14020000 f073ffff 69000000 .........s..i...
-  0x0000b1b8 00410e10 8302470e 20025f0e 10410e08 .A....G. ._..A..
-  0x0000b1c8 14000000 34020000 4074ffff 33000000 ....4...@t..3...
-  0x0000b1d8 00000000 00000000 14000000 4c020000 ............L...
-  0x0000b1e8 6874ffff 33000000 00000000 00000000 ht..3...........
-  0x0000b1f8 14000000 64020000 9074ffff 3a000000 ....d....t..:...
-  0x0000b208 00000000 00000000 1c000000 7c020000 ............|...
-  0x0000b218 b874ffff c5000000 00410e10 8302470e .t.......A....G.
-  0x0000b228 2002bb0e 10410e08 1c000000 9c020000  ....A..........
-  0x0000b238 6875ffff c8000000 00410e10 8302470e hu.......A....G.
-  0x0000b248 2002be0e 10410e08 1c000000 bc020000  ....A..........
-  0x0000b258 1876ffff c2000000 00410e10 8302470e .v.......A....G.
-  0x0000b268 2002b80e 10410e08 14000000 dc020000  ....A..........
-  0x0000b278 c876ffff 41000000 00000000 00000000 .v..A...........
-  0x0000b288 14000000 f4020000 0077ffff 65000000 .........w..e...
-  0x0000b298 00000000 00000000 14000000 0c030000 ................
-  0x0000b2a8 5877ffff 92010000 00000000 00000000 Xw..............
-  0x0000b2b8 14000000 24030000 e078ffff a0010000 ....$....x......
-  0x0000b2c8 00000000 00000000 14000000 3c030000 ............<...
-  0x0000b2d8 687affff a0010000 00000000 00000000 hz..............
-  0x0000b2e8 14000000 54030000 f07bffff a0010000 ....T....{......
-  0x0000b2f8 00000000 00000000 14000000 6c030000 ............l...
-  0x0000b308 787dffff a0010000 00000000 00000000 x}..............
-  0x0000b318 14000000 84030000 007fffff 6b000000 ............k...
-  0x0000b328 00000000 00000000 14000000 9c030000 ................
-  0x0000b338 587fffff 41000000 00440e20 7c0e0800 X...A....D. |...
-  0x0000b348 14000000 b4030000 907fffff 1e010000 ................
-  0x0000b358 00000000 00000000 14000000 cc030000 ................
-  0x0000b368 9880ffff 2f000000 00000000 00000000 ..../...........
-  0x0000b378 3c000000 e4030000 b080ffff 52000000 <...........R...
-  0x0000b388 00490e10 8c02460e 18860344 0e208304 .I....F....D. ..
-  0x0000b398 660a0e18 460e1042 0e08470b 410e1843 f...F..B..G.A..C
-  0x0000b3a8 0e10420e 0841c3c6 cc000000 00000000 ..B..A..........
-  0x0000b3b8 14000000 24040000 d080ffff 21000000 ....$.......!...
-  0x0000b3c8 00000000 00000000 14000000 3c040000 ............<...
-  0x0000b3d8 e880ffff fe010000 00000000 00000000 ................
-  0x0000b3e8 4c000000 54040000 d082ffff 96020000 L...T...........
-  0x0000b3f8 00420e10 8f02530e 188e0353 0e208d04 .B....S....S. ..
-  0x0000b408 520e288c 05520e30 8606500e 38830766 R.(..R.0..P.8..f
-  0x0000b418 0ea00203 dd010a0e 38410e30 410e2842 ........8A.0A.(B
-  0x0000b428 0e20420e 18420e10 420e0847 0b000000 . B..B..B..G....
-  0x0000b438 2c000000 a4040000 2085ffff c9000000 ,....... .......
-  0x0000b448 00470e90 0102900e 98014b0e a0015e0e .G........K...^.
-  0x0000b458 9801410e 9001470e 08000000 00000000 ..A...G.........
-  0x0000b468 14000000 d4040000 c085ffff 05000000 ................
-  0x0000b478 00000000 00000000 4c000000 ec040000 ........L.......
-  0x0000b488 b885ffff 5d050000 00420e10 8f02490e ....]....B....I.
-  0x0000b498 188e0351 0e208d04 4d0e288c 054f0e30 ...Q. ..M.(..O.0
-  0x0000b4a8 8606500e 38830772 0e800203 c5020a0e ..P.8..r........
-  0x0000b4b8 38440e30 410e2842 0e20420e 18420e10 8D.0A.(B. B..B..
-  0x0000b4c8 420e084c 0b000000 2c000000 3c050000 B..L....,...<...
-  0x0000b4d8 c88affff c9000000 00470e90 0102900e .........G......
-  0x0000b4e8 98014b0e a0015e0e 9801410e 9001470e ..K...^...A...G.
-  0x0000b4f8 08000000 00000000 14000000 6c050000 ............l...
-  0x0000b508 688bffff 05000000 00000000 00000000 h...............
-  0x0000b518 4c000000 84050000 608bffff cb040000 L.......`.......
-  0x0000b528 00420e10 8f02490e 188e0351 0e208d04 .B....I....Q. ..
-  0x0000b538 4f0e288c 05500e30 86064d0e 38830756 O.(..P.0..M.8..V
-  0x0000b548 0ee00103 ba020a0e 38440e30 410e2842 ........8D.0A.(B
-  0x0000b558 0e20420e 18420e10 420e084b 0b000000 . B..B..B..K....
-  0x0000b568 2c000000 d4050000 e08fffff c9000000 ,...............
-  0x0000b578 00470e90 0102900e 98014b0e a0015e0e .G........K...^.
-  0x0000b588 9801410e 9001470e 08000000 00000000 ..A...G.........
-  0x0000b598 14000000 04060000 8090ffff 05000000 ................
-  0x0000b5a8 00000000 00000000 4c000000 1c060000 ........L.......
-  0x0000b5b8 7890ffff 19040000 00420e10 8f02490e x........B....I.
-  0x0000b5c8 188e034d 0e208d04 450e288c 05410e30 ...M. ..E.(..A.0
-  0x0000b5d8 8606440e 38830747 0ea00103 53020a0e ..D.8..G....S...
-  0x0000b5e8 38440e30 410e2842 0e20420e 18420e10 8D.0A.(B. B..B..
-  0x0000b5f8 420e0847 0b000000 44000000 6c060000 B..G....D...l...
-  0x0000b608 9869ffff ba000000 00410e10 86024e0e .i.......A....N.
-  0x0000b618 184b0e20 4f0e284c 0e30500e 10480e18 .K. O.(L.0P..H..
-  0x0000b628 560e2045 0e28420e 30490e10 480e1856 V. E.(B.0I..H..V
-  0x0000b638 0e20450e 28420e30 500e104d 0e080000 . E.(B.0P..M....
-  0x0000b648 14000000 b4060000 0094ffff 0e000000 ................
-  0x0000b658 00000000 00000000 00000000          ............
+  0x0000afb8 14000000 00000000 017a5200 01781001 .........zR..x..
+  0x0000afc8 1b0c0708 90010000 24000000 1c000000 ........$.......
+  0x0000afd8 986bffff 30040000 000e1046 0e184a0f .k..0......F..J.
+  0x0000afe8 0b770880 003f1a3b 2a332422 00000000 .w...?.;*3$"....
+  0x0000aff8 14000000 44000000 2071ffff 05000000 ....D... q......
+  0x0000b008 00000000 00000000 14000000 5c000000 ............\...
+  0x0000b018 1871ffff 0c000000 00000000 00000000 .q..............
+  0x0000b028 14000000 74000000 1071ffff 17000000 ....t....q......
+  0x0000b038 00000000 00000000 14000000 8c000000 ................
+  0x0000b048 1871ffff 16000000 00000000 00000000 .q..............
+  0x0000b058 14000000 a4000000 2071ffff 17000000 ........ q......
+  0x0000b068 00000000 00000000 14000000 bc000000 ................
+  0x0000b078 2871ffff 17000000 00000000 00000000 (q..............
+  0x0000b088 14000000 d4000000 3071ffff 17000000 ........0q......
+  0x0000b098 00000000 00000000 14000000 ec000000 ................
+  0x0000b0a8 3871ffff 17000000 00000000 00000000 8q..............
+  0x0000b0b8 14000000 04010000 4071ffff 17000000 ........@q......
+  0x0000b0c8 00000000 00000000 14000000 1c010000 ................
+  0x0000b0d8 4871ffff 16000000 00000000 00000000 Hq..............
+  0x0000b0e8 1c000000 34010000 5071ffff 61000000 ....4...Pq..a...
+  0x0000b0f8 00410e10 8302470e 2002570e 10410e08 .A....G. .W..A..
+  0x0000b108 1c000000 54010000 a071ffff 6a000000 ....T....q..j...
+  0x0000b118 00410e10 8302470e 2002600e 10410e08 .A....G. .`..A..
+  0x0000b128 1c000000 74010000 f071ffff 5e000000 ....t....q..^...
+  0x0000b138 00410e10 8302470e 2002540e 10410e08 .A....G. .T..A..
+  0x0000b148 14000000 94010000 3072ffff 83000000 ........0r......
+  0x0000b158 0002540e 206e0e08 14000000 ac010000 ..T. n..........
+  0x0000b168 a872ffff 78000000 00024c0e 206b0e08 .r..x.....L. k..
+  0x0000b178 1c000000 c4010000 1073ffff 75000000 .........s..u...
+  0x0000b188 00640e20 730a0e08 410b0000 00000000 .d. s...A.......
+  0x0000b198 14000000 e4010000 7073ffff 33000000 ........ps..3...
+  0x0000b1a8 00000000 00000000 14000000 fc010000 ................
+  0x0000b1b8 9873ffff 41000000 00000000 00000000 .s..A...........
+  0x0000b1c8 1c000000 14020000 d073ffff 69000000 .........s..i...
+  0x0000b1d8 00410e10 8302470e 20025f0e 10410e08 .A....G. ._..A..
+  0x0000b1e8 14000000 34020000 2074ffff 33000000 ....4... t..3...
+  0x0000b1f8 00000000 00000000 14000000 4c020000 ............L...
+  0x0000b208 4874ffff 33000000 00000000 00000000 Ht..3...........
+  0x0000b218 14000000 64020000 7074ffff 3a000000 ....d...pt..:...
+  0x0000b228 00000000 00000000 1c000000 7c020000 ............|...
+  0x0000b238 9874ffff c5000000 00410e10 8302470e .t.......A....G.
+  0x0000b248 2002bb0e 10410e08 1c000000 9c020000  ....A..........
+  0x0000b258 4875ffff c8000000 00410e10 8302470e Hu.......A....G.
+  0x0000b268 2002be0e 10410e08 1c000000 bc020000  ....A..........
+  0x0000b278 f875ffff c2000000 00410e10 8302470e .u.......A....G.
+  0x0000b288 2002b80e 10410e08 14000000 dc020000  ....A..........
+  0x0000b298 a876ffff 41000000 00000000 00000000 .v..A...........
+  0x0000b2a8 14000000 f4020000 e076ffff 65000000 .........v..e...
+  0x0000b2b8 00000000 00000000 14000000 0c030000 ................
+  0x0000b2c8 3877ffff 92010000 00000000 00000000 8w..............
+  0x0000b2d8 14000000 24030000 c078ffff a0010000 ....$....x......
+  0x0000b2e8 00000000 00000000 14000000 3c030000 ............<...
+  0x0000b2f8 487affff a0010000 00000000 00000000 Hz..............
+  0x0000b308 14000000 54030000 d07bffff a0010000 ....T....{......
+  0x0000b318 00000000 00000000 14000000 6c030000 ............l...
+  0x0000b328 587dffff a0010000 00000000 00000000 X}..............
+  0x0000b338 14000000 84030000 e07effff 6b000000 .........~..k...
+  0x0000b348 00000000 00000000 14000000 9c030000 ................
+  0x0000b358 387fffff 41000000 00440e20 7c0e0800 8...A....D. |...
+  0x0000b368 14000000 b4030000 707fffff 1e010000 ........p.......
+  0x0000b378 00000000 00000000 14000000 cc030000 ................
+  0x0000b388 7880ffff 2f000000 00000000 00000000 x.../...........
+  0x0000b398 3c000000 e4030000 9080ffff 52000000 <...........R...
+  0x0000b3a8 00490e10 8c02460e 18860344 0e208304 .I....F....D. ..
+  0x0000b3b8 660a0e18 460e1042 0e08470b 410e1843 f...F..B..G.A..C
+  0x0000b3c8 0e10420e 0841c3c6 cc000000 00000000 ..B..A..........
+  0x0000b3d8 14000000 24040000 b080ffff 21000000 ....$.......!...
+  0x0000b3e8 00000000 00000000 14000000 3c040000 ............<...
+  0x0000b3f8 c880ffff fe010000 00000000 00000000 ................
+  0x0000b408 4c000000 54040000 b082ffff a6020000 L...T...........
+  0x0000b418 00420e10 8f02530e 188e034e 0e208d04 .B....S....N. ..
+  0x0000b428 4e0e288c 05500e30 8606500e 38830771 N.(..P.0..P.8..q
+  0x0000b438 0ea00203 ed010a0e 38410e30 410e2842 ........8A.0A.(B
+  0x0000b448 0e20420e 18420e10 420e0847 0b000000 . B..B..B..G....
+  0x0000b458 2c000000 a4040000 1085ffff c9000000 ,...............
+  0x0000b468 00470e90 0102900e 98014b0e a0015e0e .G........K...^.
+  0x0000b478 9801410e 9001470e 08000000 00000000 ..A...G.........
+  0x0000b488 14000000 d4040000 b085ffff 05000000 ................
+  0x0000b498 00000000 00000000 4c000000 ec040000 ........L.......
+  0x0000b4a8 a885ffff 5d050000 00420e10 8f02490e ....]....B....I.
+  0x0000b4b8 188e0351 0e208d04 4d0e288c 054f0e30 ...Q. ..M.(..O.0
+  0x0000b4c8 8606500e 38830772 0e800203 c5020a0e ..P.8..r........
+  0x0000b4d8 38440e30 410e2842 0e20420e 18420e10 8D.0A.(B. B..B..
+  0x0000b4e8 420e084c 0b000000 2c000000 3c050000 B..L....,...<...
+  0x0000b4f8 b88affff c9000000 00470e90 0102900e .........G......
+  0x0000b508 98014b0e a0015e0e 9801410e 9001470e ..K...^...A...G.
+  0x0000b518 08000000 00000000 14000000 6c050000 ............l...
+  0x0000b528 588bffff 05000000 00000000 00000000 X...............
+  0x0000b538 4c000000 84050000 508bffff cb040000 L.......P.......
+  0x0000b548 00420e10 8f02490e 188e0351 0e208d04 .B....I....Q. ..
+  0x0000b558 4f0e288c 05500e30 86064d0e 38830756 O.(..P.0..M.8..V
+  0x0000b568 0ee00103 ba020a0e 38440e30 410e2842 ........8D.0A.(B
+  0x0000b578 0e20420e 18420e10 420e084b 0b000000 . B..B..B..K....
+  0x0000b588 2c000000 d4050000 d08fffff c9000000 ,...............
+  0x0000b598 00470e90 0102900e 98014b0e a0015e0e .G........K...^.
+  0x0000b5a8 9801410e 9001470e 08000000 00000000 ..A...G.........
+  0x0000b5b8 14000000 04060000 7090ffff 05000000 ........p.......
+  0x0000b5c8 00000000 00000000 4c000000 1c060000 ........L.......
+  0x0000b5d8 6890ffff 19040000 00420e10 8f02490e h........B....I.
+  0x0000b5e8 188e034d 0e208d04 450e288c 05410e30 ...M. ..E.(..A.0
+  0x0000b5f8 8606440e 38830747 0ea00103 53020a0e ..D.8..G....S...
+  0x0000b608 38440e30 410e2842 0e20420e 18420e10 8D.0A.(B. B..B..
+  0x0000b618 420e0847 0b000000 44000000 6c060000 B..G....D...l...
+  0x0000b628 7869ffff ba000000 00410e10 86024e0e xi.......A....N.
+  0x0000b638 184b0e20 4f0e284c 0e30500e 10480e18 .K. O.(L.0P..H..
+  0x0000b648 560e2045 0e28420e 30490e10 480e1856 V. E.(B.0I..H..V
+  0x0000b658 0e20450e 28420e30 500e104d 0e080000 . E.(B.0P..M....
+  0x0000b668 14000000 b4060000 f093ffff 0e000000 ................
+  0x0000b678 00000000 00000000 00000000          ............
```

#### readelf --wide --decompress --hex-dump=.nvFatBinSegment {}

```diff
@@ -1,5 +1,5 @@
 
 Hex dump of section '.nvFatBinSegment':
-  0x0020c230 b1436246 01000000 48510000 00000000 .CbF....HQ......
+  0x0020c230 b1436246 01000000 68510000 00000000 .CbF....hQ......
   0x0020c240 00000000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.strtab':
-  0x00000000 00746d70 7866745f 30303030 35373135 .tmpxft_00005715
+  0x00000000 00746d70 7866745f 30303030 35373732 .tmpxft_00005772
   0x00000010 5f303030 30303030 302d365f 7467715f _00000000-6_tgq_
   0x00000020 73696d75 6c61746f 722e6375 64616665 simulator.cudafe
   0x00000030 312e6370 70006661 7462696e 44617461 1.cpp.fatbinData
   0x00000040 005f5a4c 32365f5f 63756461 556e7265 ._ZL26__cudaUnre
   0x00000050 67697374 65724269 6e617279 5574696c gisterBinaryUtil
   0x00000060 76005f5a 4c32305f 5f637564 61466174 v._ZL20__cudaFat
   0x00000070 43756269 6e48616e 646c6500 5f5a4c32 CubinHandle._ZL2
```

### Comparing `tgqSim-0.1.7/tgqSim.egg-info/PKG-INFO` & `tgqSim-0.1.8/tgqSim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.7
+Version: 0.1.8
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

