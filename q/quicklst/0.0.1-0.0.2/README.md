# Comparing `tmp/quicklst-0.0.1.tar.gz` & `tmp/quicklst-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quicklst-0.0.1.tar", last modified: Tue Mar 28 18:46:56 2023, max compression
+gzip compressed data, was "quicklst-0.0.2.tar", last modified: Wed May 15 01:30:34 2024, max compression
```

## Comparing `quicklst-0.0.1.tar` & `quicklst-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 goes      (1000) goes      (1000)        0 2023-03-28 18:46:56.416713 quicklst-0.0.1/
--rw-r--r--   0 goes      (1000) goes      (1000)     1069 2023-01-26 13:51:29.000000 quicklst-0.0.1/LICENSE
--rw-rw-r--   0 goes      (1000) goes      (1000)       26 2023-03-28 13:27:50.000000 quicklst-0.0.1/MANIFEST.in
--rw-rw-r--   0 goes      (1000) goes      (1000)      956 2023-03-28 18:46:56.416713 quicklst-0.0.1/PKG-INFO
--rw-r--r--   0 goes      (1000) goes      (1000)      432 2023-03-28 11:39:44.000000 quicklst-0.0.1/README.md
--rw-rw-r--   0 goes      (1000) goes      (1000)      749 2023-03-28 14:19:41.000000 quicklst-0.0.1/pyproject.toml
--rw-rw-r--   0 goes      (1000) goes      (1000)       38 2023-03-28 18:46:56.416713 quicklst-0.0.1/setup.cfg
-drwxrwxr-x   0 goes      (1000) goes      (1000)        0 2023-03-28 18:46:56.416713 quicklst-0.0.1/src/
-drwxrwxr-x   0 goes      (1000) goes      (1000)        0 2023-03-28 18:46:56.416713 quicklst-0.0.1/src/quicklst/
--rw-rw-r--   0 goes      (1000) goes      (1000)       23 2023-03-28 14:47:05.000000 quicklst-0.0.1/src/quicklst/__init__.py
--rw-rw-r--   0 goes      (1000) goes      (1000)  1214086 2023-03-28 12:03:06.000000 quicklst-0.0.1/src/quicklst/distortion_map.npz
--rw-r--r--   0 goes      (1000) goes      (1000)    22140 2023-03-28 18:26:01.000000 quicklst-0.0.1/src/quicklst/quicklst.py
-drwxrwxr-x   0 goes      (1000) goes      (1000)        0 2023-03-28 18:46:56.416713 quicklst-0.0.1/src/quicklst.egg-info/
--rw-rw-r--   0 goes      (1000) goes      (1000)      956 2023-03-28 18:46:56.000000 quicklst-0.0.1/src/quicklst.egg-info/PKG-INFO
--rw-rw-r--   0 goes      (1000) goes      (1000)      305 2023-03-28 18:46:56.000000 quicklst-0.0.1/src/quicklst.egg-info/SOURCES.txt
--rw-rw-r--   0 goes      (1000) goes      (1000)        1 2023-03-28 18:46:56.000000 quicklst-0.0.1/src/quicklst.egg-info/dependency_links.txt
--rw-rw-r--   0 goes      (1000) goes      (1000)       23 2023-03-28 18:46:56.000000 quicklst-0.0.1/src/quicklst.egg-info/requires.txt
--rw-rw-r--   0 goes      (1000) goes      (1000)        9 2023-03-28 18:46:56.000000 quicklst-0.0.1/src/quicklst.egg-info/top_level.txt
+drwxr-xr-x   0 jgoes     (1000) jgoes     (1000)        0 2024-05-15 01:30:34.038963 quicklst-0.0.2/
+-rwxrwxrwx   0 jgoes     (1000) jgoes     (1000)     1069 2023-01-26 13:51:29.000000 quicklst-0.0.2/LICENSE
+-rwxrwxrwx   0 jgoes     (1000) jgoes     (1000)       26 2023-03-28 13:27:50.000000 quicklst-0.0.2/MANIFEST.in
+-rw-r--r--   0 jgoes     (1000) jgoes     (1000)     1024 2024-05-15 01:30:34.038963 quicklst-0.0.2/PKG-INFO
+-rwxrwxrwx   0 jgoes     (1000) jgoes     (1000)      432 2023-03-28 11:39:44.000000 quicklst-0.0.2/README.md
+-rwxrwxrwx   0 jgoes     (1000) jgoes     (1000)      749 2024-05-15 01:20:54.000000 quicklst-0.0.2/pyproject.toml
+-rw-r--r--   0 jgoes     (1000) jgoes     (1000)       38 2024-05-15 01:30:34.038963 quicklst-0.0.2/setup.cfg
+drwxr-xr-x   0 jgoes     (1000) jgoes     (1000)        0 2024-05-15 01:30:34.026963 quicklst-0.0.2/src/
+drwxr-xr-x   0 jgoes     (1000) jgoes     (1000)        0 2024-05-15 01:30:34.037963 quicklst-0.0.2/src/quicklst/
+-rwxrwxrwx   0 jgoes     (1000) jgoes     (1000)       23 2023-03-28 14:47:05.000000 quicklst-0.0.2/src/quicklst/__init__.py
+-rwxrwxrwx   0 jgoes     (1000) jgoes     (1000)  1214086 2023-03-28 12:03:06.000000 quicklst-0.0.2/src/quicklst/distortion_map.npz
+-rw-r--r--   0 jgoes     (1000) jgoes     (1000)    21107 2024-05-15 00:56:25.000000 quicklst-0.0.2/src/quicklst/quicklst.py
+drwxr-xr-x   0 jgoes     (1000) jgoes     (1000)        0 2024-05-15 01:30:34.037963 quicklst-0.0.2/src/quicklst.egg-info/
+-rw-r--r--   0 jgoes     (1000) jgoes     (1000)     1024 2024-05-15 01:30:34.000000 quicklst-0.0.2/src/quicklst.egg-info/PKG-INFO
+-rwxrwxrwx   0 jgoes     (1000) jgoes     (1000)      305 2024-05-15 01:30:34.000000 quicklst-0.0.2/src/quicklst.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jgoes     (1000) jgoes     (1000)        1 2024-05-15 01:30:34.000000 quicklst-0.0.2/src/quicklst.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jgoes     (1000) jgoes     (1000)       23 2024-05-15 01:30:34.000000 quicklst-0.0.2/src/quicklst.egg-info/requires.txt
+-rwxrwxrwx   0 jgoes     (1000) jgoes     (1000)        9 2024-05-15 01:30:34.000000 quicklst-0.0.2/src/quicklst.egg-info/top_level.txt
```

### Comparing `quicklst-0.0.1/LICENSE` & `quicklst-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quicklst-0.0.1/PKG-INFO` & `quicklst-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: quicklst
-Version: 0.0.1
+Version: 0.0.2
 Summary: Read lst files produced by FAST ComTec's mpa system.
 Author-email: Joschka Goes <jajo_11@outlook.com>
 Project-URL: Homepage, https://github.com/jajo-11/quicklst
 Project-URL: Bug Tracker, https://github.com/jajo-11/quicklst/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: numpy
+Requires-Dist: numba
 
 # Quicklst
 
 Quicklst ist a python library for reading .lst files produced by FAST ComTec's mpa system. It uses numba to accelerate
 the reading of the file and supports block or chunk wise loading of large files.
 
 Limitations: Both MPA3 and MPA4A files are supported, but they need to be in binary form not in ASCII encoding, the real
```

### Comparing `quicklst-0.0.1/pyproject.toml` & `quicklst-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quicklst"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="Joschka Goes", email="jajo_11@outlook.com" },
 ]
 description = "Read lst files produced by FAST ComTec's mpa system."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `quicklst-0.0.1/src/quicklst/distortion_map.npz` & `quicklst-0.0.2/src/quicklst/distortion_map.npz`

 * *Files identical despite different names*

### Comparing `quicklst-0.0.1/src/quicklst/quicklst.py` & `quicklst-0.0.2/src/quicklst/quicklst.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
   from numba.experimental import jitclass
 else:
   from numba import jitclass
 
 import enum
 import warnings
 import os.path
-from collections.abc import Callable
 
 
 # Types of list files
 class ListFileType(enum.Enum):
   MPA3 = 0
   MPA4A = 1
 
@@ -119,35 +118,33 @@
     if self._total_time is None:
       for _ in self.blocks():
         pass  # once all blocks have been loaded the total time is set by the iterator
     return self._total_time
 
   def hist1d(self, adc: uint8, bin_size: uint16 = 1, coincident_adcs: uint8[:] = None):
     """
-    Produces histogram from data of one adcs.
+    Produces histogram from data of one adc.
 
     :param adc: index of adc to put on the x axis
     :param bin_size: bin size adc1
     :param coincident_adcs: list of adc indices that are required to be coincident for an event to be counted
     :return: returns a (adc_x_max/bin_size)X(adc_y_max/bin_size) histogram
     """
     if coincident_adcs is None:
-      coinc = 1 << adc
+      coincidence_bit_field = 1 << adc
     else:
       # make sure we have values for selected adcs
-      coinc: uint8 = 0
+      coincidence_bit_field: uint8 = 0
       for a in coincident_adcs:
-        coinc |= 1 << a
+        coincidence_bit_field |= 1 << a
 
-    x = int(np.ceil(8192 / bin_size))
-    _iter = self.blocks()
-    block = next(_iter)
-    hist = _hist_index_range(block, x, adc, bin_size, coinc, 0, block.time.size)
-    for block in _iter:
-      hist += _hist_index_range(block, x, adc, bin_size, coinc, 0, block.time.size)
+    n_bins = int(np.ceil(8192 / bin_size))
+    hist = np.zeros(n_bins, dtype='uint32')
+    for block in self.blocks():
+      _hist_index_range(block, hist, adc, bin_size, coincidence_bit_field, 0, block.time.size)
     return hist
 
   def hist2d(self, adc_x: uint8, adc_y: uint8,
              bin_size_x: uint16 = 1, bin_size_y: uint16 = 1) -> uint32[:, :]:
     """
     Produces histogram from data of two adcs.
 
@@ -155,55 +152,63 @@
     :param adc_y: index of adc to put on the y axis
     :param bin_size_x: bin size adc1
     :param bin_size_y bin size adc2
     :return: returns a (adc_x_max/bin_x)X(adc_y_max/bin_y) histogram
     """
     x = int(np.ceil(8192 / bin_size_x))
     y = int(np.ceil(8192 / bin_size_y))
-    return _iter_sum(self, _hist2d, adc_x, adc_y, x, y, bin_size_x, bin_size_y)
+    hist = np.zeros((y, x), dtype='uint32')
+    for block in self.blocks():
+      _hist2d(block, hist, adc_x, adc_y, bin_size_x, bin_size_y)
+    return hist
 
   def hist2d_area_of_interest(self, adc_x: uint8, adc_y: uint8, adc_aoi: uint8, aoi_min: uint16, aoi_max: uint16,
                               bin_size_x: uint16 = 1, bin_size_y: uint16 = 1) -> uint32[:, :]:
     """
     Produces histogram from data of two adcs for all events where the value of adc 3 lays within the range
     aoi_min..aoi_max.
 
-    :param adc_x: index of adc to put on the x axis
-    :param adc_y: index of adc to put on the y axis
+    :param adc_x: index of adc to put on the x-axis
+    :param adc_y: index of adc to put on the y-axis
     :param adc_aoi: index of adc to use for area of interest
     :param aoi_min: minimum area of interest (inclusive)
     :param aoi_max: maximum area of interest (inclusive)
     :param bin_size_x: bin size adc_x
     :param bin_size_y: bin size adc_y
     :return: returns a (adc_x_max/bin_x)X(adc_y_max/bin_y) histogram
     """
 
     x = int(np.ceil(8192 / bin_size_x))
     y = int(np.ceil(8192 / bin_size_y))
-    return _iter_sum(self, _hist2d_area_of_interest, adc_x, adc_y, adc_aoi, aoi_min, aoi_max, x, y, bin_size_x,
-                     bin_size_y)
+    hist = np.zeros((y, x), dtype='uint32')
+    for block in self.blocks():
+      _hist2d_area_of_interest(block, hist, adc_x, adc_y, adc_aoi, aoi_min, aoi_max, bin_size_x, bin_size_y)
+    return hist
 
   def hist2d_time_of_interest(self, adc_x: uint8, adc_y: uint8, time_min: int64, time_max: int64,
                               bin_size_x: uint16 = 1, bin_size_y: uint16 = 1) -> uint32[:, :]:
     """
     Produces histogram from data of two adcs for all events where the value of adc 3 lays within the range
     aoi_min..aoi_max.
 
-    :param adc_x: index of adc to put on the x axis
-    :param adc_y: index of adc to put on the y axis
+    :param adc_x: index of adc to put on the x-axis
+    :param adc_y: index of adc to put on the y-axis
     :param time_min: minimum time since start of measurement in ms (inclusive)
     :param time_max: maximum time since start of measurement in ms (inclusive)
     :param bin_size_x: bin size adc_x
     :param bin_size_y: bin size adc_y
     :return: returns a (adc_x_max/bin_size_x)X(adc_y_max/bin_size_x) histogram
     """
 
     x = int(np.ceil(8192 / bin_size_x))
     y = int(np.ceil(8192 / bin_size_y))
-    return _iter_sum(self, _hist2d_time_of_interest, x, y, adc_x, adc_y, time_min, time_max, bin_size_x, bin_size_y)
+    hist = np.zeros((y, x), dtype='uint32')
+    for block in self.blocks():
+      _hist2d_time_of_interest(block, hist, adc_x, adc_y, time_min, time_max, bin_size_x, bin_size_y)
+    return hist
 
   def hist2d_time_adc(self, adc: uint8, time_bin_size: int64, time_min: int64 = 0, time_max: int64 = None,
                       adc_bin_size: uint16 = 1, coincident_adcs: uint8[:] = None, omit_incomplete_bin=None
                       ) -> uint32[:, :]:
     """
     Get a 2d histogram with time on one axis and the values of one adc on the other
 
@@ -231,31 +236,30 @@
     make_new = True
     _iter = self.blocks()
     block = next(_iter)
     start = _seek_time(block, time_min)
     while True:
       stop = _seek_time(block, time_min + time_bin_size, start)
       if start == stop:
-        print('wait')
+        print('wait')  # TODO handle properly
       if make_new:
-        hists.append(_hist_index_range(block, x, adc, adc_bin_size, coinc, start, stop))
-      else:
-        hists[-1] += _hist_index_range(block, x, adc, adc_bin_size, coinc, start, stop)
+        hists.append(np.zeros(x, dtype='uint32'))
+      _hist_index_range(block, hists[-1], adc, adc_bin_size, coinc, start, stop)
       if stop == len(block.time):
         try:
           block = next(_iter)
         except StopIteration:
           break
         start = 0
         make_new = False
       else:
         start = stop
         time_min += time_bin_size
-        if time_max is not None and (
-            time_min > time_max or (time_min + time_bin_size > time_max and omit_incomplete_bin)):
+        if (time_max is not None and
+                (time_min > time_max or (time_min + time_bin_size > time_max and omit_incomplete_bin))):
           break
         make_new = True
 
     if time_min + time_bin_size > block.time[-1] + 1:
       if omit_incomplete_bin is None:
         warnings.warn("Last time bin is shorter than the others")
         hist = np.array(hists)
@@ -291,15 +295,15 @@
   def __init__(self,
                file: uint16[:],
                time_offset: int64,
                file_end: boolean,
                file_type: uint32,
                adc_map: int32[:]):
     """
-    Reads a ListFile block from a uint16 array.
+    Reads a ListFile block from an uint16 array.
 
     The start of the array should be aligned with one of the Signals. If
     `file_end` is true it is assumed that the end of the array is the end
     of the ListFile, if it is false the reader makes sure to stop reading
     once the content of a data Signal might be cut off. The index up to which
     was read is stored in `read_up_to`. When reading the next block the array
     should start from that index.
@@ -335,15 +339,14 @@
 
     self.active_adcs = np.empty(capacity, dtype=np.uint16)
     self.time = np.empty(capacity, dtype=np.int64)
     self.adc = np.zeros((capacity, self.adc_map.max() + 1), dtype=np.uint16)
 
     # Actual read
     ctime: int64 = time_offset
-    i = 1
     j: int64 = 0
     while i < max_i:
       # Sync
       if file[i] == 0xFFFF:
         i += 2
       # Timer
       elif file[i] & 0x4000:
@@ -383,15 +386,14 @@
 
     # allocate arrays
     self.active_adcs = np.empty(capacity, dtype=np.uint16)
     self.time = np.empty(capacity, dtype=np.int64)
     self.adc = np.zeros((capacity, self.adc_map.max() + 1), dtype=np.uint16)
 
     ctime: int64 = time_offset
-    i = 0
     j: int64 = 0
     while i < max_i:
       # Timer
       if file[i] & 0b1111 == 0x8:
         ctime += 1
         i += 4
       # Data
@@ -483,64 +485,60 @@
   if data_start == 0:
     raise RuntimeError("data marker not found")
   else:
     return data_start, list_file_type, adc_bitfield
 
 
 @njit
-def _hist2d(block: ListFileBlock, adc1: uint8, adc2: uint8, x: uint16, y: uint16, adc1_bin_size: uint16,
+def _hist2d(block: ListFileBlock, out_hist: uint32[:], adc1: uint8, adc2: uint8, adc1_bin_size: uint16,
             adc2_bin_size: uint16) -> uint32[:, :]:
-  hist = np.zeros((y, x), dtype=np.uint32)
-
   mask1 = 1 << adc1
   mask2 = 1 << adc2
   adc1i = block.adc_map[adc1]
   adc2i = block.adc_map[adc2]
 
   for i in range(len(block.time)):
     if block.active_adcs[i] & mask1 and block.active_adcs[i] & mask2:
       xv = block.adc[i, adc1i] // adc1_bin_size
       yv = block.adc[i, adc2i] // adc2_bin_size
-      hist[yv, xv] += 1
+      out_hist[yv, xv] += 1
 
-  return hist
+  return out_hist
 
 
 @njit
-def _hist2d_area_of_interest(block: ListFileBlock, adc1: uint8, adc2: uint8, adc3: uint8,
-                             aoi_min: uint16, aoi_max: uint16, x: uint16, y: uint16, adc1_bin_size: uint16,
-                             adc2_bin_size: uint16) -> uint32[:, :]:
-  hist = np.zeros((y, x), dtype=np.uint32)
-
+def _hist2d_area_of_interest(block: ListFileBlock, out_hist: uint32[:], adc1: uint8, adc2: uint8, adc3: uint8,
+                             aoi_min: uint16, aoi_max: uint16, adc1_bin_size: uint16, adc2_bin_size: uint16
+                             ) -> uint32[:, :]:
   mask1 = 1 << adc1
   mask2 = 1 << adc2
   mask3 = 1 << adc3
   adc1i = block.adc_map[adc1]
   adc2i = block.adc_map[adc2]
   adc3i = block.adc_map[adc3]
 
   for i in range(len(block.time)):
     if block.active_adcs[i] & mask1 and block.active_adcs[i] & mask2 and block.active_adcs[i] & mask3:
       if aoi_min <= block.adc[i, adc3i] <= aoi_max:
         xv = block.adc[i, adc1i] // adc1_bin_size
         yv = block.adc[i, adc2i] // adc2_bin_size
-        hist[yv, xv] += 1
+        out_hist[yv, xv] += 1
 
-  return hist
+  return out_hist
 
 
 @njit
 def _seek_time(block: ListFileBlock, time: uint32, start: int64 = 0, stop: int64 = -1) -> int64:
   """
   seek index of first event with set time or larger
 
   :param block: ListFileBlock to work on
   :param time: time to find
-  :param start: lowest index to search
-  :param stop: highest index to search (inclusive), if negative -1 means until end of block, -2 until end excluding
+  :param start: the lowest index to search
+  :param stop: the highest index to search (inclusive), if negative -1 means until end of block, -2 until end excluding
   last element etc.
   :return: index of first event with time larger than `time` or len(block.time) if time is out of range
   """
   if stop < 0:
     stop = len(block.time) + stop
   if block.time[stop] < time:
     return len(block.time)
@@ -555,91 +553,57 @@
     for i in range(start, stop + 1):
       if time < block.time[i]:
         return i
     return i
 
 
 @njit
-def _hist_index_range(block: ListFileBlock, x: int64, adc: uint8, bin_size: uint16, coinc: uint8, start: int64,
-                      stop: int64) -> uint32[:]:
+def _hist_index_range(block: ListFileBlock, out_hist: uint32[:], adc: uint8, bin_size: uint16, coinc: uint8,
+                      start: int64, stop: int64) -> uint32[:]:
   """
   Creates 1d-histogram for the given adc and block
   indices must be in range (no bounds checks are done)
   """
-  hist = np.zeros(x, dtype='uint32')
   adci = block.adc_map[adc]
 
   for i in range(start, stop):
     if block.active_adcs[i] & coinc == coinc:
       xv = block.adc[i, adci] // bin_size
-      hist[xv] += 1
+      out_hist[xv] += 1
 
-  return hist
+  return out_hist
 
 
 @njit
-def _hist2d_time_of_interest(block: ListFileBlock, x: uint16, y: uint16, adc1: uint8, adc2: uint8, time_min: int64,
+def _hist2d_time_of_interest(block: ListFileBlock, out_hist: uint32[:], adc1: uint8, adc2: uint8, time_min: int64,
                              time_max: int64, adc1_bin_size: uint16, adc2_bin_size: uint16) -> uint32[:, :]:
-  hist = np.zeros((y, x), dtype=np.uint32)
-
   mask1 = 1 << adc1
   mask2 = 1 << adc2
+  mask = mask1 & mask2
   adc1i = block.adc_map[adc1]
   adc2i = block.adc_map[adc2]
 
   i = 0
   while i < len(block.time) and block.time[i] < time_min:
     i += 1
 
   for j in range(i, len(block.time)):
     if block.time[j] > time_max:
       break
-    if block.active_adcs[j] & mask1 and block.active_adcs[j] & mask2:
+    if block.active_adcs[j] & mask == mask:
       xv = block.adc[j, adc1i] // adc1_bin_size
       yv = block.adc[j, adc2i] // adc2_bin_size
-      hist[yv, xv] += 1
+      out_hist[yv, xv] += 1
 
-  return hist
-
-
-# shifts values in histogram of the flash ebit mcp to correct for non-linearities
-@njit
-def _apply_correction(hist, distortion_map):
-  """
-  shifts values of histogram according to distortion_map to correct for non-linearities in the detector of the flash ebit
-  """
-  assert (hist.shape[0] == distortion_map.shape[0])
-  assert (hist.shape[1] == distortion_map.shape[1])
-
-  corrected_hist = np.zeros(hist.shape, dtype=np.int64)
-
-  for i in range(hist.shape[0]):
-    for j in range(hist.shape[1]):
-      new_j = j + distortion_map[i, j]
-      if 0 <= new_j < hist.shape[1]:
-        corrected_hist[i, new_j] += hist[i, j]
-
-  return corrected_hist
+  return out_hist
 
 
 @njit
 def down_bin(hist, factor=8):
   """
-  Crudely bins given 2 histogram
+  Crudely bins given 2d histogram
   """
   out = np.zeros((hist.shape[0] // factor + 1, hist.shape[1] // factor + 1), dtype=hist.dtype)
   for i in range(hist.shape[0]):
     for j in range(hist.shape[1]):
       out[i // factor, j // factor] += hist[i, j]
   return out
-
-
-def _iter_sum(lf: ListFile, fn: Callable, *args, **kwargs):
-  """
-  Utility function that sums over the results of fn while iterating over all blocks
-  this is done so that we can skip the first summation and initialization of a zero array
-  """
-  iter_ = lf.blocks()
-  rv = fn(next(iter_), *args, **kwargs)
-  for i in iter_:
-    rv += fn(i, *args, **kwargs)
-  return rv
```

### Comparing `quicklst-0.0.1/src/quicklst.egg-info/PKG-INFO` & `quicklst-0.0.2/src/quicklst.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: quicklst
-Version: 0.0.1
+Version: 0.0.2
 Summary: Read lst files produced by FAST ComTec's mpa system.
 Author-email: Joschka Goes <jajo_11@outlook.com>
 Project-URL: Homepage, https://github.com/jajo-11/quicklst
 Project-URL: Bug Tracker, https://github.com/jajo-11/quicklst/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: numpy
+Requires-Dist: numba
 
 # Quicklst
 
 Quicklst ist a python library for reading .lst files produced by FAST ComTec's mpa system. It uses numba to accelerate
 the reading of the file and supports block or chunk wise loading of large files.
 
 Limitations: Both MPA3 and MPA4A files are supported, but they need to be in binary form not in ASCII encoding, the real
```

