# Comparing `tmp/algomodule-1.0.4.tar.gz` & `tmp/algomodule-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algomodule-1.0.4.tar", last modified: Sat May  4 11:13:23 2024, max compression
+gzip compressed data, was "algomodule-1.1.0.tar", last modified: Sat May  4 21:00:22 2024, max compression
```

## Comparing `algomodule-1.0.4.tar` & `algomodule-1.1.0.tar`

### file list

```diff
@@ -1,141 +1,153 @@
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.558112 algomodule-1.0.4/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)        6 2024-04-30 21:30:57.000000 algomodule-1.0.4/.gitignore
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      115 2024-04-30 23:15:33.000000 algomodule-1.0.4/Makefile
--rw-r--r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1945 2024-05-04 11:13:23.558112 algomodule-1.0.4/PKG-INFO
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1087 2024-04-30 22:07:31.000000 algomodule-1.0.4/README.md
--rwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)      721 2024-04-30 23:23:00.000000 algomodule-1.0.4/build-wheels.sh
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      982 2024-05-04 11:11:15.000000 algomodule-1.0.4/pyproject.toml
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1236 2024-05-04 11:13:23.562112 algomodule-1.0.4/setup.cfg
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      843 2024-05-04 10:43:02.000000 algomodule-1.0.4/setup.py
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.442111 algomodule-1.0.4/src/
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.442111 algomodule-1.0.4/src/3s/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      910 2024-05-04 11:11:57.000000 algomodule-1.0.4/src/3s/3s.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      170 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/3s/3s.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)   415328 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/algomodule.c
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.558112 algomodule-1.0.4/src/algomodule.egg-info/
--rw-r--r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1945 2024-05-04 11:13:23.000000 algomodule-1.0.4/src/algomodule.egg-info/PKG-INFO
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     3211 2024-05-04 11:13:23.000000 algomodule-1.0.4/src/algomodule.egg-info/SOURCES.txt
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)        1 2024-05-04 11:13:23.000000 algomodule-1.0.4/src/algomodule.egg-info/dependency_links.txt
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)        1 2024-05-04 11:08:49.000000 algomodule-1.0.4/src/algomodule.egg-info/not-zip-safe
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)        5 2024-05-04 11:13:23.000000 algomodule-1.0.4/src/algomodule.egg-info/top_level.txt
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     6056 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/algomodule.pyx
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.450111 algomodule-1.0.4/src/bcrypt/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    21091 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/bcrypt/bcrypt.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      175 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/bcrypt/bcrypt.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.450111 algomodule-1.0.4/src/bitblock/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     3215 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/bitblock/bitblock.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      169 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/bitblock/bitblock.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.454111 algomodule-1.0.4/src/blake/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      374 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/blake/blake.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      211 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/blake/blake.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.454111 algomodule-1.0.4/src/dcrypt/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     7258 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/dcrypt/dcrypt.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      197 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/dcrypt/dcrypt.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.458111 algomodule-1.0.4/src/fresh/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1159 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/fresh/fresh.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      195 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/fresh/fresh.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.458111 algomodule-1.0.4/src/fugue/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      277 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/fugue/fugue.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      195 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/fugue/fugue.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.462112 algomodule-1.0.4/src/groestl/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1054 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/groestl/groestl.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      290 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/groestl/groestl.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.462112 algomodule-1.0.4/src/hefty1/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     2037 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/hefty1/hefty1.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      198 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/hefty1/hefty1.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.466112 algomodule-1.0.4/src/jh/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     3682 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/jh/jh.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      181 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/jh/jh.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.466112 algomodule-1.0.4/src/keccak/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      343 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/keccak/keccak.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      215 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/keccak/keccak.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.470111 algomodule-1.0.4/src/neoscrypt/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    86841 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/neoscrypt/neoscrypt.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1954 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/neoscrypt/neoscrypt.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.470111 algomodule-1.0.4/src/nist5/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1266 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/nist5/nist5.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      194 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/nist5/nist5.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.470111 algomodule-1.0.4/src/quark/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     5537 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/quark/quark.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      195 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/quark/quark.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.474112 algomodule-1.0.4/src/qubit/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1371 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/qubit/qubit.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      195 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/qubit/qubit.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.478112 algomodule-1.0.4/src/scrypt/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    17868 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/scrypt/scrypt.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      305 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/scrypt/scrypt.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     7447 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/scrypt/scryptn.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      387 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/scrypt/scryptn.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.478112 algomodule-1.0.4/src/sha256/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     6645 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha256/sha2.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     2810 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha256/sha2.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10830 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha256.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.542112 algomodule-1.0.4/src/sha3/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    23455 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/aes_helper.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    23831 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/hamsi.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)  2220992 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/hamsi_helper.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     4709 2024-04-30 22:45:52.000000 algomodule-1.0.4/src/sha3/haval_helper.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10279 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/md_helper.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     8388 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sha2big.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    27363 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_blake.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10502 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_blake.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    29235 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_bmw.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10333 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_bmw.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    17424 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_cubehash.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     9756 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_cubehash.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    23907 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_echo.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10269 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_echo.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    41926 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_fugue.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1638 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_fugue.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)   132543 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_groestl.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10715 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_groestl.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10411 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_hamsi.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    33866 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_haval.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    31238 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_haval.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    11057 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_hefty1.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     2423 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_hefty1.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    34110 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_jh.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     9347 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_jh.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    54977 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_keccak.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     9540 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_keccak.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    36137 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_luffa.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     9574 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_luffa.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     7935 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_panama.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     4379 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_panama.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    12183 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_sha2.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    21438 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_shabal.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    11323 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_shabal.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    37764 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_shavite.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10660 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_shavite.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    49399 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_simd.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10174 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_simd.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    27247 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_skein.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     9902 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_skein.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    66236 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_types.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)   191546 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_whirlpool.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     6626 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/sha3/sph_whirlpool.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.542112 algomodule-1.0.4/src/shavite3/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      568 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/shavite3/shavite3.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      202 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/shavite3/shavite3.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.546112 algomodule-1.0.4/src/skein/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      600 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/skein/skein.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      211 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/skein/skein.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.550112 algomodule-1.0.4/src/twe/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1001 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/twe/twe.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      191 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/twe/twe.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.550112 algomodule-1.0.4/src/x11/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     2486 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/x11/x11.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      189 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/x11/x11.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.550112 algomodule-1.0.4/src/x13/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     2856 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/x13/x13.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)       97 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/x13/x13.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.554113 algomodule-1.0.4/src/x14/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     3044 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/x14/x14.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)       97 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/x14/x14.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.554113 algomodule-1.0.4/src/x15/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     3268 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/x15/x15.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      189 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/x15/x15.h
-drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 11:13:23.558112 algomodule-1.0.4/src/x17/
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     3773 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/x17/x17.c
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      167 2024-04-30 22:44:25.000000 algomodule-1.0.4/src/x17/x17.h
--rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      375 2024-04-30 23:32:01.000000 algomodule-1.0.4/test.py
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.949570 algomodule-1.1.0/
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.917570 algomodule-1.1.0/.github/
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.921570 algomodule-1.1.0/.github/workflows/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     2575 2024-05-04 20:04:05.000000 algomodule-1.1.0/.github/workflows/build.yaml
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)       49 2024-05-04 15:54:05.000000 algomodule-1.1.0/.gitignore
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)       54 2024-05-04 13:31:30.000000 algomodule-1.1.0/Makefile
+-rw-r--r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1945 2024-05-04 21:00:22.949570 algomodule-1.1.0/PKG-INFO
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1087 2024-04-30 22:07:31.000000 algomodule-1.1.0/README.md
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     2266 2024-05-04 20:21:39.000000 algomodule-1.1.0/pyproject.toml
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1236 2024-05-04 21:00:22.949570 algomodule-1.1.0/setup.cfg
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1356 2024-05-04 20:49:26.000000 algomodule-1.1.0/setup.py
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.925570 algomodule-1.1.0/src/
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.925570 algomodule-1.1.0/src/3s/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      910 2024-05-04 11:11:57.000000 algomodule-1.1.0/src/3s/3s.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      170 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/3s/3s.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)   415328 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/algomodule.c
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.949570 algomodule-1.1.0/src/algomodule.egg-info/
+-rw-r--r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1945 2024-05-04 21:00:22.000000 algomodule-1.1.0/src/algomodule.egg-info/PKG-INFO
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     5063 2024-05-04 21:00:22.000000 algomodule-1.1.0/src/algomodule.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)        1 2024-05-04 21:00:22.000000 algomodule-1.1.0/src/algomodule.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)        1 2024-05-04 11:08:49.000000 algomodule-1.1.0/src/algomodule.egg-info/not-zip-safe
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)        5 2024-05-04 21:00:22.000000 algomodule-1.1.0/src/algomodule.egg-info/top_level.txt
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     6056 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/algomodule.pyx
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.929570 algomodule-1.1.0/src/bcrypt/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    21091 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/bcrypt/bcrypt.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      175 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/bcrypt/bcrypt.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.929570 algomodule-1.1.0/src/bitblock/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     3215 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/bitblock/bitblock.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      169 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/bitblock/bitblock.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.929570 algomodule-1.1.0/src/blake/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      374 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/blake/blake.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      211 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/blake/blake.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.929570 algomodule-1.1.0/src/dcrypt/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     7258 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/dcrypt/dcrypt.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      197 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/dcrypt/dcrypt.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.929570 algomodule-1.1.0/src/fresh/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1159 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/fresh/fresh.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      195 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/fresh/fresh.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.929570 algomodule-1.1.0/src/fugue/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      277 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/fugue/fugue.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      195 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/fugue/fugue.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.929570 algomodule-1.1.0/src/groestl/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1054 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/groestl/groestl.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      290 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/groestl/groestl.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.929570 algomodule-1.1.0/src/hefty1/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     2037 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/hefty1/hefty1.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      198 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/hefty1/hefty1.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.929570 algomodule-1.1.0/src/jh/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     3682 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/jh/jh.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      181 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/jh/jh.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.929570 algomodule-1.1.0/src/keccak/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      343 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/keccak/keccak.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      215 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/keccak/keccak.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.933570 algomodule-1.1.0/src/neoscrypt/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    86841 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/neoscrypt/neoscrypt.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1954 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/neoscrypt/neoscrypt.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.933570 algomodule-1.1.0/src/nist5/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1266 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/nist5/nist5.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      194 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/nist5/nist5.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.933570 algomodule-1.1.0/src/quark/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     5537 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/quark/quark.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      195 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/quark/quark.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.933570 algomodule-1.1.0/src/qubit/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1371 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/qubit/qubit.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      195 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/qubit/qubit.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.933570 algomodule-1.1.0/src/scrypt/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    17868 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/scrypt/scrypt.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      305 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/scrypt/scrypt.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     7447 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/scrypt/scryptn.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      387 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/scrypt/scryptn.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.933570 algomodule-1.1.0/src/sha256/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     6645 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha256/sha2.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     2810 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha256/sha2.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10830 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha256.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.945570 algomodule-1.1.0/src/sha3/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    23455 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/aes_helper.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    23831 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/hamsi.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)  2220992 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/hamsi_helper.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     4733 2024-05-04 16:45:09.000000 algomodule-1.1.0/src/sha3/haval_helper.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10279 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/md_helper.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     8388 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sha2big.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    27363 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_blake.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10502 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_blake.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    29235 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_bmw.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10333 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_bmw.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    17424 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_cubehash.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     9756 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_cubehash.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    23907 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_echo.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10269 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_echo.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    41926 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_fugue.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1638 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_fugue.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)   132543 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_groestl.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10715 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_groestl.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10411 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_hamsi.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    33866 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_haval.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    31238 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_haval.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    11057 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_hefty1.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     2423 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_hefty1.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    34110 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_jh.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     9347 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_jh.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    54977 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_keccak.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     9540 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_keccak.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    36137 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_luffa.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     9574 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_luffa.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     7935 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_panama.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     4379 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_panama.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    12183 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_sha2.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    21438 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_shabal.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    11323 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_shabal.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    37764 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_shavite.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10660 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_shavite.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    49399 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_simd.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    10174 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_simd.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    27247 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_skein.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     9902 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_skein.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)    66236 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_types.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)   191546 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_whirlpool.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     6626 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/sha3/sph_whirlpool.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.945570 algomodule-1.1.0/src/shavite3/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      568 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/shavite3/shavite3.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      202 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/shavite3/shavite3.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.945570 algomodule-1.1.0/src/skein/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      600 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/skein/skein.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      211 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/skein/skein.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.945570 algomodule-1.1.0/src/twe/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     1001 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/twe/twe.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      191 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/twe/twe.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.945570 algomodule-1.1.0/src/x11/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     2486 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/x11/x11.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      189 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/x11/x11.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.945570 algomodule-1.1.0/src/x13/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     2856 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/x13/x13.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)       97 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/x13/x13.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.945570 algomodule-1.1.0/src/x14/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     3044 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/x14/x14.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)       97 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/x14/x14.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.949570 algomodule-1.1.0/src/x15/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     3268 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/x15/x15.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      189 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/x15/x15.h
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.949570 algomodule-1.1.0/src/x17/
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)     3773 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/x17/x17.c
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      167 2024-04-30 22:44:25.000000 algomodule-1.1.0/src/x17/x17.h
+-rw-rw-r--   0 ahmedbodi  (1000) ahmedbodi  (1000)      375 2024-04-30 23:32:01.000000 algomodule-1.1.0/test.py
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.921570 algomodule-1.1.0/tools/
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.949570 algomodule-1.1.0/tools/cibuildwheel/
+drwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)        0 2024-05-04 21:00:22.949570 algomodule-1.1.0/tools/cibuildwheel/manylinux/
+-rwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)     1725 2024-05-04 13:11:31.000000 algomodule-1.1.0/tools/cibuildwheel/manylinux/build-openssl.sh
+-rwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)     2014 2024-05-04 13:11:31.000000 algomodule-1.1.0/tools/cibuildwheel/manylinux/build_utils.sh
+-rwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)      192 2024-05-04 13:11:31.000000 algomodule-1.1.0/tools/cibuildwheel/manylinux/openssl-version.sh
+-rwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)      545 2024-05-04 13:11:31.000000 algomodule-1.1.0/tools/cibuildwheel/manylinux/update-scripts.sh
+-rwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)      522 2024-05-04 13:11:31.000000 algomodule-1.1.0/tools/cibuildwheel/setup_boost.sh
+-rwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)      946 2024-05-04 13:11:31.000000 algomodule-1.1.0/tools/cibuildwheel/setup_ccache_on_manylinux.sh
+-rwxrwxr-x   0 ahmedbodi  (1000) ahmedbodi  (1000)      439 2024-05-04 13:11:31.000000 algomodule-1.1.0/tools/cibuildwheel/setup_openssl.sh
```

### Comparing `algomodule-1.0.4/PKG-INFO` & `algomodule-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algomodule
-Version: 1.0.4
+Version: 1.1.0
 Summary: CryptoCurrency Hashing Library
 Home-page: https://github.com/electrum-altcoin/algomodule
 Author: Ahmed Bodiwala
 Author-email: Ahmed Bodiwala <ahmedbodi@crypto-expert.com>
 License: Proprietary
 Project-URL: Code, https://github.com/electrum-altcoin/AlgoLib
 Project-URL: Homepage, https://github.com/electrum-altcoin/AlgoLib
```

### Comparing `algomodule-1.0.4/README.md` & `algomodule-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/setup.cfg` & `algomodule-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/3s/3s.c` & `algomodule-1.1.0/src/3s/3s.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/algomodule.c` & `algomodule-1.1.0/src/algomodule.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/algomodule.egg-info/PKG-INFO` & `algomodule-1.1.0/src/algomodule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algomodule
-Version: 1.0.4
+Version: 1.1.0
 Summary: CryptoCurrency Hashing Library
 Home-page: https://github.com/electrum-altcoin/algomodule
 Author: Ahmed Bodiwala
 Author-email: Ahmed Bodiwala <ahmedbodi@crypto-expert.com>
 License: Proprietary
 Project-URL: Code, https://github.com/electrum-altcoin/AlgoLib
 Project-URL: Homepage, https://github.com/electrum-altcoin/AlgoLib
```

### Comparing `algomodule-1.0.4/src/algomodule.pyx` & `algomodule-1.1.0/src/algomodule.pyx`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/bcrypt/bcrypt.c` & `algomodule-1.1.0/src/bcrypt/bcrypt.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/bitblock/bitblock.c` & `algomodule-1.1.0/src/bitblock/bitblock.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/dcrypt/dcrypt.c` & `algomodule-1.1.0/src/dcrypt/dcrypt.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/fresh/fresh.c` & `algomodule-1.1.0/src/fresh/fresh.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/groestl/groestl.c` & `algomodule-1.1.0/src/groestl/groestl.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/hefty1/hefty1.c` & `algomodule-1.1.0/src/hefty1/hefty1.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/jh/jh.c` & `algomodule-1.1.0/src/jh/jh.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/neoscrypt/neoscrypt.c` & `algomodule-1.1.0/src/neoscrypt/neoscrypt.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/neoscrypt/neoscrypt.h` & `algomodule-1.1.0/src/neoscrypt/neoscrypt.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/nist5/nist5.c` & `algomodule-1.1.0/src/nist5/nist5.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/quark/quark.c` & `algomodule-1.1.0/src/quark/quark.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/qubit/qubit.c` & `algomodule-1.1.0/src/qubit/qubit.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/scrypt/scrypt.c` & `algomodule-1.1.0/src/scrypt/scrypt.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/scrypt/scryptn.c` & `algomodule-1.1.0/src/scrypt/scryptn.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha256/sha2.c` & `algomodule-1.1.0/src/sha256/sha2.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha256/sha2.h` & `algomodule-1.1.0/src/sha256/sha2.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha256.h` & `algomodule-1.1.0/src/sha256.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/aes_helper.c` & `algomodule-1.1.0/src/sha3/aes_helper.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/hamsi.c` & `algomodule-1.1.0/src/sha3/hamsi.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/hamsi_helper.c` & `algomodule-1.1.0/src/sha3/hamsi_helper.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/haval_helper.c` & `algomodule-1.1.0/src/sha3/haval_helper.c`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,16 @@
  * SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  *
  * ===========================(LICENSE END)=============================
  *
  * @author   Thomas Pornin <thomas.pornin@cryptolog.com>
  */
 #include <stddef.h>
+#include "sph_haval.h"
+
 #undef SPH_XCAT
 #define SPH_XCAT(a, b)    SPH_XCAT_(a, b)
 #undef SPH_XCAT_
 #define SPH_XCAT_(a, b)   a ## b
 
 static void
 #ifdef SPH_UPTR
```

### Comparing `algomodule-1.0.4/src/sha3/md_helper.c` & `algomodule-1.1.0/src/sha3/md_helper.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sha2big.c` & `algomodule-1.1.0/src/sha3/sha2big.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_blake.c` & `algomodule-1.1.0/src/sha3/sph_blake.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_blake.h` & `algomodule-1.1.0/src/sha3/sph_blake.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_bmw.c` & `algomodule-1.1.0/src/sha3/sph_bmw.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_bmw.h` & `algomodule-1.1.0/src/sha3/sph_bmw.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_cubehash.c` & `algomodule-1.1.0/src/sha3/sph_cubehash.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_cubehash.h` & `algomodule-1.1.0/src/sha3/sph_cubehash.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_echo.c` & `algomodule-1.1.0/src/sha3/sph_echo.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_echo.h` & `algomodule-1.1.0/src/sha3/sph_echo.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_fugue.c` & `algomodule-1.1.0/src/sha3/sph_fugue.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_fugue.h` & `algomodule-1.1.0/src/sha3/sph_fugue.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_groestl.c` & `algomodule-1.1.0/src/sha3/sph_groestl.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_groestl.h` & `algomodule-1.1.0/src/sha3/sph_groestl.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_hamsi.h` & `algomodule-1.1.0/src/sha3/sph_hamsi.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_haval.c` & `algomodule-1.1.0/src/sha3/sph_haval.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_haval.h` & `algomodule-1.1.0/src/sha3/sph_haval.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_hefty1.c` & `algomodule-1.1.0/src/sha3/sph_hefty1.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_hefty1.h` & `algomodule-1.1.0/src/sha3/sph_hefty1.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_jh.c` & `algomodule-1.1.0/src/sha3/sph_jh.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_jh.h` & `algomodule-1.1.0/src/sha3/sph_jh.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_keccak.c` & `algomodule-1.1.0/src/sha3/sph_keccak.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_keccak.h` & `algomodule-1.1.0/src/sha3/sph_keccak.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_luffa.c` & `algomodule-1.1.0/src/sha3/sph_luffa.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_luffa.h` & `algomodule-1.1.0/src/sha3/sph_luffa.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_panama.c` & `algomodule-1.1.0/src/sha3/sph_panama.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_panama.h` & `algomodule-1.1.0/src/sha3/sph_panama.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_sha2.h` & `algomodule-1.1.0/src/sha3/sph_sha2.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_shabal.c` & `algomodule-1.1.0/src/sha3/sph_shabal.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_shabal.h` & `algomodule-1.1.0/src/sha3/sph_shabal.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_shavite.c` & `algomodule-1.1.0/src/sha3/sph_shavite.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_shavite.h` & `algomodule-1.1.0/src/sha3/sph_shavite.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_simd.c` & `algomodule-1.1.0/src/sha3/sph_simd.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_simd.h` & `algomodule-1.1.0/src/sha3/sph_simd.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_skein.c` & `algomodule-1.1.0/src/sha3/sph_skein.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_skein.h` & `algomodule-1.1.0/src/sha3/sph_skein.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_types.h` & `algomodule-1.1.0/src/sha3/sph_types.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_whirlpool.c` & `algomodule-1.1.0/src/sha3/sph_whirlpool.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/sha3/sph_whirlpool.h` & `algomodule-1.1.0/src/sha3/sph_whirlpool.h`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/shavite3/shavite3.c` & `algomodule-1.1.0/src/shavite3/shavite3.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/skein/skein.c` & `algomodule-1.1.0/src/skein/skein.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/twe/twe.c` & `algomodule-1.1.0/src/twe/twe.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/x11/x11.c` & `algomodule-1.1.0/src/x11/x11.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/x13/x13.c` & `algomodule-1.1.0/src/x13/x13.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/x14/x14.c` & `algomodule-1.1.0/src/x14/x14.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/x15/x15.c` & `algomodule-1.1.0/src/x15/x15.c`

 * *Files identical despite different names*

### Comparing `algomodule-1.0.4/src/x17/x17.c` & `algomodule-1.1.0/src/x17/x17.c`

 * *Files identical despite different names*

