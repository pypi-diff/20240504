# Comparing `tmp/asmu-0.0.1a7.tar.gz` & `tmp/asmu-0.0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmu-0.0.1a7.tar", last modified: Wed Apr 24 09:44:04 2024, max compression
+gzip compressed data, was "asmu-0.0.1a8.tar", last modified: Sat May  4 15:55:33 2024, max compression
```

## Comparing `asmu-0.0.1a7.tar` & `asmu-0.0.1a8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:44:04.189603 asmu-0.0.1a7/
--rw-rw-rw-   0 root         (0) root         (0)    35148 2024-04-24 09:43:51.000000 asmu-0.0.1a7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      846 2024-04-24 09:44:04.188603 asmu-0.0.1a7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-04-24 09:43:51.000000 asmu-0.0.1a7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:44:04.187603 asmu-0.0.1a7/asmu/
--rw-rw-rw-   0 root         (0) root         (0)      551 2024-04-24 09:43:51.000000 asmu-0.0.1a7/asmu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-04-24 09:43:51.000000 asmu-0.0.1a7/asmu/afile.py
--rw-rw-rw-   0 root         (0) root         (0)     2786 2024-04-24 09:43:51.000000 asmu-0.0.1a7/asmu/analyzer.py
--rw-rw-rw-   0 root         (0) root         (0)     3207 2024-04-24 09:43:51.000000 asmu-0.0.1a7/asmu/asetup.py
--rw-rw-rw-   0 root         (0) root         (0)     6150 2024-04-24 09:43:51.000000 asmu-0.0.1a7/asmu/generator.py
--rw-rw-rw-   0 root         (0) root         (0)    10972 2024-04-24 09:43:51.000000 asmu-0.0.1a7/asmu/io.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2024-04-24 09:43:51.000000 asmu-0.0.1a7/asmu/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:44:04.188603 asmu-0.0.1a7/asmu.egg-info/
--rw-r--r--   0 root         (0) root         (0)      846 2024-04-24 09:44:04.000000 asmu-0.0.1a7/asmu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      276 2024-04-24 09:44:04.000000 asmu-0.0.1a7/asmu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 09:44:04.000000 asmu-0.0.1a7/asmu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-24 09:44:04.000000 asmu-0.0.1a7/asmu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-24 09:44:04.000000 asmu-0.0.1a7/asmu.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      739 2024-04-24 09:43:51.000000 asmu-0.0.1a7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 09:44:04.189603 asmu-0.0.1a7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 15:55:33.343035 asmu-0.0.1a8/
+-rw-rw-rw-   0 root         (0) root         (0)    35148 2024-05-04 15:55:19.000000 asmu-0.0.1a8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      846 2024-05-04 15:55:33.342034 asmu-0.0.1a8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-05-04 15:55:19.000000 asmu-0.0.1a8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 15:55:33.341035 asmu-0.0.1a8/asmu/
+-rw-rw-rw-   0 root         (0) root         (0)      551 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/afile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2925 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3207 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/asetup.py
+-rw-rw-rw-   0 root         (0) root         (0)     7136 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10940 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 15:55:33.342034 asmu-0.0.1a8/asmu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      846 2024-05-04 15:55:33.000000 asmu-0.0.1a8/asmu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      276 2024-05-04 15:55:33.000000 asmu-0.0.1a8/asmu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-04 15:55:33.000000 asmu-0.0.1a8/asmu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-04 15:55:33.000000 asmu-0.0.1a8/asmu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-04 15:55:33.000000 asmu-0.0.1a8/asmu.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      739 2024-05-04 15:55:19.000000 asmu-0.0.1a8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-04 15:55:33.343035 asmu-0.0.1a8/setup.cfg
```

### Comparing `asmu-0.0.1a7/LICENSE` & `asmu-0.0.1a8/LICENSE`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a7/PKG-INFO` & `asmu-0.0.1a8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asmu
-Version: 0.0.1a7
+Version: 0.0.1a8
 Summary: Acoustic Signal Measurement Utilities
 Author-email: felhub <felhub@net4us.at>
 Project-URL: Repository, https://gitlab.com/felhub/asmu
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `asmu-0.0.1a7/asmu/__init__.py` & `asmu-0.0.1a8/asmu/__init__.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a7/asmu/afile.py` & `asmu-0.0.1a8/asmu/afile.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,93 +4,90 @@
 import os
 import json
 from datetime import datetime
 import numpy as np
 
 
 class AFile(soundfile.SoundFile):
-    def __init__(self, afile_path:str, mode:str="r", samplerate:int=None, channels:int=None) -> None:
+    def __init__(self, afile_path:str, mode:str="r", samplerate:int=None, channels:int=None, temp:bool=False) -> None:
         """The AFile class handles .wav sound files. Metadata is used to store and load additional settings.
         It is recommended to open AFile's in a with statement.
 
         Args:
             afile_path (str): Path to .wav file.
             mode ({"r", "r+", "w", "w+"}, optional): File open mode.
             samplerate (int, optional): Samplerate, only used in write mode.
             channels (int, optional): Channel count, only used in write mode.
+            temp (bool): Set file temporary (deleted on close). Only used in write mode.
 
         Example:
             ```python linenums="1" title="Load a file"
             from asmu import AFile
 
             with AFile(AFILE_PATH) as afile:
                 print(afile.data.shape)
             ```
         """
         self._afile_path = afile_path
+        self.settings = {}
         if mode == "r":
-            super().__init__(afile_path)
+            super().__init__(afile_path, mode=mode)
+            # load settings
+            if self.comment:
+                self.settings = json.loads(self.comment)
         else:
             _name = os.path.split(afile_path)[1].replace(".wav", "")
-            self._tmp = tempfile.NamedTemporaryFile(prefix=_name, suffix='.wav', dir="", delete=True)
-            super().__init__(self._tmp, mode=mode, samplerate=samplerate, channels=channels, subtype="PCM_24", format="WAV")
+            if temp:
+                self._tmp = tempfile.NamedTemporaryFile(prefix=_name, suffix='.wav', dir="", delete=True)
+                super().__init__(self._tmp, mode=mode, samplerate=samplerate, channels=channels, subtype="PCM_24", format="WAV")
+            else:
+                super().__init__(afile_path, mode=mode, samplerate=samplerate, channels=channels, subtype="PCM_24", format="WAV")
             now = datetime.now()
             # set wav metadata
             self.title = _name
             self.date = now.strftime("%d/%m/%Y %H:%M:%S")
     
     # store settings as json string in metadata "comment"
     @property
     def settings(self) -> dict:
         """Additional JSON settings in the metadata's comment field."""
-        if not self.comment:
-            return {}
-        else:
-            return json.loads(self.comment)
+        return self._settings
     @settings.setter
     def settings(self, value: dict) -> None:
-        self.comment = json.dumps(value)
+        self._settings = value
 
     @property
     def latency(self) -> int:
         """Latency in samples."""
         try:
             return int(self.settings["latency"])
         except KeyError:
             return None
     @latency.setter
     def latency(self, value: int) -> None:
-        settings = self.settings
-        settings["latency"] = int(value)
-        self.settings = settings
+        self.settings["latency"] = int(value)
 
     @property
     def data(self) -> np.ndarray:
         """Data of AFile as numpy array of shape ("samples" x "channels")."""
         self.flush()
         self.seek(0)
         return self.read(dtype="float32", always_2d=True)
     
-    def __getattr__(self, name):
+    def __exit__(self, *args):
         try:
-            return super().__getattr__(name)
-        except AttributeError:
-            return object.__getattribute__(self, name)
+            self.comment = json.dumps(self.settings)
+        except soundfile.LibsndfileError:
+            pass
+        self.close()
 
     def cal_latency(self, time):
         """Calculate and store loopback latency without physical connection.
 
         !!! warning
             Dont rely on this method, as it only calculates the ADC/DAC's internal latency. 
             Use [latency_from_rec.py](../examples.md/#latency_from_recpy) to compare this result with the real loopback calibration.
 
         Args:
             time (CData): The time object given in the Interface callback function.
         """
         self.latency = round((time.outputBufferDacTime-time.inputBufferAdcTime)*self.samplerate + 1) # the +1 was measured experimentally (could be the cable?)
-
-    def save_file(self):
-        """Persist the temporary file at the given afile_path."""
-        self.flush()
-        self._tmp.seek(0)
-        with open(self._afile_path, 'wb') as file:
-            shutil.copyfileobj(self._tmp, file)
```

### Comparing `asmu-0.0.1a7/asmu/analyzer.py` & `asmu-0.0.1a8/asmu/analyzer.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     def start_process_thread(self, stream):
         def runner(self, stream):
             while stream.active:
                 try:
                     self._process_queue()
                 except queue.Empty:
                     pass
+            # flush the remaining queue ater stream is closed
+            while not self._q.empty():
+                self._process_queue()
         threading.Thread(target=runner, args=(self, stream, )).start()
 
 
     def _get_fft(self) -> np.ndarray:
         raise NotImplementedError() # TODO: Move this to helper function
         return np.fft.rfft(self._q.get()*self._w, axis=0, norm="forward")*2/np.mean(self._w)
```

### Comparing `asmu-0.0.1a7/asmu/asetup.py` & `asmu-0.0.1a8/asmu/asetup.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a7/asmu/generator.py` & `asmu-0.0.1a8/asmu/generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,14 +57,42 @@
             return None
         elif length < self._blocksize:
             pad = np.zeros((self._blocksize, self._asfile.channels))
             pad[:length, :] = data
             return pad
         else:
             return data
+        
+class Vector(Generator):
+    def __init__(self, blocksize: int, vector:np.ndarray, queuesize=10):
+        """_summary_
+
+        Args:
+            blocksize (int): _description_
+            vector (np.ndarray): 2D Numpy vector to play with the shape [samples x channels].
+            queuesize (int, optional): _description_. Defaults to 10.
+        """
+        self._blocksize = blocksize
+        self._vector = np.copy(vector.astype(np.float32)).T # TODO - maybe improove this
+        self._idx = 0
+        super().__init__(queuesize)
+
+    def _gen(self) -> np.ndarray:
+        data = self._vector[self._idx:self._idx+self._blocksize, :]
+        self._idx += self._blocksize
+
+        length = np.ma.size(data, axis=0)
+        if data.size == 0:
+            return None
+        elif length < self._blocksize:
+            pad = np.zeros((self._blocksize, np.ma.size(data, axis=1)))
+            pad[:length, :] = data
+            return pad
+        else:
+            return data
 
 class Chirp(Generator):
     def __init__(self, samplerate: int, blocksize: int, f0: float, f1: float, duration: int, queuesize: int=10) -> None:
         self._samplerate = samplerate
         self._blocksize = blocksize
         
         t = np.arange(0, int(duration*samplerate)) / samplerate
```

### Comparing `asmu-0.0.1a7/asmu/io.py` & `asmu-0.0.1a8/asmu/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         """
         try:
             self._init_sounddevice(io)
         except AttributeError as exc:
             raise exc
         return sd.Stream(callback=self._callback, finished_callback=finished_callback)
     
-    def stop_stream(self, exc_type, exc_value, traceback) -> None:
+    def stop_stream(self) -> None:
         """Stops the interface stream.
 
         Raises:
             sd.CallbackStop: Stop the sounddevice Stream.
         """
         raise sd.CallbackStop
```

### Comparing `asmu-0.0.1a7/asmu/view.py` & `asmu-0.0.1a8/asmu/view.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a7/asmu.egg-info/PKG-INFO` & `asmu-0.0.1a8/asmu.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asmu
-Version: 0.0.1a7
+Version: 0.0.1a8
 Summary: Acoustic Signal Measurement Utilities
 Author-email: felhub <felhub@net4us.at>
 Project-URL: Repository, https://gitlab.com/felhub/asmu
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `asmu-0.0.1a7/pyproject.toml` & `asmu-0.0.1a8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asmu"
-version = "v0.0.1a7"
+version = "v0.0.1a8"
 authors = [
     {name = "felhub", email = "felhub@net4us.at"},
 ]
 description = "Acoustic Signal Measurement Utilities"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

