# Comparing `tmp/paicorelib-1.0.0rc1.tar.gz` & `tmp/paicorelib-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paicorelib-1.0.0rc1.tar", max compression
+gzip compressed data, was "paicorelib-1.1.0rc1.tar", max compression
```

## Comparing `paicorelib-1.0.0rc1.tar` & `paicorelib-1.1.0rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       63 2024-04-16 07:52:04.051343 paicorelib-1.0.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0      888 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/README.md
--rw-r--r--   0        0        0     1742 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/docs/Table-of-Terms.md
--rw-r--r--   0        0        0     1189 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/__init__.py
--rw-r--r--   0        0        0    14867 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/coordinate.py
--rw-r--r--   0        0        0       75 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/__init__.py
--rw-r--r--   0        0        0     5142 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/base.py
--rw-r--r--   0        0        0     7150 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/frame_defs.py
--rw-r--r--   0        0        0     9920 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/frame_gen.py
--rw-r--r--   0        0        0    21957 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/frames.py
--rw-r--r--   0        0        0      706 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/types.py
--rw-r--r--   0        0        0     3988 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/utils.py
--rw-r--r--   0        0        0     1461 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/hw_defs.py
--rw-r--r--   0        0        0     2312 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/hw_types.py
--rw-r--r--   0        0        0     7472 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/ram_model.py
--rw-r--r--   0        0        0     2618 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/ram_types.py
--rw-r--r--   0        0        0     5844 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/reg_model.py
--rw-r--r--   0        0        0     4265 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/reg_types.py
--rw-r--r--   0        0        0     5174 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/routing_defs.py
--rw-r--r--   0        0        0     1571 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 paicorelib-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      163 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/LICENSE
+-rw-r--r--   0        0        0      837 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/README.md
+-rw-r--r--   0        0        0     1775 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/docs/Table-of-Terms.md
+-rw-r--r--   0        0        0     1188 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/__init__.py
+-rw-r--r--   0        0        0    15668 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/coordinate.py
+-rw-r--r--   0        0        0       81 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/__init__.py
+-rw-r--r--   0        0        0     5212 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/base.py
+-rw-r--r--   0        0        0     7150 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/frame_defs.py
+-rw-r--r--   0        0        0     9900 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/frame_gen.py
+-rw-r--r--   0        0        0    22003 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/frames.py
+-rw-r--r--   0        0        0      736 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/types.py
+-rw-r--r--   0        0        0     4034 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/utils.py
+-rw-r--r--   0        0        0     1532 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/hw_defs.py
+-rw-r--r--   0        0        0     2312 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/hw_types.py
+-rw-r--r--   0        0        0     7488 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/ram_model.py
+-rw-r--r--   0        0        0     2618 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/ram_types.py
+-rw-r--r--   0        0        0     5816 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/reg_model.py
+-rw-r--r--   0        0        0     4265 2024-05-15 07:32:44.424499 paicorelib-1.1.0rc1/paicorelib/reg_types.py
+-rw-r--r--   0        0        0     5757 2024-05-15 07:32:44.424499 paicorelib-1.1.0rc1/paicorelib/routing_defs.py
+-rw-r--r--   0        0        0     1732 2024-05-15 07:32:44.424499 paicorelib-1.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 paicorelib-1.1.0rc1/PKG-INFO
```

### Comparing `paicorelib-1.0.0rc1/LICENSE` & `paicorelib-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `paicorelib-1.0.0rc1/README.md` & `paicorelib-1.1.0rc1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIlib/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paicorelib">
     </a>
-    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.0.0rc1">
-        <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?include_prereleases&color=orange">
+    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.1.0rc1">
+        <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIlib">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIlib/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIlib/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIlib/master.svg" alt="pre-commit.ci status">
     </a>
 
 </p>
 
-术语对照表：[Table of Terms](docs/Table-of-Terms.md)
+[Changelog](./CHANGELOG.md)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
                            # Library of PAICORE 2.0
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_c_o_r_e_l_i_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
- _g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_?_i_n_c_l_u_d_e___p_r_e_r_e_l_e_a_s_e_s_&_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-
-                               _c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
-æ¯è¯­å¯¹ç§è¡¨ï¼[Table of Terms](docs/Table-of-Terms.md)
+   _g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_?_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+   _c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
+                                    _s_t_a_t_u_s_]
+[Changelog](./CHANGELOG.md)
```

### Comparing `paicorelib-1.0.0rc1/docs/Table-of-Terms.md` & `paicorelib-1.1.0rc1/docs/Table-of-Terms.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Table of Terms
 
-|     V2.1参数名     |                   定义                   |   原类型名或变量名   | 输入参数模型的统一类型名或变量名 | 参数模型导出字典键 |
+|     V2.1参数名      |                   定义                   |   原类型名或变量名    | 输入参数模型的统一类型名或变量名 | 参数模型导出字典键 |
 | :-----------------: | :--------------------------------------: | :-------------------: | :------------------------------: | :----------------: |
-|  weight_det_stoch  |        突触整合确定或随机模式选择        |    LeakModeType    |     SynapticIntegrationMode     |    Same as V2.1    |
-|   leak_det_stoch   |        泄露整合确定或随机模式选择        |    WeightModeType    |      LeakIntegrationMode      |    Same as V2.1    |
-| leak_reversal_flag |        泄露正向或反向反转模式选择        | LeakDirectionType |       LeakDirectionMode       |    Same as V2.1    |
-|      leak_post      |           比较前后泄露模式选择           | LeakComparisonType |      LeakComparisonMode      |    Same as V2.1    |
-|     reset_mode     |            膜电平复位模式选择            |     ResetModeType     |            ResetMode            |    Same as V2.1    |
-|       reset_v       |          膜电平常数复位的复位值          |        reset_v        |             reset_v             |    Same as V2.1    |
-| threshold_neg_mode | 负阈值地板（饱和）或重置（复位）模式选择 | NegativeThresModeType |      NegativeThresholdMode      |    Same as V2.1    |
-| threshold_mask_ctrl |              阈值随机数掩码              |    thres_mask_ctrl    |       threshold_mask_bits       |    Same as V2.1    |
+|  weight_det_stoch   |        突触整合确定或随机模式选择        |     LeakModeType      |     SynapticIntegrationMode      |    Same as V2.1    |
+|   leak_det_stoch    |        泄露整合确定或随机模式选择        |    WeightModeType     |       LeakIntegrationMode        |    Same as V2.1    |
+| leak_reversal_flag  |        泄露正向或反向反转模式选择        |   LeakDirectionType   |        LeakDirectionMode         |    Same as V2.1    |
+|      leak_post      |           比较前后泄露模式选择           |  LeakComparisonType   |        LeakComparisonMode        |    Same as V2.1    |
+|     reset_mode      |            膜电平复位模式选择            |     ResetModeType     |            ResetMode             |    Same as V2.1    |
+|       reset_v       |          膜电平常数复位的复位值          |        reset_v        |             reset_v              |    Same as V2.1    |
+| threshold_neg_mode  | 负阈值地板（饱和）或重置（复位）模式选择 | NegativeThresModeType |      NegativeThresholdMode       |    Same as V2.1    |
+| threshold_mask_ctrl |              阈值随机数掩码              |    thres_mask_ctrl    |       threshold_mask_bits        |    Same as V2.1    |
 |       vjt_pre       |               神经元膜电位               |        vjt_pre        |             vjt_init             |      vjt_init      |
```

### Comparing `paicorelib-1.0.0rc1/paicorelib/__init__.py` & `paicorelib-1.1.0rc1/paicorelib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from importlib.metadata import version
+
 from .coordinate import *
 from .framelib import *
 
 # In recent versions, `HwConfig` for external packages remain unchanged.
 from .hw_defs import HwParams as HwConfig
 from .hw_types import *
 from .ram_model import *
@@ -19,14 +21,11 @@
 from .reg_types import LCNExtensionType as LCN_EX
 from .reg_types import MaxPoolingEnableType as MaxPoolingEnable
 from .reg_types import SNNModeEnableType as SNNModeEnable
 from .reg_types import SpikeWidthFormatType as SpikeWidthFormat
 from .reg_types import WeightPrecisionType as WeightPrecision
 from .routing_defs import *
 
-
-from importlib.metadata import version
-
 try:
     __version__ = version("paicorelib")
 except Exception:
     __version__ = None
```

### Comparing `paicorelib-1.0.0rc1/paicorelib/coordinate.py` & `paicorelib-1.1.0rc1/paicorelib/coordinate.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,37 +11,41 @@
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 from .hw_defs import HwParams
 
 __all__ = [
+    "ChipCoord",
     "Coord",
+    "CoordAddr",
     "CoordOffset",
     "ReplicationId",
     "CoordLike",
     "RIdLike",
     "to_coord",
+    "to_coords",
     "to_coordoffset",
     "to_rid",
 ]
 
 CoordTuple: TypeAlias = Tuple[int, int]
+CoordAddr: TypeAlias = int
 
 
 def _xy_parser(other: Union[CoordTuple, "CoordOffset"]) -> CoordTuple:
     """Parse the coordinate in tuple format."""
     if not isinstance(other, (tuple, CoordOffset)):
         raise TypeError(f"unsupported type: {type(other)}.")
 
     if isinstance(other, tuple):
         if len(other) != 2:
             raise ValueError(f"expected a tuple of 2 elements, but got {len(other)}.")
 
-        return CoordOffset.from_tuple(other).to_tuple()
+        return CoordOffset(*other).to_tuple()  # check the range of coordoffset
     else:
         return other.to_tuple()
 
 
 class _CoordIdentifier(ABC):
     """Identifier to descripe coordinate of hardware unit. \
         The subclass of identifier must implement `__eq__` & `__ne__`."""
@@ -59,30 +63,22 @@
 class Coord(_CoordIdentifier):
     """Coordinate of the cores. Set coordinate (x, y) for every core.
 
     Left to right, +X, up to down, +Y.
     """
 
     x: int = Field(
-        default=HwParams.CORE_X_MIN,
-        ge=HwParams.CORE_X_MIN,
-        le=HwParams.CORE_X_MAX,
+        default=HwParams.CORE_X_MIN, ge=HwParams.CORE_X_MIN, le=HwParams.CORE_X_MAX
     )
     y: int = Field(
-        default=HwParams.CORE_Y_MIN,
-        ge=HwParams.CORE_Y_MIN,
-        le=HwParams.CORE_Y_MAX,
+        default=HwParams.CORE_Y_MIN, ge=HwParams.CORE_Y_MIN, le=HwParams.CORE_Y_MAX
     )
 
     @classmethod
-    def from_tuple(cls, pos: CoordTuple) -> "Coord":
-        return cls(*pos)
-
-    @classmethod
-    def from_addr(cls, addr: int) -> "Coord":
+    def from_addr(cls, addr: CoordAddr) -> "Coord":
         return cls(addr >> HwParams.N_BIT_CORE_Y, addr & HwParams.CORE_Y_MAX)
 
     def __add__(self, __other: "CoordOffset") -> "Coord":
         """
         Example:
         >>> c1 = Coord(1, 1)
         >>> c2 = c1 + CoordOffset(1, 1)
@@ -219,44 +215,65 @@
     def __xor__(self, __other: "Coord") -> "ReplicationId":
         return ReplicationId(self.x ^ __other.x, self.y ^ __other.y)
 
     def __hash__(self) -> int:
         return hash(self.address)
 
     def __str__(self) -> str:
-        return f"({self.x}, {self.y})"
-
-    def __repr__(self) -> str:
-        return f"Coord({self.x}, {self.y})"
+        return f"({self.x},{self.y})"
 
     def to_tuple(self) -> CoordTuple:
         """Convert to tuple"""
         return (self.x, self.y)
 
     @property
-    def address(self) -> int:
+    def address(self) -> CoordAddr:
         """Convert to address, 10 bits"""
         return (self.x << HwParams.N_BIT_CORE_Y) | self.y
 
 
 @final
 class ReplicationId(Coord):
     @classmethod
-    def from_addr(cls, addr: int) -> "ReplicationId":
+    def from_addr(cls, addr: CoordAddr) -> "ReplicationId":
         return cls(addr >> HwParams.N_BIT_CORE_Y, addr & HwParams.CORE_Y_MAX)
 
     def __and__(self, __other: Union[Coord, "ReplicationId"]) -> "ReplicationId":
         return ReplicationId(self.x & __other.x, self.y & __other.y)
 
     def __or__(self, __other: Union[Coord, "ReplicationId"]) -> "ReplicationId":
         return ReplicationId(self.x | __other.x, self.y | __other.y)
 
     def __xor__(self, __other: Union[Coord, "ReplicationId"]) -> "ReplicationId":
         return ReplicationId(self.x ^ __other.x, self.y ^ __other.y)
 
+    def __iand__(self, __other: Union[Coord, "ReplicationId"]) -> "ReplicationId":
+        self.x &= __other.x
+        self.y &= __other.y
+
+        return self
+
+    def __ior__(self, __other: Union[Coord, "ReplicationId"]) -> "ReplicationId":
+        self.x |= __other.x
+        self.y |= __other.y
+
+        return self
+
+    def __ixor__(self, __other: Union[Coord, "ReplicationId"]) -> "ReplicationId":
+        self.x ^= __other.x
+        self.y ^= __other.y
+
+        return self
+
+    def __str__(self) -> str:
+        return f"({self.x}, {self.y})*"
+
+    def __repr__(self) -> str:
+        return f"RId({self.x}, {self.y})"
+
     # def __lshift__(self, __bit: int) -> int:
     #     return self.address << __bit
 
     # def __rshift__(self, __bit: int) -> int:
     #     return self.address >> __bit
 
 
@@ -274,16 +291,16 @@
         default=HwParams.CORE_X_MIN, ge=-HwParams.CORE_X_MAX, le=HwParams.CORE_X_MAX
     )
     delta_y: int = Field(
         default=HwParams.CORE_Y_MIN, ge=-HwParams.CORE_Y_MAX, le=HwParams.CORE_Y_MAX
     )
 
     @classmethod
-    def from_tuple(cls, pos: CoordTuple) -> "CoordOffset":
-        return cls(*pos)
+    def from_offset(cls, offset: int) -> "CoordOffset":
+        return cls(offset >> HwParams.N_BIT_CORE_Y, offset & HwParams.CORE_Y_MAX)
 
     @overload
     def __add__(self, __other: Coord) -> Coord: ...
 
     @overload
     def __add__(self, __other: "CoordOffset") -> "CoordOffset": ...
 
@@ -375,14 +392,20 @@
             return self.delta_x == __other.delta_x and self.delta_y == __other.delta_y
         else:
             raise TypeError(f"unsupported type: {type(__other)}.")
 
     def __ne__(self, __other: "CoordOffset") -> bool:
         return not self.__eq__(__other)
 
+    def __str__(self) -> str:
+        return f"({self.delta_x}, {self.delta_y})"
+
+    def __repr__(self) -> str:
+        return f"CoordOffset({self.delta_x}, {self.delta_y})"
+
     def to_tuple(self) -> CoordTuple:
         """Convert to tuple"""
         return (self.delta_x, self.delta_y)
 
     def to_distance(
         self, distance_type: DistanceType = DistanceType.DISTANCE_ENCLIDEAN
     ) -> Union[float, int]:
@@ -454,20 +477,21 @@
                 raise ValueError(
                     f"coordinate of X out of low limit {HwParams.CORE_X_MIN}."
                 )
 
     return cx, cy
 
 
-CoordLike = TypeVar("CoordLike", Coord, int, List[int], CoordTuple)
-RIdLike = TypeVar("RIdLike", ReplicationId, int, List[int], CoordTuple)
+ChipCoord: TypeAlias = Coord
+CoordLike = TypeVar("CoordLike", Coord, CoordAddr, CoordTuple)
+RIdLike = TypeVar("RIdLike", ReplicationId, CoordAddr, CoordTuple)
 
 
 def to_coord(coordlike: CoordLike) -> Coord:
-    if isinstance(coordlike, int):
+    if isinstance(coordlike, CoordAddr):
         return Coord.from_addr(coordlike)
 
     if isinstance(coordlike, (list, tuple)):
         if len(coordlike) != 2:
             raise TypeError(
                 f"expected a tuple or list of 2 elements, but got {len(coordlike)}."
             )
@@ -484,15 +508,15 @@
 def to_coordoffset(offset: int) -> CoordOffset:
     return CoordOffset(
         offset % (HwParams.CORE_X_MAX + 1), offset // (HwParams.CORE_Y_MAX + 1)
     )
 
 
 def to_rid(ridlike: RIdLike) -> ReplicationId:
-    if isinstance(ridlike, int):
+    if isinstance(ridlike, CoordAddr):
         return ReplicationId.from_addr(ridlike)
 
     if isinstance(ridlike, (list, tuple)):
         if len(ridlike) != 2:
             raise ValueError(
                 f"expected a tuple or list of 2 elements, but got {len(ridlike)}."
             )
```

### Comparing `paicorelib-1.0.0rc1/paicorelib/framelib/base.py` & `paicorelib-1.1.0rc1/paicorelib/framelib/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+import copy
 from dataclasses import dataclass, field
 from typing import Union
-import copy
+
 import numpy as np
 
-from paicorelib import Coord, ReplicationId as RId
+from paicorelib import Coord
+from paicorelib import ReplicationId as RId
+
+from .frame_defs import FrameFormat as FF
+from .frame_defs import FrameHeader as FH
+from .frame_defs import FrameType as FT
 from .types import FRAME_DTYPE, FrameArrayType
-from .frame_defs import FrameFormat as FF, FrameHeader as FH, FrameType as FT
 from .utils import header2type
 
 
 @dataclass
 class Frame:
     """frames which contains information.
```

### Comparing `paicorelib-1.0.0rc1/paicorelib/framelib/frame_defs.py` & `paicorelib-1.1.0rc1/paicorelib/framelib/frame_defs.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.0.0rc1/paicorelib/framelib/frame_gen.py` & `paicorelib-1.1.0rc1/paicorelib/framelib/frame_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from typing import Any, Dict, Union, overload
+
 import numpy as np
 from numpy.typing import NDArray
 
-from paicorelib import Coord, LCN_EX, NeuronAttrs, NeuronDestInfo, ParamsReg
+from paicorelib import LCN_EX, Coord, NeuronAttrs, NeuronDestInfo, ParamsReg
 from paicorelib import ReplicationId as RId
 from paicorelib import WeightPrecision as WP
-from .frames import *
-from .types import (
-    DataArrayType,
-    FrameArrayType,
-    FRAME_DTYPE,
-    IntScalarType,
-)
 
+from .frames import *
+from .types import FRAME_DTYPE, DataArrayType, FrameArrayType, IntScalarType
 
 __all__ = ["OfflineFrameGen"]
 
 
 class OfflineFrameGen:
     """Offline frame generator."""
```

### Comparing `paicorelib-1.0.0rc1/paicorelib/framelib/frames.py` & `paicorelib-1.1.0rc1/paicorelib/framelib/frames.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 from typing import Any, ClassVar, Dict, Optional, Union
 
 import numpy as np
 from numpy.typing import NDArray
 
 from paicorelib import Coord, CoordLike
 from paicorelib import ReplicationId as RId
-from paicorelib import RIdLike
-from paicorelib import to_coord, to_rid
+from paicorelib import RIdLike, to_coord, to_rid
 from paicorelib.hw_defs import HwParams
 from paicorelib.ram_model import NeuronAttrsChecker, NeuronDestInfoChecker
 from paicorelib.reg_model import ParamsRegChecker
-from .types import FRAME_DTYPE, ArrayType, DataType, FrameArrayType
+
 from .base import Frame, FramePackage
-from .frame_defs import (
-    FrameFormat as FF,
-    FrameHeader as FH,
-    ParameterRAMFormat as RAMF,
-    ParameterRegFormat as RegF,
-    SpikeFrameFormat as WF1F,
-)
+from .frame_defs import FrameFormat as FF
+from .frame_defs import FrameHeader as FH
+from .frame_defs import ParameterRAMFormat as RAMF
+from .frame_defs import ParameterRegFormat as RegF
+from .frame_defs import SpikeFrameFormat as WF1F
+from .types import FRAME_DTYPE, ArrayType, DataType, FrameArrayType
 from .utils import (
+    OUT_OF_RANGE_WARNING,
     ShapeError,
     TruncationWarning,
     bin_split,
     params_check,
     params_check2,
-    OUT_OF_RANGE_WARNING,
 )
 
 __all__ = [
     "OfflineConfigFrame1",
     "OfflineConfigFrame2",
     "OfflineConfigFrame3",
     "OfflineConfigFrame4",
```

### Comparing `paicorelib-1.0.0rc1/paicorelib/framelib/types.py` & `paicorelib-1.1.0rc1/paicorelib/framelib/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 
 FRAME_DTYPE: TypeAlias = np.uint64
 FrameArrayType: TypeAlias = NDArray[FRAME_DTYPE]
 ArrayType = TypeVar("ArrayType", List[int], Tuple[int, ...], np.ndarray)
 BasicFrameArray = TypeVar(
     "BasicFrameArray", int, List[int], Tuple[int, ...], NDArray[FRAME_DTYPE]
 )
-IntScalarType = TypeVar("IntScalarType", int, np.integer)
-DataType = TypeVar("DataType", int, np.integer, np.ndarray)
+IntScalarType = TypeVar("IntScalarType", int, np.bool_, np.integer)
+DataType = TypeVar("DataType", int, np.bool_, np.integer, np.ndarray)
 DataArrayType = TypeVar(
-    "DataArrayType", int, np.integer, List[int], Tuple[int, ...], np.ndarray
+    "DataArrayType", int, np.bool_, np.integer, List[int], Tuple[int, ...], np.ndarray
 )
```

### Comparing `paicorelib-1.0.0rc1/paicorelib/framelib/utils.py` & `paicorelib-1.1.0rc1/paicorelib/framelib/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from functools import wraps
 from pathlib import Path
 from typing import Any, Dict, Optional, Tuple
 
 import numpy as np
 from pydantic import TypeAdapter
 
-from .frame_defs import FrameFormat as FF, FrameHeader as FH, FrameType as FT
+from .frame_defs import FrameFormat as FF
+from .frame_defs import FrameHeader as FH
+from .frame_defs import FrameType as FT
 from .types import FRAME_DTYPE, BasicFrameArray, FrameArrayType
 
 
 class FrameIllegalError(ValueError):
     """Frame is illegal."""
 
     pass
```

### Comparing `paicorelib-1.0.0rc1/paicorelib/hw_defs.py` & `paicorelib-1.1.0rc1/paicorelib/hw_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from typing import Literal
 
-
 __all__ = ["HwParams"]
 
 
 class HwParams:
     """Basic hardware configuration of PAICORE 2.0."""
 
     COORD_Y_PRIORITY: bool = True
     """Coordinate priority"""
 
     WEIGHT_BITORDER: Literal["little", "big"] = "little"
 
+    N_CHIP_MAX = 1024
     CHIP_X_MIN = 0
     CHIP_X_MAX = 0
     CHIP_Y_MIN = 0
     CHIP_Y_MAX = 0
 
     N_BIT_CORE_X = 5
     N_BIT_CORE_Y = 5
 
     CORE_X_MIN = 0
     CORE_X_MAX = (1 << N_BIT_CORE_X) - 1
     CORE_Y_MIN = 0
     CORE_Y_MAX = (1 << N_BIT_CORE_Y) - 1
 
+    N_CORE_MAX_INCHIP = 1024
     N_CORE_OFFLINE = 1008
-    """The #N of offline cores."""
+    N_CORE_ONLINE = N_CORE_MAX_INCHIP - N_CORE_OFFLINE
+
     CORE_X_OFFLINE_MIN = CORE_X_MIN
     CORE_Y_OFFLINE_MIN = CORE_Y_MIN
     CORE_X_OFFLINE_MAX = 0b11011
     CORE_Y_OFFLINE_MAX = 0b11011
     CORE_X_ONLINE_MIN = 0b11100
     CORE_Y_ONLINE_MIN = 0b11100
     CORE_X_ONLINE_MAX = CORE_X_MAX
```

### Comparing `paicorelib-1.0.0rc1/paicorelib/hw_types.py` & `paicorelib-1.1.0rc1/paicorelib/hw_types.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.0.0rc1/paicorelib/ram_model.py` & `paicorelib-1.1.0rc1/paicorelib/ram_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,16 @@
     InstanceOf,
     field_serializer,
     field_validator,
     model_validator,
 )
 from pydantic.type_adapter import TypeAdapter
 from pydantic.types import NonNegativeInt
-from typing_extensions import (
-    NotRequired,
-    TypedDict,  # Use `typing_extensions.TypedDict`.
-)
+from typing_extensions import TypedDict  # Use `typing_extensions.TypedDict`.
+from typing_extensions import NotRequired
 
 from .hw_defs import HwParams
 from .hw_types import AxonCoord
 from .ram_types import *
 
 __all__ = ["NeuronDestInfo", "NeuronAttrs"]
```

### Comparing `paicorelib-1.0.0rc1/paicorelib/ram_types.py` & `paicorelib-1.1.0rc1/paicorelib/ram_types.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.0.0rc1/paicorelib/reg_model.py` & `paicorelib-1.1.0rc1/paicorelib/reg_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 from typing import Literal
-from pydantic import (
-    BaseModel,
-    ConfigDict,
-    Field,
-    field_serializer,
-    model_validator,
-)
+
+from pydantic import BaseModel, ConfigDict, Field, field_serializer, model_validator
 from pydantic.type_adapter import TypeAdapter
 from pydantic.types import NonNegativeInt
 from typing_extensions import TypedDict  # Use `typing_extensions.TypedDict`.
 
 from .coordinate import Coord
 from .hw_defs import HwParams
 from .reg_types import *
@@ -18,27 +13,27 @@
 
 NUM_DENDRITE_BIT_MAX = 13
 TICK_WAIT_START_BIT_MAX = 15
 TICK_WAIT_END_BIT_MAX = 15
 TARGET_LCN_BIT_MAX = 4
 TEST_CHIP_ADDR_BIT_MAX = 10
 
-NUM_DENDRITE_OUT_OF_RANGE_FORMAT = (
+NUM_DENDRITE_OUT_OF_RANGE_TEXT = (
     "param 'num_dendrite' out of range. When input width is 8-bit in {0} mode, "
     + "the number of dendrites should be no more than {1}."
 )
 
 
 def _num_dendrite_out_of_range_repr(mode: Literal["ANN", "SNN"]) -> str:
     if mode == "ANN":
         max_limit = HwParams.N_DENDRITE_MAX_ANN
     else:
         max_limit = HwParams.N_DENDRITE_MAX_SNN
 
-    return NUM_DENDRITE_OUT_OF_RANGE_FORMAT.format(mode, max_limit)
+    return NUM_DENDRITE_OUT_OF_RANGE_TEXT.format(mode, max_limit)
 
 
 class CoreParams(BaseModel):
     """Parameter model of register parameters listed in Section 2.4.1.
 
     NOTE: The parameters input in the model are declared in `docs/Table-of-Terms.md`.
     """
```

### Comparing `paicorelib-1.0.0rc1/paicorelib/reg_types.py` & `paicorelib-1.1.0rc1/paicorelib/reg_types.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.0.0rc1/paicorelib/routing_defs.py` & `paicorelib-1.1.0rc1/paicorelib/routing_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     "ROUTING_DIRECTIONS_IDX",
     "RoutingCoord",
     "get_routing_consumption",
     "get_multicast_cores",
     "get_replication_id",
 ]
 
+N_ROUTING_LEVEL = 6  # L0~L5
+MAX_ROUTING_PATH_LENGTH = N_ROUTING_LEVEL - 1
+
 
 @unique
 class RoutingLevel(IntEnum):
     """The level of routing node.
 
     L0-level nodes are leaves of tree to store data. A L0-cluster is a physical core.
     """
@@ -31,34 +34,33 @@
     L3 = 3
     L4 = 4
     L5 = 5
 
 
 @unique
 class RoutingDirection(Enum):
-    """Indicate the 4 children of a cluster.
-
-    NOTE: There is an X/Y coordinate priority method to specify the order.
-    """
+    """Indicate the direction of the four children in the cluster."""
 
     X0Y0 = (0, 0)
     X0Y1 = (0, 1)
     X1Y0 = (1, 0)
     X1Y1 = (1, 1)
     ANY = (-1, -1)
-    """Don't care when a level direction is `ANY`."""
 
     def to_index(self) -> int:
         """Convert the direction to index in children list."""
         if self is RoutingDirection.ANY:
             raise TypeError(f"The direction of routing is not specified.")
 
         x, y = self.value
 
-        return (x << 1) + y
+        if HwParams.COORD_Y_PRIORITY:
+            return (x << 1) + y
+        else:
+            return (y << 1) + x
 
 
 @unique
 class RoutingStatus(IntEnum):
     """Indicate the status of L0-level cluster. Not used."""
 
     AVAILABLE = 0
@@ -76,22 +78,26 @@
 
 class RoutingCost(NamedTuple):
     n_L0: int
     n_L1: int
     n_L2: int
     n_L3: int
     n_L4: int
+    n_L5: int = 1
 
     def get_routing_level(self) -> RoutingLevel:
-        """Return the routing cluster level.
-
-        If the #N of Lx-level > 1, then we need a cluster with level Lx+1.
-        And we need the #N of routing sub-level clusters.
+        """Return the routing cluster level. If the #N of Lx-level > 1, then we need a  \
+            cluster with level Lx+1. And we need the #N of routing sub-level clusters.
+        
+        XXX: At present, if #N of L5 > 1, raise exception. 
         """
-        for i in reversed(range(5)):
+        if self.n_L5 > 1:
+            raise ValueError(f"#N of L5-level node out of range, got {self.n_L5}.")
+
+        for i in reversed(range(N_ROUTING_LEVEL)):
             if self[i] > 1:
                 return RoutingLevel(i + 1)
 
         return RoutingLevel.L1
 
 
 ROUTING_DIRECTIONS_IDX = (
@@ -110,32 +116,43 @@
     )
 )
 
 
 class RoutingCoord(NamedTuple):
     """Use router directions to represent the coordinate of a cluster."""
 
-    L4: RoutingDirection
-    L3: RoutingDirection
-    L2: RoutingDirection
-    L1: RoutingDirection
-    L0: RoutingDirection
+    L4: RoutingDirection = RoutingDirection.ANY
+    L3: RoutingDirection = RoutingDirection.ANY
+    L2: RoutingDirection = RoutingDirection.ANY
+    L1: RoutingDirection = RoutingDirection.ANY
+    L0: RoutingDirection = RoutingDirection.ANY
+
+    def _coord_specify_check(self) -> None:
+        if RoutingDirection.ANY in self:
+            raise ValueError(
+                f"The direction of routing is not specified completely, got {self}."
+            )
+
+    def _L0_property(self) -> None:
+        if self.level > RoutingLevel.L0:
+            raise AttributeError(
+                f"This property is only for L0-level cluster, but self is {self.level}."
+            )
 
     @property
     def level(self) -> RoutingLevel:
         for i in range(len(self)):
             if self[i] is RoutingDirection.ANY:
-                return RoutingLevel(5 - i)
+                return RoutingLevel(MAX_ROUTING_PATH_LENGTH - i)
 
         return RoutingLevel.L0
 
-    @property
-    def coordinate(self) -> Coord:
-        if self.level > RoutingLevel.L0:
-            raise AttributeError("This property is only for L0-level cluster.")
+    def to_coord(self) -> Coord:
+        self._L0_property()
+        self._coord_specify_check()
 
         x = (
             (self.L4.value[0] << 4)
             + (self.L3.value[0] << 3)
             + (self.L2.value[0] << 2)
             + (self.L1.value[0] << 1)
             + self.L0.value[0]
@@ -153,23 +170,21 @@
 
 
 def get_routing_consumption(n_core: int) -> RoutingCost:
     """Get the consumption of clusters at different levels by given the `n_core`."""
     n_sub_node = HwParams.N_SUB_ROUTING_NODE
 
     # Find the nearest #N(=2^X) to accommodate `n_core` L0-level clusters.
-    # If n_core = 5, return 8.
-    # If n_core = 20, return 32.
-    n_L0 = 1 << (n_core - 1).bit_length()
-    n_L1 = 1 if n_L0 < n_sub_node else (n_L0 // n_sub_node)
-    n_L2 = 1 if n_L1 < n_sub_node else (n_L1 // n_sub_node)
-    n_L3 = 1 if n_L2 < n_sub_node else (n_L2 // n_sub_node)
-    n_L4 = 1 if n_L3 < n_sub_node else (n_L3 // n_sub_node)
+    n_Lx = [0] * N_ROUTING_LEVEL
+    n_Lx[0] = 1 << (n_core - 1).bit_length()
+
+    for i in range(N_ROUTING_LEVEL - 1):
+        n_Lx[1 + i] = 1 if n_Lx[i] < n_sub_node else (n_Lx[i] // n_sub_node)
 
-    return RoutingCost(n_L0, n_L1, n_L2, n_L3, n_L4)
+    return RoutingCost(*n_Lx)
 
 
 def get_replication_id(coords: Sequence[Coord]) -> RId:
     """Get the replication ID by given the coordinates.
 
     Args:
         - coords: sequence of coordinates.
```

### Comparing `paicorelib-1.0.0rc1/pyproject.toml` & `paicorelib-1.1.0rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 [tool.poetry]
 name = "paicorelib"
-version = "1.0.0rc1"
-description = "Library of PAICORE 2.0."
+version = "1.1.0rc1"
+description = "Library of PAICORE 2.0"
 authors = ["Ziru Pan <zrpan@stu.pku.edu.cn>"]
-maintainers = ["Ziru Pan <zrpan@stu.pku.edu.cn>"]
+maintainers = [
+    "Hongtu Xia <hongtux@pku.edu.cn>",
+    "Siyuan Gao <siyuan-gao@outlook.com>",
+    "Zhaoyang Hao <hzyang2218@gmail.com>",
+    "Ziru Pan <zrpan@stu.pku.edu.cn>",
+]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/PAICookers/PAIlib"
 homepage = "https://github.com/PAICookers/PAIlib"
 documentation = "https://github.com/PAICookers/PAIlib#readme"
-keywords = ["PAICORE 2.0", "PAIBox", "PAILib"]
+keywords = ["PAICORE 2.0", "PAICORE library", "PAILib"]
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -30,15 +35,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.24.0"
 pydantic = "^2.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = { version = "^7.4.0", python = "^3.8" }
+pytest = { version = "^8.0.0", python = "^3.8" }
+pytest-md = "^0.2.0"
 
 
 [tool.pytest.ini_options]
 minversion = "7.0.0"
 testpaths = ["tests"]
```

### Comparing `paicorelib-1.0.0rc1/PKG-INFO` & `paicorelib-1.1.0rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: paicorelib
-Version: 1.0.0rc1
-Summary: Library of PAICORE 2.0.
+Version: 1.1.0rc1
+Summary: Library of PAICORE 2.0
 Home-page: https://github.com/PAICookers/PAIlib
 License: GPL-3.0-or-later
-Keywords: PAICORE 2.0,PAIBox,PAILib
+Keywords: PAICORE 2.0,PAICORE library,PAILib
 Author: Ziru Pan
 Author-email: zrpan@stu.pku.edu.cn
-Maintainer: Ziru Pan
-Maintainer-email: zrpan@stu.pku.edu.cn
+Maintainer: Hongtu Xia
+Maintainer-email: hongtux@pku.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -34,21 +34,21 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIlib/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paicorelib">
     </a>
-    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.0.0rc1">
-        <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?include_prereleases&color=orange">
+    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.1.0rc1">
+        <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIlib">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIlib/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIlib/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIlib/master.svg" alt="pre-commit.ci status">
     </a>
 
 </p>
 
-术语对照表：[Table of Terms](docs/Table-of-Terms.md)
+[Changelog](./CHANGELOG.md)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: paicorelib Version: 1.0.0rc1 Summary: Library of
-PAICORE 2.0. Home-page: https://github.com/PAICookers/PAIlib License: GPL-3.0-
-or-later Keywords: PAICORE 2.0,PAIBox,PAILib Author: Ziru Pan Author-email:
-zrpan@stu.pku.edu.cn Maintainer: Ziru Pan Maintainer-email:
-zrpan@stu.pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: Intended Audience
-:: Science/Research Classifier: License :: OSI Approved :: GNU General Public
+Metadata-Version: 2.1 Name: paicorelib Version: 1.1.0rc1 Summary: Library of
+PAICORE 2.0 Home-page: https://github.com/PAICookers/PAIlib License: GPL-3.0-
+or-later Keywords: PAICORE 2.0,PAICORE library,PAILib Author: Ziru Pan Author-
+email: zrpan@stu.pku.edu.cn Maintainer: Hongtu Xia Maintainer-email:
+hongtux@pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Libraries Requires-Dist: numpy (>=1.24.0,<2.0.0) Requires-Dist:
 pydantic (>=2.0,<3.0) Project-URL: Documentation, https://github.com/
 PAICookers/PAIlib#readme Project-URL: Repository, https://github.com/
 PAICookers/PAIlib Description-Content-Type: text/markdown
                            # Library of PAICORE 2.0
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_c_o_r_e_l_i_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
- _g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_?_i_n_c_l_u_d_e___p_r_e_r_e_l_e_a_s_e_s_&_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-
-                               _c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
-æ¯è¯­å¯¹ç§è¡¨ï¼[Table of Terms](docs/Table-of-Terms.md)
+   _g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_?_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+   _c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
+                                    _s_t_a_t_u_s_]
+[Changelog](./CHANGELOG.md)
```

