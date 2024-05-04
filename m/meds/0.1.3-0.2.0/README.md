# Comparing `tmp/meds-0.1.3.tar.gz` & `tmp/meds-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meds-0.1.3.tar", last modified: Wed Mar 20 19:27:49 2024, max compression
+gzip compressed data, was "meds-0.2.0.tar", last modified: Sat May  4 21:47:23 2024, max compression
```

## Comparing `meds-0.1.3.tar` & `meds-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:27:49.678992 meds-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-20 19:27:44.000000 meds-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-20 19:27:49.678992 meds-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-20 19:27:44.000000 meds-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-20 19:27:44.000000 meds-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 19:27:49.678992 meds-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:27:49.678992 meds-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:27:49.678992 meds-0.1.3/src/meds/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-20 19:27:44.000000 meds-0.1.3/src/meds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:27:44.000000 meds-0.1.3/src/meds/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-03-20 19:27:44.000000 meds-0.1.3/src/meds/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:27:49.678992 meds-0.1.3/src/meds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-20 19:27:49.000000 meds-0.1.3/src/meds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-20 19:27:49.000000 meds-0.1.3/src/meds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 19:27:49.000000 meds-0.1.3/src/meds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-20 19:27:49.000000 meds-0.1.3/src/meds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-20 19:27:49.000000 meds-0.1.3/src/meds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:27:49.678992 meds-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-03-20 19:27:44.000000 meds-0.1.3/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:47:23.344482 meds-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-04 21:47:19.000000 meds-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:47:23.340482 meds-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:47:23.344482 meds-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-04 21:47:19.000000 meds-0.2.0/.github/workflows/meds-etl-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-04 21:47:19.000000 meds-0.2.0/.github/workflows/python-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-04 21:47:19.000000 meds-0.2.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-04 21:47:19.000000 meds-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-04 21:47:19.000000 meds-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-04 21:47:19.000000 meds-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-04 21:47:23.344482 meds-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-04 21:47:19.000000 meds-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-04 21:47:19.000000 meds-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 21:47:23.344482 meds-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:47:23.340482 meds-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:47:23.344482 meds-0.2.0/src/meds/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-04 21:47:19.000000 meds-0.2.0/src/meds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-04 21:47:23.000000 meds-0.2.0/src/meds/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:47:19.000000 meds-0.2.0/src/meds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-04 21:47:19.000000 meds-0.2.0/src/meds/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:47:23.344482 meds-0.2.0/src/meds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-04 21:47:23.000000 meds-0.2.0/src/meds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-04 21:47:23.000000 meds-0.2.0/src/meds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 21:47:23.000000 meds-0.2.0/src/meds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 21:47:23.000000 meds-0.2.0/src/meds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 21:47:23.000000 meds-0.2.0/src/meds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:47:23.344482 meds-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-04 21:47:19.000000 meds-0.2.0/tests/test_schema.py
```

### Comparing `meds-0.1.3/LICENSE` & `meds-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meds-0.1.3/PKG-INFO` & `meds-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 Metadata-Version: 2.1
 Name: meds
-Version: 0.1.3
+Version: 0.2.0
 Summary: A data standard for working with event stream data
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow>=8
-Requires-Dist: jsonschema
+Requires-Dist: jsonschema>=4.0.0
 Requires-Dist: typing_extensions>=4.0
 
 # Medical Event Data Standard
 
 The Medical Event Data Standard (MEDS) is a draft data schema for storing streams of medical events, often sourced from either Electronic Health Records or claims records.
 
 The core of the standard is that we define a ``patient`` data structure that contains a series of time stamped events, that in turn contain measurements of various sorts.
 
 The Python type signature for the schema is as follows:
 
 ```python
 
 Patient = TypedDict('Patient', {
   'patient_id': int,
-  'static_measurements': List[Measurement],
   'events': List[Event],
 })
 
 Event = TypedDict('Event',{
-    'time': datetime.datetime,
-    'measurements': List[Measurement],
-})
-
-Measurement = TypedDict('Measurement', {
+    'time': NotRequired[datetime.datetime],
     'code': str,
     'text_value': NotRequired[str],
     'numeric_value': NotRequired[float],
     'datetime_value': NotRequired[datetime.datetime],
     'metadata': NotRequired[Mapping[str, Any]],
 })
 ```
```

### Comparing `meds-0.1.3/README.md` & `meds-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,19 @@
 
 The Python type signature for the schema is as follows:
 
 ```python
 
 Patient = TypedDict('Patient', {
   'patient_id': int,
-  'static_measurements': List[Measurement],
   'events': List[Event],
 })
 
 Event = TypedDict('Event',{
-    'time': datetime.datetime,
-    'measurements': List[Measurement],
-})
-
-Measurement = TypedDict('Measurement', {
+    'time': NotRequired[datetime.datetime],
     'code': str,
     'text_value': NotRequired[str],
     'numeric_value': NotRequired[float],
     'datetime_value': NotRequired[datetime.datetime],
     'metadata': NotRequired[Mapping[str, Any]],
 })
 ```
```

### Comparing `meds-0.1.3/pyproject.toml` & `meds-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [build-system]
-requires = ["setuptools >= 69.0"]
+requires = ["setuptools >= 69.0", "setuptools-scm>=8.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "meds"
-version = "0.1.3"
+dynamic = ["version"]
 description = "A data standard for working with event stream data"
 readme = "README.md"
 license = {text = "Apache-2.0"}
 
 dependencies = [
     "pyarrow >= 8",
-    "jsonschema",
+    "jsonschema >= 4.0.0",
     "typing_extensions >= 4.0",
 ]
 
+[tool.setuptools_scm]
+version_file = "src/meds/_version.py"
+
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 line_length = 120
```

### Comparing `meds-0.1.3/src/meds/schema.py` & `meds-0.2.0/src/meds/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from typing import Any, List, Mapping
+from typing import Any, List, Mapping, Optional
 
 import pyarrow as pa
 from typing_extensions import NotRequired, TypedDict
 
 # Medical Event Data Standard consists of three main components:
 # 1. A patient data schema
 # 2. A label schema
@@ -17,72 +17,78 @@
 
 # The patient data schema.
 
 # We define some codes for particularly important events
 birth_code = "SNOMED/184099003"
 death_code = "SNOMED/419620001"
 
-
-def patient_schema(per_event_metadata_schema=pa.null()):
+def patient_schema(per_event_properties_schema=pa.null()):
     # Return a patient schema with a particular per event metadata subschema
-    measurement = pa.struct(
+    event = pa.struct(
         [
+            ("time", pa.timestamp("us")), # Static events will have a null timestamp
             ("code", pa.string()),
             ("text_value", pa.string()),
             ("numeric_value", pa.float32()),
             ("datetime_value", pa.timestamp("us")),
-            ("metadata", per_event_metadata_schema),
+            ("properties", per_event_properties_schema),
         ]
     )
 
-    event = pa.struct([("time", pa.timestamp("us")), ("measurements", pa.list_(measurement))])
-
     patient = pa.schema(
         [
             ("patient_id", pa.int64()),
-            ("static_measurements", pa.list_(measurement)),
-            ("events", pa.list_(event)),  # Require ordered by time
+            ("events", pa.list_(event)),  # Require ordered by time, nulls must be first
         ]
     )
 
     return patient
 
 
 # Python types for the above schema
 
-Measurement = TypedDict(
-    "Measurement",
+Event = TypedDict(
+    "Event",
     {
+        "time": NotRequired[datetime.datetime],
         "code": str,
         "text_value": NotRequired[str],
         "numeric_value": NotRequired[float],
         "datetime_value": NotRequired[datetime.datetime],
-        "metadata": NotRequired[Any],
+        "properties": NotRequired[Any],
     },
 )
 
-Event = TypedDict("Event", {"time": datetime.datetime, "measurements": List[Measurement]})
-
-Patient = TypedDict("Patient", {"patient_id": int, "static_measurements": List[Measurement], "events": List[Event]})
+Patient = TypedDict("Patient", {"patient_id": int, "events": List[Event]})
 
 ############################################################
 
 # The label schema.
 
 label = pa.schema(
     [
         ("patient_id", pa.int64()),
         ("prediction_time", pa.timestamp("us")),
         ("boolean_value", pa.bool_()),
+        ("integer_value", pa.int64()),
+        ("float_value", pa.float64()),
+        ("categorical_value", pa.string()),
     ]
 )
 
 # Python types for the above schema
 
-Label = TypedDict("Label", {"patient_id": int, "prediction_time": datetime.datetime, "boolean_value": bool})
+Label = TypedDict("Label", {
+    "patient_id": int, 
+    "prediction_time": datetime.datetime, 
+    "boolean_value": Optional[bool],
+    "integer_value" : Optional[int],
+    "float_value" : Optional[float],
+    "categorical_value" : Optional[str],
+})
 
 ############################################################
 
 # The dataset metadata schema.
 # This is a JSON schema.
 # This data should be stored in metadata.json within the dataset folder.
```

### Comparing `meds-0.1.3/src/meds.egg-info/PKG-INFO` & `meds-0.2.0/src/meds.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 Metadata-Version: 2.1
 Name: meds
-Version: 0.1.3
+Version: 0.2.0
 Summary: A data standard for working with event stream data
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow>=8
-Requires-Dist: jsonschema
+Requires-Dist: jsonschema>=4.0.0
 Requires-Dist: typing_extensions>=4.0
 
 # Medical Event Data Standard
 
 The Medical Event Data Standard (MEDS) is a draft data schema for storing streams of medical events, often sourced from either Electronic Health Records or claims records.
 
 The core of the standard is that we define a ``patient`` data structure that contains a series of time stamped events, that in turn contain measurements of various sorts.
 
 The Python type signature for the schema is as follows:
 
 ```python
 
 Patient = TypedDict('Patient', {
   'patient_id': int,
-  'static_measurements': List[Measurement],
   'events': List[Event],
 })
 
 Event = TypedDict('Event',{
-    'time': datetime.datetime,
-    'measurements': List[Measurement],
-})
-
-Measurement = TypedDict('Measurement', {
+    'time': NotRequired[datetime.datetime],
     'code': str,
     'text_value': NotRequired[str],
     'numeric_value': NotRequired[float],
     'datetime_value': NotRequired[datetime.datetime],
     'metadata': NotRequired[Mapping[str, Any]],
 })
 ```
```

### Comparing `meds-0.1.3/tests/test_schema.py` & `meds-0.2.0/tests/test_schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,30 +11,21 @@
     """
     Test that mock patient data follows the patient_schema schema.
     """
     # Each element in the list is a row in the table
     patient_data = [
         {
             "patient_id": 123,
-            "static_measurements": [{
-                "code": "some_static_code",
-                "text_value": "example",
-                "numeric_value": 1.0,
-                "datetime_value": datetime.datetime(2019, 1, 1, 0, 0, 0),
-                "metadata": None,
-            }],
             "events": [{  # Nested list for events
                 "time": datetime.datetime(2020, 1, 1, 12, 0, 0),
-                "measurements": [{  # Nested list for measurements
-                    "code": "some_code",
-                    "text_value": "Example",
-                    "numeric_value": 10.0,
-                    "datetime_value": datetime.datetime(2020, 1, 1, 12, 0, 0),
-                    "metadata": None
-                }]
+                "code": "some_code",
+                "text_value": "Example",
+                "numeric_value": 10.0,
+                "datetime_value": datetime.datetime(2020, 1, 1, 12, 0, 0),
+                "properties": None
             }]
         }
     ]
 
     patient_table = pa.Table.from_pylist(patient_data, schema=patient_schema())
     assert patient_table.schema.equals(patient_schema()), "Patient schema does not match"
 
@@ -46,15 +37,44 @@
     label_data = [
         {
             "patient_id": 123,
             "prediction_time": datetime.datetime(2020, 1, 1, 12, 0, 0),
             "boolean_value": True
         }
     ]
+    label_table = pa.Table.from_pylist(label_data, schema=label)
+    assert label_table.schema.equals(label), "Label schema does not match"
 
+    label_data = [
+        {
+            "patient_id": 123,
+            "prediction_time": datetime.datetime(2020, 1, 1, 12, 0, 0),
+            "integer_value": 4
+        }
+    ]
+    label_table = pa.Table.from_pylist(label_data, schema=label)
+    assert label_table.schema.equals(label), "Label schema does not match"
+    
+    label_data = [
+        {
+            "patient_id": 123,
+            "prediction_time": datetime.datetime(2020, 1, 1, 12, 0, 0),
+            "float_value": 0.4
+        }
+    ]
+    label_table = pa.Table.from_pylist(label_data, schema=label)
+    assert label_table.schema.equals(label), "Label schema does not match"
+    
+    label_data = [
+        {
+            "patient_id": 123,
+            "prediction_time": datetime.datetime(2020, 1, 1, 12, 0, 0),
+            "categorical_value": "text"
+        }
+    ]
     label_table = pa.Table.from_pylist(label_data, schema=label)
     assert label_table.schema.equals(label), "Label schema does not match"
 
 def test_dataset_metadata_schema():
     """
     Test that mock metadata follows dataset_metadata schema.
     """
```

