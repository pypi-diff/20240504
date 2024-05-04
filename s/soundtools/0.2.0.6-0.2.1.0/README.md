# Comparing `tmp/soundtools-0.2.0.6.tar.gz` & `tmp/soundtools-0.2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.2.0.6.tar", last modified: Wed May  1 19:29:21 2024, max compression
+gzip compressed data, was "soundtools-0.2.1.0.tar", last modified: Sat May  4 02:18:36 2024, max compression
```

## Comparing `soundtools-0.2.0.6.tar` & `soundtools-0.2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 19:29:21.502435 soundtools-0.2.0.6/
--rw-rw-rw-   0        0        0      701 2024-05-01 19:29:21.501434 soundtools-0.2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 19:29:21.502435 soundtools-0.2.0.6/setup.cfg
--rw-rw-rw-   0        0        0      789 2024-05-01 19:28:55.000000 soundtools-0.2.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 19:29:21.471098 soundtools-0.2.0.6/soundtools/
--rw-rw-rw-   0        0        0      399 2024-05-01 19:28:44.000000 soundtools-0.2.0.6/soundtools/__init__.py
--rw-rw-rw-   0        0        0    37237 2024-05-01 19:28:36.000000 soundtools-0.2.0.6/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-05-01 19:29:21.491167 soundtools-0.2.0.6/soundtools.egg-info/
--rw-rw-rw-   0        0        0      701 2024-05-01 19:29:21.000000 soundtools-0.2.0.6/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-05-01 19:29:21.000000 soundtools-0.2.0.6/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 19:29:21.000000 soundtools-0.2.0.6/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-01 19:29:21.000000 soundtools-0.2.0.6/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 02:18:36.541693 soundtools-0.2.1.0/
+-rw-rw-rw-   0        0        0      701 2024-05-04 02:18:36.541693 soundtools-0.2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 02:18:36.542690 soundtools-0.2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      789 2024-05-04 02:18:14.000000 soundtools-0.2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 02:18:36.538703 soundtools-0.2.1.0/soundtools/
+-rw-rw-rw-   0        0        0      399 2024-05-04 02:16:57.000000 soundtools-0.2.1.0/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    37676 2024-05-04 02:16:50.000000 soundtools-0.2.1.0/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-05-04 02:18:36.541693 soundtools-0.2.1.0/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-05-04 02:18:36.000000 soundtools-0.2.1.0/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-05-04 02:18:36.000000 soundtools-0.2.1.0/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 02:18:36.000000 soundtools-0.2.1.0/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-04 02:18:36.000000 soundtools-0.2.1.0/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.2.0.6/PKG-INFO` & `soundtools-0.2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.0.6
+Version: 0.2.1.0
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.0.6
+version: 0.2.1.0
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

### Comparing `soundtools-0.2.0.6/setup.py` & `soundtools-0.2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 setup(
 name='soundtools',
-version='0.2.0.6',
+version='0.2.1.0',
 description="used to work with sounds waves",
 long_description="""made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.0.6
+version: 0.2.1.0
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves""",
 author='Mohammad Erfan Karami',
```

### Comparing `soundtools-0.2.0.6/soundtools/soundtools.py` & `soundtools-0.2.1.0/soundtools/soundtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """### made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-### version: 0.2.0.6
+### version: 0.2.1.0
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves"""
 
@@ -21,14 +21,15 @@
 from soundfile import read as sfRead
 
 
 # types
 Dtype = np.dtype[np.float32|np.int16|np.uint8]
 SoundBuffer = np.ndarray[np.any, Dtype]
 Wave = Callable[[float, float, float], SoundBuffer]
+Note = str|float
 
 
 # its just a dictionary
 class Notes(dict[str, float]):
     """a dictionary used to store note names and frequencies"""
     def __init__(self):
         super().__init__()
@@ -55,16 +56,16 @@
         
         self.change_dtype(dtype)
     
     
     def change_dtype(self, dtype: Dtype):
         self.dtype = dtype
         if self.dtype == np.float32:
-            self.min_amp = -0.95
-            self.max_amp = 0.95
+            self.min_amp = 0
+            self.max_amp = 1
         else:
             i = np.iinfo(self.dtype)
             self.min_amp = i.min+1
             self.max_amp = i.max-1
     
     
     # caches the waves so if you had to generate a note multiple times its not gonna take long to execute
@@ -297,17 +298,17 @@
     
     def fade_in_out(self, buffer: SoundBuffer, fadein_len:int = 1500, fadeout_len:int = 1500) -> SoundBuffer:
         buffer = self.fade_in(buffer, fadein_len)
         buffer = self.fade_out(buffer, fadeout_len)
         return buffer
     
     
-    def staccato(self, wave: SoundBuffer, dur: float, play_time: float=0.75) -> SoundBuffer:
+    def staccato(self, wave: SoundBuffer, play_time: float=0.75) -> SoundBuffer:
         playing = len(wave)*play_time
-        resting = (1-play_time)*dur
+        resting = (1-play_time) * (wave.size/self.default_sample_rate)
         return np.append(wave[0:int(playing)], self.generate_note_buffer(0, self.sine_wave, resting))
     
     
     def array_to_tuple(self, np_array: SoundBuffer) -> tuple:
         """Iterates recursivelly."""
         try:
             return tuple(self.array_to_tuple(_) for _ in np_array)
@@ -383,15 +384,15 @@
     def export_to_wav(self, file_path:str, buffer: np.ndarray|bytes, sample_rate: int, dtype) -> None:
         if type(buffer) == bytes:
             buffer = np.frombuffer(buffer[8:], dtype=dtype)
         
         wf.write(file_path, sample_rate, buffer)
     
     # reads and return the bytes containing the sound from an erfan file
-    def read_from_erfan(self, file_name: str) -> bytes:
+    def read_from_erfan(self, file_name: str) -> SoundBuffer:
         """read and returns data from \".erfan\" file"""
         with open(file_name, "rb") as f:
             data = f.read()
             sample_rate = int.from_bytes(data[0:4], "little")
             sampwidth = int.from_bytes(data[4:6], "little")
             channels = int.from_bytes(data[6:8], "little")
             
@@ -535,15 +536,18 @@
         self.input_channels = n_channels
     
     
     def config_stream(self, samp_width: int|str, channels: int, sample_rate: int) -> pyaudio.Stream:
         if type(samp_width) == str:
             samp_width = self.get_sampwidth_from_str(dtype=samp_width)
         
-        return self.AUDIO_OBJECT.open(format=self.AUDIO_OBJECT.get_format_from_width(samp_width),
+        if not samp_width in (8, 32):
+            samp_width = self.AUDIO_OBJECT.get_format_from_width(samp_width)
+        
+        return self.AUDIO_OBJECT.open(format=samp_width,
                                       channels=channels,
                                       rate=sample_rate,
                                       output=True)
     
     
     def generate_note_names(self) -> None:
         # the number of note names has to be the same as the tune so if its less its not going to work.
@@ -564,17 +568,17 @@
     # if you want to change the middle a in the middle of a song you need to use this function
     def assign_middle_a(self, new_frequency:int|float=None) -> None:
         if new_frequency:
             self.MIDDLE_A = new_frequency
         self.BASS_A = self.MIDDLE_A
         self._hbl = 1
         
-        while self.BASS_A >= 20:
-            self.BASS_A /= 2
-            self._hbl += 1
+        exponent = int(np.log2(self.MIDDLE_A / 20))
+        self.BASS_A /= 2**exponent
+        self._hbl = exponent+1
     
     # you need to call the "assign_frequencies" function after it to change all the note's frecuencies based on the new middle a
     # although you can just change the self.middle_a value and use init after it, which will also call this function.
     
     
     # this function will create a dictionary of all the notes with a range of 20- to 20'000 frequencies.
     # it is depended on the middle_a and the tune that you're using.
@@ -605,19 +609,16 @@
         else:
             duration = float(duration[:-1])
         
         return duration
     
     
     def fix_volume(self, volume:float=0) -> float:
-        if volume == 0:
-            volume = self.DEFAULT_VOLUME
-
-        if volume > self.max_amp:
-            volume = self.max_amp
+        if volume > self.max_amp or volume < self.min_amp:
+            raise f"volume must be between {self.min_amp} and {self.max_amp}"
         
         return volume
     
     
     def get_file_data(self, file_path: str) -> tuple[SoundBuffer, int]:
         """gets the file data and returns a tuple[wave, sample_rate]
         you ca access other information as shown below
@@ -674,42 +675,50 @@
         return effect.pitch_shift(wave,
                                   sr=sample_rate,
                                   n_steps=n_semitones,
                                   bins_per_octave=semitones_per_octave)
     
     
     # creates a note buffer but doesn't turn it into bytes
-    def generate_note_buffer(self, note:str|float|int, wave_type: Wave, duration:str|float=0, volume:float=0) -> SoundBuffer:
+    def generate_note_buffer(self, note:Note, wave_type: Wave, duration:str|float=0, volume:float=0) -> SoundBuffer:
         """creates a sound wave based on the given note, wave type, duration and volume\n
         ### parameter note:
         can be a float as a frequency, or a string representing the note name forexample: \"A4\" or \"c#3\" or 220
         ### duration:
         can be an int representing the duration in beats (so it can be different based on the tempo)
         or can be a string representing the duration in seconds like this: \"2s\"
         ### note!:
-        if duration or volume are not passed as arguments when using the function, the default for both are 1, and you can change the default as well
+        if duration or volume are not passed as arguments when using the function, it will use `self.DEFAULT_DURATION` and `self.DEFAULT_VOLUME`, which you can change as well.
         ### example:
-        >>> generate_note_buffer("a4", sine_wave, \"1.5s\", 1)"""
+        >>> import soundtools
+        >>> m = soundtools.Music()
+        >>> m.init()
+        >>> note = m.generate_note_buffer("a4", m.sine_wave, \"1.5s\", 1)
+        >>> m.play_buffer(note)"""
         duration = self.fix_duration(duration)
         volume = self.fix_volume(volume)
         if str(note)[0].isdigit():
             f = float(note)
         else:
             f = self._NOTES[note]
         
         buf = wave_type(f, duration, volume)
         return buf
     
     
     # creates a chord buffer but doesn't turn it into bytes
-    def generate_chord_buffer(self, notes: Iterable[str|float], wave_type: Wave, duration:str|float=0, volume:float=0) -> SoundBuffer:
+    def generate_chord_buffer(self, notes: Iterable[Note], wave_type: Wave, duration:str|float=0, volume:float=0) -> SoundBuffer:
         """creates a sound wave based on the given notes, wave type, duration and volume\n
         ### parameter notes:
         is an iterable of floats as a frequency, or a strings representing the note name forexample:
-        >>> generate_chord_buffer((220, \"C#3\", \"e3\"), wave_type, 1.5, 1)"""
+        >>> import soundtools
+        >>> m = soundtools.Music()
+        >>> m.init()
+        >>> chord = generate_chord_buffer((220, \"C#3\", \"e3\"), m.sine_wave, 1.5, 1)
+        >>> m.play_buffer(chord)"""
         
         buf = self.generate_note_buffer(notes[0], wave_type, duration, volume)
         for n in notes[1:]:
             buf += self.generate_note_buffer(n, wave_type, duration, volume)
         return (buf/len(notes))
     
     
@@ -725,15 +734,15 @@
         
         buf = np.frombuffer(total_frames, self.input_dtype)
         return buf
     
     
     def add_buffers(a: SoundBuffer, b: SoundBuffer) -> SoundBuffer:
         s = a.size if a.size < b.size else b.size
-        return a[:s] + b[:s]
+        return (a[:s] + b[:s]) / 2
     
     
     def add_multiple_buffers(*buffers: SoundBuffer):
         s: int = buffers[0].size
         for buffer in buffers[1:]:
             if buffer.size < s:
                 s = buffer.size
```

### Comparing `soundtools-0.2.0.6/soundtools.egg-info/PKG-INFO` & `soundtools-0.2.1.0/soundtools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.0.6
+Version: 0.2.1.0
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.0.6
+version: 0.2.1.0
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

