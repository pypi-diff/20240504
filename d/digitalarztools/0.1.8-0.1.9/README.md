# Comparing `tmp/digitalarztools-0.1.8.tar.gz` & `tmp/digitalarztools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/digitalarztools-0.1.8.tar", last modified: Wed Nov 15 10:51:13 2023, max compression
+gzip compressed data, was "dist/digitalarztools-0.1.9.tar", last modified: Tue Dec 12 09:53:48 2023, max compression
```

## Comparing `digitalarztools-0.1.8.tar` & `digitalarztools-0.1.9.tar`

### file list

```diff
@@ -1,145 +1,149 @@
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.325578 digitalarztools-0.1.8/
--rw-r--r--   0 atherashraf   (501) staff       (20)      616 2023-11-15 10:51:13.325043 digitalarztools-0.1.8/PKG-INFO
--rw-r--r--   0 atherashraf   (501) staff       (20)     1484 2023-05-28 07:28:15.000000 digitalarztools-0.1.8/README.md
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.194085 digitalarztools-0.1.8/digitalarztools/
--rw-r--r--   0 atherashraf   (501) staff       (20)        2 2022-12-04 11:04:00.000000 digitalarztools-0.1.8/digitalarztools/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.199875 digitalarztools-0.1.8/digitalarztools/adapters/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-03-15 19:09:16.000000 digitalarztools-0.1.8/digitalarztools/adapters/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3525 2023-08-03 11:25:22.000000 digitalarztools-0.1.8/digitalarztools/adapters/db.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     8305 2023-10-25 21:40:52.000000 digitalarztools-0.1.8/digitalarztools/adapters/manager-old.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     9914 2023-10-25 21:40:52.000000 digitalarztools-0.1.8/digitalarztools/adapters/manager.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      924 2023-07-31 07:52:11.000000 digitalarztools-0.1.8/digitalarztools/adapters/model_utils.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.201737 digitalarztools-0.1.8/digitalarztools/distributions/
--rw-r--r--   0 atherashraf   (501) staff       (20)     5256 2023-05-28 07:28:15.000000 digitalarztools-0.1.8/digitalarztools/distributions/GumbleDistribution.py
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-05-28 07:28:15.000000 digitalarztools-0.1.8/digitalarztools/distributions/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.204311 digitalarztools-0.1.8/digitalarztools/io/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 11:46:14.000000 digitalarztools-0.1.8/digitalarztools/io/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.208460 digitalarztools-0.1.8/digitalarztools/io/datasets/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/datasets/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    42583 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/datasets/rio_landsat.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      173 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/datasets/rio_modis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2263 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/datasets/rio_probav_viirs.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7553 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/file_io.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      801 2023-05-28 08:35:47.000000 digitalarztools-0.1.8/digitalarztools/io/image_io.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.219263 digitalarztools-0.1.8/digitalarztools/io/raster/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/raster/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    11586 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/raster/band_process.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    10191 2023-10-21 13:33:07.000000 digitalarztools-0.1.8/digitalarztools/io/raster/cog_raster.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    15208 2023-09-17 09:28:32.000000 digitalarztools-0.1.8/digitalarztools/io/raster/gdal_raster.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2635 2023-09-17 09:28:32.000000 digitalarztools-0.1.8/digitalarztools/io/raster/gdal_raster_io.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     8497 2023-09-17 09:28:32.000000 digitalarztools-0.1.8/digitalarztools/io/raster/hdf_reader.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1875 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/raster/indices.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.220876 digitalarztools-0.1.8/digitalarztools/io/raster/opencv/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/raster/opencv/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     6860 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/raster/opencv/segmentation.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2121 2023-09-17 09:28:32.000000 digitalarztools-0.1.8/digitalarztools/io/raster/rio_extraction.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     9846 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/raster/rio_process.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    36769 2023-11-15 10:50:38.000000 digitalarztools-0.1.8/digitalarztools/io/raster/rio_raster.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      603 2023-05-28 07:28:15.000000 digitalarztools-0.1.8/digitalarztools/io/url_io.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.224185 digitalarztools-0.1.8/digitalarztools/io/vector/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/vector/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    13644 2023-10-18 18:54:38.000000 digitalarztools-0.1.8/digitalarztools/io/vector/gpd_vector.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    13359 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/io/vector/gpd_vector_old.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.230456 digitalarztools-0.1.8/digitalarztools/pipelines/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.8/digitalarztools/pipelines/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     5622 2023-09-17 09:22:23.000000 digitalarztools-0.1.8/digitalarztools/pipelines/alos_palser.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.231964 digitalarztools-0.1.8/digitalarztools/pipelines/config/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.1.8/digitalarztools/pipelines/config/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     4183 2023-05-28 07:28:15.000000 digitalarztools-0.1.8/digitalarztools/pipelines/config/data_centers.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.234550 digitalarztools-0.1.8/digitalarztools/pipelines/earth_explorer/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.1.8/digitalarztools/pipelines/earth_explorer/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     5639 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/pipelines/earth_explorer/landsat.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    15210 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/pipelines/earth_explorer/m2m.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1445 2023-09-17 09:22:23.000000 digitalarztools-0.1.8/digitalarztools/pipelines/fao_livestock.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.236261 digitalarztools-0.1.8/digitalarztools/pipelines/gee/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.237235 digitalarztools-0.1.8/digitalarztools/pipelines/gee/analysis/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/analysis/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1035 2023-02-09 19:26:46.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/analysis/indices.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.247938 digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2019 2023-05-28 07:28:15.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/auth.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      887 2022-12-14 14:45:50.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/feature_collection.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2748 2023-02-09 19:26:46.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/gee_api.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1092 2023-02-09 19:26:46.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/gee_map.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     8867 2023-06-03 12:56:03.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/image.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     6624 2023-05-28 07:28:15.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/image_collection.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     4954 2023-05-28 07:28:15.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/region.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.252317 digitalarztools-0.1.8/digitalarztools/pipelines/gee/tags/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/tags/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      861 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/tags/hydro.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1484 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/tags/lulc.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1436 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/tags/precipitation.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1143 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gee/tags/soil_moisture.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.256197 digitalarztools-0.1.8/digitalarztools/pipelines/gmap/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-08-01 22:32:01.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gmap/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2098 2023-08-03 11:10:47.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gmap/models.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     6833 2023-09-17 09:27:23.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gmap/poi.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      477 2023-09-17 09:27:23.000000 digitalarztools-0.1.8/digitalarztools/pipelines/gmap/test.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      213 2023-02-09 19:26:46.000000 digitalarztools-0.1.8/digitalarztools/pipelines/grace.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.262305 digitalarztools-0.1.8/digitalarztools/pipelines/nasa/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.1.8/digitalarztools/pipelines/nasa/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2994 2023-09-17 09:27:23.000000 digitalarztools-0.1.8/digitalarztools/pipelines/nasa/chirp.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    13068 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/pipelines/nasa/geos.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    24731 2023-09-17 09:27:22.000000 digitalarztools-0.1.8/digitalarztools/pipelines/nasa/merra.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    10724 2023-02-09 19:26:46.000000 digitalarztools-0.1.8/digitalarztools/pipelines/nasa/variables_info.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.272011 digitalarztools-0.1.8/digitalarztools/pipelines/soil_grids/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.1.8/digitalarztools/pipelines/soil_grids/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3624 2023-09-17 09:22:23.000000 digitalarztools-0.1.8/digitalarztools/pipelines/soil_grids/n_van_genuchten.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    12840 2023-09-17 09:22:23.000000 digitalarztools-0.1.8/digitalarztools/pipelines/soil_grids/soil_contents.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     4918 2023-09-17 09:22:23.000000 digitalarztools-0.1.8/digitalarztools/pipelines/soil_grids/theta_fc.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3708 2023-09-17 09:22:23.000000 digitalarztools-0.1.8/digitalarztools/pipelines/soil_grids/theta_res.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7300 2023-09-17 09:22:23.000000 digitalarztools-0.1.8/digitalarztools/pipelines/soil_grids/theta_sat2.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     4043 2023-09-17 09:27:23.000000 digitalarztools-0.1.8/digitalarztools/pipelines/srtm.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.273884 digitalarztools-0.1.8/digitalarztools/propcessing/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.307109 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1512 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/biomass_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    14835 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/clear_sky_radiation.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3828 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/constants.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3700 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/dem_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1427 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/emissivity_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    17336 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/et_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     6426 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/leaf_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    39751 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/meteo_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3811 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/resistance_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7415 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/roughness_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     9895 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/soil_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    40168 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/soil_moisture.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    49086 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/solar_radiation.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    15057 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/temperature_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    27093 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/unstable.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7841 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/vegitation_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      666 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/analysis/water_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    37949 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/energy_blance_model.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.309668 digitalarztools-0.1.8/digitalarztools/propcessing/operations/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/operations/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3927 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/operations/distance_raster.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1595 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/operations/transformation.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7238 2023-09-17 09:13:20.000000 digitalarztools-0.1.8/digitalarztools/propcessing/operations/utils.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.310630 digitalarztools-0.1.8/digitalarztools/test/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.8/digitalarztools/test/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.312386 digitalarztools-0.1.8/digitalarztools/test/raster/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.8/digitalarztools/test/raster/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      913 2022-12-14 14:45:50.000000 digitalarztools-0.1.8/digitalarztools/test/raster/test_functionalities.py
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.8/digitalarztools/test/test_config.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.320487 digitalarztools-0.1.8/digitalarztools/utils/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.8/digitalarztools/utils/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7383 2023-03-02 21:25:38.000000 digitalarztools-0.1.8/digitalarztools/utils/date_utils.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1128 2023-02-09 19:26:46.000000 digitalarztools-0.1.8/digitalarztools/utils/logger.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     5686 2023-10-21 13:33:07.000000 digitalarztools-0.1.8/digitalarztools/utils/s3_utils.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1009 2023-02-09 19:26:46.000000 digitalarztools-0.1.8/digitalarztools/utils/waitbar_console.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.197000 digitalarztools-0.1.8/digitalarztools.egg-info/
--rw-r--r--   0 atherashraf   (501) staff       (20)      616 2023-11-15 10:51:13.000000 digitalarztools-0.1.8/digitalarztools.egg-info/PKG-INFO
--rw-r--r--   0 atherashraf   (501) staff       (20)     5041 2023-11-15 10:51:13.000000 digitalarztools-0.1.8/digitalarztools.egg-info/SOURCES.txt
--rw-r--r--   0 atherashraf   (501) staff       (20)        1 2023-11-15 10:51:13.000000 digitalarztools-0.1.8/digitalarztools.egg-info/dependency_links.txt
--rw-r--r--   0 atherashraf   (501) staff       (20)     1915 2023-11-15 10:51:13.000000 digitalarztools-0.1.8/digitalarztools.egg-info/requires.txt
--rw-r--r--   0 atherashraf   (501) staff       (20)       21 2023-11-15 10:51:13.000000 digitalarztools-0.1.8/digitalarztools.egg-info/top_level.txt
--rw-r--r--   0 atherashraf   (501) staff       (20)       38 2023-11-15 10:51:13.326008 digitalarztools-0.1.8/setup.cfg
--rw-r--r--   0 atherashraf   (501) staff       (20)     1538 2023-11-15 10:50:52.000000 digitalarztools-0.1.8/setup.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-11-15 10:51:13.323868 digitalarztools-0.1.8/test/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 11:02:02.000000 digitalarztools-0.1.8/test/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      112 2022-12-03 18:32:14.000000 digitalarztools-0.1.8/test/test_config.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      787 2023-09-17 09:22:23.000000 digitalarztools-0.1.8/test/test_raster_io.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      493 2023-09-17 09:22:23.000000 digitalarztools-0.1.8/test/test_vector_io.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.859402 digitalarztools-0.1.9/
+-rw-r--r--   0 atherashraf   (501) staff       (20)      616 2023-12-12 09:53:48.858803 digitalarztools-0.1.9/PKG-INFO
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1484 2023-05-28 07:28:15.000000 digitalarztools-0.1.9/README.md
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.546570 digitalarztools-0.1.9/digitalarztools/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        2 2022-12-04 11:04:00.000000 digitalarztools-0.1.9/digitalarztools/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.557248 digitalarztools-0.1.9/digitalarztools/adapters/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-03-15 19:09:16.000000 digitalarztools-0.1.9/digitalarztools/adapters/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3525 2023-08-03 11:25:22.000000 digitalarztools-0.1.9/digitalarztools/adapters/db.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     8305 2023-10-25 21:40:52.000000 digitalarztools-0.1.9/digitalarztools/adapters/manager-old.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    11166 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/adapters/manager.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      924 2023-07-31 07:52:11.000000 digitalarztools-0.1.9/digitalarztools/adapters/model_utils.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.561414 digitalarztools-0.1.9/digitalarztools/distributions/
+-rw-r--r--   0 atherashraf   (501) staff       (20)     5256 2023-05-28 07:28:15.000000 digitalarztools-0.1.9/digitalarztools/distributions/GumbleDistribution.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-05-28 07:28:15.000000 digitalarztools-0.1.9/digitalarztools/distributions/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.566087 digitalarztools-0.1.9/digitalarztools/io/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 11:46:14.000000 digitalarztools-0.1.9/digitalarztools/io/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.571659 digitalarztools-0.1.9/digitalarztools/io/datasets/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/io/datasets/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    42583 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/io/datasets/rio_landsat.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      173 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/io/datasets/rio_modis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2263 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/io/datasets/rio_probav_viirs.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7678 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/io/file_io.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      801 2023-05-28 08:35:47.000000 digitalarztools-0.1.9/digitalarztools/io/image_io.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.578117 digitalarztools-0.1.9/digitalarztools/io/map/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/io/map/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      930 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/io/map/da_folium.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.602103 digitalarztools-0.1.9/digitalarztools/io/raster/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/io/raster/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    11586 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/io/raster/band_process.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    10191 2023-10-21 13:33:07.000000 digitalarztools-0.1.9/digitalarztools/io/raster/cog_raster.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    15208 2023-09-17 09:28:32.000000 digitalarztools-0.1.9/digitalarztools/io/raster/gdal_raster.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2635 2023-09-17 09:28:32.000000 digitalarztools-0.1.9/digitalarztools/io/raster/gdal_raster_io.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     8497 2023-09-17 09:28:32.000000 digitalarztools-0.1.9/digitalarztools/io/raster/hdf_reader.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1875 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/io/raster/indices.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.604680 digitalarztools-0.1.9/digitalarztools/io/raster/opencv/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/io/raster/opencv/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     6860 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/io/raster/opencv/segmentation.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2121 2023-09-17 09:28:32.000000 digitalarztools-0.1.9/digitalarztools/io/raster/rio_extraction.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    10213 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/io/raster/rio_process.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    36769 2023-11-15 10:50:38.000000 digitalarztools-0.1.9/digitalarztools/io/raster/rio_raster.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      603 2023-05-28 07:28:15.000000 digitalarztools-0.1.9/digitalarztools/io/url_io.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.609356 digitalarztools-0.1.9/digitalarztools/io/vector/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/io/vector/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    14886 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/io/vector/gpd_vector.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.621148 digitalarztools-0.1.9/digitalarztools/pipelines/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.9/digitalarztools/pipelines/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7908 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/pipelines/alos_palser.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.623996 digitalarztools-0.1.9/digitalarztools/pipelines/config/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.1.9/digitalarztools/pipelines/config/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     4183 2023-05-28 07:28:15.000000 digitalarztools-0.1.9/digitalarztools/pipelines/config/data_centers.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.632931 digitalarztools-0.1.9/digitalarztools/pipelines/earth_explorer/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.1.9/digitalarztools/pipelines/earth_explorer/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     5639 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/pipelines/earth_explorer/landsat.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    15210 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/pipelines/earth_explorer/m2m.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1445 2023-09-17 09:22:23.000000 digitalarztools-0.1.9/digitalarztools/pipelines/fao_livestock.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.634299 digitalarztools-0.1.9/digitalarztools/pipelines/gee/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.637847 digitalarztools-0.1.9/digitalarztools/pipelines/gee/analysis/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/analysis/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    11863 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/analysis/ground_recharge.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1035 2023-02-09 19:26:46.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/analysis/indices.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.653083 digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2019 2023-05-28 07:28:15.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/auth.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      887 2022-12-14 14:45:50.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/feature_collection.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2748 2023-02-09 19:26:46.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/gee_api.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1110 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/gee_map.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     9708 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/image.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    11883 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/image_collection.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     6483 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/region.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.666494 digitalarztools-0.1.9/digitalarztools/pipelines/gee/tags/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/tags/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      861 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/tags/hydro.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1484 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/tags/lulc.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3212 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/tags/precipitation.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     9358 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/tags/soil.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1143 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gee/tags/soil_moisture.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.670791 digitalarztools-0.1.9/digitalarztools/pipelines/gmap/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-08-01 22:32:01.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gmap/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2098 2023-08-03 11:10:47.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gmap/models.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     6833 2023-09-17 09:27:23.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gmap/poi.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      477 2023-09-17 09:27:23.000000 digitalarztools-0.1.9/digitalarztools/pipelines/gmap/test.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      213 2023-02-09 19:26:46.000000 digitalarztools-0.1.9/digitalarztools/pipelines/grace.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.680191 digitalarztools-0.1.9/digitalarztools/pipelines/nasa/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.1.9/digitalarztools/pipelines/nasa/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2994 2023-09-17 09:27:23.000000 digitalarztools-0.1.9/digitalarztools/pipelines/nasa/chirp.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    13068 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/pipelines/nasa/geos.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    24731 2023-09-17 09:27:22.000000 digitalarztools-0.1.9/digitalarztools/pipelines/nasa/merra.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    10724 2023-02-09 19:26:46.000000 digitalarztools-0.1.9/digitalarztools/pipelines/nasa/variables_info.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.688670 digitalarztools-0.1.9/digitalarztools/pipelines/soil_grids/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.1.9/digitalarztools/pipelines/soil_grids/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3624 2023-09-17 09:22:23.000000 digitalarztools-0.1.9/digitalarztools/pipelines/soil_grids/n_van_genuchten.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    12840 2023-09-17 09:22:23.000000 digitalarztools-0.1.9/digitalarztools/pipelines/soil_grids/soil_contents.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     4918 2023-09-17 09:22:23.000000 digitalarztools-0.1.9/digitalarztools/pipelines/soil_grids/theta_fc.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3708 2023-09-17 09:22:23.000000 digitalarztools-0.1.9/digitalarztools/pipelines/soil_grids/theta_res.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7300 2023-09-17 09:22:23.000000 digitalarztools-0.1.9/digitalarztools/pipelines/soil_grids/theta_sat2.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     6524 2023-12-12 09:15:26.000000 digitalarztools-0.1.9/digitalarztools/pipelines/srtm.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.699960 digitalarztools-0.1.9/digitalarztools/propcessing/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.807390 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1512 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/biomass_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    14835 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/clear_sky_radiation.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3828 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/constants.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3700 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/dem_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1427 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/emissivity_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    17336 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/et_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     6426 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/leaf_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    39751 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/meteo_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3811 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/resistance_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7415 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/roughness_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     9895 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/soil_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    40168 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/soil_moisture.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    49086 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/solar_radiation.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    15057 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/temperature_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    27093 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/unstable.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7841 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/vegitation_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      666 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/analysis/water_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    37949 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/energy_blance_model.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.834579 digitalarztools-0.1.9/digitalarztools/propcessing/operations/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/operations/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3927 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/operations/distance_raster.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1595 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/operations/transformation.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7238 2023-09-17 09:13:20.000000 digitalarztools-0.1.9/digitalarztools/propcessing/operations/utils.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.837054 digitalarztools-0.1.9/digitalarztools/test/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.9/digitalarztools/test/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.837957 digitalarztools-0.1.9/digitalarztools/test/raster/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.9/digitalarztools/test/raster/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      913 2022-12-14 14:45:50.000000 digitalarztools-0.1.9/digitalarztools/test/raster/test_functionalities.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.9/digitalarztools/test/test_config.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.846906 digitalarztools-0.1.9/digitalarztools/utils/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.1.9/digitalarztools/utils/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7383 2023-03-02 21:25:38.000000 digitalarztools-0.1.9/digitalarztools/utils/date_utils.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1128 2023-02-09 19:26:46.000000 digitalarztools-0.1.9/digitalarztools/utils/logger.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     5686 2023-10-21 13:33:07.000000 digitalarztools-0.1.9/digitalarztools/utils/s3_utils.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1009 2023-02-09 19:26:46.000000 digitalarztools-0.1.9/digitalarztools/utils/waitbar_console.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.551417 digitalarztools-0.1.9/digitalarztools.egg-info/
+-rw-r--r--   0 atherashraf   (501) staff       (20)      616 2023-12-12 09:53:48.000000 digitalarztools-0.1.9/digitalarztools.egg-info/PKG-INFO
+-rw-r--r--   0 atherashraf   (501) staff       (20)     5169 2023-12-12 09:53:48.000000 digitalarztools-0.1.9/digitalarztools.egg-info/SOURCES.txt
+-rw-r--r--   0 atherashraf   (501) staff       (20)        1 2023-12-12 09:53:48.000000 digitalarztools-0.1.9/digitalarztools.egg-info/dependency_links.txt
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1915 2023-12-12 09:53:48.000000 digitalarztools-0.1.9/digitalarztools.egg-info/requires.txt
+-rw-r--r--   0 atherashraf   (501) staff       (20)       21 2023-12-12 09:53:48.000000 digitalarztools-0.1.9/digitalarztools.egg-info/top_level.txt
+-rw-r--r--   0 atherashraf   (501) staff       (20)       38 2023-12-12 09:53:48.859604 digitalarztools-0.1.9/setup.cfg
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1537 2023-12-12 09:53:27.000000 digitalarztools-0.1.9/setup.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-12-12 09:53:48.856420 digitalarztools-0.1.9/test/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 11:02:02.000000 digitalarztools-0.1.9/test/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      112 2022-12-03 18:32:14.000000 digitalarztools-0.1.9/test/test_config.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      787 2023-09-17 09:22:23.000000 digitalarztools-0.1.9/test/test_raster_io.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      493 2023-09-17 09:22:23.000000 digitalarztools-0.1.9/test/test_vector_io.py
```

### Comparing `digitalarztools-0.1.8/PKG-INFO` & `digitalarztools-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalarztools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Digital Arz tools for applications
 Home-page: UNKNOWN
 Author: Ather Ashraf
 Author-email: atherashraf@gmail.com
 License: UNKNOWN
 Keywords: raster,vector,digitalarz
 Platform: UNKNOWN
```

### Comparing `digitalarztools-0.1.8/README.md` & `digitalarztools-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/adapters/db.py` & `digitalarztools-0.1.9/digitalarztools/adapters/db.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/adapters/manager-old.py` & `digitalarztools-0.1.9/digitalarztools/adapters/manager-old.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/adapters/manager.py` & `digitalarztools-0.1.9/digitalarztools/adapters/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 from urllib import parse
 
 import pandas as pd
 import geopandas as gpd
 from dotenv import load_dotenv
 from pydantic import BaseModel
 from shapely import wkb, wkt
-from sqlalchemy import Engine, create_engine, Select, text, MetaData, Table, Column, Integer, String
+from sqlalchemy import Engine, create_engine, Select, text, MetaData, Table, Column, Integer, String, inspect, func
 from sqlalchemy.orm import sessionmaker, Query
+from geoalchemy2 import Geometry, WKBElement
 
 from digitalarztools.utils.logger import da_logger
 
 load_dotenv()
+import logging
 
+logging.disable(logging.WARNING)
 
 class DBString(BaseModel):
     host: str
     user: str
     password: str
     name: str
     port: str
@@ -102,16 +105,17 @@
                 table_name,
                 metadata,
                 # autoload=True,
                 autoload_with=self.engine,
                 schema=schema_name
             )
             return tbl
+
         except Exception as e:
-            da_logger.error(str(e))
+            traceback.print_exc()
             return None
 
     def create_xyz_cache_table(self, table_name: str):
         meta_data = MetaData()
         xyz_table = Table(table_name, meta_data,
                           Column('id', Integer, primary_key=True, autoincrement=True),
                           Column('x', Integer),
@@ -155,25 +159,14 @@
            # :param limit_value:
            :return:
        """
         with self.get_session() as session:
             if isinstance(query, Table):
                 qs = session.query(query)
                 return qs.all()
-            # elif isinstance(query, Query):
-            #     # rs = session.execute(query).all()
-            #     # rs = query.all()
-            #     # return [row.__dict__ for row in query.all()]
-            #     # Convert the SQLAlchemy model instances to a list of dictionaries
-            #     data_dicts = [obj.__dict__ for obj in query.all()]
-            #
-            #     # Remove the '_sa_instance_state' key from each dictionary
-            #     data_dicts = [{k: v for k, v in d.items() if k != '_sa_instance_state'} for d in data_dicts]
-            #
-            #     return data_dicts
             elif isinstance(query, Select):
                 rs = session.execute(query)
                 return rs.fetchall()
             else:
                 rs = session.execute(text(query))
                 return rs.fetchall()
 
@@ -188,15 +181,16 @@
                 if isinstance(stmt, str):
                     stmt = text(stmt)
                 session.execute(stmt)
                 session.commit()
                 session.close_all()
                 return True
         except Exception as e:
-            print(traceback.print_exc())
+            traceback.print_exc()
+            # print(traceback.print_exc())
             # print("Cannot perform DDL operation")
         return False
 
     def execute_ddl(self, stmt):
         try:
             with self.get_session() as session:
                 if isinstance(stmt, str):
@@ -224,54 +218,95 @@
             tbl = self.get_sqlalchemy_table(tbl)
         # geom_cols = self.get_geometry_cols(tbl)
         data = self.get_query_data(tbl)
         # geom_col = geom_cols[0]
         # srid = self.get_geom_col_srid(tbl, geom_col)
         return pd.DataFrame(data)
 
+    @staticmethod
+    def get_table_column_names(table: Table) -> list:
+        if table is not None:
+            cols = [col.name for col in inspect(table).columns]
+            return cols
+
+    @staticmethod
+    def get_table_column_types(table: Table) -> list:
+        if table is not None:
+            cols = [col.type for col in inspect(table).columns]
+            return cols
+
+    def inspect_table(self, table_name, schema='public'):
+        # inspector = inspect(self.db)
+        # columns = inspector.get_columns(table_name, schema=schema)
+        s_t = table_name.split(".")
+        schema_name = s_t[0] if len(s_t) > 1 else "public"
+        table_name = s_t[-1]
+        tbl = self.get_sqlalchemy_table(table_name,schema_name)
+
+        # print(f"class {table_name.title().replace('_', '')}(DBBase):")
+        # for column in columns:
+        #     column = str(column).replace("{","(").replace(":","=").replace("}", ")")
+        #     print(f"\tColumn{column}")
+        # s = {"scheman":}
+        # print(f'\t__tablename__ = "{table_name}"')
+        # if schema_name != "public":
+        #     print('\t__table_args__ = {"schema": "'+schema_name+'"}')
+        for column in tbl.columns:
+            col = f"db.{str(column.type).replace(' ','_')}, nullable={column.nullable}"
+            if column.default is not None:
+                col += f", default={column.default}"
+            if column.unique:
+                col += f", default={column.unique}"
+
+            # print(f"\t{column.name}=Column({col})")
+
 
 class GeoDBManager(DBManager):
     @staticmethod
     def get_geometry_cols(table: Table) -> list:
         geom_cols = [col for col in list(table.columns) if 'geometry' in str(col.type)]
         return geom_cols
 
     def get_geom_col_srid(self, tbl, geom_col):
-        with self.get_session() as session:
-            res = session.query(tbl.c[geom_col].st_srid()).first()
-            return res[0] if len(res) > 0 else 0
+        try:
+            return geom_col.type.srid
+        except Exception as e:
+            with self.get_session() as session:
+                res = session.query(func.ST_SRID(tbl.c['geometry'])).first()
+                return res[0] if len(res) > 0 else 0
 
     @staticmethod
     def data_to_gdf(data, geom_col, srid=0, is_wkb=True):
         # data = list(data)
         # data = [row for row in data]
         if len(data) > 0:
             gdf = gpd.GeoDataFrame(data)
-            gdf = gdf.dropna(axis=0)
+            # gdf = gdf.dropna(axis=0)
             if is_wkb:
-                gdf["geom"] = gdf[geom_col].apply(lambda x: wkb.loads(x, hex=True))
+                gdf["geom"] = gdf[geom_col].apply(lambda x:wkb.loads(bytes(x.data)) if isinstance(x, WKBElement) else wkb.loads(x, hex=True))
             else:
                 gdf["geom"] = gdf[geom_col].apply(lambda x: wkt.loads(str(x)))
             if geom_col != "geom":
                 gdf = gdf.drop(geom_col, axis=1)
             gdf = gdf.set_geometry("geom")
             if srid != 0:
                 gdf.crs = srid
             return gdf
         else:
             return gpd.GeoDataFrame()
 
-    def table_to_gdf(self, tbl: Union[Table, str], geom_col="geom", limit=-1):
+    def table_to_gdf(self, tbl: Union[Table, str], geom_col_name="geom", limit=-1):
         if isinstance(tbl, str):
             tbl = self.get_sqlalchemy_table(tbl)
-        # geom_cols = self.get_geometry_cols(tbl)
+        geom_cols = self.get_geometry_cols(tbl)
         # data = self.get_all_data(tbl, limit)
-        query = Select(tbl).query()
+        query = Select(tbl)
         data = self.get_query_data(query)
-        # geom_col = geom_cols[0]
+        geom_col = geom_cols[0]
         srid = self.get_geom_col_srid(tbl, geom_col)
-        return self.data_to_gdf(data, geom_col, srid)
+        # geom_col_name = geom_col.name
+        return self.data_to_gdf(data, geom_col_name, srid)
 
     def execute_query_as_gdf(self, query, srid, geom_col='geom', is_wkb=True):
         data = self.get_query_data(query)
         # if data and len(data) > 0:
         return self.data_to_gdf(data, geom_col, srid, is_wkb)
```

### Comparing `digitalarztools-0.1.8/digitalarztools/adapters/model_utils.py` & `digitalarztools-0.1.9/digitalarztools/adapters/model_utils.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/distributions/GumbleDistribution.py` & `digitalarztools-0.1.9/digitalarztools/distributions/GumbleDistribution.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/datasets/rio_landsat.py` & `digitalarztools-0.1.9/digitalarztools/io/datasets/rio_landsat.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/datasets/rio_probav_viirs.py` & `digitalarztools-0.1.9/digitalarztools/io/datasets/rio_probav_viirs.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/file_io.py` & `digitalarztools-0.1.9/digitalarztools/io/file_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,7 +218,11 @@
         elif sfp[-1] == "zip":
             output_folder = cls.extract_zip_file(fp)
         if output_folder is None:
             da_logger.info(f"No tool available for extracting extension {sfp[-1]}")
         else:
             da_logger.info(f"{os.path.basename(fp)} is unzipped extracted successfully")
         return output_folder
+
+    @classmethod
+    def mvFile(cls, source_path, destination_folder):
+        shutil.move(source_path, destination_folder)
```

### Comparing `digitalarztools-0.1.8/digitalarztools/io/image_io.py` & `digitalarztools-0.1.9/digitalarztools/io/image_io.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/raster/band_process.py` & `digitalarztools-0.1.9/digitalarztools/io/raster/band_process.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/raster/cog_raster.py` & `digitalarztools-0.1.9/digitalarztools/io/raster/cog_raster.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/raster/gdal_raster.py` & `digitalarztools-0.1.9/digitalarztools/io/raster/gdal_raster.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/raster/gdal_raster_io.py` & `digitalarztools-0.1.9/digitalarztools/io/raster/gdal_raster_io.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/raster/hdf_reader.py` & `digitalarztools-0.1.9/digitalarztools/io/raster/hdf_reader.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/raster/indices.py` & `digitalarztools-0.1.9/digitalarztools/io/raster/indices.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/raster/opencv/segmentation.py` & `digitalarztools-0.1.9/digitalarztools/io/raster/opencv/segmentation.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/raster/rio_extraction.py` & `digitalarztools-0.1.9/digitalarztools/io/raster/rio_extraction.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/raster/rio_process.py` & `digitalarztools-0.1.9/digitalarztools/io/raster/rio_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,27 @@
     def __init__(self):
         pass
 
     @staticmethod
     def mosaic_images(img_folder: str) -> RioRaster:
         ds_files: [DatasetReader]
         path = Path(img_folder)
+        issues_folder = os.path.join(img_folder, "issue_in_files")
+        FileIO.mkdirs(issues_folder)
         # test = [str(p) for p in path.iterdir() if p.suffix == ".tif"]
-        ds_files = [RioRaster(str(p)).get_dataset() for p in path.iterdir() if p.suffix == ".tif"]
+        ds_files = []
+        for p in path.iterdir():
+            if p.suffix == ".tif":
+                try:
+                    ds_files.append(RioRaster(str(p)).get_dataset())
+                except Exception as e:
+                    print(str(e))
+                    FileIO.mvFile(str(p), issues_folder)
+                    # problem_files.append(str(p))
+
         mosaic, out_trans = merge(ds_files)
         crs = ds_files[0].crs
         raster = RioRaster.raster_from_array(mosaic, crs=crs, g_transform=out_trans)
         return raster
 
     @staticmethod
     def classify_ndwi(rio_raster, band=8) -> np.ndarray:
```

### Comparing `digitalarztools-0.1.8/digitalarztools/io/raster/rio_raster.py` & `digitalarztools-0.1.9/digitalarztools/io/raster/rio_raster.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/url_io.py` & `digitalarztools-0.1.9/digitalarztools/io/url_io.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/io/vector/gpd_vector.py` & `digitalarztools-0.1.9/digitalarztools/io/vector/gpd_vector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import math
 import os.path
 import traceback
+from typing import List, Dict
 
 import fiona
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import shapely
 from pyproj import CRS
@@ -19,30 +20,46 @@
 from digitalarztools.utils.logger import da_logger
 
 
 class GPDVector(gpd.GeoDataFrame):
     # gdf: gpd.GeoDataFrame
     orig_crs: CRS
 
-    def __init__(self, gdf: gpd.GeoDataFrame):
+    def __init__(self, gdf: gpd.GeoDataFrame = None):
+        if gdf is None:
+            gdf = gpd.GeoDataFrame()
         super().__init__(gdf)
         self.orig_crs = self.crs if hasattr(self, 'crs') else None
 
     @classmethod
     def from_kml(cls, fp):
         fiona.drvsupport.supported_drivers['KML'] = 'rw'
         gdf = gpd.read_file(fp, driver='KML')
         return cls(gdf)
 
     @property
     def extent(self):
         return self.total_bounds
 
     @classmethod
-    def from_xy(cls, src, sheet_name='Sheet1', x_col='X', y_col='Y', crs='epsg:4326') -> 'GPDVector':
+    def from_xy(cls, data: List[Dict], x_col='X', y_col='Y', crs='epsg:4326') -> 'GPDVector':
+        """
+        create GeoDataFrame from xy value in the data
+        :param data: array of dict
+        :param x_col:
+        :param y_col:
+        :param crs:
+        :return: GPDVector
+        """
+        df = pd.DataFrame(data)
+        gdf = gpd.GeoDataFrame(df, geometry=gpd.points_from_xy(df['centerLon'], df['centerLat']), crs='EPSG:4326')
+        return cls(gdf)
+
+    @classmethod
+    def from_excel_xy(cls, src, sheet_name='Sheet1', x_col='X', y_col='Y', crs='epsg:4326') -> 'GPDVector':
         """
         Create GeoDataFrame from xy value in an excel file
         :param src:
         :param sheet_name:
         :param x_col:
         :param y_col:
         :param crs:
@@ -140,33 +157,36 @@
 
         mode = mode if os.path.exists(des) else 'w'
         sheet_exists = 'replace' if os.path.exists(des) else None
         with pd.ExcelWriter(des, engine="openpyxl", mode=mode, if_sheet_exists=sheet_exists) as writer:
             self.to_gdf().to_excel(writer, sheet_name=sheet_name, index_label="id")
             da_logger.info(f"Excel file successfully created at {des}")
 
-    def to_file(self, des):
-        self.to_gdf().to_file(des)
+    # def to_file(self, des, driver=):
+    #     self.to_gdf().to_file(des)
+
+    def to_4326(self) -> 'GPDVector':
+        if str(self.crs) != "EPSG:4326":
+            aoi = GPDVector(self.get_gdf().to_crs(epsg=4326))
+            return GPDVector(aoi)
+        return self
 
     def get_srs(self) -> str:
         return self.crs.srs
 
     def get_crs(self):
         return self.crs
 
-    def to_crs(self, crs=None, epsg=None):
+    def to_crs(self, crs=None, epsg=None) -> 'GPDVector':
         """
         :param crs:
         :param epsg:
         :return:
         """
-        if crs is not None:
-            self = self.to_crs(crs)
-        if epsg is not None:
-            self = self.to_crs(epsg=epsg)
+        return GPDVector(self.get_gdf().to_crs(crs=crs, epsg=epsg))
 
     def to_raster(self, res, value_col='id') -> 'RioRaster':
         # out_arr = np.zeros((rows,cols))
         # shapes = ((geom, value) for geom, value in zip(self.geometry, self[value_col]))
         # rasterize(shapes=shapes, fill=0, out=out_arr, transform=out.transform)
         extent = tuple(self.get_extent())
         out_shape = (math.ceil((extent[2] - extent[0]) / res), math.ceil((extent[3] - extent[1]) / res))
@@ -252,32 +272,35 @@
         if attr_name:
             # return [(row['geometry'], row[attr_name]) for index, row in self.iterrows()]
             return list(zip(self['geometry'], self[attr_name]))
         else:
             return self.geometry.tolist()
 
     def spatial_operation(self, gdf: gpd.GeoDataFrame):
+        intersects_result = self.is_intersects(gdf)
+        self.__init__(self[intersects_result])
+
+    def is_intersects(self, gdf: gpd.GeoDataFrame):
         if str(self.crs) != str(gdf.crs):
             gdf.to_crs(self.crs)
-        intersects_result = self.intersects(gdf)
-        self.__init__(self[intersects_result])
+        return self.intersects(gdf)
 
     def spatial_join(self, input_gdf: gpd.GeoDataFrame, predicate='intersects', how="inner") -> 'GPDVector':
         # inp, res = self.geometry.sindex.query_bulk(input_gdf.geometry, predicate=predicate)
         # res_df = pd.DataFrame({
         #     'self_index': res,
         #     'inp_index': inp
         # })
         # return res_df
         if str(input_gdf.crs) != str(self.get_crs()):
             input_gdf = input_gdf.to_crs(self.get_crs())
         join_result = self.sjoin(input_gdf, how="inner", predicate=predicate)
         return GPDVector(join_result)
 
-    def to_goejson(self, fp: str = None):
+    def to_geojson(self, fp: str = None):
         # gdf = self.dropna()
         gdf_json = self.to_gdf(inplace=False)
         # convert date column to string column
         for col in gdf_json.columns:
             if pd.api.types.is_datetime64_any_dtype(gdf_json[col]):
                 gdf_json[col] = gdf_json[col].dt.strftime('%Y-%m-%d %H:%M:%S')
 
@@ -384,7 +407,21 @@
     def clip_data(self, gdf: gpd.GeoDataFrame) -> 'GPDVector':
         if str(gdf.crs) != str(self.crs):
             gdf.to_crs(self.crs, inplace=True)
         new_gdf = self.clip(gdf, False)
         # new_gdf.set_geometry(gdf.geometry)
         # new_gdf.crs = gdf.crs
         return GPDVector(new_gdf)
+
+    """"
+        Spatial operation
+    """
+
+    def within_aoi(self, aoi: 'GPDVector') -> 'GPDVector':
+        if str(self.crs).lower() != str(aoi.crs).lower():
+            aoi = aoi.get_gdf().to_crs(self.crs)
+        else:
+            aoi = aoi.get_gdf()
+        aoi_polygon = aoi.unary_union
+
+        gdf_within_aoi = self[self.geometry.within(aoi_polygon)]
+        return GPDVector(gdf_within_aoi)
```

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/alos_palser.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/alos_palser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 ### https://search.asf.alaska.edu/
 import os.path
+import traceback
 from multiprocessing import Pool
-
+from urllib.parse import urlencode
 import geopandas as gpd
 import asf_search as asf
+
 from datetime import date
 
 import numpy as np
+import pandas as pd
+import requests
 from dateutil.relativedelta import relativedelta
+from shapely import Polygon
 from tqdm import tqdm
 
 # from tqdm import tqdm
 
 from digitalarztools.io.file_io import FileIO
 from digitalarztools.io.raster.rio_process import RioProcess
 from digitalarztools.io.raster.rio_raster import RioRaster
@@ -42,14 +47,16 @@
     def download_alos_palsar(cls, aoi: GPDVector, aoi_name: str, aoi_buffer: int) -> RioRaster:
         """
         :param aoi:  area of interest as GPDVector
         :param aoi_name: name of the area of interest
         :param aoi_buffer: buffer size in meter for cliping
         :return: DEM as RioRaster
         """
+        EARTHSAT_USER = ""
+        EARTHSAT_PASSWORD = ""
         MEDIA_DIR = os.path.join(os.path.dirname(__file__), '../media')
         output_path = os.path.join(MEDIA_DIR, 'alos_palsar_data')
 
         img_des = os.path.join(output_path, f"alos_dem_{aoi_name.lower().replace(' ', '_')}.tif")
         gpkg_file = os.path.join(output_path, f'aoi_{aoi_name}.gpkg')
         if not os.path.exists(output_path):
             os.makedirs(output_path)
@@ -92,40 +99,86 @@
                 da_logger.error(f"error:{fp}")
 
         rio_raster = RioProcess.mosaic_images(extracted_folder)
         FileIO.delete_folder(extracted_folder)
         return rio_raster
 
     @classmethod
-    def get_dem_urls(cls, aoi, gpkg_file):
-        if not os.path.exists(gpkg_file):
+    def get_dem_urls(cls, aoi:GPDVector, gpkg_fp: str, layer='alos_palsar_dem') -> gpd.GeoDataFrame:
+        if not os.path.exists(gpkg_fp):
+            dir_name = FileIO.mkdirs(gpkg_fp)
+            aoi = aoi.to_4326()
             da_logger.debug("Searching for ALOS Palsar data")
-            start_date, end_date = cls.get_date_range(18)
-            geom = aoi.get_unary_union()
-            options = {
-                'intersectsWith': geom.wkt,
-                'platform': 'ALOS',
-                'instrument': 'PALSAR',
-                'processingLevel': [
-                    # 'RTC_LOW_RES',
-                    'RTC_HI_RES'
-                ],
-                # 'flightDirection': 'Descending',
-                # 'maxResults': 250
-                # 'start': start_date,
-                # 'end': end_date
+            # start_date, end_date = cls.get_date_range(18)
+            # geom : Polygon = aoi.get_unary_union()
+            # geom = geom.envelope
+            # search_params = {
+            #     'intersectsWith': geom.wkt,
+            #     'platform':"SRTM",  #'ALOS', "SRTM",
+            #     # 'instrument': asf.PALSAR, #'PALSAR',
+            #     "output": "json"
+            #     # 'processingLevel': [
+            #     #     'RTC_LOW_RES',
+            #     #     'RTC_HI_RES'
+            #     # ],
+            #     # 'flightDirection': 'Descending',
+            #     # 'maxResults': 250
+            #     # 'start': start_date,
+            #     # 'end': end_date
+            # }
+
+
+            # Set up the ASF Geospatial Search API URL
+            api_url = "https://api.daac.asf.alaska.edu/services/search/param"
+            # Define a bounding box for the KSA region (adjust coordinates as needed)
+            # bounding_box = [34.4959, 35.9402, 38.4110, 39.1201]  # [min_lon, min_lat, max_lon, max_lat]
+            bounding_box = aoi.total_bounds
+            # Set the search parameters for the specified bounding box and ALOS PALSAR DEM
+            search_params = {
+                "bbox": ",".join(map(str, bounding_box)),
+                "platform": "ALOS",
+                "processingLevel": "L1.5",
+                "beamMode": "FBS",
+                "output": "json"
             }
-            results = asf.geo_search(**options)
-            res_gdf = gpd.read_file(str(results), driver='GeoJSON')
-            # getting latest datasets
-            res_gdf = res_gdf.sort_values('startTime', ascending=False).drop_duplicates(['geometry'])
-            res_gdf.drop_duplicates()
-            # res_df['startTime'] = res_df['startTime'].apply(lambda a: pd.to_datetime(a).date())
-            # res_df['stopTime'] = res_df['stopTime'].apply(lambda a: pd.to_datetime(a).date())
 
-            da_logger.info('total tiles:', res_gdf.shape)
+            full_url = f"{api_url}?{urlencode(search_params)}"
+            # results = asf.geo_search(**search_params)
+            try:
+                # Make a GET request to the ASF Geospatial Search API
+                response = requests.get(full_url)
+                response.raise_for_status()
+
+                # Parse the JSON response
+                data = response.json()
+
+                # Check if any scenes were found
+                if len(data) == 0:
+                    print("No ALOS PALSAR DEM data found for the specified region in KSA.")
+                    return
+                # res_gdf = gpd.read_file(str(data), driver='GeoJSON')
+                # res_gdf = gpd.GeoDataFrame(data[0])
+                res_gdv = GPDVector.from_xy(data[0],x_col='centerLon', y_col='centerLat')
+                if not res_gdv.empty:
+                    res_gdv = res_gdv.within_aoi(aoi)
+                    # res_gdf = res_gdf.sort_values('startTime', ascending=False).drop_duplicates(['geometry'])
+                    # res_gdf.drop_duplicates()
+                    # res_df['startTime'] = res_df['startTime'].apply(lambda a: pd.to_datetime(a).date())
+                    # res_df['stopTime'] = res_df['stopTime'].apply(lambda a: pd.to_datetime(a).date())
+                    res_gdf = res_gdv.drop_duplicates()
+                    da_logger.info('total tiles:', res_gdv.shape)
+
+                    # res_df.to_excel(os.path.join(output_path, 'search_result.xlsx'))
+                    res_gdf.to_file(gpkg_fp, layer=layer, driver="GPKG")
+                else:
+                    da_logger.info("no data found within aoi")
+
+            except requests.exceptions.RequestException as e:
+                da_logger.error(f"Error: {e}")
+                traceback.print_stack()
+
 
-            # res_df.to_excel(os.path.join(output_path, 'search_result.xlsx'))
-            res_gdf.to_file(gpkg_file, layer='alos_palsar_rtc_hi_res', driver="GPKG")
+            # getting latest datasets
         else:
-            res_gdf = gpd.read_file(gpkg_file, layer='alos_palsar_rtc_hi_res', driver="GPKG")
-        return list(res_gdf['url'].values)
+            res_gdf = gpd.read_file(gpkg_fp, layer=layer, driver="GPKG")
+        # return list(res_gdf['url'].values)
+        return res_gdf
```

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/config/data_centers.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/config/data_centers.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/earth_explorer/landsat.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/earth_explorer/landsat.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/earth_explorer/m2m.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/earth_explorer/m2m.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/fao_livestock.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/fao_livestock.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/gee/analysis/indices.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/gee/analysis/indices.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/auth.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/auth.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/feature_collection.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/feature_collection.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/gee_api.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/gee_api.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/gee_map.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/gee_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import webbrowser
 
 import ee
+from folium import Map
+
 # from geemap.foliumap import Map
 
 from digitalarztools.pipelines.gee.core.region import GEERegion
 
 
 class GEEMap():
     def __init__(self, region: GEERegion):
         center = region.center.getInfo()
         coordinates = center['coordinates']
         loc = [coordinates[1], coordinates[0]]
-        # self.Map = Map(location=loc, zoom_start=11)
-        # self.Map.addLayerControl()
-        # self.Map.add_minimap()
+        self.Map = Map(location=loc, zoom_start=11)
+        self.Map.addLayerControl()
+        self.Map.add_minimap()
         # self.map.add
 
     def save_map(self):
         self.Map.save("../templates/map.html")
 
     def show(self):
         self.save_map()
```

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/image.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 import os
 import shutil
+import time
 import traceback
 
 import ee
 import numpy as np
+import pandas as pd
 from ee.batch import Export
 
 from digitalarztools.io.file_io import FileIO
+from digitalarztools.io.raster.rio_process import RioProcess
 from digitalarztools.io.url_io import UrlIO
+from digitalarztools.io.vector.gpd_vector import GPDVector
 from digitalarztools.pipelines.gee.core.region import GEERegion
-from digitalarztools.raster.rio_process import RioProcess
+from tqdm import tqdm
 
 
 class GEEImage:
     image: ee.Image
 
     def __init__(self, img: ee.Image):
         self.image = img
+        # self.bands = self.get_image_bands()
+        self.bands = None
 
     @classmethod
-    def get_image_by_tag(cls, tag: str)->'GEEImage':
+    def get_image_by_tag(cls, tag: str) -> 'GEEImage':
         img = ee.Image(tag)
         return cls(img)
 
     def get_gee_image(self) -> ee.Image:
         return self.image
 
-    def get_band(self, band_name, in_place = False) -> 'GEEImage':
+    def get_band(self, band_name, in_place=False) -> 'GEEImage':
         # nir = self.image.select('B5')
         if in_place:
             self.image = self.image.select(band_name)
         else:
             return GEEImage(self.image.select(band_name))
 
     def get_image_bands(self):
@@ -114,65 +120,73 @@
         }
         return res
 
     def get_url_template(self, vis_params):
         map_id_dict = self.image.getMapId(vis_params)
         return map_id_dict['tile_fetcher'].url_format
 
-    def get_download_url(self, img_name, aoi: ee.Geometry.Polygon, out_bands=None, scale=None):
-        if not out_bands:
-            out_bands = self.get_image_bands()
+    def get_download_url(self, img_name, aoi: ee.Geometry.Polygon, scale=None):
+        if not self.bands:
+            self.bands = self.get_image_bands()
         url = self.image.getDownloadURL({
             'image': self.image.serialize(),
             'region': aoi,
-            'bands': out_bands,
+            'bands': self.bands,
             'name': img_name,
             'scale': scale,
             'format': 'GEO_TIFF'
         })
+        # print(url)
         return url
 
     def download_image(self, file_path, img_region: GEERegion, scale=30,
-                       bands=None, bit_depth=32):
-        if not bands:
-            bands = self.get_image_bands()
+                       bit_depth=32, no_of_bands=None):
 
+        if no_of_bands is None:
+            self.bands = self.get_image_bands()
+            no_of_bands = len(self.bands)
+        print("downloading images...")
         dir_name = os.path.dirname(file_path)
         img_name, img_ext = FileIO.get_file_name_ext(os.path.basename(file_path))
         download_dir_name = os.path.join(dir_name, img_name)
-        FileIO.mkdirs(download_dir_name)
-        # final_file_name = os.path.join(dir_name, f'{img_name}.tif')
-        # if not os.path.exists(download_dir_name):
-        #     os.makedirs(download_dir_name)
-        # regions = img_region.get_tiles(len(bands), scale,bit_depth=32)
-        # print("regions", regions)
-        # print("downloading", index)
-        # for region, index in regions:
-        # region = img_region
-        for region, index in img_region.get_tiles(len(bands), scale, bit_depth=bit_depth):
-            print(region, index)
-            aoi = region.get_aoi()
-            # print("aoi", aoi)
-            url = self.get_download_url(img_name, aoi=aoi, scale=scale, out_bands=bands)
-            # downloaded_obj = requests.get(url, allow_redirects=True)
-            # # index = [1, 1]
+        dirname = FileIO.mkdirs(download_dir_name)
+
+        required_tiles = []
+
+        for region, index in img_region.get_tiles(no_of_bands, scale, bit_depth=bit_depth):
+            required_tiles.append((region, index))
+            # print(region, index)
+        # df = pd.DataFrame(required_tiles)
+        # Create a tqdm progress bar for the loop
+        progress_bar = tqdm(desc="Processing Tiles", unit="tile", total=len(required_tiles))
+
+        for i, (region, index) in enumerate(required_tiles):
             temp_file_path = os.path.join(download_dir_name, f"r{index[0]}c{index[1]}.tif")
-            # # print("file_path", file_path)
-            # with open(file_path, "wb") as file:
-            #     file.write(downloaded_obj.content)
-            res = UrlIO.download_url(url, temp_file_path)
-        if res:
-            try:
-                raster = RioProcess.mosaic_images(download_dir_name)
-                raster.save_to_file(file_path)
-                shutil.rmtree(download_dir_name)
-                print('Image downloaded as ', file_path)
-            except:
-                traceback.print_exc()
-                res = False
+            if not os.path.exists(temp_file_path):
+                aoi = region.get_aoi()
+                url = self.get_download_url(img_name, aoi=aoi, scale=scale)
+
+                res = UrlIO.download_url(url, temp_file_path)
+            # Simulate some processing time
+            # time.sleep(0.1)
+
+            # Update the tqdm progress bar
+            progress_bar.update(1)
+        # Close the tqdm progress bar
+        progress_bar.close()
+        res = False
+        try:
+            raster = RioProcess.mosaic_images(download_dir_name)
+            raster.save_to_file(file_path)
+            # FileIO.delete_folder(download_dir_name)
+            print('Image downloaded as ', file_path)
+            res = True
+        except:
+            traceback.print_exc()
+            res = False
         return res
 
     def gee_image_2_numpy(self, image, aoi: ee.Geometry.Polygon):
         if image.args:
             # aoi = ee.Geometry.Polygon(
             #     [[[-110.82, 44.72],
             #       [-110.82, 44.71],
@@ -227,7 +241,20 @@
         res.start()
         while res.status()['state'] not in ['FAILED', 'COMPLETED']:
             print(res.status())
         res_status = res.status()
         if res_status['state'] == 'FAILED':
             print("error:", res_status['error_message'])
         return res_status
+
+    def get_histogram_data(self, band_name, aoi_sub: ee.Geometry.Polygon):
+        data = self.image.select(band_name).reduceRegion(
+            ee.Reducer.fixedHistogram(0, 0.5, 500), aoi_sub).get(band_name).getInfo()
+        return data
+
+    def get_statistic(self, band_name, aoi_sub: ee.Geometry.Polygon):
+        mean = self.image.select(band_name).reduceRegion(
+            ee.Reducer.mean(), aoi_sub).get(band_name).getInfo()
+        variance = self.image.select(band_name).reduceRegion(
+            ee.Reducer.variance(), aoi_sub).get(band_name).getInfo()
+
+        return mean, variance
```

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/gee/core/region.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/gee/core/region.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,45 @@
 import math
 from typing import Union
-
 import ee
-from shapely.geometry import box, mapping
+from shapely.geometry import box, mapping, shape
+import geopandas as gpd
 
+from digitalarztools.io.vector.gpd_vector import GPDVector
 from digitalarztools.pipelines.gee.core.feature_collection import GEEFeatureCollection
 
 
 class GEERegion:
     fc: ee.FeatureCollection = None
     aoi: ee.Geometry.Polygon = None
+    aoi_gdv: GPDVector = None
     bounds: ee.Geometry.Polygon = None
     center: ee.Geometry.Point = None
+    extent: list = None
     vis_params: dict = {'color': 'red'}
 
+    def set_gdv_aoi(self, data: [GPDVector, dict]):
+        if isinstance(data, GPDVector):
+            self.aoi_gdv = data
+        elif isinstance(data, dict):
+            # Extract features from the GeoJSON dictionary
+            self.aoi_gdv = GPDVector.from_geojson(data)
+
+    @classmethod
+    def from_gdv(cls, aoi: GPDVector):
+        if str(aoi.get_crs()).upper() != "EPSG:4326":
+            aoi = aoi.get_gdf().to_crs(epsg=4326)
+        polygon = aoi.unary_union
+        gdf = gpd.GeoDataFrame(geometry=[polygon], crs=aoi.crs)
+        aoi = GPDVector(gdf)
+        geojson = aoi.to_geojson()
+        region = GEERegion.from_geojson(geojson)
+        region.aoi_gdv = aoi
+        return region
+
     @classmethod
     def from_geojson_polygon(cls, polygon, proj='EPSG:4326'):
         region = cls()
         polygon: ee.Geometry.Polygon = ee.Geometry(polygon, opt_proj=proj)
         region.aoi = polygon
         region.set_center()
         region.set_bounds()
@@ -30,14 +52,23 @@
         for feature in fc['features']:
             geom = ee.Geometry(feature["geometry"], opt_proj=proj)
             ee_features.append(ee.Feature(geom, feature['properties']))
         region.fc = ee.FeatureCollection(ee_features)
         region.aoi = region.fc.union().geometry()
         region.set_bounds()
         region.set_center()
+        region.set_gdv_aoi(fc)
+        # Convert GeoJSON to Shapely polygon
+        # shapely_polygon = shape(fc)
+        # region.extent = list(shapely_polygon.bounds)
+        gdf = gpd.GeoDataFrame.from_features(fc["features"])
+        total_bounds = gdf.unary_union.bounds
+
+        region.extent = list(total_bounds)
+
         return region
 
     @classmethod
     def from_feature_collection(cls, fc: Union[GEEFeatureCollection, ee.FeatureCollection]):
         region = cls()
         if isinstance(fc, GEEFeatureCollection):
             fc = fc.get_fc()
@@ -66,17 +97,19 @@
     def set_center(self):
         self.center = self.aoi.centroid()
 
     def set_bounds(self):
         self.bounds = self.aoi.bounds()
 
     def get_extent(self):
-        coordinates = self.bounds.coordinates().getInfo()[0]
-        extent = [coordinates[0][0], coordinates[0][1], coordinates[2][0], coordinates[2][1]]
-        return extent
+        if self.extent is None:
+            coordinates = self.bounds.coordinates().getInfo()[0]
+            self.extent = [coordinates[0][0], coordinates[0][1], coordinates[2][0], coordinates[2][1]]
+        return self.extent
+
         # width = coordinates[2] - coordinates
 
     def get_coordinates(self):
         return self.bounds.coordinates().getInfo()[0]
 
     def get_center_coordinates(self):
         return self.center.coordinates().getInfo()
@@ -98,42 +131,49 @@
     def get_tiles(self, no_of_bands, spatial_res, bit_depth):
         regions = []
         spatial_res_deg = spatial_res / (110 * 1000)
         max_tile_size = 10 * 1024 * 1024  # 10MB
         # img_res = max_tile_size * 8 / ((no_of_bands + 1) * bit_depth)
         tile_res = max_tile_size / ((no_of_bands + 1) * bit_depth)
         # sqr_length = (math.sqrt(tile_res) * spatial_res) / (110 * 1000)
-        tile_length =  math.sqrt(tile_res) * spatial_res_deg
+        tile_length = math.sqrt(tile_res) * spatial_res_deg
         extent = self.get_extent()
         # print("extent", extent)
         # max_width = (extent[2] - extent[0])
         # max_height = (extent[3] - extent[1])
         min_x, min_y = extent[0], extent[1]
         r, c = 0, 0,
         pad = 0.00001
         while extent[3] >= min_y:
             min_x = extent[0]
             max_y = min_y + tile_length
-            max_y = max_y if max_y < extent[3] else extent[3]+pad
+            max_y = max_y if max_y < extent[3] else extent[3] + pad
             r += 1
             c = 0
             while extent[2] >= min_x:
                 max_x = min_x + tile_length
-                max_x = extent[2]+pad if max_x > extent[2] else max_x
+                max_x = extent[2] + pad if max_x > extent[2] else max_x
                 n_extent = [min_x, min_y, max_x, max_y]
                 # print(n_extent)
                 # geometry = box(Polygon.from_bbox)
                 # geojson = json.loads(geometry.json)
                 geometry = box(*n_extent)
-                geojson = mapping(geometry)
+                add_tile = True
+                if self.aoi_gdv is not None:
+                    gdf = gpd.GeoDataFrame(geometry=[geometry], crs='epsg:4326')
+                    add_tile = self.aoi_gdv.is_intersects(gdf).values[0]
+
                 # print(geojson)
-                min_x = max_x
                 c += 1
-                reg = self.from_geojson_polygon(geojson)
-                # regions.append([reg, (r, c)])
-                yield reg, (r, c)
+                if add_tile:
+                    geojson = mapping(geometry)
+                    reg = self.from_geojson_polygon(geojson)
+                    # regions.append([reg, (r, c)])
+                    yield reg, (r, c)
+                min_x = max_x
             min_y = max_y
+        print("total image", r*c)
             # return regions
 
     def __str__(self):
         # return f"extent:{','.join(str(e) for e in self.get_extent())}"
         return str(self.get_extent())
```

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/gee/tags/hydro.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/gee/tags/hydro.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/gee/tags/lulc.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/gee/tags/lulc.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/gee/tags/precipitation.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/gee/tags/soil_moisture.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,25 @@
-from datetime import datetime
-from typing import Union
-
-from digitalarztools.pipelines.gee.core.auth import GEEAuth
 from digitalarztools.pipelines.gee.core.image import GEEImage
 from digitalarztools.pipelines.gee.core.image_collection import GEEImageCollection
-from digitalarztools.pipelines.gee.core.region import GEERegion
 from digitalarztools.utils.logger import da_logger
 
 
-class Precipitation:
-    """
-    Extrat data from different sources
-    """
+class SoilMoisture:
 
     @staticmethod
-    def chirps_data_using_gee(gee_auth: GEEAuth, region: GEERegion, start_date: Union[str, datetime],
-                           end_date: Union[str, datetime], how='mean') -> GEEImage:
+    def smap_data_using_gee(gee_auth, region, start_date, end_date,  how='mean', band="sm_surface") -> GEEImage:
         """
-        Extract CHIRPS data using following code
-        https://developers.google.com/earth-engine/datasets/catalog/UCSB-CHG_CHIRPS_DAILY
-        :param gee_auth: authentiation
-        :param gdv: for define AOI
+        https://developers.google.com/earth-engine/datasets/catalog/NASA_SMAP_SPL4SMGP_007#bands
+         :param gdv: for define AOI
         :param start_date:
         :param end_date:
-          :param how: choices are 'median', 'max', 'mean', 'first', 'cloud_cover'
-        :return:
+          :param how: choices are 'median', 'max', 'mean', 'first', 'cloud_cover',
+        :param band: choices are sm_surface, sm_rootzone,sm_profile etc. see detail in above url
+        :return: GEEImage
         """
-
         if gee_auth.is_initialized:
             date_range = (start_date, end_date)
-            img_collection = GEEImageCollection(region, 'UCSB-CHG/CHIRPS/DAILY', date_range)
-            img_collection.select_dataset('precipitation')
+            img_collection = GEEImageCollection(region, "NASA/SMAP/SPL4SMGP/007", date_range)
+            img_collection.select_dataset(band)
             return GEEImage(img_collection.get_image(how))
         else:
             da_logger.error("Please initialized GEE before further processing")
```

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/gmap/models.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/gmap/models.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/gmap/poi.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/gmap/poi.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/nasa/chirp.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/nasa/chirp.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/nasa/geos.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/nasa/geos.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/nasa/merra.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/nasa/merra.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/nasa/variables_info.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/nasa/variables_info.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/soil_grids/n_van_genuchten.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/soil_grids/n_van_genuchten.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/soil_grids/soil_contents.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/soil_grids/soil_contents.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/soil_grids/theta_fc.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/soil_grids/theta_fc.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/soil_grids/theta_res.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/soil_grids/theta_res.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/pipelines/soil_grids/theta_sat2.py` & `digitalarztools-0.1.9/digitalarztools/pipelines/soil_grids/theta_sat2.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/biomass_analysis.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/biomass_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/clear_sky_radiation.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/clear_sky_radiation.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/constants.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/constants.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/dem_analysis.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/dem_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/emissivity_analysis.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/emissivity_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/et_analysis.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/et_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/leaf_analysis.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/leaf_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/meteo_analysis.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/meteo_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/resistance_analysis.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/resistance_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/roughness_analysis.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/roughness_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/soil_analysis.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/soil_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/soil_moisture.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/soil_moisture.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/solar_radiation.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/solar_radiation.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/temperature_analysis.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/temperature_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/unstable.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/unstable.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/vegitation_analysis.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/vegitation_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/analysis/water_analysis.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/analysis/water_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/energy_blance_model.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/energy_blance_model.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/operations/distance_raster.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/operations/distance_raster.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/operations/transformation.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/operations/transformation.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/propcessing/operations/utils.py` & `digitalarztools-0.1.9/digitalarztools/propcessing/operations/utils.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/test/raster/test_functionalities.py` & `digitalarztools-0.1.9/digitalarztools/test/raster/test_functionalities.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/utils/date_utils.py` & `digitalarztools-0.1.9/digitalarztools/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/utils/logger.py` & `digitalarztools-0.1.9/digitalarztools/utils/logger.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/utils/s3_utils.py` & `digitalarztools-0.1.9/digitalarztools/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools/utils/waitbar_console.py` & `digitalarztools-0.1.9/digitalarztools/utils/waitbar_console.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.1.8/digitalarztools.egg-info/PKG-INFO` & `digitalarztools-0.1.9/digitalarztools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalarztools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Digital Arz tools for applications
 Home-page: UNKNOWN
 Author: Ather Ashraf
 Author-email: atherashraf@gmail.com
 License: UNKNOWN
 Keywords: raster,vector,digitalarz
 Platform: UNKNOWN
```

### Comparing `digitalarztools-0.1.8/digitalarztools.egg-info/SOURCES.txt` & `digitalarztools-0.1.9/digitalarztools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,54 +17,57 @@
 digitalarztools/io/file_io.py
 digitalarztools/io/image_io.py
 digitalarztools/io/url_io.py
 digitalarztools/io/datasets/__init__.py
 digitalarztools/io/datasets/rio_landsat.py
 digitalarztools/io/datasets/rio_modis.py
 digitalarztools/io/datasets/rio_probav_viirs.py
+digitalarztools/io/map/__init__.py
+digitalarztools/io/map/da_folium.py
 digitalarztools/io/raster/__init__.py
 digitalarztools/io/raster/band_process.py
 digitalarztools/io/raster/cog_raster.py
 digitalarztools/io/raster/gdal_raster.py
 digitalarztools/io/raster/gdal_raster_io.py
 digitalarztools/io/raster/hdf_reader.py
 digitalarztools/io/raster/indices.py
 digitalarztools/io/raster/rio_extraction.py
 digitalarztools/io/raster/rio_process.py
 digitalarztools/io/raster/rio_raster.py
 digitalarztools/io/raster/opencv/__init__.py
 digitalarztools/io/raster/opencv/segmentation.py
 digitalarztools/io/vector/__init__.py
 digitalarztools/io/vector/gpd_vector.py
-digitalarztools/io/vector/gpd_vector_old.py
 digitalarztools/pipelines/__init__.py
 digitalarztools/pipelines/alos_palser.py
 digitalarztools/pipelines/fao_livestock.py
 digitalarztools/pipelines/grace.py
 digitalarztools/pipelines/srtm.py
 digitalarztools/pipelines/config/__init__.py
 digitalarztools/pipelines/config/data_centers.py
 digitalarztools/pipelines/earth_explorer/__init__.py
 digitalarztools/pipelines/earth_explorer/landsat.py
 digitalarztools/pipelines/earth_explorer/m2m.py
 digitalarztools/pipelines/gee/__init__.py
 digitalarztools/pipelines/gee/analysis/__init__.py
+digitalarztools/pipelines/gee/analysis/ground_recharge.py
 digitalarztools/pipelines/gee/analysis/indices.py
 digitalarztools/pipelines/gee/core/__init__.py
 digitalarztools/pipelines/gee/core/auth.py
 digitalarztools/pipelines/gee/core/feature_collection.py
 digitalarztools/pipelines/gee/core/gee_api.py
 digitalarztools/pipelines/gee/core/gee_map.py
 digitalarztools/pipelines/gee/core/image.py
 digitalarztools/pipelines/gee/core/image_collection.py
 digitalarztools/pipelines/gee/core/region.py
 digitalarztools/pipelines/gee/tags/__init__.py
 digitalarztools/pipelines/gee/tags/hydro.py
 digitalarztools/pipelines/gee/tags/lulc.py
 digitalarztools/pipelines/gee/tags/precipitation.py
+digitalarztools/pipelines/gee/tags/soil.py
 digitalarztools/pipelines/gee/tags/soil_moisture.py
 digitalarztools/pipelines/gmap/__init__.py
 digitalarztools/pipelines/gmap/models.py
 digitalarztools/pipelines/gmap/poi.py
 digitalarztools/pipelines/gmap/test.py
 digitalarztools/pipelines/nasa/__init__.py
 digitalarztools/pipelines/nasa/chirp.py
```

### Comparing `digitalarztools-0.1.8/digitalarztools.egg-info/requires.txt` & `digitalarztools-0.1.9/digitalarztools.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 affine==2.3.1
 anyio==3.6.2
+asf-search
 attrs==22.1.0
 beautifulsoup4==4.12.2
 bleach==5.0.1
 boto3==1.26.113
-botocore==1.29.113
+botocore
 cachetools==5.3.0
 certifi==2022.9.24
 cffi==1.15.1
 cftime==1.6.2
 charset-normalizer==2.1.1
 click==8.1.3
 click-plugins==1.1.1
@@ -17,14 +18,15 @@
 colorama==0.4.6
 commonmark==0.9.1
 cryptography==41.0.3
 docutils==0.19
 earthengine-api==0.1.369
 et-xmlfile==1.1.0
 Fiona==1.8.22
+folium
 GeoAlchemy2==0.14.1
 geopandas==0.13.2
 google-api-core==2.11.1
 google-api-python-client==2.99.0
 google-auth==2.23.0
 google-auth-httplib2==0.1.1
 google-cloud-core==2.3.3
@@ -75,15 +77,15 @@
 python-dateutil==2.8.2
 python-dotenv==1.0.0
 pytz==2022.6
 PyWavelets==1.4.1
 PyYAML==6.0.1
 rasterio==1.3.4
 readme-renderer==37.3
-requests==2.28.1
+requests
 requests-toolbelt==0.10.1
 rfc3986==2.0.0
 rich==12.6.0
 rio-cogeo==3.5.1
 rio-tiler==4.1.10
 rsa==4.9
 Rtree==1.0.1
```

### Comparing `digitalarztools-0.1.8/setup.py` & `digitalarztools-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
 lib_folder = os.path.dirname(os.path.realpath(__file__))
 requirement_path = os.path.join(lib_folder, 'digitalarztools/requirements.txt') #lib_folder + '/digitalarztools/requirements.txt'
 install_requires = []  # Here we'll get: ["gunicorn", "docutils>=0.3", "lxml==0.5a7"]
 if os.path.isfile(requirement_path):
     with open(requirement_path) as f:
         install_requires = f.read().splitlines()
-
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'Digital Arz tools for applications'
 LONG_DESCRIPTION = 'Package provides tool for developing digitalarz application using rasterio, gdal, geopandas, and pandas'
 
 # Setting up
 setuptools.setup(
     name="digitalarztools",
     version=VERSION,
```

### Comparing `digitalarztools-0.1.8/test/test_raster_io.py` & `digitalarztools-0.1.9/test/test_raster_io.py`

 * *Files identical despite different names*

