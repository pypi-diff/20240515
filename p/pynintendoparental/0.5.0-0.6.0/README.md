# Comparing `tmp/pynintendoparental-0.5.0.tar.gz` & `tmp/pynintendoparental-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynintendoparental-0.5.0.tar", last modified: Thu Mar 21 10:57:51 2024, max compression
+gzip compressed data, was "pynintendoparental-0.6.0.tar", last modified: Wed May 15 20:30:55 2024, max compression
```

## Comparing `pynintendoparental-0.5.0.tar` & `pynintendoparental-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:57:51.560215 pynintendoparental-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-21 10:57:51.560215 pynintendoparental-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:57:51.556215 pynintendoparental-0.5.0/pynintendoparental/
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/pynintendoparental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/pynintendoparental/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/pynintendoparental/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:57:51.560215 pynintendoparental-0.5.0/pynintendoparental/authenticator/
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/pynintendoparental/authenticator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/pynintendoparental/authenticator/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/pynintendoparental/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    20569 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/pynintendoparental/device.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/pynintendoparental/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/pynintendoparental/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/pynintendoparental/player.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/pynintendoparental/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:57:51.560215 pynintendoparental-0.5.0/pynintendoparental.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-21 10:57:51.000000 pynintendoparental-0.5.0/pynintendoparental.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 10:57:51.000000 pynintendoparental-0.5.0/pynintendoparental.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:57:51.000000 pynintendoparental-0.5.0/pynintendoparental.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-21 10:57:51.000000 pynintendoparental-0.5.0/pynintendoparental.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-21 10:57:51.000000 pynintendoparental-0.5.0/pynintendoparental.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:57:51.560215 pynintendoparental-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-21 10:57:29.000000 pynintendoparental-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:30:55.277441 pynintendoparental-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-15 20:30:55.277441 pynintendoparental-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:30:55.277441 pynintendoparental-0.6.0/pynintendoparental/
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/pynintendoparental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/pynintendoparental/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/pynintendoparental/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:30:55.277441 pynintendoparental-0.6.0/pynintendoparental/authenticator/
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/pynintendoparental/authenticator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/pynintendoparental/authenticator/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/pynintendoparental/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19600 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/pynintendoparental/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/pynintendoparental/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/pynintendoparental/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/pynintendoparental/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/pynintendoparental/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:30:55.277441 pynintendoparental-0.6.0/pynintendoparental.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-15 20:30:55.000000 pynintendoparental-0.6.0/pynintendoparental.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-15 20:30:55.000000 pynintendoparental-0.6.0/pynintendoparental.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:30:55.000000 pynintendoparental-0.6.0/pynintendoparental.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-15 20:30:55.000000 pynintendoparental-0.6.0/pynintendoparental.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 20:30:55.000000 pynintendoparental-0.6.0/pynintendoparental.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:30:55.277441 pynintendoparental-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-15 20:30:30.000000 pynintendoparental-0.6.0/setup.py
```

### Comparing `pynintendoparental-0.5.0/LICENSE` & `pynintendoparental-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynintendoparental-0.5.0/PKG-INFO` & `pynintendoparental-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynintendoparental
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python module to interact with Nintendo Parental Controls
 Home-page: http://github.com/pantherale0/pynintendoparental
 Author: pantherale0
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pynintendoparental-0.5.0/README.md` & `pynintendoparental-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pynintendoparental-0.5.0/pynintendoparental/__init__.py` & `pynintendoparental-0.6.0/pynintendoparental/__init__.py`

 * *Files identical despite different names*

### Comparing `pynintendoparental-0.5.0/pynintendoparental/api.py` & `pynintendoparental-0.6.0/pynintendoparental/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,21 +71,23 @@
             session.headers.add("X-Moon-Os-Version", OS_VERSION)
             session.headers.add("X-Moon-Model", DEVICE_MODEL)
             session.headers.add("X-Moon-TimeZone", self._tz)
             session.headers.add("X-Moon-Os-Language", self._language)
             session.headers.add("X-Moon-App-Language", self._language)
             session.headers.add("X-Moon-App-Display-Version", MOBILE_APP_VERSION)
             session.headers.add("X-Moon-App-Internal-Version", MOBILE_APP_BUILD)
-            #session.headers.add("X-Moon-Smart-Device-Id", "190207e4-2f6f-4db7-bc96-fdfe109124f0")
             async with session.request(
                 method=e_point.get("method"),
                 url=url,
                 json=body
             ) as response:
-                _LOGGER.debug("Request to %s status code %s", url, response.status)
+                _LOGGER.debug("%s request to %s status code %s",
+                              e_point.get("method"),
+                              url,
+                              response.status)
                 if _check_http_success(response.status):
                     resp["status"] = response.status
                     resp["text"] = await response.text()
                     resp["json"] = await response.json()
                     resp["headers"] = response.headers
                 else:
                     raise HttpException("HTTP Error", response.status)
```

### Comparing `pynintendoparental-0.5.0/pynintendoparental/application.py` & `pynintendoparental-0.6.0/pynintendoparental/application.py`

 * *Files identical despite different names*

### Comparing `pynintendoparental-0.5.0/pynintendoparental/authenticator/__init__.py` & `pynintendoparental-0.6.0/pynintendoparental/authenticator/__init__.py`

 * *Files identical despite different names*

### Comparing `pynintendoparental-0.5.0/pynintendoparental/authenticator/const.py` & `pynintendoparental-0.6.0/pynintendoparental/authenticator/const.py`

 * *Files identical despite different names*

### Comparing `pynintendoparental-0.5.0/pynintendoparental/const.py` & `pynintendoparental-0.6.0/pynintendoparental/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pylint: disable=line-too-long
 """pynintendoparental"""
-__version__ = '0.5.0'
+__version__ = '0.6.0'
 
 import logging
 
 _LOGGER = logging.getLogger(__package__)
 MOBILE_APP_PKG = "com.nintendo.znma"
 MOBILE_APP_VERSION = "1.20.0"
 MOBILE_APP_BUILD = "282"
```

### Comparing `pynintendoparental-0.5.0/pynintendoparental/device.py` & `pynintendoparental-0.6.0/pynintendoparental/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,15 @@
         self.sync_state: str = None
         self.extra: dict = {}
         self._api: Api = api
         self.daily_summaries: dict = {}
         self.parental_control_settings: dict = {}
         self.players: list[Player] = []
         self.limit_time: int = 0
-        self._limit_time_overflow: int = 0 # max 6 hrs on limit time
         self.timer_mode: str = ""
-        self.previous_limit_time: int = 0
         self.today_playing_time: int = 0
         self.bedtime_alarm: time
         self.month_playing_time: int = 0
         self.today_disabled_time: int = 0
         self.today_exceeded_time: int = 0
         self.today_notices: list = []
         self.today_important_info: list = []
@@ -47,27 +45,24 @@
         self.application_update_failed: bool = False
         _LOGGER.debug("Device init complete for %s", self.device_id)
 
     async def update(self):
         """Update data."""
         _LOGGER.debug(">> Device.update()")
         await asyncio.gather(
-                self._update_daily_summaries(),
-                self._update_parental_control_setting(),
+                self._get_daily_summaries(),
+                self._get_parental_control_setting(),
                 self.get_monthly_summary(),
-                self._update_extras()
+                self._get_extras()
         )
         if self.players is None:
             self.players = Player.from_device_daily_summary(self.daily_summaries)
         else:
             for player in self.players:
                 player.update_from_daily_summary(self.daily_summaries)
-        if self.limit_time == self._limit_time_overflow:
-            if self._limit_time_overflow < self.today_playing_time:
-                await self.update_max_daily_playtime(0, False)
 
     async def set_new_pin(self, pin: str):
         """Updates the pin for the device."""
         _LOGGER.debug(">> Device.set_new_pin(pin=REDACTED)")
         self.parental_control_settings["unlockCode"] = pin
         await self._set_parental_control_setting()
 
@@ -105,55 +100,49 @@
         """Shortcut method to deduplicate code used to update parental control settings."""
         _LOGGER.debug(">> Device._set_parental_control_setting()")
         await self._api.send_request(
             endpoint="update_device_parental_control_setting",
             body=self._get_update_parental_control_setting_body(),
             DEVICE_ID=self.device_id
         )
-        await self._update_parental_control_setting()
+        await self._get_parental_control_setting()
 
-    async def update_max_daily_playtime(self, minutes: int | None = 0, restore: bool = False):
+    async def update_max_daily_playtime(self, minutes: int | None = 0):
         """Updates the maximum daily playtime of a device."""
-        _LOGGER.debug(">> Device.update_max_daily_playtime(minutes=%s, restore=%s)",
-                      minutes,
-                      restore)
+        _LOGGER.debug(">> Device.update_max_daily_playtime(minutes=%s)",
+                      minutes)
         time_to_play_in_one_day_enabled = True
-        if restore and self.previous_limit_time == 0:
-            raise RuntimeError("Invalid state for restore operation.")
-        if (minutes is not None and minutes > 360):
-            self._limit_time_overflow = minutes
+        if minutes > 360:
+            raise ValueError("Only values up to 360 minutes (6 hours) are accepted.")
+        if minutes is not None:
             time_to_play_in_one_day_enabled = False
-        if restore:
-            minutes = self.previous_limit_time
-        elif not restore and minutes == 0:
-            self.previous_limit_time = self.limit_time
         if self.timer_mode == "DAILY":
             _LOGGER.debug(
                 "Setting timeToPlayInOneDay.limitTime for device %s to value %s",
                 self.device_id,
                 minutes)
             self.parental_control_settings["playTimerRegulations"]["dailyRegulations"]["timeToPlayInOneDay"]["enabled"] = time_to_play_in_one_day_enabled
             if time_to_play_in_one_day_enabled and minutes is not None:
                 self.parental_control_settings["playTimerRegulations"]["dailyRegulations"]["timeToPlayInOneDay"]["limitTime"] = minutes
             else:
-                self.parental_control_settings["playTimerRegulations"]["dailyRegulations"]["timeToPlayInOneDay"]["limitTime"] = None
+                self.parental_control_settings["playTimerRegulations"]["dailyRegulations"]["timeToPlayInOneDay"]["limitTime"] = -1
             await self._set_parental_control_setting()
         else:
             _LOGGER.debug(
                 "Setting timeToPlayInOneDay.limitTime for device %s to value %s",
                 self.device_id,
                 minutes
             )
             day_of_week_regs = self.parental_control_settings["playTimerRegulations"]["eachDayOfTheWeekRegulations"]
             current_day = DAYS_OF_WEEK[datetime.now().weekday()]
             day_of_week_regs[current_day]["timeToPlayInOneDay"]["enabled"] = time_to_play_in_one_day_enabled
             if time_to_play_in_one_day_enabled and minutes is not None:
                 day_of_week_regs[current_day]["timeToPlayInOneDay"]["limitTime"] = minutes
             else:
-                day_of_week_regs[current_day]["timeToPlayInOneDay"]["limitTime"] = None
+                day_of_week_regs[current_day]["timeToPlayInOneDay"]["limitTime"] = -1
             await self._set_parental_control_setting()
 
     def _get_update_parental_control_setting_body(self):
         """Returns the dict that is required to update the parental control settings."""
         return {
             "unlockCode": self.parental_control_settings["unlockCode"],
             "functionalRestrictionLevel": self.parental_control_settings["functionalRestrictionLevel"],
@@ -174,23 +163,17 @@
 
     def _update_day_of_week_regulations(self):
         """Override the limit / bed time for the device from parental_control_settings if individual days are configured."""
         day_of_week_regs = self.parental_control_settings["playTimerRegulations"].get("eachDayOfTheWeekRegulations", {})
         current_day = day_of_week_regs.get(DAYS_OF_WEEK[datetime.now().weekday()], {})
         self.timer_mode = self.parental_control_settings["playTimerRegulations"]["timerMode"]
         if self.timer_mode == "EACH_DAY_OF_THE_WEEK":
-            if self._limit_time_overflow > 0:
-                self.limit_time = self._limit_time_overflow
-            else:
-                self.limit_time = current_day["timeToPlayInOneDay"]["limitTime"]
+            self.limit_time = current_day["timeToPlayInOneDay"]["limitTime"]
         else:
-            if self._limit_time_overflow > 0:
-                self.limit_time = self._limit_time_overflow
-            else:
-                self.limit_time = self.parental_control_settings["playTimerRegulations"]["dailyRegulations"]["timeToPlayInOneDay"]["limitTime"]
+            self.limit_time = self.parental_control_settings["playTimerRegulations"]["dailyRegulations"]["timeToPlayInOneDay"]["limitTime"]
 
         if self.timer_mode == "EACH_DAY_OF_THE_WEEK":
             if current_day["bedtime"]["enabled"]:
                 self.bedtime_alarm = time(hour=
                                         current_day["bedtime"]["endingTime"]["hour"],
                                         minute=current_day["bedtime"]["endingTime"]["minute"])
             else:
@@ -199,65 +182,61 @@
             bedtime_alarm = self.parental_control_settings["playTimerRegulations"]["dailyRegulations"]["bedtime"]
             if bedtime_alarm["enabled"]:
                 self.bedtime_alarm = time(hour=
                                         bedtime_alarm["endingTime"]["hour"],
                                         minute=bedtime_alarm["endingTime"]["minute"])
             else:
                 self.bedtime_alarm = None
-
-
-        if self.previous_limit_time is None:
-            self.previous_limit_time = self.limit_time
         return True
 
-    async def _update_parental_control_setting(self):
+    async def _get_parental_control_setting(self):
         """Retreives parental control settings from the API."""
-        _LOGGER.debug(">> Device._update_parental_control_setting()")
+        _LOGGER.debug(">> Device._get_parental_control_setting()")
         response = await self._api.send_request(
             endpoint="get_device_parental_control_setting",
             DEVICE_ID=self.device_id
         )
         self.parental_control_settings = response["json"]
         self.forced_termination_mode = (
             self.parental_control_settings["playTimerRegulations"]["restrictionMode"] == str(RestrictionMode.FORCED_TERMINATION)
         )
         self._update_day_of_week_regulations()
-        self._update_whitelisted_applications()
+        self._get_whitelisted_applications()
         self._update_applications()
 
-    def _update_whitelisted_applications(self):
+    def _get_whitelisted_applications(self):
         """Update whitelisted applications from local parental control settings."""
         for app_id in self.parental_control_settings["whitelistedApplications"]:
             self.whitelisted_applications[app_id] = (
                 self.parental_control_settings["whitelistedApplications"][app_id]["safeLaunch"] == "ALLOW"
             )
 
-    async def _update_daily_summaries(self):
-        """Update daily summaries."""
-        _LOGGER.debug(">> Device._update_daily_summaries()")
+    async def _get_daily_summaries(self):
+        """Retrieve daily summaries."""
+        _LOGGER.debug(">> Device._get_daily_summaries()")
         response = await self._api.send_request(
             endpoint="get_device_daily_summaries",
             DEVICE_ID = self.device_id
         )
         self.daily_summaries = response["json"]["items"]
         _LOGGER.debug("New daily summary %s", self.daily_summaries)
         try:
             today_playing_time = self.get_date_summary()[0].get("playingTime", 0)
             self.today_playing_time = None if today_playing_time is None else today_playing_time/60
             today_disabled_time = self.get_date_summary()[0].get("disabledTime", 0)
             self.today_disabled_time = None if today_disabled_time is None else today_disabled_time/60
             today_exceeded_time = self.get_date_summary()[0].get("exceededTime", 0)
             self.today_exceeded_time = None if today_exceeded_time is None else today_exceeded_time/60
-            _LOGGER.debug("Set playing, disabled and exceeded time for today for device %s",
+            _LOGGER.debug("Cached playing, disabled and exceeded time for today for device %s",
                         self.device_id)
 
             self.today_important_info = self.get_date_summary()[0].get("importantInfos", [])
             self.today_notices = self.get_date_summary()[0].get("notices", [])
             self.today_observations = self.get_date_summary()[0].get("observations", [])
-            _LOGGER.debug("Set today important info, notices and observations for device %s",
+            _LOGGER.debug("Cached today important info, notices and observations for device %s",
                         self.device_id)
             self.stats_update_failed = False
         except ValueError as err:
             _LOGGER.warning("Unable to update daily summary for device %s: %s", self.name, err)
             self.stats_update_failed = True
 
         current_month = datetime(
@@ -267,53 +246,53 @@
         month_playing_time: int = 0
 
         for summary in self.daily_summaries:
             date_parsed = datetime.strptime(summary["date"], "%Y-%m-%d")
             if date_parsed > current_month:
                 month_playing_time += summary["playingTime"]
         self.month_playing_time = month_playing_time
-        _LOGGER.debug("Set current month playing time for device %s", self.device_id)
+        _LOGGER.debug("Cached current month playing time for device %s", self.device_id)
         parsed_apps = Application.from_daily_summary(self.daily_summaries)
         for app in parsed_apps:
             try:
                 int_app = self.get_application(app.application_id)
-                _LOGGER.debug("Updating app %s for device %s",
+                _LOGGER.debug("Updating cached app state %s for device %s",
                               int_app.application_id,
                               self.device_id)
                 int_app.update(app)
             except ValueError:
-                _LOGGER.debug("Creating new application entry %s for device %s",
+                _LOGGER.debug("Creating new cached application entry %s for device %s",
                               app.application_id,
                               self.device_id)
                 self.applications.append(app)
 
         # update application playtime
         try:
             for player in self.get_date_summary()[0].get("devicePlayers", []):
                 for app in player.get("playedApps", []):
                     self.get_application(app["applicationId"]).update_today_time_played(app)
             self.application_update_failed = False
         except ValueError as err:
-            _LOGGER.warning("Unable to update applications for device %s: %s", self.name, err)
+            _LOGGER.warning("Unable to retrieve applications for device %s: %s", self.name, err)
             self.application_update_failed = True
 
-    async def _update_extras(self):
-        """Update extra props."""
-        _LOGGER.debug(">> Device._update_extras()")
+    async def _get_extras(self):
+        """Retrieve extra properties."""
+        _LOGGER.debug(">> Device._get_extras()")
         if self.alarms_enabled is not None:
             # first refresh can come from self.extra without http request
             response = await self._api.send_request(
                 endpoint="get_account_device",
                 ACCOUNT_ID = self._api.account_id,
                 DEVICE_ID = self.device_id
             )
             self.extra = response["json"]
         status = self.extra["device"]["alarmSetting"]["visibility"]
         self.alarms_enabled = status == str(AlarmSettingState.VISIBLE)
-        _LOGGER.debug("Set alarms enabled to state %s for device %s",
+        _LOGGER.debug("Cached alarms enabled to state %s for device %s",
                       self.alarms_enabled,
                       self.device_id)
 
     async def get_monthly_summary(self, search_date: datetime = None):
         """Gets the monthly summary."""
         _LOGGER.debug(">> Device.get_monthly_summary(search_date=%s)", search_date)
         latest = False
@@ -371,15 +350,15 @@
         current_state = self.parental_control_settings["whitelistedApplications"]
         current_state[app_id]["safeLaunch"] = "ALLOW" if allowed else "NONE"
         await self._api.send_request(
             endpoint="update_device_whitelisted_applications",
             body=current_state,
             DEVICE_ID=self.device_id
         )
-        await self._update_parental_control_setting()
+        await self._get_parental_control_setting()
 
     def get_date_summary(self, input_date: datetime = datetime.now()) -> dict:
         """Returns usage for a given date."""
         summary = [
             x for x in self.daily_summaries
             if x["date"] == input_date.strftime('%Y-%m-%d')
         ]
```

### Comparing `pynintendoparental-0.5.0/pynintendoparental/player.py` & `pynintendoparental-0.6.0/pynintendoparental/player.py`

 * *Files identical despite different names*

### Comparing `pynintendoparental-0.5.0/pynintendoparental.egg-info/PKG-INFO` & `pynintendoparental-0.6.0/pynintendoparental.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynintendoparental
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python module to interact with Nintendo Parental Controls
 Home-page: http://github.com/pantherale0/pynintendoparental
 Author: pantherale0
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pynintendoparental-0.5.0/pynintendoparental.egg-info/SOURCES.txt` & `pynintendoparental-0.6.0/pynintendoparental.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynintendoparental-0.5.0/setup.py` & `pynintendoparental-0.6.0/setup.py`

 * *Files identical despite different names*

