# Comparing `tmp/odex-0.0.2.tar.gz` & `tmp/odex-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odex-0.0.2.tar", max compression
+gzip compressed data, was "odex-0.0.3.tar", max compression
```

## Comparing `odex-0.0.2.tar` & `odex-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1062 2024-05-14 22:45:34.863882 odex-0.0.2/LICENSE
--rw-r--r--   0        0        0      962 2024-05-14 22:45:34.863882 odex-0.0.2/README.md
--rw-r--r--   0        0        0      633 2024-05-14 22:45:34.863882 odex-0.0.2/odex/__init__.py
--rw-r--r--   0        0        0     7055 2024-05-14 22:45:34.863882 odex-0.0.2/odex/condition.py
--rw-r--r--   0        0        0      701 2024-05-14 22:45:34.863882 odex-0.0.2/odex/container.py
--rw-r--r--   0        0        0      829 2024-05-14 22:45:34.863882 odex-0.0.2/odex/context.py
--rw-r--r--   0        0        0     3530 2024-05-14 22:45:34.863882 odex-0.0.2/odex/index.py
--rw-r--r--   0        0        0     4528 2024-05-14 22:45:34.863882 odex-0.0.2/odex/optimize.py
--rw-r--r--   0        0        0     4439 2024-05-14 22:45:34.863882 odex-0.0.2/odex/parse.py
--rw-r--r--   0        0        0     3467 2024-05-14 22:45:34.863882 odex-0.0.2/odex/plan.py
--rw-r--r--   0        0        0     7698 2024-05-14 22:45:34.863882 odex-0.0.2/odex/set.py
--rw-r--r--   0        0        0      600 2024-05-14 22:45:34.863882 odex-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1676 1970-01-01 00:00:00.000000 odex-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-15 13:32:22.748617 odex-0.0.3/LICENSE
+-rw-r--r--   0        0        0      955 2024-05-15 13:32:22.748617 odex-0.0.3/README.md
+-rw-r--r--   0        0        0      631 2024-05-15 13:32:22.748617 odex-0.0.3/odex/__init__.py
+-rw-r--r--   0        0        0     7055 2024-05-15 13:32:22.748617 odex-0.0.3/odex/condition.py
+-rw-r--r--   0        0        0      701 2024-05-15 13:32:22.748617 odex-0.0.3/odex/container.py
+-rw-r--r--   0        0        0      857 2024-05-15 13:32:22.748617 odex-0.0.3/odex/context.py
+-rw-r--r--   0        0        0     3472 2024-05-15 13:32:22.748617 odex-0.0.3/odex/index.py
+-rw-r--r--   0        0        0     3542 2024-05-15 13:32:22.748617 odex-0.0.3/odex/optimize.py
+-rw-r--r--   0        0        0     4569 2024-05-15 13:32:22.748617 odex-0.0.3/odex/parse.py
+-rw-r--r--   0        0        0     3437 2024-05-15 13:32:22.748617 odex-0.0.3/odex/plan.py
+-rw-r--r--   0        0        0     8087 2024-05-15 13:32:22.748617 odex-0.0.3/odex/set.py
+-rw-r--r--   0        0        0      280 2024-05-15 13:32:22.748617 odex-0.0.3/odex/utils.py
+-rw-r--r--   0        0        0      600 2024-05-15 13:32:22.748617 odex-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1669 1970-01-01 00:00:00.000000 odex-0.0.3/PKG-INFO
```

### Comparing `odex-0.0.2/LICENSE` & `odex-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `odex-0.0.2/README.md` & `odex-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # odex
 
-Python object index for fast, declarative retrieval.
+Python object index for fast, declarative retrieval
 
 ## Install
 
 ```
 pip install odex
 ```
 
 ## Usage
 
 Odex provides a set-like collection called `IndexedSet`:
 
 ```python
+from collections import namedtuple
 from odex import IndexedSet, HashIndex, attr, and_
 
-class X:
-    def __init__(self, a, b):
-        self.a = a
-        self.b = b
-
-objs = [
-    X(a=1, b=4),
-    X(a=2, b=5),
-    X(a=2, b=6),
-    X(a=3, b=7),
-]
-        
-iset = IndexedSet(objs, indexes=[HashIndex("a")])
+X = namedtuple("X", ["a", "b"])
+
+iset = IndexedSet(
+    [
+        X(a=1, b=4),
+        X(a=2, b=5),
+        X(a=2, b=6),
+        X(a=3, b=7),
+    ], 
+    indexes=[HashIndex("a")]
+)
 
 # Filter objects with SQL-like expressions:
-assert iset.filter("a = 2 AND b = 5") == {objs[1]}
+iset.filter("a = 2 AND b = 5") == {X(a=2, b=5)}
 
 # Or, using the fluent interface:
-assert iset.filter(
+iset.filter(
     and_(
         attr("a").eq(2),
         attr("b").eq(5)
     )
-) == {objs[1]}
+) == {X(a=2, b=5)}
 ```
 
 ## Related projects
 
 - [sqlglot](https://github.com/tobymao/sqlglot) - odex uses sqlglot for expression parsing
 - [ducks](https://github.com/manimino/ducks) - similar project with different tradeoffs
```

### Comparing `odex-0.0.2/odex/__init__.py` & `odex-0.0.3/odex/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from odex.set import IndexedSet as IndexedSet
-from odex.index import HashIndex as HashIndex, MultiHashIndex as MultiHashIndex
+from odex.index import HashIndex as HashIndex, InvertedIndex as InvertedIndex
 from odex.condition import (
     literal as literal,
     attr as attr,
     and_ as and_,
     or_ as or_,
     add as add,
     div as div,
```

### Comparing `odex-0.0.2/odex/condition.py` & `odex-0.0.3/odex/condition.py`

 * *Files identical despite different names*

### Comparing `odex-0.0.2/odex/container.py` & `odex-0.0.3/odex/container.py`

 * *Files identical despite different names*

### Comparing `odex-0.0.2/odex/context.py` & `odex-0.0.3/odex/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from dataclasses import dataclass, field
 
-from typing import Any, TYPE_CHECKING, Set, TypeVar, List
+from typing import Any, Dict, TYPE_CHECKING, Set, TypeVar, List
 from typing_extensions import Protocol
 
 if TYPE_CHECKING:
     from odex.index import Index
     from odex.set import Attributes
 
 T = TypeVar("T")
 
 
 class Context(Protocol[T]):
     """Interface for filter context, so `IndexedSet` can pass context to optimizers"""
 
-    indexes: "List[Index]"
+    indexes: "Dict[str, List[Index]]"
     objs: Set[T]
     attrs: "Attributes"
 
     def getattr(self, obj: T, item: str) -> Any: ...
 
 
 @dataclass
 class SimpleContext(Context[T]):
     """Context as a dataclass. Intended for testing."""
 
-    indexes: "List[Index]" = field(default_factory=list)
+    indexes: "Dict[str, List[Index]]" = field(default_factory=dict)
     objs: Set[T] = field(default_factory=set)
     attrs: "Attributes" = field(default_factory=dict)
 
     def getattr(self, obj: T, item: str) -> Any:
         return getattr(obj, item)
```

### Comparing `odex-0.0.2/odex/index.py` & `odex-0.0.3/odex/index.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from abc import abstractmethod
-from typing import Generic, TypeVar, Set, Any, Optional, Iterable, Dict
+from typing import Generic, TypeVar, Set, Any, Optional, Iterable, Dict, List
 from typing_extensions import Protocol
 
-from odex.condition import Condition, Eq, Literal, Attribute, In
+from odex.condition import Condition, Eq, Literal, In, BinOp
 from odex.context import Context
 from odex.plan import IndexLookup
 
 T = TypeVar("T")
 
 
 class Index(Protocol[T]):
+    attributes: List[str]
+
     @abstractmethod
     def add(self, objs: Set[T], ctx: Context[T]) -> None:
         """Add `objs` to the index"""
 
     @abstractmethod
     def remove(self, objs: Set[T], ctx: Context[T]) -> None:
         """Remove `objs` from the index"""
 
     @abstractmethod
-    def match(self, condition: Condition) -> "Optional[IndexLookup]":
+    def match(self, condition: BinOp, operand: Condition) -> "Optional[IndexLookup]":
         """
         Determine if this index can serve the given `condition`.
 
+        This assumes the optimizer has already found which side of the condition is the attribute.
+
         Args:
-            condition: logical expression
+            condition: the entire binary operator
+            operand: the side of the binary operator opposite the attribute
         Returns:
             `None` if this index can't serve the condition.
             `IndexLoop` plan if it can.
         """
 
     @abstractmethod
     def lookup(self, value: Any) -> Set[T]:
@@ -55,14 +60,15 @@
 
     Args:
         attr: name of the attribute to index
     """
 
     def __init__(self, attr: str):
         self.attr = attr
+        self.attributes = [attr]
         self.idx: Dict[Any, Set[T]] = {}
 
     def add(self, objs: Set[T], ctx: Context[T]) -> None:
         for o in objs:
             for val in self._extract_values(o, ctx):
                 self.idx.setdefault(val, set()).add(o)
 
@@ -70,47 +76,40 @@
         for o in objs:
             for val in self._extract_values(o, ctx):
                 self.idx.setdefault(val, set()).remove(o)
 
     def lookup(self, value: Any) -> Set[T]:
         return self.idx.get(value) or set()
 
-    def match(self, condition: Condition) -> Optional[IndexLookup]:
-        value = self._match(condition)
+    def match(self, condition: BinOp, operand: Condition) -> "Optional[IndexLookup]":
+        value = self._match(condition, operand)
         if value is _NotFound:
             return None
-        objs = self.idx.get(value) or set()
-        return IndexLookup(index=self, cost=len(objs), value=value)
+        return IndexLookup(index=self, value=value)
 
     def _extract_values(self, obj: T, ctx: Context[T]) -> Iterable[Any]:
         yield ctx.getattr(obj, self.attr)
 
-    def _match(self, condition: Condition) -> Any:
-        if isinstance(condition, Eq):
-            l, r = condition.left, condition.right
-            if isinstance(l, Attribute) and l.name == self.attr and isinstance(r, Literal):
-                return r.value
-            elif isinstance(r, Attribute) and r.name == self.attr and isinstance(l, Literal):
-                return l.value
+    def _match(self, condition: BinOp, operand: Condition) -> Any:
+        if isinstance(condition, Eq) and isinstance(operand, Literal):
+            return operand.value
         return _NotFound
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.attr})"
 
 
-class MultiHashIndex(Generic[T], HashIndex[T]):
+class InvertedIndex(Generic[T], HashIndex[T]):
     """
     Same as a `HashIndex`, except this assumes the attribute is a collection of values.
 
     This matches IN expressions, e.g. `1 in a`
     """
 
     def _extract_values(self, obj: T, ctx: Context[T]) -> Iterable[Any]:
         for val in ctx.getattr(obj, self.attr):
             yield val
 
-    def _match(self, condition: Condition) -> Any:
-        if isinstance(condition, In):
-            member, container = condition.left, condition.right
-            if isinstance(member, Literal) and isinstance(container, Attribute):
-                return member.value
+    def _match(self, condition: BinOp, operand: Condition) -> Any:
+        if isinstance(condition, In) and operand is condition.left and isinstance(operand, Literal):
+            return operand.value
         return _NotFound
```

### Comparing `odex-0.0.2/odex/optimize.py` & `odex-0.0.3/odex/optimize.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Dict, Type, Callable, Sequence, cast
+from typing import Callable, Sequence
 from typing_extensions import Protocol
 
-from odex.condition import and_
+from odex.condition import and_, BinOp, Attribute
 from odex.context import Context
-from odex.plan import Plan, SetOp, Intersect, Filter, ScanFilter, Union, IndexLookup
+from odex.plan import Plan, SetOp, Intersect, Filter, ScanFilter
 
 
 class Rule(Protocol):
     def __call__(self, plan: Plan, ctx: Context) -> Plan: ...
 
 
 class TransformerWithContext:
@@ -49,22 +49,29 @@
 
 
 class UseIndex(TransformerRule):
     """Replace scans with index lookups"""
 
     def transform(self, plan: Plan, ctx: Context) -> Plan:
         if isinstance(plan, ScanFilter):
-            best_plan: Plan = plan
-            best_cost = len(ctx.objs)
-            for idx in ctx.indexes:
-                match = idx.match(plan.condition)
-                if match:
-                    if best_cost is None or match.cost <= best_cost:
-                        best_plan, best_cost = match, match.cost
-            return best_plan
+            condition = plan.condition
+            if isinstance(condition, BinOp):
+                l, r = condition.left, condition.right
+
+                if isinstance(l, Attribute) and not isinstance(r, Attribute):
+                    name, value = l.name, r
+                elif isinstance(r, Attribute) and not isinstance(l, Attribute):
+                    name, value = r.name, l
+                else:
+                    return plan
+
+                for idx in ctx.indexes.get(name) or []:
+                    match = idx.match(condition, value)
+                    if match:
+                        return match
 
         return plan
 
 
 class CombineFilters(TransformerRule):
     """Combine multiple filters into one"""
 
@@ -89,48 +96,19 @@
                 else:
                     return ScanFilter(
                         condition=combined,
                     )
         return plan
 
 
-class OrderIntersects(Rule):
-    """Reorder intersections so that the plans with the smallest cost are first"""
-
-    def __init__(self) -> None:
-        self.estimators: Dict[Type[Plan], Callable[[Plan, Context], int]] = {
-            ScanFilter: lambda plan, ctx: len(ctx.objs),
-            Filter: lambda plan, ctx: self._estimate(cast(Filter, plan).input, ctx),
-            IndexLookup: lambda plan, ctx: cast(IndexLookup, plan).cost,
-            Union: lambda plan, ctx: max(self._estimate(i, ctx) for i in cast(Union, plan).inputs),
-            Intersect: self._estimate_intersect,
-        }
-
-    def __call__(self, plan: Plan, ctx: Context) -> Plan:
-        self._estimate(plan, ctx)
-        return plan
-
-    def _estimate(self, plan: Plan, ctx: Context) -> int:
-        estimator = self.estimators.get(plan.__class__)
-        return estimator(plan, ctx) if estimator else len(ctx.objs)
-
-    def _estimate_intersect(self, plan: Plan, ctx: Context) -> int:
-        plan = cast(Intersect, plan)
-        costs = sorted(((self._estimate(i, ctx), i) for i in plan.inputs), key=lambda t: t[0])
-        plan.inputs = [i[1] for i in costs]
-        return costs[0][0]
-
-
 class Chain(Rule):
     """Chain multiple rules together"""
 
-    DEFAULT_RULES = (MergeSetOps(), UseIndex(), CombineFilters(), OrderIntersects())
+    DEFAULT_RULES = (MergeSetOps(), UseIndex(), CombineFilters())
 
     def __init__(self, rules: Sequence[Rule] = DEFAULT_RULES):
         self.rules = list(rules)
 
     def __call__(self, plan: Plan, ctx: Context) -> Plan:
         for rule in self.rules:
             plan = rule(plan, ctx)
-            # print(rule)
-            # print(plan)
         return plan
```

### Comparing `odex-0.0.2/odex/parse.py` & `odex-0.0.3/odex/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,21 @@
             exp.GT: lambda e: self._convert_binary(cond.Gt, e),
             exp.GTE: lambda e: self._convert_binary(cond.Ge, e),
             exp.EQ: lambda e: self._convert_binary(cond.Eq, e),
             exp.NEQ: lambda e: self._convert_binary(cond.Ne, e),
             exp.And: lambda e: self._convert_binary(cond.And, e),
             exp.Or: lambda e: self._convert_binary(cond.Or, e),
             exp.Not: lambda e: self._convert_unary(cond.Not, e),
+            exp.BitwiseNot: lambda e: self._convert_unary(cond.Invert, e),
             exp.Literal: self._convert_literal,
             exp.Column: self._convert_column,
             exp.In: self._convert_in,
             exp.Null: lambda e: Literal(None),
             exp.Boolean: lambda e: Literal(e.this),
+            exp.Paren: lambda e: self.convert(e.this),
         }
 
     def convert(self, expression: exp.Expression) -> Condition:
         converter = self.converters.get(expression.__class__)
         if not converter:
             raise ValueError(f"Unsupported sqlglot Expression: {expression.__class__}")
         return converter(expression)
```

### Comparing `odex-0.0.2/odex/plan.py` & `odex-0.0.3/odex/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,21 +103,20 @@
 
 @dataclass
 class IndexLookup(Plan):
     """Return objects by looking up `value` in `index`"""
 
     index: "Index"
     value: Any
-    cost: int
 
     def to_s(self, depth=0):
         return f"IndexLookup: {self.index} = {self.value}"
 
     def __deepcopy__(self, memodict):
-        return IndexLookup(index=self.index, value=deepcopy(self.value), cost=self.cost)
+        return IndexLookup(index=self.index, value=deepcopy(self.value))
 
 
 class Planner:
     def plan(self, condition: Condition) -> Plan:
         """
         Convert a syntax tree into a query plan.
```

### Comparing `odex-0.0.2/odex/set.py` & `odex-0.0.3/odex/set.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,24 @@
     Dict,
     List,
     Union as UnionType,
     Optional,
     Iterable,
     Iterator,
     MutableSet,
+    Sequence,
 )
 
 from odex.index import Index
 from odex.optimize import Chain, Rule
 from odex.parse import Parser
 from odex.plan import Plan, Union, Intersect, ScanFilter, Filter, Planner, IndexLookup
 from odex import condition as cond
 from odex.condition import BinOp, UnaryOp, Attribute, Literal, Condition
+from odex.utils import intersect
 
 T = TypeVar("T", bound=Hashable)
 
 Attributes = Dict[str, Callable[[T, str], Any]]
 
 
 class IndexedSet(MutableSet[T]):
@@ -82,37 +84,41 @@
         cond.Not: operator.not_,
         cond.Invert: operator.invert,
     }
 
     def __init__(
         self,
         objs: Optional[Iterable[T]] = None,
-        indexes: Optional[List[Index[T]]] = None,
+        indexes: Optional[Sequence[Index[T]]] = None,
         attrs: Optional[Attributes] = None,
         parser: Optional[Parser] = None,
         planner: Optional[Planner] = None,
         optimizer: Optional[Rule] = None,
     ):
         self.objs = objs if isinstance(objs, set) else set(objs) if objs else set()
         self.planner = planner or Planner()
         self.optimizer = optimizer or Chain()
         self.parser = parser or Parser()
         self.attrs = attrs or {}
-        self.indexes = indexes or []
+        self.indexes: Dict[str, List[Index]] = {}
+        for index in indexes or []:
+            for attr in index.attributes:
+                self.indexes.setdefault(attr, []).append(index)
+
         self.update(self.objs)
 
         self.executors: Dict[Type[Plan], Callable[[Plan], Set[T]]] = {
             ScanFilter: lambda plan: {o for o in self.objs if self.match(plan.condition, o)},  # type: ignore
             Filter: lambda plan: {
                 o
                 for o in self.execute(plan.input)  # type: ignore
                 if self.match(plan.condition, o)  # type: ignore
             },
             Union: lambda plan: set.union(*(self.execute(i) for i in plan.inputs)),  # type: ignore
-            Intersect: lambda plan: set.intersection(*(self.execute(i) for i in plan.inputs)),  # type: ignore
+            Intersect: lambda plan: intersect(*(self.execute(i) for i in plan.inputs)),  # type: ignore
             IndexLookup: lambda plan: plan.index.lookup(plan.value),  # type: ignore
         }
 
         def match_binop(op: Callable[[Any, Any], Any]) -> Callable[[BinOp, T], Any]:
             def matcher(condition: BinOp, obj: T) -> Any:
                 return op(self.match(condition.left, obj), self.match(condition.right, obj))
 
@@ -207,34 +213,39 @@
 
     def getattr(self, obj: T, item: str) -> Any:
         """Get the attribute `item` from `obj`"""
         return self.attrs.get(item, getattr)(obj, item)
 
     def add(self, obj: T) -> None:
         self.objs.add(obj)
-        for index in self.indexes:
+        for index in self._iter_indexes():
             index.add({obj}, self)
 
     def discard(self, obj: T) -> None:
         self.objs.discard(obj)
-        for index in self.indexes:
+        for index in self._iter_indexes():
             index.remove({obj}, self)
 
     def __contains__(self, x: Any) -> bool:
         return x in self.objs
 
     def __len__(self) -> int:
         return len(self.objs)
 
     def __iter__(self) -> Iterator[T]:
         for i in self.objs:
             yield i
 
     def update(self, objs: Set[T]) -> None:
         self.objs.update(objs)
-        for index in self.indexes:
+        for index in self._iter_indexes():
             index.add(objs, self)
 
     def difference_update(self, objs: Set[T]) -> None:
         self.objs.difference_update(objs)
-        for index in self.indexes:
+        for index in self._iter_indexes():
             index.remove(objs, self)
+
+    def _iter_indexes(self) -> Iterator[Index]:
+        for indexes in self.indexes.values():
+            for index in indexes:
+                yield index
```

### Comparing `odex-0.0.2/pyproject.toml` & `odex-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odex"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python object index for fast, declarative retrieval"
 authors = ["Barak Alon"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/barakalon/odex"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `odex-0.0.2/PKG-INFO` & `odex-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odex
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python object index for fast, declarative retrieval
 Home-page: https://github.com/barakalon/odex
 License: MIT
 Author: Barak Alon
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,53 +16,52 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: sqlglot
 Requires-Dist: typing_extensions
 Description-Content-Type: text/markdown
 
 # odex
 
-Python object index for fast, declarative retrieval.
+Python object index for fast, declarative retrieval
 
 ## Install
 
 ```
 pip install odex
 ```
 
 ## Usage
 
 Odex provides a set-like collection called `IndexedSet`:
 
 ```python
+from collections import namedtuple
 from odex import IndexedSet, HashIndex, attr, and_
 
-class X:
-    def __init__(self, a, b):
-        self.a = a
-        self.b = b
-
-objs = [
-    X(a=1, b=4),
-    X(a=2, b=5),
-    X(a=2, b=6),
-    X(a=3, b=7),
-]
-        
-iset = IndexedSet(objs, indexes=[HashIndex("a")])
+X = namedtuple("X", ["a", "b"])
+
+iset = IndexedSet(
+    [
+        X(a=1, b=4),
+        X(a=2, b=5),
+        X(a=2, b=6),
+        X(a=3, b=7),
+    ], 
+    indexes=[HashIndex("a")]
+)
 
 # Filter objects with SQL-like expressions:
-assert iset.filter("a = 2 AND b = 5") == {objs[1]}
+iset.filter("a = 2 AND b = 5") == {X(a=2, b=5)}
 
 # Or, using the fluent interface:
-assert iset.filter(
+iset.filter(
     and_(
         attr("a").eq(2),
         attr("b").eq(5)
     )
-) == {objs[1]}
+) == {X(a=2, b=5)}
 ```
 
 ## Related projects
 
 - [sqlglot](https://github.com/tobymao/sqlglot) - odex uses sqlglot for expression parsing
 - [ducks](https://github.com/manimino/ducks) - similar project with different tradeoffs
```

