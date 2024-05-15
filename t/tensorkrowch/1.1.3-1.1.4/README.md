# Comparing `tmp/tensorkrowch-1.1.3.tar.gz` & `tmp/tensorkrowch-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorkrowch-1.1.3.tar", last modified: Mon May 13 13:39:42 2024, max compression
+gzip compressed data, was "tensorkrowch-1.1.4.tar", last modified: Wed May 15 08:25:29 2024, max compression
```

## Comparing `tensorkrowch-1.1.3.tar` & `tensorkrowch-1.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-13 13:39:42.157220 tensorkrowch-1.1.3/
--rw-rw-r--   0 jose      (1000) jose      (1000)     1086 2023-05-25 11:43:07.000000 tensorkrowch-1.1.3/LICENSE.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       11 2024-03-06 17:59:45.000000 tensorkrowch-1.1.3/MANIFEST.in
--rw-r--r--   0 jose      (1000) jose      (1000)    10354 2024-05-13 13:39:42.157220 tensorkrowch-1.1.3/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)     7808 2024-05-10 08:16:58.000000 tensorkrowch-1.1.3/README.md
--rw-rw-r--   0 jose      (1000) jose      (1000)     1482 2024-05-10 08:16:58.000000 tensorkrowch-1.1.3/pyproject.toml
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-05-13 13:39:42.157220 tensorkrowch-1.1.3/setup.cfg
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-03-06 17:59:45.000000 tensorkrowch-1.1.3/setup.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-13 13:39:42.153220 tensorkrowch-1.1.3/tensorkrowch/
--rw-rw-r--   0 jose      (1000) jose      (1000)     1382 2024-05-13 13:38:52.000000 tensorkrowch-1.1.3/tensorkrowch/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   198462 2024-05-13 12:13:53.000000 tensorkrowch-1.1.3/tensorkrowch/components.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-13 13:39:42.153220 tensorkrowch-1.1.3/tensorkrowch/decompositions/
--rw-rw-r--   0 jose      (1000) jose      (1000)       81 2024-05-10 08:17:27.000000 tensorkrowch-1.1.3/tensorkrowch/decompositions/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    10787 2024-05-09 20:25:43.000000 tensorkrowch-1.1.3/tensorkrowch/decompositions/svd_decompositions.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    13298 2024-04-18 22:46:59.000000 tensorkrowch-1.1.3/tensorkrowch/embeddings.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     6401 2024-04-18 22:46:59.000000 tensorkrowch-1.1.3/tensorkrowch/initializers.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-13 13:39:42.153220 tensorkrowch-1.1.3/tensorkrowch/models/
--rw-rw-r--   0 jose      (1000) jose      (1000)      384 2024-04-14 00:06:08.000000 tensorkrowch-1.1.3/tensorkrowch/models/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    52552 2024-05-13 13:37:43.000000 tensorkrowch-1.1.3/tensorkrowch/models/mpo.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   180174 2024-05-13 13:36:20.000000 tensorkrowch-1.1.3/tensorkrowch/models/mps.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    21760 2024-04-18 22:46:59.000000 tensorkrowch-1.1.3/tensorkrowch/models/mps_data.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    58352 2024-04-18 22:46:59.000000 tensorkrowch-1.1.3/tensorkrowch/models/peps.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    37360 2024-03-06 17:59:45.000000 tensorkrowch-1.1.3/tensorkrowch/models/tree.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   182494 2024-05-10 08:16:58.000000 tensorkrowch-1.1.3/tensorkrowch/operations.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     9156 2024-04-14 00:06:08.000000 tensorkrowch-1.1.3/tensorkrowch/utils.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-13 13:39:42.153220 tensorkrowch-1.1.3/tensorkrowch.egg-info/
--rw-r--r--   0 jose      (1000) jose      (1000)    10354 2024-05-13 13:39:42.000000 tensorkrowch-1.1.3/tensorkrowch.egg-info/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)      657 2024-05-13 13:39:42.000000 tensorkrowch-1.1.3/tensorkrowch.egg-info/SOURCES.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        1 2024-05-13 13:39:42.000000 tensorkrowch-1.1.3/tensorkrowch.egg-info/dependency_links.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)      307 2024-05-13 13:39:42.000000 tensorkrowch-1.1.3/tensorkrowch.egg-info/requires.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       13 2024-05-13 13:39:42.000000 tensorkrowch-1.1.3/tensorkrowch.egg-info/top_level.txt
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-15 08:25:29.141437 tensorkrowch-1.1.4/
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1086 2023-05-25 11:43:07.000000 tensorkrowch-1.1.4/LICENSE.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)       11 2024-03-06 17:59:45.000000 tensorkrowch-1.1.4/MANIFEST.in
+-rw-r--r--   0 jose      (1000) jose      (1000)    10354 2024-05-15 08:25:29.141437 tensorkrowch-1.1.4/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)     7808 2024-05-10 08:16:58.000000 tensorkrowch-1.1.4/README.md
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1482 2024-05-10 08:16:58.000000 tensorkrowch-1.1.4/pyproject.toml
+-rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-05-15 08:25:29.141437 tensorkrowch-1.1.4/setup.cfg
+-rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-03-06 17:59:45.000000 tensorkrowch-1.1.4/setup.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-15 08:25:29.137437 tensorkrowch-1.1.4/tensorkrowch/
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1388 2024-05-15 08:24:51.000000 tensorkrowch-1.1.4/tensorkrowch/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   200908 2024-05-14 14:34:34.000000 tensorkrowch-1.1.4/tensorkrowch/components.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-15 08:25:29.137437 tensorkrowch-1.1.4/tensorkrowch/decompositions/
+-rw-rw-r--   0 jose      (1000) jose      (1000)       81 2024-05-13 13:42:02.000000 tensorkrowch-1.1.4/tensorkrowch/decompositions/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    10923 2024-05-13 18:32:46.000000 tensorkrowch-1.1.4/tensorkrowch/decompositions/svd_decompositions.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    13298 2024-04-18 22:46:59.000000 tensorkrowch-1.1.4/tensorkrowch/embeddings.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     6401 2024-04-18 22:46:59.000000 tensorkrowch-1.1.4/tensorkrowch/initializers.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-15 08:25:29.137437 tensorkrowch-1.1.4/tensorkrowch/models/
+-rw-rw-r--   0 jose      (1000) jose      (1000)      384 2024-04-14 00:06:08.000000 tensorkrowch-1.1.4/tensorkrowch/models/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    53913 2024-05-14 19:32:41.000000 tensorkrowch-1.1.4/tensorkrowch/models/mpo.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   183143 2024-05-14 18:59:08.000000 tensorkrowch-1.1.4/tensorkrowch/models/mps.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    23202 2024-05-13 19:17:37.000000 tensorkrowch-1.1.4/tensorkrowch/models/mps_data.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    58352 2024-04-18 22:46:59.000000 tensorkrowch-1.1.4/tensorkrowch/models/peps.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    37360 2024-03-06 17:59:45.000000 tensorkrowch-1.1.4/tensorkrowch/models/tree.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   185846 2024-05-14 19:24:55.000000 tensorkrowch-1.1.4/tensorkrowch/operations.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     9244 2024-05-13 18:24:46.000000 tensorkrowch-1.1.4/tensorkrowch/utils.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-15 08:25:29.137437 tensorkrowch-1.1.4/tensorkrowch.egg-info/
+-rw-r--r--   0 jose      (1000) jose      (1000)    10354 2024-05-15 08:25:29.000000 tensorkrowch-1.1.4/tensorkrowch.egg-info/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)      657 2024-05-15 08:25:29.000000 tensorkrowch-1.1.4/tensorkrowch.egg-info/SOURCES.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)        1 2024-05-15 08:25:29.000000 tensorkrowch-1.1.4/tensorkrowch.egg-info/dependency_links.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)      307 2024-05-15 08:25:29.000000 tensorkrowch-1.1.4/tensorkrowch.egg-info/requires.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)       13 2024-05-15 08:25:29.000000 tensorkrowch-1.1.4/tensorkrowch.egg-info/top_level.txt
```

### Comparing `tensorkrowch-1.1.3/LICENSE.txt` & `tensorkrowch-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.3/PKG-INFO` & `tensorkrowch-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorkrowch
-Version: 1.1.3
+Version: 1.1.4
 Summary: Tensor Networks with PyTorch
 Author-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 Maintainer-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 José Ramón Pareja Monturiol
```

### Comparing `tensorkrowch-1.1.3/README.md` & `tensorkrowch-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.3/pyproject.toml` & `tensorkrowch-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.3/tensorkrowch/__init__.py` & `tensorkrowch-1.1.4/tensorkrowch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 TensorKrowch
 ============
 
 Tensor Networks with PyTorch
 """
 
 # Version
-__version__ = '1.1.3'
+__version__ = '1.1.4'
 
 # Network components
 from tensorkrowch.components import Axis
 from tensorkrowch.components import AbstractNode, Node, ParamNode
 from tensorkrowch.components import StackNode, ParamStackNode
 from tensorkrowch.components import Edge, StackEdge
 from tensorkrowch.components import Successor, TensorNetwork
@@ -30,14 +30,14 @@
                                      contract, contract_)
 
 # Node operations
 from tensorkrowch.operations import Operation
 from tensorkrowch.operations import get_shared_edges  # Not in docs
 
 from tensorkrowch.operations import (permute, permute_, tprod, mul, div, add,
-                                     sub, renormalize)
+                                     sub, renormalize, conj)
 from tensorkrowch.operations import (split, split_, contract_edges,
                                      contract_between, contract_between_,
                                      stack, unbind, einsum, stacked_einsum)
 
 # Models
 import tensorkrowch.models as models
```

### Comparing `tensorkrowch-1.1.3/tensorkrowch/components.py` & `tensorkrowch-1.1.4/tensorkrowch/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,14 +446,15 @@
                  override_node: bool = False,
                  tensor: Optional[Tensor] = None,
                  edges: Optional[List['Edge']] = None,
                  override_edges: bool = False,
                  node1_list: Optional[List[bool]] = None,
                  init_method: Optional[Text] = None,
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs: float) -> None:
 
         super().__init__()
 
         # Check shape and tensor.shape
         if (shape is None) == (tensor is None):
             if shape is None:
@@ -557,15 +558,18 @@
             for edge in self._edges:
                 self._network._remove_edge(edge)
 
         # Set tensor
         if shape is not None:
             if init_method is not None:
                 self._unrestricted_set_tensor(
-                    init_method=init_method, device=device, **kwargs)
+                    init_method=init_method,
+                    device=device,
+                    dtype=dtype,
+                    **kwargs)
         else:
             self._unrestricted_set_tensor(tensor=tensor)
 
     @classmethod
     def _create_resultant(cls, *args, **kwargs) -> 'AbstractNode':
         """
         Private constructor to create resultant nodes. Called from
@@ -765,14 +769,44 @@
         Returns a boolean indicating if the node is a ``resultant`` node. These
         are nodes that result from an :class:`Operation`. They are intermediate
         nodes that (almost always) inherit edges from ``leaf`` and ``data``
         nodes, the ones that really form the network. These nodes can store
         their own tensors or use other node's tensor.
         """
         return not (self._leaf or self._data or self._virtual)
+    
+    def is_conj(self) -> bool:
+        """
+        Equivalent to `torch.is_conj()
+        <https://pytorch.org/docs/stable/generated/torch.is_conj.html>`_.
+        """
+        tensor = self.tensor
+        if tensor is None:
+            return
+        return tensor.is_conj()
+    
+    def is_complex(self) -> bool:
+        """
+        Equivalent to `torch.is_complex()
+        <https://pytorch.org/docs/stable/generated/torch.is_complex.html>`_.
+        """
+        tensor = self.tensor
+        if tensor is None:
+            return
+        return tensor.is_complex()
+    
+    def is_floating_point(self) -> bool:
+        """
+        Equivalent to `torch.is_floating_point()
+        <https://pytorch.org/docs/stable/generated/torch.is_floating_point.html>`_.
+        """
+        tensor = self.tensor
+        if tensor is None:
+            return
+        return tensor.is_floating_point()
 
     def size(self, axis: Optional[Ax] = None) -> Union[Size, int]:
         """
         Returns the size of the node's tensor. If ``axis`` is specified, returns
         the size of that axis; otherwise returns the shape of the node (same as
         :attr:`shape`).
 
@@ -1166,70 +1200,76 @@
         for edge in edges:
             if edge.is_attached_to(self):
                 if not edge.is_dangling():
                     edge | edge
 
     @staticmethod
     def _make_copy_tensor(shape: Shape,
-                          device: torch.device = torch.device('cpu')) -> Tensor:
+                          device: Optional[torch.device] = None,
+                          dtype: Optional[torch.dtype] = None) -> Tensor:
         """Returns copy tensor (ones in the "diagonal", zeros elsewhere)."""
-        copy_tensor = torch.zeros(shape, device=device)
+        copy_tensor = torch.zeros(shape, device=device, dtype=dtype)
         rank = len(shape)
         if rank <= 1:
             i = 0
         else:
             i = torch.arange(min(shape), device=device)
         copy_tensor[(i,) * rank] = 1.
         return copy_tensor
 
     @staticmethod
     def _make_rand_tensor(shape: Shape,
                           low: float = 0.,
                           high: float = 1.,
-                          device: torch.device = torch.device('cpu')) -> Tensor:
+                          device: Optional[torch.device] = None,
+                          dtype: Optional[torch.dtype] = None) -> Tensor:
         """Returns tensor whose entries are drawn from the uniform distribution."""
         if not isinstance(low, float):
             raise TypeError('`low` should be float type')
         if not isinstance(high, float):
             raise TypeError('`high` should be float type')
         if low >= high:
             raise ValueError('`low` should be strictly smaller than `high`')
-        return torch.rand(shape, device=device) * (high - low) + low
+        return torch.rand(shape, device=device, dtype=dtype) * (high - low) + low
 
     @staticmethod
     def _make_randn_tensor(shape: Shape,
                            mean: float = 0.,
                            std: float = 1.,
-                           device: torch.device = torch.device('cpu')) -> Tensor:
+                           device: Optional[torch.device] = None,
+                           dtype: Optional[torch.dtype] = None) -> Tensor:
         """Returns tensor whose entries are drawn from the normal distribution."""
         if not isinstance(mean, float):
             raise TypeError('`mean` should be float type')
         if not isinstance(std, float):
             raise TypeError('`std` should be float type')
         if std <= 0:
             raise ValueError('`std` should be positive')
-        return torch.randn(shape, device=device) * std + mean
+        return torch.randn(shape, device=device, dtype=dtype) * std + mean
 
     def make_tensor(self,
                     shape: Optional[Shape] = None,
                     init_method: Text = 'zeros',
-                    device: torch.device = torch.device('cpu'),
+                    device: Optional[torch.device] = None,
+                    dtype: Optional[torch.dtype] = None,
                     **kwargs: float) -> Tensor:
         """
         Returns a tensor that can be put in the node, and is initialized according
         to ``init_method``. By default, it has the same shape as the node.
 
         Parameters
         ----------
         shape : list[int], tuple[int] or torch.Size, optional
             Shape of the tensor. If ``None``, node's shape will be used.
         init_method : {"zeros", "ones", "copy", "rand", "randn"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensor.
+        dtype : torch.dtype, optional
+            Dtype of the tensor.
         kwargs : float
             Keyword arguments for the different initialization methods:
 
             * ``low``, ``high`` for uniform initialization. See
               `torch.rand() <https://pytorch.org/docs/stable/generated/torch.rand.html>`_
 
             * ``mean``, ``std`` for normal initialization. See
@@ -1243,23 +1283,25 @@
         ------
         ValueError
             If ``init_method`` is not one of "zeros", "ones", "copy", "rand", "randn".
         """
         if shape is None:
             shape = self._shape
         if init_method == 'zeros':
-            return torch.zeros(shape, device=device)
+            return torch.zeros(shape, device=device, dtype=dtype)
         elif init_method == 'ones':
-            return torch.ones(shape, device=device)
+            return torch.ones(shape, device=device, dtype=dtype)
         elif init_method == 'copy':
-            return self._make_copy_tensor(shape, device=device)
+            return self._make_copy_tensor(shape, device=device, dtype=dtype)
         elif init_method == 'rand':
-            return self._make_rand_tensor(shape, device=device, **kwargs)
+            return self._make_rand_tensor(shape, device=device, dtype=dtype,
+                                          **kwargs)
         elif init_method == 'randn':
-            return self._make_randn_tensor(shape, device=device, **kwargs)
+            return self._make_randn_tensor(shape, device=device, dtype=dtype,
+                                           **kwargs)
         else:
             raise ValueError('Choose a valid `init_method`: "zeros", '
                              '"ones", "copy", "rand", "randn"')
 
     def _compatible_shape(self, tensor: Tensor) -> bool:
         """
         Checks if tensor's shape is "compatible" with the node's shape, meaning
@@ -1324,14 +1366,15 @@
         self._save_in_network(tensor)
         self._shape = tensor.shape
 
     def _unrestricted_set_tensor(self,
                                  tensor: Optional[Tensor] = None,
                                  init_method: Optional[Text] = 'zeros',
                                  device: Optional[torch.device] = None,
+                                 dtype: Optional[torch.dtype] = None,
                                  **kwargs: float) -> None:
         """
         Sets a new node's tensor or creates one with :meth:`make_tensor` and sets
         it. Before setting it, it is cast to the correct type, so that a
         ``torch.Tensor`` can be turned into a ``torch.nn.Parameter`` when setting
         it in :class:`ParamNodes <ParamNode>`. This is not restricted, can be
         used in any node, even in ``resultant`` nodes.
@@ -1342,48 +1385,58 @@
             Tensor to be set in the node. If ``None``, and ``init_method`` is
             provided, the tensor is created with :meth:`make_tensor`. Otherwise,
             a ``None`` is set as node's tensor.
         init_method : {"zeros", "ones", "copy", "rand", "randn"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensor.
+        dtype : torch.dtype, optional
+            Dtype of the tensor.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`make_tensor`.
         """
         if tensor is not None:
             if not isinstance(tensor, Tensor):
                 raise TypeError('`tensor` should be torch.Tensor type')
-            elif device is not None:
+            if device is not None:
                 warnings.warn('`device` was specified but is being ignored. '
                               'Provide a tensor that is already in the required'
                               ' device')
+            if dtype is not None:
+                warnings.warn('`dtype` was specified but is being ignored. '
+                              'Provide a tensor that already has the required'
+                              ' dtype')
 
             if not self._compatible_shape(tensor):
                 tensor = self._crop_tensor(tensor)
             correct_format_tensor = self._set_tensor_format(tensor)
 
         elif init_method is not None:
             node_tensor = self.tensor
-            if (device is None) and (node_tensor is not None):
-                device = node_tensor.device
+            if node_tensor is not None:
+                if device is None:
+                    device = node_tensor.device
+                if dtype is None:
+                    dtype = node_tensor.dtype
             tensor = self.make_tensor(
-                init_method=init_method, device=device, **kwargs)
+                init_method=init_method, device=device, dtype=dtype, **kwargs)
             correct_format_tensor = self._set_tensor_format(tensor)
 
         else:
             correct_format_tensor = None
 
         self._save_in_network(correct_format_tensor)
         self._shape = tensor.shape
 
     def set_tensor(self,
                    tensor: Optional[Tensor] = None,
                    init_method: Optional[Text] = 'zeros',
                    device: Optional[torch.device] = None,
+                   dtype: Optional[torch.dtype] = None,
                    **kwargs: float) -> None:
         """
         Sets new node's tensor or creates one with :meth:`make_tensor` and sets
         it. Before setting it, it is cast to the correct type: ``torch.Tensor``
         for :class:`Node` and ``torch.nn.Parameter`` for :class:`ParamNode`.
         
         When a tensor is **set** in the node, it means the node stores it, that
@@ -1409,14 +1462,16 @@
             Tensor to be set in the node. If ``None``, and ``init_method`` is
             provided, the tensor is created with :meth:`make_tensor`. Otherwise,
             a ``None`` is set as node's tensor.
         init_method : {"zeros", "ones", "copy", "rand", "randn"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensor.
+        dtype : torch.dtype, optional
+            Dtype of the tensor.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`make_tensor`.
 
         Raises
         ------
         ValueError
@@ -1449,14 +1504,15 @@
         if not self.is_resultant() and (self._tensor_info['address'] is not None):
             if (tensor is not None) and not self._compatible_shape(tensor):
                 warnings.warn(f'`tensor` is being cropped to fit the shape of '
                               f'node "{self!s}" at non-batch edges')
             self._unrestricted_set_tensor(tensor=tensor,
                                           init_method=init_method,
                                           device=device,
+                                          dtype=dtype,
                                           **kwargs)
         else:
             raise ValueError('Node\'s tensor can only be changed if it is not'
                              ' resultant and stores its own tensor')
 
     def unset_tensor(self) -> None:
         """
@@ -2001,14 +2057,16 @@
     node1_list : list[bool], optional
         If ``edges`` are provided, the list of ``node1`` attributes of each edge
         should also be provided.
     init_method : {"zeros", "ones", "copy", "rand", "randn"}, optional
         Initialization method.
     device : torch.device, optional
         Device where to initialize the tensor if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+        Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`AbstractNode.make_tensor`.
         
     Examples
     --------
     >>> node = tk.Node(shape=(2, 5, 2),
@@ -2325,14 +2383,16 @@
     node1_list : list[bool], optional
         If ``edges`` are provided, the list of ``node1`` attributes of each edge
         should also be provided.
     init_method : {"zeros", "ones", "copy", "rand", "randn"}, optional
         Initialization method.
     device : torch.device, optional
         Device where to initialize the tensor if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+        Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`AbstractNode.make_tensor`.
         
     Examples
     --------
     >>> node = tk.ParamNode(shape=(2, 5, 2),
@@ -2406,14 +2466,15 @@
                  override_node: bool = False,
                  tensor: Optional[Tensor] = None,
                  edges: Optional[List['Edge']] = None,
                  override_edges: bool = False,
                  node1_list: Optional[List[bool]] = None,
                  init_method: Optional[Text] = None,
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs: float) -> None:
 
         super().__init__(shape=shape,
                          axes_names=axes_names,
                          name=name,
                          network=network,
                          data=False,
@@ -2421,14 +2482,15 @@
                          override_node=override_node,
                          tensor=tensor,
                          edges=edges,
                          override_edges=override_edges,
                          node1_list=node1_list,
                          init_method=init_method,
                          device=device,
+                         dtype=dtype,
                          **kwargs)
 
     # ----------
     # Properties
     # ----------
     @property
     def grad(self) -> Optional[Tensor]:
```

### Comparing `tensorkrowch-1.1.3/tensorkrowch/decompositions/svd_decompositions.py` & `tensorkrowch-1.1.4/tensorkrowch/decompositions/svd_decompositions.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,17 @@
             aux_norm = s.norm(dim=-1, keepdim=True)
             if not aux_norm.isinf().any() and (aux_norm > 0).any():
                 s = s / aux_norm
                 log_norm += aux_norm.log()
         
         tensors.append(u)
         prev_bond = aux_rank
+        
+        if vh.is_complex():
+            s = s.to(vh.dtype)
         vec = torch.diag_embed(s) @ vh
         
     tensors.append(vec)
     
     if log_norm is not 0:
         rescale = (log_norm / len(tensors)).exp()
         for vec in tensors:
@@ -277,14 +280,17 @@
             aux_norm = s.norm(dim=-1)
             if not aux_norm.isinf() and (aux_norm > 0):
                 s = s / aux_norm
                 log_norm += aux_norm.log()
         
         tensors.append(u)
         prev_bond = aux_rank
+        
+        if vh.is_complex():
+            s = s.to(vh.dtype)
         mat = torch.diag_embed(s) @ vh
     
     mat = mat.reshape(aux_rank, in_out_dims[-2], in_out_dims[-1])
     tensors.append(mat)
     
     if renormalize:
         rescale = (log_norm / len(tensors)).exp()
```

### Comparing `tensorkrowch-1.1.3/tensorkrowch/embeddings.py` & `tensorkrowch-1.1.4/tensorkrowch/embeddings.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.3/tensorkrowch/initializers.py` & `tensorkrowch-1.1.4/tensorkrowch/initializers.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.3/tensorkrowch/models/mpo.py` & `tensorkrowch-1.1.4/tensorkrowch/models/mpo.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,16 @@
         be ``n_batches = 2`` (one edge for data batched, other edge for image
         patches in convolutional layers).
     init_method : {"zeros", "ones", "copy", "rand", "randn"}, optional
         Initialization method. Check :meth:`initialize` for a more detailed
         explanation of the different initialization methods.
     device : torch.device, optional
         Device where to initialize the tensors if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+        Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         
     Examples
     --------
     ``MPO`` with same input/output dimensions:
@@ -117,14 +119,15 @@
                  out_dim: Optional[Union[int, Sequence[int]]] = None,
                  bond_dim: Optional[Union[int, Sequence[int]]] = None,
                  boundary: Text = 'obc',
                  tensors: Optional[Sequence[torch.Tensor]] = None,
                  n_batches: int = 1,
                  init_method: Text = 'randn',
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs) -> None:
 
         super().__init__(name='mpo')
         
         if tensors is None:
             # boundary
             if boundary not in ['obc', 'pbc']:
@@ -263,14 +266,15 @@
         self._mats_env = []
 
         # Create Tensor Network
         self._make_nodes()
         self.initialize(tensors=tensors,
                         init_method=init_method,
                         device=device,
+                        dtype=dtype,
                         **kwargs)
     
     # ----------
     # Properties
     # ----------
     @property
     def n_features(self) -> int:
@@ -395,94 +399,108 @@
                 if i == self._n_features - 1:
                     self._mats_env[-1]['right'] ^ self._right_node['left']
     
     def initialize(self,
                    tensors: Optional[Sequence[torch.Tensor]] = None,
                    init_method: Optional[Text] = 'randn',
                    device: Optional[torch.device] = None,
+                   dtype: Optional[torch.dtype] = None,
                    **kwargs: float) -> None:
         """
         Initializes all the nodes of the :class:`MPO`. It can be called when
         instantiating the model, or to override the existing nodes' tensors.
         
         There are different methods to initialize the nodes:
         
         * ``{"zeros", "ones", "copy", "rand", "randn"}``: Each node is
           initialized calling :meth:`~tensorkrowch.AbstractNode.set_tensor` with
-          the given method, ``device`` and ``kwargs``.
+          the given method, ``device``, ``dtype`` and ``kwargs``.
         
         Parameters
         ----------
         tensors : list[torch.Tensor] or tuple[torch.Tensor], optional
             Sequence of tensors to set in each of the MPO nodes. If ``boundary``
             is ``"obc"``, all tensors should be rank-4, except the first and
             last ones, which can be rank-3, or rank-2 (if the first and last are
             the same). If ``boundary`` is ``"pbc"``, all tensors should be
             rank-4.
         init_method : {"zeros", "ones", "copy", "rand", "randn"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
+        dtype : torch.dtype, optional
+            Dtype of the tensor if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
         if tensors is not None:
             if len(tensors) != self._n_features:
                 raise ValueError('`tensors` should be a sequence of `n_features`'
                                  ' elements')
             
             if self._boundary == 'obc':
                 tensors = tensors[:]
                 
                 if device is None:
                     device = tensors[0].device
+                if dtype is None:
+                    dtype = tensors[0].dtype
                 
                 if len(tensors) == 1:
                     tensors[0] = tensors[0].reshape(1,
                                                     tensors[0].shape[0],
                                                     1,
                                                     tensors[0].shape[1])
                     
                 else:
                     # Left node
                     aux_tensor = torch.zeros(*self._mats_env[0].shape,
-                                             device=device)
+                                             device=device,
+                                             dtype=dtype)
                     aux_tensor[0] = tensors[0]
                     tensors[0] = aux_tensor
                     
                     # Right node
                     aux_tensor = torch.zeros(*self._mats_env[-1].shape,
-                                             device=device)
+                                             device=device,
+                                             dtype=dtype)
                     aux_tensor[..., 0, :] = tensors[-1]
                     tensors[-1] = aux_tensor
                 
             for tensor, node in zip(tensors, self._mats_env):
                 node.tensor = tensor
                 
         elif init_method is not None:
                 
             for i, node in enumerate(self._mats_env):
                 node.set_tensor(init_method=init_method,
                                 device=device,
+                                dtype=dtype,
                                 **kwargs)
                 
                 if self._boundary == 'obc':
-                    aux_tensor = torch.zeros(*node.shape, device=device)
+                    aux_tensor = torch.zeros(*node.shape,
+                                             device=device,
+                                             dtype=dtype)
                     if i == 0:
                         # Left node
                         aux_tensor[0] = node.tensor[0]
                     elif i == (self._n_features - 1):
                         # Right node
                         aux_tensor[..., 0, :] = node.tensor[..., 0, :]
                     node.tensor = aux_tensor
         
         if self._boundary == 'obc':
-            self._left_node.set_tensor(init_method='copy', device=device)
-            self._right_node.set_tensor(init_method='copy', device=device)
+            self._left_node.set_tensor(init_method='copy',
+                                       device=device,
+                                       dtype=dtype)
+            self._right_node.set_tensor(init_method='copy',
+                                        device=device,
+                                        dtype=dtype)
     
     def set_data_nodes(self) -> None:
         """
         Creates ``data`` nodes and connects each of them to the ``"input"``
         edge of each node.
         """      
         input_edges = [node['input'] for node in self._mats_env]
@@ -511,15 +529,16 @@
                       in_dim=self._in_dim,
                       out_dim=self._out_dim,
                       bond_dim=self._bond_dim,
                       boundary=self._boundary,
                       tensors=None,
                       n_batches=self._n_batches,
                       init_method=None,
-                      device=None)
+                      device=None,
+                      dtype=None)
         new_mpo.name = self.name + '_copy'
         if share_tensors:
             for new_node, node in zip(new_mpo._mats_env, self._mats_env):
                 new_node.tensor = node.tensor
         else:
             for new_node, node in zip(new_mpo._mats_env, self._mats_env):
                 new_node.tensor = node.tensor.clone()
@@ -1021,14 +1040,16 @@
         be ``n_batches = 2`` (one edge for data batched, other edge for image
         patches in convolutional layers).
     init_method : {"zeros", "ones", "copy", "rand", "randn"}, optional
         Initialization method. Check :meth:`initialize` for a more detailed
         explanation of the different initialization methods.
     device : torch.device, optional
         Device where to initialize the tensors if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+        Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         
     Examples
     --------
     >>> mpo = tk.models.UMPO(n_features=4,
@@ -1049,14 +1070,15 @@
                  in_dim: Optional[int] = None,
                  out_dim: Optional[int] = None,
                  bond_dim: Optional[int] = None,
                  tensor: Optional[torch.Tensor] = None,
                  n_batches: int = 1,
                  init_method: Text = 'randn',
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs) -> None:
 
         tensors = None
         
         # n_features
         if not isinstance(n_features, int):
             raise TypeError('`n_features` should be int type')
@@ -1093,14 +1115,15 @@
                          out_dim=out_dim,
                          bond_dim=bond_dim,
                          boundary='pbc',
                          tensors=tensors,
                          n_batches=n_batches,
                          init_method=init_method,
                          device=device,
+                         dtype=dtype,
                          **kwargs)
         self.name = 'umpo'
     
     def _make_nodes(self) -> None:
         """Creates all the nodes of the MPO."""
         super()._make_nodes()
         
@@ -1118,45 +1141,49 @@
         for node in self._mats_env:
             node.set_tensor_from(uniform_memory)
     
     def initialize(self,
                    tensors: Optional[Sequence[torch.Tensor]] = None,
                    init_method: Optional[Text] = 'randn',
                    device: Optional[torch.device] = None,
+                   dtype: Optional[torch.dtype] = None,
                    **kwargs: float) -> None:
         """
         Initializes the common tensor of the :class:`UMPO`. It can be called
         when instantiating the model, or to override the existing nodes' tensors.
         
         There are different methods to initialize the nodes:
         
         * ``{"zeros", "ones", "copy", "rand", "randn"}``: The tensor is
           initialized calling :meth:`~tensorkrowch.AbstractNode.set_tensor` with
-          the given method, ``device`` and ``kwargs``.
+          the given method, ``device``, ``dtype`` and ``kwargs``.
         
         Parameters
         ----------
         tensors : list[torch.Tensor] or tuple[torch.Tensor], optional
             Sequence of a single tensor to set in each of the MPO nodes. The
             tensor should be rank-4, with its first and third dimensions being
             equal.
         init_method : {"zeros", "ones", "copy", "rand", "randn"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
+        dtype : torch.dtype, optional
+            Dtype of the tensor if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
         if tensors is not None:
             self.uniform_memory.tensor = tensors[0]
         
         elif init_method is not None:
             self.uniform_memory.set_tensor(init_method=init_method,
                                            device=device,
+                                           dtype=dtype,
                                            **kwargs)
     
     def copy(self, share_tensors: bool = False) -> 'UMPO':
         """
         Creates a copy of the :class:`UMPO`.
 
         Parameters
@@ -1176,15 +1203,16 @@
         new_mpo = UMPO(n_features=self._n_features,
                        in_dim=self._in_dim[0],
                        out_dim=self._out_dim[0],
                        bond_dim=self._bond_dim[0],
                        tensor=None,
                        n_batches=self._n_batches,
                        init_method=None,
-                       device=None)
+                       device=None,
+                       dtype=None)
         new_mpo.name = self.name + '_copy'
         if share_tensors:
             new_mpo.uniform_memory.tensor = self.uniform_memory.tensor
         else:
             new_mpo.uniform_memory.tensor = self.uniform_memory.tensor.clone()
         return new_mpo
```

### Comparing `tensorkrowch-1.1.3/tensorkrowch/models/mps.py` & `tensorkrowch-1.1.4/tensorkrowch/models/mps.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,16 @@
         be ``n_batches = 2`` (one edge for data batched, other edge for image
         patches in convolutional layers).
     init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit"}, optional
         Initialization method. Check :meth:`initialize` for a more detailed
         explanation of the different initialization methods.
     device : torch.device, optional
         Device where to initialize the tensors if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+        Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         
     Examples
     --------
     ``MPS`` with the same physical dimensions:
@@ -166,14 +168,15 @@
                  boundary: Text = 'obc',
                  tensors: Optional[Sequence[torch.Tensor]] = None,
                  in_features: Optional[Sequence[int]] = None,
                  out_features: Optional[Sequence[int]] = None,
                  n_batches: int = 1,
                  init_method: Text = 'randn',
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs) -> None:
 
         super().__init__(name='mps')
         
         if tensors is None:
             # boundary
             if boundary not in ['obc', 'pbc']:
@@ -359,14 +362,15 @@
         self._mats_env = []
 
         # Create Tensor Network
         self._make_nodes()
         self.initialize(tensors=tensors,
                         init_method=init_method,
                         device=device,
+                        dtype=dtype,
                         **kwargs)
     
     # ----------
     # Properties
     # ----------
     @property
     def n_features(self) -> int:
@@ -575,15 +579,17 @@
                     self._mats_env[-1]['right'] ^ periodic_edge
             else:
                 if i == 0:
                     self._left_node['right'] ^ self._mats_env[-1]['left']
                 if i == self._n_features - 1:
                     self._mats_env[-1]['right'] ^ self._right_node['left']
     
-    def _make_canonical(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+    def _make_canonical(self,
+                        device: Optional[torch.device] = None,
+                        dtype: Optional[torch.dtype] = None) -> List[torch.Tensor]:
         """
         Creates random unitaries to initialize the MPS in canonical form with
         orthogonality center at the rightmost node. Unitaries in nodes are
         scaled so that the total norm squared of the initial MPS is the product
         of all the physical dimensions.
         """
         tensors = []
@@ -603,30 +609,30 @@
                     phys_dim = node_shape[1]
             else:
                 node_shape = node.shape
                 aux_shape = (node.shape[:2].numel(), node.shape[2])
                 phys_dim = node_shape[1]
             size = max(aux_shape[0], aux_shape[1])
             
-            tensor = random_unitary(size, device=device)
+            tensor = random_unitary(size, device=device, dtype=dtype)
             tensor = tensor[:min(aux_shape[0], size), :min(aux_shape[1], size)]
             tensor = tensor.reshape(*node_shape)
             
             if i == (self._n_features - 1):
-                if self._boundary == 'obc':
-                    tensor = tensor.t() / tensor.norm() * sqrt(phys_dim)
-                else:
-                    tensor = tensor / tensor.norm() * sqrt(phys_dim)
-            else:
-                tensor = tensor * sqrt(phys_dim)
+                if (self._boundary == 'obc') and (i == 0):
+                    tensor = tensor[:, 0]
+                tensor = tensor / tensor.norm()
+            tensor = tensor * sqrt(phys_dim)
             
             tensors.append(tensor)
         return tensors
     
-    def _make_unitaries(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+    def _make_unitaries(self,
+                        device: Optional[torch.device] = None,
+                        dtype: Optional[torch.dtype] = None) -> List[torch.Tensor]:
         """
         Creates random unitaries to initialize the MPS nodes as stacks of
         unitaries.
         """
         tensors = []
         for i, node in enumerate(self._mats_env):
             units = []
@@ -642,45 +648,44 @@
                     size_1 = min(node.shape[0], size)
                     size_2 = min(node.shape[2], size)
             else:
                 size_1 = min(node.shape[0], size)
                 size_2 = min(node.shape[2], size)
             
             for _ in range(node.shape[1]):
-                tensor = random_unitary(size, device=device)
+                tensor = random_unitary(size, device=device, dtype=dtype)
                 tensor = tensor[:size_1, :size_2]
                 units.append(tensor)
             
             units = torch.stack(units, dim=1)
             
             if self._boundary == 'obc':
                 if i == 0:
-                    tensors.append(units.squeeze(0))
+                    units = units.squeeze(0)
                 elif i == (self._n_features - 1):
-                    tensors.append(units.squeeze(-1))
-                else:
-                    tensors.append(units)
-            else:    
-                tensors.append(units)
+                    units = units.squeeze(-1)
+            tensors.append(units)
+        
         return tensors
 
     def initialize(self,
                    tensors: Optional[Sequence[torch.Tensor]] = None,
                    init_method: Optional[Text] = 'randn',
                    device: Optional[torch.device] = None,
+                   dtype: Optional[torch.dtype] = None,
                    **kwargs: float) -> None:
         """
         Initializes all the nodes of the :class:`MPS`. It can be called when
         instantiating the model, or to override the existing nodes' tensors.
         
         There are different methods to initialize the nodes:
         
         * ``{"zeros", "ones", "copy", "rand", "randn"}``: Each node is
           initialized calling :meth:`~tensorkrowch.AbstractNode.set_tensor` with
-          the given method, ``device`` and ``kwargs``.
+          the given method, ``device``, ``dtype`` and ``kwargs``.
         
         * ``"randn_eye"``: Nodes are initialized as in this
           `paper <https://arxiv.org/abs/1605.03795>`_, adding identities at the
           top of random gaussian tensors. In this case, ``std`` should be
           specified with a low value, e.g., ``std = 1e-9``.
         
         * ``"unit"``: Nodes are initialized as stacks of random unitaries. This,
@@ -702,46 +707,52 @@
             last ones, which can be rank-2, or rank-1 (if the first and last are
             the same). If ``boundary`` is ``"pbc"``, all tensors should be
             rank-3.
         init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit", "canonical"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
+        dtype : torch.dtype, optional
+            Dtype of the tensor if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
         if init_method == 'unit':
-            tensors = self._make_unitaries(device=device)
+            tensors = self._make_unitaries(device=device, dtype=dtype)
         elif init_method == 'canonical':
-            tensors = self._make_canonical(device=device)
+            tensors = self._make_canonical(device=device, dtype=dtype)
 
         if tensors is not None:
             if len(tensors) != self._n_features:
                 raise ValueError(
                     '`tensors` should be a sequence of `n_features` elements')
             
             if self._boundary == 'obc':
                 tensors = tensors[:]
                 
                 if device is None:
                     device = tensors[0].device
+                if dtype is None:
+                    dtype = tensors[0].dtype
                 
                 if len(tensors) == 1:
                     tensors[0] = tensors[0].reshape(1, -1, 1)
                 else:
                     # Left node
                     aux_tensor = torch.zeros(*self._mats_env[0].shape,
-                                             device=device)
+                                             device=device,
+                                             dtype=dtype)
                     aux_tensor[0] = tensors[0]
                     tensors[0] = aux_tensor
                     
                     # Right node
                     aux_tensor = torch.zeros(*self._mats_env[-1].shape,
-                                             device=device)
+                                             device=device,
+                                             dtype=dtype)
                     aux_tensor[..., 0] = tensors[-1]
                     tensors[-1] = aux_tensor
                 
             for tensor, node in zip(tensors, self._mats_env):
                 node.tensor = tensor
                 
         elif init_method is not None:
@@ -749,36 +760,44 @@
             if init_method == 'randn_eye':
                 init_method = 'randn'
                 add_eye = True
                 
             for i, node in enumerate(self._mats_env):
                 node.set_tensor(init_method=init_method,
                                 device=device,
+                                dtype=dtype,
                                 **kwargs)
                 if add_eye:
                     aux_tensor = node.tensor.detach()
                     aux_tensor[:, 0, :] += torch.eye(node.shape[0],
                                                      node.shape[2],
-                                                     device=device)
+                                                     device=device,
+                                                     dtype=dtype)
                     node.tensor = aux_tensor
                 
                 if self._boundary == 'obc':
-                    aux_tensor = torch.zeros(*node.shape, device=device)
+                    aux_tensor = torch.zeros(*node.shape,
+                                             device=device,
+                                             dtype=dtype)
                     if i == 0:
                         # Left node
                         aux_tensor[0] = node.tensor[0]
                         node.tensor = aux_tensor
                     elif i == (self._n_features - 1):
                         # Right node
                         aux_tensor[..., 0] = node.tensor[..., 0]
                         node.tensor = aux_tensor
         
         if self._boundary == 'obc':
-            self._left_node.set_tensor(init_method='copy', device=device)
-            self._right_node.set_tensor(init_method='copy', device=device)
+            self._left_node.set_tensor(init_method='copy',
+                                       device=device,
+                                       dtype=dtype)
+            self._right_node.set_tensor(init_method='copy',
+                                        device=device,
+                                        dtype=dtype)
 
     def set_data_nodes(self) -> None:
         """
         Creates ``data`` nodes and connects each of them to the ``"input"``
         edge of each input node.
         """      
         input_edges = [node['input'] for node in self.in_env]
@@ -808,15 +827,16 @@
                       bond_dim=self._bond_dim,
                       boundary=self._boundary,
                       tensors=None,
                       in_features=self._in_features,
                       out_features=self._out_features,
                       n_batches=self._n_batches,
                       init_method=None,
-                      device=None)
+                      device=None,
+                      dtype=None)
         new_mps.name = self.name + '_copy'
         if share_tensors:
             for new_node, node in zip(new_mps._mats_env, self._mats_env):
                 new_node.tensor = node.tensor
         else:
             for new_node, node in zip(new_mps._mats_env, self._mats_env):
                 new_node.tensor = node.tensor.clone()
@@ -1221,18 +1241,18 @@
                                                   renormalize=renormalize)
             
             else:
                 # Copy output nodes sharing tensors
                 copied_nodes = []
                 for node in nodes_out_env:
                     copied_node = node.__class__(shape=node._shape,
-                                              axes_names=node.axes_names,
-                                              name='virtual_result_copy',
-                                              network=self,
-                                              virtual=True)
+                                                 axes_names=node.axes_names,
+                                                 name='virtual_result_copy',
+                                                 network=self,
+                                                 virtual=True)
                     copied_node.set_tensor_from(node)
                     copied_nodes.append(copied_node)
                     
                     # Change batch names so that they not coincide with
                     # original batches, which gives dupliicate output batches
                     for ax in copied_node.axes:
                         if ax._batch:
@@ -1312,14 +1332,20 @@
                     for node, copied_node in zip(nodes_out_env, copied_nodes):
                         # Reattach input edges
                         node.reattach_edges(axes=['input'])
                         
                         # Connect copies directly to output nodes
                         copied_node['input'] ^ node['input']
                 
+                # If MPS nodes are complex, copied nodes are their conjugates
+                is_complex = copied_nodes[0].is_complex()
+                if is_complex:
+                    for i, node in enumerate(copied_nodes):
+                        copied_nodes[i] = node.conj()
+                
                 # Contract output nodes with copies
                 mats_out_env = self._input_contraction(
                     nodes_env=nodes_out_env,
                     input_nodes=copied_nodes,
                     inline_input=True)
                 
                 # Contract resultant matrices
@@ -1433,14 +1459,20 @@
                 
                 # Connect copies directly to output nodes
                 copied_node['input'] ^ node['input']
         else:
             copied_nodes = []
             for node in all_nodes:
                 copied_nodes.append(node.neighbours('input'))
+        
+        # If MPS nodes are complex, copied nodes are their conjugates
+        is_complex = copied_nodes[0].is_complex()
+        if is_complex:
+            for i, node in enumerate(copied_nodes):
+                copied_nodes[i] = node.conj()
             
         # Contract output nodes with copies
         mats_out_env = self._input_contraction(
             nodes_env=all_nodes,
             input_nodes=copied_nodes,
             inline_input=True)
         
@@ -1541,18 +1573,22 @@
             
             data.append(aux.reshape(*dims, 1))
         
         n_dims = len(set(dims))
         if n_dims >= 1:
             if n_dims == 1:
                 data = torch.cat(data, dim=-1)
-                data = basis(data, dim=dims[0]).float().to(self.in_env[0].device)
+                data = basis(data, dim=dims[0])\
+                    .to(self.in_env[0].dtype)\
+                    .to(self.in_env[0].device)
             elif n_dims > 1:
                 data = [
-                    basis(dat, dim=dim).squeeze(-2).float().to(self.in_env[0].device)
+                    basis(dat, dim=dim).squeeze(-2)\
+                        .to(self.in_env[0].dtype)\
+                        .to(self.in_env[0].device)
                     for dat, dim in zip(data, dims)
                     ]
             
             self.n_batches = len(dims)
             result = self.forward(data,
                                   renormalize=renormalize,
                                   marginalize_output=True)
@@ -1671,15 +1707,15 @@
         # Compute mutual information
         middle_tensor = nodes[middle_site].tensor.clone()
         _, s, _ = torch.linalg.svd(
             middle_tensor.reshape(middle_tensor.shape[:-1].numel(), # left x input
                                   middle_tensor.shape[-1]),         # right
             full_matrices=False)
         
-        s = s[s > 0]
+        s = s[s.pow(2) > 0]
         entropy = -(s.pow(2) * s.pow(2).log()).sum()
         
         # Rescale
         if log_norm != 0:
             rescale = (log_norm / len(nodes)).exp()
         
         if renormalize and (log_norm != 0):
@@ -1864,14 +1900,15 @@
 
     def _project_to_bond_dim(self,
                              nodes: List[AbstractNode],
                              bond_dim: int,
                              side: Text = 'right'):
         """Projects all nodes into a space of dimension ``bond_dim``."""
         device = nodes[0].tensor.device
+        dtype = nodes[0].tensor.dtype
 
         if side == 'left':
             nodes.reverse()
         elif side != 'right':
             raise ValueError('`side` can only be \'left\' or \'right\'')
 
         for node in nodes:
@@ -1888,15 +1925,15 @@
                                      axes_names=(*(['input'] * len(phys_dim_lst)),
                                                  'bond_dim'),
                                      name=f'proj_mat_node_{side}',
                                      network=self)
 
                 proj_mat_node.tensor = torch.eye(
                     torch.tensor(phys_dim_lst).prod().int().item(),
-                    bond_dim).view(*phys_dim_lst, -1).to(device)
+                    bond_dim).view(*phys_dim_lst, -1).to(dtype).to(device)
                 for k in range(j + 1):
                     nodes[k]['input'] ^ proj_mat_node[k]
 
                 aux_result = proj_mat_node
                 for k in range(j + 1):
                     aux_result @= nodes[k]
                 line_mat_nodes.append(aux_result)  # bond_dim x left x right
@@ -1908,15 +1945,15 @@
                                  axes_names=(*(['input'] * len(phys_dim_lst)),
                                              'bond_dim'),
                                  name=f'proj_mat_node_{side}',
                                  network=self)
 
             proj_mat_node.tensor = torch.eye(
                 torch.tensor(phys_dim_lst).prod().int().item(),
-                bond_dim).view(*phys_dim_lst, -1).to(device)
+                bond_dim).view(*phys_dim_lst, -1).to(dtype).to(device)
             for k in range(j + 1):
                 nodes[k]['input'] ^ proj_mat_node[k]
 
             aux_result = proj_mat_node
             for k in range(j + 1):
                 aux_result @= nodes[k]
             line_mat_nodes.append(aux_result)
@@ -1925,15 +1962,16 @@
         while k < len(nodes):
             phys_dim = nodes[k]['input'].size()
             proj_vec_node = Node(shape=(phys_dim,),
                                  axes_names=('input',),
                                  name=f'proj_vec_node_{side}_({k})',
                                  network=self)
 
-            proj_vec_node.tensor = torch.eye(phys_dim, 1).squeeze().to(device)
+            proj_vec_node.tensor = torch.eye(phys_dim, 1).squeeze()\
+                .to(dtype).to(device)
             nodes[k]['input'] ^ proj_vec_node['input']
             line_mat_nodes.append(proj_vec_node @ nodes[k])
 
             k += 1
 
         line_mat_nodes.reverse()
         result = line_mat_nodes[0]
@@ -2093,14 +2131,16 @@
         be ``n_batches = 2`` (one edge for data batched, other edge for image
         patches in convolutional layers).
     init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit"}, optional
         Initialization method. Check :meth:`initialize` for a more detailed
         explanation of the different initialization methods.
     device : torch.device, optional
         Device where to initialize the tensors if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+        Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         
     Examples
     --------
     >>> mps = tk.models.UMPS(n_features=4,
@@ -2121,14 +2161,15 @@
                  bond_dim: Optional[int] = None,
                  tensor: Optional[torch.Tensor] = None,
                  in_features: Optional[Sequence[int]] = None,
                  out_features: Optional[Sequence[int]] = None,
                  n_batches: int = 1,
                  init_method: Text = 'randn',
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs) -> None:
         
         tensors = None
         
         # n_features
         if not isinstance(n_features, int):
             raise TypeError('`n_features` should be int type')
@@ -2162,14 +2203,15 @@
                          boundary='pbc',
                          tensors=tensors,
                          in_features=in_features,
                          out_features=out_features,
                          n_batches=n_batches,
                          init_method=init_method,
                          device=device,
+                         dtype=dtype,
                          **kwargs)
         self.name = 'umps'
 
     def _make_nodes(self) -> None:
         """Creates all the nodes of the MPS."""
         super()._make_nodes()
         
@@ -2182,63 +2224,68 @@
                                    network=self,
                                    virtual=True)
         self.uniform_memory = uniform_memory
         
         for node in self._mats_env:
             node.set_tensor_from(uniform_memory)
     
-    def _make_canonical(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+    def _make_canonical(self,
+                        device: Optional[torch.device] = None,
+                        dtype: Optional[torch.dtype] = None) -> List[torch.Tensor]:
         """
         Creates random unitaries to initialize the MPS in canonical form with
         orthogonality center at the rightmost node. Unitaries in nodes are
         scaled so that the total norm squared of the initial MPS is the product
         of all the physical dimensions.
         """
         node = self.uniform_memory
         node_shape = node.shape
         aux_shape = (node.shape[:2].numel(), node.shape[2])
         
         size = max(aux_shape[0], aux_shape[1])
         phys_dim = node_shape[1]
         
-        tensor = random_unitary(size, device=device)
+        tensor = random_unitary(size, device=device, dtype=dtype)
         tensor = tensor[:min(aux_shape[0], size), :min(aux_shape[1], size)]
         tensor = tensor.reshape(*node_shape)
         tensor = tensor * sqrt(phys_dim)
         return tensor
     
-    def _make_unitaries(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+    def _make_unitaries(self,
+                        device: Optional[torch.device] = None,
+                        dtype: Optional[torch.dtype] = None) -> List[torch.Tensor]:
         """
         Creates random unitaries to initialize the MPS nodes as stacks of
         unitaries.
         """
         node = self.uniform_memory
         node_shape = node.shape
         
         units = []
         for _ in range(node_shape[1]):
-            tensor = random_unitary(node_shape[0], device=device)
+            tensor = random_unitary(node_shape[0], device=device, dtype=dtype)
             units.append(tensor)
         tensor = torch.stack(units, dim=1)
         return tensor
 
     def initialize(self,
                    tensors: Optional[Sequence[torch.Tensor]] = None,
                    init_method: Optional[Text] = 'randn',
                    device: Optional[torch.device] = None,
+                   dtype: Optional[torch.dtype] = None,
                    **kwargs: float) -> None:
         """
         Initializes the common tensor of the :class:`UMPS`. It can be called
         when instantiating the model, or to override the existing nodes' tensors.
         
         There are different methods to initialize the nodes:
         
         * ``{"zeros", "ones", "copy", "rand", "randn"}``: The tensor is
           initialized calling :meth:`~tensorkrowch.AbstractNode.set_tensor` with
-          the given method, ``device`` and ``kwargs``.
+          the given method, ``device``, ``dtype`` and ``kwargs``.
         
         * ``"randn_eye"``: Tensor is initialized as in this
           `paper <https://arxiv.org/abs/1605.03795>`_, adding identities at the
           top of a random gaussian tensor. In this case, ``std`` should be
           specified with a low value, e.g., ``std = 1e-9``.
         
         * ``"unit"``: Tensor is initialized as a stack of random unitaries. This,
@@ -2257,42 +2304,46 @@
             Sequence of a single tensor to set in each of the MPS nodes. The
             tensor should be rank-3, with its first and last dimensions being
             equal.
         init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit", "canonical"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
+        dtype : torch.dtype, optional
+            Dtype of the tensor if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
         node = self.uniform_memory
         
         if init_method == 'unit':
-            tensors = [self._make_unitaries(device=device)]
+            tensors = [self._make_unitaries(device=device, dtype=dtype)]
         elif init_method == 'canonical':
-            tensors = [self._make_canonical(device=device)]
+            tensors = [self._make_canonical(device=device, dtype=dtype)]
         
         if tensors is not None:
             node.tensor = tensors[0]
         
         elif init_method is not None:
             add_eye = False
             if init_method == 'randn_eye':
                 init_method = 'randn'
                 add_eye = True
             
             node.set_tensor(init_method=init_method,
                             device=device,
+                            dtype=dtype,
                             **kwargs)
             if add_eye:
                 aux_tensor = node.tensor.detach()
                 aux_tensor[:, 0, :] += torch.eye(node.shape[0],
                                                  node.shape[2],
-                                                 device=device)
+                                                 device=device,
+                                                 dtype=dtype)
                 node.tensor = aux_tensor
     
     def copy(self, share_tensors: bool = False) -> 'UMPS':
         """
         Creates a copy of the :class:`UMPS`.
 
         Parameters
@@ -2313,15 +2364,16 @@
                        phys_dim=self._phys_dim[0],
                        bond_dim=self._bond_dim[0],
                        tensor=None,
                        in_features=self._in_features,
                        out_features=self._out_features,
                        n_batches=self._n_batches,
                        init_method=None,
-                       device=None)
+                       device=None,
+                       dtype=None)
         new_mps.name = self.name + '_copy'
         if share_tensors:
             new_mps.uniform_memory.tensor = self.uniform_memory.tensor
         else:
             new_mps.uniform_memory.tensor = self.uniform_memory.tensor.clone()
         return new_mps
     
@@ -2457,14 +2509,16 @@
         be ``n_batches = 2`` (e.g. one edge for data batched, other edge for
         image patches in convolutional layers).
     init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit"}, optional
         Initialization method. Check :meth:`initialize` for a more detailed
         explanation of the different initialization methods.
     device : torch.device, optional
         Device where to initialize the tensors if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+        Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         
     Examples
     --------
     ``MPSLayer`` with same input dimensions:
@@ -2498,14 +2552,15 @@
                  bond_dim: Optional[Union[int, Sequence[int]]] = None,
                  out_position: Optional[int] = None,
                  boundary: Text = 'obc',
                  tensors: Optional[Sequence[torch.Tensor]] = None,
                  n_batches: int = 1,
                  init_method: Text = 'randn',
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs) -> None:
         
         phys_dim = None
         
         if tensors is not None:
             if not isinstance(tensors, (list, tuple)):
                 raise TypeError('`tensors` should be a tuple[torch.Tensor] or '
@@ -2559,14 +2614,15 @@
                          boundary=boundary,
                          tensors=tensors,
                          in_features=None,
                          out_features=[out_position],
                          n_batches=n_batches,
                          init_method=init_method,
                          device=device,
+                         dtype=dtype,
                          **kwargs)
         self.name = 'mpslayer'
         self._in_dim = self._phys_dim[:out_position] + \
             self._phys_dim[(out_position + 1):]
         self._out_dim = self._phys_dim[out_position]
     
     @property
@@ -2588,15 +2644,17 @@
         return self._out_position
     
     @property
     def out_node(self) -> ParamNode:
         """Returns the output node."""
         return self._mats_env[self._out_position]
     
-    def _make_canonical(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+    def _make_canonical(self,
+                        device: Optional[torch.device] = None,
+                        dtype: Optional[torch.dtype] = None) -> List[torch.Tensor]:
         """
         Creates random unitaries to initialize the MPS in canonical form with
         orthogonality center at the rightmost node. Unitaries in nodes are
         scaled so that the total norm squared of the initial MPS is the product
         of all the physical dimensions.
         """
         # Left nodes
@@ -2613,22 +2671,24 @@
                     phys_dim = node_shape[1]
             else:
                 node_shape = node.shape
                 aux_shape = (node.shape[:2].numel(), node.shape[2])
                 phys_dim = node_shape[1]
             size = max(aux_shape[0], aux_shape[1])
             
-            tensor = random_unitary(size, device=device)
+            tensor = random_unitary(size, device=device, dtype=dtype)
             tensor = tensor[:min(aux_shape[0], size), :min(aux_shape[1], size)]
             tensor = tensor.reshape(*node_shape)
             
             left_tensors.append(tensor * sqrt(phys_dim))
         
         # Output node
-        out_tensor = torch.randn(self.out_node.shape, device=device)
+        out_tensor = torch.randn(self.out_node.shape,
+                                 device=device,
+                                 dtype=dtype)
         phys_dim = out_tensor.shape[1]
         if self._boundary == 'obc':
             if self._out_position == 0:
                 out_tensor = out_tensor[0]
             if self._out_position == (self._n_features - 1):
                 out_tensor = out_tensor[..., 0]
         out_tensor = out_tensor / out_tensor.norm() * sqrt(phys_dim)
@@ -2647,26 +2707,28 @@
                     phys_dim = node_shape[1]
             else:
                 node_shape = node.shape
                 aux_shape = (node.shape[0], node.shape[1:].numel())
                 phys_dim = node_shape[1]
             size = max(aux_shape[0], aux_shape[1])
             
-            tensor = random_unitary(size, device=device)
+            tensor = random_unitary(size, device=device, dtype=dtype)
             tensor = tensor[:min(aux_shape[0], size), :min(aux_shape[1], size)]
             tensor = tensor.reshape(*node_shape)
             
             right_tensors.append(tensor * sqrt(phys_dim))
         right_tensors.reverse()
         
         # All tensors
         tensors = left_tensors + [out_tensor] + right_tensors
         return tensors
     
-    def _make_unitaries(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+    def _make_unitaries(self,
+                        device: Optional[torch.device] = None,
+                        dtype: Optional[torch.dtype] = None) -> List[torch.Tensor]:
         """
         Creates random unitaries to initialize the MPS nodes as stacks of
         unitaries.
         """
         # Left_nodes
         left_tensors = []
         for i, node in enumerate(self._mats_env[:self._out_position]):
@@ -2680,30 +2742,32 @@
                     size_1 = min(node.shape[0], size)
                     size_2 = min(node.shape[2], size)
             else:
                 size_1 = min(node.shape[0], size)
                 size_2 = min(node.shape[2], size)
             
             for _ in range(node.shape[1]):
-                tensor = random_unitary(size, device=device)
+                tensor = random_unitary(size, device=device, dtype=dtype)
                 tensor = tensor[:size_1, :size_2]
                 units.append(tensor)
             
             units = torch.stack(units, dim=1)
             
             if self._boundary == 'obc':
                 if i == 0:
                     left_tensors.append(units.squeeze(0))
                 else:
                     left_tensors.append(units)
             else:    
                 left_tensors.append(units)
         
         # Output node
-        out_tensor = torch.randn(self.out_node.shape, device=device)
+        out_tensor = torch.randn(self.out_node.shape,
+                                 device=device,
+                                 dtype=dtype)
         if self._boundary == 'obc':
             if self._out_position == 0:
                 out_tensor = out_tensor[0]
             if self._out_position == (self._n_features - 1):
                 out_tensor = out_tensor[..., 0]
         
         # Right nodes
@@ -2719,15 +2783,15 @@
                     size_1 = min(node.shape[0], size)
                     size_2 = min(node.shape[2], size)
             else:
                 size_1 = min(node.shape[0], size)
                 size_2 = min(node.shape[2], size)
             
             for _ in range(node.shape[1]):
-                tensor = random_unitary(size, device=device).t()
+                tensor = random_unitary(size, device=device, dtype=dtype).H
                 tensor = tensor[:size_1, :size_2]
                 units.append(tensor)
             
             units = torch.stack(units, dim=1)
             
             if self._boundary == 'obc':
                 if i == 0:
@@ -2737,81 +2801,30 @@
             else:    
                 right_tensors.append(units)
         right_tensors.reverse()
         
         # All tensors
         tensors = left_tensors + [out_tensor] + right_tensors
         return tensors
-
-    def initialize(self,
-                   tensors: Optional[Sequence[torch.Tensor]] = None,
-                   init_method: Optional[Text] = 'randn',
-                   device: Optional[torch.device] = None,
-                   **kwargs: float) -> None:
-        """
-        Initializes all the nodes of the :class:`MPS`. It can be called when
-        instantiating the model, or to override the existing nodes' tensors.
-        
-        There are different methods to initialize the nodes:
-        
-        * ``{"zeros", "ones", "copy", "rand", "randn"}``: Each node is
-          initialized calling :meth:`~tensorkrowch.AbstractNode.set_tensor` with
-          the given method, ``device`` and ``kwargs``.
-        
-        * ``"randn_eye"``: Nodes are initialized as in this
-          `paper <https://arxiv.org/abs/1605.03795>`_, adding identities at the
-          top of random gaussian tensors. In this case, ``std`` should be
-          specified with a low value, e.g., ``std = 1e-9``.
-        
-        * ``"unit"``: Nodes are initialized as stacks of random unitaries. This,
-          combined (at least) with an embedding of the inputs as elements of
-          the computational basis (:func:`~tensorkrowch.embeddings.discretize`
-          combined with :func:`~tensorkrowch.embeddings.basis`)
-        
-        * ``"canonical"```: MPS is initialized in canonical form with a squared
-          norm `close` to the product of all the physical dimensions (if bond
-          dimensions are bigger than the powers of the physical dimensions,
-          the norm could vary). Th orthogonality center is at the rightmost
-          node.
-        
-        Parameters
-        ----------
-        tensors : list[torch.Tensor] or tuple[torch.Tensor], optional
-            Sequence of tensors to set in each of the MPS nodes. If ``boundary``
-            is ``"obc"``, all tensors should be rank-3, except the first and
-            last ones, which can be rank-2, or rank-1 (if the first and last are
-            the same). If ``boundary`` is ``"pbc"``, all tensors should be
-            rank-3.
-        init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit", "canonical"}, optional
-            Initialization method.
-        device : torch.device, optional
-            Device where to initialize the tensors if ``init_method`` is provided.
-        kwargs : float
-            Keyword arguments for the different initialization methods. See
-            :meth:`~tensorkrowch.AbstractNode.make_tensor`.
-        """
-        if init_method == 'unit':
-            tensors = self._make_unitaries(device=device)
-        elif init_method == 'canonical':
-            tensors = self._make_canonical(device=device)
     
     def initialize(self,
                    tensors: Optional[Sequence[torch.Tensor]] = None,
                    init_method: Optional[Text] = 'randn',
                    device: Optional[torch.device] = None,
+                   dtype: Optional[torch.dtype] = None,
                    **kwargs: float) -> None:
         """
         Initializes all the nodes of the :class:`MPSLayer`. It can be called when
         instantiating the model, or to override the existing nodes' tensors.
         
         There are different methods to initialize the nodes:
         
         * ``{"zeros", "ones", "copy", "rand", "randn"}``: Each node is
           initialized calling :meth:`~tensorkrowch.AbstractNode.set_tensor` with
-          the given method, ``device`` and ``kwargs``.
+          the given method, ``device``, ``dtype`` and ``kwargs``.
         
         * ``"randn_eye"``: Nodes are initialized as in this
           `paper <https://arxiv.org/abs/1605.03795>`_, adding identities at the
           top of random gaussian tensors. In this case, ``std`` should be
           specified with a low value, e.g., ``std = 1e-9``.
         
         * ``"unit"``: Nodes are initialized as stacks of random unitaries. This,
@@ -2832,46 +2845,52 @@
             last ones, which can be rank-2, or rank-1 (if the first and last are
             the same). If ``boundary`` is ``"pbc"``, all tensors should be
             rank-3.
         init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit", "canonical"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
+        dtype : torch.dtype, optional
+            Dtype of the tensor if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
         if init_method == 'unit':
-            tensors = self._make_unitaries(device=device)
+            tensors = self._make_unitaries(device=device, dtype=dtype)
         elif init_method == 'canonical':
-            tensors = self._make_canonical(device=device)
+            tensors = self._make_canonical(device=device, dtype=dtype)
 
         if tensors is not None:
             if len(tensors) != self._n_features:
                 raise ValueError('`tensors` should be a sequence of `n_features`'
                                  ' elements')
             
             if self._boundary == 'obc':
                 tensors = tensors[:]
                 
                 if device is None:
                     device = tensors[0].device
+                if dtype is None:
+                    dtype = tensors[0].dtype
                 
                 if len(tensors) == 1:
                     tensors[0] = tensors[0].reshape(1, -1, 1)
                 else:
                     # Left node
                     aux_tensor = torch.zeros(*self._mats_env[0].shape,
-                                             device=device)
+                                             device=device,
+                                             dtype=dtype)
                     aux_tensor[0] = tensors[0]
                     tensors[0] = aux_tensor
                     
                     # Right node
                     aux_tensor = torch.zeros(*self._mats_env[-1].shape,
-                                             device=device)
+                                             device=device,
+                                             dtype=dtype)
                     aux_tensor[..., 0] = tensors[-1]
                     tensors[-1] = aux_tensor
                 
             for tensor, node in zip(tensors, self._mats_env):
                 node.tensor = tensor
                 
         elif init_method is not None:
@@ -2879,42 +2898,50 @@
             if init_method == 'randn_eye':
                 init_method = 'randn'
                 add_eye = True
                 
             for i, node in enumerate(self._mats_env):
                 node.set_tensor(init_method=init_method,
                                 device=device,
+                                dtype=dtype,
                                 **kwargs)
                 if add_eye:
                     aux_tensor = node.tensor.detach()
                     eye_tensor = torch.eye(node.shape[0],
                                            node.shape[2],
-                                           device=device)
+                                           device=device,
+                                           dtype=dtype)
                     if i == self._out_position:
                         eye_tensor = eye_tensor.unsqueeze(1)
                         eye_tensor = eye_tensor.expand(node.shape)
                         aux_tensor += eye_tensor
                     else:
                         aux_tensor[:, 0, :] += eye_tensor
                     node.tensor = aux_tensor
                 
                 if self._boundary == 'obc':
-                    aux_tensor = torch.zeros(*node.shape, device=device)
+                    aux_tensor = torch.zeros(*node.shape,
+                                             device=device,
+                                             dtype=dtype)
                     if i == 0:
                         # Left node
                         aux_tensor[0] = node.tensor[0]
                         node.tensor = aux_tensor
                     elif i == (self._n_features - 1):
                         # Right node
                         aux_tensor[..., 0] = node.tensor[..., 0]
                         node.tensor = aux_tensor
         
         if self._boundary == 'obc':
-            self._left_node.set_tensor(init_method='copy', device=device)
-            self._right_node.set_tensor(init_method='copy', device=device)
+            self._left_node.set_tensor(init_method='copy',
+                                       device=device,
+                                       dtype=dtype)
+            self._right_node.set_tensor(init_method='copy',
+                                        device=device,
+                                        dtype=dtype)
 
     def copy(self, share_tensors: bool = False) -> 'MPSLayer':
         """
         Creates a copy of the :class:`MPSLayer`.
 
         Parameters
         ----------
@@ -2935,15 +2962,16 @@
                            out_dim=self._out_dim,
                            bond_dim=self._bond_dim,
                            out_position=self._out_position,
                            boundary=self._boundary,
                            tensors=None,
                            n_batches=self._n_batches,
                            init_method=None,
-                           device=None)
+                           device=None,
+                           dtype=None)
         new_mps.name = self.name + '_copy'
         if share_tensors:
             for new_node, node in zip(new_mps._mats_env, self._mats_env):
                 new_node.tensor = node.tensor
         else:
             for new_node, node in zip(new_mps._mats_env, self._mats_env):
                 new_node.tensor = node.tensor.clone()
@@ -2997,14 +3025,16 @@
         be ``n_batches = 2`` (one edge for data batched, other edge for image
         patches in convolutional layers).
     init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit"}, optional
         Initialization method. Check :meth:`initialize` for a more detailed
         explanation of the different initialization methods.
     device : torch.device, optional
         Device where to initialize the tensors if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+        Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         
     Examples
     --------
     >>> mps_layer = tk.models.UMPSLayer(n_features=4,
@@ -3027,14 +3057,15 @@
                  out_dim: Optional[int] = None,
                  bond_dim: Optional[int] = None,
                  out_position: Optional[int] = None,
                  tensors: Optional[Sequence[torch.Tensor]] = None,
                  n_batches: int = 1,
                  init_method: Text = 'randn',
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs) -> None:
         
         phys_dim = None
         
         # n_features
         if not isinstance(n_features, int):
             raise TypeError('`n_features` should be int type')
@@ -3102,14 +3133,15 @@
                          boundary='pbc',
                          tensors=tensors,
                          in_features=None,
                          out_features=[out_position],
                          n_batches=n_batches,
                          init_method=init_method,
                          device=device,
+                         dtype=dtype,
                          **kwargs)
         self.name = 'umpslayer'
         self._in_dim = self._phys_dim[:out_position] + \
             self._phys_dim[(out_position + 1):]
         self._out_dim = self._phys_dim[out_position]
     
     @property
@@ -3150,72 +3182,81 @@
         self.uniform_memory = uniform_memory
         
         in_nodes = self._mats_env[:self._out_position] + \
             self._mats_env[(self._out_position + 1):]
         for node in in_nodes:
             node.set_tensor_from(uniform_memory)
     
-    def _make_canonical(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+    def _make_canonical(self,
+                        device: Optional[torch.device] = None,
+                        dtype: Optional[torch.dtype] = None) -> List[torch.Tensor]:
         """
         Creates random unitaries to initialize the MPS in canonical form with
         orthogonality center at the rightmost node. Unitaries in nodes are
         scaled so that the total norm squared of the initial MPS is the product
         of all the physical dimensions.
         """
         # Uniform node
         node = self.uniform_memory
         node_shape = node.shape
         aux_shape = (node.shape[:2].numel(), node.shape[2])
         
         size = max(aux_shape[0], aux_shape[1])
         phys_dim = node_shape[1]
         
-        uni_tensor = random_unitary(size, device=device)
+        uni_tensor = random_unitary(size, device=device, dtype=dtype)
         uni_tensor = uni_tensor[:min(aux_shape[0], size), :min(aux_shape[1], size)]
         uni_tensor = uni_tensor.reshape(*node_shape)
         uni_tensor = uni_tensor * sqrt(phys_dim)
         
         # Output node
-        out_tensor = torch.randn(self.out_node.shape, device=device)
+        out_tensor = torch.randn(self.out_node.shape,
+                                 device=device,
+                                 dtype=dtype)
         out_tensor = out_tensor / out_tensor.norm() * sqrt(out_tensor.shape[1])
         
         return [uni_tensor, out_tensor]
     
-    def _make_unitaries(self, device: Optional[torch.device] = None) -> List[torch.Tensor]:
+    def _make_unitaries(self,
+                        device: Optional[torch.device] = None,
+                        dtype: Optional[torch.dtype] = None) -> List[torch.Tensor]:
         """
         Creates random unitaries to initialize the MPS nodes as stacks of
         unitaries.
         """
         tensors = []
         for node in [self.uniform_memory, self.out_node]:
             node_shape = node.shape
             
             units = []
             for _ in range(node_shape[1]):
-                tensor = random_unitary(node_shape[0], device=device)
+                tensor = random_unitary(node_shape[0],
+                                        device=device,
+                                        dtype=dtype)
                 units.append(tensor)
             
             tensors.append(torch.stack(units, dim=1))
         
         return tensors
 
     def initialize(self,
                    tensors: Optional[Sequence[torch.Tensor]] = None,
                    init_method: Optional[Text] = 'randn',
                    device: Optional[torch.device] = None,
+                   dtype: Optional[torch.dtype] = None,
                    **kwargs: float) -> None:
         """
         Initializes the common tensor of the :class:`UMPSLayer`. It can be called
         when instantiating the model, or to override the existing nodes' tensors.
         
         There are different methods to initialize the nodes:
         
         * ``{"zeros", "ones", "copy", "rand", "randn"}``: The tensor is
           initialized calling :meth:`~tensorkrowch.AbstractNode.set_tensor` with
-          the given method, ``device`` and ``kwargs``.
+          the given method, ``device``, ``dtype`` and ``kwargs``.
         
         * ``"randn_eye"``: Tensor is initialized as in this
           `paper <https://arxiv.org/abs/1605.03795>`_, adding identities at the
           top of a random gaussian tensor. In this case, ``std`` should be
           specified with a low value, e.g., ``std = 1e-9``.
           
         * ``"unit"``: Tensor is initialized as a stack of random unitaries. This,
@@ -3235,42 +3276,46 @@
             that will be set in all input nodes, and the second one will be the
             output node's tensor. Both tensors should be rank-3, with all their
             first and last dimensions being equal.
         init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit", "canonical"}, optional
             Initialization method.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
+        dtype : torch.dtype, optional
+            Dtype of the tensor if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
         if init_method == 'unit':
-            tensors = self._make_unitaries(device=device)
+            tensors = self._make_unitaries(device=device, dtype=dtype)
         elif init_method == 'canonical':
-            tensors = self._make_canonical(device=device)
+            tensors = self._make_canonical(device=device, dtype=dtype)
         
         if tensors is not None:
             self.uniform_memory.tensor = tensors[0]
             self.out_node.tensor = tensors[-1]
         
         elif init_method is not None:
             for i, node in enumerate([self.uniform_memory, self.out_node]):
                 add_eye = False
                 if init_method == 'randn_eye':
                     init_method = 'randn'
                     add_eye = True
                 
                 node.set_tensor(init_method=init_method,
                                 device=device,
+                                dtype=dtype,
                                 **kwargs)
                 if add_eye:
                     aux_tensor = node.tensor.detach()
                     eye_tensor = torch.eye(node.shape[0],
                                            node.shape[2],
-                                           device=device)
+                                           device=device,
+                                           dtype=dtype)
                     if i == 0:
                         aux_tensor[:, 0, :] += eye_tensor
                     else:
                         eye_tensor = eye_tensor.unsqueeze(1)
                         eye_tensor = eye_tensor.expand(node.shape)
                         aux_tensor += eye_tensor
                     node.tensor = aux_tensor
@@ -3297,15 +3342,16 @@
                             in_dim=self._in_dim[0] if self._in_dim else None,
                             out_dim=self._out_dim,
                             bond_dim=self._bond_dim,
                             out_position=self._out_position,
                             tensor=None,
                             n_batches=self._n_batches,
                             init_method=None,
-                            device=None)
+                            device=None,
+                            dtype=None)
         new_mps.name = self.name + '_copy'
         if share_tensors:
             new_mps.uniform_memory.tensor = self.uniform_memory.tensor
             new_mps.out_node.tensor = self.out_node.tensor
         else:
             new_mps.uniform_memory.tensor = self.uniform_memory.tensor.clone()
             new_mps.out_node.tensor = self.out_node.tensor.clone()
@@ -3538,14 +3584,16 @@
         ``tensors`` contains a single element, it can be rank-1 ("obc") or
         rank-3 ("pbc").
     init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit"}, optional
         Initialization method. Check :meth:`~MPS.initialize` for a more detailed
         explanation of the different initialization methods.
     device : torch.device, optional
         Device where to initialize the tensors if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+        Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         
     Examples
     --------
     >>> conv_mps = tk.models.ConvMPS(in_channels=2,
@@ -3564,14 +3612,15 @@
                  stride: int = 1,
                  padding: int = 0,
                  dilation: int = 1,
                  boundary: Text = 'obc',
                  tensors: Optional[Sequence[torch.Tensor]] = None,
                  init_method: Text = 'randn',
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs):
         
         unfold = self._set_attributes(in_channels=in_channels,
                                       kernel_size=kernel_size,
                                       stride=stride,
                                       padding=padding,
                                       dilation=dilation)
@@ -3581,14 +3630,15 @@
                      phys_dim=in_channels,
                      bond_dim=bond_dim,
                      boundary=boundary,
                      tensors=tensors,
                      n_batches=2,
                      init_method=init_method,
                      device=device,
+                     dtype=dtype,
                      **kwargs)
         
         self.unfold = unfold
     
     @property
     def in_channels(self) -> int:
         """Returns ``in_channels``. Same as ``phys_dim`` in :class:`MPS`."""
@@ -3649,15 +3699,16 @@
                           kernel_size=self._kernel_size,
                           stride=self._stride,
                           padding=self._padding,
                           dilation=self.dilation,
                           boundary=self._boundary,
                           tensors=None,
                           init_method=None,
-                          device=None)
+                          device=None,
+                          dtype=None)
         new_mps.name = self.name + '_copy'
         if share_tensors:
             for new_node, node in zip(new_mps._mats_env, self._mats_env):
                 new_node.tensor = node.tensor
         else:
             for new_node, node in zip(new_mps._mats_env, self._mats_env):
                 new_node.tensor = node.tensor.clone()
@@ -3701,14 +3752,16 @@
         To initialize MPS nodes, a MPS tensor can be provided. The tensor
         should be rank-3, with its first and last dimensions being equal.
     init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit"}, optional
         Initialization method. Check :meth:`~UMPS.initialize` for a more detailed
         explanation of the different initialization methods.
     device : torch.device, optional
         Device where to initialize the tensors if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+        Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`~tensorkrowch.AbstractNode.make_tensor`.
     
     
     Examples
     --------
@@ -3730,14 +3783,15 @@
                  kernel_size: Union[int, Sequence],
                  stride: int = 1,
                  padding: int = 0,
                  dilation: int = 1,
                  tensor: Optional[torch.Tensor] = None,
                  init_method: Text = 'randn',
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs):
 
         unfold = self._set_attributes(in_channels=in_channels,
                                       kernel_size=kernel_size,
                                       stride=stride,
                                       padding=padding,
                                       dilation=dilation)
@@ -3746,14 +3800,15 @@
                       n_features=self._kernel_size[0] * self._kernel_size[1],
                       phys_dim=in_channels,
                       bond_dim=bond_dim,
                       tensor=tensor,
                       n_batches=2,
                       init_method=init_method,
                       device=device,
+                      dtype=dtype,
                       **kwargs)
         
         self.unfold = unfold
     
     @property
     def in_channels(self) -> int:
         """Returns ``in_channels``. Same as ``phys_dim`` in :class:`MPS`."""
@@ -3813,15 +3868,16 @@
                            bond_dim=self._bond_dim[0],
                            kernel_size=self._kernel_size,
                            stride=self._stride,
                            padding=self._padding,
                            dilation=self.dilation,
                            tensor=None,
                            init_method=None,
-                           device=None)
+                           device=None,
+                           dtype=None)
         new_mps.name = self.name + '_copy'
         if share_tensors:
             new_mps.uniform_memory.tensor = self.uniform_memory.tensor
         else:
             new_mps.uniform_memory.tensor = self.uniform_memory.tensor.clone()
         
         return new_mps
@@ -3881,14 +3937,16 @@
         ``tensors`` contains a single element, it can be rank-1 ("obc") or
         rank-3 ("pbc").
     init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit"}, optional
         Initialization method. Check :meth:`~MPSLayer.initialize` for a more detailed
         explanation of the different initialization methods.
     device : torch.device, optional
         Device where to initialize the tensors if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+        Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         
     Examples
     --------
     >>> conv_mps_layer = tk.models.ConvMPSLayer(in_channels=2,
@@ -3910,14 +3968,15 @@
                  padding: int = 0,
                  dilation: int = 1,
                  out_position: Optional[int] = None,
                  boundary: Text = 'obc',
                  tensors: Optional[Sequence[torch.Tensor]] = None,
                  init_method: Text = 'randn',
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs):
 
         unfold = self._set_attributes(in_channels=in_channels,
                                       kernel_size=kernel_size,
                                       stride=stride,
                                       padding=padding,
                                       dilation=dilation)
@@ -3930,14 +3989,15 @@
                           bond_dim=bond_dim,
                           out_position=out_position,
                           boundary=boundary,
                           tensors=tensors,
                           n_batches=2,
                           init_method=init_method,
                           device=device,
+                          dtype=dtype,
                           **kwargs)
         
         self._out_channels = out_channels
         self.unfold = unfold
     
     @property
     def in_channels(self) -> int:
@@ -4005,15 +4065,16 @@
                                kernel_size=self._kernel_size,
                                stride=self._stride,
                                padding=self._padding,
                                dilation=self.dilation,
                                boundary=self._boundary,
                                tensors=None,
                                init_method=None,
-                               device=None)
+                               device=None,
+                               dtype=None)
         new_mps.name = self.name + '_copy'
         if share_tensors:
             for new_node, node in zip(new_mps._mats_env, self._mats_env):
                 new_node.tensor = node.tensor
         else:
             for new_node, node in zip(new_mps._mats_env, self._mats_env):
                 new_node.tensor = node.tensor.clone()
@@ -4066,14 +4127,16 @@
         output node's tensor. Both tensors should be rank-3, with all their
         first and last dimensions being equal.
     init_method : {"zeros", "ones", "copy", "rand", "randn", "randn_eye", "unit"}, optional
         Initialization method. Check :meth:`~UMPSLayer.initialize` for a more
         detailed explanation of the different initialization methods.
     device : torch.device, optional
         Device where to initialize the tensors if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+        Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         
     Examples
     --------
     >>> conv_mps_layer = tk.models.ConvUMPSLayer(in_channels=2,
@@ -4098,14 +4161,15 @@
                  stride: int = 1,
                  padding: int = 0,
                  dilation: int = 1,
                  out_position: Optional[int] = None,
                  tensors: Optional[Sequence[torch.Tensor]] = None,
                  init_method: Text = 'randn',
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs):
 
         unfold = self._set_attributes(in_channels=in_channels,
                                       kernel_size=kernel_size,
                                       stride=stride,
                                       padding=padding,
                                       dilation=dilation)
@@ -4117,14 +4181,15 @@
                            out_dim=out_channels,
                            bond_dim=bond_dim,
                            out_position=out_position,
                            tensors=tensors,
                            n_batches=2,
                            init_method=init_method,
                            device=device,
+                           dtype=dtype,
                            **kwargs)
         
         self._out_channels = out_channels
         self.unfold = unfold
     
     @property
     def in_channels(self) -> int:
@@ -4196,15 +4261,16 @@
                                 bond_dim=self._bond_dim[0],
                                 kernel_size=self._kernel_size,
                                 stride=self._stride,
                                 padding=self._padding,
                                 dilation=self.dilation,
                                 tensor=None,
                                 init_method=None,
-                                device=None)
+                                device=None,
+                                dtype=None)
         new_mps.name = self.name + '_copy'
         if share_tensors:
             new_mps.uniform_memory.tensor = self.uniform_memory.tensor
             new_mps.out_node.tensor = self.out_node.tensor
         else:
             new_mps.uniform_memory.tensor = self.uniform_memory.tensor.clone()
             new_mps.out_node.tensor = self.out_node.tensor.clone()
```

### Comparing `tensorkrowch-1.1.3/tensorkrowch/models/mps_data.py` & `tensorkrowch-1.1.4/tensorkrowch/models/mps_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,16 @@
         Initialization method. Check :meth:`initialize` for a more detailed
         explanation of the different initialization methods. By default it is
         ``None``, since ``MPSData`` is intended to store input data vectors in
         MPS form, rather than initializing its own random tensors. Check
         :meth:`add_data` to see how to initialize MPS nodes with data tensors.
     device : torch.device, optional
         Device where to initialize the tensors if ``init_method`` is provided.
+    dtype : torch.dtype, optional
+            Dtype of the tensor if ``init_method`` is provided.
     kwargs : float
         Keyword arguments for the different initialization methods. See
         :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         
     Examples
     --------
     >>> mps = tk.models.MPSData(n_features=5,
@@ -108,14 +110,15 @@
                  phys_dim: Optional[Union[int, Sequence[int]]] = None,
                  bond_dim: Optional[Union[int, Sequence[int]]] = None,
                  boundary: Text = 'obc',
                  n_batches: int = 1,
                  tensors: Optional[Sequence[torch.Tensor]] = None,
                  init_method: Optional[Text] = None,
                  device: Optional[torch.device] = None,
+                 dtype: Optional[torch.dtype] = None,
                  **kwargs) -> None:
 
         super().__init__(name='mps_data')
         
         # n_batches
         if not isinstance(n_batches, int):
             raise TypeError('`n_batches` should be int type')
@@ -237,14 +240,15 @@
         self._right_node = None
         self._mats_env = []
 
         # Create Tensor Network
         self._make_nodes()
         self.initialize(init_method=init_method,
                             device=device,
+                            dtype=dtype,
                             **kwargs)
         
         if tensors is not None:
             self.add_data(data=tensors)
     
     # ----------
     # Properties
@@ -285,14 +289,23 @@
         return self._right_node
     
     @property
     def mats_env(self) -> List[AbstractNode]:
         """Returns the list of nodes in ``mats_env``."""
         return self._mats_env
     
+    @property
+    def tensors(self) -> List[torch.Tensor]:
+        """Returns the list of MPS tensors."""
+        mps_tensors = [node.tensor for node in self._mats_env]
+        if self._boundary == 'obc':
+            mps_tensors[0] = mps_tensors[0][0, :, :]
+            mps_tensors[-1] = mps_tensors[-1][:, :, 0]
+        return mps_tensors
+    
     # -------
     # Methods
     # -------
     def _make_nodes(self) -> None:
         """Creates all the nodes of the MPS."""
         if self._leaf_nodes:
             raise ValueError('Cannot create MPS nodes if the MPS already has '
@@ -342,48 +355,58 @@
                     self._left_node['right'] ^ self._mats_env[-1]['left']
                 if i == self._n_features - 1:
                     self._mats_env[-1]['right'] ^ self._right_node['left']
     
     def initialize(self,
                    init_method: Optional[Text] = 'randn',
                    device: Optional[torch.device] = None,
+                   dtype: Optional[torch.dtype] = None,
                    **kwargs: float) -> None:
         """
         Initializes all the nodes of the :class:`MPSData`. It can be called when
         instantiating the model, or to override the existing nodes' tensors.
         
         There are different methods to initialize the nodes:
         
         * ``{"zeros", "ones", "copy", "rand", "randn"}``: Each node is
           initialized calling :meth:`~tensorkrowch.AbstractNode.set_tensor` with
-          the given method, ``device`` and ``kwargs``.
+          the given method, ``device``, ``dtype`` and ``kwargs``.
         
         Parameters
         ----------
         init_method : {"zeros", "ones", "copy", "rand", "randn"}, optional
             Initialization method. Check :meth:`add_data` to see how to
             initialize MPS nodes with data tensors.
         device : torch.device, optional
             Device where to initialize the tensors if ``init_method`` is provided.
+        dtype : torch.dtype, optional
+            Dtype of the tensor if ``init_method`` is provided.
         kwargs : float
             Keyword arguments for the different initialization methods. See
             :meth:`~tensorkrowch.AbstractNode.make_tensor`.
         """
         if self._boundary == 'obc':
-            self._left_node.set_tensor(init_method='copy', device=device)
-            self._right_node.set_tensor(init_method='copy', device=device)
+            self._left_node.set_tensor(init_method='copy',
+                                       device=device,
+                                       dtype=dtype)
+            self._right_node.set_tensor(init_method='copy',
+                                        device=device,
+                                        dtype=dtype)
                 
         if init_method is not None:
             for i, node in enumerate(self._mats_env):
                 node.set_tensor(init_method=init_method,
                                 device=device,
+                                dtype=dtype,
                                 **kwargs)
                 
                 if self._boundary == 'obc':
-                    aux_tensor = torch.zeros(*node.shape, device=device)
+                    aux_tensor = torch.zeros(*node.shape,
+                                             device=device,
+                                             dtype=dtype)
                     if i == 0:
                         # Left node
                         aux_tensor[..., 0, :, :] = node.tensor[..., 0, :, :]
                         node.tensor = aux_tensor
                     elif i == (self._n_features - 1):
                         # Right node
                         aux_tensor[..., 0] = node.tensor[..., 0]
@@ -431,44 +454,52 @@
                         f'Physical dimension {data_tensor.shape[-2]} of '
                         f'data tensor at position {i} does not coincide '
                         f'with the corresponding physical dimension '
                         f'{node.shape[-2]} of the MPS')
         
         data = data[:]
         device = data[0].device
+        dtype = data[0].dtype
         for i, node in enumerate(self._mats_env):
             if self._boundary == 'obc':
-                aux_tensor = torch.zeros(*node.shape, device=device)
                 if (i == 0) and (i == (self._n_features - 1)):
                     aux_tensor = torch.zeros(*data[i].shape[:-1],
                                              *node.shape[-3:],
-                                             device=device)
+                                             device=device,
+                                             dtype=dtype)
                     aux_tensor[..., 0, :, 0] = data[i]
                     data[i] = aux_tensor
                 elif i == 0:
                     aux_tensor = torch.zeros(*data[i].shape[:-2],
                                              *node.shape[-3:-1],
                                              data[i].shape[-1],
-                                             device=device)
+                                             device=device,
+                                             dtype=dtype)
                     aux_tensor[..., 0, :, :] = data[i]
                     data[i] = aux_tensor
                 elif i == (self._n_features - 1):
                     aux_tensor = torch.zeros(*data[i].shape[:-1],
                                              *node.shape[-2:],
-                                             device=device)
+                                             device=device,
+                                             dtype=dtype)
                     aux_tensor[..., 0] = data[i]
                     data[i] = aux_tensor
                     
             node._direct_set_tensor(data[i])
         
-        # Send left and right nodes to correct device
+        # Send left and right nodes to correct device and dtype
         if self._boundary == 'obc':
             if self._left_node.device != device:
                 self._left_node.tensor = self._left_node.tensor.to(device)
+            if self._left_node.dtype != dtype:
+                self._left_node.tensor = self._left_node.tensor.to(dtype)
+            
             if self._right_node.device != device:
                 self._right_node.tensor = self._right_node.tensor.to(device)
+            if self._right_node.dtype != dtype:
+                self._right_node.tensor = self._right_node.tensor.to(dtype)
         
         # Update bond dim
         if self._boundary == 'obc':
             self._bond_dim = [node['right'].size() for node in self._mats_env[:-1]]
         else:
             self._bond_dim = [node['right'].size() for node in self._mats_env]
```

### Comparing `tensorkrowch-1.1.3/tensorkrowch/models/peps.py` & `tensorkrowch-1.1.4/tensorkrowch/models/peps.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.3/tensorkrowch/models/tree.py` & `tensorkrowch-1.1.4/tensorkrowch/models/tree.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.3/tensorkrowch/operations.py` & `tensorkrowch-1.1.4/tensorkrowch/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,19 @@
         * Operation
         
     Tensor-like operations:
         * permute
         * permute_           (in-place)
         * tprod
         * mul
+        * div
         * add
         * sub
+        * renormalize
+        * conj
         
     Node-like operations:
         * split
         * split_             (in-place)
         * svd                           (edge operation)
         * svd_               (in-place) (edge operation)
         * svdr                          (edge operation)
@@ -1462,14 +1465,128 @@
     >>> renormA.norm()
     tensor(1.)
     """
 
 AbstractNode.renormalize = renormalize_node
 
 
+##################################   conj    ##################################
+# MARK: conj
+def _check_first_conj(node: AbstractNode) -> Optional[Successor]:
+    args = (node,)
+    successors = node._successors.get('conj')
+    if not successors:
+        return None
+    return successors.get(args)
+
+
+def _conj_first(node: AbstractNode) -> Node:
+    new_node = Node._create_resultant(axes_names=node.axes_names,
+                                      name='conj',
+                                      network=node._network,
+                                      tensor=node.tensor.conj(),
+                                      edges=node._edges,
+                                      node1_list=node.is_node1())
+    
+    # Create successor
+    net = node._network
+    args = (node,)
+    successor = Successor(node_ref=node.node_ref(),
+                          index=node._tensor_info['index'],
+                          child=new_node)
+
+    # Add successor to parent
+    if 'conj' in node._successors:
+        node._successors['conj'].update({args: successor})
+    else:
+        node._successors['conj'] = {args: successor}
+
+    # Add operation to list of performed operations of TN
+    net._seq_ops.append(('conj', args))
+
+    # Record in inverse_memory while tracing
+    if net._tracing:
+        node._record_in_inverse_memory()
+
+    return new_node
+
+
+def _conj_next(successor: Successor, node: AbstractNode) -> Node:
+    tensor = node._direct_get_tensor(successor.node_ref,
+                                     successor.index)
+    child = successor.child
+    child._direct_set_tensor(tensor.conj())
+
+    # Record in inverse_memory while contracting, if network is traced
+    # (to delete memory if possible)
+    if node._network._traced:
+        node._check_inverse_memory(successor.node_ref)
+    
+    return child
+
+
+conj_op = Operation('conj',
+                    _check_first_conj,
+                    _conj_first,
+                    _conj_next)
+
+
+def conj(node: AbstractNode) -> Node:
+    """
+    Returns a view of the node's tensor with a flipped conjugate bit. If the
+    node has a non-complex dtype, this function returns a new node with the
+    same tensor.
+
+    See `conj <https://pytorch.org/docs/stable/generated/torch.conj.html>`_
+    in the **PyTorch** documentation.
+
+    Parameters
+    ----------
+    node : Node or ParamNode
+        Node that is to be conjugated.
+
+    Returns
+    -------
+    Node
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn((3, 3), dtype=torch.complex64)
+    >>> conjA = tk.conj(nodeA)
+    >>> conjA.is_conj()
+    True
+    """
+    return conj_op(node)
+
+
+conj_node = copy_func(conj)
+conj_node.__doc__ = \
+    """
+    Returns a view of the node's tensor with a flipped conjugate bit. If the
+    node has a non-complex dtype, this function returns a new node with the
+    same tensor.
+
+    See `conj <https://pytorch.org/docs/stable/generated/torch.conj.html>`_
+    in the **PyTorch** documentation.
+
+    Returns
+    -------
+    Node
+    
+    Examples
+    --------
+    >>> nodeA = tk.randn((3, 3), dtype=torch.complex64)
+    >>> conjA = nodeA.conj()
+    >>> conjA.is_conj()
+    True
+    """
+
+AbstractNode.conj = conj_node
+
+
 ###############################################################################
 #                            NODE-LIKE OPERATIONS                             #
 ###############################################################################
 
 ##################################   SPLIT    #################################
 # MARK: split
 def _check_first_split(node: AbstractNode,
@@ -1595,17 +1712,20 @@
         
         # Select rank from specified restrictions
         rank = min(lst_ranks)
         
         u = u[..., :rank]
         s = s[..., :rank]
         vh = vh[..., :rank, :]
+        
+        if u.is_complex():
+            s = s.to(u.dtype)
 
         if mode == 'svdr':
-            phase = torch.sign(torch.randn(s.shape))
+            phase = torch.sgn(torch.randn_like(s))
             phase = torch.diag_embed(phase)
             u = u @ phase
             vh = phase @ vh
 
         if side == 'left':
             u = u @ torch.diag_embed(s)
         elif side == 'right':
@@ -1794,17 +1914,20 @@
         
         # Select rank from specified restrictions
         rank = min(lst_ranks)
         
         u = u[..., :rank]
         s = s[..., :rank]
         vh = vh[..., :rank, :]
+        
+        if u.is_complex():
+            s = s.to(u.dtype)
 
         if mode == 'svdr':
-            phase = torch.sign(torch.randn(s.shape))
+            phase = torch.sgn(torch.randn_like(s))
             phase = torch.diag_embed(phase)
             u = u @ phase
             vh = phase @ vh
 
         if side == 'left':
             u = u @ torch.diag_embed(s)
         elif side == 'right':
```

### Comparing `tensorkrowch-1.1.3/tensorkrowch/utils.py` & `tensorkrowch-1.1.4/tensorkrowch/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,20 +303,22 @@
         else:
             regions.append(current_region)
             current_region = [lst[i]]
 
     regions.append(current_region)
     return regions
 
-def random_unitary(n, device: Optional[torch.device] = None):
+def random_unitary(n,
+                   device: Optional[torch.device] = None,
+                   dtype: Optional[torch.dtype] = None):
     """
     Returns random unitary matrix from the Haar measure of size n x n.
     
     Unitary matrix is created as described in this `paper
     <https://arxiv.org/abs/math-ph/0609050v2>`_.
     """
-    mat = torch.randn(n, n, device=device)
+    mat = torch.randn(n, n, device=device, dtype=dtype)
     q, r = torch.linalg.qr(mat)
     d = torch.diagonal(r)
     ph = d / d.abs()
     q = q @ torch.diag(ph)
     return q
```

### Comparing `tensorkrowch-1.1.3/tensorkrowch.egg-info/PKG-INFO` & `tensorkrowch-1.1.4/tensorkrowch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorkrowch
-Version: 1.1.3
+Version: 1.1.4
 Summary: Tensor Networks with PyTorch
 Author-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 Maintainer-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 José Ramón Pareja Monturiol
```

### Comparing `tensorkrowch-1.1.3/tensorkrowch.egg-info/SOURCES.txt` & `tensorkrowch-1.1.4/tensorkrowch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

