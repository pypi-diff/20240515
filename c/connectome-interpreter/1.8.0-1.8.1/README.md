# Comparing `tmp/connectome_interpreter-1.8.0.tar.gz` & `tmp/connectome_interpreter-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.8.0.tar", last modified: Sat May 11 20:39:56 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.8.1.tar", last modified: Wed May 15 13:24:31 2024, max compression
```

## Comparing `connectome_interpreter-1.8.0.tar` & `connectome_interpreter-1.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 20:39:56.027077 connectome_interpreter-1.8.0/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.8.0/LICENSE
--rw-rw-rw-   0        0        0     1066 2024-05-11 20:39:56.026082 connectome_interpreter-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.8.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 20:39:55.973568 connectome_interpreter-1.8.0/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.8.0/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    36418 2024-05-11 20:34:13.000000 connectome_interpreter-1.8.0/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    22584 2024-05-06 14:40:18.000000 connectome_interpreter-1.8.0/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    16221 2024-05-07 10:46:28.000000 connectome_interpreter-1.8.0/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    35523 2024-05-06 21:27:16.000000 connectome_interpreter-1.8.0/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-11 20:39:56.012791 connectome_interpreter-1.8.0/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0     1066 2024-05-11 20:39:55.000000 connectome_interpreter-1.8.0/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-05-11 20:39:55.000000 connectome_interpreter-1.8.0/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 20:39:55.000000 connectome_interpreter-1.8.0/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-05-11 20:39:55.000000 connectome_interpreter-1.8.0/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-11 20:39:55.000000 connectome_interpreter-1.8.0/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 20:39:56.027077 connectome_interpreter-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0     2068 2024-05-06 14:43:28.000000 connectome_interpreter-1.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 20:39:56.023090 connectome_interpreter-1.8.0/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.8.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.8.0/tests/test_compress_paths.py
--rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.8.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:24:31.139007 connectome_interpreter-1.8.1/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.8.1/LICENSE
+-rw-rw-rw-   0        0        0     1066 2024-05-15 13:24:31.137919 connectome_interpreter-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 13:24:31.069807 connectome_interpreter-1.8.1/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.8.1/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    36418 2024-05-11 20:34:13.000000 connectome_interpreter-1.8.1/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    22758 2024-05-15 13:20:48.000000 connectome_interpreter-1.8.1/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    16221 2024-05-07 10:46:28.000000 connectome_interpreter-1.8.1/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    35703 2024-05-15 13:17:34.000000 connectome_interpreter-1.8.1/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:24:31.113193 connectome_interpreter-1.8.1/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0     1066 2024-05-15 13:24:30.000000 connectome_interpreter-1.8.1/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-05-15 13:24:30.000000 connectome_interpreter-1.8.1/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 13:24:30.000000 connectome_interpreter-1.8.1/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-05-15 13:24:30.000000 connectome_interpreter-1.8.1/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-15 13:24:30.000000 connectome_interpreter-1.8.1/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 13:24:31.139007 connectome_interpreter-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     2068 2024-05-15 13:20:58.000000 connectome_interpreter-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:24:31.135929 connectome_interpreter-1.8.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.8.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.8.1/tests/test_compress_paths.py
+-rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.8.1/tests/test_utils.py
```

### Comparing `connectome_interpreter-1.8.0/LICENSE` & `connectome_interpreter-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.0/PKG-INFO` & `connectome_interpreter-1.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome_interpreter
-Version: 1.8.0
+Version: 1.8.1
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
```

### Comparing `connectome_interpreter-1.8.0/README.md` & `connectome_interpreter-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.0/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.8.1/connectome_interpreter/activation_maximisation.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.0/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.8.1/connectome_interpreter/compress_paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .utils import dynamic_representation, torch_sparse_where, to_nparray, tensor_to_csc
 
 
 def compress_paths(inprop, step_number, threshold=0, output_threshold=1e-4, root=False):
     """
     Performs iterative multiplication of a sparse matrix `inprop` for a specified number of steps, 
     applying thresholding to filter out values below a certain `threshold` to optimize memory usage 
-    and computation speed. The function is optimized to run on GPU if available. 
+    and computation speed. The function is optimized to run on GPU if available. It needs >= size_of_inprop * 3 amount of GPU memory, for matrix multiplication, and thresholding. 
 
     This function multiplies the connectivity matrix (input in rows; output in columns) `inprop` with itself `step_number` times, 
     with each step's result being thresholded to zero out elements below a given threshold. 
     The function stores each step's result in a list, where each result is further 
     processed to drop values below the `output_threshold` to save memory.
 
     Args:
@@ -52,40 +52,41 @@
         >>> print(compressed_paths)
     """
     steps_fast = []
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     inprop_tensor = torch.tensor(inprop.toarray(), device=device)
 
-    for i in tqdm(range(step_number)):
-        if i == 0:
-            out_tensor = inprop_tensor
-        else:
-            out_tensor = torch.matmul(out_tensor, inprop_tensor)
-
-        # Thresholding during matmul
-        if threshold != 0:
-            out_tensor = torch.where(
-                out_tensor >= threshold, out_tensor, torch.tensor(0.0, device=device))
-        # Dynamic representation based on density
-        # out_tensor = dynamic_representation(out_tensor)
-
-        if root:
-            out_csc = torch.pow(out_tensor, 1/(i+1))
-        else:
-            out_csc = out_tensor.clone()
-
-        if output_threshold > 0:
-            out_csc = torch_sparse_where(out_csc, output_threshold)
-        out_csc = tensor_to_csc(out_csc.to('cpu'))
-        out_csc.eliminate_zeros()
+    with torch.no_grad():
+        for i in tqdm(range(step_number)):
+            if i == 0:
+                out_tensor = inprop_tensor.clone()
+            else:
+                out_tensor = torch.matmul(out_tensor, inprop_tensor)
+
+            # Thresholding during matmul
+            if threshold != 0:
+                out_tensor = torch.where(
+                    out_tensor >= threshold, out_tensor, torch.tensor(0.0, device=device))
+
+            # Convert to csc for output
+            out_csc = tensor_to_csc(out_tensor.to('cpu'))
+            out_csc.eliminate_zeros()
+
+            if root:
+                out_csc.data = np.power(out_csc.data, 1/(i+1))
+
+            if output_threshold > 0:
+                out_csc.data = np.where(
+                    out_csc.data >= output_threshold, out_csc.data, 0)
+                out_csc.eliminate_zeros()
 
-        steps_fast.append(out_csc)
+            steps_fast.append(out_csc)
+            torch.cuda.empty_cache()
 
-    torch.cuda.empty_cache()
     return steps_fast
 
 
 def compress_paths_signed(inprop, idx_to_sign, target_layer_number, threshold=0, output_threshold=1e-4, root=False):
     """
     Calculates the excitatory and inhibitory influences across specified layers of a neural network, using PyTorch for GPU acceleration. This function processes a connectivity matrix (where presynaptic neurons are represented by rows and postsynaptic neurons by columns) to distinguish and compute the influence of excitatory and inhibitory neurons at each layer.
```

### Comparing `connectome_interpreter-1.8.0/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.8.1/connectome_interpreter/path_finding.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.0/connectome_interpreter/utils.py` & `connectome_interpreter-1.8.1/connectome_interpreter/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,19 @@
 import matplotlib.colors as mcl
 import matplotlib.pyplot as plt
 from tqdm import tqdm
 import networkx as nx
 
 
 def dynamic_representation(tensor, density_threshold=0.2):
-    """Convert tensor to sparse if density is below threshold, otherwise to dense."""
-    nonzero_elements = torch.nonzero(tensor).size(0)
+    """Convert tensor to sparse if density is below threshold, otherwise to dense. This might be memory intensive."""
+    # nonzero_elements = torch.nonzero(tensor).size(0)
+    # .nonzero() doesn't work if the tensor has more than INT_MAX elements
+    # Calculate the number of non-zero elements without using torch.nonzero()
+    nonzero_elements = tensor.count_nonzero().item()
 
     # to_sparse() doesn't support operations on tensors with more than INT_MAX (2,147,483,647) elements
     if nonzero_elements < 2147483647:
         total_elements = tensor.numel()
         density = nonzero_elements / total_elements
 
         if density < density_threshold:
@@ -72,20 +75,18 @@
     if tensor.is_sparse:
         tensor = tensor.coalesce()
         indices = tensor.indices().numpy()
         values = tensor.values().numpy()
         shape = tensor.shape
         coo = coo_matrix((values, (indices[0], indices[1])), shape=shape)
     else:
-        # Convert dense tensor to COO directly, necessary if the tensor is not sparse
-        indices = torch.nonzero(tensor).t()
-        values = tensor[indices[0], indices[1]]
-        shape = tensor.shape
-        coo = coo_matrix(
-            (values.numpy(), (indices[0].numpy(), indices[1].numpy())), shape=shape)
+        coo = coo_matrix(tensor.numpy())
+        coo.eliminate_zeros()
+        # .nonzero() is too memory consuming for large tensors
+        # memory usage can be further reduced by first spliting the tensor/COO matrix into smaller chunks, for future work
 
     return coo.tocsc()
 
 
 def coo_tensor_to_el(coo_tensor):
     """
     Convert a PyTorch sparse COO tensor to a DataFrame representing an edge list.
```

### Comparing `connectome_interpreter-1.8.0/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.8.1/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome-interpreter
-Version: 1.8.0
+Version: 1.8.1
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
```

### Comparing `connectome_interpreter-1.8.0/connectome_interpreter.egg-info/SOURCES.txt` & `connectome_interpreter-1.8.1/connectome_interpreter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.0/setup.py` & `connectome_interpreter-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.8.0',
+    version='1.8.1',
     packages=find_packages(),
     install_requires=install_requires_list,
     extras_require={
         'get_ngl_link': ['nglscenes'],
         'wandb': ['wandb'],
     },
     # Optional metadata
```

### Comparing `connectome_interpreter-1.8.0/tests/test_compress_paths.py` & `connectome_interpreter-1.8.1/tests/test_compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.0/tests/test_utils.py` & `connectome_interpreter-1.8.1/tests/test_utils.py`

 * *Files identical despite different names*

