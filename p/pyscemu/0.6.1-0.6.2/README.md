# Comparing `tmp/pyscemu-0.6.1.tar.gz` & `tmp/pyscemu-0.6.2.tar.gz`

## Comparing `pyscemu-0.6.1.tar` & `pyscemu-0.6.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.6.1/Cargo.toml
--rw-r--r--   0     1000     1000      692 2024-01-16 17:48:02.000000 pyscemu-0.6.1/.gitignore
--rw-r--r--   0     1000     1000    12030 2024-01-16 17:46:26.000000 pyscemu-0.6.1/DOCUMENTATION.md
--rw-r--r--   0     1000     1000    10154 2024-01-16 17:48:02.000000 pyscemu-0.6.1/README.md
--rw-r--r--   0     1000     1000     2017 2024-01-16 17:46:26.000000 pyscemu-0.6.1/examples/danabot_rsa.ipynb
--rw-r--r--   0     1000     1000     6831 2024-01-16 17:46:26.000000 pyscemu-0.6.1/examples/raccoon_strings.ipynb
--rw-r--r--   0     1000     1000        0 2024-01-16 17:46:26.000000 pyscemu-0.6.1/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
--rw-r--r--   0     1000     1000     1110 2024-01-24 15:06:32.000000 pyscemu-0.6.1/examples/scripts/api_implementation.py
--rw-r--r--   0     1000     1000      597 2024-01-24 15:06:32.000000 pyscemu-0.6.1/examples/scripts/danabot_crypto.py
--rw-r--r--   0     1000     1000      861 2024-01-24 15:06:32.000000 pyscemu-0.6.1/examples/scripts/danabot_extract.py
--rw-r--r--   0     1000     1000      534 2024-01-24 15:06:32.000000 pyscemu-0.6.1/examples/scripts/danabot_get_string_emu.py
--rw-r--r--   0     1000     1000      292 2024-01-24 15:06:32.000000 pyscemu-0.6.1/examples/scripts/danabot_int_deobfus_emu.py
--rw-r--r--   0     1000     1000      541 2024-01-24 15:06:32.000000 pyscemu-0.6.1/examples/scripts/emu_pwer.py
--rw-r--r--   0     1000     1000     1344 2024-01-24 15:08:08.000000 pyscemu-0.6.1/examples/scripts/gozi_decryptbss_emu.py
--rw-r--r--   0     1000     1000      404 2024-01-24 15:09:58.000000 pyscemu-0.6.1/examples/scripts/gozi_dga.py
--rw-r--r--   0     1000     1000      706 2024-01-24 15:09:01.000000 pyscemu-0.6.1/examples/scripts/raccoon_strings.py
--rw-r--r--   0     1000     1000      733 2024-01-24 15:06:32.000000 pyscemu-0.6.1/examples/scripts/ssl_key128_gen.py
--rw-r--r--   0     1000     1000      701 2024-01-24 15:08:32.000000 pyscemu-0.6.1/examples/scripts/test.py
--rw-r--r--   0     1000     1000      523 2024-01-24 15:06:32.000000 pyscemu-0.6.1/examples/scripts/vidar_strings.py
--rw-r--r--   0     1000     1000      273 2024-01-24 15:06:32.000000 pyscemu-0.6.1/examples/scripts/vidar_strings2.py
--rw-r--r--   0     1000     1000      522 2024-01-24 15:06:32.000000 pyscemu-0.6.1/examples/scripts/xloader_dexor.py
--rw-r--r--   0     1000     1000      443 2024-01-24 15:06:32.000000 pyscemu-0.6.1/examples/scripts/xloader_keygen.py
--rw-r--r--   0     1000     1000     1757 2024-01-16 17:46:26.000000 pyscemu-0.6.1/examples/xloader_keygen.ipynb
--rw-r--r--   0     1000     1000    27179 2024-03-27 19:08:18.000000 pyscemu-0.6.1/src/lib.rs
--rw-r--r--   0     1000     1000    23209 2024-04-19 08:59:42.000000 pyscemu-0.6.1/Cargo.lock
--rw-r--r--   0     1000     1000      433 2024-01-16 17:46:26.000000 pyscemu-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    10480 1970-01-01 00:00:00.000000 pyscemu-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.6.2/Cargo.toml
+-rw-r--r--   0     1000     1000      692 2024-01-16 17:48:02.000000 pyscemu-0.6.2/.gitignore
+-rw-r--r--   0     1000     1000    12030 2024-01-16 17:46:26.000000 pyscemu-0.6.2/DOCUMENTATION.md
+-rw-r--r--   0     1000     1000    10154 2024-01-16 17:48:02.000000 pyscemu-0.6.2/README.md
+-rw-r--r--   0     1000     1000     2017 2024-01-16 17:46:26.000000 pyscemu-0.6.2/examples/danabot_rsa.ipynb
+-rw-r--r--   0     1000     1000     6831 2024-01-16 17:46:26.000000 pyscemu-0.6.2/examples/raccoon_strings.ipynb
+-rw-r--r--   0     1000     1000        0 2024-01-16 17:46:26.000000 pyscemu-0.6.2/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
+-rw-r--r--   0     1000     1000     1110 2024-01-24 15:06:32.000000 pyscemu-0.6.2/examples/scripts/api_implementation.py
+-rw-r--r--   0     1000     1000      597 2024-01-24 15:06:32.000000 pyscemu-0.6.2/examples/scripts/danabot_crypto.py
+-rw-r--r--   0     1000     1000      861 2024-01-24 15:06:32.000000 pyscemu-0.6.2/examples/scripts/danabot_extract.py
+-rw-r--r--   0     1000     1000      534 2024-01-24 15:06:32.000000 pyscemu-0.6.2/examples/scripts/danabot_get_string_emu.py
+-rw-r--r--   0     1000     1000      292 2024-01-24 15:06:32.000000 pyscemu-0.6.2/examples/scripts/danabot_int_deobfus_emu.py
+-rw-r--r--   0     1000     1000      541 2024-01-24 15:06:32.000000 pyscemu-0.6.2/examples/scripts/emu_pwer.py
+-rw-r--r--   0     1000     1000     1344 2024-01-24 15:08:08.000000 pyscemu-0.6.2/examples/scripts/gozi_decryptbss_emu.py
+-rw-r--r--   0     1000     1000      404 2024-01-24 15:09:58.000000 pyscemu-0.6.2/examples/scripts/gozi_dga.py
+-rw-r--r--   0     1000     1000      706 2024-01-24 15:09:01.000000 pyscemu-0.6.2/examples/scripts/raccoon_strings.py
+-rw-r--r--   0     1000     1000      733 2024-01-24 15:06:32.000000 pyscemu-0.6.2/examples/scripts/ssl_key128_gen.py
+-rw-r--r--   0     1000     1000      701 2024-01-24 15:08:32.000000 pyscemu-0.6.2/examples/scripts/test.py
+-rw-r--r--   0     1000     1000      523 2024-01-24 15:06:32.000000 pyscemu-0.6.2/examples/scripts/vidar_strings.py
+-rw-r--r--   0     1000     1000      273 2024-01-24 15:06:32.000000 pyscemu-0.6.2/examples/scripts/vidar_strings2.py
+-rw-r--r--   0     1000     1000      522 2024-01-24 15:06:32.000000 pyscemu-0.6.2/examples/scripts/xloader_dexor.py
+-rw-r--r--   0     1000     1000      443 2024-01-24 15:06:32.000000 pyscemu-0.6.2/examples/scripts/xloader_keygen.py
+-rw-r--r--   0     1000     1000     1757 2024-01-16 17:46:26.000000 pyscemu-0.6.2/examples/xloader_keygen.ipynb
+-rw-r--r--   0     1000     1000    27179 2024-03-27 19:08:18.000000 pyscemu-0.6.2/src/lib.rs
+-rw-r--r--   0     1000     1000    23209 2024-05-04 17:32:07.000000 pyscemu-0.6.2/Cargo.lock
+-rw-r--r--   0     1000     1000      433 2024-01-16 17:46:26.000000 pyscemu-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    10480 1970-01-01 00:00:00.000000 pyscemu-0.6.2/PKG-INFO
```

### Comparing `pyscemu-0.6.1/.gitignore` & `pyscemu-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/DOCUMENTATION.md` & `pyscemu-0.6.2/DOCUMENTATION.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/README.md` & `pyscemu-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/danabot_rsa.ipynb` & `pyscemu-0.6.2/examples/danabot_rsa.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/raccoon_strings.ipynb` & `pyscemu-0.6.2/examples/raccoon_strings.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/scripts/api_implementation.py` & `pyscemu-0.6.2/examples/scripts/api_implementation.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/scripts/danabot_crypto.py` & `pyscemu-0.6.2/examples/scripts/danabot_crypto.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/scripts/danabot_extract.py` & `pyscemu-0.6.2/examples/scripts/danabot_extract.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/scripts/danabot_get_string_emu.py` & `pyscemu-0.6.2/examples/scripts/danabot_get_string_emu.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/scripts/emu_pwer.py` & `pyscemu-0.6.2/examples/scripts/emu_pwer.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/scripts/gozi_decryptbss_emu.py` & `pyscemu-0.6.2/examples/scripts/gozi_decryptbss_emu.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/scripts/raccoon_strings.py` & `pyscemu-0.6.2/examples/scripts/raccoon_strings.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/scripts/ssl_key128_gen.py` & `pyscemu-0.6.2/examples/scripts/ssl_key128_gen.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/scripts/test.py` & `pyscemu-0.6.2/examples/scripts/test.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/scripts/vidar_strings.py` & `pyscemu-0.6.2/examples/scripts/vidar_strings.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/scripts/xloader_dexor.py` & `pyscemu-0.6.2/examples/scripts/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/examples/xloader_keygen.ipynb` & `pyscemu-0.6.2/examples/xloader_keygen.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/src/lib.rs` & `pyscemu-0.6.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyscemu-0.6.1/Cargo.lock` & `pyscemu-0.6.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -243,17 +243,17 @@
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libscemu"
-version = "0.16.1"
+version = "0.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6886b6e9f8facf4945d4a0b1c6e011072df2816f0f26e3b2a1526eb71515774"
+checksum = "2b457912abab0fec8f4045397b4ee014c1cf4f9d54fabf27a64a011f774af0f1"
 dependencies = [
  "atty",
  "chrono",
  "ctrlc",
  "iced-x86",
  "lazy_static",
  "md5",
@@ -444,15 +444,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.6.1"
+version = "0.6.2"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyscemu-0.6.1/PKG-INFO` & `pyscemu-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.6.1
+Version: 0.6.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
```

