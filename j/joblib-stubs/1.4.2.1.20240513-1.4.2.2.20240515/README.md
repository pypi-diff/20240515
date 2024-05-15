# Comparing `tmp/joblib_stubs-1.4.2.1.20240513.tar.gz` & `tmp/joblib_stubs-1.4.2.2.20240515.tar.gz`

## Comparing `joblib_stubs-1.4.2.1.20240513.tar` & `joblib_stubs-1.4.2.2.20240515.tar`

### file list

```diff
@@ -1,52 +1,54 @@
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/ruff.toml
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/__init__.pyi
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/_cloudpickle_wrapper.pyi
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/_dask.pyi
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/_memmapping_reducer.pyi
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/_multiprocessing_helpers.pyi
--rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/_parallel_backends.pyi
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/_store_backends.pyi
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/_utils.pyi
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/backports.pyi
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/compressor.pyi
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/disk.pyi
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/executor.pyi
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/func_inspect.pyi
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/hashing.pyi
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/logger.pyi
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/memory.pyi
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/numpy_pickle.pyi
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/numpy_pickle_compat.pyi
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/numpy_pickle_utils.pyi
--rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/parallel.pyi
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/pool.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/__init__.pyi
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/cloudpickle/__init__.pyi
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/cloudpickle/cloudpickle.pyi
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/cloudpickle/cloudpickle_fast.pyi
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/__init__.pyi
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/_base.pyi
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/cloudpickle_wrapper.pyi
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/initializers.pyi
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/process_executor.pyi
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/reusable_executor.pyi
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/__init__.pyi
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/_posix_reduction.pyi
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/_win_reduction.pyi
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/context.pyi
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/fork_exec.pyi
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/popen_loky_posix.pyi
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/popen_loky_win32.pyi
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/process.pyi
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/queues.pyi
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/reduction.pyi
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/resource_tracker.pyi
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/spawn.pyi
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/synchronize.pyi
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/utils.pyi
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/LICENSE
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/README.md
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/pyproject.toml
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.1.20240513/PKG-INFO
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/ruff.toml
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/.vscode/extensions.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/.vscode/settings.json
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/__init__.pyi
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/_cloudpickle_wrapper.pyi
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/_dask.pyi
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/_memmapping_reducer.pyi
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/_multiprocessing_helpers.pyi
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/_parallel_backends.pyi
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/_store_backends.pyi
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/_utils.pyi
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/backports.pyi
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/compressor.pyi
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/disk.pyi
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/executor.pyi
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/func_inspect.pyi
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/hashing.pyi
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/logger.pyi
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/memory.pyi
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/numpy_pickle.pyi
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/numpy_pickle_compat.pyi
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/numpy_pickle_utils.pyi
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/parallel.pyi
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/pool.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/__init__.pyi
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/cloudpickle/__init__.pyi
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/cloudpickle/cloudpickle.pyi
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/cloudpickle/cloudpickle_fast.pyi
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/__init__.pyi
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/_base.pyi
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/cloudpickle_wrapper.pyi
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/initializers.pyi
+-rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/process_executor.pyi
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/reusable_executor.pyi
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/__init__.pyi
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/_posix_reduction.pyi
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/_win_reduction.pyi
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/context.pyi
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/fork_exec.pyi
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/popen_loky_posix.pyi
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/popen_loky_win32.pyi
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/process.pyi
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/queues.pyi
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/reduction.pyi
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/resource_tracker.pyi
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/spawn.pyi
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/synchronize.pyi
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/utils.pyi
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/LICENSE
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/README.md
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/pyproject.toml
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 joblib_stubs-1.4.2.2.20240515/PKG-INFO
```

### Comparing `joblib_stubs-1.4.2.1.20240513/ruff.toml` & `joblib_stubs-1.4.2.2.20240515/ruff.toml`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/.github/workflows/publish.yaml` & `joblib_stubs-1.4.2.2.20240515/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/__init__.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/_dask.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/_dask.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 import typing
 import weakref
 from concurrent import futures
 from multiprocessing.pool import AsyncResult as AsyncResult
 
+import typing_extensions
 from dask.distributed import Client as Client
 from dask.distributed import Future as Future
 from distributed.deploy.cluster import Cluster as Cluster
-from joblib.parallel import _R
 from joblib.parallel import AutoBatchingMixin as AutoBatchingMixin
 from joblib.parallel import Parallel as Parallel
 from joblib.parallel import ParallelBackendBase as ParallelBackendBase
+from joblib.parallel import _ReturnAs as _ReturnAs
 from joblib.parallel import parallel_config as parallel_config
 from tornado.ioloop import IOLoop as IOLoop
 
+_T = typing_extensions.TypeVar("_T")
+_P = typing_extensions.ParamSpec("_P")
+_R = typing_extensions.TypeVar(
+    "_R",
+    default=typing.Literal["list"],
+    bound="_ReturnAs",  # noqa: PYI020
+)
+
 def is_weakrefable(obj: typing.Any) -> bool: ...
 
 class _WeakKeyDictionary:
     def __init__(self) -> None: ...
     def __getitem__(self, obj: typing.Any) -> typing.Any: ...
     def __setitem__(self, obj: typing.Any, value: typing.Any) -> None: ...
     def __len__(self) -> int: ...
     def clear(self) -> None: ...
 
-type _TaskItem[**P, T] = tuple[
-    typing.Callable[P, T], list[typing.Any], dict[str, typing.Any]
+_TaskItem: typing_extensions.TypeAlias = tuple[
+    typing.Callable[_P, _T], list[typing.Any], dict[str, typing.Any]
 ]
 
-class Batch[T]:
-    def __init__(self, tasks: list[_TaskItem[..., T]]) -> None: ...
-    def __call__(self, tasks: list[_TaskItem[..., T]] | None = ...) -> list[T]: ...
-
-type _ScatterIterItem = list[typing.Any] | dict[typing.Any, typing.Any]
+class Batch(typing.Generic[_T]):
+    def __init__(self, tasks: list[_TaskItem[..., _T]]) -> None: ...
+    def __call__(self, tasks: list[_TaskItem[..., _T]] | None = ...) -> list[_T]: ...
+
+_ScatterIterItem: typing_extensions.TypeAlias = (
+    list[typing.Any] | dict[typing.Any, typing.Any]
+)
 
 class DaskDistributedBackend(
     AutoBatchingMixin[_R], ParallelBackendBase[_R], typing.Generic[_R]
 ):
     MIN_IDEAL_BATCH_DURATION: typing.ClassVar[float]
-    MAX_IDEAL_BATCH_DURATION: typing.ClassVar[float]
     client: Client
     data_futures: dict[int, Future]
     wait_for_workers_timeout: float
     submit_kwargs: dict[str, typing.Any]
     waiting_futures: typing.Iterator[Future]
     def __init__(
         self,
@@ -48,23 +58,25 @@
         scatter: _ScatterIterItem | typing.Any | None = ...,
         client: Client | None = ...,
         loop: IOLoop | None = ...,
         wait_for_workers_timeout: float = ...,
         **submit_kwargs: typing.Any,
     ) -> None: ...
     def __reduce__(self) -> tuple[type[DaskDistributedBackend], tuple[()]]: ...
-    def get_nested_backend(
+    def get_nested_backend(  # type: ignore[override]
         self,
     ) -> tuple[DaskDistributedBackend, typing.Literal[-1]]: ...
-    parallel: Parallel
-    def configure(
+    parallel: Parallel[_R]
+    def configure(  # type: ignore[override]
         self,
         n_jobs: int = ...,
-        parallel: Parallel | None = ...,
+        parallel: Parallel[_R] | None = ...,
         **backend_args: typing.Any,
     ) -> int: ...
     call_data_futures: weakref.WeakKeyDictionary[typing.Any, typing.Any]
-    def apply_async[T](
+    def apply_async(
         self,
-        func: typing.Callable[[], T],
-        callback: typing.Callable[[T], typing.Any] | None = ...,
-    ) -> futures.Future[T]: ...
+        func: typing.Callable[[], _T],
+        callback: typing.Callable[[_T], typing.Any] | None = ...,
+    ) -> futures.Future[_T]: ...
+    # mypy
+    def effective_n_jobs(self, n_jobs: int) -> int: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/_memmapping_reducer.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/_memmapping_reducer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from joblib.disk import delete_folder as delete_folder
 from joblib.externals.loky.backend import resource_tracker as resource_tracker
 from joblib.numpy_pickle import dump as dump
 from joblib.numpy_pickle import load as load
 from joblib.numpy_pickle import load_temporary_memmap as load_temporary_memmap
 from numpy.typing import ArrayLike, NDArray
 
-type _MmapMode = typing.Literal["r+", "r", "w+", "c"]
+_MmapMode: typing_extensions.TypeAlias = typing.Literal["r+", "r", "w+", "c"]
 
 WindowsError: type[OSError | None]
 SYSTEM_SHARED_MEM_FS: str
 SYSTEM_SHARED_MEM_FS_MIN_SIZE: int
 FOLDER_PERMISSIONS: int
 FILE_PERMISSIONS: int
 JOBLIB_MMAPS: set[str]
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/_parallel_backends.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/_parallel_backends.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 import typing
 from abc import ABCMeta, abstractmethod
 from collections.abc import Generator
 from concurrent import futures
 from multiprocessing.pool import AsyncResult as AsyncResult
 
+import typing_extensions
 from joblib._multiprocessing_helpers import mp as mp
 from joblib.executor import get_memmapping_executor as get_memmapping_executor
 from joblib.externals.loky import cpu_count as cpu_count
 from joblib.externals.loky import process_executor as process_executor
 from joblib.externals.loky.process_executor import (
     ShutdownExecutorError as ShutdownExecutorError,
 )
-from joblib.parallel import _R
 from joblib.parallel import Parallel as Parallel
+from joblib.parallel import _ReturnAs as _ReturnAs
 from joblib.pool import MemmappingPool as MemmappingPool
 
-type _Prefer = typing.Literal["processes", "threads"]
-type _Require = typing.Literal["sharedmem"]
+_T = typing_extensions.TypeVar("_T")
+_T_co = typing_extensions.TypeVar("_T_co", covariant=True)
+_R = typing_extensions.TypeVar(
+    "_R",
+    default=typing.Literal["list"],
+    bound="_ReturnAs",  # noqa: PYI020
+)
+
+class _AnyContainer(typing.Protocol[_T_co]): ...  # mypy override error
+
+_Prefer: typing_extensions.TypeAlias = typing.Literal["processes", "threads"]
+_Require: typing_extensions.TypeAlias = typing.Literal["sharedmem"]
 
 class ParallelBackendBase(typing.Generic[_R], metaclass=ABCMeta):
     supports_inner_max_num_threads: typing.ClassVar[bool]
     supports_retrieve_callback: typing.ClassVar[bool]
     default_n_jobs: typing.ClassVar[int]
     @property
     def supports_return_generator(self) -> bool: ...
@@ -35,25 +46,23 @@
         **kwargs: typing.Any,
     ) -> None: ...
     MAX_NUM_THREADS_VARS: typing.ClassVar[list[str]]
     TBB_ENABLE_IPC_VAR: typing.ClassVar[str]
     @abstractmethod
     def effective_n_jobs(self, n_jobs: int) -> int: ...
     @abstractmethod
-    def apply_async[T](
+    def apply_async(
         self,
-        func: typing.Callable[[], T],
-        callback: typing.Callable[[futures.Future[T] | AsyncResult[T]], typing.Any]
-        | typing.Callable[[futures.Future[T]], typing.Any]
-        | typing.Callable[[AsyncResult[T]], typing.Any]
+        func: typing.Callable[[], _T],
+        callback: typing.Callable[[_AnyContainer[_T]], typing.Any]  # FIXME: mypy error
         | None = ...,
-    ) -> futures.Future[T] | AsyncResult[T]: ...
-    def retrieve_result_callback[T](
-        self, out: futures.Future[T] | AsyncResult[T]
-    ) -> T: ...
+    ) -> _AnyContainer[_T]: ...
+    def retrieve_result_callback(
+        self, out: futures.Future[_T] | AsyncResult[_T]
+    ) -> _T: ...
     parallel: Parallel[_R]
     def configure(
         self,
         n_jobs: int = ...,
         parallel: Parallel[_R] | None = ...,
         prefer: _Prefer | None = ...,
         require: _Require | None = ...,
@@ -81,23 +90,25 @@
     supports_retrieve_callback: typing.ClassVar[bool]
     supports_sharedmem: typing.ClassVar[bool]
     def apply_async(
         self,
         func: typing.Callable[[], typing.Any],
         callback: typing.Callable[..., typing.Any] | None = ...,
     ) -> typing.NoReturn: ...
+    # mypy
+    def effective_n_jobs(self, n_jobs: int) -> int: ...
 
 class PoolManagerMixin:
     def effective_n_jobs(self, n_jobs: int) -> int: ...
     def terminate(self) -> None: ...
-    def apply_async[T](
+    def apply_async(
         self,
-        func: typing.Callable[[], T],
-        callback: typing.Callable[[AsyncResult[T]], typing.Any] | None = ...,
-    ) -> AsyncResult[T]: ...
+        func: typing.Callable[[], _T],
+        callback: typing.Callable[[AsyncResult[_T]], typing.Any] | None = ...,
+    ) -> AsyncResult[_T]: ...
     def retrieve_result_callback(self, out: typing.Any) -> typing.Any: ...
     def abort_everything(self, ensure_ready: bool = ...) -> None: ...
 
 class AutoBatchingMixin(typing.Generic[_R]):
     MIN_IDEAL_BATCH_DURATION: typing.ClassVar[float]
     MAX_IDEAL_BATCH_DURATION: typing.ClassVar[int]
     parallel: Parallel[_R]
@@ -106,53 +117,55 @@
     def batch_completed(self, batch_size: int, duration: float) -> None: ...
     def reset_batch_stats(self) -> None: ...
 
 class ThreadingBackend(PoolManagerMixin, ParallelBackendBase[_R], typing.Generic[_R]):
     supports_retrieve_callback: typing.ClassVar[bool]
     uses_threads: typing.ClassVar[bool]
     supports_sharedmem: typing.ClassVar[bool]
-    def configure(
+    def configure(  # type: ignore[override]
         self,
         n_jobs: int = ...,
         parallel: Parallel[_R] | None = ...,
         **backend_args: typing.Any,
     ) -> int: ...
 
-class MultiprocessingBackend(
+class MultiprocessingBackend(  # type: ignore[misc] # FIXME
     PoolManagerMixin, AutoBatchingMixin[_R], ParallelBackendBase[_R], typing.Generic[_R]
 ):
     supports_retrieve_callback: typing.ClassVar[bool]
     supports_return_generator: typing.ClassVar[bool]
     def configure(
         self,
         n_jobs: int = ...,
         parallel: Parallel[_R] | None = ...,
         prefer: _Prefer | None = ...,
         require: _Require | None = ...,
         **memmappingpool_args: typing.Any,
     ) -> int: ...
 
-class LokyBackend(AutoBatchingMixin[_R], ParallelBackendBase[_R], typing.Generic[_R]):
+class LokyBackend(AutoBatchingMixin[_R], ParallelBackendBase[_R], typing.Generic[_R]):  # type: ignore[misc] # FIXME
     supports_retrieve_callback: typing.ClassVar[bool]
     supports_inner_max_num_threads: typing.ClassVar[bool]
     def configure(
         self,
         n_jobs: int = ...,
         parallel: Parallel[_R] | None = ...,
         prefer: _Prefer | None = ...,
         require: _Require | None = ...,
         idle_worker_timeout: float = ...,
         **memmappingexecutor_args: typing.Any,
     ) -> int: ...
     def terminate(self) -> None: ...
     def abort_everything(self, ensure_ready: bool = ...) -> None: ...
-    def apply_async[T](
+    def apply_async(
         self,
-        func: typing.Callable[[], T],
-        callback: typing.Callable[[futures.Future[T]], typing.Any] | None = ...,
-    ) -> futures.Future[T]: ...
+        func: typing.Callable[[], _T],
+        callback: typing.Callable[[futures.Future[_T]], typing.Any] | None = ...,
+    ) -> futures.Future[_T]: ...
+    # mypy
+    def effective_n_jobs(self, n_jobs: int) -> int: ...
 
 class FallbackToBackend(Exception):  # noqa: N818
     backend: ParallelBackendBase[typing.Any]
     def __init__(self, backend: ParallelBackendBase[typing.Any]) -> None: ...
 
 def inside_dask_worker() -> bool: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/_store_backends.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/_store_backends.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import typing
 from abc import ABCMeta, abstractmethod
 from datetime import datetime, timedelta
 
+import typing_extensions
 from joblib import numpy_pickle as numpy_pickle
 from joblib._memmapping_reducer import _MmapMode
 from joblib.backports import concurrency_safe_rename as concurrency_safe_rename
 from joblib.disk import memstr_to_bytes as memstr_to_bytes
 from joblib.disk import mkdirp as mkdirp
 from joblib.disk import rm_subdirs as rm_subdirs
 from joblib.logger import format_time as format_time
 
+_T = typing_extensions.TypeVar("_T")
+
 class _ItemInfo(typing.TypedDict, total=True):
     location: str
 
 class CacheItemInfo(typing.NamedTuple):
     path: str
     size: int
     last_access: datetime
 
 class CacheWarning(Warning): ...
 
-def concurrency_safe_write[T](
-    object_to_write: T, filename: str, write_func: typing.Callable[[T, str], typing.Any]
+def concurrency_safe_write(
+    object_to_write: _T,
+    filename: str,
+    write_func: typing.Callable[[_T, str], typing.Any],
 ) -> str: ...
 
 class StoreBackendBase(metaclass=ABCMeta):
     location: str
     @abstractmethod
     def create_location(self, location: str) -> None: ...
     @abstractmethod
@@ -73,7 +78,17 @@
         age_limit: timedelta | None = ...,
     ) -> None: ...
 
 class FileSystemStoreBackend(StoreBackendBase, StoreBackendMixin):
     compress: bool
     mmap_mode: _MmapMode
     verbose: int
+    # mypy
+    def create_location(self, location: str) -> None: ...
+    def clear_location(self, location: str) -> None: ...
+    def get_items(self) -> list[CacheItemInfo]: ...
+    def configure(
+        self,
+        location: str,
+        verbose: int = ...,
+        backend_options: dict[str, typing.Any] | None = ...,
+    ) -> None: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/_utils.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/_utils.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import ast
 import typing
 from dataclasses import dataclass
 
+import typing_extensions
 from joblib._multiprocessing_helpers import mp as mp
 
+_T = typing_extensions.TypeVar("_T")
+_P = typing_extensions.ParamSpec("_P")
+
 operators: dict[ast.AST, typing.Callable[[typing.Any, typing.Any], typing.Any]]
 
 def eval_expr(expr: str) -> typing.Any: ...
 def eval_(node: ast.AST) -> typing.Any: ...
 @dataclass(frozen=True)
-class _Sentinel[T]:
-    default_value: T
-    def __init__(self, default_value: T) -> None: ...
+class _Sentinel(typing.Generic[_T]):
+    default_value: _T
+    def __init__(self, default_value: _T) -> None: ...
 
-class _TracebackCapturingWrapper[**P, T]:
-    func: typing.Callable[P, T]
-    def __init__(self, func: typing.Callable[P, T]) -> None: ...
-    def __call__(self, **kwargs: typing.Any) -> T: ...
+class _TracebackCapturingWrapper(typing.Generic[_P, _T]):
+    func: typing.Callable[_P, _T]
+    def __init__(self, func: typing.Callable[_P, _T]) -> None: ...
+    def __call__(self, **kwargs: typing.Any) -> _T: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/backports.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/backports.pyi`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/compressor.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/compressor.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import bz2
 import io
 import lzma
 import typing
 from io import BufferedIOBase as BufferedIOBase
 
+import typing_extensions
+from _typeshed import ReadableBuffer, WriteableBuffer
 from joblib.backports import LooseVersion as LooseVersion
 from lz4.frame import LZ4FrameFile  # type: ignore
 
+_BufferedIOBaseT = typing_extensions.TypeVar("_BufferedIOBaseT", bound=BufferedIOBase)
+
 LZ4_NOT_INSTALLED_ERROR: str
-_COMPRESSORS: dict[str, CompressorWrapper]
+_COMPRESSORS: dict[str, CompressorWrapper[typing.Any]]
 _ZFILE_PREFIX: bytes
 _ZLIB_PREFIX: bytes
 _GZIP_PREFIX: bytes
 _BZ2_PREFIX: bytes
 _XZ_PREFIX: bytes
 _LZMA_PREFIX: bytes
 _LZ4_PREFIX: bytes
 
 def register_compressor(
-    compressor_name: str, compressor: CompressorWrapper, force: bool = ...
+    compressor_name: str, compressor: CompressorWrapper[typing.Any], force: bool = ...
 ) -> None: ...
 
-class CompressorWrapper[T: BufferedIOBase]:
-    fileobj_factory: type[T]
+class CompressorWrapper(typing.Generic[_BufferedIOBaseT]):
+    fileobj_factory: type[_BufferedIOBaseT]
     prefix: bytes
     extension: str
     def __init__(
         self, obj: typing.Any, prefix: bytes = ..., extension: str = ...
     ) -> None: ...
     def compressor_file(
         self, fileobj: typing.Any, compresslevel: int | None = ...
-    ) -> T: ...
-    def decompressor_file(self, fileobj: typing.Any) -> T: ...
+    ) -> _BufferedIOBaseT: ...
+    def decompressor_file(self, fileobj: typing.Any) -> _BufferedIOBaseT: ...
 
 class BZ2CompressorWrapper(CompressorWrapper[bz2.BZ2File]): ...
 class LZMACompressorWrapper(CompressorWrapper[lzma.LZMAFile]): ...
 class XZCompressorWrapper(LZMACompressorWrapper): ...
 class LZ4CompressorWrapper(CompressorWrapper[LZ4FrameFile]): ...
 
 _MODE_CLOSED: typing.Literal[0]
@@ -56,17 +60,17 @@
     def close(self) -> None: ...
     @property
     def closed(self) -> bool: ...
     def fileno(self) -> int: ...
     def seekable(self) -> bool: ...
     def readable(self) -> bool: ...
     def writable(self) -> bool: ...
-    def read(self, size: int = ...) -> bytes | None: ...
-    def readinto(self, b: bytes) -> int: ...
-    def write(self, data: bytes) -> int: ...
+    def read(self, size: int = ...) -> bytes | None: ...  # type: ignore[override]
+    def readinto(self, b: WriteableBuffer) -> int: ...
+    def write(self, data: ReadableBuffer) -> int: ...
     def seek(self, offset: int, whence: int = ...) -> int: ...
     def tell(self) -> int: ...
 
 class ZlibCompressorWrapper(CompressorWrapper[BinaryZlibFile]):
     def __init__(self) -> None: ...
 
 class BinaryGzipFile(BinaryZlibFile): ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/disk.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/disk.pyi`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/executor.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/executor.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import typing
 from concurrent import futures
 
+import typing_extensions
 from joblib._memmapping_reducer import (
     TemporaryResourcesManager as TemporaryResourcesManager,
 )
 from joblib._memmapping_reducer import (
     get_memmapping_reducers as get_memmapping_reducers,
 )
 from joblib.externals.loky.reusable_executor import _ReusablePoolExecutor
 
+_T = typing_extensions.TypeVar("_T")
+
 def get_memmapping_executor(n_jobs: int, **kwargs: typing.Any) -> futures.Executor: ...
 
 class MemmappingExecutor(_ReusablePoolExecutor):
     @classmethod
     def get_memmapping_executor(
         cls,
         n_jobs: int,
@@ -23,13 +26,13 @@
         temp_folder: str | None = ...,
         context_id: tuple[str, ...] | None = ...,
         **backend_args: typing.Any,
     ) -> futures.Executor: ...
     def terminate(self, kill_workers: bool = ...) -> None: ...
 
 class _TestingMemmappingExecutor(MemmappingExecutor):
-    def apply_async[T](
-        self, func: typing.Callable[..., T], args: tuple[typing.Any, ...]
-    ) -> futures.Future[T]: ...
-    def map[T](
-        self, f: typing.Callable[..., T], *args: typing.Iterable[typing.Any]
-    ) -> list[T]: ...
+    def apply_async(
+        self, func: typing.Callable[..., _T], args: tuple[typing.Any, ...]
+    ) -> futures.Future[_T]: ...
+    def map(
+        self, f: typing.Callable[..., _T], *args: typing.Iterable[typing.Any]
+    ) -> list[_T]: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/func_inspect.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/func_inspect.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import types
 import typing
 
+import typing_extensions
 from joblib.logger import pformat as pformat
 
+_P = typing_extensions.ParamSpec("_P")
+
 full_argspec_fields: str
 
 class _FullArgSpec(typing.NamedTuple):
     args: list[str]
     varargs: str
     varkw: str
     defaults: tuple[typing.Any, ...]
@@ -24,16 +27,16 @@
 ) -> tuple[list[str], str]: ...
 def filter_args(
     func: typing.Callable[..., typing.Any],
     ignore_lst: list[str],
     args: tuple[typing.Any, ...] = ...,
     kwargs: dict[str, typing.Any] = ...,
 ) -> dict[str, typing.Any]: ...
-def format_signature[**P](
-    func: typing.Callable[P, typing.Any], *args: P.args, **kwargs: P.kwargs
+def format_signature(
+    func: typing.Callable[_P, typing.Any], *args: _P.args, **kwargs: _P.kwargs
 ) -> tuple[list[str], str]: ...
 def format_call(
     func: typing.Callable[..., typing.Any],
     args: tuple[typing.Any, ...],
     kwargs: dict[str, typing.Any],
     object_name: str = ...,
 ) -> str: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/hashing.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/hashing.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import types
 import typing
 
 import typing_extensions
 from joblib.pool import _Dispatch as _Dispatch
 
 Pickler = pickle.Pickler
-type _HashType = typing.Literal["md5", "sha1"]
+_HashType: typing_extensions.TypeAlias = typing.Literal["md5", "sha1"]
 
 class _ConsistentSet:
     def __init__(self, set_sequence: typing.Iterable[typing.Hashable]) -> None: ...
 
 class _MyHash:
     args: tuple[typing.Any]
     def __init__(self, *args: typing.Any) -> None: ...
@@ -26,15 +26,15 @@
         self,
         obj: typing.Any,
         name: str | None = ...,
         pack: typing.Callable[
             typing_extensions.Concatenate[str | bytes, ...], bytes
         ] = ...,
     ) -> None: ...
-    dispatch: dict[type[typing.Any], _Dispatch[typing.Any]]
+    # dispatch: dict[type[typing.Any], _Dispatch[typing.Any]]  # noqa: ERA001
     def save_set(self, set_items: typing.Iterable[typing.Hashable]) -> None: ...
 
 class NumpyHasher(Hasher):
     coerce_mmap: bool
     np: types.ModuleType
     def __init__(self, hash_name: _HashType = ..., coerce_mmap: bool = ...) -> None: ...
     def save(self, obj: typing.Any) -> None: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/logger.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/logger.pyi`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/memory.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/memory.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,76 @@
 import typing
 from datetime import timedelta
 
+import typing_extensions
 from joblib import hashing as hashing
 from joblib._store_backends import CacheWarning as CacheWarning
 from joblib._store_backends import FileSystemStoreBackend as FileSystemStoreBackend
 from joblib._store_backends import StoreBackendBase as StoreBackendBase
 from joblib.func_inspect import filter_args as filter_args
 from joblib.func_inspect import format_call as format_call
 from joblib.func_inspect import format_signature as format_signature
 from joblib.func_inspect import get_func_code as get_func_code
 from joblib.func_inspect import get_func_name as get_func_name
 from joblib.logger import Logger as Logger
 from joblib.logger import format_time as format_time
 from joblib.logger import pformat as pformat
 
+_T = typing_extensions.TypeVar("_T")
+_P = typing_extensions.ParamSpec("_P")
+
 FIRST_LINE_TEXT: str
 _STORE_BACKENDS: dict[str, type[StoreBackendBase]]
-type _MmepMode = typing.Literal["r+", "r", "w+", "c"]
-type _AnyAwaitable[T] = (
-    typing.Awaitable[T] | typing.Coroutine[typing.Any, typing.Any, T]
+_MmepMode: typing_extensions.TypeAlias = typing.Literal["r+", "r", "w+", "c"]
+_AnyAwaitable: typing_extensions.TypeAlias = (
+    typing.Awaitable[_T] | typing.Coroutine[typing.Any, typing.Any, _T]
 )
-type _AnyAwaitableCallable[**P, T] = (
-    typing.Callable[P, typing.Awaitable[T]]
-    | typing.Callable[P, typing.Coroutine[typing.Any, typing.Any, T]]
+_AnyAwaitableCallable: typing_extensions.TypeAlias = (
+    typing.Callable[_P, typing.Awaitable[_T]]
+    | typing.Callable[_P, typing.Coroutine[typing.Any, typing.Any, _T]]
 )
 
 class _CacheFunc(typing.Protocol):
     @typing.overload
     def __call__(
         self,
         func: None,
         ignore: list[str] | None = ...,
         verbose: int | None = ...,
         mmap_mode: _MmepMode | bool = ...,
         cache_validation_callback: typing.Callable[..., typing.Any] | None = ...,
     ) -> _CacheFunc: ...
     @typing.overload
-    def __call__[**P, T](
+    def __call__(
         self,
-        func: _AnyAwaitableCallable[P, T],
+        func: _AnyAwaitableCallable[_P, _T],
         ignore: list[str] | None = ...,
         verbose: int | None = ...,
         mmap_mode: _MmepMode | bool = ...,
         cache_validation_callback: typing.Callable[..., typing.Any] | None = ...,
-    ) -> AsyncMemorizedFunc[P, T]: ...
+    ) -> AsyncMemorizedFunc[_P, _T]: ...
     @typing.overload
-    def __call__[**P, T](
+    def __call__(
         self,
-        func: typing.Callable[P, T],
+        func: typing.Callable[_P, _T],
         ignore: list[str] | None = ...,
         verbose: int | None = ...,
         mmap_mode: _MmepMode | bool = ...,
         cache_validation_callback: typing.Callable[..., typing.Any] | None = ...,
-    ) -> MemorizedFunc[P, T]: ...
+    ) -> MemorizedFunc[_P, _T]: ...
 
 def extract_first_line(func_code: str) -> tuple[str, int]: ...
 
 class JobLibCollisionWarning(UserWarning): ...
 
 def register_store_backend(
     backend_name: str, backend: type[StoreBackendBase]
 ) -> None: ...
 
-class MemorizedResult[T](Logger):
+class MemorizedResult(Logger, typing.Generic[_T]):
     store_backend: StoreBackendBase
     mmap_mode: _MmepMode
     metadata: dict[str, typing.Any]
     duration: float
     verbose: int
     timestamp: float
     def __init__(
@@ -83,105 +87,107 @@
     def func(self) -> str: ...
     @property
     def func_id(self) -> str: ...
     @property
     def args_id(self) -> str: ...
     @property
     def argument_hash(self) -> str: ...
-    def get(self) -> T: ...
+    def get(self) -> _T: ...
     def clear(self) -> None: ...
 
-class NotMemorizedResult[T]:
-    value: T
+class NotMemorizedResult(typing.Generic[_T]):
+    value: _T
     valid: bool
-    def __init__(self, value: T) -> None: ...
-    def get(self) -> T: ...
+    def __init__(self, value: _T) -> None: ...
+    def get(self) -> _T: ...
     def clear(self) -> None: ...
 
-class NotMemorizedFunc[**P, T]:
-    func: typing.Callable[P, T]
-    def __init__(self, func: typing.Callable[P, T]) -> None: ...
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T: ...
+class NotMemorizedFunc(typing.Generic[_P, _T]):
+    func: typing.Callable[_P, _T]
+    def __init__(self, func: typing.Callable[_P, _T]) -> None: ...
+    def __call__(self, *args: _P.args, **kwargs: _P.kwargs) -> _T: ...
     def call_and_shelve(
-        self, *args: P.args, **kwargs: P.kwargs
-    ) -> NotMemorizedResult[T]: ...
+        self, *args: _P.args, **kwargs: _P.kwargs
+    ) -> NotMemorizedResult[_T]: ...
     def clear(self, warn: bool = ...) -> None: ...
     def call(
-        self, *args: P.args, **kwargs: P.kwargs
-    ) -> tuple[T, dict[typing.Any, typing.Any]]: ...
+        self, *args: _P.args, **kwargs: _P.kwargs
+    ) -> tuple[_T, dict[typing.Any, typing.Any]]: ...
     def check_call_in_cache(self, *args: typing.Any, **kwargs: typing.Any) -> bool: ...
 
-class AsyncNotMemorizedFunc[**P, T](NotMemorizedFunc[P, _AnyAwaitable[T]]):
-    func: _AnyAwaitableCallable[P, T]
-    def __init__(self, func: _AnyAwaitableCallable[P, T]) -> None: ...
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> _AnyAwaitable[T]: ...
-    async def call_and_shelve(
-        self, *args: P.args, **kwargs: P.kwargs
-    ) -> NotMemorizedResult[T]: ...
-    def call(self) -> tuple[_AnyAwaitable[T], dict[typing.Any, typing.Any]]: ...
+class AsyncNotMemorizedFunc(
+    NotMemorizedFunc[_P, _AnyAwaitable[_T]], typing.Generic[_P, _T]
+):
+    func: _AnyAwaitableCallable[_P, _T]
+    def __init__(self, func: _AnyAwaitableCallable[_P, _T]) -> None: ...
+    def __call__(self, *args: _P.args, **kwargs: _P.kwargs) -> _AnyAwaitable[_T]: ...
+    async def call_and_shelve(  # type: ignore[override]
+        self, *args: _P.args, **kwargs: _P.kwargs
+    ) -> NotMemorizedResult[_T]: ...
+    def call(self) -> tuple[_AnyAwaitable[_T], dict[typing.Any, typing.Any]]: ...  # type: ignore[override]
 
-class MemorizedFunc[**P, T](Logger):
+class MemorizedFunc(Logger, typing.Generic[_P, _T]):
     mmap_mode: _MmepMode
     compress: bool | int
-    func: typing.Callable[P, T]
+    func: typing.Callable[_P, _T]
     cache_validation_callback: typing.Callable[..., typing.Any] | None
     func_id: str
     ignore: list[str]
     store_backend: StoreBackendBase
     timestamp: float
     __doc__: str
     def __init__(
         self,
-        func: typing.Callable[P, T],
+        func: typing.Callable[_P, _T],
         location: str,
         backend: str = ...,
         ignore: list[str] | None = ...,
         mmap_mode: _MmepMode | None = ...,
         compress: bool | int = ...,
         verbose: int = ...,
         timestamp: float | None = ...,
         cache_validation_callback: typing.Callable[..., typing.Any] | None = ...,
     ) -> None: ...
     @property
     def func_code_info(self) -> tuple[typing.Any, ...]: ...
     def call_and_shelve(
-        self, *args: P.args, **kwargs: P.kwargs
-    ) -> MemorizedResult[T] | NotMemorizedResult[T]: ...
+        self, *args: _P.args, **kwargs: _P.kwargs
+    ) -> MemorizedResult[_T] | NotMemorizedResult[_T]: ...
     def __call__(
-        self, *args: P.args, **kwargs: P.kwargs
-    ) -> MemorizedResult[T] | NotMemorizedResult[T]: ...
-    def check_call_in_cache(self, *args: P.args, **kwargs: P.kwargs) -> bool: ...
+        self, *args: _P.args, **kwargs: _P.kwargs
+    ) -> MemorizedResult[_T] | NotMemorizedResult[_T]: ...
+    def check_call_in_cache(self, *args: _P.args, **kwargs: _P.kwargs) -> bool: ...
     def clear(self, warn: bool = ...) -> None: ...
     def call(
-        self, *args: P.args, **kwargs: P.kwargs
-    ) -> tuple[MemorizedResult[T] | NotMemorizedResult[T], dict[str, typing.Any]]: ...
+        self, *args: _P.args, **kwargs: _P.kwargs
+    ) -> tuple[MemorizedResult[_T] | NotMemorizedResult[_T], dict[str, typing.Any]]: ...
 
-class AsyncMemorizedFunc[**P, T](MemorizedFunc[P, _AnyAwaitable[T]]):
-    func: _AnyAwaitableCallable[P, T]
+class AsyncMemorizedFunc(MemorizedFunc[_P, _AnyAwaitable[_T]], typing.Generic[_P, _T]):
+    func: _AnyAwaitableCallable[_P, _T]
     def __init__(
         self,
-        func: _AnyAwaitableCallable[P, T],
+        func: _AnyAwaitableCallable[_P, _T],
         location: str,
         backend: str = ...,
         ignore: list[str] | None = ...,
         mmap_mode: _MmepMode | None = ...,
         compress: bool | int = ...,
         verbose: int = ...,
         timestamp: float | None = ...,
         cache_validation_callback: typing.Callable[..., typing.Any] | None = ...,
     ) -> None: ...
-    async def __call__(
-        self, *args: P.args, **kwargs: P.kwargs
-    ) -> MemorizedResult[T] | NotMemorizedResult[T]: ...
-    async def call_and_shelve(
-        self, *args: P.args, **kwargs: P.kwargs
-    ) -> MemorizedResult[T] | NotMemorizedResult[T]: ...
-    async def call(
-        self, *args: P.args, **kwargs: P.kwargs
-    ) -> tuple[MemorizedResult[T] | NotMemorizedResult[T], dict[str, typing.Any]]: ...
+    async def __call__(  # type: ignore[override]
+        self, *args: _P.args, **kwargs: _P.kwargs
+    ) -> MemorizedResult[_T] | NotMemorizedResult[_T]: ...
+    async def call_and_shelve(  # type: ignore[override]
+        self, *args: _P.args, **kwargs: _P.kwargs
+    ) -> MemorizedResult[_T] | NotMemorizedResult[_T]: ...
+    async def call(  # type: ignore[override]
+        self, *args: _P.args, **kwargs: _P.kwargs
+    ) -> tuple[MemorizedResult[_T] | NotMemorizedResult[_T], dict[str, typing.Any]]: ...
 
 class Memory(Logger):
     mmap_mode: _MmepMode
     timestamp: float
     bytes_limit: int | str
     backend: str
     compress: bool | int
@@ -204,48 +210,50 @@
         func: None,
         ignore: list[str] | None = ...,
         verbose: int | None = ...,
         mmap_mode: _MmepMode | bool = ...,
         cache_validation_callback: typing.Callable[..., typing.Any] | None = ...,
     ) -> _CacheFunc: ...
     @typing.overload
-    def cache[**P, T](
+    def cache(
         self,
-        func: _AnyAwaitableCallable[P, T],
+        func: _AnyAwaitableCallable[_P, _T],
         ignore: list[str] | None = ...,
         verbose: int | None = ...,
         mmap_mode: _MmepMode | bool = ...,
         cache_validation_callback: typing.Callable[..., typing.Any] | None = ...,
-    ) -> AsyncMemorizedFunc[P, T]: ...
+    ) -> AsyncMemorizedFunc[_P, _T]: ...
     @typing.overload
-    def cache[**P, T](
+    def cache(
         self,
-        func: typing.Callable[P, T],
+        func: typing.Callable[_P, _T],
         ignore: list[str] | None = ...,
         verbose: int | None = ...,
         mmap_mode: _MmepMode | bool = ...,
         cache_validation_callback: typing.Callable[..., typing.Any] | None = ...,
-    ) -> MemorizedFunc[P, T]: ...
+    ) -> MemorizedFunc[_P, _T]: ...
     def clear(self, warn: bool = ...) -> None: ...
     def reduce_size(
         self,
         bytes_limit: int | str | None = ...,
         items_limit: int | None = ...,
         age_limit: timedelta | None = ...,
     ) -> None: ...
+    # awaitble -> awaitable
+    # non-awaitable -> non-awaitable
     @typing.overload
-    def eval[**P, T](
-        self, func: _AnyAwaitableCallable[P, T], *args: P.args, **kwargs: P.kwargs
+    def eval(
+        self, func: _AnyAwaitableCallable[_P, _T], *args: _P.args, **kwargs: _P.kwargs
     ) -> typing.Coroutine[
-        typing.Any, typing.Any, T | NotMemorizedResult[T] | MemorizedResult[T]
+        typing.Any, typing.Any, _T | NotMemorizedResult[_T] | MemorizedResult[_T]
     ]: ...
     @typing.overload
-    def eval[**P, T](
-        self, func: typing.Callable[P, T], *args: P.args, **kwargs: P.kwargs
-    ) -> T | NotMemorizedResult[T] | MemorizedResult[T]: ...
+    def eval(
+        self, func: typing.Callable[_P, _T], *args: _P.args, **kwargs: _P.kwargs
+    ) -> _T | NotMemorizedResult[_T] | MemorizedResult[_T]: ...
 
 def expires_after(
     days: int = ...,
     seconds: int = ...,
     microseconds: int = ...,
     milliseconds: int = ...,
     minutes: int = ...,
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/numpy_pickle.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/numpy_pickle.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     file_handle: typing.BinaryIO
     buffered: bool
     np: types.ModuleType
     def __init__(self, fp: typing.BinaryIO, protocol: int | None = ...) -> None: ...
     def save(self, obj: typing.Any) -> None: ...
 
 class NumpyUnpickler(Unpickler):
-    dispatch: typing.ClassVar[dict[type[typing.Any], _Dispatch[typing.Any]]]
+    # dispatch: typing.ClassVar[dict[type[typing.Any], _Dispatch[typing.Any]]]  # noqa: ERA001, E501
     mmap_mode: _MmapMode
     file_handle: typing.BinaryIO
     filename: str
     compat_mode: bool
     np: types.ModuleType
     def __init__(
         self,
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/numpy_pickle_compat.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/numpy_pickle_compat.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         filename: str,
         init_args: tuple[typing.Any, ...],
         state: tuple[typing.Any, ...],
     ) -> None: ...
     def read(self, unpickler: Unpickler) -> NDArray[typing.Any]: ...
 
 class ZipNumpyUnpickler(Unpickler):
-    dispatch: typing.ClassVar[dict[type[typing.Any], _Dispatch[typing.Any]]]
+    # dispatch: typing.ClassVar[dict[type[typing.Any], _Dispatch[typing.Any]]]  # noqa: ERA001, E501
     mmap_mode: _MmapMode
     file_handle: typing.BinaryIO
     np: types.ModuleType
     def __init__(
         self,
         filename: str,
         file_handle: typing.BinaryIO,
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/parallel.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/parallel.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -19,24 +19,28 @@
 from joblib._utils import _Sentinel
 from joblib._utils import eval_expr as eval_expr
 from joblib.disk import memstr_to_bytes as memstr_to_bytes
 from joblib.externals import loky as loky
 from joblib.logger import Logger as Logger
 from joblib.logger import short_format_time as short_format_time
 
-type _ReturnList = typing.Literal["list"]
-type _ReturnGererator = typing.Literal["generator"]
-type _ReturnGereratorUnordered = typing.Literal["generator_unordered"]
-type _ReturnUnknown = str
-type _ReturnAs = (
+_T = typing_extensions.TypeVar("_T")
+_P = typing_extensions.ParamSpec("_P")
+
+_ReturnList: typing_extensions.TypeAlias = typing.Literal["list"]
+_ReturnGererator: typing_extensions.TypeAlias = typing.Literal["generator"]
+_ReturnGereratorUnordered: typing_extensions.TypeAlias = typing.Literal[
+    "generator_unordered"
+]
+_ReturnUnknown: typing_extensions.TypeAlias = str
+_ReturnAs: typing_extensions.TypeAlias = (
     _ReturnList | _ReturnGererator | _ReturnGereratorUnordered | _ReturnUnknown
 )
 _R = typing_extensions.TypeVar(
     "_R",
-    infer_variance=True,
     default=typing.Literal["list"],
     bound="_ReturnAs",  # noqa: PYI020
 )
 
 IS_PYPY: bool
 BACKENDS: dict[str, type[ParallelBackendBase[typing.Any]]]
 DEFAULT_BACKEND: str
@@ -83,21 +87,21 @@
     def __init__(
         self,
         backend: ParallelBackendBase[_R],
         n_jobs: int = ...,
         inner_max_num_threads: int | None = ...,
         **backend_params: typing.Any,
     ) -> None: ...
-    def __enter__(self) -> tuple[ParallelBackendBase[_R], int]: ...
+    def __enter__(self) -> tuple[ParallelBackendBase[_R], int]: ...  # type: ignore[override]
 
 DEFAULT_MP_CONTEXT: BaseContext | None
 method: str | None
 
-type _BatchedCall[**P, T] = tuple[
-    typing.Callable[P, T], tuple[typing.Any, ...], dict[str, typing.Any]
+_BatchedCall: typing_extensions.TypeAlias = tuple[
+    typing.Callable[_P, _T], tuple[typing.Any, ...], dict[str, typing.Any]
 ]
 
 class BatchedCalls:
     items: list[_BatchedCall[..., typing.Any]]
     def __init__(
         self,
         iterator_slice: typing.Iterable[_BatchedCall[..., typing.Any]],
@@ -121,32 +125,32 @@
     def __len__(self) -> int: ...
 
 TASK_DONE: typing.Literal["Done"]
 TASK_ERROR: typing.Literal["Error"]
 TASK_PENDING: typing.Literal["Pending"]
 
 def cpu_count(only_physical_cores: bool = ...) -> int: ...
-def delayed[**P, T](
-    function: typing.Callable[P, T],
-) -> typing.Callable[P, _BatchedCall[P, T]]: ...
+def delayed(
+    function: typing.Callable[_P, _T],
+) -> typing.Callable[_P, _BatchedCall[_P, _T]]: ...
 
-class BatchCompletionCallBack[T]:
+class BatchCompletionCallBack(typing.Generic[_T]):
     dispatch_timestamp: float
     batch_size: int
     parallel: Parallel
     parallel_call_id: tuple[str, ...]
-    job: futures.Future[T] | AsyncResult[T] | None
+    job: futures.Future[_T] | AsyncResult[_T] | None
     status: str
     def __init__(
         self, dispatch_timestamp: float, batch_size: int, parallel: Parallel
     ) -> None: ...
-    def register_job(self, job: futures.Future[T] | AsyncResult[T]) -> None: ...
+    def register_job(self, job: futures.Future[_T] | AsyncResult[_T]) -> None: ...
     def get_result(self, timeout: float) -> typing.Any: ...
     def get_status(self, timeout: float) -> str: ...
-    def __call__(self, out: futures.Future[T] | AsyncResult[T]) -> None: ...
+    def __call__(self, out: futures.Future[_T] | AsyncResult[_T]) -> None: ...
 
 def register_parallel_backend(
     name: str, factory: type[ParallelBackendBase[typing.Any]], make_default: bool = ...
 ) -> None: ...
 def effective_n_jobs(n_jobs: int = ...) -> int: ...
 
 class Parallel(Logger, typing.Generic[_R]):
@@ -251,15 +255,15 @@
         temp_folder: str | None = ...,
         max_nbytes: int | str | None = ...,
         mmap_mode: _MmapMode | None = ...,
         prefer: _Prefer | None = ...,
         require: _Require | None = ...,
     ) -> Parallel[_ReturnUnknown]: ...
     @typing.overload
-    def __new__(
+    def __new__(  # type: ignore[misc]
         cls,
         n_jobs: int | None = ...,
         backend: str | ParallelBackendBase[typing.Any] | None = ...,
         return_as: _ReturnAs = ...,
         verbose: int | None = ...,
         timeout: float | None = ...,
         pre_dispatch: int | str = ...,
@@ -280,32 +284,32 @@
     ) -> None: ...
     def dispatch_next(self) -> None: ...
     def dispatch_one_batch(
         self, iterator: typing.Iterable[_BatchedCall[..., typing.Any]]
     ) -> bool: ...
     def print_progress(self) -> None: ...
     @typing.overload
-    def __call__[T](
-        self: Parallel[_ReturnList], iterable: typing.Iterable[_BatchedCall[..., T]]
-    ) -> list[T]: ...
+    def __call__(
+        self: Parallel[_ReturnList], iterable: typing.Iterable[_BatchedCall[..., _T]]
+    ) -> list[_T]: ...
     @typing.overload
-    def __call__[T](
+    def __call__(
         self: Parallel[_ReturnGererator],
-        iterable: typing.Iterable[_BatchedCall[..., T]],
-    ) -> typing.Generator[T, None, None]: ...
+        iterable: typing.Iterable[_BatchedCall[..., _T]],
+    ) -> typing.Generator[_T, None, None]: ...
     @typing.overload
-    def __call__[T](
+    def __call__(
         self: Parallel[_ReturnGereratorUnordered],
-        iterable: typing.Iterable[_BatchedCall[..., T]],
-    ) -> typing.Generator[T, None, None]: ...
+        iterable: typing.Iterable[_BatchedCall[..., _T]],
+    ) -> typing.Generator[_T, None, None]: ...
     @typing.overload
-    def __call__[T](
-        self: Parallel[_ReturnUnknown], iterable: typing.Iterable[_BatchedCall[..., T]]
-    ) -> list[T] | typing.Generator[T, None, None]: ...
-    @typing.overload
-    def __call__[T](
-        self: Parallel[typing.Any], iterable: typing.Iterable[_BatchedCall[..., T]]
-    ) -> list[T] | typing.Generator[T, None, None]: ...
-    @typing.overload
-    def __call__[T](
-        self, iterable: typing.Iterable[_BatchedCall[..., T]]
-    ) -> list[T] | typing.Generator[T, None, None]: ...
+    def __call__(
+        self: Parallel[_ReturnUnknown], iterable: typing.Iterable[_BatchedCall[..., _T]]
+    ) -> list[_T] | typing.Generator[_T, None, None]: ...
+    @typing.overload
+    def __call__(
+        self: Parallel[typing.Any], iterable: typing.Iterable[_BatchedCall[..., _T]]
+    ) -> list[_T] | typing.Generator[_T, None, None]: ...
+    @typing.overload
+    def __call__(
+        self, iterable: typing.Iterable[_BatchedCall[..., _T]]
+    ) -> list[_T] | typing.Generator[_T, None, None]: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/pool.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/pool.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -12,32 +12,34 @@
 from joblib._memmapping_reducer import _MmapMode
 from joblib._memmapping_reducer import (
     get_memmapping_reducers as get_memmapping_reducers,
 )
 from joblib._multiprocessing_helpers import assert_spawning as assert_spawning
 from joblib._multiprocessing_helpers import mp as mp
 
-type _Reducer[T] = typing.Callable[
-    typing_extensions.Concatenate[type[T], ...], typing.Any
+_T = typing_extensions.TypeVar("_T")
+
+_Reducer: typing_extensions.TypeAlias = typing.Callable[
+    typing_extensions.Concatenate[type[_T], ...], typing.Any
 ]
-type _Dispatch[T] = typing.Callable[[Unpickler, T], None]
+_Dispatch: typing_extensions.TypeAlias = typing.Callable[[Unpickler, _T], None]  # noqa: PYI047
 
 class CustomizablePickler(Pickler):
-    dispatch: dict[type[typing.Any], _Dispatch[typing.Any]]
+    # dispatch: dict[type[typing.Any], _Dispatch[typing.Any]]  # noqa: ERA001
     dispatch_table: dict[type[typing.Any], _Reducer[typing.Any]]
     def __init__(
         self,
         writer: SupportsWrite[bytes],
         reducers: dict[type[typing.Any], _Reducer[typing.Any]] | None = ...,
         protocol: int = ...,
     ) -> None: ...
-    def register[T](
+    def register(
         self,
-        type: type[T],  # noqa: A002
-        reduce_func: _Reducer[T],
+        type: type[_T],  # noqa: A002
+        reduce_func: _Reducer[_T],
     ) -> None: ...
 
 class CustomizablePicklingQueue:
     def __init__(
         self,
         context: BaseContext,
         reducers: dict[type[typing.Any], _Reducer[typing.Any]] | None = ...,
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/cloudpickle/__init__.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/cloudpickle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/cloudpickle/cloudpickle.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/cloudpickle/cloudpickle.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import weakref
 
 import typing_extensions
 from _typeshed import ReadableBuffer, SupportsWrite
 from joblib.pool import _Dispatch as _Dispatch
 from joblib.pool import _Reducer as _Reducer
 
+_T = typing_extensions.TypeVar("_T")
+
 _PICKLE_BY_VALUE_MODULES: set[str]
 _DYNAMIC_CLASS_TRACKER_BY_CLASS: weakref.WeakKeyDictionary[typing.Any, str]
 _DYNAMIC_CLASS_TRACKER_BY_ID: weakref.WeakValueDictionary[str, typing.Any]
 _DYNAMIC_CLASS_TRACKER_LOCK: threading.Lock
 
 DEFAULT_PROTOCOL: int
 PYPY: bool
@@ -31,15 +33,15 @@
 
 def is_tornado_coroutine(func: typing.Callable[..., typing.Any]) -> bool: ...
 def subimport(name: str) -> types.ModuleType: ...
 def dynamic_subimport(
     name: str,
     vars: typing.Mapping[str, typing.Any],  # noqa: A002
 ) -> types.ModuleType: ...
-def instance[T](cls: type[T]) -> T: ...
+def instance(cls: type[_T]) -> _T: ...
 
 # decorated by `instance`
 class _EmptyCellValueClass:
     @classmethod
     def __reduce__(cls) -> str: ...
 
 _empty_cell_value: _EmptyCellValueClass
@@ -47,18 +49,20 @@
 class _PickleBuffer:
     def __init__(self, buffer: ReadableBuffer) -> None: ...
     def raw(self) -> memoryview: ...
     def release(self) -> None: ...
     def __buffer__(self, flags: int, /) -> memoryview: ...
     def __release_buffer__(self, buffer: memoryview, /) -> None: ...
 
-type _BufferCallback = typing.Callable[[_PickleBuffer], typing.Any] | None
+_BufferCallback: typing_extensions.TypeAlias = (
+    typing.Callable[[_PickleBuffer], typing.Any] | None
+)
 
 class Pickler(pickle.Pickler):
-    dispatch_table: typing.ClassVar[dict[type[typing.Any], _Reducer[typing.Any]]]
+    dispatch_table: typing.ClassVar[dict[type[typing.Any], _Reducer[typing.Any]]]  # type: ignore[misc]
     def dump(self, obj: typing.Any) -> None: ...
     globals_ref: dict[int, dict[str, typing.Any]]
     proto: int
     def __init__(
         self,
         file: SupportsWrite[bytes],
         protocol: int | None = ...,
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/__init__.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/__init__.pyi`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/process_executor.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/process_executor.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import typing
 import weakref
 from concurrent import futures
 from concurrent.futures import Executor
 from concurrent.futures.process import BrokenProcessPool as _BPPException
 from multiprocessing.context import BaseContext
 
+import typing_extensions
 from joblib.externals.loky._base import Future as Future
 from joblib.externals.loky.backend import get_context as get_context
 from joblib.externals.loky.backend.context import cpu_count as cpu_count
 from joblib.externals.loky.backend.queues import Queue as Queue
 from joblib.externals.loky.backend.queues import SimpleQueue as SimpleQueue
 from joblib.externals.loky.backend.reduction import (
     get_loky_pickler_name as get_loky_pickler_name,
@@ -26,15 +27,18 @@
 
 MAX_DEPTH: int
 _CURRENT_DEPTH: int
 _MEMORY_LEAK_CHECK_DELAY: float
 _MAX_MEMORY_LEAK_SIZE: int
 _USE_PSUTIL: bool
 
-type _Lock = Lock | RLock
+_Lock: typing_extensions.TypeAlias = Lock | RLock
+_BaseExceptionT = typing.TypeVar("_BaseExceptionT", bound=BaseException)
+_T = typing_extensions.TypeVar("_T")
+_P = typing_extensions.ParamSpec("_P")
 
 class _ThreadWakeup:
     def __init__(self) -> None: ...
     def close(self) -> None: ...
     def wakeup(self) -> None: ...
     def clear(self) -> None: ...
 
@@ -57,83 +61,87 @@
 process_pool_executor_at_exit: typing.Callable[..., typing.Any] | None
 EXTRA_QUEUED_CALLS: int
 
 class _RemoteTraceback(Exception):  # noqa: N818
     tb: str
     def __init__(self, tb: typing.Any = ...) -> None: ...
 
-type _RebuildExc[T: BaseException] = typing.Callable[[T, str], T]
+_RebuildExc: typing_extensions.TypeAlias = typing.Callable[
+    [_BaseExceptionT, str], _BaseExceptionT
+]
 
-class _ExceptionWithTraceback[T: BaseException]:
-    exc: T
+class _ExceptionWithTraceback(typing.Generic[_BaseExceptionT]):
+    exc: _BaseExceptionT
     tb: str
-    def __init__(self, exc: T) -> None: ...
-    def __reduce__(self) -> tuple[_RebuildExc[T], tuple[T, str]]: ...
+    def __init__(self, exc: _BaseExceptionT) -> None: ...
+    def __reduce__(
+        self,
+    ) -> tuple[_RebuildExc[_BaseExceptionT], tuple[_BaseExceptionT, str]]: ...
 
-class _WorkItem[**P, T]:
-    future: futures.Future[T]
-    fn: typing.Callable[P, T]
+class _WorkItem(typing.Generic[_P, _T]):
+    future: futures.Future[_T]
+    fn: typing.Callable[_P, _T]
     args: tuple[typing.Any, ...]
     kwargs: dict[str, typing.Any]
     def __init__(
         self,
-        future: Future[T],
-        fn: typing.Callable[P, T],
+        future: Future[_T],
+        fn: typing.Callable[_P, _T],
         args: tuple[typing.Any, ...],
         kwargs: dict[str, typing.Any],
     ) -> None: ...
 
-class _ResultItem[T]:
+class _ResultItem(typing.Generic[_T]):
     work_id: int
     exception: BaseException | None
-    result: T | None
+    result: _T | None
     def __init__(
         self,
         work_id: int,
         exception: BaseException | None = ...,
-        result: T | None = ...,  # pyright: ignore[reportInvalidTypeVarUse]
+        result: _T | None = ...,  # pyright: ignore[reportInvalidTypeVarUse]
     ) -> None: ...
 
-class _CallItem[**P, T]:
+class _CallItem(typing.Generic[_P, _T]):
     work_id: int
-    fn: typing.Callable[P, T]
+    fn: typing.Callable[_P, _T]
     args: tuple[typing.Any, ...]
     kwargs: dict[str, typing.Any]
     loky_pickler: str
     def __init__(
         self,
         work_id: int,
-        fn: typing.Callable[P, T],
+        fn: typing.Callable[_P, _T],
         args: tuple[typing.Any, ...],
         kwargs: dict[str, typing.Any],
     ) -> None: ...
-    def __call__(self) -> T: ...
+    def __call__(self) -> _T: ...
 
-class _SafeQueue[T](Queue[T]):
+class _SafeQueue(Queue[_T], typing.Generic[_T]):
     thread_wakeup: _ThreadWakeup | None
-    pending_work_items: dict[int, _WorkItem[..., T]] | None
+    pending_work_items: dict[int, _WorkItem[..., _T]] | None
     running_work_items: list[int] | None
     def __init__(
         self,
         max_size: int = ...,
         ctx: BaseContext | None = ...,
-        pending_work_items: dict[int, _WorkItem[..., T]] | None = ...,  # pyright: ignore[reportInvalidTypeVarUse]
+        pending_work_items: dict[int, _WorkItem[..., _T]] | None = ...,  # pyright: ignore[reportInvalidTypeVarUse]
         running_work_items: list[int] | None = ...,
         thread_wakeup: _ThreadWakeup | None = ...,
         reducers: dict[type[typing.Any], _Reducer[typing.Any]] | None = ...,
     ) -> None: ...
 
 class _ExecutorManagerThread(threading.Thread):
     thread_wakeup: _ThreadWakeup | None
     shutdown_lock: threading.Lock
     executor_reference: weakref.ReferenceType[ProcessPoolExecutor]
     executor_flags: _ExecutorFlags
     processes: dict[int, _Process]
-    call_queue: _SafeQueue | None
-    result_queue: SimpleQueue | None
+    call_queue: _SafeQueue[_CallItem[..., typing.Any]] | None
+    result_queue: SimpleQueue[_ResultItem[typing.Any]] | None
     work_ids_queue: Queue[int]
     pending_work_items: dict[int, _WorkItem[..., typing.Any]]
     running_work_items: list[int]
     processes_management_lock: _Lock
     daemon: bool
     def __init__(self, executor: ProcessPoolExecutor) -> None: ...
     def run(self) -> None: ...
@@ -172,19 +180,19 @@
         result_reducers: dict[type[typing.Any], _Reducer[typing.Any]] | None = ...,
         timeout: float | None = ...,
         context: BaseContext | None = ...,
         initializer: typing.Callable[..., typing.Any] | None = ...,
         initargs: tuple[typing.Any, ...] = ...,
         env: dict[str, str] | None = ...,
     ) -> None: ...
-    def submit[**P, T](
-        self, fn: typing.Callable[P, T], *args: P.args, **kwargs: P.kwargs
-    ) -> futures.Future[T]: ...
-    def map[T](
+    def submit(
+        self, fn: typing.Callable[_P, _T], *args: _P.args, **kwargs: _P.kwargs
+    ) -> futures.Future[_T]: ...
+    def map(
         self,
-        fn: typing.Callable[..., T],
+        fn: typing.Callable[..., _T],
         *iterables: typing.Iterable[typing.Any],
         timeout: float | None = ...,
         chunksize: int = ...,
         **kwargs: typing.Any,
-    ) -> typing.Generator[T, typing.Any, None]: ...
+    ) -> typing.Generator[_T, typing.Any, None]: ...
     def shutdown(self, wait: bool = ..., kill_workers: bool = ...) -> None: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/reusable_executor.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/reusable_executor.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import threading
 import typing
 from concurrent import futures
 from multiprocessing.context import BaseContext
 
+import typing_extensions
 from _typeshed import Incomplete
 from joblib.externals.loky.process_executor import ProcessPoolExecutor
 
 __all__ = ["get_reusable_executor"]
 
-type _Context = str | BaseContext
+_T = typing_extensions.TypeVar("_T")
+_P = typing_extensions.ParamSpec("_P")
+
+_Context: typing_extensions.TypeAlias = str | BaseContext
 
 def get_reusable_executor(
     max_workers: int | None = ...,
     context: _Context | None = ...,
     timeout: float = ...,
     kill_workers: bool = ...,
     reuse: str = ...,
@@ -53,10 +57,10 @@
         | None = ...,
         result_reducers: dict[type[typing.Any], typing.Callable[..., typing.Any]]
         | None = ...,
         initializer: typing.Callable[..., typing.Any] | None = ...,
         initargs: tuple[typing.Any, ...] = ...,
         env: dict[str, str] | None = ...,
     ) -> _ReusablePoolExecutor: ...
-    def submit[**P, T](
-        self, fn: typing.Callable[P, T], *args: P.args, **kwargs: P.kwargs
-    ) -> futures.Future[T]: ...
+    def submit(
+        self, fn: typing.Callable[_P, _T], *args: _P.args, **kwargs: _P.kwargs
+    ) -> futures.Future[_T]: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/_posix_reduction.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/_posix_reduction.pyi`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/context.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/context.pyi`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/popen_loky_posix.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/popen_loky_posix.pyi`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/process.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/process.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         kwargs: typing.Mapping[str, typing.Any] = ...,
         daemon: bool | None = ...,
         init_main_module: bool = ...,
         env: dict[str, str] | None = ...,
     ) -> None: ...
 
 class LokyInitMainProcess(LokyProcess):
-    _start_method: typing.Literal["loky_init_main"]
+    _start_method: typing.Literal["loky_init_main"]  # type: ignore[assignment]
 
     def __init__(
         self,
         group: None = ...,
         target: typing.Callable[..., typing.Any] | None = ...,
         name: str | None = ...,
         args: typing.Iterable[typing.Any] = ...,
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/queues.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/queues.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import typing
 from multiprocessing.context import BaseContext
 from multiprocessing.queues import Queue as mp_Queue
 from multiprocessing.queues import SimpleQueue as mp_SimpleQueue
 from queue import Full
 
+import typing_extensions
 from joblib.pool import _Reducer
 
 __all__ = ["Queue", "SimpleQueue", "Full"]
 
-class Queue[T](mp_Queue[T]):
+_T = typing_extensions.TypeVar("_T")
+
+class Queue(mp_Queue[_T], typing.Generic[_T]):
     def __init__(
         self,
         maxsize: int = ...,
         reducers: dict[type[typing.Any], _Reducer[typing.Any]] | None = ...,
         ctx: BaseContext | None = ...,
     ) -> None: ...
 
-class SimpleQueue[T](mp_SimpleQueue[T]):
+class SimpleQueue(mp_SimpleQueue[_T], typing.Generic[_T]):
     def __init__(
         self,
         reducers: dict[type[typing.Any], _Reducer[typing.Any]] | None = ...,
         ctx: BaseContext | None = ...,
     ) -> None: ...
     def close(self) -> None: ...
-    def put(self, obj: T) -> None: ...
+    def put(self, obj: _T) -> None: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/reduction.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/reduction.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import typing
 from pickle import Pickler
 from pickle import loads as loads
 
+import typing_extensions
 from _typeshed import SupportsWrite
 from joblib.pool import _Reducer
 
 __all__ = ["dump", "dumps", "loads", "register", "set_loky_pickler"]
 
+_T = typing_extensions.TypeVar("_T")
+
 DEFAULT_ENV: str
 ENV_LOKY_PICKLER: str
 
-def register[T](type_: type[T], reduce_function: _Reducer[T]) -> None: ...
+def register(type_: type[_T], reduce_function: _Reducer[_T]) -> None: ...
 
 class _C:
     def f(self) -> None: ...
     @classmethod
     def h(cls) -> None: ...
 
 def set_loky_pickler(loky_pickler: str | None = ...) -> None: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/resource_tracker.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/resource_tracker.pyi`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/src/joblib-stubs/externals/loky/backend/synchronize.pyi` & `joblib_stubs-1.4.2.2.20240515/src/joblib-stubs/externals/loky/backend/synchronize.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import typing
 
 import typing_extensions
 from _typeshed import Incomplete
 
 __all__ = ["Lock", "RLock", "Semaphore", "BoundedSemaphore", "Condition", "Event"]
 
+_T = typing_extensions.TypeVar("_T")
+
 class SemLock:
     name: str | None
     def __init__(
         self, kind: Incomplete, value: int, maxvalue: Incomplete, name: str | None = ...
     ) -> None: ...
     def __enter__(self) -> Incomplete: ...
     def __exit__(self, *args: object) -> typing.Any: ...
@@ -29,17 +31,17 @@
 class Condition:
     def __init__(self, lock: Lock | RLock | None = ...) -> None: ...
     def __enter__(self) -> typing_extensions.Self: ...
     def __exit__(self, *args: object) -> typing.Any: ...
     def wait(self, timeout: float | None = ...) -> Incomplete: ...
     def notify(self) -> None: ...
     def notify_all(self) -> None: ...
-    def wait_for[T](
-        self, predicate: typing.Callable[[], T], timeout: float | None = ...
-    ) -> T: ...
+    def wait_for(
+        self, predicate: typing.Callable[[], _T], timeout: float | None = ...
+    ) -> _T: ...
 
 class Event:
     def __init__(self) -> None: ...
     def is_set(self) -> bool: ...
     def set(self) -> None: ...
     def clear(self) -> None: ...
     def wait(self, timeout: float | None = ...) -> bool: ...
```

### Comparing `joblib_stubs-1.4.2.1.20240513/.gitignore` & `joblib_stubs-1.4.2.2.20240515/.gitignore`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/LICENSE` & `joblib_stubs-1.4.2.2.20240515/LICENSE`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/README.md` & `joblib_stubs-1.4.2.2.20240515/README.md`

 * *Files identical despite different names*

### Comparing `joblib_stubs-1.4.2.1.20240513/pyproject.toml` & `joblib_stubs-1.4.2.2.20240515/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "joblib-stubs"
-version = "1.4.2.1.20240513"
+version = "1.4.2.2.20240515"
 description = "joblib stubs"
 authors = [{ name = "phi", email = "phi.friday@gmail.com" }]
 dependencies = [
     "typing-extensions>=4.4.0",
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
@@ -26,20 +26,27 @@
 [tool.rye]
 managed = true
 dev-dependencies = [
     "joblib>=1.4.2",
     "numpy>=1.24.4",
     "dask>=2023.5.0",
     "distributed>=2023.5.0",
+    "mypy>=1.10.0",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/joblib-stubs"]
 
 [tool.pyright]
 pythonVersion = '3.8'
 pythonPlatform = 'Linux'
 diagnostic = 'basic'
 stubPath = "./typings"
+
+[tool.mypy]
+python_version = "3.8"
+strict = true
+disable_error_code = "import-untyped,overload-overlap,override"
+disallow_subclassing_any = false
```

### Comparing `joblib_stubs-1.4.2.1.20240513/PKG-INFO` & `joblib_stubs-1.4.2.2.20240515/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: joblib-stubs
-Version: 1.4.2.1.20240513
+Version: 1.4.2.2.20240515
 Summary: joblib stubs
 Project-URL: Repository, https://github.com/phi-friday/joblib-stubs
 Author-email: phi <phi.friday@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Choi Min-yeong
```

