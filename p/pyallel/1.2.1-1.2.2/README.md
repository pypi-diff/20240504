# Comparing `tmp/pyallel-1.2.1.tar.gz` & `tmp/pyallel-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyallel-1.2.1.tar", max compression
+gzip compressed data, was "pyallel-1.2.2.tar", max compression
```

## Comparing `pyallel-1.2.1.tar` & `pyallel-1.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-12-20 08:59:25.146414 pyallel-1.2.1/LICENSE
--rw-r--r--   0        0        0     4983 2024-04-23 11:39:12.544453 pyallel-1.2.1/README.md
--rw-r--r--   0        0        0     1047 2024-04-23 11:40:29.451691 pyallel-1.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-20 08:59:25.146880 pyallel-1.2.1/src/pyallel/__init__.py
--rw-r--r--   0        0        0      893 2024-03-07 08:35:52.711592 pyallel-1.2.1/src/pyallel/colours.py
--rw-r--r--   0        0        0      571 2024-04-23 11:33:30.180565 pyallel-1.2.1/src/pyallel/constants.py
--rw-r--r--   0        0        0      368 2023-12-20 08:59:25.146977 pyallel-1.2.1/src/pyallel/errors.py
--rw-r--r--   0        0        0     2190 2024-04-22 08:12:02.701958 pyallel-1.2.1/src/pyallel/main.py
--rw-r--r--   0        0        0     2799 2024-04-22 08:12:02.702095 pyallel-1.2.1/src/pyallel/parser.py
--rw-r--r--   0        0        0     1830 2024-04-22 08:12:02.702258 pyallel-1.2.1/src/pyallel/process.py
--rw-r--r--   0        0        0    10864 2024-04-23 11:25:05.548244 pyallel-1.2.1/src/pyallel/process_group.py
--rw-r--r--   0        0        0     2919 2024-04-22 08:12:02.702497 pyallel-1.2.1/src/pyallel/process_group_manager.py
--rw-r--r--   0        0        0        0 2023-12-20 08:59:25.147305 pyallel-1.2.1/src/pyallel/py.typed
--rw-r--r--   0        0        0     5891 1970-01-01 00:00:00.000000 pyallel-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-12-10 12:28:31.474872 pyallel-1.2.2/LICENSE
+-rw-r--r--   0        0        0     4816 2024-05-04 09:12:18.605062 pyallel-1.2.2/README.md
+-rw-r--r--   0        0        0     1047 2024-05-04 09:11:54.176818 pyallel-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-10 12:28:31.486873 pyallel-1.2.2/src/pyallel/__init__.py
+-rw-r--r--   0        0        0      893 2024-04-13 11:42:32.468688 pyallel-1.2.2/src/pyallel/colours.py
+-rw-r--r--   0        0        0      571 2024-04-27 09:07:06.951363 pyallel-1.2.2/src/pyallel/constants.py
+-rw-r--r--   0        0        0      368 2023-12-10 16:41:29.922819 pyallel-1.2.2/src/pyallel/errors.py
+-rw-r--r--   0        0        0     2190 2024-04-27 11:37:14.693370 pyallel-1.2.2/src/pyallel/main.py
+-rw-r--r--   0        0        0     2799 2024-04-27 11:37:14.693370 pyallel-1.2.2/src/pyallel/parser.py
+-rw-r--r--   0        0        0     1830 2024-04-21 10:06:23.117760 pyallel-1.2.2/src/pyallel/process.py
+-rw-r--r--   0        0        0    11841 2024-05-04 09:07:28.510120 pyallel-1.2.2/src/pyallel/process_group.py
+-rw-r--r--   0        0        0     2919 2024-04-27 11:37:14.693370 pyallel-1.2.2/src/pyallel/process_group_manager.py
+-rw-r--r--   0        0        0        0 2023-12-10 12:28:32.010876 pyallel-1.2.2/src/pyallel/py.typed
+-rw-r--r--   0        0        0     5724 1970-01-01 00:00:00.000000 pyallel-1.2.2/PKG-INFO
```

### Comparing `pyallel-1.2.1/LICENSE` & `pyallel-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyallel-1.2.1/README.md` & `pyallel-1.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -115,17 +115,14 @@
 ```
 
 ## TODOs
 
 - [x] Add support to have commands depend on other commands (some commands must complete
       before a given command can start)
 - [ ] Add a debug mode that logs debug information to a log file
-- [ ] Fix wrapping of long commands in the command status line
-- [ ] Fix wrapping of very long lines in command output that pushes other commands off the
-      screen
 - [ ] Add support to state how many lines a command can use for it's output in interactive mode
 - [ ] Maybe add support to allow the user to provide stdin for commands that request it
       (such as a REPL)
 - [ ] Add custom parsing of command output to support filtering for errors (like vim's
       `errorformat`)
 - [ ] Allow list of files to be provided to supply as input arguments to each command
 - [ ] Allow input to be piped into `pyallel` via stdin to supply as standard input to each
```

### Comparing `pyallel-1.2.1/pyproject.toml` & `pyallel-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyallel"
-version = "1.2.1"
+version = "1.2.2"
 description = "Run and handle the output of multiple executables in pyallel (as in parallel)"
 authors = ["Daniel Black <danielcrblack@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Danthewaann/pyallel"
 repository = "https://github.com/Danthewaann/pyallel"
 keywords = ["parallel", "command", "runner", "executable", "shell", "terminal"]
```

### Comparing `pyallel-1.2.1/src/pyallel/colours.py` & `pyallel-1.2.2/src/pyallel/colours.py`

 * *Files identical despite different names*

### Comparing `pyallel-1.2.1/src/pyallel/constants.py` & `pyallel-1.2.2/src/pyallel/constants.py`

 * *Files identical despite different names*

### Comparing `pyallel-1.2.1/src/pyallel/main.py` & `pyallel-1.2.2/src/pyallel/main.py`

 * *Files identical despite different names*

### Comparing `pyallel-1.2.1/src/pyallel/parser.py` & `pyallel-1.2.2/src/pyallel/parser.py`

 * *Files identical despite different names*

### Comparing `pyallel-1.2.1/src/pyallel/process.py` & `pyallel-1.2.2/src/pyallel/process.py`

 * *Files identical despite different names*

### Comparing `pyallel-1.2.1/src/pyallel/process_group.py` & `pyallel-1.2.2/src/pyallel/process_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 
 def get_num_lines(output: str, columns: int | None = None) -> int:
     lines = 0
     columns = columns or constants.COLUMNS()
     for line in output.splitlines():
         line = constants.ANSI_ESCAPE.sub("", line)
         length = len(line)
-        lines += 1 * (length // columns + 1 if length > columns else 1)
+        line_lines = 1
+        if length > columns:
+            line_lines = length // columns
+            remainder = length % columns
+            if remainder:
+                line_lines += 1
+        lines += 1 * line_lines
     return lines
 
 
 def format_time_taken(time_taken: float) -> str:
     time_taken = round(time_taken, 1)
     seconds = time_taken % (24 * 3600)
 
@@ -254,50 +260,65 @@
         for i in range(num_processes):
             self.process_lines[i] = tail
         if remainder:
             self.process_lines[-1] += remainder - 2
         else:
             self.process_lines[-1] -= 2
 
-        output = ""
+        output = f"lines = {constants.LINES()}, process_lines = {self.process_lines}\n"
         for i, process in enumerate(self.processes, start=1):
+            process_output = ""
             if process.poll() is not None:
                 self.completed_processes.add(process.id)
                 if process.return_code() != 0:
                     self.passed = False
-                output += self._get_command_status(
+                process_output += self._get_command_status(
                     process,
                     passed=process.return_code() == 0,
                     timer=self.timer,
                 )
-                output += "\n"
+                process_output += "\n"
             else:
-                output += self._get_command_status(
+                process_output += self._get_command_status(
                     process,
                     icon=constants.ICONS[self.icon],
                     timer=self.timer,
                 )
-                output += "\n"
+                process_output += "\n"
 
-            process_output = process.read().decode()
+            command_lines = get_num_lines(process_output)
+            p_output = process.read().decode()
             if not self.output[process.id]:
                 self.output[process.id].append("")
-            self.output[process.id][0] += process_output
-            process_output = self.output[process.id][0]
-            if process_output:
+            self.output[process.id][0] += p_output
+            p_output = self.output[process.id][0]
+            p_output_lines = 0
+            if p_output:
                 if not all:
-                    process_output = "\n".join(
-                        process_output.splitlines()[-self.process_lines[i - 1] :]
-                    )
-                    process_output += "\n"
-                output += self._prefix(process_output)
-                if output and output[-1] != "\n":
-                    output += "\n"
+                    p_output_lines = p_output.splitlines()[-self.process_lines[i - 1] :]
+                    p_output = ""
+                    for line in p_output_lines:
+                        if len(line) + 3 > constants.COLUMNS():
+                            p_output += f"{''.join(line[:constants.COLUMNS()-3])}\n"
+                        else:
+                            p_output += line + "\n"
+                p_output = self._prefix(p_output)
+                if p_output and p_output[-1] != "\n":
+                    p_output += "\n"
                 if i != num_processes:
-                    output += "\n"
+                    p_output += "\n"
+                p_output_lines = get_num_lines(p_output)
+
+            if not all and (command_lines + p_output_lines) > self.process_lines[i - 1]:
+                truncate = (command_lines + p_output_lines) - self.process_lines[i - 1]
+                p_output = "\n".join(p_output.splitlines()[truncate:])
+                p_output += "\n"
+
+            process_output += p_output
+            output += process_output
 
         if self.interrupt_count == 0:
             return output
 
         if self.interrupt_count == 1:
             output += (
                 f"\n{self.colours.yellow_bold}Interrupt!{self.colours.reset_colour}"
```

### Comparing `pyallel-1.2.1/src/pyallel/process_group_manager.py` & `pyallel-1.2.2/src/pyallel/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `pyallel-1.2.1/PKG-INFO` & `pyallel-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyallel
-Version: 1.2.1
+Version: 1.2.2
 Summary: Run and handle the output of multiple executables in pyallel (as in parallel)
 Home-page: https://github.com/Danthewaann/pyallel
 License: MIT
 Keywords: parallel,command,runner,executable,shell,terminal
 Author: Daniel Black
 Author-email: danielcrblack@gmail.com
 Requires-Python: >=3.8,<3.13
@@ -137,17 +137,14 @@
 ```
 
 ## TODOs
 
 - [x] Add support to have commands depend on other commands (some commands must complete
       before a given command can start)
 - [ ] Add a debug mode that logs debug information to a log file
-- [ ] Fix wrapping of long commands in the command status line
-- [ ] Fix wrapping of very long lines in command output that pushes other commands off the
-      screen
 - [ ] Add support to state how many lines a command can use for it's output in interactive mode
 - [ ] Maybe add support to allow the user to provide stdin for commands that request it
       (such as a REPL)
 - [ ] Add custom parsing of command output to support filtering for errors (like vim's
       `errorformat`)
 - [ ] Allow list of files to be provided to supply as input arguments to each command
 - [ ] Allow input to be piped into `pyallel` via stdin to supply as standard input to each
```

