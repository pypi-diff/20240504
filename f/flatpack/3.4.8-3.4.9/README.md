# Comparing `tmp/flatpack-3.4.8.tar.gz` & `tmp/flatpack-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.4.8.tar", last modified: Thu May  2 14:59:36 2024, max compression
+gzip compressed data, was "flatpack-3.4.9.tar", last modified: Thu May  2 22:54:15 2024, max compression
```

## Comparing `flatpack-3.4.8.tar` & `flatpack-3.4.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:59:36.216545 flatpack-3.4.8/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.8/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 14:59:36.216280 flatpack-3.4.8/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.8/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:59:36.213283 flatpack-3.4.8/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.8/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.8/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:59:36.214770 flatpack-3.4.8/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.8/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-05-02 08:44:24.000000 flatpack-3.4.8/flatpack/engines/engine_llama_cpp.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.8/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-02 14:38:54.000000 flatpack-3.4.8/flatpack/load_engines.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26624 2024-05-02 14:58:46.000000 flatpack-3.4.8/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:59:36.215589 flatpack-3.4.8/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.8/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.8/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.8/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:59:36.215935 flatpack-3.4.8/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 14:59:36.000000 flatpack-3.4.8/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-02 14:59:36.000000 flatpack-3.4.8/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 14:59:36.000000 flatpack-3.4.8/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 14:59:36.000000 flatpack-3.4.8/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 14:59:36.000000 flatpack-3.4.8/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 14:59:36.000000 flatpack-3.4.8/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 14:59:36.216601 flatpack-3.4.8/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-02 14:56:51.000000 flatpack-3.4.8/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 22:54:15.770763 flatpack-3.4.9/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.9/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 22:54:15.770566 flatpack-3.4.9/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.9/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 22:54:15.768324 flatpack-3.4.9/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.9/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.9/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 22:54:15.769398 flatpack-3.4.9/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.9/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-05-02 08:44:24.000000 flatpack-3.4.9/flatpack/engines/engine_llama_cpp.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.9/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-02 14:38:54.000000 flatpack-3.4.9/flatpack/load_engines.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    27166 2024-05-02 17:28:01.000000 flatpack-3.4.9/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 22:54:15.770036 flatpack-3.4.9/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.9/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.9/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.9/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 22:54:15.770307 flatpack-3.4.9/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 22:54:15.000000 flatpack-3.4.9/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-02 22:54:15.000000 flatpack-3.4.9/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 22:54:15.000000 flatpack-3.4.9/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 22:54:15.000000 flatpack-3.4.9/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 22:54:15.000000 flatpack-3.4.9/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 22:54:15.000000 flatpack-3.4.9/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 22:54:15.770809 flatpack-3.4.9/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-02 15:56:21.000000 flatpack-3.4.9/setup.py
```

### Comparing `flatpack-3.4.8/LICENSE` & `flatpack-3.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.8/PKG-INFO` & `flatpack-3.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.8
+Version: 3.4.9
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.8/README.md` & `flatpack-3.4.9/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.8/flatpack/agent_manager.py` & `flatpack-3.4.9/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.8/flatpack/datasets.py` & `flatpack-3.4.9/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.8/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.4.9/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.8/flatpack/instructions.py` & `flatpack-3.4.9/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.8/flatpack/main.py` & `flatpack-3.4.9/flatpack/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,23 +149,23 @@
 distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing
 permissions and limitations under the License.
 {please_note}
 To accept, type 'YES'. To decline, type 'NO'.
 -----------------------------------------------------
-"""
+    """
 
     please_note_content = """
 PLEASE NOTE: The flatpack you are about to unbox is
 governed by its own licenses and terms, separate from
 this software. You may find further details at:
 
 https://fpk.ai/w/{}
-""".format(directory_name)
+    """.format(directory_name)
 
     please_note_colored = fpk_colorize(please_note_content, "yellow")
     print(disclaimer_template.format(please_note=please_note_colored))
 
 
 def fpk_encrypt_data(data: str, key: bytes) -> str:
     """Encrypt data using the provided key."""
@@ -465,14 +465,16 @@
                                          help='Build a model using the building script from the last unboxed flatpack.')
     parser_build.add_argument('directory', nargs='?', default=None, help='The directory of the flatpack to build.')
     parser_build.add_argument('--verbose', action='store_true', help='Display detailed outputs for debugging.')
     parser_build.set_defaults(func=lambda args, session: fpk_cli_handle_build(args, session))
 
     # Run server
     parser_run = subparsers.add_parser('run', help='Run the FastAPI server.')
+    parser_run.add_argument('input', nargs='?', default=None, help='The name of the flatpack to run.')
+    parser_run.add_argument('--verbose', action='store_true', help='Display detailed outputs for debugging.')
     parser_run.set_defaults(func=lambda args, session: fpk_cli_handle_run(args, session))
 
     # Vector database management
     parser_vector = subparsers.add_parser('vector', help='Vector database management')
     vector_subparsers = parser_vector.add_subparsers(dest='vector_command')
 
     parser_add_text = vector_subparsers.add_parser('add-texts',
@@ -575,14 +577,25 @@
 def fpk_cli_handle_list_agents(args, session):
     """List active agents."""
     agent_manager = AgentManager()
     agent_manager.list_agents()
 
 
 def fpk_cli_handle_run(args, session):
+    if not args.input:
+        print("❌ Please specify a flatpack for the run command.")
+        return
+
+    directory_name = args.input
+    existing_dirs = fpk_fetch_github_dirs(session)
+
+    if directory_name not in existing_dirs:
+        print(f"❌ The flatpack '{directory_name}' does not exist.")
+        return
+
     fpk_check_ngrok_auth()
     try:
         port = 8000
         listener = ngrok.forward(port, authtoken_from_env=True)
         print(f"Ingress established at {listener.url()}")
         uvicorn.run(app, host="0.0.0.0", port=port)
     except KeyboardInterrupt:
```

### Comparing `flatpack-3.4.8/flatpack/modules/lstm.py` & `flatpack-3.4.9/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.8/flatpack/modules/rnn.py` & `flatpack-3.4.9/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.8/flatpack/parsers.py` & `flatpack-3.4.9/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.8/flatpack/vector_manager.py` & `flatpack-3.4.9/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.8/flatpack.egg-info/PKG-INFO` & `flatpack-3.4.9/flatpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.8
+Version: 3.4.9
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.8/flatpack.egg-info/SOURCES.txt` & `flatpack-3.4.9/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.8/setup.py` & `flatpack-3.4.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.4.8",
+    version="3.4.9",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.2",
```

