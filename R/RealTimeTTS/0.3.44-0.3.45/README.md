# Comparing `tmp/RealTimeTTS-0.3.44.tar.gz` & `tmp/RealTimeTTS-0.3.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RealTimeTTS-0.3.44.tar", last modified: Mon Apr  8 00:16:32 2024, max compression
+gzip compressed data, was "RealTimeTTS-0.3.45.tar", last modified: Sat May  4 20:20:11 2024, max compression
```

## Comparing `RealTimeTTS-0.3.44.tar` & `RealTimeTTS-0.3.45.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 00:16:32.331675 RealTimeTTS-0.3.44/
--rw-rw-rw-   0        0        0    19233 2024-04-08 00:16:32.330673 RealTimeTTS-0.3.44/PKG-INFO
--rw-rw-rw-   0        0        0    18114 2024-04-08 00:07:46.000000 RealTimeTTS-0.3.44/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 00:16:32.329673 RealTimeTTS-0.3.44/RealTimeTTS.egg-info/
--rw-rw-rw-   0        0        0    19233 2024-04-08 00:16:32.000000 RealTimeTTS-0.3.44/RealTimeTTS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2024-04-08 00:16:32.000000 RealTimeTTS-0.3.44/RealTimeTTS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 00:16:32.000000 RealTimeTTS-0.3.44/RealTimeTTS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2024-04-08 00:16:32.000000 RealTimeTTS-0.3.44/RealTimeTTS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-08 00:16:32.000000 RealTimeTTS-0.3.44/RealTimeTTS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 00:16:32.242551 RealTimeTTS-0.3.44/RealtimeTTS/
--rw-rw-rw-   0        0        0      422 2023-12-28 10:50:12.000000 RealTimeTTS-0.3.44/RealtimeTTS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 00:16:32.325669 RealTimeTTS-0.3.44/RealtimeTTS/engines/
--rw-rw-rw-   0        0        0      397 2023-12-28 10:50:55.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/__init__.py
--rw-rw-rw-   0        0        0     9413 2024-03-15 16:54:18.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/azure_engine.py
--rw-rw-rw-   0        0        0     4490 2023-12-01 16:58:58.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/base_engine.py
--rw-rw-rw-   0        0        0   506471 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/chinese.json
--rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/coqui_default_voice.json
--rw-rw-rw-   0        0        0    38627 2024-04-07 23:58:16.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/coqui_engine.py
--rw-rw-rw-   0        0        0    10331 2023-12-01 16:58:58.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/elevenlabs_engine.py
--rw-rw-rw-   0        0        0   505425 2023-11-17 22:30:40.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/female.json
--rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/male.json
--rw-rw-rw-   0        0        0     3477 2023-12-28 10:13:43.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/openai_engine.py
--rw-rw-rw-   0        0        0     4834 2023-12-07 10:47:05.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/system_engine.py
--rw-rw-rw-   0        0        0    10159 2024-04-08 00:13:32.000000 RealTimeTTS-0.3.44/RealtimeTTS/stream_player.py
--rw-rw-rw-   0        0        0    27936 2024-04-08 00:03:01.000000 RealTimeTTS-0.3.44/RealtimeTTS/text_to_stream.py
--rw-rw-rw-   0        0        0    10179 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.44/RealtimeTTS/threadsafe_generators.py
--rw-rw-rw-   0        0        0       42 2024-04-08 00:16:32.331675 RealTimeTTS-0.3.44/setup.cfg
--rw-rw-rw-   0        0        0     1295 2024-04-08 00:16:23.000000 RealTimeTTS-0.3.44/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 00:16:32.327670 RealTimeTTS-0.3.44/tests/
--rw-rw-rw-   0        0        0     1361 2023-11-03 15:39:11.000000 RealTimeTTS-0.3.44/tests/test_callbacks.py
--rw-rw-rw-   0        0        0      637 2024-02-21 18:39:01.000000 RealTimeTTS-0.3.44/tests/test_on_audio_chunk_callback.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:20:11.892651 RealTimeTTS-0.3.45/
+-rw-rw-rw-   0        0        0    19619 2024-05-04 20:20:11.890650 RealTimeTTS-0.3.45/PKG-INFO
+-rw-rw-rw-   0        0        0    18500 2024-04-21 08:30:40.000000 RealTimeTTS-0.3.45/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 20:20:11.889649 RealTimeTTS-0.3.45/RealTimeTTS.egg-info/
+-rw-rw-rw-   0        0        0    19619 2024-05-04 20:20:11.000000 RealTimeTTS-0.3.45/RealTimeTTS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2024-05-04 20:20:11.000000 RealTimeTTS-0.3.45/RealTimeTTS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 20:20:11.000000 RealTimeTTS-0.3.45/RealTimeTTS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2024-05-04 20:20:11.000000 RealTimeTTS-0.3.45/RealTimeTTS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-04 20:20:11.000000 RealTimeTTS-0.3.45/RealTimeTTS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 20:20:11.789644 RealTimeTTS-0.3.45/RealtimeTTS/
+-rw-rw-rw-   0        0        0      422 2023-12-28 10:50:12.000000 RealTimeTTS-0.3.45/RealtimeTTS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:20:11.856701 RealTimeTTS-0.3.45/RealtimeTTS/engines/
+-rw-rw-rw-   0        0        0      397 2023-12-28 10:50:55.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/__init__.py
+-rw-rw-rw-   0        0        0     9455 2024-04-12 11:47:00.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/azure_engine.py
+-rw-rw-rw-   0        0        0     4490 2023-12-01 16:58:58.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/base_engine.py
+-rw-rw-rw-   0        0        0   506471 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/chinese.json
+-rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/coqui_default_voice.json
+-rw-rw-rw-   0        0        0    47582 2024-04-22 12:17:29.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/coqui_engine.py
+-rw-rw-rw-   0        0        0    10595 2024-04-28 18:45:00.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/elevenlabs_engine.py
+-rw-rw-rw-   0        0        0   505425 2023-11-17 22:30:40.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/female.json
+-rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/male.json
+-rw-rw-rw-   0        0        0     3477 2023-12-28 10:13:43.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/openai_engine.py
+-rw-rw-rw-   0        0        0     5340 2024-04-11 20:41:30.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/system_engine.py
+-rw-rw-rw-   0        0        0    10373 2024-05-04 20:11:35.000000 RealTimeTTS-0.3.45/RealtimeTTS/stream_player.py
+-rw-rw-rw-   0        0        0    29553 2024-05-04 20:09:08.000000 RealTimeTTS-0.3.45/RealtimeTTS/text_to_stream.py
+-rw-rw-rw-   0        0        0    10179 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.45/RealtimeTTS/threadsafe_generators.py
+-rw-rw-rw-   0        0        0       42 2024-05-04 20:20:11.892651 RealTimeTTS-0.3.45/setup.cfg
+-rw-rw-rw-   0        0        0     1295 2024-05-04 20:19:49.000000 RealTimeTTS-0.3.45/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:20:11.888647 RealTimeTTS-0.3.45/tests/
+-rw-rw-rw-   0        0        0     1361 2023-11-03 15:39:11.000000 RealTimeTTS-0.3.45/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0      637 2024-02-21 18:39:01.000000 RealTimeTTS-0.3.45/tests/test_on_audio_chunk_callback.py
```

### Comparing `RealTimeTTS-0.3.44/PKG-INFO` & `RealTimeTTS-0.3.45/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RealTimeTTS
-Version: 0.3.44
+Version: 0.3.45
 Summary: *Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.
 Home-page: https://github.com/KoljaB/RealTimeTTS
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,text-to-speech,TTS,streaming,audio,voice,synthesis,sentence-segmentation,low-latency,character-streaming,dynamic feedback,audio-output,text-input,TTS-engine,audio-playback,stream-player,sentence-fragment,audio-feedback,interactive,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,14 +26,16 @@
 
 *Easy to use, low-latency text-to-speech library for realtime applications*
 
 ## About the Project
 
 RealtimeTTS is a state-of-the-art text-to-speech (TTS) library designed for real-time applications. It stands out in its ability to convert text streams fast into high-quality auditory output with minimal latency. 
 
+> **Hint:** *<strong>Check out [Linguflex](https://github.com/KoljaB/Linguflex)</strong>, the original project from which RealtimeTTS is spun off. It lets you control your environment by speaking and is one of the most capable and sophisticated open-source assistants currently available.*
+
 https://github.com/KoljaB/RealtimeTTS/assets/7604638/87dcd9a5-3a4e-4f57-be45-837fc63237e7
 
 ## Key Features
 
 - **Low Latency**
   - almost instantaneous text-to-speech conversion
   - compatible with LLM outputs
@@ -44,28 +46,32 @@
 - **Multilingual**
 - **Robust and Reliable**: 
   - ensures continuous operation with a fallback mechanism
   - switches to alternative engines in case of disruptions guaranteeing consistent performance and reliability, which is vital for critical and professional use cases
 
 > **Hint**: *check out [RealtimeSTT](https://github.com/KoljaB/RealtimeSTT), the input counterpart of this library, for speech-to-text capabilities. Together, they form a powerful realtime audio wrapper around large language models.*
 
+## FAQ
+
+Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
+
 ## Updates
 
 Latest Version: v0.3.44
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
 - **Text-to-Speech Engines**
   - **OpenAIEngine**: OpenAI's TTS system offers 6 natural sounding voices.
   - **CoquiEngine**: High quality local neural TTS.
-  - **AzureEngine**: Microsoft's leading TTS technology. 250000 chars free per month.
+  - **AzureEngine**: Microsoft's leading TTS technology. 500000 chars free per month.
   - **ElevenlabsEngine**: Offer the best sounding voices available.
   - **SystemEngine**: Native engine for quick setup.
 
 - **Sentence Boundary Detection**
   - **NLTK Sentence Tokenizer**: Uses the Natural Language Toolkit's sentence tokenizer for precise and efficient sentence segmentation.
 
 *By using "industry standard" components RealtimeTTS offers a reliable, high-end technological foundation for developing advanced voice solutions.*
@@ -127,15 +133,15 @@
 ### CoquiEngine
 
 Delivers high quality, local, neural TTS with voice-cloning.  
 
 Downloads a neural TTS model first. In most cases it be fast enought for Realtime using GPU synthesis. Needs around 4-5 GB VRAM.
 
 - to clone a voice submit the filename of a wave file containing the source voice as "voice" parameter to the CoquiEngine constructor
-- in my experience voice cloning works best with a 22050 Hz mono 16bit WAV file containing a short (~10-30 sec) sample 
+- voice cloning works best with a 22050 Hz mono 16bit WAV file containing a short (~5-30 sec) sample 
 
 On most systems GPU support will be needed to run fast enough for realtime, otherwise you will experience stuttering.
 
 ## Quick Start
 
 Here's a basic usage example:
```

### Comparing `RealTimeTTS-0.3.44/README.md` & `RealTimeTTS-0.3.45/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 *Easy to use, low-latency text-to-speech library for realtime applications*
 
 ## About the Project
 
 RealtimeTTS is a state-of-the-art text-to-speech (TTS) library designed for real-time applications. It stands out in its ability to convert text streams fast into high-quality auditory output with minimal latency. 
 
+> **Hint:** *<strong>Check out [Linguflex](https://github.com/KoljaB/Linguflex)</strong>, the original project from which RealtimeTTS is spun off. It lets you control your environment by speaking and is one of the most capable and sophisticated open-source assistants currently available.*
+
 https://github.com/KoljaB/RealtimeTTS/assets/7604638/87dcd9a5-3a4e-4f57-be45-837fc63237e7
 
 ## Key Features
 
 - **Low Latency**
   - almost instantaneous text-to-speech conversion
   - compatible with LLM outputs
@@ -20,28 +22,32 @@
 - **Multilingual**
 - **Robust and Reliable**: 
   - ensures continuous operation with a fallback mechanism
   - switches to alternative engines in case of disruptions guaranteeing consistent performance and reliability, which is vital for critical and professional use cases
 
 > **Hint**: *check out [RealtimeSTT](https://github.com/KoljaB/RealtimeSTT), the input counterpart of this library, for speech-to-text capabilities. Together, they form a powerful realtime audio wrapper around large language models.*
 
+## FAQ
+
+Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
+
 ## Updates
 
 Latest Version: v0.3.44
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
 - **Text-to-Speech Engines**
   - **OpenAIEngine**: OpenAI's TTS system offers 6 natural sounding voices.
   - **CoquiEngine**: High quality local neural TTS.
-  - **AzureEngine**: Microsoft's leading TTS technology. 250000 chars free per month.
+  - **AzureEngine**: Microsoft's leading TTS technology. 500000 chars free per month.
   - **ElevenlabsEngine**: Offer the best sounding voices available.
   - **SystemEngine**: Native engine for quick setup.
 
 - **Sentence Boundary Detection**
   - **NLTK Sentence Tokenizer**: Uses the Natural Language Toolkit's sentence tokenizer for precise and efficient sentence segmentation.
 
 *By using "industry standard" components RealtimeTTS offers a reliable, high-end technological foundation for developing advanced voice solutions.*
@@ -103,15 +109,15 @@
 ### CoquiEngine
 
 Delivers high quality, local, neural TTS with voice-cloning.  
 
 Downloads a neural TTS model first. In most cases it be fast enought for Realtime using GPU synthesis. Needs around 4-5 GB VRAM.
 
 - to clone a voice submit the filename of a wave file containing the source voice as "voice" parameter to the CoquiEngine constructor
-- in my experience voice cloning works best with a 22050 Hz mono 16bit WAV file containing a short (~10-30 sec) sample 
+- voice cloning works best with a 22050 Hz mono 16bit WAV file containing a short (~5-30 sec) sample 
 
 On most systems GPU support will be needed to run fast enough for realtime, otherwise you will experience stuttering.
 
 ## Quick Start
 
 Here's a basic usage example:
```

### Comparing `RealTimeTTS-0.3.44/RealTimeTTS.egg-info/PKG-INFO` & `RealTimeTTS-0.3.45/RealTimeTTS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RealTimeTTS
-Version: 0.3.44
+Version: 0.3.45
 Summary: *Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.
 Home-page: https://github.com/KoljaB/RealTimeTTS
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,text-to-speech,TTS,streaming,audio,voice,synthesis,sentence-segmentation,low-latency,character-streaming,dynamic feedback,audio-output,text-input,TTS-engine,audio-playback,stream-player,sentence-fragment,audio-feedback,interactive,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,14 +26,16 @@
 
 *Easy to use, low-latency text-to-speech library for realtime applications*
 
 ## About the Project
 
 RealtimeTTS is a state-of-the-art text-to-speech (TTS) library designed for real-time applications. It stands out in its ability to convert text streams fast into high-quality auditory output with minimal latency. 
 
+> **Hint:** *<strong>Check out [Linguflex](https://github.com/KoljaB/Linguflex)</strong>, the original project from which RealtimeTTS is spun off. It lets you control your environment by speaking and is one of the most capable and sophisticated open-source assistants currently available.*
+
 https://github.com/KoljaB/RealtimeTTS/assets/7604638/87dcd9a5-3a4e-4f57-be45-837fc63237e7
 
 ## Key Features
 
 - **Low Latency**
   - almost instantaneous text-to-speech conversion
   - compatible with LLM outputs
@@ -44,28 +46,32 @@
 - **Multilingual**
 - **Robust and Reliable**: 
   - ensures continuous operation with a fallback mechanism
   - switches to alternative engines in case of disruptions guaranteeing consistent performance and reliability, which is vital for critical and professional use cases
 
 > **Hint**: *check out [RealtimeSTT](https://github.com/KoljaB/RealtimeSTT), the input counterpart of this library, for speech-to-text capabilities. Together, they form a powerful realtime audio wrapper around large language models.*
 
+## FAQ
+
+Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
+
 ## Updates
 
 Latest Version: v0.3.44
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
 - **Text-to-Speech Engines**
   - **OpenAIEngine**: OpenAI's TTS system offers 6 natural sounding voices.
   - **CoquiEngine**: High quality local neural TTS.
-  - **AzureEngine**: Microsoft's leading TTS technology. 250000 chars free per month.
+  - **AzureEngine**: Microsoft's leading TTS technology. 500000 chars free per month.
   - **ElevenlabsEngine**: Offer the best sounding voices available.
   - **SystemEngine**: Native engine for quick setup.
 
 - **Sentence Boundary Detection**
   - **NLTK Sentence Tokenizer**: Uses the Natural Language Toolkit's sentence tokenizer for precise and efficient sentence segmentation.
 
 *By using "industry standard" components RealtimeTTS offers a reliable, high-end technological foundation for developing advanced voice solutions.*
@@ -127,15 +133,15 @@
 ### CoquiEngine
 
 Delivers high quality, local, neural TTS with voice-cloning.  
 
 Downloads a neural TTS model first. In most cases it be fast enought for Realtime using GPU synthesis. Needs around 4-5 GB VRAM.
 
 - to clone a voice submit the filename of a wave file containing the source voice as "voice" parameter to the CoquiEngine constructor
-- in my experience voice cloning works best with a 22050 Hz mono 16bit WAV file containing a short (~10-30 sec) sample 
+- voice cloning works best with a 22050 Hz mono 16bit WAV file containing a short (~5-30 sec) sample 
 
 On most systems GPU support will be needed to run fast enough for realtime, otherwise you will experience stuttering.
 
 ## Quick Start
 
 Here's a basic usage example:
```

### Comparing `RealTimeTTS-0.3.44/RealTimeTTS.egg-info/SOURCES.txt` & `RealTimeTTS-0.3.45/RealTimeTTS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/engines/azure_engine.py` & `RealTimeTTS-0.3.45/RealtimeTTS/engines/azure_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,14 +208,15 @@
     def set_voice(self, voice: Union[str, AzureVoice]):
         """
         Sets the voice to be used for speech synthesis.
 
         Args:
             voice (Union[str, AzureVoice]): The voice to be used for speech synthesis.
         """
+        print(f"Setting voice: {voice}")
         if isinstance(voice, AzureVoice):
             self.voice_name = voice.full_name
             self.language = self.voice_name[:5]
         else:
             installed_voices = self.get_voices()
             for installed_voice in installed_voices:
                 if voice in installed_voice.full_name:
```

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/engines/base_engine.py` & `RealTimeTTS-0.3.45/RealtimeTTS/engines/base_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/engines/chinese.json` & `RealTimeTTS-0.3.45/RealtimeTTS/engines/chinese.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/engines/coqui_default_voice.json` & `RealTimeTTS-0.3.45/RealtimeTTS/engines/coqui_default_voice.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/engines/coqui_engine.py` & `RealTimeTTS-0.3.45/RealtimeTTS/engines/coqui_engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -71,15 +71,16 @@
                  use_mps=False,
                  use_deepspeed=False,
                  prepare_text_for_synthesis_callback=None,
                  add_sentence_filter=False,
                  pretrained=False,
                  comma_silence_duration=0.3,
                  sentence_silence_duration=0.6,
-                 default_silence_duration=0.3
+                 default_silence_duration=0.3,
+                 delay_per_character=0,
                  ):
         """
         Initializes a coqui voice realtime text to speech engine object.
 
         Args:
             model_name (str):
               Name of the coqui model to use.
@@ -155,14 +156,15 @@
         self.full_sentences = full_sentences
         self.use_mps = use_mps
         self.use_deepspeed = use_deepspeed
         self.add_sentence_filter = add_sentence_filter
         self.comma_silence_duration = comma_silence_duration
         self.sentence_silence_duration = sentence_silence_duration
         self.default_silence_duration = default_silence_duration
+        self.delay_per_character = delay_per_character
 
         self.cloning_reference_wav = voice
         self.speed = speed
         self.specific_model = specific_model
         if not local_models_path:
             local_models_path = os.environ.get("COQUI_MODEL_PATH")
             if local_models_path and len(local_models_path) > 0:
@@ -218,14 +220,15 @@
         self.output_worker_thread.start()
 
         self.main_synthesize_ready_event = mp.Event()
         self.parent_synthesize_pipe, child_synthesize_pipe = mp.Pipe()
         self.voices_list = []
         self.retrieve_coqui_voices()
 
+        log_level = logging.getLogger().getEffectiveLevel()
         self.synthesize_process = mp.Process(
             target=CoquiEngine._synthesize_worker, args=(
                 self.output_queue,
                 child_synthesize_pipe,
                 self.model_name,
                 self.cloning_reference_wav,
                 self.language,
@@ -246,15 +249,17 @@
                 self.model_path,
                 self.use_deepspeed,
                 self.voices_path,
                 self.voices_list,
                 self.pretrained,
                 self.comma_silence_duration,
                 self.sentence_silence_duration,
-                self.default_silence_duration
+                self.default_silence_duration,
+                self.delay_per_character,
+                log_level
             ))
         self.synthesize_process.start()
 
         logging.debug('Waiting for coqui model start')
         self.main_synthesize_ready_event.wait()
         logging.info('Coqui synthesis model ready')
 
@@ -285,28 +290,31 @@
             local_model_path,
             use_deepspeed,
             voices_path,
             predefined_voices,
             pretrained,
             comma_silence_duration,
             sentence_silence_duration,
-            default_silence_duration):
+            default_silence_duration,
+            delay_per_character,
+            log_level):
         """
         Worker process for the coqui text to speech synthesis model.
 
         Args:
             conn (multiprocessing.Connection):
               Connection to the parent process.
             model_name (str): Name of the coqui model to use.
             cloning_reference_wav (str):
               Name to the file containing the voice to clone.
             language (str): Language to use for the coqui model.
             ready_event (multiprocessing.Event):
               Event to signal when the model is ready.
         """
+        logging.basicConfig(level=log_level)
         sys.stdout = QueueWriter(output_queue)
 
         from TTS.utils.generic_utils import get_user_data_dir
         from TTS.config import load_config
         from TTS.tts.models import setup_model as setup_tts_model
         from TTS.tts.layers.xtts.xtts_manager import SpeakerManager
 
@@ -508,36 +516,63 @@
 
         ready_event.set()
 
         logging.info('Coqui text to speech synthesize model initialized successfully')
 
         try:
             while True:
-                message = conn.recv()  
+                try:
+                    message = conn.recv()
+                except EOFError:
+                    logging.error("EOFError caught, likely the parent process has closed the pipe", exc_info=True)
+                    break
+
                 command = message['command']
                 data = message['data']
 
                 if command == 'update_reference':
                     new_wav_path = data['cloning_reference_wav']
-                    logging.info(f'Updating reference WAV to {new_wav_path}')                    
+                    logging.info(f'Updating reference WAV to {new_wav_path}')
                     gpt_cond_latent, speaker_embedding = get_conditioning_latents(new_wav_path, tts)
+                    logging.debug("Sending message from worker process.")
                     conn.send(('success', 'Reference updated successfully'))
 
+                elif command == 'get_embeddings':
+                    new_wav_path = data['reference_wav']
+                    logging.info(f'Retrieving embedding for {new_wav_path}')
+                    try:
+                        gpt_cond_latent, speaker_embedding = tts.get_conditioning_latents(audio_path=new_wav_path, gpt_cond_len=30, max_ref_length=60)
+                        speaker_embedding = speaker_embedding.cpu().squeeze().half().tolist()
+                        logging.debug("Sending message from worker process.")
+                        conn.send(('success', speaker_embedding))
+                    except Exception as e:
+                        logging.debug("Sending message from worker process.")
+                        conn.send(('error', f'Could not retrieve embeddings, error: {e}'))
+
                 elif command == 'set_speed':
                     speed = data['speed']
+                    logging.debug("Sending message from worker process.")
                     conn.send(('success', 'Speed updated successfully'))
 
                 elif command == 'set_model':
                     checkpoint = data['checkpoint']
-                    logging.info(f'Updating model checkpoint to {checkpoint}')
-                    tts = load_model(checkpoint, tts)
-                    conn.send(('success', 'Model updated successfully'))
+                    try:
+                        logging.info(f'Updating model checkpoint to {checkpoint}')
+                        tts = load_model(checkpoint, tts)
+                    except Exception as e:
+                        logging.error("Error loading model", exc_info=True)
+                        logging.debug("Sending message from worker process.")
+                        conn.send(('error', f'Error updating model: {e}'))
+                    else:
+                        logging.debug("Sending message from worker process.")
+                        conn.send(('success', 'Model updated successfully'))
 
                 elif command == 'shutdown':
                     logging.info('Shutdown command received. Exiting worker process.')
+                    logging.debug("Sending message from worker process.")
                     conn.send(('shutdown', 'shutdown'))
                     break  # This exits the loop, effectively stopping the worker process.
 
                 elif command == 'synthesize':
 
                     text = data['text']
                     language = data['language']
@@ -547,133 +582,228 @@
                     print(f"XTTS Synthesizing: {text}")
                     time_start = time.time()
                     seconds_to_first_chunk = 0.0
                     full_generated_seconds = 0.0
                     raw_inference_start = 0.0
                     first_chunk_length_seconds = 0.0
 
-                    chunks = tts.inference_stream(
-                        text,
-                        language,
-                        gpt_cond_latent,
-                        speaker_embedding,
-                        stream_chunk_size=stream_chunk_size,
-                        overlap_wav_len=overlap_wav_len,
-                        temperature=temperature,
-                        length_penalty=length_penalty,
-                        repetition_penalty=repetition_penalty,
-                        top_k=top_k,
-                        top_p=top_p,
-                        speed=speed,
-                        enable_text_splitting=enable_text_splitting
-                    )
-
-                    if full_sentences:
-                        chunklist = []
-
-                        for i, chunk in enumerate(chunks):
-                            chunk = postprocess_wave(chunk)
-                            chunk_bytes = chunk.tobytes()
-                            chunklist.append(chunk_bytes)
-                            chunk_duration = len(chunk_bytes) / (4 * 24000)
-                            full_generated_seconds += chunk_duration
-                            if i == 0:
-                                first_chunk_length_seconds = chunk_duration
-                                raw_inference_start = time.time()
-                                seconds_to_first_chunk = raw_inference_start - time_start
-
-                        for i, chunk in enumerate(chunks):
-                            chunk = postprocess_wave(chunk)
-                            chunklist.append(chunk.tobytes())
+                    try:
+                        chunks = tts.inference_stream(
+                            text,
+                            language,
+                            gpt_cond_latent,
+                            speaker_embedding,
+                            stream_chunk_size=stream_chunk_size,
+                            overlap_wav_len=overlap_wav_len,
+                            temperature=temperature,
+                            length_penalty=length_penalty,
+                            repetition_penalty=repetition_penalty,
+                            top_k=top_k,
+                            top_p=top_p,
+                            speed=speed,
+                            enable_text_splitting=enable_text_splitting
+                        )
+                    except Exception as e:
+                        logging.error("Error perforing synthesis in tts.inference_stream", exc_info=True)
+                        logging.debug("Sending message from worker process.")
+                        conn.send(('error', f'Error during synthesis: {e}'))
+
+                    try:
+                        if full_sentences:
+                            chunklist = []
+
+                            for i, chunk in enumerate(chunks):
+                                chunk = postprocess_wave(chunk)
+                                chunk_bytes = chunk.tobytes()
+                                chunklist.append(chunk_bytes)
+                                chunk_duration = len(chunk_bytes) / (4 * 24000)
+                                full_generated_seconds += chunk_duration
+                                if i == 0:
+                                    first_chunk_length_seconds = chunk_duration
+                                    raw_inference_start = time.time()
+                                    seconds_to_first_chunk = raw_inference_start - time_start
+
+                            for chunk in chunklist:
+                                logging.debug("Sending message from worker process.")
+                                conn.send(('success', chunk))
+
+                        elif delay_per_character is not None and delay_per_character > 0:
+                            delayed_sent = False
+                            delay_time = delay_per_character * len(text)
+                            delay_time_end = time_start + delay_time
+
+                            chunklist = []
+
+                            print(f"Start time: {time_start}, delay_time: {delay_time}, delay_time_end: {delay_time_end}")
+
+                            for i, chunk in enumerate(chunks):
+                                
+                                delay_time_passed = time.time() > delay_time_end
+                                chunk = postprocess_wave(chunk)
+                                chunk_bytes = chunk.tobytes()
+                                chunk_duration = len(chunk_bytes) / (4 * 24000)
+                                full_generated_seconds += chunk_duration
+
+                                if i == 0:
+                                    first_chunk_length_seconds = chunk_duration
+                                    raw_inference_start = time.time()
+                                    seconds_to_first_chunk = raw_inference_start - time_start
+
+                                if delayed_sent:
+                                    logging.debug("Sending message from worker process.")
+                                    conn.send(('success', chunk_bytes))
+                                    continue
+
+                                chunklist.append(chunk_bytes)
+                                if delay_time_passed and not delayed_sent:
+                                    print(f"Delayed sending of {len(chunklist)} chunks")
+                                    delayed_sent = True
+                                    for chunk in chunklist:
+                                        logging.debug("Sending message from worker process.")
+                                        conn.send(('success', chunk))
+                                    chunklist = []
+
+                            if not delayed_sent:
+                                for chunk in chunklist:
+                                    logging.debug("Sending message from worker process.")
+                                    conn.send(('success', chunk))
 
-                        for chunk in chunklist:
-                            conn.send(('success', chunk))
-                    else:
-                        for i, chunk in enumerate(chunks):
-                            chunk = postprocess_wave(chunk)
-                            chunk_bytes = chunk.tobytes()
-                            conn.send(('success', chunk_bytes))
-                            chunk_duration = len(chunk_bytes) / (4 * 24000)  # 4 bytes per sample, 24000 Hz
-                            full_generated_seconds += chunk_duration
-                            if i == 0:
-                                first_chunk_length_seconds = chunk_duration
-                                raw_inference_start = time.time()
-                                seconds_to_first_chunk = raw_inference_start - time_start
-
-                    time_end = time.time()
-                    seconds = time_end - time_start
-
-                    if full_generated_seconds > 0 and (full_generated_seconds - first_chunk_length_seconds) > 0:
-
-                        realtime_factor = seconds / full_generated_seconds
-                        raw_inference_time = seconds - seconds_to_first_chunk
-                        raw_inference_factor = raw_inference_time / (full_generated_seconds - first_chunk_length_seconds) 
-
-                        # print(
-                        #     f"XTTS synthesized {full_generated_seconds:.2f}s"
-                        #     f" audio in {seconds:.2f}s"
-                        #     f" realtime factor: {realtime_factor:.2f}x"
-                        # )
-                        # print(
-                        #     f"seconds to first chunk: {seconds_to_first_chunk:.2f}s"
-                        #     f" raw_inference_factor: {raw_inference_factor:.2f}x"
-                        # )
-
-                    # Send silent audio
-                    sample_rate = config.audio.sample_rate
-
-                    end_sentence_delimeters = ".!?…。¡¿"
-                    mid_sentence_delimeters = ";:,\n()[]{}-“”„”—/|《》"
-
-                    if text[-1] in end_sentence_delimeters:
-                        silence_duration = sentence_silence_duration
-                    elif text[-1] in mid_sentence_delimeters:
-                        silence_duration = comma_silence_duration
-                    else:
-                        silence_duration = default_silence_duration
+                        else:
+                            for i, chunk in enumerate(chunks):
+                                chunk = postprocess_wave(chunk)
+                                chunk_bytes = chunk.tobytes()
+                                logging.debug("Sending message from worker process.")
+                                conn.send(('success', chunk_bytes))
+                                chunk_duration = len(chunk_bytes) / (4 * 24000)  # 4 bytes per sample, 24000 Hz
+                                full_generated_seconds += chunk_duration
+                                if i == 0:
+                                    first_chunk_length_seconds = chunk_duration
+                                    raw_inference_start = time.time()
+                                    seconds_to_first_chunk = raw_inference_start - time_start
+                    except Exception as e:
+                        logging.error("Error processing and sending chunks during synthesis process ", exc_info=True)
+                        logging.debug("Sending message from worker process.")
+                        conn.send(('error', f'Error during synthesis: {e}'))
+
+                    try:
+
+                        time_end = time.time()
+                        seconds = time_end - time_start
+
+                        if full_generated_seconds > 0 and (full_generated_seconds - first_chunk_length_seconds) > 0:
+
+                            realtime_factor = seconds / full_generated_seconds
+                            raw_inference_time = seconds - seconds_to_first_chunk
+                            raw_inference_factor = raw_inference_time / (full_generated_seconds - first_chunk_length_seconds) 
+
+                            if realtime_factor > 1.0:
+                                desired_delay_seconds = seconds - full_generated_seconds
+                                desired_ratio = desired_delay_seconds / full_generated_seconds
+                                desired_delay_chars = desired_ratio * len(text)
+                                delay_per_character = desired_delay_seconds / desired_delay_chars
+
+                                print(f"desired_delay_seconds = {desired_delay_seconds} "
+                                    f"desired_ratio = {desired_ratio} "
+                                    f"desired_delay_chars = {desired_delay_chars} "
+                                    f"delay_per_character = {delay_per_character}")
+
+                                # len(text) in seconds synthesized
+                                # hat to be faster for (seconds - full_generated_seconds) seconds => this is our delay
+                                # delay = seconds - full_generated_seconds
+                                # wieviel characters entspricht das?
+                                # 
+                                # len_text = len(text)
+                                # duration = 
+
+                                print(f"Realtime factor: {realtime_factor:.2f}x, suggested delay_per_character: {delay_per_character:.2f}")
+                            # print(f"full_generated_seconds: {full_generated_seconds}, first_chunk_length_seconds: {first_chunk_length_seconds}")
+                            # print(f"raw_inferece_time: {raw_inference_time}")
+
+                            logging.info(
+                                f"XTTS synthesized {full_generated_seconds:.2f}s"
+                                f" audio in {seconds:.2f}s"
+                                f" realtime factor: {realtime_factor:.2f}x"
+                                f" seconds to first chunk: {seconds_to_first_chunk:.2f}s"
+                                f" raw_inference_factor: {raw_inference_factor:.2f}x"
+                            )
+                    except Exception as e:
+                        logging.error("Error calculating realtime factor", exc_info=True)
+
+                    try:
+
+                        # Send silent audio
+                        sample_rate = config.audio.sample_rate
+
+                        end_sentence_delimeters = ".!?…。¡¿"
+                        mid_sentence_delimeters = ";:,\n()[]{}-“”„”—/|《》"
+
+                        if text[-1] in end_sentence_delimeters:
+                            silence_duration = sentence_silence_duration
+                        elif text[-1] in mid_sentence_delimeters:
+                            silence_duration = comma_silence_duration
+                        else:
+                            silence_duration = default_silence_duration
 
-                    silent_samples = int(sample_rate * silence_duration)
-                    silent_chunk = np.zeros(silent_samples, dtype=np.float32)
-                    conn.send(('success', silent_chunk.tobytes()))
+                        silent_samples = int(sample_rate * silence_duration)
+                        silent_chunk = np.zeros(silent_samples, dtype=np.float32)
 
-                    conn.send(('finished', ''))
+                        logging.debug("Sending message from worker process.")
+                        conn.send(('success', silent_chunk.tobytes()))
+                        logging.debug("Sending message from worker process.")
+                        conn.send(('finished', ''))
+
+                    except Exception as e:
+                        logging.error("Error sending silent chunk", exc_info=True)
+                        logging.debug("Sending message from worker process.")
+                        conn.send(('error', f'Error sending silent chunk: {e}'))
 
         except KeyboardInterrupt:
             logging.info("Keyboard interrupt received. "
                          "Exiting worker process.")
+            logging.debug("Sending message from worker process.")
             conn.send(('shutdown', 'shutdown'))
 
         except Exception as e:
-            logging.error(f"General synthesis error: {e} occured in "
-                          "synthesize worker thread of coqui engine.")
-
-            tb_str = traceback.format_exc()
-            print(f"Traceback: {tb_str}")
-            print(f"Error: {e}")
-
-            conn.send(('error', str(e)))
+            logging.error("Caught an exception in _synthesize_worker", exc_info=True)
+            traceback_str = traceback.format_exc()
+            print(f"Traceback in _synthesize_worker: {traceback_str}")
+            try:
+                logging.debug("Sending message from worker process.")
+                conn.send(('error', str(e)))
+            except Exception as send_error:
+                logging.error("Failed to send error message to parent process", exc_info=True)
 
         sys.stdout = sys.__stdout__
 
     def send_command(self, command, data):
         """
-        Send a command to the worker process.
+        Send a command to the worker process, handling closed pipes.
         """
-        message = {'command': command, 'data': data}
-        self.parent_synthesize_pipe.send(message)            
+        try:
+            message = {'command': command, 'data': data}
+            logging.debug("Sending message to worker process.")
+            self.parent_synthesize_pipe.send(message)
+            return True
+        except BrokenPipeError:
+            logging.error("Failed to send command: pipe is closed.")
+            return False
+        except Exception as e:
+            logging.error(f"Failed to send command due to: {e}")
+            return False
 
     def set_cloning_reference(self, cloning_reference_wav: str):
         """
         Send an 'update_reference' command and wait for a response.
         """
         if not isinstance(cloning_reference_wav, list):
             cloning_reference_wav = [cloning_reference_wav]        
         self.send_command('update_reference', {'cloning_reference_wav': cloning_reference_wav})
 
         # Wait for the response from the worker process
+        logging.debug("Receiving message from worker process.")
         status, result = self.parent_synthesize_pipe.recv()
         if status == 'success':
             logging.info('Reference WAV updated successfully')
         else:
             logging.error(f'Error updating reference WAV: {cloning_reference_wav}')
 
         return status, result
@@ -681,14 +811,15 @@
     def set_speed(self, speed: float):
         """
         Sets the speed of the speech synthesis.
         """
         self.send_command('set_speed', {'speed': speed})
 
         # Wait for the response from the worker process
+        logging.debug("Receiving message from worker process.")
         status, result = self.parent_synthesize_pipe.recv()
         if status == 'success':
             logging.info('Speed updated successfully')
         else:
             logging.error('Error updating speed')
 
         return status, result
@@ -786,23 +917,25 @@
 
             if len(text) < 1:
                 return
 
             data = {'text': text, 'language': self.language}
             self.send_command('synthesize', data)
 
+            logging.debug("Receiving message from worker process.")
             status, result = self.parent_synthesize_pipe.recv()
 
             while not 'finished' in status:
                 if 'shutdown' in status or 'error' in status:
-                    if 'error' in status:
-                        logging.error(f'Error synthesizing text: {text}')
-                        logging.error(f'Error: {result}')
+                    logging.error(f'Error synthesizing text: {text}')
+                    logging.error(f'Error: {result}')
                     return False
                 self.queue.put(result)
+                
+                logging.debug("Receiving message from worker process.")
                 status, result = self.parent_synthesize_pipe.recv()
 
             return True
 
     @staticmethod
     def download_file(url, destination):
         response = requests.get(url, stream=True)
@@ -845,14 +978,30 @@
                 CoquiEngine.download_file(url, file_path)
                 logging.info(f"{file_name} downloaded successfully.")
             else:
                 logging.info(f"{file_name} exists in {file_path} (no download).")
 
         return model_folder
 
+    def get_embeddings(self, path_to_wave):
+        """
+        Gets speaker embeddings for the given wave file.        
+        """
+        self.send_command('get_embeddings', {'reference_wav': path_to_wave})
+
+        # Wait for the response from the worker process
+        logging.debug("Receiving message from worker process.")
+        status, result = self.parent_synthesize_pipe.recv()
+        if status == 'success':
+            logging.info('Retrieved embedding successfully')
+        else:
+            logging.error(f'Error retrieving embedding for: {path_to_wave}')
+
+        return result
+
     def get_voices(self):
         """
         Retrieves the installed voices available for the Coqui TTS engine.
         """
 
         voice_objects = []
         voices_appended = []
@@ -912,14 +1061,15 @@
         self.send_command('shutdown', {})
 
         self.output_queue.put("STOP")
         self.output_worker_thread.join()
 
         # Wait for the worker process to acknowledge the shutdown
         try:
+            logging.debug("Receiving message from worker process.")
             status, _ = self.parent_synthesize_pipe.recv()
             if 'shutdown' in status:
                 logging.info('Worker process acknowledged shutdown')
         except EOFError:
             # Pipe was closed, meaning the process is already down
             logging.warning('Worker process pipe was closed before shutdown acknowledgement')
```

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/engines/elevenlabs_engine.py` & `RealTimeTTS-0.3.45/RealtimeTTS/engines/elevenlabs_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         self.clarity = clarity
         self.stability = stability
         self.style_exxageration = style_exxageration
         self.model = model
         self.pause_event = threading.Event()
         self.immediate_stop = threading.Event()
         self.on_audio_chunk = None
+        self.muted = False
         self.on_playback_started = False
 
         self.set_api_key(api_key)
         
     def post_init(self):
         """ Information that this engine can handle generators directly """ 
         self.can_consume_generators = True
@@ -78,14 +79,18 @@
         """        
         return pyaudio.paCustomFormat, -1, -1
     
     def pause(self):
         """Pauses playback of the synthesized audio stream (won't work properly with elevenlabs)."""
         self.pause_event.set()
 
+    def set_muted(self, muted: bool):
+        """Mutes the audio stream."""
+        self.muted = muted
+
     def resume(self):
         """Resumes a previously paused playback of the synthesized audio stream (won't work properly with elevenlabs)."""
         self.pause_event.clear()
 
     def stop(self):
         """Stops the playback of the synthesized audio stream immediately."""
         self.mpv_process.terminate()
@@ -159,41 +164,44 @@
             message = (
                 "mpv not found, necessary to stream audio. "
                 "On mac you can install it with 'brew install mpv'. "
                 "On linux and windows you can install it from https://mpv.io/"
             )
             raise ValueError(message)
 
-        mpv_command = ["mpv", "--no-cache", "--no-terminal", "--", "fd://0"]
-        self.mpv_process = subprocess.Popen(
-            mpv_command,
-            stdin=subprocess.PIPE,
-            stdout=subprocess.DEVNULL,
-            stderr=subprocess.DEVNULL,
-        )
+        if not self.muted:
+            mpv_command = ["mpv", "--no-cache", "--no-terminal", "--", "fd://0"]
+            self.mpv_process = subprocess.Popen(
+                mpv_command,
+                stdin=subprocess.PIPE,
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
+            )
 
         audio = b""
 
         try: 
             for chunk in audio_stream:
                 if chunk is not None:
                     if not self.on_playback_started and self.on_playback_start:
                         self.on_playback_start()
                     self.on_playback_started = True
-                    self.mpv_process.stdin.write(chunk)
-                    self.mpv_process.stdin.flush()
+                    if not self.muted:
+                        self.mpv_process.stdin.write(chunk)
+                        self.mpv_process.stdin.flush()
                     audio += chunk
                     if self.on_audio_chunk: 
                         self.on_audio_chunk(chunk)
         except BrokenPipeError:
             pass
 
-        if self.mpv_process.stdin:
-            self.mpv_process.stdin.close()
-        self.mpv_process.wait()
+        if not self.muted:
+            if self.mpv_process.stdin:
+                self.mpv_process.stdin.close()
+            self.mpv_process.wait()
 
         return audio            
     
     def get_voices(self):
         """
         Retrieves the voices available from the Elevenlabs voice source.
 
@@ -236,15 +244,15 @@
             for installed_voice in installed_voices:
                 if voice in installed_voice.name:
                     logging.info(f"Setting voice to {installed_voice.name}")
                     self.voice_name = installed_voice.name
                     self.id = installed_voice.voice_id
                     self.category = installed_voice.category
                     return
-                
+
         logging.warning(f"Voice {voice} not found.")
 
     def set_voice_parameters(self, **voice_parameters):
         """
         Sets the voice parameters to be used for speech synthesis.
 
         Args:
```

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/engines/female.json` & `RealTimeTTS-0.3.45/RealtimeTTS/engines/female.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/engines/male.json` & `RealTimeTTS-0.3.45/RealtimeTTS/engines/male.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/engines/openai_engine.py` & `RealTimeTTS-0.3.45/RealtimeTTS/engines/openai_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/engines/system_engine.py` & `RealTimeTTS-0.3.45/RealtimeTTS/engines/system_engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 from .base_engine import BaseEngine
 from pydub.utils import mediainfo
 from pydub import AudioSegment
 from typing import Union
+import subprocess
+import platform
 import tempfile
 import pyaudio
 import pyttsx3
 import wave
 import os
 
-SYNTHESIS_FILE = 'system_speech_synthesis.wav' 
+IS_MAC = platform.system() == "Darwin"
+
+if IS_MAC:
+    SYNTHESIS_FILE = "system_speech_synthesis.aiff"
+    DEFAULT_VOICE = "Alex"
+else:
+    SYNTHESIS_FILE = "system_speech_synthesis.wav"
+    DEFAULT_VOICE = "Zira"
 
 
 class SystemVoice:
     def __init__(self, name, id):
         self.name = name
         self.id = id
 
     def __repr__(self):
         return self.name
-        #return f"<Voice(name={self.name})>"
 
 
 class SystemEngine(BaseEngine):
 
     def __init__(self, 
-                 voice: str = "Zira",
+                 voice: str = DEFAULT_VOICE,
                  print_installed_voices: bool = False):
         """
         Initializes a system realtime text to speech engine object.
 
         Args:
             voice (str, optional): Voice name. Defaults to "Zira".
             print_installed_voices (bool, optional): Indicates if the list of installed voices should be printed. Defaults to False.
@@ -61,16 +69,24 @@
         """
         Synthesizes text to audio stream.
 
         Args:
             text (str): Text to synthesize.
         """
 
-        self.engine.save_to_file(text, self.file_path)
-        self.engine.runAndWait()
+        if IS_MAC:
+            # Output file path
+            output_file = SYNTHESIS_FILE
+
+            # Synthesize speech and save to file
+            subprocess.call(['say', '-v', self.voice, '-o', output_file, text])
+
+        else:
+            self.engine.save_to_file(text, self.file_path)
+            self.engine.runAndWait()
 
         # Get media info of the file
         info = mediainfo(self.file_path)
 
         # Check if the file format is AIFF and convert to WAV if necessary
         if info['format_name'] == 'aiff':
             audio = AudioSegment.from_file(self.file_path, format="aiff")
@@ -110,22 +126,24 @@
     def set_voice(self, voice: Union[str, SystemVoice]):
         """
         Sets the voice to be used for speech synthesis.
 
         Args:
             voice (Union[str, SystemVoice]): The voice to be used for speech synthesis.
         """
-        if isinstance(voice, SystemVoice):
-            self.engine.setProperty('voice', voice.id)            
-        else:
-            installed_voices = self.engine.getProperty('voices')
-            if not voice is None:
-                for installed_voice in installed_voices:
-                    if voice in installed_voice.name:
-                        self.engine.setProperty('voice', installed_voice.id)
+        if not IS_MAC:
+            if isinstance(voice, SystemVoice):
+                self.engine.setProperty('voice', voice.id)            
+            else:
+                installed_voices = self.engine.getProperty('voices')
+                if not voice is None:
+                    for installed_voice in installed_voices:
+                        if voice in installed_voice.name:
+                            self.engine.setProperty('voice', installed_voice.id)
+        self.voice = voice
 
     def set_voice_parameters(self, **voice_parameters):
         """
         Sets the voice parameters to be used for speech synthesis.
 
         Args:
             **voice_parameters: The voice parameters to be used for speech synthesis.
```

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/stream_player.py` & `RealTimeTTS-0.3.45/RealtimeTTS/stream_player.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
             self.stream.stop_stream()
 
     def close_stream(self):
         """Closes the audio stream."""
         if self.stream:
             self.stop_stream()
             self.stream.close()
+            self.stream = None
 
     def is_stream_active(self) -> bool:
         """
         Checks if the audio stream is active.
 
         Returns:
             bool: True if the stream is active, False otherwise.
@@ -219,24 +220,25 @@
             chunk = segment.raw_data
 
         sub_chunk_size = 1024
 
         for i in range(0, len(chunk), sub_chunk_size):
             sub_chunk = chunk[i:i + sub_chunk_size]
 
+            # print("Playing/yielding chunk")
+            if not self.first_chunk_played and self.on_playback_start:
+                self.on_playback_start()
+                self.first_chunk_played = True
+
             if not self.muted:
                 self.audio_stream.stream.write(sub_chunk)
 
             if self.on_audio_chunk:
                 self.on_audio_chunk(sub_chunk)
 
-            if not self.first_chunk_played and self.on_playback_start:
-                self.on_playback_start()
-                self.first_chunk_played = True
-
             # Pause playback if the event is set
             while self.pause_event.is_set():
                 time.sleep(0.01)
 
             if self.immediate_stop.is_set():
                 break
 
@@ -271,18 +273,22 @@
         )
         return total_samples / self.audio_stream.config.rate
 
     def start(self):
         """Starts audio playback."""
         self.first_chunk_played = False
         self.playback_active = True
-        self.audio_stream.open_stream()
+        if not self.audio_stream.stream:
+            self.audio_stream.open_stream()
+
         self.audio_stream.start_stream()
-        self.playback_thread = threading.Thread(target=self._process_buffer)
-        self.playback_thread.start()
+
+        if not self.playback_thread or not self.playback_thread.is_alive():
+            self.playback_thread = threading.Thread(target=self._process_buffer)
+            self.playback_thread.start()
 
     def stop(self, immediate: bool = False):
         """
         Stops audio playback.
 
         Args:
             immediate (bool): If True, stops playback immediately
```

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/text_to_stream.py` & `RealTimeTTS-0.3.45/RealtimeTTS/text_to_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         self.output_wavfile = None
         self.chunk_callback = None
         self.wf = None
         self.abort_events = []
         self.tokenizer = tokenizer
         self.language = language
         self.player = None
+        self.play_lock = threading.Lock()
+        self.is_playing_flag = False
 
         self._create_iterators()
 
         logging.info(f"Initializing tokenizer {tokenizer} "
                      f"for language {language}")
         s2s.init_tokenizer(tokenizer, language)
 
@@ -162,19 +164,30 @@
                    muted: bool = False,
                    sentence_fragment_delimiters: str = ".?!;:,\n…)]}。-",
                    force_first_fragment_after_words=15,
                    ):
         """
         Async handling of text to audio synthesis, see play() method.
         """
-        self.stream_running = True
+        if not self.is_playing_flag:
+            self.is_playing_flag = True
+            # Pass additional parameter to differentiate external call
+            args = (fast_sentence_fragment, buffer_threshold_seconds, minimum_sentence_length, 
+                    minimum_first_fragment_length, log_synthesized_text, reset_generated_text, 
+                    output_wavfile, on_sentence_synthesized, on_audio_chunk, tokenizer, 
+                    language, context_size, muted, sentence_fragment_delimiters, 
+                    force_first_fragment_after_words, True)
+            self.play_thread = threading.Thread(target=self.play, args=args)
+            self.play_thread.start()
+        else:
+            logging.warning("play_async() called while already playing audio, skipping")
 
-        self.play_thread = threading.Thread(target=self.play, args=(fast_sentence_fragment, buffer_threshold_seconds, minimum_sentence_length, minimum_first_fragment_length, log_synthesized_text, reset_generated_text, output_wavfile, on_sentence_synthesized, on_audio_chunk, tokenizer, language, context_size, muted, sentence_fragment_delimiters, force_first_fragment_after_words))
-        self.play_thread.daemon = True
-        self.play_thread.start()
+        # self.play_thread = threading.Thread(target=self.play, args=(fast_sentence_fragment, buffer_threshold_seconds, minimum_sentence_length, minimum_first_fragment_length, log_synthesized_text, reset_generated_text, output_wavfile, on_sentence_synthesized, on_audio_chunk, tokenizer, language, context_size, muted, sentence_fragment_delimiters, force_first_fragment_after_words))
+        # self.play_thread.daemon = True
+        # self.play_thread.start()
 
     def play(
             self,
             fast_sentence_fragment: bool = True,
             buffer_threshold_seconds: float = 0.0,
             minimum_sentence_length: int = 10,
             minimum_first_fragment_length: int = 10,
@@ -185,14 +198,15 @@
             on_audio_chunk=None,
             tokenizer: str = "nltk",
             language: str = "en",
             context_size: int = 12,
             muted: bool = False,
             sentence_fragment_delimiters: str = ".?!;:,\n…)]}。-",
             force_first_fragment_after_words=15,
+            is_external_call=True
             ):
         """
         Handles the synthesis of text to audio.
         Plays the audio stream and waits until it is finished playing.
         If the engine can't consume generators, it utilizes a player.
 
         Args:
@@ -214,28 +228,37 @@
         - sentence_fragment_delimiters (str): A string of characters that are
             considered sentence delimiters. Default is ".?!;:,\n…)]}。-".
         - force_first_fragment_after_words (int): The number of words after
             which the first sentence fragment is forced to be yielded.
             Default is 15 words.
         """
 
+        if is_external_call:
+            if not self.play_lock.acquire(blocking=False):
+                logging.warning("play() called while already playing audio, skipping")
+                return
+
+        self.is_playing_flag = True
+
         # Log the start of the stream
         logging.info(f"stream start")
 
         tokenizer = tokenizer if tokenizer else self.tokenizer 
         language = language if language else self.language
 
         # Set the stream_running flag to indicate the stream is active
         self.stream_start_time = time.time()
         self.stream_running = True
         abort_event = threading.Event()
         self.abort_events.append(abort_event)
 
         if self.player:
             self.player.mute(muted)
+        elif hasattr(self.engine, "set_muted"):
+            self.engine.set_muted(muted)
 
         self.output_wavfile = output_wavfile
         self.chunk_callback = on_audio_chunk
 
         if output_wavfile:
             if self._is_engine_mpeg():
                 self.wf = open(output_wavfile, 'wb')
@@ -268,14 +291,15 @@
                 self.stream_running = False
                 logging.info("stream stop")
 
                 # Accumulate the generated text and reset the character iterators
                 self.generated_text += self.char_iter.iterated_text
 
                 self._create_iterators()
+                self.is_playing_flag = False
         else:
             try:
                 # Start the audio player to handle playback
                 self.player.start()
                 self.player.on_audio_chunk = self._on_audio_chunk
 
                 # Generate sentences from the characters
@@ -335,31 +359,32 @@
                 worker_thread.start()      
 
                 # Iterate through the synthesized chunks and feed them to the engine for audio synthesis
                 for sentence in chunk_generator:
                     if abort_event.is_set():
                         break
                     sentence = sentence.strip()
-                    sentence_queue.put(sentence)
-                    if not self.stream_running:
-                        break
+                    if sentence:
+                        sentence_queue.put(sentence)
+                    else:
+                        continue  # Skip empty sentences
 
                 # Signal to the worker to stop
                 sentence_queue.put(None)
-                worker_thread.join()   
+                worker_thread.join()
 
             except Exception as e:
                 logging.warning(f"error in play() with engine {self.engine.engine_name}: {e}")
                 tb_str = traceback.format_exc()
                 print (f"Traceback: {tb_str}")
                 print (f"Error: {e}")
 
             finally:
                 try:
-                   
+                
                     self.player.stop()
 
                     self.abort_events.remove(abort_event)
                     self.stream_running = False
                     logging.info("stream stop")
 
                     self.output_wavfile = None
@@ -382,19 +407,25 @@
                     reset_generated_text=False,
                     output_wavfile=output_wavfile,
                     on_sentence_synthesized=on_sentence_synthesized,
                     on_audio_chunk=on_audio_chunk,
                     tokenizer=tokenizer,
                     language=language,
                     context_size=context_size,
-                    muted=muted)
-            else:
+                    muted=muted,
+                    sentence_fragment_delimiters=sentence_fragment_delimiters,
+                    force_first_fragment_after_words=force_first_fragment_after_words,
+                    is_external_call=False)
+
+            if is_external_call:
                 if self.on_audio_stream_stop:
                     self.on_audio_stream_stop()
 
+                self.is_playing_flag = False
+                self.play_lock.release()
 
     def pause(self):
         """
         Pauses playback of the synthesized audio stream (won't work properly with elevenlabs).
         """
         if self.is_playing():
             logging.info("stream pause")
@@ -515,15 +546,15 @@
 
         # If an on_text_stream_stop callback is defined, invoke it to signal the end of the text stream
         if self.on_text_stream_stop:
             self.on_text_stream_stop()
 
         # If log_characters flag is True, print a new line for better log readability
         if self.log_characters:
-            print()    
+            print()
 
         self._create_iterators()
 
 
     def _create_iterators(self):
         """
         Creates iterators required for text-to-audio streaming.
```

### Comparing `RealTimeTTS-0.3.44/RealtimeTTS/threadsafe_generators.py` & `RealTimeTTS-0.3.45/RealtimeTTS/threadsafe_generators.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.44/setup.py` & `RealTimeTTS-0.3.45/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Read requirements.txt
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="RealTimeTTS",
-    version="0.3.44",
+    version="0.3.45",
     author="Kolja Beigel",
     author_email="kolja.beigel@web.de",
     description="*Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KoljaB/RealTimeTTS",
     packages=setuptools.find_packages(),
```

### Comparing `RealTimeTTS-0.3.44/tests/test_callbacks.py` & `RealTimeTTS-0.3.45/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.44/tests/test_on_audio_chunk_callback.py` & `RealTimeTTS-0.3.45/tests/test_on_audio_chunk_callback.py`

 * *Files identical despite different names*

