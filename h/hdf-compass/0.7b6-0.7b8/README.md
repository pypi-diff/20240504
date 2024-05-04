# Comparing `tmp/hdf_compass-0.7b6.tar.gz` & `tmp/hdf_compass-0.7b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hdf_compass-0.7b6.tar", last modified: Thu Jun 21 12:25:17 2018, max compression
+gzip compressed data, was "dist\hdf_compass-0.7b8.tar", last modified: Sun Dec  2 20:20:14 2018, max compression
```

## Comparing `hdf_compass-0.7b6.tar` & `hdf_compass-0.7b8.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/additional_legal/
--rw-rw-rw-   0        0        0     3346 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/additional_legal/ADIOS_Copyrights_and_Licenses.txt
--rw-rw-rw-   0        0        0     2160 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/additional_legal/cartopy_Copyrights_and_Licenses.txt
--rw-rw-rw-   0        0        0    11754 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/additional_legal/h5py_Copyrights_and_Licenses.txt
--rw-rw-rw-   0        0        0     1828 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/additional_legal/hydroffice_bag_Copyrights_and_Licenses.txt
--rw-rw-rw-   0        0        0     1419 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/additional_legal/HydroPro_Icons_Terms.txt
--rw-rw-rw-   0        0        0     7978 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/additional_legal/KDE_Oxygen_Icon_Set_Copyright_and_License.txt
--rw-rw-rw-   0        0        0     2767 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/additional_legal/matplotlib_Copyright_and_License.txt
--rw-rw-rw-   0        0        0     1624 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/additional_legal/NumPy_Copyright_and_License.txt
--rw-rw-rw-   0        0        0     1154 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/additional_legal/PyDAP_Copyright_and_License.txt
--rw-rw-rw-   0        0        0    18660 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/additional_legal/PyInstaller_Copyrights_and_Licenses.txt
--rw-rw-rw-   0        0        0     2747 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/additional_legal/Python_Copyright_and_License.txt
--rw-rw-rw-   0        0        0    32786 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/additional_legal/wxWidgets_Copyrights_and_Licenses.txt
--rw-rw-rw-   0        0        0     5782 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/COPYING
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/data/
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/data/asc/
--rw-rw-rw-   0        0        0      196 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/data/asc/sample.asc
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/data/bag/
--rw-rw-rw-   0        0        0    28128 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/data/bag/bdb_00.bag
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/data/hdf5/
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/data/hdf5/Download/
--rw-rw-rw-   0        0        0     1133 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/data/hdf5/Download/download_data.py
--rw-rw-rw-   0        0        0     8292 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/data/hdf5/tall.h5
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/docs/
--rw-rw-rw-   0        0        0     9397 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/docs/conf.py
--rw-rw-rw-   0        0        0    10863 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/docs/data_model.rst
--rw-rw-rw-   0        0        0       71 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/docs/how_to_contribute.rst
--rw-rw-rw-   0        0        0       63 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/docs/how_to_freeze.rst
--rw-rw-rw-   0        0        0       37 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/docs/how_to_install.rst
--rw-rw-rw-   0        0        0      667 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/docs/how_to_release.rst
--rw-rw-rw-   0        0        0       29 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/docs/how_to_use.rst
--rw-rw-rw-   0        0        0     1322 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/docs/index.rst
--rw-rw-rw-   0        0        0     5729 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/docs/license.rst
--rwxrwxrwx   0        0        0     7252 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/docs/make.bat
--rw-rw-rw-   0        0        0       33 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/docs/requirements.rst
--rw-rw-rw-   0        0        0      330 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/HDFCompass.desktop
--rw-rw-rw-   0        0        0   167754 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/HDFCompass.icns
--rw-rw-rw-   0        0        0    68714 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/HDFCompass.ico
--rw-rw-rw-   0        0        0     1719 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/HDFCompass.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/adios_model/
--rw-rw-rw-   0        0        0     9438 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/adios_model/model.py
--rw-rw-rw-   0        0        0     1354 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/adios_model/test.py
--rw-rw-rw-   0        0        0     1227 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/adios_model/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/array_model/
--rw-rw-rw-   0        0        0     8871 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/array_model/model.py
--rw-rw-rw-   0        0        0     1116 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/array_model/test.py
--rw-rw-rw-   0        0        0     1064 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/array_model/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/asc_model/
--rw-rw-rw-   0        0        0     5621 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/asc_model/model.py
--rw-rw-rw-   0        0        0     1112 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/asc_model/test.py
--rw-rw-rw-   0        0        0     1048 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/asc_model/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/bag_model/
--rw-rw-rw-   0        0        0    22860 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/bag_model/model.py
--rw-rw-rw-   0        0        0     1334 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/bag_model/test.py
--rw-rw-rw-   0        0        0     1256 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/bag_model/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/compass_model/
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/
--rw-rw-rw-   0        0        0      800 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/array_16.png
--rw-rw-rw-   0        0        0     5320 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/array_64.png
--rw-rw-rw-   0        0        0      365 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/folder_16.png
--rw-rw-rw-   0        0        0     1684 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/folder_64.png
--rw-rw-rw-   0        0        0      689 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/image_16.png
--rw-rw-rw-   0        0        0     5749 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/image_64.png
--rw-rw-rw-   0        0        0      903 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/kv_16.png
--rw-rw-rw-   0        0        0     6429 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/kv_64.png
--rw-rw-rw-   0        0        0     7814 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/license.txt
--rw-rw-rw-   0        0        0      265 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/readme.txt
--rw-rw-rw-   0        0        0      676 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/text_16.png
--rw-rw-rw-   0        0        0     3877 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/text_64.png
--rw-rw-rw-   0        0        0      900 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/unknown_16.png
--rw-rw-rw-   0        0        0     5470 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/unknown_64.png
--rw-rw-rw-   0        0        0      606 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/xml_16.png
--rw-rw-rw-   0        0        0     4224 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_model/icons/xml_64.png
--rw-rw-rw-   0        0        0    15786 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_model/model.py
--rw-rw-rw-   0        0        0     7485 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_model/test.py
--rw-rw-rw-   0        0        0     1139 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_model/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/array/
--rw-rw-rw-   0        0        0    23901 2018-06-19 09:18:41.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/array/frame.py
--rw-rw-rw-   0        0        0     7018 2018-06-19 09:53:01.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/array/plot.py
--rw-rw-rw-   0        0        0     1041 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/array/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/container/
--rw-rw-rw-   0        0        0     8646 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/container/frame.py
--rw-rw-rw-   0        0        0     8438 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/container/list.py
--rw-rw-rw-   0        0        0     1049 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/container/__init__.py
--rw-rw-rw-   0        0        0     2028 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/events.py
--rw-rw-rw-   0        0        0    19035 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/frame.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_array/
--rw-rw-rw-   0        0        0    14655 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_array/frame.py
--rw-rw-rw-   0        0        0     8821 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_array/plot.py
--rw-rw-rw-   0        0        0     1208 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_array/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_surface/
--rw-rw-rw-   0        0        0    14665 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_surface/frame.py
--rw-rw-rw-   0        0        0    10257 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_surface/plot.py
--rw-rw-rw-   0        0        0     1212 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_surface/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/
--rw-rw-rw-   0        0        0     2658 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/favicon_32.png
--rw-rw-rw-   0        0        0     4915 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/favicon_48.png
--rw-rw-rw-   0        0        0     1146 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_back_24.png
--rw-rw-rw-   0        0        0     1479 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_back_32.png
--rw-rw-rw-   0        0        0     1145 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_next_24.png
--rw-rw-rw-   0        0        0     1497 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_next_32.png
--rw-rw-rw-   0        0        0     1094 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_top_24.png
--rw-rw-rw-   0        0        0     1547 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_top_32.png
--rw-rw-rw-   0        0        0     1127 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_up_24.png
--rw-rw-rw-   0        0        0     1537 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_up_32.png
--rw-rw-rw-   0        0        0     7814 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/license.txt
--rw-rw-rw-   0        0        0    78588 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/logo.png
--rw-rw-rw-   0        0        0      268 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/readme.txt
--rw-rw-rw-   0        0        0     1121 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/save_24.png
--rw-rw-rw-   0        0        0     1005 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/view_icon_24.png
--rw-rw-rw-   0        0        0      543 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/view_icon_32.png
--rw-rw-rw-   0        0        0      711 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/view_list_24.png
--rw-rw-rw-   0        0        0      508 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/view_list_32.png
--rw-rw-rw-   0        0        0      743 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/view_tree_32.png
--rw-rw-rw-   0        0        0     1135 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/viz_copy_24.png
--rw-rw-rw-   0        0        0      885 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/viz_plot_24.png
--rw-rw-rw-   0        0        0     1652 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/viz_plot_32.png
--rw-rw-rw-   0        0        0      896 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/xml_validate_24.png
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/image/
--rw-rw-rw-   0        0        0     2310 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/image/frame.py
--rw-rw-rw-   0        0        0     1043 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/image/__init__.py
--rw-rw-rw-   0        0        0     4842 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/info.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/keyvalue/
--rw-rw-rw-   0        0        0     3397 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/keyvalue/frame.py
--rw-rw-rw-   0        0        0     1047 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/keyvalue/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/text/
--rw-rw-rw-   0        0        0     7131 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/text/frame.py
--rw-rw-rw-   0        0        0    10895 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/text/text_ctrl.py
--rw-rw-rw-   0        0        0     1211 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/text/__init__.py
--rw-rw-rw-   0        0        0     8961 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/viewer.py
--rw-rw-rw-   0        0        0     1069 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/__init__.py
--rw-rw-rw-   0        0        0     1715 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/compass_viewer/__main__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/filesystem_model/
--rw-rw-rw-   0        0        0     4856 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/filesystem_model/model.py
--rw-rw-rw-   0        0        0     1113 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/filesystem_model/test.py
--rw-rw-rw-   0        0        0     1056 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/filesystem_model/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/hdf5rest_model/
--rw-rw-rw-   0        0        0    17741 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/hdf5rest_model/hdf5dtype.py
--rw-rw-rw-   0        0        0    14054 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/hdf5rest_model/model.py
--rw-rw-rw-   0        0        0     1411 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/hdf5rest_model/test.py
--rw-rw-rw-   0        0        0     1084 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/hdf5rest_model/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/hdf5_model/
--rw-rw-rw-   0        0        0    10206 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/hdf5_model/model.py
--rw-rw-rw-   0        0        0     1184 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/hdf5_model/test.py
--rw-rw-rw-   0        0        0     1064 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/hdf5_model/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/opendap_model/
--rw-rw-rw-   0        0        0     8053 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/opendap_model/model.py
--rw-rw-rw-   0        0        0      304 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/hdf_compass/opendap_model/test.py
--rw-rw-rw-   0        0        0     1068 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/opendap_model/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass/utils/
--rw-rw-rw-   0        0        0     2001 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/utils/utils.py
--rw-rw-rw-   0        0        0     1103 2018-06-21 12:25:13.000000 hdf_compass-0.7b6/hdf_compass/utils/__init__.py
--rw-rw-rw-   0        0        0      208 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/hdf_compass/__init__.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass.egg-info/
--rw-rw-rw-   0        0        0        1 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0     5526 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      132 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass.egg-info/requires.txt
--rw-rw-rw-   0        0        0     5338 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/hdf_compass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      389 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/MANIFEST.in
--rw-rw-rw-   0        0        0     5526 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/PKG-INFO
--rw-rw-rw-   0        0        0     3755 2018-04-08 22:16:59.000000 hdf_compass-0.7b6/README.rst
--rw-rw-rw-   0        0        0      245 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/setup.cfg
--rw-rw-rw-   0        0        0     4772 2018-06-21 12:25:13.000000 hdf_compass-0.7b6/setup.py
-drwxrwxrwx   0        0        0        0 2018-06-21 12:25:17.000000 hdf_compass-0.7b6/tests/
--rw-rw-rw-   0        0        0    13551 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/tests/HDFCompassTestLog.rst
--rw-rw-rw-   0        0        0    13697 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/tests/HDFCompassTestPlan.rst
--rw-rw-rw-   0        0        0      196 2018-04-08 22:16:26.000000 hdf_compass-0.7b6/tests/sample.asc
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:13.000000 hdf_compass-0.7b8/additional_legal/
+-rw-rw-rw-   0        0        0     3346 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/additional_legal/ADIOS_Copyrights_and_Licenses.txt
+-rw-rw-rw-   0        0        0     2160 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/additional_legal/cartopy_Copyrights_and_Licenses.txt
+-rw-rw-rw-   0        0        0    11754 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/additional_legal/h5py_Copyrights_and_Licenses.txt
+-rw-rw-rw-   0        0        0     1830 2018-12-02 19:17:16.000000 hdf_compass-0.7b8/additional_legal/hydroffice_bag_Copyrights_and_Licenses.txt
+-rw-rw-rw-   0        0        0     1419 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/additional_legal/HydroPro_Icons_Terms.txt
+-rw-rw-rw-   0        0        0     7978 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/additional_legal/KDE_Oxygen_Icon_Set_Copyright_and_License.txt
+-rw-rw-rw-   0        0        0     2767 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/additional_legal/matplotlib_Copyright_and_License.txt
+-rw-rw-rw-   0        0        0     1624 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/additional_legal/NumPy_Copyright_and_License.txt
+-rw-rw-rw-   0        0        0     1154 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/additional_legal/PyDAP_Copyright_and_License.txt
+-rw-rw-rw-   0        0        0    18660 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/additional_legal/PyInstaller_Copyrights_and_Licenses.txt
+-rw-rw-rw-   0        0        0     2747 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/additional_legal/Python_Copyright_and_License.txt
+-rw-rw-rw-   0        0        0    32786 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/additional_legal/wxWidgets_Copyrights_and_Licenses.txt
+-rw-rw-rw-   0        0        0     5781 2018-12-02 19:35:08.000000 hdf_compass-0.7b8/COPYING
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:13.000000 hdf_compass-0.7b8/data/
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:13.000000 hdf_compass-0.7b8/data/asc/
+-rw-rw-rw-   0        0        0      196 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/data/asc/sample.asc
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:13.000000 hdf_compass-0.7b8/data/bag/
+-rw-rw-rw-   0        0        0    28128 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/data/bag/bdb_00.bag
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/data/hdf5/
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/data/hdf5/Download/
+-rw-rw-rw-   0        0        0     1133 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/data/hdf5/Download/download_data.py
+-rw-rw-rw-   0        0        0     8292 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/data/hdf5/tall.h5
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/docs/
+-rw-rw-rw-   0        0        0     9397 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/docs/conf.py
+-rw-rw-rw-   0        0        0    10863 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/docs/data_model.rst
+-rw-rw-rw-   0        0        0       71 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/docs/how_to_contribute.rst
+-rw-rw-rw-   0        0        0       63 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/docs/how_to_freeze.rst
+-rw-rw-rw-   0        0        0       37 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/docs/how_to_install.rst
+-rw-rw-rw-   0        0        0      667 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/docs/how_to_release.rst
+-rw-rw-rw-   0        0        0       29 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/docs/how_to_use.rst
+-rw-rw-rw-   0        0        0     1322 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/docs/index.rst
+-rw-rw-rw-   0        0        0     5730 2018-12-02 19:17:16.000000 hdf_compass-0.7b8/docs/license.rst
+-rwxrwxrwx   0        0        0     7252 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/docs/make.bat
+-rw-rw-rw-   0        0        0       33 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/docs/requirements.rst
+-rw-rw-rw-   0        0        0      330 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/HDFCompass.desktop
+-rw-rw-rw-   0        0        0   167754 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/HDFCompass.icns
+-rw-rw-rw-   0        0        0    68714 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/HDFCompass.ico
+-rw-rw-rw-   0        0        0     1719 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/HDFCompass.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/adios_model/
+-rw-rw-rw-   0        0        0     9438 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/adios_model/model.py
+-rw-rw-rw-   0        0        0     1354 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/adios_model/test.py
+-rw-rw-rw-   0        0        0     1227 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/adios_model/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/array_model/
+-rw-rw-rw-   0        0        0     8871 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/array_model/model.py
+-rw-rw-rw-   0        0        0     1116 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/array_model/test.py
+-rw-rw-rw-   0        0        0     1064 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/array_model/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/asc_model/
+-rw-rw-rw-   0        0        0     5621 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/asc_model/model.py
+-rw-rw-rw-   0        0        0     1112 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/asc_model/test.py
+-rw-rw-rw-   0        0        0     1048 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/asc_model/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/bag_model/
+-rw-rw-rw-   0        0        0    22863 2018-12-02 19:17:16.000000 hdf_compass-0.7b8/hdf_compass/bag_model/model.py
+-rw-rw-rw-   0        0        0     1334 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/bag_model/test.py
+-rw-rw-rw-   0        0        0     1256 2018-12-02 19:11:27.000000 hdf_compass-0.7b8/hdf_compass/bag_model/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/compass_model/
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/
+-rw-rw-rw-   0        0        0      800 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/array_16.png
+-rw-rw-rw-   0        0        0     5320 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/array_64.png
+-rw-rw-rw-   0        0        0      365 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/folder_16.png
+-rw-rw-rw-   0        0        0     1684 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/folder_64.png
+-rw-rw-rw-   0        0        0      689 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/image_16.png
+-rw-rw-rw-   0        0        0     5749 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/image_64.png
+-rw-rw-rw-   0        0        0      903 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/kv_16.png
+-rw-rw-rw-   0        0        0     6429 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/kv_64.png
+-rw-rw-rw-   0        0        0     7814 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/license.txt
+-rw-rw-rw-   0        0        0      265 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/readme.txt
+-rw-rw-rw-   0        0        0      676 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/text_16.png
+-rw-rw-rw-   0        0        0     3877 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/text_64.png
+-rw-rw-rw-   0        0        0      900 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/unknown_16.png
+-rw-rw-rw-   0        0        0     5470 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/unknown_64.png
+-rw-rw-rw-   0        0        0      606 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/xml_16.png
+-rw-rw-rw-   0        0        0     4224 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_model/icons/xml_64.png
+-rw-rw-rw-   0        0        0    15786 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_model/model.py
+-rw-rw-rw-   0        0        0     7485 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_model/test.py
+-rw-rw-rw-   0        0        0     1139 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_model/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/array/
+-rw-rw-rw-   0        0        0    23901 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/array/frame.py
+-rw-rw-rw-   0        0        0     7018 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/array/plot.py
+-rw-rw-rw-   0        0        0     1041 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/array/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/container/
+-rw-rw-rw-   0        0        0     8646 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/container/frame.py
+-rw-rw-rw-   0        0        0     8438 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/container/list.py
+-rw-rw-rw-   0        0        0     1049 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/container/__init__.py
+-rw-rw-rw-   0        0        0     2028 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/events.py
+-rw-rw-rw-   0        0        0    19035 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/frame.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_array/
+-rw-rw-rw-   0        0        0    14655 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_array/frame.py
+-rw-rw-rw-   0        0        0     9298 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_array/plot.py
+-rw-rw-rw-   0        0        0     1208 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_array/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_surface/
+-rw-rw-rw-   0        0        0    14665 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_surface/frame.py
+-rw-rw-rw-   0        0        0    10734 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_surface/plot.py
+-rw-rw-rw-   0        0        0     1212 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_surface/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/
+-rw-rw-rw-   0        0        0     2658 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/favicon_32.png
+-rw-rw-rw-   0        0        0     4915 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/favicon_48.png
+-rw-rw-rw-   0        0        0     1146 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_back_24.png
+-rw-rw-rw-   0        0        0     1479 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_back_32.png
+-rw-rw-rw-   0        0        0     1145 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_next_24.png
+-rw-rw-rw-   0        0        0     1497 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_next_32.png
+-rw-rw-rw-   0        0        0     1094 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_top_24.png
+-rw-rw-rw-   0        0        0     1547 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_top_32.png
+-rw-rw-rw-   0        0        0     1127 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_up_24.png
+-rw-rw-rw-   0        0        0     1537 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_up_32.png
+-rw-rw-rw-   0        0        0     7814 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/license.txt
+-rw-rw-rw-   0        0        0    78588 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/logo.png
+-rw-rw-rw-   0        0        0      268 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/readme.txt
+-rw-rw-rw-   0        0        0     1121 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/save_24.png
+-rw-rw-rw-   0        0        0     1005 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/view_icon_24.png
+-rw-rw-rw-   0        0        0      543 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/view_icon_32.png
+-rw-rw-rw-   0        0        0      711 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/view_list_24.png
+-rw-rw-rw-   0        0        0      508 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/view_list_32.png
+-rw-rw-rw-   0        0        0      743 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/view_tree_32.png
+-rw-rw-rw-   0        0        0     1135 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/viz_copy_24.png
+-rw-rw-rw-   0        0        0      885 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/viz_plot_24.png
+-rw-rw-rw-   0        0        0     1652 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/viz_plot_32.png
+-rw-rw-rw-   0        0        0      896 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/xml_validate_24.png
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/image/
+-rw-rw-rw-   0        0        0     2310 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/image/frame.py
+-rw-rw-rw-   0        0        0     1043 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/image/__init__.py
+-rw-rw-rw-   0        0        0     4842 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/info.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/keyvalue/
+-rw-rw-rw-   0        0        0     3397 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/keyvalue/frame.py
+-rw-rw-rw-   0        0        0     1047 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/keyvalue/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/text/
+-rw-rw-rw-   0        0        0     7131 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/text/frame.py
+-rw-rw-rw-   0        0        0    10895 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/text/text_ctrl.py
+-rw-rw-rw-   0        0        0     1211 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/text/__init__.py
+-rw-rw-rw-   0        0        0     9117 2018-12-02 19:29:12.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/viewer.py
+-rw-rw-rw-   0        0        0     1069 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/__init__.py
+-rw-rw-rw-   0        0        0     1715 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/compass_viewer/__main__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/filesystem_model/
+-rw-rw-rw-   0        0        0     4856 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/filesystem_model/model.py
+-rw-rw-rw-   0        0        0     1113 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/filesystem_model/test.py
+-rw-rw-rw-   0        0        0     1056 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/filesystem_model/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/hdf5rest_model/
+-rw-rw-rw-   0        0        0    17741 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/hdf5rest_model/hdf5dtype.py
+-rw-rw-rw-   0        0        0    14054 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/hdf5rest_model/model.py
+-rw-rw-rw-   0        0        0     1411 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/hdf5rest_model/test.py
+-rw-rw-rw-   0        0        0     1084 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/hdf5rest_model/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/hdf5_model/
+-rw-rw-rw-   0        0        0    10206 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/hdf5_model/model.py
+-rw-rw-rw-   0        0        0     1184 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/hdf5_model/test.py
+-rw-rw-rw-   0        0        0     1064 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/hdf5_model/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/opendap_model/
+-rw-rw-rw-   0        0        0     8053 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/opendap_model/model.py
+-rw-rw-rw-   0        0        0      304 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/hdf_compass/opendap_model/test.py
+-rw-rw-rw-   0        0        0     1068 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/opendap_model/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass/utils/
+-rw-rw-rw-   0        0        0     2001 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/utils/utils.py
+-rw-rw-rw-   0        0        0     1103 2018-12-02 19:11:27.000000 hdf_compass-0.7b8/hdf_compass/utils/__init__.py
+-rw-rw-rw-   0        0        0      208 2018-10-27 03:40:56.000000 hdf_compass-0.7b8/hdf_compass/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/hdf_compass.egg-info/
+-rw-rw-rw-   0        0        0        1 2018-12-02 20:20:13.000000 hdf_compass-0.7b8/hdf_compass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2018-12-02 20:20:13.000000 hdf_compass-0.7b8/hdf_compass.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2018-12-02 20:20:13.000000 hdf_compass-0.7b8/hdf_compass.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0     5730 2018-12-02 20:20:13.000000 hdf_compass-0.7b8/hdf_compass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      133 2018-12-02 20:20:13.000000 hdf_compass-0.7b8/hdf_compass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     5338 2018-12-02 20:20:13.000000 hdf_compass-0.7b8/hdf_compass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2018-12-02 20:20:13.000000 hdf_compass-0.7b8/hdf_compass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      389 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5730 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/PKG-INFO
+-rw-rw-rw-   0        0        0     3927 2018-12-02 19:17:16.000000 hdf_compass-0.7b8/README.rst
+-rw-rw-rw-   0        0        0      245 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/setup.cfg
+-rw-rw-rw-   0        0        0     4773 2018-12-02 19:12:34.000000 hdf_compass-0.7b8/setup.py
+drwxrwxrwx   0        0        0        0 2018-12-02 20:20:14.000000 hdf_compass-0.7b8/tests/
+-rw-rw-rw-   0        0        0    13551 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/tests/HDFCompassTestLog.rst
+-rw-rw-rw-   0        0        0    13697 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/tests/HDFCompassTestPlan.rst
+-rw-rw-rw-   0        0        0      196 2018-10-27 03:40:38.000000 hdf_compass-0.7b8/tests/sample.asc
```

### Comparing `hdf_compass-0.7b6/additional_legal/ADIOS_Copyrights_and_Licenses.txt` & `hdf_compass-0.7b8/additional_legal/ADIOS_Copyrights_and_Licenses.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/additional_legal/cartopy_Copyrights_and_Licenses.txt` & `hdf_compass-0.7b8/additional_legal/cartopy_Copyrights_and_Licenses.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/additional_legal/h5py_Copyrights_and_Licenses.txt` & `hdf_compass-0.7b8/additional_legal/h5py_Copyrights_and_Licenses.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/additional_legal/hydroffice_bag_Copyrights_and_Licenses.txt` & `hdf_compass-0.7b8/additional_legal/hydroffice_bag_Copyrights_and_Licenses.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 Copyright Notice and License Terms for 
-hyo.bag - BAG package for HydrOffice
+hyo2.bag - BAG package for HydrOffice
 
 -----------------------------------------------------------------------------
 
-hyo.bag
+hyo2.bag
 
 Copyright 2015 - G.Masetti and B.R.Calder.
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted for any purpose (including commercial purposes)
```

### Comparing `hdf_compass-0.7b6/additional_legal/HydroPro_Icons_Terms.txt` & `hdf_compass-0.7b8/additional_legal/HydroPro_Icons_Terms.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/additional_legal/KDE_Oxygen_Icon_Set_Copyright_and_License.txt` & `hdf_compass-0.7b8/additional_legal/KDE_Oxygen_Icon_Set_Copyright_and_License.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/additional_legal/matplotlib_Copyright_and_License.txt` & `hdf_compass-0.7b8/additional_legal/matplotlib_Copyright_and_License.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/additional_legal/NumPy_Copyright_and_License.txt` & `hdf_compass-0.7b8/additional_legal/NumPy_Copyright_and_License.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/additional_legal/PyDAP_Copyright_and_License.txt` & `hdf_compass-0.7b8/additional_legal/PyDAP_Copyright_and_License.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/additional_legal/PyInstaller_Copyrights_and_Licenses.txt` & `hdf_compass-0.7b8/additional_legal/PyInstaller_Copyrights_and_Licenses.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/additional_legal/Python_Copyright_and_License.txt` & `hdf_compass-0.7b8/additional_legal/Python_Copyright_and_License.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/additional_legal/wxWidgets_Copyrights_and_Licenses.txt` & `hdf_compass-0.7b8/additional_legal/wxWidgets_Copyrights_and_Licenses.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/COPYING` & `hdf_compass-0.7b8/COPYING`

 * *Files 2% similar despite different names*

```diff
@@ -92,19 +92,19 @@
 
     HDF5 for Python (h5py)
       Provided by: Andrew Collette and contributors
       Copyright and license information: additional_legal/h5py_Copyrights_and_Licenses.txt
       Original source: http://docs.h5py.org/en/latest/licenses.html
       License type: BSD-style license
 
-    HydrOffice BAG (hyo.bag)
+    HydrOffice BAG (hyo2.bag)
       Provided by: G.Masetti, B.R.Calder, and contributors
       Copyright and license information: additional_legal/hydroffice_bag_Copyrights_and_Licenses.txt
-      Original source: https://bitbucket.org/ccomjhc/hyo_bag/raw/tip/COPYING.txt
-      License type: BSD-style license
+      Original source: https://github.com/hydroffice/hyo2_bag/raw/master/COPYING
+      License type: LGPL v3 license
 
     NumPy
       Provided by: NumPy Developers
       Copyright and license information: additional_legal/NumPy_Copyright_and_License.txt
       Original source: http://www.numpy.org/license.html
       License type: BSD-style license
```

### Comparing `hdf_compass-0.7b6/data/bag/bdb_00.bag` & `hdf_compass-0.7b8/data/bag/bdb_00.bag`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/data/hdf5/Download/download_data.py` & `hdf_compass-0.7b8/data/hdf5/Download/download_data.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/data/hdf5/tall.h5` & `hdf_compass-0.7b8/data/hdf5/tall.h5`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/docs/conf.py` & `hdf_compass-0.7b8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/docs/data_model.rst` & `hdf_compass-0.7b8/docs/data_model.rst`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/docs/how_to_release.rst` & `hdf_compass-0.7b8/docs/how_to_release.rst`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/docs/index.rst` & `hdf_compass-0.7b8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/docs/license.rst` & `hdf_compass-0.7b8/docs/license.rst`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     HDF5 for Python (h5py)
       Provided by: Andrew Collette and contributors
       Copyright and license information: additional_legal/h5py_Copyrights_and_Licenses.txt
       Original source: http://docs.h5py.org/en/latest/licenses.html
       License type: BSD-style license
 
-    HydrOffice BAG (hyo.bag)
+    HydrOffice BAG (hyo2.bag)
       Provided by: G.Masetti, B.R.Calder, and contributors
       Copyright and license information: additional_legal/hydroffice_bag_Copyrights_and_Licenses.txt
       Original source: https://bitbucket.org/ccomjhc/hyo_bag/raw/tip/COPYING.txt
       License type: BSD-style license
 
     NumPy
       Provided by: NumPy Developers
```

### Comparing `hdf_compass-0.7b6/docs/make.bat` & `hdf_compass-0.7b8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/HDFCompass.icns` & `hdf_compass-0.7b8/HDFCompass.icns`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/HDFCompass.ico` & `hdf_compass-0.7b8/HDFCompass.ico`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/HDFCompass.py` & `hdf_compass-0.7b8/HDFCompass.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/adios_model/model.py` & `hdf_compass-0.7b8/hdf_compass/adios_model/model.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/adios_model/test.py` & `hdf_compass-0.7b8/hdf_compass/adios_model/test.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/adios_model/__init__.py` & `hdf_compass-0.7b8/hdf_compass/adios_model/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/array_model/model.py` & `hdf_compass-0.7b8/hdf_compass/array_model/model.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/array_model/test.py` & `hdf_compass-0.7b8/hdf_compass/array_model/test.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/array_model/__init__.py` & `hdf_compass-0.7b8/hdf_compass/array_model/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/asc_model/model.py` & `hdf_compass-0.7b8/hdf_compass/asc_model/model.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/asc_model/test.py` & `hdf_compass-0.7b8/hdf_compass/asc_model/test.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/asc_model/__init__.py` & `hdf_compass-0.7b8/hdf_compass/asc_model/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/bag_model/model.py` & `hdf_compass-0.7b8/hdf_compass/bag_model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 Implementation of compass_model classes for BAG files.
 """
 from itertools import groupby
 import os.path as op
 import posixpath as pp
 import h5py
 
-from hyo.bag import is_bag
-from hyo.bag import BAGFile
-from hyo.bag import BAGError
+from hyo2.bag import is_bag
+from hyo2.bag import BAGFile
+from hyo2.bag import BAGError
 
 from hdf_compass import compass_model
 from hdf_compass.utils import url2path
 
 import logging
 logger = logging.getLogger(__name__)
```

### Comparing `hdf_compass-0.7b6/hdf_compass/bag_model/test.py` & `hdf_compass-0.7b8/hdf_compass/bag_model/test.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/bag_model/__init__.py` & `hdf_compass-0.7b8/hdf_compass/bag_model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 #                                                                            #
 # author: gmasetti@ccom.unh.edu                                              #
 ##############################################################################
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 from hdf_compass.bag_model.model import BAGStore, BAGDataset, BAGGroup, BAGImage, BAGKV
 
 import logging
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
```

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/array_16.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/array_16.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/array_64.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/array_64.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/folder_64.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/folder_64.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/image_16.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/image_16.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/image_64.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/image_64.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/kv_16.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/kv_16.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/kv_64.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/kv_64.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/license.txt` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/license.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/text_16.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/text_16.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/text_64.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/text_64.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/unknown_16.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/unknown_16.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/unknown_64.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/unknown_64.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/xml_16.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/xml_16.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/icons/xml_64.png` & `hdf_compass-0.7b8/hdf_compass/compass_model/icons/xml_64.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/model.py` & `hdf_compass-0.7b8/hdf_compass/compass_model/model.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/test.py` & `hdf_compass-0.7b8/hdf_compass/compass_model/test.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_model/__init__.py` & `hdf_compass-0.7b8/hdf_compass/compass_model/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/array/frame.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/array/frame.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/array/plot.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/array/plot.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/array/__init__.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/array/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/container/frame.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/container/frame.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/container/list.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/container/list.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/container/__init__.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/container/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/events.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/events.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/frame.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/frame.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_array/frame.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_array/frame.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_array/plot.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_array/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,21 @@
                 self.axes.legend(tuple(lines), tuple(self.names))
 
 
 class ContourPlotFrame(PlotFrame):
     def __init__(self, data, extent, names=None, title="Contour Map"):
         self.geo_extent = extent
         logger.debug("Extent: %f, %f, %f, %f" % self.geo_extent)
+        if (self.geo_extent[0] > self.geo_extent[1]) or (self.geo_extent[2] > self.geo_extent[3]):
+            msg = "Invalid geographic extent! Check values:\n" \
+                  "- West: %f, East: %f\n" \
+                  "- South: %f, North: %f" % self.geo_extent
+            dlg = wx.MessageDialog(None, msg, "Geographic Bounding Box", wx.OK | wx.ICON_WARNING)
+            dlg.ShowModal()
+
         # need to be set before calling the parent (need for plotting)
         self.colormap = "jet"
         self.cb = None  # matplotlib color-bar
         self.surf = None
         self.xx = None
         self.yy = None
 
@@ -190,14 +197,16 @@
         grl.xformatter = LONGITUDE_FORMATTER
         grl.yformatter = LATITUDE_FORMATTER
         grl.xlabel_style = {'size': 8}
         grl.ylabel_style = {'size': 8}
         grl.ylabels_right = False
         grl.xlabels_top = False
 
+        self.axes.set_extent(self.geo_extent, crs=ccrs.PlateCarree())
+
         if self.cb:
             self.cb.on_mappable_changed(img)
         else:
             self.cb = plt.colorbar(img, ax=self.axes)
         self.cb.ax.tick_params(labelsize=8)
 
     def change_cursor(self, event):
```

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_array/__init__.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_array/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_surface/frame.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_surface/frame.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_surface/plot.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_surface/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,14 +97,21 @@
                 self.axes.legend(tuple(lines), tuple(self.names))
 
 
 class ContourPlotFrame(PlotFrame):
     def __init__(self, data, extent, names=None, title="Surface Map"):
         self.geo_extent = extent
         logger.debug("Extent: %f, %f, %f, %f" % self.geo_extent)
+        if (self.geo_extent[0] > self.geo_extent[1]) or (self.geo_extent[2] > self.geo_extent[3]):
+            msg = "Invalid geographic extent! Check values:\n" \
+                  "- West: %f, East: %f\n" \
+                  "- South: %f, North: %f" % self.geo_extent
+            dlg = wx.MessageDialog(None, msg, "Geographic Bounding Box", wx.OK | wx.ICON_WARNING)
+            dlg.ShowModal()
+
         # need to be set before calling the parent (need for plotting)
         self.colormap = LinearSegmentedColormap.from_list("BAG",
                                                           ["#63006c", "#2b4ef4", "#2f73ff", "#4b8af4", "#bee2bf"])
         # register a new colormap
         cm.register_cmap(cmap=self.colormap)
         self.cb = None  # matplotlib color-bar
         self.xx = None
@@ -214,27 +221,29 @@
                 self.surf = self.data[::row_stride, ::col_stride]
                 blended_surface = ls.shade(self.surf, cmap=self.colormap, vert_exag=5, blend_mode="overlay",
                                            vmin=np.nanmin(self.surf), vmax=np.nanmax(self.surf))
 
             logger.debug("too big: %s x %s > subsampled to %s x %s"
                          % (self.data.shape[0], self.data.shape[1], self.surf.shape[0], self.surf.shape[1]))
 
-        self.axes.coastlines(resolution='50m', color='gray', linewidth=1)
         img = self.axes.imshow(blended_surface, origin='lower', cmap=self.colormap,
                                extent=self.geo_extent, transform=ccrs.PlateCarree())
         img.set_clim(vmin=np.nanmin(self.surf), vmax=np.nanmax(self.surf))
+        self.axes.coastlines(resolution='50m', color='gray', linewidth=1)
         # add gridlines with labels only on the left and on the bottom
         grl = self.axes.gridlines(crs=ccrs.PlateCarree(), color='gray', draw_labels=True)
         grl.xformatter = LONGITUDE_FORMATTER
         grl.yformatter = LATITUDE_FORMATTER
         grl.xlabel_style = {'size': 8}
         grl.ylabel_style = {'size': 8}
         grl.ylabels_right = False
         grl.xlabels_top = False
 
+        self.axes.set_extent(self.geo_extent, crs=ccrs.PlateCarree())
+
         if self.cb:
             self.cb.on_mappable_changed(img)
         else:
             self.cb = plt.colorbar(img, ax=self.axes)
         self.cb.ax.tick_params(labelsize=8)
 
     def change_cursor(self, event):
```

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/geo_surface/__init__.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/geo_surface/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/favicon_32.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/favicon_32.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/favicon_48.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/favicon_48.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_back_24.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_back_24.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_back_32.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_back_32.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_next_24.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_next_24.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_next_32.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_next_32.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_top_24.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_top_24.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_top_32.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_top_32.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_up_24.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_up_24.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/go_up_32.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/go_up_32.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/license.txt` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/license.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/logo.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/logo.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/save_24.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/save_24.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/view_icon_24.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/view_icon_24.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/view_icon_32.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/view_icon_32.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/view_list_24.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/view_list_24.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/view_tree_32.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/view_tree_32.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/viz_copy_24.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/viz_copy_24.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/viz_plot_24.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/viz_plot_24.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/viz_plot_32.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/viz_plot_32.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/icons/xml_validate_24.png` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/icons/xml_validate_24.png`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/image/frame.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/image/frame.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/image/__init__.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/info.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/info.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/keyvalue/frame.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/keyvalue/frame.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/keyvalue/__init__.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/keyvalue/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/text/frame.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/text/frame.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/text/text_ctrl.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/text/text_ctrl.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/text/__init__.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/text/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/viewer.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,19 @@
     import platform
     logger.debug("Python %s %s on %s %s (%s)" % (platform.python_version(), platform.architecture()[0],
                                                  platform.uname()[0], platform.uname()[2], platform.uname()[4]))
     import numpy
     logger.debug("numpy %s" % numpy.__version__)
     logger.debug("matplotlib %s" % matplotlib.__version__)
     logger.debug("wxPython %s" % wx.__version__)
+    try:
+        import cartopy
+        logger.debug("cartopy %s" % cartopy.__version__)
+    except ImportError:
+        logger.debug("cartopy N/A")
 
     from hdf_compass import compass_model
 
     try:
         from hdf_compass import filesystem_model
     except ImportError:
         logger.warning("Filesystem plugin: NOT loaded")
@@ -208,17 +213,17 @@
         logger.debug("h5py %s" % h5py.__version__)
     except ImportError as e:
         logger.info(e)
         logger.warning("HDF5 plugin: NOT loaded")
 
     try:
         from hdf_compass import bag_model
-        from hyo import bag
+        from hyo2 import bag
         from lxml import etree
-        logger.debug("hyo.bag %s" % bag.__version__)
+        logger.debug("hyo2.bag %s" % bag.__version__)
         logger.debug("lxml %s (libxml %s, libxslt %s)"
                      % (etree.__version__, ".".join(str(i) for i in etree.LIBXML_VERSION),
                         ".".join(str(i) for i in etree.LIBXSLT_VERSION)))
     except (ImportError, OSError):
         logger.warning("BAG plugin: NOT loaded")
 
     try:
```

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/__init__.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/compass_viewer/__main__.py` & `hdf_compass-0.7b8/hdf_compass/compass_viewer/__main__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/filesystem_model/model.py` & `hdf_compass-0.7b8/hdf_compass/filesystem_model/model.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/filesystem_model/test.py` & `hdf_compass-0.7b8/hdf_compass/filesystem_model/test.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/filesystem_model/__init__.py` & `hdf_compass-0.7b8/hdf_compass/filesystem_model/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/hdf5rest_model/hdf5dtype.py` & `hdf_compass-0.7b8/hdf_compass/hdf5rest_model/hdf5dtype.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/hdf5rest_model/model.py` & `hdf_compass-0.7b8/hdf_compass/hdf5rest_model/model.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/hdf5rest_model/test.py` & `hdf_compass-0.7b8/hdf_compass/hdf5rest_model/test.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/hdf5rest_model/__init__.py` & `hdf_compass-0.7b8/hdf_compass/hdf5rest_model/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/hdf5_model/model.py` & `hdf_compass-0.7b8/hdf_compass/hdf5_model/model.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/hdf5_model/test.py` & `hdf_compass-0.7b8/hdf_compass/hdf5_model/test.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/hdf5_model/__init__.py` & `hdf_compass-0.7b8/hdf_compass/hdf5_model/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/opendap_model/model.py` & `hdf_compass-0.7b8/hdf_compass/opendap_model/model.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/opendap_model/__init__.py` & `hdf_compass-0.7b8/hdf_compass/opendap_model/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/utils/utils.py` & `hdf_compass-0.7b8/hdf_compass/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/hdf_compass/utils/__init__.py` & `hdf_compass-0.7b8/hdf_compass/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 from hdf_compass.utils.utils import is_darwin, is_win, is_linux, url2path, path2url, data_url
 
 
-__version__ = "0.7.b6"
+__version__ = "0.7.b8"
```

### Comparing `hdf_compass-0.7b6/hdf_compass.egg-info/PKG-INFO` & `hdf_compass-0.7b8/hdf_compass.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdf-compass
-Version: 0.7b6
+Version: 0.7b8
 Summary: An experimental viewer program for HDF5 and related formats.
 Home-page: https://github.com/HDFGroup/hdf-compass/
 Author: HDFGroup
 Author-email: help@hdfgroup.org
 License: BSD-like license
 Description: HDF Compass
         ===========
@@ -52,15 +52,15 @@
         
         * `Python 3.6 <https://www.python.org/downloads/>`_
         * `NumPy <https://github.com/numpy/numpy>`_
         * `Matplotlib <https://github.com/matplotlib/matplotlib>`_
         * `wxPython Phoenix 4.0.0+ <https://github.com/wxWidgets/Phoenix>`_ (`PyPI <https://pypi.python.org/pypi/wxPython>`_ and `extra wheels for Linux <https://wxpython.org/pages/downloads/>`_)
         * `Cartopy <https://github.com/SciTools/cartopy>`_
         * `h5py <https://github.com/h5py/h5py>`_ *[HDF plugin]*
-        * `hyo.bag <https://bitbucket.org/ccomjhc/hyo_bag>`_ *[BAG plugin]*
+        * `hyo2.bag <https://bitbucket.org/ccomjhc/hyo_bag>`_ *[BAG plugin]*
         * `Pydap <https://github.com/robertodealmeida/pydap>`_ *[OPeNDAP plugin]* (>=3.3)
         * `Requests <https://github.com/kennethreitz/requests>`_ *[HDF Rest API plugin]*
         * `adios <https://github.com/ornladios/ADIOS>`_ *[ADIOS Plugin]* (Linux/OSX only)
         
         For packaging the app:
         
         * `PyInstaller <https://github.com/pyinstaller/pyinstaller>`_ *(>= 3.3 or `latest dev <https://github.com/pyinstaller/pyinstaller/archive/develop.zip>`_ )*
@@ -77,14 +77,18 @@
         build of python...".  In this case use the pythonw command:
         
             ``$ pythonw HDFCompass.py``
                    
         Note: on Mac, HDF Compass doesn't create an initial window, use the system Application
         menu to open a file or remote resource.
         
+        Note: If you are using conda and see debug message like "No module named 'h5py'" with the h5py package installed,
+        install python.app: ``$ conda install python.app``
+        
+        
         
         Packaging
         ---------
         
         Single-file:
         
             ``$ pyinstaller --clean -y HDFCompass.1file.spec``
@@ -111,11 +115,11 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Office/Business :: Office Suites
 Classifier: Topic :: Utilities
+Provides-Extra: GeoNodes
 Provides-Extra: ADIOS
 Provides-Extra: OpenDAP
-Provides-Extra: GeoNodes
 Provides-Extra: BAG
```

### Comparing `hdf_compass-0.7b6/hdf_compass.egg-info/SOURCES.txt` & `hdf_compass-0.7b8/hdf_compass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/PKG-INFO` & `hdf_compass-0.7b8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdf_compass
-Version: 0.7b6
+Version: 0.7b8
 Summary: An experimental viewer program for HDF5 and related formats.
 Home-page: https://github.com/HDFGroup/hdf-compass/
 Author: HDFGroup
 Author-email: help@hdfgroup.org
 License: BSD-like license
 Description: HDF Compass
         ===========
@@ -52,15 +52,15 @@
         
         * `Python 3.6 <https://www.python.org/downloads/>`_
         * `NumPy <https://github.com/numpy/numpy>`_
         * `Matplotlib <https://github.com/matplotlib/matplotlib>`_
         * `wxPython Phoenix 4.0.0+ <https://github.com/wxWidgets/Phoenix>`_ (`PyPI <https://pypi.python.org/pypi/wxPython>`_ and `extra wheels for Linux <https://wxpython.org/pages/downloads/>`_)
         * `Cartopy <https://github.com/SciTools/cartopy>`_
         * `h5py <https://github.com/h5py/h5py>`_ *[HDF plugin]*
-        * `hyo.bag <https://bitbucket.org/ccomjhc/hyo_bag>`_ *[BAG plugin]*
+        * `hyo2.bag <https://bitbucket.org/ccomjhc/hyo_bag>`_ *[BAG plugin]*
         * `Pydap <https://github.com/robertodealmeida/pydap>`_ *[OPeNDAP plugin]* (>=3.3)
         * `Requests <https://github.com/kennethreitz/requests>`_ *[HDF Rest API plugin]*
         * `adios <https://github.com/ornladios/ADIOS>`_ *[ADIOS Plugin]* (Linux/OSX only)
         
         For packaging the app:
         
         * `PyInstaller <https://github.com/pyinstaller/pyinstaller>`_ *(>= 3.3 or `latest dev <https://github.com/pyinstaller/pyinstaller/archive/develop.zip>`_ )*
@@ -77,14 +77,18 @@
         build of python...".  In this case use the pythonw command:
         
             ``$ pythonw HDFCompass.py``
                    
         Note: on Mac, HDF Compass doesn't create an initial window, use the system Application
         menu to open a file or remote resource.
         
+        Note: If you are using conda and see debug message like "No module named 'h5py'" with the h5py package installed,
+        install python.app: ``$ conda install python.app``
+        
+        
         
         Packaging
         ---------
         
         Single-file:
         
             ``$ pyinstaller --clean -y HDFCompass.1file.spec``
@@ -111,11 +115,11 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Office/Business :: Office Suites
 Classifier: Topic :: Utilities
+Provides-Extra: GeoNodes
 Provides-Extra: ADIOS
 Provides-Extra: OpenDAP
-Provides-Extra: GeoNodes
 Provides-Extra: BAG
```

### Comparing `hdf_compass-0.7b6/README.rst` & `hdf_compass-0.7b8/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 * `Python 3.6 <https://www.python.org/downloads/>`_
 * `NumPy <https://github.com/numpy/numpy>`_
 * `Matplotlib <https://github.com/matplotlib/matplotlib>`_
 * `wxPython Phoenix 4.0.0+ <https://github.com/wxWidgets/Phoenix>`_ (`PyPI <https://pypi.python.org/pypi/wxPython>`_ and `extra wheels for Linux <https://wxpython.org/pages/downloads/>`_)
 * `Cartopy <https://github.com/SciTools/cartopy>`_
 * `h5py <https://github.com/h5py/h5py>`_ *[HDF plugin]*
-* `hyo.bag <https://bitbucket.org/ccomjhc/hyo_bag>`_ *[BAG plugin]*
+* `hyo2.bag <https://bitbucket.org/ccomjhc/hyo_bag>`_ *[BAG plugin]*
 * `Pydap <https://github.com/robertodealmeida/pydap>`_ *[OPeNDAP plugin]* (>=3.3)
 * `Requests <https://github.com/kennethreitz/requests>`_ *[HDF Rest API plugin]*
 * `adios <https://github.com/ornladios/ADIOS>`_ *[ADIOS Plugin]* (Linux/OSX only)
 
 For packaging the app:
 
 * `PyInstaller <https://github.com/pyinstaller/pyinstaller>`_ *(>= 3.3 or `latest dev <https://github.com/pyinstaller/pyinstaller/archive/develop.zip>`_ )*
@@ -69,14 +69,18 @@
 build of python...".  In this case use the pythonw command:
 
     ``$ pythonw HDFCompass.py``
            
 Note: on Mac, HDF Compass doesn't create an initial window, use the system Application
 menu to open a file or remote resource.
 
+Note: If you are using conda and see debug message like "No module named 'h5py'" with the h5py package installed,
+install python.app: ``$ conda install python.app``
+
+
 
 Packaging
 ---------
 
 Single-file:
 
     ``$ pyinstaller --clean -y HDFCompass.1file.spec``
```

### Comparing `hdf_compass-0.7b6/setup.py` & `hdf_compass-0.7b8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # ---------------------------------------------------------------------------
 
 # Create a dict with the basic information that is passed to setup after keys are added.
 setup_args = dict()
 
 setup_args['name'] = 'hdf_compass'
 # The adopted versioning scheme follow PEP40
-setup_args['version'] = '0.7.b6'
+setup_args['version'] = '0.7.b8'
 setup_args['url'] = 'https://github.com/HDFGroup/hdf-compass/'
 setup_args['license'] = 'BSD-like license'
 setup_args['author'] = 'HDFGroup'
 setup_args['author_email'] = 'help@hdfgroup.org'
 
 #
 # descriptive stuff
@@ -95,15 +95,15 @@
         "h5py",
         "wxPython",
         "requests"
     ]
 setup_args['extras_require'] =\
     {
         "GeoNodes": ["cartopy[plotting]", ],  # required for visualization of GeoArray and GeoSurface nodes
-        "BAG": ["hyo.bag", ],  # required by BAG plugin
+        "BAG": ["hyo2.bag", ],  # required by BAG plugin
         "OpenDAP": ["pydap>=3.2", ],  # required by OpenDAP plugin, there is an issue
                                       # with pydap 3.2: https://github.com/pydap/pydap/issues/66
         "ADIOS": ["adios>=1.9.1b19", ],  # required by ADIOS plugin
     }
 # hdf_compass namespace, packages and other files
 setup_args['namespace_packages'] = ['hdf_compass']
 setup_args['packages'] = find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests", "*.test*",
```

### Comparing `hdf_compass-0.7b6/tests/HDFCompassTestLog.rst` & `hdf_compass-0.7b8/tests/HDFCompassTestLog.rst`

 * *Files identical despite different names*

### Comparing `hdf_compass-0.7b6/tests/HDFCompassTestPlan.rst` & `hdf_compass-0.7b8/tests/HDFCompassTestPlan.rst`

 * *Files identical despite different names*

