# Comparing `tmp/rustitude-0.3.4.tar.gz` & `tmp/rustitude-0.4.0.tar.gz`

## Comparing `rustitude-0.3.4.tar` & `rustitude-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,50 @@
--rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 rustitude-0.3.4/Cargo.toml
--rw-r--r--   0     1001      127     3469 2024-05-06 23:06:20.000000 rustitude-0.3.4/.github/workflows/maturin.yml
--rw-r--r--   0     1001      127      316 2024-05-06 23:06:20.000000 rustitude-0.3.4/.github/workflows/rust.yml
--rw-r--r--   0     1001      127     3136 2024-05-06 23:06:20.000000 rustitude-0.3.4/.gitignore
--rw-r--r--   0     1001      127    15705 2024-05-06 23:06:20.000000 rustitude-0.3.4/CHANGELOG.md
--rw-r--r--   0     1001      127     1507 2024-05-06 23:06:20.000000 rustitude-0.3.4/LICENSE
--rw-r--r--   0     1001      127    11361 2024-05-06 23:06:20.000000 rustitude-0.3.4/README.md
--rw-r--r--   0     1001      127     2846 2024-05-06 23:06:20.000000 rustitude-0.3.4/bacon.toml
--rw-r--r--   0     1001      127    32108 2024-05-06 23:06:20.000000 rustitude-0.3.4/media/logo.png
--rw-r--r--   0     1001      127     1723 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/__init__.py
--rw-r--r--   0     1001      127     4264 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/__init__.pyi
--rw-r--r--   0     1001      127      145 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/amplitude.pyi
--rw-r--r--   0     1001      127      840 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/dataset.pyi
--rw-r--r--   0     1001      127      535 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/four_momentum.pyi
--rw-r--r--   0     1001      127       90 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/gluex/__init__.pyi
--rw-r--r--   0     1001      127       83 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/gluex/dalitz.pyi
--rw-r--r--   0     1001      127     4632 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/gluex/harmonics.pyi
--rw-r--r--   0     1001      127      566 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/gluex/resonances.pyi
--rw-r--r--   0     1001      127      347 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/gluex/sdmes.pyi
--rw-r--r--   0     1001      127     3275 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/manager.pyi
--rw-r--r--   0     1001      127        0 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/py.typed
--rw-r--r--   0     1001      127     1650 2024-05-06 23:06:20.000000 rustitude-0.3.4/src/lib.rs
--rw-r--r--   0     1001      127    37972 2024-05-06 23:06:20.000000 rustitude-0.3.4/Cargo.lock
--rw-r--r--   0     1001      127      911 2024-05-06 23:06:20.000000 rustitude-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    12144 1970-01-01 00:00:00.000000 rustitude-0.3.4/PKG-INFO
+-rw-r--r--   0     1001      127      843 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/Cargo.toml
+-rw-r--r--   0     1001      127      316 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127       66 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/.gitignore
+-rw-r--r--   0     1001      127    15381 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/CHANGELOG.md
+-rw-r--r--   0     1001      127     1509 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/LICENSE
+-rw-r--r--   0     1001      127    11271 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/README.md
+-rw-r--r--   0     1001      127     2773 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/bacon.toml
+-rw-r--r--   0     1001      127    32108 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/media/logo.png
+-rw-r--r--   0     1001      127    37710 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/src/amplitude.rs
+-rw-r--r--   0     1001      127    25986 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/src/dataset.rs
+-rw-r--r--   0     1001      127     1596 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/src/docs-header.html
+-rw-r--r--   0     1001      127    10542 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/src/four_momentum.rs
+-rw-r--r--   0     1001      127      826 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/src/lib.rs
+-rw-r--r--   0     1001      127     2334 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/src/manager.rs
+-rw-r--r--   0     1001      127      566 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/Cargo.toml
+-rw-r--r--   0     1001      127      316 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127       14 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/.gitignore
+-rw-r--r--   0     1001      127     5364 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/CHANGELOG.md
+-rw-r--r--   0     1001      127     1507 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/LICENSE
+-rw-r--r--   0     1001      127    14640 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/README.md
+-rw-r--r--   0     1001      127     2773 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/bacon.toml
+-rw-r--r--   0     1001      127    24055 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/media/logo.png
+-rw-r--r--   0     1001      127     3086 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/src/dalitz.rs
+-rw-r--r--   0     1001      127     8462 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/src/harmonics.rs
+-rw-r--r--   0     1001      127       85 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/src/lib.rs
+-rw-r--r--   0     1001      127    22294 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/src/resonances.rs
+-rw-r--r--   0     1001      127     7565 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/src/sdmes.rs
+-rw-r--r--   0     1001      127     7940 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/src/utils.rs
+-rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 rustitude-0.4.0/Cargo.toml
+-rw-r--r--   0     1001      127     3469 2024-05-15 00:01:52.000000 rustitude-0.4.0/.github/workflows/maturin.yml
+-rw-r--r--   0     1001      127      316 2024-05-15 00:01:52.000000 rustitude-0.4.0/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127     3144 2024-05-15 00:01:52.000000 rustitude-0.4.0/.gitignore
+-rw-r--r--   0     1001      127      159 2024-05-15 00:01:52.000000 rustitude-0.4.0/.justfile
+-rw-r--r--   0     1001      127    13263 2024-05-15 00:01:52.000000 rustitude-0.4.0/CHANGELOG.md
+-rw-r--r--   0     1001      127     1507 2024-05-15 00:01:52.000000 rustitude-0.4.0/LICENSE
+-rw-r--r--   0     1001      127    10688 2024-05-15 00:01:52.000000 rustitude-0.4.0/README.md
+-rw-r--r--   0     1001      127     2846 2024-05-15 00:01:52.000000 rustitude-0.4.0/bacon.toml
+-rw-r--r--   0     1001      127    32108 2024-05-15 00:01:52.000000 rustitude-0.4.0/media/logo.png
+-rw-r--r--   0     1001      127     1841 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/__init__.py
+-rw-r--r--   0     1001      127     4013 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/__init__.pyi
+-rw-r--r--   0     1001      127       90 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/gluex/__init__.pyi
+-rw-r--r--   0     1001      127       75 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/gluex/dalitz.pyi
+-rw-r--r--   0     1001      127     3778 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/gluex/harmonics.pyi
+-rw-r--r--   0     1001      127      535 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/gluex/resonances.pyi
+-rw-r--r--   0     1001      127      336 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/gluex/sdmes.pyi
+-rw-r--r--   0     1001      127        0 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/py.typed
+-rw-r--r--   0     1001      127     1654 2024-05-15 00:01:52.000000 rustitude-0.4.0/src/lib.rs
+-rw-r--r--   0     1001      127    38250 2024-05-15 00:01:52.000000 rustitude-0.4.0/Cargo.lock
+-rw-r--r--   0     1001      127     1029 2024-05-15 00:01:52.000000 rustitude-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11471 1970-01-01 00:00:00.000000 rustitude-0.4.0/PKG-INFO
```

### Comparing `rustitude-0.3.4/Cargo.toml` & `rustitude-0.4.0/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
+[workspace]
+resolver = "2"
+
 [package]
-exclude = ["convert", "resources"]
 name = "rustitude"
-version = "0.3.4"
+version = "0.4.0"
 edition = "2021"
 authors = ["Nathaniel Dene Hoffman <dene@cmu.edu>"]
 description = "A library to create and operate models for particle physics amplitude analyses"
 repository = "https://github.com/denehoffman/rustitude/"
 homepage = "https://github.com/denehoffman/rustitude/"
 license = "BSD-3-Clause"
 readme = "README.md"
-# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 name = "rustitude"
 crate-type = ["cdylib"]
 
 [dependencies]
 rayon = "1.10.0"
-rustitude-core = { version = "0.3.3", git = "https://github.com/denehoffman/rustitude-core.git" }
-rustitude-gluex = { version = "0.1.4", optional = true, git = "https://github.com/denehoffman/rustitude-gluex.git" }
+rustitude-core = { path = "crates/rustitude-core" }
+rustitude-gluex = { path = "crates/rustitude-gluex", optional = true }
 
 [dependencies.pyo3]
 version = "0.21.2"
 features = ["abi3-py37"]
 
 [features]
 default = ["gluex"]
```

### Comparing `rustitude-0.3.4/.github/workflows/maturin.yml` & `rustitude-0.4.0/.github/workflows/maturin.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 on:
   push:
     branches:
       - main
       - master
     tags:
-      - '*'
+      - "*"
   pull_request:
   workflow_dispatch:
 
 permissions:
   contents: read
 
 jobs:
@@ -36,21 +36,21 @@
             target: s390x
           - runner: ubuntu-latest
             target: ppc64le
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
-          python-version: '3.10'
+          python-version: "3.10"
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.platform.target }}
           args: --release --out dist
-          sccache: 'true'
+          sccache: "true"
           manylinux: auto
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheels-linux-${{ matrix.platform.target }}
           path: dist
 
@@ -63,22 +63,22 @@
             target: x64
           - runner: windows-latest
             target: x86
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
-          python-version: '3.10'
+          python-version: "3.10"
           architecture: ${{ matrix.platform.target }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.platform.target }}
           args: --release --out dist
-          sccache: 'true'
+          sccache: "true"
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheels-windows-${{ matrix.platform.target }}
           path: dist
 
   macos:
@@ -90,21 +90,21 @@
             target: x86_64
           - runner: macos-14
             target: aarch64
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
-          python-version: '3.10'
+          python-version: "3.10"
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.platform.target }}
           args: --release --out dist
-          sccache: 'true'
+          sccache: "true"
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheels-macos-${{ matrix.platform.target }}
           path: dist
 
   sdist:
```

### Comparing `rustitude-0.3.4/.gitignore` & `rustitude-0.4.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -164,7 +164,8 @@
 debug/
 **/*.rs.bk
 *.pdb
 
 resources/
 *.svg
 notes
+demo.py
```

### Comparing `rustitude-0.3.4/CHANGELOG.md` & `rustitude-0.4.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,53 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 0.4.0 (2024-05-15)
+
+### Bug Fixes
+
+ - <csr-id-b71f07c33445f310969e445e7b158bdeef726a8d/> make add_submodule public
+
+### Other
+
+ - <csr-id-f39aab03b7160ba3817614170d67bfcfdb22642b/> reorganize crate structure
+
+### Commit Statistics
+
+<csr-read-only-do-not-edit/>
+
+ - 2 commits contributed to the release over the course of 1 calendar day.
+ - 8 days passed between releases.
+ - 2 commits were understood as [conventional](https://www.conventionalcommits.org).
+ - 0 issues like '(#ID)' were seen in commit messages
+
+### Commit Details
+
+<csr-read-only-do-not-edit/>
+
+<details><summary>view details</summary>
+
+ * **Uncategorized**
+    - Reorganize crate structure ([`f39aab0`](https://github.com/denehoffman/rustitude/commit/f39aab03b7160ba3817614170d67bfcfdb22642b))
+    - Make add_submodule public ([`b71f07c`](https://github.com/denehoffman/rustitude/commit/b71f07c33445f310969e445e7b158bdeef726a8d))
+</details>
+
 ## 0.3.4 (2024-05-06)
 
+<csr-id-475682fc30d7dc6a817030dd754cc4fb7dd295cc/>
+<csr-id-f64c86d2e21c17fe6bc5638240293a774185159a/>
+<csr-id-4a88e2b13fb01de2812f91ef4d55eea6b37fe7b2/>
+<csr-id-1747d5dc4a63bf47f2f5cbc479f879459e900c4c/>
+<csr-id-42f29669736bb72ed4d85f4669df1a48288a2db8/>
+<csr-id-d94179156007fd86b69b8efbfd2f1799d0bb71b8/>
+
 ### Chore
 
  - <csr-id-475682fc30d7dc6a817030dd754cc4fb7dd295cc/> bump python library version
 
 ### Documentation
 
  - <csr-id-6d613a1c49ce065ffa4a50df09380f41359218be/> Update README.md
@@ -35,77 +72,48 @@
    A release only happens with a new tag
  - <csr-id-d94179156007fd86b69b8efbfd2f1799d0bb71b8/> update pyproject.toml version
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
 
- - 13 commits contributed to the release over the course of 3 calendar days.
+ - 1 commit contributed to the release over the course of 1 calendar day.
  - 3 days passed between releases.
- - 12 commits were understood as [conventional](https://www.conventionalcommits.org).
+ - 1 commit was understood as [conventional](https://www.conventionalcommits.org).
  - 0 issues like '(#ID)' were seen in commit messages
 
 ### Commit Details
 
 <csr-read-only-do-not-edit/>
 
 <details><summary>view details</summary>
 
  * **Uncategorized**
-    - Merge branch 'main' of https://github.com/denehoffman/rustitude ([`7a3806c`](https://github.com/denehoffman/rustitude/commit/7a3806caf8741dc55283deb803653d4b0f892a61))
-    - Bump python library version ([`475682f`](https://github.com/denehoffman/rustitude/commit/475682fc30d7dc6a817030dd754cc4fb7dd295cc))
-    - Update Cargo.lock ([`f64c86d`](https://github.com/denehoffman/rustitude/commit/f64c86d2e21c17fe6bc5638240293a774185159a))
-    - Update README.md ([`6d613a1`](https://github.com/denehoffman/rustitude/commit/6d613a1c49ce065ffa4a50df09380f41359218be))
-    - Correct spelling ([`9735d57`](https://github.com/denehoffman/rustitude/commit/9735d57d039946cc7b5de57a9965c4fd01c2964f))
-    - Update README.md ([`48a7362`](https://github.com/denehoffman/rustitude/commit/48a73623f151336f198009097c028d000d3e43c5))
-    - Fixed some links ([`2d548c4`](https://github.com/denehoffman/rustitude/commit/2d548c4865b90043005b2aed7977612a28dad409))
     - Add type checking and re-export rustitude-core and rustitude-gluex as their own submodules ([`6fc5c77`](https://github.com/denehoffman/rustitude/commit/6fc5c77477602403f3b892b240064de9f717d406))
-    - Update README.md ([`3dc6275`](https://github.com/denehoffman/rustitude/commit/3dc627598be4f79ffc230f8bff813423d57491f2))
-    - Re-enable tag check ([`4a88e2b`](https://github.com/denehoffman/rustitude/commit/4a88e2b13fb01de2812f91ef4d55eea6b37fe7b2))
-    - Temporarily disable tag check so we can push to pypi through an action ([`1747d5d`](https://github.com/denehoffman/rustitude/commit/1747d5dc4a63bf47f2f5cbc479f879459e900c4c))
-    - Re-enable on-push and on-PR workflow conditions ([`42f2966`](https://github.com/denehoffman/rustitude/commit/42f29669736bb72ed4d85f4669df1a48288a2db8))
-    - Update pyproject.toml version ([`d941791`](https://github.com/denehoffman/rustitude/commit/d94179156007fd86b69b8efbfd2f1799d0bb71b8))
 </details>
 
-## 0.3.3-pypi (2024-05-03)
+## 0.3.3 (2024-05-03)
+
+<csr-id-e0c32f773b601e2703a0803849a1a2db130e2ffc/>
+<csr-id-158ddc248dc8463e08eb14b7f633952fc28abcd6/>
+<csr-id-f8370544ef666930bfd5f3a1b555e34e53525b6f/>
+<csr-id-db8b1a32563700203f896c0d357ed96d1144d202/>
 
 ### Chore
 
  - <csr-id-e0c32f773b601e2703a0803849a1a2db130e2ffc/> update pyproject.toml info
 
 ### Other
 
  - <csr-id-158ddc248dc8463e08eb14b7f633952fc28abcd6/> remove unused library in rustitude-gluex which prevented cross-compilation
  - <csr-id-f8370544ef666930bfd5f3a1b555e34e53525b6f/> Update maturin.yml
    don't publish on every push, need to set up more for that
  - <csr-id-db8b1a32563700203f896c0d357ed96d1144d202/> add maturin github actions
 
-### Commit Statistics
-
-<csr-read-only-do-not-edit/>
-
- - 5 commits contributed to the release.
- - 4 commits were understood as [conventional](https://www.conventionalcommits.org).
- - 0 issues like '(#ID)' were seen in commit messages
-
-### Commit Details
-
-<csr-read-only-do-not-edit/>
-
-<details><summary>view details</summary>
-
- * **Uncategorized**
-    - Release rustitude v0.3.3 ([`b5748e4`](https://github.com/denehoffman/rustitude/commit/b5748e46a5bb8c19e74b71b10de3d6ba48edbf87))
-    - Remove unused library in rustitude-gluex which prevented cross-compilation ([`158ddc2`](https://github.com/denehoffman/rustitude/commit/158ddc248dc8463e08eb14b7f633952fc28abcd6))
-    - Update maturin.yml ([`f837054`](https://github.com/denehoffman/rustitude/commit/f8370544ef666930bfd5f3a1b555e34e53525b6f))
-    - Add maturin github actions ([`db8b1a3`](https://github.com/denehoffman/rustitude/commit/db8b1a32563700203f896c0d357ed96d1144d202))
-    - Update pyproject.toml info ([`e0c32f7`](https://github.com/denehoffman/rustitude/commit/e0c32f773b601e2703a0803849a1a2db130e2ffc))
-</details>
-
-## 0.3.3 (2024-05-03)
+## 0.3.3-pypi (2024-05-03)
 
 <csr-id-e0c32f773b601e2703a0803849a1a2db130e2ffc/>
 <csr-id-158ddc248dc8463e08eb14b7f633952fc28abcd6/>
 <csr-id-f8370544ef666930bfd5f3a1b555e34e53525b6f/>
 <csr-id-db8b1a32563700203f896c0d357ed96d1144d202/>
 
 ### Chore
@@ -152,35 +160,27 @@
  - <csr-id-e2cb6e54946744299506a39a5d3559ee099378fb/> Create LICENSE
  - <csr-id-310f89c2a2da584beabad3e208484be186e8f7fd/> update .gitignore
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
 
- - 10 commits contributed to the release over the course of 1 calendar day.
- - 8 commits were understood as [conventional](https://www.conventionalcommits.org).
+ - 2 commits contributed to the release over the course of 1 calendar day.
+ - 2 commits were understood as [conventional](https://www.conventionalcommits.org).
  - 0 issues like '(#ID)' were seen in commit messages
 
 ### Commit Details
 
 <csr-read-only-do-not-edit/>
 
 <details><summary>view details</summary>
 
  * **Uncategorized**
-    - Release rustitude v0.3.2 ([`3e77a7e`](https://github.com/denehoffman/rustitude/commit/3e77a7e589335c6d901cd07232ed558c026007cb))
-    - Bump rustitude dependency versions ([`023cfea`](https://github.com/denehoffman/rustitude/commit/023cfea357b0d6e5c12f724df32d4ed30c9f24c7))
     - Opt for implementing all pyo3 bindings in their own submodules - this package will be very lightweight! ([`3126b7a`](https://github.com/denehoffman/rustitude/commit/3126b7a26b835ee24d112883ca540c172d97dd82))
-    - Merge branch 'main' of https://github.com/denehoffman/rustitude ([`ee950cd`](https://github.com/denehoffman/rustitude/commit/ee950cda479ebd9b3ee2c9d829aa16b359f39022))
-    - Add local notes ([`aaa07cd`](https://github.com/denehoffman/rustitude/commit/aaa07cd742e03461449269e8261e7f326600b2a0))
-    - Create LICENSE ([`e2cb6e5`](https://github.com/denehoffman/rustitude/commit/e2cb6e54946744299506a39a5d3559ee099378fb))
-    - Create rust.yml ([`7646b89`](https://github.com/denehoffman/rustitude/commit/7646b89c792c0f55b8898832abe6a743a052fc7a))
     - Initial commit to rustitude meta-crate ([`157c864`](https://github.com/denehoffman/rustitude/commit/157c8648dbcc1a6111d8c262a31139990ab09f3b))
-    - Update .gitignore ([`310f89c`](https://github.com/denehoffman/rustitude/commit/310f89c2a2da584beabad3e208484be186e8f7fd))
-    - Add README and CHANGELOG ([`8bd07de`](https://github.com/denehoffman/rustitude/commit/8bd07de2425e48f4489a59ce4c168eaa9df9cc42))
 </details>
 
 ## 0.3.1 (2024-04-10)
 
 <csr-id-35fd81ade394522801d288e4a2d084b581d5e5a5/>
 <csr-id-1d91ee9b2928b9761b0568104ea5e8b7841bf24c/>
 <csr-id-73067f2c6f657ba3b35a197a0ab2ea8029e359e6/>
```

### Comparing `rustitude-0.3.4/LICENSE` & `rustitude-0.4.0/crates/rustitude-gluex/LICENSE`

 * *Files identical despite different names*

### Comparing `rustitude-0.3.4/README.md` & `rustitude-0.4.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -18,120 +18,122 @@
   <a href="https://crates.io/crates/rustitude" alt="Rustitude on crates.io">
     <img src="https://img.shields.io/crates/v/rustitude" /></a>
   <a href="https://docs.rs/rustitude" alt="Rustitude documentation on docs.rs">
     <img src="https://img.shields.io/docsrs/rustitude" /></a>
 </p>
 
 ### Table of Contents:
+
 - [Introduction](#Introduction)
 - [Theory](#Theory)
 - [Installation](#Installation)
 - [Usage](#Usage)
 - [TODOs](#TODOs)
 
 # Introduction
+
 This project began with a desire to make a fast but easy to use interface for fitting amplitudes to particle physics data. That being said, there are performant methods such as [`AmpTools`](https://github.com/mashephe/AmpTools), which is written in C++, but in my personal experience, it can be a bit tricky to use and extend, and it generally requires a lot of boilerplate code to generate new amplitudes or plotting scripts. On the other hand, there are also libraries like [`PyPWA`](https://github.com/JeffersonLab/PyPWA/) (written in Python) which seem like they could be easy to use, but often fail in this aspect due to Python's limiting syntax, speed issues, and a general lack of documentation and ongoing development. There have been attempts to bridge the gap between AmpTools and Python, most recently (and successfully) [`PyAmpTools`](https://github.com/lan13005/PyAmpTools). The difficulty with this method is that it relies on PyROOT, which also means you need ROOT installed (and built with your version of Python). For now, I'll spare you the anti-ROOT rant and just say that ROOT should be an opt-in, not a requirement. So where does that leave `rustitude`?
 
 As the name suggests, `rustitude` was written in Rust, so let's get the obvious downside out of the way: not many particle physicists know how to write Rust code. Hopefully, this will change over the next decade (and there has already been some [support](https://www.whitehouse.gov/oncd/briefing-room/2024/02/26/memory-safety-statements-of-support/) from the US government, of all places). While Rust carries the disadvantage of relative obscurity compared to C++, it also has many benefits. No `null` means no null references (Tony Hoare's ["billion dollar mistake"](https://web.archive.org/web/20090628071208/http://qconlondon.com/london-2009/speaker/Tony+Hoare)). Pointers (called references in Rust) are always valid, a guarantee made by a very helpful and only occasionally frustrating borrow checker. Rust "crates" are set up in a way which encourages documentation (see [`rustitude-core`'s documentation](https://docs.rs/rustitude-core/)), and the basic syntax is fairly easy to learn for people who have been using optional type checking in Python. Perhaps one of the biggest benefits of Rust is how easy it is to employ [parallelization](https://crates.io/crates/rayon), but the two reasons I like it most are that it's incredibly easy to write Python bindings (that's what this library is after all) and it has a package manager. This second point is important -- unlike C/C++, where a developer is swamped with some menagerie `Makefile`, `CMakeLists.txt`, or some `scons` monstrosity which may only work on "X" system and only if you install and use `make`, `cmake`, `g++`, or whatever (oh yeah, and you made sure all your external dependencies are linked correctly, right? Right?), Rust supports adding a package by simply adding a line to `Cargo.toml` (or using the `cargo add` command). In many ways, package management in Rust is actually simpler than Python, since there's only one prefered method of creating and managing projects, formatting, linting, and compiling.
 
 Now I've covered why I don't like some of the existing solutions, and why I chose to use Rust, but what does this project have that makes it stand out? Here are some reasons to entice you:
 
 - `rustitude` will automatically parallelize amplitudes over the events in a dataset. There's no reason for a developer to ever write parallelized code themselves.
 - Implementing [`Node`](https://docs.rs/rustitude-core/latest/rustitude_core/amplitude/trait.Node.html) on a struct is all that is needed to use it as an amplitude. This means developers need only write two to three total methods to describe the entire functionality of their amplitude, and one of these just gives the names and order of the amplitude's input parameters.
 - A major goal of `rustitude` was to increase processing speed by sacrificing memory. This is done by precalculating parts of amplitudes which don't change when the free parameter inputs change. `AmpTools` supports a version of this, but only on the level of each general amplitude rather than on an individual basis. The simplest example of this is the `Ylm` amplitude (spherical harmonic), which can be entirely precalculated given the value of `l` and `m`. In `AmpTools`, different instances of `Ylm` with different `l`s and `m`s share precalculated data, whereas in `rustitude`, they don't. The `AmpTools` implementation of `Ylm` needs to calculate a spherical harmonic for every event on every function call, while `rustitude` just needs to look up a value in an array!
 - The majority of the library (the public interface) has Python bindings, so if there is no need for custom amplitudes, a developer never actually has to write any Rust code, and the resulting calculations will be as performant as if they were written in Rust.
 
 # Theory
 
 Amplitudes are registered into a named `sum` and `group`. Similar to `AmpTools`, the typical calculation for any event $e$ and list of parameters $\overrightarrow{p}$ will then be:
+
 ```math
 I(\overrightarrow{p}, e) = \sum_{\text{groups} \in \text{sums}}\left|\sum_{\text{amplitudes} \in \text{groups}} \prod_{\text{amp} \in \text{amplitudes}} \text{amp}(\overrightarrow{p}, e)\right|^2
 ```
 
 # Installation
+
 Adding `rustitude` to an existing Rust project is as simple as
+
 ```shell
 cargo add rustitude
 ```
 
 The Python installation is equally straightforward:
+
 ```shell
 pip install rustitude
 ```
 
 # Usage
-See the [`rustitude-core`](https://github.com/denehoffman/rustitude-core) crate for a more in-depth tutorial on writing custom amplitudes in Rust. This package is mostly focused on the Python side of things. Here is the setup for an example analysis:
+
+See the [`rustitude-core`](https://github.com/denehoffman/rustitude/tree/main/crates/rustitude-core) crate for a more in-depth tutorial on writing custom amplitudes in Rust. This package is mostly focused on the Python side of things. Here is the setup for an example analysis:
+
 ```python
 import rustitude as rt
 from rustitude import gluex
 import numpy as np
 
-# Load data files
-# This uses uproot under the hood
+# Start by creating some amplitudes:
+f0p = gluex.resonances.KMatrixF0('f0+', channel=2)
+f0n = gluex.resonances.KMatrixF0('f0-', channel=2)
+f2 = gluex.resonances.KMatrixF2('f2', channel=2)
+a0p = gluex.resonances.KMatrixA0('a0+', channel=1)
+a0n = gluex.resonances.KMatrixA0('a0-', channel=1)
+a2 = gluex.resonances.KMatrixA2('a2', channel=1)
+s0p = gluex.harmonics.Zlm('Z00+', 0, 0, reflectivity='+')
+s0n = gluex.harmonics.Zlm('Z00-', 0, 0, reflectivity='-')
+d2p = gluex.harmonics.Zlm('Z22+', 2, 2, reflectivity='+')
+
+# Next, let's put them together into a model
+# The API supports addition, and multiplication and has additional methods for the absolute-square (`norm_sqr`), real part (`real`) and imaginary part (`imag`).
+pos_re_sum = (f0p + a0p) * s0p.real() + (f2 + a2) * d2p.real()
+pos_im_sum = (f0p + a0p) * s0p.imag() + (f2 + a2) * d2p.imag()
+neg_re_sum = (f0n + a0n) * s0n.real()
+neg_im_sum = (f0n + a0n) * s0n.imag()
+
+mod = rt.Model(pos_re_sum.norm_sqr() + pos_im_sum.norm_sqr() + neg_re_sum.norm_sqr() + neg_im_sum.norm_sqr())
+
+# There is no need to constrain amplitudes, since each named amplitude is only ever evaluated once and a cached value gets pulled if we run across an amplitude by the same name!
+# We should, however, fix some of the values to make the fit less ambiguous. For instance, suppose we are above the threshold for the f_0(500) which is included in the F0 K-Matrix:
+mod.fix("f0+", "f0_500 re", 0.0)
+mod.fix("f0+", "f0_500 im", 0.0)
+mod.fix("f0-", "f0_500 re", 0.0)
+mod.fix("f0-", "f0_500 im", 0.0)
+
+# As mentioned, we should also fix at least one complex phase per coherent sum:
+mod.fix("f0+", "f0_980 im", 0.0)
+mod.fix("f0-", "f0_980 im", 0.0)
+
+# All done! Now let's load our model into a Manager, which helps coordinate the model with datasets.
+# First, load up some datasets. rustitude provides an open operation that uses uproot under the hood:
 ds = rt.open('data.root')
 ds_mc = rt.open('mc.root')
 
-# Create a new "manager" to handle the interface between data and amplitudes
-m = rt.ExtendedLogLikelihood(ds, ds_mc)
+m_data = rt.Manager(mod, ds)
+m_mc = rt.Manager(mod, ds_mc)
+
+# We could stop here and evaluate just one dataset at a time:
+
+# res = m_data([1.0, 3.4, 2.8, -3.6, ... ])
+# -> [5.3, 0.2, ...], a list of intensities from the amplitude calculation
+
+# Or, what we probably want to do is find the negative log-likelihood for some choice of parameters:
 
-# Register some amplitudes
-# We provide a sum name, group name, and a named amplitude
-# This function also runs the precalculation method over the datasets
-m.register('pos re', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
-m.register('pos re', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
-m.register('pos re', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='+', part='real'))
-m.register('pos re', 'D', gluex.resonances.KMatrixF2('f2', channel=2))
-m.register('pos re', 'D', gluex.resonances.KMatrixA2('a2', channel=1))
-m.register('pos re', 'D', gluex.harmonics.Zlm('z22', 0, 0, reflectivity='+', part='real'))
-
-m.register('pos im', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
-m.register('pos im', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
-m.register('pos im', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='+', part='imag'))
-m.register('pos im', 'D', gluex.resonances.KMatrixF2('f2', channel=2))
-m.register('pos im', 'D', gluex.resonances.KMatrixA2('a2', channel=1))
-m.register('pos im', 'D', gluex.harmonics.Zlm('z22', 0, 0, reflectivity='+', part='imag'))
-
-# We can constrain all the free parameters of one amplitude to be equal to those of another,
-# provided they have the same free parameters. To constrain an individual amplitude, we can use
-# m.constrain(('pos re', 'S', 'f0', 'f0_500 re'), ('pos re', 'S', 'f0', 'f0_500 im')) for example,
-# which would make the real and imaginary part of equal to each other in the calculation.
-# This step reduces the number of free parameters in the calculation.
-m.constrain_amplitude(('pos re', 'S', 'f0'), ('pos im', 'S', 'f0'))
-m.constrain_amplitude(('pos re', 'S', 'a0'), ('pos im', 'S', 'a0'))
-m.constrain_amplitude(('pos re', 'D', 'f2'), ('pos im', 'D', 'f2'))
-m.constrain_amplitude(('pos re', 'D', 'a2'), ('pos im', 'D', 'a2'))
-
-# Fix some parameters to a given value (zero in this case)
-m.fix(('pos re', 'S', 'f0', 'f0_500 re'), 0.0)
-m.fix(('pos re', 'S', 'f0', 'f0_500 im'), 0.0)
-m.fix(('pos re', 'S', 'f0', 'f0_980 im'), 0.0)
-
-m.register('neg re', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
-m.register('neg re', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
-m.register('neg re', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='-', part='real'))
-
-m.register('neg im', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
-m.register('neg im', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
-m.register('neg im', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='-', part='imag'))
-
-m.constrain_amplitude(('neg re', 'S', 'f0'), ('neg im', 'S', 'f0'))
-m.constrain_amplitude(('neg re', 'S', 'a0'), ('neg im', 'S', 'a0'))
-
-m.fix(('neg re', 'S', 'f0', 'f0_500 re'), 0.0)
-m.fix(('neg re', 'S', 'f0', 'f0_500 im'), 0.0)
-m.fix(('neg re', 'S', 'f0', 'f0_980 im'), 0.0)
-
-# Calculate the negative log-likelihood given some random input parameters:
-rng = np.random.default_rng()
-nll = m(rng.random(len(m.parameters())) * 100.0)
+nll = rt.ExtendedLogLikelihood(m_data, m_mc)
+
+res = nll([10.0] * mod.get_n_free())
+print(res) # prints some value for the NLL
 ```
 
-See the [`rustitude-gluex`](https://github.com/denehoffman/rustitude-gluex) package for some of the currently implemented amplitudes (derived from GlueX's [halld_sim](https://github.com/JeffersonLab/halld_sim) repo). There are also some helper methods `scalar`, `cscalar`, and `pcscalar` to create amplitudes which represent a single free parameter, a single complex free parameter, and a single complex free parameter in polar coordinates respectively.
+See the [`rustitude-gluex`](https://github.com/denehoffman/rustitude/tree/main/crates/rustitude-gluex) package for some of the currently implemented amplitudes (derived from GlueX's [halld_sim](https://github.com/JeffersonLab/halld_sim) repo). There are also some helper methods `Scalar`, `CScalar`, and `PCScalar` to create amplitudes which represent a single free parameter, a single complex free parameter, and a single complex free parameter in polar coordinates respectively.
 
 # TODOs
+
 In no particular order, here is a list of what (probably) needs to be done before I will stop making any breaking changes:
+
 - Pure Rust parsing of ROOT files without the `uproot` backend (I have some moderate success with `oxyroot`, but there are still a few issues reading larger files)
 - Add plotting methods
 - A way to check if the number of parameters matches the input at compile time would be nice, not sure if it's possible though
 - Give managers a way to apply amplitudes to new datasets, like using the result from a fit to weight some generated Monte-Carlo for plotting the result. This is possible to do through Python, but a convenience method is probably needed
 - Lots of documentation
 - Lots of tests
```

#### html2text {}

```diff
@@ -75,69 +75,59 @@
 for any event $e$ and list of parameters $\overrightarrow{p}$ will then be:
 ```math I(\overrightarrow{p}, e) = \sum_{\text{groups} \in \text
 {sums}}\left|\sum_{\text{amplitudes} \in \text{groups}} \prod_{\text{amp} \in
 \text{amplitudes}} \text{amp}(\overrightarrow{p}, e)\right|^2 ``` #
 Installation Adding `rustitude` to an existing Rust project is as simple as
 ```shell cargo add rustitude ``` The Python installation is equally
 straightforward: ```shell pip install rustitude ``` # Usage See the
-[`rustitude-core`](https://github.com/denehoffman/rustitude-core) crate for a
-more in-depth tutorial on writing custom amplitudes in Rust. This package is
-mostly focused on the Python side of things. Here is the setup for an example
-analysis: ```python import rustitude as rt from rustitude import gluex import
-numpy as np # Load data files # This uses uproot under the hood ds = rt.open
-('data.root') ds_mc = rt.open('mc.root') # Create a new "manager" to handle the
-interface between data and amplitudes m = rt.ExtendedLogLikelihood(ds, ds_mc) #
-Register some amplitudes # We provide a sum name, group name, and a named
-amplitude # This function also runs the precalculation method over the datasets
-m.register('pos re', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
-m.register('pos re', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
-m.register('pos re', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='+',
-part='real')) m.register('pos re', 'D', gluex.resonances.KMatrixF2('f2',
-channel=2)) m.register('pos re', 'D', gluex.resonances.KMatrixA2('a2',
-channel=1)) m.register('pos re', 'D', gluex.harmonics.Zlm('z22', 0, 0,
-reflectivity='+', part='real')) m.register('pos im', 'S',
-gluex.resonances.KMatrixF0('f0', channel=2)) m.register('pos im', 'S',
-gluex.resonances.KMatrixA0('a0', channel=1)) m.register('pos im', 'S',
-gluex.harmonics.Zlm('z00', 0, 0, reflectivity='+', part='imag')) m.register
-('pos im', 'D', gluex.resonances.KMatrixF2('f2', channel=2)) m.register('pos
-im', 'D', gluex.resonances.KMatrixA2('a2', channel=1)) m.register('pos im',
-'D', gluex.harmonics.Zlm('z22', 0, 0, reflectivity='+', part='imag')) # We can
-constrain all the free parameters of one amplitude to be equal to those of
-another, # provided they have the same free parameters. To constrain an
-individual amplitude, we can use # m.constrain(('pos re', 'S', 'f0', 'f0_500
-re'), ('pos re', 'S', 'f0', 'f0_500 im')) for example, # which would make the
-real and imaginary part of equal to each other in the calculation. # This step
-reduces the number of free parameters in the calculation. m.constrain_amplitude
-(('pos re', 'S', 'f0'), ('pos im', 'S', 'f0')) m.constrain_amplitude(('pos re',
-'S', 'a0'), ('pos im', 'S', 'a0')) m.constrain_amplitude(('pos re', 'D', 'f2'),
-('pos im', 'D', 'f2')) m.constrain_amplitude(('pos re', 'D', 'a2'), ('pos im',
-'D', 'a2')) # Fix some parameters to a given value (zero in this case) m.fix(
-('pos re', 'S', 'f0', 'f0_500 re'), 0.0) m.fix(('pos re', 'S', 'f0', 'f0_500
-im'), 0.0) m.fix(('pos re', 'S', 'f0', 'f0_980 im'), 0.0) m.register('neg re',
-'S', gluex.resonances.KMatrixF0('f0', channel=2)) m.register('neg re', 'S',
-gluex.resonances.KMatrixA0('a0', channel=1)) m.register('neg re', 'S',
-gluex.harmonics.Zlm('z00', 0, 0, reflectivity='-', part='real')) m.register
-('neg im', 'S', gluex.resonances.KMatrixF0('f0', channel=2)) m.register('neg
-im', 'S', gluex.resonances.KMatrixA0('a0', channel=1)) m.register('neg im',
-'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='-', part='imag'))
-m.constrain_amplitude(('neg re', 'S', 'f0'), ('neg im', 'S', 'f0'))
-m.constrain_amplitude(('neg re', 'S', 'a0'), ('neg im', 'S', 'a0')) m.fix(('neg
-re', 'S', 'f0', 'f0_500 re'), 0.0) m.fix(('neg re', 'S', 'f0', 'f0_500 im'),
-0.0) m.fix(('neg re', 'S', 'f0', 'f0_980 im'), 0.0) # Calculate the negative
-log-likelihood given some random input parameters: rng = np.random.default_rng
-() nll = m(rng.random(len(m.parameters())) * 100.0) ``` See the [`rustitude-
-gluex`](https://github.com/denehoffman/rustitude-gluex) package for some of the
-currently implemented amplitudes (derived from GlueX's [halld_sim](https://
-github.com/JeffersonLab/halld_sim) repo). There are also some helper methods
-`scalar`, `cscalar`, and `pcscalar` to create amplitudes which represent a
-single free parameter, a single complex free parameter, and a single complex
-free parameter in polar coordinates respectively. # TODOs In no particular
-order, here is a list of what (probably) needs to be done before I will stop
-making any breaking changes: - Pure Rust parsing of ROOT files without the
-`uproot` backend (I have some moderate success with `oxyroot`, but there are
-still a few issues reading larger files) - Add plotting methods - A way to
-check if the number of parameters matches the input at compile time would be
-nice, not sure if it's possible though - Give managers a way to apply
-amplitudes to new datasets, like using the result from a fit to weight some
-generated Monte-Carlo for plotting the result. This is possible to do through
-Python, but a convenience method is probably needed - Lots of documentation -
-Lots of tests
+[`rustitude-core`](https://github.com/denehoffman/rustitude/tree/main/crates/
+rustitude-core) crate for a more in-depth tutorial on writing custom amplitudes
+in Rust. This package is mostly focused on the Python side of things. Here is
+the setup for an example analysis: ```python import rustitude as rt from
+rustitude import gluex import numpy as np # Start by creating some amplitudes:
+f0p = gluex.resonances.KMatrixF0('f0+', channel=2) f0n =
+gluex.resonances.KMatrixF0('f0-', channel=2) f2 = gluex.resonances.KMatrixF2
+('f2', channel=2) a0p = gluex.resonances.KMatrixA0('a0+', channel=1) a0n =
+gluex.resonances.KMatrixA0('a0-', channel=1) a2 = gluex.resonances.KMatrixA2
+('a2', channel=1) s0p = gluex.harmonics.Zlm('Z00+', 0, 0, reflectivity='+') s0n
+= gluex.harmonics.Zlm('Z00-', 0, 0, reflectivity='-') d2p = gluex.harmonics.Zlm
+('Z22+', 2, 2, reflectivity='+') # Next, let's put them together into a model #
+The API supports addition, and multiplication and has additional methods for
+the absolute-square (`norm_sqr`), real part (`real`) and imaginary part
+(`imag`). pos_re_sum = (f0p + a0p) * s0p.real() + (f2 + a2) * d2p.real()
+pos_im_sum = (f0p + a0p) * s0p.imag() + (f2 + a2) * d2p.imag() neg_re_sum =
+(f0n + a0n) * s0n.real() neg_im_sum = (f0n + a0n) * s0n.imag() mod = rt.Model
+(pos_re_sum.norm_sqr() + pos_im_sum.norm_sqr() + neg_re_sum.norm_sqr() +
+neg_im_sum.norm_sqr()) # There is no need to constrain amplitudes, since each
+named amplitude is only ever evaluated once and a cached value gets pulled if
+we run across an amplitude by the same name! # We should, however, fix some of
+the values to make the fit less ambiguous. For instance, suppose we are above
+the threshold for the f_0(500) which is included in the F0 K-Matrix: mod.fix
+("f0+", "f0_500 re", 0.0) mod.fix("f0+", "f0_500 im", 0.0) mod.fix("f0-",
+"f0_500 re", 0.0) mod.fix("f0-", "f0_500 im", 0.0) # As mentioned, we should
+also fix at least one complex phase per coherent sum: mod.fix("f0+", "f0_980
+im", 0.0) mod.fix("f0-", "f0_980 im", 0.0) # All done! Now let's load our model
+into a Manager, which helps coordinate the model with datasets. # First, load
+up some datasets. rustitude provides an open operation that uses uproot under
+the hood: ds = rt.open('data.root') ds_mc = rt.open('mc.root') m_data =
+rt.Manager(mod, ds) m_mc = rt.Manager(mod, ds_mc) # We could stop here and
+evaluate just one dataset at a time: # res = m_data([1.0, 3.4, 2.8, -3.6, ...
+]) # -> [5.3, 0.2, ...], a list of intensities from the amplitude calculation #
+Or, what we probably want to do is find the negative log-likelihood for some
+choice of parameters: nll = rt.ExtendedLogLikelihood(m_data, m_mc) res = nll(
+[10.0] * mod.get_n_free()) print(res) # prints some value for the NLL ``` See
+the [`rustitude-gluex`](https://github.com/denehoffman/rustitude/tree/main/
+crates/rustitude-gluex) package for some of the currently implemented
+amplitudes (derived from GlueX's [halld_sim](https://github.com/JeffersonLab/
+halld_sim) repo). There are also some helper methods `Scalar`, `CScalar`, and
+`PCScalar` to create amplitudes which represent a single free parameter, a
+single complex free parameter, and a single complex free parameter in polar
+coordinates respectively. # TODOs In no particular order, here is a list of
+what (probably) needs to be done before I will stop making any breaking
+changes: - Pure Rust parsing of ROOT files without the `uproot` backend (I have
+some moderate success with `oxyroot`, but there are still a few issues reading
+larger files) - Add plotting methods - A way to check if the number of
+parameters matches the input at compile time would be nice, not sure if it's
+possible though - Give managers a way to apply amplitudes to new datasets, like
+using the result from a fit to weight some generated Monte-Carlo for plotting
+the result. This is possible to do through Python, but a convenience method is
+probably needed - Lots of documentation - Lots of tests
```

### Comparing `rustitude-0.3.4/bacon.toml` & `rustitude-0.4.0/bacon.toml`

 * *Files identical despite different names*

### Comparing `rustitude-0.3.4/media/logo.png` & `rustitude-0.4.0/crates/rustitude-core/media/logo.png`

 * *Files identical despite different names*

### Comparing `rustitude-0.3.4/rustitude/__init__.py` & `rustitude-0.4.0/rustitude/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,41 +2,48 @@
 
 from pathlib import Path
 
 import numpy as np
 import uproot
 
 from ._rustitude import amplitude, dataset, four_momentum, gluex, manager
-from .amplitude import cscalar, pcscalar, scalar
-from .dataset import Dataset
-from .manager import ExtendedLogLikelihood, Manager, MultiManager
+from .amplitude import CScalar, PCScalar, Scalar, PiecewiseM, AmpOp, Parameter, Model, Amplitude
+from .dataset import Event, Dataset
+from .manager import ExtendedLogLikelihood, Manager
 
 __all__ = [
     'dataset',
     'manager',
     'amplitude',
     'four_momentum',
+    'Event',
     'Dataset',
     'Manager',
-    'MultiManager',
     'ExtendedLogLikelihood',
-    'scalar',
-    'cscalar',
-    'pcscalar',
+    'Amplitude',
+    'Scalar',
+    'CScalar',
+    'PCScalar',
+    'PiecewiseM',
+    'AmpOp',
+    'Parameter',
+    'Model',
     'gluex',
     'open',
 ]
 
 
 def __dir__():
     return __all__
 
 
 # TODO: add a method to calculate EPS from a given polarization angle and amount
-def open(file_name: str | Path, tree_name: str | None = None, *, pol_in_beam: bool = False) -> Dataset:  # noqa: A001
+def open(
+    file_name: str | Path, tree_name: str | None = None, *, pol_in_beam: bool = False
+) -> Dataset:  # noqa: A001
     filepath = (file_name if isinstance(file_name, Path) else Path(file_name)).resolve()
     tfile = uproot.open(filepath)
     ttree = tfile[tree_name] if tree_name else tfile.get(tfile.keys()[0])
     requested_branches = [
         'E_Beam',
         'Px_Beam',
         'Py_Beam',
```

### Comparing `rustitude-0.3.4/rustitude/gluex/harmonics.pyi` & `rustitude-0.4.0/rustitude/gluex/harmonics.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,120 @@
 from typing import Literal, overload
 
-from rustitude import Amplitude
+from rustitude import AmpOp
 
 @overload
 def Ylm(
     name: str,
     l: Literal[0],  # noqa: E741
     m: Literal[0],
-    part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
 @overload
 def Ylm(
     name: str,
     l: Literal[1],  # noqa: E741
     m: Literal[-1, 0, 1],
-    part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
 @overload
 def Ylm(
     name: str,
     l: Literal[2],  # noqa: E741
     m: Literal[-2, -1, 0, 1, 2],
-    part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
 @overload
 def Ylm(
     name: str,
     l: Literal[3],  # noqa: E741
     m: Literal[-3, -2, -1, 0, 1, 2, 3],
-    part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
 @overload
 def Zlm(
     name: str,
     l: Literal[0],  # noqa: E741
     m: Literal[0],
-    reflectivity: Literal['positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'] = 'positive',
-    part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
+    reflectivity: Literal[
+        'positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'
+    ] = 'positive',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
 @overload
 def Zlm(
     name: str,
     l: Literal[1],  # noqa: E741
     m: Literal[-1, 0, 1],
-    reflectivity: Literal['positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'] = 'positive',
-    part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
+    reflectivity: Literal[
+        'positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'
+    ] = 'positive',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
 @overload
 def Zlm(
     name: str,
     l: Literal[2],  # noqa: E741
     m: Literal[-2, -1, 0, 1, 2],
-    reflectivity: Literal['positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'] = 'positive',
-    part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
+    reflectivity: Literal[
+        'positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'
+    ] = 'positive',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
 @overload
 def Zlm(
     name: str,
     l: Literal[3],  # noqa: E741
     m: Literal[-3, -2, -1, 0, 1, 2, 3],
-    reflectivity: Literal['positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'] = 'positive',
-    part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
+    reflectivity: Literal[
+        'positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'
+    ] = 'positive',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
 def OnePS(  # noqa: N802
     name: str,
-    reflectivity: Literal['positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'] = 'positive',
-    part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
+    reflectivity: Literal[
+        'positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'
+    ] = 'positive',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
 @overload
 def TwoPS(
     name: str,
     l: Literal[0],  # noqa: E741
     m: Literal[0],
-    reflectivity: Literal['positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'] = 'positive',
-    part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
+    reflectivity: Literal[
+        'positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'
+    ] = 'positive',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
 @overload
 def TwoPS(
     name: str,
     l: Literal[1],  # noqa: E741
     m: Literal[-1, 0, 1],
-    reflectivity: Literal['positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'] = 'positive',
+    reflectivity: Literal[
+        'positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'
+    ] = 'positive',
     part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
 @overload
 def TwoPS(
     name: str,
     l: Literal[2],  # noqa: E741
     m: Literal[-2, -1, 0, 1, 2],
-    reflectivity: Literal['positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'] = 'positive',
-    part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
+    reflectivity: Literal[
+        'positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'
+    ] = 'positive',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
 @overload
 def TwoPS(
     name: str,
     l: Literal[3],  # noqa: E741
     m: Literal[-3, -2, -1, 0, 1, 2, 3],
-    reflectivity: Literal['positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'] = 'positive',
-    part: Literal['real', 're', 'imaginary', 'imag', 'im', 'both'] = 'real',
+    reflectivity: Literal[
+        'positive', 'pos', 'p', '+', 'plus', 'negative', 'neg', 'n', '-', 'minus', 'm'
+    ] = 'positive',
     frame: Literal['helicity', 'hx', 'gottfried-jackson', 'gj'] = 'helicity',
-) -> Amplitude: ...
+) -> AmpOp: ...
```

### Comparing `rustitude-0.3.4/rustitude/gluex/resonances.pyi` & `rustitude-0.4.0/rustitude/gluex/resonances.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from rustitude import Amplitude
+from rustitude import AmpOp
 
-def BreitWigner(name: str, p1_indices: list[int], p2_indices: list[int]) -> Amplitude: ...  # noqa: N802
-def KMatrixA0(name: str, channel: int) -> Amplitude: ...  # noqa: N802
-def KMatrixA2(name: str, channel: int) -> Amplitude: ...  # noqa: N802
-def KMatrixF0(name: str, channel: int) -> Amplitude: ...  # noqa: N802
-def KMatrixF2(name: str, channel: int) -> Amplitude: ...  # noqa: N802
-def KMatrixPi1(name: str, channel: int) -> Amplitude: ...  # noqa: N802
-def KMatrixRho(name: str, channel: int) -> Amplitude: ...  # noqa: N802
+
+def BreitWigner(name: str, p1_indices: list[int], p2_indices: list[int]) -> AmpOp: ...  # noqa: N802
+def KMatrixA0(name: str, channel: int) -> AmpOp: ...  # noqa: N802
+def KMatrixA2(name: str, channel: int) -> AmpOp: ...  # noqa: N802
+def KMatrixF0(name: str, channel: int) -> AmpOp: ...  # noqa: N802
+def KMatrixF2(name: str, channel: int) -> AmpOp: ...  # noqa: N802
+def KMatrixPi1(name: str, channel: int) -> AmpOp: ...  # noqa: N802
+def KMatrixRho(name: str, channel: int) -> AmpOp: ...  # noqa: N802
```

### Comparing `rustitude-0.3.4/src/lib.rs` & `rustitude-0.4.0/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pub mod prelude {
     pub use rustitude_core::prelude::*;
 }
 pub mod gluex {
     pub use rustitude_gluex::*;
 }
 
-fn add_submodule<F>(parent: &Bound<'_, PyModule>, name: &str, mod_init: F) -> PyResult<()>
+pub fn add_submodule<F>(parent: &Bound<'_, PyModule>, name: &str, mod_init: F) -> PyResult<()>
 where
     F: Fn(&Bound<'_, PyModule>) -> PyResult<()>,
 {
     let child_module = PyModule::new_bound(parent.py(), name)?;
     mod_init(&child_module)?;
     parent.add(name.split('.').last().unwrap(), &child_module)?;
     parent
```

### Comparing `rustitude-0.3.4/Cargo.lock` & `rustitude-0.4.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -222,17 +222,17 @@
 name = "bumpalo"
 version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
+checksum = "78834c15cb5d5efe3452d58b1e8ba890dd62d21907f867f383358198e56ebca5"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
@@ -696,55 +696,54 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3135b08af27d103b0a51f2ae0f8632117b7b185ccf931445affa8df530576a41"
+checksum = "35bd024e8b2ff75562e5f34e7f4905839deb4b22955ef5e73d2fea1b9813cb23"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
+checksum = "c165a9ab64cf766f73521c0dd2cfdff64f488b8f0b3e621face3462d3db536d7"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-derive"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed3955f1a9c7c0c15e092f9c887db08b1fc683305fdf6eb6684f22555355e202"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
@@ -761,19 +760,18 @@
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+checksum = "f83d14da390562dca69fc84082e73e548e1ad308d24accdedd2720017cb37824"
 dependencies = [
- "autocfg",
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
@@ -876,17 +874,17 @@
  "thrift",
  "twox-hash",
  "zstd",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
 
 [[package]]
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
@@ -920,17 +918,17 @@
  "primal-bit",
  "primal-estimate",
  "smallvec",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.21.2"
@@ -974,28 +972,28 @@
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
@@ -1074,60 +1072,60 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustitude"
-version = "0.3.4"
+version = "0.4.0"
 dependencies = [
  "pyo3",
  "rayon",
  "rustitude-core",
  "rustitude-gluex",
 ]
 
 [[package]]
 name = "rustitude-core"
-version = "0.3.4"
-source = "git+https://github.com/denehoffman/rustitude-core.git#c8943f2cec72300c0a0de4fb283367ac8df4f1e4"
+version = "1.0.0"
 dependencies = [
  "approx",
  "indexmap",
  "itertools",
  "nalgebra",
  "num",
  "num-complex",
  "num-traits",
  "oxyroot",
  "parking_lot",
  "parquet",
  "pyo3",
  "rayon",
+ "sphrs",
+ "thiserror",
 ]
 
 [[package]]
 name = "rustitude-gluex"
-version = "0.1.5"
-source = "git+https://github.com/denehoffman/rustitude-gluex.git#f2f72ff64a12806352534459cc3faa6ebdbdb449"
+version = "0.2.0"
 dependencies = [
  "factorial",
  "nalgebra",
  "num-complex",
  "pyo3",
  "rayon",
  "rustitude-core",
  "sphrs",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "safe_arch"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f398075ce1e6a179b46f51bd88d0598b92b00d3551f1a2d4ac49e771b56ac354"
 dependencies = [
@@ -1138,17 +1136,17 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
-version = "1.0.22"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
+checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 
 [[package]]
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
@@ -1203,30 +1201,50 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "bf5be731623ca1a1fb7d8be6f261a3be6d3e2337b8a1f97be944d020c8fcb704"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
+name = "thiserror"
+version = "1.0.60"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
+dependencies = [
+ "thiserror-impl",
+]
+
+[[package]]
+name = "thiserror-impl"
+version = "1.0.60"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.63",
+]
+
+[[package]]
 name = "thrift"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
 dependencies = [
  "byteorder",
  "integer-encoding",
@@ -1316,15 +1334,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1338,30 +1356,30 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "wide"
-version = "0.7.17"
+version = "0.7.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f0e39d2c603fdc0504b12b458cf1f34e0b937ed2f4f2dc20796e3e86f34e11f"
+checksum = "aab6594190de06d718a5dbc5fa781ab62f8903797056480e549ca74add6b7065"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "windows-core"
@@ -1443,30 +1461,30 @@
 checksum = "388c44dc09d76f1536602ead6d325eb532f5c122f17782bd57fb47baeeb767e2"
 dependencies = [
  "lzma-sys",
 ]
 
 [[package]]
 name = "zerocopy"
-version = "0.7.33"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "087eca3c1eaf8c47b94d02790dd086cd594b912d2043d4de4bfdd466b3befb7c"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.33"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f4b6c273f496d8fd4eaf18853e6b448760225dc030ff2c485a786859aea6393"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "zstd"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
```

### Comparing `rustitude-0.3.4/pyproject.toml` & `rustitude-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.maturin]
 module-name = "rustitude._rustitude"
 features = ["pyo3/extension-module"]
 
 [project]
 name = "rustitude"
-version = "0.3.4"
+version = "0.4.0"
 description = "Python bindings for the Rustitude library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["physics", "math", "rust"]
 authors = [{ email = "dene@cmu.edu" }, { name = "Nathaniel Dene Hoffman" }]
 maintainers = [{ name = "Nathaniel Dene Hoffman", email = "dene@cmu.edu" }]
@@ -24,7 +24,15 @@
 dependencies = ["uproot", "numpy"]
 
 [project.urls]
 homepage = "https://github.com/denehoffman/rustitude"
 repository = "https://github.com/denehoffman/rustitude"
 changelog = "https://github.com/denehoffman/rustitude/blob/main/CHANGELOG.md"
 # TODO: documentation = "readthedocs.org"
+
+[tool.ruff]
+line-length = 100
+
+[tool.ruff.format]
+quote-style = "single"
+docstring-code-format = true
+preview = true
```

### Comparing `rustitude-0.3.4/PKG-INFO` & `rustitude-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rustitude
-Version: 0.3.4
+Version: 0.4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Dist: uproot
 Requires-Dist: numpy
 License-File: LICENSE
 Summary: Python bindings for the Rustitude library
 Keywords: physics,math,rust
@@ -39,121 +39,123 @@
   <a href="https://crates.io/crates/rustitude" alt="Rustitude on crates.io">
     <img src="https://img.shields.io/crates/v/rustitude" /></a>
   <a href="https://docs.rs/rustitude" alt="Rustitude documentation on docs.rs">
     <img src="https://img.shields.io/docsrs/rustitude" /></a>
 </p>
 
 ### Table of Contents:
+
 - [Introduction](#Introduction)
 - [Theory](#Theory)
 - [Installation](#Installation)
 - [Usage](#Usage)
 - [TODOs](#TODOs)
 
 # Introduction
+
 This project began with a desire to make a fast but easy to use interface for fitting amplitudes to particle physics data. That being said, there are performant methods such as [`AmpTools`](https://github.com/mashephe/AmpTools), which is written in C++, but in my personal experience, it can be a bit tricky to use and extend, and it generally requires a lot of boilerplate code to generate new amplitudes or plotting scripts. On the other hand, there are also libraries like [`PyPWA`](https://github.com/JeffersonLab/PyPWA/) (written in Python) which seem like they could be easy to use, but often fail in this aspect due to Python's limiting syntax, speed issues, and a general lack of documentation and ongoing development. There have been attempts to bridge the gap between AmpTools and Python, most recently (and successfully) [`PyAmpTools`](https://github.com/lan13005/PyAmpTools). The difficulty with this method is that it relies on PyROOT, which also means you need ROOT installed (and built with your version of Python). For now, I'll spare you the anti-ROOT rant and just say that ROOT should be an opt-in, not a requirement. So where does that leave `rustitude`?
 
 As the name suggests, `rustitude` was written in Rust, so let's get the obvious downside out of the way: not many particle physicists know how to write Rust code. Hopefully, this will change over the next decade (and there has already been some [support](https://www.whitehouse.gov/oncd/briefing-room/2024/02/26/memory-safety-statements-of-support/) from the US government, of all places). While Rust carries the disadvantage of relative obscurity compared to C++, it also has many benefits. No `null` means no null references (Tony Hoare's ["billion dollar mistake"](https://web.archive.org/web/20090628071208/http://qconlondon.com/london-2009/speaker/Tony+Hoare)). Pointers (called references in Rust) are always valid, a guarantee made by a very helpful and only occasionally frustrating borrow checker. Rust "crates" are set up in a way which encourages documentation (see [`rustitude-core`'s documentation](https://docs.rs/rustitude-core/)), and the basic syntax is fairly easy to learn for people who have been using optional type checking in Python. Perhaps one of the biggest benefits of Rust is how easy it is to employ [parallelization](https://crates.io/crates/rayon), but the two reasons I like it most are that it's incredibly easy to write Python bindings (that's what this library is after all) and it has a package manager. This second point is important -- unlike C/C++, where a developer is swamped with some menagerie `Makefile`, `CMakeLists.txt`, or some `scons` monstrosity which may only work on "X" system and only if you install and use `make`, `cmake`, `g++`, or whatever (oh yeah, and you made sure all your external dependencies are linked correctly, right? Right?), Rust supports adding a package by simply adding a line to `Cargo.toml` (or using the `cargo add` command). In many ways, package management in Rust is actually simpler than Python, since there's only one prefered method of creating and managing projects, formatting, linting, and compiling.
 
 Now I've covered why I don't like some of the existing solutions, and why I chose to use Rust, but what does this project have that makes it stand out? Here are some reasons to entice you:
 
 - `rustitude` will automatically parallelize amplitudes over the events in a dataset. There's no reason for a developer to ever write parallelized code themselves.
 - Implementing [`Node`](https://docs.rs/rustitude-core/latest/rustitude_core/amplitude/trait.Node.html) on a struct is all that is needed to use it as an amplitude. This means developers need only write two to three total methods to describe the entire functionality of their amplitude, and one of these just gives the names and order of the amplitude's input parameters.
 - A major goal of `rustitude` was to increase processing speed by sacrificing memory. This is done by precalculating parts of amplitudes which don't change when the free parameter inputs change. `AmpTools` supports a version of this, but only on the level of each general amplitude rather than on an individual basis. The simplest example of this is the `Ylm` amplitude (spherical harmonic), which can be entirely precalculated given the value of `l` and `m`. In `AmpTools`, different instances of `Ylm` with different `l`s and `m`s share precalculated data, whereas in `rustitude`, they don't. The `AmpTools` implementation of `Ylm` needs to calculate a spherical harmonic for every event on every function call, while `rustitude` just needs to look up a value in an array!
 - The majority of the library (the public interface) has Python bindings, so if there is no need for custom amplitudes, a developer never actually has to write any Rust code, and the resulting calculations will be as performant as if they were written in Rust.
 
 # Theory
 
 Amplitudes are registered into a named `sum` and `group`. Similar to `AmpTools`, the typical calculation for any event $e$ and list of parameters $\overrightarrow{p}$ will then be:
+
 ```math
 I(\overrightarrow{p}, e) = \sum_{\text{groups} \in \text{sums}}\left|\sum_{\text{amplitudes} \in \text{groups}} \prod_{\text{amp} \in \text{amplitudes}} \text{amp}(\overrightarrow{p}, e)\right|^2
 ```
 
 # Installation
+
 Adding `rustitude` to an existing Rust project is as simple as
+
 ```shell
 cargo add rustitude
 ```
 
 The Python installation is equally straightforward:
+
 ```shell
 pip install rustitude
 ```
 
 # Usage
-See the [`rustitude-core`](https://github.com/denehoffman/rustitude-core) crate for a more in-depth tutorial on writing custom amplitudes in Rust. This package is mostly focused on the Python side of things. Here is the setup for an example analysis:
+
+See the [`rustitude-core`](https://github.com/denehoffman/rustitude/tree/main/crates/rustitude-core) crate for a more in-depth tutorial on writing custom amplitudes in Rust. This package is mostly focused on the Python side of things. Here is the setup for an example analysis:
+
 ```python
 import rustitude as rt
 from rustitude import gluex
 import numpy as np
 
-# Load data files
-# This uses uproot under the hood
+# Start by creating some amplitudes:
+f0p = gluex.resonances.KMatrixF0('f0+', channel=2)
+f0n = gluex.resonances.KMatrixF0('f0-', channel=2)
+f2 = gluex.resonances.KMatrixF2('f2', channel=2)
+a0p = gluex.resonances.KMatrixA0('a0+', channel=1)
+a0n = gluex.resonances.KMatrixA0('a0-', channel=1)
+a2 = gluex.resonances.KMatrixA2('a2', channel=1)
+s0p = gluex.harmonics.Zlm('Z00+', 0, 0, reflectivity='+')
+s0n = gluex.harmonics.Zlm('Z00-', 0, 0, reflectivity='-')
+d2p = gluex.harmonics.Zlm('Z22+', 2, 2, reflectivity='+')
+
+# Next, let's put them together into a model
+# The API supports addition, and multiplication and has additional methods for the absolute-square (`norm_sqr`), real part (`real`) and imaginary part (`imag`).
+pos_re_sum = (f0p + a0p) * s0p.real() + (f2 + a2) * d2p.real()
+pos_im_sum = (f0p + a0p) * s0p.imag() + (f2 + a2) * d2p.imag()
+neg_re_sum = (f0n + a0n) * s0n.real()
+neg_im_sum = (f0n + a0n) * s0n.imag()
+
+mod = rt.Model(pos_re_sum.norm_sqr() + pos_im_sum.norm_sqr() + neg_re_sum.norm_sqr() + neg_im_sum.norm_sqr())
+
+# There is no need to constrain amplitudes, since each named amplitude is only ever evaluated once and a cached value gets pulled if we run across an amplitude by the same name!
+# We should, however, fix some of the values to make the fit less ambiguous. For instance, suppose we are above the threshold for the f_0(500) which is included in the F0 K-Matrix:
+mod.fix("f0+", "f0_500 re", 0.0)
+mod.fix("f0+", "f0_500 im", 0.0)
+mod.fix("f0-", "f0_500 re", 0.0)
+mod.fix("f0-", "f0_500 im", 0.0)
+
+# As mentioned, we should also fix at least one complex phase per coherent sum:
+mod.fix("f0+", "f0_980 im", 0.0)
+mod.fix("f0-", "f0_980 im", 0.0)
+
+# All done! Now let's load our model into a Manager, which helps coordinate the model with datasets.
+# First, load up some datasets. rustitude provides an open operation that uses uproot under the hood:
 ds = rt.open('data.root')
 ds_mc = rt.open('mc.root')
 
-# Create a new "manager" to handle the interface between data and amplitudes
-m = rt.ExtendedLogLikelihood(ds, ds_mc)
+m_data = rt.Manager(mod, ds)
+m_mc = rt.Manager(mod, ds_mc)
+
+# We could stop here and evaluate just one dataset at a time:
+
+# res = m_data([1.0, 3.4, 2.8, -3.6, ... ])
+# -> [5.3, 0.2, ...], a list of intensities from the amplitude calculation
+
+# Or, what we probably want to do is find the negative log-likelihood for some choice of parameters:
 
-# Register some amplitudes
-# We provide a sum name, group name, and a named amplitude
-# This function also runs the precalculation method over the datasets
-m.register('pos re', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
-m.register('pos re', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
-m.register('pos re', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='+', part='real'))
-m.register('pos re', 'D', gluex.resonances.KMatrixF2('f2', channel=2))
-m.register('pos re', 'D', gluex.resonances.KMatrixA2('a2', channel=1))
-m.register('pos re', 'D', gluex.harmonics.Zlm('z22', 0, 0, reflectivity='+', part='real'))
-
-m.register('pos im', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
-m.register('pos im', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
-m.register('pos im', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='+', part='imag'))
-m.register('pos im', 'D', gluex.resonances.KMatrixF2('f2', channel=2))
-m.register('pos im', 'D', gluex.resonances.KMatrixA2('a2', channel=1))
-m.register('pos im', 'D', gluex.harmonics.Zlm('z22', 0, 0, reflectivity='+', part='imag'))
-
-# We can constrain all the free parameters of one amplitude to be equal to those of another,
-# provided they have the same free parameters. To constrain an individual amplitude, we can use
-# m.constrain(('pos re', 'S', 'f0', 'f0_500 re'), ('pos re', 'S', 'f0', 'f0_500 im')) for example,
-# which would make the real and imaginary part of equal to each other in the calculation.
-# This step reduces the number of free parameters in the calculation.
-m.constrain_amplitude(('pos re', 'S', 'f0'), ('pos im', 'S', 'f0'))
-m.constrain_amplitude(('pos re', 'S', 'a0'), ('pos im', 'S', 'a0'))
-m.constrain_amplitude(('pos re', 'D', 'f2'), ('pos im', 'D', 'f2'))
-m.constrain_amplitude(('pos re', 'D', 'a2'), ('pos im', 'D', 'a2'))
-
-# Fix some parameters to a given value (zero in this case)
-m.fix(('pos re', 'S', 'f0', 'f0_500 re'), 0.0)
-m.fix(('pos re', 'S', 'f0', 'f0_500 im'), 0.0)
-m.fix(('pos re', 'S', 'f0', 'f0_980 im'), 0.0)
-
-m.register('neg re', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
-m.register('neg re', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
-m.register('neg re', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='-', part='real'))
-
-m.register('neg im', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
-m.register('neg im', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
-m.register('neg im', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='-', part='imag'))
-
-m.constrain_amplitude(('neg re', 'S', 'f0'), ('neg im', 'S', 'f0'))
-m.constrain_amplitude(('neg re', 'S', 'a0'), ('neg im', 'S', 'a0'))
-
-m.fix(('neg re', 'S', 'f0', 'f0_500 re'), 0.0)
-m.fix(('neg re', 'S', 'f0', 'f0_500 im'), 0.0)
-m.fix(('neg re', 'S', 'f0', 'f0_980 im'), 0.0)
-
-# Calculate the negative log-likelihood given some random input parameters:
-rng = np.random.default_rng()
-nll = m(rng.random(len(m.parameters())) * 100.0)
+nll = rt.ExtendedLogLikelihood(m_data, m_mc)
+
+res = nll([10.0] * mod.get_n_free())
+print(res) # prints some value for the NLL
 ```
 
-See the [`rustitude-gluex`](https://github.com/denehoffman/rustitude-gluex) package for some of the currently implemented amplitudes (derived from GlueX's [halld_sim](https://github.com/JeffersonLab/halld_sim) repo). There are also some helper methods `scalar`, `cscalar`, and `pcscalar` to create amplitudes which represent a single free parameter, a single complex free parameter, and a single complex free parameter in polar coordinates respectively.
+See the [`rustitude-gluex`](https://github.com/denehoffman/rustitude/tree/main/crates/rustitude-gluex) package for some of the currently implemented amplitudes (derived from GlueX's [halld_sim](https://github.com/JeffersonLab/halld_sim) repo). There are also some helper methods `Scalar`, `CScalar`, and `PCScalar` to create amplitudes which represent a single free parameter, a single complex free parameter, and a single complex free parameter in polar coordinates respectively.
 
 # TODOs
+
 In no particular order, here is a list of what (probably) needs to be done before I will stop making any breaking changes:
+
 - Pure Rust parsing of ROOT files without the `uproot` backend (I have some moderate success with `oxyroot`, but there are still a few issues reading larger files)
 - Add plotting methods
 - A way to check if the number of parameters matches the input at compile time would be nice, not sure if it's possible though
 - Give managers a way to apply amplitudes to new datasets, like using the result from a fit to weight some generated Monte-Carlo for plotting the result. This is possible to do through Python, but a convenience method is probably needed
 - Lots of documentation
 - Lots of tests
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: rustitude Version: 0.3.4 Classifier: Development
+Metadata-Version: 2.3 Name: rustitude Version: 0.4.0 Classifier: Development
 Status :: 4 - Beta Classifier: Programming Language :: Python Requires-Dist:
 uproot Requires-Dist: numpy License-File: LICENSE Summary: Python bindings for
 the Rustitude library Keywords: physics,math,rust Home-Page: https://
 github.com/denehoffman/rustitude/ Author: Nathaniel Dene Hoffman Author-email:
 dene@cmu.edu Maintainer-email: Nathaniel Dene Hoffman
 cmu.edu> License: BSD-3-Clause Requires-Python: >=3.7 Description-Content-Type:
 text/markdown; charset=UTF-8; variant=GFM Project-URL: homepage, https://
@@ -86,69 +86,59 @@
 for any event $e$ and list of parameters $\overrightarrow{p}$ will then be:
 ```math I(\overrightarrow{p}, e) = \sum_{\text{groups} \in \text
 {sums}}\left|\sum_{\text{amplitudes} \in \text{groups}} \prod_{\text{amp} \in
 \text{amplitudes}} \text{amp}(\overrightarrow{p}, e)\right|^2 ``` #
 Installation Adding `rustitude` to an existing Rust project is as simple as
 ```shell cargo add rustitude ``` The Python installation is equally
 straightforward: ```shell pip install rustitude ``` # Usage See the
-[`rustitude-core`](https://github.com/denehoffman/rustitude-core) crate for a
-more in-depth tutorial on writing custom amplitudes in Rust. This package is
-mostly focused on the Python side of things. Here is the setup for an example
-analysis: ```python import rustitude as rt from rustitude import gluex import
-numpy as np # Load data files # This uses uproot under the hood ds = rt.open
-('data.root') ds_mc = rt.open('mc.root') # Create a new "manager" to handle the
-interface between data and amplitudes m = rt.ExtendedLogLikelihood(ds, ds_mc) #
-Register some amplitudes # We provide a sum name, group name, and a named
-amplitude # This function also runs the precalculation method over the datasets
-m.register('pos re', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
-m.register('pos re', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
-m.register('pos re', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='+',
-part='real')) m.register('pos re', 'D', gluex.resonances.KMatrixF2('f2',
-channel=2)) m.register('pos re', 'D', gluex.resonances.KMatrixA2('a2',
-channel=1)) m.register('pos re', 'D', gluex.harmonics.Zlm('z22', 0, 0,
-reflectivity='+', part='real')) m.register('pos im', 'S',
-gluex.resonances.KMatrixF0('f0', channel=2)) m.register('pos im', 'S',
-gluex.resonances.KMatrixA0('a0', channel=1)) m.register('pos im', 'S',
-gluex.harmonics.Zlm('z00', 0, 0, reflectivity='+', part='imag')) m.register
-('pos im', 'D', gluex.resonances.KMatrixF2('f2', channel=2)) m.register('pos
-im', 'D', gluex.resonances.KMatrixA2('a2', channel=1)) m.register('pos im',
-'D', gluex.harmonics.Zlm('z22', 0, 0, reflectivity='+', part='imag')) # We can
-constrain all the free parameters of one amplitude to be equal to those of
-another, # provided they have the same free parameters. To constrain an
-individual amplitude, we can use # m.constrain(('pos re', 'S', 'f0', 'f0_500
-re'), ('pos re', 'S', 'f0', 'f0_500 im')) for example, # which would make the
-real and imaginary part of equal to each other in the calculation. # This step
-reduces the number of free parameters in the calculation. m.constrain_amplitude
-(('pos re', 'S', 'f0'), ('pos im', 'S', 'f0')) m.constrain_amplitude(('pos re',
-'S', 'a0'), ('pos im', 'S', 'a0')) m.constrain_amplitude(('pos re', 'D', 'f2'),
-('pos im', 'D', 'f2')) m.constrain_amplitude(('pos re', 'D', 'a2'), ('pos im',
-'D', 'a2')) # Fix some parameters to a given value (zero in this case) m.fix(
-('pos re', 'S', 'f0', 'f0_500 re'), 0.0) m.fix(('pos re', 'S', 'f0', 'f0_500
-im'), 0.0) m.fix(('pos re', 'S', 'f0', 'f0_980 im'), 0.0) m.register('neg re',
-'S', gluex.resonances.KMatrixF0('f0', channel=2)) m.register('neg re', 'S',
-gluex.resonances.KMatrixA0('a0', channel=1)) m.register('neg re', 'S',
-gluex.harmonics.Zlm('z00', 0, 0, reflectivity='-', part='real')) m.register
-('neg im', 'S', gluex.resonances.KMatrixF0('f0', channel=2)) m.register('neg
-im', 'S', gluex.resonances.KMatrixA0('a0', channel=1)) m.register('neg im',
-'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='-', part='imag'))
-m.constrain_amplitude(('neg re', 'S', 'f0'), ('neg im', 'S', 'f0'))
-m.constrain_amplitude(('neg re', 'S', 'a0'), ('neg im', 'S', 'a0')) m.fix(('neg
-re', 'S', 'f0', 'f0_500 re'), 0.0) m.fix(('neg re', 'S', 'f0', 'f0_500 im'),
-0.0) m.fix(('neg re', 'S', 'f0', 'f0_980 im'), 0.0) # Calculate the negative
-log-likelihood given some random input parameters: rng = np.random.default_rng
-() nll = m(rng.random(len(m.parameters())) * 100.0) ``` See the [`rustitude-
-gluex`](https://github.com/denehoffman/rustitude-gluex) package for some of the
-currently implemented amplitudes (derived from GlueX's [halld_sim](https://
-github.com/JeffersonLab/halld_sim) repo). There are also some helper methods
-`scalar`, `cscalar`, and `pcscalar` to create amplitudes which represent a
-single free parameter, a single complex free parameter, and a single complex
-free parameter in polar coordinates respectively. # TODOs In no particular
-order, here is a list of what (probably) needs to be done before I will stop
-making any breaking changes: - Pure Rust parsing of ROOT files without the
-`uproot` backend (I have some moderate success with `oxyroot`, but there are
-still a few issues reading larger files) - Add plotting methods - A way to
-check if the number of parameters matches the input at compile time would be
-nice, not sure if it's possible though - Give managers a way to apply
-amplitudes to new datasets, like using the result from a fit to weight some
-generated Monte-Carlo for plotting the result. This is possible to do through
-Python, but a convenience method is probably needed - Lots of documentation -
-Lots of tests
+[`rustitude-core`](https://github.com/denehoffman/rustitude/tree/main/crates/
+rustitude-core) crate for a more in-depth tutorial on writing custom amplitudes
+in Rust. This package is mostly focused on the Python side of things. Here is
+the setup for an example analysis: ```python import rustitude as rt from
+rustitude import gluex import numpy as np # Start by creating some amplitudes:
+f0p = gluex.resonances.KMatrixF0('f0+', channel=2) f0n =
+gluex.resonances.KMatrixF0('f0-', channel=2) f2 = gluex.resonances.KMatrixF2
+('f2', channel=2) a0p = gluex.resonances.KMatrixA0('a0+', channel=1) a0n =
+gluex.resonances.KMatrixA0('a0-', channel=1) a2 = gluex.resonances.KMatrixA2
+('a2', channel=1) s0p = gluex.harmonics.Zlm('Z00+', 0, 0, reflectivity='+') s0n
+= gluex.harmonics.Zlm('Z00-', 0, 0, reflectivity='-') d2p = gluex.harmonics.Zlm
+('Z22+', 2, 2, reflectivity='+') # Next, let's put them together into a model #
+The API supports addition, and multiplication and has additional methods for
+the absolute-square (`norm_sqr`), real part (`real`) and imaginary part
+(`imag`). pos_re_sum = (f0p + a0p) * s0p.real() + (f2 + a2) * d2p.real()
+pos_im_sum = (f0p + a0p) * s0p.imag() + (f2 + a2) * d2p.imag() neg_re_sum =
+(f0n + a0n) * s0n.real() neg_im_sum = (f0n + a0n) * s0n.imag() mod = rt.Model
+(pos_re_sum.norm_sqr() + pos_im_sum.norm_sqr() + neg_re_sum.norm_sqr() +
+neg_im_sum.norm_sqr()) # There is no need to constrain amplitudes, since each
+named amplitude is only ever evaluated once and a cached value gets pulled if
+we run across an amplitude by the same name! # We should, however, fix some of
+the values to make the fit less ambiguous. For instance, suppose we are above
+the threshold for the f_0(500) which is included in the F0 K-Matrix: mod.fix
+("f0+", "f0_500 re", 0.0) mod.fix("f0+", "f0_500 im", 0.0) mod.fix("f0-",
+"f0_500 re", 0.0) mod.fix("f0-", "f0_500 im", 0.0) # As mentioned, we should
+also fix at least one complex phase per coherent sum: mod.fix("f0+", "f0_980
+im", 0.0) mod.fix("f0-", "f0_980 im", 0.0) # All done! Now let's load our model
+into a Manager, which helps coordinate the model with datasets. # First, load
+up some datasets. rustitude provides an open operation that uses uproot under
+the hood: ds = rt.open('data.root') ds_mc = rt.open('mc.root') m_data =
+rt.Manager(mod, ds) m_mc = rt.Manager(mod, ds_mc) # We could stop here and
+evaluate just one dataset at a time: # res = m_data([1.0, 3.4, 2.8, -3.6, ...
+]) # -> [5.3, 0.2, ...], a list of intensities from the amplitude calculation #
+Or, what we probably want to do is find the negative log-likelihood for some
+choice of parameters: nll = rt.ExtendedLogLikelihood(m_data, m_mc) res = nll(
+[10.0] * mod.get_n_free()) print(res) # prints some value for the NLL ``` See
+the [`rustitude-gluex`](https://github.com/denehoffman/rustitude/tree/main/
+crates/rustitude-gluex) package for some of the currently implemented
+amplitudes (derived from GlueX's [halld_sim](https://github.com/JeffersonLab/
+halld_sim) repo). There are also some helper methods `Scalar`, `CScalar`, and
+`PCScalar` to create amplitudes which represent a single free parameter, a
+single complex free parameter, and a single complex free parameter in polar
+coordinates respectively. # TODOs In no particular order, here is a list of
+what (probably) needs to be done before I will stop making any breaking
+changes: - Pure Rust parsing of ROOT files without the `uproot` backend (I have
+some moderate success with `oxyroot`, but there are still a few issues reading
+larger files) - Add plotting methods - A way to check if the number of
+parameters matches the input at compile time would be nice, not sure if it's
+possible though - Give managers a way to apply amplitudes to new datasets, like
+using the result from a fit to weight some generated Monte-Carlo for plotting
+the result. This is possible to do through Python, but a convenience method is
+probably needed - Lots of documentation - Lots of tests
```

