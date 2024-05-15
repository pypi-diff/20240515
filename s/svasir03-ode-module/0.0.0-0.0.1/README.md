# Comparing `tmp/svasir03_ode_module-0.0.0.tar.gz` & `tmp/svasir03_ode_module-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svasir03_ode_module-0.0.0.tar", last modified: Mon May 13 15:14:43 2024, max compression
+gzip compressed data, was "svasir03_ode_module-0.0.1.tar", last modified: Wed May 15 18:57:50 2024, max compression
```

## Comparing `svasir03_ode_module-0.0.0.tar` & `svasir03_ode_module-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 15:14:43.054858 svasir03_ode_module-0.0.0/
--rw-rw-rw-   0        0        0     1107 2024-05-13 15:07:21.000000 svasir03_ode_module-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      489 2024-05-13 15:14:43.052857 svasir03_ode_module-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       75 2024-05-13 15:07:19.000000 svasir03_ode_module-0.0.0/README.md
--rw-rw-rw-   0        0        0      500 2024-05-13 15:00:50.000000 svasir03_ode_module-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 15:14:43.054858 svasir03_ode_module-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 15:14:43.035591 svasir03_ode_module-0.0.0/src/
--rw-rw-rw-   0        0        0        0 2024-05-13 14:52:59.000000 svasir03_ode_module-0.0.0/src/__init__.py
--rw-rw-rw-   0        0        0     1527 2024-05-13 14:53:02.000000 svasir03_ode_module-0.0.0/src/ode.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:14:43.051861 svasir03_ode_module-0.0.0/src/svasir03_ode_module.egg-info/
--rw-rw-rw-   0        0        0      489 2024-05-13 15:14:42.000000 svasir03_ode_module-0.0.0/src/svasir03_ode_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-05-13 15:14:42.000000 svasir03_ode_module-0.0.0/src/svasir03_ode_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 15:14:42.000000 svasir03_ode_module-0.0.0/src/svasir03_ode_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-13 15:14:42.000000 svasir03_ode_module-0.0.0/src/svasir03_ode_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-13 15:14:42.000000 svasir03_ode_module-0.0.0/src/svasir03_ode_module.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 15:14:43.049857 svasir03_ode_module-0.0.0/tests/
--rw-rw-rw-   0        0        0     1205 2024-05-13 14:08:46.000000 svasir03_ode_module-0.0.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:57:50.181262 svasir03_ode_module-0.0.1/
+-rw-rw-rw-   0        0        0     1107 2024-05-13 15:07:21.000000 svasir03_ode_module-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0      489 2024-05-15 18:57:50.179615 svasir03_ode_module-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2024-05-13 15:07:19.000000 svasir03_ode_module-0.0.1/README.md
+-rw-rw-rw-   0        0        0      500 2024-05-14 11:10:03.000000 svasir03_ode_module-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 18:57:50.182340 svasir03_ode_module-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 18:57:50.147661 svasir03_ode_module-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 18:57:50.162978 svasir03_ode_module-0.0.1/src/odeSolver/
+-rw-rw-rw-   0        0        0       16 2024-05-14 11:09:59.000000 svasir03_ode_module-0.0.1/src/odeSolver/__init__.py
+-rw-rw-rw-   0        0        0     1532 2024-05-14 07:54:12.000000 svasir03_ode_module-0.0.1/src/odeSolver/ode.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:57:50.178603 svasir03_ode_module-0.0.1/src/svasir03_ode_module.egg-info/
+-rw-rw-rw-   0        0        0      489 2024-05-15 18:57:50.000000 svasir03_ode_module-0.0.1/src/svasir03_ode_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-05-15 18:57:50.000000 svasir03_ode_module-0.0.1/src/svasir03_ode_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 18:57:50.000000 svasir03_ode_module-0.0.1/src/svasir03_ode_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-15 18:57:50.000000 svasir03_ode_module-0.0.1/src/svasir03_ode_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 18:57:50.000000 svasir03_ode_module-0.0.1/src/svasir03_ode_module.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 18:57:50.162978 svasir03_ode_module-0.0.1/tests/
+-rw-rw-rw-   0        0        0     1287 2024-05-14 07:54:00.000000 svasir03_ode_module-0.0.1/tests/test.py
```

### Comparing `svasir03_ode_module-0.0.0/LICENSE` & `svasir03_ode_module-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `svasir03_ode_module-0.0.0/src/ode.py` & `svasir03_ode_module-0.0.1/src/odeSolver/ode.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     times = np.linspace(time_span[0], time_span[1], num_of_steps + 1)
     values = np.zeros((len(times), len(initial_value)))
     values[0] = initial_value
 
     time_step = times[1] - times[0]
 
     def calc_next_value(time, value):
-        next_value = value + time_step * ode_func(time, value, args)
+        next_value = value + time_step * ode_func(time, value, *args)
         return next_value
 
     for i in range(len(times) - 1):
         next_value = calc_next_value(times[i], values[i])
         values[i+1] = next_value
 
     values = np.transpose(values)
@@ -26,18 +26,18 @@
     times = np.linspace(time_span[0], time_span[1], num_of_steps + 1)
     values = np.zeros((len(times), len(initial_value)))
     values[0] = initial_value
 
     time_step = times[1] - times[0]
 
     def calc_next_value(time, value):
-        k1 = ode_func(time, value, args)
-        k2 = ode_func(time + time_step / 2, value + k1 * time_step / 2, args)
-        k3 = ode_func(time + time_step / 2, value + k2 * time_step / 2, args)
-        k4 = ode_func(time + time_step, value + k3 * time_step, args)
+        k1 = ode_func(time, value, *args)
+        k2 = ode_func(time + time_step / 2, value + k1 * time_step / 2, *args)
+        k3 = ode_func(time + time_step / 2, value + k2 * time_step / 2, *args)
+        k4 = ode_func(time + time_step, value + k3 * time_step, *args)
 
         next_value = value + time_step / 6 * (k1 + 2*k2 + 2*k3 + k4)
         return next_value
 
     for i in range(len(times) - 1):
         next_value = calc_next_value(times[i], values[i])
         values[i+1] = next_value
```

### Comparing `svasir03_ode_module-0.0.0/tests/test.py` & `svasir03_ode_module-0.0.1/tests/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import numpy as np
 import matplotlib.pyplot as plt
-from ..src import ode
+import ode
 
 #Params
 TIME_SPAN = (0, 9.9)
-INITIAL_VALUE = np.array([0, 0])
+INITIAL_VALUE = np.array([np.pi / 4, 0])
 omega = 2*np.pi
 omega_0 = 3*np.pi
 gamma = 0.1
 NUM_OF_STEPS = 10000
 
 #ODE func
-def ODE_func(time,value, params):
+def ODE_func(time,value, a, b, c):
     angle_vel= value[1]
-    angle_acc = params[2] * (params[1]**2)*np.cos(params[0]*time) -(params[1]**2)*value[0]
+    angle_acc = c * (b**2)*np.cos(a*time) -(b**2)*value[0]
+    
+    return np.array([angle_vel, angle_acc])
+
+def ode_func(time, value):
+    angle_vel= value[1]
+    angle_acc = -np.sin(value[0])
     
     return np.array([angle_vel, angle_acc])
 
 
 #analytic func
 def analytic_func(time, omega, omega0, gamma):
     #case w==w0
@@ -34,13 +40,12 @@
 #times_RK4, values_RK4 = ode.solve_RK4(ODE_func, TIME_SPAN, NUM_OF_STEPS, INITIAL_VALUE, omega, omega_0, gamma)
 
 #plt.plot(times_RK4, values_RK4[0])
 
 #error = values_RK4[0][-1] - analytic_func(9.9, omega, omega_0, gamma)
 #print(error)
 
-times_RK1, values_RK1 = ode.solve_RK1(ODE_func, TIME_SPAN, NUM_OF_STEPS, INITIAL_VALUE, omega, omega_0, gamma)
+times_RK1, values_RK1 = ode.solve_RK1(ode_func, TIME_SPAN, NUM_OF_STEPS, INITIAL_VALUE)
 
 plt.plot(times_RK1, values_RK1[0])
 
-
 plt.show()
```

