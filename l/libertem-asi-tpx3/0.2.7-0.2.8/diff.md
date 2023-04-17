# Comparing `tmp/libertem_asi_tpx3-0.2.7.tar.gz` & `tmp/libertem_asi_tpx3-0.2.8.tar.gz`

## Comparing `libertem_asi_tpx3-0.2.7.tar` & `libertem_asi_tpx3-0.2.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/Cargo.toml
--rw-r--r--   0     1001      123      247 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/README.md
--rw-r--r--   0     1001      123     2815 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/examples/consumer/main.rs
--rw-r--r--   0     1001      123     3772 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/examples/producer/main.rs
--rwxr-xr-x   0     1001      123      121 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/run-consumer.sh
--rwxr-xr-x   0     1001      123      121 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/run-producer.sh
--rw-r--r--   0     1001      123       31 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/rust-toolchain.toml
--rw-r--r--   0     1001      123     6872 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/src/backend_memfd.rs
--rw-r--r--   0     1001      123     2823 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/src/backend_shm.rs
--rw-r--r--   0     1001      123     3741 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/src/freestack.rs
--rw-r--r--   0     1001      123     1029 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/src/lib.rs
--rw-r--r--   0     1001      123    19891 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/src/slab.rs
--rw-r--r--   0        0        0      189 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.7/local_dependencies/stats/Cargo.toml
--rw-r--r--   0     1001      123     2581 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/local_dependencies/stats/src/lib.rs
--rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.7/Cargo.toml
--rw-r--r--   0     1001      123      332 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/README.md
--rw-r--r--   0     1001      123    14832 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/examples/acquisition.py
--rw-r--r--   0     1001      123     3363 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/examples/compare.py
--rw-r--r--   0     1001      123     1443 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/examples/crash.py
--rw-r--r--   0     1001      123     1096 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/examples/live_client.py
--rw-r--r--   0     1001      123    12763 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/examples/live_server.py
--rw-r--r--   0     1001      123     1361 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/examples/run_udf.py
--rw-r--r--   0     1001      123     2540 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/examples/sim.py
--rw-r--r--   0     1001      123     2274 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/examples/simple.py
--rw-r--r--   0     1001      123      450 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/pyproject.toml
--rw-r--r--   0     1001      123       31 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/rust-toolchain.toml
--rw-r--r--   0     1001      123     6609 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/cam_client.rs
--rw-r--r--   0     1001      123    25695 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/chunk_stack.rs
--rw-r--r--   0     1001      123      343 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/common.rs
--rw-r--r--   0     1001      123     4293 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/csr_view.rs
--rw-r--r--   0     1001      123     3384 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/csr_view_raw.rs
--rw-r--r--   0     1001      123      987 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/deserialize.rs
--rw-r--r--   0     1001      123      291 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/exceptions.rs
--rw-r--r--   0     1001      123     7487 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/headers.rs
--rw-r--r--   0     1001      123      649 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/headers_py.rs
--rw-r--r--   0     1001      123      280 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/lib.rs
--rw-r--r--   0     1001      123    11265 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/main_py.rs
--rw-r--r--   0     1001      123    21644 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/receiver.rs
--rw-r--r--   0     1001      123      872 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/serialize.rs
--rw-r--r--   0     1001      123    18935 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/sparse_csr.rs
--rw-r--r--   0     1001      123      746 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/stats.rs
--rw-r--r--   0     1001      123     2489 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/src/stream.rs
--rw-r--r--   0     1001      123    95572 2023-03-22 14:09:24.000000 libertem_asi_tpx3-0.2.7/Cargo.lock
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      189 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.8/local_dependencies/stats/Cargo.toml
+-rw-r--r--   0     1001      123     2581 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/stats/src/lib.rs
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/Cargo.toml
+-rw-r--r--   0     1001      123      247 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/README.md
+-rw-r--r--   0     1001      123     2815 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/examples/consumer/main.rs
+-rw-r--r--   0     1001      123     3772 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/examples/producer/main.rs
+-rwxr-xr-x   0     1001      123      121 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/run-consumer.sh
+-rwxr-xr-x   0     1001      123      121 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/run-producer.sh
+-rw-r--r--   0     1001      123       31 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/rust-toolchain.toml
+-rw-r--r--   0     1001      123     6872 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/backend_memfd.rs
+-rw-r--r--   0     1001      123     2823 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/backend_shm.rs
+-rw-r--r--   0     1001      123     3741 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/freestack.rs
+-rw-r--r--   0     1001      123     1029 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/lib.rs
+-rw-r--r--   0     1001      123    19891 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/slab.rs
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.8/Cargo.toml
+-rw-r--r--   0     1001      123      332 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/README.md
+-rw-r--r--   0     1001      123    14832 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/acquisition.py
+-rw-r--r--   0     1001      123     3363 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/compare.py
+-rw-r--r--   0     1001      123     1443 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/crash.py
+-rw-r--r--   0     1001      123     1096 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/live_client.py
+-rw-r--r--   0     1001      123    12763 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/live_server.py
+-rw-r--r--   0     1001      123     1361 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/run_udf.py
+-rw-r--r--   0     1001      123     2540 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/sim.py
+-rw-r--r--   0     1001      123     2274 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/examples/simple.py
+-rw-r--r--   0     1001      123      450 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/pyproject.toml
+-rw-r--r--   0     1001      123       31 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/rust-toolchain.toml
+-rw-r--r--   0     1001      123     6609 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/cam_client.rs
+-rw-r--r--   0     1001      123    25695 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/chunk_stack.rs
+-rw-r--r--   0     1001      123      343 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/common.rs
+-rw-r--r--   0     1001      123     4293 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/csr_view.rs
+-rw-r--r--   0     1001      123     3384 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/csr_view_raw.rs
+-rw-r--r--   0     1001      123      987 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/deserialize.rs
+-rw-r--r--   0     1001      123      291 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/exceptions.rs
+-rw-r--r--   0     1001      123     7487 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/headers.rs
+-rw-r--r--   0     1001      123      649 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/headers_py.rs
+-rw-r--r--   0     1001      123      280 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/lib.rs
+-rw-r--r--   0     1001      123    11265 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/main_py.rs
+-rw-r--r--   0     1001      123    22613 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/receiver.rs
+-rw-r--r--   0     1001      123      872 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/serialize.rs
+-rw-r--r--   0     1001      123    18935 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/sparse_csr.rs
+-rw-r--r--   0     1001      123      746 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/stats.rs
+-rw-r--r--   0     1001      123     2672 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/src/stream.rs
+-rw-r--r--   0     1001      123    95572 2023-04-17 16:17:45.000000 libertem_asi_tpx3-0.2.8/Cargo.lock
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 libertem_asi_tpx3-0.2.8/PKG-INFO
```

### Comparing `libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/Cargo.toml` & `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/Cargo.toml`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/examples/consumer/main.rs` & `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/examples/consumer/main.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/examples/producer/main.rs` & `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/examples/producer/main.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/src/backend_memfd.rs` & `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/backend_memfd.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/src/backend_shm.rs` & `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/backend_shm.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/src/freestack.rs` & `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/freestack.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/src/lib.rs` & `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/local_dependencies/ipc-test/src/slab.rs` & `libertem_asi_tpx3-0.2.8/local_dependencies/ipc-test/src/slab.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/local_dependencies/stats/src/lib.rs` & `libertem_asi_tpx3-0.2.8/local_dependencies/stats/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/Cargo.toml` & `libertem_asi_tpx3-0.2.8/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 name = "libertem-asi-tpx3"
 authors = ["Alexander Clausen <a.clausen@fz-juelich.de>"]
 license = "MIT"
-version = "0.2.7"
+version = "0.2.8"
 edition = "2021"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "libertem_asi_tpx3"
 crate-type = ["cdylib"]
```

### Comparing `libertem_asi_tpx3-0.2.7/examples/acquisition.py` & `libertem_asi_tpx3-0.2.8/examples/acquisition.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/examples/compare.py` & `libertem_asi_tpx3-0.2.8/examples/compare.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/examples/crash.py` & `libertem_asi_tpx3-0.2.8/examples/crash.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/examples/live_client.py` & `libertem_asi_tpx3-0.2.8/examples/live_client.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/examples/live_server.py` & `libertem_asi_tpx3-0.2.8/examples/live_server.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/examples/run_udf.py` & `libertem_asi_tpx3-0.2.8/examples/run_udf.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/examples/sim.py` & `libertem_asi_tpx3-0.2.8/examples/sim.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/examples/simple.py` & `libertem_asi_tpx3-0.2.8/examples/simple.py`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/src/cam_client.rs` & `libertem_asi_tpx3-0.2.8/src/cam_client.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/src/chunk_stack.rs` & `libertem_asi_tpx3-0.2.8/src/chunk_stack.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/src/csr_view.rs` & `libertem_asi_tpx3-0.2.8/src/csr_view.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/src/csr_view_raw.rs` & `libertem_asi_tpx3-0.2.8/src/csr_view_raw.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/src/deserialize.rs` & `libertem_asi_tpx3-0.2.8/src/deserialize.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/src/headers.rs` & `libertem_asi_tpx3-0.2.8/src/headers.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/src/headers_py.rs` & `libertem_asi_tpx3-0.2.8/src/headers_py.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/src/main_py.rs` & `libertem_asi_tpx3-0.2.8/src/main_py.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/src/receiver.rs` & `libertem_asi_tpx3-0.2.8/src/receiver.rs`

 * *Files 3% similar despite different names*

```diff
@@ -123,24 +123,39 @@
             AcquisitionError::StreamError { err } => {
                 write!(f, "stream error: {err:?}")
             }
         }
     }
 }
 
+#[derive(Debug)]
+pub enum ControlError {
+    Cancelled,
+    StateError { msg: String },
+}
+
+impl From<ControlError> for AcquisitionError {
+    fn from(value: ControlError) -> Self {
+        match value {
+            ControlError::Cancelled => AcquisitionError::Cancelled,
+            ControlError::StateError { msg } => AcquisitionError::StateError { msg },
+        }
+    }
+}
+
 /// With a running acquisition, check for control messages;
 /// especially convert `ControlMsg::StopThread` to `AcquisitionError::Cancelled`.
-fn check_for_control(control_channel: &Receiver<ControlMsg>) -> Result<(), AcquisitionError> {
+fn check_for_control(control_channel: &Receiver<ControlMsg>) -> Result<(), ControlError> {
     match control_channel.try_recv() {
-        Ok(ControlMsg::StartAcquisitionPassive) => Err(AcquisitionError::StateError {
+        Ok(ControlMsg::StartAcquisitionPassive) => Err(ControlError::StateError {
             msg: "received StartAcquisitionPassive while an acquisition was already running"
                 .to_string(),
         }),
-        Ok(ControlMsg::StopThread) => Err(AcquisitionError::Cancelled),
-        Err(TryRecvError::Disconnected) => Err(AcquisitionError::Cancelled),
+        Ok(ControlMsg::StopThread) => Err(ControlError::Cancelled),
+        Err(TryRecvError::Disconnected) => Err(ControlError::Cancelled),
         Err(TryRecvError::Empty) => Ok(()),
     }
 }
 
 /// Passively listen for global acquisition and scan headers
 /// and automatically latch on to them.
 fn wait_for_acquisition(
@@ -150,15 +165,19 @@
     frame_stack_size: usize,
     shm: &mut SharedSlabAllocator,
 ) -> Result<(), AcquisitionError> {
     // message headers are always 32 bytes; so we put them on the stack here:
     let mut header_bytes: [u8; 32] = [0; 32];
     loop {
         info!("waiting for acquisition header...");
-        let header = stream_recv_header(stream, &mut header_bytes)?;
+        let header = stream_recv_header(
+            stream,
+            &mut header_bytes,
+            Box::new(|_kind| Ok(check_for_control(control_channel)?)),
+        )?;
 
         trace!("got a header: {header:?}");
 
         match header {
             HeaderTypes::AcquisitionStart { header } => {
                 match wait_for_scan(
                     header,
@@ -207,15 +226,19 @@
     frame_stack_size: usize,
     shm: &mut SharedSlabAllocator,
 ) -> Result<(), AcquisitionError> {
     // message headers are always 32 bytes; so we put them on the stack here:
     let mut header_bytes: [u8; 32] = [0; 32];
     info!("waiting for scan header...");
     loop {
-        let header = stream_recv_header(stream, &mut header_bytes)?;
+        let header = stream_recv_header(
+            stream,
+            &mut header_bytes,
+            Box::new(|_kind| Ok(check_for_control(control_channel)?)),
+        )?;
         trace!("got a header: {header:?}");
 
         match header {
             HeaderTypes::ScanStart { header } => {
                 match handle_scan(
                     acquisition_header.clone(),
                     header,
@@ -303,15 +326,19 @@
     loop {
         if last_control_check.elapsed() > Duration::from_millis(100) {
             last_control_check = Instant::now();
             check_for_control(to_thread_r)?;
         }
 
         let mut header_bytes: [u8; 32] = [0; 32];
-        let header = stream_recv_header(stream, &mut header_bytes)?;
+        let header = stream_recv_header(
+            stream,
+            &mut header_bytes,
+            Box::new(|_kind| Ok(check_for_control(to_thread_r)?)),
+        )?;
 
         match header {
             HeaderTypes::ArrayChunk { header } => {
                 let nbytes = header.get_chunk_size_bytes(&acquisition_header);
 
                 if chunk_stack.total_size() < nbytes {
                     // chunk is too large for the slot size, bail out...
@@ -463,14 +490,19 @@
                 shm,
             ) {
                 Ok(_) => {}
                 Err(AcquisitionError::Disconnected) => {
                     return Ok(()); // the other end of the channel is gone, so :shrug:
                 }
                 Err(AcquisitionError::StreamError { err }) => {
+                    // special case: if the acquisition has been cancelled,
+                    // don't try to reconnect
+                    if let StreamError::ControlError(ControlError::Cancelled) = err {
+                        return Err(AcquisitionError::Cancelled);
+                    }
                     // FIXME: should probably bubble this one up further, as it
                     // may leave buffer contents "undefined"... => clean SHM is best
                     error!("Got a stream error: {err:?} - reconnecting...");
                     break 'inner;
                 }
                 e => {
                     return e; // other error, give up? maybe we can retry instead?
```

### Comparing `libertem_asi_tpx3-0.2.7/src/serialize.rs` & `libertem_asi_tpx3-0.2.8/src/serialize.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/src/sparse_csr.rs` & `libertem_asi_tpx3-0.2.8/src/sparse_csr.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/src/stats.rs` & `libertem_asi_tpx3-0.2.8/src/stats.rs`

 * *Files identical despite different names*

### Comparing `libertem_asi_tpx3-0.2.7/src/stream.rs` & `libertem_asi_tpx3-0.2.8/src/stream.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 use std::{io::Read, net::TcpStream};
 
-use log::trace;
+use log::warn;
 
-use crate::headers::{HeaderTypes, WireFormatError};
+use crate::{
+    headers::{HeaderTypes, WireFormatError},
+    receiver::ControlError,
+};
 
 #[derive(Debug)]
 pub enum StreamError {
     Timeout,
     IoError(std::io::Error),
     FormatError(WireFormatError),
+    ControlError(ControlError),
 }
 
 impl From<std::io::Error> for StreamError {
     fn from(value: std::io::Error) -> Self {
         match value.kind() {
             std::io::ErrorKind::TimedOut => StreamError::Timeout,
             _ => StreamError::IoError(value),
@@ -22,30 +26,36 @@
 
 impl From<WireFormatError> for StreamError {
     fn from(value: WireFormatError) -> Self {
         Self::FormatError(value)
     }
 }
 
+impl From<ControlError> for StreamError {
+    fn from(value: ControlError) -> Self {
+        Self::ControlError(value)
+    }
+}
+
+type RecvCallback<'a> = Box<dyn Fn(&std::io::ErrorKind) -> Result<(), StreamError> + 'a>;
+
 pub fn stream_recv_header(
     stream: &mut TcpStream,
     header_bytes: &mut [u8; 32],
+    timeout_cb: RecvCallback,
 ) -> Result<HeaderTypes, StreamError> {
     // TODO: timeout? can't block indefinitely - can we make this atomic?
-    // TODO: we may have to periodically check for control messages etc.
-    // maybe just use a simple timeout and return `None` here?
-
-    //stream.read_exact(header_bytes)?;
 
     loop {
         match stream.read_exact(header_bytes) {
             Ok(_) => break,
             Err(e) => match e.kind() {
                 std::io::ErrorKind::WouldBlock | std::io::ErrorKind::TimedOut => {
-                    trace!("stream error: {e}");
+                    warn!("stream error: {e}");
+                    timeout_cb(&e.kind())?;
                     continue;
                 }
                 _ => return Err(e.into()),
             },
         }
     }
```

### Comparing `libertem_asi_tpx3-0.2.7/Cargo.lock` & `libertem_asi_tpx3-0.2.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1654,15 +1654,15 @@
 name = "libc"
 version = "0.2.140"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
 
 [[package]]
 name = "libertem-asi-tpx3"
-version = "0.2.7"
+version = "0.2.8"
 dependencies = [
  "bincode",
  "crossbeam",
  "crossbeam-channel",
  "env_logger",
  "ipc-test",
  "log",
@@ -1673,15 +1673,15 @@
  "tempfile",
  "uuid",
  "zerocopy",
 ]
 
 [[package]]
 name = "libertem-dectris"
-version = "0.2.7"
+version = "0.2.8"
 dependencies = [
  "bincode",
  "bs_sys",
  "clap 3.2.23",
  "crossbeam",
  "crossbeam-channel",
  "env_logger",
```

### Comparing `libertem_asi_tpx3-0.2.7/PKG-INFO` & `libertem_asi_tpx3-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libertem-asi-tpx3
-Version: 0.2.7
+Version: 0.2.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Author: Alexander Clausen <a.clausen@fz-juelich.de>
 Author-email: Alexander Clausen <a.clausen@fz-juelich.de>
 License: MIT
 Requires-Python: >=3.7
```

