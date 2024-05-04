# Comparing `tmp/image2grid-0.1.0.tar.gz` & `tmp/image2grid-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2grid-0.1.0.tar", max compression
+gzip compressed data, was "image2grid-0.1.1.tar", max compression
```

## Comparing `image2grid-0.1.0.tar` & `image2grid-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-05-03 04:50:34.490774 image2grid-0.1.0/LICENSE
--rw-r--r--   0        0        0     1153 2024-05-03 04:50:34.490909 image2grid-0.1.0/README.md
--rw-r--r--   0        0        0       65 2024-05-03 04:50:34.491251 image2grid-0.1.0/image2grid/__init__.py
--rw-r--r--   0        0        0      453 2024-05-03 04:50:34.491383 image2grid-0.1.0/image2grid/cli.py
--rw-r--r--   0        0        0     4265 2024-05-03 04:50:34.491551 image2grid-0.1.0/image2grid/cropper.py
--rw-r--r--   0        0        0     1087 2024-05-03 04:50:34.492197 image2grid-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 image2grid-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-04 06:52:48.940989 image2grid-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1707 2024-05-04 06:52:48.940989 image2grid-0.1.1/README.md
+-rw-r--r--   0        0        0       65 2024-05-04 06:52:48.940989 image2grid-0.1.1/image2grid/__init__.py
+-rw-r--r--   0        0        0      453 2024-05-04 06:52:48.940989 image2grid-0.1.1/image2grid/cli.py
+-rw-r--r--   0        0        0     4265 2024-05-04 06:52:48.940989 image2grid-0.1.1/image2grid/cropper.py
+-rw-r--r--   0        0        0     1087 2024-05-04 06:52:48.940989 image2grid-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 image2grid-0.1.1/PKG-INFO
```

### Comparing `image2grid-0.1.0/LICENSE` & `image2grid-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image2grid-0.1.0/README.md` & `image2grid-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,68 @@
+Metadata-Version: 2.1
+Name: image2grid
+Version: 0.1.1
+Summary: Turn an image into a grid images
+Home-page: https://github.com/kiwamizamurai
+License: MIT
+Author: kiwamizamurai
+Author-email: 24860100+kiwamizamurai@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: gitpython (==3.1.43)
+Requires-Dist: moviepy (==1.0.3)
+Requires-Dist: pillow (==9.5.0)
+Project-URL: Repository, https://github.com/kiwamizamurai/image2grid
+Description-Content-Type: text/markdown
+
 <div align="center">
   <h1>image2grid</h1>
+  <img src="https://raw.githubusercontent.com/kiwamizamurai/image2grid/main/example.png" alt="example output by image2grid" width="400" height="300">
   <p>
   Generate grid-like images or gifs for your GitHub README Profile.<br />Inspired by <a href=https://github.com/mathdroid/crop-github-images-cli>crop-github-images-cli</a>
   </p>
 </div>
 
+[![Publish to PyPI](https://github.com/kiwamizamurai/image2grid/actions/workflows/publish-to-pypi.yaml/badge.svg)](https://github.com/kiwamizamurai/image2grid/actions/workflows/publish-to-pypi.yaml)
 
 ## Table of contents
 - [Features](#features)
 - [Usage](#usage)
 - [Installation](#installation)
 - [Contribution](#contribution)
 - [Thanks](#thanks)
 
 ## Features
 
-- Split the image into a grid
-- Create gists and upload files
+1. Split the image into a grid
+2. Create gists and upload files
 
 ## Usage
 
 ```bash
-❯ image2grid ./example.png -t Github_Personal_access_token
+❯ image2grid ./example.gif
+❯ image2grid ./example.png -t PAT
 ```
 
+scoped [gist] [Personal Access Token (PAT)](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens) is required if you create a gists.
+
 ## Installation
 
 ```bash
-❯ pip install image2grid
+❯ pipx install image2grid
 ```
 
 ## Contribution
 
 Whether it's reporting bugs, suggesting features, maintaining packages, or submitting a PR, contribution is always welcome! Please read CONTRIBUTING.md for details on how to contribute to bottom.
 
 ![Alt](https://repobeats.axiom.co/api/embed/72ed4cd2868b94489518a171f0404b6de7386c74.svg "Repobeats analytics image")
 
 ## Thanks
 
 - This project is very much inspired by [crop-github-images-cli](https://github.com/mathdroid/crop-github-images-cli)
-- This project is made with reference to [bottom](https://github.com/ClementTsang/bottom)
+- This project is made with reference to [bottom](https://github.com/ClementTsang/bottom)
+
```

#### html2text {}

```diff
@@ -1,15 +1,33 @@
+Metadata-Version: 2.1 Name: image2grid Version: 0.1.1 Summary: Turn an image
+into a grid images Home-page: https://github.com/kiwamizamurai License: MIT
+Author: kiwamizamurai Author-email:
+24860100+kiwamizamurai@users.noreply.github.com Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Dist: gitpython (==3.1.43) Requires-Dist:
+moviepy (==1.0.3) Requires-Dist: pillow (==9.5.0) Project-URL: Repository,
+https://github.com/kiwamizamurai/image2grid Description-Content-Type: text/
+markdown
                            ************ iimmaaggee22ggrriidd ************
+                        [example output by image2grid]
        Generate grid-like images or gifs for your GitHub README Profile.
                       Inspired by _c_r_o_p_-_g_i_t_h_u_b_-_i_m_a_g_e_s_-_c_l_i
-## Table of contents - [Features](#features) - [Usage](#usage) - [Installation]
-(#installation) - [Contribution](#contribution) - [Thanks](#thanks) ## Features
-- Split the image into a grid - Create gists and upload files ## Usage ```bash
-â¯ image2grid ./example.png -t Github_Personal_access_token ``` ##
-Installation ```bash â¯ pip install image2grid ``` ## Contribution Whether
-it's reporting bugs, suggesting features, maintaining packages, or submitting a
-PR, contribution is always welcome! Please read CONTRIBUTING.md for details on
-how to contribute to bottom. ![Alt](https://repobeats.axiom.co/api/embed/
+[![Publish to PyPI](https://github.com/kiwamizamurai/image2grid/actions/
+workflows/publish-to-pypi.yaml/badge.svg)](https://github.com/kiwamizamurai/
+image2grid/actions/workflows/publish-to-pypi.yaml) ## Table of contents -
+[Features](#features) - [Usage](#usage) - [Installation](#installation) -
+[Contribution](#contribution) - [Thanks](#thanks) ## Features 1. Split the
+image into a grid 2. Create gists and upload files ## Usage ```bash â¯
+image2grid ./example.gif â¯ image2grid ./example.png -t PAT ``` scoped [gist]
+[Personal Access Token (PAT)](https://docs.github.com/en/authentication/
+keeping-your-account-and-data-secure/managing-your-personal-access-tokens) is
+required if you create a gists. ## Installation ```bash â¯ pipx install
+image2grid ``` ## Contribution Whether it's reporting bugs, suggesting
+features, maintaining packages, or submitting a PR, contribution is always
+welcome! Please read CONTRIBUTING.md for details on how to contribute to
+bottom. ![Alt](https://repobeats.axiom.co/api/embed/
 72ed4cd2868b94489518a171f0404b6de7386c74.svg "Repobeats analytics image") ##
 Thanks - This project is very much inspired by [crop-github-images-cli](https:/
 /github.com/mathdroid/crop-github-images-cli) - This project is made with
 reference to [bottom](https://github.com/ClementTsang/bottom)
```

### Comparing `image2grid-0.1.0/image2grid/cropper.py` & `image2grid-0.1.1/image2grid/cropper.py`

 * *Files identical despite different names*

### Comparing `image2grid-0.1.0/pyproject.toml` & `image2grid-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "image2grid"
-version = "0.1.0"
+version = "0.1.1"
 description = "Turn an image into a grid images"
 authors = ["kiwamizamurai <24860100+kiwamizamurai@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kiwamizamurai"
 repository = "https://github.com/kiwamizamurai/image2grid"
```

