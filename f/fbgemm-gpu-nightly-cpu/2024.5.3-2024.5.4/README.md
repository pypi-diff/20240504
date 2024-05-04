# Comparing `tmp/fbgemm_gpu_nightly_cpu-2024.5.3-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2024.5.4-cp38-cp38-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,57 +1,57 @@
-Zip file size: 3139602 bytes, number of entries: 55
--rw-r--r--  2.0 unx      914 b- defN 24-May-03 12:59 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx     3079 b- defN 24-May-03 12:59 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      789 b- defN 24-May-03 12:59 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 10846712 b- defN 24-May-03 12:59 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5663 b- defN 24-May-03 12:59 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2362 b- defN 24-May-03 12:59 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2752 b- defN 24-May-03 12:59 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7885 b- defN 24-May-03 12:59 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4143 b- defN 24-May-03 12:59 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     6947 b- defN 24-May-03 12:59 fbgemm_gpu/runtime_monitor.py
--rw-r--r--  2.0 unx    20601 b- defN 24-May-03 12:59 fbgemm_gpu/sparse_ops.py
--rw-r--r--  2.0 unx     5774 b- defN 24-May-03 12:59 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     7058 b- defN 24-May-03 12:59 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx      540 b- defN 24-May-03 12:59 fbgemm_gpu/split_embedding_optimizer_ops.py
--rw-r--r--  2.0 unx    26853 b- defN 24-May-03 12:59 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2339 b- defN 24-May-03 12:59 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     3493 b- defN 24-May-03 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    66800 b- defN 24-May-03 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx    98158 b- defN 24-May-03 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    40680 b- defN 24-May-03 12:59 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      925 b- defN 24-May-03 12:59 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx      383 b- defN 24-May-03 12:59 fbgemm_gpu/docs/__init__.py
--rw-r--r--  2.0 unx      273 b- defN 24-May-03 12:59 fbgemm_gpu/docs/common.py
--rw-r--r--  2.0 unx     2377 b- defN 24-May-03 12:59 fbgemm_gpu/docs/examples.py
--rw-r--r--  2.0 unx     7381 b- defN 24-May-03 12:59 fbgemm_gpu/docs/jagged_tensor_ops.py
--rw-r--r--  2.0 unx     7708 b- defN 24-May-03 12:59 fbgemm_gpu/docs/table_batched_embedding_ops.py
--rw-r--r--  2.0 unx      263 b- defN 24-May-03 12:59 fbgemm_gpu/docs/version.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4180 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     4180 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
--rw-r--r--  2.0 unx     3395 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     3395 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
--rw-r--r--  2.0 unx     2147 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     3395 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     3395 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
--rw-r--r--  2.0 unx     3144 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     3144 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
--rw-r--r--  2.0 unx     2420 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     2420 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
--rw-r--r--  2.0 unx     3100 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     3100 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
--rw-r--r--  2.0 unx     3100 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     3100 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
--rw-r--r--  2.0 unx     4512 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     4512 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
--rw-r--r--  2.0 unx     3964 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     3964 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
--rw-r--r--  2.0 unx     3762 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     3762 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
--rw-r--r--  2.0 unx      649 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
--rw-r--r--  2.0 unx     6162 b- defN 24-May-03 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
--rw-r--r--  2.0 unx     2601 b- defN 24-May-03 12:59 fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 24-May-03 12:59 fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-03 12:59 fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6018 b- defN 24-May-03 12:59 fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/RECORD
-55 files, 11261955 bytes uncompressed, 3129522 bytes compressed:  72.2%
+Zip file size: 3139604 bytes, number of entries: 55
+-rw-r--r--  2.0 unx      914 b- defN 24-May-04 12:56 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx     3079 b- defN 24-May-04 12:56 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      789 b- defN 24-May-04 12:56 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 10846712 b- defN 24-May-04 12:56 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5663 b- defN 24-May-04 12:56 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2362 b- defN 24-May-04 12:56 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2752 b- defN 24-May-04 12:56 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7885 b- defN 24-May-04 12:56 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4143 b- defN 24-May-04 12:56 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     6947 b- defN 24-May-04 12:56 fbgemm_gpu/runtime_monitor.py
+-rw-r--r--  2.0 unx    20601 b- defN 24-May-04 12:56 fbgemm_gpu/sparse_ops.py
+-rw-r--r--  2.0 unx     5774 b- defN 24-May-04 12:56 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     7058 b- defN 24-May-04 12:56 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx      540 b- defN 24-May-04 12:56 fbgemm_gpu/split_embedding_optimizer_ops.py
+-rw-r--r--  2.0 unx    26853 b- defN 24-May-04 12:56 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2339 b- defN 24-May-04 12:56 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     3493 b- defN 24-May-04 12:56 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    66800 b- defN 24-May-04 12:56 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx    98158 b- defN 24-May-04 12:56 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    40680 b- defN 24-May-04 12:56 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      925 b- defN 24-May-04 12:56 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx      383 b- defN 24-May-04 12:56 fbgemm_gpu/docs/__init__.py
+-rw-r--r--  2.0 unx      273 b- defN 24-May-04 12:56 fbgemm_gpu/docs/common.py
+-rw-r--r--  2.0 unx     2377 b- defN 24-May-04 12:56 fbgemm_gpu/docs/examples.py
+-rw-r--r--  2.0 unx     7381 b- defN 24-May-04 12:56 fbgemm_gpu/docs/jagged_tensor_ops.py
+-rw-r--r--  2.0 unx     7708 b- defN 24-May-04 12:56 fbgemm_gpu/docs/table_batched_embedding_ops.py
+-rw-r--r--  2.0 unx      263 b- defN 24-May-04 12:56 fbgemm_gpu/docs/version.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4180 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     4180 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
+-rw-r--r--  2.0 unx     2147 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
+-rw-r--r--  2.0 unx     3144 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     3144 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
+-rw-r--r--  2.0 unx     2420 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     2420 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
+-rw-r--r--  2.0 unx     4512 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4512 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3964 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     3964 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
+-rw-r--r--  2.0 unx     3762 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     3762 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
+-rw-r--r--  2.0 unx      649 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
+-rw-r--r--  2.0 unx     6162 b- defN 24-May-04 12:54 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     2601 b- defN 24-May-04 12:56 fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 24-May-04 12:56 fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-04 12:56 fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6018 b- defN 24-May-04 12:56 fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/RECORD
+55 files, 11261955 bytes uncompressed, 3129524 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -147,20 +147,20 @@
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/fbgemm_gpu_py.so

### strings --all --bytes=8 {}

```diff
@@ -15976,53 +15976,53 @@
 SymFloat
 GenericList
 PyObject
 Uninitialized
 Quantizer
 Generator
 InvalidTag(
-extra_meta_ && extra_meta_->symbolic_shape_meta_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1723, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h
+extra_meta_ && extra_meta_->symbolic_shape_meta_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/TensorImpl.h":1723, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/TensorImpl.h
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/training/forward/embedding_forward_split_cpu.cpp
 Expected !indice_weights.defined() || indice_weights.scalar_type() != at::kHalf to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 split_embedding_codegen_forward_cpu_meta
 split_embedding_codegen_forward_cpu(Tensor weights, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, Tensor hash_size_cumsum, Tensor indices, Tensor offsets, int pooling_mode, Tensor indice_weights, int output_dtype) -> Tensor
 Expected weights.is_contiguous() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 split_embedding_forward_cpu_kernel
 split_embedding_grad_indice_weights_cpu_outer
 split_embedding_grad_indice_weights_cpu
 split_embedding_codegen_grad_indice_weights_cpu(Tensor grad_output, Tensor weights, Tensor weights_offsets, Tensor D_offsets, Tensor indices, Tensor offsets, Tensor feature_requires_grad) -> Tensor
 tensor does not have a device
 device_default
 There is an error in the layout calculation logic.
-is_mkldnn() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1290, please report a bug to PyTorch. 
+is_mkldnn() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/TensorImpl.h":1290, please report a bug to PyTorch. 
 Operators taking TensorOptions cannot take a TensorOptions with options.requires_grad set as true. This isn't implemented yet.
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/CheckMemoryFormat.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/CheckMemoryFormat.h
 check_tensor_options_and_extract_memory_format
 Cannot set memory_format both in TensorOptions and explicit argument; please delete the redundant setter.
 basic_string::_S_construct null not valid
 basic_string::append
 IntArrayRef contains an int that cannot be represented as a SymInt: 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymIntArrayRef.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymIntArrayRef.h
 fromIntArrayRefSlow
  dims but tensor has 
 TensorAccessor expected 
 accessor
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/TensorBase.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/TensorBase.h
  is out of bounds: 
 , range 
 report_embedding_error
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/include/fbgemm_gpu/cpu_utils.h
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h
-0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":652, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h
+0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":652, please report a bug to PyTorch. 
 expected int
 vector::_M_realloc_insert
 Expected SymInt or int but got 
-isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":237, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h
+isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":237, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h
 toSymInt
 St19bad_optional_access
 N3c1020intrusive_ptr_targetE
 N3c1014OperatorKernelE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_S5_S5_S5_EXadL_Z47split_embedding_codegen_grad_indice_weights_cpuS5_S5_S5_S5_S5_S5_S5_EEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_S5_S5_EEEEE
 FN2at6TensorES0_S0_S0_S0_S0_S0_S0_E
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_NS_6SymIntES5_S5_S5_lS5_lEXadL_Z35split_embedding_codegen_forward_cpuS5_S5_S5_S6_S5_S5_S5_lS5_lEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S6_S5_S5_S5_lS5_lEEEEE
@@ -16050,133 +16050,133 @@
 TensorQueue
 Expected GenericDict but got 
 toGenericDict
 Unknown Exception Type
  devices
 getDeviceGuardImpl
 PyTorch is not linked with support for 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/impl/DeviceGuardImplInterface.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/impl/DeviceGuardImplInterface.h
 Event device type 
  does not match blocking stream's device type 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/impl/InlineEvent.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/impl/InlineEvent.h
 Expected !name.empty() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/qualified_name.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/qualified_name.h
 Invalid name for qualified name: '
-!atom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/qualified_name.h":24, please report a bug to PyTorch. 
-!finalAtom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/qualified_name.h":32, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/util/ArrayRef.h
+!atom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/qualified_name.h":24, please report a bug to PyTorch. 
+!finalAtom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/qualified_name.h":32, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/util/ArrayRef.h
 QualifiedName
 basic_string::substr
 ArrayRef: invalid slice, N = 
 ; size = 
 Expected a 0-dim Tensor, but got Tensor with dimensions: 
-tensor.dim() == 0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":317, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h
+tensor.dim() == 0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":317, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h
  in its first dimension, but got Tensor with size 
-tensor.sizes()[0] == (int64_t)init_list_.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":324, please report a bug to PyTorch. 
+tensor.sizes()[0] == (int64_t)init_list_.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":324, please report a bug to PyTorch. 
 TensorDataContainer is already a Tensor type, `fill_tensor` should not be called
-false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":338, please report a bug to PyTorch. 
+false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":338, please report a bug to PyTorch. 
 Invalid TensorDataContainer type
-false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":342, please report a bug to PyTorch. 
+false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":342, please report a bug to PyTorch. 
 fill_tensor
 Expected a Tensor with size 
  in its first dimension
 can not do torch::tensor(complex, dtype=non-complex) because complex can not be casted to real number without loss of information
-false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":272, please report a bug to PyTorch. 
+false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":272, please report a bug to PyTorch. 
 convert_to_tensor
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/inference/embedding_forward_quantized_host_cpu.cpp
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function shouldn't be called for CPU; it is only for GPU.
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1972, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1972, please report a bug to PyTorch. 
 vector::_M_range_check: __n (which is %zu) >= this->size() (which is %zu)
 __getstate__ should take exactly one argument: self. Got: 
 self argument of __getstate__ must be the custom class type. Got 
 __getstate__ should return exactly one value for serialization. Got: 
 __getstate__'s return type should be a subtype of input argument of __setstate__. Got 
-isString() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2362, please report a bug to PyTorch. 
+isString() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2361, please report a bug to PyTorch. 
 //deeplearning/fbgemm/fbgemm_gpu:sparse_ops_py
 int_nbit_split_embedding_codegen_lookup_function(Tensor dev_weights, Tensor uvm_weights, Tensor weights_placements, Tensor weights_offsets, Tensor weights_tys, Tensor D_offsets, SymInt total_D, int max_int2_D, int max_int4_D, int max_int8_D, int max_float16_D, int max_float32_D, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, int output_dtype=1, Tensor? lxu_cache_weights=None, Tensor? lxu_cache_locations=None, int? row_alignment = None, int? max_float8_D=0, int? fp8_exponent_bits=-1, int? fp8_exponent_bias=-1) -> Tensor
 int_nbit_split_embedding_codegen_lookup_function
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function(Tensor dev_weights, Tensor uvm_weights, Tensor weights_placements, Tensor weights_offsets, Tensor weights_tys, Tensor D_offsets, SymInt total_D, int max_int2_D, int max_int4_D, int max_int8_D, int max_float16_D, int max_float32_D, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights=None, int output_dtype=1, Tensor? lxu_cache_weights=None, Tensor? lxu_cache_locations=None, int? row_alignment=-1, int? max_float8_D=0, int? fp8_exponent_bits=-1, int? fp8_exponent_bias=-1, Tensor? cache_hash_size_cumsum=None, int? total_cache_hash_size=-1, Tensor? cache_index_table_map=None, Tensor? lxu_cache_state=None, Tensor? lxu_state=None) -> Tensor
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function
 pruned_hashmap_insert(Tensor indices, Tensor dense_indices, Tensor offsets, Tensor(a!) hash_table, Tensor hash_table_offsets) -> ()
 pruned_hashmap_lookup(Tensor indices, Tensor offsets, Tensor hash_table, Tensor hash_table_offsets) -> Tensor
 pruned_array_lookup(Tensor indices, Tensor offsets, Tensor index_remappings, Tensor index_remappings_offsets) -> Tensor
-isGenericDict() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2088, please report a bug to PyTorch. 
-self_impl INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h":305, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h
+isGenericDict() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2088, please report a bug to PyTorch. 
+self_impl INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/variable.h":305, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/variable.h
 Only Tensors of floating point and complex dtype can require gradients
 AutogradMeta
 set_requires_grad
 Expected T > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected B > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected maps_.size() == T to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 , got one on device 
 getDevicesOfStorages
 Expected all data ptrs to be on a device of type 
 vector::reserve
 Expected map.size() == (table_offsets_acc[t + 1] - table_offsets_acc[t]) to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 serialize
 table_offsets
 vector::_M_fill_insert
-schema_.returns().size() == 1 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/builtin_function.h":22, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/builtin_function.h
+schema_.returns().size() == 1 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/builtin_function.h":22, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/builtin_function.h
 BuiltinOpFunction
 defineMethod
 Default values must be specified for none or all arguments
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/custom_class.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/custom_class.h
 TensorImpl with nullptr is not supported
 vector::_M_default_append
 cannot create std::deque larger than max_size()
 *ZN5torch6class_I12PrunedMapCPUE12defineMethodIZNS2_10def_pickleINL20PrunedMapCPURegistryMUlRKN3c1013intrusive_ptrIS1_NS5_6detail34intrusive_target_default_null_typeIS1_EEEEE_ENL20PrunedMapCPURegistryMUlSsE0_EEERS2_OT_OT0_EUlNS5_14tagged_capsuleIS1_EEOSsE_EEPNS_3jit8FunctionESsSG_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS5_6IValueESaISV_EEE_
 *ZN5torch6class_I13AtomicCounterE12defineMethodIZNS2_10def_pickleINL21AtomicCounterRegistryMUlRKN3c1013intrusive_ptrIS1_NS5_6detail34intrusive_target_default_null_typeIS1_EEEEE_ENL21AtomicCounterRegistryMUlSsE0_EEERS2_OT_OT0_EUlNS5_14tagged_capsuleIS1_EEOSsE_EEPNS_3jit8FunctionESsSG_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS5_6IValueESaISV_EEE_
 *ZN5torch6class_I11TensorQueueE12defineMethodIZNS2_10def_pickleINL19TensorQueueRegistryMUlRKN3c1013intrusive_ptrIS1_NS5_6detail34intrusive_target_default_null_typeIS1_EEEEE_ENL19TensorQueueRegistryMUlNS5_4DictISsN2at6TensorEEEE0_EEERS2_OT_OT0_EUlNS5_14tagged_capsuleIS1_EEOSH_E_EEPNS_3jit8FunctionESsSK_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS5_6IValueESaISZ_EEE_
 *ZN5torch6class_I12PrunedMapCPUE12defineMethodINL20PrunedMapCPURegistryMUlRKN3c1013intrusive_ptrIS1_NS4_6detail34intrusive_target_default_null_typeIS1_EEEEE_EEEPNS_3jit8FunctionESsT_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS4_6IValueESaISL_EEE_
 *ZN5torch6class_I13AtomicCounterE12defineMethodINL21AtomicCounterRegistryMUlRKN3c1013intrusive_ptrIS1_NS4_6detail34intrusive_target_default_null_typeIS1_EEEEE_EEEPNS_3jit8FunctionESsT_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS4_6IValueESaISL_EEE_
 *ZN5torch6class_I11TensorQueueE12defineMethodINL19TensorQueueRegistryMUlRKN3c1013intrusive_ptrIS1_NS4_6detail34intrusive_target_default_null_typeIS1_EEEEE_EEEPNS_3jit8FunctionESsT_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS4_6IValueESaISL_EEE_
 Expected Object but got 
 toObject
-isObject() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":133, please report a bug to PyTorch. 
+isObject() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":133, please report a bug to PyTorch. 
 Argument passed to at() was not in the map.
 init_tensor
 Streams have a mix of device types: stream 0 is on 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/impl/InlineStreamGuard.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/impl/InlineStreamGuard.h
  while stream 
  is on device 
 getDeviceTypeOfStreams
 , trying to set error: 
 setErrorInternal
 Error already set on this Future: 
 Future is already marked completed
-!completed() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1221, please report a bug to PyTorch. 
+!completed() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1221, please report a bug to PyTorch. 
  which are not among the expected device(s) 
 The result contained tensors residing on device(s) 
 Attempting to mark a completed Future as complete again. Note that a Future can only be marked completed once.
  does not match recording stream's device type 
 ensureIsSubsetOfDevices
 markCompleted
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::intrusive_ptr<TensorQueue>; c10::string_view = c10::basic_string_view<char>]
  could not be converted to any of the known types.
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/jit_type.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/jit_type.h
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::tagged_capsule<TensorQueue>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::intrusive_ptr<AtomicCounter>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::tagged_capsule<AtomicCounter>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::intrusive_ptr<PrunedMapCPU>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::tagged_capsule<PrunedMapCPU>; c10::string_view = c10::basic_string_view<char>]
 Tried to cast IValue to custom class but it did not contain a custom class!
-isCapsule() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":225, please report a bug to PyTorch. 
+isCapsule() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":225, please report a bug to PyTorch. 
 toCustomClass
 toCapsule
 Tried to cast a Dict<
 > to a Dict<
 >. Key types mismatch.
 toTypedDict
 >. Value types mismatch.
-*getTypePtr<Key>() == *dict.impl_->elementTypes.keyType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/Dict_inl.h":26, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/Dict_inl.h
-*getTypePtr<Value>() == *dict.impl_->elementTypes.valueType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/Dict_inl.h":27, please report a bug to PyTorch. 
+*getTypePtr<Key>() == *dict.impl_->elementTypes.keyType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/Dict_inl.h":26, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/Dict_inl.h
+*getTypePtr<Value>() == *dict.impl_->elementTypes.valueType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/Dict_inl.h":27, please report a bug to PyTorch. 
 N3c105ErrorE
 N3c1010ValueErrorE
 N3c1011StorageImplE
 N3c1015VariableVersion14VersionCounterE
 N3c104impl24DeviceGuardImplInterfaceE
 N3c106detail8ListImplE
 N5torch17CustomClassHolderE
@@ -16222,37 +16222,37 @@
 pooling_mode
 function 
 apply_with_saved
 missing before())
 vector<bool>::_M_insert_aux
 Please open a feature request on GitHub if you need this.
 jvp is not implemented for the c++ API of custom Function yet.
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h
 compiled_args not implemented for non-traceable node: 
 dense_embedding_codegen_lookup_function(Tensor dev_weights, Tensor weights_offsets, Tensor D_offsets, int total_D, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, int output_dtype=0) -> Tensor
 dense_embedding_codegen_lookup_function
 Cannot update a node's topological_nr after it already has a parent. If we allow this, we can no longer guarantee that a parent's topo_nr is always greater than those of all its children
-!has_parent_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/function.h":262, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/function.h
+!has_parent_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/function.h":262, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/function.h
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/training/backward/embedding_backward_dense_host_cpu.cpp
 Check failed: grad_outputs.size() == 1 (
  returned an incorrect number of gradients (expected 
  returned a gradient different that is defined at position 
 , but the corresponding forward input was not a Variable
-ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":221, please report a bug to PyTorch. 
-ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":222, please report a bug to PyTorch. 
-it != _saved_variables.end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":138, please report a bug to PyTorch. 
-arg.proxy_tensor.defined() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":561, please report a bug to PyTorch. 
-ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":224, please report a bug to PyTorch. 
-it != this->end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":760, please report a bug to PyTorch. 
-ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":231, please report a bug to PyTorch. 
-ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":232, please report a bug to PyTorch. 
-ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":234, please report a bug to PyTorch. 
-sym_sizes_index < sym_sizes.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":531, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h
+ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":221, please report a bug to PyTorch. 
+ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":222, please report a bug to PyTorch. 
+it != _saved_variables.end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":138, please report a bug to PyTorch. 
+arg.proxy_tensor.defined() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":561, please report a bug to PyTorch. 
+ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":224, please report a bug to PyTorch. 
+it != this->end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":760, please report a bug to PyTorch. 
+ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":231, please report a bug to PyTorch. 
+ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":232, please report a bug to PyTorch. 
+ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":234, please report a bug to PyTorch. 
+sym_sizes_index < sym_sizes.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":531, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h
 next_sym_size
 PFvPN5torch8autograd4NodeEE
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEE5applyIS3_JRN2at6TensorES8_S8_RlS9_S8_S9_S8_S8_S9_RSt8optionalIS7_ESC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSE_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSF_EUlRKSt6vectorIS7_SaIS7_EESP_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEE5applyIS3_JRN2at6TensorES8_S8_RlS9_S8_S9_S8_S8_S9_RSt8optionalIS7_ESC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSE_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSF_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_llS5_lS5_S5_lSt8optionalIS5_ES7_lEXadL_ZN12_GLOBAL__N_145split_embedding_codegen_lookup_dense_functionES5_S5_S5_llS5_lS5_S5_lS7_S7_lEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_llS5_lS5_S5_lS7_S7_lEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
@@ -16295,17 +16295,17 @@
 sum_reduce_to_one
 merge_pooled_embeddings
 t must be a CPU tensor; it is currently on device 
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/merge_pooled_embedding_ops/merge_pooled_embedding_ops_cpu.cpp
 Expected input_tensors.size() > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 input_0 must be a CPU tensor; it is currently on device 
 input_tensors[i] must be a CPU tensor; it is currently on device 
-isDevice() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":931, please report a bug to PyTorch. 
-isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2040, please report a bug to PyTorch. 
-isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2044, please report a bug to PyTorch. 
+isDevice() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":931, please report a bug to PyTorch. 
+isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2040, please report a bug to PyTorch. 
+isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2044, please report a bug to PyTorch. 
 toDevice
 Expected TensorList but got 
 toTensorList
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorESt6vectorIS5_SaIS5_EElNS_6DeviceElEXadL_ZN10fbgemm_gpu27merge_pooled_embeddings_cpuES8_lS9_lEEEES5_NS_4guts8typelist8typelistIJS8_lS9_lEEEEE
 FN2at6TensorESt6vectorIS0_SaIS0_EElN3c106DeviceElE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorESt6vectorIS5_SaIS5_EENS_6DeviceEEXadL_ZN10fbgemm_gpu21sum_reduce_to_one_cpuES8_S9_EEEES5_NS_4guts8typelist8typelistIJS8_S9_EEEEE
 FN2at6TensorESt6vectorIS0_SaIS0_EEN3c106DeviceEE
@@ -16314,21 +16314,21 @@
 merge_pooled_embeddings(Tensor[] pooled_embeddings, SymInt uncat_dim_size, Device target_device, SymInt cat_dim=all_to_one_device(Tensor[] input_tensors, Device target_device) sum_reduce_to_onfbgemm::permute_pooled_embs
 expected bool
 fbgemm::permute_duplicate_pooled_embs
 offset_dim_list needs to have long/int64 type
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/permute_pooled_embedding_ops/permute_pooled_embedding_function.cpp
 permute_list needs to have long/int64 type
 Expected ptr_->is_bool() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymBool.h
-0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":676, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymBool.h
+0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":676, please report a bug to PyTorch. 
 permute_pooled_embs does not support allow_duplicates in backward!
 Tried to access the schema for 
  which doesn't have a schema registered yet
-schema_.has_value() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h":80, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h
+schema_.has_value() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h":80, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h
 FN2at6TensorERKS0_S2_S2_S2_S2_E
 inv_offset_dim_linv_permute_listallow_duplicatespermute_pooled_embs_cpu_impl
 permute_pooled_embs_auto_grad
 permute_duplicate_pooled_embs
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/permute_pooled_embedding_ops/permute_pooled_embedding_ops_cpu.cpp
 permute_duplicate_pooled_embs_auto_grad
 N5torch8autograd7CppNodeIN10fbgemm_gpu25PermutePooledEmbsFunctionEEE
@@ -16386,27 +16386,27 @@
 num_output_rows
 slice_length
 fbgemm::jagged_slice_forward
 lengths is currently on 
 start should be <= len
 jagged_dense_dense_elementwise_add_jagged_output
 batched_dense_vec_jagged_2d_mul
-isList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2072, please report a bug to PyTorch. 
+isList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2072, please report a bug to PyTorch. 
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/jagged_tensor_ops/jagged_tensor_ops_autograd.cpp
 Expected grad_outputs.size() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected total_L >= 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 fbgemm::jagged_to_padded_dense_backward
 fbgemm::jagged_to_padded_dense_forward
 Expected values.dim() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected offsets.dim() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected max_L > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected max_lengths.size() == x_offsets.size() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected SymIntList or IntList but got 
-isSymIntList() || isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1984, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h
+isSymIntList() || isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1984, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymInt.h
 Expected dense_values_grad.sym_sizes() == dense_shape to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 fbgemm::jagged_dense_dense_elementwise_add_jagged_output_forward
 fbgemm::jagged_dense_elementwise_mul_backward
 fbgemm::jagged_dense_elementwise_mul_forward
 fbgemm::batched_dense_vec_jagged_2d_mul_backward
 fbgemm::batched_dense_vec_jagged_2d_mul_forward
 fbgemm::dense_to_jagged_forward
@@ -16426,15 +16426,15 @@
 fbgemm::jagged_index_select_2d_forward_v2
 output_lengths is currently on 
 grad must be on the same device as output_lengths! grad is currently on 
 Tensor 'values' must have 1 dimension(s). Found 
 values must be on the same device as lengths! values is currently on 
 start should be always be positive
 type with contained types did not overload createWithContained: 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/jit_type_base.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/jit_type_base.h
 createWithContained
 ; Length = 
 ArrayRef: invalid index Index = 
  with None type
 Can not create 
 : SymIntArrayRef expected to contain only concrete integers
 asIntArrayRefSlow
@@ -16480,24 +16480,24 @@
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_115DenseToJaggedOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_136JaggedDenseElementwiseAddJaggedOutOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_115JaggedSoftmaxOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_117JaggedJaggedBmmOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_116JaggedDenseBmmOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_121JaggedIndexSelect2dOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_113JaggedSliceOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
-isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":245, please report a bug to PyTorch. 
+isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":245, please report a bug to PyTorch. 
 Tried to cast a List<
 > to a List<
 >. Types mismatch.
 toTypedList
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/List_inl.h
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/boxing/KernelFunction_impl.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/List_inl.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/boxing/KernelFunction_impl.h
 Expected ptr_->is_float() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymFloat.h
-0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":540, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymFloat.h
+0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":540, please report a bug to PyTorch. 
 expected double
 toDouble
 St23enable_shared_from_thisIN3c1010SharedTypeEE
 N3c1010SharedTypeE
 N3c1017SingleElementTypeILNS_8TypeKindE6ENS_8ListTypeEEE
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EEN3c108ArrayRefINS8_6SymIntEEEdE
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EEN3c108ArrayRefIlEEdE
@@ -16692,15 +16692,15 @@
 jagged_jagged_elementwise_dense_output_kernel_
 Expected !NO_INNER_DENSE || output.size(-1) == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 unsupported number of jagged dim 
 jagged_2d_to_dense_forward_cpu
 jagged_2d_to_dense_backward_kernel
 fbgemm::jagged_index_select_2d_forward
 fbgemm::jagged_index_add_2d_forward
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1968, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1968, please report a bug to PyTorch. 
 FN2at6TensorERKS0_S2_S2_S2_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_RKSt6vectorIS5_SaIS5_EES7_EXadL_ZN10fbgemm_gpu28jagged_dense_elementwise_addES7_SC_S7_EEEES5_NS_4guts8typelist8typelistIJS7_SC_S7_EEEEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFSt6vectorIN2at6TensorESaIS6_EES6_S6_RKS4_IlSaIlEESC_lEXadL_ZN10fbgemm_gpu30stacked_jagged_1d_to_dense_cpuES6_S6_SC_SC_lEEEES8_NS_4guts8typelist8typelistIJS6_S6_SC_SC_lEEEEE
 FSt6vectorIN2at6TensorESaIS1_EES1_S1_RKS_IlSaIlEES7_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFSt6vectorIN2at6TensorESaIS6_EES6_S6_RKS4_IlSaIlEESC_lEXadL_ZN10fbgemm_gpu30stacked_jagged_2d_to_dense_cpuES6_S6_SC_SC_lEEEES8_NS_4guts8typelist8typelistIJS6_S6_SC_SC_lEEEEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_lEXadL_ZN10fbgemm_gpu34jagged_index_select_2d_forward_cpuES7_S7_S7_S7_lEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_lEEEEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_llEXadL_ZN10fbgemm_gpu31jagged_index_add_2d_forward_cpuES7_S7_S7_S7_llEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_llEEEEE
@@ -17208,15 +17208,15 @@
 FvN2at6TensorES0_lS0_S0_S0_S0_S0_S0_S0_S0_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_lbSt8optionalIS5_ES7_S7_EXadL_ZN10fbgemm_gpu20lxu_cache_lookup_cpuES5_S5_lbS7_S7_S7_EEEES5_NS_4guts8typelist8typelistIJS5_S5_lbS7_S7_S7_EEEEE
 FN2at6TensorES0_S0_lbSt8optionalIS0_ES2_S2_E
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_lbSt8optionalIS5_EEXadL_ZN10fbgemm_gpu34direct_mapped_lxu_cache_lookup_cpuES5_S5_lbS7_EEEES5_NS_4guts8typelist8typelistIJS5_S5_lbS7_EEEEE
 FN2at6TensorES0_S0_lbSt8optionalIS0_EE
 linearize_cache_indices(Tensor cache_hash_size_cumsum, Tensor indices, Tensor offsets, Tensor? B_offsets=None, int max_B=-1) -> indices_from_row_idx(Tensor cache_hash_size_cumsum, Tensor update_table_indices, Tensor update_row_indices) -> Tdirect_mapped_lxu_cache_lookup(Tensor linear_cache_indices, Tensor lxu_cache_state, int invalid_index = -1, bool gather_cache_stats=False, Tensor(a!)? uvm_cache_stats=None) -> lxu_cache_slot(int h_in, int C) lxu_cache_locking_counter_decrement(Tensor(a!) lxu_cache_locking_counter, Tensor lxu_cache_locatget_unique_indices(Tensor linear_indices, int max_indices, bool compute_count) -> (Tensor, Tensobatch_index_select_dim0
 batch_index_select_dim0_cpu
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1976, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1976, please report a bug to PyTorch. 
 toIntVector
 batch_index_select_dim0(    Tensor inputs,    Tensor indices,    SymInt[] input_num_indices,    SymInt[] input_rows,    SymInt[] input_columns,    bool permute_output_dim_0_1=False) -> Tensor
 [batch_index_select_dim0] input_rows must have the same length as input_num_indices.
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/training/index_select/batch_index_select_dim0_cpu_host.cpp
 [batch_index_select_dim0] input_columns must have the same length as input_num_indices.
 Currently batch_index_select only supports 16-byte align input tensors
 [batch_index_select_dim0] All input_columns must be the same.
@@ -17234,15 +17234,15 @@
 ZN5torch8autograd8FunctionI25BatchIndexSelectDim0CPUOpE5applyIS2_JRN2at6TensorES7_RSt6vectorIlSaIlEESB_SB_RKbEEENSt9enable_ifIX9is_same_vIT_S2_EEDTclsrSF_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSG_EUlRKS6_E0_
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_St6vectorIlSaIlEES8_S8_bEXadL_Z27batch_index_select_dim0_cpuS5_S5_S8_S8_S8_bEEEES5_NS_4guts8typelist8typelistIJS5_S5_S8_S8_S8_bEEEEE
 FN2at6TensorES0_S0_St6vectorIlSaIlEES3_S3_bE
 St19_Sp_counted_deleterIPN5torch8autograd7CppNodeI25BatchIndexSelectDim0CPUOpEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 Unsupported SparseType: 
 pruned_array_lookup_cpu
 Expected placement != PlacementType::DEVICE to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_forward_quantized_unweighted_codegen_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_forward_quantized_unweighted_codegen_cpu.cpp
 int8 output are only supported for int8 weights
 Expected offsets_nobag.numel() == index_size + 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected offsets_nobag_ptr[index_size] - offsets_nobag_ptr[0] == index_size to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 int_nbit_split_embedding_codegen_forward_unweighted_cpu
 Expected B >= 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected total_D > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Enabling both CUDA and HIP in ATen is not supported, as HIP masquerades to be CUDA (e.g., when you say CUDA, on a HIP build of ATen, this actually means HIP.  Rebuild PyTorch with one or the other disabled.
@@ -17255,30 +17255,30 @@
 int_nbit_split_embedding_nobag_codegen_forward_
 "intn_split_embedding_nobag_codegen_forward_kernel"
 pruned_hashmap_lookup_unweighted_cpu
 hash_table must be a CPU tensor; it is currently on device 
 hash_table_offsets must be a CPU tensor; it is currently on device 
 pruned_hashmap_insert_unweighted_cpu
 dense_indices must be a CPU tensor; it is currently on device 
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_forward_quantized_weighted_codegen_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_forward_quantized_weighted_codegen_cpu.cpp
 pruned_hashmap_lookup_weighted_cpu
 pruned_hashmap_insert_weighted_cpu
 int_nbit_split_embedding_codegen_forward_weighted_cpu
 indice_weights must be empty or a CPU tensor; it is currently on device 
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_dense_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_dense_split_cpu.cpp
 Check failed: host_weights.dim() == 1 (
 split_embedding_backward_exact_cpu
 split_embedding_backward_codegen_dense_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, float unused = 0) -> Tensor
 split_embedding_backward_codegen_dense_cpu
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_dEXadL_Z42split_embedding_backward_codegen_dense_cpuS5_S5_S5_S5_lS5_lS5_S5_lS5_dEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_lS5_lS5_S5_lS5_dEEEEE
 FN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_dE
 split_embedding_codegen_grad_indice_weights_pt2_wrapper
 split_embedding_codegen_forward_weighted_pt2_wrapper
 split_embedding_codegen_forward_unweighted_pt2_wrapper
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_forward_split_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_forward_split_pt2_cpu_wrapper.cpp
 fbgemm::split_embedding_codegen_grad_indice_weights_cpu
 fbgemm::split_embedding_codegen_forward_cpu
 FN2at6TensorES0_S0_S0_lS0_S0_S0_lS0_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_NS_6SymIntES7_S7_S7_S7_EXadL_Z59split_embedding_codegen_grad_indice_weights_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_S8_S7_S7_S7_S7_EEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_S8_S7_S7_S7_S7_EEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_N3c106SymIntES2_S2_S2_S2_E
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_NS_6SymIntES8_S7_S7_S7_lS7_S7_S7_blEXadL_Z56split_embedding_codegen_forward_weighted_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S8_S8_S7_S7_S7_lS7_S7_S7_blEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S8_S8_S7_S7_S7_lS7_S7_S7_blEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_N3c106SymIntES4_S2_S2_S2_lS2_S2_S2_blE
@@ -17286,150 +17286,150 @@
 gradient_clipping
 max_gradient
 stochastic_rounding
 output_dtype
 learning_rate
 split_embedding_codegen_lookup_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, int output_dtype=0) -> Tensor
 split_embedding_codegen_lookup_adagrad_function_cpu
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_adagrad_cpu.cpp
 fbgemm::split_embedding_backward_codegen_adagrad_cpu
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKSt6vectorIS7_SaIS7_EESU_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_ddlEXadL_ZN12_GLOBAL__N_151split_embedding_codegen_lookup_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddlEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 FvN2at6TensorES0_S0_S0_S0_N3c106SymIntES0_lS0_S0_lS0_bS0_S0_S0_ddlE
 FvN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_bS0_S0_S0_ddlE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_ddlE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_adagrad_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_adagrad_pt2_cpu_wrapper.cpp
 split_embedding_backward_codegen_adagrad_weighted_exact_pt2_wrapper
 split_embedding_backward_codegen_adagrad_unweighted_exact_pt2_wrapper
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEXadL_Z71split_embedding_backward_codegen_adagrad_weighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_lS2_lS2_S2_lS2_S2_llbllbbS0_S0_S0_S0_S0_ddlE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEXadL_Z73split_embedding_backward_codegen_adagrad_unweighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEEE
 weight_decay
 weight_decay_mode
 max_norm
 split_embedding_codegen_lookup_rowwise_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, float max_norm = 0.0, int output_dtype=0) -> Tensor
 split_embedding_codegen_lookup_rowwise_adagrad_function_cpu
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_cpu.cpp
 fbgemm::split_embedding_backward_codegen_rowwise_adagrad_cpu
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SH_SC_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKSt6vectorIS7_SaIS7_EESU_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SH_SC_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddldlEXadL_ZN12_GLOBAL__N_159split_embedding_codegen_lookup_rowwise_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddldlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddldlEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 FvN2at6TensorES0_S0_S0_S0_N3c106SymIntES0_lS0_S0_lS0_bS0_S0_S0_dddldlE
 FvN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_bS0_S0_S0_dddldlE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_dddldlE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_pt2_cpu_wrapper.cpp
 split_embedding_backward_codegen_rowwise_adagrad_weighted_exact_pt2_wrapper
 split_embedding_backward_codegen_rowwise_adagrad_unweighted_exact_pt2_wrapper
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEXadL_Z79split_embedding_backward_codegen_rowwise_adagrad_weighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_lS2_lS2_S2_lS2_S2_llbllbbS0_S0_S0_S0_S0_dddldlE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEXadL_Z81split_embedding_backward_codegen_rowwise_adagrad_unweighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEEE
 split_embedding_codegen_lookup_sgd_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, float learning_rate = 0, int output_dtype=0) -> Tensor
 split_embedding_codegen_lookup_sgd_function_cpu
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_sgd_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_sgd_cpu.cpp
 fbgemm::split_embedding_backward_codegen_sgd_cpu
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKSt6vectorIS7_SaIS7_EESU_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbdlEXadL_ZN12_GLOBAL__N_147split_embedding_codegen_lookup_sgd_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 FvN2at6TensorES0_S0_S0_S0_N3c106SymIntES0_lS0_S0_lS0_bdlE
 FvN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_bdlE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbdlE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_sgd_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_sgd_pt2_cpu_wrapper.cpp
 split_embedding_backward_codegen_sgd_weighted_exact_pt2_wrapper
 split_embedding_backward_codegen_sgd_unweighted_exact_pt2_wrapper
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEXadL_Z67split_embedding_backward_codegen_sgd_weighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_lS2_lS2_S2_lS2_S2_llbllbbdlE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEXadL_Z69split_embedding_backward_codegen_sgd_unweighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEEE
 split_embedding_codegen_lookup_adam_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_adam_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_adam_cpu.cpp
 split_embedding_codegen_lookup_adam_function_cpu
 split_embedding_codegen_lookup_adam_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_148split_embedding_codegen_lookup_adam_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_S0_S0_S0_dddddllE
 split_embedding_codegen_lookup_lamb_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_lamb_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_lamb_cpu.cpp
 split_embedding_codegen_lookup_lamb_function_cpu
 split_embedding_codegen_lookup_lamb_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_148split_embedding_codegen_lookup_lamb_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 split_embedding_codegen_lookup_partial_rowwise_adam_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_partial_rowwise_adam_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_partial_rowwise_adam_cpu.cpp
 split_embedding_codegen_lookup_partial_rowwise_adam_function_cpu
 split_embedding_codegen_lookup_partial_rowwise_adam_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_164split_embedding_codegen_lookup_partial_rowwise_adam_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_partial_rowwise_lamb_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_partial_rowwise_lamb_cpu.cpp
 split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpu
 split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_164split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 split_embedding_codegen_lookup_lars_sgd_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_lars_sgd_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_lars_sgd_cpu.cpp
 split_embedding_codegen_lookup_lars_sgd_function_cpu
 split_embedding_codegen_lookup_lars_sgd_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float learning_rate = 0, float eta = 0, float momentum = 0, float weight_decay = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_ddddlEXadL_ZN12_GLOBAL__N_152split_embedding_codegen_lookup_lars_sgd_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddddlEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_ddddlE
 split_embedding_codegen_lookup_none_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_none_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_none_cpu.cpp
 split_embedding_codegen_lookup_none_function_cpu
 split_embedding_codegen_lookup_none_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, int total_hash_size = 0, int total_unique_indices = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdblllEXadL_ZN12_GLOBAL__N_148split_embedding_codegen_lookup_none_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdblllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdblllEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdblllE
 split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_counter_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_counter_cpu.cpp
 split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpu
 split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor prev_iter_host, Tensor prev_iter_placements, Tensor prev_iter_offsets, Tensor row_counter_host, Tensor row_counter_placements, Tensor row_counter_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int iter = 0, int counter_halflife = -1, int adjustment_iter = -1, float adjustment_ub = 1.0, int learning_rate_mode = -1, int weight_decay_mode = 1, int grad_sum_decay = -1, float max_counter = 0, float tail_id_threshold = 0.0, int is_tail_id_thresh_ratio = 0, int regularization_mode = 0, float weight_norm_coefficient = 0.0, float lower_bound = 0.0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEXadL_ZN12_GLOBAL__N_172split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_S0_S0_S0_S0_S0_S0_dddllldlllddllddlE
 split_embedding_codegen_lookup_approx_sgd_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_sgd_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_sgd_cpu.cpp
 split_embedding_codegen_lookup_approx_sgd_function_cpu
 split_embedding_codegen_lookup_approx_sgd_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, float learning_rate = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbdlEXadL_ZN12_GLOBAL__N_154split_embedding_codegen_lookup_approx_sgd_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEEE
 split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_cpu.cpp
 split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpu
 split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_166split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_dddllE
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_counter_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_counter_cpu.cpp
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpu
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor prev_iter_host, Tensor prev_iter_placements, Tensor prev_iter_offsets, Tensor row_counter_host, Tensor row_counter_placements, Tensor row_counter_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int iter = 0, int counter_halflife = -1, int adjustment_iter = -1, float adjustment_ub = 1.0, int learning_rate_mode = -1, int weight_decay_mode = 1, int grad_sum_decay = -1, float max_counter = 0, float tail_id_threshold = 0.0, int is_tail_id_thresh_ratio = 0, int regularization_mode = 0, float weight_norm_coefficient = 0.0, float lower_bound = 0.0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEXadL_ZN12_GLOBAL__N_179split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEEE
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_weight_decay_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_weight_decay_cpu.cpp
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpu
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_184split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
 split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_weight_decay_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_weight_decay_cpu.cpp
 split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpu
 split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_177split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
 split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_weighted_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_weighted_adagrad_cpu.cpp
 split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpu
 split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_168split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_adagrad_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_adagrad_split_cpu.cpp
 split_embedding_backward_exact_cpu_outer
 CPU exact rowwise adagrad currently doesn't support embedding tables with more than 2B rows
 split_embedding_backward_codegen_adagrad_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, bool stochastic_rounding, Tensor(b!) momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, int output_dtype = 0) -> ()
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_ddlEXadL_Z44split_embedding_backward_codegen_adagrad_cpuS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_ddlEEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_ddlEEEEE
 does not match c_block size: 
 num of rows processed by adagrad: 
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_rowwise_adagrad_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_rowwise_adagrad_split_cpu.cpp
 split_embedding_backward_codegen_rowwise_adagrad_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, bool stochastic_rounding, Tensor(b!) momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, float max_norm = 0.0, int output_dtype = 0) -> ()
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_dddldlEXadL_Z52split_embedding_backward_codegen_rowwise_adagrad_cpuS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_dddldlEEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_dddldlEEEEE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_sgd_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_sgd_split_cpu.cpp
 split_embedding_backward_codegen_sgd_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, bool stochastic_rounding, float learning_rate = 0, int output_dtype = 0) -> ()
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_bdlEXadL_Z40split_embedding_backward_codegen_sgd_cpuS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bdlEEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bdlEEEEE
 GCC: (conda-forge gcc 10.4.0-19) 10.4.0
 .shstrtab
 .gnu.hash
 .gnu.version
 .gnu.version_r
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -983054,15 +983054,15 @@
 	mov    %r12,%rdx
 	mov    %r14,%rdi
 	lea    0x80(%rsp),%rsi
 	mov    %rax,0x80(%rsp)
 	call   1bbe30 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r14,%r8
 	lea    0x3815d2(%rip),%rcx        # 979f20 <std::__detail::__to_chars_10_impl<unsigned int>(char*, unsigned int, unsigned int)::__digits@@Base+0x1300>
-	mov    $0x93a,%edx
+	mov    $0x939,%edx
 	lea    0x37fe76(%rip),%rsi        # 9787d0 <typeinfo name for std::__future_base::_State_baseV2::_Setter<int (*)(int, unsigned long, float*, float const*, float*, int const*, float, float, int const*, float, double const*, long), int (* const&)(int, unsigned long, float*, float const*, float*, int const*, float, float, int const*, float, double const*, long)>@@Base+0x1970>
 	lea    0x380542(%rip),%rdi        # 978ea3 <std::__detail::__to_chars_10_impl<unsigned int>(char*, unsigned int, unsigned int)::__digits@@Base+0x283>
 	call   1b6cc0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    %r15,%rdi
 	call   5f7290 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor)>()@@Base+0x630>
 	jmp    5f87f9 <int_nbit_split_embedding_uvm_caching_codegen_lookup_function_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, long, long, long, long, at::Tensor, at::Tensor, long, std::optional<at::Tensor>, long, std::optional<at::Tensor>, std::optional<at::Tensor>, std::optional<long>, std::optional<long>, std::optional<long>, std::optional<long>, std::optional<at::Tensor>, std::optional<long>, std::optional<at::Tensor>, std::optional<at::Tensor>, std::optional<at::Tensor>)@@Base+0xd19>
@@ -984102,15 +984102,15 @@
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	lea    0x37f07e(%rip),%rax        # 978e8a <std::__detail::__to_chars_10_impl<unsigned int>(char*, unsigned int, unsigned int)::__digits@@Base+0x26a>
 	mov    %rax,0x40(%rsp)
 	call   1bbe30 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)@plt>
 	mov    %r15,%r8
 	lea    0x380100(%rip),%rcx        # 979f20 <std::__detail::__to_chars_10_impl<unsigned int>(char*, unsigned int, unsigned int)::__digits@@Base+0x1300>
-	mov    $0x93a,%edx
+	mov    $0x939,%edx
 	lea    0x37e9a4(%rip),%rsi        # 9787d0 <typeinfo name for std::__future_base::_State_baseV2::_Setter<int (*)(int, unsigned long, float*, float const*, float*, int const*, float, float, int const*, float, double const*, long), int (* const&)(int, unsigned long, float*, float const*, float*, int const*, float, float, int const*, float, double const*, long)>@@Base+0x1970>
 	lea    0x37f070(%rip),%rdi        # 978ea3 <std::__detail::__to_chars_10_impl<unsigned int>(char*, unsigned int, unsigned int)::__digits@@Base+0x283>
 	call   1b6cc0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopl   0x0(%rax,%rax,1)
 	call   5f6e30 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor)>()@@Base+0x1d0>
 	jmp    5f9bb9 <int_nbit_split_embedding_uvm_caching_codegen_lookup_function_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, long, long, long, long, at::Tensor, at::Tensor, long, std::optional<at::Tensor>, long, std::optional<at::Tensor>, std::optional<at::Tensor>, std::optional<long>, std::optional<long>, std::optional<long>, std::optional<long>, std::optional<at::Tensor>, std::optional<long>, std::optional<at::Tensor>, std::optional<at::Tensor>, std::optional<at::Tensor>)@@Base+0x20d9>
 	nopw   0x0(%rax,%rax,1)
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -10935,24 +10935,24 @@
   0x00977b40 78747261 5f6d6574 615f2d3e 73796d62 xtra_meta_->symb
   0x00977b50 6f6c6963 5f736861 70655f6d 6574615f olic_shape_meta_
   0x00977b60 20494e54 45524e41 4c204153 53455254  INTERNAL ASSERT
   0x00977b70 20464149 4c454420 61742022 2f676974  FAILED at "/git
   0x00977b80 6875622f 686f6d65 2f6d696e 69636f6e hub/home/minicon
   0x00977b90 64612f65 6e76732f 6275696c 645f6269 da/envs/build_bi
   0x00977ba0 6e617279 2f6c6962 2f707974 686f6e33 nary/lib/python3
-  0x00977bb0 2e392f73 6974652d 7061636b 61676573 .9/site-packages
+  0x00977bb0 2e382f73 6974652d 7061636b 61676573 .8/site-packages
   0x00977bc0 2f746f72 63682f69 6e636c75 64652f63 /torch/include/c
   0x00977bd0 31302f63 6f72652f 54656e73 6f72496d 10/core/TensorIm
   0x00977be0 706c2e68 223a3137 32332c20 706c6561 pl.h":1723, plea
   0x00977bf0 73652072 65706f72 74206120 62756720 se report a bug 
   0x00977c00 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x00977c10 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00977c20 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00977c30 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00977c40 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00977c40 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00977c50 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00977c60 64652f63 31302f63 6f72652f 54656e73 de/c10/core/Tens
   0x00977c70 6f72496d 706c2e68 00000000 00000000 orImpl.h........
   0x00977c80 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x00977c90 4d4d2f66 6267656d 6d5f6770 752f636f MM/fbgemm_gpu/co
   0x00977ca0 64656765 6e2f7472 61696e69 6e672f66 degen/training/f
   0x00977cb0 6f727761 72642f65 6d626564 64696e67 orward/embedding
@@ -11027,15 +11027,15 @@
   0x00978100 206c6179 6f757420 63616c63 756c6174  layout calculat
   0x00978110 696f6e20 6c6f6769 632e0000 00000000 ion logic.......
   0x00978120 69735f6d 6b6c646e 6e282920 494e5445 is_mkldnn() INTE
   0x00978130 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x00978140 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x00978150 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x00978160 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x00978170 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x00978170 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x00978180 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00978190 682f696e 636c7564 652f6331 302f636f h/include/c10/co
   0x009781a0 72652f54 656e736f 72496d70 6c2e6822 re/TensorImpl.h"
   0x009781b0 3a313239 302c2070 6c656173 65207265 :1290, please re
   0x009781c0 706f7274 20612062 75672074 6f205079 port a bug to Py
   0x009781d0 546f7263 682e2000 4f706572 61746f72 Torch. .Operator
   0x009781e0 73207461 6b696e67 2054656e 736f724f s taking TensorO
@@ -11044,15 +11044,15 @@
   0x00978210 6e732077 69746820 6f707469 6f6e732e ns with options.
   0x00978220 72657175 69726573 5f677261 64207365 requires_grad se
   0x00978230 74206173 20747275 652e2054 68697320 t as true. This 
   0x00978240 69736e27 7420696d 706c656d 656e7465 isn't implemente
   0x00978250 64207965 742e0000 2f676974 6875622f d yet.../github/
   0x00978260 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00978270 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00978280 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00978280 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00978290 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009782a0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x009782b0 636f7265 2f436865 636b4d65 6d6f7279 core/CheckMemory
   0x009782c0 466f726d 61742e68 00000000 00000000 Format.h........
   0x009782d0 63686563 6b5f7465 6e736f72 5f6f7074 check_tensor_opt
   0x009782e0 696f6e73 5f616e64 5f657874 72616374 ions_and_extract
   0x009782f0 5f6d656d 6f72795f 666f726d 61740000 _memory_format..
@@ -11070,51 +11070,51 @@
   0x009783b0 496e7441 72726179 52656620 636f6e74 IntArrayRef cont
   0x009783c0 61696e73 20616e20 696e7420 74686174 ains an int that
   0x009783d0 2063616e 6e6f7420 62652072 65707265  cannot be repre
   0x009783e0 73656e74 65642061 73206120 53796d49 sented as a SymI
   0x009783f0 6e743a20 00000000 2f676974 6875622f nt: ..../github/
   0x00978400 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00978410 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00978420 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00978420 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00978430 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00978440 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x00978450 6f72652f 53796d49 6e744172 72617952 ore/SymIntArrayR
   0x00978460 65662e68 0066726f 6d496e74 41727261 ef.h.fromIntArra
   0x00978470 79526566 536c6f77 00206469 6d732062 yRefSlow. dims b
   0x00978480 75742074 656e736f 72206861 73200054 ut tensor has .T
   0x00978490 656e736f 72416363 6573736f 72206578 ensorAccessor ex
   0x009784a0 70656374 65642000 61636365 73736f72 pected .accessor
   0x009784b0 00000000 00000000 2f676974 6875622f ......../github/
   0x009784c0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009784d0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009784e0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009784e0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009784f0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00978500 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00978510 636f7265 2f54656e 736f7242 6173652e core/TensorBase.
   0x00978520 68002d31 00496e64 65782000 20697320 h.-1.Index . is 
   0x00978530 6f757420 6f662062 6f756e64 733a2000 out of bounds: .
   0x00978540 2c207261 6e676520 0020746f 20007265 , range . to .re
   0x00978550 706f7274 5f656d62 65646469 6e675f65 port_embedding_e
   0x00978560 72726f72 00000000 2f5f5f77 2f464247 rror..../__w/FBG
   0x00978570 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x00978580 6d5f6770 752f696e 636c7564 652f6662 m_gpu/include/fb
   0x00978590 67656d6d 5f677075 2f637075 5f757469 gemm_gpu/cpu_uti
   0x009785a0 6c732e68 00000000 2f676974 6875622f ls.h..../github/
   0x009785b0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009785c0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009785d0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009785d0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009785e0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009785f0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00978600 636f7265 2f697661 6c75652e 68000000 core/ivalue.h...
   0x00978610 3020494e 5445524e 414c2041 53534552 0 INTERNAL ASSER
   0x00978620 54204641 494c4544 20617420 222f6769 T FAILED at "/gi
   0x00978630 74687562 2f686f6d 652f6d69 6e69636f thub/home/minico
   0x00978640 6e64612f 656e7673 2f627569 6c645f62 nda/envs/build_b
   0x00978650 696e6172 792f6c69 622f7079 74686f6e inary/lib/python
-  0x00978660 332e392f 73697465 2d706163 6b616765 3.9/site-package
+  0x00978660 332e382f 73697465 2d706163 6b616765 3.8/site-package
   0x00978670 732f746f 7263682f 696e636c 7564652f s/torch/include/
   0x00978680 4154656e 2f636f72 652f6976 616c7565 ATen/core/ivalue
   0x00978690 2e68223a 3635322c 20706c65 61736520 .h":652, please 
   0x009786a0 7265706f 72742061 20627567 20746f20 report a bug to 
   0x009786b0 5079546f 7263682e 20006578 70656374 PyTorch. .expect
   0x009786c0 65642069 6e740074 6f496e74 00766563 ed int.toInt.vec
   0x009786d0 746f723a 3a5f4d5f 7265616c 6c6f635f tor::_M_realloc_
@@ -11122,25 +11122,25 @@
   0x009786f0 2053796d 496e7420 6f722069 6e742062  SymInt or int b
   0x00978700 75742067 6f742000 69735379 6d496e74 ut got .isSymInt
   0x00978710 2829207c 7c206973 496e7428 2920494e () || isInt() IN
   0x00978720 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x00978730 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x00978740 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x00978750 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x00978760 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x00978760 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x00978770 73697465 2d706163 6b616765 732f746f site-packages/to
   0x00978780 7263682f 696e636c 7564652f 4154656e rch/include/ATen
   0x00978790 2f636f72 652f6976 616c7565 5f696e6c /core/ivalue_inl
   0x009787a0 2e68223a 3233372c 20706c65 61736520 .h":237, please 
   0x009787b0 7265706f 72742061 20627567 20746f20 report a bug to 
   0x009787c0 5079546f 7263682e 20000000 00000000 PyTorch. .......
   0x009787d0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x009787e0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x009787f0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00978800 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00978800 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00978810 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00978820 64652f41 54656e2f 636f7265 2f697661 de/ATen/core/iva
   0x00978830 6c75655f 696e6c2e 6800746f 53796d49 lue_inl.h.toSymI
   0x00978840 6e740000 00000000 00000000 00000000 nt..............
   0x00978850 53743139 6261645f 6f707469 6f6e616c St19bad_optional
   0x00978860 5f616363 65737300 00000000 00000000 _access.........
   0x00978870 4e336331 30323069 6e747275 73697665 N3c1020intrusive
@@ -11272,28 +11272,28 @@
   0x00979050 6e642000 20646576 69636573 00676574 nd . devices.get
   0x00979060 44657669 63654775 61726449 6d706c00 DeviceGuardImpl.
   0x00979070 5079546f 72636820 6973206e 6f74206c PyTorch is not l
   0x00979080 696e6b65 64207769 74682073 7570706f inked with suppo
   0x00979090 72742066 6f722000 2f676974 6875622f rt for ./github/
   0x009790a0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009790b0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009790c0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009790c0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009790d0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009790e0 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x009790f0 6f72652f 696d706c 2f446576 69636547 ore/impl/DeviceG
   0x00979100 75617264 496d706c 496e7465 72666163 uardImplInterfac
   0x00979110 652e6800 4576656e 74206465 76696365 e.h.Event device
   0x00979120 20747970 65200062 6c6f636b 00000000  type .block....
   0x00979130 20646f65 73206e6f 74206d61 74636820  does not match 
   0x00979140 626c6f63 6b696e67 20737472 65616d27 blocking stream'
   0x00979150 73206465 76696365 20747970 65200000 s device type ..
   0x00979160 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00979170 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00979180 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00979190 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00979190 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x009791a0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x009791b0 64652f63 31302f63 6f72652f 696d706c de/c10/core/impl
   0x009791c0 2f496e6c 696e6545 76656e74 2e680000 /InlineEvent.h..
   0x009791d0 45787065 63746564 20216e61 6d652e65 Expected !name.e
   0x009791e0 6d707479 28292074 6f206265 20747275 mpty() to be tru
   0x009791f0 652c2062 75742067 6f742066 616c7365 e, but got false
   0x00979200 2e202028 436f756c 64207468 69732065 .  (Could this e
@@ -11301,49 +11301,49 @@
   0x00979220 696d7072 6f766564 3f202049 6620736f improved?  If so
   0x00979230 2c20706c 65617365 20726570 6f727420 , please report 
   0x00979240 616e2065 6e68616e 63656d65 6e742072 an enhancement r
   0x00979250 65717565 73742074 6f205079 546f7263 equest to PyTorc
   0x00979260 682e2900 00000000 2f676974 6875622f h.)...../github/
   0x00979270 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00979280 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00979290 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00979290 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009792a0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009792b0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x009792c0 636f7265 2f717561 6c696669 65645f6e core/qualified_n
   0x009792d0 616d652e 68000000 496e7661 6c696420 ame.h...Invalid 
   0x009792e0 6e616d65 20666f72 20717561 6c696669 name for qualifi
   0x009792f0 6564206e 616d653a 20270000 00000000 ed name: '......
   0x00979300 2161746f 6d2e656d 70747928 2920494e !atom.empty() IN
   0x00979310 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x00979320 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x00979330 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x00979340 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x00979350 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x00979350 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x00979360 73697465 2d706163 6b616765 732f746f site-packages/to
   0x00979370 7263682f 696e636c 7564652f 4154656e rch/include/ATen
   0x00979380 2f636f72 652f7175 616c6966 6965645f /core/qualified_
   0x00979390 6e616d65 2e68223a 32342c20 706c6561 name.h":24, plea
   0x009793a0 73652072 65706f72 74206120 62756720 se report a bug 
   0x009793b0 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x009793c0 2166696e 616c4174 6f6d2e65 6d707479 !finalAtom.empty
   0x009793d0 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x009793e0 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x009793f0 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x00979400 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x00979410 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x00979420 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x00979420 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x00979430 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00979440 2f415465 6e2f636f 72652f71 75616c69 /ATen/core/quali
   0x00979450 66696564 5f6e616d 652e6822 3a33322c fied_name.h":32,
   0x00979460 20706c65 61736520 7265706f 72742061  please report a
   0x00979470 20627567 20746f20 5079546f 7263682e  bug to PyTorch.
   0x00979480 20000000 00000000 2f676974 6875622f  ......./github/
   0x00979490 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009794a0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009794b0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009794b0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009794c0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009794d0 63682f69 6e636c75 64652f63 31302f75 ch/include/c10/u
   0x009794e0 74696c2f 41727261 79526566 2e680051 til/ArrayRef.h.Q
   0x009794f0 75616c69 66696564 4e616d65 00626173 ualifiedName.bas
   0x00979500 69635f73 7472696e 673a3a73 75627374 ic_string::subst
   0x00979510 72004172 72617952 65663a20 696e7661 r.ArrayRef: inva
   0x00979520 6c696420 736c6963 652c204e 203d2000 lid slice, N = .
@@ -11354,27 +11354,27 @@
   0x00979570 77697468 2064696d 656e7369 6f6e733a with dimensions:
   0x00979580 20000000 00000000 74656e73 6f722e64  .......tensor.d
   0x00979590 696d2829 203d3d20 3020494e 5445524e im() == 0 INTERN
   0x009795a0 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x009795b0 20617420 222f6769 74687562 2f686f6d  at "/github/hom
   0x009795c0 652f6d69 6e69636f 6e64612f 656e7673 e/miniconda/envs
   0x009795d0 2f627569 6c645f62 696e6172 792f6c69 /build_binary/li
-  0x009795e0 622f7079 74686f6e 332e392f 73697465 b/python3.9/site
+  0x009795e0 622f7079 74686f6e 332e382f 73697465 b/python3.8/site
   0x009795f0 2d706163 6b616765 732f746f 7263682f -packages/torch/
   0x00979600 696e636c 7564652f 746f7263 682f6373 include/torch/cs
   0x00979610 72632f61 70692f69 6e636c75 64652f74 rc/api/include/t
   0x00979620 6f726368 2f646574 61696c2f 54656e73 orch/detail/Tens
   0x00979630 6f724461 7461436f 6e746169 6e65722e orDataContainer.
   0x00979640 68223a33 31372c20 706c6561 73652072 h":317, please r
   0x00979650 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x00979660 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x00979670 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00979680 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00979690 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x009796a0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x009796a0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x009796b0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x009796c0 64652f74 6f726368 2f637372 632f6170 de/torch/csrc/ap
   0x009796d0 692f696e 636c7564 652f746f 7263682f i/include/torch/
   0x009796e0 64657461 696c2f54 656e736f 72446174 detail/TensorDat
   0x009796f0 61436f6e 7461696e 65722e68 00000000 aContainer.h....
   0x00979700 20696e20 69747320 66697273 74206469  in its first di
   0x00979710 6d656e73 696f6e2c 20627574 20676f74 mension, but got
@@ -11383,15 +11383,15 @@
   0x00979740 697a6573 28295b30 5d203d3d 2028696e izes()[0] == (in
   0x00979750 7436345f 7429696e 69745f6c 6973745f t64_t)init_list_
   0x00979760 2e73697a 65282920 494e5445 524e414c .size() INTERNAL
   0x00979770 20415353 45525420 4641494c 45442061  ASSERT FAILED a
   0x00979780 7420222f 67697468 75622f68 6f6d652f t "/github/home/
   0x00979790 6d696e69 636f6e64 612f656e 76732f62 miniconda/envs/b
   0x009797a0 75696c64 5f62696e 6172792f 6c69622f uild_binary/lib/
-  0x009797b0 70797468 6f6e332e 392f7369 74652d70 python3.9/site-p
+  0x009797b0 70797468 6f6e332e 382f7369 74652d70 python3.8/site-p
   0x009797c0 61636b61 6765732f 746f7263 682f696e ackages/torch/in
   0x009797d0 636c7564 652f746f 7263682f 63737263 clude/torch/csrc
   0x009797e0 2f617069 2f696e63 6c756465 2f746f72 /api/include/tor
   0x009797f0 63682f64 65746169 6c2f5465 6e736f72 ch/detail/Tensor
   0x00979800 44617461 436f6e74 61696e65 722e6822 DataContainer.h"
   0x00979810 3a333234 2c20706c 65617365 20726570 :324, please rep
   0x00979820 6f727420 61206275 6720746f 20507954 ort a bug to PyT
@@ -11402,15 +11402,15 @@
   0x00979870 6f726020 73686f75 6c64206e 6f742062 or` should not b
   0x00979880 65206361 6c6c6564 00000000 00000000 e called........
   0x00979890 66616c73 6520494e 5445524e 414c2041 false INTERNAL A
   0x009798a0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x009798b0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x009798c0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x009798d0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x009798e0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x009798e0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x009798f0 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x00979900 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x00979910 70692f69 6e636c75 64652f74 6f726368 pi/include/torch
   0x00979920 2f646574 61696c2f 54656e73 6f724461 /detail/TensorDa
   0x00979930 7461436f 6e746169 6e65722e 68223a33 taContainer.h":3
   0x00979940 33382c20 706c6561 73652072 65706f72 38, please repor
   0x00979950 74206120 62756720 746f2050 79546f72 t a bug to PyTor
@@ -11418,15 +11418,15 @@
   0x00979970 54656e73 6f724461 7461436f 6e746169 TensorDataContai
   0x00979980 6e657220 74797065 00000000 00000000 ner type........
   0x00979990 66616c73 6520494e 5445524e 414c2041 false INTERNAL A
   0x009799a0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x009799b0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x009799c0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x009799d0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x009799e0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x009799e0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x009799f0 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x00979a00 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x00979a10 70692f69 6e636c75 64652f74 6f726368 pi/include/torch
   0x00979a20 2f646574 61696c2f 54656e73 6f724461 /detail/TensorDa
   0x00979a30 7461436f 6e746169 6e65722e 68223a33 taContainer.h":3
   0x00979a40 34322c20 706c6561 73652072 65706f72 42, please repor
   0x00979a50 74206120 62756720 746f2050 79546f72 t a bug to PyTor
@@ -11444,15 +11444,15 @@
   0x00979b10 74686f75 74206c6f 7373206f 6620696e thout loss of in
   0x00979b20 666f726d 6174696f 6e000000 00000000 formation.......
   0x00979b30 66616c73 6520494e 5445524e 414c2041 false INTERNAL A
   0x00979b40 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00979b50 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x00979b60 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x00979b70 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x00979b80 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x00979b80 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x00979b90 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x00979ba0 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x00979bb0 70692f69 6e636c75 64652f74 6f726368 pi/include/torch
   0x00979bc0 2f646574 61696c2f 54656e73 6f724461 /detail/TensorDa
   0x00979bd0 7461436f 6e746169 6e65722e 68223a32 taContainer.h":2
   0x00979be0 37322c20 706c6561 73652072 65706f72 72, please repor
   0x00979bf0 74206120 62756720 746f2050 79546f72 t a bug to PyTor
@@ -11472,15 +11472,15 @@
   0x00979cd0 3b206974 20697320 6f6e6c79 20666f72 ; it is only for
   0x00979ce0 20475055 2e000000 6973496e 744c6973  GPU....isIntLis
   0x00979cf0 74282920 494e5445 524e414c 20415353 t() INTERNAL ASS
   0x00979d00 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x00979d10 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x00979d20 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x00979d30 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
-  0x00979d40 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
+  0x00979d40 6f6e332e 382f7369 74652d70 61636b61 on3.8/site-packa
   0x00979d50 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00979d60 652f4154 656e2f63 6f72652f 6976616c e/ATen/core/ival
   0x00979d70 75655f69 6e6c2e68 223a3139 37322c20 ue_inl.h":1972, 
   0x00979d80 706c6561 73652072 65706f72 74206120 please report a 
   0x00979d90 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x00979da0 00000000 00000000 76656374 6f723a3a ........vector::
   0x00979db0 5f4d5f72 616e6765 5f636865 636b3a20 _M_range_check: 
@@ -11507,19 +11507,19 @@
   0x00979f00 61726775 6d656e74 206f6620 5f5f7365 argument of __se
   0x00979f10 74737461 74655f5f 2e20476f 74200000 tstate__. Got ..
   0x00979f20 69735374 72696e67 28292049 4e544552 isString() INTER
   0x00979f30 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x00979f40 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x00979f50 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x00979f60 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x00979f70 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x00979f70 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x00979f80 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x00979f90 2f696e63 6c756465 2f415465 6e2f636f /include/ATen/co
   0x00979fa0 72652f69 76616c75 655f696e 6c2e6822 re/ivalue_inl.h"
-  0x00979fb0 3a323336 322c2070 6c656173 65207265 :2362, please re
+  0x00979fb0 3a323336 312c2070 6c656173 65207265 :2361, please re
   0x00979fc0 706f7274 20612062 75672074 6f205079 port a bug to Py
   0x00979fd0 546f7263 682e2000 2f2f6465 65706c65 Torch. .//deeple
   0x00979fe0 61726e69 6e672f66 6267656d 6d2f6662 arning/fbgemm/fb
   0x00979ff0 67656d6d 5f677075 3a737061 7273655f gemm_gpu:sparse_
   0x0097a000 6f70735f 70790000 696e745f 6e626974 ops_py..int_nbit
   0x0097a010 5f73706c 69745f65 6d626564 64696e67 _split_embedding
   0x0097a020 5f636f64 6567656e 5f6c6f6f 6b75705f _codegen_lookup_
@@ -11633,36 +11633,36 @@
   0x0097a6e0 73657473 29202d3e 2054656e 736f7200 sets) -> Tensor.
   0x0097a6f0 69734765 6e657269 63446963 74282920 isGenericDict() 
   0x0097a700 494e5445 524e414c 20415353 45525420 INTERNAL ASSERT 
   0x0097a710 4641494c 45442061 7420222f 67697468 FAILED at "/gith
   0x0097a720 75622f68 6f6d652f 6d696e69 636f6e64 ub/home/minicond
   0x0097a730 612f656e 76732f62 75696c64 5f62696e a/envs/build_bin
   0x0097a740 6172792f 6c69622f 70797468 6f6e332e ary/lib/python3.
-  0x0097a750 392f7369 74652d70 61636b61 6765732f 9/site-packages/
+  0x0097a750 382f7369 74652d70 61636b61 6765732f 8/site-packages/
   0x0097a760 746f7263 682f696e 636c7564 652f4154 torch/include/AT
   0x0097a770 656e2f63 6f72652f 6976616c 75655f69 en/core/ivalue_i
   0x0097a780 6e6c2e68 223a3230 38382c20 706c6561 nl.h":2088, plea
   0x0097a790 73652072 65706f72 74206120 62756720 se report a bug 
   0x0097a7a0 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x0097a7b0 73656c66 5f696d70 6c20494e 5445524e self_impl INTERN
   0x0097a7c0 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x0097a7d0 20617420 222f6769 74687562 2f686f6d  at "/github/hom
   0x0097a7e0 652f6d69 6e69636f 6e64612f 656e7673 e/miniconda/envs
   0x0097a7f0 2f627569 6c645f62 696e6172 792f6c69 /build_binary/li
-  0x0097a800 622f7079 74686f6e 332e392f 73697465 b/python3.9/site
+  0x0097a800 622f7079 74686f6e 332e382f 73697465 b/python3.8/site
   0x0097a810 2d706163 6b616765 732f746f 7263682f -packages/torch/
   0x0097a820 696e636c 7564652f 746f7263 682f6373 include/torch/cs
   0x0097a830 72632f61 75746f67 7261642f 76617269 rc/autograd/vari
   0x0097a840 61626c65 2e68223a 3330352c 20706c65 able.h":305, ple
   0x0097a850 61736520 7265706f 72742061 20627567 ase report a bug
   0x0097a860 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x0097a870 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0097a880 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0097a890 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0097a8a0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0097a8a0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0097a8b0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0097a8c0 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x0097a8d0 746f6772 61642f76 61726961 626c652e tograd/variable.
   0x0097a8e0 68000000 00000000 4f6e6c79 2054656e h.......Only Ten
   0x0097a8f0 736f7273 206f6620 666c6f61 74696e67 sors of floating
   0x0097a900 20706f69 6e742061 6e642063 6f6d706c  point and compl
   0x0097a910 65782064 74797065 2063616e 20726571 ex dtype can req
@@ -11722,37 +11722,37 @@
   0x0097ac70 73657274 00000000 73636865 6d615f2e sert....schema_.
   0x0097ac80 72657475 726e7328 292e7369 7a652829 returns().size()
   0x0097ac90 203d3d20 3120494e 5445524e 414c2041  == 1 INTERNAL A
   0x0097aca0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x0097acb0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x0097acc0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x0097acd0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x0097ace0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x0097ace0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x0097acf0 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x0097ad00 7564652f 4154656e 2f636f72 652f6275 ude/ATen/core/bu
   0x0097ad10 696c7469 6e5f6675 6e637469 6f6e2e68 iltin_function.h
   0x0097ad20 223a3232 2c20706c 65617365 20726570 ":22, please rep
   0x0097ad30 6f727420 61206275 6720746f 20507954 ort a bug to PyT
   0x0097ad40 6f726368 2e200000 2f676974 6875622f orch. ../github/
   0x0097ad50 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0097ad60 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0097ad70 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0097ad70 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0097ad80 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0097ad90 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0097ada0 636f7265 2f627569 6c74696e 5f66756e core/builtin_fun
   0x0097adb0 6374696f 6e2e6800 4275696c 74696e4f ction.h.BuiltinO
   0x0097adc0 7046756e 6374696f 6e006465 66696e65 pFunction.define
   0x0097add0 4d657468 6f640000 44656661 756c7420 Method..Default 
   0x0097ade0 76616c75 6573206d 75737420 62652073 values must be s
   0x0097adf0 70656369 66696564 20666f72 206e6f6e pecified for non
   0x0097ae00 65206f72 20616c6c 20617267 756d656e e or all argumen
   0x0097ae10 74730000 00000000 2f676974 6875622f ts....../github/
   0x0097ae20 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0097ae30 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0097ae40 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0097ae40 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0097ae50 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0097ae60 63682f69 6e636c75 64652f74 6f726368 ch/include/torch
   0x0097ae70 2f637573 746f6d5f 636c6173 732e6800 /custom_class.h.
   0x0097ae80 54656e73 6f72496d 706c2077 69746820 TensorImpl with 
   0x0097ae90 6e756c6c 70747220 6973206e 6f742073 nullptr is not s
   0x0097aea0 7570706f 72746564 00766563 746f723a upported.vector:
   0x0097aeb0 3a5f4d5f 64656661 756c745f 61707065 :_M_default_appe
@@ -11890,15 +11890,15 @@
   0x0097b6f0 204f626a 65637420 62757420 676f7420  Object but got 
   0x0097b700 00746f4f 626a6563 74000000 00000000 .toObject.......
   0x0097b710 69734f62 6a656374 28292049 4e544552 isObject() INTER
   0x0097b720 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x0097b730 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x0097b740 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x0097b750 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x0097b760 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x0097b760 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x0097b770 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x0097b780 2f696e63 6c756465 2f415465 6e2f636f /include/ATen/co
   0x0097b790 72652f69 76616c75 655f696e 6c2e6822 re/ivalue_inl.h"
   0x0097b7a0 3a313333 2c20706c 65617365 20726570 :133, please rep
   0x0097b7b0 6f727420 61206275 6720746f 20507954 ort a bug to PyT
   0x0097b7c0 6f726368 2e200000 41726775 6d656e74 orch. ..Argument
   0x0097b7d0 20706173 73656420 746f2061 74282920  passed to at() 
@@ -11907,15 +11907,15 @@
   0x0097b800 71756575 65002f73 697a6500 2f000000 queue./size./...
   0x0097b810 53747265 616d7320 68617665 2061206d Streams have a m
   0x0097b820 6978206f 66206465 76696365 20747970 ix of device typ
   0x0097b830 65733a20 73747265 616d2030 20697320 es: stream 0 is 
   0x0097b840 6f6e2000 00000000 2f676974 6875622f on ...../github/
   0x0097b850 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0097b860 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0097b870 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0097b870 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0097b880 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0097b890 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x0097b8a0 6f72652f 696d706c 2f496e6c 696e6553 ore/impl/InlineS
   0x0097b8b0 74726561 6d477561 72642e68 00207768 treamGuard.h. wh
   0x0097b8c0 696c6520 73747265 616d2000 20697320 ile stream . is 
   0x0097b8d0 6f6e2064 65766963 65200067 65744465 on device .getDe
   0x0097b8e0 76696365 54797065 4f665374 7265616d viceTypeOfStream
@@ -11928,15 +11928,15 @@
   0x0097b950 7320616c 72656164 79206d61 726b6564 s already marked
   0x0097b960 20636f6d 706c6574 65640000 00000000  completed......
   0x0097b970 21636f6d 706c6574 65642829 20494e54 !completed() INT
   0x0097b980 45524e41 4c204153 53455254 20464149 ERNAL ASSERT FAI
   0x0097b990 4c454420 61742022 2f676974 6875622f LED at "/github/
   0x0097b9a0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0097b9b0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0097b9c0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0097b9c0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0097b9d0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0097b9e0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0097b9f0 636f7265 2f697661 6c75655f 696e6c2e core/ivalue_inl.
   0x0097ba00 68223a31 3232312c 20706c65 61736520 h":1221, please 
   0x0097ba10 7265706f 72742061 20627567 20746f20 report a bug to 
   0x0097ba20 5079546f 7263682e 20000000 00000000 PyTorch. .......
   0x0097ba30 20776869 63682061 7265206e 6f742061  which are not a
@@ -11972,15 +11972,15 @@
   0x0097bc10 3e5d0000 00000000 20636f75 6c64206e >]...... could n
   0x0097bc20 6f742062 6520636f 6e766572 74656420 ot be converted 
   0x0097bc30 746f2061 6e79206f 66207468 65206b6e to any of the kn
   0x0097bc40 6f776e20 74797065 732e0000 00000000 own types.......
   0x0097bc50 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0097bc60 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0097bc70 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0097bc80 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0097bc80 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0097bc90 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0097bca0 64652f41 54656e2f 636f7265 2f6a6974 de/ATen/core/jit
   0x0097bcb0 5f747970 652e6800 54797065 20000000 _type.h.Type ...
   0x0097bcc0 636f6e73 74657870 72206331 303a3a73 constexpr c10::s
   0x0097bcd0 7472696e 675f7669 65772063 31303a3a tring_view c10::
   0x0097bce0 7574696c 3a3a6465 7461696c 3a3a6675 util::detail::fu
   0x0097bcf0 6c6c795f 7175616c 69666965 645f7479 lly_qualified_ty
@@ -12041,15 +12041,15 @@
   0x0097c060 6e6f7420 636f6e74 61696e20 61206375 not contain a cu
   0x0097c070 73746f6d 20636c61 73732100 00000000 stom class!.....
   0x0097c080 69734361 7073756c 65282920 494e5445 isCapsule() INTE
   0x0097c090 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x0097c0a0 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x0097c0b0 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x0097c0c0 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x0097c0d0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x0097c0d0 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x0097c0e0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x0097c0f0 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x0097c100 6f72652f 6976616c 75655f69 6e6c2e68 ore/ivalue_inl.h
   0x0097c110 223a3232 352c2070 6c656173 65207265 ":225, please re
   0x0097c120 706f7274 20612062 75672074 6f205079 port a bug to Py
   0x0097c130 546f7263 682e2000 746f4375 73746f6d Torch. .toCustom
   0x0097c140 436c6173 7300746f 43617073 756c6500 Class.toCapsule.
@@ -12063,36 +12063,36 @@
   0x0097c1c0 2829203d 3d202a64 6963742e 696d706c () == *dict.impl
   0x0097c1d0 5f2d3e65 6c656d65 6e745479 7065732e _->elementTypes.
   0x0097c1e0 6b657954 79706520 494e5445 524e414c keyType INTERNAL
   0x0097c1f0 20415353 45525420 4641494c 45442061  ASSERT FAILED a
   0x0097c200 7420222f 67697468 75622f68 6f6d652f t "/github/home/
   0x0097c210 6d696e69 636f6e64 612f656e 76732f62 miniconda/envs/b
   0x0097c220 75696c64 5f62696e 6172792f 6c69622f uild_binary/lib/
-  0x0097c230 70797468 6f6e332e 392f7369 74652d70 python3.9/site-p
+  0x0097c230 70797468 6f6e332e 382f7369 74652d70 python3.8/site-p
   0x0097c240 61636b61 6765732f 746f7263 682f696e ackages/torch/in
   0x0097c250 636c7564 652f4154 656e2f63 6f72652f clude/ATen/core/
   0x0097c260 44696374 5f696e6c 2e68223a 32362c20 Dict_inl.h":26, 
   0x0097c270 706c6561 73652072 65706f72 74206120 please report a 
   0x0097c280 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x0097c290 00000000 00000000 2f676974 6875622f ......../github/
   0x0097c2a0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0097c2b0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0097c2c0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0097c2c0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0097c2d0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0097c2e0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0097c2f0 636f7265 2f446963 745f696e 6c2e6800 core/Dict_inl.h.
   0x0097c300 2a676574 54797065 5074723c 56616c75 *getTypePtr<Valu
   0x0097c310 653e2829 203d3d20 2a646963 742e696d e>() == *dict.im
   0x0097c320 706c5f2d 3e656c65 6d656e74 54797065 pl_->elementType
   0x0097c330 732e7661 6c756554 79706520 494e5445 s.valueType INTE
   0x0097c340 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x0097c350 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x0097c360 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x0097c370 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x0097c380 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x0097c380 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x0097c390 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x0097c3a0 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x0097c3b0 6f72652f 44696374 5f696e6c 2e68223a ore/Dict_inl.h":
   0x0097c3c0 32372c20 706c6561 73652072 65706f72 27, please repor
   0x0097c3d0 74206120 62756720 746f2050 79546f72 t a bug to PyTor
   0x0097c3e0 63682e20 00000000 4e336331 30354572 ch. ....N3c105Er
   0x0097c3f0 726f7245 00000000 00000000 00000000 rorE............
@@ -12452,15 +12452,15 @@
   0x0097da10 6a767020 6973206e 6f742069 6d706c65 jvp is not imple
   0x0097da20 6d656e74 65642066 6f722074 68652063 mented for the c
   0x0097da30 2b2b2041 5049206f 66206375 73746f6d ++ API of custom
   0x0097da40 2046756e 6374696f 6e207965 742e0000  Function yet...
   0x0097da50 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0097da60 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0097da70 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0097da80 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0097da80 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0097da90 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0097daa0 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x0097dab0 746f6772 61642f63 7573746f 6d5f6675 tograd/custom_fu
   0x0097dac0 6e637469 6f6e2e68 00000000 00000000 nction.h........
   0x0097dad0 636f6d70 696c6564 5f617267 73206e6f compiled_args no
   0x0097dae0 7420696d 706c656d 656e7465 6420666f t implemented fo
   0x0097daf0 72206e6f 6e2d7472 61636561 626c6520 r non-traceable 
@@ -12500,25 +12500,25 @@
   0x0097dd10 6620616c 6c206974 73206368 696c6472 f all its childr
   0x0097dd20 656e0000 00000000 21686173 5f706172 en......!has_par
   0x0097dd30 656e745f 20494e54 45524e41 4c204153 ent_ INTERNAL AS
   0x0097dd40 53455254 20464149 4c454420 61742022 SERT FAILED at "
   0x0097dd50 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0097dd60 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0097dd70 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0097dd80 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0097dd80 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0097dd90 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0097dda0 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x0097ddb0 746f6772 61642f66 756e6374 696f6e2e tograd/function.
   0x0097ddc0 68223a32 36322c20 706c6561 73652072 h":262, please r
   0x0097ddd0 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x0097dde0 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x0097ddf0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0097de00 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0097de10 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0097de20 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0097de20 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0097de30 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0097de40 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x0097de50 746f6772 61642f66 756e6374 696f6e2e tograd/function.
   0x0097de60 68000000 00000000 2f5f5f77 2f464247 h......./__w/FBG
   0x0097de70 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0097de80 6d5f6770 752f636f 64656765 6e2f7472 m_gpu/codegen/tr
   0x0097de90 61696e69 6e672f62 61636b77 6172642f aining/backward/
@@ -12542,147 +12542,147 @@
   0x0097dfb0 6374785f 2e6e6f6e 5f646966 66657265 ctx_.non_differe
   0x0097dfc0 6e746961 626c655f 2e656d70 74792829 ntiable_.empty()
   0x0097dfd0 20494e54 45524e41 4c204153 53455254  INTERNAL ASSERT
   0x0097dfe0 20464149 4c454420 61742022 2f676974  FAILED at "/git
   0x0097dff0 6875622f 686f6d65 2f6d696e 69636f6e hub/home/minicon
   0x0097e000 64612f65 6e76732f 6275696c 645f6269 da/envs/build_bi
   0x0097e010 6e617279 2f6c6962 2f707974 686f6e33 nary/lib/python3
-  0x0097e020 2e392f73 6974652d 7061636b 61676573 .9/site-packages
+  0x0097e020 2e382f73 6974652d 7061636b 61676573 .8/site-packages
   0x0097e030 2f746f72 63682f69 6e636c75 64652f74 /torch/include/t
   0x0097e040 6f726368 2f637372 632f6175 746f6772 orch/csrc/autogr
   0x0097e050 61642f63 7573746f 6d5f6675 6e637469 ad/custom_functi
   0x0097e060 6f6e2e68 223a3232 312c2070 6c656173 on.h":221, pleas
   0x0097e070 65207265 706f7274 20612062 75672074 e report a bug t
   0x0097e080 6f205079 546f7263 682e2000 00000000 o PyTorch. .....
   0x0097e090 6374785f 2e646972 74795f69 6e707574 ctx_.dirty_input
   0x0097e0a0 735f2e65 6d707479 28292049 4e544552 s_.empty() INTER
   0x0097e0b0 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x0097e0c0 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x0097e0d0 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x0097e0e0 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x0097e0f0 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x0097e0f0 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x0097e100 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x0097e110 2f696e63 6c756465 2f746f72 63682f63 /include/torch/c
   0x0097e120 7372632f 6175746f 67726164 2f637573 src/autograd/cus
   0x0097e130 746f6d5f 66756e63 74696f6e 2e68223a tom_function.h":
   0x0097e140 3232322c 20706c65 61736520 7265706f 222, please repo
   0x0097e150 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x0097e160 7263682e 20000000 69742021 3d205f73 rch. ...it != _s
   0x0097e170 61766564 5f766172 6961626c 65732e65 aved_variables.e
   0x0097e180 6e642829 20494e54 45524e41 4c204153 nd() INTERNAL AS
   0x0097e190 53455254 20464149 4c454420 61742022 SERT FAILED at "
   0x0097e1a0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0097e1b0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0097e1c0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0097e1d0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0097e1d0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0097e1e0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0097e1f0 64652f74 6f726368 2f637372 632f6479 de/torch/csrc/dy
   0x0097e200 6e616d6f 2f636f6d 70696c65 645f6175 namo/compiled_au
   0x0097e210 746f6772 61642e68 223a3133 382c2070 tograd.h":138, p
   0x0097e220 6c656173 65207265 706f7274 20612062 lease report a b
   0x0097e230 75672074 6f205079 546f7263 682e2000 ug to PyTorch. .
   0x0097e240 6172672e 70726f78 795f7465 6e736f72 arg.proxy_tensor
   0x0097e250 2e646566 696e6564 28292049 4e544552 .defined() INTER
   0x0097e260 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x0097e270 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x0097e280 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x0097e290 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x0097e2a0 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x0097e2a0 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x0097e2b0 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x0097e2c0 2f696e63 6c756465 2f746f72 63682f63 /include/torch/c
   0x0097e2d0 7372632f 64796e61 6d6f2f63 6f6d7069 src/dynamo/compi
   0x0097e2e0 6c65645f 6175746f 67726164 2e68223a led_autograd.h":
   0x0097e2f0 3536312c 20706c65 61736520 7265706f 561, please repo
   0x0097e300 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x0097e310 7263682e 20000000 6374785f 2e746f5f rch. ...ctx_.to_
   0x0097e320 73617665 5f2e656d 70747928 2920494e save_.empty() IN
   0x0097e330 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x0097e340 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x0097e350 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x0097e360 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x0097e370 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x0097e370 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x0097e380 73697465 2d706163 6b616765 732f746f site-packages/to
   0x0097e390 7263682f 696e636c 7564652f 746f7263 rch/include/torc
   0x0097e3a0 682f6373 72632f61 75746f67 7261642f h/csrc/autograd/
   0x0097e3b0 63757374 6f6d5f66 756e6374 696f6e2e custom_function.
   0x0097e3c0 68223a32 32342c20 706c6561 73652072 h":224, please r
   0x0097e3d0 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x0097e3e0 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x0097e3f0 69742021 3d207468 69732d3e 656e6428 it != this->end(
   0x0097e400 2920494e 5445524e 414c2041 53534552 ) INTERNAL ASSER
   0x0097e410 54204641 494c4544 20617420 222f6769 T FAILED at "/gi
   0x0097e420 74687562 2f686f6d 652f6d69 6e69636f thub/home/minico
   0x0097e430 6e64612f 656e7673 2f627569 6c645f62 nda/envs/build_b
   0x0097e440 696e6172 792f6c69 622f7079 74686f6e inary/lib/python
-  0x0097e450 332e392f 73697465 2d706163 6b616765 3.9/site-package
+  0x0097e450 332e382f 73697465 2d706163 6b616765 3.8/site-package
   0x0097e460 732f746f 7263682f 696e636c 7564652f s/torch/include/
   0x0097e470 746f7263 682f6373 72632f64 796e616d torch/csrc/dynam
   0x0097e480 6f2f636f 6d70696c 65645f61 75746f67 o/compiled_autog
   0x0097e490 7261642e 68223a37 36302c20 706c6561 rad.h":760, plea
   0x0097e4a0 73652072 65706f72 74206120 62756720 se report a bug 
   0x0097e4b0 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x0097e4c0 6374785f 2e6e6f6e 5f646966 66657265 ctx_.non_differe
   0x0097e4d0 6e746961 626c655f 2e656d70 74792829 ntiable_.empty()
   0x0097e4e0 20494e54 45524e41 4c204153 53455254  INTERNAL ASSERT
   0x0097e4f0 20464149 4c454420 61742022 2f676974  FAILED at "/git
   0x0097e500 6875622f 686f6d65 2f6d696e 69636f6e hub/home/minicon
   0x0097e510 64612f65 6e76732f 6275696c 645f6269 da/envs/build_bi
   0x0097e520 6e617279 2f6c6962 2f707974 686f6e33 nary/lib/python3
-  0x0097e530 2e392f73 6974652d 7061636b 61676573 .9/site-packages
+  0x0097e530 2e382f73 6974652d 7061636b 61676573 .8/site-packages
   0x0097e540 2f746f72 63682f69 6e636c75 64652f74 /torch/include/t
   0x0097e550 6f726368 2f637372 632f6175 746f6772 orch/csrc/autogr
   0x0097e560 61642f63 7573746f 6d5f6675 6e637469 ad/custom_functi
   0x0097e570 6f6e2e68 223a3233 312c2070 6c656173 on.h":231, pleas
   0x0097e580 65207265 706f7274 20612062 75672074 e report a bug t
   0x0097e590 6f205079 546f7263 682e2000 00000000 o PyTorch. .....
   0x0097e5a0 6374785f 2e646972 74795f69 6e707574 ctx_.dirty_input
   0x0097e5b0 735f2e65 6d707479 28292049 4e544552 s_.empty() INTER
   0x0097e5c0 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x0097e5d0 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x0097e5e0 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x0097e5f0 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x0097e600 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x0097e600 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x0097e610 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x0097e620 2f696e63 6c756465 2f746f72 63682f63 /include/torch/c
   0x0097e630 7372632f 6175746f 67726164 2f637573 src/autograd/cus
   0x0097e640 746f6d5f 66756e63 74696f6e 2e68223a tom_function.h":
   0x0097e650 3233322c 20706c65 61736520 7265706f 232, please repo
   0x0097e660 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x0097e670 7263682e 20000000 6374785f 2e746f5f rch. ...ctx_.to_
   0x0097e680 73617665 5f2e656d 70747928 2920494e save_.empty() IN
   0x0097e690 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x0097e6a0 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x0097e6b0 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x0097e6c0 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x0097e6d0 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x0097e6d0 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x0097e6e0 73697465 2d706163 6b616765 732f746f site-packages/to
   0x0097e6f0 7263682f 696e636c 7564652f 746f7263 rch/include/torc
   0x0097e700 682f6373 72632f61 75746f67 7261642f h/csrc/autograd/
   0x0097e710 63757374 6f6d5f66 756e6374 696f6e2e custom_function.
   0x0097e720 68223a32 33342c20 706c6561 73652072 h":234, please r
   0x0097e730 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x0097e740 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x0097e750 73796d5f 73697a65 735f696e 64657820 sym_sizes_index 
   0x0097e760 3c207379 6d5f7369 7a65732e 73697a65 < sym_sizes.size
   0x0097e770 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x0097e780 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x0097e790 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x0097e7a0 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x0097e7b0 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x0097e7c0 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x0097e7c0 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x0097e7d0 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x0097e7e0 2f746f72 63682f63 7372632f 64796e61 /torch/csrc/dyna
   0x0097e7f0 6d6f2f63 6f6d7069 6c65645f 6175746f mo/compiled_auto
   0x0097e800 67726164 2e68223a 3533312c 20706c65 grad.h":531, ple
   0x0097e810 61736520 7265706f 72742061 20627567 ase report a bug
   0x0097e820 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x0097e830 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0097e840 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0097e850 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0097e860 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0097e860 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0097e870 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0097e880 64652f74 6f726368 2f637372 632f6479 de/torch/csrc/dy
   0x0097e890 6e616d6f 2f636f6d 70696c65 645f6175 namo/compiled_au
   0x0097e8a0 746f6772 61642e68 006e6578 745f7379 tograd.h.next_sy
   0x0097e8b0 6d5f7369 7a650000 00000000 00000000 m_size..........
   0x0097e8c0 50467650 4e35746f 72636838 6175746f PFvPN5torch8auto
   0x0097e8d0 67726164 344e6f64 65454500 00000000 grad4NodeEE.....
@@ -12964,38 +12964,38 @@
   0x0097fa10 547ecaff 047ecaff bc7dcaff 747dcaff T~...~...}..t}..
   0x0097fa20 147dcaff 8484caff 69734465 76696365 .}......isDevice
   0x0097fa30 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x0097fa40 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x0097fa50 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x0097fa60 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x0097fa70 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x0097fa80 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x0097fa80 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x0097fa90 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x0097faa0 2f415465 6e2f636f 72652f69 76616c75 /ATen/core/ivalu
   0x0097fab0 652e6822 3a393331 2c20706c 65617365 e.h":931, please
   0x0097fac0 20726570 6f727420 61206275 6720746f  report a bug to
   0x0097fad0 20507954 6f726368 2e200000 00000000  PyTorch. ......
   0x0097fae0 69735465 6e736f72 4c697374 28292049 isTensorList() I
   0x0097faf0 4e544552 4e414c20 41535345 52542046 NTERNAL ASSERT F
   0x0097fb00 41494c45 44206174 20222f67 69746875 AILED at "/githu
   0x0097fb10 622f686f 6d652f6d 696e6963 6f6e6461 b/home/miniconda
   0x0097fb20 2f656e76 732f6275 696c645f 62696e61 /envs/build_bina
-  0x0097fb30 72792f6c 69622f70 7974686f 6e332e39 ry/lib/python3.9
+  0x0097fb30 72792f6c 69622f70 7974686f 6e332e38 ry/lib/python3.8
   0x0097fb40 2f736974 652d7061 636b6167 65732f74 /site-packages/t
   0x0097fb50 6f726368 2f696e63 6c756465 2f415465 orch/include/ATe
   0x0097fb60 6e2f636f 72652f69 76616c75 655f696e n/core/ivalue_in
   0x0097fb70 6c2e6822 3a323034 302c2070 6c656173 l.h":2040, pleas
   0x0097fb80 65207265 706f7274 20612062 75672074 e report a bug t
   0x0097fb90 6f205079 546f7263 682e2000 00000000 o PyTorch. .....
   0x0097fba0 69735465 6e736f72 4c697374 28292049 isTensorList() I
   0x0097fbb0 4e544552 4e414c20 41535345 52542046 NTERNAL ASSERT F
   0x0097fbc0 41494c45 44206174 20222f67 69746875 AILED at "/githu
   0x0097fbd0 622f686f 6d652f6d 696e6963 6f6e6461 b/home/miniconda
   0x0097fbe0 2f656e76 732f6275 696c645f 62696e61 /envs/build_bina
-  0x0097fbf0 72792f6c 69622f70 7974686f 6e332e39 ry/lib/python3.9
+  0x0097fbf0 72792f6c 69622f70 7974686f 6e332e38 ry/lib/python3.8
   0x0097fc00 2f736974 652d7061 636b6167 65732f74 /site-packages/t
   0x0097fc10 6f726368 2f696e63 6c756465 2f415465 orch/include/ATe
   0x0097fc20 6e2f636f 72652f69 76616c75 655f696e n/core/ivalue_in
   0x0097fc30 6c2e6822 3a323034 342c2070 6c656173 l.h":2044, pleas
   0x0097fc40 65207265 706f7274 20612062 75672074 e report a bug t
   0x0097fc50 6f205079 546f7263 682e2000 746f4465 o PyTorch. .toDe
   0x0097fc60 76696365 00457870 65637465 64205465 vice.Expected Te
@@ -13097,23 +13097,23 @@
   0x00980260 65643f20 20496620 736f2c20 706c6561 ed?  If so, plea
   0x00980270 73652072 65706f72 7420616e 20656e68 se report an enh
   0x00980280 616e6365 6d656e74 20726571 75657374 ancement request
   0x00980290 20746f20 5079546f 7263682e 29000000  to PyTorch.)...
   0x009802a0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x009802b0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x009802c0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x009802d0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x009802d0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x009802e0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x009802f0 64652f63 31302f63 6f72652f 53796d42 de/c10/core/SymB
   0x00980300 6f6f6c2e 68000000 3020494e 5445524e ool.h...0 INTERN
   0x00980310 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x00980320 20617420 222f6769 74687562 2f686f6d  at "/github/hom
   0x00980330 652f6d69 6e69636f 6e64612f 656e7673 e/miniconda/envs
   0x00980340 2f627569 6c645f62 696e6172 792f6c69 /build_binary/li
-  0x00980350 622f7079 74686f6e 332e392f 73697465 b/python3.9/site
+  0x00980350 622f7079 74686f6e 332e382f 73697465 b/python3.8/site
   0x00980360 2d706163 6b616765 732f746f 7263682f -packages/torch/
   0x00980370 696e636c 7564652f 4154656e 2f636f72 include/ATen/cor
   0x00980380 652f6976 616c7565 2e68223a 3637362c e/ivalue.h":676,
   0x00980390 20706c65 61736520 7265706f 72742061  please report a
   0x009803a0 20627567 20746f20 5079546f 7263682e  bug to PyTorch.
   0x009803b0 20000000 00000000 7065726d 7574655f  .......permute_
   0x009803c0 706f6f6c 65645f65 6d627320 646f6573 pooled_embs does
@@ -13133,25 +13133,25 @@
   0x009804a0 68656d61 20726567 69737465 72656420 hema registered 
   0x009804b0 79657400 00000000 73636865 6d615f2e yet.....schema_.
   0x009804c0 6861735f 76616c75 65282920 494e5445 has_value() INTE
   0x009804d0 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x009804e0 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x009804f0 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x00980500 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x00980510 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x00980510 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x00980520 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00980530 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x00980540 6f72652f 64697370 61746368 2f4f7065 ore/dispatch/Ope
   0x00980550 7261746f 72456e74 72792e68 223a3830 ratorEntry.h":80
   0x00980560 2c20706c 65617365 20726570 6f727420 , please report 
   0x00980570 61206275 6720746f 20507954 6f726368 a bug to PyTorch
   0x00980580 2e200000 00000000 2f676974 6875622f . ....../github/
   0x00980590 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009805a0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009805b0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009805b0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009805c0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009805d0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x009805e0 636f7265 2f646973 70617463 682f4f70 core/dispatch/Op
   0x009805f0 65726174 6f72456e 7472792e 68007363 eratorEntry.h.sc
   0x00980600 68656d61 00000000 00000000 00000000 hema............
   0x00980610 00000000 00000000 00000000 00000000 ................
   0x00980620 464e3261 74365465 6e736f72 45524b53 FN2at6TensorERKS
@@ -13648,15 +13648,15 @@
   0x009824d0 64656e73 655f7665 635f6a61 67676564 dense_vec_jagged
   0x009824e0 5f32645f 6d756c00 69734c69 73742829 _2d_mul.isList()
   0x009824f0 20494e54 45524e41 4c204153 53455254  INTERNAL ASSERT
   0x00982500 20464149 4c454420 61742022 2f676974  FAILED at "/git
   0x00982510 6875622f 686f6d65 2f6d696e 69636f6e hub/home/minicon
   0x00982520 64612f65 6e76732f 6275696c 645f6269 da/envs/build_bi
   0x00982530 6e617279 2f6c6962 2f707974 686f6e33 nary/lib/python3
-  0x00982540 2e392f73 6974652d 7061636b 61676573 .9/site-packages
+  0x00982540 2e382f73 6974652d 7061636b 61676573 .8/site-packages
   0x00982550 2f746f72 63682f69 6e636c75 64652f41 /torch/include/A
   0x00982560 54656e2f 636f7265 2f697661 6c75655f Ten/core/ivalue_
   0x00982570 696e6c2e 68223a32 3037322c 20706c65 inl.h":2072, ple
   0x00982580 61736520 7265706f 72742061 20627567 ase report a bug
   0x00982590 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x009825a0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009825b0 4d4d2f66 6267656d 6d5f6770 752f7372 MM/fbgemm_gpu/sr
@@ -13732,25 +13732,25 @@
   0x00982a10 6e744c69 73742062 75742067 6f742000 ntList but got .
   0x00982a20 69735379 6d496e74 4c697374 2829207c isSymIntList() |
   0x00982a30 7c206973 496e744c 69737428 2920494e | isIntList() IN
   0x00982a40 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x00982a50 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x00982a60 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x00982a70 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x00982a80 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x00982a80 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x00982a90 73697465 2d706163 6b616765 732f746f site-packages/to
   0x00982aa0 7263682f 696e636c 7564652f 4154656e rch/include/ATen
   0x00982ab0 2f636f72 652f6976 616c7565 5f696e6c /core/ivalue_inl
   0x00982ac0 2e68223a 31393834 2c20706c 65617365 .h":1984, please
   0x00982ad0 20726570 6f727420 61206275 6720746f  report a bug to
   0x00982ae0 20507954 6f726368 2e200000 00000000  PyTorch. ......
   0x00982af0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00982b00 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00982b10 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00982b20 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00982b20 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00982b30 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00982b40 64652f63 31302f63 6f72652f 53796d49 de/c10/core/SymI
   0x00982b50 6e742e68 00000000 45787065 63746564 nt.h....Expected
   0x00982b60 2064656e 73655f76 616c7565 735f6772  dense_values_gr
   0x00982b70 61642e73 796d5f73 697a6573 2829203d ad.sym_sizes() =
   0x00982b80 3d206465 6e73655f 73686170 6520746f = dense_shape to
   0x00982b90 20626520 74727565 2c206275 7420676f  be true, but go
@@ -13859,15 +13859,15 @@
   0x00983200 6820636f 6e746169 6e656420 74797065 h contained type
   0x00983210 73206469 64206e6f 74206f76 65726c6f s did not overlo
   0x00983220 61642063 72656174 65576974 68436f6e ad createWithCon
   0x00983230 7461696e 65643a20 00000000 00000000 tained: ........
   0x00983240 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00983250 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00983260 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00983270 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00983270 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00983280 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00983290 64652f41 54656e2f 636f7265 2f6a6974 de/ATen/core/jit
   0x009832a0 5f747970 655f6261 73652e68 00637265 _type_base.h.cre
   0x009832b0 61746557 69746843 6f6e7461 696e6564 ateWithContained
   0x009832c0 003b204c 656e6774 68203d20 00000000 .; Length = ....
   0x009832d0 41727261 79526566 3a20696e 76616c69 ArrayRef: invali
   0x009832e0 6420696e 64657820 496e6465 78203d20 d index Index = 
@@ -14452,35 +14452,35 @@
   0x00985710 45450000 00000000 00000000 78000000 EE..........x...
   0x00985720 69735379 6d496e74 2829207c 7c206973 isSymInt() || is
   0x00985730 496e7428 2920494e 5445524e 414c2041 Int() INTERNAL A
   0x00985740 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00985750 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x00985760 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x00985770 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x00985780 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x00985780 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x00985790 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x009857a0 7564652f 4154656e 2f636f72 652f6976 ude/ATen/core/iv
   0x009857b0 616c7565 5f696e6c 2e68223a 3234352c alue_inl.h":245,
   0x009857c0 20706c65 61736520 7265706f 72742061  please report a
   0x009857d0 20627567 20746f20 5079546f 7263682e  bug to PyTorch.
   0x009857e0 20005472 69656420 746f2063 61737420  .Tried to cast 
   0x009857f0 61204c69 73743c00 3e20746f 2061204c a List<.> to a L
   0x00985800 6973743c 003e2e20 54797065 73206d69 ist<.>. Types mi
   0x00985810 736d6174 63682e00 746f5479 7065644c smatch..toTypedL
   0x00985820 69737400 00000000 2f676974 6875622f ist...../github/
   0x00985830 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00985840 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00985850 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00985850 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00985860 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00985870 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00985880 636f7265 2f4c6973 745f696e 6c2e6800 core/List_inl.h.
   0x00985890 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x009858a0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x009858b0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x009858c0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x009858c0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x009858d0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x009858e0 64652f41 54656e2f 636f7265 2f626f78 de/ATen/core/box
   0x009858f0 696e672f 4b65726e 656c4675 6e637469 ing/KernelFuncti
   0x00985900 6f6e5f69 6d706c2e 68000000 00000000 on_impl.h.......
   0x00985910 45787065 63746564 20707472 5f2d3e69 Expected ptr_->i
   0x00985920 735f666c 6f617428 2920746f 20626520 s_float() to be 
   0x00985930 74727565 2c206275 7420676f 74206661 true, but got fa
@@ -14489,24 +14489,24 @@
   0x00985960 62652069 6d70726f 7665643f 20204966 be improved?  If
   0x00985970 20736f2c 20706c65 61736520 7265706f  so, please repo
   0x00985980 72742061 6e20656e 68616e63 656d656e rt an enhancemen
   0x00985990 74207265 71756573 7420746f 20507954 t request to PyT
   0x009859a0 6f726368 2e290000 2f676974 6875622f orch.)../github/
   0x009859b0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009859c0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009859d0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009859d0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009859e0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009859f0 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x00985a00 6f72652f 53796d46 6c6f6174 2e680000 ore/SymFloat.h..
   0x00985a10 3020494e 5445524e 414c2041 53534552 0 INTERNAL ASSER
   0x00985a20 54204641 494c4544 20617420 222f6769 T FAILED at "/gi
   0x00985a30 74687562 2f686f6d 652f6d69 6e69636f thub/home/minico
   0x00985a40 6e64612f 656e7673 2f627569 6c645f62 nda/envs/build_b
   0x00985a50 696e6172 792f6c69 622f7079 74686f6e inary/lib/python
-  0x00985a60 332e392f 73697465 2d706163 6b616765 3.9/site-package
+  0x00985a60 332e382f 73697465 2d706163 6b616765 3.8/site-package
   0x00985a70 732f746f 7263682f 696e636c 7564652f s/torch/include/
   0x00985a80 4154656e 2f636f72 652f6976 616c7565 ATen/core/ivalue
   0x00985a90 2e68223a 3534302c 20706c65 61736520 .h":540, please 
   0x00985aa0 7265706f 72742061 20627567 20746f20 report a bug to 
   0x00985ab0 5079546f 7263682e 20006578 70656374 PyTorch. .expect
   0x00985ac0 65642064 6f75626c 6500746f 446f7562 ed double.toDoub
   0x00985ad0 6c650000 00000000 00000000 00000000 le..............
@@ -15950,15 +15950,15 @@
   0x0098b4b0 6e646578 5f616464 5f32645f 666f7277 ndex_add_2d_forw
   0x0098b4c0 61726400 76656374 6f720000 00000000 ard.vector......
   0x0098b4d0 6973496e 744c6973 74282920 494e5445 isIntList() INTE
   0x0098b4e0 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x0098b4f0 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x0098b500 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x0098b510 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x0098b520 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x0098b520 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x0098b530 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x0098b540 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x0098b550 6f72652f 6976616c 75655f69 6e6c2e68 ore/ivalue_inl.h
   0x0098b560 223a3139 36382c20 706c6561 73652072 ":1968, please r
   0x0098b570 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x0098b580 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x0098b590 464e3261 74365465 6e736f72 45524b53 FN2at6TensorERKS
@@ -19590,15 +19590,15 @@
   0x00999830 01010101 01010201 01010102 04080101 ................
   0x00999840 01010101 01000000 00000000 70000000 ............p...
   0x00999850 6973496e 744c6973 74282920 494e5445 isIntList() INTE
   0x00999860 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x00999870 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x00999880 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x00999890 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x009998a0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x009998a0 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x009998b0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x009998c0 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x009998d0 6f72652f 6976616c 75655f69 6e6c2e68 ore/ivalue_inl.h
   0x009998e0 223a3139 37362c20 706c6561 73652072 ":1976, please r
   0x009998f0 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x00999900 79546f72 63682e20 00746f49 6e745665 yTorch. .toIntVe
   0x00999910 63746f72 00000000 62617463 685f696e ctor....batch_in
@@ -19755,15 +19755,15 @@
   0x0099a280 49662073 6f2c2070 6c656173 65207265 If so, please re
   0x0099a290 706f7274 20616e20 656e6861 6e63656d port an enhancem
   0x0099a2a0 656e7420 72657175 65737420 746f2050 ent request to P
   0x0099a2b0 79546f72 63682e29 00000000 00000000 yTorch.)........
   0x0099a2c0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0099a2d0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0099a2e0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0099a2f0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0099a2f0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0099a300 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0099a310 675f666f 72776172 645f7175 616e7469 g_forward_quanti
   0x0099a320 7a65645f 756e7765 69676874 65645f63 zed_unweighted_c
   0x0099a330 6f646567 656e5f63 70752e63 70700000 odegen_cpu.cpp..
   0x0099a340 696e7438 206f7574 70757420 61726520 int8 output are 
   0x0099a350 6f6e6c79 20737570 706f7274 65642066 only supported f
   0x0099a360 6f722069 6e743820 77656967 68747300 or int8 weights.
@@ -19896,15 +19896,15 @@
   0x0099ab50 90e5f2ff 80e5f2ff f0e6f2ff e0e6f2ff ................
   0x0099ab60 d0e6f2ff c0e6f2ff f0e5f2ff e0e5f2ff ................
   0x0099ab70 d0e5f2ff c0e5f2ff 50e5f2ff 40e5f2ff ........P...@...
   0x0099ab80 60e5f2ff 06050010 110f0000 00000000 `...............
   0x0099ab90 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0099aba0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0099abb0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0099abc0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0099abc0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0099abd0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0099abe0 675f666f 72776172 645f7175 616e7469 g_forward_quanti
   0x0099abf0 7a65645f 77656967 68746564 5f636f64 zed_weighted_cod
   0x0099ac00 6567656e 5f637075 2e637070 00000000 egen_cpu.cpp....
   0x0099ac10 7072756e 65645f68 6173686d 61705f6c pruned_hashmap_l
   0x0099ac20 6f6f6b75 705f7765 69676874 65645f63 ookup_weighted_c
   0x0099ac30 70750000 00000000 7072756e 65645f68 pu......pruned_h
@@ -19917,15 +19917,15 @@
   0x0099aca0 65696768 7473206d 75737420 62652065 eights must be e
   0x0099acb0 6d707479 206f7220 61204350 55207465 mpty or a CPU te
   0x0099acc0 6e736f72 3b206974 20697320 63757272 nsor; it is curr
   0x0099acd0 656e746c 79206f6e 20646576 69636520 ently on device 
   0x0099ace0 00000000 00000000 2f5f5f77 2f464247 ......../__w/FBG
   0x0099acf0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0099ad00 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0099ad10 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0099ad10 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0099ad20 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0099ad30 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0099ad40 72645f64 656e7365 5f73706c 69745f63 rd_dense_split_c
   0x0099ad50 70752e63 70700000 43686563 6b206661 pu.cpp..Check fa
   0x0099ad60 696c6564 3a20686f 73745f77 65696768 iled: host_weigh
   0x0099ad70 74732e64 696d2829 203d3d20 31202800 ts.dim() == 1 (.
   0x0099ad80 73706c69 745f656d 62656464 696e675f split_embedding_
@@ -20005,15 +20005,15 @@
   0x0099b220 70706572 00000000 73706c69 745f656d pper....split_em
   0x0099b230 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x0099b240 666f7277 6172645f 756e7765 69676874 forward_unweight
   0x0099b250 65645f70 74325f77 72617070 65720000 ed_pt2_wrapper..
   0x0099b260 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0099b270 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0099b280 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0099b290 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0099b290 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0099b2a0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0099b2b0 675f666f 72776172 645f7370 6c69745f g_forward_split_
   0x0099b2c0 7074325f 6370755f 77726170 7065722e pt2_cpu_wrapper.
   0x0099b2d0 63707000 00000000 66626765 6d6d3a3a cpp.....fbgemm::
   0x0099b2e0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0099b2f0 636f6465 67656e5f 67726164 5f696e64 codegen_grad_ind
   0x0099b300 6963655f 77656967 6874735f 63707500 ice_weights_cpu.
@@ -20144,15 +20144,15 @@
   0x0099bad0 3d302920 2d3e2054 656e736f 72000000 =0) -> Tensor...
   0x0099bae0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0099baf0 636f6465 67656e5f 6c6f6f6b 75705f61 codegen_lookup_a
   0x0099bb00 64616772 61645f66 756e6374 696f6e5f dagrad_function_
   0x0099bb10 63707500 00000000 2f5f5f77 2f464247 cpu...../__w/FBG
   0x0099bb20 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0099bb30 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0099bb40 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0099bb40 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0099bb50 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0099bb60 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0099bb70 72645f73 706c6974 5f616461 67726164 rd_split_adagrad
   0x0099bb80 5f637075 2e637070 00000000 00000000 _cpu.cpp........
   0x0099bb90 66626765 6d6d3a3a 73706c69 745f656d fbgemm::split_em
   0x0099bba0 62656464 696e675f 6261636b 77617264 bedding_backward
   0x0099bbb0 5f636f64 6567656e 5f616461 67726164 _codegen_adagrad
@@ -20267,15 +20267,15 @@
   0x0099c280 c05ef5ff a85ef5ff 905ef5ff 785ef5ff .^...^...^..x^..
   0x0099c290 605ef5ff 485ef5ff 305ef5ff 205ef5ff `^..H^..0^.. ^..
   0x0099c2a0 105ef5ff 005ef5ff f05df5ff e05df5ff .^...^...]...]..
   0x0099c2b0 d05df5ff a85df5ff f85ff5ff 00000000 .]...]..._......
   0x0099c2c0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0099c2d0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0099c2e0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0099c2f0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0099c2f0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0099c300 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0099c310 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0099c320 5f616461 67726164 5f707432 5f637075 _adagrad_pt2_cpu
   0x0099c330 5f777261 70706572 2e637070 00000000 _wrapper.cpp....
   0x0099c340 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0099c350 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x0099c360 5f616461 67726164 5f776569 67687465 _adagrad_weighte
@@ -20389,15 +20389,15 @@
   0x0099ca20 00000000 00000000 73706c69 745f656d ........split_em
   0x0099ca30 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x0099ca40 6c6f6f6b 75705f72 6f777769 73655f61 lookup_rowwise_a
   0x0099ca50 64616772 61645f66 756e6374 696f6e5f dagrad_function_
   0x0099ca60 63707500 00000000 2f5f5f77 2f464247 cpu...../__w/FBG
   0x0099ca70 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0099ca80 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0099ca90 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0099ca90 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0099caa0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0099cab0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0099cac0 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x0099cad0 5f616461 67726164 5f637075 2e637070 _adagrad_cpu.cpp
   0x0099cae0 00000000 00000000 66626765 6d6d3a3a ........fbgemm::
   0x0099caf0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0099cb00 6261636b 77617264 5f636f64 6567656e backward_codegen
@@ -20517,15 +20517,15 @@
   0x0099d220 7caef6ff 64aef6ff 4caef6ff 34aef6ff |...d...L...4...
   0x0099d230 1caef6ff 04aef6ff ecadf6ff d4adf6ff ................
   0x0099d240 bcadf6ff a4adf6ff 94adf6ff 84adf6ff ................
   0x0099d250 74adf6ff 64adf6ff 54adf6ff 44adf6ff t...d...T...D...
   0x0099d260 1cadf6ff 6caff6ff 2f5f5f77 2f464247 ....l.../__w/FBG
   0x0099d270 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0099d280 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0099d290 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0099d290 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0099d2a0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0099d2b0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0099d2c0 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x0099d2d0 5f616461 67726164 5f707432 5f637075 _adagrad_pt2_cpu
   0x0099d2e0 5f777261 70706572 2e637070 00000000 _wrapper.cpp....
   0x0099d2f0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0099d300 6261636b 77617264 5f636f64 6567656e backward_codegen
@@ -20629,15 +20629,15 @@
   0x0099d920 745f6474 7970653d 3029202d 3e205465 t_dtype=0) -> Te
   0x0099d930 6e736f72 00000000 73706c69 745f656d nsor....split_em
   0x0099d940 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x0099d950 6c6f6f6b 75705f73 67645f66 756e6374 lookup_sgd_funct
   0x0099d960 696f6e5f 63707500 2f5f5f77 2f464247 ion_cpu./__w/FBG
   0x0099d970 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0099d980 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0099d990 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0099d990 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0099d9a0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0099d9b0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0099d9c0 72645f73 706c6974 5f736764 5f637075 rd_split_sgd_cpu
   0x0099d9d0 2e637070 00000000 66626765 6d6d3a3a .cpp....fbgemm::
   0x0099d9e0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0099d9f0 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x0099da00 5f736764 5f637075 00000000 00000000 _sgd_cpu........
@@ -20745,15 +20745,15 @@
   0x0099e060 c0ddf7ff a8ddf7ff 90ddf7ff 78ddf7ff ............x...
   0x0099e070 60ddf7ff 48ddf7ff 30ddf7ff 20ddf7ff `...H...0... ...
   0x0099e080 10ddf7ff 00ddf7ff f0dcf7ff e0dcf7ff ................
   0x0099e090 d0dcf7ff a8dcf7ff f8def7ff 00000000 ................
   0x0099e0a0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0099e0b0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0099e0c0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0099e0d0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0099e0d0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0099e0e0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0099e0f0 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0099e100 5f736764 5f707432 5f637075 5f777261 _sgd_pt2_cpu_wra
   0x0099e110 70706572 2e637070 00000000 00000000 pper.cpp........
   0x0099e120 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0099e130 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x0099e140 5f736764 5f776569 67687465 645f6578 _sgd_weighted_ex
@@ -20825,15 +20825,15 @@
   0x0099e560 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x0099e570 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x0099e580 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x0099e590 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x0099e5a0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0099e5b0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0099e5c0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0099e5d0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0099e5d0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0099e5e0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0099e5f0 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0099e600 5f616461 6d5f6370 752e6370 70000000 _adam_cpu.cpp...
   0x0099e610 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0099e620 636f6465 67656e5f 6c6f6f6b 75705f61 codegen_lookup_a
   0x0099e630 64616d5f 66756e63 74696f6e 5f637075 dam_function_cpu
   0x0099e640 00000000 00000000 73706c69 745f656d ........split_em
@@ -20930,15 +20930,15 @@
   0x0099ebf0 65652068 74747073 3a2f2f67 69746875 ee https://githu
   0x0099ec00 622e636f 6d2f7079 746f7263 682f4642 b.com/pytorch/FB
   0x0099ec10 47454d4d 2f646973 63757373 696f6e73 GEMM/discussions
   0x0099ec20 2f313732 3720666f 72206d6f 72652064 /1727 for more d
   0x0099ec30 65746169 6c2e0000 2f5f5f77 2f464247 etail.../__w/FBG
   0x0099ec40 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0099ec50 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0099ec60 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0099ec60 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0099ec70 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0099ec80 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0099ec90 72645f73 706c6974 5f6c616d 625f6370 rd_split_lamb_cp
   0x0099eca0 752e6370 70000000 73706c69 745f656d u.cpp...split_em
   0x0099ecb0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x0099ecc0 6c6f6f6b 75705f6c 616d625f 66756e63 lookup_lamb_func
   0x0099ecd0 74696f6e 5f637075 00000000 00000000 tion_cpu........
@@ -21029,15 +21029,15 @@
   0x0099f220 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x0099f230 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x0099f240 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x0099f250 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x0099f260 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0099f270 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0099f280 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0099f290 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0099f290 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0099f2a0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0099f2b0 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0099f2c0 5f706172 7469616c 5f726f77 77697365 _partial_rowwise
   0x0099f2d0 5f616461 6d5f6370 752e6370 70000000 _adam_cpu.cpp...
   0x0099f2e0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0099f2f0 636f6465 67656e5f 6c6f6f6b 75705f70 codegen_lookup_p
   0x0099f300 61727469 616c5f72 6f777769 73655f61 artial_rowwise_a
@@ -21132,15 +21132,15 @@
   0x0099f890 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x0099f8a0 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x0099f8b0 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x0099f8c0 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x0099f8d0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0099f8e0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0099f8f0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0099f900 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0099f900 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0099f910 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0099f920 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0099f930 5f706172 7469616c 5f726f77 77697365 _partial_rowwise
   0x0099f940 5f6c616d 625f6370 752e6370 70000000 _lamb_cpu.cpp...
   0x0099f950 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0099f960 636f6465 67656e5f 6c6f6f6b 75705f70 codegen_lookup_p
   0x0099f970 61727469 616c5f72 6f777769 73655f6c artial_rowwise_l
@@ -21235,15 +21235,15 @@
   0x0099ff00 74747073 3a2f2f67 69746875 622e636f ttps://github.co
   0x0099ff10 6d2f7079 746f7263 682f4642 47454d4d m/pytorch/FBGEMM
   0x0099ff20 2f646973 63757373 696f6e73 2f313732 /discussions/172
   0x0099ff30 3720666f 72206d6f 72652064 65746169 7 for more detai
   0x0099ff40 6c2e0000 00000000 2f5f5f77 2f464247 l......./__w/FBG
   0x0099ff50 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0099ff60 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0099ff70 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0099ff70 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0099ff80 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0099ff90 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0099ffa0 72645f73 706c6974 5f6c6172 735f7367 rd_split_lars_sg
   0x0099ffb0 645f6370 752e6370 70000000 00000000 d_cpu.cpp.......
   0x0099ffc0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0099ffd0 636f6465 67656e5f 6c6f6f6b 75705f6c codegen_lookup_l
   0x0099ffe0 6172735f 7367645f 66756e63 74696f6e ars_sgd_function
@@ -21334,15 +21334,15 @@
   0x009a0530 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x009a0540 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x009a0550 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x009a0560 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x009a0570 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009a0580 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009a0590 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009a05a0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009a05a0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009a05b0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009a05c0 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009a05d0 5f6e6f6e 655f6370 752e6370 70000000 _none_cpu.cpp...
   0x009a05e0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009a05f0 636f6465 67656e5f 6c6f6f6b 75705f6e codegen_lookup_n
   0x009a0600 6f6e655f 66756e63 74696f6e 5f637075 one_function_cpu
   0x009a0610 00000000 00000000 73706c69 745f656d ........split_em
@@ -21420,15 +21420,15 @@
   0x009a0a90 65652068 74747073 3a2f2f67 69746875 ee https://githu
   0x009a0aa0 622e636f 6d2f7079 746f7263 682f4642 b.com/pytorch/FB
   0x009a0ab0 47454d4d 2f646973 63757373 696f6e73 GEMM/discussions
   0x009a0ac0 2f313732 3720666f 72206d6f 72652064 /1727 for more d
   0x009a0ad0 65746169 6c2e0000 2f5f5f77 2f464247 etail.../__w/FBG
   0x009a0ae0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009a0af0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009a0b00 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009a0b00 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009a0b10 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009a0b20 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009a0b30 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009a0b40 5f616461 67726164 5f776974 685f636f _adagrad_with_co
   0x009a0b50 756e7465 725f6370 752e6370 70000000 unter_cpu.cpp...
   0x009a0b60 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009a0b70 636f6465 67656e5f 6c6f6f6b 75705f72 codegen_lookup_r
@@ -21562,15 +21562,15 @@
   0x009a1370 2f676974 6875622e 636f6d2f 7079746f /github.com/pyto
   0x009a1380 7263682f 46424745 4d4d2f64 69736375 rch/FBGEMM/discu
   0x009a1390 7373696f 6e732f31 37323720 666f7220 ssions/1727 for 
   0x009a13a0 6d6f7265 20646574 61696c2e 00000000 more detail.....
   0x009a13b0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009a13c0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009a13d0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009a13e0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009a13e0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009a13f0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009a1400 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009a1410 5f617070 726f785f 7367645f 6370752e _approx_sgd_cpu.
   0x009a1420 63707000 00000000 73706c69 745f656d cpp.....split_em
   0x009a1430 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009a1440 6c6f6f6b 75705f61 7070726f 785f7367 lookup_approx_sg
   0x009a1450 645f6675 6e637469 6f6e5f63 70750000 d_function_cpu..
@@ -21643,15 +21643,15 @@
   0x009a1880 70733a2f 2f676974 6875622e 636f6d2f ps://github.com/
   0x009a1890 7079746f 7263682f 46424745 4d4d2f64 pytorch/FBGEMM/d
   0x009a18a0 69736375 7373696f 6e732f31 37323720 iscussions/1727 
   0x009a18b0 666f7220 6d6f7265 20646574 61696c2e for more detail.
   0x009a18c0 00000000 00000000 2f5f5f77 2f464247 ......../__w/FBG
   0x009a18d0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009a18e0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009a18f0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009a18f0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009a1900 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009a1910 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009a1920 72645f73 706c6974 5f617070 726f785f rd_split_approx_
   0x009a1930 726f7777 6973655f 61646167 7261645f rowwise_adagrad_
   0x009a1940 6370752e 63707000 73706c69 745f656d cpu.cpp.split_em
   0x009a1950 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009a1960 6c6f6f6b 75705f61 7070726f 785f726f lookup_approx_ro
@@ -21746,15 +21746,15 @@
   0x009a1ef0 2f2f6769 74687562 2e636f6d 2f707974 //github.com/pyt
   0x009a1f00 6f726368 2f464247 454d4d2f 64697363 orch/FBGEMM/disc
   0x009a1f10 75737369 6f6e732f 31373237 20666f72 ussions/1727 for
   0x009a1f20 206d6f72 65206465 7461696c 2e000000  more detail....
   0x009a1f30 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009a1f40 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009a1f50 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009a1f60 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009a1f60 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009a1f70 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009a1f80 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009a1f90 5f617070 726f785f 726f7777 6973655f _approx_rowwise_
   0x009a1fa0 61646167 7261645f 77697468 5f636f75 adagrad_with_cou
   0x009a1fb0 6e746572 5f637075 2e637070 00000000 nter_cpu.cpp....
   0x009a1fc0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009a1fd0 636f6465 67656e5f 6c6f6f6b 75705f61 codegen_lookup_a
@@ -21882,15 +21882,15 @@
   0x009a2770 69746875 622e636f 6d2f7079 746f7263 ithub.com/pytorc
   0x009a2780 682f4642 47454d4d 2f646973 63757373 h/FBGEMM/discuss
   0x009a2790 696f6e73 2f313732 3720666f 72206d6f ions/1727 for mo
   0x009a27a0 72652064 65746169 6c2e0000 00000000 re detail.......
   0x009a27b0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009a27c0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009a27d0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009a27e0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009a27e0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009a27f0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009a2800 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009a2810 5f617070 726f785f 726f7777 6973655f _approx_rowwise_
   0x009a2820 61646167 7261645f 77697468 5f776569 adagrad_with_wei
   0x009a2830 6768745f 64656361 795f6370 752e6370 ght_decay_cpu.cp
   0x009a2840 70000000 00000000 73706c69 745f656d p.......split_em
   0x009a2850 62656464 696e675f 636f6465 67656e5f bedding_codegen_
@@ -21982,15 +21982,15 @@
   0x009a2db0 68747470 733a2f2f 67697468 75622e63 https://github.c
   0x009a2dc0 6f6d2f70 79746f72 63682f46 4247454d om/pytorch/FBGEM
   0x009a2dd0 4d2f6469 73637573 73696f6e 732f3137 M/discussions/17
   0x009a2de0 32372066 6f72206d 6f726520 64657461 27 for more deta
   0x009a2df0 696c2e00 00000000 2f5f5f77 2f464247 il....../__w/FBG
   0x009a2e00 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009a2e10 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009a2e20 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009a2e20 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009a2e30 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009a2e40 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009a2e50 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009a2e60 5f616461 67726164 5f776974 685f7765 _adagrad_with_we
   0x009a2e70 69676874 5f646563 61795f63 70752e63 ight_decay_cpu.c
   0x009a2e80 70700000 00000000 73706c69 745f656d pp......split_em
   0x009a2e90 62656464 696e675f 636f6465 67656e5f bedding_codegen_
@@ -22081,15 +22081,15 @@
   0x009a33e0 74747073 3a2f2f67 69746875 622e636f ttps://github.co
   0x009a33f0 6d2f7079 746f7263 682f4642 47454d4d m/pytorch/FBGEMM
   0x009a3400 2f646973 63757373 696f6e73 2f313732 /discussions/172
   0x009a3410 3720666f 72206d6f 72652064 65746169 7 for more detai
   0x009a3420 6c2e0000 00000000 2f5f5f77 2f464247 l......./__w/FBG
   0x009a3430 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009a3440 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009a3450 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009a3450 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009a3460 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009a3470 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009a3480 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009a3490 5f776569 67687465 645f6164 61677261 _weighted_adagra
   0x009a34a0 645f6370 752e6370 70000000 00000000 d_cpu.cpp.......
   0x009a34b0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009a34c0 636f6465 67656e5f 6c6f6f6b 75705f72 codegen_lookup_r
@@ -22182,15 +22182,15 @@
   0x009a3a30 0891f9ff f090f9ff d890f9ff c090f9ff ................
   0x009a3a40 a890f9ff 9090f9ff 7890f9ff 6090f9ff ........x...`...
   0x009a3a50 4890f9ff 3890f9ff 2890f9ff 1890f9ff H...8...(.......
   0x009a3a60 0890f9ff f88ff9ff e88ff9ff c08ff9ff ................
   0x009a3a70 1092f9ff 00000000 2f5f5f77 2f464247 ......../__w/FBG
   0x009a3a80 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009a3a90 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009a3aa0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009a3aa0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009a3ab0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009a3ac0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009a3ad0 72645f61 64616772 61645f73 706c6974 rd_adagrad_split
   0x009a3ae0 5f637075 2e637070 00000000 00000000 _cpu.cpp........
   0x009a3af0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009a3b00 6261636b 77617264 5f657861 63745f63 backward_exact_c
   0x009a3b10 70755f6f 75746572 00000000 00000000 pu_outer........
@@ -22269,15 +22269,15 @@
   0x009a3fa0 2815faff 1815faff 0815faff e014faff (...............
   0x009a3fb0 3017faff 00000000 6e756d20 6f662072 0.......num of r
   0x009a3fc0 6f777320 70726f63 65737365 64206279 ows processed by
   0x009a3fd0 20616461 67726164 3a200000 00000000  adagrad: ......
   0x009a3fe0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009a3ff0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009a4000 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009a4010 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009a4010 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009a4020 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009a4030 675f6261 636b7761 72645f72 6f777769 g_backward_rowwi
   0x009a4040 73655f61 64616772 61645f73 706c6974 se_adagrad_split
   0x009a4050 5f637075 2e637070 00000000 00000000 _cpu.cpp........
   0x009a4060 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009a4070 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x009a4080 5f726f77 77697365 5f616461 67726164 _rowwise_adagrad
@@ -22349,15 +22349,15 @@
   0x009a44a0 7c78faff 6478faff 4c78faff 3478faff |x..dx..Lx..4x..
   0x009a44b0 1c78faff 0478faff ec77faff d477faff .x...x...w...w..
   0x009a44c0 bc77faff a477faff 9477faff 8477faff .w...w...w...w..
   0x009a44d0 7477faff 6477faff 5477faff 4477faff tw..dw..Tw..Dw..
   0x009a44e0 1c77faff 6c79faff 2f5f5f77 2f464247 .w..ly../__w/FBG
   0x009a44f0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009a4500 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009a4510 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009a4510 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009a4520 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009a4530 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009a4540 72645f73 67645f73 706c6974 5f637075 rd_sgd_split_cpu
   0x009a4550 2e637070 00000000 73706c69 745f656d .cpp....split_em
   0x009a4560 62656464 696e675f 6261636b 77617264 bedding_backward
   0x009a4570 5f636f64 6567656e 5f736764 5f637075 _codegen_sgd_cpu
   0x009a4580 2854656e 736f7220 67726164 5f6f7574 (Tensor grad_out
```

## fbgemm_gpu/docs/version.py

```diff
@@ -2,8 +2,8 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-__version__: str = "2024.5.3"
+__version__: str = "2024.5.4"
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2024.5.3
+Version: 2024.5.4
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 fbgemm_gpu/__init__.py,sha256=ZPy0iaSSHb6-eT6lz8MSpr-5Ircj9SLmVpL0o0ejcNQ,914
 fbgemm_gpu/batched_unary_embeddings_ops.py,sha256=dpxZAueNsadJVuK7Dwo8GbOlho9r67Lfh8kesqRKJNI,3079
 fbgemm_gpu/enums.py,sha256=GVuzF5cFTLzttkvlH1SdcGrxrppMhDSbQj_Vm_4zmEo,789
-fbgemm_gpu/fbgemm_gpu_py.so,sha256=i1LXi4SfQ7QLpOtOfH7_qkxVyUobnLLL2JlNPvZYS_M,10846712
+fbgemm_gpu/fbgemm_gpu_py.so,sha256=XjV-OL7__CINpywGBCRKIL5pGM3vJHUtgCeD0GXIp94,10846712
 fbgemm_gpu/metrics.py,sha256=TsurFLJf0nJvPDN7urWb4LMQlf5RgdWPTTTDO7S4wtI,5663
 fbgemm_gpu/permute_pooled_embedding_modules.py,sha256=4mHJ2fo3SeG25iSwdm2YsM8q_oWsF1LxRguYmxSnuDI,2362
 fbgemm_gpu/permute_pooled_embedding_modules_split.py,sha256=cUrEbRIvLFW_3Zmh07QkN4S1Cfvvge6TYO1VXBFCpz8,2752
 fbgemm_gpu/quantize_comm.py,sha256=UZcVSC2JQ0oSkwsJQnjaZ2k8mm2p3hvVzpyg7X5xFXM,7885
 fbgemm_gpu/quantize_utils.py,sha256=-vwHIEkyStDo1TWoYfwmC5U6DvR6iRMHXyjFc9lO_p8,4143
 fbgemm_gpu/runtime_monitor.py,sha256=tIdxkJIWkJ8705btxs9NqzEXC7QprFh3sA8Q4LpvtJ8,6947
 fbgemm_gpu/sparse_ops.py,sha256=4SyIpm3Rw2pHPm4NzsnD6GrisufwQ3v-_bbdYhkyIOc,20601
@@ -20,15 +20,15 @@
 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py,sha256=S6qWfFzpqNIB8l9N3LAsYfaXSExg53f_b3fl47d1b1U,40680
 fbgemm_gpu/uvm.py,sha256=-cZunsuvnAKUEQptIwdYVar_3hUE99FbQUsyfBVeXPE,925
 fbgemm_gpu/docs/__init__.py,sha256=BbAfYbNZsBhO7L5Am4wyBLet4mTY2aXFucyGTxF9IlI,383
 fbgemm_gpu/docs/common.py,sha256=8ipXTwVb222X-aZ71O6n8fhxHCHPNhJEHMFiO7epcIs,273
 fbgemm_gpu/docs/examples.py,sha256=ZMN_6sL74LH_hrp2bF_hmg8gi29GhcgvwV3kCMjxkoE,2377
 fbgemm_gpu/docs/jagged_tensor_ops.py,sha256=Bsx-ZxvvdMv5CaldSvuw9GPR-HRcLbRR2IEXCOCm9r0,7381
 fbgemm_gpu/docs/table_batched_embedding_ops.py,sha256=h_EQOIMsdVlr-Pygul-fDGxx7JqLRjaBMI_z0PFrGAE,7708
-fbgemm_gpu/docs/version.py,sha256=e6pZ7LnfzQr3p-nLPRmgzVsCoDuKkbmkSBbeq3wEkgc,263
+fbgemm_gpu/docs/version.py,sha256=-Faaohgm67QcjOIL6ovHpD8RP5xBWDHmtvHPnrV8j-A,263
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py,sha256=lfob_IDNeAs2FjS2WCldKlw0gm_qUZdp043fngI8sGE,1466
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py,sha256=x17z36WrjIloP-pLVzyxpxjats7XjxJZv8OysT9JxD4,4180
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py,sha256=x17z36WrjIloP-pLVzyxpxjats7XjxJZv8OysT9JxD4,4180
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py,sha256=EBR6BEDV_SOuJM_yGq4IEfdL8umYkAmCWekcAwpHpNQ,3395
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py,sha256=EBR6BEDV_SOuJM_yGq4IEfdL8umYkAmCWekcAwpHpNQ,3395
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py,sha256=ibfUa6H9BY85_e9VgbKujKi4nuR7Mgyw77VbFMkLKCs,2147
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py,sha256=xhDnYR0vVDSK96nbcNSs5NbGXqFF3FGIs3DPDBJYt08,3395
@@ -45,11 +45,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py,sha256=Aljkdf4GB0zetL2j5YIhTZaOqiIMIlQ9iTDM421lbiM,4512
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=Qr3xtASUsgNbPJD46__jyKkR3xy0n-n2IZSa5QPD-NA,3964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py,sha256=Qr3xtASUsgNbPJD46__jyKkR3xy0n-n2IZSa5QPD-NA,3964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=fOgbq-u3VtbtKFqLTGQJiCwoHpa_xP-rBIvj98S78F4,3762
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py,sha256=fOgbq-u3VtbtKFqLTGQJiCwoHpa_xP-rBIvj98S78F4,3762
 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py,sha256=yiD3_bG5yT5VXLoGw4eeRKQ2Nj087DRq0qKCVPb52SY,649
 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py,sha256=OFw5PM2YDiKvr6T9ZW7BKiq58gB7txcKfuJkBUROxdI,6162
-fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/METADATA,sha256=F11RbIOegyjJK0p5-67kbuFcpAf5Rk9Cv1myjrdJNWA,2601
-fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/WHEEL,sha256=AdAOsf8BL1uIBxiEcIdcPDjJWWb0G5USb4X4msVaesE,105
-fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2024.5.3.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/METADATA,sha256=vhbQBJTQC_JpcPdBqTjx6AboiYTlc7x32228WymfUpE,2601
+fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/WHEEL,sha256=OEmkRrFcnutAqrz0YyBUaC3hh1288y58dKLCWma58N0,105
+fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2024.5.4.dist-info/RECORD,,
```

