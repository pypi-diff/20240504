# Comparing `tmp/onediff-1.0.0.dev202405020126.tar.gz` & `tmp/onediff-1.0.0.dev202405030127.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediff-1.0.0.dev202405020126.tar", last modified: Thu May  2 01:26:20 2024, max compression
+gzip compressed data, was "onediff-1.0.0.dev202405030127.tar", last modified: Fri May  3 01:27:55 2024, max compression
```

## Comparing `onediff-1.0.0.dev202405020126.tar` & `onediff-1.0.0.dev202405030127.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.178638 onediff-1.0.0.dev202405020126/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14685 2024-05-02 01:26:20.178638 onediff-1.0.0.dev202405020126/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:26:20.178638 onediff-1.0.0.dev202405020126/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.166638 onediff-1.0.0.dev202405020126/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.170638 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.170638 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77110 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.170638 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers_enterprise_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.170638 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_onediff_quant/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_onediff_quant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.170638 onediff-1.0.0.dev202405020126/src/onediff/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.170638 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.174638 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/backends/oneflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/backends/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/deployable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.174638 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/import_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/import_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/import_tools/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/import_tools/import_module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/import_tools/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.174638 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/oneflow/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/oneflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/oneflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/oneflow/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/oneflow/dual_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/oneflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/oneflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.174638 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/transform/builtin_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/transform/custom_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/transform/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/transform/patch_for_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.178638 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/args_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/cost_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/graph_management_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/model_inplace_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/module_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/online_quantization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/param_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/patch_for_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/patch_for_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/version_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/with_fx_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/with_fx_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/with_onediff_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.178638 onediff-1.0.0.dev202405020126/src/onediff/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/optimization/attention_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/optimization/quant_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/optimization/rewrite_self_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.178638 onediff-1.0.0.dev202405020126/src/onediff/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/quantization/load_quantized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/quantization/quant_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/quantization/quantize_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/quantization/quantize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.178638 onediff-1.0.0.dev202405020126/src/onediff/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/src/onediff/schedulers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.178638 onediff-1.0.0.dev202405020126/src/onediff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14685 2024-05-02 01:26:20.000000 onediff-1.0.0.dev202405020126/src/onediff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-02 01:26:20.000000 onediff-1.0.0.dev202405020126/src/onediff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:26:20.000000 onediff-1.0.0.dev202405020126/src/onediff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 01:26:20.000000 onediff-1.0.0.dev202405020126/src/onediff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 01:26:20.000000 onediff-1.0.0.dev202405020126/src/onediff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:26:20.178638 onediff-1.0.0.dev202405020126/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/tests/test_dual_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/tests/test_pipelines_oneflow_img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/tests/test_quantitative_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-02 01:26:14.000000 onediff-1.0.0.dev202405020126/tests/test_quantize_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.986923 onediff-1.0.0.dev202405030127/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14685 2024-05-03 01:27:55.986923 onediff-1.0.0.dev202405030127/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 01:27:55.986923 onediff-1.0.0.dev202405030127/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.970922 onediff-1.0.0.dev202405030127/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.974923 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.974923 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77110 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.974923 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers_enterprise_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.974923 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_onediff_quant/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_onediff_quant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.974923 onediff-1.0.0.dev202405030127/src/onediff/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.978922 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.978922 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/backends/oneflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/backends/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/deployable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.978922 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/import_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/import_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/import_tools/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/import_tools/import_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/import_tools/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.978922 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/oneflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/oneflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/oneflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/oneflow/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/oneflow/dual_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/oneflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/oneflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.978922 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/transform/builtin_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/transform/custom_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/transform/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/transform/patch_for_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.982922 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/args_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/cost_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/graph_management_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/model_inplace_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/module_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/online_quantization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/param_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/patch_for_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/patch_for_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/version_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/with_fx_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/with_fx_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/with_onediff_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.982922 onediff-1.0.0.dev202405030127/src/onediff/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/optimization/attention_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/optimization/quant_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/optimization/rewrite_self_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.982922 onediff-1.0.0.dev202405030127/src/onediff/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/quantization/load_quantized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/quantization/quant_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/quantization/quantize_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/quantization/quantize_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.982922 onediff-1.0.0.dev202405030127/src/onediff/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/src/onediff/schedulers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.986923 onediff-1.0.0.dev202405030127/src/onediff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14685 2024-05-03 01:27:55.000000 onediff-1.0.0.dev202405030127/src/onediff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-03 01:27:55.000000 onediff-1.0.0.dev202405030127/src/onediff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:27:55.000000 onediff-1.0.0.dev202405030127/src/onediff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 01:27:55.000000 onediff-1.0.0.dev202405030127/src/onediff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-03 01:27:55.000000 onediff-1.0.0.dev202405030127/src/onediff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:55.986923 onediff-1.0.0.dev202405030127/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/tests/test_dual_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/tests/test_pipelines_oneflow_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/tests/test_quantitative_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-03 01:27:49.000000 onediff-1.0.0.dev202405030127/tests/test_quantize_custom_model.py
```

### Comparing `onediff-1.0.0.dev202405020126/LICENSE` & `onediff-1.0.0.dev202405030127/LICENSE`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/PKG-INFO` & `onediff-1.0.0.dev202405030127/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.0.0.dev202405020126
+Version: 1.0.0.dev202405030127
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405020126 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405030127 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `onediff-1.0.0.dev202405020126/README.md` & `onediff-1.0.0.dev202405030127/README.md`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/setup.py` & `onediff-1.0.0.dev202405030127/setup.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/__init__.py` & `onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py` & `onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/resnet_oflow.py` & `onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py` & `onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py` & `onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py` & `onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py` & `onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py` & `onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/infer_compiler_registry/register_onediff_quant/__init__.py` & `onediff-1.0.0.dev202405030127/src/infer_compiler_registry/register_onediff_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/__init__.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/backends/oneflow.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/backends/oneflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/backends/registry.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/backends/registry.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/import_tools/format_utils.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/import_tools/format_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/import_tools/import_module_utils.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/import_tools/import_module_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/import_tools/importer.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/import_tools/importer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/oneflow/config.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/oneflow/config.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/oneflow/deployable_module.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/oneflow/deployable_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/oneflow/dual_module.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/oneflow/dual_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/oneflow/graph.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/oneflow/graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/oneflow/utils.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/oneflow/utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/transform/builtin_transform.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/transform/builtin_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/transform/custom_transform.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/transform/custom_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/transform/manager.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/transform/manager.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/transform/patch_for_comfy.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/transform/patch_for_comfy.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/args_tree_util.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/args_tree_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/cost_util.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/cost_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/env_var.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/graph_management_utils.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/graph_management_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/log_utils.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/model_inplace_assign.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/model_inplace_assign.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/module_operations.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/module_operations.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/oneflow_exec_mode.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/online_quantization_utils.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/online_quantization_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/options.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/options.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/param_utils.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/param_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/patch_for_compiler.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/patch_for_compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/patch_for_diffusers.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/patch_for_diffusers.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/utils/version_util.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/utils/version_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/with_fx_graph.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/with_fx_graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/infer_compiler/with_fx_interpreter.py` & `onediff-1.0.0.dev202405030127/src/onediff/infer_compiler/with_fx_interpreter.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/optimization/attention_processor.py` & `onediff-1.0.0.dev202405030127/src/onediff/optimization/attention_processor.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/optimization/quant_optimizer.py` & `onediff-1.0.0.dev202405030127/src/onediff/optimization/quant_optimizer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/optimization/rewrite_self_attention.py` & `onediff-1.0.0.dev202405030127/src/onediff/optimization/rewrite_self_attention.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/quantization/load_quantized_model.py` & `onediff-1.0.0.dev202405030127/src/onediff/quantization/load_quantized_model.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/quantization/quant_pipeline_test.py` & `onediff-1.0.0.dev202405030127/src/onediff/quantization/quant_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/quantization/quantize_pipeline.py` & `onediff-1.0.0.dev202405030127/src/onediff/quantization/quantize_pipeline.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff/quantization/quantize_utils.py` & `onediff-1.0.0.dev202405030127/src/onediff/quantization/quantize_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/src/onediff.egg-info/PKG-INFO` & `onediff-1.0.0.dev202405030127/src/onediff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.0.0.dev202405020126
+Version: 1.0.0.dev202405030127
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405020126 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405030127 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `onediff-1.0.0.dev202405020126/src/onediff.egg-info/SOURCES.txt` & `onediff-1.0.0.dev202405030127/src/onediff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/tests/test_dual_module_list.py` & `onediff-1.0.0.dev202405030127/tests/test_dual_module_list.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/tests/test_pipelines_oneflow_img2img.py` & `onediff-1.0.0.dev202405030127/tests/test_pipelines_oneflow_img2img.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/tests/test_quantitative_quality.py` & `onediff-1.0.0.dev202405030127/tests/test_quantitative_quality.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405020126/tests/test_quantize_custom_model.py` & `onediff-1.0.0.dev202405030127/tests/test_quantize_custom_model.py`

 * *Files identical despite different names*

