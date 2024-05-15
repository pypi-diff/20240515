# Comparing `tmp/rlbot_flatbuffers-0.3.5.tar.gz` & `tmp/rlbot_flatbuffers-0.3.6.tar.gz`

## Comparing `rlbot_flatbuffers-0.3.5.tar` & `rlbot_flatbuffers-0.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.5/Cargo.toml
--rw-r--r--   0     1001      127     1070 2024-05-14 21:23:39.000000 rlbot_flatbuffers-0.3.5/LICENSE
--rw-r--r--   0     1001      127      479 2024-05-14 21:23:39.000000 rlbot_flatbuffers-0.3.5/README.md
--rw-r--r--   0     1001      127    61922 2024-05-14 21:23:39.000000 rlbot_flatbuffers-0.3.5/build.rs
--rw-r--r--   0     1001      127      182 2024-05-14 21:23:40.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/README.md
--rw-r--r--   0     1001      127      401 2024-05-14 21:23:40.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/comms.fbs
--rw-r--r--   0     1001      127     1932 2024-05-14 21:23:40.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/event.fbs
--rwxr-xr-x   0     1001      127  6685928 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/flatc
--rw-r--r--   0     1001      127  3488256 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/flatc.exe
--rwxr-xr-x   0     1001      127  6896752 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/flatc_mac
--rw-r--r--   0     1001      127     1281 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/gamestate.fbs
--rw-r--r--   0     1001      127     5824 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/matchstart.fbs
--rw-r--r--   0     1001      127     1162 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/rendering.fbs
--rw-r--r--   0     1001      127     6296 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/rlbot.fbs
--rw-r--r--   0     1001      127     5543 2024-05-14 21:23:39.000000 rlbot_flatbuffers-0.3.5/src/lib.rs
--rw-r--r--   0     1001      127    13114 2024-05-14 21:23:39.000000 rlbot_flatbuffers-0.3.5/Cargo.lock
--rw-r--r--   0     1001      127      418 2024-05-14 21:23:39.000000 rlbot_flatbuffers-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.6/Cargo.toml
+-rw-r--r--   0     1001      127     1070 2024-05-15 05:32:42.000000 rlbot_flatbuffers-0.3.6/LICENSE
+-rw-r--r--   0     1001      127     2443 2024-05-15 05:32:42.000000 rlbot_flatbuffers-0.3.6/README.md
+-rw-r--r--   0     1001      127    62107 2024-05-15 05:32:42.000000 rlbot_flatbuffers-0.3.6/build.rs
+-rw-r--r--   0     1001      127      182 2024-05-15 05:32:44.000000 rlbot_flatbuffers-0.3.6/flatbuffers-schema/README.md
+-rw-r--r--   0     1001      127      401 2024-05-15 05:32:44.000000 rlbot_flatbuffers-0.3.6/flatbuffers-schema/comms.fbs
+-rw-r--r--   0     1001      127     1932 2024-05-15 05:32:44.000000 rlbot_flatbuffers-0.3.6/flatbuffers-schema/event.fbs
+-rwxr-xr-x   0     1001      127  6685928 2024-05-15 05:32:44.000000 rlbot_flatbuffers-0.3.6/flatbuffers-schema/flatc
+-rw-r--r--   0     1001      127  3488256 2024-05-15 05:32:44.000000 rlbot_flatbuffers-0.3.6/flatbuffers-schema/flatc.exe
+-rwxr-xr-x   0     1001      127  6896752 2024-05-15 05:32:44.000000 rlbot_flatbuffers-0.3.6/flatbuffers-schema/flatc_mac
+-rw-r--r--   0     1001      127     1281 2024-05-15 05:32:44.000000 rlbot_flatbuffers-0.3.6/flatbuffers-schema/gamestate.fbs
+-rw-r--r--   0     1001      127     5824 2024-05-15 05:32:44.000000 rlbot_flatbuffers-0.3.6/flatbuffers-schema/matchstart.fbs
+-rw-r--r--   0     1001      127     1162 2024-05-15 05:32:44.000000 rlbot_flatbuffers-0.3.6/flatbuffers-schema/rendering.fbs
+-rw-r--r--   0     1001      127     6296 2024-05-15 05:32:44.000000 rlbot_flatbuffers-0.3.6/flatbuffers-schema/rlbot.fbs
+-rw-r--r--   0     1001      127     5543 2024-05-15 05:32:42.000000 rlbot_flatbuffers-0.3.6/src/lib.rs
+-rw-r--r--   0     1001      127    13114 2024-05-15 05:32:42.000000 rlbot_flatbuffers-0.3.6/Cargo.lock
+-rw-r--r--   0     1001      127      418 2024-05-15 05:32:42.000000 rlbot_flatbuffers-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.6/PKG-INFO
```

### Comparing `rlbot_flatbuffers-0.3.5/Cargo.toml` & `rlbot_flatbuffers-0.3.6/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 name = "rlbot-flatbuffers-py"
-version = "0.3.5"
+version = "0.3.6"
 edition = "2021"
 description = "A Python module implemented in Rust for serializing and deserializing RLBot's flatbuffers"
-repository = "https://github.com/VirxEC/rlbot-flatbuffers-py"
+repository = "https://github.com/VirxEC/rlbot_flatbuffers_py"
 license = "MIT"
 readme = "README.md"
 exclude = [".github", "pytest.py", "rustfmt.toml", ".gitignore", ".gitmodules"]
 publish = false
 
 [lints.clippy]
 all = "warn"
```

### Comparing `rlbot_flatbuffers-0.3.5/LICENSE` & `rlbot_flatbuffers-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.5/build.rs` & `rlbot_flatbuffers-0.3.6/build.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1360,24 +1360,26 @@
                     file_contents.push(Cow::Owned(format!("    {variable_name}: {type_name}")));
                 } else {
                     python_types.push(variable_type.clone());
                     file_contents.push(Cow::Owned(format!("    {variable_name}: {variable_type}")));
                 }
             }
 
-            file_contents.push(Cow::Borrowed(""));
-
-            if is_enum {
+            if types.is_empty() {
+                file_contents.push(Cow::Borrowed("    def __init__(self): ..."));
+            } else if is_enum {
+                file_contents.push(Cow::Borrowed(""));
                 file_contents.push(Cow::Borrowed("    def __init__(self, value: int = 0):"));
                 file_contents.push(Cow::Borrowed("        \"\"\""));
                 file_contents.push(Cow::Borrowed(
                     "        :raises ValueError: If the `value` is not a valid enum value",
                 ));
-                file_contents.push(Cow::Borrowed("        \"\"\""));
+                file_contents.push(Cow::Borrowed("        \"\"\"\n"));
             } else {
+                file_contents.push(Cow::Borrowed(""));
                 file_contents.push(Cow::Borrowed("    def __init__("));
                 file_contents.push(Cow::Borrowed("        self,"));
 
                 let mut i = 0;
                 for variable_info in types {
                     if &variable_info[0] == "NONE" {
                         continue;
@@ -1403,15 +1405,15 @@
                             } else {
                                 Cow::Owned(format!("{}()", t.trim_end_matches('T')))
                             }
                         }
                     };
 
                     let python_type = &python_types[i];
-                    file_contents.push(Cow::Owned(format!("        {variable_name}: {python_type}={default_value},")));
+                    file_contents.push(Cow::Owned(format!("        {variable_name}: {python_type} = {default_value},")));
 
                     i += 1;
                 }
 
                 file_contents.push(Cow::Borrowed("    ): ..."));
             }
         }
```

### Comparing `rlbot_flatbuffers-0.3.5/flatbuffers-schema/event.fbs` & `rlbot_flatbuffers-0.3.6/flatbuffers-schema/event.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.5/flatbuffers-schema/flatc` & `rlbot_flatbuffers-0.3.6/flatbuffers-schema/flatc`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.5/flatbuffers-schema/flatc.exe` & `rlbot_flatbuffers-0.3.6/flatbuffers-schema/flatc.exe`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.5/flatbuffers-schema/flatc_mac` & `rlbot_flatbuffers-0.3.6/flatbuffers-schema/flatc_mac`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.5/flatbuffers-schema/gamestate.fbs` & `rlbot_flatbuffers-0.3.6/flatbuffers-schema/gamestate.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.5/flatbuffers-schema/matchstart.fbs` & `rlbot_flatbuffers-0.3.6/flatbuffers-schema/matchstart.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.5/flatbuffers-schema/rendering.fbs` & `rlbot_flatbuffers-0.3.6/flatbuffers-schema/rendering.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.5/flatbuffers-schema/rlbot.fbs` & `rlbot_flatbuffers-0.3.6/flatbuffers-schema/rlbot.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.5/src/lib.rs` & `rlbot_flatbuffers-0.3.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.5/Cargo.lock` & `rlbot_flatbuffers-0.3.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -325,15 +325,15 @@
 checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "rlbot-flatbuffers-py"
-version = "0.3.5"
+version = "0.3.6"
 dependencies = [
  "flatbuffers",
  "get-size",
  "pyo3",
  "serde",
 ]
```

