# Comparing `tmp/ReverseBox-0.8.3.tar.gz` & `tmp/ReverseBox-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseBox-0.8.3.tar", last modified: Fri May  3 22:58:03 2024, max compression
+gzip compressed data, was "ReverseBox-0.8.4.tar", last modified: Fri May  3 23:02:17 2024, max compression
```

## Comparing `ReverseBox-0.8.3.tar` & `ReverseBox-0.8.4.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.383428 ReverseBox-0.8.3/
--rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:48.000000 ReverseBox-0.8.3/LICENSE
--rw-rw-rw-   0        0        0     6931 2024-05-03 22:58:03.382431 ReverseBox-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     5530 2024-05-02 09:31:21.000000 ReverseBox-0.8.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.315609 ReverseBox-0.8.3/ReverseBox.egg-info/
--rw-rw-rw-   0        0        0     6931 2024-05-03 22:58:03.000000 ReverseBox-0.8.3/ReverseBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2754 2024-05-03 22:58:03.000000 ReverseBox-0.8.3/ReverseBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 22:58:03.000000 ReverseBox-0.8.3/ReverseBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-03 22:58:03.000000 ReverseBox-0.8.3/ReverseBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-03 22:58:03.000000 ReverseBox-0.8.3/ReverseBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.316607 ReverseBox-0.8.3/reversebox/
--rw-rw-rw-   0        0        0        0 2022-06-25 12:19:28.000000 ReverseBox-0.8.3/reversebox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.320596 ReverseBox-0.8.3/reversebox/checksum/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.3/reversebox/checksum/__init__.py
--rw-rw-rw-   0        0        0      404 2023-01-08 20:51:08.000000 ReverseBox-0.8.3/reversebox/checksum/checksum_adler32.py
--rw-rw-rw-   0        0        0      404 2023-07-06 21:19:52.000000 ReverseBox-0.8.3/reversebox/checksum/checksum_bsd16.py
--rw-rw-rw-   0        0        0      403 2023-01-09 21:19:58.000000 ReverseBox-0.8.3/reversebox/checksum/checksum_fletcher16.py
--rw-rw-rw-   0        0        0      510 2023-01-09 22:41:54.000000 ReverseBox-0.8.3/reversebox/checksum/checksum_fletcher32.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.322591 ReverseBox-0.8.3/reversebox/common/
--rw-rw-rw-   0        0        0        0 2022-06-25 16:29:14.000000 ReverseBox-0.8.3/reversebox/common/__init__.py
--rw-rw-rw-   0        0        0      491 2023-07-05 21:46:48.000000 ReverseBox-0.8.3/reversebox/common/common.py
--rw-rw-rw-   0        0        0      730 2022-09-07 19:55:28.000000 ReverseBox-0.8.3/reversebox/common/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.327577 ReverseBox-0.8.3/reversebox/compression/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.3/reversebox/compression/__init__.py
--rw-rw-rw-   0        0        0      473 2024-05-03 14:40:28.000000 ReverseBox-0.8.3/reversebox/compression/compression_jcalg1.py
--rw-rw-rw-   0        0        0      335 2022-12-27 14:57:00.000000 ReverseBox-0.8.3/reversebox/compression/compression_lzo.py
--rw-rw-rw-   0        0        0      796 2024-05-03 22:56:37.000000 ReverseBox-0.8.3/reversebox/compression/compression_refpack.py
--rw-rw-rw-   0        0        0      330 2022-10-15 10:41:40.000000 ReverseBox-0.8.3/reversebox/compression/compression_zlib.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.337551 ReverseBox-0.8.3/reversebox/crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:26:30.000000 ReverseBox-0.8.3/reversebox/crc/__init__.py
--rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:20.000000 ReverseBox-0.8.3/reversebox/crc/crc16_arc.py
--rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:32.000000 ReverseBox-0.8.3/reversebox/crc/crc16_ccitt.py
--rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:08.000000 ReverseBox-0.8.3/reversebox/crc/crc16_dnp.py
--rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:20.000000 ReverseBox-0.8.3/reversebox/crc/crc16_kermit.py
--rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:38.000000 ReverseBox-0.8.3/reversebox/crc/crc16_modbus.py
--rw-rw-rw-   0        0        0      735 2022-07-21 21:35:32.000000 ReverseBox-0.8.3/reversebox/crc/crc16_sick.py
--rw-rw-rw-   0        0        0     3784 2023-09-13 22:28:42.000000 ReverseBox-0.8.3/reversebox/crc/crc32_asobo.py
--rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:20.000000 ReverseBox-0.8.3/reversebox/crc/crc32_iso_hdlc.py
--rw-rw-rw-   0        0        0     6040 2023-11-15 15:34:51.000000 ReverseBox-0.8.3/reversebox/crc/crc64_asobo.py
--rw-rw-rw-   0        0        0     1402 2023-07-08 10:59:02.000000 ReverseBox-0.8.3/reversebox/crc/crc8.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.343535 ReverseBox-0.8.3/reversebox/encryption/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.3/reversebox/encryption/__init__.py
--rw-rw-rw-   0        0        0     1094 2023-11-16 14:56:06.000000 ReverseBox-0.8.3/reversebox/encryption/encryption_rot13.py
--rw-rw-rw-   0        0        0      579 2022-07-17 23:25:20.000000 ReverseBox-0.8.3/reversebox/encryption/encryption_xor_basic.py
--rw-rw-rw-   0        0        0     1551 2024-03-17 21:48:42.000000 ReverseBox-0.8.3/reversebox/encryption/encryption_xor_basic_key_guesser.py
--rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:02.000000 ReverseBox-0.8.3/reversebox/encryption/encryption_xor_gianas_return_zda.py
--rw-rw-rw-   0        0        0      574 2022-07-17 23:25:20.000000 ReverseBox-0.8.3/reversebox/encryption/encryption_xor_retro64_eco.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.348521 ReverseBox-0.8.3/reversebox/hash/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.3/reversebox/hash/__init__.py
--rw-rw-rw-   0        0        0     2127 2024-04-29 16:13:10.000000 ReverseBox-0.8.3/reversebox/hash/hash_fnv.py
--rw-rw-rw-   0        0        0      386 2023-11-15 15:27:56.000000 ReverseBox-0.8.3/reversebox/hash/hash_md2.py
--rw-rw-rw-   0        0        0      280 2022-09-11 18:48:38.000000 ReverseBox-0.8.3/reversebox/hash/hash_md5.py
--rw-rw-rw-   0        0        0      283 2023-01-08 14:05:02.000000 ReverseBox-0.8.3/reversebox/hash/hash_sha1.py
--rw-rw-rw-   0        0        0      289 2023-01-08 14:07:32.000000 ReverseBox-0.8.3/reversebox/hash/hash_sha2.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.354505 ReverseBox-0.8.3/reversebox/image/
--rw-rw-rw-   0        0        0        0 2022-12-27 21:18:26.000000 ReverseBox-0.8.3/reversebox/image/__init__.py
--rw-rw-rw-   0        0        0     2836 2024-05-02 09:31:33.000000 ReverseBox-0.8.3/reversebox/image/image_dds.py
--rw-rw-rw-   0        0        0    11793 2024-05-02 11:12:02.000000 ReverseBox-0.8.3/reversebox/image/image_decoder.py
--rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:20.000000 ReverseBox-0.8.3/reversebox/image/image_finder_gui.py
--rw-rw-rw-   0        0        0      713 2023-04-23 00:00:02.000000 ReverseBox-0.8.3/reversebox/image/image_finder_main.py
--rw-rw-rw-   0        0        0      614 2024-05-02 09:31:21.000000 ReverseBox-0.8.3/reversebox/image/image_formats.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.361487 ReverseBox-0.8.3/reversebox/image/swizzling/
--rw-rw-rw-   0        0        0        0 2024-04-12 20:30:39.000000 ReverseBox-0.8.3/reversebox/image/swizzling/__init__.py
--rw-rw-rw-   0        0        0      848 2024-04-14 22:08:19.000000 ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_3ds.py
--rw-rw-rw-   0        0        0     2045 2024-04-14 21:57:16.000000 ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_cmpr.py
--rw-rw-rw-   0        0        0     2457 2024-04-14 21:57:16.000000 ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_ps2.py
--rw-rw-rw-   0        0        0     1529 2024-04-14 21:59:10.000000 ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_psp.py
--rw-rw-rw-   0        0        0     1854 2024-04-14 22:03:05.000000 ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_psvita.py
--rw-rw-rw-   0        0        0     1571 2024-04-14 22:03:55.000000 ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_switch.py
--rw-rw-rw-   0        0        0       93 2024-04-14 21:57:16.000000 ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_xbox.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.368468 ReverseBox-0.8.3/reversebox/io_files/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.3/reversebox/io_files/__init__.py
--rw-rw-rw-   0        0        0     1420 2024-04-26 22:10:36.000000 ReverseBox-0.8.3/reversebox/io_files/bytes_handler.py
--rw-rw-rw-   0        0        0      789 2024-05-02 10:36:13.000000 ReverseBox-0.8.3/reversebox/io_files/bytes_helper_functions.py
--rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:50.000000 ReverseBox-0.8.3/reversebox/io_files/check_file.py
--rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:42.000000 ReverseBox-0.8.3/reversebox/io_files/file_handler.py
--rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:16.000000 ReverseBox-0.8.3/reversebox/io_files/mod_handler.py
--rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:24.000000 ReverseBox-0.8.3/reversebox/io_files/translation_text_handler.py
--rw-rw-rw-   0        0        0       42 2024-05-03 22:58:03.383428 ReverseBox-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1884 2024-05-03 22:56:59.000000 ReverseBox-0.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.369465 ReverseBox-0.8.3/tests/
--rw-rw-rw-   0        0        0        0 2022-07-19 22:27:12.000000 ReverseBox-0.8.3/tests/__init__.py
--rw-rw-rw-   0        0        0      879 2024-03-17 21:42:22.000000 ReverseBox-0.8.3/tests/common.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:03.381434 ReverseBox-0.8.3/tests/tests_crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:28:34.000000 ReverseBox-0.8.3/tests/tests_crc/__init__.py
--rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:10.000000 ReverseBox-0.8.3/tests/tests_crc/test_crc16_arc.py
--rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:10.000000 ReverseBox-0.8.3/tests/tests_crc/test_crc16_ccitt.py
--rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:10.000000 ReverseBox-0.8.3/tests/tests_crc/test_crc16_dnp.py
--rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:10.000000 ReverseBox-0.8.3/tests/tests_crc/test_crc16_kermit.py
--rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:10.000000 ReverseBox-0.8.3/tests/tests_crc/test_crc16_modbus.py
--rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:10.000000 ReverseBox-0.8.3/tests/tests_crc/test_crc16_sick.py
--rw-rw-rw-   0        0        0     2209 2023-09-13 22:24:14.000000 ReverseBox-0.8.3/tests/tests_crc/test_crc32_asobo.py
--rw-rw-rw-   0        0        0     2655 2023-04-23 00:00:02.000000 ReverseBox-0.8.3/tests/tests_crc/test_crc32_iso_hdlc.py
--rw-rw-rw-   0        0        0     1822 2023-07-08 10:59:02.000000 ReverseBox-0.8.3/tests/tests_crc/test_crc8.py
--rw-rw-rw-   0        0        0     1850 2023-07-08 10:59:02.000000 ReverseBox-0.8.3/tests/tests_crc/test_crc8_cdma_2000.py
--rw-rw-rw-   0        0        0     1832 2023-07-08 10:59:02.000000 ReverseBox-0.8.3/tests/tests_crc/test_crc8_darc.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.098256 ReverseBox-0.8.4/
+-rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:48.000000 ReverseBox-0.8.4/LICENSE
+-rw-rw-rw-   0        0        0     6982 2024-05-03 23:02:17.098256 ReverseBox-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5581 2024-05-03 23:01:57.000000 ReverseBox-0.8.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.032432 ReverseBox-0.8.4/ReverseBox.egg-info/
+-rw-rw-rw-   0        0        0     6982 2024-05-03 23:02:16.000000 ReverseBox-0.8.4/ReverseBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2754 2024-05-03 23:02:16.000000 ReverseBox-0.8.4/ReverseBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 23:02:16.000000 ReverseBox-0.8.4/ReverseBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-03 23:02:16.000000 ReverseBox-0.8.4/ReverseBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-03 23:02:16.000000 ReverseBox-0.8.4/ReverseBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.033429 ReverseBox-0.8.4/reversebox/
+-rw-rw-rw-   0        0        0        0 2022-06-25 12:19:28.000000 ReverseBox-0.8.4/reversebox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.037418 ReverseBox-0.8.4/reversebox/checksum/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.4/reversebox/checksum/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-01-08 20:51:08.000000 ReverseBox-0.8.4/reversebox/checksum/checksum_adler32.py
+-rw-rw-rw-   0        0        0      404 2023-07-06 21:19:52.000000 ReverseBox-0.8.4/reversebox/checksum/checksum_bsd16.py
+-rw-rw-rw-   0        0        0      403 2023-01-09 21:19:58.000000 ReverseBox-0.8.4/reversebox/checksum/checksum_fletcher16.py
+-rw-rw-rw-   0        0        0      510 2023-01-09 22:41:54.000000 ReverseBox-0.8.4/reversebox/checksum/checksum_fletcher32.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.040411 ReverseBox-0.8.4/reversebox/common/
+-rw-rw-rw-   0        0        0        0 2022-06-25 16:29:14.000000 ReverseBox-0.8.4/reversebox/common/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-07-05 21:46:48.000000 ReverseBox-0.8.4/reversebox/common/common.py
+-rw-rw-rw-   0        0        0      730 2022-09-07 19:55:28.000000 ReverseBox-0.8.4/reversebox/common/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.044400 ReverseBox-0.8.4/reversebox/compression/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.4/reversebox/compression/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-05-03 14:40:28.000000 ReverseBox-0.8.4/reversebox/compression/compression_jcalg1.py
+-rw-rw-rw-   0        0        0      335 2022-12-27 14:57:00.000000 ReverseBox-0.8.4/reversebox/compression/compression_lzo.py
+-rw-rw-rw-   0        0        0      796 2024-05-03 22:56:37.000000 ReverseBox-0.8.4/reversebox/compression/compression_refpack.py
+-rw-rw-rw-   0        0        0      330 2022-10-15 10:41:40.000000 ReverseBox-0.8.4/reversebox/compression/compression_zlib.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.054373 ReverseBox-0.8.4/reversebox/crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:26:30.000000 ReverseBox-0.8.4/reversebox/crc/__init__.py
+-rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:20.000000 ReverseBox-0.8.4/reversebox/crc/crc16_arc.py
+-rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:32.000000 ReverseBox-0.8.4/reversebox/crc/crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:08.000000 ReverseBox-0.8.4/reversebox/crc/crc16_dnp.py
+-rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:20.000000 ReverseBox-0.8.4/reversebox/crc/crc16_kermit.py
+-rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:38.000000 ReverseBox-0.8.4/reversebox/crc/crc16_modbus.py
+-rw-rw-rw-   0        0        0      735 2022-07-21 21:35:32.000000 ReverseBox-0.8.4/reversebox/crc/crc16_sick.py
+-rw-rw-rw-   0        0        0     3784 2023-09-13 22:28:42.000000 ReverseBox-0.8.4/reversebox/crc/crc32_asobo.py
+-rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:20.000000 ReverseBox-0.8.4/reversebox/crc/crc32_iso_hdlc.py
+-rw-rw-rw-   0        0        0     6040 2023-11-15 15:34:51.000000 ReverseBox-0.8.4/reversebox/crc/crc64_asobo.py
+-rw-rw-rw-   0        0        0     1402 2023-07-08 10:59:02.000000 ReverseBox-0.8.4/reversebox/crc/crc8.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.059360 ReverseBox-0.8.4/reversebox/encryption/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.4/reversebox/encryption/__init__.py
+-rw-rw-rw-   0        0        0     1094 2023-11-16 14:56:06.000000 ReverseBox-0.8.4/reversebox/encryption/encryption_rot13.py
+-rw-rw-rw-   0        0        0      579 2022-07-17 23:25:20.000000 ReverseBox-0.8.4/reversebox/encryption/encryption_xor_basic.py
+-rw-rw-rw-   0        0        0     1551 2024-03-17 21:48:42.000000 ReverseBox-0.8.4/reversebox/encryption/encryption_xor_basic_key_guesser.py
+-rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:02.000000 ReverseBox-0.8.4/reversebox/encryption/encryption_xor_gianas_return_zda.py
+-rw-rw-rw-   0        0        0      574 2022-07-17 23:25:20.000000 ReverseBox-0.8.4/reversebox/encryption/encryption_xor_retro64_eco.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.065344 ReverseBox-0.8.4/reversebox/hash/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.4/reversebox/hash/__init__.py
+-rw-rw-rw-   0        0        0     2127 2024-04-29 16:13:10.000000 ReverseBox-0.8.4/reversebox/hash/hash_fnv.py
+-rw-rw-rw-   0        0        0      386 2023-11-15 15:27:56.000000 ReverseBox-0.8.4/reversebox/hash/hash_md2.py
+-rw-rw-rw-   0        0        0      280 2022-09-11 18:48:38.000000 ReverseBox-0.8.4/reversebox/hash/hash_md5.py
+-rw-rw-rw-   0        0        0      283 2023-01-08 14:05:02.000000 ReverseBox-0.8.4/reversebox/hash/hash_sha1.py
+-rw-rw-rw-   0        0        0      289 2023-01-08 14:07:32.000000 ReverseBox-0.8.4/reversebox/hash/hash_sha2.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.070331 ReverseBox-0.8.4/reversebox/image/
+-rw-rw-rw-   0        0        0        0 2022-12-27 21:18:26.000000 ReverseBox-0.8.4/reversebox/image/__init__.py
+-rw-rw-rw-   0        0        0     2836 2024-05-02 09:31:33.000000 ReverseBox-0.8.4/reversebox/image/image_dds.py
+-rw-rw-rw-   0        0        0    11793 2024-05-02 11:12:02.000000 ReverseBox-0.8.4/reversebox/image/image_decoder.py
+-rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:20.000000 ReverseBox-0.8.4/reversebox/image/image_finder_gui.py
+-rw-rw-rw-   0        0        0      713 2023-04-23 00:00:02.000000 ReverseBox-0.8.4/reversebox/image/image_finder_main.py
+-rw-rw-rw-   0        0        0      614 2024-05-02 09:31:21.000000 ReverseBox-0.8.4/reversebox/image/image_formats.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.077312 ReverseBox-0.8.4/reversebox/image/swizzling/
+-rw-rw-rw-   0        0        0        0 2024-04-12 20:30:39.000000 ReverseBox-0.8.4/reversebox/image/swizzling/__init__.py
+-rw-rw-rw-   0        0        0      848 2024-04-14 22:08:19.000000 ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_3ds.py
+-rw-rw-rw-   0        0        0     2045 2024-04-14 21:57:16.000000 ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_cmpr.py
+-rw-rw-rw-   0        0        0     2457 2024-04-14 21:57:16.000000 ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_ps2.py
+-rw-rw-rw-   0        0        0     1529 2024-04-14 21:59:10.000000 ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_psp.py
+-rw-rw-rw-   0        0        0     1854 2024-04-14 22:03:05.000000 ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_psvita.py
+-rw-rw-rw-   0        0        0     1571 2024-04-14 22:03:55.000000 ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_switch.py
+-rw-rw-rw-   0        0        0       93 2024-04-14 21:57:16.000000 ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_xbox.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.084293 ReverseBox-0.8.4/reversebox/io_files/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.4/reversebox/io_files/__init__.py
+-rw-rw-rw-   0        0        0     1420 2024-04-26 22:10:36.000000 ReverseBox-0.8.4/reversebox/io_files/bytes_handler.py
+-rw-rw-rw-   0        0        0      789 2024-05-02 10:36:13.000000 ReverseBox-0.8.4/reversebox/io_files/bytes_helper_functions.py
+-rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:50.000000 ReverseBox-0.8.4/reversebox/io_files/check_file.py
+-rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:42.000000 ReverseBox-0.8.4/reversebox/io_files/file_handler.py
+-rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:16.000000 ReverseBox-0.8.4/reversebox/io_files/mod_handler.py
+-rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:24.000000 ReverseBox-0.8.4/reversebox/io_files/translation_text_handler.py
+-rw-rw-rw-   0        0        0       42 2024-05-03 23:02:17.099253 ReverseBox-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1884 2024-05-03 23:01:57.000000 ReverseBox-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.086288 ReverseBox-0.8.4/tests/
+-rw-rw-rw-   0        0        0        0 2022-07-19 22:27:12.000000 ReverseBox-0.8.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      879 2024-03-17 21:42:22.000000 ReverseBox-0.8.4/tests/common.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:02:17.096261 ReverseBox-0.8.4/tests/tests_crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:28:34.000000 ReverseBox-0.8.4/tests/tests_crc/__init__.py
+-rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:10.000000 ReverseBox-0.8.4/tests/tests_crc/test_crc16_arc.py
+-rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:10.000000 ReverseBox-0.8.4/tests/tests_crc/test_crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:10.000000 ReverseBox-0.8.4/tests/tests_crc/test_crc16_dnp.py
+-rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:10.000000 ReverseBox-0.8.4/tests/tests_crc/test_crc16_kermit.py
+-rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:10.000000 ReverseBox-0.8.4/tests/tests_crc/test_crc16_modbus.py
+-rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:10.000000 ReverseBox-0.8.4/tests/tests_crc/test_crc16_sick.py
+-rw-rw-rw-   0        0        0     2209 2023-09-13 22:24:14.000000 ReverseBox-0.8.4/tests/tests_crc/test_crc32_asobo.py
+-rw-rw-rw-   0        0        0     2655 2023-04-23 00:00:02.000000 ReverseBox-0.8.4/tests/tests_crc/test_crc32_iso_hdlc.py
+-rw-rw-rw-   0        0        0     1822 2023-07-08 10:59:02.000000 ReverseBox-0.8.4/tests/tests_crc/test_crc8.py
+-rw-rw-rw-   0        0        0     1850 2023-07-08 10:59:02.000000 ReverseBox-0.8.4/tests/tests_crc/test_crc8_cdma_2000.py
+-rw-rw-rw-   0        0        0     1832 2023-07-08 10:59:02.000000 ReverseBox-0.8.4/tests/tests_crc/test_crc8_darc.py
```

### Comparing `ReverseBox-0.8.3/LICENSE` & `ReverseBox-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/PKG-INFO` & `ReverseBox-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.8.3
+Version: 0.8.4
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python,image,decode,decoding,RGB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -84,15 +84,15 @@
   - GZIP (TODO) ❌
   - JCALG1 (TODO) ❌
   - LZMA (TODO) ❌
   - LZO / LZO1X ✔️ <span style="color:yellow">(wrapper only)</span>
   - LZSS (TODO) ❌
   - NitroSDK (TODO) ❌
   - Oodle (TODO) ❌
-  - Refpack (EA) (TODO) ❌
+  - Refpack (EA Games) ✔️ <span style="color:yellow">(wrapper only)</span>
   - RNC (TODO) ❌
   - ZLIB ✔️ <span style="color:yellow">(wrapper only)</span>
 
 * Encryption
   - AES (TODO) ❌
   - DES (TODO) ❌
   - Lucifer / DTD-1 (TODO) ❌
```

### Comparing `ReverseBox-0.8.3/README.md` & `ReverseBox-0.8.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
   - GZIP (TODO) ❌
   - JCALG1 (TODO) ❌
   - LZMA (TODO) ❌
   - LZO / LZO1X ✔️ <span style="color:yellow">(wrapper only)</span>
   - LZSS (TODO) ❌
   - NitroSDK (TODO) ❌
   - Oodle (TODO) ❌
-  - Refpack (EA) (TODO) ❌
+  - Refpack (EA Games) ✔️ <span style="color:yellow">(wrapper only)</span>
   - RNC (TODO) ❌
   - ZLIB ✔️ <span style="color:yellow">(wrapper only)</span>
 
 * Encryption
   - AES (TODO) ❌
   - DES (TODO) ❌
   - Lucifer / DTD-1 (TODO) ❌
```

### Comparing `ReverseBox-0.8.3/ReverseBox.egg-info/PKG-INFO` & `ReverseBox-0.8.4/ReverseBox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.8.3
+Version: 0.8.4
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python,image,decode,decoding,RGB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -84,15 +84,15 @@
   - GZIP (TODO) ❌
   - JCALG1 (TODO) ❌
   - LZMA (TODO) ❌
   - LZO / LZO1X ✔️ <span style="color:yellow">(wrapper only)</span>
   - LZSS (TODO) ❌
   - NitroSDK (TODO) ❌
   - Oodle (TODO) ❌
-  - Refpack (EA) (TODO) ❌
+  - Refpack (EA Games) ✔️ <span style="color:yellow">(wrapper only)</span>
   - RNC (TODO) ❌
   - ZLIB ✔️ <span style="color:yellow">(wrapper only)</span>
 
 * Encryption
   - AES (TODO) ❌
   - DES (TODO) ❌
   - Lucifer / DTD-1 (TODO) ❌
```

### Comparing `ReverseBox-0.8.3/ReverseBox.egg-info/SOURCES.txt` & `ReverseBox-0.8.4/ReverseBox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/common/logger.py` & `ReverseBox-0.8.4/reversebox/common/logger.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/compression/compression_refpack.py` & `ReverseBox-0.8.4/reversebox/compression/compression_refpack.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/crc/crc16_arc.py` & `ReverseBox-0.8.4/reversebox/crc/crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/crc/crc16_ccitt.py` & `ReverseBox-0.8.4/reversebox/crc/crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/crc/crc16_dnp.py` & `ReverseBox-0.8.4/reversebox/crc/crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/crc/crc16_kermit.py` & `ReverseBox-0.8.4/reversebox/crc/crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/crc/crc16_modbus.py` & `ReverseBox-0.8.4/reversebox/crc/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/crc/crc16_sick.py` & `ReverseBox-0.8.4/reversebox/crc/crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/crc/crc32_asobo.py` & `ReverseBox-0.8.4/reversebox/crc/crc32_asobo.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/crc/crc32_iso_hdlc.py` & `ReverseBox-0.8.4/reversebox/crc/crc32_iso_hdlc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/crc/crc64_asobo.py` & `ReverseBox-0.8.4/reversebox/crc/crc64_asobo.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/crc/crc8.py` & `ReverseBox-0.8.4/reversebox/crc/crc8.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/encryption/encryption_rot13.py` & `ReverseBox-0.8.4/reversebox/encryption/encryption_rot13.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/encryption/encryption_xor_basic.py` & `ReverseBox-0.8.4/reversebox/encryption/encryption_xor_basic.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/encryption/encryption_xor_basic_key_guesser.py` & `ReverseBox-0.8.4/reversebox/encryption/encryption_xor_basic_key_guesser.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/encryption/encryption_xor_gianas_return_zda.py` & `ReverseBox-0.8.4/reversebox/encryption/encryption_xor_gianas_return_zda.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/encryption/encryption_xor_retro64_eco.py` & `ReverseBox-0.8.4/reversebox/encryption/encryption_xor_retro64_eco.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/hash/hash_fnv.py` & `ReverseBox-0.8.4/reversebox/hash/hash_fnv.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/image/image_dds.py` & `ReverseBox-0.8.4/reversebox/image/image_dds.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/image/image_decoder.py` & `ReverseBox-0.8.4/reversebox/image/image_decoder.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/image/image_finder_gui.py` & `ReverseBox-0.8.4/reversebox/image/image_finder_gui.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/image/image_finder_main.py` & `ReverseBox-0.8.4/reversebox/image/image_finder_main.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/image/image_formats.py` & `ReverseBox-0.8.4/reversebox/image/image_formats.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_3ds.py` & `ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_3ds.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_cmpr.py` & `ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_cmpr.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_ps2.py` & `ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_ps2.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_psp.py` & `ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_psp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_psvita.py` & `ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_psvita.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/image/swizzling/swizzle_switch.py` & `ReverseBox-0.8.4/reversebox/image/swizzling/swizzle_switch.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/io_files/bytes_handler.py` & `ReverseBox-0.8.4/reversebox/io_files/bytes_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/io_files/bytes_helper_functions.py` & `ReverseBox-0.8.4/reversebox/io_files/bytes_helper_functions.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/io_files/check_file.py` & `ReverseBox-0.8.4/reversebox/io_files/check_file.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/io_files/file_handler.py` & `ReverseBox-0.8.4/reversebox/io_files/file_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/io_files/mod_handler.py` & `ReverseBox-0.8.4/reversebox/io_files/mod_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/reversebox/io_files/translation_text_handler.py` & `ReverseBox-0.8.4/reversebox/io_files/translation_text_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/setup.py` & `ReverseBox-0.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 License: GPL-3.0 License
 """
 
 import os
 
 import setuptools
 
-VERSION_NUM = "0.8.3"
+VERSION_NUM = "0.8.4"
 
 
 def get_long_description() -> str:
     with open(
         os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf8"
     ) as readme:
         readme_text = readme.read()
```

### Comparing `ReverseBox-0.8.3/tests/common.py` & `ReverseBox-0.8.4/tests/common.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/tests/tests_crc/test_crc16_arc.py` & `ReverseBox-0.8.4/tests/tests_crc/test_crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/tests/tests_crc/test_crc16_ccitt.py` & `ReverseBox-0.8.4/tests/tests_crc/test_crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/tests/tests_crc/test_crc16_dnp.py` & `ReverseBox-0.8.4/tests/tests_crc/test_crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/tests/tests_crc/test_crc16_kermit.py` & `ReverseBox-0.8.4/tests/tests_crc/test_crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/tests/tests_crc/test_crc16_modbus.py` & `ReverseBox-0.8.4/tests/tests_crc/test_crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/tests/tests_crc/test_crc16_sick.py` & `ReverseBox-0.8.4/tests/tests_crc/test_crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/tests/tests_crc/test_crc32_asobo.py` & `ReverseBox-0.8.4/tests/tests_crc/test_crc32_asobo.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/tests/tests_crc/test_crc32_iso_hdlc.py` & `ReverseBox-0.8.4/tests/tests_crc/test_crc32_iso_hdlc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/tests/tests_crc/test_crc8.py` & `ReverseBox-0.8.4/tests/tests_crc/test_crc8.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/tests/tests_crc/test_crc8_cdma_2000.py` & `ReverseBox-0.8.4/tests/tests_crc/test_crc8_cdma_2000.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.3/tests/tests_crc/test_crc8_darc.py` & `ReverseBox-0.8.4/tests/tests_crc/test_crc8_darc.py`

 * *Files identical despite different names*

