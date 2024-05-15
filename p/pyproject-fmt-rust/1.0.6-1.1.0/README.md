# Comparing `tmp/pyproject_fmt_rust-1.0.6.tar.gz` & `tmp/pyproject_fmt_rust-1.1.0.tar.gz`

## Comparing `pyproject_fmt_rust-1.0.6.tar` & `pyproject_fmt_rust-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.6/Cargo.toml
--rw-r--r--   0     1001      127       36 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.github/FUNDING.yml
--rw-r--r--   0     1001      127      365 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.github/SECURITY.md
--rw-r--r--   0     1001      127      117 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.github/dependabot.yml
--rw-r--r--   0     1001      127       76 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.github/release.yml
--rw-r--r--   0     1001      127     2248 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.github/workflows/check.yml
--rw-r--r--   0     1001      127     3714 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.github/workflows/release.yml
--rw-r--r--   0     1001      127      158 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.gitignore
--rw-r--r--   0     1001      127      973 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      240 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.pre-commit-hooks.yaml
--rw-r--r--   0     1001      127       16 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.rustfmt.toml
--rw-r--r--   0     1001      127     3256 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127     1023 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/LICENSE.txt
--rw-r--r--   0     1001      127      861 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/README.md
--rw-r--r--   0     1001      127     3370 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/build_system.rs
--rw-r--r--   0     1001      127     3755 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/global.rs
--rw-r--r--   0     1001      127     8964 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/helpers/array.rs
--rw-r--r--   0     1001      127     4529 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/helpers/create.rs
--rw-r--r--   0     1001      127       78 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/helpers/mod.rs
--rw-r--r--   0     1001      127     4595 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/helpers/pep508.rs
--rw-r--r--   0     1001      127     1605 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/helpers/string.rs
--rw-r--r--   0     1001      127     9369 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/helpers/table.rs
--rw-r--r--   0     1001      127     5748 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/main.rs
--rw-r--r--   0     1001      127    30490 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/project.rs
--rw-r--r--   0     1001      127       29 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust-toolchain.toml
--rw-r--r--   0     1001      127      161 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/src/pyproject_fmt_rust/__init__.py
--rw-r--r--   0     1001      127      638 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/src/pyproject_fmt_rust/_lib.pyi
--rw-r--r--   0     1001      127        0 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/src/pyproject_fmt_rust/py.typed
--rw-r--r--   0     1001      127      991 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/tests/test_main.py
--rw-r--r--   0     1001      127     2081 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/tox.ini
--rw-r--r--   0     1001      127    26478 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/Cargo.lock
--rw-r--r--   0     1001      127     3312 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.1.0/Cargo.toml
+-rw-r--r--   0     1001      127       36 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/.github/FUNDING.yml
+-rw-r--r--   0     1001      127      365 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/.github/SECURITY.md
+-rw-r--r--   0     1001      127      117 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/.github/dependabot.yml
+-rw-r--r--   0     1001      127       76 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/.github/release.yml
+-rw-r--r--   0     1001      127     2248 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/.github/workflows/check.yml
+-rw-r--r--   0     1001      127     3714 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      158 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/.gitignore
+-rw-r--r--   0     1001      127      973 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      240 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/.pre-commit-hooks.yaml
+-rw-r--r--   0     1001      127       16 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/.rustfmt.toml
+-rw-r--r--   0     1001      127     3256 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127     1023 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/LICENSE.txt
+-rw-r--r--   0     1001      127      861 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/README.md
+-rw-r--r--   0     1001      127     3185 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/build_system.rs
+-rw-r--r--   0     1001      127     3447 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/data/ruff-order.expected.toml
+-rw-r--r--   0     1001      127     3281 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/data/ruff-order.start.toml
+-rw-r--r--   0     1001      127     3755 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/global.rs
+-rw-r--r--   0     1001      127     8964 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/helpers/array.rs
+-rw-r--r--   0     1001      127     4529 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/helpers/create.rs
+-rw-r--r--   0     1001      127       78 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/helpers/mod.rs
+-rw-r--r--   0     1001      127     4595 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/helpers/pep508.rs
+-rw-r--r--   0     1001      127     1605 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/helpers/string.rs
+-rw-r--r--   0     1001      127    11333 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/helpers/table.rs
+-rw-r--r--   0     1001      127     6416 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/main.rs
+-rw-r--r--   0     1001      127    30465 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/project.rs
+-rw-r--r--   0     1001      127     8213 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust/src/ruff.rs
+-rw-r--r--   0     1001      127       29 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/rust-toolchain.toml
+-rw-r--r--   0     1001      127      161 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/src/pyproject_fmt_rust/__init__.py
+-rw-r--r--   0     1001      127      638 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/src/pyproject_fmt_rust/_lib.pyi
+-rw-r--r--   0     1001      127        0 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/src/pyproject_fmt_rust/py.typed
+-rw-r--r--   0     1001      127      991 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/tests/test_main.py
+-rw-r--r--   0     1001      127     2081 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/tox.ini
+-rw-r--r--   0     1001      127    26478 2024-05-14 21:02:39.000000 pyproject_fmt_rust-1.1.0/Cargo.lock
+-rw-r--r--   0     1001      127     3312 2024-05-14 21:02:26.000000 pyproject_fmt_rust-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.1.0/PKG-INFO
```

### Comparing `pyproject_fmt_rust-1.0.6/Cargo.toml` & `pyproject_fmt_rust-1.1.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyproject-fmt-rust"
-version = "1.0.6"
+version = "1.1.0"
 description = "Format pyproject.toml files"
 repository = "https://github.com/tox-dev/pyproject-fmt"
 readme = "README.md"
 license = "MIT"
 edition = "2021"
 
 [lib]
```

### Comparing `pyproject_fmt_rust-1.0.6/.github/workflows/check.yml` & `pyproject_fmt_rust-1.1.0/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/.github/workflows/release.yml` & `pyproject_fmt_rust-1.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/.pre-commit-config.yaml` & `pyproject_fmt_rust-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/CODE_OF_CONDUCT.md` & `pyproject_fmt_rust-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/LICENSE.txt` & `pyproject_fmt_rust-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/README.md` & `pyproject_fmt_rust-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/rust/src/build_system.rs` & `pyproject_fmt_rust-1.1.0/rust/src/build_system.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 use crate::helpers::array::{sort, transform};
 use crate::helpers::pep508::{format_requirement, get_canonic_requirement_name};
 use crate::helpers::table::{for_entries, reorder_table_keys, Tables};
 
-pub fn fix_build(tables: &mut Tables, keep_full_version: bool) {
+pub fn fix(tables: &mut Tables, keep_full_version: bool) {
     let table_element = tables.get(&String::from("build-system"));
     if table_element.is_none() {
         return;
     }
-    let table = &mut table_element.unwrap().borrow_mut();
+    let table = &mut table_element.unwrap().first().unwrap().borrow_mut();
     for_entries(table, &mut |key, entry| match key.as_str() {
         "requires" => {
             transform(entry, &|s| format_requirement(s, keep_full_version));
             sort(entry, |e| get_canonic_requirement_name(e).to_lowercase());
         }
         "backend-path" => {
             sort(entry, str::to_lowercase);
@@ -25,22 +25,22 @@
 mod tests {
     use indoc::indoc;
     use rstest::rstest;
     use taplo::formatter::{format_syntax, Options};
     use taplo::parser::parse;
     use taplo::syntax::SyntaxElement;
 
-    use crate::build_system::fix_build;
+    use crate::build_system::fix;
     use crate::helpers::table::Tables;
 
     fn evaluate(start: &str, keep_full_version: bool) -> String {
         let root_ast = parse(start).into_syntax().clone_for_update();
         let count = root_ast.children_with_tokens().count();
         let mut tables = Tables::from_ast(&root_ast);
-        fix_build(&mut tables, keep_full_version);
+        fix(&mut tables, keep_full_version);
         let entries = tables
             .table_set
             .iter()
             .flat_map(|e| e.borrow().clone())
             .collect::<Vec<SyntaxElement>>();
         root_ast.splice_children(0..count, entries);
         let opt = Options {
@@ -80,42 +80,37 @@
     requires = [
       "a>=1.0.0",
       "b-c>=1.5.0",
     ]
     "#},
         true
     )]
-    // #[case::build_system_order(
-    // indoc ! {r#"
-    // [build-system]
-    // # more
-    // more = true # more post
-    // #  extra
-    // extra = 1 # extra post
-    // # path
-    // backend-path = ['A'] # path post
-    // # requires
-    // requires = ["B"] # requires post
-    // # backend
-    // build-backend = "hatchling.build" # backend post
-    // # post
-    // "#},
-    // indoc ! {r#"
-    // [build-system]
-    // # more
-    // build-backend = "hatchling.build" # backend post
-    // # post
-    // requires = ["b"] # requires post
-    // # backend
-    // backend-path = ['A'] # path post
-    // # requires
-    // more = true # more post
-    // #  extra
-    // extra = 1 # extra post
-    // # path
-    // "#},
-    // true
-    // )]
-    fn test_normalize_requirement(#[case] start: &str, #[case] expected: &str, #[case] keep_full_version: bool) {
+    #[case::join(
+        indoc ! {r#"
+    [build-system]
+    requires=["a"]
+    [build-system]
+    build-backend = "hatchling.build"
+    [[build-system.a]]
+    name = "Hammer"
+    [[build-system.a]]  # empty table within the array
+    [[build-system.a]]
+    name = "Nail"
+    "#},
+        indoc ! {r#"
+    [build-system]
+    build-backend = "hatchling.build"
+    requires = [
+      "a",
+    ]
+    [[build-system.a]]
+    name = "Hammer"
+    [[build-system.a]] # empty table within the array
+    [[build-system.a]]
+    name = "Nail"
+    "#},
+        false
+    )]
+    fn test_format_build_systems(#[case] start: &str, #[case] expected: &str, #[case] keep_full_version: bool) {
         assert_eq!(evaluate(start, keep_full_version), expected);
     }
 }
```

### Comparing `pyproject_fmt_rust-1.0.6/rust/src/global.rs` & `pyproject_fmt_rust-1.1.0/rust/src/global.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/rust/src/helpers/array.rs` & `pyproject_fmt_rust-1.1.0/rust/src/helpers/array.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/rust/src/helpers/create.rs` & `pyproject_fmt_rust-1.1.0/rust/src/helpers/create.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/rust/src/helpers/pep508.rs` & `pyproject_fmt_rust-1.1.0/rust/src/helpers/pep508.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/rust/src/helpers/string.rs` & `pyproject_fmt_rust-1.1.0/rust/src/helpers/string.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/rust/src/helpers/table.rs` & `pyproject_fmt_rust-1.1.0/rust/src/helpers/table.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,72 @@
 use std::cell::{RefCell, RefMut};
 use std::collections::HashMap;
 use std::iter::zip;
+use std::ops::Index;
 
 use taplo::syntax::SyntaxKind::{TABLE_ARRAY_HEADER, TABLE_HEADER};
 use taplo::syntax::{SyntaxElement, SyntaxKind, SyntaxNode};
 use taplo::HashSet;
 
 use crate::helpers::create::{make_empty_newline, make_key, make_newline, make_table_entry};
 use crate::helpers::string::load_text;
 
 #[derive(Debug)]
 pub struct Tables {
-    pub header_to_pos: HashMap<String, usize>,
+    pub header_to_pos: HashMap<String, Vec<usize>>,
     pub table_set: Vec<RefCell<Vec<SyntaxElement>>>,
 }
 
 impl Tables {
-    pub(crate) fn get(&mut self, key: &str) -> Option<&RefCell<Vec<SyntaxElement>>> {
+    pub(crate) fn get(&mut self, key: &str) -> Option<Vec<&RefCell<Vec<SyntaxElement>>>> {
         if self.header_to_pos.contains_key(key) {
-            Some(&self.table_set[self.header_to_pos[key]])
+            let mut res = Vec::<&RefCell<Vec<SyntaxElement>>>::new();
+            for pos in &self.header_to_pos[key] {
+                res.push(&self.table_set[*pos]);
+            }
+            Some(res)
         } else {
             None
         }
     }
 
     pub fn from_ast(root_ast: &SyntaxNode) -> Self {
-        let mut header_to_pos = HashMap::<String, usize>::new();
+        let mut header_to_pos = HashMap::<String, Vec<usize>>::new();
         let mut table_set = Vec::<RefCell<Vec<SyntaxElement>>>::new();
         let entry_set = RefCell::new(Vec::<SyntaxElement>::new());
-        let mut add_to_table_set = || {
+        let mut table_kind = TABLE_HEADER;
+        let mut add_to_table_set = |kind| {
             let mut entry_set_borrow = entry_set.borrow_mut();
             if !entry_set_borrow.is_empty() {
-                header_to_pos.insert(get_table_name(&entry_set_borrow[0]), table_set.len());
-                table_set.push(RefCell::new(entry_set_borrow.clone()));
+                let table_name = get_table_name(&entry_set_borrow[0]);
+                let indexes = header_to_pos.entry(table_name).or_default();
+                if kind == TABLE_ARRAY_HEADER || (kind == TABLE_HEADER && indexes.is_empty()) {
+                    indexes.push(table_set.len());
+                    table_set.push(RefCell::new(entry_set_borrow.clone()));
+                } else if kind == TABLE_HEADER && !indexes.is_empty() {
+                    // join tables
+                    let pos = indexes.first().unwrap();
+                    let mut res = table_set.index(*pos).borrow_mut();
+                    for element in entry_set_borrow.clone() {
+                        if element.kind() != TABLE_HEADER {
+                            res.push(element);
+                        }
+                    }
+                }
                 entry_set_borrow.clear();
             }
         };
         for c in root_ast.children_with_tokens() {
             if [TABLE_ARRAY_HEADER, TABLE_HEADER].contains(&c.kind()) {
-                add_to_table_set();
+                add_to_table_set(table_kind);
+                table_kind = c.kind();
             }
             entry_set.borrow_mut().push(c);
         }
-        add_to_table_set();
-
+        add_to_table_set(table_kind);
         Self {
             header_to_pos,
             table_set,
         }
     }
 
     pub fn reorder(&mut self, root_ast: &SyntaxNode, order: &[&str]) {
@@ -57,41 +76,51 @@
         let order = calculate_order(&self.header_to_pos, order);
         let mut next = order.clone();
         if !next.is_empty() {
             next.remove(0);
         }
         next.push(String::new());
         for (name, next_name) in zip(order.iter(), next.iter()) {
-            let mut entries = self.get(name).unwrap().borrow().clone();
-            if entries.is_empty() {
-                continue;
-            }
-            entry_count += entries.len();
-            let last = entries.last().unwrap();
-            if name.is_empty() && last.kind() == SyntaxKind::NEWLINE && entries.len() == 1 {
-                continue;
-            }
-            if last.kind() == SyntaxKind::NEWLINE && get_key(name) != get_key(next_name) {
-                entries.splice(entries.len() - 1..entries.len(), [make_empty_newline()]);
+            for entries in self.get(name).unwrap() {
+                let got = entries.borrow_mut();
+                if !got.is_empty() {
+                    entry_count += got.len();
+                    let last = got.last().unwrap();
+                    if name.is_empty() && last.kind() == SyntaxKind::NEWLINE && got.len() == 1 {
+                        continue;
+                    }
+                    let mut add = got.clone();
+                    if get_key(name) != get_key(next_name) {
+                        if last.kind() == SyntaxKind::NEWLINE {
+                            // replace existing newline to ensure single newline
+                            add.pop();
+                        }
+                        add.push(make_empty_newline());
+                    }
+                    to_insert.extend(add);
+                }
             }
-            to_insert.extend(entries);
         }
         root_ast.splice_children(0..entry_count, to_insert);
     }
 }
 
-fn calculate_order(header_to_pos: &HashMap<String, usize>, ordering: &[&str]) -> Vec<String> {
+fn calculate_order(header_to_pos: &HashMap<String, Vec<usize>>, ordering: &[&str]) -> Vec<String> {
     let max_ordering = ordering.len() * 2;
     let key_to_pos = ordering
         .iter()
         .enumerate()
         .map(|(k, v)| (v, k * 2))
         .collect::<HashMap<&&str, usize>>();
 
-    let mut header_pos: Vec<(String, usize)> = header_to_pos.clone().into_iter().collect();
+    let mut header_pos: Vec<(String, usize)> = header_to_pos
+        .clone()
+        .into_iter()
+        .map(|(k, v)| (k, *v.iter().min().unwrap()))
+        .collect();
 
     header_pos.sort_by_cached_key(|(k, file_pos)| -> (usize, usize) {
         let key = get_key(k);
         let pos = key_to_pos.get(&key.as_str());
 
         (
             if let Some(&pos) = pos {
@@ -115,36 +144,40 @@
             String::from(parts[0])
         };
     }
     String::from(k)
 }
 
 pub fn reorder_table_keys(table: &mut RefMut<Vec<SyntaxElement>>, order: &[&str]) {
-    let size = table.len();
-    let (key_to_pos, key_set) = load_keys(table);
-    let mut to_insert = Vec::<SyntaxElement>::new();
-    let mut handled = HashSet::<usize>::new();
-    for key in order {
-        let mut parts = key_to_pos
-            .keys()
-            .filter(|k| {
-                key == k || (k.starts_with(key) && k.len() > key.len() && k.chars().nth(key.len()).unwrap() == '.')
+    let (size, mut to_insert) = (table.len(), Vec::<SyntaxElement>::new());
+    let (key_to_position, key_set) = load_keys(table);
+    let mut handled_positions = HashSet::<usize>::new();
+    for current_key in order {
+        let mut matching_keys = key_to_position
+            .iter()
+            .filter(|(checked_key, position)| {
+                !handled_positions.contains(position)
+                    && (current_key == checked_key
+                        || (checked_key.starts_with(current_key)
+                            && checked_key.len() > current_key.len()
+                            && checked_key.chars().nth(current_key.len()).unwrap() == '.'))
             })
+            .map(|(key, _)| key)
             .clone()
             .collect::<Vec<&String>>();
-        parts.sort_by_key(|s| s.to_lowercase().replace('"', ""));
-        for element in parts {
-            let pos = key_to_pos[element];
-            to_insert.extend(key_set[pos].clone());
-            handled.insert(pos);
+        matching_keys.sort_by_key(|key| key.to_lowercase().replace('"', ""));
+        for key in matching_keys {
+            let position = key_to_position[key];
+            to_insert.extend(key_set[position].clone());
+            handled_positions.insert(position);
         }
     }
-    for (at, entry) in key_set.into_iter().enumerate() {
-        if !handled.contains(&at) {
-            to_insert.extend(entry);
+    for (position, entries) in key_set.into_iter().enumerate() {
+        if !handled_positions.contains(&position) {
+            to_insert.extend(entries);
         }
     }
     table.splice(0..size, to_insert);
 }
 
 fn load_keys(table: &RefMut<Vec<SyntaxElement>>) -> (HashMap<String, usize>, Vec<Vec<SyntaxElement>>) {
     let mut key_to_pos = HashMap::<String, usize>::new();
@@ -208,20 +241,30 @@
     let h2p = tables.header_to_pos.clone();
     let sub_name_prefix = format!("{name}.");
     let sub_table_keys: Vec<&String> = h2p.keys().filter(|s| s.starts_with(sub_name_prefix.as_str())).collect();
     if sub_table_keys.is_empty() {
         return;
     }
     if !tables.header_to_pos.contains_key(name) {
-        tables.header_to_pos.insert(String::from(name), tables.table_set.len());
+        tables
+            .header_to_pos
+            .insert(String::from(name), vec![tables.table_set.len()]);
         tables.table_set.push(RefCell::new(make_table_entry(name)));
     }
-    let mut main = tables.table_set[tables.header_to_pos[name]].borrow_mut();
+    let main_positions = tables.header_to_pos[name].clone();
+    if main_positions.len() != 1 {
+        return;
+    }
+    let mut main = tables.table_set[*main_positions.first().unwrap()].borrow_mut();
     for key in sub_table_keys {
-        let mut sub = tables.table_set[tables.header_to_pos[key]].borrow_mut();
+        let sub_positions = tables.header_to_pos[key].clone();
+        if sub_positions.len() != 1 {
+            continue;
+        }
+        let mut sub = tables.table_set[*sub_positions.first().unwrap()].borrow_mut();
         let sub_name = key.strip_prefix(sub_name_prefix.as_str()).unwrap();
         let mut header = false;
         for child in sub.iter() {
             let kind = child.kind();
             if kind == SyntaxKind::TABLE_HEADER {
                 header = true;
                 continue;
```

### Comparing `pyproject_fmt_rust-1.0.6/rust/src/main.rs` & `pyproject_fmt_rust-1.1.0/rust/src/main.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 use std::string::String;
 
 use pyo3::prelude::PyModule;
 use pyo3::{pyclass, pyfunction, pymethods, pymodule, wrap_pyfunction, Bound, PyResult};
 use taplo::formatter::{format_syntax, Options};
 use taplo::parser::parse;
 
-use crate::build_system::fix_build;
 use crate::global::reorder_tables;
 use crate::helpers::table::Tables;
-use crate::project::fix_project_table;
 
 mod build_system;
 mod project;
 
 mod global;
 mod helpers;
+mod ruff;
 
 #[pyclass(frozen, get_all)]
 pub struct Settings {
     column_width: usize,
     indent: usize,
     keep_full_version: bool,
     max_supported_python: (u8, u8),
@@ -49,21 +48,22 @@
 /// Format toml file
 #[must_use]
 #[pyfunction]
 pub fn format_toml(content: &str, opt: &Settings) -> String {
     let root_ast = parse(content).into_syntax().clone_for_update();
     let mut tables = Tables::from_ast(&root_ast);
 
-    fix_build(&mut tables, opt.keep_full_version);
-    fix_project_table(
+    build_system::fix(&mut tables, opt.keep_full_version);
+    project::fix(
         &mut tables,
         opt.keep_full_version,
         opt.max_supported_python,
         opt.min_supported_python,
     );
+    ruff::fix(&mut tables);
     reorder_tables(&root_ast, &mut tables);
 
     let options = Options {
         align_entries: false,           // do not align by =
         align_comments: true,           // align inline comments
         align_single_comments: true,    // align comments after entries
         array_trailing_comma: true,     // ensure arrays finish with trailing comma
@@ -191,40 +191,71 @@
     "#},
         indoc ! {r#"
     [project]
     classifiers = [
       "Programming Language :: Python :: 3 :: Only",
       "Programming Language :: Python :: 3.8",
     ]
+
     [tool.coverage]
     a = 0
     [tool.coverage.report]
     a = 2
     [tool.coverage.paths]
     a = 1
     [tool.coverage.run]
     a = 3
     "#},
         2,
         true,
         (3, 8)
     )]
+    #[case::array_of_tables(
+        indoc ! {r#"
+        [tool.commitizen]
+        name = "cz_customize"
+
+        [tool.commitizen.customize]
+        message_template = ""
+
+        [[tool.commitizen.customize.questions]]
+        type = "list"
+        [[tool.commitizen.customize.questions]]
+        type = "input"
+    "#},
+        indoc ! {r#"
+    [tool.commitizen]
+    name = "cz_customize"
+
+    [tool.commitizen.customize]
+    message_template = ""
+
+    [[tool.commitizen.customize.questions]]
+    type = "list"
+
+    [[tool.commitizen.customize.questions]]
+    type = "input"
+    "#},
+        2,
+        true,
+        (3, 8)
+    )]
     fn test_format_toml(
         #[case] start: &str,
         #[case] expected: &str,
         #[case] indent: usize,
         #[case] keep_full_version: bool,
         #[case] max_supported_python: (u8, u8),
     ) {
-        let got = format_toml(
-            start,
-            &Settings {
-                column_width: 1,
-                indent,
-                keep_full_version,
-                max_supported_python,
-                min_supported_python: (3, 8),
-            },
-        );
+        let settings = Settings {
+            column_width: 1,
+            indent,
+            keep_full_version,
+            max_supported_python,
+            min_supported_python: (3, 8),
+        };
+        let got = format_toml(start, &settings);
         assert_eq!(got, expected);
+        let second = format_toml(got.as_str(), &settings);
+        assert_eq!(got, second);
     }
 }
```

### Comparing `pyproject_fmt_rust-1.0.6/rust/src/project.rs` & `pyproject_fmt_rust-1.1.0/rust/src/project.rs`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 
 use crate::helpers::array::{sort, transform};
 use crate::helpers::create::{make_array, make_array_entry, make_comma, make_entry_of_string, make_newline};
 use crate::helpers::pep508::{format_requirement, get_canonic_requirement_name};
 use crate::helpers::string::{load_text, update_content};
 use crate::helpers::table::{collapse_sub_tables, for_entries, reorder_table_keys, Tables};
 
-pub fn fix_project_table(
+pub fn fix(
     tables: &mut Tables,
     keep_full_version: bool,
     max_supported_python: (u8, u8),
     min_supported_python: (u8, u8),
 ) {
     collapse_sub_tables(tables, "project");
     let table_element = tables.get(&String::from("project"));
     if table_element.is_none() {
         return;
     }
-    let table = &mut table_element.unwrap().borrow_mut();
+    let table = &mut table_element.unwrap().first().unwrap().borrow_mut();
     expand_entry_points_inline_tables(table);
     for_entries(table, &mut |key, entry| match key.split('.').next().unwrap() {
         "name" => {
             update_content(entry, get_canonic_requirement_name);
         }
         "version" | "readme" | "license-files" | "scripts" | "entry-points" | "gui-scripts" => {
             update_content(entry, |s| String::from(s));
@@ -372,21 +372,21 @@
     use indoc::indoc;
     use rstest::rstest;
     use taplo::formatter::{format_syntax, Options};
     use taplo::parser::parse;
     use taplo::syntax::SyntaxElement;
 
     use crate::helpers::table::Tables;
-    use crate::project::fix_project_table;
+    use crate::project::fix;
 
     fn evaluate(start: &str, keep_full_version: bool, max_supported_python: (u8, u8)) -> String {
         let root_ast = parse(start).into_syntax().clone_for_update();
         let count = root_ast.children_with_tokens().count();
         let mut tables = Tables::from_ast(&root_ast);
-        fix_project_table(&mut tables, keep_full_version, max_supported_python, (3, 8));
+        fix(&mut tables, keep_full_version, max_supported_python, (3, 8));
         let entries = tables
             .table_set
             .iter()
             .flat_map(|e| e.borrow().clone())
             .collect::<Vec<SyntaxElement>>();
         root_ast.splice_children(0..count, entries);
         let opt = Options {
```

### Comparing `pyproject_fmt_rust-1.0.6/src/pyproject_fmt_rust/_lib.pyi` & `pyproject_fmt_rust-1.1.0/src/pyproject_fmt_rust/_lib.pyi`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/tests/test_main.py` & `pyproject_fmt_rust-1.1.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/tox.ini` & `pyproject_fmt_rust-1.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/Cargo.lock` & `pyproject_fmt_rust-1.1.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -516,15 +516,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyproject-fmt-rust"
-version = "1.0.6"
+version = "1.1.0"
 dependencies = [
  "indoc",
  "lexical-sort",
  "pep440_rs",
  "pep508_rs",
  "pyo3",
  "regex",
```

### Comparing `pyproject_fmt_rust-1.0.6/pyproject.toml` & `pyproject_fmt_rust-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.6/PKG-INFO` & `pyproject_fmt_rust-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt-rust
-Version: 1.0.6
+Version: 1.1.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

