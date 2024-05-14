# Comparing `tmp/dansplotcore-6.4.0.tar.gz` & `tmp/dansplotcore-6.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dansplotcore-6.4.0.tar", last modified: Tue May 14 19:12:35 2024, max compression
+gzip compressed data, was "dansplotcore-6.4.1.tar", last modified: Tue May 14 19:18:10 2024, max compression
```

## Comparing `dansplotcore-6.4.0.tar` & `dansplotcore-6.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-14 19:12:35.643064 dansplotcore-6.4.0/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-14 19:12:35.643064 dansplotcore-6.4.0/PKG-INFO
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-14 19:12:35.643064 dansplotcore-6.4.0/dansplotcore/
--rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.4.0/dansplotcore/__init__.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.4.0/dansplotcore/media.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9713 2024-05-13 23:40:36.000000 dansplotcore-6.4.0/dansplotcore/plot.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.4.0/dansplotcore/primitives.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2208 2024-05-14 19:02:20.000000 dansplotcore-6.4.0/dansplotcore/process.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9612 2024-05-13 23:31:06.000000 dansplotcore-6.4.0/dansplotcore/show.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.4.0/dansplotcore/transforms.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.4.0/dansplotcore/vector_text.py
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-14 19:12:35.643064 dansplotcore-6.4.0/dansplotcore.egg-info/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-14 19:12:35.000000 dansplotcore-6.4.0/dansplotcore.egg-info/PKG-INFO
--rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-05-14 19:12:35.000000 dansplotcore-6.4.0/dansplotcore.egg-info/SOURCES.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-05-14 19:12:35.000000 dansplotcore-6.4.0/dansplotcore.egg-info/dependency_links.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-05-14 19:12:35.000000 dansplotcore-6.4.0/dansplotcore.egg-info/requires.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-05-14 19:12:35.000000 dansplotcore-6.4.0/dansplotcore.egg-info/top_level.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-05-14 19:12:35.643064 dansplotcore-6.4.0/setup.cfg
--rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-05-14 19:12:14.000000 dansplotcore-6.4.0/setup.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-14 19:18:10.908516 dansplotcore-6.4.1/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-14 19:18:10.908516 dansplotcore-6.4.1/PKG-INFO
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-14 19:18:10.904516 dansplotcore-6.4.1/dansplotcore/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.4.1/dansplotcore/__init__.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.4.1/dansplotcore/media.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9713 2024-05-13 23:40:36.000000 dansplotcore-6.4.1/dansplotcore/plot.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.4.1/dansplotcore/primitives.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2234 2024-05-14 19:17:01.000000 dansplotcore-6.4.1/dansplotcore/process.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9612 2024-05-13 23:31:06.000000 dansplotcore-6.4.1/dansplotcore/show.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.4.1/dansplotcore/transforms.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.4.1/dansplotcore/vector_text.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-14 19:18:10.908516 dansplotcore-6.4.1/dansplotcore.egg-info/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-14 19:18:10.000000 dansplotcore-6.4.1/dansplotcore.egg-info/PKG-INFO
+-rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-05-14 19:18:10.000000 dansplotcore-6.4.1/dansplotcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-05-14 19:18:10.000000 dansplotcore-6.4.1/dansplotcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-05-14 19:18:10.000000 dansplotcore-6.4.1/dansplotcore.egg-info/requires.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-05-14 19:18:10.000000 dansplotcore-6.4.1/dansplotcore.egg-info/top_level.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-05-14 19:18:10.908516 dansplotcore-6.4.1/setup.cfg
+-rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-05-14 19:17:40.000000 dansplotcore-6.4.1/setup.py
```

### Comparing `dansplotcore-6.4.0/dansplotcore/media.py` & `dansplotcore-6.4.1/dansplotcore/media.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.4.0/dansplotcore/plot.py` & `dansplotcore-6.4.1/dansplotcore/plot.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.4.0/dansplotcore/primitives.py` & `dansplotcore-6.4.1/dansplotcore/primitives.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.4.0/dansplotcore/process.py` & `dansplotcore-6.4.1/dansplotcore/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     bucket_size = data_range / bucket_count * 1.001
     buckets = [0 for _ in range(bucket_count)]
     for i in l:
         index = math.floor((i - data_min) / bucket_size)
         buckets[index] += 1
     return [(data_min + i * bucket_size, v) for i, v in enumerate(buckets)]
 
-def contours(points, *, n=5, ticks=1000, spread=50, plot=None):
+def contours(points, *, n=5, ticks=1000, spread=100, plot=None):
     '''
     Take in a list of (x, y) points and spit out a list of (x, *y_avg_i) for i in [0, n).
     A window is slid from min(x) to max(x) and at each spot, n trimmed averages are taken.
     y_avg_0 is the minimum value in the window.
     y_avg_m is the average of the window for odd n, m = (n-1)/2
     y_avg_h is the high-half trimmed average of the window, h ~= n * 3 / 4
     y_avg_M is the maximum value in the window, M = n-1
@@ -33,15 +33,15 @@
     x_min = min(i[0] for i in points)
     x_max = max(i[0] for i in points)
     x_range = x_max - x_min
     x_scale = x_range / ticks
     x_spread = x_scale * spread / 2
     lines = []
     for tick in range(ticks):
-        x = tick * x_scale
+        x = x_min + tick * x_scale
         window_min = x - x_spread
         window_max = x + x_spread
         bucket = sorted(y for (x, y) in points if window_min <= x < window_max)
         if not bucket: continue
         avgs = []
         for i in range(0, n):
             a = int((len(bucket) - 1) * (i / (n-1) * 2 - 1))
@@ -51,7 +51,8 @@
             avgs.append(avg(bucket[a:b]))
         lines.append((x, *avgs))
     if plot:
         for (xi, *yi), (xf, *yf) in zip(lines, lines[1:]):
             for i in range(n):
                 m = (n-1) / 2
                 plot.line(xi, yi[i], xf, yf[i], r=0, g=1 - abs(i - m) / m)
+    return lines
```

### Comparing `dansplotcore-6.4.0/dansplotcore/show.py` & `dansplotcore-6.4.1/dansplotcore/show.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.4.0/dansplotcore/transforms.py` & `dansplotcore-6.4.1/dansplotcore/transforms.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.4.0/dansplotcore/vector_text.py` & `dansplotcore-6.4.1/dansplotcore/vector_text.py`

 * *Files identical despite different names*

