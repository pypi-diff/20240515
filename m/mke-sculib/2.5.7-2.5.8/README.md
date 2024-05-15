# Comparing `tmp/mke_sculib-2.5.7.tar.gz` & `tmp/mke_sculib-2.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.5.7.tar", last modified: Mon May 13 18:13:19 2024, max compression
+gzip compressed data, was "mke_sculib-2.5.8.tar", last modified: Wed May 15 19:54:01 2024, max compression
```

## Comparing `mke_sculib-2.5.7.tar` & `mke_sculib-2.5.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 18:13:19.256970 mke_sculib-2.5.7/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.5.7/LICENSE
--rw-rw-rw-   0        0        0     4120 2024-05-13 18:13:19.256970 mke_sculib-2.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.5.7/README.rst
--rw-rw-rw-   0        0        0     1017 2024-05-13 18:13:19.257957 mke_sculib-2.5.7/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:13:19.231105 mke_sculib-2.5.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 18:13:19.247969 mke_sculib-2.5.7/src/mke_sculib/
--rw-rw-rw-   0        0        0     1216 2024-05-13 18:12:53.000000 mke_sculib-2.5.7/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0   102025 2024-05-11 06:53:52.000000 mke_sculib-2.5.7/src/mke_sculib/acu.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.5.7/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.5.7/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.5.7/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0    10152 2024-05-11 15:06:30.000000 mke_sculib-2.5.7/src/mke_sculib/js_helpers.py
--rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.5.7/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0   106939 2024-05-13 18:12:43.000000 mke_sculib-2.5.7/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.5.7/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.5.7/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:13:19.254973 mke_sculib-2.5.7/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-05-13 18:13:19.000000 mke_sculib-2.5.7/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2024-05-13 18:13:19.000000 mke_sculib-2.5.7/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:13:19.000000 mke_sculib-2.5.7/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-13 18:13:19.000000 mke_sculib-2.5.7/src/mke_sculib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 18:13:19.000000 mke_sculib-2.5.7/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 18:13:19.255956 mke_sculib-2.5.7/tests/
--rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.5.7/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.5.7/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:54:01.397412 mke_sculib-2.5.8/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.5.8/LICENSE
+-rw-rw-rw-   0        0        0     4120 2024-05-15 19:54:01.397412 mke_sculib-2.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.5.8/README.rst
+-rw-rw-rw-   0        0        0     1017 2024-05-15 19:54:01.398412 mke_sculib-2.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:54:01.381408 mke_sculib-2.5.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 19:54:01.392411 mke_sculib-2.5.8/src/mke_sculib/
+-rw-rw-rw-   0        0        0     1216 2024-05-15 19:50:49.000000 mke_sculib-2.5.8/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0   102025 2024-05-11 06:53:52.000000 mke_sculib-2.5.8/src/mke_sculib/acu.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.5.8/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.5.8/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.5.8/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0    10152 2024-05-11 15:06:30.000000 mke_sculib-2.5.8/src/mke_sculib/js_helpers.py
+-rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.5.8/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0   108468 2024-05-15 19:53:14.000000 mke_sculib-2.5.8/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    21285 2024-05-15 19:50:24.000000 mke_sculib-2.5.8/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.5.8/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:54:01.395412 mke_sculib-2.5.8/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2024-05-15 19:54:01.000000 mke_sculib-2.5.8/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2024-05-15 19:54:01.000000 mke_sculib-2.5.8/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:54:01.000000 mke_sculib-2.5.8/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-15 19:54:01.000000 mke_sculib-2.5.8/src/mke_sculib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 19:54:01.000000 mke_sculib-2.5.8/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 19:54:01.396412 mke_sculib-2.5.8/tests/
+-rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.5.8/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.5.8/tests/test_scu.py
```

### Comparing `mke_sculib-2.5.7/LICENSE` & `mke_sculib-2.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.7/PKG-INFO` & `mke_sculib-2.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.5.7
+Version: 2.5.8
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.5.7/README.rst` & `mke_sculib-2.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.7/setup.cfg` & `mke_sculib-2.5.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.7/src/mke_sculib/__init__.py` & `mke_sculib-2.5.8/src/mke_sculib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.5.7'
+__version__ = '2.5.8'
 
 from mke_sculib.scu import scu as scu_api, plot_tt, print_color, colors
 from mke_sculib.sim import scu_sim
 from mke_sculib.stellarium_api import stellarium_api as stellar_api
 from mke_sculib.sim import plot_motion_pyplot as plot_motion
 from mke_sculib.helpers import get_utcnow, make_zulustr, parse_zulutime
```

### Comparing `mke_sculib-2.5.7/src/mke_sculib/acu.py` & `mke_sculib-2.5.8/src/mke_sculib/acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.7/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.5.8/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.7/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.5.8/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.7/src/mke_sculib/helpers.py` & `mke_sculib-2.5.8/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.7/src/mke_sculib/js_helpers.py` & `mke_sculib-2.5.8/src/mke_sculib/js_helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.7/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.5.8/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.7/src/mke_sculib/scu.py` & `mke_sculib-2.5.8/src/mke_sculib/scu.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,23 +263,23 @@
             log('WARNING, logger already recording - attempting to stop and start a fresh logger...', color=colors.WARNING)
             scu.stop_logger()  
             scu.wait_duration(2, not self.verb)
         
         log(f'Uploading tracking table...', color=colors.OKBLUE)
         dt_wait = scu.upload_track_table(t, az, el, wait_for_start=False)
         t_now = scu.t_internal
-        if self.wait_start and t_start - 3*u.s > t_now:
-            log(f'Waiting for track start time. dt={(t_now - t_start).to(u.s) - 3*u.s}', color=colors.OKBLUE)
+        if self.wait_start and (t_start - 3*u.s) > t_now:
+            log(f'Waiting for track start time. dt={(t_start - t_now).to(u.s) - 3*u.s}', color=colors.OKBLUE)
             scu.wait_until(t_start - 3*u.s, not self.verb)
 
         if activate_logging:
             # start logging for my testrun
             scu.start_logger(config_name=config_name, stop_if_need=False)
         
-        if self.wait_start and t_start - 3*u.s > scu.t_internal:
+        if self.wait_start and (t_start - 3*u.s) > scu.t_internal:
             scu.wait_until(t_start, not self.verb)
         log(f'Waiting for state to be either TRACK or SLEW...', color=colors.OKBLUE)
         scu.wait_state('acu.general_management_and_controller.state', ['TRACK', "SLEW"], timeout=20, query_delay=.25, operator = 'IN')
         return self
     
     def __exit__(self, *args):
         scu = self.scu
@@ -351,14 +351,20 @@
         self.dish_type = dish_type.lower()
         self.bands_possible = bands_dc
         self.post_put_delay = post_put_delay
 
         self.use_socket = use_socket
         self.data_streamer = DataStreamHandler(self)
 
+    def keys(self):
+        if self.use_socket:
+            return self.data_streamer.data.keys()
+        else:
+            return self.get_channel_list(with_values=False, with_timestamps=False)
+        
     @property
     def address(self):
         return f'http://{self.ip}:{self.port}'
     
     @property
     def version_acu(self):
         if self.dish_type == 'mke':
@@ -785,15 +791,15 @@
     #         b = self.status_Value("acu.tracking.act_pt_act_index_a")
     #         return (int(a) - int(b)) > 0
         
 
     #     self.wait_by_testfun(tester, timeout, query_delay)
     #     log('   -> done')
 
-    def wait_settle(self, axis='all', timeout=600, query_delay=.25, tolerance=0.01, wait_by_pos=True, initial_delay=1.0):
+    def wait_settle(self, axis='all', timeout=600, query_delay=.25, tolerance=0.01, wait_by_pos=True, initial_delay=2.0):
         """
         alias for waitForStatusValue but mapping 'AZ', 'EL', 'FI' to 'acu.azimuth.p_act'
         'acu.elevation.p_act' and 'acu.feed_indexer.p_act'
 
         Periodically queries a device status 'path' until a specific value is reached.
 
         Args:
@@ -999,16 +1005,19 @@
                 if not no_stout and not is_first:
                     log('  -> done', color=colors.OKBLUE)
                 return True
 
             if not no_stout and is_first:
                 if isinstance(value, float):
                     log('wait for {}: {:.3f} (currently at: {:.3f})'.format(path, value, v), color=colors.OKBLUE)
+                elif 'state' in path:
+                    log('wait for {}: {} (currently at: {})'.format(path, state_dc.get(value, value), state_dc.get(v, v)), color=colors.OKBLUE)
                 else:
                     log('wait for {}: {} (currently at: {})'.format(path, value, v), color=colors.OKBLUE)
+
                 is_first = False
 
             self.wait_duration(query_delay, no_stout=True)  
 
         err = "Sensor: {} not equal to {} after {}s. Current value: {}".format(path, value, timeout, v)
         log(err, color=colors.FAIL)
         raise TimeoutError(err)
@@ -1078,15 +1087,15 @@
     #commands to ACU
     def deactivate_lowpowermode(self):
         return self.scu_put("/devices/command", {"path":"acu.dish_management_controller.set_power_mode","params":{"action":"0"}}).text
     
     def activate_lowpowermode(self):
         return self.scu_put("/devices/command", {"path":"acu.dish_management_controller.set_power_mode","params":{"action":"1"}}).text
 
-    def stow(self, pre_move=True):
+    def stow(self, pre_move=True, nowait=False):
         """stow the antenna on pos 1 (both axes) and wait for stowing to be completed
         """
         log('Stowing...')
 
 
         if self.get_state() != 'Stowed':
 
@@ -1099,56 +1108,56 @@
                 self.reset_dmc() # because the ACU seems to be ignoring stows sometimes if this is not done 
                 self.scu_put("/devices/command", {"path": "acu.azimuth.drive_to_stow", "params":{"action": "1"}})
                 self.wait_duration(1.0)
                 self.scu_put("/devices/command", {"path": "acu.elevation.drive_to_stow", "params":{"action": "1"}})
             else:
                 self.scu_put("/devices/command", {"path": "acu.dish_management_controller.stow", "params": {"action": "1"}})
 
-
-        self.wait_state("acu.stow_pin_controller.azimuth_status", "DEPLOYED", operator='==')
-        self.wait_state("acu.stow_pin_controller.elevation_status", "DEPLOYED", operator='==')
-        self.wait_duration(1, no_stout=True)  
+        if not nowait:
+            self.wait_state("acu.stow_pin_controller.azimuth_status", "DEPLOYED", operator='==')
+            self.wait_state("acu.stow_pin_controller.elevation_status", "DEPLOYED", operator='==')
+            self.wait_duration(1, no_stout=True)  
         
-    def unstow(self):
+    def unstow(self, nowait=False):
         """
         Unstow both axes
         """
         log('Unstowing...')
         self.scu_put("/devices/command", {"path": "acu.dish_management_controller.unstow"})
 
 
-
-        self.wait_duration(3, no_stout=True)      
-        self.wait_state("acu.stow_pin_controller.azimuth_status", "RETRACTED", operator='==')
-        self.wait_state("acu.stow_pin_controller.elevation_status", "RETRACTED", operator='==')
-        self.wait_duration(1, no_stout=True)  
+        if not nowait:
+            self.wait_duration(3, no_stout=True)      
+            self.wait_state("acu.stow_pin_controller.azimuth_status", "RETRACTED", operator='==')
+            self.wait_state("acu.stow_pin_controller.elevation_status", "RETRACTED", operator='==')
+            self.wait_duration(1, no_stout=True)  
 
 
     def activate_axes(self):
         """
         Activate axes
         """
         self.scu_put("/devices/command", {"path": "acu.azimuth.activate"})
         self.scu_put("/devices/command", {"path": "acu.elevation.activate"})
 
         self.wait_duration(1, no_stout=True)
-        self.waitForStatusValue("acu.azimuth.axis_bit_status.abs_active", True, timeout=10)
-        self.waitForStatusValue("acu.elevation.axis_bit_status.abs_active", True, timeout=10)
+        self.waitForStatusValue("acu.azimuth.axis_bit_status.abs_active", True, timeout=15)
+        self.waitForStatusValue("acu.elevation.axis_bit_status.abs_active", True, timeout=15)
 
 
     def deactivate_axes(self):
         """
         Activate axes
         """
         self.scu_put("/devices/command", {"path": "acu.azimuth.deactivate"})
         self.scu_put("/devices/command", {"path": "acu.elevation.deactivate"})
 
         self.wait_duration(1, no_stout=True)        
-        self.waitForStatusValue("acu.azimuth.axis_bit_status.abs_active", False, timeout=10)
-        self.waitForStatusValue("acu.elevation.axis_bit_status.abs_active", False, timeout=10)
+        self.waitForStatusValue("acu.azimuth.axis_bit_status.abs_active", False, timeout=15)
+        self.waitForStatusValue("acu.elevation.axis_bit_status.abs_active", False, timeout=15)
 
 
     def release_command_authority(self):
         """
         Release command authority.
         """
         log('Releasing Command Authority...')
@@ -1844,20 +1853,40 @@
         """
         if not no_stout:
             log('wait for {:.1f}s'.format(seconds), color=colors.OKBLUE)
         time.sleep(seconds)
         # if not no_stout:
         #     log('  -> done', color=colors.OKBLUE)
 
+    # def set_time_source(self, select='2'):
+    #     self.scu_put("/devices/command", payload={"path": "time_controller.time_source",
+    #                 "params": {"time_controller.time_source.choose_time_source": str(select)}})
+        
     #Simplified track table functions
         
     def __point_toggle(self, action, select):
         self.scu_put("/devices/command", payload={"path": "acu.pointing_controller.pointing_correction_toggle",
                     "params": {"action": str(action), "select": str(select)}})
+
         
+    def time_test(self):
+        try:
+            tworld = requests.get('http://worldtimeapi.org/api/timezone/utc').json()['utc_datetime']
+        except Exception as err:
+            tworld = 'Error while fetching: ' + str(err)
+        
+        dct = {'local_ntp': Time.now().iso, 
+            'worldtimeapi': tworld,
+            'D119_ptp_direct' : Time(self['acu.time.external_ptp'], format='mjd').iso,
+            'D119A_internal': self.t_internal.iso, 
+            }
+        return dct
+    
+
+
 
     def point_all_ON(self):
         self.__point_toggle(1, '1')
 
     def point_all_OFF(self):
         self.__point_toggle(0, '1')
     
@@ -2450,55 +2479,69 @@
 
     if do_show:
         plt.show()
 
     return f, (ax1, ax2)
         
         
-if __name__ == '__main__':
-    log("main")
+# if __name__ == '__main__':
+#     log("main")
+
+#     # print(websockets.__version__)
+#     # with websockets.sync.client.connect(f'ws://{"10.96.66.10"}:{8080}/wsstatus') as ws:
+#     #     print('success!')
+
+#     # from astropy.time import Time
+#     # from astropy import units as u
+
+#     d119 = scu('http://10.96.66.10:8080/', debug=False, use_socket=True)
 
-    # print(websockets.__version__)
-    # with websockets.sync.client.connect(f'ws://{"10.96.66.10"}:{8080}/wsstatus') as ws:
-    #     print('success!')
+#     d119.set_time_source()
+
+#     d119.wait_duration(10)
+    
+#     print({k:v for k, v in d119.get_channel_list(with_values=True) if 'time' in k})
+
+#     # stream = DataStreamHandler(d119)
+#     # stream.start()
+#     # while 1:
+#     #     print(f'{stream.t_last_local=} | {stream.t_last_remote=}')
+#     # try:
 
-    # from astropy.time import Time
-    # from astropy import units as u
 
-    d119 = scu('http://10.96.66.10:8080/', debug=False, use_socket=True)
 
-    # stream = DataStreamHandler(d119)
-    # stream.start()
-    # while 1:
-    #     print(f'{stream.t_last_local=} | {stream.t_last_remote=}')
-    # try:
+#     el = 80
 
+#     az, el = 0, 15
 
+#     d119.move_to_azel(az, el)
+#     d119.wait_settle()
+#     print(d119.azel)
+#     d119.reset_dmc()
 
-    el = 80
+#     #t0 = datetime.datetime.now(tz=datetime.timezone.utc)
+#     t0 = d119.t_internal.datetime
+#     t0p = t0.replace(second=0, microsecond=0)
 
 
-    azp = np.append(np.arange(-30, 0, 1.), np.arange(0, -30, 1.))
-    azs = azp.copy()
-    els = np.ones_like(azp) * el
 
-    for el in [70, 60, 50, 40, 30, 20]:
-        azs = np.append(azs, azp)
-        els = np.append(els, np.ones_like(azp) * el)
-    t = np.arange(0, len(azs)) * u.s
+#     t0, t0p
+#     if t0.second > 30:
+#         t00 = Time(t0p) + 2*u.minute
+#     else:
+#         t00 = Time(t0p) + 1*u.minute
+
+    
+#     t = np.arange(0, 60, 0.5)
+#     azs = np.linspace(az, az+10, len(t))
+#     els = np.ones_like(t) * el
+#     tmjd = (t00 + t * u.s).mjd
 
-    d119.move_to_azel(azs[0], els[0])
-    d119.wait_settle()
-    # d119.start()
-    print(d119.azel)
-    d119.reset_dmc()
-    d119.run_track_table((d119.t_internal + t).mjd, azs, els, wait_start=False, verb=True)
+#     d119.run_track_table(tmjd, azs, els, wait_start=False, verb=True)
 
-    d119.wait_duration(10.)
-    d119.shutdown()
     # finally:
     #     d119.shutdown()
     # D119A.reset_dmc()
     # D119A.stow()
 
     # D119A.move_to_azel(45, 80)
     # D119A.wait_settle()
```

### Comparing `mke_sculib-2.5.7/src/mke_sculib/sim.py` & `mke_sculib-2.5.8/src/mke_sculib/sim.py`

 * *Files 10% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     (ahead of time) in order to debug test scripts etc.
 
     This simulators motion control capabilities as well as functional interface is reduced 
     compared to a real antenna.
 
     (This class inherits from a real SCU interface object and overwrites the communication channels)
     """
-    def __init__(self, address='', ip='', port='8080', use_realtime=False, debug=True, speedup_factor=1, t_start = astropy.time.Time.now(), UPDATE_INTERVAL = .1, lims_az=(-270.0, 270, 3.0), lims_el=(15, 90, 1.35), dish_type='mke', post_put_delay=0.0):
+    def __init__(self, address='', ip='', port='8080', use_realtime=False, debug=True, speedup_factor=1, t_start = astropy.time.Time.now(), UPDATE_INTERVAL = .1, lims_az=(-270.0, 270, 3.0), lims_el=(15, 90, 1.35), dish_type='mke', post_put_delay=0.0, **kwargs):
         """create an antenna scu/acu simulator object, which can be used to simulate the motion of
         a real Antenna in simulation time (ahead of time) in order to debug test scripts etc.
 
         This simulators motion control capeabilities as well as functional interface is reduced 
         compared to a real antenna.
 
         Args:
@@ -161,16 +161,71 @@
                                     use_realtime = use_realtime, 
                                     UPDATE_INTERVAL = UPDATE_INTERVAL, 
                                     do_write_history=True)        
 
         self.routes = get_routes(self.telescope)
 
 
-        scu.scu.__init__(self, address=address, ip=ip, port=port, debug=debug, lims_az=lims_az, lims_el=lims_el, dish_type=dish_type, post_put_delay=post_put_delay)
+        scu.scu.__init__(self, address=address, ip=ip, port=port, debug=debug, lims_az=lims_az, lims_el=lims_el, dish_type=dish_type, post_put_delay=post_put_delay, use_socket=False)
+    
+
+    @property
+    def data_streamer(self):
+        return None
+
+    @data_streamer.setter
+    def data_streamer(self, value):
+        pass
+
+    @property
+    def use_socket(self):
+        return None
+    
+    @use_socket.setter
+    def use_socket(self, value):
+        pass
+
+    @property
+    def data(self):
+        return self.telescope.data
 
+    def getc(self, key, as_dict=False):
+        """get one or many channel values. key(s) must be string or list of strings
+
+        Args:
+            key (string or iterable[str]): the channel names to get
+
+        Returns:
+            dict, list or immuteable: type depending on the input.
+        """
+        try:
+            if self.use_socket:
+                if isinstance(key, str):
+                    return {key: self[key]} if as_dict else self[key]
+                else:
+                    return self.get_many(channels=key, as_dict=as_dict)
+        except Exception as err:
+            log(f'error while getting data from socket stream... falling back to HTTP api. {err=}', color=colors.WARNING)
+
+        if key is None:
+            return dict(self.get_channel_list(with_values=True, with_timestamps=False))
+        elif not isinstance(key, str) and hasattr(self, '__len__'):
+            allchans = self.data
+            if as_dict:
+                return {k:allchans[k] for k in key}
+            else:
+                return [allchans[k] for k in key]
+        else:
+            return self._get_device_status_value(key)
+
+    def __getitem__(self, key):
+        return self.data[key]
+    
+    def __contains__(self, key):
+        return key in self.data
 
     @property
     def t_internal(self):
         """internal telescope time as astropy Time object based on MJD format
 
         Returns:
             astropy.time.Time: the ACU internal time now
@@ -316,15 +371,15 @@
             send_default_configs (bool, optional): Whether or not to generate the default logging configs on the SCU on startup. Defaults to True.
         """
 
         log('=== INITIATING STARTUP ROUTINE ===')
         self.get_command_authority()
         # self.reset_dmc()
         self.wait_duration(3)
-        self.unstow()
+        self.unstow(nowait=True)
 
         self.wait_duration(5)
         # self.activate_dmc()
         self.wait_duration(5)
         # self.activate_axes()
         self.wait_duration(5)
 
@@ -340,15 +395,15 @@
             self.wait_duration(3)
         log('=== STARTUP ROUTINE COMPLETED ===')
 
     def shutdown(self):
         """Stow, deactivate, and release command authority for antenna in order to finish before handing back the antenna
         """
         log('=== INITIATING SHUTDOWN ROUTINE ===')
-        self.stow()
+        self.stow(nowait=True)
         self.wait_duration(5)
         # self.deactivate_axes()
         self.wait_duration(5)
         # self.deactivate_dmc()
         self.wait_duration(5)
         self.release_command_authority()
         self.wait_duration(5)
@@ -422,15 +477,15 @@
     for ax, s, c in zip(axs[1:], telescope_axes, colors):
         setp, actp = f'acu.{s}.p_set', f'acu.{s}.p_act'
 
         ax.plot(x, df[setp], '-k')
         ax.plot(x, df[actp], '-' + c)
 
         if df_tt is not None and s in df_tt:
-            ax.plot(x_tt, df_tt[s], ':k')
+            ax.plot(x_tt, df_tt[s], ':k', label=f'tracking table: {s}')
 
         if xlims is None:
             xlims = ax.get_xlim()
 
         act_lim_l, act_lim_h  = ax.get_ylim()
         lim_l, lim_h = lims[s]
```

### Comparing `mke_sculib-2.5.7/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.5.8/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.7/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.5.8/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.5.7
+Version: 2.5.8
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.5.7/src/mke_sculib.egg-info/SOURCES.txt` & `mke_sculib-2.5.8/src/mke_sculib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.7/tests/test_acu_sim.py` & `mke_sculib-2.5.8/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.7/tests/test_scu.py` & `mke_sculib-2.5.8/tests/test_scu.py`

 * *Files identical despite different names*

