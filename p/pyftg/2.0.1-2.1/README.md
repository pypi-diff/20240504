# Comparing `tmp/pyftg-2.0.1.tar.gz` & `tmp/pyftg-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftg-2.0.1.tar", last modified: Mon Feb 19 04:01:31 2024, max compression
+gzip compressed data, was "pyftg-2.1.tar", last modified: Sat May  4 15:51:26 2024, max compression
```

## Comparing `pyftg-2.0.1.tar` & `pyftg-2.1.tar`

### file list

```diff
@@ -1,56 +1,85 @@
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-02-19 04:01:31.774979 pyftg-2.0.1/
--rw-r--r--   0 staciiaz   (501) staff       (20)     1072 2024-02-18 17:20:43.000000 pyftg-2.0.1/LICENSE
--rw-r--r--   0 staciiaz   (501) staff       (20)     1423 2024-02-19 04:01:31.774819 pyftg-2.0.1/PKG-INFO
--rw-r--r--   0 staciiaz   (501) staff       (20)      821 2024-02-18 17:20:43.000000 pyftg-2.0.1/README.md
--rw-r--r--   0 staciiaz   (501) staff       (20)      556 2024-02-19 04:01:27.000000 pyftg-2.0.1/pyproject.toml
--rw-r--r--   0 staciiaz   (501) staff       (20)       38 2024-02-19 04:01:31.775010 pyftg-2.0.1/setup.cfg
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-02-19 04:01:31.770503 pyftg-2.0.1/src/
--rw-r--r--   0 staciiaz   (501) staff       (20)     1525 2023-10-08 11:53:34.000000 pyftg-2.0.1/src/Main_Capture.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     3230 2023-10-08 07:42:51.000000 pyftg-2.0.1/src/Main_Collector.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1643 2023-10-17 07:13:15.000000 pyftg-2.0.1/src/Main_FDG.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-02-19 04:01:31.771045 pyftg-2.0.1/src/pyftg/
--rw-r--r--   0 staciiaz   (501) staff       (20)      190 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/__init__.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     2431 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/ai_controller.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-02-19 04:01:31.771845 pyftg-2.0.1/src/pyftg/aiinterface/
--rw-r--r--   0 staciiaz   (501) staff       (20)       80 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/aiinterface/__init__.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      814 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/aiinterface/ai_interface.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     6224 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/aiinterface/command_center.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-02-19 04:01:31.772057 pyftg-2.0.1/src/pyftg/aio/
--rw-r--r--   0 staciiaz   (501) staff       (20)     2417 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/aio/ai_controller.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     2346 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/aio/gateway.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-02-19 04:01:31.772711 pyftg-2.0.1/src/pyftg/enum/
--rw-r--r--   0 staciiaz   (501) staff       (20)       84 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/enum/__init__.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1103 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/enum/action.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      116 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/enum/data_flag.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      129 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/enum/flag.py
--rw-r--r--   0 staciiaz   (501) staff       (20)       97 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/enum/state.py
--rw-r--r--   0 staciiaz   (501) staff       (20)       79 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/enum/status_code.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     2208 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/gateway.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     2188 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/observer_gateway.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      445 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/observer_handler.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-02-19 04:01:31.773373 pyftg-2.0.1/src/pyftg/protoc/
--rw-r--r--   0 staciiaz   (501) staff       (20)        0 2023-04-11 11:53:26.000000 pyftg-2.0.1/src/pyftg/protoc/__init__.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     3459 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/protoc/enum_pb2.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      159 2023-04-11 11:53:26.000000 pyftg-2.0.1/src/pyftg/protoc/enum_pb2_grpc.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     5607 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/protoc/message_pb2.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      159 2023-04-11 11:53:26.000000 pyftg-2.0.1/src/pyftg/protoc/message_pb2_grpc.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     4715 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/protoc/service_pb2.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     8467 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/protoc/service_pb2_grpc.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-02-19 04:01:31.774531 pyftg-2.0.1/src/pyftg/struct/
--rw-r--r--   0 staciiaz   (501) staff       (20)      388 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/struct/__init__.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1366 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/struct/attack_data.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      467 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/struct/audio_data.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1398 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/struct/character_data.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      197 2023-04-11 11:53:26.000000 pyftg-2.0.1/src/pyftg/struct/fft_data.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1172 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/struct/frame_data.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      556 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/struct/game_data.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      213 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/struct/hit_area.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      518 2023-04-11 11:53:26.000000 pyftg-2.0.1/src/pyftg/struct/key.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      243 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/struct/round_result.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      285 2024-02-18 17:20:43.000000 pyftg-2.0.1/src/pyftg/struct/screen_data.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-02-19 04:01:31.774672 pyftg-2.0.1/src/pyftg.egg-info/
--rw-r--r--   0 staciiaz   (501) staff       (20)     1423 2024-02-19 04:01:31.000000 pyftg-2.0.1/src/pyftg.egg-info/PKG-INFO
--rw-r--r--   0 staciiaz   (501) staff       (20)     1274 2024-02-19 04:01:31.000000 pyftg-2.0.1/src/pyftg.egg-info/SOURCES.txt
--rw-r--r--   0 staciiaz   (501) staff       (20)        1 2024-02-19 04:01:31.000000 pyftg-2.0.1/src/pyftg.egg-info/dependency_links.txt
--rw-r--r--   0 staciiaz   (501) staff       (20)       35 2024-02-19 04:01:31.000000 pyftg-2.0.1/src/pyftg.egg-info/requires.txt
--rw-r--r--   0 staciiaz   (501) staff       (20)       43 2024-02-19 04:01:31.000000 pyftg-2.0.1/src/pyftg.egg-info/top_level.txt
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.508325 pyftg-2.1/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1072 2024-02-18 17:20:43.000000 pyftg-2.1/LICENSE
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1634 2024-05-04 15:51:26.508158 pyftg-2.1/PKG-INFO
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1031 2024-04-24 09:41:02.000000 pyftg-2.1/README.md
+-rw-r--r--   0 staciiaz   (501) staff       (20)      573 2024-05-04 15:51:19.000000 pyftg-2.1/pyproject.toml
+-rw-r--r--   0 staciiaz   (501) staff       (20)       38 2024-05-04 15:51:26.508359 pyftg-2.1/setup.cfg
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.502121 pyftg-2.1/src/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     3407 2024-04-13 17:15:22.000000 pyftg-2.1/src/DisplayInfo.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1858 2024-04-10 19:07:27.000000 pyftg-2.1/src/KickAI.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1525 2023-10-08 11:53:34.000000 pyftg-2.1/src/Main_Capture.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     3230 2023-10-08 07:42:51.000000 pyftg-2.1/src/Main_Collector.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1643 2023-10-17 07:13:15.000000 pyftg-2.1/src/Main_FDG.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1175 2024-04-11 13:38:52.000000 pyftg-2.1/src/Main_PyAIvsPyAI.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1134 2024-04-11 13:51:53.000000 pyftg-2.1/src/Main_SinglePyAI.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      864 2024-04-24 09:42:13.000000 pyftg-2.1/src/Main_SoundAI.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      765 2024-04-24 09:42:13.000000 pyftg-2.1/src/TestSoundAI.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.502230 pyftg-2.1/src/pyftg/
+-rw-r--r--   0 staciiaz   (501) staff       (20)      381 2024-04-24 09:41:02.000000 pyftg-2.1/src/pyftg/__init__.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.503151 pyftg-2.1/src/pyftg/aiinterface/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1237 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/aiinterface/ai_interface.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     6231 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/aiinterface/command_center.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      757 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/aiinterface/soundgenai_interface.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.500249 pyftg-2.1/src/pyftg/grpc/
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.503364 pyftg-2.1/src/pyftg/grpc/asyncio/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2805 2024-04-24 09:41:02.000000 pyftg-2.1/src/pyftg/grpc/asyncio/ai_controller.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2568 2024-04-11 13:33:38.000000 pyftg-2.1/src/pyftg/grpc/asyncio/gateway.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.503834 pyftg-2.1/src/pyftg/grpc/threading/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2742 2024-04-24 09:41:02.000000 pyftg-2.1/src/pyftg/grpc/threading/ai_controller.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2348 2024-04-11 13:33:38.000000 pyftg-2.1/src/pyftg/grpc/threading/gateway.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2508 2024-04-11 13:33:38.000000 pyftg-2.1/src/pyftg/grpc/threading/observer_gateway.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      603 2024-04-11 13:33:38.000000 pyftg-2.1/src/pyftg/grpc/threading/observer_handler.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.503946 pyftg-2.1/src/pyftg/interfaces/
+-rw-r--r--   0 staciiaz   (501) staff       (20)      541 2024-04-11 13:33:38.000000 pyftg-2.1/src/pyftg/interfaces/async_gateway.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.505140 pyftg-2.1/src/pyftg/models/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     5349 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/models/attack_data.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1346 2024-04-13 17:13:16.000000 pyftg-2.1/src/pyftg/models/audio_data.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      346 2024-04-12 17:24:08.000000 pyftg-2.1/src/pyftg/models/base_model.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     4873 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/models/character_data.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.505958 pyftg-2.1/src/pyftg/models/enums/
+-rw-r--r--   0 staciiaz   (501) staff       (20)        0 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/enums/__init__.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1847 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/enums/action.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      121 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/enums/data_flag.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      153 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/models/enums/flag.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1111 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/enums/int_action.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      105 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/enums/int_state.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      346 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/enums/state.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      100 2024-04-11 13:33:38.000000 pyftg-2.1/src/pyftg/models/enums/status_code.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      953 2024-04-13 17:13:16.000000 pyftg-2.1/src/pyftg/models/fft_data.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2849 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/models/frame_data.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1482 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/game_data.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      990 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/hit_area.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1427 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/key.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1136 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/round_result.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      851 2024-04-13 17:13:16.000000 pyftg-2.1/src/pyftg/models/screen_data.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.506730 pyftg-2.1/src/pyftg/protoc/
+-rw-r--r--   0 staciiaz   (501) staff       (20)        0 2023-04-11 11:53:26.000000 pyftg-2.1/src/pyftg/protoc/__init__.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/__init__.pyi
+-rw-r--r--   0 staciiaz   (501) staff       (20)     3286 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/enum_pb2.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)       87 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/enum_pb2_grpc.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     5662 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/message_pb2.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)       87 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/message_pb2_grpc.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     4602 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/service_pb2.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     6775 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/service_pb2_grpc.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.500735 pyftg-2.1/src/pyftg/socket/
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.507053 pyftg-2.1/src/pyftg/socket/asyncio/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     3144 2024-04-24 09:41:02.000000 pyftg-2.1/src/pyftg/socket/asyncio/ai_controller.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2872 2024-04-12 17:24:08.000000 pyftg-2.1/src/pyftg/socket/asyncio/gateway.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2649 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/socket/asyncio/generative_sound_gateway.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.507251 pyftg-2.1/src/pyftg/socket/threading/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     3133 2024-04-24 09:41:02.000000 pyftg-2.1/src/pyftg/socket/threading/ai_controller.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2763 2024-04-12 17:24:08.000000 pyftg-2.1/src/pyftg/socket/threading/gateway.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.507456 pyftg-2.1/src/pyftg/socket/utils/
+-rw-r--r--   0 staciiaz   (501) staff       (20)      642 2024-04-12 17:24:08.000000 pyftg-2.1/src/pyftg/socket/utils/asyncio.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      508 2024-04-12 17:24:08.000000 pyftg-2.1/src/pyftg/socket/utils/threading.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.507854 pyftg-2.1/src/pyftg/utils/
+-rw-r--r--   0 staciiaz   (501) staff       (20)      417 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/utils/gateway.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      430 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/utils/logging.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      258 2024-04-24 09:41:02.000000 pyftg-2.1/src/pyftg/utils/protobuf.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      252 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/utils/resource_loader.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.507995 pyftg-2.1/src/pyftg.egg-info/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1634 2024-05-04 15:51:26.000000 pyftg-2.1/src/pyftg.egg-info/PKG-INFO
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2073 2024-05-04 15:51:26.000000 pyftg-2.1/src/pyftg.egg-info/SOURCES.txt
+-rw-r--r--   0 staciiaz   (501) staff       (20)        1 2024-05-04 15:51:26.000000 pyftg-2.1/src/pyftg.egg-info/dependency_links.txt
+-rw-r--r--   0 staciiaz   (501) staff       (20)       53 2024-05-04 15:51:26.000000 pyftg-2.1/src/pyftg.egg-info/requires.txt
+-rw-r--r--   0 staciiaz   (501) staff       (20)      119 2024-05-04 15:51:26.000000 pyftg-2.1/src/pyftg.egg-info/top_level.txt
```

### Comparing `pyftg-2.0.1/LICENSE` & `pyftg-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyftg-2.0.1/README.md` & `pyftg-2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # pyftg
 
 An interface for implementing python AI in DareFightingICE
 
-**Note:** Version 2.0 is the latest version compatible with the legacy [FightingICE](https://github.com/TeamFightingICE/FightingICE). Future versions will only support [DareFightingICE-Unity](https://github.com/TeamFightingICE/DareFightingICE-Unity).
+**Note:** Version 2.0 is the latest version compatible with the legacy [FightingICE](https://github.com/TeamFightingICE/FightingICE). Version 2.1 and later will only support [DareFightingICE-Unity](https://github.com/TeamFightingICE/DareFightingICE-Unity).
 
 First, install `pyftg` with pip.
 ```
 pip install pyftg
 ```
 
 Initiate `Gateway` for connecting to DareFightingICE platform.
 ```
-from pyftg.gateway import Gateway
-gateway = Gateway(port=50051)
+from pyftg.utils.gateway import get_async_gateway
+gateway = get_async_gateway(port=50051)
 ```
 
 Construct an agent and register it to gateway and then run the game by using following code.
 ```
-agent = KickAI()
-gateway.register_ai("KickAI", agent)
-gateway.run_game(["ZEN", "ZEN"], ["KickAI", "MctsAi23i"], 1)
+agent1 = KickAI()
+agent2 = DisplayInfo()
+gateway.register_ai("KickAI", agent1)
+gateway.register_ai("DisplayInfo", agent2)
+await gateway.run_game(["ZEN", "ZEN"], ["KickAI", "DisplayInfo"], game_num)
 ```
 
 After all the process are done, please also close the gateway.
 ```
-gateway.close()
+await gateway.close()
 ```
+
+Please refer to the examples provided in the `examples` directory for more information.
```

### Comparing `pyftg-2.0.1/pyproject.toml` & `pyftg-2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [project]
 name = "pyftg"
-version = "2.0.1"
+version = "2.1"
 authors = [
   { name="TeamFightingICE" },
 ]
 description = "An interface for implementing python AI in DareFightingICE"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
-  'grpcio',
-  'grpcio-tools',
-  'protobuf',
-  'numpy',
+  'grpcio ~= 1.62.1',
+  'grpcio-tools ~= 1.62.1',
+  'protobuf ~= 4.25.3',
 ]
 
 [project.urls]
 Homepage = "https://github.com/TeamFightingICE/pyftg"
 Issues = "https://github.com/TeamFightingICE/pyftg/issues"
```

### Comparing `pyftg-2.0.1/src/Main_Capture.py` & `pyftg-2.1/src/Main_Capture.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.0.1/src/Main_Collector.py` & `pyftg-2.1/src/Main_Collector.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.0.1/src/Main_FDG.py` & `pyftg-2.1/src/Main_FDG.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.0.1/src/pyftg/ai_controller.py` & `pyftg-2.1/src/pyftg/grpc/asyncio/ai_controller.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,62 @@
-from threading import Thread
+import logging
+from typing import AsyncGenerator
 
-from .aiinterface.ai_interface import AIInterface
-from .enum.flag import Flag
-from .protoc import message_pb2, service_pb2, service_pb2_grpc
-from .struct import (AudioData, FrameData, GameData, Key, RoundResult,
-                     ScreenData)
+from google.protobuf.message import Message
 
+from pyftg.aiinterface.ai_interface import AIInterface
+from pyftg.models.audio_data import AudioData
+from pyftg.models.enums.flag import Flag
+from pyftg.models.frame_data import FrameData
+from pyftg.models.game_data import GameData
+from pyftg.models.key import Key
+from pyftg.models.round_result import RoundResult
+from pyftg.models.screen_data import ScreenData
+from pyftg.protoc import service_pb2, service_pb2_grpc
+from pyftg.utils.protobuf import convert_key_to_proto
 
-class AIController(Thread):
+logger = logging.getLogger(__name__)
+
+
+class AIController():
     def __init__(self, stub: service_pb2_grpc.ServiceStub, ai: AIInterface, player_number: bool):
-        Thread.__init__(self)
         self.stub = stub
         self.ai = ai
         self.player_number = player_number
     
-    def initialize_rpc(self):
+    async def initialize_rpc(self) -> str:
         request = service_pb2.InitializeRequest(player_number=self.player_number, player_name=self.ai.name(), is_blind=self.ai.is_blind())
-        response = self.stub.Initialize(request)
-        self.player_uuid: str = response.player_uuid
+        response = await self.stub.Initialize(request)
+        return response.player_uuid
 
-    def participate_rpc(self):
-        request = service_pb2.ParticipateRequest(player_uuid=self.player_uuid)
+    async def participate_rpc(self, player_uuid: str) -> AsyncGenerator[Message, None]:
+        request = service_pb2.ParticipateRequest(player_uuid=player_uuid)
         return self.stub.Participate(request)
     
-    def input_rpc(self, key: Key):
-        grpc_key = message_pb2.GrpcKey(A=key.A, B=key.B, C=key.C, U=key.U, D=key.D, L=key.L, R=key.R)
-        self.stub.Input(service_pb2.PlayerInput(player_uuid=self.player_uuid, input_key=grpc_key))
+    async def input_rpc(self, player_uuid: str, key: Key) -> None:
+        proto_key = convert_key_to_proto(key)
+        await self.stub.Input(service_pb2.PlayerInput(player_uuid=player_uuid, input_key=proto_key))
     
-    def run(self):
-        self.initialize_rpc()
-        for state in self.participate_rpc():
+    async def run(self):
+        player_uuid = await self.initialize_rpc()
+        grpc_stream_call = await self.participate_rpc(player_uuid)
+        async for state in grpc_stream_call:
             flag = Flag(state.state_flag)
             if flag is Flag.INITIALIZE:
-                self.ai.initialize(GameData(state.game_data), self.player_number)
+                self.ai.initialize(GameData.from_proto(state.game_data), self.player_number)
             elif flag is Flag.PROCESSING:
-                frame_data = FrameData(None if not state.HasField("frame_data") else state.frame_data)
-
                 if state.HasField("non_delay_frame_data"):
-                    self.ai.get_non_delay_frame_data(FrameData(state.non_delay_frame_data))
-
-                self.ai.get_information(frame_data, state.is_control)
+                    self.ai.get_non_delay_frame_data(FrameData.from_proto(state.non_delay_frame_data))
 
                 if state.HasField("screen_data"):
-                    self.ai.get_screen_data(ScreenData(state.screen_data))
+                    self.ai.get_screen_data(ScreenData.from_proto(state.screen_data))
 
-                if state.HasField("audio_data"):
-                    self.ai.get_audio_data(AudioData(state.audio_data))
+                self.ai.get_information(FrameData.from_proto(state.frame_data), state.is_control)
+                self.ai.get_audio_data(AudioData.from_proto(state.audio_data))
                     
                 self.ai.processing()
-                self.input_rpc(self.ai.input())
+                await self.input_rpc(player_uuid, self.ai.input())
             elif flag is Flag.ROUND_END:
-                self.ai.round_end(RoundResult(state.round_result))
+                self.ai.round_end(RoundResult.from_proto(state.round_result))
             elif flag is Flag.GAME_END:
-                self.ai.round_end(RoundResult(state.round_result))
+                self.ai.round_end(RoundResult.from_proto(state.round_result))
                 self.ai.game_end()
```

### Comparing `pyftg-2.0.1/src/pyftg/aiinterface/command_center.py` & `pyftg-2.1/src/pyftg/aiinterface/command_center.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from ..struct.frame_data import FrameData
-from ..struct.key import Key
+from pyftg.models.frame_data import FrameData
+from pyftg.models.key import Key
 
 
 class CommandCenter:
     def __init__(self):
-        self.skill_key: 'list[Key]' = []
-        self.frame_data = FrameData()
-        self.player_number = True
+        self.skill_key: list[Key] = []
+        self.frame_data: FrameData = None
+        self.player_number = False
 
     def command_call(self, str):
         if not self.skill_key:
             self.action_to_command(str)
 
     def action_to_command(self, str: str):
         if str == "FORWARD_WALK":
@@ -148,24 +148,24 @@
 
     def get_skill_key(self) -> Key:
         if self.get_skill_flag():
             return self.skill_key.pop(0)
         else:
             return Key()
 
-    def get_skill_keys(self) -> 'list[Key]':
+    def get_skill_keys(self) -> list[Key]:
         return self.skill_key
 
     def skill_cancel(self):
         self.skill_key.clear()
 
     def is_player_number(self) -> bool:
         return self.player_number
 
-    def reverse_key(self, commands: 'list[str]'):
+    def reverse_key(self, commands: list[str]):
         buffer = [0]*len(commands)
         for i in range(len(commands)):
             if commands[i] == "L" or commands[i] == "4":
                 buffer[i] = "6"
             elif commands[i] == "R" or commands[i] == "6":
                 buffer[i] = "4"
             elif commands[i] == "LD" or commands[i] == "1":
```

### Comparing `pyftg-2.0.1/src/pyftg/aio/ai_controller.py` & `pyftg-2.1/src/pyftg/socket/threading/ai_controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,77 @@
-from ..aiinterface import AIInterface
-from ..enum.flag import Flag
-from ..protoc import message_pb2, service_pb2, service_pb2_grpc
-from ..struct import (AudioData, FrameData, GameData, Key, RoundResult,
-                      ScreenData)
-
-
-class AIController():
-    def __init__(self, stub: service_pb2_grpc.ServiceStub, ai: AIInterface, player_number: bool):
-        self.stub = stub
+import logging
+import socket
+from threading import Thread
+
+from google.protobuf.message import Message
+
+from pyftg.aiinterface.ai_interface import AIInterface
+from pyftg.models.audio_data import AudioData
+from pyftg.models.enums.flag import Flag
+from pyftg.models.frame_data import FrameData
+from pyftg.models.game_data import GameData
+from pyftg.models.key import Key
+from pyftg.models.round_result import RoundResult
+from pyftg.models.screen_data import ScreenData
+from pyftg.protoc import service_pb2
+from pyftg.socket.utils.threading import recv_data, send_data
+from pyftg.utils.protobuf import convert_key_to_proto
+
+logger = logging.getLogger(__name__)
+
+CLOSE = b'\x00'
+PROCESSING = b'\x01'
+
+
+class AIController(Thread):
+    def __init__(self, host: str, port: int, ai: AIInterface, player_number: bool):
+        Thread.__init__(self)
+        self.host = host
+        self.port = port
         self.ai = ai
         self.player_number = player_number
     
-    async def initialize_rpc(self):
-        request = service_pb2.InitializeRequest(player_number=self.player_number, player_name=self.ai.name(), is_blind=self.ai.is_blind())
-        response = await self.stub.Initialize(request)
-        self.player_uuid: str = response.player_uuid
-
-    async def participate_rpc(self):
-        request = service_pb2.ParticipateRequest(player_uuid=self.player_uuid)
-        return self.stub.Participate(request)
-    
-    async def input_rpc(self, key: Key):
-        grpc_key = message_pb2.GrpcKey(A=key.A, B=key.B, C=key.C, U=key.U, D=key.D, L=key.L, R=key.R)
-        await self.stub.Input(service_pb2.PlayerInput(player_uuid=self.player_uuid, input_key=grpc_key))
-    
-    async def run(self):
-        await self.initialize_rpc()
-        async for state in await self.participate_rpc():
-            flag = Flag(state.state_flag)
-            if flag is Flag.INITIALIZE:
-                self.ai.initialize(GameData(state.game_data), self.player_number)
-            elif flag is Flag.PROCESSING:
-                frame_data = FrameData(None if not state.HasField("frame_data") else state.frame_data)
-
-                if state.HasField("non_delay_frame_data"):
-                    self.ai.get_non_delay_frame_data(FrameData(state.non_delay_frame_data))
-
-                self.ai.get_information(frame_data, state.is_control)
+    def initialize(self) -> None:
+        self.client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.client.connect((self.host, self.port))
+        request: Message = service_pb2.InitializeRequest(player_number=self.player_number, player_name=self.ai.name(), is_blind=self.ai.is_blind())
+        send_data(self.client, b'\x01', with_header=False)  # 1: Initialize
+        send_data(self.client, request.SerializeToString())
+
+    def send_input_key(self, key: Key) -> None:
+        proto_key = convert_key_to_proto(key)
+        send_data(self.client, proto_key.SerializeToString())
+
+    def run(self):
+        self.initialize()
+        while True:
+            data = self.client.recv(1)
+            if not data or data == CLOSE:
+                break
+            elif data == PROCESSING:
+                state_packet = recv_data(self.client)
+                state: Message = service_pb2.PlayerGameState()
+                state.ParseFromString(state_packet)
+
+                flag = Flag(state.state_flag)
+                if flag is Flag.INITIALIZE:
+                    self.ai.initialize(GameData.from_proto(state.game_data), self.player_number)
+                elif flag is Flag.PROCESSING:
+                    if state.HasField("non_delay_frame_data"):
+                        self.ai.get_non_delay_frame_data(FrameData.from_proto(state.non_delay_frame_data))
 
-                if state.HasField("screen_data"):
-                    self.ai.get_screen_data(ScreenData(state.screen_data))
+                    if state.HasField("screen_data"):
+                        self.ai.get_screen_data(ScreenData.from_proto(state.screen_data))
 
-                if state.HasField("audio_data"):
-                    self.ai.get_audio_data(AudioData(state.audio_data))
+                    self.ai.get_information(FrameData.from_proto(state.frame_data), state.is_control)
+                    self.ai.get_audio_data(AudioData.from_proto(state.audio_data))
                     
-                self.ai.processing()
-                await self.input_rpc(self.ai.input())
-            elif flag is Flag.ROUND_END:
-                self.ai.round_end(RoundResult(state.round_result))
-            elif flag is Flag.GAME_END:
-                self.ai.round_end(RoundResult(state.round_result))
-                self.ai.game_end()
+                    self.ai.processing()
+                    self.send_input_key(self.ai.input())
+                elif flag is Flag.ROUND_END:
+                    self.ai.round_end(RoundResult.from_proto(state.round_result))
+                elif flag is Flag.GAME_END:
+                    self.ai.round_end(RoundResult.from_proto(state.round_result))
+                    self.ai.game_end()
+    
+    def close(self):
+        self.client.close()
```

### Comparing `pyftg-2.0.1/src/pyftg/aio/gateway.py` & `pyftg-2.1/src/pyftg/socket/threading/gateway.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,70 @@
-import asyncio
 import logging
+import socket
+from contextlib import closing
 
-import grpc
+from google.protobuf.message import Message
 
-from ..aiinterface import AIInterface
-from ..enum.status_code import StatusCode
-from ..protoc import service_pb2, service_pb2_grpc
-from .ai_controller import AIController
+from pyftg.aiinterface.ai_interface import AIInterface
+from pyftg.models.enums.status_code import StatusCode
+from pyftg.protoc import service_pb2
+from pyftg.socket.threading.ai_controller import AIController
+from pyftg.socket.utils.threading import recv_data, send_data
+from pyftg.utils.resource_loader import load_ai
 
+logger = logging.getLogger(__name__)
 
-def load_ai(ai_path: str) -> AIInterface:
-    path = ai_path.split('.')
-    module_name, class_name = path[0], path[int(len(path) == 2)]
-    return getattr(__import__(module_name), class_name)()
 
 class Gateway:
     def __init__(self, host='127.0.0.1', port=50051):
         self.host = host
         self.port = port
-        self.channel = grpc.aio.insecure_channel(
-            target=f"{host}:{port}",
-            compression=grpc.Compression.Gzip,
-        )
-        self.stub = service_pb2_grpc.ServiceStub(self.channel)
-        self.registered_agents: 'dict[str, AIInterface]' = dict()
-        self.agents: 'list[AIInterface]' = [None, None]
-        self.ais: 'list[AIController]' = [None, None]
+        self.registered_agents: dict[str, AIInterface] = dict()
+        self.agents: list[AIInterface] = [None, None]
+        self.ais: list[AIController] = [None, None]
     
-    def load_agent(self, ai_names: 'list[str]'):
+    def load_agent(self, ai_names: list[str]):
+        if ai_names[0] is None and ai_names[1] is None:
+            raise Exception("At least one agent must be specified.")
         for i, ai_name in enumerate(ai_names):
             if ai_name:
                 self.agents[i] = load_ai(ai_name)
     
     def register_ai(self, name: str, agent: AIInterface):
         self.registered_agents[name] = agent
 
-    async def run_game(self, characters: 'list[str]', agents: 'list[str]', game_number: int):
+    def run_game(self, characters: list[str], agents: list[str], game_number: int):
         for i in range(2):
             if agents[i] == 'Sandbox':
                 agents[i] = None
             elif agents[i] in self.registered_agents:
                 self.agents[i] = self.registered_agents[agents[i]]
-        response = await self.stub.RunGame(service_pb2.RunGameRequest(character_1=characters[0], character_2=characters[1], player_1=agents[0], player_2=agents[1], game_number=game_number))
-        if StatusCode(response.status_code) == StatusCode.FAILED:
-            raise Exception(response.response_message)
-        await self.start_ai()
-    
-    async def start_ai(self):
-        tasks = list()
-        loop = asyncio.get_event_loop()
+        
+        with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as client:
+            client.connect((self.host, self.port))
+            request: Message = service_pb2.RunGameRequest(character_1=characters[0], character_2=characters[1],
+                                                      player_1=agents[0], player_2=agents[1], game_number=game_number)
+            send_data(client, b'\x02', with_header=False)  # 2: Run Game
+            send_data(client, request.SerializeToString())
+            
+            response_packet = recv_data(client)
+            response: Message = service_pb2.RunGameResponse()
+            response.ParseFromString(response_packet)
+
+            if response.status_code is StatusCode.FAILED:
+                logger.error(response.response_message)
+                exit(1)
+        
+        self.start_ai()
+
+    def start_ai(self):
         for i, agent in enumerate(self.agents):
             if agent:
-                self.ais[i] = AIController(self.stub, agent, i == 0)
-                tasks.append(loop.create_task(self.ais[i].run()))
-                logging.info(f"AI controller for P{i+1} ({agent.name()}) is ready.")
-        await asyncio.gather(*tasks)
+                self.ais[i] = AIController(self.host, self.port, agent, i == 0)
+                self.ais[i].start()
+                logger.info(f"AI controller for P{i+1} ({agent.name()}) is ready.")
+        return [x.join() for x in self.ais if x]
     
-    async def close(self):
-        await self.channel.close()
+    def close(self):
+        for ai in self.ais:
+            if ai:
+                ai.close()
```

### Comparing `pyftg-2.0.1/src/pyftg/enum/action.py` & `pyftg-2.1/src/pyftg/models/enums/int_action.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 
 
-class Action(Enum):
+class IntAction(int, Enum):
     NEUTRAL = 0
     STAND = 1
     FORWARD_WALK = 2
     DASH = 3
     BACK_STEP = 4
     CROUCH = 5
     JUMP = 6
```

### Comparing `pyftg-2.0.1/src/pyftg/gateway.py` & `pyftg-2.1/src/pyftg/grpc/threading/gateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 import logging
 
 import grpc
 
-from .ai_controller import AIController
-from .aiinterface import AIInterface
-from .enum.status_code import StatusCode
-from .protoc import service_pb2, service_pb2_grpc
+from pyftg.aiinterface.ai_interface import AIInterface
+from pyftg.grpc.threading.ai_controller import AIController
+from pyftg.models.enums.status_code import StatusCode
+from pyftg.protoc import service_pb2, service_pb2_grpc
+from pyftg.utils.resource_loader import load_ai
 
+logger = logging.getLogger(__name__)
 
-def load_ai(ai_path: str) -> AIInterface:
-    path = ai_path.split('.')
-    module_name, class_name = path[0], path[int(len(path) == 2)]
-    return getattr(__import__(module_name), class_name)()
 
 class Gateway:
     def __init__(self, host='127.0.0.1', port=50051):
         self.host = host
         self.port = port
         self.channel = grpc.insecure_channel(
             target=f"{host}:{port}",
             compression=grpc.Compression.Gzip,
         )
         self.stub = service_pb2_grpc.ServiceStub(self.channel)
-        self.registered_agents: 'dict[str, AIInterface]' = dict()
-        self.agents: 'list[AIInterface]' = [None, None]
-        self.ais: 'list[AIController]' = [None, None]
+        self.registered_agents: dict[str, AIInterface] = dict()
+        self.agents: list[AIInterface] = [None, None]
+        self.ais: list[AIController] = [None, None]
     
-    def load_agent(self, ai_names: 'list[str]'):
+    def load_agent(self, ai_names: list[str]):
+        if ai_names[0] is None and ai_names[1] is None:
+            raise Exception("At least one agent must be specified.")
         for i, ai_name in enumerate(ai_names):
             if ai_name:
                 self.agents[i] = load_ai(ai_name)
     
     def register_ai(self, name: str, agent: AIInterface):
         self.registered_agents[name] = agent
 
-    def run_game(self, characters: 'list[str]', agents: 'list[str]', game_number: int):
+    def run_game(self, characters: list[str], agents: list[str], game_number: int):
         for i in range(2):
             if agents[i] == 'Sandbox':
                 agents[i] = None
             elif agents[i] in self.registered_agents:
                 self.agents[i] = self.registered_agents[agents[i]]
-        response = self.stub.RunGame(service_pb2.RunGameRequest(character_1=characters[0], character_2=characters[1], player_1=agents[0], player_2=agents[1], game_number=game_number))
-        if StatusCode(response.status_code) == StatusCode.FAILED:
-            raise Exception(response.response_message)
+        response = self.stub.RunGame(service_pb2.RunGameRequest(character_1=characters[0], character_2=characters[1], 
+                                                                player_1=agents[0], player_2=agents[1], game_number=game_number))
+        if StatusCode(response.status_code) is StatusCode.FAILED:
+            logger.error(response.response_message)
+            exit(1)
 
         self.start_ai()
     
     def start_ai(self):
         for i, agent in enumerate(self.agents):
             if agent:
                 self.ais[i] = AIController(self.stub, agent, i == 0)
                 self.ais[i].start()
-                logging.info(f"AI controller for P{i+1} ({agent.name()}) is ready.")
+                logger.info(f"AI controller for P{i+1} ({agent.name()}) is ready.")
         return [x.join() for x in self.ais if x]
     
     def close(self):
         self.channel.close()
```

### Comparing `pyftg-2.0.1/src/pyftg/observer_gateway.py` & `pyftg-2.1/src/pyftg/grpc/threading/observer_gateway.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import grpc
 
-from .enum.data_flag import DataFlag
-from .enum.flag import Flag
-from .observer_handler import ObserverHandler
-from .protoc import service_pb2, service_pb2_grpc
-from .struct import AudioData, FrameData, GameData, RoundResult, ScreenData
+from pyftg.grpc.threading.observer_handler import ObserverHandler
+from pyftg.models.audio_data import AudioData
+from pyftg.models.enums.data_flag import DataFlag
+from pyftg.models.enums.flag import Flag
+from pyftg.models.frame_data import FrameData
+from pyftg.models.game_data import GameData
+from pyftg.models.round_result import RoundResult
+from pyftg.models.screen_data import ScreenData
+from pyftg.protoc import service_pb2, service_pb2_grpc
 
 
 class ObserverGateway:
     def __init__(self, handler: ObserverHandler, data_flag: DataFlag, interval=1, host='127.0.0.1', port=50051):
         self.host = host
         self.port = port
         self.channel = grpc.insecure_channel(
@@ -39,17 +43,18 @@
         request = service_pb2.SpectateRequest(interval=self.interval, frame_data_flag=frame_data_flag, screen_data_flag=screen_data_flag, audio_data_flag=audio_data_flag)
         return self.stub.Spectate(request)
     
     def start(self):
         for state in self.spectate_rpc():
             flag = Flag(state.state_flag)
             if flag is Flag.INITIALIZE:
-                self.handler.on_initialize(GameData(state.game_data))
+                self.handler.on_initialize(GameData.from_proto(state.game_data))
             elif flag is Flag.PROCESSING:
-                self.handler.on_game_update(FrameData(state.frame_data), ScreenData(state.screen_data), AudioData(state.audio_data))
+                self.handler.on_game_update(FrameData.from_proto(state.frame_data), ScreenData.from_proto(state.screen_data), 
+                                            AudioData.from_proto(state.audio_data))
             elif flag is Flag.ROUND_END:
-                self.handler.on_round_end(RoundResult(state.round_result), False)
+                self.handler.on_round_end(RoundResult.from_proto(state.round_result), False)
             elif flag is Flag.GAME_END:
-                self.handler.on_round_end(RoundResult(state.round_result), True)
+                self.handler.on_round_end(RoundResult.from_proto(state.round_result), True)
     
     def close(self):
         self.channel.close()
```

### Comparing `pyftg-2.0.1/src/pyftg/protoc/message_pb2.py` & `pyftg-2.1/src/pyftg/protoc/message_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,34 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: message.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-# @@protoc_insertion_point(imports)
-
 _sym_db = _symbol_database.Default()
-
-
 from . import enum_pb2 as enum__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rmessage.proto\x12\x07service\x1a\nenum.proto\"G\n\x0bGrpcHitArea\x12\x0c\n\x04left\x18\x01 \x01(\x05\x12\r\n\x05right\x18\x02 \x01(\x05\x12\x0b\n\x03top\x18\x03 \x01(\x05\x12\x0e\n\x06\x62ottom\x18\x04 \x01(\x05\"\x9c\x04\n\x0eGrpcAttackData\x12.\n\x10setting_hit_area\x18\x01 \x01(\x0b\x32\x14.service.GrpcHitArea\x12\x17\n\x0fsetting_speed_x\x18\x02 \x01(\x05\x12\x17\n\x0fsetting_speed_y\x18\x03 \x01(\x05\x12.\n\x10\x63urrent_hit_area\x18\x04 \x01(\x0b\x32\x14.service.GrpcHitArea\x12\x15\n\rcurrent_frame\x18\x05 \x01(\x05\x12\x15\n\rplayer_number\x18\x06 \x01(\x08\x12\x0f\n\x07speed_x\x18\x07 \x01(\x05\x12\x0f\n\x07speed_y\x18\x08 \x01(\x05\x12\x10\n\x08start_up\x18\t \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\n \x01(\x05\x12\x12\n\nhit_damage\x18\x0b \x01(\x05\x12\x14\n\x0cguard_damage\x18\x0c \x01(\x05\x12\x18\n\x10start_add_energy\x18\r \x01(\x05\x12\x16\n\x0ehit_add_energy\x18\x0e \x01(\x05\x12\x18\n\x10guard_add_energy\x18\x0f \x01(\x05\x12\x13\n\x0bgive_energy\x18\x10 \x01(\x05\x12\x10\n\x08impact_x\x18\x11 \x01(\x05\x12\x10\n\x08impact_y\x18\x12 \x01(\x05\x12\x18\n\x10give_guard_recov\x18\x13 \x01(\x05\x12\x13\n\x0b\x61ttack_type\x18\x14 \x01(\x05\x12\x11\n\tdown_prop\x18\x15 \x01(\x08\x12\x15\n\ris_projectile\x18\x16 \x01(\x08\"\xf1\x03\n\x11GrpcCharacterData\x12\x15\n\rplayer_number\x18\x01 \x01(\x08\x12\n\n\x02hp\x18\x02 \x01(\x05\x12\x0e\n\x06\x65nergy\x18\x03 \x01(\x05\x12\t\n\x01x\x18\x04 \x01(\x05\x12\t\n\x01y\x18\x05 \x01(\x05\x12\x0c\n\x04left\x18\x06 \x01(\x05\x12\r\n\x05right\x18\x07 \x01(\x05\x12\x0b\n\x03top\x18\x08 \x01(\x05\x12\x0e\n\x06\x62ottom\x18\t \x01(\x05\x12\x0f\n\x07speed_x\x18\n \x01(\x05\x12\x0f\n\x07speed_y\x18\x0b \x01(\x05\x12!\n\x05state\x18\x0c \x01(\x0e\x32\x12.service.GrpcState\x12#\n\x06\x61\x63tion\x18\r \x01(\x0e\x32\x13.service.GrpcAction\x12\r\n\x05\x66ront\x18\x0e \x01(\x08\x12\x0f\n\x07\x63ontrol\x18\x0f \x01(\x08\x12,\n\x0b\x61ttack_data\x18\x10 \x01(\x0b\x32\x17.service.GrpcAttackData\x12\x17\n\x0fremaining_frame\x18\x11 \x01(\x05\x12\x13\n\x0bhit_confirm\x18\x12 \x01(\x08\x12\x16\n\x0egraphic_size_x\x18\x13 \x01(\x05\x12\x16\n\x0egraphic_size_y\x18\x14 \x01(\x05\x12\x18\n\x10graphic_adjust_x\x18\x15 \x01(\x05\x12\x11\n\thit_count\x18\x16 \x01(\x05\x12\x16\n\x0elast_hit_frame\x18\x17 \x01(\x05\"\xcd\x01\n\rGrpcFrameData\x12\x32\n\x0e\x63haracter_data\x18\x01 \x03(\x0b\x32\x1a.service.GrpcCharacterData\x12\x1c\n\x14\x63urrent_frame_number\x18\x02 \x01(\x05\x12\x15\n\rcurrent_round\x18\x03 \x01(\x05\x12\x30\n\x0fprojectile_data\x18\x04 \x03(\x0b\x32\x17.service.GrpcAttackData\x12\x12\n\nempty_flag\x18\x05 \x01(\x08\x12\r\n\x05\x66ront\x18\x06 \x03(\x08\"J\n\x0bGrpcFftData\x12\x1a\n\x12real_data_as_bytes\x18\x01 \x01(\x0c\x12\x1f\n\x17imaginary_data_as_bytes\x18\x02 \x01(\x0c\"\'\n\x0eGrpcScreenData\x12\x15\n\rdisplay_bytes\x18\x01 \x01(\x0c\"u\n\rGrpcAudioData\x12\x19\n\x11raw_data_as_bytes\x18\x01 \x01(\x0c\x12&\n\x08\x66\x66t_data\x18\x02 \x03(\x0b\x32\x14.service.GrpcFftData\x12!\n\x19spectrogram_data_as_bytes\x18\x03 \x01(\x0c\"`\n\x0cGrpcGameData\x12\x0f\n\x07max_hps\x18\x01 \x03(\x05\x12\x14\n\x0cmax_energies\x18\x02 \x03(\x05\x12\x17\n\x0f\x63haracter_names\x18\x03 \x03(\t\x12\x10\n\x08\x61i_names\x18\x04 \x03(\t\"V\n\x0fGrpcRoundResult\x12\x15\n\rcurrent_round\x18\x01 \x01(\x05\x12\x15\n\rremaining_hps\x18\x02 \x03(\x05\x12\x15\n\relapsed_frame\x18\x03 \x01(\x05\"V\n\x07GrpcKey\x12\t\n\x01\x41\x18\x01 \x01(\x08\x12\t\n\x01\x42\x18\x02 \x01(\x08\x12\t\n\x01\x43\x18\x03 \x01(\x08\x12\t\n\x01U\x18\x04 \x01(\x08\x12\t\n\x01R\x18\x05 \x01(\x08\x12\t\n\x01\x44\x18\x06 \x01(\x08\x12\t\n\x01L\x18\x07 \x01(\x08\x42\x1d\xaa\x02\x1a\x44\x61reFightingICE.Grpc.Protob\x06proto3')
-
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rmessage.proto\x12\x07service\x1a\nenum.proto"G\n\x0bGrpcHitArea\x12\x0c\n\x04left\x18\x01 \x01(\x05\x12\r\n\x05right\x18\x02 \x01(\x05\x12\x0b\n\x03top\x18\x03 \x01(\x05\x12\x0e\n\x06bottom\x18\x04 \x01(\x05"\xd5\x04\n\x0eGrpcAttackData\x12.\n\x10setting_hit_area\x18\x01 \x01(\x0b2\x14.service.GrpcHitArea\x12\x17\n\x0fsetting_speed_x\x18\x02 \x01(\x05\x12\x17\n\x0fsetting_speed_y\x18\x03 \x01(\x05\x12.\n\x10current_hit_area\x18\x04 \x01(\x0b2\x14.service.GrpcHitArea\x12\x15\n\rcurrent_frame\x18\x05 \x01(\x05\x12\x15\n\rplayer_number\x18\x06 \x01(\x08\x12\x0f\n\x07speed_x\x18\x07 \x01(\x05\x12\x0f\n\x07speed_y\x18\x08 \x01(\x05\x12\x10\n\x08start_up\x18\t \x01(\x05\x12\x0e\n\x06active\x18\n \x01(\x05\x12\x12\n\nhit_damage\x18\x0b \x01(\x05\x12\x14\n\x0cguard_damage\x18\x0c \x01(\x05\x12\x18\n\x10start_add_energy\x18\r \x01(\x05\x12\x16\n\x0ehit_add_energy\x18\x0e \x01(\x05\x12\x18\n\x10guard_add_energy\x18\x0f \x01(\x05\x12\x13\n\x0bgive_energy\x18\x10 \x01(\x05\x12\x10\n\x08impact_x\x18\x11 \x01(\x05\x12\x10\n\x08impact_y\x18\x12 \x01(\x05\x12\x18\n\x10give_guard_recov\x18\x13 \x01(\x05\x12\x13\n\x0battack_type\x18\x14 \x01(\x05\x12\x11\n\tdown_prop\x18\x15 \x01(\x08\x12\x15\n\ris_projectile\x18\x16 \x01(\x08\x12\x0f\n\x07is_live\x18\x17 \x01(\x08\x12\x12\n\nempty_flag\x18\x18 \x01(\x08\x12\x12\n\nidentifier\x18\x19 \x01(\t"\xa5\x04\n\x11GrpcCharacterData\x12\x15\n\rplayer_number\x18\x01 \x01(\x08\x12\n\n\x02hp\x18\x02 \x01(\x05\x12\x0e\n\x06energy\x18\x03 \x01(\x05\x12\t\n\x01x\x18\x04 \x01(\x05\x12\t\n\x01y\x18\x05 \x01(\x05\x12\x0c\n\x04left\x18\x06 \x01(\x05\x12\r\n\x05right\x18\x07 \x01(\x05\x12\x0b\n\x03top\x18\x08 \x01(\x05\x12\x0e\n\x06bottom\x18\t \x01(\x05\x12\x0f\n\x07speed_x\x18\n \x01(\x05\x12\x0f\n\x07speed_y\x18\x0b \x01(\x05\x12!\n\x05state\x18\x0c \x01(\x0e2\x12.service.GrpcState\x12#\n\x06action\x18\r \x01(\x0e2\x13.service.GrpcAction\x12\r\n\x05front\x18\x0e \x01(\x08\x12\x0f\n\x07control\x18\x0f \x01(\x08\x12,\n\x0battack_data\x18\x10 \x01(\x0b2\x17.service.GrpcAttackData\x12\x17\n\x0fremaining_frame\x18\x11 \x01(\x05\x12\x13\n\x0bhit_confirm\x18\x12 \x01(\x08\x12\x16\n\x0egraphic_size_x\x18\x13 \x01(\x05\x12\x16\n\x0egraphic_size_y\x18\x14 \x01(\x05\x12\x18\n\x10graphic_adjust_x\x18\x15 \x01(\x05\x12\x11\n\thit_count\x18\x16 \x01(\x05\x12\x16\n\x0elast_hit_frame\x18\x17 \x01(\x05\x122\n\x11projectile_attack\x18\x18 \x03(\x0b2\x17.service.GrpcAttackData"\xcd\x01\n\rGrpcFrameData\x122\n\x0echaracter_data\x18\x01 \x03(\x0b2\x1a.service.GrpcCharacterData\x12\x1c\n\x14current_frame_number\x18\x02 \x01(\x05\x12\x15\n\rcurrent_round\x18\x03 \x01(\x05\x120\n\x0fprojectile_data\x18\x04 \x03(\x0b2\x17.service.GrpcAttackData\x12\x12\n\nempty_flag\x18\x05 \x01(\x08\x12\r\n\x05front\x18\x06 \x03(\x08"J\n\x0bGrpcFftData\x12\x1a\n\x12real_data_as_bytes\x18\x01 \x01(\x0c\x12\x1f\n\x17imaginary_data_as_bytes\x18\x02 \x01(\x0c"\'\n\x0eGrpcScreenData\x12\x15\n\rdisplay_bytes\x18\x01 \x01(\x0c"u\n\rGrpcAudioData\x12\x19\n\x11raw_data_as_bytes\x18\x01 \x01(\x0c\x12&\n\x08fft_data\x18\x02 \x03(\x0b2\x14.service.GrpcFftData\x12!\n\x19spectrogram_data_as_bytes\x18\x03 \x01(\x0c"`\n\x0cGrpcGameData\x12\x0f\n\x07max_hps\x18\x01 \x03(\x05\x12\x14\n\x0cmax_energies\x18\x02 \x03(\x05\x12\x17\n\x0fcharacter_names\x18\x03 \x03(\t\x12\x10\n\x08ai_names\x18\x04 \x03(\t"V\n\x0fGrpcRoundResult\x12\x15\n\rcurrent_round\x18\x01 \x01(\x05\x12\x15\n\rremaining_hps\x18\x02 \x03(\x05\x12\x15\n\relapsed_frame\x18\x03 \x01(\x05"V\n\x07GrpcKey\x12\t\n\x01A\x18\x01 \x01(\x08\x12\t\n\x01B\x18\x02 \x01(\x08\x12\t\n\x01C\x18\x03 \x01(\x08\x12\t\n\x01U\x18\x04 \x01(\x08\x12\t\n\x01R\x18\x05 \x01(\x08\x12\t\n\x01D\x18\x06 \x01(\x08\x12\t\n\x01L\x18\x07 \x01(\x08B5\n\x06protocB\x0cMessageProtoP\x00\xaa\x02\x1aDareFightingICE.Grpc.Protob\x06proto3')
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'message_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\252\002\032DareFightingICE.Grpc.Proto'
-  _globals['_GRPCHITAREA']._serialized_start=38
-  _globals['_GRPCHITAREA']._serialized_end=109
-  _globals['_GRPCATTACKDATA']._serialized_start=112
-  _globals['_GRPCATTACKDATA']._serialized_end=652
-  _globals['_GRPCCHARACTERDATA']._serialized_start=655
-  _globals['_GRPCCHARACTERDATA']._serialized_end=1152
-  _globals['_GRPCFRAMEDATA']._serialized_start=1155
-  _globals['_GRPCFRAMEDATA']._serialized_end=1360
-  _globals['_GRPCFFTDATA']._serialized_start=1362
-  _globals['_GRPCFFTDATA']._serialized_end=1436
-  _globals['_GRPCSCREENDATA']._serialized_start=1438
-  _globals['_GRPCSCREENDATA']._serialized_end=1477
-  _globals['_GRPCAUDIODATA']._serialized_start=1479
-  _globals['_GRPCAUDIODATA']._serialized_end=1596
-  _globals['_GRPCGAMEDATA']._serialized_start=1598
-  _globals['_GRPCGAMEDATA']._serialized_end=1694
-  _globals['_GRPCROUNDRESULT']._serialized_start=1696
-  _globals['_GRPCROUNDRESULT']._serialized_end=1782
-  _globals['_GRPCKEY']._serialized_start=1784
-  _globals['_GRPCKEY']._serialized_end=1870
-# @@protoc_insertion_point(module_scope)
+    _globals['DESCRIPTOR']._options = None
+    _globals['DESCRIPTOR']._serialized_options = b'\n\x06protocB\x0cMessageProtoP\x00\xaa\x02\x1aDareFightingICE.Grpc.Proto'
+    _globals['_GRPCHITAREA']._serialized_start = 38
+    _globals['_GRPCHITAREA']._serialized_end = 109
+    _globals['_GRPCATTACKDATA']._serialized_start = 112
+    _globals['_GRPCATTACKDATA']._serialized_end = 709
+    _globals['_GRPCCHARACTERDATA']._serialized_start = 712
+    _globals['_GRPCCHARACTERDATA']._serialized_end = 1261
+    _globals['_GRPCFRAMEDATA']._serialized_start = 1264
+    _globals['_GRPCFRAMEDATA']._serialized_end = 1469
+    _globals['_GRPCFFTDATA']._serialized_start = 1471
+    _globals['_GRPCFFTDATA']._serialized_end = 1545
+    _globals['_GRPCSCREENDATA']._serialized_start = 1547
+    _globals['_GRPCSCREENDATA']._serialized_end = 1586
+    _globals['_GRPCAUDIODATA']._serialized_start = 1588
+    _globals['_GRPCAUDIODATA']._serialized_end = 1705
+    _globals['_GRPCGAMEDATA']._serialized_start = 1707
+    _globals['_GRPCGAMEDATA']._serialized_end = 1803
+    _globals['_GRPCROUNDRESULT']._serialized_start = 1805
+    _globals['_GRPCROUNDRESULT']._serialized_end = 1891
+    _globals['_GRPCKEY']._serialized_start = 1893
+    _globals['_GRPCKEY']._serialized_end = 1979
```

### Comparing `pyftg-2.0.1/src/pyftg/protoc/service_pb2.py` & `pyftg-2.1/src/pyftg/protoc/service_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,36 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: service.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-# @@protoc_insertion_point(imports)
-
 _sym_db = _symbol_database.Default()
-
-
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from . import enum_pb2 as enum__pb2
 from . import message_pb2 as message__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rservice.proto\x12\x07service\x1a\x1bgoogle/protobuf/empty.proto\x1a\nenum.proto\x1a\rmessage.proto\"s\n\x0eRunGameRequest\x12\x13\n\x0b\x63haracter_1\x18\x01 \x01(\t\x12\x13\n\x0b\x63haracter_2\x18\x02 \x01(\t\x12\x10\n\x08player_1\x18\x03 \x01(\t\x12\x10\n\x08player_2\x18\x04 \x01(\t\x12\x13\n\x0bgame_number\x18\x05 \x01(\x05\"Y\n\x0fRunGameResponse\x12,\n\x0bstatus_code\x18\x01 \x01(\x0e\x32\x17.service.GrpcStatusCode\x12\x18\n\x10response_message\x18\x02 \x01(\t\"o\n\x0fSpectateRequest\x12\x10\n\x08interval\x18\x01 \x01(\x05\x12\x17\n\x0f\x66rame_data_flag\x18\x02 \x01(\x08\x12\x18\n\x10screen_data_flag\x18\x03 \x01(\x08\x12\x17\n\x0f\x61udio_data_flag\x18\x04 \x01(\x08\"\x9b\x02\n\x12SpectatorGameState\x12%\n\nstate_flag\x18\x01 \x01(\x0e\x32\x11.service.GrpcFlag\x12(\n\tgame_data\x18\x02 \x01(\x0b\x32\x15.service.GrpcGameData\x12*\n\nframe_data\x18\x03 \x01(\x0b\x32\x16.service.GrpcFrameData\x12,\n\x0bscreen_data\x18\x04 \x01(\x0b\x32\x17.service.GrpcScreenData\x12*\n\naudio_data\x18\x05 \x01(\x0b\x32\x16.service.GrpcAudioData\x12.\n\x0cround_result\x18\x06 \x01(\x0b\x32\x18.service.GrpcRoundResult\"Q\n\x11InitializeRequest\x12\x15\n\rplayer_number\x18\x01 \x01(\x08\x12\x13\n\x0bplayer_name\x18\x02 \x01(\t\x12\x10\n\x08is_blind\x18\x03 \x01(\x08\")\n\x12InitializeResponse\x12\x13\n\x0bplayer_uuid\x18\x01 \x01(\t\")\n\x12ParticipateRequest\x12\x13\n\x0bplayer_uuid\x18\x01 \x01(\t\"\xe2\x02\n\x0fPlayerGameState\x12%\n\nstate_flag\x18\x01 \x01(\x0e\x32\x11.service.GrpcFlag\x12\x12\n\nis_control\x18\x02 \x01(\x08\x12*\n\nframe_data\x18\x03 \x01(\x0b\x32\x16.service.GrpcFrameData\x12\x34\n\x14non_delay_frame_data\x18\x04 \x01(\x0b\x32\x16.service.GrpcFrameData\x12,\n\x0bscreen_data\x18\x05 \x01(\x0b\x32\x17.service.GrpcScreenData\x12*\n\naudio_data\x18\x06 \x01(\x0b\x32\x16.service.GrpcAudioData\x12(\n\tgame_data\x18\x07 \x01(\x0b\x32\x15.service.GrpcGameData\x12.\n\x0cround_result\x18\x08 \x01(\x0b\x32\x18.service.GrpcRoundResult\"G\n\x0bPlayerInput\x12\x13\n\x0bplayer_uuid\x18\x01 \x01(\t\x12#\n\tinput_key\x18\x02 \x01(\x0b\x32\x10.service.GrpcKey2\xdc\x02\n\x07Service\x12>\n\x07RunGame\x12\x17.service.RunGameRequest\x1a\x18.service.RunGameResponse\"\x00\x12\x45\n\x08Spectate\x12\x18.service.SpectateRequest\x1a\x1b.service.SpectatorGameState\"\x00\x30\x01\x12G\n\nInitialize\x12\x1a.service.InitializeRequest\x1a\x1b.service.InitializeResponse\"\x00\x12H\n\x0bParticipate\x12\x1b.service.ParticipateRequest\x1a\x18.service.PlayerGameState\"\x00\x30\x01\x12\x37\n\x05Input\x12\x14.service.PlayerInput\x1a\x16.google.protobuf.Empty\"\x00\x42\x1d\xaa\x02\x1a\x44\x61reFightingICE.Grpc.Protob\x06proto3')
-
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rservice.proto\x12\x07service\x1a\x1bgoogle/protobuf/empty.proto\x1a\nenum.proto\x1a\rmessage.proto"s\n\x0eRunGameRequest\x12\x13\n\x0bcharacter_1\x18\x01 \x01(\t\x12\x13\n\x0bcharacter_2\x18\x02 \x01(\t\x12\x10\n\x08player_1\x18\x03 \x01(\t\x12\x10\n\x08player_2\x18\x04 \x01(\t\x12\x13\n\x0bgame_number\x18\x05 \x01(\x05"Y\n\x0fRunGameResponse\x12,\n\x0bstatus_code\x18\x01 \x01(\x0e2\x17.service.GrpcStatusCode\x12\x18\n\x10response_message\x18\x02 \x01(\t"o\n\x0fSpectateRequest\x12\x10\n\x08interval\x18\x01 \x01(\x05\x12\x17\n\x0fframe_data_flag\x18\x02 \x01(\x08\x12\x18\n\x10screen_data_flag\x18\x03 \x01(\x08\x12\x17\n\x0faudio_data_flag\x18\x04 \x01(\x08"\x9b\x02\n\x12SpectatorGameState\x12%\n\nstate_flag\x18\x01 \x01(\x0e2\x11.service.GrpcFlag\x12(\n\tgame_data\x18\x02 \x01(\x0b2\x15.service.GrpcGameData\x12*\n\nframe_data\x18\x03 \x01(\x0b2\x16.service.GrpcFrameData\x12,\n\x0bscreen_data\x18\x04 \x01(\x0b2\x17.service.GrpcScreenData\x12*\n\naudio_data\x18\x05 \x01(\x0b2\x16.service.GrpcAudioData\x12.\n\x0cround_result\x18\x06 \x01(\x0b2\x18.service.GrpcRoundResult"Q\n\x11InitializeRequest\x12\x15\n\rplayer_number\x18\x01 \x01(\x08\x12\x13\n\x0bplayer_name\x18\x02 \x01(\t\x12\x10\n\x08is_blind\x18\x03 \x01(\x08")\n\x12InitializeResponse\x12\x13\n\x0bplayer_uuid\x18\x01 \x01(\t")\n\x12ParticipateRequest\x12\x13\n\x0bplayer_uuid\x18\x01 \x01(\t"\xe2\x02\n\x0fPlayerGameState\x12%\n\nstate_flag\x18\x01 \x01(\x0e2\x11.service.GrpcFlag\x12\x12\n\nis_control\x18\x02 \x01(\x08\x12*\n\nframe_data\x18\x03 \x01(\x0b2\x16.service.GrpcFrameData\x124\n\x14non_delay_frame_data\x18\x04 \x01(\x0b2\x16.service.GrpcFrameData\x12,\n\x0bscreen_data\x18\x05 \x01(\x0b2\x17.service.GrpcScreenData\x12*\n\naudio_data\x18\x06 \x01(\x0b2\x16.service.GrpcAudioData\x12(\n\tgame_data\x18\x07 \x01(\x0b2\x15.service.GrpcGameData\x12.\n\x0cround_result\x18\x08 \x01(\x0b2\x18.service.GrpcRoundResult"G\n\x0bPlayerInput\x12\x13\n\x0bplayer_uuid\x18\x01 \x01(\t\x12#\n\tinput_key\x18\x02 \x01(\x0b2\x10.service.GrpcKey2\xdc\x02\n\x07Service\x12>\n\x07RunGame\x12\x17.service.RunGameRequest\x1a\x18.service.RunGameResponse"\x00\x12E\n\x08Spectate\x12\x18.service.SpectateRequest\x1a\x1b.service.SpectatorGameState"\x000\x01\x12G\n\nInitialize\x12\x1a.service.InitializeRequest\x1a\x1b.service.InitializeResponse"\x00\x12H\n\x0bParticipate\x12\x1b.service.ParticipateRequest\x1a\x18.service.PlayerGameState"\x000\x01\x127\n\x05Input\x12\x14.service.PlayerInput\x1a\x16.google.protobuf.Empty"\x00B5\n\x06protocB\x0cServiceProtoP\x00\xaa\x02\x1aDareFightingICE.Grpc.Protob\x06proto3')
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\252\002\032DareFightingICE.Grpc.Proto'
-  _globals['_RUNGAMEREQUEST']._serialized_start=82
-  _globals['_RUNGAMEREQUEST']._serialized_end=197
-  _globals['_RUNGAMERESPONSE']._serialized_start=199
-  _globals['_RUNGAMERESPONSE']._serialized_end=288
-  _globals['_SPECTATEREQUEST']._serialized_start=290
-  _globals['_SPECTATEREQUEST']._serialized_end=401
-  _globals['_SPECTATORGAMESTATE']._serialized_start=404
-  _globals['_SPECTATORGAMESTATE']._serialized_end=687
-  _globals['_INITIALIZEREQUEST']._serialized_start=689
-  _globals['_INITIALIZEREQUEST']._serialized_end=770
-  _globals['_INITIALIZERESPONSE']._serialized_start=772
-  _globals['_INITIALIZERESPONSE']._serialized_end=813
-  _globals['_PARTICIPATEREQUEST']._serialized_start=815
-  _globals['_PARTICIPATEREQUEST']._serialized_end=856
-  _globals['_PLAYERGAMESTATE']._serialized_start=859
-  _globals['_PLAYERGAMESTATE']._serialized_end=1213
-  _globals['_PLAYERINPUT']._serialized_start=1215
-  _globals['_PLAYERINPUT']._serialized_end=1286
-  _globals['_SERVICE']._serialized_start=1289
-  _globals['_SERVICE']._serialized_end=1637
-# @@protoc_insertion_point(module_scope)
+    _globals['DESCRIPTOR']._options = None
+    _globals['DESCRIPTOR']._serialized_options = b'\n\x06protocB\x0cServiceProtoP\x00\xaa\x02\x1aDareFightingICE.Grpc.Proto'
+    _globals['_RUNGAMEREQUEST']._serialized_start = 82
+    _globals['_RUNGAMEREQUEST']._serialized_end = 197
+    _globals['_RUNGAMERESPONSE']._serialized_start = 199
+    _globals['_RUNGAMERESPONSE']._serialized_end = 288
+    _globals['_SPECTATEREQUEST']._serialized_start = 290
+    _globals['_SPECTATEREQUEST']._serialized_end = 401
+    _globals['_SPECTATORGAMESTATE']._serialized_start = 404
+    _globals['_SPECTATORGAMESTATE']._serialized_end = 687
+    _globals['_INITIALIZEREQUEST']._serialized_start = 689
+    _globals['_INITIALIZEREQUEST']._serialized_end = 770
+    _globals['_INITIALIZERESPONSE']._serialized_start = 772
+    _globals['_INITIALIZERESPONSE']._serialized_end = 813
+    _globals['_PARTICIPATEREQUEST']._serialized_start = 815
+    _globals['_PARTICIPATEREQUEST']._serialized_end = 856
+    _globals['_PLAYERGAMESTATE']._serialized_start = 859
+    _globals['_PLAYERGAMESTATE']._serialized_end = 1213
+    _globals['_PLAYERINPUT']._serialized_start = 1215
+    _globals['_PLAYERINPUT']._serialized_end = 1286
+    _globals['_SERVICE']._serialized_start = 1289
+    _globals['_SERVICE']._serialized_end = 1637
```

