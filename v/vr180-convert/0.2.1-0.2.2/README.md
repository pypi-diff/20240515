# Comparing `tmp/vr180_convert-0.2.1.tar.gz` & `tmp/vr180_convert-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vr180_convert-0.2.1.tar", max compression
+gzip compressed data, was "vr180_convert-0.2.2.tar", max compression
```

## Comparing `vr180_convert-0.2.1.tar` & `vr180_convert-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2024-05-11 03:21:10.758015 vr180_convert-0.2.1/LICENSE
--rw-r--r--   0        0        0    10741 2024-05-11 03:21:10.758015 vr180_convert-0.2.1/README.md
--rw-r--r--   0        0        0     3836 2024-05-11 03:21:11.642016 vr180_convert-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      707 2024-05-11 03:21:11.642016 vr180_convert-0.2.1/src/vr180_convert/__init__.py
--rw-r--r--   0        0        0      113 2024-05-11 03:21:10.774015 vr180_convert-0.2.1/src/vr180_convert/__main__.py
--rw-r--r--   0        0        0    12817 2024-05-11 03:21:10.774015 vr180_convert-0.2.1/src/vr180_convert/cli.py
--rw-r--r--   0        0        0        0 2024-05-11 03:21:10.774015 vr180_convert-0.2.1/src/vr180_convert/py.typed
--rw-r--r--   0        0        0    12090 2024-05-11 03:21:10.774015 vr180_convert-0.2.1/src/vr180_convert/remapper.py
--rw-r--r--   0        0        0     1889 2024-05-11 03:21:10.774015 vr180_convert-0.2.1/src/vr180_convert/testing.py
--rw-r--r--   0        0        0    18069 2024-05-11 03:21:10.774015 vr180_convert-0.2.1/src/vr180_convert/transformer.py
--rw-r--r--   0        0        0    12139 1970-01-01 00:00:00.000000 vr180_convert-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-15 03:22:30.419482 vr180_convert-0.2.2/LICENSE
+-rw-r--r--   0        0        0    10741 2024-05-15 03:22:30.419482 vr180_convert-0.2.2/README.md
+-rw-r--r--   0        0        0     3837 2024-05-15 03:22:31.855484 vr180_convert-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      707 2024-05-15 03:22:31.855484 vr180_convert-0.2.2/src/vr180_convert/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-15 03:22:30.435482 vr180_convert-0.2.2/src/vr180_convert/__main__.py
+-rw-r--r--   0        0        0    12817 2024-05-15 03:22:30.435482 vr180_convert-0.2.2/src/vr180_convert/cli.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:22:30.435482 vr180_convert-0.2.2/src/vr180_convert/py.typed
+-rw-r--r--   0        0        0    12090 2024-05-15 03:22:30.435482 vr180_convert-0.2.2/src/vr180_convert/remapper.py
+-rw-r--r--   0        0        0     1889 2024-05-15 03:22:30.435482 vr180_convert-0.2.2/src/vr180_convert/testing.py
+-rw-r--r--   0        0        0    18069 2024-05-15 03:22:30.435482 vr180_convert-0.2.2/src/vr180_convert/transformer.py
+-rw-r--r--   0        0        0    12140 1970-01-01 00:00:00.000000 vr180_convert-0.2.2/PKG-INFO
```

### Comparing `vr180_convert-0.2.1/LICENSE` & `vr180_convert-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.1/README.md` & `vr180_convert-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.1/pyproject.toml` & `vr180_convert-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vr180-convert"
-version = "0.2.1"
+version = "0.2.2"
 description = "Simple VR180 image converter"
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/vr180-convert"
 documentation = "https://vr180-convert.readthedocs.io"
 classifiers = [
@@ -25,15 +25,15 @@
 [tool.poetry.scripts]
 vr180-convert = "vr180_convert.cli:app"
 v1c = "vr180_convert.cli:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = ">=10"
-typer = {extras = ["all"], version = "^0.9.0"}
+typer = {extras = ["all"], version = "^0.12.0"}
 opencv-python = "^4.9.0.80"
 attrs = "^23.2.0"
 scikit-learn = "^1.4.2"
 numpy-quaternion = "^2023.0.3"
 strenum = "^0.4.15"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `vr180_convert-0.2.1/src/vr180_convert/__init__.py` & `vr180_convert-0.2.2/src/vr180_convert/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 from .remapper import apply, apply_lr, get_map
 from .transformer import (
     DenormalizeTransformer,
     EquirectangularEncoder,
     Euclidean3DRotator,
     Euclidean3DTransformer,
     FisheyeDecoder,
```

### Comparing `vr180_convert-0.2.1/src/vr180_convert/cli.py` & `vr180_convert-0.2.2/src/vr180_convert/cli.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.1/src/vr180_convert/remapper.py` & `vr180_convert-0.2.2/src/vr180_convert/remapper.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.1/src/vr180_convert/testing.py` & `vr180_convert-0.2.2/src/vr180_convert/testing.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.1/src/vr180_convert/transformer.py` & `vr180_convert-0.2.2/src/vr180_convert/transformer.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.1/PKG-INFO` & `vr180_convert-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vr180-convert
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple VR180 image converter
 Home-page: https://github.com/34j/vr180-convert
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -20,15 +20,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: attrs (>=23.2.0,<24.0.0)
 Requires-Dist: numpy-quaternion (>=2023.0.3,<2024.0.0)
 Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: rich (>=10)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Requires-Dist: strenum (>=0.4.15,<0.5.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: typer[all] (>=0.12.0,<0.13.0)
 Project-URL: Bug Tracker, https://github.com/34j/vr180-convert/issues
 Project-URL: Changelog, https://github.com/34j/vr180-convert/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://vr180-convert.readthedocs.io
 Project-URL: Repository, https://github.com/34j/vr180-convert
 Description-Content-Type: text/markdown
 
 # VR180 image converter
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: vr180-convert Version: 0.2.1 Summary: Simple VR180
+Metadata-Version: 2.1 Name: vr180-convert Version: 0.2.2 Summary: Simple VR180
 image converter Home-page: https://github.com/34j/vr180-convert License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Topic :: Software Development ::
 Libraries Requires-Dist: attrs (>=23.2.0,<24.0.0) Requires-Dist: numpy-
 quaternion (>=2023.0.3,<2024.0.0) Requires-Dist: opencv-python
 (>=4.9.0.80,<5.0.0.0) Requires-Dist: rich (>=10) Requires-Dist: scikit-learn
 (>=1.4.2,<2.0.0) Requires-Dist: strenum (>=0.4.15,<0.5.0) Requires-Dist: typer
-[all] (>=0.9.0,<0.10.0) Project-URL: Bug Tracker, https://github.com/34j/vr180-
-convert/issues Project-URL: Changelog, https://github.com/34j/vr180-convert/
-blob/main/CHANGELOG.md Project-URL: Documentation, https://vr180-
+[all] (>=0.12.0,<0.13.0) Project-URL: Bug Tracker, https://github.com/34j/
+vr180-convert/issues Project-URL: Changelog, https://github.com/34j/vr180-
+convert/blob/main/CHANGELOG.md Project-URL: Documentation, https://vr180-
 convert.readthedocs.io Project-URL: Repository, https://github.com/34j/vr180-
 convert Description-Content-Type: text/markdown # VR180 image converter
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 --- **Documentation**: _h_t_t_p_s_:_/_/_v_r_1_8_0_-_c_o_n_v_e_r_t_._r_e_a_d_t_h_e_d_o_c_s_._i_o_ **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_3_4_j_/_v_r_1_8_0_-_c_o_n_v_e_r_t_ --- Simple VR180 image converter on top of
```

