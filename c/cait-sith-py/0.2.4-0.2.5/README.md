# Comparing `tmp/cait_sith_py-0.2.4.tar.gz` & `tmp/cait_sith_py-0.2.5.tar.gz`

## Comparing `cait_sith_py-0.2.4.tar` & `cait_sith_py-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 cait_sith_py-0.2.4/Cargo.toml
--rw-r--r--   0     1001      127     2650 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     1890 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/.gitignore
--rw-r--r--   0     1001      127    11357 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/LICENSE
--rw-r--r--   0     1001      127     1572 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/action.rs
--rw-r--r--   0     1001      127     1995 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/arithmetic.rs
--rw-r--r--   0     1001      127     3158 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/keyshare.rs
--rw-r--r--   0     1001      127     1698 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/lib.rs
--rw-r--r--   0     1001      127     1579 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/participant.rs
--rw-r--r--   0     1001      127     4118 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/presign.rs
--rw-r--r--   0     1001      127     1728 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/protocol.rs
--rw-r--r--   0     1001      127     4020 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/sign.rs
--rw-r--r--   0     1001      127     4598 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/triples.rs
--rw-r--r--   0     1001      127    35142 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/Cargo.lock
--rw-r--r--   0     1001      127      923 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 cait_sith_py-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 cait_sith_py-0.2.5/Cargo.toml
+-rw-r--r--   0     1001      127     2650 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     1890 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/.gitignore
+-rw-r--r--   0     1001      127    11357 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/LICENSE
+-rw-r--r--   0     1001      127     1572 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/src/action.rs
+-rw-r--r--   0     1001      127     1995 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/src/arithmetic.rs
+-rw-r--r--   0     1001      127     3158 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/src/keyshare.rs
+-rw-r--r--   0     1001      127     1698 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/src/lib.rs
+-rw-r--r--   0     1001      127     1579 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/src/participant.rs
+-rw-r--r--   0     1001      127     4375 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/src/presign.rs
+-rw-r--r--   0     1001      127     1728 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/src/protocol.rs
+-rw-r--r--   0     1001      127     4020 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/src/sign.rs
+-rw-r--r--   0     1001      127     4598 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/src/triples.rs
+-rw-r--r--   0     1001      127    35142 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/Cargo.lock
+-rw-r--r--   0     1001      127      923 2024-05-15 21:38:25.000000 cait_sith_py-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 cait_sith_py-0.2.5/PKG-INFO
```

### Comparing `cait_sith_py-0.2.4/.github/workflows/CI.yml` & `cait_sith_py-0.2.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.4/.gitignore` & `cait_sith_py-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.4/LICENSE` & `cait_sith_py-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.4/src/action.rs` & `cait_sith_py-0.2.5/src/action.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.4/src/arithmetic.rs` & `cait_sith_py-0.2.5/src/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.4/src/keyshare.rs` & `cait_sith_py-0.2.5/src/keyshare.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.4/src/lib.rs` & `cait_sith_py-0.2.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.4/src/participant.rs` & `cait_sith_py-0.2.5/src/participant.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.4/src/presign.rs` & `cait_sith_py-0.2.5/src/presign.rs`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 use cait_sith::protocol::Participant;
 use cait_sith::{
     protocol::Action, protocol::MessageData, protocol::Protocol, PresignArguments, PresignOutput,
 };
 
 use k256::Secp256k1;
 use pyo3::{pyclass, pyfunction, pymethods, PyErr, PyResult};
+use serde::{Deserialize, Serialize};
 
 use crate::{participant::convert_participants, participant::PyParticipant};
 
 use crate::keyshare::{derive_epsilon, PyKeygenOutput};
 use crate::triples::PyTripleGenerationOutput;
 
 /// The arguments needed to create a presignature.
@@ -58,15 +59,15 @@
 }
 
 /// The output of the presigning protocol.
 ///
 /// This output is basically all the parts of the signature that we can perform
 /// without knowing the message.
 #[pyclass(name = "PresignOutput")]
-#[derive(Debug, Clone)]
+#[derive(Debug, Clone, Serialize, Deserialize)]
 pub struct PyPresignOutput {
     /// The public nonce commitment.
     #[pyo3(get)]
     pub big_r: String,
     /// Our share of the nonce value.
     #[pyo3(get)]
     pub k: String,
@@ -105,16 +106,26 @@
             big_r: view.big_r,
             k: view.k,
             sigma: view.sigma + epsilon * view.k,
         };
 
         derived_presign.into()
     }
+
+    fn to_json(&self) -> String {
+        serde_json::to_string(&self).unwrap()
+    }
+
+    #[new]
+    fn new(json_data: String) -> Self {
+        serde_json::from_str(&json_data).unwrap()
+    }
 }
 
+
 create_action_enum!(
     PresignGenerationAction,
     PresignOutput<Secp256k1>,
     PyPresignOutput
 );
 
 create_protocol!(
```

### Comparing `cait_sith_py-0.2.4/src/protocol.rs` & `cait_sith_py-0.2.5/src/protocol.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.4/src/sign.rs` & `cait_sith_py-0.2.5/src/sign.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.4/src/triples.rs` & `cait_sith_py-0.2.5/src/triples.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.4/Cargo.lock` & `cait_sith_py-0.2.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
  "serde",
  "smol",
  "subtle",
 ]
 
 [[package]]
 name = "cait-sith-py"
-version = "0.2.4"
+version = "0.2.5"
 dependencies = [
  "cait-sith",
  "k256",
  "pyo3",
  "serde",
  "serde_json",
 ]
```

### Comparing `cait_sith_py-0.2.4/pyproject.toml` & `cait_sith_py-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cait_sith_py"
-version = "0.2.4"
+version = "0.2.5"
 description = "Cait Sith rust wrapper on python"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 maturin = "0.14.3"
@@ -19,15 +19,15 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 
 [project]
 name = "cait_sith_py"
-version = "0.2.4"
+version = "0.2.5"
 description = "Cait Sith rust wrapper on python"
 license = {file = "LICENSE"} # relative to the package/ directory
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
```

