# Comparing `tmp/fleece_network-0.4.1.tar.gz` & `tmp/fleece_network-0.4.2.tar.gz`

## Comparing `fleece_network-0.4.1.tar` & `fleece_network-0.4.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0     1000     1000     1045 2024-05-15 09:06:31.000000 fleece_network-0.4.1/fleece-network/Cargo.toml
--rw-r--r--   0     1000     1000   117062 2024-05-15 09:06:32.000000 fleece_network-0.4.1/fleece-network/Cargo.lock
--rw-r--r--   0     1000     1000      668 2024-05-08 04:34:11.000000 fleece_network-0.4.1/fleece-network/src/bin/center.rs
--rw-r--r--   0     1000     1000     2337 2024-05-15 13:39:02.000000 fleece_network-0.4.1/fleece-network/src/bin/peer.rs
--rw-r--r--   0     1000     1000     3440 2024-05-14 04:23:22.000000 fleece_network-0.4.1/fleece-network/src/center/mod.rs
--rw-r--r--   0     1000     1000     9715 2024-05-15 13:21:47.000000 fleece_network-0.4.1/fleece-network/src/channel/behaviour.rs
--rw-r--r--   0     1000     1000     4075 2024-05-15 09:06:31.000000 fleece_network-0.4.1/fleece-network/src/channel/codec.rs
--rw-r--r--   0     1000     1000    16555 2024-05-15 13:51:26.000000 fleece_network-0.4.1/fleece-network/src/channel/handler.rs
--rw-r--r--   0     1000     1000     5149 2024-05-15 12:54:22.000000 fleece_network-0.4.1/fleece-network/src/channel/message.rs
--rw-r--r--   0     1000     1000      365 2024-05-15 13:52:39.000000 fleece_network-0.4.1/fleece-network/src/channel/mod.rs
--rw-r--r--   0     1000     1000      438 2024-05-08 04:34:11.000000 fleece_network-0.4.1/fleece-network/src/error.rs
--rw-r--r--   0     1000     1000      112 2024-05-15 13:52:49.000000 fleece_network-0.4.1/fleece-network/src/lib.rs
--rw-r--r--   0     1000     1000     1821 2024-05-15 12:54:22.000000 fleece_network-0.4.1/fleece-network/src/peer/behaviour.rs
--rw-r--r--   0     1000     1000     5214 2024-05-15 08:21:07.000000 fleece_network-0.4.1/fleece-network/src/peer/codec.rs
--rw-r--r--   0     1000     1000     3147 2024-05-14 02:45:36.000000 fleece_network-0.4.1/fleece-network/src/peer/codec_legacy.rs
--rw-r--r--   0     1000     1000    10466 2024-05-15 13:52:29.000000 fleece_network-0.4.1/fleece-network/src/peer/eventloop.rs
--rw-r--r--   0     1000     1000     1099 2024-05-08 04:34:11.000000 fleece_network-0.4.1/fleece-network/src/peer/handler.rs
--rw-r--r--   0     1000     1000      121 2024-05-10 06:59:55.000000 fleece_network-0.4.1/fleece-network/src/peer/mod.rs
--rw-r--r--   0     1000     1000     3092 2024-05-15 12:54:22.000000 fleece_network-0.4.1/fleece-network/src/peer/peer.rs
--rw-r--r--   0     1000     1000     2368 2024-05-15 12:54:22.000000 fleece_network-0.4.1/fleece-network/src/peer/proxy.rs
--rw-r--r--   0     1000     1000     1751 2024-05-12 15:31:08.000000 fleece_network-0.4.1/fleece-network/src/router.rs
--rw-r--r--   0     1000     1000     3915 2024-05-12 15:30:41.000000 fleece_network-0.4.1/fleece-network/src/transport.rs
--rw-r--r--   0     1000     1000     2159 2024-05-14 11:01:37.000000 fleece_network-0.4.1/fleece-network/src/utils/chunk.rs
--rw-r--r--   0     1000     1000       15 2024-05-15 13:52:53.000000 fleece_network-0.4.1/fleece-network/src/utils/mod.rs
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 fleece_network-0.4.1/python/Cargo.toml
--rw-r--r--   0     1000     1000       25 2024-05-14 08:51:32.000000 fleece_network-0.4.1/python/.gitignore
--rw-r--r--   0     1000     1000      570 2024-05-15 13:17:16.000000 fleece_network-0.4.1/python/example.py
--rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 fleece_network-0.4.1/python/pysrc/fleece_network/__init__.py
--rw-r--r--   0     1000     1000     1788 2024-05-15 13:16:11.000000 fleece_network-0.4.1/python/pysrc/fleece_network/peer.py
--rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 fleece_network-0.4.1/python/pysrc/fleece_network/py.typed
--rw-r--r--   0     1000     1000      640 2024-05-15 06:51:33.000000 fleece_network-0.4.1/python/pysrc/fleece_network/serde.py
--rw-r--r--   0     1000     1000       15 2024-05-08 04:34:11.000000 fleece_network-0.4.1/python/src/lib.rs
--rw-r--r--   0     1000     1000     6034 2024-05-15 13:09:37.000000 fleece_network-0.4.1/python/src/proxy.rs
--rw-r--r--   0     1000     1000   120623 2024-05-15 13:55:59.000000 fleece_network-0.4.1/python/Cargo.lock
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 fleece_network-0.4.1/pyproject.toml
--rw-r--r--   0     1000     1000     1788 2024-05-15 13:16:11.000000 fleece_network-0.4.1/pysrc/fleece_network/peer.py
--rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 fleece_network-0.4.1/pysrc/fleece_network/__init__.py
--rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 fleece_network-0.4.1/pysrc/fleece_network/py.typed
--rw-r--r--   0     1000     1000      640 2024-05-15 06:51:33.000000 fleece_network-0.4.1/pysrc/fleece_network/serde.py
--rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 fleece_network-0.4.1/PKG-INFO
+-rw-r--r--   0     1000     1000     1045 2024-05-15 09:06:31.000000 fleece_network-0.4.2/fleece-network/Cargo.toml
+-rw-r--r--   0     1000     1000   117062 2024-05-15 09:06:32.000000 fleece_network-0.4.2/fleece-network/Cargo.lock
+-rw-r--r--   0     1000     1000      668 2024-05-08 04:34:11.000000 fleece_network-0.4.2/fleece-network/src/bin/center.rs
+-rw-r--r--   0     1000     1000     2337 2024-05-15 13:39:02.000000 fleece_network-0.4.2/fleece-network/src/bin/peer.rs
+-rw-r--r--   0     1000     1000     3440 2024-05-14 04:23:22.000000 fleece_network-0.4.2/fleece-network/src/center/mod.rs
+-rw-r--r--   0     1000     1000     9715 2024-05-15 13:21:47.000000 fleece_network-0.4.2/fleece-network/src/channel/behaviour.rs
+-rw-r--r--   0     1000     1000     4075 2024-05-15 09:06:31.000000 fleece_network-0.4.2/fleece-network/src/channel/codec.rs
+-rw-r--r--   0     1000     1000    16555 2024-05-15 13:51:26.000000 fleece_network-0.4.2/fleece-network/src/channel/handler.rs
+-rw-r--r--   0     1000     1000     5149 2024-05-15 12:54:22.000000 fleece_network-0.4.2/fleece-network/src/channel/message.rs
+-rw-r--r--   0     1000     1000      365 2024-05-15 13:52:39.000000 fleece_network-0.4.2/fleece-network/src/channel/mod.rs
+-rw-r--r--   0     1000     1000      438 2024-05-08 04:34:11.000000 fleece_network-0.4.2/fleece-network/src/error.rs
+-rw-r--r--   0     1000     1000      112 2024-05-15 13:52:49.000000 fleece_network-0.4.2/fleece-network/src/lib.rs
+-rw-r--r--   0     1000     1000     1822 2024-05-15 14:52:12.000000 fleece_network-0.4.2/fleece-network/src/peer/behaviour.rs
+-rw-r--r--   0     1000     1000     5214 2024-05-15 08:21:07.000000 fleece_network-0.4.2/fleece-network/src/peer/codec.rs
+-rw-r--r--   0     1000     1000     3147 2024-05-14 02:45:36.000000 fleece_network-0.4.2/fleece-network/src/peer/codec_legacy.rs
+-rw-r--r--   0     1000     1000    10466 2024-05-15 13:52:29.000000 fleece_network-0.4.2/fleece-network/src/peer/eventloop.rs
+-rw-r--r--   0     1000     1000     1099 2024-05-08 04:34:11.000000 fleece_network-0.4.2/fleece-network/src/peer/handler.rs
+-rw-r--r--   0     1000     1000      121 2024-05-10 06:59:55.000000 fleece_network-0.4.2/fleece-network/src/peer/mod.rs
+-rw-r--r--   0     1000     1000     3093 2024-05-15 14:52:33.000000 fleece_network-0.4.2/fleece-network/src/peer/peer.rs
+-rw-r--r--   0     1000     1000     2369 2024-05-15 14:52:27.000000 fleece_network-0.4.2/fleece-network/src/peer/proxy.rs
+-rw-r--r--   0     1000     1000     1751 2024-05-12 15:31:08.000000 fleece_network-0.4.2/fleece-network/src/router.rs
+-rw-r--r--   0     1000     1000     3915 2024-05-12 15:30:41.000000 fleece_network-0.4.2/fleece-network/src/transport.rs
+-rw-r--r--   0     1000     1000     2159 2024-05-14 11:01:37.000000 fleece_network-0.4.2/fleece-network/src/utils/chunk.rs
+-rw-r--r--   0     1000     1000       15 2024-05-15 13:52:53.000000 fleece_network-0.4.2/fleece-network/src/utils/mod.rs
+-rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 fleece_network-0.4.2/python/Cargo.toml
+-rw-r--r--   0     1000     1000       25 2024-05-14 08:51:32.000000 fleece_network-0.4.2/python/.gitignore
+-rw-r--r--   0     1000     1000      570 2024-05-15 13:17:16.000000 fleece_network-0.4.2/python/example.py
+-rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 fleece_network-0.4.2/python/pysrc/fleece_network/__init__.py
+-rw-r--r--   0     1000     1000     1788 2024-05-15 13:16:11.000000 fleece_network-0.4.2/python/pysrc/fleece_network/peer.py
+-rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 fleece_network-0.4.2/python/pysrc/fleece_network/py.typed
+-rw-r--r--   0     1000     1000      640 2024-05-15 06:51:33.000000 fleece_network-0.4.2/python/pysrc/fleece_network/serde.py
+-rw-r--r--   0     1000     1000       15 2024-05-08 04:34:11.000000 fleece_network-0.4.2/python/src/lib.rs
+-rw-r--r--   0     1000     1000     6217 2024-05-15 14:54:26.000000 fleece_network-0.4.2/python/src/proxy.rs
+-rw-r--r--   0     1000     1000   120623 2024-05-15 14:52:56.000000 fleece_network-0.4.2/python/Cargo.lock
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 fleece_network-0.4.2/pyproject.toml
+-rw-r--r--   0     1000     1000     1788 2024-05-15 13:16:11.000000 fleece_network-0.4.2/pysrc/fleece_network/peer.py
+-rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 fleece_network-0.4.2/pysrc/fleece_network/__init__.py
+-rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 fleece_network-0.4.2/pysrc/fleece_network/py.typed
+-rw-r--r--   0     1000     1000      640 2024-05-15 06:51:33.000000 fleece_network-0.4.2/pysrc/fleece_network/serde.py
+-rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 fleece_network-0.4.2/PKG-INFO
```

### Comparing `fleece_network-0.4.1/fleece-network/Cargo.toml` & `fleece_network-0.4.2/fleece-network/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/Cargo.lock` & `fleece_network-0.4.2/fleece-network/Cargo.lock`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/bin/center.rs` & `fleece_network-0.4.2/fleece-network/src/bin/center.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/bin/peer.rs` & `fleece_network-0.4.2/fleece-network/src/bin/peer.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/center/mod.rs` & `fleece_network-0.4.2/fleece-network/src/center/mod.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/channel/behaviour.rs` & `fleece_network-0.4.2/fleece-network/src/channel/behaviour.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/channel/codec.rs` & `fleece_network-0.4.2/fleece-network/src/channel/codec.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/channel/handler.rs` & `fleece_network-0.4.2/fleece-network/src/channel/handler.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/channel/message.rs` & `fleece_network-0.4.2/fleece-network/src/channel/message.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/peer/behaviour.rs` & `fleece_network-0.4.2/fleece-network/src/peer/behaviour.rs`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         keypair: &Keypair,
         relay_behaviour: relay::client::Behaviour,
     ) -> (
         Self,
         mpsc::Receiver<InboundHandle<codec::Request, codec::Response>>,
     ) {
         let codec = codec::Codec::default();
-        let (sender, receiver) = mpsc::channel(16);
+        let (sender, receiver) = mpsc::channel(128);
         (
             Self {
                 identify: identify::Behaviour::new(identify::Config::new(
                     "/TODO/1.0.0".to_string(),
                     keypair.public(),
                 )),
                 rendezvous: rendezvous::client::Behaviour::new(keypair.clone()),
```

### Comparing `fleece_network-0.4.1/fleece-network/src/peer/codec.rs` & `fleece_network-0.4.2/fleece-network/src/peer/codec.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/peer/codec_legacy.rs` & `fleece_network-0.4.2/fleece-network/src/peer/codec_legacy.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/peer/eventloop.rs` & `fleece_network-0.4.2/fleece-network/src/peer/eventloop.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/peer/handler.rs` & `fleece_network-0.4.2/fleece-network/src/peer/handler.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/peer/peer.rs` & `fleece_network-0.4.2/fleece-network/src/peer/peer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         let mut swarm = Swarm::new(transport, behaviour, peer_id.clone(), swarm_config);
 
         // setup for direct connection
         swarm.listen_on(self_addr.clone()).unwrap();
 
         // setup for stream
 
-        let (command_tx, command_rx) = mpsc::channel(32);
+        let (command_tx, command_rx) = mpsc::channel(128);
         let eventloop = EventLoop::new(
             swarm,
             command_tx.clone(),
             command_rx,
             center_addr.clone(),
             center_peer_id.clone(),
         );
```

### Comparing `fleece_network-0.4.1/fleece-network/src/peer/proxy.rs` & `fleece_network-0.4.2/fleece-network/src/peer/proxy.rs`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             .with(Protocol::P2pCircuit)
             .with(Protocol::P2p(peer_id));
         swarm.listen_on(relay_addr.clone()).unwrap();
         swarm.add_external_address(relay_addr.clone());
 
         // setup for stream
 
-        let (command_tx, command_rx) = mpsc::channel(32);
+        let (command_tx, command_rx) = mpsc::channel(128);
         let eventloop = EventLoop::new(
             swarm,
             command_tx.clone(),
             command_rx,
             center_addr.clone(),
             center_peer_id.clone(),
         );
```

### Comparing `fleece_network-0.4.1/fleece-network/src/router.rs` & `fleece_network-0.4.2/fleece-network/src/router.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/transport.rs` & `fleece_network-0.4.2/fleece-network/src/transport.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/fleece-network/src/utils/chunk.rs` & `fleece_network-0.4.2/fleece-network/src/utils/chunk.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/python/Cargo.toml` & `fleece_network-0.4.2/python/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "fleece-network-python"
-version = "0.4.1"
+version = "0.4.2"
 edition = "2021"
 
 [lib]
 name = "fleece_network_rust"
 crate-type = ["cdylib"]
 
 [dependencies]
```

### Comparing `fleece_network-0.4.1/python/example.py` & `fleece_network-0.4.2/python/example.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/python/pysrc/fleece_network/peer.py` & `fleece_network-0.4.2/python/pysrc/fleece_network/peer.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/python/pysrc/fleece_network/serde.py` & `fleece_network-0.4.2/python/pysrc/fleece_network/serde.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/python/src/proxy.rs` & `fleece_network-0.4.2/python/src/proxy.rs`

 * *Files 3% similar despite different names*

```diff
@@ -96,24 +96,33 @@
             .try_init();
     }
 
     fn peer_id(this: PyRef<'_, Self>) -> String {
         this.peer_id.to_string()
     }
 
-    fn send(this: PyRefMut<'_, Self>, peer_id: String, request: PyCodecRequest) -> PyCodecResponse {
+    fn send(
+        this: PyRefMut<'_, Self>,
+        peer_id: String,
+        request: PyCodecRequest,
+        py: Python<'_>,
+    ) -> PyCodecResponse {
         let (tx, rx) = oneshot::channel();
-        this.command_tx
-            .blocking_send(Command::Request {
-                peer_id: peer_id.parse().unwrap(),
-                request: request.into(),
-                sender: tx,
-            })
-            .unwrap();
-        rx.blocking_recv().unwrap().unwrap().into()
+        let command_tx = this.command_tx.clone();
+        Python::allow_threads(py, || {
+            command_tx
+                .blocking_send(Command::Request {
+                    peer_id: peer_id.parse().unwrap(),
+                    request: request.into(),
+                    sender: tx,
+                })
+                .unwrap();
+
+            rx.blocking_recv().unwrap().unwrap().into()
+        })
     }
 
     fn recv(this: Py<Self>, py: Python<'_>) -> Option<(PyCodecRequest, PyCallback)> {
         let mut request_rx = this.borrow_mut(py).request_rx.take().unwrap();
         let (request_rx, result) =
             Python::allow_threads(py, move || match request_rx.blocking_recv() {
                 Some(handle) => {
```

### Comparing `fleece_network-0.4.1/python/Cargo.lock` & `fleece_network-0.4.2/python/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1226,15 +1226,15 @@
  "tracing-flame",
  "tracing-subscriber",
  "void",
 ]
 
 [[package]]
 name = "fleece-network-python"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
  "bytes",
  "chrono",
  "crossbeam-channel",
  "dyn-clone",
  "fleece-network",
  "futures",
```

### Comparing `fleece_network-0.4.1/pyproject.toml` & `fleece_network-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/pysrc/fleece_network/peer.py` & `fleece_network-0.4.2/pysrc/fleece_network/peer.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.1/pysrc/fleece_network/serde.py` & `fleece_network-0.4.2/pysrc/fleece_network/serde.py`

 * *Files identical despite different names*

