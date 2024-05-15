# Comparing `tmp/jax_tqdm-0.2.0.tar.gz` & `tmp/jax_tqdm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_tqdm-0.2.0.tar", max compression
+gzip compressed data, was "jax_tqdm-0.2.1.tar", max compression
```

## Comparing `jax_tqdm-0.2.0.tar` & `jax_tqdm-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-25 10:44:36.938920 jax_tqdm-0.2.0/LICENSE
--rw-r--r--   0        0        0     2832 2024-04-26 10:38:40.256768 jax_tqdm-0.2.0/README.md
--rw-r--r--   0        0        0       47 2023-11-21 19:48:26.044384 jax_tqdm-0.2.0/jax_tqdm/__init__.py
--rw-r--r--   0        0        0     4657 2024-04-25 10:44:36.938920 jax_tqdm-0.2.0/jax_tqdm/pbar.py
--rw-r--r--   0        0        0      850 2024-04-26 10:38:40.256768 jax_tqdm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 jax_tqdm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-25 10:44:36.938920 jax_tqdm-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2832 2024-04-26 10:38:40.256768 jax_tqdm-0.2.1/README.md
+-rw-r--r--   0        0        0       47 2023-11-21 19:48:26.044384 jax_tqdm-0.2.1/jax_tqdm/__init__.py
+-rw-r--r--   0        0        0     4718 2024-05-15 08:30:31.905662 jax_tqdm-0.2.1/jax_tqdm/pbar.py
+-rw-r--r--   0        0        0      850 2024-05-15 08:38:31.046907 jax_tqdm-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 jax_tqdm-0.2.1/PKG-INFO
```

### Comparing `jax_tqdm-0.2.0/LICENSE` & `jax_tqdm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_tqdm-0.2.0/README.md` & `jax_tqdm-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jax_tqdm-0.2.0/jax_tqdm/pbar.py` & `jax_tqdm-0.2.1/jax_tqdm/pbar.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,47 +127,47 @@
     remainder = n % print_rate
 
     def _define_tqdm(arg, transform):
         tqdm_bars[0] = tqdm(range(n), **kwargs)
         tqdm_bars[0].set_description(message, refresh=False)
 
     def _update_tqdm(arg, transform):
-        tqdm_bars[0].update(arg)
+        tqdm_bars[0].update(int(arg))
 
     def _update_progress_bar(iter_num):
         "Updates tqdm from a JAX scan or loop"
         _ = jax.lax.cond(
             iter_num == 0,
-            lambda _: callback(_define_tqdm, None, None),
+            lambda _: callback(_define_tqdm, None, None, ordered=True),
             lambda _: None,
             operand=None,
         )
 
         _ = jax.lax.cond(
             # update tqdm every multiple of `print_rate` except at the end
             (iter_num % print_rate == 0) & (iter_num != n - remainder),
-            lambda _: callback(_update_tqdm, print_rate, None),
+            lambda _: callback(_update_tqdm, print_rate, None, ordered=True),
             lambda _: None,
             operand=None,
         )
 
         _ = jax.lax.cond(
             # update tqdm by `remainder`
             iter_num == n - remainder,
-            lambda _: callback(_update_tqdm, remainder, None),
+            lambda _: callback(_update_tqdm, remainder, None, ordered=True),
             lambda _: None,
             operand=None,
         )
 
     def _close_tqdm(arg, transform):
         tqdm_bars[0].close()
 
     def close_tqdm(result, iter_num):
         _ = jax.lax.cond(
             iter_num == n - 1,
-            lambda _: callback(_close_tqdm, None, None),
+            lambda _: callback(_close_tqdm, None, None, ordered=True),
             lambda _: None,
             operand=None,
         )
         return result
 
     return _update_progress_bar, close_tqdm
```

### Comparing `jax_tqdm-0.2.0/pyproject.toml` & `jax_tqdm-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jax-tqdm"
-version = "0.2.0"
+version = "0.2.1"
 description = "Tqdm progress bar for JAX scans and loops"
 authors = [
     "Jeremie Coullon <jeremie.coullon@gmail.com>",
     "zombie-einstein <zombie-einstein@proton.me>"
 ]
 readme = "README.md"
 packages = [{include = "jax_tqdm"}]
```

### Comparing `jax_tqdm-0.2.0/PKG-INFO` & `jax_tqdm-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-tqdm
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tqdm progress bar for JAX scans and loops
 Home-page: https://github.com/jeremiecoullon/jax-tqdm
 License: MIT
 Keywords: jax,tqdm
 Author: Jeremie Coullon
 Author-email: jeremie.coullon@gmail.com
 Requires-Python: >=3.9,<4.0
```

