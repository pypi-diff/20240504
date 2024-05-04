# Comparing `tmp/aps-toolkit-0.5.3.tar.gz` & `tmp/aps-toolkit-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps-toolkit-0.5.3.tar", last modified: Wed May  1 12:30:22 2024, max compression
+gzip compressed data, was "aps-toolkit-0.5.4.tar", last modified: Sat May  4 09:15:07 2024, max compression
```

## Comparing `aps-toolkit-0.5.3.tar` & `aps-toolkit-0.5.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 12:30:22.963682 aps-toolkit-0.5.3/
--rw-r--r--   0 chuongmep   (501) staff       (20)     1908 2024-05-01 12:30:22.963458 aps-toolkit-0.5.3/PKG-INFO
--rw-r--r--   0 chuongmep   (501) staff       (20)       38 2024-05-01 12:30:22.963723 aps-toolkit-0.5.3/setup.cfg
--rw-r--r--   0 chuongmep   (501) staff       (20)      874 2024-05-01 12:30:08.000000 aps-toolkit-0.5.3/setup.py
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 12:30:22.947691 aps-toolkit-0.5.3/src/
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 12:30:22.957871 aps-toolkit-0.5.3/src/aps_toolkit/
--rw-r--r--   0 chuongmep   (501) staff       (20)     5733 2024-05-01 12:27:47.000000 aps-toolkit-0.5.3/src/aps_toolkit/Auth.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    10134 2024-03-27 11:22:45.000000 aps-toolkit-0.5.3/src/aps_toolkit/BIM360.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     8892 2024-03-27 12:37:29.000000 aps-toolkit-0.5.3/src/aps_toolkit/Bucket.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     2449 2024-03-24 09:10:01.000000 aps-toolkit-0.5.3/src/aps_toolkit/DbReader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    12604 2024-03-24 09:10:01.000000 aps-toolkit-0.5.3/src/aps_toolkit/Derivative.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3845 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/Fragments.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     2322 2024-03-27 12:03:33.000000 aps-toolkit-0.5.3/src/aps_toolkit/InputStream.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      880 2024-03-23 03:57:09.000000 aps-toolkit-0.5.3/src/aps_toolkit/ManifestItem.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1136 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/MaterialProperties.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1726 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/Materials.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3686 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/PackFileReader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      925 2024-03-23 03:57:09.000000 aps-toolkit-0.5.3/src/aps_toolkit/PathInfo.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     4471 2024-03-21 13:54:46.000000 aps-toolkit-0.5.3/src/aps_toolkit/ProDbReaderCad.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3505 2024-03-24 09:10:01.000000 aps-toolkit-0.5.3/src/aps_toolkit/ProDbReaderNavis.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    13555 2024-03-19 13:36:16.000000 aps-toolkit-0.5.3/src/aps_toolkit/ProDbReaderRevit.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    13105 2024-03-27 11:22:45.000000 aps-toolkit-0.5.3/src/aps_toolkit/PropReader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1376 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/Resource.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1067 2024-03-21 15:00:38.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFContent.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3333 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFGeometries.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1160 2024-03-23 03:57:09.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFImage.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1037 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFLines.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      830 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFManifestType.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      886 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFMaterialGroup.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      773 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFMaterialMap.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      834 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFMaterialMapScale.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     7567 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFMaterials.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     9759 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFMesh.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      859 2024-03-23 03:57:09.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFMetadata.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      936 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFPoints.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     6690 2024-03-23 03:57:09.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFReader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      822 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFTransform.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      799 2024-03-17 07:21:07.000000 aps-toolkit-0.5.3/src/aps_toolkit/SVFUVMap.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      983 2024-03-27 11:30:06.000000 aps-toolkit-0.5.3/src/aps_toolkit/Token.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      701 2024-03-27 11:35:19.000000 aps-toolkit-0.5.3/src/aps_toolkit/__init__.py
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 12:30:22.958648 aps-toolkit-0.5.3/src/aps_toolkit.egg-info/
--rw-r--r--   0 chuongmep   (501) staff       (20)     1908 2024-05-01 12:30:22.000000 aps-toolkit-0.5.3/src/aps_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 chuongmep   (501) staff       (20)     1722 2024-05-01 12:30:22.000000 aps-toolkit-0.5.3/src/aps_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 chuongmep   (501) staff       (20)        1 2024-05-01 12:30:22.000000 aps-toolkit-0.5.3/src/aps_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 chuongmep   (501) staff       (20)       16 2024-05-01 12:30:22.000000 aps-toolkit-0.5.3/src/aps_toolkit.egg-info/requires.txt
--rw-r--r--   0 chuongmep   (501) staff       (20)       17 2024-05-01 12:30:22.000000 aps-toolkit-0.5.3/src/aps_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 12:30:22.963023 aps-toolkit-0.5.3/src/test/
--rw-r--r--   0 chuongmep   (501) staff       (20)        0 2024-03-12 14:17:11.000000 aps-toolkit-0.5.3/src/test/__init__.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      946 2024-03-27 11:35:19.000000 aps-toolkit-0.5.3/src/test/context.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1330 2024-05-01 12:28:20.000000 aps-toolkit-0.5.3/src/test/test_auth.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     2668 2024-03-27 11:22:45.000000 aps-toolkit-0.5.3/src/test/test_bim360.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1962 2024-03-27 12:24:47.000000 aps-toolkit-0.5.3/src/test/test_bucket.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      836 2024-03-24 09:10:01.000000 aps-toolkit-0.5.3/src/test/test_db_reader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1874 2024-03-24 09:10:01.000000 aps-toolkit-0.5.3/src/test/test_derivative.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      997 2024-03-13 15:06:23.000000 aps-toolkit-0.5.3/src/test/test_fragment.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      858 2024-03-13 15:27:50.000000 aps-toolkit-0.5.3/src/test/test_geometries.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      766 2024-03-23 03:57:09.000000 aps-toolkit-0.5.3/src/test/test_image.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1233 2024-03-13 15:27:50.000000 aps-toolkit-0.5.3/src/test/test_material.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      691 2024-03-13 15:27:50.000000 aps-toolkit-0.5.3/src/test/test_mesh.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      494 2024-03-23 03:57:09.000000 aps-toolkit-0.5.3/src/test/test_metadata.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1840 2024-03-27 11:22:45.000000 aps-toolkit-0.5.3/src/test/test_prop_reader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1442 2024-03-21 13:54:46.000000 aps-toolkit-0.5.3/src/test/test_prop_reader_cad.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      777 2024-03-24 09:10:01.000000 aps-toolkit-0.5.3/src/test/test_prop_reader_navis.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3383 2024-03-12 14:17:11.000000 aps-toolkit-0.5.3/src/test/test_prop_reader_revit.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     2915 2024-03-23 03:57:09.000000 aps-toolkit-0.5.3/src/test/test_svf_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:15:07.202363 aps-toolkit-0.5.4/
+-rw-rw-rw-   0        0        0     1990 2024-05-04 09:15:07.201363 aps-toolkit-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-04 09:15:07.202363 aps-toolkit-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      902 2024-05-04 09:14:49.000000 aps-toolkit-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:15:07.158367 aps-toolkit-0.5.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 09:15:07.184364 aps-toolkit-0.5.4/src/aps_toolkit/
+-rw-rw-rw-   0        0        0     6000 2024-05-04 09:09:37.000000 aps-toolkit-0.5.4/src/aps_toolkit/Auth.py
+-rw-rw-rw-   0        0        0    10333 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/BIM360.py
+-rw-rw-rw-   0        0        0     9081 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/Bucket.py
+-rw-rw-rw-   0        0        0     2512 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/DbReader.py
+-rw-rw-rw-   0        0        0    12931 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/Derivative.py
+-rw-rw-rw-   0        0        0     3949 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/Fragments.py
+-rw-rw-rw-   0        0        0     2401 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/InputStream.py
+-rw-rw-rw-   0        0        0      905 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/ManifestItem.py
+-rw-rw-rw-   0        0        0     1164 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/MaterialProperties.py
+-rw-rw-rw-   0        0        0     1769 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/Materials.py
+-rw-rw-rw-   0        0        0     3792 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/PackFileReader.py
+-rw-rw-rw-   0        0        0      950 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/PathInfo.py
+-rw-rw-rw-   0        0        0     4586 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/ProDbReaderCad.py
+-rw-rw-rw-   0        0        0     3592 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/ProDbReaderNavis.py
+-rw-rw-rw-   0        0        0    13855 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/ProDbReaderRevit.py
+-rw-rw-rw-   0        0        0    13418 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/PropReader.py
+-rw-rw-rw-   0        0        0     1410 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/Resource.py
+-rw-rw-rw-   0        0        0     1095 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFContent.py
+-rw-rw-rw-   0        0        0     3414 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFGeometries.py
+-rw-rw-rw-   0        0        0     1190 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFImage.py
+-rw-rw-rw-   0        0        0     1063 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFLines.py
+-rw-rw-rw-   0        0        0      851 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFManifestType.py
+-rw-rw-rw-   0        0        0      910 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFMaterialGroup.py
+-rw-rw-rw-   0        0        0      793 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFMaterialMap.py
+-rw-rw-rw-   0        0        0      854 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFMaterialMapScale.py
+-rw-rw-rw-   0        0        0     7744 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFMaterials.py
+-rw-rw-rw-   0        0        0     9990 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFMesh.py
+-rw-rw-rw-   0        0        0      882 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFMetadata.py
+-rw-rw-rw-   0        0        0      959 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFPoints.py
+-rw-rw-rw-   0        0        0     6840 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFReader.py
+-rw-rw-rw-   0        0        0      844 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFTransform.py
+-rw-rw-rw-   0        0        0      819 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/SVFUVMap.py
+-rw-rw-rw-   0        0        0     1010 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/Token.py
+-rw-rw-rw-   0        0        0      721 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/aps_toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:15:07.187362 aps-toolkit-0.5.4/src/aps_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-04 09:15:06.000000 aps-toolkit-0.5.4/src/aps_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1722 2024-05-04 09:15:06.000000 aps-toolkit-0.5.4/src/aps_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 09:15:06.000000 aps-toolkit-0.5.4/src/aps_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-04 09:15:06.000000 aps-toolkit-0.5.4/src/aps_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-04 09:15:06.000000 aps-toolkit-0.5.4/src/aps_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 09:15:07.200366 aps-toolkit-0.5.4/src/test/
+-rw-rw-rw-   0        0        0        0 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/__init__.py
+-rw-rw-rw-   0        0        0      974 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/context.py
+-rw-rw-rw-   0        0        0     1367 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_auth.py
+-rw-rw-rw-   0        0        0     2734 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_bim360.py
+-rw-rw-rw-   0        0        0     2019 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_bucket.py
+-rw-rw-rw-   0        0        0      860 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_db_reader.py
+-rw-rw-rw-   0        0        0     1919 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_derivative.py
+-rw-rw-rw-   0        0        0     1022 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_fragment.py
+-rw-rw-rw-   0        0        0      879 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_geometries.py
+-rw-rw-rw-   0        0        0      786 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_image.py
+-rw-rw-rw-   0        0        0     1263 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_material.py
+-rw-rw-rw-   0        0        0      709 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_mesh.py
+-rw-rw-rw-   0        0        0      509 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_metadata.py
+-rw-rw-rw-   0        0        0     1891 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_prop_reader.py
+-rw-rw-rw-   0        0        0     1481 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_prop_reader_cad.py
+-rw-rw-rw-   0        0        0      799 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_prop_reader_navis.py
+-rw-rw-rw-   0        0        0     3472 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_prop_reader_revit.py
+-rw-rw-rw-   0        0        0     2998 2024-05-04 09:04:49.000000 aps-toolkit-0.5.4/src/test/test_svf_reader.py
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/Auth.py` & `aps-toolkit-0.5.4/src/aps_toolkit/Auth.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,141 +1,142 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import os
-import requests
-from .Token import Token
-import urllib.parse
-import webbrowser
-import requests
-import os
-from http.server import HTTPServer, BaseHTTPRequestHandler
-import http.server
-from typing import Optional
-
-
-class Auth:
-    def __init__(self, client_id: Optional[str] = None, client_secret: Optional[str] = None):
-        if client_id and client_secret:
-            self.client_id = client_id
-            self.client_secret = client_secret
-        else:
-            self.client_id = os.environ.get('APS_CLIENT_ID')
-            self.client_secret = os.environ.get('APS_CLIENT_SECRET')
-        # Initialize token variables
-        self.access_token = None
-        self.token_type = None
-        self.expires_in = None
-        self.refresh_token = None
-
-    def auth2leg(self) -> Token:
-        Host = "https://developer.api.autodesk.com"
-        url = "/authentication/v2/token"
-
-        # body
-        body = {
-            "client_id": self.client_id,
-            "client_secret": self.client_secret,
-            "grant_type": "client_credentials",
-            "scope": "data:read data:write data:search data:create bucket:read bucket:create user:read bucket:update bucket:delete code:all"
-        }
-        response = requests.post(Host + url, data=body)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        content = response.json()
-        access_token = content['access_token']
-        expires_in = content['expires_in']
-        token_type = content['token_type']
-        result = Token(access_token, token_type, expires_in)
-        return result
-
-    def auth3leg(self, callback_url=None, scopes=None) -> Token:
-        if not scopes:
-            scopes = 'data:read data:write data:create data:search bucket:create bucket:read bucket:update bucket:delete code:all'
-        if not callback_url:
-            # Default callback url
-            callback_url = "http://localhost:8080/api/auth/callback"
-
-        class CallbackHandler(BaseHTTPRequestHandler):
-            def do_GET(self):
-                nonlocal auth_instance
-                query = urllib.parse.urlparse(self.path).query
-                params = urllib.parse.parse_qs(query)
-                code = params.get('code', [''])[0]
-                if code:
-                    self.send_response(200)
-                    self.end_headers()
-                    self.wfile.write(b"Authentication successful. You can close this window now.")
-                    result_token = handle_callback(callback_url, code)
-                    auth_instance.access_token = result_token['access_token']
-                    auth_instance.token_type = result_token['token_type']
-                    auth_instance.expires_in = result_token['expires_in']
-                    auth_instance.refresh_token = result_token.get('refresh_token')
-
-                else:
-                    self.send_response(400)
-                    self.end_headers()
-                    self.wfile.write(b"Bad Request")
-
-        def handle_callback(callback_url, code):
-            tokenUrl = "https://developer.api.autodesk.com/authentication/v2/token"
-            payload = {
-                "grant_type": "authorization_code",
-                "code": code,
-                "client_id": self.client_id,
-                "client_secret": self.client_secret,
-                "redirect_uri": callback_url
-            }
-            resp = requests.post(tokenUrl, data=payload)
-            if resp.status_code != 200:
-                raise Exception(resp.content)
-            respJson = resp.json()
-            return respJson
-
-        def start_callback_server():
-            server_address = ('', 8080)
-            httpd = HTTPServer(server_address, CallbackHandler)
-            httpd.handle_request()
-
-        auth_instance = self  # Reference to the Auth instance
-
-        auth_url = f"https://developer.api.autodesk.com/authentication/v2/authorize?response_type=code&client_id={self.client_id}&redirect_uri={callback_url}&scope={scopes}"
-        webbrowser.open(auth_url)
-        start_callback_server()
-
-        # Return the token object using the global variables
-        return Token(self.access_token, self.token_type, self.expires_in, self.refresh_token)
-
-    def refresh_new_token(self, old_refresh_token) -> Token:
-        Host = "https://developer.api.autodesk.com"
-        url = "/authentication/v2/token"
-
-        # body
-        body = {
-            "client_id": self.client_id,
-            "client_secret": self.client_secret,
-            "grant_type": "refresh_token",
-            "refresh_token": old_refresh_token
-        }
-        response = requests.post(Host + url, data=body)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        content = response.json()
-        access_token = content['access_token']
-        expires_in = content['expires_in']
-        token_type = content['token_type']
-        refresh_token = content.get('refresh_token')
-        result = Token(access_token, token_type, expires_in, refresh_token)
-        return result
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+import os
+import requests
+from .Token import Token
+import urllib.parse
+import webbrowser
+import requests
+import os
+from http.server import HTTPServer, BaseHTTPRequestHandler
+import http.server
+from typing import Optional
+
+
+class Auth:
+    def __init__(self, client_id: Optional[str] = None, client_secret: Optional[str] = None):
+        if client_id and client_secret:
+            self.client_id = client_id
+            self.client_secret = client_secret
+        else:
+            self.client_id = os.environ.get('APS_CLIENT_ID')
+            self.client_secret = os.environ.get('APS_CLIENT_SECRET')
+        # Initialize token variables
+        self.access_token = None
+        self.token_type = None
+        self.expires_in = None
+        self.refresh_token = None
+
+    def auth2leg(self) -> Token:
+        Host = "https://developer.api.autodesk.com"
+        url = "/authentication/v2/token"
+
+        # body
+        body = {
+            "client_id": self.client_id,
+            "client_secret": self.client_secret,
+            "grant_type": "client_credentials",
+            "scope": "data:read data:write data:search data:create bucket:read bucket:create user:read bucket:update bucket:delete code:all"
+        }
+        response = requests.post(Host + url, data=body)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        content = response.json()
+        access_token = content['access_token']
+        expires_in = content['expires_in']
+        token_type = content['token_type']
+        result = Token(access_token, token_type, expires_in)
+        return result
+
+    def auth3leg(self, callback_url=None, scopes=None) -> Token:
+        if not scopes:
+            scopes = 'data:read data:write data:create data:search bucket:create bucket:read bucket:update bucket:delete code:all'
+        if not callback_url:
+            # Default callback url
+            callback_url = "http://localhost:8080/api/auth/callback"
+
+        class CallbackHandler(BaseHTTPRequestHandler):
+            def do_GET(self):
+                nonlocal auth_instance
+                query = urllib.parse.urlparse(self.path).query
+                params = urllib.parse.parse_qs(query)
+                code = params.get('code', [''])[0]
+                if code:
+                    self.send_response(200)
+                    self.end_headers()
+                    self.wfile.write(b"Authentication successful. You can close this window now.")
+                    result_token = handle_callback(callback_url, code)
+                    auth_instance.access_token = result_token['access_token']
+                    auth_instance.token_type = result_token['token_type']
+                    auth_instance.expires_in = result_token['expires_in']
+                    auth_instance.refresh_token = result_token.get('refresh_token')
+
+                else:
+                    self.send_response(400)
+                    self.end_headers()
+                    self.wfile.write(b"Bad Request")
+
+        def handle_callback(callback_url, code):
+            tokenUrl = "https://developer.api.autodesk.com/authentication/v2/token"
+            payload = {
+                "grant_type": "authorization_code",
+                "code": code,
+                "client_id": self.client_id,
+                "client_secret": self.client_secret,
+                "redirect_uri": callback_url
+            }
+            resp = requests.post(tokenUrl, data=payload)
+            if resp.status_code != 200:
+                raise Exception(resp.content)
+            respJson = resp.json()
+            return respJson
+
+        def start_callback_server(callback_url):
+            parsed_url = urllib.parse.urlparse(callback_url)
+            server_address = ('', parsed_url.port if parsed_url.port else 8080)
+            httpd = HTTPServer(server_address, CallbackHandler)
+            httpd.handle_request()
+
+        auth_instance = self  # Reference to the Auth instance
+
+        auth_url = f"https://developer.api.autodesk.com/authentication/v2/authorize?response_type=code&client_id={self.client_id}&redirect_uri={callback_url}&scope={scopes}"
+        webbrowser.open(auth_url)
+        start_callback_server(callback_url)
+
+        # Return the token object using the global variables
+        return Token(self.access_token, self.token_type, self.expires_in, self.refresh_token)
+
+    def refresh_new_token(self, old_refresh_token) -> Token:
+        Host = "https://developer.api.autodesk.com"
+        url = "/authentication/v2/token"
+
+        # body
+        body = {
+            "client_id": self.client_id,
+            "client_secret": self.client_secret,
+            "grant_type": "refresh_token",
+            "refresh_token": old_refresh_token
+        }
+        response = requests.post(Host + url, data=body)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        content = response.json()
+        access_token = content['access_token']
+        expires_in = content['expires_in']
+        token_type = content['token_type']
+        refresh_token = content.get('refresh_token')
+        result = Token(access_token, token_type, expires_in, refresh_token)
+        return result
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/BIM360.py` & `aps-toolkit-0.5.4/src/aps_toolkit/BIM360.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,199 +1,199 @@
-﻿"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import requests
-import pandas as pd
-from .Auth import Auth
-
-
-class BIM360:
-    def __init__(self, token=None):
-        self.token = token
-        if self.token is None:
-            auth = Auth()
-            self.token = auth.auth2leg()
-        self.host = "https://developer.api.autodesk.com"
-
-    def get_hubs(self):
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        url = f"{self.host}/project/v1/hubs"
-        response = requests.get(url, headers=headers)
-        if response.status_code == 200:
-            return response.json()
-        else:
-            raise Exception(response.content)
-
-    def get_projects(self, hub_id):
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        url = f"{self.host}/project/v1/hubs/{hub_id}/projects"
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        return response.json()
-
-    def get_top_folders(self, hub_id, project_id):
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        url = f"{self.host}/project/v1/hubs/{hub_id}/projects/{project_id}/topFolders"
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        return response.json()
-
-    def get_top_folder_project_files(self, hub_id, project_id):
-        data = self.get_top_folders(hub_id, project_id)
-        for item in data['data']:
-            if item['attributes']['name'] == "Project Files":
-                return item
-        return None
-
-    def get_folder_contents(self, project_id, folder_id):
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        url = f"{self.host}/data/v1/projects/{project_id}/folders/{folder_id}/contents"
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        return response.json()
-
-    def get_item_versions(self, project_id, item_id):
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}/versions"
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        return response.json()
-
-    def get_item_info(self, project_id, item_id):
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}"
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        return response.json()
-
-    def batch_report_projects(self, hub_id) -> pd.DataFrame:
-        df = pd.DataFrame(columns=['project_id', 'project_name', "project_type", 'top_folder_id'])
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        url = f"{self.host}/project/v1/hubs/{hub_id}/projects"
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        projects = response.json()
-        for project in projects['data']:
-            project_id = project['id']
-            project_name = project['attributes']['name']
-            project_type = project['attributes']['extension']["data"]["projectType"]
-            top_folder = self.get_top_folders(hub_id, project_id)
-            top_folder_id = top_folder["data"][0]["id"]
-            df = pd.concat([df, pd.DataFrame(
-                {'project_id': project_id, 'project_name': project_name, 'project_type': project_type,
-                 'top_folder_id': top_folder_id}, index=[0])], ignore_index=True)
-        return df
-
-    def batch_report_item_versions(self, project_id, item_id) -> pd.DataFrame:
-        # create a dataframe to save data report with columns : item_id,version,derivative_urn,last_modified_time
-        df = pd.DataFrame(columns=['item_id', 'version', 'derivative_urn', 'last_modified_time'])
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}/versions"
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        item_versions = response.json()
-        for item_version in item_versions['data']:
-            version = item_version['attributes']['versionNumber']
-            # check if item_version have derivatives
-            if 'derivatives' not in item_version['relationships']:
-                continue
-            derivative_urn = item_version['relationships']['derivatives']['data']['id']
-            last_modified_time = item_version['attributes']['lastModifiedTime']
-            df = pd.concat([df, pd.DataFrame({'item_id': item_id, 'version': version, 'derivative_urn': derivative_urn,
-                                              'last_modified_time': last_modified_time}, index=[0])], ignore_index=True)
-        return df
-
-    def get_item_display_name(self, project_id, item_id):
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}"
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        item = response.json()
-        return item['data']['attributes']['displayName']
-
-    def batch_report_items(self, project_id, folder_id, extension=".rvt", is_sub_folder=False) -> pd.DataFrame:
-        df = pd.DataFrame(columns=['project_id', 'folder_id', 'item_name', 'item_id', 'last_version', 'derivative_urn',
-                                   'last_modified_time'])
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        url = f"{self.host}/data/v1/projects/{project_id}/folders/{folder_id}/contents"
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        folder_contents = response.json()
-        for folder_content in folder_contents['data']:
-            if folder_content['type'] == "items":
-                item_id = folder_content['id']
-                item_name = folder_content['attributes']['displayName']
-                if not item_name.endswith(extension):
-                    continue
-                item_versions = self._get_latest_version(project_id, item_id)
-                # getfrom dict with keys : version
-                last_version = item_versions["version"]
-                derivative_urn = item_versions["derivative_urn"]
-                last_modified_time = folder_content['attributes']['lastModifiedTime']
-                df = pd.concat([df, pd.DataFrame(
-                    {'project_id': project_id, 'folder_id': folder_id, 'item_name': item_name, 'item_id': item_id,
-                     'last_version': last_version, 'derivative_urn': derivative_urn,
-                     'last_modified_time': last_modified_time}, index=[0])], ignore_index=True)
-            elif folder_content['type'] == "folders" and is_sub_folder:
-                if is_sub_folder:
-                    df = pd.concat(
-                        [df, self.batch_report_items(project_id, folder_content['id'], extension, is_sub_folder)],
-                        ignore_index=True)
-        return df
-
-    def _get_number_latest_item_version(self, project_id, item_id) -> int:
-        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}/versions"
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        item_versions = response.json()
-        return len(item_versions['data'])
-
-    def _get_latest_version(self, project_id, item_id) -> dict:
-        # dict with keys : version,derivative_urn,last_modified_time
-        latest_version = {}
-        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}/versions"
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        item_versions = response.json()
-        # add to latest_version
-        latest_version['version'] = item_versions['data'][0]['attributes']['versionNumber']
-        latest_version['last_modified_time'] = item_versions['data'][0]['attributes']['lastModifiedTime']
-        latest_version['derivative_urn'] = item_versions['data'][0]['relationships']['derivatives']['data']['id']
-        return latest_version
-
-    def get_urn_item_version(self, project_id, item_id, version):
-        headers = {'Authorization': 'Bearer ' + self.token.access_token}
-        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}/versions"
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        item_versions = response.json()
-        for item_version in item_versions['data']:
-            if item_version['attributes']['versionNumber'] == version:
-                return item_version['relationships']['derivatives']['data']['id']
-        return None
+﻿"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+import requests
+import pandas as pd
+from .Auth import Auth
+
+
+class BIM360:
+    def __init__(self, token=None):
+        self.token = token
+        if self.token is None:
+            auth = Auth()
+            self.token = auth.auth2leg()
+        self.host = "https://developer.api.autodesk.com"
+
+    def get_hubs(self):
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/project/v1/hubs"
+        response = requests.get(url, headers=headers)
+        if response.status_code == 200:
+            return response.json()
+        else:
+            raise Exception(response.content)
+
+    def get_projects(self, hub_id):
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/project/v1/hubs/{hub_id}/projects"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        return response.json()
+
+    def get_top_folders(self, hub_id, project_id):
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/project/v1/hubs/{hub_id}/projects/{project_id}/topFolders"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        return response.json()
+
+    def get_top_folder_project_files(self, hub_id, project_id):
+        data = self.get_top_folders(hub_id, project_id)
+        for item in data['data']:
+            if item['attributes']['name'] == "Project Files":
+                return item
+        return None
+
+    def get_folder_contents(self, project_id, folder_id):
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/data/v1/projects/{project_id}/folders/{folder_id}/contents"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        return response.json()
+
+    def get_item_versions(self, project_id, item_id):
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}/versions"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        return response.json()
+
+    def get_item_info(self, project_id, item_id):
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        return response.json()
+
+    def batch_report_projects(self, hub_id) -> pd.DataFrame:
+        df = pd.DataFrame(columns=['project_id', 'project_name', "project_type", 'top_folder_id'])
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/project/v1/hubs/{hub_id}/projects"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        projects = response.json()
+        for project in projects['data']:
+            project_id = project['id']
+            project_name = project['attributes']['name']
+            project_type = project['attributes']['extension']["data"]["projectType"]
+            top_folder = self.get_top_folders(hub_id, project_id)
+            top_folder_id = top_folder["data"][0]["id"]
+            df = pd.concat([df, pd.DataFrame(
+                {'project_id': project_id, 'project_name': project_name, 'project_type': project_type,
+                 'top_folder_id': top_folder_id}, index=[0])], ignore_index=True)
+        return df
+
+    def batch_report_item_versions(self, project_id, item_id) -> pd.DataFrame:
+        # create a dataframe to save data report with columns : item_id,version,derivative_urn,last_modified_time
+        df = pd.DataFrame(columns=['item_id', 'version', 'derivative_urn', 'last_modified_time'])
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}/versions"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        item_versions = response.json()
+        for item_version in item_versions['data']:
+            version = item_version['attributes']['versionNumber']
+            # check if item_version have derivatives
+            if 'derivatives' not in item_version['relationships']:
+                continue
+            derivative_urn = item_version['relationships']['derivatives']['data']['id']
+            last_modified_time = item_version['attributes']['lastModifiedTime']
+            df = pd.concat([df, pd.DataFrame({'item_id': item_id, 'version': version, 'derivative_urn': derivative_urn,
+                                              'last_modified_time': last_modified_time}, index=[0])], ignore_index=True)
+        return df
+
+    def get_item_display_name(self, project_id, item_id):
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        item = response.json()
+        return item['data']['attributes']['displayName']
+
+    def batch_report_items(self, project_id, folder_id, extension=".rvt", is_sub_folder=False) -> pd.DataFrame:
+        df = pd.DataFrame(columns=['project_id', 'folder_id', 'item_name', 'item_id', 'last_version', 'derivative_urn',
+                                   'last_modified_time'])
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/data/v1/projects/{project_id}/folders/{folder_id}/contents"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        folder_contents = response.json()
+        for folder_content in folder_contents['data']:
+            if folder_content['type'] == "items":
+                item_id = folder_content['id']
+                item_name = folder_content['attributes']['displayName']
+                if not item_name.endswith(extension):
+                    continue
+                item_versions = self._get_latest_version(project_id, item_id)
+                # getfrom dict with keys : version
+                last_version = item_versions["version"]
+                derivative_urn = item_versions["derivative_urn"]
+                last_modified_time = folder_content['attributes']['lastModifiedTime']
+                df = pd.concat([df, pd.DataFrame(
+                    {'project_id': project_id, 'folder_id': folder_id, 'item_name': item_name, 'item_id': item_id,
+                     'last_version': last_version, 'derivative_urn': derivative_urn,
+                     'last_modified_time': last_modified_time}, index=[0])], ignore_index=True)
+            elif folder_content['type'] == "folders" and is_sub_folder:
+                if is_sub_folder:
+                    df = pd.concat(
+                        [df, self.batch_report_items(project_id, folder_content['id'], extension, is_sub_folder)],
+                        ignore_index=True)
+        return df
+
+    def _get_number_latest_item_version(self, project_id, item_id) -> int:
+        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}/versions"
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        item_versions = response.json()
+        return len(item_versions['data'])
+
+    def _get_latest_version(self, project_id, item_id) -> dict:
+        # dict with keys : version,derivative_urn,last_modified_time
+        latest_version = {}
+        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}/versions"
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        item_versions = response.json()
+        # add to latest_version
+        latest_version['version'] = item_versions['data'][0]['attributes']['versionNumber']
+        latest_version['last_modified_time'] = item_versions['data'][0]['attributes']['lastModifiedTime']
+        latest_version['derivative_urn'] = item_versions['data'][0]['relationships']['derivatives']['data']['id']
+        return latest_version
+
+    def get_urn_item_version(self, project_id, item_id, version):
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}/versions"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        item_versions = response.json()
+        for item_version in item_versions['data']:
+            if item_version['attributes']['versionNumber'] == version:
+                return item_version['relationships']['derivatives']['data']['id']
+        return None
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/Bucket.py` & `aps-toolkit-0.5.4/src/aps_toolkit/Bucket.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-from enum import Enum
-import pandas as pd
-import requests
-from .Token import Token
-
-
-class PublicKey(Enum):
-    transient = "transient"
-    temporary = "temporary"
-    persistent = "persistent"
-
-
-class Bucket:
-    def __init__(self, token: Token, region="US"):
-        self.token = token
-        self.region = region
-        self.host = "https://developer.api.autodesk.com/oss/v2/buckets"
-
-    def get_all_buckets(self) -> pd.DataFrame:
-        """
-          Retrieves all the buckets from the Autodesk OSS API.
-
-          This method sends a GET request to the Autodesk OSS API and includes an Authorization header with a bearer token for authentication. If the response status code is not 200, it raises an exception with the response content.
-
-          If the request is successful, it processes the JSON response to create a pandas DataFrame. The 'createdDate' field, which is in milliseconds since epoch, is converted to a real date and updated in the DataFrame.
-
-          Returns:
-              pd.DataFrame: A DataFrame containing all the buckets.
-          """
-        headers = {
-            "Authorization": f"Bearer {self.token.access_token}"
-        }
-        response = requests.get(self.host, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        data = response.json()
-        df = pd.DataFrame(data["items"])
-        milliseconds_since_epoch = df["createdDate"]
-        seconds_since_epoch = milliseconds_since_epoch // 1000
-        real_date = pd.to_datetime(seconds_since_epoch, unit="s")
-        df["createdDate"] = real_date
-        return df
-
-    def create_bucket(self, bucket_name: str, policy_key: PublicKey) -> dict:
-        """
-            Creates a new bucket in the Autodesk OSS API.
-
-            This method sends a POST request to the Autodesk OSS API. It includes an Authorization header with a
-            bearer token for authentication and a Content-Type header set to "application/json". The bucket name and
-            policy key are passed in the body of the request as JSON data. If the response status code is not 200,
-            it raises an exception with the response content.
-
-            Args: bucket_name (str): The name of the bucket to be created. policy_key (PublicKey): The policy key for
-            the bucket. It can be one of the following: 'transient', 'temporary', or 'persistent'.
-
-            Returns:
-                dict: A dictionary containing the response from the Autodesk OSS API.
-            """
-        headers = {
-            "Authorization": f"Bearer {self.token.access_token}",
-            "Content-Type": "application/json"
-        }
-        data = {
-            "bucketKey": bucket_name,
-            "policyKey": policy_key.value
-        }
-        response = requests.post(self.host, headers=headers, json=data)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        return response.json()
-
-    def delete_bucket(self, bucket_name: str) -> dict:
-        """
-            Deletes a bucket in the Autodesk OSS API.
-
-            This method sends a DELETE request to the Autodesk OSS API. It includes an Authorization header with a bearer token for authentication. The bucket name is passed in the URL of the request. If the response status code is not 200, it raises an exception with the response content.
-
-            Args:
-                bucket_name (str): The name of the bucket to be deleted.
-
-            Returns:
-                dict: A dictionary containing the response from the Autodesk OSS API.
-            """
-        headers = {
-            "Authorization": f"Bearer {self.token.access_token}"
-        }
-        url = f"{self.host}/{bucket_name}"
-        response = requests.delete(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        return response.content
-
-    def get_objects(self, bucket_name: str) -> pd.DataFrame:
-        """
-          Retrieves all the objects in a specified bucket from the Autodesk OSS API.
-
-          This method sends a GET request to the Autodesk OSS API. It includes an Authorization header with a bearer token for authentication. The bucket name is passed in the URL of the request. If the response status code is not 200, it raises an exception with the response content.
-
-          Args:
-              bucket_name (str): The name of the bucket from which to retrieve objects.
-
-          Returns:
-              pd.DataFrame: A DataFrame containing all the objects in the specified bucket.
-          """
-        headers = {
-            "Authorization": f"Bearer {self.token.access_token}"
-        }
-        url = f"{self.host}/{bucket_name}/objects"
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        data = response.json()
-        df = pd.DataFrame(data["items"])
-        return df
-
-    def upload_object(self, bucket_name: str, file_path: str, object_name: str) -> dict:
-        """
-           Uploads an object to a specified bucket in the Autodesk OSS API.
-
-           This method sends a PUT request to the Autodesk OSS API. It includes an Authorization header with a bearer token for authentication and a Content-Type header set to "application/octet-stream". The bucket name and object name are passed in the URL of the request, and the file to be uploaded is passed in the body of the request as binary data. If the response status code is not 200, it raises an exception with the response content.
-
-           Args:
-               bucket_name (str): The name of the bucket to which the object will be uploaded.
-               file_path (str): The path of the file to be uploaded.
-               object_name (str): The name of the object to be created in the bucket.
-
-           Returns:
-               dict: A dictionary containing the response from the Autodesk OSS API.
-           """
-        headers = {
-            "Authorization": f"Bearer {self.token.access_token}",
-            "Content-Type": "application/octet-stream"
-        }
-        url = f"{self.host}/{bucket_name}/objects/{object_name}"
-        with open(file_path, "rb") as file:
-            response = requests.put(url, headers=headers, data=file)
-            if response.status_code != 200:
-                raise Exception(response.content)
-            return response.json()
-
-    def delete_object(self, bucket_name: str, object_name: str) -> dict:
-        """
-            Deletes an object from a specified bucket in the Autodesk OSS API.
-
-            This method sends a DELETE request to the Autodesk OSS API. It includes an Authorization header with a bearer token for authentication. The bucket name and object name are passed in the URL of the request. If the response status code is not 200, it raises an exception with the response content.
-
-            Args:
-                bucket_name (str): The name of the bucket from which the object will be deleted.
-                object_name (str): The name of the object to be deleted.
-
-            Returns:
-                dict: A dictionary containing the response from the Autodesk OSS API.
-            """
-        headers = {
-            "Authorization": f"Bearer {self.token.access_token}"
-        }
-        url = f"{self.host}/{bucket_name}/objects/{object_name}"
-        response = requests.delete(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        return response.content
-
-    def download_object(self, bucket_name: str, object_name: str, file_path: str) -> None:
-        """
-            Downloads an object from a specified bucket in the Autodesk OSS API.
-
-            This method sends a GET request to the Autodesk OSS API. It includes an Authorization header with a bearer token for authentication. The bucket name and object name are passed in the URL of the request. If the response status code is not 200, it raises an exception with the response content.
-
-            The downloaded content is written to a file at the specified file path.
-
-            Args:
-                bucket_name (str): The name of the bucket from which the object will be downloaded.
-                object_name (str): The name of the object to be downloaded.
-                file_path (str): The path where the downloaded file will be saved.
-
-            Returns:
-                None
-            """
-        headers = {
-            "Authorization": f"Bearer {self.token.access_token}"
-        }
-        url = f"{self.host}/{bucket_name}/objects/{object_name}"
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        with open(file_path, "wb") as file:
-            file.write(response.content)
-            file.close()
-        return None
+from enum import Enum
+import pandas as pd
+import requests
+from .Token import Token
+
+
+class PublicKey(Enum):
+    transient = "transient"
+    temporary = "temporary"
+    persistent = "persistent"
+
+
+class Bucket:
+    def __init__(self, token: Token, region="US"):
+        self.token = token
+        self.region = region
+        self.host = "https://developer.api.autodesk.com/oss/v2/buckets"
+
+    def get_all_buckets(self) -> pd.DataFrame:
+        """
+          Retrieves all the buckets from the Autodesk OSS API.
+
+          This method sends a GET request to the Autodesk OSS API and includes an Authorization header with a bearer token for authentication. If the response status code is not 200, it raises an exception with the response content.
+
+          If the request is successful, it processes the JSON response to create a pandas DataFrame. The 'createdDate' field, which is in milliseconds since epoch, is converted to a real date and updated in the DataFrame.
+
+          Returns:
+              pd.DataFrame: A DataFrame containing all the buckets.
+          """
+        headers = {
+            "Authorization": f"Bearer {self.token.access_token}"
+        }
+        response = requests.get(self.host, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        data = response.json()
+        df = pd.DataFrame(data["items"])
+        milliseconds_since_epoch = df["createdDate"]
+        seconds_since_epoch = milliseconds_since_epoch // 1000
+        real_date = pd.to_datetime(seconds_since_epoch, unit="s")
+        df["createdDate"] = real_date
+        return df
+
+    def create_bucket(self, bucket_name: str, policy_key: PublicKey) -> dict:
+        """
+            Creates a new bucket in the Autodesk OSS API.
+
+            This method sends a POST request to the Autodesk OSS API. It includes an Authorization header with a
+            bearer token for authentication and a Content-Type header set to "application/json". The bucket name and
+            policy key are passed in the body of the request as JSON data. If the response status code is not 200,
+            it raises an exception with the response content.
+
+            Args: bucket_name (str): The name of the bucket to be created. policy_key (PublicKey): The policy key for
+            the bucket. It can be one of the following: 'transient', 'temporary', or 'persistent'.
+
+            Returns:
+                dict: A dictionary containing the response from the Autodesk OSS API.
+            """
+        headers = {
+            "Authorization": f"Bearer {self.token.access_token}",
+            "Content-Type": "application/json"
+        }
+        data = {
+            "bucketKey": bucket_name,
+            "policyKey": policy_key.value
+        }
+        response = requests.post(self.host, headers=headers, json=data)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        return response.json()
+
+    def delete_bucket(self, bucket_name: str) -> dict:
+        """
+            Deletes a bucket in the Autodesk OSS API.
+
+            This method sends a DELETE request to the Autodesk OSS API. It includes an Authorization header with a bearer token for authentication. The bucket name is passed in the URL of the request. If the response status code is not 200, it raises an exception with the response content.
+
+            Args:
+                bucket_name (str): The name of the bucket to be deleted.
+
+            Returns:
+                dict: A dictionary containing the response from the Autodesk OSS API.
+            """
+        headers = {
+            "Authorization": f"Bearer {self.token.access_token}"
+        }
+        url = f"{self.host}/{bucket_name}"
+        response = requests.delete(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        return response.content
+
+    def get_objects(self, bucket_name: str) -> pd.DataFrame:
+        """
+          Retrieves all the objects in a specified bucket from the Autodesk OSS API.
+
+          This method sends a GET request to the Autodesk OSS API. It includes an Authorization header with a bearer token for authentication. The bucket name is passed in the URL of the request. If the response status code is not 200, it raises an exception with the response content.
+
+          Args:
+              bucket_name (str): The name of the bucket from which to retrieve objects.
+
+          Returns:
+              pd.DataFrame: A DataFrame containing all the objects in the specified bucket.
+          """
+        headers = {
+            "Authorization": f"Bearer {self.token.access_token}"
+        }
+        url = f"{self.host}/{bucket_name}/objects"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        data = response.json()
+        df = pd.DataFrame(data["items"])
+        return df
+
+    def upload_object(self, bucket_name: str, file_path: str, object_name: str) -> dict:
+        """
+           Uploads an object to a specified bucket in the Autodesk OSS API.
+
+           This method sends a PUT request to the Autodesk OSS API. It includes an Authorization header with a bearer token for authentication and a Content-Type header set to "application/octet-stream". The bucket name and object name are passed in the URL of the request, and the file to be uploaded is passed in the body of the request as binary data. If the response status code is not 200, it raises an exception with the response content.
+
+           Args:
+               bucket_name (str): The name of the bucket to which the object will be uploaded.
+               file_path (str): The path of the file to be uploaded.
+               object_name (str): The name of the object to be created in the bucket.
+
+           Returns:
+               dict: A dictionary containing the response from the Autodesk OSS API.
+           """
+        headers = {
+            "Authorization": f"Bearer {self.token.access_token}",
+            "Content-Type": "application/octet-stream"
+        }
+        url = f"{self.host}/{bucket_name}/objects/{object_name}"
+        with open(file_path, "rb") as file:
+            response = requests.put(url, headers=headers, data=file)
+            if response.status_code != 200:
+                raise Exception(response.content)
+            return response.json()
+
+    def delete_object(self, bucket_name: str, object_name: str) -> dict:
+        """
+            Deletes an object from a specified bucket in the Autodesk OSS API.
+
+            This method sends a DELETE request to the Autodesk OSS API. It includes an Authorization header with a bearer token for authentication. The bucket name and object name are passed in the URL of the request. If the response status code is not 200, it raises an exception with the response content.
+
+            Args:
+                bucket_name (str): The name of the bucket from which the object will be deleted.
+                object_name (str): The name of the object to be deleted.
+
+            Returns:
+                dict: A dictionary containing the response from the Autodesk OSS API.
+            """
+        headers = {
+            "Authorization": f"Bearer {self.token.access_token}"
+        }
+        url = f"{self.host}/{bucket_name}/objects/{object_name}"
+        response = requests.delete(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        return response.content
+
+    def download_object(self, bucket_name: str, object_name: str, file_path: str) -> None:
+        """
+            Downloads an object from a specified bucket in the Autodesk OSS API.
+
+            This method sends a GET request to the Autodesk OSS API. It includes an Authorization header with a bearer token for authentication. The bucket name and object name are passed in the URL of the request. If the response status code is not 200, it raises an exception with the response content.
+
+            The downloaded content is written to a file at the specified file path.
+
+            Args:
+                bucket_name (str): The name of the bucket from which the object will be downloaded.
+                object_name (str): The name of the object to be downloaded.
+                file_path (str): The path where the downloaded file will be saved.
+
+            Returns:
+                None
+            """
+        headers = {
+            "Authorization": f"Bearer {self.token.access_token}"
+        }
+        url = f"{self.host}/{bucket_name}/objects/{object_name}"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        with open(file_path, "wb") as file:
+            file.write(response.content)
+            file.close()
+        return None
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/DbReader.py` & `aps-toolkit-0.5.4/src/aps_toolkit/DbReader.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import os
-import requests
-from .Auth import Auth
-import pandas as pd
-import sqlite3
-
-
-class DbReader:
-    def __init__(self, urn, token=None):
-        self.urn = urn
-        if token is None:
-            auth = Auth()
-            self.token = auth.auth2leg()
-        else:
-            self.token = token
-        self.host = "https://developer.api.autodesk.com"
-        url = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest"
-        headers = {
-            "Authorization": f"Bearer {self.token.access_token}"
-        }
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            raise Exception(response.content)
-        json_response = response.json()
-        if json_response["status"] != "success":
-            raise Exception(json_response)
-        childrens = json_response['derivatives'][0]["children"]
-        self.path = ""
-        for child in childrens:
-            if child["type"] == "resource" and child["mime"] == "application/autodesk-db":
-                self.path = child["urn"]
-                break
-        url = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest/{self.path}"
-        response = requests.get(url, headers=headers)
-        temp_path = os.path.join(os.path.dirname(__file__), "database")
-        extension = self.path.split(".")[-1]
-        temp_path = os.path.join(temp_path, self.urn + "." + extension)
-        self.db_path = temp_path
-        if not os.path.exists(temp_path):
-            os.makedirs(os.path.dirname(temp_path), exist_ok=True)
-        with open(temp_path, "wb") as file:
-            file.write(response.content)
-            file.close()
-
-    def execute_query(self, query):
-        conn = sqlite3.connect(self.db_path)
-        return pd.read_sql_query(query, conn)
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+import os
+import requests
+from .Auth import Auth
+import pandas as pd
+import sqlite3
+
+
+class DbReader:
+    def __init__(self, urn, token=None):
+        self.urn = urn
+        if token is None:
+            auth = Auth()
+            self.token = auth.auth2leg()
+        else:
+            self.token = token
+        self.host = "https://developer.api.autodesk.com"
+        url = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest"
+        headers = {
+            "Authorization": f"Bearer {self.token.access_token}"
+        }
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        json_response = response.json()
+        if json_response["status"] != "success":
+            raise Exception(json_response)
+        childrens = json_response['derivatives'][0]["children"]
+        self.path = ""
+        for child in childrens:
+            if child["type"] == "resource" and child["mime"] == "application/autodesk-db":
+                self.path = child["urn"]
+                break
+        url = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest/{self.path}"
+        response = requests.get(url, headers=headers)
+        temp_path = os.path.join(os.path.dirname(__file__), "database")
+        extension = self.path.split(".")[-1]
+        temp_path = os.path.join(temp_path, self.urn + "." + extension)
+        self.db_path = temp_path
+        if not os.path.exists(temp_path):
+            os.makedirs(os.path.dirname(temp_path), exist_ok=True)
+        with open(temp_path, "wb") as file:
+            file.write(response.content)
+            file.close()
+
+    def execute_query(self, query):
+        conn = sqlite3.connect(self.db_path)
+        return pd.read_sql_query(query, conn)
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/Derivative.py` & `aps-toolkit-0.5.4/src/aps_toolkit/Derivative.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,327 +1,327 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import requests
-import gzip
-from io import BytesIO
-import zipfile
-from json import loads as json_loads
-from typing import List
-from urllib.parse import unquote, quote, urljoin
-import re
-from os.path import join, normpath
-import os
-from .PathInfo import PathInfo
-from .Resource import Resource
-from .ManifestItem import ManifestItem
-import json
-
-
-class Derivative:
-    def __init__(self, urn, token, region="US"):
-        self.urn = urn
-        self.token = token
-        self.region = region
-        self.host = "https://developer.api.autodesk.com"
-
-    def translate_job(self, root_file_name, type="svf", generate_master_views=False):
-        url = "https://developer.api.autodesk.com/modelderivative/v2/designdata/job"
-        access_token = self.token.access_token
-        if not access_token:
-            raise Exception("Have no access token to translate job.")
-        payload = json.dumps({
-            "input": {
-                "urn": self.urn,
-                "rootFilename": root_file_name
-            },
-            "output": {
-                "destination": {
-                    "region": self.region.lower()
-                },
-                "formats": [
-                    {
-                        "type": type,
-                        "views": [
-                            "2d",
-                            "3d"
-                        ],
-                        "advanced": {
-                            "generateMasterViews": generate_master_views
-                        }
-                    }
-                ]
-            }
-        })
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Authorization': 'Bearer ' + access_token,
-            'x-ads-force': 'true'
-        }
-        response = requests.post(url, headers=headers, data=payload)
-        return response.text
-
-    def check_job_status(self):
-        url = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest"
-        access_token = self.token.access_token
-        if not access_token:
-            raise Exception("Have no access token to check job status.")
-        headers = {
-            "Authorization": f"Bearer {access_token}",
-            "region": self.region
-        }
-        response = requests.get(url, headers=headers)
-        return response.json()
-
-    def read_svf_manifest_items(self) -> List[ManifestItem]:
-        """
-        Reads SVF manifest items associated with the URN.
-
-        Returns:
-        List[ManifestItem]: A list of SVF manifest items.
-        """
-        URL = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest"
-        access_token = self.token.access_token
-        if not access_token:
-            raise Exception("Have no access token to get manifest items.")
-        headers = {
-            "Authorization": f"Bearer {access_token}",
-            "region": self.region
-        }
-        # request
-        response = requests.get(URL, headers=headers)
-        if response.status_code == 404:
-            raise Exception(response.content)
-        json_response = response.json()
-        children = json_response['derivatives'][0]["children"]
-        manifest_items = []
-        image_items = []
-        for child in children:
-            if child["type"] == "geometry":
-                for c in child["children"]:
-                    # check if contains 'mime' and 'application/autodesk-svf
-                    if "mime" in c and c["mime"] == "application/autodesk-svf":
-                        urn_json = c["urn"]
-                        json_content = self._unzip_svf(urn_json)
-                        path_info = self._decompose_urn(urn_json)
-                        path_info.files = self._get_assets(json_content)
-                        guid = c["guid"]
-                        mime = c["mime"]
-                        # add svf files
-                        path_info.files.append(path_info.root_file_name)
-                        manifest_items.append(ManifestItem(guid, mime, path_info, urn_json))
-                    # case mapping image with svf
-                    if "type" in c and c["role"] == "thumbnail":
-                        guid = c["guid"]
-                        mime = c["mime"]
-                        urn = c["urn"]
-                        path_info = self._decompose_urn(urn)
-                        image_items.append(ManifestItem(guid, mime, path_info, urn))
-        # add files images to manifest items by mapp with local_path
-        for image in image_items:
-            for manifest_item in manifest_items:
-                if image.path_info.local_path == manifest_item.path_info.local_path:
-                    manifest_item.path_info.files.append(image.path_info.root_file_name)
-                    continue
-        return manifest_items
-
-    def read_svf_resource_item(self, manifest_item) -> List[Resource]:
-        """
-        Reads SVF resource items from the manifest item.
-
-        Parameters:
-        manifest_item (ManifestItem): The manifest item containing information about SVF resources.
-
-        Returns:
-        List[Resource]: A list of SVF resource items extracted from the manifest item.
-        """
-        resources = []
-        derivative_path = "derivativeservice/v2/derivatives/"
-        for file in manifest_item.path_info.files:
-            file_name = file[file.rfind("/") + 1:]
-            uri_local_path = "file://" + manifest_item.path_info.local_path + file
-            local_path = unquote(uri_local_path)[len("file://"):]
-            # Normalize the path to remove /../../
-            local_path = normpath(local_path)
-            myUri = "file://" + manifest_item.path_info.base_path + file
-            remote_path = join(derivative_path, unquote(myUri)[len("file://"):])
-            remote_path = normpath(remote_path)
-            resources.append(Resource(file_name, remote_path, local_path))
-        return resources
-
-    def read_svf_resource(self) -> dict[str, List[Resource]]:
-        """
-        Reads SVF resources from the SVF manifest items.
-
-        Returns:
-        List[Resource]: A list of resources extracted from the SVF manifest.
-        """
-        manifest_items = self.read_svf_manifest_items()
-        resources = {}
-        for manifest_item in manifest_items:
-            source_items = self.read_svf_resource_item(manifest_item)
-            resources[manifest_item.guid] = source_items
-        return resources
-
-    def _unzip_svf(self, svf_urn):
-        """
-        Retrieves and unzips the manifest associated with the given URN.
-
-        Parameters:
-        urn (str): The URN of the manifest to retrieve and unzip.
-
-        Returns:
-        dict: The contents of the unzipped manifest in JSON format.
-        """
-        URL = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest/{svf_urn}"
-        access_token = self.token.access_token
-        headers = {
-            "Authorization": f"Bearer {access_token}",
-            "region": self.region
-        }
-        response = requests.get(URL, headers=headers)
-        if response.status_code == 404:
-            raise Exception(response.content)
-        manifest_json = None
-        # unzip it
-        if ".gz" in response.headers.get("Content-Type", ""):
-            with gzip.GzipFile(fileobj=BytesIO(response.content), mode="rb") as gzip_file:
-                manifest_json = json_loads(gzip_file.read().decode("utf-8"))
-        else:
-            with zipfile.ZipFile(BytesIO(response.content)) as zip_file:
-                with zip_file.open("manifest.json") as manifest_data:
-                    manifest_json = json_loads(manifest_data.read().decode("utf-8"))
-
-        return manifest_json
-
-    def read_svf_metadata(self, svf_urn):
-        """
-        Retrieves and unzips the manifest associated with the given URN.
-
-        Parameters:
-        urn (str): The URN of the manifest to retrieve and unzip.
-
-        Returns:
-        dict: The contents of the unzipped manifest in JSON format.
-        """
-        URL = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest/{svf_urn}"
-        access_token = self.token.access_token
-        headers = {
-            "Authorization": f"Bearer {access_token}",
-            "region": self.region
-        }
-        response = requests.get(URL, headers=headers)
-        if response.status_code == 404:
-            raise Exception(response.content)
-        meta_data_json = None
-        # unzip it
-        if ".gz" in response.headers.get("Content-Type", ""):
-            with gzip.GzipFile(fileobj=BytesIO(response.content), mode="rb") as gzip_file:
-                meta_data_json = json_loads(gzip_file.read().decode("utf-8"))
-        else:
-            with zipfile.ZipFile(BytesIO(response.content)) as zip_file:
-                with zip_file.open("metadata.json") as manifest_data:
-                    meta_data_json = json_loads(manifest_data.read().decode("utf-8"))
-
-        return meta_data_json
-
-    def _get_assets(self, manifest) -> List[str]:
-        """
-        Extracts asset URIs from the given manifest.
-
-        Parameters:
-        manifest (dict): The manifest containing information about assets.
-
-        Returns:
-        List[str]: A list of asset URIs extracted from the manifest.
-        """
-        files = []
-        # Iterate over each "asset" in the manifest
-        for asset in manifest.get("assets", []):
-            uri = asset.get("URI", "")
-            if "embed:/" in uri:
-                continue
-            files.append(uri)
-
-        return files
-
-    def _decompose_urn(self, encodedUrn):
-        """
-            Decomposes the given encoded URN into its constituent parts.
-
-            Parameters:
-            encodedUrn (str): The encoded URN to be decomposed.
-
-            Returns:
-            PathInfo: An object containing the decomposed parts of the URN,
-                      including root filename, base path, local path, and the original URN.
-        """
-        urn = unquote(encodedUrn)
-
-        rootFileName = urn[urn.rfind('/') + 1:]
-        basePath = urn[:urn.rfind('/') + 1]
-        localPath = basePath[basePath.find('/') + 1:]
-        localPath = re.sub(r"[/]?output/", "", localPath)
-
-        return PathInfo(rootFileName, basePath, localPath, urn)
-
-    def download_stream_resource(self, resource) -> BytesIO:
-        """
-        Downloads a resource from a URL and returns it as a stream.
-
-        Parameters:
-        resource (Resource): The resource object containing the URL to download.
-
-        Returns:
-        BytesIO: A stream containing the downloaded resource.
-        """
-        url = resource.url
-        access_token = self.token.access_token
-        if not access_token:
-            raise Exception("Have no access token to download resource.")
-        headers = {
-            "Authorization": f"Bearer {access_token}",
-            "region": self.region
-        }
-        response = requests.get(url, headers=headers)
-        return BytesIO(response.content)
-
-    def download_resource(self, resource, local_path) -> str:
-        """
-        Downloads a resource from a URL and saves it to a local path.
-
-        Parameters:
-        resource (Resource): The resource object containing the URL to download.
-        local_path (str): The local path where the resource will be saved.
-
-        Returns:
-        str: The local path where the resource has been saved.
-        """
-        url = resource.url
-        access_token = self.token.access_token
-        if not access_token:
-            raise Exception("Have no access token to download resource.")
-        headers = {
-            "Authorization": f"Bearer {access_token}",
-            "region": self.region
-        }
-        response = requests.get(url, headers=headers)
-        # if dir not exist, create it
-        if not os.path.exists(os.path.dirname(local_path)):
-            os.makedirs(os.path.dirname(local_path))
-        with open(local_path, "wb") as f:
-            f.write(response.content)
-        return local_path
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+import requests
+import gzip
+from io import BytesIO
+import zipfile
+from json import loads as json_loads
+from typing import List
+from urllib.parse import unquote, quote, urljoin
+import re
+from os.path import join, normpath
+import os
+from .PathInfo import PathInfo
+from .Resource import Resource
+from .ManifestItem import ManifestItem
+import json
+
+
+class Derivative:
+    def __init__(self, urn, token, region="US"):
+        self.urn = urn
+        self.token = token
+        self.region = region
+        self.host = "https://developer.api.autodesk.com"
+
+    def translate_job(self, root_file_name, type="svf", generate_master_views=False):
+        url = "https://developer.api.autodesk.com/modelderivative/v2/designdata/job"
+        access_token = self.token.access_token
+        if not access_token:
+            raise Exception("Have no access token to translate job.")
+        payload = json.dumps({
+            "input": {
+                "urn": self.urn,
+                "rootFilename": root_file_name
+            },
+            "output": {
+                "destination": {
+                    "region": self.region.lower()
+                },
+                "formats": [
+                    {
+                        "type": type,
+                        "views": [
+                            "2d",
+                            "3d"
+                        ],
+                        "advanced": {
+                            "generateMasterViews": generate_master_views
+                        }
+                    }
+                ]
+            }
+        })
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Authorization': 'Bearer ' + access_token,
+            'x-ads-force': 'true'
+        }
+        response = requests.post(url, headers=headers, data=payload)
+        return response.text
+
+    def check_job_status(self):
+        url = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest"
+        access_token = self.token.access_token
+        if not access_token:
+            raise Exception("Have no access token to check job status.")
+        headers = {
+            "Authorization": f"Bearer {access_token}",
+            "region": self.region
+        }
+        response = requests.get(url, headers=headers)
+        return response.json()
+
+    def read_svf_manifest_items(self) -> List[ManifestItem]:
+        """
+        Reads SVF manifest items associated with the URN.
+
+        Returns:
+        List[ManifestItem]: A list of SVF manifest items.
+        """
+        URL = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest"
+        access_token = self.token.access_token
+        if not access_token:
+            raise Exception("Have no access token to get manifest items.")
+        headers = {
+            "Authorization": f"Bearer {access_token}",
+            "region": self.region
+        }
+        # request
+        response = requests.get(URL, headers=headers)
+        if response.status_code == 404:
+            raise Exception(response.content)
+        json_response = response.json()
+        children = json_response['derivatives'][0]["children"]
+        manifest_items = []
+        image_items = []
+        for child in children:
+            if child["type"] == "geometry":
+                for c in child["children"]:
+                    # check if contains 'mime' and 'application/autodesk-svf
+                    if "mime" in c and c["mime"] == "application/autodesk-svf":
+                        urn_json = c["urn"]
+                        json_content = self._unzip_svf(urn_json)
+                        path_info = self._decompose_urn(urn_json)
+                        path_info.files = self._get_assets(json_content)
+                        guid = c["guid"]
+                        mime = c["mime"]
+                        # add svf files
+                        path_info.files.append(path_info.root_file_name)
+                        manifest_items.append(ManifestItem(guid, mime, path_info, urn_json))
+                    # case mapping image with svf
+                    if "type" in c and c["role"] == "thumbnail":
+                        guid = c["guid"]
+                        mime = c["mime"]
+                        urn = c["urn"]
+                        path_info = self._decompose_urn(urn)
+                        image_items.append(ManifestItem(guid, mime, path_info, urn))
+        # add files images to manifest items by mapp with local_path
+        for image in image_items:
+            for manifest_item in manifest_items:
+                if image.path_info.local_path == manifest_item.path_info.local_path:
+                    manifest_item.path_info.files.append(image.path_info.root_file_name)
+                    continue
+        return manifest_items
+
+    def read_svf_resource_item(self, manifest_item) -> List[Resource]:
+        """
+        Reads SVF resource items from the manifest item.
+
+        Parameters:
+        manifest_item (ManifestItem): The manifest item containing information about SVF resources.
+
+        Returns:
+        List[Resource]: A list of SVF resource items extracted from the manifest item.
+        """
+        resources = []
+        derivative_path = "derivativeservice/v2/derivatives/"
+        for file in manifest_item.path_info.files:
+            file_name = file[file.rfind("/") + 1:]
+            uri_local_path = "file://" + manifest_item.path_info.local_path + file
+            local_path = unquote(uri_local_path)[len("file://"):]
+            # Normalize the path to remove /../../
+            local_path = normpath(local_path)
+            myUri = "file://" + manifest_item.path_info.base_path + file
+            remote_path = join(derivative_path, unquote(myUri)[len("file://"):])
+            remote_path = normpath(remote_path)
+            resources.append(Resource(file_name, remote_path, local_path))
+        return resources
+
+    def read_svf_resource(self) -> dict[str, List[Resource]]:
+        """
+        Reads SVF resources from the SVF manifest items.
+
+        Returns:
+        List[Resource]: A list of resources extracted from the SVF manifest.
+        """
+        manifest_items = self.read_svf_manifest_items()
+        resources = {}
+        for manifest_item in manifest_items:
+            source_items = self.read_svf_resource_item(manifest_item)
+            resources[manifest_item.guid] = source_items
+        return resources
+
+    def _unzip_svf(self, svf_urn):
+        """
+        Retrieves and unzips the manifest associated with the given URN.
+
+        Parameters:
+        urn (str): The URN of the manifest to retrieve and unzip.
+
+        Returns:
+        dict: The contents of the unzipped manifest in JSON format.
+        """
+        URL = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest/{svf_urn}"
+        access_token = self.token.access_token
+        headers = {
+            "Authorization": f"Bearer {access_token}",
+            "region": self.region
+        }
+        response = requests.get(URL, headers=headers)
+        if response.status_code == 404:
+            raise Exception(response.content)
+        manifest_json = None
+        # unzip it
+        if ".gz" in response.headers.get("Content-Type", ""):
+            with gzip.GzipFile(fileobj=BytesIO(response.content), mode="rb") as gzip_file:
+                manifest_json = json_loads(gzip_file.read().decode("utf-8"))
+        else:
+            with zipfile.ZipFile(BytesIO(response.content)) as zip_file:
+                with zip_file.open("manifest.json") as manifest_data:
+                    manifest_json = json_loads(manifest_data.read().decode("utf-8"))
+
+        return manifest_json
+
+    def read_svf_metadata(self, svf_urn):
+        """
+        Retrieves and unzips the manifest associated with the given URN.
+
+        Parameters:
+        urn (str): The URN of the manifest to retrieve and unzip.
+
+        Returns:
+        dict: The contents of the unzipped manifest in JSON format.
+        """
+        URL = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest/{svf_urn}"
+        access_token = self.token.access_token
+        headers = {
+            "Authorization": f"Bearer {access_token}",
+            "region": self.region
+        }
+        response = requests.get(URL, headers=headers)
+        if response.status_code == 404:
+            raise Exception(response.content)
+        meta_data_json = None
+        # unzip it
+        if ".gz" in response.headers.get("Content-Type", ""):
+            with gzip.GzipFile(fileobj=BytesIO(response.content), mode="rb") as gzip_file:
+                meta_data_json = json_loads(gzip_file.read().decode("utf-8"))
+        else:
+            with zipfile.ZipFile(BytesIO(response.content)) as zip_file:
+                with zip_file.open("metadata.json") as manifest_data:
+                    meta_data_json = json_loads(manifest_data.read().decode("utf-8"))
+
+        return meta_data_json
+
+    def _get_assets(self, manifest) -> List[str]:
+        """
+        Extracts asset URIs from the given manifest.
+
+        Parameters:
+        manifest (dict): The manifest containing information about assets.
+
+        Returns:
+        List[str]: A list of asset URIs extracted from the manifest.
+        """
+        files = []
+        # Iterate over each "asset" in the manifest
+        for asset in manifest.get("assets", []):
+            uri = asset.get("URI", "")
+            if "embed:/" in uri:
+                continue
+            files.append(uri)
+
+        return files
+
+    def _decompose_urn(self, encodedUrn):
+        """
+            Decomposes the given encoded URN into its constituent parts.
+
+            Parameters:
+            encodedUrn (str): The encoded URN to be decomposed.
+
+            Returns:
+            PathInfo: An object containing the decomposed parts of the URN,
+                      including root filename, base path, local path, and the original URN.
+        """
+        urn = unquote(encodedUrn)
+
+        rootFileName = urn[urn.rfind('/') + 1:]
+        basePath = urn[:urn.rfind('/') + 1]
+        localPath = basePath[basePath.find('/') + 1:]
+        localPath = re.sub(r"[/]?output/", "", localPath)
+
+        return PathInfo(rootFileName, basePath, localPath, urn)
+
+    def download_stream_resource(self, resource) -> BytesIO:
+        """
+        Downloads a resource from a URL and returns it as a stream.
+
+        Parameters:
+        resource (Resource): The resource object containing the URL to download.
+
+        Returns:
+        BytesIO: A stream containing the downloaded resource.
+        """
+        url = resource.url
+        access_token = self.token.access_token
+        if not access_token:
+            raise Exception("Have no access token to download resource.")
+        headers = {
+            "Authorization": f"Bearer {access_token}",
+            "region": self.region
+        }
+        response = requests.get(url, headers=headers)
+        return BytesIO(response.content)
+
+    def download_resource(self, resource, local_path) -> str:
+        """
+        Downloads a resource from a URL and saves it to a local path.
+
+        Parameters:
+        resource (Resource): The resource object containing the URL to download.
+        local_path (str): The local path where the resource will be saved.
+
+        Returns:
+        str: The local path where the resource has been saved.
+        """
+        url = resource.url
+        access_token = self.token.access_token
+        if not access_token:
+            raise Exception("Have no access token to download resource.")
+        headers = {
+            "Authorization": f"Bearer {access_token}",
+            "region": self.region
+        }
+        response = requests.get(url, headers=headers)
+        # if dir not exist, create it
+        if not os.path.exists(os.path.dirname(local_path)):
+            os.makedirs(os.path.dirname(local_path))
+        with open(local_path, "wb") as f:
+            f.write(response.content)
+        return local_path
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/Fragments.py` & `aps-toolkit-0.5.4/src/aps_toolkit/Fragments.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-from .PackFileReader import PackFileReader
-from .Derivative import Derivative
-from .ManifestItem import ManifestItem
-class Fragments:
-    def __init__(self):
-        self.visible = False
-        self.materialID = 0
-        self.geometryID = 0
-        self.dbID = 0
-        self.transform = None
-        self.bbox = [0, 0, 0, 0, 0, 0]
-
-    @staticmethod
-    def parse_fragments_from_urn(urn, token, region="US") -> dict:
-        """
-        Parse fragments from urn
-        :param urn: the urn of the model
-        :param token: the token authentication
-        :param region:  the region of hub (default is US)
-        :return:  a dictionary of fragments with key is the guid of the manifest item and value is the list of fragments
-        """
-        fragments = {}
-        derivative = Derivative(urn, token, region)
-        manifest_items = derivative.read_svf_manifest_items()
-        for manifest_item in manifest_items:
-            resources = derivative.read_svf_resource_item(manifest_item)
-            for resource in resources:
-                if resource.local_path.endswith("FragmentList.pack"):
-                    bytes_io = derivative.download_stream_resource(resource)
-                    buffer = bytes_io.read()
-                    frags = Fragments.parse_fragments(buffer)
-                    fragments[manifest_item.guid] = frags
-        return fragments
-
-    @staticmethod
-    def parse_fragments_from_file(file_path) -> list:
-        """
-        Parse fragments from file
-        :param file_path:  FragmentList.pack
-        :return:  a list of fragments
-        """
-        with open(file_path, "rb") as f:
-            buffer = f.read()
-            return Fragments.parse_fragments(buffer)
-
-    @staticmethod
-    def parse_fragments(buffer: bytes) -> list:
-        """
-        Parse fragments from buffer
-        :param buffer:  the buffer of the fragment list
-        :return:  a list of fragments
-        """
-        fragments = []
-        pfr = PackFileReader(buffer)
-
-        for i in range(pfr.num_entries()):
-            entry_type = pfr.seek_entry(i)
-            assert entry_type is not None
-            assert entry_type.version > 4
-
-            flags = pfr.get_uint8()
-            visible = (flags & 0x01) != 0
-            material_id = pfr.get_varint()
-            geometry_id = pfr.get_varint()
-            transform = pfr.get_transform()
-            bbox = [0, 0, 0, 0, 0, 0]
-            bbox_offset = [0, 0, 0]
-            if entry_type.version > 3:
-                if transform is not None and transform.t is not None:
-                    bbox_offset[0] = transform.t[0]
-                    bbox_offset[1] = transform.t[1]
-                    bbox_offset[2] = transform.t[2]
-
-            for j in range(6):
-                bbox[j] = pfr.get_float32() + bbox_offset[j % 3]
-
-            db_id = pfr.get_varint()
-
-            fragment = Fragments()
-            fragment.visible = visible
-            fragment.materialID = material_id
-            fragment.geometryID = geometry_id
-            fragment.dbID = db_id
-            fragment.transform = transform
-            fragment.bbox = bbox
-            fragments.append(fragment)
-
-        return fragments
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+from .PackFileReader import PackFileReader
+from .Derivative import Derivative
+from .ManifestItem import ManifestItem
+class Fragments:
+    def __init__(self):
+        self.visible = False
+        self.materialID = 0
+        self.geometryID = 0
+        self.dbID = 0
+        self.transform = None
+        self.bbox = [0, 0, 0, 0, 0, 0]
+
+    @staticmethod
+    def parse_fragments_from_urn(urn, token, region="US") -> dict:
+        """
+        Parse fragments from urn
+        :param urn: the urn of the model
+        :param token: the token authentication
+        :param region:  the region of hub (default is US)
+        :return:  a dictionary of fragments with key is the guid of the manifest item and value is the list of fragments
+        """
+        fragments = {}
+        derivative = Derivative(urn, token, region)
+        manifest_items = derivative.read_svf_manifest_items()
+        for manifest_item in manifest_items:
+            resources = derivative.read_svf_resource_item(manifest_item)
+            for resource in resources:
+                if resource.local_path.endswith("FragmentList.pack"):
+                    bytes_io = derivative.download_stream_resource(resource)
+                    buffer = bytes_io.read()
+                    frags = Fragments.parse_fragments(buffer)
+                    fragments[manifest_item.guid] = frags
+        return fragments
+
+    @staticmethod
+    def parse_fragments_from_file(file_path) -> list:
+        """
+        Parse fragments from file
+        :param file_path:  FragmentList.pack
+        :return:  a list of fragments
+        """
+        with open(file_path, "rb") as f:
+            buffer = f.read()
+            return Fragments.parse_fragments(buffer)
+
+    @staticmethod
+    def parse_fragments(buffer: bytes) -> list:
+        """
+        Parse fragments from buffer
+        :param buffer:  the buffer of the fragment list
+        :return:  a list of fragments
+        """
+        fragments = []
+        pfr = PackFileReader(buffer)
+
+        for i in range(pfr.num_entries()):
+            entry_type = pfr.seek_entry(i)
+            assert entry_type is not None
+            assert entry_type.version > 4
+
+            flags = pfr.get_uint8()
+            visible = (flags & 0x01) != 0
+            material_id = pfr.get_varint()
+            geometry_id = pfr.get_varint()
+            transform = pfr.get_transform()
+            bbox = [0, 0, 0, 0, 0, 0]
+            bbox_offset = [0, 0, 0]
+            if entry_type.version > 3:
+                if transform is not None and transform.t is not None:
+                    bbox_offset[0] = transform.t[0]
+                    bbox_offset[1] = transform.t[1]
+                    bbox_offset[2] = transform.t[2]
+
+            for j in range(6):
+                bbox[j] = pfr.get_float32() + bbox_offset[j % 3]
+
+            db_id = pfr.get_varint()
+
+            fragment = Fragments()
+            fragment.visible = visible
+            fragment.materialID = material_id
+            fragment.geometryID = geometry_id
+            fragment.dbID = db_id
+            fragment.transform = transform
+            fragment.bbox = bbox
+            fragments.append(fragment)
+
+        return fragments
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/ManifestItem.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFTransform.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-from .PathInfo import PathInfo
-
-
-class ManifestItem:
-    def __init__(self, guid, mime, path_info: [PathInfo], urn):
-        self.guid = guid
-        self.mime = mime
-        self.urn = urn
-        self.path_info = path_info
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+class SVFTransform:
+    def __init__(self, t=None, q=None, s=None, matrix=None):
+        self.t = t
+        self.q = q
+        self.s = s
+        self.matrix = matrix
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/MaterialProperties.py` & `aps-toolkit-0.5.4/src/aps_toolkit/MaterialProperties.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-class MaterialProperties:
-    def __init__(self, integers=None, booleans=None, strings=None, uris=None, scalars=None, colors=None,
-                 choicelists=None, uuids=None, references=None):
-        self.integers = integers
-        self.booleans = booleans
-        self.strings = strings
-        self.uris = uris
-        self.scalars = scalars
-        self.colors = colors
-        self.choicelists = choicelists
-        self.uuids = uuids
-        self.references = references
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+class MaterialProperties:
+    def __init__(self, integers=None, booleans=None, strings=None, uris=None, scalars=None, colors=None,
+                 choicelists=None, uuids=None, references=None):
+        self.integers = integers
+        self.booleans = booleans
+        self.strings = strings
+        self.uris = uris
+        self.scalars = scalars
+        self.colors = colors
+        self.choicelists = choicelists
+        self.uuids = uuids
+        self.references = references
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/Materials.py` & `aps-toolkit-0.5.4/src/aps_toolkit/Materials.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-from .MaterialProperties import MaterialProperties
-from .SVFMaterialMap import SVFMaterialMap
-
-
-class Materials:
-    def __init__(self, diffuse=None, specular=None, ambient=None, emissive=None, glossiness=None, reflectivity=None,
-                 opacity=None, metal=None, map: [SVFMaterialMap] = None, tag=None,
-                 proteinType=None, definition=None, transparent=None, keywords=None, categories=None,
-                 properties: [MaterialProperties] = None,
-                 textures=None):
-        self.diffuse = diffuse
-        self.specular = specular
-        self.ambient = ambient
-        self.emissive = emissive
-        self.glossiness = glossiness
-        self.reflectivity = reflectivity
-        self.opacity = opacity
-        self.metal = metal
-        self.map = map
-        self.tag = tag
-        self.proteinType = proteinType
-        self.definition = definition
-        self.transparent = transparent
-        self.keywords = keywords
-        self.categories = categories
-        self.properties = properties
-        self.textures = textures
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+from .MaterialProperties import MaterialProperties
+from .SVFMaterialMap import SVFMaterialMap
+
+
+class Materials:
+    def __init__(self, diffuse=None, specular=None, ambient=None, emissive=None, glossiness=None, reflectivity=None,
+                 opacity=None, metal=None, map: [SVFMaterialMap] = None, tag=None,
+                 proteinType=None, definition=None, transparent=None, keywords=None, categories=None,
+                 properties: [MaterialProperties] = None,
+                 textures=None):
+        self.diffuse = diffuse
+        self.specular = specular
+        self.ambient = ambient
+        self.emissive = emissive
+        self.glossiness = glossiness
+        self.reflectivity = reflectivity
+        self.opacity = opacity
+        self.metal = metal
+        self.map = map
+        self.tag = tag
+        self.proteinType = proteinType
+        self.definition = definition
+        self.transparent = transparent
+        self.keywords = keywords
+        self.categories = categories
+        self.properties = properties
+        self.textures = textures
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/PathInfo.py` & `aps-toolkit-0.5.4/src/aps_toolkit/PathInfo.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-
-class PathInfo:
-    def __init__(self, root_file_name=None, base_path=None, local_path=None, urn=None):
-        self.root_file_name = root_file_name
-        self.local_path = local_path
-        self.base_path = base_path
-        self.urn = urn
-        self.files = []
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+
+class PathInfo:
+    def __init__(self, root_file_name=None, base_path=None, local_path=None, urn=None):
+        self.root_file_name = root_file_name
+        self.local_path = local_path
+        self.base_path = base_path
+        self.urn = urn
+        self.files = []
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/ProDbReaderCad.py` & `aps-toolkit-0.5.4/src/aps_toolkit/ProDbReaderCad.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import re
-from typing import List
-import pandas as pd
-from .ManifestItem import ManifestItem
-from .PropReader import PropReader
-
-
-class PropDbReaderCad(PropReader):
-    def __int__(self, urn, token, region="US", manifest_item: [ManifestItem] = None):
-        super().__init__(urn, token, region, manifest_item)
-
-    def get_document_info(self) -> pd.Series:
-        schema_name = "DocumentData"
-        indexs = []
-        # get index at value DocumentData
-        for i, s in enumerate(self.ids):
-            if s == schema_name:
-                indexs.append(i)
-        df = self.get_recursive_ids(indexs)
-        series = df.iloc[0]
-        return series
-
-    def get_all_layers(self):
-        db_layers = []
-        df = pd.DataFrame()
-        for i, s in enumerate(self.ids):
-            properties = self.enumerate_properties(i)
-            flag_layer = [p for p in properties if p.name == "type" and p.value == "AcDbLayerTableRecord"]
-            if flag_layer:
-                df_single = self.get_recursive_ids([i])
-                df = pd.concat([df, df_single])
-        return df
-
-    def get_all_categories(self) -> dict:
-        db_categories = {}
-        for i, s in enumerate(self.ids):
-            properties = self.enumerate_properties(i)
-            type = "AcDbBlockTableRecord"
-            dbid = None
-            flag = [p for p in properties if p.name == "type" and p.value == type]
-            if flag:
-                dbid = i
-            if dbid:
-                childs = self.get_children(dbid)
-                for child in childs:
-                    properties = self.enumerate_properties(child)
-                    for p in properties:
-                        if p.name == "type":
-                            db_categories[child] = p.value
-        return db_categories
-
-    def get_data_by_category(self, category) -> pd.DataFrame:
-        """
-        Get data by cad category : eg: MText, Line, Circle, ...
-        :param category: the category name of cad file, e.g : MText, Line, Circle,Tables ...
-        :return: pandas dataframe
-        """
-        db_categories = self.get_all_categories()
-        category_ids = [k for k, v in db_categories.items() if v.lower() == category.lower()]
-        childs = self.get_children(category_ids[0])
-        return self.get_recursive_ids(childs)
-
-    def get_data_by_categories(self, categories: List[str]) -> pd.DataFrame:
-        """
-        Get data by multiple cad categories
-        :param categories: list of category names
-        :return: pandas dataframe
-        """
-        df = pd.DataFrame()
-        for category in categories:
-            df = pd.concat([df, self.get_data_by_category(category)])
-        return df
-
-    def get_data_by_categories_and_params(self, categories: List[str], params: List[str]) -> pd.DataFrame:
-        """
-        Get data by multiple cad categories and multiple parameters
-        :param categories: list of category names
-        :param params: list of parameters
-        :return: pandas dataframe
-        """
-        db_categories = self.get_all_categories()
-        category_ids = [k for k, v in db_categories.items() if v.lower() in [c.lower() for c in categories]]
-        childs = [self.get_children(category_id) for category_id in category_ids]
-        # flatten list of list
-        childs = [item for sublist in childs for item in sublist]
-        df = self.get_recursive_ids_by_parameters(childs, params)
-        return df
-
-    def get_all_data(self) -> pd.DataFrame:
-        """
-        Get all data from cad file
-        :return: pandas dataframe
-        """
-        cates = self.get_all_categories()
-        df = pd.DataFrame()
-        for k, v in cates.items():
-            childs = self.get_children(k)
-            df = pd.concat([df, self.get_recursive_ids(childs)])
-        return df
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+import re
+from typing import List
+import pandas as pd
+from .ManifestItem import ManifestItem
+from .PropReader import PropReader
+
+
+class PropDbReaderCad(PropReader):
+    def __int__(self, urn, token, region="US", manifest_item: [ManifestItem] = None):
+        super().__init__(urn, token, region, manifest_item)
+
+    def get_document_info(self) -> pd.Series:
+        schema_name = "DocumentData"
+        indexs = []
+        # get index at value DocumentData
+        for i, s in enumerate(self.ids):
+            if s == schema_name:
+                indexs.append(i)
+        df = self.get_recursive_ids(indexs)
+        series = df.iloc[0]
+        return series
+
+    def get_all_layers(self):
+        db_layers = []
+        df = pd.DataFrame()
+        for i, s in enumerate(self.ids):
+            properties = self.enumerate_properties(i)
+            flag_layer = [p for p in properties if p.name == "type" and p.value == "AcDbLayerTableRecord"]
+            if flag_layer:
+                df_single = self.get_recursive_ids([i])
+                df = pd.concat([df, df_single])
+        return df
+
+    def get_all_categories(self) -> dict:
+        db_categories = {}
+        for i, s in enumerate(self.ids):
+            properties = self.enumerate_properties(i)
+            type = "AcDbBlockTableRecord"
+            dbid = None
+            flag = [p for p in properties if p.name == "type" and p.value == type]
+            if flag:
+                dbid = i
+            if dbid:
+                childs = self.get_children(dbid)
+                for child in childs:
+                    properties = self.enumerate_properties(child)
+                    for p in properties:
+                        if p.name == "type":
+                            db_categories[child] = p.value
+        return db_categories
+
+    def get_data_by_category(self, category) -> pd.DataFrame:
+        """
+        Get data by cad category : eg: MText, Line, Circle, ...
+        :param category: the category name of cad file, e.g : MText, Line, Circle,Tables ...
+        :return: pandas dataframe
+        """
+        db_categories = self.get_all_categories()
+        category_ids = [k for k, v in db_categories.items() if v.lower() == category.lower()]
+        childs = self.get_children(category_ids[0])
+        return self.get_recursive_ids(childs)
+
+    def get_data_by_categories(self, categories: List[str]) -> pd.DataFrame:
+        """
+        Get data by multiple cad categories
+        :param categories: list of category names
+        :return: pandas dataframe
+        """
+        df = pd.DataFrame()
+        for category in categories:
+            df = pd.concat([df, self.get_data_by_category(category)])
+        return df
+
+    def get_data_by_categories_and_params(self, categories: List[str], params: List[str]) -> pd.DataFrame:
+        """
+        Get data by multiple cad categories and multiple parameters
+        :param categories: list of category names
+        :param params: list of parameters
+        :return: pandas dataframe
+        """
+        db_categories = self.get_all_categories()
+        category_ids = [k for k, v in db_categories.items() if v.lower() in [c.lower() for c in categories]]
+        childs = [self.get_children(category_id) for category_id in category_ids]
+        # flatten list of list
+        childs = [item for sublist in childs for item in sublist]
+        df = self.get_recursive_ids_by_parameters(childs, params)
+        return df
+
+    def get_all_data(self) -> pd.DataFrame:
+        """
+        Get all data from cad file
+        :return: pandas dataframe
+        """
+        cates = self.get_all_categories()
+        df = pd.DataFrame()
+        for k, v in cates.items():
+            childs = self.get_children(k)
+            df = pd.concat([df, self.get_recursive_ids(childs)])
+        return df
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/ProDbReaderNavis.py` & `aps-toolkit-0.5.4/src/aps_toolkit/ProDbReaderNavis.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-from typing import List
-import re
-import pandas as pd
-import json
-import requests
-from .PropReader import PropReader
-from .ManifestItem import ManifestItem
-
-
-class PropDbReaderNavis(PropReader):
-    def __int__(self, urn, token, region="US", manifest_item: [ManifestItem] = None):
-        super().__init__(urn, token, region, manifest_item)
-
-    def _get_recursive_child(self, output, id, name):
-        children = self.get_children(id)
-        for child in children:
-            properties = self.enumerate_properties(child)
-            property = [prop.value for prop in properties if prop.name == name]
-            if len(property) == 0:
-                self._get_recursive_child(output, child, name)
-            else:
-                if str(property[0]) == "": continue
-                output[child] = property[0].strip()
-
-    def get_external_id(self, id) -> str:
-        return self.ids[id]
-
-    def get_document_info(self) -> pd.DataFrame:
-        props = {}
-        for prop in self.enumerate_properties(1):
-            props[prop.display_name] = prop.value
-        df = pd.DataFrame.from_dict(props, orient='index')
-        df = df.rename(columns={0: "value"})
-        df = df.reset_index()
-        df = df.rename(columns={"index": "property"})
-        return df
-
-    def get_all_categories(self) -> List[str]:
-        categories = []
-        rg = re.compile(r'^__\w+__$')
-        for i in range(1, len(self.attrs)):
-            if self.attrs[i][1] not in categories and not rg.match(self.attrs[i][1]):
-                categories.append(self.attrs[i][1])
-        return categories
-
-    def get_data_by_category(self, category) -> pd.DataFrame:
-        db_ids = [1]
-        df = self._get_recursive_ids_by_category(db_ids, category)
-        df = df.drop_duplicates(subset=df.columns.difference(['DbId']))
-        return df
-
-    def _get_recursive_ids_by_category(self, db_ids: List[int], category) -> pd.DataFrame:
-        dataframe = pd.DataFrame()
-        props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
-        if len(db_ids) == 0:
-            return dataframe
-        for id in db_ids:
-            props = self.enumerate_properties(id)
-            properties = {}
-            flag = [p for p in props if p.category == category]
-            if flag:
-                properties["DbId"] = id
-                for p in props:
-                    if p.name not in props_ignore and p.category == category:
-                        properties[p.display_name] = p.value
-                singleDF = pd.DataFrame(properties, index=[0])
-                dataframe = pd.concat([dataframe, singleDF], ignore_index=True)
-            children = self.get_children(id)
-            df = self._get_recursive_ids_by_category(children, category)
-            dataframe = pd.concat([dataframe, df], ignore_index=True)
-        return dataframe
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+from typing import List
+import re
+import pandas as pd
+import json
+import requests
+from .PropReader import PropReader
+from .ManifestItem import ManifestItem
+
+
+class PropDbReaderNavis(PropReader):
+    def __int__(self, urn, token, region="US", manifest_item: [ManifestItem] = None):
+        super().__init__(urn, token, region, manifest_item)
+
+    def _get_recursive_child(self, output, id, name):
+        children = self.get_children(id)
+        for child in children:
+            properties = self.enumerate_properties(child)
+            property = [prop.value for prop in properties if prop.name == name]
+            if len(property) == 0:
+                self._get_recursive_child(output, child, name)
+            else:
+                if str(property[0]) == "": continue
+                output[child] = property[0].strip()
+
+    def get_external_id(self, id) -> str:
+        return self.ids[id]
+
+    def get_document_info(self) -> pd.DataFrame:
+        props = {}
+        for prop in self.enumerate_properties(1):
+            props[prop.display_name] = prop.value
+        df = pd.DataFrame.from_dict(props, orient='index')
+        df = df.rename(columns={0: "value"})
+        df = df.reset_index()
+        df = df.rename(columns={"index": "property"})
+        return df
+
+    def get_all_categories(self) -> List[str]:
+        categories = []
+        rg = re.compile(r'^__\w+__$')
+        for i in range(1, len(self.attrs)):
+            if self.attrs[i][1] not in categories and not rg.match(self.attrs[i][1]):
+                categories.append(self.attrs[i][1])
+        return categories
+
+    def get_data_by_category(self, category) -> pd.DataFrame:
+        db_ids = [1]
+        df = self._get_recursive_ids_by_category(db_ids, category)
+        df = df.drop_duplicates(subset=df.columns.difference(['DbId']))
+        return df
+
+    def _get_recursive_ids_by_category(self, db_ids: List[int], category) -> pd.DataFrame:
+        dataframe = pd.DataFrame()
+        props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
+        if len(db_ids) == 0:
+            return dataframe
+        for id in db_ids:
+            props = self.enumerate_properties(id)
+            properties = {}
+            flag = [p for p in props if p.category == category]
+            if flag:
+                properties["DbId"] = id
+                for p in props:
+                    if p.name not in props_ignore and p.category == category:
+                        properties[p.display_name] = p.value
+                singleDF = pd.DataFrame(properties, index=[0])
+                dataframe = pd.concat([dataframe, singleDF], ignore_index=True)
+            children = self.get_children(id)
+            df = self._get_recursive_ids_by_category(children, category)
+            dataframe = pd.concat([dataframe, df], ignore_index=True)
+        return dataframe
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/ProDbReaderRevit.py` & `aps-toolkit-0.5.4/src/aps_toolkit/ProDbReaderRevit.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,300 +1,300 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-from typing import List
-import re
-import pandas as pd
-import json
-import requests
-from .PropReader import PropReader
-from .ManifestItem import ManifestItem
-
-
-class PropDbReaderRevit(PropReader):
-    def __int__(self, urn, token, region="US", manifest_item: [ManifestItem] = None):
-        super().__init__(urn, token, region, manifest_item)
-
-    def _get_recursive_child(self, output, id, name):
-        children = self.get_children(id)
-        for child in children:
-            properties = self.enumerate_properties(child)
-            property = [prop.value for prop in properties if prop.name == name]
-            if len(property) == 0:
-                self._get_recursive_child(output, child, name)
-            else:
-                if str(property[0]) == "": continue
-                output[child] = property[0].strip()
-
-    def get_external_id(self, id) -> str:
-        return self.ids[id]
-
-    def get_document_info(self) -> pd.Series:
-        properties = self.get_all_properties(1)
-        return pd.Series(properties)
-
-    def _get_aec_model_data(self):
-        URL = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest"
-        access_token = self.token.access_token
-        headers = {
-            "Authorization": f"Bearer {access_token}",
-            "region": self.region
-        }
-        # request
-        response = requests.get(URL, headers=headers)
-        json_response = response.json()
-        children = json_response['derivatives'][0]["children"]
-        urn_json = ""
-        for child in children:
-            if child["type"] == "resource" and child["role"] == "Autodesk.AEC.ModelData":
-                urn_json = child["urn"]
-        URL = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest/{urn_json}"
-        response = requests.get(URL, headers=headers)
-        json_response = response.json()
-        return json_response
-
-    def get_phases(self) -> List[str]:
-        phases = []
-        json_response = self._get_aec_model_data()
-        for phase in json_response["phases"]:
-            phases.append(phase["name"])
-        return phases
-
-    def get_document_id(self) -> str:
-        json_response = self._get_aec_model_data()
-        return json_response["documentId"]
-
-    def get_levels(self) -> pd.DataFrame:
-        json_response = self._get_aec_model_data()
-        levels = json_response["levels"]
-        df = pd.DataFrame(levels)
-        return df
-
-    def get_grids(self) -> pd.DataFrame:
-        json_response = self._get_aec_model_data()
-        grids = json_response["grids"]
-        df = pd.DataFrame(grids)
-        return df
-
-    def get_linked_documents(self) -> list:
-        json_response = self._get_aec_model_data()
-        linked_documents = json_response["linkedDocuments"]
-        return linked_documents
-
-    def get_ref_point_transformation(self) -> list:
-        json_response = self._get_aec_model_data()
-        return json_response["refPointTransformation"]
-
-    def get_all_categories(self) -> dict:
-        categories = {}
-        self._get_recursive_child(categories, 1, "_RC")
-        return categories
-
-    def get_all_data(self, is_get_sub_family=False) -> pd.DataFrame:
-        categories_dict = self.get_all_categories()
-        dbids = list(categories_dict.keys())
-        dataframe = pd.DataFrame()
-        for dbid in dbids:
-            df = self._get_recursive_ids([dbid], is_get_sub_family)
-            dataframe = pd.concat([dataframe, df], ignore_index=True)
-        return dataframe
-
-    def get_all_families(self) -> dict:
-        families = {}
-        self._get_recursive_child(families, 1, "_RFN")
-        return families
-
-    def get_all_families_types(self) -> dict:
-        families_types = {}
-        self._get_recursive_child(families_types, 1, "_RFT")
-        return families_types
-
-    def get_data_by_category(self, category, is_get_sub_family=False) -> pd.DataFrame:
-        categories = self.get_all_categories()
-        # if category starts with Revit, remove it
-        if category.startswith("Revit"):
-            category = category[5:].strip()
-        category_id = [key for key, value in categories.items() if value == category]
-        dataframe = self._get_recursive_ids(category_id, is_get_sub_family)
-        return dataframe
-
-    def get_data_by_categories(self, categories: List[str], is_get_sub_family=False) -> pd.DataFrame:
-        dataframe = pd.DataFrame()
-        for category in categories:
-            dataframe = pd.concat([dataframe, self.get_data_by_category(category, is_get_sub_family)],
-                                  ignore_index=True)
-        return dataframe
-
-    def get_data_by_categories_and_params(self, categories: List[str], params: List[str],
-                                          is_get_sub_family=False) -> pd.DataFrame:
-        dataframe = pd.DataFrame()
-        all_categories = self.get_all_categories()
-        category_ids = [key for key, value in all_categories.items() if value in categories]
-        for category_id in category_ids:
-            dataframe = pd.concat([dataframe, self._get_recursive_ids_prams([category_id], params, is_get_sub_family)],
-                                  ignore_index=True)
-        # remove all row have all values is null, ignore dbId and external_id columns
-        dataframe = dataframe.dropna(how='all',
-                                     subset=[col for col in dataframe.columns if col not in ['dbId', 'external_id']])
-        return dataframe
-
-    def get_data_by_family(self, family_name, is_get_sub_family=False) -> pd.DataFrame:
-        families = self.get_all_families()
-        category_id = [key for key, value in families.items() if value == family_name]
-        dataframe = self._get_recursive_ids(category_id, is_get_sub_family)
-        return dataframe
-
-    def get_data_by_family_type(self, family_type, is_get_sub_family=False) -> pd.DataFrame:
-        family_types = self.get_all_families_types()
-        type_id = [key for key, value in family_types.items() if value == family_type]
-        dataframe = self._get_recursive_ids(type_id, is_get_sub_family)
-        return dataframe
-
-    def _get_recursive_ids(self, db_ids: List[int], get_sub_family) -> pd.DataFrame:
-        dataframe = pd.DataFrame()
-        props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
-        if len(db_ids) == 0:
-            return dataframe
-        for id in db_ids:
-            props = self.enumerate_properties(id)
-            flag_sub_families = False
-            properties = {}
-            # if props contain _RC, _RFN, _RFT, it's not a leaf node, continue to get children
-            if len([prop for prop in props if prop.name in ["_RC", "_RFN", "_RFT"]]) > 0:
-                ids = self.get_children(id)
-                dataframe = pd.concat([dataframe, self._get_recursive_ids(ids, get_sub_family)], ignore_index=True)
-                continue
-            for prop in props:
-                if prop.category == "__internalref__" and prop.name == "Sub Family":
-                    flag_sub_families = True
-                if prop.name not in props_ignore:
-                    if prop.name == "name":
-                        properties["Name"] = prop.value
-                    else:
-                        properties[prop.name] = prop.value
-            db_id = id
-            external_id = self.ids[id]
-            properties['dbId'] = db_id
-            properties['external_id'] = external_id
-            if flag_sub_families and not get_sub_family:
-                ids = self.get_children(id)
-                dataframe = pd.concat([dataframe, self._get_recursive_ids(ids, get_sub_family)], ignore_index=True)
-                continue
-            ins = self.get_instance(id)
-            if len(ins) > 0:
-                for instance in ins:
-                    types = self.get_properties(instance)
-                    properties = {**properties, **types}
-            singleDF = pd.DataFrame(properties, index=[0])
-            dataframe = pd.concat([dataframe, singleDF], ignore_index=True)
-            ids = self.get_children(id)
-            dataframe = pd.concat([dataframe, self._get_recursive_ids(ids, get_sub_family)], ignore_index=True)
-        if 'dbId' in dataframe.columns and 'external_id' in dataframe.columns:
-            dataframe = dataframe[
-                ['dbId', 'external_id'] + [col for col in dataframe.columns if col not in ['dbId', 'external_id']]]
-        return dataframe
-
-    def _get_recursive_ids_prams(self, childs: List[int], params: List[str], get_sub_family) -> pd.DataFrame:
-        dataframe = pd.DataFrame()
-        props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
-        if len(childs) == 0:
-            return dataframe
-        for id in childs:
-            flag_sub_families = False
-            props = self.enumerate_properties(id)
-            # if props contain _RC, _RFN, _RFT, it's not a leaf node, continue to get children
-            if len([prop for prop in props if prop.name in ["_RC", "_RFN", "_RFT"]]) > 0:
-                ids = self.get_children(id)
-                dataframe = pd.concat([dataframe, self._get_recursive_ids_prams(ids, params, get_sub_family)],
-                                      ignore_index=True)
-                continue
-            properties = {}
-            for prop in props:
-                if prop.category == "__internalref__" and prop.name == "Sub Family":
-                    flag_sub_families = True
-                if prop.name not in props_ignore:
-                    if prop.name == "name":
-                        properties["Name"] = prop.value
-                    else:
-                        properties[prop.name] = prop.value
-            db_id = id
-            external_id = self.ids[id]
-            # filter just get properties name in params list
-            properties = {k: v for k, v in properties.items() if k in params}
-            properties['dbId'] = db_id
-            properties['external_id'] = external_id
-            if flag_sub_families and not get_sub_family:
-                ids = self.get_children(id)
-                dataframe = pd.concat([dataframe, self._get_recursive_ids_prams(ids, params, get_sub_family)],
-                                      ignore_index=True)
-                continue
-            # get instances
-            ins = self.get_instance(id)
-            if len(ins) > 0:
-                for instance in ins:
-                    types = self.get_all_properties(instance)
-                    types = {k: v for k, v in types.items() if k in params}
-                    properties = {**properties, **types}
-            single_df = pd.DataFrame(properties, index=[0])
-            dataframe = pd.concat([dataframe, single_df], ignore_index=True)
-            ids = self.get_children(id)
-            dataframe = pd.concat([dataframe, self._get_recursive_ids_prams(ids, params, get_sub_family)],
-                                  ignore_index=True)
-        # set dbid and external_id to first and second column if it exists
-        if 'dbId' in dataframe.columns and 'external_id' in dataframe.columns:
-            dataframe = dataframe[
-                ['dbId', 'external_id'] + [col for col in dataframe.columns if col not in ['dbId', 'external_id']]]
-        return dataframe
-
-    def get_data_by_external_id(self, external_id, is_get_sub_family=False) -> pd.DataFrame:
-        db_id = None
-        for idx in range(0, len(self.ids)):
-            if self.ids[idx] == external_id:
-                db_id = idx
-                break
-        if db_id is None:
-            return pd.DataFrame()
-        dataframe = self._get_recursive_ids([db_id], is_get_sub_family)
-        return dataframe
-
-    def get_data_by_element_id(self, element_id) -> dict:
-        rg = re.compile(r'^__\w+__$')
-        properties = {}
-        for i in range(0, len(self.ids)):
-            props = self.enumerate_properties(i)
-            for prop in props:
-                if prop.name == "ElementId" and prop.value == str(element_id):
-                    for prop in props:
-                        if not rg.match(prop.category):
-                            properties[prop.name] = prop.value
-                    # get instance
-                    instances = self.get_instance(i)
-                    for instance in instances:
-                        types = self.get_properties(instance)
-                        properties = {**properties, **types}
-                    break
-        properties = dict(sorted(properties.items()))
-        return properties
-
-    def get_all_parameters(self) -> List:
-        parameters = []
-        for id in range(0, len(self.ids)):
-            props_dict = self.get_properties(id)
-            for key, value in props_dict.items():
-                if key not in parameters:
-                    parameters.append(key)
-        parameters = list(set(parameters))
-        parameters.sort()
-        return parameters
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+from typing import List
+import re
+import pandas as pd
+import json
+import requests
+from .PropReader import PropReader
+from .ManifestItem import ManifestItem
+
+
+class PropDbReaderRevit(PropReader):
+    def __int__(self, urn, token, region="US", manifest_item: [ManifestItem] = None):
+        super().__init__(urn, token, region, manifest_item)
+
+    def _get_recursive_child(self, output, id, name):
+        children = self.get_children(id)
+        for child in children:
+            properties = self.enumerate_properties(child)
+            property = [prop.value for prop in properties if prop.name == name]
+            if len(property) == 0:
+                self._get_recursive_child(output, child, name)
+            else:
+                if str(property[0]) == "": continue
+                output[child] = property[0].strip()
+
+    def get_external_id(self, id) -> str:
+        return self.ids[id]
+
+    def get_document_info(self) -> pd.Series:
+        properties = self.get_all_properties(1)
+        return pd.Series(properties)
+
+    def _get_aec_model_data(self):
+        URL = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest"
+        access_token = self.token.access_token
+        headers = {
+            "Authorization": f"Bearer {access_token}",
+            "region": self.region
+        }
+        # request
+        response = requests.get(URL, headers=headers)
+        json_response = response.json()
+        children = json_response['derivatives'][0]["children"]
+        urn_json = ""
+        for child in children:
+            if child["type"] == "resource" and child["role"] == "Autodesk.AEC.ModelData":
+                urn_json = child["urn"]
+        URL = f"{self.host}/modelderivative/v2/designdata/{self.urn}/manifest/{urn_json}"
+        response = requests.get(URL, headers=headers)
+        json_response = response.json()
+        return json_response
+
+    def get_phases(self) -> List[str]:
+        phases = []
+        json_response = self._get_aec_model_data()
+        for phase in json_response["phases"]:
+            phases.append(phase["name"])
+        return phases
+
+    def get_document_id(self) -> str:
+        json_response = self._get_aec_model_data()
+        return json_response["documentId"]
+
+    def get_levels(self) -> pd.DataFrame:
+        json_response = self._get_aec_model_data()
+        levels = json_response["levels"]
+        df = pd.DataFrame(levels)
+        return df
+
+    def get_grids(self) -> pd.DataFrame:
+        json_response = self._get_aec_model_data()
+        grids = json_response["grids"]
+        df = pd.DataFrame(grids)
+        return df
+
+    def get_linked_documents(self) -> list:
+        json_response = self._get_aec_model_data()
+        linked_documents = json_response["linkedDocuments"]
+        return linked_documents
+
+    def get_ref_point_transformation(self) -> list:
+        json_response = self._get_aec_model_data()
+        return json_response["refPointTransformation"]
+
+    def get_all_categories(self) -> dict:
+        categories = {}
+        self._get_recursive_child(categories, 1, "_RC")
+        return categories
+
+    def get_all_data(self, is_get_sub_family=False) -> pd.DataFrame:
+        categories_dict = self.get_all_categories()
+        dbids = list(categories_dict.keys())
+        dataframe = pd.DataFrame()
+        for dbid in dbids:
+            df = self._get_recursive_ids([dbid], is_get_sub_family)
+            dataframe = pd.concat([dataframe, df], ignore_index=True)
+        return dataframe
+
+    def get_all_families(self) -> dict:
+        families = {}
+        self._get_recursive_child(families, 1, "_RFN")
+        return families
+
+    def get_all_families_types(self) -> dict:
+        families_types = {}
+        self._get_recursive_child(families_types, 1, "_RFT")
+        return families_types
+
+    def get_data_by_category(self, category, is_get_sub_family=False) -> pd.DataFrame:
+        categories = self.get_all_categories()
+        # if category starts with Revit, remove it
+        if category.startswith("Revit"):
+            category = category[5:].strip()
+        category_id = [key for key, value in categories.items() if value == category]
+        dataframe = self._get_recursive_ids(category_id, is_get_sub_family)
+        return dataframe
+
+    def get_data_by_categories(self, categories: List[str], is_get_sub_family=False) -> pd.DataFrame:
+        dataframe = pd.DataFrame()
+        for category in categories:
+            dataframe = pd.concat([dataframe, self.get_data_by_category(category, is_get_sub_family)],
+                                  ignore_index=True)
+        return dataframe
+
+    def get_data_by_categories_and_params(self, categories: List[str], params: List[str],
+                                          is_get_sub_family=False) -> pd.DataFrame:
+        dataframe = pd.DataFrame()
+        all_categories = self.get_all_categories()
+        category_ids = [key for key, value in all_categories.items() if value in categories]
+        for category_id in category_ids:
+            dataframe = pd.concat([dataframe, self._get_recursive_ids_prams([category_id], params, is_get_sub_family)],
+                                  ignore_index=True)
+        # remove all row have all values is null, ignore dbId and external_id columns
+        dataframe = dataframe.dropna(how='all',
+                                     subset=[col for col in dataframe.columns if col not in ['dbId', 'external_id']])
+        return dataframe
+
+    def get_data_by_family(self, family_name, is_get_sub_family=False) -> pd.DataFrame:
+        families = self.get_all_families()
+        category_id = [key for key, value in families.items() if value == family_name]
+        dataframe = self._get_recursive_ids(category_id, is_get_sub_family)
+        return dataframe
+
+    def get_data_by_family_type(self, family_type, is_get_sub_family=False) -> pd.DataFrame:
+        family_types = self.get_all_families_types()
+        type_id = [key for key, value in family_types.items() if value == family_type]
+        dataframe = self._get_recursive_ids(type_id, is_get_sub_family)
+        return dataframe
+
+    def _get_recursive_ids(self, db_ids: List[int], get_sub_family) -> pd.DataFrame:
+        dataframe = pd.DataFrame()
+        props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
+        if len(db_ids) == 0:
+            return dataframe
+        for id in db_ids:
+            props = self.enumerate_properties(id)
+            flag_sub_families = False
+            properties = {}
+            # if props contain _RC, _RFN, _RFT, it's not a leaf node, continue to get children
+            if len([prop for prop in props if prop.name in ["_RC", "_RFN", "_RFT"]]) > 0:
+                ids = self.get_children(id)
+                dataframe = pd.concat([dataframe, self._get_recursive_ids(ids, get_sub_family)], ignore_index=True)
+                continue
+            for prop in props:
+                if prop.category == "__internalref__" and prop.name == "Sub Family":
+                    flag_sub_families = True
+                if prop.name not in props_ignore:
+                    if prop.name == "name":
+                        properties["Name"] = prop.value
+                    else:
+                        properties[prop.name] = prop.value
+            db_id = id
+            external_id = self.ids[id]
+            properties['dbId'] = db_id
+            properties['external_id'] = external_id
+            if flag_sub_families and not get_sub_family:
+                ids = self.get_children(id)
+                dataframe = pd.concat([dataframe, self._get_recursive_ids(ids, get_sub_family)], ignore_index=True)
+                continue
+            ins = self.get_instance(id)
+            if len(ins) > 0:
+                for instance in ins:
+                    types = self.get_properties(instance)
+                    properties = {**properties, **types}
+            singleDF = pd.DataFrame(properties, index=[0])
+            dataframe = pd.concat([dataframe, singleDF], ignore_index=True)
+            ids = self.get_children(id)
+            dataframe = pd.concat([dataframe, self._get_recursive_ids(ids, get_sub_family)], ignore_index=True)
+        if 'dbId' in dataframe.columns and 'external_id' in dataframe.columns:
+            dataframe = dataframe[
+                ['dbId', 'external_id'] + [col for col in dataframe.columns if col not in ['dbId', 'external_id']]]
+        return dataframe
+
+    def _get_recursive_ids_prams(self, childs: List[int], params: List[str], get_sub_family) -> pd.DataFrame:
+        dataframe = pd.DataFrame()
+        props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
+        if len(childs) == 0:
+            return dataframe
+        for id in childs:
+            flag_sub_families = False
+            props = self.enumerate_properties(id)
+            # if props contain _RC, _RFN, _RFT, it's not a leaf node, continue to get children
+            if len([prop for prop in props if prop.name in ["_RC", "_RFN", "_RFT"]]) > 0:
+                ids = self.get_children(id)
+                dataframe = pd.concat([dataframe, self._get_recursive_ids_prams(ids, params, get_sub_family)],
+                                      ignore_index=True)
+                continue
+            properties = {}
+            for prop in props:
+                if prop.category == "__internalref__" and prop.name == "Sub Family":
+                    flag_sub_families = True
+                if prop.name not in props_ignore:
+                    if prop.name == "name":
+                        properties["Name"] = prop.value
+                    else:
+                        properties[prop.name] = prop.value
+            db_id = id
+            external_id = self.ids[id]
+            # filter just get properties name in params list
+            properties = {k: v for k, v in properties.items() if k in params}
+            properties['dbId'] = db_id
+            properties['external_id'] = external_id
+            if flag_sub_families and not get_sub_family:
+                ids = self.get_children(id)
+                dataframe = pd.concat([dataframe, self._get_recursive_ids_prams(ids, params, get_sub_family)],
+                                      ignore_index=True)
+                continue
+            # get instances
+            ins = self.get_instance(id)
+            if len(ins) > 0:
+                for instance in ins:
+                    types = self.get_all_properties(instance)
+                    types = {k: v for k, v in types.items() if k in params}
+                    properties = {**properties, **types}
+            single_df = pd.DataFrame(properties, index=[0])
+            dataframe = pd.concat([dataframe, single_df], ignore_index=True)
+            ids = self.get_children(id)
+            dataframe = pd.concat([dataframe, self._get_recursive_ids_prams(ids, params, get_sub_family)],
+                                  ignore_index=True)
+        # set dbid and external_id to first and second column if it exists
+        if 'dbId' in dataframe.columns and 'external_id' in dataframe.columns:
+            dataframe = dataframe[
+                ['dbId', 'external_id'] + [col for col in dataframe.columns if col not in ['dbId', 'external_id']]]
+        return dataframe
+
+    def get_data_by_external_id(self, external_id, is_get_sub_family=False) -> pd.DataFrame:
+        db_id = None
+        for idx in range(0, len(self.ids)):
+            if self.ids[idx] == external_id:
+                db_id = idx
+                break
+        if db_id is None:
+            return pd.DataFrame()
+        dataframe = self._get_recursive_ids([db_id], is_get_sub_family)
+        return dataframe
+
+    def get_data_by_element_id(self, element_id) -> dict:
+        rg = re.compile(r'^__\w+__$')
+        properties = {}
+        for i in range(0, len(self.ids)):
+            props = self.enumerate_properties(i)
+            for prop in props:
+                if prop.name == "ElementId" and prop.value == str(element_id):
+                    for prop in props:
+                        if not rg.match(prop.category):
+                            properties[prop.name] = prop.value
+                    # get instance
+                    instances = self.get_instance(i)
+                    for instance in instances:
+                        types = self.get_properties(instance)
+                        properties = {**properties, **types}
+                    break
+        properties = dict(sorted(properties.items()))
+        return properties
+
+    def get_all_parameters(self) -> List:
+        parameters = []
+        for id in range(0, len(self.ids)):
+            props_dict = self.get_properties(id)
+            for key, value in props_dict.items():
+                if key not in parameters:
+                    parameters.append(key)
+        parameters = list(set(parameters))
+        parameters.sort()
+        return parameters
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/PropReader.py` & `aps-toolkit-0.5.4/src/aps_toolkit/PropReader.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,313 +1,313 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import gzip
-import json
-import re
-import codecs
-import requests
-from .Derivative import Derivative
-from .ManifestItem import ManifestItem
-import pandas as pd
-from typing import List
-
-
-class PropReader:
-
-    def __init__(self, urn, token, region="US", manifest_item: [ManifestItem] = None):
-        # get manifest
-        self.host = "https://developer.api.autodesk.com"
-        self.urn = urn
-        self.token = token
-        self.region = region
-        if manifest_item:
-            derivative = Derivative(self.urn, self.token, self.region)
-            self._read_metadata_item(derivative, manifest_item)
-        else:
-            self._read_metadata()
-
-    def _read_metadata(self):
-        derivative = Derivative(self.urn, self.token, self.region)
-        manifest_items = derivative.read_svf_manifest_items()
-        if len(manifest_items) > 0:
-            self._read_metadata_item(derivative, manifest_items[0])
-        else:
-            raise Exception("No manifest item found")
-
-    def _read_metadata_item(self, derivative, manifest_item):
-        items = [
-            "objects_attrs.json.gz",
-            "objects_vals.json.gz",
-            "objects_ids.json.gz",
-            "objects_offs.json.gz",
-            "objects_avs.json.gz",
-            "objects_ids.json.gz"
-        ]
-        resources = derivative.read_svf_resource_item(manifest_item)
-        # filters just get items
-        downloaded_files = {}
-        access_token = self.token.access_token
-        if not access_token:
-            raise Exception("No access token found")
-        headers = {
-            "Authorization": f"Bearer {access_token}",
-            "region": self.region
-        }
-        for source in resources:
-            if source.file_name in items:
-                downloaded_files[source.file_name] = source.url
-                response = requests.get(source.url, headers=headers)
-                if response.status_code == 200:
-                    file_bytes = response.content
-                    downloaded_files[source.file_name] = file_bytes
-        self.ids = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_ids.json.gz"]), 'utf-8'))
-        self.offsets = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_offs.json.gz"]), 'utf-8'))
-        self.avs = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_avs.json.gz"]), 'utf-8'))
-        self.attrs = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_attrs.json.gz"]), 'utf-8'))
-        self.vals = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_vals.json.gz"]), 'utf-8'))
-
-    def enumerate_properties(self, id) -> list:
-        properties = []
-        if 0 < id < len(self.offsets):
-            av_start = 2 * self.offsets[id]
-            av_end = len(self.avs) if id == len(self.offsets) - 1 else 2 * self.offsets[id + 1]
-            for i in range(av_start, av_end, 2):
-                attr_offset = self.avs[i]
-                val_offset = self.avs[i + 1]
-                attr_obj = self.attrs[attr_offset]
-
-                # Check if attr_obj is a list and has at least two elements
-                if isinstance(attr_obj, list) and len(attr_obj) >= 2:
-                    property_id = self.ids[id]
-                    name = attr_obj[0]
-                    category = attr_obj[1]
-                    data_type = self.attrs[2]
-                    data_type_context = attr_obj[3]
-                    description = attr_obj[4]
-                    display_name = attr_obj[5]
-                    flags = attr_obj[6]
-                    display_precision = attr_obj[7]
-                    forge_parameter_id = attr_obj[8]
-                value = self.vals[val_offset]
-                properties.append(
-                    Property(property_id, name, category, data_type, data_type_context, description, display_name,
-                             flags,
-                             display_precision, forge_parameter_id, value))
-        return properties
-
-    """
-    Get all properties exclude internal properties
-    """
-
-    def get_properties(self, id) -> dict:
-        props = {}
-        rg = re.compile(r'^__\w+__$')
-        for prop in self.enumerate_properties(id):
-            if prop.category and not rg.match(prop.category):
-                props[prop.name] = prop.value
-        return props
-
-    """
-    Get all properties include internal properties
-    """
-
-    def get_all_properties(self, id) -> dict:
-        props = {}
-        for prop in self.enumerate_properties(id):
-            props[prop.name] = prop.value
-        return props
-
-    def get_property_values_by_names(self, names: List[str]) -> dict:
-        result = {}
-        for i in range(len(self.offsets)):
-            av_start = 2 * self.offsets[i]
-            av_end = len(self.avs) if i == len(self.offsets) - 1 else 2 * self.offsets[i + 1]
-            for j in range(av_start, av_end, 2):
-                attr_offset = self.avs[j]
-                attr_obj = self.attrs[attr_offset]
-                if isinstance(attr_obj, list) and len(attr_obj) >= 2:
-                    name = attr_obj[0]
-                    if name in names:
-                        value = self.vals[self.avs[j + 1]]
-                        values = result.get(name, [])
-                        if value not in values:
-                            values.append(value)
-                            result[name] = values
-        return result
-
-    def get_property_values_by_display_names(self, display_names: List[str]) -> dict:
-        result = {}
-        for i in range(len(self.offsets)):
-            av_start = 2 * self.offsets[i]
-            av_end = len(self.avs) if i == len(self.offsets) - 1 else 2 * self.offsets[i + 1]
-            for j in range(av_start, av_end, 2):
-                attr_offset = self.avs[j]
-                attr_obj = self.attrs[attr_offset]
-                if isinstance(attr_obj, list) and len(attr_obj) >= 2:
-                    display_name = attr_obj[5]
-                    if display_name in display_names:
-                        value = self.vals[self.avs[j + 1]]
-                        values = result.get(display_name, [])
-                        if value not in values:
-                            values.append(value)
-                            result[display_name] = values
-
-        return result
-
-    def get_properties_group_by_category(self, id) -> dict:
-        properties = {}
-        rg = re.compile(r'^__\w+__$')
-        categories = []
-
-        props = self.enumerate_properties(id)
-        for prop in props:
-            if prop.category:
-                if not rg.match(prop.category):
-                    if not any(category in prop.category for category in categories):
-                        categories.append(prop.category)
-
-        for category in categories:
-            prop_result = [prop for prop in props if prop.category == category]
-            prop_dictionary = []
-            for prop in prop_result:
-                prop_key = prop.name
-                prop_dictionary.append((prop_key, prop.value))
-            properties[category] = prop_dictionary
-
-        return properties
-
-    def get_children(self, id) -> list:
-        children = []
-        for prop in self.enumerate_properties(id):
-            if prop.category == "__child__":
-                children.append(int(prop.value))
-        return children
-
-    def get_parent(self, id) -> list:
-        parent = []
-        for prop in self.enumerate_properties(id):
-            if prop.category == "__parent__":
-                parent.append(int(prop.value))
-        return parent
-
-    def get_instance(self, id) -> list:
-        instance_of = []
-        for prop in self.enumerate_properties(id):
-            if prop.category == "__instanceof__":
-                instance_of.append(int(prop.value))
-        return instance_of
-
-    def get_internal_ref(self, id) -> list:
-        reference = []
-        for prop in self.enumerate_properties(id):
-            if prop.category == "__internalref__":
-                reference.append(int(prop.value))
-
-    # TODO : It too slow, need find another way to get all data with less time and cover all format : dwg, rvt, nwd, ifc, ...
-    # def get_all_data(self) -> pd.DataFrame:
-    #     db_index_ids = [i for i in range(len(self.offsets))]
-    #     return self.get_recursive_ids(db_index_ids)
-
-    def get_recursive_ids(self, db_ids: List[int]) -> pd.DataFrame:
-        dataframe = pd.DataFrame()
-        props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
-        if len(db_ids) == 0:
-            return dataframe
-        for id in db_ids:
-            props = self.enumerate_properties(id)
-            properties = {}
-            for prop in props:
-                if prop.name == 'name':
-                    continue
-                if prop.name not in props_ignore:
-                    properties[prop.name] = prop.value
-            db_id = id
-            properties['dbId'] = db_id
-            ins = self.get_instance(id)
-            if len(ins) > 0:
-                for instance in ins:
-                    types = self.get_properties(instance)
-                    properties = {**properties, **types}
-            singleDF = pd.DataFrame(properties, index=[0])
-            dataframe = pd.concat([dataframe, singleDF], ignore_index=True)
-            ids = self.get_children(id)
-            dataframe = pd.concat([dataframe, self.get_recursive_ids(ids)], ignore_index=True)
-        if 'dbId' in dataframe.columns:
-            dataframe = dataframe[
-                ['dbId'] + [col for col in dataframe.columns if col not in ['dbId']]]
-        return dataframe
-
-    def get_recursive_ids_by_parameters(self, db_ids: List[int], params: List[str]) -> pd.DataFrame:
-        dataframe = pd.DataFrame()
-        props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
-        if len(db_ids) == 0:
-            return dataframe
-        for id in db_ids:
-            props = self.enumerate_properties(id)
-            properties = {}
-            for prop in props:
-                if prop.name == 'name':
-                    continue
-                if prop.name not in props_ignore:
-                    properties[prop.name] = prop.value
-            db_id = id
-            properties = {k: v for k, v in properties.items() if k in params}
-            properties['dbId'] = db_id
-            ins = self.get_instance(id)
-            if len(ins) > 0:
-                for instance in ins:
-                    types = self.get_properties(instance)
-                    types = {k: v for k, v in types.items() if k in params}
-                    properties = {**properties, **types}
-            singleDF = pd.DataFrame(properties, index=[0])
-            dataframe = pd.concat([dataframe, singleDF], ignore_index=True)
-            ids = self.get_children(id)
-            dataframe = pd.concat([dataframe, self.get_recursive_ids_by_parameters(ids, params)], ignore_index=True)
-        if 'dbId' in dataframe.columns:
-            dataframe = dataframe[['dbId'] + [col for col in dataframe.columns if col not in ['dbId']]]
-        return dataframe
-
-    def get_all_properties_names(self) -> List[str]:
-        props_names = []
-        for i in range(len(self.offsets)):
-            av_start = 2 * self.offsets[i]
-            av_end = len(self.avs) if i == len(self.offsets) - 1 else 2 * self.offsets[i + 1]
-            for j in range(av_start, av_end, 2):
-                attr_offset = self.avs[j]
-                attr_obj = self.attrs[attr_offset]
-                if isinstance(attr_obj, list) and len(attr_obj) >= 2:
-                    name = attr_obj[0]
-                    props_names.append(name)
-        props_names = list(set(props_names))
-        props_names.sort()
-        return props_names
-
-
-class Property():
-    def __init__(self, id=None, name=None, category=None, data_type=None, data_type_context=None, description=None,
-                 display_name=None, flags=None,
-                 display_precision=None, forge_parameter_id=None, value=None):
-        self.id = id,
-        self.name = name
-        self.category = category
-        self.data_type = data_type
-        self.data_type_context = data_type_context
-        self.description = description
-        self.display_name = display_name
-        self.flags = flags
-        self.display_precision = display_precision
-        self.forge_parameter_id = forge_parameter_id
-        self.value = value
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+import gzip
+import json
+import re
+import codecs
+import requests
+from .Derivative import Derivative
+from .ManifestItem import ManifestItem
+import pandas as pd
+from typing import List
+
+
+class PropReader:
+
+    def __init__(self, urn, token, region="US", manifest_item: [ManifestItem] = None):
+        # get manifest
+        self.host = "https://developer.api.autodesk.com"
+        self.urn = urn
+        self.token = token
+        self.region = region
+        if manifest_item:
+            derivative = Derivative(self.urn, self.token, self.region)
+            self._read_metadata_item(derivative, manifest_item)
+        else:
+            self._read_metadata()
+
+    def _read_metadata(self):
+        derivative = Derivative(self.urn, self.token, self.region)
+        manifest_items = derivative.read_svf_manifest_items()
+        if len(manifest_items) > 0:
+            self._read_metadata_item(derivative, manifest_items[0])
+        else:
+            raise Exception("No manifest item found")
+
+    def _read_metadata_item(self, derivative, manifest_item):
+        items = [
+            "objects_attrs.json.gz",
+            "objects_vals.json.gz",
+            "objects_ids.json.gz",
+            "objects_offs.json.gz",
+            "objects_avs.json.gz",
+            "objects_ids.json.gz"
+        ]
+        resources = derivative.read_svf_resource_item(manifest_item)
+        # filters just get items
+        downloaded_files = {}
+        access_token = self.token.access_token
+        if not access_token:
+            raise Exception("No access token found")
+        headers = {
+            "Authorization": f"Bearer {access_token}",
+            "region": self.region
+        }
+        for source in resources:
+            if source.file_name in items:
+                downloaded_files[source.file_name] = source.url
+                response = requests.get(source.url, headers=headers)
+                if response.status_code == 200:
+                    file_bytes = response.content
+                    downloaded_files[source.file_name] = file_bytes
+        self.ids = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_ids.json.gz"]), 'utf-8'))
+        self.offsets = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_offs.json.gz"]), 'utf-8'))
+        self.avs = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_avs.json.gz"]), 'utf-8'))
+        self.attrs = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_attrs.json.gz"]), 'utf-8'))
+        self.vals = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_vals.json.gz"]), 'utf-8'))
+
+    def enumerate_properties(self, id) -> list:
+        properties = []
+        if 0 < id < len(self.offsets):
+            av_start = 2 * self.offsets[id]
+            av_end = len(self.avs) if id == len(self.offsets) - 1 else 2 * self.offsets[id + 1]
+            for i in range(av_start, av_end, 2):
+                attr_offset = self.avs[i]
+                val_offset = self.avs[i + 1]
+                attr_obj = self.attrs[attr_offset]
+
+                # Check if attr_obj is a list and has at least two elements
+                if isinstance(attr_obj, list) and len(attr_obj) >= 2:
+                    property_id = self.ids[id]
+                    name = attr_obj[0]
+                    category = attr_obj[1]
+                    data_type = self.attrs[2]
+                    data_type_context = attr_obj[3]
+                    description = attr_obj[4]
+                    display_name = attr_obj[5]
+                    flags = attr_obj[6]
+                    display_precision = attr_obj[7]
+                    forge_parameter_id = attr_obj[8]
+                value = self.vals[val_offset]
+                properties.append(
+                    Property(property_id, name, category, data_type, data_type_context, description, display_name,
+                             flags,
+                             display_precision, forge_parameter_id, value))
+        return properties
+
+    """
+    Get all properties exclude internal properties
+    """
+
+    def get_properties(self, id) -> dict:
+        props = {}
+        rg = re.compile(r'^__\w+__$')
+        for prop in self.enumerate_properties(id):
+            if prop.category and not rg.match(prop.category):
+                props[prop.name] = prop.value
+        return props
+
+    """
+    Get all properties include internal properties
+    """
+
+    def get_all_properties(self, id) -> dict:
+        props = {}
+        for prop in self.enumerate_properties(id):
+            props[prop.name] = prop.value
+        return props
+
+    def get_property_values_by_names(self, names: List[str]) -> dict:
+        result = {}
+        for i in range(len(self.offsets)):
+            av_start = 2 * self.offsets[i]
+            av_end = len(self.avs) if i == len(self.offsets) - 1 else 2 * self.offsets[i + 1]
+            for j in range(av_start, av_end, 2):
+                attr_offset = self.avs[j]
+                attr_obj = self.attrs[attr_offset]
+                if isinstance(attr_obj, list) and len(attr_obj) >= 2:
+                    name = attr_obj[0]
+                    if name in names:
+                        value = self.vals[self.avs[j + 1]]
+                        values = result.get(name, [])
+                        if value not in values:
+                            values.append(value)
+                            result[name] = values
+        return result
+
+    def get_property_values_by_display_names(self, display_names: List[str]) -> dict:
+        result = {}
+        for i in range(len(self.offsets)):
+            av_start = 2 * self.offsets[i]
+            av_end = len(self.avs) if i == len(self.offsets) - 1 else 2 * self.offsets[i + 1]
+            for j in range(av_start, av_end, 2):
+                attr_offset = self.avs[j]
+                attr_obj = self.attrs[attr_offset]
+                if isinstance(attr_obj, list) and len(attr_obj) >= 2:
+                    display_name = attr_obj[5]
+                    if display_name in display_names:
+                        value = self.vals[self.avs[j + 1]]
+                        values = result.get(display_name, [])
+                        if value not in values:
+                            values.append(value)
+                            result[display_name] = values
+
+        return result
+
+    def get_properties_group_by_category(self, id) -> dict:
+        properties = {}
+        rg = re.compile(r'^__\w+__$')
+        categories = []
+
+        props = self.enumerate_properties(id)
+        for prop in props:
+            if prop.category:
+                if not rg.match(prop.category):
+                    if not any(category in prop.category for category in categories):
+                        categories.append(prop.category)
+
+        for category in categories:
+            prop_result = [prop for prop in props if prop.category == category]
+            prop_dictionary = []
+            for prop in prop_result:
+                prop_key = prop.name
+                prop_dictionary.append((prop_key, prop.value))
+            properties[category] = prop_dictionary
+
+        return properties
+
+    def get_children(self, id) -> list:
+        children = []
+        for prop in self.enumerate_properties(id):
+            if prop.category == "__child__":
+                children.append(int(prop.value))
+        return children
+
+    def get_parent(self, id) -> list:
+        parent = []
+        for prop in self.enumerate_properties(id):
+            if prop.category == "__parent__":
+                parent.append(int(prop.value))
+        return parent
+
+    def get_instance(self, id) -> list:
+        instance_of = []
+        for prop in self.enumerate_properties(id):
+            if prop.category == "__instanceof__":
+                instance_of.append(int(prop.value))
+        return instance_of
+
+    def get_internal_ref(self, id) -> list:
+        reference = []
+        for prop in self.enumerate_properties(id):
+            if prop.category == "__internalref__":
+                reference.append(int(prop.value))
+
+    # TODO : It too slow, need find another way to get all data with less time and cover all format : dwg, rvt, nwd, ifc, ...
+    # def get_all_data(self) -> pd.DataFrame:
+    #     db_index_ids = [i for i in range(len(self.offsets))]
+    #     return self.get_recursive_ids(db_index_ids)
+
+    def get_recursive_ids(self, db_ids: List[int]) -> pd.DataFrame:
+        dataframe = pd.DataFrame()
+        props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
+        if len(db_ids) == 0:
+            return dataframe
+        for id in db_ids:
+            props = self.enumerate_properties(id)
+            properties = {}
+            for prop in props:
+                if prop.name == 'name':
+                    continue
+                if prop.name not in props_ignore:
+                    properties[prop.name] = prop.value
+            db_id = id
+            properties['dbId'] = db_id
+            ins = self.get_instance(id)
+            if len(ins) > 0:
+                for instance in ins:
+                    types = self.get_properties(instance)
+                    properties = {**properties, **types}
+            singleDF = pd.DataFrame(properties, index=[0])
+            dataframe = pd.concat([dataframe, singleDF], ignore_index=True)
+            ids = self.get_children(id)
+            dataframe = pd.concat([dataframe, self.get_recursive_ids(ids)], ignore_index=True)
+        if 'dbId' in dataframe.columns:
+            dataframe = dataframe[
+                ['dbId'] + [col for col in dataframe.columns if col not in ['dbId']]]
+        return dataframe
+
+    def get_recursive_ids_by_parameters(self, db_ids: List[int], params: List[str]) -> pd.DataFrame:
+        dataframe = pd.DataFrame()
+        props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
+        if len(db_ids) == 0:
+            return dataframe
+        for id in db_ids:
+            props = self.enumerate_properties(id)
+            properties = {}
+            for prop in props:
+                if prop.name == 'name':
+                    continue
+                if prop.name not in props_ignore:
+                    properties[prop.name] = prop.value
+            db_id = id
+            properties = {k: v for k, v in properties.items() if k in params}
+            properties['dbId'] = db_id
+            ins = self.get_instance(id)
+            if len(ins) > 0:
+                for instance in ins:
+                    types = self.get_properties(instance)
+                    types = {k: v for k, v in types.items() if k in params}
+                    properties = {**properties, **types}
+            singleDF = pd.DataFrame(properties, index=[0])
+            dataframe = pd.concat([dataframe, singleDF], ignore_index=True)
+            ids = self.get_children(id)
+            dataframe = pd.concat([dataframe, self.get_recursive_ids_by_parameters(ids, params)], ignore_index=True)
+        if 'dbId' in dataframe.columns:
+            dataframe = dataframe[['dbId'] + [col for col in dataframe.columns if col not in ['dbId']]]
+        return dataframe
+
+    def get_all_properties_names(self) -> List[str]:
+        props_names = []
+        for i in range(len(self.offsets)):
+            av_start = 2 * self.offsets[i]
+            av_end = len(self.avs) if i == len(self.offsets) - 1 else 2 * self.offsets[i + 1]
+            for j in range(av_start, av_end, 2):
+                attr_offset = self.avs[j]
+                attr_obj = self.attrs[attr_offset]
+                if isinstance(attr_obj, list) and len(attr_obj) >= 2:
+                    name = attr_obj[0]
+                    props_names.append(name)
+        props_names = list(set(props_names))
+        props_names.sort()
+        return props_names
+
+
+class Property():
+    def __init__(self, id=None, name=None, category=None, data_type=None, data_type_context=None, description=None,
+                 display_name=None, flags=None,
+                 display_precision=None, forge_parameter_id=None, value=None):
+        self.id = id,
+        self.name = name
+        self.category = category
+        self.data_type = data_type
+        self.data_type_context = data_type_context
+        self.description = description
+        self.display_name = display_name
+        self.flags = flags
+        self.display_precision = display_precision
+        self.forge_parameter_id = forge_parameter_id
+        self.value = value
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/Resource.py` & `aps-toolkit-0.5.4/src/aps_toolkit/Resource.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-from urllib.parse import urljoin, quote
-
-
-class Resource:
-    def __init__(self, file_name, remote_path, local_path):
-        self.host = "https://developer.api.autodesk.com"
-        self.file_name = file_name
-        self.remote_path = self._resolve_path_slashes(remote_path)
-        self.url = self._resolve_url(remote_path)
-        self.local_path = self._resolve_path_slashes(local_path)
-
-    def _resolve_path_slashes(self, path):
-        url_with_forward_slashes = path.replace('\\', '/')
-        return url_with_forward_slashes
-
-    def _resolve_url(self, remote_path):
-        url_with_forward_slashes = remote_path.replace('\\', '/')
-        return urljoin(self.host, quote(url_with_forward_slashes, safe=':/'))
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+from urllib.parse import urljoin, quote
+
+
+class Resource:
+    def __init__(self, file_name, remote_path, local_path):
+        self.host = "https://developer.api.autodesk.com"
+        self.file_name = file_name
+        self.remote_path = self._resolve_path_slashes(remote_path)
+        self.url = self._resolve_url(remote_path)
+        self.local_path = self._resolve_path_slashes(local_path)
+
+    def _resolve_path_slashes(self, path):
+        url_with_forward_slashes = path.replace('\\', '/')
+        return url_with_forward_slashes
+
+    def _resolve_url(self, remote_path):
+        url_with_forward_slashes = remote_path.replace('\\', '/')
+        return urljoin(self.host, quote(url_with_forward_slashes, safe=':/'))
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFContent.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFContent.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-
-class SVFContent:
-    def __init__(self, metadata=None, fragments=None, geometries=None, meshpacks=None, materials=None, properties=None,
-                 images=None):
-        self.metadata = metadata
-        self.fragments = fragments
-        self.geometries = geometries
-        self.meshpacks = meshpacks
-        self.materials = materials
-        self.properties = properties
-        self.images = images
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+
+class SVFContent:
+    def __init__(self, metadata=None, fragments=None, geometries=None, meshpacks=None, materials=None, properties=None,
+                 images=None):
+        self.metadata = metadata
+        self.fragments = fragments
+        self.geometries = geometries
+        self.meshpacks = meshpacks
+        self.materials = materials
+        self.properties = properties
+        self.images = images
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFGeometries.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFGeometries.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-from .Derivative import Derivative
-from .PackFileReader import PackFileReader
-from .ManifestItem import ManifestItem
-
-
-class SVFGeometries:
-    def __init__(self, frag_type=None, prim_count=None, pack_id=None, entity_id=None, topo_id=None):
-        self.fragment_type = frag_type
-        self.primitive_count = prim_count
-        self.pack_id = pack_id
-        self.entity_id = entity_id
-        self.topo_id = topo_id
-
-    @staticmethod
-    def parse_geometries_from_urn(urn, token, region="US") -> dict:
-        """
-        Parse geometries from urn
-        :param urn: the urn of the model
-        :param token: the token authentication
-        :param region:  the region of hub (default is US)
-        :return:  a dictionary of geometries with key is the guid of the manifest item and value is the list of geometries
-        """
-        geometries = {}
-        derivative = Derivative(urn, token, region)
-        manifest_items = derivative.read_svf_manifest_items()
-        for manifest_item in manifest_items:
-            geos = SVFGeometries.parse_geos_from_manifest_item(derivative, manifest_item)
-            geometries[manifest_item.guid] = geos
-        return geometries
-
-    @staticmethod
-    def parse_geos_from_manifest_item(derivative: [Derivative], manifest_item: [ManifestItem]) -> list:
-        geometries = []
-        resources = derivative.read_svf_resource_item(manifest_item)
-        for resource in resources:
-            if resource.local_path.endswith("GeometryMetadata.pf"):
-                bytes_io = derivative.download_stream_resource(resource)
-                buffer = bytes_io.read()
-                geos = SVFGeometries.parse_geometries(buffer)
-                geometries.extend(geos)
-        return geometries
-
-    @staticmethod
-    def parse_geometries(buffer) -> list:
-        """
-        Parse geometries from buffer
-        :param buffer:  the buffer of the geometry metadata file
-        :return:  a list of geometries
-        """
-        geometries = []
-        pfr = PackFileReader(buffer)
-        for i in range(pfr.num_entries()):
-            entry = pfr.seek_entry(i)
-            if entry is not None and entry.version >= 3:
-                frag_type = pfr.get_uint8()
-                # Skip past object space bbox -- we don't use that
-                pfr.seek(pfr.offset + 24)
-                prim_count = pfr.get_uint16()
-                p_id = pfr.get_string(pfr.get_varint()).replace(".pf", "")
-                pack_id = int(p_id)
-                entity_id = pfr.get_varint()
-                geometry = SVFGeometries(frag_type, prim_count, pack_id, entity_id)
-                geometries.append(geometry)
-
-        return geometries
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+from .Derivative import Derivative
+from .PackFileReader import PackFileReader
+from .ManifestItem import ManifestItem
+
+
+class SVFGeometries:
+    def __init__(self, frag_type=None, prim_count=None, pack_id=None, entity_id=None, topo_id=None):
+        self.fragment_type = frag_type
+        self.primitive_count = prim_count
+        self.pack_id = pack_id
+        self.entity_id = entity_id
+        self.topo_id = topo_id
+
+    @staticmethod
+    def parse_geometries_from_urn(urn, token, region="US") -> dict:
+        """
+        Parse geometries from urn
+        :param urn: the urn of the model
+        :param token: the token authentication
+        :param region:  the region of hub (default is US)
+        :return:  a dictionary of geometries with key is the guid of the manifest item and value is the list of geometries
+        """
+        geometries = {}
+        derivative = Derivative(urn, token, region)
+        manifest_items = derivative.read_svf_manifest_items()
+        for manifest_item in manifest_items:
+            geos = SVFGeometries.parse_geos_from_manifest_item(derivative, manifest_item)
+            geometries[manifest_item.guid] = geos
+        return geometries
+
+    @staticmethod
+    def parse_geos_from_manifest_item(derivative: [Derivative], manifest_item: [ManifestItem]) -> list:
+        geometries = []
+        resources = derivative.read_svf_resource_item(manifest_item)
+        for resource in resources:
+            if resource.local_path.endswith("GeometryMetadata.pf"):
+                bytes_io = derivative.download_stream_resource(resource)
+                buffer = bytes_io.read()
+                geos = SVFGeometries.parse_geometries(buffer)
+                geometries.extend(geos)
+        return geometries
+
+    @staticmethod
+    def parse_geometries(buffer) -> list:
+        """
+        Parse geometries from buffer
+        :param buffer:  the buffer of the geometry metadata file
+        :return:  a list of geometries
+        """
+        geometries = []
+        pfr = PackFileReader(buffer)
+        for i in range(pfr.num_entries()):
+            entry = pfr.seek_entry(i)
+            if entry is not None and entry.version >= 3:
+                frag_type = pfr.get_uint8()
+                # Skip past object space bbox -- we don't use that
+                pfr.seek(pfr.offset + 24)
+                prim_count = pfr.get_uint16()
+                p_id = pfr.get_string(pfr.get_varint()).replace(".pf", "")
+                pack_id = int(p_id)
+                entity_id = pfr.get_varint()
+                geometry = SVFGeometries(frag_type, prim_count, pack_id, entity_id)
+                geometries.append(geometry)
+
+        return geometries
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFLines.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFLines.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-class SVFLines:
-    def __init__(self, isLines=False, v_count=None, l_count=None, vertices=None, indices=None, colors=None,
-                 line_width=None):
-        self.isLines = isLines
-        self.v_count = v_count
-        self.l_count = l_count
-        self.vertices = vertices
-        self.indices = indices
-        self.colors = colors
-        self.line_width = line_width
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+class SVFLines:
+    def __init__(self, isLines=False, v_count=None, l_count=None, vertices=None, indices=None, colors=None,
+                 line_width=None):
+        self.isLines = isLines
+        self.v_count = v_count
+        self.l_count = l_count
+        self.vertices = vertices
+        self.indices = indices
+        self.colors = colors
+        self.line_width = line_width
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFManifestType.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFManifestType.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-class SVFManifestType:
-    def __init__(self, type_class="", type="", version=0):
-        self.type_class = type_class
-        self.type = type
-        self.version = version
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+class SVFManifestType:
+    def __init__(self, type_class="", type="", version=0):
+        self.type_class = type_class
+        self.type = type
+        self.version = version
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFMaterialGroup.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFMaterialGroup.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-from .Materials import Materials
-
-
-class SVFMaterialGroup:
-    def __init__(self, version, userassets, materials: [Materials]):
-        self.version = version
-        self.userassets = userassets
-        self.materials = materials
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+from .Materials import Materials
+
+
+class SVFMaterialGroup:
+    def __init__(self, version, userassets, materials: [Materials]):
+        self.version = version
+        self.userassets = userassets
+        self.materials = materials
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFMaterialMap.py` & `aps-toolkit-0.5.4/src/aps_toolkit/Token.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-class SVFMaterialMap:
-    def __init__(self, uri=None, scale=None):
-        self.uri = uri
-        self.scale = scale
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+
+class Token():
+    def __init__(self, access_token, token_type, expires_in, refresh_token=None):
+        self.access_token = access_token
+        self.token_type = token_type
+        self.expires_in = expires_in
+        self.refresh_token = refresh_token
+
+    def is_expired(self) -> bool:
+        return self.expires_in <= 0
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFMaterialMapScale.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFMaterialMapScale.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-class SVFMaterialMapScale:
-    def __init__(self, texture_u_scale, texture_v_scale):
-        self.texture_u_scale = texture_u_scale
-        self.texture_v_scale = texture_v_scale
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+class SVFMaterialMapScale:
+    def __init__(self, texture_u_scale, texture_v_scale):
+        self.texture_u_scale = texture_u_scale
+        self.texture_v_scale = texture_v_scale
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFMaterials.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFMaterials.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-from .MaterialProperties import MaterialProperties
-from .SVFMaterialMap import SVFMaterialMap
-from .SVFMaterialMapScale import SVFMaterialMapScale
-from .SVFMaterialGroup import SVFMaterialGroup
-from .Materials import Materials
-import json
-from .PackFileReader import PackFileReader
-from .Derivative import Derivative
-from .ManifestItem import ManifestItem
-
-
-class SVFMaterials:
-    def __init__(self):
-        pass
-
-    @staticmethod
-    def parse_materials_from_urn(urn, token, region="US") -> dict[str, list[Materials]]:
-        materials = {}
-        derivative = Derivative(urn, token, region)
-        manifest_items = derivative.read_svf_manifest_items()
-        for manifest_item in manifest_items:
-            mats = SVFMaterials.parse_materials_from_manifest_item(derivative, manifest_item)
-            materials[manifest_item.guid] = mats
-        return materials
-
-    @staticmethod
-    def parse_materials_from_manifest_item(derivative: [Derivative], manifest_item: [ManifestItem]) -> list[Materials]:
-        resources = derivative.read_svf_resource_item(manifest_item)
-        materials = []
-        for resource in resources:
-            if resource.local_path.endswith("Materials.json.gz"):
-                bytes_io = derivative.download_stream_resource(resource)
-                buffer = bytes_io.read()
-                mats = SVFMaterials.parse_materials(buffer)
-                materials.extend(mats)
-        return materials
-
-    @staticmethod
-    def parse_materials_from_file(file_path) -> list[Materials]:
-        with open(file_path, "rb") as file:
-            buffer = file.read()
-            return SVFMaterials.parse_materials(buffer)
-
-    @staticmethod
-    def parse_materials(buffer) -> list[Materials]:
-        materials = []
-
-        # Decompress buffer (assuming it's already implemented)
-        buffer = PackFileReader.decompress_buffer(buffer)
-
-        if len(buffer) > 0:
-            # Decode buffer to string assuming default encoding
-            json_str = buffer.decode()
-
-            # Deserialize JSON string to Materials object
-            svf_mat = json.loads(json_str)
-            for key, group in svf_mat['materials'].items():
-                group_materials = SVFMaterialGroup(**group)
-                material = group_materials.materials[group_materials.userassets[0]]
-                material = Materials(**material)
-                if str(material.definition) == 'SimplePhong':
-                    materials.append(SVFMaterials.parse_simple_phong_material(group_materials))
-                else:
-                    print("Unsupported material definition:", material.definition)
-
-        return materials
-
-    @staticmethod
-    def parse_simple_phong_material(group: [SVFMaterialGroup]):
-        result = Materials()
-        material = Materials(**group.materials[group.userassets[0]])
-
-        result.diffuse = SVFMaterials.parse_color_property(material, "generic_diffuse", [0, 0, 0, 1])
-        result.specular = SVFMaterials.parse_color_property(material, "generic_specular", [0, 0, 0, 1])
-        result.ambient = SVFMaterials.parse_color_property(material, "generic_ambient", [0, 0, 0, 1])
-        result.emissive = SVFMaterials.parse_color_property(material, "generic_emissive", [0, 0, 0, 1])
-
-        result.glossiness = SVFMaterials.parse_scalar_property(material, "generic_glossiness", 30)
-        result.reflectivity = SVFMaterials.parse_scalar_property(material, "generic_reflectivity_at_0deg", 0)
-        result.opacity = 1.0 - SVFMaterials.parse_scalar_property(material, "generic_transparency", 0)
-
-        result.metal = SVFMaterials.parse_boolean_property(material, "generic_is_metal", False)
-
-        if material.textures:
-            maps = SVFMaterialMap()
-            diffuse = SVFMaterials.parse_texture_property(material, group, "generic_diffuse")
-            if diffuse:
-                maps.diffuse = diffuse
-
-            specular = SVFMaterials.parse_texture_property(material, group, "generic_specular")
-            if specular:
-                maps.specular = specular
-
-            alpha = SVFMaterials.parse_texture_property(material, group, "generic_alpha")
-            if alpha:
-                maps.alpha = alpha
-
-            bump = SVFMaterials.parse_texture_property(material, group, "generic_bump")
-            if bump:
-                if SVFMaterials.parse_boolean_property(material, "generic_bump_is_normal", False):
-                    maps.normal = bump
-                else:
-                    maps.bump = bump
-
-            result.maps = maps
-
-        return result
-
-    @staticmethod
-    def parse_boolean_property(material: [Materials], prop, default_value) -> bool:
-        props = MaterialProperties(**material.properties)
-        if props.booleans is not None and prop in props.booleans:
-            return props.booleans[prop]
-        else:
-            return default_value
-
-    @staticmethod
-    def parse_scalar_property(material: [Materials], prop, default_value) -> float:
-        props = MaterialProperties(**material.properties)
-        if props.scalars is not None and prop in props.scalars:
-            return props.scalars[prop]["values"][0]
-        else:
-            return default_value
-
-    @staticmethod
-    def parse_color_property(material: [Materials], prop, default_value) -> [float]:
-        props = MaterialProperties(**material.properties)
-        if props.colors is not None and prop in props.colors:
-            color = props.colors[prop]["values"][0]
-            return [color["r"], color["g"], color["b"], color["a"]]
-        else:
-            return default_value
-
-    @staticmethod
-    def parse_texture_property(material: [Materials], group: [SVFMaterialGroup], prop: str) -> SVFMaterialMap:
-        if material.textures is not None and prop in material.textures:
-            connection = material.textures[prop]["connections"][0]
-            texture = group.materials[connection]
-            texture = SVFTexture(**texture)
-            mat_props = MaterialProperties(**texture.properties)
-            if "unifiedbitmap_Bitmap" in mat_props.uris:
-                uri = mat_props.uris["unifiedbitmap_Bitmap"]["values"][0]
-                texture_uscale, texture_vscale = 0.0, 0.0
-
-                if mat_props.scalars is not None \
-                        and "texture_UScale" in mat_props.scalars \
-                        and "texture_VScale" in mat_props.scalars:
-                    texture_uscale = mat_props.scalars["texture_UScale"]["values"][0]
-                    texture_vscale = mat_props.scalars["texture_VScale"]["values"][0]
-
-                if uri is not None:
-                    return SVFMaterialMap(uri=uri, scale=SVFMaterialMapScale(texture_uscale, texture_vscale))
-        return None
-
-
-class SVFTexture:
-    def __init__(self, tag=None, definition=None, properties=None):
-        self.tag = tag
-        self.definition = definition
-        self.properties = properties
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from .MaterialProperties import MaterialProperties
+from .SVFMaterialMap import SVFMaterialMap
+from .SVFMaterialMapScale import SVFMaterialMapScale
+from .SVFMaterialGroup import SVFMaterialGroup
+from .Materials import Materials
+import json
+from .PackFileReader import PackFileReader
+from .Derivative import Derivative
+from .ManifestItem import ManifestItem
+
+
+class SVFMaterials:
+    def __init__(self):
+        pass
+
+    @staticmethod
+    def parse_materials_from_urn(urn, token, region="US") -> dict[str, list[Materials]]:
+        materials = {}
+        derivative = Derivative(urn, token, region)
+        manifest_items = derivative.read_svf_manifest_items()
+        for manifest_item in manifest_items:
+            mats = SVFMaterials.parse_materials_from_manifest_item(derivative, manifest_item)
+            materials[manifest_item.guid] = mats
+        return materials
+
+    @staticmethod
+    def parse_materials_from_manifest_item(derivative: [Derivative], manifest_item: [ManifestItem]) -> list[Materials]:
+        resources = derivative.read_svf_resource_item(manifest_item)
+        materials = []
+        for resource in resources:
+            if resource.local_path.endswith("Materials.json.gz"):
+                bytes_io = derivative.download_stream_resource(resource)
+                buffer = bytes_io.read()
+                mats = SVFMaterials.parse_materials(buffer)
+                materials.extend(mats)
+        return materials
+
+    @staticmethod
+    def parse_materials_from_file(file_path) -> list[Materials]:
+        with open(file_path, "rb") as file:
+            buffer = file.read()
+            return SVFMaterials.parse_materials(buffer)
+
+    @staticmethod
+    def parse_materials(buffer) -> list[Materials]:
+        materials = []
+
+        # Decompress buffer (assuming it's already implemented)
+        buffer = PackFileReader.decompress_buffer(buffer)
+
+        if len(buffer) > 0:
+            # Decode buffer to string assuming default encoding
+            json_str = buffer.decode()
+
+            # Deserialize JSON string to Materials object
+            svf_mat = json.loads(json_str)
+            for key, group in svf_mat['materials'].items():
+                group_materials = SVFMaterialGroup(**group)
+                material = group_materials.materials[group_materials.userassets[0]]
+                material = Materials(**material)
+                if str(material.definition) == 'SimplePhong':
+                    materials.append(SVFMaterials.parse_simple_phong_material(group_materials))
+                else:
+                    print("Unsupported material definition:", material.definition)
+
+        return materials
+
+    @staticmethod
+    def parse_simple_phong_material(group: [SVFMaterialGroup]):
+        result = Materials()
+        material = Materials(**group.materials[group.userassets[0]])
+
+        result.diffuse = SVFMaterials.parse_color_property(material, "generic_diffuse", [0, 0, 0, 1])
+        result.specular = SVFMaterials.parse_color_property(material, "generic_specular", [0, 0, 0, 1])
+        result.ambient = SVFMaterials.parse_color_property(material, "generic_ambient", [0, 0, 0, 1])
+        result.emissive = SVFMaterials.parse_color_property(material, "generic_emissive", [0, 0, 0, 1])
+
+        result.glossiness = SVFMaterials.parse_scalar_property(material, "generic_glossiness", 30)
+        result.reflectivity = SVFMaterials.parse_scalar_property(material, "generic_reflectivity_at_0deg", 0)
+        result.opacity = 1.0 - SVFMaterials.parse_scalar_property(material, "generic_transparency", 0)
+
+        result.metal = SVFMaterials.parse_boolean_property(material, "generic_is_metal", False)
+
+        if material.textures:
+            maps = SVFMaterialMap()
+            diffuse = SVFMaterials.parse_texture_property(material, group, "generic_diffuse")
+            if diffuse:
+                maps.diffuse = diffuse
+
+            specular = SVFMaterials.parse_texture_property(material, group, "generic_specular")
+            if specular:
+                maps.specular = specular
+
+            alpha = SVFMaterials.parse_texture_property(material, group, "generic_alpha")
+            if alpha:
+                maps.alpha = alpha
+
+            bump = SVFMaterials.parse_texture_property(material, group, "generic_bump")
+            if bump:
+                if SVFMaterials.parse_boolean_property(material, "generic_bump_is_normal", False):
+                    maps.normal = bump
+                else:
+                    maps.bump = bump
+
+            result.maps = maps
+
+        return result
+
+    @staticmethod
+    def parse_boolean_property(material: [Materials], prop, default_value) -> bool:
+        props = MaterialProperties(**material.properties)
+        if props.booleans is not None and prop in props.booleans:
+            return props.booleans[prop]
+        else:
+            return default_value
+
+    @staticmethod
+    def parse_scalar_property(material: [Materials], prop, default_value) -> float:
+        props = MaterialProperties(**material.properties)
+        if props.scalars is not None and prop in props.scalars:
+            return props.scalars[prop]["values"][0]
+        else:
+            return default_value
+
+    @staticmethod
+    def parse_color_property(material: [Materials], prop, default_value) -> [float]:
+        props = MaterialProperties(**material.properties)
+        if props.colors is not None and prop in props.colors:
+            color = props.colors[prop]["values"][0]
+            return [color["r"], color["g"], color["b"], color["a"]]
+        else:
+            return default_value
+
+    @staticmethod
+    def parse_texture_property(material: [Materials], group: [SVFMaterialGroup], prop: str) -> SVFMaterialMap:
+        if material.textures is not None and prop in material.textures:
+            connection = material.textures[prop]["connections"][0]
+            texture = group.materials[connection]
+            texture = SVFTexture(**texture)
+            mat_props = MaterialProperties(**texture.properties)
+            if "unifiedbitmap_Bitmap" in mat_props.uris:
+                uri = mat_props.uris["unifiedbitmap_Bitmap"]["values"][0]
+                texture_uscale, texture_vscale = 0.0, 0.0
+
+                if mat_props.scalars is not None \
+                        and "texture_UScale" in mat_props.scalars \
+                        and "texture_VScale" in mat_props.scalars:
+                    texture_uscale = mat_props.scalars["texture_UScale"]["values"][0]
+                    texture_vscale = mat_props.scalars["texture_VScale"]["values"][0]
+
+                if uri is not None:
+                    return SVFMaterialMap(uri=uri, scale=SVFMaterialMapScale(texture_uscale, texture_vscale))
+        return None
+
+
+class SVFTexture:
+    def __init__(self, tag=None, definition=None, properties=None):
+        self.tag = tag
+        self.definition = definition
+        self.properties = properties
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFMesh.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFMesh.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,231 +1,231 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-from .SVFUVMap import SVFUVMap
-from .PackFileReader import PackFileReader
-import math
-from .SVFLines import SVFLines
-from .SVFPoints import SVFPoints
-from .Derivative import Derivative
-import re
-from .ManifestItem import ManifestItem
-
-
-class SVFMesh:
-    def __init__(self, v_count=None, t_count=None, uv_count=None, attrs=None, flags=None, comment=None,
-                 uv_maps: [SVFUVMap] = None,
-                 indices=None, vertices=None, normals=None, colors=None, min=None, max=None):
-        self.v_count = v_count
-        self.t_count = t_count
-        self.uv_count = uv_count
-        self.attrs = attrs
-        self.flags = flags
-        self.comment = comment
-        self.uv_maps = uv_maps
-        self.indices = indices
-        self.vertices = vertices
-        self.normals = normals
-        self.colors = colors
-        self.min = min
-        self.max = max
-
-    @staticmethod
-    def parse_mesh_from_urn(urn, token, region="US") -> dict:
-        """
-        Reads mesh data from a specified URN (Uniform Resource Name) and returns a dictionary of mesh packs.
-
-        Parameters:
-        urn (str): The URN from which to read the mesh data.
-        token (str): The token used for authentication.
-        region (str, optional): The region where the data is stored. Defaults to "US".
-
-        Returns:
-        dict: A dictionary where the keys are GUIDs of manifest items and the values are lists of meshes associated with each manifest item.
-
-        The function works by creating a `Derivative` object using the provided URN, token, and region. It then reads the manifest items from the `Derivative` object. For each manifest item, it reads the associated resources and filters them to include only those with a file name that matches the pattern `<number>.pf`. For each of these filtered resources, the function downloads the resource as a stream, reads the content into a buffer, and parses the buffer into a mesh using the `Mesh.parse_mesh` method. The parsed meshes are stored in a list. Finally, the function adds the list of parsed meshes to a dictionary, using the manifest item's GUID as the key. This dictionary is returned as the result of the function.
-        """
-        derivative = Derivative(urn, token, region)
-        manifest_items = derivative.read_svf_manifest_items()
-        mesh_packs = {}
-        for manifest_item in manifest_items:
-            meshes_manifest_item = SVFMesh.parse_mesh_from_manifest_item(derivative, manifest_item)
-            mesh_packs[manifest_item.guid] = meshes_manifest_item
-        return mesh_packs
-
-    @staticmethod
-    def parse_mesh_from_manifest_item(derivative:[Derivative], manifest_item: [ManifestItem]) -> list:
-        svf_resources = derivative.read_svf_resource_item(manifest_item)
-        # filter the resources have file extension .pf and name follow <number>.pf
-        pattern = re.compile(r"^\d+\.pf$")
-        file_packs = [resource for resource in svf_resources if pattern.match(resource.file_name)]
-        meshes_manifest_item = []
-        for file_pack in file_packs:
-            bytes_io = derivative.download_stream_resource(file_pack)
-            buffer = bytes_io.read()
-            meshes = SVFMesh.parse_mesh(buffer)
-            meshes_manifest_item.extend(meshes)
-        return meshes_manifest_item
-    @staticmethod
-    def parse_mesh_from_file(file_path):
-        with open(file_path, "rb") as file:
-            buffer = file.read()
-        return SVFMesh.parse_mesh(buffer)
-
-    @staticmethod
-    def parse_mesh(buffer):
-        mesh_packs = []
-        pfr = PackFileReader(buffer)
-        for i in range(pfr.num_entries()):
-            entry = pfr.seek_entry(i)
-            assert entry is not None
-            assert entry.version >= 1
-            if entry.type == "Autodesk.CloudPlatform.OpenCTM":
-                mesh_packs.append(SVFMesh.parse_mesh_octm(pfr))
-            elif entry.type == "Autodesk.CloudPlatform.Lines":
-                mesh_packs.append(SVFMesh.parse_lines(pfr, entry.version))
-            elif entry.type == "Autodesk.CloudPlatform.Points":
-                mesh_packs.append(SVFMesh.parse_points(pfr, entry.version))
-        return mesh_packs
-
-    @staticmethod
-    def parse_mesh_octm(pfr: [PackFileReader]):
-        fourcc = pfr.get_string(4)
-        assert fourcc == "OCTM"
-
-        version = pfr.get_int32()
-        assert version == 5
-
-        method = pfr.get_string(3)
-        pfr.get_uint8()  # Read the last 0 char of the RAW or MG2 fourCC
-
-        if method == "RAW":
-            return SVFMesh.parse_mesh_raw(pfr)
-        else:
-            print("Unsupported OpenCTM method " + method)
-            return None
-
-    @staticmethod
-    def parse_mesh_raw(pfr: [PackFileReader]):
-        vcount = pfr.get_int32()  # Num of vertices
-        tcount = pfr.get_int32()  # Num of triangles
-        uvcount = pfr.get_int32()  # Num of UV maps
-        attrs = pfr.get_int32()  # Number of custom attributes per vertex
-        flags = pfr.get_int32()  # Additional flags (e.g., whether normals are present)
-        comment = pfr.get_string(pfr.get_int32())
-
-        # Indices
-        name = pfr.get_string(4)
-        assert name == "INDX"
-        indices = [pfr.get_uint32() for _ in range(tcount * 3)]
-
-        # Vertices
-        name = pfr.get_string(4)
-        assert name == "VERT"
-        vertices = []
-        min_values = [float('inf')] * 3
-        max_values = [float('-inf')] * 3
-        for _ in range(vcount):
-            x, y, z = pfr.get_float32(), pfr.get_float32(), pfr.get_float32()
-            min_values = [min(x, min_values[0]), min(y, min_values[1]), min(z, min_values[2])]
-            max_values = [max(x, max_values[0]), max(y, max_values[1]), max(z, max_values[2])]
-            vertices.extend([x, y, z])
-
-        # Normals
-        normals = None
-        if flags & 1 != 0:
-            name = pfr.get_string(4)
-            assert name == "NORM"
-            normals = []
-            for _ in range(vcount):
-                x, y, z = pfr.get_float32(), pfr.get_float32(), pfr.get_float32()
-                # Make sure the normals have unit length
-                dot = x * x + y * y + z * z
-                if dot != 1.0:
-                    length = math.sqrt(dot)
-                    x /= length
-                    y /= length
-                    z /= length
-                normals.extend([x, y, z])
-
-        # Parse zero or more UV maps
-        uvmaps = []
-        for _ in range(uvcount):
-            name = pfr.get_string(4)
-            assert name == "TEXC"
-            uvmap_name = pfr.get_string(pfr.get_int32())
-            uvmap_file = pfr.get_string(pfr.get_int32())
-            uvs = []
-            for _ in range(vcount):
-                u, v = pfr.get_float32(), 1.0 - pfr.get_float32()
-                uvs.extend([u, v])
-            uvmaps.append({"name": uvmap_name, "file": uvmap_file, "uvs": uvs})
-
-        # Parse custom attributes (currently we only support "Color" attrs)
-        colors = None
-        if attrs > 0:
-            name = pfr.get_string(4)
-            assert name == "ATTR"
-            for _ in range(attrs):
-                attr_name = pfr.get_string(pfr.get_int32())
-                if attr_name == "Color":
-                    colors = [pfr.get_float32() for _ in range(vcount * 4)]
-                else:
-                    pfr.seek(pfr.offset + vcount * 4)
-
-        mesh = SVFMesh(vcount, tcount, uvcount, attrs, flags, comment, uvmaps, indices, vertices, normals, colors,
-                       min_values, max_values)
-        if normals is not None:
-            mesh.normals = normals
-        if colors is not None:
-            mesh.colors = colors
-
-        return mesh
-
-    @staticmethod
-    def parse_lines(pfr: [PackFileReader], entry_version) -> SVFLines:
-        assert entry_version >= 2
-
-        vertex_count = pfr.get_uint16()
-        index_count = pfr.get_uint16()
-        bounds_count = pfr.get_uint16()  # Ignoring for now
-        line_width = pfr.get_float32() if entry_version > 2 else 1.0
-        has_colors = pfr.get_uint8() != 0
-        is_line = True
-        l_count = index_count // 2
-        vertices = [pfr.get_float32() for _ in range(vertex_count * 3)]
-        indices = [pfr.get_uint16() for _ in range(index_count)]
-        lines = SVFLines(is_line, vertex_count, l_count, vertices, indices, None, line_width)
-        # Parse colors
-        if has_colors:
-            lines.colors = [pfr.get_float32() for _ in range(vertex_count * 3)]
-
-        # TODO: Parse polyline bounds
-
-        return lines
-
-    @staticmethod
-    def parse_points(self, pfr: [PackFileReader], entry_version) -> SVFPoints:
-        assert entry_version >= 2
-        vertex_count = pfr.get_uint16()
-        index_count = pfr.get_uint16()
-        point_size = pfr.get_float32()
-        has_colors = pfr.get_uint8() != 0
-        vertices = [pfr.get_float32() for _ in range(vertex_count * 3)]
-        points = SVFPoints(True, vertex_count, vertices, None, point_size)
-        # Parse colors
-        if has_colors:
-            points.colors = [pfr.get_float32() for _ in range(vertex_count * 3)]
-        return points
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+from .SVFUVMap import SVFUVMap
+from .PackFileReader import PackFileReader
+import math
+from .SVFLines import SVFLines
+from .SVFPoints import SVFPoints
+from .Derivative import Derivative
+import re
+from .ManifestItem import ManifestItem
+
+
+class SVFMesh:
+    def __init__(self, v_count=None, t_count=None, uv_count=None, attrs=None, flags=None, comment=None,
+                 uv_maps: [SVFUVMap] = None,
+                 indices=None, vertices=None, normals=None, colors=None, min=None, max=None):
+        self.v_count = v_count
+        self.t_count = t_count
+        self.uv_count = uv_count
+        self.attrs = attrs
+        self.flags = flags
+        self.comment = comment
+        self.uv_maps = uv_maps
+        self.indices = indices
+        self.vertices = vertices
+        self.normals = normals
+        self.colors = colors
+        self.min = min
+        self.max = max
+
+    @staticmethod
+    def parse_mesh_from_urn(urn, token, region="US") -> dict:
+        """
+        Reads mesh data from a specified URN (Uniform Resource Name) and returns a dictionary of mesh packs.
+
+        Parameters:
+        urn (str): The URN from which to read the mesh data.
+        token (str): The token used for authentication.
+        region (str, optional): The region where the data is stored. Defaults to "US".
+
+        Returns:
+        dict: A dictionary where the keys are GUIDs of manifest items and the values are lists of meshes associated with each manifest item.
+
+        The function works by creating a `Derivative` object using the provided URN, token, and region. It then reads the manifest items from the `Derivative` object. For each manifest item, it reads the associated resources and filters them to include only those with a file name that matches the pattern `<number>.pf`. For each of these filtered resources, the function downloads the resource as a stream, reads the content into a buffer, and parses the buffer into a mesh using the `Mesh.parse_mesh` method. The parsed meshes are stored in a list. Finally, the function adds the list of parsed meshes to a dictionary, using the manifest item's GUID as the key. This dictionary is returned as the result of the function.
+        """
+        derivative = Derivative(urn, token, region)
+        manifest_items = derivative.read_svf_manifest_items()
+        mesh_packs = {}
+        for manifest_item in manifest_items:
+            meshes_manifest_item = SVFMesh.parse_mesh_from_manifest_item(derivative, manifest_item)
+            mesh_packs[manifest_item.guid] = meshes_manifest_item
+        return mesh_packs
+
+    @staticmethod
+    def parse_mesh_from_manifest_item(derivative:[Derivative], manifest_item: [ManifestItem]) -> list:
+        svf_resources = derivative.read_svf_resource_item(manifest_item)
+        # filter the resources have file extension .pf and name follow <number>.pf
+        pattern = re.compile(r"^\d+\.pf$")
+        file_packs = [resource for resource in svf_resources if pattern.match(resource.file_name)]
+        meshes_manifest_item = []
+        for file_pack in file_packs:
+            bytes_io = derivative.download_stream_resource(file_pack)
+            buffer = bytes_io.read()
+            meshes = SVFMesh.parse_mesh(buffer)
+            meshes_manifest_item.extend(meshes)
+        return meshes_manifest_item
+    @staticmethod
+    def parse_mesh_from_file(file_path):
+        with open(file_path, "rb") as file:
+            buffer = file.read()
+        return SVFMesh.parse_mesh(buffer)
+
+    @staticmethod
+    def parse_mesh(buffer):
+        mesh_packs = []
+        pfr = PackFileReader(buffer)
+        for i in range(pfr.num_entries()):
+            entry = pfr.seek_entry(i)
+            assert entry is not None
+            assert entry.version >= 1
+            if entry.type == "Autodesk.CloudPlatform.OpenCTM":
+                mesh_packs.append(SVFMesh.parse_mesh_octm(pfr))
+            elif entry.type == "Autodesk.CloudPlatform.Lines":
+                mesh_packs.append(SVFMesh.parse_lines(pfr, entry.version))
+            elif entry.type == "Autodesk.CloudPlatform.Points":
+                mesh_packs.append(SVFMesh.parse_points(pfr, entry.version))
+        return mesh_packs
+
+    @staticmethod
+    def parse_mesh_octm(pfr: [PackFileReader]):
+        fourcc = pfr.get_string(4)
+        assert fourcc == "OCTM"
+
+        version = pfr.get_int32()
+        assert version == 5
+
+        method = pfr.get_string(3)
+        pfr.get_uint8()  # Read the last 0 char of the RAW or MG2 fourCC
+
+        if method == "RAW":
+            return SVFMesh.parse_mesh_raw(pfr)
+        else:
+            print("Unsupported OpenCTM method " + method)
+            return None
+
+    @staticmethod
+    def parse_mesh_raw(pfr: [PackFileReader]):
+        vcount = pfr.get_int32()  # Num of vertices
+        tcount = pfr.get_int32()  # Num of triangles
+        uvcount = pfr.get_int32()  # Num of UV maps
+        attrs = pfr.get_int32()  # Number of custom attributes per vertex
+        flags = pfr.get_int32()  # Additional flags (e.g., whether normals are present)
+        comment = pfr.get_string(pfr.get_int32())
+
+        # Indices
+        name = pfr.get_string(4)
+        assert name == "INDX"
+        indices = [pfr.get_uint32() for _ in range(tcount * 3)]
+
+        # Vertices
+        name = pfr.get_string(4)
+        assert name == "VERT"
+        vertices = []
+        min_values = [float('inf')] * 3
+        max_values = [float('-inf')] * 3
+        for _ in range(vcount):
+            x, y, z = pfr.get_float32(), pfr.get_float32(), pfr.get_float32()
+            min_values = [min(x, min_values[0]), min(y, min_values[1]), min(z, min_values[2])]
+            max_values = [max(x, max_values[0]), max(y, max_values[1]), max(z, max_values[2])]
+            vertices.extend([x, y, z])
+
+        # Normals
+        normals = None
+        if flags & 1 != 0:
+            name = pfr.get_string(4)
+            assert name == "NORM"
+            normals = []
+            for _ in range(vcount):
+                x, y, z = pfr.get_float32(), pfr.get_float32(), pfr.get_float32()
+                # Make sure the normals have unit length
+                dot = x * x + y * y + z * z
+                if dot != 1.0:
+                    length = math.sqrt(dot)
+                    x /= length
+                    y /= length
+                    z /= length
+                normals.extend([x, y, z])
+
+        # Parse zero or more UV maps
+        uvmaps = []
+        for _ in range(uvcount):
+            name = pfr.get_string(4)
+            assert name == "TEXC"
+            uvmap_name = pfr.get_string(pfr.get_int32())
+            uvmap_file = pfr.get_string(pfr.get_int32())
+            uvs = []
+            for _ in range(vcount):
+                u, v = pfr.get_float32(), 1.0 - pfr.get_float32()
+                uvs.extend([u, v])
+            uvmaps.append({"name": uvmap_name, "file": uvmap_file, "uvs": uvs})
+
+        # Parse custom attributes (currently we only support "Color" attrs)
+        colors = None
+        if attrs > 0:
+            name = pfr.get_string(4)
+            assert name == "ATTR"
+            for _ in range(attrs):
+                attr_name = pfr.get_string(pfr.get_int32())
+                if attr_name == "Color":
+                    colors = [pfr.get_float32() for _ in range(vcount * 4)]
+                else:
+                    pfr.seek(pfr.offset + vcount * 4)
+
+        mesh = SVFMesh(vcount, tcount, uvcount, attrs, flags, comment, uvmaps, indices, vertices, normals, colors,
+                       min_values, max_values)
+        if normals is not None:
+            mesh.normals = normals
+        if colors is not None:
+            mesh.colors = colors
+
+        return mesh
+
+    @staticmethod
+    def parse_lines(pfr: [PackFileReader], entry_version) -> SVFLines:
+        assert entry_version >= 2
+
+        vertex_count = pfr.get_uint16()
+        index_count = pfr.get_uint16()
+        bounds_count = pfr.get_uint16()  # Ignoring for now
+        line_width = pfr.get_float32() if entry_version > 2 else 1.0
+        has_colors = pfr.get_uint8() != 0
+        is_line = True
+        l_count = index_count // 2
+        vertices = [pfr.get_float32() for _ in range(vertex_count * 3)]
+        indices = [pfr.get_uint16() for _ in range(index_count)]
+        lines = SVFLines(is_line, vertex_count, l_count, vertices, indices, None, line_width)
+        # Parse colors
+        if has_colors:
+            lines.colors = [pfr.get_float32() for _ in range(vertex_count * 3)]
+
+        # TODO: Parse polyline bounds
+
+        return lines
+
+    @staticmethod
+    def parse_points(self, pfr: [PackFileReader], entry_version) -> SVFPoints:
+        assert entry_version >= 2
+        vertex_count = pfr.get_uint16()
+        index_count = pfr.get_uint16()
+        point_size = pfr.get_float32()
+        has_colors = pfr.get_uint8() != 0
+        vertices = [pfr.get_float32() for _ in range(vertex_count * 3)]
+        points = SVFPoints(True, vertex_count, vertices, None, point_size)
+        # Parse colors
+        if has_colors:
+            points.colors = [pfr.get_float32() for _ in range(vertex_count * 3)]
+        return points
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFMetadata.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFMetadata.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from .Derivative import Derivative
-from .ManifestItem import ManifestItem
-
-
-class SVFMetadata:
-    def __init__(self, version, metadata):
-        self.version = version
-        self.metadata = metadata
-
-    @staticmethod
-    def parse_metadata_from_urn(urn, token, region="US") -> dict:
-        meta_datas = {}
-        derivative = Derivative(urn, token, region)
-        manifest_items = derivative.read_svf_manifest_items()
-        for manifest_item in manifest_items:
-            meta_data = SVFMetadata.parse_metadata_from_derivative(derivative, manifest_item)
-            meta_datas[manifest_item.guid] = meta_data
-        return meta_datas
-
-    @staticmethod
-    def parse_metadata_from_derivative(derivative: [Derivative], manifest_item: [ManifestItem]) -> str:
-        metadata = derivative.read_svf_metadata(manifest_item.urn)
-        return metadata
+from .Derivative import Derivative
+from .ManifestItem import ManifestItem
+
+
+class SVFMetadata:
+    def __init__(self, version, metadata):
+        self.version = version
+        self.metadata = metadata
+
+    @staticmethod
+    def parse_metadata_from_urn(urn, token, region="US") -> dict:
+        meta_datas = {}
+        derivative = Derivative(urn, token, region)
+        manifest_items = derivative.read_svf_manifest_items()
+        for manifest_item in manifest_items:
+            meta_data = SVFMetadata.parse_metadata_from_derivative(derivative, manifest_item)
+            meta_datas[manifest_item.guid] = meta_data
+        return meta_datas
+
+    @staticmethod
+    def parse_metadata_from_derivative(derivative: [Derivative], manifest_item: [ManifestItem]) -> str:
+        metadata = derivative.read_svf_metadata(manifest_item.urn)
+        return metadata
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFPoints.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFPoints.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-class SVFPoints:
-    def __init__(self, is_points=None, v_vount=None, vertices=None, colors=None, point_size=None):
-        self.is_points = is_points
-        self.v_count = v_vount
-        self.vertices = vertices
-        self.colors = colors
-        self.point_size = point_size
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+class SVFPoints:
+    def __init__(self, is_points=None, v_vount=None, vertices=None, colors=None, point_size=None):
+        self.is_points = is_points
+        self.v_count = v_vount
+        self.vertices = vertices
+        self.colors = colors
+        self.point_size = point_size
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFReader.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFReader.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-from os.path import join
-import os
-from .Derivative import Derivative
-from .Fragments import Fragments
-from .SVFGeometries import SVFGeometries
-from .ManifestItem import ManifestItem
-from .Resource import Resource
-from .PropReader import PropReader
-from .SVFContent import SVFContent
-from .SVFMesh import SVFMesh
-from .Materials import Materials
-from .SVFMaterials import SVFMaterials
-from .SVFImage import SVFImage
-from .SVFMetadata import SVFMetadata
-
-
-class SVFReader:
-    def __init__(self, urn, token, region="US"):
-        self.urn = urn
-        self.token = token
-        self.region = region
-        self.derivative = Derivative(self.urn, self.token, self.region)
-
-    def read_contents(self, manifest_item: [ManifestItem] = None) -> list[SVFContent]:
-        contents = []
-        if manifest_item:
-            content = self._read_contents_manifest(manifest_item)
-            contents.append(content)
-        else:
-            manifest_items = self.read_svf_manifest_items()
-            for manifest_item in manifest_items:
-                content = self._read_contents_manifest(manifest_item)
-                contents.append(content)
-        return contents
-
-    def _read_contents_manifest(self, manifest_item: [ManifestItem] = None) -> SVFContent:
-        content = SVFContent()
-        content.fragments = self.read_fragments(manifest_item).items().__iter__().__next__()[1]
-        content.geometries = self.read_geometries(manifest_item).items().__iter__().__next__()[1]
-        content.properties = self.read_properties()
-        content.meshpacks = self.read_meshes(manifest_item).items().__iter__().__next__()[1]
-        content.materials = self.read_materials(manifest_item).items().__iter__().__next__()[1]
-        content.images = self.read_images(manifest_item).items().__iter__().__next__()[1]
-        content.metadata = self.read_meta_data(manifest_item).items().__iter__().__next__()[1]
-        return content
-
-    def read_sources(self) -> dict[str, Resource]:
-        resources = self.derivative.read_svf_resource()
-        return resources
-
-    def read_svf_manifest_items(self):
-        items = self.derivative.read_svf_manifest_items()
-        return items
-
-    def read_fragments(self, manifest_item: [ManifestItem] = None) -> dict:
-        fragments = {}
-        if manifest_item:
-            resources = self.derivative.read_svf_resource_item(manifest_item)
-            for resource in resources:
-                if resource.local_path.endswith("FragmentList.pack"):
-                    bytes_io = self.derivative.download_stream_resource(resource)
-                    buffer = bytes_io.read()
-                    frags = Fragments.parse_fragments(buffer)
-                    fragments[manifest_item.guid] = frags
-        else:
-            fragments = Fragments.parse_fragments_from_urn(self.urn, self.token, self.region)
-        return fragments
-
-    def read_geometries(self, manifest_item: [ManifestItem] = None) -> dict:
-        geometries = {}
-        if manifest_item:
-            geos = SVFGeometries.parse_geos_from_manifest_item(self.derivative, manifest_item)
-            geometries[manifest_item.guid] = geos
-        else:
-            geometries = SVFGeometries.parse_geometries_from_urn(self.urn, self.token, self.region)
-        return geometries
-
-    def read_meshes(self, manifest_item: [ManifestItem] = None) -> dict:
-        meshes = {}
-        if manifest_item:
-            mesh = SVFMesh.parse_mesh_from_manifest_item(self.derivative, manifest_item)
-            meshes[manifest_item.guid] = mesh
-        else:
-            meshes = SVFMesh.parse_mesh_from_urn(self.urn, self.token, self.region)
-        return meshes
-
-    def read_materials(self, manifest_item: [ManifestItem] = None) -> dict[str, list[Materials]]:
-        materials = {}
-        if manifest_item:
-            mats = SVFMaterials.parse_materials_from_manifest_item(self.derivative, manifest_item)
-            materials[manifest_item.guid] = mats
-        else:
-            materials = SVFMaterials.parse_materials_from_urn(self.urn, self.token, self.region)
-        return materials
-
-    def read_images(self, manifest_item: [ManifestItem] = None) -> dict[str, list[SVFImage]]:
-        images = {}
-        if manifest_item:
-            imgs = SVFImage.parse_images_from_derivative(self.derivative, manifest_item)
-            images[manifest_item.guid] = imgs
-        else:
-            images = SVFImage.parse_images_from_urn(self.urn, self.token, self.region)
-        return images
-
-    def read_meta_data(self, manifest_item: [ManifestItem] = None) -> dict:
-        meta_datas = {}
-        if manifest_item:
-            meta_data = SVFMetadata.parse_metadata_from_derivative(self.derivative, manifest_item)
-            meta_datas[manifest_item.guid] = meta_data
-        else:
-            meta_datas = SVFMetadata.parse_metadata_from_urn(self.urn, self.token, self.region)
-        return meta_datas
-
-    def read_properties(self) -> PropReader:
-        return PropReader(self.urn, self.token, self.region)
-
-    def download(self, output_dir, manifest_item: [ManifestItem] = None):
-        if manifest_item:
-            resources = self.derivative.read_svf_resource_item(manifest_item)
-            for resource in resources:
-                localpath = resource.local_path
-                combined_path = join(output_dir, localpath)
-                if not os.path.exists(os.path.dirname(combined_path)):
-                    os.makedirs(os.path.dirname(combined_path))
-                self.derivative.download_resource(resource, combined_path)
-        else:
-            resources = self.read_sources()
-            for _, items in resources.items():
-                for source in items:
-                    localpath = source.local_path
-                    combined_path = join(output_dir, localpath)
-                    if not os.path.exists(os.path.dirname(combined_path)):
-                        os.makedirs(os.path.dirname(combined_path))
-                    self.derivative.download_resource(source, combined_path)
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+from os.path import join
+import os
+from .Derivative import Derivative
+from .Fragments import Fragments
+from .SVFGeometries import SVFGeometries
+from .ManifestItem import ManifestItem
+from .Resource import Resource
+from .PropReader import PropReader
+from .SVFContent import SVFContent
+from .SVFMesh import SVFMesh
+from .Materials import Materials
+from .SVFMaterials import SVFMaterials
+from .SVFImage import SVFImage
+from .SVFMetadata import SVFMetadata
+
+
+class SVFReader:
+    def __init__(self, urn, token, region="US"):
+        self.urn = urn
+        self.token = token
+        self.region = region
+        self.derivative = Derivative(self.urn, self.token, self.region)
+
+    def read_contents(self, manifest_item: [ManifestItem] = None) -> list[SVFContent]:
+        contents = []
+        if manifest_item:
+            content = self._read_contents_manifest(manifest_item)
+            contents.append(content)
+        else:
+            manifest_items = self.read_svf_manifest_items()
+            for manifest_item in manifest_items:
+                content = self._read_contents_manifest(manifest_item)
+                contents.append(content)
+        return contents
+
+    def _read_contents_manifest(self, manifest_item: [ManifestItem] = None) -> SVFContent:
+        content = SVFContent()
+        content.fragments = self.read_fragments(manifest_item).items().__iter__().__next__()[1]
+        content.geometries = self.read_geometries(manifest_item).items().__iter__().__next__()[1]
+        content.properties = self.read_properties()
+        content.meshpacks = self.read_meshes(manifest_item).items().__iter__().__next__()[1]
+        content.materials = self.read_materials(manifest_item).items().__iter__().__next__()[1]
+        content.images = self.read_images(manifest_item).items().__iter__().__next__()[1]
+        content.metadata = self.read_meta_data(manifest_item).items().__iter__().__next__()[1]
+        return content
+
+    def read_sources(self) -> dict[str, Resource]:
+        resources = self.derivative.read_svf_resource()
+        return resources
+
+    def read_svf_manifest_items(self):
+        items = self.derivative.read_svf_manifest_items()
+        return items
+
+    def read_fragments(self, manifest_item: [ManifestItem] = None) -> dict:
+        fragments = {}
+        if manifest_item:
+            resources = self.derivative.read_svf_resource_item(manifest_item)
+            for resource in resources:
+                if resource.local_path.endswith("FragmentList.pack"):
+                    bytes_io = self.derivative.download_stream_resource(resource)
+                    buffer = bytes_io.read()
+                    frags = Fragments.parse_fragments(buffer)
+                    fragments[manifest_item.guid] = frags
+        else:
+            fragments = Fragments.parse_fragments_from_urn(self.urn, self.token, self.region)
+        return fragments
+
+    def read_geometries(self, manifest_item: [ManifestItem] = None) -> dict:
+        geometries = {}
+        if manifest_item:
+            geos = SVFGeometries.parse_geos_from_manifest_item(self.derivative, manifest_item)
+            geometries[manifest_item.guid] = geos
+        else:
+            geometries = SVFGeometries.parse_geometries_from_urn(self.urn, self.token, self.region)
+        return geometries
+
+    def read_meshes(self, manifest_item: [ManifestItem] = None) -> dict:
+        meshes = {}
+        if manifest_item:
+            mesh = SVFMesh.parse_mesh_from_manifest_item(self.derivative, manifest_item)
+            meshes[manifest_item.guid] = mesh
+        else:
+            meshes = SVFMesh.parse_mesh_from_urn(self.urn, self.token, self.region)
+        return meshes
+
+    def read_materials(self, manifest_item: [ManifestItem] = None) -> dict[str, list[Materials]]:
+        materials = {}
+        if manifest_item:
+            mats = SVFMaterials.parse_materials_from_manifest_item(self.derivative, manifest_item)
+            materials[manifest_item.guid] = mats
+        else:
+            materials = SVFMaterials.parse_materials_from_urn(self.urn, self.token, self.region)
+        return materials
+
+    def read_images(self, manifest_item: [ManifestItem] = None) -> dict[str, list[SVFImage]]:
+        images = {}
+        if manifest_item:
+            imgs = SVFImage.parse_images_from_derivative(self.derivative, manifest_item)
+            images[manifest_item.guid] = imgs
+        else:
+            images = SVFImage.parse_images_from_urn(self.urn, self.token, self.region)
+        return images
+
+    def read_meta_data(self, manifest_item: [ManifestItem] = None) -> dict:
+        meta_datas = {}
+        if manifest_item:
+            meta_data = SVFMetadata.parse_metadata_from_derivative(self.derivative, manifest_item)
+            meta_datas[manifest_item.guid] = meta_data
+        else:
+            meta_datas = SVFMetadata.parse_metadata_from_urn(self.urn, self.token, self.region)
+        return meta_datas
+
+    def read_properties(self) -> PropReader:
+        return PropReader(self.urn, self.token, self.region)
+
+    def download(self, output_dir, manifest_item: [ManifestItem] = None):
+        if manifest_item:
+            resources = self.derivative.read_svf_resource_item(manifest_item)
+            for resource in resources:
+                localpath = resource.local_path
+                combined_path = join(output_dir, localpath)
+                if not os.path.exists(os.path.dirname(combined_path)):
+                    os.makedirs(os.path.dirname(combined_path))
+                self.derivative.download_resource(resource, combined_path)
+        else:
+            resources = self.read_sources()
+            for _, items in resources.items():
+                for source in items:
+                    localpath = source.local_path
+                    combined_path = join(output_dir, localpath)
+                    if not os.path.exists(os.path.dirname(combined_path)):
+                        os.makedirs(os.path.dirname(combined_path))
+                    self.derivative.download_resource(source, combined_path)
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFTransform.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFMaterialMap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-class SVFTransform:
-    def __init__(self, t=None, q=None, s=None, matrix=None):
-        self.t = t
-        self.q = q
-        self.s = s
-        self.matrix = matrix
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+class SVFMaterialMap:
+    def __init__(self, uri=None, scale=None):
+        self.uri = uri
+        self.scale = scale
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit/SVFUVMap.py` & `aps-toolkit-0.5.4/src/aps_toolkit/SVFUVMap.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""
-Copyright (C) 2024  chuongmep.com
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-class SVFUVMap:
-    def __init__(self, name=None, file=None, uvs=None):
-        self.name = name
-        self.file = file
+"""
+Copyright (C) 2024  chuongmep.com
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+class SVFUVMap:
+    def __init__(self, name=None, file=None, uvs=None):
+        self.name = name
+        self.file = file
         self.uvs = uvs
```

### Comparing `aps-toolkit-0.5.3/src/aps_toolkit.egg-info/SOURCES.txt` & `aps-toolkit-0.5.4/src/aps_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.3/src/test/context.py` & `aps-toolkit-0.5.4/src/test/context.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-﻿import os
-import sys
-
-# Assuming the src folder is at the same level as the test folder
-src_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
-print(src_dir)
-sys.path.append(src_dir)
-# Now you can import modules from the project folder
-from aps_toolkit import PropReader
-from aps_toolkit import PropDbReaderRevit
-from aps_toolkit import PropDbReaderCad
-from aps_toolkit import PropDbReaderNavis
-from aps_toolkit import DbReader
-from aps_toolkit import Auth
-from aps_toolkit import Token
-from aps_toolkit import BIM360
-from aps_toolkit import Fragments
-from aps_toolkit import SVFGeometries
-from aps_toolkit import SVFMesh
-from aps_toolkit import Derivative
-from aps_toolkit import SVFReader
-from aps_toolkit import SVFMaterials
-from aps_toolkit import SVFImage
-from aps_toolkit import SVFMetadata
-from aps_toolkit import Bucket
-
-APS_CLIENT_ID = os.environ["APS_CLIENT_ID"]
-APS_CLIENT_SECRET = os.environ["APS_CLIENT_SECRET"]
+﻿import os
+import sys
+
+# Assuming the src folder is at the same level as the test folder
+src_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
+print(src_dir)
+sys.path.append(src_dir)
+# Now you can import modules from the project folder
+from aps_toolkit import PropReader
+from aps_toolkit import PropDbReaderRevit
+from aps_toolkit import PropDbReaderCad
+from aps_toolkit import PropDbReaderNavis
+from aps_toolkit import DbReader
+from aps_toolkit import Auth
+from aps_toolkit import Token
+from aps_toolkit import BIM360
+from aps_toolkit import Fragments
+from aps_toolkit import SVFGeometries
+from aps_toolkit import SVFMesh
+from aps_toolkit import Derivative
+from aps_toolkit import SVFReader
+from aps_toolkit import SVFMaterials
+from aps_toolkit import SVFImage
+from aps_toolkit import SVFMetadata
+from aps_toolkit import Bucket
+
+APS_CLIENT_ID = os.environ["APS_CLIENT_ID"]
+APS_CLIENT_SECRET = os.environ["APS_CLIENT_SECRET"]
```

### Comparing `aps-toolkit-0.5.3/src/test/test_bim360.py` & `aps-toolkit-0.5.4/src/test/test_bim360.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-﻿from unittest import TestCase
-import os
-
-from .context import BIM360
-
-from .context import Auth
-
-
-class TestBIM360(TestCase):
-    def setUp(self):
-        self.token = Auth().auth2leg()
-        self.bim360 = BIM360(self.token)
-        self.hub_id = "b.1715cf2b-cc12-46fd-9279-11bbc47e72f6"
-        self.project_id = "b.1f7aa830-c6ef-48be-8a2d-bd554779e74b"
-        self.folder_id = "urn:adsk.wipprod:fs.folder:co.5ufH-U8yRjaZ-USJxxN_Mw"
-        self.item_id = "urn:adsk.wipprod:dm.lineage:DjXtlXoJQyS6D1R-gRhI8A"
-
-    def test_get_hubs(self):
-        hubs = self.bim360.get_hubs()
-        self.assertNotEquals(hubs, 0)
-
-    def test_get_projects(self):
-        hubs = self.bim360.get_hubs()
-        projects = self.bim360.get_projects(hubs['data'][0]['id'])
-        self.assertNotEquals(projects, 0)
-
-    def test_get_top_folders(self):
-        hubs = self.bim360.get_hubs()
-        projects = self.bim360.get_projects(hubs['data'][0]['id'])
-        top_folders = self.bim360.get_top_folders(hubs['data'][0]['id'], projects['data'][0]['id'])
-        self.assertNotEquals(top_folders, 0)
-
-    def test_get_folder_contents(self):
-        hubs = self.bim360.get_hubs()
-        projects = self.bim360.get_projects(hubs['data'][0]['id'])
-        top_folders = self.bim360.get_top_folders(hubs['data'][0]['id'], projects['data'][0]['id'])
-        folder_contents = self.bim360.get_folder_contents(projects['data'][0]['id'], top_folders['data'][0]['id'])
-        self.assertNotEquals(folder_contents, 0)
-
-    def test_get_top_folder_project_files(self):
-        project_files = self.bim360.get_top_folder_project_files(self.hub_id, self.project_id)
-        self.assertNotEquals(project_files, 0)
-
-    def test_get_item_info(self):
-        item_info = self.bim360.get_item_info(self.project_id, self.item_id)
-        self.assertNotEquals(item_info, 0)
-
-    def test_get_item_versions(self):
-        items = self.bim360.batch_report_items(self.project_id, self.folder_id)
-        self.assertNotEquals(len(items), 0)
-
-    def test_batch_report_item_versions(self):
-        df = self.bim360.batch_report_item_versions(self.project_id, self.item_id)
-        self.assertNotEquals(df.empty, True)
-
-    def test_get_urn_item_version(self):
-        urn = self.bim360.get_urn_item_version(self.project_id, self.item_id, 2)
-        self.assertNotEquals(urn, "")
-
-    def test_batch_report_projects(self):
-        df = self.bim360.batch_report_projects(self.hub_id)
-        self.assertNotEquals(df.empty, True)
-
-    def test_get_item__display_name(self):
-        item_name = self.bim360.get_item_display_name(self.project_id, self.item_id)
-        self.assertNotEquals(item_name, "")
+﻿from unittest import TestCase
+import os
+
+from .context import BIM360
+
+from .context import Auth
+
+
+class TestBIM360(TestCase):
+    def setUp(self):
+        self.token = Auth().auth2leg()
+        self.bim360 = BIM360(self.token)
+        self.hub_id = "b.1715cf2b-cc12-46fd-9279-11bbc47e72f6"
+        self.project_id = "b.1f7aa830-c6ef-48be-8a2d-bd554779e74b"
+        self.folder_id = "urn:adsk.wipprod:fs.folder:co.5ufH-U8yRjaZ-USJxxN_Mw"
+        self.item_id = "urn:adsk.wipprod:dm.lineage:DjXtlXoJQyS6D1R-gRhI8A"
+
+    def test_get_hubs(self):
+        hubs = self.bim360.get_hubs()
+        self.assertNotEquals(hubs, 0)
+
+    def test_get_projects(self):
+        hubs = self.bim360.get_hubs()
+        projects = self.bim360.get_projects(hubs['data'][0]['id'])
+        self.assertNotEquals(projects, 0)
+
+    def test_get_top_folders(self):
+        hubs = self.bim360.get_hubs()
+        projects = self.bim360.get_projects(hubs['data'][0]['id'])
+        top_folders = self.bim360.get_top_folders(hubs['data'][0]['id'], projects['data'][0]['id'])
+        self.assertNotEquals(top_folders, 0)
+
+    def test_get_folder_contents(self):
+        hubs = self.bim360.get_hubs()
+        projects = self.bim360.get_projects(hubs['data'][0]['id'])
+        top_folders = self.bim360.get_top_folders(hubs['data'][0]['id'], projects['data'][0]['id'])
+        folder_contents = self.bim360.get_folder_contents(projects['data'][0]['id'], top_folders['data'][0]['id'])
+        self.assertNotEquals(folder_contents, 0)
+
+    def test_get_top_folder_project_files(self):
+        project_files = self.bim360.get_top_folder_project_files(self.hub_id, self.project_id)
+        self.assertNotEquals(project_files, 0)
+
+    def test_get_item_info(self):
+        item_info = self.bim360.get_item_info(self.project_id, self.item_id)
+        self.assertNotEquals(item_info, 0)
+
+    def test_get_item_versions(self):
+        items = self.bim360.batch_report_items(self.project_id, self.folder_id)
+        self.assertNotEquals(len(items), 0)
+
+    def test_batch_report_item_versions(self):
+        df = self.bim360.batch_report_item_versions(self.project_id, self.item_id)
+        self.assertNotEquals(df.empty, True)
+
+    def test_get_urn_item_version(self):
+        urn = self.bim360.get_urn_item_version(self.project_id, self.item_id, 2)
+        self.assertNotEquals(urn, "")
+
+    def test_batch_report_projects(self):
+        df = self.bim360.batch_report_projects(self.hub_id)
+        self.assertNotEquals(df.empty, True)
+
+    def test_get_item__display_name(self):
+        item_name = self.bim360.get_item_display_name(self.project_id, self.item_id)
+        self.assertNotEquals(item_name, "")
```

### Comparing `aps-toolkit-0.5.3/src/test/test_bucket.py` & `aps-toolkit-0.5.4/src/test/test_bucket.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import unittest
-
-from aps_toolkit.Bucket import PublicKey
-from .context import Bucket
-from .context import Auth
-
-
-class TestBucket(unittest.TestCase):
-    def setUp(self):
-        self.token = Auth().auth2leg()
-
-    def test_get_all_buckets(self):
-        bucket = Bucket(self.token)
-        buckets = bucket.get_all_buckets()
-        self.assertNotEqual(len(buckets), 0)
-
-    def test_create_bucket(self):
-        bucket = Bucket(self.token)
-        bucket_name = "hello_world_23232"
-        policy_key = PublicKey.transient
-        response = bucket.create_bucket(bucket_name, policy_key)
-        self.assertEqual(response["bucketKey"], bucket_name)
-
-    def test_delete_bucket(self):
-        bucket = Bucket(self.token)
-        bucket_name = "hello_world_23232"
-        result = bucket.delete_bucket(bucket_name)
-        self.assertEqual(result, b'')
-
-    def test_get_objects(self):
-        bucket = Bucket(self.token)
-        bucket_name = "chuong_bucket"
-        objects = bucket.get_objects(bucket_name)
-        self.assertNotEqual(len(objects), 0)
-
-    def test_upload_object(self):
-        bucket = Bucket(self.token)
-        bucket_name = "chuong_bucket"
-        file_path = "/Users/chuongmep/Downloads/008950495344-Sep_2023.pdf"
-        object_name = "chuong.pdf"
-        response = bucket.upload_object(bucket_name, file_path, object_name)
-        self.assertEqual(response["bucketKey"], bucket_name)
-
-    def test_delete_object(self):
-        bucket = Bucket(self.token)
-        bucket_name = "chuong_bucket"
-        object_name = "chuong.pdf"
-        result = bucket.delete_object(bucket_name, object_name)
-        self.assertEqual(result, b'')
-
-    def test_download_object(self):
-        bucket = Bucket(self.token)
-        bucket_name = "chuong_bucket"
-        object_name = "chuong.pdf"
-        file_path = "/Users/chuongmep/Downloads/hello.pdf"
-        bucket.download_object(bucket_name, object_name, file_path)
-        self.assertTrue(True)
+import unittest
+
+from aps_toolkit.Bucket import PublicKey
+from .context import Bucket
+from .context import Auth
+
+
+class TestBucket(unittest.TestCase):
+    def setUp(self):
+        self.token = Auth().auth2leg()
+
+    def test_get_all_buckets(self):
+        bucket = Bucket(self.token)
+        buckets = bucket.get_all_buckets()
+        self.assertNotEqual(len(buckets), 0)
+
+    def test_create_bucket(self):
+        bucket = Bucket(self.token)
+        bucket_name = "hello_world_23232"
+        policy_key = PublicKey.transient
+        response = bucket.create_bucket(bucket_name, policy_key)
+        self.assertEqual(response["bucketKey"], bucket_name)
+
+    def test_delete_bucket(self):
+        bucket = Bucket(self.token)
+        bucket_name = "hello_world_23232"
+        result = bucket.delete_bucket(bucket_name)
+        self.assertEqual(result, b'')
+
+    def test_get_objects(self):
+        bucket = Bucket(self.token)
+        bucket_name = "chuong_bucket"
+        objects = bucket.get_objects(bucket_name)
+        self.assertNotEqual(len(objects), 0)
+
+    def test_upload_object(self):
+        bucket = Bucket(self.token)
+        bucket_name = "chuong_bucket"
+        file_path = "/Users/chuongmep/Downloads/008950495344-Sep_2023.pdf"
+        object_name = "chuong.pdf"
+        response = bucket.upload_object(bucket_name, file_path, object_name)
+        self.assertEqual(response["bucketKey"], bucket_name)
+
+    def test_delete_object(self):
+        bucket = Bucket(self.token)
+        bucket_name = "chuong_bucket"
+        object_name = "chuong.pdf"
+        result = bucket.delete_object(bucket_name, object_name)
+        self.assertEqual(result, b'')
+
+    def test_download_object(self):
+        bucket = Bucket(self.token)
+        bucket_name = "chuong_bucket"
+        object_name = "chuong.pdf"
+        file_path = "/Users/chuongmep/Downloads/hello.pdf"
+        bucket.download_object(bucket_name, object_name, file_path)
+        self.assertTrue(True)
```

### Comparing `aps-toolkit-0.5.3/src/test/test_db_reader.py` & `aps-toolkit-0.5.4/src/test/test_db_reader.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-﻿from unittest import TestCase
-import os
-from .context import Auth
-from .context import DbReader
-
-
-class TestDbReader(TestCase):
-    def setUp(self):
-        self.client_id = os.environ['APS_CLIENT_ID']
-        self.client_secret = os.environ['APS_CLIENT_SECRET']
-        self.auth = Auth(self.client_id, self.client_secret)
-        self.token = self.auth.auth2leg()
-        self.urn = "dXJuOmFkc2sub2JqZWN0czpvcy5vYmplY3Q6Y2h1b25nX2J1Y2tldC9NeUhvdXNlLm53Yw"
-
-    def test_reader(self):
-        db_reader = DbReader(self.urn, self.token)
-        self.assertNotEquals(db_reader, "")
-
-    def test_execute_query(self):
-        db_reader = DbReader(self.urn, self.token)
-        print(db_reader.db_path)
-        query = "SELECT * FROM _objects_id"
-        df = db_reader.execute_query(query)
-        self.assertNotEquals(df.empty, True)
+﻿from unittest import TestCase
+import os
+from .context import Auth
+from .context import DbReader
+
+
+class TestDbReader(TestCase):
+    def setUp(self):
+        self.client_id = os.environ['APS_CLIENT_ID']
+        self.client_secret = os.environ['APS_CLIENT_SECRET']
+        self.auth = Auth(self.client_id, self.client_secret)
+        self.token = self.auth.auth2leg()
+        self.urn = "dXJuOmFkc2sub2JqZWN0czpvcy5vYmplY3Q6Y2h1b25nX2J1Y2tldC9NeUhvdXNlLm53Yw"
+
+    def test_reader(self):
+        db_reader = DbReader(self.urn, self.token)
+        self.assertNotEquals(db_reader, "")
+
+    def test_execute_query(self):
+        db_reader = DbReader(self.urn, self.token)
+        print(db_reader.db_path)
+        query = "SELECT * FROM _objects_id"
+        df = db_reader.execute_query(query)
+        self.assertNotEquals(df.empty, True)
```

### Comparing `aps-toolkit-0.5.3/src/test/test_derivative.py` & `aps-toolkit-0.5.4/src/test/test_derivative.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from unittest import TestCase
-
-from .context import Derivative
-from .context import Auth
-
-
-class TestDerivative(TestCase):
-    def setUp(self):
-        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLk9kOHR4RGJLU1NlbFRvVmcxb2MxVkE_dmVyc2lvbj0yNA"
-        self.token = Auth().auth2leg()
-
-    def test_translate_job(self):
-        self.urn = "dXJuOmFkc2sub2JqZWN0czpvcy5vYmplY3Q6Y2h1b25nX2J1Y2tldC9NeUhvdXNlLm53Yw"
-        derivative = Derivative(self.urn, self.token)
-        response = derivative.translate_job("Project Completion.ifc")
-        self.assertNotEquals(response, "")
-
-    def test_check_job_status(self):
-        self.urn = "dXJuOmFkc2sub2JqZWN0czpvcy5vYmplY3Q6Y2h1b25nX2J1Y2tldC9NeUhvdXNlLm53Yw"
-        derivative = Derivative(self.urn, self.token)
-        response = derivative.check_job_status()
-        self.assertNotEquals(response, "")
-
-    def test_read_svf_manifest_items(self):
-        derivative = Derivative(self.urn, self.token)
-        manifest_items = derivative.read_svf_manifest_items()
-        self.assertNotEquals(len(manifest_items), 0)
-
-    def test_read_svf_resource(self):
-        derivative = Derivative(self.urn, self.token)
-        svf_resources = derivative.read_svf_resource()
-        self.assertNotEquals(len(svf_resources), 0)
-
-    def test_read_svf_resource_item(self):
-        derivative = Derivative(self.urn, self.token)
-        manifest_items = derivative.read_svf_manifest_items()
-        svf_resources = derivative.read_svf_resource_item(manifest_items[0])
-        self.assertNotEquals(len(svf_resources), 0)
-
-    def test_read_metadata(self):
-        derivative = Derivative(self.urn, self.token)
-        manifest_items = derivative.read_svf_manifest_items()
-        for manifest_item in manifest_items:
-            metadata = derivative.read_svf_metadata(manifest_item.urn)
-            self.assertNotEquals(metadata, "")
+from unittest import TestCase
+
+from .context import Derivative
+from .context import Auth
+
+
+class TestDerivative(TestCase):
+    def setUp(self):
+        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLk9kOHR4RGJLU1NlbFRvVmcxb2MxVkE_dmVyc2lvbj0yNA"
+        self.token = Auth().auth2leg()
+
+    def test_translate_job(self):
+        self.urn = "dXJuOmFkc2sub2JqZWN0czpvcy5vYmplY3Q6Y2h1b25nX2J1Y2tldC9NeUhvdXNlLm53Yw"
+        derivative = Derivative(self.urn, self.token)
+        response = derivative.translate_job("Project Completion.ifc")
+        self.assertNotEquals(response, "")
+
+    def test_check_job_status(self):
+        self.urn = "dXJuOmFkc2sub2JqZWN0czpvcy5vYmplY3Q6Y2h1b25nX2J1Y2tldC9NeUhvdXNlLm53Yw"
+        derivative = Derivative(self.urn, self.token)
+        response = derivative.check_job_status()
+        self.assertNotEquals(response, "")
+
+    def test_read_svf_manifest_items(self):
+        derivative = Derivative(self.urn, self.token)
+        manifest_items = derivative.read_svf_manifest_items()
+        self.assertNotEquals(len(manifest_items), 0)
+
+    def test_read_svf_resource(self):
+        derivative = Derivative(self.urn, self.token)
+        svf_resources = derivative.read_svf_resource()
+        self.assertNotEquals(len(svf_resources), 0)
+
+    def test_read_svf_resource_item(self):
+        derivative = Derivative(self.urn, self.token)
+        manifest_items = derivative.read_svf_manifest_items()
+        svf_resources = derivative.read_svf_resource_item(manifest_items[0])
+        self.assertNotEquals(len(svf_resources), 0)
+
+    def test_read_metadata(self):
+        derivative = Derivative(self.urn, self.token)
+        manifest_items = derivative.read_svf_manifest_items()
+        for manifest_item in manifest_items:
+            metadata = derivative.read_svf_metadata(manifest_item.urn)
+            self.assertNotEquals(metadata, "")
```

### Comparing `aps-toolkit-0.5.3/src/test/test_fragment.py` & `aps-toolkit-0.5.4/src/test/test_fragment.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from unittest import TestCase
-from .context import Fragments
-from .context import Auth
-
-
-class TestFragment(TestCase):
-    def setUp(self):
-        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLk9kOHR4RGJLU1NlbFRvVmcxb2MxVkE_dmVyc2lvbj0yNA"
-        self.token = Auth().auth2leg()
-        self.file_path = (r".\output\svfs\Resource\3D View\08f99ae5-b8be-4f8d-881b-128675723c10\Project "
-                            r"Completion\FragmentList.pack")
-
-    def test_parse_fragments(self):
-        with open(self.file_path, 'rb') as f:
-            buffer = f.read()
-        fragment = Fragments.parse_fragments(buffer)
-        self.assertNotEquals(len(fragment), 0)
-
-    def test_parse_fragments_from_file(self):
-        fragment = Fragments.parse_fragments_from_file(self.file_path)
-        self.assertNotEquals(len(fragment), 0)
-
-    def test_parse_fragments_from_urn(self):
-        fragment = Fragments.parse_fragments_from_urn(self.urn, self.token)
-        self.assertNotEquals(len(fragment), 0)
+from unittest import TestCase
+from .context import Fragments
+from .context import Auth
+
+
+class TestFragment(TestCase):
+    def setUp(self):
+        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLk9kOHR4RGJLU1NlbFRvVmcxb2MxVkE_dmVyc2lvbj0yNA"
+        self.token = Auth().auth2leg()
+        self.file_path = (r".\output\svfs\Resource\3D View\08f99ae5-b8be-4f8d-881b-128675723c10\Project "
+                            r"Completion\FragmentList.pack")
+
+    def test_parse_fragments(self):
+        with open(self.file_path, 'rb') as f:
+            buffer = f.read()
+        fragment = Fragments.parse_fragments(buffer)
+        self.assertNotEquals(len(fragment), 0)
+
+    def test_parse_fragments_from_file(self):
+        fragment = Fragments.parse_fragments_from_file(self.file_path)
+        self.assertNotEquals(len(fragment), 0)
+
+    def test_parse_fragments_from_urn(self):
+        fragment = Fragments.parse_fragments_from_urn(self.urn, self.token)
+        self.assertNotEquals(len(fragment), 0)
```

### Comparing `aps-toolkit-0.5.3/src/test/test_image.py` & `aps-toolkit-0.5.4/src/test/test_image.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from unittest import TestCase
-from .context import SVFImage
-from .context import Auth
-from .context import Derivative
-
-
-class TestImage(TestCase):
-    def setUp(self):
-        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLk9kOHR4RGJLU1NlbFRvVmcxb2MxVkE_dmVyc2lvbj0yNA"
-        self.token = Auth().auth2leg()
-
-    def test_parse_images_from_urn(self):
-        images = SVFImage.parse_images_from_urn(self.urn, self.token)
-        self.assertNotEquals(len(images), 0)
-
-    def test_parse_images_from_derivative(self):
-        derivative = Derivative(self.urn, self.token)
-        manifest_items = derivative.read_svf_manifest_items()
-        images = SVFImage.parse_images_from_derivative(derivative, manifest_items[0])
-        self.assertNotEquals(len(images), 0)
+from unittest import TestCase
+from .context import SVFImage
+from .context import Auth
+from .context import Derivative
+
+
+class TestImage(TestCase):
+    def setUp(self):
+        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLk9kOHR4RGJLU1NlbFRvVmcxb2MxVkE_dmVyc2lvbj0yNA"
+        self.token = Auth().auth2leg()
+
+    def test_parse_images_from_urn(self):
+        images = SVFImage.parse_images_from_urn(self.urn, self.token)
+        self.assertNotEquals(len(images), 0)
+
+    def test_parse_images_from_derivative(self):
+        derivative = Derivative(self.urn, self.token)
+        manifest_items = derivative.read_svf_manifest_items()
+        images = SVFImage.parse_images_from_derivative(derivative, manifest_items[0])
+        self.assertNotEquals(len(images), 0)
```

### Comparing `aps-toolkit-0.5.3/src/test/test_material.py` & `aps-toolkit-0.5.4/src/test/test_material.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from unittest import TestCase
-
-from .context import SVFReader
-from .context import Auth
-from .context import SVFMaterials
-import os
-from .context import Derivative
-
-
-class TestMaterial(TestCase):
-    def setUp(self):
-        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLk9kOHR4RGJLU1NlbFRvVmcxb2MxVkE_dmVyc2lvbj0yNA"
-        self.token = Auth().auth2leg()
-        self.file_path = (r"./output/svfs/Resource/3D View/08f99ae5-b8be-4f8d-881b-128675723c10/Project "
-                          r"Completion/Materials.json.gz")
-
-    def test_parse_materials_from_urn(self):
-        materials = SVFMaterials.parse_materials_from_urn(self.urn, self.token)
-        self.assertNotEquals(len(materials), 0)
-
-    def test_parse_materials_from_manifest_item(self):
-        derivative = Derivative(self.urn, self.token)
-        manifest_items = derivative.read_svf_manifest_items()
-        materials = SVFMaterials.parse_materials_from_manifest_item(derivative, manifest_items[0])
-        self.assertNotEquals(len(materials), 0)
-
-    def test_read_from_file(self):
-        self.assertTrue(os.path.exists(self.file_path))
-        materials = SVFMaterials.parse_materials_from_file(self.file_path)
-        self.assertNotEquals(len(materials), 0)
+from unittest import TestCase
+
+from .context import SVFReader
+from .context import Auth
+from .context import SVFMaterials
+import os
+from .context import Derivative
+
+
+class TestMaterial(TestCase):
+    def setUp(self):
+        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLk9kOHR4RGJLU1NlbFRvVmcxb2MxVkE_dmVyc2lvbj0yNA"
+        self.token = Auth().auth2leg()
+        self.file_path = (r"./output/svfs/Resource/3D View/08f99ae5-b8be-4f8d-881b-128675723c10/Project "
+                          r"Completion/Materials.json.gz")
+
+    def test_parse_materials_from_urn(self):
+        materials = SVFMaterials.parse_materials_from_urn(self.urn, self.token)
+        self.assertNotEquals(len(materials), 0)
+
+    def test_parse_materials_from_manifest_item(self):
+        derivative = Derivative(self.urn, self.token)
+        manifest_items = derivative.read_svf_manifest_items()
+        materials = SVFMaterials.parse_materials_from_manifest_item(derivative, manifest_items[0])
+        self.assertNotEquals(len(materials), 0)
+
+    def test_read_from_file(self):
+        self.assertTrue(os.path.exists(self.file_path))
+        materials = SVFMaterials.parse_materials_from_file(self.file_path)
+        self.assertNotEquals(len(materials), 0)
```

### Comparing `aps-toolkit-0.5.3/src/test/test_mesh.py` & `aps-toolkit-0.5.4/src/test/test_mesh.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from unittest import TestCase
-from .context import SVFMesh
-from .context import Auth
-
-
-class TestMesh(TestCase):
-    def setUp(self):
-        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLk9kOHR4RGJLU1NlbFRvVmcxb2MxVkE_dmVyc2lvbj0yNA"
-        self.token = Auth().auth2leg()
-        self.file_path = r".\output\svfs\Resource\3D View\08f99ae5-b8be-4f8d-881b-128675723c10\Project Completion\0.pf"
-
-    def test_parse_mesh_from_file(self):
-        mesh = SVFMesh.parse_mesh_from_file(self.file_path)
-        self.assertNotEquals(len(mesh), 0)
-
-    def test_parse_mesh_from_urn(self):
-        mesh = SVFMesh.parse_mesh_from_urn(self.urn, self.token)
-        self.assertNotEquals(len(mesh), 0)
+from unittest import TestCase
+from .context import SVFMesh
+from .context import Auth
+
+
+class TestMesh(TestCase):
+    def setUp(self):
+        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLk9kOHR4RGJLU1NlbFRvVmcxb2MxVkE_dmVyc2lvbj0yNA"
+        self.token = Auth().auth2leg()
+        self.file_path = r".\output\svfs\Resource\3D View\08f99ae5-b8be-4f8d-881b-128675723c10\Project Completion\0.pf"
+
+    def test_parse_mesh_from_file(self):
+        mesh = SVFMesh.parse_mesh_from_file(self.file_path)
+        self.assertNotEquals(len(mesh), 0)
+
+    def test_parse_mesh_from_urn(self):
+        mesh = SVFMesh.parse_mesh_from_urn(self.urn, self.token)
+        self.assertNotEquals(len(mesh), 0)
```

### Comparing `aps-toolkit-0.5.3/src/test/test_prop_reader_cad.py` & `aps-toolkit-0.5.4/src/test/test_prop_reader_cad.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-﻿from unittest import TestCase
-import os
-from .context import PropDbReaderCad
-from .context import Auth
-
-
-class TestPropDbReader(TestCase):
-    def setUp(self):
-        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLm5KaEpjQkQ1UXd1bjlIV1ktNWViQmc_dmVyc2lvbj0x"
-        self.token = Auth().auth2leg()
-        self.prop_reader = PropDbReaderCad(self.urn, self.token)
-
-    def test_get_document_info(self):
-        document_info = self.prop_reader.get_document_info()
-        self.assertIsNotNone(document_info)
-
-    def test_get_all_layers(self):
-        layers = self.prop_reader.get_all_layers()
-        self.assertNotEquals(len(layers), 0)
-
-    def test_get_all_categories(self):
-        categories = self.prop_reader.get_all_categories()
-        self.assertNotEquals(len(categories), 0)
-
-    def test_get_all_data(self):
-        data = self.prop_reader.get_all_data()
-        self.assertIsNotNone(data)
-
-    def test_get_data_by_category(self):
-        df = self.prop_reader.get_data_by_category("Lines")
-        self.assertNotEquals(df.empty, True)
-
-    def test_get_data_by_categories(self):
-        df = self.prop_reader.get_data_by_categories(["Lines", "Circles"])
-        self.assertNotEquals(df.empty, True)
-
-    def test_get_data_by_categories_and_params(self):
-        df = self.prop_reader.get_data_by_categories_and_params(["Lines", "Circles"], ["Name", "Layer", "Color", "type"])
-        self.assertNotEquals(df.empty, True)
+﻿from unittest import TestCase
+import os
+from .context import PropDbReaderCad
+from .context import Auth
+
+
+class TestPropDbReader(TestCase):
+    def setUp(self):
+        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLm5KaEpjQkQ1UXd1bjlIV1ktNWViQmc_dmVyc2lvbj0x"
+        self.token = Auth().auth2leg()
+        self.prop_reader = PropDbReaderCad(self.urn, self.token)
+
+    def test_get_document_info(self):
+        document_info = self.prop_reader.get_document_info()
+        self.assertIsNotNone(document_info)
+
+    def test_get_all_layers(self):
+        layers = self.prop_reader.get_all_layers()
+        self.assertNotEquals(len(layers), 0)
+
+    def test_get_all_categories(self):
+        categories = self.prop_reader.get_all_categories()
+        self.assertNotEquals(len(categories), 0)
+
+    def test_get_all_data(self):
+        data = self.prop_reader.get_all_data()
+        self.assertIsNotNone(data)
+
+    def test_get_data_by_category(self):
+        df = self.prop_reader.get_data_by_category("Lines")
+        self.assertNotEquals(df.empty, True)
+
+    def test_get_data_by_categories(self):
+        df = self.prop_reader.get_data_by_categories(["Lines", "Circles"])
+        self.assertNotEquals(df.empty, True)
+
+    def test_get_data_by_categories_and_params(self):
+        df = self.prop_reader.get_data_by_categories_and_params(["Lines", "Circles"], ["Name", "Layer", "Color", "type"])
+        self.assertNotEquals(df.empty, True)
```

### Comparing `aps-toolkit-0.5.3/src/test/test_prop_reader_navis.py` & `aps-toolkit-0.5.4/src/test/test_prop_reader_navis.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from unittest import TestCase
-from .context import PropDbReaderNavis
-from .context import Auth
-
-
-class TestPropDbReaderNavis(TestCase):
-    def setUp(self):
-        self.token = Auth().auth2leg()
-        self.urn = "dXJuOmFkc2sub2JqZWN0czpvcy5vYmplY3Q6Y2h1b25nX2J1Y2tldC9NeUhvdXNlLm53Yw"
-        self.prop_reader = PropDbReaderNavis(self.urn, self.token)
-
-    def test_get_document_info(self):
-        document_info = self.prop_reader.get_document_info()
-        self.assertIsNotNone(document_info)
-
-    def test_get_all_categories(self):
-        categories = self.prop_reader.get_all_categories()
-        self.assertIsNotNone(categories)
-
-    def test_get_data_by_property(self):
-        data = self.prop_reader.get_data_by_category("Item")
-        self.assertIsNotNone(data)
+from unittest import TestCase
+from .context import PropDbReaderNavis
+from .context import Auth
+
+
+class TestPropDbReaderNavis(TestCase):
+    def setUp(self):
+        self.token = Auth().auth2leg()
+        self.urn = "dXJuOmFkc2sub2JqZWN0czpvcy5vYmplY3Q6Y2h1b25nX2J1Y2tldC9NeUhvdXNlLm53Yw"
+        self.prop_reader = PropDbReaderNavis(self.urn, self.token)
+
+    def test_get_document_info(self):
+        document_info = self.prop_reader.get_document_info()
+        self.assertIsNotNone(document_info)
+
+    def test_get_all_categories(self):
+        categories = self.prop_reader.get_all_categories()
+        self.assertIsNotNone(categories)
+
+    def test_get_data_by_property(self):
+        data = self.prop_reader.get_data_by_category("Item")
+        self.assertIsNotNone(data)
```

### Comparing `aps-toolkit-0.5.3/src/test/test_prop_reader_revit.py` & `aps-toolkit-0.5.4/src/test/test_prop_reader_revit.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-﻿from unittest import TestCase
-import os
-from .context import PropDbReaderRevit
-from .context import Auth
-
-
-class TestPropDbReaderRevit(TestCase):
-    def setUp(self):
-        self.token = Auth().auth2leg()
-        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLk9kOHR4RGJLU1NlbFRvVmcxb2MxVkE_dmVyc2lvbj0yNA"
-        self.prop_reader = PropDbReaderRevit(self.urn, self.token)
-
-    def test_get_document_info(self):
-        document_info = self.prop_reader.get_document_info()
-        self.assertIsNotNone(document_info)
-
-    def test_get_documentId(self):
-        documentId = self.prop_reader.get_document_id()
-        self.assertIsNotNone(documentId)
-
-    def test_get_levels(self):
-        levels = self.prop_reader.get_levels()
-        self.assertNotEquals(len(levels), 0)
-
-    def test_get_grids(self):
-        grids = self.prop_reader.get_grids()
-        self.assertNotEquals(len(grids), 0)
-
-    def test_get_phases(self):
-        phases = self.prop_reader.get_phases()
-        self.assertNotEquals(len(phases), 0)
-
-    def test_get_all_categories(self):
-        categories = self.prop_reader.get_all_categories()
-        print(categories)
-        self.assertNotEquals(categories, 0)
-
-    def test_get_all_families(self):
-        families = self.prop_reader.get_all_families()
-        self.assertNotEquals(families, 0)
-
-    def test_get_all_families_types(self):
-        families_types = self.prop_reader.get_all_families_types()
-        self.assertNotEquals(families_types, 0)
-
-    def test_get_all_data(self):
-        data = self.prop_reader.get_all_data()
-        self.assertIsNotNone(data)
-
-    def test_get_data_by_category(self):
-        df = self.prop_reader.get_data_by_category("Windows", True)
-        # check if dataframe have rows = 1
-        df_rows = df.shape[0]
-        self.assertNotEquals(df_rows, 0)
-
-    def test_get_data_by_categories(self):
-        df = self.prop_reader.get_data_by_categories(["Doors", "Windows"])
-        self.assertNotEquals(df.empty, True)
-
-    def test_get_data_by_family(self):
-        family_name = "Seating-LAMMHULTS-PENNE-Chair"
-        df = self.prop_reader.get_data_by_family(family_name)
-        self.assertNotEquals(df.empty, True)
-
-    def test_get_data_by_family_type(self):
-        family_type = "Plastic-Seat"
-        df = self.prop_reader.get_data_by_family_type(family_type)
-        self.assertNotEquals(df.empty, True)
-
-    def test_get_data_by_categories_and_params(self):
-        df = self.prop_reader.get_data_by_categories_and_params(["Doors", "Windows"],
-                                                                ["name", "Category", "ElementId", "Width", "Height",
-                                                                 "IfcGUID"], True)
-        self.assertNotEquals(df.empty, True)
-
-    def test_get_data_by_external_id(self):
-        external_id = "6d22740f-4d3f-4cc6-a442-8c98ddd54f1f-0004923b"
-        df = self.prop_reader.get_data_by_external_id(external_id, True)
-        self.assertNotEquals(df.empty, True)
-
-    def test_get_data_by_element_id(self):
-        element_id = 289790
-        parameters = self.prop_reader.get_data_by_element_id(element_id)
-        self.assertIsNotNone(parameters)
-        self.assertNotEquals(len(parameters), 0)
-
-    def test_get_all_parametes(self):
-        parameters = self.prop_reader.get_all_parameters()
-        self.assertNotEquals(parameters, 0)
+﻿from unittest import TestCase
+import os
+from .context import PropDbReaderRevit
+from .context import Auth
+
+
+class TestPropDbReaderRevit(TestCase):
+    def setUp(self):
+        self.token = Auth().auth2leg()
+        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLk9kOHR4RGJLU1NlbFRvVmcxb2MxVkE_dmVyc2lvbj0yNA"
+        self.prop_reader = PropDbReaderRevit(self.urn, self.token)
+
+    def test_get_document_info(self):
+        document_info = self.prop_reader.get_document_info()
+        self.assertIsNotNone(document_info)
+
+    def test_get_documentId(self):
+        documentId = self.prop_reader.get_document_id()
+        self.assertIsNotNone(documentId)
+
+    def test_get_levels(self):
+        levels = self.prop_reader.get_levels()
+        self.assertNotEquals(len(levels), 0)
+
+    def test_get_grids(self):
+        grids = self.prop_reader.get_grids()
+        self.assertNotEquals(len(grids), 0)
+
+    def test_get_phases(self):
+        phases = self.prop_reader.get_phases()
+        self.assertNotEquals(len(phases), 0)
+
+    def test_get_all_categories(self):
+        categories = self.prop_reader.get_all_categories()
+        print(categories)
+        self.assertNotEquals(categories, 0)
+
+    def test_get_all_families(self):
+        families = self.prop_reader.get_all_families()
+        self.assertNotEquals(families, 0)
+
+    def test_get_all_families_types(self):
+        families_types = self.prop_reader.get_all_families_types()
+        self.assertNotEquals(families_types, 0)
+
+    def test_get_all_data(self):
+        data = self.prop_reader.get_all_data()
+        self.assertIsNotNone(data)
+
+    def test_get_data_by_category(self):
+        df = self.prop_reader.get_data_by_category("Windows", True)
+        # check if dataframe have rows = 1
+        df_rows = df.shape[0]
+        self.assertNotEquals(df_rows, 0)
+
+    def test_get_data_by_categories(self):
+        df = self.prop_reader.get_data_by_categories(["Doors", "Windows"])
+        self.assertNotEquals(df.empty, True)
+
+    def test_get_data_by_family(self):
+        family_name = "Seating-LAMMHULTS-PENNE-Chair"
+        df = self.prop_reader.get_data_by_family(family_name)
+        self.assertNotEquals(df.empty, True)
+
+    def test_get_data_by_family_type(self):
+        family_type = "Plastic-Seat"
+        df = self.prop_reader.get_data_by_family_type(family_type)
+        self.assertNotEquals(df.empty, True)
+
+    def test_get_data_by_categories_and_params(self):
+        df = self.prop_reader.get_data_by_categories_and_params(["Doors", "Windows"],
+                                                                ["name", "Category", "ElementId", "Width", "Height",
+                                                                 "IfcGUID"], True)
+        self.assertNotEquals(df.empty, True)
+
+    def test_get_data_by_external_id(self):
+        external_id = "6d22740f-4d3f-4cc6-a442-8c98ddd54f1f-0004923b"
+        df = self.prop_reader.get_data_by_external_id(external_id, True)
+        self.assertNotEquals(df.empty, True)
+
+    def test_get_data_by_element_id(self):
+        element_id = 289790
+        parameters = self.prop_reader.get_data_by_element_id(element_id)
+        self.assertIsNotNone(parameters)
+        self.assertNotEquals(len(parameters), 0)
+
+    def test_get_all_parametes(self):
+        parameters = self.prop_reader.get_all_parameters()
+        self.assertNotEquals(parameters, 0)
```

### Comparing `aps-toolkit-0.5.3/src/test/test_svf_reader.py` & `aps-toolkit-0.5.4/src/test/test_svf_reader.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-from unittest import TestCase
-
-from .context import SVFReader
-from .context import Auth
-import os
-
-
-class TestSVFReader(TestCase):
-    def setUp(self):
-        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLm5KaEpjQkQ1UXd1bjlIV1ktNWViQmc_dmVyc2lvbj0x"
-        self.token = Auth().auth2leg()
-        self.reader = SVFReader(self.urn, self.token)
-
-    def test_read_contents(self):
-        contents = self.reader.read_contents()
-        self.assertTrue(len(contents) > 0)
-
-    def test_read_contents_manifest(self):
-        manifest_items = self.reader.read_svf_manifest_items()
-        contents = self.reader.read_contents(manifest_items[0])
-        self.assertTrue(len(contents) > 0)
-
-    def test_read_svf(self):
-        resources = self.reader.read_sources()
-        self.assertTrue(len(resources) > 0)
-
-    def test_read_fragment(self):
-        fragments = self.reader.read_fragments()
-        self.assertTrue(len(fragments) > 0)
-
-    def test_read_fragment_item(self):
-        manifest_items = self.reader.read_svf_manifest_items()
-        fragments = self.reader.read_fragments(manifest_items[0])
-        self.assertTrue(len(fragments) > 0)
-
-    def test_read_geometries(self):
-        geometries = self.reader.read_geometries()
-        self.assertTrue(len(geometries) > 0)
-
-    def test_read_geometries_item(self):
-        manifest_items = self.reader.read_svf_manifest_items()
-        geometries = self.reader.read_geometries(manifest_items[0])
-        self.assertTrue(len(geometries) > 0)
-
-    def test_read_meshes(self):
-        meshes = self.reader.read_meshes()
-        self.assertTrue(len(meshes) > 0)
-
-    def test_read_meshes_item(self):
-        manifest_items = self.reader.read_svf_manifest_items()
-        meshes = self.reader.read_meshes(manifest_items[0])
-        self.assertTrue(len(meshes) > 0)
-
-    def test_read_properties(self):
-        prop_reader = self.reader.read_properties()
-        self.assertTrue(len(prop_reader.attrs) > 0)
-        self.assertTrue(len(prop_reader.vals) > 0)
-
-    def test_read_materials(self):
-        materials = self.reader.read_materials()
-        self.assertTrue(len(materials) > 0)
-
-    def test_read_images(self):
-        images = self.reader.read_images()
-        self.assertTrue(len(images) > 0)
-
-    def test_read_meta_data(self):
-        meta_data = self.reader.read_meta_data()
-        self.assertTrue(len(meta_data) > 0)
-
-    def test_read_materials_item(self):
-        manifest_items = self.reader.read_svf_manifest_items()
-        materials = self.reader.read_materials(manifest_items[0])
-        self.assertTrue(len(materials) > 0)
-
-    def test_download_svf(self):
-        folder = r"./output/svfs/"
-        self.reader.download(folder)
-        self.assertTrue(len(os.listdir(folder)) > 0)
-
-    def test_read_svf_manifest_items(self):
-        manifest_items = self.reader.read_svf_manifest_items()
-        self.assertTrue(len(manifest_items) > 0)
+from unittest import TestCase
+
+from .context import SVFReader
+from .context import Auth
+import os
+
+
+class TestSVFReader(TestCase):
+    def setUp(self):
+        self.urn = "dXJuOmFkc2sud2lwcHJvZDpmcy5maWxlOnZmLm5KaEpjQkQ1UXd1bjlIV1ktNWViQmc_dmVyc2lvbj0x"
+        self.token = Auth().auth2leg()
+        self.reader = SVFReader(self.urn, self.token)
+
+    def test_read_contents(self):
+        contents = self.reader.read_contents()
+        self.assertTrue(len(contents) > 0)
+
+    def test_read_contents_manifest(self):
+        manifest_items = self.reader.read_svf_manifest_items()
+        contents = self.reader.read_contents(manifest_items[0])
+        self.assertTrue(len(contents) > 0)
+
+    def test_read_svf(self):
+        resources = self.reader.read_sources()
+        self.assertTrue(len(resources) > 0)
+
+    def test_read_fragment(self):
+        fragments = self.reader.read_fragments()
+        self.assertTrue(len(fragments) > 0)
+
+    def test_read_fragment_item(self):
+        manifest_items = self.reader.read_svf_manifest_items()
+        fragments = self.reader.read_fragments(manifest_items[0])
+        self.assertTrue(len(fragments) > 0)
+
+    def test_read_geometries(self):
+        geometries = self.reader.read_geometries()
+        self.assertTrue(len(geometries) > 0)
+
+    def test_read_geometries_item(self):
+        manifest_items = self.reader.read_svf_manifest_items()
+        geometries = self.reader.read_geometries(manifest_items[0])
+        self.assertTrue(len(geometries) > 0)
+
+    def test_read_meshes(self):
+        meshes = self.reader.read_meshes()
+        self.assertTrue(len(meshes) > 0)
+
+    def test_read_meshes_item(self):
+        manifest_items = self.reader.read_svf_manifest_items()
+        meshes = self.reader.read_meshes(manifest_items[0])
+        self.assertTrue(len(meshes) > 0)
+
+    def test_read_properties(self):
+        prop_reader = self.reader.read_properties()
+        self.assertTrue(len(prop_reader.attrs) > 0)
+        self.assertTrue(len(prop_reader.vals) > 0)
+
+    def test_read_materials(self):
+        materials = self.reader.read_materials()
+        self.assertTrue(len(materials) > 0)
+
+    def test_read_images(self):
+        images = self.reader.read_images()
+        self.assertTrue(len(images) > 0)
+
+    def test_read_meta_data(self):
+        meta_data = self.reader.read_meta_data()
+        self.assertTrue(len(meta_data) > 0)
+
+    def test_read_materials_item(self):
+        manifest_items = self.reader.read_svf_manifest_items()
+        materials = self.reader.read_materials(manifest_items[0])
+        self.assertTrue(len(materials) > 0)
+
+    def test_download_svf(self):
+        folder = r"./output/svfs/"
+        self.reader.download(folder)
+        self.assertTrue(len(os.listdir(folder)) > 0)
+
+    def test_read_svf_manifest_items(self):
+        manifest_items = self.reader.read_svf_manifest_items()
+        self.assertTrue(len(manifest_items) > 0)
```

