# Comparing `tmp/vkdispatch-0.0.3.tar.gz` & `tmp/vkdispatch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vkdispatch-0.0.3.tar", last modified: Wed Apr  3 19:24:59 2024, max compression
+gzip compressed data, was "vkdispatch-0.0.4.tar", last modified: Sat May  4 15:55:18 2024, max compression
```

## Comparing `vkdispatch-0.0.3.tar` & `vkdispatch-0.0.4.tar`

### file list

```diff
@@ -1,125 +1,373 @@
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.225972 vkdispatch-0.0.3/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11357 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/LICENSE
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1581 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/MANIFEST.in
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-04-03 19:24:59.225772 vkdispatch-0.0.3/PKG-INFO
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      121 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/README.md
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.201936 vkdispatch-0.0.3/deps/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.201848 vkdispatch-0.0.3/deps/VKL/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.201772 vkdispatch-0.0.3/deps/VKL/include/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.205981 vkdispatch-0.0.3/deps/VKL/include/VKL/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      553 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKL.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2037 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLBuffer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2580 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLCommandBuffer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      829 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLDescriptorSet.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8273 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLDevice.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1384 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLFramebuffer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2695 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLImage.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      834 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLImageView.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4280 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLInstance.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1482 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLPhysicalDevice.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2240 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLPipeline.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2984 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLPipelineLayout.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1166 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLQueue.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3570 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLRenderPass.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      671 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLStaticAllocator.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1790 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLSurface.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1628 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLSwapChain.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3975 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKL_base.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.208360 vkdispatch-0.0.3/deps/VKL/src/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8143 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLBuffer.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7097 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLCommandBuffer.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3646 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLDescriptorSet.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    24498 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLDevice.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3322 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLFramebuffer.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15023 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLImage.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2433 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLImageView.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11594 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLInstance.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3688 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLPhysicalDevice.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12903 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLPipeline.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12219 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLPipelineLayout.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2421 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLQueue.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6916 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLRenderPass.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3383 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLStaticAllocator.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5516 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLSurface.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10971 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLSwapChain.cpp
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.201990 vkdispatch-0.0.3/deps/VkFFT/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.208526 vkdispatch-0.0.3/deps/VkFFT/vkFFT/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.202939 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.208920 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12556 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91082 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    44680 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.202667 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.209370 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15591 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12866 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.202379 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.210229 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9486 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14546 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6762 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4342 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23925 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15546 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.210389 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23235 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7697 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.219662 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.220584 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5753 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11508 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    19521 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    22937 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   141736 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91669 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102595 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35985 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28166 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    84118 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6365 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.221118 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12743 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9610 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.221314 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   114660 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.221478 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1722 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.202875 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.222324 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    33238 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5016 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    26535 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27280 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16495 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    80386 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.222952 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    37848 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102541 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    73734 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   147838 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.223375 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    50505 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    17441 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.223559 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    58072 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3191 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      801 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/pyproject.toml
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       38 2024-04-03 19:24:59.226008 vkdispatch-0.0.3/setup.cfg
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2351 2024-04-03 19:23:31.000000 vkdispatch-0.0.3/setup.py
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.223823 vkdispatch-0.0.3/vkdispatch/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       51 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch/__init__.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1578 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch/init.py
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.225313 vkdispatch-0.0.3/vkdispatch.egg-info/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-04-03 19:24:59.000000 vkdispatch-0.0.3/vkdispatch.egg-info/PKG-INFO
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5203 2024-04-03 19:24:59.000000 vkdispatch-0.0.3/vkdispatch.egg-info/SOURCES.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-04-03 19:24:59.000000 vkdispatch-0.0.3/vkdispatch.egg-info/dependency_links.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-04-03 19:22:33.000000 vkdispatch-0.0.3/vkdispatch.egg-info/not-zip-safe
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       23 2024-04-03 19:24:59.000000 vkdispatch-0.0.3/vkdispatch.egg-info/requires.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-04-03 19:24:59.000000 vkdispatch-0.0.3/vkdispatch.egg-info/top_level.txt
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.225177 vkdispatch-0.0.3/vkdispatch_native/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      289 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch_native/base.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1736 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch_native/init.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      402 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch_native/init.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1329 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch_native/init_wrapper.pxd
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      432 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch_native/internal.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      164 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch_native/wrapper.pyx
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.088520 vkdispatch-0.0.4/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11357 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/LICENSE
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      764 2024-05-04 05:34:22.000000 vkdispatch-0.0.4/MANIFEST.in
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-05-04 15:55:18.087929 vkdispatch-0.0.4/PKG-INFO
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      121 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/README.md
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.020008 vkdispatch-0.0.4/deps/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.019345 vkdispatch-0.0.4/deps/VKL/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.018857 vkdispatch-0.0.4/deps/VKL/deps/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.022585 vkdispatch-0.0.4/deps/VKL/deps/VMA/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1099 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VKL/deps/VMA/LICENSE.txt
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.022715 vkdispatch-0.0.4/deps/VKL/deps/VMA/include/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   711190 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VKL/deps/VMA/include/vk_mem_alloc.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.023732 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      458 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/LICENSE.md
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.016959 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.027894 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vk_video/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16507 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_av1std.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4250 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_av1std_decode.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    13853 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2722 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std_decode.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6878 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h264std_encode.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23416 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2428 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std_decode.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7462 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codec_h265std_encode.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      660 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vk_video/vulkan_video_codecs_common.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.032646 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8164 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_icd.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7073 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_layer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2828 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vk_platform.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1555 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6201 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_android.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10381 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_beta.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)  1000714 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_core.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1866 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_directfb.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12470 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_fuchsia.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1896 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_ggp.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1309 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_ios.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1341 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_macos.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5907 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_metal.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4064 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_screen.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1282 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_vi.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1866 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_wayland.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15112 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_win32.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1880 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xcb.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1861 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xlib.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1411 2024-05-04 05:19:24.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Headers/include/vulkan/vulkan_xlib_xrandr.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.032791 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Utility-Libraries/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      304 2024-05-04 05:33:49.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Utility-Libraries/LICENSE.md
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.017130 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Utility-Libraries/include/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.032926 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.033314 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/layer/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3565 2024-05-04 05:33:49.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/layer/vk_layer_settings.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.033634 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   129114 2024-05-04 05:33:49.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/vk_dispatch_table.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   144058 2024-05-04 05:33:49.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/utility/vk_format_utils.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   495518 2024-05-04 05:33:49.000000 vkdispatch-0.0.4/deps/VKL/deps/Vulkan-Utility-Libraries/include/vulkan/vk_enum_string_helper.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.033831 vkdispatch-0.0.4/deps/VKL/deps/glslang/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    54705 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/LICENSE.txt
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.040536 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.040673 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/CInterface/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4254 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/CInterface/spirv_c_interface.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3616 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/GLSL.ext.AMD.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1598 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/GLSL.ext.ARM.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2585 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/GLSL.ext.EXT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4486 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/GLSL.ext.KHR.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3781 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/GLSL.ext.NV.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1808 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/GLSL.ext.QCOM.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4126 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/GLSL.std.450.h
+-rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)   461067 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/GlslangToSpv.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2666 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/GlslangToSpv.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5747 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/InReadableOrder.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2731 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/Logger.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2685 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/Logger.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1858 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/NonSemanticDebugPrintf.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7908 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/NonSemanticShaderDebugInfo100.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11638 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/SPVRemapper.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   152756 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/SpvBuilder.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    45577 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/SpvBuilder.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    21678 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/SpvPostProcess.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12426 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/SpvTools.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4677 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/SpvTools.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3316 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/bitutils.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35712 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/disassemble.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1926 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/disassemble.h
+-rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)   195172 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/doc.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8080 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/doc.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    39345 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/hex_float.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   140795 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/spirv.hpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    19791 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/SPIRV/spvIR.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.040921 vkdispatch-0.0.4/deps/VKL/deps/glslang/StandAlone/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5782 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/StandAlone/DirStackFileIncluder.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2821 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/StandAlone/Worklist.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.041351 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/bar.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       30 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/foo.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       24 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/i1.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.042819 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc1/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       21 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc1/badInc.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc1/bar.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       32 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc1/foo.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.043347 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc1/path1/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       14 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc1/path1/bar.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc1/path1/local.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       51 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc1/path1/notHere.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.043705 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc1/path2/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       14 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc1/path2/bar.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       15 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc1/path2/notHere.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc1/path2/remote.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.044007 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc2/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       28 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc2/bar.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/inc2/foo.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       11 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/Test/parent.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.018668 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.044125 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/CInterface/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16918 2024-05-04 04:47:39.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/CInterface/glslang_c_interface.cpp
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.044372 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/GenericCodeGen/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2607 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/GenericCodeGen/CodeGen.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2750 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/GenericCodeGen/Link.cpp
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.045595 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/HLSL/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2132 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/HLSL/hlslAttributes.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6781 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/HLSL/hlslGrammar.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2327 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/HLSL/hlslOpMap.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28652 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/HLSL/hlslParseHelper.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2622 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/HLSL/hlslParseables.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3560 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/HLSL/hlslScanContext.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3856 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/HLSL/hlslTokenStream.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9628 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/HLSL/hlslTokens.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1996 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/HLSL/pch.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.047605 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/
+-rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)    21618 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/BaseTypes.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9241 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/Common.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35998 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/ConstantUnion.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5927 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/InfoSink.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1854 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/InitializeGlobals.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11856 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/PoolAlloc.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5664 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/ResourceLimits.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6312 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/ShHandle.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4413 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/SpirvIntrinsics.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   109017 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/Types.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12025 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/arrays.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11752 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/glslang_c_interface.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9017 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/glslang_c_shader_types.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    61736 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Include/intermediate.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.060521 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    61113 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/Constant.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3142 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/InfoSink.cpp
+-rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)   562823 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/Initialize.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5491 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/Initialize.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8084 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/IntermTraverse.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   139980 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/Intermediate.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6435 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/LiveTraverser.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27638 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseContextBase.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   481062 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseHelper.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    33022 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/ParseHelper.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9110 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/PoolAlloc.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3121 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/RemoveTree.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1704 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/RemoveTree.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    76508 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/Scan.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9697 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/Scan.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3206 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/ScanContext.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    83435 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/ShaderLang.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12826 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/SpirvIntrinsics.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    17198 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/SymbolTable.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    36832 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/SymbolTable.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    69599 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/Versions.cpp
+-rwxr-xr-x   0 shaharsandhaus   (501) staff       (20)    25529 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/Versions.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12678 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/attribute.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4554 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/attribute.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10171 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/gl_types.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   654870 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/glslang_tab.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28552 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/glslang_tab.cpp.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    94894 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/intermOut.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    76316 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/iomapper.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14491 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/iomapper.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6408 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/limits.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   109336 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/linkValidate.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    53321 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/localintermediate.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7568 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/parseConst.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10098 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/parseVersions.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1896 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/pch.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.061510 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    50129 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/Pp.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6672 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpAtom.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5211 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpContext.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27894 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpContext.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    57222 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpScanner.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7488 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpTokens.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5791 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/preprocessor/PpTokens.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    40778 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/propagateNoContraction.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2417 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/propagateNoContraction.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    56404 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/reflection.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8171 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/reflection.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3346 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/MachineIndependent/span.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.061662 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/OSDependent/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1751 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/OSDependent/osinclude.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.062092 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Public/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2438 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Public/ResourceLimits.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    43942 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Public/ShaderLang.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2295 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/Public/resource_limits_c.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.062393 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/ResourceLimits/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    34391 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/ResourceLimits/ResourceLimits.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2145 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/glslang/ResourceLimits/resource_limits_c.cpp
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.063346 vkdispatch-0.0.4/deps/VKL/deps/glslang/gtests/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2130 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/gtests/Initializer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2142 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/gtests/Settings.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    32978 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/gtests/TestFixture.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1678 2024-05-04 04:29:15.000000 vkdispatch-0.0.4/deps/VKL/deps/glslang/gtests/pch.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.018920 vkdispatch-0.0.4/deps/VKL/deps/volk/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.064746 vkdispatch-0.0.4/deps/VKL/deps/volk/volk/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1066 2024-05-04 03:43:54.000000 vkdispatch-0.0.4/deps/VKL/deps/volk/volk/LICENSE.md
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   252357 2024-05-04 03:43:54.000000 vkdispatch-0.0.4/deps/VKL/deps/volk/volk/volk.c
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   127213 2024-05-04 03:43:54.000000 vkdispatch-0.0.4/deps/VKL/deps/volk/volk/volk.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.019131 vkdispatch-0.0.4/deps/VKL/include/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.068799 vkdispatch-0.0.4/deps/VKL/include/VKL/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      553 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKL.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1937 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLBuffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2741 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLCommandBuffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      829 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLDescriptorSet.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8377 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLDevice.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1384 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLFramebuffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2938 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLImage.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      834 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLImageView.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4176 2024-05-04 03:41:07.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLInstance.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1859 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLPhysicalDevice.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2240 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLPipeline.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2984 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLPipelineLayout.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1077 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLQueue.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3570 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLRenderPass.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      671 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLStaticAllocator.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1790 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLSurface.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1628 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKLSwapChain.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4305 2024-05-04 04:04:13.000000 vkdispatch-0.0.4/deps/VKL/include/VKL/VKL_base.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.068953 vkdispatch-0.0.4/deps/VKL/include/glslang/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2895 2024-05-04 05:27:42.000000 vkdispatch-0.0.4/deps/VKL/include/glslang/build_info.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.071755 vkdispatch-0.0.4/deps/VKL/src/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7536 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/src/VKLBuffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7748 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/src/VKLCommandBuffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3646 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/src/VKLDescriptorSet.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    25947 2024-05-04 04:01:54.000000 vkdispatch-0.0.4/deps/VKL/src/VKLDevice.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3322 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/src/VKLFramebuffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16236 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/src/VKLImage.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2433 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/src/VKLImageView.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14379 2024-05-04 03:41:46.000000 vkdispatch-0.0.4/deps/VKL/src/VKLInstance.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4502 2024-05-04 03:29:09.000000 vkdispatch-0.0.4/deps/VKL/src/VKLPhysicalDevice.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12903 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/src/VKLPipeline.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12997 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/src/VKLPipelineLayout.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2167 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/src/VKLQueue.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6916 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/src/VKLRenderPass.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3383 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/src/VKLStaticAllocator.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5503 2024-05-04 03:31:09.000000 vkdispatch-0.0.4/deps/VKL/src/VKLSurface.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10896 2024-05-04 03:04:57.000000 vkdispatch-0.0.4/deps/VKL/src/VKLSwapChain.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       52 2024-05-04 03:22:46.000000 vkdispatch-0.0.4/deps/VKL/src/VMAImpl.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       53 2024-05-04 03:22:41.000000 vkdispatch-0.0.4/deps/VKL/src/VolkImpl.cpp
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.071871 vkdispatch-0.0.4/deps/VkFFT/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1084 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/LICENSE
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.071979 vkdispatch-0.0.4/deps/VkFFT/vkFFT/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.021543 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.072502 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12556 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91082 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    44680 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.021258 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.073067 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15591 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12866 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.020855 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.073983 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9486 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14546 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6762 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4342 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23925 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15546 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.074198 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23235 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7697 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.075914 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.076624 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5753 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11508 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    19521 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    22937 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   141736 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91669 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102595 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35985 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28166 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    84118 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6365 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.077025 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12743 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9610 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.077180 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   114660 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.077345 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1722 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.021484 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.078172 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    33238 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5016 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    26535 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27280 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16495 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    80386 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.078782 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    37848 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102541 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    73734 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   147838 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.079127 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    50505 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    17441 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.079273 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    58072 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3191 2024-05-04 03:06:00.000000 vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      851 2024-05-04 15:54:43.000000 vkdispatch-0.0.4/pyproject.toml
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       38 2024-05-04 15:55:18.088655 vkdispatch-0.0.4/setup.cfg
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3786 2024-05-04 06:49:14.000000 vkdispatch-0.0.4/setup.py
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.081230 vkdispatch-0.0.4/vkdispatch/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1057 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch/__init__.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       88 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch/__main__.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1327 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch/buffer.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2060 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch/command_list.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1625 2024-05-04 15:49:26.000000 vkdispatch-0.0.4/vkdispatch/context.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      374 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch/descriptor_set.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4176 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch/dtype.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7426 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch/image.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4678 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch/init.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9696 2024-05-04 15:49:45.000000 vkdispatch-0.0.4/vkdispatch/shader_builder.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4287 2024-05-04 15:50:15.000000 vkdispatch-0.0.4/vkdispatch/shader_decorator.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8396 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch/shader_variable.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      858 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch/stage_compute.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2026 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch/stage_fft.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8475 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch/stage_transfer.py
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.087323 vkdispatch-0.0.4/vkdispatch.egg-info/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-05-04 15:55:17.000000 vkdispatch-0.0.4/vkdispatch.egg-info/PKG-INFO
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15881 2024-05-04 15:55:18.000000 vkdispatch-0.0.4/vkdispatch.egg-info/SOURCES.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-05-04 15:55:17.000000 vkdispatch-0.0.4/vkdispatch.egg-info/dependency_links.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       52 2024-05-04 15:55:17.000000 vkdispatch-0.0.4/vkdispatch.egg-info/entry_points.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-05-04 03:06:34.000000 vkdispatch-0.0.4/vkdispatch.egg-info/not-zip-safe
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       23 2024-05-04 15:55:17.000000 vkdispatch-0.0.4/vkdispatch.egg-info/requires.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-05-04 15:55:17.000000 vkdispatch-0.0.4/vkdispatch.egg-info/top_level.txt
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-05-04 15:55:18.087158 vkdispatch-0.0.4/vkdispatch_native/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      222 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/base.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3664 2024-05-04 03:12:26.000000 vkdispatch-0.0.4/vkdispatch_native/buffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      661 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/buffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1740 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/buffer.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3138 2024-05-04 05:22:58.000000 vkdispatch-0.0.4/vkdispatch_native/command_list.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      605 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/command_list.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1642 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/command_list.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1729 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/context.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      276 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/context.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1239 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/context.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1141 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/descriptor_set.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      378 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/descriptor_set.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1040 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/descriptor_set.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8683 2024-05-04 05:33:00.000000 vkdispatch-0.0.4/vkdispatch_native/image.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1017 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/image.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4124 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/image.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4108 2024-05-04 03:40:31.000000 vkdispatch-0.0.4/vkdispatch_native/init.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1133 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/init.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2864 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/init.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1703 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/internal.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3574 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/stage_compute.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      797 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/stage_compute.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2108 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/stage_compute.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2803 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/stage_fft.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      410 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/stage_fft.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1519 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/stage_fft.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7021 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/stage_transfer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1383 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/stage_transfer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5522 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/stage_transfer.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      308 2024-05-04 03:04:33.000000 vkdispatch-0.0.4/vkdispatch_native/wrapper.pyx
```

### Comparing `vkdispatch-0.0.3/LICENSE` & `vkdispatch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/PKG-INFO` & `vkdispatch-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkdispatch
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python module for orchestrating and dispatching large computations across multi-GPU systems using Vulkan.
 Author-email: Shahar Sandhaus <shahar.sandhaus@gmail.com>
 Project-URL: Homepage, https://github.com/sharhar/vkdispatch
 Project-URL: Issues, https://github.com/sharhar/vkdispatch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKL.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKL.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLCommandBuffer.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLCommandBuffer.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 #ifndef VKLCommandBuffer_h
 #define VKLCommandBuffer_h
 
 #include "VKL_base.h"
 
 class VKLCommandBuffer : public VKLHandle<VkCommandBuffer> {
 public:
-	VKLCommandBuffer(const VKLQueue* queue);
+	VKLCommandBuffer(const VKLQueue* queue, int count = 1);
 
 	VkCommandPool pool() const;
+	VkCommandPool* pPool() const;
+
+	VkFence fence() const;
+	VkFence* pFence() const;
 	
 	void bufferBarrier(VKLBuffer* buffer, VkPipelineStageFlags srcStageMask, VkPipelineStageFlags dstStageMask) const;
 	
 	void copyBuffer(const VKLBuffer* dst, const VKLBuffer* src, VkBufferCopy bufferCopy) const;
 	void copyImage(const VKLImage* dst, const VKLImage* src, VkImageCopy imageCopy) const;
 	
 	void begin() const;
 	void end() const;
-	void reset() const;
 	
 	void beginRenderPass(const VKLFramebuffer& framebuffer, VkSubpassContents contents) const;
 	void beginRenderPass(const VKLFramebuffer& framebuffer, VkSubpassContents contents, VkRect2D area) const;
 	
 	void beginRenderPass(const VKLFramebuffer* framebuffer, VkSubpassContents contents) const;
 	void beginRenderPass(const VKLFramebuffer* framebuffer, VkSubpassContents contents, VkRect2D area) const;
 	
@@ -48,13 +51,17 @@
 	
 	void draw(uint32_t vertexCount, uint32_t instanceCount, uint32_t firstVertex, uint32_t firstInstance) const;
 	void dispatch(uint32_t x, uint32_t y, uint32_t z) const;
 
 	void destroy();
 //private:
 	VkCommandPool m_pool;
+	VkCommandBuffer* m_handles;
+	VkFence* m_fences;
+	int m_count;
+	int m_current_index;
 	
 	const VKLQueue* m_queue;
 	const VKLDevice* m_device;
 };
 
 #endif /* VKLCommandBuffer_h */
```

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLDescriptorSet.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLDescriptorSet.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLDevice.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLDevice.h`

 * *Files 4% similar despite different names*

```diff
@@ -138,14 +138,16 @@
 	PFN_vkAcquireNextImageKHR AcquireNextImageKHR;
 	PFN_vkQueuePresentKHR QueuePresentKHR;
 
 	PFN_vkGetMemoryFdKHR GetMemoryFdKHR;
 	PFN_vkGetSemaphoreFdKHR GetSemaphoreFdKHR;
 } VKLDevicePFNS;
 
+#define VKL_QUEUE_TYPE_COUNT 4
+
 typedef enum VKLQueueType {
 	VKL_QUEUE_TYPE_GRAPHICS = 0,
 	VKL_QUEUE_TYPE_COMPUTE = 1,
 	VKL_QUEUE_TYPE_TRANSFER = 2,
 	VKL_QUEUE_TYPE_ALL = 3
 } VKLQueueType;
 
@@ -181,29 +183,30 @@
 	void _printSelections();
 
 	bool _supportsExtension(const char* extension);
 	bool _supportsLayer(const char* layer);
 
 	std::vector<VkDeviceQueueCreateInfo> m_queueCreateInfos;
 	VkDeviceCreateInfo m_createInfo;
-	VkPhysicalDeviceFeatures m_features;
+	VkPhysicalDeviceFeatures2 m_features;
 
 	bool _validate();
 
 	friend class VKLDevice;
 };
 
 class VKLDevice : public VKLHandle<VkDevice>, public VKLCreator<VKLDeviceCreateInfo> {
 public:
 	VKLDevice();
 	VKLDevice(const VKLDeviceCreateInfo& createInfo);
 
 	const VkAllocationCallbacks* allocationCallbacks() const;
 	PFN_vkVoidFunction procAddr(const char* name) const;
 	const VKLPhysicalDevice* physical() const;
+	const VmaAllocator& allocatorVMA() const;
 	
 	const VKLQueue* getQueue(VKLQueueType type, uint32_t queueIndex) const;
 	
 	VkFence createFence(VkFenceCreateFlags flags) const;
 	void waitForFence(VkFence fence) const;
 	void resetFence(VkFence fence) const;
 	void destroyFence(VkFence fence) const;
@@ -216,13 +219,15 @@
 	VKLDevicePFNS vk;
 private:
 	std::vector<VKLQueue> m_queues[4];
 
 	const VKLInstance* m_instance;
 	const VKLPhysicalDevice* m_physicalDevice;
 	const VkAllocationCallbacks* m_allocationCallbacks;
+
+	VmaAllocator m_allocator;
 	
 	void _destroy();
 	void _create(const VKLDeviceCreateInfo& createInfo);
 };
 
 #endif
```

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLFramebuffer.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLFramebuffer.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLImage.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLImage.h`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,32 @@
 	VKLImageCreateInfo& imageType(VkImageType type);
 	VKLImageCreateInfo& format(VkFormat format);
 	VKLImageCreateInfo& extent(uint32_t width, uint32_t height, uint32_t depth);
 	VKLImageCreateInfo& tiling(VkImageTiling tiling);
 	VKLImageCreateInfo& usage(VkImageUsageFlags usage);
 	VKLImageCreateInfo& initialLayout(VkImageLayout layout);
 
-	VKLImageCreateInfo& arrayLevels(uint32_t arrayLevels);
+	VKLImageCreateInfo& arrayLayers(uint32_t arrayLayers);
 	
 	VKLImageCreateInfo& memoryProperties(VkMemoryPropertyFlags memoryProperties);	
 
+	VKLImageCreateInfo& useVMA(bool useVMA);
+	VKLImageCreateInfo& usageVMA(VmaMemoryUsage usage);
+	VKLImageCreateInfo& flagsVMA(VmaAllocationCreateFlags flags);
+
 private:
 	VkImageCreateInfo m_imageCreateInfo;
-
 	void* m_allocationPNext;
-	
 	VkMemoryPropertyFlags m_memoryProperties;
-	
 	const VKLDevice* m_device;
 
+	bool useVMAFlag;
+	VmaMemoryUsage usageVMAFlag;
+	VmaAllocationCreateFlags flagsVMAFlag;
+
 	bool _validate();
 
 	friend class VKLImage;
 };
 
 class VKLImage : public VKLHandle<VkImage>, public VKLCreator<VKLImageCreateInfo> {
 public:
```

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLImageView.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLImageView.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLInstance.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLInstance.h`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 #define VKLInstance_h
 
 #include <VKL/VKL_base.h>
 #include <VKL/VKLPhysicalDevice.h>
 
 #include <vector>
 
+/*
+
 typedef struct VKLInstancePFNS {
 	PFN_vkCreateInstance CreateInstance;
 	PFN_vkDestroyInstance DestroyInstance;
 	PFN_vkEnumeratePhysicalDevices EnumeratePhysicalDevices;
 	PFN_vkGetInstanceProcAddr GetInstanceProcAddr;
 	PFN_vkEnumerateInstanceExtensionProperties EnumerateInstanceExtensionProperties;
 	PFN_vkEnumerateInstanceLayerProperties EnumerateInstanceLayerProperties;
 
-	PFN_vkCreateDebugReportCallbackEXT CreateDebugReportCallbackEXT;
-	PFN_vkDestroyDebugReportCallbackEXT DestroyDebugReportCallbackEXT;
-	PFN_vkDebugReportMessageEXT DebugReportMessageEXT;
+	PFN_vkCreateDebugUtilsMessengerEXT CreateDebugUtilsMessengerEXT;
+	PFN_vkDestroyDebugUtilsMessengerEXT DestroyDebugUtilsMessengerEXT;
 
 	PFN_vkGetPhysicalDeviceFeatures GetPhysicalDeviceFeatures;
 	PFN_vkGetPhysicalDeviceFormatProperties GetPhysicalDeviceFormatProperties;
 	PFN_vkGetPhysicalDeviceImageFormatProperties GetPhysicalDeviceImageFormatProperties;
 	PFN_vkGetPhysicalDeviceProperties GetPhysicalDeviceProperties;
 	PFN_vkGetPhysicalDeviceProperties2 GetPhysicalDeviceProperties2;
 	PFN_vkGetPhysicalDeviceQueueFamilyProperties GetPhysicalDeviceQueueFamilyProperties;
@@ -43,25 +44,25 @@
 	PFN_vkVoidFunction GetPhysicalDeviceWin32PresentationSupportKHR;
 #endif
 	
 #ifdef VKL_SURFACE_MACOS
 	PFN_vkVoidFunction CreateMetalSurfaceEXT;
 #endif
 } __VKLInstancePFNS;
+*/
 
 class VKLInstanceCreateInfo : public VKLCreateInfo<VKLInstanceCreateInfo>{
 public:
 	VKLInstanceCreateInfo();
 	
 	VKLInstanceCreateInfo& allocationCallbacks(VkAllocationCallbacks* allocationCallbacks);
 	VKLInstanceCreateInfo& addLayer(const char* layer);
 	VKLInstanceCreateInfo& addExtension(const char* extension);
 	VKLInstanceCreateInfo& addExtensions(const char** extensions, uint32_t extensionCount);
 	VKLInstanceCreateInfo& debug(VkBool32 debug);
-	VKLInstanceCreateInfo& procAddr(PFN_vkGetInstanceProcAddr vkFunc);
 	
 	void printSelections();
 	
 	bool supportsExtension(const char* extension);
 	bool supportsLayer(const char* layer);
 	
 	std::vector<VkExtensionProperties> supportedExtensions;
@@ -69,15 +70,14 @@
 private:
 	PFN_vkEnumerateInstanceExtensionProperties m_vkEnumerateInstanceExtensionProperties;
 	PFN_vkEnumerateInstanceLayerProperties m_vkEnumerateInstanceLayerProperties;
 
 	VkApplicationInfo m_appInfo;
 	VkInstanceCreateInfo m_createInfo;
 
-	PFN_vkGetInstanceProcAddr m_procAddr;
 	VkAllocationCallbacks* m_allocationCallbacks;
 
 	void _printSelections();
 
 	bool _supportsExtension(const char* extension);
 	bool _supportsLayer(const char* layer);
 
@@ -94,25 +94,27 @@
 class VKLInstance : public VKLHandle<VkInstance>, public VKLCreator<VKLInstanceCreateInfo> {
 public:
 	VKLInstance();
 	VKLInstance(const VKLInstanceCreateInfo& createInfo);
 	
 	const VkAllocationCallbacks* allocationCallbacks() const;
 	PFN_vkVoidFunction procAddr(const char* name) const;
-	const std::vector<VKLPhysicalDevice>& getPhysicalDevices() const;
+	const std::vector<VKLPhysicalDevice*>& getPhysicalDevices() const;
 	const std::vector<const char*>& getLayers() const;
 	const std::vector<const char*>& getExtensions() const;
 	
-	VKLInstancePFNS vk;
+	//VKLInstancePFNS vk;
 private:
 	const VkAllocationCallbacks* m_allocationCallbacks;
 
+	VkDebugUtilsMessengerEXT debug_messenger;
+
 	VkDebugReportCallbackEXT m_debugCallback;
 
-	std::vector<VKLPhysicalDevice> m_physicalDevices;
+	std::vector<VKLPhysicalDevice*> m_physicalDevices;
 	
 	std::vector<const char*> m_layers;
 	std::vector<const char*> m_extensions;
 
 	void _create(const VKLInstanceCreateInfo& createInfo);
 	void _destroy();
 };
```

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLPhysicalDevice.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLPhysicalDevice.h`

 * *Files 12% similar despite different names*

```diff
@@ -6,32 +6,38 @@
 #include <vector>
 
 class VKLPhysicalDevice : public VKLHandle<VkPhysicalDevice> {
 public:
 	const VKLInstance* instance() const;
 
 	VkPhysicalDeviceFeatures getFeatures() const;
+	VkPhysicalDeviceFeatures2 getFeatures2() const;
+	VkPhysicalDeviceShaderAtomicFloatFeaturesEXT getAtomicFloatFeatures() const;	
 	VkFormatProperties getFormatProperties(VkFormat format) const;
 	VkImageFormatProperties getImageFormatProperties(VkFormat format, VkImageType type, VkImageTiling tiling, VkImageUsageFlags usage, VkImageCreateFlags flags) const;
 	VkPhysicalDeviceProperties getProperties() const;
+	VkPhysicalDeviceProperties2 getProperties2() const;
+	VkPhysicalDeviceSubgroupProperties getSubgroupProperties() const;
 	const std::vector<VkQueueFamilyProperties>& getQueueFamilyProperties() const;
 	VkPhysicalDeviceMemoryProperties getMemoryProperties() const;
 	const std::vector<VkExtensionProperties>& getExtensions() const;
 	
 	VkBool32 getSurfaceSupport(VkSurfaceKHR surface, uint32_t queueFamilyIndex) const;
 	VkSurfaceCapabilitiesKHR getSurfaceCapabilities(VkSurfaceKHR surface) const;
 	std::vector<VkSurfaceFormatKHR> getSurfaceFormats(VkSurfaceKHR surface) const;
 	std::vector<VkPresentModeKHR> getSurfacePresentModes(VkSurfaceKHR surface) const;
 private:
 	VKLPhysicalDevice(VkPhysicalDevice physicalDevice, const VKLInstance* instance);
 
 	const VKLInstance* m_instance;
 
-	VkPhysicalDeviceFeatures m_features;
-	VkPhysicalDeviceProperties m_properties;
+	VkPhysicalDeviceFeatures2 m_features;
+	VkPhysicalDeviceShaderAtomicFloatFeaturesEXT m_atomicFloatFeatures;
+	VkPhysicalDeviceProperties2 m_properties;
+	VkPhysicalDeviceSubgroupProperties m_subgroupProperties;
 	std::vector<VkQueueFamilyProperties> m_queueFamilyProperties;
 	std::vector<VkExtensionProperties> m_extensions;
 	VkPhysicalDeviceMemoryProperties m_memoryProperties;
 
 	friend class VKLInstance;
 };
```

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLPipeline.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLPipeline.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLPipelineLayout.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLPipelineLayout.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLQueue.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLQueue.h`

 * *Files 21% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 
 #include "VKL_base.h"
 
 class VKLQueue : public VKLHandle<VkQueue> {
 public:
 	uint32_t getFamilyIndex() const;
 	const VKLDevice* device() const;
-	VkFence fence() const;
 	VKLCommandBuffer* getCmdBuffer() const;
 	
 	void submitAndWait(const VKLCommandBuffer* cmdBuffer) const;
 	void submitAndWait(const VKLCommandBuffer* cmdBuffer, uint32_t waitSemaphoreCount, const VkSemaphore* pWaitSemaphores, const VkPipelineStageFlags* pWaitDstStageMask) const;
 	
-	void submit(const VKLCommandBuffer* cmdBuffer, VkFence fence) const;
-	void submit(const VKLCommandBuffer* cmdBuffer, VkFence fence, const VkSemaphore* signalSempahore) const;
-	void submit(const VKLCommandBuffer* cmdBuffer, VkFence fence, const VkSemaphore* signalSempahore, uint32_t waitSemaphoreCount, const VkSemaphore* pWaitSemaphores, const VkPipelineStageFlags* pWaitDstStageMask) const;
+	void submit(const VKLCommandBuffer* cmdBuffer) const;
+	void submit(const VKLCommandBuffer* cmdBuffer, const VkSemaphore* signalSempahore) const;
+	void submit(const VKLCommandBuffer* cmdBuffer, const VkSemaphore* signalSempahore, uint32_t waitSemaphoreCount, const VkSemaphore* pWaitSemaphores, const VkPipelineStageFlags* pWaitDstStageMask) const;
 	void waitIdle() const;
 private:
 	VKLQueue();
 	void init(const VKLDevice* device, VkQueue queue, uint32_t familyIndex);
 	void destroy();
 	
 	uint32_t m_familyIndex;
 	VKLCommandBuffer* m_cmdBuffer;
-	
-	VkFence m_fence;
 
 	const VKLDevice* m_device;
 	
 	friend class VKLDevice;
 };
 
 #endif
```

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLRenderPass.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLRenderPass.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLStaticAllocator.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLStaticAllocator.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLSurface.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLSurface.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLSwapChain.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKLSwapChain.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/include/VKL/VKL_base.h` & `vkdispatch-0.0.4/deps/VKL/include/VKL/VKL_base.h`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,20 @@
 
 //#ifndef _DEBUG
 //#define VK_CALL(result) result;
 //#endif
 
 #define VKL_VALIDATION
 
-//#define VK_NO_PROTOTYPES
+#define VK_NO_PROTOTYPES
+#define VMA_STATIC_VULKAN_FUNCTIONS 0
+#define VMA_DYNAMIC_VULKAN_FUNCTIONS 1
 #include <vulkan/vulkan.h>
+#include <volk/volk.h>
+#include <vk_mem_alloc.h>
 
 #include <assert.h>
 #include <stdio.h>
 #include <string.h>
 #include <stdlib.h>
 
 class VKLInstance;
@@ -50,15 +54,15 @@
         vprintf(full_format, args);
         free(full_format);
     }
 
     va_end(args);
 }
 
-#define LOGGING_INFO
+//#define LOGGING_INFO
 #define LOGGING_ERROR
 
 #ifdef LOGGING_INFO
 
 inline void log_message_noendl(const char* level, const char* format, ...) {
     va_list args;
     va_start(args, format);
@@ -99,14 +103,15 @@
 
 
 template<typename T>
 class VKLHandle {
 public:
 	VKLHandle() { m_handle = (T)VK_NULL_HANDLE;}
 	T handle() const { return m_handle; }
+	T* pHandle() const { return (T*)&m_handle; }
 protected:
 	T m_handle;
 };
 
 template<typename T>
 class VKLCreateInfo {
 public:
@@ -173,14 +178,21 @@
 	const char* m_name;
 	
 	virtual void _destroy() = 0;
 	virtual void _create(const T& createInfo) = 0;
 };
 
 typedef struct {
+	uint32_t vma_enabled;
+	VmaAllocation vma_allocation = {};
+	VmaAllocationInfo vma_allocation_info = {};
+
 	VkDeviceMemory memory = (VkDeviceMemory)VK_NULL_HANDLE;
 	VkDeviceSize size = 0;
 	VkDeviceSize offset = 0;
+
+	VKLImage* image = NULL;
+	VKLBuffer* buffer = NULL;
 } VKLAllocation;
 
 
 #endif
```

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLBuffer.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLBuffer.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -23,72 +23,53 @@
 	m_memoryBarrier.srcQueueFamilyIndex = VK_QUEUE_FAMILY_IGNORED;
 	m_memoryBarrier.dstQueueFamilyIndex = VK_QUEUE_FAMILY_IGNORED;
 	m_memoryBarrier.offset = 0;
 	
 	this->create(createInfo);
 }
 
-void VKLBuffer::setData(void* data, size_t size, size_t offset) {
-	uint8_t* mappedData;
-	VK_CALL(m_device->vk.MapMemory(m_device->handle(), m_allocation.memory, m_allocation.offset, m_allocation.size, 0, (void**)&mappedData));	
-	memcpy(mappedData + offset, data, size);
-	m_device->vk.UnmapMemory(m_device->handle(), m_allocation.memory);
-}
-
-void VKLBuffer::setData(const VKLQueue* transferQueue, VKLBuffer* stagingBuffer, void* data, size_t size, size_t offset) {
-	LOG_INFO("Setting data through staging buffer");
-	stagingBuffer->setData(data, size, 0);
-	
-	VkBufferCopy bufferCopy;
-	bufferCopy.size = size;
-	bufferCopy.dstOffset = offset;
-	bufferCopy.srcOffset = 0;
-	
-	LOG_INFO("Copying data from staging buffer to buffer");
-
-	copyFrom(stagingBuffer, transferQueue, bufferCopy);
-}
-
 void* VKLBuffer::map() {
 	void* result;
-	VK_CALL(m_device->vk.MapMemory(m_device->handle(), m_allocation.memory, m_allocation.offset, m_allocation.size, 0, &result));
+	
+	if (m_allocation.vma_enabled)
+		VK_CALL(vmaMapMemory(m_device->allocatorVMA(), m_allocation.vma_allocation, &result)) 
+	else
+		VK_CALL(m_device->vk.MapMemory(m_device->handle(), m_allocation.memory, m_allocation.offset, m_allocation.size, 0, &result));
+
 	return result;
 }
 void VKLBuffer::unmap() {
-	m_device->vk.UnmapMemory(m_device->handle(), m_allocation.memory);
+	if (m_allocation.vma_enabled)
+		vmaUnmapMemory(m_device->allocatorVMA(), m_allocation.vma_allocation);
+	else
+		m_device->vk.UnmapMemory(m_device->handle(), m_allocation.memory);
+}
+
+void VKLBuffer::setData(void* data, size_t size, size_t offset) {
+	uint8_t* mappedData = (uint8_t*)map();
+	memcpy(mappedData + offset, data, size);
+	unmap();
 }
 
 void VKLBuffer::getData(void* data, size_t size, size_t offset) {
-	uint8_t* mappedData;
-	VK_CALL(m_device->vk.MapMemory(m_device->handle(), m_allocation.memory, m_allocation.offset, m_allocation.size, 0, (void**)&mappedData));
+	uint8_t* mappedData = (uint8_t*)map();
 	memcpy(data, mappedData + offset, size);
-	m_device->vk.UnmapMemory(m_device->handle(), m_allocation.memory);
+	unmap();
 }
 
 VKLAllocation VKLBuffer::allocation() const {
 	return m_allocation;
 }
 
 VkMemoryRequirements VKLBuffer::memoryRequirements() const {
 	VkMemoryRequirements memoryRequirements;
 	m_device->vk.GetBufferMemoryRequirements(m_device->handle(), m_handle, &memoryRequirements);
 	return memoryRequirements;
 }
 
-void VKLBuffer::getData(const VKLQueue* transferQueue, VKLBuffer* stagingBuffer, void* data, size_t size, size_t offset) {
-	VkBufferCopy bufferCopy;
-	bufferCopy.size = size;
-	bufferCopy.dstOffset = 0;
-	bufferCopy.srcOffset = offset;
-	
-	stagingBuffer->copyFrom(this, transferQueue, bufferCopy);
-	
-	stagingBuffer->getData(data, size, 0);
-}
-
 void VKLBuffer::setNewAccessMask(VkAccessFlags accessMask) {
 	m_memoryBarrier.dstAccessMask = accessMask;
 }
 
 VkBufferMemoryBarrier* VKLBuffer::getMemoryBarrier() {
 	return &m_memoryBarrier;
 }
@@ -100,91 +81,102 @@
 
 void VKLBuffer::copyFrom(VKLBuffer* src, const VKLQueue* transferQueue, VkBufferCopy bufferCopy) {
 	transferQueue->getCmdBuffer()->begin();
 	transferQueue->getCmdBuffer()->copyBuffer(this, src, bufferCopy);
 	transferQueue->getCmdBuffer()->end();
 	
 	transferQueue->submitAndWait(transferQueue->getCmdBuffer());
-	
-	transferQueue->getCmdBuffer()->reset();
 }
 
 void VKLBuffer::uploadData(const VKLQueue* transferQueue, void* data, size_t size, size_t offset) {
-	VKLBufferCreateInfo tempBufferCreateInfo;
-	
-	LOG_INFO("Creating temp buffer for upload");
+	VKLBuffer tempStageBuffer(
+		VKLBufferCreateInfo()
+		.device(m_device)
+		.size(size)
+		.usageVMA(VMA_MEMORY_USAGE_AUTO_PREFER_HOST)
+		.flagsVMA(VMA_ALLOCATION_CREATE_HOST_ACCESS_SEQUENTIAL_WRITE_BIT)
+		.usage(VK_BUFFER_USAGE_TRANSFER_SRC_BIT)
+	);
 
-	tempBufferCreateInfo.device(m_device).size(size)
-						.memoryProperties(VK_MEMORY_PROPERTY_HOST_COHERENT_BIT | VK_MEMORY_PROPERTY_HOST_VISIBLE_BIT)
-						.usage(VK_BUFFER_USAGE_TRANSFER_SRC_BIT);
+	tempStageBuffer.setData(data, size, 0);
 	
+	VkBufferCopy bufferCopy;
+	bufferCopy.size = size;
+	bufferCopy.dstOffset = offset;
+	bufferCopy.srcOffset = 0;
 
-	VKLBuffer tempStageBuffer(tempBufferCreateInfo);
-
-	VKLAllocation allocation;
-	allocation.memory = m_device->allocateMemory(tempStageBuffer.memoryRequirements(), 
-													VK_MEMORY_PROPERTY_HOST_COHERENT_BIT | VK_MEMORY_PROPERTY_HOST_VISIBLE_BIT);
-	allocation.offset = 0;
-	allocation.size = tempStageBuffer.memoryRequirements().size;
-
-	tempStageBuffer.bind(allocation);
+	this->copyFrom(&tempStageBuffer, transferQueue, bufferCopy);
 	
-	LOG_INFO("Uploading data through temp buffer");
-
-	setData(transferQueue, &tempStageBuffer, data, size, offset);
-
-	LOG_INFO("Destroying temp buffer...");
-
 	tempStageBuffer.destroy();
-
-	m_device->vk.FreeMemory(m_device->handle(), allocation.memory, m_device->allocationCallbacks());
 }
 
 void VKLBuffer::downloadData(const VKLQueue* transferQueue, void* data, size_t size, size_t offset) {
-	VKLBufferCreateInfo tempBufferCreateInfo;
-	tempBufferCreateInfo.device(m_device).size(size)
-						.memoryProperties(VK_MEMORY_PROPERTY_HOST_COHERENT_BIT | VK_MEMORY_PROPERTY_HOST_VISIBLE_BIT)
-						.usage(VK_BUFFER_USAGE_TRANSFER_DST_BIT);
-	
-	VKLBuffer tempStageBuffer(tempBufferCreateInfo);
-
-	VKLAllocation allocation;
-	allocation.memory = m_device->allocateMemory(tempStageBuffer.memoryRequirements(), 
-													VK_MEMORY_PROPERTY_HOST_COHERENT_BIT | VK_MEMORY_PROPERTY_HOST_VISIBLE_BIT);
-	allocation.offset = 0;
-	allocation.size = tempStageBuffer.memoryRequirements().size;
-	
-	tempStageBuffer.bind(allocation);
+	VKLBuffer tempStageBuffer(
+		VKLBufferCreateInfo()
+		.device(m_device)
+		.size(size)
+		.usageVMA(VMA_MEMORY_USAGE_AUTO_PREFER_HOST)
+		.flagsVMA(VMA_ALLOCATION_CREATE_HOST_ACCESS_RANDOM_BIT)
+		.usage(VK_BUFFER_USAGE_TRANSFER_DST_BIT)
+	);
+
+	VkBufferCopy bufferCopy;
+	bufferCopy.size = size;
+	bufferCopy.dstOffset = 0;
+	bufferCopy.srcOffset = offset;
 	
-	getData(transferQueue, &tempStageBuffer, data, size, offset);
+	tempStageBuffer.copyFrom(this, transferQueue, bufferCopy);	
+	tempStageBuffer.getData(data, size, 0);
 	
 	tempStageBuffer.destroy();
-
-	m_device->vk.FreeMemory(m_device->handle(), allocation.memory, m_device->allocationCallbacks());
 }
 
 void VKLBuffer::_create(const VKLBufferCreateInfo& createInfo) {
 	m_device = createInfo.m_device;
-	
-	VK_CALL(m_device->vk.CreateBuffer(m_device->handle(), &createInfo.m_bufferCreateInfo, m_device->allocationCallbacks(), &m_handle));
-	
+
+	if(createInfo.useVMAFlag) {
+		VmaAllocationCreateInfo vmaAllocationCreateInfo = {};
+		vmaAllocationCreateInfo.flags = createInfo.flagsVMAFlag;
+		vmaAllocationCreateInfo.usage = createInfo.usageVMAFlag;
+		vmaAllocationCreateInfo.pUserData = &m_allocation;
+
+		VK_CALL(vmaCreateBuffer(m_device->allocatorVMA() , &createInfo.m_bufferCreateInfo, &vmaAllocationCreateInfo, &m_handle, &m_allocation.vma_allocation, &m_allocation.vma_allocation_info));
+
+		m_allocation.vma_enabled = 1;
+	} else {
+		VK_CALL(m_device->vk.CreateBuffer(m_device->handle(), &createInfo.m_bufferCreateInfo, m_device->allocationCallbacks(), &m_handle));
+		m_allocation.vma_enabled = 0;
+	}
+
 	m_memoryBarrier.buffer = m_handle;
 	m_memoryBarrier.size = createInfo.m_bufferCreateInfo.size;
+
+	m_allocation.buffer = this;
 }
 
 void VKLBuffer::bind(VKLAllocation allocation) {
+	if(m_allocation.vma_enabled) {
+		LOG_ERROR("Cannot bind memory for VMA buffer");
+		return;
+	}
+
 	LOG_INFO("Binding buffer to memory: %d, %d, %d", allocation.memory, allocation.offset, allocation.size);
 
-	m_allocation = allocation;
+	m_allocation.memory = allocation.memory;
+	m_allocation.offset = allocation.offset;
+	m_allocation.size = allocation.size;
 
 	VK_CALL(m_device->vk.BindBufferMemory(m_device->handle(), m_handle, m_allocation.memory, m_allocation.offset));
 }
 
 void VKLBuffer::_destroy() {
-	m_device->vk.DestroyBuffer(m_device->handle(), m_handle, m_device->allocationCallbacks());
+	if(m_allocation.vma_enabled)
+		vmaDestroyBuffer(m_device->allocatorVMA(), m_handle, m_allocation.vma_allocation);
+	else
+		m_device->vk.DestroyBuffer(m_device->handle(), m_handle, m_device->allocationCallbacks());
 }
 
 VKLBufferCreateInfo::VKLBufferCreateInfo() {
 	m_device = NULL;
 	
 	memset(&m_bufferCreateInfo, 0, sizeof(VkBufferCreateInfo));
 	m_bufferCreateInfo.sType = VK_STRUCTURE_TYPE_BUFFER_CREATE_INFO;
@@ -192,17 +184,17 @@
 	m_bufferCreateInfo.flags = 0;
 	m_bufferCreateInfo.usage = 0;
 	m_bufferCreateInfo.size = 0;
 	m_bufferCreateInfo.sharingMode = VK_SHARING_MODE_EXCLUSIVE;
 	m_bufferCreateInfo.queueFamilyIndexCount = 0;
 	m_bufferCreateInfo.pQueueFamilyIndices = NULL;
 
-	m_memoryProperties = VK_MEMORY_PROPERTY_DEVICE_LOCAL_BIT;
-
-	m_allocationPNext = NULL;
+	useVMAFlag = true;
+	usageVMAFlag = VMA_MEMORY_USAGE_AUTO_PREFER_DEVICE;
+	flagsVMAFlag = 0;
 }
 
 VKLBufferCreateInfo& VKLBufferCreateInfo::pNext(void* pNext) {
 	m_bufferCreateInfo.pNext = pNext;
 	
 	return invalidate();
 }
@@ -221,23 +213,35 @@
 
 VKLBufferCreateInfo& VKLBufferCreateInfo::usage(VkBufferUsageFlags usage) {
 	m_bufferCreateInfo.usage = usage;
 	
 	return invalidate();
 }
 
-VKLBufferCreateInfo& VKLBufferCreateInfo::allocationPNext(void* pNext) {
-	m_allocationPNext = pNext;
+VKLBufferCreateInfo& VKLBufferCreateInfo::useVMA(bool useVMA) {
+	useVMAFlag = useVMA;
 	
 	return invalidate();
 }
+
+VKLBufferCreateInfo& VKLBufferCreateInfo::usageVMA(VmaMemoryUsage usage) {
+	usageVMAFlag = usage;
 	
-VKLBufferCreateInfo& VKLBufferCreateInfo::memoryProperties(VkMemoryPropertyFlags memoryProperties) {
-	m_memoryProperties = memoryProperties;
+	return invalidate();
+}
 
+VKLBufferCreateInfo& VKLBufferCreateInfo::flagsVMA(VmaAllocationCreateFlags flags) {
+	flagsVMAFlag = flags;
+	
+	return invalidate();
+}
+
+VKLBufferCreateInfo& VKLBufferCreateInfo::memoryProperties(VkMemoryPropertyFlags memoryProperties) {
+	m_bufferCreateInfo.usage = memoryProperties;
+	
 	return invalidate();
 }
 
 bool VKLBufferCreateInfo::_validate() {
 	if(m_device == NULL) {
 		printf("VKL Validation Error: VKLBufferCreateInfo::device is not set!\n");
 		return false;
```

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLCommandBuffer.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLCommandBuffer.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include <VKL/VKL.h>
 
-VKLCommandBuffer::VKLCommandBuffer(const VKLQueue* queue) {
+VKLCommandBuffer::VKLCommandBuffer(const VKLQueue* queue, int count) {
 	m_queue = queue;
 	m_device = queue->device();
 	
 	VkCommandPoolCreateInfo commandPoolCreateInfo;
 	commandPoolCreateInfo.sType = VK_STRUCTURE_TYPE_COMMAND_POOL_CREATE_INFO;
 	commandPoolCreateInfo.pNext = NULL;
 	commandPoolCreateInfo.flags = VK_COMMAND_POOL_CREATE_RESET_COMMAND_BUFFER_BIT;
@@ -13,53 +13,78 @@
 	VK_CALL(m_device->vk.CreateCommandPool(m_device->handle(), &commandPoolCreateInfo, m_device->allocationCallbacks(), &m_pool));
 	
 	VkCommandBufferAllocateInfo commandBufferAllocationInfo;
 	commandBufferAllocationInfo.sType = VK_STRUCTURE_TYPE_COMMAND_BUFFER_ALLOCATE_INFO;
 	commandBufferAllocationInfo.pNext = NULL;
 	commandBufferAllocationInfo.commandPool = m_pool;
 	commandBufferAllocationInfo.level = VK_COMMAND_BUFFER_LEVEL_PRIMARY;
-	commandBufferAllocationInfo.commandBufferCount = 1;
+	commandBufferAllocationInfo.commandBufferCount = count;
 
-	VK_CALL(m_device->vk.AllocateCommandBuffers(m_device->handle(), &commandBufferAllocationInfo, &m_handle));
+	m_count = count;
+	m_handles = (VkCommandBuffer*)malloc(sizeof(VkCommandBuffer) * count);
+	m_current_index = 0;
+
+	VK_CALL(m_device->vk.AllocateCommandBuffers(m_device->handle(), &commandBufferAllocationInfo, m_handles));
+
+	m_fences = (VkFence*)malloc(sizeof(VkFence) * count);
+
+	for (int i = 0; i < count; i++) {
+		m_fences[i] = m_device->createFence(VK_FENCE_CREATE_SIGNALED_BIT);
+	}
 }
 
 VkCommandPool VKLCommandBuffer::pool() const {
 	return m_pool;
 }
 
+VkCommandPool* VKLCommandBuffer::pPool() const {
+	return (VkCommandPool*)&m_pool;
+}
+
+VkFence VKLCommandBuffer::fence() const {
+	return m_fences[m_current_index];
+}
+
+VkFence* VKLCommandBuffer::pFence() const {
+	return (VkFence*)&m_fences[m_current_index];
+}
+
 void VKLCommandBuffer::bufferBarrier(VKLBuffer* buffer, VkPipelineStageFlags srcStageMask, VkPipelineStageFlags dstStageMask) const {
 	m_device->vk.CmdPipelineBarrier(m_handle, srcStageMask, dstStageMask, 0, 0, NULL, 1, buffer->getMemoryBarrier(), 0, NULL);
 }
 
 void VKLCommandBuffer::copyBuffer(const VKLBuffer* dst, const VKLBuffer* src, VkBufferCopy bufferCopy) const {
 	m_device->vk.CmdCopyBuffer(m_handle, src->handle(), dst->handle(), 1, &bufferCopy);
 }
 
 void VKLCommandBuffer::copyImage(const VKLImage* dst, const VKLImage* src, VkImageCopy imageCopy) const {
 	m_device->vk.CmdCopyImage(m_handle, src->handle(), src->layout(), dst->handle(), dst->layout(), 1, &imageCopy);
 }
 
 void VKLCommandBuffer::begin() const {
+	*((int*)&m_current_index) = (m_current_index + 1) % m_count;
+
+	m_device->waitForFence(m_fences[m_current_index]);
+	m_device->resetFence(m_fences[m_current_index]);
+
+	*((VkCommandBuffer*)&m_handle) = m_handles[m_current_index];
+	
 	VkCommandBufferBeginInfo beginInfo;
 	beginInfo.sType = VK_STRUCTURE_TYPE_COMMAND_BUFFER_BEGIN_INFO;
 	beginInfo.pNext = NULL;
 	beginInfo.flags = 0;
 	beginInfo.pInheritanceInfo = NULL;
 
 	m_device->vk.BeginCommandBuffer(m_handle, &beginInfo);
 }
 
 void VKLCommandBuffer::end() const {
 	m_device->vk.EndCommandBuffer(m_handle);
 }
 
-void VKLCommandBuffer::reset() const {
-	//m_device->vk.ResetCommandBuffer(m_handle, VK_COMMAND_BUFFER_RESET_RELEASE_RESOURCES_BIT);
-}
-
 void VKLCommandBuffer::beginRenderPass(const VKLFramebuffer& framebuffer, VkSubpassContents contents) const  {
 	beginRenderPass(&framebuffer, contents);
 }
 
 void VKLCommandBuffer::beginRenderPass(const VKLFramebuffer& framebuffer, VkSubpassContents contents, VkRect2D area) const {
 	beginRenderPass(&framebuffer, contents, area);
 }
@@ -168,10 +193,10 @@
 }
 
 void VKLCommandBuffer::dispatch(uint32_t x, uint32_t y, uint32_t z) const {
 	m_device->vk.CmdDispatch(m_handle, x, y, z);
 }
 
 void VKLCommandBuffer::destroy() {
-	m_device->vk.FreeCommandBuffers(m_device->handle(), m_pool, 1, &m_handle);
+	m_device->vk.FreeCommandBuffers(m_device->handle(), m_pool, m_count, m_handles);
 	m_device->vk.DestroyCommandPool(m_device->handle(), m_pool, m_device->allocationCallbacks());
 }
```

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLDescriptorSet.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLDescriptorSet.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLDevice.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLDevice.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,29 @@
 
 	memset(&vk, 0, sizeof(VKLDevicePFNS));
 
 	create(createInfo);
 }
 
 void VKLDevice::_create(const VKLDeviceCreateInfo& createInfo) {
+	LOG_INFO("Creating device");
+	
 	m_instance = createInfo.m_instance;
 	m_physicalDevice = createInfo.m_physicalDevice;
 	m_allocationCallbacks = m_instance->allocationCallbacks();
 
 	vk.CreateDevice = (PFN_vkCreateDevice)m_instance->procAddr("vkCreateDevice");
 	vk.GetDeviceProcAddr = (PFN_vkGetDeviceProcAddr)m_instance->procAddr("vkGetDeviceProcAddr");
 
+	LOG_INFO("Calling vkCreateDevice");
+
 	VK_CALL(vk.CreateDevice(m_physicalDevice->handle(), &createInfo.m_createInfo, m_instance->allocationCallbacks(), &m_handle));
 
+	LOG_INFO("Device created");
+
 	vk.DestroyDevice = (PFN_vkDestroyDevice)procAddr("vkDestroyDevice");
 	vk.GetDeviceQueue = (PFN_vkGetDeviceQueue)procAddr("vkGetDeviceQueue");
 	vk.QueueSubmit = (PFN_vkQueueSubmit)procAddr("vkQueueSubmit");
 	vk.QueueWaitIdle = (PFN_vkQueueWaitIdle)procAddr("vkQueueWaitIdle");
 	vk.DeviceWaitIdle = (PFN_vkDeviceWaitIdle)procAddr("vkDeviceWaitIdle");
 	vk.AllocateMemory = (PFN_vkAllocateMemory)procAddr("vkAllocateMemory");
 	vk.FreeMemory = (PFN_vkFreeMemory)procAddr("vkFreeMemory");
@@ -156,44 +162,69 @@
 	vk.GetSwapchainImagesKHR = (PFN_vkGetSwapchainImagesKHR)procAddr("vkGetSwapchainImagesKHR");
 	vk.AcquireNextImageKHR = (PFN_vkAcquireNextImageKHR)procAddr("vkAcquireNextImageKHR");
 	vk.QueuePresentKHR = (PFN_vkQueuePresentKHR)procAddr("vkQueuePresentKHR");
 
 	vk.GetMemoryFdKHR = (PFN_vkGetMemoryFdKHR)procAddr("vkGetMemoryFdKHR");
 	vk.GetSemaphoreFdKHR = (PFN_vkGetSemaphoreFdKHR)procAddr("vkGetSemaphoreFdKHR");
 
+	LOG_INFO("Device functions loaded");
+
 	uint32_t* queueFamilyCurrentIndicies = (uint32_t*)malloc(sizeof(uint32_t) * physical()->getQueueFamilyProperties().size());
 	memset(queueFamilyCurrentIndicies, 0, sizeof(uint32_t) * physical()->getQueueFamilyProperties().size());
 	
-	for(int i = 0; i < 4; i++) {
+	for(int i = 0; i < VKL_QUEUE_TYPE_COUNT; i++) {
 		for(int j = 0; j < createInfo.m_queueTypeIndicies[i].size(); j++) {
 			VKLQueueLocation queueLocation = createInfo.m_queueTypeIndicies[i][j];
 			
-			VkQueue queue;
+			VkQueue queue = VK_NULL_HANDLE;
 			vk.GetDeviceQueue(m_handle, queueLocation.familyIndex, queueLocation.localIndex, &queue);
+
+			LOG_INFO("Created queue: %d %d %p", queueLocation.familyIndex, queueLocation.localIndex, queue);
 			
 			m_queues[i].push_back(VKLQueue());
 			m_queues[i].back().init(this, queue, queueLocation.familyIndex);
 		}
 	}
 	
 	free(queueFamilyCurrentIndicies);
+
+	LOG_INFO("Queues created");
+
+	VmaVulkanFunctions vmaVulkanFunctions = {};
+	vmaVulkanFunctions.vkGetInstanceProcAddr = vkGetInstanceProcAddr;
+	vmaVulkanFunctions.vkGetDeviceProcAddr = vkGetDeviceProcAddr;
+
+	VmaAllocatorCreateInfo allocatorCreateInfo = {};
+	allocatorCreateInfo.vulkanApiVersion = VK_API_VERSION_1_2;
+	allocatorCreateInfo.physicalDevice = m_physicalDevice->handle();
+	allocatorCreateInfo.device = m_handle;
+	allocatorCreateInfo.instance = m_instance->handle();
+	allocatorCreateInfo.pVulkanFunctions = &vmaVulkanFunctions;
+	
+	VK_CALL(vmaCreateAllocator(&allocatorCreateInfo, &m_allocator));
+
+	LOG_INFO("Allocator created");
 }
 
 const VkAllocationCallbacks* VKLDevice::allocationCallbacks() const {
 	return m_allocationCallbacks;
 }
 
 PFN_vkVoidFunction VKLDevice::procAddr(const char* name) const {
 	return vk.GetDeviceProcAddr(m_handle, name);
 }
 
 const VKLPhysicalDevice* VKLDevice::physical() const {
 	return m_physicalDevice;
 }
 
+const VmaAllocator& VKLDevice::allocatorVMA() const {
+	return m_allocator;
+}
+
 const VKLQueue* VKLDevice::getQueue(VKLQueueType type, uint32_t queueIndex) const {
 	return &m_queues[type][queueIndex];
 }
 
 VkFence VKLDevice::createFence(VkFenceCreateFlags flags) const {
 	VkFenceCreateInfo fenceCreateInfo;
 	fenceCreateInfo.sType = VK_STRUCTURE_TYPE_FENCE_CREATE_INFO;
@@ -261,61 +292,66 @@
 	VkDeviceMemory memory;
 	VK_CALL(vk.AllocateMemory(m_handle, &memoryAllocateInfo, m_allocationCallbacks, &memory));
 
 	return memory;
 }
 
 void VKLDevice::_destroy() {
-	for (int i = 0; i < 3; i++) {
+	for (int i = 0; i < VKL_QUEUE_TYPE_COUNT; i++) {
 		for (int j = 0; j < m_queues[i].size(); j++) {
 			m_queues[i][j].destroy();
 		}
 	}
 
+	vmaDestroyAllocator(m_allocator);
 	vk.DestroyDevice(m_handle, allocationCallbacks());
 }
 
 VKLDeviceCreateInfo::VKLDeviceCreateInfo() {
 	m_physicalDevice = NULL;
 	m_instance = NULL;
 	
 	m_queueTypeCounts[0] = 0;
 	m_queueTypeCounts[1] = 0;
 	m_queueTypeCounts[2] = 0;
 	m_queueTypeCounts[3] = 0;
 	
-	memset(&m_features, 0, sizeof(VkPhysicalDeviceFeatures));
+	memset(&m_features, 0, sizeof(VkPhysicalDeviceFeatures2));
 	memset(&m_createInfo, 0, sizeof(VkDeviceCreateInfo));
 	
 	m_createInfo.sType = VK_STRUCTURE_TYPE_DEVICE_CREATE_INFO;
 	m_createInfo.pNext = NULL;
 	m_createInfo.flags = 0;
-	m_createInfo.pEnabledFeatures = &m_features;
+	m_createInfo.pEnabledFeatures = NULL;
 }
 
 VKLDeviceCreateInfo& VKLDeviceCreateInfo::physicalDevice(const VKLPhysicalDevice* physicalDevice) {
 	m_physicalDevice = physicalDevice;
 	
 	m_instance = physicalDevice->instance();
 	
-	m_features = physicalDevice->getFeatures();
+	m_features = physicalDevice->getFeatures2();
 	
 	m_createInfo.enabledLayerCount = m_instance->getLayers().size();
 	m_createInfo.ppEnabledLayerNames = m_instance->getLayers().data();
+
+	m_createInfo.pNext = &m_features;
 	
 	return invalidate();
 }
 
 VKLDeviceCreateInfo& VKLDeviceCreateInfo::queueTypeCount(VKLQueueType type, uint32_t count) {
 	m_queueTypeCounts[type] = count;
 	
 	return invalidate();
 }
 
 VKLDeviceCreateInfo& VKLDeviceCreateInfo::addExtension(const char* extension) {
+	LOG_INFO("Adding extension %s", extension);
+
 	m_extensions.push_back(extension);
 	
 	m_createInfo.enabledExtensionCount = m_extensions.size();
 	m_createInfo.ppEnabledExtensionNames = m_extensions.data();
 	
 	return invalidate();
 }
@@ -366,18 +402,20 @@
 		printf("\n");
 	}	
 }
 
 bool VKLDeviceCreateInfo::_supportsExtension(const char* extension) {
 	for (int i = 0; i < m_physicalDevice->getExtensions().size(); i++) {
 		if (strcmp(m_physicalDevice->getExtensions()[i].extensionName, extension) == 0) {
+			LOG_INFO("Extension %s supported", extension);
 			return true;
 		}
 	}
 
+	LOG_INFO("Extension %s unsupported", extension);
 	return false;
 }
 
 bool VKLDeviceCreateInfo::_supportsLayer(const char* layer) {
 	return true;
 }
 
@@ -473,14 +511,24 @@
 	}
 #endif
 
 	if (_supportsExtension("VK_KHR_portability_subset")) {
 		addExtension("VK_KHR_portability_subset");
 	}
 
+	if(_supportsExtension("VK_KHR_shader_non_semantic_info")) {
+		addExtension("VK_KHR_shader_non_semantic_info");
+	}
+
+	if(_supportsExtension("VK_EXT_shader_atomic_float")) {
+		addExtension("VK_EXT_shader_atomic_float");
+	}
+
+	
+
 	//_printSelections();
 	
 	m_queueCreateInfos.clear();
 	m_queueTypeIndicies[0].clear();
 	m_queueTypeIndicies[1].clear();
 	m_queueTypeIndicies[2].clear();
 	m_queueTypeIndicies[3].clear();
```

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLFramebuffer.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLFramebuffer.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLImage.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLImage.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -17,30 +17,51 @@
 	_create(createInfo, (VkImage)VK_NULL_HANDLE);
 }
 
 void VKLImage::_create(const VKLImageCreateInfo& createInfo, VkImage handle) {
 	m_device = createInfo.m_device;
 	m_format = createInfo.m_imageCreateInfo.format;
 	m_size = createInfo.m_imageCreateInfo.extent;
-	m_layers = createInfo.m_imageCreateInfo.arrayLayers;	
+	m_layers = createInfo.m_imageCreateInfo.arrayLayers;
 	
 	if(handle == VK_NULL_HANDLE) {
-		VK_CALL(m_device->vk.CreateImage(m_device->handle(), &createInfo.m_imageCreateInfo, m_device->allocationCallbacks(), &m_handle));
+		if(createInfo.useVMAFlag) {
+			VmaAllocationCreateInfo vmaAllocationCreateInfo = {};
+			vmaAllocationCreateInfo.flags = createInfo.flagsVMAFlag;
+			vmaAllocationCreateInfo.usage = createInfo.usageVMAFlag;
+			vmaAllocationCreateInfo.pUserData = &m_allocation;
+			
+			VK_CALL(vmaCreateImage(m_device->allocatorVMA(), &createInfo.m_imageCreateInfo, &vmaAllocationCreateInfo, &m_handle, &m_allocation.vma_allocation, &m_allocation.vma_allocation_info));
+			
+			m_allocation.vma_enabled = 1;
+		} else {
+			VK_CALL(m_device->vk.CreateImage(m_device->handle(), &createInfo.m_imageCreateInfo, m_device->allocationCallbacks(), &m_handle));
+
+			m_allocation.vma_enabled = 0;
+		}		
 
 		m_memoryBarrier.oldLayout = createInfo.m_imageCreateInfo.initialLayout;
 	} else {
 		m_handle = handle;
 
 		initBarrier(createInfo.m_imageCreateInfo.initialLayout);
 	}
 }
 
-
 void VKLImage::bind(VKLAllocation allocation) {
-	m_allocation = allocation;
+	if(m_allocation.vma_enabled) {
+		LOG_ERROR("Cannot bind memory for VMA image");
+		return;
+	}
+
+		LOG_INFO("Binding image to memory: %d, %d, %d", allocation.memory, allocation.offset, allocation.size);
+
+	m_allocation.memory = allocation.memory;
+	m_allocation.offset = allocation.offset;
+	m_allocation.size = allocation.size;
 	
 	VK_CALL(m_device->vk.BindImageMemory(m_device->handle(), m_handle, m_allocation.memory, m_allocation.offset));	
 	
 	initBarrier(m_memoryBarrier.oldLayout);
 }
 
 void VKLImage::initBarrier(VkImageLayout layout) {
@@ -102,27 +123,25 @@
 }
 
 void VKLImage::transition(const VKLQueue* queue, VkAccessFlags accessMask, VkImageLayout layout, VkPipelineStageFlags srcStageMask, VkPipelineStageFlags dstStageMask) {
 	queue->getCmdBuffer()->begin();
 	cmdTransitionBarrier(queue->getCmdBuffer(), accessMask, layout, srcStageMask, dstStageMask);
 	queue->getCmdBuffer()->end();
 	queue->submitAndWait(queue->getCmdBuffer());
-	queue->getCmdBuffer()->reset();
 }
 
 VkFormat VKLImage::format() const {
 	return m_format;
 }
 
 void VKLImage::copyFrom(VKLImage* src, const VKLQueue* transferQueue, VkImageCopy imageCopy) {
 	transferQueue->getCmdBuffer()->begin();
 	transferQueue->getCmdBuffer()->copyImage(this, src, imageCopy);
 	transferQueue->getCmdBuffer()->end();
 	transferQueue->submitAndWait(transferQueue->getCmdBuffer());
-	transferQueue->getCmdBuffer()->reset();	
 }
 
 void VKLImage::setData(void* data, size_t size, size_t pixelSize) {
 	VkImageSubresource subresource;
 	memset(&subresource, 0, sizeof(VkImageSubresource));
 	subresource.aspectMask = VK_IMAGE_ASPECT_COLOR_BIT;
 	subresource.mipLevel = 0;
@@ -190,15 +209,15 @@
 							.device(m_device)
 							.extent(m_size.width, m_size.height, m_size.depth)
 							.format(m_format)
 							.tiling(VK_IMAGE_TILING_LINEAR)
 							.usage(VK_IMAGE_USAGE_TRANSFER_SRC_BIT)
 							.initialLayout(VK_IMAGE_LAYOUT_PREINITIALIZED)
 							.memoryProperties(VK_MEMORY_PROPERTY_HOST_COHERENT_BIT)
-							.arrayLevels(m_layers));
+							.arrayLayers(m_layers));
 	
 	VKLAllocation allocation;
 	allocation.memory = m_device->allocateMemory(stagingImage.memoryRequirements(), 
 													VK_MEMORY_PROPERTY_HOST_COHERENT_BIT | VK_MEMORY_PROPERTY_HOST_VISIBLE_BIT);
 	allocation.offset = 0;
 	allocation.size = stagingImage.memoryRequirements().size;
 
@@ -220,16 +239,14 @@
 									  VK_PIPELINE_STAGE_TRANSFER_BIT, VK_PIPELINE_STAGE_TRANSFER_BIT);
 	
 	transferQueue->getCmdBuffer()->copyImage(this, &stagingImage, imageCopy);
 	transferQueue->getCmdBuffer()->end();
 	
 	transferQueue->submitAndWait(transferQueue->getCmdBuffer());
 	
-	transferQueue->getCmdBuffer()->reset();
-	
 	stagingImage.destroy();
 
 	m_device->vk.FreeMemory(m_device->handle(), allocation.memory, m_device->allocationCallbacks());
 }
 
 
 void VKLImage::uploadDataBuffer(const VKLQueue* transferQueue, void* data, size_t size) {
@@ -273,16 +290,14 @@
 		&bufferImageCopy
 	);
 
 	transferQueue->getCmdBuffer()->end();
 	
 	transferQueue->submitAndWait(transferQueue->getCmdBuffer());
 	
-	transferQueue->getCmdBuffer()->reset();
-	
 	stagingBuffer.destroy();
 	m_device->vk.FreeMemory(m_device->handle(), allocation.memory, m_device->allocationCallbacks());
 }
 
 
 void VKLImage::downloadDataBuffer(const VKLQueue* transferQueue, void* data, size_t size) {
 	VKLBuffer stagingBuffer(VKLBufferCreateInfo()
@@ -323,24 +338,25 @@
 		&bufferImageCopy
 	);
 
 	transferQueue->getCmdBuffer()->end();
 	
 	transferQueue->submitAndWait(transferQueue->getCmdBuffer());
 	
-	transferQueue->getCmdBuffer()->reset();
-
 	stagingBuffer.getData(data, size, 0);
 	
 	stagingBuffer.destroy();
 	m_device->vk.FreeMemory(m_device->handle(), allocation.memory, m_device->allocationCallbacks());
 }
 
 void VKLImage::_destroy() {
-	m_device->vk.DestroyImage(m_device->handle(), m_handle, m_device->allocationCallbacks());
+	if(m_allocation.vma_enabled)
+		vmaDestroyImage(m_device->allocatorVMA(), m_handle, m_allocation.vma_allocation);
+	else
+		m_device->vk.DestroyImage(m_device->handle(), m_handle, m_device->allocationCallbacks());
 }
 
 VKLImageCreateInfo::VKLImageCreateInfo() {
 	memset(&m_imageCreateInfo, 0, sizeof(VkImageCreateInfo));
 	m_imageCreateInfo.sType = VK_STRUCTURE_TYPE_IMAGE_CREATE_INFO;
 	m_imageCreateInfo.pNext = NULL;
 	m_imageCreateInfo.flags = 0;
@@ -353,14 +369,18 @@
 	m_imageCreateInfo.sharingMode = VK_SHARING_MODE_EXCLUSIVE;
 	m_imageCreateInfo.initialLayout = VK_IMAGE_LAYOUT_UNDEFINED;
 
 	m_memoryProperties = VK_MEMORY_PROPERTY_DEVICE_LOCAL_BIT;
 
 	m_allocationPNext = NULL;
 
+	useVMAFlag = true;
+	usageVMAFlag = VMA_MEMORY_USAGE_AUTO_PREFER_DEVICE;
+	flagsVMAFlag = 0;
+
 	LOG_INFO("Init VKLImageCreateInfo");
 }
 
 VKLImageCreateInfo& VKLImageCreateInfo::device(const VKLDevice* device) {
 	LOG_INFO("VKLImageCreateInfo::device");
 
 	m_device = device;
@@ -419,26 +439,44 @@
 
 VKLImageCreateInfo& VKLImageCreateInfo::initialLayout(VkImageLayout layout) {
 	m_imageCreateInfo.initialLayout = layout;
 	
 	return invalidate();
 }
 
-VKLImageCreateInfo& VKLImageCreateInfo::arrayLevels(uint32_t arrayLevels) {
-	m_imageCreateInfo.arrayLayers = arrayLevels;
+VKLImageCreateInfo& VKLImageCreateInfo::arrayLayers(uint32_t arrayLayers) {
+	m_imageCreateInfo.arrayLayers = arrayLayers;
 	
 	return invalidate();
 }
 
 VKLImageCreateInfo& VKLImageCreateInfo::memoryProperties(VkMemoryPropertyFlags memoryProperties) {
 	m_memoryProperties = memoryProperties;
 
 	return invalidate();
 }
 
+VKLImageCreateInfo& VKLImageCreateInfo::useVMA(bool useVMA) {
+	useVMAFlag = useVMA;
+	
+	return invalidate();
+}
+
+VKLImageCreateInfo& VKLImageCreateInfo::usageVMA(VmaMemoryUsage usage) {
+	usageVMAFlag = usage;
+	
+	return invalidate();
+}
+
+VKLImageCreateInfo& VKLImageCreateInfo::flagsVMA(VmaAllocationCreateFlags flags) {
+	flagsVMAFlag = flags;
+	
+	return invalidate();
+}
+
 bool VKLImageCreateInfo::_validate() {
 	if(m_device == NULL) {
 		printf("VKL Validation Error: VKLImageCreateInfo::device is not set!\n");
 		return false;
 	}
 	
 	if (m_imageCreateInfo.extent.width == 0 || m_imageCreateInfo.extent.height == 0 || m_imageCreateInfo.extent.depth == 0) {
```

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLImageView.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLImageView.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLPipeline.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLPipeline.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLPipelineLayout.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLPipelineLayout.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #include <VKL/VKL.h>
 
 #include <glslang/Public/resource_limits_c.h>
+//#include <spirv-tools/libspirv.hpp>
 
 VKLPipelineLayout::VKLPipelineLayout() : VKLCreator<VKLPipelineLayoutCreateInfo>("VKLPipelineLayout") {
 	
 }
 
 VKLPipelineLayout::VKLPipelineLayout(const VKLPipelineLayoutCreateInfo& createInfo) : VKLCreator<VKLPipelineLayoutCreateInfo>("VKLPipelineLayout") {
 	this->create(createInfo);
@@ -147,15 +148,15 @@
 uint32_t* util_compile_shader_code(glslang_stage_t stage, size_t* size, const char* shader_source, const char* shader_name) {
     glslang_input_t input = {};
 	input.language = GLSLANG_SOURCE_GLSL;
 	input.stage = stage;
 	input.client = GLSLANG_CLIENT_VULKAN;
 	input.client_version = GLSLANG_TARGET_VULKAN_1_2;
 	input.target_language = GLSLANG_TARGET_SPV;
-	input.target_language_version = GLSLANG_TARGET_SPV_1_0;
+	input.target_language_version = GLSLANG_TARGET_SPV_1_3;
 	input.code = shader_source;
 	input.default_version = 100;
 	input.default_profile = GLSLANG_NO_PROFILE;
 	input.force_default_version_and_profile = false;
 	input.forward_compatible = false;
 	input.messages = GLSLANG_MSG_DEFAULT_BIT;
 	input.resource = glslang_default_resource();
@@ -191,18 +192,47 @@
         glslang_shader_delete(shader);
         return NULL;
     }
 
     glslang_program_SPIRV_generate(program, stage);
 
     *size = glslang_program_SPIRV_get_size(program) * sizeof(uint32_t);
-    
+
     uint32_t* words = (uint32_t*)malloc(*size);
     glslang_program_SPIRV_get(program, words);
 
+/*
+	size_t table_width = 4;
+
+	int word_index = 0;
+	char word_buffs[2][256];
+	memset(word_buffs, 0, sizeof(word_buffs));
+
+	char text_buff[table_width * 4 + 1];
+	text_buff[table_width * 4] = 0;
+	for (size_t i = 0; i < *size / sizeof(uint32_t); i += table_width) {
+		memset(word_buffs, 0, sizeof(word_buffs));
+		memcpy(text_buff, &words[i], 4 * table_width);
+
+		for(size_t j = 0; j < table_width * 4; j++) {
+			if(text_buff[j] < 32 || text_buff[j] > 126) {
+				text_buff[j] = '.';
+			}
+		}
+
+		for(size_t j = 0; j < table_width; j++) {
+			word_index = (word_index + 1) % 2;
+			sprintf(word_buffs[word_index], "%s%08x ", word_buffs[(word_index + 1) % 2], words[i + j]);
+		}
+		
+
+		LOG_INFO("%04d %s%s", i, word_buffs[word_index], text_buff);
+	}
+	*/
+
     const char* spirv_messages = glslang_program_SPIRV_get_messages(program);
     if (spirv_messages)
         LOG_ERROR("(%s) %s\b", shader_name, spirv_messages);
 
     glslang_program_delete(program);
     glslang_shader_delete(shader);
```

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLQueue.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLQueue.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -7,73 +7,62 @@
 }
 
 void VKLQueue::init(const VKLDevice* device, VkQueue queue, uint32_t familyIndex) {
 	m_handle = queue;
 	m_device = device;
 	m_familyIndex = familyIndex;
 	
-	m_fence = m_device->createFence(0);
-	
 	m_cmdBuffer = new VKLCommandBuffer(this);
 }
 
 const VKLDevice* VKLQueue::device() const {
 	return m_device;
 }
 
-VkFence VKLQueue::fence() const {
-	return m_fence;
-}
-
 VKLCommandBuffer* VKLQueue::getCmdBuffer() const {
 	return m_cmdBuffer;
 }
 
 uint32_t VKLQueue::getFamilyIndex() const {
 	return m_familyIndex;
 }
 
 void VKLQueue::submitAndWait(const VKLCommandBuffer* cmdBuffer) const {
 	submitAndWait(cmdBuffer, 0, NULL, NULL);
 }
 
 void VKLQueue::submitAndWait(const VKLCommandBuffer* cmdBuffer, uint32_t waitSemaphoreCount, const VkSemaphore* pWaitSemaphores, const VkPipelineStageFlags* pWaitDstStageMask) const {
-	submit(cmdBuffer, m_fence, NULL, waitSemaphoreCount, pWaitSemaphores, pWaitDstStageMask);
-	m_device->waitForFence(m_fence);
-	m_device->resetFence(m_fence);
+	submit(cmdBuffer, NULL, waitSemaphoreCount, pWaitSemaphores, pWaitDstStageMask);
+	m_device->waitForFence(cmdBuffer->fence());
 }
 
-void VKLQueue::submit(const VKLCommandBuffer* cmdBuffer, VkFence fence) const {
-	submit(cmdBuffer, fence, NULL, 0, NULL, NULL);
+void VKLQueue::submit(const VKLCommandBuffer* cmdBuffer) const {
+	submit(cmdBuffer, NULL, 0, NULL, NULL);
 }
 
-void VKLQueue::submit(const VKLCommandBuffer* cmdBuffer, VkFence fence, const VkSemaphore* signalSempahore) const {
-	submit(cmdBuffer, fence, signalSempahore, 0, NULL, NULL);
+void VKLQueue::submit(const VKLCommandBuffer* cmdBuffer, const VkSemaphore* signalSempahore) const {
+	submit(cmdBuffer, signalSempahore, 0, NULL, NULL);
 }
 
-void VKLQueue::submit(const VKLCommandBuffer* cmdBuffer, VkFence fence, const VkSemaphore* signalSempahore, uint32_t waitSemaphoreCount, const VkSemaphore* pWaitSemaphores, const VkPipelineStageFlags* pWaitDstStageMask) const {
-	VkCommandBuffer cmdBuffHandle = cmdBuffer->handle();
-	
+void VKLQueue::submit(const VKLCommandBuffer* cmdBuffer, const VkSemaphore* signalSempahore, uint32_t waitSemaphoreCount, const VkSemaphore* pWaitSemaphores, const VkPipelineStageFlags* pWaitDstStageMask) const {
 	VkSubmitInfo submitInfo;
 	memset(&submitInfo, 0, sizeof(VkSubmitInfo));
 	submitInfo.sType = VK_STRUCTURE_TYPE_SUBMIT_INFO;
 	submitInfo.pNext = NULL;
 	submitInfo.waitSemaphoreCount = waitSemaphoreCount;
 	submitInfo.pWaitSemaphores = pWaitSemaphores;
 	submitInfo.pWaitDstStageMask = pWaitDstStageMask;
 	submitInfo.commandBufferCount = 1;
-	submitInfo.pCommandBuffers = &cmdBuffHandle;
+	submitInfo.pCommandBuffers = cmdBuffer->pHandle();
 	submitInfo.signalSemaphoreCount = signalSempahore == NULL ? 0 : 1;
 	submitInfo.pSignalSemaphores = signalSempahore;
 	
-	VK_CALL(m_device->vk.QueueSubmit(m_handle, 1, &submitInfo, fence));
+	VK_CALL(m_device->vk.QueueSubmit(m_handle, 1, &submitInfo, cmdBuffer->fence()));
 }
 
 void VKLQueue::waitIdle() const {
 	m_device->vk.QueueWaitIdle(m_handle);
 }
 
-
 void VKLQueue::destroy() {
 	m_cmdBuffer->destroy();
-	m_device->destroyFence(m_fence);
 }
```

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLRenderPass.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLRenderPass.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLStaticAllocator.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLStaticAllocator.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLSurface.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLSurface.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 		break;
 	default:
 		break;
 	}
 }
 
 void VKLSurface::_destroy() {
-	m_instance->vk.DestroySurfaceKHR(m_instance->handle(), m_handle, m_instance->allocationCallbacks());
+	vkDestroySurfaceKHR(m_instance->handle(), m_handle, m_instance->allocationCallbacks());
 }
 
 VKLSurfaceCreateInfo::VKLSurfaceCreateInfo() {
 	m_createInfoPtr = NULL;
 	m_type = VKL_SURFACE_CREATE_INFO_TYPE_UNDEFINED;
 	m_instance = NULL;
 }
```

### Comparing `vkdispatch-0.0.3/deps/VKL/src/VKLSwapChain.cpp` & `vkdispatch-0.0.4/deps/VKL/src/VKLSwapChain.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 		m_swapChainImages[i].cmdTransitionBarrier(m_cmdBuffer, VK_ACCESS_TRANSFER_WRITE_BIT, VK_IMAGE_LAYOUT_TRANSFER_DST_OPTIMAL, VK_PIPELINE_STAGE_TRANSFER_BIT, VK_PIPELINE_STAGE_TRANSFER_BIT);
 	}
 
 	free(presentImages);
 	
 	m_cmdBuffer->end();
 	
-	m_queue->submit(m_cmdBuffer, (VkFence)VK_NULL_HANDLE);
+	m_queue->submit(m_cmdBuffer);
 	m_queue->waitIdle();
 	
 	VK_CALL(m_device->vk.AcquireNextImageKHR(m_device->handle(), m_handle, UINT64_MAX, (VkSemaphore)VK_NULL_HANDLE, m_fence, &m_currentImgIndex));
 	
 	m_device->waitForFence(m_fence);
 	m_device->resetFence(m_fence);
 }
@@ -104,15 +104,15 @@
 	m_cmdBuffer->begin();
 	
 	m_device->vk.CmdBlitImage(m_cmdBuffer->handle(), image->handle(), image->layout(), getCurrentImage().handle(), VK_IMAGE_LAYOUT_TRANSFER_DST_OPTIMAL, 1, &imageBlit, VK_FILTER_LINEAR);
 	
 	getCurrentImage().cmdTransitionBarrier(m_cmdBuffer, VK_ACCESS_MEMORY_READ_BIT, VK_IMAGE_LAYOUT_PRESENT_SRC_KHR, VK_PIPELINE_STAGE_TRANSFER_BIT, VK_PIPELINE_STAGE_TRANSFER_BIT);
 	m_cmdBuffer->end();
 	
-	m_queue->submit(m_cmdBuffer, (VkFence)VK_NULL_HANDLE, NULL, waitSemaphoreCount, waitSemaphores, pWaitDstStageMask);
+	m_queue->submit(m_cmdBuffer, NULL, waitSemaphoreCount, waitSemaphores, pWaitDstStageMask);
 	m_queue->waitIdle();
 	
 	VkPresentInfoKHR presentInfo;
 	presentInfo.sType = VK_STRUCTURE_TYPE_PRESENT_INFO_KHR;
 	presentInfo.pNext = NULL;
 	presentInfo.waitSemaphoreCount = 0;
 	presentInfo.pWaitSemaphores = NULL;
@@ -123,15 +123,15 @@
 	
 	VK_CALL(m_device->vk.QueuePresentKHR(m_queue->handle(), &presentInfo));
 	
 	m_cmdBuffer->begin();
 	getCurrentImage().cmdTransitionBarrier(m_cmdBuffer, VK_ACCESS_TRANSFER_WRITE_BIT, VK_IMAGE_LAYOUT_TRANSFER_DST_OPTIMAL, VK_PIPELINE_STAGE_TRANSFER_BIT, VK_PIPELINE_STAGE_TRANSFER_BIT);
 	m_cmdBuffer->end();
 	
-	m_queue->submit(m_cmdBuffer, (VkFence)VK_NULL_HANDLE);
+	m_queue->submit(m_cmdBuffer);
 	m_queue->waitIdle();
 	
 	VK_CALL(m_device->vk.AcquireNextImageKHR(m_device->handle(), m_handle, UINT64_MAX, (VkSemaphore)VK_NULL_HANDLE, m_fence, &m_currentImgIndex));
 	
 	m_device->waitForFence(m_fence);
 	m_device->resetFence(m_fence);
 }
```

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT.h` & `vkdispatch-0.0.4/deps/VkFFT/vkFFT/vkFFT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.3/pyproject.toml` & `vkdispatch-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "Cython",
     "numpy"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vkdispatch"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Shahar Sandhaus", email="shahar.sandhaus@gmail.com" },
 ]
 description = "A Python module for orchestrating and dispatching large computations across multi-GPU systems using Vulkan."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -22,11 +22,12 @@
     "Operating System :: OS Independent",
     "Development Status :: 1 - Planning",
 ]
 dependencies = [
     "setuptools>=61.0",
     "numpy",
 ]
+scripts = { vdlist = 'vkdispatch.__main__:main' }
 
 [project.urls]
 Homepage = "https://github.com/sharhar/vkdispatch"
 Issues = "https://github.com/sharhar/vkdispatch/issues"
```

### Comparing `vkdispatch-0.0.3/vkdispatch.egg-info/PKG-INFO` & `vkdispatch-0.0.4/vkdispatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkdispatch
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python module for orchestrating and dispatching large computations across multi-GPU systems using Vulkan.
 Author-email: Shahar Sandhaus <shahar.sandhaus@gmail.com>
 Project-URL: Homepage, https://github.com/sharhar/vkdispatch
 Project-URL: Issues, https://github.com/sharhar/vkdispatch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

