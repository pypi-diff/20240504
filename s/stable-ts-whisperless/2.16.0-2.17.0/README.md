# Comparing `tmp/stable-ts-whisperless-2.16.0.tar.gz` & `tmp/stable-ts-whisperless-2.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-whisperless-2.16.0.tar", last modified: Thu Apr 25 00:54:55 2024, max compression
+gzip compressed data, was "stable-ts-whisperless-2.17.0.tar", last modified: Fri May  3 03:58:25 2024, max compression
```

## Comparing `stable-ts-whisperless-2.16.0.tar` & `stable-ts-whisperless-2.17.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 00:54:55.953309 stable-ts-whisperless-2.16.0/
--rw-rw-rw-   0        0        0     1082 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/LICENSE
--rw-rw-rw-   0        0        0    86483 2024-04-25 00:54:55.952306 stable-ts-whisperless-2.16.0/PKG-INFO
--rw-rw-rw-   0        0        0    86082 2024-04-25 00:29:59.000000 stable-ts-whisperless-2.16.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 00:54:55.954309 stable-ts-whisperless-2.16.0/setup.cfg
--rw-rw-rw-   0        0        0     1040 2024-04-24 23:42:29.000000 stable-ts-whisperless-2.16.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:54:55.949309 stable-ts-whisperless-2.16.0/stable_ts_whisperless.egg-info/
--rw-rw-rw-   0        0        0    86483 2024-04-25 00:54:55.000000 stable-ts-whisperless-2.16.0/stable_ts_whisperless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1287 2024-04-25 00:54:55.000000 stable-ts-whisperless-2.16.0/stable_ts_whisperless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 00:54:55.000000 stable-ts-whisperless-2.16.0/stable_ts_whisperless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-25 00:54:55.000000 stable-ts-whisperless-2.16.0/stable_ts_whisperless.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-04-25 00:54:55.000000 stable-ts-whisperless-2.16.0/stable_ts_whisperless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-25 00:54:55.000000 stable-ts-whisperless-2.16.0/stable_ts_whisperless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 00:54:55.913309 stable-ts-whisperless-2.16.0/stable_whisper/
--rw-rw-rw-   0        0        0      353 2024-04-25 00:54:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       50 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       24 2024-04-25 00:53:59.000000 stable-ts-whisperless-2.16.0/stable_whisper/_version.py
--rw-rw-rw-   0        0        0    64912 2024-04-22 00:22:18.000000 stable-ts-whisperless-2.16.0/stable_whisper/alignment.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:54:55.927309 stable-ts-whisperless-2.16.0/stable_whisper/audio/
--rw-rw-rw-   0        0        0    24130 2024-04-23 22:32:22.000000 stable-ts-whisperless-2.16.0/stable_whisper/audio/__init__.py
--rw-rw-rw-   0        0        0     7657 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/audio/demucs.py
--rw-rw-rw-   0        0        0     3276 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/audio/dfnet.py
--rw-rw-rw-   0        0        0     2952 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/audio/noisereduce.py
--rw-rw-rw-   0        0        0     1977 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/audio/output.py
--rw-rw-rw-   0        0        0     8761 2024-04-23 22:32:22.000000 stable-ts-whisperless-2.16.0/stable_whisper/audio/utils.py
--rw-rw-rw-   0        0        0     4522 2024-04-23 22:42:18.000000 stable-ts-whisperless-2.16.0/stable_whisper/decode.py
--rw-rw-rw-   0        0        0     2047 2024-04-21 22:07:38.000000 stable-ts-whisperless-2.16.0/stable_whisper/default.py
--rw-rw-rw-   0        0        0    15841 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/non_whisper.py
--rw-rw-rw-   0        0        0     2308 2024-04-21 23:41:41.000000 stable-ts-whisperless-2.16.0/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0   103107 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/result.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:54:55.935309 stable-ts-whisperless-2.16.0/stable_whisper/stabilization/
--rw-rw-rw-   0        0        0    17009 2024-04-23 22:32:22.000000 stable-ts-whisperless-2.16.0/stable_whisper/stabilization/__init__.py
--rw-rw-rw-   0        0        0     4936 2024-04-23 22:32:22.000000 stable-ts-whisperless-2.16.0/stable_whisper/stabilization/nonvad.py
--rw-rw-rw-   0        0        0     2246 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/stabilization/silero_vad.py
--rw-rw-rw-   0        0        0     4111 2024-04-22 01:45:28.000000 stable-ts-whisperless-2.16.0/stable_whisper/stabilization/utils.py
--rw-rw-rw-   0        0        0    24042 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    11350 2024-04-21 23:39:30.000000 stable-ts-whisperless-2.16.0/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2622 2024-04-21 22:17:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/utils.py
--rw-rw-rw-   0        0        0     4020 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0     8347 2024-04-25 00:54:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/whisper_compatibility.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:54:55.946308 stable-ts-whisperless-2.16.0/stable_whisper/whisper_word_level/
--rw-rw-rw-   0        0        0      454 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/whisper_word_level/__init__.py
--rw-rw-rw-   0        0        0    39229 2024-04-25 00:44:08.000000 stable-ts-whisperless-2.16.0/stable_whisper/whisper_word_level/cli.py
--rw-rw-rw-   0        0        0    11029 2024-04-24 00:22:24.000000 stable-ts-whisperless-2.16.0/stable_whisper/whisper_word_level/faster_whisper.py
--rw-rw-rw-   0        0        0     9957 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.16.0/stable_whisper/whisper_word_level/hf_whisper.py
--rw-rw-rw-   0        0        0    42113 2024-04-24 00:32:36.000000 stable-ts-whisperless-2.16.0/stable_whisper/whisper_word_level/original_whisper.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:58:25.421067 stable-ts-whisperless-2.17.0/
+-rw-rw-rw-   0        0        0     1082 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.17.0/LICENSE
+-rw-rw-rw-   0        0        0    86923 2024-05-03 03:58:25.420068 stable-ts-whisperless-2.17.0/PKG-INFO
+-rw-rw-rw-   0        0        0    86522 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 03:58:25.421067 stable-ts-whisperless-2.17.0/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2024-05-03 03:41:17.000000 stable-ts-whisperless-2.17.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:58:25.418068 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/
+-rw-rw-rw-   0        0        0    86923 2024-05-03 03:58:25.000000 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1287 2024-05-03 03:58:25.000000 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 03:58:25.000000 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-03 03:58:25.000000 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-05-03 03:58:25.000000 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-03 03:58:25.000000 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 03:58:25.390068 stable-ts-whisperless-2.17.0/stable_whisper/
+-rw-rw-rw-   0        0        0      353 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       24 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0    69318 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/alignment.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:58:25.401067 stable-ts-whisperless-2.17.0/stable_whisper/audio/
+-rw-rw-rw-   0        0        0    24130 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/audio/__init__.py
+-rw-rw-rw-   0        0        0     7657 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/audio/demucs.py
+-rw-rw-rw-   0        0        0     3276 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/audio/dfnet.py
+-rw-rw-rw-   0        0        0     2952 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/audio/noisereduce.py
+-rw-rw-rw-   0        0        0     1977 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/audio/output.py
+-rw-rw-rw-   0        0        0     8761 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/audio/utils.py
+-rw-rw-rw-   0        0        0     4522 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0     2047 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/default.py
+-rw-rw-rw-   0        0        0    16051 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/non_whisper.py
+-rw-rw-rw-   0        0        0     2308 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0   103457 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/result.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:58:25.408067 stable-ts-whisperless-2.17.0/stable_whisper/stabilization/
+-rw-rw-rw-   0        0        0    18720 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/stabilization/__init__.py
+-rw-rw-rw-   0        0        0     4936 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/stabilization/nonvad.py
+-rw-rw-rw-   0        0        0     2246 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/stabilization/silero_vad.py
+-rw-rw-rw-   0        0        0     4491 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/stabilization/utils.py
+-rw-rw-rw-   0        0        0    24042 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    11350 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2622 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/utils.py
+-rw-rw-rw-   0        0        0     4020 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0     9426 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/whisper_compatibility.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:58:25.416068 stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/
+-rw-rw-rw-   0        0        0      454 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/__init__.py
+-rw-rw-rw-   0        0        0    39229 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/cli.py
+-rw-rw-rw-   0        0        0    11231 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/faster_whisper.py
+-rw-rw-rw-   0        0        0     9957 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/hf_whisper.py
+-rw-rw-rw-   0        0        0    42315 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/original_whisper.py
```

### Comparing `stable-ts-whisperless-2.16.0/LICENSE` & `stable-ts-whisperless-2.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/PKG-INFO` & `stable-ts-whisperless-2.17.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts-whisperless
-Version: 2.16.0
+Version: 2.17.0
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -185,14 +185,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.1
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     prepend_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Punctuations to prepend to next word.
     append_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
@@ -309,14 +311,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float, default 0.1
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.1
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     only_ffmpeg : bool, default False
         Whether to use only FFmpeg (instead of not yt-dlp) for URls
     options
@@ -424,14 +428,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.3
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     only_ffmpeg : bool, default False
         Whether to use only FFmpeg (instead of not yt-dlp) for URls
     check_sorted : bool, default True
@@ -872,14 +878,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.1
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     prepend_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Punctuations to prepend to next word.
     append_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
```

### Comparing `stable-ts-whisperless-2.16.0/README.md` & `stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: stable-ts-whisperless
+Version: 2.17.0
+Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
+Home-page: https://github.com/jianfch/stable-ts
+Author: Jian
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: torch
+Requires-Dist: torchaudio
+Requires-Dist: tqdm
+
 # Stabilizing Timestamps for Whisper
 
 This library modifies [Whisper](https://github.com/openai/whisper) to produce more reliable timestamps and extends its functionality.
 
 https://github.com/jianfch/stable-ts/assets/28970749/7adf0540-3620-4b2b-b2d4-e316906d6dfa
 
 * [Setup](#setup)
@@ -170,14 +185,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.1
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     prepend_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Punctuations to prepend to next word.
     append_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
@@ -294,14 +311,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float, default 0.1
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.1
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     only_ffmpeg : bool, default False
         Whether to use only FFmpeg (instead of not yt-dlp) for URls
     options
@@ -409,14 +428,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.3
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     only_ffmpeg : bool, default False
         Whether to use only FFmpeg (instead of not yt-dlp) for URls
     check_sorted : bool, default True
@@ -857,14 +878,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.1
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     prepend_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Punctuations to prepend to next word.
     append_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
```

### Comparing `stable-ts-whisperless-2.16.0/setup.py` & `stable-ts-whisperless-2.17.0/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_ts_whisperless.egg-info/PKG-INFO` & `stable-ts-whisperless-2.17.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: stable-ts-whisperless
-Version: 2.16.0
-Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
-Home-page: https://github.com/jianfch/stable-ts
-Author: Jian
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: torch
-Requires-Dist: torchaudio
-Requires-Dist: tqdm
-
 # Stabilizing Timestamps for Whisper
 
 This library modifies [Whisper](https://github.com/openai/whisper) to produce more reliable timestamps and extends its functionality.
 
 https://github.com/jianfch/stable-ts/assets/28970749/7adf0540-3620-4b2b-b2d4-e316906d6dfa
 
 * [Setup](#setup)
@@ -185,14 +170,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.1
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     prepend_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Punctuations to prepend to next word.
     append_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
@@ -309,14 +296,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float, default 0.1
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.1
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     only_ffmpeg : bool, default False
         Whether to use only FFmpeg (instead of not yt-dlp) for URls
     options
@@ -424,14 +413,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.3
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     only_ffmpeg : bool, default False
         Whether to use only FFmpeg (instead of not yt-dlp) for URls
     check_sorted : bool, default True
@@ -872,14 +863,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.1
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     prepend_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Punctuations to prepend to next word.
     append_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
```

### Comparing `stable-ts-whisperless-2.16.0/stable_ts_whisperless.egg-info/SOURCES.txt` & `stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/alignment.py` & `stable-ts-whisperless-2.17.0/stable_whisper/alignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .utils import safe_print, format_timestamp
 from .whisper_compatibility import warn_compatibility_issues, get_tokenizer
 from .stabilization import NonSpeechPredictor
 from .default import get_min_word_dur, get_prepend_punctuations, get_append_punctuations
 
 from .whisper_compatibility import (
     SAMPLE_RATE, N_FRAMES, N_FFT, pad_or_trim, log_mel_spectrogram, FRAMES_PER_SECOND, CHUNK_LENGTH, N_SAMPLES,
-    median_filter, DecodingTask, DecodingOptions, SuppressTokens, whisper
+    median_filter, DecodingTask, DecodingOptions, SuppressTokens, whisper, TOKENS_PER_SECOND
 )
 
 if TYPE_CHECKING:
     from .whisper_compatibility import Whisper
     from .whisper_compatibility import Tokenizer
 
 __all__ = ['align', 'refine', 'locate']
@@ -36,14 +36,15 @@
         verbose: Optional[bool] = False,
         regroup: bool = True,
         suppress_silence: bool = True,
         suppress_word_ts: bool = True,
         suppress_attention: bool = False,
         use_word_position: bool = True,
         min_word_dur: Optional[float] = None,
+        min_silence_dur: Optional[float] = None,
         nonspeech_error: float = 0.1,
         q_levels: int = 20,
         k_size: int = 5,
         vad: bool = False,
         vad_threshold: float = 0.35,
         vad_onnx: bool = False,
         denoiser: Optional[str] = None,
@@ -140,14 +141,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.1
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     prepend_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Punctuations to prepend to next word.
     append_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
@@ -203,21 +206,22 @@
     )
     prepend_punctuations = get_prepend_punctuations(prepend_punctuations)
     append_punctuations = get_append_punctuations(append_punctuations)
     min_word_dur = get_min_word_dur(min_word_dur)
     if failure_threshold is not None and (failure_threshold < 0 or failure_threshold > 1):
         raise ValueError(f'``failure_threshold`` ({failure_threshold}) must be between 0 and 1.')
     is_faster_model = model.__module__.startswith('faster_whisper.')
+    if not is_faster_model:
+        warn_compatibility_issues(whisper, ignore_compatibility)
     max_token_step = (model.max_length if is_faster_model else model.dims.n_text_ctx) - 6
     if token_step < 1:
         token_step = max_token_step
     elif token_step > max_token_step:
         raise ValueError(f'The max value for [token_step] is {max_token_step} but got {token_step}.')
 
-    warn_compatibility_issues(whisper, ignore_compatibility)
     split_indices_by_char = []
     if isinstance(text, WhisperResult):
         if language is None:
             language = text.language
         if original_split and len(text.segments) > 1 and text.has_words:
             split_indices_by_char = np.cumsum([sum(len(w.word) for w in seg.words) for seg in text.segments])
         text = text.all_tokens() if text.has_words and all(w.tokens for w in text.all_words()) else text.text
@@ -374,68 +378,143 @@
                 m.append(i+1)
         return w, wt, m
     result = []
 
     nonspeech_predictor = NonSpeechPredictor(
         vad=vad if suppress_silence else None,
         mask_pad_func=pad_or_trim,
-        get_mask=False,
+        get_mask=True,
         min_word_dur=min_word_dur,
         q_levels=q_levels,
         k_size=k_size,
         vad_threshold=vad_threshold,
         vad_onnx=vad_onnx,
         vad_window=audio.new_chunk_divisor,
         sampling_rate=SAMPLE_RATE,
         verbose=None if audio.stream else verbose,
         store_timings=True,
-        ignore_is_silent=True
+        ignore_is_silent=True,
+        min_silence_dur=min_silence_dur
     )
     audio.update_post_prep_callback(nonspeech_predictor.get_on_prep_callback(audio.stream))
     failure_count, max_fail = 0, total_words * (failure_threshold or 1)
+    all_punctuations = prepend_punctuations + append_punctuations
+
+    def fix_temp_words(target_word: dict, word_sources: List[dict], second_target: Optional[dict] = None):
+        first_word_src = word_sources[0]
+        assert target_word['word'].startswith(first_word_src['word'])
+        if target_word['word'] != first_word_src['word']:
+            if len(word_sources) < 2:
+                return None, []
+            first_word_src['probability'] = [first_word_src['probability']]
+            if first_word_src['word'].strip() in all_punctuations:
+                first_word_src['start'], first_word_src['end'] = word_sources[1]['start'], word_sources[1]['end']
+            for _ in range(len(word_sources)-1):
+                tw = word_sources.pop(1)
+                fullword = first_word_src['word'] + tw['word']
+                assert target_word['word'].startswith(fullword)
+                first_word_src['word'] = fullword
+                first_word_src['tokens'] += tw['tokens']
+                first_word_src['probability'].append(tw['probability'])
+                if tw['word'].strip() not in all_punctuations:
+                    first_word_src['end'] = tw['end']
+                if target_word['word'] == first_word_src['word']:
+                    break
+            if target_word['word'] != first_word_src['word']:
+                return None, []
+            if isinstance(first_word_src['probability'], list):
+                first_word_src['probability'] = np.mean(first_word_src['probability']).item()
+        elif second_target:
+            if len(word_sources) == 1:
+                return first_word_src, []
+            second_word_src, word_sources = fix_temp_words(second_target, word_sources[1:])
+            if second_word_src is not None:
+                word_sources = [second_word_src] + word_sources
+            return first_word_src, word_sources
+
+        return first_word_src, word_sources[1:]
+
+    def speech_percentage(_word: dict, _mask: torch.Tensor, _offset: float):
+        s, e = _word['start'], _word['end']
+        s = int((s - _offset) * TOKENS_PER_SECOND)
+        e = int((e - _offset) * TOKENS_PER_SECOND)
+        return 1 - _mask[s:e].float().mean().nan_to_num()
+
+    def is_new_better(w0, m0, o0, w1, m1, o1):
+        speech0 = speech_percentage(w0, m0, o0).round(decimals=1)
+        speech1 = speech_percentage(w1, m1, o1).round(decimals=1)
+        return speech0 >= speech1 or w0['probability'] >= w1['probability']
 
     with tqdm(total=initial_duration, unit='sec', disable=verbose is not False, desc='Align') as tqdm_pbar:
 
         def update_pbar(finish: bool = False):
             curr_total = audio.get_duration(2)
             if need_refresh := curr_total != tqdm_pbar.total:
                 tqdm_pbar.total = curr_total
             tqdm_pbar.update((curr_total if finish else min(round(last_ts, 2), curr_total)) - tqdm_pbar.n)
             if need_refresh:
                 tqdm_pbar.refresh()
             if progress_callback is not None:
                 progress_callback(seek=tqdm_pbar.n, total=tqdm_pbar.total)
 
+        def update_curr_words():
+            if temp_data['temp_word'] is not None:
+                temp_words = [temp_data['temp_word']] + temp_data['extra_words'][:len(curr_words) - 1]
+                curr_words[:len(temp_words)] = temp_words
+                temp_data['temp_word'] = None
+
         def redo_words(_idx: int = None):
-            nonlocal seg_words, seg_tokens, seg_words, words, word_tokens, curr_words, temp_word
-            if _idx is not None and curr_words and temp_word is not None:
-                assert curr_words[0]['word'] == temp_word['word']
-                if curr_words[0]['probability'] >= temp_word['probability']:
-                    temp_word = curr_words[0]
+            nonlocal seg_words, seg_tokens, seg_words, words, word_tokens, curr_words, temp_data
+            if _idx is not None and curr_words and temp_data['temp_word'] is not None:
+                temp_data['temp_word'], temp_data['extra_words'] = fix_temp_words(
+                    curr_words[0],
+                    [temp_data['temp_word']] + temp_data['extra_words'],
+                    curr_words[1] if len(curr_words) > 1 else None
+                )
+
+                if temp_data['temp_word']:
+                    use_new = is_new_better(
+                        curr_words[0], nonspeech_preds['mask'], time_offset,
+                        temp_data['temp_word'], temp_data['temp_mask'], temp_data['temp_offset']
+                    )
+                    new_extra_words = []
+                    if use_new:
+                        temp_data['temp_word'] = curr_words[0]
+                    else:
+                        for wi, (cw, tw) in enumerate(zip(curr_words[1:], temp_data['extra_words'])):
+                            assert cw['word'].startswith(tw['word'])
+                            use_new = is_new_better(
+                                cw, nonspeech_preds['mask'], time_offset,
+                                tw, temp_data['temp_mask'], temp_data['temp_offset']
+                            )
+                            if use_new or cw['word'] != tw['word'] or cw['end'] < tw['end']:
+                                break
+                            new_extra_words.append(tw)
+                    temp_data['extra_words'] = new_extra_words
+
             if _idx is None:  # redo all
                 words = seg_words + words
                 word_tokens = seg_tokens + word_tokens
                 curr_words = []
             elif _idx != len(seg_words):  # redo from _idx
                 words = seg_words[_idx:] + words
                 word_tokens = seg_tokens[_idx:] + word_tokens
-                curr_words = curr_words[:_idx]
+                curr_words, new_extra_words = curr_words[:_idx], curr_words[_idx:]
                 if curr_words:
-                    if temp_word is not None:
-                        curr_words[0] = temp_word
-                        temp_word = None
+                    update_curr_words()
                     words = seg_words[_idx-1:_idx] + words
                     word_tokens = seg_tokens[_idx-1:_idx] + word_tokens
-                    temp_word = curr_words.pop(-1)
+                    temp_data['temp_word'] = curr_words.pop(-1)
+                    temp_data['extra_words'] = new_extra_words
+                    temp_data['temp_mask'] = nonspeech_preds['mask']
+                    temp_data['temp_offset'] = time_offset
             else:
-                if temp_word is not None:
-                    curr_words[0] = temp_word
-                    temp_word = None
+                update_curr_words()
 
-        temp_word = None
+        temp_data: dict = dict(temp_word=None)
 
         while words:
 
             time_offset = seek_sample / SAMPLE_RATE
             audio_segment = audio.next_chunk(seek_sample, N_SAMPLES)
             if audio_segment is None:
                 break
@@ -557,16 +636,16 @@
             if failure_threshold is not None:
                 failure_count += sum(1 for w in curr_words if w['end'] - w['start'] == 0)
                 if failure_count > max_fail:
                     break
 
         update_pbar(failure_count <= max_fail)
 
-    if temp_word is not None:
-        result.append(temp_word)
+    if temp_data.get('temp_word') is not None:
+        result.append(temp_data['temp_word'])
     if not result:
         warnings.warn('Failed to align text.', stacklevel=2)
     if failure_count > max_fail:
         warnings.warn(f'Alignment aborted. Failed word percentage exceeded {failure_threshold * 100}% at '
                       f'{format_timestamp(seek_sample / SAMPLE_RATE)}.',
                       stacklevel=2)
     elif words:
```

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/audio/__init__.py` & `stable-ts-whisperless-2.17.0/stable_whisper/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/audio/demucs.py` & `stable-ts-whisperless-2.17.0/stable_whisper/audio/demucs.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/audio/dfnet.py` & `stable-ts-whisperless-2.17.0/stable_whisper/audio/dfnet.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/audio/noisereduce.py` & `stable-ts-whisperless-2.17.0/stable_whisper/audio/noisereduce.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/audio/output.py` & `stable-ts-whisperless-2.17.0/stable_whisper/audio/output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/audio/utils.py` & `stable-ts-whisperless-2.17.0/stable_whisper/audio/utils.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/decode.py` & `stable-ts-whisperless-2.17.0/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/default.py` & `stable-ts-whisperless-2.17.0/stable_whisper/default.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/non_whisper.py` & `stable-ts-whisperless-2.17.0/stable_whisper/non_whisper.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         denoiser_options: Optional[dict] = None,
         demucs: bool = False,
         demucs_options: dict = None,
         vad: bool = False,
         vad_threshold: float = 0.35,
         vad_onnx: bool = False,
         min_word_dur: Optional[float] = None,
+        min_silence_dur: Optional[float] = None,
         nonspeech_error: float = 0.1,
         use_word_position: bool = True,
         only_voice_freq: bool = False,
         only_ffmpeg: bool = False,
         force_order: bool = False,
         check_sorted: bool = True
 ) -> WhisperResult:
@@ -103,14 +104,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.1
         Relative error of non-speech sections that appear in between a word for silence suppression.
     use_word_position : bool, default True
         Whether to use position of the word in its segment to determine whether to keep end or start timestamps if
         adjustments are required. If it is the first word, keep end. Else if it is the last word, keep the start.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
@@ -344,15 +347,16 @@
             result.adjust_by_silence(
                 audio, vad,
                 vad_onnx=vad_onnx, vad_threshold=vad_threshold,
                 q_levels=q_levels, k_size=k_size,
                 sample_rate=curr_audio_sr(True), min_word_dur=min_word_dur,
                 word_level=suppress_word_ts, verbose=True,
                 nonspeech_error=nonspeech_error,
-                use_word_position=use_word_position
+                use_word_position=use_word_position,
+                min_silence_dur=min_silence_dur
             )
 
         if result.has_words and regroup:
             result.regroup(regroup)
 
     finally:
         if temp_audio_file is not None:
```

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/quantization.py` & `stable-ts-whisperless-2.17.0/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/result.py` & `stable-ts-whisperless-2.17.0/stable_whisper/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,6431 +15,6453 @@
 000000e0: 696d 706f 7274 2073 7570 7072 6573 735f  import suppress_
 000000f0: 7369 6c65 6e63 652c 2067 6574 5f76 6164  silence, get_vad
 00000100: 5f73 696c 656e 6365 5f66 756e 632c 2056  _silence_func, V
 00000110: 4144 5f53 414d 504c 455f 5241 5445 530d  AD_SAMPLE_RATES.
 00000120: 0a66 726f 6d20 2e73 7461 6269 6c69 7a61  .from .stabiliza
 00000130: 7469 6f6e 2e6e 6f6e 7661 6420 696d 706f  tion.nonvad impo
 00000140: 7274 2061 7564 696f 3274 696d 696e 6773  rt audio2timings
-00000150: 0d0a 6672 6f6d 202e 7465 7874 5f6f 7574  ..from .text_out
-00000160: 7075 7420 696d 706f 7274 202a 0d0a 6672  put import *..fr
-00000170: 6f6d 202e 7574 696c 7320 696d 706f 7274  om .utils import
-00000180: 2073 7472 5f74 6f5f 7661 6c69 645f 7479   str_to_valid_ty
-00000190: 7065 2c20 666f 726d 6174 5f74 696d 6573  pe, format_times
-000001a0: 7461 6d70 2c20 556e 736f 7274 6564 4578  tamp, UnsortedEx
-000001b0: 6365 7074 696f 6e0d 0a66 726f 6d20 2e61  ception..from .a
-000001c0: 7564 696f 2e75 7469 6c73 2069 6d70 6f72  udio.utils impor
-000001d0: 7420 6175 6469 6f5f 746f 5f74 656e 736f  t audio_to_tenso
-000001e0: 725f 7265 7361 6d70 6c65 0d0a 6672 6f6d  r_resample..from
-000001f0: 202e 6465 6661 756c 7420 696d 706f 7274   .default import
-00000200: 2067 6574 5f6d 696e 5f77 6f72 645f 6475   get_min_word_du
-00000210: 722c 2067 6574 5f61 7070 656e 645f 7075  r, get_append_pu
-00000220: 6e63 7475 6174 696f 6e73 2c20 6765 745f  nctuations, get_
-00000230: 7072 6570 656e 645f 7075 6e63 7475 6174  prepend_punctuat
-00000240: 696f 6e73 0d0a 0d0a 0d0a 5f5f 616c 6c5f  ions......__all_
-00000250: 5f20 3d20 5b27 5768 6973 7065 7252 6573  _ = ['WhisperRes
-00000260: 756c 7427 2c20 2753 6567 6d65 6e74 275d  ult', 'Segment']
-00000270: 0d0a 0d0a 0d0a 6465 6620 5f63 6f6d 6269  ......def _combi
-00000280: 6e65 5f61 7474 7228 6f62 6a3a 206f 626a  ne_attr(obj: obj
-00000290: 6563 742c 206f 7468 6572 5f6f 626a 3a20  ect, other_obj: 
-000002a0: 6f62 6a65 6374 2c20 6174 7472 3a20 7374  object, attr: st
-000002b0: 7229 3a0d 0a20 2020 2069 6620 2876 616c  r):..    if (val
-000002c0: 203a 3d20 6765 7461 7474 7228 6f62 6a2c   := getattr(obj,
-000002d0: 2061 7474 7229 2920 6973 206e 6f74 204e   attr)) is not N
-000002e0: 6f6e 653a 0d0a 2020 2020 2020 2020 6f74  one:..        ot
-000002f0: 6865 725f 7661 6c20 3d20 6765 7461 7474  her_val = getatt
-00000300: 7228 6f74 6865 725f 6f62 6a2c 2061 7474  r(other_obj, att
-00000310: 7229 0d0a 2020 2020 2020 2020 6966 2069  r)..        if i
-00000320: 7369 6e73 7461 6e63 6528 7661 6c2c 206c  sinstance(val, l
-00000330: 6973 7429 3a0d 0a20 2020 2020 2020 2020  ist):..         
-00000340: 2020 2069 6620 6f74 6865 725f 7661 6c20     if other_val 
-00000350: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00000360: 2020 2020 2020 2020 2020 7365 7461 7474            setatt
-00000370: 7228 6f62 6a2c 2061 7474 722c 204e 6f6e  r(obj, attr, Non
-00000380: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00000390: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000003a0: 2020 2020 2020 2076 616c 2e65 7874 656e         val.exten
-000003b0: 6428 6f74 6865 725f 7661 6c29 0d0a 2020  d(other_val)..  
-000003c0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-000003d0: 2020 2020 2020 2020 206e 6577 5f76 616c           new_val
-000003e0: 203d 204e 6f6e 6520 6966 206f 7468 6572   = None if other
-000003f0: 5f76 616c 2069 7320 4e6f 6e65 2065 6c73  _val is None els
-00000400: 6520 2828 7661 6c20 2b20 6f74 6865 725f  e ((val + other_
-00000410: 7661 6c29 202f 2032 290d 0a20 2020 2020  val) / 2)..     
-00000420: 2020 2020 2020 2073 6574 6174 7472 286f         setattr(o
-00000430: 626a 2c20 6174 7472 2c20 6e65 775f 7661  bj, attr, new_va
-00000440: 6c29 0d0a 0d0a 0d0a 6465 6620 5f69 6e63  l)......def _inc
-00000450: 7265 6d65 6e74 5f61 7474 7228 6f62 6a3a  rement_attr(obj:
-00000460: 206f 626a 6563 742c 2061 7474 723a 2073   object, attr: s
-00000470: 7472 2c20 7661 6c3a 2055 6e69 6f6e 5b69  tr, val: Union[i
-00000480: 6e74 2c20 666c 6f61 745d 293a 0d0a 2020  nt, float]):..  
-00000490: 2020 6966 2028 6375 7272 5f76 616c 203a    if (curr_val :
-000004a0: 3d20 6765 7461 7474 7228 6f62 6a2c 2061  = getattr(obj, a
-000004b0: 7474 722c 204e 6f6e 6529 2920 6973 206e  ttr, None)) is n
-000004c0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-000004d0: 2020 7365 7461 7474 7228 6f62 6a2c 2061    setattr(obj, a
-000004e0: 7474 722c 2063 7572 725f 7661 6c20 2b20  ttr, curr_val + 
-000004f0: 7661 6c29 0d0a 0d0a 0d0a 6465 6620 5f72  val)......def _r
-00000500: 6f75 6e64 5f74 696d 6573 7461 6d70 2874  ound_timestamp(t
-00000510: 733a 2055 6e69 6f6e 5b66 6c6f 6174 2c20  s: Union[float, 
-00000520: 4e6f 6e65 5d29 3a0d 0a20 2020 2069 6620  None]):..    if 
-00000530: 6e6f 7420 7473 3a0d 0a20 2020 2020 2020  not ts:..       
-00000540: 2072 6574 7572 6e20 7473 0d0a 2020 2020   return ts..    
-00000550: 7265 7475 726e 2072 6f75 6e64 2874 732c  return round(ts,
-00000560: 2033 290d 0a0d 0a0d 0a63 6c61 7373 2057   3)......class W
-00000570: 6f72 6454 696d 696e 673a 0d0a 0d0a 2020  ordTiming:....  
-00000580: 2020 6465 6620 5f5f 696e 6974 5f5f 280d    def __init__(.
-00000590: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000005a0: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
-000005b0: 776f 7264 3a20 7374 722c 0d0a 2020 2020  word: str,..    
-000005c0: 2020 2020 2020 2020 7374 6172 743a 2066          start: f
-000005d0: 6c6f 6174 2c0d 0a20 2020 2020 2020 2020  loat,..         
-000005e0: 2020 2065 6e64 3a20 666c 6f61 742c 0d0a     end: float,..
-000005f0: 2020 2020 2020 2020 2020 2020 7072 6f62              prob
-00000600: 6162 696c 6974 793a 204f 7074 696f 6e61  ability: Optiona
-00000610: 6c5b 666c 6f61 745d 203d 204e 6f6e 652c  l[float] = None,
-00000620: 0d0a 2020 2020 2020 2020 2020 2020 746f  ..            to
-00000630: 6b65 6e73 3a20 4f70 7469 6f6e 616c 5b4c  kens: Optional[L
-00000640: 6973 745b 696e 745d 5d20 3d20 4e6f 6e65  ist[int]] = None
-00000650: 2c0d 0a20 2020 2020 2020 2020 2020 206c  ,..            l
-00000660: 6566 745f 6c6f 636b 6564 3a20 626f 6f6c  eft_locked: bool
-00000670: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
-00000680: 2020 2020 2020 2072 6967 6874 5f6c 6f63         right_loc
-00000690: 6b65 643a 2062 6f6f 6c20 3d20 4661 6c73  ked: bool = Fals
-000006a0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000006b0: 7365 676d 656e 745f 6964 3a20 4f70 7469  segment_id: Opti
-000006c0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-000006d0: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
-000006e0: 643a 204f 7074 696f 6e61 6c5b 696e 745d  d: Optional[int]
-000006f0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00000700: 2020 2020 2020 7365 676d 656e 743a 204f        segment: O
-00000710: 7074 696f 6e61 6c5b 2753 6567 6d65 6e74  ptional['Segment
-00000720: 275d 203d 204e 6f6e 652c 0d0a 2020 2020  '] = None,..    
-00000730: 2020 2020 2020 2020 726f 756e 645f 7473          round_ts
-00000740: 3a20 626f 6f6c 203d 2054 7275 652c 0d0a  : bool = True,..
-00000750: 2020 2020 2020 2020 2020 2020 6967 6e6f              igno
-00000760: 7265 5f75 6e75 7365 645f 6172 6773 3a20  re_unused_args: 
-00000770: 626f 6f6c 203d 2046 616c 7365 0d0a 2020  bool = False..  
-00000780: 2020 293a 0d0a 2020 2020 2020 2020 6966    ):..        if
-00000790: 206e 6f74 2069 676e 6f72 655f 756e 7573   not ignore_unus
-000007a0: 6564 5f61 7267 7320 616e 6420 7365 676d  ed_args and segm
-000007b0: 656e 745f 6964 2069 7320 6e6f 7420 4e6f  ent_id is not No
-000007c0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-000007d0: 2077 6172 6e69 6e67 732e 7761 726e 2827   warnings.warn('
-000007e0: 5468 6520 7061 7261 6d65 7465 7220 6060  The parameter ``
-000007f0: 7365 676d 656e 745f 6964 6060 2069 7320  segment_id`` is 
-00000800: 6967 6e6f 7265 642e 2027 0d0a 2020 2020  ignored. '..    
-00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000820: 2020 2020 2020 2753 7065 6369 6679 2074        'Specify t
-00000830: 6865 2063 7572 7265 6e74 2073 6567 6d65  he current segme
-00000840: 6e74 2069 6e73 7461 6e63 6520 7769 7468  nt instance with
-00000850: 2060 6073 6567 6d65 6e74 6060 2e27 2c0d   ``segment``.',.
-00000860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000870: 2020 2020 2020 2020 2020 2073 7461 636b             stack
-00000880: 6c65 7665 6c3d 3229 0d0a 2020 2020 2020  level=2)..      
-00000890: 2020 7365 6c66 2e72 6f75 6e64 5f74 7320    self.round_ts 
-000008a0: 3d20 726f 756e 645f 7473 0d0a 2020 2020  = round_ts..    
-000008b0: 2020 2020 7365 6c66 2e77 6f72 6420 3d20      self.word = 
-000008c0: 776f 7264 0d0a 2020 2020 2020 2020 7365  word..        se
-000008d0: 6c66 2e5f 7374 6172 7420 3d20 7365 6c66  lf._start = self
-000008e0: 2e72 6f75 6e64 2873 7461 7274 290d 0a20  .round(start).. 
-000008f0: 2020 2020 2020 2073 656c 662e 5f65 6e64         self._end
-00000900: 203d 2073 656c 662e 726f 756e 6428 656e   = self.round(en
-00000910: 6429 0d0a 2020 2020 2020 2020 7365 6c66  d)..        self
-00000920: 2e70 726f 6261 6269 6c69 7479 203d 2070  .probability = p
-00000930: 726f 6261 6269 6c69 7479 0d0a 2020 2020  robability..    
-00000940: 2020 2020 7365 6c66 2e74 6f6b 656e 7320      self.tokens 
-00000950: 3d20 746f 6b65 6e73 0d0a 2020 2020 2020  = tokens..      
-00000960: 2020 7365 6c66 2e6c 6566 745f 6c6f 636b    self.left_lock
-00000970: 6564 203d 206c 6566 745f 6c6f 636b 6564  ed = left_locked
-00000980: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-00000990: 6967 6874 5f6c 6f63 6b65 6420 3d20 7269  ight_locked = ri
-000009a0: 6768 745f 6c6f 636b 6564 0d0a 2020 2020  ght_locked..    
-000009b0: 2020 2020 7365 6c66 2e73 6567 6d65 6e74      self.segment
-000009c0: 203d 2073 6567 6d65 6e74 0d0a 2020 2020   = segment..    
-000009d0: 2020 2020 7365 6c66 2e69 6420 3d20 6964      self.id = id
-000009e0: 0d0a 0d0a 2020 2020 6465 6620 5f5f 7265  ....    def __re
-000009f0: 7072 5f5f 2873 656c 6629 3a0d 0a20 2020  pr__(self):..   
-00000a00: 2020 2020 2072 6574 7572 6e20 6627 576f       return f'Wo
-00000a10: 7264 5469 6d69 6e67 2873 7461 7274 3d7b  rdTiming(start={
-00000a20: 7365 6c66 2e73 7461 7274 7d2c 2065 6e64  self.start}, end
-00000a30: 3d7b 7365 6c66 2e65 6e64 7d2c 2077 6f72  ={self.end}, wor
-00000a40: 643d 227b 7365 6c66 2e77 6f72 647d 2229  d="{self.word}")
-00000a50: 270d 0a0d 0a20 2020 2064 6566 205f 5f6c  '....    def __l
-00000a60: 656e 5f5f 2873 656c 6629 3a0d 0a20 2020  en__(self):..   
-00000a70: 2020 2020 2072 6574 7572 6e20 6c65 6e28       return len(
-00000a80: 7365 6c66 2e77 6f72 6429 0d0a 0d0a 2020  self.word)....  
-00000a90: 2020 6465 6620 5f5f 6164 645f 5f28 7365    def __add__(se
-00000aa0: 6c66 2c20 6f74 6865 723a 2027 576f 7264  lf, other: 'Word
-00000ab0: 5469 6d69 6e67 2729 3a0d 0a20 2020 2020  Timing'):..     
-00000ac0: 2020 2073 656c 665f 636f 7079 203d 2057     self_copy = W
-00000ad0: 6f72 6454 696d 696e 6728 0d0a 2020 2020  ordTiming(..    
-00000ae0: 2020 2020 2020 2020 776f 7264 3d73 656c          word=sel
-00000af0: 662e 776f 7264 202b 206f 7468 6572 2e77  f.word + other.w
-00000b00: 6f72 642c 0d0a 2020 2020 2020 2020 2020  ord,..          
-00000b10: 2020 7374 6172 743d 6d69 6e28 7365 6c66    start=min(self
-00000b20: 2e73 7461 7274 2c20 6f74 6865 722e 7374  .start, other.st
-00000b30: 6172 7429 2c0d 0a20 2020 2020 2020 2020  art),..         
-00000b40: 2020 2065 6e64 3d6d 6178 2873 656c 662e     end=max(self.
-00000b50: 656e 642c 206f 7468 6572 2e65 6e64 292c  end, other.end),
-00000b60: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00000b70: 6f62 6162 696c 6974 793d 7365 6c66 2e70  obability=self.p
-00000b80: 726f 6261 6269 6c69 7479 2c0d 0a20 2020  robability,..   
-00000b90: 2020 2020 2020 2020 2074 6f6b 656e 733d           tokens=
-00000ba0: 4e6f 6e65 2069 6620 7365 6c66 2e74 6f6b  None if self.tok
-00000bb0: 656e 7320 6973 204e 6f6e 6520 656c 7365  ens is None else
-00000bc0: 2073 656c 662e 746f 6b65 6e73 2e63 6f70   self.tokens.cop
-00000bd0: 7928 292c 0d0a 2020 2020 2020 2020 2020  y(),..          
-00000be0: 2020 6c65 6674 5f6c 6f63 6b65 643d 7365    left_locked=se
-00000bf0: 6c66 2e6c 6566 745f 6c6f 636b 6564 206f  lf.left_locked o
-00000c00: 7220 6f74 6865 722e 6c65 6674 5f6c 6f63  r other.left_loc
-00000c10: 6b65 642c 0d0a 2020 2020 2020 2020 2020  ked,..          
-00000c20: 2020 7269 6768 745f 6c6f 636b 6564 3d73    right_locked=s
-00000c30: 656c 662e 7269 6768 745f 6c6f 636b 6564  elf.right_locked
-00000c40: 206f 7220 6f74 6865 722e 7269 6768 745f   or other.right_
-00000c50: 6c6f 636b 6564 2c0d 0a20 2020 2020 2020  locked,..       
-00000c60: 2020 2020 2069 643d 7365 6c66 2e69 642c       id=self.id,
-00000c70: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00000c80: 676d 656e 743d 7365 6c66 2e73 6567 6d65  gment=self.segme
-00000c90: 6e74 0d0a 2020 2020 2020 2020 290d 0a20  nt..        ).. 
-00000ca0: 2020 2020 2020 205f 636f 6d62 696e 655f         _combine_
-00000cb0: 6174 7472 2873 656c 665f 636f 7079 2c20  attr(self_copy, 
-00000cc0: 6f74 6865 722c 2027 7072 6f62 6162 696c  other, 'probabil
-00000cd0: 6974 7927 290d 0a20 2020 2020 2020 205f  ity')..        _
-00000ce0: 636f 6d62 696e 655f 6174 7472 2873 656c  combine_attr(sel
-00000cf0: 665f 636f 7079 2c20 6f74 6865 722c 2027  f_copy, other, '
-00000d00: 746f 6b65 6e73 2729 0d0a 0d0a 2020 2020  tokens')....    
-00000d10: 2020 2020 7265 7475 726e 2073 656c 665f      return self_
-00000d20: 636f 7079 0d0a 0d0a 2020 2020 6465 6620  copy....    def 
-00000d30: 5f5f 6465 6570 636f 7079 5f5f 2873 656c  __deepcopy__(sel
-00000d40: 662c 206d 656d 6f3d 4e6f 6e65 293a 0d0a  f, memo=None):..
-00000d50: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00000d60: 656c 662e 636f 7079 2863 6f70 795f 746f  elf.copy(copy_to
-00000d70: 6b65 6e73 3d54 7275 6529 0d0a 0d0a 2020  kens=True)....  
-00000d80: 2020 6465 6620 5f5f 636f 7079 5f5f 2873    def __copy__(s
-00000d90: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00000da0: 6574 7572 6e20 7365 6c66 2e63 6f70 7928  eturn self.copy(
-00000db0: 290d 0a0d 0a20 2020 2064 6566 2063 6f70  )....    def cop
-00000dc0: 7928 0d0a 2020 2020 2020 2020 2020 2020  y(..            
-00000dd0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-00000de0: 2020 206b 6565 705f 7365 676d 656e 743a     keep_segment:
-00000df0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
-00000e00: 2020 2020 2020 2020 2020 2020 636f 7079              copy
-00000e10: 5f74 6f6b 656e 733a 2062 6f6f 6c20 3d20  _tokens: bool = 
-00000e20: 4661 6c73 650d 0a20 2020 2029 3a0d 0a20  False..    ):.. 
-00000e30: 2020 2020 2020 2072 6574 7572 6e20 576f         return Wo
-00000e40: 7264 5469 6d69 6e67 280d 0a20 2020 2020  rdTiming(..     
-00000e50: 2020 2020 2020 2077 6f72 643d 7365 6c66         word=self
-00000e60: 2e77 6f72 642c 0d0a 2020 2020 2020 2020  .word,..        
-00000e70: 2020 2020 7374 6172 743d 7365 6c66 2e73      start=self.s
-00000e80: 7461 7274 2c0d 0a20 2020 2020 2020 2020  tart,..         
-00000e90: 2020 2065 6e64 3d73 656c 662e 656e 642c     end=self.end,
-00000ea0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00000eb0: 6f62 6162 696c 6974 793d 7365 6c66 2e70  obability=self.p
-00000ec0: 726f 6261 6269 6c69 7479 2c0d 0a20 2020  robability,..   
-00000ed0: 2020 2020 2020 2020 2074 6f6b 656e 733d           tokens=
-00000ee0: 4e6f 6e65 2069 6620 2873 656c 662e 746f  None if (self.to
-00000ef0: 6b65 6e73 2069 7320 4e6f 6e65 2920 656c  kens is None) el
-00000f00: 7365 2028 7365 6c66 2e74 6f6b 656e 732e  se (self.tokens.
-00000f10: 636f 7079 2829 2069 6620 636f 7079 5f74  copy() if copy_t
-00000f20: 6f6b 656e 7320 656c 7365 2073 656c 662e  okens else self.
-00000f30: 746f 6b65 6e73 292c 0d0a 2020 2020 2020  tokens),..      
-00000f40: 2020 2020 2020 6c65 6674 5f6c 6f63 6b65        left_locke
-00000f50: 643d 7365 6c66 2e6c 6566 745f 6c6f 636b  d=self.left_lock
-00000f60: 6564 2c0d 0a20 2020 2020 2020 2020 2020  ed,..           
-00000f70: 2072 6967 6874 5f6c 6f63 6b65 643d 7365   right_locked=se
-00000f80: 6c66 2e72 6967 6874 5f6c 6f63 6b65 642c  lf.right_locked,
-00000f90: 0d0a 2020 2020 2020 2020 2020 2020 6964  ..            id
-00000fa0: 3d73 656c 662e 6964 2c0d 0a20 2020 2020  =self.id,..     
-00000fb0: 2020 2020 2020 2073 6567 6d65 6e74 3d73         segment=s
-00000fc0: 656c 662e 7365 676d 656e 7420 6966 206b  elf.segment if k
-00000fd0: 6565 705f 7365 676d 656e 7420 656c 7365  eep_segment else
-00000fe0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00000ff0: 2020 2020 726f 756e 645f 7473 3d73 656c      round_ts=sel
-00001000: 662e 726f 756e 645f 7473 0d0a 2020 2020  f.round_ts..    
-00001010: 2020 2020 290d 0a0d 0a20 2020 2064 6566      )....    def
-00001020: 2072 6f75 6e64 2873 656c 662c 2074 696d   round(self, tim
-00001030: 6573 7461 6d70 3a20 666c 6f61 7429 202d  estamp: float) -
-00001040: 3e20 666c 6f61 743a 0d0a 2020 2020 2020  > float:..      
-00001050: 2020 6966 206e 6f74 2073 656c 662e 726f    if not self.ro
-00001060: 756e 645f 7473 3a0d 0a20 2020 2020 2020  und_ts:..       
-00001070: 2020 2020 2072 6574 7572 6e20 7469 6d65       return time
-00001080: 7374 616d 700d 0a20 2020 2020 2020 2072  stamp..        r
-00001090: 6574 7572 6e20 5f72 6f75 6e64 5f74 696d  eturn _round_tim
-000010a0: 6573 7461 6d70 2874 696d 6573 7461 6d70  estamp(timestamp
-000010b0: 290d 0a0d 0a20 2020 2040 7072 6f70 6572  )....    @proper
-000010c0: 7479 0d0a 2020 2020 6465 6620 7374 6172  ty..    def star
-000010d0: 7428 7365 6c66 293a 0d0a 2020 2020 2020  t(self):..      
-000010e0: 2020 7265 7475 726e 2073 656c 662e 5f73    return self._s
-000010f0: 7461 7274 0d0a 0d0a 2020 2020 4070 726f  tart....    @pro
-00001100: 7065 7274 790d 0a20 2020 2064 6566 2065  perty..    def e
-00001110: 6e64 2873 656c 6629 3a0d 0a20 2020 2020  nd(self):..     
-00001120: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00001130: 656e 640d 0a0d 0a20 2020 2040 7374 6172  end....    @star
-00001140: 742e 7365 7474 6572 0d0a 2020 2020 6465  t.setter..    de
-00001150: 6620 7374 6172 7428 7365 6c66 2c20 7661  f start(self, va
-00001160: 6c29 3a0d 0a20 2020 2020 2020 2073 656c  l):..        sel
-00001170: 662e 5f73 7461 7274 203d 2073 656c 662e  f._start = self.
-00001180: 726f 756e 6428 7661 6c29 0d0a 0d0a 2020  round(val)....  
-00001190: 2020 4065 6e64 2e73 6574 7465 720d 0a20    @end.setter.. 
-000011a0: 2020 2064 6566 2065 6e64 2873 656c 662c     def end(self,
-000011b0: 2076 616c 293a 0d0a 2020 2020 2020 2020   val):..        
-000011c0: 7365 6c66 2e5f 656e 6420 3d20 7365 6c66  self._end = self
-000011d0: 2e72 6f75 6e64 2876 616c 290d 0a0d 0a20  .round(val).... 
-000011e0: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
-000011f0: 2020 6465 6620 7365 676d 656e 745f 6964    def segment_id
-00001200: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00001210: 2072 6574 7572 6e20 4e6f 6e65 2069 6620   return None if 
-00001220: 7365 6c66 2e73 6567 6d65 6e74 2069 7320  self.segment is 
-00001230: 4e6f 6e65 2065 6c73 6520 7365 6c66 2e73  None else self.s
-00001240: 6567 6d65 6e74 2e69 640d 0a0d 0a20 2020  egment.id....   
-00001250: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-00001260: 6465 6620 6475 7261 7469 6f6e 2873 656c  def duration(sel
-00001270: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-00001280: 7572 6e20 7365 6c66 2e72 6f75 6e64 2873  urn self.round(s
-00001290: 656c 662e 656e 6420 2d20 7365 6c66 2e73  elf.end - self.s
-000012a0: 7461 7274 290d 0a0d 0a20 2020 2064 6566  tart)....    def
-000012b0: 2072 6f75 6e64 5f61 6c6c 5f74 696d 6573   round_all_times
-000012c0: 7461 6d70 7328 7365 6c66 293a 0d0a 2020  tamps(self):..  
-000012d0: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-000012e0: 6172 6e28 2760 602e 726f 756e 645f 616c  arn('``.round_al
-000012f0: 6c5f 7469 6d65 7374 616d 7073 2829 6060  l_timestamps()``
-00001300: 2069 7320 6465 7072 6563 6174 6564 2061   is deprecated a
-00001310: 6e64 2077 696c 6c20 6265 2072 656d 6f76  nd will be remov
-00001320: 6564 2069 6e20 6675 7475 7265 2076 6572  ed in future ver
-00001330: 7369 6f6e 732e 2027 0d0a 2020 2020 2020  sions. '..      
-00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001350: 2755 7365 2060 602e 726f 756e 645f 7473  'Use ``.round_ts
-00001360: 3d54 7275 6560 6020 746f 2072 6f75 6e64  =True`` to round
-00001370: 2074 696d 6573 7461 6d70 7320 6279 2064   timestamps by d
-00001380: 6566 6175 6c74 2069 6e73 7465 6164 2e27  efault instead.'
-00001390: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000013a0: 2020 2020 2020 2020 2073 7461 636b 6c65           stackle
-000013b0: 7665 6c3d 3229 0d0a 2020 2020 2020 2020  vel=2)..        
-000013c0: 7365 6c66 2e72 6f75 6e64 5f74 7320 3d20  self.round_ts = 
-000013d0: 5472 7565 0d0a 0d0a 2020 2020 6465 6620  True....    def 
-000013e0: 6f66 6673 6574 5f74 696d 6528 7365 6c66  offset_time(self
-000013f0: 2c20 6f66 6673 6574 5f73 6563 6f6e 6473  , offset_seconds
-00001400: 3a20 666c 6f61 7429 3a0d 0a20 2020 2020  : float):..     
-00001410: 2020 2073 656c 662e 7374 6172 7420 3d20     self.start = 
-00001420: 7365 6c66 2e73 7461 7274 202b 206f 6666  self.start + off
-00001430: 7365 745f 7365 636f 6e64 730d 0a20 2020  set_seconds..   
-00001440: 2020 2020 2073 656c 662e 656e 6420 3d20       self.end = 
-00001450: 7365 6c66 2e65 6e64 202b 206f 6666 7365  self.end + offse
-00001460: 745f 7365 636f 6e64 730d 0a0d 0a20 2020  t_seconds....   
-00001470: 2064 6566 2074 6f5f 6469 6374 2873 656c   def to_dict(sel
-00001480: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-00001490: 7572 6e20 6469 6374 280d 0a20 2020 2020  urn dict(..     
-000014a0: 2020 2020 2020 2077 6f72 643d 7365 6c66         word=self
-000014b0: 2e77 6f72 642c 0d0a 2020 2020 2020 2020  .word,..        
-000014c0: 2020 2020 7374 6172 743d 7365 6c66 2e73      start=self.s
-000014d0: 7461 7274 2c0d 0a20 2020 2020 2020 2020  tart,..         
-000014e0: 2020 2065 6e64 3d73 656c 662e 656e 642c     end=self.end,
-000014f0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00001500: 6f62 6162 696c 6974 793d 7365 6c66 2e70  obability=self.p
-00001510: 726f 6261 6269 6c69 7479 2c0d 0a20 2020  robability,..   
-00001520: 2020 2020 2020 2020 2074 6f6b 656e 733d           tokens=
-00001530: 4e6f 6e65 2069 6620 7365 6c66 2e74 6f6b  None if self.tok
-00001540: 656e 7320 6973 204e 6f6e 6520 656c 7365  ens is None else
-00001550: 2073 656c 662e 746f 6b65 6e73 2e63 6f70   self.tokens.cop
-00001560: 7928 290d 0a20 2020 2020 2020 2029 0d0a  y()..        )..
-00001570: 0d0a 2020 2020 6465 6620 6c6f 636b 5f6c  ..    def lock_l
-00001580: 6566 7428 7365 6c66 293a 0d0a 2020 2020  eft(self):..    
-00001590: 2020 2020 7365 6c66 2e6c 6566 745f 6c6f      self.left_lo
-000015a0: 636b 6564 203d 2054 7275 650d 0a0d 0a20  cked = True.... 
-000015b0: 2020 2064 6566 206c 6f63 6b5f 7269 6768     def lock_righ
-000015c0: 7428 7365 6c66 293a 0d0a 2020 2020 2020  t(self):..      
-000015d0: 2020 7365 6c66 2e72 6967 6874 5f6c 6f63    self.right_loc
-000015e0: 6b65 6420 3d20 5472 7565 0d0a 0d0a 2020  ked = True....  
-000015f0: 2020 6465 6620 6c6f 636b 5f62 6f74 6828    def lock_both(
-00001600: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00001610: 7365 6c66 2e6c 6f63 6b5f 6c65 6674 2829  self.lock_left()
-00001620: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00001630: 6f63 6b5f 7269 6768 7428 290d 0a0d 0a20  ock_right().... 
-00001640: 2020 2064 6566 2075 6e6c 6f63 6b5f 626f     def unlock_bo
-00001650: 7468 2873 656c 6629 3a0d 0a20 2020 2020  th(self):..     
-00001660: 2020 2073 656c 662e 6c65 6674 5f6c 6f63     self.left_loc
-00001670: 6b65 6420 3d20 4661 6c73 650d 0a20 2020  ked = False..   
-00001680: 2020 2020 2073 656c 662e 7269 6768 745f       self.right_
-00001690: 6c6f 636b 6564 203d 2046 616c 7365 0d0a  locked = False..
-000016a0: 0d0a 2020 2020 6465 6620 7375 7070 7265  ..    def suppre
-000016b0: 7373 5f73 696c 656e 6365 2873 656c 662c  ss_silence(self,
-000016c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000016d0: 2020 2020 2020 2020 2020 2073 696c 656e             silen
-000016e0: 745f 7374 6172 7473 3a20 6e70 2e6e 6461  t_starts: np.nda
-000016f0: 7272 6179 2c0d 0a20 2020 2020 2020 2020  rray,..         
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 7369 6c65 6e74 5f65 6e64 733a 206e 702e  silent_ends: np.
-00001720: 6e64 6172 7261 792c 0d0a 2020 2020 2020  ndarray,..      
+00000150: 0d0a 6672 6f6d 202e 7374 6162 696c 697a  ..from .stabiliz
+00000160: 6174 696f 6e2e 7574 696c 7320 696d 706f  ation.utils impo
+00000170: 7274 2066 696c 7465 725f 7469 6d69 6e67  rt filter_timing
+00000180: 730d 0a66 726f 6d20 2e74 6578 745f 6f75  s..from .text_ou
+00000190: 7470 7574 2069 6d70 6f72 7420 2a0d 0a66  tput import *..f
+000001a0: 726f 6d20 2e75 7469 6c73 2069 6d70 6f72  rom .utils impor
+000001b0: 7420 7374 725f 746f 5f76 616c 6964 5f74  t str_to_valid_t
+000001c0: 7970 652c 2066 6f72 6d61 745f 7469 6d65  ype, format_time
+000001d0: 7374 616d 702c 2055 6e73 6f72 7465 6445  stamp, UnsortedE
+000001e0: 7863 6570 7469 6f6e 0d0a 6672 6f6d 202e  xception..from .
+000001f0: 6175 6469 6f2e 7574 696c 7320 696d 706f  audio.utils impo
+00000200: 7274 2061 7564 696f 5f74 6f5f 7465 6e73  rt audio_to_tens
+00000210: 6f72 5f72 6573 616d 706c 650d 0a66 726f  or_resample..fro
+00000220: 6d20 2e64 6566 6175 6c74 2069 6d70 6f72  m .default impor
+00000230: 7420 6765 745f 6d69 6e5f 776f 7264 5f64  t get_min_word_d
+00000240: 7572 2c20 6765 745f 6170 7065 6e64 5f70  ur, get_append_p
+00000250: 756e 6374 7561 7469 6f6e 732c 2067 6574  unctuations, get
+00000260: 5f70 7265 7065 6e64 5f70 756e 6374 7561  _prepend_punctua
+00000270: 7469 6f6e 730d 0a0d 0a0d 0a5f 5f61 6c6c  tions......__all
+00000280: 5f5f 203d 205b 2757 6869 7370 6572 5265  __ = ['WhisperRe
+00000290: 7375 6c74 272c 2027 5365 676d 656e 7427  sult', 'Segment'
+000002a0: 5d0d 0a0d 0a0d 0a64 6566 205f 636f 6d62  ]......def _comb
+000002b0: 696e 655f 6174 7472 286f 626a 3a20 6f62  ine_attr(obj: ob
+000002c0: 6a65 6374 2c20 6f74 6865 725f 6f62 6a3a  ject, other_obj:
+000002d0: 206f 626a 6563 742c 2061 7474 723a 2073   object, attr: s
+000002e0: 7472 293a 0d0a 2020 2020 6966 2028 7661  tr):..    if (va
+000002f0: 6c20 3a3d 2067 6574 6174 7472 286f 626a  l := getattr(obj
+00000300: 2c20 6174 7472 2929 2069 7320 6e6f 7420  , attr)) is not 
+00000310: 4e6f 6e65 3a0d 0a20 2020 2020 2020 206f  None:..        o
+00000320: 7468 6572 5f76 616c 203d 2067 6574 6174  ther_val = getat
+00000330: 7472 286f 7468 6572 5f6f 626a 2c20 6174  tr(other_obj, at
+00000340: 7472 290d 0a20 2020 2020 2020 2069 6620  tr)..        if 
+00000350: 6973 696e 7374 616e 6365 2876 616c 2c20  isinstance(val, 
+00000360: 6c69 7374 293a 0d0a 2020 2020 2020 2020  list):..        
+00000370: 2020 2020 6966 206f 7468 6572 5f76 616c      if other_val
+00000380: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00000390: 2020 2020 2020 2020 2020 2073 6574 6174             setat
+000003a0: 7472 286f 626a 2c20 6174 7472 2c20 4e6f  tr(obj, attr, No
+000003b0: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
+000003c0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+000003d0: 2020 2020 2020 2020 7661 6c2e 6578 7465          val.exte
+000003e0: 6e64 286f 7468 6572 5f76 616c 290d 0a20  nd(other_val).. 
+000003f0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00000400: 2020 2020 2020 2020 2020 6e65 775f 7661            new_va
+00000410: 6c20 3d20 4e6f 6e65 2069 6620 6f74 6865  l = None if othe
+00000420: 725f 7661 6c20 6973 204e 6f6e 6520 656c  r_val is None el
+00000430: 7365 2028 2876 616c 202b 206f 7468 6572  se ((val + other
+00000440: 5f76 616c 2920 2f20 3229 0d0a 2020 2020  _val) / 2)..    
+00000450: 2020 2020 2020 2020 7365 7461 7474 7228          setattr(
+00000460: 6f62 6a2c 2061 7474 722c 206e 6577 5f76  obj, attr, new_v
+00000470: 616c 290d 0a0d 0a0d 0a64 6566 205f 696e  al)......def _in
+00000480: 6372 656d 656e 745f 6174 7472 286f 626a  crement_attr(obj
+00000490: 3a20 6f62 6a65 6374 2c20 6174 7472 3a20  : object, attr: 
+000004a0: 7374 722c 2076 616c 3a20 556e 696f 6e5b  str, val: Union[
+000004b0: 696e 742c 2066 6c6f 6174 5d29 3a0d 0a20  int, float]):.. 
+000004c0: 2020 2069 6620 2863 7572 725f 7661 6c20     if (curr_val 
+000004d0: 3a3d 2067 6574 6174 7472 286f 626a 2c20  := getattr(obj, 
+000004e0: 6174 7472 2c20 4e6f 6e65 2929 2069 7320  attr, None)) is 
+000004f0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00000500: 2020 2073 6574 6174 7472 286f 626a 2c20     setattr(obj, 
+00000510: 6174 7472 2c20 6375 7272 5f76 616c 202b  attr, curr_val +
+00000520: 2076 616c 290d 0a0d 0a0d 0a64 6566 205f   val)......def _
+00000530: 726f 756e 645f 7469 6d65 7374 616d 7028  round_timestamp(
+00000540: 7473 3a20 556e 696f 6e5b 666c 6f61 742c  ts: Union[float,
+00000550: 204e 6f6e 655d 293a 0d0a 2020 2020 6966   None]):..    if
+00000560: 206e 6f74 2074 733a 0d0a 2020 2020 2020   not ts:..      
+00000570: 2020 7265 7475 726e 2074 730d 0a20 2020    return ts..   
+00000580: 2072 6574 7572 6e20 726f 756e 6428 7473   return round(ts
+00000590: 2c20 3329 0d0a 0d0a 0d0a 636c 6173 7320  , 3)......class 
+000005a0: 576f 7264 5469 6d69 6e67 3a0d 0a0d 0a20  WordTiming:.... 
+000005b0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000005c0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+000005d0: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
+000005e0: 2077 6f72 643a 2073 7472 2c0d 0a20 2020   word: str,..   
+000005f0: 2020 2020 2020 2020 2073 7461 7274 3a20           start: 
+00000600: 666c 6f61 742c 0d0a 2020 2020 2020 2020  float,..        
+00000610: 2020 2020 656e 643a 2066 6c6f 6174 2c0d      end: float,.
+00000620: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+00000630: 6261 6269 6c69 7479 3a20 4f70 7469 6f6e  bability: Option
+00000640: 616c 5b66 6c6f 6174 5d20 3d20 4e6f 6e65  al[float] = None
+00000650: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+00000660: 6f6b 656e 733a 204f 7074 696f 6e61 6c5b  okens: Optional[
+00000670: 4c69 7374 5b69 6e74 5d5d 203d 204e 6f6e  List[int]] = Non
+00000680: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00000690: 6c65 6674 5f6c 6f63 6b65 643a 2062 6f6f  left_locked: boo
+000006a0: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
+000006b0: 2020 2020 2020 2020 7269 6768 745f 6c6f          right_lo
+000006c0: 636b 6564 3a20 626f 6f6c 203d 2046 616c  cked: bool = Fal
+000006d0: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
+000006e0: 2073 6567 6d65 6e74 5f69 643a 204f 7074   segment_id: Opt
+000006f0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00000700: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00000710: 6964 3a20 4f70 7469 6f6e 616c 5b69 6e74  id: Optional[int
+00000720: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
+00000730: 2020 2020 2020 2073 6567 6d65 6e74 3a20         segment: 
+00000740: 4f70 7469 6f6e 616c 5b27 5365 676d 656e  Optional['Segmen
+00000750: 7427 5d20 3d20 4e6f 6e65 2c0d 0a20 2020  t'] = None,..   
+00000760: 2020 2020 2020 2020 2072 6f75 6e64 5f74           round_t
+00000770: 733a 2062 6f6f 6c20 3d20 5472 7565 2c0d  s: bool = True,.
+00000780: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
+00000790: 6f72 655f 756e 7573 6564 5f61 7267 733a  ore_unused_args:
+000007a0: 2062 6f6f 6c20 3d20 4661 6c73 650d 0a20   bool = False.. 
+000007b0: 2020 2029 3a0d 0a20 2020 2020 2020 2069     ):..        i
+000007c0: 6620 6e6f 7420 6967 6e6f 7265 5f75 6e75  f not ignore_unu
+000007d0: 7365 645f 6172 6773 2061 6e64 2073 6567  sed_args and seg
+000007e0: 6d65 6e74 5f69 6420 6973 206e 6f74 204e  ment_id is not N
+000007f0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00000800: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
+00000810: 2754 6865 2070 6172 616d 6574 6572 2060  'The parameter `
+00000820: 6073 6567 6d65 6e74 5f69 6460 6020 6973  `segment_id`` is
+00000830: 2069 676e 6f72 6564 2e20 270d 0a20 2020   ignored. '..   
+00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000850: 2020 2020 2020 2027 5370 6563 6966 7920         'Specify 
+00000860: 7468 6520 6375 7272 656e 7420 7365 676d  the current segm
+00000870: 656e 7420 696e 7374 616e 6365 2077 6974  ent instance wit
+00000880: 6820 6060 7365 676d 656e 7460 602e 272c  h ``segment``.',
+00000890: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000008a0: 2020 2020 2020 2020 2020 2020 7374 6163              stac
+000008b0: 6b6c 6576 656c 3d32 290d 0a20 2020 2020  klevel=2)..     
+000008c0: 2020 2073 656c 662e 726f 756e 645f 7473     self.round_ts
+000008d0: 203d 2072 6f75 6e64 5f74 730d 0a20 2020   = round_ts..   
+000008e0: 2020 2020 2073 656c 662e 776f 7264 203d       self.word =
+000008f0: 2077 6f72 640d 0a20 2020 2020 2020 2073   word..        s
+00000900: 656c 662e 5f73 7461 7274 203d 2073 656c  elf._start = sel
+00000910: 662e 726f 756e 6428 7374 6172 7429 0d0a  f.round(start)..
+00000920: 2020 2020 2020 2020 7365 6c66 2e5f 656e          self._en
+00000930: 6420 3d20 7365 6c66 2e72 6f75 6e64 2865  d = self.round(e
+00000940: 6e64 290d 0a20 2020 2020 2020 2073 656c  nd)..        sel
+00000950: 662e 7072 6f62 6162 696c 6974 7920 3d20  f.probability = 
+00000960: 7072 6f62 6162 696c 6974 790d 0a20 2020  probability..   
+00000970: 2020 2020 2073 656c 662e 746f 6b65 6e73       self.tokens
+00000980: 203d 2074 6f6b 656e 730d 0a20 2020 2020   = tokens..     
+00000990: 2020 2073 656c 662e 6c65 6674 5f6c 6f63     self.left_loc
+000009a0: 6b65 6420 3d20 6c65 6674 5f6c 6f63 6b65  ked = left_locke
+000009b0: 640d 0a20 2020 2020 2020 2073 656c 662e  d..        self.
+000009c0: 7269 6768 745f 6c6f 636b 6564 203d 2072  right_locked = r
+000009d0: 6967 6874 5f6c 6f63 6b65 640d 0a20 2020  ight_locked..   
+000009e0: 2020 2020 2073 656c 662e 7365 676d 656e       self.segmen
+000009f0: 7420 3d20 7365 676d 656e 740d 0a20 2020  t = segment..   
+00000a00: 2020 2020 2073 656c 662e 6964 203d 2069       self.id = i
+00000a10: 640d 0a0d 0a20 2020 2064 6566 205f 5f72  d....    def __r
+00000a20: 6570 725f 5f28 7365 6c66 293a 0d0a 2020  epr__(self):..  
+00000a30: 2020 2020 2020 7265 7475 726e 2066 2757        return f'W
+00000a40: 6f72 6454 696d 696e 6728 7374 6172 743d  ordTiming(start=
+00000a50: 7b73 656c 662e 7374 6172 747d 2c20 656e  {self.start}, en
+00000a60: 643d 7b73 656c 662e 656e 647d 2c20 776f  d={self.end}, wo
+00000a70: 7264 3d22 7b73 656c 662e 776f 7264 7d22  rd="{self.word}"
+00000a80: 2927 0d0a 0d0a 2020 2020 6465 6620 5f5f  )'....    def __
+00000a90: 6c65 6e5f 5f28 7365 6c66 293a 0d0a 2020  len__(self):..  
+00000aa0: 2020 2020 2020 7265 7475 726e 206c 656e        return len
+00000ab0: 2873 656c 662e 776f 7264 290d 0a0d 0a20  (self.word).... 
+00000ac0: 2020 2064 6566 205f 5f61 6464 5f5f 2873     def __add__(s
+00000ad0: 656c 662c 206f 7468 6572 3a20 2757 6f72  elf, other: 'Wor
+00000ae0: 6454 696d 696e 6727 293a 0d0a 2020 2020  dTiming'):..    
+00000af0: 2020 2020 7365 6c66 5f63 6f70 7920 3d20      self_copy = 
+00000b00: 576f 7264 5469 6d69 6e67 280d 0a20 2020  WordTiming(..   
+00000b10: 2020 2020 2020 2020 2077 6f72 643d 7365           word=se
+00000b20: 6c66 2e77 6f72 6420 2b20 6f74 6865 722e  lf.word + other.
+00000b30: 776f 7264 2c0d 0a20 2020 2020 2020 2020  word,..         
+00000b40: 2020 2073 7461 7274 3d6d 696e 2873 656c     start=min(sel
+00000b50: 662e 7374 6172 742c 206f 7468 6572 2e73  f.start, other.s
+00000b60: 7461 7274 292c 0d0a 2020 2020 2020 2020  tart),..        
+00000b70: 2020 2020 656e 643d 6d61 7828 7365 6c66      end=max(self
+00000b80: 2e65 6e64 2c20 6f74 6865 722e 656e 6429  .end, other.end)
+00000b90: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
+00000ba0: 726f 6261 6269 6c69 7479 3d73 656c 662e  robability=self.
+00000bb0: 7072 6f62 6162 696c 6974 792c 0d0a 2020  probability,..  
+00000bc0: 2020 2020 2020 2020 2020 746f 6b65 6e73            tokens
+00000bd0: 3d4e 6f6e 6520 6966 2073 656c 662e 746f  =None if self.to
+00000be0: 6b65 6e73 2069 7320 4e6f 6e65 2065 6c73  kens is None els
+00000bf0: 6520 7365 6c66 2e74 6f6b 656e 732e 636f  e self.tokens.co
+00000c00: 7079 2829 2c0d 0a20 2020 2020 2020 2020  py(),..         
+00000c10: 2020 206c 6566 745f 6c6f 636b 6564 3d73     left_locked=s
+00000c20: 656c 662e 6c65 6674 5f6c 6f63 6b65 6420  elf.left_locked 
+00000c30: 6f72 206f 7468 6572 2e6c 6566 745f 6c6f  or other.left_lo
+00000c40: 636b 6564 2c0d 0a20 2020 2020 2020 2020  cked,..         
+00000c50: 2020 2072 6967 6874 5f6c 6f63 6b65 643d     right_locked=
+00000c60: 7365 6c66 2e72 6967 6874 5f6c 6f63 6b65  self.right_locke
+00000c70: 6420 6f72 206f 7468 6572 2e72 6967 6874  d or other.right
+00000c80: 5f6c 6f63 6b65 642c 0d0a 2020 2020 2020  _locked,..      
+00000c90: 2020 2020 2020 6964 3d73 656c 662e 6964        id=self.id
+00000ca0: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+00000cb0: 6567 6d65 6e74 3d73 656c 662e 7365 676d  egment=self.segm
+00000cc0: 656e 740d 0a20 2020 2020 2020 2029 0d0a  ent..        )..
+00000cd0: 2020 2020 2020 2020 5f63 6f6d 6269 6e65          _combine
+00000ce0: 5f61 7474 7228 7365 6c66 5f63 6f70 792c  _attr(self_copy,
+00000cf0: 206f 7468 6572 2c20 2770 726f 6261 6269   other, 'probabi
+00000d00: 6c69 7479 2729 0d0a 2020 2020 2020 2020  lity')..        
+00000d10: 5f63 6f6d 6269 6e65 5f61 7474 7228 7365  _combine_attr(se
+00000d20: 6c66 5f63 6f70 792c 206f 7468 6572 2c20  lf_copy, other, 
+00000d30: 2774 6f6b 656e 7327 290d 0a0d 0a20 2020  'tokens')....   
+00000d40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00000d50: 5f63 6f70 790d 0a0d 0a20 2020 2064 6566  _copy....    def
+00000d60: 205f 5f64 6565 7063 6f70 795f 5f28 7365   __deepcopy__(se
+00000d70: 6c66 2c20 6d65 6d6f 3d4e 6f6e 6529 3a0d  lf, memo=None):.
+00000d80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000d90: 7365 6c66 2e63 6f70 7928 636f 7079 5f74  self.copy(copy_t
+00000da0: 6f6b 656e 733d 5472 7565 290d 0a0d 0a20  okens=True).... 
+00000db0: 2020 2064 6566 205f 5f63 6f70 795f 5f28     def __copy__(
+00000dc0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000dd0: 7265 7475 726e 2073 656c 662e 636f 7079  return self.copy
+00000de0: 2829 0d0a 0d0a 2020 2020 6465 6620 636f  ()....    def co
+00000df0: 7079 280d 0a20 2020 2020 2020 2020 2020  py(..           
+00000e00: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
+00000e10: 2020 2020 6b65 6570 5f73 6567 6d65 6e74      keep_segment
+00000e20: 3a20 626f 6f6c 203d 2046 616c 7365 2c0d  : bool = False,.
+00000e30: 0a20 2020 2020 2020 2020 2020 2063 6f70  .            cop
+00000e40: 795f 746f 6b65 6e73 3a20 626f 6f6c 203d  y_tokens: bool =
+00000e50: 2046 616c 7365 0d0a 2020 2020 293a 0d0a   False..    ):..
+00000e60: 2020 2020 2020 2020 7265 7475 726e 2057          return W
+00000e70: 6f72 6454 696d 696e 6728 0d0a 2020 2020  ordTiming(..    
+00000e80: 2020 2020 2020 2020 776f 7264 3d73 656c          word=sel
+00000e90: 662e 776f 7264 2c0d 0a20 2020 2020 2020  f.word,..       
+00000ea0: 2020 2020 2073 7461 7274 3d73 656c 662e       start=self.
+00000eb0: 7374 6172 742c 0d0a 2020 2020 2020 2020  start,..        
+00000ec0: 2020 2020 656e 643d 7365 6c66 2e65 6e64      end=self.end
+00000ed0: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
+00000ee0: 726f 6261 6269 6c69 7479 3d73 656c 662e  robability=self.
+00000ef0: 7072 6f62 6162 696c 6974 792c 0d0a 2020  probability,..  
+00000f00: 2020 2020 2020 2020 2020 746f 6b65 6e73            tokens
+00000f10: 3d4e 6f6e 6520 6966 2028 7365 6c66 2e74  =None if (self.t
+00000f20: 6f6b 656e 7320 6973 204e 6f6e 6529 2065  okens is None) e
+00000f30: 6c73 6520 2873 656c 662e 746f 6b65 6e73  lse (self.tokens
+00000f40: 2e63 6f70 7928 2920 6966 2063 6f70 795f  .copy() if copy_
+00000f50: 746f 6b65 6e73 2065 6c73 6520 7365 6c66  tokens else self
+00000f60: 2e74 6f6b 656e 7329 2c0d 0a20 2020 2020  .tokens),..     
+00000f70: 2020 2020 2020 206c 6566 745f 6c6f 636b         left_lock
+00000f80: 6564 3d73 656c 662e 6c65 6674 5f6c 6f63  ed=self.left_loc
+00000f90: 6b65 642c 0d0a 2020 2020 2020 2020 2020  ked,..          
+00000fa0: 2020 7269 6768 745f 6c6f 636b 6564 3d73    right_locked=s
+00000fb0: 656c 662e 7269 6768 745f 6c6f 636b 6564  elf.right_locked
+00000fc0: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
+00000fd0: 643d 7365 6c66 2e69 642c 0d0a 2020 2020  d=self.id,..    
+00000fe0: 2020 2020 2020 2020 7365 676d 656e 743d          segment=
+00000ff0: 7365 6c66 2e73 6567 6d65 6e74 2069 6620  self.segment if 
+00001000: 6b65 6570 5f73 6567 6d65 6e74 2065 6c73  keep_segment els
+00001010: 6520 4e6f 6e65 2c0d 0a20 2020 2020 2020  e None,..       
+00001020: 2020 2020 2072 6f75 6e64 5f74 733d 7365       round_ts=se
+00001030: 6c66 2e72 6f75 6e64 5f74 730d 0a20 2020  lf.round_ts..   
+00001040: 2020 2020 2029 0d0a 0d0a 2020 2020 6465       )....    de
+00001050: 6620 726f 756e 6428 7365 6c66 2c20 7469  f round(self, ti
+00001060: 6d65 7374 616d 703a 2066 6c6f 6174 2920  mestamp: float) 
+00001070: 2d3e 2066 6c6f 6174 3a0d 0a20 2020 2020  -> float:..     
+00001080: 2020 2069 6620 6e6f 7420 7365 6c66 2e72     if not self.r
+00001090: 6f75 6e64 5f74 733a 0d0a 2020 2020 2020  ound_ts:..      
+000010a0: 2020 2020 2020 7265 7475 726e 2074 696d        return tim
+000010b0: 6573 7461 6d70 0d0a 2020 2020 2020 2020  estamp..        
+000010c0: 7265 7475 726e 205f 726f 756e 645f 7469  return _round_ti
+000010d0: 6d65 7374 616d 7028 7469 6d65 7374 616d  mestamp(timestam
+000010e0: 7029 0d0a 0d0a 2020 2020 4070 726f 7065  p)....    @prope
+000010f0: 7274 790d 0a20 2020 2064 6566 2073 7461  rty..    def sta
+00001100: 7274 2873 656c 6629 3a0d 0a20 2020 2020  rt(self):..     
+00001110: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00001120: 7374 6172 740d 0a0d 0a20 2020 2040 7072  start....    @pr
+00001130: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
+00001140: 656e 6428 7365 6c66 293a 0d0a 2020 2020  end(self):..    
+00001150: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00001160: 5f65 6e64 0d0a 0d0a 2020 2020 4073 7461  _end....    @sta
+00001170: 7274 2e73 6574 7465 720d 0a20 2020 2064  rt.setter..    d
+00001180: 6566 2073 7461 7274 2873 656c 662c 2076  ef start(self, v
+00001190: 616c 293a 0d0a 2020 2020 2020 2020 7365  al):..        se
+000011a0: 6c66 2e5f 7374 6172 7420 3d20 7365 6c66  lf._start = self
+000011b0: 2e72 6f75 6e64 2876 616c 290d 0a0d 0a20  .round(val).... 
+000011c0: 2020 2040 656e 642e 7365 7474 6572 0d0a     @end.setter..
+000011d0: 2020 2020 6465 6620 656e 6428 7365 6c66      def end(self
+000011e0: 2c20 7661 6c29 3a0d 0a20 2020 2020 2020  , val):..       
+000011f0: 2073 656c 662e 5f65 6e64 203d 2073 656c   self._end = sel
+00001200: 662e 726f 756e 6428 7661 6c29 0d0a 0d0a  f.round(val)....
+00001210: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+00001220: 2020 2064 6566 2073 6567 6d65 6e74 5f69     def segment_i
+00001230: 6428 7365 6c66 293a 0d0a 2020 2020 2020  d(self):..      
+00001240: 2020 7265 7475 726e 204e 6f6e 6520 6966    return None if
+00001250: 2073 656c 662e 7365 676d 656e 7420 6973   self.segment is
+00001260: 204e 6f6e 6520 656c 7365 2073 656c 662e   None else self.
+00001270: 7365 676d 656e 742e 6964 0d0a 0d0a 2020  segment.id....  
+00001280: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00001290: 2064 6566 2064 7572 6174 696f 6e28 7365   def duration(se
+000012a0: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
+000012b0: 7475 726e 2073 656c 662e 726f 756e 6428  turn self.round(
+000012c0: 7365 6c66 2e65 6e64 202d 2073 656c 662e  self.end - self.
+000012d0: 7374 6172 7429 0d0a 0d0a 2020 2020 6465  start)....    de
+000012e0: 6620 726f 756e 645f 616c 6c5f 7469 6d65  f round_all_time
+000012f0: 7374 616d 7073 2873 656c 6629 3a0d 0a20  stamps(self):.. 
+00001300: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
+00001310: 7761 726e 2827 6060 2e72 6f75 6e64 5f61  warn('``.round_a
+00001320: 6c6c 5f74 696d 6573 7461 6d70 7328 2960  ll_timestamps()`
+00001330: 6020 6973 2064 6570 7265 6361 7465 6420  ` is deprecated 
+00001340: 616e 6420 7769 6c6c 2062 6520 7265 6d6f  and will be remo
+00001350: 7665 6420 696e 2066 7574 7572 6520 7665  ved in future ve
+00001360: 7273 696f 6e73 2e20 270d 0a20 2020 2020  rsions. '..     
+00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001380: 2027 5573 6520 6060 2e72 6f75 6e64 5f74   'Use ``.round_t
+00001390: 733d 5472 7565 6060 2074 6f20 726f 756e  s=True`` to roun
+000013a0: 6420 7469 6d65 7374 616d 7073 2062 7920  d timestamps by 
+000013b0: 6465 6661 756c 7420 696e 7374 6561 642e  default instead.
+000013c0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+000013d0: 2020 2020 2020 2020 2020 7374 6163 6b6c            stackl
+000013e0: 6576 656c 3d32 290d 0a20 2020 2020 2020  evel=2)..       
+000013f0: 2073 656c 662e 726f 756e 645f 7473 203d   self.round_ts =
+00001400: 2054 7275 650d 0a0d 0a20 2020 2064 6566   True....    def
+00001410: 206f 6666 7365 745f 7469 6d65 2873 656c   offset_time(sel
+00001420: 662c 206f 6666 7365 745f 7365 636f 6e64  f, offset_second
+00001430: 733a 2066 6c6f 6174 293a 0d0a 2020 2020  s: float):..    
+00001440: 2020 2020 7365 6c66 2e73 7461 7274 203d      self.start =
+00001450: 2073 656c 662e 7374 6172 7420 2b20 6f66   self.start + of
+00001460: 6673 6574 5f73 6563 6f6e 6473 0d0a 2020  fset_seconds..  
+00001470: 2020 2020 2020 7365 6c66 2e65 6e64 203d        self.end =
+00001480: 2073 656c 662e 656e 6420 2b20 6f66 6673   self.end + offs
+00001490: 6574 5f73 6563 6f6e 6473 0d0a 0d0a 2020  et_seconds....  
+000014a0: 2020 6465 6620 746f 5f64 6963 7428 7365    def to_dict(se
+000014b0: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
+000014c0: 7475 726e 2064 6963 7428 0d0a 2020 2020  turn dict(..    
+000014d0: 2020 2020 2020 2020 776f 7264 3d73 656c          word=sel
+000014e0: 662e 776f 7264 2c0d 0a20 2020 2020 2020  f.word,..       
+000014f0: 2020 2020 2073 7461 7274 3d73 656c 662e       start=self.
+00001500: 7374 6172 742c 0d0a 2020 2020 2020 2020  start,..        
+00001510: 2020 2020 656e 643d 7365 6c66 2e65 6e64      end=self.end
+00001520: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
+00001530: 726f 6261 6269 6c69 7479 3d73 656c 662e  robability=self.
+00001540: 7072 6f62 6162 696c 6974 792c 0d0a 2020  probability,..  
+00001550: 2020 2020 2020 2020 2020 746f 6b65 6e73            tokens
+00001560: 3d4e 6f6e 6520 6966 2073 656c 662e 746f  =None if self.to
+00001570: 6b65 6e73 2069 7320 4e6f 6e65 2065 6c73  kens is None els
+00001580: 6520 7365 6c66 2e74 6f6b 656e 732e 636f  e self.tokens.co
+00001590: 7079 2829 0d0a 2020 2020 2020 2020 290d  py()..        ).
+000015a0: 0a0d 0a20 2020 2064 6566 206c 6f63 6b5f  ...    def lock_
+000015b0: 6c65 6674 2873 656c 6629 3a0d 0a20 2020  left(self):..   
+000015c0: 2020 2020 2073 656c 662e 6c65 6674 5f6c       self.left_l
+000015d0: 6f63 6b65 6420 3d20 5472 7565 0d0a 0d0a  ocked = True....
+000015e0: 2020 2020 6465 6620 6c6f 636b 5f72 6967      def lock_rig
+000015f0: 6874 2873 656c 6629 3a0d 0a20 2020 2020  ht(self):..     
+00001600: 2020 2073 656c 662e 7269 6768 745f 6c6f     self.right_lo
+00001610: 636b 6564 203d 2054 7275 650d 0a0d 0a20  cked = True.... 
+00001620: 2020 2064 6566 206c 6f63 6b5f 626f 7468     def lock_both
+00001630: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00001640: 2073 656c 662e 6c6f 636b 5f6c 6566 7428   self.lock_left(
+00001650: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00001660: 6c6f 636b 5f72 6967 6874 2829 0d0a 0d0a  lock_right()....
+00001670: 2020 2020 6465 6620 756e 6c6f 636b 5f62      def unlock_b
+00001680: 6f74 6828 7365 6c66 293a 0d0a 2020 2020  oth(self):..    
+00001690: 2020 2020 7365 6c66 2e6c 6566 745f 6c6f      self.left_lo
+000016a0: 636b 6564 203d 2046 616c 7365 0d0a 2020  cked = False..  
+000016b0: 2020 2020 2020 7365 6c66 2e72 6967 6874        self.right
+000016c0: 5f6c 6f63 6b65 6420 3d20 4661 6c73 650d  _locked = False.
+000016d0: 0a0d 0a20 2020 2064 6566 2073 7570 7072  ...    def suppr
+000016e0: 6573 735f 7369 6c65 6e63 6528 7365 6c66  ess_silence(self
+000016f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001700: 2020 2020 2020 2020 2020 2020 7369 6c65              sile
+00001710: 6e74 5f73 7461 7274 733a 206e 702e 6e64  nt_starts: np.nd
+00001720: 6172 7261 792c 0d0a 2020 2020 2020 2020  array,..        
 00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 2020 206d 696e 5f77 6f72 645f 6475 723a     min_word_dur:
-00001750: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
-00001760: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001780: 2020 206e 6f6e 7370 6565 6368 5f65 7272     nonspeech_err
-00001790: 6f72 3a20 666c 6f61 7420 3d20 302e 332c  or: float = 0.3,
-000017a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000017b0: 2020 2020 2020 2020 2020 206b 6565 705f             keep_
-000017c0: 656e 643a 204f 7074 696f 6e61 6c5b 626f  end: Optional[bo
-000017d0: 6f6c 5d20 3d20 5472 7565 293a 0d0a 2020  ol] = True):..  
-000017e0: 2020 2020 2020 7375 7070 7265 7373 5f73        suppress_s
-000017f0: 696c 656e 6365 2873 656c 662c 2073 696c  ilence(self, sil
-00001800: 656e 745f 7374 6172 7473 2c20 7369 6c65  ent_starts, sile
-00001810: 6e74 5f65 6e64 732c 206d 696e 5f77 6f72  nt_ends, min_wor
-00001820: 645f 6475 722c 206e 6f6e 7370 6565 6368  d_dur, nonspeech
-00001830: 5f65 7272 6f72 2c20 6b65 6570 5f65 6e64  _error, keep_end
-00001840: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00001850: 6e20 7365 6c66 0d0a 0d0a 2020 2020 6465  n self....    de
-00001860: 6620 7265 7363 616c 655f 7469 6d65 2873  f rescale_time(s
-00001870: 656c 662c 2073 6361 6c65 5f66 6163 746f  elf, scale_facto
-00001880: 723a 2066 6c6f 6174 293a 0d0a 2020 2020  r: float):..    
-00001890: 2020 2020 7365 6c66 2e73 7461 7274 203d      self.start =
-000018a0: 2073 656c 662e 7374 6172 7420 2a20 7363   self.start * sc
-000018b0: 616c 655f 6661 6374 6f72 0d0a 2020 2020  ale_factor..    
-000018c0: 2020 2020 7365 6c66 2e65 6e64 203d 2073      self.end = s
-000018d0: 656c 662e 656e 6420 2a20 7363 616c 655f  elf.end * scale_
-000018e0: 6661 6374 6f72 0d0a 0d0a 2020 2020 6465  factor....    de
-000018f0: 6620 636c 616d 705f 6d61 7828 7365 6c66  f clamp_max(self
-00001900: 2c20 6d61 785f 6475 723a 2066 6c6f 6174  , max_dur: float
-00001910: 2c20 636c 6970 5f73 7461 7274 3a20 626f  , clip_start: bo
-00001920: 6f6c 203d 2046 616c 7365 2c20 7665 7262  ol = False, verb
-00001930: 6f73 653a 2062 6f6f 6c20 3d20 4661 6c73  ose: bool = Fals
-00001940: 6529 3a0d 0a20 2020 2020 2020 2069 6620  e):..        if 
-00001950: 7365 6c66 2e64 7572 6174 696f 6e20 3e20  self.duration > 
-00001960: 6d61 785f 6475 723a 0d0a 2020 2020 2020  max_dur:..      
-00001970: 2020 2020 2020 6966 2063 6c69 705f 7374        if clip_st
-00001980: 6172 743a 0d0a 2020 2020 2020 2020 2020  art:..          
-00001990: 2020 2020 2020 6e65 775f 7374 6172 7420        new_start 
-000019a0: 3d20 726f 756e 6428 7365 6c66 2e65 6e64  = round(self.end
-000019b0: 202d 206d 6178 5f64 7572 2c20 3329 0d0a   - max_dur, 3)..
-000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019d0: 6966 2076 6572 626f 7365 3a0d 0a20 2020  if verbose:..   
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019f0: 2070 7269 6e74 2866 2753 7461 7274 3a20   print(f'Start: 
-00001a00: 7b73 656c 662e 7374 6172 747d 202d 3e20  {self.start} -> 
-00001a10: 7b6e 6577 5f73 7461 7274 7d5c 6e45 6e64  {new_start}\nEnd
-00001a20: 3a20 7b73 656c 662e 656e 647d 5c6e 5465  : {self.end}\nTe
-00001a30: 7874 3a22 7b73 656c 662e 776f 7264 7d22  xt:"{self.word}"
-00001a40: 5c6e 2729 0d0a 2020 2020 2020 2020 2020  \n')..          
-00001a50: 2020 2020 2020 7365 6c66 2e73 7461 7274        self.start
-00001a60: 203d 206e 6577 5f73 7461 7274 0d0a 0d0a   = new_start....
-00001a70: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00001a80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001a90: 2020 206e 6577 5f65 6e64 203d 2072 6f75     new_end = rou
-00001aa0: 6e64 2873 656c 662e 7374 6172 7420 2b20  nd(self.start + 
-00001ab0: 6d61 785f 6475 722c 2033 290d 0a20 2020  max_dur, 3)..   
-00001ac0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00001ad0: 7665 7262 6f73 653a 0d0a 2020 2020 2020  verbose:..      
-00001ae0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00001af0: 696e 7428 6627 5374 6172 743a 207b 7365  int(f'Start: {se
-00001b00: 6c66 2e73 7461 7274 7d5c 6e45 6e64 3a20  lf.start}\nEnd: 
-00001b10: 7b73 656c 662e 656e 647d 202d 3e20 7b6e  {self.end} -> {n
-00001b20: 6577 5f65 6e64 7d5c 6e54 6578 743a 227b  ew_end}\nText:"{
-00001b30: 7365 6c66 2e77 6f72 647d 225c 6e27 290d  self.word}"\n').
-00001b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001b50: 2073 656c 662e 656e 6420 3d20 6e65 775f   self.end = new_
-00001b60: 656e 640d 0a0d 0a20 2020 2064 6566 2073  end....    def s
-00001b70: 6574 5f73 6567 6d65 6e74 2873 656c 662c  et_segment(self,
-00001b80: 2073 6567 6d65 6e74 3a20 2753 6567 6d65   segment: 'Segme
-00001b90: 6e74 2729 3a0d 0a20 2020 2020 2020 2077  nt'):..        w
-00001ba0: 6172 6e69 6e67 732e 7761 726e 2827 6060  arnings.warn('``
-00001bb0: 2e73 6574 5f73 6567 6d65 6e74 2863 7572  .set_segment(cur
-00001bc0: 7265 6e74 5f73 6567 6d65 6e74 5f69 6e73  rent_segment_ins
-00001bd0: 7461 6e63 6529 6060 2069 7320 6465 7072  tance)`` is depr
-00001be0: 6563 6174 6564 2061 6e64 2077 696c 6c20  ecated and will 
-00001bf0: 6265 2072 656d 6f76 6564 2069 6e20 6675  be removed in fu
-00001c00: 7475 7265 2076 6572 7369 6f6e 732e 270d  ture versions.'.
-00001c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001c20: 2020 2020 2020 2027 2055 7365 2060 602e         ' Use ``.
-00001c30: 7365 676d 656e 7420 3d20 6375 7272 656e  segment = curren
-00001c40: 745f 7365 676d 656e 7460 6020 696e 7374  t_segment`` inst
-00001c50: 6561 642e 272c 0d0a 2020 2020 2020 2020  ead.',..        
-00001c60: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00001c70: 6163 6b6c 6576 656c 3d32 290d 0a20 2020  acklevel=2)..   
-00001c80: 2020 2020 2073 656c 662e 7365 676d 656e       self.segmen
-00001c90: 7420 3d20 7365 676d 656e 740d 0a0d 0a20  t = segment.... 
-00001ca0: 2020 2064 6566 2067 6574 5f73 6567 6d65     def get_segme
-00001cb0: 6e74 2873 656c 6629 202d 3e20 556e 696f  nt(self) -> Unio
-00001cc0: 6e5b 2753 6567 6d65 6e74 272c 204e 6f6e  n['Segment', Non
-00001cd0: 655d 3a0d 0a20 2020 2020 2020 2022 2222  e]:..        """
-00001ce0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00001cf0: 2069 6e73 7461 6e63 6520 6f66 203a 636c   instance of :cl
-00001d00: 6173 733a 6073 7461 626c 655f 7768 6973  ass:`stable_whis
-00001d10: 7065 722e 7265 7375 6c74 2e53 6567 6d65  per.result.Segme
-00001d20: 6e74 6020 7468 6174 2074 6869 7320 696e  nt` that this in
-00001d30: 7374 616e 6365 2069 7320 6120 7061 7274  stance is a part
-00001d40: 206f 662e 0d0a 2020 2020 2020 2020 2222   of...        ""
-00001d50: 220d 0a20 2020 2020 2020 2077 6172 6e69  "..        warni
-00001d60: 6e67 732e 7761 726e 2827 6060 2e67 6574  ngs.warn('``.get
-00001d70: 5f73 6567 6d65 6e74 2829 6060 2077 696c  _segment()`` wil
-00001d80: 6c20 6265 2072 656d 6f76 6564 2069 6e20  l be removed in 
-00001d90: 6675 7475 7265 2076 6572 7369 6f6e 732e  future versions.
-00001da0: 2055 7365 2060 602e 7365 676d 656e 7460   Use ``.segment`
-00001db0: 6020 696e 7374 6561 642e 272c 0d0a 2020  ` instead.',..  
-00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dd0: 2020 2020 7374 6163 6b6c 6576 656c 3d32      stacklevel=2
-00001de0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00001df0: 6e20 7365 6c66 2e73 6567 6d65 6e74 0d0a  n self.segment..
-00001e00: 0d0a 0d0a 6465 6620 5f77 6f72 6473 5f62  ....def _words_b
-00001e10: 795f 6c6f 636b 2877 6f72 6473 3a20 4c69  y_lock(words: Li
-00001e20: 7374 5b57 6f72 6454 696d 696e 675d 2c20  st[WordTiming], 
-00001e30: 6f6e 6c79 5f74 6578 743a 2062 6f6f 6c20  only_text: bool 
-00001e40: 3d20 4661 6c73 652c 2069 6e63 6c75 6465  = False, include
-00001e50: 5f73 696e 676c 653a 2062 6f6f 6c20 3d20  _single: bool = 
-00001e60: 4661 6c73 6529 3a0d 0a20 2020 2022 2222  False):..    """
-00001e70: 0d0a 2020 2020 5265 7475 726e 2061 206e  ..    Return a n
-00001e80: 6573 7465 6420 6c69 7374 206f 6620 776f  ested list of wo
-00001e90: 7264 7320 7375 6368 2074 6861 7420 6561  rds such that ea
-00001ea0: 6368 2073 7562 6c69 7374 2063 6f6e 7461  ch sublist conta
-00001eb0: 696e 7320 776f 7264 7320 7468 6174 2061  ins words that a
-00001ec0: 7265 206c 6f63 6b65 6420 746f 6765 7468  re locked togeth
-00001ed0: 6572 2e0d 0a20 2020 2022 2222 0d0a 2020  er...    """..  
-00001ee0: 2020 616c 6c5f 776f 7264 7320 3d20 5b5d    all_words = []
-00001ef0: 0d0a 2020 2020 666f 7220 776f 7264 2069  ..    for word i
-00001f00: 6e20 776f 7264 733a 0d0a 2020 2020 2020  n words:..      
-00001f10: 2020 6966 206c 656e 2861 6c6c 5f77 6f72    if len(all_wor
-00001f20: 6473 2920 3d3d 2030 206f 7220 6e6f 7420  ds) == 0 or not 
-00001f30: 2861 6c6c 5f77 6f72 6473 5b2d 315d 5b2d  (all_words[-1][-
-00001f40: 315d 2e72 6967 6874 5f6c 6f63 6b65 6420  1].right_locked 
-00001f50: 6f72 2077 6f72 642e 6c65 6674 5f6c 6f63  or word.left_loc
-00001f60: 6b65 6429 3a0d 0a20 2020 2020 2020 2020  ked):..         
-00001f70: 2020 2061 6c6c 5f77 6f72 6473 2e61 7070     all_words.app
-00001f80: 656e 6428 5b77 6f72 645d 290d 0a20 2020  end([word])..   
-00001f90: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00001fa0: 2020 2020 2020 2020 616c 6c5f 776f 7264          all_word
-00001fb0: 735b 2d31 5d2e 6170 7065 6e64 2877 6f72  s[-1].append(wor
-00001fc0: 6429 0d0a 2020 2020 6966 206f 6e6c 795f  d)..    if only_
-00001fd0: 7465 7874 3a0d 0a20 2020 2020 2020 2061  text:..        a
-00001fe0: 6c6c 5f77 6f72 6473 203d 206c 6973 7428  ll_words = list(
-00001ff0: 6d61 7028 6c61 6d62 6461 2077 733a 206c  map(lambda ws: l
-00002000: 6973 7428 6d61 7028 6c61 6d62 6461 2077  ist(map(lambda w
-00002010: 3a20 772e 776f 7264 2c20 7773 2929 2c20  : w.word, ws)), 
-00002020: 616c 6c5f 776f 7264 7329 290d 0a20 2020  all_words))..   
-00002030: 2069 6620 6e6f 7420 696e 636c 7564 655f   if not include_
-00002040: 7369 6e67 6c65 3a0d 0a20 2020 2020 2020  single:..       
-00002050: 2061 6c6c 5f77 6f72 6473 203d 205b 7773   all_words = [ws
-00002060: 2066 6f72 2077 7320 696e 2061 6c6c 5f77   for ws in all_w
-00002070: 6f72 6473 2069 6620 6c65 6e28 7773 2920  ords if len(ws) 
-00002080: 3e20 315d 0d0a 2020 2020 7265 7475 726e  > 1]..    return
-00002090: 2061 6c6c 5f77 6f72 6473 0d0a 0d0a 0d0a   all_words......
-000020a0: 636c 6173 7320 5365 676d 656e 743a 0d0a  class Segment:..
-000020b0: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-000020c0: 5f5f 280d 0a20 2020 2020 2020 2020 2020  __(..           
-000020d0: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
-000020e0: 2020 2020 7374 6172 743a 204f 7074 696f      start: Optio
-000020f0: 6e61 6c5b 666c 6f61 745d 203d 204e 6f6e  nal[float] = Non
-00002100: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00002110: 656e 643a 204f 7074 696f 6e61 6c5b 666c  end: Optional[fl
-00002120: 6f61 745d 203d 204e 6f6e 652c 0d0a 2020  oat] = None,..  
-00002130: 2020 2020 2020 2020 2020 7465 7874 3a20            text: 
-00002140: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00002150: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
-00002160: 2020 2073 6565 6b3a 204f 7074 696f 6e61     seek: Optiona
-00002170: 6c5b 666c 6f61 745d 203d 204e 6f6e 652c  l[float] = None,
-00002180: 0d0a 2020 2020 2020 2020 2020 2020 746f  ..            to
-00002190: 6b65 6e73 3a20 4c69 7374 5b69 6e74 5d20  kens: List[int] 
-000021a0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-000021b0: 2020 2020 2074 656d 7065 7261 7475 7265       temperature
-000021c0: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-000021d0: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-000021e0: 2020 2020 2020 2061 7667 5f6c 6f67 7072         avg_logpr
-000021f0: 6f62 3a20 4f70 7469 6f6e 616c 5b66 6c6f  ob: Optional[flo
-00002200: 6174 5d20 3d20 4e6f 6e65 2c0d 0a20 2020  at] = None,..   
-00002210: 2020 2020 2020 2020 2063 6f6d 7072 6573           compres
-00002220: 7369 6f6e 5f72 6174 696f 3a20 4f70 7469  sion_ratio: Opti
-00002230: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
-00002240: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-00002250: 206e 6f5f 7370 6565 6368 5f70 726f 623a   no_speech_prob:
-00002260: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
-00002270: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00002280: 2020 2020 2020 776f 7264 733a 204f 7074        words: Opt
-00002290: 696f 6e61 6c5b 556e 696f 6e5b 4c69 7374  ional[Union[List
-000022a0: 5b57 6f72 6454 696d 696e 675d 2c20 4c69  [WordTiming], Li
-000022b0: 7374 5b64 6963 745d 5d5d 203d 204e 6f6e  st[dict]]] = Non
-000022c0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000022d0: 6964 3a20 4f70 7469 6f6e 616c 5b69 6e74  id: Optional[int
-000022e0: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-000022f0: 2020 2020 2020 2072 6573 756c 743a 204f         result: O
-00002300: 7074 696f 6e61 6c5b 2257 6869 7370 6572  ptional["Whisper
-00002310: 5265 7375 6c74 225d 203d 204e 6f6e 652c  Result"] = None,
-00002320: 0d0a 2020 2020 2020 2020 2020 2020 726f  ..            ro
-00002330: 756e 645f 7473 3a20 626f 6f6c 203d 2054  und_ts: bool = T
-00002340: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-00002350: 2020 6967 6e6f 7265 5f75 6e75 7365 645f    ignore_unused_
-00002360: 6172 6773 3a20 626f 6f6c 203d 2046 616c  args: bool = Fal
-00002370: 7365 0d0a 2020 2020 293a 0d0a 2020 2020  se..    ):..    
-00002380: 2020 2020 6966 2077 6f72 6473 3a0d 0a20      if words:.. 
-00002390: 2020 2020 2020 2020 2020 2069 6620 6967             if ig
-000023a0: 6e6f 7265 5f75 6e75 7365 645f 6172 6773  nore_unused_args
-000023b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000023c0: 2020 2073 7461 7274 203d 2065 6e64 203d     start = end =
-000023d0: 2074 6578 7420 3d20 746f 6b65 6e73 203d   text = tokens =
-000023e0: 204e 6f6e 650d 0a20 2020 2020 2020 2020   None..         
-000023f0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00002400: 2020 2020 2020 2020 2020 6966 2028 7374            if (st
-00002410: 6172 7420 6f72 2065 6e64 2920 6973 206e  art or end) is n
-00002420: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00002430: 2020 2020 2020 2020 2020 2020 2020 7761                wa
-00002440: 726e 696e 6773 2e77 6172 6e28 2741 7267  rnings.warn('Arg
-00002450: 756d 656e 7473 2066 6f72 2060 6073 7461  uments for ``sta
-00002460: 7274 6060 2061 6e64 2060 6065 6e64 6060  rt`` and ``end``
-00002470: 2077 696c 6c20 6265 2069 676e 6f72 6564   will be ignored
-00002480: 2027 0d0a 2020 2020 2020 2020 2020 2020   '..            
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 2020 2020 2020 2761 6e64 2074 6865 2060        'and the `
-000024b0: 6073 7461 7274 6060 2061 6e64 2060 6065  `start`` and ``e
-000024c0: 6e64 6060 2077 696c 6c20 7461 6b65 6e20  nd`` will taken 
-000024d0: 6672 6f6d 2074 6865 2066 6972 7374 2061  from the first a
-000024e0: 6e64 206c 6173 7420 6060 776f 7264 7360  nd last ``words`
-000024f0: 602e 272c 0d0a 2020 2020 2020 2020 2020  `.',..          
-00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002510: 2020 2020 2020 2020 7374 6163 6b6c 6576          stacklev
-00002520: 656c 3d32 290d 0a20 2020 2020 2020 2020  el=2)..         
-00002530: 2020 2020 2020 2069 6620 7465 7874 2069         if text i
-00002540: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002560: 2077 6172 6e69 6e67 732e 7761 726e 2827   warnings.warn('
-00002570: 5468 6520 6172 6775 6d65 6e74 2066 6f72  The argument for
-00002580: 2060 6074 6578 7460 6020 7769 6c6c 2062   ``text`` will b
-00002590: 6520 6967 6e6f 7265 6420 270d 0a20 2020  e ignored '..   
-000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025b0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000025c0: 616e 6420 6974 2077 696c 6c20 616c 7761  and it will alwa
-000025d0: 7973 2062 6520 7468 6520 636f 6e63 6174  ys be the concat
-000025e0: 656e 6174 696f 6e20 6f66 2074 6578 7420  enation of text 
-000025f0: 696e 2060 6077 6f72 6473 6060 272c 0d0a  in ``words``',..
-00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002620: 2020 7374 6163 6b6c 6576 656c 3d32 290d    stacklevel=2).
+00001740: 2073 696c 656e 745f 656e 6473 3a20 6e70   silent_ends: np
+00001750: 2e6e 6461 7272 6179 2c0d 0a20 2020 2020  .ndarray,..     
+00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001770: 2020 2020 6d69 6e5f 776f 7264 5f64 7572      min_word_dur
+00001780: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
+00001790: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
+000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017b0: 2020 2020 6e6f 6e73 7065 6563 685f 6572      nonspeech_er
+000017c0: 726f 723a 2066 6c6f 6174 203d 2030 2e33  ror: float = 0.3
+000017d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000017e0: 2020 2020 2020 2020 2020 2020 6b65 6570              keep
+000017f0: 5f65 6e64 3a20 4f70 7469 6f6e 616c 5b62  _end: Optional[b
+00001800: 6f6f 6c5d 203d 2054 7275 6529 3a0d 0a20  ool] = True):.. 
+00001810: 2020 2020 2020 2073 7570 7072 6573 735f         suppress_
+00001820: 7369 6c65 6e63 6528 7365 6c66 2c20 7369  silence(self, si
+00001830: 6c65 6e74 5f73 7461 7274 732c 2073 696c  lent_starts, sil
+00001840: 656e 745f 656e 6473 2c20 6d69 6e5f 776f  ent_ends, min_wo
+00001850: 7264 5f64 7572 2c20 6e6f 6e73 7065 6563  rd_dur, nonspeec
+00001860: 685f 6572 726f 722c 206b 6565 705f 656e  h_error, keep_en
+00001870: 6429 0d0a 2020 2020 2020 2020 7265 7475  d)..        retu
+00001880: 726e 2073 656c 660d 0a0d 0a20 2020 2064  rn self....    d
+00001890: 6566 2072 6573 6361 6c65 5f74 696d 6528  ef rescale_time(
+000018a0: 7365 6c66 2c20 7363 616c 655f 6661 6374  self, scale_fact
+000018b0: 6f72 3a20 666c 6f61 7429 3a0d 0a20 2020  or: float):..   
+000018c0: 2020 2020 2073 656c 662e 7374 6172 7420       self.start 
+000018d0: 3d20 7365 6c66 2e73 7461 7274 202a 2073  = self.start * s
+000018e0: 6361 6c65 5f66 6163 746f 720d 0a20 2020  cale_factor..   
+000018f0: 2020 2020 2073 656c 662e 656e 6420 3d20       self.end = 
+00001900: 7365 6c66 2e65 6e64 202a 2073 6361 6c65  self.end * scale
+00001910: 5f66 6163 746f 720d 0a0d 0a20 2020 2064  _factor....    d
+00001920: 6566 2063 6c61 6d70 5f6d 6178 2873 656c  ef clamp_max(sel
+00001930: 662c 206d 6178 5f64 7572 3a20 666c 6f61  f, max_dur: floa
+00001940: 742c 2063 6c69 705f 7374 6172 743a 2062  t, clip_start: b
+00001950: 6f6f 6c20 3d20 4661 6c73 652c 2076 6572  ool = False, ver
+00001960: 626f 7365 3a20 626f 6f6c 203d 2046 616c  bose: bool = Fal
+00001970: 7365 293a 0d0a 2020 2020 2020 2020 6966  se):..        if
+00001980: 2073 656c 662e 6475 7261 7469 6f6e 203e   self.duration >
+00001990: 206d 6178 5f64 7572 3a0d 0a20 2020 2020   max_dur:..     
+000019a0: 2020 2020 2020 2069 6620 636c 6970 5f73         if clip_s
+000019b0: 7461 7274 3a0d 0a20 2020 2020 2020 2020  tart:..         
+000019c0: 2020 2020 2020 206e 6577 5f73 7461 7274         new_start
+000019d0: 203d 2072 6f75 6e64 2873 656c 662e 656e   = round(self.en
+000019e0: 6420 2d20 6d61 785f 6475 722c 2033 290d  d - max_dur, 3).
+000019f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001a00: 2069 6620 7665 7262 6f73 653a 0d0a 2020   if verbose:..  
+00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a20: 2020 7072 696e 7428 6627 5374 6172 743a    print(f'Start:
+00001a30: 207b 7365 6c66 2e73 7461 7274 7d20 2d3e   {self.start} ->
+00001a40: 207b 6e65 775f 7374 6172 747d 5c6e 456e   {new_start}\nEn
+00001a50: 643a 207b 7365 6c66 2e65 6e64 7d5c 6e54  d: {self.end}\nT
+00001a60: 6578 743a 227b 7365 6c66 2e77 6f72 647d  ext:"{self.word}
+00001a70: 225c 6e27 290d 0a20 2020 2020 2020 2020  "\n')..         
+00001a80: 2020 2020 2020 2073 656c 662e 7374 6172         self.star
+00001a90: 7420 3d20 6e65 775f 7374 6172 740d 0a0d  t = new_start...
+00001aa0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00001ab0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001ac0: 2020 2020 6e65 775f 656e 6420 3d20 726f      new_end = ro
+00001ad0: 756e 6428 7365 6c66 2e73 7461 7274 202b  und(self.start +
+00001ae0: 206d 6178 5f64 7572 2c20 3329 0d0a 2020   max_dur, 3)..  
+00001af0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00001b00: 2076 6572 626f 7365 3a0d 0a20 2020 2020   verbose:..     
+00001b10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00001b20: 7269 6e74 2866 2753 7461 7274 3a20 7b73  rint(f'Start: {s
+00001b30: 656c 662e 7374 6172 747d 5c6e 456e 643a  elf.start}\nEnd:
+00001b40: 207b 7365 6c66 2e65 6e64 7d20 2d3e 207b   {self.end} -> {
+00001b50: 6e65 775f 656e 647d 5c6e 5465 7874 3a22  new_end}\nText:"
+00001b60: 7b73 656c 662e 776f 7264 7d22 5c6e 2729  {self.word}"\n')
+00001b70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001b80: 2020 7365 6c66 2e65 6e64 203d 206e 6577    self.end = new
+00001b90: 5f65 6e64 0d0a 0d0a 2020 2020 6465 6620  _end....    def 
+00001ba0: 7365 745f 7365 676d 656e 7428 7365 6c66  set_segment(self
+00001bb0: 2c20 7365 676d 656e 743a 2027 5365 676d  , segment: 'Segm
+00001bc0: 656e 7427 293a 0d0a 2020 2020 2020 2020  ent'):..        
+00001bd0: 7761 726e 696e 6773 2e77 6172 6e28 2760  warnings.warn('`
+00001be0: 602e 7365 745f 7365 676d 656e 7428 6375  `.set_segment(cu
+00001bf0: 7272 656e 745f 7365 676d 656e 745f 696e  rrent_segment_in
+00001c00: 7374 616e 6365 2960 6020 6973 2064 6570  stance)`` is dep
+00001c10: 7265 6361 7465 6420 616e 6420 7769 6c6c  recated and will
+00001c20: 2062 6520 7265 6d6f 7665 6420 696e 2066   be removed in f
+00001c30: 7574 7572 6520 7665 7273 696f 6e73 2e27  uture versions.'
+00001c40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001c50: 2020 2020 2020 2020 2720 5573 6520 6060          ' Use ``
+00001c60: 2e73 6567 6d65 6e74 203d 2063 7572 7265  .segment = curre
+00001c70: 6e74 5f73 6567 6d65 6e74 6060 2069 6e73  nt_segment`` ins
+00001c80: 7465 6164 2e27 2c0d 0a20 2020 2020 2020  tead.',..       
+00001c90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001ca0: 7461 636b 6c65 7665 6c3d 3229 0d0a 2020  tacklevel=2)..  
+00001cb0: 2020 2020 2020 7365 6c66 2e73 6567 6d65        self.segme
+00001cc0: 6e74 203d 2073 6567 6d65 6e74 0d0a 0d0a  nt = segment....
+00001cd0: 2020 2020 6465 6620 6765 745f 7365 676d      def get_segm
+00001ce0: 656e 7428 7365 6c66 2920 2d3e 2055 6e69  ent(self) -> Uni
+00001cf0: 6f6e 5b27 5365 676d 656e 7427 2c20 4e6f  on['Segment', No
+00001d00: 6e65 5d3a 0d0a 2020 2020 2020 2020 2222  ne]:..        ""
+00001d10: 220d 0a20 2020 2020 2020 2052 6574 7572  "..        Retur
+00001d20: 6e20 696e 7374 616e 6365 206f 6620 3a63  n instance of :c
+00001d30: 6c61 7373 3a60 7374 6162 6c65 5f77 6869  lass:`stable_whi
+00001d40: 7370 6572 2e72 6573 756c 742e 5365 676d  sper.result.Segm
+00001d50: 656e 7460 2074 6861 7420 7468 6973 2069  ent` that this i
+00001d60: 6e73 7461 6e63 6520 6973 2061 2070 6172  nstance is a par
+00001d70: 7420 6f66 2e0d 0a20 2020 2020 2020 2022  t of...        "
+00001d80: 2222 0d0a 2020 2020 2020 2020 7761 726e  ""..        warn
+00001d90: 696e 6773 2e77 6172 6e28 2760 602e 6765  ings.warn('``.ge
+00001da0: 745f 7365 676d 656e 7428 2960 6020 7769  t_segment()`` wi
+00001db0: 6c6c 2062 6520 7265 6d6f 7665 6420 696e  ll be removed in
+00001dc0: 2066 7574 7572 6520 7665 7273 696f 6e73   future versions
+00001dd0: 2e20 5573 6520 6060 2e73 6567 6d65 6e74  . Use ``.segment
+00001de0: 6060 2069 6e73 7465 6164 2e27 2c0d 0a20  `` instead.',.. 
+00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e00: 2020 2020 2073 7461 636b 6c65 7665 6c3d       stacklevel=
+00001e10: 3229 0d0a 2020 2020 2020 2020 7265 7475  2)..        retu
+00001e20: 726e 2073 656c 662e 7365 676d 656e 740d  rn self.segment.
+00001e30: 0a0d 0a0d 0a64 6566 205f 776f 7264 735f  .....def _words_
+00001e40: 6279 5f6c 6f63 6b28 776f 7264 733a 204c  by_lock(words: L
+00001e50: 6973 745b 576f 7264 5469 6d69 6e67 5d2c  ist[WordTiming],
+00001e60: 206f 6e6c 795f 7465 7874 3a20 626f 6f6c   only_text: bool
+00001e70: 203d 2046 616c 7365 2c20 696e 636c 7564   = False, includ
+00001e80: 655f 7369 6e67 6c65 3a20 626f 6f6c 203d  e_single: bool =
+00001e90: 2046 616c 7365 293a 0d0a 2020 2020 2222   False):..    ""
+00001ea0: 220d 0a20 2020 2052 6574 7572 6e20 6120  "..    Return a 
+00001eb0: 6e65 7374 6564 206c 6973 7420 6f66 2077  nested list of w
+00001ec0: 6f72 6473 2073 7563 6820 7468 6174 2065  ords such that e
+00001ed0: 6163 6820 7375 626c 6973 7420 636f 6e74  ach sublist cont
+00001ee0: 6169 6e73 2077 6f72 6473 2074 6861 7420  ains words that 
+00001ef0: 6172 6520 6c6f 636b 6564 2074 6f67 6574  are locked toget
+00001f00: 6865 722e 0d0a 2020 2020 2222 220d 0a20  her...    """.. 
+00001f10: 2020 2061 6c6c 5f77 6f72 6473 203d 205b     all_words = [
+00001f20: 5d0d 0a20 2020 2066 6f72 2077 6f72 6420  ]..    for word 
+00001f30: 696e 2077 6f72 6473 3a0d 0a20 2020 2020  in words:..     
+00001f40: 2020 2069 6620 6c65 6e28 616c 6c5f 776f     if len(all_wo
+00001f50: 7264 7329 203d 3d20 3020 6f72 206e 6f74  rds) == 0 or not
+00001f60: 2028 616c 6c5f 776f 7264 735b 2d31 5d5b   (all_words[-1][
+00001f70: 2d31 5d2e 7269 6768 745f 6c6f 636b 6564  -1].right_locked
+00001f80: 206f 7220 776f 7264 2e6c 6566 745f 6c6f   or word.left_lo
+00001f90: 636b 6564 293a 0d0a 2020 2020 2020 2020  cked):..        
+00001fa0: 2020 2020 616c 6c5f 776f 7264 732e 6170      all_words.ap
+00001fb0: 7065 6e64 285b 776f 7264 5d29 0d0a 2020  pend([word])..  
+00001fc0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00001fd0: 2020 2020 2020 2020 2061 6c6c 5f77 6f72           all_wor
+00001fe0: 6473 5b2d 315d 2e61 7070 656e 6428 776f  ds[-1].append(wo
+00001ff0: 7264 290d 0a20 2020 2069 6620 6f6e 6c79  rd)..    if only
+00002000: 5f74 6578 743a 0d0a 2020 2020 2020 2020  _text:..        
+00002010: 616c 6c5f 776f 7264 7320 3d20 6c69 7374  all_words = list
+00002020: 286d 6170 286c 616d 6264 6120 7773 3a20  (map(lambda ws: 
+00002030: 6c69 7374 286d 6170 286c 616d 6264 6120  list(map(lambda 
+00002040: 773a 2077 2e77 6f72 642c 2077 7329 292c  w: w.word, ws)),
+00002050: 2061 6c6c 5f77 6f72 6473 2929 0d0a 2020   all_words))..  
+00002060: 2020 6966 206e 6f74 2069 6e63 6c75 6465    if not include
+00002070: 5f73 696e 676c 653a 0d0a 2020 2020 2020  _single:..      
+00002080: 2020 616c 6c5f 776f 7264 7320 3d20 5b77    all_words = [w
+00002090: 7320 666f 7220 7773 2069 6e20 616c 6c5f  s for ws in all_
+000020a0: 776f 7264 7320 6966 206c 656e 2877 7329  words if len(ws)
+000020b0: 203e 2031 5d0d 0a20 2020 2072 6574 7572   > 1]..    retur
+000020c0: 6e20 616c 6c5f 776f 7264 730d 0a0d 0a0d  n all_words.....
+000020d0: 0a63 6c61 7373 2053 6567 6d65 6e74 3a0d  .class Segment:.
+000020e0: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
+000020f0: 745f 5f28 0d0a 2020 2020 2020 2020 2020  t__(..          
+00002100: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
+00002110: 2020 2020 2073 7461 7274 3a20 4f70 7469       start: Opti
+00002120: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
+00002130: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
+00002140: 2065 6e64 3a20 4f70 7469 6f6e 616c 5b66   end: Optional[f
+00002150: 6c6f 6174 5d20 3d20 4e6f 6e65 2c0d 0a20  loat] = None,.. 
+00002160: 2020 2020 2020 2020 2020 2074 6578 743a             text:
+00002170: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00002180: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+00002190: 2020 2020 7365 656b 3a20 4f70 7469 6f6e      seek: Option
+000021a0: 616c 5b66 6c6f 6174 5d20 3d20 4e6f 6e65  al[float] = None
+000021b0: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+000021c0: 6f6b 656e 733a 204c 6973 745b 696e 745d  okens: List[int]
+000021d0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+000021e0: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
+000021f0: 653a 204f 7074 696f 6e61 6c5b 666c 6f61  e: Optional[floa
+00002200: 745d 203d 204e 6f6e 652c 0d0a 2020 2020  t] = None,..    
+00002210: 2020 2020 2020 2020 6176 675f 6c6f 6770          avg_logp
+00002220: 726f 623a 204f 7074 696f 6e61 6c5b 666c  rob: Optional[fl
+00002230: 6f61 745d 203d 204e 6f6e 652c 0d0a 2020  oat] = None,..  
+00002240: 2020 2020 2020 2020 2020 636f 6d70 7265            compre
+00002250: 7373 696f 6e5f 7261 7469 6f3a 204f 7074  ssion_ratio: Opt
+00002260: 696f 6e61 6c5b 666c 6f61 745d 203d 204e  ional[float] = N
+00002270: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+00002280: 2020 6e6f 5f73 7065 6563 685f 7072 6f62    no_speech_prob
+00002290: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
+000022a0: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
+000022b0: 2020 2020 2020 2077 6f72 6473 3a20 4f70         words: Op
+000022c0: 7469 6f6e 616c 5b55 6e69 6f6e 5b4c 6973  tional[Union[Lis
+000022d0: 745b 576f 7264 5469 6d69 6e67 5d2c 204c  t[WordTiming], L
+000022e0: 6973 745b 6469 6374 5d5d 5d20 3d20 4e6f  ist[dict]]] = No
+000022f0: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
+00002300: 2069 643a 204f 7074 696f 6e61 6c5b 696e   id: Optional[in
+00002310: 745d 203d 204e 6f6e 652c 0d0a 2020 2020  t] = None,..    
+00002320: 2020 2020 2020 2020 7265 7375 6c74 3a20          result: 
+00002330: 4f70 7469 6f6e 616c 5b22 5768 6973 7065  Optional["Whispe
+00002340: 7252 6573 756c 7422 5d20 3d20 4e6f 6e65  rResult"] = None
+00002350: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00002360: 6f75 6e64 5f74 733a 2062 6f6f 6c20 3d20  ound_ts: bool = 
+00002370: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00002380: 2020 2069 676e 6f72 655f 756e 7573 6564     ignore_unused
+00002390: 5f61 7267 733a 2062 6f6f 6c20 3d20 4661  _args: bool = Fa
+000023a0: 6c73 650d 0a20 2020 2029 3a0d 0a20 2020  lse..    ):..   
+000023b0: 2020 2020 2069 6620 776f 7264 733a 0d0a       if words:..
+000023c0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+000023d0: 676e 6f72 655f 756e 7573 6564 5f61 7267  gnore_unused_arg
+000023e0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000023f0: 2020 2020 7374 6172 7420 3d20 656e 6420      start = end 
+00002400: 3d20 7465 7874 203d 2074 6f6b 656e 7320  = text = tokens 
+00002410: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
+00002420: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002430: 2020 2020 2020 2020 2020 2069 6620 2873             if (s
+00002440: 7461 7274 206f 7220 656e 6429 2069 7320  tart or end) is 
+00002450: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00002460: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00002470: 6172 6e69 6e67 732e 7761 726e 2827 4172  arnings.warn('Ar
+00002480: 6775 6d65 6e74 7320 666f 7220 6060 7374  guments for ``st
+00002490: 6172 7460 6020 616e 6420 6060 656e 6460  art`` and ``end`
+000024a0: 6020 7769 6c6c 2062 6520 6967 6e6f 7265  ` will be ignore
+000024b0: 6420 270d 0a20 2020 2020 2020 2020 2020  d '..           
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2020 2020 2020 2027 616e 6420 7468 6520         'and the 
+000024e0: 6060 7374 6172 7460 6020 616e 6420 6060  ``start`` and ``
+000024f0: 656e 6460 6020 7769 6c6c 2074 616b 656e  end`` will taken
+00002500: 2066 726f 6d20 7468 6520 6669 7273 7420   from the first 
+00002510: 616e 6420 6c61 7374 2060 6077 6f72 6473  and last ``words
+00002520: 6060 2e27 2c0d 0a20 2020 2020 2020 2020  ``.',..         
+00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002540: 2020 2020 2020 2020 2073 7461 636b 6c65           stackle
+00002550: 7665 6c3d 3229 0d0a 2020 2020 2020 2020  vel=2)..        
+00002560: 2020 2020 2020 2020 6966 2074 6578 7420          if text 
+00002570: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002590: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
+000025a0: 2754 6865 2061 7267 756d 656e 7420 666f  'The argument fo
+000025b0: 7220 6060 7465 7874 6060 2077 696c 6c20  r ``text`` will 
+000025c0: 6265 2069 676e 6f72 6564 2027 0d0a 2020  be ignored '..  
+000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025f0: 2761 6e64 2069 7420 7769 6c6c 2061 6c77  'and it will alw
+00002600: 6179 7320 6265 2074 6865 2063 6f6e 6361  ays be the conca
+00002610: 7465 6e61 7469 6f6e 206f 6620 7465 7874  tenation of text
+00002620: 2069 6e20 6060 776f 7264 7360 6027 2c0d   in ``words``',.
 00002630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002640: 2069 6620 746f 6b65 6e73 2069 7320 6e6f   if tokens is no
-00002650: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00002660: 2020 2020 2020 2020 2020 2020 2077 6172               war
-00002670: 6e69 6e67 732e 7761 726e 2827 5468 6520  nings.warn('The 
-00002680: 6172 6775 6d65 6e74 2066 6f72 2060 6074  argument for ``t
-00002690: 6f6b 656e 7360 6020 7769 6c6c 2062 6520  okens`` will be 
-000026a0: 6967 6e6f 7265 6420 270d 0a20 2020 2020  ignored '..     
-000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 2020 2020 2020 2020 2020 2020 2027 616e               'an
-000026d0: 6420 6974 2077 696c 6c20 616c 7761 7973  d it will always
-000026e0: 2062 6520 7468 6520 636f 6e63 6174 656e   be the concaten
-000026f0: 6174 696f 6e20 6f66 2074 6f6b 656e 7320  ation of tokens 
-00002700: 696e 2060 6077 6f72 6473 6060 272c 0d0a  in ``words``',..
-00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002730: 2020 7374 6163 6b6c 6576 656c 3d32 290d    stacklevel=2).
-00002740: 0a20 2020 2020 2020 2073 656c 662e 726f  .        self.ro
-00002750: 756e 645f 7473 203d 2072 6f75 6e64 5f74  und_ts = round_t
-00002760: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-00002770: 5f64 6566 6175 6c74 5f73 7461 7274 203d  _default_start =
-00002780: 2073 656c 662e 726f 756e 6428 7374 6172   self.round(star
-00002790: 7429 2069 6620 7374 6172 7420 656c 7365  t) if start else
-000027a0: 2030 2e30 0d0a 2020 2020 2020 2020 7365   0.0..        se
-000027b0: 6c66 2e5f 6465 6661 756c 745f 656e 6420  lf._default_end 
-000027c0: 3d20 7365 6c66 2e72 6f75 6e64 2865 6e64  = self.round(end
-000027d0: 2920 6966 2065 6e64 2065 6c73 6520 302e  ) if end else 0.
-000027e0: 300d 0a20 2020 2020 2020 2073 656c 662e  0..        self.
-000027f0: 5f64 6566 6175 6c74 5f74 6578 7420 3d20  _default_text = 
-00002800: 7465 7874 206f 7220 2727 0d0a 2020 2020  text or ''..    
-00002810: 2020 2020 7365 6c66 2e5f 6465 6661 756c      self._defaul
-00002820: 745f 746f 6b65 6e73 203d 2074 6f6b 656e  t_tokens = token
-00002830: 7320 6f72 205b 5d0d 0a20 2020 2020 2020  s or []..       
-00002840: 2073 656c 662e 7365 656b 203d 2073 6565   self.seek = see
-00002850: 6b0d 0a20 2020 2020 2020 2073 656c 662e  k..        self.
-00002860: 7465 6d70 6572 6174 7572 6520 3d20 7465  temperature = te
-00002870: 6d70 6572 6174 7572 650d 0a20 2020 2020  mperature..     
-00002880: 2020 2073 656c 662e 6176 675f 6c6f 6770     self.avg_logp
-00002890: 726f 6220 3d20 6176 675f 6c6f 6770 726f  rob = avg_logpro
-000028a0: 620d 0a20 2020 2020 2020 2073 656c 662e  b..        self.
-000028b0: 636f 6d70 7265 7373 696f 6e5f 7261 7469  compression_rati
-000028c0: 6f20 3d20 636f 6d70 7265 7373 696f 6e5f  o = compression_
-000028d0: 7261 7469 6f0d 0a20 2020 2020 2020 2073  ratio..        s
-000028e0: 656c 662e 6e6f 5f73 7065 6563 685f 7072  elf.no_speech_pr
-000028f0: 6f62 203d 206e 6f5f 7370 6565 6368 5f70  ob = no_speech_p
-00002900: 726f 620d 0a20 2020 2020 2020 2073 656c  rob..        sel
-00002910: 662e 776f 7264 7320 3d20 776f 7264 730d  f.words = words.
-00002920: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00002930: 2e77 6f72 6473 2061 6e64 2069 7369 6e73  .words and isins
-00002940: 7461 6e63 6528 776f 7264 735b 305d 2c20  tance(words[0], 
-00002950: 6469 6374 293a 0d0a 2020 2020 2020 2020  dict):..        
-00002960: 2020 2020 7365 6c66 2e77 6f72 6473 203d      self.words =
-00002970: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-00002980: 2020 2020 576f 7264 5469 6d69 6e67 280d      WordTiming(.
-00002990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000029a0: 2020 2020 202a 2a77 6f72 642c 0d0a 2020       **word,..  
-000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029c0: 2020 7365 676d 656e 743d 7365 6c66 2c0d    segment=self,.
-000029d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000029e0: 2020 2020 2072 6f75 6e64 5f74 733d 7365       round_ts=se
-000029f0: 6c66 2e72 6f75 6e64 5f74 732c 0d0a 2020  lf.round_ts,..  
-00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a10: 2020 6967 6e6f 7265 5f75 6e75 7365 645f    ignore_unused_
-00002a20: 6172 6773 3d54 7275 650d 0a20 2020 2020  args=True..     
-00002a30: 2020 2020 2020 2020 2020 2029 2066 6f72             ) for
-00002a40: 2077 6f72 6420 696e 2073 656c 662e 776f   word in self.wo
-00002a50: 7264 730d 0a20 2020 2020 2020 2020 2020  rds..           
-00002a60: 205d 0d0a 2020 2020 2020 2020 7365 6c66   ]..        self
-00002a70: 2e69 6420 3d20 6964 0d0a 2020 2020 2020  .id = id..      
-00002a80: 2020 7365 6c66 2e5f 7265 7665 7273 6564    self._reversed
-00002a90: 5f74 6578 7420 3d20 4661 6c73 650d 0a20  _text = False.. 
-00002aa0: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
-00002ab0: 6c74 203d 2072 6573 756c 740d 0a0d 0a20  lt = result.... 
-00002ac0: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
-00002ad0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00002ae0: 7265 7475 726e 2066 2753 6567 6d65 6e74  return f'Segment
-00002af0: 2873 7461 7274 3d7b 7365 6c66 2e73 7461  (start={self.sta
-00002b00: 7274 7d2c 2065 6e64 3d7b 7365 6c66 2e65  rt}, end={self.e
-00002b10: 6e64 7d2c 2074 6578 743d 227b 7365 6c66  nd}, text="{self
-00002b20: 2e74 6578 747d 2229 270d 0a0d 0a20 2020  .text}")'....   
-00002b30: 2064 6566 205f 5f67 6574 6974 656d 5f5f   def __getitem__
-00002b40: 2873 656c 662c 2069 6e64 6578 3a20 696e  (self, index: in
-00002b50: 7429 202d 3e20 576f 7264 5469 6d69 6e67  t) -> WordTiming
-00002b60: 3a0d 0a20 2020 2020 2020 2069 6620 7365  :..        if se
-00002b70: 6c66 2e77 6f72 6473 2069 7320 4e6f 6e65  lf.words is None
-00002b80: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00002b90: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00002ba0: 2773 6567 6d65 6e74 2063 6f6e 7461 696e  'segment contain
-00002bb0: 7320 6e6f 2077 6f72 6473 2729 0d0a 2020  s no words')..  
-00002bc0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00002bd0: 662e 776f 7264 735b 696e 6465 785d 0d0a  f.words[index]..
-00002be0: 0d0a 2020 2020 6465 6620 5f5f 6465 6c69  ..    def __deli
-00002bf0: 7465 6d5f 5f28 7365 6c66 2c20 696e 6465  tem__(self, inde
-00002c00: 783a 2069 6e74 293a 0d0a 2020 2020 2020  x: int):..      
-00002c10: 2020 6966 2073 656c 662e 776f 7264 7320    if self.words 
-00002c20: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00002c30: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00002c40: 6545 7272 6f72 2827 7365 676d 656e 7420  eError('segment 
-00002c50: 636f 6e74 6169 6e73 206e 6f20 776f 7264  contains no word
-00002c60: 7327 290d 0a20 2020 2020 2020 2064 656c  s')..        del
-00002c70: 2073 656c 662e 776f 7264 735b 696e 6465   self.words[inde
-00002c80: 785d 0d0a 2020 2020 2020 2020 7365 6c66  x]..        self
-00002c90: 2e72 6561 7373 6967 6e5f 6964 7328 696e  .reassign_ids(in
-00002ca0: 6465 7829 0d0a 0d0a 2020 2020 6465 6620  dex)....    def 
-00002cb0: 5f5f 6465 6570 636f 7079 5f5f 2873 656c  __deepcopy__(sel
-00002cc0: 662c 206d 656d 6f3d 4e6f 6e65 293a 0d0a  f, memo=None):..
-00002cd0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002ce0: 656c 662e 636f 7079 2863 6f70 795f 776f  elf.copy(copy_wo
-00002cf0: 7264 733d 5472 7565 2c20 636f 7079 5f74  rds=True, copy_t
-00002d00: 6f6b 656e 733d 5472 7565 290d 0a0d 0a20  okens=True).... 
-00002d10: 2020 2064 6566 205f 5f63 6f70 795f 5f28     def __copy__(
-00002d20: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00002d30: 7265 7475 726e 2073 656c 662e 636f 7079  return self.copy
-00002d40: 2829 0d0a 0d0a 2020 2020 6465 6620 636f  ()....    def co
-00002d50: 7079 280d 0a20 2020 2020 2020 2020 2020  py(..           
-00002d60: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
-00002d70: 2020 2020 6e65 775f 776f 7264 733a 204f      new_words: O
-00002d80: 7074 696f 6e61 6c5b 4c69 7374 5b57 6f72  ptional[List[Wor
-00002d90: 6454 696d 696e 675d 5d20 3d20 4e6f 6e65  dTiming]] = None
-00002da0: 2c0d 0a20 2020 2020 2020 2020 2020 206b  ,..            k
-00002db0: 6565 705f 7265 7375 6c74 3a20 626f 6f6c  eep_result: bool
-00002dc0: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
-00002dd0: 2020 2020 2020 2063 6f70 795f 776f 7264         copy_word
-00002de0: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
-00002df0: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00002e00: 7079 5f74 6f6b 656e 733a 2062 6f6f 6c20  py_tokens: bool 
-00002e10: 3d20 4661 6c73 650d 0a20 2020 2029 3a0d  = False..    ):.
-00002e20: 0a20 2020 2020 2020 2069 6620 6e65 775f  .        if new_
-00002e30: 776f 7264 7320 6973 204e 6f6e 653a 0d0a  words is None:..
-00002e40: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00002e50: 656c 662e 6861 735f 776f 7264 733a 0d0a  elf.has_words:..
-00002e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e70: 776f 7264 7320 3d20 5b77 2e63 6f70 7928  words = [w.copy(
-00002e80: 636f 7079 5f74 6f6b 656e 733d 636f 7079  copy_tokens=copy
-00002e90: 5f74 6f6b 656e 7329 2066 6f72 2077 2069  _tokens) for w i
-00002ea0: 6e20 7365 6c66 2e77 6f72 6473 5d20 6966  n self.words] if
-00002eb0: 2063 6f70 795f 776f 7264 7320 656c 7365   copy_words else
-00002ec0: 2073 656c 662e 776f 7264 730d 0a20 2020   self.words..   
-00002ed0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00002ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ef0: 776f 7264 7320 3d20 4e6f 6e65 0d0a 2020  words = None..  
-00002f00: 2020 2020 2020 2020 2020 6465 665f 7374            def_st
-00002f10: 6172 7420 3d20 7365 6c66 2e5f 6465 6661  art = self._defa
-00002f20: 756c 745f 7374 6172 740d 0a20 2020 2020  ult_start..     
-00002f30: 2020 2020 2020 2064 6566 5f65 6e64 203d         def_end =
-00002f40: 2073 656c 662e 5f64 6566 6175 6c74 5f65   self._default_e
-00002f50: 6e64 0d0a 2020 2020 2020 2020 2020 2020  nd..            
-00002f60: 6465 665f 7465 7874 203d 2073 656c 662e  def_text = self.
-00002f70: 5f64 6566 6175 6c74 5f74 6578 740d 0a20  _default_text.. 
-00002f80: 2020 2020 2020 2020 2020 2064 6566 5f74             def_t
-00002f90: 6f6b 656e 7320 3d20 7365 6c66 2e5f 6465  okens = self._de
-00002fa0: 6661 756c 745f 746f 6b65 6e73 0d0a 2020  fault_tokens..  
-00002fb0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00002fc0: 2020 2020 2020 2020 2077 6f72 6473 203d           words =
-00002fd0: 205b 772e 636f 7079 2863 6f70 795f 746f   [w.copy(copy_to
-00002fe0: 6b65 6e73 3d63 6f70 795f 746f 6b65 6e73  kens=copy_tokens
-00002ff0: 2920 666f 7220 7720 696e 206e 6577 5f77  ) for w in new_w
-00003000: 6f72 6473 5d20 6966 2063 6f70 795f 776f  ords] if copy_wo
-00003010: 7264 7320 656c 7365 206e 6577 5f77 6f72  rds else new_wor
-00003020: 6473 0d0a 2020 2020 2020 2020 2020 2020  ds..            
-00003030: 6465 665f 7374 6172 7420 3d20 6465 665f  def_start = def_
-00003040: 656e 6420 3d20 6465 665f 7465 7874 203d  end = def_text =
-00003050: 2064 6566 5f74 6f6b 656e 7320 3d20 4e6f   def_tokens = No
-00003060: 6e65 0d0a 2020 2020 2020 2020 6e65 775f  ne..        new_
-00003070: 7365 6720 3d20 5365 676d 656e 7428 0d0a  seg = Segment(..
-00003080: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00003090: 743d 6465 665f 7374 6172 742c 0d0a 2020  t=def_start,..  
-000030a0: 2020 2020 2020 2020 2020 656e 643d 6465            end=de
-000030b0: 665f 656e 642c 0d0a 2020 2020 2020 2020  f_end,..        
-000030c0: 2020 2020 7465 7874 3d64 6566 5f74 6578      text=def_tex
-000030d0: 742c 0d0a 2020 2020 2020 2020 2020 2020  t,..            
-000030e0: 7365 656b 3d73 656c 662e 7365 656b 2c0d  seek=self.seek,.
-000030f0: 0a20 2020 2020 2020 2020 2020 2074 6f6b  .            tok
-00003100: 656e 733d 6465 665f 746f 6b65 6e73 2c0d  ens=def_tokens,.
-00003110: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-00003120: 7065 7261 7475 7265 3d73 656c 662e 7465  perature=self.te
-00003130: 6d70 6572 6174 7572 652c 0d0a 2020 2020  mperature,..    
-00003140: 2020 2020 2020 2020 6176 675f 6c6f 6770          avg_logp
-00003150: 726f 623d 7365 6c66 2e61 7667 5f6c 6f67  rob=self.avg_log
-00003160: 7072 6f62 2c0d 0a20 2020 2020 2020 2020  prob,..         
-00003170: 2020 2063 6f6d 7072 6573 7369 6f6e 5f72     compression_r
-00003180: 6174 696f 3d73 656c 662e 636f 6d70 7265  atio=self.compre
-00003190: 7373 696f 6e5f 7261 7469 6f2c 0d0a 2020  ssion_ratio,..  
-000031a0: 2020 2020 2020 2020 2020 6e6f 5f73 7065            no_spe
-000031b0: 6563 685f 7072 6f62 3d73 656c 662e 6e6f  ech_prob=self.no
-000031c0: 5f73 7065 6563 685f 7072 6f62 2c0d 0a20  _speech_prob,.. 
-000031d0: 2020 2020 2020 2020 2020 2077 6f72 6473             words
-000031e0: 3d77 6f72 6473 2c0d 0a20 2020 2020 2020  =words,..       
-000031f0: 2020 2020 2069 643d 7365 6c66 2e69 642c       id=self.id,
-00003200: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00003210: 7375 6c74 3d73 656c 662e 7265 7375 6c74  sult=self.result
-00003220: 2069 6620 6b65 6570 5f72 6573 756c 7420   if keep_result 
-00003230: 656c 7365 204e 6f6e 652c 0d0a 2020 2020  else None,..    
-00003240: 2020 2020 2020 2020 726f 756e 645f 7473          round_ts
-00003250: 3d73 656c 662e 726f 756e 645f 7473 2c0d  =self.round_ts,.
-00003260: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
-00003270: 6f72 655f 756e 7573 6564 5f61 7267 733d  ore_unused_args=
-00003280: 5472 7565 0d0a 2020 2020 2020 2020 290d  True..        ).
-00003290: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000032a0: 6e65 775f 7365 670d 0a0d 0a20 2020 2064  new_seg....    d
-000032b0: 6566 2072 6f75 6e64 2873 656c 662c 2074  ef round(self, t
-000032c0: 696d 6573 7461 6d70 3a20 666c 6f61 7429  imestamp: float)
-000032d0: 202d 3e20 666c 6f61 743a 0d0a 2020 2020   -> float:..    
-000032e0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-000032f0: 726f 756e 645f 7473 3a0d 0a20 2020 2020  round_ts:..     
-00003300: 2020 2020 2020 2072 6574 7572 6e20 7469         return ti
-00003310: 6d65 7374 616d 700d 0a20 2020 2020 2020  mestamp..       
-00003320: 2072 6574 7572 6e20 5f72 6f75 6e64 5f74   return _round_t
-00003330: 696d 6573 7461 6d70 2874 696d 6573 7461  imestamp(timesta
-00003340: 6d70 290d 0a0d 0a20 2020 2064 6566 2074  mp)....    def t
-00003350: 6f5f 6469 7370 6c61 795f 7374 7228 7365  o_display_str(se
-00003360: 6c66 2c20 6f6e 6c79 5f73 6567 6d65 6e74  lf, only_segment
-00003370: 3a20 626f 6f6c 203d 2046 616c 7365 293a  : bool = False):
-00003380: 0d0a 2020 2020 2020 2020 6c69 6e65 203d  ..        line =
-00003390: 2066 275b 7b66 6f72 6d61 745f 7469 6d65   f'[{format_time
-000033a0: 7374 616d 7028 7365 6c66 2e73 7461 7274  stamp(self.start
-000033b0: 297d 202d 2d3e 207b 666f 726d 6174 5f74  )} --> {format_t
-000033c0: 696d 6573 7461 6d70 2873 656c 662e 656e  imestamp(self.en
-000033d0: 6429 7d5d 2022 7b73 656c 662e 7465 7874  d)}] "{self.text
-000033e0: 7d22 270d 0a20 2020 2020 2020 2069 6620  }"'..        if 
-000033f0: 7365 6c66 2e68 6173 5f77 6f72 6473 2061  self.has_words a
-00003400: 6e64 206e 6f74 206f 6e6c 795f 7365 676d  nd not only_segm
-00003410: 656e 743a 0d0a 2020 2020 2020 2020 2020  ent:..          
-00003420: 2020 6c69 6e65 202b 3d20 275c 6e27 202b    line += '\n' +
-00003430: 2027 5c6e 272e 6a6f 696e 280d 0a20 2020   '\n'.join(..   
-00003440: 2020 2020 2020 2020 2020 2020 2066 222d               f"-
-00003450: 5b7b 666f 726d 6174 5f74 696d 6573 7461  [{format_timesta
-00003460: 6d70 2877 2e73 7461 7274 297d 5d20 2d3e  mp(w.start)}] ->
-00003470: 205b 7b66 6f72 6d61 745f 7469 6d65 7374   [{format_timest
-00003480: 616d 7028 772e 656e 6429 7d5d 205c 227b  amp(w.end)}] \"{
-00003490: 772e 776f 7264 7d5c 2222 2066 6f72 2077  w.word}\"" for w
-000034a0: 2069 6e20 7365 6c66 2e77 6f72 6473 0d0a   in self.words..
-000034b0: 2020 2020 2020 2020 2020 2020 2920 2b20              ) + 
-000034c0: 275c 6e27 0d0a 2020 2020 2020 2020 7265  '\n'..        re
-000034d0: 7475 726e 206c 696e 650d 0a0d 0a20 2020  turn line....   
-000034e0: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-000034f0: 6465 6620 6861 735f 776f 7264 7328 7365  def has_words(se
-00003500: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-00003510: 7475 726e 2062 6f6f 6c28 7365 6c66 2e77  turn bool(self.w
-00003520: 6f72 6473 290d 0a0d 0a20 2020 2040 7072  ords)....    @pr
-00003530: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
-00003540: 6f72 695f 6861 735f 776f 7264 7328 7365  ori_has_words(se
-00003550: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-00003560: 7475 726e 2073 656c 662e 776f 7264 7320  turn self.words 
-00003570: 6973 206e 6f74 204e 6f6e 650d 0a0d 0a20  is not None.... 
-00003580: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
-00003590: 2020 6465 6620 7374 6172 7428 7365 6c66    def start(self
-000035a0: 293a 0d0a 2020 2020 2020 2020 6966 2073  ):..        if s
-000035b0: 656c 662e 6861 735f 776f 7264 733a 0d0a  elf.has_words:..
-000035c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000035d0: 726e 2073 656c 662e 776f 7264 735b 305d  rn self.words[0]
-000035e0: 2e73 7461 7274 0d0a 2020 2020 2020 2020  .start..        
-000035f0: 7265 7475 726e 2073 656c 662e 5f64 6566  return self._def
-00003600: 6175 6c74 5f73 7461 7274 0d0a 0d0a 2020  ault_start....  
-00003610: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
-00003620: 2064 6566 2065 6e64 2873 656c 6629 3a0d   def end(self):.
-00003630: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00003640: 2e68 6173 5f77 6f72 6473 3a0d 0a20 2020  .has_words:..   
-00003650: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00003660: 7365 6c66 2e77 6f72 6473 5b2d 315d 2e65  self.words[-1].e
-00003670: 6e64 0d0a 2020 2020 2020 2020 7265 7475  nd..        retu
-00003680: 726e 2073 656c 662e 5f64 6566 6175 6c74  rn self._default
-00003690: 5f65 6e64 0d0a 0d0a 2020 2020 4073 7461  _end....    @sta
-000036a0: 7274 2e73 6574 7465 720d 0a20 2020 2064  rt.setter..    d
-000036b0: 6566 2073 7461 7274 2873 656c 662c 2076  ef start(self, v
-000036c0: 616c 293a 0d0a 2020 2020 2020 2020 6966  al):..        if
-000036d0: 2073 656c 662e 6861 735f 776f 7264 733a   self.has_words:
-000036e0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000036f0: 6c66 2e77 6f72 6473 5b30 5d2e 7374 6172  lf.words[0].star
-00003700: 7420 3d20 7661 6c0d 0a20 2020 2020 2020  t = val..       
-00003710: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-00003720: 2020 2020 2073 656c 662e 5f64 6566 6175       self._defau
-00003730: 6c74 5f73 7461 7274 203d 2073 656c 662e  lt_start = self.
-00003740: 726f 756e 6428 7661 6c29 0d0a 0d0a 2020  round(val)....  
-00003750: 2020 4065 6e64 2e73 6574 7465 720d 0a20    @end.setter.. 
-00003760: 2020 2064 6566 2065 6e64 2873 656c 662c     def end(self,
-00003770: 2076 616c 293a 0d0a 2020 2020 2020 2020   val):..        
-00003780: 6966 2073 656c 662e 6861 735f 776f 7264  if self.has_word
-00003790: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000037a0: 7365 6c66 2e77 6f72 6473 5b2d 315d 2e65  self.words[-1].e
-000037b0: 6e64 203d 2076 616c 0d0a 2020 2020 2020  nd = val..      
-000037c0: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
-000037d0: 2020 2020 2020 7365 6c66 2e5f 6465 6661        self._defa
-000037e0: 756c 745f 656e 6420 3d20 7365 6c66 2e72  ult_end = self.r
-000037f0: 6f75 6e64 2876 616c 290d 0a0d 0a20 2020  ound(val)....   
-00003800: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-00003810: 6465 6620 7465 7874 2873 656c 6629 202d  def text(self) -
-00003820: 3e20 7374 723a 0d0a 2020 2020 2020 2020  > str:..        
-00003830: 6966 2073 656c 662e 6861 735f 776f 7264  if self.has_word
-00003840: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00003850: 7265 7475 726e 2027 272e 6a6f 696e 2877  return ''.join(w
-00003860: 6f72 642e 776f 7264 2066 6f72 2077 6f72  ord.word for wor
-00003870: 6420 696e 2073 656c 662e 776f 7264 7329  d in self.words)
-00003880: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00003890: 2073 656c 662e 5f64 6566 6175 6c74 5f74   self._default_t
-000038a0: 6578 740d 0a0d 0a20 2020 2040 7072 6f70  ext....    @prop
-000038b0: 6572 7479 0d0a 2020 2020 6465 6620 746f  erty..    def to
-000038c0: 6b65 6e73 2873 656c 6629 202d 3e20 4c69  kens(self) -> Li
-000038d0: 7374 5b69 6e74 5d3a 0d0a 2020 2020 2020  st[int]:..      
-000038e0: 2020 6966 2073 656c 662e 6861 735f 776f    if self.has_wo
-000038f0: 7264 7320 616e 6420 7365 6c66 2e77 6f72  rds and self.wor
-00003900: 6473 5b30 5d2e 746f 6b65 6e73 3a0d 0a20  ds[0].tokens:.. 
-00003910: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003920: 6e20 6c69 7374 2863 6861 696e 2e66 726f  n list(chain.fro
-00003930: 6d5f 6974 6572 6162 6c65 2877 6f72 642e  m_iterable(word.
-00003940: 746f 6b65 6e73 2066 6f72 2077 6f72 6420  tokens for word 
-00003950: 696e 2073 656c 662e 776f 7264 7329 290d  in self.words)).
-00003960: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003970: 7365 6c66 2e5f 6465 6661 756c 745f 746f  self._default_to
-00003980: 6b65 6e73 0d0a 0d0a 2020 2020 4070 726f  kens....    @pro
-00003990: 7065 7274 790d 0a20 2020 2064 6566 2064  perty..    def d
-000039a0: 7572 6174 696f 6e28 7365 6c66 293a 0d0a  uration(self):..
-000039b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000039c0: 656c 662e 656e 6420 2d20 7365 6c66 2e73  elf.end - self.s
-000039d0: 7461 7274 0d0a 0d0a 2020 2020 6465 6620  tart....    def 
-000039e0: 776f 7264 5f63 6f75 6e74 2873 656c 6629  word_count(self)
-000039f0: 3a0d 0a20 2020 2020 2020 2069 6620 7365  :..        if se
-00003a00: 6c66 2e68 6173 5f77 6f72 6473 3a0d 0a20  lf.has_words:.. 
-00003a10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003a20: 6e20 6c65 6e28 7365 6c66 2e77 6f72 6473  n len(self.words
-00003a30: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00003a40: 6e20 2d31 0d0a 0d0a 2020 2020 6465 6620  n -1....    def 
-00003a50: 6368 6172 5f63 6f75 6e74 2873 656c 6629  char_count(self)
-00003a60: 3a0d 0a20 2020 2020 2020 2069 6620 7365  :..        if se
-00003a70: 6c66 2e68 6173 5f77 6f72 6473 3a0d 0a20  lf.has_words:.. 
-00003a80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003a90: 6e20 7375 6d28 6c65 6e28 7729 2066 6f72  n sum(len(w) for
-00003aa0: 2077 2069 6e20 7365 6c66 2e77 6f72 6473   w in self.words
-00003ab0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00003ac0: 6e20 6c65 6e28 7365 6c66 2e74 6578 7429  n len(self.text)
-00003ad0: 0d0a 0d0a 2020 2020 6465 6620 6164 6428  ....    def add(
-00003ae0: 7365 6c66 2c20 6f74 6865 723a 2027 5365  self, other: 'Se
-00003af0: 676d 656e 7427 2c20 636f 7079 5f77 6f72  gment', copy_wor
-00003b00: 6473 3a20 626f 6f6c 203d 2046 616c 7365  ds: bool = False
-00003b10: 293a 0d0a 2020 2020 2020 2020 6966 2073  ):..        if s
-00003b20: 656c 662e 6f72 695f 6861 735f 776f 7264  elf.ori_has_word
-00003b30: 7320 3d3d 206f 7468 6572 2e6f 7269 5f68  s == other.ori_h
-00003b40: 6173 5f77 6f72 6473 3a0d 0a20 2020 2020  as_words:..     
-00003b50: 2020 2020 2020 2077 6f72 6473 203d 2028         words = (
-00003b60: 7365 6c66 2e77 6f72 6473 202b 206f 7468  self.words + oth
-00003b70: 6572 2e77 6f72 6473 2920 6966 2073 656c  er.words) if sel
-00003b80: 662e 6f72 695f 6861 735f 776f 7264 7320  f.ori_has_words 
-00003b90: 656c 7365 204e 6f6e 650d 0a20 2020 2020  else None..     
-00003ba0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00003bb0: 2020 2020 2020 7365 6c66 5f73 7461 7465        self_state
-00003bc0: 203d 2027 7769 7468 2720 6966 2073 656c   = 'with' if sel
-00003bd0: 662e 6f72 695f 6861 735f 776f 7264 7320  f.ori_has_words 
-00003be0: 656c 7365 2027 7769 7468 6f75 7427 0d0a  else 'without'..
-00003bf0: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-00003c00: 725f 7374 6174 6520 3d20 2777 6974 6827  r_state = 'with'
-00003c10: 2069 6620 6f74 6865 722e 6f72 695f 6861   if other.ori_ha
-00003c20: 735f 776f 7264 7320 656c 7365 2027 7769  s_words else 'wi
-00003c30: 7468 6f75 7427 0d0a 2020 2020 2020 2020  thout'..        
-00003c40: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00003c50: 7272 6f72 2866 2243 616e 2774 206d 6572  rror(f"Can't mer
-00003c60: 6765 2073 6567 6d65 6e74 207b 7365 6c66  ge segment {self
-00003c70: 5f73 7461 7465 7d20 776f 7264 7320 616e  _state} words an
-00003c80: 6420 6120 7365 676d 656e 7420 7b6f 7468  d a segment {oth
-00003c90: 6572 5f73 7461 7465 7d20 776f 7264 732e  er_state} words.
-00003ca0: 2229 0d0a 0d0a 2020 2020 2020 2020 7365  ")....        se
-00003cb0: 6c66 5f63 6f70 7920 3d20 7365 6c66 2e63  lf_copy = self.c
-00003cc0: 6f70 7928 776f 7264 732c 2063 6f70 795f  opy(words, copy_
-00003cd0: 776f 7264 733d 636f 7079 5f77 6f72 6473  words=copy_words
-00003ce0: 290d 0a20 2020 2020 2020 205f 636f 6d62  )..        _comb
-00003cf0: 696e 655f 6174 7472 2873 656c 665f 636f  ine_attr(self_co
-00003d00: 7079 2c20 6f74 6865 722c 2027 7465 6d70  py, other, 'temp
-00003d10: 6572 6174 7572 6527 290d 0a20 2020 2020  erature')..     
-00003d20: 2020 205f 636f 6d62 696e 655f 6174 7472     _combine_attr
-00003d30: 2873 656c 665f 636f 7079 2c20 6f74 6865  (self_copy, othe
-00003d40: 722c 2027 6176 675f 6c6f 6770 726f 6227  r, 'avg_logprob'
-00003d50: 290d 0a20 2020 2020 2020 205f 636f 6d62  )..        _comb
-00003d60: 696e 655f 6174 7472 2873 656c 665f 636f  ine_attr(self_co
-00003d70: 7079 2c20 6f74 6865 722c 2027 636f 6d70  py, other, 'comp
-00003d80: 7265 7373 696f 6e5f 7261 7469 6f27 290d  ression_ratio').
-00003d90: 0a20 2020 2020 2020 205f 636f 6d62 696e  .        _combin
-00003da0: 655f 6174 7472 2873 656c 665f 636f 7079  e_attr(self_copy
-00003db0: 2c20 6f74 6865 722c 2027 6e6f 5f73 7065  , other, 'no_spe
-00003dc0: 6563 685f 7072 6f62 2729 0d0a 0d0a 2020  ech_prob')....  
-00003dd0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00003de0: 665f 636f 7079 0d0a 0d0a 2020 2020 6465  f_copy....    de
-00003df0: 6620 5f5f 6164 645f 5f28 7365 6c66 2c20  f __add__(self, 
-00003e00: 6f74 6865 723a 2027 5365 676d 656e 7427  other: 'Segment'
-00003e10: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-00003e20: 726e 2073 656c 662e 6164 6428 6f74 6865  rn self.add(othe
-00003e30: 722c 2063 6f70 795f 776f 7264 733d 5472  r, copy_words=Tr
-00003e40: 7565 290d 0a0d 0a20 2020 2064 6566 205f  ue)....    def _
-00003e50: 776f 7264 5f6f 7065 7261 7469 6f6e 7328  word_operations(
-00003e60: 7365 6c66 2c20 6f70 6572 6174 696f 6e3a  self, operation:
-00003e70: 2073 7472 2c20 2a61 7267 732c 202a 2a6b   str, *args, **k
-00003e80: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-00003e90: 2069 6620 7365 6c66 2e68 6173 5f77 6f72   if self.has_wor
-00003ea0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-00003eb0: 2066 6f72 2077 2069 6e20 7365 6c66 2e77   for w in self.w
-00003ec0: 6f72 6473 3a0d 0a20 2020 2020 2020 2020  ords:..         
-00003ed0: 2020 2020 2020 2067 6574 6174 7472 2877         getattr(w
-00003ee0: 2c20 6f70 6572 6174 696f 6e29 282a 6172  , operation)(*ar
-00003ef0: 6773 2c20 2a2a 6b77 6172 6773 290d 0a0d  gs, **kwargs)...
-00003f00: 0a20 2020 2064 6566 2072 6f75 6e64 5f61  .    def round_a
-00003f10: 6c6c 5f74 696d 6573 7461 6d70 7328 7365  ll_timestamps(se
-00003f20: 6c66 293a 0d0a 2020 2020 2020 2020 7761  lf):..        wa
-00003f30: 726e 696e 6773 2e77 6172 6e28 2760 602e  rnings.warn('``.
-00003f40: 726f 756e 645f 616c 6c5f 7469 6d65 7374  round_all_timest
-00003f50: 616d 7073 2829 6060 2069 7320 6465 7072  amps()`` is depr
-00003f60: 6563 6174 6564 2061 6e64 2077 696c 6c20  ecated and will 
-00003f70: 6265 2072 656d 6f76 6564 2069 6e20 6675  be removed in fu
-00003f80: 7475 7265 2076 6572 7369 6f6e 732e 2027  ture versions. '
-00003f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003fa0: 2020 2020 2020 2020 2755 7365 2060 602e          'Use ``.
-00003fb0: 726f 756e 645f 7473 3d54 7275 6560 6020  round_ts=True`` 
-00003fc0: 746f 2072 6f75 6e64 2074 696d 6573 7461  to round timesta
-00003fd0: 6d70 7320 6279 2064 6566 6175 6c74 2069  mps by default i
-00003fe0: 6e73 7465 6164 2e27 2c0d 0a20 2020 2020  nstead.',..     
-00003ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004000: 2073 7461 636b 6c65 7665 6c3d 3229 0d0a   stacklevel=2)..
-00004010: 2020 2020 2020 2020 7365 6c66 2e72 6f75          self.rou
-00004020: 6e64 5f74 7320 3d20 5472 7565 0d0a 0d0a  nd_ts = True....
-00004030: 2020 2020 6465 6620 6f66 6673 6574 5f74      def offset_t
-00004040: 696d 6528 7365 6c66 2c20 6f66 6673 6574  ime(self, offset
-00004050: 5f73 6563 6f6e 6473 3a20 666c 6f61 7429  _seconds: float)
-00004060: 3a0d 0a20 2020 2020 2020 2069 6620 7365  :..        if se
-00004070: 6c66 2e73 6565 6b20 6973 206e 6f74 204e  lf.seek is not N
-00004080: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00004090: 2020 7365 6c66 2e73 6565 6b20 2b3d 206f    self.seek += o
-000040a0: 6666 7365 745f 7365 636f 6e64 730d 0a20  ffset_seconds.. 
-000040b0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-000040c0: 6173 5f77 6f72 6473 3a0d 0a20 2020 2020  as_words:..     
-000040d0: 2020 2020 2020 2073 656c 662e 5f77 6f72         self._wor
-000040e0: 645f 6f70 6572 6174 696f 6e73 2827 6f66  d_operations('of
-000040f0: 6673 6574 5f74 696d 6527 2c20 6f66 6673  fset_time', offs
-00004100: 6574 5f73 6563 6f6e 6473 290d 0a20 2020  et_seconds)..   
-00004110: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00004120: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00004130: 7274 203d 2073 656c 662e 7374 6172 7420  rt = self.start 
-00004140: 2b20 6f66 6673 6574 5f73 6563 6f6e 6473  + offset_seconds
-00004150: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00004160: 6c66 2e65 6e64 203d 2073 656c 662e 656e  lf.end = self.en
-00004170: 6420 2b20 6f66 6673 6574 5f73 6563 6f6e  d + offset_secon
-00004180: 6473 0d0a 0d0a 2020 2020 6465 6620 6164  ds....    def ad
-00004190: 645f 776f 7264 7328 7365 6c66 2c20 696e  d_words(self, in
-000041a0: 6465 7830 3a20 696e 742c 2069 6e64 6578  dex0: int, index
-000041b0: 313a 2069 6e74 2c20 696e 706c 6163 653a  1: int, inplace:
-000041c0: 2062 6f6f 6c20 3d20 4661 6c73 6529 3a0d   bool = False):.
-000041d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000041e0: 2e68 6173 5f77 6f72 6473 3a0d 0a20 2020  .has_words:..   
-000041f0: 2020 2020 2020 2020 206e 6577 5f77 6f72           new_wor
-00004200: 6420 3d20 7365 6c66 2e77 6f72 6473 5b69  d = self.words[i
-00004210: 6e64 6578 305d 202b 2073 656c 662e 776f  ndex0] + self.wo
-00004220: 7264 735b 696e 6465 7831 5d0d 0a20 2020  rds[index1]..   
-00004230: 2020 2020 2020 2020 2069 6620 696e 706c           if inpl
-00004240: 6163 653a 0d0a 2020 2020 2020 2020 2020  ace:..          
-00004250: 2020 2020 2020 6930 2c20 6931 203d 2073        i0, i1 = s
-00004260: 6f72 7465 6428 5b69 6e64 6578 302c 2069  orted([index0, i
-00004270: 6e64 6578 315d 290d 0a20 2020 2020 2020  ndex1])..       
-00004280: 2020 2020 2020 2020 2073 656c 662e 776f           self.wo
-00004290: 7264 735b 6930 5d20 3d20 6e65 775f 776f  rds[i0] = new_wo
-000042a0: 7264 0d0a 2020 2020 2020 2020 2020 2020  rd..            
-000042b0: 2020 2020 6465 6c20 7365 6c66 2e77 6f72      del self.wor
-000042c0: 6473 5b69 315d 0d0a 2020 2020 2020 2020  ds[i1]..        
-000042d0: 2020 2020 7265 7475 726e 206e 6577 5f77      return new_w
-000042e0: 6f72 640d 0a0d 0a20 2020 2064 6566 2072  ord....    def r
-000042f0: 6573 6361 6c65 5f74 696d 6528 7365 6c66  escale_time(self
-00004300: 2c20 7363 616c 655f 6661 6374 6f72 3a20  , scale_factor: 
-00004310: 666c 6f61 7429 3a0d 0a20 2020 2020 2020  float):..       
-00004320: 2069 6620 7365 6c66 2e73 6565 6b20 6973   if self.seek is
-00004330: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00004340: 2020 2020 2020 2020 7365 6c66 2e73 6565          self.see
-00004350: 6b20 2a3d 2073 6361 6c65 5f66 6163 746f  k *= scale_facto
-00004360: 720d 0a20 2020 2020 2020 2069 6620 7365  r..        if se
-00004370: 6c66 2e68 6173 5f77 6f72 6473 3a0d 0a20  lf.has_words:.. 
-00004380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004390: 5f77 6f72 645f 6f70 6572 6174 696f 6e73  _word_operations
-000043a0: 2827 7265 7363 616c 655f 7469 6d65 272c  ('rescale_time',
-000043b0: 2073 6361 6c65 5f66 6163 746f 7229 0d0a   scale_factor)..
-000043c0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000043d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000043e0: 7374 6172 7420 3d20 7365 6c66 2e73 7461  start = self.sta
-000043f0: 7274 202a 2073 6361 6c65 5f66 6163 746f  rt * scale_facto
-00004400: 720d 0a20 2020 2020 2020 2020 2020 2073  r..            s
-00004410: 656c 662e 656e 6420 3d20 7365 6c66 2e65  elf.end = self.e
-00004420: 6e64 202a 2073 6361 6c65 5f66 6163 746f  nd * scale_facto
-00004430: 720d 0a0d 0a20 2020 2064 6566 2061 7070  r....    def app
-00004440: 6c79 5f6d 696e 5f64 7572 2873 656c 662c  ly_min_dur(self,
-00004450: 206d 696e 5f64 7572 3a20 666c 6f61 742c   min_dur: float,
-00004460: 2069 6e70 6c61 6365 3a20 626f 6f6c 203d   inplace: bool =
-00004470: 2046 616c 7365 293a 0d0a 2020 2020 2020   False):..      
-00004480: 2020 2222 220d 0a20 2020 2020 2020 204d    """..        M
-00004490: 6572 6765 2061 6e79 2077 6f72 6420 7769  erge any word wi
-000044a0: 7468 2061 646a 6163 656e 7420 776f 7264  th adjacent word
-000044b0: 2069 6620 6974 7320 6475 7261 7469 6f6e   if its duration
-000044c0: 2069 7320 6c65 7373 2074 6861 6e20 6060   is less than ``
-000044d0: 6d69 6e5f 6475 7260 602e 0d0a 2020 2020  min_dur``...    
-000044e0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000044f0: 2073 6567 6d65 6e74 203d 2073 656c 6620   segment = self 
-00004500: 6966 2069 6e70 6c61 6365 2065 6c73 6520  if inplace else 
-00004510: 6465 6570 636f 7079 2873 656c 6629 0d0a  deepcopy(self)..
-00004520: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00004530: 656c 662e 6861 735f 776f 7264 733a 0d0a  elf.has_words:..
-00004540: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00004550: 726e 2073 6567 6d65 6e74 0d0a 2020 2020  rn segment..    
-00004560: 2020 2020 6d61 785f 6920 3d20 6c65 6e28      max_i = len(
-00004570: 7365 676d 656e 742e 776f 7264 7329 202d  segment.words) -
-00004580: 2031 0d0a 2020 2020 2020 2020 6966 206d   1..        if m
-00004590: 6178 5f69 203d 3d20 303a 0d0a 2020 2020  ax_i == 0:..    
-000045a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000045b0: 6567 6d65 6e74 0d0a 2020 2020 2020 2020  egment..        
-000045c0: 666f 7220 6920 696e 2072 6576 6572 7365  for i in reverse
-000045d0: 6428 7261 6e67 6528 6c65 6e28 7365 676d  d(range(len(segm
-000045e0: 656e 742e 776f 7264 7329 2929 3a0d 0a20  ent.words))):.. 
-000045f0: 2020 2020 2020 2020 2020 2069 6620 6d61             if ma
-00004600: 785f 6920 3d3d 2030 3a0d 0a20 2020 2020  x_i == 0:..     
-00004610: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00004620: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00004630: 2073 6567 6d65 6e74 2e77 6f72 6473 5b69   segment.words[i
-00004640: 5d2e 6475 7261 7469 6f6e 203c 206d 696e  ].duration < min
-00004650: 5f64 7572 3a0d 0a20 2020 2020 2020 2020  _dur:..         
-00004660: 2020 2020 2020 2069 6620 6920 3d3d 206d         if i == m
-00004670: 6178 5f69 3a0d 0a20 2020 2020 2020 2020  ax_i:..         
-00004680: 2020 2020 2020 2020 2020 2073 6567 6d65             segme
-00004690: 6e74 2e61 6464 5f77 6f72 6473 2869 2d31  nt.add_words(i-1
-000046a0: 2c20 692c 2069 6e70 6c61 6365 3d54 7275  , i, inplace=Tru
-000046b0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-000046c0: 2020 2020 656c 6966 2069 203d 3d20 303a      elif i == 0:
-000046d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000046e0: 2020 2020 2020 7365 676d 656e 742e 6164        segment.ad
-000046f0: 645f 776f 7264 7328 692c 2069 2b31 2c20  d_words(i, i+1, 
-00004700: 696e 706c 6163 653d 5472 7565 290d 0a20  inplace=True).. 
-00004710: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00004720: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00004730: 2020 2020 2020 2020 2020 6966 2073 6567            if seg
-00004740: 6d65 6e74 2e77 6f72 6473 5b69 2b31 5d2e  ment.words[i+1].
-00004750: 6475 7261 7469 6f6e 203c 2073 6567 6d65  duration < segme
-00004760: 6e74 2e77 6f72 6473 5b69 2d31 5d2e 6475  nt.words[i-1].du
-00004770: 7261 7469 6f6e 3a0d 0a20 2020 2020 2020  ration:..       
-00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004790: 2073 6567 6d65 6e74 2e61 6464 5f77 6f72   segment.add_wor
-000047a0: 6473 2869 2d31 2c20 692c 2069 6e70 6c61  ds(i-1, i, inpla
-000047b0: 6365 3d54 7275 6529 0d0a 2020 2020 2020  ce=True)..      
-000047c0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000047d0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000047e0: 2020 2020 2020 2020 2020 2020 2073 6567               seg
-000047f0: 6d65 6e74 2e61 6464 5f77 6f72 6473 2869  ment.add_words(i
-00004800: 2c20 692b 312c 2069 6e70 6c61 6365 3d54  , i+1, inplace=T
-00004810: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
-00004820: 2020 2020 2020 6d61 785f 6920 2d3d 2031        max_i -= 1
-00004830: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00004840: 2073 6567 6d65 6e74 0d0a 0d0a 2020 2020   segment....    
-00004850: 6465 6620 5f74 6f5f 7265 7665 7273 655f  def _to_reverse_
-00004860: 7465 7874 280d 0a20 2020 2020 2020 2020  text(..         
-00004870: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
-00004880: 2020 2020 2020 7072 6570 656e 645f 7075        prepend_pu
-00004890: 6e63 7475 6174 696f 6e73 3a20 4f70 7469  nctuations: Opti
-000048a0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-000048b0: 2c0d 0a20 2020 2020 2020 2020 2020 2061  ,..            a
-000048c0: 7070 656e 645f 7075 6e63 7475 6174 696f  ppend_punctuatio
-000048d0: 6e73 3a20 4f70 7469 6f6e 616c 5b73 7472  ns: Optional[str
-000048e0: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2029  ] = None,..    )
-000048f0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00004900: 2020 2020 2020 2020 5265 7475 726e 2061          Return a
-00004910: 2063 6f70 7920 7769 7468 2077 6f72 6473   copy with words
-00004920: 2072 6576 6572 7365 6420 6f72 6465 7220   reversed order 
-00004930: 7065 7220 7365 676d 656e 742e 0d0a 2020  per segment...  
-00004940: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00004950: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
-00004960: 2827 6060 5f74 6f5f 7265 7665 7273 655f  ('``_to_reverse_
-00004970: 7465 7874 2829 6060 2069 7320 6465 7072  text()`` is depr
-00004980: 6563 6174 6564 2061 6e64 2077 696c 6c20  ecated and will 
-00004990: 6265 2072 656d 6f76 6564 2069 6e20 6675  be removed in fu
-000049a0: 7475 7265 2076 6572 7369 6f6e 732e 272c  ture versions.',
-000049b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000049c0: 2020 2020 2020 2020 6361 7465 676f 7279          category
-000049d0: 3d44 6570 7265 6361 7469 6f6e 5761 726e  =DeprecationWarn
-000049e0: 696e 672c 2073 7461 636b 6c65 7665 6c3d  ing, stacklevel=
-000049f0: 3229 0d0a 2020 2020 2020 2020 7072 6570  2)..        prep
-00004a00: 656e 645f 7075 6e63 7475 6174 696f 6e73  end_punctuations
-00004a10: 203d 2067 6574 5f70 7265 7065 6e64 5f70   = get_prepend_p
-00004a20: 756e 6374 7561 7469 6f6e 7328 7072 6570  unctuations(prep
-00004a30: 656e 645f 7075 6e63 7475 6174 696f 6e73  end_punctuations
-00004a40: 290d 0a20 2020 2020 2020 2069 6620 7072  )..        if pr
-00004a50: 6570 656e 645f 7075 6e63 7475 6174 696f  epend_punctuatio
-00004a60: 6e73 2061 6e64 2027 2027 206e 6f74 2069  ns and ' ' not i
-00004a70: 6e20 7072 6570 656e 645f 7075 6e63 7475  n prepend_punctu
-00004a80: 6174 696f 6e73 3a0d 0a20 2020 2020 2020  ations:..       
-00004a90: 2020 2020 2070 7265 7065 6e64 5f70 756e       prepend_pun
-00004aa0: 6374 7561 7469 6f6e 7320 2b3d 2027 2027  ctuations += ' '
-00004ab0: 0d0a 2020 2020 2020 2020 6170 7065 6e64  ..        append
-00004ac0: 5f70 756e 6374 7561 7469 6f6e 7320 3d20  _punctuations = 
-00004ad0: 6765 745f 6170 7065 6e64 5f70 756e 6374  get_append_punct
-00004ae0: 7561 7469 6f6e 7328 6170 7065 6e64 5f70  uations(append_p
-00004af0: 756e 6374 7561 7469 6f6e 7329 0d0a 2020  unctuations)..  
-00004b00: 2020 2020 2020 7365 6c66 5f63 6f70 7920        self_copy 
-00004b10: 3d20 7365 6c66 2e63 6f70 7928 636f 7079  = self.copy(copy
-00004b20: 5f77 6f72 6473 3d54 7275 6529 0d0a 2020  _words=True)..  
-00004b30: 2020 2020 2020 6861 735f 7072 6570 656e        has_prepen
-00004b40: 6420 3d20 626f 6f6c 2870 7265 7065 6e64  d = bool(prepend
-00004b50: 5f70 756e 6374 7561 7469 6f6e 7329 0d0a  _punctuations)..
-00004b60: 2020 2020 2020 2020 6861 735f 6170 7065          has_appe
-00004b70: 6e64 203d 2062 6f6f 6c28 6170 7065 6e64  nd = bool(append
-00004b80: 5f70 756e 6374 7561 7469 6f6e 7329 0d0a  _punctuations)..
-00004b90: 2020 2020 2020 2020 6966 2068 6173 5f70          if has_p
-00004ba0: 7265 7065 6e64 206f 7220 6861 735f 6170  repend or has_ap
-00004bb0: 7065 6e64 3a0d 0a20 2020 2020 2020 2020  pend:..         
-00004bc0: 2020 2077 6f72 645f 6f62 6a73 203d 2028     word_objs = (
-00004bd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004be0: 2020 7365 6c66 5f63 6f70 792e 776f 7264    self_copy.word
-00004bf0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00004c00: 2020 2069 6620 7365 6c66 5f63 6f70 792e     if self_copy.
-00004c10: 6861 735f 776f 7264 7320 656c 7365 0d0a  has_words else..
-00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 5b57 6f72 6454 696d 696e 6728 772c 2030  [WordTiming(w, 0
-00004c40: 2c20 312c 2030 2920 666f 7220 7720 696e  , 1, 0) for w in
-00004c50: 2073 656c 665f 636f 7079 2e74 6578 742e   self_copy.text.
-00004c60: 7370 6c69 7428 2720 2729 5d0d 0a20 2020  split(' ')]..   
-00004c70: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00004c80: 2020 2020 2020 2020 666f 7220 776f 7264          for word
-00004c90: 2069 6e20 776f 7264 5f6f 626a 733a 0d0a   in word_objs:..
-00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cb0: 6e65 775f 6170 7065 6e64 203d 2027 270d  new_append = ''.
-00004cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004cd0: 2069 6620 6861 735f 7072 6570 656e 643a   if has_prepend:
-00004ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004cf0: 2020 2020 2020 666f 7220 5f20 696e 2072        for _ in r
-00004d00: 616e 6765 286c 656e 2877 6f72 6429 293a  ange(len(word)):
-00004d10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004d20: 2020 2020 2020 2020 2020 6368 6172 203d            char =
-00004d30: 2077 6f72 642e 776f 7264 5b30 5d0d 0a20   word.word[0].. 
-00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d50: 2020 2020 2020 2069 6620 6368 6172 2069         if char i
-00004d60: 6e20 7072 6570 656e 645f 7075 6e63 7475  n prepend_punctu
-00004d70: 6174 696f 6e73 3a0d 0a20 2020 2020 2020  ations:..       
-00004d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d90: 2020 2020 206e 6577 5f61 7070 656e 6420       new_append 
-00004da0: 2b3d 2063 6861 720d 0a20 2020 2020 2020  += char..       
+00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002650: 2020 2073 7461 636b 6c65 7665 6c3d 3229     stacklevel=2)
+00002660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002670: 2020 6966 2074 6f6b 656e 7320 6973 206e    if tokens is n
+00002680: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00002690: 2020 2020 2020 2020 2020 2020 2020 7761                wa
+000026a0: 726e 696e 6773 2e77 6172 6e28 2754 6865  rnings.warn('The
+000026b0: 2061 7267 756d 656e 7420 666f 7220 6060   argument for ``
+000026c0: 746f 6b65 6e73 6060 2077 696c 6c20 6265  tokens`` will be
+000026d0: 2069 676e 6f72 6564 2027 0d0a 2020 2020   ignored '..    
+000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2761                'a
+00002700: 6e64 2069 7420 7769 6c6c 2061 6c77 6179  nd it will alway
+00002710: 7320 6265 2074 6865 2063 6f6e 6361 7465  s be the concate
+00002720: 6e61 7469 6f6e 206f 6620 746f 6b65 6e73  nation of tokens
+00002730: 2069 6e20 6060 776f 7264 7360 6027 2c0d   in ``words``',.
+00002740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 2073 7461 636b 6c65 7665 6c3d 3229     stacklevel=2)
+00002770: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
+00002780: 6f75 6e64 5f74 7320 3d20 726f 756e 645f  ound_ts = round_
+00002790: 7473 0d0a 2020 2020 2020 2020 7365 6c66  ts..        self
+000027a0: 2e5f 6465 6661 756c 745f 7374 6172 7420  ._default_start 
+000027b0: 3d20 7365 6c66 2e72 6f75 6e64 2873 7461  = self.round(sta
+000027c0: 7274 2920 6966 2073 7461 7274 2065 6c73  rt) if start els
+000027d0: 6520 302e 300d 0a20 2020 2020 2020 2073  e 0.0..        s
+000027e0: 656c 662e 5f64 6566 6175 6c74 5f65 6e64  elf._default_end
+000027f0: 203d 2073 656c 662e 726f 756e 6428 656e   = self.round(en
+00002800: 6429 2069 6620 656e 6420 656c 7365 2030  d) if end else 0
+00002810: 2e30 0d0a 2020 2020 2020 2020 7365 6c66  .0..        self
+00002820: 2e5f 6465 6661 756c 745f 7465 7874 203d  ._default_text =
+00002830: 2074 6578 7420 6f72 2027 270d 0a20 2020   text or ''..   
+00002840: 2020 2020 2073 656c 662e 5f64 6566 6175       self._defau
+00002850: 6c74 5f74 6f6b 656e 7320 3d20 746f 6b65  lt_tokens = toke
+00002860: 6e73 206f 7220 5b5d 0d0a 2020 2020 2020  ns or []..      
+00002870: 2020 7365 6c66 2e73 6565 6b20 3d20 7365    self.seek = se
+00002880: 656b 0d0a 2020 2020 2020 2020 7365 6c66  ek..        self
+00002890: 2e74 656d 7065 7261 7475 7265 203d 2074  .temperature = t
+000028a0: 656d 7065 7261 7475 7265 0d0a 2020 2020  emperature..    
+000028b0: 2020 2020 7365 6c66 2e61 7667 5f6c 6f67      self.avg_log
+000028c0: 7072 6f62 203d 2061 7667 5f6c 6f67 7072  prob = avg_logpr
+000028d0: 6f62 0d0a 2020 2020 2020 2020 7365 6c66  ob..        self
+000028e0: 2e63 6f6d 7072 6573 7369 6f6e 5f72 6174  .compression_rat
+000028f0: 696f 203d 2063 6f6d 7072 6573 7369 6f6e  io = compression
+00002900: 5f72 6174 696f 0d0a 2020 2020 2020 2020  _ratio..        
+00002910: 7365 6c66 2e6e 6f5f 7370 6565 6368 5f70  self.no_speech_p
+00002920: 726f 6220 3d20 6e6f 5f73 7065 6563 685f  rob = no_speech_
+00002930: 7072 6f62 0d0a 2020 2020 2020 2020 7365  prob..        se
+00002940: 6c66 2e77 6f72 6473 203d 2077 6f72 6473  lf.words = words
+00002950: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00002960: 662e 776f 7264 7320 616e 6420 6973 696e  f.words and isin
+00002970: 7374 616e 6365 2877 6f72 6473 5b30 5d2c  stance(words[0],
+00002980: 2064 6963 7429 3a0d 0a20 2020 2020 2020   dict):..       
+00002990: 2020 2020 2073 656c 662e 776f 7264 7320       self.words 
+000029a0: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
+000029b0: 2020 2020 2057 6f72 6454 696d 696e 6728       WordTiming(
+000029c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000029d0: 2020 2020 2020 2a2a 776f 7264 2c0d 0a20        **word,.. 
+000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029f0: 2020 2073 6567 6d65 6e74 3d73 656c 662c     segment=self,
+00002a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002a10: 2020 2020 2020 726f 756e 645f 7473 3d73        round_ts=s
+00002a20: 656c 662e 726f 756e 645f 7473 2c0d 0a20  elf.round_ts,.. 
+00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a40: 2020 2069 676e 6f72 655f 756e 7573 6564     ignore_unused
+00002a50: 5f61 7267 733d 5472 7565 0d0a 2020 2020  _args=True..    
+00002a60: 2020 2020 2020 2020 2020 2020 2920 666f              ) fo
+00002a70: 7220 776f 7264 2069 6e20 7365 6c66 2e77  r word in self.w
+00002a80: 6f72 6473 0d0a 2020 2020 2020 2020 2020  ords..          
+00002a90: 2020 5d0d 0a20 2020 2020 2020 2073 656c    ]..        sel
+00002aa0: 662e 6964 203d 2069 640d 0a20 2020 2020  f.id = id..     
+00002ab0: 2020 2073 656c 662e 5f72 6576 6572 7365     self._reverse
+00002ac0: 645f 7465 7874 203d 2046 616c 7365 0d0a  d_text = False..
+00002ad0: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
+00002ae0: 756c 7420 3d20 7265 7375 6c74 0d0a 0d0a  ult = result....
+00002af0: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
+00002b00: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00002b10: 2072 6574 7572 6e20 6627 5365 676d 656e   return f'Segmen
+00002b20: 7428 7374 6172 743d 7b73 656c 662e 7374  t(start={self.st
+00002b30: 6172 747d 2c20 656e 643d 7b73 656c 662e  art}, end={self.
+00002b40: 656e 647d 2c20 7465 7874 3d22 7b73 656c  end}, text="{sel
+00002b50: 662e 7465 7874 7d22 2927 0d0a 0d0a 2020  f.text}")'....  
+00002b60: 2020 6465 6620 5f5f 6765 7469 7465 6d5f    def __getitem_
+00002b70: 5f28 7365 6c66 2c20 696e 6465 783a 2069  _(self, index: i
+00002b80: 6e74 2920 2d3e 2057 6f72 6454 696d 696e  nt) -> WordTimin
+00002b90: 673a 0d0a 2020 2020 2020 2020 6966 2073  g:..        if s
+00002ba0: 656c 662e 776f 7264 7320 6973 204e 6f6e  elf.words is Non
+00002bb0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002bc0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00002bd0: 2827 7365 676d 656e 7420 636f 6e74 6169  ('segment contai
+00002be0: 6e73 206e 6f20 776f 7264 7327 290d 0a20  ns no words').. 
+00002bf0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00002c00: 6c66 2e77 6f72 6473 5b69 6e64 6578 5d0d  lf.words[index].
+00002c10: 0a0d 0a20 2020 2064 6566 205f 5f64 656c  ...    def __del
+00002c20: 6974 656d 5f5f 2873 656c 662c 2069 6e64  item__(self, ind
+00002c30: 6578 3a20 696e 7429 3a0d 0a20 2020 2020  ex: int):..     
+00002c40: 2020 2069 6620 7365 6c66 2e77 6f72 6473     if self.words
+00002c50: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00002c60: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00002c70: 7565 4572 726f 7228 2773 6567 6d65 6e74  ueError('segment
+00002c80: 2063 6f6e 7461 696e 7320 6e6f 2077 6f72   contains no wor
+00002c90: 6473 2729 0d0a 2020 2020 2020 2020 6465  ds')..        de
+00002ca0: 6c20 7365 6c66 2e77 6f72 6473 5b69 6e64  l self.words[ind
+00002cb0: 6578 5d0d 0a20 2020 2020 2020 2073 656c  ex]..        sel
+00002cc0: 662e 7265 6173 7369 676e 5f69 6473 2869  f.reassign_ids(i
+00002cd0: 6e64 6578 290d 0a0d 0a20 2020 2064 6566  ndex)....    def
+00002ce0: 205f 5f64 6565 7063 6f70 795f 5f28 7365   __deepcopy__(se
+00002cf0: 6c66 2c20 6d65 6d6f 3d4e 6f6e 6529 3a0d  lf, memo=None):.
+00002d00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002d10: 7365 6c66 2e63 6f70 7928 636f 7079 5f77  self.copy(copy_w
+00002d20: 6f72 6473 3d54 7275 652c 2063 6f70 795f  ords=True, copy_
+00002d30: 746f 6b65 6e73 3d54 7275 6529 0d0a 0d0a  tokens=True)....
+00002d40: 2020 2020 6465 6620 5f5f 636f 7079 5f5f      def __copy__
+00002d50: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00002d60: 2072 6574 7572 6e20 7365 6c66 2e63 6f70   return self.cop
+00002d70: 7928 290d 0a0d 0a20 2020 2064 6566 2063  y()....    def c
+00002d80: 6f70 7928 0d0a 2020 2020 2020 2020 2020  opy(..          
+00002d90: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
+00002da0: 2020 2020 206e 6577 5f77 6f72 6473 3a20       new_words: 
+00002db0: 4f70 7469 6f6e 616c 5b4c 6973 745b 576f  Optional[List[Wo
+00002dc0: 7264 5469 6d69 6e67 5d5d 203d 204e 6f6e  rdTiming]] = Non
+00002dd0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00002de0: 6b65 6570 5f72 6573 756c 743a 2062 6f6f  keep_result: boo
+00002df0: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
+00002e00: 2020 2020 2020 2020 636f 7079 5f77 6f72          copy_wor
+00002e10: 6473 3a20 626f 6f6c 203d 2046 616c 7365  ds: bool = False
+00002e20: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
+00002e30: 6f70 795f 746f 6b65 6e73 3a20 626f 6f6c  opy_tokens: bool
+00002e40: 203d 2046 616c 7365 0d0a 2020 2020 293a   = False..    ):
+00002e50: 0d0a 2020 2020 2020 2020 6966 206e 6577  ..        if new
+00002e60: 5f77 6f72 6473 2069 7320 4e6f 6e65 3a0d  _words is None:.
+00002e70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002e80: 7365 6c66 2e68 6173 5f77 6f72 6473 3a0d  self.has_words:.
+00002e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ea0: 2077 6f72 6473 203d 205b 772e 636f 7079   words = [w.copy
+00002eb0: 2863 6f70 795f 746f 6b65 6e73 3d63 6f70  (copy_tokens=cop
+00002ec0: 795f 746f 6b65 6e73 2920 666f 7220 7720  y_tokens) for w 
+00002ed0: 696e 2073 656c 662e 776f 7264 735d 2069  in self.words] i
+00002ee0: 6620 636f 7079 5f77 6f72 6473 2065 6c73  f copy_words els
+00002ef0: 6520 7365 6c66 2e77 6f72 6473 0d0a 2020  e self.words..  
+00002f00: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00002f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002f20: 2077 6f72 6473 203d 204e 6f6e 650d 0a20   words = None.. 
+00002f30: 2020 2020 2020 2020 2020 2064 6566 5f73             def_s
+00002f40: 7461 7274 203d 2073 656c 662e 5f64 6566  tart = self._def
+00002f50: 6175 6c74 5f73 7461 7274 0d0a 2020 2020  ault_start..    
+00002f60: 2020 2020 2020 2020 6465 665f 656e 6420          def_end 
+00002f70: 3d20 7365 6c66 2e5f 6465 6661 756c 745f  = self._default_
+00002f80: 656e 640d 0a20 2020 2020 2020 2020 2020  end..           
+00002f90: 2064 6566 5f74 6578 7420 3d20 7365 6c66   def_text = self
+00002fa0: 2e5f 6465 6661 756c 745f 7465 7874 0d0a  ._default_text..
+00002fb0: 2020 2020 2020 2020 2020 2020 6465 665f              def_
+00002fc0: 746f 6b65 6e73 203d 2073 656c 662e 5f64  tokens = self._d
+00002fd0: 6566 6175 6c74 5f74 6f6b 656e 730d 0a20  efault_tokens.. 
+00002fe0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00002ff0: 2020 2020 2020 2020 2020 776f 7264 7320            words 
+00003000: 3d20 5b77 2e63 6f70 7928 636f 7079 5f74  = [w.copy(copy_t
+00003010: 6f6b 656e 733d 636f 7079 5f74 6f6b 656e  okens=copy_token
+00003020: 7329 2066 6f72 2077 2069 6e20 6e65 775f  s) for w in new_
+00003030: 776f 7264 735d 2069 6620 636f 7079 5f77  words] if copy_w
+00003040: 6f72 6473 2065 6c73 6520 6e65 775f 776f  ords else new_wo
+00003050: 7264 730d 0a20 2020 2020 2020 2020 2020  rds..           
+00003060: 2064 6566 5f73 7461 7274 203d 2064 6566   def_start = def
+00003070: 5f65 6e64 203d 2064 6566 5f74 6578 7420  _end = def_text 
+00003080: 3d20 6465 665f 746f 6b65 6e73 203d 204e  = def_tokens = N
+00003090: 6f6e 650d 0a20 2020 2020 2020 206e 6577  one..        new
+000030a0: 5f73 6567 203d 2053 6567 6d65 6e74 280d  _seg = Segment(.
+000030b0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+000030c0: 7274 3d64 6566 5f73 7461 7274 2c0d 0a20  rt=def_start,.. 
+000030d0: 2020 2020 2020 2020 2020 2065 6e64 3d64             end=d
+000030e0: 6566 5f65 6e64 2c0d 0a20 2020 2020 2020  ef_end,..       
+000030f0: 2020 2020 2074 6578 743d 6465 665f 7465       text=def_te
+00003100: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
+00003110: 2073 6565 6b3d 7365 6c66 2e73 6565 6b2c   seek=self.seek,
+00003120: 0d0a 2020 2020 2020 2020 2020 2020 746f  ..            to
+00003130: 6b65 6e73 3d64 6566 5f74 6f6b 656e 732c  kens=def_tokens,
+00003140: 0d0a 2020 2020 2020 2020 2020 2020 7465  ..            te
+00003150: 6d70 6572 6174 7572 653d 7365 6c66 2e74  mperature=self.t
+00003160: 656d 7065 7261 7475 7265 2c0d 0a20 2020  emperature,..   
+00003170: 2020 2020 2020 2020 2061 7667 5f6c 6f67           avg_log
+00003180: 7072 6f62 3d73 656c 662e 6176 675f 6c6f  prob=self.avg_lo
+00003190: 6770 726f 622c 0d0a 2020 2020 2020 2020  gprob,..        
+000031a0: 2020 2020 636f 6d70 7265 7373 696f 6e5f      compression_
+000031b0: 7261 7469 6f3d 7365 6c66 2e63 6f6d 7072  ratio=self.compr
+000031c0: 6573 7369 6f6e 5f72 6174 696f 2c0d 0a20  ession_ratio,.. 
+000031d0: 2020 2020 2020 2020 2020 206e 6f5f 7370             no_sp
+000031e0: 6565 6368 5f70 726f 623d 7365 6c66 2e6e  eech_prob=self.n
+000031f0: 6f5f 7370 6565 6368 5f70 726f 622c 0d0a  o_speech_prob,..
+00003200: 2020 2020 2020 2020 2020 2020 776f 7264              word
+00003210: 733d 776f 7264 732c 0d0a 2020 2020 2020  s=words,..      
+00003220: 2020 2020 2020 6964 3d73 656c 662e 6964        id=self.id
+00003230: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00003240: 6573 756c 743d 7365 6c66 2e72 6573 756c  esult=self.resul
+00003250: 7420 6966 206b 6565 705f 7265 7375 6c74  t if keep_result
+00003260: 2065 6c73 6520 4e6f 6e65 2c0d 0a20 2020   else None,..   
+00003270: 2020 2020 2020 2020 2072 6f75 6e64 5f74           round_t
+00003280: 733d 7365 6c66 2e72 6f75 6e64 5f74 732c  s=self.round_ts,
+00003290: 0d0a 2020 2020 2020 2020 2020 2020 6967  ..            ig
+000032a0: 6e6f 7265 5f75 6e75 7365 645f 6172 6773  nore_unused_args
+000032b0: 3d54 7275 650d 0a20 2020 2020 2020 2029  =True..        )
+000032c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000032d0: 206e 6577 5f73 6567 0d0a 0d0a 2020 2020   new_seg....    
+000032e0: 6465 6620 726f 756e 6428 7365 6c66 2c20  def round(self, 
+000032f0: 7469 6d65 7374 616d 703a 2066 6c6f 6174  timestamp: float
+00003300: 2920 2d3e 2066 6c6f 6174 3a0d 0a20 2020  ) -> float:..   
+00003310: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00003320: 2e72 6f75 6e64 5f74 733a 0d0a 2020 2020  .round_ts:..    
+00003330: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00003340: 696d 6573 7461 6d70 0d0a 2020 2020 2020  imestamp..      
+00003350: 2020 7265 7475 726e 205f 726f 756e 645f    return _round_
+00003360: 7469 6d65 7374 616d 7028 7469 6d65 7374  timestamp(timest
+00003370: 616d 7029 0d0a 0d0a 2020 2020 6465 6620  amp)....    def 
+00003380: 746f 5f64 6973 706c 6179 5f73 7472 2873  to_display_str(s
+00003390: 656c 662c 206f 6e6c 795f 7365 676d 656e  elf, only_segmen
+000033a0: 743a 2062 6f6f 6c20 3d20 4661 6c73 6529  t: bool = False)
+000033b0: 3a0d 0a20 2020 2020 2020 206c 696e 6520  :..        line 
+000033c0: 3d20 6627 5b7b 666f 726d 6174 5f74 696d  = f'[{format_tim
+000033d0: 6573 7461 6d70 2873 656c 662e 7374 6172  estamp(self.star
+000033e0: 7429 7d20 2d2d 3e20 7b66 6f72 6d61 745f  t)} --> {format_
+000033f0: 7469 6d65 7374 616d 7028 7365 6c66 2e65  timestamp(self.e
+00003400: 6e64 297d 5d20 227b 7365 6c66 2e74 6578  nd)}] "{self.tex
+00003410: 747d 2227 0d0a 2020 2020 2020 2020 6966  t}"'..        if
+00003420: 2073 656c 662e 6861 735f 776f 7264 7320   self.has_words 
+00003430: 616e 6420 6e6f 7420 6f6e 6c79 5f73 6567  and not only_seg
+00003440: 6d65 6e74 3a0d 0a20 2020 2020 2020 2020  ment:..         
+00003450: 2020 206c 696e 6520 2b3d 2027 5c6e 2720     line += '\n' 
+00003460: 2b20 275c 6e27 2e6a 6f69 6e28 0d0a 2020  + '\n'.join(..  
+00003470: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00003480: 2d5b 7b66 6f72 6d61 745f 7469 6d65 7374  -[{format_timest
+00003490: 616d 7028 772e 7374 6172 7429 7d5d 202d  amp(w.start)}] -
+000034a0: 3e20 5b7b 666f 726d 6174 5f74 696d 6573  > [{format_times
+000034b0: 7461 6d70 2877 2e65 6e64 297d 5d20 5c22  tamp(w.end)}] \"
+000034c0: 7b77 2e77 6f72 647d 5c22 2220 666f 7220  {w.word}\"" for 
+000034d0: 7720 696e 2073 656c 662e 776f 7264 730d  w in self.words.
+000034e0: 0a20 2020 2020 2020 2020 2020 2029 202b  .            ) +
+000034f0: 2027 5c6e 270d 0a20 2020 2020 2020 2072   '\n'..        r
+00003500: 6574 7572 6e20 6c69 6e65 0d0a 0d0a 2020  eturn line....  
+00003510: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00003520: 2064 6566 2068 6173 5f77 6f72 6473 2873   def has_words(s
+00003530: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
+00003540: 6574 7572 6e20 626f 6f6c 2873 656c 662e  eturn bool(self.
+00003550: 776f 7264 7329 0d0a 0d0a 2020 2020 4070  words)....    @p
+00003560: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00003570: 206f 7269 5f68 6173 5f77 6f72 6473 2873   ori_has_words(s
+00003580: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
+00003590: 6574 7572 6e20 7365 6c66 2e77 6f72 6473  eturn self.words
+000035a0: 2069 7320 6e6f 7420 4e6f 6e65 0d0a 0d0a   is not None....
+000035b0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+000035c0: 2020 2064 6566 2073 7461 7274 2873 656c     def start(sel
+000035d0: 6629 3a0d 0a20 2020 2020 2020 2069 6620  f):..        if 
+000035e0: 7365 6c66 2e68 6173 5f77 6f72 6473 3a0d  self.has_words:.
+000035f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00003600: 7572 6e20 7365 6c66 2e77 6f72 6473 5b30  urn self.words[0
+00003610: 5d2e 7374 6172 740d 0a20 2020 2020 2020  ].start..       
+00003620: 2072 6574 7572 6e20 7365 6c66 2e5f 6465   return self._de
+00003630: 6661 756c 745f 7374 6172 740d 0a0d 0a20  fault_start.... 
+00003640: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
+00003650: 2020 6465 6620 656e 6428 7365 6c66 293a    def end(self):
+00003660: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00003670: 662e 6861 735f 776f 7264 733a 0d0a 2020  f.has_words:..  
+00003680: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00003690: 2073 656c 662e 776f 7264 735b 2d31 5d2e   self.words[-1].
+000036a0: 656e 640d 0a20 2020 2020 2020 2072 6574  end..        ret
+000036b0: 7572 6e20 7365 6c66 2e5f 6465 6661 756c  urn self._defaul
+000036c0: 745f 656e 640d 0a0d 0a20 2020 2040 7374  t_end....    @st
+000036d0: 6172 742e 7365 7474 6572 0d0a 2020 2020  art.setter..    
+000036e0: 6465 6620 7374 6172 7428 7365 6c66 2c20  def start(self, 
+000036f0: 7661 6c29 3a0d 0a20 2020 2020 2020 2069  val):..        i
+00003700: 6620 7365 6c66 2e68 6173 5f77 6f72 6473  f self.has_words
+00003710: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00003720: 656c 662e 776f 7264 735b 305d 2e73 7461  elf.words[0].sta
+00003730: 7274 203d 2076 616c 0d0a 2020 2020 2020  rt = val..      
+00003740: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
+00003750: 2020 2020 2020 7365 6c66 2e5f 6465 6661        self._defa
+00003760: 756c 745f 7374 6172 7420 3d20 7365 6c66  ult_start = self
+00003770: 2e72 6f75 6e64 2876 616c 290d 0a0d 0a20  .round(val).... 
+00003780: 2020 2040 656e 642e 7365 7474 6572 0d0a     @end.setter..
+00003790: 2020 2020 6465 6620 656e 6428 7365 6c66      def end(self
+000037a0: 2c20 7661 6c29 3a0d 0a20 2020 2020 2020  , val):..       
+000037b0: 2069 6620 7365 6c66 2e68 6173 5f77 6f72   if self.has_wor
+000037c0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+000037d0: 2073 656c 662e 776f 7264 735b 2d31 5d2e   self.words[-1].
+000037e0: 656e 6420 3d20 7661 6c0d 0a20 2020 2020  end = val..     
+000037f0: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
+00003800: 2020 2020 2020 2073 656c 662e 5f64 6566         self._def
+00003810: 6175 6c74 5f65 6e64 203d 2073 656c 662e  ault_end = self.
+00003820: 726f 756e 6428 7661 6c29 0d0a 0d0a 2020  round(val)....  
+00003830: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00003840: 2064 6566 2074 6578 7428 7365 6c66 2920   def text(self) 
+00003850: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
+00003860: 2069 6620 7365 6c66 2e68 6173 5f77 6f72   if self.has_wor
+00003870: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00003880: 2072 6574 7572 6e20 2727 2e6a 6f69 6e28   return ''.join(
+00003890: 776f 7264 2e77 6f72 6420 666f 7220 776f  word.word for wo
+000038a0: 7264 2069 6e20 7365 6c66 2e77 6f72 6473  rd in self.words
+000038b0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+000038c0: 6e20 7365 6c66 2e5f 6465 6661 756c 745f  n self._default_
+000038d0: 7465 7874 0d0a 0d0a 2020 2020 4070 726f  text....    @pro
+000038e0: 7065 7274 790d 0a20 2020 2064 6566 2074  perty..    def t
+000038f0: 6f6b 656e 7328 7365 6c66 2920 2d3e 204c  okens(self) -> L
+00003900: 6973 745b 696e 745d 3a0d 0a20 2020 2020  ist[int]:..     
+00003910: 2020 2069 6620 7365 6c66 2e68 6173 5f77     if self.has_w
+00003920: 6f72 6473 2061 6e64 2073 656c 662e 776f  ords and self.wo
+00003930: 7264 735b 305d 2e74 6f6b 656e 733a 0d0a  rds[0].tokens:..
+00003940: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00003950: 726e 206c 6973 7428 6368 6169 6e2e 6672  rn list(chain.fr
+00003960: 6f6d 5f69 7465 7261 626c 6528 776f 7264  om_iterable(word
+00003970: 2e74 6f6b 656e 7320 666f 7220 776f 7264  .tokens for word
+00003980: 2069 6e20 7365 6c66 2e77 6f72 6473 2929   in self.words))
+00003990: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000039a0: 2073 656c 662e 5f64 6566 6175 6c74 5f74   self._default_t
+000039b0: 6f6b 656e 730d 0a0d 0a20 2020 2040 7072  okens....    @pr
+000039c0: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
+000039d0: 6475 7261 7469 6f6e 2873 656c 6629 3a0d  duration(self):.
+000039e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000039f0: 7365 6c66 2e65 6e64 202d 2073 656c 662e  self.end - self.
+00003a00: 7374 6172 740d 0a0d 0a20 2020 2064 6566  start....    def
+00003a10: 2077 6f72 645f 636f 756e 7428 7365 6c66   word_count(self
+00003a20: 293a 0d0a 2020 2020 2020 2020 6966 2073  ):..        if s
+00003a30: 656c 662e 6861 735f 776f 7264 733a 0d0a  elf.has_words:..
+00003a40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00003a50: 726e 206c 656e 2873 656c 662e 776f 7264  rn len(self.word
+00003a60: 7329 0d0a 2020 2020 2020 2020 7265 7475  s)..        retu
+00003a70: 726e 202d 310d 0a0d 0a20 2020 2064 6566  rn -1....    def
+00003a80: 2063 6861 725f 636f 756e 7428 7365 6c66   char_count(self
+00003a90: 293a 0d0a 2020 2020 2020 2020 6966 2073  ):..        if s
+00003aa0: 656c 662e 6861 735f 776f 7264 733a 0d0a  elf.has_words:..
+00003ab0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00003ac0: 726e 2073 756d 286c 656e 2877 2920 666f  rn sum(len(w) fo
+00003ad0: 7220 7720 696e 2073 656c 662e 776f 7264  r w in self.word
+00003ae0: 7329 0d0a 2020 2020 2020 2020 7265 7475  s)..        retu
+00003af0: 726e 206c 656e 2873 656c 662e 7465 7874  rn len(self.text
+00003b00: 290d 0a0d 0a20 2020 2064 6566 2061 6464  )....    def add
+00003b10: 2873 656c 662c 206f 7468 6572 3a20 2753  (self, other: 'S
+00003b20: 6567 6d65 6e74 272c 2063 6f70 795f 776f  egment', copy_wo
+00003b30: 7264 733a 2062 6f6f 6c20 3d20 4661 6c73  rds: bool = Fals
+00003b40: 6529 3a0d 0a20 2020 2020 2020 2069 6620  e):..        if 
+00003b50: 7365 6c66 2e6f 7269 5f68 6173 5f77 6f72  self.ori_has_wor
+00003b60: 6473 203d 3d20 6f74 6865 722e 6f72 695f  ds == other.ori_
+00003b70: 6861 735f 776f 7264 733a 0d0a 2020 2020  has_words:..    
+00003b80: 2020 2020 2020 2020 776f 7264 7320 3d20          words = 
+00003b90: 2873 656c 662e 776f 7264 7320 2b20 6f74  (self.words + ot
+00003ba0: 6865 722e 776f 7264 7329 2069 6620 7365  her.words) if se
+00003bb0: 6c66 2e6f 7269 5f68 6173 5f77 6f72 6473  lf.ori_has_words
+00003bc0: 2065 6c73 6520 4e6f 6e65 0d0a 2020 2020   else None..    
+00003bd0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00003be0: 2020 2020 2020 2073 656c 665f 7374 6174         self_stat
+00003bf0: 6520 3d20 2777 6974 6827 2069 6620 7365  e = 'with' if se
+00003c00: 6c66 2e6f 7269 5f68 6173 5f77 6f72 6473  lf.ori_has_words
+00003c10: 2065 6c73 6520 2777 6974 686f 7574 270d   else 'without'.
+00003c20: 0a20 2020 2020 2020 2020 2020 206f 7468  .            oth
+00003c30: 6572 5f73 7461 7465 203d 2027 7769 7468  er_state = 'with
+00003c40: 2720 6966 206f 7468 6572 2e6f 7269 5f68  ' if other.ori_h
+00003c50: 6173 5f77 6f72 6473 2065 6c73 6520 2777  as_words else 'w
+00003c60: 6974 686f 7574 270d 0a20 2020 2020 2020  ithout'..       
+00003c70: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00003c80: 4572 726f 7228 6622 4361 6e27 7420 6d65  Error(f"Can't me
+00003c90: 7267 6520 7365 676d 656e 7420 7b73 656c  rge segment {sel
+00003ca0: 665f 7374 6174 657d 2077 6f72 6473 2061  f_state} words a
+00003cb0: 6e64 2061 2073 6567 6d65 6e74 207b 6f74  nd a segment {ot
+00003cc0: 6865 725f 7374 6174 657d 2077 6f72 6473  her_state} words
+00003cd0: 2e22 290d 0a0d 0a20 2020 2020 2020 2073  .")....        s
+00003ce0: 656c 665f 636f 7079 203d 2073 656c 662e  elf_copy = self.
+00003cf0: 636f 7079 2877 6f72 6473 2c20 636f 7079  copy(words, copy
+00003d00: 5f77 6f72 6473 3d63 6f70 795f 776f 7264  _words=copy_word
+00003d10: 7329 0d0a 2020 2020 2020 2020 5f63 6f6d  s)..        _com
+00003d20: 6269 6e65 5f61 7474 7228 7365 6c66 5f63  bine_attr(self_c
+00003d30: 6f70 792c 206f 7468 6572 2c20 2774 656d  opy, other, 'tem
+00003d40: 7065 7261 7475 7265 2729 0d0a 2020 2020  perature')..    
+00003d50: 2020 2020 5f63 6f6d 6269 6e65 5f61 7474      _combine_att
+00003d60: 7228 7365 6c66 5f63 6f70 792c 206f 7468  r(self_copy, oth
+00003d70: 6572 2c20 2761 7667 5f6c 6f67 7072 6f62  er, 'avg_logprob
+00003d80: 2729 0d0a 2020 2020 2020 2020 5f63 6f6d  ')..        _com
+00003d90: 6269 6e65 5f61 7474 7228 7365 6c66 5f63  bine_attr(self_c
+00003da0: 6f70 792c 206f 7468 6572 2c20 2763 6f6d  opy, other, 'com
+00003db0: 7072 6573 7369 6f6e 5f72 6174 696f 2729  pression_ratio')
+00003dc0: 0d0a 2020 2020 2020 2020 5f63 6f6d 6269  ..        _combi
+00003dd0: 6e65 5f61 7474 7228 7365 6c66 5f63 6f70  ne_attr(self_cop
+00003de0: 792c 206f 7468 6572 2c20 276e 6f5f 7370  y, other, 'no_sp
+00003df0: 6565 6368 5f70 726f 6227 290d 0a0d 0a20  eech_prob').... 
+00003e00: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00003e10: 6c66 5f63 6f70 790d 0a0d 0a20 2020 2064  lf_copy....    d
+00003e20: 6566 205f 5f61 6464 5f5f 2873 656c 662c  ef __add__(self,
+00003e30: 206f 7468 6572 3a20 2753 6567 6d65 6e74   other: 'Segment
+00003e40: 2729 3a0d 0a20 2020 2020 2020 2072 6574  '):..        ret
+00003e50: 7572 6e20 7365 6c66 2e61 6464 286f 7468  urn self.add(oth
+00003e60: 6572 2c20 636f 7079 5f77 6f72 6473 3d54  er, copy_words=T
+00003e70: 7275 6529 0d0a 0d0a 2020 2020 6465 6620  rue)....    def 
+00003e80: 5f77 6f72 645f 6f70 6572 6174 696f 6e73  _word_operations
+00003e90: 2873 656c 662c 206f 7065 7261 7469 6f6e  (self, operation
+00003ea0: 3a20 7374 722c 202a 6172 6773 2c20 2a2a  : str, *args, **
+00003eb0: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+00003ec0: 2020 6966 2073 656c 662e 6861 735f 776f    if self.has_wo
+00003ed0: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
+00003ee0: 2020 666f 7220 7720 696e 2073 656c 662e    for w in self.
+00003ef0: 776f 7264 733a 0d0a 2020 2020 2020 2020  words:..        
+00003f00: 2020 2020 2020 2020 6765 7461 7474 7228          getattr(
+00003f10: 772c 206f 7065 7261 7469 6f6e 2928 2a61  w, operation)(*a
+00003f20: 7267 732c 202a 2a6b 7761 7267 7329 0d0a  rgs, **kwargs)..
+00003f30: 0d0a 2020 2020 6465 6620 726f 756e 645f  ..    def round_
+00003f40: 616c 6c5f 7469 6d65 7374 616d 7073 2873  all_timestamps(s
+00003f50: 656c 6629 3a0d 0a20 2020 2020 2020 2077  elf):..        w
+00003f60: 6172 6e69 6e67 732e 7761 726e 2827 6060  arnings.warn('``
+00003f70: 2e72 6f75 6e64 5f61 6c6c 5f74 696d 6573  .round_all_times
+00003f80: 7461 6d70 7328 2960 6020 6973 2064 6570  tamps()`` is dep
+00003f90: 7265 6361 7465 6420 616e 6420 7769 6c6c  recated and will
+00003fa0: 2062 6520 7265 6d6f 7665 6420 696e 2066   be removed in f
+00003fb0: 7574 7572 6520 7665 7273 696f 6e73 2e20  uture versions. 
+00003fc0: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
+00003fd0: 2020 2020 2020 2020 2027 5573 6520 6060           'Use ``
+00003fe0: 2e72 6f75 6e64 5f74 733d 5472 7565 6060  .round_ts=True``
+00003ff0: 2074 6f20 726f 756e 6420 7469 6d65 7374   to round timest
+00004000: 616d 7073 2062 7920 6465 6661 756c 7420  amps by default 
+00004010: 696e 7374 6561 642e 272c 0d0a 2020 2020  instead.',..    
+00004020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004030: 2020 7374 6163 6b6c 6576 656c 3d32 290d    stacklevel=2).
+00004040: 0a20 2020 2020 2020 2073 656c 662e 726f  .        self.ro
+00004050: 756e 645f 7473 203d 2054 7275 650d 0a0d  und_ts = True...
+00004060: 0a20 2020 2064 6566 206f 6666 7365 745f  .    def offset_
+00004070: 7469 6d65 2873 656c 662c 206f 6666 7365  time(self, offse
+00004080: 745f 7365 636f 6e64 733a 2066 6c6f 6174  t_seconds: float
+00004090: 293a 0d0a 2020 2020 2020 2020 6966 2073  ):..        if s
+000040a0: 656c 662e 7365 656b 2069 7320 6e6f 7420  elf.seek is not 
+000040b0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000040c0: 2020 2073 656c 662e 7365 656b 202b 3d20     self.seek += 
+000040d0: 6f66 6673 6574 5f73 6563 6f6e 6473 0d0a  offset_seconds..
+000040e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000040f0: 6861 735f 776f 7264 733a 0d0a 2020 2020  has_words:..    
+00004100: 2020 2020 2020 2020 7365 6c66 2e5f 776f          self._wo
+00004110: 7264 5f6f 7065 7261 7469 6f6e 7328 276f  rd_operations('o
+00004120: 6666 7365 745f 7469 6d65 272c 206f 6666  ffset_time', off
+00004130: 7365 745f 7365 636f 6e64 7329 0d0a 2020  set_seconds)..  
+00004140: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00004150: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00004160: 6172 7420 3d20 7365 6c66 2e73 7461 7274  art = self.start
+00004170: 202b 206f 6666 7365 745f 7365 636f 6e64   + offset_second
+00004180: 730d 0a20 2020 2020 2020 2020 2020 2073  s..            s
+00004190: 656c 662e 656e 6420 3d20 7365 6c66 2e65  elf.end = self.e
+000041a0: 6e64 202b 206f 6666 7365 745f 7365 636f  nd + offset_seco
+000041b0: 6e64 730d 0a0d 0a20 2020 2064 6566 2061  nds....    def a
+000041c0: 6464 5f77 6f72 6473 2873 656c 662c 2069  dd_words(self, i
+000041d0: 6e64 6578 303a 2069 6e74 2c20 696e 6465  ndex0: int, inde
+000041e0: 7831 3a20 696e 742c 2069 6e70 6c61 6365  x1: int, inplace
+000041f0: 3a20 626f 6f6c 203d 2046 616c 7365 293a  : bool = False):
+00004200: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00004210: 662e 6861 735f 776f 7264 733a 0d0a 2020  f.has_words:..  
+00004220: 2020 2020 2020 2020 2020 6e65 775f 776f            new_wo
+00004230: 7264 203d 2073 656c 662e 776f 7264 735b  rd = self.words[
+00004240: 696e 6465 7830 5d20 2b20 7365 6c66 2e77  index0] + self.w
+00004250: 6f72 6473 5b69 6e64 6578 315d 0d0a 2020  ords[index1]..  
+00004260: 2020 2020 2020 2020 2020 6966 2069 6e70            if inp
+00004270: 6c61 6365 3a0d 0a20 2020 2020 2020 2020  lace:..         
+00004280: 2020 2020 2020 2069 302c 2069 3120 3d20         i0, i1 = 
+00004290: 736f 7274 6564 285b 696e 6465 7830 2c20  sorted([index0, 
+000042a0: 696e 6465 7831 5d29 0d0a 2020 2020 2020  index1])..      
+000042b0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
+000042c0: 6f72 6473 5b69 305d 203d 206e 6577 5f77  ords[i0] = new_w
+000042d0: 6f72 640d 0a20 2020 2020 2020 2020 2020  ord..           
+000042e0: 2020 2020 2064 656c 2073 656c 662e 776f       del self.wo
+000042f0: 7264 735b 6931 5d0d 0a20 2020 2020 2020  rds[i1]..       
+00004300: 2020 2020 2072 6574 7572 6e20 6e65 775f       return new_
+00004310: 776f 7264 0d0a 0d0a 2020 2020 6465 6620  word....    def 
+00004320: 7265 7363 616c 655f 7469 6d65 2873 656c  rescale_time(sel
+00004330: 662c 2073 6361 6c65 5f66 6163 746f 723a  f, scale_factor:
+00004340: 2066 6c6f 6174 293a 0d0a 2020 2020 2020   float):..      
+00004350: 2020 6966 2073 656c 662e 7365 656b 2069    if self.seek i
+00004360: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00004370: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00004380: 656b 202a 3d20 7363 616c 655f 6661 6374  ek *= scale_fact
+00004390: 6f72 0d0a 2020 2020 2020 2020 6966 2073  or..        if s
+000043a0: 656c 662e 6861 735f 776f 7264 733a 0d0a  elf.has_words:..
+000043b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000043c0: 2e5f 776f 7264 5f6f 7065 7261 7469 6f6e  ._word_operation
+000043d0: 7328 2772 6573 6361 6c65 5f74 696d 6527  s('rescale_time'
+000043e0: 2c20 7363 616c 655f 6661 6374 6f72 290d  , scale_factor).
+000043f0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00004400: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00004410: 2e73 7461 7274 203d 2073 656c 662e 7374  .start = self.st
+00004420: 6172 7420 2a20 7363 616c 655f 6661 6374  art * scale_fact
+00004430: 6f72 0d0a 2020 2020 2020 2020 2020 2020  or..            
+00004440: 7365 6c66 2e65 6e64 203d 2073 656c 662e  self.end = self.
+00004450: 656e 6420 2a20 7363 616c 655f 6661 6374  end * scale_fact
+00004460: 6f72 0d0a 0d0a 2020 2020 6465 6620 6170  or....    def ap
+00004470: 706c 795f 6d69 6e5f 6475 7228 7365 6c66  ply_min_dur(self
+00004480: 2c20 6d69 6e5f 6475 723a 2066 6c6f 6174  , min_dur: float
+00004490: 2c20 696e 706c 6163 653a 2062 6f6f 6c20  , inplace: bool 
+000044a0: 3d20 4661 6c73 6529 3a0d 0a20 2020 2020  = False):..     
+000044b0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000044c0: 4d65 7267 6520 616e 7920 776f 7264 2077  Merge any word w
+000044d0: 6974 6820 6164 6a61 6365 6e74 2077 6f72  ith adjacent wor
+000044e0: 6420 6966 2069 7473 2064 7572 6174 696f  d if its duratio
+000044f0: 6e20 6973 206c 6573 7320 7468 616e 2060  n is less than `
+00004500: 606d 696e 5f64 7572 6060 2e0d 0a20 2020  `min_dur``...   
+00004510: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00004520: 2020 7365 676d 656e 7420 3d20 7365 6c66    segment = self
+00004530: 2069 6620 696e 706c 6163 6520 656c 7365   if inplace else
+00004540: 2064 6565 7063 6f70 7928 7365 6c66 290d   deepcopy(self).
+00004550: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00004560: 7365 6c66 2e68 6173 5f77 6f72 6473 3a0d  self.has_words:.
+00004570: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00004580: 7572 6e20 7365 676d 656e 740d 0a20 2020  urn segment..   
+00004590: 2020 2020 206d 6178 5f69 203d 206c 656e       max_i = len
+000045a0: 2873 6567 6d65 6e74 2e77 6f72 6473 2920  (segment.words) 
+000045b0: 2d20 310d 0a20 2020 2020 2020 2069 6620  - 1..        if 
+000045c0: 6d61 785f 6920 3d3d 2030 3a0d 0a20 2020  max_i == 0:..   
+000045d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000045e0: 7365 676d 656e 740d 0a20 2020 2020 2020  segment..       
+000045f0: 2066 6f72 2069 2069 6e20 7265 7665 7273   for i in revers
+00004600: 6564 2872 616e 6765 286c 656e 2873 6567  ed(range(len(seg
+00004610: 6d65 6e74 2e77 6f72 6473 2929 293a 0d0a  ment.words))):..
+00004620: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00004630: 6178 5f69 203d 3d20 303a 0d0a 2020 2020  ax_i == 0:..    
+00004640: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00004650: 6b0d 0a20 2020 2020 2020 2020 2020 2069  k..            i
+00004660: 6620 7365 676d 656e 742e 776f 7264 735b  f segment.words[
+00004670: 695d 2e64 7572 6174 696f 6e20 3c20 6d69  i].duration < mi
+00004680: 6e5f 6475 723a 0d0a 2020 2020 2020 2020  n_dur:..        
+00004690: 2020 2020 2020 2020 6966 2069 203d 3d20          if i == 
+000046a0: 6d61 785f 693a 0d0a 2020 2020 2020 2020  max_i:..        
+000046b0: 2020 2020 2020 2020 2020 2020 7365 676d              segm
+000046c0: 656e 742e 6164 645f 776f 7264 7328 692d  ent.add_words(i-
+000046d0: 312c 2069 2c20 696e 706c 6163 653d 5472  1, i, inplace=Tr
+000046e0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+000046f0: 2020 2020 2065 6c69 6620 6920 3d3d 2030       elif i == 0
+00004700: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004710: 2020 2020 2020 2073 6567 6d65 6e74 2e61         segment.a
+00004720: 6464 5f77 6f72 6473 2869 2c20 692b 312c  dd_words(i, i+1,
+00004730: 2069 6e70 6c61 6365 3d54 7275 6529 0d0a   inplace=True)..
+00004740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004750: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00004760: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00004770: 676d 656e 742e 776f 7264 735b 692b 315d  gment.words[i+1]
+00004780: 2e64 7572 6174 696f 6e20 3c20 7365 676d  .duration < segm
+00004790: 656e 742e 776f 7264 735b 692d 315d 2e64  ent.words[i-1].d
+000047a0: 7572 6174 696f 6e3a 0d0a 2020 2020 2020  uration:..      
+000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047c0: 2020 7365 676d 656e 742e 6164 645f 776f    segment.add_wo
+000047d0: 7264 7328 692d 312c 2069 2c20 696e 706c  rds(i-1, i, inpl
+000047e0: 6163 653d 5472 7565 290d 0a20 2020 2020  ace=True)..     
+000047f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00004800: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00004810: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004820: 676d 656e 742e 6164 645f 776f 7264 7328  gment.add_words(
+00004830: 692c 2069 2b31 2c20 696e 706c 6163 653d  i, i+1, inplace=
+00004840: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
+00004850: 2020 2020 2020 206d 6178 5f69 202d 3d20         max_i -= 
+00004860: 310d 0a20 2020 2020 2020 2072 6574 7572  1..        retur
+00004870: 6e20 7365 676d 656e 740d 0a0d 0a20 2020  n segment....   
+00004880: 2064 6566 205f 746f 5f72 6576 6572 7365   def _to_reverse
+00004890: 5f74 6578 7428 0d0a 2020 2020 2020 2020  _text(..        
+000048a0: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+000048b0: 2020 2020 2020 2070 7265 7065 6e64 5f70         prepend_p
+000048c0: 756e 6374 7561 7469 6f6e 733a 204f 7074  unctuations: Opt
+000048d0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000048e0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000048f0: 6170 7065 6e64 5f70 756e 6374 7561 7469  append_punctuati
+00004900: 6f6e 733a 204f 7074 696f 6e61 6c5b 7374  ons: Optional[st
+00004910: 725d 203d 204e 6f6e 652c 0d0a 2020 2020  r] = None,..    
+00004920: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+00004930: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
+00004940: 6120 636f 7079 2077 6974 6820 776f 7264  a copy with word
+00004950: 7320 7265 7665 7273 6564 206f 7264 6572  s reversed order
+00004960: 2070 6572 2073 6567 6d65 6e74 2e0d 0a20   per segment... 
+00004970: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00004980: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
+00004990: 6e28 2760 605f 746f 5f72 6576 6572 7365  n('``_to_reverse
+000049a0: 5f74 6578 7428 2960 6020 6973 2064 6570  _text()`` is dep
+000049b0: 7265 6361 7465 6420 616e 6420 7769 6c6c  recated and will
+000049c0: 2062 6520 7265 6d6f 7665 6420 696e 2066   be removed in f
+000049d0: 7574 7572 6520 7665 7273 696f 6e73 2e27  uture versions.'
+000049e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000049f0: 2020 2020 2020 2020 2063 6174 6567 6f72           categor
+00004a00: 793d 4465 7072 6563 6174 696f 6e57 6172  y=DeprecationWar
+00004a10: 6e69 6e67 2c20 7374 6163 6b6c 6576 656c  ning, stacklevel
+00004a20: 3d32 290d 0a20 2020 2020 2020 2070 7265  =2)..        pre
+00004a30: 7065 6e64 5f70 756e 6374 7561 7469 6f6e  pend_punctuation
+00004a40: 7320 3d20 6765 745f 7072 6570 656e 645f  s = get_prepend_
+00004a50: 7075 6e63 7475 6174 696f 6e73 2870 7265  punctuations(pre
+00004a60: 7065 6e64 5f70 756e 6374 7561 7469 6f6e  pend_punctuation
+00004a70: 7329 0d0a 2020 2020 2020 2020 6966 2070  s)..        if p
+00004a80: 7265 7065 6e64 5f70 756e 6374 7561 7469  repend_punctuati
+00004a90: 6f6e 7320 616e 6420 2720 2720 6e6f 7420  ons and ' ' not 
+00004aa0: 696e 2070 7265 7065 6e64 5f70 756e 6374  in prepend_punct
+00004ab0: 7561 7469 6f6e 733a 0d0a 2020 2020 2020  uations:..      
+00004ac0: 2020 2020 2020 7072 6570 656e 645f 7075        prepend_pu
+00004ad0: 6e63 7475 6174 696f 6e73 202b 3d20 2720  nctuations += ' 
+00004ae0: 270d 0a20 2020 2020 2020 2061 7070 656e  '..        appen
+00004af0: 645f 7075 6e63 7475 6174 696f 6e73 203d  d_punctuations =
+00004b00: 2067 6574 5f61 7070 656e 645f 7075 6e63   get_append_punc
+00004b10: 7475 6174 696f 6e73 2861 7070 656e 645f  tuations(append_
+00004b20: 7075 6e63 7475 6174 696f 6e73 290d 0a20  punctuations).. 
+00004b30: 2020 2020 2020 2073 656c 665f 636f 7079         self_copy
+00004b40: 203d 2073 656c 662e 636f 7079 2863 6f70   = self.copy(cop
+00004b50: 795f 776f 7264 733d 5472 7565 290d 0a20  y_words=True).. 
+00004b60: 2020 2020 2020 2068 6173 5f70 7265 7065         has_prepe
+00004b70: 6e64 203d 2062 6f6f 6c28 7072 6570 656e  nd = bool(prepen
+00004b80: 645f 7075 6e63 7475 6174 696f 6e73 290d  d_punctuations).
+00004b90: 0a20 2020 2020 2020 2068 6173 5f61 7070  .        has_app
+00004ba0: 656e 6420 3d20 626f 6f6c 2861 7070 656e  end = bool(appen
+00004bb0: 645f 7075 6e63 7475 6174 696f 6e73 290d  d_punctuations).
+00004bc0: 0a20 2020 2020 2020 2069 6620 6861 735f  .        if has_
+00004bd0: 7072 6570 656e 6420 6f72 2068 6173 5f61  prepend or has_a
+00004be0: 7070 656e 643a 0d0a 2020 2020 2020 2020  ppend:..        
+00004bf0: 2020 2020 776f 7264 5f6f 626a 7320 3d20      word_objs = 
+00004c00: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00004c10: 2020 2073 656c 665f 636f 7079 2e77 6f72     self_copy.wor
+00004c20: 6473 0d0a 2020 2020 2020 2020 2020 2020  ds..            
+00004c30: 2020 2020 6966 2073 656c 665f 636f 7079      if self_copy
+00004c40: 2e68 6173 5f77 6f72 6473 2065 6c73 650d  .has_words else.
+00004c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004c60: 205b 576f 7264 5469 6d69 6e67 2877 2c20   [WordTiming(w, 
+00004c70: 302c 2031 2c20 3029 2066 6f72 2077 2069  0, 1, 0) for w i
+00004c80: 6e20 7365 6c66 5f63 6f70 792e 7465 7874  n self_copy.text
+00004c90: 2e73 706c 6974 2827 2027 295d 0d0a 2020  .split(' ')]..  
+00004ca0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00004cb0: 2020 2020 2020 2020 2066 6f72 2077 6f72           for wor
+00004cc0: 6420 696e 2077 6f72 645f 6f62 6a73 3a0d  d in word_objs:.
+00004cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ce0: 206e 6577 5f61 7070 656e 6420 3d20 2727   new_append = ''
+00004cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004d00: 2020 6966 2068 6173 5f70 7265 7065 6e64    if has_prepend
+00004d10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004d20: 2020 2020 2020 2066 6f72 205f 2069 6e20         for _ in 
+00004d30: 7261 6e67 6528 6c65 6e28 776f 7264 2929  range(len(word))
+00004d40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004d50: 2020 2020 2020 2020 2020 2063 6861 7220             char 
+00004d60: 3d20 776f 7264 2e77 6f72 645b 305d 0d0a  = word.word[0]..
+00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d80: 2020 2020 2020 2020 6966 2063 6861 7220          if char 
+00004d90: 696e 2070 7265 7065 6e64 5f70 756e 6374  in prepend_punct
+00004da0: 7561 7469 6f6e 733a 0d0a 2020 2020 2020  uations:..      
 00004db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004dc0: 2020 2020 2077 6f72 642e 776f 7264 203d       word.word =
-00004dd0: 2077 6f72 642e 776f 7264 5b31 3a5d 0d0a   word.word[1:]..
+00004dc0: 2020 2020 2020 6e65 775f 6170 7065 6e64        new_append
+00004dd0: 202b 3d20 6368 6172 0d0a 2020 2020 2020   += char..      
 00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004df0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e10: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00004e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004e30: 2020 6e65 775f 7072 6570 656e 6420 3d20    new_prepend = 
-00004e40: 2727 0d0a 2020 2020 2020 2020 2020 2020  ''..            
-00004e50: 2020 2020 6966 2068 6173 5f61 7070 656e      if has_appen
-00004e60: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
-00004e70: 2020 2020 2020 2020 666f 7220 5f20 696e          for _ in
-00004e80: 2072 616e 6765 286c 656e 2877 6f72 6429   range(len(word)
-00004e90: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00004ea0: 2020 2020 2020 2020 2020 2020 6368 6172              char
-00004eb0: 203d 2077 6f72 642e 776f 7264 5b2d 315d   = word.word[-1]
-00004ec0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004ed0: 2020 2020 2020 2020 2020 6966 2063 6861            if cha
-00004ee0: 7220 696e 2061 7070 656e 645f 7075 6e63  r in append_punc
-00004ef0: 7475 6174 696f 6e73 3a0d 0a20 2020 2020  tuations:..     
-00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f10: 2020 2020 2020 206e 6577 5f70 7265 7065         new_prepe
-00004f20: 6e64 202b 3d20 6368 6172 0d0a 2020 2020  nd += char..    
+00004df0: 2020 2020 2020 776f 7264 2e77 6f72 6420        word.word 
+00004e00: 3d20 776f 7264 2e77 6f72 645b 313a 5d0d  = word.word[1:].
+00004e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004e20: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e40: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00004e50: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
+00004e60: 2020 206e 6577 5f70 7265 7065 6e64 203d     new_prepend =
+00004e70: 2027 270d 0a20 2020 2020 2020 2020 2020   ''..           
+00004e80: 2020 2020 2069 6620 6861 735f 6170 7065       if has_appe
+00004e90: 6e64 3a0d 0a20 2020 2020 2020 2020 2020  nd:..           
+00004ea0: 2020 2020 2020 2020 2066 6f72 205f 2069           for _ i
+00004eb0: 6e20 7261 6e67 6528 6c65 6e28 776f 7264  n range(len(word
+00004ec0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00004ed0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+00004ee0: 7220 3d20 776f 7264 2e77 6f72 645b 2d31  r = word.word[-1
+00004ef0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00004f00: 2020 2020 2020 2020 2020 2069 6620 6368             if ch
+00004f10: 6172 2069 6e20 6170 7065 6e64 5f70 756e  ar in append_pun
+00004f20: 6374 7561 7469 6f6e 733a 0d0a 2020 2020  ctuations:..    
 00004f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f40: 2020 2020 2020 2020 776f 7264 2e77 6f72          word.wor
-00004f50: 6420 3d20 776f 7264 2e77 6f72 645b 3a2d  d = word.word[:-
-00004f60: 315d 0d0a 2020 2020 2020 2020 2020 2020  1]..            
-00004f70: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00004f80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004f90: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00004fa0: 7265 616b 0d0a 2020 2020 2020 2020 2020  reak..          
-00004fb0: 2020 2020 2020 776f 7264 2e77 6f72 6420        word.word 
-00004fc0: 3d20 6627 7b6e 6577 5f70 7265 7065 6e64  = f'{new_prepend
-00004fd0: 7d7b 776f 7264 2e77 6f72 647d 7b6e 6577  }{word.word}{new
-00004fe0: 5f61 7070 656e 645b 3a3a 2d31 5d7d 270d  _append[::-1]}'.
-00004ff0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00005000: 665f 636f 7079 2e5f 6465 6661 756c 745f  f_copy._default_
-00005010: 7465 7874 203d 2027 272e 6a6f 696e 2877  text = ''.join(w
-00005020: 2e77 6f72 6420 666f 7220 7720 696e 2072  .word for w in r
-00005030: 6576 6572 7365 6428 776f 7264 5f6f 626a  eversed(word_obj
-00005040: 7329 290d 0a0d 0a20 2020 2020 2020 2072  s))....        r
-00005050: 6574 7572 6e20 7365 6c66 5f63 6f70 790d  eturn self_copy.
-00005060: 0a0d 0a20 2020 2064 6566 2074 6f5f 6469  ...    def to_di
-00005070: 6374 2873 656c 662c 2072 6576 6572 7365  ct(self, reverse
-00005080: 5f74 6578 743a 2055 6e69 6f6e 5b62 6f6f  _text: Union[boo
-00005090: 6c2c 2074 7570 6c65 5d20 3d20 4661 6c73  l, tuple] = Fals
-000050a0: 6529 3a0d 0a20 2020 2020 2020 2069 6620  e):..        if 
-000050b0: 7265 7665 7273 655f 7465 7874 3a0d 0a20  reverse_text:.. 
-000050c0: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
-000050d0: 6e67 732e 7761 726e 2827 6060 7265 7665  ngs.warn('``reve
-000050e0: 7273 655f 7465 7874 3d54 7275 6560 6020  rse_text=True`` 
-000050f0: 6973 2064 6570 7265 6361 7465 6420 616e  is deprecated an
-00005100: 6420 7769 6c6c 2062 6520 7265 6d6f 7665  d will be remove
-00005110: 6420 696e 2066 7574 7572 6520 7665 7273  d in future vers
-00005120: 696f 6e73 2e20 270d 0a20 2020 2020 2020  ions. '..       
-00005130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005140: 2020 2027 5254 4c20 7465 7874 2070 6c61     'RTL text pla
-00005150: 7962 6163 6b20 6973 7375 6573 2061 7265  yback issues are
-00005160: 2063 6175 7365 6420 6279 2074 6865 2076   caused by the v
-00005170: 6964 656f 2070 6c61 7965 7220 696e 636f  ideo player inco
-00005180: 7272 6563 746c 7920 7061 7273 696e 6720  rrectly parsing 
-00005190: 7461 6773 2027 0d0a 2020 2020 2020 2020  tags '..        
-000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051b0: 2020 2728 6e6f 7465 3a20 7461 6773 2063    '(note: tags c
-000051c0: 6f6d 6520 6672 6f6d 2060 6073 6567 6d65  ome from ``segme
-000051d0: 6e74 5f6c 6576 656c 3d54 7275 6520 2b20  nt_level=True + 
-000051e0: 776f 7264 5f6c 6576 656c 3d54 7275 6560  word_level=True`
-000051f0: 6029 2e27 290d 0a20 2020 2020 2020 2020  `).')..         
-00005200: 2020 2073 6567 6d65 6e74 203d 2073 656c     segment = sel
-00005210: 662e 5f74 6f5f 7265 7665 7273 655f 7465  f._to_reverse_te
-00005220: 7874 282a 2872 6576 6572 7365 5f74 6578  xt(*(reverse_tex
-00005230: 7420 6966 2072 6576 6572 7365 5f74 6578  t if reverse_tex
-00005240: 7420 656c 7365 205b 5d29 290d 0a20 2020  t else []))..   
-00005250: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00005260: 2020 2020 2020 2020 7365 676d 656e 7420          segment 
-00005270: 3d20 7365 6c66 0d0a 0d0a 2020 2020 2020  = self....      
-00005280: 2020 7365 675f 6469 6374 203d 2064 6963    seg_dict = dic
-00005290: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-000052a0: 7374 6172 743d 7365 676d 656e 742e 7374  start=segment.st
-000052b0: 6172 742c 0d0a 2020 2020 2020 2020 2020  art,..          
-000052c0: 2020 656e 643d 7365 676d 656e 742e 656e    end=segment.en
-000052d0: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-000052e0: 7465 7874 3d73 6567 6d65 6e74 2e74 6578  text=segment.tex
-000052f0: 742c 0d0a 2020 2020 2020 2020 2020 2020  t,..            
-00005300: 7365 656b 3d73 6567 6d65 6e74 2e73 6565  seek=segment.see
-00005310: 6b2c 0d0a 2020 2020 2020 2020 2020 2020  k,..            
-00005320: 746f 6b65 6e73 3d4e 6f6e 6520 6966 2073  tokens=None if s
-00005330: 6567 6d65 6e74 2e74 6f6b 656e 7320 6973  egment.tokens is
-00005340: 204e 6f6e 6520 656c 7365 2073 6567 6d65   None else segme
-00005350: 6e74 2e74 6f6b 656e 732e 636f 7079 2829  nt.tokens.copy()
-00005360: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
-00005370: 656d 7065 7261 7475 7265 3d73 6567 6d65  emperature=segme
-00005380: 6e74 2e74 656d 7065 7261 7475 7265 2c0d  nt.temperature,.
-00005390: 0a20 2020 2020 2020 2020 2020 2061 7667  .            avg
-000053a0: 5f6c 6f67 7072 6f62 3d73 6567 6d65 6e74  _logprob=segment
-000053b0: 2e61 7667 5f6c 6f67 7072 6f62 2c0d 0a20  .avg_logprob,.. 
-000053c0: 2020 2020 2020 2020 2020 2063 6f6d 7072             compr
-000053d0: 6573 7369 6f6e 5f72 6174 696f 3d73 6567  ession_ratio=seg
-000053e0: 6d65 6e74 2e63 6f6d 7072 6573 7369 6f6e  ment.compression
-000053f0: 5f72 6174 696f 2c0d 0a20 2020 2020 2020  _ratio,..       
-00005400: 2020 2020 206e 6f5f 7370 6565 6368 5f70       no_speech_p
-00005410: 726f 623d 7365 676d 656e 742e 6e6f 5f73  rob=segment.no_s
-00005420: 7065 6563 685f 7072 6f62 2c0d 0a20 2020  peech_prob,..   
-00005430: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
-00005440: 2020 6966 2073 6567 6d65 6e74 2e68 6173    if segment.has
-00005450: 5f77 6f72 6473 3a0d 0a20 2020 2020 2020  _words:..       
-00005460: 2020 2020 2073 6567 5f64 6963 745b 2777       seg_dict['w
-00005470: 6f72 6473 275d 203d 205b 772e 746f 5f64  ords'] = [w.to_d
-00005480: 6963 7428 2920 666f 7220 7720 696e 2073  ict() for w in s
-00005490: 6567 6d65 6e74 2e77 6f72 6473 5d0d 0a20  egment.words].. 
-000054a0: 2020 2020 2020 2065 6c69 6620 7365 676d         elif segm
-000054b0: 656e 742e 6f72 695f 6861 735f 776f 7264  ent.ori_has_word
-000054c0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000054d0: 7365 675f 6469 6374 5b27 776f 7264 7327  seg_dict['words'
-000054e0: 5d20 3d20 5b5d 0d0a 2020 2020 2020 2020  ] = []..        
-000054f0: 6966 2072 6576 6572 7365 5f74 6578 743a  if reverse_text:
-00005500: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00005510: 675f 6469 6374 5b27 7265 7665 7273 6564  g_dict['reversed
-00005520: 5f74 6578 7427 5d20 3d20 5472 7565 0d0a  _text'] = True..
-00005530: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00005540: 6567 5f64 6963 740d 0a0d 0a20 2020 2064  eg_dict....    d
-00005550: 6566 2077 6f72 6473 5f62 795f 6c6f 636b  ef words_by_lock
-00005560: 2873 656c 662c 206f 6e6c 795f 7465 7874  (self, only_text
-00005570: 3a20 626f 6f6c 203d 2054 7275 652c 2069  : bool = True, i
-00005580: 6e63 6c75 6465 5f73 696e 676c 653a 2062  nclude_single: b
-00005590: 6f6f 6c20 3d20 4661 6c73 6529 3a0d 0a20  ool = False):.. 
-000055a0: 2020 2020 2020 2072 6574 7572 6e20 5f77         return _w
-000055b0: 6f72 6473 5f62 795f 6c6f 636b 2873 656c  ords_by_lock(sel
-000055c0: 662e 776f 7264 732c 206f 6e6c 795f 7465  f.words, only_te
-000055d0: 7874 3d6f 6e6c 795f 7465 7874 2c20 696e  xt=only_text, in
-000055e0: 636c 7564 655f 7369 6e67 6c65 3d69 6e63  clude_single=inc
-000055f0: 6c75 6465 5f73 696e 676c 6529 0d0a 0d0a  lude_single)....
-00005600: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-00005610: 2020 2064 6566 206c 6566 745f 6c6f 636b     def left_lock
-00005620: 6564 2873 656c 6629 3a0d 0a20 2020 2020  ed(self):..     
-00005630: 2020 2069 6620 7365 6c66 2e68 6173 5f77     if self.has_w
-00005640: 6f72 6473 3a0d 0a20 2020 2020 2020 2020  ords:..         
-00005650: 2020 2072 6574 7572 6e20 7365 6c66 2e77     return self.w
-00005660: 6f72 6473 5b30 5d2e 6c65 6674 5f6c 6f63  ords[0].left_loc
-00005670: 6b65 640d 0a20 2020 2020 2020 2072 6574  ked..        ret
-00005680: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
-00005690: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-000056a0: 6465 6620 7269 6768 745f 6c6f 636b 6564  def right_locked
-000056b0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-000056c0: 2069 6620 7365 6c66 2e68 6173 5f77 6f72   if self.has_wor
-000056d0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-000056e0: 2072 6574 7572 6e20 7365 6c66 2e77 6f72   return self.wor
-000056f0: 6473 5b2d 315d 2e72 6967 6874 5f6c 6f63  ds[-1].right_loc
-00005700: 6b65 640d 0a20 2020 2020 2020 2072 6574  ked..        ret
-00005710: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
-00005720: 2064 6566 206c 6f63 6b5f 6c65 6674 2873   def lock_left(s
-00005730: 656c 6629 3a0d 0a20 2020 2020 2020 2069  elf):..        i
-00005740: 6620 7365 6c66 2e68 6173 5f77 6f72 6473  f self.has_words
-00005750: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00005760: 656c 662e 776f 7264 735b 305d 2e6c 6f63  elf.words[0].loc
-00005770: 6b5f 6c65 6674 2829 0d0a 0d0a 2020 2020  k_left()....    
-00005780: 6465 6620 6c6f 636b 5f72 6967 6874 2873  def lock_right(s
-00005790: 656c 6629 3a0d 0a20 2020 2020 2020 2069  elf):..        i
-000057a0: 6620 7365 6c66 2e68 6173 5f77 6f72 6473  f self.has_words
-000057b0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000057c0: 656c 662e 776f 7264 735b 2d31 5d2e 6c6f  elf.words[-1].lo
-000057d0: 636b 5f72 6967 6874 2829 0d0a 0d0a 2020  ck_right()....  
-000057e0: 2020 6465 6620 6c6f 636b 5f62 6f74 6828    def lock_both(
-000057f0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00005800: 7365 6c66 2e6c 6f63 6b5f 6c65 6674 2829  self.lock_left()
-00005810: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00005820: 6f63 6b5f 7269 6768 7428 290d 0a0d 0a20  ock_right().... 
-00005830: 2020 2064 6566 2075 6e6c 6f63 6b5f 616c     def unlock_al
-00005840: 6c5f 776f 7264 7328 7365 6c66 293a 0d0a  l_words(self):..
-00005850: 2020 2020 2020 2020 7365 6c66 2e5f 776f          self._wo
-00005860: 7264 5f6f 7065 7261 7469 6f6e 7328 2775  rd_operations('u
-00005870: 6e6c 6f63 6b5f 626f 7468 2729 0d0a 0d0a  nlock_both')....
-00005880: 2020 2020 6465 6620 7265 6173 7369 676e      def reassign
-00005890: 5f69 6473 2873 656c 662c 2073 7461 7274  _ids(self, start
-000058a0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-000058b0: 3d20 4e6f 6e65 293a 0d0a 2020 2020 2020  = None):..      
-000058c0: 2020 6966 2073 656c 662e 6861 735f 776f    if self.has_wo
-000058d0: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
-000058e0: 2020 666f 7220 692c 2077 6f72 6420 696e    for i, word in
-000058f0: 2065 6e75 6d65 7261 7465 2873 656c 662e   enumerate(self.
-00005900: 776f 7264 735b 7374 6172 743a 5d2c 2073  words[start:], s
-00005910: 7461 7274 206f 7220 3029 3a0d 0a20 2020  tart or 0):..   
-00005920: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
-00005930: 642e 7365 676d 656e 7420 3d20 7365 6c66  d.segment = self
-00005940: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005950: 2020 776f 7264 2e69 6420 3d20 690d 0a0d    word.id = i...
-00005960: 0a20 2020 2064 6566 2075 7064 6174 655f  .    def update_
-00005970: 7365 675f 7769 7468 5f77 6f72 6473 2873  seg_with_words(s
-00005980: 656c 6629 3a0d 0a20 2020 2020 2020 2077  elf):..        w
-00005990: 6172 6e69 6e67 732e 7761 726e 2827 4174  arnings.warn('At
-000059a0: 7472 6962 7574 6573 2074 6861 7420 7265  tributes that re
-000059b0: 7175 6972 6564 2075 7064 6174 696e 6720  quired updating 
-000059c0: 6172 6520 6e6f 7720 7072 6f70 6572 7469  are now properti
-000059d0: 6573 2062 6173 6564 206f 6e20 7468 6520  es based on the 
-000059e0: 6060 776f 7264 7360 6020 6578 6365 7074  ``words`` except
-000059f0: 2066 6f72 2060 6069 6460 602e 2027 0d0a   for ``id``. '..
-00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a10: 2020 2020 2020 2760 6075 7064 6174 655f        '``update_
-00005a20: 7365 675f 7769 7468 5f77 6f72 6473 2829  seg_with_words()
-00005a30: 6060 2069 7320 6465 7072 6563 6174 6564  `` is deprecated
-00005a40: 2061 6e64 2077 696c 6c20 6265 2072 656d   and will be rem
-00005a50: 6f76 6564 2069 6e20 6675 7475 7265 2076  oved in future v
-00005a60: 6572 7369 6f6e 732e 2027 0d0a 2020 2020  ersions. '..    
-00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a80: 2020 2755 7365 2060 602e 7265 6173 7369    'Use ``.reassi
-00005a90: 676e 5f69 6473 2829 6060 2074 6f20 6d61  gn_ids()`` to ma
-00005aa0: 6e75 616c 6c79 2075 7064 6174 6520 6964  nually update id
-00005ab0: 7327 2c0d 0a20 2020 2020 2020 2020 2020  s',..           
-00005ac0: 2020 2020 2020 2020 2020 2073 7461 636b             stack
-00005ad0: 6c65 7665 6c3d 3229 0d0a 2020 2020 2020  level=2)..      
-00005ae0: 2020 7365 6c66 2e72 6561 7373 6967 6e5f    self.reassign_
-00005af0: 6964 7328 290d 0a0d 0a20 2020 2064 6566  ids()....    def
-00005b00: 2073 7570 7072 6573 735f 7369 6c65 6e63   suppress_silenc
-00005b10: 6528 7365 6c66 2c0d 0a20 2020 2020 2020  e(self,..       
-00005b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b30: 2020 7369 6c65 6e74 5f73 7461 7274 733a    silent_starts:
-00005b40: 206e 702e 6e64 6172 7261 792c 0d0a 2020   np.ndarray,..  
+00004f40: 2020 2020 2020 2020 6e65 775f 7072 6570          new_prep
+00004f50: 656e 6420 2b3d 2063 6861 720d 0a20 2020  end += char..   
+00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f70: 2020 2020 2020 2020 2077 6f72 642e 776f           word.wo
+00004f80: 7264 203d 2077 6f72 642e 776f 7264 5b3a  rd = word.word[:
+00004f90: 2d31 5d0d 0a20 2020 2020 2020 2020 2020  -1]..           
+00004fa0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00004fb0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fd0: 6272 6561 6b0d 0a20 2020 2020 2020 2020  break..         
+00004fe0: 2020 2020 2020 2077 6f72 642e 776f 7264         word.word
+00004ff0: 203d 2066 277b 6e65 775f 7072 6570 656e   = f'{new_prepen
+00005000: 647d 7b77 6f72 642e 776f 7264 7d7b 6e65  d}{word.word}{ne
+00005010: 775f 6170 7065 6e64 5b3a 3a2d 315d 7d27  w_append[::-1]}'
+00005020: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00005030: 6c66 5f63 6f70 792e 5f64 6566 6175 6c74  lf_copy._default
+00005040: 5f74 6578 7420 3d20 2727 2e6a 6f69 6e28  _text = ''.join(
+00005050: 772e 776f 7264 2066 6f72 2077 2069 6e20  w.word for w in 
+00005060: 7265 7665 7273 6564 2877 6f72 645f 6f62  reversed(word_ob
+00005070: 6a73 2929 0d0a 0d0a 2020 2020 2020 2020  js))....        
+00005080: 7265 7475 726e 2073 656c 665f 636f 7079  return self_copy
+00005090: 0d0a 0d0a 2020 2020 6465 6620 746f 5f64  ....    def to_d
+000050a0: 6963 7428 7365 6c66 2c20 7265 7665 7273  ict(self, revers
+000050b0: 655f 7465 7874 3a20 556e 696f 6e5b 626f  e_text: Union[bo
+000050c0: 6f6c 2c20 7475 706c 655d 203d 2046 616c  ol, tuple] = Fal
+000050d0: 7365 293a 0d0a 2020 2020 2020 2020 6966  se):..        if
+000050e0: 2072 6576 6572 7365 5f74 6578 743a 0d0a   reverse_text:..
+000050f0: 2020 2020 2020 2020 2020 2020 7761 726e              warn
+00005100: 696e 6773 2e77 6172 6e28 2760 6072 6576  ings.warn('``rev
+00005110: 6572 7365 5f74 6578 743d 5472 7565 6060  erse_text=True``
+00005120: 2069 7320 6465 7072 6563 6174 6564 2061   is deprecated a
+00005130: 6e64 2077 696c 6c20 6265 2072 656d 6f76  nd will be remov
+00005140: 6564 2069 6e20 6675 7475 7265 2076 6572  ed in future ver
+00005150: 7369 6f6e 732e 2027 0d0a 2020 2020 2020  sions. '..      
+00005160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005170: 2020 2020 2752 544c 2074 6578 7420 706c      'RTL text pl
+00005180: 6179 6261 636b 2069 7373 7565 7320 6172  ayback issues ar
+00005190: 6520 6361 7573 6564 2062 7920 7468 6520  e caused by the 
+000051a0: 7669 6465 6f20 706c 6179 6572 2069 6e63  video player inc
+000051b0: 6f72 7265 6374 6c79 2070 6172 7369 6e67  orrectly parsing
+000051c0: 2074 6167 7320 270d 0a20 2020 2020 2020   tags '..       
+000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051e0: 2020 2027 286e 6f74 653a 2074 6167 7320     '(note: tags 
+000051f0: 636f 6d65 2066 726f 6d20 6060 7365 676d  come from ``segm
+00005200: 656e 745f 6c65 7665 6c3d 5472 7565 202b  ent_level=True +
+00005210: 2077 6f72 645f 6c65 7665 6c3d 5472 7565   word_level=True
+00005220: 6060 292e 2729 0d0a 2020 2020 2020 2020  ``).')..        
+00005230: 2020 2020 7365 676d 656e 7420 3d20 7365      segment = se
+00005240: 6c66 2e5f 746f 5f72 6576 6572 7365 5f74  lf._to_reverse_t
+00005250: 6578 7428 2a28 7265 7665 7273 655f 7465  ext(*(reverse_te
+00005260: 7874 2069 6620 7265 7665 7273 655f 7465  xt if reverse_te
+00005270: 7874 2065 6c73 6520 5b5d 2929 0d0a 2020  xt else []))..  
+00005280: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00005290: 2020 2020 2020 2020 2073 6567 6d65 6e74           segment
+000052a0: 203d 2073 656c 660d 0a0d 0a20 2020 2020   = self....     
+000052b0: 2020 2073 6567 5f64 6963 7420 3d20 6469     seg_dict = di
+000052c0: 6374 280d 0a20 2020 2020 2020 2020 2020  ct(..           
+000052d0: 2073 7461 7274 3d73 6567 6d65 6e74 2e73   start=segment.s
+000052e0: 7461 7274 2c0d 0a20 2020 2020 2020 2020  tart,..         
+000052f0: 2020 2065 6e64 3d73 6567 6d65 6e74 2e65     end=segment.e
+00005300: 6e64 2c0d 0a20 2020 2020 2020 2020 2020  nd,..           
+00005310: 2074 6578 743d 7365 676d 656e 742e 7465   text=segment.te
+00005320: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
+00005330: 2073 6565 6b3d 7365 676d 656e 742e 7365   seek=segment.se
+00005340: 656b 2c0d 0a20 2020 2020 2020 2020 2020  ek,..           
+00005350: 2074 6f6b 656e 733d 4e6f 6e65 2069 6620   tokens=None if 
+00005360: 7365 676d 656e 742e 746f 6b65 6e73 2069  segment.tokens i
+00005370: 7320 4e6f 6e65 2065 6c73 6520 7365 676d  s None else segm
+00005380: 656e 742e 746f 6b65 6e73 2e63 6f70 7928  ent.tokens.copy(
+00005390: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+000053a0: 7465 6d70 6572 6174 7572 653d 7365 676d  temperature=segm
+000053b0: 656e 742e 7465 6d70 6572 6174 7572 652c  ent.temperature,
+000053c0: 0d0a 2020 2020 2020 2020 2020 2020 6176  ..            av
+000053d0: 675f 6c6f 6770 726f 623d 7365 676d 656e  g_logprob=segmen
+000053e0: 742e 6176 675f 6c6f 6770 726f 622c 0d0a  t.avg_logprob,..
+000053f0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00005400: 7265 7373 696f 6e5f 7261 7469 6f3d 7365  ression_ratio=se
+00005410: 676d 656e 742e 636f 6d70 7265 7373 696f  gment.compressio
+00005420: 6e5f 7261 7469 6f2c 0d0a 2020 2020 2020  n_ratio,..      
+00005430: 2020 2020 2020 6e6f 5f73 7065 6563 685f        no_speech_
+00005440: 7072 6f62 3d73 6567 6d65 6e74 2e6e 6f5f  prob=segment.no_
+00005450: 7370 6565 6368 5f70 726f 622c 0d0a 2020  speech_prob,..  
+00005460: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+00005470: 2020 2069 6620 7365 676d 656e 742e 6861     if segment.ha
+00005480: 735f 776f 7264 733a 0d0a 2020 2020 2020  s_words:..      
+00005490: 2020 2020 2020 7365 675f 6469 6374 5b27        seg_dict['
+000054a0: 776f 7264 7327 5d20 3d20 5b77 2e74 6f5f  words'] = [w.to_
+000054b0: 6469 6374 2829 2066 6f72 2077 2069 6e20  dict() for w in 
+000054c0: 7365 676d 656e 742e 776f 7264 735d 0d0a  segment.words]..
+000054d0: 2020 2020 2020 2020 656c 6966 2073 6567          elif seg
+000054e0: 6d65 6e74 2e6f 7269 5f68 6173 5f77 6f72  ment.ori_has_wor
+000054f0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00005500: 2073 6567 5f64 6963 745b 2777 6f72 6473   seg_dict['words
+00005510: 275d 203d 205b 5d0d 0a20 2020 2020 2020  '] = []..       
+00005520: 2069 6620 7265 7665 7273 655f 7465 7874   if reverse_text
+00005530: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00005540: 6567 5f64 6963 745b 2772 6576 6572 7365  eg_dict['reverse
+00005550: 645f 7465 7874 275d 203d 2054 7275 650d  d_text'] = True.
+00005560: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00005570: 7365 675f 6469 6374 0d0a 0d0a 2020 2020  seg_dict....    
+00005580: 6465 6620 776f 7264 735f 6279 5f6c 6f63  def words_by_loc
+00005590: 6b28 7365 6c66 2c20 6f6e 6c79 5f74 6578  k(self, only_tex
+000055a0: 743a 2062 6f6f 6c20 3d20 5472 7565 2c20  t: bool = True, 
+000055b0: 696e 636c 7564 655f 7369 6e67 6c65 3a20  include_single: 
+000055c0: 626f 6f6c 203d 2046 616c 7365 293a 0d0a  bool = False):..
+000055d0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000055e0: 776f 7264 735f 6279 5f6c 6f63 6b28 7365  words_by_lock(se
+000055f0: 6c66 2e77 6f72 6473 2c20 6f6e 6c79 5f74  lf.words, only_t
+00005600: 6578 743d 6f6e 6c79 5f74 6578 742c 2069  ext=only_text, i
+00005610: 6e63 6c75 6465 5f73 696e 676c 653d 696e  nclude_single=in
+00005620: 636c 7564 655f 7369 6e67 6c65 290d 0a0d  clude_single)...
+00005630: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
+00005640: 2020 2020 6465 6620 6c65 6674 5f6c 6f63      def left_loc
+00005650: 6b65 6428 7365 6c66 293a 0d0a 2020 2020  ked(self):..    
+00005660: 2020 2020 6966 2073 656c 662e 6861 735f      if self.has_
+00005670: 776f 7264 733a 0d0a 2020 2020 2020 2020  words:..        
+00005680: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00005690: 776f 7264 735b 305d 2e6c 6566 745f 6c6f  words[0].left_lo
+000056a0: 636b 6564 0d0a 2020 2020 2020 2020 7265  cked..        re
+000056b0: 7475 726e 2046 616c 7365 0d0a 0d0a 2020  turn False....  
+000056c0: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+000056d0: 2064 6566 2072 6967 6874 5f6c 6f63 6b65   def right_locke
+000056e0: 6428 7365 6c66 293a 0d0a 2020 2020 2020  d(self):..      
+000056f0: 2020 6966 2073 656c 662e 6861 735f 776f    if self.has_wo
+00005700: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
+00005710: 2020 7265 7475 726e 2073 656c 662e 776f    return self.wo
+00005720: 7264 735b 2d31 5d2e 7269 6768 745f 6c6f  rds[-1].right_lo
+00005730: 636b 6564 0d0a 2020 2020 2020 2020 7265  cked..        re
+00005740: 7475 726e 2046 616c 7365 0d0a 0d0a 2020  turn False....  
+00005750: 2020 6465 6620 6c6f 636b 5f6c 6566 7428    def lock_left(
+00005760: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00005770: 6966 2073 656c 662e 6861 735f 776f 7264  if self.has_word
+00005780: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00005790: 7365 6c66 2e77 6f72 6473 5b30 5d2e 6c6f  self.words[0].lo
+000057a0: 636b 5f6c 6566 7428 290d 0a0d 0a20 2020  ck_left()....   
+000057b0: 2064 6566 206c 6f63 6b5f 7269 6768 7428   def lock_right(
+000057c0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000057d0: 6966 2073 656c 662e 6861 735f 776f 7264  if self.has_word
+000057e0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000057f0: 7365 6c66 2e77 6f72 6473 5b2d 315d 2e6c  self.words[-1].l
+00005800: 6f63 6b5f 7269 6768 7428 290d 0a0d 0a20  ock_right().... 
+00005810: 2020 2064 6566 206c 6f63 6b5f 626f 7468     def lock_both
+00005820: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00005830: 2073 656c 662e 6c6f 636b 5f6c 6566 7428   self.lock_left(
+00005840: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00005850: 6c6f 636b 5f72 6967 6874 2829 0d0a 0d0a  lock_right()....
+00005860: 2020 2020 6465 6620 756e 6c6f 636b 5f61      def unlock_a
+00005870: 6c6c 5f77 6f72 6473 2873 656c 6629 3a0d  ll_words(self):.
+00005880: 0a20 2020 2020 2020 2073 656c 662e 5f77  .        self._w
+00005890: 6f72 645f 6f70 6572 6174 696f 6e73 2827  ord_operations('
+000058a0: 756e 6c6f 636b 5f62 6f74 6827 290d 0a0d  unlock_both')...
+000058b0: 0a20 2020 2064 6566 2072 6561 7373 6967  .    def reassig
+000058c0: 6e5f 6964 7328 7365 6c66 2c20 7374 6172  n_ids(self, star
+000058d0: 743a 204f 7074 696f 6e61 6c5b 696e 745d  t: Optional[int]
+000058e0: 203d 204e 6f6e 6529 3a0d 0a20 2020 2020   = None):..     
+000058f0: 2020 2069 6620 7365 6c66 2e68 6173 5f77     if self.has_w
+00005900: 6f72 6473 3a0d 0a20 2020 2020 2020 2020  ords:..         
+00005910: 2020 2066 6f72 2069 2c20 776f 7264 2069     for i, word i
+00005920: 6e20 656e 756d 6572 6174 6528 7365 6c66  n enumerate(self
+00005930: 2e77 6f72 6473 5b73 7461 7274 3a5d 2c20  .words[start:], 
+00005940: 7374 6172 7420 6f72 2030 293a 0d0a 2020  start or 0):..  
+00005950: 2020 2020 2020 2020 2020 2020 2020 776f                wo
+00005960: 7264 2e73 6567 6d65 6e74 203d 2073 656c  rd.segment = sel
+00005970: 660d 0a20 2020 2020 2020 2020 2020 2020  f..             
+00005980: 2020 2077 6f72 642e 6964 203d 2069 0d0a     word.id = i..
+00005990: 0d0a 2020 2020 6465 6620 7570 6461 7465  ..    def update
+000059a0: 5f73 6567 5f77 6974 685f 776f 7264 7328  _seg_with_words(
+000059b0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000059c0: 7761 726e 696e 6773 2e77 6172 6e28 2741  warnings.warn('A
+000059d0: 7474 7269 6275 7465 7320 7468 6174 2072  ttributes that r
+000059e0: 6571 7569 7265 6420 7570 6461 7469 6e67  equired updating
+000059f0: 2061 7265 206e 6f77 2070 726f 7065 7274   are now propert
+00005a00: 6965 7320 6261 7365 6420 6f6e 2074 6865  ies based on the
+00005a10: 2060 6077 6f72 6473 6060 2065 7863 6570   ``words`` excep
+00005a20: 7420 666f 7220 6060 6964 6060 2e20 270d  t for ``id``. '.
+00005a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005a40: 2020 2020 2020 2027 6060 7570 6461 7465         '``update
+00005a50: 5f73 6567 5f77 6974 685f 776f 7264 7328  _seg_with_words(
+00005a60: 2960 6020 6973 2064 6570 7265 6361 7465  )`` is deprecate
+00005a70: 6420 616e 6420 7769 6c6c 2062 6520 7265  d and will be re
+00005a80: 6d6f 7665 6420 696e 2066 7574 7572 6520  moved in future 
+00005a90: 7665 7273 696f 6e73 2e20 270d 0a20 2020  versions. '..   
+00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ab0: 2020 2027 5573 6520 6060 2e72 6561 7373     'Use ``.reass
+00005ac0: 6967 6e5f 6964 7328 2960 6020 746f 206d  ign_ids()`` to m
+00005ad0: 616e 7561 6c6c 7920 7570 6461 7465 2069  anually update i
+00005ae0: 6473 272c 0d0a 2020 2020 2020 2020 2020  ds',..          
+00005af0: 2020 2020 2020 2020 2020 2020 7374 6163              stac
+00005b00: 6b6c 6576 656c 3d32 290d 0a20 2020 2020  klevel=2)..     
+00005b10: 2020 2073 656c 662e 7265 6173 7369 676e     self.reassign
+00005b20: 5f69 6473 2829 0d0a 0d0a 2020 2020 6465  _ids()....    de
+00005b30: 6620 7375 7070 7265 7373 5f73 696c 656e  f suppress_silen
+00005b40: 6365 2873 656c 662c 0d0a 2020 2020 2020  ce(self,..      
 00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b60: 2020 2020 2020 2073 696c 656e 745f 656e         silent_en
-00005b70: 6473 3a20 6e70 2e6e 6461 7272 6179 2c0d  ds: np.ndarray,.
-00005b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005b90: 2020 2020 2020 2020 2020 6d69 6e5f 776f            min_wo
-00005ba0: 7264 5f64 7572 3a20 4f70 7469 6f6e 616c  rd_dur: Optional
-00005bb0: 5b66 6c6f 6174 5d20 3d20 4e6f 6e65 2c0d  [float] = None,.
-00005bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005bd0: 2020 2020 2020 2020 2020 776f 7264 5f6c            word_l
-00005be0: 6576 656c 3a20 626f 6f6c 203d 2054 7275  evel: bool = Tru
-00005bf0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00005c00: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00005c10: 7370 6565 6368 5f65 7272 6f72 3a20 666c  speech_error: fl
-00005c20: 6f61 7420 3d20 302e 332c 0d0a 2020 2020  oat = 0.3,..    
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 2020 2020 2075 7365 5f77 6f72 645f 706f       use_word_po
-00005c50: 7369 7469 6f6e 3a20 626f 6f6c 203d 2054  sition: bool = T
-00005c60: 7275 6529 3a0d 0a20 2020 2020 2020 206d  rue):..        m
-00005c70: 696e 5f77 6f72 645f 6475 7220 3d20 6765  in_word_dur = ge
-00005c80: 745f 6d69 6e5f 776f 7264 5f64 7572 286d  t_min_word_dur(m
-00005c90: 696e 5f77 6f72 645f 6475 7229 0d0a 2020  in_word_dur)..  
-00005ca0: 2020 2020 2020 6966 2073 656c 662e 6861        if self.ha
-00005cb0: 735f 776f 7264 733a 0d0a 2020 2020 2020  s_words:..      
-00005cc0: 2020 2020 2020 656e 6469 6e67 5f70 756e        ending_pun
-00005cd0: 6374 7561 7469 6f6e 7320 3d20 6765 745f  ctuations = get_
-00005ce0: 6170 7065 6e64 5f70 756e 6374 7561 7469  append_punctuati
-00005cf0: 6f6e 7328 290d 0a20 2020 2020 2020 2020  ons()..         
-00005d00: 2020 2077 6f72 6473 203d 2073 656c 662e     words = self.
-00005d10: 776f 7264 7320 6966 2077 6f72 645f 6c65  words if word_le
-00005d20: 7665 6c20 6f72 206c 656e 2873 656c 662e  vel or len(self.
-00005d30: 776f 7264 7329 203d 3d20 3120 656c 7365  words) == 1 else
-00005d40: 205b 7365 6c66 2e77 6f72 6473 5b30 5d2c   [self.words[0],
-00005d50: 2073 656c 662e 776f 7264 735b 2d31 5d5d   self.words[-1]]
-00005d60: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00005d70: 7220 692c 2077 2069 6e20 656e 756d 6572  r i, w in enumer
-00005d80: 6174 6528 776f 7264 732c 2031 293a 0d0a  ate(words, 1):..
-00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005da0: 6966 2075 7365 5f77 6f72 645f 706f 7369  if use_word_posi
-00005db0: 7469 6f6e 3a0d 0a20 2020 2020 2020 2020  tion:..         
-00005dc0: 2020 2020 2020 2020 2020 206b 6565 705f             keep_
-00005dd0: 656e 6420 3d20 772e 776f 7264 5b2d 315d  end = w.word[-1]
-00005de0: 206e 6f74 2069 6e20 656e 6469 6e67 5f70   not in ending_p
-00005df0: 756e 6374 7561 7469 6f6e 730d 0a20 2020  unctuations..   
-00005e00: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00005e10: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00005e20: 2020 2020 2020 2020 6b65 6570 5f65 6e64          keep_end
-00005e30: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
-00005e40: 2020 2020 2020 2020 2077 2e73 7570 7072           w.suppr
-00005e50: 6573 735f 7369 6c65 6e63 6528 7369 6c65  ess_silence(sile
-00005e60: 6e74 5f73 7461 7274 732c 2073 696c 656e  nt_starts, silen
-00005e70: 745f 656e 6473 2c20 6d69 6e5f 776f 7264  t_ends, min_word
-00005e80: 5f64 7572 2c20 6e6f 6e73 7065 6563 685f  _dur, nonspeech_
-00005e90: 6572 726f 722c 206b 6565 705f 656e 6429  error, keep_end)
-00005ea0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00005eb0: 0a20 2020 2020 2020 2020 2020 2073 7570  .            sup
-00005ec0: 7072 6573 735f 7369 6c65 6e63 6528 7365  press_silence(se
-00005ed0: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
-00005ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ef0: 2020 7369 6c65 6e74 5f73 7461 7274 732c    silent_starts,
-00005f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005f10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005f20: 696c 656e 745f 656e 6473 2c0d 0a20 2020  ilent_ends,..   
-00005f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f40: 2020 2020 2020 2020 2020 6d69 6e5f 776f            min_wo
-00005f50: 7264 5f64 7572 2c0d 0a20 2020 2020 2020  rd_dur,..       
-00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f70: 2020 2020 2020 6e6f 6e73 7065 6563 685f        nonspeech_
-00005f80: 6572 726f 7229 0d0a 0d0a 2020 2020 2020  error)....      
-00005f90: 2020 7265 7475 726e 2073 656c 660d 0a0d    return self...
-00005fa0: 0a20 2020 2064 6566 2067 6574 5f6c 6f63  .    def get_loc
-00005fb0: 6b65 645f 696e 6469 6365 7328 7365 6c66  ked_indices(self
-00005fc0: 293a 0d0a 2020 2020 2020 2020 6c6f 636b  ):..        lock
-00005fd0: 6564 5f69 6e64 6963 6573 203d 205b 690d  ed_indices = [i.
-00005fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005ff0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00006000: 2c20 286c 6566 742c 2072 6967 6874 2920  , (left, right) 
-00006010: 696e 2065 6e75 6d65 7261 7465 287a 6970  in enumerate(zip
-00006020: 2873 656c 662e 776f 7264 735b 313a 5d2c  (self.words[1:],
-00006030: 2073 656c 662e 776f 7264 735b 3a2d 315d   self.words[:-1]
-00006040: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00006050: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00006060: 206c 6566 742e 6c65 6674 5f6c 6f63 6b65   left.left_locke
-00006070: 6420 6f72 2072 6967 6874 2e72 6967 6874  d or right.right
-00006080: 5f6c 6f63 6b65 645d 0d0a 2020 2020 2020  _locked]..      
-00006090: 2020 7265 7475 726e 206c 6f63 6b65 645f    return locked_
-000060a0: 696e 6469 6365 730d 0a0d 0a20 2020 2064  indices....    d
-000060b0: 6566 2067 6574 5f67 6170 7328 7365 6c66  ef get_gaps(self
-000060c0: 2c20 6173 5f6e 6461 7272 6179 3d46 616c  , as_ndarray=Fal
-000060d0: 7365 293a 0d0a 2020 2020 2020 2020 6966  se):..        if
-000060e0: 2073 656c 662e 6861 735f 776f 7264 733a   self.has_words:
-000060f0: 0d0a 2020 2020 2020 2020 2020 2020 735f  ..            s_
-00006100: 7473 203d 206e 702e 6172 7261 7928 5b77  ts = np.array([w
-00006110: 2e73 7461 7274 2066 6f72 2077 2069 6e20  .start for w in 
-00006120: 7365 6c66 2e77 6f72 6473 5d29 0d0a 2020  self.words])..  
-00006130: 2020 2020 2020 2020 2020 655f 7473 203d            e_ts =
-00006140: 206e 702e 6172 7261 7928 5b77 2e65 6e64   np.array([w.end
-00006150: 2066 6f72 2077 2069 6e20 7365 6c66 2e77   for w in self.w
-00006160: 6f72 6473 5d29 0d0a 2020 2020 2020 2020  ords])..        
-00006170: 2020 2020 6761 7020 3d20 735f 7473 5b31      gap = s_ts[1
-00006180: 3a5d 202d 2065 5f74 735b 3a2d 315d 0d0a  :] - e_ts[:-1]..
-00006190: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000061a0: 726e 2067 6170 2069 6620 6173 5f6e 6461  rn gap if as_nda
-000061b0: 7272 6179 2065 6c73 6520 6761 702e 746f  rray else gap.to
-000061c0: 6c69 7374 2829 0d0a 2020 2020 2020 2020  list()..        
-000061d0: 7265 7475 726e 205b 5d0d 0a0d 0a20 2020  return []....   
-000061e0: 2064 6566 2067 6574 5f67 6170 5f69 6e64   def get_gap_ind
-000061f0: 6963 6573 2873 656c 662c 206d 6178 5f67  ices(self, max_g
-00006200: 6170 3a20 666c 6f61 7420 3d20 302e 3129  ap: float = 0.1)
-00006210: 3a20 2023 2066 6f72 2073 706c 6974 7469  :  # for splitti
-00006220: 6e67 0d0a 2020 2020 2020 2020 6966 206e  ng..        if n
-00006230: 6f74 2073 656c 662e 6861 735f 776f 7264  ot self.has_word
-00006240: 7320 6f72 206c 656e 2873 656c 662e 776f  s or len(self.wo
-00006250: 7264 7329 203c 2032 3a0d 0a20 2020 2020  rds) < 2:..     
-00006260: 2020 2020 2020 2072 6574 7572 6e20 5b5d         return []
-00006270: 0d0a 2020 2020 2020 2020 6966 206d 6178  ..        if max
-00006280: 5f67 6170 2069 7320 4e6f 6e65 3a0d 0a20  _gap is None:.. 
-00006290: 2020 2020 2020 2020 2020 206d 6178 5f67             max_g
-000062a0: 6170 203d 2030 0d0a 2020 2020 2020 2020  ap = 0..        
-000062b0: 696e 6469 6365 7320 3d20 2873 656c 662e  indices = (self.
-000062c0: 6765 745f 6761 7073 2854 7275 6529 203e  get_gaps(True) >
-000062d0: 206d 6178 5f67 6170 292e 6e6f 6e7a 6572   max_gap).nonzer
-000062e0: 6f28 295b 305d 2e74 6f6c 6973 7428 290d  o()[0].tolist().
-000062f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006300: 736f 7274 6564 2873 6574 2869 6e64 6963  sorted(set(indic
-00006310: 6573 2920 2d20 7365 7428 7365 6c66 2e67  es) - set(self.g
-00006320: 6574 5f6c 6f63 6b65 645f 696e 6469 6365  et_locked_indice
-00006330: 7328 2929 290d 0a0d 0a20 2020 2064 6566  s()))....    def
-00006340: 2067 6574 5f70 756e 6374 7561 7469 6f6e   get_punctuation
-00006350: 5f69 6e64 6963 6573 2873 656c 662c 2070  _indices(self, p
-00006360: 756e 6374 7561 7469 6f6e 3a20 556e 696f  unctuation: Unio
-00006370: 6e5b 4c69 7374 5b73 7472 5d2c 204c 6973  n[List[str], Lis
-00006380: 745b 5475 706c 655b 7374 722c 2073 7472  t[Tuple[str, str
-00006390: 5d5d 2c20 7374 725d 293a 2020 2320 666f  ]], str]):  # fo
-000063a0: 7220 7370 6c69 7474 696e 670d 0a20 2020  r splitting..   
-000063b0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-000063c0: 2e68 6173 5f77 6f72 6473 206f 7220 6c65  .has_words or le
-000063d0: 6e28 7365 6c66 2e77 6f72 6473 2920 3c20  n(self.words) < 
-000063e0: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
-000063f0: 7265 7475 726e 205b 5d0d 0a20 2020 2020  return []..     
-00006400: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00006410: 2870 756e 6374 7561 7469 6f6e 2c20 7374  (punctuation, st
-00006420: 7229 3a0d 0a20 2020 2020 2020 2020 2020  r):..           
-00006430: 2070 756e 6374 7561 7469 6f6e 203d 205b   punctuation = [
-00006440: 7075 6e63 7475 6174 696f 6e5d 0d0a 2020  punctuation]..  
-00006450: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
-00006460: 5b5d 0d0a 2020 2020 2020 2020 666f 7220  []..        for 
-00006470: 7020 696e 2070 756e 6374 7561 7469 6f6e  p in punctuation
-00006480: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00006490: 6620 6973 696e 7374 616e 6365 2870 2c20  f isinstance(p, 
-000064a0: 7374 7229 3a0d 0a20 2020 2020 2020 2020  str):..         
-000064b0: 2020 2020 2020 2066 6f72 2069 2c20 7320         for i, s 
-000064c0: 696e 2065 6e75 6d65 7261 7465 2873 656c  in enumerate(sel
-000064d0: 662e 776f 7264 735b 3a2d 315d 293a 0d0a  f.words[:-1]):..
-000064e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064f0: 2020 2020 6966 2073 2e77 6f72 642e 656e      if s.word.en
-00006500: 6473 7769 7468 2870 293a 0d0a 2020 2020  dswith(p):..    
-00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006520: 2020 2020 696e 6469 6365 732e 6170 7065      indices.appe
-00006530: 6e64 2869 290d 0a20 2020 2020 2020 2020  nd(i)..         
-00006540: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00006550: 6920 213d 2030 2061 6e64 2073 2e77 6f72  i != 0 and s.wor
-00006560: 642e 7374 6172 7473 7769 7468 2870 293a  d.startswith(p):
-00006570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006580: 2020 2020 2020 2020 2020 696e 6469 6365            indice
-00006590: 732e 6170 7065 6e64 2869 2d31 290d 0a20  s.append(i-1).. 
-000065a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000065b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000065c0: 2020 656e 6469 6e67 2c20 6265 6769 6e6e    ending, beginn
-000065d0: 696e 6720 3d20 700d 0a20 2020 2020 2020  ing = p..       
-000065e0: 2020 2020 2020 2020 2069 6e64 6963 6573           indices
-000065f0: 2e65 7874 656e 6428 5b69 2066 6f72 2069  .extend([i for i
-00006600: 2c20 2877 302c 2077 3129 2069 6e20 656e  , (w0, w1) in en
-00006610: 756d 6572 6174 6528 7a69 7028 7365 6c66  umerate(zip(self
-00006620: 2e77 6f72 6473 5b3a 2d31 5d2c 2073 656c  .words[:-1], sel
-00006630: 662e 776f 7264 735b 313a 5d29 290d 0a20  f.words[1:])).. 
-00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006650: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00006660: 6620 7730 2e77 6f72 642e 656e 6473 7769  f w0.word.endswi
-00006670: 7468 2865 6e64 696e 6729 2061 6e64 2077  th(ending) and w
-00006680: 312e 776f 7264 2e73 7461 7274 7377 6974  1.word.startswit
-00006690: 6828 6265 6769 6e6e 696e 6729 5d29 0d0a  h(beginning)])..
-000066a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000066b0: 2073 6f72 7465 6428 7365 7428 696e 6469   sorted(set(indi
-000066c0: 6365 7329 202d 2073 6574 2873 656c 662e  ces) - set(self.
-000066d0: 6765 745f 6c6f 636b 6564 5f69 6e64 6963  get_locked_indic
-000066e0: 6573 2829 2929 0d0a 0d0a 2020 2020 6465  es()))....    de
-000066f0: 6620 6765 745f 6c65 6e67 7468 5f69 6e64  f get_length_ind
-00006700: 6963 6573 2873 656c 662c 206d 6178 5f63  ices(self, max_c
-00006710: 6861 7273 3a20 696e 7420 3d20 4e6f 6e65  hars: int = None
-00006720: 2c20 6d61 785f 776f 7264 733a 2069 6e74  , max_words: int
-00006730: 203d 204e 6f6e 652c 2065 7665 6e5f 7370   = None, even_sp
-00006740: 6c69 743a 2062 6f6f 6c20 3d20 5472 7565  lit: bool = True
-00006750: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00006760: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00006770: 636c 7564 655f 6c6f 636b 3a20 626f 6f6c  clude_lock: bool
-00006780: 203d 2046 616c 7365 293a 0d0a 2020 2020   = False):..    
-00006790: 2020 2020 2320 666f 7220 7370 6c69 7474      # for splitt
-000067a0: 696e 670d 0a20 2020 2020 2020 2069 6620  ing..        if 
-000067b0: 6e6f 7420 7365 6c66 2e68 6173 5f77 6f72  not self.has_wor
-000067c0: 6473 206f 7220 286d 6178 5f63 6861 7273  ds or (max_chars
-000067d0: 2069 7320 4e6f 6e65 2061 6e64 206d 6178   is None and max
-000067e0: 5f77 6f72 6473 2069 7320 4e6f 6e65 293a  _words is None):
-000067f0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00006800: 7475 726e 205b 5d0d 0a20 2020 2020 2020  turn []..       
-00006810: 2061 7373 6572 7420 6d61 785f 6368 6172   assert max_char
-00006820: 7320 213d 2030 2061 6e64 206d 6178 5f77  s != 0 and max_w
-00006830: 6f72 6473 2021 3d20 302c 205c 0d0a 2020  ords != 0, \..  
-00006840: 2020 2020 2020 2020 2020 6627 6d61 785f            f'max_
-00006850: 6368 6172 7320 616e 6420 6d61 785f 776f  chars and max_wo
-00006860: 7264 7320 6d75 7374 2062 6520 6772 6561  rds must be grea
-00006870: 7465 7220 302c 2062 7574 2067 6f74 207b  ter 0, but got {
-00006880: 6d61 785f 6368 6172 737d 2061 6e64 207b  max_chars} and {
-00006890: 6d61 785f 776f 7264 737d 270d 0a20 2020  max_words}'..   
-000068a0: 2020 2020 2069 6620 6c65 6e28 7365 6c66       if len(self
-000068b0: 2e77 6f72 6473 2920 3c20 323a 0d0a 2020  .words) < 2:..  
-000068c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000068d0: 205b 5d0d 0a20 2020 2020 2020 2069 6e64   []..        ind
-000068e0: 6963 6573 203d 205b 5d0d 0a20 2020 2020  ices = []..     
-000068f0: 2020 2069 6620 6576 656e 5f73 706c 6974     if even_split
-00006900: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
-00006910: 6861 725f 636f 756e 7420 3d20 2d31 2069  har_count = -1 i
-00006920: 6620 6d61 785f 6368 6172 7320 6973 204e  f max_chars is N
-00006930: 6f6e 6520 656c 7365 2073 756d 286d 6170  one else sum(map
-00006940: 286c 656e 2c20 7365 6c66 2e77 6f72 6473  (len, self.words
-00006950: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00006960: 776f 7264 5f63 6f75 6e74 203d 202d 3120  word_count = -1 
-00006970: 6966 206d 6178 5f77 6f72 6473 2069 7320  if max_words is 
-00006980: 4e6f 6e65 2065 6c73 6520 6c65 6e28 7365  None else len(se
-00006990: 6c66 2e77 6f72 6473 290d 0a20 2020 2020  lf.words)..     
-000069a0: 2020 2020 2020 2065 7863 6565 645f 6368         exceed_ch
-000069b0: 6172 7320 3d20 6d61 785f 6368 6172 7320  ars = max_chars 
-000069c0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-000069d0: 6368 6172 5f63 6f75 6e74 203e 206d 6178  char_count > max
-000069e0: 5f63 6861 7273 0d0a 2020 2020 2020 2020  _chars..        
-000069f0: 2020 2020 6578 6365 6564 5f77 6f72 6473      exceed_words
-00006a00: 203d 206d 6178 5f77 6f72 6473 2069 7320   = max_words is 
-00006a10: 6e6f 7420 4e6f 6e65 2061 6e64 2077 6f72  not None and wor
-00006a20: 645f 636f 756e 7420 3e20 6d61 785f 776f  d_count > max_wo
-00006a30: 7264 730d 0a20 2020 2020 2020 2020 2020  rds..           
-00006a40: 2069 6620 6578 6365 6564 5f63 6861 7273   if exceed_chars
-00006a50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00006a60: 2020 2073 706c 6974 7320 3d20 6e70 2e63     splits = np.c
-00006a70: 6569 6c28 6368 6172 5f63 6f75 6e74 202f  eil(char_count /
-00006a80: 206d 6178 5f63 6861 7273 290d 0a20 2020   max_chars)..   
-00006a90: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00006aa0: 7273 5f70 6572 5f73 706c 6974 203d 2063  rs_per_split = c
-00006ab0: 6861 725f 636f 756e 7420 2f20 7370 6c69  har_count / spli
-00006ac0: 7473 0d0a 2020 2020 2020 2020 2020 2020  ts..            
-00006ad0: 2020 2020 6375 6d5f 6368 6172 5f63 6f75      cum_char_cou
-00006ae0: 6e74 203d 206e 702e 6375 6d73 756d 285b  nt = np.cumsum([
-00006af0: 6c65 6e28 772e 776f 7264 2920 666f 7220  len(w.word) for 
-00006b00: 7720 696e 2073 656c 662e 776f 7264 735b  w in self.words[
-00006b10: 3a2d 315d 5d29 0d0a 2020 2020 2020 2020  :-1]])..        
-00006b20: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
-00006b30: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
-00006b40: 2020 2020 2020 2020 2028 6e70 2e61 6273           (np.abs
-00006b50: 2863 756d 5f63 6861 725f 636f 756e 742d  (cum_char_count-
-00006b60: 2869 2a63 6861 7273 5f70 6572 5f73 706c  (i*chars_per_spl
-00006b70: 6974 2929 292e 6172 676d 696e 2829 0d0a  it))).argmin()..
-00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b90: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00006ba0: 6765 2831 2c20 696e 7428 7370 6c69 7473  ge(1, int(splits
-00006bb0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00006bc0: 2020 2020 5d0d 0a20 2020 2020 2020 2020      ]..         
-00006bd0: 2020 2020 2020 2069 6620 6d61 785f 776f         if max_wo
-00006be0: 7264 7320 6973 206e 6f74 204e 6f6e 653a  rds is not None:
-00006bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006c00: 2020 2020 2020 6578 6365 6564 5f77 6f72        exceed_wor
-00006c10: 6473 203d 2061 6e79 286a 2d69 2b31 203e  ds = any(j-i+1 >
-00006c20: 206d 6178 5f77 6f72 6473 2066 6f72 2069   max_words for i
-00006c30: 2c20 6a20 696e 207a 6970 285b 305d 2b69  , j in zip([0]+i
-00006c40: 6e64 6963 6573 2c20 696e 6469 6365 732b  ndices, indices+
-00006c50: 5b6c 656e 2873 656c 662e 776f 7264 7329  [len(self.words)
-00006c60: 5d29 290d 0a0d 0a20 2020 2020 2020 2020  ]))....         
-00006c70: 2020 2069 6620 6578 6365 6564 5f77 6f72     if exceed_wor
-00006c80: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-00006c90: 2020 2020 2073 706c 6974 7320 3d20 6e70       splits = np
-00006ca0: 2e63 6569 6c28 776f 7264 5f63 6f75 6e74  .ceil(word_count
-00006cb0: 202f 206d 6178 5f77 6f72 6473 290d 0a20   / max_words).. 
-00006cc0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00006cd0: 6f72 6473 5f70 6572 5f73 706c 6974 203d  ords_per_split =
-00006ce0: 2077 6f72 645f 636f 756e 7420 2f20 7370   word_count / sp
-00006cf0: 6c69 7473 0d0a 2020 2020 2020 2020 2020  lits..          
-00006d00: 2020 2020 2020 6375 6d5f 776f 7264 5f63        cum_word_c
-00006d10: 6f75 6e74 203d 206e 702e 6172 7261 7928  ount = np.array(
-00006d20: 7261 6e67 6528 312c 206c 656e 2873 656c  range(1, len(sel
-00006d30: 662e 776f 7264 7329 2b31 2929 0d0a 2020  f.words)+1))..  
-00006d40: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00006d50: 6469 6365 7320 3d20 5b0d 0a20 2020 2020  dices = [..     
-00006d60: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00006d70: 702e 6162 7328 6375 6d5f 776f 7264 5f63  p.abs(cum_word_c
-00006d80: 6f75 6e74 2d28 692a 776f 7264 735f 7065  ount-(i*words_pe
-00006d90: 725f 7370 6c69 7429 292e 6172 676d 696e  r_split)).argmin
-00006da0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00006db0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00006dc0: 2072 616e 6765 2831 2c20 696e 7428 7370   range(1, int(sp
-00006dd0: 6c69 7473 2929 0d0a 2020 2020 2020 2020  lits))..        
-00006de0: 2020 2020 2020 2020 5d0d 0a0d 0a20 2020          ]....   
-00006df0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00006e00: 2020 2020 2020 2020 6375 7272 5f77 6f72          curr_wor
-00006e10: 6473 203d 2030 0d0a 2020 2020 2020 2020  ds = 0..        
-00006e20: 2020 2020 6375 7272 5f63 6861 7273 203d      curr_chars =
-00006e30: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
-00006e40: 6c6f 636b 6564 5f69 6e64 6963 6573 203d  locked_indices =
-00006e50: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00006e60: 2069 6620 696e 636c 7564 655f 6c6f 636b   if include_lock
-00006e70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00006e80: 2020 206c 6f63 6b65 645f 696e 6469 6365     locked_indice
-00006e90: 7320 3d20 7365 6c66 2e67 6574 5f6c 6f63  s = self.get_loc
-00006ea0: 6b65 645f 696e 6469 6365 7328 290d 0a20  ked_indices().. 
-00006eb0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00006ec0: 2c20 776f 7264 2069 6e20 656e 756d 6572  , word in enumer
-00006ed0: 6174 6528 7365 6c66 2e77 6f72 6473 293a  ate(self.words):
-00006ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006ef0: 2020 6375 7272 5f77 6f72 6473 202b 3d20    curr_words += 
-00006f00: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
-00006f10: 2020 2063 7572 725f 6368 6172 7320 2b3d     curr_chars +=
-00006f20: 206c 656e 2877 6f72 6429 0d0a 2020 2020   len(word)..    
-00006f30: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00006f40: 2021 3d20 303a 0d0a 2020 2020 2020 2020   != 0:..        
-00006f50: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00006f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006f70: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00006f80: 785f 6368 6172 7320 6973 206e 6f74 204e  x_chars is not N
-00006f90: 6f6e 6520 616e 6420 6375 7272 5f63 6861  one and curr_cha
-00006fa0: 7273 203e 206d 6178 5f63 6861 7273 0d0a  rs > max_chars..
+00005b60: 2020 2073 696c 656e 745f 7374 6172 7473     silent_starts
+00005b70: 3a20 6e70 2e6e 6461 7272 6179 2c0d 0a20  : np.ndarray,.. 
+00005b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b90: 2020 2020 2020 2020 7369 6c65 6e74 5f65          silent_e
+00005ba0: 6e64 733a 206e 702e 6e64 6172 7261 792c  nds: np.ndarray,
+00005bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005bc0: 2020 2020 2020 2020 2020 206d 696e 5f77             min_w
+00005bd0: 6f72 645f 6475 723a 204f 7074 696f 6e61  ord_dur: Optiona
+00005be0: 6c5b 666c 6f61 745d 203d 204e 6f6e 652c  l[float] = None,
+00005bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005c00: 2020 2020 2020 2020 2020 2077 6f72 645f             word_
+00005c10: 6c65 7665 6c3a 2062 6f6f 6c20 3d20 5472  level: bool = Tr
+00005c20: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00005c30: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00005c40: 6e73 7065 6563 685f 6572 726f 723a 2066  nspeech_error: f
+00005c50: 6c6f 6174 203d 2030 2e33 2c0d 0a20 2020  loat = 0.3,..   
+00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c70: 2020 2020 2020 7573 655f 776f 7264 5f70        use_word_p
+00005c80: 6f73 6974 696f 6e3a 2062 6f6f 6c20 3d20  osition: bool = 
+00005c90: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
+00005ca0: 6d69 6e5f 776f 7264 5f64 7572 203d 2067  min_word_dur = g
+00005cb0: 6574 5f6d 696e 5f77 6f72 645f 6475 7228  et_min_word_dur(
+00005cc0: 6d69 6e5f 776f 7264 5f64 7572 290d 0a20  min_word_dur).. 
+00005cd0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+00005ce0: 6173 5f77 6f72 6473 3a0d 0a20 2020 2020  as_words:..     
+00005cf0: 2020 2020 2020 2065 6e64 696e 675f 7075         ending_pu
+00005d00: 6e63 7475 6174 696f 6e73 203d 2067 6574  nctuations = get
+00005d10: 5f61 7070 656e 645f 7075 6e63 7475 6174  _append_punctuat
+00005d20: 696f 6e73 2829 0d0a 2020 2020 2020 2020  ions()..        
+00005d30: 2020 2020 776f 7264 7320 3d20 7365 6c66      words = self
+00005d40: 2e77 6f72 6473 2069 6620 776f 7264 5f6c  .words if word_l
+00005d50: 6576 656c 206f 7220 6c65 6e28 7365 6c66  evel or len(self
+00005d60: 2e77 6f72 6473 2920 3d3d 2031 2065 6c73  .words) == 1 els
+00005d70: 6520 5b73 656c 662e 776f 7264 735b 305d  e [self.words[0]
+00005d80: 2c20 7365 6c66 2e77 6f72 6473 5b2d 315d  , self.words[-1]
+00005d90: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
+00005da0: 6f72 2069 2c20 7720 696e 2065 6e75 6d65  or i, w in enume
+00005db0: 7261 7465 2877 6f72 6473 2c20 3129 3a0d  rate(words, 1):.
+00005dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005dd0: 2069 6620 7573 655f 776f 7264 5f70 6f73   if use_word_pos
+00005de0: 6974 696f 6e3a 0d0a 2020 2020 2020 2020  ition:..        
+00005df0: 2020 2020 2020 2020 2020 2020 6b65 6570              keep
+00005e00: 5f65 6e64 203d 206e 6f74 2028 772e 776f  _end = not (w.wo
+00005e10: 7264 5b2d 315d 2069 6e20 656e 6469 6e67  rd[-1] in ending
+00005e20: 5f70 756e 6374 7561 7469 6f6e 7320 6f72  _punctuations or
+00005e30: 2069 203d 3d20 6c65 6e28 776f 7264 7329   i == len(words)
+00005e40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00005e50: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00005e60: 2020 2020 2020 2020 2020 2020 2020 6b65                ke
+00005e70: 6570 5f65 6e64 203d 204e 6f6e 650d 0a20  ep_end = None.. 
+00005e80: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00005e90: 2e73 7570 7072 6573 735f 7369 6c65 6e63  .suppress_silenc
+00005ea0: 6528 7369 6c65 6e74 5f73 7461 7274 732c  e(silent_starts,
+00005eb0: 2073 696c 656e 745f 656e 6473 2c20 6d69   silent_ends, mi
+00005ec0: 6e5f 776f 7264 5f64 7572 2c20 6e6f 6e73  n_word_dur, nons
+00005ed0: 7065 6563 685f 6572 726f 722c 206b 6565  peech_error, kee
+00005ee0: 705f 656e 6429 0d0a 2020 2020 2020 2020  p_end)..        
+00005ef0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00005f00: 2020 2073 7570 7072 6573 735f 7369 6c65     suppress_sile
+00005f10: 6e63 6528 7365 6c66 2c0d 0a20 2020 2020  nce(self,..     
+00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f30: 2020 2020 2020 2020 7369 6c65 6e74 5f73          silent_s
+00005f40: 7461 7274 732c 0d0a 2020 2020 2020 2020  tarts,..        
+00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f60: 2020 2020 2073 696c 656e 745f 656e 6473       silent_ends
+00005f70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f90: 6d69 6e5f 776f 7264 5f64 7572 2c0d 0a20  min_word_dur,.. 
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fb0: 2020 2020 2020 2020 2020 2020 6e6f 6e73              nons
+00005fc0: 7065 6563 685f 6572 726f 7229 0d0a 0d0a  peech_error)....
+00005fd0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00005fe0: 656c 660d 0a0d 0a20 2020 2064 6566 2067  elf....    def g
+00005ff0: 6574 5f6c 6f63 6b65 645f 696e 6469 6365  et_locked_indice
+00006000: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
+00006010: 2020 6c6f 636b 6564 5f69 6e64 6963 6573    locked_indices
+00006020: 203d 205b 690d 0a20 2020 2020 2020 2020   = [i..         
+00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006040: 2066 6f72 2069 2c20 286c 6566 742c 2072   for i, (left, r
+00006050: 6967 6874 2920 696e 2065 6e75 6d65 7261  ight) in enumera
+00006060: 7465 287a 6970 2873 656c 662e 776f 7264  te(zip(self.word
+00006070: 735b 313a 5d2c 2073 656c 662e 776f 7264  s[1:], self.word
+00006080: 735b 3a2d 315d 2929 0d0a 2020 2020 2020  s[:-1]))..      
+00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060a0: 2020 2020 6966 206c 6566 742e 6c65 6674      if left.left
+000060b0: 5f6c 6f63 6b65 6420 6f72 2072 6967 6874  _locked or right
+000060c0: 2e72 6967 6874 5f6c 6f63 6b65 645d 0d0a  .right_locked]..
+000060d0: 2020 2020 2020 2020 7265 7475 726e 206c          return l
+000060e0: 6f63 6b65 645f 696e 6469 6365 730d 0a0d  ocked_indices...
+000060f0: 0a20 2020 2064 6566 2067 6574 5f67 6170  .    def get_gap
+00006100: 7328 7365 6c66 2c20 6173 5f6e 6461 7272  s(self, as_ndarr
+00006110: 6179 3d46 616c 7365 293a 0d0a 2020 2020  ay=False):..    
+00006120: 2020 2020 6966 2073 656c 662e 6861 735f      if self.has_
+00006130: 776f 7264 733a 0d0a 2020 2020 2020 2020  words:..        
+00006140: 2020 2020 735f 7473 203d 206e 702e 6172      s_ts = np.ar
+00006150: 7261 7928 5b77 2e73 7461 7274 2066 6f72  ray([w.start for
+00006160: 2077 2069 6e20 7365 6c66 2e77 6f72 6473   w in self.words
+00006170: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00006180: 655f 7473 203d 206e 702e 6172 7261 7928  e_ts = np.array(
+00006190: 5b77 2e65 6e64 2066 6f72 2077 2069 6e20  [w.end for w in 
+000061a0: 7365 6c66 2e77 6f72 6473 5d29 0d0a 2020  self.words])..  
+000061b0: 2020 2020 2020 2020 2020 6761 7020 3d20            gap = 
+000061c0: 735f 7473 5b31 3a5d 202d 2065 5f74 735b  s_ts[1:] - e_ts[
+000061d0: 3a2d 315d 0d0a 2020 2020 2020 2020 2020  :-1]..          
+000061e0: 2020 7265 7475 726e 2067 6170 2069 6620    return gap if 
+000061f0: 6173 5f6e 6461 7272 6179 2065 6c73 6520  as_ndarray else 
+00006200: 6761 702e 746f 6c69 7374 2829 0d0a 2020  gap.tolist()..  
+00006210: 2020 2020 2020 7265 7475 726e 205b 5d0d        return [].
+00006220: 0a0d 0a20 2020 2064 6566 2067 6574 5f67  ...    def get_g
+00006230: 6170 5f69 6e64 6963 6573 2873 656c 662c  ap_indices(self,
+00006240: 206d 6178 5f67 6170 3a20 666c 6f61 7420   max_gap: float 
+00006250: 3d20 302e 3129 3a20 2023 2066 6f72 2073  = 0.1):  # for s
+00006260: 706c 6974 7469 6e67 0d0a 2020 2020 2020  plitting..      
+00006270: 2020 6966 206e 6f74 2073 656c 662e 6861    if not self.ha
+00006280: 735f 776f 7264 7320 6f72 206c 656e 2873  s_words or len(s
+00006290: 656c 662e 776f 7264 7329 203c 2032 3a0d  elf.words) < 2:.
+000062a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000062b0: 7572 6e20 5b5d 0d0a 2020 2020 2020 2020  urn []..        
+000062c0: 6966 206d 6178 5f67 6170 2069 7320 4e6f  if max_gap is No
+000062d0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+000062e0: 206d 6178 5f67 6170 203d 2030 0d0a 2020   max_gap = 0..  
+000062f0: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
+00006300: 2873 656c 662e 6765 745f 6761 7073 2854  (self.get_gaps(T
+00006310: 7275 6529 203e 206d 6178 5f67 6170 292e  rue) > max_gap).
+00006320: 6e6f 6e7a 6572 6f28 295b 305d 2e74 6f6c  nonzero()[0].tol
+00006330: 6973 7428 290d 0a20 2020 2020 2020 2072  ist()..        r
+00006340: 6574 7572 6e20 736f 7274 6564 2873 6574  eturn sorted(set
+00006350: 2869 6e64 6963 6573 2920 2d20 7365 7428  (indices) - set(
+00006360: 7365 6c66 2e67 6574 5f6c 6f63 6b65 645f  self.get_locked_
+00006370: 696e 6469 6365 7328 2929 290d 0a0d 0a20  indices())).... 
+00006380: 2020 2064 6566 2067 6574 5f70 756e 6374     def get_punct
+00006390: 7561 7469 6f6e 5f69 6e64 6963 6573 2873  uation_indices(s
+000063a0: 656c 662c 2070 756e 6374 7561 7469 6f6e  elf, punctuation
+000063b0: 3a20 556e 696f 6e5b 4c69 7374 5b73 7472  : Union[List[str
+000063c0: 5d2c 204c 6973 745b 5475 706c 655b 7374  ], List[Tuple[st
+000063d0: 722c 2073 7472 5d5d 2c20 7374 725d 293a  r, str]], str]):
+000063e0: 2020 2320 666f 7220 7370 6c69 7474 696e    # for splittin
+000063f0: 670d 0a20 2020 2020 2020 2069 6620 6e6f  g..        if no
+00006400: 7420 7365 6c66 2e68 6173 5f77 6f72 6473  t self.has_words
+00006410: 206f 7220 6c65 6e28 7365 6c66 2e77 6f72   or len(self.wor
+00006420: 6473 2920 3c20 323a 0d0a 2020 2020 2020  ds) < 2:..      
+00006430: 2020 2020 2020 7265 7475 726e 205b 5d0d        return [].
+00006440: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00006450: 7374 616e 6365 2870 756e 6374 7561 7469  stance(punctuati
+00006460: 6f6e 2c20 7374 7229 3a0d 0a20 2020 2020  on, str):..     
+00006470: 2020 2020 2020 2070 756e 6374 7561 7469         punctuati
+00006480: 6f6e 203d 205b 7075 6e63 7475 6174 696f  on = [punctuatio
+00006490: 6e5d 0d0a 2020 2020 2020 2020 696e 6469  n]..        indi
+000064a0: 6365 7320 3d20 5b5d 0d0a 2020 2020 2020  ces = []..      
+000064b0: 2020 666f 7220 7020 696e 2070 756e 6374    for p in punct
+000064c0: 7561 7469 6f6e 3a0d 0a20 2020 2020 2020  uation:..       
+000064d0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+000064e0: 6365 2870 2c20 7374 7229 3a0d 0a20 2020  ce(p, str):..   
+000064f0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00006500: 2069 2c20 7320 696e 2065 6e75 6d65 7261   i, s in enumera
+00006510: 7465 2873 656c 662e 776f 7264 735b 3a2d  te(self.words[:-
+00006520: 315d 293a 0d0a 2020 2020 2020 2020 2020  1]):..          
+00006530: 2020 2020 2020 2020 2020 6966 2073 2e77            if s.w
+00006540: 6f72 642e 656e 6473 7769 7468 2870 293a  ord.endswith(p):
+00006550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006560: 2020 2020 2020 2020 2020 696e 6469 6365            indice
+00006570: 732e 6170 7065 6e64 2869 290d 0a20 2020  s.append(i)..   
+00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006590: 2065 6c69 6620 6920 213d 2030 2061 6e64   elif i != 0 and
+000065a0: 2073 2e77 6f72 642e 7374 6172 7473 7769   s.word.startswi
+000065b0: 7468 2870 293a 0d0a 2020 2020 2020 2020  th(p):..        
+000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065d0: 696e 6469 6365 732e 6170 7065 6e64 2869  indices.append(i
+000065e0: 2d31 290d 0a20 2020 2020 2020 2020 2020  -1)..           
+000065f0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00006600: 2020 2020 2020 2020 656e 6469 6e67 2c20          ending, 
+00006610: 6265 6769 6e6e 696e 6720 3d20 700d 0a20  beginning = p.. 
+00006620: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00006630: 6e64 6963 6573 2e65 7874 656e 6428 5b69  ndices.extend([i
+00006640: 2066 6f72 2069 2c20 2877 302c 2077 3129   for i, (w0, w1)
+00006650: 2069 6e20 656e 756d 6572 6174 6528 7a69   in enumerate(zi
+00006660: 7028 7365 6c66 2e77 6f72 6473 5b3a 2d31  p(self.words[:-1
+00006670: 5d2c 2073 656c 662e 776f 7264 735b 313a  ], self.words[1:
+00006680: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
+00006690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066a0: 2020 2020 2069 6620 7730 2e77 6f72 642e       if w0.word.
+000066b0: 656e 6473 7769 7468 2865 6e64 696e 6729  endswith(ending)
+000066c0: 2061 6e64 2077 312e 776f 7264 2e73 7461   and w1.word.sta
+000066d0: 7274 7377 6974 6828 6265 6769 6e6e 696e  rtswith(beginnin
+000066e0: 6729 5d29 0d0a 0d0a 2020 2020 2020 2020  g)])....        
+000066f0: 7265 7475 726e 2073 6f72 7465 6428 7365  return sorted(se
+00006700: 7428 696e 6469 6365 7329 202d 2073 6574  t(indices) - set
+00006710: 2873 656c 662e 6765 745f 6c6f 636b 6564  (self.get_locked
+00006720: 5f69 6e64 6963 6573 2829 2929 0d0a 0d0a  _indices()))....
+00006730: 2020 2020 6465 6620 6765 745f 6c65 6e67      def get_leng
+00006740: 7468 5f69 6e64 6963 6573 2873 656c 662c  th_indices(self,
+00006750: 206d 6178 5f63 6861 7273 3a20 696e 7420   max_chars: int 
+00006760: 3d20 4e6f 6e65 2c20 6d61 785f 776f 7264  = None, max_word
+00006770: 733a 2069 6e74 203d 204e 6f6e 652c 2065  s: int = None, e
+00006780: 7665 6e5f 7370 6c69 743a 2062 6f6f 6c20  ven_split: bool 
+00006790: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
+000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067b0: 2020 2020 696e 636c 7564 655f 6c6f 636b      include_lock
+000067c0: 3a20 626f 6f6c 203d 2046 616c 7365 293a  : bool = False):
+000067d0: 0d0a 2020 2020 2020 2020 2320 666f 7220  ..        # for 
+000067e0: 7370 6c69 7474 696e 670d 0a20 2020 2020  splitting..     
+000067f0: 2020 2069 6620 6e6f 7420 7365 6c66 2e68     if not self.h
+00006800: 6173 5f77 6f72 6473 206f 7220 286d 6178  as_words or (max
+00006810: 5f63 6861 7273 2069 7320 4e6f 6e65 2061  _chars is None a
+00006820: 6e64 206d 6178 5f77 6f72 6473 2069 7320  nd max_words is 
+00006830: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
+00006840: 2020 2020 7265 7475 726e 205b 5d0d 0a20      return [].. 
+00006850: 2020 2020 2020 2061 7373 6572 7420 6d61         assert ma
+00006860: 785f 6368 6172 7320 213d 2030 2061 6e64  x_chars != 0 and
+00006870: 206d 6178 5f77 6f72 6473 2021 3d20 302c   max_words != 0,
+00006880: 205c 0d0a 2020 2020 2020 2020 2020 2020   \..            
+00006890: 6627 6d61 785f 6368 6172 7320 616e 6420  f'max_chars and 
+000068a0: 6d61 785f 776f 7264 7320 6d75 7374 2062  max_words must b
+000068b0: 6520 6772 6561 7465 7220 302c 2062 7574  e greater 0, but
+000068c0: 2067 6f74 207b 6d61 785f 6368 6172 737d   got {max_chars}
+000068d0: 2061 6e64 207b 6d61 785f 776f 7264 737d   and {max_words}
+000068e0: 270d 0a20 2020 2020 2020 2069 6620 6c65  '..        if le
+000068f0: 6e28 7365 6c66 2e77 6f72 6473 2920 3c20  n(self.words) < 
+00006900: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
+00006910: 7265 7475 726e 205b 5d0d 0a20 2020 2020  return []..     
+00006920: 2020 2069 6e64 6963 6573 203d 205b 5d0d     indices = [].
+00006930: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
+00006940: 5f73 706c 6974 3a0d 0a20 2020 2020 2020  _split:..       
+00006950: 2020 2020 2063 6861 725f 636f 756e 7420       char_count 
+00006960: 3d20 2d31 2069 6620 6d61 785f 6368 6172  = -1 if max_char
+00006970: 7320 6973 204e 6f6e 6520 656c 7365 2073  s is None else s
+00006980: 756d 286d 6170 286c 656e 2c20 7365 6c66  um(map(len, self
+00006990: 2e77 6f72 6473 2929 0d0a 2020 2020 2020  .words))..      
+000069a0: 2020 2020 2020 776f 7264 5f63 6f75 6e74        word_count
+000069b0: 203d 202d 3120 6966 206d 6178 5f77 6f72   = -1 if max_wor
+000069c0: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
+000069d0: 6c65 6e28 7365 6c66 2e77 6f72 6473 290d  len(self.words).
+000069e0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+000069f0: 6565 645f 6368 6172 7320 3d20 6d61 785f  eed_chars = max_
+00006a00: 6368 6172 7320 6973 206e 6f74 204e 6f6e  chars is not Non
+00006a10: 6520 616e 6420 6368 6172 5f63 6f75 6e74  e and char_count
+00006a20: 203e 206d 6178 5f63 6861 7273 0d0a 2020   > max_chars..  
+00006a30: 2020 2020 2020 2020 2020 6578 6365 6564            exceed
+00006a40: 5f77 6f72 6473 203d 206d 6178 5f77 6f72  _words = max_wor
+00006a50: 6473 2069 7320 6e6f 7420 4e6f 6e65 2061  ds is not None a
+00006a60: 6e64 2077 6f72 645f 636f 756e 7420 3e20  nd word_count > 
+00006a70: 6d61 785f 776f 7264 730d 0a20 2020 2020  max_words..     
+00006a80: 2020 2020 2020 2069 6620 6578 6365 6564         if exceed
+00006a90: 5f63 6861 7273 3a0d 0a20 2020 2020 2020  _chars:..       
+00006aa0: 2020 2020 2020 2020 2073 706c 6974 7320           splits 
+00006ab0: 3d20 6e70 2e63 6569 6c28 6368 6172 5f63  = np.ceil(char_c
+00006ac0: 6f75 6e74 202f 206d 6178 5f63 6861 7273  ount / max_chars
+00006ad0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00006ae0: 2020 2063 6861 7273 5f70 6572 5f73 706c     chars_per_spl
+00006af0: 6974 203d 2063 6861 725f 636f 756e 7420  it = char_count 
+00006b00: 2f20 7370 6c69 7473 0d0a 2020 2020 2020  / splits..      
+00006b10: 2020 2020 2020 2020 2020 6375 6d5f 6368            cum_ch
+00006b20: 6172 5f63 6f75 6e74 203d 206e 702e 6375  ar_count = np.cu
+00006b30: 6d73 756d 285b 6c65 6e28 772e 776f 7264  msum([len(w.word
+00006b40: 2920 666f 7220 7720 696e 2073 656c 662e  ) for w in self.
+00006b50: 776f 7264 735b 3a2d 315d 5d29 0d0a 2020  words[:-1]])..  
+00006b60: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00006b70: 6469 6365 7320 3d20 5b0d 0a20 2020 2020  dices = [..     
+00006b80: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00006b90: 6e70 2e61 6273 2863 756d 5f63 6861 725f  np.abs(cum_char_
+00006ba0: 636f 756e 742d 2869 2a63 6861 7273 5f70  count-(i*chars_p
+00006bb0: 6572 5f73 706c 6974 2929 292e 6172 676d  er_split))).argm
+00006bc0: 696e 2829 0d0a 2020 2020 2020 2020 2020  in()..          
+00006bd0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00006be0: 696e 2072 616e 6765 2831 2c20 696e 7428  in range(1, int(
+00006bf0: 7370 6c69 7473 2929 0d0a 2020 2020 2020  splits))..      
+00006c00: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
+00006c10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00006c20: 6d61 785f 776f 7264 7320 6973 206e 6f74  max_words is not
+00006c30: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00006c40: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00006c50: 6564 5f77 6f72 6473 203d 2061 6e79 286a  ed_words = any(j
+00006c60: 2d69 2b31 203e 206d 6178 5f77 6f72 6473  -i+1 > max_words
+00006c70: 2066 6f72 2069 2c20 6a20 696e 207a 6970   for i, j in zip
+00006c80: 285b 305d 2b69 6e64 6963 6573 2c20 696e  ([0]+indices, in
+00006c90: 6469 6365 732b 5b6c 656e 2873 656c 662e  dices+[len(self.
+00006ca0: 776f 7264 7329 5d29 290d 0a0d 0a20 2020  words)]))....   
+00006cb0: 2020 2020 2020 2020 2069 6620 6578 6365           if exce
+00006cc0: 6564 5f77 6f72 6473 3a0d 0a20 2020 2020  ed_words:..     
+00006cd0: 2020 2020 2020 2020 2020 2073 706c 6974             split
+00006ce0: 7320 3d20 6e70 2e63 6569 6c28 776f 7264  s = np.ceil(word
+00006cf0: 5f63 6f75 6e74 202f 206d 6178 5f77 6f72  _count / max_wor
+00006d00: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
+00006d10: 2020 2020 2077 6f72 6473 5f70 6572 5f73       words_per_s
+00006d20: 706c 6974 203d 2077 6f72 645f 636f 756e  plit = word_coun
+00006d30: 7420 2f20 7370 6c69 7473 0d0a 2020 2020  t / splits..    
+00006d40: 2020 2020 2020 2020 2020 2020 6375 6d5f              cum_
+00006d50: 776f 7264 5f63 6f75 6e74 203d 206e 702e  word_count = np.
+00006d60: 6172 7261 7928 7261 6e67 6528 312c 206c  array(range(1, l
+00006d70: 656e 2873 656c 662e 776f 7264 7329 2b31  en(self.words)+1
+00006d80: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00006d90: 2020 2020 696e 6469 6365 7320 3d20 5b0d      indices = [.
+00006da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006db0: 2020 2020 206e 702e 6162 7328 6375 6d5f       np.abs(cum_
+00006dc0: 776f 7264 5f63 6f75 6e74 2d28 692a 776f  word_count-(i*wo
+00006dd0: 7264 735f 7065 725f 7370 6c69 7429 292e  rds_per_split)).
+00006de0: 6172 676d 696e 2829 0d0a 2020 2020 2020  argmin()..      
+00006df0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00006e00: 7220 6920 696e 2072 616e 6765 2831 2c20  r i in range(1, 
+00006e10: 696e 7428 7370 6c69 7473 2929 0d0a 2020  int(splits))..  
+00006e20: 2020 2020 2020 2020 2020 2020 2020 5d0d                ].
+00006e30: 0a0d 0a20 2020 2020 2020 2065 6c73 653a  ...        else:
+00006e40: 0d0a 2020 2020 2020 2020 2020 2020 6375  ..            cu
+00006e50: 7272 5f77 6f72 6473 203d 2030 0d0a 2020  rr_words = 0..  
+00006e60: 2020 2020 2020 2020 2020 6375 7272 5f63            curr_c
+00006e70: 6861 7273 203d 2030 0d0a 2020 2020 2020  hars = 0..      
+00006e80: 2020 2020 2020 6c6f 636b 6564 5f69 6e64        locked_ind
+00006e90: 6963 6573 203d 205b 5d0d 0a20 2020 2020  ices = []..     
+00006ea0: 2020 2020 2020 2069 6620 696e 636c 7564         if includ
+00006eb0: 655f 6c6f 636b 3a0d 0a20 2020 2020 2020  e_lock:..       
+00006ec0: 2020 2020 2020 2020 206c 6f63 6b65 645f           locked_
+00006ed0: 696e 6469 6365 7320 3d20 7365 6c66 2e67  indices = self.g
+00006ee0: 6574 5f6c 6f63 6b65 645f 696e 6469 6365  et_locked_indice
+00006ef0: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
+00006f00: 2066 6f72 2069 2c20 776f 7264 2069 6e20   for i, word in 
+00006f10: 656e 756d 6572 6174 6528 7365 6c66 2e77  enumerate(self.w
+00006f20: 6f72 6473 293a 0d0a 2020 2020 2020 2020  ords):..        
+00006f30: 2020 2020 2020 2020 6375 7272 5f77 6f72          curr_wor
+00006f40: 6473 202b 3d20 310d 0a20 2020 2020 2020  ds += 1..       
+00006f50: 2020 2020 2020 2020 2063 7572 725f 6368           curr_ch
+00006f60: 6172 7320 2b3d 206c 656e 2877 6f72 6429  ars += len(word)
+00006f70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006f80: 2020 6966 2069 2021 3d20 303a 0d0a 2020    if i != 0:..  
+00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fa0: 2020 6966 2028 0d0a 2020 2020 2020 2020    if (..        
 00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fc0: 2020 2020 2020 2020 2020 2020 6f72 0d0a              or..
-00006fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fe0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-00006ff0: 776f 7264 7320 6973 206e 6f74 204e 6f6e  words is not Non
-00007000: 6520 616e 6420 6375 7272 5f77 6f72 6473  e and curr_words
-00007010: 203e 206d 6178 5f77 6f72 6473 0d0a 2020   > max_words..  
+00006fc0: 2020 2020 6d61 785f 6368 6172 7320 6973      max_chars is
+00006fd0: 206e 6f74 204e 6f6e 6520 616e 6420 6375   not None and cu
+00006fe0: 7272 5f63 6861 7273 203e 206d 6178 5f63  rr_chars > max_c
+00006ff0: 6861 7273 0d0a 2020 2020 2020 2020 2020  hars..          
+00007000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007010: 2020 6f72 0d0a 2020 2020 2020 2020 2020    or..          
 00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007030: 2020 2920 616e 6420 692d 3120 6e6f 7420    ) and i-1 not 
-00007040: 696e 206c 6f63 6b65 645f 696e 6469 6365  in locked_indice
-00007050: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00007060: 2020 2020 2020 2020 2020 2020 696e 6469              indi
-00007070: 6365 732e 6170 7065 6e64 2869 2d31 290d  ces.append(i-1).
-00007080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007090: 2020 2020 2020 2020 2063 7572 725f 776f           curr_wo
-000070a0: 7264 7320 3d20 310d 0a20 2020 2020 2020  rds = 1..       
-000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070c0: 2063 7572 725f 6368 6172 7320 3d20 6c65   curr_chars = le
-000070d0: 6e28 776f 7264 290d 0a20 2020 2020 2020  n(word)..       
-000070e0: 2072 6574 7572 6e20 696e 6469 6365 730d   return indices.
-000070f0: 0a0d 0a20 2020 2064 6566 2067 6574 5f64  ...    def get_d
-00007100: 7572 6174 696f 6e5f 696e 6469 6365 7328  uration_indices(
-00007110: 7365 6c66 2c20 6d61 785f 6475 723a 2066  self, max_dur: f
-00007120: 6c6f 6174 2c20 6576 656e 5f73 706c 6974  loat, even_split
-00007130: 3a20 626f 6f6c 203d 2054 7275 652c 2069  : bool = True, i
-00007140: 6e63 6c75 6465 5f6c 6f63 6b3a 2062 6f6f  nclude_lock: boo
-00007150: 6c20 3d20 4661 6c73 6529 3a0d 0a20 2020  l = False):..   
-00007160: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00007170: 2e68 6173 5f77 6f72 6473 206f 7220 2874  .has_words or (t
-00007180: 6f74 616c 5f64 7572 6174 696f 6e20 3a3d  otal_duration :=
-00007190: 206e 702e 7375 6d28 5b77 2e64 7572 6174   np.sum([w.durat
-000071a0: 696f 6e20 666f 7220 7720 696e 2073 656c  ion for w in sel
-000071b0: 662e 776f 7264 735d 2929 203c 3d20 6d61  f.words])) <= ma
-000071c0: 785f 6475 723a 0d0a 2020 2020 2020 2020  x_dur:..        
-000071d0: 2020 2020 7265 7475 726e 205b 5d0d 0a20      return [].. 
-000071e0: 2020 2020 2020 2069 6620 6576 656e 5f73         if even_s
-000071f0: 706c 6974 3a0d 0a20 2020 2020 2020 2020  plit:..         
-00007200: 2020 2073 706c 6974 7320 3d20 6e70 2e63     splits = np.c
-00007210: 6569 6c28 746f 7461 6c5f 6475 7261 7469  eil(total_durati
-00007220: 6f6e 202f 206d 6178 5f64 7572 290d 0a20  on / max_dur).. 
-00007230: 2020 2020 2020 2020 2020 2064 7572 5f70             dur_p
-00007240: 6572 5f73 706c 6974 203d 2074 6f74 616c  er_split = total
-00007250: 5f64 7572 6174 696f 6e20 2f20 7370 6c69  _duration / spli
-00007260: 7473 0d0a 2020 2020 2020 2020 2020 2020  ts..            
-00007270: 6375 6d5f 6475 7220 3d20 6e70 2e63 756d  cum_dur = np.cum
-00007280: 7375 6d28 5b77 2e64 7572 6174 696f 6e20  sum([w.duration 
-00007290: 666f 7220 7720 696e 2073 656c 662e 776f  for w in self.wo
-000072a0: 7264 735b 3a2d 315d 5d29 0d0a 2020 2020  rds[:-1]])..    
-000072b0: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
-000072c0: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
-000072d0: 2020 2020 2028 6e70 2e61 6273 2863 756d       (np.abs(cum
-000072e0: 5f64 7572 202d 2028 6920 2a20 6475 725f  _dur - (i * dur_
-000072f0: 7065 725f 7370 6c69 7429 2929 2e61 7267  per_split))).arg
-00007300: 6d69 6e28 290d 0a20 2020 2020 2020 2020  min()..         
-00007310: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00007320: 7261 6e67 6528 312c 2069 6e74 2873 706c  range(1, int(spl
-00007330: 6974 7329 290d 0a20 2020 2020 2020 2020  its))..         
-00007340: 2020 205d 0d0a 2020 2020 2020 2020 656c     ]..        el
-00007350: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00007360: 2069 6e64 6963 6573 203d 205b 5d0d 0a20   indices = [].. 
-00007370: 2020 2020 2020 2020 2020 2063 7572 725f             curr_
-00007380: 746f 7461 6c5f 6475 7220 3d20 302e 300d  total_dur = 0.0.
-00007390: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
-000073a0: 6b65 645f 696e 6469 6365 7320 3d20 7365  ked_indices = se
-000073b0: 6c66 2e67 6574 5f6c 6f63 6b65 645f 696e  lf.get_locked_in
-000073c0: 6469 6365 7328 2920 6966 2069 6e63 6c75  dices() if inclu
-000073d0: 6465 5f6c 6f63 6b20 656c 7365 205b 5d0d  de_lock else [].
-000073e0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000073f0: 2069 2c20 776f 7264 2069 6e20 656e 756d   i, word in enum
-00007400: 6572 6174 6528 7365 6c66 2e77 6f72 6473  erate(self.words
-00007410: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00007420: 2020 2020 6375 7272 5f74 6f74 616c 5f64      curr_total_d
-00007430: 7572 202b 3d20 776f 7264 2e64 7572 6174  ur += word.durat
-00007440: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00007450: 2020 2020 2069 6620 6920 213d 2030 3a0d       if i != 0:.
-00007460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007470: 2020 2020 2069 6620 6375 7272 5f74 6f74       if curr_tot
-00007480: 616c 5f64 7572 203e 206d 6178 5f64 7572  al_dur > max_dur
-00007490: 2061 6e64 2069 202d 2031 206e 6f74 2069   and i - 1 not i
-000074a0: 6e20 6c6f 636b 6564 5f69 6e64 6963 6573  n locked_indices
-000074b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000074c0: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
-000074d0: 6573 2e61 7070 656e 6428 6920 2d20 3129  es.append(i - 1)
-000074e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000074f0: 2020 2020 2020 2020 2020 6375 7272 5f74            curr_t
-00007500: 6f74 616c 5f64 7572 203d 2077 6f72 642e  otal_dur = word.
-00007510: 6475 7261 7469 6f6e 0d0a 2020 2020 2020  duration..      
-00007520: 2020 7265 7475 726e 2069 6e64 6963 6573    return indices
-00007530: 0d0a 0d0a 2020 2020 6465 6620 7370 6c69  ....    def spli
-00007540: 7428 7365 6c66 2c20 696e 6469 6365 733a  t(self, indices:
-00007550: 204c 6973 745b 696e 745d 293a 0d0a 2020   List[int]):..  
-00007560: 2020 2020 2020 6966 206c 656e 2869 6e64        if len(ind
-00007570: 6963 6573 2920 3d3d 2030 3a0d 0a20 2020  ices) == 0:..   
-00007580: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00007590: 5b5d 0d0a 2020 2020 2020 2020 6966 2069  []..        if i
-000075a0: 6e64 6963 6573 5b2d 315d 2021 3d20 6c65  ndices[-1] != le
-000075b0: 6e28 7365 6c66 2e77 6f72 6473 2920 2d20  n(self.words) - 
-000075c0: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-000075d0: 696e 6469 6365 732e 6170 7065 6e64 286c  indices.append(l
-000075e0: 656e 2873 656c 662e 776f 7264 7329 202d  en(self.words) -
-000075f0: 2031 290d 0a20 2020 2020 2020 2073 6567   1)..        seg
-00007600: 5f63 6f70 6965 7320 3d20 5b5d 0d0a 2020  _copies = []..  
-00007610: 2020 2020 2020 7072 6576 5f69 203d 2030        prev_i = 0
-00007620: 0d0a 2020 2020 2020 2020 666f 7220 6920  ..        for i 
-00007630: 696e 2069 6e64 6963 6573 3a0d 0a20 2020  in indices:..   
-00007640: 2020 2020 2020 2020 2069 202b 3d20 310d           i += 1.
-00007650: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
-00007660: 5f77 6f72 6473 203d 2073 656c 662e 776f  _words = self.wo
-00007670: 7264 735b 7072 6576 5f69 3a69 5d0d 0a20  rds[prev_i:i].. 
-00007680: 2020 2020 2020 2020 2020 206e 6577 5f73             new_s
-00007690: 6567 203d 2073 656c 662e 636f 7079 286e  eg = self.copy(n
-000076a0: 6577 5f77 6f72 6473 2c20 636f 7079 5f77  ew_words, copy_w
-000076b0: 6f72 6473 3d46 616c 7365 290d 0a20 2020  ords=False)..   
-000076c0: 2020 2020 2020 2020 2073 6567 5f63 6f70           seg_cop
-000076d0: 6965 732e 6170 7065 6e64 286e 6577 5f73  ies.append(new_s
-000076e0: 6567 290d 0a20 2020 2020 2020 2020 2020  eg)..           
-000076f0: 2070 7265 765f 6920 3d20 690d 0a20 2020   prev_i = i..   
-00007700: 2020 2020 2072 6574 7572 6e20 7365 675f       return seg_
-00007710: 636f 7069 6573 0d0a 0d0a 2020 2020 6465  copies....    de
-00007720: 6620 7365 745f 7265 7375 6c74 2873 656c  f set_result(sel
-00007730: 662c 2072 6573 756c 743a 2027 5768 6973  f, result: 'Whis
-00007740: 7065 7252 6573 756c 7427 293a 0d0a 2020  perResult'):..  
-00007750: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-00007760: 6172 6e28 2760 602e 7365 745f 7265 7375  arn('``.set_resu
-00007770: 6c74 2863 7572 7265 6e74 5f72 6573 756c  lt(current_resul
-00007780: 745f 696e 7374 616e 6365 2960 6020 6973  t_instance)`` is
-00007790: 2064 6570 7265 6361 7465 6420 616e 6420   deprecated and 
-000077a0: 7769 6c6c 2062 6520 7265 6d6f 7665 6420  will be removed 
-000077b0: 696e 2066 7574 7572 6520 7665 7273 696f  in future versio
-000077c0: 6e73 2e20 270d 0a20 2020 2020 2020 2020  ns. '..         
-000077d0: 2020 2020 2020 2020 2020 2020 2027 5573               'Us
-000077e0: 6520 6060 2e72 6573 756c 7420 3d20 6375  e ``.result = cu
-000077f0: 7272 656e 745f 7265 7375 6c74 5f69 6e73  rrent_result_ins
-00007800: 7461 6e63 6560 6020 696e 7374 6561 642e  tance`` instead.
-00007810: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00007820: 2020 2020 2020 2020 2020 7374 6163 6b6c            stackl
-00007830: 6576 656c 3d32 290d 0a20 2020 2020 2020  evel=2)..       
-00007840: 2073 656c 662e 7265 7375 6c74 203d 2072   self.result = r
-00007850: 6573 756c 740d 0a0d 0a20 2020 2064 6566  esult....    def
-00007860: 2067 6574 5f72 6573 756c 7428 7365 6c66   get_result(self
-00007870: 2920 2d3e 2055 6e69 6f6e 5b27 5768 6973  ) -> Union['Whis
-00007880: 7065 7252 6573 756c 7427 2c20 4e6f 6e65  perResult', None
-00007890: 5d3a 0d0a 2020 2020 2020 2020 2222 220d  ]:..        """.
-000078a0: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
-000078b0: 6f75 7465 7220 696e 7374 616e 6365 206f  outer instance o
-000078c0: 6620 3a63 6c61 7373 3a60 7374 6162 6c65  f :class:`stable
-000078d0: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
-000078e0: 5768 6973 7065 7252 6573 756c 7460 2074  WhisperResult` t
-000078f0: 6861 7420 6060 7365 6c66 6060 2069 7320  hat ``self`` is 
-00007900: 6120 7061 7274 206f 662e 0d0a 2020 2020  a part of...    
-00007910: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00007920: 2077 6172 6e69 6e67 732e 7761 726e 2827   warnings.warn('
-00007930: 6060 2e67 6574 5f72 6573 756c 7428 2960  ``.get_result()`
-00007940: 6020 7769 6c6c 2062 6520 7265 6d6f 7665  ` will be remove
-00007950: 6420 696e 2066 7574 7572 6520 7665 7273  d in future vers
-00007960: 696f 6e73 2e20 5573 6520 6060 2e72 6573  ions. Use ``.res
-00007970: 756c 7460 6020 696e 7374 6561 642e 272c  ult`` instead.',
-00007980: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007990: 2020 2020 2020 2020 7374 6163 6b6c 6576          stacklev
-000079a0: 656c 3d32 290d 0a20 2020 2020 2020 2072  el=2)..        r
-000079b0: 6574 7572 6e20 7365 6c66 2e72 6573 756c  eturn self.resul
-000079c0: 740d 0a0d 0a0d 0a63 6c61 7373 2057 6869  t......class Whi
-000079d0: 7370 6572 5265 7375 6c74 3a0d 0a0d 0a20  sperResult:.... 
-000079e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000079f0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00007a00: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
-00007a10: 2072 6573 756c 743a 2055 6e69 6f6e 5b73   result: Union[s
-00007a20: 7472 2c20 6469 6374 2c20 6c69 7374 5d2c  tr, dict, list],
-00007a30: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00007a40: 7263 655f 6f72 6465 723a 2062 6f6f 6c20  rce_order: bool 
-00007a50: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
-00007a60: 2020 2020 2020 6368 6563 6b5f 736f 7274        check_sort
-00007a70: 6564 3a20 556e 696f 6e5b 626f 6f6c 2c20  ed: Union[bool, 
-00007a80: 7374 725d 203d 2054 7275 652c 0d0a 2020  str] = True,..  
-00007a90: 2020 2020 2020 2020 2020 7368 6f77 5f75            show_u
-00007aa0: 6e73 6f72 7465 643a 2062 6f6f 6c20 3d20  nsorted: bool = 
-00007ab0: 5472 7565 0d0a 2020 2020 293a 0d0a 2020  True..    ):..  
-00007ac0: 2020 2020 2020 7265 7375 6c74 2c20 7365        result, se
-00007ad0: 6c66 2e70 6174 6820 3d20 7365 6c66 2e5f  lf.path = self._
-00007ae0: 7374 616e 6461 7264 697a 655f 7265 7375  standardize_resu
-00007af0: 6c74 2872 6573 756c 7429 0d0a 2020 2020  lt(result)..    
-00007b00: 2020 2020 7365 6c66 2e6f 7269 5f64 6963      self.ori_dic
-00007b10: 7420 3d20 7265 7375 6c74 2e67 6574 2827  t = result.get('
-00007b20: 6f72 695f 6469 6374 2729 206f 7220 7265  ori_dict') or re
-00007b30: 7375 6c74 0d0a 2020 2020 2020 2020 7365  sult..        se
-00007b40: 6c66 2e6c 616e 6775 6167 6520 3d20 7365  lf.language = se
-00007b50: 6c66 2e6f 7269 5f64 6963 742e 6765 7428  lf.ori_dict.get(
-00007b60: 276c 616e 6775 6167 6527 290d 0a20 2020  'language')..   
-00007b70: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
-00007b80: 7570 5f68 6973 746f 7279 203d 2072 6573  up_history = res
-00007b90: 756c 742e 6765 7428 2772 6567 726f 7570  ult.get('regroup
-00007ba0: 5f68 6973 746f 7279 272c 2027 2729 0d0a  _history', '')..
-00007bb0: 2020 2020 2020 2020 7365 6c66 2e5f 6e6f          self._no
-00007bc0: 6e73 7065 6563 685f 7365 6374 696f 6e73  nspeech_sections
-00007bd0: 203d 2072 6573 756c 742e 6765 7428 276e   = result.get('n
-00007be0: 6f6e 7370 6565 6368 5f73 6563 7469 6f6e  onspeech_section
-00007bf0: 7327 2c20 5b5d 290d 0a20 2020 2020 2020  s', [])..       
-00007c00: 2073 6567 6d65 6e74 7320 3d20 2872 6573   segments = (res
-00007c10: 756c 742e 6765 7428 2773 6567 6d65 6e74  ult.get('segment
-00007c20: 7327 2c20 7365 6c66 2e6f 7269 5f64 6963  s', self.ori_dic
-00007c30: 742e 6765 7428 2773 6567 6d65 6e74 7327  t.get('segments'
-00007c40: 2929 206f 7220 7b7d 292e 636f 7079 2829  )) or {}).copy()
-00007c50: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00007c60: 6567 6d65 6e74 7320 3d20 5b53 6567 6d65  egments = [Segme
-00007c70: 6e74 282a 2a73 2c20 6967 6e6f 7265 5f75  nt(**s, ignore_u
-00007c80: 6e75 7365 645f 6172 6773 3d54 7275 6529  nused_args=True)
-00007c90: 2066 6f72 2073 2069 6e20 7365 676d 656e   for s in segmen
-00007ca0: 7473 5d20 6966 2073 6567 6d65 6e74 7320  ts] if segments 
-00007cb0: 656c 7365 205b 5d0d 0a20 2020 2020 2020  else []..       
-00007cc0: 2073 656c 662e 5f66 6f72 6365 645f 6f72   self._forced_or
-00007cd0: 6465 7220 3d20 666f 7263 655f 6f72 6465  der = force_orde
-00007ce0: 720d 0a20 2020 2020 2020 2069 6620 7365  r..        if se
-00007cf0: 6c66 2e5f 666f 7263 6564 5f6f 7264 6572  lf._forced_order
-00007d00: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00007d10: 656c 662e 666f 7263 655f 6f72 6465 7228  elf.force_order(
-00007d20: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007d30: 7261 6973 655f 666f 725f 756e 736f 7274  raise_for_unsort
-00007d40: 6564 2863 6865 636b 5f73 6f72 7465 642c  ed(check_sorted,
-00007d50: 2073 686f 775f 756e 736f 7274 6564 290d   show_unsorted).
-00007d60: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00007d70: 6d6f 7665 5f6e 6f5f 776f 7264 5f73 6567  move_no_word_seg
-00007d80: 6d65 6e74 7328 616e 7928 7365 672e 6861  ments(any(seg.ha
-00007d90: 735f 776f 7264 7320 666f 7220 7365 6720  s_words for seg 
-00007da0: 696e 2073 656c 662e 7365 676d 656e 7473  in self.segments
-00007db0: 2929 0d0a 0d0a 2020 2020 6465 6620 5f5f  ))....    def __
-00007dc0: 6765 7469 7465 6d5f 5f28 7365 6c66 2c20  getitem__(self, 
-00007dd0: 696e 6465 783a 2069 6e74 2920 2d3e 2053  index: int) -> S
-00007de0: 6567 6d65 6e74 3a0d 0a20 2020 2020 2020  egment:..       
-00007df0: 2072 6574 7572 6e20 7365 6c66 2e73 6567   return self.seg
-00007e00: 6d65 6e74 735b 696e 6465 785d 0d0a 0d0a  ments[index]....
-00007e10: 2020 2020 6465 6620 5f5f 6465 6c69 7465      def __delite
-00007e20: 6d5f 5f28 7365 6c66 2c20 696e 6465 783a  m__(self, index:
-00007e30: 2069 6e74 293a 0d0a 2020 2020 2020 2020   int):..        
-00007e40: 6465 6c20 7365 6c66 2e73 6567 6d65 6e74  del self.segment
-00007e50: 735b 696e 6465 785d 0d0a 2020 2020 2020  s[index]..      
-00007e60: 2020 7365 6c66 2e72 6561 7373 6967 6e5f    self.reassign_
-00007e70: 6964 7328 5472 7565 2c20 7374 6172 743d  ids(True, start=
-00007e80: 696e 6465 7829 0d0a 0d0a 2020 2020 4070  index)....    @p
-00007e90: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
-00007ea0: 2064 7572 6174 696f 6e28 7365 6c66 293a   duration(self):
-00007eb0: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-00007ec0: 2073 656c 662e 7365 676d 656e 7473 3a0d   self.segments:.
-00007ed0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00007ee0: 7572 6e20 302e 300d 0a20 2020 2020 2020  urn 0.0..       
-00007ef0: 2072 6574 7572 6e20 5f72 6f75 6e64 5f74   return _round_t
-00007f00: 696d 6573 7461 6d70 2873 656c 662e 7365  imestamp(self.se
-00007f10: 676d 656e 7473 5b2d 315d 2e65 6e64 202d  gments[-1].end -
-00007f20: 2073 656c 662e 7365 676d 656e 7473 5b30   self.segments[0
-00007f30: 5d2e 7374 6172 7429 0d0a 0d0a 2020 2020  ].start)....    
-00007f40: 4073 7461 7469 636d 6574 686f 640d 0a20  @staticmethod.. 
-00007f50: 2020 2064 6566 205f 7374 616e 6461 7264     def _standard
-00007f60: 697a 655f 7265 7375 6c74 2872 6573 756c  ize_result(resul
-00007f70: 743a 2055 6e69 6f6e 5b73 7472 2c20 6469  t: Union[str, di
-00007f80: 6374 2c20 4c69 7374 5b64 6963 745d 2c20  ct, List[dict], 
-00007f90: 4c69 7374 5b4c 6973 745b 6469 6374 5d5d  List[List[dict]]
-00007fa0: 5d29 202d 3e20 5475 706c 655b 6469 6374  ]) -> Tuple[dict
-00007fb0: 2c20 556e 696f 6e5b 7374 722c 204e 6f6e  , Union[str, Non
-00007fc0: 655d 5d3a 0d0a 2020 2020 2020 2020 7061  e]]:..        pa
-00007fd0: 7468 203d 204e 6f6e 650d 0a20 2020 2020  th = None..     
-00007fe0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00007ff0: 2872 6573 756c 742c 2073 7472 293a 0d0a  (result, str):..
-00008000: 2020 2020 2020 2020 2020 2020 7061 7468              path
-00008010: 203d 2072 6573 756c 740d 0a20 2020 2020   = result..     
-00008020: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00008030: 6c6f 6164 5f72 6573 756c 7428 7061 7468  load_result(path
-00008040: 290d 0a20 2020 2020 2020 2069 6620 6973  )..        if is
-00008050: 696e 7374 616e 6365 2872 6573 756c 742c  instance(result,
-00008060: 2064 6963 7429 3a0d 0a20 2020 2020 2020   dict):..       
-00008070: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00008080: 6c74 2c20 7061 7468 0d0a 2020 2020 2020  lt, path..      
-00008090: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-000080a0: 6e63 6528 7265 7375 6c74 2c20 6c69 7374  nce(result, list
-000080b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000080c0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-000080d0: 6627 4578 7065 6374 2072 6573 756c 7420  f'Expect result 
-000080e0: 746f 2062 6520 6c69 7374 2062 7574 2067  to be list but g
-000080f0: 6f74 207b 7479 7065 2872 6573 756c 7429  ot {type(result)
-00008100: 7d27 290d 0a20 2020 2020 2020 2069 6620  }')..        if 
-00008110: 6e6f 7420 7265 7375 6c74 206f 7220 6e6f  not result or no
-00008120: 7420 7265 7375 6c74 5b30 5d3a 0d0a 2020  t result[0]:..  
-00008130: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008140: 207b 7d2c 2070 6174 680d 0a20 2020 2020   {}, path..     
-00008150: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00008160: 2872 6573 756c 745b 305d 2c20 6c69 7374  (result[0], list
-00008170: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00008180: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-00008190: 6528 7265 7375 6c74 5b30 5d5b 305d 2c20  e(result[0][0], 
-000081a0: 6469 6374 293a 0d0a 2020 2020 2020 2020  dict):..        
-000081b0: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-000081c0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-000081d0: 7228 6627 476f 7420 6c69 7374 206f 6620  r(f'Got list of 
-000081e0: 6c69 7374 206f 6620 7b74 7970 6528 7265  list of {type(re
-000081f0: 7375 6c74 5b30 5d29 7d20 6275 7420 6578  sult[0])} but ex
-00008200: 7065 6374 7320 6c69 7374 206f 6620 6c69  pects list of li
-00008210: 7374 206f 6620 6469 6374 2729 0d0a 2020  st of dict')..  
-00008220: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00008230: 203d 2064 6963 7428 0d0a 2020 2020 2020   = dict(..      
-00008240: 2020 2020 2020 2020 2020 7365 676d 656e            segmen
-00008250: 7473 3d5b 0d0a 2020 2020 2020 2020 2020  ts=[..          
-00008260: 2020 2020 2020 2020 2020 6469 6374 280d            dict(.
-00008270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008280: 2020 2020 2020 2020 2073 7461 7274 3d77           start=w
-00008290: 6f72 6473 5b30 5d5b 2773 7461 7274 275d  ords[0]['start']
-000082a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000082b0: 2020 2020 2020 2020 2020 2065 6e64 3d77             end=w
-000082c0: 6f72 6473 5b2d 315d 5b27 656e 6427 5d2c  ords[-1]['end'],
-000082d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000082e0: 2020 2020 2020 2020 2020 7465 7874 3d27            text='
-000082f0: 272e 6a6f 696e 2877 5b27 776f 7264 275d  '.join(w['word']
-00008300: 2066 6f72 2077 2069 6e20 776f 7264 7329   for w in words)
-00008310: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00008320: 2020 2020 2020 2020 2020 2077 6f72 6473             words
-00008330: 3d77 6f72 6473 0d0a 2020 2020 2020 2020  =words..        
-00008340: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00008350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008360: 2020 2066 6f72 2077 6f72 6473 2069 6e20     for words in 
-00008370: 7265 7375 6c74 2069 6620 776f 7264 730d  result if words.
-00008380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008390: 205d 0d0a 2020 2020 2020 2020 2020 2020   ]..            
-000083a0: 290d 0a0d 0a20 2020 2020 2020 2065 6c69  )....        eli
-000083b0: 6620 6973 696e 7374 616e 6365 2872 6573  f isinstance(res
-000083c0: 756c 745b 305d 2c20 6469 6374 293a 0d0a  ult[0], dict):..
-000083d0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000083e0: 6c74 203d 2064 6963 7428 7365 676d 656e  lt = dict(segmen
-000083f0: 7473 3d72 6573 756c 7429 0d0a 2020 2020  ts=result)..    
-00008400: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00008410: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-00008420: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-00008430: 2866 2747 6f74 206c 6973 7420 6f66 207b  (f'Got list of {
-00008440: 7479 7065 2872 6573 756c 745b 305d 297d  type(result[0])}
-00008450: 2062 7574 2065 7870 6563 7473 206c 6973   but expects lis
-00008460: 7420 6f66 206c 6973 742f 6469 6374 2729  t of list/dict')
-00008470: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00008480: 2072 6573 756c 742c 2070 6174 680d 0a0d   result, path...
-00008490: 0a20 2020 2064 6566 2066 6f72 6365 5f6f  .    def force_o
-000084a0: 7264 6572 2873 656c 6629 3a0d 0a20 2020  rder(self):..   
-000084b0: 2020 2020 2070 7265 765f 7473 5f65 6e64       prev_ts_end
-000084c0: 203d 2030 0d0a 2020 2020 2020 2020 7469   = 0..        ti
-000084d0: 6d65 7374 616d 7073 203d 2073 656c 662e  mestamps = self.
-000084e0: 616c 6c5f 776f 7264 735f 6f72 5f73 6567  all_words_or_seg
-000084f0: 6d65 6e74 7328 290d 0a20 2020 2020 2020  ments()..       
-00008500: 2066 6f72 2069 2c20 7473 2069 6e20 656e   for i, ts in en
-00008510: 756d 6572 6174 6528 7469 6d65 7374 616d  umerate(timestam
-00008520: 7073 2c20 3129 3a0d 0a20 2020 2020 2020  ps, 1):..       
-00008530: 2020 2020 2069 6620 7473 2e73 7461 7274       if ts.start
-00008540: 203c 2070 7265 765f 7473 5f65 6e64 3a0d   < prev_ts_end:.
-00008550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008560: 2074 732e 7374 6172 7420 3d20 7072 6576   ts.start = prev
-00008570: 5f74 735f 656e 640d 0a20 2020 2020 2020  _ts_end..       
-00008580: 2020 2020 2069 6620 7473 2e73 7461 7274       if ts.start
-00008590: 203e 2074 732e 656e 643a 0d0a 2020 2020   > ts.end:..    
-000085a0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-000085b0: 7265 765f 7473 5f65 6e64 203e 2074 732e  rev_ts_end > ts.
-000085c0: 656e 643a 0d0a 2020 2020 2020 2020 2020  end:..          
-000085d0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-000085e0: 6773 2e77 6172 6e28 274d 756c 7469 706c  gs.warn('Multipl
-000085f0: 6520 636f 6e73 6563 7574 6976 6520 7469  e consecutive ti
-00008600: 6d65 7374 616d 7073 2061 7265 206f 7574  mestamps are out
-00008610: 206f 6620 6f72 6465 722e 2053 6f6d 6520   of order. Some 
-00008620: 7061 7274 7320 7769 6c6c 2068 6176 6520  parts will have 
-00008630: 6e6f 2064 7572 6174 696f 6e2e 2729 0d0a  no duration.')..
-00008640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008650: 2020 2020 7473 2e73 7461 7274 203d 2074      ts.start = t
-00008660: 732e 656e 640d 0a20 2020 2020 2020 2020  s.end..         
-00008670: 2020 2020 2020 2020 2020 2066 6f72 206a             for j
-00008680: 2069 6e20 7261 6e67 6528 692d 322c 202d   in range(i-2, -
-00008690: 312c 202d 3129 3a0d 0a20 2020 2020 2020  1, -1):..       
-000086a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086b0: 2069 6620 7469 6d65 7374 616d 7073 5b6a   if timestamps[j
-000086c0: 5d2e 656e 6420 3e20 7473 2e65 6e64 3a0d  ].end > ts.end:.
-000086d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000086e0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-000086f0: 6573 7461 6d70 735b 6a5d 2e65 6e64 203d  estamps[j].end =
-00008700: 2074 732e 656e 640d 0a20 2020 2020 2020   ts.end..       
-00008710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008720: 2069 6620 7469 6d65 7374 616d 7073 5b6a   if timestamps[j
-00008730: 5d2e 7374 6172 7420 3e20 7473 2e65 6e64  ].start > ts.end
-00008740: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00008750: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00008760: 696d 6573 7461 6d70 735b 6a5d 2e73 7461  imestamps[j].sta
-00008770: 7274 203d 2074 732e 656e 640d 0a20 2020  rt = ts.end..   
-00008780: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00008790: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000087a0: 2020 2020 2020 2020 6966 2074 732e 7374          if ts.st
-000087b0: 6172 7420 213d 2070 7265 765f 7473 5f65  art != prev_ts_e
-000087c0: 6e64 3a0d 0a20 2020 2020 2020 2020 2020  nd:..           
-000087d0: 2020 2020 2020 2020 2020 2020 2074 732e               ts.
-000087e0: 7374 6172 7420 3d20 7072 6576 5f74 735f  start = prev_ts_
-000087f0: 656e 640d 0a20 2020 2020 2020 2020 2020  end..           
-00008800: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00007030: 2020 6d61 785f 776f 7264 7320 6973 206e    max_words is n
+00007040: 6f74 204e 6f6e 6520 616e 6420 6375 7272  ot None and curr
+00007050: 5f77 6f72 6473 203e 206d 6178 5f77 6f72  _words > max_wor
+00007060: 6473 0d0a 2020 2020 2020 2020 2020 2020  ds..            
+00007070: 2020 2020 2020 2020 2920 616e 6420 692d          ) and i-
+00007080: 3120 6e6f 7420 696e 206c 6f63 6b65 645f  1 not in locked_
+00007090: 696e 6469 6365 733a 0d0a 2020 2020 2020  indices:..      
+000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070b0: 2020 696e 6469 6365 732e 6170 7065 6e64    indices.append
+000070c0: 2869 2d31 290d 0a20 2020 2020 2020 2020  (i-1)..         
+000070d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000070e0: 7572 725f 776f 7264 7320 3d20 310d 0a20  urr_words = 1.. 
+000070f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007100: 2020 2020 2020 2063 7572 725f 6368 6172         curr_char
+00007110: 7320 3d20 6c65 6e28 776f 7264 290d 0a20  s = len(word).. 
+00007120: 2020 2020 2020 2072 6574 7572 6e20 696e         return in
+00007130: 6469 6365 730d 0a0d 0a20 2020 2064 6566  dices....    def
+00007140: 2067 6574 5f64 7572 6174 696f 6e5f 696e   get_duration_in
+00007150: 6469 6365 7328 7365 6c66 2c20 6d61 785f  dices(self, max_
+00007160: 6475 723a 2066 6c6f 6174 2c20 6576 656e  dur: float, even
+00007170: 5f73 706c 6974 3a20 626f 6f6c 203d 2054  _split: bool = T
+00007180: 7275 652c 2069 6e63 6c75 6465 5f6c 6f63  rue, include_loc
+00007190: 6b3a 2062 6f6f 6c20 3d20 4661 6c73 6529  k: bool = False)
+000071a0: 3a0d 0a20 2020 2020 2020 2069 6620 6e6f  :..        if no
+000071b0: 7420 7365 6c66 2e68 6173 5f77 6f72 6473  t self.has_words
+000071c0: 206f 7220 2874 6f74 616c 5f64 7572 6174   or (total_durat
+000071d0: 696f 6e20 3a3d 206e 702e 7375 6d28 5b77  ion := np.sum([w
+000071e0: 2e64 7572 6174 696f 6e20 666f 7220 7720  .duration for w 
+000071f0: 696e 2073 656c 662e 776f 7264 735d 2929  in self.words]))
+00007200: 203c 3d20 6d61 785f 6475 723a 0d0a 2020   <= max_dur:..  
+00007210: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00007220: 205b 5d0d 0a20 2020 2020 2020 2069 6620   []..        if 
+00007230: 6576 656e 5f73 706c 6974 3a0d 0a20 2020  even_split:..   
+00007240: 2020 2020 2020 2020 2073 706c 6974 7320           splits 
+00007250: 3d20 6e70 2e63 6569 6c28 746f 7461 6c5f  = np.ceil(total_
+00007260: 6475 7261 7469 6f6e 202f 206d 6178 5f64  duration / max_d
+00007270: 7572 290d 0a20 2020 2020 2020 2020 2020  ur)..           
+00007280: 2064 7572 5f70 6572 5f73 706c 6974 203d   dur_per_split =
+00007290: 2074 6f74 616c 5f64 7572 6174 696f 6e20   total_duration 
+000072a0: 2f20 7370 6c69 7473 0d0a 2020 2020 2020  / splits..      
+000072b0: 2020 2020 2020 6375 6d5f 6475 7220 3d20        cum_dur = 
+000072c0: 6e70 2e63 756d 7375 6d28 5b77 2e64 7572  np.cumsum([w.dur
+000072d0: 6174 696f 6e20 666f 7220 7720 696e 2073  ation for w in s
+000072e0: 656c 662e 776f 7264 735b 3a2d 315d 5d29  elf.words[:-1]])
+000072f0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00007300: 6469 6365 7320 3d20 5b0d 0a20 2020 2020  dices = [..     
+00007310: 2020 2020 2020 2020 2020 2028 6e70 2e61             (np.a
+00007320: 6273 2863 756d 5f64 7572 202d 2028 6920  bs(cum_dur - (i 
+00007330: 2a20 6475 725f 7065 725f 7370 6c69 7429  * dur_per_split)
+00007340: 2929 2e61 7267 6d69 6e28 290d 0a20 2020  )).argmin()..   
+00007350: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00007360: 2069 2069 6e20 7261 6e67 6528 312c 2069   i in range(1, i
+00007370: 6e74 2873 706c 6974 7329 290d 0a20 2020  nt(splits))..   
+00007380: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
+00007390: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000073a0: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
+000073b0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000073c0: 2063 7572 725f 746f 7461 6c5f 6475 7220   curr_total_dur 
+000073d0: 3d20 302e 300d 0a20 2020 2020 2020 2020  = 0.0..         
+000073e0: 2020 206c 6f63 6b65 645f 696e 6469 6365     locked_indice
+000073f0: 7320 3d20 7365 6c66 2e67 6574 5f6c 6f63  s = self.get_loc
+00007400: 6b65 645f 696e 6469 6365 7328 2920 6966  ked_indices() if
+00007410: 2069 6e63 6c75 6465 5f6c 6f63 6b20 656c   include_lock el
+00007420: 7365 205b 5d0d 0a20 2020 2020 2020 2020  se []..         
+00007430: 2020 2066 6f72 2069 2c20 776f 7264 2069     for i, word i
+00007440: 6e20 656e 756d 6572 6174 6528 7365 6c66  n enumerate(self
+00007450: 2e77 6f72 6473 293a 0d0a 2020 2020 2020  .words):..      
+00007460: 2020 2020 2020 2020 2020 6375 7272 5f74            curr_t
+00007470: 6f74 616c 5f64 7572 202b 3d20 776f 7264  otal_dur += word
+00007480: 2e64 7572 6174 696f 6e0d 0a20 2020 2020  .duration..     
+00007490: 2020 2020 2020 2020 2020 2069 6620 6920             if i 
+000074a0: 213d 2030 3a0d 0a20 2020 2020 2020 2020  != 0:..         
+000074b0: 2020 2020 2020 2020 2020 2069 6620 6375             if cu
+000074c0: 7272 5f74 6f74 616c 5f64 7572 203e 206d  rr_total_dur > m
+000074d0: 6178 5f64 7572 2061 6e64 2069 202d 2031  ax_dur and i - 1
+000074e0: 206e 6f74 2069 6e20 6c6f 636b 6564 5f69   not in locked_i
+000074f0: 6e64 6963 6573 3a0d 0a20 2020 2020 2020  ndices:..       
+00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007510: 2069 6e64 6963 6573 2e61 7070 656e 6428   indices.append(
+00007520: 6920 2d20 3129 0d0a 2020 2020 2020 2020  i - 1)..        
+00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007540: 6375 7272 5f74 6f74 616c 5f64 7572 203d  curr_total_dur =
+00007550: 2077 6f72 642e 6475 7261 7469 6f6e 0d0a   word.duration..
+00007560: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00007570: 6e64 6963 6573 0d0a 0d0a 2020 2020 6465  ndices....    de
+00007580: 6620 7370 6c69 7428 7365 6c66 2c20 696e  f split(self, in
+00007590: 6469 6365 733a 204c 6973 745b 696e 745d  dices: List[int]
+000075a0: 293a 0d0a 2020 2020 2020 2020 6966 206c  ):..        if l
+000075b0: 656e 2869 6e64 6963 6573 2920 3d3d 2030  en(indices) == 0
+000075c0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+000075d0: 6574 7572 6e20 5b5d 0d0a 2020 2020 2020  eturn []..      
+000075e0: 2020 6966 2069 6e64 6963 6573 5b2d 315d    if indices[-1]
+000075f0: 2021 3d20 6c65 6e28 7365 6c66 2e77 6f72   != len(self.wor
+00007600: 6473 2920 2d20 313a 0d0a 2020 2020 2020  ds) - 1:..      
+00007610: 2020 2020 2020 696e 6469 6365 732e 6170        indices.ap
+00007620: 7065 6e64 286c 656e 2873 656c 662e 776f  pend(len(self.wo
+00007630: 7264 7329 202d 2031 290d 0a20 2020 2020  rds) - 1)..     
+00007640: 2020 2073 6567 5f63 6f70 6965 7320 3d20     seg_copies = 
+00007650: 5b5d 0d0a 2020 2020 2020 2020 7072 6576  []..        prev
+00007660: 5f69 203d 2030 0d0a 2020 2020 2020 2020  _i = 0..        
+00007670: 666f 7220 6920 696e 2069 6e64 6963 6573  for i in indices
+00007680: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00007690: 202b 3d20 310d 0a20 2020 2020 2020 2020   += 1..         
+000076a0: 2020 206e 6577 5f77 6f72 6473 203d 2073     new_words = s
+000076b0: 656c 662e 776f 7264 735b 7072 6576 5f69  elf.words[prev_i
+000076c0: 3a69 5d0d 0a20 2020 2020 2020 2020 2020  :i]..           
+000076d0: 206e 6577 5f73 6567 203d 2073 656c 662e   new_seg = self.
+000076e0: 636f 7079 286e 6577 5f77 6f72 6473 2c20  copy(new_words, 
+000076f0: 636f 7079 5f77 6f72 6473 3d46 616c 7365  copy_words=False
+00007700: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00007710: 6567 5f63 6f70 6965 732e 6170 7065 6e64  eg_copies.append
+00007720: 286e 6577 5f73 6567 290d 0a20 2020 2020  (new_seg)..     
+00007730: 2020 2020 2020 2070 7265 765f 6920 3d20         prev_i = 
+00007740: 690d 0a20 2020 2020 2020 2072 6574 7572  i..        retur
+00007750: 6e20 7365 675f 636f 7069 6573 0d0a 0d0a  n seg_copies....
+00007760: 2020 2020 6465 6620 7365 745f 7265 7375      def set_resu
+00007770: 6c74 2873 656c 662c 2072 6573 756c 743a  lt(self, result:
+00007780: 2027 5768 6973 7065 7252 6573 756c 7427   'WhisperResult'
+00007790: 293a 0d0a 2020 2020 2020 2020 7761 726e  ):..        warn
+000077a0: 696e 6773 2e77 6172 6e28 2760 602e 7365  ings.warn('``.se
+000077b0: 745f 7265 7375 6c74 2863 7572 7265 6e74  t_result(current
+000077c0: 5f72 6573 756c 745f 696e 7374 616e 6365  _result_instance
+000077d0: 2960 6020 6973 2064 6570 7265 6361 7465  )`` is deprecate
+000077e0: 6420 616e 6420 7769 6c6c 2062 6520 7265  d and will be re
+000077f0: 6d6f 7665 6420 696e 2066 7574 7572 6520  moved in future 
+00007800: 7665 7273 696f 6e73 2e20 270d 0a20 2020  versions. '..   
+00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007820: 2020 2027 5573 6520 6060 2e72 6573 756c     'Use ``.resul
+00007830: 7420 3d20 6375 7272 656e 745f 7265 7375  t = current_resu
+00007840: 6c74 5f69 6e73 7461 6e63 6560 6020 696e  lt_instance`` in
+00007850: 7374 6561 642e 272c 0d0a 2020 2020 2020  stead.',..      
+00007860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007870: 7374 6163 6b6c 6576 656c 3d32 290d 0a20  stacklevel=2).. 
+00007880: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
+00007890: 6c74 203d 2072 6573 756c 740d 0a0d 0a20  lt = result.... 
+000078a0: 2020 2064 6566 2067 6574 5f72 6573 756c     def get_resul
+000078b0: 7428 7365 6c66 2920 2d3e 2055 6e69 6f6e  t(self) -> Union
+000078c0: 5b27 5768 6973 7065 7252 6573 756c 7427  ['WhisperResult'
+000078d0: 2c20 4e6f 6e65 5d3a 0d0a 2020 2020 2020  , None]:..      
+000078e0: 2020 2222 220d 0a20 2020 2020 2020 2052    """..        R
+000078f0: 6574 7572 6e20 6f75 7465 7220 696e 7374  eturn outer inst
+00007900: 616e 6365 206f 6620 3a63 6c61 7373 3a60  ance of :class:`
+00007910: 7374 6162 6c65 5f77 6869 7370 6572 2e72  stable_whisper.r
+00007920: 6573 756c 742e 5768 6973 7065 7252 6573  esult.WhisperRes
+00007930: 756c 7460 2074 6861 7420 6060 7365 6c66  ult` that ``self
+00007940: 6060 2069 7320 6120 7061 7274 206f 662e  `` is a part of.
+00007950: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00007960: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
+00007970: 7761 726e 2827 6060 2e67 6574 5f72 6573  warn('``.get_res
+00007980: 756c 7428 2960 6020 7769 6c6c 2062 6520  ult()`` will be 
+00007990: 7265 6d6f 7665 6420 696e 2066 7574 7572  removed in futur
+000079a0: 6520 7665 7273 696f 6e73 2e20 5573 6520  e versions. Use 
+000079b0: 6060 2e72 6573 756c 7460 6020 696e 7374  ``.result`` inst
+000079c0: 6561 642e 272c 0d0a 2020 2020 2020 2020  ead.',..        
+000079d0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+000079e0: 6163 6b6c 6576 656c 3d32 290d 0a20 2020  acklevel=2)..   
+000079f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00007a00: 2e72 6573 756c 740d 0a0d 0a0d 0a63 6c61  .result......cla
+00007a10: 7373 2057 6869 7370 6572 5265 7375 6c74  ss WhisperResult
+00007a20: 3a0d 0a0d 0a20 2020 2064 6566 205f 5f69  :....    def __i
+00007a30: 6e69 745f 5f28 0d0a 2020 2020 2020 2020  nit__(..        
+00007a40: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+00007a50: 2020 2020 2020 2072 6573 756c 743a 2055         result: U
+00007a60: 6e69 6f6e 5b73 7472 2c20 6469 6374 2c20  nion[str, dict, 
+00007a70: 6c69 7374 5d2c 0d0a 2020 2020 2020 2020  list],..        
+00007a80: 2020 2020 666f 7263 655f 6f72 6465 723a      force_order:
+00007a90: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
+00007aa0: 2020 2020 2020 2020 2020 2020 6368 6563              chec
+00007ab0: 6b5f 736f 7274 6564 3a20 556e 696f 6e5b  k_sorted: Union[
+00007ac0: 626f 6f6c 2c20 7374 725d 203d 2054 7275  bool, str] = Tru
+00007ad0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00007ae0: 7368 6f77 5f75 6e73 6f72 7465 643a 2062  show_unsorted: b
+00007af0: 6f6f 6c20 3d20 5472 7565 0d0a 2020 2020  ool = True..    
+00007b00: 293a 0d0a 2020 2020 2020 2020 7265 7375  ):..        resu
+00007b10: 6c74 2c20 7365 6c66 2e70 6174 6820 3d20  lt, self.path = 
+00007b20: 7365 6c66 2e5f 7374 616e 6461 7264 697a  self._standardiz
+00007b30: 655f 7265 7375 6c74 2872 6573 756c 7429  e_result(result)
+00007b40: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
+00007b50: 7269 5f64 6963 7420 3d20 7265 7375 6c74  ri_dict = result
+00007b60: 2e67 6574 2827 6f72 695f 6469 6374 2729  .get('ori_dict')
+00007b70: 206f 7220 7265 7375 6c74 0d0a 2020 2020   or result..    
+00007b80: 2020 2020 7365 6c66 2e6c 616e 6775 6167      self.languag
+00007b90: 6520 3d20 7365 6c66 2e6f 7269 5f64 6963  e = self.ori_dic
+00007ba0: 742e 6765 7428 276c 616e 6775 6167 6527  t.get('language'
+00007bb0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007bc0: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
+00007bd0: 203d 2072 6573 756c 742e 6765 7428 2772   = result.get('r
+00007be0: 6567 726f 7570 5f68 6973 746f 7279 272c  egroup_history',
+00007bf0: 2027 2729 0d0a 2020 2020 2020 2020 7365   '')..        se
+00007c00: 6c66 2e5f 6e6f 6e73 7065 6563 685f 7365  lf._nonspeech_se
+00007c10: 6374 696f 6e73 203d 2072 6573 756c 742e  ctions = result.
+00007c20: 6765 7428 276e 6f6e 7370 6565 6368 5f73  get('nonspeech_s
+00007c30: 6563 7469 6f6e 7327 2c20 5b5d 290d 0a20  ections', []).. 
+00007c40: 2020 2020 2020 2073 6567 6d65 6e74 7320         segments 
+00007c50: 3d20 2872 6573 756c 742e 6765 7428 2773  = (result.get('s
+00007c60: 6567 6d65 6e74 7327 2c20 7365 6c66 2e6f  egments', self.o
+00007c70: 7269 5f64 6963 742e 6765 7428 2773 6567  ri_dict.get('seg
+00007c80: 6d65 6e74 7327 2929 206f 7220 7b7d 292e  ments')) or {}).
+00007c90: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
+00007ca0: 7365 6c66 2e73 6567 6d65 6e74 7320 3d20  self.segments = 
+00007cb0: 5b53 6567 6d65 6e74 282a 2a73 2c20 6967  [Segment(**s, ig
+00007cc0: 6e6f 7265 5f75 6e75 7365 645f 6172 6773  nore_unused_args
+00007cd0: 3d54 7275 6529 2066 6f72 2073 2069 6e20  =True) for s in 
+00007ce0: 7365 676d 656e 7473 5d20 6966 2073 6567  segments] if seg
+00007cf0: 6d65 6e74 7320 656c 7365 205b 5d0d 0a20  ments else [].. 
+00007d00: 2020 2020 2020 2073 656c 662e 5f66 6f72         self._for
+00007d10: 6365 645f 6f72 6465 7220 3d20 666f 7263  ced_order = forc
+00007d20: 655f 6f72 6465 720d 0a20 2020 2020 2020  e_order..       
+00007d30: 2069 6620 7365 6c66 2e5f 666f 7263 6564   if self._forced
+00007d40: 5f6f 7264 6572 3a0d 0a20 2020 2020 2020  _order:..       
+00007d50: 2020 2020 2073 656c 662e 666f 7263 655f       self.force_
+00007d60: 6f72 6465 7228 290d 0a20 2020 2020 2020  order()..       
+00007d70: 2073 656c 662e 7261 6973 655f 666f 725f   self.raise_for_
+00007d80: 756e 736f 7274 6564 2863 6865 636b 5f73  unsorted(check_s
+00007d90: 6f72 7465 642c 2073 686f 775f 756e 736f  orted, show_unso
+00007da0: 7274 6564 290d 0a20 2020 2020 2020 2073  rted)..        s
+00007db0: 656c 662e 7265 6d6f 7665 5f6e 6f5f 776f  elf.remove_no_wo
+00007dc0: 7264 5f73 6567 6d65 6e74 7328 616e 7928  rd_segments(any(
+00007dd0: 7365 672e 6861 735f 776f 7264 7320 666f  seg.has_words fo
+00007de0: 7220 7365 6720 696e 2073 656c 662e 7365  r seg in self.se
+00007df0: 676d 656e 7473 2929 0d0a 0d0a 2020 2020  gments))....    
+00007e00: 6465 6620 5f5f 6765 7469 7465 6d5f 5f28  def __getitem__(
+00007e10: 7365 6c66 2c20 696e 6465 783a 2069 6e74  self, index: int
+00007e20: 2920 2d3e 2053 6567 6d65 6e74 3a0d 0a20  ) -> Segment:.. 
+00007e30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00007e40: 6c66 2e73 6567 6d65 6e74 735b 696e 6465  lf.segments[inde
+00007e50: 785d 0d0a 0d0a 2020 2020 6465 6620 5f5f  x]....    def __
+00007e60: 6465 6c69 7465 6d5f 5f28 7365 6c66 2c20  delitem__(self, 
+00007e70: 696e 6465 783a 2069 6e74 293a 0d0a 2020  index: int):..  
+00007e80: 2020 2020 2020 6465 6c20 7365 6c66 2e73        del self.s
+00007e90: 6567 6d65 6e74 735b 696e 6465 785d 0d0a  egments[index]..
+00007ea0: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
+00007eb0: 7373 6967 6e5f 6964 7328 5472 7565 2c20  ssign_ids(True, 
+00007ec0: 7374 6172 743d 696e 6465 7829 0d0a 0d0a  start=index)....
+00007ed0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+00007ee0: 2020 2064 6566 2064 7572 6174 696f 6e28     def duration(
+00007ef0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00007f00: 6966 206e 6f74 2073 656c 662e 7365 676d  if not self.segm
+00007f10: 656e 7473 3a0d 0a20 2020 2020 2020 2020  ents:..         
+00007f20: 2020 2072 6574 7572 6e20 302e 300d 0a20     return 0.0.. 
+00007f30: 2020 2020 2020 2072 6574 7572 6e20 5f72         return _r
+00007f40: 6f75 6e64 5f74 696d 6573 7461 6d70 2873  ound_timestamp(s
+00007f50: 656c 662e 7365 676d 656e 7473 5b2d 315d  elf.segments[-1]
+00007f60: 2e65 6e64 202d 2073 656c 662e 7365 676d  .end - self.segm
+00007f70: 656e 7473 5b30 5d2e 7374 6172 7429 0d0a  ents[0].start)..
+00007f80: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00007f90: 686f 640d 0a20 2020 2064 6566 205f 7374  hod..    def _st
+00007fa0: 616e 6461 7264 697a 655f 7265 7375 6c74  andardize_result
+00007fb0: 2872 6573 756c 743a 2055 6e69 6f6e 5b73  (result: Union[s
+00007fc0: 7472 2c20 6469 6374 2c20 4c69 7374 5b64  tr, dict, List[d
+00007fd0: 6963 745d 2c20 4c69 7374 5b4c 6973 745b  ict], List[List[
+00007fe0: 6469 6374 5d5d 5d29 202d 3e20 5475 706c  dict]]]) -> Tupl
+00007ff0: 655b 6469 6374 2c20 556e 696f 6e5b 7374  e[dict, Union[st
+00008000: 722c 204e 6f6e 655d 5d3a 0d0a 2020 2020  r, None]]:..    
+00008010: 2020 2020 7061 7468 203d 204e 6f6e 650d      path = None.
+00008020: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00008030: 7374 616e 6365 2872 6573 756c 742c 2073  stance(result, s
+00008040: 7472 293a 0d0a 2020 2020 2020 2020 2020  tr):..          
+00008050: 2020 7061 7468 203d 2072 6573 756c 740d    path = result.
+00008060: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00008070: 756c 7420 3d20 6c6f 6164 5f72 6573 756c  ult = load_resul
+00008080: 7428 7061 7468 290d 0a20 2020 2020 2020  t(path)..       
+00008090: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
+000080a0: 6573 756c 742c 2064 6963 7429 3a0d 0a20  esult, dict):.. 
+000080b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000080c0: 6e20 7265 7375 6c74 2c20 7061 7468 0d0a  n result, path..
+000080d0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+000080e0: 7369 6e73 7461 6e63 6528 7265 7375 6c74  sinstance(result
+000080f0: 2c20 6c69 7374 293a 0d0a 2020 2020 2020  , list):..      
+00008100: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
+00008110: 4572 726f 7228 6627 4578 7065 6374 2072  Error(f'Expect r
+00008120: 6573 756c 7420 746f 2062 6520 6c69 7374  esult to be list
+00008130: 2062 7574 2067 6f74 207b 7479 7065 2872   but got {type(r
+00008140: 6573 756c 7429 7d27 290d 0a20 2020 2020  esult)}')..     
+00008150: 2020 2069 6620 6e6f 7420 7265 7375 6c74     if not result
+00008160: 206f 7220 6e6f 7420 7265 7375 6c74 5b30   or not result[0
+00008170: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
+00008180: 7265 7475 726e 207b 7d2c 2070 6174 680d  return {}, path.
+00008190: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+000081a0: 7374 616e 6365 2872 6573 756c 745b 305d  stance(result[0]
+000081b0: 2c20 6c69 7374 293a 0d0a 2020 2020 2020  , list):..      
+000081c0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+000081d0: 6e73 7461 6e63 6528 7265 7375 6c74 5b30  nstance(result[0
+000081e0: 5d5b 305d 2c20 6469 6374 293a 0d0a 2020  ][0], dict):..  
+000081f0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00008200: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+00008210: 6564 4572 726f 7228 6627 476f 7420 6c69  edError(f'Got li
+00008220: 7374 206f 6620 6c69 7374 206f 6620 7b74  st of list of {t
+00008230: 7970 6528 7265 7375 6c74 5b30 5d29 7d20  ype(result[0])} 
+00008240: 6275 7420 6578 7065 6374 7320 6c69 7374  but expects list
+00008250: 206f 6620 6c69 7374 206f 6620 6469 6374   of list of dict
+00008260: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00008270: 7265 7375 6c74 203d 2064 6963 7428 0d0a  result = dict(..
+00008280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008290: 7365 676d 656e 7473 3d5b 0d0a 2020 2020  segments=[..    
+000082a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082b0: 6469 6374 280d 0a20 2020 2020 2020 2020  dict(..         
+000082c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000082d0: 7461 7274 3d77 6f72 6473 5b30 5d5b 2773  tart=words[0]['s
+000082e0: 7461 7274 275d 2c0d 0a20 2020 2020 2020  tart'],..       
+000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008300: 2065 6e64 3d77 6f72 6473 5b2d 315d 5b27   end=words[-1]['
+00008310: 656e 6427 5d2c 0d0a 2020 2020 2020 2020  end'],..        
+00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008330: 7465 7874 3d27 272e 6a6f 696e 2877 5b27  text=''.join(w['
+00008340: 776f 7264 275d 2066 6f72 2077 2069 6e20  word'] for w in 
+00008350: 776f 7264 7329 2c0d 0a20 2020 2020 2020  words),..       
+00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008370: 2077 6f72 6473 3d77 6f72 6473 0d0a 2020   words=words..  
+00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008390: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+000083a0: 2020 2020 2020 2020 2066 6f72 2077 6f72           for wor
+000083b0: 6473 2069 6e20 7265 7375 6c74 2069 6620  ds in result if 
+000083c0: 776f 7264 730d 0a20 2020 2020 2020 2020  words..         
+000083d0: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+000083e0: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+000083f0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00008400: 6365 2872 6573 756c 745b 305d 2c20 6469  ce(result[0], di
+00008410: 6374 293a 0d0a 2020 2020 2020 2020 2020  ct):..          
+00008420: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+00008430: 7365 676d 656e 7473 3d72 6573 756c 7429  segments=result)
+00008440: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00008450: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00008460: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
+00008470: 6445 7272 6f72 2866 2747 6f74 206c 6973  dError(f'Got lis
+00008480: 7420 6f66 207b 7479 7065 2872 6573 756c  t of {type(resul
+00008490: 745b 305d 297d 2062 7574 2065 7870 6563  t[0])} but expec
+000084a0: 7473 206c 6973 7420 6f66 206c 6973 742f  ts list of list/
+000084b0: 6469 6374 2729 0d0a 2020 2020 2020 2020  dict')..        
+000084c0: 7265 7475 726e 2072 6573 756c 742c 2070  return result, p
+000084d0: 6174 680d 0a0d 0a20 2020 2064 6566 2066  ath....    def f
+000084e0: 6f72 6365 5f6f 7264 6572 2873 656c 6629  orce_order(self)
+000084f0: 3a0d 0a20 2020 2020 2020 2070 7265 765f  :..        prev_
+00008500: 7473 5f65 6e64 203d 2030 0d0a 2020 2020  ts_end = 0..    
+00008510: 2020 2020 7469 6d65 7374 616d 7073 203d      timestamps =
+00008520: 2073 656c 662e 616c 6c5f 776f 7264 735f   self.all_words_
+00008530: 6f72 5f73 6567 6d65 6e74 7328 290d 0a20  or_segments().. 
+00008540: 2020 2020 2020 2066 6f72 2069 2c20 7473         for i, ts
+00008550: 2069 6e20 656e 756d 6572 6174 6528 7469   in enumerate(ti
+00008560: 6d65 7374 616d 7073 2c20 3129 3a0d 0a20  mestamps, 1):.. 
+00008570: 2020 2020 2020 2020 2020 2069 6620 7473             if ts
+00008580: 2e73 7461 7274 203c 2070 7265 765f 7473  .start < prev_ts
+00008590: 5f65 6e64 3a0d 0a20 2020 2020 2020 2020  _end:..         
+000085a0: 2020 2020 2020 2074 732e 7374 6172 7420         ts.start 
+000085b0: 3d20 7072 6576 5f74 735f 656e 640d 0a20  = prev_ts_end.. 
+000085c0: 2020 2020 2020 2020 2020 2069 6620 7473             if ts
+000085d0: 2e73 7461 7274 203e 2074 732e 656e 643a  .start > ts.end:
+000085e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000085f0: 2020 6966 2070 7265 765f 7473 5f65 6e64    if prev_ts_end
+00008600: 203e 2074 732e 656e 643a 0d0a 2020 2020   > ts.end:..    
+00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008620: 7761 726e 696e 6773 2e77 6172 6e28 274d  warnings.warn('M
+00008630: 756c 7469 706c 6520 636f 6e73 6563 7574  ultiple consecut
+00008640: 6976 6520 7469 6d65 7374 616d 7073 2061  ive timestamps a
+00008650: 7265 206f 7574 206f 6620 6f72 6465 722e  re out of order.
+00008660: 2053 6f6d 6520 7061 7274 7320 7769 6c6c   Some parts will
+00008670: 2068 6176 6520 6e6f 2064 7572 6174 696f   have no duratio
+00008680: 6e2e 2729 0d0a 2020 2020 2020 2020 2020  n.')..          
+00008690: 2020 2020 2020 2020 2020 7473 2e73 7461            ts.sta
+000086a0: 7274 203d 2074 732e 656e 640d 0a20 2020  rt = ts.end..   
+000086b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086c0: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
+000086d0: 692d 322c 202d 312c 202d 3129 3a0d 0a20  i-2, -1, -1):.. 
+000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086f0: 2020 2020 2020 2069 6620 7469 6d65 7374         if timest
+00008700: 616d 7073 5b6a 5d2e 656e 6420 3e20 7473  amps[j].end > ts
+00008710: 2e65 6e64 3a0d 0a20 2020 2020 2020 2020  .end:..         
+00008720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008730: 2020 2074 696d 6573 7461 6d70 735b 6a5d     timestamps[j]
+00008740: 2e65 6e64 203d 2074 732e 656e 640d 0a20  .end = ts.end.. 
+00008750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008760: 2020 2020 2020 2069 6620 7469 6d65 7374         if timest
+00008770: 616d 7073 5b6a 5d2e 7374 6172 7420 3e20  amps[j].start > 
+00008780: 7473 2e65 6e64 3a0d 0a20 2020 2020 2020  ts.end:..       
+00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087a0: 2020 2020 2074 696d 6573 7461 6d70 735b       timestamps[
+000087b0: 6a5d 2e73 7461 7274 203d 2074 732e 656e  j].start = ts.en
+000087c0: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
+000087d0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+000087e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000087f0: 2074 732e 7374 6172 7420 213d 2070 7265   ts.start != pre
+00008800: 765f 7473 5f65 6e64 3a0d 0a20 2020 2020  v_ts_end:..     
 00008810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008820: 2020 2020 2020 2020 7473 2e65 6e64 203d          ts.end =
-00008830: 2074 732e 7374 6172 7420 6966 2069 203d   ts.start if i =
-00008840: 3d20 6c65 6e28 7469 6d65 7374 616d 7073  = len(timestamps
-00008850: 2920 656c 7365 2074 696d 6573 7461 6d70  ) else timestamp
-00008860: 735b 695d 2e73 7461 7274 0d0a 2020 2020  s[i].start..    
-00008870: 2020 2020 2020 2020 7072 6576 5f74 735f          prev_ts_
-00008880: 656e 6420 3d20 7473 2e65 6e64 0d0a 0d0a  end = ts.end....
-00008890: 2020 2020 6465 6620 7261 6973 655f 666f      def raise_fo
-000088a0: 725f 756e 736f 7274 6564 2873 656c 662c  r_unsorted(self,
-000088b0: 2063 6865 636b 5f73 6f72 7465 643a 2055   check_sorted: U
-000088c0: 6e69 6f6e 5b62 6f6f 6c2c 2073 7472 5d20  nion[bool, str] 
-000088d0: 3d20 5472 7565 2c20 7368 6f77 5f75 6e73  = True, show_uns
-000088e0: 6f72 7465 643a 2062 6f6f 6c20 3d20 5472  orted: bool = Tr
-000088f0: 7565 293a 0d0a 2020 2020 2020 2020 6966  ue):..        if
-00008900: 2063 6865 636b 5f73 6f72 7465 6420 6973   check_sorted is
-00008910: 2046 616c 7365 3a0d 0a20 2020 2020 2020   False:..       
-00008920: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-00008930: 2020 2020 2061 6c6c 5f70 6172 7473 203d       all_parts =
-00008940: 2073 656c 662e 616c 6c5f 776f 7264 735f   self.all_words_
-00008950: 6f72 5f73 6567 6d65 6e74 7328 290d 0a20  or_segments().. 
-00008960: 2020 2020 2020 2069 6620 6e6f 7420 616c         if not al
-00008970: 6c5f 7061 7274 733a 0d0a 2020 2020 2020  l_parts:..      
-00008980: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
-00008990: 2020 2020 2020 6973 5f77 6f72 6420 3d20        is_word = 
-000089a0: 6973 696e 7374 616e 6365 2861 6c6c 5f70  isinstance(all_p
-000089b0: 6172 7473 5b30 5d2c 2057 6f72 6454 696d  arts[0], WordTim
-000089c0: 696e 6729 0d0a 2020 2020 2020 2020 7469  ing)..        ti
-000089d0: 6d65 7374 616d 7073 203d 206e 702e 6172  mestamps = np.ar
-000089e0: 7261 7928 6c69 7374 2863 6861 696e 2e66  ray(list(chain.f
-000089f0: 726f 6d5f 6974 6572 6162 6c65 2828 702e  rom_iterable((p.
-00008a00: 7374 6172 742c 2070 2e65 6e64 2920 666f  start, p.end) fo
-00008a10: 7220 7020 696e 2061 6c6c 5f70 6172 7473  r p in all_parts
-00008a20: 2929 290d 0a20 2020 2020 2020 2069 6620  )))..        if 
-00008a30: 6c65 6e28 7469 6d65 7374 616d 7073 2920  len(timestamps) 
-00008a40: 3e20 3120 616e 6420 2875 6e73 6f72 7465  > 1 and (unsorte
-00008a50: 645f 6d61 736b 203a 3d20 7469 6d65 7374  d_mask := timest
-00008a60: 616d 7073 5b3a 2d31 5d20 3e20 7469 6d65  amps[:-1] > time
-00008a70: 7374 616d 7073 5b31 3a5d 292e 616e 7928  stamps[1:]).any(
-00008a80: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00008a90: 6966 2073 686f 775f 756e 736f 7274 6564  if show_unsorted
-00008aa0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00008ab0: 2020 2064 6566 2067 6574 5f70 6172 745f     def get_part_
-00008ac0: 696e 666f 2869 6478 293a 0d0a 2020 2020  info(idx):..    
-00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ae0: 6375 7272 5f70 6172 7420 3d20 616c 6c5f  curr_part = all_
-00008af0: 7061 7274 735b 6964 785d 0d0a 2020 2020  parts[idx]..    
-00008b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b10: 7365 675f 6964 203d 2063 7572 725f 7061  seg_id = curr_pa
-00008b20: 7274 2e73 6567 6d65 6e74 5f69 6420 6966  rt.segment_id if
-00008b30: 2069 735f 776f 7264 2065 6c73 6520 6375   is_word else cu
-00008b40: 7272 5f70 6172 742e 6964 0d0a 2020 2020  rr_part.id..    
-00008b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b60: 776f 7264 5f69 645f 7374 7220 3d20 6627  word_id_str = f'
-00008b70: 576f 7264 2049 443a 207b 6375 7272 5f70  Word ID: {curr_p
-00008b80: 6172 742e 6964 7d5c 6e27 2069 6620 6973  art.id}\n' if is
-00008b90: 5f77 6f72 6420 656c 7365 2027 270d 0a20  _word else ''.. 
-00008ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bb0: 2020 2072 6574 7572 6e20 280d 0a20 2020     return (..   
-00008bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bd0: 2020 2020 2066 2753 6567 6d65 6e74 2049       f'Segment I
-00008be0: 443a 207b 7365 675f 6964 7d5c 6e7b 776f  D: {seg_id}\n{wo
-00008bf0: 7264 5f69 645f 7374 727d 270d 0a20 2020  rd_id_str}'..   
-00008c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c10: 2020 2020 2066 2753 7461 7274 3a20 7b63       f'Start: {c
-00008c20: 7572 725f 7061 7274 2e73 7461 7274 7d5c  urr_part.start}\
-00008c30: 6e45 6e64 3a20 7b63 7572 725f 7061 7274  nEnd: {curr_part
-00008c40: 2e65 6e64 7d5c 6e27 0d0a 2020 2020 2020  .end}\n'..      
-00008c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c60: 2020 6627 5465 7874 3a20 227b 6375 7272    f'Text: "{curr
-00008c70: 5f70 6172 742e 776f 7264 2069 6620 6973  _part.word if is
-00008c80: 5f77 6f72 6420 656c 7365 2063 7572 725f  _word else curr_
-00008c90: 7061 7274 2e74 6578 747d 2227 0d0a 2020  part.text}"'..  
-00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cb0: 2020 292c 2063 7572 725f 7061 7274 2e73    ), curr_part.s
-00008cc0: 7461 7274 2c20 6375 7272 5f70 6172 742e  tart, curr_part.
-00008cd0: 656e 640d 0a0d 0a20 2020 2020 2020 2020  end....         
-00008ce0: 2020 2020 2020 2066 6f72 2069 2c20 756e         for i, un
-00008cf0: 736f 7274 6564 2069 6e20 656e 756d 6572  sorted in enumer
-00008d00: 6174 6528 756e 736f 7274 6564 5f6d 6173  ate(unsorted_mas
-00008d10: 6b2c 2032 293a 0d0a 2020 2020 2020 2020  k, 2):..        
-00008d20: 2020 2020 2020 2020 2020 2020 6966 2075              if u
-00008d30: 6e73 6f72 7465 643a 0d0a 2020 2020 2020  nsorted:..      
-00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d50: 2020 776f 7264 5f69 6420 3d20 692f 2f32    word_id = i//2
-00008d60: 2d31 0d0a 2020 2020 2020 2020 2020 2020  -1..            
-00008d70: 2020 2020 2020 2020 2020 2020 7061 7274              part
-00008d80: 5f69 6e66 6f2c 2073 7461 7274 2c20 656e  _info, start, en
-00008d90: 6420 3d20 6765 745f 7061 7274 5f69 6e66  d = get_part_inf
-00008da0: 6f28 776f 7264 5f69 6429 0d0a 2020 2020  o(word_id)..    
+00008820: 2020 2074 732e 7374 6172 7420 3d20 7072     ts.start = pr
+00008830: 6576 5f74 735f 656e 640d 0a20 2020 2020  ev_ts_end..     
+00008840: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00008850: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00008860: 2020 2020 2020 2020 2020 2020 2020 7473                ts
+00008870: 2e65 6e64 203d 2074 732e 7374 6172 7420  .end = ts.start 
+00008880: 6966 2069 203d 3d20 6c65 6e28 7469 6d65  if i == len(time
+00008890: 7374 616d 7073 2920 656c 7365 2074 696d  stamps) else tim
+000088a0: 6573 7461 6d70 735b 695d 2e73 7461 7274  estamps[i].start
+000088b0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+000088c0: 6576 5f74 735f 656e 6420 3d20 7473 2e65  ev_ts_end = ts.e
+000088d0: 6e64 0d0a 0d0a 2020 2020 6465 6620 7261  nd....    def ra
+000088e0: 6973 655f 666f 725f 756e 736f 7274 6564  ise_for_unsorted
+000088f0: 2873 656c 662c 2063 6865 636b 5f73 6f72  (self, check_sor
+00008900: 7465 643a 2055 6e69 6f6e 5b62 6f6f 6c2c  ted: Union[bool,
+00008910: 2073 7472 5d20 3d20 5472 7565 2c20 7368   str] = True, sh
+00008920: 6f77 5f75 6e73 6f72 7465 643a 2062 6f6f  ow_unsorted: boo
+00008930: 6c20 3d20 5472 7565 293a 0d0a 2020 2020  l = True):..    
+00008940: 2020 2020 6966 2063 6865 636b 5f73 6f72      if check_sor
+00008950: 7465 6420 6973 2046 616c 7365 3a0d 0a20  ted is False:.. 
+00008960: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00008970: 6e0d 0a20 2020 2020 2020 2061 6c6c 5f70  n..        all_p
+00008980: 6172 7473 203d 2073 656c 662e 616c 6c5f  arts = self.all_
+00008990: 776f 7264 735f 6f72 5f73 6567 6d65 6e74  words_or_segment
+000089a0: 7328 290d 0a20 2020 2020 2020 2069 6620  s()..        if 
+000089b0: 6e6f 7420 616c 6c5f 7061 7274 733a 0d0a  not all_parts:..
+000089c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000089d0: 726e 0d0a 2020 2020 2020 2020 6973 5f77  rn..        is_w
+000089e0: 6f72 6420 3d20 6973 696e 7374 616e 6365  ord = isinstance
+000089f0: 2861 6c6c 5f70 6172 7473 5b30 5d2c 2057  (all_parts[0], W
+00008a00: 6f72 6454 696d 696e 6729 0d0a 2020 2020  ordTiming)..    
+00008a10: 2020 2020 7469 6d65 7374 616d 7073 203d      timestamps =
+00008a20: 206e 702e 6172 7261 7928 6c69 7374 2863   np.array(list(c
+00008a30: 6861 696e 2e66 726f 6d5f 6974 6572 6162  hain.from_iterab
+00008a40: 6c65 2828 702e 7374 6172 742c 2070 2e65  le((p.start, p.e
+00008a50: 6e64 2920 666f 7220 7020 696e 2061 6c6c  nd) for p in all
+00008a60: 5f70 6172 7473 2929 290d 0a20 2020 2020  _parts)))..     
+00008a70: 2020 2069 6620 6c65 6e28 7469 6d65 7374     if len(timest
+00008a80: 616d 7073 2920 3e20 3120 616e 6420 2875  amps) > 1 and (u
+00008a90: 6e73 6f72 7465 645f 6d61 736b 203a 3d20  nsorted_mask := 
+00008aa0: 7469 6d65 7374 616d 7073 5b3a 2d31 5d20  timestamps[:-1] 
+00008ab0: 3e20 7469 6d65 7374 616d 7073 5b31 3a5d  > timestamps[1:]
+00008ac0: 292e 616e 7928 293a 0d0a 2020 2020 2020  ).any():..      
+00008ad0: 2020 2020 2020 6966 2073 686f 775f 756e        if show_un
+00008ae0: 736f 7274 6564 3a0d 0a20 2020 2020 2020  sorted:..       
+00008af0: 2020 2020 2020 2020 2064 6566 2067 6574           def get
+00008b00: 5f70 6172 745f 696e 666f 2869 6478 293a  _part_info(idx):
+00008b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008b20: 2020 2020 2020 6375 7272 5f70 6172 7420        curr_part 
+00008b30: 3d20 616c 6c5f 7061 7274 735b 6964 785d  = all_parts[idx]
+00008b40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008b50: 2020 2020 2020 7365 675f 6964 203d 2063        seg_id = c
+00008b60: 7572 725f 7061 7274 2e73 6567 6d65 6e74  urr_part.segment
+00008b70: 5f69 6420 6966 2069 735f 776f 7264 2065  _id if is_word e
+00008b80: 6c73 6520 6375 7272 5f70 6172 742e 6964  lse curr_part.id
+00008b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008ba0: 2020 2020 2020 776f 7264 5f69 645f 7374        word_id_st
+00008bb0: 7220 3d20 6627 576f 7264 2049 443a 207b  r = f'Word ID: {
+00008bc0: 6375 7272 5f70 6172 742e 6964 7d5c 6e27  curr_part.id}\n'
+00008bd0: 2069 6620 6973 5f77 6f72 6420 656c 7365   if is_word else
+00008be0: 2027 270d 0a20 2020 2020 2020 2020 2020   ''..           
+00008bf0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008c00: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00008c10: 2020 2020 2020 2020 2020 2066 2753 6567             f'Seg
+00008c20: 6d65 6e74 2049 443a 207b 7365 675f 6964  ment ID: {seg_id
+00008c30: 7d5c 6e7b 776f 7264 5f69 645f 7374 727d  }\n{word_id_str}
+00008c40: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
+00008c50: 2020 2020 2020 2020 2020 2066 2753 7461             f'Sta
+00008c60: 7274 3a20 7b63 7572 725f 7061 7274 2e73  rt: {curr_part.s
+00008c70: 7461 7274 7d5c 6e45 6e64 3a20 7b63 7572  tart}\nEnd: {cur
+00008c80: 725f 7061 7274 2e65 6e64 7d5c 6e27 0d0a  r_part.end}\n'..
+00008c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ca0: 2020 2020 2020 2020 6627 5465 7874 3a20          f'Text: 
+00008cb0: 227b 6375 7272 5f70 6172 742e 776f 7264  "{curr_part.word
+00008cc0: 2069 6620 6973 5f77 6f72 6420 656c 7365   if is_word else
+00008cd0: 2063 7572 725f 7061 7274 2e74 6578 747d   curr_part.text}
+00008ce0: 2227 0d0a 2020 2020 2020 2020 2020 2020  "'..            
+00008cf0: 2020 2020 2020 2020 292c 2063 7572 725f          ), curr_
+00008d00: 7061 7274 2e73 7461 7274 2c20 6375 7272  part.start, curr
+00008d10: 5f70 6172 742e 656e 640d 0a0d 0a20 2020  _part.end....   
+00008d20: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00008d30: 2069 2c20 756e 736f 7274 6564 2069 6e20   i, unsorted in 
+00008d40: 656e 756d 6572 6174 6528 756e 736f 7274  enumerate(unsort
+00008d50: 6564 5f6d 6173 6b2c 2032 293a 0d0a 2020  ed_mask, 2):..  
+00008d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d70: 2020 6966 2075 6e73 6f72 7465 643a 0d0a    if unsorted:..
+00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d90: 2020 2020 2020 2020 776f 7264 5f69 6420          word_id 
+00008da0: 3d20 692f 2f32 2d31 0d0a 2020 2020 2020  = i//2-1..      
 00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dc0: 2020 2020 6966 2069 2025 2032 203d 3d20      if i % 2 == 
-00008dd0: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008df0: 6e65 7874 5f69 6e66 6f2c 206e 6578 745f  next_info, next_
-00008e00: 7374 6172 742c 205f 203d 2067 6574 5f70  start, _ = get_p
-00008e10: 6172 745f 696e 666f 2877 6f72 645f 6964  art_info(word_id
-00008e20: 2b31 290d 0a20 2020 2020 2020 2020 2020  +1)..           
-00008e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e40: 2070 6172 745f 696e 666f 202b 3d20 6627   part_info += f'
-00008e50: 5c6e 436f 6e66 6c69 6374 3a20 656e 6420  \nConflict: end 
-00008e60: 287b 656e 647d 2920 3e20 6e65 7874 2073  ({end}) > next s
-00008e70: 7461 7274 2028 7b6e 6578 745f 7374 6172  tart ({next_star
-00008e80: 747d 295c 6e7b 6e65 7874 5f69 6e66 6f7d  t})\n{next_info}
-00008e90: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00008ea0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00008eb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008ec0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00008ed0: 7274 5f69 6e66 6f20 2b3d 2066 275c 6e43  rt_info += f'\nC
-00008ee0: 6f6e 666c 6963 743a 2073 7461 7274 2028  onflict: start (
-00008ef0: 7b73 7461 7274 7d29 203e 2065 6e64 2028  {start}) > end (
-00008f00: 7b65 6e64 7d29 270d 0a20 2020 2020 2020  {end})'..       
-00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f20: 2070 7269 6e74 2870 6172 745f 696e 666f   print(part_info
-00008f30: 2c20 656e 643d 275c 6e5c 6e27 290d 0a0d  , end='\n\n')...
-00008f40: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00008f50: 6120 3d20 7365 6c66 2e74 6f5f 6469 6374  a = self.to_dict
-00008f60: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00008f70: 6966 2063 6865 636b 5f73 6f72 7465 6420  if check_sorted 
-00008f80: 6973 2054 7275 653a 0d0a 2020 2020 2020  is True:..      
-00008f90: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00008fa0: 556e 736f 7274 6564 4578 6365 7074 696f  UnsortedExceptio
-00008fb0: 6e28 6461 7461 3d64 6174 6129 0d0a 2020  n(data=data)..  
-00008fc0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-00008fd0: 6773 2e77 6172 6e28 2754 696d 6573 7461  gs.warn('Timesta
-00008fe0: 6d70 7320 6172 6520 6e6f 7420 696e 2061  mps are not in a
-00008ff0: 7363 656e 6469 6e67 206f 7264 6572 2e20  scending order. 
-00009000: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00009010: 2020 2020 2020 2020 2020 2020 2027 4966               'If
-00009020: 2064 6174 6120 6973 2070 726f 6475 6365   data is produce
-00009030: 6420 6279 2053 7461 626c 652d 7473 2c20  d by Stable-ts, 
-00009040: 706c 6561 7365 2073 7562 6d69 7420 616e  please submit an
-00009050: 2069 7373 7565 2077 6974 6820 7468 6520   issue with the 
-00009060: 7361 7665 6420 6461 7461 2e27 290d 0a20  saved data.').. 
-00009070: 2020 2020 2020 2020 2020 2073 6176 655f             save_
-00009080: 6173 5f6a 736f 6e28 6461 7461 2c20 6368  as_json(data, ch
-00009090: 6563 6b5f 736f 7274 6564 290d 0a0d 0a20  eck_sorted).... 
-000090a0: 2020 2064 6566 2075 7064 6174 655f 616c     def update_al
-000090b0: 6c5f 7365 6773 5f77 6974 685f 776f 7264  l_segs_with_word
-000090c0: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
-000090d0: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-000090e0: 2741 7474 7269 6275 7465 7320 7468 6174  'Attributes that
-000090f0: 2072 6571 7569 7265 6420 7570 6461 7469   required updati
-00009100: 6e67 2061 7265 206e 6f77 2070 726f 7065  ng are now prope
-00009110: 7274 6965 7320 6261 7365 6420 6f6e 2074  rties based on t
-00009120: 6865 2060 6077 6f72 6473 6060 2065 7863  he ``words`` exc
-00009130: 6570 7420 666f 7220 6060 6964 6060 2e20  ept for ``id``. 
-00009140: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00009150: 2020 2020 2020 2020 2027 6060 7570 6461           '``upda
-00009160: 7465 5f61 6c6c 5f73 6567 735f 7769 7468  te_all_segs_with
-00009170: 5f77 6f72 6473 2829 6060 2069 7320 6465  _words()`` is de
-00009180: 7072 6563 6174 6564 2061 6e64 2077 696c  precated and wil
-00009190: 6c20 6265 2072 656d 6f76 6564 2069 6e20  l be removed in 
-000091a0: 6675 7475 7265 2076 6572 7369 6f6e 732e  future versions.
-000091b0: 2027 0d0a 2020 2020 2020 2020 2020 2020   '..            
-000091c0: 2020 2020 2020 2020 2020 2755 7365 2060            'Use `
-000091d0: 602e 7265 6173 7369 676e 5f69 6473 2829  `.reassign_ids()
-000091e0: 6060 2074 6f20 6d61 6e75 616c 6c79 2075  `` to manually u
-000091f0: 7064 6174 6520 6964 7327 2c0d 0a20 2020  pdate ids',..   
+00008dc0: 2020 7061 7274 5f69 6e66 6f2c 2073 7461    part_info, sta
+00008dd0: 7274 2c20 656e 6420 3d20 6765 745f 7061  rt, end = get_pa
+00008de0: 7274 5f69 6e66 6f28 776f 7264 5f69 6429  rt_info(word_id)
+00008df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008e00: 2020 2020 2020 2020 2020 6966 2069 2025            if i %
+00008e10: 2032 203d 3d20 313a 0d0a 2020 2020 2020   2 == 1:..      
+00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e30: 2020 2020 2020 6e65 7874 5f69 6e66 6f2c        next_info,
+00008e40: 206e 6578 745f 7374 6172 742c 205f 203d   next_start, _ =
+00008e50: 2067 6574 5f70 6172 745f 696e 666f 2877   get_part_info(w
+00008e60: 6f72 645f 6964 2b31 290d 0a20 2020 2020  ord_id+1)..     
+00008e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e80: 2020 2020 2020 2070 6172 745f 696e 666f         part_info
+00008e90: 202b 3d20 6627 5c6e 436f 6e66 6c69 6374   += f'\nConflict
+00008ea0: 3a20 656e 6420 287b 656e 647d 2920 3e20  : end ({end}) > 
+00008eb0: 6e65 7874 2073 7461 7274 2028 7b6e 6578  next start ({nex
+00008ec0: 745f 7374 6172 747d 295c 6e7b 6e65 7874  t_start})\n{next
+00008ed0: 5f69 6e66 6f7d 270d 0a20 2020 2020 2020  _info}'..       
+00008ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ef0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00008f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f10: 2020 2020 7061 7274 5f69 6e66 6f20 2b3d      part_info +=
+00008f20: 2066 275c 6e43 6f6e 666c 6963 743a 2073   f'\nConflict: s
+00008f30: 7461 7274 2028 7b73 7461 7274 7d29 203e  tart ({start}) >
+00008f40: 2065 6e64 2028 7b65 6e64 7d29 270d 0a20   end ({end})'.. 
+00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f60: 2020 2020 2020 2070 7269 6e74 2870 6172         print(par
+00008f70: 745f 696e 666f 2c20 656e 643d 275c 6e5c  t_info, end='\n\
+00008f80: 6e27 290d 0a0d 0a20 2020 2020 2020 2020  n')....         
+00008f90: 2020 2064 6174 6120 3d20 7365 6c66 2e74     data = self.t
+00008fa0: 6f5f 6469 6374 2829 0d0a 2020 2020 2020  o_dict()..      
+00008fb0: 2020 2020 2020 6966 2063 6865 636b 5f73        if check_s
+00008fc0: 6f72 7465 6420 6973 2054 7275 653a 0d0a  orted is True:..
+00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fe0: 7261 6973 6520 556e 736f 7274 6564 4578  raise UnsortedEx
+00008ff0: 6365 7074 696f 6e28 6461 7461 3d64 6174  ception(data=dat
+00009000: 6129 0d0a 2020 2020 2020 2020 2020 2020  a)..            
+00009010: 7761 726e 696e 6773 2e77 6172 6e28 2754  warnings.warn('T
+00009020: 696d 6573 7461 6d70 7320 6172 6520 6e6f  imestamps are no
+00009030: 7420 696e 2061 7363 656e 6469 6e67 206f  t in ascending o
+00009040: 7264 6572 2e20 270d 0a20 2020 2020 2020  rder. '..       
+00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009060: 2020 2027 4966 2064 6174 6120 6973 2070     'If data is p
+00009070: 726f 6475 6365 6420 6279 2053 7461 626c  roduced by Stabl
+00009080: 652d 7473 2c20 706c 6561 7365 2073 7562  e-ts, please sub
+00009090: 6d69 7420 616e 2069 7373 7565 2077 6974  mit an issue wit
+000090a0: 6820 7468 6520 7361 7665 6420 6461 7461  h the saved data
+000090b0: 2e27 290d 0a20 2020 2020 2020 2020 2020  .')..           
+000090c0: 2073 6176 655f 6173 5f6a 736f 6e28 6461   save_as_json(da
+000090d0: 7461 2c20 6368 6563 6b5f 736f 7274 6564  ta, check_sorted
+000090e0: 290d 0a0d 0a20 2020 2064 6566 2075 7064  )....    def upd
+000090f0: 6174 655f 616c 6c5f 7365 6773 5f77 6974  ate_all_segs_wit
+00009100: 685f 776f 7264 7328 7365 6c66 293a 0d0a  h_words(self):..
+00009110: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
+00009120: 2e77 6172 6e28 2741 7474 7269 6275 7465  .warn('Attribute
+00009130: 7320 7468 6174 2072 6571 7569 7265 6420  s that required 
+00009140: 7570 6461 7469 6e67 2061 7265 206e 6f77  updating are now
+00009150: 2070 726f 7065 7274 6965 7320 6261 7365   properties base
+00009160: 6420 6f6e 2074 6865 2060 6077 6f72 6473  d on the ``words
+00009170: 6060 2065 7863 6570 7420 666f 7220 6060  `` except for ``
+00009180: 6964 6060 2e20 270d 0a20 2020 2020 2020  id``. '..       
+00009190: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000091a0: 6060 7570 6461 7465 5f61 6c6c 5f73 6567  ``update_all_seg
+000091b0: 735f 7769 7468 5f77 6f72 6473 2829 6060  s_with_words()``
+000091c0: 2069 7320 6465 7072 6563 6174 6564 2061   is deprecated a
+000091d0: 6e64 2077 696c 6c20 6265 2072 656d 6f76  nd will be remov
+000091e0: 6564 2069 6e20 6675 7475 7265 2076 6572  ed in future ver
+000091f0: 7369 6f6e 732e 2027 0d0a 2020 2020 2020  sions. '..      
 00009200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009210: 2020 2073 7461 636b 6c65 7665 6c3d 3229     stacklevel=2)
-00009220: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-00009230: 6561 7373 6967 6e5f 6964 7328 290d 0a0d  eassign_ids()...
-00009240: 0a20 2020 2064 6566 2075 7064 6174 655f  .    def update_
-00009250: 6e6f 6e73 7065 6563 685f 7365 6374 696f  nonspeech_sectio
-00009260: 6e73 2873 656c 662c 2073 696c 656e 745f  ns(self, silent_
-00009270: 7374 6172 7473 2c20 7369 6c65 6e74 5f65  starts, silent_e
-00009280: 6e64 7329 3a0d 0a20 2020 2020 2020 2073  nds):..        s
-00009290: 656c 662e 5f6e 6f6e 7370 6565 6368 5f73  elf._nonspeech_s
-000092a0: 6563 7469 6f6e 7320 3d20 5b0d 0a20 2020  ections = [..   
-000092b0: 2020 2020 2020 2020 2064 6963 7428 7374           dict(st
-000092c0: 6172 743d 726f 756e 6428 732c 2033 292c  art=round(s, 3),
-000092d0: 2065 6e64 3d72 6f75 6e64 2865 2c20 3329   end=round(e, 3)
-000092e0: 2920 666f 7220 732c 2065 2069 6e20 7a69  ) for s, e in zi
-000092f0: 7028 7369 6c65 6e74 5f73 7461 7274 732c  p(silent_starts,
-00009300: 2073 696c 656e 745f 656e 6473 290d 0a20   silent_ends).. 
-00009310: 2020 2020 2020 205d 0d0a 0d0a 2020 2020         ]....    
-00009320: 6465 6620 6164 645f 7365 676d 656e 7473  def add_segments
-00009330: 2873 656c 662c 2069 6e64 6578 303a 2069  (self, index0: i
-00009340: 6e74 2c20 696e 6465 7831 3a20 696e 742c  nt, index1: int,
-00009350: 2069 6e70 6c61 6365 3a20 626f 6f6c 203d   inplace: bool =
-00009360: 2046 616c 7365 2c20 6c6f 636b 3a20 626f   False, lock: bo
-00009370: 6f6c 203d 2046 616c 7365 293a 0d0a 2020  ol = False):..  
-00009380: 2020 2020 2020 6e65 775f 7365 6720 3d20        new_seg = 
-00009390: 7365 6c66 2e73 6567 6d65 6e74 735b 696e  self.segments[in
-000093a0: 6465 7830 5d2e 6164 6428 7365 6c66 2e73  dex0].add(self.s
-000093b0: 6567 6d65 6e74 735b 696e 6465 7831 5d2c  egments[index1],
-000093c0: 2063 6f70 795f 776f 7264 733d 4661 6c73   copy_words=Fals
-000093d0: 6529 0d0a 2020 2020 2020 2020 6966 206c  e)..        if l
-000093e0: 6f63 6b20 616e 6420 7365 6c66 2e73 6567  ock and self.seg
-000093f0: 6d65 6e74 735b 696e 6465 7830 5d2e 6861  ments[index0].ha
-00009400: 735f 776f 7264 733a 0d0a 2020 2020 2020  s_words:..      
-00009410: 2020 2020 2020 6c6f 636b 5f69 6478 203d        lock_idx =
-00009420: 206c 656e 2873 656c 662e 7365 676d 656e   len(self.segmen
-00009430: 7473 5b69 6e64 6578 305d 2e77 6f72 6473  ts[index0].words
-00009440: 290d 0a20 2020 2020 2020 2020 2020 206e  )..            n
-00009450: 6577 5f73 6567 2e77 6f72 6473 5b6c 6f63  ew_seg.words[loc
-00009460: 6b5f 6964 7820 2d20 315d 2e6c 6f63 6b5f  k_idx - 1].lock_
-00009470: 7269 6768 7428 290d 0a20 2020 2020 2020  right()..       
-00009480: 2020 2020 2069 6620 6c6f 636b 5f69 6478       if lock_idx
-00009490: 203c 206c 656e 286e 6577 5f73 6567 2e77   < len(new_seg.w
-000094a0: 6f72 6473 293a 0d0a 2020 2020 2020 2020  ords):..        
-000094b0: 2020 2020 2020 2020 6e65 775f 7365 672e          new_seg.
-000094c0: 776f 7264 735b 6c6f 636b 5f69 6478 5d2e  words[lock_idx].
-000094d0: 6c6f 636b 5f6c 6566 7428 290d 0a20 2020  lock_left()..   
-000094e0: 2020 2020 2069 6620 696e 706c 6163 653a       if inplace:
-000094f0: 0d0a 2020 2020 2020 2020 2020 2020 6930  ..            i0
-00009500: 2c20 6931 203d 2073 6f72 7465 6428 5b69  , i1 = sorted([i
-00009510: 6e64 6578 302c 2069 6e64 6578 315d 290d  ndex0, index1]).
-00009520: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00009530: 662e 7365 676d 656e 7473 5b69 305d 203d  f.segments[i0] =
-00009540: 206e 6577 5f73 6567 0d0a 2020 2020 2020   new_seg..      
-00009550: 2020 2020 2020 6465 6c20 7365 6c66 2e73        del self.s
-00009560: 6567 6d65 6e74 735b 6931 5d0d 0a20 2020  egments[i1]..   
-00009570: 2020 2020 2072 6574 7572 6e20 6e65 775f       return new_
-00009580: 7365 670d 0a0d 0a20 2020 2064 6566 2072  seg....    def r
-00009590: 6573 6361 6c65 5f74 696d 6528 7365 6c66  escale_time(self
-000095a0: 2c20 7363 616c 655f 6661 6374 6f72 3a20  , scale_factor: 
-000095b0: 666c 6f61 7429 3a0d 0a20 2020 2020 2020  float):..       
-000095c0: 2066 6f72 2073 2069 6e20 7365 6c66 2e73   for s in self.s
-000095d0: 6567 6d65 6e74 733a 0d0a 2020 2020 2020  egments:..      
-000095e0: 2020 2020 2020 732e 7265 7363 616c 655f        s.rescale_
-000095f0: 7469 6d65 2873 6361 6c65 5f66 6163 746f  time(scale_facto
-00009600: 7229 0d0a 0d0a 2020 2020 6465 6620 6170  r)....    def ap
-00009610: 706c 795f 6d69 6e5f 6475 7228 7365 6c66  ply_min_dur(self
-00009620: 2c20 6d69 6e5f 6475 723a 2066 6c6f 6174  , min_dur: float
-00009630: 2c20 696e 706c 6163 653a 2062 6f6f 6c20  , inplace: bool 
-00009640: 3d20 4661 6c73 6529 3a0d 0a20 2020 2020  = False):..     
-00009650: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00009660: 4d65 7267 6520 616e 7920 776f 7264 2f73  Merge any word/s
-00009670: 6567 6d65 6e74 2077 6974 6820 6164 6a61  egment with adja
-00009680: 6365 6e74 2077 6f72 642f 7365 676d 656e  cent word/segmen
-00009690: 7420 6966 2069 7473 2064 7572 6174 696f  t if its duratio
-000096a0: 6e20 6973 206c 6573 7320 7468 616e 2060  n is less than `
-000096b0: 606d 696e 5f64 7572 6060 2e0d 0a20 2020  `min_dur``...   
-000096c0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000096d0: 2020 7265 7375 6c74 203d 2073 656c 6620    result = self 
-000096e0: 6966 2069 6e70 6c61 6365 2065 6c73 6520  if inplace else 
-000096f0: 6465 6570 636f 7079 2873 656c 6629 0d0a  deepcopy(self)..
-00009700: 2020 2020 2020 2020 6d61 785f 6920 3d20          max_i = 
-00009710: 6c65 6e28 7265 7375 6c74 2e73 6567 6d65  len(result.segme
-00009720: 6e74 7329 202d 2031 0d0a 2020 2020 2020  nts) - 1..      
-00009730: 2020 6966 206d 6178 5f69 203d 3d20 303a    if max_i == 0:
-00009740: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00009750: 7475 726e 2072 6573 756c 740d 0a20 2020  turn result..   
-00009760: 2020 2020 2066 6f72 2069 2069 6e20 7265       for i in re
-00009770: 7665 7273 6564 2872 616e 6765 286c 656e  versed(range(len
-00009780: 2872 6573 756c 742e 7365 676d 656e 7473  (result.segments
-00009790: 2929 293a 0d0a 2020 2020 2020 2020 2020  ))):..          
-000097a0: 2020 6966 206d 6178 5f69 203d 3d20 303a    if max_i == 0:
-000097b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000097c0: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
-000097d0: 2020 2020 2069 6620 7265 7375 6c74 2e73       if result.s
-000097e0: 6567 6d65 6e74 735b 695d 2e64 7572 6174  egments[i].durat
-000097f0: 696f 6e20 3c20 6d69 6e5f 6475 723a 0d0a  ion < min_dur:..
-00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009810: 6966 2069 203d 3d20 6d61 785f 693a 0d0a  if i == max_i:..
-00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009830: 2020 2020 7265 7375 6c74 2e61 6464 5f73      result.add_s
-00009840: 6567 6d65 6e74 7328 692d 312c 2069 2c20  egments(i-1, i, 
-00009850: 696e 706c 6163 653d 5472 7565 290d 0a20  inplace=True).. 
-00009860: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00009870: 6c69 6620 6920 3d3d 2030 3a0d 0a20 2020  lif i == 0:..   
-00009880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009890: 2072 6573 756c 742e 6164 645f 7365 676d   result.add_segm
-000098a0: 656e 7473 2869 2c20 692b 312c 2069 6e70  ents(i, i+1, inp
-000098b0: 6c61 6365 3d54 7275 6529 0d0a 2020 2020  lace=True)..    
-000098c0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000098d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000098e0: 2020 2020 2020 2069 6620 7265 7375 6c74         if result
-000098f0: 2e73 6567 6d65 6e74 735b 692b 315d 2e64  .segments[i+1].d
-00009900: 7572 6174 696f 6e20 3c20 7265 7375 6c74  uration < result
-00009910: 2e73 6567 6d65 6e74 735b 692d 315d 2e64  .segments[i-1].d
-00009920: 7572 6174 696f 6e3a 0d0a 2020 2020 2020  uration:..      
-00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009940: 2020 7265 7375 6c74 2e61 6464 5f73 6567    result.add_seg
-00009950: 6d65 6e74 7328 692d 312c 2069 2c20 696e  ments(i-1, i, in
-00009960: 706c 6163 653d 5472 7565 290d 0a20 2020  place=True)..   
+00009210: 2755 7365 2060 602e 7265 6173 7369 676e  'Use ``.reassign
+00009220: 5f69 6473 2829 6060 2074 6f20 6d61 6e75  _ids()`` to manu
+00009230: 616c 6c79 2075 7064 6174 6520 6964 7327  ally update ids'
+00009240: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009250: 2020 2020 2020 2020 2073 7461 636b 6c65           stackle
+00009260: 7665 6c3d 3229 0d0a 2020 2020 2020 2020  vel=2)..        
+00009270: 7365 6c66 2e72 6561 7373 6967 6e5f 6964  self.reassign_id
+00009280: 7328 290d 0a0d 0a20 2020 2064 6566 2075  s()....    def u
+00009290: 7064 6174 655f 6e6f 6e73 7065 6563 685f  pdate_nonspeech_
+000092a0: 7365 6374 696f 6e73 2873 656c 662c 2073  sections(self, s
+000092b0: 696c 656e 745f 7374 6172 7473 2c20 7369  ilent_starts, si
+000092c0: 6c65 6e74 5f65 6e64 7329 3a0d 0a20 2020  lent_ends):..   
+000092d0: 2020 2020 2073 656c 662e 5f6e 6f6e 7370       self._nonsp
+000092e0: 6565 6368 5f73 6563 7469 6f6e 7320 3d20  eech_sections = 
+000092f0: 5b0d 0a20 2020 2020 2020 2020 2020 2064  [..            d
+00009300: 6963 7428 7374 6172 743d 726f 756e 6428  ict(start=round(
+00009310: 732c 2033 292c 2065 6e64 3d72 6f75 6e64  s, 3), end=round
+00009320: 2865 2c20 3329 2920 666f 7220 732c 2065  (e, 3)) for s, e
+00009330: 2069 6e20 7a69 7028 7369 6c65 6e74 5f73   in zip(silent_s
+00009340: 7461 7274 732c 2073 696c 656e 745f 656e  tarts, silent_en
+00009350: 6473 290d 0a20 2020 2020 2020 205d 0d0a  ds)..        ]..
+00009360: 0d0a 2020 2020 6465 6620 6164 645f 7365  ..    def add_se
+00009370: 676d 656e 7473 2873 656c 662c 2069 6e64  gments(self, ind
+00009380: 6578 303a 2069 6e74 2c20 696e 6465 7831  ex0: int, index1
+00009390: 3a20 696e 742c 2069 6e70 6c61 6365 3a20  : int, inplace: 
+000093a0: 626f 6f6c 203d 2046 616c 7365 2c20 6c6f  bool = False, lo
+000093b0: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
+000093c0: 293a 0d0a 2020 2020 2020 2020 6e65 775f  ):..        new_
+000093d0: 7365 6720 3d20 7365 6c66 2e73 6567 6d65  seg = self.segme
+000093e0: 6e74 735b 696e 6465 7830 5d2e 6164 6428  nts[index0].add(
+000093f0: 7365 6c66 2e73 6567 6d65 6e74 735b 696e  self.segments[in
+00009400: 6465 7831 5d2c 2063 6f70 795f 776f 7264  dex1], copy_word
+00009410: 733d 4661 6c73 6529 0d0a 2020 2020 2020  s=False)..      
+00009420: 2020 6966 206c 6f63 6b20 616e 6420 7365    if lock and se
+00009430: 6c66 2e73 6567 6d65 6e74 735b 696e 6465  lf.segments[inde
+00009440: 7830 5d2e 6861 735f 776f 7264 733a 0d0a  x0].has_words:..
+00009450: 2020 2020 2020 2020 2020 2020 6c6f 636b              lock
+00009460: 5f69 6478 203d 206c 656e 2873 656c 662e  _idx = len(self.
+00009470: 7365 676d 656e 7473 5b69 6e64 6578 305d  segments[index0]
+00009480: 2e77 6f72 6473 290d 0a20 2020 2020 2020  .words)..       
+00009490: 2020 2020 206e 6577 5f73 6567 2e77 6f72       new_seg.wor
+000094a0: 6473 5b6c 6f63 6b5f 6964 7820 2d20 315d  ds[lock_idx - 1]
+000094b0: 2e6c 6f63 6b5f 7269 6768 7428 290d 0a20  .lock_right().. 
+000094c0: 2020 2020 2020 2020 2020 2069 6620 6c6f             if lo
+000094d0: 636b 5f69 6478 203c 206c 656e 286e 6577  ck_idx < len(new
+000094e0: 5f73 6567 2e77 6f72 6473 293a 0d0a 2020  _seg.words):..  
+000094f0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00009500: 775f 7365 672e 776f 7264 735b 6c6f 636b  w_seg.words[lock
+00009510: 5f69 6478 5d2e 6c6f 636b 5f6c 6566 7428  _idx].lock_left(
+00009520: 290d 0a20 2020 2020 2020 2069 6620 696e  )..        if in
+00009530: 706c 6163 653a 0d0a 2020 2020 2020 2020  place:..        
+00009540: 2020 2020 6930 2c20 6931 203d 2073 6f72      i0, i1 = sor
+00009550: 7465 6428 5b69 6e64 6578 302c 2069 6e64  ted([index0, ind
+00009560: 6578 315d 290d 0a20 2020 2020 2020 2020  ex1])..         
+00009570: 2020 2073 656c 662e 7365 676d 656e 7473     self.segments
+00009580: 5b69 305d 203d 206e 6577 5f73 6567 0d0a  [i0] = new_seg..
+00009590: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
+000095a0: 7365 6c66 2e73 6567 6d65 6e74 735b 6931  self.segments[i1
+000095b0: 5d0d 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
+000095c0: 6e20 6e65 775f 7365 670d 0a0d 0a20 2020  n new_seg....   
+000095d0: 2064 6566 2072 6573 6361 6c65 5f74 696d   def rescale_tim
+000095e0: 6528 7365 6c66 2c20 7363 616c 655f 6661  e(self, scale_fa
+000095f0: 6374 6f72 3a20 666c 6f61 7429 3a0d 0a20  ctor: float):.. 
+00009600: 2020 2020 2020 2066 6f72 2073 2069 6e20         for s in 
+00009610: 7365 6c66 2e73 6567 6d65 6e74 733a 0d0a  self.segments:..
+00009620: 2020 2020 2020 2020 2020 2020 732e 7265              s.re
+00009630: 7363 616c 655f 7469 6d65 2873 6361 6c65  scale_time(scale
+00009640: 5f66 6163 746f 7229 0d0a 0d0a 2020 2020  _factor)....    
+00009650: 6465 6620 6170 706c 795f 6d69 6e5f 6475  def apply_min_du
+00009660: 7228 7365 6c66 2c20 6d69 6e5f 6475 723a  r(self, min_dur:
+00009670: 2066 6c6f 6174 2c20 696e 706c 6163 653a   float, inplace:
+00009680: 2062 6f6f 6c20 3d20 4661 6c73 6529 3a0d   bool = False):.
+00009690: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000096a0: 2020 2020 2020 4d65 7267 6520 616e 7920        Merge any 
+000096b0: 776f 7264 2f73 6567 6d65 6e74 2077 6974  word/segment wit
+000096c0: 6820 6164 6a61 6365 6e74 2077 6f72 642f  h adjacent word/
+000096d0: 7365 676d 656e 7420 6966 2069 7473 2064  segment if its d
+000096e0: 7572 6174 696f 6e20 6973 206c 6573 7320  uration is less 
+000096f0: 7468 616e 2060 606d 696e 5f64 7572 6060  than ``min_dur``
+00009700: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00009710: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00009720: 2073 656c 6620 6966 2069 6e70 6c61 6365   self if inplace
+00009730: 2065 6c73 6520 6465 6570 636f 7079 2873   else deepcopy(s
+00009740: 656c 6629 0d0a 2020 2020 2020 2020 6d61  elf)..        ma
+00009750: 785f 6920 3d20 6c65 6e28 7265 7375 6c74  x_i = len(result
+00009760: 2e73 6567 6d65 6e74 7329 202d 2031 0d0a  .segments) - 1..
+00009770: 2020 2020 2020 2020 6966 206d 6178 5f69          if max_i
+00009780: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+00009790: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000097a0: 740d 0a20 2020 2020 2020 2066 6f72 2069  t..        for i
+000097b0: 2069 6e20 7265 7665 7273 6564 2872 616e   in reversed(ran
+000097c0: 6765 286c 656e 2872 6573 756c 742e 7365  ge(len(result.se
+000097d0: 676d 656e 7473 2929 293a 0d0a 2020 2020  gments))):..    
+000097e0: 2020 2020 2020 2020 6966 206d 6178 5f69          if max_i
+000097f0: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+00009800: 2020 2020 2020 2020 6272 6561 6b0d 0a20          break.. 
+00009810: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+00009820: 7375 6c74 2e73 6567 6d65 6e74 735b 695d  sult.segments[i]
+00009830: 2e64 7572 6174 696f 6e20 3c20 6d69 6e5f  .duration < min_
+00009840: 6475 723a 0d0a 2020 2020 2020 2020 2020  dur:..          
+00009850: 2020 2020 2020 6966 2069 203d 3d20 6d61        if i == ma
+00009860: 785f 693a 0d0a 2020 2020 2020 2020 2020  x_i:..          
+00009870: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00009880: 2e61 6464 5f73 6567 6d65 6e74 7328 692d  .add_segments(i-
+00009890: 312c 2069 2c20 696e 706c 6163 653d 5472  1, i, inplace=Tr
+000098a0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+000098b0: 2020 2020 2065 6c69 6620 6920 3d3d 2030       elif i == 0
+000098c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000098d0: 2020 2020 2020 2072 6573 756c 742e 6164         result.ad
+000098e0: 645f 7365 676d 656e 7473 2869 2c20 692b  d_segments(i, i+
+000098f0: 312c 2069 6e70 6c61 6365 3d54 7275 6529  1, inplace=True)
+00009900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009910: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00009920: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00009930: 7265 7375 6c74 2e73 6567 6d65 6e74 735b  result.segments[
+00009940: 692b 315d 2e64 7572 6174 696f 6e20 3c20  i+1].duration < 
+00009950: 7265 7375 6c74 2e73 6567 6d65 6e74 735b  result.segments[
+00009960: 692d 315d 2e64 7572 6174 696f 6e3a 0d0a  i-1].duration:..
 00009970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009980: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099a0: 7265 7375 6c74 2e61 6464 5f73 6567 6d65  result.add_segme
-000099b0: 6e74 7328 692c 2069 2b31 2c20 696e 706c  nts(i, i+1, inpl
-000099c0: 6163 653d 5472 7565 290d 0a20 2020 2020  ace=True)..     
-000099d0: 2020 2020 2020 2020 2020 206d 6178 5f69             max_i
-000099e0: 202d 3d20 310d 0a20 2020 2020 2020 2072   -= 1..        r
-000099f0: 6573 756c 742e 7265 6173 7369 676e 5f69  esult.reassign_i
-00009a00: 6473 2829 0d0a 2020 2020 2020 2020 666f  ds()..        fo
-00009a10: 7220 7320 696e 2072 6573 756c 742e 7365  r s in result.se
-00009a20: 676d 656e 7473 3a0d 0a20 2020 2020 2020  gments:..       
-00009a30: 2020 2020 2073 2e61 7070 6c79 5f6d 696e       s.apply_min
-00009a40: 5f64 7572 286d 696e 5f64 7572 2c20 696e  _dur(min_dur, in
-00009a50: 706c 6163 653d 5472 7565 290d 0a20 2020  place=True)..   
-00009a60: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00009a70: 6c74 0d0a 0d0a 2020 2020 6465 6620 6f66  lt....    def of
-00009a80: 6673 6574 5f74 696d 6528 7365 6c66 2c20  fset_time(self, 
-00009a90: 6f66 6673 6574 5f73 6563 6f6e 6473 3a20  offset_seconds: 
-00009aa0: 666c 6f61 7429 3a0d 0a20 2020 2020 2020  float):..       
-00009ab0: 2066 6f72 2073 2069 6e20 7365 6c66 2e73   for s in self.s
-00009ac0: 6567 6d65 6e74 733a 0d0a 2020 2020 2020  egments:..      
-00009ad0: 2020 2020 2020 732e 6f66 6673 6574 5f74        s.offset_t
-00009ae0: 696d 6528 6f66 6673 6574 5f73 6563 6f6e  ime(offset_secon
-00009af0: 6473 290d 0a0d 0a20 2020 2064 6566 2073  ds)....    def s
-00009b00: 7570 7072 6573 735f 7369 6c65 6e63 6528  uppress_silence(
-00009b10: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00009b20: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
-00009b30: 2073 696c 656e 745f 7374 6172 7473 3a20   silent_starts: 
-00009b40: 6e70 2e6e 6461 7272 6179 2c0d 0a20 2020  np.ndarray,..   
-00009b50: 2020 2020 2020 2020 2073 696c 656e 745f           silent_
-00009b60: 656e 6473 3a20 6e70 2e6e 6461 7272 6179  ends: np.ndarray
-00009b70: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-00009b80: 696e 5f77 6f72 645f 6475 723a 204f 7074  in_word_dur: Opt
-00009b90: 696f 6e61 6c5b 666c 6f61 745d 203d 204e  ional[float] = N
-00009ba0: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-00009bb0: 2020 776f 7264 5f6c 6576 656c 3a20 626f    word_level: bo
-00009bc0: 6f6c 203d 2054 7275 652c 0d0a 2020 2020  ol = True,..    
-00009bd0: 2020 2020 2020 2020 6e6f 6e73 7065 6563          nonspeec
-00009be0: 685f 6572 726f 723a 2066 6c6f 6174 203d  h_error: float =
-00009bf0: 2030 2e33 2c0d 0a20 2020 2020 2020 2020   0.3,..         
-00009c00: 2020 2075 7365 5f77 6f72 645f 706f 7369     use_word_posi
-00009c10: 7469 6f6e 3a20 626f 6f6c 203d 2054 7275  tion: bool = Tru
-00009c20: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00009c30: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
-00009c40: 5472 7565 0d0a 2020 2020 2920 2d3e 2022  True..    ) -> "
-00009c50: 5768 6973 7065 7252 6573 756c 7422 3a0d  WhisperResult":.
-00009c60: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00009c70: 2020 2020 2020 4d6f 7665 2061 6e79 2073        Move any s
-00009c80: 7461 7274 2f65 6e64 2074 696d 6573 7461  tart/end timesta
-00009c90: 6d70 7320 696e 2073 696c 656e 6365 2070  mps in silence p
-00009ca0: 6172 7473 206f 6620 6175 6469 6f20 746f  arts of audio to
-00009cb0: 2074 6865 2062 6f75 6e64 6172 6965 7320   the boundaries 
-00009cc0: 6f66 2074 6865 2073 696c 656e 6365 2e0d  of the silence..
-00009cd0: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00009ce0: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
-00009cf0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-00009d00: 2020 2073 696c 656e 745f 7374 6172 7473     silent_starts
-00009d10: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
-00009d20: 0d0a 2020 2020 2020 2020 2020 2020 416e  ..            An
-00009d30: 2061 7272 6179 2073 7461 7274 696e 6720   array starting 
-00009d40: 7469 6d65 7374 616d 7073 206f 6620 7369  timestamps of si
-00009d50: 6c65 6e74 2073 6563 7469 6f6e 7320 6f66  lent sections of
-00009d60: 2061 7564 696f 2e0d 0a20 2020 2020 2020   audio...       
-00009d70: 2073 696c 656e 745f 656e 6473 203a 206e   silent_ends : n
-00009d80: 756d 7079 2e6e 6461 7272 6179 0d0a 2020  umpy.ndarray..  
-00009d90: 2020 2020 2020 2020 2020 416e 2061 7272            An arr
-00009da0: 6179 2065 6e64 696e 6720 7469 6d65 7374  ay ending timest
-00009db0: 616d 7073 206f 6620 7369 6c65 6e74 2073  amps of silent s
-00009dc0: 6563 7469 6f6e 7320 6f66 2061 7564 696f  ections of audio
-00009dd0: 2e0d 0a20 2020 2020 2020 206d 696e 5f77  ...        min_w
-00009de0: 6f72 645f 6475 7220 3a20 666c 6f61 7420  ord_dur : float 
-00009df0: 6f72 204e 6f6e 652c 2064 6566 6175 6c74  or None, default
-00009e00: 204e 6f6e 6520 6d65 616e 696e 6720 7573   None meaning us
-00009e10: 6520 6060 7374 6162 6c65 5f77 6869 7370  e ``stable_whisp
-00009e20: 6572 2e64 6566 6175 6c74 2e44 4546 4155  er.default.DEFAU
-00009e30: 4c54 5f56 414c 5545 5360 600d 0a20 2020  LT_VALUES``..   
-00009e40: 2020 2020 2020 2020 2053 686f 7274 6573           Shortes
-00009e50: 7420 6475 7261 7469 6f6e 2065 6163 6820  t duration each 
-00009e60: 776f 7264 2069 7320 616c 6c6f 7765 6420  word is allowed 
-00009e70: 746f 2072 6561 6368 2066 6f72 2061 646a  to reach for adj
-00009e80: 7573 746d 656e 7473 2e0d 0a20 2020 2020  ustments...     
-00009e90: 2020 2077 6f72 645f 6c65 7665 6c20 3a20     word_level : 
-00009ea0: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-00009eb0: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-00009ec0: 2057 6865 7468 6572 2074 6f20 7365 7474   Whether to sett
-00009ed0: 696e 6773 2074 6f20 776f 7264 206c 6576  ings to word lev
-00009ee0: 656c 2074 696d 6573 7461 6d70 732e 0d0a  el timestamps...
-00009ef0: 2020 2020 2020 2020 6e6f 6e73 7065 6563          nonspeec
-00009f00: 685f 6572 726f 7220 3a20 666c 6f61 742c  h_error : float,
-00009f10: 2064 6566 6175 6c74 2030 2e33 0d0a 2020   default 0.3..  
-00009f20: 2020 2020 2020 2020 2020 5265 6c61 7469            Relati
-00009f30: 7665 2065 7272 6f72 206f 6620 6e6f 6e2d  ve error of non-
-00009f40: 7370 6565 6368 2073 6563 7469 6f6e 7320  speech sections 
-00009f50: 7468 6174 2061 7070 6561 7220 696e 2062  that appear in b
-00009f60: 6574 7765 656e 2061 2077 6f72 6420 666f  etween a word fo
-00009f70: 7220 6164 6a75 7374 6d65 6e74 732e 0d0a  r adjustments...
-00009f80: 2020 2020 2020 2020 7573 655f 776f 7264          use_word
-00009f90: 5f70 6f73 6974 696f 6e20 3a20 626f 6f6c  _position : bool
-00009fa0: 2c20 6465 6661 756c 7420 5472 7565 0d0a  , default True..
-00009fb0: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-00009fc0: 6865 7220 746f 2075 7365 2070 6f73 6974  her to use posit
-00009fd0: 696f 6e20 6f66 2074 6865 2077 6f72 6420  ion of the word 
-00009fe0: 696e 2069 7473 2073 6567 6d65 6e74 2074  in its segment t
-00009ff0: 6f20 6465 7465 726d 696e 6520 7768 6574  o determine whet
-0000a000: 6865 7220 746f 206b 6565 7020 656e 6420  her to keep end 
-0000a010: 6f72 2073 7461 7274 2074 696d 6573 7461  or start timesta
-0000a020: 6d70 7320 6966 0d0a 2020 2020 2020 2020  mps if..        
-0000a030: 2020 2020 6164 6a75 7374 6d65 6e74 7320      adjustments 
-0000a040: 6172 6520 7265 7175 6972 6564 2e20 4966  are required. If
-0000a050: 2069 7420 6973 2074 6865 2066 6972 7374   it is the first
-0000a060: 2077 6f72 642c 206b 6565 7020 656e 642e   word, keep end.
-0000a070: 2045 6c73 6520 6966 2069 7420 6973 2074   Else if it is t
-0000a080: 6865 206c 6173 7420 776f 7264 2c20 6b65  he last word, ke
-0000a090: 6570 2074 6865 2073 7461 7274 2e0d 0a20  ep the start... 
-0000a0a0: 2020 2020 2020 2076 6572 626f 7365 203a         verbose :
-0000a0b0: 2062 6f6f 6c2c 2064 6566 6175 6c74 2054   bool, default T
-0000a0c0: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
-0000a0d0: 2057 6865 7468 6572 2074 6f20 7573 6520   Whether to use 
-0000a0e0: 7072 6f67 7265 7373 6261 7220 746f 2073  progressbar to s
-0000a0f0: 686f 7720 7072 6f67 7265 7373 2e0d 0a0d  how progress....
-0000a100: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000a110: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-0000a120: 2d0d 0a20 2020 2020 2020 2073 7461 626c  -..        stabl
-0000a130: 655f 7768 6973 7065 722e 7265 7375 6c74  e_whisper.result
-0000a140: 2e57 6869 7370 6572 5265 7375 6c74 0d0a  .WhisperResult..
-0000a150: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0000a160: 6375 7272 656e 7420 696e 7374 616e 6365  current instance
-0000a170: 2061 6674 6572 2074 6865 2063 6861 6e67   after the chang
-0000a180: 6573 2e0d 0a20 2020 2020 2020 2022 2222  es...        """
-0000a190: 0d0a 2020 2020 2020 2020 6d69 6e5f 776f  ..        min_wo
-0000a1a0: 7264 5f64 7572 203d 2067 6574 5f6d 696e  rd_dur = get_min
-0000a1b0: 5f77 6f72 645f 6475 7228 6d69 6e5f 776f  _word_dur(min_wo
-0000a1c0: 7264 5f64 7572 290d 0a20 2020 2020 2020  rd_dur)..       
-0000a1d0: 206d 6178 5f74 7320 3d20 7365 6c66 2e73   max_ts = self.s
-0000a1e0: 6567 6d65 6e74 735b 2d31 5d2e 656e 6420  egments[-1].end 
-0000a1f0: 6966 2073 656c 662e 7365 676d 656e 7473  if self.segments
-0000a200: 2065 6c73 6520 300d 0a20 2020 2020 2020   else 0..       
-0000a210: 2077 6974 6820 7471 646d 2874 6f74 616c   with tqdm(total
-0000a220: 3d6d 6178 5f74 732c 2075 6e69 743d 2773  =max_ts, unit='s
-0000a230: 6563 272c 2064 6973 6162 6c65 3d6e 6f74  ec', disable=not
-0000a240: 2076 6572 626f 7365 2c20 6465 7363 3d27   verbose, desc='
-0000a250: 4164 6a75 7374 6d65 6e74 2729 2061 7320  Adjustment') as 
-0000a260: 7471 646d 5f70 6261 723a 0d0a 2020 2020  tqdm_pbar:..    
-0000a270: 2020 2020 2020 2020 666f 7220 7320 696e          for s in
-0000a280: 2073 656c 662e 7365 676d 656e 7473 3a0d   self.segments:.
-0000a290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a2a0: 2073 2e73 7570 7072 6573 735f 7369 6c65   s.suppress_sile
-0000a2b0: 6e63 6528 0d0a 2020 2020 2020 2020 2020  nce(..          
-0000a2c0: 2020 2020 2020 2020 2020 7369 6c65 6e74            silent
-0000a2d0: 5f73 7461 7274 732c 0d0a 2020 2020 2020  _starts,..      
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 7369                si
-0000a2f0: 6c65 6e74 5f65 6e64 732c 0d0a 2020 2020  lent_ends,..    
+00009980: 2020 2020 2020 2020 7265 7375 6c74 2e61          result.a
+00009990: 6464 5f73 6567 6d65 6e74 7328 692d 312c  dd_segments(i-1,
+000099a0: 2069 2c20 696e 706c 6163 653d 5472 7565   i, inplace=True
+000099b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000099c0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000099d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099e0: 2020 2020 2020 7265 7375 6c74 2e61 6464        result.add
+000099f0: 5f73 6567 6d65 6e74 7328 692c 2069 2b31  _segments(i, i+1
+00009a00: 2c20 696e 706c 6163 653d 5472 7565 290d  , inplace=True).
+00009a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009a20: 206d 6178 5f69 202d 3d20 310d 0a20 2020   max_i -= 1..   
+00009a30: 2020 2020 2072 6573 756c 742e 7265 6173       result.reas
+00009a40: 7369 676e 5f69 6473 2829 0d0a 2020 2020  sign_ids()..    
+00009a50: 2020 2020 666f 7220 7320 696e 2072 6573      for s in res
+00009a60: 756c 742e 7365 676d 656e 7473 3a0d 0a20  ult.segments:.. 
+00009a70: 2020 2020 2020 2020 2020 2073 2e61 7070             s.app
+00009a80: 6c79 5f6d 696e 5f64 7572 286d 696e 5f64  ly_min_dur(min_d
+00009a90: 7572 2c20 696e 706c 6163 653d 5472 7565  ur, inplace=True
+00009aa0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00009ab0: 6e20 7265 7375 6c74 0d0a 0d0a 2020 2020  n result....    
+00009ac0: 6465 6620 6f66 6673 6574 5f74 696d 6528  def offset_time(
+00009ad0: 7365 6c66 2c20 6f66 6673 6574 5f73 6563  self, offset_sec
+00009ae0: 6f6e 6473 3a20 666c 6f61 7429 3a0d 0a20  onds: float):.. 
+00009af0: 2020 2020 2020 2066 6f72 2073 2069 6e20         for s in 
+00009b00: 7365 6c66 2e73 6567 6d65 6e74 733a 0d0a  self.segments:..
+00009b10: 2020 2020 2020 2020 2020 2020 732e 6f66              s.of
+00009b20: 6673 6574 5f74 696d 6528 6f66 6673 6574  fset_time(offset
+00009b30: 5f73 6563 6f6e 6473 290d 0a0d 0a20 2020  _seconds)....   
+00009b40: 2064 6566 2073 7570 7072 6573 735f 7369   def suppress_si
+00009b50: 6c65 6e63 6528 0d0a 2020 2020 2020 2020  lence(..        
+00009b60: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+00009b70: 2020 2020 2020 2073 696c 656e 745f 7374         silent_st
+00009b80: 6172 7473 3a20 6e70 2e6e 6461 7272 6179  arts: np.ndarray
+00009b90: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+00009ba0: 696c 656e 745f 656e 6473 3a20 6e70 2e6e  ilent_ends: np.n
+00009bb0: 6461 7272 6179 2c0d 0a20 2020 2020 2020  darray,..       
+00009bc0: 2020 2020 206d 696e 5f77 6f72 645f 6475       min_word_du
+00009bd0: 723a 204f 7074 696f 6e61 6c5b 666c 6f61  r: Optional[floa
+00009be0: 745d 203d 204e 6f6e 652c 0d0a 2020 2020  t] = None,..    
+00009bf0: 2020 2020 2020 2020 776f 7264 5f6c 6576          word_lev
+00009c00: 656c 3a20 626f 6f6c 203d 2054 7275 652c  el: bool = True,
+00009c10: 0d0a 2020 2020 2020 2020 2020 2020 6e6f  ..            no
+00009c20: 6e73 7065 6563 685f 6572 726f 723a 2066  nspeech_error: f
+00009c30: 6c6f 6174 203d 2030 2e33 2c0d 0a20 2020  loat = 0.3,..   
+00009c40: 2020 2020 2020 2020 2075 7365 5f77 6f72           use_wor
+00009c50: 645f 706f 7369 7469 6f6e 3a20 626f 6f6c  d_position: bool
+00009c60: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
+00009c70: 2020 2020 2020 7665 7262 6f73 653a 2062        verbose: b
+00009c80: 6f6f 6c20 3d20 5472 7565 2c0d 0a20 2020  ool = True,..   
+00009c90: 2029 202d 3e20 2257 6869 7370 6572 5265   ) -> "WhisperRe
+00009ca0: 7375 6c74 223a 0d0a 2020 2020 2020 2020  sult":..        
+00009cb0: 2222 220d 0a20 2020 2020 2020 204d 6f76  """..        Mov
+00009cc0: 6520 616e 7920 7374 6172 742f 656e 6420  e any start/end 
+00009cd0: 7469 6d65 7374 616d 7073 2069 6e20 7369  timestamps in si
+00009ce0: 6c65 6e63 6520 7061 7274 7320 6f66 2061  lence parts of a
+00009cf0: 7564 696f 2074 6f20 7468 6520 626f 756e  udio to the boun
+00009d00: 6461 7269 6573 206f 6620 7468 6520 7369  daries of the si
+00009d10: 6c65 6e63 652e 0d0a 0d0a 2020 2020 2020  lence.....      
+00009d20: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
+00009d30: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00009d40: 0d0a 2020 2020 2020 2020 7369 6c65 6e74  ..        silent
+00009d50: 5f73 7461 7274 7320 3a20 6e75 6d70 792e  _starts : numpy.
+00009d60: 6e64 6172 7261 790d 0a20 2020 2020 2020  ndarray..       
+00009d70: 2020 2020 2041 6e20 6172 7261 7920 7374       An array st
+00009d80: 6172 7469 6e67 2074 696d 6573 7461 6d70  arting timestamp
+00009d90: 7320 6f66 2073 696c 656e 7420 7365 6374  s of silent sect
+00009da0: 696f 6e73 206f 6620 6175 6469 6f2e 0d0a  ions of audio...
+00009db0: 2020 2020 2020 2020 7369 6c65 6e74 5f65          silent_e
+00009dc0: 6e64 7320 3a20 6e75 6d70 792e 6e64 6172  nds : numpy.ndar
+00009dd0: 7261 790d 0a20 2020 2020 2020 2020 2020  ray..           
+00009de0: 2041 6e20 6172 7261 7920 656e 6469 6e67   An array ending
+00009df0: 2074 696d 6573 7461 6d70 7320 6f66 2073   timestamps of s
+00009e00: 696c 656e 7420 7365 6374 696f 6e73 206f  ilent sections o
+00009e10: 6620 6175 6469 6f2e 0d0a 2020 2020 2020  f audio...      
+00009e20: 2020 6d69 6e5f 776f 7264 5f64 7572 203a    min_word_dur :
+00009e30: 2066 6c6f 6174 206f 7220 4e6f 6e65 2c20   float or None, 
+00009e40: 6465 6661 756c 7420 4e6f 6e65 206d 6561  default None mea
+00009e50: 6e69 6e67 2075 7365 2060 6073 7461 626c  ning use ``stabl
+00009e60: 655f 7768 6973 7065 722e 6465 6661 756c  e_whisper.defaul
+00009e70: 742e 4445 4641 554c 545f 5641 4c55 4553  t.DEFAULT_VALUES
+00009e80: 6060 0d0a 2020 2020 2020 2020 2020 2020  ``..            
+00009e90: 5368 6f72 7465 7374 2064 7572 6174 696f  Shortest duratio
+00009ea0: 6e20 6561 6368 2077 6f72 6420 6973 2061  n each word is a
+00009eb0: 6c6c 6f77 6564 2074 6f20 7265 6163 6820  llowed to reach 
+00009ec0: 666f 7220 6164 6a75 7374 6d65 6e74 732e  for adjustments.
+00009ed0: 0d0a 2020 2020 2020 2020 776f 7264 5f6c  ..        word_l
+00009ee0: 6576 656c 203a 2062 6f6f 6c2c 2064 6566  evel : bool, def
+00009ef0: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
+00009f00: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+00009f10: 746f 2073 6574 7469 6e67 7320 746f 2077  to settings to w
+00009f20: 6f72 6420 6c65 7665 6c20 7469 6d65 7374  ord level timest
+00009f30: 616d 7073 2e0d 0a20 2020 2020 2020 206e  amps...        n
+00009f40: 6f6e 7370 6565 6368 5f65 7272 6f72 203a  onspeech_error :
+00009f50: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
+00009f60: 302e 330d 0a20 2020 2020 2020 2020 2020  0.3..           
+00009f70: 2052 656c 6174 6976 6520 6572 726f 7220   Relative error 
+00009f80: 6f66 206e 6f6e 2d73 7065 6563 6820 7365  of non-speech se
+00009f90: 6374 696f 6e73 2074 6861 7420 6170 7065  ctions that appe
+00009fa0: 6172 2069 6e20 6265 7477 6565 6e20 6120  ar in between a 
+00009fb0: 776f 7264 2066 6f72 2061 646a 7573 746d  word for adjustm
+00009fc0: 656e 7473 2e0d 0a20 2020 2020 2020 2075  ents...        u
+00009fd0: 7365 5f77 6f72 645f 706f 7369 7469 6f6e  se_word_position
+00009fe0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+00009ff0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
+0000a000: 2020 2057 6865 7468 6572 2074 6f20 7573     Whether to us
+0000a010: 6520 706f 7369 7469 6f6e 206f 6620 7468  e position of th
+0000a020: 6520 776f 7264 2069 6e20 6974 7320 7365  e word in its se
+0000a030: 676d 656e 7420 746f 2064 6574 6572 6d69  gment to determi
+0000a040: 6e65 2077 6865 7468 6572 2074 6f20 6b65  ne whether to ke
+0000a050: 6570 2065 6e64 206f 7220 7374 6172 7420  ep end or start 
+0000a060: 7469 6d65 7374 616d 7073 2069 660d 0a20  timestamps if.. 
+0000a070: 2020 2020 2020 2020 2020 2061 646a 7573             adjus
+0000a080: 746d 656e 7473 2061 7265 2072 6571 7569  tments are requi
+0000a090: 7265 642e 2049 6620 6974 2069 7320 7468  red. If it is th
+0000a0a0: 6520 6669 7273 7420 776f 7264 2c20 6b65  e first word, ke
+0000a0b0: 6570 2065 6e64 2e20 456c 7365 2069 6620  ep end. Else if 
+0000a0c0: 6974 2069 7320 7468 6520 6c61 7374 2077  it is the last w
+0000a0d0: 6f72 642c 206b 6565 7020 7468 6520 7374  ord, keep the st
+0000a0e0: 6172 742e 0d0a 2020 2020 2020 2020 7665  art...        ve
+0000a0f0: 7262 6f73 6520 3a20 626f 6f6c 2c20 6465  rbose : bool, de
+0000a100: 6661 756c 7420 5472 7565 0d0a 2020 2020  fault True..    
+0000a110: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+0000a120: 746f 2075 7365 2070 726f 6772 6573 7362  to use progressb
+0000a130: 6172 2074 6f20 7368 6f77 2070 726f 6772  ar to show progr
+0000a140: 6573 732e 0d0a 0d0a 2020 2020 2020 2020  ess.....        
+0000a150: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
+0000a160: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020   -------..      
+0000a170: 2020 7374 6162 6c65 5f77 6869 7370 6572    stable_whisper
+0000a180: 2e72 6573 756c 742e 5768 6973 7065 7252  .result.WhisperR
+0000a190: 6573 756c 740d 0a20 2020 2020 2020 2020  esult..         
+0000a1a0: 2020 2054 6865 2063 7572 7265 6e74 2069     The current i
+0000a1b0: 6e73 7461 6e63 6520 6166 7465 7220 7468  nstance after th
+0000a1c0: 6520 6368 616e 6765 732e 0d0a 2020 2020  e changes...    
+0000a1d0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0000a1e0: 206d 696e 5f77 6f72 645f 6475 7220 3d20   min_word_dur = 
+0000a1f0: 6765 745f 6d69 6e5f 776f 7264 5f64 7572  get_min_word_dur
+0000a200: 286d 696e 5f77 6f72 645f 6475 7229 0d0a  (min_word_dur)..
+0000a210: 2020 2020 2020 2020 6d61 785f 7473 203d          max_ts =
+0000a220: 2073 656c 662e 7365 676d 656e 7473 5b2d   self.segments[-
+0000a230: 315d 2e65 6e64 2069 6620 7365 6c66 2e73  1].end if self.s
+0000a240: 6567 6d65 6e74 7320 656c 7365 2030 0d0a  egments else 0..
+0000a250: 2020 2020 2020 2020 7769 7468 2074 7164          with tqd
+0000a260: 6d28 746f 7461 6c3d 6d61 785f 7473 2c20  m(total=max_ts, 
+0000a270: 756e 6974 3d27 7365 6327 2c20 6469 7361  unit='sec', disa
+0000a280: 626c 653d 6e6f 7420 7665 7262 6f73 652c  ble=not verbose,
+0000a290: 2064 6573 633d 2741 646a 7573 746d 656e   desc='Adjustmen
+0000a2a0: 7427 2920 6173 2074 7164 6d5f 7062 6172  t') as tqdm_pbar
+0000a2b0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+0000a2c0: 6f72 2073 2069 6e20 7365 6c66 2e73 6567  or s in self.seg
+0000a2d0: 6d65 6e74 733a 0d0a 2020 2020 2020 2020  ments:..        
+0000a2e0: 2020 2020 2020 2020 732e 7375 7070 7265          s.suppre
+0000a2f0: 7373 5f73 696c 656e 6365 280d 0a20 2020  ss_silence(..   
 0000a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a310: 6d69 6e5f 776f 7264 5f64 7572 2c0d 0a20  min_word_dur,.. 
-0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a330: 2020 2077 6f72 645f 6c65 7665 6c3d 776f     word_level=wo
-0000a340: 7264 5f6c 6576 656c 2c0d 0a20 2020 2020  rd_level,..     
-0000a350: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000a360: 6f6e 7370 6565 6368 5f65 7272 6f72 3d6e  onspeech_error=n
-0000a370: 6f6e 7370 6565 6368 5f65 7272 6f72 2c0d  onspeech_error,.
-0000a380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a390: 2020 2020 2075 7365 5f77 6f72 645f 706f       use_word_po
-0000a3a0: 7369 7469 6f6e 3d75 7365 5f77 6f72 645f  sition=use_word_
-0000a3b0: 706f 7369 7469 6f6e 0d0a 2020 2020 2020  position..      
-0000a3c0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-0000a3d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000a3e0: 7665 7262 6f73 653a 0d0a 2020 2020 2020  verbose:..      
-0000a3f0: 2020 2020 2020 2020 2020 2020 2020 7471                tq
-0000a400: 646d 5f70 6261 722e 7570 6461 7465 2873  dm_pbar.update(s
-0000a410: 2e65 6e64 202d 2074 7164 6d5f 7062 6172  .end - tqdm_pbar
-0000a420: 2e6e 290d 0a20 2020 2020 2020 2020 2020  .n)..           
-0000a430: 2074 7164 6d5f 7062 6172 2e75 7064 6174   tqdm_pbar.updat
-0000a440: 6528 7471 646d 5f70 6261 722e 746f 7461  e(tqdm_pbar.tota
-0000a450: 6c20 2d20 7471 646d 5f70 6261 722e 6e29  l - tqdm_pbar.n)
-0000a460: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-0000a470: 726e 2073 656c 660d 0a0d 0a20 2020 2064  rn self....    d
-0000a480: 6566 2061 646a 7573 745f 6279 5f73 696c  ef adjust_by_sil
-0000a490: 656e 6365 280d 0a20 2020 2020 2020 2020  ence(..         
-0000a4a0: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
-0000a4b0: 2020 2020 2020 6175 6469 6f3a 2055 6e69        audio: Uni
-0000a4c0: 6f6e 5b74 6f72 6368 2e54 656e 736f 722c  on[torch.Tensor,
-0000a4d0: 206e 702e 6e64 6172 7261 792c 2073 7472   np.ndarray, str
-0000a4e0: 2c20 6279 7465 735d 2c0d 0a20 2020 2020  , bytes],..     
-0000a4f0: 2020 2020 2020 2076 6164 3a20 626f 6f6c         vad: bool
-0000a500: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
-0000a510: 2020 2020 2020 202a 2c0d 0a20 2020 2020         *,..     
-0000a520: 2020 2020 2020 2076 6572 626f 7365 3a20         verbose: 
-0000a530: 2862 6f6f 6c2c 204e 6f6e 6529 203d 2046  (bool, None) = F
-0000a540: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
-0000a550: 2020 2073 616d 706c 655f 7261 7465 3a20     sample_rate: 
-0000a560: 696e 7420 3d20 4e6f 6e65 2c0d 0a20 2020  int = None,..   
-0000a570: 2020 2020 2020 2020 2076 6164 5f6f 6e6e           vad_onn
-0000a580: 783a 2062 6f6f 6c20 3d20 4661 6c73 652c  x: bool = False,
-0000a590: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-0000a5a0: 645f 7468 7265 7368 6f6c 643a 2066 6c6f  d_threshold: flo
-0000a5b0: 6174 203d 2030 2e33 352c 0d0a 2020 2020  at = 0.35,..    
-0000a5c0: 2020 2020 2020 2020 715f 6c65 7665 6c73          q_levels
-0000a5d0: 3a20 696e 7420 3d20 3230 2c0d 0a20 2020  : int = 20,..   
-0000a5e0: 2020 2020 2020 2020 206b 5f73 697a 653a           k_size:
-0000a5f0: 2069 6e74 203d 2035 2c0d 0a20 2020 2020   int = 5,..     
-0000a600: 2020 2020 2020 206d 696e 5f77 6f72 645f         min_word_
-0000a610: 6475 723a 204f 7074 696f 6e61 6c5b 666c  dur: Optional[fl
-0000a620: 6f61 745d 203d 204e 6f6e 652c 0d0a 2020  oat] = None,..  
-0000a630: 2020 2020 2020 2020 2020 776f 7264 5f6c            word_l
-0000a640: 6576 656c 3a20 626f 6f6c 203d 2054 7275  evel: bool = Tru
-0000a650: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000a660: 6e6f 6e73 7065 6563 685f 6572 726f 723a  nonspeech_error:
-0000a670: 2066 6c6f 6174 203d 2030 2e33 2c0d 0a20   float = 0.3,.. 
-0000a680: 2020 2020 2020 2020 2020 2075 7365 5f77             use_w
-0000a690: 6f72 645f 706f 7369 7469 6f6e 3a20 626f  ord_position: bo
-0000a6a0: 6f6c 203d 2054 7275 650d 0a0d 0a20 2020  ol = True....   
-0000a6b0: 2029 202d 3e20 2257 6869 7370 6572 5265   ) -> "WhisperRe
-0000a6c0: 7375 6c74 223a 0d0a 2020 2020 2020 2020  sult":..        
-0000a6d0: 2222 220d 0a20 2020 2020 2020 2041 646a  """..        Adj
-0000a6e0: 7573 7420 7469 6d65 7374 616d 7073 2062  ust timestamps b
-0000a6f0: 6173 6520 6f6e 2064 6574 6563 7465 6420  ase on detected 
-0000a700: 7370 6565 6368 2067 6170 732e 0d0a 0d0a  speech gaps.....
-0000a710: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
-0000a720: 6d65 7468 6f64 2063 6f6d 6269 6e65 7320  method combines 
-0000a730: 3a6d 6574 683a 6073 7461 626c 655f 7768  :meth:`stable_wh
-0000a740: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
-0000a750: 7370 6572 5265 7375 6c74 2e73 7570 7072  sperResult.suppr
-0000a760: 6573 735f 7369 6c65 6e63 6560 2077 6974  ess_silence` wit
-0000a770: 6820 7369 6c65 6e63 6520 6465 7465 6374  h silence detect
-0000a780: 696f 6e2e 0d0a 0d0a 2020 2020 2020 2020  ion.....        
-0000a790: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-0000a7a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-0000a7b0: 2020 2020 2020 2020 6175 6469 6f20 3a20          audio : 
-0000a7c0: 7374 7220 6f72 206e 756d 7079 2e6e 6461  str or numpy.nda
-0000a7d0: 7272 6179 206f 7220 746f 7263 682e 5465  rray or torch.Te
-0000a7e0: 6e73 6f72 206f 7220 6279 7465 730d 0a20  nsor or bytes.. 
-0000a7f0: 2020 2020 2020 2020 2020 2050 6174 682f             Path/
-0000a800: 5552 4c20 746f 2074 6865 2061 7564 696f  URL to the audio
-0000a810: 2066 696c 652c 2074 6865 2061 7564 696f   file, the audio
-0000a820: 2077 6176 6566 6f72 6d2c 206f 7220 6279   waveform, or by
-0000a830: 7465 7320 6f66 2061 7564 696f 2066 696c  tes of audio fil
-0000a840: 652e 0d0a 2020 2020 2020 2020 7661 6420  e...        vad 
-0000a850: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-0000a860: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-0000a870: 2020 2057 6865 7468 6572 2074 6f20 7573     Whether to us
-0000a880: 6520 5369 6c65 726f 2056 4144 2074 6f20  e Silero VAD to 
-0000a890: 6765 6e65 7261 7465 2074 696d 6573 7461  generate timesta
-0000a8a0: 6d70 2073 7570 7072 6573 7369 6f6e 206d  mp suppression m
-0000a8b0: 6173 6b2e 0d0a 2020 2020 2020 2020 2020  ask...          
-0000a8c0: 2020 5369 6c65 726f 2056 4144 2072 6571    Silero VAD req
-0000a8d0: 7569 7265 7320 5079 546f 7263 6820 312e  uires PyTorch 1.
-0000a8e0: 3132 2e30 2b2e 204f 6666 6963 6961 6c20  12.0+. Official 
-0000a8f0: 7265 706f 2c20 6874 7470 733a 2f2f 6769  repo, https://gi
-0000a900: 7468 7562 2e63 6f6d 2f73 6e61 6b65 7273  thub.com/snakers
-0000a910: 342f 7369 6c65 726f 2d76 6164 2e0d 0a20  4/silero-vad... 
-0000a920: 2020 2020 2020 2076 6572 626f 7365 203a         verbose :
-0000a930: 2062 6f6f 6c20 6f72 204e 6f6e 652c 2064   bool or None, d
-0000a940: 6566 6175 6c74 2046 616c 7365 0d0a 2020  efault False..  
-0000a950: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
-0000a960: 7220 746f 2075 7365 2070 726f 6772 6573  r to use progres
-0000a970: 7362 6172 2074 6f20 7368 6f77 2070 726f  sbar to show pro
-0000a980: 6772 6573 732e 0d0a 2020 2020 2020 2020  gress...        
-0000a990: 2020 2020 4966 2060 6076 6164 203d 2054      If ``vad = T
-0000a9a0: 7275 6560 6020 616e 6420 6060 4661 6c73  rue`` and ``Fals
-0000a9b0: 6560 602c 206d 7574 6520 6d65 7373 6167  e``, mute messag
-0000a9c0: 6573 2061 626f 7574 2068 6974 7469 6e67  es about hitting
-0000a9d0: 206c 6f63 616c 2063 6163 6865 732e 0d0a   local caches...
-0000a9e0: 2020 2020 2020 2020 2020 2020 4e6f 7465              Note
-0000a9f0: 2074 6861 7420 7468 6520 6d65 7373 6167   that the messag
-0000aa00: 6520 6162 6f75 7420 6669 7273 7420 646f  e about first do
-0000aa10: 776e 6c6f 6164 2063 616e 6e6f 7420 6265  wnload cannot be
-0000aa20: 206d 7574 6564 2e0d 0a20 2020 2020 2020   muted...       
-0000aa30: 2073 616d 706c 655f 7261 7465 203a 2069   sample_rate : i
-0000aa40: 6e74 2c20 6465 6661 756c 7420 4e6f 6e65  nt, default None
-0000aa50: 2c20 6d65 616e 696e 6720 6060 7768 6973  , meaning ``whis
-0000aa60: 7065 722e 6175 6469 6f2e 5341 4d50 4c45  per.audio.SAMPLE
-0000aa70: 5f52 4154 4560 602c 2031 366b 485a 0d0a  _RATE``, 16kHZ..
-0000aa80: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0000aa90: 7361 6d70 6c65 2072 6174 6520 6f66 2060  sample rate of `
-0000aaa0: 6061 7564 696f 6060 2e0d 0a20 2020 2020  `audio``...     
-0000aab0: 2020 2076 6164 5f6f 6e6e 7820 3a20 626f     vad_onnx : bo
-0000aac0: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-0000aad0: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
-0000aae0: 6865 7468 6572 2074 6f20 7573 6520 4f4e  hether to use ON
-0000aaf0: 4e58 2066 6f72 2053 696c 6572 6f20 5641  NX for Silero VA
-0000ab00: 442e 0d0a 2020 2020 2020 2020 7661 645f  D...        vad_
-0000ab10: 7468 7265 7368 6f6c 6420 3a20 666c 6f61  threshold : floa
-0000ab20: 742c 2064 6566 6175 6c74 2030 2e33 350d  t, default 0.35.
-0000ab30: 0a20 2020 2020 2020 2020 2020 2054 6872  .            Thr
-0000ab40: 6573 686f 6c64 2066 6f72 2064 6574 6563  eshold for detec
-0000ab50: 7469 6e67 2073 7065 6563 6820 7769 7468  ting speech with
-0000ab60: 2053 696c 6572 6f20 5641 442e 204c 6f77   Silero VAD. Low
-0000ab70: 2074 6872 6573 686f 6c64 2072 6564 7563   threshold reduc
-0000ab80: 6573 2066 616c 7365 2070 6f73 6974 6976  es false positiv
-0000ab90: 6573 2066 6f72 2073 696c 656e 6365 2064  es for silence d
-0000aba0: 6574 6563 7469 6f6e 2e0d 0a20 2020 2020  etection...     
-0000abb0: 2020 2071 5f6c 6576 656c 7320 3a20 696e     q_levels : in
-0000abc0: 742c 2064 6566 6175 6c74 2032 300d 0a20  t, default 20.. 
-0000abd0: 2020 2020 2020 2020 2020 2051 7561 6e74             Quant
-0000abe0: 697a 6174 696f 6e20 6c65 7665 6c73 2066  ization levels f
-0000abf0: 6f72 2067 656e 6572 6174 696e 6720 7469  or generating ti
-0000ac00: 6d65 7374 616d 7020 7375 7070 7265 7373  mestamp suppress
-0000ac10: 696f 6e20 6d61 736b 3b20 6967 6e6f 7265  ion mask; ignore
-0000ac20: 6420 6966 2060 6076 6164 203d 2074 7275  d if ``vad = tru
-0000ac30: 6560 602e 0d0a 2020 2020 2020 2020 2020  e``...          
-0000ac40: 2020 4163 7473 2061 7320 6120 7468 7265    Acts as a thre
-0000ac50: 7368 6f6c 6420 746f 206d 6172 6b69 6e67  shold to marking
-0000ac60: 2073 6f75 6e64 2061 7320 7369 6c65 6e74   sound as silent
-0000ac70: 2e0d 0a20 2020 2020 2020 2020 2020 2046  ...            F
-0000ac80: 6577 6572 206c 6576 656c 7320 7769 6c6c  ewer levels will
-0000ac90: 2069 6e63 7265 6173 6520 7468 6520 7468   increase the th
-0000aca0: 7265 7368 6f6c 6420 6f66 2076 6f6c 756d  reshold of volum
-0000acb0: 6520 6174 2077 6869 6368 2074 6f20 6d61  e at which to ma
-0000acc0: 726b 2061 2073 6f75 6e64 2061 7320 7369  rk a sound as si
-0000acd0: 6c65 6e74 2e0d 0a20 2020 2020 2020 206b  lent...        k
-0000ace0: 5f73 697a 6520 3a20 696e 742c 2064 6566  _size : int, def
-0000acf0: 6175 6c74 2035 0d0a 2020 2020 2020 2020  ault 5..        
-0000ad00: 2020 2020 4b65 726e 656c 2073 697a 6520      Kernel size 
-0000ad10: 666f 7220 6176 672d 706f 6f6c 696e 6720  for avg-pooling 
-0000ad20: 7761 7665 666f 726d 2074 6f20 6765 6e65  waveform to gene
-0000ad30: 7261 7465 2074 696d 6573 7461 6d70 2073  rate timestamp s
-0000ad40: 7570 7072 6573 7369 6f6e 206d 6173 6b3b  uppression mask;
-0000ad50: 2069 676e 6f72 6564 2069 6620 6060 7661   ignored if ``va
-0000ad60: 6420 3d20 7472 7565 6060 2e0d 0a20 2020  d = true``...   
-0000ad70: 2020 2020 2020 2020 2052 6563 6f6d 6d65           Recomme
-0000ad80: 6e64 2035 206f 7220 333b 2068 6967 6865  nd 5 or 3; highe
-0000ad90: 7220 7369 7a65 7320 7769 6c6c 2072 6564  r sizes will red
-0000ada0: 7563 6520 6465 7465 6374 696f 6e20 6f66  uce detection of
-0000adb0: 2073 696c 656e 6365 2e0d 0a20 2020 2020   silence...     
-0000adc0: 2020 206d 696e 5f77 6f72 645f 6475 7220     min_word_dur 
-0000add0: 3a20 666c 6f61 7420 6f72 204e 6f6e 652c  : float or None,
-0000ade0: 2064 6566 6175 6c74 204e 6f6e 6520 6d65   default None me
-0000adf0: 616e 696e 6720 7573 6520 6060 7374 6162  aning use ``stab
-0000ae00: 6c65 5f77 6869 7370 6572 2e64 6566 6175  le_whisper.defau
-0000ae10: 6c74 2e44 4546 4155 4c54 5f56 414c 5545  lt.DEFAULT_VALUE
-0000ae20: 5360 600d 0a20 2020 2020 2020 2020 2020  S``..           
-0000ae30: 2053 686f 7274 6573 7420 6475 7261 7469   Shortest durati
-0000ae40: 6f6e 2065 6163 6820 776f 7264 2069 7320  on each word is 
-0000ae50: 616c 6c6f 7765 6420 746f 2072 6561 6368  allowed to reach
-0000ae60: 2066 726f 6d20 6164 6a75 7374 6d65 6e74   from adjustment
-0000ae70: 732e 0d0a 2020 2020 2020 2020 776f 7264  s...        word
-0000ae80: 5f6c 6576 656c 203a 2062 6f6f 6c2c 2064  _level : bool, d
-0000ae90: 6566 6175 6c74 2054 7275 650d 0a20 2020  efault True..   
-0000aea0: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
-0000aeb0: 2074 6f20 7365 7474 696e 6773 2074 6f20   to settings to 
-0000aec0: 776f 7264 206c 6576 656c 2074 696d 6573  word level times
-0000aed0: 7461 6d70 732e 0d0a 2020 2020 2020 2020  tamps...        
-0000aee0: 6e6f 6e73 7065 6563 685f 6572 726f 7220  nonspeech_error 
-0000aef0: 3a20 666c 6f61 742c 2064 6566 6175 6c74  : float, default
-0000af00: 2030 2e33 0d0a 2020 2020 2020 2020 2020   0.3..          
-0000af10: 2020 5265 6c61 7469 7665 2065 7272 6f72    Relative error
-0000af20: 206f 6620 6e6f 6e2d 7370 6565 6368 2073   of non-speech s
-0000af30: 6563 7469 6f6e 7320 7468 6174 2061 7070  ections that app
-0000af40: 6561 7220 696e 2062 6574 7765 656e 2061  ear in between a
-0000af50: 2077 6f72 6420 666f 7220 6164 6a75 7374   word for adjust
-0000af60: 6d65 6e74 732e 0d0a 2020 2020 2020 2020  ments...        
-0000af70: 7573 655f 776f 7264 5f70 6f73 6974 696f  use_word_positio
-0000af80: 6e20 3a20 626f 6f6c 2c20 6465 6661 756c  n : bool, defaul
-0000af90: 7420 5472 7565 0d0a 2020 2020 2020 2020  t True..        
-0000afa0: 2020 2020 5768 6574 6865 7220 746f 2075      Whether to u
-0000afb0: 7365 2070 6f73 6974 696f 6e20 6f66 2074  se position of t
-0000afc0: 6865 2077 6f72 6420 696e 2069 7473 2073  he word in its s
-0000afd0: 6567 6d65 6e74 2074 6f20 6465 7465 726d  egment to determ
-0000afe0: 696e 6520 7768 6574 6865 7220 746f 206b  ine whether to k
-0000aff0: 6565 7020 656e 6420 6f72 2073 7461 7274  eep end or start
-0000b000: 2074 696d 6573 7461 6d70 7320 6966 0d0a   timestamps if..
-0000b010: 2020 2020 2020 2020 2020 2020 6164 6a75              adju
-0000b020: 7374 6d65 6e74 7320 6172 6520 7265 7175  stments are requ
-0000b030: 6972 6564 2e20 4966 2069 7420 6973 2074  ired. If it is t
-0000b040: 6865 2066 6972 7374 2077 6f72 642c 206b  he first word, k
-0000b050: 6565 7020 656e 642e 2045 6c73 6520 6966  eep end. Else if
-0000b060: 2069 7420 6973 2074 6865 206c 6173 7420   it is the last 
-0000b070: 776f 7264 2c20 6b65 6570 2074 6865 2073  word, keep the s
-0000b080: 7461 7274 2e0d 0a0d 0a20 2020 2020 2020  tart.....       
-0000b090: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-0000b0a0: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-0000b0b0: 2020 2073 7461 626c 655f 7768 6973 7065     stable_whispe
-0000b0c0: 722e 7265 7375 6c74 2e57 6869 7370 6572  r.result.Whisper
-0000b0d0: 5265 7375 6c74 0d0a 2020 2020 2020 2020  Result..        
-0000b0e0: 2020 2020 5468 6520 6375 7272 656e 7420      The current 
-0000b0f0: 696e 7374 616e 6365 2061 6674 6572 2074  instance after t
-0000b100: 6865 2063 6861 6e67 6573 2e0d 0a0d 0a20  he changes..... 
-0000b110: 2020 2020 2020 204e 6f74 6573 0d0a 2020         Notes..  
-0000b120: 2020 2020 2020 2d2d 2d2d 2d0d 0a20 2020        -----..   
-0000b130: 2020 2020 2054 6869 7320 6f70 6572 6174       This operat
-0000b140: 696f 6e20 6973 2061 6c72 6561 6479 2070  ion is already p
-0000b150: 6572 666f 726d 6564 2062 7920 3a66 756e  erformed by :fun
-0000b160: 633a 6073 7461 626c 655f 7768 6973 7065  c:`stable_whispe
-0000b170: 722e 7768 6973 7065 725f 776f 7264 5f6c  r.whisper_word_l
-0000b180: 6576 656c 2e74 7261 6e73 6372 6962 655f  evel.transcribe_
-0000b190: 7374 6162 6c65 6020 2f0d 0a20 2020 2020  stable` /..     
-0000b1a0: 2020 203a 6675 6e63 3a60 7374 6162 6c65     :func:`stable
-0000b1b0: 5f77 6869 7370 6572 2e77 6869 7370 6572  _whisper.whisper
-0000b1c0: 5f77 6f72 645f 6c65 7665 6c2e 7472 616e  _word_level.tran
-0000b1d0: 7363 7269 6265 5f6d 696e 696d 616c 602f  scribe_minimal`/
-0000b1e0: 0d0a 2020 2020 2020 2020 3a66 756e 633a  ..        :func:
-0000b1f0: 6073 7461 626c 655f 7768 6973 7065 722e  `stable_whisper.
-0000b200: 6e6f 6e5f 7768 6973 7065 722e 7472 616e  non_whisper.tran
-0000b210: 7363 7269 6265 5f61 6e79 6020 2f20 3a66  scribe_any` / :f
-0000b220: 756e 633a 6073 7461 626c 655f 7768 6973  unc:`stable_whis
-0000b230: 7065 722e 616c 6967 6e6d 656e 742e 616c  per.alignment.al
-0000b240: 6967 6e60 0d0a 2020 2020 2020 2020 6966  ign`..        if
-0000b250: 2060 6073 7570 7072 6573 735f 7369 6c65   ``suppress_sile
-0000b260: 6e63 6520 3d20 5472 7565 6060 2e0d 0a20  nce = True``... 
-0000b270: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-0000b280: 2020 2020 6d69 6e5f 776f 7264 5f64 7572      min_word_dur
-0000b290: 203d 2067 6574 5f6d 696e 5f77 6f72 645f   = get_min_word_
-0000b2a0: 6475 7228 6d69 6e5f 776f 7264 5f64 7572  dur(min_word_dur
-0000b2b0: 290d 0a20 2020 2020 2020 2069 6620 7661  )..        if va
-0000b2c0: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
-0000b2d0: 6175 6469 6f20 3d20 6175 6469 6f5f 746f  audio = audio_to
-0000b2e0: 5f74 656e 736f 725f 7265 7361 6d70 6c65  _tensor_resample
-0000b2f0: 2861 7564 696f 2c20 7361 6d70 6c65 5f72  (audio, sample_r
-0000b300: 6174 652c 2056 4144 5f53 414d 504c 455f  ate, VAD_SAMPLE_
-0000b310: 5241 5445 535b 305d 290d 0a20 2020 2020  RATES[0])..     
-0000b320: 2020 2020 2020 2073 616d 706c 655f 7261         sample_ra
-0000b330: 7465 203d 2056 4144 5f53 414d 504c 455f  te = VAD_SAMPLE_
-0000b340: 5241 5445 535b 305d 0d0a 2020 2020 2020  RATES[0]..      
-0000b350: 2020 2020 2020 7369 6c65 6e74 5f74 696d        silent_tim
-0000b360: 696e 6773 203d 2067 6574 5f76 6164 5f73  ings = get_vad_s
-0000b370: 696c 656e 6365 5f66 756e 6328 0d0a 2020  ilence_func(..  
-0000b380: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
-0000b390: 6e78 3d76 6164 5f6f 6e6e 782c 0d0a 2020  nx=vad_onnx,..  
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 7665                ve
-0000b3b0: 7262 6f73 653d 7665 7262 6f73 650d 0a20  rbose=verbose.. 
-0000b3c0: 2020 2020 2020 2020 2020 2029 2861 7564             )(aud
-0000b3d0: 696f 2c20 7370 6565 6368 5f74 6872 6573  io, speech_thres
-0000b3e0: 686f 6c64 3d76 6164 5f74 6872 6573 686f  hold=vad_thresho
-0000b3f0: 6c64 2c20 7372 3d73 616d 706c 655f 7261  ld, sr=sample_ra
-0000b400: 7465 290d 0a20 2020 2020 2020 2065 6c73  te)..        els
-0000b410: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000b420: 7369 6c65 6e74 5f74 696d 696e 6773 203d  silent_timings =
-0000b430: 2061 7564 696f 3274 696d 696e 6773 2861   audio2timings(a
-0000b440: 7564 696f 2c20 715f 6c65 7665 6c73 3d71  udio, q_levels=q
-0000b450: 5f6c 6576 656c 732c 206b 5f73 697a 653d  _levels, k_size=
-0000b460: 6b5f 7369 7a65 2c20 7372 3d73 616d 706c  k_size, sr=sampl
-0000b470: 655f 7261 7465 290d 0a20 2020 2020 2020  e_rate)..       
-0000b480: 2069 6620 7369 6c65 6e74 5f74 696d 696e   if silent_timin
-0000b490: 6773 2069 7320 4e6f 6e65 3a0d 0a20 2020  gs is None:..   
-0000b4a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000b4b0: 7365 6c66 0d0a 2020 2020 2020 2020 7365  self..        se
-0000b4c0: 6c66 2e73 7570 7072 6573 735f 7369 6c65  lf.suppress_sile
-0000b4d0: 6e63 6528 0d0a 2020 2020 2020 2020 2020  nce(..          
-0000b4e0: 2020 2a73 696c 656e 745f 7469 6d69 6e67    *silent_timing
-0000b4f0: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-0000b500: 6d69 6e5f 776f 7264 5f64 7572 3d6d 696e  min_word_dur=min
-0000b510: 5f77 6f72 645f 6475 722c 0d0a 2020 2020  _word_dur,..    
-0000b520: 2020 2020 2020 2020 776f 7264 5f6c 6576          word_lev
-0000b530: 656c 3d77 6f72 645f 6c65 7665 6c2c 0d0a  el=word_level,..
-0000b540: 2020 2020 2020 2020 2020 2020 6e6f 6e73              nons
-0000b550: 7065 6563 685f 6572 726f 723d 6e6f 6e73  peech_error=nons
-0000b560: 7065 6563 685f 6572 726f 722c 0d0a 2020  peech_error,..  
-0000b570: 2020 2020 2020 2020 2020 7573 655f 776f            use_wo
-0000b580: 7264 5f70 6f73 6974 696f 6e3d 7573 655f  rd_position=use_
-0000b590: 776f 7264 5f70 6f73 6974 696f 6e2c 0d0a  word_position,..
-0000b5a0: 2020 2020 2020 2020 2020 2020 7665 7262              verb
-0000b5b0: 6f73 653d 7665 7262 6f73 650d 0a20 2020  ose=verbose..   
-0000b5c0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0000b5d0: 7365 6c66 2e75 7064 6174 655f 6e6f 6e73  self.update_nons
-0000b5e0: 7065 6563 685f 7365 6374 696f 6e73 282a  peech_sections(*
-0000b5f0: 7369 6c65 6e74 5f74 696d 696e 6773 290d  silent_timings).
-0000b600: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000b610: 7365 6c66 0d0a 0d0a 2020 2020 6465 6620  self....    def 
-0000b620: 6164 6a75 7374 5f62 795f 7265 7375 6c74  adjust_by_result
-0000b630: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
-0000b640: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
-0000b650: 2020 6f74 6865 725f 7265 7375 6c74 3a20    other_result: 
-0000b660: 2257 6869 7370 6572 5265 7375 6c74 222c  "WhisperResult",
-0000b670: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
-0000b680: 6e5f 776f 7264 5f64 7572 3a20 4f70 7469  n_word_dur: Opti
-0000b690: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
-0000b6a0: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-0000b6b0: 2076 6572 626f 7365 3a20 626f 6f6c 203d   verbose: bool =
-0000b6c0: 2046 616c 7365 0d0a 2020 2020 293a 0d0a   False..    ):..
-0000b6d0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0000b6e0: 2020 2020 204d 696e 696d 697a 6520 7468       Minimize th
-0000b6f0: 6520 6475 7261 7469 6f6e 206f 6620 776f  e duration of wo
-0000b700: 7264 7320 7573 696e 6720 7469 6d65 7374  rds using timest
-0000b710: 616d 7073 206f 6620 616e 6f74 6865 7220  amps of another 
-0000b720: 7265 7375 6c74 2e0d 0a0d 0a20 2020 2020  result.....     
-0000b730: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
-0000b740: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0000b750: 2d0d 0a20 2020 2020 2020 206f 7468 6572  -..        other
-0000b760: 5f72 6573 756c 7420 3a20 2257 6869 7370  _result : "Whisp
-0000b770: 6572 5265 7375 6c74 220d 0a20 2020 2020  erResult"..     
-0000b780: 2020 2020 2020 2054 696d 696e 6720 6461         Timing da
-0000b790: 7461 206f 6620 7468 6520 7361 6d65 2077  ta of the same w
-0000b7a0: 6f72 6473 2069 6e20 6120 5768 6973 7065  ords in a Whispe
-0000b7b0: 7252 6573 756c 7420 696e 7374 616e 6365  rResult instance
-0000b7c0: 2e0d 0a20 2020 2020 2020 206d 696e 5f77  ...        min_w
-0000b7d0: 6f72 645f 6475 7220 3a20 666c 6f61 7420  ord_dur : float 
-0000b7e0: 6f72 204e 6f6e 652c 2064 6566 6175 6c74  or None, default
-0000b7f0: 204e 6f6e 6520 6d65 616e 696e 6720 7573   None meaning us
-0000b800: 6520 6060 7374 6162 6c65 5f77 6869 7370  e ``stable_whisp
-0000b810: 6572 2e64 6566 6175 6c74 2e44 4546 4155  er.default.DEFAU
-0000b820: 4c54 5f56 414c 5545 5360 600d 0a20 2020  LT_VALUES``..   
-0000b830: 2020 2020 2020 2020 2050 7265 7665 6e74           Prevent
-0000b840: 2063 6861 6e67 6573 2074 6f20 7469 6d65   changes to time
-0000b850: 7374 616d 7073 2069 6620 7468 6520 7265  stamps if the re
-0000b860: 7375 6c74 616e 7420 776f 7264 2064 7572  sultant word dur
-0000b870: 6174 696f 6e20 6973 206c 6573 7320 7468  ation is less th
-0000b880: 616e 2060 606d 696e 5f77 6f72 645f 6475  an ``min_word_du
-0000b890: 7260 602e 0d0a 2020 2020 2020 2020 7665  r``...        ve
-0000b8a0: 7262 6f73 6520 3a20 626f 6f6c 2c20 6465  rbose : bool, de
-0000b8b0: 6661 756c 7420 4661 6c73 650d 0a20 2020  fault False..   
-0000b8c0: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
-0000b8d0: 2074 6f20 7072 696e 7420 6f75 7420 7468   to print out th
-0000b8e0: 6520 7469 6d65 7374 616d 7020 6368 616e  e timestamp chan
-0000b8f0: 6765 732e 0d0a 2020 2020 2020 2020 2222  ges...        ""
-0000b900: 220d 0a20 2020 2020 2020 2069 6620 6e6f  "..        if no
-0000b910: 7420 2873 656c 662e 6861 735f 776f 7264  t (self.has_word
-0000b920: 7320 616e 6420 6f74 6865 725f 7265 7375  s and other_resu
-0000b930: 6c74 2e68 6173 5f77 6f72 6473 293a 0d0a  lt.has_words):..
-0000b940: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000b950: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
-0000b960: 4572 726f 7228 2754 6869 7320 6f70 6572  Error('This oper
-0000b970: 6174 696f 6e20 6361 6e20 6f6e 6c79 2062  ation can only b
-0000b980: 6520 7065 7266 6f72 6d65 6420 6f6e 2072  e performed on r
-0000b990: 6573 756c 7473 2077 6974 6820 776f 7264  esults with word
-0000b9a0: 2074 696d 6573 7461 6d70 7327 290d 0a20   timestamps').. 
-0000b9b0: 2020 2020 2020 2061 7373 6572 7420 5b77         assert [w
-0000b9c0: 2e77 6f72 6420 666f 7220 7720 696e 2073  .word for w in s
-0000b9d0: 656c 662e 616c 6c5f 776f 7264 7328 295d  elf.all_words()]
-0000b9e0: 203d 3d20 5b77 2e77 6f72 6420 666f 7220   == [w.word for 
-0000b9f0: 7720 696e 206f 7468 6572 5f72 6573 756c  w in other_resul
-0000ba00: 742e 616c 6c5f 776f 7264 7328 295d 2c20  t.all_words()], 
-0000ba10: 5c0d 0a20 2020 2020 2020 2020 2020 2027  \..            '
-0000ba20: 5468 6520 776f 7264 7320 696e 205b 6f74  The words in [ot
-0000ba30: 6865 725f 7265 7375 6c74 5d20 646f 206e  her_result] do n
-0000ba40: 6f74 206d 6174 6368 2074 6865 2063 7572  ot match the cur
-0000ba50: 7265 6e74 2077 6f72 6473 2e27 0d0a 2020  rent words.'..  
-0000ba60: 2020 2020 2020 6d69 6e5f 776f 7264 5f64        min_word_d
-0000ba70: 7572 203d 2067 6574 5f6d 696e 5f77 6f72  ur = get_min_wor
-0000ba80: 645f 6475 7228 6d69 6e5f 776f 7264 5f64  d_dur(min_word_d
-0000ba90: 7572 290d 0a20 2020 2020 2020 2066 6f72  ur)..        for
-0000baa0: 2077 6f72 642c 206f 7468 6572 5f77 6f72   word, other_wor
-0000bab0: 6420 696e 207a 6970 2873 656c 662e 616c  d in zip(self.al
-0000bac0: 6c5f 776f 7264 7328 292c 206f 7468 6572  l_words(), other
-0000bad0: 5f72 6573 756c 742e 616c 6c5f 776f 7264  _result.all_word
-0000bae0: 7328 2929 3a0d 0a20 2020 2020 2020 2020  s()):..         
-0000baf0: 2020 2069 6620 776f 7264 2e65 6e64 203e     if word.end >
-0000bb00: 206f 7468 6572 5f77 6f72 642e 7374 6172   other_word.star
-0000bb10: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-0000bb20: 2020 2020 6e65 775f 7374 6172 7420 3d20      new_start = 
-0000bb30: 6d61 7828 776f 7264 2e73 7461 7274 2c20  max(word.start, 
-0000bb40: 6f74 6865 725f 776f 7264 2e73 7461 7274  other_word.start
-0000bb50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000bb60: 2020 206e 6577 5f65 6e64 203d 206d 696e     new_end = min
-0000bb70: 2877 6f72 642e 656e 642c 206f 7468 6572  (word.end, other
-0000bb80: 5f77 6f72 642e 656e 6429 0d0a 2020 2020  _word.end)..    
-0000bb90: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000bba0: 6577 5f65 6e64 202d 206e 6577 5f73 7461  ew_end - new_sta
-0000bbb0: 7274 203e 3d20 6d69 6e5f 776f 7264 5f64  rt >= min_word_d
-0000bbc0: 7572 3a0d 0a20 2020 2020 2020 2020 2020  ur:..           
-0000bbd0: 2020 2020 2020 2020 206c 696e 6520 3d20           line = 
-0000bbe0: 2727 0d0a 2020 2020 2020 2020 2020 2020  ''..            
-0000bbf0: 2020 2020 2020 2020 6966 2077 6f72 642e          if word.
-0000bc00: 7374 6172 7420 213d 206e 6577 5f73 7461  start != new_sta
-0000bc10: 7274 3a0d 0a20 2020 2020 2020 2020 2020  rt:..           
-0000bc20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000bc30: 7665 7262 6f73 653a 0d0a 2020 2020 2020  verbose:..      
-0000bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc50: 2020 2020 2020 6c69 6e65 202b 3d20 6627        line += f'
-0000bc60: 5b53 7461 7274 3a7b 776f 7264 2e73 7461  [Start:{word.sta
-0000bc70: 7274 3a2e 3366 7d2d 3e7b 6e65 775f 7374  rt:.3f}->{new_st
-0000bc80: 6172 743a 2e33 667d 5d20 270d 0a20 2020  art:.3f}] '..   
-0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 2020 2020 2077 6f72 642e 7374 6172 7420       word.start 
-0000bcb0: 3d20 6e65 775f 7374 6172 740d 0a20 2020  = new_start..   
-0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcd0: 2069 6620 776f 7264 2e65 6e64 2021 3d20   if word.end != 
-0000bce0: 6e65 775f 656e 643a 0d0a 2020 2020 2020  new_end:..      
-0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd00: 2020 6966 2076 6572 626f 7365 3a0d 0a20    if verbose:.. 
-0000bd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd20: 2020 2020 2020 2020 2020 206c 696e 6520             line 
-0000bd30: 2b3d 2066 275b 456e 643a 7b77 6f72 642e  += f'[End:{word.
-0000bd40: 656e 643a 2e33 667d 2d3e 7b6e 6577 5f65  end:.3f}->{new_e
-0000bd50: 6e64 3a2e 3366 7d5d 2020 270d 0a20 2020  nd:.3f}]  '..   
-0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd70: 2020 2020 2077 6f72 642e 656e 6420 3d20       word.end = 
-0000bd80: 6e65 775f 656e 640d 0a20 2020 2020 2020  new_end..       
-0000bd90: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000bda0: 6c69 6e65 3a0d 0a20 2020 2020 2020 2020  line:..         
-0000bdb0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000bdc0: 7269 6e74 2866 277b 6c69 6e65 7d22 7b77  rint(f'{line}"{w
-0000bdd0: 6f72 642e 776f 7264 7d22 2729 0d0a 0d0a  ord.word}"')....
-0000bde0: 2020 2020 6465 6620 7265 6173 7369 676e      def reassign
-0000bdf0: 5f69 6473 2873 656c 662c 206f 6e6c 795f  _ids(self, only_
-0000be00: 7365 676d 656e 7473 3a20 626f 6f6c 203d  segments: bool =
-0000be10: 2046 616c 7365 2c20 7374 6172 743a 204f   False, start: O
-0000be20: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-0000be30: 6f6e 6529 3a0d 0a20 2020 2020 2020 2066  one):..        f
-0000be40: 6f72 2069 2c20 7320 696e 2065 6e75 6d65  or i, s in enume
-0000be50: 7261 7465 2873 656c 662e 7365 676d 656e  rate(self.segmen
-0000be60: 7473 5b73 7461 7274 3a5d 2c20 7374 6172  ts[start:], star
-0000be70: 7420 6f72 2030 293a 0d0a 2020 2020 2020  t or 0):..      
-0000be80: 2020 2020 2020 732e 6964 203d 2069 0d0a        s.id = i..
-0000be90: 2020 2020 2020 2020 2020 2020 732e 7265              s.re
-0000bea0: 7375 6c74 203d 2073 656c 660d 0a20 2020  sult = self..   
-0000beb0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0000bec0: 6f6e 6c79 5f73 6567 6d65 6e74 733a 0d0a  only_segments:..
-0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bee0: 732e 7265 6173 7369 676e 5f69 6473 2829  s.reassign_ids()
-0000bef0: 0d0a 0d0a 2020 2020 6465 6620 7265 6d6f  ....    def remo
-0000bf00: 7665 5f6e 6f5f 776f 7264 5f73 6567 6d65  ve_no_word_segme
-0000bf10: 6e74 7328 7365 6c66 2c20 6967 6e6f 7265  nts(self, ignore
-0000bf20: 5f6f 7269 3d46 616c 7365 2c20 7265 6173  _ori=False, reas
-0000bf30: 7369 676e 5f69 6473 3a20 626f 6f6c 203d  sign_ids: bool =
-0000bf40: 2054 7275 6529 3a0d 0a20 2020 2020 2020   True):..       
-0000bf50: 2066 6f72 2069 2069 6e20 7265 7665 7273   for i in revers
-0000bf60: 6564 2872 616e 6765 286c 656e 2873 656c  ed(range(len(sel
-0000bf70: 662e 7365 676d 656e 7473 2929 293a 0d0a  f.segments))):..
-0000bf80: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-0000bf90: 6967 6e6f 7265 5f6f 7269 206f 7220 7365  ignore_ori or se
-0000bfa0: 6c66 2e73 6567 6d65 6e74 735b 695d 2e6f  lf.segments[i].o
-0000bfb0: 7269 5f68 6173 5f77 6f72 6473 2920 616e  ri_has_words) an
-0000bfc0: 6420 6e6f 7420 7365 6c66 2e73 6567 6d65  d not self.segme
-0000bfd0: 6e74 735b 695d 2e68 6173 5f77 6f72 6473  nts[i].has_words
-0000bfe0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000bff0: 2020 2064 656c 2073 656c 662e 7365 676d     del self.segm
-0000c000: 656e 7473 5b69 5d0d 0a20 2020 2020 2020  ents[i]..       
-0000c010: 2069 6620 7265 6173 7369 676e 5f69 6473   if reassign_ids
-0000c020: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-0000c030: 656c 662e 7265 6173 7369 676e 5f69 6473  elf.reassign_ids
-0000c040: 2829 0d0a 0d0a 2020 2020 6465 6620 6765  ()....    def ge
-0000c050: 745f 6c6f 636b 6564 5f69 6e64 6963 6573  t_locked_indices
-0000c060: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-0000c070: 206c 6f63 6b65 645f 696e 6469 6365 7320   locked_indices 
-0000c080: 3d20 5b69 0d0a 2020 2020 2020 2020 2020  = [i..          
-0000c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0a0: 666f 7220 692c 2028 6c65 6674 2c20 7269  for i, (left, ri
-0000c0b0: 6768 7429 2069 6e20 656e 756d 6572 6174  ght) in enumerat
-0000c0c0: 6528 7a69 7028 7365 6c66 2e73 6567 6d65  e(zip(self.segme
-0000c0d0: 6e74 735b 313a 5d2c 2073 656c 662e 7365  nts[1:], self.se
-0000c0e0: 676d 656e 7473 5b3a 2d31 5d29 290d 0a20  gments[:-1])).. 
-0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c100: 2020 2020 2020 2020 2069 6620 6c65 6674           if left
-0000c110: 2e6c 6566 745f 6c6f 636b 6564 206f 7220  .left_locked or 
-0000c120: 7269 6768 742e 7269 6768 745f 6c6f 636b  right.right_lock
-0000c130: 6564 5d0d 0a20 2020 2020 2020 2072 6574  ed]..        ret
-0000c140: 7572 6e20 6c6f 636b 6564 5f69 6e64 6963  urn locked_indic
-0000c150: 6573 0d0a 0d0a 2020 2020 6465 6620 6765  es....    def ge
-0000c160: 745f 6761 7073 2873 656c 662c 2061 735f  t_gaps(self, as_
-0000c170: 6e64 6172 7261 793d 4661 6c73 6529 3a0d  ndarray=False):.
-0000c180: 0a20 2020 2020 2020 2073 5f74 7320 3d20  .        s_ts = 
-0000c190: 6e70 2e61 7272 6179 285b 732e 7374 6172  np.array([s.star
-0000c1a0: 7420 666f 7220 7320 696e 2073 656c 662e  t for s in self.
-0000c1b0: 7365 676d 656e 7473 5d29 0d0a 2020 2020  segments])..    
-0000c1c0: 2020 2020 655f 7473 203d 206e 702e 6172      e_ts = np.ar
-0000c1d0: 7261 7928 5b73 2e65 6e64 2066 6f72 2073  ray([s.end for s
-0000c1e0: 2069 6e20 7365 6c66 2e73 6567 6d65 6e74   in self.segment
-0000c1f0: 735d 290d 0a20 2020 2020 2020 2067 6170  s])..        gap
-0000c200: 203d 2073 5f74 735b 313a 5d20 2d20 655f   = s_ts[1:] - e_
-0000c210: 7473 5b3a 2d31 5d0d 0a20 2020 2020 2020  ts[:-1]..       
-0000c220: 2072 6574 7572 6e20 6761 7020 6966 2061   return gap if a
-0000c230: 735f 6e64 6172 7261 7920 656c 7365 2067  s_ndarray else g
-0000c240: 6170 2e74 6f6c 6973 7428 290d 0a0d 0a20  ap.tolist().... 
-0000c250: 2020 2064 6566 2067 6574 5f67 6170 5f69     def get_gap_i
-0000c260: 6e64 6963 6573 2873 656c 662c 206d 696e  ndices(self, min
-0000c270: 5f67 6170 3a20 666c 6f61 7420 3d20 302e  _gap: float = 0.
-0000c280: 3129 3a20 2023 2066 6f72 206d 6572 6769  1):  # for mergi
-0000c290: 6e67 0d0a 2020 2020 2020 2020 6966 206c  ng..        if l
-0000c2a0: 656e 2873 656c 662e 7365 676d 656e 7473  en(self.segments
-0000c2b0: 2920 3c20 323a 0d0a 2020 2020 2020 2020  ) < 2:..        
-0000c2c0: 2020 2020 7265 7475 726e 205b 5d0d 0a20      return [].. 
-0000c2d0: 2020 2020 2020 2069 6620 6d69 6e5f 6761         if min_ga
-0000c2e0: 7020 6973 204e 6f6e 653a 0d0a 2020 2020  p is None:..    
-0000c2f0: 2020 2020 2020 2020 6d69 6e5f 6761 7020          min_gap 
-0000c300: 3d20 300d 0a20 2020 2020 2020 2069 6e64  = 0..        ind
-0000c310: 6963 6573 203d 2028 7365 6c66 2e67 6574  ices = (self.get
-0000c320: 5f67 6170 7328 5472 7565 2920 3c3d 206d  _gaps(True) <= m
-0000c330: 696e 5f67 6170 292e 6e6f 6e7a 6572 6f28  in_gap).nonzero(
-0000c340: 295b 305d 2e74 6f6c 6973 7428 290d 0a20  )[0].tolist().. 
-0000c350: 2020 2020 2020 2072 6574 7572 6e20 736f         return so
-0000c360: 7274 6564 2873 6574 2869 6e64 6963 6573  rted(set(indices
-0000c370: 2920 2d20 7365 7428 7365 6c66 2e67 6574  ) - set(self.get
-0000c380: 5f6c 6f63 6b65 645f 696e 6469 6365 7328  _locked_indices(
-0000c390: 2929 290d 0a0d 0a20 2020 2064 6566 2067  )))....    def g
-0000c3a0: 6574 5f70 756e 6374 7561 7469 6f6e 5f69  et_punctuation_i
-0000c3b0: 6e64 6963 6573 2873 656c 662c 2070 756e  ndices(self, pun
-0000c3c0: 6374 7561 7469 6f6e 3a20 556e 696f 6e5b  ctuation: Union[
-0000c3d0: 4c69 7374 5b73 7472 5d2c 204c 6973 745b  List[str], List[
-0000c3e0: 5475 706c 655b 7374 722c 2073 7472 5d5d  Tuple[str, str]]
-0000c3f0: 2c20 7374 725d 293a 2020 2320 666f 7220  , str]):  # for 
-0000c400: 6d65 7267 696e 670d 0a20 2020 2020 2020  merging..       
-0000c410: 2069 6620 6c65 6e28 7365 6c66 2e73 6567   if len(self.seg
-0000c420: 6d65 6e74 7329 203c 2032 3a0d 0a20 2020  ments) < 2:..   
-0000c430: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000c440: 5b5d 0d0a 2020 2020 2020 2020 6966 2069  []..        if i
-0000c450: 7369 6e73 7461 6e63 6528 7075 6e63 7475  sinstance(punctu
-0000c460: 6174 696f 6e2c 2073 7472 293a 0d0a 2020  ation, str):..  
-0000c470: 2020 2020 2020 2020 2020 7075 6e63 7475            punctu
-0000c480: 6174 696f 6e20 3d20 5b70 756e 6374 7561  ation = [punctua
-0000c490: 7469 6f6e 5d0d 0a20 2020 2020 2020 2069  tion]..        i
-0000c4a0: 6e64 6963 6573 203d 205b 5d0d 0a20 2020  ndices = []..   
-0000c4b0: 2020 2020 2066 6f72 2070 2069 6e20 7075       for p in pu
-0000c4c0: 6e63 7475 6174 696f 6e3a 0d0a 2020 2020  nctuation:..    
-0000c4d0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000c4e0: 7461 6e63 6528 702c 2073 7472 293a 0d0a  tance(p, str):..
-0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c500: 666f 7220 692c 2073 2069 6e20 656e 756d  for i, s in enum
-0000c510: 6572 6174 6528 7365 6c66 2e73 6567 6d65  erate(self.segme
-0000c520: 6e74 735b 3a2d 315d 293a 0d0a 2020 2020  nts[:-1]):..    
-0000c530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c540: 6966 2073 2e74 6578 742e 656e 6473 7769  if s.text.endswi
-0000c550: 7468 2870 293a 0d0a 2020 2020 2020 2020  th(p):..        
-0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c570: 696e 6469 6365 732e 6170 7065 6e64 2869  indices.append(i
-0000c580: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000c590: 2020 2020 2020 2065 6c69 6620 6920 213d         elif i !=
-0000c5a0: 2030 2061 6e64 2073 2e74 6578 742e 7374   0 and s.text.st
-0000c5b0: 6172 7473 7769 7468 2870 293a 0d0a 2020  artswith(p):..  
-0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5d0: 2020 2020 2020 696e 6469 6365 732e 6170        indices.ap
-0000c5e0: 7065 6e64 2869 2d31 290d 0a20 2020 2020  pend(i-1)..     
-0000c5f0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000c600: 2020 2020 2020 2020 2020 2020 2020 656e                en
-0000c610: 6469 6e67 2c20 6265 6769 6e6e 696e 6720  ding, beginning 
-0000c620: 3d20 700d 0a20 2020 2020 2020 2020 2020  = p..           
-0000c630: 2020 2020 2069 6e64 6963 6573 2e65 7874       indices.ext
-0000c640: 656e 6428 5b69 2066 6f72 2069 2c20 2873  end([i for i, (s
-0000c650: 302c 2073 3129 2069 6e20 656e 756d 6572  0, s1) in enumer
-0000c660: 6174 6528 7a69 7028 7365 6c66 2e73 6567  ate(zip(self.seg
-0000c670: 6d65 6e74 735b 3a2d 315d 2c20 7365 6c66  ments[:-1], self
-0000c680: 2e73 6567 6d65 6e74 735b 313a 5d29 290d  .segments[1:])).
-0000c690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6b0: 2069 6620 7330 2e74 6578 742e 656e 6473   if s0.text.ends
-0000c6c0: 7769 7468 2865 6e64 696e 6729 2061 6e64  with(ending) and
-0000c6d0: 2073 312e 7465 7874 2e73 7461 7274 7377   s1.text.startsw
-0000c6e0: 6974 6828 6265 6769 6e6e 696e 6729 5d29  ith(beginning)])
-0000c6f0: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-0000c700: 726e 2073 6f72 7465 6428 7365 7428 696e  rn sorted(set(in
-0000c710: 6469 6365 7329 202d 2073 6574 2873 656c  dices) - set(sel
-0000c720: 662e 6765 745f 6c6f 636b 6564 5f69 6e64  f.get_locked_ind
-0000c730: 6963 6573 2829 2929 0d0a 0d0a 2020 2020  ices()))....    
-0000c740: 6465 6620 616c 6c5f 776f 7264 7328 7365  def all_words(se
-0000c750: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-0000c760: 7475 726e 206c 6973 7428 6368 6169 6e2e  turn list(chain.
-0000c770: 6672 6f6d 5f69 7465 7261 626c 6528 732e  from_iterable(s.
-0000c780: 776f 7264 7320 666f 7220 7320 696e 2073  words for s in s
-0000c790: 656c 662e 7365 676d 656e 7473 2929 0d0a  elf.segments))..
-0000c7a0: 0d0a 2020 2020 6465 6620 616c 6c5f 776f  ..    def all_wo
-0000c7b0: 7264 735f 6f72 5f73 6567 6d65 6e74 7328  rds_or_segments(
-0000c7c0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-0000c7d0: 7265 7475 726e 2073 656c 662e 616c 6c5f  return self.all_
-0000c7e0: 776f 7264 7328 2920 6966 2073 656c 662e  words() if self.
-0000c7f0: 6861 735f 776f 7264 7320 656c 7365 2073  has_words else s
-0000c800: 656c 662e 7365 676d 656e 7473 0d0a 0d0a  elf.segments....
-0000c810: 2020 2020 6465 6620 616c 6c5f 776f 7264      def all_word
-0000c820: 735f 6279 5f6c 6f63 6b28 7365 6c66 2c20  s_by_lock(self, 
-0000c830: 6f6e 6c79 5f74 6578 743a 2062 6f6f 6c20  only_text: bool 
-0000c840: 3d20 5472 7565 2c20 6279 5f73 6567 6d65  = True, by_segme
-0000c850: 6e74 3a20 626f 6f6c 203d 2046 616c 7365  nt: bool = False
-0000c860: 2c20 696e 636c 7564 655f 7369 6e67 6c65  , include_single
-0000c870: 3a20 626f 6f6c 203d 2046 616c 7365 293a  : bool = False):
-0000c880: 0d0a 2020 2020 2020 2020 6966 2062 795f  ..        if by_
-0000c890: 7365 676d 656e 743a 0d0a 2020 2020 2020  segment:..      
-0000c8a0: 2020 2020 2020 7265 7475 726e 205b 0d0a        return [..
-0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8c0: 7365 676d 656e 742e 776f 7264 735f 6279  segment.words_by
-0000c8d0: 5f6c 6f63 6b28 6f6e 6c79 5f74 6578 743d  _lock(only_text=
-0000c8e0: 6f6e 6c79 5f74 6578 742c 2069 6e63 6c75  only_text, inclu
-0000c8f0: 6465 5f73 696e 676c 653d 696e 636c 7564  de_single=includ
-0000c900: 655f 7369 6e67 6c65 290d 0a20 2020 2020  e_single)..     
-0000c910: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-0000c920: 6567 6d65 6e74 2069 6e20 7365 6c66 2e73  egment in self.s
-0000c930: 6567 6d65 6e74 730d 0a20 2020 2020 2020  egments..       
-0000c940: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
-0000c950: 7265 7475 726e 205f 776f 7264 735f 6279  return _words_by
-0000c960: 5f6c 6f63 6b28 7365 6c66 2e61 6c6c 5f77  _lock(self.all_w
-0000c970: 6f72 6473 2829 2c20 6f6e 6c79 5f74 6578  ords(), only_tex
-0000c980: 743d 6f6e 6c79 5f74 6578 742c 2069 6e63  t=only_text, inc
-0000c990: 6c75 6465 5f73 696e 676c 653d 696e 636c  lude_single=incl
-0000c9a0: 7564 655f 7369 6e67 6c65 290d 0a0d 0a20  ude_single).... 
-0000c9b0: 2020 2064 6566 2061 6c6c 5f74 6f6b 656e     def all_token
-0000c9c0: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
-0000c9d0: 2020 7265 7475 726e 206c 6973 7428 6368    return list(ch
-0000c9e0: 6169 6e2e 6672 6f6d 5f69 7465 7261 626c  ain.from_iterabl
-0000c9f0: 6528 732e 746f 6b65 6e73 2066 6f72 2073  e(s.tokens for s
-0000ca00: 2069 6e20 7365 6c66 2e61 6c6c 5f77 6f72   in self.all_wor
-0000ca10: 6473 2829 2929 0d0a 0d0a 2020 2020 6465  ds()))....    de
-0000ca20: 6620 746f 5f64 6963 7428 7365 6c66 293a  f to_dict(self):
-0000ca30: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000ca40: 2064 6963 7428 7465 7874 3d73 656c 662e   dict(text=self.
-0000ca50: 7465 7874 2c0d 0a20 2020 2020 2020 2020  text,..         
-0000ca60: 2020 2020 2020 2020 2020 2073 6567 6d65             segme
-0000ca70: 6e74 733d 7365 6c66 2e73 6567 6d65 6e74  nts=self.segment
-0000ca80: 735f 746f 5f64 6963 7473 2829 2c0d 0a20  s_to_dicts(),.. 
-0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000caa0: 2020 206c 616e 6775 6167 653d 7365 6c66     language=self
-0000cab0: 2e6c 616e 6775 6167 652c 0d0a 2020 2020  .language,..    
-0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cad0: 6f72 695f 6469 6374 3d73 656c 662e 6f72  ori_dict=self.or
-0000cae0: 695f 6469 6374 2c0d 0a20 2020 2020 2020  i_dict,..       
-0000caf0: 2020 2020 2020 2020 2020 2020 2072 6567               reg
-0000cb00: 726f 7570 5f68 6973 746f 7279 3d73 656c  roup_history=sel
-0000cb10: 662e 5f72 6567 726f 7570 5f68 6973 746f  f._regroup_histo
-0000cb20: 7279 2c0d 0a20 2020 2020 2020 2020 2020  ry,..           
-0000cb30: 2020 2020 2020 2020 206e 6f6e 7370 6565           nonspee
-0000cb40: 6368 5f73 6563 7469 6f6e 733d 7365 6c66  ch_sections=self
-0000cb50: 2e5f 6e6f 6e73 7065 6563 685f 7365 6374  ._nonspeech_sect
-0000cb60: 696f 6e73 290d 0a0d 0a20 2020 2064 6566  ions)....    def
-0000cb70: 2073 6567 6d65 6e74 735f 746f 5f64 6963   segments_to_dic
-0000cb80: 7473 2873 656c 662c 2072 6576 6572 7365  ts(self, reverse
-0000cb90: 5f74 6578 743a 2055 6e69 6f6e 5b62 6f6f  _text: Union[boo
-0000cba0: 6c2c 2074 7570 6c65 5d20 3d20 4661 6c73  l, tuple] = Fals
-0000cbb0: 6529 3a0d 0a20 2020 2020 2020 2072 6574  e):..        ret
-0000cbc0: 7572 6e20 5b73 2e74 6f5f 6469 6374 2872  urn [s.to_dict(r
-0000cbd0: 6576 6572 7365 5f74 6578 743d 7265 7665  everse_text=reve
-0000cbe0: 7273 655f 7465 7874 2920 666f 7220 7320  rse_text) for s 
-0000cbf0: 696e 2073 656c 662e 7365 676d 656e 7473  in self.segments
-0000cc00: 5d0d 0a0d 0a20 2020 2064 6566 205f 7370  ]....    def _sp
-0000cc10: 6c69 745f 7365 676d 656e 7473 2873 656c  lit_segments(sel
-0000cc20: 662c 2067 6574 5f69 6e64 6963 6573 2c20  f, get_indices, 
-0000cc30: 6172 6773 3a20 6c69 7374 203d 204e 6f6e  args: list = Non
-0000cc40: 652c 202a 2c20 6c6f 636b 3a20 626f 6f6c  e, *, lock: bool
-0000cc50: 203d 2046 616c 7365 2c20 6e65 776c 696e   = False, newlin
-0000cc60: 653a 2062 6f6f 6c20 3d20 4661 6c73 6529  e: bool = False)
-0000cc70: 3a0d 0a20 2020 2020 2020 2069 6620 6172  :..        if ar
-0000cc80: 6773 2069 7320 4e6f 6e65 3a0d 0a20 2020  gs is None:..   
-0000cc90: 2020 2020 2020 2020 2061 7267 7320 3d20           args = 
-0000cca0: 5b5d 0d0a 2020 2020 2020 2020 6e6f 5f77  []..        no_w
-0000ccb0: 6f72 6473 203d 2046 616c 7365 0d0a 2020  ords = False..  
-0000ccc0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-0000ccd0: 6576 6572 7365 6428 7261 6e67 6528 302c  eversed(range(0,
-0000cce0: 206c 656e 2873 656c 662e 7365 676d 656e   len(self.segmen
-0000ccf0: 7473 2929 293a 0d0a 2020 2020 2020 2020  ts))):..        
-0000cd00: 2020 2020 6e6f 5f77 6f72 6473 203d 206e      no_words = n
-0000cd10: 6f5f 776f 7264 7320 6f72 206e 6f74 2073  o_words or not s
-0000cd20: 656c 662e 7365 676d 656e 7473 5b69 5d2e  elf.segments[i].
-0000cd30: 6861 735f 776f 7264 730d 0a20 2020 2020  has_words..     
-0000cd40: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
-0000cd50: 2073 6f72 7465 6428 7365 7428 6765 745f   sorted(set(get_
-0000cd60: 696e 6469 6365 7328 7365 6c66 2e73 6567  indices(self.seg
-0000cd70: 6d65 6e74 735b 695d 2c20 2a61 7267 7329  ments[i], *args)
-0000cd80: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000cd90: 6966 206e 6f74 2069 6e64 6963 6573 3a0d  if not indices:.
-0000cda0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cdb0: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
-0000cdc0: 2020 2020 2020 2069 6620 6e65 776c 696e         if newlin
-0000cdd0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000cde0: 2020 2020 6966 2069 6e64 6963 6573 5b2d      if indices[-
-0000cdf0: 315d 203d 3d20 6c65 6e28 7365 6c66 2e73  1] == len(self.s
-0000ce00: 6567 6d65 6e74 735b 695d 2e77 6f72 6473  egments[i].words
-0000ce10: 2920 2d20 313a 0d0a 2020 2020 2020 2020  ) - 1:..        
-0000ce20: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-0000ce30: 696e 6469 6365 735b 2d31 5d0d 0a20 2020  indices[-1]..   
-0000ce40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce50: 2069 6620 6e6f 7420 696e 6469 6365 733a   if not indices:
-0000ce60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ce70: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0000ce80: 7565 0d0a 0d0a 2020 2020 2020 2020 2020  ue....          
-0000ce90: 2020 2020 2020 666f 7220 776f 7264 5f69        for word_i
-0000cea0: 6478 2069 6e20 696e 6469 6365 733a 0d0a  dx in indices:..
-0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cec0: 2020 2020 6966 2073 656c 662e 7365 676d      if self.segm
-0000ced0: 656e 7473 5b69 5d2e 776f 7264 735b 776f  ents[i].words[wo
-0000cee0: 7264 5f69 6478 5d2e 776f 7264 2e65 6e64  rd_idx].word.end
-0000cef0: 7377 6974 6828 275c 6e27 293a 0d0a 2020  swith('\n'):..  
-0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf10: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
-0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf30: 2020 2020 7365 6c66 2e73 6567 6d65 6e74      self.segment
-0000cf40: 735b 695d 2e77 6f72 6473 5b77 6f72 645f  s[i].words[word_
-0000cf50: 6964 785d 2e77 6f72 6420 2b3d 2027 5c6e  idx].word += '\n
-0000cf60: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-0000cf70: 2020 2020 2020 2069 6620 6c6f 636b 3a0d         if lock:.
-0000cf80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cf90: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0000cfa0: 676d 656e 7473 5b69 5d2e 776f 7264 735b  gments[i].words[
-0000cfb0: 776f 7264 5f69 6478 5d2e 6c6f 636b 5f72  word_idx].lock_r
-0000cfc0: 6967 6874 2829 0d0a 2020 2020 2020 2020  ight()..        
-0000cfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfe0: 6966 2077 6f72 645f 6964 7820 2b20 3120  if word_idx + 1 
-0000cff0: 3c20 6c65 6e28 7365 6c66 2e73 6567 6d65  < len(self.segme
-0000d000: 6e74 735b 695d 2e77 6f72 6473 293a 0d0a  nts[i].words):..
+0000a310: 2073 696c 656e 745f 7374 6172 7473 2c0d   silent_starts,.
+0000a320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a330: 2020 2020 2073 696c 656e 745f 656e 6473       silent_ends
+0000a340: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a350: 2020 2020 2020 206d 696e 5f77 6f72 645f         min_word_
+0000a360: 6475 722c 0d0a 2020 2020 2020 2020 2020  dur,..          
+0000a370: 2020 2020 2020 2020 2020 776f 7264 5f6c            word_l
+0000a380: 6576 656c 3d77 6f72 645f 6c65 7665 6c2c  evel=word_level,
+0000a390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a3a0: 2020 2020 2020 6e6f 6e73 7065 6563 685f        nonspeech_
+0000a3b0: 6572 726f 723d 6e6f 6e73 7065 6563 685f  error=nonspeech_
+0000a3c0: 6572 726f 722c 0d0a 2020 2020 2020 2020  error,..        
+0000a3d0: 2020 2020 2020 2020 2020 2020 7573 655f              use_
+0000a3e0: 776f 7264 5f70 6f73 6974 696f 6e3d 7573  word_position=us
+0000a3f0: 655f 776f 7264 5f70 6f73 6974 696f 6e0d  e_word_position.
+0000a400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a410: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0000a420: 2020 2020 6966 2076 6572 626f 7365 3a0d      if verbose:.
+0000a430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a440: 2020 2020 2074 7164 6d5f 7062 6172 2e75       tqdm_pbar.u
+0000a450: 7064 6174 6528 732e 656e 6420 2d20 7471  pdate(s.end - tq
+0000a460: 646d 5f70 6261 722e 6e29 0d0a 2020 2020  dm_pbar.n)..    
+0000a470: 2020 2020 2020 2020 7471 646d 5f70 6261          tqdm_pba
+0000a480: 722e 7570 6461 7465 2874 7164 6d5f 7062  r.update(tqdm_pb
+0000a490: 6172 2e74 6f74 616c 202d 2074 7164 6d5f  ar.total - tqdm_
+0000a4a0: 7062 6172 2e6e 290d 0a0d 0a20 2020 2020  pbar.n)....     
+0000a4b0: 2020 2072 6574 7572 6e20 7365 6c66 0d0a     return self..
+0000a4c0: 0d0a 2020 2020 6465 6620 6164 6a75 7374  ..    def adjust
+0000a4d0: 5f62 795f 7369 6c65 6e63 6528 0d0a 2020  _by_silence(..  
+0000a4e0: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
+0000a4f0: 0a20 2020 2020 2020 2020 2020 2061 7564  .            aud
+0000a500: 696f 3a20 556e 696f 6e5b 746f 7263 682e  io: Union[torch.
+0000a510: 5465 6e73 6f72 2c20 6e70 2e6e 6461 7272  Tensor, np.ndarr
+0000a520: 6179 2c20 7374 722c 2062 7974 6573 5d2c  ay, str, bytes],
+0000a530: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+0000a540: 643a 2062 6f6f 6c20 3d20 4661 6c73 652c  d: bool = False,
+0000a550: 0d0a 2020 2020 2020 2020 2020 2020 2a2c  ..            *,
+0000a560: 0d0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
+0000a570: 7262 6f73 653a 2028 626f 6f6c 2c20 4e6f  rbose: (bool, No
+0000a580: 6e65 2920 3d20 4661 6c73 652c 0d0a 2020  ne) = False,..  
+0000a590: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
+0000a5a0: 5f72 6174 653a 2069 6e74 203d 204e 6f6e  _rate: int = Non
+0000a5b0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+0000a5c0: 7661 645f 6f6e 6e78 3a20 626f 6f6c 203d  vad_onnx: bool =
+0000a5d0: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
+0000a5e0: 2020 2020 2076 6164 5f74 6872 6573 686f       vad_thresho
+0000a5f0: 6c64 3a20 666c 6f61 7420 3d20 302e 3335  ld: float = 0.35
+0000a600: 2c0d 0a20 2020 2020 2020 2020 2020 2071  ,..            q
+0000a610: 5f6c 6576 656c 733a 2069 6e74 203d 2032  _levels: int = 2
+0000a620: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+0000a630: 6b5f 7369 7a65 3a20 696e 7420 3d20 352c  k_size: int = 5,
+0000a640: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
+0000a650: 6e5f 776f 7264 5f64 7572 3a20 4f70 7469  n_word_dur: Opti
+0000a660: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
+0000a670: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
+0000a680: 206d 696e 5f73 696c 656e 6365 5f64 7572   min_silence_dur
+0000a690: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
+0000a6a0: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
+0000a6b0: 2020 2020 2020 2077 6f72 645f 6c65 7665         word_leve
+0000a6c0: 6c3a 2062 6f6f 6c20 3d20 5472 7565 2c0d  l: bool = True,.
+0000a6d0: 0a20 2020 2020 2020 2020 2020 206e 6f6e  .            non
+0000a6e0: 7370 6565 6368 5f65 7272 6f72 3a20 666c  speech_error: fl
+0000a6f0: 6f61 7420 3d20 302e 332c 0d0a 2020 2020  oat = 0.3,..    
+0000a700: 2020 2020 2020 2020 7573 655f 776f 7264          use_word
+0000a710: 5f70 6f73 6974 696f 6e3a 2062 6f6f 6c20  _position: bool 
+0000a720: 3d20 5472 7565 0d0a 0d0a 2020 2020 2920  = True....    ) 
+0000a730: 2d3e 2022 5768 6973 7065 7252 6573 756c  -> "WhisperResul
+0000a740: 7422 3a0d 0a20 2020 2020 2020 2022 2222  t":..        """
+0000a750: 0d0a 2020 2020 2020 2020 4164 6a75 7374  ..        Adjust
+0000a760: 2074 696d 6573 7461 6d70 7320 6261 7365   timestamps base
+0000a770: 206f 6e20 6465 7465 6374 6564 2073 7065   on detected spe
+0000a780: 6563 6820 6761 7073 2e0d 0a0d 0a20 2020  ech gaps.....   
+0000a790: 2020 2020 2054 6869 7320 6973 206d 6574       This is met
+0000a7a0: 686f 6420 636f 6d62 696e 6573 203a 6d65  hod combines :me
+0000a7b0: 7468 3a60 7374 6162 6c65 5f77 6869 7370  th:`stable_whisp
+0000a7c0: 6572 2e72 6573 756c 742e 5768 6973 7065  er.result.Whispe
+0000a7d0: 7252 6573 756c 742e 7375 7070 7265 7373  rResult.suppress
+0000a7e0: 5f73 696c 656e 6365 6020 7769 7468 2073  _silence` with s
+0000a7f0: 696c 656e 6365 2064 6574 6563 7469 6f6e  ilence detection
+0000a800: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
+0000a810: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
+0000a820: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
+0000a830: 2020 2020 2061 7564 696f 203a 2073 7472       audio : str
+0000a840: 206f 7220 6e75 6d70 792e 6e64 6172 7261   or numpy.ndarra
+0000a850: 7920 6f72 2074 6f72 6368 2e54 656e 736f  y or torch.Tenso
+0000a860: 7220 6f72 2062 7974 6573 0d0a 2020 2020  r or bytes..    
+0000a870: 2020 2020 2020 2020 5061 7468 2f55 524c          Path/URL
+0000a880: 2074 6f20 7468 6520 6175 6469 6f20 6669   to the audio fi
+0000a890: 6c65 2c20 7468 6520 6175 6469 6f20 7761  le, the audio wa
+0000a8a0: 7665 666f 726d 2c20 6f72 2062 7974 6573  veform, or bytes
+0000a8b0: 206f 6620 6175 6469 6f20 6669 6c65 2e0d   of audio file..
+0000a8c0: 0a20 2020 2020 2020 2076 6164 203a 2062  .        vad : b
+0000a8d0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
+0000a8e0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
+0000a8f0: 5768 6574 6865 7220 746f 2075 7365 2053  Whether to use S
+0000a900: 696c 6572 6f20 5641 4420 746f 2067 656e  ilero VAD to gen
+0000a910: 6572 6174 6520 7469 6d65 7374 616d 7020  erate timestamp 
+0000a920: 7375 7070 7265 7373 696f 6e20 6d61 736b  suppression mask
+0000a930: 2e0d 0a20 2020 2020 2020 2020 2020 2053  ...            S
+0000a940: 696c 6572 6f20 5641 4420 7265 7175 6972  ilero VAD requir
+0000a950: 6573 2050 7954 6f72 6368 2031 2e31 322e  es PyTorch 1.12.
+0000a960: 302b 2e20 4f66 6669 6369 616c 2072 6570  0+. Official rep
+0000a970: 6f2c 2068 7474 7073 3a2f 2f67 6974 6875  o, https://githu
+0000a980: 622e 636f 6d2f 736e 616b 6572 7334 2f73  b.com/snakers4/s
+0000a990: 696c 6572 6f2d 7661 642e 0d0a 2020 2020  ilero-vad...    
+0000a9a0: 2020 2020 7665 7262 6f73 6520 3a20 626f      verbose : bo
+0000a9b0: 6f6c 206f 7220 4e6f 6e65 2c20 6465 6661  ol or None, defa
+0000a9c0: 756c 7420 4661 6c73 650d 0a20 2020 2020  ult False..     
+0000a9d0: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
+0000a9e0: 6f20 7573 6520 7072 6f67 7265 7373 6261  o use progressba
+0000a9f0: 7220 746f 2073 686f 7720 7072 6f67 7265  r to show progre
+0000aa00: 7373 2e0d 0a20 2020 2020 2020 2020 2020  ss...           
+0000aa10: 2049 6620 6060 7661 6420 3d20 5472 7565   If ``vad = True
+0000aa20: 6060 2061 6e64 2060 6046 616c 7365 6060  `` and ``False``
+0000aa30: 2c20 6d75 7465 206d 6573 7361 6765 7320  , mute messages 
+0000aa40: 6162 6f75 7420 6869 7474 696e 6720 6c6f  about hitting lo
+0000aa50: 6361 6c20 6361 6368 6573 2e0d 0a20 2020  cal caches...   
+0000aa60: 2020 2020 2020 2020 204e 6f74 6520 7468           Note th
+0000aa70: 6174 2074 6865 206d 6573 7361 6765 2061  at the message a
+0000aa80: 626f 7574 2066 6972 7374 2064 6f77 6e6c  bout first downl
+0000aa90: 6f61 6420 6361 6e6e 6f74 2062 6520 6d75  oad cannot be mu
+0000aaa0: 7465 642e 0d0a 2020 2020 2020 2020 7361  ted...        sa
+0000aab0: 6d70 6c65 5f72 6174 6520 3a20 696e 742c  mple_rate : int,
+0000aac0: 2064 6566 6175 6c74 204e 6f6e 652c 206d   default None, m
+0000aad0: 6561 6e69 6e67 2060 6077 6869 7370 6572  eaning ``whisper
+0000aae0: 2e61 7564 696f 2e53 414d 504c 455f 5241  .audio.SAMPLE_RA
+0000aaf0: 5445 6060 2c20 3136 6b48 5a0d 0a20 2020  TE``, 16kHZ..   
+0000ab00: 2020 2020 2020 2020 2054 6865 2073 616d           The sam
+0000ab10: 706c 6520 7261 7465 206f 6620 6060 6175  ple rate of ``au
+0000ab20: 6469 6f60 602e 0d0a 2020 2020 2020 2020  dio``...        
+0000ab30: 7661 645f 6f6e 6e78 203a 2062 6f6f 6c2c  vad_onnx : bool,
+0000ab40: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
+0000ab50: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+0000ab60: 6865 7220 746f 2075 7365 204f 4e4e 5820  her to use ONNX 
+0000ab70: 666f 7220 5369 6c65 726f 2056 4144 2e0d  for Silero VAD..
+0000ab80: 0a20 2020 2020 2020 2076 6164 5f74 6872  .        vad_thr
+0000ab90: 6573 686f 6c64 203a 2066 6c6f 6174 2c20  eshold : float, 
+0000aba0: 6465 6661 756c 7420 302e 3335 0d0a 2020  default 0.35..  
+0000abb0: 2020 2020 2020 2020 2020 5468 7265 7368            Thresh
+0000abc0: 6f6c 6420 666f 7220 6465 7465 6374 696e  old for detectin
+0000abd0: 6720 7370 6565 6368 2077 6974 6820 5369  g speech with Si
+0000abe0: 6c65 726f 2056 4144 2e20 4c6f 7720 7468  lero VAD. Low th
+0000abf0: 7265 7368 6f6c 6420 7265 6475 6365 7320  reshold reduces 
+0000ac00: 6661 6c73 6520 706f 7369 7469 7665 7320  false positives 
+0000ac10: 666f 7220 7369 6c65 6e63 6520 6465 7465  for silence dete
+0000ac20: 6374 696f 6e2e 0d0a 2020 2020 2020 2020  ction...        
+0000ac30: 715f 6c65 7665 6c73 203a 2069 6e74 2c20  q_levels : int, 
+0000ac40: 6465 6661 756c 7420 3230 0d0a 2020 2020  default 20..    
+0000ac50: 2020 2020 2020 2020 5175 616e 7469 7a61          Quantiza
+0000ac60: 7469 6f6e 206c 6576 656c 7320 666f 7220  tion levels for 
+0000ac70: 6765 6e65 7261 7469 6e67 2074 696d 6573  generating times
+0000ac80: 7461 6d70 2073 7570 7072 6573 7369 6f6e  tamp suppression
+0000ac90: 206d 6173 6b3b 2069 676e 6f72 6564 2069   mask; ignored i
+0000aca0: 6620 6060 7661 6420 3d20 7472 7565 6060  f ``vad = true``
+0000acb0: 2e0d 0a20 2020 2020 2020 2020 2020 2041  ...            A
+0000acc0: 6374 7320 6173 2061 2074 6872 6573 686f  cts as a thresho
+0000acd0: 6c64 2074 6f20 6d61 726b 696e 6720 736f  ld to marking so
+0000ace0: 756e 6420 6173 2073 696c 656e 742e 0d0a  und as silent...
+0000acf0: 2020 2020 2020 2020 2020 2020 4665 7765              Fewe
+0000ad00: 7220 6c65 7665 6c73 2077 696c 6c20 696e  r levels will in
+0000ad10: 6372 6561 7365 2074 6865 2074 6872 6573  crease the thres
+0000ad20: 686f 6c64 206f 6620 766f 6c75 6d65 2061  hold of volume a
+0000ad30: 7420 7768 6963 6820 746f 206d 6172 6b20  t which to mark 
+0000ad40: 6120 736f 756e 6420 6173 2073 696c 656e  a sound as silen
+0000ad50: 742e 0d0a 2020 2020 2020 2020 6b5f 7369  t...        k_si
+0000ad60: 7a65 203a 2069 6e74 2c20 6465 6661 756c  ze : int, defaul
+0000ad70: 7420 350d 0a20 2020 2020 2020 2020 2020  t 5..           
+0000ad80: 204b 6572 6e65 6c20 7369 7a65 2066 6f72   Kernel size for
+0000ad90: 2061 7667 2d70 6f6f 6c69 6e67 2077 6176   avg-pooling wav
+0000ada0: 6566 6f72 6d20 746f 2067 656e 6572 6174  eform to generat
+0000adb0: 6520 7469 6d65 7374 616d 7020 7375 7070  e timestamp supp
+0000adc0: 7265 7373 696f 6e20 6d61 736b 3b20 6967  ression mask; ig
+0000add0: 6e6f 7265 6420 6966 2060 6076 6164 203d  nored if ``vad =
+0000ade0: 2074 7275 6560 602e 0d0a 2020 2020 2020   true``...      
+0000adf0: 2020 2020 2020 5265 636f 6d6d 656e 6420        Recommend 
+0000ae00: 3520 6f72 2033 3b20 6869 6768 6572 2073  5 or 3; higher s
+0000ae10: 697a 6573 2077 696c 6c20 7265 6475 6365  izes will reduce
+0000ae20: 2064 6574 6563 7469 6f6e 206f 6620 7369   detection of si
+0000ae30: 6c65 6e63 652e 0d0a 2020 2020 2020 2020  lence...        
+0000ae40: 6d69 6e5f 776f 7264 5f64 7572 203a 2066  min_word_dur : f
+0000ae50: 6c6f 6174 206f 7220 4e6f 6e65 2c20 6465  loat or None, de
+0000ae60: 6661 756c 7420 4e6f 6e65 206d 6561 6e69  fault None meani
+0000ae70: 6e67 2075 7365 2060 6073 7461 626c 655f  ng use ``stable_
+0000ae80: 7768 6973 7065 722e 6465 6661 756c 742e  whisper.default.
+0000ae90: 4445 4641 554c 545f 5641 4c55 4553 6060  DEFAULT_VALUES``
+0000aea0: 0d0a 2020 2020 2020 2020 2020 2020 5368  ..            Sh
+0000aeb0: 6f72 7465 7374 2064 7572 6174 696f 6e20  ortest duration 
+0000aec0: 6561 6368 2077 6f72 6420 6973 2061 6c6c  each word is all
+0000aed0: 6f77 6564 2074 6f20 7265 6163 6820 6672  owed to reach fr
+0000aee0: 6f6d 2061 646a 7573 746d 656e 7473 2e0d  om adjustments..
+0000aef0: 0a20 2020 2020 2020 206d 696e 5f73 696c  .        min_sil
+0000af00: 656e 6365 5f64 7572 203a 2066 6c6f 6174  ence_dur : float
+0000af10: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+0000af20: 2020 2020 2020 2020 5368 6f72 7465 7374          Shortest
+0000af30: 2064 7572 6174 696f 6e20 6f66 2073 696c   duration of sil
+0000af40: 656e 6365 2061 6c6c 6f77 6564 2066 6f72  ence allowed for
+0000af50: 2073 696c 656e 6365 2073 7570 7072 6573   silence suppres
+0000af60: 7369 6f6e 2e0d 0a20 2020 2020 2020 2077  sion...        w
+0000af70: 6f72 645f 6c65 7665 6c20 3a20 626f 6f6c  ord_level : bool
+0000af80: 2c20 6465 6661 756c 7420 5472 7565 0d0a  , default True..
+0000af90: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+0000afa0: 6865 7220 746f 2073 6574 7469 6e67 7320  her to settings 
+0000afb0: 746f 2077 6f72 6420 6c65 7665 6c20 7469  to word level ti
+0000afc0: 6d65 7374 616d 7073 2e0d 0a20 2020 2020  mestamps...     
+0000afd0: 2020 206e 6f6e 7370 6565 6368 5f65 7272     nonspeech_err
+0000afe0: 6f72 203a 2066 6c6f 6174 2c20 6465 6661  or : float, defa
+0000aff0: 756c 7420 302e 330d 0a20 2020 2020 2020  ult 0.3..       
+0000b000: 2020 2020 2052 656c 6174 6976 6520 6572       Relative er
+0000b010: 726f 7220 6f66 206e 6f6e 2d73 7065 6563  ror of non-speec
+0000b020: 6820 7365 6374 696f 6e73 2074 6861 7420  h sections that 
+0000b030: 6170 7065 6172 2069 6e20 6265 7477 6565  appear in betwee
+0000b040: 6e20 6120 776f 7264 2066 6f72 2061 646a  n a word for adj
+0000b050: 7573 746d 656e 7473 2e0d 0a20 2020 2020  ustments...     
+0000b060: 2020 2075 7365 5f77 6f72 645f 706f 7369     use_word_posi
+0000b070: 7469 6f6e 203a 2062 6f6f 6c2c 2064 6566  tion : bool, def
+0000b080: 6175 6c74 2054 7275 650d 0a20 2020 2020  ault True..     
+0000b090: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
+0000b0a0: 6f20 7573 6520 706f 7369 7469 6f6e 206f  o use position o
+0000b0b0: 6620 7468 6520 776f 7264 2069 6e20 6974  f the word in it
+0000b0c0: 7320 7365 676d 656e 7420 746f 2064 6574  s segment to det
+0000b0d0: 6572 6d69 6e65 2077 6865 7468 6572 2074  ermine whether t
+0000b0e0: 6f20 6b65 6570 2065 6e64 206f 7220 7374  o keep end or st
+0000b0f0: 6172 7420 7469 6d65 7374 616d 7073 2069  art timestamps i
+0000b100: 660d 0a20 2020 2020 2020 2020 2020 2061  f..            a
+0000b110: 646a 7573 746d 656e 7473 2061 7265 2072  djustments are r
+0000b120: 6571 7569 7265 642e 2049 6620 6974 2069  equired. If it i
+0000b130: 7320 7468 6520 6669 7273 7420 776f 7264  s the first word
+0000b140: 2c20 6b65 6570 2065 6e64 2e20 456c 7365  , keep end. Else
+0000b150: 2069 6620 6974 2069 7320 7468 6520 6c61   if it is the la
+0000b160: 7374 2077 6f72 642c 206b 6565 7020 7468  st word, keep th
+0000b170: 6520 7374 6172 742e 0d0a 0d0a 2020 2020  e start.....    
+0000b180: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
+0000b190: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
+0000b1a0: 2020 2020 2020 7374 6162 6c65 5f77 6869        stable_whi
+0000b1b0: 7370 6572 2e72 6573 756c 742e 5768 6973  sper.result.Whis
+0000b1c0: 7065 7252 6573 756c 740d 0a20 2020 2020  perResult..     
+0000b1d0: 2020 2020 2020 2054 6865 2063 7572 7265         The curre
+0000b1e0: 6e74 2069 6e73 7461 6e63 6520 6166 7465  nt instance afte
+0000b1f0: 7220 7468 6520 6368 616e 6765 732e 0d0a  r the changes...
+0000b200: 0d0a 2020 2020 2020 2020 4e6f 7465 730d  ..        Notes.
+0000b210: 0a20 2020 2020 2020 202d 2d2d 2d2d 0d0a  .        -----..
+0000b220: 2020 2020 2020 2020 5468 6973 206f 7065          This ope
+0000b230: 7261 7469 6f6e 2069 7320 616c 7265 6164  ration is alread
+0000b240: 7920 7065 7266 6f72 6d65 6420 6279 203a  y performed by :
+0000b250: 6675 6e63 3a60 7374 6162 6c65 5f77 6869  func:`stable_whi
+0000b260: 7370 6572 2e77 6869 7370 6572 5f77 6f72  sper.whisper_wor
+0000b270: 645f 6c65 7665 6c2e 7472 616e 7363 7269  d_level.transcri
+0000b280: 6265 5f73 7461 626c 6560 202f 0d0a 2020  be_stable` /..  
+0000b290: 2020 2020 2020 3a66 756e 633a 6073 7461        :func:`sta
+0000b2a0: 626c 655f 7768 6973 7065 722e 7768 6973  ble_whisper.whis
+0000b2b0: 7065 725f 776f 7264 5f6c 6576 656c 2e74  per_word_level.t
+0000b2c0: 7261 6e73 6372 6962 655f 6d69 6e69 6d61  ranscribe_minima
+0000b2d0: 6c60 2f0d 0a20 2020 2020 2020 203a 6675  l`/..        :fu
+0000b2e0: 6e63 3a60 7374 6162 6c65 5f77 6869 7370  nc:`stable_whisp
+0000b2f0: 6572 2e6e 6f6e 5f77 6869 7370 6572 2e74  er.non_whisper.t
+0000b300: 7261 6e73 6372 6962 655f 616e 7960 202f  ranscribe_any` /
+0000b310: 203a 6675 6e63 3a60 7374 6162 6c65 5f77   :func:`stable_w
+0000b320: 6869 7370 6572 2e61 6c69 676e 6d65 6e74  hisper.alignment
+0000b330: 2e61 6c69 676e 600d 0a20 2020 2020 2020  .align`..       
+0000b340: 2069 6620 6060 7375 7070 7265 7373 5f73   if ``suppress_s
+0000b350: 696c 656e 6365 203d 2054 7275 6560 602e  ilence = True``.
+0000b360: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0000b370: 2020 2020 2020 206d 696e 5f77 6f72 645f         min_word_
+0000b380: 6475 7220 3d20 6765 745f 6d69 6e5f 776f  dur = get_min_wo
+0000b390: 7264 5f64 7572 286d 696e 5f77 6f72 645f  rd_dur(min_word_
+0000b3a0: 6475 7229 0d0a 2020 2020 2020 2020 6966  dur)..        if
+0000b3b0: 2076 6164 3a0d 0a20 2020 2020 2020 2020   vad:..         
+0000b3c0: 2020 2061 7564 696f 203d 2061 7564 696f     audio = audio
+0000b3d0: 5f74 6f5f 7465 6e73 6f72 5f72 6573 616d  _to_tensor_resam
+0000b3e0: 706c 6528 6175 6469 6f2c 2073 616d 706c  ple(audio, sampl
+0000b3f0: 655f 7261 7465 2c20 5641 445f 5341 4d50  e_rate, VAD_SAMP
+0000b400: 4c45 5f52 4154 4553 5b30 5d29 0d0a 2020  LE_RATES[0])..  
+0000b410: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
+0000b420: 5f72 6174 6520 3d20 5641 445f 5341 4d50  _rate = VAD_SAMP
+0000b430: 4c45 5f52 4154 4553 5b30 5d0d 0a20 2020  LE_RATES[0]..   
+0000b440: 2020 2020 2020 2020 2073 696c 656e 745f           silent_
+0000b450: 7469 6d69 6e67 7320 3d20 6765 745f 7661  timings = get_va
+0000b460: 645f 7369 6c65 6e63 655f 6675 6e63 280d  d_silence_func(.
+0000b470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b480: 206f 6e6e 783d 7661 645f 6f6e 6e78 2c0d   onnx=vad_onnx,.
+0000b490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b4a0: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
+0000b4b0: 0d0a 2020 2020 2020 2020 2020 2020 2928  ..            )(
+0000b4c0: 6175 6469 6f2c 2073 7065 6563 685f 7468  audio, speech_th
+0000b4d0: 7265 7368 6f6c 643d 7661 645f 7468 7265  reshold=vad_thre
+0000b4e0: 7368 6f6c 642c 2073 723d 7361 6d70 6c65  shold, sr=sample
+0000b4f0: 5f72 6174 6529 0d0a 2020 2020 2020 2020  _rate)..        
+0000b500: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0000b510: 2020 2073 696c 656e 745f 7469 6d69 6e67     silent_timing
+0000b520: 7320 3d20 6175 6469 6f32 7469 6d69 6e67  s = audio2timing
+0000b530: 7328 6175 6469 6f2c 2071 5f6c 6576 656c  s(audio, q_level
+0000b540: 733d 715f 6c65 7665 6c73 2c20 6b5f 7369  s=q_levels, k_si
+0000b550: 7a65 3d6b 5f73 697a 652c 2073 723d 7361  ze=k_size, sr=sa
+0000b560: 6d70 6c65 5f72 6174 6529 0d0a 2020 2020  mple_rate)..    
+0000b570: 2020 2020 6966 2073 696c 656e 745f 7469      if silent_ti
+0000b580: 6d69 6e67 7320 6973 204e 6f6e 653a 0d0a  mings is None:..
+0000b590: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000b5a0: 726e 2073 656c 660d 0a20 2020 2020 2020  rn self..       
+0000b5b0: 2069 6620 6d69 6e5f 7369 6c65 6e63 655f   if min_silence_
+0000b5c0: 6475 723a 0d0a 2020 2020 2020 2020 2020  dur:..          
+0000b5d0: 2020 7369 6c65 6e74 5f74 696d 696e 6773    silent_timings
+0000b5e0: 203d 2066 696c 7465 725f 7469 6d69 6e67   = filter_timing
+0000b5f0: 7328 7369 6c65 6e74 5f74 696d 696e 6773  s(silent_timings
+0000b600: 2c20 6d69 6e5f 7369 6c65 6e63 655f 6475  , min_silence_du
+0000b610: 7229 0d0a 2020 2020 2020 2020 7365 6c66  r)..        self
+0000b620: 2e73 7570 7072 6573 735f 7369 6c65 6e63  .suppress_silenc
+0000b630: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
+0000b640: 2a73 696c 656e 745f 7469 6d69 6e67 732c  *silent_timings,
+0000b650: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
+0000b660: 6e5f 776f 7264 5f64 7572 3d6d 696e 5f77  n_word_dur=min_w
+0000b670: 6f72 645f 6475 722c 0d0a 2020 2020 2020  ord_dur,..      
+0000b680: 2020 2020 2020 776f 7264 5f6c 6576 656c        word_level
+0000b690: 3d77 6f72 645f 6c65 7665 6c2c 0d0a 2020  =word_level,..  
+0000b6a0: 2020 2020 2020 2020 2020 6e6f 6e73 7065            nonspe
+0000b6b0: 6563 685f 6572 726f 723d 6e6f 6e73 7065  ech_error=nonspe
+0000b6c0: 6563 685f 6572 726f 722c 0d0a 2020 2020  ech_error,..    
+0000b6d0: 2020 2020 2020 2020 7573 655f 776f 7264          use_word
+0000b6e0: 5f70 6f73 6974 696f 6e3d 7573 655f 776f  _position=use_wo
+0000b6f0: 7264 5f70 6f73 6974 696f 6e2c 0d0a 2020  rd_position,..  
+0000b700: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
+0000b710: 653d 7665 7262 6f73 650d 0a20 2020 2020  e=verbose..     
+0000b720: 2020 2029 0d0a 2020 2020 2020 2020 7365     )..        se
+0000b730: 6c66 2e75 7064 6174 655f 6e6f 6e73 7065  lf.update_nonspe
+0000b740: 6563 685f 7365 6374 696f 6e73 282a 7369  ech_sections(*si
+0000b750: 6c65 6e74 5f74 696d 696e 6773 290d 0a20  lent_timings).. 
+0000b760: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000b770: 6c66 0d0a 0d0a 2020 2020 6465 6620 6164  lf....    def ad
+0000b780: 6a75 7374 5f62 795f 7265 7375 6c74 280d  just_by_result(.
+0000b790: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000b7a0: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
+0000b7b0: 6f74 6865 725f 7265 7375 6c74 3a20 2257  other_result: "W
+0000b7c0: 6869 7370 6572 5265 7375 6c74 222c 0d0a  hisperResult",..
+0000b7d0: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
+0000b7e0: 776f 7264 5f64 7572 3a20 4f70 7469 6f6e  word_dur: Option
+0000b7f0: 616c 5b66 6c6f 6174 5d20 3d20 4e6f 6e65  al[float] = None
+0000b800: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
+0000b810: 6572 626f 7365 3a20 626f 6f6c 203d 2046  erbose: bool = F
+0000b820: 616c 7365 0d0a 2020 2020 293a 0d0a 2020  alse..    ):..  
+0000b830: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0000b840: 2020 204d 696e 696d 697a 6520 7468 6520     Minimize the 
+0000b850: 6475 7261 7469 6f6e 206f 6620 776f 7264  duration of word
+0000b860: 7320 7573 696e 6720 7469 6d65 7374 616d  s using timestam
+0000b870: 7073 206f 6620 616e 6f74 6865 7220 7265  ps of another re
+0000b880: 7375 6c74 2e0d 0a0d 0a20 2020 2020 2020  sult.....       
+0000b890: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+0000b8a0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
+0000b8b0: 0a20 2020 2020 2020 206f 7468 6572 5f72  .        other_r
+0000b8c0: 6573 756c 7420 3a20 2257 6869 7370 6572  esult : "Whisper
+0000b8d0: 5265 7375 6c74 220d 0a20 2020 2020 2020  Result"..       
+0000b8e0: 2020 2020 2054 696d 696e 6720 6461 7461       Timing data
+0000b8f0: 206f 6620 7468 6520 7361 6d65 2077 6f72   of the same wor
+0000b900: 6473 2069 6e20 6120 5768 6973 7065 7252  ds in a WhisperR
+0000b910: 6573 756c 7420 696e 7374 616e 6365 2e0d  esult instance..
+0000b920: 0a20 2020 2020 2020 206d 696e 5f77 6f72  .        min_wor
+0000b930: 645f 6475 7220 3a20 666c 6f61 7420 6f72  d_dur : float or
+0000b940: 204e 6f6e 652c 2064 6566 6175 6c74 204e   None, default N
+0000b950: 6f6e 6520 6d65 616e 696e 6720 7573 6520  one meaning use 
+0000b960: 6060 7374 6162 6c65 5f77 6869 7370 6572  ``stable_whisper
+0000b970: 2e64 6566 6175 6c74 2e44 4546 4155 4c54  .default.DEFAULT
+0000b980: 5f56 414c 5545 5360 600d 0a20 2020 2020  _VALUES``..     
+0000b990: 2020 2020 2020 2050 7265 7665 6e74 2063         Prevent c
+0000b9a0: 6861 6e67 6573 2074 6f20 7469 6d65 7374  hanges to timest
+0000b9b0: 616d 7073 2069 6620 7468 6520 7265 7375  amps if the resu
+0000b9c0: 6c74 616e 7420 776f 7264 2064 7572 6174  ltant word durat
+0000b9d0: 696f 6e20 6973 206c 6573 7320 7468 616e  ion is less than
+0000b9e0: 2060 606d 696e 5f77 6f72 645f 6475 7260   ``min_word_dur`
+0000b9f0: 602e 0d0a 2020 2020 2020 2020 7665 7262  `...        verb
+0000ba00: 6f73 6520 3a20 626f 6f6c 2c20 6465 6661  ose : bool, defa
+0000ba10: 756c 7420 4661 6c73 650d 0a20 2020 2020  ult False..     
+0000ba20: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
+0000ba30: 6f20 7072 696e 7420 6f75 7420 7468 6520  o print out the 
+0000ba40: 7469 6d65 7374 616d 7020 6368 616e 6765  timestamp change
+0000ba50: 732e 0d0a 2020 2020 2020 2020 2222 220d  s...        """.
+0000ba60: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000ba70: 2873 656c 662e 6861 735f 776f 7264 7320  (self.has_words 
+0000ba80: 616e 6420 6f74 6865 725f 7265 7375 6c74  and other_result
+0000ba90: 2e68 6173 5f77 6f72 6473 293a 0d0a 2020  .has_words):..  
+0000baa0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000bab0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+0000bac0: 726f 7228 2754 6869 7320 6f70 6572 6174  ror('This operat
+0000bad0: 696f 6e20 6361 6e20 6f6e 6c79 2062 6520  ion can only be 
+0000bae0: 7065 7266 6f72 6d65 6420 6f6e 2072 6573  performed on res
+0000baf0: 756c 7473 2077 6974 6820 776f 7264 2074  ults with word t
+0000bb00: 696d 6573 7461 6d70 7327 290d 0a20 2020  imestamps')..   
+0000bb10: 2020 2020 2061 7373 6572 7420 5b77 2e77       assert [w.w
+0000bb20: 6f72 6420 666f 7220 7720 696e 2073 656c  ord for w in sel
+0000bb30: 662e 616c 6c5f 776f 7264 7328 295d 203d  f.all_words()] =
+0000bb40: 3d20 5b77 2e77 6f72 6420 666f 7220 7720  = [w.word for w 
+0000bb50: 696e 206f 7468 6572 5f72 6573 756c 742e  in other_result.
+0000bb60: 616c 6c5f 776f 7264 7328 295d 2c20 5c0d  all_words()], \.
+0000bb70: 0a20 2020 2020 2020 2020 2020 2027 5468  .            'Th
+0000bb80: 6520 776f 7264 7320 696e 205b 6f74 6865  e words in [othe
+0000bb90: 725f 7265 7375 6c74 5d20 646f 206e 6f74  r_result] do not
+0000bba0: 206d 6174 6368 2074 6865 2063 7572 7265   match the curre
+0000bbb0: 6e74 2077 6f72 6473 2e27 0d0a 2020 2020  nt words.'..    
+0000bbc0: 2020 2020 6d69 6e5f 776f 7264 5f64 7572      min_word_dur
+0000bbd0: 203d 2067 6574 5f6d 696e 5f77 6f72 645f   = get_min_word_
+0000bbe0: 6475 7228 6d69 6e5f 776f 7264 5f64 7572  dur(min_word_dur
+0000bbf0: 290d 0a20 2020 2020 2020 2066 6f72 2077  )..        for w
+0000bc00: 6f72 642c 206f 7468 6572 5f77 6f72 6420  ord, other_word 
+0000bc10: 696e 207a 6970 2873 656c 662e 616c 6c5f  in zip(self.all_
+0000bc20: 776f 7264 7328 292c 206f 7468 6572 5f72  words(), other_r
+0000bc30: 6573 756c 742e 616c 6c5f 776f 7264 7328  esult.all_words(
+0000bc40: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+0000bc50: 2069 6620 776f 7264 2e65 6e64 203e 206f   if word.end > o
+0000bc60: 7468 6572 5f77 6f72 642e 7374 6172 743a  ther_word.start:
+0000bc70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bc80: 2020 6e65 775f 7374 6172 7420 3d20 6d61    new_start = ma
+0000bc90: 7828 776f 7264 2e73 7461 7274 2c20 6f74  x(word.start, ot
+0000bca0: 6865 725f 776f 7264 2e73 7461 7274 290d  her_word.start).
+0000bcb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bcc0: 206e 6577 5f65 6e64 203d 206d 696e 2877   new_end = min(w
+0000bcd0: 6f72 642e 656e 642c 206f 7468 6572 5f77  ord.end, other_w
+0000bce0: 6f72 642e 656e 6429 0d0a 2020 2020 2020  ord.end)..      
+0000bcf0: 2020 2020 2020 2020 2020 6966 206e 6577            if new
+0000bd00: 5f65 6e64 202d 206e 6577 5f73 7461 7274  _end - new_start
+0000bd10: 203e 3d20 6d69 6e5f 776f 7264 5f64 7572   >= min_word_dur
+0000bd20: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000bd30: 2020 2020 2020 206c 696e 6520 3d20 2727         line = ''
+0000bd40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bd50: 2020 2020 2020 6966 2077 6f72 642e 7374        if word.st
+0000bd60: 6172 7420 213d 206e 6577 5f73 7461 7274  art != new_start
+0000bd70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000bd80: 2020 2020 2020 2020 2020 2069 6620 7665             if ve
+0000bd90: 7262 6f73 653a 0d0a 2020 2020 2020 2020  rbose:..        
+0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdb0: 2020 2020 6c69 6e65 202b 3d20 6627 5b53      line += f'[S
+0000bdc0: 7461 7274 3a7b 776f 7264 2e73 7461 7274  tart:{word.start
+0000bdd0: 3a2e 3366 7d2d 3e7b 6e65 775f 7374 6172  :.3f}->{new_star
+0000bde0: 743a 2e33 667d 5d20 270d 0a20 2020 2020  t:.3f}] '..     
+0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be00: 2020 2077 6f72 642e 7374 6172 7420 3d20     word.start = 
+0000be10: 6e65 775f 7374 6172 740d 0a20 2020 2020  new_start..     
+0000be20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000be30: 6620 776f 7264 2e65 6e64 2021 3d20 6e65  f word.end != ne
+0000be40: 775f 656e 643a 0d0a 2020 2020 2020 2020  w_end:..        
+0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be60: 6966 2076 6572 626f 7365 3a0d 0a20 2020  if verbose:..   
+0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be80: 2020 2020 2020 2020 206c 696e 6520 2b3d           line +=
+0000be90: 2066 275b 456e 643a 7b77 6f72 642e 656e   f'[End:{word.en
+0000bea0: 643a 2e33 667d 2d3e 7b6e 6577 5f65 6e64  d:.3f}->{new_end
+0000beb0: 3a2e 3366 7d5d 2020 270d 0a20 2020 2020  :.3f}]  '..     
+0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bed0: 2020 2077 6f72 642e 656e 6420 3d20 6e65     word.end = ne
+0000bee0: 775f 656e 640d 0a20 2020 2020 2020 2020  w_end..         
+0000bef0: 2020 2020 2020 2020 2020 2069 6620 6c69             if li
+0000bf00: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000bf10: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+0000bf20: 6e74 2866 277b 6c69 6e65 7d22 7b77 6f72  nt(f'{line}"{wor
+0000bf30: 642e 776f 7264 7d22 2729 0d0a 0d0a 2020  d.word}"')....  
+0000bf40: 2020 6465 6620 7265 6173 7369 676e 5f69    def reassign_i
+0000bf50: 6473 2873 656c 662c 206f 6e6c 795f 7365  ds(self, only_se
+0000bf60: 676d 656e 7473 3a20 626f 6f6c 203d 2046  gments: bool = F
+0000bf70: 616c 7365 2c20 7374 6172 743a 204f 7074  alse, start: Opt
+0000bf80: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+0000bf90: 6529 3a0d 0a20 2020 2020 2020 2066 6f72  e):..        for
+0000bfa0: 2069 2c20 7320 696e 2065 6e75 6d65 7261   i, s in enumera
+0000bfb0: 7465 2873 656c 662e 7365 676d 656e 7473  te(self.segments
+0000bfc0: 5b73 7461 7274 3a5d 2c20 7374 6172 7420  [start:], start 
+0000bfd0: 6f72 2030 293a 0d0a 2020 2020 2020 2020  or 0):..        
+0000bfe0: 2020 2020 732e 6964 203d 2069 0d0a 2020      s.id = i..  
+0000bff0: 2020 2020 2020 2020 2020 732e 7265 7375            s.resu
+0000c000: 6c74 203d 2073 656c 660d 0a20 2020 2020  lt = self..     
+0000c010: 2020 2020 2020 2069 6620 6e6f 7420 6f6e         if not on
+0000c020: 6c79 5f73 6567 6d65 6e74 733a 0d0a 2020  ly_segments:..  
+0000c030: 2020 2020 2020 2020 2020 2020 2020 732e                s.
+0000c040: 7265 6173 7369 676e 5f69 6473 2829 0d0a  reassign_ids()..
+0000c050: 0d0a 2020 2020 6465 6620 7265 6d6f 7665  ..    def remove
+0000c060: 5f6e 6f5f 776f 7264 5f73 6567 6d65 6e74  _no_word_segment
+0000c070: 7328 7365 6c66 2c20 6967 6e6f 7265 5f6f  s(self, ignore_o
+0000c080: 7269 3d46 616c 7365 2c20 7265 6173 7369  ri=False, reassi
+0000c090: 676e 5f69 6473 3a20 626f 6f6c 203d 2054  gn_ids: bool = T
+0000c0a0: 7275 6529 3a0d 0a20 2020 2020 2020 2066  rue):..        f
+0000c0b0: 6f72 2069 2069 6e20 7265 7665 7273 6564  or i in reversed
+0000c0c0: 2872 616e 6765 286c 656e 2873 656c 662e  (range(len(self.
+0000c0d0: 7365 676d 656e 7473 2929 293a 0d0a 2020  segments))):..  
+0000c0e0: 2020 2020 2020 2020 2020 6966 2028 6967            if (ig
+0000c0f0: 6e6f 7265 5f6f 7269 206f 7220 7365 6c66  nore_ori or self
+0000c100: 2e73 6567 6d65 6e74 735b 695d 2e6f 7269  .segments[i].ori
+0000c110: 5f68 6173 5f77 6f72 6473 2920 616e 6420  _has_words) and 
+0000c120: 6e6f 7420 7365 6c66 2e73 6567 6d65 6e74  not self.segment
+0000c130: 735b 695d 2e68 6173 5f77 6f72 6473 3a0d  s[i].has_words:.
+0000c140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c150: 2064 656c 2073 656c 662e 7365 676d 656e   del self.segmen
+0000c160: 7473 5b69 5d0d 0a20 2020 2020 2020 2069  ts[i]..        i
+0000c170: 6620 7265 6173 7369 676e 5f69 6473 3a0d  f reassign_ids:.
+0000c180: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c190: 662e 7265 6173 7369 676e 5f69 6473 2829  f.reassign_ids()
+0000c1a0: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
+0000c1b0: 6c6f 636b 6564 5f69 6e64 6963 6573 2873  locked_indices(s
+0000c1c0: 656c 6629 3a0d 0a20 2020 2020 2020 206c  elf):..        l
+0000c1d0: 6f63 6b65 645f 696e 6469 6365 7320 3d20  ocked_indices = 
+0000c1e0: 5b69 0d0a 2020 2020 2020 2020 2020 2020  [i..            
+0000c1f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000c200: 7220 692c 2028 6c65 6674 2c20 7269 6768  r i, (left, righ
+0000c210: 7429 2069 6e20 656e 756d 6572 6174 6528  t) in enumerate(
+0000c220: 7a69 7028 7365 6c66 2e73 6567 6d65 6e74  zip(self.segment
+0000c230: 735b 313a 5d2c 2073 656c 662e 7365 676d  s[1:], self.segm
+0000c240: 656e 7473 5b3a 2d31 5d29 290d 0a20 2020  ents[:-1]))..   
+0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c260: 2020 2020 2020 2069 6620 6c65 6674 2e6c         if left.l
+0000c270: 6566 745f 6c6f 636b 6564 206f 7220 7269  eft_locked or ri
+0000c280: 6768 742e 7269 6768 745f 6c6f 636b 6564  ght.right_locked
+0000c290: 5d0d 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
+0000c2a0: 6e20 6c6f 636b 6564 5f69 6e64 6963 6573  n locked_indices
+0000c2b0: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
+0000c2c0: 6761 7073 2873 656c 662c 2061 735f 6e64  gaps(self, as_nd
+0000c2d0: 6172 7261 793d 4661 6c73 6529 3a0d 0a20  array=False):.. 
+0000c2e0: 2020 2020 2020 2073 5f74 7320 3d20 6e70         s_ts = np
+0000c2f0: 2e61 7272 6179 285b 732e 7374 6172 7420  .array([s.start 
+0000c300: 666f 7220 7320 696e 2073 656c 662e 7365  for s in self.se
+0000c310: 676d 656e 7473 5d29 0d0a 2020 2020 2020  gments])..      
+0000c320: 2020 655f 7473 203d 206e 702e 6172 7261    e_ts = np.arra
+0000c330: 7928 5b73 2e65 6e64 2066 6f72 2073 2069  y([s.end for s i
+0000c340: 6e20 7365 6c66 2e73 6567 6d65 6e74 735d  n self.segments]
+0000c350: 290d 0a20 2020 2020 2020 2067 6170 203d  )..        gap =
+0000c360: 2073 5f74 735b 313a 5d20 2d20 655f 7473   s_ts[1:] - e_ts
+0000c370: 5b3a 2d31 5d0d 0a20 2020 2020 2020 2072  [:-1]..        r
+0000c380: 6574 7572 6e20 6761 7020 6966 2061 735f  eturn gap if as_
+0000c390: 6e64 6172 7261 7920 656c 7365 2067 6170  ndarray else gap
+0000c3a0: 2e74 6f6c 6973 7428 290d 0a0d 0a20 2020  .tolist()....   
+0000c3b0: 2064 6566 2067 6574 5f67 6170 5f69 6e64   def get_gap_ind
+0000c3c0: 6963 6573 2873 656c 662c 206d 696e 5f67  ices(self, min_g
+0000c3d0: 6170 3a20 666c 6f61 7420 3d20 302e 3129  ap: float = 0.1)
+0000c3e0: 3a20 2023 2066 6f72 206d 6572 6769 6e67  :  # for merging
+0000c3f0: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+0000c400: 2873 656c 662e 7365 676d 656e 7473 2920  (self.segments) 
+0000c410: 3c20 323a 0d0a 2020 2020 2020 2020 2020  < 2:..          
+0000c420: 2020 7265 7475 726e 205b 5d0d 0a20 2020    return []..   
+0000c430: 2020 2020 2069 6620 6d69 6e5f 6761 7020       if min_gap 
+0000c440: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+0000c450: 2020 2020 2020 6d69 6e5f 6761 7020 3d20        min_gap = 
+0000c460: 300d 0a20 2020 2020 2020 2069 6e64 6963  0..        indic
+0000c470: 6573 203d 2028 7365 6c66 2e67 6574 5f67  es = (self.get_g
+0000c480: 6170 7328 5472 7565 2920 3c3d 206d 696e  aps(True) <= min
+0000c490: 5f67 6170 292e 6e6f 6e7a 6572 6f28 295b  _gap).nonzero()[
+0000c4a0: 305d 2e74 6f6c 6973 7428 290d 0a20 2020  0].tolist()..   
+0000c4b0: 2020 2020 2072 6574 7572 6e20 736f 7274       return sort
+0000c4c0: 6564 2873 6574 2869 6e64 6963 6573 2920  ed(set(indices) 
+0000c4d0: 2d20 7365 7428 7365 6c66 2e67 6574 5f6c  - set(self.get_l
+0000c4e0: 6f63 6b65 645f 696e 6469 6365 7328 2929  ocked_indices())
+0000c4f0: 290d 0a0d 0a20 2020 2064 6566 2067 6574  )....    def get
+0000c500: 5f70 756e 6374 7561 7469 6f6e 5f69 6e64  _punctuation_ind
+0000c510: 6963 6573 2873 656c 662c 2070 756e 6374  ices(self, punct
+0000c520: 7561 7469 6f6e 3a20 556e 696f 6e5b 4c69  uation: Union[Li
+0000c530: 7374 5b73 7472 5d2c 204c 6973 745b 5475  st[str], List[Tu
+0000c540: 706c 655b 7374 722c 2073 7472 5d5d 2c20  ple[str, str]], 
+0000c550: 7374 725d 293a 2020 2320 666f 7220 6d65  str]):  # for me
+0000c560: 7267 696e 670d 0a20 2020 2020 2020 2069  rging..        i
+0000c570: 6620 6c65 6e28 7365 6c66 2e73 6567 6d65  f len(self.segme
+0000c580: 6e74 7329 203c 2032 3a0d 0a20 2020 2020  nts) < 2:..     
+0000c590: 2020 2020 2020 2072 6574 7572 6e20 5b5d         return []
+0000c5a0: 0d0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
+0000c5b0: 6e73 7461 6e63 6528 7075 6e63 7475 6174  nstance(punctuat
+0000c5c0: 696f 6e2c 2073 7472 293a 0d0a 2020 2020  ion, str):..    
+0000c5d0: 2020 2020 2020 2020 7075 6e63 7475 6174          punctuat
+0000c5e0: 696f 6e20 3d20 5b70 756e 6374 7561 7469  ion = [punctuati
+0000c5f0: 6f6e 5d0d 0a20 2020 2020 2020 2069 6e64  on]..        ind
+0000c600: 6963 6573 203d 205b 5d0d 0a20 2020 2020  ices = []..     
+0000c610: 2020 2066 6f72 2070 2069 6e20 7075 6e63     for p in punc
+0000c620: 7475 6174 696f 6e3a 0d0a 2020 2020 2020  tuation:..      
+0000c630: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000c640: 6e63 6528 702c 2073 7472 293a 0d0a 2020  nce(p, str):..  
+0000c650: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000c660: 7220 692c 2073 2069 6e20 656e 756d 6572  r i, s in enumer
+0000c670: 6174 6528 7365 6c66 2e73 6567 6d65 6e74  ate(self.segment
+0000c680: 735b 3a2d 315d 293a 0d0a 2020 2020 2020  s[:-1]):..      
+0000c690: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000c6a0: 2073 2e74 6578 742e 656e 6473 7769 7468   s.text.endswith
+0000c6b0: 2870 293a 0d0a 2020 2020 2020 2020 2020  (p):..          
+0000c6c0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000c6d0: 6469 6365 732e 6170 7065 6e64 2869 290d  dices.append(i).
+0000c6e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c6f0: 2020 2020 2065 6c69 6620 6920 213d 2030       elif i != 0
+0000c700: 2061 6e64 2073 2e74 6578 742e 7374 6172   and s.text.star
+0000c710: 7473 7769 7468 2870 293a 0d0a 2020 2020  tswith(p):..    
+0000c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c730: 2020 2020 696e 6469 6365 732e 6170 7065      indices.appe
+0000c740: 6e64 2869 2d31 290d 0a20 2020 2020 2020  nd(i-1)..       
+0000c750: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000c760: 2020 2020 2020 2020 2020 2020 656e 6469              endi
+0000c770: 6e67 2c20 6265 6769 6e6e 696e 6720 3d20  ng, beginning = 
+0000c780: 700d 0a20 2020 2020 2020 2020 2020 2020  p..             
+0000c790: 2020 2069 6e64 6963 6573 2e65 7874 656e     indices.exten
+0000c7a0: 6428 5b69 2066 6f72 2069 2c20 2873 302c  d([i for i, (s0,
+0000c7b0: 2073 3129 2069 6e20 656e 756d 6572 6174   s1) in enumerat
+0000c7c0: 6528 7a69 7028 7365 6c66 2e73 6567 6d65  e(zip(self.segme
+0000c7d0: 6e74 735b 3a2d 315d 2c20 7365 6c66 2e73  nts[:-1], self.s
+0000c7e0: 6567 6d65 6e74 735b 313a 5d29 290d 0a20  egments[1:])).. 
+0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c800: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000c810: 6620 7330 2e74 6578 742e 656e 6473 7769  f s0.text.endswi
+0000c820: 7468 2865 6e64 696e 6729 2061 6e64 2073  th(ending) and s
+0000c830: 312e 7465 7874 2e73 7461 7274 7377 6974  1.text.startswit
+0000c840: 6828 6265 6769 6e6e 696e 6729 5d29 0d0a  h(beginning)])..
+0000c850: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000c860: 2073 6f72 7465 6428 7365 7428 696e 6469   sorted(set(indi
+0000c870: 6365 7329 202d 2073 6574 2873 656c 662e  ces) - set(self.
+0000c880: 6765 745f 6c6f 636b 6564 5f69 6e64 6963  get_locked_indic
+0000c890: 6573 2829 2929 0d0a 0d0a 2020 2020 6465  es()))....    de
+0000c8a0: 6620 616c 6c5f 776f 7264 7328 7365 6c66  f all_words(self
+0000c8b0: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
+0000c8c0: 726e 206c 6973 7428 6368 6169 6e2e 6672  rn list(chain.fr
+0000c8d0: 6f6d 5f69 7465 7261 626c 6528 732e 776f  om_iterable(s.wo
+0000c8e0: 7264 7320 666f 7220 7320 696e 2073 656c  rds for s in sel
+0000c8f0: 662e 7365 676d 656e 7473 2929 0d0a 0d0a  f.segments))....
+0000c900: 2020 2020 6465 6620 616c 6c5f 776f 7264      def all_word
+0000c910: 735f 6f72 5f73 6567 6d65 6e74 7328 7365  s_or_segments(se
+0000c920: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
+0000c930: 7475 726e 2073 656c 662e 616c 6c5f 776f  turn self.all_wo
+0000c940: 7264 7328 2920 6966 2073 656c 662e 6861  rds() if self.ha
+0000c950: 735f 776f 7264 7320 656c 7365 2073 656c  s_words else sel
+0000c960: 662e 7365 676d 656e 7473 0d0a 0d0a 2020  f.segments....  
+0000c970: 2020 6465 6620 616c 6c5f 776f 7264 735f    def all_words_
+0000c980: 6279 5f6c 6f63 6b28 7365 6c66 2c20 6f6e  by_lock(self, on
+0000c990: 6c79 5f74 6578 743a 2062 6f6f 6c20 3d20  ly_text: bool = 
+0000c9a0: 5472 7565 2c20 6279 5f73 6567 6d65 6e74  True, by_segment
+0000c9b0: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
+0000c9c0: 696e 636c 7564 655f 7369 6e67 6c65 3a20  include_single: 
+0000c9d0: 626f 6f6c 203d 2046 616c 7365 293a 0d0a  bool = False):..
+0000c9e0: 2020 2020 2020 2020 6966 2062 795f 7365          if by_se
+0000c9f0: 676d 656e 743a 0d0a 2020 2020 2020 2020  gment:..        
+0000ca00: 2020 2020 7265 7475 726e 205b 0d0a 2020      return [..  
+0000ca10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ca20: 676d 656e 742e 776f 7264 735f 6279 5f6c  gment.words_by_l
+0000ca30: 6f63 6b28 6f6e 6c79 5f74 6578 743d 6f6e  ock(only_text=on
+0000ca40: 6c79 5f74 6578 742c 2069 6e63 6c75 6465  ly_text, include
+0000ca50: 5f73 696e 676c 653d 696e 636c 7564 655f  _single=include_
+0000ca60: 7369 6e67 6c65 290d 0a20 2020 2020 2020  single)..       
+0000ca70: 2020 2020 2020 2020 2066 6f72 2073 6567           for seg
+0000ca80: 6d65 6e74 2069 6e20 7365 6c66 2e73 6567  ment in self.seg
+0000ca90: 6d65 6e74 730d 0a20 2020 2020 2020 2020  ments..         
+0000caa0: 2020 205d 0d0a 2020 2020 2020 2020 7265     ]..        re
+0000cab0: 7475 726e 205f 776f 7264 735f 6279 5f6c  turn _words_by_l
+0000cac0: 6f63 6b28 7365 6c66 2e61 6c6c 5f77 6f72  ock(self.all_wor
+0000cad0: 6473 2829 2c20 6f6e 6c79 5f74 6578 743d  ds(), only_text=
+0000cae0: 6f6e 6c79 5f74 6578 742c 2069 6e63 6c75  only_text, inclu
+0000caf0: 6465 5f73 696e 676c 653d 696e 636c 7564  de_single=includ
+0000cb00: 655f 7369 6e67 6c65 290d 0a0d 0a20 2020  e_single)....   
+0000cb10: 2064 6566 2061 6c6c 5f74 6f6b 656e 7328   def all_tokens(
+0000cb20: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+0000cb30: 7265 7475 726e 206c 6973 7428 6368 6169  return list(chai
+0000cb40: 6e2e 6672 6f6d 5f69 7465 7261 626c 6528  n.from_iterable(
+0000cb50: 732e 746f 6b65 6e73 2066 6f72 2073 2069  s.tokens for s i
+0000cb60: 6e20 7365 6c66 2e61 6c6c 5f77 6f72 6473  n self.all_words
+0000cb70: 2829 2929 0d0a 0d0a 2020 2020 6465 6620  ()))....    def 
+0000cb80: 746f 5f64 6963 7428 7365 6c66 293a 0d0a  to_dict(self):..
+0000cb90: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+0000cba0: 6963 7428 7465 7874 3d73 656c 662e 7465  ict(text=self.te
+0000cbb0: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
+0000cbc0: 2020 2020 2020 2020 2073 6567 6d65 6e74           segment
+0000cbd0: 733d 7365 6c66 2e73 6567 6d65 6e74 735f  s=self.segments_
+0000cbe0: 746f 5f64 6963 7473 2829 2c0d 0a20 2020  to_dicts(),..   
+0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc00: 206c 616e 6775 6167 653d 7365 6c66 2e6c   language=self.l
+0000cc10: 616e 6775 6167 652c 0d0a 2020 2020 2020  anguage,..      
+0000cc20: 2020 2020 2020 2020 2020 2020 2020 6f72                or
+0000cc30: 695f 6469 6374 3d73 656c 662e 6f72 695f  i_dict=self.ori_
+0000cc40: 6469 6374 2c0d 0a20 2020 2020 2020 2020  dict,..         
+0000cc50: 2020 2020 2020 2020 2020 2072 6567 726f             regro
+0000cc60: 7570 5f68 6973 746f 7279 3d73 656c 662e  up_history=self.
+0000cc70: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
+0000cc80: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000cc90: 2020 2020 2020 206e 6f6e 7370 6565 6368         nonspeech
+0000cca0: 5f73 6563 7469 6f6e 733d 7365 6c66 2e5f  _sections=self._
+0000ccb0: 6e6f 6e73 7065 6563 685f 7365 6374 696f  nonspeech_sectio
+0000ccc0: 6e73 290d 0a0d 0a20 2020 2064 6566 2073  ns)....    def s
+0000ccd0: 6567 6d65 6e74 735f 746f 5f64 6963 7473  egments_to_dicts
+0000cce0: 2873 656c 662c 2072 6576 6572 7365 5f74  (self, reverse_t
+0000ccf0: 6578 743a 2055 6e69 6f6e 5b62 6f6f 6c2c  ext: Union[bool,
+0000cd00: 2074 7570 6c65 5d20 3d20 4661 6c73 6529   tuple] = False)
+0000cd10: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+0000cd20: 6e20 5b73 2e74 6f5f 6469 6374 2872 6576  n [s.to_dict(rev
+0000cd30: 6572 7365 5f74 6578 743d 7265 7665 7273  erse_text=revers
+0000cd40: 655f 7465 7874 2920 666f 7220 7320 696e  e_text) for s in
+0000cd50: 2073 656c 662e 7365 676d 656e 7473 5d0d   self.segments].
+0000cd60: 0a0d 0a20 2020 2064 6566 205f 7370 6c69  ...    def _spli
+0000cd70: 745f 7365 676d 656e 7473 2873 656c 662c  t_segments(self,
+0000cd80: 2067 6574 5f69 6e64 6963 6573 2c20 6172   get_indices, ar
+0000cd90: 6773 3a20 6c69 7374 203d 204e 6f6e 652c  gs: list = None,
+0000cda0: 202a 2c20 6c6f 636b 3a20 626f 6f6c 203d   *, lock: bool =
+0000cdb0: 2046 616c 7365 2c20 6e65 776c 696e 653a   False, newline:
+0000cdc0: 2062 6f6f 6c20 3d20 4661 6c73 6529 3a0d   bool = False):.
+0000cdd0: 0a20 2020 2020 2020 2069 6620 6172 6773  .        if args
+0000cde0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+0000cdf0: 2020 2020 2020 2061 7267 7320 3d20 5b5d         args = []
+0000ce00: 0d0a 2020 2020 2020 2020 6e6f 5f77 6f72  ..        no_wor
+0000ce10: 6473 203d 2046 616c 7365 0d0a 2020 2020  ds = False..    
+0000ce20: 2020 2020 666f 7220 6920 696e 2072 6576      for i in rev
+0000ce30: 6572 7365 6428 7261 6e67 6528 302c 206c  ersed(range(0, l
+0000ce40: 656e 2873 656c 662e 7365 676d 656e 7473  en(self.segments
+0000ce50: 2929 293a 0d0a 2020 2020 2020 2020 2020  ))):..          
+0000ce60: 2020 6e6f 5f77 6f72 6473 203d 206e 6f5f    no_words = no_
+0000ce70: 776f 7264 7320 6f72 206e 6f74 2073 656c  words or not sel
+0000ce80: 662e 7365 676d 656e 7473 5b69 5d2e 6861  f.segments[i].ha
+0000ce90: 735f 776f 7264 730d 0a20 2020 2020 2020  s_words..       
+0000cea0: 2020 2020 2069 6e64 6963 6573 203d 2073       indices = s
+0000ceb0: 6f72 7465 6428 7365 7428 6765 745f 696e  orted(set(get_in
+0000cec0: 6469 6365 7328 7365 6c66 2e73 6567 6d65  dices(self.segme
+0000ced0: 6e74 735b 695d 2c20 2a61 7267 7329 2929  nts[i], *args)))
+0000cee0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000cef0: 206e 6f74 2069 6e64 6963 6573 3a0d 0a20   not indices:.. 
+0000cf00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000cf10: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
+0000cf20: 2020 2020 2069 6620 6e65 776c 696e 653a       if newline:
+0000cf30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cf40: 2020 6966 2069 6e64 6963 6573 5b2d 315d    if indices[-1]
+0000cf50: 203d 3d20 6c65 6e28 7365 6c66 2e73 6567   == len(self.seg
+0000cf60: 6d65 6e74 735b 695d 2e77 6f72 6473 2920  ments[i].words) 
+0000cf70: 2d20 313a 0d0a 2020 2020 2020 2020 2020  - 1:..          
+0000cf80: 2020 2020 2020 2020 2020 6465 6c20 696e            del in
+0000cf90: 6469 6365 735b 2d31 5d0d 0a20 2020 2020  dices[-1]..     
+0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000cfb0: 6620 6e6f 7420 696e 6469 6365 733a 0d0a  f not indices:..
+0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfd0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+0000cfe0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000cff0: 2020 2020 666f 7220 776f 7264 5f69 6478      for word_idx
+0000d000: 2069 6e20 696e 6469 6365 733a 0d0a 2020   in indices:..  
 0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d030: 2e73 6567 6d65 6e74 735b 695d 2e77 6f72  .segments[i].wor
-0000d040: 6473 5b77 6f72 645f 6964 782b 315d 2e6c  ds[word_idx+1].l
-0000d050: 6f63 6b5f 6c65 6674 2829 0d0a 2020 2020  ock_left()..    
-0000d060: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0000d070: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000d080: 6577 5f73 6567 6d65 6e74 7320 3d20 7365  ew_segments = se
-0000d090: 6c66 2e73 6567 6d65 6e74 735b 695d 2e73  lf.segments[i].s
-0000d0a0: 706c 6974 2869 6e64 6963 6573 290d 0a20  plit(indices).. 
-0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d0c0: 6620 6c6f 636b 3a0d 0a20 2020 2020 2020  f lock:..       
-0000d0d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000d0e0: 2073 2069 6e20 6e65 775f 7365 676d 656e   s in new_segmen
-0000d0f0: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
-0000d100: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000d110: 7320 3d3d 206e 6577 5f73 6567 6d65 6e74  s == new_segment
-0000d120: 735b 305d 3a0d 0a20 2020 2020 2020 2020  s[0]:..         
-0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d140: 2020 2073 2e6c 6f63 6b5f 7269 6768 7428     s.lock_right(
-0000d150: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000d160: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000d170: 7320 3d3d 206e 6577 5f73 6567 6d65 6e74  s == new_segment
-0000d180: 735b 2d31 5d3a 0d0a 2020 2020 2020 2020  s[-1]:..        
-0000d190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1a0: 2020 2020 732e 6c6f 636b 5f6c 6566 7428      s.lock_left(
-0000d1b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000d1c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000d1d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d1e0: 2020 2020 2020 2020 2020 2020 2020 732e                s.
-0000d1f0: 6c6f 636b 5f62 6f74 6828 290d 0a20 2020  lock_both()..   
-0000d200: 2020 2020 2020 2020 2020 2020 2064 656c               del
-0000d210: 2073 656c 662e 7365 676d 656e 7473 5b69   self.segments[i
-0000d220: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0000d230: 2020 2066 6f72 2073 2069 6e20 7265 7665     for s in reve
-0000d240: 7273 6564 286e 6577 5f73 6567 6d65 6e74  rsed(new_segment
-0000d250: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
-0000d260: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0000d270: 676d 656e 7473 2e69 6e73 6572 7428 692c  gments.insert(i,
-0000d280: 2073 290d 0a20 2020 2020 2020 2069 6620   s)..        if 
-0000d290: 6e6f 5f77 6f72 6473 3a0d 0a20 2020 2020  no_words:..     
-0000d2a0: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-0000d2b0: 7761 726e 2827 466f 756e 6420 7365 676d  warn('Found segm
-0000d2c0: 656e 7428 7329 2077 6974 686f 7574 2077  ent(s) without w
-0000d2d0: 6f72 6420 7469 6d69 6e67 732e 2054 6865  ord timings. The
-0000d2e0: 7365 2073 6567 6d65 6e74 2873 2920 6361  se segment(s) ca
-0000d2f0: 6e6e 6f74 2062 6520 7370 6c69 742e 2729  nnot be split.')
-0000d300: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-0000d310: 656d 6f76 655f 6e6f 5f77 6f72 645f 7365  emove_no_word_se
-0000d320: 676d 656e 7473 2829 0d0a 0d0a 2020 2020  gments()....    
-0000d330: 6465 6620 5f6d 6572 6765 5f73 6567 6d65  def _merge_segme
-0000d340: 6e74 7328 7365 6c66 2c20 696e 6469 6365  nts(self, indice
-0000d350: 733a 204c 6973 745b 696e 745d 2c0d 0a20  s: List[int],.. 
-0000d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d370: 2020 2020 2020 202a 2c20 6d61 785f 776f         *, max_wo
-0000d380: 7264 733a 2069 6e74 203d 204e 6f6e 652c  rds: int = None,
-0000d390: 206d 6178 5f63 6861 7273 3a20 696e 7420   max_chars: int 
-0000d3a0: 3d20 4e6f 6e65 2c20 6973 5f73 756d 5f6d  = None, is_sum_m
-0000d3b0: 6178 3a20 626f 6f6c 203d 2046 616c 7365  ax: bool = False
-0000d3c0: 2c20 6c6f 636b 3a20 626f 6f6c 203d 2046  , lock: bool = F
-0000d3d0: 616c 7365 293a 0d0a 2020 2020 2020 2020  alse):..        
-0000d3e0: 6966 206c 656e 2869 6e64 6963 6573 2920  if len(indices) 
-0000d3f0: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
-0000d400: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
-0000d410: 2020 2066 6f72 2069 2069 6e20 7265 7665     for i in reve
-0000d420: 7273 6564 2869 6e64 6963 6573 293a 0d0a  rsed(indices):..
-0000d430: 2020 2020 2020 2020 2020 2020 7365 6720              seg 
-0000d440: 3d20 7365 6c66 2e73 6567 6d65 6e74 735b  = self.segments[
-0000d450: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
-0000d460: 6966 2028 0d0a 2020 2020 2020 2020 2020  if (..          
-0000d470: 2020 2020 2020 2020 2020 280d 0a20 2020            (..   
-0000d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d490: 2020 2020 2020 2020 206d 6178 5f77 6f72           max_wor
-0000d4a0: 6473 2061 6e64 0d0a 2020 2020 2020 2020  ds and..        
-0000d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4c0: 2020 2020 7365 672e 6861 735f 776f 7264      seg.has_word
-0000d4d0: 7320 616e 640d 0a20 2020 2020 2020 2020  s and..         
-0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4f0: 2020 2028 0d0a 2020 2020 2020 2020 2020     (..          
-0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d510: 2020 2020 2020 2020 2020 2873 6567 2e77            (seg.w
-0000d520: 6f72 645f 636f 756e 7428 2920 2b20 7365  ord_count() + se
-0000d530: 6c66 2e73 6567 6d65 6e74 735b 6920 2b20  lf.segments[i + 
-0000d540: 315d 2e77 6f72 645f 636f 756e 7428 2920  1].word_count() 
-0000d550: 3e20 6d61 785f 776f 7264 7329 0d0a 2020  > max_words)..  
-0000d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d580: 2020 6966 2069 735f 7375 6d5f 6d61 7820    if is_sum_max 
-0000d590: 656c 7365 0d0a 2020 2020 2020 2020 2020  else..          
-0000d5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5b0: 2020 2020 2020 2020 2020 2873 6567 2e77            (seg.w
-0000d5c0: 6f72 645f 636f 756e 7428 2920 3e20 6d61  ord_count() > ma
-0000d5d0: 785f 776f 7264 7320 616e 6420 7365 6c66  x_words and self
-0000d5e0: 2e73 6567 6d65 6e74 735b 6920 2b20 315d  .segments[i + 1]
-0000d5f0: 2e77 6f72 645f 636f 756e 7428 2920 3e20  .word_count() > 
-0000d600: 6d61 785f 776f 7264 7329 0d0a 2020 2020  max_words)..    
+0000d020: 2020 6966 2073 656c 662e 7365 676d 656e    if self.segmen
+0000d030: 7473 5b69 5d2e 776f 7264 735b 776f 7264  ts[i].words[word
+0000d040: 5f69 6478 5d2e 776f 7264 2e65 6e64 7377  _idx].word.endsw
+0000d050: 6974 6828 275c 6e27 293a 0d0a 2020 2020  ith('\n'):..    
+0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d070: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
+0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d090: 2020 7365 6c66 2e73 6567 6d65 6e74 735b    self.segments[
+0000d0a0: 695d 2e77 6f72 6473 5b77 6f72 645f 6964  i].words[word_id
+0000d0b0: 785d 2e77 6f72 6420 2b3d 2027 5c6e 270d  x].word += '\n'.
+0000d0c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d0d0: 2020 2020 2069 6620 6c6f 636b 3a0d 0a20       if lock:.. 
+0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0f0: 2020 2020 2020 2073 656c 662e 7365 676d         self.segm
+0000d100: 656e 7473 5b69 5d2e 776f 7264 735b 776f  ents[i].words[wo
+0000d110: 7264 5f69 6478 5d2e 6c6f 636b 5f72 6967  rd_idx].lock_rig
+0000d120: 6874 2829 0d0a 2020 2020 2020 2020 2020  ht()..          
+0000d130: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000d140: 2077 6f72 645f 6964 7820 2b20 3120 3c20   word_idx + 1 < 
+0000d150: 6c65 6e28 7365 6c66 2e73 6567 6d65 6e74  len(self.segment
+0000d160: 735b 695d 2e77 6f72 6473 293a 0d0a 2020  s[i].words):..  
+0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d180: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000d190: 6567 6d65 6e74 735b 695d 2e77 6f72 6473  egments[i].words
+0000d1a0: 5b77 6f72 645f 6964 782b 315d 2e6c 6f63  [word_idx+1].loc
+0000d1b0: 6b5f 6c65 6674 2829 0d0a 2020 2020 2020  k_left()..      
+0000d1c0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0000d1d0: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000d1e0: 5f73 6567 6d65 6e74 7320 3d20 7365 6c66  _segments = self
+0000d1f0: 2e73 6567 6d65 6e74 735b 695d 2e73 706c  .segments[i].spl
+0000d200: 6974 2869 6e64 6963 6573 290d 0a20 2020  it(indices)..   
+0000d210: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d220: 6c6f 636b 3a0d 0a20 2020 2020 2020 2020  lock:..         
+0000d230: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
+0000d240: 2069 6e20 6e65 775f 7365 676d 656e 7473   in new_segments
+0000d250: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000d260: 2020 2020 2020 2020 2020 2069 6620 7320             if s 
+0000d270: 3d3d 206e 6577 5f73 6567 6d65 6e74 735b  == new_segments[
+0000d280: 305d 3a0d 0a20 2020 2020 2020 2020 2020  0]:..           
+0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2a0: 2073 2e6c 6f63 6b5f 7269 6768 7428 290d   s.lock_right().
+0000d2b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d2c0: 2020 2020 2020 2020 2065 6c69 6620 7320           elif s 
+0000d2d0: 3d3d 206e 6577 5f73 6567 6d65 6e74 735b  == new_segments[
+0000d2e0: 2d31 5d3a 0d0a 2020 2020 2020 2020 2020  -1]:..          
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d300: 2020 732e 6c6f 636b 5f6c 6566 7428 290d    s.lock_left().
+0000d310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d320: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d340: 2020 2020 2020 2020 2020 2020 732e 6c6f              s.lo
+0000d350: 636b 5f62 6f74 6828 290d 0a20 2020 2020  ck_both()..     
+0000d360: 2020 2020 2020 2020 2020 2064 656c 2073             del s
+0000d370: 656c 662e 7365 676d 656e 7473 5b69 5d0d  elf.segments[i].
+0000d380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d390: 2066 6f72 2073 2069 6e20 7265 7665 7273   for s in revers
+0000d3a0: 6564 286e 6577 5f73 6567 6d65 6e74 7329  ed(new_segments)
+0000d3b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000d3c0: 2020 2020 2020 2073 656c 662e 7365 676d         self.segm
+0000d3d0: 656e 7473 2e69 6e73 6572 7428 692c 2073  ents.insert(i, s
+0000d3e0: 290d 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+0000d3f0: 5f77 6f72 6473 3a0d 0a20 2020 2020 2020  _words:..       
+0000d400: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+0000d410: 726e 2827 466f 756e 6420 7365 676d 656e  rn('Found segmen
+0000d420: 7428 7329 2077 6974 686f 7574 2077 6f72  t(s) without wor
+0000d430: 6420 7469 6d69 6e67 732e 2054 6865 7365  d timings. These
+0000d440: 2073 6567 6d65 6e74 2873 2920 6361 6e6e   segment(s) cann
+0000d450: 6f74 2062 6520 7370 6c69 742e 2729 0d0a  ot be split.')..
+0000d460: 2020 2020 2020 2020 7365 6c66 2e72 656d          self.rem
+0000d470: 6f76 655f 6e6f 5f77 6f72 645f 7365 676d  ove_no_word_segm
+0000d480: 656e 7473 2829 0d0a 0d0a 2020 2020 6465  ents()....    de
+0000d490: 6620 5f6d 6572 6765 5f73 6567 6d65 6e74  f _merge_segment
+0000d4a0: 7328 7365 6c66 2c20 696e 6469 6365 733a  s(self, indices:
+0000d4b0: 204c 6973 745b 696e 745d 2c0d 0a20 2020   List[int],..   
+0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4d0: 2020 2020 202a 2c20 6d61 785f 776f 7264       *, max_word
+0000d4e0: 733a 2069 6e74 203d 204e 6f6e 652c 206d  s: int = None, m
+0000d4f0: 6178 5f63 6861 7273 3a20 696e 7420 3d20  ax_chars: int = 
+0000d500: 4e6f 6e65 2c20 6973 5f73 756d 5f6d 6178  None, is_sum_max
+0000d510: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
+0000d520: 6c6f 636b 3a20 626f 6f6c 203d 2046 616c  lock: bool = Fal
+0000d530: 7365 293a 0d0a 2020 2020 2020 2020 6966  se):..        if
+0000d540: 206c 656e 2869 6e64 6963 6573 2920 3d3d   len(indices) ==
+0000d550: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+0000d560: 2072 6574 7572 6e0d 0a20 2020 2020 2020   return..       
+0000d570: 2066 6f72 2069 2069 6e20 7265 7665 7273   for i in revers
+0000d580: 6564 2869 6e64 6963 6573 293a 0d0a 2020  ed(indices):..  
+0000d590: 2020 2020 2020 2020 2020 7365 6720 3d20            seg = 
+0000d5a0: 7365 6c66 2e73 6567 6d65 6e74 735b 695d  self.segments[i]
+0000d5b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000d5c0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+0000d5d0: 2020 2020 2020 2020 280d 0a20 2020 2020          (..     
+0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5f0: 2020 2020 2020 206d 6178 5f77 6f72 6473         max_words
+0000d600: 2061 6e64 0d0a 2020 2020 2020 2020 2020   and..          
 0000d610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d620: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0000d630: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000d640: 206f 720d 0a20 2020 2020 2020 2020 2020   or..           
-0000d650: 2020 2020 2020 2020 2028 0d0a 2020 2020           (..    
+0000d620: 2020 7365 672e 6861 735f 776f 7264 7320    seg.has_words 
+0000d630: 616e 640d 0a20 2020 2020 2020 2020 2020  and..           
+0000d640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d650: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
 0000d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d670: 2020 2020 2020 2020 6d61 785f 6368 6172          max_char
-0000d680: 7320 616e 640d 0a20 2020 2020 2020 2020  s and..         
-0000d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6a0: 2020 2028 0d0a 2020 2020 2020 2020 2020     (..          
-0000d6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6c0: 2020 2020 2020 2020 2020 2873 6567 2e63            (seg.c
-0000d6d0: 6861 725f 636f 756e 7428 2920 2b20 7365  har_count() + se
-0000d6e0: 6c66 2e73 6567 6d65 6e74 735b 6920 2b20  lf.segments[i + 
-0000d6f0: 315d 2e63 6861 725f 636f 756e 7428 2920  1].char_count() 
-0000d700: 3e20 6d61 785f 6368 6172 7329 0d0a 2020  > max_chars)..  
-0000d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d730: 2020 6966 2069 735f 7375 6d5f 6d61 7820    if is_sum_max 
-0000d740: 656c 7365 0d0a 2020 2020 2020 2020 2020  else..          
-0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d760: 2020 2020 2020 2020 2020 2873 6567 2e63            (seg.c
-0000d770: 6861 725f 636f 756e 7428 2920 3e20 6d61  har_count() > ma
-0000d780: 785f 6368 6172 7320 616e 6420 7365 6c66  x_chars and self
-0000d790: 2e73 6567 6d65 6e74 735b 6920 2b20 315d  .segments[i + 1]
-0000d7a0: 2e63 6861 725f 636f 756e 7428 2920 3e20  .char_count() > 
-0000d7b0: 6d61 785f 6368 6172 7329 0d0a 2020 2020  max_chars)..    
+0000d670: 2020 2020 2020 2020 2873 6567 2e77 6f72          (seg.wor
+0000d680: 645f 636f 756e 7428 2920 2b20 7365 6c66  d_count() + self
+0000d690: 2e73 6567 6d65 6e74 735b 6920 2b20 315d  .segments[i + 1]
+0000d6a0: 2e77 6f72 645f 636f 756e 7428 2920 3e20  .word_count() > 
+0000d6b0: 6d61 785f 776f 7264 7329 0d0a 2020 2020  max_words)..    
+0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6e0: 6966 2069 735f 7375 6d5f 6d61 7820 656c  if is_sum_max el
+0000d6f0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
+0000d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d710: 2020 2020 2020 2020 2873 6567 2e77 6f72          (seg.wor
+0000d720: 645f 636f 756e 7428 2920 3e20 6d61 785f  d_count() > max_
+0000d730: 776f 7264 7320 616e 6420 7365 6c66 2e73  words and self.s
+0000d740: 6567 6d65 6e74 735b 6920 2b20 315d 2e77  egments[i + 1].w
+0000d750: 6f72 645f 636f 756e 7428 2920 3e20 6d61  ord_count() > ma
+0000d760: 785f 776f 7264 7329 0d0a 2020 2020 2020  x_words)..      
+0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d780: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0000d790: 2020 2020 2020 2020 2020 2020 2029 206f               ) o
+0000d7a0: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
+0000d7b0: 2020 2020 2020 2028 0d0a 2020 2020 2020         (..      
 0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7d0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0000d7e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000d7f0: 0d0a 2020 2020 2020 2020 2020 2020 293a  ..            ):
-0000d800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d810: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
-0000d820: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
-0000d830: 5f73 6567 6d65 6e74 7328 692c 2069 202b  _segments(i, i +
-0000d840: 2031 2c20 696e 706c 6163 653d 5472 7565   1, inplace=True
-0000d850: 2c20 6c6f 636b 3d6c 6f63 6b29 0d0a 2020  , lock=lock)..  
-0000d860: 2020 2020 2020 7365 6c66 2e72 656d 6f76        self.remov
-0000d870: 655f 6e6f 5f77 6f72 645f 7365 676d 656e  e_no_word_segmen
-0000d880: 7473 2829 0d0a 0d0a 2020 2020 6465 6620  ts()....    def 
-0000d890: 6765 745f 636f 6e74 656e 745f 6279 5f74  get_content_by_t
-0000d8a0: 696d 6528 0d0a 2020 2020 2020 2020 2020  ime(..          
-0000d8b0: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-0000d8c0: 2020 2020 2074 696d 653a 2055 6e69 6f6e       time: Union
-0000d8d0: 5b66 6c6f 6174 2c20 5475 706c 655b 666c  [float, Tuple[fl
-0000d8e0: 6f61 742c 2066 6c6f 6174 5d2c 2064 6963  oat, float], dic
-0000d8f0: 745d 2c0d 0a20 2020 2020 2020 2020 2020  t],..           
-0000d900: 2077 6974 6869 6e3a 2062 6f6f 6c20 3d20   within: bool = 
-0000d910: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000d920: 2020 2020 7365 676d 656e 745f 6c65 7665      segment_leve
-0000d930: 6c3a 2062 6f6f 6c20 3d20 4661 6c73 650d  l: bool = False.
-0000d940: 0a20 2020 2029 202d 3e20 556e 696f 6e5b  .    ) -> Union[
-0000d950: 4c69 7374 5b57 6f72 6454 696d 696e 675d  List[WordTiming]
-0000d960: 2c20 4c69 7374 5b53 6567 6d65 6e74 5d5d  , List[Segment]]
-0000d970: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-0000d980: 2020 2020 2020 2020 5265 7475 726e 2063          Return c
-0000d990: 6f6e 7465 6e74 2069 6e20 7468 6520 6060  ontent in the ``
-0000d9a0: 7469 6d65 6060 2072 616e 6765 2e0d 0a0d  time`` range....
-0000d9b0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0000d9c0: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
-0000d9d0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-0000d9e0: 2074 696d 6520 3a20 666c 6f61 7420 6f72   time : float or
-0000d9f0: 2074 7570 6c65 206f 6620 2866 6c6f 6174   tuple of (float
-0000da00: 2c20 666c 6f61 7429 206f 7220 6469 6374  , float) or dict
-0000da10: 0d0a 2020 2020 2020 2020 2020 2020 5261  ..            Ra
-0000da20: 6e67 6520 6f66 2074 696d 6520 746f 2066  nge of time to f
-0000da30: 696e 6420 636f 6e74 656e 742e 2046 6f72  ind content. For
-0000da40: 2074 7570 6c65 206f 6620 7477 6f20 666c   tuple of two fl
-0000da50: 6f61 7473 2c20 6669 7273 7420 7661 6c75  oats, first valu
-0000da60: 6520 6973 2074 6865 2073 7461 7274 2074  e is the start t
-0000da70: 696d 6520 616e 6420 7365 636f 6e64 2076  ime and second v
-0000da80: 616c 7565 2069 730d 0a20 2020 2020 2020  alue is..       
-0000da90: 2020 2020 2074 6865 2065 6e64 2074 696d       the end tim
-0000daa0: 652e 2046 6f72 2061 2073 696e 676c 6520  e. For a single 
-0000dab0: 666c 6f61 7420 7661 6c75 652c 2069 7420  float value, it 
-0000dac0: 6973 2074 7265 6174 6564 2061 7320 626f  is treated as bo
-0000dad0: 7468 2074 6865 2073 7461 7274 2061 6e64  th the start and
-0000dae0: 2065 6e64 2074 696d 652e 0d0a 2020 2020   end time...    
-0000daf0: 2020 2020 7769 7468 696e 203a 2062 6f6f      within : boo
-0000db00: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-0000db10: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-0000db20: 6574 6865 7220 746f 206f 6e6c 7920 6669  ether to only fi
-0000db30: 6e64 2063 6f6e 7465 6e74 2066 756c 6c79  nd content fully
-0000db40: 206f 7665 726c 6170 7320 7769 7468 2060   overlaps with `
-0000db50: 6074 696d 6560 6020 7261 6e67 652e 0d0a  `time`` range...
-0000db60: 2020 2020 2020 2020 7365 676d 656e 745f          segment_
-0000db70: 6c65 7665 6c20 3a20 626f 6f6c 2c20 6465  level : bool, de
-0000db80: 6661 756c 7420 4661 6c73 650d 0a20 2020  fault False..   
-0000db90: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
-0000dba0: 2074 6f20 6c6f 6f6b 206f 6e6c 7920 6f6e   to look only on
-0000dbb0: 2074 6865 2073 6567 6d65 6e74 206c 6576   the segment lev
-0000dbc0: 656c 2061 6e64 2072 6574 7572 6e20 696e  el and return in
-0000dbd0: 7374 616e 6365 7320 6f66 203a 636c 6173  stances of :clas
-0000dbe0: 733a 6073 7461 626c 655f 7768 6973 7065  s:`stable_whispe
-0000dbf0: 722e 7265 7375 6c74 2e53 6567 6d65 6e74  r.result.Segment
-0000dc00: 600d 0a20 2020 2020 2020 2020 2020 2069  `..            i
-0000dc10: 6e73 7465 6164 206f 6620 3a63 6c61 7373  nstead of :class
-0000dc20: 3a60 7374 6162 6c65 5f77 6869 7370 6572  :`stable_whisper
-0000dc30: 2e72 6573 756c 742e 576f 7264 5469 6d69  .result.WordTimi
-0000dc40: 6e67 602e 0d0a 0d0a 2020 2020 2020 2020  ng`.....        
-0000dc50: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
-0000dc60: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020   -------..      
-0000dc70: 2020 6c69 7374 206f 6620 7374 6162 6c65    list of stable
-0000dc80: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
-0000dc90: 576f 7264 5469 6d69 6e67 206f 7220 6c69  WordTiming or li
-0000dca0: 7374 206f 6620 7374 6162 6c65 5f77 6869  st of stable_whi
-0000dcb0: 7370 6572 2e72 6573 756c 742e 5365 676d  sper.result.Segm
-0000dcc0: 656e 740d 0a20 2020 2020 2020 2020 2020  ent..           
-0000dcd0: 204c 6973 7420 6f66 2063 6f6e 7465 6e74   List of content
-0000dce0: 7320 696e 2074 6865 2060 6074 696d 6560  s in the ``time`
-0000dcf0: 6020 7261 6e67 652e 2054 6865 2063 6f6e  ` range. The con
-0000dd00: 7465 6e74 7320 6172 6520 696e 7374 616e  tents are instan
-0000dd10: 6365 7320 6f66 0d0a 2020 2020 2020 2020  ces of..        
-0000dd20: 2020 2020 3a63 6c61 7373 3a60 7374 6162      :class:`stab
-0000dd30: 6c65 5f77 6869 7370 6572 2e72 6573 756c  le_whisper.resul
-0000dd40: 742e 5365 676d 656e 7460 2069 6620 6060  t.Segment` if ``
-0000dd50: 7365 676d 656e 745f 6c65 7665 6c20 3d20  segment_level = 
-0000dd60: 5472 7565 6060 2065 6c73 650d 0a20 2020  True`` else..   
-0000dd70: 2020 2020 2020 2020 203a 636c 6173 733a           :class:
-0000dd80: 6073 7461 626c 655f 7768 6973 7065 722e  `stable_whisper.
-0000dd90: 7265 7375 6c74 2e57 6f72 6454 696d 696e  result.WordTimin
-0000dda0: 6760 2e0d 0a20 2020 2020 2020 2022 2222  g`...        """
-0000ddb0: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-0000ddc0: 2073 6567 6d65 6e74 5f6c 6576 656c 2061   segment_level a
-0000ddd0: 6e64 206e 6f74 2073 656c 662e 6861 735f  nd not self.has_
-0000dde0: 776f 7264 733a 0d0a 2020 2020 2020 2020  words:..        
-0000ddf0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000de00: 7272 6f72 2827 4d69 7373 696e 6720 776f  rror('Missing wo
-0000de10: 7264 2074 696d 6573 7461 6d70 7320 696e  rd timestamps in
-0000de20: 2072 6573 756c 742e 2055 7365 2060 6073   result. Use ``s
-0000de30: 6567 6d65 6e74 5f6c 6576 656c 3d54 7275  egment_level=Tru
-0000de40: 6560 6020 696e 7374 6561 642e 2729 0d0a  e`` instead.')..
-0000de50: 2020 2020 2020 2020 636f 6e74 656e 7473          contents
-0000de60: 203d 2073 656c 662e 7365 676d 656e 7473   = self.segments
-0000de70: 2069 6620 7365 676d 656e 745f 6c65 7665   if segment_leve
-0000de80: 6c20 656c 7365 2073 656c 662e 616c 6c5f  l else self.all_
-0000de90: 776f 7264 7328 290d 0a20 2020 2020 2020  words()..       
-0000dea0: 2069 6620 6973 696e 7374 616e 6365 2874   if isinstance(t
-0000deb0: 696d 652c 2028 666c 6f61 742c 2069 6e74  ime, (float, int
-0000dec0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-0000ded0: 2074 696d 6520 3d20 5b74 696d 652c 2074   time = [time, t
-0000dee0: 696d 655d 0d0a 2020 2020 2020 2020 656c  ime]..        el
-0000def0: 6966 2069 7369 6e73 7461 6e63 6528 7469  if isinstance(ti
-0000df00: 6d65 2c20 6469 6374 293a 0d0a 2020 2020  me, dict):..    
-0000df10: 2020 2020 2020 2020 7469 6d65 203d 205b          time = [
-0000df20: 7469 6d65 5b27 7374 6172 7427 5d2c 2074  time['start'], t
-0000df30: 696d 655b 2765 6e64 275d 5d0d 0a20 2020  ime['end']]..   
-0000df40: 2020 2020 2073 7461 7274 2c20 656e 6420       start, end 
-0000df50: 3d20 7469 6d65 0d0a 0d0a 2020 2020 2020  = time....      
-0000df60: 2020 6966 2077 6974 6869 6e3a 0d0a 2020    if within:..  
-0000df70: 2020 2020 2020 2020 2020 6465 6620 6973            def is
-0000df80: 5f69 6e5f 7261 6e67 6528 6329 3a0d 0a20  _in_range(c):.. 
-0000df90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000dfa0: 6574 7572 6e20 7374 6172 7420 3c3d 2063  eturn start <= c
-0000dfb0: 2e73 7461 7274 2061 6e64 2065 6e64 203e  .start and end >
-0000dfc0: 3d20 632e 656e 640d 0a20 2020 2020 2020  = c.end..       
-0000dfd0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0000dfe0: 2020 2020 6465 6620 6973 5f69 6e5f 7261      def is_in_ra
-0000dff0: 6e67 6528 6329 3a0d 0a20 2020 2020 2020  nge(c):..       
-0000e000: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000e010: 7374 6172 7420 3c3d 2063 2e65 6e64 2061  start <= c.end a
-0000e020: 6e64 2065 6e64 203e 3d20 632e 7374 6172  nd end >= c.star
-0000e030: 740d 0a0d 0a20 2020 2020 2020 2072 6574  t....        ret
-0000e040: 7572 6e20 5b63 2066 6f72 2063 2069 6e20  urn [c for c in 
-0000e050: 636f 6e74 656e 7473 2069 6620 6973 5f69  contents if is_i
-0000e060: 6e5f 7261 6e67 6528 6329 5d0d 0a0d 0a20  n_range(c)].... 
-0000e070: 2020 2064 6566 2073 706c 6974 5f62 795f     def split_by_
-0000e080: 6761 7028 0d0a 2020 2020 2020 2020 2020  gap(..          
-0000e090: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-0000e0a0: 2020 2020 206d 6178 5f67 6170 3a20 666c       max_gap: fl
-0000e0b0: 6f61 7420 3d20 302e 312c 0d0a 2020 2020  oat = 0.1,..    
-0000e0c0: 2020 2020 2020 2020 6c6f 636b 3a20 626f          lock: bo
-0000e0d0: 6f6c 203d 2046 616c 7365 2c0d 0a20 2020  ol = False,..   
-0000e0e0: 2020 2020 2020 2020 206e 6577 6c69 6e65           newline
-0000e0f0: 3a20 626f 6f6c 203d 2046 616c 7365 0d0a  : bool = False..
-0000e100: 2020 2020 2920 2d3e 2022 5768 6973 7065      ) -> "Whispe
-0000e110: 7252 6573 756c 7422 3a0d 0a20 2020 2020  rResult":..     
-0000e120: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-0000e130: 5370 6c69 7420 2869 6e2d 706c 6163 6529  Split (in-place)
-0000e140: 2061 6e79 2073 6567 6d65 6e74 2077 6865   any segment whe
-0000e150: 7265 2074 6865 2067 6170 2062 6574 7765  re the gap betwe
-0000e160: 656e 2074 776f 206f 6620 6974 7320 776f  en two of its wo
-0000e170: 7264 7320 6973 2067 7265 6174 6572 2074  rds is greater t
-0000e180: 6861 6e20 6060 6d61 785f 6761 7060 602e  han ``max_gap``.
-0000e190: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
-0000e1a0: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
-0000e1b0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
-0000e1c0: 2020 2020 6d61 785f 6761 7020 3a20 666c      max_gap : fl
-0000e1d0: 6f61 742c 2064 6566 6175 6c74 2030 2e31  oat, default 0.1
-0000e1e0: 0d0a 2020 2020 2020 2020 2020 2020 4d61  ..            Ma
-0000e1f0: 7869 6d75 6d20 7365 636f 6e64 2873 2920  ximum second(s) 
-0000e200: 616c 6c6f 7765 6420 6265 7477 6565 6e20  allowed between 
-0000e210: 7477 6f20 776f 7264 7320 6966 2074 6865  two words if the
-0000e220: 2073 616d 6520 7365 676d 656e 742e 0d0a   same segment...
-0000e230: 2020 2020 2020 2020 6c6f 636b 203a 2062          lock : b
-0000e240: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
-0000e250: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-0000e260: 5768 6574 6865 7220 746f 2070 7265 7665  Whether to preve
-0000e270: 6e74 2066 7574 7572 6520 7370 6c69 7473  nt future splits
-0000e280: 2f6d 6572 6765 7320 6672 6f6d 2061 6c74  /merges from alt
-0000e290: 6572 696e 6720 6368 616e 6765 7320 6d61  ering changes ma
-0000e2a0: 6465 2062 7920 7468 6973 206d 6574 686f  de by this metho
-0000e2b0: 642e 0d0a 2020 2020 2020 2020 6e65 776c  d...        newl
-0000e2c0: 696e 653a 2062 6f6f 6c2c 2064 6566 6175  ine: bool, defau
-0000e2d0: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
-0000e2e0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-0000e2f0: 2069 6e73 6572 7420 6c69 6e65 2062 7265   insert line bre
-0000e300: 616b 2061 7420 7468 6520 7370 6c69 7420  ak at the split 
-0000e310: 706f 696e 7473 2069 6e73 7465 6164 206f  points instead o
-0000e320: 6620 7370 6c69 7474 696e 6720 696e 746f  f splitting into
-0000e330: 2073 6570 6172 6174 6520 7365 676d 656e   separate segmen
-0000e340: 7473 2e0d 0a0d 0a20 2020 2020 2020 2052  ts.....        R
-0000e350: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
-0000e360: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-0000e370: 2073 7461 626c 655f 7768 6973 7065 722e   stable_whisper.
-0000e380: 7265 7375 6c74 2e57 6869 7370 6572 5265  result.WhisperRe
-0000e390: 7375 6c74 0d0a 2020 2020 2020 2020 2020  sult..          
-0000e3a0: 2020 5468 6520 6375 7272 656e 7420 696e    The current in
-0000e3b0: 7374 616e 6365 2061 6674 6572 2074 6865  stance after the
-0000e3c0: 2063 6861 6e67 6573 2e0d 0a20 2020 2020   changes...     
-0000e3d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-0000e3e0: 7365 6c66 2e5f 7370 6c69 745f 7365 676d  self._split_segm
-0000e3f0: 656e 7473 286c 616d 6264 6120 783a 2078  ents(lambda x: x
-0000e400: 2e67 6574 5f67 6170 5f69 6e64 6963 6573  .get_gap_indices
-0000e410: 286d 6178 5f67 6170 292c 206c 6f63 6b3d  (max_gap), lock=
-0000e420: 6c6f 636b 2c20 6e65 776c 696e 653d 6e65  lock, newline=ne
-0000e430: 776c 696e 6529 0d0a 2020 2020 2020 2020  wline)..        
-0000e440: 6966 2073 656c 662e 5f72 6567 726f 7570  if self._regroup
-0000e450: 5f68 6973 746f 7279 3a0d 0a20 2020 2020  _history:..     
-0000e460: 2020 2020 2020 2073 656c 662e 5f72 6567         self._reg
-0000e470: 726f 7570 5f68 6973 746f 7279 202b 3d20  roup_history += 
-0000e480: 275f 270d 0a20 2020 2020 2020 2073 656c  '_'..        sel
-0000e490: 662e 5f72 6567 726f 7570 5f68 6973 746f  f._regroup_histo
-0000e4a0: 7279 202b 3d20 6627 7367 3d7b 6d61 785f  ry += f'sg={max_
-0000e4b0: 6761 707d 2b7b 696e 7428 6c6f 636b 297d  gap}+{int(lock)}
-0000e4c0: 2b7b 696e 7428 6e65 776c 696e 6529 7d27  +{int(newline)}'
-0000e4d0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000e4e0: 2073 656c 660d 0a0d 0a20 2020 2064 6566   self....    def
-0000e4f0: 206d 6572 6765 5f62 795f 6761 7028 0d0a   merge_by_gap(..
-0000e500: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e510: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-0000e520: 696e 5f67 6170 3a20 666c 6f61 7420 3d20  in_gap: float = 
-0000e530: 302e 312c 0d0a 2020 2020 2020 2020 2020  0.1,..          
-0000e540: 2020 6d61 785f 776f 7264 733a 2069 6e74    max_words: int
-0000e550: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-0000e560: 2020 2020 2020 6d61 785f 6368 6172 733a        max_chars:
-0000e570: 2069 6e74 203d 204e 6f6e 652c 0d0a 2020   int = None,..  
-0000e580: 2020 2020 2020 2020 2020 6973 5f73 756d            is_sum
-0000e590: 5f6d 6178 3a20 626f 6f6c 203d 2046 616c  _max: bool = Fal
-0000e5a0: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000e5b0: 206c 6f63 6b3a 2062 6f6f 6c20 3d20 4661   lock: bool = Fa
-0000e5c0: 6c73 650d 0a20 2020 2029 202d 3e20 2257  lse..    ) -> "W
-0000e5d0: 6869 7370 6572 5265 7375 6c74 223a 0d0a  hisperResult":..
-0000e5e0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0000e5f0: 2020 2020 204d 6572 6765 2028 696e 2d70       Merge (in-p
-0000e600: 6c61 6365 2920 616e 7920 7061 6972 206f  lace) any pair o
-0000e610: 6620 6164 6a61 6365 6e74 2073 6567 6d65  f adjacent segme
-0000e620: 6e74 7320 6966 2074 6865 2067 6170 2062  nts if the gap b
-0000e630: 6574 7765 656e 2074 6865 6d20 3c3d 2060  etween them <= `
-0000e640: 606d 696e 5f67 6170 6060 2e0d 0a0d 0a20  `min_gap``..... 
-0000e650: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-0000e660: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-0000e670: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 206d  -----..        m
-0000e680: 696e 5f67 6170 203a 2066 6c6f 6174 2c20  in_gap : float, 
-0000e690: 6465 6661 756c 7420 302e 310d 0a20 2020  default 0.1..   
-0000e6a0: 2020 2020 2020 2020 204d 696e 696d 756d           Minimum
-0000e6b0: 2073 6563 6f6e 6428 7329 2061 6c6c 6f77   second(s) allow
-0000e6c0: 2062 6574 7765 656e 2074 776f 2073 6567   between two seg
-0000e6d0: 6d65 6e74 2e0d 0a20 2020 2020 2020 206d  ment...        m
-0000e6e0: 6178 5f77 6f72 6473 203a 2069 6e74 2c20  ax_words : int, 
-0000e6f0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-0000e700: 2020 2020 2020 4d61 7869 6d75 6d20 6e75        Maximum nu
-0000e710: 6d62 6572 206f 6620 776f 7264 7320 616c  mber of words al
-0000e720: 6c6f 7765 6420 696e 2065 6163 6820 7365  lowed in each se
-0000e730: 676d 656e 742e 0d0a 2020 2020 2020 2020  gment...        
-0000e740: 6d61 785f 6368 6172 7320 3a20 696e 742c  max_chars : int,
-0000e750: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-0000e760: 2020 2020 2020 204d 6178 696d 756d 206e         Maximum n
-0000e770: 756d 6265 7220 6f66 2063 6861 7261 6374  umber of charact
-0000e780: 6572 7320 616c 6c6f 7765 6420 696e 2065  ers allowed in e
-0000e790: 6163 6820 7365 676d 656e 742e 0d0a 2020  ach segment...  
-0000e7a0: 2020 2020 2020 6973 5f73 756d 5f6d 6178        is_sum_max
-0000e7b0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-0000e7c0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-0000e7d0: 2020 2020 5768 6574 6865 7220 6060 6d61      Whether ``ma
-0000e7e0: 785f 776f 7264 7360 6020 616e 6420 6060  x_words`` and ``
-0000e7f0: 6d61 785f 6368 6172 7360 6020 6973 2061  max_chars`` is a
-0000e800: 7070 6c69 6564 2074 6f20 7468 6520 6d65  pplied to the me
-0000e810: 7267 6564 2073 6567 6d65 6e74 2069 6e73  rged segment ins
-0000e820: 7465 6164 206f 6620 7468 6520 696e 6469  tead of the indi
-0000e830: 7669 6475 616c 2073 6567 6d65 6e74 730d  vidual segments.
-0000e840: 0a20 2020 2020 2020 2020 2020 2074 6f20  .            to 
-0000e850: 6265 206d 6572 6765 642e 0d0a 2020 2020  be merged...    
-0000e860: 2020 2020 6c6f 636b 203a 2062 6f6f 6c2c      lock : bool,
-0000e870: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
-0000e880: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-0000e890: 6865 7220 746f 2070 7265 7665 6e74 2066  her to prevent f
-0000e8a0: 7574 7572 6520 7370 6c69 7473 2f6d 6572  uture splits/mer
-0000e8b0: 6765 7320 6672 6f6d 2061 6c74 6572 696e  ges from alterin
-0000e8c0: 6720 6368 616e 6765 7320 6d61 6465 2062  g changes made b
-0000e8d0: 7920 7468 6973 206d 6574 686f 642e 0d0a  y this method...
-0000e8e0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000e8f0: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-0000e900: 2d2d 0d0a 2020 2020 2020 2020 7374 6162  --..        stab
-0000e910: 6c65 5f77 6869 7370 6572 2e72 6573 756c  le_whisper.resul
-0000e920: 742e 5768 6973 7065 7252 6573 756c 740d  t.WhisperResult.
-0000e930: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-0000e940: 2063 7572 7265 6e74 2069 6e73 7461 6e63   current instanc
-0000e950: 6520 6166 7465 7220 7468 6520 6368 616e  e after the chan
-0000e960: 6765 732e 0d0a 2020 2020 2020 2020 2222  ges...        ""
-0000e970: 220d 0a20 2020 2020 2020 2069 6e64 6963  "..        indic
-0000e980: 6573 203d 2073 656c 662e 6765 745f 6761  es = self.get_ga
-0000e990: 705f 696e 6469 6365 7328 6d69 6e5f 6761  p_indices(min_ga
-0000e9a0: 7029 0d0a 2020 2020 2020 2020 7365 6c66  p)..        self
-0000e9b0: 2e5f 6d65 7267 655f 7365 676d 656e 7473  ._merge_segments
-0000e9c0: 2869 6e64 6963 6573 2c0d 0a20 2020 2020  (indices,..     
-0000e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9e0: 2020 2020 2020 2020 6d61 785f 776f 7264          max_word
-0000e9f0: 733d 6d61 785f 776f 7264 732c 206d 6178  s=max_words, max
-0000ea00: 5f63 6861 7273 3d6d 6178 5f63 6861 7273  _chars=max_chars
-0000ea10: 2c20 6973 5f73 756d 5f6d 6178 3d69 735f  , is_sum_max=is_
-0000ea20: 7375 6d5f 6d61 782c 206c 6f63 6b3d 6c6f  sum_max, lock=lo
-0000ea30: 636b 290d 0a20 2020 2020 2020 2069 6620  ck)..        if 
-0000ea40: 7365 6c66 2e5f 7265 6772 6f75 705f 6869  self._regroup_hi
-0000ea50: 7374 6f72 793a 0d0a 2020 2020 2020 2020  story:..        
-0000ea60: 2020 2020 7365 6c66 2e5f 7265 6772 6f75      self._regrou
-0000ea70: 705f 6869 7374 6f72 7920 2b3d 2027 5f27  p_history += '_'
-0000ea80: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-0000ea90: 7265 6772 6f75 705f 6869 7374 6f72 7920  regroup_history 
-0000eaa0: 2b3d 2066 276d 673d 7b6d 696e 5f67 6170  += f'mg={min_gap
-0000eab0: 7d2b 7b6d 6178 5f77 6f72 6473 206f 7220  }+{max_words or 
-0000eac0: 2222 7d2b 7b6d 6178 5f63 6861 7273 206f  ""}+{max_chars o
-0000ead0: 7220 2222 7d2b 7b69 6e74 2869 735f 7375  r ""}+{int(is_su
-0000eae0: 6d5f 6d61 7829 7d2b 7b69 6e74 286c 6f63  m_max)}+{int(loc
-0000eaf0: 6b29 7d27 0d0a 2020 2020 2020 2020 7265  k)}'..        re
-0000eb00: 7475 726e 2073 656c 660d 0a0d 0a20 2020  turn self....   
-0000eb10: 2064 6566 2073 706c 6974 5f62 795f 7075   def split_by_pu
-0000eb20: 6e63 7475 6174 696f 6e28 0d0a 2020 2020  nctuation(..    
-0000eb30: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-0000eb40: 2020 2020 2020 2020 2020 2070 756e 6374             punct
-0000eb50: 7561 7469 6f6e 3a20 556e 696f 6e5b 4c69  uation: Union[Li
-0000eb60: 7374 5b73 7472 5d2c 204c 6973 745b 5475  st[str], List[Tu
-0000eb70: 706c 655b 7374 722c 2073 7472 5d5d 2c20  ple[str, str]], 
-0000eb80: 7374 725d 2c0d 0a20 2020 2020 2020 2020  str],..         
-0000eb90: 2020 206c 6f63 6b3a 2062 6f6f 6c20 3d20     lock: bool = 
-0000eba0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000ebb0: 2020 2020 6e65 776c 696e 653a 2062 6f6f      newline: boo
-0000ebc0: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
-0000ebd0: 2020 2020 2020 2020 6d69 6e5f 776f 7264          min_word
-0000ebe0: 733a 204f 7074 696f 6e61 6c5b 696e 745d  s: Optional[int]
-0000ebf0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-0000ec00: 2020 2020 2020 6d69 6e5f 6368 6172 733a        min_chars:
-0000ec10: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-0000ec20: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-0000ec30: 2020 2020 6d69 6e5f 6475 723a 204f 7074      min_dur: Opt
-0000ec40: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-0000ec50: 650d 0a20 2020 2029 202d 3e20 2257 6869  e..    ) -> "Whi
-0000ec60: 7370 6572 5265 7375 6c74 223a 0d0a 2020  sperResult":..  
-0000ec70: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-0000ec80: 2020 2053 706c 6974 2028 696e 2d70 6c61     Split (in-pla
-0000ec90: 6365 2920 7365 676d 656e 7473 2061 7420  ce) segments at 
-0000eca0: 776f 7264 7320 7468 6174 2073 7461 7274  words that start
-0000ecb0: 2f65 6e64 2077 6974 6820 6060 7075 6e63  /end with ``punc
-0000ecc0: 7475 6174 696f 6e60 602e 0d0a 0d0a 2020  tuation``.....  
-0000ecd0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0000ece0: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-0000ecf0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7075  ----..        pu
-0000ed00: 6e63 7475 6174 696f 6e20 3a20 6c69 7374  nctuation : list
-0000ed10: 206f 6620 7374 7220 6f66 206c 6973 7420   of str of list 
-0000ed20: 6f66 2074 7570 6c65 206f 6620 2873 7472  of tuple of (str
-0000ed30: 2c20 7374 7229 206f 7220 7374 720d 0a20  , str) or str.. 
-0000ed40: 2020 2020 2020 2020 2020 2050 756e 6374             Punct
-0000ed50: 7561 7469 6f6e 2873 2920 746f 2073 706c  uation(s) to spl
-0000ed60: 6974 2073 6567 6d65 6e74 7320 6279 2e0d  it segments by..
-0000ed70: 0a20 2020 2020 2020 206c 6f63 6b20 3a20  .        lock : 
-0000ed80: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-0000ed90: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-0000eda0: 2057 6865 7468 6572 2074 6f20 7072 6576   Whether to prev
-0000edb0: 656e 7420 6675 7475 7265 2073 706c 6974  ent future split
-0000edc0: 732f 6d65 7267 6573 2066 726f 6d20 616c  s/merges from al
-0000edd0: 7465 7269 6e67 2063 6861 6e67 6573 206d  tering changes m
-0000ede0: 6164 6520 6279 2074 6869 7320 6d65 7468  ade by this meth
-0000edf0: 6f64 2e0d 0a20 2020 2020 2020 206e 6577  od...        new
-0000ee00: 6c69 6e65 203a 2062 6f6f 6c2c 2064 6566  line : bool, def
-0000ee10: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
-0000ee20: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-0000ee30: 746f 2069 6e73 6572 7420 6c69 6e65 2062  to insert line b
-0000ee40: 7265 616b 2061 7420 7468 6520 7370 6c69  reak at the spli
-0000ee50: 7420 706f 696e 7473 2069 6e73 7465 6164  t points instead
-0000ee60: 206f 6620 7370 6c69 7474 696e 6720 696e   of splitting in
-0000ee70: 746f 2073 6570 6172 6174 6520 7365 676d  to separate segm
-0000ee80: 656e 7473 2e0d 0a20 2020 2020 2020 206d  ents...        m
-0000ee90: 696e 5f77 6f72 6473 203a 2069 6e74 2c20  in_words : int, 
-0000eea0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-0000eeb0: 2020 2020 2020 5370 6c69 7420 7365 676d        Split segm
-0000eec0: 656e 7473 2077 6974 6820 776f 7264 7320  ents with words 
-0000eed0: 3e3d 2060 606d 696e 5f77 6f72 6473 6060  >= ``min_words``
-0000eee0: 2e0d 0a20 2020 2020 2020 206d 696e 5f63  ...        min_c
-0000eef0: 6861 7273 203a 2069 6e74 2c20 6f70 7469  hars : int, opti
-0000ef00: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
-0000ef10: 2020 5370 6c69 7420 7365 676d 656e 7473    Split segments
-0000ef20: 2077 6974 6820 6368 6172 6163 7465 7273   with characters
-0000ef30: 203e 3d20 6060 6d69 6e5f 6368 6172 7360   >= ``min_chars`
-0000ef40: 602e 0d0a 2020 2020 2020 2020 6d69 6e5f  `...        min_
-0000ef50: 6475 7220 3a20 696e 742c 206f 7074 696f  dur : int, optio
-0000ef60: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
-0000ef70: 2073 706c 6974 2073 6567 6d65 6e74 7320   split segments 
-0000ef80: 7769 7468 2064 7572 6174 696f 6e20 2869  with duration (i
-0000ef90: 6e20 7365 636f 6e64 7329 203e 3d20 6060  n seconds) >= ``
-0000efa0: 6d69 6e5f 6475 7260 602e 0d0a 0d0a 2020  min_dur``.....  
-0000efb0: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
-0000efc0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
-0000efd0: 2020 2020 2020 2020 7374 6162 6c65 5f77          stable_w
-0000efe0: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
-0000eff0: 6973 7065 7252 6573 756c 740d 0a20 2020  isperResult..   
-0000f000: 2020 2020 2020 2020 2054 6865 2063 7572           The cur
-0000f010: 7265 6e74 2069 6e73 7461 6e63 6520 6166  rent instance af
-0000f020: 7465 7220 7468 6520 6368 616e 6765 732e  ter the changes.
-0000f030: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-0000f040: 2020 2020 2020 2064 6566 205f 6f76 6572         def _over
-0000f050: 5f6d 6178 2878 3a20 5365 676d 656e 7429  _max(x: Segment)
-0000f060: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0000f070: 6574 7572 6e20 280d 0a20 2020 2020 2020  eturn (..       
-0000f080: 2020 2020 2020 2020 2020 2020 2028 6d69               (mi
-0000f090: 6e5f 776f 7264 7320 616e 6420 6c65 6e28  n_words and len(
-0000f0a0: 782e 776f 7264 7329 203e 3d20 6d69 6e5f  x.words) >= min_
-0000f0b0: 776f 7264 7329 206f 720d 0a20 2020 2020  words) or..     
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0000f0d0: 6d69 6e5f 6368 6172 7320 616e 6420 782e  min_chars and x.
-0000f0e0: 6368 6172 5f63 6f75 6e74 2829 203e 3d20  char_count() >= 
-0000f0f0: 6d69 6e5f 6368 6172 7329 206f 720d 0a20  min_chars) or.. 
-0000f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f110: 2020 2028 6d69 6e5f 6475 7220 616e 6420     (min_dur and 
-0000f120: 782e 6475 7261 7469 6f6e 203e 3d20 6d69  x.duration >= mi
-0000f130: 6e5f 6475 7229 0d0a 2020 2020 2020 2020  n_dur)..        
-0000f140: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
-0000f150: 2069 6e64 6963 6573 203d 2073 6574 2873   indices = set(s
-0000f160: 2e69 6420 666f 7220 7320 696e 2073 656c  .id for s in sel
-0000f170: 662e 7365 676d 656e 7473 2069 6620 5f6f  f.segments if _o
-0000f180: 7665 725f 6d61 7828 7329 2920 6966 2061  ver_max(s)) if a
-0000f190: 6e79 2828 6d69 6e5f 776f 7264 732c 206d  ny((min_words, m
-0000f1a0: 696e 5f63 6861 7273 2c20 6d69 6e5f 6475  in_chars, min_du
-0000f1b0: 7229 2920 656c 7365 204e 6f6e 650d 0a0d  r)) else None...
-0000f1c0: 0a20 2020 2020 2020 2064 6566 205f 6765  .        def _ge
-0000f1d0: 745f 696e 6469 6365 7328 783a 2053 6567  t_indices(x: Seg
-0000f1e0: 6d65 6e74 293a 0d0a 2020 2020 2020 2020  ment):..        
-0000f1f0: 2020 2020 7265 7475 726e 2078 2e67 6574      return x.get
-0000f200: 5f70 756e 6374 7561 7469 6f6e 5f69 6e64  _punctuation_ind
-0000f210: 6963 6573 2870 756e 6374 7561 7469 6f6e  ices(punctuation
-0000f220: 2920 6966 2069 6e64 6963 6573 2069 7320  ) if indices is 
-0000f230: 4e6f 6e65 206f 7220 782e 6964 2069 6e20  None or x.id in 
-0000f240: 696e 6469 6365 7320 656c 7365 205b 5d0d  indices else [].
-0000f250: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-0000f260: 5f73 706c 6974 5f73 6567 6d65 6e74 7328  _split_segments(
-0000f270: 5f67 6574 5f69 6e64 6963 6573 2c20 6c6f  _get_indices, lo
-0000f280: 636b 3d6c 6f63 6b2c 206e 6577 6c69 6e65  ck=lock, newline
-0000f290: 3d6e 6577 6c69 6e65 290d 0a20 2020 2020  =newline)..     
-0000f2a0: 2020 2069 6620 7365 6c66 2e5f 7265 6772     if self._regr
-0000f2b0: 6f75 705f 6869 7374 6f72 793a 0d0a 2020  oup_history:..  
-0000f2c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000f2d0: 7265 6772 6f75 705f 6869 7374 6f72 7920  regroup_history 
-0000f2e0: 2b3d 2027 5f27 0d0a 2020 2020 2020 2020  += '_'..        
-0000f2f0: 7075 6e63 745f 7374 7220 3d20 272f 272e  punct_str = '/'.
-0000f300: 6a6f 696e 2870 2069 6620 6973 696e 7374  join(p if isinst
-0000f310: 616e 6365 2870 2c20 7374 7229 2065 6c73  ance(p, str) els
-0000f320: 6520 272a 272e 6a6f 696e 2870 2920 666f  e '*'.join(p) fo
-0000f330: 7220 7020 696e 2070 756e 6374 7561 7469  r p in punctuati
-0000f340: 6f6e 290d 0a20 2020 2020 2020 2073 656c  on)..        sel
-0000f350: 662e 5f72 6567 726f 7570 5f68 6973 746f  f._regroup_histo
-0000f360: 7279 202b 3d20 6627 7370 3d7b 7075 6e63  ry += f'sp={punc
-0000f370: 745f 7374 727d 2b7b 696e 7428 6c6f 636b  t_str}+{int(lock
-0000f380: 297d 2b7b 696e 7428 6e65 776c 696e 6529  )}+{int(newline)
-0000f390: 7d27 0d0a 2020 2020 2020 2020 7365 6c66  }'..        self
-0000f3a0: 2e5f 7265 6772 6f75 705f 6869 7374 6f72  ._regroup_histor
-0000f3b0: 7920 2b3d 2066 272b 7b6d 696e 5f77 6f72  y += f'+{min_wor
-0000f3c0: 6473 206f 7220 2222 7d2b 7b6d 696e 5f63  ds or ""}+{min_c
-0000f3d0: 6861 7273 206f 7220 2222 7d2b 7b6d 696e  hars or ""}+{min
-0000f3e0: 5f64 7572 206f 7220 2222 7d27 2e72 7374  _dur or ""}'.rst
-0000f3f0: 7269 7028 272b 2729 0d0a 2020 2020 2020  rip('+')..      
-0000f400: 2020 7265 7475 726e 2073 656c 660d 0a0d    return self...
-0000f410: 0a20 2020 2064 6566 206d 6572 6765 5f62  .    def merge_b
-0000f420: 795f 7075 6e63 7475 6174 696f 6e28 0d0a  y_punctuation(..
-0000f430: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f440: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
-0000f450: 756e 6374 7561 7469 6f6e 3a20 556e 696f  unctuation: Unio
-0000f460: 6e5b 4c69 7374 5b73 7472 5d2c 204c 6973  n[List[str], Lis
-0000f470: 745b 5475 706c 655b 7374 722c 2073 7472  t[Tuple[str, str
-0000f480: 5d5d 2c20 7374 725d 2c0d 0a20 2020 2020  ]], str],..     
-0000f490: 2020 2020 2020 206d 6178 5f77 6f72 6473         max_words
-0000f4a0: 3a20 696e 7420 3d20 4e6f 6e65 2c0d 0a20  : int = None,.. 
-0000f4b0: 2020 2020 2020 2020 2020 206d 6178 5f63             max_c
-0000f4c0: 6861 7273 3a20 696e 7420 3d20 4e6f 6e65  hars: int = None
-0000f4d0: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
-0000f4e0: 735f 7375 6d5f 6d61 783a 2062 6f6f 6c20  s_sum_max: bool 
-0000f4f0: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
-0000f500: 2020 2020 2020 6c6f 636b 3a20 626f 6f6c        lock: bool
-0000f510: 203d 2046 616c 7365 0d0a 2020 2020 2920   = False..    ) 
-0000f520: 2d3e 2022 5768 6973 7065 7252 6573 756c  -> "WhisperResul
-0000f530: 7422 3a0d 0a20 2020 2020 2020 2022 2222  t":..        """
-0000f540: 0d0a 2020 2020 2020 2020 4d65 7267 6520  ..        Merge 
-0000f550: 2869 6e2d 706c 6163 6529 2061 6e79 2074  (in-place) any t
-0000f560: 776f 2073 6567 6d65 6e74 7320 7468 6174  wo segments that
-0000f570: 2068 6173 2073 7065 6369 6669 6320 7075   has specific pu
-0000f580: 6e63 7475 6174 696f 6e73 2069 6e62 6574  nctuations inbet
-0000f590: 7765 656e 2e0d 0a0d 0a20 2020 2020 2020  ween.....       
-0000f5a0: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
-0000f5b0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
-0000f5c0: 0a20 2020 2020 2020 2070 756e 6374 7561  .        punctua
-0000f5d0: 7469 6f6e 203a 206c 6973 7420 6f66 2073  tion : list of s
-0000f5e0: 7472 206f 6620 6c69 7374 206f 6620 7475  tr of list of tu
-0000f5f0: 706c 6520 6f66 2028 7374 722c 2073 7472  ple of (str, str
-0000f600: 2920 6f72 2073 7472 0d0a 2020 2020 2020  ) or str..      
-0000f610: 2020 2020 2020 5075 6e63 7475 6174 696f        Punctuatio
-0000f620: 6e28 7329 2074 6f20 6d65 7267 6520 7365  n(s) to merge se
-0000f630: 676d 656e 7473 2062 792e 0d0a 2020 2020  gments by...    
-0000f640: 2020 2020 6d61 785f 776f 7264 7320 3a20      max_words : 
-0000f650: 696e 742c 206f 7074 696f 6e61 6c0d 0a20  int, optional.. 
-0000f660: 2020 2020 2020 2020 2020 204d 6178 696d             Maxim
-0000f670: 756d 206e 756d 6265 7220 6f66 2077 6f72  um number of wor
-0000f680: 6473 2061 6c6c 6f77 6564 2069 6e20 6561  ds allowed in ea
-0000f690: 6368 2073 6567 6d65 6e74 2e0d 0a20 2020  ch segment...   
-0000f6a0: 2020 2020 206d 6178 5f63 6861 7273 203a       max_chars :
-0000f6b0: 2069 6e74 2c20 6f70 7469 6f6e 616c 0d0a   int, optional..
-0000f6c0: 2020 2020 2020 2020 2020 2020 4d61 7869              Maxi
-0000f6d0: 6d75 6d20 6e75 6d62 6572 206f 6620 6368  mum number of ch
-0000f6e0: 6172 6163 7465 7273 2061 6c6c 6f77 6564  aracters allowed
-0000f6f0: 2069 6e20 6561 6368 2073 6567 6d65 6e74   in each segment
-0000f700: 2e0d 0a20 2020 2020 2020 2069 735f 7375  ...        is_su
-0000f710: 6d5f 6d61 7820 3a20 626f 6f6c 2c20 6465  m_max : bool, de
-0000f720: 6661 756c 7420 4661 6c73 650d 0a20 2020  fault False..   
-0000f730: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
-0000f740: 2060 606d 6178 5f77 6f72 6473 6060 2061   ``max_words`` a
-0000f750: 6e64 2060 606d 6178 5f63 6861 7273 6060  nd ``max_chars``
-0000f760: 2069 7320 6170 706c 6965 6420 746f 2074   is applied to t
-0000f770: 6865 206d 6572 6765 6420 7365 676d 656e  he merged segmen
-0000f780: 7420 696e 7374 6561 6420 6f66 2074 6865  t instead of the
-0000f790: 2069 6e64 6976 6964 7561 6c20 7365 676d   individual segm
-0000f7a0: 656e 7473 0d0a 2020 2020 2020 2020 2020  ents..          
-0000f7b0: 2020 746f 2062 6520 6d65 7267 6564 2e0d    to be merged..
-0000f7c0: 0a20 2020 2020 2020 206c 6f63 6b20 3a20  .        lock : 
-0000f7d0: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-0000f7e0: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-0000f7f0: 2057 6865 7468 6572 2074 6f20 7072 6576   Whether to prev
-0000f800: 656e 7420 6675 7475 7265 2073 706c 6974  ent future split
-0000f810: 732f 6d65 7267 6573 2066 726f 6d20 616c  s/merges from al
-0000f820: 7465 7269 6e67 2063 6861 6e67 6573 206d  tering changes m
-0000f830: 6164 6520 6279 2074 6869 7320 6d65 7468  ade by this meth
-0000f840: 6f64 2e0d 0a0d 0a20 2020 2020 2020 2052  od.....        R
-0000f850: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
-0000f860: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-0000f870: 2073 7461 626c 655f 7768 6973 7065 722e   stable_whisper.
-0000f880: 7265 7375 6c74 2e57 6869 7370 6572 5265  result.WhisperRe
-0000f890: 7375 6c74 0d0a 2020 2020 2020 2020 2020  sult..          
-0000f8a0: 2020 5468 6520 6375 7272 656e 7420 696e    The current in
-0000f8b0: 7374 616e 6365 2061 6674 6572 2074 6865  stance after the
-0000f8c0: 2063 6861 6e67 6573 2e0d 0a20 2020 2020   changes...     
-0000f8d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-0000f8e0: 696e 6469 6365 7320 3d20 7365 6c66 2e67  indices = self.g
-0000f8f0: 6574 5f70 756e 6374 7561 7469 6f6e 5f69  et_punctuation_i
-0000f900: 6e64 6963 6573 2870 756e 6374 7561 7469  ndices(punctuati
-0000f910: 6f6e 290d 0a20 2020 2020 2020 2073 656c  on)..        sel
-0000f920: 662e 5f6d 6572 6765 5f73 6567 6d65 6e74  f._merge_segment
-0000f930: 7328 696e 6469 6365 732c 0d0a 2020 2020  s(indices,..    
-0000f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f950: 2020 2020 2020 2020 206d 6178 5f77 6f72           max_wor
-0000f960: 6473 3d6d 6178 5f77 6f72 6473 2c20 6d61  ds=max_words, ma
-0000f970: 785f 6368 6172 733d 6d61 785f 6368 6172  x_chars=max_char
-0000f980: 732c 2069 735f 7375 6d5f 6d61 783d 6973  s, is_sum_max=is
-0000f990: 5f73 756d 5f6d 6178 2c20 6c6f 636b 3d6c  _sum_max, lock=l
-0000f9a0: 6f63 6b29 0d0a 2020 2020 2020 2020 6966  ock)..        if
-0000f9b0: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
-0000f9c0: 6973 746f 7279 3a0d 0a20 2020 2020 2020  istory:..       
-0000f9d0: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
-0000f9e0: 7570 5f68 6973 746f 7279 202b 3d20 275f  up_history += '_
-0000f9f0: 270d 0a20 2020 2020 2020 2070 756e 6374  '..        punct
-0000fa00: 5f73 7472 203d 2027 2f27 2e6a 6f69 6e28  _str = '/'.join(
-0000fa10: 7020 6966 2069 7369 6e73 7461 6e63 6528  p if isinstance(
-0000fa20: 702c 2073 7472 2920 656c 7365 2027 2a27  p, str) else '*'
-0000fa30: 2e6a 6f69 6e28 7029 2066 6f72 2070 2069  .join(p) for p i
-0000fa40: 6e20 7075 6e63 7475 6174 696f 6e29 0d0a  n punctuation)..
-0000fa50: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
-0000fa60: 6772 6f75 705f 6869 7374 6f72 7920 2b3d  group_history +=
-0000fa70: 2066 276d 703d 7b70 756e 6374 5f73 7472   f'mp={punct_str
-0000fa80: 7d2b 7b6d 6178 5f77 6f72 6473 206f 7220  }+{max_words or 
-0000fa90: 2222 7d2b 7b6d 6178 5f63 6861 7273 206f  ""}+{max_chars o
-0000faa0: 7220 2222 7d2b 7b69 6e74 2869 735f 7375  r ""}+{int(is_su
-0000fab0: 6d5f 6d61 7829 7d2b 7b69 6e74 286c 6f63  m_max)}+{int(loc
-0000fac0: 6b29 7d27 0d0a 2020 2020 2020 2020 7265  k)}'..        re
-0000fad0: 7475 726e 2073 656c 660d 0a0d 0a20 2020  turn self....   
-0000fae0: 2064 6566 206d 6572 6765 5f61 6c6c 5f73   def merge_all_s
-0000faf0: 6567 6d65 6e74 7328 7365 6c66 2920 2d3e  egments(self) ->
-0000fb00: 2022 5768 6973 7065 7252 6573 756c 7422   "WhisperResult"
-0000fb10: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-0000fb20: 2020 2020 2020 2020 4d65 7267 6520 616c          Merge al
-0000fb30: 6c20 7365 676d 656e 7473 2069 6e74 6f20  l segments into 
-0000fb40: 6f6e 6520 7365 676d 656e 742e 0d0a 0d0a  one segment.....
-0000fb50: 2020 2020 2020 2020 5265 7475 726e 730d          Returns.
-0000fb60: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000fb70: 0d0a 2020 2020 2020 2020 7374 6162 6c65  ..        stable
-0000fb80: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
-0000fb90: 5768 6973 7065 7252 6573 756c 740d 0a20  WhisperResult.. 
-0000fba0: 2020 2020 2020 2020 2020 2054 6865 2063             The c
-0000fbb0: 7572 7265 6e74 2069 6e73 7461 6e63 6520  urrent instance 
-0000fbc0: 6166 7465 7220 7468 6520 6368 616e 6765  after the change
-0000fbd0: 732e 0d0a 2020 2020 2020 2020 2222 220d  s...        """.
-0000fbe0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000fbf0: 7365 6c66 2e73 6567 6d65 6e74 733a 0d0a  self.segments:..
-0000fc00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000fc10: 726e 2073 656c 660d 0a20 2020 2020 2020  rn self..       
-0000fc20: 2069 6620 7365 6c66 2e68 6173 5f77 6f72   if self.has_wor
-0000fc30: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-0000fc40: 206e 6577 5f73 6567 203d 2073 656c 662e   new_seg = self.
-0000fc50: 7365 676d 656e 7473 5b30 5d2e 636f 7079  segments[0].copy
-0000fc60: 2873 656c 662e 616c 6c5f 776f 7264 7328  (self.all_words(
-0000fc70: 292c 206b 6565 705f 7265 7375 6c74 3d54  ), keep_result=T
-0000fc80: 7275 652c 2063 6f70 795f 776f 7264 733d  rue, copy_words=
-0000fc90: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
-0000fca0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0000fcb0: 2020 206e 6577 5f73 6567 203d 2073 656c     new_seg = sel
-0000fcc0: 662e 7365 676d 656e 7473 5b30 5d0d 0a20  f.segments[0].. 
-0000fcd0: 2020 2020 2020 2020 2020 206e 6577 5f73             new_s
-0000fce0: 6567 2e5f 6465 6661 756c 745f 7465 7874  eg._default_text
-0000fcf0: 202b 3d20 2727 2e6a 6f69 6e28 732e 7465   += ''.join(s.te
-0000fd00: 7874 2066 6f72 2073 2069 6e20 7365 6c66  xt for s in self
-0000fd10: 2e73 6567 6d65 6e74 735b 313a 5d29 0d0a  .segments[1:])..
-0000fd20: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-0000fd30: 6c6c 2873 2e74 6f6b 656e 7320 6973 206e  ll(s.tokens is n
-0000fd40: 6f74 204e 6f6e 6520 666f 7220 7320 696e  ot None for s in
-0000fd50: 2073 656c 662e 7365 676d 656e 7473 293a   self.segments):
-0000fd60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fd70: 2020 6e65 775f 7365 672e 5f64 6566 6175    new_seg._defau
-0000fd80: 6c74 5f74 6f6b 656e 7320 2b3d 206c 6973  lt_tokens += lis
-0000fd90: 7428 6368 6169 6e2e 6672 6f6d 5f69 7465  t(chain.from_ite
-0000fda0: 7261 626c 6528 732e 746f 6b65 6e73 2066  rable(s.tokens f
-0000fdb0: 6f72 2073 2069 6e20 7365 6c66 2e73 6567  or s in self.seg
-0000fdc0: 6d65 6e74 735b 313a 5d29 290d 0a20 2020  ments[1:]))..   
-0000fdd0: 2020 2020 2020 2020 206e 6577 5f73 6567           new_seg
-0000fde0: 2e65 6e64 203d 2073 656c 662e 7365 676d  .end = self.segm
-0000fdf0: 656e 7473 5b2d 315d 2e65 6e64 0d0a 2020  ents[-1].end..  
-0000fe00: 2020 2020 2020 7365 6c66 2e73 6567 6d65        self.segme
-0000fe10: 6e74 7320 3d20 5b6e 6577 5f73 6567 5d0d  nts = [new_seg].
-0000fe20: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-0000fe30: 6173 7369 676e 5f69 6473 2829 0d0a 2020  assign_ids()..  
-0000fe40: 2020 2020 2020 6966 2073 656c 662e 5f72        if self._r
-0000fe50: 6567 726f 7570 5f68 6973 746f 7279 3a0d  egroup_history:.
-0000fe60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000fe70: 662e 5f72 6567 726f 7570 5f68 6973 746f  f._regroup_histo
-0000fe80: 7279 202b 3d20 275f 270d 0a20 2020 2020  ry += '_'..     
-0000fe90: 2020 2073 656c 662e 5f72 6567 726f 7570     self._regroup
-0000fea0: 5f68 6973 746f 7279 202b 3d20 276d 7327  _history += 'ms'
-0000feb0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000fec0: 2073 656c 660d 0a0d 0a20 2020 2064 6566   self....    def
-0000fed0: 2073 706c 6974 5f62 795f 6c65 6e67 7468   split_by_length
-0000fee0: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
-0000fef0: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
-0000ff00: 2020 6d61 785f 6368 6172 733a 2069 6e74    max_chars: int
-0000ff10: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-0000ff20: 2020 2020 2020 6d61 785f 776f 7264 733a        max_words:
-0000ff30: 2069 6e74 203d 204e 6f6e 652c 0d0a 2020   int = None,..  
-0000ff40: 2020 2020 2020 2020 2020 6576 656e 5f73            even_s
-0000ff50: 706c 6974 3a20 626f 6f6c 203d 2054 7275  plit: bool = Tru
-0000ff60: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000ff70: 666f 7263 655f 6c65 6e3a 2062 6f6f 6c20  force_len: bool 
-0000ff80: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
-0000ff90: 2020 2020 2020 6c6f 636b 3a20 626f 6f6c        lock: bool
-0000ffa0: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
-0000ffb0: 2020 2020 2020 2069 6e63 6c75 6465 5f6c         include_l
-0000ffc0: 6f63 6b3a 2062 6f6f 6c20 3d20 4661 6c73  ock: bool = Fals
-0000ffd0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000ffe0: 6e65 776c 696e 653a 2062 6f6f 6c20 3d20  newline: bool = 
-0000fff0: 4661 6c73 650d 0a20 2020 2029 202d 3e20  False..    ) -> 
-00010000: 2257 6869 7370 6572 5265 7375 6c74 223a  "WhisperResult":
-00010010: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00010020: 2020 2020 2020 2053 706c 6974 2028 696e         Split (in
-00010030: 2d70 6c61 6365 2920 616e 7920 7365 676d  -place) any segm
-00010040: 656e 7420 7468 6174 2065 7863 6565 6473  ent that exceeds
-00010050: 2060 606d 6178 5f63 6861 7273 6060 206f   ``max_chars`` o
-00010060: 7220 6060 6d61 785f 776f 7264 7360 6020  r ``max_words`` 
-00010070: 696e 746f 2073 6d61 6c6c 6572 2073 6567  into smaller seg
-00010080: 6d65 6e74 732e 0d0a 0d0a 2020 2020 2020  ments.....      
-00010090: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
-000100a0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-000100b0: 0d0a 2020 2020 2020 2020 6d61 785f 6368  ..        max_ch
-000100c0: 6172 7320 3a20 696e 742c 206f 7074 696f  ars : int, optio
-000100d0: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
-000100e0: 204d 6178 696d 756d 206e 756d 6265 7220   Maximum number 
-000100f0: 6f66 2063 6861 7261 6374 6572 7320 616c  of characters al
-00010100: 6c6f 7765 6420 696e 2065 6163 6820 7365  lowed in each se
-00010110: 676d 656e 742e 0d0a 2020 2020 2020 2020  gment...        
-00010120: 6d61 785f 776f 7264 7320 3a20 696e 742c  max_words : int,
-00010130: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-00010140: 2020 2020 2020 204d 6178 696d 756d 206e         Maximum n
-00010150: 756d 6265 7220 6f66 2077 6f72 6473 2061  umber of words a
-00010160: 6c6c 6f77 6564 2069 6e20 6561 6368 2073  llowed in each s
-00010170: 6567 6d65 6e74 2e0d 0a20 2020 2020 2020  egment...       
-00010180: 2065 7665 6e5f 7370 6c69 7420 3a20 626f   even_split : bo
-00010190: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
-000101a0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-000101b0: 6574 6865 7220 746f 2065 7665 6e6c 7920  ether to evenly 
-000101c0: 7370 6c69 7420 6120 7365 676d 656e 7420  split a segment 
-000101d0: 696e 206c 656e 6774 6820 6966 2069 7420  in length if it 
-000101e0: 6578 6365 6564 7320 6060 6d61 785f 6368  exceeds ``max_ch
-000101f0: 6172 7360 6020 6f72 2060 606d 6178 5f77  ars`` or ``max_w
-00010200: 6f72 6473 6060 2e0d 0a20 2020 2020 2020  ords``...       
-00010210: 2066 6f72 6365 5f6c 656e 203a 2062 6f6f   force_len : boo
-00010220: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-00010230: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-00010240: 6574 6865 7220 746f 2066 6f72 6365 2061  ether to force a
-00010250: 2063 6f6e 7374 616e 7420 6c65 6e67 7468   constant length
-00010260: 2066 6f72 2065 6163 6820 7365 676d 656e   for each segmen
-00010270: 7420 6578 6365 7074 2074 6865 206c 6173  t except the las
-00010280: 7420 7365 676d 656e 742e 0d0a 2020 2020  t segment...    
-00010290: 2020 2020 2020 2020 5468 6973 2077 696c          This wil
-000102a0: 6c20 6967 6e6f 7265 2061 6c6c 2070 7265  l ignore all pre
-000102b0: 7669 6f75 7320 6e6f 6e2d 6c6f 636b 6564  vious non-locked
-000102c0: 2073 6567 6d65 6e74 2062 6f75 6e64 6172   segment boundar
-000102d0: 6965 732e 0d0a 2020 2020 2020 2020 6c6f  ies...        lo
-000102e0: 636b 203a 2062 6f6f 6c2c 2064 6566 6175  ck : bool, defau
-000102f0: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
-00010300: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-00010310: 2070 7265 7665 6e74 2066 7574 7572 6520   prevent future 
-00010320: 7370 6c69 7473 2f6d 6572 6765 7320 6672  splits/merges fr
-00010330: 6f6d 2061 6c74 6572 696e 6720 6368 616e  om altering chan
-00010340: 6765 7320 6d61 6465 2062 7920 7468 6973  ges made by this
-00010350: 206d 6574 686f 642e 0d0a 2020 2020 2020   method...      
-00010360: 2020 696e 636c 7564 655f 6c6f 636b 3a20    include_lock: 
-00010370: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-00010380: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-00010390: 2057 6865 7468 6572 2074 6f20 696e 636c   Whether to incl
-000103a0: 7564 6520 7072 6576 696f 7573 206c 6f63  ude previous loc
-000103b0: 6b20 6265 666f 7265 2073 706c 6974 7469  k before splitti
-000103c0: 6e67 2062 6173 6564 206f 6e20 6d61 785f  ng based on max_
-000103d0: 776f 7264 732c 2069 6620 6060 6576 656e  words, if ``even
-000103e0: 5f73 706c 6974 203d 2046 616c 7365 6060  _split = False``
-000103f0: 2e0d 0a20 2020 2020 2020 2020 2020 2053  ...            S
-00010400: 706c 6974 7469 6e67 2077 696c 6c20 6265  plitting will be
-00010410: 2064 6f6e 6520 6166 7465 7220 7468 6520   done after the 
-00010420: 6669 7273 7420 6e6f 6e2d 6c6f 636b 6564  first non-locked
-00010430: 2077 6f72 6420 3e20 6060 6d61 785f 6368   word > ``max_ch
-00010440: 6172 7360 6020 2f20 6060 6d61 785f 776f  ars`` / ``max_wo
-00010450: 7264 7360 602e 0d0a 2020 2020 2020 2020  rds``...        
-00010460: 6e65 776c 696e 653a 2062 6f6f 6c2c 2064  newline: bool, d
-00010470: 6566 6175 6c74 2046 616c 7365 0d0a 2020  efault False..  
-00010480: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
-00010490: 7220 746f 2069 6e73 6572 7420 6c69 6e65  r to insert line
-000104a0: 2062 7265 616b 2061 7420 7468 6520 7370   break at the sp
-000104b0: 6c69 7420 706f 696e 7473 2069 6e73 7465  lit points inste
-000104c0: 6164 206f 6620 7370 6c69 7474 696e 6720  ad of splitting 
-000104d0: 696e 746f 2073 6570 6172 6174 6520 7365  into separate se
-000104e0: 676d 656e 7473 2e0d 0a0d 0a20 2020 2020  gments.....     
-000104f0: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-00010500: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-00010510: 2020 2020 2073 7461 626c 655f 7768 6973       stable_whis
-00010520: 7065 722e 7265 7375 6c74 2e57 6869 7370  per.result.Whisp
-00010530: 6572 5265 7375 6c74 0d0a 2020 2020 2020  erResult..      
-00010540: 2020 2020 2020 5468 6520 6375 7272 656e        The curren
-00010550: 7420 696e 7374 616e 6365 2061 6674 6572  t instance after
-00010560: 2074 6865 2063 6861 6e67 6573 2e0d 0a0d   the changes....
-00010570: 0a20 2020 2020 2020 204e 6f74 6573 0d0a  .        Notes..
-00010580: 2020 2020 2020 2020 2d2d 2d2d 2d0d 0a20          -----.. 
-00010590: 2020 2020 2020 2049 6620 6060 6576 656e         If ``even
-000105a0: 5f73 706c 6974 203d 2054 7275 6560 602c  _split = True``,
-000105b0: 2073 6567 6d65 6e74 7320 6361 6e20 7374   segments can st
-000105c0: 696c 6c20 6578 6365 6564 2060 606d 6178  ill exceed ``max
-000105d0: 5f63 6861 7273 6060 2061 6e64 206c 6f63  _chars`` and loc
-000105e0: 6b65 6420 776f 7264 7320 7769 6c6c 2062  ked words will b
-000105f0: 6520 6967 6e6f 7265 6420 746f 2061 766f  e ignored to avo
-00010600: 6964 0d0a 2020 2020 2020 2020 756e 6576  id..        unev
-00010610: 656e 2073 706c 6974 7469 6e67 2e0d 0a20  en splitting... 
-00010620: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00010630: 2020 2020 6966 2066 6f72 6365 5f6c 656e      if force_len
-00010640: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00010650: 656c 662e 6d65 7267 655f 616c 6c5f 7365  elf.merge_all_se
-00010660: 676d 656e 7473 2829 0d0a 2020 2020 2020  gments()..      
-00010670: 2020 7365 6c66 2e5f 7370 6c69 745f 7365    self._split_se
-00010680: 676d 656e 7473 280d 0a20 2020 2020 2020  gments(..       
-00010690: 2020 2020 206c 616d 6264 6120 783a 2078       lambda x: x
-000106a0: 2e67 6574 5f6c 656e 6774 685f 696e 6469  .get_length_indi
-000106b0: 6365 7328 0d0a 2020 2020 2020 2020 2020  ces(..          
-000106c0: 2020 2020 2020 6d61 785f 6368 6172 733d        max_chars=
-000106d0: 6d61 785f 6368 6172 732c 0d0a 2020 2020  max_chars,..    
-000106e0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-000106f0: 776f 7264 733d 6d61 785f 776f 7264 732c  words=max_words,
-00010700: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010710: 2020 6576 656e 5f73 706c 6974 3d65 7665    even_split=eve
-00010720: 6e5f 7370 6c69 742c 0d0a 2020 2020 2020  n_split,..      
-00010730: 2020 2020 2020 2020 2020 696e 636c 7564            includ
-00010740: 655f 6c6f 636b 3d69 6e63 6c75 6465 5f6c  e_lock=include_l
-00010750: 6f63 6b0d 0a20 2020 2020 2020 2020 2020  ock..           
-00010760: 2029 2c0d 0a20 2020 2020 2020 2020 2020   ),..           
-00010770: 206c 6f63 6b3d 6c6f 636b 2c0d 0a20 2020   lock=lock,..   
-00010780: 2020 2020 2020 2020 206e 6577 6c69 6e65           newline
-00010790: 3d6e 6577 6c69 6e65 0d0a 2020 2020 2020  =newline..      
-000107a0: 2020 290d 0a20 2020 2020 2020 2069 6620    )..        if 
-000107b0: 7365 6c66 2e5f 7265 6772 6f75 705f 6869  self._regroup_hi
-000107c0: 7374 6f72 793a 0d0a 2020 2020 2020 2020  story:..        
-000107d0: 2020 2020 7365 6c66 2e5f 7265 6772 6f75      self._regrou
-000107e0: 705f 6869 7374 6f72 7920 2b3d 2027 5f27  p_history += '_'
-000107f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00010800: 7265 6772 6f75 705f 6869 7374 6f72 7920  regroup_history 
-00010810: 2b3d 2028 6627 736c 3d7b 6d61 785f 6368  += (f'sl={max_ch
-00010820: 6172 7320 6f72 2022 227d 2b7b 6d61 785f  ars or ""}+{max_
-00010830: 776f 7264 7320 6f72 2022 227d 2b7b 696e  words or ""}+{in
-00010840: 7428 6576 656e 5f73 706c 6974 297d 2b7b  t(even_split)}+{
-00010850: 696e 7428 666f 7263 655f 6c65 6e29 7d27  int(force_len)}'
-00010860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010880: 2020 2020 6627 2b7b 696e 7428 6c6f 636b      f'+{int(lock
-00010890: 297d 2b7b 696e 7428 696e 636c 7564 655f  )}+{int(include_
-000108a0: 6c6f 636b 297d 2b7b 696e 7428 6e65 776c  lock)}+{int(newl
-000108b0: 696e 6529 7d27 290d 0a20 2020 2020 2020  ine)}')..       
-000108c0: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
-000108d0: 2020 2020 6465 6620 7370 6c69 745f 6279      def split_by
-000108e0: 5f64 7572 6174 696f 6e28 0d0a 2020 2020  _duration(..    
-000108f0: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-00010900: 2020 2020 2020 2020 2020 206d 6178 5f64             max_d
-00010910: 7572 3a20 666c 6f61 742c 0d0a 2020 2020  ur: float,..    
-00010920: 2020 2020 2020 2020 6576 656e 5f73 706c          even_spl
-00010930: 6974 3a20 626f 6f6c 203d 2054 7275 652c  it: bool = True,
-00010940: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00010950: 7263 655f 6c65 6e3a 2062 6f6f 6c20 3d20  rce_len: bool = 
-00010960: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-00010970: 2020 2020 6c6f 636b 3a20 626f 6f6c 203d      lock: bool =
-00010980: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
-00010990: 2020 2020 2069 6e63 6c75 6465 5f6c 6f63       include_loc
-000109a0: 6b3a 2062 6f6f 6c20 3d20 4661 6c73 652c  k: bool = False,
-000109b0: 0d0a 2020 2020 2020 2020 2020 2020 6e65  ..            ne
-000109c0: 776c 696e 653a 2062 6f6f 6c20 3d20 4661  wline: bool = Fa
-000109d0: 6c73 650d 0a20 2020 2029 202d 3e20 2257  lse..    ) -> "W
-000109e0: 6869 7370 6572 5265 7375 6c74 223a 0d0a  hisperResult":..
-000109f0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00010a00: 2020 2020 2053 706c 6974 2028 696e 2d70       Split (in-p
-00010a10: 6c61 6365 2920 616e 7920 7365 676d 656e  lace) any segmen
-00010a20: 7420 7468 6174 2065 7863 6565 6473 2060  t that exceeds `
-00010a30: 606d 6178 5f64 7572 6060 2069 6e74 6f20  `max_dur`` into 
-00010a40: 736d 616c 6c65 7220 7365 676d 656e 7473  smaller segments
-00010a50: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
-00010a60: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
-00010a70: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
-00010a80: 2020 2020 206d 6178 5f64 7572 203a 2066       max_dur : f
-00010a90: 6c6f 6174 0d0a 2020 2020 2020 2020 2020  loat..          
-00010aa0: 2020 4d61 7869 6d75 6d20 6475 7261 7469    Maximum durati
-00010ab0: 6f6e 2028 696e 2073 6563 6f6e 6473 2920  on (in seconds) 
-00010ac0: 7065 7220 7365 676d 656e 742e 0d0a 2020  per segment...  
-00010ad0: 2020 2020 2020 6576 656e 5f73 706c 6974        even_split
-00010ae0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-00010af0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
-00010b00: 2020 2057 6865 7468 6572 2074 6f20 6576     Whether to ev
-00010b10: 656e 6c79 2073 706c 6974 2061 2073 6567  enly split a seg
-00010b20: 6d65 6e74 2069 6e20 6c65 6e67 7468 2069  ment in length i
-00010b30: 6620 6974 2065 7863 6565 6473 2060 606d  f it exceeds ``m
-00010b40: 6178 5f64 7572 6060 2e0d 0a20 2020 2020  ax_dur``...     
-00010b50: 2020 2066 6f72 6365 5f6c 656e 203a 2062     force_len : b
-00010b60: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
-00010b70: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-00010b80: 5768 6574 6865 7220 746f 2066 6f72 6365  Whether to force
-00010b90: 2061 2063 6f6e 7374 616e 7420 6c65 6e67   a constant leng
-00010ba0: 7468 2066 6f72 2065 6163 6820 7365 676d  th for each segm
-00010bb0: 656e 7420 6578 6365 7074 2074 6865 206c  ent except the l
-00010bc0: 6173 7420 7365 676d 656e 742e 0d0a 2020  ast segment...  
-00010bd0: 2020 2020 2020 2020 2020 5468 6973 2077            This w
-00010be0: 696c 6c20 6967 6e6f 7265 2061 6c6c 2070  ill ignore all p
-00010bf0: 7265 7669 6f75 7320 6e6f 6e2d 6c6f 636b  revious non-lock
-00010c00: 6564 2073 6567 6d65 6e74 2062 6f75 6e64  ed segment bound
-00010c10: 6172 6965 732e 0d0a 2020 2020 2020 2020  aries...        
-00010c20: 6c6f 636b 203a 2062 6f6f 6c2c 2064 6566  lock : bool, def
-00010c30: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
-00010c40: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-00010c50: 746f 2070 7265 7665 6e74 2066 7574 7572  to prevent futur
-00010c60: 6520 7370 6c69 7473 2f6d 6572 6765 7320  e splits/merges 
-00010c70: 6672 6f6d 2061 6c74 6572 696e 6720 6368  from altering ch
-00010c80: 616e 6765 7320 6d61 6465 2062 7920 7468  anges made by th
-00010c90: 6973 206d 6574 686f 642e 0d0a 2020 2020  is method...    
-00010ca0: 2020 2020 696e 636c 7564 655f 6c6f 636b      include_lock
-00010cb0: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-00010cc0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-00010cd0: 2020 2057 6865 7468 6572 2074 6f20 696e     Whether to in
-00010ce0: 636c 7564 6520 7072 6576 696f 7573 206c  clude previous l
-00010cf0: 6f63 6b20 6265 666f 7265 2073 706c 6974  ock before split
-00010d00: 7469 6e67 2062 6173 6564 206f 6e20 6d61  ting based on ma
-00010d10: 785f 776f 7264 732c 2069 6620 6060 6576  x_words, if ``ev
-00010d20: 656e 5f73 706c 6974 203d 2046 616c 7365  en_split = False
-00010d30: 6060 2e0d 0a20 2020 2020 2020 2020 2020  ``...           
-00010d40: 2053 706c 6974 7469 6e67 2077 696c 6c20   Splitting will 
-00010d50: 6265 2064 6f6e 6520 6166 7465 7220 7468  be done after th
-00010d60: 6520 6669 7273 7420 6e6f 6e2d 6c6f 636b  e first non-lock
-00010d70: 6564 2077 6f72 6420 3e20 6060 6d61 785f  ed word > ``max_
-00010d80: 6475 7260 602e 0d0a 2020 2020 2020 2020  dur``...        
-00010d90: 6e65 776c 696e 653a 2062 6f6f 6c2c 2064  newline: bool, d
-00010da0: 6566 6175 6c74 2046 616c 7365 0d0a 2020  efault False..  
-00010db0: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
-00010dc0: 7220 746f 2069 6e73 6572 7420 6c69 6e65  r to insert line
-00010dd0: 2062 7265 616b 2061 7420 7468 6520 7370   break at the sp
-00010de0: 6c69 7420 706f 696e 7473 2069 6e73 7465  lit points inste
-00010df0: 6164 206f 6620 7370 6c69 7474 696e 6720  ad of splitting 
-00010e00: 696e 746f 2073 6570 6172 6174 6520 7365  into separate se
-00010e10: 676d 656e 7473 2e0d 0a0d 0a20 2020 2020  gments.....     
-00010e20: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-00010e30: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-00010e40: 2020 2020 2073 7461 626c 655f 7768 6973       stable_whis
-00010e50: 7065 722e 7265 7375 6c74 2e57 6869 7370  per.result.Whisp
-00010e60: 6572 5265 7375 6c74 0d0a 2020 2020 2020  erResult..      
-00010e70: 2020 2020 2020 5468 6520 6375 7272 656e        The curren
-00010e80: 7420 696e 7374 616e 6365 2061 6674 6572  t instance after
-00010e90: 2074 6865 2063 6861 6e67 6573 2e0d 0a0d   the changes....
-00010ea0: 0a20 2020 2020 2020 204e 6f74 6573 0d0a  .        Notes..
-00010eb0: 2020 2020 2020 2020 2d2d 2d2d 2d0d 0a20          -----.. 
-00010ec0: 2020 2020 2020 2049 6620 6060 6576 656e         If ``even
-00010ed0: 5f73 706c 6974 203d 2054 7275 6560 602c  _split = True``,
-00010ee0: 2073 6567 6d65 6e74 7320 6361 6e20 7374   segments can st
-00010ef0: 696c 6c20 6578 6365 6564 2060 606d 6178  ill exceed ``max
-00010f00: 5f64 7572 6060 2061 6e64 206c 6f63 6b65  _dur`` and locke
-00010f10: 6420 776f 7264 7320 7769 6c6c 2062 6520  d words will be 
-00010f20: 6967 6e6f 7265 6420 746f 2061 766f 6964  ignored to avoid
-00010f30: 0d0a 2020 2020 2020 2020 756e 6576 656e  ..        uneven
-00010f40: 2073 706c 6974 7469 6e67 2e0d 0a20 2020   splitting...   
-00010f50: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00010f60: 2020 6966 2066 6f72 6365 5f6c 656e 3a0d    if force_len:.
-00010f70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010f80: 662e 6d65 7267 655f 616c 6c5f 7365 676d  f.merge_all_segm
-00010f90: 656e 7473 2829 0d0a 2020 2020 2020 2020  ents()..        
-00010fa0: 7365 6c66 2e5f 7370 6c69 745f 7365 676d  self._split_segm
-00010fb0: 656e 7473 280d 0a20 2020 2020 2020 2020  ents(..         
-00010fc0: 2020 206c 616d 6264 6120 783a 2078 2e67     lambda x: x.g
-00010fd0: 6574 5f64 7572 6174 696f 6e5f 696e 6469  et_duration_indi
-00010fe0: 6365 7328 0d0a 2020 2020 2020 2020 2020  ces(..          
-00010ff0: 2020 2020 2020 6d61 785f 6475 723d 6d61        max_dur=ma
-00011000: 785f 6475 722c 0d0a 2020 2020 2020 2020  x_dur,..        
-00011010: 2020 2020 2020 2020 6576 656e 5f73 706c          even_spl
-00011020: 6974 3d65 7665 6e5f 7370 6c69 742c 0d0a  it=even_split,..
-00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011040: 696e 636c 7564 655f 6c6f 636b 3d69 6e63  include_lock=inc
-00011050: 6c75 6465 5f6c 6f63 6b0d 0a20 2020 2020  lude_lock..     
-00011060: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-00011070: 2020 2020 2020 206c 6f63 6b3d 6c6f 636b         lock=lock
-00011080: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
-00011090: 6577 6c69 6e65 3d6e 6577 6c69 6e65 0d0a  ewline=newline..
-000110a0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-000110b0: 2020 2069 6620 7365 6c66 2e5f 7265 6772     if self._regr
-000110c0: 6f75 705f 6869 7374 6f72 793a 0d0a 2020  oup_history:..  
-000110d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000110e0: 7265 6772 6f75 705f 6869 7374 6f72 7920  regroup_history 
-000110f0: 2b3d 2027 5f27 0d0a 2020 2020 2020 2020  += '_'..        
-00011100: 7365 6c66 2e5f 7265 6772 6f75 705f 6869  self._regroup_hi
-00011110: 7374 6f72 7920 2b3d 2028 6627 7364 3d7b  story += (f'sd={
-00011120: 6d61 785f 6475 727d 2b7b 696e 7428 6576  max_dur}+{int(ev
-00011130: 656e 5f73 706c 6974 297d 2b7b 696e 7428  en_split)}+{int(
-00011140: 666f 7263 655f 6c65 6e29 7d27 0d0a 2020  force_len)}'..  
-00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011170: 6627 2b7b 696e 7428 6c6f 636b 297d 2b7b  f'+{int(lock)}+{
-00011180: 696e 7428 696e 636c 7564 655f 6c6f 636b  int(include_lock
-00011190: 297d 2b7b 696e 7428 6e65 776c 696e 6529  )}+{int(newline)
-000111a0: 7d27 290d 0a20 2020 2020 2020 2072 6574  }')..        ret
-000111b0: 7572 6e20 7365 6c66 0d0a 0d0a 2020 2020  urn self....    
-000111c0: 6465 6620 636c 616d 705f 6d61 7828 0d0a  def clamp_max(..
-000111d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000111e0: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-000111f0: 6564 6975 6d5f 6661 6374 6f72 3a20 666c  edium_factor: fl
-00011200: 6f61 7420 3d20 322e 352c 0d0a 2020 2020  oat = 2.5,..    
-00011210: 2020 2020 2020 2020 6d61 785f 6475 723a          max_dur:
-00011220: 2066 6c6f 6174 203d 204e 6f6e 652c 0d0a   float = None,..
-00011230: 2020 2020 2020 2020 2020 2020 636c 6970              clip
-00011240: 5f73 7461 7274 3a20 4f70 7469 6f6e 616c  _start: Optional
-00011250: 5b62 6f6f 6c5d 203d 204e 6f6e 652c 0d0a  [bool] = None,..
-00011260: 2020 2020 2020 2020 2020 2020 7665 7262              verb
-00011270: 6f73 653a 2062 6f6f 6c20 3d20 4661 6c73  ose: bool = Fals
-00011280: 650d 0a20 2020 2029 202d 3e20 2257 6869  e..    ) -> "Whi
-00011290: 7370 6572 5265 7375 6c74 223a 0d0a 2020  sperResult":..  
-000112a0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000112b0: 2020 2043 6c61 6d70 2061 6c6c 2077 6f72     Clamp all wor
-000112c0: 6420 6475 7261 7469 6f6e 7320 6162 6f76  d durations abov
-000112d0: 6520 6365 7274 6169 6e20 7661 6c75 652e  e certain value.
-000112e0: 0d0a 0d0a 2020 2020 2020 2020 5468 6973  ....        This
-000112f0: 2069 7320 6d6f 7374 2065 6666 6563 7469   is most effecti
-00011300: 7665 2077 6865 6e20 6170 706c 6965 6420  ve when applied 
-00011310: 6265 666f 7265 2061 6e64 2061 6674 6572  before and after
-00011320: 206f 7468 6572 2072 6567 726f 7570 206f   other regroup o
-00011330: 7065 7261 7469 6f6e 732e 0d0a 0d0a 2020  perations.....  
-00011340: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00011350: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00011360: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6d65  ----..        me
-00011370: 6469 756d 5f66 6163 746f 7220 3a20 666c  dium_factor : fl
-00011380: 6f61 742c 2064 6566 6175 6c74 2032 2e35  oat, default 2.5
-00011390: 0d0a 2020 2020 2020 2020 2020 2020 436c  ..            Cl
-000113a0: 616d 7020 6475 7261 7469 6f6e 7320 6162  amp durations ab
-000113b0: 6f76 6520 2860 606d 6564 6975 6d5f 6661  ove (``medium_fa
-000113c0: 6374 6f72 6060 202a 206d 6564 6975 6d20  ctor`` * medium 
-000113d0: 6475 7261 7469 6f6e 2920 7065 7220 7365  duration) per se
-000113e0: 676d 656e 742e 0d0a 2020 2020 2020 2020  gment...        
-000113f0: 2020 2020 4966 2060 606d 6564 6975 6d5f      If ``medium_
-00011400: 6661 6374 6f72 203d 204e 6f6e 652f 3060  factor = None/0`
-00011410: 6020 6f72 2073 6567 6d65 6e74 2068 6173  ` or segment has
-00011420: 206c 6573 7320 7468 616e 2033 2077 6f72   less than 3 wor
-00011430: 6473 2c20 6974 2077 696c 6c20 6265 2069  ds, it will be i
-00011440: 676e 6f72 6564 2061 6e64 2075 7365 206f  gnored and use o
-00011450: 6e6c 7920 6060 6d61 785f 6475 7260 602e  nly ``max_dur``.
-00011460: 0d0a 2020 2020 2020 2020 6d61 785f 6475  ..        max_du
-00011470: 7220 3a20 666c 6f61 742c 206f 7074 696f  r : float, optio
-00011480: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
-00011490: 2043 6c61 6d70 2064 7572 6174 696f 6e73   Clamp durations
-000114a0: 2061 626f 7665 2060 606d 6178 5f64 7572   above ``max_dur
-000114b0: 6060 2e0d 0a20 2020 2020 2020 2063 6c69  ``...        cli
-000114c0: 705f 7374 6172 7420 3a20 626f 6f6c 206f  p_start : bool o
-000114d0: 7220 4e6f 6e65 2c20 6465 6661 756c 7420  r None, default 
-000114e0: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
-000114f0: 2020 5768 6574 6865 7220 746f 2063 6c61    Whether to cla
-00011500: 6d70 2074 6865 2073 7461 7274 206f 6620  mp the start of 
-00011510: 6120 776f 7264 2e20 4966 2060 604e 6f6e  a word. If ``Non
-00011520: 6560 602c 2063 6c61 6d70 2074 6865 2073  e``, clamp the s
-00011530: 7461 7274 206f 6620 6669 7273 7420 776f  tart of first wo
-00011540: 7264 2061 6e64 2065 6e64 206f 6620 6c61  rd and end of la
-00011550: 7374 2077 6f72 6420 7065 720d 0a20 2020  st word per..   
-00011560: 2020 2020 2020 2020 2073 6567 6d65 6e74           segment
-00011570: 2e0d 0a20 2020 2020 2020 2076 6572 626f  ...        verbo
-00011580: 7365 203a 2062 6f6f 6c2c 2064 6566 6175  se : bool, defau
-00011590: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
-000115a0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-000115b0: 2070 7269 6e74 206f 7574 2074 6865 2074   print out the t
-000115c0: 696d 6573 7461 6d70 2063 6861 6e67 6573  imestamp changes
-000115d0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
-000115e0: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
-000115f0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
-00011600: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
-00011610: 7375 6c74 2e57 6869 7370 6572 5265 7375  sult.WhisperResu
-00011620: 6c74 0d0a 2020 2020 2020 2020 2020 2020  lt..            
-00011630: 5468 6520 6375 7272 656e 7420 696e 7374  The current inst
-00011640: 616e 6365 2061 6674 6572 2074 6865 2063  ance after the c
-00011650: 6861 6e67 6573 2e0d 0a20 2020 2020 2020  hanges...       
-00011660: 2022 2222 0d0a 2020 2020 2020 2020 6966   """..        if
-00011670: 206e 6f74 2028 6d65 6469 756d 5f66 6163   not (medium_fac
-00011680: 746f 7220 6f72 206d 6178 5f64 7572 293a  tor or max_dur):
-00011690: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-000116a0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-000116b0: 4174 206c 6561 7374 206f 6e65 206f 6620  At least one of 
-000116c0: 666f 6c6c 6f77 696e 6720 6172 6775 6d65  following argume
-000116d0: 6e74 7320 7265 7175 6972 6573 206e 6f6e  nts requires non
-000116e0: 2d7a 6572 6f20 7661 6c75 653a 206d 6564  -zero value: med
-000116f0: 6975 6d5f 6661 6374 6f72 3b20 6d61 785f  ium_factor; max_
-00011700: 6475 7227 290d 0a0d 0a20 2020 2020 2020  dur')....       
-00011710: 2069 6620 6e6f 7420 7365 6c66 2e68 6173   if not self.has
-00011720: 5f77 6f72 6473 3a0d 0a20 2020 2020 2020  _words:..       
-00011730: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-00011740: 726e 2827 4361 6e6e 6f74 2063 6c61 6d70  rn('Cannot clamp
-00011750: 2064 7565 2074 6f20 6d69 7373 696e 672f   due to missing/
-00011760: 6e6f 2077 6f72 642d 7469 6d65 7374 616d  no word-timestam
-00011770: 7073 2729 0d0a 2020 2020 2020 2020 2020  ps')..          
-00011780: 2020 7265 7475 726e 2073 656c 660d 0a0d    return self...
-00011790: 0a20 2020 2020 2020 2066 6f72 2073 6567  .        for seg
-000117a0: 2069 6e20 7365 6c66 2e73 6567 6d65 6e74   in self.segment
-000117b0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000117c0: 6375 7272 5f6d 6178 5f64 7572 203d 204e  curr_max_dur = N
-000117d0: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
-000117e0: 2069 6620 6d65 6469 756d 5f66 6163 746f   if medium_facto
-000117f0: 7220 616e 6420 6c65 6e28 7365 672e 776f  r and len(seg.wo
-00011800: 7264 7329 203e 2032 3a0d 0a20 2020 2020  rds) > 2:..     
-00011810: 2020 2020 2020 2020 2020 2064 7572 6174             durat
-00011820: 696f 6e73 203d 206e 702e 6172 7261 7928  ions = np.array(
-00011830: 5b77 6f72 642e 6475 7261 7469 6f6e 2066  [word.duration f
-00011840: 6f72 2077 6f72 6420 696e 2073 6567 2e77  or word in seg.w
-00011850: 6f72 6473 5d29 0d0a 2020 2020 2020 2020  ords])..        
-00011860: 2020 2020 2020 2020 6475 7261 7469 6f6e          duration
-00011870: 732e 736f 7274 2829 0d0a 2020 2020 2020  s.sort()..      
-00011880: 2020 2020 2020 2020 2020 6375 7272 5f6d            curr_m
-00011890: 6178 5f64 7572 203d 206d 6564 6975 6d5f  ax_dur = medium_
-000118a0: 6661 6374 6f72 202a 2064 7572 6174 696f  factor * duratio
-000118b0: 6e73 5b6c 656e 2864 7572 6174 696f 6e73  ns[len(durations
-000118c0: 292f 2f32 202b 2031 5d0d 0a0d 0a20 2020  )//2 + 1]....   
-000118d0: 2020 2020 2020 2020 2069 6620 6d61 785f           if max_
-000118e0: 6475 7220 616e 6420 286e 6f74 2063 7572  dur and (not cur
-000118f0: 725f 6d61 785f 6475 7220 6f72 2063 7572  r_max_dur or cur
-00011900: 725f 6d61 785f 6475 7220 3e20 6d61 785f  r_max_dur > max_
-00011910: 6475 7229 3a0d 0a20 2020 2020 2020 2020  dur):..         
-00011920: 2020 2020 2020 2063 7572 725f 6d61 785f         curr_max_
-00011930: 6475 7220 3d20 6d61 785f 6475 720d 0a0d  dur = max_dur...
-00011940: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011950: 6e6f 7420 6375 7272 5f6d 6178 5f64 7572  not curr_max_dur
-00011960: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00011970: 2020 2063 6f6e 7469 6e75 650d 0a0d 0a20     continue.... 
-00011980: 2020 2020 2020 2020 2020 2069 6620 636c             if cl
-00011990: 6970 5f73 7461 7274 2069 7320 4e6f 6e65  ip_start is None
-000119a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000119b0: 2020 2073 6567 2e77 6f72 6473 5b30 5d2e     seg.words[0].
-000119c0: 636c 616d 705f 6d61 7828 6375 7272 5f6d  clamp_max(curr_m
-000119d0: 6178 5f64 7572 2c20 636c 6970 5f73 7461  ax_dur, clip_sta
-000119e0: 7274 3d54 7275 652c 2076 6572 626f 7365  rt=True, verbose
-000119f0: 3d76 6572 626f 7365 290d 0a20 2020 2020  =verbose)..     
-00011a00: 2020 2020 2020 2020 2020 2073 6567 2e77             seg.w
-00011a10: 6f72 6473 5b2d 315d 2e63 6c61 6d70 5f6d  ords[-1].clamp_m
-00011a20: 6178 2863 7572 725f 6d61 785f 6475 722c  ax(curr_max_dur,
-00011a30: 2063 6c69 705f 7374 6172 743d 4661 6c73   clip_start=Fals
-00011a40: 652c 2076 6572 626f 7365 3d76 6572 626f  e, verbose=verbo
-00011a50: 7365 290d 0a20 2020 2020 2020 2020 2020  se)..           
-00011a60: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00011a70: 2020 2020 2020 2020 666f 7220 692c 2077          for i, w
-00011a80: 6f72 6420 696e 2065 6e75 6d65 7261 7465  ord in enumerate
-00011a90: 2873 6567 2e77 6f72 6473 293a 0d0a 2020  (seg.words):..  
-00011aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ab0: 2020 776f 7264 2e63 6c61 6d70 5f6d 6178    word.clamp_max
-00011ac0: 2863 7572 725f 6d61 785f 6475 722c 2063  (curr_max_dur, c
-00011ad0: 6c69 705f 7374 6172 743d 636c 6970 5f73  lip_start=clip_s
-00011ae0: 7461 7274 2c20 7665 7262 6f73 653d 7665  tart, verbose=ve
-00011af0: 7262 6f73 6529 0d0a 0d0a 2020 2020 2020  rbose)....      
-00011b00: 2020 6966 2073 656c 662e 5f72 6567 726f    if self._regro
-00011b10: 7570 5f68 6973 746f 7279 3a0d 0a20 2020  up_history:..   
-00011b20: 2020 2020 2020 2020 2073 656c 662e 5f72           self._r
-00011b30: 6567 726f 7570 5f68 6973 746f 7279 202b  egroup_history +
-00011b40: 3d20 275f 270d 0a20 2020 2020 2020 2073  = '_'..        s
-00011b50: 656c 662e 5f72 6567 726f 7570 5f68 6973  elf._regroup_his
-00011b60: 746f 7279 202b 3d20 6627 636d 3d7b 6d65  tory += f'cm={me
-00011b70: 6469 756d 5f66 6163 746f 727d 2b7b 6d61  dium_factor}+{ma
-00011b80: 785f 6475 7220 6f72 2022 227d 2b7b 636c  x_dur or ""}+{cl
-00011b90: 6970 5f73 7461 7274 206f 7220 2222 7d2b  ip_start or ""}+
-00011ba0: 7b69 6e74 2876 6572 626f 7365 297d 270d  {int(verbose)}'.
-00011bb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011bc0: 7365 6c66 0d0a 0d0a 2020 2020 6465 6620  self....    def 
-00011bd0: 6c6f 636b 280d 0a20 2020 2020 2020 2020  lock(..         
-00011be0: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
-00011bf0: 2020 2020 2020 7374 6172 7473 7769 7468        startswith
-00011c00: 3a20 556e 696f 6e5b 7374 722c 204c 6973  : Union[str, Lis
-00011c10: 745b 7374 725d 5d20 3d20 4e6f 6e65 2c0d  t[str]] = None,.
-00011c20: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
-00011c30: 7377 6974 683a 2055 6e69 6f6e 5b73 7472  swith: Union[str
-00011c40: 2c20 4c69 7374 5b73 7472 5d5d 203d 204e  , List[str]] = N
-00011c50: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-00011c60: 2020 7269 6768 743a 2062 6f6f 6c20 3d20    right: bool = 
-00011c70: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-00011c80: 2020 206c 6566 743a 2062 6f6f 6c20 3d20     left: bool = 
-00011c90: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-00011ca0: 2020 2020 6361 7365 5f73 656e 7369 7469      case_sensiti
-00011cb0: 7665 3a20 626f 6f6c 203d 2046 616c 7365  ve: bool = False
-00011cc0: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00011cd0: 7472 6970 3a20 626f 6f6c 203d 2054 7275  trip: bool = Tru
-00011ce0: 650d 0a20 2020 2029 202d 3e20 2257 6869  e..    ) -> "Whi
-00011cf0: 7370 6572 5265 7375 6c74 223a 0d0a 2020  sperResult":..  
-00011d00: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00011d10: 2020 204c 6f63 6b20 776f 7264 732f 7365     Lock words/se
-00011d20: 676d 656e 7473 2077 6974 6820 6d61 7463  gments with matc
-00011d30: 6869 6e67 2070 7265 6669 782f 7375 6666  hing prefix/suff
-00011d40: 6978 2074 6f20 7072 6576 656e 7420 7370  ix to prevent sp
-00011d50: 6c69 7474 696e 672f 6d65 7267 696e 672e  litting/merging.
-00011d60: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
-00011d70: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
-00011d80: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
-00011d90: 2020 2020 7374 6172 7473 7769 7468 3a20      startswith: 
-00011da0: 7374 7220 6f72 206c 6973 7420 6f66 2073  str or list of s
-00011db0: 7472 0d0a 2020 2020 2020 2020 2020 2020  tr..            
-00011dc0: 5072 6566 6978 6573 2074 6f20 6c6f 636b  Prefixes to lock
-00011dd0: 2e0d 0a20 2020 2020 2020 2065 6e64 7377  ...        endsw
-00011de0: 6974 683a 2073 7472 206f 7220 6c69 7374  ith: str or list
-00011df0: 206f 6620 7374 720d 0a20 2020 2020 2020   of str..       
-00011e00: 2020 2020 2053 7566 6669 7865 7320 746f       Suffixes to
-00011e10: 206c 6f63 6b2e 0d0a 2020 2020 2020 2020   lock...        
-00011e20: 7269 6768 7420 3a20 626f 6f6c 2c20 6465  right : bool, de
-00011e30: 6661 756c 7420 5472 7565 0d0a 2020 2020  fault True..    
-00011e40: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-00011e50: 7072 6576 656e 7420 7370 6c69 7473 2f6d  prevent splits/m
-00011e60: 6572 6765 7320 7769 7468 2074 6865 206e  erges with the n
-00011e70: 6578 7420 776f 7264 2f73 6567 6d65 6e74  ext word/segment
-00011e80: 2e0d 0a20 2020 2020 2020 206c 6566 7420  ...        left 
-00011e90: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-00011ea0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-00011eb0: 2020 2057 6865 7468 6572 2070 7265 7665     Whether preve
-00011ec0: 6e74 2073 706c 6974 732f 6d65 7267 6573  nt splits/merges
-00011ed0: 2077 6974 6820 7468 6520 7072 6576 696f   with the previo
-00011ee0: 7573 2077 6f72 642f 7365 676d 656e 742e  us word/segment.
-00011ef0: 0d0a 2020 2020 2020 2020 6361 7365 5f73  ..        case_s
-00011f00: 656e 7369 7469 7665 203a 2062 6f6f 6c2c  ensitive : bool,
-00011f10: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
-00011f20: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-00011f30: 6865 7220 746f 206d 6174 6368 2074 6865  her to match the
-00011f40: 2063 6173 6520 6f66 2074 6865 2070 7265   case of the pre
-00011f50: 6669 7865 732f 7375 6666 6978 6573 2077  fixes/suffixes w
-00011f60: 6974 6820 7468 6520 776f 7264 732f 7365  ith the words/se
-00011f70: 676d 656e 7473 2e0d 0a20 2020 2020 2020  gments...       
-00011f80: 2073 7472 6970 203a 2062 6f6f 6c2c 2064   strip : bool, d
-00011f90: 6566 6175 6c74 2054 7275 650d 0a20 2020  efault True..   
-00011fa0: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
-00011fb0: 2074 6f20 6967 6e6f 7265 2073 7061 6365   to ignore space
-00011fc0: 7320 6265 666f 7265 2061 6e64 2061 6674  s before and aft
-00011fd0: 6572 2062 6f74 6820 776f 7264 732f 7365  er both words/se
-00011fe0: 676d 656e 7473 2061 6e64 2070 7265 6669  gments and prefi
-00011ff0: 7865 732f 7375 6666 6978 6573 2e0d 0a0d  xes/suffixes....
-00012000: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00012010: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00012020: 2d0d 0a20 2020 2020 2020 2073 7461 626c  -..        stabl
-00012030: 655f 7768 6973 7065 722e 7265 7375 6c74  e_whisper.result
-00012040: 2e57 6869 7370 6572 5265 7375 6c74 0d0a  .WhisperResult..
-00012050: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00012060: 6375 7272 656e 7420 696e 7374 616e 6365  current instance
-00012070: 2061 6674 6572 2074 6865 2063 6861 6e67   after the chang
-00012080: 6573 2e0d 0a20 2020 2020 2020 2022 2222  es...        """
-00012090: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-000120a0: 2073 7461 7274 7377 6974 6820 6f72 2065   startswith or e
-000120b0: 6e64 7377 6974 682c 2027 4d75 7374 2073  ndswith, 'Must s
-000120c0: 7065 6369 6679 205b 7374 6172 7473 7769  pecify [startswi
-000120d0: 7468 5d20 6f72 2f61 6e64 205b 656e 6473  th] or/and [ends
-000120e0: 7769 7468 5d2e 270d 0a20 2020 2020 2020  with].'..       
-000120f0: 2073 7461 7274 7377 6974 6820 3d20 5b5d   startswith = []
-00012100: 2069 6620 7374 6172 7473 7769 7468 2069   if startswith i
-00012110: 7320 4e6f 6e65 2065 6c73 6520 285b 7374  s None else ([st
-00012120: 6172 7473 7769 7468 5d20 6966 2069 7369  artswith] if isi
-00012130: 6e73 7461 6e63 6528 7374 6172 7473 7769  nstance(startswi
-00012140: 7468 2c20 7374 7229 2065 6c73 6520 7374  th, str) else st
-00012150: 6172 7473 7769 7468 290d 0a20 2020 2020  artswith)..     
-00012160: 2020 2065 6e64 7377 6974 6820 3d20 5b5d     endswith = []
-00012170: 2069 6620 656e 6473 7769 7468 2069 7320   if endswith is 
-00012180: 4e6f 6e65 2065 6c73 6520 285b 656e 6473  None else ([ends
-00012190: 7769 7468 5d20 6966 2069 7369 6e73 7461  with] if isinsta
-000121a0: 6e63 6528 656e 6473 7769 7468 2c20 7374  nce(endswith, st
-000121b0: 7229 2065 6c73 6520 656e 6473 7769 7468  r) else endswith
-000121c0: 290d 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
-000121d0: 7420 6361 7365 5f73 656e 7369 7469 7665  t case_sensitive
-000121e0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000121f0: 7461 7274 7377 6974 6820 3d20 5b74 2e6c  tartswith = [t.l
-00012200: 6f77 6572 2829 2066 6f72 2074 2069 6e20  ower() for t in 
-00012210: 7374 6172 7473 7769 7468 5d0d 0a20 2020  startswith]..   
-00012220: 2020 2020 2020 2020 2065 6e64 7377 6974           endswit
-00012230: 6820 3d20 5b74 2e6c 6f77 6572 2829 2066  h = [t.lower() f
-00012240: 6f72 2074 2069 6e20 656e 6473 7769 7468  or t in endswith
-00012250: 5d0d 0a20 2020 2020 2020 2069 6620 7374  ]..        if st
-00012260: 7269 703a 0d0a 2020 2020 2020 2020 2020  rip:..          
-00012270: 2020 7374 6172 7473 7769 7468 203d 205b    startswith = [
-00012280: 742e 7374 7269 7028 2920 666f 7220 7420  t.strip() for t 
-00012290: 696e 2073 7461 7274 7377 6974 685d 0d0a  in startswith]..
-000122a0: 2020 2020 2020 2020 2020 2020 656e 6473              ends
-000122b0: 7769 7468 203d 205b 742e 7374 7269 7028  with = [t.strip(
-000122c0: 2920 666f 7220 7420 696e 2065 6e64 7377  ) for t in endsw
-000122d0: 6974 685d 0d0a 2020 2020 2020 2020 666f  ith]..        fo
-000122e0: 7220 7061 7274 2069 6e20 7365 6c66 2e61  r part in self.a
-000122f0: 6c6c 5f77 6f72 6473 5f6f 725f 7365 676d  ll_words_or_segm
-00012300: 656e 7473 2829 3a0d 0a20 2020 2020 2020  ents():..       
-00012310: 2020 2020 2074 6578 7420 3d20 7061 7274       text = part
-00012320: 2e77 6f72 6420 6966 2068 6173 6174 7472  .word if hasattr
-00012330: 2870 6172 742c 2027 776f 7264 2729 2065  (part, 'word') e
-00012340: 6c73 6520 7061 7274 2e74 6578 740d 0a20  lse part.text.. 
-00012350: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00012360: 7420 6361 7365 5f73 656e 7369 7469 7665  t case_sensitive
-00012370: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00012380: 2020 2074 6578 7420 3d20 7465 7874 2e6c     text = text.l
-00012390: 6f77 6572 2829 0d0a 2020 2020 2020 2020  ower()..        
-000123a0: 2020 2020 6966 2073 7472 6970 3a0d 0a20      if strip:.. 
-000123b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000123c0: 6578 7420 3d20 7465 7874 2e73 7472 6970  ext = text.strip
-000123d0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-000123e0: 666f 7220 7072 6566 6978 2069 6e20 7374  for prefix in st
-000123f0: 6172 7473 7769 7468 3a0d 0a20 2020 2020  artswith:..     
-00012400: 2020 2020 2020 2020 2020 2069 6620 7465             if te
-00012410: 7874 2e73 7461 7274 7377 6974 6828 7072  xt.startswith(pr
-00012420: 6566 6978 293a 0d0a 2020 2020 2020 2020  efix):..        
-00012430: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00012440: 6967 6874 3a0d 0a20 2020 2020 2020 2020  ight:..         
-00012450: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00012460: 6172 742e 6c6f 636b 5f72 6967 6874 2829  art.lock_right()
-00012470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012480: 2020 2020 2020 6966 206c 6566 743a 0d0a        if left:..
-00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124a0: 2020 2020 2020 2020 7061 7274 2e6c 6f63          part.loc
-000124b0: 6b5f 6c65 6674 2829 0d0a 2020 2020 2020  k_left()..      
-000124c0: 2020 2020 2020 666f 7220 7375 6666 6978        for suffix
-000124d0: 2069 6e20 656e 6473 7769 7468 3a0d 0a20   in endswith:.. 
-000124e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000124f0: 6620 7465 7874 2e65 6e64 7377 6974 6828  f text.endswith(
-00012500: 7375 6666 6978 293a 0d0a 2020 2020 2020  suffix):..      
-00012510: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00012520: 2072 6967 6874 3a0d 0a20 2020 2020 2020   right:..       
-00012530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012540: 2070 6172 742e 6c6f 636b 5f72 6967 6874   part.lock_right
-00012550: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00012560: 2020 2020 2020 2020 6966 206c 6566 743a          if left:
-00012570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012580: 2020 2020 2020 2020 2020 7061 7274 2e6c            part.l
-00012590: 6f63 6b5f 6c65 6674 2829 0d0a 2020 2020  ock_left()..    
-000125a0: 2020 2020 6966 2073 656c 662e 5f72 6567      if self._reg
-000125b0: 726f 7570 5f68 6973 746f 7279 3a0d 0a20  roup_history:.. 
-000125c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000125d0: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
-000125e0: 202b 3d20 275f 270d 0a20 2020 2020 2020   += '_'..       
-000125f0: 2073 7461 7274 7377 6974 685f 7374 7220   startswith_str 
-00012600: 3d20 2873 7461 7274 7377 6974 6820 6966  = (startswith if
-00012610: 2069 7369 6e73 7461 6e63 6528 7374 6172   isinstance(star
-00012620: 7473 7769 7468 2c20 7374 7229 2065 6c73  tswith, str) els
-00012630: 6520 272f 272e 6a6f 696e 2873 7461 7274  e '/'.join(start
-00012640: 7377 6974 6829 2920 6966 2073 7461 7274  swith)) if start
-00012650: 7377 6974 6820 656c 7365 2022 220d 0a20  swith else "".. 
-00012660: 2020 2020 2020 2065 6e64 7377 6974 685f         endswith_
-00012670: 7374 7220 3d20 2865 6e64 7377 6974 6820  str = (endswith 
-00012680: 6966 2069 7369 6e73 7461 6e63 6528 656e  if isinstance(en
-00012690: 6473 7769 7468 2c20 7374 7229 2065 6c73  dswith, str) els
-000126a0: 6520 272f 272e 6a6f 696e 2865 6e64 7377  e '/'.join(endsw
-000126b0: 6974 6829 2920 6966 2065 6e64 7377 6974  ith)) if endswit
-000126c0: 6820 656c 7365 2022 220d 0a20 2020 2020  h else ""..     
-000126d0: 2020 2073 656c 662e 5f72 6567 726f 7570     self._regroup
-000126e0: 5f68 6973 746f 7279 202b 3d20 2866 276c  _history += (f'l
-000126f0: 3d7b 7374 6172 7473 7769 7468 5f73 7472  ={startswith_str
-00012700: 7d2b 7b65 6e64 7377 6974 685f 7374 727d  }+{endswith_str}
-00012710: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012730: 2020 2020 2066 272b 7b69 6e74 2872 6967       f'+{int(rig
-00012740: 6874 297d 2b7b 696e 7428 6c65 6674 297d  ht)}+{int(left)}
-00012750: 2b7b 696e 7428 6361 7365 5f73 656e 7369  +{int(case_sensi
-00012760: 7469 7665 297d 2b7b 696e 7428 7374 7269  tive)}+{int(stri
-00012770: 7029 7d27 290d 0a20 2020 2020 2020 2072  p)}')..        r
-00012780: 6574 7572 6e20 7365 6c66 0d0a 0d0a 2020  eturn self....  
-00012790: 2020 6465 6620 7265 6d6f 7665 5f77 6f72    def remove_wor
-000127a0: 6428 0d0a 2020 2020 2020 2020 2020 2020  d(..            
-000127b0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-000127c0: 2020 2077 6f72 643a 2055 6e69 6f6e 5b57     word: Union[W
-000127d0: 6f72 6454 696d 696e 672c 2054 7570 6c65  ordTiming, Tuple
-000127e0: 5b69 6e74 2c20 696e 745d 5d2c 0d0a 2020  [int, int]],..  
-000127f0: 2020 2020 2020 2020 2020 7265 6173 7369            reassi
-00012800: 676e 5f69 6473 3a20 626f 6f6c 203d 2054  gn_ids: bool = T
-00012810: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-00012820: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
-00012830: 3d20 5472 7565 0d0a 2020 2020 2920 2d3e  = True..    ) ->
-00012840: 2027 5768 6973 7065 7252 6573 756c 7427   'WhisperResult'
-00012850: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00012860: 2020 2020 2020 2020 5265 6d6f 7665 2061          Remove a
-00012870: 2077 6f72 642e 0d0a 0d0a 2020 2020 2020   word.....      
-00012880: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
-00012890: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-000128a0: 0d0a 2020 2020 2020 2020 776f 7264 203a  ..        word :
-000128b0: 2057 6f72 6454 696d 696e 6720 6f72 2074   WordTiming or t
-000128c0: 7570 6c65 206f 6620 2869 6e74 2c20 696e  uple of (int, in
-000128d0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-000128e0: 496e 7374 616e 6365 206f 6620 3a63 6c61  Instance of :cla
-000128f0: 7373 3a60 7374 6162 6c65 5f77 6869 7370  ss:`stable_whisp
-00012900: 6572 2e72 6573 756c 742e 576f 7264 5469  er.result.WordTi
-00012910: 6d69 6e67 6020 6f72 2074 7570 6c65 206f  ming` or tuple o
-00012920: 6620 2873 6567 6d65 6e74 2069 6e64 6578  f (segment index
-00012930: 2c20 776f 7264 2069 6e64 6578 292e 0d0a  , word index)...
-00012940: 2020 2020 2020 2020 7265 6173 7369 676e          reassign
-00012950: 5f69 6473 203a 2062 6f6f 6c2c 2064 6566  _ids : bool, def
-00012960: 6175 6c74 2054 7275 650d 0a20 2020 2020  ault True..     
-00012970: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
-00012980: 6f20 7265 6173 7369 676e 2073 6567 6d65  o reassign segme
-00012990: 6e74 2061 6e64 2077 6f72 6420 6964 7320  nt and word ids 
-000129a0: 2869 6e64 6963 6573 2920 6166 7465 7220  (indices) after 
-000129b0: 7265 6d6f 7669 6e67 2060 6077 6f72 6460  removing ``word`
-000129c0: 602e 0d0a 2020 2020 2020 2020 7665 7262  `...        verb
-000129d0: 6f73 6520 3a20 626f 6f6c 2c20 6465 6661  ose : bool, defa
-000129e0: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
-000129f0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-00012a00: 2070 7269 6e74 2064 6574 6169 6c20 6f66   print detail of
-00012a10: 2074 6865 2072 656d 6f76 6564 2077 6f72   the removed wor
-00012a20: 642e 0d0a 0d0a 2020 2020 2020 2020 5265  d.....        Re
-00012a30: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
-00012a40: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-00012a50: 7374 6162 6c65 5f77 6869 7370 6572 2e72  stable_whisper.r
-00012a60: 6573 756c 742e 5768 6973 7065 7252 6573  esult.WhisperRes
-00012a70: 756c 740d 0a20 2020 2020 2020 2020 2020  ult..           
-00012a80: 2054 6865 2063 7572 7265 6e74 2069 6e73   The current ins
-00012a90: 7461 6e63 6520 6166 7465 7220 7468 6520  tance after the 
-00012aa0: 6368 616e 6765 732e 0d0a 2020 2020 2020  changes...      
-00012ab0: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
-00012ac0: 6620 6973 696e 7374 616e 6365 2877 6f72  f isinstance(wor
-00012ad0: 642c 2057 6f72 6454 696d 696e 6729 3a0d  d, WordTiming):.
-00012ae0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00012af0: 7365 6c66 5b77 6f72 642e 7365 676d 656e  self[word.segmen
-00012b00: 745f 6964 5d5b 776f 7264 2e69 645d 2069  t_id][word.id] i
-00012b10: 7320 6e6f 7420 776f 7264 3a0d 0a20 2020  s not word:..   
-00012b20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012b30: 662e 7265 6173 7369 676e 5f69 6473 2829  f.reassign_ids()
-00012b40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012b50: 2020 6966 2073 656c 665b 776f 7264 2e73    if self[word.s
-00012b60: 6567 6d65 6e74 5f69 645d 5b77 6f72 642e  egment_id][word.
-00012b70: 6964 5d20 6973 206e 6f74 2077 6f72 643a  id] is not word:
-00012b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012b90: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00012ba0: 6545 7272 6f72 2827 776f 7264 206e 6f74  eError('word not
-00012bb0: 2069 6e20 7265 7375 6c74 2729 0d0a 2020   in result')..  
-00012bc0: 2020 2020 2020 2020 2020 7365 675f 6964            seg_id
-00012bd0: 2c20 776f 7264 5f69 6420 3d20 776f 7264  , word_id = word
-00012be0: 2e73 6567 6d65 6e74 5f69 642c 2077 6f72  .segment_id, wor
-00012bf0: 642e 6964 0d0a 2020 2020 2020 2020 656c  d.id..        el
-00012c00: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00012c10: 2073 6567 5f69 642c 2077 6f72 645f 6964   seg_id, word_id
-00012c20: 203d 2077 6f72 640d 0a20 2020 2020 2020   = word..       
-00012c30: 2069 6620 7665 7262 6f73 653a 0d0a 2020   if verbose:..  
-00012c40: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00012c50: 6627 5265 6d6f 7665 643a 207b 7365 6c66  f'Removed: {self
-00012c60: 5b73 6567 5f69 645d 5b77 6f72 645f 6964  [seg_id][word_id
-00012c70: 5d2e 746f 5f64 6963 7428 297d 2729 0d0a  ].to_dict()}')..
-00012c80: 2020 2020 2020 2020 6465 6c20 7365 6c66          del self
-00012c90: 2e73 6567 6d65 6e74 735b 7365 675f 6964  .segments[seg_id
-00012ca0: 5d2e 776f 7264 735b 776f 7264 5f69 645d  ].words[word_id]
-00012cb0: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-00012cc0: 2072 6561 7373 6967 6e5f 6964 733a 0d0a   reassign_ids:..
-00012cd0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00012ce0: 726e 2073 656c 660d 0a20 2020 2020 2020  rn self..       
-00012cf0: 2069 6620 7365 6c66 5b73 6567 5f69 645d   if self[seg_id]
-00012d00: 2e68 6173 5f77 6f72 6473 3a0d 0a20 2020  .has_words:..   
-00012d10: 2020 2020 2020 2020 2073 656c 665b 7365           self[se
-00012d20: 675f 6964 5d2e 7265 6173 7369 676e 5f69  g_id].reassign_i
-00012d30: 6473 2829 0d0a 2020 2020 2020 2020 656c  ds()..        el
-00012d40: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00012d50: 2073 656c 662e 7265 6d6f 7665 5f6e 6f5f   self.remove_no_
-00012d60: 776f 7264 5f73 6567 6d65 6e74 7328 290d  word_segments().
-00012d70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012d80: 7365 6c66 0d0a 0d0a 2020 2020 6465 6620  self....    def 
-00012d90: 7265 6d6f 7665 5f73 6567 6d65 6e74 280d  remove_segment(.
-00012da0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012db0: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
-00012dc0: 7365 676d 656e 743a 2055 6e69 6f6e 5b53  segment: Union[S
-00012dd0: 6567 6d65 6e74 2c20 696e 745d 2c0d 0a20  egment, int],.. 
-00012de0: 2020 2020 2020 2020 2020 2072 6561 7373             reass
-00012df0: 6967 6e5f 6964 733a 2062 6f6f 6c20 3d20  ign_ids: bool = 
-00012e00: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-00012e10: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
-00012e20: 203d 2054 7275 650d 0a20 2020 2029 202d   = True..    ) -
-00012e30: 3e20 2757 6869 7370 6572 5265 7375 6c74  > 'WhisperResult
-00012e40: 273a 0d0a 2020 2020 2020 2020 2222 220d  ':..        """.
-00012e50: 0a20 2020 2020 2020 2052 656d 6f76 6520  .        Remove 
-00012e60: 6120 7365 676d 656e 742e 0d0a 0d0a 2020  a segment.....  
-00012e70: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00012e80: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00012e90: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7365  ----..        se
-00012ea0: 676d 656e 7420 3a20 5365 676d 656e 7420  gment : Segment 
-00012eb0: 6f72 2069 6e74 0d0a 2020 2020 2020 2020  or int..        
-00012ec0: 2020 2020 496e 7374 616e 6365 203a 636c      Instance :cl
-00012ed0: 6173 733a 6073 7461 626c 655f 7768 6973  ass:`stable_whis
-00012ee0: 7065 722e 7265 7375 6c74 2e53 6567 6d65  per.result.Segme
-00012ef0: 6e74 6020 6f72 2073 6567 6d65 6e74 2069  nt` or segment i
-00012f00: 6e64 6578 2e0d 0a20 2020 2020 2020 2072  ndex...        r
-00012f10: 6561 7373 6967 6e5f 6964 7320 3a20 626f  eassign_ids : bo
-00012f20: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
-00012f30: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-00012f40: 6574 6865 7220 746f 2072 6561 7373 6967  ether to reassig
-00012f50: 6e20 7365 676d 656e 7420 4944 7320 2869  n segment IDs (i
-00012f60: 6e64 6963 6573 2920 6166 7465 7220 7265  ndices) after re
-00012f70: 6d6f 7669 6e67 2060 6073 6567 6d65 6e74  moving ``segment
-00012f80: 6060 2e0d 0a20 2020 2020 2020 2076 6572  ``...        ver
-00012f90: 626f 7365 203a 2062 6f6f 6c2c 2064 6566  bose : bool, def
-00012fa0: 6175 6c74 2054 7275 650d 0a20 2020 2020  ault True..     
-00012fb0: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
-00012fc0: 6f20 7072 696e 7420 6465 7461 696c 206f  o print detail o
-00012fd0: 6620 7468 6520 7265 6d6f 7665 6420 776f  f the removed wo
-00012fe0: 7264 2e0d 0a0d 0a20 2020 2020 2020 2052  rd.....        R
-00012ff0: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
-00013000: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-00013010: 2073 7461 626c 655f 7768 6973 7065 722e   stable_whisper.
-00013020: 7265 7375 6c74 2e57 6869 7370 6572 5265  result.WhisperRe
-00013030: 7375 6c74 0d0a 2020 2020 2020 2020 2020  sult..          
-00013040: 2020 5468 6520 6375 7272 656e 7420 696e    The current in
-00013050: 7374 616e 6365 2061 6674 6572 2074 6865  stance after the
-00013060: 2063 6861 6e67 6573 2e0d 0a20 2020 2020   changes...     
-00013070: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00013080: 6966 2069 7369 6e73 7461 6e63 6528 7365  if isinstance(se
-00013090: 676d 656e 742c 2053 6567 6d65 6e74 293a  gment, Segment):
-000130a0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000130b0: 2073 656c 665b 7365 676d 656e 742e 6964   self[segment.id
-000130c0: 5d20 6973 206e 6f74 2073 6567 6d65 6e74  ] is not segment
-000130d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000130e0: 2020 2073 656c 662e 7265 6173 7369 676e     self.reassign
-000130f0: 5f69 6473 2829 0d0a 2020 2020 2020 2020  _ids()..        
-00013100: 2020 2020 2020 2020 6966 2073 656c 665b          if self[
-00013110: 7365 676d 656e 742e 6964 5d20 6973 206e  segment.id] is n
-00013120: 6f74 2073 6567 6d65 6e74 3a0d 0a20 2020  ot segment:..   
-00013130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013140: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00013150: 7228 2773 6567 6d65 6e74 206e 6f74 2069  r('segment not i
-00013160: 6e20 7265 7375 6c74 2729 0d0a 2020 2020  n result')..    
-00013170: 2020 2020 2020 2020 7365 676d 656e 7420          segment 
-00013180: 3d20 7365 676d 656e 742e 6964 0d0a 2020  = segment.id..  
-00013190: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
-000131a0: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-000131b0: 7269 6e74 2866 2752 656d 6f76 6564 3a20  rint(f'Removed: 
-000131c0: 5b69 643a 7b73 656c 665b 7365 676d 656e  [id:{self[segmen
-000131d0: 745d 2e69 647d 5d20 7b73 656c 665b 7365  t].id}] {self[se
-000131e0: 676d 656e 745d 2e74 6f5f 6469 7370 6c61  gment].to_displa
-000131f0: 795f 7374 7228 5472 7565 297d 2729 0d0a  y_str(True)}')..
-00013200: 2020 2020 2020 2020 6465 6c20 7365 6c66          del self
-00013210: 2e73 6567 6d65 6e74 735b 7365 676d 656e  .segments[segmen
-00013220: 745d 0d0a 2020 2020 2020 2020 6966 206e  t]..        if n
-00013230: 6f74 2072 6561 7373 6967 6e5f 6964 733a  ot reassign_ids:
-00013240: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00013250: 7475 726e 2073 656c 660d 0a20 2020 2020  turn self..     
-00013260: 2020 2073 656c 662e 7265 6173 7369 676e     self.reassign
-00013270: 5f69 6473 2854 7275 652c 2073 7461 7274  _ids(True, start
-00013280: 3d73 6567 6d65 6e74 290d 0a20 2020 2020  =segment)..     
-00013290: 2020 2072 6574 7572 6e20 7365 6c66 0d0a     return self..
-000132a0: 0d0a 2020 2020 6465 6620 7265 6d6f 7665  ..    def remove
-000132b0: 5f72 6570 6574 6974 696f 6e28 0d0a 2020  _repetition(..  
-000132c0: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
-000132d0: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-000132e0: 5f77 6f72 6473 3a20 696e 7420 3d20 312c  _words: int = 1,
-000132f0: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
-00013300: 7365 5f73 656e 7369 7469 7665 3a20 626f  se_sensitive: bo
-00013310: 6f6c 203d 2046 616c 7365 2c0d 0a20 2020  ol = False,..   
-00013320: 2020 2020 2020 2020 2073 7472 6970 3a20           strip: 
-00013330: 626f 6f6c 203d 2054 7275 652c 0d0a 2020  bool = True,..  
-00013340: 2020 2020 2020 2020 2020 6967 6e6f 7265            ignore
-00013350: 5f70 756e 6374 7561 7469 6f6e 733a 2073  _punctuations: s
-00013360: 7472 203d 2022 5c22 272c 2e3f 2122 2c0d  tr = "\"',.?!",.
-00013370: 0a20 2020 2020 2020 2020 2020 2065 7874  .            ext
-00013380: 656e 645f 6475 7261 7469 6f6e 3a20 626f  end_duration: bo
-00013390: 6f6c 203d 2054 7275 652c 0d0a 2020 2020  ol = True,..    
-000133a0: 2020 2020 2020 2020 7665 7262 6f73 653a          verbose:
-000133b0: 2062 6f6f 6c20 3d20 5472 7565 0d0a 2020   bool = True..  
-000133c0: 2020 2920 2d3e 2027 5768 6973 7065 7252    ) -> 'WhisperR
-000133d0: 6573 756c 7427 3a0d 0a20 2020 2020 2020  esult':..       
-000133e0: 2022 2222 0d0a 2020 2020 2020 2020 5265   """..        Re
-000133f0: 6d6f 7665 2077 6f72 6473 2074 6861 7420  move words that 
-00013400: 7265 7065 6174 2063 6f6e 7365 6375 7469  repeat consecuti
-00013410: 7665 6c79 2e0d 0a0d 0a20 2020 2020 2020  vely.....       
-00013420: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
-00013430: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
-00013440: 0a20 2020 2020 2020 206d 6178 5f77 6f72  .        max_wor
-00013450: 6473 203a 2069 6e74 0d0a 2020 2020 2020  ds : int..      
-00013460: 2020 2020 2020 4d61 7869 6d75 6d20 6e75        Maximum nu
-00013470: 6d62 6572 206f 6620 776f 7264 7320 746f  mber of words to
-00013480: 206c 6f6f 6b20 666f 7220 636f 6e73 6563   look for consec
-00013490: 7574 6976 656c 792e 0d0a 2020 2020 2020  utively...      
-000134a0: 2020 6361 7365 5f73 656e 7369 7469 7665    case_sensitive
-000134b0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-000134c0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-000134d0: 2020 2020 5768 6574 6865 7220 7468 6520      Whether the 
-000134e0: 6361 7365 206f 6620 776f 7264 7320 6e65  case of words ne
-000134f0: 6564 2074 6f20 6d61 7463 6820 746f 2062  ed to match to b
-00013500: 6520 636f 6e73 6964 6572 6564 2061 7320  e considered as 
-00013510: 7265 7065 7469 7469 6f6e 2e0d 0a20 2020  repetition...   
-00013520: 2020 2020 2073 7472 6970 203a 2062 6f6f       strip : boo
-00013530: 6c2c 2064 6566 6175 6c74 2054 7275 650d  l, default True.
-00013540: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
-00013550: 7468 6572 2074 6f20 6967 6e6f 7265 2073  ther to ignore s
-00013560: 7061 6365 7320 6265 666f 7265 2061 6e64  paces before and
-00013570: 2061 6674 6572 2065 6163 6820 776f 7264   after each word
-00013580: 2e0d 0a20 2020 2020 2020 2069 676e 6f72  ...        ignor
-00013590: 655f 7075 6e63 7475 6174 696f 6e73 203a  e_punctuations :
-000135a0: 2062 6f6f 6c2c 2064 6566 6175 6c74 2027   bool, default '
-000135b0: 2227 2c2e 3f21 270d 0a20 2020 2020 2020  "',.?!'..       
-000135c0: 2020 2020 2045 6e64 696e 6720 7075 6e63       Ending punc
-000135d0: 7475 6174 696f 6e73 2074 6f20 6967 6e6f  tuations to igno
-000135e0: 7265 2e0d 0a20 2020 2020 2020 2065 7874  re...        ext
-000135f0: 656e 645f 6475 7261 7469 6f6e 3a20 626f  end_duration: bo
-00013600: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
-00013610: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-00013620: 6574 6865 7220 746f 2065 7874 656e 6420  ether to extend 
-00013630: 7468 6520 6475 7261 7469 6f6e 206f 6620  the duration of 
-00013640: 7468 6520 7072 6576 696f 7573 2077 6f72  the previous wor
-00013650: 6420 746f 2063 6f76 6572 2074 6865 2064  d to cover the d
-00013660: 7572 6174 696f 6e20 6f66 2074 6865 2072  uration of the r
-00013670: 6570 6574 6974 696f 6e2e 0d0a 2020 2020  epetition...    
-00013680: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
-00013690: 6c2c 2064 6566 6175 6c74 2054 7275 650d  l, default True.
-000136a0: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
-000136b0: 7468 6572 2074 6f20 7072 696e 7420 6465  ther to print de
-000136c0: 7461 696c 206f 6620 7468 6520 7265 6d6f  tail of the remo
-000136d0: 7665 6420 7265 7065 7469 7469 6f6e 732e  ved repetitions.
-000136e0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-000136f0: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
-00013700: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7374  ----..        st
-00013710: 6162 6c65 5f77 6869 7370 6572 2e72 6573  able_whisper.res
-00013720: 756c 742e 5768 6973 7065 7252 6573 756c  ult.WhisperResul
-00013730: 740d 0a20 2020 2020 2020 2020 2020 2054  t..            T
-00013740: 6865 2063 7572 7265 6e74 2069 6e73 7461  he current insta
-00013750: 6e63 6520 6166 7465 7220 7468 6520 6368  nce after the ch
-00013760: 616e 6765 732e 0d0a 2020 2020 2020 2020  anges...        
-00013770: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
-00013780: 6e6f 7420 7365 6c66 2e68 6173 5f77 6f72  not self.has_wor
-00013790: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-000137a0: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
-000137b0: 2020 2020 2020 2020 666f 7220 636f 756e          for coun
-000137c0: 7420 696e 2072 616e 6765 2831 2c20 6d61  t in range(1, ma
-000137d0: 785f 776f 7264 7320 2b20 3129 3a0d 0a20  x_words + 1):.. 
-000137e0: 2020 2020 2020 2020 2020 2061 6c6c 5f77             all_w
-000137f0: 6f72 6473 203d 2073 656c 662e 616c 6c5f  ords = self.all_
-00013800: 776f 7264 7328 290d 0a20 2020 2020 2020  words()..       
-00013810: 2020 2020 2069 6620 6c65 6e28 616c 6c5f       if len(all_
-00013820: 776f 7264 7329 203c 2032 3a0d 0a20 2020  words) < 2:..   
-00013830: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00013840: 7572 6e20 7365 6c66 0d0a 2020 2020 2020  urn self..      
-00013850: 2020 2020 2020 616c 6c5f 776f 7264 735f        all_words_
-00013860: 7374 7220 3d20 5b77 2e77 6f72 6420 666f  str = [w.word fo
-00013870: 7220 7720 696e 2061 6c6c 5f77 6f72 6473  r w in all_words
-00013880: 5d0d 0a20 2020 2020 2020 2020 2020 2069  ]..            i
-00013890: 6620 7374 7269 703a 0d0a 2020 2020 2020  f strip:..      
-000138a0: 2020 2020 2020 2020 2020 616c 6c5f 776f            all_wo
-000138b0: 7264 735f 7374 7220 3d20 5b77 2e73 7472  rds_str = [w.str
-000138c0: 6970 2829 2066 6f72 2077 2069 6e20 616c  ip() for w in al
-000138d0: 6c5f 776f 7264 735f 7374 725d 0d0a 2020  l_words_str]..  
-000138e0: 2020 2020 2020 2020 2020 6966 2069 676e            if ign
-000138f0: 6f72 655f 7075 6e63 7475 6174 696f 6e73  ore_punctuations
-00013900: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00013910: 2020 2070 746e 203d 2066 275b 7b69 676e     ptn = f'[{ign
-00013920: 6f72 655f 7075 6e63 7475 6174 696f 6e73  ore_punctuations
-00013930: 7d5d 2b24 270d 0a20 2020 2020 2020 2020  }]+$'..         
-00013940: 2020 2020 2020 2061 6c6c 5f77 6f72 6473         all_words
-00013950: 5f73 7472 203d 205b 7265 2e73 7562 2870  _str = [re.sub(p
-00013960: 746e 2c20 2727 2c20 7729 2066 6f72 2077  tn, '', w) for w
-00013970: 2069 6e20 616c 6c5f 776f 7264 735f 7374   in all_words_st
-00013980: 725d 0d0a 2020 2020 2020 2020 2020 2020  r]..            
-00013990: 6966 206e 6f74 2063 6173 655f 7365 6e73  if not case_sens
-000139a0: 6974 6976 653a 0d0a 2020 2020 2020 2020  itive:..        
-000139b0: 2020 2020 2020 2020 616c 6c5f 776f 7264          all_word
-000139c0: 735f 7374 7220 3d20 5b77 2e6c 6f77 6572  s_str = [w.lower
-000139d0: 2829 2066 6f72 2077 2069 6e20 616c 6c5f  () for w in all_
-000139e0: 776f 7264 735f 7374 725d 0d0a 2020 2020  words_str]..    
-000139f0: 2020 2020 2020 2020 6e65 7874 5f69 203d          next_i =
-00013a00: 204e 6f6e 650d 0a20 2020 2020 2020 2020   None..         
-00013a10: 2020 2063 6861 6e67 6573 203d 205b 5d0d     changes = [].
-00013a20: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00013a30: 2069 2069 6e20 7265 7665 7273 6564 2872   i in reversed(r
-00013a40: 616e 6765 2863 6f75 6e74 2a32 2c20 6c65  ange(count*2, le
-00013a50: 6e28 616c 6c5f 776f 7264 735f 7374 7229  n(all_words_str)
-00013a60: 2b31 2929 3a0d 0a20 2020 2020 2020 2020  +1)):..         
-00013a70: 2020 2020 2020 2069 6620 6e65 7874 5f69         if next_i
-00013a80: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00013a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013aa0: 2020 2069 6620 6e65 7874 5f69 2021 3d20     if next_i != 
-00013ab0: 693a 0d0a 2020 2020 2020 2020 2020 2020  i:..            
-00013ac0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00013ad0: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
-00013ae0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00013af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013b00: 2020 2020 2020 2020 206e 6578 745f 6920           next_i 
-00013b10: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-00013b20: 2020 2020 2020 2020 7320 3d20 6920 2d20          s = i - 
-00013b30: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
-00013b40: 2020 2020 2020 2069 6620 616c 6c5f 776f         if all_wo
-00013b50: 7264 735f 7374 725b 7320 2d20 636f 756e  rds_str[s - coun
-00013b60: 743a 735d 2021 3d20 616c 6c5f 776f 7264  t:s] != all_word
-00013b70: 735f 7374 725b 733a 695d 3a0d 0a20 2020  s_str[s:i]:..   
-00013b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b90: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
-00013ba0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00013bb0: 6920 3d20 730d 0a20 2020 2020 2020 2020  i = s..         
-00013bc0: 2020 2020 2020 2069 6620 6578 7465 6e64         if extend
-00013bd0: 5f64 7572 6174 696f 6e3a 0d0a 2020 2020  _duration:..    
-00013be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bf0: 616c 6c5f 776f 7264 735b 732d 315d 2e65  all_words[s-1].e
-00013c00: 6e64 203d 2061 6c6c 5f77 6f72 6473 5b69  nd = all_words[i
-00013c10: 2d31 5d2e 656e 640d 0a20 2020 2020 2020  -1].end..       
-00013c20: 2020 2020 2020 2020 2074 656d 705f 6368           temp_ch
-00013c30: 616e 6765 7320 3d20 5b5d 0d0a 2020 2020  anges = []..    
-00013c40: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00013c50: 6a20 696e 2072 6576 6572 7365 6428 7261  j in reversed(ra
-00013c60: 6e67 6528 732c 2069 2929 3a0d 0a20 2020  nge(s, i)):..   
-00013c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c80: 2069 6620 7665 7262 6f73 653a 0d0a 2020   if verbose:..  
-00013c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ca0: 2020 2020 2020 7465 6d70 5f63 6861 6e67        temp_chang
-00013cb0: 6573 2e61 7070 656e 6428 6627 2d20 7b61  es.append(f'- {a
-00013cc0: 6c6c 5f77 6f72 6473 5b6a 5d2e 746f 5f64  ll_words[j].to_d
-00013cd0: 6963 7428 297d 2729 0d0a 2020 2020 2020  ict()}')..      
-00013ce0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013cf0: 6c66 2e72 656d 6f76 655f 776f 7264 2861  lf.remove_word(a
-00013d00: 6c6c 5f77 6f72 6473 5b6a 5d2c 2046 616c  ll_words[j], Fal
-00013d10: 7365 2c20 7665 7262 6f73 653d 4661 6c73  se, verbose=Fals
-00013d20: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00013d30: 2020 2020 6966 2074 656d 705f 6368 616e      if temp_chan
-00013d40: 6765 733a 0d0a 2020 2020 2020 2020 2020  ges:..          
-00013d50: 2020 2020 2020 2020 2020 6368 616e 6765            change
-00013d60: 732e 6170 7065 6e64 280d 0a20 2020 2020  s.append(..     
-00013d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d80: 2020 2066 2752 656d 6f76 653a 205b 7b66     f'Remove: [{f
-00013d90: 6f72 6d61 745f 7469 6d65 7374 616d 7028  ormat_timestamp(
-00013da0: 616c 6c5f 776f 7264 735b 735d 2e73 7461  all_words[s].sta
-00013db0: 7274 297d 202d 3e20 7b66 6f72 6d61 745f  rt)} -> {format_
-00013dc0: 7469 6d65 7374 616d 7028 616c 6c5f 776f  timestamp(all_wo
-00013dd0: 7264 735b 692d 315d 2e65 6e64 297d 5d20  rds[i-1].end)}] 
-00013de0: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00013df0: 2020 2020 2020 2020 2020 202b 2027 272e             + ''.
-00013e00: 6a6f 696e 285f 772e 776f 7264 2066 6f72  join(_w.word for
-00013e10: 205f 7720 696e 2061 6c6c 5f77 6f72 6473   _w in all_words
-00013e20: 5b73 3a69 5d29 202b 2027 5c6e 270d 0a20  [s:i]) + '\n'.. 
-00013e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e40: 2020 2020 2020 202b 2027 5c6e 272e 6a6f         + '\n'.jo
-00013e50: 696e 2872 6576 6572 7365 6428 7465 6d70  in(reversed(temp
-00013e60: 5f63 6861 6e67 6573 2929 202b 2027 5c6e  _changes)) + '\n
-00013e70: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00013e80: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00013e90: 2020 2020 2020 2020 2020 666f 7220 6930            for i0
-00013ea0: 2c20 6931 2069 6e20 7a69 7028 7261 6e67  , i1 in zip(rang
-00013eb0: 6528 7320 2d20 636f 756e 742c 2073 292c  e(s - count, s),
-00013ec0: 2072 616e 6765 2873 2c20 6929 293a 0d0a   range(s, i)):..
+0000d7d0: 2020 2020 2020 6d61 785f 6368 6172 7320        max_chars 
+0000d7e0: 616e 640d 0a20 2020 2020 2020 2020 2020  and..           
+0000d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d800: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d820: 2020 2020 2020 2020 2873 6567 2e63 6861          (seg.cha
+0000d830: 725f 636f 756e 7428 2920 2b20 7365 6c66  r_count() + self
+0000d840: 2e73 6567 6d65 6e74 735b 6920 2b20 315d  .segments[i + 1]
+0000d850: 2e63 6861 725f 636f 756e 7428 2920 3e20  .char_count() > 
+0000d860: 6d61 785f 6368 6172 7329 0d0a 2020 2020  max_chars)..    
+0000d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d890: 6966 2069 735f 7375 6d5f 6d61 7820 656c  if is_sum_max el
+0000d8a0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
+0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8c0: 2020 2020 2020 2020 2873 6567 2e63 6861          (seg.cha
+0000d8d0: 725f 636f 756e 7428 2920 3e20 6d61 785f  r_count() > max_
+0000d8e0: 6368 6172 7320 616e 6420 7365 6c66 2e73  chars and self.s
+0000d8f0: 6567 6d65 6e74 735b 6920 2b20 315d 2e63  egments[i + 1].c
+0000d900: 6861 725f 636f 756e 7428 2920 3e20 6d61  har_count() > ma
+0000d910: 785f 6368 6172 7329 0d0a 2020 2020 2020  x_chars)..      
+0000d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d930: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0000d940: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0000d950: 2020 2020 2020 2020 2020 2020 293a 0d0a              ):..
+0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d970: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+0000d980: 2020 2020 2020 7365 6c66 2e61 6464 5f73        self.add_s
+0000d990: 6567 6d65 6e74 7328 692c 2069 202b 2031  egments(i, i + 1
+0000d9a0: 2c20 696e 706c 6163 653d 5472 7565 2c20  , inplace=True, 
+0000d9b0: 6c6f 636b 3d6c 6f63 6b29 0d0a 2020 2020  lock=lock)..    
+0000d9c0: 2020 2020 7365 6c66 2e72 656d 6f76 655f      self.remove_
+0000d9d0: 6e6f 5f77 6f72 645f 7365 676d 656e 7473  no_word_segments
+0000d9e0: 2829 0d0a 0d0a 2020 2020 6465 6620 6765  ()....    def ge
+0000d9f0: 745f 636f 6e74 656e 745f 6279 5f74 696d  t_content_by_tim
+0000da00: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
+0000da10: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+0000da20: 2020 2074 696d 653a 2055 6e69 6f6e 5b66     time: Union[f
+0000da30: 6c6f 6174 2c20 5475 706c 655b 666c 6f61  loat, Tuple[floa
+0000da40: 742c 2066 6c6f 6174 5d2c 2064 6963 745d  t, float], dict]
+0000da50: 2c0d 0a20 2020 2020 2020 2020 2020 2077  ,..            w
+0000da60: 6974 6869 6e3a 2062 6f6f 6c20 3d20 4661  ithin: bool = Fa
+0000da70: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+0000da80: 2020 7365 676d 656e 745f 6c65 7665 6c3a    segment_level:
+0000da90: 2062 6f6f 6c20 3d20 4661 6c73 650d 0a20   bool = False.. 
+0000daa0: 2020 2029 202d 3e20 556e 696f 6e5b 4c69     ) -> Union[Li
+0000dab0: 7374 5b57 6f72 6454 696d 696e 675d 2c20  st[WordTiming], 
+0000dac0: 4c69 7374 5b53 6567 6d65 6e74 5d5d 3a0d  List[Segment]]:.
+0000dad0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0000dae0: 2020 2020 2020 5265 7475 726e 2063 6f6e        Return con
+0000daf0: 7465 6e74 2069 6e20 7468 6520 6060 7469  tent in the ``ti
+0000db00: 6d65 6060 2072 616e 6765 2e0d 0a0d 0a20  me`` range..... 
+0000db10: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0000db20: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+0000db30: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2074  -----..        t
+0000db40: 696d 6520 3a20 666c 6f61 7420 6f72 2074  ime : float or t
+0000db50: 7570 6c65 206f 6620 2866 6c6f 6174 2c20  uple of (float, 
+0000db60: 666c 6f61 7429 206f 7220 6469 6374 0d0a  float) or dict..
+0000db70: 2020 2020 2020 2020 2020 2020 5261 6e67              Rang
+0000db80: 6520 6f66 2074 696d 6520 746f 2066 696e  e of time to fin
+0000db90: 6420 636f 6e74 656e 742e 2046 6f72 2074  d content. For t
+0000dba0: 7570 6c65 206f 6620 7477 6f20 666c 6f61  uple of two floa
+0000dbb0: 7473 2c20 6669 7273 7420 7661 6c75 6520  ts, first value 
+0000dbc0: 6973 2074 6865 2073 7461 7274 2074 696d  is the start tim
+0000dbd0: 6520 616e 6420 7365 636f 6e64 2076 616c  e and second val
+0000dbe0: 7565 2069 730d 0a20 2020 2020 2020 2020  ue is..         
+0000dbf0: 2020 2074 6865 2065 6e64 2074 696d 652e     the end time.
+0000dc00: 2046 6f72 2061 2073 696e 676c 6520 666c   For a single fl
+0000dc10: 6f61 7420 7661 6c75 652c 2069 7420 6973  oat value, it is
+0000dc20: 2074 7265 6174 6564 2061 7320 626f 7468   treated as both
+0000dc30: 2074 6865 2073 7461 7274 2061 6e64 2065   the start and e
+0000dc40: 6e64 2074 696d 652e 0d0a 2020 2020 2020  nd time...      
+0000dc50: 2020 7769 7468 696e 203a 2062 6f6f 6c2c    within : bool,
+0000dc60: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
+0000dc70: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+0000dc80: 6865 7220 746f 206f 6e6c 7920 6669 6e64  her to only find
+0000dc90: 2063 6f6e 7465 6e74 2066 756c 6c79 206f   content fully o
+0000dca0: 7665 726c 6170 7320 7769 7468 2060 6074  verlaps with ``t
+0000dcb0: 696d 6560 6020 7261 6e67 652e 0d0a 2020  ime`` range...  
+0000dcc0: 2020 2020 2020 7365 676d 656e 745f 6c65        segment_le
+0000dcd0: 7665 6c20 3a20 626f 6f6c 2c20 6465 6661  vel : bool, defa
+0000dce0: 756c 7420 4661 6c73 650d 0a20 2020 2020  ult False..     
+0000dcf0: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
+0000dd00: 6f20 6c6f 6f6b 206f 6e6c 7920 6f6e 2074  o look only on t
+0000dd10: 6865 2073 6567 6d65 6e74 206c 6576 656c  he segment level
+0000dd20: 2061 6e64 2072 6574 7572 6e20 696e 7374   and return inst
+0000dd30: 616e 6365 7320 6f66 203a 636c 6173 733a  ances of :class:
+0000dd40: 6073 7461 626c 655f 7768 6973 7065 722e  `stable_whisper.
+0000dd50: 7265 7375 6c74 2e53 6567 6d65 6e74 600d  result.Segment`.
+0000dd60: 0a20 2020 2020 2020 2020 2020 2069 6e73  .            ins
+0000dd70: 7465 6164 206f 6620 3a63 6c61 7373 3a60  tead of :class:`
+0000dd80: 7374 6162 6c65 5f77 6869 7370 6572 2e72  stable_whisper.r
+0000dd90: 6573 756c 742e 576f 7264 5469 6d69 6e67  esult.WordTiming
+0000dda0: 602e 0d0a 0d0a 2020 2020 2020 2020 5265  `.....        Re
+0000ddb0: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
+0000ddc0: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+0000ddd0: 6c69 7374 206f 6620 7374 6162 6c65 5f77  list of stable_w
+0000dde0: 6869 7370 6572 2e72 6573 756c 742e 576f  hisper.result.Wo
+0000ddf0: 7264 5469 6d69 6e67 206f 7220 6c69 7374  rdTiming or list
+0000de00: 206f 6620 7374 6162 6c65 5f77 6869 7370   of stable_whisp
+0000de10: 6572 2e72 6573 756c 742e 5365 676d 656e  er.result.Segmen
+0000de20: 740d 0a20 2020 2020 2020 2020 2020 204c  t..            L
+0000de30: 6973 7420 6f66 2063 6f6e 7465 6e74 7320  ist of contents 
+0000de40: 696e 2074 6865 2060 6074 696d 6560 6020  in the ``time`` 
+0000de50: 7261 6e67 652e 2054 6865 2063 6f6e 7465  range. The conte
+0000de60: 6e74 7320 6172 6520 696e 7374 616e 6365  nts are instance
+0000de70: 7320 6f66 0d0a 2020 2020 2020 2020 2020  s of..          
+0000de80: 2020 3a63 6c61 7373 3a60 7374 6162 6c65    :class:`stable
+0000de90: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
+0000dea0: 5365 676d 656e 7460 2069 6620 6060 7365  Segment` if ``se
+0000deb0: 676d 656e 745f 6c65 7665 6c20 3d20 5472  gment_level = Tr
+0000dec0: 7565 6060 2065 6c73 650d 0a20 2020 2020  ue`` else..     
+0000ded0: 2020 2020 2020 203a 636c 6173 733a 6073         :class:`s
+0000dee0: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
+0000def0: 7375 6c74 2e57 6f72 6454 696d 696e 6760  sult.WordTiming`
+0000df00: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+0000df10: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+0000df20: 6567 6d65 6e74 5f6c 6576 656c 2061 6e64  egment_level and
+0000df30: 206e 6f74 2073 656c 662e 6861 735f 776f   not self.has_wo
+0000df40: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
+0000df50: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0000df60: 6f72 2827 4d69 7373 696e 6720 776f 7264  or('Missing word
+0000df70: 2074 696d 6573 7461 6d70 7320 696e 2072   timestamps in r
+0000df80: 6573 756c 742e 2055 7365 2060 6073 6567  esult. Use ``seg
+0000df90: 6d65 6e74 5f6c 6576 656c 3d54 7275 6560  ment_level=True`
+0000dfa0: 6020 696e 7374 6561 642e 2729 0d0a 2020  ` instead.')..  
+0000dfb0: 2020 2020 2020 636f 6e74 656e 7473 203d        contents =
+0000dfc0: 2073 656c 662e 7365 676d 656e 7473 2069   self.segments i
+0000dfd0: 6620 7365 676d 656e 745f 6c65 7665 6c20  f segment_level 
+0000dfe0: 656c 7365 2073 656c 662e 616c 6c5f 776f  else self.all_wo
+0000dff0: 7264 7328 290d 0a20 2020 2020 2020 2069  rds()..        i
+0000e000: 6620 6973 696e 7374 616e 6365 2874 696d  f isinstance(tim
+0000e010: 652c 2028 666c 6f61 742c 2069 6e74 2929  e, (float, int))
+0000e020: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+0000e030: 696d 6520 3d20 5b74 696d 652c 2074 696d  ime = [time, tim
+0000e040: 655d 0d0a 2020 2020 2020 2020 656c 6966  e]..        elif
+0000e050: 2069 7369 6e73 7461 6e63 6528 7469 6d65   isinstance(time
+0000e060: 2c20 6469 6374 293a 0d0a 2020 2020 2020  , dict):..      
+0000e070: 2020 2020 2020 7469 6d65 203d 205b 7469        time = [ti
+0000e080: 6d65 5b27 7374 6172 7427 5d2c 2074 696d  me['start'], tim
+0000e090: 655b 2765 6e64 275d 5d0d 0a20 2020 2020  e['end']]..     
+0000e0a0: 2020 2073 7461 7274 2c20 656e 6420 3d20     start, end = 
+0000e0b0: 7469 6d65 0d0a 0d0a 2020 2020 2020 2020  time....        
+0000e0c0: 6966 2077 6974 6869 6e3a 0d0a 2020 2020  if within:..    
+0000e0d0: 2020 2020 2020 2020 6465 6620 6973 5f69          def is_i
+0000e0e0: 6e5f 7261 6e67 6528 6329 3a0d 0a20 2020  n_range(c):..   
+0000e0f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000e100: 7572 6e20 7374 6172 7420 3c3d 2063 2e73  urn start <= c.s
+0000e110: 7461 7274 2061 6e64 2065 6e64 203e 3d20  tart and end >= 
+0000e120: 632e 656e 640d 0a20 2020 2020 2020 2065  c.end..        e
+0000e130: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0000e140: 2020 6465 6620 6973 5f69 6e5f 7261 6e67    def is_in_rang
+0000e150: 6528 6329 3a0d 0a20 2020 2020 2020 2020  e(c):..         
+0000e160: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+0000e170: 6172 7420 3c3d 2063 2e65 6e64 2061 6e64  art <= c.end and
+0000e180: 2065 6e64 203e 3d20 632e 7374 6172 740d   end >= c.start.
+0000e190: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+0000e1a0: 6e20 5b63 2066 6f72 2063 2069 6e20 636f  n [c for c in co
+0000e1b0: 6e74 656e 7473 2069 6620 6973 5f69 6e5f  ntents if is_in_
+0000e1c0: 7261 6e67 6528 6329 5d0d 0a0d 0a20 2020  range(c)]....   
+0000e1d0: 2064 6566 2073 706c 6974 5f62 795f 6761   def split_by_ga
+0000e1e0: 7028 0d0a 2020 2020 2020 2020 2020 2020  p(..            
+0000e1f0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+0000e200: 2020 206d 6178 5f67 6170 3a20 666c 6f61     max_gap: floa
+0000e210: 7420 3d20 302e 312c 0d0a 2020 2020 2020  t = 0.1,..      
+0000e220: 2020 2020 2020 6c6f 636b 3a20 626f 6f6c        lock: bool
+0000e230: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
+0000e240: 2020 2020 2020 206e 6577 6c69 6e65 3a20         newline: 
+0000e250: 626f 6f6c 203d 2046 616c 7365 0d0a 2020  bool = False..  
+0000e260: 2020 2920 2d3e 2022 5768 6973 7065 7252    ) -> "WhisperR
+0000e270: 6573 756c 7422 3a0d 0a20 2020 2020 2020  esult":..       
+0000e280: 2022 2222 0d0a 2020 2020 2020 2020 5370   """..        Sp
+0000e290: 6c69 7420 2869 6e2d 706c 6163 6529 2061  lit (in-place) a
+0000e2a0: 6e79 2073 6567 6d65 6e74 2077 6865 7265  ny segment where
+0000e2b0: 2074 6865 2067 6170 2062 6574 7765 656e   the gap between
+0000e2c0: 2074 776f 206f 6620 6974 7320 776f 7264   two of its word
+0000e2d0: 7320 6973 2067 7265 6174 6572 2074 6861  s is greater tha
+0000e2e0: 6e20 6060 6d61 785f 6761 7060 602e 0d0a  n ``max_gap``...
+0000e2f0: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0000e300: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
+0000e310: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
+0000e320: 2020 6d61 785f 6761 7020 3a20 666c 6f61    max_gap : floa
+0000e330: 742c 2064 6566 6175 6c74 2030 2e31 0d0a  t, default 0.1..
+0000e340: 2020 2020 2020 2020 2020 2020 4d61 7869              Maxi
+0000e350: 6d75 6d20 7365 636f 6e64 2873 2920 616c  mum second(s) al
+0000e360: 6c6f 7765 6420 6265 7477 6565 6e20 7477  lowed between tw
+0000e370: 6f20 776f 7264 7320 6966 2074 6865 2073  o words if the s
+0000e380: 616d 6520 7365 676d 656e 742e 0d0a 2020  ame segment...  
+0000e390: 2020 2020 2020 6c6f 636b 203a 2062 6f6f        lock : boo
+0000e3a0: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+0000e3b0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+0000e3c0: 6574 6865 7220 746f 2070 7265 7665 6e74  ether to prevent
+0000e3d0: 2066 7574 7572 6520 7370 6c69 7473 2f6d   future splits/m
+0000e3e0: 6572 6765 7320 6672 6f6d 2061 6c74 6572  erges from alter
+0000e3f0: 696e 6720 6368 616e 6765 7320 6d61 6465  ing changes made
+0000e400: 2062 7920 7468 6973 206d 6574 686f 642e   by this method.
+0000e410: 0d0a 2020 2020 2020 2020 6e65 776c 696e  ..        newlin
+0000e420: 653a 2062 6f6f 6c2c 2064 6566 6175 6c74  e: bool, default
+0000e430: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+0000e440: 2020 2020 5768 6574 6865 7220 746f 2069      Whether to i
+0000e450: 6e73 6572 7420 6c69 6e65 2062 7265 616b  nsert line break
+0000e460: 2061 7420 7468 6520 7370 6c69 7420 706f   at the split po
+0000e470: 696e 7473 2069 6e73 7465 6164 206f 6620  ints instead of 
+0000e480: 7370 6c69 7474 696e 6720 696e 746f 2073  splitting into s
+0000e490: 6570 6172 6174 6520 7365 676d 656e 7473  eparate segments
+0000e4a0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+0000e4b0: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
+0000e4c0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
+0000e4d0: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
+0000e4e0: 7375 6c74 2e57 6869 7370 6572 5265 7375  sult.WhisperResu
+0000e4f0: 6c74 0d0a 2020 2020 2020 2020 2020 2020  lt..            
+0000e500: 5468 6520 6375 7272 656e 7420 696e 7374  The current inst
+0000e510: 616e 6365 2061 6674 6572 2074 6865 2063  ance after the c
+0000e520: 6861 6e67 6573 2e0d 0a20 2020 2020 2020  hanges...       
+0000e530: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
+0000e540: 6c66 2e5f 7370 6c69 745f 7365 676d 656e  lf._split_segmen
+0000e550: 7473 286c 616d 6264 6120 783a 2078 2e67  ts(lambda x: x.g
+0000e560: 6574 5f67 6170 5f69 6e64 6963 6573 286d  et_gap_indices(m
+0000e570: 6178 5f67 6170 292c 206c 6f63 6b3d 6c6f  ax_gap), lock=lo
+0000e580: 636b 2c20 6e65 776c 696e 653d 6e65 776c  ck, newline=newl
+0000e590: 696e 6529 0d0a 2020 2020 2020 2020 6966  ine)..        if
+0000e5a0: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
+0000e5b0: 6973 746f 7279 3a0d 0a20 2020 2020 2020  istory:..       
+0000e5c0: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
+0000e5d0: 7570 5f68 6973 746f 7279 202b 3d20 275f  up_history += '_
+0000e5e0: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+0000e5f0: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
+0000e600: 202b 3d20 6627 7367 3d7b 6d61 785f 6761   += f'sg={max_ga
+0000e610: 707d 2b7b 696e 7428 6c6f 636b 297d 2b7b  p}+{int(lock)}+{
+0000e620: 696e 7428 6e65 776c 696e 6529 7d27 0d0a  int(newline)}'..
+0000e630: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000e640: 656c 660d 0a0d 0a20 2020 2064 6566 206d  elf....    def m
+0000e650: 6572 6765 5f62 795f 6761 7028 0d0a 2020  erge_by_gap(..  
+0000e660: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
+0000e670: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
+0000e680: 5f67 6170 3a20 666c 6f61 7420 3d20 302e  _gap: float = 0.
+0000e690: 312c 0d0a 2020 2020 2020 2020 2020 2020  1,..            
+0000e6a0: 6d61 785f 776f 7264 733a 2069 6e74 203d  max_words: int =
+0000e6b0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+0000e6c0: 2020 2020 6d61 785f 6368 6172 733a 2069      max_chars: i
+0000e6d0: 6e74 203d 204e 6f6e 652c 0d0a 2020 2020  nt = None,..    
+0000e6e0: 2020 2020 2020 2020 6973 5f73 756d 5f6d          is_sum_m
+0000e6f0: 6178 3a20 626f 6f6c 203d 2046 616c 7365  ax: bool = False
+0000e700: 2c0d 0a20 2020 2020 2020 2020 2020 206c  ,..            l
+0000e710: 6f63 6b3a 2062 6f6f 6c20 3d20 4661 6c73  ock: bool = Fals
+0000e720: 650d 0a20 2020 2029 202d 3e20 2257 6869  e..    ) -> "Whi
+0000e730: 7370 6572 5265 7375 6c74 223a 0d0a 2020  sperResult":..  
+0000e740: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0000e750: 2020 204d 6572 6765 2028 696e 2d70 6c61     Merge (in-pla
+0000e760: 6365 2920 616e 7920 7061 6972 206f 6620  ce) any pair of 
+0000e770: 6164 6a61 6365 6e74 2073 6567 6d65 6e74  adjacent segment
+0000e780: 7320 6966 2074 6865 2067 6170 2062 6574  s if the gap bet
+0000e790: 7765 656e 2074 6865 6d20 3c3d 2060 606d  ween them <= ``m
+0000e7a0: 696e 5f67 6170 6060 2e0d 0a0d 0a20 2020  in_gap``.....   
+0000e7b0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
+0000e7c0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000e7d0: 2d2d 2d0d 0a20 2020 2020 2020 206d 696e  ---..        min
+0000e7e0: 5f67 6170 203a 2066 6c6f 6174 2c20 6465  _gap : float, de
+0000e7f0: 6661 756c 7420 302e 310d 0a20 2020 2020  fault 0.1..     
+0000e800: 2020 2020 2020 204d 696e 696d 756d 2073         Minimum s
+0000e810: 6563 6f6e 6428 7329 2061 6c6c 6f77 2062  econd(s) allow b
+0000e820: 6574 7765 656e 2074 776f 2073 6567 6d65  etween two segme
+0000e830: 6e74 2e0d 0a20 2020 2020 2020 206d 6178  nt...        max
+0000e840: 5f77 6f72 6473 203a 2069 6e74 2c20 6f70  _words : int, op
+0000e850: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+0000e860: 2020 2020 4d61 7869 6d75 6d20 6e75 6d62      Maximum numb
+0000e870: 6572 206f 6620 776f 7264 7320 616c 6c6f  er of words allo
+0000e880: 7765 6420 696e 2065 6163 6820 7365 676d  wed in each segm
+0000e890: 656e 742e 0d0a 2020 2020 2020 2020 6d61  ent...        ma
+0000e8a0: 785f 6368 6172 7320 3a20 696e 742c 206f  x_chars : int, o
+0000e8b0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+0000e8c0: 2020 2020 204d 6178 696d 756d 206e 756d       Maximum num
+0000e8d0: 6265 7220 6f66 2063 6861 7261 6374 6572  ber of character
+0000e8e0: 7320 616c 6c6f 7765 6420 696e 2065 6163  s allowed in eac
+0000e8f0: 6820 7365 676d 656e 742e 0d0a 2020 2020  h segment...    
+0000e900: 2020 2020 6973 5f73 756d 5f6d 6178 203a      is_sum_max :
+0000e910: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
+0000e920: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
+0000e930: 2020 5768 6574 6865 7220 6060 6d61 785f    Whether ``max_
+0000e940: 776f 7264 7360 6020 616e 6420 6060 6d61  words`` and ``ma
+0000e950: 785f 6368 6172 7360 6020 6973 2061 7070  x_chars`` is app
+0000e960: 6c69 6564 2074 6f20 7468 6520 6d65 7267  lied to the merg
+0000e970: 6564 2073 6567 6d65 6e74 2069 6e73 7465  ed segment inste
+0000e980: 6164 206f 6620 7468 6520 696e 6469 7669  ad of the indivi
+0000e990: 6475 616c 2073 6567 6d65 6e74 730d 0a20  dual segments.. 
+0000e9a0: 2020 2020 2020 2020 2020 2074 6f20 6265             to be
+0000e9b0: 206d 6572 6765 642e 0d0a 2020 2020 2020   merged...      
+0000e9c0: 2020 6c6f 636b 203a 2062 6f6f 6c2c 2064    lock : bool, d
+0000e9d0: 6566 6175 6c74 2046 616c 7365 0d0a 2020  efault False..  
+0000e9e0: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
+0000e9f0: 7220 746f 2070 7265 7665 6e74 2066 7574  r to prevent fut
+0000ea00: 7572 6520 7370 6c69 7473 2f6d 6572 6765  ure splits/merge
+0000ea10: 7320 6672 6f6d 2061 6c74 6572 696e 6720  s from altering 
+0000ea20: 6368 616e 6765 7320 6d61 6465 2062 7920  changes made by 
+0000ea30: 7468 6973 206d 6574 686f 642e 0d0a 0d0a  this method.....
+0000ea40: 2020 2020 2020 2020 5265 7475 726e 730d          Returns.
+0000ea50: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000ea60: 0d0a 2020 2020 2020 2020 7374 6162 6c65  ..        stable
+0000ea70: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
+0000ea80: 5768 6973 7065 7252 6573 756c 740d 0a20  WhisperResult.. 
+0000ea90: 2020 2020 2020 2020 2020 2054 6865 2063             The c
+0000eaa0: 7572 7265 6e74 2069 6e73 7461 6e63 6520  urrent instance 
+0000eab0: 6166 7465 7220 7468 6520 6368 616e 6765  after the change
+0000eac0: 732e 0d0a 2020 2020 2020 2020 2222 220d  s...        """.
+0000ead0: 0a20 2020 2020 2020 2069 6e64 6963 6573  .        indices
+0000eae0: 203d 2073 656c 662e 6765 745f 6761 705f   = self.get_gap_
+0000eaf0: 696e 6469 6365 7328 6d69 6e5f 6761 7029  indices(min_gap)
+0000eb00: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+0000eb10: 6d65 7267 655f 7365 676d 656e 7473 2869  merge_segments(i
+0000eb20: 6e64 6963 6573 2c0d 0a20 2020 2020 2020  ndices,..       
+0000eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb40: 2020 2020 2020 6d61 785f 776f 7264 733d        max_words=
+0000eb50: 6d61 785f 776f 7264 732c 206d 6178 5f63  max_words, max_c
+0000eb60: 6861 7273 3d6d 6178 5f63 6861 7273 2c20  hars=max_chars, 
+0000eb70: 6973 5f73 756d 5f6d 6178 3d69 735f 7375  is_sum_max=is_su
+0000eb80: 6d5f 6d61 782c 206c 6f63 6b3d 6c6f 636b  m_max, lock=lock
+0000eb90: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+0000eba0: 6c66 2e5f 7265 6772 6f75 705f 6869 7374  lf._regroup_hist
+0000ebb0: 6f72 793a 0d0a 2020 2020 2020 2020 2020  ory:..          
+0000ebc0: 2020 7365 6c66 2e5f 7265 6772 6f75 705f    self._regroup_
+0000ebd0: 6869 7374 6f72 7920 2b3d 2027 5f27 0d0a  history += '_'..
+0000ebe0: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+0000ebf0: 6772 6f75 705f 6869 7374 6f72 7920 2b3d  group_history +=
+0000ec00: 2066 276d 673d 7b6d 696e 5f67 6170 7d2b   f'mg={min_gap}+
+0000ec10: 7b6d 6178 5f77 6f72 6473 206f 7220 2222  {max_words or ""
+0000ec20: 7d2b 7b6d 6178 5f63 6861 7273 206f 7220  }+{max_chars or 
+0000ec30: 2222 7d2b 7b69 6e74 2869 735f 7375 6d5f  ""}+{int(is_sum_
+0000ec40: 6d61 7829 7d2b 7b69 6e74 286c 6f63 6b29  max)}+{int(lock)
+0000ec50: 7d27 0d0a 2020 2020 2020 2020 7265 7475  }'..        retu
+0000ec60: 726e 2073 656c 660d 0a0d 0a20 2020 2064  rn self....    d
+0000ec70: 6566 2073 706c 6974 5f62 795f 7075 6e63  ef split_by_punc
+0000ec80: 7475 6174 696f 6e28 0d0a 2020 2020 2020  tuation(..      
+0000ec90: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+0000eca0: 2020 2020 2020 2020 2070 756e 6374 7561           punctua
+0000ecb0: 7469 6f6e 3a20 556e 696f 6e5b 4c69 7374  tion: Union[List
+0000ecc0: 5b73 7472 5d2c 204c 6973 745b 5475 706c  [str], List[Tupl
+0000ecd0: 655b 7374 722c 2073 7472 5d5d 2c20 7374  e[str, str]], st
+0000ece0: 725d 2c0d 0a20 2020 2020 2020 2020 2020  r],..           
+0000ecf0: 206c 6f63 6b3a 2062 6f6f 6c20 3d20 4661   lock: bool = Fa
+0000ed00: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+0000ed10: 2020 6e65 776c 696e 653a 2062 6f6f 6c20    newline: bool 
+0000ed20: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
+0000ed30: 2020 2020 2020 6d69 6e5f 776f 7264 733a        min_words:
+0000ed40: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+0000ed50: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+0000ed60: 2020 2020 6d69 6e5f 6368 6172 733a 204f      min_chars: O
+0000ed70: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+0000ed80: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+0000ed90: 2020 6d69 6e5f 6475 723a 204f 7074 696f    min_dur: Optio
+0000eda0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650d  nal[int] = None.
+0000edb0: 0a20 2020 2029 202d 3e20 2257 6869 7370  .    ) -> "Whisp
+0000edc0: 6572 5265 7375 6c74 223a 0d0a 2020 2020  erResult":..    
+0000edd0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0000ede0: 2053 706c 6974 2028 696e 2d70 6c61 6365   Split (in-place
+0000edf0: 2920 7365 676d 656e 7473 2061 7420 776f  ) segments at wo
+0000ee00: 7264 7320 7468 6174 2073 7461 7274 2f65  rds that start/e
+0000ee10: 6e64 2077 6974 6820 6060 7075 6e63 7475  nd with ``punctu
+0000ee20: 6174 696f 6e60 602e 0d0a 0d0a 2020 2020  ation``.....    
+0000ee30: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
+0000ee40: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0000ee50: 2d2d 0d0a 2020 2020 2020 2020 7075 6e63  --..        punc
+0000ee60: 7475 6174 696f 6e20 3a20 6c69 7374 206f  tuation : list o
+0000ee70: 6620 7374 7220 6f66 206c 6973 7420 6f66  f str of list of
+0000ee80: 2074 7570 6c65 206f 6620 2873 7472 2c20   tuple of (str, 
+0000ee90: 7374 7229 206f 7220 7374 720d 0a20 2020  str) or str..   
+0000eea0: 2020 2020 2020 2020 2050 756e 6374 7561           Punctua
+0000eeb0: 7469 6f6e 2873 2920 746f 2073 706c 6974  tion(s) to split
+0000eec0: 2073 6567 6d65 6e74 7320 6279 2e0d 0a20   segments by... 
+0000eed0: 2020 2020 2020 206c 6f63 6b20 3a20 626f         lock : bo
+0000eee0: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
+0000eef0: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
+0000ef00: 6865 7468 6572 2074 6f20 7072 6576 656e  hether to preven
+0000ef10: 7420 6675 7475 7265 2073 706c 6974 732f  t future splits/
+0000ef20: 6d65 7267 6573 2066 726f 6d20 616c 7465  merges from alte
+0000ef30: 7269 6e67 2063 6861 6e67 6573 206d 6164  ring changes mad
+0000ef40: 6520 6279 2074 6869 7320 6d65 7468 6f64  e by this method
+0000ef50: 2e0d 0a20 2020 2020 2020 206e 6577 6c69  ...        newli
+0000ef60: 6e65 203a 2062 6f6f 6c2c 2064 6566 6175  ne : bool, defau
+0000ef70: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
+0000ef80: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+0000ef90: 2069 6e73 6572 7420 6c69 6e65 2062 7265   insert line bre
+0000efa0: 616b 2061 7420 7468 6520 7370 6c69 7420  ak at the split 
+0000efb0: 706f 696e 7473 2069 6e73 7465 6164 206f  points instead o
+0000efc0: 6620 7370 6c69 7474 696e 6720 696e 746f  f splitting into
+0000efd0: 2073 6570 6172 6174 6520 7365 676d 656e   separate segmen
+0000efe0: 7473 2e0d 0a20 2020 2020 2020 206d 696e  ts...        min
+0000eff0: 5f77 6f72 6473 203a 2069 6e74 2c20 6f70  _words : int, op
+0000f000: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+0000f010: 2020 2020 5370 6c69 7420 7365 676d 656e      Split segmen
+0000f020: 7473 2077 6974 6820 776f 7264 7320 3e3d  ts with words >=
+0000f030: 2060 606d 696e 5f77 6f72 6473 6060 2e0d   ``min_words``..
+0000f040: 0a20 2020 2020 2020 206d 696e 5f63 6861  .        min_cha
+0000f050: 7273 203a 2069 6e74 2c20 6f70 7469 6f6e  rs : int, option
+0000f060: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
+0000f070: 5370 6c69 7420 7365 676d 656e 7473 2077  Split segments w
+0000f080: 6974 6820 6368 6172 6163 7465 7273 203e  ith characters >
+0000f090: 3d20 6060 6d69 6e5f 6368 6172 7360 602e  = ``min_chars``.
+0000f0a0: 0d0a 2020 2020 2020 2020 6d69 6e5f 6475  ..        min_du
+0000f0b0: 7220 3a20 696e 742c 206f 7074 696f 6e61  r : int, optiona
+0000f0c0: 6c0d 0a20 2020 2020 2020 2020 2020 2073  l..            s
+0000f0d0: 706c 6974 2073 6567 6d65 6e74 7320 7769  plit segments wi
+0000f0e0: 7468 2064 7572 6174 696f 6e20 2869 6e20  th duration (in 
+0000f0f0: 7365 636f 6e64 7329 203e 3d20 6060 6d69  seconds) >= ``mi
+0000f100: 6e5f 6475 7260 602e 0d0a 0d0a 2020 2020  n_dur``.....    
+0000f110: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
+0000f120: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
+0000f130: 2020 2020 2020 7374 6162 6c65 5f77 6869        stable_whi
+0000f140: 7370 6572 2e72 6573 756c 742e 5768 6973  sper.result.Whis
+0000f150: 7065 7252 6573 756c 740d 0a20 2020 2020  perResult..     
+0000f160: 2020 2020 2020 2054 6865 2063 7572 7265         The curre
+0000f170: 6e74 2069 6e73 7461 6e63 6520 6166 7465  nt instance afte
+0000f180: 7220 7468 6520 6368 616e 6765 732e 0d0a  r the changes...
+0000f190: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+0000f1a0: 2020 2020 2064 6566 205f 6f76 6572 5f6d       def _over_m
+0000f1b0: 6178 2878 3a20 5365 676d 656e 7429 3a0d  ax(x: Segment):.
+0000f1c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000f1d0: 7572 6e20 280d 0a20 2020 2020 2020 2020  urn (..         
+0000f1e0: 2020 2020 2020 2020 2020 2028 6d69 6e5f             (min_
+0000f1f0: 776f 7264 7320 616e 6420 6c65 6e28 782e  words and len(x.
+0000f200: 776f 7264 7329 203e 3d20 6d69 6e5f 776f  words) >= min_wo
+0000f210: 7264 7329 206f 720d 0a20 2020 2020 2020  rds) or..       
+0000f220: 2020 2020 2020 2020 2020 2020 2028 6d69               (mi
+0000f230: 6e5f 6368 6172 7320 616e 6420 782e 6368  n_chars and x.ch
+0000f240: 6172 5f63 6f75 6e74 2829 203e 3d20 6d69  ar_count() >= mi
+0000f250: 6e5f 6368 6172 7329 206f 720d 0a20 2020  n_chars) or..   
+0000f260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f270: 2028 6d69 6e5f 6475 7220 616e 6420 782e   (min_dur and x.
+0000f280: 6475 7261 7469 6f6e 203e 3d20 6d69 6e5f  duration >= min_
+0000f290: 6475 7229 0d0a 2020 2020 2020 2020 2020  dur)..          
+0000f2a0: 2020 290d 0a0d 0a20 2020 2020 2020 2069    )....        i
+0000f2b0: 6e64 6963 6573 203d 2073 6574 2873 2e69  ndices = set(s.i
+0000f2c0: 6420 666f 7220 7320 696e 2073 656c 662e  d for s in self.
+0000f2d0: 7365 676d 656e 7473 2069 6620 5f6f 7665  segments if _ove
+0000f2e0: 725f 6d61 7828 7329 2920 6966 2061 6e79  r_max(s)) if any
+0000f2f0: 2828 6d69 6e5f 776f 7264 732c 206d 696e  ((min_words, min
+0000f300: 5f63 6861 7273 2c20 6d69 6e5f 6475 7229  _chars, min_dur)
+0000f310: 2920 656c 7365 204e 6f6e 650d 0a0d 0a20  ) else None.... 
+0000f320: 2020 2020 2020 2064 6566 205f 6765 745f         def _get_
+0000f330: 696e 6469 6365 7328 783a 2053 6567 6d65  indices(x: Segme
+0000f340: 6e74 293a 0d0a 2020 2020 2020 2020 2020  nt):..          
+0000f350: 2020 7265 7475 726e 2078 2e67 6574 5f70    return x.get_p
+0000f360: 756e 6374 7561 7469 6f6e 5f69 6e64 6963  unctuation_indic
+0000f370: 6573 2870 756e 6374 7561 7469 6f6e 2920  es(punctuation) 
+0000f380: 6966 2069 6e64 6963 6573 2069 7320 4e6f  if indices is No
+0000f390: 6e65 206f 7220 782e 6964 2069 6e20 696e  ne or x.id in in
+0000f3a0: 6469 6365 7320 656c 7365 205b 5d0d 0a0d  dices else []...
+0000f3b0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+0000f3c0: 706c 6974 5f73 6567 6d65 6e74 7328 5f67  plit_segments(_g
+0000f3d0: 6574 5f69 6e64 6963 6573 2c20 6c6f 636b  et_indices, lock
+0000f3e0: 3d6c 6f63 6b2c 206e 6577 6c69 6e65 3d6e  =lock, newline=n
+0000f3f0: 6577 6c69 6e65 290d 0a20 2020 2020 2020  ewline)..       
+0000f400: 2069 6620 7365 6c66 2e5f 7265 6772 6f75   if self._regrou
+0000f410: 705f 6869 7374 6f72 793a 0d0a 2020 2020  p_history:..    
+0000f420: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+0000f430: 6772 6f75 705f 6869 7374 6f72 7920 2b3d  group_history +=
+0000f440: 2027 5f27 0d0a 2020 2020 2020 2020 7075   '_'..        pu
+0000f450: 6e63 745f 7374 7220 3d20 272f 272e 6a6f  nct_str = '/'.jo
+0000f460: 696e 2870 2069 6620 6973 696e 7374 616e  in(p if isinstan
+0000f470: 6365 2870 2c20 7374 7229 2065 6c73 6520  ce(p, str) else 
+0000f480: 272a 272e 6a6f 696e 2870 2920 666f 7220  '*'.join(p) for 
+0000f490: 7020 696e 2070 756e 6374 7561 7469 6f6e  p in punctuation
+0000f4a0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000f4b0: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
+0000f4c0: 202b 3d20 6627 7370 3d7b 7075 6e63 745f   += f'sp={punct_
+0000f4d0: 7374 727d 2b7b 696e 7428 6c6f 636b 297d  str}+{int(lock)}
+0000f4e0: 2b7b 696e 7428 6e65 776c 696e 6529 7d27  +{int(newline)}'
+0000f4f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+0000f500: 7265 6772 6f75 705f 6869 7374 6f72 7920  regroup_history 
+0000f510: 2b3d 2066 272b 7b6d 696e 5f77 6f72 6473  += f'+{min_words
+0000f520: 206f 7220 2222 7d2b 7b6d 696e 5f63 6861   or ""}+{min_cha
+0000f530: 7273 206f 7220 2222 7d2b 7b6d 696e 5f64  rs or ""}+{min_d
+0000f540: 7572 206f 7220 2222 7d27 2e72 7374 7269  ur or ""}'.rstri
+0000f550: 7028 272b 2729 0d0a 2020 2020 2020 2020  p('+')..        
+0000f560: 7265 7475 726e 2073 656c 660d 0a0d 0a20  return self.... 
+0000f570: 2020 2064 6566 206d 6572 6765 5f62 795f     def merge_by_
+0000f580: 7075 6e63 7475 6174 696f 6e28 0d0a 2020  punctuation(..  
+0000f590: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
+0000f5a0: 0a20 2020 2020 2020 2020 2020 2070 756e  .            pun
+0000f5b0: 6374 7561 7469 6f6e 3a20 556e 696f 6e5b  ctuation: Union[
+0000f5c0: 4c69 7374 5b73 7472 5d2c 204c 6973 745b  List[str], List[
+0000f5d0: 5475 706c 655b 7374 722c 2073 7472 5d5d  Tuple[str, str]]
+0000f5e0: 2c20 7374 725d 2c0d 0a20 2020 2020 2020  , str],..       
+0000f5f0: 2020 2020 206d 6178 5f77 6f72 6473 3a20       max_words: 
+0000f600: 696e 7420 3d20 4e6f 6e65 2c0d 0a20 2020  int = None,..   
+0000f610: 2020 2020 2020 2020 206d 6178 5f63 6861           max_cha
+0000f620: 7273 3a20 696e 7420 3d20 4e6f 6e65 2c0d  rs: int = None,.
+0000f630: 0a20 2020 2020 2020 2020 2020 2069 735f  .            is_
+0000f640: 7375 6d5f 6d61 783a 2062 6f6f 6c20 3d20  sum_max: bool = 
+0000f650: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+0000f660: 2020 2020 6c6f 636b 3a20 626f 6f6c 203d      lock: bool =
+0000f670: 2046 616c 7365 0d0a 2020 2020 2920 2d3e   False..    ) ->
+0000f680: 2022 5768 6973 7065 7252 6573 756c 7422   "WhisperResult"
+0000f690: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+0000f6a0: 2020 2020 2020 2020 4d65 7267 6520 2869          Merge (i
+0000f6b0: 6e2d 706c 6163 6529 2061 6e79 2074 776f  n-place) any two
+0000f6c0: 2073 6567 6d65 6e74 7320 7468 6174 2068   segments that h
+0000f6d0: 6173 2073 7065 6369 6669 6320 7075 6e63  as specific punc
+0000f6e0: 7475 6174 696f 6e73 2069 6e62 6574 7765  tuations inbetwe
+0000f6f0: 656e 2e0d 0a0d 0a20 2020 2020 2020 2050  en.....        P
+0000f700: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
+0000f710: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+0000f720: 2020 2020 2020 2070 756e 6374 7561 7469         punctuati
+0000f730: 6f6e 203a 206c 6973 7420 6f66 2073 7472  on : list of str
+0000f740: 206f 6620 6c69 7374 206f 6620 7475 706c   of list of tupl
+0000f750: 6520 6f66 2028 7374 722c 2073 7472 2920  e of (str, str) 
+0000f760: 6f72 2073 7472 0d0a 2020 2020 2020 2020  or str..        
+0000f770: 2020 2020 5075 6e63 7475 6174 696f 6e28      Punctuation(
+0000f780: 7329 2074 6f20 6d65 7267 6520 7365 676d  s) to merge segm
+0000f790: 656e 7473 2062 792e 0d0a 2020 2020 2020  ents by...      
+0000f7a0: 2020 6d61 785f 776f 7264 7320 3a20 696e    max_words : in
+0000f7b0: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
+0000f7c0: 2020 2020 2020 2020 204d 6178 696d 756d           Maximum
+0000f7d0: 206e 756d 6265 7220 6f66 2077 6f72 6473   number of words
+0000f7e0: 2061 6c6c 6f77 6564 2069 6e20 6561 6368   allowed in each
+0000f7f0: 2073 6567 6d65 6e74 2e0d 0a20 2020 2020   segment...     
+0000f800: 2020 206d 6178 5f63 6861 7273 203a 2069     max_chars : i
+0000f810: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
+0000f820: 2020 2020 2020 2020 2020 4d61 7869 6d75            Maximu
+0000f830: 6d20 6e75 6d62 6572 206f 6620 6368 6172  m number of char
+0000f840: 6163 7465 7273 2061 6c6c 6f77 6564 2069  acters allowed i
+0000f850: 6e20 6561 6368 2073 6567 6d65 6e74 2e0d  n each segment..
+0000f860: 0a20 2020 2020 2020 2069 735f 7375 6d5f  .        is_sum_
+0000f870: 6d61 7820 3a20 626f 6f6c 2c20 6465 6661  max : bool, defa
+0000f880: 756c 7420 4661 6c73 650d 0a20 2020 2020  ult False..     
+0000f890: 2020 2020 2020 2057 6865 7468 6572 2060         Whether `
+0000f8a0: 606d 6178 5f77 6f72 6473 6060 2061 6e64  `max_words`` and
+0000f8b0: 2060 606d 6178 5f63 6861 7273 6060 2069   ``max_chars`` i
+0000f8c0: 7320 6170 706c 6965 6420 746f 2074 6865  s applied to the
+0000f8d0: 206d 6572 6765 6420 7365 676d 656e 7420   merged segment 
+0000f8e0: 696e 7374 6561 6420 6f66 2074 6865 2069  instead of the i
+0000f8f0: 6e64 6976 6964 7561 6c20 7365 676d 656e  ndividual segmen
+0000f900: 7473 0d0a 2020 2020 2020 2020 2020 2020  ts..            
+0000f910: 746f 2062 6520 6d65 7267 6564 2e0d 0a20  to be merged... 
+0000f920: 2020 2020 2020 206c 6f63 6b20 3a20 626f         lock : bo
+0000f930: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
+0000f940: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
+0000f950: 6865 7468 6572 2074 6f20 7072 6576 656e  hether to preven
+0000f960: 7420 6675 7475 7265 2073 706c 6974 732f  t future splits/
+0000f970: 6d65 7267 6573 2066 726f 6d20 616c 7465  merges from alte
+0000f980: 7269 6e67 2063 6861 6e67 6573 206d 6164  ring changes mad
+0000f990: 6520 6279 2074 6869 7320 6d65 7468 6f64  e by this method
+0000f9a0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+0000f9b0: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
+0000f9c0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
+0000f9d0: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
+0000f9e0: 7375 6c74 2e57 6869 7370 6572 5265 7375  sult.WhisperResu
+0000f9f0: 6c74 0d0a 2020 2020 2020 2020 2020 2020  lt..            
+0000fa00: 5468 6520 6375 7272 656e 7420 696e 7374  The current inst
+0000fa10: 616e 6365 2061 6674 6572 2074 6865 2063  ance after the c
+0000fa20: 6861 6e67 6573 2e0d 0a20 2020 2020 2020  hanges...       
+0000fa30: 2022 2222 0d0a 2020 2020 2020 2020 696e   """..        in
+0000fa40: 6469 6365 7320 3d20 7365 6c66 2e67 6574  dices = self.get
+0000fa50: 5f70 756e 6374 7561 7469 6f6e 5f69 6e64  _punctuation_ind
+0000fa60: 6963 6573 2870 756e 6374 7561 7469 6f6e  ices(punctuation
+0000fa70: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000fa80: 5f6d 6572 6765 5f73 6567 6d65 6e74 7328  _merge_segments(
+0000fa90: 696e 6469 6365 732c 0d0a 2020 2020 2020  indices,..      
+0000faa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fab0: 2020 2020 2020 206d 6178 5f77 6f72 6473         max_words
+0000fac0: 3d6d 6178 5f77 6f72 6473 2c20 6d61 785f  =max_words, max_
+0000fad0: 6368 6172 733d 6d61 785f 6368 6172 732c  chars=max_chars,
+0000fae0: 2069 735f 7375 6d5f 6d61 783d 6973 5f73   is_sum_max=is_s
+0000faf0: 756d 5f6d 6178 2c20 6c6f 636b 3d6c 6f63  um_max, lock=loc
+0000fb00: 6b29 0d0a 2020 2020 2020 2020 6966 2073  k)..        if s
+0000fb10: 656c 662e 5f72 6567 726f 7570 5f68 6973  elf._regroup_his
+0000fb20: 746f 7279 3a0d 0a20 2020 2020 2020 2020  tory:..         
+0000fb30: 2020 2073 656c 662e 5f72 6567 726f 7570     self._regroup
+0000fb40: 5f68 6973 746f 7279 202b 3d20 275f 270d  _history += '_'.
+0000fb50: 0a20 2020 2020 2020 2070 756e 6374 5f73  .        punct_s
+0000fb60: 7472 203d 2027 2f27 2e6a 6f69 6e28 7020  tr = '/'.join(p 
+0000fb70: 6966 2069 7369 6e73 7461 6e63 6528 702c  if isinstance(p,
+0000fb80: 2073 7472 2920 656c 7365 2027 2a27 2e6a   str) else '*'.j
+0000fb90: 6f69 6e28 7029 2066 6f72 2070 2069 6e20  oin(p) for p in 
+0000fba0: 7075 6e63 7475 6174 696f 6e29 0d0a 2020  punctuation)..  
+0000fbb0: 2020 2020 2020 7365 6c66 2e5f 7265 6772        self._regr
+0000fbc0: 6f75 705f 6869 7374 6f72 7920 2b3d 2066  oup_history += f
+0000fbd0: 276d 703d 7b70 756e 6374 5f73 7472 7d2b  'mp={punct_str}+
+0000fbe0: 7b6d 6178 5f77 6f72 6473 206f 7220 2222  {max_words or ""
+0000fbf0: 7d2b 7b6d 6178 5f63 6861 7273 206f 7220  }+{max_chars or 
+0000fc00: 2222 7d2b 7b69 6e74 2869 735f 7375 6d5f  ""}+{int(is_sum_
+0000fc10: 6d61 7829 7d2b 7b69 6e74 286c 6f63 6b29  max)}+{int(lock)
+0000fc20: 7d27 0d0a 2020 2020 2020 2020 7265 7475  }'..        retu
+0000fc30: 726e 2073 656c 660d 0a0d 0a20 2020 2064  rn self....    d
+0000fc40: 6566 206d 6572 6765 5f61 6c6c 5f73 6567  ef merge_all_seg
+0000fc50: 6d65 6e74 7328 7365 6c66 2920 2d3e 2022  ments(self) -> "
+0000fc60: 5768 6973 7065 7252 6573 756c 7422 3a0d  WhisperResult":.
+0000fc70: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0000fc80: 2020 2020 2020 4d65 7267 6520 616c 6c20        Merge all 
+0000fc90: 7365 676d 656e 7473 2069 6e74 6f20 6f6e  segments into on
+0000fca0: 6520 7365 676d 656e 742e 0d0a 0d0a 2020  e segment.....  
+0000fcb0: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
+0000fcc0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
+0000fcd0: 2020 2020 2020 2020 7374 6162 6c65 5f77          stable_w
+0000fce0: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
+0000fcf0: 6973 7065 7252 6573 756c 740d 0a20 2020  isperResult..   
+0000fd00: 2020 2020 2020 2020 2054 6865 2063 7572           The cur
+0000fd10: 7265 6e74 2069 6e73 7461 6e63 6520 6166  rent instance af
+0000fd20: 7465 7220 7468 6520 6368 616e 6765 732e  ter the changes.
+0000fd30: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0000fd40: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0000fd50: 6c66 2e73 6567 6d65 6e74 733a 0d0a 2020  lf.segments:..  
+0000fd60: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000fd70: 2073 656c 660d 0a20 2020 2020 2020 2069   self..        i
+0000fd80: 6620 7365 6c66 2e68 6173 5f77 6f72 6473  f self.has_words
+0000fd90: 3a0d 0a20 2020 2020 2020 2020 2020 206e  :..            n
+0000fda0: 6577 5f73 6567 203d 2073 656c 662e 7365  ew_seg = self.se
+0000fdb0: 676d 656e 7473 5b30 5d2e 636f 7079 2873  gments[0].copy(s
+0000fdc0: 656c 662e 616c 6c5f 776f 7264 7328 292c  elf.all_words(),
+0000fdd0: 206b 6565 705f 7265 7375 6c74 3d54 7275   keep_result=Tru
+0000fde0: 652c 2063 6f70 795f 776f 7264 733d 4661  e, copy_words=Fa
+0000fdf0: 6c73 6529 0d0a 2020 2020 2020 2020 656c  lse)..        el
+0000fe00: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000fe10: 206e 6577 5f73 6567 203d 2073 656c 662e   new_seg = self.
+0000fe20: 7365 676d 656e 7473 5b30 5d0d 0a20 2020  segments[0]..   
+0000fe30: 2020 2020 2020 2020 206e 6577 5f73 6567           new_seg
+0000fe40: 2e5f 6465 6661 756c 745f 7465 7874 202b  ._default_text +
+0000fe50: 3d20 2727 2e6a 6f69 6e28 732e 7465 7874  = ''.join(s.text
+0000fe60: 2066 6f72 2073 2069 6e20 7365 6c66 2e73   for s in self.s
+0000fe70: 6567 6d65 6e74 735b 313a 5d29 0d0a 2020  egments[1:])..  
+0000fe80: 2020 2020 2020 2020 2020 6966 2061 6c6c            if all
+0000fe90: 2873 2e74 6f6b 656e 7320 6973 206e 6f74  (s.tokens is not
+0000fea0: 204e 6f6e 6520 666f 7220 7320 696e 2073   None for s in s
+0000feb0: 656c 662e 7365 676d 656e 7473 293a 0d0a  elf.segments):..
+0000fec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fed0: 6e65 775f 7365 672e 5f64 6566 6175 6c74  new_seg._default
+0000fee0: 5f74 6f6b 656e 7320 2b3d 206c 6973 7428  _tokens += list(
+0000fef0: 6368 6169 6e2e 6672 6f6d 5f69 7465 7261  chain.from_itera
+0000ff00: 626c 6528 732e 746f 6b65 6e73 2066 6f72  ble(s.tokens for
+0000ff10: 2073 2069 6e20 7365 6c66 2e73 6567 6d65   s in self.segme
+0000ff20: 6e74 735b 313a 5d29 290d 0a20 2020 2020  nts[1:]))..     
+0000ff30: 2020 2020 2020 206e 6577 5f73 6567 2e65         new_seg.e
+0000ff40: 6e64 203d 2073 656c 662e 7365 676d 656e  nd = self.segmen
+0000ff50: 7473 5b2d 315d 2e65 6e64 0d0a 2020 2020  ts[-1].end..    
+0000ff60: 2020 2020 7365 6c66 2e73 6567 6d65 6e74      self.segment
+0000ff70: 7320 3d20 5b6e 6577 5f73 6567 5d0d 0a20  s = [new_seg].. 
+0000ff80: 2020 2020 2020 2073 656c 662e 7265 6173         self.reas
+0000ff90: 7369 676e 5f69 6473 2829 0d0a 2020 2020  sign_ids()..    
+0000ffa0: 2020 2020 6966 2073 656c 662e 5f72 6567      if self._reg
+0000ffb0: 726f 7570 5f68 6973 746f 7279 3a0d 0a20  roup_history:.. 
+0000ffc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ffd0: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
+0000ffe0: 202b 3d20 275f 270d 0a20 2020 2020 2020   += '_'..       
+0000fff0: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
+00010000: 6973 746f 7279 202b 3d20 276d 7327 0d0a  istory += 'ms'..
+00010010: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00010020: 656c 660d 0a0d 0a20 2020 2064 6566 2073  elf....    def s
+00010030: 706c 6974 5f62 795f 6c65 6e67 7468 280d  plit_by_length(.
+00010040: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010050: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
+00010060: 6d61 785f 6368 6172 733a 2069 6e74 203d  max_chars: int =
+00010070: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+00010080: 2020 2020 6d61 785f 776f 7264 733a 2069      max_words: i
+00010090: 6e74 203d 204e 6f6e 652c 0d0a 2020 2020  nt = None,..    
+000100a0: 2020 2020 2020 2020 6576 656e 5f73 706c          even_spl
+000100b0: 6974 3a20 626f 6f6c 203d 2054 7275 652c  it: bool = True,
+000100c0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+000100d0: 7263 655f 6c65 6e3a 2062 6f6f 6c20 3d20  rce_len: bool = 
+000100e0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+000100f0: 2020 2020 6c6f 636b 3a20 626f 6f6c 203d      lock: bool =
+00010100: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
+00010110: 2020 2020 2069 6e63 6c75 6465 5f6c 6f63       include_loc
+00010120: 6b3a 2062 6f6f 6c20 3d20 4661 6c73 652c  k: bool = False,
+00010130: 0d0a 2020 2020 2020 2020 2020 2020 6e65  ..            ne
+00010140: 776c 696e 653a 2062 6f6f 6c20 3d20 4661  wline: bool = Fa
+00010150: 6c73 650d 0a20 2020 2029 202d 3e20 2257  lse..    ) -> "W
+00010160: 6869 7370 6572 5265 7375 6c74 223a 0d0a  hisperResult":..
+00010170: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00010180: 2020 2020 2053 706c 6974 2028 696e 2d70       Split (in-p
+00010190: 6c61 6365 2920 616e 7920 7365 676d 656e  lace) any segmen
+000101a0: 7420 7468 6174 2065 7863 6565 6473 2060  t that exceeds `
+000101b0: 606d 6178 5f63 6861 7273 6060 206f 7220  `max_chars`` or 
+000101c0: 6060 6d61 785f 776f 7264 7360 6020 696e  ``max_words`` in
+000101d0: 746f 2073 6d61 6c6c 6572 2073 6567 6d65  to smaller segme
+000101e0: 6e74 732e 0d0a 0d0a 2020 2020 2020 2020  nts.....        
+000101f0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+00010200: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00010210: 2020 2020 2020 2020 6d61 785f 6368 6172          max_char
+00010220: 7320 3a20 696e 742c 206f 7074 696f 6e61  s : int, optiona
+00010230: 6c0d 0a20 2020 2020 2020 2020 2020 204d  l..            M
+00010240: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+00010250: 2063 6861 7261 6374 6572 7320 616c 6c6f   characters allo
+00010260: 7765 6420 696e 2065 6163 6820 7365 676d  wed in each segm
+00010270: 656e 742e 0d0a 2020 2020 2020 2020 6d61  ent...        ma
+00010280: 785f 776f 7264 7320 3a20 696e 742c 206f  x_words : int, o
+00010290: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+000102a0: 2020 2020 204d 6178 696d 756d 206e 756d       Maximum num
+000102b0: 6265 7220 6f66 2077 6f72 6473 2061 6c6c  ber of words all
+000102c0: 6f77 6564 2069 6e20 6561 6368 2073 6567  owed in each seg
+000102d0: 6d65 6e74 2e0d 0a20 2020 2020 2020 2065  ment...        e
+000102e0: 7665 6e5f 7370 6c69 7420 3a20 626f 6f6c  ven_split : bool
+000102f0: 2c20 6465 6661 756c 7420 5472 7565 0d0a  , default True..
+00010300: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+00010310: 6865 7220 746f 2065 7665 6e6c 7920 7370  her to evenly sp
+00010320: 6c69 7420 6120 7365 676d 656e 7420 696e  lit a segment in
+00010330: 206c 656e 6774 6820 6966 2069 7420 6578   length if it ex
+00010340: 6365 6564 7320 6060 6d61 785f 6368 6172  ceeds ``max_char
+00010350: 7360 6020 6f72 2060 606d 6178 5f77 6f72  s`` or ``max_wor
+00010360: 6473 6060 2e0d 0a20 2020 2020 2020 2066  ds``...        f
+00010370: 6f72 6365 5f6c 656e 203a 2062 6f6f 6c2c  orce_len : bool,
+00010380: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
+00010390: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+000103a0: 6865 7220 746f 2066 6f72 6365 2061 2063  her to force a c
+000103b0: 6f6e 7374 616e 7420 6c65 6e67 7468 2066  onstant length f
+000103c0: 6f72 2065 6163 6820 7365 676d 656e 7420  or each segment 
+000103d0: 6578 6365 7074 2074 6865 206c 6173 7420  except the last 
+000103e0: 7365 676d 656e 742e 0d0a 2020 2020 2020  segment...      
+000103f0: 2020 2020 2020 5468 6973 2077 696c 6c20        This will 
+00010400: 6967 6e6f 7265 2061 6c6c 2070 7265 7669  ignore all previ
+00010410: 6f75 7320 6e6f 6e2d 6c6f 636b 6564 2073  ous non-locked s
+00010420: 6567 6d65 6e74 2062 6f75 6e64 6172 6965  egment boundarie
+00010430: 732e 0d0a 2020 2020 2020 2020 6c6f 636b  s...        lock
+00010440: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+00010450: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00010460: 2020 2020 5768 6574 6865 7220 746f 2070      Whether to p
+00010470: 7265 7665 6e74 2066 7574 7572 6520 7370  revent future sp
+00010480: 6c69 7473 2f6d 6572 6765 7320 6672 6f6d  lits/merges from
+00010490: 2061 6c74 6572 696e 6720 6368 616e 6765   altering change
+000104a0: 7320 6d61 6465 2062 7920 7468 6973 206d  s made by this m
+000104b0: 6574 686f 642e 0d0a 2020 2020 2020 2020  ethod...        
+000104c0: 696e 636c 7564 655f 6c6f 636b 3a20 626f  include_lock: bo
+000104d0: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
+000104e0: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
+000104f0: 6865 7468 6572 2074 6f20 696e 636c 7564  hether to includ
+00010500: 6520 7072 6576 696f 7573 206c 6f63 6b20  e previous lock 
+00010510: 6265 666f 7265 2073 706c 6974 7469 6e67  before splitting
+00010520: 2062 6173 6564 206f 6e20 6d61 785f 776f   based on max_wo
+00010530: 7264 732c 2069 6620 6060 6576 656e 5f73  rds, if ``even_s
+00010540: 706c 6974 203d 2046 616c 7365 6060 2e0d  plit = False``..
+00010550: 0a20 2020 2020 2020 2020 2020 2053 706c  .            Spl
+00010560: 6974 7469 6e67 2077 696c 6c20 6265 2064  itting will be d
+00010570: 6f6e 6520 6166 7465 7220 7468 6520 6669  one after the fi
+00010580: 7273 7420 6e6f 6e2d 6c6f 636b 6564 2077  rst non-locked w
+00010590: 6f72 6420 3e20 6060 6d61 785f 6368 6172  ord > ``max_char
+000105a0: 7360 6020 2f20 6060 6d61 785f 776f 7264  s`` / ``max_word
+000105b0: 7360 602e 0d0a 2020 2020 2020 2020 6e65  s``...        ne
+000105c0: 776c 696e 653a 2062 6f6f 6c2c 2064 6566  wline: bool, def
+000105d0: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
+000105e0: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+000105f0: 746f 2069 6e73 6572 7420 6c69 6e65 2062  to insert line b
+00010600: 7265 616b 2061 7420 7468 6520 7370 6c69  reak at the spli
+00010610: 7420 706f 696e 7473 2069 6e73 7465 6164  t points instead
+00010620: 206f 6620 7370 6c69 7474 696e 6720 696e   of splitting in
+00010630: 746f 2073 6570 6172 6174 6520 7365 676d  to separate segm
+00010640: 656e 7473 2e0d 0a0d 0a20 2020 2020 2020  ents.....       
+00010650: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
+00010660: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
+00010670: 2020 2073 7461 626c 655f 7768 6973 7065     stable_whispe
+00010680: 722e 7265 7375 6c74 2e57 6869 7370 6572  r.result.Whisper
+00010690: 5265 7375 6c74 0d0a 2020 2020 2020 2020  Result..        
+000106a0: 2020 2020 5468 6520 6375 7272 656e 7420      The current 
+000106b0: 696e 7374 616e 6365 2061 6674 6572 2074  instance after t
+000106c0: 6865 2063 6861 6e67 6573 2e0d 0a0d 0a20  he changes..... 
+000106d0: 2020 2020 2020 204e 6f74 6573 0d0a 2020         Notes..  
+000106e0: 2020 2020 2020 2d2d 2d2d 2d0d 0a20 2020        -----..   
+000106f0: 2020 2020 2049 6620 6060 6576 656e 5f73       If ``even_s
+00010700: 706c 6974 203d 2054 7275 6560 602c 2073  plit = True``, s
+00010710: 6567 6d65 6e74 7320 6361 6e20 7374 696c  egments can stil
+00010720: 6c20 6578 6365 6564 2060 606d 6178 5f63  l exceed ``max_c
+00010730: 6861 7273 6060 2061 6e64 206c 6f63 6b65  hars`` and locke
+00010740: 6420 776f 7264 7320 7769 6c6c 2062 6520  d words will be 
+00010750: 6967 6e6f 7265 6420 746f 2061 766f 6964  ignored to avoid
+00010760: 0d0a 2020 2020 2020 2020 756e 6576 656e  ..        uneven
+00010770: 2073 706c 6974 7469 6e67 2e0d 0a20 2020   splitting...   
+00010780: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00010790: 2020 6966 2066 6f72 6365 5f6c 656e 3a0d    if force_len:.
+000107a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000107b0: 662e 6d65 7267 655f 616c 6c5f 7365 676d  f.merge_all_segm
+000107c0: 656e 7473 2829 0d0a 2020 2020 2020 2020  ents()..        
+000107d0: 7365 6c66 2e5f 7370 6c69 745f 7365 676d  self._split_segm
+000107e0: 656e 7473 280d 0a20 2020 2020 2020 2020  ents(..         
+000107f0: 2020 206c 616d 6264 6120 783a 2078 2e67     lambda x: x.g
+00010800: 6574 5f6c 656e 6774 685f 696e 6469 6365  et_length_indice
+00010810: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
+00010820: 2020 2020 6d61 785f 6368 6172 733d 6d61      max_chars=ma
+00010830: 785f 6368 6172 732c 0d0a 2020 2020 2020  x_chars,..      
+00010840: 2020 2020 2020 2020 2020 6d61 785f 776f            max_wo
+00010850: 7264 733d 6d61 785f 776f 7264 732c 0d0a  rds=max_words,..
+00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010870: 6576 656e 5f73 706c 6974 3d65 7665 6e5f  even_split=even_
+00010880: 7370 6c69 742c 0d0a 2020 2020 2020 2020  split,..        
+00010890: 2020 2020 2020 2020 696e 636c 7564 655f          include_
+000108a0: 6c6f 636b 3d69 6e63 6c75 6465 5f6c 6f63  lock=include_loc
+000108b0: 6b0d 0a20 2020 2020 2020 2020 2020 2029  k..            )
+000108c0: 2c0d 0a20 2020 2020 2020 2020 2020 206c  ,..            l
+000108d0: 6f63 6b3d 6c6f 636b 2c0d 0a20 2020 2020  ock=lock,..     
+000108e0: 2020 2020 2020 206e 6577 6c69 6e65 3d6e         newline=n
+000108f0: 6577 6c69 6e65 0d0a 2020 2020 2020 2020  ewline..        
+00010900: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+00010910: 6c66 2e5f 7265 6772 6f75 705f 6869 7374  lf._regroup_hist
+00010920: 6f72 793a 0d0a 2020 2020 2020 2020 2020  ory:..          
+00010930: 2020 7365 6c66 2e5f 7265 6772 6f75 705f    self._regroup_
+00010940: 6869 7374 6f72 7920 2b3d 2027 5f27 0d0a  history += '_'..
+00010950: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+00010960: 6772 6f75 705f 6869 7374 6f72 7920 2b3d  group_history +=
+00010970: 2028 6627 736c 3d7b 6d61 785f 6368 6172   (f'sl={max_char
+00010980: 7320 6f72 2022 227d 2b7b 6d61 785f 776f  s or ""}+{max_wo
+00010990: 7264 7320 6f72 2022 227d 2b7b 696e 7428  rds or ""}+{int(
+000109a0: 6576 656e 5f73 706c 6974 297d 2b7b 696e  even_split)}+{in
+000109b0: 7428 666f 7263 655f 6c65 6e29 7d27 0d0a  t(force_len)}'..
+000109c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109e0: 2020 6627 2b7b 696e 7428 6c6f 636b 297d    f'+{int(lock)}
+000109f0: 2b7b 696e 7428 696e 636c 7564 655f 6c6f  +{int(include_lo
+00010a00: 636b 297d 2b7b 696e 7428 6e65 776c 696e  ck)}+{int(newlin
+00010a10: 6529 7d27 290d 0a20 2020 2020 2020 2072  e)}')..        r
+00010a20: 6574 7572 6e20 7365 6c66 0d0a 0d0a 2020  eturn self....  
+00010a30: 2020 6465 6620 7370 6c69 745f 6279 5f64    def split_by_d
+00010a40: 7572 6174 696f 6e28 0d0a 2020 2020 2020  uration(..      
+00010a50: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+00010a60: 2020 2020 2020 2020 206d 6178 5f64 7572           max_dur
+00010a70: 3a20 666c 6f61 742c 0d0a 2020 2020 2020  : float,..      
+00010a80: 2020 2020 2020 6576 656e 5f73 706c 6974        even_split
+00010a90: 3a20 626f 6f6c 203d 2054 7275 652c 0d0a  : bool = True,..
+00010aa0: 2020 2020 2020 2020 2020 2020 666f 7263              forc
+00010ab0: 655f 6c65 6e3a 2062 6f6f 6c20 3d20 4661  e_len: bool = Fa
+00010ac0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00010ad0: 2020 6c6f 636b 3a20 626f 6f6c 203d 2046    lock: bool = F
+00010ae0: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00010af0: 2020 2069 6e63 6c75 6465 5f6c 6f63 6b3a     include_lock:
+00010b00: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
+00010b10: 2020 2020 2020 2020 2020 2020 6e65 776c              newl
+00010b20: 696e 653a 2062 6f6f 6c20 3d20 4661 6c73  ine: bool = Fals
+00010b30: 650d 0a20 2020 2029 202d 3e20 2257 6869  e..    ) -> "Whi
+00010b40: 7370 6572 5265 7375 6c74 223a 0d0a 2020  sperResult":..  
+00010b50: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00010b60: 2020 2053 706c 6974 2028 696e 2d70 6c61     Split (in-pla
+00010b70: 6365 2920 616e 7920 7365 676d 656e 7420  ce) any segment 
+00010b80: 7468 6174 2065 7863 6565 6473 2060 606d  that exceeds ``m
+00010b90: 6178 5f64 7572 6060 2069 6e74 6f20 736d  ax_dur`` into sm
+00010ba0: 616c 6c65 7220 7365 676d 656e 7473 2e0d  aller segments..
+00010bb0: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00010bc0: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
+00010bd0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
+00010be0: 2020 206d 6178 5f64 7572 203a 2066 6c6f     max_dur : flo
+00010bf0: 6174 0d0a 2020 2020 2020 2020 2020 2020  at..            
+00010c00: 4d61 7869 6d75 6d20 6475 7261 7469 6f6e  Maximum duration
+00010c10: 2028 696e 2073 6563 6f6e 6473 2920 7065   (in seconds) pe
+00010c20: 7220 7365 676d 656e 742e 0d0a 2020 2020  r segment...    
+00010c30: 2020 2020 6576 656e 5f73 706c 6974 203a      even_split :
+00010c40: 2062 6f6f 6c2c 2064 6566 6175 6c74 2054   bool, default T
+00010c50: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
+00010c60: 2057 6865 7468 6572 2074 6f20 6576 656e   Whether to even
+00010c70: 6c79 2073 706c 6974 2061 2073 6567 6d65  ly split a segme
+00010c80: 6e74 2069 6e20 6c65 6e67 7468 2069 6620  nt in length if 
+00010c90: 6974 2065 7863 6565 6473 2060 606d 6178  it exceeds ``max
+00010ca0: 5f64 7572 6060 2e0d 0a20 2020 2020 2020  _dur``...       
+00010cb0: 2066 6f72 6365 5f6c 656e 203a 2062 6f6f   force_len : boo
+00010cc0: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+00010cd0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+00010ce0: 6574 6865 7220 746f 2066 6f72 6365 2061  ether to force a
+00010cf0: 2063 6f6e 7374 616e 7420 6c65 6e67 7468   constant length
+00010d00: 2066 6f72 2065 6163 6820 7365 676d 656e   for each segmen
+00010d10: 7420 6578 6365 7074 2074 6865 206c 6173  t except the las
+00010d20: 7420 7365 676d 656e 742e 0d0a 2020 2020  t segment...    
+00010d30: 2020 2020 2020 2020 5468 6973 2077 696c          This wil
+00010d40: 6c20 6967 6e6f 7265 2061 6c6c 2070 7265  l ignore all pre
+00010d50: 7669 6f75 7320 6e6f 6e2d 6c6f 636b 6564  vious non-locked
+00010d60: 2073 6567 6d65 6e74 2062 6f75 6e64 6172   segment boundar
+00010d70: 6965 732e 0d0a 2020 2020 2020 2020 6c6f  ies...        lo
+00010d80: 636b 203a 2062 6f6f 6c2c 2064 6566 6175  ck : bool, defau
+00010d90: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
+00010da0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+00010db0: 2070 7265 7665 6e74 2066 7574 7572 6520   prevent future 
+00010dc0: 7370 6c69 7473 2f6d 6572 6765 7320 6672  splits/merges fr
+00010dd0: 6f6d 2061 6c74 6572 696e 6720 6368 616e  om altering chan
+00010de0: 6765 7320 6d61 6465 2062 7920 7468 6973  ges made by this
+00010df0: 206d 6574 686f 642e 0d0a 2020 2020 2020   method...      
+00010e00: 2020 696e 636c 7564 655f 6c6f 636b 3a20    include_lock: 
+00010e10: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
+00010e20: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+00010e30: 2057 6865 7468 6572 2074 6f20 696e 636c   Whether to incl
+00010e40: 7564 6520 7072 6576 696f 7573 206c 6f63  ude previous loc
+00010e50: 6b20 6265 666f 7265 2073 706c 6974 7469  k before splitti
+00010e60: 6e67 2062 6173 6564 206f 6e20 6d61 785f  ng based on max_
+00010e70: 776f 7264 732c 2069 6620 6060 6576 656e  words, if ``even
+00010e80: 5f73 706c 6974 203d 2046 616c 7365 6060  _split = False``
+00010e90: 2e0d 0a20 2020 2020 2020 2020 2020 2053  ...            S
+00010ea0: 706c 6974 7469 6e67 2077 696c 6c20 6265  plitting will be
+00010eb0: 2064 6f6e 6520 6166 7465 7220 7468 6520   done after the 
+00010ec0: 6669 7273 7420 6e6f 6e2d 6c6f 636b 6564  first non-locked
+00010ed0: 2077 6f72 6420 3e20 6060 6d61 785f 6475   word > ``max_du
+00010ee0: 7260 602e 0d0a 2020 2020 2020 2020 6e65  r``...        ne
+00010ef0: 776c 696e 653a 2062 6f6f 6c2c 2064 6566  wline: bool, def
+00010f00: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
+00010f10: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+00010f20: 746f 2069 6e73 6572 7420 6c69 6e65 2062  to insert line b
+00010f30: 7265 616b 2061 7420 7468 6520 7370 6c69  reak at the spli
+00010f40: 7420 706f 696e 7473 2069 6e73 7465 6164  t points instead
+00010f50: 206f 6620 7370 6c69 7474 696e 6720 696e   of splitting in
+00010f60: 746f 2073 6570 6172 6174 6520 7365 676d  to separate segm
+00010f70: 656e 7473 2e0d 0a0d 0a20 2020 2020 2020  ents.....       
+00010f80: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
+00010f90: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
+00010fa0: 2020 2073 7461 626c 655f 7768 6973 7065     stable_whispe
+00010fb0: 722e 7265 7375 6c74 2e57 6869 7370 6572  r.result.Whisper
+00010fc0: 5265 7375 6c74 0d0a 2020 2020 2020 2020  Result..        
+00010fd0: 2020 2020 5468 6520 6375 7272 656e 7420      The current 
+00010fe0: 696e 7374 616e 6365 2061 6674 6572 2074  instance after t
+00010ff0: 6865 2063 6861 6e67 6573 2e0d 0a0d 0a20  he changes..... 
+00011000: 2020 2020 2020 204e 6f74 6573 0d0a 2020         Notes..  
+00011010: 2020 2020 2020 2d2d 2d2d 2d0d 0a20 2020        -----..   
+00011020: 2020 2020 2049 6620 6060 6576 656e 5f73       If ``even_s
+00011030: 706c 6974 203d 2054 7275 6560 602c 2073  plit = True``, s
+00011040: 6567 6d65 6e74 7320 6361 6e20 7374 696c  egments can stil
+00011050: 6c20 6578 6365 6564 2060 606d 6178 5f64  l exceed ``max_d
+00011060: 7572 6060 2061 6e64 206c 6f63 6b65 6420  ur`` and locked 
+00011070: 776f 7264 7320 7769 6c6c 2062 6520 6967  words will be ig
+00011080: 6e6f 7265 6420 746f 2061 766f 6964 0d0a  nored to avoid..
+00011090: 2020 2020 2020 2020 756e 6576 656e 2073          uneven s
+000110a0: 706c 6974 7469 6e67 2e0d 0a20 2020 2020  plitting...     
+000110b0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000110c0: 6966 2066 6f72 6365 5f6c 656e 3a0d 0a20  if force_len:.. 
+000110d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000110e0: 6d65 7267 655f 616c 6c5f 7365 676d 656e  merge_all_segmen
+000110f0: 7473 2829 0d0a 2020 2020 2020 2020 7365  ts()..        se
+00011100: 6c66 2e5f 7370 6c69 745f 7365 676d 656e  lf._split_segmen
+00011110: 7473 280d 0a20 2020 2020 2020 2020 2020  ts(..           
+00011120: 206c 616d 6264 6120 783a 2078 2e67 6574   lambda x: x.get
+00011130: 5f64 7572 6174 696f 6e5f 696e 6469 6365  _duration_indice
+00011140: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
+00011150: 2020 2020 6d61 785f 6475 723d 6d61 785f      max_dur=max_
+00011160: 6475 722c 0d0a 2020 2020 2020 2020 2020  dur,..          
+00011170: 2020 2020 2020 6576 656e 5f73 706c 6974        even_split
+00011180: 3d65 7665 6e5f 7370 6c69 742c 0d0a 2020  =even_split,..  
+00011190: 2020 2020 2020 2020 2020 2020 2020 696e                in
+000111a0: 636c 7564 655f 6c6f 636b 3d69 6e63 6c75  clude_lock=inclu
+000111b0: 6465 5f6c 6f63 6b0d 0a20 2020 2020 2020  de_lock..       
+000111c0: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
+000111d0: 2020 2020 206c 6f63 6b3d 6c6f 636b 2c0d       lock=lock,.
+000111e0: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+000111f0: 6c69 6e65 3d6e 6577 6c69 6e65 0d0a 2020  line=newline..  
+00011200: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00011210: 2069 6620 7365 6c66 2e5f 7265 6772 6f75   if self._regrou
+00011220: 705f 6869 7374 6f72 793a 0d0a 2020 2020  p_history:..    
+00011230: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+00011240: 6772 6f75 705f 6869 7374 6f72 7920 2b3d  group_history +=
+00011250: 2027 5f27 0d0a 2020 2020 2020 2020 7365   '_'..        se
+00011260: 6c66 2e5f 7265 6772 6f75 705f 6869 7374  lf._regroup_hist
+00011270: 6f72 7920 2b3d 2028 6627 7364 3d7b 6d61  ory += (f'sd={ma
+00011280: 785f 6475 727d 2b7b 696e 7428 6576 656e  x_dur}+{int(even
+00011290: 5f73 706c 6974 297d 2b7b 696e 7428 666f  _split)}+{int(fo
+000112a0: 7263 655f 6c65 6e29 7d27 0d0a 2020 2020  rce_len)}'..    
+000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112c0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+000112d0: 2b7b 696e 7428 6c6f 636b 297d 2b7b 696e  +{int(lock)}+{in
+000112e0: 7428 696e 636c 7564 655f 6c6f 636b 297d  t(include_lock)}
+000112f0: 2b7b 696e 7428 6e65 776c 696e 6529 7d27  +{int(newline)}'
+00011300: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00011310: 6e20 7365 6c66 0d0a 0d0a 2020 2020 6465  n self....    de
+00011320: 6620 636c 616d 705f 6d61 7828 0d0a 2020  f clamp_max(..  
+00011330: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
+00011340: 0a20 2020 2020 2020 2020 2020 206d 6564  .            med
+00011350: 6975 6d5f 6661 6374 6f72 3a20 666c 6f61  ium_factor: floa
+00011360: 7420 3d20 322e 352c 0d0a 2020 2020 2020  t = 2.5,..      
+00011370: 2020 2020 2020 6d61 785f 6475 723a 2066        max_dur: f
+00011380: 6c6f 6174 203d 204e 6f6e 652c 0d0a 2020  loat = None,..  
+00011390: 2020 2020 2020 2020 2020 636c 6970 5f73            clip_s
+000113a0: 7461 7274 3a20 4f70 7469 6f6e 616c 5b62  tart: Optional[b
+000113b0: 6f6f 6c5d 203d 204e 6f6e 652c 0d0a 2020  ool] = None,..  
+000113c0: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
+000113d0: 653a 2062 6f6f 6c20 3d20 4661 6c73 650d  e: bool = False.
+000113e0: 0a20 2020 2029 202d 3e20 2257 6869 7370  .    ) -> "Whisp
+000113f0: 6572 5265 7375 6c74 223a 0d0a 2020 2020  erResult":..    
+00011400: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00011410: 2043 6c61 6d70 2061 6c6c 2077 6f72 6420   Clamp all word 
+00011420: 6475 7261 7469 6f6e 7320 6162 6f76 6520  durations above 
+00011430: 6365 7274 6169 6e20 7661 6c75 652e 0d0a  certain value...
+00011440: 0d0a 2020 2020 2020 2020 5468 6973 2069  ..        This i
+00011450: 7320 6d6f 7374 2065 6666 6563 7469 7665  s most effective
+00011460: 2077 6865 6e20 6170 706c 6965 6420 6265   when applied be
+00011470: 666f 7265 2061 6e64 2061 6674 6572 206f  fore and after o
+00011480: 7468 6572 2072 6567 726f 7570 206f 7065  ther regroup ope
+00011490: 7261 7469 6f6e 732e 0d0a 0d0a 2020 2020  rations.....    
+000114a0: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
+000114b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000114c0: 2d2d 0d0a 2020 2020 2020 2020 6d65 6469  --..        medi
+000114d0: 756d 5f66 6163 746f 7220 3a20 666c 6f61  um_factor : floa
+000114e0: 742c 2064 6566 6175 6c74 2032 2e35 0d0a  t, default 2.5..
+000114f0: 2020 2020 2020 2020 2020 2020 436c 616d              Clam
+00011500: 7020 6475 7261 7469 6f6e 7320 6162 6f76  p durations abov
+00011510: 6520 2860 606d 6564 6975 6d5f 6661 6374  e (``medium_fact
+00011520: 6f72 6060 202a 206d 6564 6975 6d20 6475  or`` * medium du
+00011530: 7261 7469 6f6e 2920 7065 7220 7365 676d  ration) per segm
+00011540: 656e 742e 0d0a 2020 2020 2020 2020 2020  ent...          
+00011550: 2020 4966 2060 606d 6564 6975 6d5f 6661    If ``medium_fa
+00011560: 6374 6f72 203d 204e 6f6e 652f 3060 6020  ctor = None/0`` 
+00011570: 6f72 2073 6567 6d65 6e74 2068 6173 206c  or segment has l
+00011580: 6573 7320 7468 616e 2033 2077 6f72 6473  ess than 3 words
+00011590: 2c20 6974 2077 696c 6c20 6265 2069 676e  , it will be ign
+000115a0: 6f72 6564 2061 6e64 2075 7365 206f 6e6c  ored and use onl
+000115b0: 7920 6060 6d61 785f 6475 7260 602e 0d0a  y ``max_dur``...
+000115c0: 2020 2020 2020 2020 6d61 785f 6475 7220          max_dur 
+000115d0: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
+000115e0: 6c0d 0a20 2020 2020 2020 2020 2020 2043  l..            C
+000115f0: 6c61 6d70 2064 7572 6174 696f 6e73 2061  lamp durations a
+00011600: 626f 7665 2060 606d 6178 5f64 7572 6060  bove ``max_dur``
+00011610: 2e0d 0a20 2020 2020 2020 2063 6c69 705f  ...        clip_
+00011620: 7374 6172 7420 3a20 626f 6f6c 206f 7220  start : bool or 
+00011630: 4e6f 6e65 2c20 6465 6661 756c 7420 4e6f  None, default No
+00011640: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
+00011650: 5768 6574 6865 7220 746f 2063 6c61 6d70  Whether to clamp
+00011660: 2074 6865 2073 7461 7274 206f 6620 6120   the start of a 
+00011670: 776f 7264 2e20 4966 2060 604e 6f6e 6560  word. If ``None`
+00011680: 602c 2063 6c61 6d70 2074 6865 2073 7461  `, clamp the sta
+00011690: 7274 206f 6620 6669 7273 7420 776f 7264  rt of first word
+000116a0: 2061 6e64 2065 6e64 206f 6620 6c61 7374   and end of last
+000116b0: 2077 6f72 6420 7065 720d 0a20 2020 2020   word per..     
+000116c0: 2020 2020 2020 2073 6567 6d65 6e74 2e0d         segment..
+000116d0: 0a20 2020 2020 2020 2076 6572 626f 7365  .        verbose
+000116e0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+000116f0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00011700: 2020 2020 5768 6574 6865 7220 746f 2070      Whether to p
+00011710: 7269 6e74 206f 7574 2074 6865 2074 696d  rint out the tim
+00011720: 6573 7461 6d70 2063 6861 6e67 6573 2e0d  estamp changes..
+00011730: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00011740: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
+00011750: 2d2d 2d0d 0a20 2020 2020 2020 2073 7461  ---..        sta
+00011760: 626c 655f 7768 6973 7065 722e 7265 7375  ble_whisper.resu
+00011770: 6c74 2e57 6869 7370 6572 5265 7375 6c74  lt.WhisperResult
+00011780: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00011790: 6520 6375 7272 656e 7420 696e 7374 616e  e current instan
+000117a0: 6365 2061 6674 6572 2074 6865 2063 6861  ce after the cha
+000117b0: 6e67 6573 2e0d 0a20 2020 2020 2020 2022  nges...        "
+000117c0: 2222 0d0a 2020 2020 2020 2020 6966 206e  ""..        if n
+000117d0: 6f74 2028 6d65 6469 756d 5f66 6163 746f  ot (medium_facto
+000117e0: 7220 6f72 206d 6178 5f64 7572 293a 0d0a  r or max_dur):..
+000117f0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00011800: 6520 5661 6c75 6545 7272 6f72 2827 4174  e ValueError('At
+00011810: 206c 6561 7374 206f 6e65 206f 6620 666f   least one of fo
+00011820: 6c6c 6f77 696e 6720 6172 6775 6d65 6e74  llowing argument
+00011830: 7320 7265 7175 6972 6573 206e 6f6e 2d7a  s requires non-z
+00011840: 6572 6f20 7661 6c75 653a 206d 6564 6975  ero value: mediu
+00011850: 6d5f 6661 6374 6f72 3b20 6d61 785f 6475  m_factor; max_du
+00011860: 7227 290d 0a0d 0a20 2020 2020 2020 2069  r')....        i
+00011870: 6620 6e6f 7420 7365 6c66 2e68 6173 5f77  f not self.has_w
+00011880: 6f72 6473 3a0d 0a20 2020 2020 2020 2020  ords:..         
+00011890: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
+000118a0: 2827 4361 6e6e 6f74 2063 6c61 6d70 2064  ('Cannot clamp d
+000118b0: 7565 2074 6f20 6d69 7373 696e 672f 6e6f  ue to missing/no
+000118c0: 2077 6f72 642d 7469 6d65 7374 616d 7073   word-timestamps
+000118d0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+000118e0: 7265 7475 726e 2073 656c 660d 0a0d 0a20  return self.... 
+000118f0: 2020 2020 2020 2066 6f72 2073 6567 2069         for seg i
+00011900: 6e20 7365 6c66 2e73 6567 6d65 6e74 733a  n self.segments:
+00011910: 0d0a 2020 2020 2020 2020 2020 2020 6375  ..            cu
+00011920: 7272 5f6d 6178 5f64 7572 203d 204e 6f6e  rr_max_dur = Non
+00011930: 650d 0a20 2020 2020 2020 2020 2020 2069  e..            i
+00011940: 6620 6d65 6469 756d 5f66 6163 746f 7220  f medium_factor 
+00011950: 616e 6420 6c65 6e28 7365 672e 776f 7264  and len(seg.word
+00011960: 7329 203e 2032 3a0d 0a20 2020 2020 2020  s) > 2:..       
+00011970: 2020 2020 2020 2020 2064 7572 6174 696f           duratio
+00011980: 6e73 203d 206e 702e 6172 7261 7928 5b77  ns = np.array([w
+00011990: 6f72 642e 6475 7261 7469 6f6e 2066 6f72  ord.duration for
+000119a0: 2077 6f72 6420 696e 2073 6567 2e77 6f72   word in seg.wor
+000119b0: 6473 5d29 0d0a 2020 2020 2020 2020 2020  ds])..          
+000119c0: 2020 2020 2020 6475 7261 7469 6f6e 732e        durations.
+000119d0: 736f 7274 2829 0d0a 2020 2020 2020 2020  sort()..        
+000119e0: 2020 2020 2020 2020 6375 7272 5f6d 6178          curr_max
+000119f0: 5f64 7572 203d 206d 6564 6975 6d5f 6661  _dur = medium_fa
+00011a00: 6374 6f72 202a 2064 7572 6174 696f 6e73  ctor * durations
+00011a10: 5b6c 656e 2864 7572 6174 696f 6e73 292f  [len(durations)/
+00011a20: 2f32 202b 2031 5d0d 0a0d 0a20 2020 2020  /2 + 1]....     
+00011a30: 2020 2020 2020 2069 6620 6d61 785f 6475         if max_du
+00011a40: 7220 616e 6420 286e 6f74 2063 7572 725f  r and (not curr_
+00011a50: 6d61 785f 6475 7220 6f72 2063 7572 725f  max_dur or curr_
+00011a60: 6d61 785f 6475 7220 3e20 6d61 785f 6475  max_dur > max_du
+00011a70: 7229 3a0d 0a20 2020 2020 2020 2020 2020  r):..           
+00011a80: 2020 2020 2063 7572 725f 6d61 785f 6475       curr_max_du
+00011a90: 7220 3d20 6d61 785f 6475 720d 0a0d 0a20  r = max_dur.... 
+00011aa0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00011ab0: 7420 6375 7272 5f6d 6178 5f64 7572 3a0d  t curr_max_dur:.
+00011ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011ad0: 2063 6f6e 7469 6e75 650d 0a0d 0a20 2020   continue....   
+00011ae0: 2020 2020 2020 2020 2069 6620 636c 6970           if clip
+00011af0: 5f73 7461 7274 2069 7320 4e6f 6e65 3a0d  _start is None:.
+00011b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011b10: 2073 6567 2e77 6f72 6473 5b30 5d2e 636c   seg.words[0].cl
+00011b20: 616d 705f 6d61 7828 6375 7272 5f6d 6178  amp_max(curr_max
+00011b30: 5f64 7572 2c20 636c 6970 5f73 7461 7274  _dur, clip_start
+00011b40: 3d54 7275 652c 2076 6572 626f 7365 3d76  =True, verbose=v
+00011b50: 6572 626f 7365 290d 0a20 2020 2020 2020  erbose)..       
+00011b60: 2020 2020 2020 2020 2073 6567 2e77 6f72           seg.wor
+00011b70: 6473 5b2d 315d 2e63 6c61 6d70 5f6d 6178  ds[-1].clamp_max
+00011b80: 2863 7572 725f 6d61 785f 6475 722c 2063  (curr_max_dur, c
+00011b90: 6c69 705f 7374 6172 743d 4661 6c73 652c  lip_start=False,
+00011ba0: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
+00011bb0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00011bc0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00011bd0: 2020 2020 2020 666f 7220 692c 2077 6f72        for i, wor
+00011be0: 6420 696e 2065 6e75 6d65 7261 7465 2873  d in enumerate(s
+00011bf0: 6567 2e77 6f72 6473 293a 0d0a 2020 2020  eg.words):..    
+00011c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c10: 776f 7264 2e63 6c61 6d70 5f6d 6178 2863  word.clamp_max(c
+00011c20: 7572 725f 6d61 785f 6475 722c 2063 6c69  urr_max_dur, cli
+00011c30: 705f 7374 6172 743d 636c 6970 5f73 7461  p_start=clip_sta
+00011c40: 7274 2c20 7665 7262 6f73 653d 7665 7262  rt, verbose=verb
+00011c50: 6f73 6529 0d0a 0d0a 2020 2020 2020 2020  ose)....        
+00011c60: 6966 2073 656c 662e 5f72 6567 726f 7570  if self._regroup
+00011c70: 5f68 6973 746f 7279 3a0d 0a20 2020 2020  _history:..     
+00011c80: 2020 2020 2020 2073 656c 662e 5f72 6567         self._reg
+00011c90: 726f 7570 5f68 6973 746f 7279 202b 3d20  roup_history += 
+00011ca0: 275f 270d 0a20 2020 2020 2020 2073 656c  '_'..        sel
+00011cb0: 662e 5f72 6567 726f 7570 5f68 6973 746f  f._regroup_histo
+00011cc0: 7279 202b 3d20 6627 636d 3d7b 6d65 6469  ry += f'cm={medi
+00011cd0: 756d 5f66 6163 746f 727d 2b7b 6d61 785f  um_factor}+{max_
+00011ce0: 6475 7220 6f72 2022 227d 2b7b 636c 6970  dur or ""}+{clip
+00011cf0: 5f73 7461 7274 206f 7220 2222 7d2b 7b69  _start or ""}+{i
+00011d00: 6e74 2876 6572 626f 7365 297d 270d 0a20  nt(verbose)}'.. 
+00011d10: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00011d20: 6c66 0d0a 0d0a 2020 2020 6465 6620 6c6f  lf....    def lo
+00011d30: 636b 280d 0a20 2020 2020 2020 2020 2020  ck(..           
+00011d40: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
+00011d50: 2020 2020 7374 6172 7473 7769 7468 3a20      startswith: 
+00011d60: 556e 696f 6e5b 7374 722c 204c 6973 745b  Union[str, List[
+00011d70: 7374 725d 5d20 3d20 4e6f 6e65 2c0d 0a20  str]] = None,.. 
+00011d80: 2020 2020 2020 2020 2020 2065 6e64 7377             endsw
+00011d90: 6974 683a 2055 6e69 6f6e 5b73 7472 2c20  ith: Union[str, 
+00011da0: 4c69 7374 5b73 7472 5d5d 203d 204e 6f6e  List[str]] = Non
+00011db0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00011dc0: 7269 6768 743a 2062 6f6f 6c20 3d20 5472  right: bool = Tr
+00011dd0: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00011de0: 206c 6566 743a 2062 6f6f 6c20 3d20 4661   left: bool = Fa
+00011df0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00011e00: 2020 6361 7365 5f73 656e 7369 7469 7665    case_sensitive
+00011e10: 3a20 626f 6f6c 203d 2046 616c 7365 2c0d  : bool = False,.
+00011e20: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00011e30: 6970 3a20 626f 6f6c 203d 2054 7275 650d  ip: bool = True.
+00011e40: 0a20 2020 2029 202d 3e20 2257 6869 7370  .    ) -> "Whisp
+00011e50: 6572 5265 7375 6c74 223a 0d0a 2020 2020  erResult":..    
+00011e60: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00011e70: 204c 6f63 6b20 776f 7264 732f 7365 676d   Lock words/segm
+00011e80: 656e 7473 2077 6974 6820 6d61 7463 6869  ents with matchi
+00011e90: 6e67 2070 7265 6669 782f 7375 6666 6978  ng prefix/suffix
+00011ea0: 2074 6f20 7072 6576 656e 7420 7370 6c69   to prevent spli
+00011eb0: 7474 696e 672f 6d65 7267 696e 672e 0d0a  tting/merging...
+00011ec0: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00011ed0: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
+00011ee0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
+00011ef0: 2020 7374 6172 7473 7769 7468 3a20 7374    startswith: st
+00011f00: 7220 6f72 206c 6973 7420 6f66 2073 7472  r or list of str
+00011f10: 0d0a 2020 2020 2020 2020 2020 2020 5072  ..            Pr
+00011f20: 6566 6978 6573 2074 6f20 6c6f 636b 2e0d  efixes to lock..
+00011f30: 0a20 2020 2020 2020 2065 6e64 7377 6974  .        endswit
+00011f40: 683a 2073 7472 206f 7220 6c69 7374 206f  h: str or list o
+00011f50: 6620 7374 720d 0a20 2020 2020 2020 2020  f str..         
+00011f60: 2020 2053 7566 6669 7865 7320 746f 206c     Suffixes to l
+00011f70: 6f63 6b2e 0d0a 2020 2020 2020 2020 7269  ock...        ri
+00011f80: 6768 7420 3a20 626f 6f6c 2c20 6465 6661  ght : bool, defa
+00011f90: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
+00011fa0: 2020 2020 2020 5768 6574 6865 7220 7072        Whether pr
+00011fb0: 6576 656e 7420 7370 6c69 7473 2f6d 6572  event splits/mer
+00011fc0: 6765 7320 7769 7468 2074 6865 206e 6578  ges with the nex
+00011fd0: 7420 776f 7264 2f73 6567 6d65 6e74 2e0d  t word/segment..
+00011fe0: 0a20 2020 2020 2020 206c 6566 7420 3a20  .        left : 
+00011ff0: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
+00012000: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+00012010: 2057 6865 7468 6572 2070 7265 7665 6e74   Whether prevent
+00012020: 2073 706c 6974 732f 6d65 7267 6573 2077   splits/merges w
+00012030: 6974 6820 7468 6520 7072 6576 696f 7573  ith the previous
+00012040: 2077 6f72 642f 7365 676d 656e 742e 0d0a   word/segment...
+00012050: 2020 2020 2020 2020 6361 7365 5f73 656e          case_sen
+00012060: 7369 7469 7665 203a 2062 6f6f 6c2c 2064  sitive : bool, d
+00012070: 6566 6175 6c74 2046 616c 7365 0d0a 2020  efault False..  
+00012080: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
+00012090: 7220 746f 206d 6174 6368 2074 6865 2063  r to match the c
+000120a0: 6173 6520 6f66 2074 6865 2070 7265 6669  ase of the prefi
+000120b0: 7865 732f 7375 6666 6978 6573 2077 6974  xes/suffixes wit
+000120c0: 6820 7468 6520 776f 7264 732f 7365 676d  h the words/segm
+000120d0: 656e 7473 2e0d 0a20 2020 2020 2020 2073  ents...        s
+000120e0: 7472 6970 203a 2062 6f6f 6c2c 2064 6566  trip : bool, def
+000120f0: 6175 6c74 2054 7275 650d 0a20 2020 2020  ault True..     
+00012100: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
+00012110: 6f20 6967 6e6f 7265 2073 7061 6365 7320  o ignore spaces 
+00012120: 6265 666f 7265 2061 6e64 2061 6674 6572  before and after
+00012130: 2062 6f74 6820 776f 7264 732f 7365 676d   both words/segm
+00012140: 656e 7473 2061 6e64 2070 7265 6669 7865  ents and prefixe
+00012150: 732f 7375 6666 6978 6573 2e0d 0a0d 0a20  s/suffixes..... 
+00012160: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
+00012170: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
+00012180: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
+00012190: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
+000121a0: 6869 7370 6572 5265 7375 6c74 0d0a 2020  hisperResult..  
+000121b0: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
+000121c0: 7272 656e 7420 696e 7374 616e 6365 2061  rrent instance a
+000121d0: 6674 6572 2074 6865 2063 6861 6e67 6573  fter the changes
+000121e0: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+000121f0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+00012200: 7461 7274 7377 6974 6820 6f72 2065 6e64  tartswith or end
+00012210: 7377 6974 682c 2027 4d75 7374 2073 7065  swith, 'Must spe
+00012220: 6369 6679 205b 7374 6172 7473 7769 7468  cify [startswith
+00012230: 5d20 6f72 2f61 6e64 205b 656e 6473 7769  ] or/and [endswi
+00012240: 7468 5d2e 270d 0a20 2020 2020 2020 2073  th].'..        s
+00012250: 7461 7274 7377 6974 6820 3d20 5b5d 2069  tartswith = [] i
+00012260: 6620 7374 6172 7473 7769 7468 2069 7320  f startswith is 
+00012270: 4e6f 6e65 2065 6c73 6520 285b 7374 6172  None else ([star
+00012280: 7473 7769 7468 5d20 6966 2069 7369 6e73  tswith] if isins
+00012290: 7461 6e63 6528 7374 6172 7473 7769 7468  tance(startswith
+000122a0: 2c20 7374 7229 2065 6c73 6520 7374 6172  , str) else star
+000122b0: 7473 7769 7468 290d 0a20 2020 2020 2020  tswith)..       
+000122c0: 2065 6e64 7377 6974 6820 3d20 5b5d 2069   endswith = [] i
+000122d0: 6620 656e 6473 7769 7468 2069 7320 4e6f  f endswith is No
+000122e0: 6e65 2065 6c73 6520 285b 656e 6473 7769  ne else ([endswi
+000122f0: 7468 5d20 6966 2069 7369 6e73 7461 6e63  th] if isinstanc
+00012300: 6528 656e 6473 7769 7468 2c20 7374 7229  e(endswith, str)
+00012310: 2065 6c73 6520 656e 6473 7769 7468 290d   else endswith).
+00012320: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00012330: 6361 7365 5f73 656e 7369 7469 7665 3a0d  case_sensitive:.
+00012340: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00012350: 7274 7377 6974 6820 3d20 5b74 2e6c 6f77  rtswith = [t.low
+00012360: 6572 2829 2066 6f72 2074 2069 6e20 7374  er() for t in st
+00012370: 6172 7473 7769 7468 5d0d 0a20 2020 2020  artswith]..     
+00012380: 2020 2020 2020 2065 6e64 7377 6974 6820         endswith 
+00012390: 3d20 5b74 2e6c 6f77 6572 2829 2066 6f72  = [t.lower() for
+000123a0: 2074 2069 6e20 656e 6473 7769 7468 5d0d   t in endswith].
+000123b0: 0a20 2020 2020 2020 2069 6620 7374 7269  .        if stri
+000123c0: 703a 0d0a 2020 2020 2020 2020 2020 2020  p:..            
+000123d0: 7374 6172 7473 7769 7468 203d 205b 742e  startswith = [t.
+000123e0: 7374 7269 7028 2920 666f 7220 7420 696e  strip() for t in
+000123f0: 2073 7461 7274 7377 6974 685d 0d0a 2020   startswith]..  
+00012400: 2020 2020 2020 2020 2020 656e 6473 7769            endswi
+00012410: 7468 203d 205b 742e 7374 7269 7028 2920  th = [t.strip() 
+00012420: 666f 7220 7420 696e 2065 6e64 7377 6974  for t in endswit
+00012430: 685d 0d0a 2020 2020 2020 2020 666f 7220  h]..        for 
+00012440: 7061 7274 2069 6e20 7365 6c66 2e61 6c6c  part in self.all
+00012450: 5f77 6f72 6473 5f6f 725f 7365 676d 656e  _words_or_segmen
+00012460: 7473 2829 3a0d 0a20 2020 2020 2020 2020  ts():..         
+00012470: 2020 2074 6578 7420 3d20 7061 7274 2e77     text = part.w
+00012480: 6f72 6420 6966 2068 6173 6174 7472 2870  ord if hasattr(p
+00012490: 6172 742c 2027 776f 7264 2729 2065 6c73  art, 'word') els
+000124a0: 6520 7061 7274 2e74 6578 740d 0a20 2020  e part.text..   
+000124b0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000124c0: 6361 7365 5f73 656e 7369 7469 7665 3a0d  case_sensitive:.
+000124d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000124e0: 2074 6578 7420 3d20 7465 7874 2e6c 6f77   text = text.low
+000124f0: 6572 2829 0d0a 2020 2020 2020 2020 2020  er()..          
+00012500: 2020 6966 2073 7472 6970 3a0d 0a20 2020    if strip:..   
+00012510: 2020 2020 2020 2020 2020 2020 2074 6578               tex
+00012520: 7420 3d20 7465 7874 2e73 7472 6970 2829  t = text.strip()
+00012530: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00012540: 7220 7072 6566 6978 2069 6e20 7374 6172  r prefix in star
+00012550: 7473 7769 7468 3a0d 0a20 2020 2020 2020  tswith:..       
+00012560: 2020 2020 2020 2020 2069 6620 7465 7874           if text
+00012570: 2e73 7461 7274 7377 6974 6828 7072 6566  .startswith(pref
+00012580: 6978 293a 0d0a 2020 2020 2020 2020 2020  ix):..          
+00012590: 2020 2020 2020 2020 2020 6966 2072 6967            if rig
+000125a0: 6874 3a0d 0a20 2020 2020 2020 2020 2020  ht:..           
+000125b0: 2020 2020 2020 2020 2020 2020 2070 6172               par
+000125c0: 742e 6c6f 636b 5f72 6967 6874 2829 0d0a  t.lock_right()..
+000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125e0: 2020 2020 6966 206c 6566 743a 0d0a 2020      if left:..  
+000125f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012600: 2020 2020 2020 7061 7274 2e6c 6f63 6b5f        part.lock_
+00012610: 6c65 6674 2829 0d0a 2020 2020 2020 2020  left()..        
+00012620: 2020 2020 666f 7220 7375 6666 6978 2069      for suffix i
+00012630: 6e20 656e 6473 7769 7468 3a0d 0a20 2020  n endswith:..   
+00012640: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00012650: 7465 7874 2e65 6e64 7377 6974 6828 7375  text.endswith(su
+00012660: 6666 6978 293a 0d0a 2020 2020 2020 2020  ffix):..        
+00012670: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00012680: 6967 6874 3a0d 0a20 2020 2020 2020 2020  ight:..         
+00012690: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000126a0: 6172 742e 6c6f 636b 5f72 6967 6874 2829  art.lock_right()
+000126b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000126c0: 2020 2020 2020 6966 206c 6566 743a 0d0a        if left:..
+000126d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126e0: 2020 2020 2020 2020 7061 7274 2e6c 6f63          part.loc
+000126f0: 6b5f 6c65 6674 2829 0d0a 2020 2020 2020  k_left()..      
+00012700: 2020 6966 2073 656c 662e 5f72 6567 726f    if self._regro
+00012710: 7570 5f68 6973 746f 7279 3a0d 0a20 2020  up_history:..   
+00012720: 2020 2020 2020 2020 2073 656c 662e 5f72           self._r
+00012730: 6567 726f 7570 5f68 6973 746f 7279 202b  egroup_history +
+00012740: 3d20 275f 270d 0a20 2020 2020 2020 2073  = '_'..        s
+00012750: 7461 7274 7377 6974 685f 7374 7220 3d20  tartswith_str = 
+00012760: 2873 7461 7274 7377 6974 6820 6966 2069  (startswith if i
+00012770: 7369 6e73 7461 6e63 6528 7374 6172 7473  sinstance(starts
+00012780: 7769 7468 2c20 7374 7229 2065 6c73 6520  with, str) else 
+00012790: 272f 272e 6a6f 696e 2873 7461 7274 7377  '/'.join(startsw
+000127a0: 6974 6829 2920 6966 2073 7461 7274 7377  ith)) if startsw
+000127b0: 6974 6820 656c 7365 2022 220d 0a20 2020  ith else ""..   
+000127c0: 2020 2020 2065 6e64 7377 6974 685f 7374       endswith_st
+000127d0: 7220 3d20 2865 6e64 7377 6974 6820 6966  r = (endswith if
+000127e0: 2069 7369 6e73 7461 6e63 6528 656e 6473   isinstance(ends
+000127f0: 7769 7468 2c20 7374 7229 2065 6c73 6520  with, str) else 
+00012800: 272f 272e 6a6f 696e 2865 6e64 7377 6974  '/'.join(endswit
+00012810: 6829 2920 6966 2065 6e64 7377 6974 6820  h)) if endswith 
+00012820: 656c 7365 2022 220d 0a20 2020 2020 2020  else ""..       
+00012830: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
+00012840: 6973 746f 7279 202b 3d20 2866 276c 3d7b  istory += (f'l={
+00012850: 7374 6172 7473 7769 7468 5f73 7472 7d2b  startswith_str}+
+00012860: 7b65 6e64 7377 6974 685f 7374 727d 270d  {endswith_str}'.
+00012870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012890: 2020 2066 272b 7b69 6e74 2872 6967 6874     f'+{int(right
+000128a0: 297d 2b7b 696e 7428 6c65 6674 297d 2b7b  )}+{int(left)}+{
+000128b0: 696e 7428 6361 7365 5f73 656e 7369 7469  int(case_sensiti
+000128c0: 7665 297d 2b7b 696e 7428 7374 7269 7029  ve)}+{int(strip)
+000128d0: 7d27 290d 0a20 2020 2020 2020 2072 6574  }')..        ret
+000128e0: 7572 6e20 7365 6c66 0d0a 0d0a 2020 2020  urn self....    
+000128f0: 6465 6620 7265 6d6f 7665 5f77 6f72 6428  def remove_word(
+00012900: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00012910: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
+00012920: 2077 6f72 643a 2055 6e69 6f6e 5b57 6f72   word: Union[Wor
+00012930: 6454 696d 696e 672c 2054 7570 6c65 5b69  dTiming, Tuple[i
+00012940: 6e74 2c20 696e 745d 5d2c 0d0a 2020 2020  nt, int]],..    
+00012950: 2020 2020 2020 2020 7265 6173 7369 676e          reassign
+00012960: 5f69 6473 3a20 626f 6f6c 203d 2054 7275  _ids: bool = Tru
+00012970: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00012980: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
+00012990: 5472 7565 0d0a 2020 2020 2920 2d3e 2027  True..    ) -> '
+000129a0: 5768 6973 7065 7252 6573 756c 7427 3a0d  WhisperResult':.
+000129b0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000129c0: 2020 2020 2020 5265 6d6f 7665 2061 2077        Remove a w
+000129d0: 6f72 642e 0d0a 0d0a 2020 2020 2020 2020  ord.....        
+000129e0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+000129f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00012a00: 2020 2020 2020 2020 776f 7264 203a 2057          word : W
+00012a10: 6f72 6454 696d 696e 6720 6f72 2074 7570  ordTiming or tup
+00012a20: 6c65 206f 6620 2869 6e74 2c20 696e 7429  le of (int, int)
+00012a30: 0d0a 2020 2020 2020 2020 2020 2020 496e  ..            In
+00012a40: 7374 616e 6365 206f 6620 3a63 6c61 7373  stance of :class
+00012a50: 3a60 7374 6162 6c65 5f77 6869 7370 6572  :`stable_whisper
+00012a60: 2e72 6573 756c 742e 576f 7264 5469 6d69  .result.WordTimi
+00012a70: 6e67 6020 6f72 2074 7570 6c65 206f 6620  ng` or tuple of 
+00012a80: 2873 6567 6d65 6e74 2069 6e64 6578 2c20  (segment index, 
+00012a90: 776f 7264 2069 6e64 6578 292e 0d0a 2020  word index)...  
+00012aa0: 2020 2020 2020 7265 6173 7369 676e 5f69        reassign_i
+00012ab0: 6473 203a 2062 6f6f 6c2c 2064 6566 6175  ds : bool, defau
+00012ac0: 6c74 2054 7275 650d 0a20 2020 2020 2020  lt True..       
+00012ad0: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
+00012ae0: 7265 6173 7369 676e 2073 6567 6d65 6e74  reassign segment
+00012af0: 2061 6e64 2077 6f72 6420 6964 7320 2869   and word ids (i
+00012b00: 6e64 6963 6573 2920 6166 7465 7220 7265  ndices) after re
+00012b10: 6d6f 7669 6e67 2060 6077 6f72 6460 602e  moving ``word``.
+00012b20: 0d0a 2020 2020 2020 2020 7665 7262 6f73  ..        verbos
+00012b30: 6520 3a20 626f 6f6c 2c20 6465 6661 756c  e : bool, defaul
+00012b40: 7420 5472 7565 0d0a 2020 2020 2020 2020  t True..        
+00012b50: 2020 2020 5768 6574 6865 7220 746f 2070      Whether to p
+00012b60: 7269 6e74 2064 6574 6169 6c20 6f66 2074  rint detail of t
+00012b70: 6865 2072 656d 6f76 6564 2077 6f72 642e  he removed word.
+00012b80: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00012b90: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
+00012ba0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7374  ----..        st
+00012bb0: 6162 6c65 5f77 6869 7370 6572 2e72 6573  able_whisper.res
+00012bc0: 756c 742e 5768 6973 7065 7252 6573 756c  ult.WhisperResul
+00012bd0: 740d 0a20 2020 2020 2020 2020 2020 2054  t..            T
+00012be0: 6865 2063 7572 7265 6e74 2069 6e73 7461  he current insta
+00012bf0: 6e63 6520 6166 7465 7220 7468 6520 6368  nce after the ch
+00012c00: 616e 6765 732e 0d0a 2020 2020 2020 2020  anges...        
+00012c10: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
+00012c20: 6973 696e 7374 616e 6365 2877 6f72 642c  isinstance(word,
+00012c30: 2057 6f72 6454 696d 696e 6729 3a0d 0a20   WordTiming):.. 
+00012c40: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00012c50: 6c66 5b77 6f72 642e 7365 676d 656e 745f  lf[word.segment_
+00012c60: 6964 5d5b 776f 7264 2e69 645d 2069 7320  id][word.id] is 
+00012c70: 6e6f 7420 776f 7264 3a0d 0a20 2020 2020  not word:..     
+00012c80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012c90: 7265 6173 7369 676e 5f69 6473 2829 0d0a  reassign_ids()..
+00012ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cb0: 6966 2073 656c 665b 776f 7264 2e73 6567  if self[word.seg
+00012cc0: 6d65 6e74 5f69 645d 5b77 6f72 642e 6964  ment_id][word.id
+00012cd0: 5d20 6973 206e 6f74 2077 6f72 643a 0d0a  ] is not word:..
+00012ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cf0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00012d00: 7272 6f72 2827 776f 7264 206e 6f74 2069  rror('word not i
+00012d10: 6e20 7265 7375 6c74 2729 0d0a 2020 2020  n result')..    
+00012d20: 2020 2020 2020 2020 7365 675f 6964 2c20          seg_id, 
+00012d30: 776f 7264 5f69 6420 3d20 776f 7264 2e73  word_id = word.s
+00012d40: 6567 6d65 6e74 5f69 642c 2077 6f72 642e  egment_id, word.
+00012d50: 6964 0d0a 2020 2020 2020 2020 656c 7365  id..        else
+00012d60: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00012d70: 6567 5f69 642c 2077 6f72 645f 6964 203d  eg_id, word_id =
+00012d80: 2077 6f72 640d 0a20 2020 2020 2020 2069   word..        i
+00012d90: 6620 7665 7262 6f73 653a 0d0a 2020 2020  f verbose:..    
+00012da0: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+00012db0: 5265 6d6f 7665 643a 207b 7365 6c66 5b73  Removed: {self[s
+00012dc0: 6567 5f69 645d 5b77 6f72 645f 6964 5d2e  eg_id][word_id].
+00012dd0: 746f 5f64 6963 7428 297d 2729 0d0a 2020  to_dict()}')..  
+00012de0: 2020 2020 2020 6465 6c20 7365 6c66 2e73        del self.s
+00012df0: 6567 6d65 6e74 735b 7365 675f 6964 5d2e  egments[seg_id].
+00012e00: 776f 7264 735b 776f 7264 5f69 645d 0d0a  words[word_id]..
+00012e10: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+00012e20: 6561 7373 6967 6e5f 6964 733a 0d0a 2020  eassign_ids:..  
+00012e30: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00012e40: 2073 656c 660d 0a20 2020 2020 2020 2069   self..        i
+00012e50: 6620 7365 6c66 5b73 6567 5f69 645d 2e68  f self[seg_id].h
+00012e60: 6173 5f77 6f72 6473 3a0d 0a20 2020 2020  as_words:..     
+00012e70: 2020 2020 2020 2073 656c 665b 7365 675f         self[seg_
+00012e80: 6964 5d2e 7265 6173 7369 676e 5f69 6473  id].reassign_ids
+00012e90: 2829 0d0a 2020 2020 2020 2020 656c 7365  ()..        else
+00012ea0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00012eb0: 656c 662e 7265 6d6f 7665 5f6e 6f5f 776f  elf.remove_no_wo
+00012ec0: 7264 5f73 6567 6d65 6e74 7328 290d 0a20  rd_segments().. 
+00012ed0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00012ee0: 6c66 0d0a 0d0a 2020 2020 6465 6620 7265  lf....    def re
+00012ef0: 6d6f 7665 5f73 6567 6d65 6e74 280d 0a20  move_segment(.. 
+00012f00: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00012f10: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00012f20: 676d 656e 743a 2055 6e69 6f6e 5b53 6567  gment: Union[Seg
+00012f30: 6d65 6e74 2c20 696e 745d 2c0d 0a20 2020  ment, int],..   
+00012f40: 2020 2020 2020 2020 2072 6561 7373 6967           reassig
+00012f50: 6e5f 6964 733a 2062 6f6f 6c20 3d20 5472  n_ids: bool = Tr
+00012f60: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00012f70: 2076 6572 626f 7365 3a20 626f 6f6c 203d   verbose: bool =
+00012f80: 2054 7275 650d 0a20 2020 2029 202d 3e20   True..    ) -> 
+00012f90: 2757 6869 7370 6572 5265 7375 6c74 273a  'WhisperResult':
+00012fa0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00012fb0: 2020 2020 2020 2052 656d 6f76 6520 6120         Remove a 
+00012fc0: 7365 676d 656e 742e 0d0a 0d0a 2020 2020  segment.....    
+00012fd0: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
+00012fe0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00012ff0: 2d2d 0d0a 2020 2020 2020 2020 7365 676d  --..        segm
+00013000: 656e 7420 3a20 5365 676d 656e 7420 6f72  ent : Segment or
+00013010: 2069 6e74 0d0a 2020 2020 2020 2020 2020   int..          
+00013020: 2020 496e 7374 616e 6365 203a 636c 6173    Instance :clas
+00013030: 733a 6073 7461 626c 655f 7768 6973 7065  s:`stable_whispe
+00013040: 722e 7265 7375 6c74 2e53 6567 6d65 6e74  r.result.Segment
+00013050: 6020 6f72 2073 6567 6d65 6e74 2069 6e64  ` or segment ind
+00013060: 6578 2e0d 0a20 2020 2020 2020 2072 6561  ex...        rea
+00013070: 7373 6967 6e5f 6964 7320 3a20 626f 6f6c  ssign_ids : bool
+00013080: 2c20 6465 6661 756c 7420 5472 7565 0d0a  , default True..
+00013090: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+000130a0: 6865 7220 746f 2072 6561 7373 6967 6e20  her to reassign 
+000130b0: 7365 676d 656e 7420 4944 7320 2869 6e64  segment IDs (ind
+000130c0: 6963 6573 2920 6166 7465 7220 7265 6d6f  ices) after remo
+000130d0: 7669 6e67 2060 6073 6567 6d65 6e74 6060  ving ``segment``
+000130e0: 2e0d 0a20 2020 2020 2020 2076 6572 626f  ...        verbo
+000130f0: 7365 203a 2062 6f6f 6c2c 2064 6566 6175  se : bool, defau
+00013100: 6c74 2054 7275 650d 0a20 2020 2020 2020  lt True..       
+00013110: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
+00013120: 7072 696e 7420 6465 7461 696c 206f 6620  print detail of 
+00013130: 7468 6520 7265 6d6f 7665 6420 776f 7264  the removed word
+00013140: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+00013150: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
+00013160: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
+00013170: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
+00013180: 7375 6c74 2e57 6869 7370 6572 5265 7375  sult.WhisperResu
+00013190: 6c74 0d0a 2020 2020 2020 2020 2020 2020  lt..            
+000131a0: 5468 6520 6375 7272 656e 7420 696e 7374  The current inst
+000131b0: 616e 6365 2061 6674 6572 2074 6865 2063  ance after the c
+000131c0: 6861 6e67 6573 2e0d 0a20 2020 2020 2020  hanges...       
+000131d0: 2022 2222 0d0a 2020 2020 2020 2020 6966   """..        if
+000131e0: 2069 7369 6e73 7461 6e63 6528 7365 676d   isinstance(segm
+000131f0: 656e 742c 2053 6567 6d65 6e74 293a 0d0a  ent, Segment):..
+00013200: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00013210: 656c 665b 7365 676d 656e 742e 6964 5d20  elf[segment.id] 
+00013220: 6973 206e 6f74 2073 6567 6d65 6e74 3a0d  is not segment:.
+00013230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013240: 2073 656c 662e 7265 6173 7369 676e 5f69   self.reassign_i
+00013250: 6473 2829 0d0a 2020 2020 2020 2020 2020  ds()..          
+00013260: 2020 2020 2020 6966 2073 656c 665b 7365        if self[se
+00013270: 676d 656e 742e 6964 5d20 6973 206e 6f74  gment.id] is not
+00013280: 2073 6567 6d65 6e74 3a0d 0a20 2020 2020   segment:..     
+00013290: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000132a0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000132b0: 2773 6567 6d65 6e74 206e 6f74 2069 6e20  'segment not in 
+000132c0: 7265 7375 6c74 2729 0d0a 2020 2020 2020  result')..      
+000132d0: 2020 2020 2020 7365 676d 656e 7420 3d20        segment = 
+000132e0: 7365 676d 656e 742e 6964 0d0a 2020 2020  segment.id..    
+000132f0: 2020 2020 6966 2076 6572 626f 7365 3a0d      if verbose:.
+00013300: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00013310: 6e74 2866 2752 656d 6f76 6564 3a20 5b69  nt(f'Removed: [i
+00013320: 643a 7b73 656c 665b 7365 676d 656e 745d  d:{self[segment]
+00013330: 2e69 647d 5d20 7b73 656c 665b 7365 676d  .id}] {self[segm
+00013340: 656e 745d 2e74 6f5f 6469 7370 6c61 795f  ent].to_display_
+00013350: 7374 7228 5472 7565 297d 2729 0d0a 2020  str(True)}')..  
+00013360: 2020 2020 2020 6465 6c20 7365 6c66 2e73        del self.s
+00013370: 6567 6d65 6e74 735b 7365 676d 656e 745d  egments[segment]
+00013380: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00013390: 2072 6561 7373 6967 6e5f 6964 733a 0d0a   reassign_ids:..
+000133a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000133b0: 726e 2073 656c 660d 0a20 2020 2020 2020  rn self..       
+000133c0: 2073 656c 662e 7265 6173 7369 676e 5f69   self.reassign_i
+000133d0: 6473 2854 7275 652c 2073 7461 7274 3d73  ds(True, start=s
+000133e0: 6567 6d65 6e74 290d 0a20 2020 2020 2020  egment)..       
+000133f0: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
+00013400: 2020 2020 6465 6620 7265 6d6f 7665 5f72      def remove_r
+00013410: 6570 6574 6974 696f 6e28 0d0a 2020 2020  epetition(..    
+00013420: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
+00013430: 2020 2020 2020 2020 2020 206d 6178 5f77             max_w
+00013440: 6f72 6473 3a20 696e 7420 3d20 312c 0d0a  ords: int = 1,..
+00013450: 2020 2020 2020 2020 2020 2020 6361 7365              case
+00013460: 5f73 656e 7369 7469 7665 3a20 626f 6f6c  _sensitive: bool
+00013470: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
+00013480: 2020 2020 2020 2073 7472 6970 3a20 626f         strip: bo
+00013490: 6f6c 203d 2054 7275 652c 0d0a 2020 2020  ol = True,..    
+000134a0: 2020 2020 2020 2020 6967 6e6f 7265 5f70          ignore_p
+000134b0: 756e 6374 7561 7469 6f6e 733a 2073 7472  unctuations: str
+000134c0: 203d 2022 5c22 272c 2e3f 2122 2c0d 0a20   = "\"',.?!",.. 
+000134d0: 2020 2020 2020 2020 2020 2065 7874 656e             exten
+000134e0: 645f 6475 7261 7469 6f6e 3a20 626f 6f6c  d_duration: bool
+000134f0: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
+00013500: 2020 2020 2020 7665 7262 6f73 653a 2062        verbose: b
+00013510: 6f6f 6c20 3d20 5472 7565 0d0a 2020 2020  ool = True..    
+00013520: 2920 2d3e 2027 5768 6973 7065 7252 6573  ) -> 'WhisperRes
+00013530: 756c 7427 3a0d 0a20 2020 2020 2020 2022  ult':..        "
+00013540: 2222 0d0a 2020 2020 2020 2020 5265 6d6f  ""..        Remo
+00013550: 7665 2077 6f72 6473 2074 6861 7420 7265  ve words that re
+00013560: 7065 6174 2063 6f6e 7365 6375 7469 7665  peat consecutive
+00013570: 6c79 2e0d 0a0d 0a20 2020 2020 2020 2050  ly.....        P
+00013580: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
+00013590: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+000135a0: 2020 2020 2020 206d 6178 5f77 6f72 6473         max_words
+000135b0: 203a 2069 6e74 0d0a 2020 2020 2020 2020   : int..        
+000135c0: 2020 2020 4d61 7869 6d75 6d20 6e75 6d62      Maximum numb
+000135d0: 6572 206f 6620 776f 7264 7320 746f 206c  er of words to l
+000135e0: 6f6f 6b20 666f 7220 636f 6e73 6563 7574  ook for consecut
+000135f0: 6976 656c 792e 0d0a 2020 2020 2020 2020  ively...        
+00013600: 6361 7365 5f73 656e 7369 7469 7665 203a  case_sensitive :
+00013610: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
+00013620: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
+00013630: 2020 5768 6574 6865 7220 7468 6520 6361    Whether the ca
+00013640: 7365 206f 6620 776f 7264 7320 6e65 6564  se of words need
+00013650: 2074 6f20 6d61 7463 6820 746f 2062 6520   to match to be 
+00013660: 636f 6e73 6964 6572 6564 2061 7320 7265  considered as re
+00013670: 7065 7469 7469 6f6e 2e0d 0a20 2020 2020  petition...     
+00013680: 2020 2073 7472 6970 203a 2062 6f6f 6c2c     strip : bool,
+00013690: 2064 6566 6175 6c74 2054 7275 650d 0a20   default True.. 
+000136a0: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+000136b0: 6572 2074 6f20 6967 6e6f 7265 2073 7061  er to ignore spa
+000136c0: 6365 7320 6265 666f 7265 2061 6e64 2061  ces before and a
+000136d0: 6674 6572 2065 6163 6820 776f 7264 2e0d  fter each word..
+000136e0: 0a20 2020 2020 2020 2069 676e 6f72 655f  .        ignore_
+000136f0: 7075 6e63 7475 6174 696f 6e73 203a 2062  punctuations : b
+00013700: 6f6f 6c2c 2064 6566 6175 6c74 2027 2227  ool, default '"'
+00013710: 2c2e 3f21 270d 0a20 2020 2020 2020 2020  ,.?!'..         
+00013720: 2020 2045 6e64 696e 6720 7075 6e63 7475     Ending punctu
+00013730: 6174 696f 6e73 2074 6f20 6967 6e6f 7265  ations to ignore
+00013740: 2e0d 0a20 2020 2020 2020 2065 7874 656e  ...        exten
+00013750: 645f 6475 7261 7469 6f6e 3a20 626f 6f6c  d_duration: bool
+00013760: 2c20 6465 6661 756c 7420 5472 7565 0d0a  , default True..
+00013770: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+00013780: 6865 7220 746f 2065 7874 656e 6420 7468  her to extend th
+00013790: 6520 6475 7261 7469 6f6e 206f 6620 7468  e duration of th
+000137a0: 6520 7072 6576 696f 7573 2077 6f72 6420  e previous word 
+000137b0: 746f 2063 6f76 6572 2074 6865 2064 7572  to cover the dur
+000137c0: 6174 696f 6e20 6f66 2074 6865 2072 6570  ation of the rep
+000137d0: 6574 6974 696f 6e2e 0d0a 2020 2020 2020  etition...      
+000137e0: 2020 7665 7262 6f73 653a 2062 6f6f 6c2c    verbose: bool,
+000137f0: 2064 6566 6175 6c74 2054 7275 650d 0a20   default True.. 
+00013800: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+00013810: 6572 2074 6f20 7072 696e 7420 6465 7461  er to print deta
+00013820: 696c 206f 6620 7468 6520 7265 6d6f 7665  il of the remove
+00013830: 6420 7265 7065 7469 7469 6f6e 732e 0d0a  d repetitions...
+00013840: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00013850: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+00013860: 2d2d 0d0a 2020 2020 2020 2020 7374 6162  --..        stab
+00013870: 6c65 5f77 6869 7370 6572 2e72 6573 756c  le_whisper.resul
+00013880: 742e 5768 6973 7065 7252 6573 756c 740d  t.WhisperResult.
+00013890: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+000138a0: 2063 7572 7265 6e74 2069 6e73 7461 6e63   current instanc
+000138b0: 6520 6166 7465 7220 7468 6520 6368 616e  e after the chan
+000138c0: 6765 732e 0d0a 2020 2020 2020 2020 2222  ges...        ""
+000138d0: 220d 0a20 2020 2020 2020 2069 6620 6e6f  "..        if no
+000138e0: 7420 7365 6c66 2e68 6173 5f77 6f72 6473  t self.has_words
+000138f0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00013900: 6574 7572 6e20 7365 6c66 0d0a 0d0a 2020  eturn self....  
+00013910: 2020 2020 2020 666f 7220 636f 756e 7420        for count 
+00013920: 696e 2072 616e 6765 2831 2c20 6d61 785f  in range(1, max_
+00013930: 776f 7264 7320 2b20 3129 3a0d 0a20 2020  words + 1):..   
+00013940: 2020 2020 2020 2020 2061 6c6c 5f77 6f72           all_wor
+00013950: 6473 203d 2073 656c 662e 616c 6c5f 776f  ds = self.all_wo
+00013960: 7264 7328 290d 0a20 2020 2020 2020 2020  rds()..         
+00013970: 2020 2069 6620 6c65 6e28 616c 6c5f 776f     if len(all_wo
+00013980: 7264 7329 203c 2032 3a0d 0a20 2020 2020  rds) < 2:..     
+00013990: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000139a0: 6e20 7365 6c66 0d0a 2020 2020 2020 2020  n self..        
+000139b0: 2020 2020 616c 6c5f 776f 7264 735f 7374      all_words_st
+000139c0: 7220 3d20 5b77 2e77 6f72 6420 666f 7220  r = [w.word for 
+000139d0: 7720 696e 2061 6c6c 5f77 6f72 6473 5d0d  w in all_words].
+000139e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000139f0: 7374 7269 703a 0d0a 2020 2020 2020 2020  strip:..        
+00013a00: 2020 2020 2020 2020 616c 6c5f 776f 7264          all_word
+00013a10: 735f 7374 7220 3d20 5b77 2e73 7472 6970  s_str = [w.strip
+00013a20: 2829 2066 6f72 2077 2069 6e20 616c 6c5f  () for w in all_
+00013a30: 776f 7264 735f 7374 725d 0d0a 2020 2020  words_str]..    
+00013a40: 2020 2020 2020 2020 6966 2069 676e 6f72          if ignor
+00013a50: 655f 7075 6e63 7475 6174 696f 6e73 3a0d  e_punctuations:.
+00013a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013a70: 2070 746e 203d 2066 275b 7b69 676e 6f72   ptn = f'[{ignor
+00013a80: 655f 7075 6e63 7475 6174 696f 6e73 7d5d  e_punctuations}]
+00013a90: 2b24 270d 0a20 2020 2020 2020 2020 2020  +$'..           
+00013aa0: 2020 2020 2061 6c6c 5f77 6f72 6473 5f73       all_words_s
+00013ab0: 7472 203d 205b 7265 2e73 7562 2870 746e  tr = [re.sub(ptn
+00013ac0: 2c20 2727 2c20 7729 2066 6f72 2077 2069  , '', w) for w i
+00013ad0: 6e20 616c 6c5f 776f 7264 735f 7374 725d  n all_words_str]
+00013ae0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00013af0: 206e 6f74 2063 6173 655f 7365 6e73 6974   not case_sensit
+00013b00: 6976 653a 0d0a 2020 2020 2020 2020 2020  ive:..          
+00013b10: 2020 2020 2020 616c 6c5f 776f 7264 735f        all_words_
+00013b20: 7374 7220 3d20 5b77 2e6c 6f77 6572 2829  str = [w.lower()
+00013b30: 2066 6f72 2077 2069 6e20 616c 6c5f 776f   for w in all_wo
+00013b40: 7264 735f 7374 725d 0d0a 2020 2020 2020  rds_str]..      
+00013b50: 2020 2020 2020 6e65 7874 5f69 203d 204e        next_i = N
+00013b60: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
+00013b70: 2063 6861 6e67 6573 203d 205b 5d0d 0a20   changes = [].. 
+00013b80: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00013b90: 2069 6e20 7265 7665 7273 6564 2872 616e   in reversed(ran
+00013ba0: 6765 2863 6f75 6e74 2a32 2c20 6c65 6e28  ge(count*2, len(
+00013bb0: 616c 6c5f 776f 7264 735f 7374 7229 2b31  all_words_str)+1
+00013bc0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00013bd0: 2020 2020 2069 6620 6e65 7874 5f69 2069       if next_i i
+00013be0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c00: 2069 6620 6e65 7874 5f69 2021 3d20 693a   if next_i != i:
+00013c10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013c20: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00013c30: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+00013c40: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00013c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c60: 2020 2020 2020 206e 6578 745f 6920 3d20         next_i = 
+00013c70: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
+00013c80: 2020 2020 2020 7320 3d20 6920 2d20 636f        s = i - co
+00013c90: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
+00013ca0: 2020 2020 2069 6620 616c 6c5f 776f 7264       if all_word
+00013cb0: 735f 7374 725b 7320 2d20 636f 756e 743a  s_str[s - count:
+00013cc0: 735d 2021 3d20 616c 6c5f 776f 7264 735f  s] != all_words_
+00013cd0: 7374 725b 733a 695d 3a0d 0a20 2020 2020  str[s:i]:..     
+00013ce0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013cf0: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
+00013d00: 2020 2020 2020 2020 206e 6578 745f 6920           next_i 
+00013d10: 3d20 730d 0a20 2020 2020 2020 2020 2020  = s..           
+00013d20: 2020 2020 2069 6620 6578 7465 6e64 5f64       if extend_d
+00013d30: 7572 6174 696f 6e3a 0d0a 2020 2020 2020  uration:..      
+00013d40: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00013d50: 6c5f 776f 7264 735b 732d 315d 2e65 6e64  l_words[s-1].end
+00013d60: 203d 2061 6c6c 5f77 6f72 6473 5b69 2d31   = all_words[i-1
+00013d70: 5d2e 656e 640d 0a20 2020 2020 2020 2020  ].end..         
+00013d80: 2020 2020 2020 2074 656d 705f 6368 616e         temp_chan
+00013d90: 6765 7320 3d20 5b5d 0d0a 2020 2020 2020  ges = []..      
+00013da0: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
+00013db0: 696e 2072 6576 6572 7365 6428 7261 6e67  in reversed(rang
+00013dc0: 6528 732c 2069 2929 3a0d 0a20 2020 2020  e(s, i)):..     
+00013dd0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00013de0: 6620 7665 7262 6f73 653a 0d0a 2020 2020  f verbose:..    
+00013df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e00: 2020 2020 7465 6d70 5f63 6861 6e67 6573      temp_changes
+00013e10: 2e61 7070 656e 6428 6627 2d20 7b61 6c6c  .append(f'- {all
+00013e20: 5f77 6f72 6473 5b6a 5d2e 746f 5f64 6963  _words[j].to_dic
+00013e30: 7428 297d 2729 0d0a 2020 2020 2020 2020  t()}')..        
+00013e40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013e50: 2e72 656d 6f76 655f 776f 7264 2861 6c6c  .remove_word(all
+00013e60: 5f77 6f72 6473 5b6a 5d2c 2046 616c 7365  _words[j], False
+00013e70: 2c20 7665 7262 6f73 653d 4661 6c73 6529  , verbose=False)
+00013e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013e90: 2020 6966 2074 656d 705f 6368 616e 6765    if temp_change
+00013ea0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00013eb0: 2020 2020 2020 2020 6368 616e 6765 732e          changes.
+00013ec0: 6170 7065 6e64 280d 0a20 2020 2020 2020  append(..       
 00013ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ee0: 2020 2020 6966 206c 656e 2861 6c6c 5f77      if len(all_w
-00013ef0: 6f72 6473 5b69 305d 2e77 6f72 6429 203c  ords[i0].word) <
-00013f00: 206c 656e 2861 6c6c 5f77 6f72 6473 5b69   len(all_words[i
-00013f10: 315d 2e77 6f72 6429 3a0d 0a20 2020 2020  1].word):..     
-00013f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f30: 2020 2061 6c6c 5f77 6f72 6473 5b69 315d     all_words[i1]
-00013f40: 2e73 7461 7274 203d 2061 6c6c 5f77 6f72  .start = all_wor
-00013f50: 6473 5b69 305d 2e73 7461 7274 0d0a 2020  ds[i0].start..  
-00013f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f70: 2020 2020 2020 616c 6c5f 776f 7264 735b        all_words[
-00013f80: 6931 5d2e 656e 6420 3d20 616c 6c5f 776f  i1].end = all_wo
-00013f90: 7264 735b 6930 5d2e 656e 640d 0a20 2020  rds[i0].end..   
-00013fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fb0: 2020 2020 205f 7369 642c 205f 7769 6420       _sid, _wid 
-00013fc0: 3d20 616c 6c5f 776f 7264 735b 6930 5d2e  = all_words[i0].
-00013fd0: 7365 676d 656e 745f 6964 2c20 616c 6c5f  segment_id, all_
-00013fe0: 776f 7264 735b 6930 5d2e 6964 0d0a 2020  words[i0].id..  
-00013ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014000: 2020 2020 2020 7365 6c66 2e73 6567 6d65        self.segme
-00014010: 6e74 735b 5f73 6964 5d2e 776f 7264 735b  nts[_sid].words[
-00014020: 5f77 6964 5d20 3d20 616c 6c5f 776f 7264  _wid] = all_word
-00014030: 735b 6931 5d0d 0a0d 0a20 2020 2020 2020  s[i1]....       
-00014040: 2020 2020 2069 6620 6368 616e 6765 733a       if changes:
-00014050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014060: 2020 7072 696e 7428 275c 6e27 2e6a 6f69    print('\n'.joi
-00014070: 6e28 7265 7665 7273 6564 2863 6861 6e67  n(reversed(chang
-00014080: 6573 2929 290d 0a0d 0a20 2020 2020 2020  es)))....       
-00014090: 2020 2020 2073 656c 662e 7265 6d6f 7665       self.remove
-000140a0: 5f6e 6f5f 776f 7264 5f73 6567 6d65 6e74  _no_word_segment
-000140b0: 7328 7265 6173 7369 676e 5f69 6473 3d46  s(reassign_ids=F
-000140c0: 616c 7365 290d 0a20 2020 2020 2020 2073  alse)..        s
-000140d0: 656c 662e 7265 6173 7369 676e 5f69 6473  elf.reassign_ids
-000140e0: 2829 0d0a 0d0a 2020 2020 2020 2020 7265  ()....        re
-000140f0: 7475 726e 2073 656c 660d 0a0d 0a20 2020  turn self....   
-00014100: 2064 6566 2072 656d 6f76 655f 776f 7264   def remove_word
-00014110: 735f 6279 5f73 7472 280d 0a20 2020 2020  s_by_str(..     
-00014120: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
-00014130: 2020 2020 2020 2020 2020 776f 7264 733a            words:
-00014140: 2055 6e69 6f6e 5b73 7472 2c20 4c69 7374   Union[str, List
-00014150: 5b73 7472 5d2c 204e 6f6e 655d 2c0d 0a20  [str], None],.. 
-00014160: 2020 2020 2020 2020 2020 2063 6173 655f             case_
-00014170: 7365 6e73 6974 6976 653a 2062 6f6f 6c20  sensitive: bool 
-00014180: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
-00014190: 2020 2020 2020 7374 7269 703a 2062 6f6f        strip: boo
-000141a0: 6c20 3d20 5472 7565 2c0d 0a20 2020 2020  l = True,..     
-000141b0: 2020 2020 2020 2069 676e 6f72 655f 7075         ignore_pu
-000141c0: 6e63 7475 6174 696f 6e73 3a20 7374 7220  nctuations: str 
-000141d0: 3d20 225c 2227 2c2e 3f21 222c 0d0a 2020  = "\"',.?!",..  
-000141e0: 2020 2020 2020 2020 2020 6d69 6e5f 7072            min_pr
-000141f0: 6f62 3a20 666c 6f61 7420 3d20 4e6f 6e65  ob: float = None
-00014200: 2c0d 0a20 2020 2020 2020 2020 2020 2066  ,..            f
-00014210: 696c 7465 7273 3a20 4361 6c6c 6162 6c65  ilters: Callable
-00014220: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00014230: 2020 2020 2020 7665 7262 6f73 653a 2062        verbose: b
-00014240: 6f6f 6c20 3d20 5472 7565 0d0a 2020 2020  ool = True..    
-00014250: 2920 2d3e 2027 5768 6973 7065 7252 6573  ) -> 'WhisperRes
-00014260: 756c 7427 3a0d 0a20 2020 2020 2020 2022  ult':..        "
-00014270: 2222 0d0a 2020 2020 2020 2020 5265 6d6f  ""..        Remo
-00014280: 7665 2077 6f72 6473 2074 6861 7420 6d61  ve words that ma
-00014290: 7463 6820 6060 776f 7264 7360 602e 0d0a  tch ``words``...
-000142a0: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-000142b0: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
-000142c0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-000142d0: 2020 776f 7264 7320 3a20 7374 7220 6f72    words : str or
-000142e0: 206c 6973 7420 6f66 2073 7472 206f 7220   list of str or 
-000142f0: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
-00014300: 2020 4120 776f 7264 206f 7220 6c69 7374    A word or list
-00014310: 206f 6620 776f 7264 7320 746f 2072 656d   of words to rem
-00014320: 6f76 652e 6060 4e6f 6e65 6060 2066 6f72  ove.``None`` for
-00014330: 2061 6c6c 2077 6f72 6473 2074 6f20 6265   all words to be
-00014340: 2070 6173 7365 6420 696e 746f 2060 6066   passed into ``f
-00014350: 696c 7465 7273 6060 2e0d 0a20 2020 2020  ilters``...     
-00014360: 2020 2063 6173 655f 7365 6e73 6974 6976     case_sensitiv
-00014370: 6520 3a20 626f 6f6c 2c20 6465 6661 756c  e : bool, defaul
-00014380: 7420 4661 6c73 650d 0a20 2020 2020 2020  t False..       
-00014390: 2020 2020 2057 6865 7468 6572 2074 6865       Whether the
-000143a0: 2063 6173 6520 6f66 2077 6f72 6473 206e   case of words n
-000143b0: 6565 6420 746f 206d 6174 6368 2074 6f20  eed to match to 
-000143c0: 6265 2063 6f6e 7369 6465 7265 6420 6173  be considered as
-000143d0: 2072 6570 6574 6974 696f 6e2e 0d0a 2020   repetition...  
-000143e0: 2020 2020 2020 7374 7269 7020 3a20 626f        strip : bo
-000143f0: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
-00014400: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-00014410: 6574 6865 7220 746f 2069 676e 6f72 6520  ether to ignore 
-00014420: 7370 6163 6573 2062 6566 6f72 6520 616e  spaces before an
-00014430: 6420 6166 7465 7220 6561 6368 2077 6f72  d after each wor
-00014440: 642e 0d0a 2020 2020 2020 2020 6967 6e6f  d...        igno
-00014450: 7265 5f70 756e 6374 7561 7469 6f6e 7320  re_punctuations 
-00014460: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-00014470: 2722 272c 2e3f 2127 0d0a 2020 2020 2020  '"',.?!'..      
-00014480: 2020 2020 2020 456e 6469 6e67 2070 756e        Ending pun
-00014490: 6374 7561 7469 6f6e 7320 746f 2069 676e  ctuations to ign
-000144a0: 6f72 652e 0d0a 2020 2020 2020 2020 6d69  ore...        mi
-000144b0: 6e5f 7072 6f62 203a 2066 6c6f 6174 2c20  n_prob : float, 
-000144c0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-000144d0: 2020 2020 2020 4163 7473 2061 7320 7468        Acts as th
-000144e0: 6520 6669 7273 7420 6669 6c74 6572 2074  e first filter t
-000144f0: 6865 2066 6f72 2074 6865 2077 6f72 6473  he for the words
-00014500: 2074 6861 7420 6d61 7463 6820 6060 776f   that match ``wo
-00014510: 7264 7360 602e 2057 6f72 6473 2077 6974  rds``. Words wit
-00014520: 6820 7072 6f62 6162 696c 6974 7920 3c20  h probability < 
-00014530: 6060 6d69 6e5f 7072 6f62 6060 2077 696c  ``min_prob`` wil
-00014540: 6c0d 0a20 2020 2020 2020 2020 2020 2062  l..            b
-00014550: 6520 7265 6d6f 7665 6420 6966 2060 6066  e removed if ``f
-00014560: 696c 7465 7273 6060 2069 7320 6060 4e6f  ilters`` is ``No
-00014570: 6e65 6060 2c20 656c 7365 2070 6173 7320  ne``, else pass 
-00014580: 7468 6520 776f 7264 7320 696e 746f 2060  the words into `
-00014590: 6066 696c 7465 7273 6060 2e20 576f 7264  `filters``. Word
-000145a0: 7320 7769 7468 6f75 7420 7072 6f62 6162  s without probab
-000145b0: 696c 6974 7920 7769 6c6c 0d0a 2020 2020  ility will..    
-000145c0: 2020 2020 2020 2020 6265 2074 7265 6174          be treat
-000145d0: 6564 2061 7320 6861 7669 6e67 2070 726f  ed as having pro
-000145e0: 6261 6269 6c69 7479 203c 2060 606d 696e  bability < ``min
-000145f0: 5f70 726f 6260 602e 0d0a 2020 2020 2020  _prob``...      
-00014600: 2020 6669 6c74 6572 7320 3a20 4361 6c6c    filters : Call
-00014610: 6162 6c65 2c20 6f70 7469 6f6e 616c 0d0a  able, optional..
-00014620: 2020 2020 2020 2020 2020 2020 4120 6675              A fu
-00014630: 6e63 7469 6f6e 2074 6861 7420 7461 6b65  nction that take
-00014640: 7320 616e 2069 6e73 7461 6e63 6520 6f66  s an instance of
-00014650: 203a 636c 6173 733a 6073 7461 626c 655f   :class:`stable_
-00014660: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
-00014670: 6f72 6454 696d 696e 6760 2061 7320 6974  ordTiming` as it
-00014680: 7320 6f6e 6c79 2061 7267 756d 656e 742e  s only argument.
-00014690: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-000146a0: 6973 2066 756e 6374 696f 6e20 6973 2063  is function is c
-000146b0: 7573 746f 6d20 6669 6c74 6572 2066 6f72  ustom filter for
-000146c0: 2074 6865 2077 6f72 6473 2074 6861 7420   the words that 
-000146d0: 6d61 7463 6820 6060 776f 7264 7360 6020  match ``words`` 
-000146e0: 616e 6420 7765 7265 206e 6f74 2063 6175  and were not cau
-000146f0: 6768 7420 6279 2060 606d 696e 5f70 726f  ght by ``min_pro
-00014700: 6260 602e 0d0a 2020 2020 2020 2020 7665  b``...        ve
-00014710: 7262 6f73 653a 0d0a 2020 2020 2020 2020  rbose:..        
-00014720: 2020 2020 5768 6574 6865 7220 746f 2070      Whether to p
-00014730: 7269 6e74 2064 6574 6169 6c20 6f66 2074  rint detail of t
-00014740: 6865 2072 656d 6f76 6564 2077 6f72 6473  he removed words
-00014750: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
-00014760: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
-00014770: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
-00014780: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
-00014790: 7375 6c74 2e57 6869 7370 6572 5265 7375  sult.WhisperResu
-000147a0: 6c74 0d0a 2020 2020 2020 2020 2020 2020  lt..            
-000147b0: 5468 6520 6375 7272 656e 7420 696e 7374  The current inst
-000147c0: 616e 6365 2061 6674 6572 2074 6865 2063  ance after the c
-000147d0: 6861 6e67 6573 2e0d 0a20 2020 2020 2020  hanges...       
-000147e0: 2022 2222 0d0a 2020 2020 2020 2020 6966   """..        if
-000147f0: 206e 6f74 2073 656c 662e 6861 735f 776f   not self.has_wo
-00014800: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
-00014810: 2020 7265 7475 726e 2073 656c 660d 0a20    return self.. 
-00014820: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00014830: 616e 6365 2877 6f72 6473 2c20 7374 7229  ance(words, str)
-00014840: 3a0d 0a20 2020 2020 2020 2020 2020 2077  :..            w
-00014850: 6f72 6473 203d 205b 776f 7264 735d 0d0a  ords = [words]..
-00014860: 2020 2020 2020 2020 616c 6c5f 776f 7264          all_word
-00014870: 7320 3d20 7365 6c66 2e61 6c6c 5f77 6f72  s = self.all_wor
-00014880: 6473 2829 0d0a 2020 2020 2020 2020 616c  ds()..        al
-00014890: 6c5f 776f 7264 735f 7374 7220 3d20 5b77  l_words_str = [w
-000148a0: 2e77 6f72 6420 666f 7220 7720 696e 2061  .word for w in a
-000148b0: 6c6c 5f77 6f72 6473 5d0d 0a20 2020 2020  ll_words]..     
-000148c0: 2020 2069 6620 7374 7269 703a 0d0a 2020     if strip:..  
-000148d0: 2020 2020 2020 2020 2020 616c 6c5f 776f            all_wo
-000148e0: 7264 735f 7374 7220 3d20 5b77 2e73 7472  rds_str = [w.str
-000148f0: 6970 2829 2066 6f72 2077 2069 6e20 616c  ip() for w in al
-00014900: 6c5f 776f 7264 735f 7374 725d 0d0a 2020  l_words_str]..  
-00014910: 2020 2020 2020 2020 2020 776f 7264 7320            words 
-00014920: 3d20 5b77 2e73 7472 6970 2829 2066 6f72  = [w.strip() for
-00014930: 2077 2069 6e20 776f 7264 735d 0d0a 2020   w in words]..  
-00014940: 2020 2020 2020 6966 2069 676e 6f72 655f        if ignore_
-00014950: 7075 6e63 7475 6174 696f 6e73 3a0d 0a20  punctuations:.. 
-00014960: 2020 2020 2020 2020 2020 2070 746e 203d             ptn =
-00014970: 2066 275b 7b69 676e 6f72 655f 7075 6e63   f'[{ignore_punc
-00014980: 7475 6174 696f 6e73 7d5d 2b24 270d 0a20  tuations}]+$'.. 
-00014990: 2020 2020 2020 2020 2020 2061 6c6c 5f77             all_w
-000149a0: 6f72 6473 5f73 7472 203d 205b 7265 2e73  ords_str = [re.s
-000149b0: 7562 2870 746e 2c20 2727 2c20 7729 2066  ub(ptn, '', w) f
-000149c0: 6f72 2077 2069 6e20 616c 6c5f 776f 7264  or w in all_word
-000149d0: 735f 7374 725d 0d0a 2020 2020 2020 2020  s_str]..        
-000149e0: 2020 2020 776f 7264 7320 3d20 5b72 652e      words = [re.
-000149f0: 7375 6228 7074 6e2c 2027 272c 2077 2920  sub(ptn, '', w) 
-00014a00: 666f 7220 7720 696e 2077 6f72 6473 5d0d  for w in words].
-00014a10: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00014a20: 6361 7365 5f73 656e 7369 7469 7665 3a0d  case_sensitive:.
-00014a30: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
-00014a40: 5f77 6f72 6473 5f73 7472 203d 205b 772e  _words_str = [w.
-00014a50: 6c6f 7765 7228 2920 666f 7220 7720 696e  lower() for w in
-00014a60: 2061 6c6c 5f77 6f72 6473 5f73 7472 5d0d   all_words_str].
-00014a70: 0a20 2020 2020 2020 2020 2020 2077 6f72  .            wor
-00014a80: 6473 203d 205b 772e 6c6f 7765 7228 2920  ds = [w.lower() 
-00014a90: 666f 7220 7720 696e 2077 6f72 6473 5d0d  for w in words].
-00014aa0: 0a0d 0a20 2020 2020 2020 2063 6861 6e67  ...        chang
-00014ab0: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
-00014ac0: 2066 6f72 2069 2c20 7720 696e 2072 6576   for i, w in rev
-00014ad0: 6572 7365 6428 6c69 7374 2865 6e75 6d65  ersed(list(enume
-00014ae0: 7261 7465 2861 6c6c 5f77 6f72 6473 5f73  rate(all_words_s
-00014af0: 7472 2929 293a 0d0a 2020 2020 2020 2020  tr))):..        
-00014b00: 2020 2020 6966 206e 6f74 2028 776f 7264      if not (word
-00014b10: 7320 6973 204e 6f6e 6520 6f72 2061 6e79  s is None or any
-00014b20: 2877 203d 3d20 5f77 2066 6f72 205f 7720  (w == _w for _w 
-00014b30: 696e 2077 6f72 6473 2929 3a0d 0a20 2020  in words)):..   
-00014b40: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00014b50: 7469 6e75 650d 0a20 2020 2020 2020 2020  tinue..         
-00014b60: 2020 2069 6620 280d 0a20 2020 2020 2020     if (..       
-00014b70: 2020 2020 2020 2020 2020 2020 2028 6d69               (mi
-00014b80: 6e5f 7072 6f62 2069 7320 4e6f 6e65 206f  n_prob is None o
-00014b90: 7220 616c 6c5f 776f 7264 735b 695d 2e70  r all_words[i].p
-00014ba0: 726f 6261 6269 6c69 7479 2069 7320 4e6f  robability is No
-00014bb0: 6e65 206f 7220 6d69 6e5f 7072 6f62 203e  ne or min_prob >
-00014bc0: 2061 6c6c 5f77 6f72 6473 5b69 5d2e 7072   all_words[i].pr
-00014bd0: 6f62 6162 696c 6974 7929 2061 6e64 0d0a  obability) and..
-00014be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bf0: 2020 2020 2866 696c 7465 7273 2069 7320      (filters is 
-00014c00: 4e6f 6e65 206f 7220 6669 6c74 6572 7328  None or filters(
-00014c10: 616c 6c5f 776f 7264 735b 695d 2929 0d0a  all_words[i]))..
-00014c20: 2020 2020 2020 2020 2020 2020 293a 0d0a              ):..
-00014c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c40: 6966 2076 6572 626f 7365 3a0d 0a20 2020  if verbose:..   
-00014c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c60: 2063 6861 6e67 6573 2e61 7070 656e 6428   changes.append(
-00014c70: 6627 5265 6d6f 7665 643a 207b 616c 6c5f  f'Removed: {all_
-00014c80: 776f 7264 735b 695d 2e74 6f5f 6469 6374  words[i].to_dict
-00014c90: 2829 7d27 290d 0a20 2020 2020 2020 2020  ()}')..         
-00014ca0: 2020 2020 2020 2073 656c 662e 7265 6d6f         self.remo
-00014cb0: 7665 5f77 6f72 6428 616c 6c5f 776f 7264  ve_word(all_word
-00014cc0: 735b 695d 2c20 4661 6c73 652c 2076 6572  s[i], False, ver
-00014cd0: 626f 7365 3d46 616c 7365 290d 0a20 2020  bose=False)..   
-00014ce0: 2020 2020 2069 6620 6368 616e 6765 733a       if changes:
-00014cf0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00014d00: 696e 7428 275c 6e27 2e6a 6f69 6e28 7265  int('\n'.join(re
-00014d10: 7665 7273 6564 2863 6861 6e67 6573 2929  versed(changes))
-00014d20: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00014d30: 7265 6d6f 7665 5f6e 6f5f 776f 7264 5f73  remove_no_word_s
-00014d40: 6567 6d65 6e74 7328 290d 0a0d 0a20 2020  egments()....   
-00014d50: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00014d60: 0d0a 0d0a 2020 2020 6465 6620 6669 6c6c  ....    def fill
-00014d70: 5f69 6e5f 6761 7073 280d 0a20 2020 2020  _in_gaps(..     
-00014d80: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
-00014d90: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
-00014da0: 7265 7375 6c74 3a20 556e 696f 6e5b 2757  result: Union['W
-00014db0: 6869 7370 6572 5265 7375 6c74 272c 2073  hisperResult', s
-00014dc0: 7472 5d2c 0d0a 2020 2020 2020 2020 2020  tr],..          
-00014dd0: 2020 6d69 6e5f 6761 703a 2066 6c6f 6174    min_gap: float
-00014de0: 203d 2030 2e31 2c0d 0a20 2020 2020 2020   = 0.1,..       
-00014df0: 2020 2020 2063 6173 655f 7365 6e73 6974       case_sensit
-00014e00: 6976 653a 2062 6f6f 6c20 3d20 4661 6c73  ive: bool = Fals
-00014e10: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00014e20: 7374 7269 703a 2062 6f6f 6c20 3d20 5472  strip: bool = Tr
-00014e30: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-00014e40: 2069 676e 6f72 655f 7075 6e63 7475 6174   ignore_punctuat
-00014e50: 696f 6e73 3a20 7374 7220 3d20 225c 2227  ions: str = "\"'
-00014e60: 2c2e 3f21 222c 0d0a 2020 2020 2020 2020  ,.?!",..        
-00014e70: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
-00014e80: 6c20 3d20 5472 7565 0d0a 2020 2020 2920  l = True..    ) 
-00014e90: 2d3e 2027 5768 6973 7065 7252 6573 756c  -> 'WhisperResul
-00014ea0: 7427 3a0d 0a20 2020 2020 2020 2022 2222  t':..        """
-00014eb0: 0d0a 2020 2020 2020 2020 4669 6c6c 2069  ..        Fill i
-00014ec0: 6e20 7365 676d 656e 7420 6761 7073 206c  n segment gaps l
-00014ed0: 6172 6765 7220 7468 616e 2060 606d 696e  arger than ``min
-00014ee0: 5f67 6170 6060 2077 6974 6820 636f 6e74  _gap`` with cont
-00014ef0: 656e 7420 6672 6f6d 2060 606f 7468 6572  ent from ``other
-00014f00: 5f72 6573 756c 7460 6020 6174 2074 6865  _result`` at the
-00014f10: 2074 696d 6573 206f 6620 6761 7073 2e0d   times of gaps..
-00014f20: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00014f30: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
-00014f40: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-00014f50: 2020 206f 7468 6572 5f72 6573 756c 7420     other_result 
-00014f60: 3a20 5768 6973 7065 7252 6573 756c 7420  : WhisperResult 
-00014f70: 6f72 2073 7472 0d0a 2020 2020 2020 2020  or str..        
-00014f80: 2020 2020 416e 6f74 6865 7220 7472 616e      Another tran
-00014f90: 7363 7269 7074 696f 6e20 7265 7375 6c74  scription result
-00014fa0: 2061 7320 616e 2069 6e73 7461 6e63 6520   as an instance 
-00014fb0: 6f66 203a 636c 6173 733a 6073 7461 626c  of :class:`stabl
-00014fc0: 655f 7768 6973 7065 722e 7265 7375 6c74  e_whisper.result
-00014fd0: 2e57 6869 7370 6572 5265 7375 6c74 6020  .WhisperResult` 
-00014fe0: 6f72 2070 6174 6820 746f 2074 6865 0d0a  or path to the..
-00014ff0: 2020 2020 2020 2020 2020 2020 4a53 4f4e              JSON
-00015000: 206f 6620 7468 6520 7265 7375 6c74 2e0d   of the result..
-00015010: 0a20 2020 2020 2020 206d 696e 5f67 6170  .        min_gap
-00015020: 203a 2066 6c6f 6174 2c20 6465 6661 756c   : float, defaul
-00015030: 7420 302e 310d 0a20 2020 2020 2020 2020  t 0.1..         
-00015040: 2020 2054 6865 206d 696e 696d 756d 2073     The minimum s
-00015050: 6563 6f6e 6473 206f 6620 6120 6761 7020  econds of a gap 
-00015060: 6265 7477 6565 6e20 7365 676d 656e 7473  between segments
-00015070: 2074 6861 7420 6d75 7374 2062 6520 6578   that must be ex
-00015080: 6365 6564 6564 2074 6f20 6265 2066 696c  ceeded to be fil
-00015090: 6c65 6420 696e 2e0d 0a20 2020 2020 2020  led in...       
-000150a0: 2063 6173 655f 7365 6e73 6974 6976 6520   case_sensitive 
-000150b0: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-000150c0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-000150d0: 2020 2057 6865 7468 6572 2074 6f20 636f     Whether to co
-000150e0: 6e73 6964 6572 2074 6865 2063 6173 6520  nsider the case 
-000150f0: 6f66 2074 6865 2066 6972 7374 2061 6e64  of the first and
-00015100: 206c 6173 7420 776f 7264 206f 6620 7468   last word of th
-00015110: 6520 6761 7020 746f 2064 6574 6572 6d69  e gap to determi
-00015120: 6e65 206f 7665 726c 6170 7069 6e67 2077  ne overlapping w
-00015130: 6f72 6473 2074 6f20 7265 6d6f 7665 0d0a  ords to remove..
-00015140: 2020 2020 2020 2020 2020 2020 6265 666f              befo
-00015150: 7265 2066 696c 6c69 6e67 2069 6e2e 0d0a  re filling in...
-00015160: 2020 2020 2020 2020 7374 7269 7020 3a20          strip : 
-00015170: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
-00015180: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00015190: 5768 6574 6865 7220 746f 2069 676e 6f72  Whether to ignor
-000151a0: 6520 7370 6163 6573 2062 6566 6f72 6520  e spaces before 
-000151b0: 616e 6420 6166 7465 7220 7468 6520 6669  and after the fi
-000151c0: 7273 7420 616e 6420 6c61 7374 2077 6f72  rst and last wor
-000151d0: 6420 6f66 2074 6865 2067 6170 2074 6f20  d of the gap to 
-000151e0: 6465 7465 726d 696e 6520 6f76 6572 6c61  determine overla
-000151f0: 7070 696e 6720 776f 7264 730d 0a20 2020  pping words..   
-00015200: 2020 2020 2020 2020 2074 6f20 7265 6d6f           to remo
-00015210: 7665 2062 6566 6f72 6520 6669 6c6c 696e  ve before fillin
-00015220: 6720 696e 2e0d 0a20 2020 2020 2020 2069  g in...        i
-00015230: 676e 6f72 655f 7075 6e63 7475 6174 696f  gnore_punctuatio
-00015240: 6e73 203a 2062 6f6f 6c2c 2064 6566 6175  ns : bool, defau
-00015250: 6c74 2027 2227 2c2e 3f21 270d 0a20 2020  lt '"',.?!'..   
-00015260: 2020 2020 2020 2020 2045 6e64 696e 6720           Ending 
-00015270: 7075 6e63 7475 6174 696f 6e73 2074 6f20  punctuations to 
-00015280: 6967 6e6f 7265 2069 6e20 7468 6520 6669  ignore in the fi
-00015290: 7273 7420 616e 6420 6c61 7374 2077 6f72  rst and last wor
-000152a0: 6420 6f66 2074 6865 2067 6170 2074 6f20  d of the gap to 
-000152b0: 6465 7465 726d 696e 6520 6f76 6572 6c61  determine overla
-000152c0: 7070 696e 6720 776f 7264 7320 746f 0d0a  pping words to..
-000152d0: 2020 2020 2020 2020 2020 2020 7265 6d6f              remo
-000152e0: 7665 2062 6566 6f72 6520 6669 6c6c 696e  ve before fillin
-000152f0: 6720 696e 2e0d 0a20 2020 2020 2020 2076  g in...        v
-00015300: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
-00015310: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00015320: 7072 696e 7420 6465 7461 696c 206f 6620  print detail of 
-00015330: 7468 6520 6669 6c6c 6564 2063 6f6e 7465  the filled conte
-00015340: 6e74 2e0d 0a0d 0a20 2020 2020 2020 2052  nt.....        R
-00015350: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
-00015360: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-00015370: 2073 7461 626c 655f 7768 6973 7065 722e   stable_whisper.
-00015380: 7265 7375 6c74 2e57 6869 7370 6572 5265  result.WhisperRe
-00015390: 7375 6c74 0d0a 2020 2020 2020 2020 2020  sult..          
-000153a0: 2020 5468 6520 6375 7272 656e 7420 696e    The current in
-000153b0: 7374 616e 6365 2061 6674 6572 2074 6865  stance after the
-000153c0: 2063 6861 6e67 6573 2e0d 0a20 2020 2020   changes...     
-000153d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000153e0: 6966 206c 656e 2873 656c 662e 7365 676d  if len(self.segm
-000153f0: 656e 7473 2920 3c20 323a 0d0a 2020 2020  ents) < 2:..    
-00015400: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00015410: 656c 660d 0a20 2020 2020 2020 2069 6620  elf..        if 
-00015420: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
-00015430: 5f72 6573 756c 742c 2073 7472 293a 0d0a  _result, str):..
-00015440: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-00015450: 725f 7265 7375 6c74 203d 2057 6869 7370  r_result = Whisp
-00015460: 6572 5265 7375 6c74 286f 7468 6572 5f72  erResult(other_r
-00015470: 6573 756c 7429 0d0a 0d0a 2020 2020 2020  esult)....      
-00015480: 2020 6966 2073 7472 6970 3a0d 0a20 2020    if strip:..   
-00015490: 2020 2020 2020 2020 2064 6566 2073 7472           def str
-000154a0: 6970 5f73 7061 6365 2877 293a 0d0a 2020  ip_space(w):..  
-000154b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000154c0: 7475 726e 2077 2e73 7472 6970 2829 0d0a  turn w.strip()..
-000154d0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000154e0: 2020 2020 2020 2020 2020 2064 6566 2073             def s
-000154f0: 7472 6970 5f73 7061 6365 2877 293a 0d0a  trip_space(w):..
-00015500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015510: 7265 7475 726e 2077 0d0a 0d0a 2020 2020  return w....    
-00015520: 2020 2020 6966 2069 676e 6f72 655f 7075      if ignore_pu
-00015530: 6e63 7475 6174 696f 6e73 3a0d 0a20 2020  nctuations:..   
-00015540: 2020 2020 2020 2020 2070 746e 203d 2066           ptn = f
-00015550: 275b 7b69 676e 6f72 655f 7075 6e63 7475  '[{ignore_punctu
-00015560: 6174 696f 6e73 7d5d 2b24 270d 0a0d 0a20  ations}]+$'.... 
-00015570: 2020 2020 2020 2020 2020 2064 6566 2073             def s
-00015580: 7472 6970 5f70 756e 6374 7561 7469 6f6e  trip_punctuation
-00015590: 7328 7729 3a0d 0a20 2020 2020 2020 2020  s(w):..         
-000155a0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000155b0: 2e73 7562 2870 746e 2c20 2727 2c20 7374  .sub(ptn, '', st
-000155c0: 7269 705f 7370 6163 6528 7729 290d 0a20  rip_space(w)).. 
-000155d0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000155e0: 2020 2020 2020 2020 2020 7374 7269 705f            strip_
-000155f0: 7075 6e63 7475 6174 696f 6e73 203d 2073  punctuations = s
-00015600: 7472 6970 5f73 7061 6365 0d0a 0d0a 2020  trip_space....  
-00015610: 2020 2020 2020 6966 2063 6173 655f 7365        if case_se
-00015620: 6e73 6974 6976 653a 0d0a 2020 2020 2020  nsitive:..      
-00015630: 2020 2020 2020 7374 7269 7020 3d20 7374        strip = st
-00015640: 7269 705f 7075 6e63 7475 6174 696f 6e73  rip_punctuations
-00015650: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00015660: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-00015670: 2073 7472 6970 2877 293a 0d0a 2020 2020   strip(w):..    
-00015680: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00015690: 726e 2073 7472 6970 5f70 756e 6374 7561  rn strip_punctua
-000156a0: 7469 6f6e 7328 7729 2e6c 6f77 6572 2829  tions(w).lower()
-000156b0: 0d0a 0d0a 2020 2020 2020 2020 7365 675f  ....        seg_
-000156c0: 7061 6972 7320 3d20 6c69 7374 2865 6e75  pairs = list(enu
-000156d0: 6d65 7261 7465 287a 6970 2873 656c 662e  merate(zip(self.
-000156e0: 7365 676d 656e 7473 5b3a 2d31 5d2c 2073  segments[:-1], s
-000156f0: 656c 662e 7365 676d 656e 7473 5b31 3a5d  elf.segments[1:]
-00015700: 2929 290d 0a20 2020 2020 2020 2073 6567  )))..        seg
-00015710: 5f70 6169 7273 2e69 6e73 6572 7428 302c  _pairs.insert(0,
-00015720: 2028 2d31 2c20 284e 6f6e 652c 2073 656c   (-1, (None, sel
-00015730: 662e 7365 676d 656e 7473 5b30 5d29 2929  f.segments[0])))
-00015740: 0d0a 2020 2020 2020 2020 7365 675f 7061  ..        seg_pa
-00015750: 6972 732e 6170 7065 6e64 2828 7365 675f  irs.append((seg_
-00015760: 7061 6972 735b 2d31 5d5b 305d 2b31 2c20  pairs[-1][0]+1, 
-00015770: 2873 656c 662e 7365 676d 656e 7473 5b2d  (self.segments[-
-00015780: 315d 2c20 4e6f 6e65 2929 290d 0a0d 0a20  1], None))).... 
-00015790: 2020 2020 2020 2063 6861 6e67 6573 203d         changes =
-000157a0: 205b 5d0d 0a20 2020 2020 2020 2066 6f72   []..        for
-000157b0: 2069 2c20 2873 6567 302c 2073 6567 3129   i, (seg0, seg1)
-000157c0: 2069 6e20 7265 7665 7273 6564 2873 6567   in reversed(seg
-000157d0: 5f70 6169 7273 293a 0d0a 2020 2020 2020  _pairs):..      
-000157e0: 2020 2020 2020 6669 7273 745f 776f 7264        first_word
-000157f0: 203d 204e 6f6e 6520 6966 2073 6567 3020   = None if seg0 
-00015800: 6973 204e 6f6e 6520 656c 7365 2073 6567  is None else seg
-00015810: 302e 776f 7264 735b 2d31 5d0d 0a20 2020  0.words[-1]..   
-00015820: 2020 2020 2020 2020 206c 6173 745f 776f           last_wo
-00015830: 7264 203d 204e 6f6e 6520 6966 2073 6567  rd = None if seg
-00015840: 3120 6973 204e 6f6e 6520 656c 7365 2073  1 is None else s
-00015850: 6567 312e 776f 7264 735b 305d 0d0a 2020  eg1.words[0]..  
-00015860: 2020 2020 2020 2020 2020 7374 6172 7420            start 
-00015870: 3d20 286f 7468 6572 5f72 6573 756c 745b  = (other_result[
-00015880: 305d 2e73 7461 7274 2069 6620 6669 7273  0].start if firs
-00015890: 745f 776f 7264 2069 7320 4e6f 6e65 2065  t_word is None e
-000158a0: 6c73 6520 6669 7273 745f 776f 7264 2e65  lse first_word.e
-000158b0: 6e64 290d 0a20 2020 2020 2020 2020 2020  nd)..           
-000158c0: 2065 6e64 203d 206f 7468 6572 5f72 6573   end = other_res
-000158d0: 756c 745b 2d31 5d2e 656e 6420 6966 206c  ult[-1].end if l
-000158e0: 6173 745f 776f 7264 2069 7320 4e6f 6e65  ast_word is None
-000158f0: 2065 6c73 6520 6c61 7374 5f77 6f72 642e   else last_word.
-00015900: 7374 6172 740d 0a20 2020 2020 2020 2020  start..         
-00015910: 2020 2069 6620 656e 6420 2d20 7374 6172     if end - star
-00015920: 7420 3c3d 206d 696e 5f67 6170 3a0d 0a20  t <= min_gap:.. 
-00015930: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00015940: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
-00015950: 2020 2020 2067 6170 5f77 6f72 6473 203d       gap_words =
-00015960: 206f 7468 6572 5f72 6573 756c 742e 6765   other_result.ge
-00015970: 745f 636f 6e74 656e 745f 6279 5f74 696d  t_content_by_tim
-00015980: 6528 2873 7461 7274 2c20 656e 6429 290d  e((start, end)).
-00015990: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000159a0: 6669 7273 745f 776f 7264 2069 7320 6e6f  first_word is no
-000159b0: 7420 4e6f 6e65 2061 6e64 2067 6170 5f77  t None and gap_w
-000159c0: 6f72 6473 2061 6e64 2073 7472 6970 2866  ords and strip(f
-000159d0: 6972 7374 5f77 6f72 642e 776f 7264 2920  irst_word.word) 
-000159e0: 3d3d 2073 7472 6970 2867 6170 5f77 6f72  == strip(gap_wor
-000159f0: 6473 5b30 5d2e 776f 7264 293a 0d0a 2020  ds[0].word):..  
-00015a00: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00015a10: 7273 745f 776f 7264 2e65 6e64 203d 2067  rst_word.end = g
-00015a20: 6170 5f77 6f72 6473 5b30 5d2e 656e 640d  ap_words[0].end.
-00015a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015a40: 2067 6170 5f77 6f72 6473 203d 2067 6170   gap_words = gap
-00015a50: 5f77 6f72 6473 5b31 3a5d 0d0a 2020 2020  _words[1:]..    
-00015a60: 2020 2020 2020 2020 6966 206c 6173 745f          if last_
-00015a70: 776f 7264 2069 7320 6e6f 7420 4e6f 6e65  word is not None
-00015a80: 2061 6e64 2067 6170 5f77 6f72 6473 2061   and gap_words a
-00015a90: 6e64 2073 7472 6970 286c 6173 745f 776f  nd strip(last_wo
-00015aa0: 7264 2e77 6f72 6429 203d 3d20 7374 7269  rd.word) == stri
-00015ab0: 7028 6761 705f 776f 7264 735b 2d31 5d2e  p(gap_words[-1].
-00015ac0: 776f 7264 293a 0d0a 2020 2020 2020 2020  word):..        
-00015ad0: 2020 2020 2020 2020 6c61 7374 5f77 6f72          last_wor
-00015ae0: 642e 7374 6172 7420 3d20 6761 705f 776f  d.start = gap_wo
-00015af0: 7264 735b 2d31 5d2e 7374 6172 740d 0a20  rds[-1].start.. 
-00015b00: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00015b10: 6170 5f77 6f72 6473 203d 2067 6170 5f77  ap_words = gap_w
-00015b20: 6f72 6473 5b3a 2d31 5d0d 0a20 2020 2020  ords[:-1]..     
-00015b30: 2020 2020 2020 2069 6620 6e6f 7420 6761         if not ga
-00015b40: 705f 776f 7264 733a 0d0a 2020 2020 2020  p_words:..      
-00015b50: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00015b60: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00015b70: 6966 206c 6173 745f 776f 7264 2069 7320  if last_word is 
-00015b80: 6e6f 7420 4e6f 6e65 2061 6e64 206c 6173  not None and las
-00015b90: 745f 776f 7264 2e73 7461 7274 203c 2067  t_word.start < g
-00015ba0: 6170 5f77 6f72 6473 5b2d 315d 2e65 6e64  ap_words[-1].end
-00015bb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00015bc0: 2020 206c 6173 745f 776f 7264 2e73 7461     last_word.sta
-00015bd0: 7274 203d 2067 6170 5f77 6f72 6473 5b2d  rt = gap_words[-
-00015be0: 315d 2e65 6e64 0d0a 2020 2020 2020 2020  1].end..        
-00015bf0: 2020 2020 6e65 775f 7365 676d 656e 7473      new_segments
-00015c00: 203d 205b 6f74 6865 725f 7265 7375 6c74   = [other_result
-00015c10: 5b67 6170 5f77 6f72 6473 5b30 5d2e 7365  [gap_words[0].se
-00015c20: 676d 656e 745f 6964 5d2e 636f 7079 285b  gment_id].copy([
-00015c30: 5d29 5d0d 0a20 2020 2020 2020 2020 2020  ])]..           
-00015c40: 2066 6f72 206a 2c20 6e65 775f 776f 7264   for j, new_word
-00015c50: 2069 6e20 656e 756d 6572 6174 6528 6761   in enumerate(ga
-00015c60: 705f 776f 7264 7329 3a0d 0a20 2020 2020  p_words):..     
-00015c70: 2020 2020 2020 2020 2020 206e 6577 5f77             new_w
-00015c80: 6f72 645f 636f 7079 203d 206e 6577 5f77  ord_copy = new_w
-00015c90: 6f72 642e 636f 7079 2863 6f70 795f 746f  ord.copy(copy_to
-00015ca0: 6b65 6e73 3d54 7275 6529 0d0a 2020 2020  kens=True)..    
-00015cb0: 2020 2020 2020 2020 2020 2020 6966 206a              if j
-00015cc0: 203d 3d20 3020 616e 6420 6669 7273 745f   == 0 and first_
-00015cd0: 776f 7264 2069 7320 6e6f 7420 4e6f 6e65  word is not None
-00015ce0: 2061 6e64 2066 6972 7374 5f77 6f72 642e   and first_word.
-00015cf0: 656e 6420 3e20 6761 705f 776f 7264 735b  end > gap_words[
-00015d00: 305d 2e73 7461 7274 3a0d 0a20 2020 2020  0].start:..     
-00015d10: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00015d20: 6577 5f77 6f72 645f 636f 7079 2e73 7461  ew_word_copy.sta
-00015d30: 7274 203d 2066 6972 7374 5f77 6f72 642e  rt = first_word.
-00015d40: 656e 640d 0a20 2020 2020 2020 2020 2020  end..           
-00015d50: 2020 2020 2069 6620 6e65 775f 7365 676d       if new_segm
-00015d60: 656e 7473 5b2d 315d 2e69 6420 213d 206e  ents[-1].id != n
-00015d70: 6577 5f77 6f72 642e 7365 676d 656e 745f  ew_word.segment_
-00015d80: 6964 3a0d 0a20 2020 2020 2020 2020 2020  id:..           
-00015d90: 2020 2020 2020 2020 206e 6577 5f73 6567           new_seg
-00015da0: 6d65 6e74 732e 6170 7065 6e64 286f 7468  ments.append(oth
-00015db0: 6572 5f72 6573 756c 745b 6e65 775f 776f  er_result[new_wo
-00015dc0: 7264 2e73 6567 6d65 6e74 5f69 645d 2e63  rd.segment_id].c
-00015dd0: 6f70 7928 5b5d 2929 0d0a 2020 2020 2020  opy([]))..      
-00015de0: 2020 2020 2020 2020 2020 6e65 775f 7365            new_se
-00015df0: 676d 656e 7473 5b2d 315d 2e77 6f72 6473  gments[-1].words
-00015e00: 2e61 7070 656e 6428 6e65 775f 776f 7264  .append(new_word
-00015e10: 5f63 6f70 7929 0d0a 2020 2020 2020 2020  _copy)..        
-00015e20: 2020 2020 6966 2076 6572 626f 7365 3a0d      if verbose:.
-00015e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015e40: 2063 6861 6e67 6573 2e61 7070 656e 6428   changes.append(
-00015e50: 275c 6e27 2e6a 6f69 6e28 2741 6464 6564  '\n'.join('Added
-00015e60: 3a20 2720 2b20 732e 746f 5f64 6973 706c  : ' + s.to_displ
-00015e70: 6179 5f73 7472 2854 7275 6529 2066 6f72  ay_str(True) for
-00015e80: 2073 2069 6e20 6e65 775f 7365 676d 656e   s in new_segmen
-00015e90: 7473 2929 0d0a 2020 2020 2020 2020 2020  ts))..          
-00015ea0: 2020 7365 6c66 2e73 6567 6d65 6e74 7320    self.segments 
-00015eb0: 3d20 7365 6c66 2e73 6567 6d65 6e74 735b  = self.segments[
-00015ec0: 3a69 2b31 5d20 2b20 6e65 775f 7365 676d  :i+1] + new_segm
-00015ed0: 656e 7473 202b 2073 656c 662e 7365 676d  ents + self.segm
-00015ee0: 656e 7473 5b69 2b31 3a5d 0d0a 2020 2020  ents[i+1:]..    
-00015ef0: 2020 2020 6966 2063 6861 6e67 6573 3a0d      if changes:.
-00015f00: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00015f10: 6e74 2827 5c6e 272e 6a6f 696e 2872 6576  nt('\n'.join(rev
-00015f20: 6572 7365 6428 6368 616e 6765 7329 2929  ersed(changes)))
-00015f30: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-00015f40: 6561 7373 6967 6e5f 6964 7328 290d 0a0d  eassign_ids()...
-00015f50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00015f60: 7365 6c66 0d0a 0d0a 2020 2020 6465 6620  self....    def 
-00015f70: 7265 6772 6f75 7028 0d0a 2020 2020 2020  regroup(..      
-00015f80: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
-00015f90: 2020 2020 2020 2020 2072 6567 726f 7570           regroup
-00015fa0: 5f61 6c67 6f3a 2055 6e69 6f6e 5b73 7472  _algo: Union[str
-00015fb0: 2c20 626f 6f6c 5d20 3d20 4e6f 6e65 2c0d  , bool] = None,.
-00015fc0: 0a20 2020 2020 2020 2020 2020 2076 6572  .            ver
-00015fd0: 626f 7365 3a20 626f 6f6c 203d 2046 616c  bose: bool = Fal
-00015fe0: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-00015ff0: 206f 6e6c 795f 7368 6f77 3a20 626f 6f6c   only_show: bool
-00016000: 203d 2046 616c 7365 0d0a 2020 2020 2920   = False..    ) 
-00016010: 2d3e 2022 5768 6973 7065 7252 6573 756c  -> "WhisperResul
-00016020: 7422 3a0d 0a20 2020 2020 2020 2022 2222  t":..        """
-00016030: 0d0a 2020 2020 2020 2020 5265 6772 6f75  ..        Regrou
-00016040: 7020 2869 6e2d 706c 6163 6529 2077 6f72  p (in-place) wor
-00016050: 6473 2069 6e74 6f20 7365 676d 656e 7473  ds into segments
-00016060: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
-00016070: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
-00016080: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
-00016090: 2020 2020 2072 6567 726f 7570 5f61 6c67       regroup_alg
-000160a0: 6f3a 2073 7472 206f 7220 626f 6f6c 2c20  o: str or bool, 
-000160b0: 6465 6661 756c 7420 2764 6127 0d0a 2020  default 'da'..  
-000160c0: 2020 2020 2020 2020 2020 2053 7472 696e             Strin
-000160d0: 6720 7265 7072 6573 656e 7461 7469 6f6e  g representation
-000160e0: 206f 6620 6120 6375 7374 6f6d 2072 6567   of a custom reg
-000160f0: 726f 7570 696e 6720 616c 676f 7269 7468  rouping algorith
-00016100: 6d20 6f72 2060 6054 7275 6560 6020 7573  m or ``True`` us
-00016110: 6520 746f 2074 6865 2064 6566 6175 6c74  e to the default
-00016120: 2061 6c67 6f72 6974 686d 2027 6461 272e   algorithm 'da'.
-00016130: 0d0a 2020 2020 2020 2020 7665 7262 6f73  ..        verbos
-00016140: 6520 3a20 626f 6f6c 2c20 6465 6661 756c  e : bool, defaul
-00016150: 7420 4661 6c73 650d 0a20 2020 2020 2020  t False..       
-00016160: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00016170: 7368 6f77 2061 6c6c 2074 6865 206d 6574  show all the met
-00016180: 686f 6473 2061 6e64 2061 7267 756d 656e  hods and argumen
-00016190: 7473 2070 6172 7365 6420 6672 6f6d 2060  ts parsed from `
-000161a0: 6072 6567 726f 7570 5f61 6c67 6f60 602e  `regroup_algo``.
-000161b0: 0d0a 2020 2020 2020 2020 6f6e 6c79 5f73  ..        only_s
-000161c0: 686f 7720 3a20 626f 6f6c 2c20 6465 6661  how : bool, defa
-000161d0: 756c 7420 4661 6c73 650d 0a20 2020 2020  ult False..     
-000161e0: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
-000161f0: 6f20 7368 6f77 2074 6865 2061 6c6c 206d  o show the all m
-00016200: 6574 686f 6473 2061 6e64 2061 7267 756d  ethods and argum
-00016210: 656e 7473 2070 6172 7365 6420 6672 6f6d  ents parsed from
-00016220: 2060 6072 6567 726f 7570 5f61 6c67 6f60   ``regroup_algo`
-00016230: 6020 7769 7468 6f75 7420 7275 6e6e 696e  ` without runnin
-00016240: 6720 7468 6520 6d65 7468 6f64 730d 0a0d  g the methods...
-00016250: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00016260: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00016270: 2d0d 0a20 2020 2020 2020 2073 7461 626c  -..        stabl
-00016280: 655f 7768 6973 7065 722e 7265 7375 6c74  e_whisper.result
-00016290: 2e57 6869 7370 6572 5265 7375 6c74 0d0a  .WhisperResult..
-000162a0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-000162b0: 6375 7272 656e 7420 696e 7374 616e 6365  current instance
-000162c0: 2061 6674 6572 2074 6865 2063 6861 6e67   after the chang
-000162d0: 6573 2e0d 0a0d 0a20 2020 2020 2020 204e  es.....        N
-000162e0: 6f74 6573 0d0a 2020 2020 2020 2020 2d2d  otes..        --
-000162f0: 2d2d 2d0d 0a20 2020 2020 2020 2053 796e  ---..        Syn
-00016300: 7461 7820 666f 7220 7374 7269 6e67 2072  tax for string r
-00016310: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-00016320: 2063 7573 746f 6d20 7265 6772 6f75 7069   custom regroupi
-00016330: 6e67 2061 6c67 6f72 6974 686d 2e0d 0a20  ng algorithm... 
-00016340: 2020 2020 2020 2020 2020 204d 6574 686f             Metho
-00016350: 6420 6b65 7973 3a0d 0a20 2020 2020 2020  d keys:..       
-00016360: 2020 2020 2020 2020 2073 673a 2073 706c           sg: spl
-00016370: 6974 5f62 795f 6761 700d 0a20 2020 2020  it_by_gap..     
-00016380: 2020 2020 2020 2020 2020 2073 703a 2073             sp: s
-00016390: 706c 6974 5f62 795f 7075 6e63 7475 6174  plit_by_punctuat
-000163a0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-000163b0: 2020 2020 2073 6c3a 2073 706c 6974 5f62       sl: split_b
-000163c0: 795f 6c65 6e67 7468 0d0a 2020 2020 2020  y_length..      
-000163d0: 2020 2020 2020 2020 2020 7364 3a20 7370            sd: sp
-000163e0: 6c69 745f 6279 5f64 7572 6174 696f 6e0d  lit_by_duration.
-000163f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016400: 206d 673a 206d 6572 6765 5f62 795f 6761   mg: merge_by_ga
-00016410: 700d 0a20 2020 2020 2020 2020 2020 2020  p..             
-00016420: 2020 206d 703a 206d 6572 6765 5f62 795f     mp: merge_by_
-00016430: 7075 6e63 7475 6174 696f 6e0d 0a20 2020  punctuation..   
-00016440: 2020 2020 2020 2020 2020 2020 206d 733a               ms:
-00016450: 206d 6572 6765 5f61 6c6c 5f73 6567 6d65   merge_all_segme
-00016460: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-00016470: 2020 2020 636d 3a20 636c 616d 705f 6d61      cm: clamp_ma
-00016480: 780d 0a20 2020 2020 2020 2020 2020 2020  x..             
-00016490: 2020 206c 3a20 6c6f 636b 0d0a 2020 2020     l: lock..    
-000164a0: 2020 2020 2020 2020 2020 2020 7573 3a20              us: 
-000164b0: 756e 6c6f 636b 5f61 6c6c 5f73 6567 6d65  unlock_all_segme
-000164c0: 6e74 730d 0a20 2020 2020 2020 2020 2020  nts..           
-000164d0: 2020 2020 2064 613a 2064 6566 6175 6c74       da: default
-000164e0: 2061 6c67 6f72 6974 686d 2028 636d 5f73   algorithm (cm_s
-000164f0: 703d 2c2a 202f efbc 8c5f 7367 3d2e 355f  p=,* /..._sg=.5_
-00016500: 6d67 3d2e 332b 335f 7370 3d2e 2a20 2fe3  mg=.3+3_sp=.* /.
-00016510: 8082 2f3f 2fef bc9f 290d 0a20 2020 2020  ../?/...)..     
-00016520: 2020 2020 2020 2020 2020 2072 773a 2072             rw: r
-00016530: 656d 6f76 655f 776f 7264 0d0a 2020 2020  emove_word..    
-00016540: 2020 2020 2020 2020 2020 2020 7273 3a20              rs: 
-00016550: 7265 6d6f 7665 5f73 6567 6d65 6e74 0d0a  remove_segment..
-00016560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016570: 7270 3a20 7265 6d6f 7665 5f72 6570 6574  rp: remove_repet
-00016580: 6974 696f 6e0d 0a20 2020 2020 2020 2020  ition..         
-00016590: 2020 2020 2020 2072 7773 3a20 7265 6d6f         rws: remo
-000165a0: 7665 5f77 6f72 6473 5f62 795f 7374 720d  ve_words_by_str.
-000165b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000165c0: 2066 673a 2066 696c 6c5f 696e 5f67 6170   fg: fill_in_gap
-000165d0: 730d 0a20 2020 2020 2020 2020 2020 204d  s..            M
-000165e0: 6574 6163 6861 7261 6374 6572 733a 0d0a  etacharacters:..
-000165f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016600: 3d20 7365 7061 7261 7465 7320 6120 6d65  = separates a me
-00016610: 7468 6f64 206b 6579 2061 6e64 2069 7473  thod key and its
-00016620: 2061 7267 756d 656e 7473 2028 6e6f 7420   arguments (not 
-00016630: 7573 6564 2069 6620 6e6f 2061 7267 756d  used if no argum
-00016640: 656e 7429 0d0a 2020 2020 2020 2020 2020  ent)..          
-00016650: 2020 2020 2020 5f20 7365 7061 7261 7465        _ separate
-00016660: 7320 6d65 7468 6f64 206b 6579 7320 2861  s method keys (a
-00016670: 6674 6572 2061 7267 756d 656e 7473 2069  fter arguments i
-00016680: 6620 7468 6572 6520 6172 6520 616e 7929  f there are any)
-00016690: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000166a0: 2020 2b20 7365 7061 7261 7465 7320 6172    + separates ar
-000166b0: 6775 6d65 6e74 7320 666f 7220 6120 6d65  guments for a me
-000166c0: 7468 6f64 206b 6579 0d0a 2020 2020 2020  thod key..      
-000166d0: 2020 2020 2020 2020 2020 2f20 7365 7061            / sepa
-000166e0: 7261 7465 7320 616e 2061 7267 756d 656e  rates an argumen
-000166f0: 7420 696e 746f 206c 6973 7420 6f66 2073  t into list of s
-00016700: 7472 696e 6773 0d0a 2020 2020 2020 2020  trings..        
-00016710: 2020 2020 2020 2020 2a20 7365 7061 7261          * separa
-00016720: 7465 7320 616e 2069 7465 6d20 696e 206c  tes an item in l
-00016730: 6973 7420 6f66 2073 7472 696e 6773 2069  ist of strings i
-00016740: 6e74 6f20 6120 6e65 7374 6564 206c 6973  nto a nested lis
-00016750: 7420 6f66 2073 7472 696e 6773 0d0a 2020  t of strings..  
-00016760: 2020 2020 2020 2020 2020 4e6f 7465 733a            Notes:
-00016770: 0d0a 2020 2020 2020 2020 2020 2020 2d61  ..            -a
-00016780: 7267 756d 656e 7473 2061 7265 2070 6172  rguments are par
-00016790: 7365 6420 706f 7369 7469 6f6e 616c 6c79  sed positionally
-000167a0: 0d0a 2020 2020 2020 2020 2020 2020 2d69  ..            -i
-000167b0: 6620 6e6f 2061 7267 756d 656e 7420 6973  f no argument is
-000167c0: 2070 726f 7669 6465 642c 2074 6865 2064   provided, the d
-000167d0: 6566 6175 6c74 206f 6e65 7320 7769 6c6c  efault ones will
-000167e0: 2062 6520 7573 6564 0d0a 2020 2020 2020   be used..      
-000167f0: 2020 2020 2020 2d75 7365 2031 206f 7220        -use 1 or 
-00016800: 3020 746f 2072 6570 7265 7365 6e74 2054  0 to represent T
-00016810: 7275 6520 6f72 2046 616c 7365 0d0a 2020  rue or False..  
-00016820: 2020 2020 2020 2020 2020 4578 616d 706c            Exampl
-00016830: 6520 313a 0d0a 2020 2020 2020 2020 2020  e 1:..          
-00016840: 2020 2020 2020 6d65 7267 655f 6279 5f67        merge_by_g
-00016850: 6170 282e 322c 2031 302c 206c 6f63 6b3d  ap(.2, 10, lock=
-00016860: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
-00016870: 2020 2020 2020 206d 673d 2e32 2b31 302b         mg=.2+10+
-00016880: 2b2b 310d 0a20 2020 2020 2020 2020 2020  ++1..           
-00016890: 2020 2020 204e 6f74 653a 205b 6c6f 636b       Note: [lock
-000168a0: 5d20 6973 2074 6865 2035 7468 2061 7267  ] is the 5th arg
-000168b0: 756d 656e 7420 6865 6e63 6520 7468 6520  ument hence the 
-000168c0: 3220 6d69 7373 696e 6720 6172 6775 6d65  2 missing argume
-000168d0: 6e74 7320 696e 6265 7477 6565 6e20 7468  nts inbetween th
-000168e0: 6520 7468 7265 6520 2b20 6265 666f 7265  e three + before
-000168f0: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00016900: 4578 616d 706c 6520 323a 0d0a 2020 2020  Example 2:..    
-00016910: 2020 2020 2020 2020 2020 2020 7370 6c69              spli
-00016920: 745f 6279 5f70 756e 6374 7561 7469 6f6e  t_by_punctuation
-00016930: 285b 2827 2e27 2c20 2720 2729 2c20 27e3  ([('.', ' '), '.
-00016940: 8082 272c 2027 3f27 2c20 27ef bc9f 275d  ..', '?', '...']
-00016950: 2c20 5472 7565 290d 0a20 2020 2020 2020  , True)..       
-00016960: 2020 2020 2020 2020 2073 703d 2e2a 202f           sp=.* /
-00016970: e380 822f 3f2f efbc 9f2b 310d 0a20 2020  .../?/...+1..   
-00016980: 2020 2020 2020 2020 2045 7861 6d70 6c65           Example
-00016990: 2033 3a0d 0a20 2020 2020 2020 2020 2020   3:..           
-000169a0: 2020 2020 206d 6572 6765 5f61 6c6c 5f73       merge_all_s
-000169b0: 6567 6d65 6e74 7328 292e 7370 6c69 745f  egments().split_
-000169c0: 6279 5f67 6170 282e 3529 2e6d 6572 6765  by_gap(.5).merge
-000169d0: 5f62 795f 6761 7028 2e31 352c 2033 290d  _by_gap(.15, 3).
-000169e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000169f0: 206d 735f 7367 3d2e 355f 6d67 3d2e 3135   ms_sg=.5_mg=.15
-00016a00: 2b33 0d0a 2020 2020 2020 2020 2222 220d  +3..        """.
-00016a10: 0a20 2020 2020 2020 2069 6620 7265 6772  .        if regr
-00016a20: 6f75 705f 616c 676f 2069 7320 4661 6c73  oup_algo is Fals
-00016a30: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00016a40: 7265 7475 726e 2073 656c 660d 0a20 2020  return self..   
-00016a50: 2020 2020 2069 6620 7265 6772 6f75 705f       if regroup_
-00016a60: 616c 676f 2069 7320 4e6f 6e65 206f 7220  algo is None or 
-00016a70: 7265 6772 6f75 705f 616c 676f 2069 7320  regroup_algo is 
-00016a80: 5472 7565 3a0d 0a20 2020 2020 2020 2020  True:..         
-00016a90: 2020 2072 6567 726f 7570 5f61 6c67 6f20     regroup_algo 
-00016aa0: 3d20 2764 6127 0d0a 0d0a 2020 2020 2020  = 'da'....      
-00016ab0: 2020 666f 7220 6d65 7468 6f64 2c20 6b77    for method, kw
-00016ac0: 6172 6773 2c20 6d73 6720 696e 2073 656c  args, msg in sel
-00016ad0: 662e 7061 7273 655f 7265 6772 6f75 705f  f.parse_regroup_
-00016ae0: 616c 676f 2872 6567 726f 7570 5f61 6c67  algo(regroup_alg
-00016af0: 6f2c 2069 6e63 6c75 6465 5f73 7472 3d76  o, include_str=v
-00016b00: 6572 626f 7365 206f 7220 6f6e 6c79 5f73  erbose or only_s
-00016b10: 686f 7729 3a0d 0a20 2020 2020 2020 2020  how):..         
-00016b20: 2020 2069 6620 6d73 673a 0d0a 2020 2020     if msg:..    
-00016b30: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00016b40: 7428 6d73 6729 0d0a 2020 2020 2020 2020  t(msg)..        
-00016b50: 2020 2020 6966 206e 6f74 206f 6e6c 795f      if not only_
-00016b60: 7368 6f77 3a0d 0a20 2020 2020 2020 2020  show:..         
-00016b70: 2020 2020 2020 206d 6574 686f 6428 2a2a         method(**
-00016b80: 6b77 6172 6773 290d 0a0d 0a20 2020 2020  kwargs)....     
-00016b90: 2020 2072 6574 7572 6e20 7365 6c66 0d0a     return self..
-00016ba0: 0d0a 2020 2020 6465 6620 7061 7273 655f  ..    def parse_
-00016bb0: 7265 6772 6f75 705f 616c 676f 2873 656c  regroup_algo(sel
-00016bc0: 662c 2072 6567 726f 7570 5f61 6c67 6f3a  f, regroup_algo:
-00016bd0: 2073 7472 2c20 696e 636c 7564 655f 7374   str, include_st
-00016be0: 723a 2062 6f6f 6c20 3d20 5472 7565 2920  r: bool = True) 
-00016bf0: 2d3e 204c 6973 745b 5475 706c 655b 4361  -> List[Tuple[Ca
-00016c00: 6c6c 6162 6c65 2c20 6469 6374 2c20 7374  llable, dict, st
-00016c10: 725d 5d3a 0d0a 2020 2020 2020 2020 6d65  r]]:..        me
-00016c20: 7468 6f64 7320 3d20 6469 6374 280d 0a20  thods = dict(.. 
-00016c30: 2020 2020 2020 2020 2020 2073 673d 7365             sg=se
-00016c40: 6c66 2e73 706c 6974 5f62 795f 6761 702c  lf.split_by_gap,
-00016c50: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
-00016c60: 3d73 656c 662e 7370 6c69 745f 6279 5f70  =self.split_by_p
-00016c70: 756e 6374 7561 7469 6f6e 2c0d 0a20 2020  unctuation,..   
-00016c80: 2020 2020 2020 2020 2073 6c3d 7365 6c66           sl=self
-00016c90: 2e73 706c 6974 5f62 795f 6c65 6e67 7468  .split_by_length
-00016ca0: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00016cb0: 643d 7365 6c66 2e73 706c 6974 5f62 795f  d=self.split_by_
-00016cc0: 6475 7261 7469 6f6e 2c0d 0a20 2020 2020  duration,..     
-00016cd0: 2020 2020 2020 206d 673d 7365 6c66 2e6d         mg=self.m
-00016ce0: 6572 6765 5f62 795f 6761 702c 0d0a 2020  erge_by_gap,..  
-00016cf0: 2020 2020 2020 2020 2020 6d70 3d73 656c            mp=sel
-00016d00: 662e 6d65 7267 655f 6279 5f70 756e 6374  f.merge_by_punct
-00016d10: 7561 7469 6f6e 2c0d 0a20 2020 2020 2020  uation,..       
-00016d20: 2020 2020 206d 733d 7365 6c66 2e6d 6572       ms=self.mer
-00016d30: 6765 5f61 6c6c 5f73 6567 6d65 6e74 732c  ge_all_segments,
-00016d40: 0d0a 2020 2020 2020 2020 2020 2020 636d  ..            cm
-00016d50: 3d73 656c 662e 636c 616d 705f 6d61 782c  =self.clamp_max,
-00016d60: 0d0a 2020 2020 2020 2020 2020 2020 7573  ..            us
-00016d70: 3d73 656c 662e 756e 6c6f 636b 5f61 6c6c  =self.unlock_all
-00016d80: 5f73 6567 6d65 6e74 732c 0d0a 2020 2020  _segments,..    
-00016d90: 2020 2020 2020 2020 6c3d 7365 6c66 2e6c          l=self.l
-00016da0: 6f63 6b2c 0d0a 2020 2020 2020 2020 2020  ock,..          
-00016db0: 2020 7277 3d73 656c 662e 7265 6d6f 7665    rw=self.remove
-00016dc0: 5f77 6f72 642c 0d0a 2020 2020 2020 2020  _word,..        
-00016dd0: 2020 2020 7273 3d73 656c 662e 7265 6d6f      rs=self.remo
-00016de0: 7665 5f73 6567 6d65 6e74 2c0d 0a20 2020  ve_segment,..   
-00016df0: 2020 2020 2020 2020 2072 703d 7365 6c66           rp=self
-00016e00: 2e72 656d 6f76 655f 7265 7065 7469 7469  .remove_repetiti
-00016e10: 6f6e 2c0d 0a20 2020 2020 2020 2020 2020  on,..           
-00016e20: 2072 7773 3d73 656c 662e 7265 6d6f 7665   rws=self.remove
-00016e30: 5f77 6f72 6473 5f62 795f 7374 722c 0d0a  _words_by_str,..
-00016e40: 2020 2020 2020 2020 2020 2020 6667 3d73              fg=s
-00016e50: 656c 662e 6669 6c6c 5f69 6e5f 6761 7073  elf.fill_in_gaps
-00016e60: 2c0d 0a20 2020 2020 2020 2029 0d0a 2020  ,..        )..  
-00016e70: 2020 2020 2020 6966 206e 6f74 2072 6567        if not reg
-00016e80: 726f 7570 5f61 6c67 6f3a 0d0a 2020 2020  roup_algo:..    
-00016e90: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-00016ea0: 5d0d 0a0d 0a20 2020 2020 2020 2063 616c  ]....        cal
-00016eb0: 6c73 203d 2072 6567 726f 7570 5f61 6c67  ls = regroup_alg
-00016ec0: 6f2e 7370 6c69 7428 275f 2729 0d0a 2020  o.split('_')..  
-00016ed0: 2020 2020 2020 6966 2027 6461 2720 696e        if 'da' in
-00016ee0: 2063 616c 6c73 3a0d 0a20 2020 2020 2020   calls:..       
-00016ef0: 2020 2020 2064 6566 6175 6c74 5f63 616c       default_cal
-00016f00: 6c73 203d 2027 636d 5f73 703d 2c2a 202f  ls = 'cm_sp=,* /
-00016f10: efbc 8c5f 7367 3d2e 355f 6d67 3d2e 332b  ..._sg=.5_mg=.3+
-00016f20: 335f 7370 3d2e 2a20 2fe3 8082 2f3f 2fef  3_sp=.* /.../?/.
-00016f30: bc9f 272e 7370 6c69 7428 275f 2729 0d0a  ..'.split('_')..
-00016f40: 2020 2020 2020 2020 2020 2020 6361 6c6c              call
-00016f50: 7320 3d20 6368 6169 6e2e 6672 6f6d 5f69  s = chain.from_i
-00016f60: 7465 7261 626c 6528 6465 6661 756c 745f  terable(default_
-00016f70: 6361 6c6c 7320 6966 206d 6574 686f 6420  calls if method 
-00016f80: 3d3d 2027 6461 2720 656c 7365 205b 6d65  == 'da' else [me
-00016f90: 7468 6f64 5d20 666f 7220 6d65 7468 6f64  thod] for method
-00016fa0: 2069 6e20 6361 6c6c 7329 0d0a 2020 2020   in calls)..    
-00016fb0: 2020 2020 6f70 6572 6174 696f 6e73 203d      operations =
-00016fc0: 205b 5d0d 0a20 2020 2020 2020 2066 6f72   []..        for
-00016fd0: 206d 6574 686f 6420 696e 2063 616c 6c73   method in calls
-00016fe0: 3a0d 0a20 2020 2020 2020 2020 2020 206d  :..            m
-00016ff0: 6574 686f 642c 2061 7267 7320 3d20 6d65  ethod, args = me
-00017000: 7468 6f64 2e73 706c 6974 2827 3d27 2c20  thod.split('=', 
-00017010: 6d61 7873 706c 6974 3d31 2920 6966 2027  maxsplit=1) if '
-00017020: 3d27 2069 6e20 6d65 7468 6f64 2065 6c73  =' in method els
-00017030: 6520 286d 6574 686f 642c 2027 2729 0d0a  e (method, '')..
-00017040: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-00017050: 6574 686f 6420 6e6f 7420 696e 206d 6574  ethod not in met
-00017060: 686f 6473 3a0d 0a20 2020 2020 2020 2020  hods:..         
-00017070: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-00017080: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-00017090: 2866 277b 6d65 7468 6f64 7d20 6973 206e  (f'{method} is n
-000170a0: 6f74 206f 6e65 206f 6620 7468 6520 6176  ot one of the av
-000170b0: 6169 6c61 626c 6520 6d65 7468 6f64 733a  ailable methods:
-000170c0: 207b 7475 706c 6528 6d65 7468 6f64 732e   {tuple(methods.
-000170d0: 6b65 7973 2829 297d 2729 0d0a 2020 2020  keys())}')..    
-000170e0: 2020 2020 2020 2020 6172 6773 203d 205b          args = [
-000170f0: 5d20 6966 206c 656e 2861 7267 7329 203d  ] if len(args) =
-00017100: 3d20 3020 656c 7365 206c 6973 7428 6d61  = 0 else list(ma
-00017110: 7028 7374 725f 746f 5f76 616c 6964 5f74  p(str_to_valid_t
-00017120: 7970 652c 2061 7267 732e 7370 6c69 7428  ype, args.split(
-00017130: 272b 2729 2929 0d0a 2020 2020 2020 2020  '+')))..        
-00017140: 2020 2020 6b77 6172 6773 203d 207b 6b3a      kwargs = {k:
-00017150: 2076 2066 6f72 206b 2c20 7620 696e 207a   v for k, v in z
-00017160: 6970 286d 6574 686f 6473 5b6d 6574 686f  ip(methods[metho
-00017170: 645d 2e5f 5f63 6f64 655f 5f2e 636f 5f76  d].__code__.co_v
-00017180: 6172 6e61 6d65 735b 313a 5d2c 2061 7267  arnames[1:], arg
-00017190: 7329 2069 6620 7620 6973 206e 6f74 204e  s) if v is not N
-000171a0: 6f6e 657d 0d0a 2020 2020 2020 2020 2020  one}..          
-000171b0: 2020 6966 2069 6e63 6c75 6465 5f73 7472    if include_str
-000171c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000171d0: 2020 206b 7761 7267 735f 7374 7220 3d20     kwargs_str = 
-000171e0: 272c 2027 2e6a 6f69 6e28 6627 7b6b 7d3d  ', '.join(f'{k}=
-000171f0: 227b 767d 2227 2069 6620 6973 696e 7374  "{v}"' if isinst
-00017200: 616e 6365 2876 2c20 7374 7229 2065 6c73  ance(v, str) els
-00017210: 6520 6627 7b6b 7d3d 7b76 7d27 2066 6f72  e f'{k}={v}' for
-00017220: 206b 2c20 7620 696e 206b 7761 7267 732e   k, v in kwargs.
-00017230: 6974 656d 7328 2929 0d0a 2020 2020 2020  items())..      
-00017240: 2020 2020 2020 2020 2020 6f70 5f73 7472            op_str
-00017250: 203d 2066 277b 6d65 7468 6f64 735b 6d65   = f'{methods[me
-00017260: 7468 6f64 5d2e 5f5f 6e61 6d65 5f5f 7d28  thod].__name__}(
-00017270: 7b6b 7761 7267 735f 7374 727d 2927 0d0a  {kwargs_str})'..
-00017280: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00017290: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000172a0: 2020 206f 705f 7374 7220 3d20 4e6f 6e65     op_str = None
-000172b0: 0d0a 2020 2020 2020 2020 2020 2020 6f70  ..            op
-000172c0: 6572 6174 696f 6e73 2e61 7070 656e 6428  erations.append(
-000172d0: 286d 6574 686f 6473 5b6d 6574 686f 645d  (methods[method]
-000172e0: 2c20 6b77 6172 6773 2c20 6f70 5f73 7472  , kwargs, op_str
-000172f0: 2929 0d0a 0d0a 2020 2020 2020 2020 7265  ))....        re
-00017300: 7475 726e 206f 7065 7261 7469 6f6e 730d  turn operations.
-00017310: 0a0d 0a20 2020 2064 6566 2066 696e 6428  ...    def find(
-00017320: 7365 6c66 2c20 7061 7474 6572 6e3a 2073  self, pattern: s
-00017330: 7472 2c20 776f 7264 5f6c 6576 656c 3d54  tr, word_level=T
-00017340: 7275 652c 2066 6c61 6773 3d4e 6f6e 6529  rue, flags=None)
-00017350: 202d 3e20 2257 6869 7370 6572 5265 7375   -> "WhisperResu
-00017360: 6c74 4d61 7463 6865 7322 3a0d 0a20 2020  ltMatches":..   
-00017370: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00017380: 2020 4669 6e64 2073 6567 6d65 6e74 732f    Find segments/
-00017390: 776f 7264 7320 616e 6420 7469 6d65 7374  words and timest
-000173a0: 616d 7073 2077 6974 6820 7265 6775 6c61  amps with regula
-000173b0: 7220 6578 7072 6573 7369 6f6e 2e0d 0a0d  r expression....
-000173c0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-000173d0: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
-000173e0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-000173f0: 2070 6174 7465 726e 203a 2073 7472 0d0a   pattern : str..
-00017400: 2020 2020 2020 2020 2020 2020 5265 6745              RegE
-00017410: 7820 7061 7474 6572 6e20 746f 2073 6561  x pattern to sea
-00017420: 7263 6820 666f 722e 0d0a 2020 2020 2020  rch for...      
-00017430: 2020 776f 7264 5f6c 6576 656c 203a 2062    word_level : b
-00017440: 6f6f 6c2c 2064 6566 6175 6c74 2054 7275  ool, default Tru
-00017450: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
-00017460: 6865 7468 6572 2074 6f20 7365 6172 6368  hether to search
-00017470: 2061 7420 776f 7264 2d6c 6576 656c 2e0d   at word-level..
-00017480: 0a20 2020 2020 2020 2066 6c61 6773 203a  .        flags :
-00017490: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-000174a0: 2020 2020 2020 2052 6567 4578 2066 6c61         RegEx fla
-000174b0: 6773 2e0d 0a0d 0a20 2020 2020 2020 2052  gs.....        R
-000174c0: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
-000174d0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-000174e0: 2073 7461 626c 655f 7768 6973 7065 722e   stable_whisper.
-000174f0: 7265 7375 6c74 2e57 6869 7370 6572 5265  result.WhisperRe
-00017500: 7375 6c74 4d61 7463 6865 730d 0a20 2020  sultMatches..   
-00017510: 2020 2020 2020 2020 2041 6e20 696e 7374           An inst
-00017520: 616e 6365 206f 6620 3a63 6c61 7373 3a60  ance of :class:`
-00017530: 7374 6162 6c65 5f77 6869 7370 6572 2e72  stable_whisper.r
-00017540: 6573 756c 742e 5768 6973 7065 7252 6573  esult.WhisperRes
-00017550: 756c 744d 6174 6368 6573 6020 7769 7468  ultMatches` with
-00017560: 2077 6f72 642f 7365 676d 656e 7420 7468   word/segment th
-00017570: 6174 206d 6174 6368 2060 6070 6174 7465  at match ``patte
-00017580: 726e 6060 2e0d 0a20 2020 2020 2020 2022  rn``...        "
-00017590: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-000175a0: 726e 2057 6869 7370 6572 5265 7375 6c74  rn WhisperResult
-000175b0: 4d61 7463 6865 7328 7365 6c66 292e 6669  Matches(self).fi
-000175c0: 6e64 2870 6174 7465 726e 2c20 776f 7264  nd(pattern, word
-000175d0: 5f6c 6576 656c 3d77 6f72 645f 6c65 7665  _level=word_leve
-000175e0: 6c2c 2066 6c61 6773 3d66 6c61 6773 290d  l, flags=flags).
-000175f0: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-00017600: 0d0a 2020 2020 6465 6620 7465 7874 2873  ..    def text(s
-00017610: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00017620: 6574 7572 6e20 2727 2e6a 6f69 6e28 732e  eturn ''.join(s.
-00017630: 7465 7874 2066 6f72 2073 2069 6e20 7365  text for s in se
-00017640: 6c66 2e73 6567 6d65 6e74 7329 0d0a 0d0a  lf.segments)....
-00017650: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-00017660: 2020 2064 6566 2072 6567 726f 7570 5f68     def regroup_h
-00017670: 6973 746f 7279 2873 656c 6629 3a0d 0a20  istory(self):.. 
-00017680: 2020 2020 2020 2023 2073 616d 6520 7379         # same sy
-00017690: 6e74 6178 2061 7320 6060 7265 6772 6f75  ntax as ``regrou
-000176a0: 705f 616c 676f 6060 2066 6f72 203a 6d65  p_algo`` for :me
-000176b0: 7468 3a60 6072 6573 756c 742e 5768 6973  th:``result.Whis
-000176c0: 7065 7252 6573 756c 742e 7265 6772 6f75  perResult.regrou
-000176d0: 7060 0d0a 2020 2020 2020 2020 7265 7475  p`..        retu
-000176e0: 726e 2073 656c 662e 5f72 6567 726f 7570  rn self._regroup
-000176f0: 5f68 6973 746f 7279 0d0a 0d0a 2020 2020  _history....    
-00017700: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
-00017710: 6566 206e 6f6e 7370 6565 6368 5f73 6563  ef nonspeech_sec
-00017720: 7469 6f6e 7328 7365 6c66 293a 0d0a 2020  tions(self):..  
-00017730: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00017740: 662e 5f6e 6f6e 7370 6565 6368 5f73 6563  f._nonspeech_sec
-00017750: 7469 6f6e 730d 0a0d 0a20 2020 2064 6566  tions....    def
-00017760: 2073 686f 775f 7265 6772 6f75 705f 6869   show_regroup_hi
-00017770: 7374 6f72 7928 7365 6c66 293a 0d0a 2020  story(self):..  
-00017780: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00017790: 2020 2050 7269 6e74 2064 6574 6169 6c73     Print details
-000177a0: 206f 6620 616c 6c20 7265 6772 6f75 7069   of all regroupi
-000177b0: 6e67 206f 7065 7261 7469 6f6e 7320 7468  ng operations th
-000177c0: 6174 2062 6565 6e20 7065 7266 6f72 6d65  at been performe
-000177d0: 6420 6f6e 2064 6174 612e 0d0a 2020 2020  d on data...    
-000177e0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000177f0: 2069 6620 6e6f 7420 7365 6c66 2e5f 7265   if not self._re
-00017800: 6772 6f75 705f 6869 7374 6f72 793a 0d0a  group_history:..
-00017810: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00017820: 7428 2752 6573 756c 7420 6861 7320 6e6f  t('Result has no
-00017830: 2068 6973 746f 7279 2e27 290d 0a20 2020   history.')..   
-00017840: 2020 2020 2066 6f72 202a 5f2c 206d 7367       for *_, msg
-00017850: 2069 6e20 7365 6c66 2e70 6172 7365 5f72   in self.parse_r
-00017860: 6567 726f 7570 5f61 6c67 6f28 7365 6c66  egroup_algo(self
-00017870: 2e5f 7265 6772 6f75 705f 6869 7374 6f72  ._regroup_histor
-00017880: 7929 3a0d 0a20 2020 2020 2020 2020 2020  y):..           
-00017890: 2070 7269 6e74 2866 272e 7b6d 7367 7d27   print(f'.{msg}'
-000178a0: 290d 0a0d 0a20 2020 2064 6566 205f 5f6c  )....    def __l
-000178b0: 656e 5f5f 2873 656c 6629 3a0d 0a20 2020  en__(self):..   
-000178c0: 2020 2020 2072 6574 7572 6e20 6c65 6e28       return len(
-000178d0: 7365 6c66 2e73 6567 6d65 6e74 7329 0d0a  self.segments)..
-000178e0: 0d0a 2020 2020 6465 6620 756e 6c6f 636b  ..    def unlock
-000178f0: 5f61 6c6c 5f73 6567 6d65 6e74 7328 7365  _all_segments(se
-00017900: 6c66 293a 0d0a 2020 2020 2020 2020 666f  lf):..        fo
-00017910: 7220 7320 696e 2073 656c 662e 7365 676d  r s in self.segm
-00017920: 656e 7473 3a0d 0a20 2020 2020 2020 2020  ents:..         
-00017930: 2020 2073 2e75 6e6c 6f63 6b5f 616c 6c5f     s.unlock_all_
-00017940: 776f 7264 7328 290d 0a20 2020 2020 2020  words()..       
-00017950: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
-00017960: 2020 2020 6465 6620 7265 7365 7428 7365      def reset(se
-00017970: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
-00017980: 220d 0a20 2020 2020 2020 2052 6573 746f  "..        Resto
-00017990: 7265 2061 6c6c 2076 616c 7565 7320 746f  re all values to
-000179a0: 2074 6861 7420 6174 2069 6e69 7469 616c   that at initial
-000179b0: 697a 6174 696f 6e2e 0d0a 2020 2020 2020  ization...      
-000179c0: 2020 2222 220d 0a20 2020 2020 2020 2073    """..        s
-000179d0: 656c 662e 6c61 6e67 7561 6765 203d 2073  elf.language = s
-000179e0: 656c 662e 6f72 695f 6469 6374 2e67 6574  elf.ori_dict.get
-000179f0: 2827 6c61 6e67 7561 6765 2729 0d0a 2020  ('language')..  
-00017a00: 2020 2020 2020 7365 6c66 2e5f 7265 6772        self._regr
-00017a10: 6f75 705f 6869 7374 6f72 7920 3d20 2727  oup_history = ''
-00017a20: 0d0a 2020 2020 2020 2020 7365 676d 656e  ..        segmen
-00017a30: 7473 203d 2073 656c 662e 6f72 695f 6469  ts = self.ori_di
-00017a40: 6374 2e67 6574 2827 7365 676d 656e 7473  ct.get('segments
-00017a50: 2729 0d0a 2020 2020 2020 2020 7365 6c66  ')..        self
-00017a60: 2e73 6567 6d65 6e74 7320 3d20 5b53 6567  .segments = [Seg
-00017a70: 6d65 6e74 282a 2a73 2c20 6967 6e6f 7265  ment(**s, ignore
-00017a80: 5f75 6e75 7365 645f 6172 6773 3d54 7275  _unused_args=Tru
-00017a90: 6529 2066 6f72 2073 2069 6e20 7365 676d  e) for s in segm
-00017aa0: 656e 7473 5d20 6966 2073 6567 6d65 6e74  ents] if segment
-00017ab0: 7320 656c 7365 205b 5d0d 0a20 2020 2020  s else []..     
-00017ac0: 2020 2069 6620 7365 6c66 2e5f 666f 7263     if self._forc
-00017ad0: 6564 5f6f 7264 6572 3a0d 0a20 2020 2020  ed_order:..     
-00017ae0: 2020 2020 2020 2073 656c 662e 666f 7263         self.forc
-00017af0: 655f 6f72 6465 7228 290d 0a20 2020 2020  e_order()..     
-00017b00: 2020 2073 656c 662e 7265 6d6f 7665 5f6e     self.remove_n
-00017b10: 6f5f 776f 7264 5f73 6567 6d65 6e74 7328  o_word_segments(
-00017b20: 616e 7928 7365 672e 6861 735f 776f 7264  any(seg.has_word
-00017b30: 7320 666f 7220 7365 6720 696e 2073 656c  s for seg in sel
-00017b40: 662e 7365 676d 656e 7473 2929 0d0a 0d0a  f.segments))....
-00017b50: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-00017b60: 2020 2064 6566 2068 6173 5f77 6f72 6473     def has_words
-00017b70: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00017b80: 2072 6574 7572 6e20 626f 6f6c 2873 656c   return bool(sel
-00017b90: 662e 7365 676d 656e 7473 2920 616e 6420  f.segments) and 
-00017ba0: 616c 6c28 7365 672e 6861 735f 776f 7264  all(seg.has_word
-00017bb0: 7320 666f 7220 7365 6720 696e 2073 656c  s for seg in sel
-00017bc0: 662e 7365 676d 656e 7473 290d 0a0d 0a20  f.segments).... 
-00017bd0: 2020 2074 6f5f 7372 745f 7674 7420 3d20     to_srt_vtt = 
-00017be0: 7265 7375 6c74 5f74 6f5f 7372 745f 7674  result_to_srt_vt
-00017bf0: 740d 0a20 2020 2074 6f5f 6173 7320 3d20  t..    to_ass = 
-00017c00: 7265 7375 6c74 5f74 6f5f 6173 730d 0a20  result_to_ass.. 
-00017c10: 2020 2074 6f5f 7473 7620 3d20 7265 7375     to_tsv = resu
-00017c20: 6c74 5f74 6f5f 7473 760d 0a20 2020 2074  lt_to_tsv..    t
-00017c30: 6f5f 7478 7420 3d20 7265 7375 6c74 5f74  o_txt = result_t
-00017c40: 6f5f 7478 740d 0a20 2020 2073 6176 655f  o_txt..    save_
-00017c50: 6173 5f6a 736f 6e20 3d20 7361 7665 5f61  as_json = save_a
-00017c60: 735f 6a73 6f6e 0d0a 0d0a 0d0a 636c 6173  s_json......clas
-00017c70: 7320 5365 676d 656e 744d 6174 6368 3a0d  s SegmentMatch:.
-00017c80: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-00017c90: 745f 5f28 0d0a 2020 2020 2020 2020 2020  t__(..          
-00017ca0: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-00017cb0: 2020 2020 2073 6567 6d65 6e74 733a 2055       segments: U
-00017cc0: 6e69 6f6e 5b4c 6973 745b 5365 676d 656e  nion[List[Segmen
-00017cd0: 745d 2c20 5365 676d 656e 745d 2c0d 0a20  t], Segment],.. 
-00017ce0: 2020 2020 2020 2020 2020 205f 776f 7264             _word
-00017cf0: 5f69 6e64 6963 6573 3a20 4c69 7374 5b4c  _indices: List[L
-00017d00: 6973 745b 696e 745d 5d20 3d20 4e6f 6e65  ist[int]] = None
-00017d10: 2c0d 0a20 2020 2020 2020 2020 2020 205f  ,..            _
-00017d20: 7465 7874 5f6d 6174 6368 3a20 7374 7220  text_match: str 
-00017d30: 3d20 4e6f 6e65 0d0a 2020 2020 293a 0d0a  = None..    ):..
-00017d40: 2020 2020 2020 2020 7365 6c66 2e73 6567          self.seg
-00017d50: 6d65 6e74 7320 3d20 5b73 6567 6d65 6e74  ments = [segment
-00017d60: 735d 2069 6620 6973 696e 7374 616e 6365  s] if isinstance
-00017d70: 2873 6567 6d65 6e74 732c 2053 6567 6d65  (segments, Segme
-00017d80: 6e74 2920 656c 7365 2073 6567 6d65 6e74  nt) else segment
-00017d90: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-00017da0: 776f 7264 5f69 6e64 6963 6573 203d 205b  word_indices = [
-00017db0: 5d20 6966 205f 776f 7264 5f69 6e64 6963  ] if _word_indic
-00017dc0: 6573 2069 7320 4e6f 6e65 2065 6c73 6520  es is None else 
-00017dd0: 5f77 6f72 645f 696e 6469 6365 730d 0a20  _word_indices.. 
-00017de0: 2020 2020 2020 2073 656c 662e 776f 7264         self.word
-00017df0: 7320 3d20 5b73 656c 662e 7365 676d 656e  s = [self.segmen
-00017e00: 7473 5b69 5d2e 776f 7264 735b 6a5d 2066  ts[i].words[j] f
-00017e10: 6f72 2069 2c20 696e 6469 6365 7320 696e  or i, indices in
-00017e20: 2065 6e75 6d65 7261 7465 2873 656c 662e   enumerate(self.
-00017e30: 776f 7264 5f69 6e64 6963 6573 2920 666f  word_indices) fo
-00017e40: 7220 6a20 696e 2069 6e64 6963 6573 5d0d  r j in indices].
-00017e50: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00017e60: 7365 6c66 2e77 6f72 6473 2920 213d 2030  self.words) != 0
-00017e70: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00017e80: 656c 662e 7465 7874 203d 2027 272e 6a6f  elf.text = ''.jo
-00017e90: 696e 280d 0a20 2020 2020 2020 2020 2020  in(..           
-00017ea0: 2020 2020 2073 656c 662e 7365 676d 656e       self.segmen
-00017eb0: 7473 5b69 5d2e 776f 7264 735b 6a5d 2e77  ts[i].words[j].w
-00017ec0: 6f72 640d 0a20 2020 2020 2020 2020 2020  ord..           
-00017ed0: 2020 2020 2066 6f72 2069 2c20 696e 6469       for i, indi
-00017ee0: 6365 7320 696e 2065 6e75 6d65 7261 7465  ces in enumerate
-00017ef0: 2873 656c 662e 776f 7264 5f69 6e64 6963  (self.word_indic
-00017f00: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
-00017f10: 2020 2020 2066 6f72 206a 2069 6e20 696e       for j in in
-00017f20: 6469 6365 730d 0a20 2020 2020 2020 2020  dices..         
-00017f30: 2020 2029 0d0a 2020 2020 2020 2020 656c     )..        el
-00017f40: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00017f50: 2073 656c 662e 7465 7874 203d 2027 272e   self.text = ''.
-00017f60: 6a6f 696e 2873 6567 2e74 6578 7420 666f  join(seg.text fo
-00017f70: 7220 7365 6720 696e 2073 656c 662e 7365  r seg in self.se
-00017f80: 676d 656e 7473 290d 0a20 2020 2020 2020  gments)..       
-00017f90: 2073 656c 662e 7465 7874 5f6d 6174 6368   self.text_match
-00017fa0: 203d 205f 7465 7874 5f6d 6174 6368 0d0a   = _text_match..
-00017fb0: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-00017fc0: 0a20 2020 2064 6566 2073 7461 7274 2873  .    def start(s
-00017fd0: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00017fe0: 6574 7572 6e20 280d 0a20 2020 2020 2020  eturn (..       
-00017ff0: 2020 2020 2073 656c 662e 776f 7264 735b       self.words[
-00018000: 305d 2e73 7461 7274 0d0a 2020 2020 2020  0].start..      
-00018010: 2020 2020 2020 6966 206c 656e 2873 656c        if len(sel
-00018020: 662e 776f 7264 7329 2021 3d20 3020 656c  f.words) != 0 el
-00018030: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-00018040: 2873 656c 662e 7365 676d 656e 7473 5b30  (self.segments[0
-00018050: 5d2e 7374 6172 7420 6966 206c 656e 2873  ].start if len(s
-00018060: 656c 662e 7365 676d 656e 7473 2920 213d  elf.segments) !=
-00018070: 2030 2065 6c73 6520 4e6f 6e65 290d 0a20   0 else None).. 
-00018080: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-00018090: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
-000180a0: 6566 2065 6e64 2873 656c 6629 3a0d 0a20  ef end(self):.. 
-000180b0: 2020 2020 2020 2072 6574 7572 6e20 280d         return (.
-000180c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000180d0: 662e 776f 7264 735b 2d31 5d2e 656e 640d  f.words[-1].end.
-000180e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000180f0: 6c65 6e28 7365 6c66 2e77 6f72 6473 2920  len(self.words) 
-00018100: 213d 2030 2065 6c73 650d 0a20 2020 2020  != 0 else..     
-00018110: 2020 2020 2020 2028 7365 6c66 2e73 6567         (self.seg
-00018120: 6d65 6e74 735b 2d31 5d2e 656e 6420 6966  ments[-1].end if
-00018130: 206c 656e 2873 656c 662e 7365 676d 656e   len(self.segmen
-00018140: 7473 2920 213d 2030 2065 6c73 6520 4e6f  ts) != 0 else No
-00018150: 6e65 290d 0a20 2020 2020 2020 2029 0d0a  ne)..        )..
-00018160: 0d0a 2020 2020 6465 6620 5f5f 6c65 6e5f  ..    def __len_
-00018170: 5f28 7365 6c66 293a 0d0a 2020 2020 2020  _(self):..      
-00018180: 2020 7265 7475 726e 206c 656e 2873 656c    return len(sel
-00018190: 662e 7365 676d 656e 7473 290d 0a0d 0a20  f.segments).... 
-000181a0: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
-000181b0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000181c0: 7265 7475 726e 2073 656c 662e 5f5f 6469  return self.__di
-000181d0: 6374 5f5f 2e5f 5f72 6570 725f 5f28 290d  ct__.__repr__().
-000181e0: 0a0d 0a20 2020 2064 6566 205f 5f73 7472  ...    def __str
-000181f0: 5f5f 2873 656c 6629 3a0d 0a20 2020 2020  __(self):..     
-00018200: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00018210: 5f64 6963 745f 5f2e 5f5f 7374 725f 5f28  _dict__.__str__(
-00018220: 290d 0a0d 0a0d 0a63 6c61 7373 2057 6869  )......class Whi
-00018230: 7370 6572 5265 7375 6c74 4d61 7463 6865  sperResultMatche
-00018240: 733a 0d0a 2020 2020 2222 220d 0a20 2020  s:..    """..   
-00018250: 2052 6567 4578 206d 6174 6368 6573 2066   RegEx matches f
-00018260: 6f72 2057 6869 7370 6572 5265 7375 6c74  or WhisperResult
-00018270: 732e 0d0a 2020 2020 2222 220d 0a20 2020  s...    """..   
-00018280: 2023 2055 7365 2057 6869 7370 6572 5265   # Use WhisperRe
-00018290: 7375 6c74 2e66 696e 6428 2920 696e 7374  sult.find() inst
-000182a0: 6561 6420 6f66 2069 6e73 7461 6e74 6961  ead of instantia
-000182b0: 7469 6e67 2074 6869 7320 636c 6173 7320  ting this class 
-000182c0: 6469 7265 6374 6c79 2e0d 0a20 2020 2064  directly...    d
-000182d0: 6566 205f 5f69 6e69 745f 5f28 0d0a 2020  ef __init__(..  
-000182e0: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
-000182f0: 0a20 2020 2020 2020 2020 2020 206d 6174  .            mat
-00018300: 6368 6573 3a20 556e 696f 6e5b 4c69 7374  ches: Union[List
-00018310: 5b53 6567 6d65 6e74 4d61 7463 685d 2c20  [SegmentMatch], 
-00018320: 5768 6973 7065 7252 6573 756c 745d 2c0d  WhisperResult],.
-00018330: 0a20 2020 2020 2020 2020 2020 205f 7365  .            _se
-00018340: 676d 656e 745f 696e 6469 6365 733a 204c  gment_indices: L
-00018350: 6973 745b 4c69 7374 5b69 6e74 5d5d 203d  ist[List[int]] =
-00018360: 204e 6f6e 650d 0a20 2020 2029 3a0d 0a20   None..    ):.. 
-00018370: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00018380: 616e 6365 286d 6174 6368 6573 2c20 5768  ance(matches, Wh
-00018390: 6973 7065 7252 6573 756c 7429 3a0d 0a20  isperResult):.. 
-000183a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000183b0: 6d61 7463 6865 7320 3d20 6c69 7374 286d  matches = list(m
-000183c0: 6170 2853 6567 6d65 6e74 4d61 7463 682c  ap(SegmentMatch,
-000183d0: 206d 6174 6368 6573 2e73 6567 6d65 6e74   matches.segment
-000183e0: 7329 290d 0a20 2020 2020 2020 2020 2020  s))..           
-000183f0: 2073 656c 662e 5f73 6567 6d65 6e74 5f69   self._segment_i
-00018400: 6e64 6963 6573 203d 205b 5b69 5d20 666f  ndices = [[i] fo
-00018410: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-00018420: 286d 6174 6368 6573 2e73 6567 6d65 6e74  (matches.segment
-00018430: 7329 295d 0d0a 2020 2020 2020 2020 656c  s))]..        el
-00018440: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00018450: 2073 656c 662e 6d61 7463 6865 7320 3d20   self.matches = 
-00018460: 6d61 7463 6865 730d 0a20 2020 2020 2020  matches..       
-00018470: 2020 2020 2061 7373 6572 7420 5f73 6567       assert _seg
-00018480: 6d65 6e74 5f69 6e64 6963 6573 2069 7320  ment_indices is 
-00018490: 6e6f 7420 4e6f 6e65 0d0a 2020 2020 2020  not None..      
-000184a0: 2020 2020 2020 6173 7365 7274 206c 656e        assert len
-000184b0: 2873 656c 662e 6d61 7463 6865 7329 203d  (self.matches) =
-000184c0: 3d20 6c65 6e28 5f73 6567 6d65 6e74 5f69  = len(_segment_i
-000184d0: 6e64 6963 6573 290d 0a20 2020 2020 2020  ndices)..       
-000184e0: 2020 2020 2061 7373 6572 7420 616c 6c28       assert all(
-000184f0: 6c65 6e28 6d61 7463 682e 7365 676d 656e  len(match.segmen
-00018500: 7473 2920 3d3d 206c 656e 285f 7365 676d  ts) == len(_segm
-00018510: 656e 745f 696e 6469 6365 735b 695d 2920  ent_indices[i]) 
-00018520: 666f 7220 692c 206d 6174 6368 2069 6e20  for i, match in 
-00018530: 656e 756d 6572 6174 6528 7365 6c66 2e6d  enumerate(self.m
-00018540: 6174 6368 6573 2929 0d0a 2020 2020 2020  atches))..      
-00018550: 2020 2020 2020 7365 6c66 2e5f 7365 676d        self._segm
-00018560: 656e 745f 696e 6469 6365 7320 3d20 5f73  ent_indices = _s
-00018570: 6567 6d65 6e74 5f69 6e64 6963 6573 0d0a  egment_indices..
-00018580: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-00018590: 0a20 2020 2064 6566 2073 6567 6d65 6e74  .    def segment
-000185a0: 5f69 6e64 6963 6573 2873 656c 6629 3a0d  _indices(self):.
-000185b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000185c0: 7365 6c66 2e5f 7365 676d 656e 745f 696e  self._segment_in
-000185d0: 6469 6365 730d 0a0d 0a20 2020 2064 6566  dices....    def
-000185e0: 205f 6375 7272 5f73 6567 5f67 726f 7570   _curr_seg_group
-000185f0: 7328 7365 6c66 2920 2d3e 204c 6973 745b  s(self) -> List[
-00018600: 4c69 7374 5b54 7570 6c65 5b69 6e74 2c20  List[Tuple[int, 
-00018610: 5365 676d 656e 745d 5d5d 3a0d 0a20 2020  Segment]]]:..   
-00018620: 2020 2020 2073 6567 5f67 726f 7570 732c       seg_groups,
-00018630: 2063 7572 725f 7365 6773 203d 205b 5d2c   curr_segs = [],
-00018640: 205b 5d0d 0a20 2020 2020 2020 2063 7572   []..        cur
-00018650: 725f 6d61 7820 3d20 2d31 0d0a 2020 2020  r_max = -1..    
-00018660: 2020 2020 666f 7220 7365 675f 696e 6469      for seg_indi
-00018670: 6365 732c 206d 6174 6368 2069 6e20 7a69  ces, match in zi
-00018680: 7028 7365 6c66 2e5f 7365 676d 656e 745f  p(self._segment_
-00018690: 696e 6469 6365 732c 2073 656c 662e 6d61  indices, self.ma
-000186a0: 7463 6865 7329 3a0d 0a20 2020 2020 2020  tches):..       
-000186b0: 2020 2020 2066 6f72 2069 2c20 7365 6720       for i, seg 
-000186c0: 696e 207a 6970 2873 6f72 7465 6428 7365  in zip(sorted(se
-000186d0: 675f 696e 6469 6365 7329 2c20 6d61 7463  g_indices), matc
-000186e0: 682e 7365 676d 656e 7473 293a 0d0a 2020  h.segments):..  
-000186f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00018700: 2069 203e 2063 7572 725f 6d61 783a 0d0a   i > curr_max:..
-00018710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018720: 2020 2020 6375 7272 5f73 6567 732e 6170      curr_segs.ap
-00018730: 7065 6e64 2828 692c 2073 6567 2929 0d0a  pend((i, seg))..
-00018740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018750: 2020 2020 6966 2069 202d 2031 2021 3d20      if i - 1 != 
-00018760: 6375 7272 5f6d 6178 3a0d 0a20 2020 2020  curr_max:..     
-00018770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018780: 2020 2073 6567 5f67 726f 7570 732e 6170     seg_groups.ap
-00018790: 7065 6e64 2863 7572 725f 7365 6773 290d  pend(curr_segs).
-000187a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000187b0: 2020 2020 2020 2020 2063 7572 725f 7365           curr_se
-000187c0: 6773 203d 205b 5d0d 0a20 2020 2020 2020  gs = []..       
-000187d0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000187e0: 725f 6d61 7820 3d20 690d 0a0d 0a20 2020  r_max = i....   
-000187f0: 2020 2020 2069 6620 6375 7272 5f73 6567       if curr_seg
-00018800: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00018810: 7365 675f 6772 6f75 7073 2e61 7070 656e  seg_groups.appen
-00018820: 6428 6375 7272 5f73 6567 7329 0d0a 2020  d(curr_segs)..  
-00018830: 2020 2020 2020 7265 7475 726e 2073 6567        return seg
-00018840: 5f67 726f 7570 730d 0a0d 0a20 2020 2064  _groups....    d
-00018850: 6566 2066 696e 6428 7365 6c66 2c20 7061  ef find(self, pa
-00018860: 7474 6572 6e3a 2073 7472 2c20 776f 7264  ttern: str, word
-00018870: 5f6c 6576 656c 3d54 7275 652c 2066 6c61  _level=True, fla
-00018880: 6773 3d4e 6f6e 6529 202d 3e20 2257 6869  gs=None) -> "Whi
-00018890: 7370 6572 5265 7375 6c74 4d61 7463 6865  sperResultMatche
-000188a0: 7322 3a0d 0a20 2020 2020 2020 2022 2222  s":..        """
-000188b0: 0d0a 2020 2020 2020 2020 4669 6e64 2073  ..        Find s
-000188c0: 6567 6d65 6e74 732f 776f 7264 7320 616e  egments/words an
-000188d0: 6420 7469 6d65 7374 616d 7073 2077 6974  d timestamps wit
-000188e0: 6820 7265 6775 6c61 7220 6578 7072 6573  h regular expres
-000188f0: 7369 6f6e 2e0d 0a0d 0a20 2020 2020 2020  sion.....       
-00018900: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
-00018910: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
-00018920: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-00018930: 203a 2073 7472 0d0a 2020 2020 2020 2020   : str..        
-00018940: 2020 2020 5265 6745 7820 7061 7474 6572      RegEx patter
-00018950: 6e20 746f 2073 6561 7263 6820 666f 722e  n to search for.
-00018960: 0d0a 2020 2020 2020 2020 776f 7264 5f6c  ..        word_l
-00018970: 6576 656c 203a 2062 6f6f 6c2c 2064 6566  evel : bool, def
-00018980: 6175 6c74 2054 7275 650d 0a20 2020 2020  ault True..     
-00018990: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
-000189a0: 6f20 7365 6172 6368 2061 7420 776f 7264  o search at word
-000189b0: 2d6c 6576 656c 2e0d 0a20 2020 2020 2020  -level...       
-000189c0: 2066 6c61 6773 203a 206f 7074 696f 6e61   flags : optiona
-000189d0: 6c0d 0a20 2020 2020 2020 2020 2020 2052  l..            R
-000189e0: 6567 4578 2066 6c61 6773 2e0d 0a0d 0a20  egEx flags..... 
-000189f0: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
-00018a00: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
-00018a10: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
-00018a20: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
-00018a30: 6869 7370 6572 5265 7375 6c74 4d61 7463  hisperResultMatc
-00018a40: 6865 730d 0a20 2020 2020 2020 2020 2020  hes..           
-00018a50: 2041 6e20 696e 7374 616e 6365 206f 6620   An instance of 
-00018a60: 3a63 6c61 7373 3a60 7374 6162 6c65 5f77  :class:`stable_w
-00018a70: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
-00018a80: 6973 7065 7252 6573 756c 744d 6174 6368  isperResultMatch
-00018a90: 6573 6020 7769 7468 2077 6f72 642f 7365  es` with word/se
-00018aa0: 676d 656e 7420 7468 6174 206d 6174 6368  gment that match
-00018ab0: 2060 6070 6174 7465 726e 6060 2e0d 0a20   ``pattern``... 
-00018ac0: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
-00018ad0: 2020 2020 2020 7365 675f 6772 6f75 7073        seg_groups
-00018ae0: 203d 2073 656c 662e 5f63 7572 725f 7365   = self._curr_se
-00018af0: 675f 6772 6f75 7073 2829 0d0a 2020 2020  g_groups()..    
-00018b00: 2020 2020 6d61 7463 6865 733a 204c 6973      matches: Lis
-00018b10: 745b 5365 676d 656e 744d 6174 6368 5d20  t[SegmentMatch] 
-00018b20: 3d20 5b5d 0d0a 2020 2020 2020 2020 6d61  = []..        ma
-00018b30: 7463 685f 7365 675f 696e 6469 6365 733a  tch_seg_indices:
-00018b40: 204c 6973 745b 4c69 7374 5b69 6e74 5d5d   List[List[int]]
-00018b50: 203d 205b 5d0d 0a20 2020 2020 2020 2069   = []..        i
-00018b60: 6620 776f 7264 5f6c 6576 656c 3a0d 0a20  f word_level:.. 
-00018b70: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00018b80: 7420 616c 6c28 616c 6c28 7365 672e 6861  t all(all(seg.ha
-00018b90: 735f 776f 7264 7320 666f 7220 7365 6720  s_words for seg 
-00018ba0: 696e 206d 6174 6368 2e73 6567 6d65 6e74  in match.segment
-00018bb0: 7329 2066 6f72 206d 6174 6368 2069 6e20  s) for match in 
-00018bc0: 7365 6c66 2e6d 6174 6368 6573 293a 0d0a  self.matches):..
-00018bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018be0: 7761 726e 696e 6773 2e77 6172 6e28 2743  warnings.warn('C
-00018bf0: 616e 6e6f 7420 7065 7266 6f72 6d20 776f  annot perform wo
-00018c00: 7264 2d6c 6576 656c 2073 6561 7263 6820  rd-level search 
-00018c10: 7769 7468 2073 6567 6d65 6e74 2873 2920  with segment(s) 
-00018c20: 6d69 7373 696e 6720 776f 7264 2074 696d  missing word tim
-00018c30: 6573 7461 6d70 732e 2729 0d0a 2020 2020  estamps.')..    
-00018c40: 2020 2020 2020 2020 2020 2020 776f 7264              word
-00018c50: 5f6c 6576 656c 203d 2046 616c 7365 0d0a  _level = False..
-00018c60: 0d0a 2020 2020 2020 2020 666f 7220 7365  ..        for se
-00018c70: 6773 2069 6e20 7365 675f 6772 6f75 7073  gs in seg_groups
-00018c80: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00018c90: 6620 776f 7264 5f6c 6576 656c 3a0d 0a20  f word_level:.. 
-00018ca0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00018cb0: 6478 7320 3d20 6c69 7374 2863 6861 696e  dxs = list(chain
-00018cc0: 2e66 726f 6d5f 6974 6572 6162 6c65 280d  .from_iterable(.
-00018cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ce0: 2020 2020 205b 2869 2c20 6a29 5d2a 6c65       [(i, j)]*le
-00018cf0: 6e28 776f 7264 2e77 6f72 6429 2066 6f72  n(word.word) for
-00018d00: 2028 692c 2073 6567 2920 696e 2073 6567   (i, seg) in seg
-00018d10: 7320 666f 7220 6a2c 2077 6f72 6420 696e  s for j, word in
-00018d20: 2065 6e75 6d65 7261 7465 2873 6567 2e77   enumerate(seg.w
-00018d30: 6f72 6473 290d 0a20 2020 2020 2020 2020  ords)..         
-00018d40: 2020 2020 2020 2029 290d 0a20 2020 2020         ))..     
-00018d50: 2020 2020 2020 2020 2020 2074 6578 7420             text 
-00018d60: 3d20 2727 2e6a 6f69 6e28 776f 7264 2e77  = ''.join(word.w
-00018d70: 6f72 6420 666f 7220 285f 2c20 7365 6729  ord for (_, seg)
-00018d80: 2069 6e20 7365 6773 2066 6f72 2077 6f72   in segs for wor
-00018d90: 6420 696e 2073 6567 2e77 6f72 6473 290d  d in seg.words).
-00018da0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00018db0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00018dc0: 2020 2020 6964 7873 203d 206c 6973 7428      idxs = list(
-00018dd0: 6368 6169 6e2e 6672 6f6d 5f69 7465 7261  chain.from_itera
-00018de0: 626c 6528 5b28 692c 204e 6f6e 6529 5d2a  ble([(i, None)]*
-00018df0: 6c65 6e28 7365 672e 7465 7874 2920 666f  len(seg.text) fo
-00018e00: 7220 2869 2c20 7365 6729 2069 6e20 7365  r (i, seg) in se
-00018e10: 6773 2929 0d0a 2020 2020 2020 2020 2020  gs))..          
-00018e20: 2020 2020 2020 7465 7874 203d 2027 272e        text = ''.
-00018e30: 6a6f 696e 2873 6567 2e74 6578 7420 666f  join(seg.text fo
-00018e40: 7220 285f 2c20 7365 6729 2069 6e20 7365  r (_, seg) in se
-00018e50: 6773 290d 0a20 2020 2020 2020 2020 2020  gs)..           
-00018e60: 2061 7373 6572 7420 6c65 6e28 6964 7873   assert len(idxs
-00018e70: 2920 3d3d 206c 656e 2874 6578 7429 0d0a  ) == len(text)..
-00018e80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00018e90: 6375 7272 5f6d 6174 6368 2069 6e20 7265  curr_match in re
-00018ea0: 2e66 696e 6469 7465 7228 7061 7474 6572  .finditer(patter
-00018eb0: 6e2c 2074 6578 742c 2066 6c61 6773 3d66  n, text, flags=f
-00018ec0: 6c61 6773 206f 7220 3029 3a0d 0a20 2020  lags or 0):..   
-00018ed0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-00018ee0: 7274 2c20 656e 6420 3d20 6375 7272 5f6d  rt, end = curr_m
-00018ef0: 6174 6368 2e73 7061 6e28 290d 0a20 2020  atch.span()..   
-00018f00: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00018f10: 725f 6964 7873 203d 2069 6478 735b 7374  r_idxs = idxs[st
-00018f20: 6172 743a 2065 6e64 5d0d 0a20 2020 2020  art: end]..     
-00018f30: 2020 2020 2020 2020 2020 2063 7572 725f             curr_
-00018f40: 7365 675f 6964 7873 203d 2073 6f72 7465  seg_idxs = sorte
-00018f50: 6428 7365 7428 695b 305d 2066 6f72 2069  d(set(i[0] for i
-00018f60: 2069 6e20 6375 7272 5f69 6478 7329 290d   in curr_idxs)).
-00018f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018f80: 2069 6620 776f 7264 5f6c 6576 656c 3a0d   if word_level:.
-00018f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018fa0: 2020 2020 2063 7572 725f 776f 7264 5f69       curr_word_i
-00018fb0: 6478 7320 3d20 5b0d 0a20 2020 2020 2020  dxs = [..       
-00018fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fd0: 2073 6f72 7465 6428 7365 7428 6a20 666f   sorted(set(j fo
-00018fe0: 7220 692c 206a 2069 6e20 6375 7272 5f69  r i, j in curr_i
-00018ff0: 6478 7320 6966 2069 203d 3d20 7365 675f  dxs if i == seg_
-00019000: 6964 7829 290d 0a20 2020 2020 2020 2020  idx))..         
-00019010: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00019020: 6f72 2073 6567 5f69 6478 2069 6e20 6375  or seg_idx in cu
-00019030: 7272 5f73 6567 5f69 6478 730d 0a20 2020  rr_seg_idxs..   
-00019040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019050: 205d 0d0a 2020 2020 2020 2020 2020 2020   ]..            
-00019060: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00019070: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00019080: 7572 725f 776f 7264 5f69 6478 7320 3d20  urr_word_idxs = 
-00019090: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
-000190a0: 2020 2020 2020 6d61 7463 6865 732e 6170        matches.ap
-000190b0: 7065 6e64 2853 6567 6d65 6e74 4d61 7463  pend(SegmentMatc
-000190c0: 6828 0d0a 2020 2020 2020 2020 2020 2020  h(..            
-000190d0: 2020 2020 2020 2020 7365 676d 656e 7473          segments
-000190e0: 3d5b 7320 666f 7220 692c 2073 2069 6e20  =[s for i, s in 
-000190f0: 7365 6773 2069 6620 6920 696e 2063 7572  segs if i in cur
-00019100: 725f 7365 675f 6964 7873 5d2c 0d0a 2020  r_seg_idxs],..  
-00019110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019120: 2020 5f77 6f72 645f 696e 6469 6365 733d    _word_indices=
-00019130: 6375 7272 5f77 6f72 645f 6964 7873 2c0d  curr_word_idxs,.
-00019140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019150: 2020 2020 205f 7465 7874 5f6d 6174 6368       _text_match
-00019160: 3d63 7572 725f 6d61 7463 682e 6772 6f75  =curr_match.grou
-00019170: 7028 290d 0a20 2020 2020 2020 2020 2020  p()..           
-00019180: 2020 2020 2029 290d 0a20 2020 2020 2020       ))..       
-00019190: 2020 2020 2020 2020 206d 6174 6368 5f73           match_s
-000191a0: 6567 5f69 6e64 6963 6573 2e61 7070 656e  eg_indices.appen
-000191b0: 6428 6375 7272 5f73 6567 5f69 6478 7329  d(curr_seg_idxs)
-000191c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000191d0: 2057 6869 7370 6572 5265 7375 6c74 4d61   WhisperResultMa
-000191e0: 7463 6865 7328 6d61 7463 6865 732c 206d  tches(matches, m
-000191f0: 6174 6368 5f73 6567 5f69 6e64 6963 6573  atch_seg_indices
-00019200: 290d 0a0d 0a20 2020 2064 6566 205f 5f6c  )....    def __l
-00019210: 656e 5f5f 2873 656c 6629 3a0d 0a20 2020  en__(self):..   
-00019220: 2020 2020 2072 6574 7572 6e20 6c65 6e28       return len(
-00019230: 7365 6c66 2e6d 6174 6368 6573 290d 0a0d  self.matches)...
-00019240: 0a20 2020 2064 6566 205f 5f62 6f6f 6c5f  .    def __bool_
-00019250: 5f28 7365 6c66 293a 0d0a 2020 2020 2020  _(self):..      
-00019260: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
-00019270: 6c65 6e5f 5f28 2920 213d 2030 0d0a 0d0a  len__() != 0....
-00019280: 2020 2020 6465 6620 5f5f 6765 7469 7465      def __getite
-00019290: 6d5f 5f28 7365 6c66 2c20 6964 7829 3a0d  m__(self, idx):.
-000192a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000192b0: 7365 6c66 2e6d 6174 6368 6573 5b69 6478  self.matches[idx
-000192c0: 5d0d 0a                                  ]..
+00013ee0: 2066 2752 656d 6f76 653a 205b 7b66 6f72   f'Remove: [{for
+00013ef0: 6d61 745f 7469 6d65 7374 616d 7028 616c  mat_timestamp(al
+00013f00: 6c5f 776f 7264 735b 735d 2e73 7461 7274  l_words[s].start
+00013f10: 297d 202d 3e20 7b66 6f72 6d61 745f 7469  )} -> {format_ti
+00013f20: 6d65 7374 616d 7028 616c 6c5f 776f 7264  mestamp(all_word
+00013f30: 735b 692d 315d 2e65 6e64 297d 5d20 270d  s[i-1].end)}] '.
+00013f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013f50: 2020 2020 2020 2020 202b 2027 272e 6a6f           + ''.jo
+00013f60: 696e 285f 772e 776f 7264 2066 6f72 205f  in(_w.word for _
+00013f70: 7720 696e 2061 6c6c 5f77 6f72 6473 5b73  w in all_words[s
+00013f80: 3a69 5d29 202b 2027 5c6e 270d 0a20 2020  :i]) + '\n'..   
+00013f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fa0: 2020 2020 202b 2027 5c6e 272e 6a6f 696e       + '\n'.join
+00013fb0: 2872 6576 6572 7365 6428 7465 6d70 5f63  (reversed(temp_c
+00013fc0: 6861 6e67 6573 2929 202b 2027 5c6e 270d  hanges)) + '\n'.
+00013fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013fe0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00013ff0: 2020 2020 2020 2020 666f 7220 6930 2c20          for i0, 
+00014000: 6931 2069 6e20 7a69 7028 7261 6e67 6528  i1 in zip(range(
+00014010: 7320 2d20 636f 756e 742c 2073 292c 2072  s - count, s), r
+00014020: 616e 6765 2873 2c20 6929 293a 0d0a 2020  ange(s, i)):..  
+00014030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014040: 2020 6966 206c 656e 2861 6c6c 5f77 6f72    if len(all_wor
+00014050: 6473 5b69 305d 2e77 6f72 6429 203c 206c  ds[i0].word) < l
+00014060: 656e 2861 6c6c 5f77 6f72 6473 5b69 315d  en(all_words[i1]
+00014070: 2e77 6f72 6429 3a0d 0a20 2020 2020 2020  .word):..       
+00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014090: 2061 6c6c 5f77 6f72 6473 5b69 315d 2e73   all_words[i1].s
+000140a0: 7461 7274 203d 2061 6c6c 5f77 6f72 6473  tart = all_words
+000140b0: 5b69 305d 2e73 7461 7274 0d0a 2020 2020  [i0].start..    
+000140c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140d0: 2020 2020 616c 6c5f 776f 7264 735b 6931      all_words[i1
+000140e0: 5d2e 656e 6420 3d20 616c 6c5f 776f 7264  ].end = all_word
+000140f0: 735b 6930 5d2e 656e 640d 0a20 2020 2020  s[i0].end..     
+00014100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014110: 2020 205f 7369 642c 205f 7769 6420 3d20     _sid, _wid = 
+00014120: 616c 6c5f 776f 7264 735b 6930 5d2e 7365  all_words[i0].se
+00014130: 676d 656e 745f 6964 2c20 616c 6c5f 776f  gment_id, all_wo
+00014140: 7264 735b 6930 5d2e 6964 0d0a 2020 2020  rds[i0].id..    
+00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014160: 2020 2020 7365 6c66 2e73 6567 6d65 6e74      self.segment
+00014170: 735b 5f73 6964 5d2e 776f 7264 735b 5f77  s[_sid].words[_w
+00014180: 6964 5d20 3d20 616c 6c5f 776f 7264 735b  id] = all_words[
+00014190: 6931 5d0d 0a0d 0a20 2020 2020 2020 2020  i1]....         
+000141a0: 2020 2069 6620 6368 616e 6765 733a 0d0a     if changes:..
+000141b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141c0: 7072 696e 7428 275c 6e27 2e6a 6f69 6e28  print('\n'.join(
+000141d0: 7265 7665 7273 6564 2863 6861 6e67 6573  reversed(changes
+000141e0: 2929 290d 0a0d 0a20 2020 2020 2020 2020  )))....         
+000141f0: 2020 2073 656c 662e 7265 6d6f 7665 5f6e     self.remove_n
+00014200: 6f5f 776f 7264 5f73 6567 6d65 6e74 7328  o_word_segments(
+00014210: 7265 6173 7369 676e 5f69 6473 3d46 616c  reassign_ids=Fal
+00014220: 7365 290d 0a20 2020 2020 2020 2073 656c  se)..        sel
+00014230: 662e 7265 6173 7369 676e 5f69 6473 2829  f.reassign_ids()
+00014240: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+00014250: 726e 2073 656c 660d 0a0d 0a20 2020 2064  rn self....    d
+00014260: 6566 2072 656d 6f76 655f 776f 7264 735f  ef remove_words_
+00014270: 6279 5f73 7472 280d 0a20 2020 2020 2020  by_str(..       
+00014280: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
+00014290: 2020 2020 2020 2020 776f 7264 733a 2055          words: U
+000142a0: 6e69 6f6e 5b73 7472 2c20 4c69 7374 5b73  nion[str, List[s
+000142b0: 7472 5d2c 204e 6f6e 655d 2c0d 0a20 2020  tr], None],..   
+000142c0: 2020 2020 2020 2020 2063 6173 655f 7365           case_se
+000142d0: 6e73 6974 6976 653a 2062 6f6f 6c20 3d20  nsitive: bool = 
+000142e0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+000142f0: 2020 2020 7374 7269 703a 2062 6f6f 6c20      strip: bool 
+00014300: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
+00014310: 2020 2020 2069 676e 6f72 655f 7075 6e63       ignore_punc
+00014320: 7475 6174 696f 6e73 3a20 7374 7220 3d20  tuations: str = 
+00014330: 225c 2227 2c2e 3f21 222c 0d0a 2020 2020  "\"',.?!",..    
+00014340: 2020 2020 2020 2020 6d69 6e5f 7072 6f62          min_prob
+00014350: 3a20 666c 6f61 7420 3d20 4e6f 6e65 2c0d  : float = None,.
+00014360: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+00014370: 7465 7273 3a20 4361 6c6c 6162 6c65 203d  ters: Callable =
+00014380: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+00014390: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
+000143a0: 6c20 3d20 5472 7565 0d0a 2020 2020 2920  l = True..    ) 
+000143b0: 2d3e 2027 5768 6973 7065 7252 6573 756c  -> 'WhisperResul
+000143c0: 7427 3a0d 0a20 2020 2020 2020 2022 2222  t':..        """
+000143d0: 0d0a 2020 2020 2020 2020 5265 6d6f 7665  ..        Remove
+000143e0: 2077 6f72 6473 2074 6861 7420 6d61 7463   words that matc
+000143f0: 6820 6060 776f 7264 7360 602e 0d0a 0d0a  h ``words``.....
+00014400: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00014410: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
+00014420: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00014430: 776f 7264 7320 3a20 7374 7220 6f72 206c  words : str or l
+00014440: 6973 7420 6f66 2073 7472 206f 7220 4e6f  ist of str or No
+00014450: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
+00014460: 4120 776f 7264 206f 7220 6c69 7374 206f  A word or list o
+00014470: 6620 776f 7264 7320 746f 2072 656d 6f76  f words to remov
+00014480: 652e 6060 4e6f 6e65 6060 2066 6f72 2061  e.``None`` for a
+00014490: 6c6c 2077 6f72 6473 2074 6f20 6265 2070  ll words to be p
+000144a0: 6173 7365 6420 696e 746f 2060 6066 696c  assed into ``fil
+000144b0: 7465 7273 6060 2e0d 0a20 2020 2020 2020  ters``...       
+000144c0: 2063 6173 655f 7365 6e73 6974 6976 6520   case_sensitive 
+000144d0: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
+000144e0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
+000144f0: 2020 2057 6865 7468 6572 2074 6865 2063     Whether the c
+00014500: 6173 6520 6f66 2077 6f72 6473 206e 6565  ase of words nee
+00014510: 6420 746f 206d 6174 6368 2074 6f20 6265  d to match to be
+00014520: 2063 6f6e 7369 6465 7265 6420 6173 2072   considered as r
+00014530: 6570 6574 6974 696f 6e2e 0d0a 2020 2020  epetition...    
+00014540: 2020 2020 7374 7269 7020 3a20 626f 6f6c      strip : bool
+00014550: 2c20 6465 6661 756c 7420 5472 7565 0d0a  , default True..
+00014560: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+00014570: 6865 7220 746f 2069 676e 6f72 6520 7370  her to ignore sp
+00014580: 6163 6573 2062 6566 6f72 6520 616e 6420  aces before and 
+00014590: 6166 7465 7220 6561 6368 2077 6f72 642e  after each word.
+000145a0: 0d0a 2020 2020 2020 2020 6967 6e6f 7265  ..        ignore
+000145b0: 5f70 756e 6374 7561 7469 6f6e 7320 3a20  _punctuations : 
+000145c0: 626f 6f6c 2c20 6465 6661 756c 7420 2722  bool, default '"
+000145d0: 272c 2e3f 2127 0d0a 2020 2020 2020 2020  ',.?!'..        
+000145e0: 2020 2020 456e 6469 6e67 2070 756e 6374      Ending punct
+000145f0: 7561 7469 6f6e 7320 746f 2069 676e 6f72  uations to ignor
+00014600: 652e 0d0a 2020 2020 2020 2020 6d69 6e5f  e...        min_
+00014610: 7072 6f62 203a 2066 6c6f 6174 2c20 6f70  prob : float, op
+00014620: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00014630: 2020 2020 4163 7473 2061 7320 7468 6520      Acts as the 
+00014640: 6669 7273 7420 6669 6c74 6572 2074 6865  first filter the
+00014650: 2066 6f72 2074 6865 2077 6f72 6473 2074   for the words t
+00014660: 6861 7420 6d61 7463 6820 6060 776f 7264  hat match ``word
+00014670: 7360 602e 2057 6f72 6473 2077 6974 6820  s``. Words with 
+00014680: 7072 6f62 6162 696c 6974 7920 3c20 6060  probability < ``
+00014690: 6d69 6e5f 7072 6f62 6060 2077 696c 6c0d  min_prob`` will.
+000146a0: 0a20 2020 2020 2020 2020 2020 2062 6520  .            be 
+000146b0: 7265 6d6f 7665 6420 6966 2060 6066 696c  removed if ``fil
+000146c0: 7465 7273 6060 2069 7320 6060 4e6f 6e65  ters`` is ``None
+000146d0: 6060 2c20 656c 7365 2070 6173 7320 7468  ``, else pass th
+000146e0: 6520 776f 7264 7320 696e 746f 2060 6066  e words into ``f
+000146f0: 696c 7465 7273 6060 2e20 576f 7264 7320  ilters``. Words 
+00014700: 7769 7468 6f75 7420 7072 6f62 6162 696c  without probabil
+00014710: 6974 7920 7769 6c6c 0d0a 2020 2020 2020  ity will..      
+00014720: 2020 2020 2020 6265 2074 7265 6174 6564        be treated
+00014730: 2061 7320 6861 7669 6e67 2070 726f 6261   as having proba
+00014740: 6269 6c69 7479 203c 2060 606d 696e 5f70  bility < ``min_p
+00014750: 726f 6260 602e 0d0a 2020 2020 2020 2020  rob``...        
+00014760: 6669 6c74 6572 7320 3a20 4361 6c6c 6162  filters : Callab
+00014770: 6c65 2c20 6f70 7469 6f6e 616c 0d0a 2020  le, optional..  
+00014780: 2020 2020 2020 2020 2020 4120 6675 6e63            A func
+00014790: 7469 6f6e 2074 6861 7420 7461 6b65 7320  tion that takes 
+000147a0: 616e 2069 6e73 7461 6e63 6520 6f66 203a  an instance of :
+000147b0: 636c 6173 733a 6073 7461 626c 655f 7768  class:`stable_wh
+000147c0: 6973 7065 722e 7265 7375 6c74 2e57 6f72  isper.result.Wor
+000147d0: 6454 696d 696e 6760 2061 7320 6974 7320  dTiming` as its 
+000147e0: 6f6e 6c79 2061 7267 756d 656e 742e 0d0a  only argument...
+000147f0: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00014800: 2066 756e 6374 696f 6e20 6973 2063 7573   function is cus
+00014810: 746f 6d20 6669 6c74 6572 2066 6f72 2074  tom filter for t
+00014820: 6865 2077 6f72 6473 2074 6861 7420 6d61  he words that ma
+00014830: 7463 6820 6060 776f 7264 7360 6020 616e  tch ``words`` an
+00014840: 6420 7765 7265 206e 6f74 2063 6175 6768  d were not caugh
+00014850: 7420 6279 2060 606d 696e 5f70 726f 6260  t by ``min_prob`
+00014860: 602e 0d0a 2020 2020 2020 2020 7665 7262  `...        verb
+00014870: 6f73 653a 0d0a 2020 2020 2020 2020 2020  ose:..          
+00014880: 2020 5768 6574 6865 7220 746f 2070 7269    Whether to pri
+00014890: 6e74 2064 6574 6169 6c20 6f66 2074 6865  nt detail of the
+000148a0: 2072 656d 6f76 6564 2077 6f72 6473 2e0d   removed words..
+000148b0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+000148c0: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
+000148d0: 2d2d 2d0d 0a20 2020 2020 2020 2073 7461  ---..        sta
+000148e0: 626c 655f 7768 6973 7065 722e 7265 7375  ble_whisper.resu
+000148f0: 6c74 2e57 6869 7370 6572 5265 7375 6c74  lt.WhisperResult
+00014900: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00014910: 6520 6375 7272 656e 7420 696e 7374 616e  e current instan
+00014920: 6365 2061 6674 6572 2074 6865 2063 6861  ce after the cha
+00014930: 6e67 6573 2e0d 0a20 2020 2020 2020 2022  nges...        "
+00014940: 2222 0d0a 2020 2020 2020 2020 6966 206e  ""..        if n
+00014950: 6f74 2073 656c 662e 6861 735f 776f 7264  ot self.has_word
+00014960: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00014970: 7265 7475 726e 2073 656c 660d 0a20 2020  return self..   
+00014980: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00014990: 6365 2877 6f72 6473 2c20 7374 7229 3a0d  ce(words, str):.
+000149a0: 0a20 2020 2020 2020 2020 2020 2077 6f72  .            wor
+000149b0: 6473 203d 205b 776f 7264 735d 0d0a 2020  ds = [words]..  
+000149c0: 2020 2020 2020 616c 6c5f 776f 7264 7320        all_words 
+000149d0: 3d20 7365 6c66 2e61 6c6c 5f77 6f72 6473  = self.all_words
+000149e0: 2829 0d0a 2020 2020 2020 2020 616c 6c5f  ()..        all_
+000149f0: 776f 7264 735f 7374 7220 3d20 5b77 2e77  words_str = [w.w
+00014a00: 6f72 6420 666f 7220 7720 696e 2061 6c6c  ord for w in all
+00014a10: 5f77 6f72 6473 5d0d 0a20 2020 2020 2020  _words]..       
+00014a20: 2069 6620 7374 7269 703a 0d0a 2020 2020   if strip:..    
+00014a30: 2020 2020 2020 2020 616c 6c5f 776f 7264          all_word
+00014a40: 735f 7374 7220 3d20 5b77 2e73 7472 6970  s_str = [w.strip
+00014a50: 2829 2066 6f72 2077 2069 6e20 616c 6c5f  () for w in all_
+00014a60: 776f 7264 735f 7374 725d 0d0a 2020 2020  words_str]..    
+00014a70: 2020 2020 2020 2020 776f 7264 7320 3d20          words = 
+00014a80: 5b77 2e73 7472 6970 2829 2066 6f72 2077  [w.strip() for w
+00014a90: 2069 6e20 776f 7264 735d 0d0a 2020 2020   in words]..    
+00014aa0: 2020 2020 6966 2069 676e 6f72 655f 7075      if ignore_pu
+00014ab0: 6e63 7475 6174 696f 6e73 3a0d 0a20 2020  nctuations:..   
+00014ac0: 2020 2020 2020 2020 2070 746e 203d 2066           ptn = f
+00014ad0: 275b 7b69 676e 6f72 655f 7075 6e63 7475  '[{ignore_punctu
+00014ae0: 6174 696f 6e73 7d5d 2b24 270d 0a20 2020  ations}]+$'..   
+00014af0: 2020 2020 2020 2020 2061 6c6c 5f77 6f72           all_wor
+00014b00: 6473 5f73 7472 203d 205b 7265 2e73 7562  ds_str = [re.sub
+00014b10: 2870 746e 2c20 2727 2c20 7729 2066 6f72  (ptn, '', w) for
+00014b20: 2077 2069 6e20 616c 6c5f 776f 7264 735f   w in all_words_
+00014b30: 7374 725d 0d0a 2020 2020 2020 2020 2020  str]..          
+00014b40: 2020 776f 7264 7320 3d20 5b72 652e 7375    words = [re.su
+00014b50: 6228 7074 6e2c 2027 272c 2077 2920 666f  b(ptn, '', w) fo
+00014b60: 7220 7720 696e 2077 6f72 6473 5d0d 0a20  r w in words].. 
+00014b70: 2020 2020 2020 2069 6620 6e6f 7420 6361         if not ca
+00014b80: 7365 5f73 656e 7369 7469 7665 3a0d 0a20  se_sensitive:.. 
+00014b90: 2020 2020 2020 2020 2020 2061 6c6c 5f77             all_w
+00014ba0: 6f72 6473 5f73 7472 203d 205b 772e 6c6f  ords_str = [w.lo
+00014bb0: 7765 7228 2920 666f 7220 7720 696e 2061  wer() for w in a
+00014bc0: 6c6c 5f77 6f72 6473 5f73 7472 5d0d 0a20  ll_words_str].. 
+00014bd0: 2020 2020 2020 2020 2020 2077 6f72 6473             words
+00014be0: 203d 205b 772e 6c6f 7765 7228 2920 666f   = [w.lower() fo
+00014bf0: 7220 7720 696e 2077 6f72 6473 5d0d 0a0d  r w in words]...
+00014c00: 0a20 2020 2020 2020 2063 6861 6e67 6573  .        changes
+00014c10: 203d 205b 5d0d 0a20 2020 2020 2020 2066   = []..        f
+00014c20: 6f72 2069 2c20 7720 696e 2072 6576 6572  or i, w in rever
+00014c30: 7365 6428 6c69 7374 2865 6e75 6d65 7261  sed(list(enumera
+00014c40: 7465 2861 6c6c 5f77 6f72 6473 5f73 7472  te(all_words_str
+00014c50: 2929 293a 0d0a 2020 2020 2020 2020 2020  ))):..          
+00014c60: 2020 6966 206e 6f74 2028 776f 7264 7320    if not (words 
+00014c70: 6973 204e 6f6e 6520 6f72 2061 6e79 2877  is None or any(w
+00014c80: 203d 3d20 5f77 2066 6f72 205f 7720 696e   == _w for _w in
+00014c90: 2077 6f72 6473 2929 3a0d 0a20 2020 2020   words)):..     
+00014ca0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00014cb0: 6e75 650d 0a20 2020 2020 2020 2020 2020  nue..           
+00014cc0: 2069 6620 280d 0a20 2020 2020 2020 2020   if (..         
+00014cd0: 2020 2020 2020 2020 2020 2028 6d69 6e5f             (min_
+00014ce0: 7072 6f62 2069 7320 4e6f 6e65 206f 7220  prob is None or 
+00014cf0: 616c 6c5f 776f 7264 735b 695d 2e70 726f  all_words[i].pro
+00014d00: 6261 6269 6c69 7479 2069 7320 4e6f 6e65  bability is None
+00014d10: 206f 7220 6d69 6e5f 7072 6f62 203e 2061   or min_prob > a
+00014d20: 6c6c 5f77 6f72 6473 5b69 5d2e 7072 6f62  ll_words[i].prob
+00014d30: 6162 696c 6974 7929 2061 6e64 0d0a 2020  ability) and..  
+00014d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d50: 2020 2866 696c 7465 7273 2069 7320 4e6f    (filters is No
+00014d60: 6e65 206f 7220 6669 6c74 6572 7328 616c  ne or filters(al
+00014d70: 6c5f 776f 7264 735b 695d 2929 0d0a 2020  l_words[i]))..  
+00014d80: 2020 2020 2020 2020 2020 293a 0d0a 2020            ):..  
+00014d90: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00014da0: 2076 6572 626f 7365 3a0d 0a20 2020 2020   verbose:..     
+00014db0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00014dc0: 6861 6e67 6573 2e61 7070 656e 6428 6627  hanges.append(f'
+00014dd0: 5265 6d6f 7665 643a 207b 616c 6c5f 776f  Removed: {all_wo
+00014de0: 7264 735b 695d 2e74 6f5f 6469 6374 2829  rds[i].to_dict()
+00014df0: 7d27 290d 0a20 2020 2020 2020 2020 2020  }')..           
+00014e00: 2020 2020 2073 656c 662e 7265 6d6f 7665       self.remove
+00014e10: 5f77 6f72 6428 616c 6c5f 776f 7264 735b  _word(all_words[
+00014e20: 695d 2c20 4661 6c73 652c 2076 6572 626f  i], False, verbo
+00014e30: 7365 3d46 616c 7365 290d 0a20 2020 2020  se=False)..     
+00014e40: 2020 2069 6620 6368 616e 6765 733a 0d0a     if changes:..
+00014e50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00014e60: 7428 275c 6e27 2e6a 6f69 6e28 7265 7665  t('\n'.join(reve
+00014e70: 7273 6564 2863 6861 6e67 6573 2929 290d  rsed(changes))).
+00014e80: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00014e90: 6d6f 7665 5f6e 6f5f 776f 7264 5f73 6567  move_no_word_seg
+00014ea0: 6d65 6e74 7328 290d 0a0d 0a20 2020 2020  ments()....     
+00014eb0: 2020 2072 6574 7572 6e20 7365 6c66 0d0a     return self..
+00014ec0: 0d0a 2020 2020 6465 6620 6669 6c6c 5f69  ..    def fill_i
+00014ed0: 6e5f 6761 7073 280d 0a20 2020 2020 2020  n_gaps(..       
+00014ee0: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
+00014ef0: 2020 2020 2020 2020 6f74 6865 725f 7265          other_re
+00014f00: 7375 6c74 3a20 556e 696f 6e5b 2757 6869  sult: Union['Whi
+00014f10: 7370 6572 5265 7375 6c74 272c 2073 7472  sperResult', str
+00014f20: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00014f30: 6d69 6e5f 6761 703a 2066 6c6f 6174 203d  min_gap: float =
+00014f40: 2030 2e31 2c0d 0a20 2020 2020 2020 2020   0.1,..         
+00014f50: 2020 2063 6173 655f 7365 6e73 6974 6976     case_sensitiv
+00014f60: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
+00014f70: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00014f80: 7269 703a 2062 6f6f 6c20 3d20 5472 7565  rip: bool = True
+00014f90: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
+00014fa0: 676e 6f72 655f 7075 6e63 7475 6174 696f  gnore_punctuatio
+00014fb0: 6e73 3a20 7374 7220 3d20 225c 2227 2c2e  ns: str = "\"',.
+00014fc0: 3f21 222c 0d0a 2020 2020 2020 2020 2020  ?!",..          
+00014fd0: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
+00014fe0: 3d20 5472 7565 0d0a 2020 2020 2920 2d3e  = True..    ) ->
+00014ff0: 2027 5768 6973 7065 7252 6573 756c 7427   'WhisperResult'
+00015000: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00015010: 2020 2020 2020 2020 4669 6c6c 2069 6e20          Fill in 
+00015020: 7365 676d 656e 7420 6761 7073 206c 6172  segment gaps lar
+00015030: 6765 7220 7468 616e 2060 606d 696e 5f67  ger than ``min_g
+00015040: 6170 6060 2077 6974 6820 636f 6e74 656e  ap`` with conten
+00015050: 7420 6672 6f6d 2060 606f 7468 6572 5f72  t from ``other_r
+00015060: 6573 756c 7460 6020 6174 2074 6865 2074  esult`` at the t
+00015070: 696d 6573 206f 6620 6761 7073 2e0d 0a0d  imes of gaps....
+00015080: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00015090: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
+000150a0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+000150b0: 206f 7468 6572 5f72 6573 756c 7420 3a20   other_result : 
+000150c0: 5768 6973 7065 7252 6573 756c 7420 6f72  WhisperResult or
+000150d0: 2073 7472 0d0a 2020 2020 2020 2020 2020   str..          
+000150e0: 2020 416e 6f74 6865 7220 7472 616e 7363    Another transc
+000150f0: 7269 7074 696f 6e20 7265 7375 6c74 2061  ription result a
+00015100: 7320 616e 2069 6e73 7461 6e63 6520 6f66  s an instance of
+00015110: 203a 636c 6173 733a 6073 7461 626c 655f   :class:`stable_
+00015120: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
+00015130: 6869 7370 6572 5265 7375 6c74 6020 6f72  hisperResult` or
+00015140: 2070 6174 6820 746f 2074 6865 0d0a 2020   path to the..  
+00015150: 2020 2020 2020 2020 2020 4a53 4f4e 206f            JSON o
+00015160: 6620 7468 6520 7265 7375 6c74 2e0d 0a20  f the result... 
+00015170: 2020 2020 2020 206d 696e 5f67 6170 203a         min_gap :
+00015180: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
+00015190: 302e 310d 0a20 2020 2020 2020 2020 2020  0.1..           
+000151a0: 2054 6865 206d 696e 696d 756d 2073 6563   The minimum sec
+000151b0: 6f6e 6473 206f 6620 6120 6761 7020 6265  onds of a gap be
+000151c0: 7477 6565 6e20 7365 676d 656e 7473 2074  tween segments t
+000151d0: 6861 7420 6d75 7374 2062 6520 6578 6365  hat must be exce
+000151e0: 6564 6564 2074 6f20 6265 2066 696c 6c65  eded to be fille
+000151f0: 6420 696e 2e0d 0a20 2020 2020 2020 2063  d in...        c
+00015200: 6173 655f 7365 6e73 6974 6976 6520 3a20  ase_sensitive : 
+00015210: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
+00015220: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+00015230: 2057 6865 7468 6572 2074 6f20 636f 6e73   Whether to cons
+00015240: 6964 6572 2074 6865 2063 6173 6520 6f66  ider the case of
+00015250: 2074 6865 2066 6972 7374 2061 6e64 206c   the first and l
+00015260: 6173 7420 776f 7264 206f 6620 7468 6520  ast word of the 
+00015270: 6761 7020 746f 2064 6574 6572 6d69 6e65  gap to determine
+00015280: 206f 7665 726c 6170 7069 6e67 2077 6f72   overlapping wor
+00015290: 6473 2074 6f20 7265 6d6f 7665 0d0a 2020  ds to remove..  
+000152a0: 2020 2020 2020 2020 2020 6265 666f 7265            before
+000152b0: 2066 696c 6c69 6e67 2069 6e2e 0d0a 2020   filling in...  
+000152c0: 2020 2020 2020 7374 7269 7020 3a20 626f        strip : bo
+000152d0: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+000152e0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+000152f0: 6574 6865 7220 746f 2069 676e 6f72 6520  ether to ignore 
+00015300: 7370 6163 6573 2062 6566 6f72 6520 616e  spaces before an
+00015310: 6420 6166 7465 7220 7468 6520 6669 7273  d after the firs
+00015320: 7420 616e 6420 6c61 7374 2077 6f72 6420  t and last word 
+00015330: 6f66 2074 6865 2067 6170 2074 6f20 6465  of the gap to de
+00015340: 7465 726d 696e 6520 6f76 6572 6c61 7070  termine overlapp
+00015350: 696e 6720 776f 7264 730d 0a20 2020 2020  ing words..     
+00015360: 2020 2020 2020 2074 6f20 7265 6d6f 7665         to remove
+00015370: 2062 6566 6f72 6520 6669 6c6c 696e 6720   before filling 
+00015380: 696e 2e0d 0a20 2020 2020 2020 2069 676e  in...        ign
+00015390: 6f72 655f 7075 6e63 7475 6174 696f 6e73  ore_punctuations
+000153a0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+000153b0: 2027 2227 2c2e 3f21 270d 0a20 2020 2020   '"',.?!'..     
+000153c0: 2020 2020 2020 2045 6e64 696e 6720 7075         Ending pu
+000153d0: 6e63 7475 6174 696f 6e73 2074 6f20 6967  nctuations to ig
+000153e0: 6e6f 7265 2069 6e20 7468 6520 6669 7273  nore in the firs
+000153f0: 7420 616e 6420 6c61 7374 2077 6f72 6420  t and last word 
+00015400: 6f66 2074 6865 2067 6170 2074 6f20 6465  of the gap to de
+00015410: 7465 726d 696e 6520 6f76 6572 6c61 7070  termine overlapp
+00015420: 696e 6720 776f 7264 7320 746f 0d0a 2020  ing words to..  
+00015430: 2020 2020 2020 2020 2020 7265 6d6f 7665            remove
+00015440: 2062 6566 6f72 6520 6669 6c6c 696e 6720   before filling 
+00015450: 696e 2e0d 0a20 2020 2020 2020 2076 6572  in...        ver
+00015460: 626f 7365 3a0d 0a20 2020 2020 2020 2020  bose:..         
+00015470: 2020 2057 6865 7468 6572 2074 6f20 7072     Whether to pr
+00015480: 696e 7420 6465 7461 696c 206f 6620 7468  int detail of th
+00015490: 6520 6669 6c6c 6564 2063 6f6e 7465 6e74  e filled content
+000154a0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+000154b0: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
+000154c0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
+000154d0: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
+000154e0: 7375 6c74 2e57 6869 7370 6572 5265 7375  sult.WhisperResu
+000154f0: 6c74 0d0a 2020 2020 2020 2020 2020 2020  lt..            
+00015500: 5468 6520 6375 7272 656e 7420 696e 7374  The current inst
+00015510: 616e 6365 2061 6674 6572 2074 6865 2063  ance after the c
+00015520: 6861 6e67 6573 2e0d 0a20 2020 2020 2020  hanges...       
+00015530: 2022 2222 0d0a 2020 2020 2020 2020 6966   """..        if
+00015540: 206c 656e 2873 656c 662e 7365 676d 656e   len(self.segmen
+00015550: 7473 2920 3c20 323a 0d0a 2020 2020 2020  ts) < 2:..      
+00015560: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00015570: 660d 0a20 2020 2020 2020 2069 6620 6973  f..        if is
+00015580: 696e 7374 616e 6365 286f 7468 6572 5f72  instance(other_r
+00015590: 6573 756c 742c 2073 7472 293a 0d0a 2020  esult, str):..  
+000155a0: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
+000155b0: 7265 7375 6c74 203d 2057 6869 7370 6572  result = Whisper
+000155c0: 5265 7375 6c74 286f 7468 6572 5f72 6573  Result(other_res
+000155d0: 756c 7429 0d0a 0d0a 2020 2020 2020 2020  ult)....        
+000155e0: 6966 2073 7472 6970 3a0d 0a20 2020 2020  if strip:..     
+000155f0: 2020 2020 2020 2064 6566 2073 7472 6970         def strip
+00015600: 5f73 7061 6365 2877 293a 0d0a 2020 2020  _space(w):..    
+00015610: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00015620: 726e 2077 2e73 7472 6970 2829 0d0a 2020  rn w.strip()..  
+00015630: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00015640: 2020 2020 2020 2020 2064 6566 2073 7472           def str
+00015650: 6970 5f73 7061 6365 2877 293a 0d0a 2020  ip_space(w):..  
+00015660: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00015670: 7475 726e 2077 0d0a 0d0a 2020 2020 2020  turn w....      
+00015680: 2020 6966 2069 676e 6f72 655f 7075 6e63    if ignore_punc
+00015690: 7475 6174 696f 6e73 3a0d 0a20 2020 2020  tuations:..     
+000156a0: 2020 2020 2020 2070 746e 203d 2066 275b         ptn = f'[
+000156b0: 7b69 676e 6f72 655f 7075 6e63 7475 6174  {ignore_punctuat
+000156c0: 696f 6e73 7d5d 2b24 270d 0a0d 0a20 2020  ions}]+$'....   
+000156d0: 2020 2020 2020 2020 2064 6566 2073 7472           def str
+000156e0: 6970 5f70 756e 6374 7561 7469 6f6e 7328  ip_punctuations(
+000156f0: 7729 3a0d 0a20 2020 2020 2020 2020 2020  w):..           
+00015700: 2020 2020 2072 6574 7572 6e20 7265 2e73       return re.s
+00015710: 7562 2870 746e 2c20 2727 2c20 7374 7269  ub(ptn, '', stri
+00015720: 705f 7370 6163 6528 7729 290d 0a20 2020  p_space(w))..   
+00015730: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00015740: 2020 2020 2020 2020 7374 7269 705f 7075          strip_pu
+00015750: 6e63 7475 6174 696f 6e73 203d 2073 7472  nctuations = str
+00015760: 6970 5f73 7061 6365 0d0a 0d0a 2020 2020  ip_space....    
+00015770: 2020 2020 6966 2063 6173 655f 7365 6e73      if case_sens
+00015780: 6974 6976 653a 0d0a 2020 2020 2020 2020  itive:..        
+00015790: 2020 2020 7374 7269 7020 3d20 7374 7269      strip = stri
+000157a0: 705f 7075 6e63 7475 6174 696f 6e73 0d0a  p_punctuations..
+000157b0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+000157c0: 2020 2020 2020 2020 2020 2064 6566 2073             def s
+000157d0: 7472 6970 2877 293a 0d0a 2020 2020 2020  trip(w):..      
+000157e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000157f0: 2073 7472 6970 5f70 756e 6374 7561 7469   strip_punctuati
+00015800: 6f6e 7328 7729 2e6c 6f77 6572 2829 0d0a  ons(w).lower()..
+00015810: 0d0a 2020 2020 2020 2020 7365 675f 7061  ..        seg_pa
+00015820: 6972 7320 3d20 6c69 7374 2865 6e75 6d65  irs = list(enume
+00015830: 7261 7465 287a 6970 2873 656c 662e 7365  rate(zip(self.se
+00015840: 676d 656e 7473 5b3a 2d31 5d2c 2073 656c  gments[:-1], sel
+00015850: 662e 7365 676d 656e 7473 5b31 3a5d 2929  f.segments[1:]))
+00015860: 290d 0a20 2020 2020 2020 2073 6567 5f70  )..        seg_p
+00015870: 6169 7273 2e69 6e73 6572 7428 302c 2028  airs.insert(0, (
+00015880: 2d31 2c20 284e 6f6e 652c 2073 656c 662e  -1, (None, self.
+00015890: 7365 676d 656e 7473 5b30 5d29 2929 0d0a  segments[0])))..
+000158a0: 2020 2020 2020 2020 7365 675f 7061 6972          seg_pair
+000158b0: 732e 6170 7065 6e64 2828 7365 675f 7061  s.append((seg_pa
+000158c0: 6972 735b 2d31 5d5b 305d 2b31 2c20 2873  irs[-1][0]+1, (s
+000158d0: 656c 662e 7365 676d 656e 7473 5b2d 315d  elf.segments[-1]
+000158e0: 2c20 4e6f 6e65 2929 290d 0a0d 0a20 2020  , None)))....   
+000158f0: 2020 2020 2063 6861 6e67 6573 203d 205b       changes = [
+00015900: 5d0d 0a20 2020 2020 2020 2066 6f72 2069  ]..        for i
+00015910: 2c20 2873 6567 302c 2073 6567 3129 2069  , (seg0, seg1) i
+00015920: 6e20 7265 7665 7273 6564 2873 6567 5f70  n reversed(seg_p
+00015930: 6169 7273 293a 0d0a 2020 2020 2020 2020  airs):..        
+00015940: 2020 2020 6669 7273 745f 776f 7264 203d      first_word =
+00015950: 204e 6f6e 6520 6966 2073 6567 3020 6973   None if seg0 is
+00015960: 204e 6f6e 6520 656c 7365 2073 6567 302e   None else seg0.
+00015970: 776f 7264 735b 2d31 5d0d 0a20 2020 2020  words[-1]..     
+00015980: 2020 2020 2020 206c 6173 745f 776f 7264         last_word
+00015990: 203d 204e 6f6e 6520 6966 2073 6567 3120   = None if seg1 
+000159a0: 6973 204e 6f6e 6520 656c 7365 2073 6567  is None else seg
+000159b0: 312e 776f 7264 735b 305d 0d0a 2020 2020  1.words[0]..    
+000159c0: 2020 2020 2020 2020 7374 6172 7420 3d20          start = 
+000159d0: 286f 7468 6572 5f72 6573 756c 745b 305d  (other_result[0]
+000159e0: 2e73 7461 7274 2069 6620 6669 7273 745f  .start if first_
+000159f0: 776f 7264 2069 7320 4e6f 6e65 2065 6c73  word is None els
+00015a00: 6520 6669 7273 745f 776f 7264 2e65 6e64  e first_word.end
+00015a10: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00015a20: 6e64 203d 206f 7468 6572 5f72 6573 756c  nd = other_resul
+00015a30: 745b 2d31 5d2e 656e 6420 6966 206c 6173  t[-1].end if las
+00015a40: 745f 776f 7264 2069 7320 4e6f 6e65 2065  t_word is None e
+00015a50: 6c73 6520 6c61 7374 5f77 6f72 642e 7374  lse last_word.st
+00015a60: 6172 740d 0a20 2020 2020 2020 2020 2020  art..           
+00015a70: 2069 6620 656e 6420 2d20 7374 6172 7420   if end - start 
+00015a80: 3c3d 206d 696e 5f67 6170 3a0d 0a20 2020  <= min_gap:..   
+00015a90: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00015aa0: 7469 6e75 650d 0a20 2020 2020 2020 2020  tinue..         
+00015ab0: 2020 2067 6170 5f77 6f72 6473 203d 206f     gap_words = o
+00015ac0: 7468 6572 5f72 6573 756c 742e 6765 745f  ther_result.get_
+00015ad0: 636f 6e74 656e 745f 6279 5f74 696d 6528  content_by_time(
+00015ae0: 2873 7461 7274 2c20 656e 6429 290d 0a20  (start, end)).. 
+00015af0: 2020 2020 2020 2020 2020 2069 6620 6669             if fi
+00015b00: 7273 745f 776f 7264 2069 7320 6e6f 7420  rst_word is not 
+00015b10: 4e6f 6e65 2061 6e64 2067 6170 5f77 6f72  None and gap_wor
+00015b20: 6473 2061 6e64 2073 7472 6970 2866 6972  ds and strip(fir
+00015b30: 7374 5f77 6f72 642e 776f 7264 2920 3d3d  st_word.word) ==
+00015b40: 2073 7472 6970 2867 6170 5f77 6f72 6473   strip(gap_words
+00015b50: 5b30 5d2e 776f 7264 293a 0d0a 2020 2020  [0].word):..    
+00015b60: 2020 2020 2020 2020 2020 2020 6669 7273              firs
+00015b70: 745f 776f 7264 2e65 6e64 203d 2067 6170  t_word.end = gap
+00015b80: 5f77 6f72 6473 5b30 5d2e 656e 640d 0a20  _words[0].end.. 
+00015b90: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00015ba0: 6170 5f77 6f72 6473 203d 2067 6170 5f77  ap_words = gap_w
+00015bb0: 6f72 6473 5b31 3a5d 0d0a 2020 2020 2020  ords[1:]..      
+00015bc0: 2020 2020 2020 6966 206c 6173 745f 776f        if last_wo
+00015bd0: 7264 2069 7320 6e6f 7420 4e6f 6e65 2061  rd is not None a
+00015be0: 6e64 2067 6170 5f77 6f72 6473 2061 6e64  nd gap_words and
+00015bf0: 2073 7472 6970 286c 6173 745f 776f 7264   strip(last_word
+00015c00: 2e77 6f72 6429 203d 3d20 7374 7269 7028  .word) == strip(
+00015c10: 6761 705f 776f 7264 735b 2d31 5d2e 776f  gap_words[-1].wo
+00015c20: 7264 293a 0d0a 2020 2020 2020 2020 2020  rd):..          
+00015c30: 2020 2020 2020 6c61 7374 5f77 6f72 642e        last_word.
+00015c40: 7374 6172 7420 3d20 6761 705f 776f 7264  start = gap_word
+00015c50: 735b 2d31 5d2e 7374 6172 740d 0a20 2020  s[-1].start..   
+00015c60: 2020 2020 2020 2020 2020 2020 2067 6170               gap
+00015c70: 5f77 6f72 6473 203d 2067 6170 5f77 6f72  _words = gap_wor
+00015c80: 6473 5b3a 2d31 5d0d 0a20 2020 2020 2020  ds[:-1]..       
+00015c90: 2020 2020 2069 6620 6e6f 7420 6761 705f       if not gap_
+00015ca0: 776f 7264 733a 0d0a 2020 2020 2020 2020  words:..        
+00015cb0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00015cc0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00015cd0: 206c 6173 745f 776f 7264 2069 7320 6e6f   last_word is no
+00015ce0: 7420 4e6f 6e65 2061 6e64 206c 6173 745f  t None and last_
+00015cf0: 776f 7264 2e73 7461 7274 203c 2067 6170  word.start < gap
+00015d00: 5f77 6f72 6473 5b2d 315d 2e65 6e64 3a0d  _words[-1].end:.
+00015d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015d20: 206c 6173 745f 776f 7264 2e73 7461 7274   last_word.start
+00015d30: 203d 2067 6170 5f77 6f72 6473 5b2d 315d   = gap_words[-1]
+00015d40: 2e65 6e64 0d0a 2020 2020 2020 2020 2020  .end..          
+00015d50: 2020 6e65 775f 7365 676d 656e 7473 203d    new_segments =
+00015d60: 205b 6f74 6865 725f 7265 7375 6c74 5b67   [other_result[g
+00015d70: 6170 5f77 6f72 6473 5b30 5d2e 7365 676d  ap_words[0].segm
+00015d80: 656e 745f 6964 5d2e 636f 7079 285b 5d29  ent_id].copy([])
+00015d90: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
+00015da0: 6f72 206a 2c20 6e65 775f 776f 7264 2069  or j, new_word i
+00015db0: 6e20 656e 756d 6572 6174 6528 6761 705f  n enumerate(gap_
+00015dc0: 776f 7264 7329 3a0d 0a20 2020 2020 2020  words):..       
+00015dd0: 2020 2020 2020 2020 206e 6577 5f77 6f72           new_wor
+00015de0: 645f 636f 7079 203d 206e 6577 5f77 6f72  d_copy = new_wor
+00015df0: 642e 636f 7079 2863 6f70 795f 746f 6b65  d.copy(copy_toke
+00015e00: 6e73 3d54 7275 6529 0d0a 2020 2020 2020  ns=True)..      
+00015e10: 2020 2020 2020 2020 2020 6966 206a 203d            if j =
+00015e20: 3d20 3020 616e 6420 6669 7273 745f 776f  = 0 and first_wo
+00015e30: 7264 2069 7320 6e6f 7420 4e6f 6e65 2061  rd is not None a
+00015e40: 6e64 2066 6972 7374 5f77 6f72 642e 656e  nd first_word.en
+00015e50: 6420 3e20 6761 705f 776f 7264 735b 305d  d > gap_words[0]
+00015e60: 2e73 7461 7274 3a0d 0a20 2020 2020 2020  .start:..       
+00015e70: 2020 2020 2020 2020 2020 2020 206e 6577               new
+00015e80: 5f77 6f72 645f 636f 7079 2e73 7461 7274  _word_copy.start
+00015e90: 203d 2066 6972 7374 5f77 6f72 642e 656e   = first_word.en
+00015ea0: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
+00015eb0: 2020 2069 6620 6e65 775f 7365 676d 656e     if new_segmen
+00015ec0: 7473 5b2d 315d 2e69 6420 213d 206e 6577  ts[-1].id != new
+00015ed0: 5f77 6f72 642e 7365 676d 656e 745f 6964  _word.segment_id
+00015ee0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00015ef0: 2020 2020 2020 206e 6577 5f73 6567 6d65         new_segme
+00015f00: 6e74 732e 6170 7065 6e64 286f 7468 6572  nts.append(other
+00015f10: 5f72 6573 756c 745b 6e65 775f 776f 7264  _result[new_word
+00015f20: 2e73 6567 6d65 6e74 5f69 645d 2e63 6f70  .segment_id].cop
+00015f30: 7928 5b5d 2929 0d0a 2020 2020 2020 2020  y([]))..        
+00015f40: 2020 2020 2020 2020 6e65 775f 7365 676d          new_segm
+00015f50: 656e 7473 5b2d 315d 2e77 6f72 6473 2e61  ents[-1].words.a
+00015f60: 7070 656e 6428 6e65 775f 776f 7264 5f63  ppend(new_word_c
+00015f70: 6f70 7929 0d0a 2020 2020 2020 2020 2020  opy)..          
+00015f80: 2020 6966 2076 6572 626f 7365 3a0d 0a20    if verbose:.. 
+00015f90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00015fa0: 6861 6e67 6573 2e61 7070 656e 6428 275c  hanges.append('\
+00015fb0: 6e27 2e6a 6f69 6e28 2741 6464 6564 3a20  n'.join('Added: 
+00015fc0: 2720 2b20 732e 746f 5f64 6973 706c 6179  ' + s.to_display
+00015fd0: 5f73 7472 2854 7275 6529 2066 6f72 2073  _str(True) for s
+00015fe0: 2069 6e20 6e65 775f 7365 676d 656e 7473   in new_segments
+00015ff0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00016000: 7365 6c66 2e73 6567 6d65 6e74 7320 3d20  self.segments = 
+00016010: 7365 6c66 2e73 6567 6d65 6e74 735b 3a69  self.segments[:i
+00016020: 2b31 5d20 2b20 6e65 775f 7365 676d 656e  +1] + new_segmen
+00016030: 7473 202b 2073 656c 662e 7365 676d 656e  ts + self.segmen
+00016040: 7473 5b69 2b31 3a5d 0d0a 2020 2020 2020  ts[i+1:]..      
+00016050: 2020 6966 2063 6861 6e67 6573 3a0d 0a20    if changes:.. 
+00016060: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00016070: 2827 5c6e 272e 6a6f 696e 2872 6576 6572  ('\n'.join(rever
+00016080: 7365 6428 6368 616e 6765 7329 2929 0d0a  sed(changes)))..
+00016090: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
+000160a0: 7373 6967 6e5f 6964 7328 290d 0a0d 0a20  ssign_ids().... 
+000160b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000160c0: 6c66 0d0a 0d0a 2020 2020 6465 6620 7265  lf....    def re
+000160d0: 6772 6f75 7028 0d0a 2020 2020 2020 2020  group(..        
+000160e0: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+000160f0: 2020 2020 2020 2072 6567 726f 7570 5f61         regroup_a
+00016100: 6c67 6f3a 2055 6e69 6f6e 5b73 7472 2c20  lgo: Union[str, 
+00016110: 626f 6f6c 5d20 3d20 4e6f 6e65 2c0d 0a20  bool] = None,.. 
+00016120: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
+00016130: 7365 3a20 626f 6f6c 203d 2046 616c 7365  se: bool = False
+00016140: 2c0d 0a20 2020 2020 2020 2020 2020 206f  ,..            o
+00016150: 6e6c 795f 7368 6f77 3a20 626f 6f6c 203d  nly_show: bool =
+00016160: 2046 616c 7365 0d0a 2020 2020 2920 2d3e   False..    ) ->
+00016170: 2022 5768 6973 7065 7252 6573 756c 7422   "WhisperResult"
+00016180: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00016190: 2020 2020 2020 2020 5265 6772 6f75 7020          Regroup 
+000161a0: 2869 6e2d 706c 6163 6529 2077 6f72 6473  (in-place) words
+000161b0: 2069 6e74 6f20 7365 676d 656e 7473 2e0d   into segments..
+000161c0: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+000161d0: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
+000161e0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
+000161f0: 2020 2072 6567 726f 7570 5f61 6c67 6f3a     regroup_algo:
+00016200: 2073 7472 206f 7220 626f 6f6c 2c20 6465   str or bool, de
+00016210: 6661 756c 7420 2764 6127 0d0a 2020 2020  fault 'da'..    
+00016220: 2020 2020 2020 2020 2053 7472 696e 6720           String 
+00016230: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
+00016240: 6620 6120 6375 7374 6f6d 2072 6567 726f  f a custom regro
+00016250: 7570 696e 6720 616c 676f 7269 7468 6d20  uping algorithm 
+00016260: 6f72 2060 6054 7275 6560 6020 7573 6520  or ``True`` use 
+00016270: 746f 2074 6865 2064 6566 6175 6c74 2061  to the default a
+00016280: 6c67 6f72 6974 686d 2027 6461 272e 0d0a  lgorithm 'da'...
+00016290: 2020 2020 2020 2020 7665 7262 6f73 6520          verbose 
+000162a0: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
+000162b0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
+000162c0: 2020 2057 6865 7468 6572 2074 6f20 7368     Whether to sh
+000162d0: 6f77 2061 6c6c 2074 6865 206d 6574 686f  ow all the metho
+000162e0: 6473 2061 6e64 2061 7267 756d 656e 7473  ds and arguments
+000162f0: 2070 6172 7365 6420 6672 6f6d 2060 6072   parsed from ``r
+00016300: 6567 726f 7570 5f61 6c67 6f60 602e 0d0a  egroup_algo``...
+00016310: 2020 2020 2020 2020 6f6e 6c79 5f73 686f          only_sho
+00016320: 7720 3a20 626f 6f6c 2c20 6465 6661 756c  w : bool, defaul
+00016330: 7420 4661 6c73 650d 0a20 2020 2020 2020  t False..       
+00016340: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
+00016350: 7368 6f77 2074 6865 2061 6c6c 206d 6574  show the all met
+00016360: 686f 6473 2061 6e64 2061 7267 756d 656e  hods and argumen
+00016370: 7473 2070 6172 7365 6420 6672 6f6d 2060  ts parsed from `
+00016380: 6072 6567 726f 7570 5f61 6c67 6f60 6020  `regroup_algo`` 
+00016390: 7769 7468 6f75 7420 7275 6e6e 696e 6720  without running 
+000163a0: 7468 6520 6d65 7468 6f64 730d 0a0d 0a20  the methods.... 
+000163b0: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
+000163c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
+000163d0: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
+000163e0: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
+000163f0: 6869 7370 6572 5265 7375 6c74 0d0a 2020  hisperResult..  
+00016400: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
+00016410: 7272 656e 7420 696e 7374 616e 6365 2061  rrent instance a
+00016420: 6674 6572 2074 6865 2063 6861 6e67 6573  fter the changes
+00016430: 2e0d 0a0d 0a20 2020 2020 2020 204e 6f74  .....        Not
+00016440: 6573 0d0a 2020 2020 2020 2020 2d2d 2d2d  es..        ----
+00016450: 2d0d 0a20 2020 2020 2020 2053 796e 7461  -..        Synta
+00016460: 7820 666f 7220 7374 7269 6e67 2072 6570  x for string rep
+00016470: 7265 7365 6e74 6174 696f 6e20 6f66 2063  resentation of c
+00016480: 7573 746f 6d20 7265 6772 6f75 7069 6e67  ustom regrouping
+00016490: 2061 6c67 6f72 6974 686d 2e0d 0a20 2020   algorithm...   
+000164a0: 2020 2020 2020 2020 204d 6574 686f 6420           Method 
+000164b0: 6b65 7973 3a0d 0a20 2020 2020 2020 2020  keys:..         
+000164c0: 2020 2020 2020 2073 673a 2073 706c 6974         sg: split
+000164d0: 5f62 795f 6761 700d 0a20 2020 2020 2020  _by_gap..       
+000164e0: 2020 2020 2020 2020 2073 703a 2073 706c           sp: spl
+000164f0: 6974 5f62 795f 7075 6e63 7475 6174 696f  it_by_punctuatio
+00016500: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00016510: 2020 2073 6c3a 2073 706c 6974 5f62 795f     sl: split_by_
+00016520: 6c65 6e67 7468 0d0a 2020 2020 2020 2020  length..        
+00016530: 2020 2020 2020 2020 7364 3a20 7370 6c69          sd: spli
+00016540: 745f 6279 5f64 7572 6174 696f 6e0d 0a20  t_by_duration.. 
+00016550: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016560: 673a 206d 6572 6765 5f62 795f 6761 700d  g: merge_by_gap.
+00016570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016580: 206d 703a 206d 6572 6765 5f62 795f 7075   mp: merge_by_pu
+00016590: 6e63 7475 6174 696f 6e0d 0a20 2020 2020  nctuation..     
+000165a0: 2020 2020 2020 2020 2020 206d 733a 206d             ms: m
+000165b0: 6572 6765 5f61 6c6c 5f73 6567 6d65 6e74  erge_all_segment
+000165c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000165d0: 2020 636d 3a20 636c 616d 705f 6d61 780d    cm: clamp_max.
+000165e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000165f0: 206c 3a20 6c6f 636b 0d0a 2020 2020 2020   l: lock..      
+00016600: 2020 2020 2020 2020 2020 7573 3a20 756e            us: un
+00016610: 6c6f 636b 5f61 6c6c 5f73 6567 6d65 6e74  lock_all_segment
+00016620: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00016630: 2020 2064 613a 2064 6566 6175 6c74 2061     da: default a
+00016640: 6c67 6f72 6974 686d 2028 636d 5f73 703d  lgorithm (cm_sp=
+00016650: 2c2a 202f efbc 8c5f 7367 3d2e 355f 6d67  ,* /..._sg=.5_mg
+00016660: 3d2e 332b 335f 7370 3d2e 2a20 2fe3 8082  =.3+3_sp=.* /...
+00016670: 2f3f 2fef bc9f 290d 0a20 2020 2020 2020  /?/...)..       
+00016680: 2020 2020 2020 2020 2072 773a 2072 656d           rw: rem
+00016690: 6f76 655f 776f 7264 0d0a 2020 2020 2020  ove_word..      
+000166a0: 2020 2020 2020 2020 2020 7273 3a20 7265            rs: re
+000166b0: 6d6f 7665 5f73 6567 6d65 6e74 0d0a 2020  move_segment..  
+000166c0: 2020 2020 2020 2020 2020 2020 2020 7270                rp
+000166d0: 3a20 7265 6d6f 7665 5f72 6570 6574 6974  : remove_repetit
+000166e0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+000166f0: 2020 2020 2072 7773 3a20 7265 6d6f 7665       rws: remove
+00016700: 5f77 6f72 6473 5f62 795f 7374 720d 0a20  _words_by_str.. 
+00016710: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00016720: 673a 2066 696c 6c5f 696e 5f67 6170 730d  g: fill_in_gaps.
+00016730: 0a20 2020 2020 2020 2020 2020 204d 6574  .            Met
+00016740: 6163 6861 7261 6374 6572 733a 0d0a 2020  acharacters:..  
+00016750: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
+00016760: 7365 7061 7261 7465 7320 6120 6d65 7468  separates a meth
+00016770: 6f64 206b 6579 2061 6e64 2069 7473 2061  od key and its a
+00016780: 7267 756d 656e 7473 2028 6e6f 7420 7573  rguments (not us
+00016790: 6564 2069 6620 6e6f 2061 7267 756d 656e  ed if no argumen
+000167a0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+000167b0: 2020 2020 5f20 7365 7061 7261 7465 7320      _ separates 
+000167c0: 6d65 7468 6f64 206b 6579 7320 2861 6674  method keys (aft
+000167d0: 6572 2061 7267 756d 656e 7473 2069 6620  er arguments if 
+000167e0: 7468 6572 6520 6172 6520 616e 7929 0d0a  there are any)..
+000167f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016800: 2b20 7365 7061 7261 7465 7320 6172 6775  + separates argu
+00016810: 6d65 6e74 7320 666f 7220 6120 6d65 7468  ments for a meth
+00016820: 6f64 206b 6579 0d0a 2020 2020 2020 2020  od key..        
+00016830: 2020 2020 2020 2020 2f20 7365 7061 7261          / separa
+00016840: 7465 7320 616e 2061 7267 756d 656e 7420  tes an argument 
+00016850: 696e 746f 206c 6973 7420 6f66 2073 7472  into list of str
+00016860: 696e 6773 0d0a 2020 2020 2020 2020 2020  ings..          
+00016870: 2020 2020 2020 2a20 7365 7061 7261 7465        * separate
+00016880: 7320 616e 2069 7465 6d20 696e 206c 6973  s an item in lis
+00016890: 7420 6f66 2073 7472 696e 6773 2069 6e74  t of strings int
+000168a0: 6f20 6120 6e65 7374 6564 206c 6973 7420  o a nested list 
+000168b0: 6f66 2073 7472 696e 6773 0d0a 2020 2020  of strings..    
+000168c0: 2020 2020 2020 2020 4e6f 7465 733a 0d0a          Notes:..
+000168d0: 2020 2020 2020 2020 2020 2020 2d61 7267              -arg
+000168e0: 756d 656e 7473 2061 7265 2070 6172 7365  uments are parse
+000168f0: 6420 706f 7369 7469 6f6e 616c 6c79 0d0a  d positionally..
+00016900: 2020 2020 2020 2020 2020 2020 2d69 6620              -if 
+00016910: 6e6f 2061 7267 756d 656e 7420 6973 2070  no argument is p
+00016920: 726f 7669 6465 642c 2074 6865 2064 6566  rovided, the def
+00016930: 6175 6c74 206f 6e65 7320 7769 6c6c 2062  ault ones will b
+00016940: 6520 7573 6564 0d0a 2020 2020 2020 2020  e used..        
+00016950: 2020 2020 2d75 7365 2031 206f 7220 3020      -use 1 or 0 
+00016960: 746f 2072 6570 7265 7365 6e74 2054 7275  to represent Tru
+00016970: 6520 6f72 2046 616c 7365 0d0a 2020 2020  e or False..    
+00016980: 2020 2020 2020 2020 4578 616d 706c 6520          Example 
+00016990: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+000169a0: 2020 2020 6d65 7267 655f 6279 5f67 6170      merge_by_gap
+000169b0: 282e 322c 2031 302c 206c 6f63 6b3d 5472  (.2, 10, lock=Tr
+000169c0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+000169d0: 2020 2020 206d 673d 2e32 2b31 302b 2b2b       mg=.2+10+++
+000169e0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+000169f0: 2020 204e 6f74 653a 205b 6c6f 636b 5d20     Note: [lock] 
+00016a00: 6973 2074 6865 2035 7468 2061 7267 756d  is the 5th argum
+00016a10: 656e 7420 6865 6e63 6520 7468 6520 3220  ent hence the 2 
+00016a20: 6d69 7373 696e 6720 6172 6775 6d65 6e74  missing argument
+00016a30: 7320 696e 6265 7477 6565 6e20 7468 6520  s inbetween the 
+00016a40: 7468 7265 6520 2b20 6265 666f 7265 2031  three + before 1
+00016a50: 0d0a 2020 2020 2020 2020 2020 2020 4578  ..            Ex
+00016a60: 616d 706c 6520 323a 0d0a 2020 2020 2020  ample 2:..      
+00016a70: 2020 2020 2020 2020 2020 7370 6c69 745f            split_
+00016a80: 6279 5f70 756e 6374 7561 7469 6f6e 285b  by_punctuation([
+00016a90: 2827 2e27 2c20 2720 2729 2c20 27e3 8082  ('.', ' '), '...
+00016aa0: 272c 2027 3f27 2c20 27ef bc9f 275d 2c20  ', '?', '...'], 
+00016ab0: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
+00016ac0: 2020 2020 2020 2073 703d 2e2a 202f e380         sp=.* /..
+00016ad0: 822f 3f2f efbc 9f2b 310d 0a20 2020 2020  ./?/...+1..     
+00016ae0: 2020 2020 2020 2045 7861 6d70 6c65 2033         Example 3
+00016af0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00016b00: 2020 206d 6572 6765 5f61 6c6c 5f73 6567     merge_all_seg
+00016b10: 6d65 6e74 7328 292e 7370 6c69 745f 6279  ments().split_by
+00016b20: 5f67 6170 282e 3529 2e6d 6572 6765 5f62  _gap(.5).merge_b
+00016b30: 795f 6761 7028 2e31 352c 2033 290d 0a20  y_gap(.15, 3).. 
+00016b40: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016b50: 735f 7367 3d2e 355f 6d67 3d2e 3135 2b33  s_sg=.5_mg=.15+3
+00016b60: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00016b70: 2020 2020 2020 2069 6620 7265 6772 6f75         if regrou
+00016b80: 705f 616c 676f 2069 7320 4661 6c73 653a  p_algo is False:
+00016b90: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00016ba0: 7475 726e 2073 656c 660d 0a20 2020 2020  turn self..     
+00016bb0: 2020 2069 6620 7265 6772 6f75 705f 616c     if regroup_al
+00016bc0: 676f 2069 7320 4e6f 6e65 206f 7220 7265  go is None or re
+00016bd0: 6772 6f75 705f 616c 676f 2069 7320 5472  group_algo is Tr
+00016be0: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
+00016bf0: 2072 6567 726f 7570 5f61 6c67 6f20 3d20   regroup_algo = 
+00016c00: 2764 6127 0d0a 0d0a 2020 2020 2020 2020  'da'....        
+00016c10: 666f 7220 6d65 7468 6f64 2c20 6b77 6172  for method, kwar
+00016c20: 6773 2c20 6d73 6720 696e 2073 656c 662e  gs, msg in self.
+00016c30: 7061 7273 655f 7265 6772 6f75 705f 616c  parse_regroup_al
+00016c40: 676f 2872 6567 726f 7570 5f61 6c67 6f2c  go(regroup_algo,
+00016c50: 2069 6e63 6c75 6465 5f73 7472 3d76 6572   include_str=ver
+00016c60: 626f 7365 206f 7220 6f6e 6c79 5f73 686f  bose or only_sho
+00016c70: 7729 3a0d 0a20 2020 2020 2020 2020 2020  w):..           
+00016c80: 2069 6620 6d73 673a 0d0a 2020 2020 2020   if msg:..      
+00016c90: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00016ca0: 6d73 6729 0d0a 2020 2020 2020 2020 2020  msg)..          
+00016cb0: 2020 6966 206e 6f74 206f 6e6c 795f 7368    if not only_sh
+00016cc0: 6f77 3a0d 0a20 2020 2020 2020 2020 2020  ow:..           
+00016cd0: 2020 2020 206d 6574 686f 6428 2a2a 6b77       method(**kw
+00016ce0: 6172 6773 290d 0a0d 0a20 2020 2020 2020  args)....       
+00016cf0: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
+00016d00: 2020 2020 6465 6620 7061 7273 655f 7265      def parse_re
+00016d10: 6772 6f75 705f 616c 676f 2873 656c 662c  group_algo(self,
+00016d20: 2072 6567 726f 7570 5f61 6c67 6f3a 2073   regroup_algo: s
+00016d30: 7472 2c20 696e 636c 7564 655f 7374 723a  tr, include_str:
+00016d40: 2062 6f6f 6c20 3d20 5472 7565 2920 2d3e   bool = True) ->
+00016d50: 204c 6973 745b 5475 706c 655b 4361 6c6c   List[Tuple[Call
+00016d60: 6162 6c65 2c20 6469 6374 2c20 7374 725d  able, dict, str]
+00016d70: 5d3a 0d0a 2020 2020 2020 2020 6d65 7468  ]:..        meth
+00016d80: 6f64 7320 3d20 6469 6374 280d 0a20 2020  ods = dict(..   
+00016d90: 2020 2020 2020 2020 2073 673d 7365 6c66           sg=self
+00016da0: 2e73 706c 6974 5f62 795f 6761 702c 0d0a  .split_by_gap,..
+00016db0: 2020 2020 2020 2020 2020 2020 7370 3d73              sp=s
+00016dc0: 656c 662e 7370 6c69 745f 6279 5f70 756e  elf.split_by_pun
+00016dd0: 6374 7561 7469 6f6e 2c0d 0a20 2020 2020  ctuation,..     
+00016de0: 2020 2020 2020 2073 6c3d 7365 6c66 2e73         sl=self.s
+00016df0: 706c 6974 5f62 795f 6c65 6e67 7468 2c0d  plit_by_length,.
+00016e00: 0a20 2020 2020 2020 2020 2020 2073 643d  .            sd=
+00016e10: 7365 6c66 2e73 706c 6974 5f62 795f 6475  self.split_by_du
+00016e20: 7261 7469 6f6e 2c0d 0a20 2020 2020 2020  ration,..       
+00016e30: 2020 2020 206d 673d 7365 6c66 2e6d 6572       mg=self.mer
+00016e40: 6765 5f62 795f 6761 702c 0d0a 2020 2020  ge_by_gap,..    
+00016e50: 2020 2020 2020 2020 6d70 3d73 656c 662e          mp=self.
+00016e60: 6d65 7267 655f 6279 5f70 756e 6374 7561  merge_by_punctua
+00016e70: 7469 6f6e 2c0d 0a20 2020 2020 2020 2020  tion,..         
+00016e80: 2020 206d 733d 7365 6c66 2e6d 6572 6765     ms=self.merge
+00016e90: 5f61 6c6c 5f73 6567 6d65 6e74 732c 0d0a  _all_segments,..
+00016ea0: 2020 2020 2020 2020 2020 2020 636d 3d73              cm=s
+00016eb0: 656c 662e 636c 616d 705f 6d61 782c 0d0a  elf.clamp_max,..
+00016ec0: 2020 2020 2020 2020 2020 2020 7573 3d73              us=s
+00016ed0: 656c 662e 756e 6c6f 636b 5f61 6c6c 5f73  elf.unlock_all_s
+00016ee0: 6567 6d65 6e74 732c 0d0a 2020 2020 2020  egments,..      
+00016ef0: 2020 2020 2020 6c3d 7365 6c66 2e6c 6f63        l=self.loc
+00016f00: 6b2c 0d0a 2020 2020 2020 2020 2020 2020  k,..            
+00016f10: 7277 3d73 656c 662e 7265 6d6f 7665 5f77  rw=self.remove_w
+00016f20: 6f72 642c 0d0a 2020 2020 2020 2020 2020  ord,..          
+00016f30: 2020 7273 3d73 656c 662e 7265 6d6f 7665    rs=self.remove
+00016f40: 5f73 6567 6d65 6e74 2c0d 0a20 2020 2020  _segment,..     
+00016f50: 2020 2020 2020 2072 703d 7365 6c66 2e72         rp=self.r
+00016f60: 656d 6f76 655f 7265 7065 7469 7469 6f6e  emove_repetition
+00016f70: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00016f80: 7773 3d73 656c 662e 7265 6d6f 7665 5f77  ws=self.remove_w
+00016f90: 6f72 6473 5f62 795f 7374 722c 0d0a 2020  ords_by_str,..  
+00016fa0: 2020 2020 2020 2020 2020 6667 3d73 656c            fg=sel
+00016fb0: 662e 6669 6c6c 5f69 6e5f 6761 7073 2c0d  f.fill_in_gaps,.
+00016fc0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
+00016fd0: 2020 2020 6966 206e 6f74 2072 6567 726f      if not regro
+00016fe0: 7570 5f61 6c67 6f3a 0d0a 2020 2020 2020  up_algo:..      
+00016ff0: 2020 2020 2020 7265 7475 726e 205b 5d0d        return [].
+00017000: 0a0d 0a20 2020 2020 2020 2063 616c 6c73  ...        calls
+00017010: 203d 2072 6567 726f 7570 5f61 6c67 6f2e   = regroup_algo.
+00017020: 7370 6c69 7428 275f 2729 0d0a 2020 2020  split('_')..    
+00017030: 2020 2020 6966 2027 6461 2720 696e 2063      if 'da' in c
+00017040: 616c 6c73 3a0d 0a20 2020 2020 2020 2020  alls:..         
+00017050: 2020 2064 6566 6175 6c74 5f63 616c 6c73     default_calls
+00017060: 203d 2027 636d 5f73 703d 2c2a 202f efbc   = 'cm_sp=,* /..
+00017070: 8c5f 7367 3d2e 355f 6d67 3d2e 332b 335f  ._sg=.5_mg=.3+3_
+00017080: 7370 3d2e 2a20 2fe3 8082 2f3f 2fef bc9f  sp=.* /.../?/...
+00017090: 272e 7370 6c69 7428 275f 2729 0d0a 2020  '.split('_')..  
+000170a0: 2020 2020 2020 2020 2020 6361 6c6c 7320            calls 
+000170b0: 3d20 6368 6169 6e2e 6672 6f6d 5f69 7465  = chain.from_ite
+000170c0: 7261 626c 6528 6465 6661 756c 745f 6361  rable(default_ca
+000170d0: 6c6c 7320 6966 206d 6574 686f 6420 3d3d  lls if method ==
+000170e0: 2027 6461 2720 656c 7365 205b 6d65 7468   'da' else [meth
+000170f0: 6f64 5d20 666f 7220 6d65 7468 6f64 2069  od] for method i
+00017100: 6e20 6361 6c6c 7329 0d0a 2020 2020 2020  n calls)..      
+00017110: 2020 6f70 6572 6174 696f 6e73 203d 205b    operations = [
+00017120: 5d0d 0a20 2020 2020 2020 2066 6f72 206d  ]..        for m
+00017130: 6574 686f 6420 696e 2063 616c 6c73 3a0d  ethod in calls:.
+00017140: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+00017150: 686f 642c 2061 7267 7320 3d20 6d65 7468  hod, args = meth
+00017160: 6f64 2e73 706c 6974 2827 3d27 2c20 6d61  od.split('=', ma
+00017170: 7873 706c 6974 3d31 2920 6966 2027 3d27  xsplit=1) if '='
+00017180: 2069 6e20 6d65 7468 6f64 2065 6c73 6520   in method else 
+00017190: 286d 6574 686f 642c 2027 2729 0d0a 2020  (method, '')..  
+000171a0: 2020 2020 2020 2020 2020 6966 206d 6574            if met
+000171b0: 686f 6420 6e6f 7420 696e 206d 6574 686f  hod not in metho
+000171c0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+000171d0: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
+000171e0: 706c 656d 656e 7465 6445 7272 6f72 2866  plementedError(f
+000171f0: 277b 6d65 7468 6f64 7d20 6973 206e 6f74  '{method} is not
+00017200: 206f 6e65 206f 6620 7468 6520 6176 6169   one of the avai
+00017210: 6c61 626c 6520 6d65 7468 6f64 733a 207b  lable methods: {
+00017220: 7475 706c 6528 6d65 7468 6f64 732e 6b65  tuple(methods.ke
+00017230: 7973 2829 297d 2729 0d0a 2020 2020 2020  ys())}')..      
+00017240: 2020 2020 2020 6172 6773 203d 205b 5d20        args = [] 
+00017250: 6966 206c 656e 2861 7267 7329 203d 3d20  if len(args) == 
+00017260: 3020 656c 7365 206c 6973 7428 6d61 7028  0 else list(map(
+00017270: 7374 725f 746f 5f76 616c 6964 5f74 7970  str_to_valid_typ
+00017280: 652c 2061 7267 732e 7370 6c69 7428 272b  e, args.split('+
+00017290: 2729 2929 0d0a 2020 2020 2020 2020 2020  ')))..          
+000172a0: 2020 6b77 6172 6773 203d 207b 6b3a 2076    kwargs = {k: v
+000172b0: 2066 6f72 206b 2c20 7620 696e 207a 6970   for k, v in zip
+000172c0: 286d 6574 686f 6473 5b6d 6574 686f 645d  (methods[method]
+000172d0: 2e5f 5f63 6f64 655f 5f2e 636f 5f76 6172  .__code__.co_var
+000172e0: 6e61 6d65 735b 313a 5d2c 2061 7267 7329  names[1:], args)
+000172f0: 2069 6620 7620 6973 206e 6f74 204e 6f6e   if v is not Non
+00017300: 657d 0d0a 2020 2020 2020 2020 2020 2020  e}..            
+00017310: 6966 2069 6e63 6c75 6465 5f73 7472 3a0d  if include_str:.
+00017320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017330: 206b 7761 7267 735f 7374 7220 3d20 272c   kwargs_str = ',
+00017340: 2027 2e6a 6f69 6e28 6627 7b6b 7d3d 227b   '.join(f'{k}="{
+00017350: 767d 2227 2069 6620 6973 696e 7374 616e  v}"' if isinstan
+00017360: 6365 2876 2c20 7374 7229 2065 6c73 6520  ce(v, str) else 
+00017370: 6627 7b6b 7d3d 7b76 7d27 2066 6f72 206b  f'{k}={v}' for k
+00017380: 2c20 7620 696e 206b 7761 7267 732e 6974  , v in kwargs.it
+00017390: 656d 7328 2929 0d0a 2020 2020 2020 2020  ems())..        
+000173a0: 2020 2020 2020 2020 6f70 5f73 7472 203d          op_str =
+000173b0: 2066 277b 6d65 7468 6f64 735b 6d65 7468   f'{methods[meth
+000173c0: 6f64 5d2e 5f5f 6e61 6d65 5f5f 7d28 7b6b  od].__name__}({k
+000173d0: 7761 7267 735f 7374 727d 2927 0d0a 2020  wargs_str})'..  
+000173e0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+000173f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017400: 206f 705f 7374 7220 3d20 4e6f 6e65 0d0a   op_str = None..
+00017410: 2020 2020 2020 2020 2020 2020 6f70 6572              oper
+00017420: 6174 696f 6e73 2e61 7070 656e 6428 286d  ations.append((m
+00017430: 6574 686f 6473 5b6d 6574 686f 645d 2c20  ethods[method], 
+00017440: 6b77 6172 6773 2c20 6f70 5f73 7472 2929  kwargs, op_str))
+00017450: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+00017460: 726e 206f 7065 7261 7469 6f6e 730d 0a0d  rn operations...
+00017470: 0a20 2020 2064 6566 2066 696e 6428 7365  .    def find(se
+00017480: 6c66 2c20 7061 7474 6572 6e3a 2073 7472  lf, pattern: str
+00017490: 2c20 776f 7264 5f6c 6576 656c 3d54 7275  , word_level=Tru
+000174a0: 652c 2066 6c61 6773 3d4e 6f6e 6529 202d  e, flags=None) -
+000174b0: 3e20 2257 6869 7370 6572 5265 7375 6c74  > "WhisperResult
+000174c0: 4d61 7463 6865 7322 3a0d 0a20 2020 2020  Matches":..     
+000174d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000174e0: 4669 6e64 2073 6567 6d65 6e74 732f 776f  Find segments/wo
+000174f0: 7264 7320 616e 6420 7469 6d65 7374 616d  rds and timestam
+00017500: 7073 2077 6974 6820 7265 6775 6c61 7220  ps with regular 
+00017510: 6578 7072 6573 7369 6f6e 2e0d 0a0d 0a20  expression..... 
+00017520: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00017530: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+00017540: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2070  -----..        p
+00017550: 6174 7465 726e 203a 2073 7472 0d0a 2020  attern : str..  
+00017560: 2020 2020 2020 2020 2020 5265 6745 7820            RegEx 
+00017570: 7061 7474 6572 6e20 746f 2073 6561 7263  pattern to searc
+00017580: 6820 666f 722e 0d0a 2020 2020 2020 2020  h for...        
+00017590: 776f 7264 5f6c 6576 656c 203a 2062 6f6f  word_level : boo
+000175a0: 6c2c 2064 6566 6175 6c74 2054 7275 650d  l, default True.
+000175b0: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+000175c0: 7468 6572 2074 6f20 7365 6172 6368 2061  ther to search a
+000175d0: 7420 776f 7264 2d6c 6576 656c 2e0d 0a20  t word-level... 
+000175e0: 2020 2020 2020 2066 6c61 6773 203a 206f         flags : o
+000175f0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+00017600: 2020 2020 2052 6567 4578 2066 6c61 6773       RegEx flags
+00017610: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+00017620: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
+00017630: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
+00017640: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
+00017650: 7375 6c74 2e57 6869 7370 6572 5265 7375  sult.WhisperResu
+00017660: 6c74 4d61 7463 6865 730d 0a20 2020 2020  ltMatches..     
+00017670: 2020 2020 2020 2041 6e20 696e 7374 616e         An instan
+00017680: 6365 206f 6620 3a63 6c61 7373 3a60 7374  ce of :class:`st
+00017690: 6162 6c65 5f77 6869 7370 6572 2e72 6573  able_whisper.res
+000176a0: 756c 742e 5768 6973 7065 7252 6573 756c  ult.WhisperResul
+000176b0: 744d 6174 6368 6573 6020 7769 7468 2077  tMatches` with w
+000176c0: 6f72 642f 7365 676d 656e 7420 7468 6174  ord/segment that
+000176d0: 206d 6174 6368 2060 6070 6174 7465 726e   match ``pattern
+000176e0: 6060 2e0d 0a20 2020 2020 2020 2022 2222  ``...        """
+000176f0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00017700: 2057 6869 7370 6572 5265 7375 6c74 4d61   WhisperResultMa
+00017710: 7463 6865 7328 7365 6c66 292e 6669 6e64  tches(self).find
+00017720: 2870 6174 7465 726e 2c20 776f 7264 5f6c  (pattern, word_l
+00017730: 6576 656c 3d77 6f72 645f 6c65 7665 6c2c  evel=word_level,
+00017740: 2066 6c61 6773 3d66 6c61 6773 290d 0a0d   flags=flags)...
+00017750: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
+00017760: 2020 2020 6465 6620 7465 7874 2873 656c      def text(sel
+00017770: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
+00017780: 7572 6e20 2727 2e6a 6f69 6e28 732e 7465  urn ''.join(s.te
+00017790: 7874 2066 6f72 2073 2069 6e20 7365 6c66  xt for s in self
+000177a0: 2e73 6567 6d65 6e74 7329 0d0a 0d0a 2020  .segments)....  
+000177b0: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+000177c0: 2064 6566 2072 6567 726f 7570 5f68 6973   def regroup_his
+000177d0: 746f 7279 2873 656c 6629 3a0d 0a20 2020  tory(self):..   
+000177e0: 2020 2020 2023 2073 616d 6520 7379 6e74       # same synt
+000177f0: 6178 2061 7320 6060 7265 6772 6f75 705f  ax as ``regroup_
+00017800: 616c 676f 6060 2066 6f72 203a 6d65 7468  algo`` for :meth
+00017810: 3a60 6072 6573 756c 742e 5768 6973 7065  :``result.Whispe
+00017820: 7252 6573 756c 742e 7265 6772 6f75 7060  rResult.regroup`
+00017830: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00017840: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
+00017850: 6973 746f 7279 0d0a 0d0a 2020 2020 4070  istory....    @p
+00017860: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00017870: 206e 6f6e 7370 6565 6368 5f73 6563 7469   nonspeech_secti
+00017880: 6f6e 7328 7365 6c66 293a 0d0a 2020 2020  ons(self):..    
+00017890: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000178a0: 5f6e 6f6e 7370 6565 6368 5f73 6563 7469  _nonspeech_secti
+000178b0: 6f6e 730d 0a0d 0a20 2020 2064 6566 2073  ons....    def s
+000178c0: 686f 775f 7265 6772 6f75 705f 6869 7374  how_regroup_hist
+000178d0: 6f72 7928 7365 6c66 293a 0d0a 2020 2020  ory(self):..    
+000178e0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000178f0: 2050 7269 6e74 2064 6574 6169 6c73 206f   Print details o
+00017900: 6620 616c 6c20 7265 6772 6f75 7069 6e67  f all regrouping
+00017910: 206f 7065 7261 7469 6f6e 7320 7468 6174   operations that
+00017920: 2062 6565 6e20 7065 7266 6f72 6d65 6420   been performed 
+00017930: 6f6e 2064 6174 612e 0d0a 2020 2020 2020  on data...      
+00017940: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
+00017950: 6620 6e6f 7420 7365 6c66 2e5f 7265 6772  f not self._regr
+00017960: 6f75 705f 6869 7374 6f72 793a 0d0a 2020  oup_history:..  
+00017970: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00017980: 2752 6573 756c 7420 6861 7320 6e6f 2068  'Result has no h
+00017990: 6973 746f 7279 2e27 290d 0a20 2020 2020  istory.')..     
+000179a0: 2020 2066 6f72 202a 5f2c 206d 7367 2069     for *_, msg i
+000179b0: 6e20 7365 6c66 2e70 6172 7365 5f72 6567  n self.parse_reg
+000179c0: 726f 7570 5f61 6c67 6f28 7365 6c66 2e5f  roup_algo(self._
+000179d0: 7265 6772 6f75 705f 6869 7374 6f72 7929  regroup_history)
+000179e0: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+000179f0: 7269 6e74 2866 272e 7b6d 7367 7d27 290d  rint(f'.{msg}').
+00017a00: 0a0d 0a20 2020 2064 6566 205f 5f6c 656e  ...    def __len
+00017a10: 5f5f 2873 656c 6629 3a0d 0a20 2020 2020  __(self):..     
+00017a20: 2020 2072 6574 7572 6e20 6c65 6e28 7365     return len(se
+00017a30: 6c66 2e73 6567 6d65 6e74 7329 0d0a 0d0a  lf.segments)....
+00017a40: 2020 2020 6465 6620 756e 6c6f 636b 5f61      def unlock_a
+00017a50: 6c6c 5f73 6567 6d65 6e74 7328 7365 6c66  ll_segments(self
+00017a60: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
+00017a70: 7320 696e 2073 656c 662e 7365 676d 656e  s in self.segmen
+00017a80: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00017a90: 2073 2e75 6e6c 6f63 6b5f 616c 6c5f 776f   s.unlock_all_wo
+00017aa0: 7264 7328 290d 0a20 2020 2020 2020 2072  rds()..        r
+00017ab0: 6574 7572 6e20 7365 6c66 0d0a 0d0a 2020  eturn self....  
+00017ac0: 2020 6465 6620 7265 7365 7428 7365 6c66    def reset(self
+00017ad0: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+00017ae0: 0a20 2020 2020 2020 2052 6573 746f 7265  .        Restore
+00017af0: 2061 6c6c 2076 616c 7565 7320 746f 2074   all values to t
+00017b00: 6861 7420 6174 2069 6e69 7469 616c 697a  hat at initializ
+00017b10: 6174 696f 6e2e 0d0a 2020 2020 2020 2020  ation...        
+00017b20: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
+00017b30: 662e 6c61 6e67 7561 6765 203d 2073 656c  f.language = sel
+00017b40: 662e 6f72 695f 6469 6374 2e67 6574 2827  f.ori_dict.get('
+00017b50: 6c61 6e67 7561 6765 2729 0d0a 2020 2020  language')..    
+00017b60: 2020 2020 7365 6c66 2e5f 7265 6772 6f75      self._regrou
+00017b70: 705f 6869 7374 6f72 7920 3d20 2727 0d0a  p_history = ''..
+00017b80: 2020 2020 2020 2020 7365 676d 656e 7473          segments
+00017b90: 203d 2073 656c 662e 6f72 695f 6469 6374   = self.ori_dict
+00017ba0: 2e67 6574 2827 7365 676d 656e 7473 2729  .get('segments')
+00017bb0: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00017bc0: 6567 6d65 6e74 7320 3d20 5b53 6567 6d65  egments = [Segme
+00017bd0: 6e74 282a 2a73 2c20 6967 6e6f 7265 5f75  nt(**s, ignore_u
+00017be0: 6e75 7365 645f 6172 6773 3d54 7275 6529  nused_args=True)
+00017bf0: 2066 6f72 2073 2069 6e20 7365 676d 656e   for s in segmen
+00017c00: 7473 5d20 6966 2073 6567 6d65 6e74 7320  ts] if segments 
+00017c10: 656c 7365 205b 5d0d 0a20 2020 2020 2020  else []..       
+00017c20: 2069 6620 7365 6c66 2e5f 666f 7263 6564   if self._forced
+00017c30: 5f6f 7264 6572 3a0d 0a20 2020 2020 2020  _order:..       
+00017c40: 2020 2020 2073 656c 662e 666f 7263 655f       self.force_
+00017c50: 6f72 6465 7228 290d 0a20 2020 2020 2020  order()..       
+00017c60: 2073 656c 662e 7265 6d6f 7665 5f6e 6f5f   self.remove_no_
+00017c70: 776f 7264 5f73 6567 6d65 6e74 7328 616e  word_segments(an
+00017c80: 7928 7365 672e 6861 735f 776f 7264 7320  y(seg.has_words 
+00017c90: 666f 7220 7365 6720 696e 2073 656c 662e  for seg in self.
+00017ca0: 7365 676d 656e 7473 2929 0d0a 0d0a 2020  segments))....  
+00017cb0: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00017cc0: 2064 6566 2068 6173 5f77 6f72 6473 2873   def has_words(s
+00017cd0: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
+00017ce0: 6574 7572 6e20 626f 6f6c 2873 656c 662e  eturn bool(self.
+00017cf0: 7365 676d 656e 7473 2920 616e 6420 616c  segments) and al
+00017d00: 6c28 7365 672e 6861 735f 776f 7264 7320  l(seg.has_words 
+00017d10: 666f 7220 7365 6720 696e 2073 656c 662e  for seg in self.
+00017d20: 7365 676d 656e 7473 290d 0a0d 0a20 2020  segments)....   
+00017d30: 2074 6f5f 7372 745f 7674 7420 3d20 7265   to_srt_vtt = re
+00017d40: 7375 6c74 5f74 6f5f 7372 745f 7674 740d  sult_to_srt_vtt.
+00017d50: 0a20 2020 2074 6f5f 6173 7320 3d20 7265  .    to_ass = re
+00017d60: 7375 6c74 5f74 6f5f 6173 730d 0a20 2020  sult_to_ass..   
+00017d70: 2074 6f5f 7473 7620 3d20 7265 7375 6c74   to_tsv = result
+00017d80: 5f74 6f5f 7473 760d 0a20 2020 2074 6f5f  _to_tsv..    to_
+00017d90: 7478 7420 3d20 7265 7375 6c74 5f74 6f5f  txt = result_to_
+00017da0: 7478 740d 0a20 2020 2073 6176 655f 6173  txt..    save_as
+00017db0: 5f6a 736f 6e20 3d20 7361 7665 5f61 735f  _json = save_as_
+00017dc0: 6a73 6f6e 0d0a 0d0a 0d0a 636c 6173 7320  json......class 
+00017dd0: 5365 676d 656e 744d 6174 6368 3a0d 0a0d  SegmentMatch:...
+00017de0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00017df0: 5f28 0d0a 2020 2020 2020 2020 2020 2020  _(..            
+00017e00: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+00017e10: 2020 2073 6567 6d65 6e74 733a 2055 6e69     segments: Uni
+00017e20: 6f6e 5b4c 6973 745b 5365 676d 656e 745d  on[List[Segment]
+00017e30: 2c20 5365 676d 656e 745d 2c0d 0a20 2020  , Segment],..   
+00017e40: 2020 2020 2020 2020 205f 776f 7264 5f69           _word_i
+00017e50: 6e64 6963 6573 3a20 4c69 7374 5b4c 6973  ndices: List[Lis
+00017e60: 745b 696e 745d 5d20 3d20 4e6f 6e65 2c0d  t[int]] = None,.
+00017e70: 0a20 2020 2020 2020 2020 2020 205f 7465  .            _te
+00017e80: 7874 5f6d 6174 6368 3a20 7374 7220 3d20  xt_match: str = 
+00017e90: 4e6f 6e65 0d0a 2020 2020 293a 0d0a 2020  None..    ):..  
+00017ea0: 2020 2020 2020 7365 6c66 2e73 6567 6d65        self.segme
+00017eb0: 6e74 7320 3d20 5b73 6567 6d65 6e74 735d  nts = [segments]
+00017ec0: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
+00017ed0: 6567 6d65 6e74 732c 2053 6567 6d65 6e74  egments, Segment
+00017ee0: 2920 656c 7365 2073 6567 6d65 6e74 730d  ) else segments.
+00017ef0: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
+00017f00: 7264 5f69 6e64 6963 6573 203d 205b 5d20  rd_indices = [] 
+00017f10: 6966 205f 776f 7264 5f69 6e64 6963 6573  if _word_indices
+00017f20: 2069 7320 4e6f 6e65 2065 6c73 6520 5f77   is None else _w
+00017f30: 6f72 645f 696e 6469 6365 730d 0a20 2020  ord_indices..   
+00017f40: 2020 2020 2073 656c 662e 776f 7264 7320       self.words 
+00017f50: 3d20 5b73 656c 662e 7365 676d 656e 7473  = [self.segments
+00017f60: 5b69 5d2e 776f 7264 735b 6a5d 2066 6f72  [i].words[j] for
+00017f70: 2069 2c20 696e 6469 6365 7320 696e 2065   i, indices in e
+00017f80: 6e75 6d65 7261 7465 2873 656c 662e 776f  numerate(self.wo
+00017f90: 7264 5f69 6e64 6963 6573 2920 666f 7220  rd_indices) for 
+00017fa0: 6a20 696e 2069 6e64 6963 6573 5d0d 0a20  j in indices].. 
+00017fb0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
+00017fc0: 6c66 2e77 6f72 6473 2920 213d 2030 3a0d  lf.words) != 0:.
+00017fd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00017fe0: 662e 7465 7874 203d 2027 272e 6a6f 696e  f.text = ''.join
+00017ff0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00018000: 2020 2073 656c 662e 7365 676d 656e 7473     self.segments
+00018010: 5b69 5d2e 776f 7264 735b 6a5d 2e77 6f72  [i].words[j].wor
+00018020: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
+00018030: 2020 2066 6f72 2069 2c20 696e 6469 6365     for i, indice
+00018040: 7320 696e 2065 6e75 6d65 7261 7465 2873  s in enumerate(s
+00018050: 656c 662e 776f 7264 5f69 6e64 6963 6573  elf.word_indices
+00018060: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018070: 2020 2066 6f72 206a 2069 6e20 696e 6469     for j in indi
+00018080: 6365 730d 0a20 2020 2020 2020 2020 2020  ces..           
+00018090: 2029 0d0a 2020 2020 2020 2020 656c 7365   )..        else
+000180a0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000180b0: 656c 662e 7465 7874 203d 2027 272e 6a6f  elf.text = ''.jo
+000180c0: 696e 2873 6567 2e74 6578 7420 666f 7220  in(seg.text for 
+000180d0: 7365 6720 696e 2073 656c 662e 7365 676d  seg in self.segm
+000180e0: 656e 7473 290d 0a20 2020 2020 2020 2073  ents)..        s
+000180f0: 656c 662e 7465 7874 5f6d 6174 6368 203d  elf.text_match =
+00018100: 205f 7465 7874 5f6d 6174 6368 0d0a 0d0a   _text_match....
+00018110: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+00018120: 2020 2064 6566 2073 7461 7274 2873 656c     def start(sel
+00018130: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
+00018140: 7572 6e20 280d 0a20 2020 2020 2020 2020  urn (..         
+00018150: 2020 2073 656c 662e 776f 7264 735b 305d     self.words[0]
+00018160: 2e73 7461 7274 0d0a 2020 2020 2020 2020  .start..        
+00018170: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
+00018180: 776f 7264 7329 2021 3d20 3020 656c 7365  words) != 0 else
+00018190: 0d0a 2020 2020 2020 2020 2020 2020 2873  ..            (s
+000181a0: 656c 662e 7365 676d 656e 7473 5b30 5d2e  elf.segments[0].
+000181b0: 7374 6172 7420 6966 206c 656e 2873 656c  start if len(sel
+000181c0: 662e 7365 676d 656e 7473 2920 213d 2030  f.segments) != 0
+000181d0: 2065 6c73 6520 4e6f 6e65 290d 0a20 2020   else None)..   
+000181e0: 2020 2020 2029 0d0a 0d0a 2020 2020 4070       )....    @p
+000181f0: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00018200: 2065 6e64 2873 656c 6629 3a0d 0a20 2020   end(self):..   
+00018210: 2020 2020 2072 6574 7572 6e20 280d 0a20       return (.. 
+00018220: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018230: 776f 7264 735b 2d31 5d2e 656e 640d 0a20  words[-1].end.. 
+00018240: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00018250: 6e28 7365 6c66 2e77 6f72 6473 2920 213d  n(self.words) !=
+00018260: 2030 2065 6c73 650d 0a20 2020 2020 2020   0 else..       
+00018270: 2020 2020 2028 7365 6c66 2e73 6567 6d65       (self.segme
+00018280: 6e74 735b 2d31 5d2e 656e 6420 6966 206c  nts[-1].end if l
+00018290: 656e 2873 656c 662e 7365 676d 656e 7473  en(self.segments
+000182a0: 2920 213d 2030 2065 6c73 6520 4e6f 6e65  ) != 0 else None
+000182b0: 290d 0a20 2020 2020 2020 2029 0d0a 0d0a  )..        )....
+000182c0: 2020 2020 6465 6620 5f5f 6c65 6e5f 5f28      def __len__(
+000182d0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000182e0: 7265 7475 726e 206c 656e 2873 656c 662e  return len(self.
+000182f0: 7365 676d 656e 7473 290d 0a0d 0a20 2020  segments)....   
+00018300: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
+00018310: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
+00018320: 7475 726e 2073 656c 662e 5f5f 6469 6374  turn self.__dict
+00018330: 5f5f 2e5f 5f72 6570 725f 5f28 290d 0a0d  __.__repr__()...
+00018340: 0a20 2020 2064 6566 205f 5f73 7472 5f5f  .    def __str__
+00018350: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00018360: 2072 6574 7572 6e20 7365 6c66 2e5f 5f64   return self.__d
+00018370: 6963 745f 5f2e 5f5f 7374 725f 5f28 290d  ict__.__str__().
+00018380: 0a0d 0a0d 0a63 6c61 7373 2057 6869 7370  .....class Whisp
+00018390: 6572 5265 7375 6c74 4d61 7463 6865 733a  erResultMatches:
+000183a0: 0d0a 2020 2020 2222 220d 0a20 2020 2052  ..    """..    R
+000183b0: 6567 4578 206d 6174 6368 6573 2066 6f72  egEx matches for
+000183c0: 2057 6869 7370 6572 5265 7375 6c74 732e   WhisperResults.
+000183d0: 0d0a 2020 2020 2222 220d 0a20 2020 2023  ..    """..    #
+000183e0: 2055 7365 2057 6869 7370 6572 5265 7375   Use WhisperResu
+000183f0: 6c74 2e66 696e 6428 2920 696e 7374 6561  lt.find() instea
+00018400: 6420 6f66 2069 6e73 7461 6e74 6961 7469  d of instantiati
+00018410: 6e67 2074 6869 7320 636c 6173 7320 6469  ng this class di
+00018420: 7265 6374 6c79 2e0d 0a20 2020 2064 6566  rectly...    def
+00018430: 205f 5f69 6e69 745f 5f28 0d0a 2020 2020   __init__(..    
+00018440: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
+00018450: 2020 2020 2020 2020 2020 206d 6174 6368             match
+00018460: 6573 3a20 556e 696f 6e5b 4c69 7374 5b53  es: Union[List[S
+00018470: 6567 6d65 6e74 4d61 7463 685d 2c20 5768  egmentMatch], Wh
+00018480: 6973 7065 7252 6573 756c 745d 2c0d 0a20  isperResult],.. 
+00018490: 2020 2020 2020 2020 2020 205f 7365 676d             _segm
+000184a0: 656e 745f 696e 6469 6365 733a 204c 6973  ent_indices: Lis
+000184b0: 745b 4c69 7374 5b69 6e74 5d5d 203d 204e  t[List[int]] = N
+000184c0: 6f6e 650d 0a20 2020 2029 3a0d 0a20 2020  one..    ):..   
+000184d0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+000184e0: 6365 286d 6174 6368 6573 2c20 5768 6973  ce(matches, Whis
+000184f0: 7065 7252 6573 756c 7429 3a0d 0a20 2020  perResult):..   
+00018500: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+00018510: 7463 6865 7320 3d20 6c69 7374 286d 6170  tches = list(map
+00018520: 2853 6567 6d65 6e74 4d61 7463 682c 206d  (SegmentMatch, m
+00018530: 6174 6368 6573 2e73 6567 6d65 6e74 7329  atches.segments)
+00018540: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00018550: 656c 662e 5f73 6567 6d65 6e74 5f69 6e64  elf._segment_ind
+00018560: 6963 6573 203d 205b 5b69 5d20 666f 7220  ices = [[i] for 
+00018570: 6920 696e 2072 616e 6765 286c 656e 286d  i in range(len(m
+00018580: 6174 6368 6573 2e73 6567 6d65 6e74 7329  atches.segments)
+00018590: 295d 0d0a 2020 2020 2020 2020 656c 7365  )]..        else
+000185a0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000185b0: 656c 662e 6d61 7463 6865 7320 3d20 6d61  elf.matches = ma
+000185c0: 7463 6865 730d 0a20 2020 2020 2020 2020  tches..         
+000185d0: 2020 2061 7373 6572 7420 5f73 6567 6d65     assert _segme
+000185e0: 6e74 5f69 6e64 6963 6573 2069 7320 6e6f  nt_indices is no
+000185f0: 7420 4e6f 6e65 0d0a 2020 2020 2020 2020  t None..        
+00018600: 2020 2020 6173 7365 7274 206c 656e 2873      assert len(s
+00018610: 656c 662e 6d61 7463 6865 7329 203d 3d20  elf.matches) == 
+00018620: 6c65 6e28 5f73 6567 6d65 6e74 5f69 6e64  len(_segment_ind
+00018630: 6963 6573 290d 0a20 2020 2020 2020 2020  ices)..         
+00018640: 2020 2061 7373 6572 7420 616c 6c28 6c65     assert all(le
+00018650: 6e28 6d61 7463 682e 7365 676d 656e 7473  n(match.segments
+00018660: 2920 3d3d 206c 656e 285f 7365 676d 656e  ) == len(_segmen
+00018670: 745f 696e 6469 6365 735b 695d 2920 666f  t_indices[i]) fo
+00018680: 7220 692c 206d 6174 6368 2069 6e20 656e  r i, match in en
+00018690: 756d 6572 6174 6528 7365 6c66 2e6d 6174  umerate(self.mat
+000186a0: 6368 6573 2929 0d0a 2020 2020 2020 2020  ches))..        
+000186b0: 2020 2020 7365 6c66 2e5f 7365 676d 656e      self._segmen
+000186c0: 745f 696e 6469 6365 7320 3d20 5f73 6567  t_indices = _seg
+000186d0: 6d65 6e74 5f69 6e64 6963 6573 0d0a 0d0a  ment_indices....
+000186e0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+000186f0: 2020 2064 6566 2073 6567 6d65 6e74 5f69     def segment_i
+00018700: 6e64 6963 6573 2873 656c 6629 3a0d 0a20  ndices(self):.. 
+00018710: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00018720: 6c66 2e5f 7365 676d 656e 745f 696e 6469  lf._segment_indi
+00018730: 6365 730d 0a0d 0a20 2020 2064 6566 205f  ces....    def _
+00018740: 6375 7272 5f73 6567 5f67 726f 7570 7328  curr_seg_groups(
+00018750: 7365 6c66 2920 2d3e 204c 6973 745b 4c69  self) -> List[Li
+00018760: 7374 5b54 7570 6c65 5b69 6e74 2c20 5365  st[Tuple[int, Se
+00018770: 676d 656e 745d 5d5d 3a0d 0a20 2020 2020  gment]]]:..     
+00018780: 2020 2073 6567 5f67 726f 7570 732c 2063     seg_groups, c
+00018790: 7572 725f 7365 6773 203d 205b 5d2c 205b  urr_segs = [], [
+000187a0: 5d0d 0a20 2020 2020 2020 2063 7572 725f  ]..        curr_
+000187b0: 6d61 7820 3d20 2d31 0d0a 2020 2020 2020  max = -1..      
+000187c0: 2020 666f 7220 7365 675f 696e 6469 6365    for seg_indice
+000187d0: 732c 206d 6174 6368 2069 6e20 7a69 7028  s, match in zip(
+000187e0: 7365 6c66 2e5f 7365 676d 656e 745f 696e  self._segment_in
+000187f0: 6469 6365 732c 2073 656c 662e 6d61 7463  dices, self.matc
+00018800: 6865 7329 3a0d 0a20 2020 2020 2020 2020  hes):..         
+00018810: 2020 2066 6f72 2069 2c20 7365 6720 696e     for i, seg in
+00018820: 207a 6970 2873 6f72 7465 6428 7365 675f   zip(sorted(seg_
+00018830: 696e 6469 6365 7329 2c20 6d61 7463 682e  indices), match.
+00018840: 7365 676d 656e 7473 293a 0d0a 2020 2020  segments):..    
+00018850: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00018860: 203e 2063 7572 725f 6d61 783a 0d0a 2020   > curr_max:..  
+00018870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018880: 2020 6375 7272 5f73 6567 732e 6170 7065    curr_segs.appe
+00018890: 6e64 2828 692c 2073 6567 2929 0d0a 2020  nd((i, seg))..  
+000188a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188b0: 2020 6966 2069 202d 2031 2021 3d20 6375    if i - 1 != cu
+000188c0: 7272 5f6d 6178 3a0d 0a20 2020 2020 2020  rr_max:..       
+000188d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188e0: 2073 6567 5f67 726f 7570 732e 6170 7065   seg_groups.appe
+000188f0: 6e64 2863 7572 725f 7365 6773 290d 0a20  nd(curr_segs).. 
+00018900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018910: 2020 2020 2020 2063 7572 725f 7365 6773         curr_segs
+00018920: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00018930: 2020 2020 2020 2020 2020 2063 7572 725f             curr_
+00018940: 6d61 7820 3d20 690d 0a0d 0a20 2020 2020  max = i....     
+00018950: 2020 2069 6620 6375 7272 5f73 6567 733a     if curr_segs:
+00018960: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00018970: 675f 6772 6f75 7073 2e61 7070 656e 6428  g_groups.append(
+00018980: 6375 7272 5f73 6567 7329 0d0a 2020 2020  curr_segs)..    
+00018990: 2020 2020 7265 7475 726e 2073 6567 5f67      return seg_g
+000189a0: 726f 7570 730d 0a0d 0a20 2020 2064 6566  roups....    def
+000189b0: 2066 696e 6428 7365 6c66 2c20 7061 7474   find(self, patt
+000189c0: 6572 6e3a 2073 7472 2c20 776f 7264 5f6c  ern: str, word_l
+000189d0: 6576 656c 3d54 7275 652c 2066 6c61 6773  evel=True, flags
+000189e0: 3d4e 6f6e 6529 202d 3e20 2257 6869 7370  =None) -> "Whisp
+000189f0: 6572 5265 7375 6c74 4d61 7463 6865 7322  erResultMatches"
+00018a00: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00018a10: 2020 2020 2020 2020 4669 6e64 2073 6567          Find seg
+00018a20: 6d65 6e74 732f 776f 7264 7320 616e 6420  ments/words and 
+00018a30: 7469 6d65 7374 616d 7073 2077 6974 6820  timestamps with 
+00018a40: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
+00018a50: 6f6e 2e0d 0a0d 0a20 2020 2020 2020 2050  on.....        P
+00018a60: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
+00018a70: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+00018a80: 2020 2020 2020 2070 6174 7465 726e 203a         pattern :
+00018a90: 2073 7472 0d0a 2020 2020 2020 2020 2020   str..          
+00018aa0: 2020 5265 6745 7820 7061 7474 6572 6e20    RegEx pattern 
+00018ab0: 746f 2073 6561 7263 6820 666f 722e 0d0a  to search for...
+00018ac0: 2020 2020 2020 2020 776f 7264 5f6c 6576          word_lev
+00018ad0: 656c 203a 2062 6f6f 6c2c 2064 6566 6175  el : bool, defau
+00018ae0: 6c74 2054 7275 650d 0a20 2020 2020 2020  lt True..       
+00018af0: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
+00018b00: 7365 6172 6368 2061 7420 776f 7264 2d6c  search at word-l
+00018b10: 6576 656c 2e0d 0a20 2020 2020 2020 2066  evel...        f
+00018b20: 6c61 6773 203a 206f 7074 696f 6e61 6c0d  lags : optional.
+00018b30: 0a20 2020 2020 2020 2020 2020 2052 6567  .            Reg
+00018b40: 4578 2066 6c61 6773 2e0d 0a0d 0a20 2020  Ex flags.....   
+00018b50: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
+00018b60: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
+00018b70: 2020 2020 2020 2073 7461 626c 655f 7768         stable_wh
+00018b80: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
+00018b90: 7370 6572 5265 7375 6c74 4d61 7463 6865  sperResultMatche
+00018ba0: 730d 0a20 2020 2020 2020 2020 2020 2041  s..            A
+00018bb0: 6e20 696e 7374 616e 6365 206f 6620 3a63  n instance of :c
+00018bc0: 6c61 7373 3a60 7374 6162 6c65 5f77 6869  lass:`stable_whi
+00018bd0: 7370 6572 2e72 6573 756c 742e 5768 6973  sper.result.Whis
+00018be0: 7065 7252 6573 756c 744d 6174 6368 6573  perResultMatches
+00018bf0: 6020 7769 7468 2077 6f72 642f 7365 676d  ` with word/segm
+00018c00: 656e 7420 7468 6174 206d 6174 6368 2060  ent that match `
+00018c10: 6070 6174 7465 726e 6060 2e0d 0a20 2020  `pattern``...   
+00018c20: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
+00018c30: 2020 2020 7365 675f 6772 6f75 7073 203d      seg_groups =
+00018c40: 2073 656c 662e 5f63 7572 725f 7365 675f   self._curr_seg_
+00018c50: 6772 6f75 7073 2829 0d0a 2020 2020 2020  groups()..      
+00018c60: 2020 6d61 7463 6865 733a 204c 6973 745b    matches: List[
+00018c70: 5365 676d 656e 744d 6174 6368 5d20 3d20  SegmentMatch] = 
+00018c80: 5b5d 0d0a 2020 2020 2020 2020 6d61 7463  []..        matc
+00018c90: 685f 7365 675f 696e 6469 6365 733a 204c  h_seg_indices: L
+00018ca0: 6973 745b 4c69 7374 5b69 6e74 5d5d 203d  ist[List[int]] =
+00018cb0: 205b 5d0d 0a20 2020 2020 2020 2069 6620   []..        if 
+00018cc0: 776f 7264 5f6c 6576 656c 3a0d 0a20 2020  word_level:..   
+00018cd0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00018ce0: 616c 6c28 616c 6c28 7365 672e 6861 735f  all(all(seg.has_
+00018cf0: 776f 7264 7320 666f 7220 7365 6720 696e  words for seg in
+00018d00: 206d 6174 6368 2e73 6567 6d65 6e74 7329   match.segments)
+00018d10: 2066 6f72 206d 6174 6368 2069 6e20 7365   for match in se
+00018d20: 6c66 2e6d 6174 6368 6573 293a 0d0a 2020  lf.matches):..  
+00018d30: 2020 2020 2020 2020 2020 2020 2020 7761                wa
+00018d40: 726e 696e 6773 2e77 6172 6e28 2743 616e  rnings.warn('Can
+00018d50: 6e6f 7420 7065 7266 6f72 6d20 776f 7264  not perform word
+00018d60: 2d6c 6576 656c 2073 6561 7263 6820 7769  -level search wi
+00018d70: 7468 2073 6567 6d65 6e74 2873 2920 6d69  th segment(s) mi
+00018d80: 7373 696e 6720 776f 7264 2074 696d 6573  ssing word times
+00018d90: 7461 6d70 732e 2729 0d0a 2020 2020 2020  tamps.')..      
+00018da0: 2020 2020 2020 2020 2020 776f 7264 5f6c            word_l
+00018db0: 6576 656c 203d 2046 616c 7365 0d0a 0d0a  evel = False....
+00018dc0: 2020 2020 2020 2020 666f 7220 7365 6773          for segs
+00018dd0: 2069 6e20 7365 675f 6772 6f75 7073 3a0d   in seg_groups:.
+00018de0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00018df0: 776f 7264 5f6c 6576 656c 3a0d 0a20 2020  word_level:..   
+00018e00: 2020 2020 2020 2020 2020 2020 2069 6478               idx
+00018e10: 7320 3d20 6c69 7374 2863 6861 696e 2e66  s = list(chain.f
+00018e20: 726f 6d5f 6974 6572 6162 6c65 280d 0a20  rom_iterable(.. 
+00018e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e40: 2020 205b 2869 2c20 6a29 5d2a 6c65 6e28     [(i, j)]*len(
+00018e50: 776f 7264 2e77 6f72 6429 2066 6f72 2028  word.word) for (
+00018e60: 692c 2073 6567 2920 696e 2073 6567 7320  i, seg) in segs 
+00018e70: 666f 7220 6a2c 2077 6f72 6420 696e 2065  for j, word in e
+00018e80: 6e75 6d65 7261 7465 2873 6567 2e77 6f72  numerate(seg.wor
+00018e90: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
+00018ea0: 2020 2020 2029 290d 0a20 2020 2020 2020       ))..       
+00018eb0: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
+00018ec0: 2727 2e6a 6f69 6e28 776f 7264 2e77 6f72  ''.join(word.wor
+00018ed0: 6420 666f 7220 285f 2c20 7365 6729 2069  d for (_, seg) i
+00018ee0: 6e20 7365 6773 2066 6f72 2077 6f72 6420  n segs for word 
+00018ef0: 696e 2073 6567 2e77 6f72 6473 290d 0a20  in seg.words).. 
+00018f00: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00018f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018f20: 2020 6964 7873 203d 206c 6973 7428 6368    idxs = list(ch
+00018f30: 6169 6e2e 6672 6f6d 5f69 7465 7261 626c  ain.from_iterabl
+00018f40: 6528 5b28 692c 204e 6f6e 6529 5d2a 6c65  e([(i, None)]*le
+00018f50: 6e28 7365 672e 7465 7874 2920 666f 7220  n(seg.text) for 
+00018f60: 2869 2c20 7365 6729 2069 6e20 7365 6773  (i, seg) in segs
+00018f70: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018f80: 2020 2020 7465 7874 203d 2027 272e 6a6f      text = ''.jo
+00018f90: 696e 2873 6567 2e74 6578 7420 666f 7220  in(seg.text for 
+00018fa0: 285f 2c20 7365 6729 2069 6e20 7365 6773  (_, seg) in segs
+00018fb0: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
+00018fc0: 7373 6572 7420 6c65 6e28 6964 7873 2920  ssert len(idxs) 
+00018fd0: 3d3d 206c 656e 2874 6578 7429 0d0a 2020  == len(text)..  
+00018fe0: 2020 2020 2020 2020 2020 666f 7220 6375            for cu
+00018ff0: 7272 5f6d 6174 6368 2069 6e20 7265 2e66  rr_match in re.f
+00019000: 696e 6469 7465 7228 7061 7474 6572 6e2c  inditer(pattern,
+00019010: 2074 6578 742c 2066 6c61 6773 3d66 6c61   text, flags=fla
+00019020: 6773 206f 7220 3029 3a0d 0a20 2020 2020  gs or 0):..     
+00019030: 2020 2020 2020 2020 2020 2073 7461 7274             start
+00019040: 2c20 656e 6420 3d20 6375 7272 5f6d 6174  , end = curr_mat
+00019050: 6368 2e73 7061 6e28 290d 0a20 2020 2020  ch.span()..     
+00019060: 2020 2020 2020 2020 2020 2063 7572 725f             curr_
+00019070: 6964 7873 203d 2069 6478 735b 7374 6172  idxs = idxs[star
+00019080: 743a 2065 6e64 5d0d 0a20 2020 2020 2020  t: end]..       
+00019090: 2020 2020 2020 2020 2063 7572 725f 7365           curr_se
+000190a0: 675f 6964 7873 203d 2073 6f72 7465 6428  g_idxs = sorted(
+000190b0: 7365 7428 695b 305d 2066 6f72 2069 2069  set(i[0] for i i
+000190c0: 6e20 6375 7272 5f69 6478 7329 290d 0a20  n curr_idxs)).. 
+000190d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000190e0: 6620 776f 7264 5f6c 6576 656c 3a0d 0a20  f word_level:.. 
+000190f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019100: 2020 2063 7572 725f 776f 7264 5f69 6478     curr_word_idx
+00019110: 7320 3d20 5b0d 0a20 2020 2020 2020 2020  s = [..         
+00019120: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019130: 6f72 7465 6428 7365 7428 6a20 666f 7220  orted(set(j for 
+00019140: 692c 206a 2069 6e20 6375 7272 5f69 6478  i, j in curr_idx
+00019150: 7320 6966 2069 203d 3d20 7365 675f 6964  s if i == seg_id
+00019160: 7829 290d 0a20 2020 2020 2020 2020 2020  x))..           
+00019170: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00019180: 2073 6567 5f69 6478 2069 6e20 6375 7272   seg_idx in curr
+00019190: 5f73 6567 5f69 6478 730d 0a20 2020 2020  _seg_idxs..     
+000191a0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+000191b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000191c0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+000191d0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+000191e0: 725f 776f 7264 5f69 6478 7320 3d20 4e6f  r_word_idxs = No
+000191f0: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
+00019200: 2020 2020 6d61 7463 6865 732e 6170 7065      matches.appe
+00019210: 6e64 2853 6567 6d65 6e74 4d61 7463 6828  nd(SegmentMatch(
+00019220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019230: 2020 2020 2020 7365 676d 656e 7473 3d5b        segments=[
+00019240: 7320 666f 7220 692c 2073 2069 6e20 7365  s for i, s in se
+00019250: 6773 2069 6620 6920 696e 2063 7572 725f  gs if i in curr_
+00019260: 7365 675f 6964 7873 5d2c 0d0a 2020 2020  seg_idxs],..    
+00019270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019280: 5f77 6f72 645f 696e 6469 6365 733d 6375  _word_indices=cu
+00019290: 7272 5f77 6f72 645f 6964 7873 2c0d 0a20  rr_word_idxs,.. 
+000192a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192b0: 2020 205f 7465 7874 5f6d 6174 6368 3d63     _text_match=c
+000192c0: 7572 725f 6d61 7463 682e 6772 6f75 7028  urr_match.group(
+000192d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000192e0: 2020 2029 290d 0a20 2020 2020 2020 2020     ))..         
+000192f0: 2020 2020 2020 206d 6174 6368 5f73 6567         match_seg
+00019300: 5f69 6e64 6963 6573 2e61 7070 656e 6428  _indices.append(
+00019310: 6375 7272 5f73 6567 5f69 6478 7329 0d0a  curr_seg_idxs)..
+00019320: 2020 2020 2020 2020 7265 7475 726e 2057          return W
+00019330: 6869 7370 6572 5265 7375 6c74 4d61 7463  hisperResultMatc
+00019340: 6865 7328 6d61 7463 6865 732c 206d 6174  hes(matches, mat
+00019350: 6368 5f73 6567 5f69 6e64 6963 6573 290d  ch_seg_indices).
+00019360: 0a0d 0a20 2020 2064 6566 205f 5f6c 656e  ...    def __len
+00019370: 5f5f 2873 656c 6629 3a0d 0a20 2020 2020  __(self):..     
+00019380: 2020 2072 6574 7572 6e20 6c65 6e28 7365     return len(se
+00019390: 6c66 2e6d 6174 6368 6573 290d 0a0d 0a20  lf.matches).... 
+000193a0: 2020 2064 6566 205f 5f62 6f6f 6c5f 5f28     def __bool__(
+000193b0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000193c0: 7265 7475 726e 2073 656c 662e 5f5f 6c65  return self.__le
+000193d0: 6e5f 5f28 2920 213d 2030 0d0a 0d0a 2020  n__() != 0....  
+000193e0: 2020 6465 6620 5f5f 6765 7469 7465 6d5f    def __getitem_
+000193f0: 5f28 7365 6c66 2c20 6964 7829 3a0d 0a20  _(self, idx):.. 
+00019400: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00019410: 6c66 2e6d 6174 6368 6573 5b69 6478 5d0d  lf.matches[idx].
+00019420: 0a                                       .
```

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/stabilization/__init__.py` & `stable-ts-whisperless-2.17.0/stable_whisper/stabilization/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Union, Tuple, Optional
 
 import torch
 import numpy as np
 
 from .nonvad import NONVAD_SAMPLE_RATES, audio2loudness, wav2mask, visualize_mask
 from .silero_vad import VAD_SAMPLE_RATES, load_silero_vad_model, compute_vad_probs, assert_sr_window
-from .utils import is_ascending_sequence, valid_ts, mask2timing, timing2mask
+from .utils import is_ascending_sequence, valid_ts, mask2timing, timing2mask, filter_timings
 from ..audio.utils import audio_to_tensor_resample
 from ..default import get_min_word_dur
 
 from ..whisper_compatibility import SAMPLE_RATE, FRAMES_PER_SECOND, N_SAMPLES_PER_TOKEN
 
 
 class NonSpeechPredictor:
@@ -26,17 +26,19 @@
             vad_onnx: bool = False,
             vad_window: int = None,
             sampling_rate: int = None,
             verbose: Optional[bool] = True,
             store_timings: bool = False,
             ignore_is_silent: bool = False,
             stream: bool = False,
-            units_per_seconds: int = None
+            units_per_seconds: int = None,
+            min_silence_dur: Optional[float] = None
     ):
         min_word_dur = get_min_word_dur(min_word_dur)
+        self.min_silence_dur = min_silence_dur
         self.vad = vad
         self.mask_pad_func = mask_pad_func
         self.get_mask = get_mask
         self.q_levels = q_levels
         self.k_size = k_size
         self.vad_threshold = vad_threshold
         self.vad_onnx = vad_onnx
@@ -60,22 +62,32 @@
         self.second_per_prob = self.vad_window / self.sampling_rate
         self.vad_model = None
         self._prev_speech_probs = []
         self._default_probs = []
         self._using_callback = False
         self._load_vad_model()
         if self.vad is None:
-            self.predict = self.predict_with_samples
+            self._predict = self.predict_with_samples
         else:
-            self.predict = self.predict_with_vad if self.vad else self.predict_with_nonvad
+            self._predict = self.predict_with_vad if self.vad else self.predict_with_nonvad
 
     @property
     def nonspeech_timings(self):
         return self._nonspeech_timings
 
+    def predict(
+            self,
+            audio: torch.Tensor,
+            offset: Optional[float] = None
+    ) -> dict:
+        pred = self._predict(audio, offset)
+        if self.min_silence_dur:
+            pred['timings'] = filter_timings(pred['timings'], self.min_silence_dur)
+        return pred
+
     def _load_vad_model(self):
         if self.vad:
             self.vad_model = load_silero_vad_model()[0]
             self.reset()
 
     def reset(self):
         if self.vad_model is not None:
@@ -240,17 +252,24 @@
         return dict(timings=timings, mask=mask, is_silent=is_silent)
 
     def predict_with_samples(
             self,
             audio: torch.Tensor,
             offset: Optional[float] = None
     ) -> dict:
-        mask = torch.where(audio == 0, True, False).cpu()
-        is_silent = self._silent_mask_test(mask, self.min_samples_per_word)
-        return dict(timings=None, mask=None, is_silent=is_silent)
+        if self.get_mask:
+            if extra_len := audio.shape[-1] % N_SAMPLES_PER_TOKEN:
+                audio = torch.nn.functional.pad(audio, (0, N_SAMPLES_PER_TOKEN - extra_len))
+            mask = torch.all(audio.reshape(-1, N_SAMPLES_PER_TOKEN), dim=-1)
+            min_unit_per_word = self.min_frames_per_word
+        else:
+            mask = audio == 0
+            min_unit_per_word = self.min_samples_per_word
+        is_silent = self._silent_mask_test(mask, min_unit_per_word)
+        return dict(timings=None, mask=self.pad_mask(mask) if self.get_mask else None, is_silent=is_silent)
 
 
 def get_vad_silence_func(
         onnx=False,
         verbose: Optional[bool] = False
 ):
     predictor = NonSpeechPredictor(
@@ -287,60 +306,79 @@
     if len(silent_starts) == 0 or (result_obj.end - result_obj.start) <= min_word_dur:
         return
     if isinstance(silent_starts, list):
         silent_starts = np.array(silent_starts)
     if isinstance(silent_ends, list):
         silent_ends = np.array(silent_ends)
 
-    start_overlaps = np.all(
+    start_overlaps = (keep_end is None or keep_end) and np.all(
         (silent_starts <= result_obj.start, result_obj.start < silent_ends, silent_ends <= result_obj.end),
         axis=0
     ).nonzero()[0].tolist()
     if start_overlaps:
         new_start = silent_ends[start_overlaps[0]]
         result_obj.start = min(new_start, round(result_obj.end - min_word_dur, 3))
         if (result_obj.end - result_obj.start) <= min_word_dur:
             return
 
-    end_overlaps = np.all(
+    end_overlaps = not keep_end and np.all(
         (result_obj.start <= silent_starts, silent_starts < result_obj.end, result_obj.end <= silent_ends),
         axis=0
     ).nonzero()[0].tolist()
     if end_overlaps:
         new_end = silent_starts[end_overlaps[0]]
         result_obj.end = max(new_end, round(result_obj.start + min_word_dur, 3))
         if (result_obj.end - result_obj.start) <= min_word_dur:
             return
 
     if nonspeech_error:
         matches = np.logical_and(
             result_obj.start <= silent_starts,
             result_obj.end >= silent_ends,
         ).nonzero()[0].tolist()
-        if len(matches) == 0:
+        if len(matches) != 1:
             return
-        silence_start = np.min(silent_starts[matches])
-        silence_end = np.max(silent_ends[matches])
-        start_extra = silence_start - result_obj.start
-        end_extra = result_obj.end - silence_end
-        silent_duration = silence_end - silence_start
-        start_within_error = (start_extra / silent_duration) <= nonspeech_error
-        end_within_error = (end_extra / silent_duration) <= nonspeech_error
-        if keep_end is None:
-            keep_end = start_extra <= end_extra
-            within_error = start_within_error if keep_end else end_within_error
-        else:
-            within_error = start_within_error or end_within_error
 
-        if within_error:
-            if keep_end:
+        def silence_errors(silence_start, silence_end):
+            start_extra = silence_start - result_obj.start
+            end_extra = result_obj.end - silence_end
+            silent_duration = silence_end - silence_start
+            start_error = start_extra / silent_duration
+            end_error = end_extra / silent_duration
+            return start_error, end_error
+
+        def _adjust(silence_start, silence_end, errors=None):
+            if not errors:
+                errors = silence_errors(silence_start, silence_end)
+            _keep_end = keep_end
+            start_within_error = errors[0] <= nonspeech_error
+            end_within_error = errors[1] <= nonspeech_error
+            if _keep_end is None:
+                _keep_end = errors[0] <= errors[1]
+            if not (start_within_error or end_within_error):
+                return
+            if _keep_end:
                 result_obj.start = min(silence_end, round(result_obj.end - min_word_dur, 3))
             else:
                 result_obj.end = max(silence_start, round(result_obj.start + min_word_dur, 3))
 
+        max_i = len(matches) - 1
+        for i in range(len(matches)):
+            error = None
+            if i == max_i:
+                idx = 0
+            elif keep_end is None:
+                error0 = silence_errors(silent_starts[matches[0]], silent_ends[matches[0]])
+                error1 = silence_errors(silent_starts[matches[-1]], silent_ends[matches[-1]])
+                idx, error = (0, error0) if min(error0) <= min(error1) else (-1, error1)
+            else:
+                idx = 0 if keep_end else -1
+            idx = matches.pop(idx)
+            _adjust(silent_starts[idx], silent_ends[idx], error)
+
 
 def visualize_suppression(
         audio: Union[torch.Tensor, np.ndarray, str, bytes],
         output: str = None,
         q_levels: int = 20,
         k_size: int = 5,
         vad_threshold: float = 0.35,
```

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/stabilization/nonvad.py` & `stable-ts-whisperless-2.17.0/stable_whisper/stabilization/nonvad.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/stabilization/silero_vad.py` & `stable-ts-whisperless-2.17.0/stable_whisper/stabilization/silero_vad.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/stabilization/utils.py` & `stable-ts-whisperless-2.17.0/stable_whisper/stabilization/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -100,14 +100,25 @@
     mask_e = (silent_ends * units_per_second).round().astype(np.int32)
     for mi, me in zip(mask_i, mask_e):
         ts_token_mask[mi:me+1] = True
 
     return ts_token_mask
 
 
+def filter_timings(
+        silent_timings: Union[Tuple[np.ndarray, np.ndarray], None],
+        min_silence_dur: float
+) -> (Tuple[np.ndarray, np.ndarray], None):
+    if silent_timings is None:
+        return
+    silent_starts, silent_ends = silent_timings
+    mask = (silent_ends - silent_starts) >= min_silence_dur
+    return silent_starts[mask], silent_ends[mask]
+
+
 class SetTorchThread:
     def __init__(self, temp_thread_count: int):
         self.original_thread_count = torch.get_num_threads()
         self.temp_thread_count = temp_thread_count
 
     def __enter__(self):
         torch.set_num_threads(self.temp_thread_count)
```

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/text_output.py` & `stable-ts-whisperless-2.17.0/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/timing.py` & `stable-ts-whisperless-2.17.0/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/utils.py` & `stable-ts-whisperless-2.17.0/stable_whisper/utils.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/video_output.py` & `stable-ts-whisperless-2.17.0/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/whisper_compatibility.py` & `stable-ts-whisperless-2.17.0/stable_whisper/whisper_compatibility.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,27 +45,29 @@
     from whisper.timing import median_filter, dtw, merge_punctuations
     from whisper.tokenizer import get_tokenizer as get_whisper_tokenizer
 
     from whisper.tokenizer import Tokenizer
     from whisper.model import Whisper
     from whisper.decoding import DecodingTask, DecodingOptions, DecodingResult, SuppressTokens
 else:
+    import torch
+    import numpy as np
     whisper = None
     # hard-coded audio hyperparameters from Whisper
     SAMPLE_RATE = 16000
     N_FFT = 400
     HOP_LENGTH = 160
     CHUNK_LENGTH = 30
     N_SAMPLES = CHUNK_LENGTH * SAMPLE_RATE  # 480000 samples in a 30-second chunk
     N_FRAMES = exact_div(N_SAMPLES, HOP_LENGTH)  # 3000 frames in a mel spectrogram input
     N_SAMPLES_PER_TOKEN = HOP_LENGTH * 2  # the initial convolutions has stride 2
     FRAMES_PER_SECOND = exact_div(SAMPLE_RATE, HOP_LENGTH)  # 10ms per audio frame
     TOKENS_PER_SECOND = exact_div(SAMPLE_RATE, N_SAMPLES_PER_TOKEN)  # 20ms per audio token
 
-    log_mel_spectrogram = pad_or_trim = median_filter = dtw = merge_punctuations = get_whisper_tokenizer \
+    log_mel_spectrogram = median_filter = dtw = merge_punctuations = get_whisper_tokenizer \
         = whisper_not_available
     Tokenizer = Whisper = DecodingTask = DecodingOptions = DecodingResult = SuppressTokens = Unavailable
     LANGUAGES = {
         "en": "english",
         "zh": "chinese",
         "de": "german",
         "es": "spanish",
@@ -181,14 +183,40 @@
         "moldovan": "ro",
         "sinhalese": "si",
         "castilian": "es",
         "mandarin": "zh",
     }
 
 
+    def pad_or_trim(array, length: int = N_SAMPLES, *, axis: int = -1):
+        """
+        Pad or trim the audio array to N_SAMPLES, as expected by the encoder.
+        """
+        if torch.is_tensor(array):
+            if array.shape[axis] > length:
+                array = array.index_select(
+                    dim=axis, index=torch.arange(length, device=array.device)
+                )
+
+            if array.shape[axis] < length:
+                pad_widths = [(0, 0)] * array.ndim
+                pad_widths[axis] = (0, length - array.shape[axis])
+                array = torch.nn.functional.pad(array, [pad for sizes in pad_widths[::-1] for pad in sizes])
+        else:
+            if array.shape[axis] > length:
+                array = array.take(indices=range(length), axis=axis)
+
+            if array.shape[axis] < length:
+                pad_widths = [(0, 0)] * array.ndim
+                pad_widths[axis] = (0, length - array.shape[axis])
+                array = np.pad(array, pad_widths)
+
+        return array
+
+
 def warn_compatibility_issues(
         whisper_module,
         ignore: bool = False,
         additional_msg: str = ''
 ):
     compatibility_warning = ''
     if not ignore:
```

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/whisper_word_level/cli.py` & `stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/cli.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/whisper_word_level/faster_whisper.py` & `stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/faster_whisper.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         denoiser_options: Optional[dict] = None,
         demucs: bool = False,
         demucs_options: dict = None,
         vad: bool = False,
         vad_threshold: float = 0.35,
         vad_onnx: bool = False,
         min_word_dur: Optional[float] = None,
+        min_silence_dur: Optional[float] = None,
         nonspeech_error: float = 0.1,
         only_voice_freq: bool = False,
         only_ffmpeg: bool = False,
         check_sorted: bool = True,
         progress_callback: Callable = None,
         **options
 ) -> WhisperResult:
@@ -89,14 +90,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.3
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     only_ffmpeg : bool, default False
         Whether to use only FFmpeg (instead of not yt-dlp) for URls
     check_sorted : bool, default True
@@ -156,14 +159,15 @@
         k_size=k_size,
         denoiser=denoiser,
         denoiser_options=denoiser_options,
         vad=vad,
         vad_threshold=vad_threshold,
         vad_onnx=vad_onnx,
         min_word_dur=min_word_dur,
+        min_silence_dur=min_silence_dur,
         nonspeech_error=nonspeech_error,
         use_word_position=use_word_position,
         only_voice_freq=only_voice_freq,
         only_ffmpeg=only_ffmpeg,
         force_order=True,
         check_sorted=check_sorted,
         **extra_options
```

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/whisper_word_level/hf_whisper.py` & `stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/hf_whisper.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.16.0/stable_whisper/whisper_word_level/original_whisper.py` & `stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/original_whisper.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         denoiser_options: Optional[dict] = None,
         demucs: Union[bool, torch.nn.Module] = False,
         demucs_options: dict = None,
         vad: bool = False,
         vad_threshold: float = 0.35,
         vad_onnx: bool = False,
         min_word_dur: Optional[float] = None,
+        min_silence_dur: Optional[float] = None,
         nonspeech_error: float = 0.1,
         only_voice_freq: bool = False,
         prepend_punctuations: Optional[str] = None,
         append_punctuations: Optional[str] = None,
         stream: Optional[bool] = None,
         mel_first: Optional[bool] = None,
         split_callback: Callable = None,
@@ -139,14 +140,16 @@
         Silero VAD requires PyTorch 1.12.0+. Official repo, https://github.com/snakers4/silero-vad.
     vad_threshold : float, default 0.35
         Threshold for detecting speech with Silero VAD. Low threshold reduces false positives for silence detection.
     vad_onnx : bool, default False
         Whether to use ONNX for Silero VAD.
     min_word_dur : float or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Shortest duration each word is allowed to reach for silence suppression.
+    min_silence_dur : float, optional
+        Shortest duration of silence allowed for silence suppression.
     nonspeech_error : float, default 0.1
         Relative error of non-speech sections that appear in between a word for silence suppression.
     only_voice_freq : bool, default False
         Whether to only use sound between 200 - 5000 Hz, where majority of human speech are.
     prepend_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
         Punctuations to prepend to next word.
     append_punctuations : str or None, default None meaning use ``stable_whisper.default.DEFAULT_VALUES``
@@ -398,15 +401,16 @@
         q_levels=q_levels,
         k_size=k_size,
         vad_threshold=vad_threshold,
         vad_onnx=vad_onnx,
         vad_window=512,
         sampling_rate=SAMPLE_RATE,
         verbose=None if audio.stream else verbose,
-        store_timings=True
+        store_timings=True,
+        min_silence_dur=min_silence_dur
     )
     audio.update_post_prep_callback(nonspeech_predictor.get_on_prep_callback(audio.stream))
 
     with tqdm(total=initial_duration, unit='sec', disable=verbose is not False, desc=task.title()) as tqdm_pbar:
 
         def update_pbar():
             nonlocal audio_features
```

