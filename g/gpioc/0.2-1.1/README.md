# Comparing `tmp/gpioc-0.2.tar.gz` & `tmp/gpioc-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpioc-0.2.tar", last modified: Wed Sep 20 09:40:20 2023, max compression
+gzip compressed data, was "gpioc-1.1.tar", last modified: Wed May 15 07:45:02 2024, max compression
```

## Comparing `gpioc-0.2.tar` & `gpioc-1.1.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxrwxr-x   0 cb        (1000) cb        (1000)        0 2023-09-20 09:40:20.064832 gpioc-0.2/
--rwxrwxrwx   0 cb        (1000) cb        (1000)     1063 2023-09-12 06:55:48.000000 gpioc-0.2/LICENSE
--rw-rw-r--   0 cb        (1000) cb        (1000)       63 2023-09-20 07:30:40.000000 gpioc-0.2/MANIFEST.in
--rw-r--r--   0 cb        (1000) cb        (1000)      490 2023-09-20 09:40:20.064832 gpioc-0.2/PKG-INFO
--rwxrwxrwx   0 cb        (1000) cb        (1000)      283 2023-09-20 09:35:01.000000 gpioc-0.2/README.md
-drwxrwxr-x   0 cb        (1000) cb        (1000)        0 2023-09-20 09:40:20.064832 gpioc-0.2/chips/
--rwxrwxrwx   0 cb        (1000) cb        (1000)    13765 2023-09-20 06:23:26.000000 gpioc-0.2/chips/h616.c
-drwxrwxr-x   0 cb        (1000) cb        (1000)        0 2023-09-20 09:40:20.064832 gpioc-0.2/examples-python/
--rwxrwxrwx   0 cb        (1000) cb        (1000)      263 2023-09-20 09:24:57.000000 gpioc-0.2/examples-python/gpio.py
--rwxrwxrwx   0 cb        (1000) cb        (1000)      164 2023-09-13 08:56:38.000000 gpioc-0.2/examples-python/pwm.py
-drwxrwxr-x   0 cb        (1000) cb        (1000)        0 2023-09-20 09:40:20.064832 gpioc-0.2/gpioc/
--rwxrwxrwx   0 cb        (1000) cb        (1000)     2044 2023-09-19 08:05:35.000000 gpioc-0.2/gpioc/H616.py
--rwxrwxrwx   0 cb        (1000) cb        (1000)      134 2023-09-19 08:09:01.000000 gpioc-0.2/gpioc/__init__.py
--rwxrwxrwx   0 cb        (1000) cb        (1000)     3013 2023-09-19 07:44:35.000000 gpioc-0.2/gpioc/_pin.py
--rwxrwxrwx   0 cb        (1000) cb        (1000)     1195 2023-09-19 08:03:41.000000 gpioc-0.2/gpioc/_pwm.py
-drwxrwxr-x   0 cb        (1000) cb        (1000)        0 2023-09-20 09:40:20.064832 gpioc-0.2/gpioc.egg-info/
--rw-r--r--   0 cb        (1000) cb        (1000)      490 2023-09-20 09:40:19.000000 gpioc-0.2/gpioc.egg-info/PKG-INFO
--rw-rw-r--   0 cb        (1000) cb        (1000)      381 2023-09-20 09:40:20.000000 gpioc-0.2/gpioc.egg-info/SOURCES.txt
--rw-rw-r--   0 cb        (1000) cb        (1000)        1 2023-09-20 09:40:19.000000 gpioc-0.2/gpioc.egg-info/dependency_links.txt
--rw-rw-r--   0 cb        (1000) cb        (1000)        6 2023-09-20 09:40:19.000000 gpioc-0.2/gpioc.egg-info/top_level.txt
-drwxrwxr-x   0 cb        (1000) cb        (1000)        0 2023-09-20 09:40:20.064832 gpioc-0.2/include/
--rwxrwxrwx   0 cb        (1000) cb        (1000)      781 2023-09-19 08:22:12.000000 gpioc-0.2/include/gpioc.h
--rwxrwxrwx   0 cb        (1000) cb        (1000)     1008 2023-09-14 09:01:43.000000 gpioc-0.2/include/h616.h
--rwxrwxrwx   0 cb        (1000) cb        (1000)      376 2023-09-13 09:00:11.000000 gpioc-0.2/include/softpwm.h
--rw-rw-r--   0 cb        (1000) cb        (1000)       38 2023-09-20 09:40:20.064832 gpioc-0.2/setup.cfg
--rwxrwxrwx   0 cb        (1000) cb        (1000)      925 2023-09-20 09:40:15.000000 gpioc-0.2/setup.py
-drwxrwxr-x   0 cb        (1000) cb        (1000)        0 2023-09-20 09:40:20.064832 gpioc-0.2/src/
--rwxrwxrwx   0 cb        (1000) cb        (1000)     2158 2023-09-20 06:23:46.000000 gpioc-0.2/src/gpioc.c
--rwxrwxrwx   0 cb        (1000) cb        (1000)     3259 2023-09-20 06:23:54.000000 gpioc-0.2/src/gpioc_py.c
--rwxrwxrwx   0 cb        (1000) cb        (1000)     5417 2023-09-20 06:24:21.000000 gpioc-0.2/src/softpwm.c
--rwxrwxrwx   0 cb        (1000) cb        (1000)     2894 2023-09-19 07:56:41.000000 gpioc-0.2/src/softpwm_py.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:45:02.608765 gpioc-1.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-15 07:44:58.000000 gpioc-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 07:44:58.000000 gpioc-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-15 07:45:02.608765 gpioc-1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2664 2024-05-15 07:44:58.000000 gpioc-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-15 07:44:58.000000 gpioc-1.1/README_PY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:45:02.604765 gpioc-1.1/examples-python/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      274 2024-05-15 07:44:58.000000 gpioc-1.1/examples-python/gpio.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      198 2024-05-15 07:44:58.000000 gpioc-1.1/examples-python/pwm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:45:02.604765 gpioc-1.1/gpioc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:58.000000 gpioc-1.1/gpioc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:45:02.604765 gpioc-1.1/gpioc/chips/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1103 2024-05-15 07:44:58.000000 gpioc-1.1/gpioc/chips/H616.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:58.000000 gpioc-1.1/gpioc/chips/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2997 2024-05-15 07:44:58.000000 gpioc-1.1/gpioc/pin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1136 2024-05-15 07:44:58.000000 gpioc-1.1/gpioc/pwm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:45:02.608765 gpioc-1.1/gpioc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-15 07:45:02.000000 gpioc-1.1/gpioc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-15 07:45:02.000000 gpioc-1.1/gpioc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:45:02.000000 gpioc-1.1/gpioc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 07:45:02.000000 gpioc-1.1/gpioc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:45:02.608765 gpioc-1.1/libgpio/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      239 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/board.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/board.h
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/gpio.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl-sun50i-h616-r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22484 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl-sun50i-h616.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl-sunxi.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl-sunxi.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1848 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      607 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2359 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/pinctrl_py.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4608 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/softpwm.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/softpwm.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2600 2024-05-15 07:44:58.000000 gpioc-1.1/libgpio/softpwm_py.c
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:45:02.608765 gpioc-1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1060 2024-05-15 07:44:58.000000 gpioc-1.1/setup.py
```

### Comparing `gpioc-0.2/LICENSE` & `gpioc-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpioc-0.2/gpioc/_pin.py` & `gpioc-1.1/gpioc/pin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 
-import gpioc._gpioc as _gpio
+import gpioc._pinctrl as _gpio
 
 class Pin:
     IN = 0
     OUT = 1
     LOW = 0
     HIGH = 1
     PULL_NONE = 0
     PULL_UP = 1
     PULL_DOWN = 2
 
     id = None
     _value = LOW
     _mode = IN
 
-    def _setup(self, gpio_num, dir, pull_up_down=None ):
+    def _setup(self, gpio:int, dir, pull_up_down=None ):
         if dir == _gpio.f_INPUT :
-            _gpio.set_mode(gpio_num, _gpio.f_INPUT)
+            _gpio.set_mode(gpio, _gpio.f_INPUT)
             if pull_up_down == self.PULL_UP:
-                _gpio.set_pullUpDn(gpio_num, _gpio.f_pullUp)
+                _gpio.set_pullUpDn(gpio, _gpio.f_pullUp)
             elif pull_up_down == self.PULL_DOWN:
-                _gpio.set_pullUpDn(gpio_num, _gpio.f_pullDown)
+                _gpio.set_pullUpDn(gpio, _gpio.f_pullDown)
             else:
-                _gpio.set_pullUpDn(gpio_num, _gpio.f_pull_OFF)
+                _gpio.set_pullUpDn(gpio, _gpio.f_pull_OFF)
         if dir == _gpio.f_OUTPUT :
-            _gpio.set_mode(gpio_num, _gpio.f_OUTPUT)
+            _gpio.set_mode(gpio, _gpio.f_OUTPUT)
                 
     # self.output(self.id, val)
     def _output(self, gpio_num, val):
         _gpio.write(gpio_num, val)
 
     # return _gpio.input(self.id)
     def _input(self, gpio_num):
         return _gpio.read(gpio_num)
 
-    def __init__(self, pin_name):
-        if isinstance(pin_name, tuple):
-            self.id = int(pin_name[1])
+    def __init__(self, gpio_num):
+        if isinstance(gpio_num, tuple):
+            self.id = int(gpio_num[1])
         else:
-            self.id = int(pin_name)
+            self.id = int(gpio_num)
 
     def __repr__(self):
         return str(self.id)
 
     def __eq__(self, other):
         return self.id == other
 
@@ -61,20 +61,20 @@
 
             else:
                 raise RuntimeError("Invalid mode for pin: %s" % self.id)
         if pull is not None:
             if self._mode != self.IN:
                 raise RuntimeError("Cannot set pull resistor on output")
             if pull == self.PULL_UP:
-                # GPIO.setup(self.id, GPIO.IN, pull_up_down=GPIO.PUD_UP)
+                # GPIO.setup(self.id, GPIO.IN, pull_up_down=GPIO.PULL_UP)
                 self._setup(self.id, self.IN, pull_up_down=self.PULL_UP)
                 
 
             elif pull == self.PULL_DOWN:
-                # GPIO.setup(self.id, GPIO.IN, pull_up_down=GPIO.PUD_DOWN)
+                # GPIO.setup(self.id, GPIO.IN, pull_up_down=GPIO.PULL_DOWN)
                 self._setup(self.id, self.IN, pull_up_down=self.PULL_DOWN)
 
                 pass
             else:
                 raise RuntimeError("Invalid pull for pin: %s" % self.id)
             
     def value(self, val=None):
```

### Comparing `gpioc-0.2/gpioc/_pwm.py` & `gpioc-1.1/gpioc/pwm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 import gpioc._softpwm as _pwm
-import gpioc as _gpio
+from gpioc.pin import Pin
 
-class PWMOut_father:
+class Pwm:
     """Base Pulse Width Modulation Output Class"""
-    _gpio_num = 0
-    _chip = 0 
-    def __init__(self, pin, *, frequency=500, duty_cycle=0, variable_frequency=False):
-        self._gpio_num = pin.id
-
-        pin.init(pin.OUT)
-        _pwm.switch_chip(self._chip)
-        _pwm.set_frequency(self._gpio_num, frequency)
-        _pwm.set_duty_cycle(self._gpio_num, duty_cycle)
-        _pwm.start(self._gpio_num)
+    gpio_num = 0
+    def __init__(self, gpio:int, *, frequency=500, duty_cycle=0, variable_frequency=False):
+
+        self.gpio_num = gpio
+        Pin(gpio).init(Pin.OUT)
+        _pwm.set_frequency(self.gpio_num, frequency)
+        _pwm.set_duty_cycle(self.gpio_num, duty_cycle)
+        _pwm.start(self.gpio_num)
         
 
     def __del__(self):
         self.deinit()
 
     def __enter__(self):
         return self
 
     def __exit__(self, t, value, traceback):
         self.deinit()
 
     def deinit(self):
-        _pwm.stop(self._gpio_num)
+        _pwm.stop(self.gpio_num)
 
     @property
     def duty_cycle(self):
         """The PWM's output duty cycle, 16-bit."""
-        return _pwm.get_duty_cycle(self._gpio_num)
+        return _pwm.get_duty_cycle(self.gpio_num)
         
     @duty_cycle.setter
     def duty_cycle(self, duty_cycle):
-        _pwm.set_duty_cycle(self._gpio_num, int(duty_cycle))
+        _pwm.set_duty_cycle(self.gpio_num, int(duty_cycle))
 
     @property
     def frequency(self):
-        return _pwm.get_frequency(self._gpio_num)
+        return _pwm.get_frequency(self.gpio_num)
 
     @frequency.setter
     def frequency(self, frequency):
-        _pwm.set_frequency(self._gpio_num, int(frequency))
+        _pwm.set_frequency(self.gpio_num, int(frequency))
```

### Comparing `gpioc-0.2/src/gpioc.c` & `gpioc-1.1/libgpio/pinctrl.c`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,73 @@
 #include <stdio.h>
 #include <stdlib.h>
 #include <unistd.h>
 #include <string.h>
 
-#include "../include/softpwm.h"
-#include "../include/h616.h"
+#include "pinctrl-sunxi.h"
 
-
-
-static char *chips_compatible[] = {
-    "占位符",
-    "sun50i-h616"};
-
-
-
-int detect()
-{
-    FILE *fp;
-    char buffer[1024];
-    char *compatible;
-    int i;
-    fp = fopen("/proc/device-tree/compatible", "r");
-    if (fp == NULL)
-    {
-        printf("Failed to open /proc/device-tree/compatible \n");
-        return -1;
-    }
-
-    fgets(buffer, 100, fp);
-    fclose(fp);
-
-    // printf("compatible=\t%s\r\n",buffer);
-    compatible = strtok(buffer, "\n");
-
-    for (i = 0; i < (int)sizeof(chips_compatible)/(int)sizeof(char *); i++)
-    {
-        // printf("[%d]=%s\r\n", i, chips_compatible[i]);
-        if (strstr(compatible, chips_compatible[i]) != NULL)
-        {
-            return i;
-        }
-    }
-    return -1;
-}
+static int _ops_select = 0;
 
 void (*chip_pin_set_mode[])(int, int) = {
     0,
-    H616_pin_set_mode,
-};
-
-void (*chip_pin_set_alt[])(int, int) = {
-    0,
-    H616_pin_set_alt,
+    sunxi_pin_set_mode,
 };
 
-int (*chip_pin_get_alt[])(int) = {
+int (*chip_pin_get_mode[])(int) = {
     0,
-    H616_pin_get_alt,
+    sunxi_pin_get_mode,
 };
 
 int (*chip_gpio_read[])(int) = {
     0,
-    H616_gpio_read,
+    sunxi_gpio_read,
 };
 
 void (*chip_gpio_write[])(int, int) = {
     0,
-    H616_gpio_write,
+    sunxi_gpio_write,
 };
 
 void (*chip_gpio_set_PullUpDn[])(int, int) = {
     0,
-    H616_gpio_set_PullUpDn,
+    sunxi_gpio_set_PullUpDn,
 };
 
-
+void (*chip_who_has_function[])(char *, int) = {
+    0,
+    sunxi_print_who_has_function,
+};
+const char *(*chip_gpio_pin_get_mode_name[])(int) = {
+    0,
+    sunxi_pin_get_mode_name,
+};
+const char *(*chip_gpio_pin_get_mode_name_by_num[])(int, int) = {
+    0,
+    sunxi_pin_get_mode_name_by_num,
+};
 
 int chip_detect()
 {
-    int chip = detect();
-    // printf("chip=%d\r\n",chip);
-    int num = sizeof(chip_gpio_read) / sizeof(chip_gpio_read[0]);
-
-    if (chip < 1)
-        exit(-1);
-    else if (chip > num)
-        exit(-1);
-    else
-        return chip;
-}
+    if (_ops_select == 0)
+    {
+        if (sunxi_init())
+        {
+            _ops_select = 1;
+        }
+    }
 
-int gpio_get_Alt(int gpio_num)
-{
-    return chip_pin_get_alt[chip_detect()](gpio_num);
+    return _ops_select;
 }
 
-void gpio_set_Alt(int gpio_num, int mode)
+int gpio_get_mode(int gpio_num)
 {
-    chip_pin_set_alt[chip_detect()](gpio_num, mode);
+    return chip_pin_get_mode[chip_detect()](gpio_num);
 }
 
-void gpio_set_Mode(int gpio_num, int mode)
+void gpio_set_mode(int gpio_num, int mode)
 {
     chip_pin_set_mode[chip_detect()](gpio_num, mode);
 }
 
 void gpio_set_pullUpDn(int gpio_num, int pud)
 {
     chip_gpio_set_PullUpDn[chip_detect()](gpio_num, pud);
@@ -115,7 +78,19 @@
     return chip_gpio_read[chip_detect()](gpio_num);
 }
 
 void gpio_write(int gpio_num, int value)
 {
     chip_gpio_write[chip_detect()](gpio_num, value);
 }
+void gpio_print_who_has_function(char *name_buf, int len)
+{
+    chip_who_has_function[chip_detect()](name_buf, len);
+}
+const char *gpio_pin_get_mode_name(int gpio_num)
+{
+    return chip_gpio_pin_get_mode_name[chip_detect()](gpio_num);
+}
+const char *gpio_pin_get_mode_name_by_num(int gpio_num, int mode_num)
+{
+    return chip_gpio_pin_get_mode_name_by_num[chip_detect()](gpio_num, mode_num);
+}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gpioc-0.2/src/gpioc_py.c` & `gpioc-1.1/libgpio/pinctrl_py.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,29 @@
 #include <Python.h>
 
-
-#include "../include/gpioc.h"
+#include "pinctrl.h"
 
 void define_commons(PyObject *module)
 {
-    PyModule_AddObject(module, "CHIP_H616", Py_BuildValue("i", CHIP_H616));
+    // PyModule_AddObject(module, "CHIP_H616", Py_BuildValue("i", CHIP_H616));
 
     PyModule_AddObject(module, "f_INPUT", Py_BuildValue("i", INPUT));
     PyModule_AddObject(module, "f_OUTPUT", Py_BuildValue("i", OUTPUT));
 
-    PyModule_AddObject(module, "f_pull_OFF", Py_BuildValue("i", PUD_OFF));
-    PyModule_AddObject(module, "f_pullDown", Py_BuildValue("i", PUD_DOWN));
-    PyModule_AddObject(module, "f_pullUp", Py_BuildValue("i", PUD_UP));
-}
-
-static PyObject *py_detect(PyObject *self, PyObject *args)
-{
-    return Py_BuildValue("i", detect());
+    PyModule_AddObject(module, "f_pull_OFF", Py_BuildValue("i", PULL_OFF));
+    PyModule_AddObject(module, "f_pullDown", Py_BuildValue("i", PULL_DOWN));
+    PyModule_AddObject(module, "f_pullUp", Py_BuildValue("i", PULL_UP));
 }
 
 static PyObject *py_write(PyObject *self, PyObject *args)
 {
     int ret;
     int gpio_num, value;
     ret = PyArg_ParseTuple(args, "ii", &gpio_num, &value);
 
-    // printf("ret=%d\r\n", ret);
-    // printf("gpio_num=%d\r\n", gpio_num);
-    // printf("value=%d\r\n", value);
-
     gpio_write(gpio_num, value);
 
     Py_RETURN_NONE;
 }
 static PyObject *py_read(PyObject *self, PyObject *args)
 {
     int ret;
@@ -50,62 +40,41 @@
 
     gpio_set_pullUpDn(gpio_num, pud);
 
     Py_RETURN_NONE;
 }
 static PyObject *py_set_mode(PyObject *self, PyObject *args)
 {
-    int ret;
-    int gpio_num, mode;
-    ret = PyArg_ParseTuple(args, "ii", &gpio_num, &mode);
-    gpio_set_Mode(gpio_num, mode);
-    Py_RETURN_NONE;
-}
-static PyObject *py_set_alt(PyObject *self, PyObject *args)
-{
-    int ret;
+   int ret;
     int gpio_num, mode;
     ret = PyArg_ParseTuple(args, "ii", &gpio_num, &mode);
-    gpio_set_Alt(gpio_num, mode);
+    gpio_set_mode(gpio_num, mode);
     Py_RETURN_NONE;
 }
-static PyObject *py_get_alt(PyObject *self, PyObject *args)
-{
-    int ret;
-    int gpio_num;
-    ret = PyArg_ParseTuple(args, "i", &gpio_num);
-
-    return Py_BuildValue("i", gpio_get_Alt(gpio_num));
-}
 
-static const char moduledocstring[] = "GPIO functionality of allwinner h616";
+static const char moduledocstring[] = "GPIO functionality";
 
-PyMethodDef gpioc_methods[] = {
-    {"detect", py_detect, METH_VARARGS, "detect now chip by device-tree"},
+PyMethodDef pinctrl_methods[] = {
     {"write", py_write, METH_VARARGS, "write value to gpio"},
     {"read", py_read, METH_VARARGS, "read value from gpio"},
     {"set_pullUpDn", py_set_PullUpDn, METH_VARARGS, "set the gpio with pullup or pulldown"},
     {"set_mode", py_set_mode, METH_VARARGS, "set the gpio mode with in or out"},
-    {"set_alt", py_set_alt, METH_VARARGS, "set the pin mode functiont"},
-    {"get_alt", py_get_alt, METH_VARARGS, "get the pin mode functiont"},
     {NULL, NULL, 0, NULL},
 };
-static struct PyModuleDef gpiocmodule = {
+static struct PyModuleDef module_pinctrl = {
     PyModuleDef_HEAD_INIT,
-    "gpioc._gpioc",  // name of module
+    "_pinctrl",      // name of module
     moduledocstring, // module documentation, may be NULL
     -1,              // size of per-interpreter state of the module, or -1 if the module keeps state in global variables.
-    gpioc_methods};
+    pinctrl_methods};
 
 // 在import时会被调出来执行
-PyMODINIT_FUNC PyInit__gpioc(void)
+PyMODINIT_FUNC PyInit__pinctrl(void)
 {
-    // printf("PyInit__h616\r\n");
     PyObject *module = NULL;
 
-    if ((module = PyModule_Create(&gpiocmodule)) == NULL)
+    if ((module = PyModule_Create(&module_pinctrl)) == NULL)
         return NULL;
-
     define_commons(module);
-
+    
     return module;
 }
```

### Comparing `gpioc-0.2/src/softpwm.c` & `gpioc-1.1/libgpio/softpwm.c`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,19 @@
-
 #include <stdlib.h>
 #include <stdio.h>
 #include <pthread.h>
 #include <time.h>
 #include <signal.h>
 #include <unistd.h>
 
-#include "../include/softpwm.h"
-#include "../include/gpioc.h"
-#include "../include/h616.h"
+#include "pinctrl.h"
 
 #define NS_1S 1000000000
-#define DUTY_CYCLE_FULL 65535
-
-// 不同芯片的寄存器不同，write函数也不一样
-void (*gpio_out)(int, int) = H616_gpio_write;
-void switch_chip(int flag)
-{
-    switch (flag)
-    {
-    case CHIP_H616:
-        gpio_out = H616_gpio_write;
-
-        break;
+#define DUTY_CYCLE_FULL 100
 
-    default:
-        break;
-    }
-}
 struct pwm
 {
     unsigned int gpio;
     int freq;
     int dutycycle;
 
     unsigned int cycle_high;
@@ -68,71 +50,56 @@
         {
             prev = p;
             p = p->next;
         }
     }
 }
 
-
 void calculate_times(struct pwm *p)
 {
 
     int full_cycle, cycle_high, cycle_low;
-    // printf("freq=%d\r\n", p->freq);
-    // printf("dutycycle=%d\r\n", p->dutycycle);
 
     full_cycle = NS_1S / p->freq;
     cycle_high = full_cycle / DUTY_CYCLE_FULL * p->dutycycle;
     cycle_low = full_cycle - cycle_high;
-
-    // printf("cycle_high=%d\r\n", cycle_high);
-    // printf("cycle_low=%d\r\n", cycle_low);
     p->req_on.tv_sec = 0;
     p->req_on.tv_nsec = (long)cycle_high;
 
     p->req_off.tv_sec = 0;
     p->req_off.tv_nsec = (long)cycle_low;
 }
 void full_sleep(struct timespec *req)
 {
     struct timespec rem = {0};
-
     if (nanosleep(req, &rem) == -1)
     {
-        // printf("nanosleep(req, &rem) == -1");
         full_sleep(&rem);
     }
-        usleep(100);
-}   
+}
 
 void *pwm_thread(void *threadarg)
 {
     struct pwm *p = (struct pwm *)threadarg;
-    // printf("pwm_thread\r\n");
+    gpio_set_mode(p->gpio, OUTPUT);
     while (p->running)
     {
         if (p->dutycycle > 0)
         {
-            // printf("-");
-            gpio_out(p->gpio, 1);
-            
-            // usleep(p->cycle_high);
+            gpio_write(p->gpio, 1);
             full_sleep(&p->req_on);
         }
 
         if (p->dutycycle < DUTY_CYCLE_FULL)
         {
-            // printf("+");
-            gpio_out(p->gpio, 0);
-            // usleep(p->cycle_low);
-
+            gpio_write(p->gpio, 0);
             full_sleep(&p->req_off);
         }
     }
-    gpio_out(p->gpio, 0);
+    gpio_write(p->gpio, 0);
     // clean up
     free(p);
     pthread_exit(NULL);
 }
 
 struct pwm *add_new_pwm(unsigned int gpio)
 {
@@ -263,16 +230,13 @@
         }
     }
     return 0;
 }
 
 // int main()
 // {
-//     gpio_out = H616_gpio_write;
-//     pwm_set_duty_cycle(270, 1);
-//     pwm_set_frequency(270, 1000);
+//     pwm_set_duty_cycle(270, 50);
+//     pwm_set_frequency(270, 2000);
 //     pwm_start(270);
-//     while (1)
-//         ;
-//     //  gpio_out(270, 0);
+//     while (1);
 //     return 0;
-// }
+// }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gpioc-0.2/src/softpwm_py.c` & `gpioc-1.1/libgpio/softpwm_py.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,11 @@
 #include <Python.h>
 
-// #include "h616_gpio.h"
-// #include "common.h"
 
 
-static PyObject *py_switch_chip(PyObject *self, PyObject *args)
-{
-    int ret;
-    int flag;
-    ret = PyArg_ParseTuple(args, "i", &flag);
-    switch_chip( flag);
-    Py_RETURN_NONE;
-}
 
 static PyObject *py_set_duty_cycle(PyObject *self, PyObject *args)
 {
     int ret;
     int gpio_num, dutycycle;
     ret = PyArg_ParseTuple(args, "ii", &gpio_num, &dutycycle);
     pwm_set_duty_cycle(gpio_num, dutycycle);
@@ -73,34 +63,33 @@
     pwm_exists(gpio_num);
     Py_RETURN_NONE;
 }
 
 static const char moduledocstring[] = "soft pwm";
 
 PyMethodDef pwm_methods[] = {
-    {"switch_chip", py_switch_chip, METH_VARARGS, "switch chip"},
     {"get_duty_cycle", py_get_duty_cycle, METH_VARARGS, "get_duty_cycle with gpio num"},
     {"get_frequency", py_get_frequency, METH_VARARGS, "get_frequency with gpio num"},
     {"set_duty_cycle", py_set_duty_cycle, METH_VARARGS, "set_duty_cycle with gpio num"},
     {"set_frequency", py_set_frequency, METH_VARARGS, "set_frequency with gpio num"},
     {"start", py_start, METH_VARARGS, "start pwm output"},
     {"stop", py_stop, METH_VARARGS, "stop pwm"},
     {"exists", py_exists, METH_VARARGS, "exists"},
 
 };
-static struct PyModuleDef gpiocmodule = {
+static struct PyModuleDef module_pinctrl = {
     PyModuleDef_HEAD_INIT,
     "gpioc._pwm",      // name of module
     moduledocstring, // module documentation, may be NULL
     -1,              // size of per-interpreter state of the module, or -1 if the module keeps state in global variables.
     pwm_methods};
 
 // 在import时会被调出来执行
 PyMODINIT_FUNC PyInit__softpwm(void)
 {
     PyObject *module = NULL;
 
-    if ((module = PyModule_Create(&gpiocmodule)) == NULL)
+    if ((module = PyModule_Create(&module_pinctrl)) == NULL)
         return NULL;
 
     return module;
 }
```

