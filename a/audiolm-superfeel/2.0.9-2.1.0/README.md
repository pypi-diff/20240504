# Comparing `tmp/audiolm_superfeel-2.0.9.tar.gz` & `tmp/audiolm_superfeel-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm_superfeel-2.0.9.tar", last modified: Sat May  4 10:22:29 2024, max compression
+gzip compressed data, was "audiolm_superfeel-2.1.0.tar", last modified: Sat May  4 10:30:41 2024, max compression
```

## Comparing `audiolm_superfeel-2.0.9.tar` & `audiolm_superfeel-2.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:22:29.105960 audiolm_superfeel-2.0.9/
--rw-r--r--   0 oseh       (501) staff       (20)     1066 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/LICENSE
--rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:22:29.105803 audiolm_superfeel-2.0.9/PKG-INFO
--rw-r--r--   0 oseh       (501) staff       (20)    21052 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/README.md
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:22:29.104908 audiolm_superfeel-2.0.9/audiolm_superfeel/
--rw-r--r--   0 oseh       (501) staff       (20)      932 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/__init__.py
--rw-r--r--   0 oseh       (501) staff       (20)     4170 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/attend.py
--rw-r--r--   0 oseh       (501) staff       (20)    79876 2024-05-04 10:14:52.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/audiolm_pytorch.py
--rw-r--r--   0 oseh       (501) staff       (20)     5118 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/data.py
--rw-r--r--   0 oseh       (501) staff       (20)     8077 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/encodec.py
--rw-r--r--   0 oseh       (501) staff       (20)     3071 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/hubert_kmeans.py
--rw-r--r--   0 oseh       (501) staff       (20)     1000 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/optimizer.py
--rw-r--r--   0 oseh       (501) staff       (20)    34449 2024-05-04 10:14:50.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/soundstream.py
--rw-r--r--   0 oseh       (501) staff       (20)     2555 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/t5.py
--rw-r--r--   0 oseh       (501) staff       (20)    56334 2024-05-04 10:14:55.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/trainer.py
--rw-r--r--   0 oseh       (501) staff       (20)      454 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/utils.py
--rw-r--r--   0 oseh       (501) staff       (20)       22 2024-05-04 10:22:19.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/version.py
--rw-r--r--   0 oseh       (501) staff       (20)     2351 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/vq_wav2vec.py
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:22:29.105600 audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/
--rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:22:29.000000 audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/PKG-INFO
--rw-r--r--   0 oseh       (501) staff       (20)      620 2024-05-04 10:22:29.000000 audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/SOURCES.txt
--rw-r--r--   0 oseh       (501) staff       (20)        1 2024-05-04 10:22:29.000000 audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/dependency_links.txt
--rw-r--r--   0 oseh       (501) staff       (20)      263 2024-05-04 10:22:29.000000 audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/requires.txt
--rw-r--r--   0 oseh       (501) staff       (20)       18 2024-05-04 10:22:29.000000 audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/top_level.txt
--rw-r--r--   0 oseh       (501) staff       (20)       38 2024-05-04 10:22:29.105997 audiolm_superfeel-2.0.9/setup.cfg
--rw-r--r--   0 oseh       (501) staff       (20)     1317 2024-05-04 10:21:39.000000 audiolm_superfeel-2.0.9/setup.py
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:30:41.757113 audiolm_superfeel-2.1.0/
+-rw-r--r--   0 oseh       (501) staff       (20)     1066 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.0/LICENSE
+-rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:30:41.756874 audiolm_superfeel-2.1.0/PKG-INFO
+-rw-r--r--   0 oseh       (501) staff       (20)    21070 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.0/README.md
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:30:41.755683 audiolm_superfeel-2.1.0/audiolm_superfeel/
+-rw-r--r--   0 oseh       (501) staff       (20)      958 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/__init__.py
+-rw-r--r--   0 oseh       (501) staff       (20)     4170 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/attend.py
+-rw-r--r--   0 oseh       (501) staff       (20)    79892 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/audiolm_superfeel.py
+-rw-r--r--   0 oseh       (501) staff       (20)     5120 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/data.py
+-rw-r--r--   0 oseh       (501) staff       (20)     8077 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/encodec.py
+-rw-r--r--   0 oseh       (501) staff       (20)     3073 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/hubert_kmeans.py
+-rw-r--r--   0 oseh       (501) staff       (20)     1000 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/optimizer.py
+-rw-r--r--   0 oseh       (501) staff       (20)    34453 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/soundstream.py
+-rw-r--r--   0 oseh       (501) staff       (20)     2555 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/t5.py
+-rw-r--r--   0 oseh       (501) staff       (20)    56350 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/trainer.py
+-rw-r--r--   0 oseh       (501) staff       (20)      454 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/utils.py
+-rw-r--r--   0 oseh       (501) staff       (20)       22 2024-05-04 10:30:38.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/version.py
+-rw-r--r--   0 oseh       (501) staff       (20)     2353 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.0/audiolm_superfeel/vq_wav2vec.py
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:30:41.756520 audiolm_superfeel-2.1.0/audiolm_superfeel.egg-info/
+-rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:30:41.000000 audiolm_superfeel-2.1.0/audiolm_superfeel.egg-info/PKG-INFO
+-rw-r--r--   0 oseh       (501) staff       (20)      622 2024-05-04 10:30:41.000000 audiolm_superfeel-2.1.0/audiolm_superfeel.egg-info/SOURCES.txt
+-rw-r--r--   0 oseh       (501) staff       (20)        1 2024-05-04 10:30:41.000000 audiolm_superfeel-2.1.0/audiolm_superfeel.egg-info/dependency_links.txt
+-rw-r--r--   0 oseh       (501) staff       (20)      263 2024-05-04 10:30:41.000000 audiolm_superfeel-2.1.0/audiolm_superfeel.egg-info/requires.txt
+-rw-r--r--   0 oseh       (501) staff       (20)       18 2024-05-04 10:30:41.000000 audiolm_superfeel-2.1.0/audiolm_superfeel.egg-info/top_level.txt
+-rw-r--r--   0 oseh       (501) staff       (20)       38 2024-05-04 10:30:41.757154 audiolm_superfeel-2.1.0/setup.cfg
+-rw-r--r--   0 oseh       (501) staff       (20)     1317 2024-05-04 10:21:39.000000 audiolm_superfeel-2.1.0/setup.py
```

### Comparing `audiolm_superfeel-2.0.9/LICENSE` & `audiolm_superfeel-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.9/PKG-INFO` & `audiolm_superfeel-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-superfeel
-Version: 2.0.9
+Version: 2.1.0
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/osehmathias/audiolm-superfeel
 Author: Phil Wang & Oseh Mathias
 Author-email: o@matmail.me
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm_superfeel-2.0.9/README.md` & `audiolm_superfeel-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,23 +50,23 @@
 
 ## Usage
 
 ### SoundStream & Encodec
 
 There are two options for the neural codec. If you want to use the pretrained 24kHz Encodec, just create an Encodec object as follows:
 ```python
-from audiolm_pytorch import EncodecWrapper
+from audiolm_superfeel import EncodecWrapper
 encodec = EncodecWrapper()
 # Now you can use the encodec variable in the same way you'd use the soundstream variables below.
 ```
 
 Otherwise, to stay more true to the original paper, you can use `SoundStream`. First, `SoundStream` needs to be trained on a large corpus of audio data
 
 ```python
-from audiolm_pytorch import SoundStream, SoundStreamTrainer
+from audiolm_superfeel import SoundStream, SoundStreamTrainer
 
 soundstream = SoundStream(
     codebook_size = 4096,
     rq_num_quantizers = 8,
     rq_groups = 2,                       # this paper proposes using multi-headed residual vector quantization - https://arxiv.org/abs/2305.02765
     use_lookup_free_quantizer = True,    # whether to use residual lookup free quantization - there are now reports of successful usage of this unpublished technique
     use_finite_scalar_quantizer = False, # whether to use residual finite scalar quantization
@@ -112,25 +112,25 @@
     soundstream(audio, return_recons_only = True)
 )
 ```
 
 You can also use soundstreams that are specific to `AudioLM` and `MusicLM` by importing `AudioLMSoundStream` and `MusicLMSoundStream` respectively
 
 ```python
-from audiolm_pytorch import AudioLMSoundStream, MusicLMSoundStream
+from audiolm_superfeel import AudioLMSoundStream, MusicLMSoundStream
 
 soundstream = AudioLMSoundStream(...) # say you want the hyperparameters as in Audio LM paper
 
 # rest is the same as above
 ```
 
 As of version `0.17.0`, you can now invoke the class method on `SoundStream` to load from checkpoint files, without having to remember your configurations.
 
 ```python
-from audiolm_pytorch import SoundStream
+from audiolm_superfeel import SoundStream
 
 soundstream = SoundStream.init_and_load_from('./path/to/checkpoint.pt')
 ```
 
 To use <a href="https://wandb.ai">Weights & Biases</a> tracking, first set `use_wandb_tracking = True` on the `SoundStreamTrainer`, then do the following
 
 ```python
@@ -153,15 +153,15 @@
 Then three separate transformers (`SemanticTransformer`, `CoarseTransformer`, `FineTransformer`) need to be trained
 
 
 ex. `SemanticTransformer`
 
 ```python
 import torch
-from audiolm_pytorch import HubertWithKmeans, SemanticTransformer, SemanticTransformerTrainer
+from audiolm_superfeel import HubertWithKmeans, SemanticTransformer, SemanticTransformerTrainer
 
 # hubert checkpoints can be downloaded at
 # https://github.com/facebookresearch/fairseq/tree/main/examples/hubert
 
 wav2vec = HubertWithKmeans(
     checkpoint_path = './hubert/hubert_base_ls960.pt',
     kmeans_path = './hubert/hubert_base_ls960_L9_km500.bin'
@@ -187,15 +187,15 @@
 trainer.train()
 ```
 
 ex. `CoarseTransformer`
 
 ```python
 import torch
-from audiolm_pytorch import HubertWithKmeans, SoundStream, CoarseTransformer, CoarseTransformerTrainer
+from audiolm_superfeel import HubertWithKmeans, SoundStream, CoarseTransformer, CoarseTransformerTrainer
 
 wav2vec = HubertWithKmeans(
     checkpoint_path = './hubert/hubert_base_ls960.pt',
     kmeans_path = './hubert/hubert_base_ls960_L9_km500.bin'
 )
 
 soundstream = SoundStream.init_and_load_from('/path/to/trained/soundstream.pt')
@@ -222,15 +222,15 @@
 trainer.train()
 ```
 
 ex. `FineTransformer`
 
 ```python
 import torch
-from audiolm_pytorch import SoundStream, FineTransformer, FineTransformerTrainer
+from audiolm_superfeel import SoundStream, FineTransformer, FineTransformerTrainer
 
 soundstream = SoundStream.init_and_load_from('/path/to/trained/soundstream.pt')
 
 fine_transformer = FineTransformer(
     num_coarse_quantizers = 3,
     num_fine_quantizers = 5,
     codebook_size = 1024,
@@ -250,15 +250,15 @@
 
 trainer.train()
 ```
 
 All together now
 
 ```python
-from audiolm_pytorch import AudioLM
+from audiolm_superfeel import AudioLM
 
 audiolm = AudioLM(
     wav2vec = wav2vec,
     codec = soundstream,
     semantic_transformer = semantic_transformer,
     coarse_transformer = coarse_transformer,
     fine_transformer = fine_transformer
@@ -280,15 +280,15 @@
 
 Update: Looks like this will work, given <a href="https://valle-demo.github.io/">'VALL-E'</a>
 
 ex. Semantic Transformer
 
 ```python
 import torch
-from audiolm_pytorch import HubertWithKmeans, SemanticTransformer, SemanticTransformerTrainer
+from audiolm_superfeel import HubertWithKmeans, SemanticTransformer, SemanticTransformerTrainer
 
 wav2vec = HubertWithKmeans(
     checkpoint_path = './hubert/hubert_base_ls960.pt',
     kmeans_path = './hubert/hubert_base_ls960_L9_km500.bin'
 )
 
 semantic_transformer = SemanticTransformer(
```

#### html2text {}

```diff
@@ -26,20 +26,20 @@
 compatibility! - _L_W_p_r_o_g_r_a_m_m_i_n_g for finding an issue with handling of the EOS
 token when sampling from the `FineTransformer`! - _@_Y_o_u_n_g_l_o_L_e_e for identifying a
 big bug in the 1d causal convolution for soundstream related to padding not
 accounting for strides! - _H_a_y_d_e_n for pointing out some discrepancies in the
 multi-scale discriminator for Soundstream ## Install ```bash $ pip install
 audiolm-pytorch ``` ## Usage ### SoundStream & Encodec There are two options
 for the neural codec. If you want to use the pretrained 24kHz Encodec, just
-create an Encodec object as follows: ```python from audiolm_pytorch import
+create an Encodec object as follows: ```python from audiolm_superfeel import
 EncodecWrapper encodec = EncodecWrapper() # Now you can use the encodec
 variable in the same way you'd use the soundstream variables below. ```
 Otherwise, to stay more true to the original paper, you can use `SoundStream`.
 First, `SoundStream` needs to be trained on a large corpus of audio data
-```python from audiolm_pytorch import SoundStream, SoundStreamTrainer
+```python from audiolm_superfeel import SoundStream, SoundStreamTrainer
 soundstream = SoundStream( codebook_size = 4096, rq_num_quantizers = 8,
 rq_groups = 2, # this paper proposes using multi-headed residual vector
 quantization - https://arxiv.org/abs/2305.02765 use_lookup_free_quantizer =
 True, # whether to use residual lookup free quantization - there are now
 reports of successful usage of this unpublished technique
 use_finite_scalar_quantizer = False, # whether to use residual finite scalar
 quantization attn_window_size = 128, # local attention receptive field at
@@ -56,66 +56,66 @@
 10080) - 1 channel ``` Your trained `SoundStream` can then be used as a generic
 tokenizer for audio ```python audio = torch.randn(1, 512 * 320) codes =
 soundstream.tokenize(audio) # you can now train anything with the codebook ids
 recon_audio_from_codes = soundstream.decode_from_codebook_indices(codes) #
 sanity check assert torch.allclose( recon_audio_from_codes, soundstream(audio,
 return_recons_only = True) ) ``` You can also use soundstreams that are
 specific to `AudioLM` and `MusicLM` by importing `AudioLMSoundStream` and
-`MusicLMSoundStream` respectively ```python from audiolm_pytorch import
+`MusicLMSoundStream` respectively ```python from audiolm_superfeel import
 AudioLMSoundStream, MusicLMSoundStream soundstream = AudioLMSoundStream(...) #
 say you want the hyperparameters as in Audio LM paper # rest is the same as
 above ``` As of version `0.17.0`, you can now invoke the class method on
 `SoundStream` to load from checkpoint files, without having to remember your
-configurations. ```python from audiolm_pytorch import SoundStream soundstream =
-SoundStream.init_and_load_from('./path/to/checkpoint.pt') ``` To use _W_e_i_g_h_t_s_ _&
-_B_i_a_s_e_s tracking, first set `use_wandb_tracking = True` on the
+configurations. ```python from audiolm_superfeel import SoundStream soundstream
+= SoundStream.init_and_load_from('./path/to/checkpoint.pt') ``` To use _W_e_i_g_h_t_s
+_&_ _B_i_a_s_e_s tracking, first set `use_wandb_tracking = True` on the
 `SoundStreamTrainer`, then do the following ```python trainer =
 SoundStreamTrainer( soundstream, ..., use_wandb_tracking = True ) # wrap .train
 () with contextmanager, specifying project and run name with
 trainer.wandb_tracker(project = 'soundstream', run = 'baseline'): trainer.train
 () ``` ### Hierarchical Transformers Then three separate transformers
 (`SemanticTransformer`, `CoarseTransformer`, `FineTransformer`) need to be
-trained ex. `SemanticTransformer` ```python import torch from audiolm_pytorch
+trained ex. `SemanticTransformer` ```python import torch from audiolm_superfeel
 import HubertWithKmeans, SemanticTransformer, SemanticTransformerTrainer #
 hubert checkpoints can be downloaded at # https://github.com/facebookresearch/
 fairseq/tree/main/examples/hubert wav2vec = HubertWithKmeans( checkpoint_path =
 './hubert/hubert_base_ls960.pt', kmeans_path = './hubert/
 hubert_base_ls960_L9_km500.bin' ) semantic_transformer = SemanticTransformer
 ( num_semantic_tokens = wav2vec.codebook_size, dim = 1024, depth = 6,
 flash_attn = True ).cuda() trainer = SemanticTransformerTrainer( transformer =
 semantic_transformer, wav2vec = wav2vec, folder ='/path/to/audio/files',
 batch_size = 1, data_max_length = 320 * 32, num_train_steps = 1 ) trainer.train
-() ``` ex. `CoarseTransformer` ```python import torch from audiolm_pytorch
+() ``` ex. `CoarseTransformer` ```python import torch from audiolm_superfeel
 import HubertWithKmeans, SoundStream, CoarseTransformer,
 CoarseTransformerTrainer wav2vec = HubertWithKmeans( checkpoint_path = './
 hubert/hubert_base_ls960.pt', kmeans_path = './hubert/
 hubert_base_ls960_L9_km500.bin' ) soundstream = SoundStream.init_and_load_from
 ('/path/to/trained/soundstream.pt') coarse_transformer = CoarseTransformer
 ( num_semantic_tokens = wav2vec.codebook_size, codebook_size = 1024,
 num_coarse_quantizers = 3, dim = 512, depth = 6, flash_attn = True ) trainer =
 CoarseTransformerTrainer( transformer = coarse_transformer, codec =
 soundstream, wav2vec = wav2vec, folder = '/path/to/audio/files', batch_size =
 1, data_max_length = 320 * 32, num_train_steps = 1_000_000 ) trainer.train()
-``` ex. `FineTransformer` ```python import torch from audiolm_pytorch import
+``` ex. `FineTransformer` ```python import torch from audiolm_superfeel import
 SoundStream, FineTransformer, FineTransformerTrainer soundstream =
 SoundStream.init_and_load_from('/path/to/trained/soundstream.pt')
 fine_transformer = FineTransformer( num_coarse_quantizers = 3,
 num_fine_quantizers = 5, codebook_size = 1024, dim = 512, depth = 6, flash_attn
 = True ) trainer = FineTransformerTrainer( transformer = fine_transformer,
 codec = soundstream, folder = '/path/to/audio/files', batch_size = 1,
 data_max_length = 320 * 32, num_train_steps = 1_000_000 ) trainer.train() ```
-All together now ```python from audiolm_pytorch import AudioLM audiolm =
+All together now ```python from audiolm_superfeel import AudioLM audiolm =
 AudioLM( wav2vec = wav2vec, codec = soundstream, semantic_transformer =
 semantic_transformer, coarse_transformer = coarse_transformer, fine_transformer
 = fine_transformer ) generated_wav = audiolm(batch_size = 1) # or with priming
 generated_wav_with_prime = audiolm(prime_wave = torch.randn(1, 320 * 8)) # or
 with text condition, if given generated_wav_with_text_condition = audiolm(text
 = ['chirping of birds and the distant echos of bells']) ``` ## Text Conditioned
 Audio Synthesis Update: Looks like this will work, given _'_V_A_L_L_-_E_' ex. Semantic
-Transformer ```python import torch from audiolm_pytorch import
+Transformer ```python import torch from audiolm_superfeel import
 HubertWithKmeans, SemanticTransformer, SemanticTransformerTrainer wav2vec =
 HubertWithKmeans( checkpoint_path = './hubert/hubert_base_ls960.pt',
 kmeans_path = './hubert/hubert_base_ls960_L9_km500.bin' ) semantic_transformer
 = SemanticTransformer( num_semantic_tokens = 500, dim = 1024, depth = 6,
 has_condition = True, # this will have to be set to True
 cond_as_self_attn_prefix = True # whether to condition as prefix to self
 attention, instead of cross attention, as was done in 'VALL-E' paper ).cuda() #
```

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel/__init__.py` & `audiolm_superfeel-2.1.0/audiolm_superfeel/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import torch
 from packaging import version
 
 if version.parse(torch.__version__) >= version.parse('2.0.0'):
     from einops._torch_specific import allow_ops_in_compiled_graph
     allow_ops_in_compiled_graph()
 
-from audiolm_pytorch.audiolm_pytorch import AudioLM
-from audiolm_pytorch.soundstream import SoundStream, AudioLMSoundStream, MusicLMSoundStream
-from audiolm_pytorch.encodec import EncodecWrapper
+from audiolm_superfeel.audiolm_superfeel import AudioLM
+from audiolm_superfeel.soundstream import SoundStream, AudioLMSoundStream, MusicLMSoundStream
+from audiolm_superfeel.encodec import EncodecWrapper
 
-from audiolm_pytorch.audiolm_pytorch import SemanticTransformer, CoarseTransformer, FineTransformer
-from audiolm_pytorch.audiolm_pytorch import FineTransformerWrapper, CoarseTransformerWrapper, SemanticTransformerWrapper
+from audiolm_superfeel.audiolm_superfeel import SemanticTransformer, CoarseTransformer, FineTransformer
+from audiolm_superfeel.audiolm_superfeel import FineTransformerWrapper, CoarseTransformerWrapper, SemanticTransformerWrapper
 
-from audiolm_pytorch.vq_wav2vec import FairseqVQWav2Vec
-from audiolm_pytorch.hubert_kmeans import HubertWithKmeans
+from audiolm_superfeel.vq_wav2vec import FairseqVQWav2Vec
+from audiolm_superfeel.hubert_kmeans import HubertWithKmeans
 
-from audiolm_pytorch.trainer import SoundStreamTrainer, SemanticTransformerTrainer, FineTransformerTrainer, CoarseTransformerTrainer
+from audiolm_superfeel.trainer import SoundStreamTrainer, SemanticTransformerTrainer, FineTransformerTrainer, CoarseTransformerTrainer
 
-from audiolm_pytorch.audiolm_pytorch import get_embeds
+from audiolm_superfeel.audiolm_superfeel import get_embeds
```

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel/attend.py` & `audiolm_superfeel-2.1.0/audiolm_superfeel/attend.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel/audiolm_pytorch.py` & `audiolm_superfeel-2.1.0/audiolm_superfeel/audiolm_superfeel.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 from torch.nn.utils.rnn import pad_sequence
 
 import torchaudio
 
 from einops import rearrange, repeat, reduce
 from einops.layers.torch import Rearrange
 
-from audiolm_pytorch.vq_wav2vec import FairseqVQWav2Vec
-from audiolm_pytorch.hubert_kmeans import HubertWithKmeans
+from audiolm_superfeel.vq_wav2vec import FairseqVQWav2Vec
+from audiolm_superfeel.hubert_kmeans import HubertWithKmeans
 
-from audiolm_pytorch.t5 import t5_encode_text, get_encoded_dim, DEFAULT_T5_NAME
+from audiolm_superfeel.t5 import t5_encode_text, get_encoded_dim, DEFAULT_T5_NAME
 
 from torchaudio.functional import resample
 
-from audiolm_pytorch.soundstream import SoundStream
-from audiolm_pytorch.encodec import EncodecWrapper
-from audiolm_pytorch.utils import AudioConditionerBase
-from audiolm_pytorch.attend import Attend
+from audiolm_superfeel.soundstream import SoundStream
+from audiolm_superfeel.encodec import EncodecWrapper
+from audiolm_superfeel.utils import AudioConditionerBase
+from audiolm_superfeel.attend import Attend
 
 from tqdm import tqdm
 from pathlib import Path
-from audiolm_pytorch.version import __version__
+from audiolm_superfeel.version import __version__
 from packaging import version
 
 # helper functions
 
 def exists(val):
     return val is not None
```

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel/data.py` & `audiolm_superfeel-2.1.0/audiolm_superfeel/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from torchaudio.functional import resample
 
 import torch
 import torch.nn.functional as F
 from torch.nn.utils.rnn import pad_sequence
 from torch.utils.data import Dataset, DataLoader
 
-from audiolm_pytorch.utils import curtail_to_multiple
+from audiolm_superfeel.utils import curtail_to_multiple
 
 from einops import rearrange, reduce
 
 # helper functions
 
 def exists(val):
     return val is not None
```

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel/encodec.py` & `audiolm_superfeel-2.1.0/audiolm_superfeel/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel/hubert_kmeans.py` & `audiolm_superfeel-2.1.0/audiolm_superfeel/hubert_kmeans.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 from torch import nn, einsum
 
 from torchaudio.functional import resample
 
 from einops import rearrange, repeat, pack, unpack
 
-from audiolm_pytorch.utils import curtail_to_multiple
+from audiolm_superfeel.utils import curtail_to_multiple
 
 # suppress a few warnings
 
 def noop(*args, **kwargs):
     pass
 
 import warnings
```

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel/optimizer.py` & `audiolm_superfeel-2.1.0/audiolm_superfeel/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel/soundstream.py` & `audiolm_superfeel-2.1.0/audiolm_superfeel/soundstream.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 )
 
 from local_attention import LocalMHA
 from local_attention.transformer import FeedForward, DynamicPositionBias
 
 from gateloop_transformer import SimpleGateLoopLayer as GateLoop
 
-from audiolm_pytorch.utils import curtail_to_multiple
+from audiolm_superfeel.utils import curtail_to_multiple
 
-from audiolm_pytorch.version import __version__
+from audiolm_superfeel.version import __version__
 from packaging import version
 parsed_version = version.parse(__version__)
 
 import pickle
 
 # helper functions
```

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel/t5.py` & `audiolm_superfeel-2.1.0/audiolm_superfeel/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel/trainer.py` & `audiolm_superfeel-2.1.0/audiolm_superfeel/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,36 +24,36 @@
 from torch.optim.lr_scheduler import LambdaLR, _LRScheduler
 from torch.utils.data import Dataset, DataLoader, random_split
 
 import pytorch_warmup as warmup
 
 from einops import rearrange
 
-from audiolm_pytorch.optimizer import get_optimizer
+from audiolm_superfeel.optimizer import get_optimizer
 import wandb
 from ema_pytorch import EMA
 
-from audiolm_pytorch.soundstream import SoundStream
-from audiolm_pytorch.encodec import EncodecWrapper
+from audiolm_superfeel.soundstream import SoundStream
+from audiolm_superfeel.encodec import EncodecWrapper
 
-from audiolm_pytorch.audiolm_pytorch import (
+from audiolm_superfeel.audiolm_superfeel import (
     SemanticTransformer,
     SemanticTransformerWrapper,
     CoarseTransformer,
     CoarseTransformerWrapper,
     FineTransformer,
     FineTransformerWrapper,
     FairseqVQWav2Vec,
     HubertWithKmeans
 )
 
-from audiolm_pytorch.data import SoundDataset, get_dataloader
-from audiolm_pytorch.utils import AudioConditionerBase
+from audiolm_superfeel.data import SoundDataset, get_dataloader
+from audiolm_superfeel.utils import AudioConditionerBase
 
-from audiolm_pytorch.version import __version__
+from audiolm_superfeel.version import __version__
 from packaging import version
 
 from accelerate import Accelerator, DistributedType
 from accelerate.utils import DistributedDataParallelKwargs, InitProcessGroupKwargs
 from accelerate.tracking import WandBTracker
```

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel/vq_wav2vec.py` & `audiolm_superfeel-2.1.0/audiolm_superfeel/vq_wav2vec.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from torch import nn
 from einops import rearrange
 
 import fairseq
 
 from torchaudio.functional import resample
 
-from audiolm_pytorch.utils import curtail_to_multiple
+from audiolm_superfeel.utils import curtail_to_multiple
 
 import logging
 logging.root.setLevel(logging.ERROR)
 
 def exists(val):
     return val is not None
```

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/PKG-INFO` & `audiolm_superfeel-2.1.0/audiolm_superfeel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-superfeel
-Version: 2.0.9
+Version: 2.1.0
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/osehmathias/audiolm-superfeel
 Author: Phil Wang & Oseh Mathias
 Author-email: o@matmail.me
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/SOURCES.txt` & `audiolm_superfeel-2.1.0/audiolm_superfeel.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
 README.md
 setup.py
 audiolm_superfeel/__init__.py
 audiolm_superfeel/attend.py
-audiolm_superfeel/audiolm_pytorch.py
+audiolm_superfeel/audiolm_superfeel.py
 audiolm_superfeel/data.py
 audiolm_superfeel/encodec.py
 audiolm_superfeel/hubert_kmeans.py
 audiolm_superfeel/optimizer.py
 audiolm_superfeel/soundstream.py
 audiolm_superfeel/t5.py
 audiolm_superfeel/trainer.py
```

### Comparing `audiolm_superfeel-2.0.9/setup.py` & `audiolm_superfeel-2.1.0/setup.py`

 * *Files identical despite different names*

