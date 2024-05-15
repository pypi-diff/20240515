# Comparing `tmp/nifty_ls-1.0.0rc3.tar.gz` & `tmp/nifty_ls-1.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifty_ls-1.0.0rc3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "nifty_ls-1.0.0rc5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `nifty_ls-1.0.0rc3.tar` & `nifty_ls-1.0.0rc5.tar`

### file list

```diff
@@ -1,26 +1,30 @@
--rw-r--r--   0        0        0      119 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/.github/dependabot.yaml
--rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1412 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/.github/workflows/wheels.yml
--rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/.gitignore
--rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      644 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/CMakeLists.txt
--rw-r--r--   0        0        0    11348 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/LICENSE
--rw-r--r--   0        0        0    15021 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/README.md
--rw-r--r--   0        0        0    53183 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/bench.png
--rw-r--r--   0        0        0    58451 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/bench_batch.png
--rw-r--r--   0        0        0      165 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/ci/Dockerfile
--rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/ci/Jenkinsfile
--rw-r--r--   0        0        0     1927 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0     7373 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/scripts/bench.py
--rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/src/nifty_ls/__init__.py
--rw-r--r--   0        0        0      901 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/src/nifty_ls/astropy.py
--rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/src/nifty_ls/backends.py
--rw-r--r--   0        0        0     4915 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/src/nifty_ls/core.py
--rw-r--r--   0        0        0     9281 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/src/nifty_ls/cpu_helpers.cpp
--rw-r--r--   0        0        0     7377 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/src/nifty_ls/cufinufft.py
--rw-r--r--   0        0        0     9295 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/src/nifty_ls/finufft.py
--rw-r--r--   0        0        0     1112 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/src/nifty_ls/test_helpers/utils.py
--rw-r--r--   0        0        0     1176 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/src/nifty_ls/utils.py
--rw-r--r--   0        0        0     6023 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/tests/test_ls.py
--rw-r--r--   0        0        0     3265 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/tests/test_perf.py
--rw-r--r--   0        0        0    28929 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      119 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/.github/dependabot.yaml
+-rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     2660 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       98 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/.gitignore
+-rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/CHANGES.md
+-rw-r--r--   0        0        0      765 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/CMakeLists.txt
+-rw-r--r--   0        0        0    11348 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/LICENSE
+-rw-r--r--   0        0        0    18068 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/README.md
+-rw-r--r--   0        0        0    27334 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/accuracy.png
+-rw-r--r--   0        0        0    53183 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/bench.png
+-rw-r--r--   0        0        0    58451 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/bench_batch.png
+-rw-r--r--   0        0        0      165 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/ci/Dockerfile
+-rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/ci/Jenkinsfile
+-rw-r--r--   0        0        0     2199 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     8306 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/scripts/bench.py
+-rw-r--r--   0        0        0     4081 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/scripts/compare.py
+-rw-r--r--   0        0        0     7395 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/scripts/sweep.py
+-rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/src/nifty_ls/__init__.py
+-rw-r--r--   0        0        0      901 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/src/nifty_ls/astropy.py
+-rw-r--r--   0        0        0      808 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/src/nifty_ls/backends.py
+-rw-r--r--   0        0        0     4917 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/src/nifty_ls/core.py
+-rw-r--r--   0        0        0    14474 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/src/nifty_ls/cpu_helpers.cpp
+-rw-r--r--   0        0        0     7380 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/src/nifty_ls/cufinufft.py
+-rw-r--r--   0        0        0     9811 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/src/nifty_ls/finufft.py
+-rw-r--r--   0        0        0     1112 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/src/nifty_ls/test_helpers/utils.py
+-rw-r--r--   0        0        0     1177 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/src/nifty_ls/utils.py
+-rw-r--r--   0        0        0     6023 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/tests/test_ls.py
+-rw-r--r--   0        0        0     3265 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/tests/test_perf.py
+-rw-r--r--   0        0        0    31976 2022-11-09 12:37:21.000000 nifty_ls-1.0.0rc5/PKG-INFO
```

### Comparing `nifty_ls-1.0.0rc3/.github/workflows/tests.yml` & `nifty_ls-1.0.0rc5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `nifty_ls-1.0.0rc3/CMakeLists.txt` & `nifty_ls-1.0.0rc5/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 cmake_minimum_required(VERSION 3.15...3.27)
 project(${SKBUILD_PROJECT_NAME} LANGUAGES CXX)
 
 find_package(Python 3.8 COMPONENTS Interpreter Development.Module REQUIRED)
 find_package(nanobind CONFIG REQUIRED)
-find_package(OpenMP)
+
+option(NIFTY_LS_OPENMP "Enable OpenMP support in the compiled extensions" ON)
+
+if(NIFTY_LS_OPENMP)
+    find_package(OpenMP REQUIRED)
+endif()
 
 nanobind_add_module(cpu_helpers src/nifty_ls/cpu_helpers.cpp NOMINSIZE)
 
 target_compile_options(cpu_helpers PRIVATE
     -Wall -Wextra -Werror -std=c++17
 )
```

### Comparing `nifty_ls-1.0.0rc3/LICENSE` & `nifty_ls-1.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `nifty_ls-1.0.0rc3/README.md` & `nifty_ls-1.0.0rc5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -93,21 +93,27 @@
 
 ### For best performance
 You may wish to compile and install finufft and cufinufft yourself so they will be
 built with optimizations for your hardware. To do so, first install nifty-ls, then
 follow the Python installation instructions for
 [finufft](https://finufft.readthedocs.io/en/latest/install.html#building-a-python-interface-to-a-locally-compiled-library)
 and
-[cufinufft](https://finufft.readthedocs.io/en/latest/install_gpu.html#python-interface)
-as desired.
+[cufinufft](https://finufft.readthedocs.io/en/latest/install_gpu.html#python-interface),
+configuring the libraries as desired.
 
 nifty-ls can likewise be built from source following the instructions above for
 best performance, but most of the heavy computations are offloaded to (cu)finufft,
 so the performance benefit is minimal.
 
+**⚠️ MacOS ARM users (M1/M2/etc)**: due to an OpenMP library incompatibility, the
+nifty-ls "C++ helpers" are not parallelized in the Mac ARM builds on PyPI. This is not
+expected to have a big impact on performance,as the core finufft computation will still
+be parallelized. Building both finufft and nifty-ls from source is a possible
+workaround.
+
 ## Usage
 ### From Astropy
 Importing `nifty_ls` makes nifty-ls available via `method="fastnifty"` in
 Astropy's LombScargle module. The name is prefixed with "fast" as it's part
 of the fast family of methods that assume a regularly-spaced frequency grid.
 
 ```python
@@ -180,15 +186,15 @@
 The code only supports frequency grids with fixed spacing; however, finufft does
 support type 3 NUFFTs (non-uniform to non-uniform), which would enable arbitrary
 frequency grids. It's not clear how useful this is, so it hasn't been implemented,
 but please open a GitHub issue if this is of interest to you.
 
 ## Performance
 
-Using 16 cores of an Intel Icelake CPU and a NVIDIA A100 GPU, we obtain the following performance. First, we'll look at the performance on a single periodogram (i.e. unbatched):
+Using 16 cores of an Intel Icelake CPU and a NVIDIA A100 GPU, we obtain the following performance. First, we'll look at results from a single periodogram (i.e. unbatched):
 
 ![benchmarks](bench.png)
 
 In this case, finufft is 5x faster (11x with threads) than Astropy for large transforms, and 2x faster for (very) small transforms.  Small transforms improve futher relative to Astropy with more frequency bins. (Dynamic multi-threaded dispatch of transforms is planned as a future feature which will especially benefit small $N$.)
 
 cufinufft is 200x faster than Astropy for large $N$! The performance plateaus towards small $N$, mostly due to the overhead of sending data to the GPU and fetching the result. (Concurrent job execution on the GPU is another planned feature, which will especially help small $N$.)
 
@@ -210,18 +216,33 @@
 by offloading the pre- and post-processing steps to compiled extensions. The extensions
 enable us to do much more processing element-wise, rather than array-wise. In other words,
 they enable "kernel fusion" (to borrow a term from GPU computing), increasing the compute
 density.
 
 
 ## Accuracy
-While we compared performance with Astropy's `fast` method, this isn't quite fair. nifty-ls is substantially more accurate than Astropy `fast`!
+While we compared performance with Astropy's `fast` method, this isn't quite fair. nifty-ls is much more accurate than Astropy `fast`!  Astropy `fast` uses Press & Rybicki's extirpolation approximation, trading accuracy for speed, but thanks to finufft, nifty-ls can have both.
+
+In the figure below, we plot the median periodogram error in circles and the 99th percentile error in triangles for astropy, finufft, and cufinufft for a range of $N$ (and default $N_F \approx 12N$).
+
+The astropy result is presented for two cases: a nominal case and a "worst case". Internally, astropy uses an FFT grid whose size is the next power of 2 above the target oversampling rate. Each jump to a new power of 2 typically yields an increase in accuracy. The "worst case", therefore, is the highest frequency that does not yield such a jump.
+
+![](accuracy.png)
+
+Errors of $\mathcal{O}(10\%)$ or greater are not uncommon with worst-case evaluations. Errors of $\mathcal{O}(1\%)$ or greater are common in typical evaluations. nifty-ls is conservatively 6 orders of magnitude more accurate.
+
+The reference result in the above figure comes from the "phase winding" method, which uses trigonometric identities to avoid expensive sin and cos evaluations. One can also use astropy's `fast` method as a reference with exact evaluation enabled via `use_fft=False`.  One finds the same result, but the phase winding is a few orders of magnitude faster (but still not competitive with finufft).
+
+To summarize, we see that nifty-ls is highly accurate while also giving high performance.
 
 
+### float32 vs float64
+While 32-bit floats provide a substantial speedup for finufft and cufinufft, we generally don't recommend their use for Lomb-Scargle. The reason is the challenging [condition number](https://en.wikipedia.org/wiki/Condition_number) of the problem.  The condition number is the response in the output to a small perturbation in the input—in other words, the derivative. [It can easily be shown](https://finufft.readthedocs.io/en/latest/trouble.html) that the derivative of a NUFFT with respect to the non-uniform points is proportional to $N$, the transform length (i.e. the number of modes). In other words, errors in the observation times are amplified by $\mathcal{O}(N)$.  Since float32 has a relative error of $\mathcal{O}(10^{-7})$, transforms of length $10^5$ already suffer $\mathcal{O}(1\%)$ error. Therefore, we focus on float64 in nifty-ls, but float32 is also natively supported by all backends for adventurous users.
 
+The condition number is also a likely contributor to the mild upward trend in error versus $N$ in the above figure, at least for finufft/cufinufft. With a relative error of $\mathcal{O}(10^{-16})$ for float64 and a transform length of $\mathcal{O}(10^{6})$, the minimum error is $\mathcal{O}(10^{-10})$.
 
 ## Testing
 First, install from source (`pip install .[test]`). Then, from the repo root, run:
 
 ```console
 $ pytest
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nifty_ls-1.0.0rc3/bench.png` & `nifty_ls-1.0.0rc5/bench.png`

 * *Files identical despite different names*

### Comparing `nifty_ls-1.0.0rc3/bench_batch.png` & `nifty_ls-1.0.0rc5/bench_batch.png`

 * *Files identical despite different names*

### Comparing `nifty_ls-1.0.0rc3/ci/Jenkinsfile` & `nifty_ls-1.0.0rc5/ci/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `nifty_ls-1.0.0rc3/pyproject.toml` & `nifty_ls-1.0.0rc5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -48,17 +48,23 @@
 
 [tool.ruff.format]
 quote-style = "single"
 docstring-code-format = true
 
 [tool.cibuildwheel]
 archs = "auto64"
-test-command = "pytest --benchmark-skip {project}/tests"
+test-command = "pytest -s --benchmark-skip {project}/tests"
 test-extras = "test"
 skip = "pp* *-musllinux_*"
 
 [tool.cibuildwheel.linux]
 repair-wheel-command = [
   "auditwheel repair -w {dest_dir} {wheel}",
   # run abi3audit on wheels tagged with abi3
-  'case "$(basename {wheel})" in *"-abi3-"*) pipx run abi3audit --strict --report {wheel};; esac',
+  'case "$(basename {wheel})" in *"-abi3-"*) pip install -U abi3audit && abi3audit --strict --report {wheel};; esac',
+]
+
+[tool.cibuildwheel.macos]
+repair-wheel-command = [
+  'delocate-wheel --require-archs {delocate_archs} -w {dest_dir} -v {wheel}',
+  'case "$(basename {wheel})" in *"-abi3-"*) pip install -U abi3audit && abi3audit --strict --report {wheel};; esac',
 ]
```

### Comparing `nifty_ls-1.0.0rc3/scripts/bench.py` & `nifty_ls-1.0.0rc5/scripts/bench.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pathlib import Path
-import os
 
 import matplotlib
 
 matplotlib.use('Agg')
 
 import nifty_ls.finufft
 
@@ -19,43 +18,112 @@
 import astropy.timeseries.periodograms.lombscargle.implementations.fast_impl as astropy_impl
 
 # The Gowanlock+ paper uses N_t=3554 as their single-object dataset.
 DEFAULT_N = 3554
 DEFAULT_NF = None  # 10**5
 DEFAULT_DTYPE = 'f8'
 DEFAULT_METHODS = ['cufinufft', 'finufft', 'astropy', 'finufft_par']
-NTHREAD_MAX = len(os.sched_getaffinity(0))
+NTHREAD_MAX = nifty_ls.utils.get_avail_cpus()
 DEFAULT_FFTW = nifty_ls.finufft.FFTW_MEASURE
+DEFAULT_EPS = 1e-9
 
 
 def do_nifty_finufft(*args, **kwargs):
-    return nifty_ls.finufft.lombscargle(*args, **kwargs, finufft_kwargs=DEFAULT_FFTW)
+    return nifty_ls.finufft.lombscargle(
+        *args, **kwargs, finufft_kwargs={'fftw': DEFAULT_FFTW, 'eps': DEFAULT_EPS}
+    )
 
 
 def do_nifty_cufinufft(*args, **kwargs):
-    return nifty_ls.cufinufft.lombscargle(*args, **kwargs)
+    return nifty_ls.cufinufft.lombscargle(
+        *args, **kwargs, cufinufft_kwargs={'eps': DEFAULT_EPS}
+    )
 
 
-def do_astropy(t, y, dy, fmin, df, Nf):
+def do_astropy(t, y, dy, fmin, df, Nf, **astropy_kwargs):
     f0 = fmin
     y = np.atleast_2d(y)
     dy = np.atleast_2d(dy)
     for i in range(y.shape[0]):
-        power = astropy_impl.lombscargle_fast(t, y[i], dy=dy[i], f0=f0, df=df, Nf=Nf)
+        power = astropy_impl.lombscargle_fast(
+            t, y[i], dy=dy[i], f0=f0, df=df, Nf=Nf, **astropy_kwargs
+        )
     return power  # just last power for now
 
 
+def do_winding(t, y, dy, fmin, df, Nf, center_data=True, fit_mean=True, **kwargs):
+    power = np.empty(Nf, dtype=np.float64)
+    nifty_ls.cpu_helpers.compute_winding(
+        power, t, y, dy, fmin, df, center_data, fit_mean, **kwargs
+    )
+    return power
+
+
 METHODS = {
     'finufft_par': do_nifty_finufft,
     'finufft': lambda *args, **kwargs: do_nifty_finufft(*args, **kwargs, nthreads=1),
     'cufinufft': do_nifty_cufinufft,
     'astropy': do_astropy,
+    'astropy_brute': lambda *args, **kwargs: do_astropy(*args, **kwargs, use_fft=False),
+    'winding': do_winding,
 }
 
 
+def run_one(
+    method,
+    N,
+    Nf,
+    dtype,
+    batch_size=1,
+    seed=5043,
+    squeeze=False,
+    fmax=None,
+    time=True,
+    **kwargs,
+):
+    dtype = np.dtype(dtype).type
+    rng = np.random.default_rng(seed)
+
+    # Generate fake data
+    t = np.sort(rng.uniform(0, 2 * np.pi, N).astype(dtype)) * 1000
+    y = np.sin(t * rng.uniform(0.1, 10, batch_size).reshape(-1, 1)).astype(dtype)
+    dy = rng.normal(size=(batch_size, N)).astype(dtype)
+
+    if squeeze and batch_size == 1:
+        y = y[0]
+        dy = dy[0]
+
+    f0, df, Nf = nifty_ls.utils.validate_frequency_grid(None, fmax, Nf, t)
+
+    def func():
+        return METHODS[method](t, y, dy, f0, df, Nf, **kwargs)
+
+    res = {
+        'method': method,
+        'Nf': Nf,
+        'dtype': dtype.__name__,
+        'f0': f0,
+        'df': df,
+        'N': N,
+    }
+
+    # warmup, and get result
+    t1 = -timeit.default_timer()
+    res['power'] = func()
+    t1 += timeit.default_timer()
+    res['firsttime'] = t1
+
+    if time:
+        nrep, tot_time = timeit.Timer(func).autorange()
+        t = tot_time / nrep
+        res['time'] = t
+
+    return res
+
+
 def get_plot_kwargs(method, nthread_max=NTHREAD_MAX):
     if method == 'finufft_par':
         label = (
             'nifty-ls (finufft)'
             if nthread_max == 1
             else 'nifty-ls (finufft, multi-threaded)'
         )
@@ -69,14 +137,18 @@
         label = 'nifty-ls (cufinufft)'
         color = 'C2'
         ls = '-'
     elif method == 'astropy':
         label = r'astropy (${\tt fast}$ method)'
         color = 'C0'
         ls = '-'
+    elif method == 'astropy_worst':
+        label = r'astropy (worst case)'
+        color = 'C0'
+        ls = '--'
     else:
         label = method
         color = 'C3'
         ls = '-'
 
     return {'label': label, 'color': color, 'ls': ls}
 
@@ -142,45 +214,17 @@
             if sweep == 'Nf':
                 Nf = V
                 N = DEFAULT_N
             elif sweep == 'N':
                 N = V
                 Nf = DEFAULT_NF
 
-            rng = np.random.default_rng(5043)
-
-            # Generate fake data
-            t = np.sort(rng.uniform(0, 2 * np.pi, N).astype(dtype)) * 1000
-            y = np.sin(t * rng.uniform(0.1, 10, batch_size).reshape(-1, 1)).astype(
-                dtype
-            )
-            dy = rng.normal(size=(batch_size, N)).astype(dtype)
-
-            f0, df, Nf = nifty_ls.utils.validate_frequency_grid(None, None, Nf, t)
-
-            res = {
-                'method': method,
-                'Nf': Nf,
-                'dtype': dtype.__name__,
-                'f0': f0,
-                'df': df,
-                'N': N,
-            }
-
-            # warmup, and get result
-            def func():
-                return METHODS[method](t, y, dy, f0, df, Nf)
-
-            res['power'] = func()
-
-            nrep, tot_time = timeit.Timer(func).autorange()
-            time = tot_time / nrep
-            res['time'] = time
+            res = run_one(method, N, Nf, dtype, batch_size=batch_size)
 
-            print(f'{method} took {time:.4g} sec ({Nf=})')
+            print(f'{method} took {res["time"]:.4g} sec ({Nf=})')
             all_res.append(res)
 
     all_res = Table(
         all_res,
         meta={
             'sweep': sweep,
             'nthread_max': NTHREAD_MAX,
```

### Comparing `nifty_ls-1.0.0rc3/src/nifty_ls/__init__.py` & `nifty_ls-1.0.0rc5/src/nifty_ls/__init__.py`

 * *Files identical despite different names*

### Comparing `nifty_ls-1.0.0rc3/src/nifty_ls/astropy.py` & `nifty_ls-1.0.0rc5/src/nifty_ls/astropy.py`

 * *Files identical despite different names*

### Comparing `nifty_ls-1.0.0rc3/src/nifty_ls/backends.py` & `nifty_ls-1.0.0rc5/src/nifty_ls/backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 
     for backend in BACKEND_NAMES:
         try:
             # from . import backend
             import_module(f'.{backend}', __package__)
         except ImportError as e:
             if verbose:
-                print(f'Backend {backend} is unavailable: {e}')
+                print(f'[nifty-ls] Backend {backend} is unavailable: {e}')
         else:
             backends.append(backend)
 
     return backends
```

### Comparing `nifty_ls-1.0.0rc3/src/nifty_ls/core.py` & `nifty_ls-1.0.0rc5/src/nifty_ls/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ) -> dict:
     """
     Compute a Lomb-Scargle periodogram, or a batch of periodograms if `y` and `dy` are 2D arrays.
 
     This function can dispatch to multiple backends, including 'finufft' and 'cufinufft'. The latter
     uses CUDA and requires that nifty-ls was installed with the 'cuda' extra.
 
-    The result is a dictionary containing the computed periodograms, as well as the frequency grid parameters.
+    The result is a dictionary containing the computed periodogram(s), as well as the frequency grid parameters.
     The actual frequency grid can be obtained by passing the result dict to `lombscargle_freq()`.
 
     The meanings of these parameters conform to the Lomb-Scargle implementation in Astropy:
     https://docs.astropy.org/en/stable/timeseries/lombscargle.html
 
     Parameters
     ----------
```

### Comparing `nifty_ls-1.0.0rc3/src/nifty_ls/cufinufft.py` & `nifty_ls-1.0.0rc5/src/nifty_ls/cufinufft.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,12 +245,12 @@
 
     if copy_result_to_host:
         t_copy -= timer()
         power = power.get()
         t_copy += timer()
 
     if verbose:
-        print(f'nifty-ls cufinufft: HtoD + DtoH = {t_copy:.4g} sec')
-        print(f'nifty-ls cufinufft: pre/post = {t_prepost:.4g} sec')
-        print(f'nifty-ls cufinufft: cufinufft = {t_cufinufft:.4g} sec')
+        print(f'[nifty-ls cufinufft] HtoD + DtoH = {t_copy:.4g} sec')
+        print(f'[nifty-ls cufinufft] pre/post = {t_prepost:.4g} sec')
+        print(f'[nifty-ls cufinufft] cufinufft = {t_cufinufft:.4g} sec')
 
     return power
```

### Comparing `nifty_ls-1.0.0rc3/src/nifty_ls/finufft.py` & `nifty_ls-1.0.0rc5/src/nifty_ls/finufft.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from __future__ import annotations
 
-import os
+__all__ = ['lombscargle', 'FFTW_MEASURE', 'FFTW_ESTIMATE']
+
 from timeit import default_timer as timer
 
 import finufft
 import numpy as np
 
 from . import cpu_helpers
 
 FFTW_MEASURE = 0
 FFTW_ESTIMATE = 64
 
-MAX_THREADS = len(os.sched_getaffinity(0))
-
-__all__ = ['lombscargle', 'FFTW_MEASURE', 'FFTW_ESTIMATE', 'MAX_THREADS']
-
 
 def lombscargle(
     t,
     y,
     dy,
     fmin,
     df,
@@ -59,15 +56,15 @@
         The minimum frequency of the periodogram.
     df : float
         The frequency bin width.
     Nf : int
         The number of frequency bins.
     nthreads : int, optional
         The number of threads to use. The default behavior is to use (N_t / 4) * (Nf / 2^15) threads,
-        capped to the number of available CPUs. This is a heuristic that may not work well in all cases.
+        capped to the maximum number of OpenMP threads. This is a heuristic that may not work well in all cases.
     center_data : bool, optional
         Whether to center the data before computing the periodogram. Default is True.
     fit_mean : bool, optional
         Whether to fit a mean value to the data before computing the periodogram. Default is True.
     normalization : str, optional
         The normalization method to use. One of ['standard', 'model', 'log', 'psd']. Default is 'standard'.
     _no_cpp_helpers : bool, optional
@@ -112,25 +109,30 @@
 
     # If fit_mean, we need to transform (t,yw) and (t,w),
     # so we stack yw and w into a single array to allow a batched transform.
     # Regardless, we need to do a separate (t2,w2) transform.
     Nbatch, N = y.shape
 
     if nthreads is None:
+        # This heuristic feels fragile, it would be much better if finufft could do this upstream!
         nthreads = max(1, Nbatch // 4) * max(1, Nf // (1 << 15))
-        nthreads = min(nthreads, MAX_THREADS)
+        # Using get_finufft_max_threads() is safe because finufft never calls omp_set_num_threads()
+        nthreads = min(nthreads, get_finufft_max_threads())
+        # finufft (and cpu_helpers) will warn if the user exceeds omp_get_max_threads()
 
     if verbose:
         print(
-            f'nifty-ls finufft: Using {nthreads} {"thread" if nthreads == 1 else "threads"}'
+            f'[nifty-ls finufft] Using {nthreads} {"thread" if nthreads == 1 else "threads"}'
         )
 
-    # could probably be more than finufft nthreads in many cases,
+    # Could probably be more than finufft nthreads in many cases,
     # but it's conceptually cleaner to keep them the same, and it
-    # will almost never matter in practice
+    # will almost never matter in practice.
+    # Technically, this is also suboptimal in the rare case of a finufft
+    # library without OpenMP and a nifty-ls with OpenMP
     nthreads_helpers = nthreads
 
     if fit_mean:
         yw_w_shape = (2 * Nbatch, N)
     else:
         yw_w_shape = (Nbatch, N)
 
@@ -294,13 +296,20 @@
         else:
             raise ValueError(f'Unknown normalization: {normalization}')
 
     t_helpers += timer()
 
     if verbose:
         print(
-            f'nifty-ls finufft: FINUFFT took {t_finufft:.4g} sec, pre-/post-processing took {t_helpers:.4g} sec'
+            f'[nifty-ls finufft] FINUFFT took {t_finufft:.4g} sec, pre-/post-processing took {t_helpers:.4g} sec'
         )
 
     if squeeze_output:
         power = power.squeeze()
     return power
+
+
+def get_finufft_max_threads():
+    try:
+        return finufft._finufft.lib.omp_get_max_threads()
+    except AttributeError:
+        return 1
```

### Comparing `nifty_ls-1.0.0rc3/src/nifty_ls/test_helpers/utils.py` & `nifty_ls-1.0.0rc5/src/nifty_ls/test_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `nifty_ls-1.0.0rc3/src/nifty_ls/utils.py` & `nifty_ls-1.0.0rc5/src/nifty_ls/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+
 import numpy as np
 
 __all__ = ['validate_frequency_grid']
 
 
 def validate_frequency_grid(
     fmin, fmax, Nf, t, assume_sorted_t=True, samples_per_peak=5, nyquist_factor=5
```

### Comparing `nifty_ls-1.0.0rc3/tests/test_ls.py` & `nifty_ls-1.0.0rc5/tests/test_ls.py`

 * *Files identical despite different names*

### Comparing `nifty_ls-1.0.0rc3/tests/test_perf.py` & `nifty_ls-1.0.0rc5/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `nifty_ls-1.0.0rc3/PKG-INFO` & `nifty_ls-1.0.0rc5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifty-ls
-Version: 1.0.0rc3
+Version: 1.0.0rc5
 Summary: A fast Lomb-Scargle periodogram. It's nifty, and uses a NUFFT.
 Author: Dan Foreman-Mackey
 Author-Email: Lehman Garrison <lgarrison@flatironinstitute.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -321,21 +321,27 @@
 
 ### For best performance
 You may wish to compile and install finufft and cufinufft yourself so they will be
 built with optimizations for your hardware. To do so, first install nifty-ls, then
 follow the Python installation instructions for
 [finufft](https://finufft.readthedocs.io/en/latest/install.html#building-a-python-interface-to-a-locally-compiled-library)
 and
-[cufinufft](https://finufft.readthedocs.io/en/latest/install_gpu.html#python-interface)
-as desired.
+[cufinufft](https://finufft.readthedocs.io/en/latest/install_gpu.html#python-interface),
+configuring the libraries as desired.
 
 nifty-ls can likewise be built from source following the instructions above for
 best performance, but most of the heavy computations are offloaded to (cu)finufft,
 so the performance benefit is minimal.
 
+**⚠️ MacOS ARM users (M1/M2/etc)**: due to an OpenMP library incompatibility, the
+nifty-ls "C++ helpers" are not parallelized in the Mac ARM builds on PyPI. This is not
+expected to have a big impact on performance,as the core finufft computation will still
+be parallelized. Building both finufft and nifty-ls from source is a possible
+workaround.
+
 ## Usage
 ### From Astropy
 Importing `nifty_ls` makes nifty-ls available via `method="fastnifty"` in
 Astropy's LombScargle module. The name is prefixed with "fast" as it's part
 of the fast family of methods that assume a regularly-spaced frequency grid.
 
 ```python
@@ -408,15 +414,15 @@
 The code only supports frequency grids with fixed spacing; however, finufft does
 support type 3 NUFFTs (non-uniform to non-uniform), which would enable arbitrary
 frequency grids. It's not clear how useful this is, so it hasn't been implemented,
 but please open a GitHub issue if this is of interest to you.
 
 ## Performance
 
-Using 16 cores of an Intel Icelake CPU and a NVIDIA A100 GPU, we obtain the following performance. First, we'll look at the performance on a single periodogram (i.e. unbatched):
+Using 16 cores of an Intel Icelake CPU and a NVIDIA A100 GPU, we obtain the following performance. First, we'll look at results from a single periodogram (i.e. unbatched):
 
 ![benchmarks](bench.png)
 
 In this case, finufft is 5x faster (11x with threads) than Astropy for large transforms, and 2x faster for (very) small transforms.  Small transforms improve futher relative to Astropy with more frequency bins. (Dynamic multi-threaded dispatch of transforms is planned as a future feature which will especially benefit small $N$.)
 
 cufinufft is 200x faster than Astropy for large $N$! The performance plateaus towards small $N$, mostly due to the overhead of sending data to the GPU and fetching the result. (Concurrent job execution on the GPU is another planned feature, which will especially help small $N$.)
 
@@ -438,18 +444,33 @@
 by offloading the pre- and post-processing steps to compiled extensions. The extensions
 enable us to do much more processing element-wise, rather than array-wise. In other words,
 they enable "kernel fusion" (to borrow a term from GPU computing), increasing the compute
 density.
 
 
 ## Accuracy
-While we compared performance with Astropy's `fast` method, this isn't quite fair. nifty-ls is substantially more accurate than Astropy `fast`!
+While we compared performance with Astropy's `fast` method, this isn't quite fair. nifty-ls is much more accurate than Astropy `fast`!  Astropy `fast` uses Press & Rybicki's extirpolation approximation, trading accuracy for speed, but thanks to finufft, nifty-ls can have both.
+
+In the figure below, we plot the median periodogram error in circles and the 99th percentile error in triangles for astropy, finufft, and cufinufft for a range of $N$ (and default $N_F \approx 12N$).
+
+The astropy result is presented for two cases: a nominal case and a "worst case". Internally, astropy uses an FFT grid whose size is the next power of 2 above the target oversampling rate. Each jump to a new power of 2 typically yields an increase in accuracy. The "worst case", therefore, is the highest frequency that does not yield such a jump.
+
+![](accuracy.png)
+
+Errors of $\mathcal{O}(10\%)$ or greater are not uncommon with worst-case evaluations. Errors of $\mathcal{O}(1\%)$ or greater are common in typical evaluations. nifty-ls is conservatively 6 orders of magnitude more accurate.
+
+The reference result in the above figure comes from the "phase winding" method, which uses trigonometric identities to avoid expensive sin and cos evaluations. One can also use astropy's `fast` method as a reference with exact evaluation enabled via `use_fft=False`.  One finds the same result, but the phase winding is a few orders of magnitude faster (but still not competitive with finufft).
+
+To summarize, we see that nifty-ls is highly accurate while also giving high performance.
 
 
+### float32 vs float64
+While 32-bit floats provide a substantial speedup for finufft and cufinufft, we generally don't recommend their use for Lomb-Scargle. The reason is the challenging [condition number](https://en.wikipedia.org/wiki/Condition_number) of the problem.  The condition number is the response in the output to a small perturbation in the input—in other words, the derivative. [It can easily be shown](https://finufft.readthedocs.io/en/latest/trouble.html) that the derivative of a NUFFT with respect to the non-uniform points is proportional to $N$, the transform length (i.e. the number of modes). In other words, errors in the observation times are amplified by $\mathcal{O}(N)$.  Since float32 has a relative error of $\mathcal{O}(10^{-7})$, transforms of length $10^5$ already suffer $\mathcal{O}(1\%)$ error. Therefore, we focus on float64 in nifty-ls, but float32 is also natively supported by all backends for adventurous users.
 
+The condition number is also a likely contributor to the mild upward trend in error versus $N$ in the above figure, at least for finufft/cufinufft. With a relative error of $\mathcal{O}(10^{-16})$ for float64 and a transform length of $\mathcal{O}(10^{6})$, the minimum error is $\mathcal{O}(10^{-10})$.
 
 ## Testing
 First, install from source (`pip install .[test]`). Then, from the repo root, run:
 
 ```console
 $ pytest
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

