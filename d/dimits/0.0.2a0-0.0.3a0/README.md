# Comparing `tmp/dimits-0.0.2a0.tar.gz` & `tmp/dimits-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimits-0.0.2a0.tar", max compression
+gzip compressed data, was "dimits-0.0.3a0.tar", max compression
```

## Comparing `dimits-0.0.2a0.tar` & `dimits-0.0.3a0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      163 2023-07-29 15:53:03.793881 dimits-0.0.2a0/dimits/__init__.py
--rw-r--r--   0        0        0     8114 2023-07-29 15:52:47.945568 dimits-0.0.2a0/dimits/main.py
--rw-r--r--   0        0        0     6104 2023-07-29 15:49:49.628760 dimits-0.0.2a0/dimits/ttsmodel.py
--rw-r--r--   0        0        0     2056 2023-07-06 10:19:58.221599 dimits-0.0.2a0/dimits/utils.py
--rw-r--r--   0        0        0     1079 2023-06-28 10:26:13.254270 dimits-0.0.2a0/LICENSE
--rw-r--r--   0        0        0      711 2023-07-29 15:56:45.375138 dimits-0.0.2a0/pyproject.toml
--rw-r--r--   0        0        0     2843 2023-07-29 14:58:34.457187 dimits-0.0.2a0/README.md
--rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 dimits-0.0.2a0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-04 18:11:12.817825 dimits-0.0.3a0/LICENSE
+-rw-r--r--   0        0        0     2730 2024-05-04 18:11:12.817825 dimits-0.0.3a0/README.md
+-rw-r--r--   0        0        0      197 2024-05-04 18:11:12.817825 dimits-0.0.3a0/dimits/__init__.py
+-rw-r--r--   0        0        0     7594 2024-05-04 18:11:12.817825 dimits-0.0.3a0/dimits/main.py
+-rw-r--r--   0        0        0     5921 2024-05-04 18:11:12.817825 dimits-0.0.3a0/dimits/ttsmodel.py
+-rw-r--r--   0        0        0     1310 2024-05-04 18:11:12.817825 dimits-0.0.3a0/dimits/utils.py
+-rw-r--r--   0        0        0      799 2024-05-04 18:11:12.817825 dimits-0.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0     3736 1970-01-01 00:00:00.000000 dimits-0.0.3a0/PKG-INFO
```

### Comparing `dimits-0.0.2a0/dimits/main.py` & `dimits-0.0.3a0/dimits/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,227 +1,230 @@
-import os
-
-from dimits.utils import download, untar, logger
-
-from dimits.ttsmodel import TextToSpeechModel as ttsm
-import requests
-import shutil
-import platform
-
-import requests
-
-from pathlib import Path
-
-
-
-
-class Dimits():
-    """Dimits"""         
-    def __init__(self, voice: str, verbose: bool = True):
-        """
-        Initialize a new instance of Dimits with the provided voice and verbosity.
-
-        Args:
-            voice (str): The voice to use for text-to-speech.
-            verbose (bool): Whether to print verbose output.
-
-        Returns:
-            None
-        
-
-        Example:
-            >>> from Dimits import Dimits
-            >>> dt = Dimits("voice-en-us-amy-low")
-        """
-        self.verbose = verbose
-        # Define the URL for the latest release of piper
-        arch = str(self._get_os())
-        if self._get_os() == 'unsupported_machine': 
-            logger(err= f'{arch} Detected', verbose=verbose)
-            return 
-
-        home = str(Path.home())
-        
-        self.voice = voice
-        self.folder = 'piper'
-      
-        
-        self.parent_destn = os.path.join(home, self.folder)
-        if not os.path.exists(self.parent_destn):
-            os.mkdir(self.parent_destn)
-
-       
-        # Download the voice if it does not exist
-        self._download_voice(voice)
-
-        # Set the path to the ONNX voice file
-
-        self.voice_onnx = voice
-        self.voice_onnx = os.path.join(
-        self.parent_destn, str(self.voice_onnx).replace('voice-', '') + '.onnx')
-        logger('Using ' + str(self.voice_onnx), verbose=verbose)
-
-    
-    @staticmethod    
-    def _get_os() -> str:
-        if (platform.system() in ['Windows', 'Linux']):
-            return  platform.system();
-        else: 
-            return "unsupported_machine"
-
-      
-    @staticmethod
-    def list_voice() -> list[str]:
-        """
-        Method `list_voice()` Lists the supported voice as per in from https://api.github.com/repos/rhasspy/piper/releases
-        
-        Args:
-             None
-        
-        Returns:
-             list[str] : Supported voice
-        """
-        
-        releases_url = f"https://api.github.com/repos/rhasspy/piper/releases"
-
-        response = requests.get(releases_url)
-
-        data = response.json()
-
-        return [[str(asset['name']).split('.')[0] for asset in release['assets'] if asset['name'].startswith('voice')] for release in data][-1]
-
-        # return
-
-    def _download_voice(self, name, verbose: bool = True):
-        filename = f'{name}.tar.gz'
-        filepath = os.path.join(self.parent_destn, filename)
-        if not os.path.exists(filepath):
-            filename = f'{name}.tar.gz'
-            download_url = f'https://github.com/rhasspy/piper/releases/download/v0.0.2/{filename}'
-
-            
-            if type(download(download_url, filepath, filename, verbose)) is tuple:
-                fp, f = tuple(download(download_url, filepath, filename, verbose))
-                untar(fp, f, verbose)
-            
-                
-           
-
-    def text_2_audio_file(self, text: str, filename: str, directory: str, format: str = 'wav') -> str:
-        r"""
-
-        Convert the provided text to a human-sounding audio file using a text-to-speech engine, and save it to disk.
-
-        Args:
-            text (str): The text to be converted to audio.
-            filename (str): The name of the output audio file, without the file extension.
-            format (str): The file format of the output audio file (e.g. 'wav', 'mp3', 'ogg', etc.).
-            directory (str): The directory in which to save the output audio file.
-       
-        Returns:
-            str: The path of audio file
-        
-        
-
-        Example:
-            >>> from Dimits import Dimits
-            >>> dt = ... #Initialize here
-            >>> dt.text_to_audio("Hello World", "hello_world", "wav", "/path/to/output/directory/")
-            >>> # Outputs an audio file named "hello_world.wav" in the directory "/path/to/output/directory/".
-
-       """
-        if self._get_os() == 'unsupported_machine': return
-        if not os.path.exists(directory):
-            os.mkdir(directory)
-        filepath = os.path.join(directory, f'{filename}.{format}')
-        
-     
-        out_bin = ttsm(self.voice_onnx).synthesize(text,length_scale=1.0, noise_scale=1.0, noise_w=1.0)
-        with open(filepath, 'wb') as f:
-            f.write(out_bin)
-
-        return filepath
-
-    def text_file_2_audio_file(self, text_file_path: str, audio_filename: str, directory: str, audio_format: str='wav', encoding='utf8', **kwargs) -> str:
-        """
-        Convert the provided text files to audio file
-
-        Args:
-            text_file_path (str): Path of the file to be read
-            audio_filename (str): The name of the audio file to be saved
-            directory (str): The directory to which audio file is extracted
-            audio_format (str): The format of audio file
-            encoding (str): encoding of the text file to be read utf8, utf16
-
-        Returns:
-            str: audio file path
-
-        Example:
-            >>> from dimits import Dimits 
-            >>> dd = ...
-            >>> dd.text_file_2_audio_file(file_path,'hello', dir,)
-        """
-        if self._get_os() == 'unsupported_machine': return
-        with open(text_file_path, encoding=encoding) as f:
-           return self.text_2_audio_file(f.readline(), audio_filename, directory, audio_format, **kwargs)
-
-
-    def text_2_speech(self, text: str, engine: str = None , **kwargs: str) -> None:
-        
-        r"""
-        Convert the provided text to human-sounding audio and play the audio file on-the-go.
-
-        Args:
-            text (str): The text to be converted to audio.
-            engine (str): The text-to-speech engine to play the audio file .
-                          Defaults to 'aplay'.
-                        
-        Returns:
-            None
-        
-
-        Example:
-            >>> from dimits import Dimits
-            >>> dt = ... #Initialize here
-            >>> dt.text_2_speech("Hello World", "aplay"")
-            >>> # plays the audio to the default audio output device using the 'alsa' engine.
-        """
-        
-        if self._get_os() == 'unsupported_machine': return
-        cache_dir  = os.path.join(self.parent_destn, 'cache')
-        if os.path.isdir(cache_dir):
-            shutil.rmtree(cache_dir)
-            os.mkdir(cache_dir)
-
-        filepath = self.text_2_audio_file(
-                       text, 'main', directory=cache_dir, )
-        if platform.system() == 'Linux':
-        
-           os.system(f'killall {engine}')
-           if engine == None: engine = 'aplay'
-           
-           if engine == 'aplay':
-              os.system(f'{engine} {filepath}')
-           else:
-               pass
-        elif platform.system() == 'Windows':
-            if engine == None:  engine = 'System.Media.SoundPlayer'
-
-
-           
-            if engine == 'System.Media.SoundPlayer':
-               cmd = f"""powershell (New-Object {engine} {filepath}).PlaySync()"""
-               os.system(cmd )
-           
-    
- 
-
-print(Dimits.list_voice())
-Dimits("voice-en-us-danny-low").text_2_speech(text="""
-Here is a randomly generated short story:
-
-It was a dark and stormy night. John was home alone, sitting in his living room reading a book. The wind howled outside as the rain pattered against the windows. Suddenly, there was a loud crash from the kitchen. John jumped up, his heart racing. What was that?
-
-As John slowly walked towards the kitchen, he could hear a strange skittering sound. He flipped on the light switch, but the power was out. Grabbing a flashlight from a drawer, he shined it around the room. In the beam of light, John saw the shattered remains of a flower vase on the floor.""", filename='test', directory='C:\\Users\\Ananiya\\PyProject\\PyPiperTTS\\dimits')
-
-
-
+import os
+
+from dimits.utils import download,  logger
+
+from dimits.ttsmodel import TextToSpeechModel as ttsm
+import requests
+import shutil
+
+from huggingface_hub import hf_hub_url,snapshot_download,hf_hub_download
+import platform
+
+import requests
+
+from pathlib import Path
+from huggingface_hub import HfFileSystem
+
+
+
+class Dimits():
+    """Dimits"""         
+    def __init__(self, voice: str, verbose: bool = True, modelDirectory: str = None):
+        """
+        Initialize a new instance of Dimits with the provided voice and verbosity.
+
+        Args:
+            voice (str): The voice to use for text-to-speech.
+            verbose (bool): Whether to print verbose output.
+            model (str): represents the local path to the model file. If not provided (i.e., None), the default behavior is to utilize the model hosted on GitHub.
+
+        Returns:
+            None
+        
+
+        Example:
+            >>> from Dimits import Dimits
+            >>> dt = Dimits("en_US-amy-low")
+        """
+        self.verbose = verbose
+       
+        # Define the URL for the latest release of piper
+
+        arch = str(self._get_os())
+        if self._get_os() == 'unsupported_machine': 
+            logger(err= f'{arch} Detected', verbose=verbose)
+            return 
+
+        home =  Path.home()
+        
+        self.voice = voice
+        self.folder = 'piper'
+
+        self._repo_id = "rhasspy/piper-voices"
+      
+        
+        self.parent_destn = modelDirectory if modelDirectory is not None else os.path.join(home, self.folder)
+        
+        if not os.path.exists(self.parent_destn):
+            os.mkdir(self.parent_destn)
+
+       
+        # Download the voice if it does not exist
+        self._download_voice(voice)
+
+        # Set the path to the ONNX voice file
+
+        self.voice_onnx = voice
+        self.voice_onnx = os.path.join(
+        self.parent_destn, str(self.voice_onnx) + '.onnx')
+        logger('Using ' + str(self.voice_onnx), verbose=verbose)
+
+    
+    @staticmethod    
+    def _get_os() -> str:
+        if (platform.system() in ['Windows', 'Linux']):
+            return  platform.system();
+        else: 
+            return "unsupported_machine"
+
+      
+    @staticmethod
+    def list_voice() -> list[str]:
+        """
+        Method `list_voice()` Lists the supported voice as per in from https://api.github.com/repos/rhasspy/piper/releases
+        
+        Args:
+             None
+        
+        Returns:
+             list[str] : Supported voice
+        """
+        
+        fs = HfFileSystem()
+ 
+        return [_.split("/")[-1].split(".")[0] for _ in fs.glob(f"{self._repo_id}/**.onnx", detail=False)]
+
+        # return
+
+    def _download_voice(self, name, verbose: bool = True):
+        print(name)
+        locale, p, pitch = name.split('-')
+        lang, cc = locale.split("_")
+        filename =  f"""{name}.onnx"""
+        filename2 = f"""{name}.onnx.json"""
+        filepath = os.path.join(self.parent_destn, filename)
+        filepath2 = os.path.join(self.parent_destn, filename2)
+      
+        if not os.path.exists(filepath) or not os.path.exists(filepath2) :
+        
+            
+
+
+        
+
+            url =hf_hub_url(repo_id=self._repo_id,filename=f"{lang}/{locale}/{p}/{pitch}/{name}.onnx")
+            url2 = hf_hub_url(repo_id=self._repo_id,filename=f"{lang}/{locale}/{p}/{pitch}/{name}.onnx.json")
+            download(url, filepath, filename, verbose)
+            download(url2, filepath2, filename2, verbose) 
+            
+                
+           
+
+    def text_2_audio_file(self, text: str, filename: str, directory: str, format: str = 'wav') -> str:
+        r"""
+
+        Convert the provided text to a human-sounding audio file using a text-to-speech engine, and save it to disk.
+
+        Args:
+            text (str): The text to be converted to audio.
+            filename (str): The name of the output audio file, without the file extension.
+            format (str): The file format of the output audio file (e.g. 'wav', 'mp3', 'ogg', etc.).
+            directory (str): The directory in which to save the output audio file.
+       
+        Returns:
+            str: The path of audio file
+        
+        
+
+        Example:
+            >>> from Dimits import Dimits
+            >>> dt = ... #Initialize here
+            >>> dt.text_to_audio("Hello World", "hello_world", "wav", "/path/to/output/directory/")
+            >>> # Outputs an audio file named "hello_world.wav" in the directory "/path/to/output/directory/".
+
+       """
+        if self._get_os() == 'unsupported_machine': return
+        if not os.path.exists(directory):
+            os.mkdir(directory)
+        filepath = os.path.join(directory, f'{filename}.{format}')
+        
+     
+        out_bin = ttsm(self.voice_onnx).synthesize(text,length_scale=1.0, noise_scale=1.0, noise_w=1.0)
+        with open(filepath, 'wb') as f:
+            f.write(out_bin)
+
+        return filepath
+
+    def text_file_2_audio_file(self, text_file_path: str, audio_filename: str, directory: str, audio_format: str='wav', encoding='utf8', **kwargs) -> str:
+        """
+        Convert the provided text files to audio file
+
+        Args:
+            text_file_path (str): Path of the file to be read
+            audio_filename (str): The name of the audio file to be saved
+            directory (str): The directory to which audio file is extracted
+            audio_format (str): The format of audio file
+            encoding (str): encoding of the text file to be read utf8, utf16
+
+        Returns:
+            str: audio file path
+
+        Example:
+            >>> from dimits import Dimits 
+            >>> dd = ...
+            >>> dd.text_file_2_audio_file(file_path,'hello', dir,)
+        """
+        if self._get_os() == 'unsupported_machine': return
+        with open(text_file_path, encoding=encoding) as f:
+           return self.text_2_audio_file(f.readline(), audio_filename, directory, audio_format, **kwargs)
+
+
+    def text_2_speech(self, text: str, engine: str = None , **kwargs: str) -> None:
+        
+        r"""
+        Convert the provided text to human-sounding audio and play the audio file on-the-go.
+
+        Args:
+            text (str): The text to be converted to audio.
+            engine (str): The text-to-speech engine to play the audio file .
+                          Defaults to 'aplay'.
+                        
+        Returns:
+            None
+        
+
+        Example:
+            >>> from dimits import Dimits
+            >>> dt = ... #Initialize here
+            >>> dt.text_2_speech("Hello World", "aplay"")
+            >>> # plays the audio to the default audio output device using the 'alsa' engine.
+        """
+        
+        if self._get_os() == 'unsupported_machine': return
+        cache_dir  = os.path.join(self.parent_destn, 'cache')
+        if os.path.isdir(cache_dir):
+            shutil.rmtree(cache_dir)
+            os.mkdir(cache_dir)
+
+        filepath = self.text_2_audio_file(
+                       text, 'main', directory=cache_dir, )
+        if platform.system() == 'Linux':
+        
+           os.system(f'killall {engine}')
+           if engine == None: engine = 'aplay'
+           
+           if engine == 'aplay':
+              os.system(f'{engine} {filepath}')
+           else:
+               pass
+        elif platform.system() == 'Windows':
+            if engine == None:  engine = 'System.Media.SoundPlayer'
+
+
+           
+            if engine == 'System.Media.SoundPlayer':
+               cmd = f"""powershell (New-Object {engine} {filepath}).PlaySync()"""
+               os.system(cmd )
+           
+    
+ 
+
```

### Comparing `dimits-0.0.2a0/dimits/ttsmodel.py` & `dimits-0.0.3a0/dimits/ttsmodel.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-import io
-import json
-from dataclasses import dataclass
-import logging
-import wave
-from pathlib import Path
-from typing import List, Mapping, Optional, Sequence, Union, Dict
-
-import numpy as np
-import onnxruntime as ort 
-from espeak_phonemizer import Phonemizer
-from dimits.utils import logger
-import soundfile as sf
-
-_LOGGER = logging.getLogger(__name__)
-
-_BOS = "^"
-_EOS = "$"
-_PAD = "_"
-
-@dataclass
-class AudioConfig:
-    sample_rate: int
-    quality: Optional[str] = None
-    
-@dataclass    
-class EspeakConfig:
-    voice: str
-    
-@dataclass
-class InferenceConfig:
-    noise_scale: float
-    length_scale: float
-    noise_w: float
-    
-@dataclass    
-class TTSConfig:
-
-    audio: AudioConfig
-    espeak: EspeakConfig 
-    inference: InferenceConfig
-    
-    phoneme_type: str
-    phoneme_map: Mapping[str, List[int]] 
-    phoneme_id_map: Mapping[str, List[int]]
-    
-    num_symbols: int
-    num_speakers: int
-    speaker_id_map: Dict
-    
-    piper_version: str
-    
-    language: Dict[str, str]
-    dataset: str
-
-    def __init__(self, **kwargs):
-        self.audio = AudioConfig(**kwargs.pop('audio'))
-        self.espeak = EspeakConfig(**kwargs.pop('espeak'))
-        self.inference = InferenceConfig(**kwargs.pop('inference'))
-        self.phoneme_type = kwargs.pop('phoneme_type', None)
-        self.phoneme_map = kwargs.pop('phoneme_map')
-        self.phoneme_id_map = kwargs.pop('phoneme_id_map')
-        self.num_symbols = kwargs.pop('num_symbols')
-        self.num_speakers = kwargs.pop('num_speakers')
-        self.speaker_id_map = kwargs.pop('speaker_id_map')
-        self.piper_version = kwargs.pop('piper_version', None)
-        self.language = kwargs.pop('language', None)
-        self.dataset = kwargs.pop('dataset', None)
-       
-    
-# TTS model    
-class TextToSpeechModel:
-
-    def __init__(
-        self,
-        model_path: Union[str, Path],
-        config_path: Optional[Union[str, Path]] = None,
-        use_cpu: bool =True
-    ):
-        if config_path is None:
-            config_path = f"{model_path}.json"
-            
-        self.config = self._load_config(config_path)
-      
-        self.phonemizer = Phonemizer(self.config.espeak.voice)
-        self.model = ort.InferenceSession(str(model_path),sess_options=ort.SessionOptions(),
-            providers= ["CPUExecutionProvider"] if(use_cpu == False) else ['CUDAExecutionProvider']
-           )
-
-    def synthesize(
-        self,
-        text: str,
-        speaker_id: Optional[int] = None,
-        length_scale: Optional[float] = None,
-        noise_scale: Optional[float] = None,
-        noise_w: Optional[float] = None,
-    ) -> bytes:
-        
-        # Set default parameters if needed
-        length_scale = length_scale or self.config.inference.length_scale
-        noise_scale = noise_scale or self.config.inference.noise_scale
-        noise_w = noise_w or self.config.inference.noise_w
-        
-        # Convert text to phonemes
-        phonemes = self._text_to_phonemes(text)
-        
-        # Encode phonemes to ids
-        phoneme_ids = self._phonemes_to_ids(phonemes)
-        
-        # Create model inputs
-        inputs = self._create_inputs(phoneme_ids, speaker_id, noise_scale, length_scale, noise_w)
-
-        # Run synthesis
-        audio = self.model.run(None, inputs)[0].squeeze((0,1))
-        
-        # Convert float to int16
-        audio = self._float_to_int16(audio)
-        
-        # Save as WAV
-        wav_bytes = self._write_wav(audio, self.config.audio.sample_rate)
-        
-        return wav_bytes
-
-    def _text_to_phonemes(self, text: str) -> List[str]:
-        """Convert text to phoneme sequence"""
-        phonemes = [_BOS] + list(self.phonemizer.phonemize(text,keep_clause_breakers=True ))
-       
-        return phonemes
-
-    def _phonemes_to_ids(self, phonemes: List[str]) -> List[int]:
-        """Map phonemes to ids"""
-        ids = []
-        for p in phonemes:
-           
-            if p in self.config.phoneme_id_map:
-                
-                ids.extend(self.config.phoneme_id_map[p])
-                ids.extend(self.config.phoneme_id_map[_PAD])
-            else:
-                logger(f"No id found for {p}")
-        ids.extend(self.config.phoneme_id_map[_EOS])
-        return ids
-
-    def _create_inputs(self, phoneme_ids, speaker_id, noise_scale, length_scale, noise_w):
-        """Create model input tensors"""
-        phoneme_ids = np.expand_dims(np.array(phoneme_ids,dtype=np.int64), 0)
-        length = np.array([phoneme_ids.shape[1]], dtype=np.int64)
-        scales = np.array([noise_scale, length_scale, noise_w],dtype=np.float32)
-        speaker = np.array([speaker_id], dtype=np.int64) if speaker_id is not None else None
-        
-        return {
-            "input": phoneme_ids,
-            "input_lengths": length, 
-            "scales": scales,
-            "speaker": speaker
-        }
-
-    def _float_to_int16(self, audio: np.ndarray) -> np.ndarray:
-        """Convert audio array from float to int16"""
-        audio_norm = audio * (32767 / max(0.01, np.max(np.abs(audio))))
-        audio_norm = np.clip(audio_norm, -32767, 32767).astype("int16")
-        return audio_norm 
-
-    def _write_wav(self, audio: np.ndarray, sample_rate: int) -> bytes:
-        """Save audio array as WAV file in memory"""
-        with io.BytesIO() as fout:
-            out : wave.Wave_write = wave.open(fout, "wb")
-            with out:
-               out.setframerate(sample_rate)
-               out.setsampwidth(2)
-               out.setnchannels(1)
-               out.writeframes(audio.tobytes())
-            # sf.write(fout, audio, samplerate=sample_rate, format="WAV", subtype="PCM_16")
-            return fout.getvalue()
-            
-    def _load_config(self, path):
-        """Load configuration from JSON file"""
-        with open(path,  "r", encoding="utf-8") as f:
-            data = json.load(f)
-            t = TTSConfig(**data)
-       
-            return t
-        
+import io
+import json
+from dataclasses import dataclass
+import logging
+import wave
+from pathlib import Path
+from typing import List, Mapping, Optional, Sequence, Union, Dict
+
+import numpy as np
+import onnxruntime as ort 
+from espeak_phonemizer import Phonemizer
+from dimits.utils import logger
+import soundfile as sf
+
+_LOGGER = logging.getLogger(__name__)
+
+_BOS = "^"
+_EOS = "$"
+_PAD = "_"
+
+@dataclass
+class AudioConfig:
+    sample_rate: int
+    quality: Optional[str] = None
+    
+@dataclass    
+class EspeakConfig:
+    voice: str
+    
+@dataclass
+class InferenceConfig:
+    noise_scale: float
+    length_scale: float
+    noise_w: float
+    
+@dataclass    
+class TTSConfig:
+
+    audio: AudioConfig
+    espeak: EspeakConfig 
+    inference: InferenceConfig
+    
+    phoneme_type: str
+    phoneme_map: Mapping[str, List[int]] 
+    phoneme_id_map: Mapping[str, List[int]]
+    
+    num_symbols: int
+    num_speakers: int
+    speaker_id_map: Dict
+    
+    piper_version: str
+    
+    language: Dict[str, str]
+    dataset: str
+
+    def __init__(self, **kwargs):
+        self.audio = AudioConfig(**kwargs.pop('audio'))
+        self.espeak = EspeakConfig(**kwargs.pop('espeak'))
+        self.inference = InferenceConfig(**kwargs.pop('inference'))
+        self.phoneme_type = kwargs.pop('phoneme_type', None)
+        self.phoneme_map = kwargs.pop('phoneme_map')
+        self.phoneme_id_map = kwargs.pop('phoneme_id_map')
+        self.num_symbols = kwargs.pop('num_symbols')
+        self.num_speakers = kwargs.pop('num_speakers')
+        self.speaker_id_map = kwargs.pop('speaker_id_map')
+        self.piper_version = kwargs.pop('piper_version', None)
+        self.language = kwargs.pop('language', None)
+        self.dataset = kwargs.pop('dataset', None)
+       
+    
+# TTS model    
+class TextToSpeechModel:
+
+    def __init__(
+        self,
+        model_path: Union[str, Path],
+        config_path: Optional[Union[str, Path]] = None,
+        use_cpu: bool =True
+    ):
+        if config_path is None:
+            config_path = f"{model_path}.json"
+            
+        self.config = self._load_config(config_path)
+      
+        self.phonemizer = Phonemizer(self.config.espeak.voice)
+        self.model = ort.InferenceSession(str(model_path),sess_options=ort.SessionOptions(),
+            providers= ["CPUExecutionProvider"] if(use_cpu == False) else ['CUDAExecutionProvider']
+           )
+
+    def synthesize(
+        self,
+        text: str,
+        speaker_id: Optional[int] = None,
+        length_scale: Optional[float] = None,
+        noise_scale: Optional[float] = None,
+        noise_w: Optional[float] = None,
+    ) -> bytes:
+        
+        # Set default parameters if needed
+        length_scale = length_scale or self.config.inference.length_scale
+        noise_scale = noise_scale or self.config.inference.noise_scale
+        noise_w = noise_w or self.config.inference.noise_w
+        
+        # Convert text to phonemes
+        phonemes = self._text_to_phonemes(text)
+        
+        # Encode phonemes to ids
+        phoneme_ids = self._phonemes_to_ids(phonemes)
+        
+        # Create model inputs
+        inputs = self._create_inputs(phoneme_ids, speaker_id, noise_scale, length_scale, noise_w)
+
+        # Run synthesis
+        audio = self.model.run(None, inputs)[0].squeeze((0,1))
+        
+        # Convert float to int16
+        audio = self._float_to_int16(audio)
+        
+        # Save as WAV
+        wav_bytes = self._write_wav(audio, self.config.audio.sample_rate)
+        
+        return wav_bytes
+
+    def _text_to_phonemes(self, text: str) -> List[str]:
+        """Convert text to phoneme sequence"""
+        phonemes = [_BOS] + list(self.phonemizer.phonemize(text,keep_clause_breakers=True ))
+       
+        return phonemes
+
+    def _phonemes_to_ids(self, phonemes: List[str]) -> List[int]:
+        """Map phonemes to ids"""
+        ids = []
+        for p in phonemes:
+           
+            if p in self.config.phoneme_id_map:
+                
+                ids.extend(self.config.phoneme_id_map[p])
+                ids.extend(self.config.phoneme_id_map[_PAD])
+            else:
+                logger(f"No id found for {p}")
+        ids.extend(self.config.phoneme_id_map[_EOS])
+        return ids
+
+    def _create_inputs(self, phoneme_ids, speaker_id, noise_scale, length_scale, noise_w):
+        """Create model input tensors"""
+        phoneme_ids = np.expand_dims(np.array(phoneme_ids,dtype=np.int64), 0)
+        length = np.array([phoneme_ids.shape[1]], dtype=np.int64)
+        scales = np.array([noise_scale, length_scale, noise_w],dtype=np.float32)
+        speaker = np.array([speaker_id], dtype=np.int64) if speaker_id is not None else None
+        
+        return {
+            "input": phoneme_ids,
+            "input_lengths": length, 
+            "scales": scales,
+            "speaker": speaker
+        }
+
+    def _float_to_int16(self, audio: np.ndarray) -> np.ndarray:
+        """Convert audio array from float to int16"""
+        audio_norm = audio * (32767 / max(0.01, np.max(np.abs(audio))))
+        audio_norm = np.clip(audio_norm, -32767, 32767).astype("int16")
+        return audio_norm 
+
+    def _write_wav(self, audio: np.ndarray, sample_rate: int) -> bytes:
+        """Save audio array as WAV file in memory"""
+        with io.BytesIO() as fout:
+            out : wave.Wave_write = wave.open(fout, "wb")
+            with out:
+               out.setframerate(sample_rate)
+               out.setsampwidth(2)
+               out.setnchannels(1)
+               out.writeframes(audio.tobytes())
+            # sf.write(fout, audio, samplerate=sample_rate, format="WAV", subtype="PCM_16")
+            return fout.getvalue()
+            
+    def _load_config(self, path):
+        """Load configuration from JSON file"""
+        with open(path,  "r", encoding="utf-8") as f:
+            data = json.load(f)
+            t = TTSConfig(**data)
+       
+            return t
+
```

### Comparing `dimits-0.0.2a0/LICENSE` & `dimits-0.0.3a0/LICENSE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2023 Ananiya Jemberu (Reqeique)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2023 Ananiya Jemberu (Reqeique)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `dimits-0.0.2a0/README.md` & `dimits-0.0.3a0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-
-# **Dimits - Python Bindings for Piper TTS**
-
-
-Dimits is a Python library that provides an easy-to-use interface to the Piper text-to-speech (TTS) system. It utilizes the powerful Piper TTS engine, which is optimized for Raspberry Pi 4, to generate high-quality synthesized speech.
-> 
-## Features
-
-* Simple Python bindings for Piper TTS
-* Support for multiple languages and voices
-* Compatible with Raspberry Pi 3/4 and desktop Linux systems
-
-## Installation 📥
-
-You can install Dimits via pip:
-
-```sh
-pip install dimits
-```
-
-This will automatically install the necessary dependencies
-
-## Quick Start 🏃🏻‍♀️
-
-Here's a simple example of using Dimits to synthesize speech:
-
-```python
-from dimits import Dimits
-
-# Initialize Dimits with the desired voice model
-dt = Dimits("voice-en-us-amy-low")
-
-# Convert text to audio and play it using the aplay engine
-dt.text_2_speech("Hello World", engine="aplay")
-```
-
-## Voices 🔊
-
-Dimits supports all the voices available in the Piper TTS system. To use a specific voice, simply provide  corresponding `.onnx` file namepo initializing the `Dimits` class.
-
-For a list of available voices and their download links, refer to the [Piper TTS repository](https://github.com/rhasspy/piper/releases/tag/v0.0.2).
-
-## Usage 📃
-
-### Initializing Dimits
-
-To use Dimits, first create an instance of the `Dimits` class, providing the path to the desired voice model:
-
-```python
-from dimits import Dimits
-
-dt = Dimits("voice-en-us-amy-low")
-```
-
-### Synthesizing Speech
-
-To synthesize speech and play on the go, simply call the `text_2_speech` method, providing the text to be synthesized and the desired engine:
-
-```python
-dt.text_2_speech("This is a test.",engine='aplay')
-```
-
-on other hand to synthesize speech and save it to the file, call `text_2_audio_file` finction providing `file_name` `dir` and `format`
-
-```python
-dt.text_2_audio_file("Hello World", "hello_world", "/path/to/output/directory/", format="wav")
-```
-
-### Changing Voices
-
-To change the voice used for synthesis, create a new instance of the `Dimits` class with the desired voice model:
-
-```python
-# dt = Dimits("voice-en-us-amy-low")
-dt = Dimits("voice-en-us-danny-low")
-```
-## TODO 📝
-* ~~Implement windows compatible executible to run the voice models~~
-* Support for multiple audio player engine
-* Benchmark
-* Documentation
-
-
-## License 🪪
-
-This project is licensed under the [MIT License](LICENSE).
-
-## Acknowledgements
-Dimits is based on the work of the [Piper](https://github.com/rhasspy/piper) project by [Rhasspy](https://rhasspy.readthedocs.io/en/latest/), and is made possible by the contributions of its developers and the open source community. Without their hard work and dedication, this project would not be possible.
+
+# **Dimits - Python Bindings for Piper TTS**
+
+
+Dimits is a Python library that provides an easy-to-use interface to the Piper text-to-speech (TTS) system. It utilizes the powerful Piper TTS engine, which is optimized for Raspberry Pi 4, to generate high-quality synthesized speech.
+> 
+## Features
+
+* Simple Python bindings for Piper TTS
+* Support for multiple languages and voices
+* Compatible with Raspberry Pi 3/4 and desktop Linux systems
+
+## Installation 📥
+
+You can install Dimits via pip:
+
+```sh
+pip install dimits
+```
+
+This will automatically install the necessary dependencies
+
+## Quick Start 🏃🏻‍♀️
+
+Here's a simple example of using Dimits to synthesize speech:
+
+```python
+from dimits import Dimits
+
+# Initialize Dimits with the desired voice model
+dt = Dimits("en_US-amy-low")
+
+# Convert text to audio and play it using the aplay engine
+dt.text_2_speech("Hello World", engine="aplay")
+```
+
+## Voices 🔊
+
+Dimits supports all the voices available in the Piper TTS system. To use a specific voice, simply provide  corresponding `.onnx` file namepo initializing the `Dimits` class.
+
+For a list of available voices and their download links, refer to the [Piper TTS repository](https://github.com/rhasspy/piper/releases/tag/v0.0.2).
+
+## Usage 📃
+
+### Initializing Dimits
+
+To use Dimits, first create an instance of the `Dimits` class, providing the path to the desired voice model:
+
+```python
+from dimits import Dimits
+
+dt = Dimits("en_US-amy-low")
+```
+
+### Synthesizing Speech
+
+To synthesize speech and play on the go, simply call the `text_2_speech` method, providing the text to be synthesized and the desired engine:
+
+```python
+dt.text_2_speech("This is a test.",engine='aplay')
+```
+
+on other hand to synthesize speech and save it to the file, call `text_2_audio_file` finction providing `file_name` `dir` and `format`
+
+```python
+dt.text_2_audio_file("Hello World", "hello_world", "/path/to/output/directory/", format="wav")
+```
+
+### Changing Voices
+
+To change the voice used for synthesis, create a new instance of the `Dimits` class with the desired voice model:
+
+```python
+# dt = Dimits("en_US-amy-low")
+dt = Dimits("en_US-danny-low")
+```
+## TODO 📝
+* ~~Implement windows compatible executible to run the voice models~~
+* Support for multiple audio player engine
+* Benchmark
+* Documentation
+
+
+## License 🪪
+
+This project is licensed under the [MIT License](LICENSE).
+
+## Acknowledgements
+Dimits is based on the work of the [Piper](https://github.com/rhasspy/piper) project by [Rhasspy](https://rhasspy.readthedocs.io/en/latest/), and is made possible by the contributions of its developers and the open source community. Without their hard work and dedication, this project would not be possible.
```

### Comparing `dimits-0.0.2a0/PKG-INFO` & `dimits-0.0.3a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: dimits
-Version: 0.0.2a0
+Version: 0.0.3a0
 Summary: Dimits is a Python library that provides an easy-to-use interface to the Piper text-to-speech (TTS) system. It utilizes the powerful Piper TTS engine, which is optimized for Raspberry Pi 4, to generate high-quality synthesized speech.
 License: MIT
 Author: Reqeique
 Author-email: ananiyajemberu21@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: espeak-phonemizer
 Requires-Dist: espeak-phonemizer-windows ; sys_platform == "win32"
+Requires-Dist: huggingface-hub (==0.23.0)
+Requires-Dist: onnxruntime
 Requires-Dist: requests (>=2.13.0,<3.0.0)
+Requires-Dist: soundfile
 Requires-Dist: tqdm (==4.64.0)
 Description-Content-Type: text/markdown
 
 
 # **Dimits - Python Bindings for Piper TTS**
 
 
@@ -42,15 +47,15 @@
 
 Here's a simple example of using Dimits to synthesize speech:
 
 ```python
 from dimits import Dimits
 
 # Initialize Dimits with the desired voice model
-dt = Dimits("voice-en-us-amy-low")
+dt = Dimits("en_US-amy-low")
 
 # Convert text to audio and play it using the aplay engine
 dt.text_2_speech("Hello World", engine="aplay")
 ```
 
 ## Voices 🔊
 
@@ -63,15 +68,15 @@
 ### Initializing Dimits
 
 To use Dimits, first create an instance of the `Dimits` class, providing the path to the desired voice model:
 
 ```python
 from dimits import Dimits
 
-dt = Dimits("voice-en-us-amy-low")
+dt = Dimits("en_US-amy-low")
 ```
 
 ### Synthesizing Speech
 
 To synthesize speech and play on the go, simply call the `text_2_speech` method, providing the text to be synthesized and the desired engine:
 
 ```python
@@ -85,16 +90,16 @@
 ```
 
 ### Changing Voices
 
 To change the voice used for synthesis, create a new instance of the `Dimits` class with the desired voice model:
 
 ```python
-# dt = Dimits("voice-en-us-amy-low")
-dt = Dimits("voice-en-us-danny-low")
+# dt = Dimits("en_US-amy-low")
+dt = Dimits("en_US-danny-low")
 ```
 ## TODO 📝
 * ~~Implement windows compatible executible to run the voice models~~
 * Support for multiple audio player engine
 * Benchmark
 * Documentation
```

