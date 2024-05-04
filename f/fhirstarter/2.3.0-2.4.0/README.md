# Comparing `tmp/fhirstarter-2.3.0.tar.gz` & `tmp/fhirstarter-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhirstarter-2.3.0.tar", max compression
+gzip compressed data, was "fhirstarter-2.4.0.tar", max compression
```

## Comparing `fhirstarter-2.3.0.tar` & `fhirstarter-2.4.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1071 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/LICENSE.md
--rw-r--r--   0        0        0     7650 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/README.md
--rw-r--r--   0        0        0      618 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/fhirstarter/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/fhirstarter/examples/__init__.py
--rw-r--r--   0        0        0      151 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/fhirstarter/examples/config.toml
--rw-r--r--   0        0        0     6464 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/fhirstarter/examples/example.py
--rw-r--r--   0        0        0     6289 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/fhirstarter/exceptions.py
--rw-r--r--   0        0        0       92 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/__init__.py
--rw-r--r--   0        0        0    10722 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/scripts/create_sequence_data.py
--rw-r--r--   0        0        0        0 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/__init__.py
--rw-r--r--   0        0        0   392011 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/examples.zip
--rw-r--r--   0        0        0     2814 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json
--rw-r--r--   0        0        0     3334 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/resource_types.json
--rw-r--r--   0        0        0   113904 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip
--rw-r--r--   0        0        0        0 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/__init__.py
--rw-r--r--   0        0        0   397649 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/examples.zip
--rw-r--r--   0        0        0     1800 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json
--rw-r--r--   0        0        0     3081 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/resource_types.json
--rw-r--r--   0        0        0   117431 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip
--rw-r--r--   0        0        0        0 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/__init__.py
--rw-r--r--   0        0        0   436165 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/examples.zip
--rw-r--r--   0        0        0     2356 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json
--rw-r--r--   0        0        0     3526 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/resource_types.json
--rw-r--r--   0        0        0   112399 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip
--rw-r--r--   0        0        0        0 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/__init__.py
--rw-r--r--   0        0        0   361150 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/examples.zip
--rw-r--r--   0        0        0     2624 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json
--rw-r--r--   0        0        0     2416 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/resource_types.json
--rw-r--r--   0        0        0    91155 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip
--rw-r--r--   0        0        0       32 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/__init__.py
--rw-r--r--   0        0        0     4692 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhir_specification/utils.py
--rw-r--r--   0        0        0    22399 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhirstarter.py
--rw-r--r--   0        0        0    20633 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/functions.py
--rw-r--r--   0        0        0     3354 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/interactions.py
--rw-r--r--   0        0        0     3135 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/json_patch.py
--rw-r--r--   0        0        0    10517 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/openapi.py
--rw-r--r--   0        0        0     7222 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/providers.py
--rw-r--r--   0        0        0     1691 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/resources.py
--rw-r--r--   0        0        0     6375 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/search_parameters.py
--rw-r--r--   0        0        0       68 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/testclient.py
--rw-r--r--   0        0        0        0 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/__init__.py
--rw-r--r--   0        0        0     6330 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/config.py
--rw-r--r--   0        0        0     1373 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/conftest.py
--rw-r--r--   0        0        0     1500 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/resources.py
--rw-r--r--   0        0        0     6667 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/test_capability_statement.py
--rw-r--r--   0        0        0     3547 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/test_dependencies.py
--rw-r--r--   0        0        0    10310 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/test_errors.py
--rw-r--r--   0        0        0    14721 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/test_interactions.py
--rw-r--r--   0        0        0    13703 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/test_openapi.py
--rw-r--r--   0        0        0     8906 2024-04-16 16:17:07.316562 fhirstarter-2.3.0/fhirstarter/tests/test_utils.py
--rw-r--r--   0        0        0     2552 2024-04-16 16:17:07.316562 fhirstarter-2.3.0/fhirstarter/tests/utils.py
--rw-r--r--   0        0        0    21217 2024-04-16 16:17:07.316562 fhirstarter-2.3.0/fhirstarter/utils.py
--rw-r--r--   0        0        0     3050 2024-04-16 16:17:07.316562 fhirstarter-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     9714 1970-01-01 00:00:00.000000 fhirstarter-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-04 00:45:28.893719 fhirstarter-2.4.0/LICENSE.md
+-rw-r--r--   0        0        0     7650 2024-05-04 00:45:28.893719 fhirstarter-2.4.0/README.md
+-rw-r--r--   0        0        0      618 2024-05-04 00:45:28.893719 fhirstarter-2.4.0/fhirstarter/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 00:45:28.893719 fhirstarter-2.4.0/fhirstarter/examples/__init__.py
+-rw-r--r--   0        0        0      151 2024-05-04 00:45:28.893719 fhirstarter-2.4.0/fhirstarter/examples/config.toml
+-rw-r--r--   0        0        0     6464 2024-05-04 00:45:28.893719 fhirstarter-2.4.0/fhirstarter/examples/example.py
+-rw-r--r--   0        0        0     6289 2024-05-04 00:45:28.893719 fhirstarter-2.4.0/fhirstarter/exceptions.py
+-rw-r--r--   0        0        0       92 2024-05-04 00:45:28.893719 fhirstarter-2.4.0/fhirstarter/fhir_specification/__init__.py
+-rw-r--r--   0        0        0    10722 2024-05-04 00:45:28.893719 fhirstarter-2.4.0/fhirstarter/fhir_specification/scripts/create_sequence_data.py
+-rw-r--r--   0        0        0        0 2024-05-04 00:45:28.893719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4/__init__.py
+-rw-r--r--   0        0        0   392011 2024-05-04 00:45:28.897719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4/examples.zip
+-rw-r--r--   0        0        0     2814 2024-05-04 00:45:28.897719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json
+-rw-r--r--   0        0        0     3334 2024-05-04 00:45:28.897719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4/resource_types.json
+-rw-r--r--   0        0        0   113904 2024-05-04 00:45:28.897719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip
+-rw-r--r--   0        0        0        0 2024-05-04 00:45:28.897719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4B/__init__.py
+-rw-r--r--   0        0        0   397649 2024-05-04 00:45:28.897719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4B/examples.zip
+-rw-r--r--   0        0        0     1800 2024-05-04 00:45:28.897719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json
+-rw-r--r--   0        0        0     3081 2024-05-04 00:45:28.897719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4B/resource_types.json
+-rw-r--r--   0        0        0   117431 2024-05-04 00:45:28.897719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip
+-rw-r--r--   0        0        0        0 2024-05-04 00:45:28.897719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R5/__init__.py
+-rw-r--r--   0        0        0   436165 2024-05-04 00:45:28.901719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R5/examples.zip
+-rw-r--r--   0        0        0     2356 2024-05-04 00:45:28.901719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json
+-rw-r--r--   0        0        0     3526 2024-05-04 00:45:28.901719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R5/resource_types.json
+-rw-r--r--   0        0        0   112399 2024-05-04 00:45:28.901719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip
+-rw-r--r--   0        0        0        0 2024-05-04 00:45:28.901719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/STU3/__init__.py
+-rw-r--r--   0        0        0   361150 2024-05-04 00:45:28.901719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/STU3/examples.zip
+-rw-r--r--   0        0        0     2624 2024-05-04 00:45:28.901719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json
+-rw-r--r--   0        0        0     2416 2024-05-04 00:45:28.901719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/STU3/resource_types.json
+-rw-r--r--   0        0        0    91155 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip
+-rw-r--r--   0        0        0       32 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/__init__.py
+-rw-r--r--   0        0        0     4714 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/fhir_specification/utils.py
+-rw-r--r--   0        0        0    22399 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/fhirstarter.py
+-rw-r--r--   0        0        0    20633 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/functions.py
+-rw-r--r--   0        0        0     3354 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/interactions.py
+-rw-r--r--   0        0        0     3135 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/json_patch.py
+-rw-r--r--   0        0        0    10517 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/openapi.py
+-rw-r--r--   0        0        0     7222 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/providers.py
+-rw-r--r--   0        0        0     1691 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/resources.py
+-rw-r--r--   0        0        0     6375 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/search_parameters.py
+-rw-r--r--   0        0        0       68 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/testclient.py
+-rw-r--r--   0        0        0        0 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/tests/__init__.py
+-rw-r--r--   0        0        0     6330 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/tests/config.py
+-rw-r--r--   0        0        0     1373 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/tests/conftest.py
+-rw-r--r--   0        0        0     1500 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/tests/resources.py
+-rw-r--r--   0        0        0     6667 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/tests/test_capability_statement.py
+-rw-r--r--   0        0        0     3547 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/tests/test_dependencies.py
+-rw-r--r--   0        0        0    10323 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/tests/test_errors.py
+-rw-r--r--   0        0        0    14721 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/tests/test_interactions.py
+-rw-r--r--   0        0        0    13703 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/tests/test_openapi.py
+-rw-r--r--   0        0        0     8906 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/tests/test_utils.py
+-rw-r--r--   0        0        0     2558 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/tests/utils.py
+-rw-r--r--   0        0        0    21217 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/fhirstarter/utils.py
+-rw-r--r--   0        0        0     3131 2024-05-04 00:45:28.905719 fhirstarter-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9753 1970-01-01 00:00:00.000000 fhirstarter-2.4.0/PKG-INFO
```

### Comparing `fhirstarter-2.3.0/LICENSE.md` & `fhirstarter-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/README.md` & `fhirstarter-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/__init__.py` & `fhirstarter-2.4.0/fhirstarter/__init__.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/examples/example.py` & `fhirstarter-2.4.0/fhirstarter/examples/example.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/exceptions.py` & `fhirstarter-2.4.0/fhirstarter/exceptions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/scripts/create_sequence_data.py` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/scripts/create_sequence_data.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/examples.zip` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4/examples.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/resource_types.json` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4/resource_types.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/examples.zip` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4B/examples.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/resource_types.json` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4B/resource_types.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/examples.zip` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R5/examples.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/resource_types.json` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R5/resource_types.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/examples.zip` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/STU3/examples.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/resource_types.json` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/STU3/resource_types.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/fhir_specification/utils.py` & `fhirstarter-2.4.0/fhirstarter/fhir_specification/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Utilities for working with the FHIR specification."""
 
 import importlib.metadata
-import json
 import os
 import zipfile
 from copy import deepcopy
 from typing import Dict, Set
 
+import orjson
+
 try:
     from functools import cache
 except ImportError:
     from functools import lru_cache as cache
 
 from pathlib import Path
 from typing import Any, Mapping, Union, cast
@@ -66,24 +67,24 @@
     return resource_type in _load_resources_list()
 
 
 @cache
 def _load_resources_list() -> Set[str]:
     """Load the list of resources from the JSON file."""
     with open(FHIR_DIR / "resource_types.json") as file_:
-        return set(json.load(file_))
+        return orjson.loads(file_.read())
 
 
 @cache
 def load_examples(
     resource_type: str,
 ) -> Dict[str, Dict[str, Union[str, Dict[str, Any]]]]:
     """Return the examples for a specific resource type."""
     with zipfile.ZipFile(FHIR_DIR / "examples.zip") as file_:
-        return json.loads(file_.read(f"{resource_type.lower()}.json"))
+        return orjson.loads(file_.read(f"{resource_type.lower()}.json"))
 
 
 def create_bundle_example(resource_example: Mapping[str, Any]) -> Dict[str, Any]:
     """
     Create a bundle example for a specific resource type.
 
     The standard bundle example is modified based on the given resource example.
@@ -130,14 +131,14 @@
         ],
     }
 
 
 def load_search_parameters() -> Dict[str, Any]:
     """Load the search parameters file."""
     with zipfile.ZipFile(FHIR_DIR / "search-parameters.zip") as file_:
-        return json.loads(file_.read("search-parameters.json"))
+        return orjson.loads(file_.read("search-parameters.json"))
 
 
 def load_extra_search_parameters() -> Dict[str, Dict[str, Union[str, bool]]]:
     """Load the extra search parameters file."""
     with open(FHIR_DIR / "extra-search-parameters.json") as file_:
-        return json.load(file_)
+        return orjson.loads(file_.read())
```

### Comparing `fhirstarter-2.3.0/fhirstarter/fhirstarter.py` & `fhirstarter-2.4.0/fhirstarter/fhirstarter.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/functions.py` & `fhirstarter-2.4.0/fhirstarter/functions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/interactions.py` & `fhirstarter-2.4.0/fhirstarter/interactions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/json_patch.py` & `fhirstarter-2.4.0/fhirstarter/json_patch.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/openapi.py` & `fhirstarter-2.4.0/fhirstarter/openapi.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/providers.py` & `fhirstarter-2.4.0/fhirstarter/providers.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/resources.py` & `fhirstarter-2.4.0/fhirstarter/resources.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/search_parameters.py` & `fhirstarter-2.4.0/fhirstarter/search_parameters.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/tests/config.py` & `fhirstarter-2.4.0/fhirstarter/tests/config.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/tests/conftest.py` & `fhirstarter-2.4.0/fhirstarter/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/tests/resources.py` & `fhirstarter-2.4.0/fhirstarter/tests/resources.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/tests/test_capability_statement.py` & `fhirstarter-2.4.0/fhirstarter/tests/test_capability_statement.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/tests/test_dependencies.py` & `fhirstarter-2.4.0/fhirstarter/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/tests/test_errors.py` & `fhirstarter-2.4.0/fhirstarter/tests/test_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Test FHIRStarter error handling"""
 
-import json
 from typing import Any, Callable, Coroutine, Mapping, Union, cast
 
+import orjson
 import pytest
 from fastapi import HTTPException
 
 from ..exceptions import (
     FHIRBadRequestError,
     FHIRConflictError,
     FHIRForbiddenError,
@@ -118,15 +118,15 @@
     request_body: Union[Mapping[str, Any], str],
     response_body: Mapping[str, Any],
 ) -> None:
     """
     Test FHIR create interaction that produces 400 bad request error due to a validation failure.
     """
     if isinstance(request_body, Mapping):
-        request_body = json.dumps(request_body)
+        request_body = orjson.dumps(request_body).decode()
 
     create_response = client.post("/Patient", content=request_body)
 
     assert_expected_response(
         create_response,
         status.HTTP_400_BAD_REQUEST,
         content=response_body,
```

### Comparing `fhirstarter-2.3.0/fhirstarter/tests/test_interactions.py` & `fhirstarter-2.4.0/fhirstarter/tests/test_interactions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/tests/test_openapi.py` & `fhirstarter-2.4.0/fhirstarter/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/tests/test_utils.py` & `fhirstarter-2.4.0/fhirstarter/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/fhirstarter/tests/utils.py` & `fhirstarter-2.4.0/fhirstarter/tests/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Test utilities"""
 
-import json
 from typing import Any, Dict, Mapping, Union
 from urllib.parse import urlparse
 from uuid import uuid4
 
+import orjson
 from funcy import omit
 from requests.models import Response
 
 from .. import Request
 from ..resources import Id
 
 _RESOURCE = {
@@ -39,15 +39,15 @@
 def id_from_location_header(response: Response) -> str:
     """Extract the resource identifier from a FHIR create interaction response."""
     return response.headers["Location"].split("/")[2]
 
 
 def json_dumps_pretty(value: Any) -> str:
     """Dump the value to JSON in pretty format."""
-    return json.dumps(value, indent=2, separators=(", ", ": "))
+    return orjson.dumps(value, option=orjson.OPT_INDENT_2).decode()
 
 
 def make_request(
     method: str,
     path: str,
 ) -> Request:
     """Make a request for the purpose of testing."""
```

### Comparing `fhirstarter-2.3.0/fhirstarter/utils.py` & `fhirstarter-2.4.0/fhirstarter/utils.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.3.0/pyproject.toml` & `fhirstarter-2.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fhirstarter"
-version = "2.3.0"
+version = "2.4.0"
 description = "An ASGI FHIR API framework built on top of FastAPI and FHIR Resources"
 authors = ["Christopher Sande <christopher.sande@canvasmedical.com>"]
 maintainers = ["Canvas Medical Engineering <engineering@canvasmedical.com>"]
 readme = "README.md"
 homepage = "https://github.com/canvas-medical/fhirstarter"
 repository = "https://github.com/canvas-medical/fhirstarter"
 keywords = ["fhir", "api", "server", "resources", "framework", "fastapi", "healthcare", "hl7"]
@@ -32,21 +32,21 @@
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<3.13.0"
-fastapi = ">=0.103.1,<0.111.0"
-"fhir.resources" = ">=6.4.0"
-lxml = ">=4.9.3,<6.0.0"
+fastapi = ">=0.103.1,<0.112.0"
+"fhir.resources" = {version = ">=6.4.0", extras = ["xml"]}
+orjson = "^3.10.3"
 pydantic = ">=1.10.12,<2.0.0"
 python-multipart = ">=0.0.6,<0.0.10"
 tomli = { version = ">=2.0.1,<3.0.0", markers = "python_version < '3.11'" }
-tzdata = ">=2023.3,<2025.0"
+tzdata = { version = ">=2023.3,<2025.0", markers = "platform_system == 'Windows'" }
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.7,<25.0"
 beautifulsoup4 = "^4.12.2"
 funcy = "^2.0"
 httpx = ">=0.24.1,<0.28.0"
 isort = "^5.12.0"
```

### Comparing `fhirstarter-2.3.0/PKG-INFO` & `fhirstarter-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhirstarter
-Version: 2.3.0
+Version: 2.4.0
 Summary: An ASGI FHIR API framework built on top of FastAPI and FHIR Resources
 Home-page: https://github.com/canvas-medical/fhirstarter
 Keywords: fhir,api,server,resources,framework,fastapi,healthcare,hl7
 Author: Christopher Sande
 Author-email: christopher.sande@canvasmedical.com
 Maintainer: Canvas Medical Engineering
 Maintainer-email: engineering@canvasmedical.com
@@ -29,21 +29,21 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: fastapi (>=0.103.1,<0.111.0)
-Requires-Dist: fhir.resources (>=6.4.0)
-Requires-Dist: lxml (>=4.9.3,<6.0.0)
+Requires-Dist: fastapi (>=0.103.1,<0.112.0)
+Requires-Dist: fhir.resources[xml] (>=6.4.0)
+Requires-Dist: orjson (>=3.10.3,<4.0.0)
 Requires-Dist: pydantic (>=1.10.12,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.10)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
-Requires-Dist: tzdata (>=2023.3,<2025.0)
+Requires-Dist: tzdata (>=2023.3,<2025.0) ; platform_system == "Windows"
 Project-URL: Repository, https://github.com/canvas-medical/fhirstarter
 Description-Content-Type: text/markdown
 
 # fhirstarter
 
 <p>
   <a href="https://github.com/canvas-medical/fhirstarter/actions?query=workflow%3Atests+event%3Apush+branch%3Amain" target="_blank">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fhirstarter Version: 2.3.0 Summary: An ASGI FHIR
+Metadata-Version: 2.1 Name: fhirstarter Version: 2.4.0 Summary: An ASGI FHIR
 API framework built on top of FastAPI and FHIR Resources Home-page: https://
 github.com/canvas-medical/fhirstarter Keywords:
 fhir,api,server,resources,framework,fastapi,healthcare,hl7 Author: Christopher
 Sande Author-email: christopher.sande@canvasmedical.com Maintainer: Canvas
 Medical Engineering Maintainer-email: engineering@canvasmedical.com Requires-
 Python: >=3.8.0,<3.13.0 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment Classifier: Framework :: AsyncIO
@@ -16,20 +16,21 @@
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Topic :: Internet Classifier: Topic ::
 Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development Classifier: Topic :: Software
 Development :: Libraries Classifier: Topic :: Software Development :: Libraries
 :: Application Frameworks Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Typing :: Typed Requires-Dist: fastapi
-(>=0.103.1,<0.111.0) Requires-Dist: fhir.resources (>=6.4.0) Requires-Dist:
-lxml (>=4.9.3,<6.0.0) Requires-Dist: pydantic (>=1.10.12,<2.0.0) Requires-Dist:
-python-multipart (>=0.0.6,<0.0.10) Requires-Dist: tomli (>=2.0.1,<3.0.0) ;
-python_version < "3.11" Requires-Dist: tzdata (>=2023.3,<2025.0) Project-URL:
-Repository, https://github.com/canvas-medical/fhirstarter Description-Content-
-Type: text/markdown # fhirstarter
+(>=0.103.1,<0.112.0) Requires-Dist: fhir.resources[xml] (>=6.4.0) Requires-
+Dist: orjson (>=3.10.3,<4.0.0) Requires-Dist: pydantic (>=1.10.12,<2.0.0)
+Requires-Dist: python-multipart (>=0.0.6,<0.0.10) Requires-Dist: tomli
+(>=2.0.1,<3.0.0) ; python_version < "3.11" Requires-Dist: tzdata
+(>=2023.3,<2025.0) ; platform_system == "Windows" Project-URL: Repository,
+https://github.com/canvas-medical/fhirstarter Description-Content-Type: text/
+markdown # fhirstarter
 _[_t_e_s_t_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_f_h_i_r_s_t_a_r_t_e_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/
 _p_y_v_e_r_s_i_o_n_s_/_f_h_i_r_s_t_a_r_t_e_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_f_h_i_r_s_t_a_r_t_e_r_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_]
 An ASGI [FHIR](https://hl7.org/fhir/) API framework built on top of [FastAPI]
 (https://fastapi.tiangolo.com) and [FHIR Resources](https://pypi.org/project/
 fhir.resources/). Supports FHIR sequences: * [STU (v3.0.2)](https://hl7.org/
 fhir/STU3/) * [R4 (v4.0.1)](https://hl7.org/fhir/R4/) * [R4B (v4.3.0)](https://
```

