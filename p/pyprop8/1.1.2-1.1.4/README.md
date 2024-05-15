# Comparing `tmp/pyprop8-1.1.2.tar.gz` & `tmp/pyprop8-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprop8-1.1.2.tar", last modified: Wed Aug 24 16:49:53 2022, max compression
+gzip compressed data, was "pyprop8-1.1.4.tar", last modified: Wed May 15 14:41:47 2024, max compression
```

## Comparing `pyprop8-1.1.2.tar` & `pyprop8-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 16:49:53.667065 pyprop8-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-08-24 16:49:42.000000 pyprop8-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4282 2022-08-24 16:49:53.667065 pyprop8-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3725 2022-08-24 16:49:42.000000 pyprop8-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-24 16:49:42.000000 pyprop8-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-08-24 16:49:53.667065 pyprop8-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 16:49:53.663065 pyprop8-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 16:49:53.663065 pyprop8-1.1.2/src/pyprop8/
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-08-24 16:49:42.000000 pyprop8-1.1.2/src/pyprop8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    83596 2022-08-24 16:49:42.000000 pyprop8-1.1.2/src/pyprop8/_core.py
--rw-r--r--   0 runner    (1001) docker     (121)    46867 2022-08-24 16:49:42.000000 pyprop8-1.1.2/src/pyprop8/_propagators.py
--rw-r--r--   0 runner    (1001) docker     (121)    14345 2022-08-24 16:49:42.000000 pyprop8-1.1.2/src/pyprop8/_scaledmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-08-24 16:49:42.000000 pyprop8-1.1.2/src/pyprop8/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     8983 2022-08-24 16:49:42.000000 pyprop8-1.1.2/src/pyprop8/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 16:49:53.667065 pyprop8-1.1.2/src/pyprop8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4282 2022-08-24 16:49:53.000000 pyprop8-1.1.2/src/pyprop8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-08-24 16:49:53.000000 pyprop8-1.1.2/src/pyprop8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 16:49:53.000000 pyprop8-1.1.2/src/pyprop8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-24 16:49:53.000000 pyprop8-1.1.2/src/pyprop8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-24 16:49:53.000000 pyprop8-1.1.2/src/pyprop8.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:47.785979 pyprop8-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 14:41:43.000000 pyprop8-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-15 14:41:47.785979 pyprop8-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-15 14:41:43.000000 pyprop8-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 14:41:43.000000 pyprop8-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-15 14:41:47.785979 pyprop8-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:47.781978 pyprop8-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:47.785979 pyprop8-1.1.4/src/pyprop8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-15 14:41:43.000000 pyprop8-1.1.4/src/pyprop8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85846 2024-05-15 14:41:43.000000 pyprop8-1.1.4/src/pyprop8/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46867 2024-05-15 14:41:43.000000 pyprop8-1.1.4/src/pyprop8/_propagators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-05-15 14:41:43.000000 pyprop8-1.1.4/src/pyprop8/_scaledmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-15 14:41:43.000000 pyprop8-1.1.4/src/pyprop8/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-15 14:41:43.000000 pyprop8-1.1.4/src/pyprop8/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:47.785979 pyprop8-1.1.4/src/pyprop8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-15 14:41:47.000000 pyprop8-1.1.4/src/pyprop8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-15 14:41:47.000000 pyprop8-1.1.4/src/pyprop8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:41:47.000000 pyprop8-1.1.4/src/pyprop8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 14:41:47.000000 pyprop8-1.1.4/src/pyprop8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 14:41:47.000000 pyprop8-1.1.4/src/pyprop8.egg-info/top_level.txt
```

### Comparing `pyprop8-1.1.2/LICENSE` & `pyprop8-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprop8-1.1.2/PKG-INFO` & `pyprop8-1.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pyprop8
-Version: 1.1.2
+Version: 1.1.4
 Summary: A lightweight package for synthetic seismograms
 Home-page: https://github.com/valentineap/pyprop8
 Author: Andrew Valentine
 Author-email: andrew.valentine@durham.ac.uk
 Project-URL: Bug Tracker, https://github.com/valentineap/pyprop8/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/valentineap/pyprop8/HEAD?labpath=examples%2Fdemo.ipynb)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04217/status.svg)](https://doi.org/10.21105/joss.04217) [![PyPI version](https://badge.fury.io/py/pyprop8.svg)](https://badge.fury.io/py/pyprop8) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/valentineap/pyprop8/HEAD?labpath=examples%2Fdemo.ipynb)
 
 # pyprop8
 
 This package provides a lightweight Python implementation of the seismogram calculation algorithm set out in [O'Toole & Woodhouse (2011)](https://doi.org/10.1111/j.1365-246X.2011.05210.x), together with the source derivatives set out in [O'Toole, Valentine & Woodhouse (2012)](https://doi.org/10.1111/j.1365-246X.2012.05608.x). It is intended to provide a lightweight, easy-to-install seismological forward model suitable for use in teaching and research (in particular, to provide a computationally-cheap yet physically-realistic forward problem for use in the development and testing of inversion algorithms).
 
 Full documentation is [available here](https://pyprop8.readthedocs.io/), and you can try the package out [using Binder](https://mybinder.org/v2/gh/valentineap/pyprop8/HEAD?labpath=examples%2Fdemo.ipynb).
 
@@ -42,19 +44,19 @@
 Some of the examples found in `examples/` may have additional dependencies and requirements, including [Jupyter](https://jupyter.org) and [`matplotlib`](https://matplotlib.org'). Look for a `requirements.txt` file in the relevant example directory; you can install the necessary pacakges using the command `pip install -r requirements.txt`.
 
 ## Citing this package
 
 If you make use of this code, please acknowledge the work that went into developing it! In particular, if you are preparing a publication, we would appreciate it if you cite both the paper describing the general method, and this specific implementation:
 
 - [O'Toole, T.B. & J.H. Woodhouse (2011)](https://doi.org/10.1111/j.1365-246X.2011.05210.x), "Numerically stable computation of complete synthetic seismograms including the static displacement in plane layered media", Geophysical Journal International, 187, pp.1516-1536, doi:10.1111/j.1365-246X.2011.05210.x
-- Valentine, A.P. & M. Sambridge (2022), "`pyprop8`: A lightweight code to simulate seismic observables in a layered half-space", Journal of Open Source Software
+- [Valentine, A.P. & M. Sambridge (2022)](https://doi.org/10.21105/joss.04217), "`pyprop8`: A lightweight code to simulate seismic observables in a layered half-space", Journal of Open Source Software, 7, 4217, doi:10.21105/joss.04217.
 
 
 If your work relies on being able to calculate the source parameter derivatives, you should also cite the paper describing how these are obtained:
 
-- [O'Toole, Valentine & Woodhouse (2012)](https://doi.org/10.1111/j.1365-246X.2012.05608.x), "Centroid–moment tensor inversions using high-rate GPS waveforms", Geophysical Journal International, 191, pp.257-270, doi:10.1111/j.1365-246X.2012.05608.x
+- [O'Toole, Valentine & Woodhouse (2012)](https://doi.org/10.1111/j.1365-246X.2012.05608.x), "Centroid–moment tensor inversions using high-rate GPS waveforms", Geophysical Journal International, 191, pp.257-270, doi:10.1111/j.1365-246X.2012.05608.x.
 
 ## Acknowledgements
 
 This package was developed at the Australian National University and Durham University by Andrew Valentine. It builds on earlier work by Tom O'Toole and John Woodhouse, and has benefited from sight of code written by those authors. In particular, the exponential rescaling of the propagator matrices is inspired by their implementation. However, the present code has been developed 'from scratch' based on the published algorithms.
 
 This work has received support from the Australian Research Council under grants DE180100040 and DP200100053.
```

### Comparing `pyprop8-1.1.2/README.md` & `pyprop8-1.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/valentineap/pyprop8/HEAD?labpath=examples%2Fdemo.ipynb)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04217/status.svg)](https://doi.org/10.21105/joss.04217) [![PyPI version](https://badge.fury.io/py/pyprop8.svg)](https://badge.fury.io/py/pyprop8) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/valentineap/pyprop8/HEAD?labpath=examples%2Fdemo.ipynb)
 
 # pyprop8
 
 This package provides a lightweight Python implementation of the seismogram calculation algorithm set out in [O'Toole & Woodhouse (2011)](https://doi.org/10.1111/j.1365-246X.2011.05210.x), together with the source derivatives set out in [O'Toole, Valentine & Woodhouse (2012)](https://doi.org/10.1111/j.1365-246X.2012.05608.x). It is intended to provide a lightweight, easy-to-install seismological forward model suitable for use in teaching and research (in particular, to provide a computationally-cheap yet physically-realistic forward problem for use in the development and testing of inversion algorithms).
 
 Full documentation is [available here](https://pyprop8.readthedocs.io/), and you can try the package out [using Binder](https://mybinder.org/v2/gh/valentineap/pyprop8/HEAD?labpath=examples%2Fdemo.ipynb).
 
@@ -27,19 +27,19 @@
 Some of the examples found in `examples/` may have additional dependencies and requirements, including [Jupyter](https://jupyter.org) and [`matplotlib`](https://matplotlib.org'). Look for a `requirements.txt` file in the relevant example directory; you can install the necessary pacakges using the command `pip install -r requirements.txt`.
 
 ## Citing this package
 
 If you make use of this code, please acknowledge the work that went into developing it! In particular, if you are preparing a publication, we would appreciate it if you cite both the paper describing the general method, and this specific implementation:
 
 - [O'Toole, T.B. & J.H. Woodhouse (2011)](https://doi.org/10.1111/j.1365-246X.2011.05210.x), "Numerically stable computation of complete synthetic seismograms including the static displacement in plane layered media", Geophysical Journal International, 187, pp.1516-1536, doi:10.1111/j.1365-246X.2011.05210.x
-- Valentine, A.P. & M. Sambridge (2022), "`pyprop8`: A lightweight code to simulate seismic observables in a layered half-space", Journal of Open Source Software
+- [Valentine, A.P. & M. Sambridge (2022)](https://doi.org/10.21105/joss.04217), "`pyprop8`: A lightweight code to simulate seismic observables in a layered half-space", Journal of Open Source Software, 7, 4217, doi:10.21105/joss.04217.
 
 
 If your work relies on being able to calculate the source parameter derivatives, you should also cite the paper describing how these are obtained:
 
-- [O'Toole, Valentine & Woodhouse (2012)](https://doi.org/10.1111/j.1365-246X.2012.05608.x), "Centroid–moment tensor inversions using high-rate GPS waveforms", Geophysical Journal International, 191, pp.257-270, doi:10.1111/j.1365-246X.2012.05608.x
+- [O'Toole, Valentine & Woodhouse (2012)](https://doi.org/10.1111/j.1365-246X.2012.05608.x), "Centroid–moment tensor inversions using high-rate GPS waveforms", Geophysical Journal International, 191, pp.257-270, doi:10.1111/j.1365-246X.2012.05608.x.
 
 ## Acknowledgements
 
 This package was developed at the Australian National University and Durham University by Andrew Valentine. It builds on earlier work by Tom O'Toole and John Woodhouse, and has benefited from sight of code written by those authors. In particular, the exponential rescaling of the propagator matrices is inspired by their implementation. However, the present code has been developed 'from scratch' based on the published algorithms.
 
 This work has received support from the Australian Research Council under grants DE180100040 and DP200100053.
```

### Comparing `pyprop8-1.1.2/setup.cfg` & `pyprop8-1.1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyprop8
-version = 1.1.2
+version = 1.1.4
 author = Andrew Valentine
 author_email = andrew.valentine@durham.ac.uk
 description = A lightweight package for synthetic seismograms
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/valentineap/pyprop8
 project_urls =
```

### Comparing `pyprop8-1.1.2/src/pyprop8/__init__.py` & `pyprop8-1.1.4/src/pyprop8/__init__.py`

 * *Files identical despite different names*

### Comparing `pyprop8-1.1.2/src/pyprop8/_core.py` & `pyprop8-1.1.4/src/pyprop8/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 import numpy as np
 from pyprop8._propagators import *
 import scipy.special as spec
+HAS_MULTIPROCESSING = False
+try:
+    from multiprocessing import Pool
+    HAS_MULTIPROCESSING = True
+except:
+    pass
+
 
 # from tqdm.autonotebook import tqdm edited by MS 2/3/21 due to warning in Anaconda JupyterLab
 import warnings
 
 try:
     from tqdm import tqdm
 except ImportError:
@@ -1624,14 +1631,15 @@
     alpha=None,
     source_time_function=None,
     pad_frac=0.5,
     xyz=True,
     derivatives=None,
     show_progress=True,
     squeeze_outputs=True,
+    number_of_processes=1,
     **kwargs
 ):
     """
     Calculate and return displacement seismograms for a given source and earth
     model at specified locations.
 
     :param LayeredStructureModel structure: The earth model within which
@@ -1661,14 +1669,18 @@
         the three components will be expressed in  polar coordinates:
         radial/transverse/vertical.
     :param DerivativeSwitches or None derivatives: Determines which derivatives
         are computed and returned. See also discussion of return value, below.
     :param bool show_progress: Display progress bars if available.
     :param bool squeeze_outputs: If true, apply :py:func:`numpy.squeeze` to all
         output arrays to eliminate dimensions of size '1'.
+    :param int number_of_processes: The number of processes to use while
+        performing computations. If >1, the `multiprocessing` module will be
+        used, splitting up the frequency band across processs. Due to the cost
+        of creating and managing separate processes, more is not always faster.
     :param bool \**kwargs: Any additional keyword options will be passed to
         :py:func:`~pyprop8.compute_spectra`.
 
     The output of ``compute_seismograms`` depends on value of the ``derivatives``
     parameter.
 
     :returns: If ``derivatives = None`` then ``compute_spectra`` returns a tuple,
@@ -1719,28 +1731,58 @@
         do_derivatives = False
     else:
         if derivatives.nderivs == 0:
             # Nothing actually turned on...
             do_derivatives = False
         else:
             do_derivatives = True
+    if number_of_processes==1:
+        spectra = compute_spectra(
+            structure,
+            source,
+            stations,
+            ww,
+            derivatives,
+            show_progress,
+            squeeze_outputs=False,
+            **kwargs
+        )
+        if derivatives is not None:
+            # Test on derivatives, not do_derivatives, as will return d_spectra as None if derivatives provided but all off
+            spectra, d_spectra = spectra
+    else:
+        if not HAS_MULTIPROCESSING:
+            raise ModuleNotFoundError("Setting `number_of_processes > 1` requires the `multiprocessing` module, which appears not to be available.")
+        # The following is done inside compute_spectra -- need to do it here as 'side effects' don't get copied
+        # back to the main process.
+        stations.generate_rphi(source.x,source.y)
+        stations.validate()
+        with Pool(number_of_processes) as pool:
+            # Give each thread an evenly-distributed set of frequencies as costs may be frequency-dependent
+            qs = [pool.apply_async(compute_spectra,(structure, source, stations, ww[ipool::number_of_processes], derivatives),
+                                    {'show_progress':False,'squeeze_outputs':False}|kwargs) for ipool in range(number_of_processes)]
+            # Accumulate results
+            for ipool,q in enumerate(qs):
+                spec_part = q.get()
+                if derivatives is not None:
+                    spec_part, d_spec_part = spec_part
+                if ipool==0:
+                    # Allocate arrays
+                    shape = list(spec_part.shape)
+                    shape[-1] = ww.shape[0]
+                    spectra = np.zeros(shape,dtype=spec_part.dtype)
+                    if derivatives is not None:
+                        shape = list(d_spec_part.shape)
+                        shape[-1] = ww.shape[0]
+                        d_spectra = np.zeros(shape,dtype=d_spec_part.dtype)
+                spectra[...,ipool::number_of_processes] = spec_part
+                if derivatives is not None:
+                    d_spectra[...,ipool::number_of_processes] = d_spec_part
+        pool.join()
 
-    spectra = compute_spectra(
-        structure,
-        source,
-        stations,
-        ww,
-        derivatives,
-        show_progress,
-        squeeze_outputs=False,
-        **kwargs
-    )
-    if derivatives is not None:
-        # Test on derivatives, not do_derivatives, as will return d_spectra as None if derivatives provided but all off
-        spectra, d_spectra = spectra
     if type(stations) is RegularlyDistributedReceivers:
         ess = "srpcw,w->srpcw"
         essd = "srpdcw,w->srpdcw"
         est = "ut,srpct,t->srpcu"
         estd = "ut,srpdct,t->srpdcu"
     elif type(stations) is ListOfReceivers:
         ess = "srcw,w->srcw"
```

### Comparing `pyprop8-1.1.2/src/pyprop8/_propagators.py` & `pyprop8-1.1.4/src/pyprop8/_propagators.py`

 * *Files identical despite different names*

### Comparing `pyprop8-1.1.2/src/pyprop8/_scaledmatrix.py` & `pyprop8-1.1.4/src/pyprop8/_scaledmatrix.py`

 * *Files identical despite different names*

### Comparing `pyprop8-1.1.2/src/pyprop8/tests.py` & `pyprop8-1.1.4/src/pyprop8/tests.py`

 * *Files identical despite different names*

### Comparing `pyprop8-1.1.2/src/pyprop8/utils.py` & `pyprop8-1.1.4/src/pyprop8/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -73,14 +73,37 @@
     #         = 0         otherwise
     # with T <--> `thalf`
     return np.sin(omega * thalf) / (omega * thalf)
 
 def stf_cosine_boxcar(omega, thalf, ratio=0.1):
     return np.pi**2 * np.cos(thalf*ratio*omega)*np.sin(thalf*omega*(ratio-1))/((ratio-1)*thalf*omega*(np.pi-2*ratio*thalf*omega)*(np.pi+2*ratio*thalf*omega))
 
+def stf_ricker(omega, twidth):
+    """
+    Ricker wavelet.
+    
+    This function implements the Fourier transform of
+    
+    f(t,T) = 2/(sqrt(3T).pi^(1/4)) . (1-(t/T)^2) . exp(-t^2/ (2T^2))
+    
+    which is equivalent to scipy.signal.ricker with that function's `a` <--> `twidth`.
+    
+    :param complex omega: Frequency at which evaluation is required (rad/s)
+    :param float twidth:  Width of wavelet. This is the 'standard deviation' parameter of the
+                          Gaussian from which the Ricker wavelet is derived. The peak frequency
+                          of the wavelet is related to twidth by:
+                          
+                          f_M = 1/ (sqrt(2) pi twidth)     Hz   
+                          or
+                          w_M = sqrt(2)/twidth             rad/s
+     :returns: Amplitude of the filter.               
+                          
+    """
+    return 2*np.sqrt(2/3)*np.exp(-0.5*(twidth*omega)**2)*(np.pi**0.25)*(twidth**2.5)*(omega**2)
+
 def clp_filter(w, w0, w1):
     """
     Cosine low-pass filter.
     
     :param complex w: Frequency a t which evaluation is required (rad/s)
     :param float w0: Corner frequency for start of taper; at frequencies below this the filter has no impact.
     :param float w1: Corner frequency for end of taper; frequencies above this are stopped.
```

### Comparing `pyprop8-1.1.2/src/pyprop8.egg-info/PKG-INFO` & `pyprop8-1.1.4/src/pyprop8.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pyprop8
-Version: 1.1.2
+Version: 1.1.4
 Summary: A lightweight package for synthetic seismograms
 Home-page: https://github.com/valentineap/pyprop8
 Author: Andrew Valentine
 Author-email: andrew.valentine@durham.ac.uk
 Project-URL: Bug Tracker, https://github.com/valentineap/pyprop8/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/valentineap/pyprop8/HEAD?labpath=examples%2Fdemo.ipynb)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04217/status.svg)](https://doi.org/10.21105/joss.04217) [![PyPI version](https://badge.fury.io/py/pyprop8.svg)](https://badge.fury.io/py/pyprop8) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/valentineap/pyprop8/HEAD?labpath=examples%2Fdemo.ipynb)
 
 # pyprop8
 
 This package provides a lightweight Python implementation of the seismogram calculation algorithm set out in [O'Toole & Woodhouse (2011)](https://doi.org/10.1111/j.1365-246X.2011.05210.x), together with the source derivatives set out in [O'Toole, Valentine & Woodhouse (2012)](https://doi.org/10.1111/j.1365-246X.2012.05608.x). It is intended to provide a lightweight, easy-to-install seismological forward model suitable for use in teaching and research (in particular, to provide a computationally-cheap yet physically-realistic forward problem for use in the development and testing of inversion algorithms).
 
 Full documentation is [available here](https://pyprop8.readthedocs.io/), and you can try the package out [using Binder](https://mybinder.org/v2/gh/valentineap/pyprop8/HEAD?labpath=examples%2Fdemo.ipynb).
 
@@ -42,19 +44,19 @@
 Some of the examples found in `examples/` may have additional dependencies and requirements, including [Jupyter](https://jupyter.org) and [`matplotlib`](https://matplotlib.org'). Look for a `requirements.txt` file in the relevant example directory; you can install the necessary pacakges using the command `pip install -r requirements.txt`.
 
 ## Citing this package
 
 If you make use of this code, please acknowledge the work that went into developing it! In particular, if you are preparing a publication, we would appreciate it if you cite both the paper describing the general method, and this specific implementation:
 
 - [O'Toole, T.B. & J.H. Woodhouse (2011)](https://doi.org/10.1111/j.1365-246X.2011.05210.x), "Numerically stable computation of complete synthetic seismograms including the static displacement in plane layered media", Geophysical Journal International, 187, pp.1516-1536, doi:10.1111/j.1365-246X.2011.05210.x
-- Valentine, A.P. & M. Sambridge (2022), "`pyprop8`: A lightweight code to simulate seismic observables in a layered half-space", Journal of Open Source Software
+- [Valentine, A.P. & M. Sambridge (2022)](https://doi.org/10.21105/joss.04217), "`pyprop8`: A lightweight code to simulate seismic observables in a layered half-space", Journal of Open Source Software, 7, 4217, doi:10.21105/joss.04217.
 
 
 If your work relies on being able to calculate the source parameter derivatives, you should also cite the paper describing how these are obtained:
 
-- [O'Toole, Valentine & Woodhouse (2012)](https://doi.org/10.1111/j.1365-246X.2012.05608.x), "Centroid–moment tensor inversions using high-rate GPS waveforms", Geophysical Journal International, 191, pp.257-270, doi:10.1111/j.1365-246X.2012.05608.x
+- [O'Toole, Valentine & Woodhouse (2012)](https://doi.org/10.1111/j.1365-246X.2012.05608.x), "Centroid–moment tensor inversions using high-rate GPS waveforms", Geophysical Journal International, 191, pp.257-270, doi:10.1111/j.1365-246X.2012.05608.x.
 
 ## Acknowledgements
 
 This package was developed at the Australian National University and Durham University by Andrew Valentine. It builds on earlier work by Tom O'Toole and John Woodhouse, and has benefited from sight of code written by those authors. In particular, the exponential rescaling of the propagator matrices is inspired by their implementation. However, the present code has been developed 'from scratch' based on the published algorithms.
 
 This work has received support from the Australian Research Council under grants DE180100040 and DP200100053.
```

