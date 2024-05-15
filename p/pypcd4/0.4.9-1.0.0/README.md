# Comparing `tmp/pypcd4-0.4.9.tar.gz` & `tmp/pypcd4-1.0.0.tar.gz`

## Comparing `pypcd4-0.4.9.tar` & `pypcd4-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,31 @@
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 pypcd4-0.4.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pypcd4-0.4.9/.python-version
--rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 pypcd4-0.4.9/COPYRIGHT.txt
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 pypcd4-0.4.9/requirements-dev.lock
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pypcd4-0.4.9/requirements.lock
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypcd4-0.4.9/src/pypcd4/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pypcd4-0.4.9/src/pypcd4/_version.py
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 pypcd4-0.4.9/src/pypcd4/pointcloud2.py
--rw-r--r--   0        0        0    26040 2020-02-02 00:00:00.000000 pypcd4-0.4.9/src/pypcd4/pypcd4.py
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/conftest.py
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/pcd/ascii.pcd
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/pcd/ascii_with_empty_points.pcd
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/pcd/ascii_with_underscore.pcd
--rw-r--r--   0        0        0     7504 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/pcd/binary.pcd
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/pcd/binary_compressed.pcd
--rw-r--r--   0        0        0    25133 2020-02-02 00:00:00.000000 pypcd4-0.4.9/tests/test/test_pypcd4.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pypcd4-0.4.9/.gitignore
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pypcd4-0.4.9/LICENSE.txt
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 pypcd4-0.4.9/README.md
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pypcd4-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     6959 2020-02-02 00:00:00.000000 pypcd4-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 pypcd4-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pypcd4-1.0.0/.python-version
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pypcd4-1.0.0/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 pypcd4-1.0.0/COPYRIGHT.txt
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 pypcd4-1.0.0/requirements-dev.lock
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pypcd4-1.0.0/requirements.lock
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 pypcd4-1.0.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypcd4-1.0.0/.github/workflows/deploy-pypi.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pypcd4-1.0.0/.github/workflows/deploy-testpypi.yaml
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pypcd4-1.0.0/.github/workflows/release-drafter.yaml
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pypcd4-1.0.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 pypcd4-1.0.0/.github/workflows/update-contributors.yaml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypcd4-1.0.0/src/pypcd4/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pypcd4-1.0.0/src/pypcd4/_version.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 pypcd4-1.0.0/src/pypcd4/pointcloud2.py
+-rw-r--r--   0        0        0    33410 2020-02-02 00:00:00.000000 pypcd4-1.0.0/src/pypcd4/pypcd4.py
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 pypcd4-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 pypcd4-1.0.0/tests/pcd/ascii.pcd
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pypcd4-1.0.0/tests/pcd/ascii_multi_count.pcd
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 pypcd4-1.0.0/tests/pcd/ascii_organized.pcd
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 pypcd4-1.0.0/tests/pcd/ascii_with_empty_points.pcd
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 pypcd4-1.0.0/tests/pcd/ascii_with_underscore.pcd
+-rw-r--r--   0        0        0     7504 2020-02-02 00:00:00.000000 pypcd4-1.0.0/tests/pcd/binary.pcd
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pypcd4-1.0.0/tests/pcd/binary_compressed.pcd
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pypcd4-1.0.0/tests/pcd/binary_compressed_organized.pcd
+-rw-r--r--   0        0        0    27777 2020-02-02 00:00:00.000000 pypcd4-1.0.0/tests/test/test_pypcd4.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pypcd4-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pypcd4-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 pypcd4-1.0.0/README.md
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 pypcd4-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9594 2020-02-02 00:00:00.000000 pypcd4-1.0.0/PKG-INFO
```

### Comparing `pypcd4-0.4.9/COPYRIGHT.txt` & `pypcd4-1.0.0/COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.9/requirements-dev.lock` & `pypcd4-1.0.0/requirements-dev.lock`

 * *Files 2% similar despite different names*

```diff
@@ -21,40 +21,40 @@
 coverage==7.3.2
     # via pytest-cov
 distlib==0.3.8
     # via virtualenv
 filelock==3.13.1
     # via tox
     # via virtualenv
-identify==2.5.33
+identify==2.5.36
     # via pre-commit
 iniconfig==2.0.0
     # via pytest
 mypy==1.7.1
 mypy-extensions==1.0.0
     # via mypy
 nodeenv==1.8.0
     # via pre-commit
-numpy==1.26.2
+numpy==1.24.4
     # via pypcd4
 packaging==23.2
     # via pyproject-api
     # via pytest
     # via setuptools-scm
     # via tox
 platformdirs==4.1.0
     # via tox
     # via virtualenv
 pluggy==1.3.0
     # via pytest
     # via tox
-pre-commit==3.6.0
-pydantic==2.5.2
+pre-commit==3.7.0
+pydantic==2.6.4
     # via pypcd4
-pydantic-core==2.14.5
+pydantic-core==2.16.3
     # via pydantic
 pyproject-api==1.6.1
     # via tox
 pytest==7.4.3
     # via pytest-cov
 pytest-cov==4.1.0
 python-lzf==0.2.4
```

### Comparing `pypcd4-0.4.9/src/pypcd4/pypcd4.py` & `pypcd4-1.0.0/src/pypcd4/pypcd4.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,30 @@
 
 import random
 import re
 import string
 import struct
 from enum import Enum
 from pathlib import Path
-from typing import BinaryIO, List, Literal, Optional, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, BinaryIO, List, Literal, Optional, Sequence, Tuple, Union
 
 import lzf
 import numpy as np
 import numpy.typing as npt
 from pydantic import BaseModel, NonNegativeInt, PositiveInt
 
-from .pointcloud2 import PFTYPE_TO_NPTYPE, PointCloud2, pointcloud2_to_array
+from .pointcloud2 import (
+    NPTYPE_TO_PFTYPE,
+    build_dtype_from_msg,
+    sensor_msgs__msg__PointCloud2,
+)
+
+if TYPE_CHECKING:
+    from sensor_msgs.msg import PointCloud2
+    from std_msgs.msg import Header
 
 PathLike = Union[str, Path]
 
 MetaDataVersion = Literal[".7", "0.7"]
 MetaDataViewPoint = Tuple[float, float, float, float, float, float, float]
 
 NUMPY_TYPE_TO_PCD_TYPE: dict[
@@ -153,15 +161,15 @@
         for i, field in enumerate(self.fields):
             np_type: npt.DTypeLike = np.dtype(PCD_TYPE_TO_NUMPY_TYPE[(self.type[i], self.size[i])])
 
             if (count := self.count[i]) == 1:
                 field_names.append(field)
                 np_types.append(np_type)
             else:
-                field_names.extend([f"{field}_{i:04d}" for i in range(count)])
+                field_names.extend([f"{field}__{i:04d}" for i in range(count)])
                 np_types.extend([np_type] * count)
 
         return np.dtype([x for x in zip(field_names, np_types)])
 
 
 def _parse_pc_data(fp: BinaryIO, metadata: MetaData) -> npt.NDArray:
     dtype = metadata.build_dtype()
@@ -179,18 +187,18 @@
             if (actual_size := len(buffer)) != uncompressed_size:
                 raise RuntimeError(
                     f"Failed to decompress data. "
                     f"Expected decompressed file size is {uncompressed_size}, but got {actual_size}"
                 )
 
             offset = 0
-            pc_data = np.zeros(metadata.width, dtype=dtype)
+            pc_data = np.zeros(metadata.points, dtype=dtype)
             for name in dtype.names:  # type: ignore
                 dt: np.dtype = dtype[name]
-                bytes = dt.itemsize * metadata.width
+                bytes = dt.itemsize * metadata.points
                 pc_data[name] = np.frombuffer(buffer[offset : (offset + bytes)], dtype=dt)
                 offset += bytes
     else:
         pc_data = np.empty((0, len(metadata.fields)), dtype)
 
     return pc_data
 
@@ -235,15 +243,19 @@
         Raises:
             FileNotFoundError: Raise if `path` does not exist.
 
         Returns:
             PointCloud: PointCloud object
 
         >>> PointCloud.from_path("test.pcd")
-        <pypcd4.PointCloud object at 0x7f7c9a3d8b00>
+        PointCloud(
+            fields=('x', 'y', 'z') size=(4, 4, 4) type=('F', 'F', 'F') count=(1, 1, 1) points=10000
+            width=10000 height=1 version='0.7' viewpoint=(0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0)
+            data=<Encoding.BINARY_COMPRESSED: 'binary_compressed'>
+        )
         """
 
         with open(path, mode="rb") as fp:
             return PointCloud.from_fileobj(fp)
 
     @staticmethod
     def from_points(
@@ -269,25 +281,33 @@
             PointCloud: PointCloud object
 
         >>> PointCloud.from_points(
                 np.array([[1, 2, 3], [4, 5, 6]]),
                 ("x", "y", "z"),
                 (np.float32, np.float32, np.float32)
             )
-        <pypcd4.PointCloud object at 0x7f7c9a3d8b00>
+        PointCloud(
+            fields=('x', 'y', 'z') size=(4, 4, 4) type=('F', 'F', 'F') count=(1, 1, 1) points=2
+            width=2 height=1 version='0.7' viewpoint=(0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0)
+            data=<Encoding.BINARY_COMPRESSED: 'binary_compressed'>
+        )
 
         >>> PointCloud.from_points(
                 [
                     np.array([1, 2, 3]),
                     np.array([4, 5, 6])
                 ],
                 ("x", "y", "z"),
                 (np.float32, np.float32, np.float32)
             )
-        <pypcd4.PointCloud object at 0x7f7c9a3d8b00>
+        PointCloud(
+            fields=('x', 'y', 'z') size=(4, 4, 4) type=('F', 'F', 'F') count=(1, 1, 1) points=2
+            width=2 height=1 version='0.7' viewpoint=(0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0)
+            data=<Encoding.BINARY_COMPRESSED: 'binary_compressed'>
+        )
         """
 
         if not isinstance(points, (np.ndarray, list, tuple)):
             raise TypeError(
                 "`points` must be a `np.ndarray`, `List[np.ndarray]` or `Tuple[np.ndarray]` type, "
                 f"but got `{type(points).__name__}` type"
             )
@@ -535,20 +555,101 @@
             np.uint16,
             np.uint32,
         )
 
         return PointCloud.from_points(points, fields, types)
 
     @staticmethod
-    def from_msg(msg: PointCloud2) -> PointCloud:
-        points = pointcloud2_to_array(msg)
-        fields = [f.name for f in msg.fields]
-        types: list[npt.DTypeLike] = [PFTYPE_TO_NPTYPE[f.datatype] for f in msg.fields]
+    def from_msg(msg: sensor_msgs__msg__PointCloud2) -> PointCloud:
+        """Create a PointCloud from a ROS/ROS 2 sensor_msgs.msg.PointCloud2 message
 
-        return PointCloud.from_points(points, fields, types)
+        Args:
+            msg: The ROS/ROS 2 sensor_msgs/PointCloud2 message
+
+        Returns:
+            The PointCloud
+        """
+
+        pc_data = np.frombuffer(msg.data, build_dtype_from_msg(msg))
+        metadata = MetaData.model_validate(
+            {
+                "fields": pc_data.dtype.names,
+                "size": [
+                    NUMPY_TYPE_TO_PCD_TYPE[pc_data[name].dtype][1]
+                    for name in pc_data.dtype.names  # type: ignore[union-attr]
+                ],
+                "type": [
+                    NUMPY_TYPE_TO_PCD_TYPE[pc_data[name].dtype][0]
+                    for name in pc_data.dtype.names  # type: ignore[union-attr]
+                ],
+                "count": [1] * len(pc_data.dtype.names),  # type: ignore[arg-type]
+                "points": len(pc_data),
+                "width": msg.width,
+                "height": msg.height,
+                "version": "0.7",
+                "viewpoint": (0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0),
+                "data": Encoding.BINARY,
+            }
+        )
+
+        return PointCloud(metadata, pc_data)
+
+    def to_msg(self, header: Optional["Header"] = None) -> "PointCloud2":
+        """Create a ROS/ROS 2 sensor_msgs.msg.PointCloud2 message from the PointCloud
+
+        Args:
+            header: The header to use for the message.
+                    If None, a default header will be used. Default: None.
+
+        Returns:
+            The ROS/ROS 2 sensor_msgs/PointCloud2 message
+        """
+
+        try:
+            from sensor_msgs.msg import PointCloud2, PointField
+            from std_msgs.msg import Header
+        except ImportError:
+            raise ImportError(
+                "The PointCloud.to_msg() method requires an additional ROS/ROS 2 sensor_msg module."
+                " Please install it according to the official installation guide."
+            ) from None
+
+        fields = []
+        itemsize = 0
+        row_step = 0
+        for i, (field, type_, count) in enumerate(zip(self.fields, self.types, self.counts)):
+            type_ = np.dtype(type_)
+
+            itemsize += type_.itemsize
+            row_step += type_.itemsize * self.points
+
+            fields.append(
+                PointField(
+                    name=field,
+                    offset=i * type_.itemsize,
+                    datatype=NPTYPE_TO_PFTYPE[type_],
+                    count=count,
+                )
+            )
+
+        data = self.pc_data.tobytes()
+
+        msg = PointCloud2(
+            header=Header() if header is None else header,
+            height=1,
+            width=self.points,
+            is_dense=False,
+            is_bigendian=False,
+            fields=fields,
+            point_step=itemsize,
+            row_step=len(data),
+            data=data,
+        )
+
+        return msg
 
     @staticmethod
     def encode_rgb(rgb: npt.NDArray | list[npt.NDArray]) -> npt.NDArray:
         """
         Encode Nx3 uint8 array with RGB values to
         Nx1 float32 array with bit-packed RGB
         """
@@ -588,47 +689,97 @@
     def fields(self) -> Tuple[str, ...]:
         """
         Returns fields of the point cloud
 
         Returns:
             Tuple[str, ...]: Tuple of field names for each field
 
-        >>> pc.fields
+        Note:
+            If the field count is not 1, the field names will be suffixed with __0000, __0001, etc.
+            If you don't want this behavior, use the `pc.metadata.fields` instead.
+
+        >>> pc1.metadata.count
+        (1, 1, 1)
+
+        >>> pc1.fields
+        ("x", "y", "z")
+
+        >>> pc2.metadata.count
+        (1, 1, 2)
+
+        >>> pc2.fields
+        ("x", "y", "z__0000", "z__0001")
+
+        >>> pc2.metadata.fields
         ("x", "y", "z")
         """
 
-        return self.metadata.fields
+        fields = []
+        for field, count in zip(self.metadata.fields, self.metadata.count):
+            if count == 1:
+                fields.append(field)
+            else:
+                fields.extend(f"{field}__{c:04d}" for c in range(count))
+
+        return tuple(fields)
 
     @property
     def types(self) -> Tuple[npt.DTypeLike, ...]:
         """Returns types of the point cloud
 
         Returns:
             Tuple[npt.DTypeLike, ...]: Tuple of numpy types for each field
 
-        >>> pc.types
-        (np.float32, np.float32, np.float32)
+        Note:
+            If the field count is not 1, the type will be repeated for the number of fields
+
+        >>> pc1.metadata.count
+        (1, 1, 1)
+
+        >>> pc1.types
+        (np.float32, np.int32, np.float32)
+
+        >>> pc2.metadata.count
+        (1, 2, 1)
+
+        >>> pc2.types
+        (np.float32, np.int32, np.int32, np.float32)
         """
 
-        return tuple(
-            PCD_TYPE_TO_NUMPY_TYPE[ts] for ts in zip(self.metadata.type, self.metadata.size)
-        )
+        types = []
+        for ts, count in zip(zip(self.metadata.type, self.metadata.size), self.metadata.count):
+            if count == 1:
+                types.append(PCD_TYPE_TO_NUMPY_TYPE[ts])
+            else:
+                types.extend(PCD_TYPE_TO_NUMPY_TYPE[ts] for _ in range(count))
+
+        return tuple(types)
 
     @property
-    def count(self) -> Tuple[PositiveInt, ...]:
+    def counts(self) -> Tuple[PositiveInt, ...]:
         """Returns number of elements in each field
 
         Returns:
             Tuple[PositiveInt, ...]: Tuple of number of elements in each field
 
-        >>> pc.counts
+        Note:
+            If the field count is not 1, the count will be repeated for the number of its counts
+            If you don't want this behavior, use the `pc.metadata.count` instead.
+
+        >>> pc1.metadata.count
         (1, 1, 1)
+
+        >>> pc2.metadata.count
+        (1, 2, 1)
+
+        >>> pc2.counts
+        (1, 1, 1, 1)
         """
 
-        return self.metadata.count
+        return (1,) * sum(self.metadata.count)
 
     @property
     def points(self) -> int:
         """Returns number of points in the point cloud
 
         Returns:
             int: The number of points
@@ -680,71 +831,14 @@
         if self.metadata.points == 0:
             return np.empty((0, len(fields)))
 
         _stack = tuple(self.pc_data[field] for field in fields)
 
         return np.vstack(_stack).T
 
-    def concatenate(self, other: PointCloud) -> PointCloud:
-        """
-        Concatenates two point clouds together
-        """
-
-        return self.__add__(other)
-
-    def __add__(self, other: PointCloud) -> PointCloud:
-        """
-        Concatenates two point clouds together
-        """
-
-        if self.fields != other.fields:
-            raise ValueError(
-                "Can't concatenate point clouds with different fields. "
-                f"({self.fields} vs. {other.fields})"
-            )
-        if self.types != other.types:
-            raise ValueError(
-                "Can't concatenate point clouds with different types. "
-                f"({self.types} vs. {other.types})"
-            )
-
-        concatenated_pc = PointCloud.from_points(
-            np.vstack((self.numpy(), other.numpy())), self.fields, self.types
-        )
-
-        return concatenated_pc
-
-    def __getitem__(self, mask: npt.NDArray[np.bool_]) -> PointCloud:
-        """Returns a point cloud with only the points that match the mask
-
-        >>> np.random.seed(42)
-        >>> pc = PointCloud.from_xyz_points(np.random.rand(100, 3))
-        >>> pc.points
-        10
-        >>> mask = (pc.pc_data["x"] > 0.5) & (pc.pc_data["y"] < 0.5)
-        >>> pc[mask].points
-        3
-        >>> pc[mask].numpy()
-        [[0.5986585  0.15601864 0.15599452]
-        [0.7080726  0.02058449 0.96990985]
-        [0.83244264 0.21233912 0.18182497]]
-        """
-
-        mask = mask.squeeze()
-
-        if mask.ndim != 1:
-            raise ValueError(f"mask array must be 1-dimensional but got {mask.ndim}")
-
-        points_list = [
-            self.pc_data[field][mask]
-            for field in self.pc_data.dtype.names  # type: ignore
-        ]
-
-        return PointCloud.from_points(points_list, self.fields, self.types)
-
     def _save_as_ascii(self, fp: BinaryIO) -> None:
         """Saves point cloud to a file as a ascii
 
         Args:
             fp (BinaryIO): io buffer.
         """
 
@@ -816,7 +910,116 @@
             elif encoding == Encoding.BINARY:
                 self._save_as_binary(fp)
             else:
                 self._save_as_binary_compressed(fp)
         finally:
             if is_open:
                 fp.close()
+
+    def __add__(self, other: PointCloud) -> PointCloud:
+        """Concatenates two point clouds together
+
+        Args:
+            other (PointCloud): Point cloud to concatenate with
+
+        Returns:
+            PointCloud: Concatenated point cloud
+
+        >>> pc1 = PointCloud.from_xyz_points(np.random.rand(10000, 3))
+        >>> pc2 = PointCloud.from_xyz_points(np.random.rand(10000, 3))
+
+        >>> pc1 + pc2
+        PointCloud(
+            fields=('x', 'y', 'z') size=(4, 4, 4) type=('F', 'F', 'F') count=(1, 1, 1) points=20000
+            width=20000 height=1 version='0.7' viewpoint=(0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0)
+            data=<Encoding.BINARY_COMPRESSED: 'binary_compressed'>
+        )
+        """
+
+        if self.fields != other.fields:
+            raise ValueError(
+                "Can't concatenate point clouds with different fields. "
+                f"({self.fields} vs. {other.fields})"
+            )
+        if self.types != other.types:
+            raise ValueError(
+                "Can't concatenate point clouds with different types. "
+                f"({self.types} vs. {other.types})"
+            )
+
+        concatenated_pc = PointCloud.from_points(
+            np.vstack((self.numpy(), other.numpy())), self.fields, self.types
+        )
+
+        return concatenated_pc
+
+    def __getitem__(
+        self, subscript: Union[slice, str, list[str], tuple[str, ...], npt.NDArray[np.bool_]]
+    ) -> PointCloud:
+        """Returns a point cloud with only the points that match the subscript
+
+        Args:
+            subscript (Union[slice, npt.NDArray[np.bool_]]): Subscript to match.
+
+        Returns:
+            PointCloud: Point cloud with only the points that match the subscript.
+
+        >>> pc = PointCloud.from_xyz_points(np.random.rand(10000, 3))
+
+        >>> pc[3:8]
+        PointCloud(
+            fields=('x', 'y', 'z') size=(4, 4, 4) type=('F', 'F', 'F') count=(1, 1, 1) points=5
+            width=5 height=1 version='0.7' viewpoint=(0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0)
+            data=<Encoding.BINARY_COMPRESSED: 'binary_compressed'>
+        )
+
+        >>> mask = (pc.pc_data["x"] > 0.5) & (pc.pc_data["y"] < 0.5)
+        >>> pc[mask]
+        PointCloud(
+            fields=('x', 'y', 'z') size=(4, 4, 4) type=('F', 'F', 'F') count=(1, 1, 1) points=2593
+            width=2593 height=1 version='0.7' viewpoint=(0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0)
+            data=<Encoding.BINARY_COMPRESSED: 'binary_compressed'>
+        )
+
+        >>> pc[("x", "y")]
+        PointCloud(
+            fields=('x', 'y') size=(4, 4) type=('F', 'F') count=(1, 1) points=10000
+            width=10000 height=1 version='0.7' viewpoint=(0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0)
+            data=<Encoding.BINARY_COMPRESSED: 'binary_compressed'>
+        )
+        """
+
+        points_list: list[npt.NDArray]
+        fields = self.fields
+        types = self.types
+        if isinstance(subscript, slice):
+            points_list = tuple(
+                self.pc_data[field][subscript]
+                for field in self.pc_data.dtype.names  # type: ignore[assignment,union-attr]
+            )
+        elif isinstance(subscript, np.ndarray):
+            mask = subscript.squeeze()
+            if mask.ndim != 1:
+                raise ValueError(f"Mask array must be 1-dimensional but got {mask.ndim}")
+
+            points_list = tuple(
+                self.pc_data[field][mask]
+                for field in self.pc_data.dtype.names  # type: ignore[assignment,union-attr]
+            )
+        elif isinstance(subscript, str) or all(isinstance(s, str) for s in subscript):
+            if isinstance(subscript, str):
+                subscript = (subscript,)
+
+            if not np.isin(subscript, self.fields).all():
+                raise ValueError(f"Invalid field name(s): {subscript}")
+
+            points_list = [self.pc_data[field] for field in subscript]
+            fields = tuple(subscript)
+            types = tuple(self.pc_data[field].dtype for field in subscript)
+
+        return PointCloud.from_points(points_list, fields, types)
+
+    def __str__(self) -> str:
+        return f"PointCloud({self.metadata})"
+
+    def __len__(self) -> int:
+        return self.points
```

### Comparing `pypcd4-0.4.9/tests/conftest.py` & `pypcd4-1.0.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# ruff: noqa: ANN001, ANN201
+
 from pathlib import Path
 
 import pytest
 
 
 @pytest.fixture
 def pcd_header():
@@ -289,14 +291,27 @@
 
 @pytest.fixture
 def xyzrgb_ascii_with_empty_points_path():
     return f"{Path(__file__).resolve().parent}/pcd/ascii_with_empty_points.pcd"
 
 
 @pytest.fixture
+def xyzintensity_ascii_organized_path():
+    return f"{Path(__file__).resolve().parent}/pcd/ascii_organized.pcd"
+
+
+@pytest.fixture
+def xyzintensity_ascii_multi_count_path():
+    return f"{Path(__file__).resolve().parent}/pcd/ascii_multi_count.pcd"
+
+@pytest.fixture
 def xyzrgb_binary_path():
     return f"{Path(__file__).resolve().parent}/pcd/binary.pcd"
 
 
 @pytest.fixture
 def xyzrgb_binary_compressed_path():
     return f"{Path(__file__).resolve().parent}/pcd/binary_compressed.pcd"
+
+@pytest.fixture
+def xyzintensity_binary_compressed_organized_path():
+    return f"{Path(__file__).resolve().parent}/pcd/binary_compressed_organized.pcd"
```

### Comparing `pypcd4-0.4.9/tests/pcd/ascii.pcd` & `pypcd4-1.0.0/tests/pcd/ascii.pcd`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.9/tests/pcd/ascii_with_underscore.pcd` & `pypcd4-1.0.0/tests/pcd/ascii_with_underscore.pcd`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.9/tests/pcd/binary.pcd` & `pypcd4-1.0.0/tests/pcd/binary.pcd`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.9/tests/pcd/binary_compressed.pcd` & `pypcd4-1.0.0/tests/pcd/binary_compressed.pcd`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.9/tests/test/test_pypcd4.py` & `pypcd4-1.0.0/tests/test/test_pypcd4.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# ruff: noqa: ANN001, ANN201
+
 from io import BytesIO
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import numpy as np
 import pytest
 from pydantic import ValidationError
@@ -177,18 +179,18 @@
 
 def test_build_dtype_with_multi_count_fields(pcd_header_with_multi_count_fields):
     metadata = MetaData.parse_header(pcd_header_with_multi_count_fields)
 
     assert metadata.build_dtype() == [
         ("x", "<f4"),
         ("y", "<f4"),
-        ("z_0000", "<f4"),
-        ("z_0001", "<f4"),
-        ("z_0002", "<f4"),
-        ("z_0003", "<f4"),
+        ("z__0000", "<f4"),
+        ("z__0001", "<f4"),
+        ("z__0002", "<f4"),
+        ("z__0003", "<f4"),
     ]
 
 
 def test_parse_pcd_header_with_invalid_version(pcd_header_with_invalid_version):
     with pytest.raises(ValidationError):
         MetaData.parse_header(pcd_header_with_invalid_version)
 
@@ -238,14 +240,22 @@
     pc = PointCloud.from_path(xyzrgb_ascii_with_empty_points_path)
 
     assert pc.metadata.data == "ascii"
     assert pc.pc_data.dtype.names == pc.metadata.fields
     assert len(pc.pc_data) == pc.metadata.points
 
 
+def test_load_xyzintensity_ascii_organized_pcd(xyzintensity_ascii_organized_path):
+    pc = PointCloud.from_path(xyzintensity_ascii_organized_path)
+
+    assert pc.metadata.data == "ascii"
+    assert pc.pc_data.dtype.names == pc.metadata.fields
+    assert len(pc.pc_data) == pc.metadata.points
+
+
 def test_load_binary_pcd(xyzrgb_binary_path):
     pc = PointCloud.from_path(xyzrgb_binary_path)
 
     assert pc.metadata.data == "binary"
     assert pc.pc_data.dtype.names == pc.metadata.fields
     assert len(pc.pc_data) == pc.metadata.points
 
@@ -254,26 +264,34 @@
     pc = PointCloud.from_path(xyzrgb_binary_compressed_path)
 
     assert pc.metadata.data == "binary_compressed"
     assert pc.pc_data.dtype.names == pc.metadata.fields
     assert len(pc.pc_data) == pc.metadata.points
 
 
+def test_load_binary_compressed_organized_pcd(xyzintensity_binary_compressed_organized_path):
+    pc = PointCloud.from_path(xyzintensity_binary_compressed_organized_path)
+
+    assert pc.metadata.data == "binary_compressed"
+    assert pc.pc_data.dtype.names == pc.metadata.fields
+    assert len(pc.pc_data) == pc.metadata.points
+
+
 def test_from_points():
     array = np.array([[1, 2, 3], [4, 5, 6]])
     fields = ("x", "y", "z")
     types = (np.float32, np.float32, np.float32)
-    count = (1, 1, 1)
+    counts = (1, 1, 1)
 
-    pc = PointCloud.from_points(array, fields, types, count)
+    pc = PointCloud.from_points(array, fields, types, counts)
 
     assert pc.fields == fields
     assert pc.types == types
     assert pc.points == 2
-    assert pc.count == count
+    assert pc.counts == counts
     assert pc.pc_data.dtype.names == fields
 
     assert np.array_equal(pc.pc_data["x"], array.T[0])
     assert np.array_equal(pc.pc_data["y"], array.T[1])
     assert np.array_equal(pc.pc_data["z"], array.T[2])
 
     assert pc.pc_data["x"].dtype == np.dtype(types[0])
@@ -658,14 +676,50 @@
     out_points = pc.numpy(fields=("x", "y"))
     assert np.allclose(out_points, in_points[:, :2])
 
     out_points = pc.numpy(fields=[])
     assert np.allclose(out_points, np.empty((0, 0)))
 
 
+def test_numpy_with_multi_count_fields(xyzintensity_ascii_multi_count_path):
+    pc = PointCloud.from_path(xyzintensity_ascii_multi_count_path)
+
+    assert pc.fields == (
+        "x",
+        "y",
+        "z",
+        "intensity__0000",
+        "intensity__0001",
+        "intensity__0002",
+        "intensity__0003",
+    )
+    assert pc.metadata.fields == (
+        "x",
+        "y",
+        "z",
+        "intensity",
+    )
+    assert pc.types == (
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+        np.float32,
+    )
+    assert pc.counts == (1, 1, 1, 1, 1, 1, 1)
+    assert pc.metadata.count == (1, 1, 1, 4)
+    assert pc.points == 8
+
+    points = pc.numpy()
+
+    assert points.shape == (8, 7)
+
+
 def test_save_as_ascii():
     in_points = np.random.randint(0, 1000, (100, 3))
     fields = ("x", "y", "z")
     types = (np.float32, np.int8, np.uint64)
     pc = PointCloud.from_points(in_points, fields, types)
 
     with TemporaryDirectory() as dirname:
@@ -805,32 +859,68 @@
 
     # Cannot concatenate because types are different
     pc5 = PointCloud.from_points(in_points, fields, (np.float32, np.int8, np.float32))
     with pytest.raises(ValueError):
         pc + pc5
 
 
-def test_pointcloud_getitem():
+def test_pointcloud_getitem_with_slice():
+    in_points = np.random.randint(0, 1000, (100, 3))
+    fields = ("x", "y", "z")
+    types = (np.float32, np.int8, np.uint64)
+    pc = PointCloud.from_points(in_points, fields, types)
+
+    # Can filter PointCloud with a slice
+    pc2 = pc[10:30]
+    assert pc2.points == 20
+    assert pc2.fields == pc.fields
+    assert pc2.types == pc.types
+
+
+def test_pointcloud_getitem_with_boolean_mask():
     in_points = np.random.randint(0, 1000, (100, 3))
     fields = ("x", "y", "z")
     types = (np.float32, np.int8, np.uint64)
     pc = PointCloud.from_points(in_points, fields, types)
 
-    # Can filter PointCloud
+    # Can filter PointCloud with a boolean mask
     mask1 = (pc.pc_data["x"] > 0.5) & (pc.pc_data["y"] < 0.5)
     pc2 = pc[mask1]
     assert pc2.points == np.count_nonzero(mask1)
     assert pc2.fields == pc.fields
     assert pc2.types == pc.types
 
-    # Can filter PointCloud with mask can be squeezed
+    # Can filter PointCloud with a boolean mask can be squeezed
     mask2 = pc.numpy("x") > 0.5
     mask2 = mask2[:, None, None, None]
     pc3 = pc[mask2]
     assert pc3.points == np.count_nonzero(mask2)
     assert pc3.fields == pc.fields
     assert pc3.types == pc.types
 
-    # Cannot filter mask dimension is not 1
+    # Cannot filter by a boolean mask since the dimension is not 1
     mask3 = pc.numpy(("x", "y")) > 0.5
     with pytest.raises(ValueError):
         pc[mask3]
+
+
+def test_pointcloud_getitem_with_field_names():
+    in_points = np.random.randint(0, 1000, (100, 3))
+    fields = ("x", "y", "z")
+    types = (np.float32, np.int8, np.uint64)
+    pc = PointCloud.from_points(in_points, fields, types)
+
+    # Can filter PointCloud with a field name "x"
+    pc2 = pc["x"]
+    assert pc2.points == pc.points
+    assert pc2.fields == ("x",)
+    assert pc2.types == (np.float32,)
+
+    # Can filter PointCloud with a field names "x" and "y"
+    pc3 = pc[("x", "y")]
+    assert pc3.points == pc.points
+    assert pc3.fields == ("x", "y")
+    assert pc3.types == (np.float32, np.int8)
+
+    # Cannot filter by fields names since the field name "a" is invalid
+    with pytest.raises(ValueError):
+        pc[("x", "y", "a")]
```

### Comparing `pypcd4-0.4.9/.gitignore` & `pypcd4-1.0.0/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 cover/
+pytest-coverage.txt
+pytest.xml
 
 # Environments
 .env
 .venv
 env/
 venv/
 ENV/
@@ -60,7 +62,10 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Editor
 .vscode/
+
+# Ruff
+.ruff_cache/
```

### Comparing `pypcd4-0.4.9/LICENSE.txt` & `pypcd4-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypcd4-0.4.9/pyproject.toml` & `pypcd4-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "pypcd4"
 dynamic = ["version"]
 description = "Read and write PCL .pcd files in python"
 authors = [{ name = "urasakikeisuke", email = "keisuke.urasaki@map4.jp" }]
 dependencies = [
     "numpy>=1.21.0",
     "python-lzf>=0.2.4",
-    "pydantic >=1.10.8, <=2.5.2",
+    "pydantic >=1.10.8, <=2.6.4",
 ]
 readme = "README.md"
 requires-python = ">= 3.8.2"
 license = { file = "LICENSE.txt" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -55,17 +55,17 @@
 [tool.rye.scripts]
 lint = { chain = [
     "lint:ruff-lint",
     "lint:ruff-format",
     "lint:mypy",
     "lint:tox",
 ] }
-"lint:ruff-lint" = "ruff check --verbose --fix src"
-"lint:ruff-format" = "ruff format --verbose src"
-"lint:mypy" = "mypy --verbose src"
+"lint:ruff-lint" = "ruff check --fix src"
+"lint:ruff-format" = "ruff format src"
+"lint:mypy" = "mypy src"
 "lint:tox" = "tox"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch]
 version.source = "vcs"
@@ -81,15 +81,15 @@
 
 [tool.ruff]
 line-length = 100
 indent-width = 4
 
 [tool.ruff.lint]
 select = ["E", "F", "I", "PLR", "B", "ANN"]
-ignore = ["ANN101", "ANN102"]
+ignore = ["ANN101", "ANN102", "PLR2004"]
 fixable = ["ALL"]
 unfixable = []
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
 docstring-code-format = true
```

### Comparing `pypcd4-0.4.9/PKG-INFO` & `pypcd4-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypcd4
-Version: 0.4.9
+Version: 1.0.0
 Summary: Read and write PCL .pcd files in python
 Project-URL: Release Notes, https://github.com/MapIV/pypcd4/releases
 Project-URL: Source, https://github.com/MapIV/pypcd4
 Project-URL: Tracker, https://github.com/MapIV/pypcd4/issues
 Author-email: urasakikeisuke <keisuke.urasaki@map4.jp>
 License: BSD 3-Clause License
         
@@ -52,24 +52,45 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8.2
 Requires-Dist: numpy>=1.21.0
-Requires-Dist: pydantic<=2.5.2,>=1.10.8
+Requires-Dist: pydantic<=2.6.4,>=1.10.8
 Requires-Dist: python-lzf>=0.2.4
 Provides-Extra: dev
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: setuptools-scm; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # pypcd4
 
+[![Test](https://github.com/MapIV/pypcd4/actions/workflows/test.yaml/badge.svg)](https://github.com/MapIV/pypcd4/actions/workflows/test.yaml)
+![PyPI - Version](https://img.shields.io/pypi/v/pypcd4)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pypcd4)
+![GitHub License](https://img.shields.io/github/license/MapIV/pypcd4)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pypcd4)
+
+## Table of Contents
+
+* [Description](#description)
+* [Installation](#installation)
+* [Usage](#usage)
+  * [Importing pypcd4](#getting-started)
+  * [Loading PCD File](#working-with-pcd-files)
+  * [Converting to NumPy Array](#converting-between-pointcloud-and-numpy-array)
+  * [Converting to ROS Message](#working-with-ros-pointcloud2-messages)
+  * [Concatenating PointClouds](#concatenating-two-pointclouds)
+  * [Filtering PointClouds](#filtering-a-pointcloud)
+  * [Saving Your Work](#saving-your-work)
+* [Contributing](#contributing)
+* [License](#license)
+
 ## Description
 
 pypcd4 is a modern reimagining of the original [pypcd](https://github.com/dimatura/pypcd) library,
 offering enhanced capabilities and performance for working with Point Cloud Data (PCD) files.
 
 This library builds upon the foundation laid by the original pypcd while incorporating modern
 Python3 syntax and methodologies to provide a more efficient and user-friendly experience.
@@ -146,22 +167,28 @@
 types = (np.float32, np.float32, np.float32, np.float32, np.float64)
 
 pc = PointCloud.from_points(array, fields, types)
 ```
 
 ### Working with ROS PointCloud2 Messages
 
-As of v0.4.0, you can convert a ROS PointCloud2 Message to a PointCloud:
+You can convert a ROS PointCloud2 Message to a PointCloud and vice versa:
 
 ```python
-def callback(msg):
-    pc = PointCloud.from_msg(msg)
+def callback(in_msg: sensor_msgs.msg.PointCloud2):
+    # Convert ROS PointCloud2 Message to a PointCloud
+    pc = PointCloud.from_msg(in_msg)
 
     pc.fields
     # ("x", "y", "z", "intensity", "ring", "time")
+
+    # Convert PointCloud to ROS PointCloud2 Message with the input message header
+    out_msg = pc.to_msg(in_msg.header)
+
+    publisher.publish(out_msg)
 ```
 
 ### Concatenating Two PointClouds
 
 The `pypcd4` supports concatenating two `PointCloud` objects together using the `+` operator.
 This can be very useful when you want to merge two point clouds into one.
 
@@ -175,38 +202,100 @@
 pc3: PointCloud = pc1 + pc2
 ```
 
 Please note that the two PointCloud objects must have the same fields and types. If they don’t, a `ValueError` will be raised.
 
 ### Filtering a PointCloud
 
-The `pypcd4` library provides a convenient way to filter a `PointCloud` using a mask.
-Here's an example of how you can use it:
+The `pypcd4` library provides a convenient way to filter a `PointCloud` using a subscript.
+
+#### Using a Slice
+
+You can use a slice to access a range of points in the point cloud. Here’s an example:
 
 ```python
-# Create a random PointCloud
-pc = PointCloud.from_xyz_points(np.random.rand(100, 3))
+# Create a point cloud with random points
+pc = PointCloud.from_xyz_points(np.random.rand(10, 3))
+
+# Access points using a slice
+subset = pc[3:8]
+```
+
+In this case, subset will be a new PointCloud object containing only the points from index 3 to 7.
 
-# Create a mask
+#### Using a Boolean Mask
+
+You can use a boolean mask to access points that satisfy certain conditions. Here’s an example:
+
+```python
+# Create a point cloud with random points
+pc = PointCloud.from_xyz_points(np.random.rand(10000, 3))
+
+# Create a boolean mask
 mask = (pc.pc_data["x"] > 0.5) & (pc.pc_data["y"] < 0.5)
 
-# Apply the mask to the PointCloud
-filtered_pc = pc[mask]
+# Access points using the mask
+subset = pc[mask]
+```
+
+In this case, subset will be a new PointCloud object containing only the points where the x-coordinate is greater than 0.5 and the y-coordinate is less than 0.5.
+
+#### Using Field Names
+
+You can use a field name or a sequence of field names to access specific fields in the point cloud. Here’s an example:
 
-# The filtered PointCloud only includes the points that match the mask
-print(filtered_pc.numpy())
+```python
+# Create a point cloud with random points
+pc = PointCloud.from_xyz_points(np.random.rand(100, 3))
+
+# Access specific fields
+subset = pc[("x", "y")]
 ```
 
-Please note that the mask must be a 1-dimensional array. If it’s not, a `ValueError` will be raised.
+In this case, subset will be a new PointCloud object containing only the x and y coordinates of the points.
+The z-coordinate will not be included.
 
 ### Saving Your Work
 
 Finally, you can save your PointCloud as a .pcd file:
 
 ```python
 pc.save("nice_point_cloud.pcd")
 ```
 
+## Contributing
+
+We are always looking for contributors. If you are interested in contributing,
+please run the lint and test before submitting a pull request:
+
+### Using Rye (Recommended)
+
+Just run the following command:
+
+```bash
+rye sync
+rye run lint
+```
+
+### Using pip
+
+Install the testing dependencies by the following command:
+
+```bash
+pip install mypy pytest ruff
+```
+
+Then run the following command:
+
+```bash
+ruff check --fix src
+ruff format src
+mypy src
+pytest
+```
+
+Make sure all lints and tests pass before submitting a pull request.
+
 ## License
 
 The library was rewritten and does not borrow any code from the original [pypcd](https://github.com/dimatura/pypcd) library.
 Since it was heavily inspired by the original author's work, we extend his original BSD 3-Clause License and include his Copyright notice.
```

