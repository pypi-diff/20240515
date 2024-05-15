# Comparing `tmp/reolink_aio-0.8.8.tar.gz` & `tmp/reolink_aio-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reolink_aio-0.8.8.tar", last modified: Mon Feb 19 18:10:23 2024, max compression
+gzip compressed data, was "reolink_aio-0.8.9.tar", last modified: Sun Mar  3 16:52:03 2024, max compression
```

## Comparing `reolink_aio-0.8.8.tar` & `reolink_aio-0.8.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:10:23.031134 reolink_aio-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-02-19 18:10:23.027135 reolink_aio-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:10:23.027135 reolink_aio-0.8.8/reolink_aio/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/reolink_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   226519 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/reolink_aio/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/reolink_aio/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/reolink_aio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/reolink_aio/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/reolink_aio/software_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/reolink_aio/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15466 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/reolink_aio/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/reolink_aio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:10:23.027135 reolink_aio-0.8.8/reolink_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-02-19 18:10:23.000000 reolink_aio-0.8.8/reolink_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-19 18:10:23.000000 reolink_aio-0.8.8/reolink_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 18:10:23.000000 reolink_aio-0.8.8/reolink_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 18:10:22.000000 reolink_aio-0.8.8/reolink_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-19 18:10:23.000000 reolink_aio-0.8.8/reolink_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-19 18:10:23.000000 reolink_aio-0.8.8/reolink_aio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 18:10:23.031134 reolink_aio-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:10:23.027135 reolink_aio-0.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    15443 2024-02-19 18:10:15.000000 reolink_aio-0.8.8/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:52:03.326796 reolink_aio-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-03-03 16:52:03.326796 reolink_aio-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:52:03.326796 reolink_aio-0.8.9/reolink_aio/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   229509 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/software_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15466 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:52:03.326796 reolink_aio-0.8.9/reolink_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-03-03 16:52:03.000000 reolink_aio-0.8.9/reolink_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-03 16:52:03.000000 reolink_aio-0.8.9/reolink_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 16:52:03.000000 reolink_aio-0.8.9/reolink_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 16:52:03.000000 reolink_aio-0.8.9/reolink_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-03 16:52:03.000000 reolink_aio-0.8.9/reolink_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-03 16:52:03.000000 reolink_aio-0.8.9/reolink_aio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 16:52:03.326796 reolink_aio-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:52:03.326796 reolink_aio-0.8.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15443 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/tests/test.py
```

### Comparing `reolink_aio-0.8.8/LICENSE` & `reolink_aio-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.8/PKG-INFO` & `reolink_aio-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink_aio
-Version: 0.8.8
+Version: 0.8.9
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink_aio Version: 0.8.8 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink_aio Version: 0.8.9 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.8.8/README.md` & `reolink_aio-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.8/reolink_aio/api.py` & `reolink_aio-0.8.9/reolink_aio/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,25 +41,26 @@
 from .utils import datetime_to_reolink_time, reolink_time_to_datetime
 
 MANUFACTURER = "Reolink"
 DEFAULT_STREAM = "sub"
 DEFAULT_PROTOCOL = "rtmp"
 DEFAULT_TIMEOUT = 30
 RETRY_ATTEMPTS = 3
-MAX_CHUNK_ITEMS = 40
+MAX_CHUNK_ITEMS = 35
 DEFAULT_RTMP_AUTH_METHOD = "PASSWORD"
 SUBSCRIPTION_TERMINATION_TIME = 15  # minutes
 LONG_POLL_TIMEOUT = 5  # minutes
 
 MOTION_DETECTION_TYPE = "motion"
 FACE_DETECTION_TYPE = "face"
 PERSON_DETECTION_TYPE = "person"
 VEHICLE_DETECTION_TYPE = "vehicle"
 PET_DETECTION_TYPE = "pet"
 VISITOR_DETECTION_TYPE = "visitor"
+PACKAGE_DETECTION_TYPE = "package"
 
 _LOGGER = logging.getLogger(__name__)
 _LOGGER_DATA = logging.getLogger(__name__ + ".data")
 _LOGGER_RTSP = logging.getLogger(__name__ + ".aiortsp")
 _LOGGER_RTSP.setLevel(logging.WARNING)
 
 SSL_CONTEXT = ssl.create_default_context()
@@ -173,14 +174,15 @@
         self._rtsp_mainStream: dict[int, str] = {}
         self._rtsp_subStream: dict[int, str] = {}
         self._rtsp_verified: dict[int, dict[str, str]] = {}
 
         ##############################################################################
         # Presets
         self._ptz_presets: dict[int, dict] = {}
+        self._ptz_patrols: dict[int, dict] = {}
 
         ##############################################################################
         # Saved info response-blocks
         self._hdd_info: list[dict] = []
         self._local_link: Optional[dict] = None
         self._wifi_signal: Optional[int] = None
         self._users: Optional[dict] = None
@@ -200,14 +202,15 @@
         self._image_settings: dict[int, dict] = {}
         self._ftp_settings: dict[int, dict] = {}
         self._osd_settings: dict[int, dict] = {}
         self._push_settings: dict[int, dict] = {}
         self._webhook_settings: dict[int, dict] = {}
         self._enc_settings: dict[int, dict] = {}
         self._ptz_presets_settings: dict[int, dict] = {}
+        self._ptz_patrol_settings: dict[int, dict] = {}
         self._ptz_guard_settings: dict[int, dict] = {}
         self._ptz_position: dict[int, dict] = {}
         self._email_settings: dict[int, dict] = {}
         self._ir_settings: dict[int, dict] = {}
         self._status_led_settings: dict[int, dict] = {}
         self._whiteled_settings: dict[int, dict] = {}
         self._recording_settings: dict[int, dict] = {}
@@ -1129,18 +1132,19 @@
                 self._capabilities[channel].append("floodLight")
 
             if self.api_version("GetAudioCfg") > 0:
                 self._capabilities[channel].append("volume")
                 if self.api_version("supportVisitorLoudspeaker", channel) > 0:
                     self._capabilities[channel].append("doorbell_button_sound")
 
-            if (self.api_version("supportAudioFileList", channel) > 0 and self.api_version("supportAutoReply", channel) > 0) or (
-                not self.is_nvr and self.api_version("supportAudioFileList") > 0 and self.api_version("supportAutoReply") > 0
-            ):
-                self._capabilities[channel].append("quick_reply")
+            if (self.api_version("supportAudioFileList", channel) > 0) or (not self.is_nvr and self.api_version("supportAudioFileList") > 0):
+                if self.api_version("supportAutoReply", channel) > 0 or (not self.is_nvr and self.api_version("supportAutoReply") > 0):
+                    self._capabilities[channel].append("quick_reply")
+                if self.api_version("supportAudioPlay", channel) > 0:
+                    self._capabilities[channel].append("play_quick_reply")
 
             if self.api_version("alarmAudio", channel) > 0 and channel in self._audio_alarm_settings:
                 self._capabilities[channel].append("siren")
                 self._capabilities[channel].append("siren_play")  # if self.api_version("supportAoAdjust", channel) > 0
 
             if self.audio_record(channel) is not None:
                 self._capabilities[channel].append("audio")
@@ -1171,14 +1175,16 @@
                         self._capabilities[channel].append("ptz_guard")
                     if self.api_version("GetPtzCurPos", channel) > 0:
                         self._capabilities[channel].append("ptz_position")
                 if ptz_ver in [2, 3]:
                     self._capabilities[channel].append("ptz_speed")
                 if channel in self._ptz_presets and len(self._ptz_presets[channel]) != 0:
                     self._capabilities[channel].append("ptz_presets")
+                if channel in self._ptz_patrols and len(self._ptz_patrols[channel]) != 0:
+                    self._capabilities[channel].append("ptz_patrol")
 
             if self.api_version("supportDigitalZoom", channel) > 0 and "zoom" not in self._capabilities[channel]:
                 min_zoom = self._zoom_focus_range.get(channel, {}).get("zoom", {}).get("pos", {}).get("min")
                 max_zoom = self._zoom_focus_range.get(channel, {}).get("zoom", {}).get("pos", {}).get("max")
                 if min_zoom is not None and max_zoom is not None:
                     self._capabilities[channel].append("zoom_basic")
                     self._capabilities[channel].append("zoom")
@@ -1281,14 +1287,16 @@
                 ch_body = [{"cmd": "GetPowerLed", "action": 0, "param": {"channel": channel}}]
             elif cmd == "GetWhiteLed":
                 ch_body = [{"cmd": "GetWhiteLed", "action": 0, "param": {"channel": channel}}]
             elif cmd == "GetWebHook":
                 ch_body = [{"cmd": "GetWebHook", "action": 0, "param": {"channel": channel}}]
             elif cmd == "GetPtzPreset":
                 ch_body = [{"cmd": "GetPtzPreset", "action": 0, "param": {"channel": channel}}]
+            elif cmd == "GetPtzPatrol":
+                ch_body = [{"cmd": "GetPtzPatrol", "action": 0, "param": {"channel": channel}}]
             elif cmd == "GetAutoFocus":
                 ch_body = [{"cmd": "GetAutoFocus", "action": 0, "param": {"channel": channel}}]
             elif cmd == "GetZoomFocus":
                 ch_body = [{"cmd": "GetZoomFocus", "action": 0, "param": {"channel": channel}}]
             elif cmd == "GetPtzGuard":
                 ch_body = [{"cmd": "GetPtzGuard", "action": 0, "param": {"channel": channel}}]
             elif cmd == "GetPtzCurPos":
@@ -1609,14 +1617,15 @@
             if self.supported(channel, "webhook"):
                 ch_body.append({"cmd": "GetWebHook", "action": 0, "param": {"channel": channel}})
             # checking range
             if self.supported(channel, "zoom_basic"):
                 ch_body.append({"cmd": "GetZoomFocus", "action": 1, "param": {"channel": channel}})
             if self.supported(channel, "pan_tilt") and self.api_version("ptzPreset", channel) >= 1:
                 ch_body.append({"cmd": "GetPtzPreset", "action": 0, "param": {"channel": channel}})
+                ch_body.append({"cmd": "GetPtzPatrol", "action": 0, "param": {"channel": channel}})
                 ch_body.append({"cmd": "GetPtzGuard", "action": 0, "param": {"channel": channel}})
                 ch_body.append({"cmd": "GetPtzCurPos", "action": 0, "param": {"PtzCurPos": {"channel": channel}}})
             if self.supported(channel, "auto_track"):
                 ch_body.append({"cmd": "GetAiCfg", "action": 1, "param": {"channel": channel}})
             # checking API versions
             if self.api_version("supportBuzzer") > 0:
                 ch_body.append({"cmd": "GetBuzzerAlarmV20", "action": 0, "param": {"channel": channel}})
@@ -2685,14 +2694,23 @@
                     self._ptz_presets[channel] = {}
                     for preset in data["value"]["PtzPreset"]:
                         if int(preset["enable"]) == 1:
                             preset_name = preset["name"]
                             preset_id = int(preset["id"])
                             self._ptz_presets[channel][preset_name] = preset_id
 
+                elif data["cmd"] == "GetPtzPatrol":
+                    self._ptz_patrol_settings[channel] = data["value"]
+                    self._ptz_patrols[channel] = {}
+                    for patrol in data["value"]["PtzPatrol"]:
+                        if int(patrol["enable"]) == 1:
+                            patrol_name = patrol["name"]
+                            patrol_id = int(patrol["id"])
+                            self._ptz_patrols[channel][patrol_name] = patrol_id
+
                 elif data["cmd"] == "GetPtzGuard":
                     self._ptz_guard_settings[channel] = data["value"]
 
                 elif data["cmd"] == "GetPtzCurPos":
                     self._ptz_position[channel] = data["value"]
 
                 elif data["cmd"] == "GetAiCfg":
@@ -2945,25 +2963,44 @@
 
     def ptz_presets(self, channel: int) -> dict:
         if channel not in self._ptz_presets:
             return {}
 
         return self._ptz_presets[channel]
 
-    async def set_ptz_command(self, channel: int, command: str | None = None, preset: int | str | None = None, speed: int | None = None) -> None:
+    def ptz_patrols(self, channel: int) -> dict:
+        if channel not in self._ptz_patrols:
+            return {}
+
+        return self._ptz_patrols[channel]
+
+    async def ctrl_ptz_patrol(self, channel: int, value: bool) -> None:
+        """Start/Stop PTZ patrol."""
+        if not self.supported(channel, "ptz_patrol"):
+            raise NotSupportedError(f"ctrl_ptz_patrol: ptz patrol on camera {self.camera_name(channel)} is not available")
+
+        patrol = list(self.ptz_patrols(channel).values())[0]
+        if value:
+            cmd = "StartPatrol"
+        else:
+            cmd = "StopPatrol"
+
+        await self.set_ptz_command(channel, command=cmd, patrol=patrol)
+
+    async def set_ptz_command(self, channel: int, command: str | None = None, preset: int | str | None = None, speed: int | None = None, patrol: int | None = None) -> None:
         """Send PTZ command to the camera, list of possible commands see PtzEnum."""
 
         if channel not in self._channels:
             raise InvalidParameterError(f"set_ptz_command: no camera connected to channel '{channel}'")
         if speed is not None and not isinstance(speed, int):
             raise InvalidParameterError(f"set_ptz_command: speed {speed} is not integer")
         if speed is not None and not self.supported(channel, "ptz_speed"):
             raise NotSupportedError(f"set_ptz_command: ptz speed on camera {self.camera_name(channel)} is not available")
         command_list = [com.value for com in PtzEnum]
-        if command is not None and command not in command_list:
+        if command is not None and command not in command_list and patrol is None:
             raise InvalidParameterError(f"set_ptz_command: command {command} not in {command_list}")
 
         if preset is not None:
             command = "ToPos"
             if isinstance(preset, str):
                 if preset not in self.ptz_presets(channel):
                     raise InvalidParameterError(f"set_ptz_command: preset '{preset}' not in available presets {list(self.ptz_presets(channel).keys())}")
@@ -2982,14 +3019,16 @@
             }
         ]
 
         if speed:
             body[0]["param"]["speed"] = speed
         if preset:
             body[0]["param"]["id"] = preset
+        if patrol:
+            body[0]["param"]["id"] = patrol
 
         await self.send_setting(body)
 
     def ptz_pan_position(self, channel: int) -> int:
         """pan position"""
         if channel not in self._ptz_position:
             return 0
@@ -3506,14 +3545,27 @@
             params["volume"] = volume
         if doorbell_button_sound is not None:
             params["visitorLoudspeaker"] = 1 if doorbell_button_sound else 0
 
         body = [{"cmd": "SetAudioCfg", "action": 0, "param": {"AudioCfg": params}}]
         await self.send_setting(body)
 
+    async def play_quick_reply(self, channel: int, file_id: int) -> None:
+        if channel not in self._channels:
+            raise InvalidParameterError(f"play_quick_reply: no camera connected to channel '{channel}'")
+        if not self.supported(channel, "play_quick_reply"):
+            raise NotSupportedError(f"play_quick_reply: Play quick reply on camera {self.camera_name(channel)} is not available")
+        if file_id is not None and not isinstance(file_id, int):
+            raise InvalidParameterError(f"play_quick_reply: file_id {file_id} not integer")
+        if file_id is not None and file_id not in self.quick_reply_dict(channel):
+            raise InvalidParameterError(f"play_quick_reply: file_id {file_id} not in {list(self.quick_reply_dict(channel))}")
+
+        body = [{"cmd": "QuickReplyPlay", "action": 0, "param": {"id": file_id}}]
+        await self.send_setting(body)
+
     async def set_quick_reply(self, channel: int, enable: bool | None = None, file_id: int | None = None, time: int | None = None) -> None:
         if channel not in self._channels:
             raise InvalidParameterError(f"set_quick_reply: no camera connected to channel '{channel}'")
         if not self.supported(channel, "quick_reply"):
             raise NotSupportedError(f"set_quick_reply: Quick reply on camera {self.camera_name(channel)} is not available")
         if file_id is not None and not isinstance(file_id, int):
             raise InvalidParameterError(f"set_quick_reply: file_id {file_id} not integer")
@@ -4846,23 +4898,23 @@
             data_element = message.find(f".//\u007bhttp://www.onvif.org/ver10/schema\u007dSimpleItem[@Name='{key}']")
             if data_element is None or "Value" not in data_element.attrib:
                 if f"ONVIF_{rule}_no_data" not in self._log_once:
                     self._log_once.append(f"ONVIF_{rule}_no_data")
                     _LOGGER.warning("ONVIF event '%s' did not contain data:\n%s", rule, data)
                 continue
 
-            if rule not in ["Motion", "MotionAlarm", "FaceDetect", "PeopleDetect", "VehicleDetect", "DogCatDetect", "Visitor"]:
+            if rule not in ["Motion", "MotionAlarm", "FaceDetect", "PeopleDetect", "VehicleDetect", "DogCatDetect", "Package", "Visitor"]:
                 if f"ONVIF_unknown_{rule}" not in self._log_once:
                     self._log_once.append(f"ONVIF_unknown_{rule}")
                     _LOGGER.warning("ONVIF event with unknown rule: '%s'", rule)
                 continue
 
             if channel not in event_channels:
                 event_channels.append(channel)
-            if rule in ["FaceDetect", "PeopleDetect", "VehicleDetect", "DogCatDetect", "Visitor"]:
+            if rule in ["FaceDetect", "PeopleDetect", "VehicleDetect", "DogCatDetect", "Package", "Visitor"]:
                 self._onvif_only_motion[sub_type] = False
 
             state = data_element.attrib["Value"] == "true"
             _LOGGER.info("Reolink %s ONVIF event channel %s, %s: %s", self.nvr_name, channel, rule, state)
 
             if rule == "Motion":
                 self._motion_detection_states[channel] = state
@@ -4872,14 +4924,16 @@
                 self._ai_detection_states[channel]["face"] = state
             elif rule == "PeopleDetect":
                 self._ai_detection_states[channel]["people"] = state
             elif rule == "VehicleDetect":
                 self._ai_detection_states[channel]["vehicle"] = state
             elif rule == "DogCatDetect":
                 self._ai_detection_states[channel]["dog_cat"] = state
+            elif rule == "Package":
+                self._ai_detection_states[channel]["package"] = state
             elif rule == "Visitor":
                 self._visitor_states[channel] = state
 
         if not event_channels and not contains_channels:
             # ONVIF notification withouth known events
             if "ONVIF_no_known" not in self._log_once:
                 self._log_once.append("ONVIF_no_known")
```

### Comparing `reolink_aio-0.8.8/reolink_aio/enums.py` & `reolink_aio-0.8.9/reolink_aio/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 class StatusLedEnum(Enum):
     """Options for the status led mode"""
 
     stayoff = "KeepOff"
     auto = "Off"
     alwaysonatnight = "On"
+    alwayson = "Always"
 
 
 class DayNightEnum(Enum):
     """Options for the DayNight setting"""
 
     auto = "Auto"
     color = "Color"
```

### Comparing `reolink_aio-0.8.8/reolink_aio/exceptions.py` & `reolink_aio-0.8.9/reolink_aio/exceptions.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.8/reolink_aio/software_version.py` & `reolink_aio-0.8.9/reolink_aio/software_version.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.8/reolink_aio/templates.py` & `reolink_aio-0.8.9/reolink_aio/templates.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.8/reolink_aio/typings.py` & `reolink_aio-0.8.9/reolink_aio/typings.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.8/reolink_aio/utils.py` & `reolink_aio-0.8.9/reolink_aio/utils.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.8/reolink_aio.egg-info/PKG-INFO` & `reolink_aio-0.8.9/reolink_aio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink_aio
-Version: 0.8.8
+Version: 0.8.9
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink_aio Version: 0.8.8 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink_aio Version: 0.8.9 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.8.8/setup.py` & `reolink_aio-0.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='reolink_aio',
-      version='0.8.8',
+      version='0.8.9',
       description='Reolink NVR/cameras API package',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/starkillerOG/reolink_aio',
       author='starkillerOG',
       author_email='starkiller.og@gmail.com',
       license='MIT',
```

### Comparing `reolink_aio-0.8.8/tests/test.py` & `reolink_aio-0.8.9/tests/test.py`

 * *Files identical despite different names*

