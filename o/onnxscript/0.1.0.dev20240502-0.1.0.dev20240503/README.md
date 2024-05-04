# Comparing `tmp/onnxscript-0.1.0.dev20240502.tar.gz` & `tmp/onnxscript-0.1.0.dev20240503.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240502.tar", last modified: Thu May  2 00:01:05 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240503.tar", last modified: Fri May  3 00:01:13 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240502.tar` & `onnxscript-0.1.0.dev20240503.tar`

### file list

```diff
@@ -1,218 +1,217 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.934937 onnxscript-0.1.0.dev20240502/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-05-02 00:01:05.934937 onnxscript-0.1.0.dev20240502/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.898936 onnxscript-0.1.0.dev20240502/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.902937 onnxscript-0.1.0.dev20240502/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.902937 onnxscript-0.1.0.dev20240502/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.902937 onnxscript-0.1.0.dev20240502/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.902937 onnxscript-0.1.0.dev20240502/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.894936 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.902937 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.914936 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.894936 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.894936 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.914936 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.914936 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.914936 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.918937 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.922937 onnxscript-0.1.0.dev20240502/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.922937 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.926936 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.930936 onnxscript-0.1.0.dev20240502/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4597 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.930936 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6603 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35227 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.930936 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5522 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.934937 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36123 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.934937 onnxscript-0.1.0.dev20240502/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.934937 onnxscript-0.1.0.dev20240502/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 00:01:05.934937 onnxscript-0.1.0.dev20240502/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-05-02 00:01:05.000000 onnxscript-0.1.0.dev20240502/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-05-02 00:01:05.000000 onnxscript-0.1.0.dev20240502/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-02 00:01:05.000000 onnxscript-0.1.0.dev20240502/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-02 00:01:05.000000 onnxscript-0.1.0.dev20240502/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-02 00:01:05.000000 onnxscript-0.1.0.dev20240502/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-02 00:01:05.934937 onnxscript-0.1.0.dev20240502/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-02 00:00:49.000000 onnxscript-0.1.0.dev20240502/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.804663 onnxscript-0.1.0.dev20240503/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.808663 onnxscript-0.1.0.dev20240503/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.808663 onnxscript-0.1.0.dev20240503/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.808663 onnxscript-0.1.0.dev20240503/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.808663 onnxscript-0.1.0.dev20240503/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.800663 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.812663 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.824663 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.800663 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.800663 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.824663 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.824663 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.824663 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.828663 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.832663 onnxscript-0.1.0.dev20240503/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.832663 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.840663 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.840663 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4385 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10232 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.844663 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6405 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35227 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.844663 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5196 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1824 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34065 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-05-03 00:01:13.000000 onnxscript-0.1.0.dev20240503/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8162 2024-05-03 00:01:13.000000 onnxscript-0.1.0.dev20240503/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-03 00:01:13.000000 onnxscript-0.1.0.dev20240503/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-03 00:01:13.000000 onnxscript-0.1.0.dev20240503/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-03 00:01:13.000000 onnxscript-0.1.0.dev20240503/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240502/LICENSE` & `onnxscript-0.1.0.dev20240503/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/PKG-INFO` & `onnxscript-0.1.0.dev20240503/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240502
+Version: 0.1.0.dev20240503
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240502/README.md` & `onnxscript-0.1.0.dev20240503/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240503/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240503/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240503/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240503/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240503/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240503/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240503/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240503/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240503/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240503/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240503/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240503/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240503/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240503/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240503/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240503/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240503/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240503/onnxscript/ir/_convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240503/onnxscript/ir/_core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240503/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240503/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240503/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240503/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240503/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240503/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240503/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240503/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240503/onnxscript/ir/serde.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240503/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/main.py` & `onnxscript-0.1.0.dev20240503/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240503/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 from typing import Any
 
 import onnx
 import onnx.shape_inference
 
 from onnxscript import rewriter
 from onnxscript.optimizer.constant_folding import fold_constants
-from onnxscript.optimizer.copy_propagation import (
-    do_copy_propagation,
-    do_sequence_simplification,
-)
 from onnxscript.optimizer.remove_unused import remove_unused_nodes
 from onnxscript.optimizer.remove_unused_function import remove_unused_functions
 from onnxscript.optimizer.simple_function_folding import (
     inline_functions_with_unused_outputs,
     inline_simple_functions,
 )
 from onnxscript.rewriter import (
@@ -104,18 +100,15 @@
                 function.domain,
                 function.name,
                 node.domain,
                 node.op_type,
                 node.name,
             )
 
-    # do_sequence_simplification(model)
     return model
 
 
 __all__ = [
     "fold_constants",
     "remove_unused_nodes",
     "optimize",
-    "do_copy_propagation",
-    "do_sequence_simplification",
 ]
```

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/constant_folding.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,15 +259,18 @@
 
 def fold_constants(
     model: onnx.ModelProto,
     external_data_folder: str = "",
     *,
     onnx_shape_inference: bool = False,
 ) -> bool:
-    """Returns true iff the model was modified."""
+    """
+    Applies constant folding optimization to the model.
+    Returns true iff the model was modified.
+    """
     folder = ConstantFolder(
         evaluator.registry,
         external_data_folder,
         do_shape_inference=onnx_shape_inference,
     )
     folder.visit_model(model)
     for op in folder.counts:
```

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/simple_function_folding.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,14 +196,15 @@
 
     @property
     def function_with_unused_outputs(self) -> dict[ir.FunctionId, onnx.FunctionProto]:
         return self._function_with_unused_outputs
 
 
 def inline_simple_functions(model: onnx.ModelProto, node_count: int = 2) -> bool:
+    """Inlines simple functions based on a node count threshold"""
     inliner = FunctionInliner(node_count)
     inliner.visit_model(model)
     logger.info(
         "inlined %s simple functions based on node count threshold %s.",
         len(inliner.counts),
         node_count,
     )
@@ -214,14 +215,15 @@
             op[1],
             inliner.counts[op],
         )
     return inliner.modified
 
 
 def inline_functions_with_unused_outputs(model: onnx.ModelProto) -> bool:
+    """Inlines function nodes that have unused outputs."""
     # TODO: Use onnx.inliner after 1.16.
     # This visitor based inliner is used to ensure the function inner value info remains consistent.
     visitor = FindFunctionWithUnusedOutputsVisitor()
     visitor.visit_model(model)
     # FIXME: Fix the type of the argument passed into SelectedFunctionInliner
     inliner = SelectedFunctionInliner(visitor.function_with_unused_outputs.values())  # type: ignore[arg-type]
     inliner.visit_model(model)
```

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 from __future__ import annotations
 
 import logging
-from typing import Any
 
 import numpy as np
 
-from onnxscript import ir
 from onnxscript.rewriter import _ir_utils, pattern
 
 op = pattern.onnxop
 logger = logging.getLogger(__name__)
 
 
 # condition to check if we need to replace the pattern
-def check_if_need_reshape(match_bindings: dict[str, ir.Value | Any]) -> bool:
+def check_if_need_reshape(input_a, input_b, shape_c, **_) -> bool:
     """If matmul broadcasting is enough, then we don't need the reshapes.
 
     To validate this, we need to check the following:
     1. Input shapes check: input_a and input_b should be broadcastable
     2. Output shape check: shape_c should be the same as the output shape from the matmul(input_a, input_b)
 
     If the above are true, then we don't need the reshapes.
 
-    Args:
-        match_bindings: The match binding dictionary from a MatchResult.
-
     Returns:
         bool: True if we need to replace the pattern, False otherwise.
 
     """
-    input_a_shape = match_bindings["input_a"].shape
-    input_b_shape = match_bindings["input_b"].shape
+    input_a_shape = input_a.shape
+    input_b_shape = input_b.shape
     # TODO: Get a helper func to get const_value
-    shape_c_value = _ir_utils.propagate_const_value(match_bindings["shape_c"])
+    shape_c_value = _ir_utils.propagate_const_value(shape_c)
     shape_c = shape_c_value.const_value.numpy()  # type: ignore[union-attr]
     if shape_c is None:
         return False
     if not isinstance(shape_c, np.ndarray):
         logger.info("Unexpected shape_c value. Expected np.ndarray, got %s", type(shape_c))
         return False
     if len(shape_c.shape) != 1:
```

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 from __future__ import annotations
 
 import logging
-from typing import Any
 
 import numpy as np
 import onnx
 
-from onnxscript import ir
 from onnxscript.rewriter import _ir_utils, pattern
 
 op = pattern.onnxop
 msft_op = pattern.msft_op
 torch_module_op = pattern.torch_module_op
 
 logger = logging.getLogger(__name__)
 
 
-def _check_if_simulated_instance_norm_is_used_impl(
+def check_if_simulated_instance_norm_is_used(
     input_x,
     adjusted_input_shape,
     original_input_shape,
     weight_for_norm,
     bias_for_norm,
     weight_full,
     bias_full,
-    **kwargs,
+    **_,
 ) -> bool:
+    """Check if the simulated instance normalization is used.
+
+    In torchlib with opset18, onnx.GroupNorm is using wrong definition, so
+    we use InstanceNormalization to simulate GroupNormalization. We need to check if there are arguments created to simulation.
+    If there are, then we need to replace the pattern. If they are not used, then we don't need to replace the pattern.
+
+    To validate this, we need to check the following:
+    1. weight_for_norm are all 1 and bias_for_norm are all 0, as they are created for the simulation.
+    2. weight_full and bias_full are unsqueezed to be easily broadcastable.
+    3. input rank should be 4
+    4. weight_full and bias_full should have ones except first dim.
+    5. adjusted_input_shape is a constant tensor of form [0, g, -1]
+    6. original_input_shape is the same as input_x shape.
+
+    Returns:
+        bool: True if the simulated instance normalization is used, False otherwise.
+    """
     weight_for_norm = _ir_utils.propagate_const_value(weight_for_norm)
     weight_for_norm = _ir_utils.get_numpy_from_ir_value(weight_for_norm)
 
     bias_for_norm = _ir_utils.propagate_const_value(bias_for_norm)
     bias_for_norm = _ir_utils.get_numpy_from_ir_value(bias_for_norm)
 
     if not np.all(weight_for_norm == 1):
@@ -66,40 +81,14 @@
     original_input_shape = _ir_utils.get_numpy_from_ir_value(original_input_shape)
     if original_input_shape is None or original_input_shape.tolist() != input_x.shape:
         return False
 
     return True
 
 
-def check_if_simulated_instance_norm_is_used(
-    match_bindings: dict[str, ir.Value | Any],
-) -> bool:
-    """Check if the simulated instance normalization is used.
-
-    In torchlib with opset18, onnx.GroupNorm is using wrong definition, so
-    we use InstanceNormalization to simulate GroupNormalization. We need to check if there are arguments created to simulation.
-    If there are, then we need to replace the pattern. If they are not used, then we don't need to replace the pattern.
-
-    To validate this, we need to check the following:
-    1. weight_for_norm are all 1 and bias_for_norm are all 0, as they are created for the simulation.
-    2. weight_full and bias_full are unsqueezed to be easily broadcastable.
-    3. input rank should be 4
-    4. weight_full and bias_full should have ones except first dim.
-    5. adjusted_input_shape is a constant tensor of form [0, g, -1]
-    6. original_input_shape is the same as input_x shape.
-
-    Args:
-        match_bindings: The match binding dictionary from a MatchResult.
-
-    Returns:
-        bool: True if the simulated instance normalization is used, False otherwise.
-    """
-    return _check_if_simulated_instance_norm_is_used_impl(**match_bindings)
-
-
 def instance_simulates_group_normalization_pattern(
     input_x,
     adjusted_input_shape,
     original_input_shape,
     weight_for_norm,
     bias_for_norm,
     weight_full,
```

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import logging
-from typing import Any
 
 import onnx
 
 from onnxscript import ir
 from onnxscript.rewriter import pattern
 
 op = pattern.onnxop
@@ -28,23 +27,22 @@
     return op.Cast(softmax, to=onnx.TensorProto.FLOAT16)
 
 
 def softmax_without_axis(op, input):
     return op.Softmax(input)
 
 
-def check_if_fp16_input(match_bindings: dict[str, ir.Value | Any]) -> bool:
-    input_val = match_bindings.get("input")
-    if input_val is None:
+def check_if_fp16_input(input, **_) -> bool:
+    if input is None:
         logger.warning(
             "Cannot perform softmax upcast removal: "
             "cannot retrieve match_bindings for 'input' for dtype validation."
         )
         return False
-    return input_val.dtype == ir.DataType.FLOAT16
+    return input.dtype == ir.DataType.FLOAT16
 
 
 # pylint: disable=pointless-string-statement
 """
 This is an onnxruntime specific pattern. Softmax upcast is a common
 pattern observed in transformers models to prevent overflow. However
 this is not required since onnxruntime implementation already takes
```

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/pattern.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,302 +1,205 @@
 from __future__ import annotations
 
 import dataclasses
 import inspect
 import itertools
 import math
-from typing import Any, Callable, List, MutableSequence, Optional, Sequence, Tuple
+from typing import (
+    Any,
+    Callable,
+    List,
+    MutableSequence,
+    Optional,
+    Protocol,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
-import numpy as np
 import onnx
-import onnx.numpy_helper
-import onnx.printer
 
 from onnxscript import ir
 from onnxscript.ir import _convenience
 from onnxscript.rewriter import _ir_utils, _tape
 
-# Overview of the pattern module: The classes below are used to define both
-# patterns (that we search for) and replacements for rewrite rules.
-# The matches() method of a pattern is used to check if an IR component
-# matches the pattern.
-# TODO: Ensure that all matches() methods have same type signature (where
-# appropriate).
+T = TypeVar("T")
 
 
-class PythonPattern:
-    def __init__(self, value: int | str | Sequence, name: str | None = None) -> None:
-        self._value = value
-        self._name = name
-
-    @property
-    def value(self) -> int | str | Sequence:
-        return self._value
-
-    @property
-    def name(self) -> str | None:
-        return self._name
-
-    def matches(self, value: int | str | Sequence) -> bool:
-        return value == self.value
-
-
-class StringConstantPattern:
-    def __init__(self, value: str, name: str) -> None:
-        self._value = value
-        self._name = name
-
-    @property
-    def value(self) -> str:
-        return self._value
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    def matches(self, attr: ir.AttrString) -> bool:
-        return attr.value == self.value
-
-
-class IntConstantPattern:
-    def __init__(self, value: int, name: str) -> None:
-        self._value = value
-        self._name = name
-
-    @property
-    def value(self) -> int:
-        return self._value
+class Pattern(Protocol[T]):  # type: ignore[misc]
+    """This is essentially a Predicate[T], that is, a Callable[[T], bool] bound to the name "matches"."""
 
-    @property
-    def name(self) -> str:
-        return self._name
+    def matches(self, item: T) -> bool: ...
 
-    def matches(self, attr: ir.AttrInt64) -> bool:
-        return attr.value == self.value
 
+class StringConstantPattern(Pattern[str]):
+    """Matches strings with given value."""
 
-class ListConstantPattern:
-    def __init__(self, value: Sequence[int | str | float], name: str) -> None:
+    def __init__(self, value: str):
         self._value = value
-        self._name = name
-
-    @property
-    def value(self) -> Sequence[int | str | float]:
-        return self._value
-
-    @property
-    def name(self) -> str:
-        return self._name
 
-    def matches(self, attr: ir.AttrFloat32s | ir.AttrInt64s | ir.AttrStrings) -> bool:
-        # TODO: Need more data points to determine if this is the right way to compare lists.
-        return attr.value == self.value
+    def matches(self, item: str) -> bool:
+        return item == self._value
 
 
-class PrefixPattern:
-    """This pattern is used to simplify submodule opset pattern matching."""
+class PrefixPattern(Pattern[str]):
+    """Matches strings with a given prefix."""
 
     def __init__(self, value: str) -> None:
         self._value = value
 
-    @property
-    def value(self) -> str:
-        return self._value
-
     def matches(self, value: str) -> bool:
-        return value.startswith(self.value)
-
-
-class FloatConstantPattern:
-    def __init__(
-        self, value: float, name: str, rel_tol: float = 1e-5, abs_tol: float = 1e-8
-    ) -> None:
-        self._value = value
-        self._name = name
-        self._rel_tol = rel_tol
-        self._abs_tol = abs_tol
-
-    @property
-    def value(self):
-        return self._value
+        return value.startswith(self._value)
 
-    @property
-    def name(self):
-        return self._name
-
-    def matches(self, attr: ir.AttrFloat32):
-        return math.isclose(
-            attr.value, self.value, rel_tol=self._rel_tol, abs_tol=self._abs_tol
-        )
 
+class AttrPattern(Pattern[Union[ir.Attr, ir.RefAttr]]):
+    """Base class for an attribute pattern. Matches any attribute value by default."""
 
-class TensorConstantPattern:
-    def __init__(
-        self, value: ir.TensorProtocol, name, rel_tol: float = 1e-3, abs_tol: float = 1e-3
-    ) -> None:
-        self._value = value
-        self._name = name
-        self._rel_tol = rel_tol
-        self._abs_tol = abs_tol
+    def __init__(self, name: str | None):
+        self.name = name
 
-    @property
-    def value(self):
-        return self._value
+    def matches(self, attr: ir.Attr | ir.RefAttr) -> bool:
+        return True
 
-    @property
-    def name(self):
-        return self._name
 
-    def matches(self, attr: ir.AttrTensor):
-        return (
-            attr.value.dtype == self._value.dtype
-            and attr.value.shape == self._value.shape
-            and np.allclose(
-                attr.value,
-                self._value,
-                rtol=self._rel_tol,
-                atol=self._abs_tol,
-            )
-        )
+# TODO: Support tensors. Align with usage elsewhere.
+SupportedAttrTypes = Union[
+    int,
+    float,
+    str,
+    Sequence[int],
+    Sequence[float],
+    Sequence[str],
+]
 
 
-def _make_constant_pattern(
-    value: float | int | Sequence | ir.TensorProtocol, name: str
-) -> (
-    IntConstantPattern
-    | FloatConstantPattern
-    | TensorConstantPattern
-    | StringConstantPattern
-    | ListConstantPattern
-):
-    """Convert an attrbute value to a ConstantPattern."""
-    if isinstance(value, float):
-        return FloatConstantPattern(value, name)
-    if isinstance(value, int):
-        return IntConstantPattern(value, name)
-    if isinstance(value, str):
-        return StringConstantPattern(value, name)
-    if isinstance(value, Sequence):
-        return ListConstantPattern(value, name)
-    if isinstance(value, ir.TensorProtocol):
-        return TensorConstantPattern(value, name)
-    raise TypeError(f"Cannot convert {type(value)} to ConstantPattern")
+class AttrConstantPattern(AttrPattern):
+    """Matches attributes with given value.
 
+    Uses standard equality for matching. For list-valued attributes, the order of elements matters.
+    If order is immaterial, we need to define a separate pattern for that.
+    """
 
-class AnyPattern:
-    def matches(self, value) -> bool:
-        return True
+    def __init__(self, value: SupportedAttrTypes):
+        super().__init__(None)
+        self._value = value
 
+    def matches(self, attr: ir.Attr | ir.RefAttr) -> bool:
+        return isinstance(attr, ir.Attr) and attr.value == self._value
 
-class AttrPattern:
-    def __init__(
-        self, value: Var | int | float | Sequence | ir.TensorProtocol, name: str
-    ) -> None:
-        if isinstance(value, Var):
-            self.value_pattern = value
-        elif isinstance(value, (int, float, Sequence, ir.TensorProtocol)):
-            self.value_pattern = _make_constant_pattern(value, name)  # type: ignore[assignment]
-        else:
-            raise TypeError(f"Cannot convert {type(value)} to AttrPattern")
 
-    def matches(
-        self,
-        attr_val: int | float | Sequence | Var | ir.TensorProtocol | ir.Value,
-        model: ir.Model,
-    ) -> MatchResult:
-        if isinstance(self.value_pattern, Var):
-            return self.value_pattern.matches(attr_val, model)  # type: ignore[arg-type]
-        return self.value_pattern.matches(attr_val)
+def _to_attr_pattern(value: AttrPattern | ValuePattern | SupportedAttrTypes) -> AttrPattern:
+    """Represents promotion of values allowed as keyword-arguments in a pattern-builder call to an AttrPattern."""
+    if isinstance(value, AttrPattern):
+        return value
+    if type(value) == ValuePattern:
+        # This is a hack. Currently, when we create pattern-variables, we create them as ValuePattern,
+        # and change them to AttrPattern if/when used in an attribute context. We could use type
+        # annotations to distinguish between ValuePattern and AttrPattern, but forces users to
+        # use these type annotations.
+        # TODO: check for misuse at rule-creation time. (Currently will be caught by matcher at match-time.)
+        return AttrPattern(value.name)
+    if isinstance(value, (int, float, str)):
+        return AttrConstantPattern(value)
+    if isinstance(value, Sequence):
+        if all(isinstance(i, (int, float)) for i in value):
+            return AttrConstantPattern(value)
+        if all(isinstance(i, str) for i in value):
+            return AttrConstantPattern(value)
+        raise ValueError("Only lists of int/float/str can be used as an AttrPattern")
+    raise TypeError(f"Cannot convert {type(value)} to AttrPattern")
 
 
-class OpsetPattern:
+class OpsetPatternBuilder(Pattern[str]):
     """Represents an opset pattern.
 
-    It is used primarily to create a NodePattern (via OpPattern).
+    (i) It is used to create a NodePattern (via OpPatternBuilder).
     Example usage:
     ::
 
         z = op.Matmul(x, y)
 
-    Here, `op` is an instance of OpsetPattern and `op.Matmul` is an instance
-    of OpPattern, and  `op.Matmul(x, y)` is an instance of NodePattern.
+    Here, `op` is an instance of OpsetPatternBuilder and `op.Matmul` is an instance
+    of OpPatternBuilder, and  `op.Matmul(x, y)` is an instance of NodePattern.
 
-    An opset pattern is also matched against the actual opset used in the
+    (ii) An opset pattern is also matched against the actual opset domain used in the
     input model.
     """
 
-    def __init__(self, domain_pattern: PythonPattern | PrefixPattern | str) -> None:
+    def __init__(self, domain_pattern: Pattern[str] | str) -> None:
         if isinstance(domain_pattern, str):
-            domain_pattern = PythonPattern(domain_pattern)
+            domain_pattern = StringConstantPattern(domain_pattern)
         self.domain_pattern = domain_pattern
 
     @classmethod
-    def domain_prefix(cls, domain: str) -> OpsetPattern:
+    def domain_prefix(cls, domain: str) -> OpsetPatternBuilder:
         return cls(PrefixPattern(domain))
 
     def matches(self, domain):
         return self.domain_pattern.matches(domain)
 
-    def __getattr__(self, name: str) -> Any:
-        return OpPattern(self, PythonPattern(name))
+    def __getattr__(self, name: str) -> OpPatternBuilder:
+        return OpPatternBuilder(self, StringConstantPattern(name))
 
-    def submodule(self, name: str) -> Any:
+    def submodule(self, name: str) -> OpPatternBuilder:
         """This method is used to match against submodule ops with prefix."""
-        return OpPattern(self, PrefixPattern(name))
+        return OpPatternBuilder(self, PrefixPattern(name))
 
 
-onnxop = OpsetPattern("")
+onnxop = OpsetPatternBuilder("")
 
-msft_op = OpsetPattern("com.microsoft")
+msft_op = OpsetPatternBuilder("com.microsoft")
 
-torch_module_op = OpsetPattern.domain_prefix("pkg.torch")
+torch_module_op = OpsetPatternBuilder.domain_prefix("pkg.torch")
 
 
-class OpPattern:
+class OpPatternBuilder:
     """A utility class to build a NodePattern.
 
     It is used primarily to create a NodePattern.
     Example usage:
     ::
 
         z = op.Matmul(x, y)
 
-    Here, `op` is an instance of OpsetPattern and `op.Matmul` is an instance
-    of OpPattern, and  `op.Matmul(x, y)` is an instance of NodePattern.
+    Here, `op` is an instance of OpsetPatternBuilder and `op.Matmul` is an instance
+    of OpPatternBuilder, and  `op.Matmul(x, y)` is an instance of NodePattern.
 
     """
 
     def __init__(
         self,
-        opset_pattern: OpsetPattern,
-        op_name_pattern: PythonPattern | PrefixPattern,
+        opset_pattern: Pattern[str],
+        op_name_pattern: Pattern[str],
     ) -> None:
         self.opset_pattern = opset_pattern
         self.op_name_pattern = op_name_pattern
 
     def __call__(self, *args, **kwargs):
         # TODO(rama): Unify with convention used elsewhere.
         if "_num_outputs" in kwargs:
             num_outputs = kwargs["_num_outputs"]
             del kwargs["_num_outputs"]
         else:
             num_outputs = 1
-        attributes = {
-            name: AttrPattern(value=value, name=name) for (name, value) in kwargs.items()
-        }
-        node_pattern = NodePattern(self.opset_pattern, self.op_name_pattern, args, attributes)
+        inputs = [_to_value_pattern(x) for x in args]
+        attributes = {name: _to_attr_pattern(value) for (name, value) in kwargs.items()}
+        node_pattern = NodePattern(
+            self.opset_pattern, self.op_name_pattern, inputs, attributes
+        )
         if num_outputs == 1:
             return NodeOutputPattern(node_pattern, 0)
         else:
             return [NodeOutputPattern(node_pattern, i) for i in range(num_outputs)]
 
 
 def _to_value_pattern(
     x: ValuePattern | int | float | None,
-) -> NodeOutputPattern | Constant | ValuePattern | None:
+) -> ValuePattern | None:
     """Promotes an input-value used to construct a NodePattern to a ValuePattern.
 
     Example usage:
     ::
         x = op.MatMul(a, b)
         z = op.Add(x, 0)
 
@@ -306,16 +209,21 @@
     Note that this is a shorthand for creating a Constant pattern. The user can more
     explicitly write this as:
     ::
         z = op.Add(x, op.Constant(0))
     """
     if x is None or isinstance(x, ValuePattern):
         return x
-    if isinstance(x, (int, float, Sequence)):
+    if isinstance(x, (int, float)):
         return Constant(x)
+    # TODO(rama): support lists of int/float
+    # if isinstance(x, list):
+    #     if all(isinstance(i, (int, float)) for i in x):
+    #         return Constant(x)
+    #     raise ValueError("Only lists of int/float can be used as a ValuePattern")
     # TODO(titaiwang): Could this be wrapped Constant?
     raise TypeError(f"Cannot convert {type(x)} to ValuePattern")
 
 
 class MatchResult:
     """Represents the result of a match operation.
 
@@ -352,16 +260,27 @@
     def FAIL(cls):
         return cls(False)
 
     @property
     def nodes(self) -> MutableSequence[ir.Node]:
         return self.matched_nodes
 
-    def bind(self, var: str, value: Any):
+    def bind(self, var: str, value: Any) -> bool:
+        """Binds a pattern variable name to a value from the matched IR.
+
+        Returns True if the binding is successful, False otherwise (when the binding is inconsistent).
+        """
+        if var in self.bindings:
+            # TODO(rama): Use appropriate equality-check here.
+            if self.bindings[var] == value:
+                return True
+            self.success = False
+            return False
         self.bindings[var] = value
+        return True
 
     def extend(self, other: MatchResult | bool):
         if not self.success:
             return
         if not other:
             self.success = False
             return
@@ -388,15 +307,15 @@
 
     def __init__(self, name: str | None) -> None:
         self.name = name
 
     def __repr__(self) -> str:
         return f"ValuePattern({self.name!r})"
 
-    def matches(self, value: ir.Value, model: ir.Model):
+    def matches(self, value: ir.Value):
         result = MatchResult(success=True)
         if self.name is not None:
             result.bind(self.name, value)
         return result
 
     def commute(self) -> Sequence[ValuePattern]:
         """Return a list of commuted patterns.
@@ -441,26 +360,25 @@
     This differs from a NodeOutputPattern in that it matches against a node (which
     may produce 1 or more outputs), whereas a NodeOutputPattern matches against
     a specific output of a node.
     """
 
     def __init__(
         self,
-        domain: OpsetPattern,
-        op: PythonPattern | PrefixPattern,
+        domain: Pattern[str],
+        op: Pattern[str],
         inputs: Sequence[int | float | ValuePattern | None],
         attributes: dict[str, AttrPattern],
     ):
         self.domain = domain
         self.op = op
         self.inputs = [_to_value_pattern(x) for x in inputs]
         self.attributes = attributes
-        self.bound_value = None
 
-    def matches_node(self, node: ir.Node, model: ir.Model) -> MatchResult:
+    def matches_node(self, node: ir.Node) -> MatchResult:
         """Examine if the IR node matches the self pattern."""
         if not self.domain.matches(node.domain):
             return MatchResult.FAIL()
         if not self.op.matches(node.op_type):
             return MatchResult.FAIL()
         match = MatchResult(success=True)
         # TODO: We should add filtered logging starting from here to emit why
@@ -468,32 +386,32 @@
         # because at least the starting node op_type is already matched.
         for arg_value, previous_node_output_pattern in zip(node.inputs, self.inputs):
             # previous_node_output_pattern could be a Var, if it's the original arg.
             if arg_value is None and previous_node_output_pattern is None:
                 continue
             if arg_value is None or previous_node_output_pattern is None:
                 return MatchResult.FAIL()
-            sub_match = previous_node_output_pattern.matches(arg_value, model)  # type: ignore[attr-defined]
+            sub_match = previous_node_output_pattern.matches(arg_value)
             match.extend(sub_match)
             if not match:  # If sub-match failed,
                 return match
         # Sub-graphs not handled yet.
         for name, attr_pattern in self.attributes.items():
             attr_value = node.attributes.get(name)
             if attr_value is None:
                 return MatchResult.FAIL()
-            sub_match = attr_pattern.matches(attr_value, model)  # type: ignore[arg-type]
-            if not sub_match:
+            if not attr_pattern.matches(attr_value):
                 return MatchResult.FAIL()
-            match.extend(sub_match)
+            if attr_pattern.name is not None:
+                if not match.bind(attr_pattern.name, attr_value):
+                    return match
         for name in node.attributes:
             # TODO: Support matching default nodes for attributes.
             if name not in self.attributes:
                 return MatchResult.FAIL()
-        assert match.nodes is not None, "Matched nodes should not be None."
         match.nodes.append(node)
         return match
 
     def commute(self) -> Sequence[NodePattern]:
         list_of_lists = [
             [None] if pattern is None else pattern.commute() for pattern in self.inputs
         ]  # type: ignore[attr-defined]
@@ -524,24 +442,25 @@
     def __init__(
         self, node_pattern: NodePattern, output_index: int, name: str | None = None
     ) -> None:
         super().__init__(name)
         self.node_pattern = node_pattern
         self.output_index = output_index
 
-    def matches(self, value: ir.Value, model: ir.Model):
+    def matches(self, value: ir.Value):
         """Match the StaticValueInfo from IR with the `matches_node()` in node pattern."""
         node = value.producer()
         if node is None:
             return MatchResult.FAIL()
         if value.index() != self.output_index:
             return MatchResult.FAIL()
-        return self.node_pattern.matches_node(node, model)
+        return self.node_pattern.matches_node(node)
 
     def commute(self) -> Sequence[ValuePattern]:
+        # TODO
         return [
             NodeOutputPattern(pattern, self.output_index, self.name)
             for pattern in self.node_pattern.commute()
         ]
 
 
 Var = ValuePattern
@@ -564,15 +483,15 @@
         )
         # Note: If the value is produced by a Constant node, we could include
         # the Constant node in the return_value list. However, we don't do that.
         # Instead, we will rely on DCE to remove the constant node if it is not
         # used elsewhere.
         return MatchResult(success=status)
 
-    def matches(self, value: ir.Value, model: ir.Model):
+    def matches(self, value: ir.Value):
         value = _ir_utils.propagate_const_value(value)
         constant_value = _ir_utils.get_numpy_from_ir_value(value)
         if constant_value is None:
             return MatchResult.FAIL()
 
         # TODO (rama): allow users to specify shape requirement, if desired.
         if constant_value.size != 1:
@@ -580,57 +499,86 @@
 
         return self.match_scalar(constant_value.item())
 
     def commute(self) -> list[ValuePattern]:
         return [self]
 
 
-def _handle_pattern_return_value(
-    node_output_pattern: NodeOutputPattern | list[NodeOutputPattern],
-) -> tuple[NodePattern, int]:
-    """This checks and cleans up the return value of a pattern-construction function.
+class GraphPattern:
+    """Represents a pattern that can be matched against a subgraph."""
+
+    def __init__(self, outputs: Sequence[ValuePattern]) -> None:
+        self.outputs = outputs
+        if len(outputs) == 0:
+            raise ValueError("GraphPattern must have at least one output")
+        # Check if all outputs are produced by the same node.
+        output_node = None
+        for i, value_pattern in enumerate(outputs):
+            if not isinstance(value_pattern, ValuePattern):
+                raise TypeError(
+                    f"Invalid type {type(value_pattern)} for graph pattern output."
+                )
+            if not isinstance(value_pattern, NodeOutputPattern) or (
+                value_pattern.output_index != i
+            ):
+                output_node = None
+            elif i == 0:
+                output_node = value_pattern.node_pattern
+            elif value_pattern.node_pattern is not output_node:
+                output_node = None
+        self._output_node = output_node
+
+    @property
+    def num_outputs(self) -> int:
+        return len(self.outputs)
+
+    def matches_node(self, node: ir.Node) -> MatchResult:
+        if self._output_node is None:
+            return MatchResult.FAIL()
+        return self._output_node.matches_node(node)
+
+    def commute(self) -> Sequence[GraphPattern]:
+        if self._output_node is None:
+            raise NotImplementedError(
+                "Cannot commute a graph pattern with multiple output nodes."
+            )
+        nodes = self._output_node.commute()
+        return [
+            GraphPattern([NodeOutputPattern(n, i) for i in range(self.num_outputs)])
+            for n in nodes
+        ]
+
+
+def _to_graph_pattern(pattern_constructor: Callable) -> GraphPattern:
+    """Convert a pattern-construction function to a GraphPattern.
 
     A pattern-construction function will return values as below:
     ::
-        def pattern(x, shape1, shape2):
+        def pattern(x: Var, shape1: Var, shape2: Var):
             ...
-            return op.SomeOp(...)
-    However, `SomeOp` may represent an ONNX op that produces multiple outputs.
-    This function validates that the return values represent the outputs of
-    a single NodePattern. It returns the node_pattern and the number of outputs.
-
-    This follows an important restriction of the pattern-matcher algorithm: it
-    only matches against subgraphs that end in a single terminal node. If we
-    permit two terminal nodes, then we would have to match against all possible
-    pairs of nodes in the graph, which produces an extra quadratic factor in the
-    complexity of the pattern-matching algorithm. In general, the complexity becomes
-    exponential in the number of terminal nodes.
+            return outputs
+
+    We create a pattern graph by creating pattern-variables for each parameter of the function,
+    and calling the function. The returned values are normalized to a list of ValuePatterns,
+    which represent the outputs of the pattern graph.
 
     Args:
-        node_output_pattern: NodeOutputPattern | Sequence[NodeOutputPattern]
+        pattern_constructor: Callable
 
     Returns:
-        tuple[NodePattern, int]: The last node_pattern, num_outputs
+        GraphPattern: A representation of the pattern that can be matched against a subgraph.
     """
-    if isinstance(node_output_pattern, NodeOutputPattern):
-        node_pattern = node_output_pattern.node_pattern
-        num_outputs = 1
-    elif isinstance(node_output_pattern, Sequence):
-        node_pattern = node_output_pattern[0].node_pattern
-        num_outputs = len(node_output_pattern)
-        for i, p in enumerate(node_output_pattern):
-            assert isinstance(p, NodeOutputPattern)
-            if (p.node_pattern is not node_pattern) or (p.output_index != i):
-                raise NotImplementedError(
-                    "Multi-output pattern not handled by this API. "
-                    "Use other APIs to handle multi-output patterns."
-                )
-    else:
-        raise TypeError(f"Invalid type {type(node_output_pattern)} for pattern")
-    return node_pattern, num_outputs
+    _pattern_vars = inspect.signature(pattern_constructor).parameters
+    vars = [Var(v) for v in _pattern_vars]
+    pattern_outputs = pattern_constructor(*vars)
+    # Returned value could be a single ValuePattern or a list of ValuePatterns.
+    # Normalize representation to a list of ValuePatterns.
+    if isinstance(pattern_outputs, ValuePattern):
+        pattern_outputs = [pattern_outputs]
+    return GraphPattern(pattern_outputs)
 
 
 def _valid_to_replace(matched_nodes: Sequence[ir.Node]) -> bool:
     """Check that values computed by the matched_nodes, except for the last one, are used only by the matched_nodes."""
     # * Must check that all values matched by pattern are used only by pattern,
     # except for the value that is replaced.
     # * Must ensure that replacement subgraph does not use any of the deleted
@@ -643,33 +591,14 @@
                 return False
             for consumer, _ in v.uses():
                 if consumer not in matched_nodes:
                     return False
     return True
 
 
-class TargetPatternFunction:
-    """The targeted pattern that will be replaced by the replacement pattern.
-
-    Attributes:
-        function (Callable): The pattern function that will be matched against the IR.
-    """
-
-    def __init__(self, function: Callable) -> None:
-        self._function = function
-
-    @property
-    def function(self) -> Callable:
-        return self._function
-
-    def get_pattern(self, variables: Sequence[Var]) -> tuple[NodePattern, int]:
-        node_output_pattern = self._function(*variables)
-        return _handle_pattern_return_value(node_output_pattern)
-
-
 # A type representing the domains/versions used in creating a replacement subgraph
 UsedOpsets = List[Tuple[str, Optional[int]]]
 
 
 class RewriterContext:
     """Context parameter used to build the replacement pattern."""
 
@@ -755,15 +684,15 @@
                 f"Expected version {imports[domain]}, but got {version}."
             )
 
 
 class RewriteRule:
     def __init__(
         self,
-        target_pattern: TargetPatternFunction | Callable | None = None,
+        target_pattern: GraphPattern | Callable | None = None,
         replacement_pattern: ReplacementPatternFunction | Callable | None = None,
         condition_function: Callable | None = None,
     ) -> None:
         """Create a rewrite rule.
 
         Args:
             target_pattern: The pattern function that will be
@@ -780,41 +709,33 @@
             assert replacement_pattern is None
             assert condition_function is None
             return
         elif replacement_pattern is None:
             raise ValueError(
                 "replacement_pattern must be provided if target_pattern is provided"
             )
-        # TODO: Do we want to tolerate Callable inputs?
-        if callable(target_pattern):
-            target_pattern = TargetPatternFunction(target_pattern)
-        if callable(replacement_pattern):
-            replacement_pattern = ReplacementPatternFunction(replacement_pattern)
 
+        if not isinstance(target_pattern, GraphPattern):
+            target_pattern = _to_graph_pattern(target_pattern)
         self._target_pattern = target_pattern
+
+        if not isinstance(replacement_pattern, ReplacementPatternFunction):
+            replacement_pattern = ReplacementPatternFunction(replacement_pattern)
         self._replacement_pattern = replacement_pattern
         self._condition_function = condition_function
 
-        _pattern_vars = inspect.signature(self._target_pattern.function).parameters
-
-        self._vars = [Var(v) for v in _pattern_vars]
-        # Get the last node pattern and number of outputs from the pattern function
-        self._target_node_pattern, self._target_num_outputs = self._target_pattern.get_pattern(
-            self._vars  # type: ignore[arg-type]
-        )
-
     def matches(self, node: ir.Node, model: ir.Model) -> MatchResult:
         """Check if the node from IR matches the pattern."""
-        if len(node.outputs) != self._target_num_outputs:
+        if len(node.outputs) != self._target_pattern.num_outputs:
             return MatchResult.FAIL()
-        match = self._target_node_pattern.matches_node(node, model)
+        match = self._target_pattern.matches_node(node)
         if (
             self._condition_function is not None
             and match
-            and not self._condition_function(match.bindings)
+            and not self._condition_function(**match.bindings)
         ):
             return MatchResult.FAIL()
         return match
 
     def try_rewrite(
         self, model: ir.Model, graph_or_function: ir.Graph | ir.Function, node: ir.Node
     ) -> ReplacementSubgraph | None:
@@ -822,18 +743,18 @@
         match = self.matches(node, model)
         if match:
             assert match.nodes is not None, "Matched values should not be None."
             if _valid_to_replace(match.nodes):
                 replacement_subgraph = self._replacement_pattern.get_replacement(match)
                 if replacement_subgraph is None:
                     return None
-                if len(replacement_subgraph.new_outputs) != self._target_num_outputs:
+                if len(replacement_subgraph.new_outputs) != self._target_pattern.num_outputs:
                     raise ValueError(
                         f"Number of outputs from replacement function does not match the number of outputs from the target pattern. "
-                        f"Expected {self._target_num_outputs}, but got {len(replacement_subgraph.new_outputs)}."
+                        f"Expected {self._target_pattern.num_outputs}, but got {len(replacement_subgraph.new_outputs)}."
                     )
                 # TODO(rama): Check/update opset-imports
                 # (i) Following is required by multi-output matcher too; move this.
                 # (ii) Remove the opset imports from deleted nodes?
                 _update_opset_imports(graph_or_function, replacement_subgraph)
                 _update_opset_imports(model.graph, replacement_subgraph)
                 return replacement_subgraph
@@ -847,21 +768,19 @@
         return RewriteRuleSet([self], commute=commute).count_matches(model)
 
     def commute(self) -> Sequence[RewriteRule]:
         def replace_pattern(new_pattern):
             """Return a shallow copy of self with node_pattern replaced by new_pattern."""
             rule = RewriteRule()
             rule._condition_function = self._condition_function
-            rule._target_node_pattern = new_pattern
-            rule._target_num_outputs = self._target_num_outputs
+            rule._target_pattern = new_pattern
             rule._replacement_pattern = self._replacement_pattern
-            rule._vars = self._vars
             return rule
 
-        return [replace_pattern(p) for p in self._target_node_pattern.commute()]
+        return [replace_pattern(p) for p in self._target_pattern.commute()]
 
 
 def _apply_delta(
     graph_or_function: ir.Graph | ir.Function,
     node: ir.Node,
     # TODO(jutinchuby): Use a more descriptive data structure to store deltas
     delta,
```

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240503/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240503/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240503/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240503/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240503/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240503/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240503/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript/values.py` & `onnxscript-0.1.0.dev20240503/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240503/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240502
+Version: 0.1.0.dev20240503
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240502/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240503/onnxscript.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,14 @@
 onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
 onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
 onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
 onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
 onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
 onnxscript/optimizer/__init__.py
 onnxscript/optimizer/constant_folding.py
-onnxscript/optimizer/copy_propagation.py
 onnxscript/optimizer/evaluator.py
 onnxscript/optimizer/fold_constants_v0.py
 onnxscript/optimizer/remove_unused.py
 onnxscript/optimizer/remove_unused_function.py
 onnxscript/optimizer/simple_function_folding.py
 onnxscript/rewriter/__init__.py
 onnxscript/rewriter/_ir_utils.py
```

### Comparing `onnxscript-0.1.0.dev20240502/pyproject.toml` & `onnxscript-0.1.0.dev20240503/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240502/setup.py` & `onnxscript-0.1.0.dev20240503/setup.py`

 * *Files identical despite different names*

