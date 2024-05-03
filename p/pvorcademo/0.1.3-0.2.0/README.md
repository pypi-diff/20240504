# Comparing `tmp/pvorcademo-0.1.3.tar.gz` & `tmp/pvorcademo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvorcademo-0.1.3.tar", last modified: Thu Feb 15 15:41:37 2024, max compression
+gzip compressed data, was "pvorcademo-0.2.0.tar", last modified: Fri May  3 22:32:58 2024, max compression
```

## Comparing `pvorcademo-0.1.3.tar` & `pvorcademo-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-02-15 15:41:37.707230 pvorcademo-0.1.3/
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       59 2024-02-15 15:41:37.000000 pvorcademo-0.1.3/MANIFEST.in
--rw-r--r--   0 srinivasa  (1000) srinivasa  (1000)     2059 2024-02-15 15:41:37.707230 pvorcademo-0.1.3/PKG-INFO
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     1395 2024-01-26 22:38:54.000000 pvorcademo-0.1.3/README.md
-drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-02-15 15:41:37.707230 pvorcademo-0.1.3/pvorcademo/
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)    11344 2024-02-15 15:41:37.000000 pvorcademo-0.1.3/pvorcademo/LICENSE
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     2347 2024-02-15 15:41:37.000000 pvorcademo-0.1.3/pvorcademo/orca_demo.py
-drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-02-15 15:41:37.707230 pvorcademo-0.1.3/pvorcademo.egg-info/
--rw-r--r--   0 srinivasa  (1000) srinivasa  (1000)     2059 2024-02-15 15:41:37.000000 pvorcademo-0.1.3/pvorcademo.egg-info/PKG-INFO
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      279 2024-02-15 15:41:37.000000 pvorcademo-0.1.3/pvorcademo.egg-info/SOURCES.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)        1 2024-02-15 15:41:37.000000 pvorcademo-0.1.3/pvorcademo.egg-info/dependency_links.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       56 2024-02-15 15:41:37.000000 pvorcademo-0.1.3/pvorcademo.egg-info/entry_points.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       14 2024-02-15 15:41:37.000000 pvorcademo-0.1.3/pvorcademo.egg-info/requires.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       11 2024-02-15 15:41:37.000000 pvorcademo-0.1.3/pvorcademo.egg-info/top_level.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       38 2024-02-15 15:41:37.707230 pvorcademo-0.1.3/setup.cfg
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     1607 2024-02-15 15:28:49.000000 pvorcademo-0.1.3/setup.py
+drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-03 22:32:58.576616 pvorcademo-0.2.0/
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      101 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/MANIFEST.in
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     3069 2024-05-03 22:32:58.576616 pvorcademo-0.2.0/PKG-INFO
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     2377 2024-05-03 22:08:49.000000 pvorcademo-0.2.0/README.md
+drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-03 22:32:58.576616 pvorcademo-0.2.0/pvorcademo/
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)    11344 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo/LICENSE
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     2822 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo/orca_demo.py
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)    13421 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo/orca_demo_streaming.py
+drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-03 22:32:58.576616 pvorcademo-0.2.0/pvorcademo.egg-info/
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     3069 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo.egg-info/PKG-INFO
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      313 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo.egg-info/SOURCES.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)        1 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo.egg-info/dependency_links.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      115 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo.egg-info/entry_points.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       63 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo.egg-info/requires.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       11 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo.egg-info/top_level.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       38 2024-05-03 22:32:58.576616 pvorcademo-0.2.0/setup.cfg
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     1794 2024-05-03 22:26:21.000000 pvorcademo-0.2.0/setup.py
```

### Comparing `pvorcademo-0.1.3/pvorcademo/LICENSE` & `pvorcademo-0.2.0/pvorcademo/LICENSE`

 * *Files identical despite different names*

### Comparing `pvorcademo-0.1.3/pvorcademo/orca_demo.py` & `pvorcademo-0.2.0/pvorcademo/orca_demo.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,57 +7,79 @@
 #    Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 #    an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 #    specific language governing permissions and limitations under the License.
 #
 
 import argparse
 import struct
+import time
 import wave
 
 from pvorca import create, OrcaActivationLimitError
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         '--access_key',
+        '-a',
         required=True,
         help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)')
     parser.add_argument(
         '--text',
+        '-t',
         required=True,
         help='Text to be synthesized')
     parser.add_argument(
         '--output_path',
+        '-o',
         required=True,
         help='Absolute path to .wav file where the generated audio will be stored')
     parser.add_argument(
         '--library_path',
+        '-l',
         help='Absolute path to dynamic library. Default: using the library provided by `pvorca`')
     parser.add_argument(
         '--model_path',
+        '-m',
         help='Absolute path to Orca model. Default: using the model provided by `pvorca`')
     args = parser.parse_args()
 
-    if not args.output_path.lower().endswith('.wav'):
+    access_key = args.access_key
+    model_path = args.model_path
+    library_path = args.library_path
+    output_path = args.output_path
+    text = args.text
+
+    if not output_path.lower().endswith('.wav'):
         raise ValueError('Given argument --output_path must have WAV file extension')
 
-    orca = create(access_key=args.access_key, model_path=args.model_path, library_path=args.library_path)
+    orca = create(access_key=access_key, model_path=model_path, library_path=library_path)
 
     try:
-        print('Orca version: %s' % orca.version)
-        pcm = orca.synthesize(args.text)
+        print(f"Orca version: {orca.version}")
+
+        start = time.time()
+
+        pcm, alignments = orca.synthesize(text)
+
+        processing_time = time.time() - start
         length_sec = len(pcm) / orca.sample_rate
-        with wave.open(args.output_path, 'wb') as output_file:
+
+        with wave.open(output_path, "wb") as output_file:
             output_file.setnchannels(1)
             output_file.setsampwidth(2)
             output_file.setframerate(orca.sample_rate)
-            output_file.writeframes(struct.pack('%dh' % len(pcm), *pcm))
-        print('%.2f seconds of audio were written to `%s`.' % (length_sec, args.output_path))
+            output_file.writeframes(struct.pack(f"{len(pcm)}h", *pcm))
+
+        print(
+            f"Orca took {processing_time:.2f} seconds to synthesize {length_sec:.2f} seconds of speech which is "
+            f"~{length_sec / processing_time:.0f} times faster than real-time.")
+        print(f"Audio written to `{output_path}`.")
     except OrcaActivationLimitError:
-        print('AccessKey has reached its processing limit')
+        print("AccessKey has reached its processing limit")
     finally:
         orca.delete()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `pvorcademo-0.1.3/setup.py` & `pvorcademo-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 import os
 import shutil
 
 import setuptools
 
+INCLUDE_FILES = [
+    "../../LICENSE",
+    "orca_demo.py",
+    "orca_demo_streaming.py"]
 
-INCLUDE_FILES = ('../../LICENSE', 'orca_demo.py')
+os.system("git clean -dfx")
 
-os.system('git clean -dfx')
-
-package_folder = os.path.join(os.path.dirname(__file__), 'pvorcademo')
+package_folder = os.path.join(os.path.dirname(__file__), "pvorcademo")
 os.mkdir(package_folder)
 manifest_in = ""
 
 for rel_path in INCLUDE_FILES:
     shutil.copy(os.path.join(os.path.dirname(__file__), rel_path), package_folder)
     manifest_in += "include pvorcademo/%s\n" % os.path.basename(rel_path)
 
-with open(os.path.join(os.path.dirname(__file__), 'MANIFEST.in'), 'w') as f:
+with open(os.path.join(os.path.dirname(__file__), "MANIFEST.in"), "w") as f:
     f.write(manifest_in)
 
-with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
+with open(os.path.join(os.path.dirname(__file__), "README.md"), "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvorcademo",
-    version="0.1.3",
+    version="0.2.0",
     author="Picovoice",
     author_email="hello@picovoice.ai",
-    description="Orca Text-to-Speech Engine demos",
+    description="Orca Streaming Text-to-Speech Engine demos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/orca",
     packages=["pvorcademo"],
-    install_requires=["pvorca==0.1.4"],
+    install_requires=["numpy>=1.24.0", "pvorca==0.2.0", "sounddevice==0.4.6", "tiktoken==0.6.0"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Topic :: Multimedia :: Sound/Audio :: Speech"
     ],
     entry_points=dict(
         console_scripts=[
-            'orca_demo=pvorcademo.orca_demo:main',
+            "orca_demo=pvorcademo.orca_demo:main",
+            "orca_demo_streaming=pvorcademo.orca_demo_streaming:main",
         ],
     ),
-    python_requires='>=3.7',
-    keywords="Text-to-Speech, TTS, Speech Synthesis, Voice Generation, Speech Engine",
+    python_requires=">=3.8",
+    keywords="Streaming Text-to-Speech, TTS, Speech Synthesis, Voice Generation, Speech Engine",
 )
```

