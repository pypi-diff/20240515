# Comparing `tmp/axidence-0.2.2.tar.gz` & `tmp/axidence-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axidence-0.2.2.tar", max compression
+gzip compressed data, was "axidence-0.3.0.tar", max compression
```

## Comparing `axidence-0.2.2.tar` & `axidence-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1522 2024-04-30 21:22:48.104117 axidence-0.2.2/LICENSE
--rw-r--r--   0        0        0     1046 2024-04-30 21:22:48.104117 axidence-0.2.2/README.md
--rw-r--r--   0        0        0      206 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/__init__.py
--rw-r--r--   0        0        0     8260 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/context.py
--rw-r--r--   0        0        0     2239 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/dtypes.py
--rw-r--r--   0        0        0     2001 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugin.py
--rw-r--r--   0        0        0      219 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/__init__.py
--rw-r--r--   0        0        0      259 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/cuts/__init__.py
--rw-r--r--   0        0        0      959 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/cuts/cut_event_building.py
--rw-r--r--   0        0        0     1001 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/cuts/cut_isolated_s1.py
--rw-r--r--   0        0        0      981 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/cuts/cut_isolated_s2.py
--rw-r--r--   0        0        0      545 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/cuts/cut_pairing_exists.py
--rw-r--r--   0        0        0      107 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/isolated/__init__.py
--rw-r--r--   0        0        0     1674 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/isolated/isolated_s1.py
--rw-r--r--   0        0        0     2918 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/isolated/isolated_s2.py
--rw-r--r--   0        0        0       47 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/meta/__init__.py
--rw-r--r--   0        0        0      505 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/meta/run_meta.py
--rw-r--r--   0        0        0      113 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/pairing/__init__.py
--rw-r--r--   0        0        0     7404 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/pairing/events_paired.py
--rw-r--r--   0        0        0    33786 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/pairing/peaks_paired.py
--rw-r--r--   0        0        0      295 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/salting/__init__.py
--rw-r--r--   0        0        0     7283 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/salting/event_building.py
--rw-r--r--   0        0        0     1935 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/salting/event_fields.py
--rw-r--r--   0        0        0     7813 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/salting/events_salting.py
--rw-r--r--   0        0        0     4841 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/salting/peak_correlation.py
--rw-r--r--   0        0        0     3109 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/salting/peaks_salted.py
--rw-r--r--   0        0        0     1964 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/samplers.py
--rw-r--r--   0        0        0     2593 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/utils.py
--rw-r--r--   0        0        0      933 2024-04-30 21:22:48.108117 axidence-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 axidence-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1522 2024-05-14 23:40:20.220815 axidence-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1046 2024-05-14 23:40:20.220815 axidence-0.3.0/README.md
+-rw-r--r--   0        0        0      206 2024-05-14 23:40:20.220815 axidence-0.3.0/axidence/__init__.py
+-rw-r--r--   0        0        0    11675 2024-05-14 23:40:20.220815 axidence-0.3.0/axidence/context.py
+-rw-r--r--   0        0        0     2254 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/dtypes.py
+-rw-r--r--   0        0        0     1376 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugin.py
+-rw-r--r--   0        0        0      219 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/__init__.py
+-rw-r--r--   0        0        0      261 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/cuts/__init__.py
+-rw-r--r--   0        0        0     1001 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/cuts/cut_isolated_s1.py
+-rw-r--r--   0        0        0     1146 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/cuts/cut_isolated_s2.py
+-rw-r--r--   0        0        0      572 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/cuts/cut_pairing_exists.py
+-rw-r--r--   0        0        0     1001 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/cuts/cuts_event_building.py
+-rw-r--r--   0        0        0      107 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/isolated/__init__.py
+-rw-r--r--   0        0        0     1774 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/isolated/isolated_s1.py
+-rw-r--r--   0        0        0     3098 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/isolated/isolated_s2.py
+-rw-r--r--   0        0        0       47 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/meta/__init__.py
+-rw-r--r--   0        0        0      500 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/meta/run_meta.py
+-rw-r--r--   0        0        0      113 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/pairing/__init__.py
+-rw-r--r--   0        0        0     7365 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/pairing/events_paired.py
+-rw-r--r--   0        0        0    33605 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/pairing/peaks_paired.py
+-rw-r--r--   0        0        0      353 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/__init__.py
+-rw-r--r--   0        0        0     7993 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/event_building.py
+-rw-r--r--   0        0        0     1422 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/event_combine.py
+-rw-r--r--   0        0        0     2155 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/event_fields.py
+-rw-r--r--   0        0        0     9693 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/events_salting.py
+-rw-r--r--   0        0        0     4841 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/peak_correlation.py
+-rw-r--r--   0        0        0     3148 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/peaks_salted.py
+-rw-r--r--   0        0        0     2035 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/samplers.py
+-rw-r--r--   0        0        0     2685 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/utils.py
+-rw-r--r--   0        0        0      933 2024-05-14 23:40:20.224815 axidence-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 axidence-0.3.0/PKG-INFO
```

### Comparing `axidence-0.2.2/LICENSE` & `axidence-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `axidence-0.2.2/README.md` & `axidence-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `axidence-0.2.2/axidence/dtypes.py` & `axidence-0.3.0/axidence/dtypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     + ambience_fields
     + se_density_fields
     + nearest_triggering_fields
     + peak_misc_fields
 )
 
 event_level_fields = [
+    "n_peaks",
     "s1_center_time",
     "s2_center_time",
     "s1_area",
     "alt_s1_area",
     "s2_area",
     "alt_s2_area",
     "s1_index",
```

### Comparing `axidence-0.2.2/axidence/plugins/cuts/cut_event_building.py` & `axidence-0.3.0/axidence/plugins/cuts/cuts_event_building.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from strax import CutPlugin, CutList
 
 
 class MainS1Trigger(CutPlugin):
-    __version__ = "0.0.0"
+    __version__ = "0.1.0"
     depends_on = "event_basics"
     provides = "cut_main_s1_trigger"
     cut_name = "cut_main_s1_trigger"
     cut_description = "Whether the salting S1 can be the main S2"
 
     def cut_by(self, events):
-        mask = events["s1_salt_number"] >= 0
+        mask = events["s1_salt_number"] == events["salt_number"]
         return mask
 
 
 class MainS2Trigger(CutPlugin):
-    __version__ = "0.0.0"
+    __version__ = "0.1.0"
     depends_on = "event_basics"
     provides = "cut_main_s2_trigger"
     cut_name = "cut_main_s2_trigger"
     cut_description = "Whether the salting S2 can be the main S2"
 
     def cut_by(self, events):
-        mask = events["s2_salt_number"] >= 0
+        mask = events["s2_salt_number"] == events["salt_number"]
         return mask
 
 
 class EventBuilding(CutList):
     __version__ = "0.0.0"
-    provides = "cut_event_building"
-    accumulated_cuts_string = "cut_event_building"
+    provides = "cuts_event_building"
+    accumulated_cuts_string = "cuts_event_building"
     cut_description = "Whether the salting S1 or S2 can be the main S1 or S2"
 
     cuts = (MainS1Trigger, MainS2Trigger)
```

### Comparing `axidence-0.2.2/axidence/plugins/cuts/cut_isolated_s1.py` & `axidence-0.3.0/axidence/plugins/cuts/cut_isolated_s1.py`

 * *Files identical despite different names*

### Comparing `axidence-0.2.2/axidence/plugins/cuts/cut_isolated_s2.py` & `axidence-0.3.0/axidence/plugins/cuts/cut_isolated_s2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,30 @@
+import strax
 from strax import parse_selection, CutPlugin
 from strax import SaveWhen
 import straxen
+from straxen import Events
 
+export, __all__ = strax.exporter()
 
+trigger_min_area = Events.takes_config["trigger_min_area"].default
+
+
+@export
 class IsolatedS2Mask(CutPlugin):
     __version__ = "0.0.0"
     depends_on = "event_basics"
     provides = "cut_isolated_s2"
     cut_name = "cut_isolated_s2"
     data_kind = "events"
     cut_description = "Isolated S2 selection, a event-level cut."
     save_when = SaveWhen.NEVER
 
     isolated_s2_area_range = straxen.URLConfig(
-        default=(1e2, 2e4),
+        default=(trigger_min_area, 2e4),
         type=(list, tuple),
         help="Range of isolated S2 area",
     )
 
     isolated_s2_selection = straxen.URLConfig(
         default=None,
         type=(str, None),
```

### Comparing `axidence-0.2.2/axidence/plugins/cuts/cut_pairing_exists.py` & `axidence-0.3.0/axidence/plugins/cuts/cut_pairing_exists.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 class PairingExists(CutPlugin):
     """Cut of successfully paired AC with AC-type(`event_type`)"""
 
     __version__ = "0.0.0"
     depends_on = "event_infos_paired"
     provides = "cut_pairing_exists"
     cut_name = "cut_pairing_exists"
-    data_kind = "event_paired"
+    data_kind = "events_paired"
     cut_description = (
         "Whether isolated S2 influenced by pairing, and whether the event is considered as AC event"
     )
+    allow_hyperrun = True
 
     def cut_by(self, events_paired):
         return np.isin(events_paired["event_type"], [1, 3])
```

### Comparing `axidence-0.2.2/axidence/plugins/isolated/isolated_s1.py` & `axidence-0.3.0/axidence/plugins/isolated/isolated_s1.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,22 +37,24 @@
         )
         return strax.unpack_dtype(union_dtype)
 
     def infer_dtype(self):
         dtype_reference = self.refer_dtype("peaks")
         dtype = copy_dtype(dtype_reference, self.isolated_peaks_fields)
         dtype += [
+            (("Run id", "run_id"), np.int32),
             (("Group number of peaks", "group_number"), np.int64),
         ]
         return dtype
 
     def compute(self, peaks):
         _result = peaks[peaks["cut_isolated_s1"]]
         result = np.empty(len(_result), dtype=self.dtype)
         for n in result.dtype.names:
-            if n not in ["group_number"]:
+            if n not in ["run_id", "group_number"]:
                 result[n] = _result[n]
 
+        result["run_id"] = int(self.run_id)
         result["group_number"] = np.arange(len(result)) + self.groups_seen
 
         self.groups_seen += len(result)
         return result
```

### Comparing `axidence-0.2.2/axidence/plugins/isolated/isolated_s2.py` & `axidence-0.3.0/axidence/plugins/isolated/isolated_s2.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,34 +52,39 @@
         # Note that here we only save the time and endtime of peaks, but not events
         for n in ["time", "endtime", "x", "y"]:
             if n in self.isolated_events_fields:
                 raise ValueError(f"{n} is not allowed in isolated_events_fields!")
         dtype = copy_dtype(self.refer_dtype("peaks"), self.isolated_peaks_fields)
         dtype += copy_dtype(self.refer_dtype("events"), self.isolated_events_fields)
         dtype += [
+            (("Run id", "run_id"), np.int32),
             (("Group number of peaks", "group_number"), np.int64),
         ]
         return dtype
 
     def compute(self, events, peaks):
         _events = events[events["cut_isolated_s2"]]
+        if len(_events) == 0:
+            return np.empty(0, dtype=self.dtype)
+
         split_peaks = strax.split_by_containment(peaks, _events)
         _peaks = np.hstack(split_peaks)
         if _events["n_peaks"].sum() != len(_peaks):
             raise ValueError(f"Expected {_events['n_peaks'].sum()} peaks, got {len(_peaks)}!")
 
         result = np.empty(_events["n_peaks"].sum(), dtype=self.dtype)
         for n in result.dtype.names:
-            if n not in ["group_number"]:
+            if n not in ["run_id", "group_number"]:
                 if n in self.isolated_peaks_fields:
                     result[n] = _peaks[n]
                 elif n in self.isolated_events_fields:
                     result[n] = np.repeat(_events[n], _events["n_peaks"])
                 else:
                     raise ValueError(f"Field {n} not found in peaks or events!")
 
+        result["run_id"] = int(self.run_id)
         result["group_number"] = (
             np.repeat(np.arange(len(_events)), _events["n_peaks"]) + self.groups_seen
         )
 
         self.groups_seen += len(_events)
         return result
```

### Comparing `axidence-0.2.2/axidence/plugins/pairing/events_paired.py` & `axidence-0.3.0/axidence/plugins/pairing/events_paired.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 from ...utils import copy_dtype
 
 export, __all__ = strax.exporter()
 
 
 class EventsForcePaired(OverlapWindowPlugin):
     """Mimicking Events Force manually pairing of isolated S1 & S2 Actually NOT
-    used in AC simulation, but just for debug."""
+    used in simulation, but just for debug."""
 
     depends_on = "peaks_paired"
     provides = "events_paired"
     data_kind = "events_paired"
     save_when = strax.SaveWhen.EXPLICIT
+    allow_hyperrun = True
 
     paring_time_interval = straxen.URLConfig(
         default=int(1e8),
         type=int,
         help="The interval which separates two events S1 [ns]",
     )
 
@@ -53,14 +54,15 @@
     time of main S1/2 peaks and the pairing-type."""
 
     __version__ = "0.0.0"
     depends_on = ("event_info_paired", "peaks_paired")
     provides = "event_infos_paired"
     data_kind = "events_paired"
     save_when = strax.SaveWhen.EXPLICIT
+    allow_hyperrun = True
 
     ambience_fields = straxen.URLConfig(
         default=["lh_before", "s0_before", "s1_before", "s2_before", "s2_near"],
         type=(list, tuple),
         help="Needed ambience related fields",
     )
 
@@ -81,17 +83,16 @@
             "pdf_s2_position_shadow",
             "nearest_dt_s1",
             "nearest_dt_s2",
             "se_density",
             "left_dtime",
             "right_dtime",
         ]
-        # TODO: reconsider about how to store run_id after implementing super runs
         required_names += [
-            # "origin_run_id",
+            "origin_run_id",
             "origin_group_number",
             "origin_time",
             "origin_endtime",
             "origin_center_time",
         ]
         return required_names
 
@@ -156,15 +157,15 @@
             for idx, main_peak in zip(
                 [event["alt_s1_index"], event["alt_s2_index"]], ["alt_s1_", "alt_s2_"]
             ):
                 if idx >= 0:
                     for n in self.peak_fields:
                         if n in self.alternative_peak_add_fields:
                             result[main_peak + n][i] = sp[n][idx]
-            # if the AC event have S2
+            # if the event have S2
             if event["s2_index"] != -1:
                 if sp["origin_s1_index"][0] == -1:
                     # if isolated S2 is pure-isolated S2(w/o main S1)
                     if event["s1_index"] != -1:
                         # if successfully paired, considered as AC
                         result["event_type"][i] = 1
                     else:
```

### Comparing `axidence-0.2.2/axidence/plugins/pairing/peaks_paired.py` & `axidence-0.3.0/axidence/plugins/pairing/peaks_paired.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import warnings
 from immutabledict import immutabledict
 import numpy as np
 import strax
-from strax import Plugin, DownChunkingPlugin
+from strax import Plugin, ExhaustPlugin, DownChunkingPlugin
 import straxen
 from straxen import units
 from straxen import PeakProximity
 import GOFevaluation as ge
 
 from ...utils import copy_dtype
-from ...samplers import SAMPLERS
 from ...dtypes import peak_positions_dtype
-from ...plugin import ExhaustPlugin
 
 
 class PeaksPaired(ExhaustPlugin, DownChunkingPlugin):
-    __version__ = "0.0.0"
+    __version__ = "0.0.1"
     depends_on = (
+        "run_meta",
         "isolated_s1",
         "isolated_s2",
-        "events_salted",
-        "event_basics_salted",
-        "event_shadow_salted",
-        "cut_main_s2_trigger_salted",
+        "peaks_salted",
+        "peak_shadow_salted",
     )
     provides = ("peaks_paired", "truth_paired")
     data_kind = immutabledict(zip(provides, provides))
     save_when = immutabledict(zip(provides, [strax.SaveWhen.EXPLICIT, strax.SaveWhen.ALWAYS]))
     rechunk_on_save = immutabledict(zip(provides, [False, True]))
+    allow_hyperrun = True
 
     pairing_seed = straxen.URLConfig(
         default=None,
         type=(int, None),
         help="Seed for pairing",
     )
 
@@ -61,27 +59,22 @@
 
     max_n_shadow_bins = straxen.URLConfig(
         default=30,
         type=int,
         help="Max bin number of 2D shadow matching",
     )
 
-    isolated_s1_rate_correction = straxen.URLConfig(
-        default=True,
-        type=bool,
-        help="Whether correct isolated S1 rate when calculating AC rate",
-    )
-
-    # multiple factor in simulation, e.g. AC rate is 1/t/y,
-    # multiple factor is 100, then we will make 100 AC events
+    # multiple factor in simulation,
+    # e.g. if number of event is is 1 in the run, and multiple factor is 100,
+    # then we will make 100 events
     paring_rate_bootstrap_factor = straxen.URLConfig(
         default=1e2,
         type=(int, float, list, tuple),
         help=(
-            "Bootstrap factor for AC rate, "
+            "Bootstrap factor for pairing rate, "
             "if list or tuple, they are the factor for 2 and 3+ hits S1"
         ),
     )
 
     s1_min_coincidence = straxen.URLConfig(
         default=2, type=int, help="Minimum tight coincidence necessary to make an S1"
     )
@@ -112,26 +105,14 @@
 
     only_salt_s1 = straxen.URLConfig(
         default=False,
         type=bool,
         help="Whether only salt S1",
     )
 
-    apply_shadow_reweight = straxen.URLConfig(
-        default=True,
-        type=bool,
-        help="Whether perform shadow reweight",
-    )
-
-    shadow_reweight_n_bins = straxen.URLConfig(
-        default=50,
-        type=int,
-        help="Bin number of shadow reweight",
-    )
-
     shadow_deltatime_exponent = straxen.URLConfig(
         default=-1.0, type=float, track=True, help="The exponent of delta t when calculating shadow"
     )
 
     fixed_drift_time = straxen.URLConfig(
         default=None,
         type=(int, float, None),
@@ -142,33 +123,32 @@
         default=int(1e8),
         type=int,
         help="The interval which separates two events S1 [ns]",
     )
 
     def infer_dtype(self):
         dtype = strax.unpack_dtype(self.deps["isolated_s1"].dtype_for("isolated_s1"))
-        # TODO: reconsider about how to store run_id after implementing super runs
         peaks_dtype = dtype + [
             # since event_number is int64 in event_basics
             (("Event number in this dataset", "event_number"), np.int64),
-            # (("Original run id", "origin_run_id"), np.int32),
+            (("Original run id", "origin_run_id"), np.int32),
             (("Original isolated S1/S2 group", "origin_group_number"), np.int32),
             (("Original time of peaks", "origin_time"), np.int64),
             (("Original endtime of peaks", "origin_endtime"), np.int64),
             (("Original center_time of peaks", "origin_center_time"), np.int64),
             (("Original n_competing", "origin_n_competing"), np.int32),
             (("Original type of group", "origin_group_type"), np.int8),
             (("Original s1_index in isolated S1", "origin_s1_index"), np.int32),
             (("Original s2_index in isolated S2", "origin_s2_index"), np.int32),
             (("Normalization of number of paired events", "normalization"), np.float32),
         ]
         truth_dtype = [
             (("Event number in this dataset", "event_number"), np.int64),
-            # (("Original run id of isolated S1", "s1_run_id"), np.int32),
-            # (("Original run id of isolated S2", "s2_run_id"), np.int32),
+            (("Original run id of isolated S1", "s1_run_id"), np.int32),
+            (("Original run id of isolated S2", "s2_run_id"), np.int32),
             (
                 ("Drift time between isolated S1 and main isolated S2 [ns]", "drift_time"),
                 np.float32,
             ),
             (("Original isolated S1 group", "s1_group_number"), np.int32),
             (("Original isolated S2 group", "s2_group_number"), np.int32),
             (("Normalization of number of paired events", "normalization"), np.float32),
@@ -193,14 +173,25 @@
                     "if provided list or tuple!"
                 )
             self.bootstrap_factor = list(self.paring_rate_bootstrap_factor)
         else:
             self.bootstrap_factor = [self.paring_rate_bootstrap_factor] * 2
 
     @staticmethod
+    def update_group_number(isolated, run_meta):
+        result = isolated.copy()
+        windows = strax.touching_windows(isolated, run_meta)
+        n_groups = np.array(
+            [np.unique(isolated["group_number"][w[0] : w[1]]).size for w in windows]
+        )
+        cumsum = np.cumsum(np.hstack([[0], n_groups])[:-1])
+        result["group_number"] += np.repeat(cumsum, windows[:, 1] - windows[:, 0])
+        return result
+
+    @staticmethod
     def preprocess_isolated_s2(s2):
         # index of isolated S2 groups
         _, s2_group_index, s2_n_peaks = np.unique(
             s2["group_number"], return_index=True, return_counts=True
         )
         # index of main S2s in isolated S2
         s2_main_index = s2_group_index + s2["s2_index"][s2_group_index]
@@ -237,48 +228,45 @@
             drift_time = np.full(n_events, fixed_drift_time)
         return paring_rate_full, (
             s1["group_number"][s1_group_index],
             s2["group_number"][s2_group_index],
             drift_time,
         )
 
-    def shadow_reference_selection(self, events_salted, s2):
+    def get_paring_rate_correction(self, peaks_salted):
+        # need to use peak-level salting because
+        # main S1 of event-level salting might be contaminated
+        return 1
+
+    def shadow_reference_selection(self, peaks_salted):
         """Select the reference events for shadow matching, also return
         weights."""
-        reference = events_salted[events_salted["cut_main_s2_trigger_salted"]]
 
         if self.only_salt_s1:
             raise ValueError("Cannot only salt S1 when performing shadow matching!")
 
-        if self.apply_shadow_reweight:
-            sampler = SAMPLERS[self.s2_distribution](
-                self.s2_area_range, self.shadow_reweight_n_bins
-            )
-            weight = sampler.reweight(reference["s2_area"], s2["s2_area"])
-        else:
-            weight = np.ones(len(reference))
+        reference = peaks_salted[peaks_salted["type"] == 2]
+        weight = np.ones(len(reference))
         weight /= weight.sum()
 
-        if np.any(np.isnan(weight)):
-            raise ValueError("Some weights are NaN!")
         dtype = np.dtype(
             [
-                ("s2_area", float),
-                ("s2_dt_s2_time_shadow", float),
-                ("s2_shadow_s2_time_shadow", float),
+                ("area", float),
+                ("dt_s2_time_shadow", float),
+                ("shadow_s2_time_shadow", float),
                 ("weight", float),
             ]
         )
         shadow_reference = np.zeros(len(reference), dtype=dtype)
         for n in dtype.names:
             if n == "weight":
                 shadow_reference[n] = weight
             else:
                 shadow_reference[n] = reference[n]
-        return shadow_reference
+        return shadow_reference, ""
 
     @staticmethod
     def digitize2d(data_sample, bin_edges, n_bins):
         """Get indices of the 2D bins to which each value in input array
         belongs.
 
         Args:
@@ -318,28 +306,29 @@
         preprocess_shadow,
         paring_rate_bootstrap_factor=1e2,
         paring_rate_correction=1.0,
         shift_dt_shadow_matching=True,
         n_drift_time_bins=50,
         shadow_deltatime_exponent=-1.0,
         max_n_shadow_bins=30,
+        prefix="",
         onlyrate=False,
     ):
         if paring_rate_bootstrap_factor < 1.0:
             raise ValueError("Bootstrap factor should be larger than 1!")
         if paring_rate_correction > 1.0:
             raise ValueError("Correction factor should be smaller than 1!")
         # perform Shadow matching technique
         # see details in xenon:xenonnt:ac:prediction:summary#fake-plugin_simulation
 
         # 2D equal binning
         # prepare the 2D space, x is log(S2/dt), y is (log(S2)**2+log(dt)**2)**0.5
         # because these 2 dimension is orthogonal
         sampled_correlation = preprocess_shadow(
-            shadow_reference, shadow_deltatime_exponent, prefix="s2_"
+            shadow_reference, shadow_deltatime_exponent, prefix=prefix
         )
         s1_sample = preprocess_shadow(s1, shadow_deltatime_exponent)
 
         # use (x, y) distribution of isolated S1 as reference
         # because it is more intense when shadow(S2/dt) is large
         reference_sample = s1_sample
         ge.check_sample_sanity(reference_sample)
@@ -408,24 +397,24 @@
                 delta_t = 0
             data_sample = preprocess_shadow(s2, shadow_deltatime_exponent, delta_t=delta_t)
             ge.check_sample_sanity(data_sample)
             # apply binning to (x, y)
             s2_shadow_count = ge.apply_irregular_binning(
                 data_sample=data_sample, bin_edges=bin_edges
             )
-            # conditional rate is AC rate in each (x, y) bin
+            # conditional rate is pairing rate in each (x, y) bin
             ac_rate_conditional = (
                 s1_shadow_count / shadow_run_time * s2_shadow_count / shadow_run_time
             )
             ac_rate_conditional *= (drift_time_bins[i + 1] - drift_time_bins[i]) / units.s
             ac_rate_conditional *= sampled_shadow_count / sampled_shadow_count.sum()
             ac_rate_conditional /= paring_rate_correction
             _paring_rate_full[i] = ac_rate_conditional.sum()
             if not onlyrate:
-                # expectation of AC in each bin in this run
+                # expectation of pairing in each bin in this run
                 lam_shadow = ac_rate_conditional * run_time * paring_rate_bootstrap_factor
                 count_pairing = rng.poisson(lam=lam_shadow).flatten()
                 if count_pairing.max() == 0:
                     count_pairing[lam_shadow.argmax()] = 1
                 s2_digit = PeaksPaired.digitize2d(data_sample, bin_edges, n_shadow_bins)
                 _s2_group_index = np.arange(len(s2))
                 s2_group_index_list = [
@@ -470,15 +459,15 @@
             drift_time,
         )
 
     def split_chunks(self, n_peaks):
         # divide results into chunks
         # max peaks number in left_i chunk
         max_in_chunk = round(
-            self.chunk_target_size_mb * 1e6 / self.dtype["peaks_paired"].itemsize * 0.9
+            0.9 * self.chunk_target_size_mb * 1e6 / self.dtype["peaks_paired"].itemsize
         )
         _n_peaks = n_peaks.copy()
         if _n_peaks.max() > max_in_chunk:
             raise ValueError("Can not fit a single paired event in a chunk!")
         seen = 0
         slices = [[0, 1]]
         for i in range(len(_n_peaks)):
@@ -506,24 +495,24 @@
         # set center time of S1 & S2
         # paired events are separated by roughly `event_interval`
         s1_center_time = np.arange(len(drift_time)).astype(int) * self.paring_time_interval + start
         s2_center_time = s1_center_time + drift_time
         # total number of isolated S1 & S2 peaks
         peaks_arrays = np.zeros(n_peaks.sum(), dtype=self.dtype["peaks_paired"])
 
-        # assign features of sampled isolated S1 and S2 in AC events
+        # assign features of sampled isolated S1 and S2 in pairing events
         peaks_count = 0
         for i in range(len(n_peaks)):
             _array = np.zeros(n_peaks[i], dtype=self.dtype["peaks_paired"])
             # isolated S1 is assigned peak by peak
             s1_index = s1_group_number[i]
             for q in self.dtype["peaks_paired"].names:
                 if "origin" not in q and q not in ["event_number", "normalization"]:
                     _array[0][q] = s1[s1_index][q]
-            # _array[0]["origin_run_id"] = s1["run_id"][s1_index]
+            _array[0]["origin_run_id"] = s1["run_id"][s1_index]
             _array[0]["origin_group_number"] = s1["group_number"][s1_index]
             _array[0]["origin_time"] = s1["time"][s1_index]
             _array[0]["origin_endtime"] = strax.endtime(s1)[s1_index]
             _array[0]["origin_center_time"] = s1["center_time"][s1_index]
             _array[0]["origin_n_competing"] = s1["n_competing"][s1_index]
             _array[0]["origin_group_type"] = 1
             _array[0]["time"] = s1_center_time[i] - (
@@ -534,15 +523,15 @@
             # isolated S2 is assigned group by group
             group_number = s2_group_number[i]
             s2_group_i = s2[s2_group_index[group_number] : s2_group_index[group_number + 1]]
             for q in self.dtype["peaks_paired"].names:
                 if "origin" not in q and q not in ["event_number", "normalization"]:
                     _array[1:][q] = s2_group_i[q]
             s2_index = s2_group_i["s2_index"]
-            # _array[1:]["origin_run_id"] = s2_group_i["run_id"]
+            _array[1:]["origin_run_id"] = s2_group_i["run_id"]
             _array[1:]["origin_group_number"] = s2_group_i["group_number"]
             _array[1:]["origin_time"] = s2_group_i["time"]
             _array[1:]["origin_endtime"] = strax.endtime(s2_group_i)
             _array[1:]["origin_center_time"] = s2_group_i["center_time"]
             _array[1:]["origin_n_competing"] = s2_group_i["n_competing"]
             _array[1:]["origin_group_type"] = 2
             _array[1:]["time"] = s2_center_time[i] - (
@@ -575,63 +564,61 @@
             np.unique(peaks_arrays["event_number"], return_index=True)[1]
         ]
         truth_arrays["endtime"] = peaks_arrays["endtime"][
             np.unique(peaks_arrays["event_number"], return_index=True)[1]
         ]
         truth_arrays["event_number"] = np.arange(len(n_peaks))
         truth_arrays["drift_time"] = drift_time
-        # truth_arrays["s1_run_id"] = s1["run_id"][s1_group_number]
-        # truth_arrays["s2_run_id"] = main_s2["run_id"][s2_group_number]
+        truth_arrays["s1_run_id"] = s1["run_id"][s1_group_number]
+        truth_arrays["s2_run_id"] = main_s2["run_id"][s2_group_number]
         truth_arrays["s1_group_number"] = s1["group_number"][s1_group_number]
         truth_arrays["s2_group_number"] = main_s2["group_number"][s2_group_number]
 
         event_number_index = np.unique(
             peaks_arrays["event_number"], return_index=True, return_counts=True
         )[1]
         if np.any(
             peaks_arrays["time"][event_number_index[1:]]
             <= peaks_arrays["endtime"][event_number_index[1:] - 1]
         ):
             raise ValueError("Some paired events overlap!")
 
         return peaks_arrays, truth_arrays
 
-    def compute(self, isolated_s1, isolated_s2, events_salted, start, end):
+    def compute(self, run_meta, isolated_s1, isolated_s2, peaks_salted, start, end):
+        isolated_s1 = self.update_group_number(isolated_s1, run_meta)
+        isolated_s2 = self.update_group_number(isolated_s2, run_meta)
         for i, s in enumerate([isolated_s1, isolated_s2]):
             if np.any(np.diff(s["group_number"]) < 0):
                 raise ValueError(f"Group number is not sorted in isolated S{i}!")
         s2_group_index, s2_main_index, s2_n_peaks, s2_length = self.preprocess_isolated_s2(
             isolated_s2
         )
         # main S2s in isolated S2
         main_isolated_s2 = isolated_s2[s2_main_index]
 
-        if self.isolated_s1_rate_correction:
-            raise NotImplementedError("AC rate correction for isolated S1 is not implemented yet!")
-        else:
-            paring_rate_correction = 1
+        paring_rate_correction = self.get_paring_rate_correction(peaks_salted)
         print(f"Isolated S1 correction factor is {paring_rate_correction:.3f}")
 
-        run_time = (end - start) / units.s
+        run_time = (run_meta["endtime"] - run_meta["time"]).sum() / units.s
         s1_rate = len(isolated_s1) / run_time
         s2_rate = len(main_isolated_s2) / run_time
+        print(f"Total run time is {run_time:.2f}s")
         print(f"There are {len(isolated_s1)} S1 peaks group")
         print(f"S1 rate is {s1_rate:.3f}Hz")
         print(f"There are {len(main_isolated_s2)} S2 peaks group")
         print(f"S2 rate is {s2_rate * 1e3:.3f}mHz")
         n_hits_2 = isolated_s1["n_hits"] == 2
         n_hits_masks = [n_hits_2, ~n_hits_2]
         truths = []
         for i, mask in enumerate(n_hits_masks):
             if mask.sum() != 0:
                 if self.apply_shadow_matching:
-                    # simulate AC's drift time bin by bin
-                    shadow_reference = self.shadow_reference_selection(
-                        events_salted, main_isolated_s2
-                    )
+                    # simulate drift time bin by bin
+                    shadow_reference, prefix = self.shadow_reference_selection(peaks_salted)
                     truth = self.shadow_matching(
                         isolated_s1[mask],
                         main_isolated_s2,
                         shadow_reference,
                         run_time,
                         self.max_drift_time,
                         self.min_drift_time,
@@ -639,14 +626,15 @@
                         self.preprocess_shadow,
                         self.bootstrap_factor[i],
                         paring_rate_correction,
                         self.shift_dt_shadow_matching,
                         self.n_drift_time_bins,
                         self.shadow_deltatime_exponent,
                         self.max_n_shadow_bins,
+                        prefix,
                     )
                 else:
                     truth = self.simple_pairing(
                         isolated_s1[mask],
                         main_isolated_s2,
                         s1_rate,
                         s2_rate,
@@ -675,16 +663,16 @@
         normalization = np.hstack(
             [
                 np.full(len(truths[0][1][0]), 1 / self.bootstrap_factor[0]),
                 np.full(len(truths[1][1][0]), 1 / self.bootstrap_factor[1]),
             ]
         )
 
-        print(f"AC pairing rate is {paring_rate_full * 1e3:.3f}mHz")
-        print(f"AC event number is {len(drift_time)}")
+        print(f"Pairing rate is {paring_rate_full * 1e3:.3f}mHz")
+        print(f"Event number is {len(drift_time)}")
 
         # make sure events are not very long
         assert (s2_length.max() + drift_time.max()) * 5.0 < self.paring_time_interval
 
         # peaks number in each event
         n_peaks = 1 + s2_n_peaks[s2_group_number]
         slices = self.split_chunks(n_peaks)
@@ -740,14 +728,15 @@
 
 class PeakProximityPaired(PeakProximity):
     __version__ = "0.0.0"
     depends_on = "peaks_paired"
     provides = "peak_proximity_paired"
     data_kind = "peaks_paired"
     save_when = strax.SaveWhen.EXPLICIT
+    allow_hyperrun = True
 
     use_origin_n_competing = straxen.URLConfig(
         default=False,
         type=bool,
         help="Whether use original n_competing",
     )
 
@@ -799,14 +788,15 @@
 
 
 class PeakPositionsPaired(Plugin):
     __version__ = "0.0.0"
     depends_on = "peaks_paired"
     provides = "peak_positions_paired"
     save_when = strax.SaveWhen.EXPLICIT
+    allow_hyperrun = True
 
     def infer_dtype(self):
         return peak_positions_dtype()
 
     def compute(self, peaks_paired):
         result = np.zeros(len(peaks_paired), dtype=self.dtype)
         for q in self.dtype.names:
```

### Comparing `axidence-0.2.2/axidence/plugins/salting/event_building.py` & `axidence-0.3.0/axidence/plugins/salting/event_building.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import warnings
 from typing import Tuple
 import numpy as np
 import strax
+from strax import ExhaustPlugin
 import straxen
 from straxen import Events, EventBasics
 
 from ...utils import needed_dtype, merge_salted_real
-from ...plugin import ExhaustPlugin
 
 
 class EventsSalted(Events, ExhaustPlugin):
-    __version__ = "0.1.0"
+    __version__ = "0.2.0"
     child_plugin = True
     depends_on = ("peaks_salted", "peak_proximity_salted", "peak_basics", "peak_proximity")
     provides = "events_salted"
     data_kind = "events_salted"
     save_when = strax.SaveWhen.EXPLICIT
 
     n_drift_time_window = straxen.URLConfig(
@@ -74,20 +74,14 @@
 
         if self.only_salt_s1 or self.only_salt_s2:
             anchor_peaks = peaks_salted
         else:
             # use S2s as anchors by default
             anchor_peaks = peaks_salted[1::2]
 
-        # check if the salting anchor can trigger
-        if self.only_salt_s1:
-            is_triggering = np.full(len(anchor_peaks), False)
-        else:
-            is_triggering = np.full(len(anchor_peaks), False)
-
         if np.unique(anchor_peaks["type"]).size != 1:
             raise ValueError("Expected only one type of anchor peaks!")
 
         # initial the final result
         if self.only_salt_s1 or self.only_salt_s2:
             n_events = len(peaks_salted)
         else:
@@ -100,45 +94,57 @@
         empty_events = np.empty(len(anchor_peaks), dtype=self.dtype)
         empty_events["time"] = anchor_peaks["time"]
         empty_events["endtime"] = anchor_peaks["endtime"]
 
         # build events at once because if a messy environment
         # make the two anchor in the same event
         # it will be considered as event building failure later
-        events = super().compute(_peaks, start, end)
-        events = strax.split_touching_windows(events, anchor_peaks)
+        _events = super().compute(_peaks, start, end)
+        # touching_windows will return the indices of things repeatedly
+        # as long as the things and container are touched so the events here can be repeated
+        events = strax.split_touching_windows(_events, anchor_peaks)
 
         # there should be only one event near the anchor
         l_events = np.array([len(event) for event in events])
         if not np.all(l_events <= 1):
             raise ValueError(f"Expected one event per anchor, got {l_events.max()}!")
 
         # merge events and placeholders
         _result = np.hstack(
             [events[i] if l_events[i] != 0 else empty_events[i] for i in range(n_events)]
         )
-        # this more fancy way will not be used
-        # _result = np.sort(np.hstack(events + [empty_events[l_events == 0]]), order="time")
+
+        # sanity checks
         if not np.all(np.diff(_result["time"]) >= 0):
             raise ValueError("Expected the result to be sorted!")
+        # some anchors are belonged to a same event
+        index = np.unique(_result["time"], return_index=True)[1]
+        if not np.all(_result["time"][index][1:] - _result["endtime"][index][:-1] >= 0):
+            raise ValueError("Expected the result to be non-overlapping!")
         for n in _result.dtype.names:
             result[n] = _result[n]
 
+        # check if the salting anchor can trigger
+        if self.only_salt_s1:
+            is_triggering = np.full(len(anchor_peaks), False)
+        else:
+            is_triggering = self._is_triggering(anchor_peaks)
+
         # assign the most important parameters
         result["is_triggering"] = is_triggering
         result["salt_number"] = np.unique(peaks_salted["salt_number"])
         result["event_number"] = result["salt_number"]
 
         if np.any(np.diff(result["time"]) < 0):
             raise ValueError("Expected time to be sorted!")
         return result
 
 
 class EventBasicsSalted(EventBasics, ExhaustPlugin):
-    __version__ = "0.0.0"
+    __version__ = "0.1.0"
     child_plugin = True
     depends_on: Tuple[str, ...] = (
         "events_salted",
         "peaks_salted",
         "peak_proximity_salted",
         "peak_basics",
         "peak_proximity",
@@ -176,24 +182,31 @@
             raise ValueError(
                 "Expected salt_number to start from 0 because "
                 f"{self.__class__.__name__} is a ExhaustPlugin plugin!"
             )
 
         _peaks = merge_salted_real(peaks_salted, peaks, self._peaks_dtype)
 
-        result = np.zeros(len(events_salted), dtype=self.dtype)
-        self.set_nan_defaults(result)
+        # we repeated events, so we need to get the unique events
+        # because the fully_contained_in function will only return the first container of the thing
+        _, index, counts = np.unique(events_salted["time"], return_index=True, return_counts=True)
 
-        split_peaks = strax.split_by_containment(_peaks, events_salted)
+        _result = np.zeros(len(index), dtype=self.dtype)
+        self.set_nan_defaults(_result)
 
-        result["time"] = events_salted["time"]
-        result["endtime"] = events_salted["endtime"]
-        result["salt_number"] = events_salted["salt_number"]
-        result["event_number"] = events_salted["event_number"]
+        split_peaks = strax.split_by_containment(_peaks, events_salted[index])
 
-        self.fill_events(result, events_salted, split_peaks)
-        result["is_triggering"] = events_salted["is_triggering"]
+        _result["time"] = events_salted["time"][index]
+        _result["endtime"] = events_salted["endtime"][index]
+
+        self.fill_events(_result, events_salted[index], split_peaks)
 
         for i in [1, 2]:
-            if np.all(result[f"s{i}_salt_number"] < 0):
+            if np.all(_result[f"s{i}_salt_number"] < 0):
                 warnings.warn(f"Found zero triggered salted S{i}!")
+
+        # recover the original event number
+        result = np.repeat(_result, counts)
+        result["is_triggering"] = events_salted["is_triggering"]
+        result["salt_number"] = events_salted["salt_number"]
+        result["event_number"] = events_salted["event_number"]
         return result
```

### Comparing `axidence-0.2.2/axidence/plugins/salting/event_fields.py` & `axidence-0.3.0/axidence/plugins/salting/event_fields.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from typing import Tuple
+import numpy as np
 import strax
 from strax import Plugin
 from straxen import EventShadow, EventAmbience, EventNearestTriggering, EventSEDensity
 
 from ...utils import merge_salted_real
 
 
 class EventFieldsSalted(Plugin):
+    __version__ = "0.1.0"
     child_plugin = True
 
     def compute(self, events_salted, peaks_salted, peaks):
         _peaks = merge_salted_real(peaks_salted, peaks, peaks.dtype)
-        return super().compute(events_salted, _peaks)
+        _, index, counts = np.unique(events_salted["time"], return_index=True, return_counts=True)
+        _result = super().compute(events_salted[index], _peaks)
+        result = np.repeat(_result, counts)
+        return result
 
 
 class EventShadowSalted(EventFieldsSalted, EventShadow):
     __version__ = "0.0.0"
     depends_on = (
         "event_basics_salted",
         "peaks_salted",
```

### Comparing `axidence-0.2.2/axidence/plugins/salting/events_salting.py` & `axidence-0.3.0/axidence/plugins/salting/events_salting.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import numpy as np
+from scipy.interpolate import interp1d
 import strax
-from strax import DownChunkingPlugin
+from strax import ExhaustPlugin, DownChunkingPlugin
 import straxen
 from straxen import units, EventBasics, EventPositions
 
 from ...utils import copy_dtype
 from ...samplers import SAMPLERS
-from ...plugin import ExhaustPlugin
 
 
 class EventsSalting(ExhaustPlugin, DownChunkingPlugin, EventPositions, EventBasics):
-    __version__ = "0.0.0"
+    __version__ = "0.0.1"
     child_plugin = True
     depends_on = "run_meta"
     provides = "events_salting"
     data_kind = "events_salting"
     save_when = strax.SaveWhen.EXPLICIT
 
     salting_seed = straxen.URLConfig(
         default=None,
         type=(int, None),
         help="Seed for salting",
     )
 
     salting_rate = straxen.URLConfig(
-        default=20,
-        type=(int, float),
-        help="Rate of salting in Hz",
+        default=10,
+        type=(int, float, list, tuple),
+        help=(
+            "Rate of salting in Hz, " "if list or tuple, they are the factor for 2 and 3+ hits S1",
+        ),
     )
 
     s1_area_range = straxen.URLConfig(
         default=(1, 150),
         type=(list, tuple),
         help="Range of S1 area in salting",
     )
@@ -45,15 +47,15 @@
         default="exponential",
         type=str,
         help="S1 distribution shape in salting",
     )
 
     s2_distribution = straxen.URLConfig(
         default="exponential",
-        type=str,
+        type=(str, list, tuple),
         help="S2 distribution shape in salting",
     )
 
     veto_length_run_start = straxen.URLConfig(
         default=10**9,
         type=int,
         help="Min time delay in [ns] for events towards the run start boundary",
@@ -61,18 +63,18 @@
 
     veto_length_run_end = straxen.URLConfig(
         default=10**8,
         type=int,
         help="Min time delay in [ns] for events towards the run end boundary",
     )
 
-    s1_n_hits_tight_coincidence = straxen.URLConfig(
-        default=2,
-        type=int,
-        help="Will assign the events's ``s1_n_hits`` and ``s1_tight_coincidence`` by this",
+    assigned_area_fraction_top = straxen.URLConfig(
+        default=1.0,
+        type=(int, float, None),
+        help="Assigned area fraction top for S2",
     )
 
     n_drift_time_window = straxen.URLConfig(
         default=5,
         type=int,
         help="How many max drift time will the event builder extend",
     )
@@ -89,38 +91,48 @@
             ]
         )
 
     def infer_dtype(self):
         dtype_reference = self.refer_dtype()
         required_names = ["time", "endtime", "s1_center_time", "s2_center_time"]
         required_names += ["s1_area", "s2_area", "s1_n_hits", "s1_tight_coincidence"]
+        required_names += ["s2_area_fraction_top"]
         required_names += ["x", "y", "z", "drift_time", "s2_x", "s2_y", "z_naive"]
         dtype = copy_dtype(dtype_reference, required_names)
         # since event_number is int64 in event_basics
         dtype += [(("Salting number of events", "salt_number"), np.int64)]
         return dtype
 
     def setup(self):
         super(EventPositions, self).setup()
         super(EventsSalting, self).setup()
 
         self.init_rng()
 
+        if isinstance(self.salting_rate, (list, tuple)):
+            if len(self.salting_rate) != 2:
+                raise ValueError(
+                    "The length of salting_rate should be 2 " "if provided list or tuple!"
+                )
+            self.hits_salting_rate = list(self.salting_rate)
+        else:
+            self.hits_salting_rate = [self.salting_rate] * 2
+
     def init_rng(self):
         """Initialize the random number generator."""
         if self.salting_seed is None:
             self.rng = np.random.default_rng(seed=int(self.run_id))
         else:
             self.rng = np.random.default_rng(seed=self.salting_seed)
 
     def sample_time(self, start, end):
         """Sample the time according to the start and end of the run."""
-        self.event_time_interval = int(units.s // self.salting_rate)
+        self.event_time_interval = int(units.s // sum(self.hits_salting_rate))
 
-        if units.s / self.salting_rate < self.drift_time_max * self.n_drift_time_window * 2:
+        if self.event_time_interval < self.drift_time_max * self.n_drift_time_window * 2:
             raise ValueError("Salting rate is too high according the drift time window!")
 
         time = np.arange(
             start + self.veto_length_run_start,
             end - self.veto_length_run_end,
             self.event_time_interval,
         ).astype(np.int64)
@@ -141,25 +153,47 @@
             )
         )
         self.slices = np.vstack([slices_idx[:-1], slices_idx[1:]]).T.astype(int).tolist()
 
         self.time_left = self.event_time_interval // 2
         self.time_right = self.event_time_interval - self.time_left
 
+    @staticmethod
+    def sample_area(distribution, area_range, n_events, rng):
+        """Sample the area according to the distribution."""
+        if isinstance(distribution, str):
+            area = SAMPLERS[distribution](area_range).sample(n_events, rng)
+        else:
+            if not all(isinstance(d, (list, tuple)) for d in distribution):
+                raise ValueError("Distribution should be (x_array, y_array) if not str!")
+            if distribution[0][0] != 0 or distribution[0][-1] != 1:
+                raise ValueError("The x_array of distribution should be normalized!")
+            cdf = rng.uniform(0, 1, size=n_events)
+            area = interp1d(distribution[0], distribution[1])(cdf)
+        return area
+
+    def sample_area_fraction_top(self, s2_area, s2_x, s2_y):
+        return self.assigned_area_fraction_top
+
     def sampling(self, start, end):
         """Sample the features of events, (t, x, y, z, S1, S2) et al."""
         time = self.sample_time(start, end)
         self.n_events = len(time)
         self.events_salting = np.empty(self.n_events, dtype=self.dtype)
         self.events_salting["salt_number"] = np.arange(self.n_events)
         self.events_salting["time"] = time
         self.events_salting["endtime"] = time
 
-        self.events_salting["s1_n_hits"] = self.s1_n_hits_tight_coincidence
-        self.events_salting["s1_tight_coincidence"] = self.s1_n_hits_tight_coincidence
+        self.events_salting["s1_n_hits"] = 2
+        self.events_salting["s1_tight_coincidence"] = 2
+        n_3hits = round(self.n_events * self.hits_salting_rate[1] / sum(self.hits_salting_rate))
+        if n_3hits > 0:
+            indices = self.rng.choice(self.n_events, size=n_3hits, replace=False)
+            self.events_salting["s1_n_hits"][indices] = 3
+            self.events_salting["s1_tight_coincidence"][indices] = 3
 
         theta = self.rng.random(size=self.n_events) * 2 * np.pi - np.pi
         r = np.sqrt(self.rng.random(size=self.n_events)) * straxen.tpc_r
         self.events_salting["x"] = np.cos(theta) * r
         self.events_salting["y"] = np.sin(theta) * r
         self.events_salting["z"] = -self.rng.random(size=self.n_events) * straxen.tpc_z
         s2_x, s2_y, z_naive = self.inverse_field_distortion(
@@ -176,24 +210,30 @@
         ) / self.electron_drift_velocity
 
         self.events_salting["s1_center_time"] = time - self.events_salting["drift_time"]
         self.events_salting["s2_center_time"] = time
 
         s1_area_range = (float(self.s1_area_range[0]), float(self.s1_area_range[1]))
         s2_area_range = (float(self.s2_area_range[0]), float(self.s2_area_range[1]))
-        self.events_salting["s1_area"] = SAMPLERS[self.s1_distribution](s1_area_range).sample(
-            self.n_events, self.rng
+        self.events_salting["s1_area"] = self.sample_area(
+            self.s1_distribution, s1_area_range, self.n_events, self.rng
         )
-        self.events_salting["s2_area"] = SAMPLERS[self.s2_distribution](s2_area_range).sample(
-            self.n_events, self.rng
+        self.events_salting["s2_area"] = self.sample_area(
+            self.s2_distribution, s2_area_range, self.n_events, self.rng
         )
         # to prevent numerical errors
         self.events_salting["s1_area"] = np.clip(self.events_salting["s1_area"], *s1_area_range)
         self.events_salting["s2_area"] = np.clip(self.events_salting["s2_area"], *s2_area_range)
 
+        self.events_salting["s2_area_fraction_top"] = self.sample_area_fraction_top(
+            self.events_salting["s2_area"],
+            self.events_salting["s2_x"],
+            self.events_salting["s2_y"],
+        )
+
         if np.any(np.diff(self.events_salting["time"]) <= 0):
             raise ValueError("The time is not strictly increasing!")
 
         self.set_chunk_splitting()
 
     def compute(self, run_meta, start, end):
         """Copy and assign the salting events into chunk."""
```

### Comparing `axidence-0.2.2/axidence/plugins/salting/peak_correlation.py` & `axidence-0.3.0/axidence/plugins/salting/peak_correlation.py`

 * *Files identical despite different names*

### Comparing `axidence-0.2.2/axidence/plugins/salting/peaks_salted.py` & `axidence-0.3.0/axidence/plugins/salting/peaks_salted.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import straxen
 from straxen import PeakBasics
 
 from ...utils import copy_dtype
 
 
 class PeaksSalted(PeakBasics):
-    __version__ = "0.0.0"
+    __version__ = "0.0.1"
     child_plugin = True
     depends_on = "events_salting"
     provides = "peaks_salted"
     data_kind = "peaks_salted"
     save_when = strax.SaveWhen.EXPLICIT
 
     only_salt_s1 = straxen.URLConfig(
@@ -28,15 +28,15 @@
 
     def refer_dtype(self):
         return strax.unpack_dtype(strax.to_numpy_dtype(super(PeaksSalted, self).infer_dtype()))
 
     def infer_dtype(self):
         dtype_reference = self.refer_dtype()
         required_names = ["time", "endtime", "center_time"]
-        required_names += ["area", "n_hits", "tight_coincidence", "type"]
+        required_names += ["area", "area_fraction_top", "n_hits", "tight_coincidence", "type"]
         dtype = copy_dtype(dtype_reference, required_names)
         # since event_number is int64 in event_basics
         dtype += [
             (("Reconstructed S2 X position (cm), uncorrected", "x"), np.float32),
             (("Reconstructed S2 Y position (cm), uncorrected", "y"), np.float32),
             (("Salting number of peaks", "salt_number"), np.int64),
         ]
@@ -63,15 +63,15 @@
         for n in "n_hits tight_coincidence".split():
             peaks_salted[n] = np.vstack(
                 [
                     events_salting[f"s1_{n}"],
                     np.full(len(events_salting), -1),
                 ]
             ).T.flatten()
-        for n in "x y".split():
+        for n in "x y area_fraction_top".split():
             peaks_salted[n] = np.vstack(
                 [
                     np.full(len(events_salting), np.nan),
                     events_salting[f"s2_{n}"],
                 ]
             ).T.flatten()
         peaks_salted["type"] = np.vstack(
```

### Comparing `axidence-0.2.2/axidence/samplers.py` & `axidence-0.3.0/axidence/samplers.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,21 +30,22 @@
 
     @property
     def bins(self):
         if not isinstance(self.n_bins, int):
             raise ValueError(f"n_bins must be int, not {type(self.n_bins)}, got {self.n_bins}!")
         return self.inverse_transform(np.linspace(*self.transform(self.interval), self.n_bins + 1))
 
-    def reweight(self, x, reference):
+    def reweight(self, x, reference, reference_weights=None):
         h_x = np.histogram(x, bins=self.bins)[0]
-        h_reference = np.histogram(reference, bins=self.bins)[0]
+        h_reference = np.histogram(reference, bins=self.bins, weights=reference_weights)[0]
         _weights = h_reference / h_x
+        indices = np.clip(np.digitize(x, self.bins) - 1, 0, len(self.bins) - 2)
         weights = np.where(
             (x > self.bins[0]) & (x < self.bins[-1]),
-            _weights[np.digitize(np.clip(x, self.bins[0], self.bins[-1]), self.bins) - 1],
+            _weights[indices],
             0.0,
         )
         return weights
 
 
 class UniformSampler(Sampler):
     def transform(self, interval):
```

### Comparing `axidence-0.2.2/axidence/utils.py` & `axidence-0.3.0/axidence/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,28 +31,32 @@
         if not found:
             raise ValueError(f"Could not find {n} in {dtype_reference}!")
     return dtype
 
 
 def needed_dtype(deps, dependencies_by_kind, func):
     # intersection depends_on's dtype.names will be needed in event building
-    needed_fields = func(
-        *tuple(
-            set.union(*tuple(set(deps[d].dtype_for(d).names) for d in dk))
-            for dk in dependencies_by_kind
-        )
-    )
-    dtype_reference = list(
+    needed_fields = sorted(
         func(
             *tuple(
-                set.union(*tuple(set(deps[d].dtype_for(d).descr) for d in dk))
+                set.union(*tuple(set(deps[d].dtype_for(d).names) for d in dk))
                 for dk in dependencies_by_kind
             )
         )
     )
+    dtype_reference = sorted(
+        list(
+            func(
+                *tuple(
+                    set.union(*tuple(set(deps[d].dtype_for(d).descr) for d in dk))
+                    for dk in dependencies_by_kind
+                )
+            )
+        )
+    )
     _peaks_dtype = copy_dtype(dtype_reference, needed_fields)
     if len(_peaks_dtype) != len(needed_fields):
         raise ValueError(
             f"Weird! Could not find all needed fields {needed_fields} in {dtype_reference}!"
         )
     return needed_fields, np.dtype(_peaks_dtype)
```

### Comparing `axidence-0.2.2/pyproject.toml` & `axidence-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "axidence"
-version = "0.2.2"
+version = "0.3.0"
 description = "strax-based data-driven accidental coincidence background simulation and peak-level salting"
 readme = "README.md"
 license = "BSD-3-Clause"
 authors = [
   "Dacheng Xu, <dx2227@columbia.edu>",
 ]
 requires-python = ">=3.9"
@@ -18,14 +18,14 @@
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 repository = "https://github.com/dachengx/axidence"
 documentation = "https://readthedocs.org/projects/axidence/"
 
 [tool.poetry.dependencies]
-strax = ">=1.6.2"
+strax = ">=1.6.3"
 straxen = ">=2.2.1"
 GOFevaluation = ">=0.1.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.8", "setuptools>=61.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `axidence-0.2.2/PKG-INFO` & `axidence-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axidence
-Version: 0.2.2
+Version: 0.3.0
 Summary: strax-based data-driven accidental coincidence background simulation and peak-level salting
 Home-page: https://github.com/dachengx/axidence
 License: BSD-3-Clause
 Author: Dacheng Xu,
 Author-email: dx2227@columbia.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: GOFevaluation (>=0.1.4)
-Requires-Dist: strax (>=1.6.2)
+Requires-Dist: strax (>=1.6.3)
 Requires-Dist: straxen (>=2.2.1)
 Project-URL: Documentation, https://readthedocs.org/projects/axidence/
 Project-URL: Repository, https://github.com/dachengx/axidence
 Description-Content-Type: text/markdown
 
 # Axidence
```

