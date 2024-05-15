# Comparing `tmp/pyBAKS-0.1.6.tar.gz` & `tmp/pyBAKS-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyBAKS-0.1.6.tar", last modified: Tue Dec 12 18:56:37 2023, max compression
+gzip compressed data, was "dist/pyBAKS-0.1.7.tar", last modified: Wed May 15 16:09:23 2024, max compression
```

## Comparing `pyBAKS-0.1.6.tar` & `pyBAKS-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-12-12 18:56:37.000000 pyBAKS-0.1.6/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      281 2023-12-12 18:56:37.000000 pyBAKS-0.1.6/PKG-INFO
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-12-12 18:56:37.000000 pyBAKS-0.1.6/pyBAKS/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    20777 2023-12-12 18:51:29.000000 pyBAKS-0.1.6/pyBAKS/BAKS.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     5760 2023-12-11 20:21:35.000000 pyBAKS-0.1.6/pyBAKS/BAKS_test.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)       25 2023-11-07 21:29:57.000000 pyBAKS-0.1.6/pyBAKS/__init__.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-12-12 18:56:37.000000 pyBAKS-0.1.6/pyBAKS.egg-info/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      701 2023-12-12 18:53:53.000000 pyBAKS-0.1.6/pyBAKS.egg-info/CHANGES.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      281 2023-12-12 18:56:36.000000 pyBAKS-0.1.6/pyBAKS.egg-info/PKG-INFO
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      239 2023-12-12 18:56:37.000000 pyBAKS-0.1.6/pyBAKS.egg-info/SOURCES.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        1 2023-12-12 18:56:36.000000 pyBAKS-0.1.6/pyBAKS.egg-info/dependency_links.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)       38 2023-12-12 18:56:37.000000 pyBAKS-0.1.6/pyBAKS.egg-info/requires.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        7 2023-12-12 18:56:37.000000 pyBAKS-0.1.6/pyBAKS.egg-info/top_level.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)       38 2023-12-12 18:56:37.000000 pyBAKS-0.1.6/setup.cfg
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      436 2023-12-12 18:54:04.000000 pyBAKS-0.1.6/setup.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2024-05-15 16:09:23.000000 pyBAKS-0.1.7/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      281 2024-05-15 16:09:23.000000 pyBAKS-0.1.7/PKG-INFO
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2024-05-15 16:09:23.000000 pyBAKS-0.1.7/pyBAKS/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    21362 2024-05-15 16:04:03.000000 pyBAKS-0.1.7/pyBAKS/BAKS.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     8659 2024-05-14 19:49:41.000000 pyBAKS-0.1.7/pyBAKS/BAKS_test.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)       25 2023-11-07 21:29:57.000000 pyBAKS-0.1.7/pyBAKS/__init__.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2024-05-15 16:09:23.000000 pyBAKS-0.1.7/pyBAKS.egg-info/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      705 2024-05-15 16:09:15.000000 pyBAKS-0.1.7/pyBAKS.egg-info/CHANGES.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      281 2024-05-15 16:09:23.000000 pyBAKS-0.1.7/pyBAKS.egg-info/PKG-INFO
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      239 2024-05-15 16:09:23.000000 pyBAKS-0.1.7/pyBAKS.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        1 2024-05-15 16:09:23.000000 pyBAKS-0.1.7/pyBAKS.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)       38 2024-05-15 16:09:23.000000 pyBAKS-0.1.7/pyBAKS.egg-info/requires.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        7 2024-05-15 16:09:23.000000 pyBAKS-0.1.7/pyBAKS.egg-info/top_level.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)       38 2024-05-15 16:09:23.000000 pyBAKS-0.1.7/setup.cfg
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      436 2024-05-15 16:09:15.000000 pyBAKS-0.1.7/setup.py
```

### Comparing `pyBAKS-0.1.6/pyBAKS/BAKS.py` & `pyBAKS-0.1.7/pyBAKS/BAKS.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,37 +16,38 @@
     
     if np.all(np.isin(SpikeTimes, [0, 1])) and len(SpikeTimes) > 2:  # if SpikeTimes is a spike array, convert to spike times
         print("SpikeTimes is a spike array, converting to spike times")
         if len(SpikeTimes) != len(Time):
             raise ValueError("Spike array and time array must have the same length.")
         SpikeTimes = extract_spike_times(SpikeTimes, Time)
 
-    elif a < 1:
-        raise ValueError("according to Ahmadi et al., alpha (a) must be >= 1")
+    # elif a < 1:
+    #     raise ValueError("according to Ahmadi et al., alpha (a) must be >= 1")
 
     N = len(SpikeTimes)
-    sumnum = 0
-    sumdenum = 0
-
     if b is None:  # if b is not specified, use the default calculation from Ahmadi et al.
         b = N ** (4 / 5)
 
+    sumnum = 0
+    sumdenum = 0
+
     # calculate h (eq 11 in Ahmadi et al.)
     for i in range(N):
-        innerterm = ((((Time - SpikeTimes[i]) ** 2) / 2) + (1 / b))
-        numerator = innerterm ** (-a)
-        denumerator = innerterm ** (-a - 0.5)
+        numerator = (((Time - SpikeTimes[i]) ** 2) / 2 + 1 / b) ** (-a)
+        denumerator = (((Time - SpikeTimes[i]) ** 2) / 2 + 1 / b) ** (-a - 0.5)
         sumnum += numerator
         sumdenum += denumerator
-    h = (gamma(a) * sumnum) / (gamma(a + 0.5) * sumdenum)
+
+    h = (gamma(a)/gamma(a + 0.5)) * (sumnum / sumdenum)
 
     # calculate firing rate (eq 12 in Ahmadi et al.)
     FiringRate = np.zeros(len(Time))
     for j in range(N):
         K = (1 / (np.sqrt(2 * np.pi) * h)) * np.exp(-((Time - SpikeTimes[j]) ** 2) / (2 * h ** 2))
+
         FiringRate += K
 
     return FiringRate, h
 
 
 def rolling_window(Spikes, dt, ws):
     """
@@ -63,59 +64,75 @@
     window = ws / dt
     window = int(window)
     kernel = np.ones(window) / window
 
     result = np.apply_along_axis(lambda x: np.convolve(x, kernel, mode='same'), axis=1, arr=Spikes)
     winAvg = result / dt
 
-    ll = firingrate_loglike(Spikes, winAvg)
-    return winAvg, ll
+    return winAvg
 
 
 def firingrate_loglike(Spikes, FiringRate):
+    if Spikes.sum() == 0:
+        raise ValueError("Spikes array is empty")
     if Spikes.ndim == 2:
-        loglike = np.sum(np.log((FiringRate ** Spikes * np.exp(-FiringRate)) / factorial(Spikes)), axis=1)
+        loglike = np.sum(np.log((FiringRate ** Spikes * np.exp(-FiringRate))), axis=1)
         if len(loglike) == 1:
-            loglike = loglike[0]
+            loglike = loglike.flatten()
     else:
-        loglike = np.sum(np.log((FiringRate ** Spikes * np.exp(-FiringRate)) / factorial(Spikes)))
+        loglike = np.sum(np.log((FiringRate ** Spikes * np.exp(-FiringRate))))
     return loglike
 
 
 def extract_spike_times(Spikes, Time):
     """
     :param Spikes: 1D binary emissions array
     :param Time: 1D time array same length as Spikes
     :param dt: time step--amount of time between each increment in time array
     :return: SpikeTimes: 1D array of spike times
     """
 
-    if len(Spikes) != len(Time):
+    if type(Spikes) == list:
+        Spikes = np.array(Spikes)
+    if type(Time) == list:
+        Time = np.array(Time)
+    if Spikes.shape != Time.shape:
         raise ValueError("Spike array and time array must have the same length.")
         
-    if sum(Spikes) == 0:
+    if Spikes.sum() == 0:
         return None
+
     else:
-        spikeIdxs = np.where(Spikes == 1)
+        spikeIdxs = np.where(Spikes)
         SpikeTimes = Time[spikeIdxs]
         return SpikeTimes
 
 
-def getMISE(true_rate, est_rate):
+def getMISE(true_rate, est_rate, dt=0.001):
     """
     getMISE is used to calculate the mean integrated square error (MISE) between the true rate and estimated rate.
     to use this tool, you should first generate a simulated "known" rate array, then use that to generate
     a simulated spike train, and then get the BAkS-estimated rate from the simulated spike train.
     getMISE calculates the MISE between an a known-rate array and a BAKS-estimated rate array.
     :param true_rate: a rate array with the (known) true rate, can be generated by spikearray_poissonsim
     :param est_rate: an array of the estimated rate
     :return MISE: mean integrated squared error between true rate and estimated rate
     """
-    nt = len(true_rate)
-    MISE = np.sum((est_rate - true_rate) ** 2) / nt
+    # Ensure the arrays are numpy arrays
+    true_rate = np.array(true_rate)
+    est_rate = np.array(est_rate)
+
+    # Compute the squared errors
+    squared_errors = (true_rate - est_rate) ** 2
+
+    # Compute the mean of the squared errors
+    mean_squared_error = np.mean(squared_errors)
+
+    # Compute the MISE
+    MISE = dt * mean_squared_error
     return MISE
 
 
 def spikearray_poissonsim(Spikes, Time):
     """
     a simulated spike array with known firing rate is required to optimize alpha for BAKS
     this function generates a similuated spike array based on Spikes
@@ -130,42 +147,40 @@
     """
 
     if Spikes.ndim == 1:
         Spikes = Spikes.reshape(1, -1)
         Time = Time.reshape(1, -1)
 
     n_time_bins = Spikes.shape[1]
-    time_range = Time[0, -1] - Time[0, 0]
-
-    dt = time_range / n_time_bins
 
+    dt = Time[0,1] - Time[0,0]
     sim_spikes = np.zeros(Spikes.shape)
     sim_rate = np.zeros(Spikes.shape)
-    step = int(n_time_bins / 4)
+    n_sim_bins = int(n_time_bins / 4)
     ntrls = Spikes.shape[0]
 
+
     for i in range(4):
         samp = np.random.randint(0, n_time_bins, size=2)
         start = np.min(samp)
         end = np.max(samp)
-
-        slice = Spikes[:, start:end]
-        slicerate = np.sum(slice, axis=1) / ((end - start) * dt)
-        sliceprob = slicerate / n_time_bins
-        sliceprob = sliceprob.reshape(-1, 1)
-        slice_vals = np.random.rand(ntrls, step)
-        slice_spikes = slice_vals <= sliceprob
-        sim_spikes[:, step * i:step * (i + 1)] = slice_spikes
-        sim_rate[:, step * i:step * (i + 1)] = slicerate.reshape(-1, 1)
+        nbins = end - start
+        arrslice = Spikes[:, start:end]
+        nspikes = arrslice.sum()
+        sliceprob = nspikes / nbins
+        slicerate = sliceprob / dt
+        slice_spikes = np.random.poisson(sliceprob, (ntrls, n_sim_bins))
+        sim_spikes[:, n_sim_bins * i:n_sim_bins * (i + 1)] = slice_spikes
+        sim_rate[:, n_sim_bins * i:n_sim_bins * (i + 1)] = slicerate.reshape(-1, 1)
 
     sim_time = Time
     return sim_spikes, sim_rate, sim_time
 
 
-def optimize_alpha_MISE(Spikes, Time, nIter=100, alpha_start=1, alpha_end=10, alpha_step=0.1):
+def optimize_alpha_MISE(Spikes, Time, nIter=100, alpha_start=0.01, alpha_end=4, alpha_step=0.01):
     """
     optimize_alpha is used to optimize alpha for BAKS from a 1D array of real spiking data.
     it uses the real data to generate a simulated spike array with known rate,
     then uses that to generate a BAKS-estimated rate,
     then getMISE to calculate the MISE between the known rate and the BAKS-estimated rate,
     and repeats this over a range of alpha values to find the alpha value with the lowest MISE.
     :param Spikes: 1D spike train from real data
@@ -173,27 +188,35 @@
     :param nIter: how many iterations to run
     :param alpha_start: minimum alpha value to test.
     :param alpha_end: maximum alpha value to test.
     :param alpha_step: step size for alpha values.
     :return: df: pandas dataframe with iternums, MISEs, and alphas
     :return: best_alpha: alpha value with lowest MISE
     """
+    if Spikes.ndim == 2: # if Spikes is a 2D array, flatten it
+        Spikes = Spikes.flatten()
+        Time = Time.flatten()
+
+    dt = Time[1] - Time[0]
 
     alpha_range = np.arange(alpha_start, alpha_end, alpha_step)
     iternums = []
     MISEs = []
     alphas = []
     likelihoods = []
-    for iter in range(nIter):
+    for i in range(nIter):
         sim_spikes, sim_rate, sim_time = spikearray_poissonsim(Spikes, Time)
+        sim_spikes = sim_spikes.flatten()
+        sim_rate = sim_rate.flatten()
+        sim_time = sim_time.flatten()
         sim_spiketimes = extract_spike_times(sim_spikes, sim_time)
         for a in alpha_range:
-            BAKSrate, h, = BAKS(sim_spiketimes, Time, a)
+            BAKSrate, h, = BAKS(sim_spiketimes, sim_time, a)
             lh = firingrate_loglike(sim_spikes, BAKSrate)
-            MISE = getMISE(sim_rate, BAKSrate)
+            MISE = getMISE(sim_rate, BAKSrate, dt)
             iternums.append(iter)
             MISEs.append(MISE)
             alphas.append(a)
             likelihoods.append(lh)
 
     # make a pandas table with iternums, MISEs, and alphas
     df = pd.DataFrame({'iteration': iternums, 'MISE': MISEs, 'alpha': alphas, 'likelihood': likelihoods})
@@ -205,51 +228,50 @@
               "Consider increasing alpha_end.")
 
     return df, best_alpha
 
 
 def parse_dims(Spikes):
     ndim = None
-    kind = None
-    if isinstance(Spikes, pd.Series):
-        kind = 'series'
+    kind = type(Spikes)
+
+    if kind == np.ndarray:
         # determine if Spikes is a list of arrays or a single array
-        if isinstance(Spikes.iloc[0], np.ndarray):
+        ndim = Spikes.ndim
+
+    elif kind == list:
+        # determine if Spikes is a list of arrays or a single array
+        if isinstance(Spikes[0], np.ndarray):
             ndim = 2
         else:
             ndim = 1
-    elif isinstance(Spikes, list):
-        kind = 'list'
-        # determine if Spikes is a list of arrays or a single array
-        if isinstance(Spikes[0], np.ndarray):
+
+    elif kind == pd.core.series.Series:
+        if isinstance(Spikes.iloc[0], np.ndarray):
             ndim = 2
         else:
             ndim = 1
-    elif isinstance(Spikes, np.ndarray):
-        kind = 'numpy'
-        ndim = Spikes.ndim
 
     if ndim is None or kind is None:
         raise ValueError("Spikes is not a list, array, or pandas series")
     else:
         return ndim, kind
 
 
-def optimize_alpha_MLE(Spikes, Time, alpha_start=1, alpha_end=10.1, alpha_step=0.1, dt=0.001, ndim=None, kind=None, unitID=None, output_df=True):
+def optimize_alpha_MLE(Spikes, Time, alpha_start=0.01, alpha_end=5, alpha_step=0.01, dt=0.001, ndim=None, kind=None, unitID=None, output_df=True):
     # generate alphas to be optimized over
     alpha_range = np.arange(alpha_start, alpha_end, alpha_step)
     df = None
     best_alpha = None
     best_FiringRate = None
     alphas = []
     loglikes = []
     FiringRates = []
     bandwidths = []
 
-    Time = Time*dt # convert to seconds
     def get_BAKS():
         spiketimes = extract_spike_times(spk, tm)
         for a in alpha_range:
             BAKSrate, h, = BAKS(spiketimes, tm, a)
             ll = firingrate_loglike(spk, BAKSrate)
             alphas.append(a)
             loglikes.append(ll)
@@ -293,20 +315,21 @@
         best_alpha = df.groupby(['alpha'])['log_likelihood'].mean().idxmax()
 
         # get rows from df where alpha == best_alpha
         best_FiringRate = df[df['alpha'] == best_alpha]['BAKSrate']
         if unitID is not None:
             df['unitID'] = unitID
 
-    if kind == 'numpy':
-        best_FiringRate = best_FiringRate.to_numpy()
-        best_FiringRate = np.vstack(best_FiringRate)
-    elif kind == 'list':
+    if kind == np.ndarray:
+        if ndim > 1:
+            best_FiringRate = best_FiringRate.to_numpy()
+            best_FiringRate = np.vstack(best_FiringRate)
+    elif kind == list:
         best_FiringRate = best_FiringRate.to_list()
-    elif kind == 'series':
+    elif kind == pd.core.series.Series:
         action = "do nothing"
     else:
         raise ValueError("Spikes is not a list, array, or pandas series")
 
     if output_df:
         return df, best_FiringRate, best_alpha
     else:
@@ -345,35 +368,38 @@
     :param alpha_start: minimum alpha value to test.
     :param alpha_end: maximum alpha value to test.
     :param alpha_step: step size for alpha values.
     :return: df: pandas dataframe with iternums, MISEs, and alphas
     :return: best_alpha: alpha value with lowest MISE
     """
 
-    if Spikes.ndim == 1:
-        Spikes = Spikes.reshape(1, -1)
-        Time = Time.reshape(1, -1)
+    if Spikes.ndim == 2:
+        Spikes = Spikes.flatten()
+        Time = Time.flatten()
 
     if ws_end is None:
-        ws_end = Time[0, -1] - Time[0, 0]
+        ws_end = Time[-1] - Time[0]
 
-    dt = Time[0, 1] - Time[0, 0]
+    dt = Time[1] - Time[0]
     window_range = np.arange(ws_start, ws_end, ws_step)
 
     iternums = []
     MISEs = []
     windows = []
     likelihoods = []
 
     for iter in range(nIter):
         sim_spikes, sim_rate, sim_time = spikearray_poissonsim(Spikes, Time)
+        sim_spikes = sim_spikes.flatten()
+        sim_rate = sim_rate.flatten()
+        sim_time = sim_time.flatten()
+
         for ws in window_range:
-            rolling_rate, _ = rolling_window(sim_spikes, dt, ws)
-            lh = firingrate_loglike(sim_spikes, rolling_rate)
-            MISE = getMISE(sim_rate, rolling_rate)
+            rolling_rate, lh = rolling_window(sim_spikes, dt, ws)
+            MISE = getMISE(sim_rate, rolling_rate, dt)
             iternums.append(iter)
             MISEs.append(MISE)
             windows.append(ws)
             likelihoods.append(lh)
 
     # make a pandas table with iternums, MISEs, and alphas
     df = pd.DataFrame({'iteration': iternums, 'MISE': MISEs, 'window_size': windows})
```

### Comparing `pyBAKS-0.1.6/pyBAKS.egg-info/CHANGES.txt` & `pyBAKS-0.1.7/pyBAKS.egg-info/CHANGES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-v0.1.6 (2023-12-12)
+v0.1.7 (2024-05-15)
 ----------------------------
--bugfix to dt adjustment in mle optimization
+skipped dist?
 
-v0.1.5 (2023-12-8)
+v0.1.5 (2024-05-15)
 ----------------------------
--small fix
+- fixing issues with LL and MISE calculation
 
 v0.1.4 (2023-12-8)
 ----------------------------
 -fixed overflow error
 -added dt option to BAKS() function to adjust for time arrays not in seconds
 
 v0.1.3 (2023-11-07)
```

