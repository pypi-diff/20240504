# Comparing `tmp/teo-0.2.8.tar.gz` & `tmp/teo-0.2.9.tar.gz`

## Comparing `teo-0.2.8.tar` & `teo-0.2.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 teo-0.2.8/Cargo.toml
--rw-r--r--   0     1001      127     3141 2024-02-26 11:23:57.000000 teo-0.2.8/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      704 2024-02-26 11:23:57.000000 teo-0.2.8/.gitignore
--rw-r--r--   0     1001      127     3371 2024-02-26 11:23:57.000000 teo-0.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127    11357 2024-02-26 11:23:57.000000 teo-0.2.8/LICENSE
--rw-r--r--   0     1001      127      263 2024-02-26 11:23:57.000000 teo-0.2.8/README.md
--rw-r--r--   0     1001      127     4453 2024-02-26 11:23:57.000000 teo-0.2.8/src/app/app.rs
--rw-r--r--   0     1001      127       12 2024-02-26 11:23:57.000000 teo-0.2.8/src/app/mod.rs
--rw-r--r--   0     1001      127    46107 2024-02-26 11:23:57.000000 teo-0.2.8/src/dynamic/mod.rs
--rw-r--r--   0     1001      127      216 2024-02-26 11:23:57.000000 teo-0.2.8/src/dynamic/model_ctx_wrapper.rs
--rw-r--r--   0     1001      127      240 2024-02-26 11:23:57.000000 teo-0.2.8/src/dynamic/model_object_wrapper.rs
--rw-r--r--   0     1001      127      234 2024-02-26 11:23:57.000000 teo-0.2.8/src/dynamic/transaction_ctx_wrapper.rs
--rw-r--r--   0     1001      127      719 2024-02-26 11:23:57.000000 teo-0.2.8/src/enum/enum.rs
--rw-r--r--   0     1001      127      766 2024-02-26 11:23:57.000000 teo-0.2.8/src/enum/member/member.rs
--rw-r--r--   0     1001      127       15 2024-02-26 11:23:57.000000 teo-0.2.8/src/enum/member/mod.rs
--rw-r--r--   0     1001      127       31 2024-02-26 11:23:57.000000 teo-0.2.8/src/enum/mod.rs
--rw-r--r--   0     1001      127     1738 2024-02-26 11:23:57.000000 teo-0.2.8/src/handler/group.rs
--rw-r--r--   0     1001      127       14 2024-02-26 11:23:57.000000 teo-0.2.8/src/handler/mod.rs
--rw-r--r--   0     1001      127     3371 2024-02-26 11:23:57.000000 teo-0.2.8/src/lib.rs
--rw-r--r--   0     1001      127      734 2024-02-26 11:23:57.000000 teo-0.2.8/src/model/field/field.rs
--rw-r--r--   0     1001      127       14 2024-02-26 11:23:57.000000 teo-0.2.8/src/model/field/mod.rs
--rw-r--r--   0     1001      127       65 2024-02-26 11:23:57.000000 teo-0.2.8/src/model/mod.rs
--rw-r--r--   0     1001      127      727 2024-02-26 11:23:57.000000 teo-0.2.8/src/model/model.rs
--rw-r--r--   0     1001      127       17 2024-02-26 11:23:57.000000 teo-0.2.8/src/model/property/mod.rs
--rw-r--r--   0     1001      127      758 2024-02-26 11:23:57.000000 teo-0.2.8/src/model/property/property.rs
--rw-r--r--   0     1001      127       17 2024-02-26 11:23:57.000000 teo-0.2.8/src/model/relation/mod.rs
--rw-r--r--   0     1001      127      758 2024-02-26 11:23:57.000000 teo-0.2.8/src/model/relation/relation.rs
--rw-r--r--   0     1001      127       18 2024-02-26 11:23:57.000000 teo-0.2.8/src/namespace/mod.rs
--rw-r--r--   0     1001      127    19345 2024-02-26 11:23:57.000000 teo-0.2.8/src/namespace/namespace.rs
--rw-r--r--   0     1001      127      392 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/arguments.rs
--rw-r--r--   0     1001      127      417 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/array.rs
--rw-r--r--   0     1001      127      466 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/interface_enum_variant.rs
--rw-r--r--   0     1001      127     1379 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/mod.rs
--rw-r--r--   0     1001      127      299 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/model.rs
--rw-r--r--   0     1001      127      357 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/pipeline.rs
--rw-r--r--   0     1001      127      174 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/struct.rs
--rw-r--r--   0     1001      127      394 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/value/decimal.rs
--rw-r--r--   0     1001      127      517 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/value/enum_variant.rs
--rw-r--r--   0     1001      127     1704 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/value/file.rs
--rw-r--r--   0     1001      127     5819 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/value/mod.rs
--rw-r--r--   0     1001      127      604 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/value/object_id.rs
--rw-r--r--   0     1001      127      152 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/value/option_variant.rs
--rw-r--r--   0     1001      127      756 2024-02-26 11:23:57.000000 teo-0.2.8/src/object/value/range.rs
--rw-r--r--   0     1001      127     1175 2024-02-26 11:23:57.000000 teo-0.2.8/src/request/ctx.rs
--rw-r--r--   0     1001      127      758 2024-02-26 11:23:57.000000 teo-0.2.8/src/request/handler_match.rs
--rw-r--r--   0     1001      127      532 2024-02-26 11:23:57.000000 teo-0.2.8/src/request/header_map.rs
--rw-r--r--   0     1001      127      200 2024-02-26 11:23:57.000000 teo-0.2.8/src/request/mod.rs
--rw-r--r--   0     1001      127      718 2024-02-26 11:23:57.000000 teo-0.2.8/src/request/request.rs
--rw-r--r--   0     1001      127      634 2024-02-26 11:23:57.000000 teo-0.2.8/src/response/header_map.rs
--rw-r--r--   0     1001      127     3364 2024-02-26 11:23:57.000000 teo-0.2.8/src/response/mod.rs
--rw-r--r--   0     1001      127     3302 2024-02-26 11:23:57.000000 teo-0.2.8/src/result/mod.rs
--rw-r--r--   0     1001      127     1058 2024-02-26 11:23:57.000000 teo-0.2.8/src/utils/await_coroutine_if_needed.rs
--rw-r--r--   0     1001      127      247 2024-02-26 11:23:57.000000 teo-0.2.8/src/utils/check_callable.rs
--rw-r--r--   0     1001      127      271 2024-02-26 11:23:57.000000 teo-0.2.8/src/utils/check_py_dict.rs
--rw-r--r--   0     1001      127      322 2024-02-26 11:23:57.000000 teo-0.2.8/src/utils/is_coroutine.rs
--rw-r--r--   0     1001      127      128 2024-02-26 11:23:57.000000 teo-0.2.8/src/utils/mod.rs
--rw-r--r--   0     1001      127      451 2024-02-26 11:23:57.000000 teo-0.2.8/src/utils/validate_result.rs
--rw-r--r--   0     1001      127     2124 2024-02-26 11:23:57.000000 teo-0.2.8/teo/__init__.py
--rw-r--r--   0     1001      127    15215 2024-02-26 11:23:57.000000 teo-0.2.8/teo/__init__.pyi
--rw-r--r--   0     1001      127      106 2024-02-26 11:23:57.000000 teo-0.2.8/teo/cli.py
--rw-r--r--   0     1001      127        0 2024-02-26 11:23:57.000000 teo-0.2.8/teo/py.typed
--rw-r--r--   0     1001      127   119995 2024-02-26 11:23:57.000000 teo-0.2.8/Cargo.lock
--rw-r--r--   0     1001      127      350 2024-02-26 11:23:57.000000 teo-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 teo-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 teo-0.2.9/Cargo.toml
+-rw-r--r--   0     1001      127     3141 2024-03-01 10:57:12.000000 teo-0.2.9/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      704 2024-03-01 10:57:12.000000 teo-0.2.9/.gitignore
+-rw-r--r--   0     1001      127     3371 2024-03-01 10:57:12.000000 teo-0.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127    11357 2024-03-01 10:57:12.000000 teo-0.2.9/LICENSE
+-rw-r--r--   0     1001      127      263 2024-03-01 10:57:12.000000 teo-0.2.9/README.md
+-rw-r--r--   0     1001      127     4453 2024-03-01 10:57:12.000000 teo-0.2.9/src/app/app.rs
+-rw-r--r--   0     1001      127       12 2024-03-01 10:57:12.000000 teo-0.2.9/src/app/mod.rs
+-rw-r--r--   0     1001      127    46107 2024-03-01 10:57:12.000000 teo-0.2.9/src/dynamic/mod.rs
+-rw-r--r--   0     1001      127      216 2024-03-01 10:57:12.000000 teo-0.2.9/src/dynamic/model_ctx_wrapper.rs
+-rw-r--r--   0     1001      127      240 2024-03-01 10:57:12.000000 teo-0.2.9/src/dynamic/model_object_wrapper.rs
+-rw-r--r--   0     1001      127      234 2024-03-01 10:57:12.000000 teo-0.2.9/src/dynamic/transaction_ctx_wrapper.rs
+-rw-r--r--   0     1001      127      719 2024-03-01 10:57:12.000000 teo-0.2.9/src/enum/enum.rs
+-rw-r--r--   0     1001      127      766 2024-03-01 10:57:12.000000 teo-0.2.9/src/enum/member/member.rs
+-rw-r--r--   0     1001      127       15 2024-03-01 10:57:12.000000 teo-0.2.9/src/enum/member/mod.rs
+-rw-r--r--   0     1001      127       31 2024-03-01 10:57:12.000000 teo-0.2.9/src/enum/mod.rs
+-rw-r--r--   0     1001      127     1738 2024-03-01 10:57:12.000000 teo-0.2.9/src/handler/group.rs
+-rw-r--r--   0     1001      127       14 2024-03-01 10:57:12.000000 teo-0.2.9/src/handler/mod.rs
+-rw-r--r--   0     1001      127     3371 2024-03-01 10:57:12.000000 teo-0.2.9/src/lib.rs
+-rw-r--r--   0     1001      127      734 2024-03-01 10:57:12.000000 teo-0.2.9/src/model/field/field.rs
+-rw-r--r--   0     1001      127       14 2024-03-01 10:57:12.000000 teo-0.2.9/src/model/field/mod.rs
+-rw-r--r--   0     1001      127       65 2024-03-01 10:57:12.000000 teo-0.2.9/src/model/mod.rs
+-rw-r--r--   0     1001      127      727 2024-03-01 10:57:12.000000 teo-0.2.9/src/model/model.rs
+-rw-r--r--   0     1001      127       17 2024-03-01 10:57:12.000000 teo-0.2.9/src/model/property/mod.rs
+-rw-r--r--   0     1001      127      758 2024-03-01 10:57:12.000000 teo-0.2.9/src/model/property/property.rs
+-rw-r--r--   0     1001      127       17 2024-03-01 10:57:12.000000 teo-0.2.9/src/model/relation/mod.rs
+-rw-r--r--   0     1001      127      758 2024-03-01 10:57:12.000000 teo-0.2.9/src/model/relation/relation.rs
+-rw-r--r--   0     1001      127       18 2024-03-01 10:57:12.000000 teo-0.2.9/src/namespace/mod.rs
+-rw-r--r--   0     1001      127    19345 2024-03-01 10:57:12.000000 teo-0.2.9/src/namespace/namespace.rs
+-rw-r--r--   0     1001      127      392 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/arguments.rs
+-rw-r--r--   0     1001      127      417 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/array.rs
+-rw-r--r--   0     1001      127      466 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/interface_enum_variant.rs
+-rw-r--r--   0     1001      127     1379 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/mod.rs
+-rw-r--r--   0     1001      127      299 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/model.rs
+-rw-r--r--   0     1001      127      357 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/pipeline.rs
+-rw-r--r--   0     1001      127      174 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/struct.rs
+-rw-r--r--   0     1001      127      394 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/value/decimal.rs
+-rw-r--r--   0     1001      127      517 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/value/enum_variant.rs
+-rw-r--r--   0     1001      127     1704 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/value/file.rs
+-rw-r--r--   0     1001      127     5819 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/value/mod.rs
+-rw-r--r--   0     1001      127      604 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/value/object_id.rs
+-rw-r--r--   0     1001      127      152 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/value/option_variant.rs
+-rw-r--r--   0     1001      127      756 2024-03-01 10:57:12.000000 teo-0.2.9/src/object/value/range.rs
+-rw-r--r--   0     1001      127     1175 2024-03-01 10:57:12.000000 teo-0.2.9/src/request/ctx.rs
+-rw-r--r--   0     1001      127      758 2024-03-01 10:57:12.000000 teo-0.2.9/src/request/handler_match.rs
+-rw-r--r--   0     1001      127      532 2024-03-01 10:57:12.000000 teo-0.2.9/src/request/header_map.rs
+-rw-r--r--   0     1001      127      200 2024-03-01 10:57:12.000000 teo-0.2.9/src/request/mod.rs
+-rw-r--r--   0     1001      127      718 2024-03-01 10:57:12.000000 teo-0.2.9/src/request/request.rs
+-rw-r--r--   0     1001      127      634 2024-03-01 10:57:12.000000 teo-0.2.9/src/response/header_map.rs
+-rw-r--r--   0     1001      127     3364 2024-03-01 10:57:12.000000 teo-0.2.9/src/response/mod.rs
+-rw-r--r--   0     1001      127     3302 2024-03-01 10:57:12.000000 teo-0.2.9/src/result/mod.rs
+-rw-r--r--   0     1001      127     1058 2024-03-01 10:57:12.000000 teo-0.2.9/src/utils/await_coroutine_if_needed.rs
+-rw-r--r--   0     1001      127      247 2024-03-01 10:57:12.000000 teo-0.2.9/src/utils/check_callable.rs
+-rw-r--r--   0     1001      127      271 2024-03-01 10:57:12.000000 teo-0.2.9/src/utils/check_py_dict.rs
+-rw-r--r--   0     1001      127      322 2024-03-01 10:57:12.000000 teo-0.2.9/src/utils/is_coroutine.rs
+-rw-r--r--   0     1001      127      128 2024-03-01 10:57:12.000000 teo-0.2.9/src/utils/mod.rs
+-rw-r--r--   0     1001      127      451 2024-03-01 10:57:12.000000 teo-0.2.9/src/utils/validate_result.rs
+-rw-r--r--   0     1001      127     2124 2024-03-01 10:57:12.000000 teo-0.2.9/teo/__init__.py
+-rw-r--r--   0     1001      127    15215 2024-03-01 10:57:12.000000 teo-0.2.9/teo/__init__.pyi
+-rw-r--r--   0     1001      127      106 2024-03-01 10:57:12.000000 teo-0.2.9/teo/cli.py
+-rw-r--r--   0     1001      127        0 2024-03-01 10:57:12.000000 teo-0.2.9/teo/py.typed
+-rw-r--r--   0     1001      127   119995 2024-03-01 10:57:12.000000 teo-0.2.9/Cargo.lock
+-rw-r--r--   0     1001      127      350 2024-03-01 10:57:12.000000 teo-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 teo-0.2.9/PKG-INFO
```

### Comparing `teo-0.2.8/Cargo.toml` & `teo-0.2.9/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [package]
 name = "teo-py"
-version = "0.2.8"
+version = "0.2.9"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "teo"
 crate-type = ["cdylib"]
 
 [dependencies]
-teo = { version = "0.2.8" }
+teo = { version = "0.2.9" }
 pyo3 = { version = "0.20.2", features = ["extension-module", "chrono", "indexmap"] }
 pyo3-asyncio = { version = "0.20.0", features = ["attributes", "tokio-runtime"] }
 tokio = { version = "1.0" }
 bson = { version = "2.7.0", features = ["chrono-0_4", "serde_with"] }
 bigdecimal = "=0.3.1"
 chrono = { version = "0.4.24" }
 indexmap = "2.1.0"
```

### Comparing `teo-0.2.8/.github/workflows/CI.yml` & `teo-0.2.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/.gitignore` & `teo-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/CODE_OF_CONDUCT.md` & `teo-0.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/LICENSE` & `teo-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/app/app.rs` & `teo-0.2.9/src/app/app.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/dynamic/mod.rs` & `teo-0.2.9/src/dynamic/mod.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/enum/enum.rs` & `teo-0.2.9/src/enum/enum.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/enum/member/member.rs` & `teo-0.2.9/src/enum/member/member.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/handler/group.rs` & `teo-0.2.9/src/handler/group.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/lib.rs` & `teo-0.2.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/model/field/field.rs` & `teo-0.2.9/src/model/field/field.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/model/model.rs` & `teo-0.2.9/src/model/model.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/model/property/property.rs` & `teo-0.2.9/src/model/property/property.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/model/relation/relation.rs` & `teo-0.2.9/src/model/relation/relation.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/namespace/namespace.rs` & `teo-0.2.9/src/namespace/namespace.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/object/mod.rs` & `teo-0.2.9/src/object/mod.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/object/value/enum_variant.rs` & `teo-0.2.9/src/object/value/enum_variant.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/object/value/file.rs` & `teo-0.2.9/src/object/value/file.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/object/value/mod.rs` & `teo-0.2.9/src/object/value/mod.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/object/value/object_id.rs` & `teo-0.2.9/src/object/value/object_id.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/object/value/range.rs` & `teo-0.2.9/src/object/value/range.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/request/ctx.rs` & `teo-0.2.9/src/request/ctx.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/request/handler_match.rs` & `teo-0.2.9/src/request/handler_match.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/request/header_map.rs` & `teo-0.2.9/src/request/header_map.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/request/request.rs` & `teo-0.2.9/src/request/request.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/response/header_map.rs` & `teo-0.2.9/src/response/header_map.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/response/mod.rs` & `teo-0.2.9/src/response/mod.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/result/mod.rs` & `teo-0.2.9/src/result/mod.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/src/utils/await_coroutine_if_needed.rs` & `teo-0.2.9/src/utils/await_coroutine_if_needed.rs`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/teo/__init__.py` & `teo-0.2.9/teo/__init__.py`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/teo/__init__.pyi` & `teo-0.2.9/teo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `teo-0.2.8/Cargo.lock` & `teo-0.2.9/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -3792,17 +3792,17 @@
  "redox_syscall",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "teo"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "723ed8a469b186500863aee0d07cbaf6c1b594c3c36a27f7f506d93981863df5"
+checksum = "3ceb338bd8a0e0a39993922403dc878d68519a9c2ed6dc5c21a0fdffced2f8c9"
 dependencies = [
  "actix-files",
  "actix-http",
  "actix-multipart",
  "actix-web",
  "array_tool",
  "async-recursion",
@@ -3845,17 +3845,17 @@
  "tokio",
  "url",
  "uuid",
 ]
 
 [[package]]
 name = "teo-generator"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fba4b166865478a84b6d3ffba6e9024efe2815bfbfe229413328b4b14802ae93"
+checksum = "c9353be0e8b5e17df878c82dd0d61848884c8e1b3771a1165f93606f28d46652"
 dependencies = [
  "askama",
  "async-recursion",
  "async-trait",
  "colored",
  "indent",
  "indexmap 2.2.3",
@@ -3871,17 +3871,17 @@
  "teo-runtime",
  "tokio",
  "toml_edit 0.22.5",
 ]
 
 [[package]]
 name = "teo-mongodb-connector"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce8f744490cad99884ce003c8f2e6fbcfe1fb605972e91b062894c368885076d"
+checksum = "75c9c838c66a29255431c8a5939a22cd0bae8f20798e1b657cfa8a5ce4d432c4"
 dependencies = [
  "async-recursion",
  "async-trait",
  "bigdecimal",
  "bson",
  "chrono",
  "futures-util",
@@ -3897,17 +3897,17 @@
  "teo-runtime",
  "teo-teon",
  "tokio",
 ]
 
 [[package]]
 name = "teo-parser"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89386277b9efaa2a9933b4f98d582d6a2022138f20c409ca3ff0f943c6c96e6b"
+checksum = "1319bbc4859d799ebcd74d3bf23e87d6af74e739b4f9594ac842c019212efd77"
 dependencies = [
  "array_tool",
  "colored",
  "educe",
  "indexmap 2.2.3",
  "itertools 0.12.1",
  "maplit",
@@ -3923,15 +3923,15 @@
  "strum",
  "strum_macros",
  "teo-teon",
 ]
 
 [[package]]
 name = "teo-py"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "bigdecimal",
  "bson",
  "chrono",
  "indexmap 2.2.3",
  "inflector-plus",
  "pyo3",
@@ -3948,17 +3948,17 @@
 checksum = "f8d61a0d23770dd302816a52c40c3193a810227e5c8bcb81a93172ceb242834f"
 dependencies = [
  "indexmap 2.2.3",
 ]
 
 [[package]]
 name = "teo-runtime"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87b2ede839a3b599db5f7df2274aed8b24b9ea5ecd5d40735cf50306c5b6d64f"
+checksum = "0acba78e61011c5fd83c2b5c7536d9c1fdb476faf2e245fe0c4d04d882799389"
 dependencies = [
  "async-recursion",
  "async-trait",
  "bigdecimal",
  "bson",
  "chrono",
  "cuid",
@@ -3986,17 +3986,17 @@
  "teo-teon",
  "tokio",
  "uuid",
 ]
 
 [[package]]
 name = "teo-sql-connector"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb20459867976d5b1980f26e7abcdfb8193348354cef7ad7bc688130d40e02a1"
+checksum = "edae9d31c2f53740d1788c268ac26f56dcd04bb685ae3a7664ee084db9e53c11"
 dependencies = [
  "array_tool",
  "async-recursion",
  "async-trait",
  "bigdecimal",
  "chrono",
  "indexmap 2.2.3",
```

### Comparing `teo-0.2.8/PKG-INFO` & `teo-0.2.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teo
-Version: 0.2.8
+Version: 0.2.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

