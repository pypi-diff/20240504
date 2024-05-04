# Comparing `tmp/stable-ts-2.8.1.tar.gz` & `tmp/stable-ts-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.8.1.tar", last modified: Sat Aug  5 00:09:41 2023, max compression
+gzip compressed data, was "stable-ts-2.9.0.tar", last modified: Fri Aug 18 21:18:26 2023, max compression
```

## Comparing `stable-ts-2.8.1.tar` & `stable-ts-2.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 00:09:41.793621 stable-ts-2.8.1/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.8.1/LICENSE
--rw-rw-rw-   0        0        0    11471 2023-08-05 00:09:41.792622 stable-ts-2.8.1/PKG-INFO
--rw-rw-rw-   0        0        0    11175 2023-08-04 23:35:49.000000 stable-ts-2.8.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-05 00:09:41.793621 stable-ts-2.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 00:09:41.768621 stable-ts-2.8.1/stable_ts.egg-info/
--rw-rw-rw-   0        0        0    11471 2023-08-05 00:09:41.000000 stable-ts-2.8.1/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-08-05 00:09:41.000000 stable-ts-2.8.1/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 00:09:41.000000 stable-ts-2.8.1/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-08-05 00:09:41.000000 stable-ts-2.8.1/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-08-05 00:09:41.000000 stable-ts-2.8.1/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-08-05 00:09:41.000000 stable-ts-2.8.1/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-05 00:09:41.790623 stable-ts-2.8.1/stable_whisper/
--rw-rw-rw-   0        0        0      241 2023-07-13 00:23:52.000000 stable-ts-2.8.1/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.8.1/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-08-05 00:06:13.000000 stable-ts-2.8.1/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     8360 2023-07-13 00:08:53.000000 stable-ts-2.8.1/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.8.1/stable_whisper/decode.py
--rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.8.1/stable_whisper/enhancement.py
--rw-rw-rw-   0        0        0    12947 2023-07-13 00:22:18.000000 stable-ts-2.8.1/stable_whisper/non_whisper.py
--rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.8.1/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    45254 2023-08-05 00:05:24.000000 stable-ts-2.8.1/stable_whisper/result.py
--rw-rw-rw-   0        0        0    14128 2023-07-12 23:15:05.000000 stable-ts-2.8.1/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.8.1/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.8.1/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.8.1/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    53252 2023-07-13 00:20:47.000000 stable-ts-2.8.1/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-08-18 21:18:26.573698 stable-ts-2.9.0/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.9.0/LICENSE
+-rw-rw-rw-   0        0        0    11502 2023-08-18 21:18:26.573698 stable-ts-2.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11206 2023-08-18 20:22:38.000000 stable-ts-2.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-18 21:18:26.574698 stable-ts-2.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-18 21:18:26.496698 stable-ts-2.9.0/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0    11502 2023-08-18 21:18:26.000000 stable-ts-2.9.0/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-08-18 21:18:26.000000 stable-ts-2.9.0/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-18 21:18:26.000000 stable-ts-2.9.0/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-08-18 21:18:26.000000 stable-ts-2.9.0/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-08-18 21:18:26.000000 stable-ts-2.9.0/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-18 21:18:26.000000 stable-ts-2.9.0/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-18 21:18:26.571699 stable-ts-2.9.0/stable_whisper/
+-rw-rw-rw-   0        0        0      241 2023-07-13 00:23:52.000000 stable-ts-2.9.0/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.9.0/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-08-18 20:13:08.000000 stable-ts-2.9.0/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     8360 2023-07-13 00:08:53.000000 stable-ts-2.9.0/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.9.0/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.9.0/stable_whisper/enhancement.py
+-rw-rw-rw-   0        0        0    12947 2023-07-13 00:22:18.000000 stable-ts-2.9.0/stable_whisper/non_whisper.py
+-rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.9.0/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    46024 2023-08-18 21:15:36.000000 stable-ts-2.9.0/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    14128 2023-07-12 23:15:05.000000 stable-ts-2.9.0/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.9.0/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.9.0/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.9.0/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    53797 2023-08-18 20:27:47.000000 stable-ts-2.9.0/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.8.1/LICENSE` & `stable-ts-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.8.1/PKG-INFO` & `stable-ts-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.8.1
+Version: 2.9.0
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -48,15 +48,15 @@
 ```python
 import stable_whisper
 model = stable_whisper.load_model('base')
 result = model.transcribe('audio.mp3')
 result.to_srt_vtt('audio.srt')
 ```
 Parameters: 
-[load_model()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L633-L658), 
+[load_model()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L651-L676), 
 [transcribe()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L68-L203)
 ### Output
 Stable-ts supports various text output formats.
 ```python
 result.to_srt_vtt('audio.srt') #SRT
 result.to_srt_vtt('audio.vtt') #VTT
 result.to_ass('audio.ass') #ASS
@@ -131,34 +131,35 @@
 
 ```python
 # The following all functionally equivalent:
 result0 = model.transcribe('audio.mp3', regroup=True) # regroup is True by default
 result1 = model.transcribe('audio.mp3', regroup=False)
 (
     result1
-    .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
+    .clamp_max()
+    .split_by_punctuation([('.', ' '), '。', '?', '？', (',', ' '), '，'])
     .split_by_gap(.5)
     .merge_by_gap(.3, max_words=3)
     .split_by_punctuation([('.', ' '), '。', '?', '？'])
 )
-result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.3+3_sp=.* /。/?/？')
+result2 = model.transcribe('audio.mp3', regroup='cm_sp=.* /。/?/？/,* /，_sg=.5_mg=.3+3_sp=.* /。/?/？')
 
 # To undo all regrouping operations:
 result0.reset()
 ```
 Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
-- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L908-L956)
-- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L705-L717)
-- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L758-L769)
-- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L820-L839)
-- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L729-L747)
-- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L781-L799)
-- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L806-L808)
-- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L858-L875)
+- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L920-L968)
+- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L717-L729)
+- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L770-L781)
+- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L832-L851)
+- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L741-L759)
+- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L793-L811)
+- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L818-L820)
+- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L870-L887)
 
 ### Locating Words
 You can locate words with regular expression.
 ```python
 # Find every sentence that contains "and"
 matches = result.find(r'[^.]+and[^.]+\.')
 # print the all matches if there are any
@@ -173,15 +174,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L999-L1015)
+[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L1013-L1029)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
```

### Comparing `stable-ts-2.8.1/README.md` & `stable-ts-2.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 ```python
 import stable_whisper
 model = stable_whisper.load_model('base')
 result = model.transcribe('audio.mp3')
 result.to_srt_vtt('audio.srt')
 ```
 Parameters: 
-[load_model()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L633-L658), 
+[load_model()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L651-L676), 
 [transcribe()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L68-L203)
 ### Output
 Stable-ts supports various text output formats.
 ```python
 result.to_srt_vtt('audio.srt') #SRT
 result.to_srt_vtt('audio.vtt') #VTT
 result.to_ass('audio.ass') #ASS
@@ -120,34 +120,35 @@
 
 ```python
 # The following all functionally equivalent:
 result0 = model.transcribe('audio.mp3', regroup=True) # regroup is True by default
 result1 = model.transcribe('audio.mp3', regroup=False)
 (
     result1
-    .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
+    .clamp_max()
+    .split_by_punctuation([('.', ' '), '。', '?', '？', (',', ' '), '，'])
     .split_by_gap(.5)
     .merge_by_gap(.3, max_words=3)
     .split_by_punctuation([('.', ' '), '。', '?', '？'])
 )
-result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.3+3_sp=.* /。/?/？')
+result2 = model.transcribe('audio.mp3', regroup='cm_sp=.* /。/?/？/,* /，_sg=.5_mg=.3+3_sp=.* /。/?/？')
 
 # To undo all regrouping operations:
 result0.reset()
 ```
 Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
-- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L908-L956)
-- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L705-L717)
-- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L758-L769)
-- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L820-L839)
-- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L729-L747)
-- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L781-L799)
-- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L806-L808)
-- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L858-L875)
+- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L920-L968)
+- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L717-L729)
+- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L770-L781)
+- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L832-L851)
+- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L741-L759)
+- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L793-L811)
+- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L818-L820)
+- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L870-L887)
 
 ### Locating Words
 You can locate words with regular expression.
 ```python
 # Find every sentence that contains "and"
 matches = result.find(r'[^.]+and[^.]+\.')
 # print the all matches if there are any
@@ -162,15 +163,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L999-L1015)
+[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L1013-L1029)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
```

### Comparing `stable-ts-2.8.1/setup.py` & `stable-ts-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.8.1/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.9.0/stable_ts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.8.1
+Version: 2.9.0
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -48,15 +48,15 @@
 ```python
 import stable_whisper
 model = stable_whisper.load_model('base')
 result = model.transcribe('audio.mp3')
 result.to_srt_vtt('audio.srt')
 ```
 Parameters: 
-[load_model()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L633-L658), 
+[load_model()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L651-L676), 
 [transcribe()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L68-L203)
 ### Output
 Stable-ts supports various text output formats.
 ```python
 result.to_srt_vtt('audio.srt') #SRT
 result.to_srt_vtt('audio.vtt') #VTT
 result.to_ass('audio.ass') #ASS
@@ -131,34 +131,35 @@
 
 ```python
 # The following all functionally equivalent:
 result0 = model.transcribe('audio.mp3', regroup=True) # regroup is True by default
 result1 = model.transcribe('audio.mp3', regroup=False)
 (
     result1
-    .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
+    .clamp_max()
+    .split_by_punctuation([('.', ' '), '。', '?', '？', (',', ' '), '，'])
     .split_by_gap(.5)
     .merge_by_gap(.3, max_words=3)
     .split_by_punctuation([('.', ' '), '。', '?', '？'])
 )
-result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.3+3_sp=.* /。/?/？')
+result2 = model.transcribe('audio.mp3', regroup='cm_sp=.* /。/?/？/,* /，_sg=.5_mg=.3+3_sp=.* /。/?/？')
 
 # To undo all regrouping operations:
 result0.reset()
 ```
 Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
-- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L908-L956)
-- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L705-L717)
-- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L758-L769)
-- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L820-L839)
-- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L729-L747)
-- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L781-L799)
-- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L806-L808)
-- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L858-L875)
+- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L920-L968)
+- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L717-L729)
+- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L770-L781)
+- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L832-L851)
+- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L741-L759)
+- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L793-L811)
+- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L818-L820)
+- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L870-L887)
 
 ### Locating Words
 You can locate words with regular expression.
 ```python
 # Find every sentence that contains "and"
 matches = result.find(r'[^.]+and[^.]+\.')
 # print the all matches if there are any
@@ -173,15 +174,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L999-L1015)
+[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L1013-L1029)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
```

### Comparing `stable-ts-2.8.1/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.9.0/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.8.1/stable_whisper/audio.py` & `stable-ts-2.9.0/stable_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.8.1/stable_whisper/decode.py` & `stable-ts-2.9.0/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.8.1/stable_whisper/enhancement.py` & `stable-ts-2.9.0/stable_whisper/enhancement.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.8.1/stable_whisper/non_whisper.py` & `stable-ts-2.9.0/stable_whisper/non_whisper.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.8.1/stable_whisper/quantization.py` & `stable-ts-2.9.0/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.8.1/stable_whisper/result.py` & `stable-ts-2.9.0/stable_whisper/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,14 +463,15 @@
 
     def __init__(self, result: Union[str, dict, list]):
         result, self.path = self._standardize_result(result)
         self.ori_dict = result.get('ori_dict') or result
         self.language = self.ori_dict.get('language')
         segments = deepcopy(result.get('segments', self.ori_dict.get('segments')))
         self.segments: List[Segment] = [Segment(**s) for s in segments] if segments else []
+        self.raise_for_unsorted()
         self.remove_no_word_segments()
         self.update_all_segs_with_words()
 
     @staticmethod
     def _standardize_result(result: Union[str, dict, list]):
         path = None
         if isinstance(result, str):
@@ -494,14 +495,25 @@
 
             elif isinstance(result[0], dict):
                 result = dict(segments=result)
             else:
                 raise NotImplementedError(f'Got list of {type(result[0])} but expects list of list/dict')
         return result, path
 
+    def raise_for_unsorted(self):
+        parts = self.all_words() if self.has_words else self.segments
+        timestamps = np.array(list(chain.from_iterable((part.start, part.end) for part in parts)))
+        if len(timestamps) < 2:
+            return
+        if ((timestamps[1:] - timestamps[:-1]) < 0).any():
+            raise NotImplementedError(f'Timestamps are not in ascending order. '
+                                      f'For transcribe_any() or data not produced by Stable-ts, '
+                                      f'sort segments/words by timestamps. '
+                                      f'Otherwise, please submit an issue.')
+
     def update_all_segs_with_words(self):
         for seg in self.segments:
             seg.update_seg_with_words()
 
     def add_segments(self, index0: int, index1: int, inplace: bool = False, lock: bool = False):
         new_seg = self.segments[index0] + self.segments[index1]
         new_seg.update_seg_with_words()
@@ -853,15 +865,15 @@
             self,
             medium_factor: float = 2.5,
             max_dur: float = None,
             clip_start: bool = None,
             verbose: bool = False):
         """
 
-        Clamp all word durations above certain value.
+        Clamp all word durations above certain value. Note: most effective when applied before other regroup operations.
 
         Parameters
         ----------
         medium_factor: float
             Clamp durations above ([medium_factor] * medium duration) per segment. (Default: 2.5)
             If [medium_factor]=None/0 or segment has less than 3 words, it will be ignored and use only [max_dur].
         max_dur: float
@@ -918,15 +930,15 @@
                     sg: split_by_gap
                     sp: split_by_punctuation
                     sl: split_by_length
                     mg: merge_by_gap
                     mp: merge_by_punctuation
                     ms: merge_all_segment
                     cm: clamp_max
-                    da: default algorithm (sp=.* /。/?/？/,/，_sg=.5_mg=.3+3_sp=.* /。/?/？)
+                    da: default algorithm (cm_sp=.* /。/?/？/,* /，_sg=.5_mg=.3+3_sp=.* /。/?/？)
 
                 Metacharacters:
                     = separates a method key and its arguments (not used if no argument)
                     _ separates method keys (after arguments if there are any)
                     + separates arguments for a method key
                     / separates an argument into list of strings
                     * separates an item in list of strings into a nested list of strings
@@ -979,15 +991,15 @@
             except ValueError:
                 pass
             finally:
                 return x
 
         calls = regroup_algo.split('_')
         if 'da' in calls:
-            default_calls = 'sp=.* /。/?/？/,/，_sg=.5_mg=.3+3_sp=.* /。/?/？'.split('_')
+            default_calls = 'cm_sp=.* /。/?/？/,* /，_sg=.5_mg=.3+3_sp=.* /。/?/？'.split('_')
             calls = chain.from_iterable(default_calls if method == 'da' else [method] for method in calls)
         for method in calls:
             method, args = method.split('=', maxsplit=1) if '=' in method else (method, '')
             if method not in methods:
                 raise NotImplementedError(f'{method} is not one of the available methods: {tuple(methods.keys())}')
             args = [] if len(args) == 0 else list(map(_to_arg, args.split('+')))
             if verbose or only_show:
```

### Comparing `stable-ts-2.8.1/stable_whisper/stabilization.py` & `stable-ts-2.9.0/stable_whisper/stabilization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.8.1/stable_whisper/text_output.py` & `stable-ts-2.9.0/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.8.1/stable_whisper/timing.py` & `stable-ts-2.9.0/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.8.1/stable_whisper/video_output.py` & `stable-ts-2.9.0/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.8.1/stable_whisper/whisper_word_level.py` & `stable-ts-2.9.0/stable_whisper/whisper_word_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,14 +344,19 @@
             ):
                 needs_fallback = True  # too repetitive
             if (
                     logprob_threshold is not None
                     and decode_result.avg_logprob < logprob_threshold
             ):
                 needs_fallback = True  # average log probability is too low
+            if (
+                no_speech_threshold is not None
+                and decode_result.no_speech_prob > no_speech_threshold
+            ):
+                needs_fallback = False  # silence
 
             if not needs_fallback:
                 break
 
         return decode_result
 
     seek_sample = 0  # samples
@@ -378,14 +383,16 @@
             "tokens": tokens,
             "temperature": result.temperature,
             "avg_logprob": result.avg_logprob,
             "compression_ratio": result.compression_ratio,
             "no_speech_prob": result.no_speech_prob,
         }
 
+    punctuations = prepend_punctuations + append_punctuations
+
     total_samples = audio.shape[-1]
     total_duration = round(total_samples / curr_sr, 2)
     n_samples_per_frame = exact_div(N_SAMPLES_PER_TOKEN * TOKENS_PER_SECOND, FRAMES_PER_SECOND)
 
     silence_timing = None
     if suppress_silence and vad:
         silence_timing = get_vad_silence_func(onnx=vad_onnx, verbose=verbose)(audio, speech_threshold=vad_threshold)
@@ -483,79 +490,91 @@
                     )
                     end_timestamp_pos = (
                             sliced_tokens[-1].item() - tokenizer.timestamp_begin
                     )
                     current_segments.append(
                         new_segment(
                             start=round(time_offset + start_timestamp_pos * time_precision, 3),
-                            end=round(time_offset + end_timestamp_pos * time_precision, 3),
+                            end=round(time_offset + min(end_timestamp_pos * time_precision, segment_duration), 3),
                             tokens=sliced_tokens,
                             result=result,
                         )
                     )
                     last_slice = current_slice
 
-                if not single_timestamp_ending:
-                    # otherwise, ignore the unfinished segment and seek to the last timestamp
-                    last_timestamp_pos = (
-                            tokens[last_slice - 1].item() - tokenizer.timestamp_begin
-                    )
-                    segment_samples = min(segment_samples, round(last_timestamp_pos * N_SAMPLES_PER_TOKEN))
             else:
                 duration = segment_duration
                 timestamps = tokens[timestamp_tokens.nonzero().flatten()]
                 if (
                         len(timestamps) > 0
                         and timestamps[-1].item() != tokenizer.timestamp_begin
                 ):
                     # no consecutive timestamps but it has a timestamp; use the last one.
-                    last_timestamp_pos = (
+                    end_timestamp_pos = (
                             timestamps[-1].item() - tokenizer.timestamp_begin
                     )
-                    duration = last_timestamp_pos * time_precision
+                    duration = min(end_timestamp_pos * time_precision, segment_duration)
+                else:
+                    end_timestamp_pos = 0
 
                 current_segments.append(
                     new_segment(
                         start=round(time_offset, 3),
                         end=round(time_offset + duration, 3),
                         tokens=tokens,
                         result=result,
                     )
                 )
 
             # if a segment is instantaneous or does not contain text, remove it
             for i in reversed(range(len(current_segments))):
                 seg = current_segments[i]
-                if seg["start"] == seg["end"] or seg["text"].strip() == "":
+                if seg["start"] == seg["end"] or seg["text"].strip() in punctuations:
                     del current_segments[i]
 
-            if len(current_segments) == 0:
-                fast_forward()
-                continue
-
-            if not condition_on_previous_text or result.temperature > 0.5:
-                # do not feed the prompt tokens if a high temperature was used
-                prompt_reset_since = len(all_tokens)
+            num_samples = segment_samples
 
             if word_timestamps:
+                if end_timestamp_pos > 0:
+                    num_samples = min(round(end_timestamp_pos * N_SAMPLES_PER_TOKEN), num_samples)
                 add_word_timestamps_stable(
                     segments=current_segments,
                     model=model,
                     tokenizer=tokenizer,
                     mel=mel_segment,
-                    num_samples=segment_samples,
+                    num_samples=num_samples,
                     prepend_punctuations=prepend_punctuations,
                     append_punctuations=append_punctuations,
                     audio_features=audio_features,
                     ts_num=ts_num,
                     ts_noise=ts_noise,
                     split_callback=split_callback,
                     gap_padding=gap_padding
                 )
 
+                # if 50%+ of the words in a segment are instantaneous, remove it
+                for i in reversed(range(len(current_segments))):
+                    zero_duration_percent = (
+                        np.array(
+                            [w['start'] == w['end'] for w in current_segments[i]['words']]
+                        )
+                        .astype(np.float16)
+                        .mean()
+                    )
+                    if zero_duration_percent >= 0.5:
+                        del current_segments[i]
+
+            if len(current_segments) == 0:
+                fast_forward()
+                continue
+
+            if not condition_on_previous_text or result.temperature > 0.5:
+                # do not feed the prompt tokens if a high temperature was used
+                prompt_reset_since = len(all_tokens)
+
             if segment_silence_timing is not None:
                 for seg_i, segment in enumerate(current_segments):
                     current_segments[seg_i] = (
                         Segment(**segment)
                         .suppress_silence(
                             *segment_silence_timing,
                             min_word_dur=min_word_dur,
@@ -584,17 +603,16 @@
                     {"id": i, **segment}
                     for i, segment in enumerate(current_segments, start=len(all_segments))
                 ]
             )
             all_tokens.extend(
                 [token for segment in current_segments for token in segment["tokens"]]
             )
-            if not single_timestamp_ending and len(consecutive) > 0 and \
-                    (alt_segment_duration := (current_segments[-1]['end'] - time_offset)) > 0:
-                segment_samples = min(round(alt_segment_duration * SAMPLE_RATE), segment_samples)
+            if not single_timestamp_ending:
+                segment_samples = num_samples
             fast_forward()
 
         # final update
         update_pbar()
 
     if model.device != torch.device('cpu'):
         torch.cuda.empty_cache()
```

