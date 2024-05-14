# Comparing `tmp/meshgpt_pytorch-1.2.4.tar.gz` & `tmp/meshgpt_pytorch-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshgpt_pytorch-1.2.4.tar", last modified: Sat May 11 02:47:40 2024, max compression
+gzip compressed data, was "meshgpt_pytorch-1.2.5.tar", last modified: Tue May 14 01:21:02 2024, max compression
```

## Comparing `meshgpt_pytorch-1.2.4.tar` & `meshgpt_pytorch-1.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:47:40.515194 meshgpt_pytorch-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-11 02:47:36.000000 meshgpt_pytorch-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-11 02:47:40.515194 meshgpt_pytorch-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-05-11 02:47:36.000000 meshgpt_pytorch-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:47:40.515194 meshgpt_pytorch-1.2.4/meshgpt_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-11 02:47:36.000000 meshgpt_pytorch-1.2.4/meshgpt_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-11 02:47:36.000000 meshgpt_pytorch-1.2.4/meshgpt_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    50136 2024-05-11 02:47:36.000000 meshgpt_pytorch-1.2.4/meshgpt_pytorch/meshgpt_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-11 02:47:36.000000 meshgpt_pytorch-1.2.4/meshgpt_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 02:47:36.000000 meshgpt_pytorch-1.2.4/meshgpt_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:47:40.515194 meshgpt_pytorch-1.2.4/meshgpt_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-11 02:47:40.000000 meshgpt_pytorch-1.2.4/meshgpt_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-11 02:47:40.000000 meshgpt_pytorch-1.2.4/meshgpt_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:47:40.000000 meshgpt_pytorch-1.2.4/meshgpt_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-11 02:47:40.000000 meshgpt_pytorch-1.2.4/meshgpt_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 02:47:40.000000 meshgpt_pytorch-1.2.4/meshgpt_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:47:40.515194 meshgpt_pytorch-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-11 02:47:36.000000 meshgpt_pytorch-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:21:02.350578 meshgpt_pytorch-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-14 01:20:58.000000 meshgpt_pytorch-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-14 01:21:02.350578 meshgpt_pytorch-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-05-14 01:20:58.000000 meshgpt_pytorch-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:21:02.346578 meshgpt_pytorch-1.2.5/meshgpt_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 01:20:58.000000 meshgpt_pytorch-1.2.5/meshgpt_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-14 01:20:58.000000 meshgpt_pytorch-1.2.5/meshgpt_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50617 2024-05-14 01:20:58.000000 meshgpt_pytorch-1.2.5/meshgpt_pytorch/meshgpt_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-14 01:20:58.000000 meshgpt_pytorch-1.2.5/meshgpt_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 01:20:58.000000 meshgpt_pytorch-1.2.5/meshgpt_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:21:02.346578 meshgpt_pytorch-1.2.5/meshgpt_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-14 01:21:02.000000 meshgpt_pytorch-1.2.5/meshgpt_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-14 01:21:02.000000 meshgpt_pytorch-1.2.5/meshgpt_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 01:21:02.000000 meshgpt_pytorch-1.2.5/meshgpt_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-14 01:21:02.000000 meshgpt_pytorch-1.2.5/meshgpt_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:21:02.000000 meshgpt_pytorch-1.2.5/meshgpt_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:21:02.350578 meshgpt_pytorch-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-14 01:20:58.000000 meshgpt_pytorch-1.2.5/setup.py
```

### Comparing `meshgpt_pytorch-1.2.4/LICENSE` & `meshgpt_pytorch-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.4/PKG-INFO` & `meshgpt_pytorch-1.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.4
+Version: 1.2.5
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshgpt_pytorch-1.2.4/README.md` & `meshgpt_pytorch-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.4/meshgpt_pytorch/data.py` & `meshgpt_pytorch-1.2.5/meshgpt_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.4/meshgpt_pytorch/meshgpt_pytorch.py` & `meshgpt_pytorch-1.2.5/meshgpt_pytorch/meshgpt_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1034,18 +1034,19 @@
         coarse_pre_gateloop_depth = 2,
         fine_pre_gateloop_depth = 2,
         gateloop_use_heinsen = False,
         fine_attn_depth = 2,
         fine_attn_dim_head = 32,
         fine_attn_heads = 8,
         pad_id = -1,
+        num_sos_tokens = 1,
         condition_on_text = False,
         text_condition_model_types = ('t5',),
         text_condition_cond_drop_prob = 0.25,
-        quads = False
+        quads = False,
     ):
         super().__init__()
         self.num_vertices_per_face = 3 if not quads else 4
 
         assert autoencoder.num_vertices_per_face == self.num_vertices_per_face, 'autoencoder and transformer must both support the same type of mesh (either all triangles, or all quads)'
 
         dim, dim_fine = (dim, dim) if isinstance(dim, int) else dim
@@ -1056,17 +1057,19 @@
         self.codebook_size = autoencoder.codebook_size
         self.num_quantizers = autoencoder.num_quantizers
 
         self.eos_token_id = self.codebook_size
 
         # the fine transformer sos token
         # as well as a projection of pooled text embeddings to condition it
-        # (todo) - sos token should be moved to the coarse transformer stage
 
-        self.sos_token = nn.Parameter(torch.randn(dim_fine))
+        assert num_sos_tokens > 0
+
+        self.num_sos_tokens = num_sos_tokens
+        self.sos_token = nn.Parameter(torch.randn(num_sos_tokens, dim))
 
         # they use axial positional embeddings
 
         assert divisible_by(max_seq_len, self.num_vertices_per_face * self.num_quantizers), f'max_seq_len ({max_seq_len}) must be divisible by (3 x {self.num_quantizers}) = {3 * self.num_quantizers}' # 3 or 4 vertices per face, with D codes per vertex
 
         self.token_embed = nn.Embedding(self.codebook_size + 1, dim)
 
@@ -1440,16 +1443,16 @@
             cached_face_codes_len = cached_attended_face_codes.shape[-2]
             cached_face_codes_len_without_sos = cached_face_codes_len - 1
 
             need_call_first_transformer = face_codes_len > cached_face_codes_len_without_sos
         else:
             # auto prepend sos token
 
-            sos = repeat(self.sos_token, 'd -> b d', b = batch)
-            face_codes, _ = pack([sos, face_codes], 'b * d')
+            sos = repeat(self.sos_token, 'n d -> b n d', b = batch)
+            face_codes, packed_sos_shape = pack([sos, face_codes], 'b * d')
 
             # if no kv cache, always call first transformer
 
             need_call_first_transformer = True
 
         should_cache_fine = not divisible_by(curr_vertex_pos + 1, num_tokens_per_face)
 
@@ -1466,14 +1469,21 @@
                 **attn_context_kwargs
             )
         else:
             attended_face_codes = None
 
         attended_face_codes = safe_cat((cached_attended_face_codes, attended_face_codes), dim = -2)
 
+        # if calling without kv cache, pool the sos tokens, if greater than 1 sos token
+
+        if not exists(cache) and self.num_sos_tokens > 1:
+            sos_tokens, attended_face_codes = unpack(attended_face_codes, packed_sos_shape, 'b * d')
+            pooled_sos_token = reduce(sos_tokens, 'b n d -> b 1 d', 'mean')
+            attended_face_codes = torch.cat((pooled_sos_token, attended_face_codes), dim = 1)
+
         # maybe project from coarse to fine dimension for hierarchical transformers
 
         attended_face_codes = self.maybe_project_coarse_to_fine(attended_face_codes)
 
         grouped_codes = pad_to_length(grouped_codes, attended_face_codes.shape[-2], dim = 1)
         fine_vertex_codes, _ = pack([attended_face_codes, grouped_codes], 'b n * d')
```

### Comparing `meshgpt_pytorch-1.2.4/meshgpt_pytorch/trainer.py` & `meshgpt_pytorch-1.2.5/meshgpt_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.4/meshgpt_pytorch.egg-info/PKG-INFO` & `meshgpt_pytorch-1.2.5/meshgpt_pytorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.4
+Version: 1.2.5
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshgpt_pytorch-1.2.4/setup.py` & `meshgpt_pytorch-1.2.5/setup.py`

 * *Files identical despite different names*

