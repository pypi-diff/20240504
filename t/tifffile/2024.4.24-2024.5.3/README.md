# Comparing `tmp/tifffile-2024.4.24.tar.gz` & `tmp/tifffile-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tifffile-2024.4.24.tar", last modified: Thu Apr 25 03:05:10 2024, max compression
+gzip compressed data, was "tifffile-2024.5.3.tar", last modified: Sat May  4 00:45:36 2024, max compression
```

## Comparing `tifffile-2024.4.24.tar` & `tifffile-2024.5.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.077372 tifffile-2024.4.24/
--rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2024.4.24/ACKNOWLEDGEMENTS.rst
--rw-rw-rw-   0        0        0    38017 2024-04-25 03:05:08.000000 tifffile-2024.4.24/CHANGES.rst
--rw-rw-rw-   0        0        0     1559 2024-04-25 03:05:08.000000 tifffile-2024.4.24/LICENSE
--rw-rw-rw-   0        0        0      569 2023-08-11 02:48:51.000000 tifffile-2024.4.24/MANIFEST.in
--rw-rw-rw-   0        0        0    31811 2024-04-25 03:05:10.077372 tifffile-2024.4.24/PKG-INFO
--rw-rw-rw-   0        0        0    30569 2024-04-25 03:05:08.000000 tifffile-2024.4.24/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.061868 tifffile-2024.4.24/docs/
-drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.061868 tifffile-2024.4.24/docs/_static/
--rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2024.4.24/docs/_static/custom.css
--rw-rw-rw-   0        0        0     1098 2023-12-25 06:05:35.000000 tifffile-2024.4.24/docs/conf.py
--rw-rw-rw-   0        0        0     3644 2023-08-12 18:29:44.000000 tifffile-2024.4.24/docs/make.py
-drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.061868 tifffile-2024.4.24/examples/
--rw-rw-rw-   0        0        0    15113 2024-02-12 18:46:43.000000 tifffile-2024.4.24/examples/earthbigdata.py
--rw-rw-rw-   0        0        0     2542 2024-01-28 18:02:54.000000 tifffile-2024.4.24/examples/issue125.py
--rw-rw-rw-   0        0        0       42 2024-04-25 03:05:10.077372 tifffile-2024.4.24/setup.cfg
--rw-rw-rw-   0        0        0     3936 2023-10-18 16:48:53.000000 tifffile-2024.4.24/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.077372 tifffile-2024.4.24/tests/
--rw-rw-rw-   0        0        0     1603 2023-08-30 07:20:06.000000 tifffile-2024.4.24/tests/conftest.py
--rw-rw-rw-   0        0        0   744389 2024-04-25 03:03:32.000000 tifffile-2024.4.24/tests/test_tifffile.py
-drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.077372 tifffile-2024.4.24/tifffile/
--rw-rw-rw-   0        0        0      110 2024-01-28 01:29:32.000000 tifffile-2024.4.24/tifffile/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2024.4.24/tifffile/__main__.py
--rw-rw-rw-   0        0        0    11865 2024-04-25 00:49:56.000000 tifffile-2024.4.24/tifffile/_imagecodecs.py
--rw-rw-rw-   0        0        0    61794 2023-07-03 00:17:39.000000 tifffile-2024.4.24/tifffile/geodb.py
--rw-rw-rw-   0        0        0      680 2023-07-03 00:17:47.000000 tifffile-2024.4.24/tifffile/lsm2bin.py
--rw-rw-rw-   0        0        0     5904 2024-01-29 17:41:17.000000 tifffile-2024.4.24/tifffile/numcodecs.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 tifffile-2024.4.24/tifffile/py.typed
--rw-rw-rw-   0        0        0     2410 2023-07-03 00:18:03.000000 tifffile-2024.4.24/tifffile/tiff2fsspec.py
--rw-rw-rw-   0        0        0     1437 2023-07-03 00:18:11.000000 tifffile-2024.4.24/tifffile/tiffcomment.py
--rw-rw-rw-   0        0        0   888550 2024-04-25 03:02:37.000000 tifffile-2024.4.24/tifffile/tifffile.py
-drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.077372 tifffile-2024.4.24/tifffile.egg-info/
--rw-rw-rw-   0        0        0    31811 2024-04-25 03:05:09.000000 tifffile-2024.4.24/tifffile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2024-04-25 03:05:10.000000 tifffile-2024.4.24/tifffile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 03:05:09.000000 tifffile-2024.4.24/tifffile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-04-25 03:05:09.000000 tifffile-2024.4.24/tifffile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2024-04-25 03:05:09.000000 tifffile-2024.4.24/tifffile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 03:05:09.000000 tifffile-2024.4.24/tifffile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/
+-rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2024.5.3/ACKNOWLEDGEMENTS.rst
+-rw-rw-rw-   0        0        0    38141 2024-05-04 00:45:34.000000 tifffile-2024.5.3/CHANGES.rst
+-rw-rw-rw-   0        0        0     1559 2024-05-04 00:45:34.000000 tifffile-2024.5.3/LICENSE
+-rw-rw-rw-   0        0        0      569 2023-08-11 02:48:51.000000 tifffile-2024.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    31893 2024-05-04 00:45:36.153592 tifffile-2024.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0    30652 2024-05-04 00:45:34.000000 tifffile-2024.5.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/docs/
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/docs/_static/
+-rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2024.5.3/docs/_static/custom.css
+-rw-rw-rw-   0        0        0     1098 2023-12-25 06:05:35.000000 tifffile-2024.5.3/docs/conf.py
+-rw-rw-rw-   0        0        0     3644 2023-08-12 18:29:44.000000 tifffile-2024.5.3/docs/make.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/examples/
+-rw-rw-rw-   0        0        0    15113 2024-02-12 18:46:43.000000 tifffile-2024.5.3/examples/earthbigdata.py
+-rw-rw-rw-   0        0        0     2542 2024-01-28 18:02:54.000000 tifffile-2024.5.3/examples/issue125.py
+-rw-rw-rw-   0        0        0       42 2024-05-04 00:45:36.153592 tifffile-2024.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     3936 2023-10-18 16:48:53.000000 tifffile-2024.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/tests/
+-rw-rw-rw-   0        0        0     1591 2024-05-04 00:43:50.000000 tifffile-2024.5.3/tests/conftest.py
+-rw-rw-rw-   0        0        0   751633 2024-05-04 00:13:02.000000 tifffile-2024.5.3/tests/test_tifffile.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/tifffile/
+-rw-rw-rw-   0        0        0      110 2024-01-28 01:29:32.000000 tifffile-2024.5.3/tifffile/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2024.5.3/tifffile/__main__.py
+-rw-rw-rw-   0        0        0    11865 2024-04-25 00:49:56.000000 tifffile-2024.5.3/tifffile/_imagecodecs.py
+-rw-rw-rw-   0        0        0    61794 2023-07-03 00:17:39.000000 tifffile-2024.5.3/tifffile/geodb.py
+-rw-rw-rw-   0        0        0      680 2023-07-03 00:17:47.000000 tifffile-2024.5.3/tifffile/lsm2bin.py
+-rw-rw-rw-   0        0        0     5904 2024-01-29 17:41:17.000000 tifffile-2024.5.3/tifffile/numcodecs.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 tifffile-2024.5.3/tifffile/py.typed
+-rw-rw-rw-   0        0        0     2410 2023-07-03 00:18:03.000000 tifffile-2024.5.3/tifffile/tiff2fsspec.py
+-rw-rw-rw-   0        0        0     1437 2023-07-03 00:18:11.000000 tifffile-2024.5.3/tifffile/tiffcomment.py
+-rw-rw-rw-   0        0        0   890009 2024-05-04 00:45:12.000000 tifffile-2024.5.3/tifffile/tifffile.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/tifffile.egg-info/
+-rw-rw-rw-   0        0        0    31893 2024-05-04 00:45:35.000000 tifffile-2024.5.3/tifffile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2024-05-04 00:45:36.000000 tifffile-2024.5.3/tifffile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 00:45:35.000000 tifffile-2024.5.3/tifffile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-05-04 00:45:35.000000 tifffile-2024.5.3/tifffile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2024-05-04 00:45:35.000000 tifffile-2024.5.3/tifffile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 00:45:35.000000 tifffile-2024.5.3/tifffile.egg-info/top_level.txt
```

### Comparing `tifffile-2024.4.24/CHANGES.rst` & `tifffile-2024.5.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 Revisions
 ---------
 
+2024.5.3
+
+- Pass 5080 tests.
+- Fix reading incompletely written LSM.
+- Fix reading Philips DP with extra rows of tiles (#253, breaking).
+
 2024.4.24
 
-- Pass 5077 tests.
 - Fix compatibility issue with numpy 2 (#252).
 
 2024.4.18
 
 - Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
 - Add option not to quote file names in write_fsspec.
 - Allow compress bilevel images with deflate, LZMA, and Zstd.
```

### Comparing `tifffile-2024.4.24/LICENSE` & `tifffile-2024.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/MANIFEST.in` & `tifffile-2024.5.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/PKG-INFO` & `tifffile-2024.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2024.4.24
+Version: 2024.5.3
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
@@ -38,15 +38,15 @@
 
 (1) store NumPy arrays in TIFF (Tagged Image File Format) files, and
 (2) read image and metadata from TIFF-like files used in bioimaging.
 
 Image and metadata can be read from TIFF, BigTIFF, OME-TIFF, DNG, STK, LSM,
 SGI, NIHImage, ImageJ, MMStack, NDTiff, FluoView, ScanImage, SEQ, GEL,
 SVS, SCN, SIS, BIF, ZIF (Zoomable Image File Format), QPTIFF (QPI, PKI), NDPI,
-and GeoTIFF formatted files.
+Philips DP, and GeoTIFF formatted files.
 
 Image data can be read as NumPy arrays or Zarr arrays/groups from strips,
 tiles, pages (IFDs), SubIFDs, higher order series, and pyramidal levels.
 
 Image data can be written to TIFF, BigTIFF, OME-TIFF, and ImageJ hyperstack
 compatible files in multi-page, volumetric, pyramidal, memory-mappable,
 tiled, predicted, or compressed form.
@@ -59,15 +59,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.3
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -111,17 +111,22 @@
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2024.5.3
+
+- Pass 5080 tests.
+- Fix reading incompletely written LSM.
+- Fix reading Philips DP with extra rows of tiles (#253, breaking).
+
 2024.4.24
 
-- Pass 5077 tests.
 - Fix compatibility issue with numpy 2 (#252).
 
 2024.4.18
 
 - Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
 - Add option not to quote file names in write_fsspec.
 - Allow compress bilevel images with deflate, LZMA, and Zstd.
@@ -325,19 +330,18 @@
   structures. Tifffile can read NDPI files > 4 GB.
   JPEG compressed segments with dimensions >65530 or missing restart markers
   cannot be decoded with common JPEG libraries. Tifffile works around this
   limitation by separately decoding the MCUs between restart markers, which
   performs poorly. BitsPerSample, SamplesPerPixel, and
   PhotometricInterpretation tags may contain wrong values, which can be
   corrected using the value of tag 65441.
-- **Philips TIFF** slides store wrong ImageWidth and ImageLength tag values
+- **Philips TIFF** slides store padded ImageWidth and ImageLength tag values
   for tiled pages. The values can be corrected using the DICOM_PIXEL_SPACING
   attributes of the XML formatted description of the first page. Tile offsets
-  and byte counts may be 0 and last rows of tiles may be missing.
-  Tifffile can read Philips slides.
+  and byte counts may be 0. Tifffile can read Philips slides.
 - **Ventana/Roche BIF** slides store tiles and metadata in a BigTIFF container.
   Tiles may overlap and require stitching based on the TileJointInfo elements
   in the XMP tag. Volumetric scans are stored using the ImageDepth extension.
   Tifffile can read BIF and decode individual tiles but does not perform
   stitching.
 - **ScanImage** optionally allows corrupted non-BigTIFF files > 2 GB.
   The values of StripOffsets and StripByteCounts can be recovered using the
@@ -410,25 +414,22 @@
   https://www.loc.gov/preservation/digital/formats/content/tiff_tags.shtml
 - CIPA DC-008-2016: Exchangeable image file format for digital still cameras:
   Exif Version 2.31.
   http://www.cipa.jp/std/documents/e/DC-008-Translation-2016-E.pdf
 - The EER (Electron Event Representation) file format.
   https://github.com/fei-company/EerReaderLib
 - Digital Negative (DNG) Specification. Version 1.5.0.0, June 2012.
-  https://www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/
-  dng_spec_1.5.0.0.pdf
+  https://www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/dng_spec_1.5.0.0.pdf
 - Roche Digital Pathology. BIF image file format for digital pathology.
-  https://diagnostics.roche.com/content/dam/diagnostics/Blueprint/en/pdf/rmd/
-  Roche-Digital-Pathology-BIF-Whitepaper.pdf
+  https://diagnostics.roche.com/content/dam/diagnostics/Blueprint/en/pdf/rmd/Roche-Digital-Pathology-BIF-Whitepaper.pdf
 - Astro-TIFF specification. https://astro-tiff.sourceforge.io/
 - Aperio Technologies, Inc. Digital Slides and Third-Party Data Interchange.
   Aperio_Digital_Slides_and_Third-party_data_interchange.pdf
 - PerkinElmer image format.
-  https://downloads.openmicroscopy.org/images/Vectra-QPTIFF/perkinelmer/
-  PKI_Image%20Format.docx
+  https://downloads.openmicroscopy.org/images/Vectra-QPTIFF/perkinelmer/PKI_Image%20Format.docx
 - NDTiffStorage. https://github.com/micro-manager/NDTiffStorage
 
 Examples
 --------
 
 Write a NumPy array to a single-page RGB TIFF file:
```

### Comparing `tifffile-2024.4.24/README.rst` & `tifffile-2024.5.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 (1) store NumPy arrays in TIFF (Tagged Image File Format) files, and
 (2) read image and metadata from TIFF-like files used in bioimaging.
 
 Image and metadata can be read from TIFF, BigTIFF, OME-TIFF, DNG, STK, LSM,
 SGI, NIHImage, ImageJ, MMStack, NDTiff, FluoView, ScanImage, SEQ, GEL,
 SVS, SCN, SIS, BIF, ZIF (Zoomable Image File Format), QPTIFF (QPI, PKI), NDPI,
-and GeoTIFF formatted files.
+Philips DP, and GeoTIFF formatted files.
 
 Image data can be read as NumPy arrays or Zarr arrays/groups from strips,
 tiles, pages (IFDs), SubIFDs, higher order series, and pyramidal levels.
 
 Image data can be written to TIFF, BigTIFF, OME-TIFF, and ImageJ hyperstack
 compatible files in multi-page, volumetric, pyramidal, memory-mappable,
 tiled, predicted, or compressed form.
@@ -26,15 +26,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.3
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -78,17 +78,22 @@
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2024.5.3
+
+- Pass 5080 tests.
+- Fix reading incompletely written LSM.
+- Fix reading Philips DP with extra rows of tiles (#253, breaking).
+
 2024.4.24
 
-- Pass 5077 tests.
 - Fix compatibility issue with numpy 2 (#252).
 
 2024.4.18
 
 - Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
 - Add option not to quote file names in write_fsspec.
 - Allow compress bilevel images with deflate, LZMA, and Zstd.
@@ -292,19 +297,18 @@
   structures. Tifffile can read NDPI files > 4 GB.
   JPEG compressed segments with dimensions >65530 or missing restart markers
   cannot be decoded with common JPEG libraries. Tifffile works around this
   limitation by separately decoding the MCUs between restart markers, which
   performs poorly. BitsPerSample, SamplesPerPixel, and
   PhotometricInterpretation tags may contain wrong values, which can be
   corrected using the value of tag 65441.
-- **Philips TIFF** slides store wrong ImageWidth and ImageLength tag values
+- **Philips TIFF** slides store padded ImageWidth and ImageLength tag values
   for tiled pages. The values can be corrected using the DICOM_PIXEL_SPACING
   attributes of the XML formatted description of the first page. Tile offsets
-  and byte counts may be 0 and last rows of tiles may be missing.
-  Tifffile can read Philips slides.
+  and byte counts may be 0. Tifffile can read Philips slides.
 - **Ventana/Roche BIF** slides store tiles and metadata in a BigTIFF container.
   Tiles may overlap and require stitching based on the TileJointInfo elements
   in the XMP tag. Volumetric scans are stored using the ImageDepth extension.
   Tifffile can read BIF and decode individual tiles but does not perform
   stitching.
 - **ScanImage** optionally allows corrupted non-BigTIFF files > 2 GB.
   The values of StripOffsets and StripByteCounts can be recovered using the
@@ -377,25 +381,22 @@
   https://www.loc.gov/preservation/digital/formats/content/tiff_tags.shtml
 - CIPA DC-008-2016: Exchangeable image file format for digital still cameras:
   Exif Version 2.31.
   http://www.cipa.jp/std/documents/e/DC-008-Translation-2016-E.pdf
 - The EER (Electron Event Representation) file format.
   https://github.com/fei-company/EerReaderLib
 - Digital Negative (DNG) Specification. Version 1.5.0.0, June 2012.
-  https://www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/
-  dng_spec_1.5.0.0.pdf
+  https://www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/dng_spec_1.5.0.0.pdf
 - Roche Digital Pathology. BIF image file format for digital pathology.
-  https://diagnostics.roche.com/content/dam/diagnostics/Blueprint/en/pdf/rmd/
-  Roche-Digital-Pathology-BIF-Whitepaper.pdf
+  https://diagnostics.roche.com/content/dam/diagnostics/Blueprint/en/pdf/rmd/Roche-Digital-Pathology-BIF-Whitepaper.pdf
 - Astro-TIFF specification. https://astro-tiff.sourceforge.io/
 - Aperio Technologies, Inc. Digital Slides and Third-Party Data Interchange.
   Aperio_Digital_Slides_and_Third-party_data_interchange.pdf
 - PerkinElmer image format.
-  https://downloads.openmicroscopy.org/images/Vectra-QPTIFF/perkinelmer/
-  PKI_Image%20Format.docx
+  https://downloads.openmicroscopy.org/images/Vectra-QPTIFF/perkinelmer/PKI_Image%20Format.docx
 - NDTiffStorage. https://github.com/micro-manager/NDTiffStorage
 
 Examples
 --------
 
 Write a NumPy array to a single-page RGB TIFF file:
```

### Comparing `tifffile-2024.4.24/docs/conf.py` & `tifffile-2024.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/docs/make.py` & `tifffile-2024.5.3/docs/make.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/examples/earthbigdata.py` & `tifffile-2024.5.3/examples/earthbigdata.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/examples/issue125.py` & `tifffile-2024.5.3/examples/issue125.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/setup.py` & `tifffile-2024.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/tests/conftest.py` & `tifffile-2024.5.3/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,18 @@
         0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
     )
 
 if os.environ.get('SKIP_CODECS', None):
     sys.modules['imagecodecs'] = None  # type: ignore
 
 
-def pytest_report_header(config, start_path, startdir):
+def pytest_report_header(config, start_path):
     try:
         from numpy import __version__ as numpy
         from test_tifffile import config
-
         from tifffile import __version__ as tifffile
 
         try:
             from imagecodecs import __version__ as imagecodecs
         except ImportError:
             imagecodecs = 'N/A'
         try:
```

### Comparing `tifffile-2024.4.24/tests/test_tifffile.py` & `tifffile-2024.5.3/tests/test_tifffile.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # mypy: check-untyped-defs=False
 
 """Unittests for the tifffile package.
 
 Public data files can be requested from the author.
 Private data files are not available due to size and copyright restrictions.
 
-:Version: 2024.4.24
+:Version: 2024.5.3
 
 """
 
 import binascii
 import datetime
 import glob
 import json
@@ -2833,83 +2833,14 @@
             compression='zlib',
             **kwargs,
         )
         im = imread(fname, maxworkers=2, buffersize=buffersize)
     assert_array_equal(im, data)
 
 
-@pytest.mark.skipif(
-    SKIP_PRIVATE or SKIP_CODECS or not imagecodecs.JPEG, reason=REASON
-)
-def test_issue_philips_fsspec():
-    """Test write_fsspec with Philips slide missing row of tiles."""
-    # https://github.com/cgohlke/tifffile/issues/249
-    fname = private_file('PhilipsDP/patient_080_node_2.tif')
-    with TiffFile(fname) as tif:
-        assert len(tif.series) == 2
-        assert len(tif.pages) == 11
-        assert tif.is_philips
-        assert tif.philips_metadata.endswith('</DataObject>')
-        page = tif.pages.first
-        assert page.compression == JPEG
-        assert page.photometric == YCBCR
-        assert page.planarconfig == CONTIG
-        assert page.tags['ImageWidth'].value == 155136
-        assert page.tags['ImageLength'].value == 78336
-        assert page.imagewidth == 155136
-        assert page.imagelength == 78336
-        assert page.bitspersample == 8
-        assert page.samplesperpixel == 3
-        assert page.tags['Software'].value == 'Philips DP v1.0'
-        series = tif.series[1]
-        assert series.kind == 'philips'
-        assert series.shape == (801, 1756, 3)
-        assert len(series.levels) == 1
-        assert not series.is_pyramidal
-        series = tif.series[0]
-        assert series.kind == 'philips'
-        assert series.shape == (78336, 155136, 3)
-        assert len(series.levels) == 10
-        assert series.is_pyramidal
-        page = series.levels[3].pages[0]
-        assert page.compression == JPEG
-        assert page.photometric == YCBCR
-        assert page.planarconfig == CONTIG
-        assert page.tags['ImageWidth'].value == 19456
-        assert page.tags['ImageLength'].value == 9728
-        assert page.imagewidth == 19392
-        assert page.imagelength == 9792
-        # assert data
-        image = tif.asarray(series=0, level=3)
-        assert image.shape == (9792, 19392, 3)
-        assert image[300, 400, 1] == 226
-        assert image[9791, 0, 1] == 0
-        assert_aszarr_method(series, image, level=3)
-        assert__str__(tif)
-
-        if SKIP_ZARR:
-            return
-
-        # write fsspec
-        from imagecodecs.numcodecs import register_codecs
-
-        register_codecs('imagecodecs_jpeg', verbose=False)
-        url = os.path.dirname(fname).replace('\\', '/')
-        with TempFileName('issue_philips_fsspec', ext='.json') as jsonfile:
-            page.aszarr().write_fsspec(jsonfile, url, version=0)
-            mapper = fsspec.get_mapper(
-                'reference://',
-                fo=jsonfile,
-                target_protocol='file',
-                remote_protocol='file',
-            )
-            zobj = zarr.open(mapper, mode='r')
-            assert_array_equal(zobj[:], image)
-
-
 class TestExceptions:
     """Test various Exceptions and Warnings."""
 
     data = random_data(numpy.uint16, (5, 13, 17))
 
     @pytest.fixture(scope='class')
     def fname(self):
@@ -8514,15 +8445,15 @@
         assert track['IlluminationChannels'][5]['Name'] == '488'
         assert track['IlluminationChannels'][5]['Wavelength'] == 488.0
         assert_aszarr_method(tif)
         assert_aszarr_method(tif, series=1)
         assert__str__(tif, 0)
 
 
-@pytest.mark.skipif(SKIP_PRIVATE or SKIP_CODECS, reason=REASON)
+@pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
 def test_read_lsm_unbounderror():
     """Test read LSM: MZSYX (196, 2, 33, 512, 512)."""
     # file is > 4GB with no time axis
     fname = private_file('lsm/48h-CM-C-2.lsm')
     with TiffFile(fname) as tif:
         assert tif.is_lsm
         assert tif.byteorder == '<'
@@ -8588,14 +8519,91 @@
         # assert lsm_scan_info tags
         tags = tif.lsm_metadata['ScanInformation']
         assert tags['ScanMode'] == 'Stack'
         assert tags['User'] == 'lfdguest1'
         assert__str__(tif)
 
 
+@pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
+def test_read_lsm_incomplete(caplog):
+    """Test read LSM: MZSYX (196, 2, 33, 512, 512)."""
+    # file is ~18 GB incompletely written, dataoffsets zeroed
+    fname = private_file('lsm/NTERT_NM-50_x2.lsm')
+
+    with TiffFile(fname) as tif:
+        assert 'LSM file incompletely written' in caplog.text
+        assert tif.is_lsm
+        assert tif.byteorder == '<'
+        assert len(tif.pages) == 2450
+        assert len(tif.series) == 2
+        # assert page properties
+        page = tif.pages.first
+        assert page.is_lsm
+        assert page.is_contiguous
+        assert page.photometric == RGB
+        assert page.planarconfig == SEPARATE
+        assert page.imagewidth == 512
+        assert page.imagelength == 512
+        assert page.bitspersample == 16
+        assert page.samplesperpixel == 33
+        page = tif.pages[1]
+        assert page.is_reduced
+        assert page.photometric == RGB
+        assert page.planarconfig == SEPARATE
+        assert page.compression == NONE
+        assert page.imagewidth == 128
+        assert page.imagelength == 128
+        assert page.samplesperpixel == 3
+        assert page.bitspersample == 8
+        # assert series properties
+        series = tif.series[0]
+        assert series.pages[-1].dataoffsets[0] == 0
+        assert series.shape == (25, 49, 33, 512, 512)
+        assert series.get_shape(False) == (25, 1, 1, 49, 33, 512, 512)
+        assert series.dtype == numpy.uint16
+        assert series.axes == 'MTCYX'
+        assert series.get_axes(False) == 'MPZTCYX'
+        assert series.kind == 'lsm'
+        if 1:
+            series = tif.series[1]
+            assert series.shape == (25, 49, 3, 128, 128)
+            assert series.get_shape(False) == (25, 1, 1, 49, 3, 128, 128)
+            assert series.dtype == numpy.uint8
+            assert series.axes == 'MTSYX'
+            assert series.get_axes(False) == 'MPZTSYX'
+            assert series.kind == 'lsm'
+        # assert data
+        data = tif.asarray()
+        assert isinstance(data, numpy.ndarray)
+        assert data.flags['C_CONTIGUOUS']
+        assert data.shape == (25, 49, 33, 512, 512)
+        assert data.dtype == numpy.uint16
+        assert data[24, 45, 32, 511, 511] == 14648
+        # assert_aszarr_method(tif, data)
+        if 1:
+            data = tif.asarray(series=1)
+            assert isinstance(data, numpy.ndarray)
+            assert data.shape == (25, 49, 3, 128, 128)
+            assert data.dtype == numpy.uint8
+            assert numpy.sum(data[24, 45]) == 0
+            # assert_aszarr_method(tif, series=1)
+        # assert lsm_info tags
+        tags = tif.lsm_metadata
+        assert tags['DimensionX'] == 512
+        assert tags['DimensionY'] == 512
+        assert tags['DimensionZ'] == 1
+        assert tags['DimensionTime'] == 49
+        assert tags['DimensionChannels'] == 33
+        # assert lsm_scan_info tags
+        tags = tif.lsm_metadata['ScanInformation']
+        assert tags['ScanMode'] == 'Plane'
+        assert tags['User'] == 'lfdguest1'
+        assert__str__(tif)
+
+
 @pytest.mark.skipif(SKIP_PRIVATE or SKIP_CODECS, reason=REASON)
 def test_read_lsm_earpax2isl11():
     """Test read LSM: TZCYX (1, 19, 3, 512, 512) uint8, RGB, LZW."""
     fname = private_file('lsm/earpax2isl11.lzw.lsm')
     with TiffFile(fname) as tif:
         assert tif.is_lsm
         assert tif.byteorder == '<'
@@ -12307,41 +12315,218 @@
     # https://camelyon17.grand-challenge.org/Data/
     fname = private_file('PhilipsDP/test_001.tif')
     with TiffFile(fname) as tif:
         assert len(tif.series) == 1
         assert len(tif.pages) == 9
         assert tif.is_philips
         assert tif.philips_metadata.endswith('</DataObject>')
+
         page = tif.pages.first
         assert page.compression == JPEG
         assert page.photometric == YCBCR
         assert page.planarconfig == CONTIG
         assert page.tags['ImageWidth'].value == 86016
         assert page.tags['ImageLength'].value == 89600
-        assert page.imagewidth == 85654
-        assert page.imagelength == 89225
+        assert page.imagewidth == 86016
+        assert page.imagelength == 89600
         assert page.bitspersample == 8
         assert page.samplesperpixel == 3
         assert page.tags['Software'].value == 'Philips DP v1.0'
+
         series = tif.series[0]
         assert series.kind == 'philips'
-        assert series.shape == (89225, 85654, 3)
+        assert series.shape == (89600, 86016, 3)
         assert len(series.levels) == 9
         assert series.is_pyramidal
+        assert series.levels[1].shape == (44800, 43008, 3)
+        assert series.levels[2].shape == (22400, 21504, 3)
+        assert series.levels[3].shape == (11200, 10752, 3)
+        assert series.levels[4].shape == (5600, 5376, 3)
+        assert series.levels[5].shape == (2800, 2688, 3)
+        assert series.levels[6].shape == (1400, 1344, 3)
+        assert series.levels[7].shape == (700, 672, 3)
+        assert series.levels[8].shape == (350, 336, 3)
+
+        page = series.levels[1].keyframe
+        assert page.compression == JPEG
+        assert page.photometric == YCBCR
+        assert page.planarconfig == CONTIG
+        assert page.tags['ImageWidth'].value == 43008
+        assert page.tags['ImageLength'].value == 45056
+        assert page.imagewidth == 43008
+        assert page.imagelength == 44800
+
+        for level in range(1, 9):
+            tif.asarray(series=0, level=level)
+
         # assert data
         image = tif.asarray(series=0, level=5)
-        assert image.shape == (2789, 2677, 3)
+        assert image.shape == (2800, 2688, 3)
         assert image[300, 400, 1] == 206
         assert_aszarr_method(series, image, level=5)
         assert_aszarr_method(series, image, level=5, chunkmode='page')
         assert__str__(tif)
 
 
 @pytest.mark.skipif(
     SKIP_PRIVATE or SKIP_CODECS or not imagecodecs.JPEG, reason=REASON
+)
+def test_read_philips_issue249():
+    """Test write_fsspec with Philips slide missing row of tiles."""
+    # https://github.com/cgohlke/tifffile/issues/249
+    fname = private_file('PhilipsDP/patient_080_node_2.tif')
+    with TiffFile(fname) as tif:
+        assert len(tif.series) == 2
+        assert len(tif.pages) == 11
+        assert tif.is_philips
+        assert tif.philips_metadata.endswith('</DataObject>')
+
+        page = tif.pages.first
+        assert page.compression == JPEG
+        assert page.photometric == YCBCR
+        assert page.planarconfig == CONTIG
+        assert page.tags['ImageWidth'].value == 155136
+        assert page.tags['ImageLength'].value == 78336
+        assert page.imagewidth == 155136
+        assert page.imagelength == 78336
+        assert page.bitspersample == 8
+        assert page.samplesperpixel == 3
+        assert page.tags['Software'].value == 'Philips DP v1.0'
+
+        series = tif.series[1]
+        assert series.kind == 'philips'
+        assert series.name == 'Macro'
+        assert series.shape == (801, 1756, 3)
+        assert len(series.levels) == 1
+        assert not series.is_pyramidal
+
+        series = tif.series[0]
+        assert series.kind == 'philips'
+        assert series.name == 'Baseline'
+        assert series.shape == (78336, 155136, 3)
+        assert len(series.levels) == 10
+        assert series.is_pyramidal
+
+        page = series.levels[3].keyframe
+        assert page.compression == JPEG
+        assert page.photometric == YCBCR
+        assert page.planarconfig == CONTIG
+        assert page.tags['ImageWidth'].value == 19456
+        assert page.tags['ImageLength'].value == 9728
+        assert page.imagewidth == 19392
+        assert page.imagelength == 9792
+
+        for level in range(1, 10):
+            tif.asarray(series=0, level=level)
+
+        # assert data
+        image = tif.asarray(series=0, level=3)
+        assert image.shape == (9792, 19392, 3)
+        assert image[300, 400, 1] == 226
+        assert image[9791, 0, 1] == 0
+        assert_aszarr_method(series, image, level=3)
+        assert__str__(tif)
+
+        if SKIP_ZARR:
+            return
+
+        # write fsspec
+        from imagecodecs.numcodecs import register_codecs
+
+        register_codecs('imagecodecs_jpeg', verbose=False)
+        url = os.path.dirname(fname).replace('\\', '/')
+        with TempFileName('issue_philips_fsspec', ext='.json') as jsonfile:
+            page.aszarr().write_fsspec(jsonfile, url, version=0)
+            mapper = fsspec.get_mapper(
+                'reference://',
+                fo=jsonfile,
+                target_protocol='file',
+                remote_protocol='file',
+            )
+            zobj = zarr.open(mapper, mode='r')
+            assert_array_equal(zobj[:], image)
+
+
+@pytest.mark.skipif(
+    SKIP_PRIVATE or SKIP_CODECS or not imagecodecs.JPEG, reason=REASON
+)
+def test_read_philips_issue253():
+    """Test read Philips DP pyramid with seemingly extra column of tiles."""
+    # https://github.com/cgohlke/tifffile/issues/253
+    # https://registry.opendata.aws/camelyon/
+    fname = private_file('PhilipsDP/sample.tiff')
+    with TiffFile(fname) as tif:
+        assert len(tif.series) == 3
+        assert len(tif.pages) == 12
+        assert tif.is_philips
+        assert tif.philips_metadata.endswith('</DataObject>')
+
+        page = tif.pages.first
+        assert page.compression == JPEG
+        assert page.photometric == RGB
+        assert page.planarconfig == CONTIG
+        assert page.tags['ImageWidth'].value == 188416
+        assert page.tags['ImageLength'].value == 93696
+        assert page.imagewidth == 188416
+        assert page.imagelength == 93696
+        assert page.bitspersample == 8
+        assert page.samplesperpixel == 3
+        assert page.tags['Software'].value == 'Philips DP v1.0'
+
+        series = tif.series[1]
+        assert series.kind == 'philips'
+        assert series.name == 'Macro'
+        assert series.shape == (812, 1806, 3)
+        assert not series.is_pyramidal
+
+        series = tif.series[2]
+        assert series.kind == 'philips'
+        assert series.name == 'Label'
+        assert series.shape == (812, 671, 3)
+        assert not series.is_pyramidal
+
+        series = tif.series[0]
+        assert series.kind == 'philips'
+        assert series.name == 'Baseline'
+        assert series.shape == (93696, 188416, 3)
+        assert len(series.levels) == 10
+        assert series.is_pyramidal
+        assert series.levels[1].shape == (46848, 94208, 3)
+        assert series.levels[2].shape == (23424, 47104, 3)
+        assert series.levels[3].shape == (11712, 23552, 3)
+        assert series.levels[4].shape == (5856, 11776, 3)
+        assert series.levels[5].shape == (2928, 5888, 3)
+        assert series.levels[6].shape == (1464, 2944, 3)
+        assert series.levels[7].shape == (732, 1472, 3)
+        assert series.levels[8].shape == (366, 736, 3)
+        assert series.levels[9].shape == (183, 368, 3)
+
+        page = series.levels[1].keyframe
+        assert page.compression == JPEG
+        assert page.photometric == RGB
+        assert page.planarconfig == CONTIG
+        assert page.tags['ImageWidth'].value == 94208
+        assert page.tags['ImageLength'].value == 47104
+        assert page.imagewidth == 94208
+        assert page.imagelength == 46848
+
+        for level in range(1, 10):
+            tif.asarray(series=0, level=level)
+
+        # assert data
+        image = tif.asarray(series=0, level=5)
+        assert image.shape == (2928, 5888, 3)
+        assert image[300, 400, 1] == 254
+        assert_aszarr_method(series, image, level=5)
+        assert_aszarr_method(series, image, level=5, chunkmode='page')
+        assert__str__(tif)
+
+
+@pytest.mark.skipif(
+    SKIP_PRIVATE or SKIP_CODECS or not imagecodecs.JPEG, reason=REASON
 )
 def test_read_zif():
     """Test read Zoomable Image Format ZIF."""
     fname = private_file('zif/ZoomifyImageExample.zif')
     with TiffFile(fname) as tif:
         # assert tif.is_zif
         assert len(tif.pages) == 5
```

### Comparing `tifffile-2024.4.24/tifffile/_imagecodecs.py` & `tifffile-2024.5.3/tifffile/_imagecodecs.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/tifffile/geodb.py` & `tifffile-2024.5.3/tifffile/geodb.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/tifffile/lsm2bin.py` & `tifffile-2024.5.3/tifffile/lsm2bin.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/tifffile/numcodecs.py` & `tifffile-2024.5.3/tifffile/numcodecs.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/tifffile/tiff2fsspec.py` & `tifffile-2024.5.3/tifffile/tiff2fsspec.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/tifffile/tiffcomment.py` & `tifffile-2024.5.3/tifffile/tiffcomment.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.24/tifffile/tifffile.py` & `tifffile-2024.5.3/tifffile/tifffile.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 (1) store NumPy arrays in TIFF (Tagged Image File Format) files, and
 (2) read image and metadata from TIFF-like files used in bioimaging.
 
 Image and metadata can be read from TIFF, BigTIFF, OME-TIFF, DNG, STK, LSM,
 SGI, NIHImage, ImageJ, MMStack, NDTiff, FluoView, ScanImage, SEQ, GEL,
 SVS, SCN, SIS, BIF, ZIF (Zoomable Image File Format), QPTIFF (QPI, PKI), NDPI,
-and GeoTIFF formatted files.
+Philips DP, and GeoTIFF formatted files.
 
 Image data can be read as NumPy arrays or Zarr arrays/groups from strips,
 tiles, pages (IFDs), SubIFDs, higher order series, and pyramidal levels.
 
 Image data can be written to TIFF, BigTIFF, OME-TIFF, and ImageJ hyperstack
 compatible files in multi-page, volumetric, pyramidal, memory-mappable,
 tiled, predicted, or compressed form.
@@ -56,15 +56,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.3
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -108,17 +108,22 @@
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2024.5.3
+
+- Pass 5080 tests.
+- Fix reading incompletely written LSM.
+- Fix reading Philips DP with extra rows of tiles (#253, breaking).
+
 2024.4.24
 
-- Pass 5077 tests.
 - Fix compatibility issue with numpy 2 (#252).
 
 2024.4.18
 
 - Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
 - Add option not to quote file names in write_fsspec.
 - Allow compress bilevel images with deflate, LZMA, and Zstd.
@@ -322,19 +327,18 @@
   structures. Tifffile can read NDPI files > 4 GB.
   JPEG compressed segments with dimensions >65530 or missing restart markers
   cannot be decoded with common JPEG libraries. Tifffile works around this
   limitation by separately decoding the MCUs between restart markers, which
   performs poorly. BitsPerSample, SamplesPerPixel, and
   PhotometricInterpretation tags may contain wrong values, which can be
   corrected using the value of tag 65441.
-- **Philips TIFF** slides store wrong ImageWidth and ImageLength tag values
+- **Philips TIFF** slides store padded ImageWidth and ImageLength tag values
   for tiled pages. The values can be corrected using the DICOM_PIXEL_SPACING
   attributes of the XML formatted description of the first page. Tile offsets
-  and byte counts may be 0 and last rows of tiles may be missing.
-  Tifffile can read Philips slides.
+  and byte counts may be 0. Tifffile can read Philips slides.
 - **Ventana/Roche BIF** slides store tiles and metadata in a BigTIFF container.
   Tiles may overlap and require stitching based on the TileJointInfo elements
   in the XMP tag. Volumetric scans are stored using the ImageDepth extension.
   Tifffile can read BIF and decode individual tiles but does not perform
   stitching.
 - **ScanImage** optionally allows corrupted non-BigTIFF files > 2 GB.
   The values of StripOffsets and StripByteCounts can be recovered using the
@@ -407,25 +411,22 @@
   https://www.loc.gov/preservation/digital/formats/content/tiff_tags.shtml
 - CIPA DC-008-2016: Exchangeable image file format for digital still cameras:
   Exif Version 2.31.
   http://www.cipa.jp/std/documents/e/DC-008-Translation-2016-E.pdf
 - The EER (Electron Event Representation) file format.
   https://github.com/fei-company/EerReaderLib
 - Digital Negative (DNG) Specification. Version 1.5.0.0, June 2012.
-  https://www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/
-  dng_spec_1.5.0.0.pdf
+  https://www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/dng_spec_1.5.0.0.pdf
 - Roche Digital Pathology. BIF image file format for digital pathology.
-  https://diagnostics.roche.com/content/dam/diagnostics/Blueprint/en/pdf/rmd/
-  Roche-Digital-Pathology-BIF-Whitepaper.pdf
+  https://diagnostics.roche.com/content/dam/diagnostics/Blueprint/en/pdf/rmd/Roche-Digital-Pathology-BIF-Whitepaper.pdf
 - Astro-TIFF specification. https://astro-tiff.sourceforge.io/
 - Aperio Technologies, Inc. Digital Slides and Third-Party Data Interchange.
   Aperio_Digital_Slides_and_Third-party_data_interchange.pdf
 - PerkinElmer image format.
-  https://downloads.openmicroscopy.org/images/Vectra-QPTIFF/perkinelmer/
-  PKI_Image%20Format.docx
+  https://downloads.openmicroscopy.org/images/Vectra-QPTIFF/perkinelmer/PKI_Image%20Format.docx
 - NDTiffStorage. https://github.com/micro-manager/NDTiffStorage
 
 Examples
 --------
 
 Write a NumPy array to a single-page RGB TIFF file:
 
@@ -832,15 +833,15 @@
 
     $ python -m tifffile temp.ome.tif
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.4.24'
+__version__ = '2024.5.3'
 
 __all__ = [
     'TiffFile',
     'TiffFileError',
     'TiffFrame',
     'TiffPage',
     'TiffPages',
@@ -4327,22 +4328,14 @@
                     self.pages._load_virtual_frames()
                 except Exception as exc:
                     logger().error(
                         f'{self!r} <TiffPages._load_virtual_frames> '
                         f'raised {exc!r}'
                     )
 
-            elif self.is_philips:
-                try:
-                    self._philips_load_pages()
-                except Exception as exc:
-                    logger().error(
-                        f'{self!r} <_philips_load_pages> raised {exc!r}'
-                    )
-
             elif self.is_ndpi:
                 try:
                     self._ndpi_load_pages()
                 except Exception as exc:
                     logger().error(
                         f'{self!r} <_ndpi_load_pages> raised {exc!r}'
                     )
@@ -5249,29 +5242,127 @@
                     s.name = 'Map'
                     # s.kind += '_map'
         self.is_uniform = False
         return series
 
     def _series_philips(self) -> list[TiffPageSeries] | None:
         """Return pyramidal image series in Philips DP file."""
-        series = self._series_generic()
-        if series is None:
+        from xml.etree import ElementTree as etree
+
+        series = []
+        pages = self.pages
+        pages.cache = False
+        pages.useframes = False
+        pages.set_keyframe(0)
+        pages._load()
+
+        meta = self.philips_metadata
+        assert meta is not None
+
+        try:
+            tree = etree.fromstring(meta)
+        except etree.ParseError as exc:
+            logger().error(f'{self!r} Philips series raised {exc!r}')
             return None
-        for s in series:
-            s.kind = 'philips'
-            if s.is_pyramidal:
-                # TODO: read name from XML
-                s.name = 'Baseline'
-                # if s.dtype.itemsize == 1:
-                #     for level in s.levels:
-                #         level.keyframe.nodata = 255
-            elif s.keyframe.description.startswith('Macro'):
-                s.name = 'Macro'
-            elif s.keyframe.description.startswith('Label'):
-                s.name = 'Label'
+
+        pixel_spacing = [
+            tuple(float(v) for v in elem.text.replace('"', '').split())
+            for elem in tree.findall(
+                './/*'
+                '/DataObject[@ObjectType="PixelDataRepresentation"]'
+                '/Attribute[@Name="DICOM_PIXEL_SPACING"]'
+            )
+            if elem.text is not None
+        ]
+        if len(pixel_spacing) < 2:
+            logger().error(
+                f'{self!r} Philips series {len(pixel_spacing)=} < 2'
+            )
+            return None
+
+        series_dict: dict[str, list[TiffPage]] = {}
+        series_dict['Level'] = []
+        series_dict['Other'] = []
+        for page in pages:
+            assert isinstance(page, TiffPage)
+            if page.description.startswith('Macro'):
+                series_dict['Macro'] = [page]
+            elif page.description.startswith('Label'):
+                series_dict['Label'] = [page]
+            elif not page.is_tiled:
+                series_dict['Other'].append(page)
+            else:
+                series_dict['Level'].append(page)
+
+        levels = series_dict.pop('Level')
+        if len(levels) != len(pixel_spacing):
+            logger().error(
+                f'{self!r} Philips series '
+                f'{len(levels)=} != {len(pixel_spacing)=}'
+            )
+            return None
+
+        # fix padding of sublevels
+        imagewidth0 = levels[0].imagewidth
+        imagelength0 = levels[0].imagelength
+        h0, w0 = pixel_spacing[0]
+        for serie, (h, w) in zip(levels[1:], pixel_spacing[1:]):
+            page = serie.keyframe
+            # if page.dtype.itemsize == 1:
+            #     page.nodata = 255
+
+            imagewidth = imagewidth0 // int(round(w / w0))
+            imagelength = imagelength0 // int(round(h / h0))
+
+            if page.imagewidth - page.tilewidth >= imagewidth:
+                logger().warning(
+                    f'{self!r} Philips series {page.index=} '
+                    f'{page.imagewidth=}-{page.tilewidth=} >= {imagewidth=}'
+                )
+                page.imagewidth -= page.tilewidth - 1
+            elif page.imagewidth < imagewidth:
+                logger().warning(
+                    f'{self!r} Philips series {page.index=} '
+                    f'{page.imagewidth=} < {imagewidth=}'
+                )
+            else:
+                page.imagewidth = imagewidth
+            imagewidth = page.imagewidth
+
+            if page.imagelength - page.tilelength >= imagelength:
+                logger().warning(
+                    f'{self!r} Philips series {page.index=} '
+                    f'{page.imagelength=}-{page.tilelength=} >= {imagelength=}'
+                )
+                page.imagelength -= page.tilelength - 1
+            # elif page.imagelength < imagelength:
+            #    # in this case image is padded with zero
+            else:
+                page.imagelength = imagelength
+            imagelength = page.imagelength
+
+            if page.shaped[-1] > 1:
+                page.shape = (imagelength, imagewidth, page.shape[-1])
+            elif page.shaped[0] > 1:
+                page.shape = (page.shape[0], imagelength, imagewidth)
+            else:
+                page.shape = (imagelength, imagewidth)
+            page.shaped = (
+                page.shaped[:2] + (imagelength, imagewidth) + page.shaped[-1:]
+            )
+
+        series = [TiffPageSeries([levels[0]], name='Baseline', kind='philips')]
+        for i, page in enumerate(levels[1:]):
+            series[0].levels.append(
+                TiffPageSeries([page], name=f'Level{i + 1}', kind='philips')
+            )
+        for key, value in series_dict.items():
+            for page in value:
+                series.append(TiffPageSeries([page], name=key, kind='philips'))
+
         self.is_uniform = False
         return series
 
     def _series_indica(self) -> list[TiffPageSeries] | None:
         """Return pyramidal image series in IndicaLabs file."""
         # TODO: need more IndicaLabs sample files
         # TODO: parse indica series from XML
@@ -6603,14 +6694,19 @@
 
         # unwrap offsets
         wrap = 0
         previousoffset = 0
         for npi in indices.flat:
             page = pages[int(npi)]
             dataoffsets = []
+            if all(i <= 0 for i in page.dataoffsets):
+                logger().warning(
+                    f'{self!r} LSM file incompletely written at {page}'
+                )
+                break
             for currentoffset in page.dataoffsets:
                 if currentoffset < previousoffset:
                     wrap += 2**32
                 dataoffsets.append(currentoffset + wrap)
                 previousoffset = currentoffset
             page.dataoffsets = tuple(dataoffsets)
 
@@ -6671,79 +6767,14 @@
                 page.bitspersample = 16
                 page.dtype = page._dtype = numpy.dtype('uint16')
                 if page.shaped[-1] > 1:
                     page.axes = page.axes[:-1]
                     page.shape = page.shape[:-1]
                     page.shaped = page.shaped[:-1] + (1,)
 
-    def _philips_load_pages(self) -> None:
-        """Read and fix all pages from Philips slide file.
-
-        The imagewidth and imagelength values of all tiled pages are corrected
-        using the DICOM_PIXEL_SPACING attributes of the XML formatted
-        description of the first page.
-
-        """
-        from xml.etree import ElementTree as etree
-
-        pages = self.pages
-        pages.cache = True
-        pages.useframes = False
-        pages._load()
-        npages = len(pages)
-        page0 = self.pages.first
-
-        root = etree.fromstring(page0.description)
-
-        width = float(page0.imagewidth)
-        length = float(page0.imagelength)
-        sizes: list[tuple[int, int]] | None = None
-        for elem in root.iter():
-            if (
-                elem.tag != 'Attribute'
-                or elem.attrib.get('Name', '') != 'DICOM_PIXEL_SPACING'
-                or elem.text is None
-            ):
-                continue
-            w, h = (float(v) for v in elem.text.replace('"', '').split())
-            if sizes is None:
-                length *= h
-                width *= w
-                sizes = []
-            else:
-                sizes.append(
-                    (
-                        int(math.ceil(length / h)),
-                        int(math.ceil(width / w)),
-                    )
-                )
-        assert sizes is not None
-        i = 0
-        for imagelength, imagewidth in sizes:
-            while i < npages and cast(TiffPage, pages[i]).tilewidth == 0:
-                # Label, Macro
-                i += 1
-                continue
-            if i == npages:
-                break
-            page = pages[i]
-            assert isinstance(page, TiffPage)
-            page.imagewidth = imagewidth
-            page.imagelength = imagelength
-            if page.shaped[-1] > 1:
-                page.shape = (imagelength, imagewidth, page.shape[-1])
-            elif page.shaped[0] > 1:
-                page.shape = (page.shape[0], imagelength, imagewidth)
-            else:
-                page.shape = (imagelength, imagewidth)
-            page.shaped = (
-                page.shaped[:2] + (imagelength, imagewidth) + page.shaped[-1:]
-            )
-            i += 1
-
     def __getattr__(self, name: str, /) -> bool:
         """Return `is_flag` attributes from first page."""
         if name[3:] in TIFF.PAGE_FLAGS:
             if not self.pages:
                 return False
             value = bool(getattr(self.pages.first, name))
             setattr(self, name, value)
```

### Comparing `tifffile-2024.4.24/tifffile.egg-info/PKG-INFO` & `tifffile-2024.5.3/tifffile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2024.4.24
+Version: 2024.5.3
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
@@ -38,15 +38,15 @@
 
 (1) store NumPy arrays in TIFF (Tagged Image File Format) files, and
 (2) read image and metadata from TIFF-like files used in bioimaging.
 
 Image and metadata can be read from TIFF, BigTIFF, OME-TIFF, DNG, STK, LSM,
 SGI, NIHImage, ImageJ, MMStack, NDTiff, FluoView, ScanImage, SEQ, GEL,
 SVS, SCN, SIS, BIF, ZIF (Zoomable Image File Format), QPTIFF (QPI, PKI), NDPI,
-and GeoTIFF formatted files.
+Philips DP, and GeoTIFF formatted files.
 
 Image data can be read as NumPy arrays or Zarr arrays/groups from strips,
 tiles, pages (IFDs), SubIFDs, higher order series, and pyramidal levels.
 
 Image data can be written to TIFF, BigTIFF, OME-TIFF, and ImageJ hyperstack
 compatible files in multi-page, volumetric, pyramidal, memory-mappable,
 tiled, predicted, or compressed form.
@@ -59,15 +59,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.24
+:Version: 2024.5.3
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -111,17 +111,22 @@
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2024.5.3
+
+- Pass 5080 tests.
+- Fix reading incompletely written LSM.
+- Fix reading Philips DP with extra rows of tiles (#253, breaking).
+
 2024.4.24
 
-- Pass 5077 tests.
 - Fix compatibility issue with numpy 2 (#252).
 
 2024.4.18
 
 - Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
 - Add option not to quote file names in write_fsspec.
 - Allow compress bilevel images with deflate, LZMA, and Zstd.
@@ -325,19 +330,18 @@
   structures. Tifffile can read NDPI files > 4 GB.
   JPEG compressed segments with dimensions >65530 or missing restart markers
   cannot be decoded with common JPEG libraries. Tifffile works around this
   limitation by separately decoding the MCUs between restart markers, which
   performs poorly. BitsPerSample, SamplesPerPixel, and
   PhotometricInterpretation tags may contain wrong values, which can be
   corrected using the value of tag 65441.
-- **Philips TIFF** slides store wrong ImageWidth and ImageLength tag values
+- **Philips TIFF** slides store padded ImageWidth and ImageLength tag values
   for tiled pages. The values can be corrected using the DICOM_PIXEL_SPACING
   attributes of the XML formatted description of the first page. Tile offsets
-  and byte counts may be 0 and last rows of tiles may be missing.
-  Tifffile can read Philips slides.
+  and byte counts may be 0. Tifffile can read Philips slides.
 - **Ventana/Roche BIF** slides store tiles and metadata in a BigTIFF container.
   Tiles may overlap and require stitching based on the TileJointInfo elements
   in the XMP tag. Volumetric scans are stored using the ImageDepth extension.
   Tifffile can read BIF and decode individual tiles but does not perform
   stitching.
 - **ScanImage** optionally allows corrupted non-BigTIFF files > 2 GB.
   The values of StripOffsets and StripByteCounts can be recovered using the
@@ -410,25 +414,22 @@
   https://www.loc.gov/preservation/digital/formats/content/tiff_tags.shtml
 - CIPA DC-008-2016: Exchangeable image file format for digital still cameras:
   Exif Version 2.31.
   http://www.cipa.jp/std/documents/e/DC-008-Translation-2016-E.pdf
 - The EER (Electron Event Representation) file format.
   https://github.com/fei-company/EerReaderLib
 - Digital Negative (DNG) Specification. Version 1.5.0.0, June 2012.
-  https://www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/
-  dng_spec_1.5.0.0.pdf
+  https://www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/dng_spec_1.5.0.0.pdf
 - Roche Digital Pathology. BIF image file format for digital pathology.
-  https://diagnostics.roche.com/content/dam/diagnostics/Blueprint/en/pdf/rmd/
-  Roche-Digital-Pathology-BIF-Whitepaper.pdf
+  https://diagnostics.roche.com/content/dam/diagnostics/Blueprint/en/pdf/rmd/Roche-Digital-Pathology-BIF-Whitepaper.pdf
 - Astro-TIFF specification. https://astro-tiff.sourceforge.io/
 - Aperio Technologies, Inc. Digital Slides and Third-Party Data Interchange.
   Aperio_Digital_Slides_and_Third-party_data_interchange.pdf
 - PerkinElmer image format.
-  https://downloads.openmicroscopy.org/images/Vectra-QPTIFF/perkinelmer/
-  PKI_Image%20Format.docx
+  https://downloads.openmicroscopy.org/images/Vectra-QPTIFF/perkinelmer/PKI_Image%20Format.docx
 - NDTiffStorage. https://github.com/micro-manager/NDTiffStorage
 
 Examples
 --------
 
 Write a NumPy array to a single-page RGB TIFF file:
```

### Comparing `tifffile-2024.4.24/tifffile.egg-info/SOURCES.txt` & `tifffile-2024.5.3/tifffile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

