# Comparing `tmp/whisperplus-0.2.8.tar.gz` & `tmp/whisperplus-0.2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisperplus-0.2.8.tar", last modified: Thu May  2 22:18:32 2024, max compression
+gzip compressed data, was "whisperplus-0.2.8.1.tar", last modified: Sat May  4 13:44:44 2024, max compression
```

## Comparing `whisperplus-0.2.8.tar` & `whisperplus-0.2.8.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-02 22:18:32.113359 whisperplus-0.2.8/
--rw-r--r--   0 kadirnar   (501) staff       (20)    11357 2024-04-29 20:18:01.000000 whisperplus-0.2.8/LICENSE
--rw-r--r--   0 kadirnar   (501) staff       (20)       25 2024-04-29 20:18:01.000000 whisperplus-0.2.8/MANIFEST.in
--rw-r--r--   0 kadirnar   (501) staff       (20)     5514 2024-05-02 22:18:32.113509 whisperplus-0.2.8/PKG-INFO
--rw-r--r--   0 kadirnar   (501) staff       (20)     5204 2024-05-02 22:01:09.000000 whisperplus-0.2.8/README.md
--rw-r--r--   0 kadirnar   (501) staff       (20)      395 2024-05-02 22:01:13.000000 whisperplus-0.2.8/requirements.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)      748 2024-05-02 22:18:32.113832 whisperplus-0.2.8/setup.cfg
--rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-29 20:18:01.000000 whisperplus-0.2.8/setup.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-02 22:18:32.110502 whisperplus-0.2.8/whisperplus/
--rw-r--r--   0 kadirnar   (501) staff       (20)      658 2024-05-02 22:18:20.000000 whisperplus-0.2.8/whisperplus/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     7729 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/app.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-02 22:18:32.112878 whisperplus-0.2.8/whisperplus/pipelines/
--rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     3123 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/autollm_chatbot.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     5543 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/lancedb_chatbot.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     2487 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/long_text_summarization.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1380 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/summarization.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-30 23:17:02.000000 whisperplus-0.2.8/whisperplus/pipelines/text2speech.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     2773 2024-05-02 22:00:09.000000 whisperplus-0.2.8/whisperplus/pipelines/whisper.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     3492 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/whisper_autocaption.py
--rw-r--r--   0 kadirnar   (501) staff       (20)    10897 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/whisper_diarize.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-02 22:18:32.113251 whisperplus-0.2.8/whisperplus/utils/
--rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/utils/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1403 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/utils/download_utils.py
--rw-r--r--   0 kadirnar   (501) staff       (20)      532 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/utils/text_utils.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-02 22:18:32.111207 whisperplus-0.2.8/whisperplus.egg-info/
--rw-r--r--   0 kadirnar   (501) staff       (20)     5514 2024-05-02 22:18:32.000000 whisperplus-0.2.8/whisperplus.egg-info/PKG-INFO
--rw-r--r--   0 kadirnar   (501) staff       (20)      740 2024-05-02 22:18:32.000000 whisperplus-0.2.8/whisperplus.egg-info/SOURCES.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)        1 2024-05-02 22:18:32.000000 whisperplus-0.2.8/whisperplus.egg-info/dependency_links.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)      395 2024-05-02 22:18:32.000000 whisperplus-0.2.8/whisperplus.egg-info/requires.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)       12 2024-05-02 22:18:32.000000 whisperplus-0.2.8/whisperplus.egg-info/top_level.txt
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-04 13:44:44.024095 whisperplus-0.2.8.1/
+-rw-r--r--   0 kadirnar   (501) staff       (20)    11357 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/LICENSE
+-rw-r--r--   0 kadirnar   (501) staff       (20)       25 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/MANIFEST.in
+-rw-r--r--   0 kadirnar   (501) staff       (20)     6101 2024-05-04 13:44:44.024251 whisperplus-0.2.8.1/PKG-INFO
+-rw-r--r--   0 kadirnar   (501) staff       (20)     5789 2024-05-04 11:16:41.000000 whisperplus-0.2.8.1/README.md
+-rw-r--r--   0 kadirnar   (501) staff       (20)      378 2024-05-04 11:16:41.000000 whisperplus-0.2.8.1/requirements.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)      748 2024-05-04 13:44:44.024558 whisperplus-0.2.8.1/setup.cfg
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/setup.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-04 13:44:44.021871 whisperplus-0.2.8.1/whisperplus/
+-rw-r--r--   0 kadirnar   (501) staff       (20)      660 2024-05-04 13:44:24.000000 whisperplus-0.2.8.1/whisperplus/__init__.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     7729 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/whisperplus/app.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-04 13:44:44.023642 whisperplus-0.2.8.1/whisperplus/pipelines/
+-rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/whisperplus/pipelines/__init__.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     3123 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/whisperplus/pipelines/autollm_chatbot.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     5543 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/whisperplus/pipelines/lancedb_chatbot.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     2487 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/whisperplus/pipelines/long_text_summarization.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1380 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/whisperplus/pipelines/summarization.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-30 23:17:02.000000 whisperplus-0.2.8.1/whisperplus/pipelines/text2speech.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     2753 2024-05-04 13:38:51.000000 whisperplus-0.2.8.1/whisperplus/pipelines/whisper.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     3492 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/whisperplus/pipelines/whisper_autocaption.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)    10897 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/whisperplus/pipelines/whisper_diarize.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1276 2024-05-04 13:38:51.000000 whisperplus-0.2.8.1/whisperplus/test.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-04 13:44:44.023998 whisperplus-0.2.8.1/whisperplus/utils/
+-rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/whisperplus/utils/__init__.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1403 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/whisperplus/utils/download_utils.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)      532 2024-04-29 20:18:01.000000 whisperplus-0.2.8.1/whisperplus/utils/text_utils.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-04 13:44:44.022481 whisperplus-0.2.8.1/whisperplus.egg-info/
+-rw-r--r--   0 kadirnar   (501) staff       (20)     6101 2024-05-04 13:44:43.000000 whisperplus-0.2.8.1/whisperplus.egg-info/PKG-INFO
+-rw-r--r--   0 kadirnar   (501) staff       (20)      760 2024-05-04 13:44:43.000000 whisperplus-0.2.8.1/whisperplus.egg-info/SOURCES.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)        1 2024-05-04 13:44:43.000000 whisperplus-0.2.8.1/whisperplus.egg-info/dependency_links.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)      378 2024-05-04 13:44:43.000000 whisperplus-0.2.8.1/whisperplus.egg-info/requires.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)       12 2024-05-04 13:44:43.000000 whisperplus-0.2.8.1/whisperplus.egg-info/top_level.txt
```

### Comparing `whisperplus-0.2.8/LICENSE` & `whisperplus-0.2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/PKG-INFO` & `whisperplus-0.2.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisperplus
-Version: 0.2.8
+Version: 0.2.8.1
 Summary: WhisperPlus: A Python library for WhisperPlus API.
 Home-page: https://github.com/kadirnar/whisperplus
 Author: kadirnar
 Author-email: kadir.nar@hotmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,15 +24,15 @@
     <a href="https://huggingface.co/spaces/ArtGAN/Audio-WebUI"><img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="HuggingFace Spaces"></a>
 </div>
 </div>
 
 ## 🛠️ Installation
 
 ```bash
-pip install whisperplus
+pip install whisperplus git+https://github.com/huggingface/transformers
 pip install flash-attn --no-build-isolation
 ```
 
 ## 🤗 Model Hub
 
 You can find the models on the [HuggingFace Model Hub](https://huggingface.co/models?search=whisper)
 
@@ -40,20 +40,45 @@
 
 To use the whisperplus library, follow the steps below for different tasks:
 
 ### 🎵 Youtube URL to Audio
 
 ```python
 from whisperplus import SpeechToTextPipeline, download_and_convert_to_mp3
+from transformers import BitsAndBytesConfig, HqqConfig
 
-url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
 
+url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
 audio_path = download_and_convert_to_mp3(url)
-pipeline = SpeechToTextPipeline(model_id="openai/whisper-large-v3")
-transcript = pipeline(audio_path, "openai/whisper-large-v3", "english")
+
+quant_config = HqqConfig(
+    nbits=1, group_size=64, quant_zero=False, quant_scale=False, axis=0
+)  # axis=0 is used by default
+
+
+bnb_config = BitsAndBytesConfig(
+    load_in_4bit=True,
+    bnb_4bit_quant_type="nf4",
+    bnb_4bit_compute_dtype=torch.bfloat16,
+    bnb_4bit_use_double_quant=True,
+)
+
+pipeline = SpeechToTextPipeline(
+    model_id="distil-whisper/distil-large-v3", quant_config=quant_config
+)  # or bnb_config
+
+transcript = pipeline(
+    audio_path="test.mp3",
+    chunk_length_s=30,
+    stride_length_s=5,
+    max_new_tokens=128,
+    batch_size=100,
+    language="english",
+    return_timestamps=False,
+)
 
 print(transcript)
 ```
 
 ### 📰 Summarization
 
 ```python
```

#### html2text {}

```diff
@@ -1,67 +1,74 @@
-Metadata-Version: 2.1 Name: whisperplus Version: 0.2.8 Summary: WhisperPlus: A
-Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
+Metadata-Version: 2.1 Name: whisperplus Version: 0.2.8.1 Summary: WhisperPlus:
+A Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
 whisperplus Author: kadirnar Author-email: kadir.nar@hotmail.com License:
 Apache License 2.0 Description-Content-Type: text/markdown License-File:
 LICENSE
   ********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh FFeeaattuurree ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
-## ð ï¸ Installation ```bash pip install whisperplus pip install flash-attn
---no-build-isolation ``` ## ð¤ Model Hub You can find the models on the
-[HuggingFace Model Hub](https://huggingface.co/models?search=whisper) ##
-ðï¸ Usage To use the whisperplus library, follow the steps below for
-different tasks: ### ðµ Youtube URL to Audio ```python from whisperplus
-import SpeechToTextPipeline, download_and_convert_to_mp3 url = "https://
-www.youtube.com/watch?v=di3rHkEZuUw" audio_path = download_and_convert_to_mp3
-(url) pipeline = SpeechToTextPipeline(model_id="openai/whisper-large-v3")
-transcript = pipeline(audio_path, "openai/whisper-large-v3", "english") print
-(transcript) ``` ### ð° Summarization ```python from whisperplus import
-TextSummarizationPipeline summarizer = TextSummarizationPipeline
-(model_id="facebook/bart-large-cnn") summary = summarizer.summarize(transcript)
-print(summary[0]["summary_text"]) ``` ### ð° Long Text Support Summarization
-```python from whisperplus import LongTextSummarizationPipeline summarizer =
-LongTextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary_text
-= summarizer.summarize(transcript) print(summary_text) ``` ### ð¬ Speaker
-Diarization ```python from whisperplus import ( ASRDiarizationPipeline,
-download_and_convert_to_mp3, format_speech_to_dialogue, ) audio_path =
-download_and_convert_to_mp3("https://www.youtube.com/watch?v=mRB14sFHw2E")
-device = "cuda" # cpu or mps pipeline = ASRDiarizationPipeline.from_pretrained
-( asr_model="openai/whisper-large-v3", diarizer_model="pyannote/speaker-
-diarization", use_auth_token=False, chunk_length_s=30, device=device, )
-output_text = pipeline(audio_path, num_speakers=2, min_speaker=1,
-max_speaker=2) dialogue = format_speech_to_dialogue(output_text) print
-(dialogue) ``` ### â­ RAG - Chat with Video(LanceDB) ```python from
-whisperplus.pipelines.chatbot import ChatWithVideo chat = ChatWithVideo
-( input_file="trascript.txt", llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF",
-llm_model_file="mistral-7b-v0.1.Q4_K_M.gguf", llm_model_type="mistral",
-embedding_model_name="sentence-transformers/all-MiniLM-L6-v2", ) query = "what
-is this video about ?" response = chat.run_query(query) print(response) ``` ###
-ð  RAG - Chat with Video(AutoLLM) ```python from whisperplus import
-AutoLLMChatWithVideo # service_context_params system_prompt = """ You are an
-friendly ai assistant that help users find the most relevant and accurate
-answers to their questions based on the documents you have access to. When
-answering the questions, mostly rely on the info in documents. """
-query_wrapper_prompt = """ The document information is below. -----------------
----- {context_str} --------------------- Using the document information and
-mostly relying on it, answer the query. Query: {query_str} Answer: """ chat =
-AutoLLMChatWithVideo( input_file="input_dir", # path of mp3 file
-openai_key="YOUR_OPENAI_KEY", # optional
-huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-turbo",
-llm_max_tokens="256", llm_temperature="0.1", system_prompt=system_prompt,
-query_wrapper_prompt=query_wrapper_prompt, embed_model="huggingface/BAAI/bge-
-large-zh", # "text-embedding-ada-002" ) query = "what is this video about ?"
-response = chat.run_query(query) print(response) ``` ### ðï¸ Speech to Text
-```python from whisperplus import TextToSpeechPipeline tts =
-TextToSpeechPipeline(model_id="suno/bark") audio = tts(text="Hello World",
-voice_preset="v2/en_speaker_6") ``` ### ð¥ AutoCaption ```python from
-whisperplus import WhisperAutoCaptionPipeline caption =
-WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3") caption
-(video_path="test.mp4", output_path="output.mp4", language="turkish") ``` ##
-ð Contributing ```bash pip install -r dev-requirements.txt pre-commit
+## ð ï¸ Installation ```bash pip install whisperplus git+https://github.com/
+huggingface/transformers pip install flash-attn --no-build-isolation ``` ##
+ð¤ Model Hub You can find the models on the [HuggingFace Model Hub](https://
+huggingface.co/models?search=whisper) ## ðï¸ Usage To use the whisperplus
+library, follow the steps below for different tasks: ### ðµ Youtube URL to
+Audio ```python from whisperplus import SpeechToTextPipeline,
+download_and_convert_to_mp3 from transformers import BitsAndBytesConfig,
+HqqConfig url = "https://www.youtube.com/watch?v=di3rHkEZuUw" audio_path =
+download_and_convert_to_mp3(url) quant_config = HqqConfig( nbits=1,
+group_size=64, quant_zero=False, quant_scale=False, axis=0 ) # axis=0 is used
+by default bnb_config = BitsAndBytesConfig( load_in_4bit=True,
+bnb_4bit_quant_type="nf4", bnb_4bit_compute_dtype=torch.bfloat16,
+bnb_4bit_use_double_quant=True, ) pipeline = SpeechToTextPipeline
+( model_id="distil-whisper/distil-large-v3", quant_config=quant_config ) # or
+bnb_config transcript = pipeline( audio_path="test.mp3", chunk_length_s=30,
+stride_length_s=5, max_new_tokens=128, batch_size=100, language="english",
+return_timestamps=False, ) print(transcript) ``` ### ð° Summarization
+```python from whisperplus import TextSummarizationPipeline summarizer =
+TextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary =
+summarizer.summarize(transcript) print(summary[0]["summary_text"]) ``` ### ð°
+Long Text Support Summarization ```python from whisperplus import
+LongTextSummarizationPipeline summarizer = LongTextSummarizationPipeline
+(model_id="facebook/bart-large-cnn") summary_text = summarizer.summarize
+(transcript) print(summary_text) ``` ### ð¬ Speaker Diarization ```python
+from whisperplus import ( ASRDiarizationPipeline, download_and_convert_to_mp3,
+format_speech_to_dialogue, ) audio_path = download_and_convert_to_mp3("https://
+www.youtube.com/watch?v=mRB14sFHw2E") device = "cuda" # cpu or mps pipeline =
+ASRDiarizationPipeline.from_pretrained( asr_model="openai/whisper-large-v3",
+diarizer_model="pyannote/speaker-diarization", use_auth_token=False,
+chunk_length_s=30, device=device, ) output_text = pipeline(audio_path,
+num_speakers=2, min_speaker=1, max_speaker=2) dialogue =
+format_speech_to_dialogue(output_text) print(dialogue) ``` ### â­ RAG - Chat
+with Video(LanceDB) ```python from whisperplus.pipelines.chatbot import
+ChatWithVideo chat = ChatWithVideo( input_file="trascript.txt",
+llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF", llm_model_file="mistral-7b-
+v0.1.Q4_K_M.gguf", llm_model_type="mistral", embedding_model_name="sentence-
+transformers/all-MiniLM-L6-v2", ) query = "what is this video about ?" response
+= chat.run_query(query) print(response) ``` ### ð  RAG - Chat with Video
+(AutoLLM) ```python from whisperplus import AutoLLMChatWithVideo #
+service_context_params system_prompt = """ You are an friendly ai assistant
+that help users find the most relevant and accurate answers to their questions
+based on the documents you have access to. When answering the questions, mostly
+rely on the info in documents. """ query_wrapper_prompt = """ The document
+information is below. --------------------- {context_str} --------------------
+- Using the document information and mostly relying on it, answer the query.
+Query: {query_str} Answer: """ chat = AutoLLMChatWithVideo
+( input_file="input_dir", # path of mp3 file openai_key="YOUR_OPENAI_KEY", #
+optional huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-
+turbo", llm_max_tokens="256", llm_temperature="0.1",
+system_prompt=system_prompt, query_wrapper_prompt=query_wrapper_prompt,
+embed_model="huggingface/BAAI/bge-large-zh", # "text-embedding-ada-002" ) query
+= "what is this video about ?" response = chat.run_query(query) print(response)
+``` ### ðï¸ Speech to Text ```python from whisperplus import
+TextToSpeechPipeline tts = TextToSpeechPipeline(model_id="suno/bark") audio =
+tts(text="Hello World", voice_preset="v2/en_speaker_6") ``` ### ð¥
+AutoCaption ```python from whisperplus import WhisperAutoCaptionPipeline
+caption = WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3")
+caption(video_path="test.mp4", output_path="output.mp4", language="turkish")
+``` ## ð Contributing ```bash pip install -r dev-requirements.txt pre-commit
 install pre-commit run --all-files ``` ## ð License This project is licensed
 under the terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
 {radford2022whisper, doi = {10.48550/ARXIV.2212.04356}, url = {https://
 arxiv.org/abs/2212.04356}, author = {Radford, Alec and Kim, Jong Wook and Xu,
 Tao and Brockman, Greg and McLeavey, Christine and Sutskever, Ilya}, title =
 {Robust Speech Recognition via Large-Scale Weak Supervision}, publisher =
 {arXiv}, year = {2022}, copyright = {arXiv.org perpetual, non-exclusive
```

### Comparing `whisperplus-0.2.8/README.md` & `whisperplus-0.2.8.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     <a href="https://huggingface.co/spaces/ArtGAN/Audio-WebUI"><img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="HuggingFace Spaces"></a>
 </div>
 </div>
 
 ## 🛠️ Installation
 
 ```bash
-pip install whisperplus
+pip install whisperplus git+https://github.com/huggingface/transformers
 pip install flash-attn --no-build-isolation
 ```
 
 ## 🤗 Model Hub
 
 You can find the models on the [HuggingFace Model Hub](https://huggingface.co/models?search=whisper)
 
@@ -29,20 +29,45 @@
 
 To use the whisperplus library, follow the steps below for different tasks:
 
 ### 🎵 Youtube URL to Audio
 
 ```python
 from whisperplus import SpeechToTextPipeline, download_and_convert_to_mp3
+from transformers import BitsAndBytesConfig, HqqConfig
 
-url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
 
+url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
 audio_path = download_and_convert_to_mp3(url)
-pipeline = SpeechToTextPipeline(model_id="openai/whisper-large-v3")
-transcript = pipeline(audio_path, "openai/whisper-large-v3", "english")
+
+quant_config = HqqConfig(
+    nbits=1, group_size=64, quant_zero=False, quant_scale=False, axis=0
+)  # axis=0 is used by default
+
+
+bnb_config = BitsAndBytesConfig(
+    load_in_4bit=True,
+    bnb_4bit_quant_type="nf4",
+    bnb_4bit_compute_dtype=torch.bfloat16,
+    bnb_4bit_use_double_quant=True,
+)
+
+pipeline = SpeechToTextPipeline(
+    model_id="distil-whisper/distil-large-v3", quant_config=quant_config
+)  # or bnb_config
+
+transcript = pipeline(
+    audio_path="test.mp3",
+    chunk_length_s=30,
+    stride_length_s=5,
+    max_new_tokens=128,
+    batch_size=100,
+    language="english",
+    return_timestamps=False,
+)
 
 print(transcript)
 ```
 
 ### 📰 Summarization
 
 ```python
```

#### html2text {}

```diff
@@ -1,62 +1,69 @@
   ********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh FFeeaattuurree ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
-## ð ï¸ Installation ```bash pip install whisperplus pip install flash-attn
---no-build-isolation ``` ## ð¤ Model Hub You can find the models on the
-[HuggingFace Model Hub](https://huggingface.co/models?search=whisper) ##
-ðï¸ Usage To use the whisperplus library, follow the steps below for
-different tasks: ### ðµ Youtube URL to Audio ```python from whisperplus
-import SpeechToTextPipeline, download_and_convert_to_mp3 url = "https://
-www.youtube.com/watch?v=di3rHkEZuUw" audio_path = download_and_convert_to_mp3
-(url) pipeline = SpeechToTextPipeline(model_id="openai/whisper-large-v3")
-transcript = pipeline(audio_path, "openai/whisper-large-v3", "english") print
-(transcript) ``` ### ð° Summarization ```python from whisperplus import
-TextSummarizationPipeline summarizer = TextSummarizationPipeline
-(model_id="facebook/bart-large-cnn") summary = summarizer.summarize(transcript)
-print(summary[0]["summary_text"]) ``` ### ð° Long Text Support Summarization
-```python from whisperplus import LongTextSummarizationPipeline summarizer =
-LongTextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary_text
-= summarizer.summarize(transcript) print(summary_text) ``` ### ð¬ Speaker
-Diarization ```python from whisperplus import ( ASRDiarizationPipeline,
-download_and_convert_to_mp3, format_speech_to_dialogue, ) audio_path =
-download_and_convert_to_mp3("https://www.youtube.com/watch?v=mRB14sFHw2E")
-device = "cuda" # cpu or mps pipeline = ASRDiarizationPipeline.from_pretrained
-( asr_model="openai/whisper-large-v3", diarizer_model="pyannote/speaker-
-diarization", use_auth_token=False, chunk_length_s=30, device=device, )
-output_text = pipeline(audio_path, num_speakers=2, min_speaker=1,
-max_speaker=2) dialogue = format_speech_to_dialogue(output_text) print
-(dialogue) ``` ### â­ RAG - Chat with Video(LanceDB) ```python from
-whisperplus.pipelines.chatbot import ChatWithVideo chat = ChatWithVideo
-( input_file="trascript.txt", llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF",
-llm_model_file="mistral-7b-v0.1.Q4_K_M.gguf", llm_model_type="mistral",
-embedding_model_name="sentence-transformers/all-MiniLM-L6-v2", ) query = "what
-is this video about ?" response = chat.run_query(query) print(response) ``` ###
-ð  RAG - Chat with Video(AutoLLM) ```python from whisperplus import
-AutoLLMChatWithVideo # service_context_params system_prompt = """ You are an
-friendly ai assistant that help users find the most relevant and accurate
-answers to their questions based on the documents you have access to. When
-answering the questions, mostly rely on the info in documents. """
-query_wrapper_prompt = """ The document information is below. -----------------
----- {context_str} --------------------- Using the document information and
-mostly relying on it, answer the query. Query: {query_str} Answer: """ chat =
-AutoLLMChatWithVideo( input_file="input_dir", # path of mp3 file
-openai_key="YOUR_OPENAI_KEY", # optional
-huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-turbo",
-llm_max_tokens="256", llm_temperature="0.1", system_prompt=system_prompt,
-query_wrapper_prompt=query_wrapper_prompt, embed_model="huggingface/BAAI/bge-
-large-zh", # "text-embedding-ada-002" ) query = "what is this video about ?"
-response = chat.run_query(query) print(response) ``` ### ðï¸ Speech to Text
-```python from whisperplus import TextToSpeechPipeline tts =
-TextToSpeechPipeline(model_id="suno/bark") audio = tts(text="Hello World",
-voice_preset="v2/en_speaker_6") ``` ### ð¥ AutoCaption ```python from
-whisperplus import WhisperAutoCaptionPipeline caption =
-WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3") caption
-(video_path="test.mp4", output_path="output.mp4", language="turkish") ``` ##
-ð Contributing ```bash pip install -r dev-requirements.txt pre-commit
+## ð ï¸ Installation ```bash pip install whisperplus git+https://github.com/
+huggingface/transformers pip install flash-attn --no-build-isolation ``` ##
+ð¤ Model Hub You can find the models on the [HuggingFace Model Hub](https://
+huggingface.co/models?search=whisper) ## ðï¸ Usage To use the whisperplus
+library, follow the steps below for different tasks: ### ðµ Youtube URL to
+Audio ```python from whisperplus import SpeechToTextPipeline,
+download_and_convert_to_mp3 from transformers import BitsAndBytesConfig,
+HqqConfig url = "https://www.youtube.com/watch?v=di3rHkEZuUw" audio_path =
+download_and_convert_to_mp3(url) quant_config = HqqConfig( nbits=1,
+group_size=64, quant_zero=False, quant_scale=False, axis=0 ) # axis=0 is used
+by default bnb_config = BitsAndBytesConfig( load_in_4bit=True,
+bnb_4bit_quant_type="nf4", bnb_4bit_compute_dtype=torch.bfloat16,
+bnb_4bit_use_double_quant=True, ) pipeline = SpeechToTextPipeline
+( model_id="distil-whisper/distil-large-v3", quant_config=quant_config ) # or
+bnb_config transcript = pipeline( audio_path="test.mp3", chunk_length_s=30,
+stride_length_s=5, max_new_tokens=128, batch_size=100, language="english",
+return_timestamps=False, ) print(transcript) ``` ### ð° Summarization
+```python from whisperplus import TextSummarizationPipeline summarizer =
+TextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary =
+summarizer.summarize(transcript) print(summary[0]["summary_text"]) ``` ### ð°
+Long Text Support Summarization ```python from whisperplus import
+LongTextSummarizationPipeline summarizer = LongTextSummarizationPipeline
+(model_id="facebook/bart-large-cnn") summary_text = summarizer.summarize
+(transcript) print(summary_text) ``` ### ð¬ Speaker Diarization ```python
+from whisperplus import ( ASRDiarizationPipeline, download_and_convert_to_mp3,
+format_speech_to_dialogue, ) audio_path = download_and_convert_to_mp3("https://
+www.youtube.com/watch?v=mRB14sFHw2E") device = "cuda" # cpu or mps pipeline =
+ASRDiarizationPipeline.from_pretrained( asr_model="openai/whisper-large-v3",
+diarizer_model="pyannote/speaker-diarization", use_auth_token=False,
+chunk_length_s=30, device=device, ) output_text = pipeline(audio_path,
+num_speakers=2, min_speaker=1, max_speaker=2) dialogue =
+format_speech_to_dialogue(output_text) print(dialogue) ``` ### â­ RAG - Chat
+with Video(LanceDB) ```python from whisperplus.pipelines.chatbot import
+ChatWithVideo chat = ChatWithVideo( input_file="trascript.txt",
+llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF", llm_model_file="mistral-7b-
+v0.1.Q4_K_M.gguf", llm_model_type="mistral", embedding_model_name="sentence-
+transformers/all-MiniLM-L6-v2", ) query = "what is this video about ?" response
+= chat.run_query(query) print(response) ``` ### ð  RAG - Chat with Video
+(AutoLLM) ```python from whisperplus import AutoLLMChatWithVideo #
+service_context_params system_prompt = """ You are an friendly ai assistant
+that help users find the most relevant and accurate answers to their questions
+based on the documents you have access to. When answering the questions, mostly
+rely on the info in documents. """ query_wrapper_prompt = """ The document
+information is below. --------------------- {context_str} --------------------
+- Using the document information and mostly relying on it, answer the query.
+Query: {query_str} Answer: """ chat = AutoLLMChatWithVideo
+( input_file="input_dir", # path of mp3 file openai_key="YOUR_OPENAI_KEY", #
+optional huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-
+turbo", llm_max_tokens="256", llm_temperature="0.1",
+system_prompt=system_prompt, query_wrapper_prompt=query_wrapper_prompt,
+embed_model="huggingface/BAAI/bge-large-zh", # "text-embedding-ada-002" ) query
+= "what is this video about ?" response = chat.run_query(query) print(response)
+``` ### ðï¸ Speech to Text ```python from whisperplus import
+TextToSpeechPipeline tts = TextToSpeechPipeline(model_id="suno/bark") audio =
+tts(text="Hello World", voice_preset="v2/en_speaker_6") ``` ### ð¥
+AutoCaption ```python from whisperplus import WhisperAutoCaptionPipeline
+caption = WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3")
+caption(video_path="test.mp4", output_path="output.mp4", language="turkish")
+``` ## ð Contributing ```bash pip install -r dev-requirements.txt pre-commit
 install pre-commit run --all-files ``` ## ð License This project is licensed
 under the terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
 {radford2022whisper, doi = {10.48550/ARXIV.2212.04356}, url = {https://
 arxiv.org/abs/2212.04356}, author = {Radford, Alec and Kim, Jong Wook and Xu,
 Tao and Brockman, Greg and McLeavey, Christine and Sutskever, Ilya}, title =
 {Robust Speech Recognition via Large-Scale Weak Supervision}, publisher =
 {arXiv}, year = {2022}, copyright = {arXiv.org perpetual, non-exclusive
```

### Comparing `whisperplus-0.2.8/setup.cfg` & `whisperplus-0.2.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/setup.py` & `whisperplus-0.2.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/whisperplus/__init__.py` & `whisperplus-0.2.8.1/whisperplus/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,10 +3,10 @@
 from whisperplus.pipelines.summarization import TextSummarizationPipeline
 from whisperplus.pipelines.text2speech import TextToSpeechPipeline
 from whisperplus.pipelines.whisper import SpeechToTextPipeline
 from whisperplus.pipelines.whisper_diarize import ASRDiarizationPipeline
 from whisperplus.utils.download_utils import download_and_convert_to_mp3
 from whisperplus.utils.text_utils import format_speech_to_dialogue
 
-__version__ = '0.2.8'
+__version__ = '0.2.8.1'
 __author__ = 'kadirnar'
 __license__ = 'Apache License 2.0'
```

### Comparing `whisperplus-0.2.8/whisperplus/app.py` & `whisperplus-0.2.8.1/whisperplus/app.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/whisperplus/pipelines/autollm_chatbot.py` & `whisperplus-0.2.8.1/whisperplus/pipelines/autollm_chatbot.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/whisperplus/pipelines/lancedb_chatbot.py` & `whisperplus-0.2.8.1/whisperplus/pipelines/lancedb_chatbot.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/whisperplus/pipelines/long_text_summarization.py` & `whisperplus-0.2.8.1/whisperplus/pipelines/long_text_summarization.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/whisperplus/pipelines/summarization.py` & `whisperplus-0.2.8.1/whisperplus/pipelines/summarization.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/whisperplus/pipelines/text2speech.py` & `whisperplus-0.2.8.1/whisperplus/pipelines/text2speech.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/whisperplus/pipelines/whisper_autocaption.py` & `whisperplus-0.2.8.1/whisperplus/pipelines/whisper_autocaption.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/whisperplus/pipelines/whisper_diarize.py` & `whisperplus-0.2.8.1/whisperplus/pipelines/whisper_diarize.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/whisperplus/utils/download_utils.py` & `whisperplus-0.2.8.1/whisperplus/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/whisperplus/utils/text_utils.py` & `whisperplus-0.2.8.1/whisperplus/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.8/whisperplus.egg-info/PKG-INFO` & `whisperplus-0.2.8.1/whisperplus.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisperplus
-Version: 0.2.8
+Version: 0.2.8.1
 Summary: WhisperPlus: A Python library for WhisperPlus API.
 Home-page: https://github.com/kadirnar/whisperplus
 Author: kadirnar
 Author-email: kadir.nar@hotmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,15 +24,15 @@
     <a href="https://huggingface.co/spaces/ArtGAN/Audio-WebUI"><img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="HuggingFace Spaces"></a>
 </div>
 </div>
 
 ## 🛠️ Installation
 
 ```bash
-pip install whisperplus
+pip install whisperplus git+https://github.com/huggingface/transformers
 pip install flash-attn --no-build-isolation
 ```
 
 ## 🤗 Model Hub
 
 You can find the models on the [HuggingFace Model Hub](https://huggingface.co/models?search=whisper)
 
@@ -40,20 +40,45 @@
 
 To use the whisperplus library, follow the steps below for different tasks:
 
 ### 🎵 Youtube URL to Audio
 
 ```python
 from whisperplus import SpeechToTextPipeline, download_and_convert_to_mp3
+from transformers import BitsAndBytesConfig, HqqConfig
 
-url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
 
+url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
 audio_path = download_and_convert_to_mp3(url)
-pipeline = SpeechToTextPipeline(model_id="openai/whisper-large-v3")
-transcript = pipeline(audio_path, "openai/whisper-large-v3", "english")
+
+quant_config = HqqConfig(
+    nbits=1, group_size=64, quant_zero=False, quant_scale=False, axis=0
+)  # axis=0 is used by default
+
+
+bnb_config = BitsAndBytesConfig(
+    load_in_4bit=True,
+    bnb_4bit_quant_type="nf4",
+    bnb_4bit_compute_dtype=torch.bfloat16,
+    bnb_4bit_use_double_quant=True,
+)
+
+pipeline = SpeechToTextPipeline(
+    model_id="distil-whisper/distil-large-v3", quant_config=quant_config
+)  # or bnb_config
+
+transcript = pipeline(
+    audio_path="test.mp3",
+    chunk_length_s=30,
+    stride_length_s=5,
+    max_new_tokens=128,
+    batch_size=100,
+    language="english",
+    return_timestamps=False,
+)
 
 print(transcript)
 ```
 
 ### 📰 Summarization
 
 ```python
```

#### html2text {}

```diff
@@ -1,67 +1,74 @@
-Metadata-Version: 2.1 Name: whisperplus Version: 0.2.8 Summary: WhisperPlus: A
-Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
+Metadata-Version: 2.1 Name: whisperplus Version: 0.2.8.1 Summary: WhisperPlus:
+A Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
 whisperplus Author: kadirnar Author-email: kadir.nar@hotmail.com License:
 Apache License 2.0 Description-Content-Type: text/markdown License-File:
 LICENSE
   ********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh FFeeaattuurree ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
-## ð ï¸ Installation ```bash pip install whisperplus pip install flash-attn
---no-build-isolation ``` ## ð¤ Model Hub You can find the models on the
-[HuggingFace Model Hub](https://huggingface.co/models?search=whisper) ##
-ðï¸ Usage To use the whisperplus library, follow the steps below for
-different tasks: ### ðµ Youtube URL to Audio ```python from whisperplus
-import SpeechToTextPipeline, download_and_convert_to_mp3 url = "https://
-www.youtube.com/watch?v=di3rHkEZuUw" audio_path = download_and_convert_to_mp3
-(url) pipeline = SpeechToTextPipeline(model_id="openai/whisper-large-v3")
-transcript = pipeline(audio_path, "openai/whisper-large-v3", "english") print
-(transcript) ``` ### ð° Summarization ```python from whisperplus import
-TextSummarizationPipeline summarizer = TextSummarizationPipeline
-(model_id="facebook/bart-large-cnn") summary = summarizer.summarize(transcript)
-print(summary[0]["summary_text"]) ``` ### ð° Long Text Support Summarization
-```python from whisperplus import LongTextSummarizationPipeline summarizer =
-LongTextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary_text
-= summarizer.summarize(transcript) print(summary_text) ``` ### ð¬ Speaker
-Diarization ```python from whisperplus import ( ASRDiarizationPipeline,
-download_and_convert_to_mp3, format_speech_to_dialogue, ) audio_path =
-download_and_convert_to_mp3("https://www.youtube.com/watch?v=mRB14sFHw2E")
-device = "cuda" # cpu or mps pipeline = ASRDiarizationPipeline.from_pretrained
-( asr_model="openai/whisper-large-v3", diarizer_model="pyannote/speaker-
-diarization", use_auth_token=False, chunk_length_s=30, device=device, )
-output_text = pipeline(audio_path, num_speakers=2, min_speaker=1,
-max_speaker=2) dialogue = format_speech_to_dialogue(output_text) print
-(dialogue) ``` ### â­ RAG - Chat with Video(LanceDB) ```python from
-whisperplus.pipelines.chatbot import ChatWithVideo chat = ChatWithVideo
-( input_file="trascript.txt", llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF",
-llm_model_file="mistral-7b-v0.1.Q4_K_M.gguf", llm_model_type="mistral",
-embedding_model_name="sentence-transformers/all-MiniLM-L6-v2", ) query = "what
-is this video about ?" response = chat.run_query(query) print(response) ``` ###
-ð  RAG - Chat with Video(AutoLLM) ```python from whisperplus import
-AutoLLMChatWithVideo # service_context_params system_prompt = """ You are an
-friendly ai assistant that help users find the most relevant and accurate
-answers to their questions based on the documents you have access to. When
-answering the questions, mostly rely on the info in documents. """
-query_wrapper_prompt = """ The document information is below. -----------------
----- {context_str} --------------------- Using the document information and
-mostly relying on it, answer the query. Query: {query_str} Answer: """ chat =
-AutoLLMChatWithVideo( input_file="input_dir", # path of mp3 file
-openai_key="YOUR_OPENAI_KEY", # optional
-huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-turbo",
-llm_max_tokens="256", llm_temperature="0.1", system_prompt=system_prompt,
-query_wrapper_prompt=query_wrapper_prompt, embed_model="huggingface/BAAI/bge-
-large-zh", # "text-embedding-ada-002" ) query = "what is this video about ?"
-response = chat.run_query(query) print(response) ``` ### ðï¸ Speech to Text
-```python from whisperplus import TextToSpeechPipeline tts =
-TextToSpeechPipeline(model_id="suno/bark") audio = tts(text="Hello World",
-voice_preset="v2/en_speaker_6") ``` ### ð¥ AutoCaption ```python from
-whisperplus import WhisperAutoCaptionPipeline caption =
-WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3") caption
-(video_path="test.mp4", output_path="output.mp4", language="turkish") ``` ##
-ð Contributing ```bash pip install -r dev-requirements.txt pre-commit
+## ð ï¸ Installation ```bash pip install whisperplus git+https://github.com/
+huggingface/transformers pip install flash-attn --no-build-isolation ``` ##
+ð¤ Model Hub You can find the models on the [HuggingFace Model Hub](https://
+huggingface.co/models?search=whisper) ## ðï¸ Usage To use the whisperplus
+library, follow the steps below for different tasks: ### ðµ Youtube URL to
+Audio ```python from whisperplus import SpeechToTextPipeline,
+download_and_convert_to_mp3 from transformers import BitsAndBytesConfig,
+HqqConfig url = "https://www.youtube.com/watch?v=di3rHkEZuUw" audio_path =
+download_and_convert_to_mp3(url) quant_config = HqqConfig( nbits=1,
+group_size=64, quant_zero=False, quant_scale=False, axis=0 ) # axis=0 is used
+by default bnb_config = BitsAndBytesConfig( load_in_4bit=True,
+bnb_4bit_quant_type="nf4", bnb_4bit_compute_dtype=torch.bfloat16,
+bnb_4bit_use_double_quant=True, ) pipeline = SpeechToTextPipeline
+( model_id="distil-whisper/distil-large-v3", quant_config=quant_config ) # or
+bnb_config transcript = pipeline( audio_path="test.mp3", chunk_length_s=30,
+stride_length_s=5, max_new_tokens=128, batch_size=100, language="english",
+return_timestamps=False, ) print(transcript) ``` ### ð° Summarization
+```python from whisperplus import TextSummarizationPipeline summarizer =
+TextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary =
+summarizer.summarize(transcript) print(summary[0]["summary_text"]) ``` ### ð°
+Long Text Support Summarization ```python from whisperplus import
+LongTextSummarizationPipeline summarizer = LongTextSummarizationPipeline
+(model_id="facebook/bart-large-cnn") summary_text = summarizer.summarize
+(transcript) print(summary_text) ``` ### ð¬ Speaker Diarization ```python
+from whisperplus import ( ASRDiarizationPipeline, download_and_convert_to_mp3,
+format_speech_to_dialogue, ) audio_path = download_and_convert_to_mp3("https://
+www.youtube.com/watch?v=mRB14sFHw2E") device = "cuda" # cpu or mps pipeline =
+ASRDiarizationPipeline.from_pretrained( asr_model="openai/whisper-large-v3",
+diarizer_model="pyannote/speaker-diarization", use_auth_token=False,
+chunk_length_s=30, device=device, ) output_text = pipeline(audio_path,
+num_speakers=2, min_speaker=1, max_speaker=2) dialogue =
+format_speech_to_dialogue(output_text) print(dialogue) ``` ### â­ RAG - Chat
+with Video(LanceDB) ```python from whisperplus.pipelines.chatbot import
+ChatWithVideo chat = ChatWithVideo( input_file="trascript.txt",
+llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF", llm_model_file="mistral-7b-
+v0.1.Q4_K_M.gguf", llm_model_type="mistral", embedding_model_name="sentence-
+transformers/all-MiniLM-L6-v2", ) query = "what is this video about ?" response
+= chat.run_query(query) print(response) ``` ### ð  RAG - Chat with Video
+(AutoLLM) ```python from whisperplus import AutoLLMChatWithVideo #
+service_context_params system_prompt = """ You are an friendly ai assistant
+that help users find the most relevant and accurate answers to their questions
+based on the documents you have access to. When answering the questions, mostly
+rely on the info in documents. """ query_wrapper_prompt = """ The document
+information is below. --------------------- {context_str} --------------------
+- Using the document information and mostly relying on it, answer the query.
+Query: {query_str} Answer: """ chat = AutoLLMChatWithVideo
+( input_file="input_dir", # path of mp3 file openai_key="YOUR_OPENAI_KEY", #
+optional huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-
+turbo", llm_max_tokens="256", llm_temperature="0.1",
+system_prompt=system_prompt, query_wrapper_prompt=query_wrapper_prompt,
+embed_model="huggingface/BAAI/bge-large-zh", # "text-embedding-ada-002" ) query
+= "what is this video about ?" response = chat.run_query(query) print(response)
+``` ### ðï¸ Speech to Text ```python from whisperplus import
+TextToSpeechPipeline tts = TextToSpeechPipeline(model_id="suno/bark") audio =
+tts(text="Hello World", voice_preset="v2/en_speaker_6") ``` ### ð¥
+AutoCaption ```python from whisperplus import WhisperAutoCaptionPipeline
+caption = WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3")
+caption(video_path="test.mp4", output_path="output.mp4", language="turkish")
+``` ## ð Contributing ```bash pip install -r dev-requirements.txt pre-commit
 install pre-commit run --all-files ``` ## ð License This project is licensed
 under the terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
 {radford2022whisper, doi = {10.48550/ARXIV.2212.04356}, url = {https://
 arxiv.org/abs/2212.04356}, author = {Radford, Alec and Kim, Jong Wook and Xu,
 Tao and Brockman, Greg and McLeavey, Christine and Sutskever, Ilya}, title =
 {Robust Speech Recognition via Large-Scale Weak Supervision}, publisher =
 {arXiv}, year = {2022}, copyright = {arXiv.org perpetual, non-exclusive
```

### Comparing `whisperplus-0.2.8/whisperplus.egg-info/SOURCES.txt` & `whisperplus-0.2.8.1/whisperplus.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 whisperplus/__init__.py
 whisperplus/app.py
+whisperplus/test.py
 whisperplus.egg-info/PKG-INFO
 whisperplus.egg-info/SOURCES.txt
 whisperplus.egg-info/dependency_links.txt
 whisperplus.egg-info/requires.txt
 whisperplus.egg-info/top_level.txt
 whisperplus/pipelines/__init__.py
 whisperplus/pipelines/autollm_chatbot.py
```

