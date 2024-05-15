# Comparing `tmp/nicegui_tabulator-0.1.1.tar.gz` & `tmp/nicegui_tabulator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicegui_tabulator-0.1.1.tar", max compression
+gzip compressed data, was "nicegui_tabulator-0.1.2.tar", max compression
```

## Comparing `nicegui_tabulator-0.1.1.tar` & `nicegui_tabulator-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1094 2024-05-08 17:39:27.737805 nicegui_tabulator-0.1.1/LICENSE
--rw-r--r--   0        0        0      128 2024-05-08 14:53:27.237225 nicegui_tabulator-0.1.1/nicegui_tabulator/__init__.py
--rw-r--r--   0        0        0      298 2024-05-08 17:33:19.252414 nicegui_tabulator-0.1.1/nicegui_tabulator/core/events.py
--rw-r--r--   0        0        0    33593 2024-05-08 15:00:49.017552 nicegui_tabulator-0.1.1/nicegui_tabulator/core/libs/tabulator.min.css
--rw-r--r--   0        0        0   484963 2024-05-08 15:01:02.793045 nicegui_tabulator-0.1.1/nicegui_tabulator/core/libs/tabulator.min.js
--rw-r--r--   0        0        0     2575 2024-05-10 14:29:33.793888 nicegui_tabulator-0.1.1/nicegui_tabulator/core/tabulator.js
--rw-r--r--   0        0        0     5674 2024-05-10 14:29:33.793888 nicegui_tabulator-0.1.1/nicegui_tabulator/core/tabulator.py
--rw-r--r--   0        0        0       97 2024-05-08 14:40:20.875090 nicegui_tabulator-0.1.1/nicegui_tabulator/version.py
--rw-r--r--   0        0        0      565 2024-05-10 14:32:42.352222 nicegui_tabulator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1830 2024-05-08 17:38:13.156421 nicegui_tabulator-0.1.1/README.md
--rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 nicegui_tabulator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-05-08 17:39:27.737805 nicegui_tabulator-0.1.2/LICENSE
+-rw-r--r--   0        0        0      128 2024-05-08 14:53:27.237225 nicegui_tabulator-0.1.2/nicegui_tabulator/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-08 17:33:19.252414 nicegui_tabulator-0.1.2/nicegui_tabulator/core/events.py
+-rw-r--r--   0        0        0    33593 2024-05-08 15:00:49.017552 nicegui_tabulator-0.1.2/nicegui_tabulator/core/libs/tabulator.min.css
+-rw-r--r--   0        0        0   484963 2024-05-08 15:01:02.793045 nicegui_tabulator-0.1.2/nicegui_tabulator/core/libs/tabulator.min.js
+-rw-r--r--   0        0        0     2698 2024-05-15 07:17:16.265715 nicegui_tabulator-0.1.2/nicegui_tabulator/core/tabulator.js
+-rw-r--r--   0        0        0     6796 2024-05-15 07:34:12.484761 nicegui_tabulator-0.1.2/nicegui_tabulator/core/tabulator.py
+-rw-r--r--   0        0        0      824 2024-05-15 07:23:00.814564 nicegui_tabulator-0.1.2/nicegui_tabulator/core/utils.py
+-rw-r--r--   0        0        0       97 2024-05-08 14:40:20.875090 nicegui_tabulator-0.1.2/nicegui_tabulator/version.py
+-rw-r--r--   0        0        0      584 2024-05-15 07:36:27.229719 nicegui_tabulator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2411 2024-05-15 07:17:14.855234 nicegui_tabulator-0.1.2/README.md
+-rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 nicegui_tabulator-0.1.2/PKG-INFO
```

### Comparing `nicegui_tabulator-0.1.1/LICENSE` & `nicegui_tabulator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nicegui_tabulator-0.1.1/nicegui_tabulator/core/libs/tabulator.min.css` & `nicegui_tabulator-0.1.2/nicegui_tabulator/core/libs/tabulator.min.css`

 * *Files identical despite different names*

### Comparing `nicegui_tabulator-0.1.1/nicegui_tabulator/core/libs/tabulator.min.js` & `nicegui_tabulator-0.1.2/nicegui_tabulator/core/libs/tabulator.min.js`

 * *Files identical despite different names*

### Comparing `nicegui_tabulator-0.1.1/nicegui_tabulator/core/tabulator.js` & `nicegui_tabulator-0.1.2/nicegui_tabulator/core/tabulator.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -79,21 +79,24 @@
         convertDynamicProperties(this.options, true);
         this.table = new Tabulator(this.$el, this.options);
 
     },
 
     methods: {
         onEvent(eventName) {
-
             this.table.on(eventName, (...args) => {
                 const eventArgs = extractEventArg(eventName, args);
                 this.$emit('table-event', {
                     eventName,
                     args: eventArgs
                 });
+
+                if (eventName === 'rowContext' || eventName === 'groupContext') {
+                    args[0].preventDefault();
+                }
             });
         },
         run_table_method(name, ...args) {
             if (name.startsWith(":")) {
                 name = name.slice(1);
                 args = args.map((arg) => new Function(`return (${arg})`)());
             }
```

### Comparing `nicegui_tabulator-0.1.1/nicegui_tabulator/core/tabulator.py` & `nicegui_tabulator-0.1.2/nicegui_tabulator/core/tabulator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 from pathlib import Path
 from typing import Callable, Dict, List, Optional
 from nicegui.element import Element
 from nicegui.events import handle_event
-from nicegui import ui, Client as ng_client
 from nicegui.awaitable_response import AwaitableResponse
 from .events import TabulatorEventArguments
 
+from .utils import DeferredTask
+
+try:
+    import pandas as pd
+except ImportError:
+    pass
+
 
 class Tabulator(Element, component="tabulator.js", libraries=["libs/tabulator.min.js"]):
     def __init__(
         self,
         options: Dict,
     ) -> None:
+        """Create a new tabulator table.
+
+        Args:
+            options (Dict): The options for the tabulator table.
+        """
         super().__init__()
         self.__deferred_task = DeferredTask()
         self._event_listener_map: Dict[str, Callable[..., None]] = {}
 
         self._props["options"] = options
         self.add_resource(Path(__file__).parent / "libs")
 
@@ -92,15 +103,18 @@
             {'title':"Age", 'field':"age"},
         ]
 
         table.set_columns(new_columns)
         ```
 
         """
-        self.run_method("setColumns", columns)
+
+        @self.__deferred_task.register
+        def _():
+            self.run_method("setColumns", columns)
 
     def update_column_definition(self, field: str, definition: Dict) -> None:
         """
         Update an existing column definition.
 
         @see https://tabulator.info/docs/6.2/columns#update
 
@@ -110,15 +124,18 @@
 
         ## Example Usage
         ```python
         table = Tabulator({...})
         table.update_column_definition("name", {'title':"Updated Title"})
         ```
         """
-        self.run_method("updateColumnDefinition", field, definition)
+
+        @self.__deferred_task.register
+        def _():
+            self.run_method("updateColumnDefinition", field, definition)
 
     def add_column(
         self,
         definition: Dict,
         before: Optional[bool] = None,
         position: Optional[str] = None,
     ) -> None:
@@ -137,37 +154,57 @@
 
         ```python
         table = Tabulator({...})
         table.add_column({'title':"Age", 'field':"age"}, True, "name")
         ```
 
         """
-        self.run_table_method("addColumn", definition, before, position)
+
+        @self.__deferred_task.register
+        def _():
+            self.run_table_method("addColumn", definition, before, position)
 
     def update(self) -> None:
         super().update()
         self.run_method("update_table")
 
+    @classmethod
+    def from_pandas(
+        cls,
+        df: "pd.DataFrame",
+    ):
+        """Create a table from a Pandas DataFrame.
+
+        Note:
+        If the DataFrame contains non-serializable columns of type `datetime64[ns]`, `timedelta64[ns]`, `complex128` or `period[M]`,
+        they will be converted to strings.
+
+        Args:
+            df (pd.DataFrame): The DataFrame to create the table from.
+        """
+
+        def is_special_dtype(dtype):
+            return (
+                pd.api.types.is_datetime64_any_dtype(dtype)
+                or pd.api.types.is_timedelta64_dtype(dtype)
+                or pd.api.types.is_complex_dtype(dtype)
+                or isinstance(dtype, pd.PeriodDtype)
+            )
+
+        special_cols = df.columns[df.dtypes.apply(is_special_dtype)]
+        if not special_cols.empty:
+            df = df.copy()
+            df[special_cols] = df[special_cols].astype(str)
+
+        if isinstance(df.columns, pd.MultiIndex):
+            raise ValueError(
+                "MultiIndex columns are not supported. "
+                "You can convert them to strings using something like "
+                '`df.columns = ["_".join(col) for col in df.columns.values]`.'
+            )
+
+        options = {
+            "data": df.to_dict(orient="records"),
+            "columns": [{"title": col, "field": col} for col in df.columns],
+        }
 
-class DeferredTask:
-    def __init__(self):
-        self._tasks = []
-
-        async def on_client_connect(
-            client: ng_client,
-        ):
-            await client.connected()
-
-            for task in self._tasks:
-                task()
-
-            # Avoid events becoming ineffective due to page refresh when sharing the client.
-            if not client.shared:
-                client.connect_handlers.remove(on_client_connect)  # type: ignore
-
-        ui.context.client.on_connect(on_client_connect)
-
-    def register(self, task: Callable[..., None]):
-        if ui.context.client.has_socket_connection:
-            task()
-        else:
-            self._tasks.append(task)
+        return cls(options)
```

### Comparing `nicegui_tabulator-0.1.1/pyproject.toml` & `nicegui_tabulator-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "nicegui-tabulator"
-version = "0.1.1"
+version = "0.1.2"
 description = "This is a Python package that provides a simple way to create tables using the Tabulator library. It is built on top of the NiceGUI library."
 authors = ["CrystalWindSnake <568166495@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nicegui = "^1.4.24"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 playwright = "^1.43.0"
 pytest-playwright = "^0.5.0"
+pandas = "^2.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nicegui_tabulator-0.1.1/README.md` & `nicegui_tabulator-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -69,7 +69,40 @@
         ],
     )
 
 
 ui.button("sort", on_click=on_sort)
 
 ```
+
+---
+
+create from pandas dataframe:
+
+```python
+from nicegui_tabulator import tabulator
+import pandas as pd
+
+
+df = pd.DataFrame(
+    {
+        "name": ["Alice", "Bob", "Charlie"],
+        "age": [25, 30, 35],
+        "color": ["blue", "red", "green"],
+        "dob": [None, "2021-01-01", "2021-02-02"],
+    }
+)
+
+
+tabulator.from_pandas(df)
+```
+
+---
+
+You can update column configurations immediately after creating the table.
+
+
+```python
+tabulator.from_pandas(df).update_column_definition(
+    "age", {"hozAlign": "left", "formatter": "progress"}
+)
+```
```

### Comparing `nicegui_tabulator-0.1.1/PKG-INFO` & `nicegui_tabulator-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicegui-tabulator
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is a Python package that provides a simple way to create tables using the Tabulator library. It is built on top of the NiceGUI library.
 Author: CrystalWindSnake
 Author-email: 568166495@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -86,7 +86,39 @@
     )
 
 
 ui.button("sort", on_click=on_sort)
 
 ```
 
+---
+
+create from pandas dataframe:
+
+```python
+from nicegui_tabulator import tabulator
+import pandas as pd
+
+
+df = pd.DataFrame(
+    {
+        "name": ["Alice", "Bob", "Charlie"],
+        "age": [25, 30, 35],
+        "color": ["blue", "red", "green"],
+        "dob": [None, "2021-01-01", "2021-02-02"],
+    }
+)
+
+
+tabulator.from_pandas(df)
+```
+
+---
+
+You can update column configurations immediately after creating the table.
+
+
+```python
+tabulator.from_pandas(df).update_column_definition(
+    "age", {"hozAlign": "left", "formatter": "progress"}
+)
+```
```

