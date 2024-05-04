# Comparing `tmp/PyLauncherMPI-0.1.5.tar.gz` & `tmp/pylaunchermpi-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLauncherMPI-0.1.5.tar", last modified: Wed May  1 14:23:25 2024, max compression
+gzip compressed data, was "pylaunchermpi-0.1.6.tar", last modified: Sat May  4 13:01:23 2024, max compression
```

## Comparing `PyLauncherMPI-0.1.5.tar` & `pylaunchermpi-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 14:23:25.867715 PyLauncherMPI-0.1.5/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1081 2024-05-01 12:21:07.000000 PyLauncherMPI-0.1.5/LICENSE
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     2565 2024-05-01 14:23:25.867715 PyLauncherMPI-0.1.5/PKG-INFO
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 14:23:25.867715 PyLauncherMPI-0.1.5/PyLauncherMPI.egg-info/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     2565 2024-05-01 14:23:25.000000 PyLauncherMPI-0.1.5/PyLauncherMPI.egg-info/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      298 2024-05-01 14:23:25.000000 PyLauncherMPI-0.1.5/PyLauncherMPI.egg-info/SOURCES.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 14:23:25.000000 PyLauncherMPI-0.1.5/PyLauncherMPI.egg-info/dependency_links.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       58 2024-05-01 14:23:25.000000 PyLauncherMPI-0.1.5/PyLauncherMPI.egg-info/entry_points.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2024-05-01 14:23:25.000000 PyLauncherMPI-0.1.5/PyLauncherMPI.egg-info/requires.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       14 2024-05-01 14:23:25.000000 PyLauncherMPI-0.1.5/PyLauncherMPI.egg-info/top_level.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1726 2024-05-01 13:26:59.000000 PyLauncherMPI-0.1.5/README.md
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 14:23:25.867715 PyLauncherMPI-0.1.5/pylaunchermpi/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 13:09:05.000000 PyLauncherMPI-0.1.5/pylaunchermpi/__init__.py
--rw-------   0 john_vm   (1000) john_vm   (1000)     3413 2024-05-01 14:21:35.000000 PyLauncherMPI-0.1.5/pylaunchermpi/main.py
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-01 14:23:25.867715 PyLauncherMPI-0.1.5/setup.cfg
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1195 2024-05-01 14:22:23.000000 PyLauncherMPI-0.1.5/setup.py
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-04 13:01:23.259848 pylaunchermpi-0.1.6/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1081 2024-05-01 12:21:07.000000 pylaunchermpi-0.1.6/LICENSE
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     2565 2024-05-04 13:01:23.259848 pylaunchermpi-0.1.6/PKG-INFO
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-04 13:01:23.259848 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     2565 2024-05-04 13:01:23.000000 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      298 2024-05-04 13:01:23.000000 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/SOURCES.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-04 13:01:23.000000 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/dependency_links.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       58 2024-05-04 13:01:23.000000 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/entry_points.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2024-05-04 13:01:23.000000 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/requires.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       14 2024-05-04 13:01:23.000000 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/top_level.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1726 2024-05-01 13:26:59.000000 pylaunchermpi-0.1.6/README.md
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-04 13:01:23.259848 pylaunchermpi-0.1.6/pylaunchermpi/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 13:09:05.000000 pylaunchermpi-0.1.6/pylaunchermpi/__init__.py
+-rw-------   0 john_vm   (1000) john_vm   (1000)     3080 2024-05-04 12:56:47.000000 pylaunchermpi-0.1.6/pylaunchermpi/main.py
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-04 13:01:23.259848 pylaunchermpi-0.1.6/setup.cfg
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1195 2024-05-04 12:59:26.000000 pylaunchermpi-0.1.6/setup.py
```

### Comparing `PyLauncherMPI-0.1.5/LICENSE` & `pylaunchermpi-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLauncherMPI-0.1.5/PKG-INFO` & `pylaunchermpi-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLauncherMPI
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.
 Home-page: https://github.com/ioannis-vm/PyLauncherMPI
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `PyLauncherMPI-0.1.5/PyLauncherMPI.egg-info/PKG-INFO` & `pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLauncherMPI
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.
 Home-page: https://github.com/ioannis-vm/PyLauncherMPI
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `PyLauncherMPI-0.1.5/README.md` & `pylaunchermpi-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `PyLauncherMPI-0.1.5/pylaunchermpi/main.py` & `pylaunchermpi-0.1.6/pylaunchermpi/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,27 @@
 from mpi4py import MPI
 import os
 import subprocess
 from datetime import datetime
 from time import perf_counter
-import hashlib
+from time import sleep
 
 
 def message(text):
     """
     Prints a message to stdout including the process ID and a
     timestamp.
 
     """
     comm = MPI.COMM_WORLD
     rank = comm.Get_rank()
     current_time = datetime.now()
     time_string = current_time.strftime("%H:%M:%S")
     message = f'{time_string} | Process {rank}: ' + text
-    print(message)
-
-
-def generate_hash(s):
-    """
-    Uses SHA-256 to hash a given string and then encode the result to
-    a 6-character string.
-
-    Parameters
-    ----------
-    s: string
-        The string to hash
-
-    Returns
-    -------
-    str
-        6-charachter hash
-
-    """
-
-    hash_object = hashlib.sha256(s.encode())
-    hex_dig = hash_object.hexdigest()  # Convert to hexadecimal
-    return hex_dig[:6]  # Return the first 6 characters
+    print(message, flush=True)
 
 
 def main():
 
     t_start = perf_counter()
 
     # Initialize the MPI environment
@@ -90,29 +68,31 @@
             allocated_commands[i % size].append(command)
     else:
         allocated_commands = None
 
     # Distribute the commands
     commands_for_process = comm.scatter(allocated_commands, root=0)
 
+    # Wait a bit for other processes to perform their IO operations
+    sleep(rank / 1000.00)  # i.e., process 1000 will start after 1 sec
+
     # Each process runs its allocated commands
     for command in commands_for_process:
-        command_hash = generate_hash(command)
-        message(f"Executing command {command_hash}: `{command}`")
+        message(f"Executing command: `{command}`")
         out = subprocess.run(command, capture_output=True, shell=True)
         if out.returncode == 0:
             message(
-                f'Command {command_hash} '
+                f'Command `{command}` '
                 f'finished successfully. '
                 f'stderr: `{out.stderr}`. '
                 f'stdout: `{out.stdout}`.'
             )
         else:
             message(
-                f'There was an error with {command_hash}. '
+                f'There was an error with command `{command}`. '
                 f'stderr: `{out.stderr}`. '
                 f'stdout: `{out.stdout}`.'
             )
 
     t_end = perf_counter()
 
     message(f'Done with all tasks. ' f'Elapsed time: {t_end - t_start:.2f} s.')
```

### Comparing `PyLauncherMPI-0.1.5/setup.py` & `pylaunchermpi-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PyLauncherMPI',
-    version='0.1.5',
+    version='0.1.6',
     author='John Vouvakis Manousakis',
     author_email='ioannis_vm@berkeley.edu',
     description=(
         'A simple MPI-based task scheduler for dynamically '
         'distributing commands across MPI processes.'
     ),
     long_description=open('README.md').read(),
```

