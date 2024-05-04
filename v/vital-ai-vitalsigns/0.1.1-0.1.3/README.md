# Comparing `tmp/vital-ai-vitalsigns-0.1.1.tar.gz` & `tmp/vital-ai-vitalsigns-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-ai-vitalsigns-0.1.1.tar", last modified: Thu Feb  8 13:01:23 2024, max compression
+gzip compressed data, was "vital-ai-vitalsigns-0.1.3.tar", last modified: Sat May  4 20:41:20 2024, max compression
```

## Comparing `vital-ai-vitalsigns-0.1.1.tar` & `vital-ai-vitalsigns-0.1.3.tar`

### file list

```diff
@@ -1,61 +1,276 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:01:23.080103 vital-ai-vitalsigns-0.1.1/
--rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-02-02 13:30:17.000000 vital-ai-vitalsigns-0.1.1/LICENSE
--rw-r--r--   0 hadfield   (501) staff       (20)      523 2024-02-08 13:01:23.079985 vital-ai-vitalsigns-0.1.1/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)       25 2024-02-02 13:30:17.000000 vital-ai-vitalsigns-0.1.1/README.md
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-02-08 13:01:23.080144 vital-ai-vitalsigns-0.1.1/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      661 2024-02-08 12:56:30.000000 vital-ai-vitalsigns-0.1.1/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:01:23.075131 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 19:32:01.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:01:23.075820 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/impl/
--rw-r--r--   0 hadfield   (501) staff       (20)     1891 2024-02-06 00:26:15.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/impl/VitalSignsImpl.py
--rw-r--r--   0 hadfield   (501) staff       (20)       43 2024-02-05 21:50:01.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/impl/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:01:23.077218 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/
--rw-r--r--   0 hadfield   (501) staff       (20)      293 2024-02-06 23:16:43.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/GraphMatch.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1467 2024-02-06 23:13:18.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/GraphObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      311 2024-02-06 23:19:04.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/KGPropertyMap.py
--rw-r--r--   0 hadfield   (501) staff       (20)      310 2024-02-06 23:18:38.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/ParameterMap.py
--rw-r--r--   0 hadfield   (501) staff       (20)      311 2024-02-06 23:18:21.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/SparqlBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      308 2024-02-06 23:18:03.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/SqlResultRow.py
--rw-r--r--   0 hadfield   (501) staff       (20)      423 2024-02-06 23:17:41.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/VITAL_Edge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      323 2024-02-06 23:17:27.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      428 2024-02-06 23:16:59.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/VITAL_HyperEdge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      428 2024-02-06 23:16:43.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/VITAL_HyperNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      424 2024-02-06 23:15:22.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/VITAL_Node.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:33:45.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:01:23.077539 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/datatype/
--rw-r--r--   0 hadfield   (501) staff       (20)      241 2024-02-06 00:37:03.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/datatype/GeoLocation.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-06 00:32:30.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/datatype/Truth.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-06 00:37:29.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/datatype/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:01:23.078971 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-02-05 21:59:24.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/BooleanProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-02-05 23:03:38.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/DateTimeProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-02-05 22:08:47.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/DoubleProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-02-05 22:09:06.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/FloatProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:25:18.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/GeoLocationProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-02-05 23:00:12.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/IProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-02-05 22:10:09.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/IntegerProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:25:47.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/LongProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:26:00.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/MultiValueProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:26:21.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/OtherProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-02-05 23:02:49.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/StringProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:26:48.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/TruthProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:27:00.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/URIProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:32:18.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/properties/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:01:23.079166 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/trait/
--rw-r--r--   0 hadfield   (501) staff       (20)      715 2024-02-06 00:12:15.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/trait/PropertyTrait.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:55:29.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/trait/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:01:23.075578 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      523 2024-02-08 13:01:23.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)     2172 2024-02-08 13:01:23.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-02-08 13:01:23.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       45 2024-02-08 13:01:23.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns.egg-info/top_level.txt
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:01:23.079252 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns_core/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:32:52.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns_core/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:01:23.079536 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns_core/model/
--rw-r--r--   0 hadfield   (501) staff       (20)      475 2024-02-05 23:26:21.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns_core/model/Person.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:31:01.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns_core/model/VITAL_Event.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:32:34.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns_core/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:01:23.079848 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns_core/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-02-05 22:37:22.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns_core/model/properties/Property_HasBirthday.py
--rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-02-05 22:17:08.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns_core/model/properties/Property_HasName.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 20:32:43.000000 vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns_core/model/properties/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.412769 vital-ai-vitalsigns-0.1.3/
+-rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.3/LICENSE
+-rw-r--r--   0 hadfield   (501) staff       (20)      660 2024-05-04 20:41:20.412534 vital-ai-vitalsigns-0.1.3/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)       25 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.3/README.md
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-04 20:41:20.412815 vital-ai-vitalsigns-0.1.3/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)     1071 2024-05-04 16:07:57.000000 vital-ai-vitalsigns-0.1.3/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.362407 vital-ai-vitalsigns-0.1.3/test/
+-rw-r--r--   0 hadfield   (501) staff       (20)      489 2024-05-02 22:13:47.000000 vital-ai-vitalsigns-0.1.3/test/test_embedding_model.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2119 2024-05-04 19:54:30.000000 vital-ai-vitalsigns-0.1.3/test/test_graph_collection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:51:38.000000 vital-ai-vitalsigns-0.1.3/test/test_package_discovery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2749 2024-05-04 14:15:24.000000 vital-ai-vitalsigns-0.1.3/test/test_query_builder.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.362780 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.364861 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/collection/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:00:36.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/collection/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)    11436 2024-05-04 20:33:20.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/collection/graph_collection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1030 2024-05-03 21:08:09.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/collection/rdf_collection_impl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1640 2024-05-03 21:19:06.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/collection/vector_collection_impl.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.365270 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/embedding/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:22:30.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/embedding/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1172 2024-05-03 15:21:19.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/embedding/embedding_model.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.366354 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/impl/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 18:25:32.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/impl/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2310 2024-05-04 18:20:33.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/impl/vitalsigns_impl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      269 2024-03-19 17:21:02.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/impl/vitalsigns_package.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     5515 2024-05-04 18:49:12.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/impl/vitalsigns_registry.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.369736 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)       47 2024-03-19 21:49:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/BaseDomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     4988 2024-05-04 20:22:24.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/GraphObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1843 2024-05-04 18:11:27.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/VITAL_Edge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      338 2024-03-17 20:11:18.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/VITAL_Edge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1690 2024-05-04 18:13:01.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      310 2024-03-17 20:11:39.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1868 2024-05-04 18:13:13.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/VITAL_HyperEdge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      354 2024-03-17 20:11:44.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/VITAL_HyperEdge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1657 2024-05-04 18:13:26.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/VITAL_HyperNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      298 2024-03-17 20:11:51.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/VITAL_HyperNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1642 2024-05-04 18:11:50.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/VITAL_Node.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      294 2024-03-17 20:11:57.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/VITAL_Node.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.370115 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/classproperties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-03 23:34:11.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/classproperties/ClassProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-03 22:18:04.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/classproperties/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.370800 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/datatype/
+-rw-r--r--   0 hadfield   (501) staff       (20)      241 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/datatype/GeoLocation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       23 2024-05-03 17:43:23.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/datatype/Truth.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/datatype/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.374741 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      492 2024-05-03 20:14:56.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/BooleanProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      603 2024-05-03 20:14:56.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/DateTimeProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      492 2024-05-03 20:22:03.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/DoubleProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      489 2024-05-03 20:22:09.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/FloatProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      552 2024-05-03 20:22:16.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/GeoLocationProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      897 2024-05-03 20:45:02.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/IProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      489 2024-05-03 20:22:27.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/IntegerProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      537 2024-05-03 20:22:27.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/LongProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      355 2024-05-03 20:22:44.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/MultiValueProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      314 2024-05-03 20:23:03.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/OtherProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      543 2024-05-03 20:26:30.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/StringProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      540 2024-05-03 20:26:30.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/TruthProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      537 2024-05-03 20:26:30.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/URIProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/properties/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.375095 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/trait/
+-rw-r--r--   0 hadfield   (501) staff       (20)      715 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/trait/PropertyTrait.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/trait/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.376726 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/query/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:00:23.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/query/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      351 2024-05-03 22:16:06.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/query/property_constraint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      293 2024-05-03 18:45:19.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/query/result_element.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      522 2024-05-03 18:46:27.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/query/result_list.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2456 2024-05-04 14:04:22.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/query/vital_graph_query.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      565 2024-05-04 14:04:22.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/query/vital_query.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      889 2024-05-04 14:12:47.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/query/vital_select_query.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.377166 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/query_impl/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:01:10.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/query_impl/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:02:54.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/query_impl/sparql_query_impl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:03:29.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/query_impl/weaviate_vector_query_impl.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.377384 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/utils/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-02 19:19:42.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/utils/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       30 2024-05-02 19:20:23.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/utils/uri_generator.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      894 2024-05-04 18:08:26.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/vitalsigns.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.363857 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      660 2024-05-04 20:41:20.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)    14057 2024-05-04 20:41:20.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-04 20:41:20.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-04 20:41:20.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns.egg-info/entry_points.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       77 2024-05-04 20:41:20.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       45 2024-05-04 20:41:20.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns.egg-info/top_level.txt
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.377669 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.398214 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)     1476 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/AggregationResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/AggregationResult.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2083 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/DatabaseConnection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      309 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/DatabaseConnection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1551 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Dataset.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      186 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Dataset.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/DomainModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      360 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/DomainModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/DomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1273 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_SameAs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_SameAs.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1285 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasApp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasApp.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1288 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasOrganization.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasOrganization.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasSegment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasSegment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasSession.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasSession.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasTransaction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/Edge_hasTransaction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/GraphMatch.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/GraphMatch.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1664 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/RDFStatement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/RDFStatement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1381 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SparqlAskResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SparqlAskResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SparqlBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SparqlBinding.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1531 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1414 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SqlResultRow.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SqlResultRow.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1382 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SqlUpdateResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/SqlUpdateResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1353 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/URIReference.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/URIReference.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_Category.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_Category.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_Event.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_Event.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1279 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1276 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_PathQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_PathQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1483 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1358 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_Query.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_Query.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1277 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalApp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalApp.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1353 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalAuthKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalAuthKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalOrganization.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalOrganization.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalProvisioning.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalProvisioning.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1458 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalSegment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalSegment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1951 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      305 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2419 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      414 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1540 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1279 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1435 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1342 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1291 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceRootKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceRootKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1923 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      294 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1555 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalSession.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalSession.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1482 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalTransaction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/VitalTransaction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:41:20.412233 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_URIProp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasAggregationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasAppID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasBackwardCompVersion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasCatalogName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasConfigString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasConnectionError.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasConnectionState.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasDatabase.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasDateRetrieved.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasDbType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasDefaultPackageValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasDefaultSegmentName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasDomainOWL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasDomainOWLHash.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasEdgeDestination.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasEdgeSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasEndpointType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasEndpointURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasGraphQueries.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasHyperEdgeDestination.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasHyperEdgeSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasListIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasOntologyIRI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasOrganizationID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasPassword.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasPoolInitialSize.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasPoolMaxTotal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasPreferredImportVersions.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasProvenance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasQueryString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasRdfContext.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasRdfObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasRdfPredicate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasRdfSubject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasRepositoryName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasRootPath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasSegmentID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasSelectQueries.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasSerializedJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasSerializedRDF.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasServerURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasSessionID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasSessionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasSourceName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasSourceUrl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasTargetAppID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasTargetOrganizationID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasTimestamp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasTransactionID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasTransactionState.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasURIRef.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasUpdateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasUpdatedRowsCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasUpdatedTriplesCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasUriGenerationStrategy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasUsername.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasVersionIRI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_hasVersionInfo.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_isActive.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_isPositiveResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_isPreferred.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_isPrimary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_isReadOnly.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_types.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/Property_vitaltype.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns_core/model/properties/__init__.py
```

### Comparing `vital-ai-vitalsigns-0.1.1/LICENSE` & `vital-ai-vitalsigns-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.1/PKG-INFO` & `vital-ai-vitalsigns-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: vital-ai-vitalsigns
-Version: 0.1.1
+Version: 0.1.3
 Summary: VitalSigns knowledge graph bindings
 Home-page: https://github.com/vital-ai/vital-vitalsigns-python
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: sentence_transformers==2.7.0
+Requires-Dist: vectordb==0.0.21
+Requires-Dist: docarray==0.40.0
+Requires-Dist: rdflib==7.0.0
 
 # vital-vitalsigns-python
```

### Comparing `vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/impl/VitalSignsImpl.py` & `vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/impl/vitalsigns_impl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from vital_ai_vitalsigns.model.trait.PropertyTrait import PropertyTrait
 import pkgutil
 import importlib
+# from vital_ai_vitalsigns.model.trait.PropertyTrait import PropertyTrait
+from vital_ai_vitalsigns.vitalsigns import VitalSigns
 
 
 class VitalSignsImpl:
 
+    """
     @staticmethod
     def import_submodules(package_name):
         try:
             package = importlib.import_module(package_name)
             package_path = package.__path__
             for loader, name, is_pkg in pkgutil.walk_packages(path=package_path):
                 full_name = f"{package_name}.{name}"
@@ -17,39 +19,54 @@
                     importlib.import_module(full_name)
                     if is_pkg:
                         VitalSignsImpl.import_submodules(full_name)
                 except ImportError as e:
                     pass  # print(f"Error importing {full_name}: {e}")
         except ImportError as e:
             pass  # print(f"Error importing package {package_name}: {e}")
+
     @staticmethod
     def find_all_subclasses(base_class):
         return base_class.__subclasses__()
+    
+    """
 
-    @staticmethod
-    def create_property_with_trait(property_class, trait_uri, value):
+    @classmethod
+    def create_property_with_trait(cls, property_class, trait_uri, value):
 
-        VitalSignsImpl.import_submodules('vital_ai_vitalsigns_core')
-        VitalSignsImpl.import_submodules('vital_ai_vitalsigns')
+        # VitalSignsImpl.import_submodules('vital_ai_vitalsigns_core')
+        # VitalSignsImpl.import_submodules('vital_ai_vitalsigns')
 
-        trait_classes = [cls for cls in PropertyTrait.__subclasses__() if cls.get_uri() == trait_uri]
+        # trait_classes = [cls for cls in PropertyTrait.__subclasses__() if cls.get_uri() == trait_uri]
 
-        if not trait_classes:
-            raise ValueError(f"No trait found with URI: {trait_uri}")
+        # if not trait_classes:
+        #    raise ValueError(f"No trait found with URI: {trait_uri}")
+
+        # trait_class = trait_classes[0]
+
+        trait_class = cls.get_trait_class_from_uri(trait_uri)
 
-        trait_class = trait_classes[0]
+        if not trait_class:
+            raise ValueError(f"No trait found with URI: {trait_uri}")
 
         class CombinedProperty(property_class, trait_class):
             def get_uri(self):
                 return super().get_uri()
 
         return CombinedProperty(value)
 
-    @staticmethod
-    def get_trait_class_from_uri(uri):
+    @classmethod
+    def get_trait_class_from_uri(cls, uri):
+
+        vs = VitalSigns()
+
+        registry = vs.get_registry()
+
+        trait_cls = registry.vitalsigns_property_classes[uri]
 
-        VitalSignsImpl.import_submodules('vital_ai_vitalsigns_core')
+        return trait_cls
 
-        for subclass in PropertyTrait.__subclasses__():
-            if subclass.get_uri() == uri:
-                return subclass
-        return None
+        # VitalSignsImpl.import_submodules('vital_ai_vitalsigns_core')
+        # for subclass in PropertyTrait.__subclasses__():
+        #   if subclass.get_uri() == uri:
+        #        return subclass
+        # return None
```

### Comparing `vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns/model/trait/PropertyTrait.py` & `vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns/model/trait/PropertyTrait.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.1/vital_ai_vitalsigns.egg-info/PKG-INFO` & `vital-ai-vitalsigns-0.1.3/vital_ai_vitalsigns.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: vital-ai-vitalsigns
-Version: 0.1.1
+Version: 0.1.3
 Summary: VitalSigns knowledge graph bindings
 Home-page: https://github.com/vital-ai/vital-vitalsigns-python
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: sentence_transformers==2.7.0
+Requires-Dist: vectordb==0.0.21
+Requires-Dist: docarray==0.40.0
+Requires-Dist: rdflib==7.0.0
 
 # vital-vitalsigns-python
```

