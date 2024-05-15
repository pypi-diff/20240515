# Comparing `tmp/roxbot-1.9.0.tar.gz` & `tmp/roxbot-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roxbot-1.9.0.tar", last modified: Sat Jan 13 20:15:07 2024, max compression
+gzip compressed data, was "roxbot-2.0.0.tar", last modified: Wed May 15 15:55:55 2024, max compression
```

## Comparing `roxbot-1.9.0.tar` & `roxbot-2.0.0.tar`

### file list

```diff
@@ -1,67 +1,40 @@
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-01-13 20:15:07.317306 roxbot-1.9.0/
--rw-rw-rw-   0 dev       (1000) dev       (1000)     1081 2024-01-13 20:14:54.000000 roxbot-1.9.0/LICENCE
--rw-r--r--   0 dev       (1000) dev       (1000)      601 2024-01-13 20:15:07.317306 roxbot-1.9.0/PKG-INFO
--rw-rw-rw-   0 dev       (1000) dev       (1000)     3902 2024-01-13 20:14:54.000000 roxbot-1.9.0/README.md
--rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-01-13 20:15:07.317306 roxbot-1.9.0/setup.cfg
--rw-rw-rw-   0 dev       (1000) dev       (1000)     1296 2024-01-13 20:14:54.000000 roxbot-1.9.0/setup.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-01-13 20:15:07.295306 roxbot-1.9.0/src/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-01-13 20:15:07.302306 roxbot-1.9.0/src/roxbot/
--rw-rw-rw-   0 dev       (1000) dev       (1000)      104 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/__init__.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-01-13 20:15:07.306306 roxbot-1.9.0/src/roxbot/bridges/
--rw-rw-rw-   0 dev       (1000) dev       (1000)       68 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/bridges/__init__.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     3597 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/bridges/base.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)      630 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/bridges/mock_bridge.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     5090 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/bridges/ros_bridge.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     3418 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/bridges/ws_bridge.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)      937 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/cli.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     1040 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/config.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     1499 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/converters.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     7041 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/gps.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-01-13 20:15:07.307306 roxbot-1.9.0/src/roxbot/hal/
--rw-rw-rw-   0 dev       (1000) dev       (1000)        0 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/hal/__init__.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     2271 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/hal/base.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     2332 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/hal/canopen.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     1410 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/hal/io.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     1033 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/interfaces.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-01-13 20:15:07.310306 roxbot-1.9.0/src/roxbot/models/
--rw-rw-rw-   0 dev       (1000) dev       (1000)      133 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/models/__init__.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     3626 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/models/diff_drive.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     1719 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/models/linear_model.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     1245 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/models/protocols.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     5849 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/models/trike.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     2237 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/models/wheels.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-01-13 20:15:07.311306 roxbot-1.9.0/src/roxbot/nodes/
--rw-rw-rw-   0 dev       (1000) dev       (1000)        0 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/nodes/__init__.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)      508 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/nodes/base.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     4374 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/nodes/gps_node.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     1450 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/odometry.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)        0 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/py.typed
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-01-13 20:15:07.311306 roxbot-1.9.0/src/roxbot/simulators/
--rw-rw-rw-   0 dev       (1000) dev       (1000)        0 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/simulators/__init__.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)      454 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/topics.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)      209 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/utils.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     6175 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/vectors.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     3347 2024-01-13 20:14:54.000000 roxbot-1.9.0/src/roxbot/version.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-01-13 20:15:07.316306 roxbot-1.9.0/src/roxbot.egg-info/
--rw-r--r--   0 dev       (1000) dev       (1000)      601 2024-01-13 20:15:07.000000 roxbot-1.9.0/src/roxbot.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)     1372 2024-01-13 20:15:07.000000 roxbot-1.9.0/src/roxbot.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-01-13 20:15:07.000000 roxbot-1.9.0/src/roxbot.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       42 2024-01-13 20:15:07.000000 roxbot-1.9.0/src/roxbot.egg-info/entry_points.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-01-13 20:14:56.000000 roxbot-1.9.0/src/roxbot.egg-info/not-zip-safe
--rw-r--r--   0 dev       (1000) dev       (1000)       84 2024-01-13 20:15:07.000000 roxbot-1.9.0/src/roxbot.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        7 2024-01-13 20:15:07.000000 roxbot-1.9.0/src/roxbot.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-01-13 20:15:07.316306 roxbot-1.9.0/tests/
--rw-rw-rw-   0 dev       (1000) dev       (1000)     1594 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_bridge.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)      462 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_cli.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     2891 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_config.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     2047 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_diffdrive.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     2963 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_gps.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)      438 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_hal.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     1308 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_interfaces.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     3120 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_models.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)      255 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_nodes.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)      840 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_odometry.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)      452 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_topics.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     2094 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_trike.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     4819 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_vectors.py
--rw-rw-rw-   0 dev       (1000) dev       (1000)     1673 2024-01-13 20:14:54.000000 roxbot-1.9.0/tests/test_ws_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.419286 roxbot-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 15:55:46.000000 roxbot-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-15 15:55:55.419286 roxbot-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-15 15:55:46.000000 roxbot-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 15:55:46.000000 roxbot-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:55:55.419286 roxbot-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.415286 roxbot-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.415286 roxbot-2.0.0/src/roxbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.419286 roxbot-2.0.0/src/roxbot/bridges/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/bridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/bridges/mqtt_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.419286 roxbot-2.0.0/src/roxbot/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/models/diff_drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/models/linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/models/wheels.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.419286 roxbot-2.0.0/src/roxbot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/utils/mock_robot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/utils/runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.419286 roxbot-2.0.0/src/roxbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-15 15:55:55.000000 roxbot-2.0.0/src/roxbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-15 15:55:55.000000 roxbot-2.0.0/src/roxbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:55:55.000000 roxbot-2.0.0/src/roxbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 15:55:55.000000 roxbot-2.0.0/src/roxbot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 15:55:55.000000 roxbot-2.0.0/src/roxbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 15:55:55.000000 roxbot-2.0.0/src/roxbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.419286 roxbot-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-15 15:55:46.000000 roxbot-2.0.0/tests/test_diffdrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-15 15:55:46.000000 roxbot-2.0.0/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-15 15:55:46.000000 roxbot-2.0.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-15 15:55:46.000000 roxbot-2.0.0/tests/test_mqtt_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 15:55:46.000000 roxbot-2.0.0/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-15 15:55:46.000000 roxbot-2.0.0/tests/test_vectors.py
```

### Comparing `roxbot-1.9.0/src/roxbot/models/diff_drive.py` & `roxbot-2.0.0/src/roxbot/models/diff_drive.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python3
 """
- Differential drive robot model
+Differential drive robot model
 
- Copyright (c) 2024 ROX Automation - Jev Kuznetsov
+Copyright (c) 2024 ROX Automation - Jev Kuznetsov
 """
 
 from typing import Tuple
 
 from roxbot.vectors import Vector
-
+from roxbot.interfaces import Pose
 from .wheels import Wheel
-from .protocols import RobotModelProtocol
 
 
 def vc_to_vels(v: float, c: float, W: float) -> Tuple[float, float]:
     """convert vel/curvature and wheelbase to Vl, Vr
 
     Args:
         v (float): linear velocity
@@ -31,15 +30,15 @@
     R = 1 / c
     vr = (v * W + 2 * R * v) / 2 / R
     vl = 2 * v - vr
 
     return vl, vr
 
 
-class DiffDriveModel(RobotModelProtocol):
+class DiffDriveModel:
     """basic differential drive robot model."""
 
     DEFAULT_WHEEL_BASE = 0.16
     DEFAULT_WHEEL_DIAMETER = 0.066
     DEFAULT_WHEEL_ACCEL = 1e6
 
     def __init__(
@@ -48,26 +47,24 @@
         wheel_diameter: float = DEFAULT_WHEEL_DIAMETER,
         wheel_accel: float = DEFAULT_WHEEL_ACCEL,
     ):
         self.left_wheel = Wheel(wheel_diameter, wheel_accel)
         self.right_wheel = Wheel(wheel_diameter, wheel_accel)
         self.W = wheel_base  # wheel base width
 
-        self.xy = Vector()  # position
-        self.theta = 0.0  # orientation
+        self.pose = Pose()  # current pose
 
         self.t = 0.0  # time counter
 
-    @property
-    def pose(self) -> Tuple[float, float, float]:
-        return (self.xy.x, self.xy.y, self.theta)
+    def get_pose(self) -> Pose:
+        return self.pose
 
-    @pose.setter
-    def pose(self, value: Tuple[float, float, float]) -> None:
-        self.xy.x, self.xy.y, self.theta = value
+    @property
+    def setpoints(self) -> Tuple[float, float]:
+        return (self.left_wheel.setpoint, self.right_wheel.setpoint)
 
     @property
     def vl(self) -> float:
         return self.left_wheel.velocity_ms
 
     @property
     def vr(self) -> float:
@@ -86,49 +83,46 @@
     def curvature(self) -> float:
         """driving curvature"""
         try:
             return 1 / (0.5 * self.W * (self.vl + self.vr) / (self.vr - self.vl))
         except ZeroDivisionError:
             return 0.0
 
-    def step(self, dt: float):
+    def step(self, dt: float) -> None:
         """perform timestep"""
 
         self.left_wheel.step(dt)
         self.right_wheel.step(dt)
 
         # using a simple approximation, should be good enough for short dt
         # don't bother with icc...
-        dxy = Vector.from_polar(self.velocity * dt, self.theta)
-        self.xy += dxy
+        dxy = Vector.from_polar(self.velocity * dt, self.pose.theta)
+        new_xy = self.pose.xy + dxy
+        new_theta = self.pose.theta + self.omega * dt
 
-        self.theta += self.omega * dt
+        self.pose = Pose(new_xy.x, new_xy.y, new_theta)
 
         self.t += dt
 
-    def cmd_vel(
-        self, linear_velocity: float, angular_velocity: float
-    ) -> tuple[float, float]:
+    def cmd_vel(self, linear_velocity: float, angular_velocity: float) -> None:
         """set wheel velocities from linear and angular velocities, returns calculated target velocities"""
 
         vl = linear_velocity - angular_velocity * self.W / 2
         vr = linear_velocity + angular_velocity * self.W / 2
 
         self.cmd_lr(vl, vr)
-        return vl, vr
 
-    def cmd_vc(self, linear_velocity: float, curvature: float) -> tuple[float, float]:
+    def cmd_curvature(self, linear_velocity: float, curvature: float) -> None:
         """set wheel velocities from linear velocity and curvature"""
 
         vl, vr = vc_to_vels(linear_velocity, curvature, self.W)
 
         self.cmd_lr(vl, vr)
-        return vl, vr
 
-    def cmd_lr(self, left_velocity: float, right_velocity: float):
+    def cmd_lr(self, left_velocity: float, right_velocity: float) -> None:
         """set wheel velocities from left and right velocities"""
 
         self.left_wheel.set_velocity_ms(left_velocity)
         self.right_wheel.set_velocity_ms(right_velocity)
 
     def __repr__(self) -> str:
         return f"diffdrive vels: ({self.vl:.2f},{self.vr:.2f}) C={self.curvature}"
```

### Comparing `roxbot-1.9.0/src/roxbot/models/linear_model.py` & `roxbot-2.0.0/src/roxbot/models/linear_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
 """
- Simple linear model for generating setpoints.
+Simple linear model for generating setpoints.
 
- Copyright (c) 2023 ROX Automation - Jev Kuznetsov
+Copyright (c) 2023-2024 ROX Automation - Jev Kuznetsov
 """
 
-
 from typing import Optional
-from roxbot.utils import sign
+import math
 
 
 class LinearModel:
     """Simple linear model for generating setpoints."""
 
     __slots__ = ("val", "roc", "setpoint", "min_val", "max_val")
 
@@ -45,15 +44,15 @@
     def step(self, delta_t: float) -> None:
         """perform timestep"""
 
         if delta_t < 0:
             raise ValueError(f"dt may not be negative, got {delta_t=} ")
 
         error = self.setpoint - self.val
-        step = sign(error) * self.roc * delta_t
+        step = math.copysign(1, error) * self.roc * delta_t
 
         if abs(step) > abs(error):
             self.val += error
         else:
             self.val += step
 
         if self.max_val is not None:
```

### Comparing `roxbot-1.9.0/src/roxbot/models/wheels.py` & `roxbot-2.0.0/src/roxbot/models/wheels.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 """
- Driving and steering wheels
+Driving and steering wheels
 
- Copyright (c) 2023 ROX Automation - Jev Kuznetsov
+Copyright (c) 2023 ROX Automation - Jev Kuznetsov
 """
 
 import math
 from typing import Optional
 from .linear_model import LinearModel
 
 
@@ -50,15 +50,15 @@
 
     @property
     def rps(self) -> float:
         """revolutions per second"""
         return self._model.val / self._circumference
 
     @property
-    def velocity_ms(self):
+    def velocity_ms(self) -> float:
         """axle velocity in m/s"""
         return self._model.val
 
     @property
     def revolutions(self) -> float:
         """number of revolutions"""
         return self.distance / self._circumference
@@ -67,14 +67,19 @@
     def ds(self) -> float:
         """distance travelled since last step"""
 
         ds = self.distance - self._distance
         self._distance = self.distance
         return ds
 
+    @property
+    def setpoint(self) -> float:
+        """get velocity setpoint in m/s"""
+        return self._model.setpoint
+
     def set_velocity_ms(self, v: float) -> None:
         """set velocity in m/s"""
         self._model.setpoint = v
 
     def step(self, delta_t: float) -> None:
         """perform timestep to update"""
         self._model.step(delta_t)
```

### Comparing `roxbot-1.9.0/src/roxbot/vectors.py` & `roxbot-2.0.0/src/roxbot/vectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 import cmath
 from math import atan2, cos, hypot, sin
 from typing import Optional
 
 import numpy as np
 from numpy.typing import NDArray  # pylint: disable=import-error, no-name-in-module
-from roxbot.converters import enu_to_latlon, latlon_to_enu
 
 
 class Vector:
     """simple 2d vector class"""
 
     def __init__(self, x: float = 0.0, y: float = 0.0):
         self.x = float(x)
@@ -135,39 +134,27 @@
     def __eq__(self, other: Vector) -> bool:  # type: ignore
         return abs(self - other) < 1e-16
 
     def __array__(self) -> NDArray[np.float32]:
         """numpy array compatibility"""
         return np.array([self.x, self.y])
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: int) -> float:
         """make subscriptable"""
         return [self.x, self.y][item]
 
-    @property
-    def latlon(self) -> tuple[float, float]:
-        """convert from xy to latlon"""
-        return enu_to_latlon(self.xy)
-
-    @classmethod
-    def from_latlon(cls, latlon: tuple[float, float]) -> Vector:
-        """convert from latlon to xy"""
-
-        x, y = latlon_to_enu(latlon)
-        return cls(x, y)
-
 
 class Line:
     """A segment is a line between two points."""
 
     def __init__(self, start: Vector, end: Vector):
         self.start = start
         self.end = end
 
-    def shift_y(self, dy: float):
+    def shift_y(self, dy: float) -> None:
         """Shifts the segment to the left by dy units.
 
         Args:
         - dy: Shift to the left of the line.
         """
 
         # Calculate the direction of the segment
@@ -181,15 +168,15 @@
 
         # Shift the start and end points
         self.start = self.start + shift_left
         self.end = self.end + shift_left
 
     @property
     def phi(self) -> float:
-        """ angle of the line """
+        """angle of the line"""
         return (self.end - self.start).phi
 
     def __repr__(self) -> str:
         return f"<Line(start={self.start}, end={self.end})>"
 
 
 def point_on_line(a: Vector, b: Vector, x: Vector) -> Vector:
```

### Comparing `roxbot-1.9.0/src/roxbot.egg-info/SOURCES.txt` & `roxbot-2.0.0/src/roxbot.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,30 @@
-LICENCE
+LICENSE
 README.md
-setup.py
+pyproject.toml
 src/roxbot/__init__.py
 src/roxbot/cli.py
-src/roxbot/config.py
-src/roxbot/converters.py
-src/roxbot/gps.py
 src/roxbot/interfaces.py
-src/roxbot/odometry.py
 src/roxbot/py.typed
-src/roxbot/topics.py
-src/roxbot/utils.py
 src/roxbot/vectors.py
 src/roxbot/version.py
 src/roxbot.egg-info/PKG-INFO
 src/roxbot.egg-info/SOURCES.txt
 src/roxbot.egg-info/dependency_links.txt
 src/roxbot.egg-info/entry_points.txt
-src/roxbot.egg-info/not-zip-safe
 src/roxbot.egg-info/requires.txt
 src/roxbot.egg-info/top_level.txt
 src/roxbot/bridges/__init__.py
-src/roxbot/bridges/base.py
-src/roxbot/bridges/mock_bridge.py
-src/roxbot/bridges/ros_bridge.py
-src/roxbot/bridges/ws_bridge.py
-src/roxbot/hal/__init__.py
-src/roxbot/hal/base.py
-src/roxbot/hal/canopen.py
-src/roxbot/hal/io.py
+src/roxbot/bridges/mqtt_bridge.py
 src/roxbot/models/__init__.py
 src/roxbot/models/diff_drive.py
 src/roxbot/models/linear_model.py
-src/roxbot/models/protocols.py
-src/roxbot/models/trike.py
 src/roxbot/models/wheels.py
-src/roxbot/nodes/__init__.py
-src/roxbot/nodes/base.py
-src/roxbot/nodes/gps_node.py
-src/roxbot/simulators/__init__.py
-tests/test_bridge.py
-tests/test_cli.py
-tests/test_config.py
+src/roxbot/utils/__init__.py
+src/roxbot/utils/mock_robot.py
+src/roxbot/utils/runners.py
 tests/test_diffdrive.py
-tests/test_gps.py
-tests/test_hal.py
 tests/test_interfaces.py
 tests/test_models.py
-tests/test_nodes.py
-tests/test_odometry.py
-tests/test_topics.py
-tests/test_trike.py
-tests/test_vectors.py
-tests/test_ws_bridge.py
+tests/test_mqtt_bridge.py
+tests/test_smoke.py
+tests/test_vectors.py
```

### Comparing `roxbot-1.9.0/tests/test_diffdrive.py` & `roxbot-2.0.0/tests/test_diffdrive.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,78 +1,91 @@
-""" tests for diff_drive model """
+"""tests for diff_drive model"""
 
 import pytest
 from roxbot.models import DiffDriveModel
+from roxbot.interfaces import Pose, MachineProtocol
 
 
 @pytest.fixture
-def robot():
+def robot() -> DiffDriveModel:
     # Setup with default or custom parameters
     return DiffDriveModel(wheel_base=0.16, wheel_diameter=0.066, wheel_accel=1e6)
 
 
-def test_curvature(robot):
+def test_protocol() -> None:
+    """check protocol compliance, not tested during run, this is for the typechecker"""
+
+    robot: MachineProtocol = DiffDriveModel()
+
+    assert isinstance(robot, DiffDriveModel)
+
+
+def test_curvature(robot: DiffDriveModel) -> None:
     # Test with non-zero velocities
     robot.cmd_lr(1.0, 2.0)
     robot.step(1.0)
     expected_curvature = 1 / (
         0.5 * robot.DEFAULT_WHEEL_BASE * (1.0 + 2.0) / (2.0 - 1.0)
     )
     assert robot.curvature == pytest.approx(expected_curvature)
 
     # Test with zero velocity difference
     robot.cmd_lr(1.0, 1.0)
     robot.step(1.0)
     assert robot.curvature == 0.0
 
 
-def test_set_pose(robot):
+def test_set_pose(robot: DiffDriveModel) -> None:
     x, y, theta = 1.0, 2.0, 3.1415
 
-    robot.pose = (x, y, theta)
+    robot.pose = Pose(x, y, theta)
 
-    assert robot.xy.x == x
-    assert robot.xy.y == y
-    assert robot.theta == theta
+    pose = robot.get_pose()
+    assert pose.x == x
+    assert pose.y == y
+    assert pose.theta == theta
 
 
-def test_vc_to_vels(robot):
+def test_vc_to_vels(robot: DiffDriveModel) -> None:
     v, c = 1.0, 0.5  # Example values for linear velocity and curvature
 
-    vl, vr = robot.cmd_vc(v, c)
+    robot.cmd_curvature(v, c)
+    vl, vr = robot.setpoints
 
     # Calculate expected values
     R = 1 / c
     expected_vr = (v * robot.DEFAULT_WHEEL_BASE + 2 * R * v) / 2 / R
     expected_vl = 2 * v - expected_vr
 
     assert vl == pytest.approx(expected_vl)
     assert vr == pytest.approx(expected_vr)
 
     # Test with zero curvature
-    vl, vr = robot.cmd_vc(v, 0.0)
+    robot.cmd_curvature(v, 0.0)
+    vl, vr = robot.setpoints
 
     assert vl == vr == v
 
 
-def test_cmd_vel_straight_line(robot):
+def test_cmd_vel_straight_line(robot: DiffDriveModel) -> None:
     # Test moving in a straight line (angular velocity = 0)
-    vl, vr = robot.cmd_vel(1.0, 0.0)  # 1 m/s linear velocity, 0 rad/s angular velocity
-    assert vl == 1.0
-    assert vr == 1.0
+    robot.cmd_vel(1.0, 0.0)  # 1 m/s linear velocity, 0 rad/s angular velocity
+    assert robot.left_wheel.setpoint == 1.0
+    assert robot.right_wheel.setpoint == 1.0
 
 
-def test_cmd_vel_turn_in_place(robot):
+def test_cmd_vel_turn_in_place(robot: DiffDriveModel) -> None:
     # Test turning in place (linear velocity = 0)
-    vl, vr = robot.cmd_vel(0.0, 1.0)  # 0 m/s linear velocity, 1 rad/s angular velocity
+    robot.cmd_vel(0.0, 1.0)  # 0 m/s linear velocity, 1 rad/s angular velocity
+    vl, vr = robot.setpoints
     assert vl == -0.08  # -W/2 * angular_velocity
     assert vr == 0.08  # W/2 * angular_velocity
 
 
-def test_repr(robot):
+def test_repr(robot: DiffDriveModel) -> None:
     robot.cmd_lr(1.0, 2.0)
 
     repr_string = repr(robot)
     expected_string = (
         f"diffdrive vels: ({robot.vl:.2f},{robot.vr:.2f}) C={robot.curvature}"
     )
```

### Comparing `roxbot-1.9.0/tests/test_models.py` & `roxbot-2.0.0/tests/test_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import math
 from roxbot.models import LinearModel, Wheel
 
 
-def test_linear_model_init():
+def test_linear_model_init() -> None:
     model = LinearModel(roc=1.0, val=5.0)
     assert model.val == 5.0
     assert model.roc == 1.0
     assert model.setpoint == 5.0
 
     # with setpoint
     model = LinearModel(roc=1.0, val=5.0, setpoint=10.0)
@@ -15,29 +15,29 @@
     assert model.roc == 1.0
     assert model.setpoint == 10.0
 
     # repr method
     assert repr(model) == "LinearModel(val=5.0, setpoint=10.0, roc=1.0)"
 
 
-def test_linear_model_set_target():
+def test_linear_model_set_target() -> None:
     model = LinearModel(roc=1.0, val=5.0)
     model.setpoint = 10.0
     assert model.setpoint == 10.0
 
 
-def test_linear_model_inf():
+def test_linear_model_inf() -> None:
     """test infinite roc"""
     model = LinearModel(roc=math.inf, val=5.0)
     model.setpoint = 10.0
     model.step(1.0)
     assert model.val == 10.0
 
 
-def test_linear_model_step():
+def test_linear_model_step() -> None:
     model = LinearModel(roc=1.0, val=5.0)
     model.setpoint = 10.0
 
     # simulate some steps
     model.step(1.0)
     assert model.val == 6.0
 
@@ -66,15 +66,15 @@
     assert model.val == 2.0
 
     # negative step
     with pytest.raises(ValueError):
         model.step(-0.01)
 
 
-def test_clipping():
+def test_clipping() -> None:
     model = LinearModel(roc=1.0, val=5.0, min_val=-10.0, max_val=10.0)
     model.setpoint = 20.0
     model.step(1.0)
     assert model.val == 6.0
 
     model.step(10.0)
     assert model.val == 10.0
@@ -87,15 +87,15 @@
     model.step(10.0)
     assert model.val == -10.0
 
     model.step(10.0)
     assert model.val == -10.0
 
 
-def test_wheel():
+def test_wheel() -> None:
     # create a wheel with a diameter of 1 meter and an acceleration of 1 radian per second squared # noqa
     wheel = Wheel(diameter=1.0, accel=1.0)
 
     # set the velocity of the wheel to 1 meter per second
     wheel.set_velocity_ms(1.0)
 
     # check acceleration
@@ -111,15 +111,15 @@
     # check that the wheel's angular velocity is correct
     assert wheel.velocity_ms == 1.0
 
     # test repr
     assert repr(wheel) == "Wheel(rps=0.32, velocity=1.00 m/s)"
 
 
-def test_wheel_max_vel():
+def test_wheel_max_vel() -> None:
     """test wheel with max velocity"""
 
     wheel = Wheel(diameter=1.0, accel=1.0, max_velocity=1.5)
 
     wheel.set_velocity_ms(2.0)
     wheel.step(1.0)
     assert wheel.velocity_ms == 1.0
@@ -130,12 +130,12 @@
     wheel.set_velocity_ms(-2.0)
     wheel.step(1.0)
     assert wheel.velocity_ms == 0.5
     wheel.step(2.0)
     assert wheel.velocity_ms == -1.5
 
 
-def test_wheel_properties():
+def test_wheel_properties() -> None:
     wheel = Wheel(diameter=1.0, accel=1.0)
     assert wheel.rps == 0.0
     assert wheel.revolutions == 0.0
     assert wheel.ds == 0.0
```

### Comparing `roxbot-1.9.0/tests/test_vectors.py` & `roxbot-2.0.0/tests/test_vectors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
+# type: ignore
 """
 
  Copyright (c) 2023 ROX Automations
 """
 # type: ignore
 
 import math
 
 import numpy as np
 import pytest
 from pytest import approx
-from roxbot import converters
 
 from roxbot.vectors import Vector, Line, distance_to_b, distance_to_line, point_on_line
 
 
 def almost_equal(v1: Vector, v2: Vector, tolerance: float = 1e-3) -> bool:
     """Checks if two Vectors are almost equal within a given tolerance."""
     return abs(v1.x - v2.x) < tolerance and abs(v1.y - v2.y) < tolerance
@@ -123,23 +123,23 @@
     assert dst == approx(0.2)
 
 
 def test_line_phi():
     a = Vector(0, 0)
     b = Vector(1, 0)
 
-    l = Line(a, b)
-    assert l.phi == 0
+    line = Line(a, b)
+    assert line.phi == 0
 
-    l = Line(Vector(0, 0), Vector(0, 1))
-    assert l.phi == math.radians(90)
+    line = Line(Vector(0, 0), Vector(0, 1))
+    assert line.phi == math.radians(90)
 
     # non-zero start
-    l = Line(Vector(1, 1), Vector(1, 2))
-    assert l.phi == math.radians(90)
+    line = Line(Vector(1, 1), Vector(1, 2))
+    assert line.phi == math.radians(90)
 
 
 def test_distance_to_line():
     """test signed distance to line calculation"""
     a = Vector(0, 0)
     b = Vector(1, 0)
     c = Vector(0.5, 0.5)
@@ -160,65 +160,40 @@
     dst = distance_to_line(a, b, c)
     assert dst == approx(-0.5)
 
     dst = distance_to_line(a, b, d)
     assert dst == approx(0.5)
 
 
-def test_from_latlon():
-    """test conversion from latlon to vector"""
-
-    latlon = (51.365948, 6.172037)
-
-    converters.set_gps_ref(*latlon)
-
-    v = Vector.from_latlon(latlon)
-    assert v.x == approx(0.000000)
-    assert v.y == approx(0.000000)
-
-
-def test_to_latlon():
-    """conversion from vector to latlon"""
-
-    latlon = (51.365948, 6.172037)
-    converters.set_gps_ref(*latlon)
-
-    v = Vector(0, 0)
-
-    lat, lon = v.latlon
-    assert lat == approx(latlon[0])
-    assert lon == approx(latlon[1])
-
-
 def test_line_initialization():
-    l = Line(Vector(0, 0), Vector(1, 1))
-    assert l.start == Vector(0, 0)
-    assert l.end == Vector(1, 1)
+    line = Line(Vector(0, 0), Vector(1, 1))
+    assert line.start == Vector(0, 0)
+    assert line.end == Vector(1, 1)
 
     # repr
-    _ = repr(l)
+    _ = repr(line)
 
 
 def test_line_shift_y():
-    l = Line(Vector(0, 0), Vector(0, 1))
-    l.shift_y(1)
-    assert l.start == Vector(-1, 0)
-    assert l.end == Vector(-1, 1)
+    line = Line(Vector(0, 0), Vector(0, 1))
+    line.shift_y(1)
+    assert line.start == Vector(-1, 0)
+    assert line.end == Vector(-1, 1)
 
     # Test for another shift
-    l.shift_y(-1)
-    assert l.start == Vector(0, 0)
-    assert l.end == Vector(0, 1)
+    line.shift_y(-1)
+    assert line.start == Vector(0, 0)
+    assert line.end == Vector(0, 1)
 
 
 @pytest.mark.parametrize(
     "start, end, dy, shifted_start, shifted_end",
     [
         (Vector(0, 0), Vector(1, 1), 1, Vector(-0.707, 0.707), Vector(0.293, 1.707)),
         (Vector(1, 1), Vector(2, 2), -1, Vector(1.707, 0.293), Vector(2.707, 1.293)),
     ],
 )
 def test_line_shift_y_parametrized(start, end, dy, shifted_start, shifted_end):
-    l = Line(start, end)
-    l.shift_y(dy)
-    assert almost_equal(l.start, shifted_start)
-    assert almost_equal(l.end, shifted_end)
+    line = Line(start, end)
+    line.shift_y(dy)
+    assert almost_equal(line.start, shifted_start)
+    assert almost_equal(line.end, shifted_end)
```

