# Comparing `tmp/calc_ultra-1.3.5.tar.gz` & `tmp/calc_ultra-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calc_ultra-1.3.5.tar", last modified: Thu May  2 10:12:50 2024, max compression
+gzip compressed data, was "calc_ultra-1.3.6.tar", last modified: Wed May 15 12:23:00 2024, max compression
```

## Comparing `calc_ultra-1.3.5.tar` & `calc_ultra-1.3.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-02 10:12:50.463678 calc_ultra-1.3.5/
--rw-r--r--   0 Huatao     (502) staff       (20)     1068 2023-12-31 12:50:35.000000 calc_ultra-1.3.5/LICENSE
--rw-r--r--   0 Huatao     (502) staff       (20)       21 2023-12-09 18:58:14.000000 calc_ultra-1.3.5/MANIFEST.in
--rw-r--r--   0 Huatao     (502) staff       (20)     4331 2024-05-02 10:12:50.463468 calc_ultra-1.3.5/PKG-INFO
--rw-r--r--   0 Huatao     (502) staff       (20)     3562 2024-05-02 06:15:42.000000 calc_ultra-1.3.5/README.md
--rw-r--r--   0 Huatao     (502) staff       (20)      892 2024-05-02 06:00:00.000000 calc_ultra-1.3.5/pyproject.toml
--rw-r--r--   0 Huatao     (502) staff       (20)       38 2024-05-02 10:12:50.463726 calc_ultra-1.3.5/setup.cfg
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-02 10:12:50.459610 calc_ultra-1.3.5/src/
--rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-05-02 10:10:35.000000 calc_ultra-1.3.5/src/.DS_Store
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-02 10:12:50.460410 calc_ultra-1.3.5/src/calc_ultra/
--rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-04-28 11:10:07.000000 calc_ultra-1.3.5/src/calc_ultra/.DS_Store
--rw-r--r--   0 Huatao     (502) staff       (20)      128 2024-02-05 08:04:02.000000 calc_ultra-1.3.5/src/calc_ultra/__init__.py
--rw-r--r--   0 Huatao     (502) staff       (20)    42581 2024-05-02 10:00:41.000000 calc_ultra-1.3.5/src/calc_ultra/main.py
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-02 10:12:50.462792 calc_ultra-1.3.5/src/calc_ultra/texts/
--rw-r--r--   0 Huatao     (502) staff       (20)        0 2023-12-09 18:58:14.000000 calc_ultra-1.3.5/src/calc_ultra/texts/__init__.py
--rw-r--r--   0 Huatao     (502) staff       (20)      546 2024-03-19 08:27:24.000000 calc_ultra-1.3.5/src/calc_ultra/texts/algcalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      740 2024-03-06 07:59:13.000000 calc_ultra-1.3.5/src/calc_ultra/texts/derivacalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      761 2024-04-14 10:36:05.000000 calc_ultra-1.3.5/src/calc_ultra/texts/intecalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      531 2024-03-06 07:59:34.000000 calc_ultra-1.3.5/src/calc_ultra/texts/limcalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      706 2024-05-01 04:38:23.000000 calc_ultra-1.3.5/src/calc_ultra/texts/main_screen.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      232 2024-04-14 10:37:09.000000 calc_ultra-1.3.5/src/calc_ultra/texts/settings.txt
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-02 10:12:50.463212 calc_ultra-1.3.5/src/calc_ultra.egg-info/
--rw-r--r--   0 Huatao     (502) staff       (20)     4331 2024-05-02 10:12:50.000000 calc_ultra-1.3.5/src/calc_ultra.egg-info/PKG-INFO
--rw-r--r--   0 Huatao     (502) staff       (20)      562 2024-05-02 10:12:50.000000 calc_ultra-1.3.5/src/calc_ultra.egg-info/SOURCES.txt
--rw-r--r--   0 Huatao     (502) staff       (20)        1 2024-05-02 10:12:50.000000 calc_ultra-1.3.5/src/calc_ultra.egg-info/dependency_links.txt
--rw-r--r--   0 Huatao     (502) staff       (20)       94 2024-05-02 10:12:50.000000 calc_ultra-1.3.5/src/calc_ultra.egg-info/requires.txt
--rw-r--r--   0 Huatao     (502) staff       (20)       11 2024-05-02 10:12:50.000000 calc_ultra-1.3.5/src/calc_ultra.egg-info/top_level.txt
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-15 12:23:00.161177 calc_ultra-1.3.6/
+-rw-r--r--   0 Huatao     (502) staff       (20)     1068 2023-12-31 12:50:35.000000 calc_ultra-1.3.6/LICENSE
+-rw-r--r--   0 Huatao     (502) staff       (20)       21 2023-12-09 18:58:14.000000 calc_ultra-1.3.6/MANIFEST.in
+-rw-r--r--   0 Huatao     (502) staff       (20)     4203 2024-05-15 12:23:00.160963 calc_ultra-1.3.6/PKG-INFO
+-rw-r--r--   0 Huatao     (502) staff       (20)     3434 2024-05-14 14:05:23.000000 calc_ultra-1.3.6/README.md
+-rw-r--r--   0 Huatao     (502) staff       (20)      892 2024-05-14 13:18:36.000000 calc_ultra-1.3.6/pyproject.toml
+-rw-r--r--   0 Huatao     (502) staff       (20)       38 2024-05-15 12:23:00.161224 calc_ultra-1.3.6/setup.cfg
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-15 12:23:00.157391 calc_ultra-1.3.6/src/
+-rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-05-15 12:22:16.000000 calc_ultra-1.3.6/src/.DS_Store
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-15 12:23:00.158212 calc_ultra-1.3.6/src/calc_ultra/
+-rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-05-15 11:24:35.000000 calc_ultra-1.3.6/src/calc_ultra/.DS_Store
+-rw-r--r--   0 Huatao     (502) staff       (20)      128 2024-02-05 08:04:02.000000 calc_ultra-1.3.6/src/calc_ultra/__init__.py
+-rw-r--r--   0 Huatao     (502) staff       (20)    46616 2024-05-15 11:27:19.000000 calc_ultra-1.3.6/src/calc_ultra/main.py
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-15 12:23:00.160464 calc_ultra-1.3.6/src/calc_ultra/texts/
+-rw-r--r--   0 Huatao     (502) staff       (20)        0 2023-12-09 18:58:14.000000 calc_ultra-1.3.6/src/calc_ultra/texts/__init__.py
+-rw-r--r--   0 Huatao     (502) staff       (20)      546 2024-03-19 08:27:24.000000 calc_ultra-1.3.6/src/calc_ultra/texts/algcalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      740 2024-03-06 07:59:13.000000 calc_ultra-1.3.6/src/calc_ultra/texts/derivacalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      761 2024-04-14 10:36:05.000000 calc_ultra-1.3.6/src/calc_ultra/texts/intecalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      531 2024-03-06 07:59:34.000000 calc_ultra-1.3.6/src/calc_ultra/texts/limcalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      706 2024-05-01 04:38:23.000000 calc_ultra-1.3.6/src/calc_ultra/texts/main_screen.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      232 2024-04-14 10:37:09.000000 calc_ultra-1.3.6/src/calc_ultra/texts/settings.txt
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-15 12:23:00.160718 calc_ultra-1.3.6/src/calc_ultra.egg-info/
+-rw-r--r--   0 Huatao     (502) staff       (20)     4203 2024-05-15 12:23:00.000000 calc_ultra-1.3.6/src/calc_ultra.egg-info/PKG-INFO
+-rw-r--r--   0 Huatao     (502) staff       (20)      562 2024-05-15 12:23:00.000000 calc_ultra-1.3.6/src/calc_ultra.egg-info/SOURCES.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)        1 2024-05-15 12:23:00.000000 calc_ultra-1.3.6/src/calc_ultra.egg-info/dependency_links.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)       94 2024-05-15 12:23:00.000000 calc_ultra-1.3.6/src/calc_ultra.egg-info/requires.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)       11 2024-05-15 12:23:00.000000 calc_ultra-1.3.6/src/calc_ultra.egg-info/top_level.txt
```

### Comparing `calc_ultra-1.3.5/LICENSE` & `calc_ultra-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.5/PKG-INFO` & `calc_ultra-1.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calc_ultra
-Version: 1.3.5
+Version: 1.3.6
 Summary: A calculus calculator with a menu-based interface.
 Author-email: Huatao <huatao.xue@outlook.com>
 Maintainer-email: Huatao <huatao.xue@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/sudoer-Huatao/calc_ultra
 Project-URL: Issues, https://github.com/sudoer-Huatao/calc_ultra/issues
 Keywords: calculus,calculator
@@ -18,15 +18,15 @@
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: rich>=13.7.1
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: prompt_toolkit>=3.0.43
 
 # calc-ultra
 
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.5-blue.svg)](https://github.com/sudoer-Huatao/calc_ultra)
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.6-blue.svg)](https://github.com/sudoer-Huatao/calc_ultra)
 
 > **Calculus made easy**
 
 (Turn on dark mode for a better aesthetic) 📲
 
 Calc-Ultra is a multi-functional calculator that uses command line interfaces. Little Python background knowledge is needed to use the calculator!
 
@@ -64,28 +64,24 @@
 
 Please make sure you have the latest version installed. To update calc-ultra, run the following command:
 
 `pip3 install --upgrade calc-ultra`
 
 ## Requirements
 
-Calc-Ultra requires these modules/packages:
+Calc-Ultra requires these modules/packages to be installed:
 
 - `sympy`
 - `numpy`
 - `matplotlib`
 - `scipy`
 - `rich`
 - `prompt-toolkit`
 
-If you do not have them installed, there is no need to worry. The modules needed should be installed automatically if you don't have them. Other required modules are built into most Python IDEs as well.
-
-## Test PYPI
-
-Previous test versions of this project are on Test PYPI. View on <https://test.pypi.org/project/calc-ultra/>. 💾
+If you do not have them installed, no need to worry! These modules should be installed automatically if you don't have them. Other required modules are built into most Python IDEs as well.
 
 ## Acknowledgements
 
 > Without them, this would be impossible
 
 A big thank-you to all GitHub users who gave feedback and/or starred this repository. ⭐️ Your encouragement is our motivation.
 The following contributors deserve a SPECIAL THANK-YOU 👍❤️:
```

### Comparing `calc_ultra-1.3.5/README.md` & `calc_ultra-1.3.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # calc-ultra
 
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.5-blue.svg)](https://github.com/sudoer-Huatao/calc_ultra)
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.6-blue.svg)](https://github.com/sudoer-Huatao/calc_ultra)
 
 > **Calculus made easy**
 
 (Turn on dark mode for a better aesthetic) 📲
 
 Calc-Ultra is a multi-functional calculator that uses command line interfaces. Little Python background knowledge is needed to use the calculator!
 
@@ -42,28 +42,24 @@
 
 Please make sure you have the latest version installed. To update calc-ultra, run the following command:
 
 `pip3 install --upgrade calc-ultra`
 
 ## Requirements
 
-Calc-Ultra requires these modules/packages:
+Calc-Ultra requires these modules/packages to be installed:
 
 - `sympy`
 - `numpy`
 - `matplotlib`
 - `scipy`
 - `rich`
 - `prompt-toolkit`
 
-If you do not have them installed, there is no need to worry. The modules needed should be installed automatically if you don't have them. Other required modules are built into most Python IDEs as well.
-
-## Test PYPI
-
-Previous test versions of this project are on Test PYPI. View on <https://test.pypi.org/project/calc-ultra/>. 💾
+If you do not have them installed, no need to worry! These modules should be installed automatically if you don't have them. Other required modules are built into most Python IDEs as well.
 
 ## Acknowledgements
 
 > Without them, this would be impossible
 
 A big thank-you to all GitHub users who gave feedback and/or starred this repository. ⭐️ Your encouragement is our motivation.
 The following contributors deserve a SPECIAL THANK-YOU 👍❤️:
```

### Comparing `calc_ultra-1.3.5/pyproject.toml` & `calc_ultra-1.3.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [wheel]
 supported_platforms = ["macos"]
 
 [project]
 name = "calc_ultra"
-version = "1.3.5"
+version = "1.3.6"
 dependencies = [
   "sympy >= 1.12",
   "numpy >= 1.26.2",
   "matplotlib >= 3.8.4",
   "rich >= 13.7.1",
   "scipy >= 1.13.0",
   "prompt_toolkit >= 3.0.43"
```

### Comparing `calc_ultra-1.3.5/src/.DS_Store` & `calc_ultra-1.3.6/src/.DS_Store`

 * *Files 22% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 00000230: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
 00000240: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
 00000250: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
 00000260: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
 00000270: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
 00000280: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
 00000290: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
-000002a0: 1018 7b7b 3339 352c 2034 3734 7d2c 207b  ..{{395, 474}, {
-000002b0: 3932 302c 2034 3336 7d7d 0908 1523 2f3b  920, 436}}...#/;
+000002a0: 1018 7b7b 3433 302c 2034 3434 7d2c 207b  ..{{430, 444}, {
+000002b0: 3835 352c 2034 3339 7d7d 0908 1523 2f3b  855, 439}}...#/;
 000002c0: 525f 6b6c 6d6e 6f8a 0000 0000 0000 0101  R_klmno.........
 000002d0: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 000002e0: 0000 0000 0000 008b 0000 000a 0063 0061  .............c.a
 000002f0: 006c 0063 005f 0075 006c 0074 0072 0061  .l.c._.u.l.t.r.a
 00000300: 7653 726e 6c6f 6e67 0000 0001 0000 0000  vSrnlong........
 00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `calc_ultra-1.3.5/src/calc_ultra/.DS_Store` & `calc_ultra-1.3.6/src/calc_ultra/.DS_Store`

 * *Files 23% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 00000120: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
 00000130: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 00000140: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 00000150: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00000160: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00000170: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00000180: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00000190: 7208 0908 095f 1018 7b7b 3432 392c 2033  r...._..{{429, 3
-000001a0: 3432 7d2c 207b 3835 352c 2034 3339 7d7d  42}, {855, 439}}
+00000190: 7208 0908 095f 1018 7b7b 3436 382c 2032  r...._..{{468, 2
+000001a0: 3734 7d2c 207b 3835 352c 2034 3339 7d7d  74}, {855, 439}}
 000001b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
 000001c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
 000001e0: 0005 0074 0065 0078 0074 0073 7653 726e  ...t.e.x.t.svSrn
 000001f0: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `calc_ultra-1.3.5/src/calc_ultra/main.py` & `calc_ultra-1.3.6/src/calc_ultra/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 ###########
 # Imports #
 ###########
 
-from sympy.core.numbers import pi, E, oo
-from math import floor, ceil
-from scipy.special import polygamma, gammainc, gammaincc, erf, erfc
-import scipy.special as ss
+
 from rich import print
-from rich.progress import (
-    Progress,
-    SpinnerColumn,
-    BarColumn,
-    MofNCompleteColumn,
-    TimeElapsedColumn,
-    TextColumn,
+
+print(
+    "\n[bright_yellow]Initializing Calc-Ultra. Might take some time on first startup ...[/bright_yellow]"
 )
-from prompt_toolkit import prompt
-from prompt_toolkit.key_binding import KeyBindings
+
 from numpy import (
     linspace,
     exp,
     log,
     sqrt,
     abs,
     sin,
@@ -32,14 +24,15 @@
     sinh,
     cosh,
     tanh,
     arcsinh,
     arccosh,
     arctanh,
     array,
+    array_equal,
     cross,
 )
 from numpy.linalg import norm, det
 from sympy import (
     diff,
     idiff,
     Integral,
@@ -51,57 +44,69 @@
     simplify,
     symbols,
     gamma,
     lowergamma,
     uppergamma,
     zeta,
 )
+from scipy.special import polygamma, gammainc, gammaincc, erf, erfc
+from rich.progress import (
+    Progress,
+    SpinnerColumn,
+    BarColumn,
+    MofNCompleteColumn,
+    TimeElapsedColumn,
+    TextColumn,
+)
+from sympy.core.numbers import pi, E, oo, I
+from math import floor, ceil
+import scipy.special as ss
+from prompt_toolkit import prompt
+from prompt_toolkit.key_binding import KeyBindings
 import matplotlib.pyplot as plt
 import datetime, logging, random, readline, os, time, warnings
 
 
 ###########
 # Presets #
 ###########
 
 warnings.filterwarnings("ignore")
 
 readline.parse_and_bind("tab: complete")
 
-x, y, z = symbols("x, y, z")
+x, y, z, t, m = symbols("x, y, z, t, m")
 
-history = []  # Stores calculation history
+history = [""]  # Stores calculation history
 
 input = prompt
 
 key_bindings = KeyBindings()
 
 idx = 1
 
 expr_replace = [
     ("^", "**"),
     ("E1**", "exp"),
     ("E1xp", "exp"),
-    ("E1rf", "erf"),
-    ("pE1r", "per"),
-    ("wE1r", "wer"),
+    ("E1r", "er"),
+    ("sIn", "sin"),
+    ("pI", "pi"),
+    ("Ia", "ia"),
     ("ln", "log"),
     ("arc", "a"),
     ("abs", "Abs"),
     ("pi", "3.141592653589793"),
     ("E1", "2.718281828459045"),
 ]
 
 graph_replace = [
     ("asin", "arcsin"),
     ("acos", "arccos"),
     ("atan", "arctan"),
-    ("asinh", "arcsinh"),
-    ("acosh", "arccosh"),
-    ("atanh", "arctanh"),
     ("csc", "1/sin"),
     ("sec", "1/cos"),
     ("cot", "1/tan"),
     ("Abs", "fabs"),
     ("gamma", "ss.gamma"),
     ("polyss.gamma", "polygamma"),
     ("lowergamma", "gammainc"),
@@ -112,66 +117,160 @@
 # Custom up/down key bindings
 
 
 @key_bindings.add("up")
 def _(event):
     global idx
 
-    if idx != -1:
-        idx -= 1
-        buffer = event.app.current_buffer
-        buffer.text = history[idx]
-        buffer.cursor_position = len(buffer.text)
-        idx = idx % len(history)
-    else:
-        idx = 0
-        buffer = event.app.current_buffer
-        buffer.text = history[idx]
-        buffer.cursor_position = len(buffer.text)
+    try:
+        if idx != -1:
+            idx -= 1
+            buffer = event.app.current_buffer
+            buffer.text = history[idx]
+            buffer.cursor_position = len(buffer.text)
+            idx = idx % len(history)
+        else:
+            idx = 0
+            buffer = event.app.current_buffer
+            buffer.text = history[idx]
+            buffer.cursor_position = len(buffer.text)
+
+    except:
+        pass
 
 
 @key_bindings.add("down")
 def _(event):
     global idx
 
-    if idx != len(history):
-        idx += 1
-        idx = idx % len(history)
-        buffer = event.app.current_buffer
-        buffer.text = history[idx]
-        buffer.cursor_position = len(buffer.text)
+    try:
+        if idx != len(history):
+            idx += 1
+            idx = idx % len(history)
+            buffer = event.app.current_buffer
+            buffer.text = history[idx]
+            buffer.cursor_position = len(buffer.text)
+
+        else:
+            idx = len(history) - 1
+            buffer = event.app.current_buffer
+            buffer.text = history[idx]
+            buffer.cursor_position = len(buffer.text)
+
+    except:
+        pass
 
-    else:
-        idx = len(history) - 1
-        buffer = event.app.current_buffer
-        buffer.text = history[idx]
-        buffer.cursor_position = len(buffer.text)
+
+@key_bindings.add("c-c")
+def _(event):
+    history = [""]
 
 
 #####################
 # Calculation funcs #
 #####################
 
 
 def simp():
     print(
-        '\n[bold bright_green](Current Screen: Simple Calculation Screen)[/bold bright_green]\n("q" to quit)\nEnter any expression to start:\n'
+        '\n[bold bright_green](Current Screen: Simple Calculation Screen)[/bold bright_green]\n("q" to quit)\nEnter any expression:\n'
     )
 
     while True:
         expr = input(key_bindings=key_bindings)
 
         try:
             if expr != "q":
                 # Easy to exit unlike VIM ;)
-                result = eval(replace_graph(expr))
-                history.append(str(result))
-                print("\n[bright_yellow]Result:[/bright_yellow]", end="")
-                pprint(result)
-                print()
+                expr = expr.replace(" ", "")
+
+                if "?=" in expr:
+                    left = replace_graph(
+                        str(simplify(replace_expr(expr[: expr.find("?=")])).evalf())
+                    ).lstrip("0*x+")
+
+                    right = replace_graph(
+                        str(simplify(replace_expr(expr[expr.find("?=") + 2 :])).evalf())
+                    ).lstrip("0*x+")
+
+                    try:
+                        if "I" in left:
+                            left = left.replace(" ", "")
+                            imag = eval((left[left.find("+") + 1 :]).rstrip("*I"))
+
+                            if imag < 0.000001 and imag > -0.000001:
+                                left = left[: left.find("+")]
+
+                        elif left < 0.000001 and left > -0.000001:
+                            left = 0
+
+                        if "I" in right:
+                            right = right.replace(" ", "")
+                            imag = eval((right[right.find("+") + 1 :]).rstrip("*I"))
+
+                            if imag < 0.000001 and imag > -0.000001:
+                                right = right[: right.find("+")]
+
+                        elif right < 0.000001 and right > -0.000001:
+                            right = 0
+
+                    except:
+                        pass
+
+                    if str(left).endswith("0") and left != 0:
+                        left = str(left).rstrip("0")
+
+                    if str(right).endswith("0") and right != 0:
+                        right = str(right).rstrip("0")
+
+                    if "x" in left and "x" in right:
+                        equals = "True"
+
+                        for i in range(-100, 100):
+                            left_result = str(eval(left.replace("x", str(i))))
+                            right_result = str(eval(right.replace("x", str(i))))
+
+                            if left_result != right_result:
+                                equals = "False."
+                                break
+
+                        print("\n" + equals + "\n")
+
+                    else:
+                        print(left)
+                        print(right)
+                        if left == right:
+                            print("\nTrue.\n")
+                        else:
+                            print("\nFalse.\n")
+
+                else:
+                    result = simplify(replace_expr(expr)).evalf()
+
+                    try:
+                        if "I" in str(result):
+                            result = str(result).replace(" ", "")
+                            imag = eval((result[result.find("+") + 1 :]).rstrip("*I"))
+
+                            if imag < 0.000001 and imag > -0.000001:
+                                result = result[: result.find("+")]
+
+                        elif result < 0.000001 and result > -0.000001:
+                            result = 0
+
+                    except:
+                        pass
+
+                    if str(result).endswith("0") and result != 0:
+                        result = eval(str(result).rstrip("0"))
+
+                    history.append(str(result))
+                    print("\n[bright_yellow]Result: [/bright_yellow]", end="")
+                    pprint(result)
+                    print()
 
             else:
                 break
 
         except:
             print()
             logging.error(f'Could not parse: "{expr}".\n')
@@ -235,16 +334,22 @@
             plt.xlabel("x", weight="bold")
             plt.ylabel("y", rotation=0, weight="bold")
             plt.plot(x_arr, f(x_arr), color="red", label="Function")
             plt.plot(x_arr, dif(x_arr), color="blue", label="Derivative")
             plt.axis([-7.5, 7.5, -7.5, 7.5])
             plt.legend(loc="lower left")
             plt.grid()
-            plt.show()
 
+            download = input("Download graph? (y/n) ")
+
+            if download == "y":
+                plt.savefig(df + ".pdf")
+                print("\nDownloaded graph.")
+
+            plt.show()
             print("\nExited graph.\n")
 
         except:
             plt.close()
             print("\n")
             logging.warning("Could not graph function.")
             print("\nExited graph.")
@@ -357,16 +462,21 @@
             plt.title(title)
             plt.xlabel("x", weight="bold")
             plt.ylabel("y", rotation=0, weight="bold")
             plt.plot(x_arr, f(x_arr), color="red", label="Function")
             plt.plot(x_arr, af(x_arr), color="blue", label="Antiderivative")
             plt.axis([-7.5, 7.5, -7.5, 7.5])
             plt.legend(loc="lower left")
-
             plt.grid()
+            download = input("Download graph? (y/n) ")
+
+            if download == "y":
+                plt.savefig(df.replace("0 * x +", "") + ".pdf")
+                print("\nDownloaded graph.")
+
             plt.show()
 
             print("\nExited graph.\n")
 
         except:
             plt.close()
             print("\n")
@@ -519,14 +629,21 @@
                         )
 
             except:
                 plt.axis([-7.5, 7.5, -7.5, 7.5])
 
             plt.legend(loc="lower left")
             plt.grid()
+
+            download = input("Download graph? (y/n) ")
+
+            if download == "y":
+                plt.savefig(df.replace("0 * x +", "") + ".pdf")
+                print("\nDownloaded graph.")
+
             plt.show()
 
             return "\nExited graph.\n"
 
         except:
             plt.close()
             print("\n")
@@ -785,20 +902,24 @@
 def check_simp(expr: str) -> bool:
     """Check for simplification of an expression.
 
     Takes an expression and simplifies/rewrites it
     if possible. Otherwise returns boolean value False.
     """
 
-    if str(simplify(expr, evaluate=False)) != expr:
-        print("\nSimplify/rewrite:\n")
-        print_expr(simplify(expr, evaluate=False))
+    try:
+        if str(simplify(expr, evaluate=False)) != expr:
+            print("\nSimplify/rewrite:\n")
+            print_expr(simplify(expr, evaluate=False))
 
-    else:
-        return False
+        else:
+            return False
+
+    except:
+        pass
 
 
 def check_order(order: str):
     """Check if the order of differentiation is valid.
 
     Takes the order of differentiation and gives an error
     if it is invalid.
@@ -833,25 +954,28 @@
 
 def replace_expr(expr: str) -> str:
     """Sanatizes an expression from input.
 
     Takes a string and sanatizes input for calculation.
     """
 
-    expr = expr.strip(" ")
+    expr = expr.strip()
 
     # The extra 1 at the end is to recognize whether the "e"
     # is part of an expression or a constant on it's own.
 
     if "E" in expr:
         expr = expr.replace("E", "E1")
 
     if "e" in expr:
         expr = expr.replace("e", "E1")
 
+    if "i" in expr:
+        expr = expr.replace("i", "I")
+
     for r in expr_replace:
         expr = expr.replace(*r)
 
     return expr
 
 
 def replace_graph(function: str) -> str:
@@ -866,15 +990,15 @@
 
     if "log" in function and ",x)" in function:
         function = function.replace("log", "mt.log")
 
     # Graph constant functions
 
     if "x" not in function:
-        function = "0 * x + " + function
+        function = "0*x+" + function
 
     for r in graph_replace:
         function = function.replace(*r)
 
     return function
 
 
@@ -910,27 +1034,27 @@
 # Driving programs #
 ####################
 
 
 def main():
     with Progress(
         SpinnerColumn(finished_text="[bright_green]√[/bright_green]"),
-        TextColumn("[green]Handling imports[/green]..."),
+        TextColumn("[bright_green]Handling imports ...[/bright_green]"),
         BarColumn(),
         MofNCompleteColumn(),
         TimeElapsedColumn(),
         transient=False,
     ) as progress:
         task = progress.add_task("", total=50)
 
         while not progress.finished:
             progress.update(task, advance=1)
             time.sleep(random.randint(2, 5) / 100)
 
-    global x, y, z, history, expr_replace, graph_replace
+    global x, y, z, t, m, history, expr_replace, graph_replace
 
     while True:
         instruct_path = (
             os.path.dirname(os.path.abspath(__file__))
             + "/texts/main_screen.txt"
             # TODO: make the PATH compatible with Windows
         )
@@ -1048,15 +1172,15 @@
                 order = input(
                     "Enter order of implicit derivative calculation: ",
                     key_bindings=key_bindings,
                 )
                 implicit_derive(circ, order)
 
             elif cmd == "4":
-                print("\n[bright_yellow]Exiting DerivaCalc ... ... ...[/bright_yellow]")
+                print("\n[bright_yellow]Exiting DerivaCalc ...[/bright_yellow]")
                 break
 
             else:
                 print("\n")
                 logging.warning(f'Invalid command:"{cmd}"')
         except:
             print("\n")
@@ -1132,15 +1256,15 @@
                 )
                 inner_up = input(
                     "Enter the upper inner bound: ", key_bindings=key_bindings
                 )
                 double_int(function, outer_low, outer_up, inner_low, inner_up)
 
             elif cmd == "5":
-                print("\n[bright_yellow]Exiting InteCalc ... ... ...[/bright_yellow]")
+                print("\n[bright_yellow]Exiting InteCalc ...[/bright_yellow]")
                 break
 
             else:
                 print("\n")
                 logging.warning(f'Invalid command: "{cmd}"')
         except:
             print("\n")
@@ -1181,15 +1305,15 @@
                 )
                 expr = input("Enter an expression: ", key_bindings=key_bindings)
                 value = input("Enter point of evaluation: ", key_bindings=key_bindings)
                 direction = input("Enter direction of limit ('left' or 'right'): ")
                 side_lim(expr, value, direction)
 
             elif cmd == "3":
-                print("\n[bright_yellow]Exiting LimCalc ... ... ...[/bright_yellow]")
+                print("\n[bright_yellow]Exiting LimCalc ...[/bright_yellow]")
                 break
 
             else:
                 print("\n")
                 logging.warning(f'Invalid command: "{cmd}"')
 
         except:
@@ -1306,15 +1430,15 @@
                         else:
                             break
                     except:
                         print("\n")
                         logging.error(f'Could not parse: "{expr}"\n')
 
             elif cmd == "4":
-                print("\n[bright_yellow]Exiting AlgCalc ... ... ...[/bright_yellow]")
+                print("\n[bright_yellow]Exiting AlgCalc ...[/bright_yellow]")
                 break
 
             else:
                 print("\n")
                 logging.warning(f'Invalid command: "{cmd}"')
 
         except:
```

### Comparing `calc_ultra-1.3.5/src/calc_ultra/texts/algcalc.txt` & `calc_ultra-1.3.6/src/calc_ultra/texts/algcalc.txt`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.5/src/calc_ultra/texts/derivacalc.txt` & `calc_ultra-1.3.6/src/calc_ultra/texts/derivacalc.txt`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.5/src/calc_ultra/texts/intecalc.txt` & `calc_ultra-1.3.6/src/calc_ultra/texts/intecalc.txt`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.5/src/calc_ultra/texts/limcalc.txt` & `calc_ultra-1.3.6/src/calc_ultra/texts/limcalc.txt`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.5/src/calc_ultra/texts/main_screen.txt` & `calc_ultra-1.3.6/src/calc_ultra/texts/main_screen.txt`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.5/src/calc_ultra.egg-info/PKG-INFO` & `calc_ultra-1.3.6/src/calc_ultra.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calc_ultra
-Version: 1.3.5
+Version: 1.3.6
 Summary: A calculus calculator with a menu-based interface.
 Author-email: Huatao <huatao.xue@outlook.com>
 Maintainer-email: Huatao <huatao.xue@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/sudoer-Huatao/calc_ultra
 Project-URL: Issues, https://github.com/sudoer-Huatao/calc_ultra/issues
 Keywords: calculus,calculator
@@ -18,15 +18,15 @@
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: rich>=13.7.1
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: prompt_toolkit>=3.0.43
 
 # calc-ultra
 
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.5-blue.svg)](https://github.com/sudoer-Huatao/calc_ultra)
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.6-blue.svg)](https://github.com/sudoer-Huatao/calc_ultra)
 
 > **Calculus made easy**
 
 (Turn on dark mode for a better aesthetic) 📲
 
 Calc-Ultra is a multi-functional calculator that uses command line interfaces. Little Python background knowledge is needed to use the calculator!
 
@@ -64,28 +64,24 @@
 
 Please make sure you have the latest version installed. To update calc-ultra, run the following command:
 
 `pip3 install --upgrade calc-ultra`
 
 ## Requirements
 
-Calc-Ultra requires these modules/packages:
+Calc-Ultra requires these modules/packages to be installed:
 
 - `sympy`
 - `numpy`
 - `matplotlib`
 - `scipy`
 - `rich`
 - `prompt-toolkit`
 
-If you do not have them installed, there is no need to worry. The modules needed should be installed automatically if you don't have them. Other required modules are built into most Python IDEs as well.
-
-## Test PYPI
-
-Previous test versions of this project are on Test PYPI. View on <https://test.pypi.org/project/calc-ultra/>. 💾
+If you do not have them installed, no need to worry! These modules should be installed automatically if you don't have them. Other required modules are built into most Python IDEs as well.
 
 ## Acknowledgements
 
 > Without them, this would be impossible
 
 A big thank-you to all GitHub users who gave feedback and/or starred this repository. ⭐️ Your encouragement is our motivation.
 The following contributors deserve a SPECIAL THANK-YOU 👍❤️:
```

### Comparing `calc_ultra-1.3.5/src/calc_ultra.egg-info/SOURCES.txt` & `calc_ultra-1.3.6/src/calc_ultra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

