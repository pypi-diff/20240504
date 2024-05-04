# Comparing `tmp/torch_nos-0.2.0b0-py3-none-any.whl.zip` & `tmp/torch_nos-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,93 +1,89 @@
-Zip file size: 1752491 bytes, number of entries: 91
--rw-r--r--  2.0 unx      424 b- defN 23-Dec-19 22:33 nos/__init__.py
--rw-r--r--  2.0 unx     1951 b- defN 24-Feb-20 17:08 nos/constants.py
--rw-r--r--  2.0 unx      750 b- defN 24-Jan-02 20:35 nos/exceptions.py
--rw-r--r--  2.0 unx     2295 b- defN 23-Dec-19 22:33 nos/logging.py
--rw-r--r--  2.0 unx     3199 b- defN 24-Jan-02 20:35 nos/protoc.py
--rw-r--r--  2.0 unx     1436 b- defN 23-Dec-19 22:33 nos/telemetry.py
--rw-r--r--  2.0 unx       23 b- defN 24-Apr-11 19:14 nos/version.py
--rw-r--r--  2.0 unx     1898 b- defN 24-Feb-20 17:08 nos/catalogs/model_profile_catalog.json
--rw-r--r--  2.0 unx      858 b- defN 24-Jan-16 08:09 nos/cli/cli.py
--rw-r--r--  2.0 unx     1417 b- defN 24-Jan-02 20:35 nos/cli/hub.py
--rw-r--r--  2.0 unx     7330 b- defN 24-Jan-02 20:35 nos/cli/predict.py
--rw-r--r--  2.0 unx    13556 b- defN 24-Apr-11 19:08 nos/cli/profile.py
--rw-r--r--  2.0 unx    19110 b- defN 24-Apr-11 00:42 nos/cli/serve.py
--rw-r--r--  2.0 unx     1838 b- defN 23-Dec-19 22:33 nos/cli/system.py
--rw-r--r--  2.0 unx      425 b- defN 23-May-05 01:05 nos/cli/utils.py
--rw-r--r--  2.0 unx     1836 b- defN 24-Apr-11 19:08 nos/cli/templates/docker-compose.serve.yml.j2
--rw-r--r--  2.0 unx      398 b- defN 24-Jan-02 20:35 nos/client/__init__.py
--rw-r--r--  2.0 unx    30281 b- defN 24-Feb-20 22:10 nos/client/grpc.py
--rw-r--r--  2.0 unx     3094 b- defN 24-Feb-20 17:08 nos/common/__init__.py
--rw-r--r--  2.0 unx      204 b- defN 23-Jun-13 21:50 nos/common/cloudpickle.py
--rw-r--r--  2.0 unx      906 b- defN 24-Jan-02 20:35 nos/common/exceptions.py
--rw-r--r--  2.0 unx     5154 b- defN 23-Sep-02 01:00 nos/common/git.py
--rw-r--r--  2.0 unx     1028 b- defN 24-Jan-02 20:35 nos/common/helpers.py
--rw-r--r--  2.0 unx      499 b- defN 23-Sep-02 01:00 nos/common/metaclass.py
--rw-r--r--  2.0 unx    20811 b- defN 24-Apr-11 19:08 nos/common/profiler.py
--rw-r--r--  2.0 unx      805 b- defN 24-Feb-20 17:08 nos/common/runtime.py
--rw-r--r--  2.0 unx    11842 b- defN 23-Dec-19 22:33 nos/common/shm.py
--rw-r--r--  2.0 unx    31844 b- defN 24-Feb-20 17:08 nos/common/spec.py
--rw-r--r--  2.0 unx     7930 b- defN 24-Jan-02 20:35 nos/common/system.py
--rw-r--r--  2.0 unx      830 b- defN 24-Jan-02 20:35 nos/common/tasks.py
--rw-r--r--  2.0 unx     6117 b- defN 24-Feb-20 17:08 nos/common/types.py
--rw-r--r--  2.0 unx     1465 b- defN 24-Feb-20 17:08 nos/common/io/__init__.py
--rw-r--r--  2.0 unx     1050 b- defN 23-Jun-15 17:56 nos/common/io/video/base.py
--rw-r--r--  2.0 unx     8777 b- defN 23-Dec-19 22:33 nos/common/io/video/opencv.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 21:50 nos/executors/__init__.py
--rw-r--r--  2.0 unx     9283 b- defN 24-Jan-02 20:35 nos/executors/ray.py
--rw-r--r--  2.0 unx     2229 b- defN 23-Dec-04 18:37 nos/externals/streamlink.py
--rw-r--r--  2.0 unx    15315 b- defN 24-Feb-20 17:08 nos/hub/__init__.py
--rw-r--r--  2.0 unx     1756 b- defN 23-Dec-19 22:33 nos/hub/config.py
--rw-r--r--  2.0 unx      538 b- defN 23-Dec-19 22:33 nos/hub/hf.py
--rw-r--r--  2.0 unx       59 b- defN 23-Oct-11 22:45 nos/managers/__init__.py
--rw-r--r--  2.0 unx    24163 b- defN 24-Feb-20 17:08 nos/managers/model.py
--rw-r--r--  2.0 unx     4738 b- defN 24-Jan-02 20:35 nos/managers/pool.py
--rw-r--r--  2.0 unx      936 b- defN 24-Feb-20 17:08 nos/models/__init__.py
--rw-r--r--  2.0 unx     3138 b- defN 24-Jan-02 20:35 nos/models/_noop.py
--rw-r--r--  2.0 unx     3841 b- defN 23-Dec-19 22:33 nos/models/blip.py
--rw-r--r--  2.0 unx     4220 b- defN 23-Dec-19 22:33 nos/models/clip.py
--rw-r--r--  2.0 unx     2830 b- defN 23-Dec-19 22:33 nos/models/faster_rcnn.py
--rw-r--r--  2.0 unx     7693 b- defN 24-Feb-20 17:08 nos/models/llm.py
--rw-r--r--  2.0 unx     2875 b- defN 23-Dec-19 22:33 nos/models/monodepth.py
--rw-r--r--  2.0 unx     2939 b- defN 23-Dec-19 22:33 nos/models/owlvit.py
--rw-r--r--  2.0 unx     2618 b- defN 23-Dec-19 22:33 nos/models/sam.py
--rw-r--r--  2.0 unx     5195 b- defN 24-Jan-02 20:35 nos/models/stable_diffusion.py
--rw-r--r--  2.0 unx     1618 b- defN 23-Oct-11 22:45 nos/models/tts.py
--rw-r--r--  2.0 unx     4296 b- defN 24-Feb-20 17:08 nos/models/whisper.py
--rw-r--r--  2.0 unx     6462 b- defN 23-Dec-19 22:33 nos/models/yolox.py
--rw-r--r--  2.0 unx     3232 b- defN 23-Dec-19 22:33 nos/models/dreambooth/dreambooth.py
--rw-r--r--  2.0 unx     4866 b- defN 23-Dec-19 22:33 nos/models/dreambooth/hub.py
--rw-r--r--  2.0 unx       25 b- defN 23-Sep-10 21:56 nos/models/openmmlab/__init__.py
--rw-r--r--  2.0 unx     4857 b- defN 23-Dec-19 22:33 nos/models/openmmlab/hub.py
--rw-r--r--  2.0 unx     6079 b- defN 23-Dec-19 22:33 nos/models/openmmlab/mmdetection.py
--rw-r--r--  2.0 unx     2130 b- defN 23-Sep-21 19:18 nos/models/super_resolution/__init__.py
--rw-r--r--  2.0 unx      472 b- defN 23-Sep-02 01:00 nos/models/super_resolution/config.py
--rw-r--r--  2.0 unx     2199 b- defN 23-Sep-02 01:00 nos/models/super_resolution/ldm.py
--rw-r--r--  2.0 unx     1865 b- defN 23-Sep-02 01:00 nos/models/super_resolution/swin2sr.py
--rw-r--r--  2.0 unx     1284 b- defN 24-Feb-20 17:08 nos/neuron/device.py
--rw-r--r--  2.0 unx     1895 b- defN 24-Jan-02 20:35 nos/proto/nos_service.proto
--rw-r--r--  2.0 unx    10483 b- defN 23-Dec-19 22:33 nos/server/__init__.py
--rw-r--r--  2.0 unx     7341 b- defN 24-Jan-02 20:35 nos/server/_docker.py
--rw-r--r--  2.0 unx     9632 b- defN 24-Feb-20 17:08 nos/server/_runtime.py
--rw-r--r--  2.0 unx    20201 b- defN 24-Feb-20 17:08 nos/server/_service.py
--rw-r--r--  2.0 unx       83 b- defN 23-Oct-24 05:52 nos/server/http/__init__.py
--rw-r--r--  2.0 unx    20019 b- defN 24-Apr-11 19:08 nos/server/http/_service.py
--rw-r--r--  2.0 unx     2865 b- defN 23-Dec-19 22:33 nos/server/http/_utils.py
--rw-r--r--  2.0 unx     4223 b- defN 24-Jan-02 20:35 nos/server/http/integrations/openai/models.py
--rw-r--r--  2.0 unx      373 b- defN 23-Apr-23 00:49 nos/test/benchmark.py
--rw-r--r--  2.0 unx    10761 b- defN 24-Jan-02 20:35 nos/test/conftest.py
--rw-r--r--  2.0 unx     2749 b- defN 24-Jan-02 20:35 nos/test/utils.py
--rw-r--r--  2.0 unx   259865 b- defN 23-Sep-21 19:18 nos/test/test_data/test.jpg
--rw-r--r--  2.0 unx   300601 b- defN 23-Sep-21 19:18 nos/test/test_data/test.mp4
--rw-r--r--  2.0 unx  1152693 b- defN 23-Sep-21 19:18 nos/test/test_data/test_speech.flac
--rw-r--r--  2.0 unx      178 b- defN 24-Jan-02 20:35 nos/test/test_data/hub/custom_model/models/model.py
--rw-r--r--  2.0 unx     2101 b- defN 24-Jan-22 21:22 nos-profiling-catalogs/nos-profile--0-1-4a--20240122--nvidia-geforce-rtx-2080.json
--rw-rw-r--  2.0 unx     2086 b- defN 24-Jan-23 21:49 nos-profiling-catalogs/nos-profile--0-1-5--20240123--nvidia-geforce-rtx-2080.json
--rw-r--r--  2.0 unx     3006 b- defN 23-Aug-29 22:59 scripts/nos_bot.py
--rw-rw-r--  2.0 unx    11355 b- defN 24-Apr-11 19:15 torch_nos-0.2.0b0.dist-info/LICENSE
--rw-r--r--  2.0 unx    26900 b- defN 24-Apr-11 19:15 torch_nos-0.2.0b0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 19:15 torch_nos-0.2.0b0.dist-info/WHEEL
--rw-r--r--  2.0 unx      135 b- defN 24-Apr-11 19:15 torch_nos-0.2.0b0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       74 b- defN 24-Apr-11 19:15 torch_nos-0.2.0b0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7431 b- defN 24-Apr-11 19:15 torch_nos-0.2.0b0.dist-info/RECORD
-91 files, 2182274 bytes uncompressed, 1740937 bytes compressed:  20.2%
+Zip file size: 1747899 bytes, number of entries: 87
+-rw-r--r--  2.0 unx       49 b- defN 24-May-04 18:32 nos/__init__.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-04 18:32 nos/constants.py
+-rw-r--r--  2.0 unx      750 b- defN 24-May-04 18:32 nos/exceptions.py
+-rw-r--r--  2.0 unx     2295 b- defN 24-May-04 18:32 nos/logging.py
+-rw-r--r--  2.0 unx     3199 b- defN 24-May-04 18:32 nos/protoc.py
+-rw-r--r--  2.0 unx     1438 b- defN 24-May-04 18:32 nos/telemetry.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-04 18:32 nos/version.py
+-rw-r--r--  2.0 unx     1898 b- defN 24-May-04 18:32 nos/catalogs/model_profile_catalog.json
+-rw-r--r--  2.0 unx      858 b- defN 24-May-04 18:32 nos/cli/cli.py
+-rw-r--r--  2.0 unx     1417 b- defN 24-May-04 18:32 nos/cli/hub.py
+-rw-r--r--  2.0 unx     7385 b- defN 24-May-04 18:32 nos/cli/predict.py
+-rw-r--r--  2.0 unx    13556 b- defN 24-May-04 18:32 nos/cli/profile.py
+-rw-r--r--  2.0 unx    19109 b- defN 24-May-04 18:32 nos/cli/serve.py
+-rw-r--r--  2.0 unx     1838 b- defN 24-May-04 18:32 nos/cli/system.py
+-rw-r--r--  2.0 unx      425 b- defN 24-May-04 18:32 nos/cli/utils.py
+-rw-r--r--  2.0 unx     1847 b- defN 24-May-04 18:32 nos/cli/templates/docker-compose.serve.yml.j2
+-rw-r--r--  2.0 unx      398 b- defN 24-May-04 18:32 nos/client/__init__.py
+-rw-r--r--  2.0 unx    30496 b- defN 24-May-04 18:32 nos/client/grpc.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-May-04 18:32 nos/common/__init__.py
+-rw-r--r--  2.0 unx      204 b- defN 24-May-04 18:32 nos/common/cloudpickle.py
+-rw-r--r--  2.0 unx      906 b- defN 24-May-04 18:32 nos/common/exceptions.py
+-rw-r--r--  2.0 unx     5154 b- defN 24-May-04 18:32 nos/common/git.py
+-rw-r--r--  2.0 unx     1028 b- defN 24-May-04 18:32 nos/common/helpers.py
+-rw-r--r--  2.0 unx      499 b- defN 24-May-04 18:32 nos/common/metaclass.py
+-rw-r--r--  2.0 unx    20811 b- defN 24-May-04 18:32 nos/common/profiler.py
+-rw-r--r--  2.0 unx      805 b- defN 24-May-04 18:32 nos/common/runtime.py
+-rw-r--r--  2.0 unx    11856 b- defN 24-May-04 18:32 nos/common/shm.py
+-rw-r--r--  2.0 unx    26198 b- defN 24-May-04 18:32 nos/common/spec.py
+-rw-r--r--  2.0 unx     7930 b- defN 24-May-04 18:32 nos/common/system.py
+-rw-r--r--  2.0 unx      830 b- defN 24-May-04 18:32 nos/common/tasks.py
+-rw-r--r--  2.0 unx     6117 b- defN 24-May-04 18:32 nos/common/types.py
+-rw-r--r--  2.0 unx     1465 b- defN 24-May-04 18:32 nos/common/io/__init__.py
+-rw-r--r--  2.0 unx     1050 b- defN 24-May-04 18:32 nos/common/io/video/base.py
+-rw-r--r--  2.0 unx     8777 b- defN 24-May-04 18:32 nos/common/io/video/opencv.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 18:32 nos/executors/__init__.py
+-rw-r--r--  2.0 unx     9283 b- defN 24-May-04 18:32 nos/executors/ray.py
+-rw-r--r--  2.0 unx    15315 b- defN 24-May-04 18:32 nos/hub/__init__.py
+-rw-r--r--  2.0 unx     1756 b- defN 24-May-04 18:32 nos/hub/config.py
+-rw-r--r--  2.0 unx      538 b- defN 24-May-04 18:32 nos/hub/hf.py
+-rw-r--r--  2.0 unx       59 b- defN 24-May-04 18:32 nos/managers/__init__.py
+-rw-r--r--  2.0 unx    24163 b- defN 24-May-04 18:32 nos/managers/model.py
+-rw-r--r--  2.0 unx     4738 b- defN 24-May-04 18:32 nos/managers/pool.py
+-rw-r--r--  2.0 unx      773 b- defN 24-May-04 18:32 nos/models/__init__.py
+-rw-r--r--  2.0 unx     3138 b- defN 24-May-04 18:32 nos/models/_noop.py
+-rw-r--r--  2.0 unx     3841 b- defN 24-May-04 18:32 nos/models/blip.py
+-rw-r--r--  2.0 unx     4220 b- defN 24-May-04 18:32 nos/models/clip.py
+-rw-r--r--  2.0 unx     2830 b- defN 24-May-04 18:32 nos/models/faster_rcnn.py
+-rw-r--r--  2.0 unx     7693 b- defN 24-May-04 18:32 nos/models/llm.py
+-rw-r--r--  2.0 unx     2875 b- defN 24-May-04 18:32 nos/models/monodepth.py
+-rw-r--r--  2.0 unx     2939 b- defN 24-May-04 18:32 nos/models/owlvit.py
+-rw-r--r--  2.0 unx     2618 b- defN 24-May-04 18:32 nos/models/sam.py
+-rw-r--r--  2.0 unx     5195 b- defN 24-May-04 18:32 nos/models/stable_diffusion.py
+-rw-r--r--  2.0 unx     1618 b- defN 24-May-04 18:32 nos/models/tts.py
+-rw-r--r--  2.0 unx     4296 b- defN 24-May-04 18:32 nos/models/whisper.py
+-rw-r--r--  2.0 unx     6462 b- defN 24-May-04 18:32 nos/models/yolox.py
+-rw-r--r--  2.0 unx     3232 b- defN 24-May-04 18:32 nos/models/dreambooth/dreambooth.py
+-rw-r--r--  2.0 unx     4866 b- defN 24-May-04 18:32 nos/models/dreambooth/hub.py
+-rw-r--r--  2.0 unx     4857 b- defN 24-May-04 18:32 nos/models/openmmlab/hub.py
+-rw-r--r--  2.0 unx     6079 b- defN 24-May-04 18:32 nos/models/openmmlab/mmdetection.py
+-rw-r--r--  2.0 unx     2130 b- defN 24-May-04 18:32 nos/models/super_resolution/__init__.py
+-rw-r--r--  2.0 unx      472 b- defN 24-May-04 18:32 nos/models/super_resolution/config.py
+-rw-r--r--  2.0 unx     2199 b- defN 24-May-04 18:32 nos/models/super_resolution/ldm.py
+-rw-r--r--  2.0 unx     1865 b- defN 24-May-04 18:32 nos/models/super_resolution/swin2sr.py
+-rw-r--r--  2.0 unx     1284 b- defN 24-May-04 18:32 nos/neuron/device.py
+-rw-r--r--  2.0 unx     1895 b- defN 24-May-04 18:32 nos/proto/nos_service.proto
+-rw-r--r--  2.0 unx    10464 b- defN 24-May-04 18:32 nos/server/__init__.py
+-rw-r--r--  2.0 unx     7341 b- defN 24-May-04 18:32 nos/server/_docker.py
+-rw-r--r--  2.0 unx     9632 b- defN 24-May-04 18:32 nos/server/_runtime.py
+-rw-r--r--  2.0 unx    20201 b- defN 24-May-04 18:32 nos/server/_service.py
+-rw-r--r--  2.0 unx     1097 b- defN 24-May-04 18:32 nos/server/http/_exceptions.py
+-rw-r--r--  2.0 unx     1066 b- defN 24-May-04 18:32 nos/server/http/_security.py
+-rw-r--r--  2.0 unx    20644 b- defN 24-May-04 18:32 nos/server/http/_service.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-04 18:32 nos/server/http/_utils.py
+-rw-r--r--  2.0 unx     4223 b- defN 24-May-04 18:32 nos/server/http/integrations/openai/models.py
+-rw-r--r--  2.0 unx      373 b- defN 24-May-04 18:32 nos/test/benchmark.py
+-rw-r--r--  2.0 unx    10900 b- defN 24-May-04 18:32 nos/test/conftest.py
+-rw-r--r--  2.0 unx     2749 b- defN 24-May-04 18:32 nos/test/utils.py
+-rw-r--r--  2.0 unx   259865 b- defN 24-May-04 18:32 nos/test/test_data/test.jpg
+-rw-r--r--  2.0 unx   300601 b- defN 24-May-04 18:32 nos/test/test_data/test.mp4
+-rw-r--r--  2.0 unx  1152693 b- defN 24-May-04 18:32 nos/test/test_data/test_speech.flac
+-rw-r--r--  2.0 unx      178 b- defN 24-May-04 18:32 nos/test/test_data/hub/custom_model/models/model.py
+-rw-r--r--  2.0 unx    11355 b- defN 24-May-04 18:48 torch_nos-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    26736 b- defN 24-May-04 18:48 torch_nos-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-04 18:48 torch_nos-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      135 b- defN 24-May-04 18:48 torch_nos-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-04 18:48 torch_nos-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6985 b- defN 24-May-04 18:48 torch_nos-0.3.0.dist-info/RECORD
+87 files, 2169076 bytes uncompressed, 1737091 bytes compressed:  19.9%
```

## zipnote {}

```diff
@@ -102,17 +102,14 @@
 
 Filename: nos/executors/__init__.py
 Comment: 
 
 Filename: nos/executors/ray.py
 Comment: 
 
-Filename: nos/externals/streamlink.py
-Comment: 
-
 Filename: nos/hub/__init__.py
 Comment: 
 
 Filename: nos/hub/config.py
 Comment: 
 
 Filename: nos/hub/hf.py
@@ -168,17 +165,14 @@
 
 Filename: nos/models/dreambooth/dreambooth.py
 Comment: 
 
 Filename: nos/models/dreambooth/hub.py
 Comment: 
 
-Filename: nos/models/openmmlab/__init__.py
-Comment: 
-
 Filename: nos/models/openmmlab/hub.py
 Comment: 
 
 Filename: nos/models/openmmlab/mmdetection.py
 Comment: 
 
 Filename: nos/models/super_resolution/__init__.py
@@ -207,15 +201,18 @@
 
 Filename: nos/server/_runtime.py
 Comment: 
 
 Filename: nos/server/_service.py
 Comment: 
 
-Filename: nos/server/http/__init__.py
+Filename: nos/server/http/_exceptions.py
+Comment: 
+
+Filename: nos/server/http/_security.py
 Comment: 
 
 Filename: nos/server/http/_service.py
 Comment: 
 
 Filename: nos/server/http/_utils.py
 Comment: 
@@ -240,35 +237,26 @@
 
 Filename: nos/test/test_data/test_speech.flac
 Comment: 
 
 Filename: nos/test/test_data/hub/custom_model/models/model.py
 Comment: 
 
-Filename: nos-profiling-catalogs/nos-profile--0-1-4a--20240122--nvidia-geforce-rtx-2080.json
-Comment: 
-
-Filename: nos-profiling-catalogs/nos-profile--0-1-5--20240123--nvidia-geforce-rtx-2080.json
-Comment: 
-
-Filename: scripts/nos_bot.py
-Comment: 
-
-Filename: torch_nos-0.2.0b0.dist-info/LICENSE
+Filename: torch_nos-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: torch_nos-0.2.0b0.dist-info/METADATA
+Filename: torch_nos-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: torch_nos-0.2.0b0.dist-info/WHEEL
+Filename: torch_nos-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: torch_nos-0.2.0b0.dist-info/entry_points.txt
+Filename: torch_nos-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: torch_nos-0.2.0b0.dist-info/top_level.txt
+Filename: torch_nos-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: torch_nos-0.2.0b0.dist-info/RECORD
+Filename: torch_nos-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nos/__init__.py

```diff
@@ -1,15 +1 @@
-import importlib
-import sys
-
-from nos.version import __version__  # noqa: F401
-
-from .client import Client  # noqa: F401
-from .logging import logger  # noqa: F401
 from .server import init, shutdown  # noqa: F401
-
-
-def internal_libs_available():
-    """Check if the internal module is available."""
-    from .common.runtime import is_package_available  # noqa: F401
-
-    return is_package_available("autonomi.nos._internal")
```

## nos/constants.py

```diff
@@ -11,19 +11,19 @@
 
 NOS_HOME.mkdir(parents=True, exist_ok=True)
 NOS_CACHE_DIR.mkdir(parents=True, exist_ok=True)
 NOS_MODELS_DIR.mkdir(parents=True, exist_ok=True)
 NOS_LOG_DIR.mkdir(parents=True, exist_ok=True)
 NOS_TMP_DIR.mkdir(parents=True, exist_ok=True)
 
-DEFAULT_HTTP_HOST = os.getenv("NOS_HTTP_HOST", "127.0.0.1")
+DEFAULT_HTTP_HOST = os.getenv("NOS_HTTP_HOST", "localhost")
 DEFAULT_HTTP_PORT = int(os.getenv("NOS_HTTP_PORT", 8000))
 DEFAULT_HTTP_ADDRESS = f"{DEFAULT_HTTP_HOST}:{DEFAULT_HTTP_PORT}"
 
-DEFAULT_GRPC_HOST = os.getenv("NOS_GRPC_HOST", "[::]")
+DEFAULT_GRPC_HOST = os.getenv("NOS_GRPC_HOST", "localhost")
 DEFAULT_GRPC_PORT = int(os.getenv("NOS_GRPC_PORT", 50051))
 DEFAULT_GRPC_ADDRESS = f"{DEFAULT_GRPC_HOST}:{DEFAULT_GRPC_PORT}"
 
 GRPC_MAX_MESSAGE_LENGTH = 32 * 1024 * 1024  # 32 MB
 GRPC_MAX_WORKER_THREADS = int(os.getenv("NOS_GRPC_MAX_WORKER_THREADS", 4))
 
 NOS_PROFILING_ENABLED = bool(int(os.getenv("NOS_PROFILING_ENABLED", "0")))
```

## nos/telemetry.py

```diff
@@ -23,17 +23,17 @@
         )
         # Initialize Sentry
         sentry_sdk.init(
             dsn=SENTRY_DSN,
             debug=SENTRY_DEBUG,
             # Set traces_sample_rate to 1.0 to capture 100%
             # of transactions for performance monitoring.
-            traces_sample_rate=1.0,
+            traces_sample_rate=0.05,
             # Set profiles_sample_rate to 1.0 to profile 100%
             # of sampled transactions.
             # We recommend adjusting this value in production.
-            profiles_sample_rate=1.0,
+            profiles_sample_rate=0.05,
             release=__version__,
             integrations=[
                 sentry_loguru,
             ],
         )
```

## nos/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.2.0b"
+__version__ = "0.3.0"
```

## nos/cli/predict.py

```diff
@@ -15,14 +15,15 @@
 import rich.console
 import rich.status
 import rich.table
 import typer
 
 from nos.client import Client
 from nos.common.exceptions import ClientException
+from nos.constants import DEFAULT_GRPC_ADDRESS
 
 
 predict_cli = typer.Typer(name="predict", help="NOS gRPC Prediction CLI.", no_args_is_help=True)
 console = rich.console.Console()
 
 
 @dataclass
@@ -32,15 +33,15 @@
     address: str
     client: Client
 
 
 @predict_cli.callback()
 def grpc_config(
     ctx: typer.Context,
-    address: str = typer.Option("[::]:50051", "-a", "--address", help="Address of the gRPC server."),
+    address: str = typer.Option(DEFAULT_GRPC_ADDRESS, "-a", "--address", help="Address of the gRPC server."),
 ):
     """Common gRPC options"""
     client = Client(address)
     ctx.obj = gRPCConfig(address, client)
     # TODO (spillai): Deploy the gRPC server here in the background (as a docker daemon)
     # TOOD (spillai): Ping the gRPC server otherwise raise an error
```

## nos/cli/serve.py

```diff
@@ -297,15 +297,15 @@
         # Render the dockerfiles
         # agipack is responsible for the "images" sections
         # which are rendered into Dockerfiles and docker-compose files.
         builder = AGIPack(config)
         dockerfiles: Dict[str, Path] = builder.render(
             filename=str(NOS_SERVE_TMP_DIR / f"Dockerfile.{sandbox_name}"),
             env="prod" if prod else "dev",
-            skip_base_builds=False,
+            skip_base_builds=True,
         )
 
         # Check if several targets are defined, if so, expect the user
         # to specify which one to build / serve
         if len(dockerfiles) > 1 and target is None:
             raise ValueError(
                 f"Several targets defined in the config, please specify which one to "
```

## nos/cli/templates/docker-compose.serve.yml.j2

```diff
@@ -1,9 +1,7 @@
-version: "3.8"
-
 services:
 {%- if http %}
   nos-http-gateway:
     image: {{ image }}
     command: nos-http-server --host {{ http_host }} --port {{ http_port }} --workers {{ http_workers }} {% if reload %}--reload --reload-dir {{ reload_dir }} {% endif %}
     environment:
       - NOS_HOME=/app/.nos
@@ -36,14 +34,15 @@
     image: {{ image }}
     {%- if config %}
     command: nos-grpc-server -c {{ config }}
     {%- endif %}
     environment:
       - NOS_HOME=/app/.nos
       - NOS_LOGGING_LEVEL={{ logging_level }}
+      - NOS_GRPC_HOST=[::]
     {%- if env_file|length > 0 %}
     env_file:
       {%- for envf in env_file %}
       - {{ envf }}
       {%- endfor %}
     {%- endif %}
     volumes:
```

## nos/client/grpc.py

```diff
@@ -16,15 +16,15 @@
 from nos.common.exceptions import (
     ClientException,
     InferenceException,
     InputValidationException,
     ServerReadyException,
 )
 from nos.common.shm import NOS_SHM_ENABLED, SharedMemoryTransportManager
-from nos.constants import DEFAULT_GRPC_PORT, GRPC_MAX_MESSAGE_LENGTH, NOS_PROFILING_ENABLED
+from nos.constants import DEFAULT_GRPC_ADDRESS, GRPC_MAX_MESSAGE_LENGTH, NOS_PROFILING_ENABLED
 from nos.logging import logger
 from nos.protoc import import_module
 from nos.version import __version__
 
 
 nos_service_pb2 = import_module("nos_service_pb2")
 nos_service_pb2_grpc = import_module("nos_service_pb2_grpc")
@@ -60,19 +60,19 @@
         >>> visual_model(images=img)  # predict with CLIP
 
         >>> fastrcnn_model = client.Module("torchvision/fasterrcnn-mobilenet-v3-large-320-fpn")  # instantiate FasterRCNN module
         >>> fastrcnn_model(images=img)
         ```
     """
 
-    def __init__(self, address: str = f"[::]:{DEFAULT_GRPC_PORT}"):
+    def __init__(self, address: str = DEFAULT_GRPC_ADDRESS):
         """Initializes the gRPC client.
 
         Args:
-            address (str): Address for the gRPC server. Defaults to f"[::]:{DEFAULT_GRPC_PORT}".
+            address (str): Address for the gRPC server. Defaults to DEFAULT_GRPC_ADDRESS.
         """
         self.address: str = address
         self._channel: grpc.Channel = None
         self._stub: nos_service_pb2_grpc.InferenceServiceStub = None
         self._uuid: str = secrets.token_hex(4)
 
     def __repr__(self) -> str:
@@ -161,15 +161,16 @@
             try:
                 return self.IsHealthy()
             except Exception:
                 elapsed = time.time() - st
                 if int(elapsed) > 10:
                     logger.warning("Waiting for server to start... (elapsed={:.0f}s)".format(time.time() - st))
                 time.sleep(retry_interval)
-        raise ServerReadyException("Failed to ping server.")
+        default_msg = """\n If you are running the server in docker, make sure the server sets `NOS_GRPC_HOST=[::]` and the client sets `NOS_GRPC_HOST=<server-container-name>` in their environment variables."""
+        raise ServerReadyException(f"Failed to ping server. {default_msg}")
 
     def GetServiceVersion(self) -> str:
         """Get service version.
 
         Returns:
             str: Service version (e.g. 0.0.4).
         Raises:
```

## nos/common/__init__.py

```diff
@@ -12,15 +12,14 @@
     FunctionSignature,
     ModelDeploymentSpec,
     ModelResources,
     ModelServiceSpec,
     ModelSpec,
     ModelSpecMetadata,
     ModelSpecMetadataCatalog,
-    ObjectTypeInfo,
 )
 from .tasks import TaskType
 from .types import Batch, EmbeddingSpec, ImageSpec, ImageT, TensorSpec, TensorT
 
 
 def tqdm(iterable: Any = None, *args, skip: int = 0, **kwargs) -> Any:
     """Wrapper around tqdm that allows for a duration to be
```

## nos/common/shm.py

```diff
@@ -249,15 +249,15 @@
         for key in shm_map.keys():
             assert key in data, f"Key {key} not found in data dict."
             if isinstance(data[key], list):
                 assert len(data[key]) == len(
                     shm_map[key]
                 ), f"Shared memory already initialized with length={len(shm_map[key])}, provided input with length={len(data[key])}."
                 # Move data from the data dict value to the shared memory segment.
-                for item, shm in zip(data[key], shm_map[key]):
+                for item, shm in zip(data[key], shm_map[key], strict=False):
                     shm.copy_from(item)
             elif isinstance(data[key], np.ndarray):
                 # Move data from the data dict value to the shared memory segment.
                 shm_map[key].copy_from(data[key])
             else:
                 raise ValueError(f"Unsupported type [type={type(data[key])}]")
```

## nos/common/spec.py

```diff
@@ -1,13 +1,13 @@
 import inspect
 import math
 import re
 from dataclasses import field
 from functools import cached_property
-from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, Union, get_args, get_origin
+from typing import Any, Callable, Dict, Literal, Optional, Tuple, Union
 
 import humanize
 from pydantic import BaseModel, Field, field_validator
 from pydantic.dataclasses import dataclass
 
 from nos.common.cloudpickle import dumps, loads
 from nos.common.exceptions import InputValidationException
@@ -20,129 +20,14 @@
 from nos.protoc import import_module
 
 
 logger.disable(__name__)
 nos_service_pb2 = import_module("nos_service_pb2")
 
 
-class ObjectTypeInfo:
-    """Function signature information.
-
-    Parameters:
-        annotation (Any): Annotation for an input/output.
-        parameter (inspect.Parameter): Parameter information (optional).
-
-    Attributes:
-        _is_batched (bool): Batched flag.
-        _batch_size (int): Batch size.
-        _base_type (Any): Base type (Image.Image, np.ndarray etc).
-        _base_spec (Any): Base type specification (None, ImageSpec, TensorSpec etc).
-    """
-
-    def __init__(self, annotation: Any, parameter: inspect.Parameter = None):
-        """Initialize the function signature information."""
-        self.annotation = annotation
-        self.parameter = parameter
-        try:
-            (annotated_cls,) = annotation.__args__
-        except AttributeError:
-            annotated_cls = annotation
-
-        # Parse Batch annotation
-        self._is_batched, self._batch_size = False, None
-        if annotated_cls == Batch:
-            annotation, batch_size = annotation.__metadata__
-            self._is_batched, self._batch_size = True, batch_size
-            try:
-                (annotated_cls,) = annotation.__args__
-            except AttributeError:
-                annotated_cls = annotation
-
-        # Parse Tensor/type annotation
-        if annotated_cls in (TensorT, ImageT):
-            object_type, object_spec = annotation.__metadata__
-        else:
-            try:
-                (object_type,) = annotation.__metadata__
-            except AttributeError:
-                object_type = annotated_cls
-            object_spec = None
-
-        # Parse the base type and spec
-        self._base_type = object_type
-        self._base_spec = object_spec
-
-    def __repr__(self) -> str:
-        """Return the function signature information representation."""
-        repr = (
-            f"""{self.__class__.__name__}(is_batched={self._is_batched}, batch_size={self._batch_size}, """
-            f"""base_type={self._base_type}, base_spec={self._base_spec})"""
-        )
-        if self.parameter:
-            p_repr = f"pname={self.parameter}, ptype={self.parameter.annotation}, pdefault={self.parameter.default}"
-            repr = f"{repr}, {p_repr}"
-        return repr
-
-    def parameter_name(self) -> str:
-        """Return the parameter name."""
-        return self.parameter.name
-
-    def parameter_annotation(self) -> Any:
-        """Return the parameter annotation."""
-        return self.parameter.annotation
-
-    def parameter_default(self) -> Any:
-        """Return the parameter default."""
-        return self.parameter.default
-
-    def is_batched(self) -> bool:
-        """Return the `is_batched` flag.
-
-        Returns:
-            bool: Flag to indicate if batching is enabled.
-                If true, `batch_size=None` implies dynamic batch size, otherwise `batch_size=<int>`.
-        """
-        return self._is_batched
-
-    def batch_size(self) -> int:
-        """Return the batch size.
-
-        Returns:
-            int: Batch size. If `None` and `is_batched` is `true`, then batch size is considered dynamic.
-        """
-        return self._batch_size
-
-    def base_type(self) -> Any:
-        """Return the base type.
-
-        Returns:
-            Any: Base type. Base type here can be simple types (e.g. `str`, `int`, ...) or
-                complex types with library dependencies (e.g. `np.ndarray`, `PIL.Image.Image` etc).
-        """
-        return self._base_type
-
-    def base_spec(self) -> Optional[Union[TensorSpec, ImageSpec, EmbeddingSpec]]:
-        """Return the base spec.
-
-        Returns:
-            Optional[Union[TensorSpec, ImageSpec, EmbeddingSpec]]: Base spec.
-        """
-        return self._base_spec
-
-
-def AnnotatedParameter(
-    annotation: Any, parameter: inspect.Parameter = None
-) -> Union[ObjectTypeInfo, List[ObjectTypeInfo]]:
-    """Annotate the parameter for inferring additional metdata."""
-    # Union of annotated types are converted into set of annotated types.
-    if get_origin(annotation) == Union:
-        return [AnnotatedParameter(ann, parameter) for ann in get_args(annotation)]
-    return ObjectTypeInfo(annotation, parameter)
-
-
 class FunctionSignature(BaseModel):
     """Function signature that fully describes the remote-model to be executed
     including `inputs`, `outputs`, `func_or_cls` to be executed,
     initialization `args`/`kwargs`."""
 
     func_or_cls: Callable
     """Class instance."""
@@ -232,42 +117,14 @@
         return {k: dumps(v) for k, v in inputs.items()}
 
     def _decode_inputs(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
         """Decode inputs based on defined signature."""
         inputs = FunctionSignature.validate(inputs, self.parameters)
         return {k: loads(v) for k, v in inputs.items()}
 
-    def get_inputs_spec(self) -> Dict[str, Union[ObjectTypeInfo, List[ObjectTypeInfo]]]:
-        """Return the full input function signature specification.
-
-        For example, for CLIP's text embedding model, the inputs/output spec is:
-            ```
-            inputs  = {'texts': ObjectTypeInfo(is_batched=True, batch_size=None, base_type=<class 'str'>, base_spec=None)}
-            outputs = {'embedding': ObjectTypeInfo(is_batched=True, batch_size=None, base_type=<class 'numpy.ndarray'>, base_spec=EmbeddingSpec(shape=(512,), dtype='float32'))}
-            ```
-        Returns:
-            Dict[str, Union[ObjectTypeInfo, List[ObjectTypeInfo]]]: Inputs spec.
-        """
-        parameters = self.parameters.copy()
-        parameters.pop("self", None)
-        return {k: AnnotatedParameter(self.input_annotations.get(k, p.annotation), p) for k, p in parameters.items()}
-
-    def get_outputs_spec(self) -> Dict[str, Union[ObjectTypeInfo, Dict[str, ObjectTypeInfo]]]:
-        """Return the full output function signature specification.
-
-        Returns:
-            Dict[str, Union[ObjectTypeInfo, Dict[str, ObjectTypeInfo]]]: Outputs spec.
-        """
-        if self.output_annotations is None:
-            return AnnotatedParameter(self.return_annotation)
-        elif isinstance(self.output_annotations, dict):
-            return {k: AnnotatedParameter(ann) for k, ann in self.output_annotations.items()}
-        else:
-            return AnnotatedParameter(self.output_annotations)
-
 
 class ModelResources(BaseModel):
     """Model resources (device/host memory etc)."""
 
     runtime: str = Field(default="auto")
     """Runtime type (cpu, gpu, trt, etc).
     See `nos.server._runtime.InferenceServiceRuntime` for the list of supported runtimes.
```

## nos/models/__init__.py

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Dict, List, Union
 
 import numpy as np
 from PIL import Image
 
-from nos import hub, internal_libs_available
+from nos import hub
 from nos.common import ImageSpec, TaskType
 from nos.common.types import Batch, ImageT
 
 from ._noop import NoOp  # noqa: F401
 from .blip import BLIP  # noqa: F401
 from .clip import CLIP  # noqa: F401
 from .faster_rcnn import FasterRCNN  # noqa: F401
@@ -17,12 +17,7 @@
 from .owlvit import OwlViT  # noqa: F401
 from .sam import SAM
 from .stable_diffusion import StableDiffusion  # noqa: F401
 from .super_resolution import SuperResolution  # noqa: F401
 from .tts import TextToSpeech  # noqa: F401
 from .whisper import Whisper  # noqa: F401
 from .yolox import YOLOX  # noqa: F401
-
-
-if internal_libs_available():
-    # Register internal models with hub
-    from autonomi.nos._internal import models  # noqa: F401, F403
```

## nos/server/__init__.py

```diff
@@ -2,15 +2,14 @@
 import math
 import platform
 import subprocess
 from collections import deque
 from typing import List, Optional, Union
 
 import psutil
-import rich.status
 
 import docker
 import docker.errors
 import docker.models.containers
 from nos.common.shm import NOS_SHM_ENABLED
 from nos.constants import DEFAULT_GRPC_PORT
 from nos.logging import logger
```

## nos/server/http/_service.py

```diff
@@ -18,14 +18,16 @@
 from nos.client import Client
 from nos.common.tasks import TaskType
 from nos.constants import DEFAULT_GRPC_ADDRESS
 from nos.logging import logger
 from nos.protoc import import_module
 from nos.version import __version__
 
+from ._exceptions import default_exception_handler, default_exception_middleware
+from ._security import ValidMachineToMachine as ValidM2M
 from ._utils import decode_item, encode_item
 from .integrations.openai.models import (
     ChatCompletionsRequest,
     ChatModel,
     Choice,
     Completion,
     DeltaChoice,
@@ -56,36 +58,22 @@
     """Whether to stream the response"""
 
 
 @dataclasses.dataclass
 class InferenceService:
     """HTTP server application for NOS API."""
 
-    version: str = field(default="v1")
-    """NOS version."""
-
     address: str = field(default=DEFAULT_GRPC_ADDRESS)
     """gRPC address."""
 
-    env: str = field(default=HTTP_ENV)
-    """Environment (dev/prod/test)."""
-
     model_config = ConfigDict(arbitrary_types_allowed=True)
     """Model configuration."""
 
     def __post_init__(self):
         """Post initialization."""
-        self.app = FastAPI(
-            title="NOS REST API",
-            description=f"NOS REST API (version={__version__}, api_version={self.version})",
-            version=self.version,
-            debug=self.env != "prod",
-        )
-        logger.debug(f"Starting NOS REST API (version={__version__}, env={self.env})")
-
         self.client = Client(self.address)
         logger.debug(f"Connecting to gRPC server (address={self.client.address})")
 
         if not self.client.WaitForServer(timeout=60, retry_interval=5):
             raise RuntimeError("Failed to connect to gRPC server")
         if not self.client.IsHealthy():
             raise RuntimeError("gRPC server is not healthy")
@@ -140,20 +128,41 @@
         version (str): NOS version.
         address (str): gRPC address.
         env (str): Environment (prod, dev, test).
 
     Returns:
         (FastAPI) FastAPI application.
     """
-    nos_app = InferenceService(version=version, address=address, env=env)
-    app = nos_app.app
+    from fastapi.middleware.cors import CORSMiddleware
+
+    svc = InferenceService(address=address)
+    logger.info(f"app_factory [env={env}]: Adding CORS middleware ...")
+    app = FastAPI(
+        title="NOS REST API",
+        description=f"NOS REST API (version={__version__}, api_version={version})",
+        version=version,
+        debug=env != "prod",
+    )
+    app.add_middleware(
+        CORSMiddleware,
+        allow_origins=["*"],
+        allow_credentials=True,
+        allow_methods=["*"],
+        allow_headers=["*"],
+    )
+    logger.debug(f"Starting NOS REST API (version={__version__}, env={env})")
+
+    # Add default exception handler
+    logger.info(f"app_factory [env={env}]: Adding default exception handlers ...")
+    app.middleware("http")(default_exception_middleware)
+    app.add_exception_handler(Exception, default_exception_handler)
 
     def get_client() -> Client:
         """Get the inference client."""
-        return nos_app.client
+        return svc.client
 
     def unnormalize_id(model_id: str) -> str:
         """Un-normalize the model identifier."""
         return model_id.replace("--", "/")
 
     def normalize_id(model_id: str) -> str:
         """Normalize the model identifier."""
@@ -188,33 +197,39 @@
         return JSONResponse(
             content={"status": "ok" if client.IsHealthy() else "not_ok"}, status_code=status.HTTP_200_OK
         )
 
     @app.get(f"/{version}/models", status_code=status.HTTP_200_OK, response_model=Model)
     def models(
         client: Client = Depends(get_client),
+        user: Depends = ValidM2M,
     ) -> Model:
         """List all available models."""
         _model_table = build_model_table(client)
         logger.debug(f"Listing models [models={_model_table.values()}]")
         return Model(data=list(_model_table.values()))
 
     @app.get(f"/{version}/models/" + "{model:path}", response_model=ChatModel)
-    def model_info(model: str, client: Client = Depends(get_client)) -> ChatModel:
+    def model_info(
+        model: str,
+        client: Client = Depends(get_client),
+        user: Depends = ValidM2M,
+    ) -> ChatModel:
         """Get model information."""
         _model_table = build_model_table(client)
         try:
             return _model_table[unnormalize_id(model)]
         except KeyError:
             raise HTTPException(status_code=400, detail=f"Invalid model {model}")
 
     @app.post(f"/{version}/chat/completions", status_code=status.HTTP_201_CREATED)
     def chat(
         request: ChatCompletionsRequest,
         client: Client = Depends(get_client),
+        user: Depends = ValidM2M,
     ) -> StreamingResponse:
         """Perform chat completion on the given input data."""
         logger.debug(f"Received chat request [model={request.model}, messages={request.messages}]")
         _model_table = build_model_table(client)
         model_id: str = unnormalize_id(request.model)
         try:
             _ = _model_table[model_id]
@@ -266,14 +281,15 @@
             choices = [Choice(message=Message(role="assistant", content=content), finish_reason="stop")]
             return Completion(id=request.id, model=request.model, choices=choices)
 
     @app.post(f"/{version}/infer", status_code=status.HTTP_201_CREATED)
     def infer(
         request: InferenceRequest,
         client: Client = Depends(get_client),
+        user: Depends = ValidM2M,
     ) -> JSONResponse:
         """Perform inference on the given input data.
 
         $ curl -X "POST" \
             "http://localhost:8000/v1/infer" \
             -H "Content-Type: appication/json" \
             -d '{
@@ -315,14 +331,15 @@
     @app.post(f"/{version}/infer/file", status_code=status.HTTP_201_CREATED)
     def infer_file(
         model_id: str = Form(...),
         method: Optional[str] = Form(None),
         file: Optional[UploadFile] = File(None),
         url: Optional[str] = Form(None),
         client: Client = Depends(get_client),
+        user: Depends = ValidM2M,
     ) -> JSONResponse:
         """Perform inference on the given input data using multipart/form-data.
 
         $ curl -X POST \
             'http://localhost:8000/v1/infer/file \
             -H 'accept: application/json' \
             -H 'Content-Type: multipart/form-data' \
```

## nos/test/conftest.py

```diff
@@ -1,11 +1,11 @@
 import pytest
 from loguru import logger
 
-from nos.constants import DEFAULT_GRPC_PORT
+from nos.constants import DEFAULT_GRPC_HOST, DEFAULT_GRPC_PORT
 from nos.protoc import import_module
 
 
 GRPC_TEST_PORT = DEFAULT_GRPC_PORT + 1
 GRPC_TEST_PORT_CPU = DEFAULT_GRPC_PORT + 2
 GRPC_TEST_PORT_GPU = DEFAULT_GRPC_PORT + 3
 
@@ -58,15 +58,15 @@
     logger.info(f"Starting gRPC test server on port: {GRPC_TEST_PORT}")
     options = [
         ("grpc.max_message_length", GRPC_MAX_MESSAGE_LENGTH),
         ("grpc.max_send_message_length", GRPC_MAX_MESSAGE_LENGTH),
         ("grpc.max_receive_message_length", GRPC_MAX_MESSAGE_LENGTH),
     ]
     server = aio.server(options=options)
-    address = f"[::]:{GRPC_TEST_PORT}"
+    address = f"{DEFAULT_GRPC_HOST}:{GRPC_TEST_PORT}"
     nos_service_pb2_grpc.add_InferenceServiceServicer_to_server(InferenceServiceImpl(), server)
     server.add_insecure_port(address)
 
     await server.start()
     assert server is not None
 
     yield server
@@ -74,31 +74,31 @@
 
 
 @pytest.fixture(scope="session")
 def grpc_client():
     """Test gRPC client (Port: 50052)."""
     from nos.client import Client
 
-    yield Client(f"[::]:{GRPC_TEST_PORT}")
+    yield Client(f"{DEFAULT_GRPC_HOST}:{GRPC_TEST_PORT}")
 
 
 @pytest.fixture(scope="session")
 def grpc_client_cpu():
     """Test gRPC client to be used with CPU docker runtime (Port: 50053)."""
     from nos.client import Client
 
-    yield Client(f"[::]:{GRPC_TEST_PORT_CPU}")
+    yield Client(f"{DEFAULT_GRPC_HOST}:{GRPC_TEST_PORT_CPU}")
 
 
 @pytest.fixture(scope="session")
 def grpc_client_gpu():
     """Test gRPC client to be used with GPU docker runtime (Port: 50054)."""
     from nos.client import Client
 
-    yield Client(f"[::]:{GRPC_TEST_PORT_GPU}")
+    yield Client(f"{DEFAULT_GRPC_HOST}:{GRPC_TEST_PORT_GPU}")
 
 
 @pytest.fixture(scope="session")
 def grpc_server_docker_runtime_cpu():
     """Test DockerRuntime CPU (Port: 50053)."""
     from nos.server import InferenceServiceRuntime
 
@@ -226,15 +226,15 @@
 def local_http_client_with_server(grpc_server):  # noqa: F811
     """Test local HTTP client with local runtime."""
     from fastapi.testclient import TestClient
 
     from nos.server.http._service import app_factory
 
     # Yield the HTTP client once the server is up and initialized
-    with TestClient(app_factory(address=f"[::]:{GRPC_TEST_PORT}")) as _client:
+    with TestClient(app_factory(address=f"{DEFAULT_GRPC_HOST}:{GRPC_TEST_PORT}")) as _client:
         yield _client
 
 
 # Note: These fixtures need to be named the same as the following variables
 # so that we reference them by value in the test functions.
 HTTP_CLIENT_WITH_CPU = "http_client_with_cpu_backend"
 
@@ -243,15 +243,15 @@
 def http_client_with_cpu_backend(grpc_server_docker_runtime_cpu):  # noqa: F811
     """Test HTTP client with initialized CPU docker runtime (Port: 50053)."""
     from fastapi.testclient import TestClient
 
     from nos.server.http._service import app_factory
 
     # Yield the HTTP client once the server is up and initialized
-    with TestClient(app_factory(address=f"[::]:{GRPC_TEST_PORT_CPU}")) as _client:
+    with TestClient(app_factory(address=f"{DEFAULT_GRPC_HOST}:{GRPC_TEST_PORT_CPU}")) as _client:
         yield _client
 
 
 # Note: These fixtures need to be named the same as the following variables
 # so that we reference them by value in the test functions.
 HTTP_CLIENT_WITH_GPU = "http_client_with_gpu_backend"
 
@@ -260,15 +260,15 @@
 def http_client_with_gpu_backend(grpc_server_docker_runtime_gpu):  # noqa: F811
     """Test HTTP client with initialized CPU docker runtime (Port: 50054)."""
     from fastapi.testclient import TestClient
 
     from nos.server.http._service import app_factory
 
     # Yield the HTTP client once the server is up and initialized
-    with TestClient(app_factory(address=f"[::]:{GRPC_TEST_PORT_GPU}")) as _client:
+    with TestClient(app_factory(address=f"{DEFAULT_GRPC_HOST}:{GRPC_TEST_PORT_GPU}")) as _client:
         yield _client
 
 
 # Needed for referencing relevant pytest fixtures
 HTTP_CLIENT_SERVER_CONFIGURATIONS = [
     # HTTP_CLIENT_WITH_LOCAL,
     # HTTP_CLIENT_WITH_CPU,
@@ -297,15 +297,15 @@
     # Wait for server to start, then start uvicorn server
     grpc_client = grpc_client_with_gpu_backend
     grpc_client.WaitForServer(timeout=180, retry_interval=5)
     logger.info("Server started!")
 
     def _run_uvicorn_server():
         uvicorn.run(
-            app_factory(address=f"[::]:{GRPC_TEST_PORT_GPU}", env="dev"),
+            app_factory(address=f"{DEFAULT_GRPC_HOST}:{GRPC_TEST_PORT_GPU}", env="dev"),
             host="localhost",
             port=HTTP_TEST_PORT,
             workers=1,
             log_level="info",
         )
 
     # Start uvicorn server
```

## Comparing `torch_nos-0.2.0b0.dist-info/LICENSE` & `torch_nos-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torch_nos-0.2.0b0.dist-info/METADATA` & `torch_nos-0.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-nos
-Version: 0.2.0b0
+Version: 0.3.0
 Summary: Nitrous Oxide for your AI Infrastructure.
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -216,19 +216,17 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8.10
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: agi-pack >=0.2.0
 Requires-Dist: cloudpickle >=2.2.1
 Requires-Dist: docker >=6.0.0
 Requires-Dist: filelock
 Requires-Dist: gitpython
@@ -370,15 +368,15 @@
 <summary> API / Usage</summary>
 <br>
 
 <b>gRPC API ⚡</b>
 ```python
 from nos.client import Client
 
-client = Client("[::]:50051")
+client = Client()
 
 model = client.Module("TinyLlama/TinyLlama-1.1B-Chat-v1.0")
 response = model.chat(message="Tell me a story of 1000 words with emojis", _stream=True)
 ```
 
 <b>REST API</b>
 ```bash
@@ -410,15 +408,15 @@
 <br>
 
 <b>gRPC API ⚡</b>
 
 ```python
 from nos.client import Client
 
-client = Client("[::]:50051")
+client = Client()
 
 sdxl = client.Module("stabilityai/stable-diffusion-xl-base-1-0")
 image, = sdxl(prompts=["hippo with glasses in a library, cartoon styling"],
               width=1024, height=1024, num_images=1)
 ```
 
 <b>REST API</b>
@@ -451,15 +449,15 @@
 <br>
 
 <b>gRPC API ⚡</b>
 
 ```python
 from nos.client import Client
 
-client = Client("[::]:50051")
+client = Client()
 
 clip = client.Module("openai/clip-vit-base-patch32")
 txt_vec = clip.encode_text(texts=["fox jumped over the moon"])
 ```
 
 <b>REST API</b>
 
@@ -492,15 +490,15 @@
 
 <b>gRPC API ⚡</b>
 
 ```python
 from pathlib import Path
 from nos.client import Client
 
-client = Client("[::]:50051")
+client = Client()
 
 model = client.Module("openai/whisper-small.en")
 with client.UploadFile(Path("audio.wav")) as remote_path:
   response = model(path=remote_path)
 # {"chunks": ...}
 ```
 
@@ -530,15 +528,15 @@
 
 <b>gRPC API ⚡</b>
 
 ```python
 from pathlib import Path
 from nos.client import Client
 
-client = Client("[::]:50051")
+client = Client()
 
 model = client.Module("yolox/medium")
 response = model(images=[Image.open("image.jpg")])
 ```
 
 <b>REST API</b>
```

## Comparing `torch_nos-0.2.0b0.dist-info/RECORD` & `torch_nos-0.3.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,87 @@
-nos/__init__.py,sha256=qNlh5FXCaooUrODrcPiHY_yK9NwtRFLCTsN4FLGRVFQ,424
-nos/constants.py,sha256=ZWv5a3CP0IqZljnPnElohGJqmvQXIDxvlfpNqlSQgQo,1951
+nos/__init__.py,sha256=YA-bFdtF2FKwtDgg_6fp1eo0148aillYHJcF-WxZET8,49
+nos/constants.py,sha256=Dwpa0Nxkb6swE3UbAyae3kZRdSyUqSaE3I8rBWFn5h0,1956
 nos/exceptions.py,sha256=i3SD26SIgCIpDq2hSJ3Tt_ECgwbK-5p3ZbjGY0lcOQw,750
 nos/logging.py,sha256=IkkbLtVKUFg6hbECKOBUUzozDdlwJ2MpmlRn6NxzbIQ,2295
 nos/protoc.py,sha256=_VoBlDRZozu1vmhnJ65SsEHOfedbHW0_SlB6NWUgI9Q,3199
-nos/telemetry.py,sha256=KclGHUUBC7x1aviM-62dUMT5SrA9IhlqY9j4Bdvw6t8,1436
-nos/version.py,sha256=jaXChwfIgwjM8CGVXQS3V5mfoUdkBU_6vPxsrLg-QJc,23
+nos/telemetry.py,sha256=uUYX8DSxMLyeJV1J9ZAVqhhn62rKU-Liyrk-qrNPE9s,1438
+nos/version.py,sha256=VrXpHDu3erkzwl_WXrqINBm9xWkcyUy53IQOj042dOs,22
 nos/catalogs/model_profile_catalog.json,sha256=fp2ec-MwGFNXoHhc4Vws1pY87TrTWr2eNypeGXLfU60,1898
 nos/cli/cli.py,sha256=H-X2g7g1qtFGHTnsmUNE-9ZnO3sC8Ys3QrI-Hty3SLc,858
 nos/cli/hub.py,sha256=apjVHOka3ltxdTZC31HSCZK47a6Ou2O5TlpzQNY_gz8,1417
-nos/cli/predict.py,sha256=acD1ZDOC-phJIKSuBzyOw8TEaNlcFT-Gq92NUozyca0,7330
+nos/cli/predict.py,sha256=O7QGF44eRvL3vEcZbOUfXPJ3PSfY8yG2dCRG0yMwUR4,7385
 nos/cli/profile.py,sha256=ZYqprxKqDMtgsu1Mi0l9a7ovXFyOUPQ7D4ShLe-uqTI,13556
-nos/cli/serve.py,sha256=MBNbneaeFFLkI3Jwv8xNSkYVTSLDMJQgJXLLOpHhixc,19110
+nos/cli/serve.py,sha256=el0FElTJ7RTSZwR34gJ65BoZWOgIKyZVMbNkdc5Mk2A,19109
 nos/cli/system.py,sha256=oeAN6WA1IdhlIR89cnW1xFhd8HEAZLl15TcwucsojSI,1838
 nos/cli/utils.py,sha256=uR1lGZyyDEuflNvxKuAmVUP-DTE55PzZL5c0c3l2h4U,425
-nos/cli/templates/docker-compose.serve.yml.j2,sha256=CnD0dlpLhV79En_aC0pMhC1_DaheiBg779Qj1CV0nwM,1836
+nos/cli/templates/docker-compose.serve.yml.j2,sha256=6nM1koOgvIYridugIpCGWKdB9KLCSMeso4cbhsV5pOg,1847
 nos/client/__init__.py,sha256=cGqTR-ItKRYX-3FNxc7EL6ex0gAuvYLev8jSJrVZhOk,398
-nos/client/grpc.py,sha256=8hQgZ12ZZrhgv6t-XmHZ6ceK8LjaSxoeE2Ivbuuildk,30281
-nos/common/__init__.py,sha256=-GcgzkFF8jP5bGOK0Y8AANC2wtiRIbtY2EkcGS3ZcaM,3094
+nos/client/grpc.py,sha256=BIIeW3x5EELC48HKkPLEKZHggV85q5QIcE0yuI9aABM,30496
+nos/common/__init__.py,sha256=0tdWq5caJSqwD1qHnRKN07E9DDzcPVPVBtBSINv6aQo,3074
 nos/common/cloudpickle.py,sha256=2VBtGaLHbVtKg9ICT-xUITweHQCd6PxsFobDKwSYE2I,204
 nos/common/exceptions.py,sha256=zP8v9dm4gFTLoCr6bKHS1TuIm2CcF4h51hJmSrp7e3s,906
 nos/common/git.py,sha256=cd-m0WkUEhVDdqNdcUAg_hVbX4SuFkev0ONkPebLe1I,5154
 nos/common/helpers.py,sha256=6wb1I6XlY2cvWG_i5LHSRbrwpRwsX7rKaqgRhginTSE,1028
 nos/common/metaclass.py,sha256=Yhicnnff8uppLxjF63rqvSnS5AxMIfTDfOsqztJMiE8,499
 nos/common/profiler.py,sha256=IBoK0fsiAo5HAEV3vdSEZxll83o4Bl_PQTnh3uuR1Uc,20811
 nos/common/runtime.py,sha256=yXPFjp4oeB-hno5Yuzkx-_B7gRER9xZRf3L32bpE-gA,805
-nos/common/shm.py,sha256=k5WLv4vUVifIRyhGQPT6LAI9IhmuU5W6Azukns0u_PE,11842
-nos/common/spec.py,sha256=ARJ-CyJY8Cv8khGen8OLrEUyYz53LbdTSVkcWULJ5s0,31844
+nos/common/shm.py,sha256=q9bjTF-kcf3KzJVFu7gni6-lyAkSbjfpidGIbjFpu8I,11856
+nos/common/spec.py,sha256=likFmDNE0fS3PnSTAdMA76sJzC8ZgKiIX7hcv0xWktE,26198
 nos/common/system.py,sha256=KPPsH36RVZEMRZ9vbi0ty3927kfpnRDg8hzBQ2y6IR8,7930
 nos/common/tasks.py,sha256=b_7DMIV7rlhWOgNO1jx0_HSNTPX6MZsOCfASv8Laakw,830
 nos/common/types.py,sha256=kZYYI6b-u1xvOsiM0e02tENIQZwauCGcCcKwZXC7ZY8,6117
 nos/common/io/__init__.py,sha256=XLg1aKxI3GKObzvb437Ht0PId1mvrA9tmiyHFMg04Yk,1465
 nos/common/io/video/base.py,sha256=rAEBnj-LqkeqlCAXqGbAP49zKL3Q-m3sHhtLo6vh2ak,1050
 nos/common/io/video/opencv.py,sha256=ZWqRVIRrszKovVGMp95ydKMXuQvKRW0IyEFiYNgv6cY,8777
 nos/executors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nos/executors/ray.py,sha256=9t13Gf64WzPLQ0TmDZi7irDz0ydYpzY34Sapzi8VQgg,9283
-nos/externals/streamlink.py,sha256=ORONhmV67Ksr2V0V_ZsDpXmxKdcQyjmT74-aMhquQ3s,2229
 nos/hub/__init__.py,sha256=zWr4NK2ojFR9EjwUxJ1ppM6s_1GlrZrHNuKBiv2S8RA,15315
 nos/hub/config.py,sha256=bAWxyY4AqeUHMoqggD2mfYoIYQ1YGPV_DOy75Md8nCE,1756
 nos/hub/hf.py,sha256=iiVjrU-Pyi8D4VL-C2nnSelq4kbraDkc0utiNISNL4s,538
 nos/managers/__init__.py,sha256=ZLKQSo3Wj5B2fFyUiTTQlgQ97KWcpxJZtO27DseVbsU,59
 nos/managers/model.py,sha256=HoQjAWrKltuhfyVg4yVfb4IrHlEPVbtD2pCOQ3Udo5Y,24163
 nos/managers/pool.py,sha256=KvjfobpzTiMtDxVRAof-hl3ji_yerVMVYwJ48PxdH7E,4738
-nos/models/__init__.py,sha256=v65W57mBYCrJ26K5y6JPGQ2mbODJMPJRSxG6vrHL-vU,936
+nos/models/__init__.py,sha256=mqs71c2c6FJfp9PUaNgzLMH3EGloDIRQ8H6hfZzL0ZI,773
 nos/models/_noop.py,sha256=ZS5UGQKB7YH1EyYUc84P2wcEoL81D_kcSZqXZnUdVq0,3138
 nos/models/blip.py,sha256=pjM6OGgMiwVKd7iGFjULEYJzJ_JcYOTzajHj8bv7Zko,3841
 nos/models/clip.py,sha256=tPD6V4rnpTlM25mBu7MhuaIztUj3DXi533Tyhic10Co,4220
 nos/models/faster_rcnn.py,sha256=w8aERm9gCbakl-w2VJlWKAIe4vbwBt1l_oozygiB0ls,2830
 nos/models/llm.py,sha256=mZOUbuk6GI187Ne2Sj63y1GG-QCDg8SSWVppmm0A16o,7693
 nos/models/monodepth.py,sha256=bzQOJT1e8sARtKkUsZEe16qSL_rhacrh3Pn8YulX8II,2875
 nos/models/owlvit.py,sha256=-dqULYIjfr0Vg_kjdbtIjTin2wBTaumfo1Zu7vhsoVo,2939
 nos/models/sam.py,sha256=TugDhCGYrgqGDwVp-0UIHPT-L-Y2HnleuhWRA995sK4,2618
 nos/models/stable_diffusion.py,sha256=eKnlnHafC8r-dde8YghroNKMRPIwGu21ga1K9KJirjc,5195
 nos/models/tts.py,sha256=r7mzEbmY3QULZkYWAavwnm0a491nj7aIvYA4kzXXry4,1618
 nos/models/whisper.py,sha256=kIBGgwIYV4hnnYQjS0ikf0uWv4C6Ee8tImR-AurfjYQ,4296
 nos/models/yolox.py,sha256=FCLBOpyK0P0_oMzbRstH9zM_KylY1HGrPmMdq8LnBcY,6462
 nos/models/dreambooth/dreambooth.py,sha256=NvBj8KN095hQ9oGvze4c3ueFMBZGiKbv5EreGTzZk0A,3232
 nos/models/dreambooth/hub.py,sha256=SsnWLYfo4fZel_OaAk-bnxXaLhjWWP0n0ibal6nLUnE,4866
-nos/models/openmmlab/__init__.py,sha256=rAbi8MdemVgxFMFm6n1w37yyZSGSRgAAxR86no5P-QY,25
 nos/models/openmmlab/hub.py,sha256=OpxFmhjGDHXJG2BK30oBwZ97b4Ck5T0WhZYyiS9RrNo,4857
 nos/models/openmmlab/mmdetection.py,sha256=uDjsBRwtaUxpo6BkbKSIHGFHQh4b6P1ErveUi7jjg7M,6079
 nos/models/super_resolution/__init__.py,sha256=BRozsVjhaiotLpEkLwANKNPIhSdCsmxp-ufHYhjFvHs,2130
 nos/models/super_resolution/config.py,sha256=pwMDwMuK3TKfYkX3UDV6uiwfNZ_cPjtfgIMrhrBxgXc,472
 nos/models/super_resolution/ldm.py,sha256=YaiT0Mc2yAuHgW4FLg7O5o4yc7jA9rIodceM8EzJwCA,2199
 nos/models/super_resolution/swin2sr.py,sha256=I74lsFyYZLuasut_E9CD4kAxmSBnVnVBS8GnXafSK7w,1865
 nos/neuron/device.py,sha256=UhDtot6HG3B1z4oa780juuEWVUsnd2uKU6NMYLAv9Vo,1284
 nos/proto/nos_service.proto,sha256=eue7x4XWSEJCI7CQFVlmnwtmYGKoSyCnpo58rFkcths,1895
-nos/server/__init__.py,sha256=8o9wTyD4DvdntWHRedVGCoszjt7ON6-LgodlRcQXZSM,10483
+nos/server/__init__.py,sha256=WwaMd0JAwWpIrpWOUh9V2jUCqyKrRy1EpVDGyR-D6p4,10464
 nos/server/_docker.py,sha256=hXRH1m_iI5v8z60n36cDdMbxs_I_uJ6517paFPwQJLw,7341
 nos/server/_runtime.py,sha256=lyIb9NS3ceYUxasvXwadU_43PyKNOIuSKz5KAcIhdzY,9632
 nos/server/_service.py,sha256=CELEBP110vyhwwqmjZAPD6iwA8i9LtT6JkjRRzv2OxA,20201
-nos/server/http/__init__.py,sha256=3HBNsYRdbgLgn6mug36-UxeMxtKa81ZDbqT_54ktng0,83
-nos/server/http/_service.py,sha256=h1Puk1aAQDWE0VtWmtmafmBbIYu4FH6Dxv0AjtW3uT4,20019
+nos/server/http/_exceptions.py,sha256=87nFBrrVYbCblvgGzBrwo4Nl4lJZ1Fgl1P7GA7u4Tio,1097
+nos/server/http/_security.py,sha256=3Uh9D6fz35GOnCPPQ9NhlwS56_eTnZ_sCCbELTDFt6o,1066
+nos/server/http/_service.py,sha256=SsENtUGCz9E6qrfJC0-3Q1J0nddMOUYOmWc_Ee7DTcg,20644
 nos/server/http/_utils.py,sha256=x6ndk5ONVxuoC9GKQD25chXvHMa3hbe_qlyzjNaXMNo,2865
 nos/server/http/integrations/openai/models.py,sha256=FYCdFLDDL2DPKB6bz6ZzNCz_C4p6H3Geqr-6rjVeNgk,4223
 nos/test/benchmark.py,sha256=b_QMHfStY5iRjHGPZwaY7VrXzy_VeFKfjld9UEVbn-g,373
-nos/test/conftest.py,sha256=3eama-JQx3R92n3MltQA1FkO7KF2ih3IV7wog8jsSYU,10761
+nos/test/conftest.py,sha256=sTOUS6_QW2UNTLx-YUeqaJ8zsI-_aCbfk0WmxmC2gyg,10900
 nos/test/utils.py,sha256=Lal3t2U-B5YgGzvKynTMoWN9Z12Jok52tlAt_IG2T7E,2749
 nos/test/test_data/test.jpg,sha256=jpqxNdp-rKve7u4Rukt7zdG_rBKM-Sqd6cefmEBgrh4,259865
 nos/test/test_data/test.mp4,sha256=uDyQB1PSe7jQ1QvON3EReYUGtQYvh69w9RBzA5ILun8,300601
 nos/test/test_data/test_speech.flac,sha256=Y6Sx5MHcZVrHCWH_v1GKzSSd8jfloBUvqumkqDaUlxU,1152693
 nos/test/test_data/hub/custom_model/models/model.py,sha256=D4pGZtlMBN8mvbgyKSfmDgUcEmCnAsr95jGUfG9AtWY,178
-nos-profiling-catalogs/nos-profile--0-1-4a--20240122--nvidia-geforce-rtx-2080.json,sha256=Aoe0GM0D4MY7mRmY_95qqJi6j4y4m5J_MRhMSAaW6RI,2101
-nos-profiling-catalogs/nos-profile--0-1-5--20240123--nvidia-geforce-rtx-2080.json,sha256=YeGfIx29NGhtuw6oJSvRgZTJq5Wo-Ig13LBipQzvmhU,2086
-scripts/nos_bot.py,sha256=JjbzNCT9caxk2wYnKEk1ZUehVO-enzdiwHPGqAeTYbg,3006
-torch_nos-0.2.0b0.dist-info/LICENSE,sha256=Sx_bJsho4SrloBQw1plyToriX8KcfYwQ2RCBVd_UAjs,11355
-torch_nos-0.2.0b0.dist-info/METADATA,sha256=W-aVsDnMVlvkolaI5lguST160OZilxHs1r697CW4LWg,26900
-torch_nos-0.2.0b0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-torch_nos-0.2.0b0.dist-info/entry_points.txt,sha256=m5LWTBk_24bET1ibsIwOn_g3YUEM1ZSjTGpNkECt3iI,135
-torch_nos-0.2.0b0.dist-info/top_level.txt,sha256=1rEZQcaUw9uO6bbe6_8o_XGGTRnYsJeIeBhdfZen8po,74
-torch_nos-0.2.0b0.dist-info/RECORD,,
+torch_nos-0.3.0.dist-info/LICENSE,sha256=Sx_bJsho4SrloBQw1plyToriX8KcfYwQ2RCBVd_UAjs,11355
+torch_nos-0.3.0.dist-info/METADATA,sha256=tpn-cVcknLyt48OdLtvLpaNOrO9ifCmGZG8sOxI3O4E,26736
+torch_nos-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+torch_nos-0.3.0.dist-info/entry_points.txt,sha256=m5LWTBk_24bET1ibsIwOn_g3YUEM1ZSjTGpNkECt3iI,135
+torch_nos-0.3.0.dist-info/top_level.txt,sha256=RgOntmzdTkyrY-Fj9H6bSke7af3bHLscoZnK1-7Aa8o,12
+torch_nos-0.3.0.dist-info/RECORD,,
```

