# Comparing `tmp/entangled_cli-2.0.2.tar.gz` & `tmp/entangled_cli-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entangled_cli-2.0.2.tar", max compression
+gzip compressed data, was "entangled_cli-2.0.3.tar", max compression
```

## Comparing `entangled_cli-2.0.2.tar` & `entangled_cli-2.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/LICENSE
--rw-r--r--   0        0        0    14973 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/README.md
--rw-r--r--   0        0        0        1 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/__init__.py
--rw-r--r--   0        0        0     2500 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/code_reader.py
--rw-r--r--   0        0        0      279 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/commands/__init__.py
--rw-r--r--   0        0        0     1356 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/commands/brei.py
--rw-r--r--   0        0        0     7071 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/commands/new.py
--rw-r--r--   0        0        0     1564 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/commands/status.py
--rw-r--r--   0        0        0     2267 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/commands/stitch.py
--rw-r--r--   0        0        0     1375 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/commands/sync.py
--rw-r--r--   0        0        0     2277 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/commands/tangle.py
--rw-r--r--   0        0        0     1714 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/commands/watch.py
--rw-r--r--   0        0        0     5634 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/config/__init__.py
--rw-r--r--   0        0        0     1783 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/config/language.py
--rw-r--r--   0        0        0      768 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/config/templates.py
--rw-r--r--   0        0        0      368 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/config/version.py
--rw-r--r--   0        0        0     4738 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/construct.py
--rw-r--r--   0        0        0     2388 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/document.py
--rw-r--r--   0        0        0        0 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/errors/__init__.py
--rw-r--r--   0        0        0      586 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/errors/internal.py
--rw-r--r--   0        0        0     1398 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/errors/user.py
--rw-r--r--   0        0        0     5586 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/filedb.py
--rw-r--r--   0        0        0     1139 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/hooks/__init__.py
--rw-r--r--   0        0        0     1510 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/hooks/base.py
--rw-r--r--   0        0        0     3594 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/hooks/build.py
--rw-r--r--   0        0        0      854 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/hooks/quarto_attributes.py
--rw-r--r--   0        0        0     3280 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/hooks/task.py
--rw-r--r--   0        0        0     1480 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/logging.py
--rw-r--r--   0        0        0     1471 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/main.py
--rw-r--r--   0        0        0     5574 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/markdown_reader.py
--rw-r--r--   0        0        0     5511 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/parsing.py
--rw-r--r--   0        0        0     2486 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/properties.py
--rw-r--r--   0        0        0        0 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/py.typed
--rw-r--r--   0        0        0      888 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/status.py
--rw-r--r--   0        0        0     3768 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/tangle.py
--rw-r--r--   0        0        0      187 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/text_location.py
--rw-r--r--   0        0        0     6971 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/transaction.py
--rw-r--r--   0        0        0      717 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/utility.py
--rw-r--r--   0        0        0       85 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/entangled/version.py
--rw-r--r--   0        0        0     1344 2023-11-18 22:44:01.312597 entangled_cli-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    15885 1970-01-01 00:00:00.000000 entangled_cli-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 14:29:23.540717 entangled_cli-2.0.3/LICENSE
+-rw-r--r--   0        0        0    15054 2024-05-15 14:29:23.540717 entangled_cli-2.0.3/README.md
+-rw-r--r--   0        0        0        1 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/__init__.py
+-rw-r--r--   0        0        0     2500 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/code_reader.py
+-rw-r--r--   0        0        0      279 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/commands/__init__.py
+-rw-r--r--   0        0        0     1356 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/commands/brei.py
+-rw-r--r--   0        0        0     7061 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/commands/new.py
+-rw-r--r--   0        0        0     1671 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/commands/status.py
+-rw-r--r--   0        0        0     2267 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/commands/stitch.py
+-rw-r--r--   0        0        0     1375 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/commands/sync.py
+-rw-r--r--   0        0        0     2277 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/commands/tangle.py
+-rw-r--r--   0        0        0     1714 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/commands/watch.py
+-rw-r--r--   0        0        0     5634 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/config/__init__.py
+-rw-r--r--   0        0        0     1827 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/config/language.py
+-rw-r--r--   0        0        0      768 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/config/templates.py
+-rw-r--r--   0        0        0      368 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/config/version.py
+-rw-r--r--   0        0        0     5445 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/construct.py
+-rw-r--r--   0        0        0     2388 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/document.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/errors/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/errors/internal.py
+-rw-r--r--   0        0        0     1398 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/errors/user.py
+-rw-r--r--   0        0        0     5586 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/filedb.py
+-rw-r--r--   0        0        0     1139 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/hooks/__init__.py
+-rw-r--r--   0        0        0     1510 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/hooks/base.py
+-rw-r--r--   0        0        0     3594 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/hooks/build.py
+-rw-r--r--   0        0        0      854 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/hooks/quarto_attributes.py
+-rw-r--r--   0        0        0     3280 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/hooks/task.py
+-rw-r--r--   0        0        0     1480 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/logging.py
+-rw-r--r--   0        0        0     1471 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/main.py
+-rw-r--r--   0        0        0     5574 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/markdown_reader.py
+-rw-r--r--   0        0        0     5511 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/parsing.py
+-rw-r--r--   0        0        0     2486 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/properties.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/py.typed
+-rw-r--r--   0        0        0      882 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/status.py
+-rw-r--r--   0        0        0     3768 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/tangle.py
+-rw-r--r--   0        0        0      187 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/text_location.py
+-rw-r--r--   0        0        0     6971 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/transaction.py
+-rw-r--r--   0        0        0      717 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/utility.py
+-rw-r--r--   0        0        0       85 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/entangled/version.py
+-rw-r--r--   0        0        0     1379 2024-05-15 14:29:23.544717 entangled_cli-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    15999 1970-01-01 00:00:00.000000 entangled_cli-2.0.3/PKG-INFO
```

### Comparing `entangled_cli-2.0.2/LICENSE` & `entangled_cli-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/README.md` & `entangled_cli-2.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,17 @@
 
 ```toml
 # required: the minimum version of Entangled
 version = "2.0"            
 
 # default watch_list is ["**/*.md"]
 watch_list = ["docs/**/*.md"]
+
+# default ignore_list is ["**/README.md"]
+ignore_list = ["docs/**/examples.md"]
 ```
 
 You may add languages as follows:
 
 ```toml
 [[languages]]
 name = "Java"
```

### Comparing `entangled_cli-2.0.2/entangled/code_reader.py` & `entangled_cli-2.0.3/entangled/code_reader.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/commands/brei.py` & `entangled_cli-2.0.3/entangled/commands/brei.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/commands/new.py` & `entangled_cli-2.0.3/entangled/commands/new.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         return
 
     if not template or not project_path:
         raise HelpfulUserError(
             "Please supply both a [template] and a [project_path].\n", print_help
         )
 
-    copy_this_template: Optional[str] = template
+    copy_this_template: str = template
     trust_this_template: bool = trust
 
     # Use an officially supported template, if available, and trust it
     # If no template is found, treat the "template" var as URL or path for copier
     template_option: Template
     for template_option in AVAILABLE_TEMPLATES:
         if template == template_option.handle:
```

### Comparing `entangled_cli-2.0.2/entangled/commands/status.py` & `entangled_cli-2.0.3/entangled/commands/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 def rich_status():
     config_table = Table()
     config_table.add_column("name")
     config_table.add_column("value")
     config_table.add_row(
         "Watch list", ", ".join(f"'{pat}'" for pat in config.watch_list)
     )
+    config_table.add_row(
+        "Ignore list", ", ".join(f"'{pat}'" for pat in config.ignore_list)
+    )
     config_table.add_row("Hooks enabled", ", ".join(config.hooks))
 
     console = Console(color_system="auto")
     group = Group(
         Panel(config_table, title="config", border_style="dark_cyan"),
         Columns(
             [
```

### Comparing `entangled_cli-2.0.2/entangled/commands/stitch.py` & `entangled_cli-2.0.3/entangled/commands/stitch.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/commands/sync.py` & `entangled_cli-2.0.3/entangled/commands/sync.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/commands/tangle.py` & `entangled_cli-2.0.3/entangled/commands/tangle.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/commands/watch.py` & `entangled_cli-2.0.3/entangled/commands/watch.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/config/__init__.py` & `entangled_cli-2.0.3/entangled/config/__init__.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/config/language.py` & `entangled_cli-2.0.3/entangled/config/language.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,9 +42,10 @@
     Language("Lua", ["lua"], Comment("--")),
     Language("Make", ["make", "makefile"], Comment("#")),
     Language("Gnuplot", ["gnuplot"], Comment("#")),
     Language("TOML", ["toml"], Comment("#")),
     Language("F#", ["fsharp"], Comment("//")),
     Language("Javascript", ["javascript", "js", "ecma"], Comment("//")),
     Language("Go", ["go", "golang"], Comment("//")),
-    Language("R", ["r", "rlang"], Comment("#"))
+    Language("R", ["r", "rlang"], Comment("#")),
+    Language("Nix", ["nix"], Comment("#"))
 ]
```

### Comparing `entangled_cli-2.0.2/entangled/config/templates.py` & `entangled_cli-2.0.3/entangled/config/templates.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/construct.py` & `entangled_cli-2.0.3/entangled/construct.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def from_str(cls, _: str) -> Self:
         raise NotImplementedError()
 
 
 def construct(annot: Any, json: Any) -> Any:
     try:
         return _construct(annot, json)
-    except (AssertionError, ValueError, KeyError) as e:
+    except (AssertionError, ValueError, KeyError, TypeError) as e:
         raise ConfigError(annot, json) from e
 
 
 def is_object_type(dtype: Type[Any]) -> TypeGuard[Type[dict[str, Any]]]:
     return (
         isgeneric(dtype)
         and typing.get_origin(dtype) is dict
@@ -43,14 +43,18 @@
     return (
         isgeneric(dtype)
         and typing.get_origin(dtype) is Union
         and typing.get_args(dtype)[1] is types.NoneType
     )
 
 
+def normalize_enum(x: str):
+    return x.upper().replace("-", "_")
+
+
 def _construct(annot: Type[T], json: Any) -> T:
     """Construct an object from a given type from a JSON stream.
 
     The `annot` type should be one of: str, int, list[T], Optional[T],
     or a dataclass, and the JSON data should match exactly the given
     definitions in the dataclass hierarchy.
     """
@@ -66,22 +70,43 @@
     if is_object_type(annot):
         assert isinstance(json, dict)
         return cast(
             T, {k: construct(typing.get_args(annot)[1], v) for k, v in json.items()}
         )
     if annot is Any:
         return cast(T, json)
-    # if annot is dict or isgeneric(annot) and typing.get_origin(annot) is dict:
-    #    assert isinstance(json, dict)
-    #    return json
-    if annot is Path and isinstance(json, str):
-        return cast(T, Path(json))
+    
+    # dicts
+    if isgeneric(annot) and typing.get_origin(annot) is dict:
+        assert isinstance(json, dict)
+        return cast(T, {construct(typing.get_args(annot)[0], k): construct(typing.get_args(annot)[1], v)
+                        for k, v in json.items()})
+    if annot is dict:
+        assert isinstance(json, dict)
+        return cast(T, json)
+    
+    # lists
     if isgeneric(annot) and typing.get_origin(annot) is list:
         assert isinstance(json, list)
         return cast(T, [construct(typing.get_args(annot)[0], item) for item in json])
+    if annot is list:
+        assert isinstance(json, list)
+        return cast(T, json)
+
+    # sets
+    if isgeneric(annot) and typing.get_origin(annot) is set:
+        assert isinstance(json, list)
+        return cast(T, {construct(typing.get_args(annot)[0], item) for item in json})
+    if annot is set:
+        assert isinstance(json, list)
+        return cast(T, set(json))
+
+    if annot is Path and isinstance(json, str):
+        return cast(T, Path(json))
+    
     if is_optional_type(annot):
         if json is None:
             return cast(T, None)
         else:
             return cast(T, construct(typing.get_args(annot)[0], json))
     if isgeneric(annot) and typing.get_origin(annot) is types.UnionType:
         for dtype in typing.get_args(annot):
@@ -93,21 +118,21 @@
                 continue
         raise ValueError("None of the choices in type union match data.")
     if type(annot) is type and issubclass(annot, FromStr) and isinstance(json, str):
         return cast(T, annot.from_str(json))
     if is_dataclass(annot):
         assert isinstance(json, dict)
         arg_annot = typing.get_type_hints(annot)
-        # assert all(k in json for k in arg_annot)
         args = {k: construct(arg_annot[k], json[k]) for k in json}
         return cast(T, annot(**args))
     if isinstance(json, str) and isinstance(annot, type) and issubclass(annot, Enum):
-        options = {opt.name.lower(): opt for opt in annot}
-        assert json.lower() in options
-        return cast(T, options[json.lower()])
+        options = {normalize_enum(e.name): e for e in annot}
+        assert isinstance(json, str)
+        assert normalize_enum(json) in options
+        return cast(T, options[normalize_enum(json)])
     raise ValueError(f"Couldn't construct {annot} from {repr(json)}")
 
 
 def read_from_file(data_type: Type[T], path: Path, section: Optional[str] = None) -> T:
     """Read a config from given `path` in given `section`. The path should refer to
     a TOML or JSON file that should decode to a `Config` object. If `section` is given, only
     that section is decoded to a `Config` object. The `section` string may contain
```

### Comparing `entangled_cli-2.0.2/entangled/document.py` & `entangled_cli-2.0.3/entangled/document.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/errors/internal.py` & `entangled_cli-2.0.3/entangled/errors/internal.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/errors/user.py` & `entangled_cli-2.0.3/entangled/errors/user.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/filedb.py` & `entangled_cli-2.0.3/entangled/filedb.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/hooks/__init__.py` & `entangled_cli-2.0.3/entangled/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/hooks/base.py` & `entangled_cli-2.0.3/entangled/hooks/base.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/hooks/build.py` & `entangled_cli-2.0.3/entangled/hooks/build.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/hooks/quarto_attributes.py` & `entangled_cli-2.0.3/entangled/hooks/quarto_attributes.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/hooks/task.py` & `entangled_cli-2.0.3/entangled/hooks/task.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/logging.py` & `entangled_cli-2.0.3/entangled/logging.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/main.py` & `entangled_cli-2.0.3/entangled/main.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/markdown_reader.py` & `entangled_cli-2.0.3/entangled/markdown_reader.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/parsing.py` & `entangled_cli-2.0.3/entangled/parsing.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/properties.py` & `entangled_cli-2.0.3/entangled/properties.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/status.py` & `entangled_cli-2.0.3/entangled/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     with file_db(readonly=True) as db:
         code_dirs = set(p.parent for p in db.managed)
     return code_dirs.union(markdown_dirs)
 
 
 def list_input_files():
     """List all input files."""
-    include_file_list = chain.from_iterable(map(Path(".").glob, config.watch_list))
+    include_file_list = chain.from_iterable(map(Path().glob, config.watch_list))
     exclude_file_list = list(
-        chain.from_iterable(map(Path(".").glob, config.ignore_list))
+        chain.from_iterable(map(Path().glob, config.ignore_list))
     )
     return [path for path in include_file_list if not path in exclude_file_list]
 
 
 def list_dependent_files():
     with file_db(readonly=True) as db:
         result = list(db.managed)
```

### Comparing `entangled_cli-2.0.2/entangled/tangle.py` & `entangled_cli-2.0.3/entangled/tangle.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/transaction.py` & `entangled_cli-2.0.3/entangled/transaction.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/entangled/utility.py` & `entangled_cli-2.0.3/entangled/utility.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.2/pyproject.toml` & `entangled_cli-2.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "entangled-cli"
-version = "2.0.2"
+version = "2.0.3"
 description = "Literate Programming toolbox"
 repository = "https://github.com/entangled/entangled.py"
 homepage = "https://entangled.github.io/"
 authors = ["Johan Hidding <j.hidding@esciencecenter.nl>"]
 license = "Apache 2"
 readme = "README.md"
 packages = [{ include = "entangled" }]
@@ -13,28 +13,30 @@
 python = "^3.11"
 mawk = "^0.1.4"          # use mawk as line parsing engine
 watchdog = "^3.0.0"      # file watching
 filelock = "^3.12.0"     # file lock for json db
 argh = "^0.30"           # easy argument parsing
 rich = "^13.3.5"         # colourful output
 tomlkit = "^0.12.1"      # read/write toml files
-copier = "^8.3.0"        # project templates
+copier = "^9"            # project templates
 brei = "^0.2.3"          # build system
 rich-argparse = "^1.4.0" # colourful help messages
+pexpect = "^4.9.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 mypy = "^1.3.0"
 black = "^23.3.0"
 pytest-cov = "^4.0.0"
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.13"
 mkdocstrings = { extras = ["python"], version = "^0.21.2" }
 twine = "^4.0.2"
 pytest-asyncio = "^0.21.1"
+ruff = "^0.4.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = ["test"]
```

### Comparing `entangled_cli-2.0.2/PKG-INFO` & `entangled_cli-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: entangled-cli
-Version: 2.0.2
+Version: 2.0.3
 Summary: Literate Programming toolbox
 Home-page: https://entangled.github.io/
 License: Apache 2
 Author: Johan Hidding
 Author-email: j.hidding@esciencecenter.nl
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argh (>=0.30,<0.31)
 Requires-Dist: brei (>=0.2.3,<0.3.0)
-Requires-Dist: copier (>=8.3.0,<9.0.0)
+Requires-Dist: copier (>=9,<10)
 Requires-Dist: filelock (>=3.12.0,<4.0.0)
 Requires-Dist: mawk (>=0.1.4,<0.2.0)
+Requires-Dist: pexpect (>=4.9.0,<5.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: rich-argparse (>=1.4.0,<2.0.0)
 Requires-Dist: tomlkit (>=0.12.1,<0.13.0)
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/entangled/entangled.py
 Description-Content-Type: text/markdown
 
@@ -118,14 +119,17 @@
 
 ```toml
 # required: the minimum version of Entangled
 version = "2.0"            
 
 # default watch_list is ["**/*.md"]
 watch_list = ["docs/**/*.md"]
+
+# default ignore_list is ["**/README.md"]
+ignore_list = ["docs/**/examples.md"]
 ```
 
 You may add languages as follows:
 
 ```toml
 [[languages]]
 name = "Java"
```

