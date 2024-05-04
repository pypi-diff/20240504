# Comparing `tmp/copy-spotter-0.1.5.tar.gz` & `tmp/copy-spotter-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copy-spotter-0.1.5.tar", last modified: Sat May  4 12:54:03 2024, max compression
+gzip compressed data, was "copy-spotter-0.1.6.tar", last modified: Sat May  4 14:14:25 2024, max compression
```

## Comparing `copy-spotter-0.1.5.tar` & `copy-spotter-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:54:03.772446 copy-spotter-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-04 12:54:03.772446 copy-spotter-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:54:03.768446 copy-spotter-0.1.5/copy_spotter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-04 12:54:03.000000 copy-spotter-0.1.5/copy_spotter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-04 12:54:03.000000 copy-spotter-0.1.5/copy_spotter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 12:54:03.000000 copy-spotter-0.1.5/copy_spotter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 12:54:03.000000 copy-spotter-0.1.5/copy_spotter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-04 12:54:03.000000 copy-spotter-0.1.5/copy_spotter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 12:54:03.000000 copy-spotter-0.1.5/copy_spotter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:54:03.772446 copy-spotter-0.1.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/html_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/processing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-04 12:54:03.772446 copy-spotter-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:54:03.772446 copy-spotter-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:54:03.772446 copy-spotter-0.1.5/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/test_html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/test_html_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/test_processing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/test_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:25.662858 copy-spotter-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-04 14:14:25.662858 copy-spotter-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:25.658858 copy-spotter-0.1.6/copy_spotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-04 14:14:25.000000 copy-spotter-0.1.6/copy_spotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-04 14:14:25.000000 copy-spotter-0.1.6/copy_spotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 14:14:25.000000 copy-spotter-0.1.6/copy_spotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 14:14:25.000000 copy-spotter-0.1.6/copy_spotter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-04 14:14:25.000000 copy-spotter-0.1.6/copy_spotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 14:14:25.000000 copy-spotter-0.1.6/copy_spotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:25.662858 copy-spotter-0.1.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/scripts/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/scripts/html_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/scripts/processing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/scripts/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-04 14:14:25.662858 copy-spotter-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:25.662858 copy-spotter-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:25.662858 copy-spotter-0.1.6/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/tests/scripts/test_html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/tests/scripts/test_html_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/tests/scripts/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/tests/scripts/test_processing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/tests/scripts/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-04 14:14:10.000000 copy-spotter-0.1.6/tests/scripts/test_utils.py
```

### Comparing `copy-spotter-0.1.5/LICENSE` & `copy-spotter-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.5/PKG-INFO` & `copy-spotter-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-spotter
-Version: 0.1.5
+Version: 0.1.6
 Summary: Make plagiarism detection easier. This package will find similar sentences between given files and highlight them in a side by side comparison.
 Home-page: https://github.com/Wazzabeee/copy-spotter
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -31,14 +31,22 @@
 ```bash
 $ pip install copy-spotter
 $ copy-spotter [-s] [-o] [-h] input_directory
 ```
 ***Positional Arguments:***
 * `input_directory`: Directory that contains one folder per pdf file (see `data/pdf/plagiarism` for example)
 
+```
+input_directory/
+│
+├── file_1.docx
+├── file_2.pdf
+└── file_3.pdf
+```
+
 ***Optional Arguments:***
 * `-s`, `--block-size`: Set minimum number of consecutive and similar words detected. (Default is 2)
 * `-o`, `--out_dir`: Set the output directory for html files. (Default is creating a new directory called results)
 * `-h`, `--help`: Show this message and exit.
 
 **Examples**
 ---
@@ -84,12 +92,8 @@
 - Ensure you have writing access when using the package 
 - If a specific file is not processed correctly feel free to [contact me](mailto:<clement45.delteil45@gmail.com>) so that I can address the issue.
 
 **TODO**
 ---
 - Add more tests on existing functions
 - Implement OCR with tesseract for scanned documents
-- Add info in console for timing (tqdm)
-- Add CSS to HTML Template to make the results better looking
-- Add support for other folder structures (right now the package is expecting one pdf files per folder)
 - Add custom naming option for pdf files
-- Fix Slate3k by installing custom fork (check if still relevant)
```

### Comparing `copy-spotter-0.1.5/README.md` & `copy-spotter-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 ```bash
 $ pip install copy-spotter
 $ copy-spotter [-s] [-o] [-h] input_directory
 ```
 ***Positional Arguments:***
 * `input_directory`: Directory that contains one folder per pdf file (see `data/pdf/plagiarism` for example)
 
+```
+input_directory/
+│
+├── file_1.docx
+├── file_2.pdf
+└── file_3.pdf
+```
+
 ***Optional Arguments:***
 * `-s`, `--block-size`: Set minimum number of consecutive and similar words detected. (Default is 2)
 * `-o`, `--out_dir`: Set the output directory for html files. (Default is creating a new directory called results)
 * `-h`, `--help`: Show this message and exit.
 
 **Examples**
 ---
@@ -68,12 +76,8 @@
 - Ensure you have writing access when using the package 
 - If a specific file is not processed correctly feel free to [contact me](mailto:<clement45.delteil45@gmail.com>) so that I can address the issue.
 
 **TODO**
 ---
 - Add more tests on existing functions
 - Implement OCR with tesseract for scanned documents
-- Add info in console for timing (tqdm)
-- Add CSS to HTML Template to make the results better looking
-- Add support for other folder structures (right now the package is expecting one pdf files per folder)
-- Add custom naming option for pdf files
-- Fix Slate3k by installing custom fork (check if still relevant)
+- Add custom naming option for pdf files
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `copy-spotter-0.1.5/copy_spotter.egg-info/PKG-INFO` & `copy-spotter-0.1.6/copy_spotter.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-spotter
-Version: 0.1.5
+Version: 0.1.6
 Summary: Make plagiarism detection easier. This package will find similar sentences between given files and highlight them in a side by side comparison.
 Home-page: https://github.com/Wazzabeee/copy-spotter
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -31,14 +31,22 @@
 ```bash
 $ pip install copy-spotter
 $ copy-spotter [-s] [-o] [-h] input_directory
 ```
 ***Positional Arguments:***
 * `input_directory`: Directory that contains one folder per pdf file (see `data/pdf/plagiarism` for example)
 
+```
+input_directory/
+│
+├── file_1.docx
+├── file_2.pdf
+└── file_3.pdf
+```
+
 ***Optional Arguments:***
 * `-s`, `--block-size`: Set minimum number of consecutive and similar words detected. (Default is 2)
 * `-o`, `--out_dir`: Set the output directory for html files. (Default is creating a new directory called results)
 * `-h`, `--help`: Show this message and exit.
 
 **Examples**
 ---
@@ -84,12 +92,8 @@
 - Ensure you have writing access when using the package 
 - If a specific file is not processed correctly feel free to [contact me](mailto:<clement45.delteil45@gmail.com>) so that I can address the issue.
 
 **TODO**
 ---
 - Add more tests on existing functions
 - Implement OCR with tesseract for scanned documents
-- Add info in console for timing (tqdm)
-- Add CSS to HTML Template to make the results better looking
-- Add support for other folder structures (right now the package is expecting one pdf files per folder)
 - Add custom naming option for pdf files
-- Fix Slate3k by installing custom fork (check if still relevant)
```

### Comparing `copy-spotter-0.1.5/copy_spotter.egg-info/SOURCES.txt` & `copy-spotter-0.1.6/copy_spotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.5/scripts/html_utils.py` & `copy-spotter-0.1.6/scripts/html_utils.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.5/scripts/html_writing.py` & `copy-spotter-0.1.6/scripts/html_writing.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.5/scripts/main.py` & `copy-spotter-0.1.6/scripts/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from tqdm import tqdm
 
 from scripts.html_writing import add_links_to_html_table, results_to_html, papers_comparison
 from scripts.html_utils import writing_results
 from scripts.processing_files import file_extension_call
 from scripts.similarity import difflib_overlap
-from scripts.utils import wait_for_file, get_student_names, parse_options
+from scripts.utils import wait_for_file, parse_options
 
 
 class MinimumFilesError(Exception):
     """Raised when there are fewer than two files for comparison."""
 
     pass
 
@@ -58,36 +58,31 @@
     if not path.exists(in_dir):
         raise PathNotFoundError(f"The specified path does not exist: {in_dir}")
 
     if not path.isabs(in_dir):
         in_dir = path.abspath(in_dir)
 
     files = [
-        f for f in listdir(in_dir) if path.isdir(path.join(in_dir, f)) or f.endswith(("txt", "pdf", "docx", "odt"))
+        f for f in listdir(in_dir) if path.isfile(path.join(in_dir, f)) and f.endswith(("txt", "pdf", "docx", "odt"))
     ]
 
     if len(files) < 2:
         raise MinimumFilesError(
             "Minimum number of files is not present. Please check that there are at least two files to compare."
         )
 
     filenames, processed_files = [], []
-    students_names = get_student_names(in_dir)
 
-    for ind, direc in enumerate(tqdm(listdir(in_dir), desc="Processing Directories")):
-        if path.isdir(path.join(in_dir, direc)):
-            for file in listdir(path.join(in_dir, direc)):
-                file_words = file_extension_call(str(path.join(in_dir, direc, file)))
-                if file_words:  # If all files have supported format
-                    processed_files.append(file_words)
-                    filenames.append(students_names[ind])
-                else:
-                    raise UnsupportedFileError(
-                        "Remove files which are not txt, pdf, docx, or odt and run the script again."
-                    )
+    for file in tqdm(files, desc="Processing Files"):
+        file_words = file_extension_call(str(path.join(in_dir, file)))
+        if file_words:  # If all files have supported format
+            processed_files.append(file_words)
+            filenames.append(path.splitext(file)[0])
+        else:
+            raise UnsupportedFileError("Remove files which are not txt, pdf, docx, or odt and run the script again.")
 
     if out_dir is not None and path.exists(out_dir):
         if not path.isabs(out_dir):
             out_dir = path.abspath(out_dir)
         results_directory = out_dir
     else:
         results_directory = writing_results(datetime.now().strftime("%Y%m%d_%H%M%S"))
```

### Comparing `copy-spotter-0.1.5/scripts/processing_files.py` & `copy-spotter-0.1.6/scripts/processing_files.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,41 +9,37 @@
 from odf import text, teletype
 from odf.opendocument import load
 
 
 def get_file_extension(filepath: str) -> str:
     """Return the file extension of the file at the specified path"""
     if not path.isfile(filepath):
-        print("Invalid file path")
-        return ""
+        raise ValueError(f"Invalid file path: {filepath}")
 
     try:
         return path.splitext(filepath)[1]
     except IndexError:
-        print("File extension error")
-        return ""
+        raise ValueError(f"File extension error for file: {filepath}")
 
 
 def file_extension_call(file: str) -> list:
     """Map file extension to appropriate function"""
 
     extension = get_file_extension(file)
 
-    if extension:
-        if extension == ".pdf":
-            return get_words_from_pdf_file(file)
-        if extension == ".docx":
-            return get_words_from_docx_file(file)
-        if extension == ".odt":
-            return get_words_from_odt_file(file)
-        if extension == ".txt":
-            return get_words_from_txt_file(file)
-
-    print("File format is not supported. Please convert to pdf, docx, odt or txt")
-    return []
+    if extension == ".pdf":
+        return get_words_from_pdf_file(file)
+    elif extension == ".docx":
+        return get_words_from_docx_file(file)
+    elif extension == ".odt":
+        return get_words_from_odt_file(file)
+    elif extension == ".txt":
+        return get_words_from_txt_file(file)
+    else:
+        raise ValueError(f"File format not supported for file: {file}. " f"Please convert to pdf, docx, odt, or txt")
 
 
 def get_words_from_pdf_file(pdf_path: str) -> list:
     """Return list of words from pdf file at specified path"""
 
     with open(pdf_path, "rb") as file:
         extracted_text = slate.PDF(file)
```

### Comparing `copy-spotter-0.1.5/scripts/similarity.py` & `copy-spotter-0.1.6/scripts/similarity.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.5/scripts/utils.py` & `copy-spotter-0.1.6/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.5/setup.py` & `copy-spotter-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.5/tests/scripts/test_utils.py` & `copy-spotter-0.1.6/tests/scripts/test_utils.py`

 * *Files identical despite different names*

