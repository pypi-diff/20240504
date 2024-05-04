# Comparing `tmp/stable-ts-whisperless-2.17.0.tar.gz` & `tmp/stable-ts-whisperless-2.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-whisperless-2.17.0.tar", last modified: Fri May  3 03:58:25 2024, max compression
+gzip compressed data, was "stable-ts-whisperless-2.17.1.tar", last modified: Sat May  4 01:23:21 2024, max compression
```

## Comparing `stable-ts-whisperless-2.17.0.tar` & `stable-ts-whisperless-2.17.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:25.421067 stable-ts-whisperless-2.17.0/
--rw-rw-rw-   0        0        0     1082 2024-04-20 20:29:43.000000 stable-ts-whisperless-2.17.0/LICENSE
--rw-rw-rw-   0        0        0    86923 2024-05-03 03:58:25.420068 stable-ts-whisperless-2.17.0/PKG-INFO
--rw-rw-rw-   0        0        0    86522 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 03:58:25.421067 stable-ts-whisperless-2.17.0/setup.cfg
--rw-rw-rw-   0        0        0     1040 2024-05-03 03:41:17.000000 stable-ts-whisperless-2.17.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:25.418068 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/
--rw-rw-rw-   0        0        0    86923 2024-05-03 03:58:25.000000 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1287 2024-05-03 03:58:25.000000 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 03:58:25.000000 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-03 03:58:25.000000 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-05-03 03:58:25.000000 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-03 03:58:25.000000 stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:25.390068 stable-ts-whisperless-2.17.0/stable_whisper/
--rw-rw-rw-   0        0        0      353 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       50 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       24 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/_version.py
--rw-rw-rw-   0        0        0    69318 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/alignment.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:25.401067 stable-ts-whisperless-2.17.0/stable_whisper/audio/
--rw-rw-rw-   0        0        0    24130 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/audio/__init__.py
--rw-rw-rw-   0        0        0     7657 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/audio/demucs.py
--rw-rw-rw-   0        0        0     3276 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/audio/dfnet.py
--rw-rw-rw-   0        0        0     2952 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/audio/noisereduce.py
--rw-rw-rw-   0        0        0     1977 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/audio/output.py
--rw-rw-rw-   0        0        0     8761 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/audio/utils.py
--rw-rw-rw-   0        0        0     4522 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/decode.py
--rw-rw-rw-   0        0        0     2047 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/default.py
--rw-rw-rw-   0        0        0    16051 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/non_whisper.py
--rw-rw-rw-   0        0        0     2308 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0   103457 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/result.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:25.408067 stable-ts-whisperless-2.17.0/stable_whisper/stabilization/
--rw-rw-rw-   0        0        0    18720 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/stabilization/__init__.py
--rw-rw-rw-   0        0        0     4936 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/stabilization/nonvad.py
--rw-rw-rw-   0        0        0     2246 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/stabilization/silero_vad.py
--rw-rw-rw-   0        0        0     4491 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/stabilization/utils.py
--rw-rw-rw-   0        0        0    24042 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    11350 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2622 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/utils.py
--rw-rw-rw-   0        0        0     4020 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0     9426 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/whisper_compatibility.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:25.416068 stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/
--rw-rw-rw-   0        0        0      454 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/__init__.py
--rw-rw-rw-   0        0        0    39229 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/cli.py
--rw-rw-rw-   0        0        0    11231 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/faster_whisper.py
--rw-rw-rw-   0        0        0     9957 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/hf_whisper.py
--rw-rw-rw-   0        0        0    42315 2024-05-03 03:48:11.000000 stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/original_whisper.py
+drwxrwxrwx   0        0        0        0 2024-05-04 01:23:21.509606 stable-ts-whisperless-2.17.1/
+-rw-rw-rw-   0        0        0     1082 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/LICENSE
+-rw-rw-rw-   0        0        0    86923 2024-05-04 01:23:21.508604 stable-ts-whisperless-2.17.1/PKG-INFO
+-rw-rw-rw-   0        0        0    86522 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 01:23:21.509606 stable-ts-whisperless-2.17.1/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 01:23:21.506602 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/
+-rw-rw-rw-   0        0        0    86923 2024-05-04 01:23:20.000000 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1287 2024-05-04 01:23:21.000000 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 01:23:20.000000 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-04 01:23:20.000000 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-05-04 01:23:20.000000 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-04 01:23:20.000000 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 01:23:21.389603 stable-ts-whisperless-2.17.1/stable_whisper/
+-rw-rw-rw-   0        0        0      353 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       24 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0    70127 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/alignment.py
+drwxrwxrwx   0        0        0        0 2024-05-04 01:23:21.438605 stable-ts-whisperless-2.17.1/stable_whisper/audio/
+-rw-rw-rw-   0        0        0    24130 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/audio/__init__.py
+-rw-rw-rw-   0        0        0     7657 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/audio/demucs.py
+-rw-rw-rw-   0        0        0     3276 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/audio/dfnet.py
+-rw-rw-rw-   0        0        0     2952 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/audio/noisereduce.py
+-rw-rw-rw-   0        0        0     1977 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/audio/output.py
+-rw-rw-rw-   0        0        0     8761 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/audio/utils.py
+-rw-rw-rw-   0        0        0     4522 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0     2047 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/default.py
+-rw-rw-rw-   0        0        0    16051 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/non_whisper.py
+-rw-rw-rw-   0        0        0     2308 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0   103457 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/result.py
+drwxrwxrwx   0        0        0        0 2024-05-04 01:23:21.463603 stable-ts-whisperless-2.17.1/stable_whisper/stabilization/
+-rw-rw-rw-   0        0        0    18720 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/stabilization/__init__.py
+-rw-rw-rw-   0        0        0     4936 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/stabilization/nonvad.py
+-rw-rw-rw-   0        0        0     2246 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/stabilization/silero_vad.py
+-rw-rw-rw-   0        0        0     4491 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/stabilization/utils.py
+-rw-rw-rw-   0        0        0    24042 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    11983 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2622 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/utils.py
+-rw-rw-rw-   0        0        0     4020 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0     9426 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/whisper_compatibility.py
+drwxrwxrwx   0        0        0        0 2024-05-04 01:23:21.503602 stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/
+-rw-rw-rw-   0        0        0      454 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/__init__.py
+-rw-rw-rw-   0        0        0    39229 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/cli.py
+-rw-rw-rw-   0        0        0    11231 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/faster_whisper.py
+-rw-rw-rw-   0        0        0     9957 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/hf_whisper.py
+-rw-rw-rw-   0        0        0    42315 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/original_whisper.py
```

### Comparing `stable-ts-whisperless-2.17.0/LICENSE` & `stable-ts-whisperless-2.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/PKG-INFO` & `stable-ts-whisperless-2.17.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts-whisperless
-Version: 2.17.0
+Version: 2.17.1
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-whisperless-2.17.0/README.md` & `stable-ts-whisperless-2.17.1/README.md`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/setup.py` & `stable-ts-whisperless-2.17.1/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/PKG-INFO` & `stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts-whisperless
-Version: 2.17.0
+Version: 2.17.1
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-whisperless-2.17.0/stable_ts_whisperless.egg-info/SOURCES.txt` & `stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/alignment.py` & `stable-ts-whisperless-2.17.1/stable_whisper/alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,19 +255,19 @@
             pad_mask = []
             cumsums = split_indices_by_char.tolist()
             cumsum_len = 0
             for word in words:
                 cumsum_len += len(word)
                 if cumsums and cumsum_len >= cumsums[0]:
                     cumsums.pop(0)
-                    pad_mask.append(True)
+                    pad_mask.extend([True]*len(word))
                 else:
-                    pad_mask.append(False)
+                    pad_mask.extend([False]*len(word))
         else:
-            pad_mask = [any(map(w.endswith, presplit)) for w in words]
+            pad_mask = [b for w in words for b in [any(map(w.endswith, presplit))]*len(w)]
 
     if isinstance(audio, AudioLoader):
         audio.validate_external_args(
             sr=SAMPLE_RATE,
             vad=vad,
             stream=stream,
             denoiser=denoiser,
@@ -286,14 +286,15 @@
             stream=stream
         )
 
     initial_duration = audio.get_duration(2)
 
     seek_sample = 0
     total_words = len(words)
+    remaining_len = sum(len(w) for w in words)
 
     if is_faster_model:
 
         def timestamp_words():
             temp_segment = dict(
                 seek=0,
                 start=0.0,
@@ -353,34 +354,37 @@
                 mel=mel_segment,
                 num_samples=segment_samples,
                 split_callback=(lambda x, _: x),
                 prepend_punctuations=prepend_punctuations,
                 append_punctuations=append_punctuations,
                 gap_padding=gap_padding if presplit else None,
                 extra_models=extra_models,
+                pad_first_seg=pad_first_seg
             )
             if len(temp_segments) == 1:
                 return temp_segments[0]
             return dict(words=[w for seg in temp_segments for w in seg['words']])
 
     def get_curr_words():
-        nonlocal words, word_tokens, pad_mask
+        nonlocal words, word_tokens, pad_mask, remaining_len
         curr_tk_count = 0
         w, wt, m = [], [], []
+        is_start_gap = (True if remaining_len == len(pad_mask) else pad_mask[-(remaining_len+1)]) if pad_mask else True
         for i in range(len(words)):
             tk_count = len(word_tokens[0])
-            m_count = 1 if pad_mask and pad_mask[0] else 0
+            m_count = 1 if pad_mask and pad_mask[-(remaining_len-len(words[0])+1)] else 0
             if curr_tk_count + len(m) + tk_count + m_count > token_step and w:
                 break
+            if pad_mask and pad_mask[-(remaining_len-len(words[0])+1)]:
+                    m.append(i+1)
+            remaining_len -= len(words[0])
             w.append(words.pop(0))
             wt.append(word_tokens.pop(0))
             curr_tk_count += tk_count
-            if pad_mask and pad_mask.pop(0):
-                m.append(i+1)
-        return w, wt, m
+        return w, wt, m, is_start_gap
     result = []
 
     nonspeech_predictor = NonSpeechPredictor(
         vad=vad if suppress_silence else None,
         mask_pad_func=pad_or_trim,
         get_mask=True,
         min_word_dur=min_word_dur,
@@ -430,23 +434,26 @@
             if second_word_src is not None:
                 word_sources = [second_word_src] + word_sources
             return first_word_src, word_sources
 
         return first_word_src, word_sources[1:]
 
     def speech_percentage(_word: dict, _mask: torch.Tensor, _offset: float):
+        if _mask is None:
+            return 1
         s, e = _word['start'], _word['end']
         s = int((s - _offset) * TOKENS_PER_SECOND)
         e = int((e - _offset) * TOKENS_PER_SECOND)
         return 1 - _mask[s:e].float().mean().nan_to_num()
 
     def is_new_better(w0, m0, o0, w1, m1, o1):
         speech0 = speech_percentage(w0, m0, o0).round(decimals=1)
         speech1 = speech_percentage(w1, m1, o1).round(decimals=1)
-        return speech0 >= speech1 or w0['probability'] >= w1['probability']
+        w0p, w1p = w0['probability'], w1['probability']
+        return ((w1p**0.75 - w0p**0.75) < 0.35 and speech0 >= speech1) or w0p >= w1p
 
     with tqdm(total=initial_duration, unit='sec', disable=verbose is not False, desc='Align') as tqdm_pbar:
 
         def update_pbar(finish: bool = False):
             curr_total = audio.get_duration(2)
             if need_refresh := curr_total != tqdm_pbar.total:
                 tqdm_pbar.total = curr_total
@@ -459,15 +466,15 @@
         def update_curr_words():
             if temp_data['temp_word'] is not None:
                 temp_words = [temp_data['temp_word']] + temp_data['extra_words'][:len(curr_words) - 1]
                 curr_words[:len(temp_words)] = temp_words
                 temp_data['temp_word'] = None
 
         def redo_words(_idx: int = None):
-            nonlocal seg_words, seg_tokens, seg_words, words, word_tokens, curr_words, temp_data
+            nonlocal seg_words, seg_tokens, seg_words, words, word_tokens, curr_words, temp_data, remaining_len
             if _idx is not None and curr_words and temp_data['temp_word'] is not None:
                 temp_data['temp_word'], temp_data['extra_words'] = fix_temp_words(
                     curr_words[0],
                     [temp_data['temp_word']] + temp_data['extra_words'],
                     curr_words[1] if len(curr_words) > 1 else None
                 )
 
@@ -488,23 +495,26 @@
                             )
                             if use_new or cw['word'] != tw['word'] or cw['end'] < tw['end']:
                                 break
                             new_extra_words.append(tw)
                     temp_data['extra_words'] = new_extra_words
 
             if _idx is None:  # redo all
+                remaining_len += sum(len(w) for w in seg_words)
                 words = seg_words + words
                 word_tokens = seg_tokens + word_tokens
                 curr_words = []
             elif _idx != len(seg_words):  # redo from _idx
+                remaining_len += sum(len(w) for w in seg_words[_idx:])
                 words = seg_words[_idx:] + words
                 word_tokens = seg_tokens[_idx:] + word_tokens
                 curr_words, new_extra_words = curr_words[:_idx], curr_words[_idx:]
                 if curr_words:
                     update_curr_words()
+                    remaining_len += sum(len(w) for w in seg_words[_idx-1:_idx])
                     words = seg_words[_idx-1:_idx] + words
                     word_tokens = seg_tokens[_idx-1:_idx] + word_tokens
                     temp_data['temp_word'] = curr_words.pop(-1)
                     temp_data['extra_words'] = new_extra_words
                     temp_data['temp_mask'] = nonspeech_preds['mask']
                     temp_data['temp_offset'] = time_offset
             else:
@@ -555,15 +565,15 @@
                             if len(nonspeech_starts) > 1:
                                 new_sample_count = round((nonspeech_starts[1] - nonspeech_ends[0]) * SAMPLE_RATE)
                             else:
                                 new_sample_count = None
                             audio_segment = audio_segment[:new_sample_count]
                             segment_samples = audio_segment.shape[-1]
 
-            curr_words, curr_word_tokens, curr_split_indices = get_curr_words()
+            curr_words, curr_word_tokens, curr_split_indices, pad_first_seg = get_curr_words()
 
             segment = timestamp_words()
             curr_words = segment['words']
             seg_words = [w['word'] for w in curr_words]
             seg_tokens = [w['tokens'] for w in curr_words]
             durations = np.array([w['end'] - w['start'] for w in curr_words]).round(3)
             nonzero_mask = durations > 0
@@ -645,16 +655,17 @@
     if not result:
         warnings.warn('Failed to align text.', stacklevel=2)
     if failure_count > max_fail:
         warnings.warn(f'Alignment aborted. Failed word percentage exceeded {failure_threshold * 100}% at '
                       f'{format_timestamp(seek_sample / SAMPLE_RATE)}.',
                       stacklevel=2)
     elif words:
+        last_ts_str = format_timestamp(result[-1]["end"] if result else 0)
         warnings.warn(f'Failed to align the last {len(words)}/{total_words} words after '
-                      f'{format_timestamp(result[-1]["end"])}.', stacklevel=2)
+                      f'{last_ts_str}.', stacklevel=2)
 
     if words and not remove_instant_words:
         final_total_duration = audio.get_duration(3)
         result.extend(
             [
                 dict(word=w, start=final_total_duration, end=final_total_duration, probability=0.0, tokens=wt)
                 for w, wt in zip(words, word_tokens)
```

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/audio/__init__.py` & `stable-ts-whisperless-2.17.1/stable_whisper/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/audio/demucs.py` & `stable-ts-whisperless-2.17.1/stable_whisper/audio/demucs.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/audio/dfnet.py` & `stable-ts-whisperless-2.17.1/stable_whisper/audio/dfnet.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/audio/noisereduce.py` & `stable-ts-whisperless-2.17.1/stable_whisper/audio/noisereduce.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/audio/output.py` & `stable-ts-whisperless-2.17.1/stable_whisper/audio/output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/audio/utils.py` & `stable-ts-whisperless-2.17.1/stable_whisper/audio/utils.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/decode.py` & `stable-ts-whisperless-2.17.1/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/default.py` & `stable-ts-whisperless-2.17.1/stable_whisper/default.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/non_whisper.py` & `stable-ts-whisperless-2.17.1/stable_whisper/non_whisper.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/quantization.py` & `stable-ts-whisperless-2.17.1/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/result.py` & `stable-ts-whisperless-2.17.1/stable_whisper/result.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/stabilization/__init__.py` & `stable-ts-whisperless-2.17.1/stable_whisper/stabilization/__init__.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/stabilization/nonvad.py` & `stable-ts-whisperless-2.17.1/stable_whisper/stabilization/nonvad.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/stabilization/silero_vad.py` & `stable-ts-whisperless-2.17.1/stable_whisper/stabilization/silero_vad.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/stabilization/utils.py` & `stable-ts-whisperless-2.17.1/stable_whisper/stabilization/utils.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/text_output.py` & `stable-ts-whisperless-2.17.1/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/timing.py` & `stable-ts-whisperless-2.17.1/stable_whisper/timing.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,16 @@
     return words, word_tokens
 
 
 def split_word_tokens(segments: List[dict],
                       tokenizer: "Tokenizer",
                       *,
                       padding: (str, int) = None,
-                      split_callback: Callable = None):
+                      split_callback: Callable = None,
+                      pad_first_seg: bool = True):
     if padding is not None:
         if isinstance(padding, str):
             padding = tokenizer.encode(padding)
         else:
             padding = [padding]
     tokens = []
     seg_indices = []
@@ -206,28 +207,40 @@
             split_callback(temp_word_tokens, tokenizer)
         )
         assert len(curr_words) == len(curr_word_tokens), \
             f'word count and token group count do not match, {len(curr_words)} and {len(curr_word_tokens)}'
         if (
                 padding is not None and
                 curr_word_tokens[0][0] != padding and
-                (len(tokens) == 0 or tokens[-1] != padding)
+                (len(tokens) == 0 or tokens[-1] != padding) and
+                (pad_first_seg or i != 0)
         ):
             tokens.extend(padding)
             words.append(None)
             word_tokens.append(padding)
         seg_indices.extend([i] * len(curr_words))
         tokens.extend(list(chain.from_iterable(curr_word_tokens)))
         words.extend(curr_words)
         word_tokens.extend(curr_word_tokens)
 
     return tokens, (words, word_tokens), seg_indices
 
 
-def pop_empty_alignment(alignment: List[WordTiming]):
+def pop_empty_alignment(alignment: List[WordTiming], seg_indices: Optional[List[int]] = None):
+    if seg_indices is not None:
+        seg_idx_pos = len(seg_indices)
+        empty_wts = {}
+        for i in reversed(range(len(alignment))):
+            assert seg_idx_pos != -1
+            if alignment[i].word is None:
+                empty_wts[seg_indices[seg_idx_pos]] = alignment.pop(i)
+            else:
+                seg_idx_pos -= 1
+        return empty_wts
+
     return list(reversed([alignment.pop(i) for i in reversed(range(len(alignment))) if alignment[i].word is None]))
 
 
 # modified version of whisper.timing.add_word_timestamps
 def add_word_timestamps_stable(
         *,
         segments: List[dict],
@@ -239,14 +252,15 @@
         append_punctuations: str = "\"'.。,，!！?？:：”)]}、",
         audio_features: torch.Tensor = None,
         ts_num: int = 0,
         ts_noise: float = None,
         min_word_dur: float = 0.1,
         split_callback: Callable = None,
         gap_padding: Optional[str] = ' ...',
+        pad_first_seg: bool = True,
         **kwargs,
 ):
     if len(segments) == 0:
         return
 
     if min_word_dur is None:
         min_word_dur = 0
@@ -257,39 +271,44 @@
     if append_punctuations is None:
         append_punctuations = "\"'.。,，!！?？:：”)]}、"
 
     def align():
         for seg in segments:
             seg['words'] = []
 
-        text_tokens, token_split, seg_indices = split_word_tokens(segments, tokenizer,
-                                                                  padding=gap_padding, split_callback=split_callback)
+        text_tokens, token_split, seg_indices = split_word_tokens(
+            segments,
+            tokenizer,
+            padding=gap_padding,
+            split_callback=split_callback,
+            pad_first_seg=pad_first_seg
+        )
 
         alignment = find_alignment_stable(model, tokenizer, text_tokens, mel, num_samples,
                                           **kwargs,
                                           token_split=token_split,
                                           audio_features=audio_features,
                                           ts_num=ts_num,
                                           ts_noise=ts_noise)
-        alt_beginning_alignment = pop_empty_alignment(alignment)
+        alt_beginning_alignment = pop_empty_alignment(alignment, seg_indices)
 
         merge_punctuations(alignment, prepend_punctuations, append_punctuations)
 
         time_offset = segments[0]["seek"]
 
         assert len(alignment) == len(seg_indices)
-        assert (gap_padding is None or len(segments) == len(alt_beginning_alignment))
+        assert (gap_padding is None or len(segments) == len(alt_beginning_alignment) + (1, 0)[pad_first_seg])
         for i, timing in zip(seg_indices, alignment):
             if len(timing.tokens) != 0:
                 start = timing.start
                 end = timing.end
                 if (
                         len(segments[i]['words']) == 0 and
                         ((end - start) < min_word_dur) and
-                        len(alt_beginning_alignment)
+                        i in alt_beginning_alignment
                 ):
                     start = alt_beginning_alignment[i].start
                 segments[i]['words'].append(
                     dict(
                         word=timing.word,
                         start=round(time_offset + start, 3),
                         end=round(time_offset + end, 3),
```

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/utils.py` & `stable-ts-whisperless-2.17.1/stable_whisper/utils.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/video_output.py` & `stable-ts-whisperless-2.17.1/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/whisper_compatibility.py` & `stable-ts-whisperless-2.17.1/stable_whisper/whisper_compatibility.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/cli.py` & `stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/cli.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/faster_whisper.py` & `stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/faster_whisper.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/hf_whisper.py` & `stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/hf_whisper.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.0/stable_whisper/whisper_word_level/original_whisper.py` & `stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/original_whisper.py`

 * *Files identical despite different names*

