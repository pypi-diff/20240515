# Comparing `tmp/poetry_stale_dependencies-0.2.1.tar.gz` & `tmp/poetry_stale_dependencies-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_stale_dependencies-0.2.1.tar", max compression
+gzip compressed data, was "poetry_stale_dependencies-0.2.2.tar", max compression
```

## Comparing `poetry_stale_dependencies-0.2.1.tar` & `poetry_stale_dependencies-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2049 2024-05-12 13:30:47.299851 poetry_stale_dependencies-0.2.1/LICENSE
--rw-r--r--   0        0        0     1369 2024-05-12 13:30:47.299851 poetry_stale_dependencies-0.2.1/README.md
--rw-r--r--   0        0        0       86 2024-05-12 13:30:47.299851 poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/__init__.py
--rw-r--r--   0        0        0       22 2024-05-12 13:31:05.203773 poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/_version.py
--rw-r--r--   0        0        0     4057 2024-05-12 13:30:47.299851 poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/config.py
--rw-r--r--   0        0        0     7306 2024-05-12 13:30:47.299851 poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/inspections.py
--rw-r--r--   0        0        0     4655 2024-05-12 13:30:47.299851 poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/lock_spec.py
--rw-r--r--   0        0        0     5581 2024-05-12 13:30:47.299851 poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/plugin.py
--rw-r--r--   0        0        0     2911 2024-05-12 13:30:47.299851 poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/project_spec.py
--rw-r--r--   0        0        0     7386 2024-05-12 13:30:47.299851 poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/remote.py
--rw-r--r--   0        0        0      575 2024-05-12 13:30:47.299851 poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/util.py
--rw-r--r--   0        0        0     3424 2024-05-12 13:30:47.299851 poetry_stale_dependencies-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 poetry_stale_dependencies-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2049 2024-05-15 10:56:15.601327 poetry_stale_dependencies-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1369 2024-05-15 10:56:15.601327 poetry_stale_dependencies-0.2.2/README.md
+-rw-r--r--   0        0        0       86 2024-05-15 10:56:15.601327 poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-15 10:56:33.953368 poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/_version.py
+-rw-r--r--   0        0        0     4057 2024-05-15 10:56:15.601327 poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/config.py
+-rw-r--r--   0        0        0     7359 2024-05-15 10:56:15.605327 poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/inspections.py
+-rw-r--r--   0        0        0     5155 2024-05-15 10:56:15.605327 poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/lock_spec.py
+-rw-r--r--   0        0        0     5581 2024-05-15 10:56:15.605327 poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/plugin.py
+-rw-r--r--   0        0        0     3043 2024-05-15 10:56:15.605327 poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/project_spec.py
+-rw-r--r--   0        0        0     7386 2024-05-15 10:56:15.605327 poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/remote.py
+-rw-r--r--   0        0        0      575 2024-05-15 10:56:15.605327 poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/util.py
+-rw-r--r--   0        0        0     3424 2024-05-15 10:56:15.605327 poetry_stale_dependencies-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 poetry_stale_dependencies-0.2.2/PKG-INFO
```

### Comparing `poetry_stale_dependencies-0.2.1/LICENSE` & `poetry_stale_dependencies-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_stale_dependencies-0.2.1/README.md` & `poetry_stale_dependencies-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/config.py` & `poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/config.py`

 * *Files identical despite different names*

### Comparing `poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/inspections.py` & `poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/inspections.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,16 @@
                     else:
                         break
 
                 dependencies: list[tuple[str, PackageDependency | ProjectDependency]] = [
                     (package_name, package_dep)
                     for package_name, package_specs in lock_spec.packages.items()
                     for package_spec in package_specs
-                    if (package_dep := package_spec.dependencies.get(self.package)) is not None
+                    if (package_deps := package_spec.dependencies.get(self.package)) is not None
+                    for package_dep in package_deps
                 ]
 
                 for group_name, group in project_spec.dependencies_groups.items():
                     if (group_deps := group.get(self.package)) is not None:
                         for project_dep in group_deps:
                             if group_name == "main":
                                 group_desc = project_spec.name
```

### Comparing `poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/lock_spec.py` & `poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/lock_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,36 +35,38 @@
 
 @dataclass
 class PackageDependency:
     version_req: str
     marker: str | None | UnkownMarker
 
     @classmethod
-    def from_raw(cls, raw: Any) -> PackageDependency | None:
+    def from_raw(cls, raw: object) -> PackageDependency | None:
         if isinstance(raw, str):
             return cls(raw, None)
+        if isinstance(raw, dict):
+            version = raw.get("version")
+            if version is None:
+                return None
+            raw_marker = raw.get("markers")
+            is_optional = raw.get("optional", False)
+            marker: str | None | UnkownMarker
+            if is_optional and raw_marker is None:
+                marker = unknown_marker
+            else:
+                marker = raw_marker
 
-        version = raw.get("version")
-        if version is None:
-            return None
-        raw_marker = raw.get("markers")
-        is_optional = raw.get("optional", False)
-        if is_optional and raw_marker is None:
-            marker = unknown_marker
-        else:
-            marker = raw_marker
-
-        return cls(version, marker)
+            return cls(version, marker)
+        return None
 
 
 @dataclass
 class PackageSpec:
     version: str
     source: LegacyPackageSource | None
-    dependencies: Mapping[PackageName, PackageDependency]
+    dependencies: Mapping[PackageName, Sequence[PackageDependency]]
 
 
 @dataclass
 class LockSpec:
     packages: dict[PackageName, list[PackageSpec]] = field(default_factory=dict)
 
     def get_packages(
@@ -120,17 +122,25 @@
                     url=raw_source.get("url"),
                     reference=raw_source.get("reference"),
                 )
 
             dependencies = {}
             if raw_dependencies := package.get("dependencies"):
                 for dep_name, dep_raw in raw_dependencies.items():
-                    if dep := PackageDependency.from_raw(dep_raw):
-                        dependencies[dep_name] = dep
+                    if isinstance(dep_raw, list):
+                        deps_raw = dep_raw
                     else:
-                        com.line_error(
-                            f"Invalid dependency {dep_name!r} for package {name}, ignoring",
-                            verbosity=Verbosity.NORMAL,
-                        )
+                        deps_raw = [dep_raw]
+                    deps = []
+                    for dep_raw_item in deps_raw:
+                        if dep := PackageDependency.from_raw(dep_raw_item):
+                            deps.append(dep)
+                        else:
+                            com.line_error(
+                                f"Invalid dependency {dep_name!r} for package {name}, ignoring",
+                                verbosity=Verbosity.NORMAL,
+                            )
+                    if deps:
+                        dependencies[dep_name] = deps
 
             packages.setdefault(to_package_name(name), []).append(PackageSpec(version, source, dependencies))
         return cls(packages)
```

### Comparing `poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/plugin.py` & `poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/project_spec.py` & `poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/project_spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,39 +11,40 @@
 
 @dataclass
 class ProjectDependency:
     version_req: str
     marker: str | None | UnkownMarker
 
     @classmethod
-    def from_raw(cls, raw: Any) -> ProjectDependency | None:
+    def from_raw(cls, raw: object) -> ProjectDependency | None:
         if isinstance(raw, str):
             return cls(raw, None)
+        if isinstance(raw, dict):
+            version = raw.get("version")
+            if version is None:
+                return None
+            marker_parts = []
+            raw_marker = raw.get("markers")
+            if raw_marker is not None:
+                marker_parts.append(raw_marker)
+            python = raw.get("python")
+            if python is not None:
+                marker_parts.append(f"python_version{python}")
+
+            is_optional = raw.get("optional", False)
+            marker: str | None | UnkownMarker
+            if is_optional and not marker_parts:
+                marker = unknown_marker
+            elif not marker_parts:
+                marker = None
+            else:
+                marker = " and ".join(marker_parts)
 
-        version = raw.get("version")
-        if version is None:
-            return None
-        marker_parts = []
-        raw_marker = raw.get("markers")
-        if raw_marker is not None:
-            marker_parts.append(raw_marker)
-        python = raw.get("python")
-        if python is not None:
-            marker_parts.append(f"python_version{python}")
-
-        is_optional = raw.get("optional", False)
-        marker: str | None | UnkownMarker
-        if is_optional and not marker_parts:
-            marker = unknown_marker
-        elif not marker_parts:
-            marker = None
-        else:
-            marker = " and ".join(marker_parts)
-
-        return cls(version, marker)
+            return cls(version, marker)
+        return None
 
 
 @dataclass
 class ProjectSpec:
     name: str = "root"
     dependencies_groups: dict[str, dict[PackageName, list[ProjectDependency]]] = field(default_factory=dict)
```

### Comparing `poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/remote.py` & `poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/remote.py`

 * *Files identical despite different names*

### Comparing `poetry_stale_dependencies-0.2.1/poetry_stale_dependencies/util.py` & `poetry_stale_dependencies-0.2.2/poetry_stale_dependencies/util.py`

 * *Files identical despite different names*

### Comparing `poetry_stale_dependencies-0.2.1/pyproject.toml` & `poetry_stale_dependencies-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-stale-dependencies"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 readme = "README.md"
 authors = ["Biocatch LTD <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 poetry = "^1.7.1"
```

### Comparing `poetry_stale_dependencies-0.2.1/PKG-INFO` & `poetry_stale_dependencies-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-stale-dependencies
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Biocatch LTD
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

