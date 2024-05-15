# Comparing `tmp/rapid_paraformer-2.0.4-py3-none-any.whl.zip` & `tmp/rapid_paraformer-2.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20841 bytes, number of entries: 13
--rw-r--r--  2.0 unx      120 b- defN 23-Aug-21 01:58 rapid_paraformer/__init__.py
--rw-r--r--  2.0 unx     4925 b- defN 23-Aug-21 01:58 rapid_paraformer/rapid_paraformer.py
--rw-r--r--  2.0 unx    12750 b- defN 23-Aug-21 01:58 rapid_paraformer/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-21 01:58 rapid_paraformer/kaldifeat/LICENSE
--rw-r--r--  2.0 unx     7414 b- defN 23-Aug-21 01:58 rapid_paraformer/kaldifeat/README.md
--rw-r--r--  2.0 unx      140 b- defN 23-Aug-21 01:58 rapid_paraformer/kaldifeat/__init__.py
--rw-r--r--  2.0 unx    18708 b- defN 23-Aug-21 01:58 rapid_paraformer/kaldifeat/feature.py
--rw-r--r--  2.0 unx     2194 b- defN 23-Aug-21 01:58 rapid_paraformer/kaldifeat/ivector.py
--rw-r--r--  2.0 unx     2551 b- defN 23-Aug-21 01:59 rapid_paraformer-2.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-21 01:59 rapid_paraformer-2.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 23-Aug-21 01:59 rapid_paraformer-2.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       44 b- defN 23-Aug-21 01:59 rapid_paraformer-2.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1166 b- defN 23-Aug-21 01:59 rapid_paraformer-2.0.4.dist-info/RECORD
-13 files, 61526 bytes uncompressed, 18863 bytes compressed:  69.3%
+Zip file size: 20483 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      145 b- defN 24-May-15 04:52 rapid_paraformer/__init__.py
+-rw-r--r--  2.0 unx     4925 b- defN 24-May-15 04:52 rapid_paraformer/main.py
+-rw-r--r--  2.0 unx    13206 b- defN 24-May-15 04:52 rapid_paraformer/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-15 04:52 rapid_paraformer/kaldifeat/LICENSE
+-rw-r--r--  2.0 unx     7414 b- defN 24-May-15 04:52 rapid_paraformer/kaldifeat/README.md
+-rw-r--r--  2.0 unx      140 b- defN 24-May-15 04:52 rapid_paraformer/kaldifeat/__init__.py
+-rw-r--r--  2.0 unx    19143 b- defN 24-May-15 04:52 rapid_paraformer/kaldifeat/feature.py
+-rw-r--r--  2.0 unx     2194 b- defN 24-May-15 04:52 rapid_paraformer/kaldifeat/ivector.py
+-rw-r--r--  2.0 unx      895 b- defN 24-May-15 04:53 rapid_paraformer-2.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-15 04:53 rapid_paraformer-2.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 24-May-15 04:53 rapid_paraformer-2.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       44 b- defN 24-May-15 04:53 rapid_paraformer-2.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1153 b- defN 24-May-15 04:53 rapid_paraformer-2.0.5.dist-info/RECORD
+13 files, 60773 bytes uncompressed, 18529 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: rapid_paraformer/__init__.py
 Comment: 
 
-Filename: rapid_paraformer/rapid_paraformer.py
+Filename: rapid_paraformer/main.py
 Comment: 
 
 Filename: rapid_paraformer/utils.py
 Comment: 
 
 Filename: rapid_paraformer/kaldifeat/LICENSE
 Comment: 
@@ -18,23 +18,23 @@
 
 Filename: rapid_paraformer/kaldifeat/feature.py
 Comment: 
 
 Filename: rapid_paraformer/kaldifeat/ivector.py
 Comment: 
 
-Filename: rapid_paraformer-2.0.4.dist-info/METADATA
+Filename: rapid_paraformer-2.0.5.dist-info/METADATA
 Comment: 
 
-Filename: rapid_paraformer-2.0.4.dist-info/WHEEL
+Filename: rapid_paraformer-2.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_paraformer-2.0.4.dist-info/entry_points.txt
+Filename: rapid_paraformer-2.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_paraformer-2.0.4.dist-info/top_level.txt
+Filename: rapid_paraformer-2.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_paraformer-2.0.4.dist-info/RECORD
+Filename: rapid_paraformer-2.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_paraformer/__init__.py

```diff
@@ -1,4 +1,5 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
-from .rapid_paraformer import RapidParaformer
+from .main import RapidParaformer
+from .utils import download_hf_model
```

## rapid_paraformer/utils.py

```diff
@@ -6,14 +6,15 @@
 import pickle
 import warnings
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, NamedTuple, Set, Tuple, Union
 
 import numpy as np
 import yaml
+from huggingface_hub import snapshot_download
 from onnxruntime import (
     GraphOptimizationLevel,
     InferenceSession,
     SessionOptions,
     get_available_providers,
     get_device,
 )
@@ -217,16 +218,16 @@
 
     def apply_cmvn(self, inputs: np.ndarray) -> np.ndarray:
         """
         Apply CMVN with mvn data
         """
         frame, dim = inputs.shape
         means = np.tile(self.cmvn[0:1, :dim], (frame, 1))
-        vars = np.tile(self.cmvn[1:2, :dim], (frame, 1))
-        inputs = (inputs + means) * vars
+        vars_np = np.tile(self.cmvn[1:2, :dim], (frame, 1))
+        inputs = (inputs + means) * vars_np
         return inputs
 
     def load_cmvn(
         self,
     ) -> np.ndarray:
         with open(self.cmvn_file, "r", encoding="utf-8") as f:
             lines = f.readlines()
@@ -245,16 +246,16 @@
                 line_item = lines[i + 1].split()
                 if line_item[0] == "<LearnRateCoef>":
                     rescale_line = line_item[3 : (len(line_item) - 1)]
                     vars_list = list(rescale_line)
                     continue
 
         means = np.array(means_list).astype(np.float64)
-        vars = np.array(vars_list).astype(np.float64)
-        cmvn = np.array([means, vars])
+        vars_np = np.array(vars_list).astype(np.float64)
+        cmvn = np.array([means, vars_np])
         return cmvn
 
 
 class Hypothesis(NamedTuple):
     """Hypothesis data type."""
 
     yseq: np.ndarray
@@ -271,18 +272,14 @@
         )._asdict()
 
 
 class TokenIDConverterError(Exception):
     pass
 
 
-class ONNXRuntimeError(Exception):
-    pass
-
-
 class OrtInferSession:
     def __init__(self, config):
         sess_opt = SessionOptions()
         sess_opt.log_severity_level = 4
         sess_opt.enable_cpu_mem_arena = False
         sess_opt.graph_optimization_level = GraphOptimizationLevel.ORT_ENABLE_ALL
 
@@ -347,14 +344,18 @@
         model_path = Path(model_path)
         if not model_path.exists():
             raise FileNotFoundError(f"{model_path} does not exists.")
         if not model_path.is_file():
             raise FileExistsError(f"{model_path} is not a file.")
 
 
+class ONNXRuntimeError(Exception):
+    pass
+
+
 def read_yaml(yaml_path: Union[str, Path]) -> Dict:
     if not Path(yaml_path).exists():
         raise FileExistsError(f"The {yaml_path} does not exist.")
 
     with open(str(yaml_path), "rb") as f:
         data = yaml.load(f, Loader=yaml.Loader)
     return data
@@ -386,7 +387,23 @@
 
     sh = logging.StreamHandler()
     sh.setFormatter(formatter)
     logger.addHandler(sh)
     logger_initialized[name] = True
     logger.propagate = False
     return logger
+
+
+def download_hf_model(
+    repo_id: str, save_dir: Union[str, Path], resume_download: bool = True
+) -> str:
+    model_dir = snapshot_download(
+        repo_id=repo_id,
+        local_dir=str(save_dir),
+        local_dir_use_symlinks=False,
+        local_files_only=False,
+        resume_download=resume_download,
+        ignore_patterns=[
+            "*.md",
+        ],
+    )
+    return model_dir
```

## rapid_paraformer/kaldifeat/feature.py

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-from scipy.fftpack import dct
 
 
 # ---------- feature-window ----------
 
 def sliding_window(x, window_size, window_shift):
     shape = x.shape[:-1] + (x.shape[-1] - window_size + 1, window_size)
     strides = x.strides + (x.strides[-1],)
@@ -133,14 +132,36 @@
     return frames, log_enery
 
 # ---------- feature-window ----------
 
 
 # ---------- feature-functions ----------
 
+def dct_np(x: np.array, norm=None):
+    x_shape = x.shape
+    N = x_shape[-1]
+
+    v = np.hstack([x[:, ::2], x[:, 1::2][:, ::-1]])
+    Vc = np.fft.fft(v)
+    Vc = np.dstack([np.real(Vc), np.imag(Vc)])
+
+    k = - np.arange(N, dtype=x.dtype)[None, :] * np.pi / (2*N)
+    W_r = np.cos(k)
+    W_i = np.sin(k)
+
+    V = Vc[:, :, 0] * W_r - Vc[:, :, 1] * W_i
+
+    if norm == "ortho":
+        V[:, 0] /= np.sqrt(N) * 2
+        V[:, 1:] /= np.sqrt(N/2) * 2
+
+    V = 2 * V
+    return V
+
+
 def compute_spectrum(frames, n):
     complex_spec = np.fft.rfft(frames, n)
     return np.absolute(complex_spec)
 
 
 def compute_power_spectrum(frames, n):
     return np.square(compute_spectrum(frames, n))
@@ -420,15 +441,15 @@
         snip_edges=snip_edges,
         use_energy=use_energy,
         use_log_fbank=True,
         use_power=True,
         window_type=window_type,
         dtype=dtype
     )
-    feat = dct(feat, type=2, axis=1, norm='ortho')[:, :num_ceps]
+    feat = dct_np(feat, norm="ortho")[:, :num_ceps]
     lifter_coeffs = compute_lifter_coeffs(cepstral_lifter, num_ceps).astype(dtype)
     feat = feat * lifter_coeffs
     if use_energy:
         feat[:, 0] = log_energy
     return feat
 
 # ---------- compute-mfcc-feats ----------
```

## Comparing `rapid_paraformer/rapid_paraformer.py` & `rapid_paraformer/main.py`

 * *Files identical despite different names*

## Comparing `rapid_paraformer-2.0.4.dist-info/RECORD` & `rapid_paraformer-2.0.5.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-rapid_paraformer/__init__.py,sha256=k7vOI_IwHBr7EULwI9ya593U4H5QTKdC-i4VYX0dOv4,120
-rapid_paraformer/rapid_paraformer.py,sha256=edH3QtEvlN4RfcKZeUgB_60cirgJuU3ruqE4l1xXmiY,4925
-rapid_paraformer/utils.py,sha256=Axkt8w0SQpCIaZlKWaTpT5Mw9Wu2b-1aV3Aeb_PIG_w,12750
+rapid_paraformer/__init__.py,sha256=25x45OLlLsEpxAZLOoN6hcpP_uox0Lat2_qoSC_jpKo,145
+rapid_paraformer/main.py,sha256=edH3QtEvlN4RfcKZeUgB_60cirgJuU3ruqE4l1xXmiY,4925
+rapid_paraformer/utils.py,sha256=hCnFA5bhVeuDncYFsVgB99ieU5bs1ZUXcPkvNg4kIPw,13206
 rapid_paraformer/kaldifeat/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
 rapid_paraformer/kaldifeat/README.md,sha256=brMJBou-ew86SElkjOL3eegRbTEVpMp0tAttPOPan-0,7414
 rapid_paraformer/kaldifeat/__init__.py,sha256=3YX1QXUS1tqDXQsH15BxHEOdI0HY8_R29xwpOe8tKsM,140
-rapid_paraformer/kaldifeat/feature.py,sha256=hu5cbkpH1601trCYMOyIQJeJs56GxwAXwxHlu0P3ztc,18708
+rapid_paraformer/kaldifeat/feature.py,sha256=nKoa2JWk8DM5gTJHnnExKg9p862oyDj2l4h3UDN-S-c,19143
 rapid_paraformer/kaldifeat/ivector.py,sha256=DAIVOb4FWtgEsw3y99frxf0K1umV0ArF0QLd3x4d44U,2194
-rapid_paraformer-2.0.4.dist-info/METADATA,sha256=Y-zI4t-s9bFgPbF-kFoGrJ8AGpVRxDfLnIEB6bM30ec,2551
-rapid_paraformer-2.0.4.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
-rapid_paraformer-2.0.4.dist-info/entry_points.txt,sha256=aDpI5rhSI_DYR6n29CXEr2zCaTuCbYYEZvmERxG2tMU,65
-rapid_paraformer-2.0.4.dist-info/top_level.txt,sha256=CReApSWSM8eVpJXcVZU2PGTsAVR_SN4OL9qcVtfYF1g,44
-rapid_paraformer-2.0.4.dist-info/RECORD,,
+rapid_paraformer-2.0.5.dist-info/METADATA,sha256=sDT_iEys8wAB7wfL_1g1FQQOEeFwj-Gh3Hph5y4AfJE,895
+rapid_paraformer-2.0.5.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+rapid_paraformer-2.0.5.dist-info/entry_points.txt,sha256=aDpI5rhSI_DYR6n29CXEr2zCaTuCbYYEZvmERxG2tMU,65
+rapid_paraformer-2.0.5.dist-info/top_level.txt,sha256=CReApSWSM8eVpJXcVZU2PGTsAVR_SN4OL9qcVtfYF1g,44
+rapid_paraformer-2.0.5.dist-info/RECORD,,
```

