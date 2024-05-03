# Comparing `tmp/drepr_v2-1.2.1.tar.gz` & `tmp/drepr_v2-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drepr_v2-1.2.1.tar", max compression
+gzip compressed data, was "drepr_v2-1.2.2.tar", max compression
```

## Comparing `drepr_v2-1.2.1.tar` & `drepr_v2-1.2.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1064 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/LICENSE
--rw-r--r--   0        0        0       53 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/README.md
--rw-r--r--   0        0        0        0 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/__init__.py
--rw-r--r--   0        0        0     3754 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/__main__.py
--rw-r--r--   0        0        0        0 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/__init__.py
--rw-r--r--   0        0        0     4710 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/align.py
--rw-r--r--   0        0        0     1263 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/attr.py
--rw-r--r--   0        0        0    18068 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/drepr.py
--rw-r--r--   0        0        0     3416 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/drepr_builder.py
--rw-r--r--   0        0        0       71 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/format.py
--rw-r--r--   0        0        0     8805 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/__init__.py
--rw-r--r--   0        0        0     5815 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/align_parser.py
--rw-r--r--   0        0        0     4494 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/attr_parser.py
--rw-r--r--   0        0        0     5940 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/path_parser.py
--rw-r--r--   0        0        0     5430 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/preprocessing_parser.py
--rw-r--r--   0        0        0     3255 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/resource_parser.py
--rw-r--r--   0        0        0     7107 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/sm_parser.py
--rw-r--r--   0        0        0     9430 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v2/__init__.py
--rw-r--r--   0        0        0    11569 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v2/path_parser.py
--rw-r--r--   0        0        0     9359 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v2/sm_parser.py
--rw-r--r--   0        0        0     6706 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/path.py
--rw-r--r--   0        0        0      326 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/prelude.py
--rw-r--r--   0        0        0     3917 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/preprocessing.py
--rw-r--r--   0        0        0     2005 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/resource.py
--rw-r--r--   0        0        0     9252 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/sm.py
--rw-r--r--   0        0        0        0 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/planning/__init__.py
--rw-r--r--   0        0        0    19789 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/planning/class_map_plan.py
--rw-r--r--   0        0        0    17577 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/planning/drepr_model_alignments.py
--rw-r--r--   0        0        0     4783 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/planning/topological_sorting.py
--rw-r--r--   0        0        0        0 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/__init__.py
--rw-r--r--   0        0        0    17908 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/alignment_fn.py
--rw-r--r--   0        0        0    23969 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/main.py
--rw-r--r--   0        0        0     1569 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/predefined_fn.py
--rw-r--r--   0        0        0    16794 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/preprocessing.py
--rw-r--r--   0        0        0     1458 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/program_space.py
--rw-r--r--   0        0        0     4966 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/writers.py
--rw-r--r--   0        0        0        0 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/readers/__init__.py
--rw-r--r--   0        0        0      157 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/readers/csv.py
--rw-r--r--   0        0        0      160 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/readers/json.py
--rw-r--r--   0        0        0      145 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/readers/prelude.py
--rw-r--r--   0        0        0      382 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/readers/spreadsheet.py
--rw-r--r--   0        0        0       61 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/__init__.py
--rw-r--r--   0        0        0     6400 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/attr_data.py
--rw-r--r--   0        0        0     2960 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/misc.py
--rw-r--r--   0        0        0      828 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/namespace_mixin.py
--rw-r--r--   0        0        0      443 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/safe.py
--rw-r--r--   0        0        0     4341 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/udf.py
--rw-r--r--   0        0        0     7798 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/validator.py
--rw-r--r--   0        0        0        0 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/writers/__init__.py
--rw-r--r--   0        0        0     3850 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/writers/base.py
--rw-r--r--   0        0        0     3627 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/writers/rdfgraph_writer.py
--rw-r--r--   0        0        0      604 2024-04-23 19:55:32.418102 drepr_v2-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 drepr_v2-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/LICENSE
+-rw-r--r--   0        0        0       53 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/__init__.py
+-rw-r--r--   0        0        0     3754 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/__init__.py
+-rw-r--r--   0        0        0     4710 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/align.py
+-rw-r--r--   0        0        0     1263 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/attr.py
+-rw-r--r--   0        0        0    18068 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/drepr.py
+-rw-r--r--   0        0        0     3416 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/drepr_builder.py
+-rw-r--r--   0        0        0       71 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/format.py
+-rw-r--r--   0        0        0     8805 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/parse_v1/__init__.py
+-rw-r--r--   0        0        0     5815 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/parse_v1/align_parser.py
+-rw-r--r--   0        0        0     4520 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/parse_v1/attr_parser.py
+-rw-r--r--   0        0        0     5940 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/parse_v1/path_parser.py
+-rw-r--r--   0        0        0     5430 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/parse_v1/preprocessing_parser.py
+-rw-r--r--   0        0        0     3255 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/parse_v1/resource_parser.py
+-rw-r--r--   0        0        0     7107 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/parse_v1/sm_parser.py
+-rw-r--r--   0        0        0     9430 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/parse_v2/__init__.py
+-rw-r--r--   0        0        0    11569 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/parse_v2/path_parser.py
+-rw-r--r--   0        0        0     9359 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/parse_v2/sm_parser.py
+-rw-r--r--   0        0        0     6706 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/path.py
+-rw-r--r--   0        0        0      326 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/prelude.py
+-rw-r--r--   0        0        0     3917 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/preprocessing.py
+-rw-r--r--   0        0        0     2005 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/resource.py
+-rw-r--r--   0        0        0     9252 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/models/sm.py
+-rw-r--r--   0        0        0        0 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/planning/__init__.py
+-rw-r--r--   0        0        0    19789 2024-05-03 23:13:35.951143 drepr_v2-1.2.2/drepr/planning/class_map_plan.py
+-rw-r--r--   0        0        0    17577 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/planning/drepr_model_alignments.py
+-rw-r--r--   0        0        0     4783 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/planning/topological_sorting.py
+-rw-r--r--   0        0        0        0 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/program_generation/__init__.py
+-rw-r--r--   0        0        0    17908 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/program_generation/alignment_fn.py
+-rw-r--r--   0        0        0    23969 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/program_generation/main.py
+-rw-r--r--   0        0        0     1569 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/program_generation/predefined_fn.py
+-rw-r--r--   0        0        0    16794 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/program_generation/preprocessing.py
+-rw-r--r--   0        0        0     1458 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/program_generation/program_space.py
+-rw-r--r--   0        0        0     4966 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/program_generation/writers.py
+-rw-r--r--   0        0        0        0 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/readers/__init__.py
+-rw-r--r--   0        0        0      157 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/readers/csv.py
+-rw-r--r--   0        0        0      160 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/readers/json.py
+-rw-r--r--   0        0        0      145 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/readers/prelude.py
+-rw-r--r--   0        0        0      382 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/readers/spreadsheet.py
+-rw-r--r--   0        0        0       61 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/utils/__init__.py
+-rw-r--r--   0        0        0     6400 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/utils/attr_data.py
+-rw-r--r--   0        0        0     2960 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/utils/misc.py
+-rw-r--r--   0        0        0      828 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/utils/namespace_mixin.py
+-rw-r--r--   0        0        0      443 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/utils/safe.py
+-rw-r--r--   0        0        0     4341 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/utils/udf.py
+-rw-r--r--   0        0        0     7798 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/utils/validator.py
+-rw-r--r--   0        0        0        0 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/writers/__init__.py
+-rw-r--r--   0        0        0     3850 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/writers/base.py
+-rw-r--r--   0        0        0     3627 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/drepr/writers/rdfgraph_writer.py
+-rw-r--r--   0        0        0      604 2024-05-03 23:13:35.955143 drepr_v2-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 drepr_v2-1.2.2/PKG-INFO
```

### Comparing `drepr_v2-1.2.1/LICENSE` & `drepr_v2-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/__main__.py` & `drepr_v2-1.2.2/drepr/__main__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/align.py` & `drepr_v2-1.2.2/drepr/models/align.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/attr.py` & `drepr_v2-1.2.2/drepr/models/attr.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/drepr.py` & `drepr_v2-1.2.2/drepr/models/drepr.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/drepr_builder.py` & `drepr_v2-1.2.2/drepr/models/drepr_builder.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/parse_v1/__init__.py` & `drepr_v2-1.2.2/drepr/models/parse_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/parse_v1/align_parser.py` & `drepr_v2-1.2.2/drepr/models/parse_v1/align_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/parse_v1/attr_parser.py` & `drepr_v2-1.2.2/drepr/models/parse_v1/attr_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             attr_conf.get("value_type", ValueType.UnspecifiedSingle.value)
         )
 
         if "missing_values" in attr_conf:
             trace = f"{parse_trace}\nParsing missing_values of the attribute"
             Validator.must_be_list(attr_conf["missing_values"], trace)
             for val in attr_conf["missing_values"]:
-                if not isinstance(val, (str, int, float)):
+                if val is not None and not isinstance(val, (str, int, bool, float)):
                     raise InputError(
                         f"{trace}\nERROR: invalid value. Expected either one of string, "
                         f"integer, or float. Get f{type(val)} instead"
                     )
 
         missing_values = attr_conf.get("missing_values", [])
         return Attr(
```

### Comparing `drepr_v2-1.2.1/drepr/models/parse_v1/path_parser.py` & `drepr_v2-1.2.2/drepr/models/parse_v1/path_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/parse_v1/preprocessing_parser.py` & `drepr_v2-1.2.2/drepr/models/parse_v1/preprocessing_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/parse_v1/resource_parser.py` & `drepr_v2-1.2.2/drepr/models/parse_v1/resource_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/parse_v1/sm_parser.py` & `drepr_v2-1.2.2/drepr/models/parse_v1/sm_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/parse_v2/__init__.py` & `drepr_v2-1.2.2/drepr/models/parse_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/parse_v2/path_parser.py` & `drepr_v2-1.2.2/drepr/models/parse_v2/path_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/parse_v2/sm_parser.py` & `drepr_v2-1.2.2/drepr/models/parse_v2/sm_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/path.py` & `drepr_v2-1.2.2/drepr/models/path.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/preprocessing.py` & `drepr_v2-1.2.2/drepr/models/preprocessing.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/resource.py` & `drepr_v2-1.2.2/drepr/models/resource.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/models/sm.py` & `drepr_v2-1.2.2/drepr/models/sm.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/planning/class_map_plan.py` & `drepr_v2-1.2.2/drepr/planning/class_map_plan.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/planning/drepr_model_alignments.py` & `drepr_v2-1.2.2/drepr/planning/drepr_model_alignments.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/planning/topological_sorting.py` & `drepr_v2-1.2.2/drepr/planning/topological_sorting.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/program_generation/alignment_fn.py` & `drepr_v2-1.2.2/drepr/program_generation/alignment_fn.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/program_generation/main.py` & `drepr_v2-1.2.2/drepr/program_generation/main.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/program_generation/predefined_fn.py` & `drepr_v2-1.2.2/drepr/program_generation/predefined_fn.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/program_generation/preprocessing.py` & `drepr_v2-1.2.2/drepr/program_generation/preprocessing.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/program_generation/program_space.py` & `drepr_v2-1.2.2/drepr/program_generation/program_space.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/program_generation/writers.py` & `drepr_v2-1.2.2/drepr/program_generation/writers.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/utils/attr_data.py` & `drepr_v2-1.2.2/drepr/utils/attr_data.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/utils/misc.py` & `drepr_v2-1.2.2/drepr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/utils/namespace_mixin.py` & `drepr_v2-1.2.2/drepr/utils/namespace_mixin.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/utils/udf.py` & `drepr_v2-1.2.2/drepr/utils/udf.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/utils/validator.py` & `drepr_v2-1.2.2/drepr/utils/validator.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/writers/base.py` & `drepr_v2-1.2.2/drepr/writers/base.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/drepr/writers/rdfgraph_writer.py` & `drepr_v2-1.2.2/drepr/writers/rdfgraph_writer.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.2.1/pyproject.toml` & `drepr_v2-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drepr-v2"
-version = "1.2.1"
+version = "1.2.2"
 description = ""
 authors = ["Binh Vu <binh@toan2.com>"]
 readme = "README.md"
 packages = [{ include = "drepr" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `drepr_v2-1.2.1/PKG-INFO` & `drepr_v2-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drepr-v2
-Version: 1.2.1
+Version: 1.2.2
 Summary: 
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

