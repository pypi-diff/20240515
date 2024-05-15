# Comparing `tmp/rvit-1.0.2.tar.gz` & `tmp/rvit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rvit-1.0.2.tar", last modified: Wed May  8 13:51:03 2024, max compression
+gzip compressed data, was "rvit-1.0.3.tar", last modified: Wed May 15 16:27:06 2024, max compression
```

## Comparing `rvit-1.0.2.tar` & `rvit-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:51:03.902834 rvit-1.0.2/
--rw-rw-rw-   0        0        0     1135 2024-05-08 13:51:03.901834 rvit-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      559 2024-05-08 12:21:15.000000 rvit-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 13:51:03.891834 rvit-1.0.2/rvit/
--rw-rw-rw-   0        0        0       74 2024-05-08 12:24:16.000000 rvit-1.0.2/rvit/__init__.py
--rw-rw-rw-   0        0        0     3740 2024-05-08 12:00:48.000000 rvit-1.0.2/rvit/registered_vision_transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:51:03.901834 rvit-1.0.2/rvit.egg-info/
--rw-rw-rw-   0        0        0     1135 2024-05-08 13:51:03.000000 rvit-1.0.2/rvit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-08 13:51:03.000000 rvit-1.0.2/rvit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:51:03.000000 rvit-1.0.2/rvit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-08 13:51:03.000000 rvit-1.0.2/rvit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-08 13:51:03.000000 rvit-1.0.2/rvit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 13:51:03.902834 rvit-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1048 2024-05-08 13:50:48.000000 rvit-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:27:06.886599 rvit-1.0.3/
+-rw-rw-rw-   0        0        0     1135 2024-05-15 16:27:06.886599 rvit-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2024-05-08 12:21:15.000000 rvit-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 16:27:06.875089 rvit-1.0.3/rvit/
+-rw-rw-rw-   0        0        0       74 2024-05-08 12:24:16.000000 rvit-1.0.3/rvit/__init__.py
+-rw-rw-rw-   0        0        0     3803 2024-05-15 16:25:11.000000 rvit-1.0.3/rvit/registered_vision_transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:27:06.885599 rvit-1.0.3/rvit.egg-info/
+-rw-rw-rw-   0        0        0     1135 2024-05-15 16:27:06.000000 rvit-1.0.3/rvit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-15 16:27:06.000000 rvit-1.0.3/rvit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 16:27:06.000000 rvit-1.0.3/rvit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-15 16:27:06.000000 rvit-1.0.3/rvit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-15 16:27:06.000000 rvit-1.0.3/rvit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 16:27:06.887600 rvit-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1048 2024-05-15 16:25:40.000000 rvit-1.0.3/setup.py
```

### Comparing `rvit-1.0.2/PKG-INFO` & `rvit-1.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rvit
-Version: 1.0.2
+Version: 1.0.3
 Summary: Vision Transformer with Registers
 Author: Joe Griffith
 Author-email: <joeagriffith@gmail.com
 Keywords: python,pytorch,vision transformer,register,registers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rvit-1.0.2/README.md` & `rvit-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rvit-1.0.2/rvit/registered_vision_transformer.py` & `rvit-1.0.3/rvit/registered_vision_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,17 @@
     def forward(self, input: torch.Tensor):
         torch._assert(input.dim() == 3, f"Expected (batch_size, seq_length, hidden_dim) got {input.shape}")
         input = input + self.pos_embedding
         # add registers to input, without positional embedding
         input = torch.cat([input, self.registers.expand(input.size(0), -1, -1)], dim=1)
         output = self.ln(self.layers(self.dropout(input)))
         # return output, excluding the registers
-        return output[:, :-self.num_registers, :]
+        if self.num_registers > 0:
+            output = output[:, :-self.num_registers, :]
+        return output
 
 
 class RegisteredVisionTransformer(VisionTransformer):
     """Registered Vision Transformer. Essentially equivalent to https://arxiv.org/abs/2010.11929, except with registers in the encoder."""
 
     def __init__(
         self,
```

### Comparing `rvit-1.0.2/rvit.egg-info/PKG-INFO` & `rvit-1.0.3/rvit.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rvit
-Version: 1.0.2
+Version: 1.0.3
 Summary: Vision Transformer with Registers
 Author: Joe Griffith
 Author-email: <joeagriffith@gmail.com
 Keywords: python,pytorch,vision transformer,register,registers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rvit-1.0.2/setup.py` & `rvit-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'Vision Transformer with Registers'
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="rvit",
     version=VERSION,
```

