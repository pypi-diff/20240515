# Comparing `tmp/fleece_network-0.4.0.tar.gz` & `tmp/fleece_network-0.4.1.tar.gz`

## Comparing `fleece_network-0.4.0.tar` & `fleece_network-0.4.1.tar`

### file list

```diff
@@ -1,44 +1,40 @@
--rw-------   0     1000     1000     1045 2024-05-10 13:42:36.000000 fleece_network-0.4.0/fleece-network/Cargo.toml
--rw-r--r--   0     1000     1000   117062 2024-05-10 13:42:36.000000 fleece_network-0.4.0/fleece-network/Cargo.lock
--rw-r--r--   0     1000     1000      668 2024-05-08 04:34:11.000000 fleece_network-0.4.0/fleece-network/src/bin/center.rs
--rw-r--r--   0     1000     1000     2320 2024-05-13 14:19:20.000000 fleece_network-0.4.0/fleece-network/src/bin/peer.rs
--rw-r--r--   0     1000     1000     3440 2024-05-14 04:23:22.000000 fleece_network-0.4.0/fleece-network/src/center/mod.rs
--rw-r--r--   0     1000     1000    11063 2024-05-13 14:23:05.000000 fleece_network-0.4.0/fleece-network/src/channel/behaviour.rs
--rw-r--r--   0     1000     1000     4075 2024-05-13 14:08:57.000000 fleece_network-0.4.0/fleece-network/src/channel/codec.rs
--rw-r--r--   0     1000     1000    17288 2024-05-13 14:01:46.000000 fleece_network-0.4.0/fleece-network/src/channel/handler.rs
--rw-r--r--   0     1000     1000     7249 2024-05-08 05:51:30.000000 fleece_network-0.4.0/fleece-network/src/channel/legacy_stream.rs
--rw-r--r--   0     1000     1000     3477 2024-05-12 12:24:02.000000 fleece_network-0.4.0/fleece-network/src/channel/message.rs
--rw-r--r--   0     1000     1000      388 2024-05-11 04:18:09.000000 fleece_network-0.4.0/fleece-network/src/channel/mod.rs
--rw-r--r--   0     1000     1000      438 2024-05-08 04:34:11.000000 fleece_network-0.4.0/fleece-network/src/error.rs
--rw-r--r--   0     1000     1000      128 2024-05-12 07:53:54.000000 fleece_network-0.4.0/fleece-network/src/lib.rs
--rw-r--r--   0     1000     1000     1410 2024-05-12 15:29:27.000000 fleece_network-0.4.0/fleece-network/src/peer/behaviour.rs
--rw-r--r--   0     1000     1000     5214 2024-05-13 14:02:22.000000 fleece_network-0.4.0/fleece-network/src/peer/codec.rs
--rw-r--r--   0     1000     1000     3147 2024-05-14 02:45:36.000000 fleece_network-0.4.0/fleece-network/src/peer/codec_legacy.rs
--rw-r--r--   0     1000     1000    11513 2024-05-14 04:23:03.000000 fleece_network-0.4.0/fleece-network/src/peer/eventloop.rs
--rw-r--r--   0     1000     1000     1099 2024-05-08 04:34:11.000000 fleece_network-0.4.0/fleece-network/src/peer/handler.rs
--rw-r--r--   0     1000     1000      121 2024-05-10 06:59:55.000000 fleece_network-0.4.0/fleece-network/src/peer/mod.rs
--rw-r--r--   0     1000     1000     4160 2024-05-14 04:23:30.000000 fleece_network-0.4.0/fleece-network/src/peer/peer.rs
--rw-r--r--   0     1000     1000     3753 2024-05-12 14:52:11.000000 fleece_network-0.4.0/fleece-network/src/peer/proxy.rs
--rw-r--r--   0     1000     1000     1751 2024-05-12 15:31:08.000000 fleece_network-0.4.0/fleece-network/src/router.rs
--rw-r--r--   0     1000     1000     7249 2024-05-12 15:30:38.000000 fleece_network-0.4.0/fleece-network/src/stream.rs
--rw-r--r--   0     1000     1000     3915 2024-05-12 15:30:41.000000 fleece_network-0.4.0/fleece-network/src/transport.rs
--rw-r--r--   0     1000     1000     4293 2024-05-12 15:30:31.000000 fleece_network-0.4.0/fleece-network/src/utils/buflist.rs
--rw-r--r--   0     1000     1000     2159 2024-05-13 14:00:02.000000 fleece_network-0.4.0/fleece-network/src/utils/chunk.rs
--rw-r--r--   0     1000     1000       32 2024-05-12 15:30:32.000000 fleece_network-0.4.0/fleece-network/src/utils/mod.rs
--rw-r--r--   0     1000     1000     2650 2024-05-08 04:34:11.000000 fleece_network-0.4.0/fleece-network/src/utils-legacy.rs
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 fleece_network-0.4.0/python/Cargo.toml
--rw-r--r--   0     1000     1000       25 2024-05-14 05:31:54.000000 fleece_network-0.4.0/python/.gitignore
--rw-r--r--   0     1000     1000      528 2024-05-14 06:17:50.000000 fleece_network-0.4.0/python/example.py
--rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 fleece_network-0.4.0/python/pysrc/fleece_network/__init__.py
--rw-r--r--   0     1000     1000     1615 2024-05-14 05:32:36.000000 fleece_network-0.4.0/python/pysrc/fleece_network/peer.py
--rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 fleece_network-0.4.0/python/pysrc/fleece_network/py.typed
--rw-r--r--   0     1000     1000      620 2024-05-14 06:18:22.000000 fleece_network-0.4.0/python/pysrc/fleece_network/serde.py
--rw-r--r--   0     1000     1000       15 2024-05-08 04:34:11.000000 fleece_network-0.4.0/python/src/lib.rs
--rw-r--r--   0     1000     1000     5518 2024-05-14 05:21:02.000000 fleece_network-0.4.0/python/src/proxy.rs
--rw-r--r--   0     1000     1000   120600 2024-05-14 06:33:50.000000 fleece_network-0.4.0/python/Cargo.lock
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 fleece_network-0.4.0/pyproject.toml
--rw-r--r--   0     1000     1000     1615 2024-05-14 05:32:36.000000 fleece_network-0.4.0/pysrc/fleece_network/peer.py
--rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 fleece_network-0.4.0/pysrc/fleece_network/__init__.py
--rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 fleece_network-0.4.0/pysrc/fleece_network/py.typed
--rw-r--r--   0     1000     1000      620 2024-05-14 06:18:22.000000 fleece_network-0.4.0/pysrc/fleece_network/serde.py
--rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 fleece_network-0.4.0/PKG-INFO
+-rw-r--r--   0     1000     1000     1045 2024-05-15 09:06:31.000000 fleece_network-0.4.1/fleece-network/Cargo.toml
+-rw-r--r--   0     1000     1000   117062 2024-05-15 09:06:32.000000 fleece_network-0.4.1/fleece-network/Cargo.lock
+-rw-r--r--   0     1000     1000      668 2024-05-08 04:34:11.000000 fleece_network-0.4.1/fleece-network/src/bin/center.rs
+-rw-r--r--   0     1000     1000     2337 2024-05-15 13:39:02.000000 fleece_network-0.4.1/fleece-network/src/bin/peer.rs
+-rw-r--r--   0     1000     1000     3440 2024-05-14 04:23:22.000000 fleece_network-0.4.1/fleece-network/src/center/mod.rs
+-rw-r--r--   0     1000     1000     9715 2024-05-15 13:21:47.000000 fleece_network-0.4.1/fleece-network/src/channel/behaviour.rs
+-rw-r--r--   0     1000     1000     4075 2024-05-15 09:06:31.000000 fleece_network-0.4.1/fleece-network/src/channel/codec.rs
+-rw-r--r--   0     1000     1000    16555 2024-05-15 13:51:26.000000 fleece_network-0.4.1/fleece-network/src/channel/handler.rs
+-rw-r--r--   0     1000     1000     5149 2024-05-15 12:54:22.000000 fleece_network-0.4.1/fleece-network/src/channel/message.rs
+-rw-r--r--   0     1000     1000      365 2024-05-15 13:52:39.000000 fleece_network-0.4.1/fleece-network/src/channel/mod.rs
+-rw-r--r--   0     1000     1000      438 2024-05-08 04:34:11.000000 fleece_network-0.4.1/fleece-network/src/error.rs
+-rw-r--r--   0     1000     1000      112 2024-05-15 13:52:49.000000 fleece_network-0.4.1/fleece-network/src/lib.rs
+-rw-r--r--   0     1000     1000     1821 2024-05-15 12:54:22.000000 fleece_network-0.4.1/fleece-network/src/peer/behaviour.rs
+-rw-r--r--   0     1000     1000     5214 2024-05-15 08:21:07.000000 fleece_network-0.4.1/fleece-network/src/peer/codec.rs
+-rw-r--r--   0     1000     1000     3147 2024-05-14 02:45:36.000000 fleece_network-0.4.1/fleece-network/src/peer/codec_legacy.rs
+-rw-r--r--   0     1000     1000    10466 2024-05-15 13:52:29.000000 fleece_network-0.4.1/fleece-network/src/peer/eventloop.rs
+-rw-r--r--   0     1000     1000     1099 2024-05-08 04:34:11.000000 fleece_network-0.4.1/fleece-network/src/peer/handler.rs
+-rw-r--r--   0     1000     1000      121 2024-05-10 06:59:55.000000 fleece_network-0.4.1/fleece-network/src/peer/mod.rs
+-rw-r--r--   0     1000     1000     3092 2024-05-15 12:54:22.000000 fleece_network-0.4.1/fleece-network/src/peer/peer.rs
+-rw-r--r--   0     1000     1000     2368 2024-05-15 12:54:22.000000 fleece_network-0.4.1/fleece-network/src/peer/proxy.rs
+-rw-r--r--   0     1000     1000     1751 2024-05-12 15:31:08.000000 fleece_network-0.4.1/fleece-network/src/router.rs
+-rw-r--r--   0     1000     1000     3915 2024-05-12 15:30:41.000000 fleece_network-0.4.1/fleece-network/src/transport.rs
+-rw-r--r--   0     1000     1000     2159 2024-05-14 11:01:37.000000 fleece_network-0.4.1/fleece-network/src/utils/chunk.rs
+-rw-r--r--   0     1000     1000       15 2024-05-15 13:52:53.000000 fleece_network-0.4.1/fleece-network/src/utils/mod.rs
+-rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 fleece_network-0.4.1/python/Cargo.toml
+-rw-r--r--   0     1000     1000       25 2024-05-14 08:51:32.000000 fleece_network-0.4.1/python/.gitignore
+-rw-r--r--   0     1000     1000      570 2024-05-15 13:17:16.000000 fleece_network-0.4.1/python/example.py
+-rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 fleece_network-0.4.1/python/pysrc/fleece_network/__init__.py
+-rw-r--r--   0     1000     1000     1788 2024-05-15 13:16:11.000000 fleece_network-0.4.1/python/pysrc/fleece_network/peer.py
+-rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 fleece_network-0.4.1/python/pysrc/fleece_network/py.typed
+-rw-r--r--   0     1000     1000      640 2024-05-15 06:51:33.000000 fleece_network-0.4.1/python/pysrc/fleece_network/serde.py
+-rw-r--r--   0     1000     1000       15 2024-05-08 04:34:11.000000 fleece_network-0.4.1/python/src/lib.rs
+-rw-r--r--   0     1000     1000     6034 2024-05-15 13:09:37.000000 fleece_network-0.4.1/python/src/proxy.rs
+-rw-r--r--   0     1000     1000   120623 2024-05-15 13:55:59.000000 fleece_network-0.4.1/python/Cargo.lock
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 fleece_network-0.4.1/pyproject.toml
+-rw-r--r--   0     1000     1000     1788 2024-05-15 13:16:11.000000 fleece_network-0.4.1/pysrc/fleece_network/peer.py
+-rw-r--r--   0     1000     1000       55 2024-05-14 06:18:20.000000 fleece_network-0.4.1/pysrc/fleece_network/__init__.py
+-rw-r--r--   0     1000     1000        0 2024-05-14 04:35:00.000000 fleece_network-0.4.1/pysrc/fleece_network/py.typed
+-rw-r--r--   0     1000     1000      640 2024-05-15 06:51:33.000000 fleece_network-0.4.1/pysrc/fleece_network/serde.py
+-rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 fleece_network-0.4.1/PKG-INFO
```

### Comparing `fleece_network-0.4.0/fleece-network/Cargo.toml` & `fleece_network-0.4.1/fleece-network/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.0/fleece-network/Cargo.lock` & `fleece_network-0.4.1/fleece-network/Cargo.lock`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.0/fleece-network/src/bin/center.rs` & `fleece_network-0.4.1/fleece-network/src/bin/center.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.0/fleece-network/src/bin/peer.rs` & `fleece_network-0.4.1/fleece-network/src/bin/peer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 use bytes::Bytes;
 use fleece_network::{
     error::Error,
     peer::{codec, eventloop::Command, handler::Handler, peer::Peer},
 };
 use libp2p::{Multiaddr, PeerId};
-use log::info;
 use tokio::{
     io::{self, AsyncBufReadExt, BufReader},
     sync::oneshot,
     time::Instant,
 };
 use tower::{service_fn, util::BoxService};
 use tracing_subscriber::EnvFilter;
@@ -39,25 +38,26 @@
             Ok(codec::Response::new(req.route, Bytes::from("world")))
         })),
     );
 
     let addr = "/ip4/0.0.0.0/tcp/0".parse().unwrap();
     let peer = Peer::new(center_addr.clone(), center_peer_id, addr, handler);
     let peer_id = peer.peer_id;
-    info!("Peer ID: {}", peer_id);
+    println!("Peer ID: {}", peer_id);
 
     let command_tx = peer.command_tx.clone();
     tokio::spawn(peer.run());
 
     let stdin = BufReader::new(io::stdin());
     let mut lines = stdin.lines();
     while let Some(line) = lines.next_line().await.unwrap() {
         let request = codec::Request::new("hello".to_string(), Bytes::from(vec![0u8; 8192 * 2]));
         let (sender, receiver) = oneshot::channel();
         let start = Instant::now();
+        // info!("Sending");
         command_tx
             .send(Command::Request {
                 request,
                 peer_id: PeerId::from_str(&line).unwrap(),
                 sender,
             })
             .await
```

### Comparing `fleece_network-0.4.0/fleece-network/src/center/mod.rs` & `fleece_network-0.4.1/fleece-network/src/center/mod.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.0/fleece-network/src/channel/codec.rs` & `fleece_network-0.4.1/fleece-network/src/channel/codec.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.0/fleece-network/src/channel/handler.rs` & `fleece_network-0.4.1/fleece-network/src/channel/handler.rs`

 * *Files 17% similar despite different names*

```diff
@@ -13,126 +13,250 @@
 use libp2p_swarm::handler::{
     ConnectionEvent, DialUpgradeError, FullyNegotiatedInbound, FullyNegotiatedOutbound,
     ListenUpgradeError,
 };
 use libp2p_swarm::{
     ConnectionHandler, ConnectionHandlerEvent, StreamUpgradeError, SubstreamProtocol,
 };
-use tokio::time;
+use tokio::{
+    sync::{mpsc, oneshot},
+    time,
+};
 use tracing::info;
 
+use crate::channel::InboundHandle;
+
 use super::{
     codec::{Codec, CodecSink, CodecStream},
-    message::{InboundMessage, InboundRequestId, OutboundMessage, OutboundRequestId},
-    OneshotSender, OutboundHandle,
+    message::{InboundMessage, InboundRequestId, OutboundRequestId},
+    OneshotSender, OutboundHandle, OutboundMessage, RequestId,
 };
 
 pub struct Handler<C: Codec> {
     peer_id: PeerId,
     codec: C,
 
     stream: StatedStream<CodecStream<C::Decoder>>,
     sink: StatedSink<CodecSink<C::Encoder>>,
 
     request_timeout: Duration,
 
     protocol: C::Protocol,
     pending_events: VecDeque<Event<C>>,
-    pending_outbound_handles: VecDeque<OutboundHandle<C::Request, C::Response>>,
+    pending_outbound_messages: HashMap<RequestId, OutboundMessage<C::Request, C::Response>>,
+    inbound_request_sender: mpsc::Sender<InboundHandle<C::Request, C::Response>>,
     outbound_request_callbacks: HashMap<OutboundRequestId, OneshotSender<C::Response>>,
-    outbound_response_callbacks: HashMap<InboundRequestId, OneshotSender<()>>,
-    // inbound_request_futures:
-    //     FuturesUnordered<Pin<Box<dyn Future<Output = (InboundRequestId, C::Response)> + Send>>>,
+    inbound_request_futures:
+        FuturesUnordered<Pin<Box<dyn Future<Output = (InboundRequestId, C::Response)> + Send>>>,
     timeout_futures: FuturesUnordered<Pin<Box<dyn Future<Output = OutboundRequestId> + Send>>>,
+    inbound_request_workers: FuturesUnordered<Pin<Box<dyn Future<Output = ()> + Send>>>,
 }
 
 impl<C: Codec> Handler<C> {
     pub(super) fn new(
         peer_id: PeerId,
         codec: C,
         protocol: C::Protocol,
+        inbound_request_sender: mpsc::Sender<InboundHandle<C::Request, C::Response>>,
         request_timeout: Duration,
     ) -> Self {
         Self {
             peer_id,
             codec,
             stream: StatedStream::Pending(None),
             sink: StatedSink::Idle,
             request_timeout,
             protocol,
             pending_events: Default::default(),
-            pending_outbound_handles: Default::default(),
+            pending_outbound_messages: Default::default(),
+            inbound_request_sender,
             outbound_request_callbacks: Default::default(),
-            outbound_response_callbacks: Default::default(),
-            // inbound_request_futures: Default::default(),
-            timeout_futures: FuturesUnordered::new(),
+            inbound_request_futures: Default::default(),
+            timeout_futures: Default::default(),
+            inbound_request_workers: Default::default(),
         }
     }
 }
 
 impl<C> Handler<C>
 where
     C: Codec + Send + Debug + Clone + Unpin + 'static,
 {
-    fn send(&mut self, handle: OutboundHandle<C::Request, C::Response>) {
+    fn send_request(&mut self, handle: OutboundHandle<C::Request, C::Response>) {
+        let request_timeout = self.request_timeout;
+        let request_id = handle.id;
+        let (message, callback) = handle.split();
+        self.timeout_futures.push(
+            async move {
+                time::sleep(request_timeout).await;
+                request_id
+            }
+            .boxed(),
+        );
+        self.outbound_request_callbacks.insert(request_id, callback);
+        self.send_message(message)
+    }
+
+    fn send_message(&mut self, message: OutboundMessage<C::Request, C::Response>) {
         match &mut self.sink {
-            StatedSink::Active(sink, waker) => match handle {
-                OutboundHandle::Request(request_id, request, callback) => {
-                    let message = OutboundMessage::Request(request_id, request);
-                    if let Err(_) = sink.start_send_unpin(message) {
-                        self.sink = StatedSink::Failed(None);
-                        callback
-                            .send(Err(io::Error::new(
-                                io::ErrorKind::BrokenPipe,
-                                "Buffer is full",
-                            )))
-                            .unwrap();
-                    } else {
-                        self.outbound_request_callbacks.insert(request_id, callback);
-                        let request_timeout = self.request_timeout.clone();
-                        self.timeout_futures.push(
-                            async move {
-                                time::sleep(request_timeout).await;
-                                request_id
-                            }
-                            .boxed(),
-                        );
-                        waker.as_ref().map(|waker| waker.wake_by_ref());
-                    }
-                }
-                OutboundHandle::Response(request_id, response, callback) => {
-                    let message = OutboundMessage::Response(request_id, response);
-                    if let Err(_) = sink.start_send_unpin(message) {
-                        self.sink = StatedSink::Failed(None);
-                        callback
-                            .send(Err(io::Error::new(
-                                io::ErrorKind::BrokenPipe,
-                                "Buffer is full",
-                            )))
-                            .unwrap();
-                    } else {
-                        self.outbound_response_callbacks
-                            .insert(request_id, callback);
-                        waker.as_ref().map(|waker| waker.wake_by_ref());
+            StatedSink::Active(sink, waker) => {
+                let request_id = match message {
+                    OutboundMessage::Request(request_id, _) => Some(request_id),
+                    _ => None,
+                };
+                if let Err(_) = sink.start_send_unpin(message) {
+                    self.sink = StatedSink::Failed(None);
+                    if let Some(request_id) = request_id {
+                        if let Some(callback) = self.outbound_request_callbacks.remove(&request_id)
+                        {
+                            callback
+                                .send(Err(io::Error::new(
+                                    io::ErrorKind::BrokenPipe,
+                                    "Buffer is full",
+                                )))
+                                .unwrap();
+                        }
                     }
+                } else {
+                    waker.as_ref().map(|waker| waker.wake_by_ref());
                 }
-            },
+            }
 
             StatedSink::Failed(waker) => {
                 waker.as_ref().map(|waker| waker.wake_by_ref());
                 self.sink = StatedSink::Idle;
-                self.pending_outbound_handles.push_back(handle);
+                self.pending_outbound_messages
+                    .insert(message.request_id(), message);
             }
 
             _ => {
-                self.pending_outbound_handles.push_back(handle);
+                self.pending_outbound_messages
+                    .insert(message.request_id(), message);
             }
         }
     }
 
+    fn flush(
+        &mut self,
+        cx: &mut Context<'_>,
+    ) -> Poll<
+        ConnectionHandlerEvent<
+            <Self as ConnectionHandler>::OutboundProtocol,
+            <Self as ConnectionHandler>::OutboundOpenInfo,
+            <Self as ConnectionHandler>::ToBehaviour,
+        >,
+    > {
+        match &mut self.sink {
+            StatedSink::Idle => {
+                self.sink = StatedSink::Pending(None);
+                info!("Send outbound substream request to {:?}", self.peer_id);
+                return Poll::Ready(ConnectionHandlerEvent::OutboundSubstreamRequest {
+                    protocol: SubstreamProtocol::new(ReadyUpgrade::new(self.protocol.clone()), ()),
+                });
+            }
+            StatedSink::Active(sink, waker) => match sink.poll_flush_unpin(cx) {
+                Poll::Ready(result) => {
+                    waker.replace(cx.waker().clone());
+                    match result {
+                        Ok(_) => {}
+                        Err(_) => {
+                            info!("Fail when write into sink");
+                            self.sink = StatedSink::Failed(Some(cx.waker().clone()));
+                            let request_callbacks = mem::replace(
+                                &mut self.outbound_request_callbacks,
+                                Default::default(),
+                            );
+                            request_callbacks.into_values().for_each(|callback| {
+                                callback
+                                    .send(Err(io::Error::new(
+                                        io::ErrorKind::BrokenPipe,
+                                        "Failed to send",
+                                    )))
+                                    .unwrap();
+                            });
+                        }
+                    }
+                }
+                Poll::Pending => {}
+            },
+            StatedSink::Failed(_) => {
+                self.sink = StatedSink::Failed(Some(cx.waker().clone()));
+            }
+            StatedSink::Pending(_) => {
+                self.sink = StatedSink::Pending(Some(cx.waker().clone()));
+            }
+        }
+
+        Poll::Pending
+    }
+
+    fn recv(
+        &mut self,
+        cx: &mut Context<'_>,
+    ) -> Poll<
+        ConnectionHandlerEvent<
+            <Self as ConnectionHandler>::OutboundProtocol,
+            <Self as ConnectionHandler>::OutboundOpenInfo,
+            <Self as ConnectionHandler>::ToBehaviour,
+        >,
+    > {
+        loop {
+            match &mut self.stream {
+                StatedStream::Active(stream) => match stream.poll_next_unpin(cx) {
+                    Poll::Ready(option) => match option {
+                        Some(message) => match message {
+                            InboundMessage::Request(request_id, request) => {
+                                info!("Received request from {:?}", self.peer_id);
+                                let (sender, receiver) = oneshot::channel();
+                                self.inbound_request_futures.push(Box::pin(async move {
+                                    (request_id, receiver.await.unwrap())
+                                }));
+                                let handle = InboundHandle::new(request_id, request, sender);
+                                let sender = self.inbound_request_sender.clone();
+                                self.inbound_request_workers.push(Box::pin(async move {
+                                    sender.send(handle).await.unwrap();
+                                }));
+                            }
+                            InboundMessage::Response(request_id, response) => {
+                                info!(
+                                    "Received response from {:?} for {:?}",
+                                    self.peer_id, request_id
+                                );
+                                if let Some(sender) =
+                                    self.outbound_request_callbacks.remove(&request_id)
+                                {
+                                    sender.send(Ok(response)).unwrap();
+                                } else {
+                                    return Poll::Ready(ConnectionHandlerEvent::NotifyBehaviour(
+                                        Event::MissedResponse {
+                                            request_id,
+                                            response,
+                                        },
+                                    ));
+                                }
+                            }
+                        },
+                        None => {
+                            info!("Inbound stream {:?} fails", self.peer_id);
+                            break;
+                        }
+                    },
+                    Poll::Pending => break,
+                },
+
+                StatedStream::Pending(_) => {
+                    self.stream = StatedStream::Pending(Some(cx.waker().clone()));
+                    break;
+                }
+            }
+        }
+
+        Poll::Pending
+    }
+
     fn on_fully_negotiated_inbound(
         &mut self,
         FullyNegotiatedInbound {
             protocol: stream,
             info: (),
         }: FullyNegotiatedInbound<
             <Self as ConnectionHandler>::InboundProtocol,
@@ -158,28 +282,30 @@
     ) {
         match &self.sink {
             StatedSink::Pending(Some(waker)) => waker.wake_by_ref(),
             StatedSink::Failed(Some(waker)) => waker.wake_by_ref(),
             _ => {}
         }
         self.sink = StatedSink::Active(CodecSink::new(stream, self.codec.new_encoder()), None);
+
         let pending_outbound_messages =
-            mem::replace(&mut self.pending_outbound_handles, VecDeque::new());
-        for message in pending_outbound_messages {
-            self.send(message);
+            mem::replace(&mut self.pending_outbound_messages, Default::default());
+        for message in pending_outbound_messages.into_values() {
+            self.send_message(message);
         }
     }
 
     fn on_dial_upgrade_error(
         &mut self,
         DialUpgradeError { error, info: () }: DialUpgradeError<
             <Self as ConnectionHandler>::OutboundOpenInfo,
             <Self as ConnectionHandler>::OutboundProtocol,
         >,
     ) {
+        info!("Dial upgrade error: {:?}", error);
         match error {
             StreamUpgradeError::Timeout => {
                 self.pending_events
                     .push_back(Event::OutboundStreamFailure(ChannelFailure::Timeout));
             }
             StreamUpgradeError::NegotiationFailed => {
                 self.pending_events.push_back(Event::OutboundStreamFailure(
@@ -196,14 +322,15 @@
     fn on_listen_upgrade_error(
         &mut self,
         ListenUpgradeError { error, .. }: ListenUpgradeError<
             <Self as ConnectionHandler>::InboundOpenInfo,
             <Self as ConnectionHandler>::InboundProtocol,
         >,
     ) {
+        info!("Listen upgrade error: {:?}", error);
         void::unreachable(error)
     }
 }
 
 impl<C> ConnectionHandler for Handler<C>
 where
     C: Codec + Send + Debug + Clone + Unpin + 'static,
@@ -216,188 +343,73 @@
 
     type OutboundProtocol = ReadyUpgrade<C::Protocol>;
 
     type InboundOpenInfo = ();
 
     type OutboundOpenInfo = ();
 
-    fn listen_protocol(
-        &self,
-    ) -> libp2p_swarm::SubstreamProtocol<Self::InboundProtocol, Self::InboundOpenInfo> {
+    fn listen_protocol(&self) -> SubstreamProtocol<Self::InboundProtocol, Self::InboundOpenInfo> {
         SubstreamProtocol::new(ReadyUpgrade::new(self.protocol.clone()), ())
     }
 
     fn poll(
         &mut self,
         cx: &mut Context<'_>,
-    ) -> std::task::Poll<
-        libp2p_swarm::ConnectionHandlerEvent<
-            Self::OutboundProtocol,
-            Self::OutboundOpenInfo,
-            Self::ToBehaviour,
-        >,
+    ) -> Poll<
+        ConnectionHandlerEvent<Self::OutboundProtocol, Self::OutboundOpenInfo, Self::ToBehaviour>,
     > {
-        match &mut self.sink {
-            StatedSink::Idle => {
-                self.sink = StatedSink::Pending(None);
-                info!("Send outbound substream request to {:?}", self.peer_id);
-                return Poll::Ready(ConnectionHandlerEvent::OutboundSubstreamRequest {
-                    protocol: SubstreamProtocol::new(ReadyUpgrade::new(self.protocol.clone()), ()),
-                });
-            }
-            StatedSink::Active(sink, waker) => {
-                waker.replace(cx.waker().clone());
-                match sink.poll_flush_unpin(cx) {
-                    Poll::Ready(result) => match result {
-                        Ok(_) => {
-                            let callbacks = mem::replace(
-                                &mut self.outbound_response_callbacks,
-                                Default::default(),
-                            );
-                            callbacks.into_values().for_each(|callback| {
-                                callback.send(Ok(())).unwrap();
-                            });
-                        }
-                        Err(_) => {
-                            self.sink = StatedSink::Failed(Some(cx.waker().clone()));
-                            let request_callbacks = mem::replace(
-                                &mut self.outbound_request_callbacks,
-                                Default::default(),
-                            );
-                            request_callbacks.into_values().for_each(|callback| {
-                                callback
-                                    .send(Err(io::Error::new(
-                                        io::ErrorKind::BrokenPipe,
-                                        "Failed to send",
-                                    )))
-                                    .unwrap();
-                            });
-                            let response_callbacks = mem::replace(
-                                &mut self.outbound_response_callbacks,
-                                Default::default(),
-                            );
-                            response_callbacks.into_values().for_each(|callback| {
-                                callback
-                                    .send(Err(io::Error::new(
-                                        io::ErrorKind::BrokenPipe,
-                                        "Failed to send",
-                                    )))
-                                    .unwrap();
-                            });
-                        }
-                    },
-                    Poll::Pending => {}
-                }
-            }
-            StatedSink::Failed(_) => {
-                self.sink = StatedSink::Failed(Some(cx.waker().clone()));
-            }
-            StatedSink::Pending(_) => {
-                self.sink = StatedSink::Pending(Some(cx.waker().clone()));
-            }
-        }
-
         if let Some(event) = self.pending_events.pop_front() {
             return Poll::Ready(ConnectionHandlerEvent::NotifyBehaviour(event));
         }
 
-        loop {
-            match &mut self.stream {
-                StatedStream::Active(stream) => match stream.poll_next_unpin(cx) {
-                    Poll::Ready(option) => match option {
-                        Some(message) => match message {
-                            InboundMessage::Request(request_id, request) => {
-                                info!("Received request from {:?}", self.peer_id);
-                                // let (sender, receiver) = oneshot::channel();
-                                // self.inbound_request_futures.push(Box::pin(async move {
-                                //     (request_id, receiver.await.unwrap())
-                                // }));
-                                return Poll::Ready(ConnectionHandlerEvent::NotifyBehaviour(
-                                    Event::Request {
-                                        peer_id: self.peer_id,
-                                        request_id,
-                                        request,
-                                    },
-                                ));
-                            }
-                            InboundMessage::Response(request_id, response) => {
-                                info!("Received response from {:?}", self.peer_id);
-                                if let Some(sender) =
-                                    self.outbound_request_callbacks.remove(&request_id)
-                                {
-                                    sender.send(Ok(response)).unwrap();
-                                } else {
-                                    return Poll::Ready(ConnectionHandlerEvent::NotifyBehaviour(
-                                        Event::MissedResponse {
-                                            request_id,
-                                            response,
-                                        },
-                                    ));
-                                }
-                            }
-                        },
-                        None => {
-                            info!("Inbound stream {:?} fails", self.peer_id);
-                            self.stream = StatedStream::Pending(Some(cx.waker().clone()));
-                            break;
-                        }
-                    },
-                    Poll::Pending => break,
-                },
+        if let Poll::Ready(event) = self.flush(cx) {
+            return Poll::Ready(event);
+        }
 
-                StatedStream::Pending(_) => {
-                    self.stream = StatedStream::Pending(Some(cx.waker().clone()));
-                    break;
+        if let Poll::Ready(event) = self.recv(cx) {
+            return Poll::Ready(event);
+        }
+
+        while !self.inbound_request_futures.is_empty() {
+            match self.inbound_request_futures.poll_next_unpin(cx) {
+                Poll::Ready(Some((request_id, response))) => {
+                    self.send_message(OutboundMessage::Response(request_id, response));
                 }
+                _ => break,
             }
         }
 
-        // loop {
-        //     match self.inbound_request_futures.poll_next_unpin(cx) {
-        //         Poll::Ready(result) => {
-        //             if let Some((request_id, response)) = result {
-        //                 if let Some(sender) = self.outbound_response_callbacks.remove(&request_id) {
-        //                     sender.send(Ok(())).unwrap();
-        //                 }
-        //                 return Poll::Ready(ConnectionHandlerEvent::NotifyBehaviour(
-        //                     Event::MissedResponse {
-        //                         request_id,
-        //                         response,
-        //                     },
-        //                 ));
-        //             }
-        //         }
-        //         _ => break,
-        //     }
-        // }
-
         while !self.timeout_futures.is_empty() {
             match self.timeout_futures.poll_next_unpin(cx) {
-                Poll::Ready(event) => {
-                    if let Some(request_id) = event {
-                        if let Some(sender) = self.outbound_request_callbacks.remove(&request_id) {
-                            info!("Polling timeout futures");
-                            sender
-                                .send(Err(io::Error::new(
-                                    io::ErrorKind::TimedOut,
-                                    "Request timed out",
-                                )))
-                                .unwrap();
-                        }
+                Poll::Ready(Some(request_id)) => {
+                    if let Some(sender) = self.outbound_request_callbacks.remove(&request_id) {
+                        sender
+                            .send(Err(io::Error::new(
+                                io::ErrorKind::TimedOut,
+                                "Request timed out",
+                            )))
+                            .unwrap();
                     }
                 }
                 _ => break,
             }
         }
 
+        while !self.inbound_request_workers.is_empty() {
+            match self.inbound_request_workers.poll_next_unpin(cx) {
+                Poll::Ready(Some(_)) => {}
+                _ => break,
+            }
+        }
+
         Poll::Pending
     }
 
     fn on_behaviour_event(&mut self, event: OutboundHandle<C::Request, C::Response>) {
-        self.send(event);
+        self.send_request(event);
     }
 
     fn on_connection_event(
         &mut self,
         event: libp2p_swarm::handler::ConnectionEvent<
             Self::InboundProtocol,
             Self::OutboundProtocol,
@@ -439,19 +451,14 @@
 }
 
 #[derive(Debug)]
 pub enum Event<C>
 where
     C: Codec,
 {
-    Request {
-        peer_id: PeerId,
-        request_id: InboundRequestId,
-        request: C::Request,
-    },
     MissedResponse {
         request_id: OutboundRequestId,
         response: C::Response,
     },
     InboundStreamFailure(ChannelFailure),
     OutboundStreamFailure(ChannelFailure),
 }
```

### Comparing `fleece_network-0.4.0/fleece-network/src/channel/message.rs` & `fleece_network-0.4.1/fleece-network/src/channel/message.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use std::{fmt::Debug, io};
 
 use serde::{Deserialize, Serialize};
 use tokio::sync::oneshot;
 
 pub(crate) type OneshotSender<T> = oneshot::Sender<Result<T, io::Error>>;
+pub(crate) type DirectSender<T> = oneshot::Sender<T>;
 
 #[derive(Debug, Clone, Copy, Eq, Hash, PartialEq, Deserialize, Serialize)]
 pub struct InboundRequestId(pub u64);
 
 impl From<OutboundRequestId> for InboundRequestId {
     fn from(value: OutboundRequestId) -> Self {
         Self(value.0)
@@ -59,14 +60,20 @@
             InboundMessage::Response(id, response) => {
                 OutboundMessage::Response(id.into(), response)
             }
         }
     }
 }
 
+impl<Req, Resp> From<OutboundHandle<Req, Resp>> for OutboundMessage<Req, Resp> {
+    fn from(value: OutboundHandle<Req, Resp>) -> Self {
+        OutboundMessage::Request(value.id, value.request)
+    }
+}
+
 #[derive(Deserialize, Serialize, Debug)]
 pub enum InboundMessage<Req, Resp> {
     Request(InboundRequestId, Req),
     Response(OutboundRequestId, Resp),
 }
 
 impl<Req, Resp> InboundMessage<Req, Resp> {
@@ -85,32 +92,84 @@
             OutboundMessage::Response(id, response) => {
                 InboundMessage::Response(id.into(), response)
             }
         }
     }
 }
 
+impl<Req, Resp> From<InboundHandle<Req, Resp>> for InboundMessage<Req, Resp> {
+    fn from(value: InboundHandle<Req, Resp>) -> Self {
+        InboundMessage::Request(value.id, value.request)
+    }
+}
+
+#[derive(Debug)]
+pub struct OutboundHandle<Req, Resp> {
+    pub id: OutboundRequestId,
+    pub request: Req,
+    pub sender: OneshotSender<Resp>,
+}
+
+impl<Req, Resp> OutboundHandle<Req, Resp> {
+    pub fn new(id: OutboundRequestId, request: Req, sender: OneshotSender<Resp>) -> Self {
+        Self {
+            id,
+            request,
+            sender,
+        }
+    }
+
+    pub fn split(self) -> (OutboundMessage<Req, Resp>, OneshotSender<Resp>) {
+        (OutboundMessage::Request(self.id, self.request), self.sender)
+    }
+}
+
+#[derive(Debug)]
+pub struct InboundHandle<Req, Resp> {
+    pub id: InboundRequestId,
+    pub request: Req,
+    pub sender: DirectSender<Resp>,
+}
+
+impl<Req, Resp> InboundHandle<Req, Resp> {
+    pub fn new(id: InboundRequestId, request: Req, sender: DirectSender<Resp>) -> Self {
+        Self {
+            id,
+            request,
+            sender,
+        }
+    }
+
+    pub fn split(self) -> (InboundMessage<Req, Resp>, DirectSender<Resp>) {
+        (InboundMessage::Request(self.id, self.request), self.sender)
+    }
+
+    pub fn into_parts(self) -> (InboundRequestId, Req, DirectSender<Resp>) {
+        (self.id, self.request, self.sender)
+    }
+}
+
 #[derive(Debug)]
-pub enum OutboundHandle<Req, Resp> {
+pub enum OutboundHandleFake<Req, Resp> {
     Request(OutboundRequestId, Req, OneshotSender<Resp>),
     Response(InboundRequestId, Resp, OneshotSender<()>),
 }
 
-impl<Req, Resp> OutboundHandle<Req, Resp> {
-    pub fn split(self) -> (OutboundMessage<Req, Resp>, OutboundCallback<Resp>) {
+impl<Req, Resp> OutboundHandleFake<Req, Resp> {
+    pub fn split(self) -> (OutboundMessage<Req, Resp>, OutboundCallbackFake<Resp>) {
         match self {
-            OutboundHandle::Request(id, request, sender) => (
+            OutboundHandleFake::Request(id, request, sender) => (
                 OutboundMessage::Request(id, request),
-                OutboundCallback::Request(sender),
+                OutboundCallbackFake::Request(sender),
             ),
-            OutboundHandle::Response(id, response, sender) => (
+            OutboundHandleFake::Response(id, response, sender) => (
                 OutboundMessage::Response(id, response),
-                OutboundCallback::Response(sender),
+                OutboundCallbackFake::Response(sender),
             ),
         }
     }
 }
 
-pub enum OutboundCallback<Resp> {
+pub enum OutboundCallbackFake<Resp> {
     Request(OneshotSender<Resp>),
     Response(OneshotSender<()>),
 }
```

### Comparing `fleece_network-0.4.0/fleece-network/src/peer/codec.rs` & `fleece_network-0.4.1/fleece-network/src/peer/codec.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.0/fleece-network/src/peer/codec_legacy.rs` & `fleece_network-0.4.1/fleece-network/src/peer/codec_legacy.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.0/fleece-network/src/peer/eventloop.rs` & `fleece_network-0.4.1/fleece-network/src/peer/eventloop.rs`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,33 @@
     swarm::{dial_opts::DialOpts, SwarmEvent},
     Multiaddr, PeerId, Swarm,
 };
 use tokio::{
     sync::{mpsc, oneshot},
     time::{self, Interval},
 };
-use tracing::{debug, info};
+use tracing::{debug, info, warn};
 
 use crate::{
-    channel::{self, InboundRequestId, OneshotSender},
+    channel::{self, OneshotSender},
     error::Error,
 };
 
 use super::{
     behaviour::{Behaviour, BehaviourEvent},
     codec,
 };
 
 type Medium<T> = oneshot::Sender<Result<T, Error>>;
 
-pub(super) struct EventLoop {
+pub struct EventLoop {
     swarm: Swarm<Behaviour>,
 
     command_tx: mpsc::Sender<Command>,
     command_rx: mpsc::Receiver<Command>,
-    event_tx: mpsc::Sender<Event>,
 
     center_addr: Multiaddr,
     center_peer_id: PeerId,
 
     interval: Interval,
     last_cookie: Option<Cookie>,
 
@@ -43,23 +42,21 @@
 }
 
 impl EventLoop {
     pub fn new(
         swarm: Swarm<Behaviour>,
         command_tx: mpsc::Sender<Command>,
         command_rx: mpsc::Receiver<Command>,
-        event_tx: mpsc::Sender<Event>,
         center_addr: Multiaddr,
         center_peer_id: PeerId,
     ) -> Self {
         Self {
             swarm,
             command_tx,
             command_rx,
-            event_tx,
             center_addr,
             center_peer_id,
             interval: time::interval(Duration::from_secs(1)),
             last_cookie: None,
             pending_dials: Default::default(),
         }
     }
@@ -128,29 +125,20 @@
                             &event.peer,
                             event.connection,
                             duration,
                         );
                     }
                 }
                 BehaviourEvent::Channel(event) => match event {
-                    channel::behaviour::Event::Request {
-                        peer_id,
+                    channel::behaviour::Event::MissedResponse {
                         request_id,
-                        request,
+                        response: _,
                     } => {
-                        self.event_tx
-                            .send(Event::Request {
-                                peer_id,
-                                request_id,
-                                request,
-                            })
-                            .await
-                            .unwrap();
+                        warn!("Missed response: {:?}", request_id);
                     }
-                    channel::behaviour::Event::MissedResponse { .. } => todo!(),
                     channel::behaviour::Event::Failure { peer_id, failure } => {
                         info!("Channel failure {:?}: {:?}", peer_id, failure);
                     }
                 },
             },
             SwarmEvent::ConnectionEstablished {
                 peer_id, endpoint, ..
@@ -188,23 +176,27 @@
                 info!("Outgoing connection error: {:?}", error);
                 if let Some(peer_id) = peer_id {
                     if let Some(sender) = self.pending_dials.remove(&peer_id) {
                         sender.send(Err(Error::from(error))).unwrap();
                     }
                 }
             }
-            SwarmEvent::NewListenAddr { .. } => {}
+            SwarmEvent::NewListenAddr {
+                listener_id: _,
+                address,
+            } => {
+                info!("New listen address: {}", address);
+            }
             SwarmEvent::ExpiredListenAddr { .. } => {}
             SwarmEvent::ListenerClosed { .. } => {}
             SwarmEvent::ListenerError { .. } => {}
             SwarmEvent::Dialing { .. } => {}
             SwarmEvent::NewExternalAddrCandidate { .. } => {}
             SwarmEvent::ExternalAddrConfirmed { address } => {
                 info!("External address confirmed: {}", address);
-                println!("External address confirmed: {}", address);
             }
             SwarmEvent::ExternalAddrExpired { .. } => {}
             SwarmEvent::NewExternalAddrOfPeer { peer_id, address } => {
                 info!("New external address of peer {}: {}", peer_id, address);
             }
             _ => todo!(),
         }
@@ -272,25 +264,14 @@
                 sender,
             } => {
                 self.swarm
                     .behaviour_mut()
                     .channel
                     .send_request(&peer_id, request, sender);
             }
-            Command::Response {
-                peer_id,
-                request_id,
-                response,
-                sender,
-            } => {
-                self.swarm
-                    .behaviour_mut()
-                    .channel
-                    .send_response(&peer_id, request_id, response, sender);
-            }
         }
     }
 }
 
 #[derive(Debug)]
 pub enum Command {
     Dial {
@@ -308,22 +289,8 @@
         namespace: String,
     },
     Request {
         peer_id: PeerId,
         request: codec::Request,
         sender: OneshotSender<codec::Response>,
     },
-    Response {
-        peer_id: PeerId,
-        request_id: channel::InboundRequestId,
-        response: codec::Response,
-        sender: OneshotSender<()>,
-    },
-}
-
-pub(super) enum Event {
-    Request {
-        peer_id: PeerId,
-        request_id: InboundRequestId,
-        request: codec::Request,
-    },
 }
```

### Comparing `fleece_network-0.4.0/fleece-network/src/peer/handler.rs` & `fleece_network-0.4.1/fleece-network/src/peer/handler.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.0/fleece-network/src/peer/peer.rs` & `fleece_network-0.4.1/fleece-network/src/peer/peer.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 use std::time::Duration;
 
 use bytes::Bytes;
 use libp2p::{identity, swarm, Multiaddr, PeerId, Swarm};
-use tokio::sync::{mpsc, oneshot};
+use tokio::sync::mpsc;
 use tower::Service;
 
-use crate::{error::Error, router::Router, transport::TransportBuilder};
+use crate::{channel::InboundHandle, error::Error, router::Router, transport::TransportBuilder};
 
 use super::{
     behaviour::Behaviour,
     codec,
-    eventloop::{Command, Event, EventLoop},
+    eventloop::{Command, EventLoop},
     handler::Handler,
 };
 
 pub struct Peer {
     pub peer_id: PeerId,
 
     eventloop: EventLoop,
 
     router:
         Router<codec::Request, codec::Response, Error, Handler<codec::Request, codec::Response>>,
+    request_receiver: mpsc::Receiver<InboundHandle<codec::Request, codec::Response>>,
 
-    event_rx: mpsc::Receiver<Event>,
     pub command_tx: mpsc::Sender<Command>,
 }
 
 impl Peer {
     pub fn new(
         center_addr: Multiaddr,
         center_peer_id: PeerId,
@@ -37,85 +37,61 @@
         let peer_id = keypair.public().to_peer_id();
         let transport_builder = TransportBuilder::new(keypair.clone())
             .with_tcp()
             .with_ws()
             .with_quic();
         let (transport_builder, relay_behaviour) = transport_builder.with_relay();
         let transport = transport_builder.build();
-        let behaviour = Behaviour::new(&keypair, relay_behaviour);
+        let (behaviour, receiver) = Behaviour::new(&keypair, relay_behaviour);
         let swarm_config = swarm::Config::with_tokio_executor()
             .with_idle_connection_timeout(Duration::from_secs(600));
         let mut swarm = Swarm::new(transport, behaviour, peer_id.clone(), swarm_config);
 
         // setup for direct connection
         swarm.listen_on(self_addr.clone()).unwrap();
 
         // setup for stream
 
         let (command_tx, command_rx) = mpsc::channel(32);
-        let (event_tx, event_rx) = mpsc::channel(32);
         let eventloop = EventLoop::new(
             swarm,
             command_tx.clone(),
             command_rx,
-            event_tx,
             center_addr.clone(),
             center_peer_id.clone(),
         );
 
         Self {
             peer_id,
             eventloop,
             router: Router::new(handler),
-            event_rx,
+            request_receiver: receiver,
             command_tx,
         }
     }
 
     pub async fn run(mut self) {
         tokio::spawn(self.eventloop.run());
         loop {
-            match self.event_rx.recv().await {
-                Some(event) => match event {
-                    Event::Request {
-                        peer_id,
-                        request_id,
-                        request,
-                    } => {
-                        let future = self.router.call(request);
-                        let command_tx = self.command_tx.clone();
-                        tokio::spawn(async move {
-                            let response = future.await;
-                            let (sender, receiver) = oneshot::channel();
-                            if response.is_err() {
-                                command_tx
-                                    .send(Command::Response {
-                                        peer_id,
-                                        request_id,
-                                        response: codec::Response::new(
-                                            String::from("error"),
-                                            Bytes::default(),
-                                        ),
-                                        sender,
-                                    })
-                                    .await
-                                    .unwrap();
-                            } else {
-                                command_tx
-                                    .send(Command::Response {
-                                        peer_id,
-                                        request_id,
-                                        response: response.unwrap(),
-                                        sender,
-                                    })
-                                    .await
-                                    .unwrap();
-                            }
-                            receiver.await.unwrap().unwrap();
-                        });
-                    }
-                },
+            match self.request_receiver.recv().await {
+                Some(handle) => {
+                    let (_, request, sender) = handle.into_parts();
+                    let future = self.router.call(request);
+                    tokio::spawn(async move {
+                        let response = future.await;
+                        if response.is_err() {
+                            sender
+                                .send(codec::Response::new(
+                                    String::from("error"),
+                                    Bytes::default(),
+                                ))
+                                .unwrap();
+                        } else {
+                            sender.send(response.unwrap()).unwrap();
+                        }
+                    });
+                }
                 None => break,
             }
         }
     }
 }
```

### Comparing `fleece_network-0.4.0/fleece-network/src/router.rs` & `fleece_network-0.4.1/fleece-network/src/router.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.0/fleece-network/src/transport.rs` & `fleece_network-0.4.1/fleece-network/src/transport.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.0/fleece-network/src/utils/chunk.rs` & `fleece_network-0.4.1/fleece-network/src/utils/chunk.rs`

 * *Files identical despite different names*

### Comparing `fleece_network-0.4.0/python/Cargo.toml` & `fleece_network-0.4.1/python/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "fleece-network-python"
-version = "0.4.0"
+version = "0.4.1"
 edition = "2021"
 
 [lib]
 name = "fleece_network_rust"
 crate-type = ["cdylib"]
 
 [dependencies]
@@ -16,13 +16,14 @@
 futures = "0.3.30"
 libp2p = "0.53.2"
 pyo3 = { version = "0.21.2", features = ["extension-module"] }
 pyo3-log = "0.10.0"
 safetensors = "0.4.3"
 tokio = { version = "1.37.0", features = ["full"] }
 tower = { version = "0.4.13", features = ["util"] }
+tracing-subscriber = { version = "0.3.18", features = ["env-filter"] }
 
 [profile.bench]
 opt-level = 3
 strip = true
 debug = false
 lto = true
```

### Comparing `fleece_network-0.4.0/python/example.py` & `fleece_network-0.4.1/python/example.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     "/ip4/127.0.0.1/tcp/9765/p2p/12D3KooWDpJ7As7BWAwRMfu1VU2WCqNjvq387JEYKDBj4kx6nXTN",
     "12D3KooWDpJ7As7BWAwRMfu1VU2WCqNjvq387JEYKDBj4kx6nXTN",
     "/ip4/0.0.0.0/tcp/0",
     {"hello": hello},
 )
 
 peer.run()
+print(peer.peer_id())
+# peer.enable_log()
 
 payload = b"0" * 8192 * 2
 
 while True:
     line = input()
     begin = time.time()
     peer.send(line, "hello", payload)
```

### Comparing `fleece_network-0.4.0/python/pysrc/fleece_network/serde.py` & `fleece_network-0.4.1/python/pysrc/fleece_network/serde.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pickle
 from typing import Any
-
 from safetensors.torch import load, save
+from torch import Tensor
 
 
-def dumps(tensors: dict[str, "Tensor"], metadata: dict[str, Any]) -> bytes:
+def dumps(tensors: dict[str, Tensor], metadata: dict[str, Any]) -> bytes:
     metadata_bytes = pickle.dumps(metadata)
     tensors_bytes = save(tensors)
     return (
         len(metadata_bytes).to_bytes(4, byteorder="big")
         + metadata_bytes
         + tensors_bytes
     )
 
 
-def loads(b: bytes) -> tuple[dict[str, "Tensor"], dict[str, Any]]:
+def loads(b: bytes) -> tuple[dict[str, Tensor], dict[str, Any]]:
     metadata_length = int.from_bytes(b[:4], byteorder="big")
     metadata = pickle.loads(b[4 : 4 + metadata_length])
     tensors = load(b[4 + metadata_length :])
     return tensors, metadata
```

### Comparing `fleece_network-0.4.0/python/src/proxy.rs` & `fleece_network-0.4.1/python/src/proxy.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 use std::{str::FromStr, thread};
 
 use bytes::Bytes;
 use crossbeam_channel::bounded;
 use fleece_network::{
-    channel::InboundRequestId,
+    channel::InboundHandle,
     peer::{codec, eventloop::Command, proxy::Proxy},
 };
 use libp2p::PeerId;
 use pyo3::prelude::*;
-use tokio::sync::oneshot;
+use tokio::sync::{mpsc, oneshot};
+use tracing_subscriber::EnvFilter;
 
 #[pyclass]
 #[derive(Default)]
 struct PyProxyBuilder {
     center_addr: Option<String>,
     center_peer_id: Option<String>,
     self_addr: Option<String>,
@@ -49,95 +50,108 @@
         thread::spawn(move || {
             let executor = tokio::runtime::Builder::new_multi_thread()
                 .worker_threads(32)
                 .enable_all()
                 .build()
                 .unwrap();
             executor.block_on(async {
-                let (proxy, future) = Proxy::new(center_addr, center_peer_id, self_addr);
+                let (proxy, eventloop) = Proxy::new(center_addr, center_peer_id, self_addr);
                 tx.send(proxy).unwrap();
-                future.await; // the only way to stall the thread
+                eventloop.run().await;
             });
         });
 
         let proxy = rx.recv().unwrap();
 
-        PyProxy { inner: proxy }
+        proxy.into()
     }
 }
 
 #[pyclass]
 struct PyProxy {
-    inner: Proxy,
+    peer_id: PeerId,
+    command_tx: mpsc::Sender<Command>,
+    request_rx: Option<mpsc::Receiver<InboundHandle<codec::Request, codec::Response>>>,
+}
+
+impl From<Proxy> for PyProxy {
+    fn from(value: Proxy) -> Self {
+        Self {
+            peer_id: value.peer_id,
+            command_tx: value.command_tx,
+            request_rx: Some(value.request_rx),
+        }
+    }
 }
 
 #[pymethods]
 impl PyProxy {
+    fn enable_log(_this: PyRefMut<'_, Self>) {
+        let _ = tracing_subscriber::fmt()
+            .event_format(
+                tracing_subscriber::fmt::format()
+                    .with_file(true)
+                    .with_line_number(true),
+            )
+            .with_env_filter(EnvFilter::from_default_env())
+            .try_init();
+    }
+
     fn peer_id(this: PyRef<'_, Self>) -> String {
-        this.inner.peer_id.to_string()
+        this.peer_id.to_string()
     }
 
-    fn send_request(
-        this: PyRefMut<'_, Self>,
-        peer_id: String,
-        request: PyCodecRequest,
-    ) -> PyCodecResponse {
+    fn send(this: PyRefMut<'_, Self>, peer_id: String, request: PyCodecRequest) -> PyCodecResponse {
         let (tx, rx) = oneshot::channel();
-        this.inner
-            .command_tx
+        this.command_tx
             .blocking_send(Command::Request {
                 peer_id: peer_id.parse().unwrap(),
                 request: request.into(),
                 sender: tx,
             })
             .unwrap();
         rx.blocking_recv().unwrap().unwrap().into()
     }
 
-    fn send_response(this: PyRefMut<'_, Self>, request_id: PyRequestId, response: PyCodecResponse) {
-        let (tx, rx) = oneshot::channel();
-        this.inner
-            .command_tx
-            .blocking_send(Command::Response {
-                peer_id: request_id.peer_id,
-                request_id: request_id.request_id,
-                response: response.into(),
-                sender: tx,
-            })
-            .unwrap();
-        rx.blocking_recv().unwrap().unwrap();
-    }
+    fn recv(this: Py<Self>, py: Python<'_>) -> Option<(PyCodecRequest, PyCallback)> {
+        let mut request_rx = this.borrow_mut(py).request_rx.take().unwrap();
+        let (request_rx, result) =
+            Python::allow_threads(py, move || match request_rx.blocking_recv() {
+                Some(handle) => {
+                    let (_, request, sender) = handle.into_parts();
+                    (request_rx, Some((request.into(), PyCallback::new(sender))))
+                }
+                None => (request_rx, None),
+            });
+        this.borrow_mut(py).request_rx = Some(request_rx);
 
-    fn recv(this: Py<Self>, py: Python<'_>) -> Option<(PyRequestId, PyCodecRequest)> {
-        let message_rx = this.borrow(py).inner.message_rx.clone();
-        Python::allow_threads(py, move || match message_rx.recv() {
-            Ok((peer_id, request_id, request)) => {
-                Some((PyRequestId::new(peer_id, request_id), request.into()))
-            }
-            Err(_) => None,
-        })
+        result
     }
 }
 
 #[pyclass]
-#[derive(Clone)]
-struct PyRequestId {
-    peer_id: PeerId,
-    request_id: InboundRequestId,
+struct PyCallback {
+    sender: Option<oneshot::Sender<codec::Response>>,
 }
 
-impl PyRequestId {
-    fn new(peer_id: PeerId, request_id: InboundRequestId) -> Self {
+impl PyCallback {
+    pub fn new(sender: oneshot::Sender<codec::Response>) -> Self {
         Self {
-            peer_id,
-            request_id,
+            sender: Some(sender),
         }
     }
 }
 
+#[pymethods]
+impl PyCallback {
+    fn send(mut this: PyRefMut<'_, Self>, response: PyCodecResponse) {
+        this.sender.take().unwrap().send(response.into()).unwrap();
+    }
+}
+
 #[pyclass]
 #[derive(Clone)]
 struct PyCodecRequest {
     #[pyo3(get, set)]
     route: String,
     #[pyo3(get, set)]
     payload: Vec<u8>,
@@ -211,12 +225,12 @@
     }
 }
 
 #[pymodule]
 fn fleece_network_rust(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<PyProxy>()?;
     m.add_class::<PyProxyBuilder>()?;
-    m.add_class::<PyRequestId>()?;
+    m.add_class::<PyCallback>()?;
     m.add_class::<PyCodecRequest>()?;
     m.add_class::<PyCodecResponse>()?;
     Ok(())
 }
```

### Comparing `fleece_network-0.4.0/python/Cargo.lock` & `fleece_network-0.4.1/python/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1226,28 +1226,29 @@
  "tracing-flame",
  "tracing-subscriber",
  "void",
 ]
 
 [[package]]
 name = "fleece-network-python"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "bytes",
  "chrono",
  "crossbeam-channel",
  "dyn-clone",
  "fleece-network",
  "futures",
  "libp2p",
  "pyo3",
  "pyo3-log",
  "safetensors",
  "tokio",
  "tower",
+ "tracing-subscriber",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
```

### Comparing `fleece_network-0.4.0/pyproject.toml` & `fleece_network-0.4.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [project]
-name = "fleece_network"
+name = "fleece-network"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Rust",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Typing :: Typed",
 ]
```

### Comparing `fleece_network-0.4.0/pysrc/fleece_network/serde.py` & `fleece_network-0.4.1/pysrc/fleece_network/serde.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pickle
 from typing import Any
-
 from safetensors.torch import load, save
+from torch import Tensor
 
 
-def dumps(tensors: dict[str, "Tensor"], metadata: dict[str, Any]) -> bytes:
+def dumps(tensors: dict[str, Tensor], metadata: dict[str, Any]) -> bytes:
     metadata_bytes = pickle.dumps(metadata)
     tensors_bytes = save(tensors)
     return (
         len(metadata_bytes).to_bytes(4, byteorder="big")
         + metadata_bytes
         + tensors_bytes
     )
 
 
-def loads(b: bytes) -> tuple[dict[str, "Tensor"], dict[str, Any]]:
+def loads(b: bytes) -> tuple[dict[str, Tensor], dict[str, Any]]:
     metadata_length = int.from_bytes(b[:4], byteorder="big")
     metadata = pickle.loads(b[4 : 4 + metadata_length])
     tensors = load(b[4 + metadata_length :])
     return tensors, metadata
```

