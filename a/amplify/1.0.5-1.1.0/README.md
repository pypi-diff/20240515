# Comparing `tmp/amplify-1.0.5-cp39-cp39-win_amd64.whl.zip` & `tmp/amplify-1.1.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 5452711 bytes, number of entries: 14
+Zip file size: 5772413 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat     1890 b- defN 24-Feb-20 03:48 amplify/__init__.py
--rw-rw-rw-  2.0 fat   236445 b- defN 24-Mar-19 09:08 amplify/__init__.pyi
--rw-rw-rw-  2.0 fat    16527 b- defN 24-Mar-19 08:55 amplify/_backward.py
--rw-rw-rw-  2.0 fat 17304576 b- defN 24-Mar-19 09:08 amplify/amplify.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      334 b- defN 24-Mar-19 09:08 amplify/amplify.cp39-win_amd64.pyd.manifest
+-rw-rw-rw-  2.0 fat   248086 b- defN 24-May-14 13:46 amplify/__init__.pyi
+-rw-rw-rw-  2.0 fat    16848 b- defN 24-Mar-28 08:00 amplify/_backward.py
+-rw-rw-rw-  2.0 fat 18060288 b- defN 24-May-14 13:46 amplify/amplify.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     2564 b- defN 24-Feb-20 03:48 amplify/constraint.py
--rw-rw-rw-  2.0 fat     4375 b- defN 24-Mar-19 08:55 amplify/client/__init__.py
--rw-rw-rw-  2.0 fat      671 b- defN 24-Mar-19 08:55 amplify/client/ocean.py
--rw-rw-rw-  2.0 fat    19518 b- defN 24-Mar-19 09:08 amplify-1.0.5.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    26622 b- defN 24-Mar-19 09:08 amplify-1.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Mar-19 09:08 amplify-1.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat    24247 b- defN 24-Mar-19 09:08 amplify-1.0.5.dist-info/open_source_license.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-Mar-19 09:05 amplify-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1164 b- defN 24-Mar-19 09:08 amplify-1.0.5.dist-info/RECORD
-14 files, 17639041 bytes uncompressed, 5450793 bytes compressed:  69.1%
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-14 13:46 amplify/py.typed
+-rw-rw-rw-  2.0 fat     4397 b- defN 24-May-09 05:53 amplify/client/__init__.py
+-rw-rw-rw-  2.0 fat      672 b- defN 24-Mar-28 08:00 amplify/client/ocean.py
+-rw-rw-rw-  2.0 fat    19518 b- defN 24-May-14 13:46 amplify-1.1.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    26624 b- defN 24-May-14 13:46 amplify-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-14 13:46 amplify-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat    24247 b- defN 24-May-14 13:46 amplify-1.1.0.dist-info/open_source_license.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-14 13:43 amplify-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1135 b- defN 24-May-14 13:46 amplify-1.1.0.dist-info/RECORD
+14 files, 18406377 bytes uncompressed, 5770549 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -6,38 +6,38 @@
 
 Filename: amplify/_backward.py
 Comment: 
 
 Filename: amplify/amplify.cp39-win_amd64.pyd
 Comment: 
 
-Filename: amplify/amplify.cp39-win_amd64.pyd.manifest
+Filename: amplify/constraint.py
 Comment: 
 
-Filename: amplify/constraint.py
+Filename: amplify/py.typed
 Comment: 
 
 Filename: amplify/client/__init__.py
 Comment: 
 
 Filename: amplify/client/ocean.py
 Comment: 
 
-Filename: amplify-1.0.5.dist-info/LICENSE.txt
+Filename: amplify-1.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: amplify-1.0.5.dist-info/METADATA
+Filename: amplify-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: amplify-1.0.5.dist-info/WHEEL
+Filename: amplify-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: amplify-1.0.5.dist-info/open_source_license.txt
+Filename: amplify-1.1.0.dist-info/open_source_license.txt
 Comment: 
 
-Filename: amplify-1.0.5.dist-info/top_level.txt
+Filename: amplify-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: amplify-1.0.5.dist-info/RECORD
+Filename: amplify-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## amplify/__init__.pyi

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Callable, Iterable, Iterator, Sequence
 from typing import Any, ClassVar, Generic, Literal, Optional, TypeVar, Union
 
-from typing_extensions import TypeAlias
+from typing_extensions import TypeAlias, Unpack
 
 from ._backward import *  # noqa: F403
 
 EllipsisType = type(...)
 import datetime
 import os
 from typing import overload
@@ -24,24 +24,26 @@
     FixstarsClient,
     DWaveSamplerClient,
     LeapHybridSamplerClient,
     LeapHybridCQMSamplerClient,
     FujitsuDA4Client,
     ToshibaSQBM2Client,
     GurobiClient,
+    NECVA2Client,
     Literal[None],
 )
-type AmplifyClient = Union[
+AmplifyClient: TypeAlias = Union[
     FixstarsClient,
     DWaveSamplerClient,
     LeapHybridSamplerClient,
     LeapHybridCQMSamplerClient,
     FujitsuDA4Client,
     ToshibaSQBM2Client,
     GurobiClient,
+    NECVA2Client,
 ]
 
 class _ClientResultDescriptor:
     @overload
     def __get__(self, instance: Result[FixstarsClient], owner: Any) -> FixstarsClient.Result: ...
     @overload
     def __get__(self, instance: Result[DWaveSamplerClient], owner: Any) -> dimod.sampleset.SampleSet: ...
@@ -52,24 +54,27 @@
     @overload
     def __get__(self, instance: Result[FujitsuDA4Client], owner: Any) -> FujitsuDA4Client.Result: ...
     @overload
     def __get__(self, instance: Result[ToshibaSQBM2Client], owner: Any) -> ToshibaSQBM2Client.Result: ...
     @overload
     def __get__(self, instance: Result[GurobiClient], owner: Any) -> GurobiClient.Result: ...
     @overload
+    def __get__(self, instance: Result[NECVA2Client], owner: Any) -> NECVA2Client.Result: ...
+    @overload
     def __get__(self, instance: Result[Literal[None]], owner: Any) -> None: ...
     @overload
     def __get__(
         self, instance: Any, owner: Any
     ) -> Union[
         FixstarsClient.Result,
         dimod.sampleset.SampleSet,
         FujitsuDA4Client.Result,
         ToshibaSQBM2Client.Result,
         GurobiClient.Result,
+        NECVA2Client.Result,
         None,
     ]: ...
 
 class _EmbeddingDescriptor:
     @overload
     def __get__(
         self,
@@ -89,17 +94,17 @@
         objective: dict[Union[VariableType, str], Union[Degree, str]] = ...,
         equality_constraints: dict[Union[VariableType, str], Union[Degree, str]] = ...,
         inequality_constraints: dict[Union[VariableType, str], Union[Degree, str]] = ...,
     ) -> None:
         """__init__
 
         Args:
-            objective (dict[Union[amplify.VariableType, str], Union[amplify.Degree, str]]): Defaults to ``{Binary: Zero, Ising: Zero, Integer: Zero, Real: Zero}``.
-            equality_constraints (dict[Union[amplify.VariableType, str], Union[amplify.Degree, str]]): Defaults to ``{Binary: Zero, Ising: Zero, Integer: Zero, Real: Zero}``.
-            inequality_constraints (dict[Union[amplify.VariableType, str], Union[amplify.Degree, str]]): Defaults to ``{Binary: Zero, Ising: Zero, Integer: Zero, Real: Zero}``.
+            objective (dict[Union[amplify.VariableType, str], Union[amplify.Degree, str]]): Defaults to ``{VariableType.Binary: Degree.Zero, VariableType.Ising: Degree.Zero, VariableType.Integer: Degree.Zero, VariableType.Real: Degree.Zero}``.
+            equality_constraints (dict[Union[amplify.VariableType, str], Union[amplify.Degree, str]]): Defaults to ``{VariableType.Binary: Degree.Zero, VariableType.Ising: Degree.Zero, VariableType.Integer: Degree.Zero, VariableType.Real: Degree.Zero}``.
+            inequality_constraints (dict[Union[amplify.VariableType, str], Union[amplify.Degree, str]]): Defaults to ``{VariableType.Binary: Degree.Zero, VariableType.Ising: Degree.Zero, VariableType.Integer: Degree.Zero, VariableType.Real: Degree.Zero}``.
         """
     @property
     def equality_constraints(self) -> dict[VariableType, Degree]:
         """equality_constraints property
 
         Returns:
             dict[amplify.VariableType, amplify.Degree]:
@@ -758,17 +763,19 @@
         """version property
 
         Returns:
             str:
         """
 
 class Degree:
+    Cubic: ClassVar[Degree] = ...
     HighOrder: ClassVar[Degree] = ...
     Linear: ClassVar[Degree] = ...
     Quadratic: ClassVar[Degree] = ...
+    Quartic: ClassVar[Degree] = ...
     Zero: ClassVar[Degree] = ...
     __name__: Any
     def __init__(self, *args, **kwargs) -> None: ...
     def __eq__(self, other) -> bool: ...
     def __ge__(self, other) -> bool: ...
     def __gt__(self, other) -> bool: ...
     def __hash__(self) -> int: ...
@@ -876,15 +883,15 @@
         def outputs(self) -> FixstarsClient.Parameters.Outputs:
             """outputs property
 
             Returns:
                 amplify.FixstarsClient.Parameters.Outputs:
             """
 
-    class Result(Generic[_AmplifyClient]):
+    class Result:
         class ExecutionParameters:
             def __init__(self, *args, **kwargs) -> None: ...
             def _repr_pretty_(self, arg0: Any, arg1: bool) -> None:
                 """_repr_pretty_
 
                 Args:
                     arg0 (Any):
@@ -1505,15 +1512,15 @@
         def timing(self) -> FujitsuDA4Client.SolverTiming:
             """timing property
 
             Returns:
                 amplify.FujitsuDA4Client.SolverTiming:
             """
 
-    class Result(Generic[_AmplifyClient]):
+    class Result:
         def __init__(self, *args, **kwargs) -> None: ...
         def _repr_pretty_(self, arg0: Any, arg1: bool) -> None:
             """_repr_pretty_
 
             Args:
                 arg0 (Any):
                 arg1 (bool):
@@ -3013,15 +3020,15 @@
             """_repr_pretty_
 
             Args:
                 arg0 (Any):
                 arg1 (bool):
             """
 
-    class Result(Generic[_AmplifyClient]):
+    class Result:
         class OptimizationStatusCode:
             Cutoff: ClassVar[GurobiClient.Result.OptimizationStatusCode] = ...
             InfOrUnbd: ClassVar[GurobiClient.Result.OptimizationStatusCode] = ...
             Infeasible: ClassVar[GurobiClient.Result.OptimizationStatusCode] = ...
             Inprogress: ClassVar[GurobiClient.Result.OptimizationStatusCode] = ...
             Interrupted: ClassVar[GurobiClient.Result.OptimizationStatusCode] = ...
             IterationLimit: ClassVar[GurobiClient.Result.OptimizationStatusCode] = ...
@@ -3917,14 +3924,385 @@
     def variables(self) -> list[Variable]:
         """alias of `~amplify.Model.get_variables`
 
         Returns:
             list[amplify.Variable]:
         """
 
+class NECVA2Client:
+    class Parameters:
+        beta_list: Optional[list[float]]
+        """beta_list property
+
+        Returns:
+            list[float] | None:
+        """
+        beta_range: Optional[tuple[float, float]]
+        """beta_range property
+
+        Returns:
+            tuple[float, float, int] | None:
+        """
+        dense: Optional[bool]
+        """dense property
+
+        Returns:
+            bool | None:
+        """
+        num_reads: Optional[int]
+        """num_reads property
+
+        Returns:
+            int | None:
+        """
+        num_results: Optional[int]
+        """num_results property
+
+        Returns:
+            int | None:
+        """
+        num_sweeps: Optional[int]
+        """num_sweeps property
+
+        Returns:
+            int | None:
+        """
+        @property
+        def timeout(self) -> Optional[datetime.timedelta]:
+            """timeout property
+
+            Returns:
+                datetime.timedelta | None:
+            """
+        @timeout.setter
+        def timeout(self, value: Union[Optional[datetime.timedelta], int]) -> None: ...
+        ve_num: Optional[int]
+        """ve_num property
+
+        Returns:
+            int | None:
+        """
+        @property
+        def vector_mode(self) -> Optional[NECVA2Client.VectorMode]:
+            """vector_mode property
+
+            Returns:
+                amplify.NECVA2Client.VectorMode | None:
+            """
+        @vector_mode.setter
+        def vector_mode(
+            self, value: Union[Optional[NECVA2Client.VectorMode], Literal["speed", "accuracy"]]
+        ) -> None: ...
+        def __init__(self, *args, **kwargs) -> None: ...
+        def _repr_pretty_(self, arg0: Any, arg1: bool) -> None:
+            """_repr_pretty_
+
+            Args:
+                arg0 (Any):
+                arg1 (bool):
+            """
+
+    class Result:
+        class Result:
+            def __init__(self, *args, **kwargs) -> None: ...
+            def _repr_pretty_(self, arg0: Any, arg1: bool) -> None:
+                """_repr_pretty_
+
+                Args:
+                    arg0 (Any):
+                    arg1 (bool):
+                """
+            @property
+            def constraint(self) -> bool:
+                """constraint property
+
+                Returns:
+                    bool:
+                """
+            @property
+            def energy(self) -> float:
+                """energy property
+
+                Returns:
+                    float:
+                """
+            @property
+            def memory_usage(self) -> float:
+                """memory_usage property
+
+                Returns:
+                    float:
+                """
+            @property
+            def spin(self) -> dict[str, int]:
+                """spin property
+
+                Returns:
+                    dict[str, int]:
+                """
+            @property
+            def time(self) -> datetime.timedelta:
+                """time property
+
+                Returns:
+                    datetime.timedelta:
+                """
+
+        class Timing:
+            def __init__(self, *args, **kwargs) -> None: ...
+            def _repr_pretty_(self, arg0: Any, arg1: bool) -> None:
+                """_repr_pretty_
+
+                Args:
+                    arg0 (Any):
+                    arg1 (bool):
+                """
+            @property
+            def execution_time(self) -> datetime.timedelta:
+                """execution_time property
+
+                Returns:
+                    datetime.timedelta:
+                """
+            @property
+            def solve_qubo_time(self) -> datetime.timedelta:
+                """solve_qubo_time property
+
+                Returns:
+                    datetime.timedelta:
+                """
+
+        def __init__(self, *args, **kwargs) -> None: ...
+        def _repr_pretty_(self, arg0: Any, arg1: bool) -> None:
+            """_repr_pretty_
+
+            Args:
+                arg0 (Any):
+                arg1 (bool):
+            """
+        @property
+        def result(self) -> list[NECVA2Client.Result.Result]:
+            """result property
+
+            Returns:
+                list[amplify.NECVA2Client.Result.Result]:
+            """
+        @property
+        def timing(self) -> NECVA2Client.Result.Timing:
+            """timing property
+
+            Returns:
+                amplify.NECVA2Client.Result.Timing:
+            """
+
+    class VectorMode:
+        Accuracy: ClassVar[NECVA2Client.VectorMode] = ...
+        Speed: ClassVar[NECVA2Client.VectorMode] = ...
+        __name__: Any
+        def __init__(self, *args, **kwargs) -> None: ...
+        def __eq__(self, other) -> bool: ...
+        def __ge__(self, other) -> bool: ...
+        def __gt__(self, other) -> bool: ...
+        def __hash__(self) -> int: ...
+        def __index__(self) -> Any: ...
+        def __int__(self) -> int: ...
+        def __le__(self, other) -> bool: ...
+        def __lt__(self, other) -> bool: ...
+        def __ne__(self, other) -> bool: ...
+
+    proxy: Optional[str]
+    """proxy property
+
+    Returns:
+        str | None:
+    """
+    set_andzero: bool
+    """set_andzero property
+
+    Returns:
+        bool:
+    """
+    set_fixed: bool
+    """set_fixed property
+
+    Returns:
+        bool:
+    """
+    set_maxone: bool
+    """set_maxone property
+
+    Returns:
+        bool:
+    """
+    set_minmaxone: bool
+    """set_minmaxone property
+
+    Returns:
+        bool:
+    """
+    set_onehot: bool
+    """set_onehot property
+
+    Returns:
+        bool:
+    """
+    set_orone: bool
+    """set_orone property
+
+    Returns:
+        bool:
+    """
+    set_supplement: bool
+    """set_supplement property
+
+    Returns:
+        bool:
+    """
+    token: str
+    """token property
+
+    Returns:
+        str:
+    """
+    url: str
+    """url property
+
+    Returns:
+        str:
+    """
+    @property
+    def write_request_data(self) -> Optional[os.PathLike]:
+        """write_request_data property
+
+        Returns:
+            os.PathLike | None:
+        """
+    @write_request_data.setter
+    def write_request_data(self, value: Union[Optional[os.PathLike], str]) -> None: ...
+    @property
+    def write_response_data(self) -> Optional[os.PathLike]:
+        """write_response_data property
+
+        Returns:
+            os.PathLike | None:
+        """
+    @write_response_data.setter
+    def write_response_data(self, value: Union[Optional[os.PathLike], str]) -> None: ...
+    @overload
+    def __init__(self) -> None: ...
+    @overload
+    def __init__(self, token: str = ..., url: str = ..., proxy: Optional[str] = ...) -> None:
+        """__init__
+
+        Args:
+            token (str): Defaults to ``''``.
+            url (str): Defaults to ``''``.
+            proxy (str | None): Defaults to ``None``.
+        """
+    def _repr_pretty_(self, arg0: Any, arg1: bool) -> None:
+        """_repr_pretty_
+
+        Args:
+            arg0 (Any):
+            arg1 (bool):
+        """
+    @overload
+    def solve(self, objective: Union[Poly, Matrix], dry_run: Literal[False] = ...) -> NECVA2Client.Result: ...
+    @overload
+    def solve(
+        self, constraint: Union[Constraint, ConstraintList], dry_run: Literal[False] = ...
+    ) -> NECVA2Client.Result: ...
+    @overload
+    def solve(
+        self,
+        objective: Union[Poly, Matrix],
+        constraint: Union[Constraint, ConstraintList],
+        dry_run: Literal[False] = ...,
+    ) -> NECVA2Client.Result: ...
+    @overload
+    def solve(self, objective: Union[Poly, Matrix], dry_run: Literal[True]) -> None: ...
+    @overload
+    def solve(self, constraint: Union[Constraint, ConstraintList], dry_run: Literal[True]) -> None: ...
+    @overload
+    def solve(
+        self, objective: Union[Poly, Matrix], constraint: Union[Constraint, ConstraintList], dry_run: Literal[True]
+    ) -> None:
+        """solve
+
+        :Overloading:
+
+        .. admonition:: 1. solve(self, objective: Union[amplify.Poly, amplify.Matrix], dry_run: Literal[False] = False) -> amplify.NECVA2Client.Result
+
+            Args:
+                * objective (amplify.Poly | amplify.Matrix):
+                * dry_run (Literal[False]): Defaults to ``False``.
+
+            Returns:
+                amplify.NECVA2Client.Result:
+
+        .. admonition:: 2. solve(self, constraint: Union[amplify.Constraint, amplify.ConstraintList], dry_run: Literal[False] = False) -> amplify.NECVA2Client.Result
+
+            Args:
+                * constraint (amplify.Constraint | amplify.ConstraintList):
+                * dry_run (Literal[False]): Defaults to ``False``.
+
+            Returns:
+                amplify.NECVA2Client.Result:
+
+        .. admonition:: 3. solve(self, objective: Union[amplify.Poly, amplify.Matrix], constraint: Union[amplify.Constraint, amplify.ConstraintList], dry_run: Literal[False] = False) -> amplify.NECVA2Client.Result
+
+            Args:
+                * objective (amplify.Poly | amplify.Matrix):
+                * constraint (amplify.Constraint | amplify.ConstraintList):
+                * dry_run (Literal[False]): Defaults to ``False``.
+
+            Returns:
+                amplify.NECVA2Client.Result:
+
+        .. admonition:: 4. solve(self, objective: Union[amplify.Poly, amplify.Matrix], dry_run: Literal[True]) -> None
+
+            Args:
+                * objective (amplify.Poly | amplify.Matrix):
+                * dry_run (Literal[True]):
+
+        .. admonition:: 5. solve(self, constraint: Union[amplify.Constraint, amplify.ConstraintList], dry_run: Literal[True]) -> None
+
+            Args:
+                * constraint (amplify.Constraint | amplify.ConstraintList):
+                * dry_run (Literal[True]):
+
+        .. admonition:: 6. solve(self, objective: Union[amplify.Poly, amplify.Matrix], constraint: Union[amplify.Constraint, amplify.ConstraintList], dry_run: Literal[True]) -> None
+
+            Args:
+                * objective (amplify.Poly | amplify.Matrix):
+                * constraint (amplify.Constraint | amplify.ConstraintList):
+                * dry_run (Literal[True]):
+        """
+    @property
+    def acceptable_degrees(self) -> AcceptableDegrees:
+        """acceptable_degrees property
+
+        Returns:
+            amplify.AcceptableDegrees:
+        """
+    @property
+    def parameters(self) -> NECVA2Client.Parameters:
+        """parameters property
+
+        Returns:
+            amplify.NECVA2Client.Parameters:
+        """
+    @property
+    def version(self) -> str:
+        """version property
+
+        Returns:
+            str:
+        """
+
 class PenaltyFormulation:
     Default: ClassVar[PenaltyFormulation] = ...
     IntegerVariable: ClassVar[PenaltyFormulation] = ...
     LinearRelaxation: ClassVar[PenaltyFormulation] = ...
     QuadraticRelaxation: ClassVar[PenaltyFormulation] = ...
     RealVariable: ClassVar[PenaltyFormulation] = ...
     Relaxation: ClassVar[PenaltyFormulation] = ...
@@ -5981,15 +6359,15 @@
         Returns:
             amplify.Result.Solution:
         """
     client_result: _ClientResultDescriptor
     """client_result property
 
     Returns:
-        amplify.FixstarsClient.Result | dimod.sampleset.SampleSet | amplify.FujitsuDA4Client.Result | amplify.ToshibaSQBM2Client.Result | amplify.GurobiClient.Result | None:
+        amplify.FixstarsClient.Result | dimod.sampleset.SampleSet | amplify.FujitsuDA4Client.Result | amplify.ToshibaSQBM2Client.Result | amplify.GurobiClient.Result | amplify.NECVA2Client.Result | None:
     """
 
     embedding: _EmbeddingDescriptor
     """embedding property
 
     Returns:
         amplify.Result.GraphConversion | None:
@@ -6689,29 +7067,31 @@
         type: Union[Literal["Binary", "Integer", "Ising", "Real"], VariableType],
         shape: Union[tuple[int, ...], int],
         bounds: tuple[Optional[float], ...] = ...,
         name: str = ...,
     ) -> PolyArray: ...
     @overload
     def array(
-        self, type: Union[Literal["Binary", "Integer", "Ising", "Real"], VariableType], *shape: *tuple[int]
+        self, type: Union[Literal["Binary", "Integer", "Ising", "Real"], VariableType], *shape: Unpack[tuple[int]]
     ) -> PolyArray[_Dim1]: ...
     @overload
     def array(
-        self, type: Union[Literal["Binary", "Integer", "Ising", "Real"], VariableType], *shape: *tuple[int, int]
+        self, type: Union[Literal["Binary", "Integer", "Ising", "Real"], VariableType], *shape: Unpack[tuple[int, int]]
     ) -> PolyArray[_Dim2]: ...
     @overload
     def array(
-        self, type: Union[Literal["Binary", "Integer", "Ising", "Real"], VariableType], *shape: *tuple[int, int, int]
+        self,
+        type: Union[Literal["Binary", "Integer", "Ising", "Real"], VariableType],
+        *shape: Unpack[tuple[int, int, int]],
     ) -> PolyArray[_Dim3]: ...
     @overload
     def array(
         self,
         type: Union[Literal["Binary", "Integer", "Ising", "Real"], VariableType],
-        *shape: *tuple[int, int, int, int],
+        *shape: Unpack[tuple[int, int, int, int]],
     ) -> PolyArray[_Dim4]: ...
     @overload
     def array(self, type: Union[Literal["Binary", "Integer", "Ising", "Real"], VariableType], *shape: int) -> PolyArray:
         """array
 
         :Overloading:
 
@@ -7617,19 +7997,19 @@
     sort_solution: Union[bool, list[bool]] = ...,
     concurrency: int = ...,
 ) -> list[Optional[Result]]:
     """parallel_solve
 
     :Overloading:
 
-    .. admonition:: 1. parallel_solve(model: Union[amplify.Model, list[amplify.Model]], client: Union[Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient], list[Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient]]], integer_encoding_method: Union[str, amplify.IntegerEncodingMethod, list[Union[str, amplify.IntegerEncodingMethod]]] = Default, quadratization_method: Union[str, amplify.QuadratizationMethod, list[Union[str, amplify.QuadratizationMethod]]] = IshikawaKZFD, substitution_multiplier: Union[float, list[float]] = 1.0, embedding_method: Union[str, amplify.EmbeddingMethod, list[Union[str, amplify.EmbeddingMethod]]] = Default, embedding_timeout: Union[float, datetime.timedelta, list[Union[float, datetime.timedelta]]] = 10.0, chain_strength: Union[float, list[float]] = 1.0, dry_run: Union[bool, list[bool]] = False, num_solves: Union[int, list[int]] = 1, filter_solution: Union[bool, list[bool]] = True, sort_solution: Union[bool, list[bool]] = True, concurrency: int = 0) -> list[Optional[amplify.Result]]
+    .. admonition:: 1. parallel_solve(model: Union[amplify.Model, list[amplify.Model]], client: Union[Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient, amplify.NECVA2Client], list[Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient, amplify.NECVA2Client]]], integer_encoding_method: Union[str, amplify.IntegerEncodingMethod, list[Union[str, amplify.IntegerEncodingMethod]]] = Default, quadratization_method: Union[str, amplify.QuadratizationMethod, list[Union[str, amplify.QuadratizationMethod]]] = IshikawaKZFD, substitution_multiplier: Union[float, list[float]] = 1.0, embedding_method: Union[str, amplify.EmbeddingMethod, list[Union[str, amplify.EmbeddingMethod]]] = Default, embedding_timeout: Union[float, datetime.timedelta, list[Union[float, datetime.timedelta]]] = 10.0, chain_strength: Union[float, list[float]] = 1.0, dry_run: Union[bool, list[bool]] = False, num_solves: Union[int, list[int]] = 1, filter_solution: Union[bool, list[bool]] = True, sort_solution: Union[bool, list[bool]] = True, concurrency: int = 0) -> list[Optional[amplify.Result]]
 
         Args:
             * model (amplify.Model | list[amplify.Model]):
-            * client (amplify.FixstarsClient | amplify.DWaveSamplerClient | amplify.LeapHybridSamplerClient | amplify.LeapHybridCQMSamplerClient | amplify.FujitsuDA4Client | amplify.ToshibaSQBM2Client | amplify.GurobiClient | list[Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient]]):
+            * client (amplify.FixstarsClient | amplify.DWaveSamplerClient | amplify.LeapHybridSamplerClient | amplify.LeapHybridCQMSamplerClient | amplify.FujitsuDA4Client | amplify.ToshibaSQBM2Client | amplify.GurobiClient | amplify.NECVA2Client | list[Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient, amplify.NECVA2Client]]):
             * integer_encoding_method (str | amplify.IntegerEncodingMethod | list[Union[str, amplify.IntegerEncodingMethod]]): Defaults to ``Default``.
             * quadratization_method (str | amplify.QuadratizationMethod | list[Union[str, amplify.QuadratizationMethod]]): Defaults to ``IshikawaKZFD``.
             * substitution_multiplier (float | list[float]): Defaults to ``1.0``.
             * embedding_method (str | amplify.EmbeddingMethod | list[Union[str, amplify.EmbeddingMethod]]): Defaults to ``Default``.
             * embedding_timeout (float | datetime.timedelta | list[Union[float, datetime.timedelta]]): Defaults to ``10.0``.
             * chain_strength (float | list[float]): Defaults to ``1.0``.
             * dry_run (bool | list[bool]): Defaults to ``False``.
@@ -7637,19 +8017,19 @@
             * filter_solution (bool | list[bool]): Defaults to ``True``.
             * sort_solution (bool | list[bool]): Defaults to ``True``.
             * concurrency (int): Defaults to ``0``.
 
         Returns:
             list[Optional[amplify.Result]]:
 
-    .. admonition:: 2. parallel_solve(model: Union[Union[amplify.Poly, amplify.Matrix, amplify.Constraint, amplify.ConstraintList], list[Union[amplify.Poly, amplify.Matrix, amplify.Constraint, amplify.ConstraintList]]], client: Union[Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient], list[Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient]]], integer_encoding_method: Union[str, amplify.IntegerEncodingMethod, list[Union[str, amplify.IntegerEncodingMethod]]] = Default, quadratization_method: Union[str, amplify.QuadratizationMethod, list[Union[str, amplify.QuadratizationMethod]]] = IshikawaKZFD, substitution_multiplier: Union[float, list[float]] = 1.0, embedding_method: Union[str, amplify.EmbeddingMethod, list[Union[str, amplify.EmbeddingMethod]]] = Default, embedding_timeout: Union[float, datetime.timedelta, list[Union[float, datetime.timedelta]]] = 10.0, chain_strength: Union[float, list[float]] = 1.0, dry_run: Union[bool, list[bool]] = False, num_solves: Union[int, list[int]] = 1, filter_solution: Union[bool, list[bool]] = True, sort_solution: Union[bool, list[bool]] = True, concurrency: int = 0) -> list[Optional[amplify.Result]]
+    .. admonition:: 2. parallel_solve(model: Union[Union[amplify.Poly, amplify.Matrix, amplify.Constraint, amplify.ConstraintList], list[Union[amplify.Poly, amplify.Matrix, amplify.Constraint, amplify.ConstraintList]]], client: Union[Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient, amplify.NECVA2Client], list[Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient, amplify.NECVA2Client]]], integer_encoding_method: Union[str, amplify.IntegerEncodingMethod, list[Union[str, amplify.IntegerEncodingMethod]]] = Default, quadratization_method: Union[str, amplify.QuadratizationMethod, list[Union[str, amplify.QuadratizationMethod]]] = IshikawaKZFD, substitution_multiplier: Union[float, list[float]] = 1.0, embedding_method: Union[str, amplify.EmbeddingMethod, list[Union[str, amplify.EmbeddingMethod]]] = Default, embedding_timeout: Union[float, datetime.timedelta, list[Union[float, datetime.timedelta]]] = 10.0, chain_strength: Union[float, list[float]] = 1.0, dry_run: Union[bool, list[bool]] = False, num_solves: Union[int, list[int]] = 1, filter_solution: Union[bool, list[bool]] = True, sort_solution: Union[bool, list[bool]] = True, concurrency: int = 0) -> list[Optional[amplify.Result]]
 
         Args:
             * model (amplify.Poly | amplify.Matrix | amplify.Constraint | amplify.ConstraintList | list[Union[amplify.Poly, amplify.Matrix, amplify.Constraint, amplify.ConstraintList]]):
-            * client (amplify.FixstarsClient | amplify.DWaveSamplerClient | amplify.LeapHybridSamplerClient | amplify.LeapHybridCQMSamplerClient | amplify.FujitsuDA4Client | amplify.ToshibaSQBM2Client | amplify.GurobiClient | list[Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient]]):
+            * client (amplify.FixstarsClient | amplify.DWaveSamplerClient | amplify.LeapHybridSamplerClient | amplify.LeapHybridCQMSamplerClient | amplify.FujitsuDA4Client | amplify.ToshibaSQBM2Client | amplify.GurobiClient | amplify.NECVA2Client | list[Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient, amplify.NECVA2Client]]):
             * integer_encoding_method (str | amplify.IntegerEncodingMethod | list[Union[str, amplify.IntegerEncodingMethod]]): Defaults to ``Default``.
             * quadratization_method (str | amplify.QuadratizationMethod | list[Union[str, amplify.QuadratizationMethod]]): Defaults to ``IshikawaKZFD``.
             * substitution_multiplier (float | list[float]): Defaults to ``1.0``.
             * embedding_method (str | amplify.EmbeddingMethod | list[Union[str, amplify.EmbeddingMethod]]): Defaults to ``Default``.
             * embedding_timeout (float | datetime.timedelta | list[Union[float, datetime.timedelta]]): Defaults to ``10.0``.
             * chain_strength (float | list[float]): Defaults to ``1.0``.
             * dry_run (bool | list[bool]): Defaults to ``False``.
@@ -7668,90 +8048,90 @@
     Args:
         arg (int):
     """
 
 @overload
 def solve(
     model: Model,
-    client: _AmplifyClient,
+    client: AmplifyClient,
     integer_encoding_method: Union[Literal["Unary", "Linear", "Binary", "Default"], IntegerEncodingMethod] = ...,
     quadratization_method: Union[Literal["IshikawaKZFD", "Substitute"], QuadratizationMethod] = ...,
     substitution_multiplier: float = ...,
     embedding_method: Union[Literal["Default", "Clique", "Minor", "Parallel"], EmbeddingMethod] = ...,
     embedding_timeout: Union[float, datetime.timedelta] = ...,
     chain_strength: float = ...,
     dry_run: Literal[False] = ...,
     num_solves: int = ...,
     filter_solution: bool = ...,
     sort_solution: bool = ...,
 ) -> Result[_AmplifyClient]: ...
 @overload
 def solve(
     model: Model,
-    client: _AmplifyClient,
+    client: AmplifyClient,
     integer_encoding_method: Union[Literal["Unary", "Linear", "Binary", "Default"], IntegerEncodingMethod] = ...,
     quadratization_method: Union[Literal["IshikawaKZFD", "Substitute"], QuadratizationMethod] = ...,
     substitution_multiplier: float = ...,
     embedding_method: Union[Literal["Default", "Clique", "Minor", "Parallel"], EmbeddingMethod] = ...,
     embedding_timeout: Union[float, datetime.timedelta] = ...,
     chain_strength: float = ...,
     dry_run: Literal[True] = ...,
     num_solves: int = ...,
     filter_solution: bool = ...,
     sort_solution: bool = ...,
 ) -> Result[Literal[None]]: ...
 @overload
 def solve(
     model: Model,
-    client: _AmplifyClient,
+    client: AmplifyClient,
     integer_encoding_method: Union[Literal["Unary", "Linear", "Binary", "Default"], IntegerEncodingMethod] = ...,
     quadratization_method: Union[Literal["IshikawaKZFD", "Substitute"], QuadratizationMethod] = ...,
     substitution_multiplier: float = ...,
     embedding_method: Union[Literal["Default", "Clique", "Minor", "Parallel"], EmbeddingMethod] = ...,
     embedding_timeout: Union[float, datetime.timedelta] = ...,
     chain_strength: float = ...,
     dry_run: bool = ...,
     num_solves: int = ...,
     filter_solution: bool = ...,
     sort_solution: bool = ...,
 ) -> Union[Result[_AmplifyClient], Result[Literal[None]]]: ...
 @overload
 def solve(
     model: Union[Poly, Matrix, Constraint, ConstraintList],
-    client: _AmplifyClient,
+    client: AmplifyClient,
     integer_encoding_method: Union[Literal["Unary", "Linear", "Binary", "Default"], IntegerEncodingMethod] = ...,
     quadratization_method: Union[Literal["IshikawaKZFD", "Substitute"], QuadratizationMethod] = ...,
     substitution_multiplier: float = ...,
     embedding_method: Union[Literal["Default", "Clique", "Minor", "Parallel"], EmbeddingMethod] = ...,
     embedding_timeout: Union[float, datetime.timedelta] = ...,
     chain_strength: float = ...,
     dry_run: Literal[False] = ...,
     num_solves: int = ...,
     filter_solution: bool = ...,
     sort_solution: bool = ...,
 ) -> Result[_AmplifyClient]: ...
 @overload
 def solve(
     model: Union[Poly, Matrix, Constraint, ConstraintList],
-    client: _AmplifyClient,
+    client: AmplifyClient,
     integer_encoding_method: Union[Literal["Unary", "Linear", "Binary", "Default"], IntegerEncodingMethod] = ...,
     quadratization_method: Union[Literal["IshikawaKZFD", "Substitute"], QuadratizationMethod] = ...,
     substitution_multiplier: float = ...,
     embedding_method: Union[Literal["Default", "Clique", "Minor", "Parallel"], EmbeddingMethod] = ...,
     embedding_timeout: Union[float, datetime.timedelta] = ...,
     chain_strength: float = ...,
     dry_run: Literal[True] = ...,
     num_solves: int = ...,
     filter_solution: bool = ...,
     sort_solution: bool = ...,
 ) -> Result[Literal[None]]: ...
 @overload
 def solve(
     model: Union[Poly, Matrix, Constraint, ConstraintList],
-    client: _AmplifyClient,
+    client: AmplifyClient,
     integer_encoding_method: Union[Literal["Unary", "Linear", "Binary", "Default"], IntegerEncodingMethod] = ...,
     quadratization_method: Union[Literal["IshikawaKZFD", "Substitute"], QuadratizationMethod] = ...,
     substitution_multiplier: float = ...,
     embedding_method: Union[Literal["Default", "Clique", "Minor", "Parallel"], EmbeddingMethod] = ...,
     embedding_timeout: Union[float, datetime.timedelta] = ...,
     chain_strength: float = ...,
     dry_run: bool = ...,
@@ -7759,38 +8139,38 @@
     filter_solution: bool = ...,
     sort_solution: bool = ...,
 ) -> Union[Result[_AmplifyClient], Result[Literal[None]]]:
     """solve
 
     :Overloading:
 
-    .. admonition:: 1. solve(model: amplify.Model, client: Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient], integer_encoding_method: Union[str, amplify.IntegerEncodingMethod] = Default, quadratization_method: Union[str, amplify.QuadratizationMethod] = IshikawaKZFD, substitution_multiplier: float = 1.0, embedding_method: Union[str, amplify.EmbeddingMethod] = Default, embedding_timeout: Union[float, datetime.timedelta] = 10.0, chain_strength: float = 1.0, dry_run: bool = False, num_solves: int = 1, filter_solution: bool = True, sort_solution: bool = True) -> amplify.Result
+    .. admonition:: 1. solve(model: amplify.Model, client: Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient, amplify.NECVA2Client], integer_encoding_method: Union[str, amplify.IntegerEncodingMethod] = Default, quadratization_method: Union[str, amplify.QuadratizationMethod] = IshikawaKZFD, substitution_multiplier: float = 1.0, embedding_method: Union[str, amplify.EmbeddingMethod] = Default, embedding_timeout: Union[float, datetime.timedelta] = 10.0, chain_strength: float = 1.0, dry_run: bool = False, num_solves: int = 1, filter_solution: bool = True, sort_solution: bool = True) -> amplify.Result
 
         Args:
             * model (amplify.Model):
-            * client (amplify.FixstarsClient | amplify.DWaveSamplerClient | amplify.LeapHybridSamplerClient | amplify.LeapHybridCQMSamplerClient | amplify.FujitsuDA4Client | amplify.ToshibaSQBM2Client | amplify.GurobiClient):
+            * client (amplify.FixstarsClient | amplify.DWaveSamplerClient | amplify.LeapHybridSamplerClient | amplify.LeapHybridCQMSamplerClient | amplify.FujitsuDA4Client | amplify.ToshibaSQBM2Client | amplify.GurobiClient | amplify.NECVA2Client):
             * integer_encoding_method (str | amplify.IntegerEncodingMethod): Defaults to ``Default``.
             * quadratization_method (str | amplify.QuadratizationMethod): Defaults to ``IshikawaKZFD``.
             * substitution_multiplier (float): Defaults to ``1.0``.
             * embedding_method (str | amplify.EmbeddingMethod): Defaults to ``Default``.
             * embedding_timeout (float | datetime.timedelta): Defaults to ``10.0``.
             * chain_strength (float): Defaults to ``1.0``.
             * dry_run (bool): Defaults to ``False``.
             * num_solves (int): Defaults to ``1``.
             * filter_solution (bool): Defaults to ``True``.
             * sort_solution (bool): Defaults to ``True``.
 
         Returns:
             amplify.Result:
 
-    .. admonition:: 2. solve(model: Union[amplify.Poly, amplify.Matrix, amplify.Constraint, amplify.ConstraintList], client: Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient], integer_encoding_method: Union[str, amplify.IntegerEncodingMethod] = Default, quadratization_method: Union[str, amplify.QuadratizationMethod] = IshikawaKZFD, substitution_multiplier: float = 1.0, embedding_method: Union[str, amplify.EmbeddingMethod] = Default, embedding_timeout: Union[float, datetime.timedelta] = 10.0, chain_strength: float = 1.0, dry_run: bool = False, num_solves: int = 1, filter_solution: bool = True, sort_solution: bool = True) -> amplify.Result
+    .. admonition:: 2. solve(model: Union[amplify.Poly, amplify.Matrix, amplify.Constraint, amplify.ConstraintList], client: Union[amplify.FixstarsClient, amplify.DWaveSamplerClient, amplify.LeapHybridSamplerClient, amplify.LeapHybridCQMSamplerClient, amplify.FujitsuDA4Client, amplify.ToshibaSQBM2Client, amplify.GurobiClient, amplify.NECVA2Client], integer_encoding_method: Union[str, amplify.IntegerEncodingMethod] = Default, quadratization_method: Union[str, amplify.QuadratizationMethod] = IshikawaKZFD, substitution_multiplier: float = 1.0, embedding_method: Union[str, amplify.EmbeddingMethod] = Default, embedding_timeout: Union[float, datetime.timedelta] = 10.0, chain_strength: float = 1.0, dry_run: bool = False, num_solves: int = 1, filter_solution: bool = True, sort_solution: bool = True) -> amplify.Result
 
         Args:
             * model (amplify.Poly | amplify.Matrix | amplify.Constraint | amplify.ConstraintList):
-            * client (amplify.FixstarsClient | amplify.DWaveSamplerClient | amplify.LeapHybridSamplerClient | amplify.LeapHybridCQMSamplerClient | amplify.FujitsuDA4Client | amplify.ToshibaSQBM2Client | amplify.GurobiClient):
+            * client (amplify.FixstarsClient | amplify.DWaveSamplerClient | amplify.LeapHybridSamplerClient | amplify.LeapHybridCQMSamplerClient | amplify.FujitsuDA4Client | amplify.ToshibaSQBM2Client | amplify.GurobiClient | amplify.NECVA2Client):
             * integer_encoding_method (str | amplify.IntegerEncodingMethod): Defaults to ``Default``.
             * quadratization_method (str | amplify.QuadratizationMethod): Defaults to ``IshikawaKZFD``.
             * substitution_multiplier (float): Defaults to ``1.0``.
             * embedding_method (str | amplify.EmbeddingMethod): Defaults to ``Default``.
             * embedding_timeout (float | datetime.timedelta): Defaults to ``10.0``.
             * chain_strength (float): Defaults to ``1.0``.
             * dry_run (bool): Defaults to ``False``.
```

## amplify/_backward.py

```diff
@@ -309,14 +309,24 @@
 
         self._method = method
         self._substitution_multiplier = 1.0
         self.__intermediate_model: Model | None = None
         self._intermediate_poly: Poly | None = None
         self._intermediate_mapping: Result.ModelConversion.IntermediateMapping | None = None
 
+    def __add__(self, arg: Constraint | ConstraintList):
+        return self.__class__(self._model + arg)
+
+    def __iadd__(self, arg: Constraint | ConstraintList):
+        self._model += arg
+        return self
+
+    def __radd__(self, arg: Constraint | ConstraintList):
+        return self.__class__(arg + self._model)
+
     @property
     def substitution_multiplier(self) -> float:
         return self._substitution_multiplier
 
     @substitution_multiplier.setter
     def substitution_multiplier(self, value: float):
         if not isinstance(value, float) or value <= 0:
```

## amplify/client/__init__.py

```diff
@@ -4,19 +4,19 @@
 from typing import NoReturn
 
 from typing_extensions import deprecated
 
 from .. import DWaveSamplerClient as _DWaveSamplerClient
 from .. import FixstarsClient as _FixstarsClient
 from .. import FujitsuDA4Client
+from .. import NECVA2Client
 from .. import GurobiClient as _GurobiClient
 from .. import LeapHybridSamplerClient as _LeapHybridSamplerClient
 from .. import ToshibaSQBM2Client as _ToshibaSQBM2Client
-from .._backward import (_deprecation_warnings_msg, _NotImplemented,
-                         _obsolete_warnings_msg)
+from .._backward import _deprecation_warnings_msg, _NotImplemented, _obsolete_warnings_msg
 
 warnings.warn(_deprecation_warnings_msg(f"{__name__} module"), DeprecationWarning, stacklevel=2)
 
 __all__ = [
     "FixstarsClient",
     "DWaveSamplerClient",
     "LeapHybridSamplerClient",
@@ -144,11 +144,10 @@
 
 
 @deprecated(_obsolete_warnings_msg("amplify.client.QulacsClient"))
 class QulacsClient(_FutureRelease):
     pass
 
 
-@deprecated(_obsolete_warnings_msg("amplify.client.NECClient"))
-class NECClient(_FutureRelease):
+@deprecated(_obsolete_warnings_msg("amplify.client.NECClient", "amplify.NECVA2Client"))
+class NECClient(NECVA2Client):
     pass
-
```

## amplify/client/ocean.py

```diff
@@ -7,15 +7,16 @@
 from .._backward import _deprecation_warnings_msg
 
 __all__ = [
     "DWaveSamplerClient",
     "LeapHybridSamplerClient",
 ]
 
+
 @deprecated(_deprecation_warnings_msg("amplify.client.DWaveSamplerClient", "amplify.DWaveSamplerClient"))
 class DWaveSamplerClient(_DWaveSamplerClient):
     pass
 
+
 @deprecated(_deprecation_warnings_msg("amplify.client.LeapHybridSamplerClient", "amplify.LeapHybridSamplerClient"))
 class LeapHybridSamplerClient(_LeapHybridSamplerClient):
     pass
-
```

## Comparing `amplify-1.0.5.dist-info/LICENSE.txt` & `amplify-1.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `amplify-1.0.5.dist-info/METADATA` & `amplify-1.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amplify
-Version: 1.0.5
+Version: 1.1.0
 Summary: Amplify SDK for Quantum Annealing and Ising Machines
 Author-email: "Fixstars Amplify Corp." <y_matsuda@fixstars.com>
 Maintainer-email: Yoshiki Matsuda <y_matsuda@fixstars.com>
 License: Terms of Use
         ________________________________________
         These Terms of Use stipulate the terms and conditions for the granting of licenses by Fixstars Amplify Corporation (“we”, “us”, “our”) to the User for use of Fixstars Amplify (“Service”), which provides Users with a software development environment and computational resources for solving mathematical optimization problems. There are two types of Service plans: the “Free plan” with certain restrictions on the scope of use, and the “Paid plan” with no such restrictions. Unless otherwise specified, these Terms apply to both plan types.
         Before using the Service, the User shall carefully read and agree to the entire text of these Terms of Use. When they click on our website to the effect that they agree to these Terms of Use, or complete the other procedures specified by us, a contract for the use of the Service is established, and the User is deemed to have fully agreed to these Terms of Use.
@@ -157,14 +157,14 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: open_source_license.txt
 Requires-Dist: numpy !=1.24.0
 Requires-Dist: typing-extensions
 Provides-Extra: extra
-Requires-Dist: dwave-system >=1.21.0 ; (platform_machine != "arm64" and python_version <= "3.11") and extra == 'extra'
+Requires-Dist: dwave-system >=1.21.0 ; (platform_machine != "arm64" or platform_system != "Darwin") and extra == 'extra'
 
 ## About Fixstars Amplify
 
 Fixstars Amplify SDK is a middleware library for Ising machines developed by Fixstars Amplify Corporation. Ising machines specialize in solving optimization problems described by quadratic polynomials of binary variables. Various types of Ising machines implemented with digital circuits and GPUs have been released, starting with the quantum annealing machine by D-Wave Systems. This middleware is an intermediate layer between hardware and applications using Ising machines. We provide various functions that improve the convenience of the machines and enable highly efficient application software development.
 
 [![Fixstars Amplify](https://img.shields.io/badge/-Fixstars%20Amplify-333333.svg?logo=data:image/png;base64,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&style=popout-square)](https://amplify.fixstars.com/) [![PyPI](https://img.shields.io/pypi/v/amplify)](https://pypi.org/project/amplify/) [![Downloads](https://static.pepy.tech/personalized-badge/amplify?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/amplify)
```

## Comparing `amplify-1.0.5.dist-info/open_source_license.txt` & `amplify-1.1.0.dist-info/open_source_license.txt`

 * *Files identical despite different names*

