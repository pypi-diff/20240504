# Comparing `tmp/copy-spotter-0.1.4.tar.gz` & `tmp/copy-spotter-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copy-spotter-0.1.4.tar", last modified: Wed May  1 14:49:21 2024, max compression
+gzip compressed data, was "copy-spotter-0.1.5.tar", last modified: Sat May  4 12:54:03 2024, max compression
```

## Comparing `copy-spotter-0.1.4.tar` & `copy-spotter-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/copy_spotter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-01 14:49:21.000000 copy-spotter-0.1.4/copy_spotter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-01 14:49:21.000000 copy-spotter-0.1.4/copy_spotter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:49:21.000000 copy-spotter-0.1.4/copy_spotter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 14:49:21.000000 copy-spotter-0.1.4/copy_spotter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-01 14:49:21.000000 copy-spotter-0.1.4/copy_spotter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 14:49:21.000000 copy-spotter-0.1.4/copy_spotter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/html_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/processing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/test_html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/test_html_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/test_processing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/test_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:54:03.772446 copy-spotter-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-04 12:54:03.772446 copy-spotter-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:54:03.768446 copy-spotter-0.1.5/copy_spotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-04 12:54:03.000000 copy-spotter-0.1.5/copy_spotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-04 12:54:03.000000 copy-spotter-0.1.5/copy_spotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 12:54:03.000000 copy-spotter-0.1.5/copy_spotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 12:54:03.000000 copy-spotter-0.1.5/copy_spotter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-04 12:54:03.000000 copy-spotter-0.1.5/copy_spotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 12:54:03.000000 copy-spotter-0.1.5/copy_spotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:54:03.772446 copy-spotter-0.1.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/html_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/processing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-04 12:54:03.772446 copy-spotter-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:54:03.772446 copy-spotter-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:54:03.772446 copy-spotter-0.1.5/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/test_html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/test_html_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/test_processing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-04 12:53:47.000000 copy-spotter-0.1.5/tests/scripts/test_utils.py
```

### Comparing `copy-spotter-0.1.4/LICENSE` & `copy-spotter-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.4/PKG-INFO` & `copy-spotter-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-spotter
-Version: 0.1.4
+Version: 0.1.5
 Summary: Make plagiarism detection easier. This package will find similar sentences between given files and highlight them in a side by side comparison.
 Home-page: https://github.com/Wazzabeee/copy-spotter
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `copy-spotter-0.1.4/README.md` & `copy-spotter-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.4/copy_spotter.egg-info/PKG-INFO` & `copy-spotter-0.1.5/copy_spotter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-spotter
-Version: 0.1.4
+Version: 0.1.5
 Summary: Make plagiarism detection easier. This package will find similar sentences between given files and highlight them in a side by side comparison.
 Home-page: https://github.com/Wazzabeee/copy-spotter
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `copy-spotter-0.1.4/copy_spotter.egg-info/SOURCES.txt` & `copy-spotter-0.1.5/copy_spotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.4/scripts/html_utils.py` & `copy-spotter-0.1.5/scripts/html_utils.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.4/scripts/html_writing.py` & `copy-spotter-0.1.5/scripts/html_writing.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.4/scripts/main.py` & `copy-spotter-0.1.5/scripts/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,27 +3,46 @@
 
 This modules compares all txt, docs, odt, pdf files present in path specified as argument.
 It writes results in a HTML table.
 It uses difflib library to find matching sequences.
 It can also use Jaccard Similarity, words counting, overlapping words for similarity
 
 """
-import sys
 import webbrowser
 from datetime import datetime
 from os import listdir, path
 from typing import List
 
+from tqdm import tqdm
+
 from scripts.html_writing import add_links_to_html_table, results_to_html, papers_comparison
 from scripts.html_utils import writing_results
 from scripts.processing_files import file_extension_call
 from scripts.similarity import difflib_overlap
 from scripts.utils import wait_for_file, get_student_names, parse_options
 
 
+class MinimumFilesError(Exception):
+    """Raised when there are fewer than two files for comparison."""
+
+    pass
+
+
+class UnsupportedFileError(Exception):
+    """Raised when there are unsupported files in the input directory."""
+
+    pass
+
+
+class PathNotFoundError(Exception):
+    """Raised when the specified input directory path does not exist."""
+
+    pass
+
+
 def main() -> None:
     """
     Main function to process and compare text files.
 
     Parses command-line arguments to obtain input and output directories and block size for comparison.
     Validates the input directory and checks if there are at least two files for comparison.
     Processes each file in the input directory, extracting text and handling different file formats.
@@ -32,74 +51,77 @@
     Creates a summary results HTML file with links to individual comparisons and opens it in a web browser.
     Exits the program if the specified path does not exist, or if there are fewer than two files for comparison.
     """
 
     args = parse_options()
     in_dir, out_dir, block_size = args.in_dir, args.out_dir, args.block_size
 
-    if path.exists(in_dir):  # Check if specified path exists
-        if not path.isabs(in_dir):
-            in_dir = path.abspath(in_dir)
-        if len(listdir(in_dir)) > 1:  # Check if there are at least 2 files at specified path
-            filenames, processed_files = [], []
-            students_names = get_student_names(in_dir)
-            for ind, direc in enumerate(listdir(in_dir)):
-                if path.isdir(path.join(in_dir, direc)):
-                    for file in listdir(path.join(in_dir, direc)):
-                        file_words = file_extension_call(str(path.join(in_dir, direc, file)))
-
-                        if file_words:  # If all files have supported format
-                            processed_files.append(file_words)
-                            filenames.append(students_names[ind])
-                        else:  # At least one file was not supported
-                            print("Remove files which are not txt, pdf, docx or odt and run the script again.")
-                            sys.exit()
-            if out_dir is not None and path.exists(out_dir):
-                if not path.isabs(out_dir):
-                    out_dir = path.abspath(out_dir)
-                results_directory = out_dir
-            else:
-                # Create new directory for storing html files
-                results_directory = writing_results(datetime.now().strftime("%Y%m%d_%H%M%S"))
+    if not path.exists(in_dir):
+        raise PathNotFoundError(f"The specified path does not exist: {in_dir}")
+
+    if not path.isabs(in_dir):
+        in_dir = path.abspath(in_dir)
+
+    files = [
+        f for f in listdir(in_dir) if path.isdir(path.join(in_dir, f)) or f.endswith(("txt", "pdf", "docx", "odt"))
+    ]
+
+    if len(files) < 2:
+        raise MinimumFilesError(
+            "Minimum number of files is not present. Please check that there are at least two files to compare."
+        )
+
+    filenames, processed_files = [], []
+    students_names = get_student_names(in_dir)
+
+    for ind, direc in enumerate(tqdm(listdir(in_dir), desc="Processing Directories")):
+        if path.isdir(path.join(in_dir, direc)):
+            for file in listdir(path.join(in_dir, direc)):
+                file_words = file_extension_call(str(path.join(in_dir, direc, file)))
+                if file_words:  # If all files have supported format
+                    processed_files.append(file_words)
+                    filenames.append(students_names[ind])
+                else:
+                    raise UnsupportedFileError(
+                        "Remove files which are not txt, pdf, docx, or odt and run the script again."
+                    )
+
+    if out_dir is not None and path.exists(out_dir):
+        if not path.isabs(out_dir):
+            out_dir = path.abspath(out_dir)
+        results_directory = out_dir
+    else:
+        results_directory = writing_results(datetime.now().strftime("%Y%m%d_%H%M%S"))
 
-            difflib_scores: List[List[float]] = [[] for _ in range(len(processed_files))]
-            file_ind = 0
+    difflib_scores: List[List[float]] = [[] for _ in range(len(processed_files))]
+    file_ind = 0
 
-            for i, text in enumerate(processed_files):
-                for j, text_bis in enumerate(processed_files):
-                    if i != j:
-                        # Append to the list the similarity score between text and text_bis
-                        difflib_scores[i].append(difflib_overlap(text, text_bis))
-
-                        # Write text with matching blocks colored in results directory
-                        papers_comparison(
-                            results_directory,
-                            file_ind,
-                            text,
-                            text_bis,
-                            (filenames[i], filenames[j]),
-                            block_size,
-                        )
-                        file_ind += 1
-                    else:
-                        difflib_scores[i].append(-1)
-
-            results_directory = path.join(results_directory, "_results.html")
-            print(results_directory)
-
-            results_to_html(difflib_scores, filenames, results_directory)
-
-            if wait_for_file(results_directory, 60):  # Wait for file to be created
-                add_links_to_html_table(results_directory)
-                webbrowser.open(results_directory)  # Open results HTML table
+    for i, text in enumerate(tqdm(processed_files, desc="Comparing Files")):
+        for j, text_bis in enumerate(processed_files):
+            if i != j:
+                difflib_scores[i].append(difflib_overlap(text, text_bis))
+                papers_comparison(
+                    results_directory,
+                    file_ind,
+                    text,
+                    text_bis,
+                    (filenames[i], filenames[j]),
+                    block_size,
+                )
+                file_ind += 1
             else:
-                print("Results file was not created...")
-        else:
-            print("Minimum number of files is not present. Please check that there are at least two files to compare.")
-            sys.exit()
+                difflib_scores[i].append(-1)
+
+    results_directory = path.join(results_directory, "_results.html")
+    print(f"Results saved at: {results_directory}")
+
+    results_to_html(difflib_scores, filenames, results_directory)
+
+    if wait_for_file(results_directory, 60):  # Wait for file to be created
+        add_links_to_html_table(results_directory)
+        webbrowser.open(results_directory)  # Open results HTML table
     else:
-        print("The specified path does not exist : " + in_dir)
-        sys.exit()
+        raise RuntimeError("Results file was not created...")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `copy-spotter-0.1.4/scripts/processing_files.py` & `copy-spotter-0.1.5/scripts/processing_files.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.4/scripts/similarity.py` & `copy-spotter-0.1.5/scripts/similarity.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.4/scripts/utils.py` & `copy-spotter-0.1.5/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.4/setup.py` & `copy-spotter-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.4/tests/scripts/test_utils.py` & `copy-spotter-0.1.5/tests/scripts/test_utils.py`

 * *Files identical despite different names*

