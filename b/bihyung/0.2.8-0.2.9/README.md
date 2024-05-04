# Comparing `tmp/bihyung-0.2.8.tar.gz` & `tmp/bihyung-0.2.9.tar.gz`

## Comparing `bihyung-0.2.8.tar` & `bihyung-0.2.9.tar`

### file list

```diff
@@ -1,8 +1,25 @@
--rw-r--r--   0        0        0      445 1970-01-01 00:00:00.000000 bihyung-0.2.8/bihyung/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-05-01 03:48:54.000000 bihyung-0.2.8/bihyung/.gitignore
--rw-r--r--   0     1001      127      426 2024-05-01 03:48:54.000000 bihyung-0.2.8/bihyung/langchain_example.py
--rw-r--r--   0     1001      127     4056 2024-05-01 03:48:54.000000 bihyung-0.2.8/bihyung/src/lib.rs
--rw-r--r--   0     1001      127   102173 2024-05-01 03:48:54.000000 bihyung-0.2.8/Cargo.lock
--rw-r--r--   0        0        0      254 1970-01-01 00:00:00.000000 bihyung-0.2.8/Cargo.toml
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 bihyung-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      256 1970-01-01 00:00:00.000000 bihyung-0.2.8/PKG-INFO
+-rw-r--r--   0     1001      127      966 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/Cargo.toml
+-rw-r--r--   0     1001      127      220 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/README.md
+-rw-r--r--   0     1001      127     2984 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/benches/port_open.rs
+-rw-r--r--   0     1001      127     1555 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/examples/langchain_llama.rs
+-rw-r--r--   0     1001      127     1456 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/examples/llamafile_daemon.rs
+-rw-r--r--   0     1001      127     1705 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/src/daemon_trait.rs
+-rw-r--r--   0     1001      127      509 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/src/lib.rs
+-rw-r--r--   0     1001      127     5189 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/src/llama_daemon/daemon3.rs
+-rw-r--r--   0     1001      127     4351 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/src/llama_daemon/llamafile.rs
+-rw-r--r--   0     1001      127     2130 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/src/llama_daemon/mod.rs
+-rw-r--r--   0     1001      127     1085 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/src/mlc_daemon/bootstrap.rs
+-rw-r--r--   0     1001      127     5081 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/src/mlc_daemon/daemon2.rs
+-rw-r--r--   0     1001      127       96 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/src/mlc_daemon/mod.rs
+-rw-r--r--   0     1001      127     8753 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/src/proxy.rs
+-rw-r--r--   0     1001      127     4121 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/src/test_client.rs
+-rw-r--r--   0     1001      127     5971 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/src/util.rs
+-rw-r--r--   0     1001      127       62 2024-05-04 03:06:46.000000 bihyung-0.2.9/llm-daemon/tests/simple_test.rs
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 bihyung-0.2.9/bihyung/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-05-04 03:06:46.000000 bihyung-0.2.9/bihyung/.gitignore
+-rw-r--r--   0     1001      127      426 2024-05-04 03:06:46.000000 bihyung-0.2.9/bihyung/langchain_example.py
+-rw-r--r--   0     1001      127     4769 2024-05-04 03:06:46.000000 bihyung-0.2.9/bihyung/src/lib.rs
+-rw-r--r--   0     1001      127   101767 2024-05-04 03:06:46.000000 bihyung-0.2.9/Cargo.lock
+-rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 bihyung-0.2.9/Cargo.toml
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 bihyung-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      256 1970-01-01 00:00:00.000000 bihyung-0.2.9/PKG-INFO
```

### Comparing `bihyung-0.2.8/bihyung/.gitignore` & `bihyung-0.2.9/bihyung/.gitignore`

 * *Files identical despite different names*

### Comparing `bihyung-0.2.8/bihyung/src/lib.rs` & `bihyung-0.2.9/bihyung/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #![allow(non_local_definitions)]
 
 use llm_daemon::{
-    self, LlamaConfig, LlmConfig as _, LlmDaemon as _, MlcConfig, ProxyConfig,
+    self, llama_config_map, LlamaConfig, LlamaConfigs, LlmConfig as _, LlmDaemon as _, MlcConfig, ProxyConfig
 };
 use pyo3::prelude::*;
 use pyo3_asyncio::tokio::get_runtime;
-use tracing::info;
 
 #[pyclass]
 pub struct Generator {
     inner: llm_daemon::Generator,
 }
 
 #[pymethods]
@@ -34,14 +33,21 @@
             let tmp = fut.await;
             Ok(tmp.expect("failed to get string"))
         })
     }
 }
 
 #[pyclass]
+pub enum Model {
+    Llama3_8b,
+    Phi3_3b,
+    Gemma2b,
+}
+
+#[pyclass]
 pub struct LlamaDaemon {
     inner: llm_daemon::LlamaDaemon,
     endpoint: String,
 }
 
 #[pymethods]
 impl LlamaDaemon {
@@ -52,15 +58,15 @@
         let inner = llm_daemon::LlamaDaemon::new(conf);
 
         Self {
             endpoint: endpoint.to_string(),
             inner,
         }
     }
-
+    
     pub fn fork_daemon(&self) -> PyResult<()> {
         self.inner.fork_daemon().expect("failed to fork daemon");
         Ok(())
     }
 
     pub fn heartbeat(&self) -> PyResult<()> {
         let runtime = get_runtime();
@@ -70,14 +76,30 @@
     }
 
     pub fn endpoint(&self) -> String {
         self.endpoint.clone()
     }
 }
 
+#[pyfunction]
+pub fn daemon_from_model<'a>(model: &'a Model) -> PyResult<LlamaDaemon> {
+    let conf = match model {
+        Model::Llama3_8b => llama_config_map()[&LlamaConfigs::Llama3].clone(),
+        Model::Phi3_3b => llama_config_map()[&LlamaConfigs::Phi3].clone(),
+        Model::Gemma2b => llama_config_map()[&LlamaConfigs::Gemma2b].clone(),
+    };
+    let endpoint = conf.endpoint();
+    let inner = llm_daemon::LlamaDaemon::new(conf);
+
+    Ok(LlamaDaemon {
+        endpoint: endpoint.to_string(),
+        inner,
+    })
+}
+
 #[pyclass]
 pub struct MlcDaemon {
     inner: llm_daemon::MlcDaemon,
     endpoint: String,
 }
 
 #[pymethods]
@@ -157,14 +179,16 @@
     // // TODO: Allow user to change log level, for debugging?
     // let subscriber = tracing_subscriber::FmtSubscriber::builder()
     //     .with_max_level(tracing::Level::WARN)
     //     .finish();
 
     // tracing::subscriber::set_global_default(subscriber)
     //     .expect("failed to config logging");
-    info!("This will be logged to stdout");
+    // info!("This will be logged to stdout");
     m.add_class::<Generator>()?;
     m.add_class::<LlamaDaemon>()?;
     m.add_class::<MlcDaemon>()?;
     m.add_class::<ProxyDaemon>()?;
+    m.add_class::<Model>()?;
+    m.add_function(wrap_pyfunction!(daemon_from_model, m)?)?;
     Ok(())
 }
```

### Comparing `bihyung-0.2.8/Cargo.lock` & `bihyung-0.2.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -58,17 +58,17 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstyle"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "anyhow"
 version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
@@ -95,15 +95,15 @@
 name = "async-openai"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11e97f9c5e0ee3260caee9700ba1bb61a6fdc34d2b6786a31e018c5de5198491"
 dependencies = [
  "async-convert",
  "backoff",
- "base64 0.22.0",
+ "base64 0.22.1",
  "bytes",
  "derive_builder 0.20.0",
  "futures",
  "rand",
  "reqwest 0.12.4",
  "reqwest-eventsource",
  "secrecy",
@@ -170,17 +170,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "axum"
 version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3a6c9af12842a67734c9a2e355436e5d03b22383ed60cf13cd0c18fbfe3dcbcf"
 dependencies = [
@@ -272,24 +272,24 @@
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "base64"
-version = "0.22.0"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
 [[package]]
 name = "bihyung"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "enum_dispatch",
- "llm-daemon 0.2.0",
+ "llm-daemon",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
  "tracing",
  "tracing-subscriber",
  "url",
 ]
@@ -372,17 +372,17 @@
 checksum = "8a17ed5635fc8536268e5d4de1e22e81ac34419e5f052d4d51f4e01dcc263fcc"
 dependencies = [
  "rustversion",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
+checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -955,17 +955,17 @@
  "serde_json",
  "tokenizers",
  "variant_count",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "filetime"
 version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
@@ -973,17 +973,17 @@
  "libc",
  "redox_syscall 0.4.1",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.29"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4556222738635b7a3417ae6130d8f52201e45a0c4d1a907f0826383adb5f85e7"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -1217,17 +1217,17 @@
 dependencies = [
  "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -1590,17 +1590,17 @@
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "langchain-rust"
-version = "4.0.4"
+version = "4.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6458a081ad77de0c579adf8e5a605ec1089193174b76be9b6198a6570f14a52d"
+checksum = "44372931fbc7d664f3338bcabd28916e20aba52c2918b0aec5a65168741ee42a"
 dependencies = [
  "async-openai",
  "async-recursion",
  "async-stream",
  "async-trait",
  "csv",
  "fastembed",
@@ -1633,17 +1633,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libredox"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
@@ -1661,37 +1661,15 @@
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "llm-daemon"
-version = "0.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "929c88315de03d76a11f848ef6a5794fcd72f305e5c14015c0551ac35ce0a190"
-dependencies = [
- "anyhow",
- "axum",
- "daemonize",
- "futures",
- "hyper 1.3.1",
- "hyper-util",
- "reqwest 0.12.4",
- "serde",
- "serde_json",
- "tempfile",
- "tokio",
- "tracing",
- "tracing-subscriber",
- "url",
-]
-
-[[package]]
-name = "llm-daemon"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "anyhow",
  "async-trait",
  "axum",
  "criterion",
  "daemonize",
  "futures",
@@ -2000,17 +1978,17 @@
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -2672,15 +2650,15 @@
 
 [[package]]
 name = "reqwest"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "566cafdd92868e0939d3fb961bd0dc25fcfaaed179291093b3d43e6b3150ea10"
 dependencies = [
- "base64 0.22.0",
+ "base64 0.22.1",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2 0.4.4",
  "http 1.1.0",
  "http-body 1.0.0",
@@ -2815,15 +2793,15 @@
 
 [[package]]
 name = "rustls-pemfile"
 version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
 dependencies = [
- "base64 0.22.0",
+ "base64 0.22.1",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2942,26 +2920,26 @@
  "precomputed-hash",
  "servo_arc",
  "smallvec",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.198"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.198"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
@@ -3060,17 +3038,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
@@ -3669,15 +3647,15 @@
 
 [[package]]
 name = "ureq"
 version = "2.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d11a831e3c0b56e438a28308e7c810799e3c118417f342d30ecec080105395cd"
 dependencies = [
- "base64 0.22.0",
+ "base64 0.22.1",
  "flate2",
  "log",
  "native-tls",
  "once_cell",
  "rustls",
  "rustls-pki-types",
  "rustls-webpki",
```

