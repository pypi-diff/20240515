# Comparing `tmp/PySDKit-0.1.tar.gz` & `tmp/PySDKit-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySDKit-0.1.tar", last modified: Fri May  3 17:02:44 2024, max compression
+gzip compressed data, was "PySDKit-0.3.tar", last modified: Wed May 15 17:43:12 2024, max compression
```

## Comparing `PySDKit-0.1.tar` & `PySDKit-0.3.tar`

### file list

```diff
@@ -1,23 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 17:02:44.602030 PySDKit-0.1/
--rw-rw-rw-   0        0        0      918 2024-05-03 17:02:44.601031 PySDKit-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 17:02:44.594031 PySDKit-0.1/PySDKit.egg-info/
--rw-rw-rw-   0        0        0      918 2024-05-03 17:02:44.000000 PySDKit-0.1/PySDKit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-05-03 17:02:44.000000 PySDKit-0.1/PySDKit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 17:02:44.000000 PySDKit-0.1/PySDKit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-03 17:02:44.000000 PySDKit-0.1/PySDKit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-03 17:02:44.000000 PySDKit-0.1/PySDKit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2024-05-03 16:59:19.000000 PySDKit-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 17:02:44.594031 PySDKit-0.1/emd/
--rw-rw-rw-   0        0        0        0 2024-05-01 16:30:06.000000 PySDKit-0.1/emd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:02:44.595030 PySDKit-0.1/ewt/
--rw-rw-rw-   0        0        0        0 2024-05-01 16:32:02.000000 PySDKit-0.1/ewt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:02:44.596031 PySDKit-0.1/mvmd/
--rw-rw-rw-   0        0        0        0 2024-05-01 16:31:22.000000 PySDKit-0.1/mvmd/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-03 17:02:44.602030 PySDKit-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1747 2024-05-03 16:59:00.000000 PySDKit-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:02:44.599030 PySDKit-0.1/vmd/
--rw-rw-rw-   0        0        0       48 2024-05-01 16:47:30.000000 PySDKit-0.1/vmd/__init__.py
--rw-rw-rw-   0        0        0     4788 2024-05-01 16:31:37.000000 PySDKit-0.1/vmd/vmd_c.py
--rw-rw-rw-   0        0        0     5766 2024-05-01 16:24:35.000000 PySDKit-0.1/vmd/vmd_f.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:02:44.600030 PySDKit-0.1/vncmd/
--rw-rw-rw-   0        0        0        0 2024-05-01 16:31:07.000000 PySDKit-0.1/vncmd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:43:12.887312 PySDKit-0.3/
+-rw-rw-rw-   0        0        0      991 2024-05-15 17:43:12.886313 PySDKit-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 17:43:12.861195 PySDKit-0.3/PySDKit.egg-info/
+-rw-rw-rw-   0        0        0      991 2024-05-15 17:43:12.000000 PySDKit-0.3/PySDKit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2024-05-15 17:43:12.000000 PySDKit-0.3/PySDKit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 17:43:12.000000 PySDKit-0.3/PySDKit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-15 17:43:12.000000 PySDKit-0.3/PySDKit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 17:43:12.000000 PySDKit-0.3/PySDKit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2024-05-15 17:25:59.000000 PySDKit-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 17:43:12.862194 PySDKit-0.3/pysdkit/
+-rw-rw-rw-   0        0        0      107 2024-05-15 16:30:12.000000 PySDKit-0.3/pysdkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:43:12.863194 PySDKit-0.3/pysdkit/data/
+-rw-rw-rw-   0        0        0      459 2024-05-08 13:49:50.000000 PySDKit-0.3/pysdkit/data/__init__.py
+-rw-rw-rw-   0        0        0     9817 2024-05-15 16:49:44.000000 PySDKit-0.3/pysdkit/data/generator.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:43:12.868195 PySDKit-0.3/pysdkit/emd/
+-rw-rw-rw-   0        0        0        0 2024-05-09 14:26:54.000000 PySDKit-0.3/pysdkit/emd/BEMD.py
+-rw-rw-rw-   0        0        0    18480 2024-05-15 17:30:35.000000 PySDKit-0.3/pysdkit/emd/EMD.py
+-rw-rw-rw-   0        0        0       24 2024-05-09 14:26:21.000000 PySDKit-0.3/pysdkit/emd/__init__.py
+-rw-rw-rw-   0        0        0     5505 2024-05-09 13:43:25.000000 PySDKit-0.3/pysdkit/emd/_find_extrema.py
+-rw-rw-rw-   0        0        0    10798 2024-05-08 15:56:55.000000 PySDKit-0.3/pysdkit/emd/_prepare_points.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:43:12.869194 PySDKit-0.3/pysdkit/emd2d/
+-rw-rw-rw-   0        0        0        0 2024-05-09 14:38:56.000000 PySDKit-0.3/pysdkit/emd2d/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:43:12.870195 PySDKit-0.3/pysdkit/ewt/
+-rw-rw-rw-   0        0        0        0 2024-05-01 16:32:02.000000 PySDKit-0.3/pysdkit/ewt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:43:12.871195 PySDKit-0.3/pysdkit/mvmd/
+-rw-rw-rw-   0        0        0        0 2024-05-01 16:31:22.000000 PySDKit-0.3/pysdkit/mvmd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:43:12.875300 PySDKit-0.3/pysdkit/plot/
+-rw-rw-rw-   0        0        0        0 2024-05-04 04:08:43.000000 PySDKit-0.3/pysdkit/plot/__init__.py
+-rw-rw-rw-   0        0        0     3168 2024-05-04 13:32:22.000000 PySDKit-0.3/pysdkit/plot/functions.py
+-rw-rw-rw-   0        0        0       94 2024-05-04 04:23:21.000000 PySDKit-0.3/pysdkit/plot/imf.py
+-rw-rw-rw-   0        0        0      105 2024-05-04 13:09:26.000000 PySDKit-0.3/pysdkit/plot/main.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:43:12.882313 PySDKit-0.3/pysdkit/utils/
+-rw-rw-rw-   0        0        0      605 2024-05-08 15:26:38.000000 PySDKit-0.3/pysdkit/utils/__init__.py
+-rw-rw-rw-   0        0        0     1709 2024-05-05 14:10:39.000000 PySDKit-0.3/pysdkit/utils/base.py
+-rw-rw-rw-   0        0        0      478 2024-05-05 14:05:40.000000 PySDKit-0.3/pysdkit/utils/fft.py
+-rw-rw-rw-   0        0        0     3879 2024-05-08 13:49:50.000000 PySDKit-0.3/pysdkit/utils/hilbert.py
+-rw-rw-rw-   0        0        0     1105 2024-05-04 03:51:06.000000 PySDKit-0.3/pysdkit/utils/mirror.py
+-rw-rw-rw-   0        0        0     6293 2024-05-15 16:56:52.000000 PySDKit-0.3/pysdkit/utils/process.py
+-rw-rw-rw-   0        0        0     2671 2024-05-05 14:10:39.000000 PySDKit-0.3/pysdkit/utils/splines.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:43:12.884312 PySDKit-0.3/pysdkit/vmd/
+-rw-rw-rw-   0        0        0       48 2024-05-01 16:47:30.000000 PySDKit-0.3/pysdkit/vmd/__init__.py
+-rw-rw-rw-   0        0        0     7388 2024-05-05 10:48:29.000000 PySDKit-0.3/pysdkit/vmd/vmd_c.py
+-rw-rw-rw-   0        0        0     5540 2024-05-04 13:50:59.000000 PySDKit-0.3/pysdkit/vmd/vmd_f.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:43:12.885312 PySDKit-0.3/pysdkit/vncmd/
+-rw-rw-rw-   0        0        0        0 2024-05-01 16:31:07.000000 PySDKit-0.3/pysdkit/vncmd/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 17:43:12.887312 PySDKit-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1818 2024-05-15 17:33:41.000000 PySDKit-0.3/setup.py
```

### Comparing `PySDKit-0.1/PKG-INFO` & `PySDKit-0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PySDKit
-Version: 0.1
-Summary: name
+Version: 0.3
+Summary: A Python library for signal decomposition algorithms with a unified interface
 Home-page: https://github.com/wwhenxuan/PySDKit
 Author: whenxuan
 Author-email: wwhenxuan@gmail.com
 Keywords: signal,decomposition
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `PySDKit-0.1/PySDKit.egg-info/PKG-INFO` & `PySDKit-0.3/PySDKit.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PySDKit
-Version: 0.1
-Summary: name
+Version: 0.3
+Summary: A Python library for signal decomposition algorithms with a unified interface
 Home-page: https://github.com/wwhenxuan/PySDKit
 Author: whenxuan
 Author-email: wwhenxuan@gmail.com
 Keywords: signal,decomposition
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `PySDKit-0.1/setup.py` & `PySDKit-0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='PySDKit',  # 使用包的名称
     packages=setuptools.find_packages(),
-    version='0.1',  # 包的版本号，应遵循语义版本控制规则
-    description='name',  # 包的简短描述
+    version='0.3',  # 包的版本号，应遵循语义版本控制规则
+    description='A Python library for signal decomposition algorithms with a unified interface',  # 包的简短描述
     url='https://github.com/wwhenxuan/PySDKit',  # 项目的地址通常来说是github
     author='whenxuan',
     author_email='wwhenxuan@gmail.com',
     keywords=['signal', 'decomposition'],  # 在PyPI上搜索的相应的关键词
     long_description=long_description,  # 这个会将README.md文件的描述放在PyPI网页中
     long_description_content_type="text/markdown",
     classifiers=[
@@ -29,8 +29,8 @@
     ],
     python_requires='>=3.6',  # 最低的Python版本限制
     install_requires=[
         'numpy>=1.24.3',
         'scipy>=1.11.1',
         'matplotlib>=3.7.2'
     ]  # 手动指定依赖的Python以及最低的版本
-)
+)
```

### Comparing `PySDKit-0.1/vmd/vmd_c.py` & `PySDKit-0.3/pysdkit/vmd/vmd_f.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,138 @@
 # -*- coding: utf-8 -*-
+"""
+Created on Sat Mar 4 11:59:21 2024
+@author: Whenxuan Wang
+@email: wwhenxuan@gmail.com
+"""
 import numpy as np
+from ..utils import fft, ifft, fftshift, ifftshift, fmirror
 
 
-class VMD(object):
-
-    def __init__(self):
-        pass
-
-    def fit_transform(self, f, alpha, tau, K, DC, init, tol):
-        if len(f) % 2:
-            f = f[:-1]
-
-        # Period and sampling frequency of input signal
-        fs = 1. / len(f)
-
-        ltemp = len(f) // 2
-        fMirr = np.append(np.flip(f[:ltemp], axis=0), f)
-        fMirr = np.append(fMirr, np.flip(f[-ltemp:], axis=0))
-
-        # Time Domain 0 to T (of mirrored signal)
-        T = len(fMirr)
-        t = np.arange(1, T + 1) / T
-
-        # Spectral Domain discretization
-        freqs = t - 0.5 - (1 / T)
-
-        # Maximum number of iterations (if not converged yet, then it won't anyway)
-        Niter = 500
-        # For future generalizations: individual alpha for each mode
-        Alpha = alpha * np.ones(K)
-
-        # Construct and center f_hat
-        f_hat = np.fft.fftshift((np.fft.fft(fMirr)))
-        f_hat_plus = np.copy(f_hat)  # copy f_hat
-        f_hat_plus[:T // 2] = 0
-
-        # Initialization of omega_k
-        omega_plus = np.zeros([Niter, K])
-
-        if init == 1:
-            for i in range(K):
-                omega_plus[0, i] = (0.5 / K) * (i)
-        elif init == 2:
-            omega_plus[0, :] = np.sort(np.exp(np.log(fs) + (np.log(0.5) - np.log(fs)) * np.random.rand(1, K)))
-        else:
-            omega_plus[0, :] = 0
-
-        # if DC mode imposed, set its omega to 0
-        if DC:
-            omega_plus[0, 0] = 0
-
-        # start with empty dual variables
-        lambda_hat = np.zeros([Niter, len(freqs)], dtype=complex)
-
-        # other inits
-        uDiff = tol + np.spacing(1)  # update step
-        n = 0  # loop counter
-        sum_uk = 0  # accumulator
-        # matrix keeping track of every iterant // could be discarded for mem
-        u_hat_plus = np.zeros([Niter, len(freqs), K], dtype=complex)
-
-        # *** Main loop for iterative updates***
-
-        while (uDiff > tol and n < Niter - 1):  # not converged and below iterations limit
-            # update first mode accumulator
-            k = 0
-            sum_uk = u_hat_plus[n, :, K - 1] + sum_uk - u_hat_plus[n, :, 0]
-
-            # update spectrum of first mode through Wiener filter of residuals
+def vmd(signal: np.array, alpha: int, K: int, tau: float, init: str = 'uniform', DC: bool = False,
+        max_iter: int = 500, tol: float = 1e-6):
+    """
+    Variational mode decomposition, object-oriented interface.
+    Original paper:
+    Dragomiretskiy, K. and Zosso, D. (2014) ‘Variational Mode Decomposition’,
+    IEEE Transactions on Signal Processing, 62(3), pp. 531–544. doi: 10.1109/TSP.2013.2288675.
+    :param signal: the time domain signal (1D numpy array)  to be decomposed
+    :param alpha: the balancing parameter of the data-fidelity constraint
+    :param K: the number of modes to be recovered
+    :param tau: time-step of the dual ascent ( pick 0 for noise-slack )
+    :param init: uniform = all omegas start uniformly distributed
+                 zero = all omegas initialized randomly
+                 random = all omegas start at 0
+    :param DC: true if the first mode is put and kept at DC (0-freq)
+    :param max_iter: Maximum number of iterations
+    :param tol: tolerance of convergence criterion; typically around 1e-6
+    :return: u - the collection of decomposed modes,
+             u_hat   - spectra of the modes,
+             omega   - estimated mode center-frequencies
+    """
+
+    if len(signal) % 2:
+        signal = signal[:-1]
+
+    # Period and sampling frequency of input signal
+    fs = 1. / len(signal)
+
+    # Mirror expansion of signals
+    sym = len(signal) // 2
+    fMirr = fmirror(ts=signal, sym=sym)
+    # Time Domain 0 to T (of mirrored signal)
+    T = len(fMirr)
+    t = np.arange(1, T + 1) / T
+
+    # Time Domain 0 to T (of mirrored signal)
+    T = len(fMirr)
+    t = np.arange(1, T + 1) / T
+
+    # Spectral Domain
+    freqs = t - 0.5 - (1 / T)
+
+    # Construct and center f_hat
+    f_hat = fftshift(ts=fft(ts=fMirr))
+    f_hat_plus = np.copy(f_hat)
+    f_hat_plus[: T // 2] = 0
+
+    # For future generalizations: individual alpha for each mode
+    alpha = np.ones(K) * alpha
+    # matrix keeping track of every iterant // could be discarded for mem
+    u_hat_plus = np.zeros([max_iter, len(freqs), K], dtype=complex)
+    # Initialization of omega_k
+    omega_plus = np.zeros([max_iter, K])
+    if init.lower() == 'uniform':
+        for i in range(K):
+            omega_plus[0, i] = (0.5 / K) * i
+    elif init.lower() == 'random':
+        omega_plus[0, :] = np.sort(np.exp(np.log(fs) + (np.log(0.5) - np.log(fs)) * np.random.rand(1, K)))
+    elif init.lower() == 'zero':
+        omega_plus[0, :] = 0.
+    else:
+        raise ValueError
+    if DC:
+        omega_plus[0, 0] = 0
+    # start with empty dual variables
+    lambda_hat = np.zeros(shape=[max_iter, len(freqs)], dtype=complex)
+
+    sum_uk = 0  # accumulator
+    convergence = np.spacing(1) + tol  # Determine whether the algorithm converges
+
+    # Main loop for iterative updates
+    for n in range(0, max_iter - 1):
+        # update spectrum of first mode through Wiener filter of residuals
+        sum_uk = u_hat_plus[n, :, K - 1] + sum_uk - u_hat_plus[n, :, 0]
+        u_hat_plus[n + 1, :, 0] = (f_hat_plus - sum_uk - lambda_hat[n, :] / 2) / (
+                1. + alpha[0] * (freqs - omega_plus[n, 0]) ** 2)
+
+        # update first omega if not held at 0
+        if not DC:
+            omega_plus[n + 1, 0] = np.dot(freqs[T // 2:T], (abs(u_hat_plus[n + 1, T // 2:T, 0]) ** 2)) / np.sum(
+                abs(u_hat_plus[n + 1, T // 2:T, 0]) ** 2)
+
+        # update of any other mode
+        for k in range(1, K):
+            # mode spectrum
+            sum_uk = u_hat_plus[n + 1, :, k - 1] + sum_uk - u_hat_plus[n, :, k]
             u_hat_plus[n + 1, :, k] = (f_hat_plus - sum_uk - lambda_hat[n, :] / 2) / (
-                    1. + Alpha[k] * (freqs - omega_plus[n, k]) ** 2)
+                    1 + alpha[k] * (freqs - omega_plus[n, k]) ** 2)
+            # center frequencies
+            omega_plus[n + 1, k] = np.dot(freqs[T // 2:T], (abs(u_hat_plus[n + 1, T // 2:T, k]) ** 2)) / np.sum(
+                abs(u_hat_plus[n + 1, T // 2:T, k]) ** 2)
+
+        # Update Lagrange multipliers
+        lambda_hat[n + 1, :] = lambda_hat[n, :] + tau * (np.sum(u_hat_plus[n + 1, :, :], axis=1) - f_hat_plus)
+
+        # Determine whether the algorithm has converged
+        for i in range(K):
+            convergence = convergence + (1 / T) * np.dot((u_hat_plus[n, :, i] - u_hat_plus[n - 1, :, i]),
+                                                         np.conj((u_hat_plus[n, :, i] - u_hat_plus[n - 1, :, i])))
+        convergence = np.abs(convergence)
+        if convergence <= tol:
+            break
+
+    # discard empty space if converged early
+    niter = np.min([max_iter, n])
+    omega = omega_plus[:niter, :]
+    idxs = np.flip(np.arange(1, T // 2 + 1), axis=0)
+
+    # signal reconstruction
+    u_hat = np.zeros([T, K], dtype=complex)
+    u_hat[T // 2:T, :] = u_hat_plus[niter - 1, T // 2:T, :]
+    u_hat[idxs, :] = np.conj(u_hat_plus[niter - 1, T // 2:T, :])
+    u_hat[0, :] = np.conj(u_hat[-1, :])
+
+    u = np.zeros([K, len(t)])
+    for k in range(K):
+        u[k, :] = np.real(ifft(ts=ifftshift(ts=u_hat[:, k])))
+
+    # remove mirror part
+    u = u[:, T // 4:3 * T // 4]
+
+    # recompute spectrum
+    u_hat = np.zeros([u.shape[1], K], dtype=complex)
+    for k in range(K):
+        u_hat[:, k] = fftshift(ts=fft(ts=u[k, :]))
 
-            # update first omega if not held at 0
-            if not (DC):
-                omega_plus[n + 1, k] = np.dot(freqs[T // 2:T], (abs(u_hat_plus[n + 1, T // 2:T, k]) ** 2)) / np.sum(
-                    abs(u_hat_plus[n + 1, T // 2:T, k]) ** 2)
-
-            # update of any other mode
-            for k in np.arange(1, K):
-                # accumulator
-                sum_uk = u_hat_plus[n + 1, :, k - 1] + sum_uk - u_hat_plus[n, :, k]
-                # mode spectrum
-                u_hat_plus[n + 1, :, k] = (f_hat_plus - sum_uk - lambda_hat[n, :] / 2) / (
-                        1 + Alpha[k] * (freqs - omega_plus[n, k]) ** 2)
-                # center frequencies
-                omega_plus[n + 1, k] = np.dot(freqs[T // 2:T], (abs(u_hat_plus[n + 1, T // 2:T, k]) ** 2)) / np.sum(
-                    abs(u_hat_plus[n + 1, T // 2:T, k]) ** 2)
-
-            # Dual ascent
-            lambda_hat[n + 1, :] = lambda_hat[n, :] + tau * (np.sum(u_hat_plus[n + 1, :, :], axis=1) - f_hat_plus)
-
-            # loop counter
-            n = n + 1
-
-            # converged yet?
-            uDiff = np.spacing(1)
-            for i in range(K):
-                uDiff = uDiff + (1 / T) * np.dot((u_hat_plus[n, :, i] - u_hat_plus[n - 1, :, i]),
-                                                 np.conj((u_hat_plus[n, :, i] - u_hat_plus[n - 1, :, i])))
-
-            uDiff = np.abs(uDiff)
-
-            # Postprocessing and cleanup
-
-        # discard empty space if converged early
-        Niter = np.min([Niter, n])
-        omega = omega_plus[:Niter, :]
-
-        idxs = np.flip(np.arange(1, T // 2 + 1), axis=0)
-        # Signal reconstruction
-        u_hat = np.zeros([T, K], dtype=complex)
-        u_hat[T // 2:T, :] = u_hat_plus[Niter - 1, T // 2:T, :]
-        u_hat[idxs, :] = np.conj(u_hat_plus[Niter - 1, T // 2:T, :])
-        u_hat[0, :] = np.conj(u_hat[-1, :])
-
-        u = np.zeros([K, len(t)])
-        for k in range(K):
-            u[k, :] = np.real(np.fft.ifft(np.fft.ifftshift(u_hat[:, k])))
-
-        # remove mirror part
-        u = u[:, T // 4:3 * T // 4]
-
-        # recompute spectrum
-        u_hat = np.zeros([u.shape[1], K], dtype=complex)
-        for k in range(K):
-            u_hat[:, k] = np.fft.fftshift(np.fft.fft(u[k, :]))
+    return u, u_hat, omega
 
-        return u, u_hat, omega
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PySDKit-0.1/vmd/vmd_f.py` & `PySDKit-0.3/pysdkit/vmd/vmd_c.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,159 +1,172 @@
 # -*- coding: utf-8 -*-
 """
-Created on Wed Feb 20 19:24:58 2019
-
-@author: Vinícius Rezende Carvalho
+Created on Sat Mar 4 11:59:21 2024
+@author: Whenxuan Wang
+@email: wwhenxuan@gmail.com
 """
 import numpy as np
+from pysdkit.utils import Base
 
 
-def vmd(f, alpha, tau, K, DC, init, tol):
+class VMD(Base):
     """
-    u,u_hat,omega = VMD(f, alpha, tau, K, DC, init, tol)
-    Variational mode decomposition
-    Python implementation by Vinícius Rezende Carvalho - vrcarva@gmail.com
-    code based on Dominique Zosso's MATLAB code, available at:
-    https://www.mathworks.com/matlabcentral/fileexchange/44765-variational-mode-decomposition
+    Variational mode decomposition, object-oriented interface.
     Original paper:
     Dragomiretskiy, K. and Zosso, D. (2014) ‘Variational Mode Decomposition’,
     IEEE Transactions on Signal Processing, 62(3), pp. 531–544. doi: 10.1109/TSP.2013.2288675.
-
-
-    Input and Parameters:
-    ---------------------
-    f       - the time domain signal (1D) to be decomposed
-    alpha   - the balancing parameter of the data-fidelity constraint
-    tau     - time-step of the dual ascent ( pick 0 for noise-slack )
-    K       - the number of modes to be recovered
-    DC      - true if the first mode is put and kept at DC (0-freq)
-    init    - 0 = all omegas start at 0
-                       1 = all omegas start uniformly distributed
-                      2 = all omegas initialized randomly
-    tol     - tolerance of convergence criterion; typically around 1e-6
-
-    Output:
-    -------
-    u       - the collection of decomposed modes
-    u_hat   - spectra of the modes
-    omega   - estimated mode center-frequencies
     """
 
-    if len(f) % 2:
-        f = f[:-1]
-
-    # Period and sampling frequency of input signal
-    fs = 1. / len(f)
-
-    ltemp = len(f) // 2
-    fMirr = np.append(np.flip(f[:ltemp], axis=0), f)
-    fMirr = np.append(fMirr, np.flip(f[-ltemp:], axis=0))
-
-    # Time Domain 0 to T (of mirrored signal)
-    T = len(fMirr)
-    t = np.arange(1, T + 1) / T
-
-    # Spectral Domain discretization
-    freqs = t - 0.5 - (1 / T)
-
-    # Maximum number of iterations (if not converged yet, then it won't anyway)
-    Niter = 500
-    # For future generalizations: individual alpha for each mode
-    Alpha = alpha * np.ones(K)
-
-    # Construct and center f_hat
-    f_hat = np.fft.fftshift((np.fft.fft(fMirr)))
-    f_hat_plus = np.copy(f_hat)  # copy f_hat
-    f_hat_plus[:T // 2] = 0
-
-    # Initialization of omega_k
-    omega_plus = np.zeros([Niter, K])
-
-    if init == 1:
-        for i in range(K):
-            omega_plus[0, i] = (0.5 / K) * (i)
-    elif init == 2:
-        omega_plus[0, :] = np.sort(np.exp(np.log(fs) + (np.log(0.5) - np.log(fs)) * np.random.rand(1, K)))
-    else:
-        omega_plus[0, :] = 0
-
-    # if DC mode imposed, set its omega to 0
-    if DC:
-        omega_plus[0, 0] = 0
-
-    # start with empty dual variables
-    lambda_hat = np.zeros([Niter, len(freqs)], dtype=complex)
-
-    # other inits
-    uDiff = tol + np.spacing(1)  # update step
-    n = 0  # loop counter
-    sum_uk = 0  # accumulator
-    # matrix keeping track of every iterant // could be discarded for mem
-    u_hat_plus = np.zeros([Niter, len(freqs), K], dtype=complex)
-
-    # *** Main loop for iterative updates***
-
-    while (uDiff > tol and n < Niter - 1):  # not converged and below iterations limit
-        # update first mode accumulator
-        k = 0
-        sum_uk = u_hat_plus[n, :, K - 1] + sum_uk - u_hat_plus[n, :, 0]
-
-        # update spectrum of first mode through Wiener filter of residuals
-        u_hat_plus[n + 1, :, k] = (f_hat_plus - sum_uk - lambda_hat[n, :] / 2) / (
-                    1. + Alpha[k] * (freqs - omega_plus[n, k]) ** 2)
-
-        # update first omega if not held at 0
-        if not (DC):
-            omega_plus[n + 1, k] = np.dot(freqs[T // 2:T], (abs(u_hat_plus[n + 1, T // 2:T, k]) ** 2)) / np.sum(
-                abs(u_hat_plus[n + 1, T // 2:T, k]) ** 2)
-
-        # update of any other mode
-        for k in np.arange(1, K):
-            # accumulator
-            sum_uk = u_hat_plus[n + 1, :, k - 1] + sum_uk - u_hat_plus[n, :, k]
-            # mode spectrum
-            u_hat_plus[n + 1, :, k] = (f_hat_plus - sum_uk - lambda_hat[n, :] / 2) / (
-                        1 + Alpha[k] * (freqs - omega_plus[n, k]) ** 2)
-            # center frequencies
-            omega_plus[n + 1, k] = np.dot(freqs[T // 2:T], (abs(u_hat_plus[n + 1, T // 2:T, k]) ** 2)) / np.sum(
-                abs(u_hat_plus[n + 1, T // 2:T, k]) ** 2)
-
-        # Dual ascent
-        lambda_hat[n + 1, :] = lambda_hat[n, :] + tau * (np.sum(u_hat_plus[n + 1, :, :], axis=1) - f_hat_plus)
-
-        # loop counter
-        n = n + 1
-
-        # converged yet?
-        uDiff = np.spacing(1)
-        for i in range(K):
-            uDiff = uDiff + (1 / T) * np.dot((u_hat_plus[n, :, i] - u_hat_plus[n - 1, :, i]),
-                                             np.conj((u_hat_plus[n, :, i] - u_hat_plus[n - 1, :, i])))
-
-        uDiff = np.abs(uDiff)
-
-        # Postprocessing and cleanup
-
-    # discard empty space if converged early
-    Niter = np.min([Niter, n])
-    omega = omega_plus[:Niter, :]
-
-    idxs = np.flip(np.arange(1, T // 2 + 1), axis=0)
-    # Signal reconstruction
-    u_hat = np.zeros([T, K], dtype=complex)
-    u_hat[T // 2:T, :] = u_hat_plus[Niter - 1, T // 2:T, :]
-    u_hat[idxs, :] = np.conj(u_hat_plus[Niter - 1, T // 2:T, :])
-    u_hat[0, :] = np.conj(u_hat[-1, :])
-
-    u = np.zeros([K, len(t)])
-    for k in range(K):
-        u[k, :] = np.real(np.fft.ifft(np.fft.ifftshift(u_hat[:, k])))
-
-    # remove mirror part
-    u = u[:, T // 4:3 * T // 4]
-
-    # recompute spectrum
-    u_hat = np.zeros([u.shape[1], K], dtype=complex)
-    for k in range(K):
-        u_hat[:, k] = np.fft.fftshift(np.fft.fft(u[k, :]))
-
-    return u, u_hat, omega
+    def __init__(self, alpha: int, K: int, tau: float, init: str = 'uniform', DC: bool = False,
+                 max_iter: int = 500, tol: float = 1e-6):
+        """
+        :param alpha: the balancing parameter of the data-fidelity constraint
+        :param K: the number of modes to be recovered
+        :param tau: time-step of the dual ascent ( pick 0 for noise-slack )
+        :param init: uniform = all omegas start uniformly distributed
+                     zero = all omegas initialized randomly
+                     random = all omegas start at 0
+        :param DC: true if the first mode is put and kept at DC (0-freq)
+        :param max_iter: Maximum number of iterations
+        :param tol: tolerance of convergence criterion; typically around 1e-6
+        """
+        super().__init__()
+        # parameters of VMD signal decomposition algorithm
+        self.alpha = alpha
+        self.K = K
+        self.tau = tau
+        self.init = init
+        self.DC = DC
+        self.max_iter = max_iter
+        self.tol = tol
+
+        # the result of signal decomposition
+        self.u, self.u_hat, self.omega = None, None, None
+
+    def __call__(self, signal: np.array, return_all: bool = False) -> np.array:
+        """allow instances to be called like functions"""
+        return self.fit_transform(signal=signal, return_all=return_all)
+
+    def __init_omega(self, fs: float) -> np.array:
+        """Initialization of omega_k"""
+        omega_plus = np.zeros([self.max_iter, self.K])
+        if self.init.lower() == 'uniform':
+            for i in range(self.K):
+                omega_plus[0, i] = (0.5 / self.K) * i
+        elif self.init.lower() == 'random':
+            omega_plus[0, :] = np.sort(np.exp(np.log(fs) + (np.log(0.5) - np.log(fs)) * np.random.rand(1, self.K)))
+        elif self.init.lower() == 'zero':
+            omega_plus[0, :] = 0.
+        else:
+            raise ValueError
+        return omega_plus
+
+    def fit_transform(self, signal: np.array, return_all: bool = False) -> np.array:
+        """
+        Signal decomposition using VMD algorithm
+        :param signal: the time domain signal (1D numpy array)  to be decomposed
+        :param return_all: Whether to return all results of the algorithm, False only return the collection of decomposed modes,
+                           True plus the spectra of the modes and the estimated mode center-frequencies
+        :return:  u       - the collection of decomposed modes,
+                  u_hat   - spectra of the modes,
+                  omega   - estimated mode center-frequencies
+        """
+        if len(signal) % 2 == 1:
+            signal = signal[:-1]
+
+        # Period and sampling frequency of input signal
+        fs = 1. / len(signal)
+
+        # Mirror expansion of signals
+        sym = len(signal) // 2
+        fMirr = self.fmirror(ts=signal, sym=sym)
+        # Time Domain 0 to T (of mirrored signal)
+        T = len(fMirr)
+        t = np.arange(1, T + 1) / T
+
+        # Spectral Domain
+        freqs = t - 0.5 - (1 / T)
+
+        # Construct and center f_hat
+        f_hat = self.fftshift(ts=self.fft(ts=fMirr))
+        f_hat_plus = np.copy(f_hat)
+        f_hat_plus[: T // 2] = 0
+
+        # For future generalizations: individual alpha for each mode
+        alpha = np.ones(self.K) * self.alpha
+        # matrix keeping track of every iterant // could be discarded for mem
+        u_hat_plus = np.zeros([self.max_iter, len(freqs), self.K], dtype=complex)
+        # Initialization of omega_k
+        omega_plus = self.__init_omega(fs=fs)
+        if self.DC:
+            omega_plus[0, 0] = 0
+        # start with empty dual variables
+        lambda_hat = np.zeros(shape=[self.max_iter, len(freqs)], dtype=complex)
+
+        sum_uk = 0  # accumulator
+        convergence = np.spacing(1) + self.tol  # Determine whether the algorithm converges
+
+        # Main loop for iterative updates
+        for n in range(0, self.max_iter - 1):
+            # update spectrum of first mode through Wiener filter of residuals
+            sum_uk = u_hat_plus[n, :, self.K - 1] + sum_uk - u_hat_plus[n, :, 0]
+            u_hat_plus[n + 1, :, 0] = (f_hat_plus - sum_uk - lambda_hat[n, :] / 2) / (
+                    1. + alpha[0] * (freqs - omega_plus[n, 0]) ** 2)
+
+            # update first omega if not held at 0
+            if not self.DC:
+                omega_plus[n + 1, 0] = np.dot(freqs[T // 2:T], (abs(u_hat_plus[n + 1, T // 2:T, 0]) ** 2)) / np.sum(
+                    abs(u_hat_plus[n + 1, T // 2:T, 0]) ** 2)
+
+            # update of any other mode
+            for k in range(1, self.K):
+                # mode spectrum
+                sum_uk = u_hat_plus[n + 1, :, k - 1] + sum_uk - u_hat_plus[n, :, k]
+                u_hat_plus[n + 1, :, k] = (f_hat_plus - sum_uk - lambda_hat[n, :] / 2) / (
+                        1 + alpha[k] * (freqs - omega_plus[n, k]) ** 2)
+                # center frequencies
+                omega_plus[n + 1, k] = np.dot(freqs[T // 2:T], (abs(u_hat_plus[n + 1, T // 2:T, k]) ** 2)) / np.sum(
+                    abs(u_hat_plus[n + 1, T // 2:T, k]) ** 2)
+
+            # Update Lagrange multipliers
+            lambda_hat[n + 1, :] = lambda_hat[n, :] + self.tau * (np.sum(u_hat_plus[n + 1, :, :], axis=1) - f_hat_plus)
+
+            # Determine whether the algorithm has converged
+            for i in range(self.K):
+                convergence = convergence + (1 / T) * np.dot((u_hat_plus[n, :, i] - u_hat_plus[n - 1, :, i]),
+                                                             np.conj((u_hat_plus[n, :, i] - u_hat_plus[n - 1, :, i])))
+            convergence = np.abs(convergence)
+            if convergence <= self.tol:
+                break
+
+        # discard empty space if converged early
+        niter = np.min([self.max_iter, n])
+        omega = omega_plus[:niter, :]
+        idxs = np.flip(np.arange(1, T // 2 + 1), axis=0)
+
+        # signal reconstruction
+        u_hat = np.zeros([T, self.K], dtype=complex)
+        u_hat[T // 2:T, :] = u_hat_plus[niter - 1, T // 2:T, :]
+        u_hat[idxs, :] = np.conj(u_hat_plus[niter - 1, T // 2:T, :])
+        u_hat[0, :] = np.conj(u_hat[-1, :])
+
+        u = np.zeros([self.K, len(t)])
+        for k in range(self.K):
+            u[k, :] = np.real(self.ifft(ts=self.ifftshift(ts=u_hat[:, k])))
+
+        # remove mirror part
+        u = u[:, T // 4:3 * T // 4]
+
+        # recompute spectrum
+        u_hat = np.zeros([u.shape[1], self.K], dtype=complex)
+        for k in range(self.K):
+            u_hat[:, k] = self.fftshift(ts=self.fft(ts=u[k, :]))
+
+        # record the result of this operation
+        self.u = u
+        self.u_hat = u_hat
+        self.omega = omega
+
+        if return_all is True:
+            return u, u_hat, omega
+        else:
+            return u
```

