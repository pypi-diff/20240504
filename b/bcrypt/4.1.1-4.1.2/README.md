# Comparing `tmp/bcrypt-4.1.1.tar.gz` & `tmp/bcrypt-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcrypt-4.1.1.tar", last modified: Tue Nov 28 15:37:30 2023, max compression
+gzip compressed data, was "bcrypt-4.1.2.tar", last modified: Fri Dec 15 14:39:20 2023, max compression
```

## Comparing `bcrypt-4.1.1.tar` & `bcrypt-4.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 15:37:30.782041 bcrypt-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-11-28 15:37:20.000000 bcrypt-4.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2023-11-28 15:37:20.000000 bcrypt-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-11-28 15:37:20.000000 bcrypt-4.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2023-11-28 15:37:30.782041 bcrypt-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2023-11-28 15:37:20.000000 bcrypt-4.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-11-28 15:37:20.000000 bcrypt-4.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 15:37:30.782041 bcrypt-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2023-11-28 15:37:20.000000 bcrypt-4.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 15:37:30.778041 bcrypt-4.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 15:37:30.778041 bcrypt-4.1.1/src/_bcrypt/
--rw-r--r--   0 runner    (1001) docker     (127)    12186 2023-11-28 15:37:20.000000 bcrypt-4.1.1/src/_bcrypt/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-11-28 15:37:20.000000 bcrypt-4.1.1/src/_bcrypt/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 15:37:30.778041 bcrypt-4.1.1/src/_bcrypt/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2023-11-28 15:37:20.000000 bcrypt-4.1.1/src/_bcrypt/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 15:37:30.782041 bcrypt-4.1.1/src/bcrypt/
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-11-28 15:37:20.000000 bcrypt-4.1.1/src/bcrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-11-28 15:37:20.000000 bcrypt-4.1.1/src/bcrypt/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 15:37:20.000000 bcrypt-4.1.1/src/bcrypt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 15:37:30.782041 bcrypt-4.1.1/src/bcrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2023-11-28 15:37:30.000000 bcrypt-4.1.1/src/bcrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-11-28 15:37:30.000000 bcrypt-4.1.1/src/bcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 15:37:30.000000 bcrypt-4.1.1/src/bcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 15:37:30.000000 bcrypt-4.1.1/src/bcrypt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-28 15:37:30.000000 bcrypt-4.1.1/src/bcrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-28 15:37:30.000000 bcrypt-4.1.1/src/bcrypt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 15:37:30.782041 bcrypt-4.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    16646 2023-11-28 15:37:20.000000 bcrypt-4.1.1/tests/test_bcrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-11-28 15:37:20.000000 bcrypt-4.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:39:20.192423 bcrypt-4.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-15 14:39:10.000000 bcrypt-4.1.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2023-12-15 14:39:10.000000 bcrypt-4.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2023-12-15 14:39:10.000000 bcrypt-4.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9472 2023-12-15 14:39:20.192423 bcrypt-4.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2023-12-15 14:39:10.000000 bcrypt-4.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-12-15 14:39:10.000000 bcrypt-4.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-15 14:39:20.192423 bcrypt-4.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2023-12-15 14:39:10.000000 bcrypt-4.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:39:20.188423 bcrypt-4.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:39:20.188423 bcrypt-4.1.2/src/_bcrypt/
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2023-12-15 14:39:10.000000 bcrypt-4.1.2/src/_bcrypt/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-15 14:39:10.000000 bcrypt-4.1.2/src/_bcrypt/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:39:20.188423 bcrypt-4.1.2/src/_bcrypt/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2023-12-15 14:39:10.000000 bcrypt-4.1.2/src/_bcrypt/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:39:20.188423 bcrypt-4.1.2/src/bcrypt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-12-15 14:39:10.000000 bcrypt-4.1.2/src/bcrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-15 14:39:10.000000 bcrypt-4.1.2/src/bcrypt/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:39:10.000000 bcrypt-4.1.2/src/bcrypt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:39:20.192423 bcrypt-4.1.2/src/bcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9472 2023-12-15 14:39:20.000000 bcrypt-4.1.2/src/bcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2023-12-15 14:39:20.000000 bcrypt-4.1.2/src/bcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 14:39:20.000000 bcrypt-4.1.2/src/bcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 14:39:19.000000 bcrypt-4.1.2/src/bcrypt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-15 14:39:20.000000 bcrypt-4.1.2/src/bcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-15 14:39:20.000000 bcrypt-4.1.2/src/bcrypt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:39:20.192423 bcrypt-4.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    16646 2023-12-15 14:39:10.000000 bcrypt-4.1.2/tests/test_bcrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-15 14:39:10.000000 bcrypt-4.1.2/tox.ini
```

### Comparing `bcrypt-4.1.1/LICENSE` & `bcrypt-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bcrypt-4.1.1/PKG-INFO` & `bcrypt-4.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcrypt
-Version: 4.1.1
+Version: 4.1.2
 Summary: Modern password hashing for your software and your servers
 Author-email: The Python Cryptographic Authority developers <cryptography-dev@python.org>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/pyca/bcrypt/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -74,18 +74,26 @@
 ============
 
 While bcrypt remains an acceptable choice for password storage, depending on your specific use case you may also want to consider using scrypt (either via `standard library`_ or `cryptography`_) or argon2id via `argon2_cffi`_.
 
 Changelog
 =========
 
+4.1.2
+-----
+
+* Publish both ``py37`` and ``py39`` wheels. This should resolve some errors
+  relating to initializing a module multiple times per process.
+
 4.1.1
 -----
 
 * Fixed the type signature on the ``kdf`` method.
+* Fixed packaging bug on Windows.
+* Fixed incompatibility with passlib package detection assumptions.
 
 4.1.0
 -----
 
 * Dropped support for Python 3.6.
 * Bumped MSRV to 1.64. (Note: Rust 1.63 can be used by setting the ``BCRYPT_ALLOW_RUST_163`` environment variable)
```

### Comparing `bcrypt-4.1.1/README.rst` & `bcrypt-4.1.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,26 @@
 ============
 
 While bcrypt remains an acceptable choice for password storage, depending on your specific use case you may also want to consider using scrypt (either via `standard library`_ or `cryptography`_) or argon2id via `argon2_cffi`_.
 
 Changelog
 =========
 
+4.1.2
+-----
+
+* Publish both ``py37`` and ``py39`` wheels. This should resolve some errors
+  relating to initializing a module multiple times per process.
+
 4.1.1
 -----
 
 * Fixed the type signature on the ``kdf`` method.
+* Fixed packaging bug on Windows.
+* Fixed incompatibility with passlib package detection assumptions.
 
 4.1.0
 -----
 
 * Dropped support for Python 3.6.
 * Bumped MSRV to 1.64. (Note: Rust 1.63 can be used by setting the ``BCRYPT_ALLOW_RUST_163`` environment variable)
```

### Comparing `bcrypt-4.1.1/pyproject.toml` & `bcrypt-4.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Point to the setuptools' PEP517 build backend explicitly to
 # disable Pip's fallback guessing
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bcrypt"
 # When updating this, also update lib.rs
-version = "4.1.1"
+version = "4.1.2"
 authors = [
     {name = "The Python Cryptographic Authority developers", email = "cryptography-dev@python.org"}
 ]
 description = "Modern password hashing for your software and your servers"
 license = {text = "Apache-2.0"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `bcrypt-4.1.1/setup.py` & `bcrypt-4.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 try:
     setup(
         rust_extensions=[
             RustExtension(
                 "bcrypt._bcrypt",
                 "src/_bcrypt/Cargo.toml",
-                py_limited_api=True,
+                py_limited_api="auto",
                 rust_version=(
                     ">=1.64.0"
                     if os.environ.get("BCRYPT_ALLOW_RUST_163", "0") != "0"
                     else ">=1.63.0"
                 ),
             ),
         ],
```

### Comparing `bcrypt-4.1.1/src/_bcrypt/Cargo.lock` & `bcrypt-4.1.2/src/_bcrypt/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -167,17 +167,17 @@
 checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.150"
+version = "0.2.151"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d92a4743f9a61002fae18374ed11e7973f530cb3a3255fb354818118b2203c"
+checksum = "302d7ab3130588088d277783b1e2d2e10c9e9e4a16dd9050e6ec93fb3e7048f4"
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
@@ -192,17 +192,17 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -347,17 +347,17 @@
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
-version = "2.0.39"
+version = "2.0.41"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23e78b90f2fcf45d3e842032ce32e3f2d1545ba6636271dcbf24fa306d87be7a"
+checksum = "44c8b28c477cc3bf0e7966561e3460130e1255f7a1cf71931075f1c5e7a7e269"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `bcrypt-4.1.1/src/_bcrypt/src/lib.rs` & `bcrypt-4.1.2/src/_bcrypt/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     m.add("__title__", "bcrypt")?;
     m.add("__summary__", "Modern(-ish) password hashing for your software and your servers")?;
     m.add("__uri__", "https://github.com/pyca/bcrypt/")?;
 
     // When updating this, also update pyproject.toml
     // This isn't named __version__ because passlib treats the existence of
     // that attribute as proof that we're a different module
-    m.add("__version_ex__", "4.1.1")?;
+    m.add("__version_ex__", "4.1.2")?;
 
     let author = "The Python Cryptographic Authority developers";
     m.add("__author__", author)?;
     m.add("__email__", "cryptography-dev@python.org")?;
 
     m.add("__license__", "Apache License, Version 2.0")?;
     m.add("__copyright__", format!("Copyright 2013-2023 {author}"))?;
```

### Comparing `bcrypt-4.1.1/src/bcrypt/__init__.py` & `bcrypt-4.1.2/src/bcrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `bcrypt-4.1.1/src/bcrypt.egg-info/PKG-INFO` & `bcrypt-4.1.2/src/bcrypt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcrypt
-Version: 4.1.1
+Version: 4.1.2
 Summary: Modern password hashing for your software and your servers
 Author-email: The Python Cryptographic Authority developers <cryptography-dev@python.org>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/pyca/bcrypt/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -74,18 +74,26 @@
 ============
 
 While bcrypt remains an acceptable choice for password storage, depending on your specific use case you may also want to consider using scrypt (either via `standard library`_ or `cryptography`_) or argon2id via `argon2_cffi`_.
 
 Changelog
 =========
 
+4.1.2
+-----
+
+* Publish both ``py37`` and ``py39`` wheels. This should resolve some errors
+  relating to initializing a module multiple times per process.
+
 4.1.1
 -----
 
 * Fixed the type signature on the ``kdf`` method.
+* Fixed packaging bug on Windows.
+* Fixed incompatibility with passlib package detection assumptions.
 
 4.1.0
 -----
 
 * Dropped support for Python 3.6.
 * Bumped MSRV to 1.64. (Note: Rust 1.63 can be used by setting the ``BCRYPT_ALLOW_RUST_163`` environment variable)
```

### Comparing `bcrypt-4.1.1/tests/test_bcrypt.py` & `bcrypt-4.1.2/tests/test_bcrypt.py`

 * *Files identical despite different names*

### Comparing `bcrypt-4.1.1/tox.ini` & `bcrypt-4.1.2/tox.ini`

 * *Files identical despite different names*

