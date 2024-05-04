# Comparing `tmp/vllm_acc-0.4.1.tar.gz` & `tmp/vllm_acc-0.4.11714782966.854302.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vllm_acc-0.4.1.tar", last modified: Sat May  4 00:12:42 2024, max compression
+gzip compressed data, was "vllm_acc-0.4.11714782966.854302.tar", last modified: Sat May  4 00:36:07 2024, max compression
```

## Comparing `vllm_acc-0.4.1.tar` & `vllm_acc-0.4.11714782966.854302.tar`

### file list

```diff
@@ -1,416 +1,416 @@
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.595488 vllm_acc-0.4.1/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9065 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/CMakeLists.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11357 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/LICENSE
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      153 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/MANIFEST.in
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8244 2024-05-04 00:12:42.595488 vllm_acc-0.4.1/PKG-INFO
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7444 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/README.md
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.559488 vllm_acc-0.4.1/cmake/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2241 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/cmake/cpu_extension.cmake
--rwxrwxr-x   0 azureuser  (1000) azureuser  (1000)     2308 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/cmake/hipify.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12858 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/cmake/utils.cmake
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.559488 vllm_acc-0.4.1/csrc/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6588 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/activation_kernels.cu
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.559488 vllm_acc-0.4.1/csrc/attention/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      160 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/attention/attention_dtypes.h
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1721 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/attention/attention_generic.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    44264 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/attention/attention_kernels.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1867 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/attention/attention_utils.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11580 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/attention/dtype_bfloat16.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12012 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/attention/dtype_float16.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5641 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/attention/dtype_float32.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      555 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/attention/dtype_fp8.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      681 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/cache.h
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13638 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/cache_kernels.cu
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.559488 vllm_acc-0.4.1/csrc/cpu/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5120 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/cpu/activation.cpp
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    32175 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/cpu/attention.cpp
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5794 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/cpu/cache.cpp
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10374 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/cpu/cpu_types.hpp
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4088 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/cpu/layernorm.cpp
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7447 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/cpu/pos_encoding.cpp
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1858 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/cpu/pybind.cpp
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      958 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/cuda_compat.h
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      184 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/cuda_utils.h
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      837 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/cuda_utils_kernels.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5757 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/custom_all_reduce.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    17097 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/custom_all_reduce.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12170 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/custom_all_reduce_test.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1679 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/dispatch_utils.h
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13097 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/layernorm_kernels.cu
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.563488 vllm_acc-0.4.1/csrc/moe/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      182 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/moe/moe_ops.cpp
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      197 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/moe/moe_ops.h
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20741 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/moe/topk_softmax_kernels.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4942 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/moe_align_block_size_kernels.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5005 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/ops.h
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8750 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/pos_encoding_kernels.cu
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.563488 vllm_acc-0.4.1/csrc/punica/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11807 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/punica/LICENSE
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.563488 vllm_acc-0.4.1/csrc/punica/bgmv/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      214 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/punica/bgmv/bgmv_bf16_bf16_bf16.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      202 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/punica/bgmv/bgmv_bf16_fp32_bf16.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6415 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/punica/bgmv/bgmv_config.h
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      190 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/punica/bgmv/bgmv_fp16_fp16_fp16.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      186 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/punica/bgmv/bgmv_fp16_fp32_fp16.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      202 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/punica/bgmv/bgmv_fp32_bf16_bf16.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      186 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/punica/bgmv/bgmv_fp32_fp16_fp16.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11313 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/punica/bgmv/bgmv_impl.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2055 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/punica/bgmv/generator.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    41110 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/punica/bgmv/vec_dtypes.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    25047 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/punica/punica_ops.cc
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4610 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/pybind.cpp
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.551488 vllm_acc-0.4.1/csrc/quantization/
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.563488 vllm_acc-0.4.1/csrc/quantization/aqlm/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20265 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/aqlm/gemm_kernels.cu
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.563488 vllm_acc-0.4.1/csrc/quantization/awq/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4155 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/awq/dequantize.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    21103 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/awq/gemm_kernels.cu
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.563488 vllm_acc-0.4.1/csrc/quantization/fp8/
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.563488 vllm_acc-0.4.1/csrc/quantization/fp8/amd_detail/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3973 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/fp8/amd_detail/hip_float8.h
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11019 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/fp8/amd_detail/hip_float8_impl.h
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13443 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/fp8/amd_detail/quant_utils.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3934 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/fp8/fp8_cuda_kernels.cu
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.563488 vllm_acc-0.4.1/csrc/quantization/fp8_e5m2_kvcache/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6770 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/fp8_e5m2_kvcache/quant_utils.cuh
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.563488 vllm_acc-0.4.1/csrc/quantization/gptq/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1703 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/gptq/compat.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9354 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/gptq/matrix_view.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    64637 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/gptq/q_gemm.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2598 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/gptq/qdq_2.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5053 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/gptq/qdq_3.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4169 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/gptq/qdq_4.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      723 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/gptq/qdq_8.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1407 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/gptq/qdq_util.cuh
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.567488 vllm_acc-0.4.1/csrc/quantization/gptq_marlin/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    58283 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/gptq_marlin/gptq_marlin.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2306 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/gptq_marlin/gptq_marlin.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10771 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/gptq_marlin/gptq_marlin_repack.cu
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.567488 vllm_acc-0.4.1/csrc/quantization/marlin/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11690 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/marlin/LICENSE
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    45316 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/marlin/marlin_cuda_kernel.cu
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.567488 vllm_acc-0.4.1/csrc/quantization/squeezellm/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5494 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/quantization/squeezellm/quant_cuda_kernel.cu
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2385 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/csrc/reduction_utils.cuh
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1281 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/pyproject.toml
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      603 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/requirements-common.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      251 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/requirements-cuda.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2024-05-04 00:12:42.595488 vllm_acc-0.4.1/setup.cfg
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14141 2024-05-03 23:33:49.000000 vllm_acc-0.4.1/setup.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.567488 vllm_acc-0.4.1/tests/
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.567488 vllm_acc-0.4.1/tests/core/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/__init__.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.567488 vllm_acc-0.4.1/tests/core/block/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/block/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      360 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/block/conftest.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3753 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/block/test_block_manager_v2.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    22046 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/block/test_block_table.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1246 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/block/test_common.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3864 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/block/test_cpu_gpu_block_allocator.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4001 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/block/test_naive_block.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20684 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/block/test_prefix_caching_block.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13753 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/test_block_manager.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    22188 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/test_chunked_prefill_scheduler.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    34201 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/test_scheduler.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2139 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/core/utils.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.571488 vllm_acc-0.4.1/tests/lora/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5399 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/conftest.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4673 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_baichuan.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3098 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_chatglm3.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1549 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_gemma.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6393 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_layer_variation.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    29994 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_layers.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10194 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_llama.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8094 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_lora.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2357 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_lora_checkpoints.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    19701 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_lora_manager.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4656 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_mixtral.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6502 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_punica.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5793 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_quant_model.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2197 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_tokenizer_group.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4325 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_utils.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2458 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/test_worker.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2846 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/lora/utils.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.571488 vllm_acc-0.4.1/tests/spec_decode/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/__init__.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.571488 vllm_acc-0.4.1/tests/spec_decode/e2e/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/e2e/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8688 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/e2e/conftest.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5190 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/e2e/test_compatibility.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    18322 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/e2e/test_multistep_correctness.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6005 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/e2e/test_ngram_correctness.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3146 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/test_batch_expansion.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6098 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/test_metrics.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13869 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/test_multi_step_worker.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6594 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/test_ngram_worker.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    24897 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/test_spec_decode_worker.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3080 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/test_utils.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8680 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/spec_decode/utils.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.571488 vllm_acc-0.4.1/tests/tensorizer_loader/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/tensorizer_loader/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8755 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/tensorizer_loader/tensorize_vllm_model_for_testing.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12383 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/tensorizer_loader/test_tensorizer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3501 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/test_cache_block_hashing.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1324 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/test_config.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      465 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/test_logger.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3820 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/test_logits_processor.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1732 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/test_regression.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      289 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/test_sampling_params.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4210 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/test_sequence.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.571488 vllm_acc-0.4.1/tests/tokenization/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/tokenization/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      896 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/tokenization/test_cached_tokenizer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8016 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/tokenization/test_detokenize.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      644 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/tokenization/test_tokenizer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3813 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/tokenization/test_tokenizer_group.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.571488 vllm_acc-0.4.1/tests/worker/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/worker/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14526 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/worker/test_model_runner.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3118 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/tests/worker/test_swap.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.575488 vllm_acc-0.4.1/vllm/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      742 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9150 2024-05-02 22:06:13.000000 vllm_acc-0.4.1/vllm/_custom_ops.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.575488 vllm_acc-0.4.1/vllm/attention/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      436 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/__init__.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.575488 vllm_acc-0.4.1/vllm/attention/backends/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/backends/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3578 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/backends/abstract.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11167 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/backends/flash_attn.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14823 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/backends/rocm_flash_attn.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9666 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/backends/torch_sdpa.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16245 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/backends/xformers.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1925 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/layer.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.575488 vllm_acc-0.4.1/vllm/attention/ops/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/ops/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7006 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/ops/paged_attn.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    26579 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/ops/prefix_prefill.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    27247 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/ops/triton_flash_attention.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2910 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/attention/selector.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2374 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/block.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    50305 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/config.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.575488 vllm_acc-0.4.1/vllm/core/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/__init__.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.579488 vllm_acc-0.4.1/vllm/core/block/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/block/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11618 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/block/block_table.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6353 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/block/common.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8191 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/block/cpu_gpu_block_allocator.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2525 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/block/interfaces.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9871 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/block/naive_block.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    21223 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/block/prefix_caching_block.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    24684 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/block_manager_v1.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10428 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/block_manager_v2.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3548 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/evictor_v1.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4344 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/evictor_v2.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2871 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/interfaces.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      958 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/policy.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    49123 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/core/scheduler.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.579488 vllm_acc-0.4.1/vllm/distributed/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       83 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/distributed/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9707 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/distributed/communication_op.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.579488 vllm_acc-0.4.1/vllm/distributed/device_communicators/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/distributed/device_communicators/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9768 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/distributed/device_communicators/custom_all_reduce.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10345 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/distributed/device_communicators/pynccl.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1761 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/distributed/device_communicators/pynccl_utils.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12937 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/distributed/parallel_state.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5321 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/distributed/utils.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.579488 vllm_acc-0.4.1/vllm/engine/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/engine/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    28601 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/engine/arg_utils.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    28908 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/engine/async_llm_engine.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    33183 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/engine/llm_engine.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    15068 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/engine/metrics.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.579488 vllm_acc-0.4.1/vllm/engine/output_processor/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/engine/output_processor/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2908 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/engine/output_processor/interfaces.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5807 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/engine/output_processor/multi_step.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13876 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/engine/output_processor/single_step.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4011 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/engine/output_processor/stop_checker.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      666 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/engine/output_processor/util.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.579488 vllm_acc-0.4.1/vllm/entrypoints/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/entrypoints/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4228 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/entrypoints/api_server.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11725 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/entrypoints/llm.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.579488 vllm_acc-0.4.1/vllm/entrypoints/openai/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/entrypoints/openai/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6442 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/entrypoints/openai/api_server.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4882 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/entrypoints/openai/cli_args.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    17060 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/entrypoints/openai/protocol.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16924 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/entrypoints/openai/serving_chat.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    15451 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/entrypoints/openai/serving_completion.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9150 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/entrypoints/openai/serving_engine.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.583488 vllm_acc-0.4.1/vllm/executor/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/executor/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6575 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/executor/cpu_executor.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4211 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/executor/distributed_gpu_executor.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4336 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/executor/executor_base.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6457 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/executor/gpu_executor.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8615 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/executor/multiproc_worker_utils.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3515 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/executor/neuron_executor.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13601 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/executor/ray_gpu_executor.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4476 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/executor/ray_utils.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4975 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/logger.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.583488 vllm_acc-0.4.1/vllm/lora/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/lora/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10193 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/lora/fully_sharded_layers.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    43117 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/lora/layers.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5124 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/lora/lora.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    27413 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/lora/models.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6652 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/lora/punica.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      910 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/lora/request.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3991 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/lora/utils.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9372 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/lora/worker_manager.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.583488 vllm_acc-0.4.1/vllm/model_executor/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      183 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/__init__.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.583488 vllm_acc-0.4.1/vllm/model_executor/guided_decoding/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1191 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/guided_decoding/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2979 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/guided_decoding/lm_format_enforcer_decoding.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4636 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/guided_decoding/outlines_decoding.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6297 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/guided_decoding/outlines_logits_processors.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.583488 vllm_acc-0.4.1/vllm/model_executor/layers/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6045 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/activation.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.583488 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      158 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/__init__.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.587488 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3254 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=16,N=1344,device_name=NVIDIA_A100-SXM4-40GB.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3250 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=16,N=1344,device_name=NVIDIA_A100-SXM4-80GB.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3246 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=16,N=1344,device_name=NVIDIA_H100_80GB_HBM3.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3254 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=16,N=2688,device_name=NVIDIA_A100-SXM4-80GB.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3257 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=16,N=2688,device_name=NVIDIA_H100_80GB_HBM3.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3250 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=1792,device_name=NVIDIA_A100-SXM4-40GB.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3252 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=1792,device_name=NVIDIA_A100-SXM4-80GB.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3255 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=1792,device_name=NVIDIA_H100_80GB_HBM3.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3256 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=2048,device_name=NVIDIA_A100-SXM4-80GB.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3254 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=2048,device_name=NVIDIA_H100_80GB_HBM3.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3254 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_A100-SXM4-40GB.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3254 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_A100-SXM4-80GB.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3114 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_H100_80GB_HBM3,dtype=float8.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3252 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_H100_80GB_HBM3.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3255 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=4096,device_name=NVIDIA_A100-SXM4-80GB.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3259 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=4096,device_name=NVIDIA_H100_80GB_HBM3.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3252 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=7168,device_name=NVIDIA_A100-SXM4-80GB.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3268 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=7168,device_name=NVIDIA_H100_80GB_HBM3,dtype=float8.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3261 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=7168,device_name=NVIDIA_H100_80GB_HBM3.json
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    19188 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/fused_moe.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1986 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/layernorm.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    30448 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/linear.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4111 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/logits_processor.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.587488 vllm_acc-0.4.1/vllm/model_executor/layers/ops/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/ops/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5091 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/ops/rand.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16675 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/ops/sample.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.587488 vllm_acc-0.4.1/vllm/model_executor/layers/quantization/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1234 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/quantization/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13684 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/quantization/aqlm.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6132 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/quantization/awq.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3113 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/quantization/base_config.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10065 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/quantization/fp8.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7881 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/quantization/gptq.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    15883 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/quantization/gptq_marlin.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7641 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/quantization/marlin.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3648 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/quantization/schema.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4558 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/quantization/squeezellm.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16541 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/rejection_sampler.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20752 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/rotary_embedding.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    45005 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/sampler.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6289 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/layers/vocab_parallel_embedding.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.587488 vllm_acc-0.4.1/vllm/model_executor/model_loader/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1309 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/model_loader/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16182 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/model_loader/loader.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5003 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/model_loader/neuron.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    15691 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/model_loader/tensorizer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1405 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/model_loader/utils.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13657 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/model_loader/weight_utils.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.591488 vllm_acc-0.4.1/vllm/model_executor/models/
--rwxrwxr-x   0 azureuser  (1000) azureuser  (1000)     4885 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    15574 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/baichuan.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11863 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/bloom.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13290 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/chatglm.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14462 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/commandr.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14762 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/dbrx.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5288 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/decilm.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    17369 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/deepseek.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    17689 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/falcon.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14689 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/gemma.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9802 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/gpt2.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9767 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/gpt_bigcode.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10126 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/gpt_j.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11098 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/gpt_neox.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12361 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/internlm2.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12256 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/jais.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    17518 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/llama.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10849 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/llava.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20813 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/minicpm.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20781 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/mixtral.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    15988 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/mixtral_quant.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10622 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/mpt.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13007 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/olmo.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13212 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/opt.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11981 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/orion.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11405 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/phi.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10218 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/qwen.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13773 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/qwen2.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    17796 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/qwen2_moe.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12390 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/stablelm.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11915 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/starcoder2.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13652 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/models/xverse.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    23648 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/sampling_metadata.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      928 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/model_executor/utils.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6038 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/outputs.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       65 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/py.typed
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16393 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/sampling_params.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    26791 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/sequence.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.595488 vllm_acc-0.4.1/vllm/spec_decode/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/spec_decode/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16116 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/spec_decode/batch_expansion.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2277 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/spec_decode/interfaces.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7243 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/spec_decode/metrics.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8972 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/spec_decode/multi_step_worker.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7076 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/spec_decode/ngram_worker.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    19775 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/spec_decode/spec_decode_worker.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7766 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/spec_decode/top1_proposer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4598 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/spec_decode/util.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1248 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/test_utils.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.595488 vllm_acc-0.4.1/vllm/transformers_utils/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2328 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/config.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.595488 vllm_acc-0.4.1/vllm/transformers_utils/configs/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      619 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/configs/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2747 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/configs/chatglm.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10918 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/configs/dbrx.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2878 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/configs/falcon.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10335 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/configs/jais.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7562 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/configs/mpt.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13148 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/detokenizer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5490 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/tokenizer.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.595488 vllm_acc-0.4.1/vllm/transformers_utils/tokenizer_group/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1267 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/tokenizer_group/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1607 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/tokenizer_group/base_tokenizer_group.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6515 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/tokenizer_group/ray_tokenizer_group.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3226 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/tokenizer_group/tokenizer_group.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.595488 vllm_acc-0.4.1/vllm/transformers_utils/tokenizers/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      114 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/tokenizers/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9390 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/transformers_utils/tokenizers/baichuan.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.595488 vllm_acc-0.4.1/vllm/usage/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/usage/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7293 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/usage/usage_lib.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20426 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/utils.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.595488 vllm_acc-0.4.1/vllm/worker/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/worker/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4111 2024-05-02 00:54:26.000000 vllm_acc-0.4.1/vllm/worker/cache_engine.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14012 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/worker/cpu_model_runner.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12699 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/worker/cpu_worker.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    46659 2024-05-02 20:38:13.000000 vllm_acc-0.4.1/vllm/worker/model_runner.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7952 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/worker/neuron_model_runner.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3480 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/worker/neuron_worker.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14659 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/worker/worker.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5472 2024-05-01 23:50:28.000000 vllm_acc-0.4.1/vllm/worker/worker_base.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:12:42.595488 vllm_acc-0.4.1/vllm_acc.egg-info/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8244 2024-05-04 00:12:42.000000 vllm_acc-0.4.1/vllm_acc.egg-info/PKG-INFO
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13287 2024-05-04 00:12:42.000000 vllm_acc-0.4.1/vllm_acc.egg-info/SOURCES.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2024-05-04 00:12:42.000000 vllm_acc-0.4.1/vllm_acc.egg-info/dependency_links.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      430 2024-05-04 00:12:42.000000 vllm_acc-0.4.1/vllm_acc.egg-info/requires.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       11 2024-05-04 00:12:42.000000 vllm_acc-0.4.1/vllm_acc.egg-info/top_level.txt
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.069345 vllm_acc-0.4.11714782966.854302/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9065 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/CMakeLists.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11357 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/LICENSE
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      153 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/MANIFEST.in
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8261 2024-05-04 00:36:07.069345 vllm_acc-0.4.11714782966.854302/PKG-INFO
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7444 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/README.md
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.033345 vllm_acc-0.4.11714782966.854302/cmake/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2241 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/cmake/cpu_extension.cmake
+-rwxrwxr-x   0 azureuser  (1000) azureuser  (1000)     2308 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/cmake/hipify.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12858 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/cmake/utils.cmake
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.033345 vllm_acc-0.4.11714782966.854302/csrc/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6588 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/activation_kernels.cu
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.033345 vllm_acc-0.4.11714782966.854302/csrc/attention/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      160 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/attention/attention_dtypes.h
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1721 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/attention/attention_generic.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    44264 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/attention/attention_kernels.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1867 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/attention/attention_utils.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11580 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/attention/dtype_bfloat16.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12012 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/attention/dtype_float16.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5641 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/attention/dtype_float32.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      555 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/attention/dtype_fp8.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      681 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/cache.h
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13638 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/cache_kernels.cu
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.033345 vllm_acc-0.4.11714782966.854302/csrc/cpu/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5120 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/cpu/activation.cpp
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    32175 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/cpu/attention.cpp
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5794 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/cpu/cache.cpp
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10374 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/cpu/cpu_types.hpp
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4088 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/cpu/layernorm.cpp
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7447 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/cpu/pos_encoding.cpp
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1858 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/cpu/pybind.cpp
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      958 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/cuda_compat.h
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      184 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/cuda_utils.h
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      837 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/cuda_utils_kernels.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5757 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/custom_all_reduce.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    17097 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/custom_all_reduce.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12170 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/custom_all_reduce_test.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1679 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/dispatch_utils.h
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13097 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/layernorm_kernels.cu
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.033345 vllm_acc-0.4.11714782966.854302/csrc/moe/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      182 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/moe/moe_ops.cpp
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      197 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/moe/moe_ops.h
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20741 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/moe/topk_softmax_kernels.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4942 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/moe_align_block_size_kernels.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5005 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/ops.h
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8750 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/pos_encoding_kernels.cu
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.033345 vllm_acc-0.4.11714782966.854302/csrc/punica/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11807 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/punica/LICENSE
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.037345 vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      214 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/bgmv_bf16_bf16_bf16.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      202 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/bgmv_bf16_fp32_bf16.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6415 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/bgmv_config.h
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      190 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/bgmv_fp16_fp16_fp16.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      186 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/bgmv_fp16_fp32_fp16.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      202 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/bgmv_fp32_bf16_bf16.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      186 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/bgmv_fp32_fp16_fp16.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11313 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/bgmv_impl.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2055 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/generator.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    41110 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/vec_dtypes.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    25047 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/punica/punica_ops.cc
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4610 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/pybind.cpp
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.025344 vllm_acc-0.4.11714782966.854302/csrc/quantization/
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.037345 vllm_acc-0.4.11714782966.854302/csrc/quantization/aqlm/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20265 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/aqlm/gemm_kernels.cu
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.037345 vllm_acc-0.4.11714782966.854302/csrc/quantization/awq/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4155 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/awq/dequantize.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    21103 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/awq/gemm_kernels.cu
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.037345 vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8/
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.037345 vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8/amd_detail/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3973 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8/amd_detail/hip_float8.h
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11019 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8/amd_detail/hip_float8_impl.h
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13443 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8/amd_detail/quant_utils.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3934 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8/fp8_cuda_kernels.cu
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.037345 vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8_e5m2_kvcache/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6770 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8_e5m2_kvcache/quant_utils.cuh
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.037345 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1703 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/compat.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9354 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/matrix_view.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    64637 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/q_gemm.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2598 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/qdq_2.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5053 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/qdq_3.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4169 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/qdq_4.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      723 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/qdq_8.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1407 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/qdq_util.cuh
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.037345 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq_marlin/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    58283 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq_marlin/gptq_marlin.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2306 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq_marlin/gptq_marlin.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10771 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq_marlin/gptq_marlin_repack.cu
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.037345 vllm_acc-0.4.11714782966.854302/csrc/quantization/marlin/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11690 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/marlin/LICENSE
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    45316 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/marlin/marlin_cuda_kernel.cu
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.037345 vllm_acc-0.4.11714782966.854302/csrc/quantization/squeezellm/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5494 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/quantization/squeezellm/quant_cuda_kernel.cu
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2385 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/csrc/reduction_utils.cuh
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1281 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/pyproject.toml
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      603 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/requirements-common.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      251 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/requirements-cuda.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2024-05-04 00:36:07.069345 vllm_acc-0.4.11714782966.854302/setup.cfg
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14184 2024-05-04 00:35:49.000000 vllm_acc-0.4.11714782966.854302/setup.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.037345 vllm_acc-0.4.11714782966.854302/tests/
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.041345 vllm_acc-0.4.11714782966.854302/tests/core/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/__init__.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.041345 vllm_acc-0.4.11714782966.854302/tests/core/block/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/block/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      360 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/block/conftest.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3753 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/block/test_block_manager_v2.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    22046 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/block/test_block_table.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1246 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/block/test_common.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3864 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/block/test_cpu_gpu_block_allocator.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4001 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/block/test_naive_block.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20684 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/block/test_prefix_caching_block.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13753 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/test_block_manager.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    22188 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/test_chunked_prefill_scheduler.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    34201 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/test_scheduler.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2139 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/core/utils.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.041345 vllm_acc-0.4.11714782966.854302/tests/lora/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5399 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/conftest.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4673 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_baichuan.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3098 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_chatglm3.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1549 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_gemma.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6393 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_layer_variation.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    29994 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_layers.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10194 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_llama.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8094 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_lora.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2357 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_lora_checkpoints.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    19701 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_lora_manager.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4656 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_mixtral.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6502 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_punica.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5793 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_quant_model.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2197 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_tokenizer_group.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4325 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_utils.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2458 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/test_worker.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2846 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/lora/utils.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.045344 vllm_acc-0.4.11714782966.854302/tests/spec_decode/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/__init__.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.045344 vllm_acc-0.4.11714782966.854302/tests/spec_decode/e2e/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/e2e/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8688 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/e2e/conftest.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5190 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/e2e/test_compatibility.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    18322 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/e2e/test_multistep_correctness.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6005 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/e2e/test_ngram_correctness.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3146 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/test_batch_expansion.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6098 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/test_metrics.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13869 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/test_multi_step_worker.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6594 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/test_ngram_worker.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    24897 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/test_spec_decode_worker.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3080 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/test_utils.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8680 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/spec_decode/utils.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.045344 vllm_acc-0.4.11714782966.854302/tests/tensorizer_loader/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/tensorizer_loader/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8755 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/tensorizer_loader/tensorize_vllm_model_for_testing.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12383 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/tensorizer_loader/test_tensorizer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3501 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/test_cache_block_hashing.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1324 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/test_config.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      465 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/test_logger.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3820 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/test_logits_processor.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1732 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/test_regression.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      289 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/test_sampling_params.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4210 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/test_sequence.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.045344 vllm_acc-0.4.11714782966.854302/tests/tokenization/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/tokenization/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      896 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/tokenization/test_cached_tokenizer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8016 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/tokenization/test_detokenize.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      644 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/tokenization/test_tokenizer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3813 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/tokenization/test_tokenizer_group.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.045344 vllm_acc-0.4.11714782966.854302/tests/worker/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/worker/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14526 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/worker/test_model_runner.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3118 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/tests/worker/test_swap.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.045344 vllm_acc-0.4.11714782966.854302/vllm/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      742 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9150 2024-05-02 22:06:13.000000 vllm_acc-0.4.11714782966.854302/vllm/_custom_ops.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.045344 vllm_acc-0.4.11714782966.854302/vllm/attention/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      436 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/__init__.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.049345 vllm_acc-0.4.11714782966.854302/vllm/attention/backends/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/backends/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3578 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/backends/abstract.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11167 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/backends/flash_attn.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14823 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/backends/rocm_flash_attn.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9666 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/backends/torch_sdpa.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16245 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/backends/xformers.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1925 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/layer.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.049345 vllm_acc-0.4.11714782966.854302/vllm/attention/ops/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/ops/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7006 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/ops/paged_attn.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    26579 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/ops/prefix_prefill.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    27247 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/ops/triton_flash_attention.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2910 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/attention/selector.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2374 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/block.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    50305 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/config.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.049345 vllm_acc-0.4.11714782966.854302/vllm/core/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/__init__.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.049345 vllm_acc-0.4.11714782966.854302/vllm/core/block/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/block/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11618 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/block/block_table.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6353 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/block/common.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8191 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/block/cpu_gpu_block_allocator.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2525 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/block/interfaces.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9871 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/block/naive_block.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    21223 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/block/prefix_caching_block.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    24684 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/block_manager_v1.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10428 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/block_manager_v2.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3548 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/evictor_v1.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4344 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/evictor_v2.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2871 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/interfaces.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      958 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/policy.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    49123 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/core/scheduler.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.049345 vllm_acc-0.4.11714782966.854302/vllm/distributed/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       83 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/distributed/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9707 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/distributed/communication_op.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.049345 vllm_acc-0.4.11714782966.854302/vllm/distributed/device_communicators/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/distributed/device_communicators/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9768 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/distributed/device_communicators/custom_all_reduce.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10345 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/distributed/device_communicators/pynccl.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1761 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/distributed/device_communicators/pynccl_utils.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12937 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/distributed/parallel_state.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5321 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/distributed/utils.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.049345 vllm_acc-0.4.11714782966.854302/vllm/engine/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/engine/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    28601 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/engine/arg_utils.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    28908 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/engine/async_llm_engine.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    33183 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/engine/llm_engine.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    15068 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/engine/metrics.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.053345 vllm_acc-0.4.11714782966.854302/vllm/engine/output_processor/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/engine/output_processor/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2908 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/engine/output_processor/interfaces.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5807 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/engine/output_processor/multi_step.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13876 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/engine/output_processor/single_step.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4011 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/engine/output_processor/stop_checker.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      666 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/engine/output_processor/util.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.053345 vllm_acc-0.4.11714782966.854302/vllm/entrypoints/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/entrypoints/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4228 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/entrypoints/api_server.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11725 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/entrypoints/llm.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.053345 vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6442 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/api_server.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4882 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/cli_args.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    17060 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/protocol.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16924 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/serving_chat.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    15451 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/serving_completion.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9150 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/serving_engine.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.053345 vllm_acc-0.4.11714782966.854302/vllm/executor/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/executor/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6575 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/executor/cpu_executor.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4211 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/executor/distributed_gpu_executor.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4336 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/executor/executor_base.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6457 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/executor/gpu_executor.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8615 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/executor/multiproc_worker_utils.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3515 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/executor/neuron_executor.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13601 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/executor/ray_gpu_executor.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4476 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/executor/ray_utils.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4975 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/logger.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.053345 vllm_acc-0.4.11714782966.854302/vllm/lora/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/lora/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10193 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/lora/fully_sharded_layers.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    43117 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/lora/layers.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5124 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/lora/lora.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    27413 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/lora/models.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6652 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/lora/punica.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      910 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/lora/request.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3991 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/lora/utils.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9372 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/lora/worker_manager.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.053345 vllm_acc-0.4.11714782966.854302/vllm/model_executor/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      183 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/__init__.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.053345 vllm_acc-0.4.11714782966.854302/vllm/model_executor/guided_decoding/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1191 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/guided_decoding/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2979 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/guided_decoding/lm_format_enforcer_decoding.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4636 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/guided_decoding/outlines_decoding.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6297 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/guided_decoding/outlines_logits_processors.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.057345 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6045 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/activation.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.057345 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      158 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/__init__.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.057345 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3254 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=16,N=1344,device_name=NVIDIA_A100-SXM4-40GB.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3250 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=16,N=1344,device_name=NVIDIA_A100-SXM4-80GB.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3246 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=16,N=1344,device_name=NVIDIA_H100_80GB_HBM3.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3254 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=16,N=2688,device_name=NVIDIA_A100-SXM4-80GB.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3257 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=16,N=2688,device_name=NVIDIA_H100_80GB_HBM3.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3250 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=1792,device_name=NVIDIA_A100-SXM4-40GB.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3252 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=1792,device_name=NVIDIA_A100-SXM4-80GB.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3255 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=1792,device_name=NVIDIA_H100_80GB_HBM3.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3256 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=2048,device_name=NVIDIA_A100-SXM4-80GB.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3254 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=2048,device_name=NVIDIA_H100_80GB_HBM3.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3254 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_A100-SXM4-40GB.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3254 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_A100-SXM4-80GB.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3114 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_H100_80GB_HBM3,dtype=float8.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3252 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_H100_80GB_HBM3.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3255 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=4096,device_name=NVIDIA_A100-SXM4-80GB.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3259 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=4096,device_name=NVIDIA_H100_80GB_HBM3.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3252 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=7168,device_name=NVIDIA_A100-SXM4-80GB.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3268 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=7168,device_name=NVIDIA_H100_80GB_HBM3,dtype=float8.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3261 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=7168,device_name=NVIDIA_H100_80GB_HBM3.json
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    19188 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/fused_moe.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1986 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/layernorm.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    30448 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/linear.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4111 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/logits_processor.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.057345 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/ops/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/ops/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5091 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/ops/rand.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16675 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/ops/sample.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.061344 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1234 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13684 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/aqlm.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6132 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/awq.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3113 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/base_config.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10065 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/fp8.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7881 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/gptq.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    15883 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/gptq_marlin.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7641 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/marlin.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3648 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/schema.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4558 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/squeezellm.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16541 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/rejection_sampler.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20752 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/rotary_embedding.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    45005 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/sampler.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6289 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/vocab_parallel_embedding.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.061344 vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1309 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16182 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/loader.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5003 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/neuron.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    15691 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/tensorizer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1405 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/utils.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13657 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/weight_utils.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.065344 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/
+-rwxrwxr-x   0 azureuser  (1000) azureuser  (1000)     4885 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    15574 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/baichuan.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11863 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/bloom.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13290 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/chatglm.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14462 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/commandr.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14762 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/dbrx.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5288 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/decilm.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    17369 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/deepseek.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    17689 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/falcon.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14689 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/gemma.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9802 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/gpt2.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9767 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/gpt_bigcode.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10126 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/gpt_j.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11098 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/gpt_neox.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12361 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/internlm2.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12256 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/jais.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    17518 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/llama.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10849 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/llava.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20813 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/minicpm.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20781 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/mixtral.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    15988 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/mixtral_quant.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10622 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/mpt.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13007 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/olmo.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13212 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/opt.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11981 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/orion.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11405 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/phi.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10218 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/qwen.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13773 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/qwen2.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    17796 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/qwen2_moe.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12390 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/stablelm.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    11915 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/starcoder2.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13652 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/xverse.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    23648 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/sampling_metadata.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      928 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/model_executor/utils.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6038 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/outputs.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       65 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/py.typed
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16393 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/sampling_params.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    26791 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/sequence.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.065344 vllm_acc-0.4.11714782966.854302/vllm/spec_decode/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/spec_decode/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    16116 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/spec_decode/batch_expansion.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2277 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/spec_decode/interfaces.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7243 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/spec_decode/metrics.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8972 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/spec_decode/multi_step_worker.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7076 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/spec_decode/ngram_worker.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    19775 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/spec_decode/spec_decode_worker.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7766 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/spec_decode/top1_proposer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4598 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/spec_decode/util.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1248 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/test_utils.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.065344 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2328 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/config.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.065344 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      619 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2747 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/chatglm.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10918 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/dbrx.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2878 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/falcon.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10335 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/jais.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7562 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/mpt.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13148 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/detokenizer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5490 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizer.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.065344 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizer_group/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1267 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizer_group/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1607 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizer_group/base_tokenizer_group.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6515 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizer_group/ray_tokenizer_group.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3226 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizer_group/tokenizer_group.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.065344 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizers/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      114 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizers/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     9390 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizers/baichuan.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.069345 vllm_acc-0.4.11714782966.854302/vllm/usage/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/usage/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7293 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/usage/usage_lib.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    20426 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/utils.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.069345 vllm_acc-0.4.11714782966.854302/vllm/worker/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/worker/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4111 2024-05-02 00:54:26.000000 vllm_acc-0.4.11714782966.854302/vllm/worker/cache_engine.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14012 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/worker/cpu_model_runner.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    12699 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/worker/cpu_worker.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    46659 2024-05-02 20:38:13.000000 vllm_acc-0.4.11714782966.854302/vllm/worker/model_runner.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7952 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/worker/neuron_model_runner.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3480 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/worker/neuron_worker.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    14659 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/worker/worker.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5472 2024-05-01 23:50:28.000000 vllm_acc-0.4.11714782966.854302/vllm/worker/worker_base.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-05-04 00:36:07.069345 vllm_acc-0.4.11714782966.854302/vllm_acc.egg-info/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     8261 2024-05-04 00:36:06.000000 vllm_acc-0.4.11714782966.854302/vllm_acc.egg-info/PKG-INFO
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    13287 2024-05-04 00:36:06.000000 vllm_acc-0.4.11714782966.854302/vllm_acc.egg-info/SOURCES.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2024-05-04 00:36:06.000000 vllm_acc-0.4.11714782966.854302/vllm_acc.egg-info/dependency_links.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      430 2024-05-04 00:36:06.000000 vllm_acc-0.4.11714782966.854302/vllm_acc.egg-info/requires.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       11 2024-05-04 00:36:06.000000 vllm_acc-0.4.11714782966.854302/vllm_acc.egg-info/top_level.txt
```

### Comparing `vllm_acc-0.4.1/CMakeLists.txt` & `vllm_acc-0.4.11714782966.854302/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/LICENSE` & `vllm_acc-0.4.11714782966.854302/LICENSE`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/PKG-INFO` & `vllm_acc-0.4.11714782966.854302/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vllm_acc
-Version: 0.4.1
+Version: 0.4.11714782966.854302
 Summary: A high-throughput and memory-efficient inference and serving engine for LLMs
 Home-page: https://github.com/vllm-project/vllm
 Author: vLLM Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/vllm-project/vllm
 Project-URL: Documentation, https://vllm.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: vllm_acc Version: 0.4.1 Summary: A high-throughput
-and memory-efficient inference and serving engine for LLMs Home-page: https://
-github.com/vllm-project/vllm Author: vLLM Team License: Apache 2.0 Project-URL:
-Homepage, https://github.com/vllm-project/vllm Project-URL: Documentation,
-https://vllm.readthedocs.io/en/latest/ Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-tensorizer License-File: LICENSE
+Metadata-Version: 2.1 Name: vllm_acc Version: 0.4.11714782966.854302 Summary: A
+high-throughput and memory-efficient inference and serving engine for LLMs
+Home-page: https://github.com/vllm-project/vllm Author: vLLM Team License:
+Apache 2.0 Project-URL: Homepage, https://github.com/vllm-project/vllm Project-
+URL: Documentation, https://vllm.readthedocs.io/en/latest/ Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Provides-Extra: tensorizer License-File: LICENSE
                                     [vLLM]
            ******** EEaassyy,, ffaasstt,, aanndd cchheeaapp LLLLMM sseerrvviinngg ffoorr eevveerryyoonnee ********
                   | _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn | _BB_ll_oo_gg | _PP_aa_pp_ee_rr | _DD_ii_ss_cc_oo_rr_dd |
 *Latest News* ð¥ - [2024/04] We hosted [the third vLLM meetup](https://
 robloxandvllmmeetup2024.splashthat.com/) with Roblox! Please find the meetup
 slides [here](https://docs.google.com/presentation/d/1A--
 47JAK4BJ39t954HyTkvtfwn0fkqtsL8NGFuslReM/edit?usp=sharing). - [2024/01] We
```

### Comparing `vllm_acc-0.4.1/README.md` & `vllm_acc-0.4.11714782966.854302/README.md`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/cmake/cpu_extension.cmake` & `vllm_acc-0.4.11714782966.854302/cmake/cpu_extension.cmake`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/cmake/hipify.py` & `vllm_acc-0.4.11714782966.854302/cmake/hipify.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/cmake/utils.cmake` & `vllm_acc-0.4.11714782966.854302/cmake/utils.cmake`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/activation_kernels.cu` & `vllm_acc-0.4.11714782966.854302/csrc/activation_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/attention/attention_generic.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/attention/attention_generic.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/attention/attention_kernels.cu` & `vllm_acc-0.4.11714782966.854302/csrc/attention/attention_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/attention/attention_utils.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/attention/attention_utils.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/attention/dtype_bfloat16.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/attention/dtype_bfloat16.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/attention/dtype_float16.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/attention/dtype_float16.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/attention/dtype_float32.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/attention/dtype_float32.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/attention/dtype_fp8.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/attention/dtype_fp8.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/cache.h` & `vllm_acc-0.4.11714782966.854302/csrc/cache.h`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/cache_kernels.cu` & `vllm_acc-0.4.11714782966.854302/csrc/cache_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/cpu/activation.cpp` & `vllm_acc-0.4.11714782966.854302/csrc/cpu/activation.cpp`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/cpu/attention.cpp` & `vllm_acc-0.4.11714782966.854302/csrc/cpu/attention.cpp`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/cpu/cache.cpp` & `vllm_acc-0.4.11714782966.854302/csrc/cpu/cache.cpp`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/cpu/cpu_types.hpp` & `vllm_acc-0.4.11714782966.854302/csrc/cpu/cpu_types.hpp`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/cpu/layernorm.cpp` & `vllm_acc-0.4.11714782966.854302/csrc/cpu/layernorm.cpp`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/cpu/pos_encoding.cpp` & `vllm_acc-0.4.11714782966.854302/csrc/cpu/pos_encoding.cpp`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/cpu/pybind.cpp` & `vllm_acc-0.4.11714782966.854302/csrc/cpu/pybind.cpp`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/cuda_compat.h` & `vllm_acc-0.4.11714782966.854302/csrc/cuda_compat.h`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/cuda_utils_kernels.cu` & `vllm_acc-0.4.11714782966.854302/csrc/cuda_utils_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/custom_all_reduce.cu` & `vllm_acc-0.4.11714782966.854302/csrc/custom_all_reduce.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/custom_all_reduce.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/custom_all_reduce.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/custom_all_reduce_test.cu` & `vllm_acc-0.4.11714782966.854302/csrc/custom_all_reduce_test.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/dispatch_utils.h` & `vllm_acc-0.4.11714782966.854302/csrc/dispatch_utils.h`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/layernorm_kernels.cu` & `vllm_acc-0.4.11714782966.854302/csrc/layernorm_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/moe/topk_softmax_kernels.cu` & `vllm_acc-0.4.11714782966.854302/csrc/moe/topk_softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/moe_align_block_size_kernels.cu` & `vllm_acc-0.4.11714782966.854302/csrc/moe_align_block_size_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/ops.h` & `vllm_acc-0.4.11714782966.854302/csrc/ops.h`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/pos_encoding_kernels.cu` & `vllm_acc-0.4.11714782966.854302/csrc/pos_encoding_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/punica/LICENSE` & `vllm_acc-0.4.11714782966.854302/csrc/punica/LICENSE`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/punica/bgmv/bgmv_config.h` & `vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/bgmv_config.h`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/punica/bgmv/bgmv_impl.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/bgmv_impl.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/punica/bgmv/generator.py` & `vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/generator.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/punica/bgmv/vec_dtypes.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/punica/bgmv/vec_dtypes.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/punica/punica_ops.cc` & `vllm_acc-0.4.11714782966.854302/csrc/punica/punica_ops.cc`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/pybind.cpp` & `vllm_acc-0.4.11714782966.854302/csrc/pybind.cpp`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/aqlm/gemm_kernels.cu` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/aqlm/gemm_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/awq/dequantize.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/awq/dequantize.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/awq/gemm_kernels.cu` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/awq/gemm_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/fp8/amd_detail/hip_float8.h` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8/amd_detail/hip_float8.h`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/fp8/amd_detail/hip_float8_impl.h` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8/amd_detail/hip_float8_impl.h`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/fp8/amd_detail/quant_utils.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8/amd_detail/quant_utils.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/fp8/fp8_cuda_kernels.cu` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8/fp8_cuda_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/fp8_e5m2_kvcache/quant_utils.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/fp8_e5m2_kvcache/quant_utils.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/gptq/compat.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/compat.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/gptq/matrix_view.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/matrix_view.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/gptq/q_gemm.cu` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/q_gemm.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/gptq/qdq_2.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/qdq_2.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/gptq/qdq_3.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/qdq_3.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/gptq/qdq_4.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/qdq_4.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/gptq/qdq_8.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/qdq_8.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/gptq/qdq_util.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq/qdq_util.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/gptq_marlin/gptq_marlin.cu` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq_marlin/gptq_marlin.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/gptq_marlin/gptq_marlin.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq_marlin/gptq_marlin.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/gptq_marlin/gptq_marlin_repack.cu` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/gptq_marlin/gptq_marlin_repack.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/marlin/LICENSE` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/marlin/LICENSE`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/marlin/marlin_cuda_kernel.cu` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/marlin/marlin_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/quantization/squeezellm/quant_cuda_kernel.cu` & `vllm_acc-0.4.11714782966.854302/csrc/quantization/squeezellm/quant_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/csrc/reduction_utils.cuh` & `vllm_acc-0.4.11714782966.854302/csrc/reduction_utils.cuh`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/pyproject.toml` & `vllm_acc-0.4.11714782966.854302/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/requirements-common.txt` & `vllm_acc-0.4.11714782966.854302/requirements-common.txt`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/setup.py` & `vllm_acc-0.4.11714782966.854302/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,16 @@
 
     Adapted from https://github.com/ray-project/ray/blob/0b190ee1160eeca9796bc091e07eaebf4c85b511/python/setup.py
     """
     with open(filepath) as fp:
         version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]",
                                   fp.read(), re.M)
         if version_match:
-            return version_match.group(1)
+            import time
+            return version_match.group(1) + str(time.time())
         raise RuntimeError("Unable to find version string.")
 
 
 def get_vllm_version() -> str:
     version = find_version(get_path("vllm", "__init__.py"))
     """
     if _is_cuda():
```

### Comparing `vllm_acc-0.4.1/tests/core/block/test_block_manager_v2.py` & `vllm_acc-0.4.11714782966.854302/tests/core/block/test_block_manager_v2.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/core/block/test_block_table.py` & `vllm_acc-0.4.11714782966.854302/tests/core/block/test_block_table.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/core/block/test_common.py` & `vllm_acc-0.4.11714782966.854302/tests/core/block/test_common.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/core/block/test_cpu_gpu_block_allocator.py` & `vllm_acc-0.4.11714782966.854302/tests/core/block/test_cpu_gpu_block_allocator.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/core/block/test_naive_block.py` & `vllm_acc-0.4.11714782966.854302/tests/core/block/test_naive_block.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/core/block/test_prefix_caching_block.py` & `vllm_acc-0.4.11714782966.854302/tests/core/block/test_prefix_caching_block.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/core/test_block_manager.py` & `vllm_acc-0.4.11714782966.854302/tests/core/test_block_manager.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/core/test_chunked_prefill_scheduler.py` & `vllm_acc-0.4.11714782966.854302/tests/core/test_chunked_prefill_scheduler.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/core/test_scheduler.py` & `vllm_acc-0.4.11714782966.854302/tests/core/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/core/utils.py` & `vllm_acc-0.4.11714782966.854302/tests/core/utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/conftest.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/conftest.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_baichuan.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_baichuan.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_chatglm3.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_chatglm3.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_gemma.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_gemma.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_layer_variation.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_layer_variation.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_layers.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_layers.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_llama.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_llama.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_lora.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_lora.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_lora_checkpoints.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_lora_checkpoints.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_lora_manager.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_lora_manager.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_mixtral.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_mixtral.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_punica.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_punica.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_quant_model.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_quant_model.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_tokenizer_group.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_tokenizer_group.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_utils.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/test_worker.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/test_worker.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/lora/utils.py` & `vllm_acc-0.4.11714782966.854302/tests/lora/utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/spec_decode/e2e/conftest.py` & `vllm_acc-0.4.11714782966.854302/tests/spec_decode/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/spec_decode/e2e/test_compatibility.py` & `vllm_acc-0.4.11714782966.854302/tests/spec_decode/e2e/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/spec_decode/e2e/test_multistep_correctness.py` & `vllm_acc-0.4.11714782966.854302/tests/spec_decode/e2e/test_multistep_correctness.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/spec_decode/e2e/test_ngram_correctness.py` & `vllm_acc-0.4.11714782966.854302/tests/spec_decode/e2e/test_ngram_correctness.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/spec_decode/test_batch_expansion.py` & `vllm_acc-0.4.11714782966.854302/tests/spec_decode/test_batch_expansion.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/spec_decode/test_metrics.py` & `vllm_acc-0.4.11714782966.854302/tests/spec_decode/test_metrics.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/spec_decode/test_multi_step_worker.py` & `vllm_acc-0.4.11714782966.854302/tests/spec_decode/test_multi_step_worker.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/spec_decode/test_ngram_worker.py` & `vllm_acc-0.4.11714782966.854302/tests/spec_decode/test_ngram_worker.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/spec_decode/test_spec_decode_worker.py` & `vllm_acc-0.4.11714782966.854302/tests/spec_decode/test_spec_decode_worker.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/spec_decode/test_utils.py` & `vllm_acc-0.4.11714782966.854302/tests/spec_decode/test_utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/spec_decode/utils.py` & `vllm_acc-0.4.11714782966.854302/tests/spec_decode/utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/tensorizer_loader/tensorize_vllm_model_for_testing.py` & `vllm_acc-0.4.11714782966.854302/tests/tensorizer_loader/tensorize_vllm_model_for_testing.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/tensorizer_loader/test_tensorizer.py` & `vllm_acc-0.4.11714782966.854302/tests/tensorizer_loader/test_tensorizer.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/test_cache_block_hashing.py` & `vllm_acc-0.4.11714782966.854302/tests/test_cache_block_hashing.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/test_config.py` & `vllm_acc-0.4.11714782966.854302/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/test_logits_processor.py` & `vllm_acc-0.4.11714782966.854302/tests/test_logits_processor.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/test_regression.py` & `vllm_acc-0.4.11714782966.854302/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/test_sequence.py` & `vllm_acc-0.4.11714782966.854302/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/tokenization/test_cached_tokenizer.py` & `vllm_acc-0.4.11714782966.854302/tests/tokenization/test_cached_tokenizer.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/tokenization/test_detokenize.py` & `vllm_acc-0.4.11714782966.854302/tests/tokenization/test_detokenize.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/tokenization/test_tokenizer.py` & `vllm_acc-0.4.11714782966.854302/tests/tokenization/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/tokenization/test_tokenizer_group.py` & `vllm_acc-0.4.11714782966.854302/tests/tokenization/test_tokenizer_group.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/worker/test_model_runner.py` & `vllm_acc-0.4.11714782966.854302/tests/worker/test_model_runner.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/tests/worker/test_swap.py` & `vllm_acc-0.4.11714782966.854302/tests/worker/test_swap.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/__init__.py` & `vllm_acc-0.4.11714782966.854302/vllm/__init__.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/_custom_ops.py` & `vllm_acc-0.4.11714782966.854302/vllm/_custom_ops.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/attention/backends/abstract.py` & `vllm_acc-0.4.11714782966.854302/vllm/attention/backends/abstract.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/attention/backends/flash_attn.py` & `vllm_acc-0.4.11714782966.854302/vllm/attention/backends/flash_attn.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/attention/backends/rocm_flash_attn.py` & `vllm_acc-0.4.11714782966.854302/vllm/attention/backends/rocm_flash_attn.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/attention/backends/torch_sdpa.py` & `vllm_acc-0.4.11714782966.854302/vllm/attention/backends/torch_sdpa.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/attention/backends/xformers.py` & `vllm_acc-0.4.11714782966.854302/vllm/attention/backends/xformers.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/attention/layer.py` & `vllm_acc-0.4.11714782966.854302/vllm/attention/layer.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/attention/ops/paged_attn.py` & `vllm_acc-0.4.11714782966.854302/vllm/attention/ops/paged_attn.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/attention/ops/prefix_prefill.py` & `vllm_acc-0.4.11714782966.854302/vllm/attention/ops/prefix_prefill.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/attention/ops/triton_flash_attention.py` & `vllm_acc-0.4.11714782966.854302/vllm/attention/ops/triton_flash_attention.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/attention/selector.py` & `vllm_acc-0.4.11714782966.854302/vllm/attention/selector.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/block.py` & `vllm_acc-0.4.11714782966.854302/vllm/block.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/config.py` & `vllm_acc-0.4.11714782966.854302/vllm/config.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/block/block_table.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/block/block_table.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/block/common.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/block/common.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/block/cpu_gpu_block_allocator.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/block/cpu_gpu_block_allocator.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/block/interfaces.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/block/interfaces.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/block/naive_block.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/block/naive_block.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/block/prefix_caching_block.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/block/prefix_caching_block.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/block_manager_v1.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/block_manager_v1.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/block_manager_v2.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/block_manager_v2.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/evictor_v1.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/evictor_v1.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/evictor_v2.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/evictor_v2.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/interfaces.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/policy.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/policy.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/core/scheduler.py` & `vllm_acc-0.4.11714782966.854302/vllm/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/distributed/communication_op.py` & `vllm_acc-0.4.11714782966.854302/vllm/distributed/communication_op.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/distributed/device_communicators/custom_all_reduce.py` & `vllm_acc-0.4.11714782966.854302/vllm/distributed/device_communicators/custom_all_reduce.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/distributed/device_communicators/pynccl.py` & `vllm_acc-0.4.11714782966.854302/vllm/distributed/device_communicators/pynccl.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/distributed/device_communicators/pynccl_utils.py` & `vllm_acc-0.4.11714782966.854302/vllm/distributed/device_communicators/pynccl_utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/distributed/parallel_state.py` & `vllm_acc-0.4.11714782966.854302/vllm/distributed/parallel_state.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/distributed/utils.py` & `vllm_acc-0.4.11714782966.854302/vllm/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/engine/arg_utils.py` & `vllm_acc-0.4.11714782966.854302/vllm/engine/arg_utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/engine/async_llm_engine.py` & `vllm_acc-0.4.11714782966.854302/vllm/engine/async_llm_engine.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/engine/llm_engine.py` & `vllm_acc-0.4.11714782966.854302/vllm/engine/llm_engine.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/engine/metrics.py` & `vllm_acc-0.4.11714782966.854302/vllm/engine/metrics.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/engine/output_processor/interfaces.py` & `vllm_acc-0.4.11714782966.854302/vllm/engine/output_processor/interfaces.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/engine/output_processor/multi_step.py` & `vllm_acc-0.4.11714782966.854302/vllm/engine/output_processor/multi_step.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/engine/output_processor/single_step.py` & `vllm_acc-0.4.11714782966.854302/vllm/engine/output_processor/single_step.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/engine/output_processor/stop_checker.py` & `vllm_acc-0.4.11714782966.854302/vllm/engine/output_processor/stop_checker.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/engine/output_processor/util.py` & `vllm_acc-0.4.11714782966.854302/vllm/engine/output_processor/util.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/entrypoints/api_server.py` & `vllm_acc-0.4.11714782966.854302/vllm/entrypoints/api_server.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/entrypoints/llm.py` & `vllm_acc-0.4.11714782966.854302/vllm/entrypoints/llm.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/entrypoints/openai/api_server.py` & `vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/api_server.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/entrypoints/openai/cli_args.py` & `vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/cli_args.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/entrypoints/openai/protocol.py` & `vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/protocol.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/entrypoints/openai/serving_chat.py` & `vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/serving_chat.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/entrypoints/openai/serving_completion.py` & `vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/serving_completion.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/entrypoints/openai/serving_engine.py` & `vllm_acc-0.4.11714782966.854302/vllm/entrypoints/openai/serving_engine.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/executor/cpu_executor.py` & `vllm_acc-0.4.11714782966.854302/vllm/executor/cpu_executor.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/executor/distributed_gpu_executor.py` & `vllm_acc-0.4.11714782966.854302/vllm/executor/distributed_gpu_executor.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/executor/executor_base.py` & `vllm_acc-0.4.11714782966.854302/vllm/executor/executor_base.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/executor/gpu_executor.py` & `vllm_acc-0.4.11714782966.854302/vllm/executor/gpu_executor.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/executor/multiproc_worker_utils.py` & `vllm_acc-0.4.11714782966.854302/vllm/executor/multiproc_worker_utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/executor/neuron_executor.py` & `vllm_acc-0.4.11714782966.854302/vllm/executor/neuron_executor.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/executor/ray_gpu_executor.py` & `vllm_acc-0.4.11714782966.854302/vllm/executor/ray_gpu_executor.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/executor/ray_utils.py` & `vllm_acc-0.4.11714782966.854302/vllm/executor/ray_utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/logger.py` & `vllm_acc-0.4.11714782966.854302/vllm/logger.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/lora/fully_sharded_layers.py` & `vllm_acc-0.4.11714782966.854302/vllm/lora/fully_sharded_layers.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/lora/layers.py` & `vllm_acc-0.4.11714782966.854302/vllm/lora/layers.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/lora/lora.py` & `vllm_acc-0.4.11714782966.854302/vllm/lora/lora.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/lora/models.py` & `vllm_acc-0.4.11714782966.854302/vllm/lora/models.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/lora/punica.py` & `vllm_acc-0.4.11714782966.854302/vllm/lora/punica.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/lora/request.py` & `vllm_acc-0.4.11714782966.854302/vllm/lora/request.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/lora/utils.py` & `vllm_acc-0.4.11714782966.854302/vllm/lora/utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/lora/worker_manager.py` & `vllm_acc-0.4.11714782966.854302/vllm/lora/worker_manager.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/guided_decoding/__init__.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/guided_decoding/__init__.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/guided_decoding/lm_format_enforcer_decoding.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/guided_decoding/lm_format_enforcer_decoding.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/guided_decoding/outlines_decoding.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/guided_decoding/outlines_decoding.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/guided_decoding/outlines_logits_processors.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/guided_decoding/outlines_logits_processors.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/activation.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/activation.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=16,N=1344,device_name=NVIDIA_A100-SXM4-40GB.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=16,N=1344,device_name=NVIDIA_A100-SXM4-40GB.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=16,N=1344,device_name=NVIDIA_A100-SXM4-80GB.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=16,N=1344,device_name=NVIDIA_A100-SXM4-80GB.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=16,N=1344,device_name=NVIDIA_H100_80GB_HBM3.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=16,N=1344,device_name=NVIDIA_H100_80GB_HBM3.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=16,N=2688,device_name=NVIDIA_A100-SXM4-80GB.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=16,N=2688,device_name=NVIDIA_A100-SXM4-80GB.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=16,N=2688,device_name=NVIDIA_H100_80GB_HBM3.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=16,N=2688,device_name=NVIDIA_H100_80GB_HBM3.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=1792,device_name=NVIDIA_A100-SXM4-40GB.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=1792,device_name=NVIDIA_A100-SXM4-40GB.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=1792,device_name=NVIDIA_A100-SXM4-80GB.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=1792,device_name=NVIDIA_A100-SXM4-80GB.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=1792,device_name=NVIDIA_H100_80GB_HBM3.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=1792,device_name=NVIDIA_H100_80GB_HBM3.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=2048,device_name=NVIDIA_A100-SXM4-80GB.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=2048,device_name=NVIDIA_A100-SXM4-80GB.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=2048,device_name=NVIDIA_H100_80GB_HBM3.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=2048,device_name=NVIDIA_H100_80GB_HBM3.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_A100-SXM4-40GB.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_A100-SXM4-40GB.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_A100-SXM4-80GB.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_A100-SXM4-80GB.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_H100_80GB_HBM3,dtype=float8.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_H100_80GB_HBM3,dtype=float8.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_H100_80GB_HBM3.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=3584,device_name=NVIDIA_H100_80GB_HBM3.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=4096,device_name=NVIDIA_A100-SXM4-80GB.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=4096,device_name=NVIDIA_A100-SXM4-80GB.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=4096,device_name=NVIDIA_H100_80GB_HBM3.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=4096,device_name=NVIDIA_H100_80GB_HBM3.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=7168,device_name=NVIDIA_A100-SXM4-80GB.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=7168,device_name=NVIDIA_A100-SXM4-80GB.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=7168,device_name=NVIDIA_H100_80GB_HBM3,dtype=float8.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=7168,device_name=NVIDIA_H100_80GB_HBM3,dtype=float8.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/configs/E=8,N=7168,device_name=NVIDIA_H100_80GB_HBM3.json` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/configs/E=8,N=7168,device_name=NVIDIA_H100_80GB_HBM3.json`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/fused_moe/fused_moe.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/fused_moe/fused_moe.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/layernorm.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/layernorm.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/linear.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/linear.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/logits_processor.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/logits_processor.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/ops/rand.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/ops/rand.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/ops/sample.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/ops/sample.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/quantization/__init__.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/quantization/aqlm.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/aqlm.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/quantization/awq.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/awq.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/quantization/base_config.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/base_config.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/quantization/fp8.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/fp8.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/quantization/gptq.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/gptq.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/quantization/gptq_marlin.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/gptq_marlin.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/quantization/marlin.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/marlin.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/quantization/schema.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/schema.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/quantization/squeezellm.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/quantization/squeezellm.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/rejection_sampler.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/rejection_sampler.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/rotary_embedding.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/rotary_embedding.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/sampler.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/sampler.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/layers/vocab_parallel_embedding.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/layers/vocab_parallel_embedding.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/model_loader/__init__.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/model_loader/loader.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/loader.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/model_loader/neuron.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/neuron.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/model_loader/tensorizer.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/tensorizer.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/model_loader/utils.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/model_loader/weight_utils.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/model_loader/weight_utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/__init__.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/baichuan.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/baichuan.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/bloom.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/bloom.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/chatglm.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/chatglm.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/commandr.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/commandr.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/dbrx.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/decilm.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/decilm.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/deepseek.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/deepseek.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/falcon.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/falcon.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/gemma.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/gemma.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/gpt2.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/gpt_bigcode.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/gpt_bigcode.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/gpt_j.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/gpt_j.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/gpt_neox.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/internlm2.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/internlm2.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/jais.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/jais.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/llama.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/llama.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/llava.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/llava.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/minicpm.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/minicpm.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/mixtral.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/mixtral_quant.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/mixtral_quant.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/mpt.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/mpt.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/olmo.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/olmo.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/opt.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/opt.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/orion.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/orion.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/phi.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/phi.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/qwen.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/qwen.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/qwen2.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/qwen2_moe.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/qwen2_moe.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/stablelm.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/stablelm.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/starcoder2.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/starcoder2.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/models/xverse.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/models/xverse.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/sampling_metadata.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/sampling_metadata.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/model_executor/utils.py` & `vllm_acc-0.4.11714782966.854302/vllm/model_executor/utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/outputs.py` & `vllm_acc-0.4.11714782966.854302/vllm/outputs.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/sampling_params.py` & `vllm_acc-0.4.11714782966.854302/vllm/sampling_params.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/sequence.py` & `vllm_acc-0.4.11714782966.854302/vllm/sequence.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/spec_decode/batch_expansion.py` & `vllm_acc-0.4.11714782966.854302/vllm/spec_decode/batch_expansion.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/spec_decode/interfaces.py` & `vllm_acc-0.4.11714782966.854302/vllm/spec_decode/interfaces.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/spec_decode/metrics.py` & `vllm_acc-0.4.11714782966.854302/vllm/spec_decode/metrics.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/spec_decode/multi_step_worker.py` & `vllm_acc-0.4.11714782966.854302/vllm/spec_decode/multi_step_worker.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/spec_decode/ngram_worker.py` & `vllm_acc-0.4.11714782966.854302/vllm/spec_decode/ngram_worker.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/spec_decode/spec_decode_worker.py` & `vllm_acc-0.4.11714782966.854302/vllm/spec_decode/spec_decode_worker.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/spec_decode/top1_proposer.py` & `vllm_acc-0.4.11714782966.854302/vllm/spec_decode/top1_proposer.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/spec_decode/util.py` & `vllm_acc-0.4.11714782966.854302/vllm/spec_decode/util.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/test_utils.py` & `vllm_acc-0.4.11714782966.854302/vllm/test_utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/config.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/config.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/configs/__init__.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/configs/chatglm.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/chatglm.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/configs/dbrx.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/dbrx.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/configs/falcon.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/falcon.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/configs/jais.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/jais.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/configs/mpt.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/configs/mpt.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/detokenizer.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/detokenizer.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/tokenizer.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/tokenizer_group/__init__.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizer_group/__init__.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/tokenizer_group/base_tokenizer_group.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizer_group/base_tokenizer_group.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/tokenizer_group/ray_tokenizer_group.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizer_group/ray_tokenizer_group.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/tokenizer_group/tokenizer_group.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizer_group/tokenizer_group.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/transformers_utils/tokenizers/baichuan.py` & `vllm_acc-0.4.11714782966.854302/vllm/transformers_utils/tokenizers/baichuan.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/usage/usage_lib.py` & `vllm_acc-0.4.11714782966.854302/vllm/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/utils.py` & `vllm_acc-0.4.11714782966.854302/vllm/utils.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/worker/cache_engine.py` & `vllm_acc-0.4.11714782966.854302/vllm/worker/cache_engine.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/worker/cpu_model_runner.py` & `vllm_acc-0.4.11714782966.854302/vllm/worker/cpu_model_runner.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/worker/cpu_worker.py` & `vllm_acc-0.4.11714782966.854302/vllm/worker/cpu_worker.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/worker/model_runner.py` & `vllm_acc-0.4.11714782966.854302/vllm/worker/model_runner.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/worker/neuron_model_runner.py` & `vllm_acc-0.4.11714782966.854302/vllm/worker/neuron_model_runner.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/worker/neuron_worker.py` & `vllm_acc-0.4.11714782966.854302/vllm/worker/neuron_worker.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/worker/worker.py` & `vllm_acc-0.4.11714782966.854302/vllm/worker/worker.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm/worker/worker_base.py` & `vllm_acc-0.4.11714782966.854302/vllm/worker/worker_base.py`

 * *Files identical despite different names*

### Comparing `vllm_acc-0.4.1/vllm_acc.egg-info/PKG-INFO` & `vllm_acc-0.4.11714782966.854302/vllm_acc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vllm-acc
-Version: 0.4.1
+Version: 0.4.11714782966.854302
 Summary: A high-throughput and memory-efficient inference and serving engine for LLMs
 Home-page: https://github.com/vllm-project/vllm
 Author: vLLM Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/vllm-project/vllm
 Project-URL: Documentation, https://vllm.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: vllm-acc Version: 0.4.1 Summary: A high-throughput
-and memory-efficient inference and serving engine for LLMs Home-page: https://
-github.com/vllm-project/vllm Author: vLLM Team License: Apache 2.0 Project-URL:
-Homepage, https://github.com/vllm-project/vllm Project-URL: Documentation,
-https://vllm.readthedocs.io/en/latest/ Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-tensorizer License-File: LICENSE
+Metadata-Version: 2.1 Name: vllm-acc Version: 0.4.11714782966.854302 Summary: A
+high-throughput and memory-efficient inference and serving engine for LLMs
+Home-page: https://github.com/vllm-project/vllm Author: vLLM Team License:
+Apache 2.0 Project-URL: Homepage, https://github.com/vllm-project/vllm Project-
+URL: Documentation, https://vllm.readthedocs.io/en/latest/ Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Provides-Extra: tensorizer License-File: LICENSE
                                     [vLLM]
            ******** EEaassyy,, ffaasstt,, aanndd cchheeaapp LLLLMM sseerrvviinngg ffoorr eevveerryyoonnee ********
                   | _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn | _BB_ll_oo_gg | _PP_aa_pp_ee_rr | _DD_ii_ss_cc_oo_rr_dd |
 *Latest News* ð¥ - [2024/04] We hosted [the third vLLM meetup](https://
 robloxandvllmmeetup2024.splashthat.com/) with Roblox! Please find the meetup
 slides [here](https://docs.google.com/presentation/d/1A--
 47JAK4BJ39t954HyTkvtfwn0fkqtsL8NGFuslReM/edit?usp=sharing). - [2024/01] We
```

### Comparing `vllm_acc-0.4.1/vllm_acc.egg-info/SOURCES.txt` & `vllm_acc-0.4.11714782966.854302/vllm_acc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

