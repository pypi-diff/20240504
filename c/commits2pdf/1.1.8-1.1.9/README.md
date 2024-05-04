# Comparing `tmp/commits2pdf-1.1.8.tar.gz` & `tmp/commits2pdf-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commits2pdf-1.1.8.tar", last modified: Wed May  1 09:15:24 2024, max compression
+gzip compressed data, was "commits2pdf-1.1.9.tar", last modified: Fri May  3 09:02:01 2024, max compression
```

## Comparing `commits2pdf-1.1.8.tar` & `commits2pdf-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:15:24.061236 commits2pdf-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-05-01 09:15:24.061236 commits2pdf-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:15:24.061236 commits2pdf-1.1.8/commits2pdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    14282 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/commits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/render_cairo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/render_fpdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:15:24.061236 commits2pdf-1.1.8/commits2pdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-05-01 09:15:24.000000 commits2pdf-1.1.8/commits2pdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-01 09:15:24.000000 commits2pdf-1.1.8/commits2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:15:24.000000 commits2pdf-1.1.8/commits2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 09:15:24.000000 commits2pdf-1.1.8/commits2pdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 09:15:24.000000 commits2pdf-1.1.8/commits2pdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 09:15:24.000000 commits2pdf-1.1.8/commits2pdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 09:15:24.061236 commits2pdf-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:02:01.085420 commits2pdf-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 09:01:50.000000 commits2pdf-1.1.9/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-05-03 09:02:01.085420 commits2pdf-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-03 09:01:50.000000 commits2pdf-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:02:01.085420 commits2pdf-1.1.9/commits2pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:01:50.000000 commits2pdf-1.1.9/commits2pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-03 09:01:50.000000 commits2pdf-1.1.9/commits2pdf/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-05-03 09:01:50.000000 commits2pdf-1.1.9/commits2pdf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12401 2024-05-03 09:01:50.000000 commits2pdf-1.1.9/commits2pdf/commits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-03 09:01:50.000000 commits2pdf-1.1.9/commits2pdf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-03 09:01:50.000000 commits2pdf-1.1.9/commits2pdf/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-03 09:01:50.000000 commits2pdf-1.1.9/commits2pdf/render_cairo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-05-03 09:01:50.000000 commits2pdf-1.1.9/commits2pdf/render_fpdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:02:01.085420 commits2pdf-1.1.9/commits2pdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-05-03 09:02:01.000000 commits2pdf-1.1.9/commits2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-03 09:02:01.000000 commits2pdf-1.1.9/commits2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:02:01.000000 commits2pdf-1.1.9/commits2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-03 09:02:01.000000 commits2pdf-1.1.9/commits2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 09:02:01.000000 commits2pdf-1.1.9/commits2pdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 09:02:01.000000 commits2pdf-1.1.9/commits2pdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:02:01.085420 commits2pdf-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-03 09:01:50.000000 commits2pdf-1.1.9/setup.py
```

### Comparing `commits2pdf-1.1.8/LICENCE.md` & `commits2pdf-1.1.9/LICENCE.md`

 * *Files identical despite different names*

### Comparing `commits2pdf-1.1.8/PKG-INFO` & `commits2pdf-1.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commits2pdf
-Version: 1.1.8
+Version: 1.1.9
 Summary: View a filtered commit history in PDF form.
 Home-page: https://github.com/tomasvana10/commits2pdf
 Author: Tomas Vana
 License: MIT
 Platform: any
 Classifier: Topic :: Multimedia
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,31 +19,34 @@
 Classifier: Topic :: Education
 Classifier: Topic :: Office/Business
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 Requires-Dist: GitPython
 Requires-Dist: pycairo
 Requires-Dist: fpdf
-Requires-Dist: progressbar
+Requires-Dist: tqdm
 
 ![Licence](https://img.shields.io/badge/licence-MIT-green?style=flat?logo=licence)
 [![PyPI version](https://img.shields.io/pypi/v/commits2pdf?style=flat-square)](https://pypi.org/project/commits2pdf/)
 [![Publish to PyPI.org](https://github.com/tomasvana10/commits2pdf/actions/workflows/publish.yml/badge.svg)](https://github.com/tomasvana10/commits2pdf/actions/workflows/publish.yml)
 [![Release)](https://img.shields.io/github/v/release/tomasvana10/commits2pdf?logo=github)](https://github.com/tomasvana10/commits2pdf/releases/latest)
 [![Issues](https://img.shields.io/github/issues-raw/tomasvana10/commits2pdf.svg?maxAge=25000)](https://github.com/tomasvana10/commits2pdf/issues)
 [![CodeQL](https://github.com/tomasvana10/commits2pdf/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/tomasvana10/commits2pdf/actions/workflows/github-code-scanning/codeql)
 [![Tests](https://github.com/tomasvana10/commits2pdf/actions/workflows/tox-tests.yml/badge.svg)](https://github.com/tomasvana10/commits2pdf/actions/workflows/tox-tests.yml)
 
 # commits2pdf
 Visualise a GitHub repository's commit history in PDF form via the command-line
+---
+![ezgif-pdf-tutorial](https://github.com/tomasvana10/commits2pdf/assets/124552709/fcc4b5da-2326-4405-80fe-cf984f61129c)
 <br><br>
 ## Dependencies
 `pycairo`<br>
 `GitPython`<br>
-`fpdf`
+`fpdf`<br>
+`progressbar`
 <br><br>
 ## Installation
 **Requires [pip](https://pip.pypa.io/en/stable/installation/)**
 
 Make a virtual environment (recommended)
 ```
 pip install virtualenv OR pip3 install virtualenv
@@ -52,140 +55,104 @@
 ON WINDOWS: venv\scripts\activate
 ```
 
 Install the package in your system directory/virtual environment:
 ```
 pip install -U commits2pdf OR pip3 install -U commits2pdf
 ```
-OR, install the package in your home directory (good if you aren't using a virtual environment):
+OR, install the package in your home directory if you aren't using a virtual environment:
 ```
 pip install --user -U commits2pdf
 ```
 
 
 **If you encounter errors with building `pycairo`, click [here](https://stackoverflow.com/a/76175684/23245953)**
 <br><br>
+
 ## Command-line parameters
 ```
 positional arguments:
   owner                 The owner of the git repository. Required.
 
 options:
   -h, --help            show this help message and exit
   -o OUTPUT, --output OUTPUT
-                        Directory path to your PDF output. Set to "." by default. Will be created if it does not exist. Example: -o ./work/my_pdfs
+                        Directory path to your PDF output. Set to "." (your current directory) by default. Will be created if it does not exist. Example:
+                        ./work/my_pdfs
   -b BRANCH, --branch BRANCH
                         The repository branch. Set to "main" by default.
   -a AUTHORS, --authors AUTHORS
-                        Filter commits from a comma-separated list of authors. Format: <author@email.com> OR <author1@email.com,author2@email.com> etc. Set to all authors by
-                        default.
+                        Filter commits from a comma-separated list of authors. Format: <author@email.com> OR <author1@email.com,author2@email.com> etc. Set to all      
+                        authors by default.
   -s START_DATE, --start_date START_DATE
-                        Filter from start date of commits. Format: YYYY-mm-dd or YYYY-m-d. Example: 2023-12-05
+                        Filter from start date of commits. Format: d/m/YYYY. Example: 5/12/2023
   -e END_DATE, --end_date END_DATE
-                        Filter to end date of commits. Format: YYYY-mm-dd or YYYY-m-d. Example: 2023-12-05
+                        Filter to end date of commits. Format: d/m/YYYY. Example: 5/12/2023
   -r, --reverse         Output the commits from newest to oldest. Set to oldest to newest by default
-  -d, --dark            Toggle dark mode for the output PDF. Set to "light" by default.
+  -dark                 Toggle dark mode for the output PDF. Set to "light" by default.
   -po, --prevent-open   Prevent commits2pdf from automatically opening the directory the PDF was created in.
   -sc SCALING, --scaling SCALING
                         Set the scaling of the output PDF. Only available with gen2a and gen2b.
+  -in INCLUDE, --include INCLUDE
+                        Include commits with the given string sequences in their title or description. Format: "<string1>" OR "<string1,string2>". Whitespace
+                        sensitive and case insensitive. NOTE: This query is performed BEFORE excluding commits.
+  -ex EXCLUDE, --exclude EXCLUDE
+                        Exclude commits with the given string sequences in their title or description. Format: "<string1>" OR "<string1,string2>". Whitespace
+                        sensitive and case insensitive.
   -gen1, --pdf_gen_1    PDF rendering implementation with ``pycairo``.
   -gen2a, --pdf_gen_2a  The first PDF rendering implementation with ``fpdf``.
   -gen2b, --pdf_gen_2b  The second PDF rendering implementation with ``pycairo``. The default option.
-  -qa QUERIES_ANY, --query-any QUERIES_ANY
-                        Select the commits whose title OR description match ANY part of your query. Format: "<query1>" OR "<query1,query2>" etc. Note: queries can have leading or    
-                        trailing whitespace.
-  -QA QUERIES_ALL, --query-all QUERIES_ALL
-                        Select the commits whose title OR description match ALL parts of your query. Format: "<query1>" OR "<query1,query2>" etc. Note: queries can have leading or   
-                        trailing whitespace.
   -rp RPATH, --repo-path RPATH
-                        Path to your repository directory. Set to "." by default.
+                        Path to your repository directory. Set to "." (your current directory) by default.
   -fc RNAME, --repo-from-clone RNAME
                         Clone a repo into the working directory and generate the commits PDF from it automatically. Format: <repo name> (case insensitive).
   -nnc NEWEST_N_COMMITS, --newest-n-commits NEWEST_N_COMMITS
                         Select the newest n number amount of commits to include after filtering.
   -onc OLDEST_N_COMMITS, --oldest-n-commits OLDEST_N_COMMITS
                         Select the oldest n number amount of commits to include after filtering.
 ```
-<br>
 
 ## Usage
-<br>**Simple usage - what you will be using the most**:
+**Usage example #1**
 ```
 c2p tomasvana10
 ```
-_Explanation_: Run the CLI tool in the current directory (assuming it is a Git repository). The owner name must be provided in all cases.
-
-<br>**Advanced usage example #1**:
-```
-c2p tomasvana10 -rp ../seriescalculator_sdd -a person@email.com,other_person@gmail.com -s 2024-11-30 -e 2024-12-30 -b other_branch -d
-```
-_Explanation_: 
-1. Override the default repository path (``-rp ..\seriescalculator_sdd``) with a folder in the parent directory.
-2. Look for specific commit emails (separated by commas)
-3. Search for commits from the -s date until the -e date
-4. Search for commits only made to `other_branch`
-5. Toggle dark mode for the PDF output
+> Output a PDF to your current directory (assuming it is a git repository that is owned by `tomasvana10`).
 
-<br>**Advanced usage example #2**
+<br>**Usage example #2**
 ```
-c2p tomasvana10 -nnc 10 -r
+c2p tomasvana10 -o .. -rp ./my_repo
 ```
-_Explanation_: Display the newest ten commits (after any filtering) in reverse order (newest to oldest instead of the default, which is oldest to newest).
+> Output a PDF to the parent directory, selecting `./my_repo` as your git repository to access the commits from.
 
-<br>**Advanced usage example #3**
+<br>**Usage example #3**
 ```
-c2p tomasvana10 -qa "javascript,test " -onc 5 -po -o ..
+c2p tomasvana10 -nnc 10 -in "javascript,build" -ex "testing"
 ```
-_Explanation_: 
-1. Display the 5 oldest commits after querying the current repository's commits for either "javascript" OR "test "
-2. Prevent the PDF directory from being automatically opened.
-3. Output the PDF to the parent directory (`..`)
-
-**NOTE**: -qa selects commits that include **any** query criteria in the title **OR** description, while -QA selects commits that include **ALL** query criteria in the title or description.
+> Output a PDF to the current directory, displaying the newest 10 commits after filtering commits that contain "javascript" or "build in their title or description and do not contain "testing"
 
-<br>**Advanced usage example #4**
+<br>**Usage example #4**
 ```
-c2p tomasvana10 -QA "dev ,testing" -gen2a -sc 0.8
+c2p devguarv -fc Yr-12-HSC-SDD-Task-2 -e 28/4/2024
 ```
-_Explanation_:
-1. Query the repo for both "dev " AND "testing"
-2. Use the `gen2a` PDF renderer to visualise the PDF
-3. Set the scaling of the PDF output to 0.8
-
-**NOTE**: Scaling (`-sc`) is only available when using `gen2a` or `gen2b`. `gen2b` is default.
+> Clone the repo `Yr-12-HSC-SDD-Task-2` into the current directory and output a PDF into the same place after filtering commits that were made up to `28/4/2024`
+<br>
 
-<br>**Clone the repo you want to document on-demand**:
-```
-c2p tomasvana10 -fc some_repo_name
-```
-_Explanation_: Create the repo you have specified and make the PDF. This repo is always cloned into the current working directory.
-<br><br>
 ## PDF Generation implementations
 ### pycairo (gen1)
-+ Fast
-- Looks like crap 
-- No hyperlinks, therefore the entire link to a commit's diff is displayed
-- Occasional bugs in rendering
+👍 Fast<br>
+👎 Cannot write multipage commits<br>
+👎 Looks like crap<br>
+👎 No hyperlinks, therefore the entire link to a commit's diff is displayed
 
 ### fpdf (gen2a)
-+ Fast
-+ Can be scaled with the `-sc <float>` argument 
-+ Sleek design
-+ Information title page
-+ Contains hyperlinks
-+ Stores PDF metadata
-- Inconsistent page breaks, a general limitation with FPDF when trying to fit as many whole commits on a single page 
+👍 Fast<br>
+👍 Can be scaled with the `-sc <float>` argument<br> 
+👍 Sleek design<br>
+👍 Information title page<br>
+👍 Contains hyperlinks<br>
+👍 Stores PDF metadata<br>
+👎 Inconsistent page breaks, a general limitation with FPDF when trying to fit as many whole commits on a single page<br> 
 
 ### fpdf (gen2b - Default)
-+ Same as gen2a but with perfectly accurate page breaking
-- Slow when generating large amounts of commits (generally, it is a good idea to switch to gen2a when drawing over 5000 commits)
-
-<br><br>
-## Gallery
-**gen1 title page**<br>
-<img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/b243e102-0eda-4750-bbce-027f5738405b" alt="gen1 pdf title page" width=561.12>
-
-**gen2 title page in dark mode**<br>
-<img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/e1f2fe53-1c72-42a6-a89b-44a27c0b06a9" alt="gen2 pdf title page dark" width=561.12>
-
-**gen2 commit page in dark mode**<br>
-<img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/a9fd3341-e661-4355-91e7-0dc3182e7239" alt="gen2 pdf commit page dark" width=561.12>
+👍 Same as gen2a but with perfectly accurate page breaking<br>
+👎 Slow when generating large amounts of commits (generally, it is a good idea to switch to gen2a (with the `-gen2a` argument) when drawing over 5000 commits)<br>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `commits2pdf-1.1.8/README.md` & `commits2pdf-1.1.9/commits2pdf.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,52 @@
+Metadata-Version: 2.1
+Name: commits2pdf
+Version: 1.1.9
+Summary: View a filtered commit history in PDF form.
+Home-page: https://github.com/tomasvana10/commits2pdf
+Author: Tomas Vana
+License: MIT
+Platform: any
+Classifier: Topic :: Multimedia
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Education
+Classifier: Topic :: Office/Business
+Description-Content-Type: text/markdown
+License-File: LICENCE.md
+Requires-Dist: GitPython
+Requires-Dist: pycairo
+Requires-Dist: fpdf
+Requires-Dist: tqdm
+
 ![Licence](https://img.shields.io/badge/licence-MIT-green?style=flat?logo=licence)
 [![PyPI version](https://img.shields.io/pypi/v/commits2pdf?style=flat-square)](https://pypi.org/project/commits2pdf/)
 [![Publish to PyPI.org](https://github.com/tomasvana10/commits2pdf/actions/workflows/publish.yml/badge.svg)](https://github.com/tomasvana10/commits2pdf/actions/workflows/publish.yml)
 [![Release)](https://img.shields.io/github/v/release/tomasvana10/commits2pdf?logo=github)](https://github.com/tomasvana10/commits2pdf/releases/latest)
 [![Issues](https://img.shields.io/github/issues-raw/tomasvana10/commits2pdf.svg?maxAge=25000)](https://github.com/tomasvana10/commits2pdf/issues)
 [![CodeQL](https://github.com/tomasvana10/commits2pdf/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/tomasvana10/commits2pdf/actions/workflows/github-code-scanning/codeql)
 [![Tests](https://github.com/tomasvana10/commits2pdf/actions/workflows/tox-tests.yml/badge.svg)](https://github.com/tomasvana10/commits2pdf/actions/workflows/tox-tests.yml)
 
 # commits2pdf
 Visualise a GitHub repository's commit history in PDF form via the command-line
+---
+![ezgif-pdf-tutorial](https://github.com/tomasvana10/commits2pdf/assets/124552709/fcc4b5da-2326-4405-80fe-cf984f61129c)
 <br><br>
 ## Dependencies
 `pycairo`<br>
 `GitPython`<br>
-`fpdf`
+`fpdf`<br>
+`progressbar`
 <br><br>
 ## Installation
 **Requires [pip](https://pip.pypa.io/en/stable/installation/)**
 
 Make a virtual environment (recommended)
 ```
 pip install virtualenv OR pip3 install virtualenv
@@ -25,140 +55,104 @@
 ON WINDOWS: venv\scripts\activate
 ```
 
 Install the package in your system directory/virtual environment:
 ```
 pip install -U commits2pdf OR pip3 install -U commits2pdf
 ```
-OR, install the package in your home directory (good if you aren't using a virtual environment):
+OR, install the package in your home directory if you aren't using a virtual environment:
 ```
 pip install --user -U commits2pdf
 ```
 
 
 **If you encounter errors with building `pycairo`, click [here](https://stackoverflow.com/a/76175684/23245953)**
 <br><br>
+
 ## Command-line parameters
 ```
 positional arguments:
   owner                 The owner of the git repository. Required.
 
 options:
   -h, --help            show this help message and exit
   -o OUTPUT, --output OUTPUT
-                        Directory path to your PDF output. Set to "." by default. Will be created if it does not exist. Example: -o ./work/my_pdfs
+                        Directory path to your PDF output. Set to "." (your current directory) by default. Will be created if it does not exist. Example:
+                        ./work/my_pdfs
   -b BRANCH, --branch BRANCH
                         The repository branch. Set to "main" by default.
   -a AUTHORS, --authors AUTHORS
-                        Filter commits from a comma-separated list of authors. Format: <author@email.com> OR <author1@email.com,author2@email.com> etc. Set to all authors by
-                        default.
+                        Filter commits from a comma-separated list of authors. Format: <author@email.com> OR <author1@email.com,author2@email.com> etc. Set to all      
+                        authors by default.
   -s START_DATE, --start_date START_DATE
-                        Filter from start date of commits. Format: YYYY-mm-dd or YYYY-m-d. Example: 2023-12-05
+                        Filter from start date of commits. Format: d/m/YYYY. Example: 5/12/2023
   -e END_DATE, --end_date END_DATE
-                        Filter to end date of commits. Format: YYYY-mm-dd or YYYY-m-d. Example: 2023-12-05
+                        Filter to end date of commits. Format: d/m/YYYY. Example: 5/12/2023
   -r, --reverse         Output the commits from newest to oldest. Set to oldest to newest by default
-  -d, --dark            Toggle dark mode for the output PDF. Set to "light" by default.
+  -dark                 Toggle dark mode for the output PDF. Set to "light" by default.
   -po, --prevent-open   Prevent commits2pdf from automatically opening the directory the PDF was created in.
   -sc SCALING, --scaling SCALING
                         Set the scaling of the output PDF. Only available with gen2a and gen2b.
+  -in INCLUDE, --include INCLUDE
+                        Include commits with the given string sequences in their title or description. Format: "<string1>" OR "<string1,string2>". Whitespace
+                        sensitive and case insensitive. NOTE: This query is performed BEFORE excluding commits.
+  -ex EXCLUDE, --exclude EXCLUDE
+                        Exclude commits with the given string sequences in their title or description. Format: "<string1>" OR "<string1,string2>". Whitespace
+                        sensitive and case insensitive.
   -gen1, --pdf_gen_1    PDF rendering implementation with ``pycairo``.
   -gen2a, --pdf_gen_2a  The first PDF rendering implementation with ``fpdf``.
   -gen2b, --pdf_gen_2b  The second PDF rendering implementation with ``pycairo``. The default option.
-  -qa QUERIES_ANY, --query-any QUERIES_ANY
-                        Select the commits whose title OR description match ANY part of your query. Format: "<query1>" OR "<query1,query2>" etc. Note: queries can have leading or    
-                        trailing whitespace.
-  -QA QUERIES_ALL, --query-all QUERIES_ALL
-                        Select the commits whose title OR description match ALL parts of your query. Format: "<query1>" OR "<query1,query2>" etc. Note: queries can have leading or   
-                        trailing whitespace.
   -rp RPATH, --repo-path RPATH
-                        Path to your repository directory. Set to "." by default.
+                        Path to your repository directory. Set to "." (your current directory) by default.
   -fc RNAME, --repo-from-clone RNAME
                         Clone a repo into the working directory and generate the commits PDF from it automatically. Format: <repo name> (case insensitive).
   -nnc NEWEST_N_COMMITS, --newest-n-commits NEWEST_N_COMMITS
                         Select the newest n number amount of commits to include after filtering.
   -onc OLDEST_N_COMMITS, --oldest-n-commits OLDEST_N_COMMITS
                         Select the oldest n number amount of commits to include after filtering.
 ```
-<br>
 
 ## Usage
-<br>**Simple usage - what you will be using the most**:
+**Usage example #1**
 ```
 c2p tomasvana10
 ```
-_Explanation_: Run the CLI tool in the current directory (assuming it is a Git repository). The owner name must be provided in all cases.
-
-<br>**Advanced usage example #1**:
-```
-c2p tomasvana10 -rp ../seriescalculator_sdd -a person@email.com,other_person@gmail.com -s 2024-11-30 -e 2024-12-30 -b other_branch -d
-```
-_Explanation_: 
-1. Override the default repository path (``-rp ..\seriescalculator_sdd``) with a folder in the parent directory.
-2. Look for specific commit emails (separated by commas)
-3. Search for commits from the -s date until the -e date
-4. Search for commits only made to `other_branch`
-5. Toggle dark mode for the PDF output
+> Output a PDF to your current directory (assuming it is a git repository that is owned by `tomasvana10`).
 
-<br>**Advanced usage example #2**
+<br>**Usage example #2**
 ```
-c2p tomasvana10 -nnc 10 -r
+c2p tomasvana10 -o .. -rp ./my_repo
 ```
-_Explanation_: Display the newest ten commits (after any filtering) in reverse order (newest to oldest instead of the default, which is oldest to newest).
+> Output a PDF to the parent directory, selecting `./my_repo` as your git repository to access the commits from.
 
-<br>**Advanced usage example #3**
+<br>**Usage example #3**
 ```
-c2p tomasvana10 -qa "javascript,test " -onc 5 -po -o ..
+c2p tomasvana10 -nnc 10 -in "javascript,build" -ex "testing"
 ```
-_Explanation_: 
-1. Display the 5 oldest commits after querying the current repository's commits for either "javascript" OR "test "
-2. Prevent the PDF directory from being automatically opened.
-3. Output the PDF to the parent directory (`..`)
+> Output a PDF to the current directory, displaying the newest 10 commits after filtering commits that contain "javascript" or "build in their title or description and do not contain "testing"
 
-**NOTE**: -qa selects commits that include **any** query criteria in the title **OR** description, while -QA selects commits that include **ALL** query criteria in the title or description.
-
-<br>**Advanced usage example #4**
+<br>**Usage example #4**
 ```
-c2p tomasvana10 -QA "dev ,testing" -gen2a -sc 0.8
+c2p devguarv -fc Yr-12-HSC-SDD-Task-2 -e 28/4/2024
 ```
-_Explanation_:
-1. Query the repo for both "dev " AND "testing"
-2. Use the `gen2a` PDF renderer to visualise the PDF
-3. Set the scaling of the PDF output to 0.8
-
-**NOTE**: Scaling (`-sc`) is only available when using `gen2a` or `gen2b`. `gen2b` is default.
+> Clone the repo `Yr-12-HSC-SDD-Task-2` into the current directory and output a PDF into the same place after filtering commits that were made up to `28/4/2024`
+<br>
 
-<br>**Clone the repo you want to document on-demand**:
-```
-c2p tomasvana10 -fc some_repo_name
-```
-_Explanation_: Create the repo you have specified and make the PDF. This repo is always cloned into the current working directory.
-<br><br>
 ## PDF Generation implementations
 ### pycairo (gen1)
-+ Fast
-- Looks like crap 
-- No hyperlinks, therefore the entire link to a commit's diff is displayed
-- Occasional bugs in rendering
+👍 Fast<br>
+👎 Cannot write multipage commits<br>
+👎 Looks like crap<br>
+👎 No hyperlinks, therefore the entire link to a commit's diff is displayed
 
 ### fpdf (gen2a)
-+ Fast
-+ Can be scaled with the `-sc <float>` argument 
-+ Sleek design
-+ Information title page
-+ Contains hyperlinks
-+ Stores PDF metadata
-- Inconsistent page breaks, a general limitation with FPDF when trying to fit as many whole commits on a single page 
+👍 Fast<br>
+👍 Can be scaled with the `-sc <float>` argument<br> 
+👍 Sleek design<br>
+👍 Information title page<br>
+👍 Contains hyperlinks<br>
+👍 Stores PDF metadata<br>
+👎 Inconsistent page breaks, a general limitation with FPDF when trying to fit as many whole commits on a single page<br> 
 
 ### fpdf (gen2b - Default)
-+ Same as gen2a but with perfectly accurate page breaking
-- Slow when generating large amounts of commits (generally, it is a good idea to switch to gen2a when drawing over 5000 commits)
-
-<br><br>
-## Gallery
-**gen1 title page**<br>
-<img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/b243e102-0eda-4750-bbce-027f5738405b" alt="gen1 pdf title page" width=561.12>
-
-**gen2 title page in dark mode**<br>
-<img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/e1f2fe53-1c72-42a6-a89b-44a27c0b06a9" alt="gen2 pdf title page dark" width=561.12>
-
-**gen2 commit page in dark mode**<br>
-<img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/a9fd3341-e661-4355-91e7-0dc3182e7239" alt="gen2 pdf commit page dark" width=561.12>
+👍 Same as gen2a but with perfectly accurate page breaking<br>
+👎 Slow when generating large amounts of commits (generally, it is a good idea to switch to gen2a (with the `-gen2a` argument) when drawing over 5000 commits)<br>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `commits2pdf-1.1.8/commits2pdf/args.py` & `commits2pdf-1.1.9/commits2pdf/args.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,77 +13,107 @@
     help="The owner of the git repository. Required.",
 )
 parser.add_argument(
     "-o",
     "--output",
     dest="output",
     default=".",
-    help='Directory path to your PDF output. Set to "." (your current directory)'
-    " by default. Will be created if it does not exist. Example: -o ./work/my_pdfs",
+    help=(
+        'Directory path to your PDF output. Set to "." (your current'
+        " directory) by default. Will be created if it does not exist."
+        " Example: ./work/my_pdfs"
+    ),
 )
 parser.add_argument(
     "-b",
     "--branch",
     dest="branch",
     default="main",
     type=str,
     help='The repository branch. Set to "main" by default.',
 )
 parser.add_argument(
     "-a",
     "--authors",
     dest="authors",
-    help="Filter commits from a comma-separated list of authors. Format: "
-    "<author@email.com> OR <author1@email.com,author2@email.com> etc. "
-    "Set to all authors by default.",
+    help=(
+        "Filter commits from a comma-separated list of authors. Format: "
+        "<author@email.com> OR <author1@email.com,author2@email.com> etc. "
+        "Set to all authors by default."
+    ),
 )
 parser.add_argument(
     "-s",
     "--start_date",
     dest="start_date",
-    help="Filter from start date of commits. Format: YYYY-mm-dd or YYYY-m-d. "
-    "Example: 2023-12-05",
+    help="Filter from start date of commits. Format: d/m/YYYY. Example: 5/12/2023",
 )
 parser.add_argument(
     "-e",
     "--end_date",
     dest="end_date",
-    help="Filter to end date of commits. Format: YYYY-mm-dd or YYYY-m-d.  "
-    "Example: 2023-12-05",
+    help="Filter to end date of commits. Format: d/m/YYYY. Example: 5/12/2023",
 )
 parser.add_argument(
     "-r",
     "--reverse",
     dest="reverse",
     action="store_true",
-    help="Output the commits from newest to oldest. Set to oldest to newest "
-    "by default",
+    help=(
+        "Output the commits from newest to oldest. Set to oldest to newest "
+        "by default"
+    ),
 )
 parser.add_argument(
-    "-d",
-    "--dark",
+    "-dark",
     dest="dark",
     action="store_true",
     help='Toggle dark mode for the output PDF. Set to "light" by default.',
 )
 parser.add_argument(
     "-po",
     "--prevent-open",
     dest="prevent_open",
     action="store_true",
-    help="Prevent commits2pdf from automatically opening the directory the "
-    "PDF was created in.",
+    help=(
+        "Prevent commits2pdf from automatically opening the directory the "
+        "PDF was created in."
+    ),
 )
 parser.add_argument(
     "-sc",
     "--scaling",
     dest="scaling",
     type=float,
     default=1.0,
-    help="Set the scaling of the output PDF. Only available with gen2a and gen2b.",
+    help=(
+        "Set the scaling of the output PDF. Only available with gen2a and"
+        " gen2b."
+    ),
+)
+parser.add_argument(
+    "-in",
+    "--include",
+    dest="include",
+    help=(
+        "Include commits with the given string sequences in their title or"
+        ' description. Format: "<string1>" OR "<string1,string2>". Whitespace'
+        " sensitive and case insensitive. NOTE: This query is performed"
+        " BEFORE excluding commits."
+    ),
+)
+parser.add_argument(
+    "-ex",
+    "--exclude",
+    dest="exclude",
+    help=(
+        "Exclude commits with the given string sequences in their title or"
+        ' description. Format: "<string1>" OR "<string1,string2>". Whitespace'
+        " sensitive and case insensitive."
+    ),
 )
 
 # Group for the selection of a PDF generation implementation
 gen_group = parser.add_mutually_exclusive_group()
 gen_group.add_argument(
     "-gen1",
     "--pdf_gen_1",
@@ -99,69 +129,60 @@
     help="The first PDF rendering implementation with ``fpdf``.",
 )
 gen_group.add_argument(
     "-gen2b",
     "--pdf_gen_2b",
     action="store_true",
     dest="gen2b",
-    help="The second PDF rendering implementation with ``pycairo``. The "
-    "default option.",
-)
-
-# Group for either an AND or OR query
-query_group = parser.add_mutually_exclusive_group()
-query_group.add_argument(
-    "-qa",
-    "--query-any",
-    dest="queries_any",
-    help="Select the commits whose title OR description match ANY part of "
-    'your query. Format: "<query1>" OR "<query1,query2>" etc. Note: '
-    "queries can have leading or trailing whitespace.",
-)
-query_group.add_argument(
-    "-QA",
-    "--query-all",
-    dest="queries_all",
-    help="Select the commits whose title OR description match ALL parts of "
-    'your query. Format: "<query1>" OR "<query1,query2>" etc. Note: '
-    "queries can have leading or trailing whitespace.",
+    help=(
+        "The second PDF rendering implementation with ``pycairo``. The "
+        "default option."
+    ),
 )
 
 # Group for specifying either a path to a git repo or the name of the repo
 # to clone from
 repo_group = parser.add_mutually_exclusive_group()
 repo_group.add_argument(
     "-rp",
     "--repo-path",
     dest="rpath",
     default=".",
     type=str,
-    help='Path to your repository directory. Set to "." (your current directory)'
-    " by default.",
+    help=(
+        'Path to your repository directory. Set to "." (your current'
+        " directory) by default."
+    ),
 )
 repo_group.add_argument(
     "-fc",
     "--repo-from-clone",
     dest="rname",
     type=str,
-    help="Clone a repo into the working directory and generate the commits "
-    "PDF from it automatically. Format: <repo name> (case insensitive).",
+    help=(
+        "Clone a repo into the working directory and generate the commits "
+        "PDF from it automatically. Format: <repo name> (case insensitive)."
+    ),
 )
 
 # Group for selecting either the newest or oldest n number of commits
 n_commits_group = parser.add_mutually_exclusive_group()
 n_commits_group.add_argument(
     "-nnc",
     "--newest-n-commits",
     dest="newest_n_commits",
     type=int,
-    help="Select the newest n number amount of commits to include after "
-    "filtering.",
+    help=(
+        "Select the newest n number amount of commits to include after "
+        "filtering."
+    ),
 )
 n_commits_group.add_argument(
     "-onc",
     "--oldest-n-commits",
     dest="oldest_n_commits",
     type=int,
-    help="Select the oldest n number amount of commits to include after "
-    "filtering.",
+    help=(
+        "Select the oldest n number amount of commits to include after "
+        "filtering."
+    ),
 )
```

### Comparing `commits2pdf-1.1.8/commits2pdf/cli.py` & `commits2pdf-1.1.9/commits2pdf/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 handle arguments. Imports a PDF generation implementation from this package
 (either ``pycairo`` or ``fpdf``) based on the users input.
 """
 
 from argparse import Namespace
 from datetime import datetime
 from os import path
-from re import match
+from re import match, search
 
 from .args import parser
 from .commits import Commits
 from .constants import (
     CAIRO_DARK,
     CAIRO_LIGHT,
     CANNOT_USE_SCALE_WARNING,
     DATE,
     EMAILS,
     FPDF_DARK,
     FPDF_LIGHT,
     INVALID_ARG_WARNING,
     INVALID_BASENAME_WARNING,
-    QUERY,
+    INVALID_QUERIES,
 )
 from .logger import logger
 
 
 def main() -> None:
     """Parses arguments, provides warnings, and collects the commits based on
     the arguments using the ``Commits`` class.
@@ -33,20 +33,20 @@
     (
         appearance,
         rpath,
         url,
         authors,
         start_date,
         end_date,
-        queries_any,
-        queries_all,
+        include,
+        exclude,
         gen,
         mode,
         scaling,
-    ) = _handle_arguments(args)
+    ) = _validate_args(args)
 
     if args.rpath and not args.rname:
         logger.warn(INVALID_BASENAME_WARNING)
 
     commits = Commits(
         rpath=rpath,
         owner=args.owner,
@@ -54,16 +54,16 @@
         branch=args.branch,
         authors=args.authors,
         start_date=start_date,
         end_date=end_date,
         reverse=args.reverse,
         newest_n_commits=args.newest_n_commits,
         oldest_n_commits=args.oldest_n_commits,
-        queries_any=queries_any,
-        queries_all=queries_all,
+        include=include,
+        exclude=exclude,
     )
 
     if not commits.err_flag:
         _make_pdf(commits, appearance, args, gen, mode, scaling)
     else:
         return  # Any errors would have been logged by ``commits.py``, so exit
 
@@ -126,56 +126,55 @@
 
             if plat == "Darwin":
                 os_system("open %s" % p)
             elif plat == "Linux":
                 os_system("xdg-open %s" % p)
 
 
-def _handle_arguments(args: Namespace) -> tuple[None | str | list[str]]:
+def _validate_args(args: Namespace) -> tuple[None | str | list[str]]:
     """Process arguments through some conditions and regex matching to ensure
     they are valid. Raise errors if they are not valid.
     """
-    url = authors = start_date = end_date = queries_any = queries_all = (
-        scaling
-    ) = None
+    url = authors = start_date = end_date = include = exclude = scaling = None
 
     if args.rname:
-        rpath: str = args.rname  # Set the repository path to the name of the
-        # repository that will be cloned
+        rpath: str = args.rname  # Set the repo path to the name of the repo 
+                                 # that will be cloned
         url: str = f"https://github.com/{args.owner}/{args.rname}"
     else:
         rpath: str = args.rpath
 
     if args.authors:
         if not match(EMAILS, args.authors):
             logger.error(INVALID_ARG_WARNING.format("email"))
             exit(1)
         authors: list[str] = args.authors.split(",")
 
     if args.start_date:
         if not match(DATE, args.start_date):
             logger.error(INVALID_ARG_WARNING.format("date"))
             exit(1)
-        start_date: datetime = datetime.strptime(args.start_date, "%Y-%m-%d")
+        start_date: datetime = datetime.strptime(args.start_date, "%d/%m/%Y")
     if args.end_date:
         if not match(DATE, args.end_date):
             logger.error(INVALID_ARG_WARNING.format("date"))
             exit(1)
-        end_date: datetime = datetime.strptime(args.end_date, "%Y-%m-%d")
+        end_date: datetime = datetime.strptime(args.end_date, "%d/%m/%Y")
 
-    if args.queries_any:
-        if not match(QUERY, args.queries_any):
+    if args.include:
+        if search(INVALID_QUERIES, args.include):
             logger.error(INVALID_ARG_WARNING.format("query"))
             exit(1)
-        queries_any: list[str] = args.queries_any.split(",")
-    elif args.queries_all:
-        if not match(QUERY, args.queries_all):
+        include: list[str] = args.include.split(",")
+        
+    if args.exclude:
+        if search(INVALID_QUERIES, args.exclude):
             logger.error(INVALID_ARG_WARNING.format("query"))
             exit(1)
-        queries_all: list[str] = args.queries_all.split(",")
+        exclude: list[str] = args.exclude.split(",")
 
     if args.gen1:
         gen, mode = "gen1", None
         appearance: dict[str, tuple[int]] = (
             CAIRO_LIGHT if not args.dark else CAIRO_DARK
         )
         if args.scaling:
@@ -192,13 +191,13 @@
     return (
         appearance,
         rpath,
         url,
         authors,
         start_date,
         end_date,
-        queries_any,
-        queries_all,
+        include,
+        exclude,
         gen,
         mode,
         scaling,
     )
```

### Comparing `commits2pdf-1.1.8/commits2pdf/commits.py` & `commits2pdf-1.1.9/commits2pdf/commits.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,37 @@
+from __future__ import annotations
+
 from datetime import datetime
 from os import path
 from shutil import rmtree
 from typing import Optional
 
 from git import (
     GitCommandError,
+    Head,
     InvalidGitRepositoryError,
     NoSuchPathError,
     Repo,
 )
+from git import Commit as GitCommit
 
 from .constants import (
     CLONING_REPO_INFO,
     CODING,
     DETACHED_BRANCH_ERROR,
     FILTER_INFO,
     GATHERED_COMMITS_INFO,
     INVALID_GIT_REPO_ERROR,
     N_COMMITS_INFO,
     N_COMMITS_WARNING,
     NONEXISTING_BRANCH_WARNING,
     NONEXISTING_OR_INVALID_REPO_ERROR,
     NONEXISTING_REPO_ERROR,
     REPO_ALREADY_EXISTS_WARNING,
-    UNEXPECTED_BUG_ERROR,
+    MUST_RECLONE_ERROR,
 )
 from .logger import logger
 
 
 class Commits(object):
     """Represents a filtered set of commits along with filter information."""
 
@@ -41,190 +45,146 @@
         self.branch: Optional[str] = kwargs["branch"]
         self.authors: Optional[list[str]] = kwargs["authors"]
         self.start_date: Optional[datetime] = kwargs["start_date"]
         self.end_date: Optional[datetime] = kwargs["end_date"]
         self.reverse: Optional[bool] = kwargs["reverse"]
         self.newest_n_commits: Optional[int] = kwargs["newest_n_commits"]
         self.oldest_n_commits: Optional[int] = kwargs["oldest_n_commits"]
-        self.queries_any: Optional[list[str]] = kwargs["queries_any"]
-        self.queries_all: Optional[list[str]] = kwargs["queries_all"]
+        self.include: Optional[list[str]] = kwargs["include"]
+        self.exclude: Optional[list[str]] = kwargs["exclude"]
 
         self.r: Repo = self._get_repo()
         if isinstance(self.r, Repo):  # Repo was successfully found, continue
             self._init_repo_data()
         elif self.r == "DELTREE":  # Perform buffered deletion due to errors in
-            # ``_get_repo``.
+                                   # ``_get_repo``.
             rmtree(self.rpath, ignore_errors=True)
             self.err_flag = True
-        elif not self.r:  # ``_get_repo`` returned NoneType, so the repo could 
+        elif not self.r:  # ``_get_repo`` returned NoneType, so the repo could
                           # not be accessed
             self.err_flag = True
 
     def _init_repo_data(self) -> None:
         """Find the repo name (preferrably from the remote), then
         sequentially build the filtered commits from the commits of the
         repo.
         """
         if len(self.r.remotes) > 0:  # Use remote name
-            self.rname = self.r.remotes.origin.url.split(".git")[0].split("/")[
-                -1
-            ]
+            self.rname: str = self.r.remotes.origin.url.split(".git")[0].split(
+                "/"
+            )[-1]
         else:  # No remote exists, just get the name of the directory
-            self.rname = path.basename(self.r.working_tree_dir.split("/")[-1])
+            self.rname: str = path.basename(
+                self.r.working_tree_dir.split("/")[-1]
+            )
 
         self.raw_commits: list[Repo.commit] = self._gather_commits()
         self.commit_objects: list[Commit] = self._instantiate_commits()
         self.filtered_commits: list[Commit] = self._filter_commits()
 
+    def _retry_clone(self, e) -> Repo | str | None:
+        """Reattempt cloning if possible and update ``self.branch`` accordingly."""
+        rmtree(self.rpath, ignore_errors=True)
+        if "remote branch" in str(e).casefold(): # User entered invalid branch, 
+                                                 # so clone repo without
+                                                 # specifying a branch argument
+            r: Repo = Repo.clone_from(self.url, self.rpath, no_checkout=True)
+            try:
+                b: Head = r.active_branch
+            except TypeError:  # Repo branch is detached
+                return logger.error(DETACHED_BRANCH_ERROR.format(self.branch))
+
+            logger.warning(NONEXISTING_BRANCH_WARNING.format(self.branch, b))
+            self.branch = b
+            return r
+
+        else:  # Some other error occurred
+            logger.error(NONEXISTING_OR_INVALID_REPO_ERROR.format(self.url))
+            return "DELTREE"
+
+    def _validate_branch(self, r: Repo) -> bool | None:
+        """Ensure that ``self.branch`` exists. If not, attempt to set it to the
+        repo's active branch.
+        """
+        if self.branch == r.active_branch:
+            return True
+
+        try:  # The branch they want does not exist, so access the active branch
+            b: Head = r.active_branch
+            print("got new active branch", b)
+        except TypeError:
+            return logger.error(DETACHED_BRANCH_ERROR.format(self.branch))
+
+        logger.warning(NONEXISTING_BRANCH_WARNING.format(self.branch, b))
+        self.branch: Head = b  # Update the branch to the repo's active branch
+        return True
+
+    def _clone_repo(self) -> Repo | str | None:
+        """Attempt to clone a repo's .git directory."""
+        logger.info(CLONING_REPO_INFO)
+        try:
+            r: Repo = Repo.clone_from(
+                self.url,
+                self.rpath,
+                branch=self.branch,
+                no_checkout=True,
+            )
+            return r
+        except GitCommandError as e:
+            return self._retry_clone(e)
+
     def _get_repo(self) -> Repo | str | None:
         """Access a repo, or clone it and then access it, and update
         ``self.branch`` if necessary. Complete with extensive error handling,
         ensuring a high chance of the user's requests being processed.
         """
         if self.url:  # User wants to clone a repo
             if path.exists(self.rpath) and path.isdir(self.rpath):  # Repo may
                                                                     # exist
                 if path.exists(path.join(self.rpath, ".git")):  # .git exists
                     logger.warn(REPO_ALREADY_EXISTS_WARNING)
                     try:
-                        r = Repo(self.rpath)  # Attempt to access repo
+                        r: Repo = Repo(self.rpath)  # Attempt to access repo
                     except NoSuchPathError:
                         return logger.error(NONEXISTING_REPO_ERROR)
 
-                    if self.branch:  # User is looking for specific branch
-                        try:
-                            b = r.active_branch
-                        except TypeError:  # Branch is detached
-                            return logger.error(
-                                DETACHED_BRANCH_ERROR.format(self.branch)
-                            )
-
-                        if not str(b) == str(
-                            self.branch
-                        ):  # Branch of existing repo is not the branch the user wants
-                            logger.warning(
-                                NONEXISTING_BRANCH_WARNING.format(
-                                    self.branch, b
-                                )
-                            )
-                            self.branch = b  # Update the branch to the repo's
-                                             # active branch
-
-                    return r  # Repo was accessed with no problems
+                    return r if self._validate_branch(r) else None
 
                 else:  # .git does not exist, delete the existing folder and
                        # clone the repo
                     rmtree(self.rpath, ignore_errors=True)
-                    try:
-                        logger.info(CLONING_REPO_INFO)
-                        r = Repo.clone_from(
-                            self.url,
-                            self.rpath,
-                            branch=self.branch,
-                            no_checkout=True,
-                        )
-                    except GitCommandError as e:
-                        if (
-                            "remote branch" in str(e).casefold()
-                        ):  # User entered invalid branch
-                            logger.info(CLONING_REPO_INFO)
-                            r = Repo.clone_from(
-                                self.url, self.rpath, no_checkout=True
-                            )
-                            try:
-                                b = r.active_branch
-                            except TypeError:
-                                return logger.error(
-                                    DETACHED_BRANCH_ERROR.format(self.branch)
-                                )
-                            logger.warning(
-                                NONEXISTING_BRANCH_WARNING.format(
-                                    self.branch, b
-                                )
-                            )
-                            self.branch = b  # Update the branch to the repo's
-                                             # active branch
-                        else:  # Some other error occurred
-                            logger.error(
-                                NONEXISTING_OR_INVALID_REPO_ERROR.format(
-                                    self.url
-                                )
-                            )
-                            return "DELTREE"
+                    return self._clone_repo()
 
             else:  # Repo does not exist, just clone it
-                try:
-                    logger.info(CLONING_REPO_INFO)
-                    r = Repo.clone_from(
-                        self.url,
-                        self.rpath,
-                        branch=self.branch,
-                        no_checkout=True,
-                    )
-                except GitCommandError as e:
-                    if "remote branch" in str(e).casefold():
-                        logger.info(CLONING_REPO_INFO)
-                        r = Repo.clone_from(
-                            self.url, self.rpath, no_checkout=True
-                        )
-                        try:
-                            b = r.active_branch
-                        except TypeError:
-                            return logger.error(
-                                DETACHED_BRANCH_ERROR.format(self.branch)
-                            )
-                        logger.warning(
-                            NONEXISTING_BRANCH_WARNING.format(self.branch, b)
-                        )
-                        self.branch = b
-                    else:  # Some other error occurred
-                        logger.error(
-                            NONEXISTING_OR_INVALID_REPO_ERROR.format(self.url)
-                        )
-                        return "DELTREE"
+                return self._clone_repo()
 
         else:  # Just access the repo normally
             try:
-                r = Repo(self.rpath)
-                if self.branch:
-                    try:
-                        b = r.active_branch
-                    except TypeError:
-                        return logger.error(
-                            DETACHED_BRANCH_ERROR.format(self.branch)
-                        )
-                    if not str(b) == str(self.branch):  # Branch of repo is not
-                                                        # the branch the user wants
-                        logger.warning(
-                            NONEXISTING_BRANCH_WARNING.format(self.branch, b)
-                        )
-                        self.branch = b  # Update the branch to the repo's
-                                         # active branch
+                r: Repo = Repo(self.rpath)
+                return r if self._validate_branch(r) else None
 
             except InvalidGitRepositoryError:
                 return logger.error(INVALID_GIT_REPO_ERROR.format(self.rpath))
             except NoSuchPathError:
                 return logger.error(NONEXISTING_REPO_ERROR)
 
-        return r
-
-    def _gather_commits(self) -> list[Repo.commit]:
+    def _gather_commits(self) -> list[GitCommit]:
         """Find all the commits that match the user's since, until and branch
         specifications.
         """
         try:
-            commits = list(
-                self.r.iter_commits(  # If any of the params are NoneType, no prob!
+            commits: list[GitCommit] = list(
+                self.r.iter_commits(
                     since=self.start_date,
                     until=self.end_date,
                     rev=self.branch,
                 )
             )
         except Exception:
-            logger.error(UNEXPECTED_BUG_ERROR)
+            logger.error(MUST_RECLONE_ERROR)
             self.err_flag = True
             exit(1)
 
         logger.info(GATHERED_COMMITS_INFO.format(len(commits)))
 
         return commits
 
@@ -236,41 +196,51 @@
         for commit in self.raw_commits:
             commit_objects.append(
                 Commit(self.owner, self.rname, self.branch, commit)
             )
 
         return commit_objects
 
-    def _filter_commits(self) -> list[dict[str, str]]:
+    def _filter_commits(self) -> list[Commit]:
         """Process the Commit objects based on user-specified criteria such as
         authors and queries.
         """
-        filtered_commits = self.commit_objects
-        if self.queries_any or self.queries_all:
-            queries, query_func = (
-                (self.queries_any, any)
-                if self.queries_any
-                else (self.queries_all, all)
-            )
-            filtered_commits = [
+        filtered_commits: list[Commit] = self.commit_objects
+        if self.include:
+            filtered_commits: list[Commit] = [
                 commit
                 for commit in self.commit_objects
-                if query_func(
-                    q in commit["description"] or q in commit["title"]
-                    for q in queries
+                for q in self.include
+                if q.casefold() in commit["description"].casefold()
+                or q.casefold() in commit["title"].casefold()
+            ]
+            logger.info(
+                FILTER_INFO.format(
+                    len(filtered_commits),
+                    len(self.commit_objects),
+                    "include queries",
                 )
+            )
+        if self.exclude:
+            prior_len: int = len(filtered_commits)
+            filtered_commits: list[Commit] = [
+                commit
+                for commit in filtered_commits
+                for q in self.exclude
+                if q.casefold() not in commit["description"].casefold()
+                and q.casefold() not in commit["title"].casefold()
             ]
             logger.info(
                 FILTER_INFO.format(
-                    len(filtered_commits), len(self.commit_objects), "query"
+                    len(filtered_commits), prior_len, "exclude queries"
                 )
             )
         if self.authors:
-            prior_len = len(filtered_commits)
-            filtered_commits = [
+            prior_len: int = len(filtered_commits)
+            filtered_commits: list[Commit] = [
                 commit
                 for commit in filtered_commits
                 if commit["author_email"] in self.authors
             ]
             logger.info(
                 FILTER_INFO.format(
                     len(filtered_commits), prior_len, "author_email"
@@ -300,15 +270,15 @@
             else:
                 logger.warn(
                     N_COMMITS_WARNING.format(
                         "Oldest", self.oldest_n_commits, len(filtered_commits)
                     )
                 )
 
-        step = -1 if not self.reverse else 1
+        step: int = -1 if not self.reverse else 1
         filtered_commits = filtered_commits[::step]
 
         return filtered_commits
 
 
 class Commit(dict):
     """A simple way of representing a commit as a dictionary."""
@@ -325,17 +295,17 @@
         self["hexsha_short"] = commit.hexsha[:7]
         self["hexsha_long"] = commit.hexsha
         self["diff_url"] = (
             f"https://github.com/{owner}/{rname}/commit/{commit.hexsha}"
         )
 
         self["info"] = (
-            f"{self['hexsha_short']} | Branch: {self['branch']} | "
+            f"{self['hexsha_short']} | "
             f"By {self['author_name']} ({self['author_email']}) | "
-            f"At {self['date'].strftime('%Y-%m-%d')}"
+            f"At {self['date'].strftime('%d/%m/%Y')}"
         )
         self["info"] = Commit._code(self["info"])
 
         # Extract the message from the title
         msg = commit.message.split("\n")
         self["title"] = Commit._code(msg[0])
         self["description"] = (
```

### Comparing `commits2pdf-1.1.8/commits2pdf/constants.py` & `commits2pdf-1.1.9/commits2pdf/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import re
 
 """Regex for arg parser"""
-DATE = re.compile(
-    r"^\d{4}\-(0?[1-9]|1[012])\-(0?[1-9]|[12][0-9]|3[01])$"
-)  # YYYY/m/d or YYYY/mm/dd
+DATE = re.compile((
+    r"^(?:(?:31(\/|-|\.)(?:0?[13578]|1[02]))\1|(?:(?:29|30)(\/|-|\.)(?:0?[13-9]"
+    r"|1[0-2])\2))(?:(?:1[6-9]|[2-9]\d)?\d{2})$|^(?:29(\/|-|\.)0?2\3(?:(?:(?:1"
+    r"[6-9]|[2-9]\d)?(?:0[48]|[2468][048]|[13579][26])|(?:(?:16|[2468][048]|[3"
+    r"579][26])00))))$|^(?:0?[1-9]|1\d|2[0-8])(\/|-|\.)(?:(?:0?[1-9])|(?:1[0-2]"
+    r"))\4(?:(?:1[6-9]|[2-9]\d)?\d{2})$"
+))  # d/m/yyyy or dd/mm/yyyy
 
 EMAILS = re.compile(
     r"^([\w+-.%]+@[\w.-]+\.[A-Za-z]{2,4})(,[\w+-.%]+@[\w.-]+\.[A-Za-z]{2,4})*$"
 )  # usr@email.com or usr@email.com,user2@email.com, etc
 
-QUERY = re.compile(
-    r"^\s*(?:[^,\s]+(?:\s*,\s*[^,\s]+)*)?\s*$"
-)  # value1,value2 etc or value1 (can have leading/trailing whitespace)
+INVALID_QUERIES = re.compile(r"^,|,$")
 
 """Other stuff for arg parsing process"""
 USAGE_INFO = (
     "Simply run ``c2p -O <owner_name>`` in the command-line to generate a PDF"
     " of your repo's commit history (assuming your current directory is a"
     " repository). Run commits2pdf -h for more information."
 )
@@ -55,16 +57,18 @@
 CLONING_REPO_INFO = (
     "Cloning the .git file of your specified repository. This may take a"
     " while..."
 )
 NONEXISTING_REPO_ERROR = (
     "The repository you specified does not exist. Exiting..."
 )
-UNEXPECTED_BUG_ERROR = (
-    "Please delete your specified repository's directory and try again."
+MUST_RECLONE_ERROR = (
+    "Please delete your repository from your file system and rerun your"
+    " console command to clone a different branch of your specified"
+    " repository."
 )
 
 
 """Handling the filtering of the repository's commits"""
 FILTER_INFO = "Filtered {} commit(s) from {} existing commit(s) based on {}."
 N_COMMITS_INFO = "Selecting n {} number of commits ({})."
 N_COMMITS_WARNING = (
@@ -73,15 +77,14 @@
 )
 GATHERED_COMMITS_INFO = (
     "Gathered {} commit(s) based on since, until and branch filters."
 )
 
 
 """General PDF messages"""
-GENERATING_PDF_INFO = "Generating your PDF..."
 WRITING_PDF_INFO = "Writing your PDF to {}"
 
 
 """For the pycairo PDF implementation"""
 WIDTH = 612
 HEIGHT = 792
 MARGIN = 50
@@ -91,41 +94,45 @@
 RECURSION_ERROR = (
     "An error occured when using the gen2b renderer. Please try adding the"
     " -gen2a flag to your console command and try again."
 )
 CODING = "latin-1"
 TITLE_FONT = ["Arial", "B", 36]
 SUBTITLE_FONT = ["Arial", "", 30]
-MARGIN_FONT = ["Arial", "I", 8]
+MARGIN_FONT = ["Arial", "I", 9.5]
 SMALL_TEXT_FONT = ["Arial", "", 12]
 MEDIUM_TEXT_FONT = ["Arial", "", 16]
 TITLE_PAGE_INFO_FONT = ["Courier", "", 15]
 MEDIUM_TEXT_FONT_BOLD = ["Arial", "B", 16]
 INFO_TEXT_FONT = ["Courier", "", 12]
 MARGIN_LR = 25.4
 MARGIN_TB = 25.4
 
 
 """Appearances"""
 CAIRO_LIGHT = {
     "background": (1, 1, 1),
     "text": (0, 0, 0),
     "diff_url": (0, 0, 1),
+    "TYPE": "LIGHT",
 }
 
 CAIRO_DARK = {
     "background": (0.2, 0.2, 0.2),
     "text": (0.9, 0.9, 0.9),
     "diff_url": (0.6, 0.6, 1),
+    "TYPE": "DARK",
 }
 
 FPDF_LIGHT = {
     "background": (255, 255, 255),
     "text": (0, 0, 0),
     "diff_url": (0, 0, 255),
+    "TYPE": "LIGHT",
 }
 
 FPDF_DARK = {
     "background": (51, 51, 51),
     "text": (229, 229, 229),
     "diff_url": (123, 127, 232),
+    "TYPE": "DARK",
 }
```

### Comparing `commits2pdf-1.1.8/commits2pdf/render_cairo.py` & `commits2pdf-1.1.9/commits2pdf/render_cairo.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,17 @@
     FONT_SLANT_ITALIC,
     FONT_SLANT_NORMAL,
     FONT_WEIGHT_BOLD,
     FONT_WEIGHT_NORMAL,
     Context,
     PDFSurface,
 )
-from progressbar import ETA, Bar, Percentage, ProgressBar
+from tqdm import tqdm
 
 from .constants import (
-    GENERATING_PDF_INFO,
     HEIGHT,
     MARGIN,
     WIDTH,
     WRITING_PDF_INFO,
 )
 from .logger import logger
 
@@ -37,20 +36,15 @@
         self._commits, self._output, self._filename, self._ap = (
             commits,
             output,
             filename,
             appearance,
         )
         self.timestamp = datetime.fromtimestamp(int(time())).strftime(
-            "%Y-%m-%d %H:%M:%S"
-        )
-        # Keep track of generation progress for the user
-        self._progress = ProgressBar(
-            maxval=len(self._commits.filtered_commits),
-            widgets=[Percentage(), Bar(), ETA()],
+            "%d/%m/%Y %H:%M:%S"
         )
 
         self._s = PDFSurface(path.join(output, filename), WIDTH, HEIGHT)
         self._c = Context(self._s)
         self.page: int = 1
         self.y: int = MARGIN
 
@@ -58,47 +52,44 @@
         self._draw_footer()
         self._draw_title("Commit Report", self.y)
         self.y += 30
         self._draw_rname(commits.rname, self.y)
         self.y += 40
 
         if len(self._commits.filtered_commits) > 0:
-            logger.info(GENERATING_PDF_INFO)
             self._draw_commits()
             logger.info(
                 WRITING_PDF_INFO.format(
                     self._output + " ..."
                     if self._output != "."
                     else "your current directory..."
                 )
             )
             self._s.finish()
 
     def _draw_commits(self) -> None:
         """Driver function to draw all the commits."""
-        counter: int = 0
-        self._progress.start()
-        for commit in self._commits.filtered_commits:
+        for commit in tqdm(
+            self._commits.filtered_commits,
+            ncols=85,
+            desc="Generating",
+        ):
             text = self._get_commit_text(commit)
             height = sum(len(t) for t in text) * 14 + 50
             if self.y + height + 25 > HEIGHT - MARGIN:
                 self._s.show_page()
                 self.page += 1
                 self.y = MARGIN
 
                 self._draw_bg()
                 self._draw_footer()
 
             self.draw_commit(commit, self.y, *text)
-            counter += 1
-            self._progress.update(counter)
             self.y += height + 50
 
-        self._progress.finish()
-
     def _set_font(self, t: str, font: str = "Arial") -> None:
         """Set the font face, consisting of the family, slant and weight."""
         if t == "n":
             self._c.select_font_face(
                 font, FONT_SLANT_NORMAL, FONT_WEIGHT_NORMAL
             )
         elif t == "b":
```

### Comparing `commits2pdf-1.1.8/commits2pdf/render_fpdf.py` & `commits2pdf-1.1.9/commits2pdf/render_fpdf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 from datetime import datetime
 from os import makedirs, path
 from pickle import dumps, loads
 from time import time
 
 from fpdf import FPDF
-from progressbar import ETA, Bar, Percentage, ProgressBar
+from tqdm import tqdm
 
 from .constants import (
-    GENERATING_PDF_INFO,
     INFO_TEXT_FONT,
     MARGIN_FONT,
     MARGIN_LR,
     MARGIN_TB,
     MEDIUM_TEXT_FONT,
     MEDIUM_TEXT_FONT_BOLD,
     RECURSION_ERROR,
     SMALL_TEXT_FONT,
     SUBTITLE_FONT,
     TITLE_FONT,
     TITLE_PAGE_INFO_FONT,
     WRITING_PDF_INFO,
+    FPDF_DARK
 )
 from .logger import logger
 
+def footer():
+    pass
 
+def _beginpage_addon(func):
+    def wrapper(self, *args, **kwargs):
+        result = func(self, *args, **kwargs)
+        self.set_fill_color(*FPDF_DARK["background"])
+        self.rect(h=self.h, w=self.w, x=0, y=0, style="DF")
+        return result
+    return wrapper
+    
+    
 class FPDF_PDF:
     """PDF generation class implementing 2 methods of generation (``gen2a`` and
     ``gen2b``.
     """
 
     def __init__(
         self,
@@ -39,32 +50,30 @@
         scaling: str,
     ) -> None:
         super().__init__()  # portrait; millimetres; a4
         FPDF_PDF._set_scaling(scaling)
 
         self.err_flag: bool = False
         self.timestamp = datetime.fromtimestamp(int(time())).strftime(
-            "%Y-%m-%d %H:%M:%S"
+            "%d/%m/%Y %H:%M:%S"
         )
         self._commits, self._output, self._filename, self._ap, self._mode = (
             commits,
             output,
             filename,
             appearance,
             mode,
         )
-        # Keep track of generation progress for the user
-        self._progress = ProgressBar(
-            maxval=len(self._commits.filtered_commits),
-            widgets=[Percentage(), Bar(), ETA()],
-        )
-
-        self._p = FPDF()  # Contains the PDF data
+        self.commit_count = len(self._commits.filtered_commits)
+            
+        if self._ap["TYPE"] == "DARK": # Inject decorators to detect new page
+            FPDF._beginpage = _beginpage_addon(FPDF._beginpage)
+        self._p = FPDF()
+            
         self._configure_fpdf()
-        logger.info(GENERATING_PDF_INFO)
         self._prepare_and_draw()
         logger.info(
             WRITING_PDF_INFO.format(
                 self._output + " ..."
                 if self._output != "."
                 else "your current directory..."
             )
@@ -94,25 +103,25 @@
         )
         self._p.set_margins(MARGIN_LR, MARGIN_TB)
 
     def _prepare_and_draw(self):
         self._p.add_page()
         self._draw_page_bg()
         self._draw_title_page()
-        self._p.set_auto_page_break(auto=True)
         if self._mode == "unstable":
             self.do_pre_vis: bool = True
             self._p.set_auto_page_break(auto=False)
         else:
             self.do_pre_vis: bool = False
+            self._p.set_auto_page_break(auto=True)
 
-        if len(self._commits.filtered_commits) > 0:
+        if self.commit_count > 0:
             self._draw_commits()
 
-    def _draw_footer(self) -> None:
+    def footer(self) -> None:
         self._p.set_y(-1 * (MARGIN_TB / 2))
         self._set_font(*MARGIN_FONT)
         self._p.set_text_color(*self._ap["text"])
         self._p.cell(1, 0, f"Page {self._p.page_no()}", 0, 0, "L")
         self._p.cell(
             0, 0, f"Generated by commits2pdf at {self.timestamp}", 0, 0, "C"
         )
@@ -130,56 +139,75 @@
     def _set_font(
         self, *args: list[float], obj: str | object = "main"
     ) -> None:
         """Set the current font to a RGB value."""
         p = self._p if obj == "main" else obj
         p.set_font(args[0], args[1], args[2])
 
+    def _draw_newpage_commit(self, commit, no_divider=False):
+        """Draw a commit that cannot fit on the existing page."""
+        self.footer()
+        self._p.add_page()
+        self._draw_page_bg()
+        self._p.set_auto_page_break(auto=True, margin=MARGIN_TB)
+        self._p.footer = self.footer # Temporarily override the empty ``footer``
+                                     # method inherited from ``FPDF`` to 
+                                     # automatically generate a footer if this
+                                     # new commit spans more than a single page.
+        page_no_before_draw = self._p.page
+        self._draw_commit(commit, no_divider=no_divider)
+        self._p.set_auto_page_break(auto=False)
+        self._p.footer = footer # Set the footer method of ``self._p`` back to 
+                                # an empty method to prevent a recursion error
+                                # when cloning an instance of ``FPDF``.
+        if self._p.page > page_no_before_draw: 
+            self.footer()
+        self.commit_counter += 1
+
     def _draw_commits(self) -> None:
         """Driver function to draw all the commits using either the
         pre-visualisation method or the commit height estimation method.
         """
         self._p.add_page()  # Draw separate to the title page
         self._draw_page_bg()
-
-        self._progress.start()
-        counter: int = 0
+        self.commit_counter: int = 0
         # gen2b
         if self._mode == "unstable":
-            for commit in self._commits.filtered_commits:
+            for commit in tqdm(
+                self._commits.filtered_commits,
+                ncols=85,
+                desc="Generating",
+            ):
                 result = self._draw_commit(commit, pre_vis=True)
                 if result == "NEW_PAGE_OK":  # Break page
-                    self._draw_footer()
-                    self._p.add_page()
-                    self._draw_page_bg()
-                    self._draw_commit(commit)
+                    self._draw_newpage_commit(commit)
                 elif (
                     result == "NEW_PAGE_OK_BUT_NO_DIVIDER"
-                ):  # The divider just
-                    # barely doesn't fit
-                    self._draw_commit(commit, no_divider=True)
+                ):  # The divider just barely doesn't fit
+                    self._draw_newpage_commit(commit, no_divider=True)
                 else:  # No need to break the page
                     self._draw_commit(commit)
-
-                counter += 1
-                self._progress.update(counter)
+                    self.commit_counter += 1
+                    if self.commit_counter == self.commit_count:
+                        self.footer()
 
         # gen2a
         elif self._mode == "stable":
-            for commit in self._commits.filtered_commits:
+            for commit in tqdm(
+                self._commits.filtered_commits,
+                ncols=85,
+                desc="Generating",
+            ):
                 if self._commit_exceeds_size(commit):  # Break page
-                    self._draw_footer()
-                    self._p.add_page()
-                    self._draw_page_bg()
-                self._draw_commit(commit)
-
-                counter += 1
-                self._progress.update(counter)
-
-        self._progress.finish()
+                    self._draw_newpage_commit(commit)
+                else:
+                    self._draw_commit(commit)
+                    self.commit_counter += 1
+                    if self.commit_counter == self.commit_count:
+                        self.footer()
 
     def _draw_commit(
         self,
         commit: dict[str, str],
         pre_vis: bool = False,
         no_divider: bool = False,
     ) -> str | None:
@@ -304,16 +332,23 @@
         )
         self._p.ln()
         self._p.multi_cell(
             0,
             self._p.font_size * 1.5,
             align="C",
             txt=f"Start date: "
-            f"{self._commits.start_date.strftime('%Y-%m-%d') if self._commits.start_date else 'N/A'} "
-            f"| End date: {self._commits.end_date.strftime('%Y-%m-%d') if self._commits.end_date else 'N/A'}",
+            f"{self._commits.start_date.strftime('%d/%m/%Y') if self._commits.start_date else 'N/A'} "
+            f"| End date: {self._commits.end_date.strftime('%d/%m/%Y') if self._commits.end_date else 'N/A'}",
+        )
+        self._p.ln()
+        self._p.multi_cell(
+            0,
+            self._p.font_size * 1.5,
+            align="C",
+            txt=f"Branch: {self._commits.branch}"
         )
         self._p.ln()
         self._p.multi_cell(
             0,
             self._p.font_size * 1.5,
             txt=f"Newest n commits: "
             f"{self._commits.newest_n_commits} | Oldest n commits: "
@@ -321,24 +356,24 @@
             align="C",
         )
         self._p.ln()
         self._p.multi_cell(
             0,
             self._p.font_size * 1.5,
             align="C",
-            txt=f"AND queries: "
-            f"{', '.join(self._commits.queries_all) if self._commits.queries_all else 'None'}",
+            txt=f"Including: "
+            f"{', '.join(self._commits.include) if self._commits.include else 'No specification'}",
         )
         self._p.ln()
         self._p.multi_cell(
             0,
             self._p.font_size * 1.5,
             align="C",
-            txt=f"OR queries: "
-            f"{', '.join(self._commits.queries_any) if self._commits.queries_any else 'None'}",
+            txt=f"Excluding: "
+            f"{', '.join(self._commits.exclude) if self._commits.exclude else 'No specification'}",
         )
         self._p.ln()
         self._p.multi_cell(
             0,
             self._p.font_size * 1.5,
             align="C",
             txt=f"Sorting: "
```

### Comparing `commits2pdf-1.1.8/setup.py` & `commits2pdf-1.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
-with open("README.md") as f:
+with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="commits2pdf",
-    version="1.1.8",
+    version="1.1.9",
     author="Tomas Vana",
     url="https://github.com/tomasvana10/commits2pdf",
     description="View a filtered commit history in PDF form.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     license="MIT",
     platforms="any",
     install_requires=[
         "GitPython",
         "pycairo",
         "fpdf",
-        "progressbar"
+        "tqdm"
     ],
     entry_points={
         "console_scripts": [
             "c2p = commits2pdf.cli:main"
         ]
     },
     classifiers=[
```

