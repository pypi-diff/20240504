# Comparing `tmp/cvutil-0.0.3.tar.gz` & `tmp/cvutil-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvutil-0.0.3.tar", last modified: Wed Apr 17 10:54:34 2024, max compression
+gzip compressed data, was "cvutil-0.0.4.tar", last modified: Sat May  4 09:31:54 2024, max compression
```

## Comparing `cvutil-0.0.3.tar` & `cvutil-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 osmr      (1000) osmr      (1000)        0 2024-04-17 10:54:34.208789 cvutil-0.0.3/
--rw-r--r--   0 osmr      (1000) osmr      (1000)      839 2024-04-17 10:54:34.208789 cvutil-0.0.3/PKG-INFO
--rw-rw-r--   0 osmr      (1000) osmr      (1000)       88 2024-04-17 10:30:23.000000 cvutil-0.0.3/README.md
-drwxrwxr-x   0 osmr      (1000) osmr      (1000)        0 2024-04-17 10:54:34.208789 cvutil-0.0.3/cvutil/
--rw-rw-r--   0 osmr      (1000) osmr      (1000)       22 2024-04-17 10:42:08.000000 cvutil-0.0.3/cvutil/__init__.py
--rw-rw-r--   0 osmr      (1000) osmr      (1000)     5437 2022-07-03 15:42:54.000000 cvutil-0.0.3/cvutil/envs.py
--rw-rw-r--   0 osmr      (1000) osmr      (1000)     4463 2022-06-12 11:54:56.000000 cvutil-0.0.3/cvutil/ffmpeg.py
--rw-rw-r--   0 osmr      (1000) osmr      (1000)     3439 2022-06-12 12:12:30.000000 cvutil-0.0.3/cvutil/image.py
--rw-rw-r--   0 osmr      (1000) osmr      (1000)     3998 2024-04-17 10:33:08.000000 cvutil-0.0.3/cvutil/logger.py
--rw-rw-r--   0 osmr      (1000) osmr      (1000)     2956 2023-03-30 18:40:27.000000 cvutil-0.0.3/cvutil/math.py
--rw-rw-r--   0 osmr      (1000) osmr      (1000)    15116 2022-06-12 12:15:09.000000 cvutil-0.0.3/cvutil/path.py
--rw-rw-r--   0 osmr      (1000) osmr      (1000)     2369 2024-04-17 10:39:06.000000 cvutil-0.0.3/cvutil/render.py
--rw-rw-r--   0 osmr      (1000) osmr      (1000)     1043 2022-06-12 09:37:10.000000 cvutil-0.0.3/cvutil/strings.py
-drwxrwxr-x   0 osmr      (1000) osmr      (1000)        0 2024-04-17 10:54:34.208789 cvutil-0.0.3/cvutil.egg-info/
--rw-r--r--   0 osmr      (1000) osmr      (1000)      839 2024-04-17 10:54:34.000000 cvutil-0.0.3/cvutil.egg-info/PKG-INFO
--rw-rw-r--   0 osmr      (1000) osmr      (1000)      326 2024-04-17 10:54:34.000000 cvutil-0.0.3/cvutil.egg-info/SOURCES.txt
--rw-rw-r--   0 osmr      (1000) osmr      (1000)        1 2024-04-17 10:54:34.000000 cvutil-0.0.3/cvutil.egg-info/dependency_links.txt
--rw-rw-r--   0 osmr      (1000) osmr      (1000)       23 2024-04-17 10:54:34.000000 cvutil-0.0.3/cvutil.egg-info/requires.txt
--rw-rw-r--   0 osmr      (1000) osmr      (1000)        7 2024-04-17 10:54:34.000000 cvutil-0.0.3/cvutil.egg-info/top_level.txt
--rw-rw-r--   0 osmr      (1000) osmr      (1000)      141 2024-04-17 10:54:34.208789 cvutil-0.0.3/setup.cfg
--rw-rw-r--   0 osmr      (1000) osmr      (1000)     1177 2024-04-17 10:36:01.000000 cvutil-0.0.3/setup.py
+drwxrwxr-x   0 osmr      (1000) osmr      (1000)        0 2024-05-04 09:31:54.215267 cvutil-0.0.4/
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)     1074 2024-04-17 10:30:37.000000 cvutil-0.0.4/LICENSE
+-rw-r--r--   0 osmr      (1000) osmr      (1000)      846 2024-05-04 09:31:54.215267 cvutil-0.0.4/PKG-INFO
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)       88 2024-04-17 10:30:23.000000 cvutil-0.0.4/README.md
+drwxrwxr-x   0 osmr      (1000) osmr      (1000)        0 2024-05-04 09:31:54.215267 cvutil-0.0.4/cvutil/
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)       22 2024-05-04 08:30:16.000000 cvutil-0.0.4/cvutil/__init__.py
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)     5385 2024-05-03 18:13:21.000000 cvutil-0.0.4/cvutil/envs.py
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)     4439 2024-05-03 18:15:48.000000 cvutil-0.0.4/cvutil/ffmpeg.py
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)     3414 2024-05-03 18:17:18.000000 cvutil-0.0.4/cvutil/image.py
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)     3939 2024-05-03 18:31:13.000000 cvutil-0.0.4/cvutil/logger.py
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)     2919 2024-05-03 18:33:32.000000 cvutil-0.0.4/cvutil/math.py
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)    15056 2024-05-03 18:47:16.000000 cvutil-0.0.4/cvutil/path.py
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)      997 2024-05-03 18:35:11.000000 cvutil-0.0.4/cvutil/strings.py
+drwxrwxr-x   0 osmr      (1000) osmr      (1000)        0 2024-05-04 09:31:54.215267 cvutil-0.0.4/cvutil.egg-info/
+-rw-r--r--   0 osmr      (1000) osmr      (1000)      846 2024-05-04 09:31:54.000000 cvutil-0.0.4/cvutil.egg-info/PKG-INFO
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)      317 2024-05-04 09:31:54.000000 cvutil-0.0.4/cvutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)        1 2024-05-04 09:31:54.000000 cvutil-0.0.4/cvutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)       14 2024-05-04 09:31:54.000000 cvutil-0.0.4/cvutil.egg-info/requires.txt
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)        7 2024-05-04 09:31:54.000000 cvutil-0.0.4/cvutil.egg-info/top_level.txt
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)      137 2024-05-04 09:31:54.215267 cvutil-0.0.4/setup.cfg
+-rw-rw-r--   0 osmr      (1000) osmr      (1000)     1174 2024-05-04 08:30:47.000000 cvutil-0.0.4/setup.py
```

### Comparing `cvutil-0.0.3/PKG-INFO` & `cvutil-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cvutil
-Version: 0.0.3
+Version: 0.0.4
 Summary: Set of auxiliary scripts for computer vision tasks
 Home-page: https://github.com/osmr/cvutil
 Author: Oleg Sémery
 Author-email: osemery@gmail.com
 License: MIT
-Keywords: datasets image audio processing
+Keywords: datasets image video audio processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: opencv-python
-Requires-Dist: pyrender
 
 # Computer Vision Auxiliary Scripts
 
 Set of auxiliary scripts for computer vision tasks.
```

### Comparing `cvutil-0.0.3/cvutil/envs.py` & `cvutil-0.0.4/cvutil/envs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 
 __all__ = ['get_env_stats']
 
 import os
 import sys
 import subprocess
 import platform
-from typing import List, Dict, Optional
 
 
-def get_platform_info() -> Dict[str, str]:
+def get_platform_info() -> dict[str, str]:
     """
     Get platform (operational system) information.
 
     Returns
     -------
     dict(str, str)
         Resulted info.
@@ -45,15 +44,15 @@
     """
     try:
         return "{0}.{1}.{2}".format(*sys.version_info[0:3])
     except Exception:
         return "unknown"
 
 
-def get_git_commit_info(script_path: Optional[str] = None) -> str:
+def get_git_commit_info(script_path: str | None = None) -> str:
     """
     Get the last Git repo commit information.
 
     Parameters
     ----------
     script_path : str or None, default None
         Path to a script from repository.
@@ -75,15 +74,15 @@
         output_bytes = subprocess.check_output(command, shell=True)
         output_text = output_bytes.decode("utf-8").strip()
     except Exception:
         output_text = "unknown"
     return output_text
 
 
-def get_package_versions(module_names: List[str]) -> Dict[str, str]:
+def get_package_versions(module_names: list[str]) -> dict[str, str]:
     """
     Get packages information by inspecting __version__ attribute.
 
     Parameters
     ----------
     module_names : list(str)
         List of module names.
@@ -100,16 +99,16 @@
         except ImportError:
             module_versions[module_name] = None
         except AttributeError:
             module_versions[module_name] = "unknown"
     return module_versions
 
 
-def get_pip_package_descriptions(package_names: List[str],
-                                 python_version: str = "") -> Dict[str, str]:
+def get_pip_package_descriptions(package_names: list[str],
+                                 python_version: str = "") -> dict[str, str]:
     """
     Get packages information by using 'pip show' command.
 
     Parameters
     ----------
     package_names : list(str)
         List of package names.
@@ -147,18 +146,18 @@
         output_bytes = subprocess.check_output(["ffmpeg", "-version"])
         output_text = output_bytes.decode("utf-8").strip().split("\n")[0]
     except (subprocess.CalledProcessError, OSError):
         output_text = "unknown"
     return output_text
 
 
-def get_env_stats(packages: Optional[List[str]],
-                  pip_packages: Optional[List[str]],
-                  main_script_path: Optional[str] = None,
-                  check_ffmpeg: bool = False) -> Dict[str, str]:
+def get_env_stats(packages: list[str] | None,
+                  pip_packages: list[str] | None,
+                  main_script_path: str | None = None,
+                  check_ffmpeg: bool = False) -> dict[str, str]:
     """
     Get environment statistics.
 
     Parameters
     ----------
     packages : list(str) or None
         list of package names to inspect only __version__.
```

### Comparing `cvutil-0.0.3/cvutil/ffmpeg.py` & `cvutil-0.0.4/cvutil/ffmpeg.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,17 @@
     Video/audio processing via FFMPEG auxiliary functions.
 """
 
 __all__ = ['extract_frames_from_video', 'extract_audio_from_video', 'merge_video_with_audio']
 
 import logging
 import subprocess
-from typing import List
 
 
-def _run_command(command: List[str],
+def _run_command(command: list[str],
                  show_output: bool = False):
     """
     Run shell command as subprocess.
 
     Parameters
     ----------
     command : list(str)
```

### Comparing `cvutil-0.0.3/cvutil/image.py` & `cvutil-0.0.4/cvutil/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,19 @@
     Image auxiliary functions.
 """
 
 __all__ = ['resize_image', 'resize_image_with_min_size', 'crop_image', 'center_crop_image']
 
 import numpy as np
 import cv2
-from typing import Tuple
 from .math import calc_pad_value
 
 
 def resize_image(image: np.ndarray,
-                 image_size: Tuple[int, int],
+                 image_size: tuple[int, int],
                  interpolation: int = cv2.INTER_LINEAR) -> np.ndarray:
     """
     Resize image.
 
     Parameters
     ----------
     image : np.ndarray
@@ -37,15 +36,15 @@
     else:
         return cv2.resize(image, dsize=image_size[::-1], interpolation=interpolation)
 
 
 def resize_image_with_min_size(image: np.ndarray,
                                min_size: int,
                                downscale: bool = False,
-                               interpolation: int = cv2.INTER_LINEAR) -> Tuple[np.ndarray, Tuple[int, int]]:
+                               interpolation: int = cv2.INTER_LINEAR) -> tuple[np.ndarray, tuple[int, int]]:
     """
     Resize image with minimal size.
 
     Parameters
     ----------
     image : np.ndarray
         Original image.
@@ -68,15 +67,15 @@
     if (scale != 1.0) and ((scale > 1.0) or downscale):
         new_height, new_width = tuple(round(dim * scale) for dim in (height, width))
         image = cv2.resize(image, dsize=(new_width, new_height), interpolation=interpolation)
     return image, (height, width)
 
 
 def crop_image(image: np.ndarray,
-               crop_params: Tuple[int, int, int, int]) -> np.ndarray:
+               crop_params: tuple[int, int, int, int]) -> np.ndarray:
     """
     Crop image patch.
 
     Parameters
     ----------
     image : np.ndarray
         Cropping image.
@@ -90,15 +89,15 @@
     """
     height, width = image.shape[:2]
     x_left_pad, y_left_pad, x_right_pad, y_right_pad = crop_params
     return image[y_left_pad:(height - y_right_pad), x_left_pad:(width - x_right_pad)]
 
 
 def center_crop_image(image: np.ndarray,
-                      dst_image_size: Tuple[int, int]) -> np.ndarray:
+                      dst_image_size: tuple[int, int]) -> np.ndarray:
     """
     Crop image patch from the center so that sides are equal to pads.
 
     Parameters
     ----------
     image : np.ndarray
         Cropping image.
```

### Comparing `cvutil-0.0.3/cvutil/logger.py` & `cvutil-0.0.4/cvutil/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 
 __all__ = ['initialize_logging']
 
 import os
 import sys
 import logging
 import argparse
-from typing import Tuple, Optional
 from .strings import split_str, pretty_print_dict_to_str
 from .envs import get_env_stats
 
 
-def prepare_logger(logging_dir_path: Optional[str],
-                   logging_file_name: Optional[str]) -> Tuple[logging.Logger, bool]:
+def prepare_logger(logging_dir_path: str | None,
+                   logging_file_name: str | None) -> tuple[logging.Logger, bool]:
     """
     Prepare logger.
 
     Parameters
     ----------
     logging_dir_path : str or None
         Path to logging directory.
@@ -46,21 +45,21 @@
         fh = logging.FileHandler(log_file_path)
         logger.addHandler(fh)
         if log_file_exist:
             logging.info("--------------------------------")
     return logger, log_file_exist
 
 
-def initialize_logging(logging_dir_path: Optional[str] = None,
-                       logging_file_name: Optional[str] = None,
-                       main_script_path: Optional[str] = None,
-                       script_args: Optional[argparse.Namespace] = None,
-                       packages: Optional[str] = "log_packages",
-                       pip_packages: Optional[str] = "log_pip_packages",
-                       check_ffmpeg: bool = False) -> Tuple[logging.Logger, bool]:
+def initialize_logging(logging_dir_path: str | None = None,
+                       logging_file_name: str | None = None,
+                       main_script_path: str | None = None,
+                       script_args: argparse.Namespace | None = None,
+                       packages: str | None = "log_packages",
+                       pip_packages: str | None = "log_pip_packages",
+                       check_ffmpeg: bool = False) -> tuple[logging.Logger, bool]:
     """
     Initialize logging subsystem.
 
     Parameters
     ----------
     logging_dir_path : str or None, default None
         Path to logging directory.
```

### Comparing `cvutil-0.0.3/cvutil/math.py` & `cvutil-0.0.4/cvutil/math.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 """
     Mathematical auxiliary functions.
 """
 
 __all__ = ['calc_pad_value', 'encode_vectors_via_pca', 'decode_vectors_via_pca']
 
-from typing import Tuple, Dict, Union
-
 import numpy as np
 
 
 def calc_pad_value(src_value: int,
-                   dst_value: int) -> Tuple[int, int]:
+                   dst_value: int) -> tuple[int, int]:
     """
     Calculate a padding values for a pair of source and destination numbers.
 
     Parameters
     ----------
     src_value : int
         Source number.
     dst_value : int
         Destination number.
 
     Returns
     -------
-    tuple(int, int)
-        Left and right paddings.
+    int
+        Left padding.
+    int
+        Right padding.
     """
     if dst_value < src_value:
         raise Exception("Destination value is smaller than source one")
     if src_value == dst_value:
         pad_left = 0
         pad_right = 0
     else:
         pad_value = dst_value - src_value
         pad_left = pad_value // 2
         pad_right = pad_value - pad_left
     return pad_left, pad_right
 
 
 def encode_vectors_via_pca(vectors: np.ndarray,
-                           pca_params: Dict[str, np.ndarray],
+                           pca_params: dict[str, np.ndarray],
                            calc_whitening: bool = False,
-                           return_both: bool = False) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
+                           return_both: bool = False) -> np.ndarray | tuple[np.ndarray, np.ndarray]:
     """
     Encode (project to subspace) vectors via PCA.
 
     Parameters
     ----------
     vectors : np.ndarray
         Input float vector. It's a matrix (n, m), where n is vector count, m is vector length.
-    pca_params : Dict[str, np.ndarray]
+    pca_params : dict[str, np.ndarray]
         PCA params.
     calc_whitening : bool, default False
         Whether to encode with whitening.
     return_both : bool, default False
         Whether to return both encoded vectors (without whitening and with).
 
     Returns
@@ -70,24 +70,24 @@
         if not return_both:
             return vw
         else:
             return vp, vw
 
 
 def decode_vectors_via_pca(vectors: np.ndarray,
-                           pca_params: Dict[str, np.ndarray],
+                           pca_params: dict[str, np.ndarray],
                            used_whitening: bool = False) -> np.ndarray:
     """
     Decode (reconstruct from subspace projections) vectors via PCA.
 
     Parameters
     ----------
     vectors : np.ndarray
         Input float vector. It's a matrix (n, m), where n is vector count, m is vector length.
-    pca_params : Dict[str, np.ndarray]
+    pca_params : dict[str, np.ndarray]
         PCA params.
     used_whitening : bool, default False
         Whether whitening was used during encoding.
 
     Returns
     -------
     np.ndarray
```

### Comparing `cvutil-0.0.3/cvutil/path.py` & `cvutil-0.0.4/cvutil/path.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,62 +6,61 @@
            'get_json_file_paths', 'gen_output_file_path', 'gen_output_dir_path', 'check_rewrite_file_path',
            'gen_output_file_path_with_rewrite', 'gen_output_dir_path_with_rewrite']
 
 import os
 import re
 import logging
 import shutil
-from typing import Tuple, List, Dict, Union, Optional
 
 
 class FileExtChecker(object):
     """
     File extension checker.
 
     Parameters
     ----------
     exts : tuple(str, ...)
         File extensions.
     force_complex_ext : bool, default False
         Whether to forcibly treat extensions as complex ones.
     """
     def __init__(self,
-                 exts: Tuple[str, ...],
+                 exts: tuple[str, ...],
                  force_complex_ext: bool = False):
         super(FileExtChecker, self).__init__()
         self.exts = exts
         self.has_complex_ext = force_complex_ext or\
                                any([(len(ext) == 0) or (ext[0] != ".") or ("." in ext[1:]) for ext in exts])
 
     def __call__(self, file_name: str) -> bool:
         """
         Process check request.
 
-        Parameters:
+        Parameters
         ----------
         file_name : str
             File name.
 
-        Returns:
+        Returns
         -------
         bool
             Is the file extension the same.
         """
         if self.has_complex_ext:
             return any([file_name.endswith(ext) for ext in self.exts])
         else:
             _, file_ext = os.path.splitext(file_name)
             return file_ext.lower() in self.exts
 
 
 def get_file_paths_in_dir(dir_path: str,
-                          exts: Tuple[str, ...],
+                          exts: tuple[str, ...],
                           explore_subdirs: bool,
                           return_dict: bool,
-                          force_complex_ext: bool = False) -> Union[List[str], Dict[str, str]]:
+                          force_complex_ext: bool = False) -> list[str] | dict[str, str]:
     """
     Get all specific file paths in directory.
 
     Parameters
     ----------
     dir_path : str
         Path to working directory.
@@ -101,29 +100,29 @@
                 continue
             if ext_checker(file_name):
                 if return_dict:
                     file_paths[dir_path].append(file_name)
                 else:
                     file_paths.append(file_path)
 
-    def sort_key(x: List) -> List:
+    def sort_key(x: list) -> list:
         return [int(y) if y.isdigit() else y for y in re.findall(r"[^0-9]|[0-9]+", x)]
 
     if return_dict:
         file_paths = {k: sorted(file_paths[k], key=sort_key) for k in sorted(file_paths.keys(), key=sort_key)}
     else:
         file_paths = sorted(file_paths, key=sort_key)
     return file_paths
 
 
 def get_video_file_paths(dir_path: str,
-                         exts: Tuple[str, ...] = (".mp4", ".mkv", ".avi", ".mov", ".m4v"),
+                         exts: tuple[str, ...] = (".mp4", ".mkv", ".avi", ".mov", ".m4v"),
                          explore_subdirs: bool = False,
-                         return_dict=False,
-                         **kwargs) -> Union[List[str], Dict[str, str]]:
+                         return_dict: bool = False,
+                         **kwargs) -> list[str] | dict[str, str]:
     """
     Get all video file paths in directory.
 
     Parameters
     ----------
     dir_path : str
         Path to working directory.
@@ -144,18 +143,18 @@
         exts=exts,
         explore_subdirs=explore_subdirs,
         return_dict=return_dict,
         **kwargs)
 
 
 def get_image_file_paths(dir_path: str,
-                         exts: Tuple[str, ...] = (".jpg", ".png"),
+                         exts: tuple[str, ...] = (".jpg", ".png"),
                          explore_subdirs: bool = False,
-                         return_dict=False,
-                         **kwargs) -> Union[List[str], Dict[str, str]]:
+                         return_dict: bool = False,
+                         **kwargs) -> list[str] | dict[str, str]:
     """
     Get all image file paths in directory.
 
     Parameters
     ----------
     dir_path : str
         Path to working directory.
@@ -176,18 +175,18 @@
         exts=exts,
         explore_subdirs=explore_subdirs,
         return_dict=return_dict,
         **kwargs)
 
 
 def get_audio_file_paths(dir_path: str,
-                         exts: Tuple[str, ...] = (".wav", ".mp3", "wma"),
+                         exts: tuple[str, ...] = (".wav", ".mp3", "wma"),
                          explore_subdirs: bool = False,
-                         return_dict=False,
-                         **kwargs) -> Union[List[str], Dict[str, str]]:
+                         return_dict: bool = False,
+                         **kwargs) -> list[str] | dict[str, str]:
     """
     Get all audio file paths in directory.
 
     Parameters
     ----------
     dir_path : str
         Path to working directory.
@@ -208,18 +207,18 @@
         exts=exts,
         explore_subdirs=explore_subdirs,
         return_dict=return_dict,
         **kwargs)
 
 
 def get_json_file_paths(dir_path: str,
-                        exts: Tuple[str, ...] = (".json",),
+                        exts: tuple[str, ...] = (".json",),
                         explore_subdirs: bool = False,
-                        return_dict=False,
-                        **kwargs) -> Union[List[str], Dict[str, str]]:
+                        return_dict: bool = False,
+                        **kwargs) -> list[str] | dict[str, str]:
     """
     Get all JSON file paths in directory.
 
     Parameters
     ----------
     dir_path : str
         Path to working directory.
@@ -241,15 +240,15 @@
         explore_subdirs=explore_subdirs,
         return_dict=return_dict,
         **kwargs)
 
 
 def gen_output_file_path(input_file_path: str,
                          output_dir_path: str,
-                         output_file_ext: Optional[str] = None,
+                         output_file_ext: str | None = None,
                          output_file_suf: str = "",
                          input_file_suf_len: int = 0,
                          is_output_dir: bool = False) -> str:
     """
     Generate output file/directory path based on input file path.
 
     Parameters
@@ -361,20 +360,20 @@
     if is_dir:
         os.mkdir(file_path)
     return False
 
 
 def gen_output_file_path_with_rewrite(input_file_path: str,
                                       output_dir_path: str,
-                                      output_file_ext: Optional[str] = None,
+                                      output_file_ext: str | None = None,
                                       output_file_suf: str = "",
                                       input_file_suf_len: int = 0,
                                       is_output_dir: bool = False,
                                       rewrite: bool = False,
-                                      show_message: bool = True) -> Tuple[str, bool]:
+                                      show_message: bool = True) -> tuple[str, bool]:
     """
     Generate output file/directory path based on input file path. And check file/directory for non-existence.
 
     Parameters
     ----------
     input_file_path : str
         Input file path.
@@ -416,15 +415,15 @@
 
 
 def gen_output_dir_path_with_rewrite(input_file_path: str,
                                      output_base_dir_path: str,
                                      output_dir_suf: str,
                                      input_file_suf_len: int = 0,
                                      rewrite: bool = False,
-                                     show_message: bool = True) -> Tuple[str, bool]:
+                                     show_message: bool = True) -> tuple[str, bool]:
     """
     Generate output directory path based on input file path. And check directory for non-existence.
 
     Parameters
     ----------
     input_file_path : str
         Input file path.
```

### Comparing `cvutil-0.0.3/cvutil.egg-info/PKG-INFO` & `cvutil-0.0.4/cvutil.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cvutil
-Version: 0.0.3
+Version: 0.0.4
 Summary: Set of auxiliary scripts for computer vision tasks
 Home-page: https://github.com/osmr/cvutil
 Author: Oleg Sémery
 Author-email: osemery@gmail.com
 License: MIT
-Keywords: datasets image audio processing
+Keywords: datasets image video audio processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: opencv-python
-Requires-Dist: pyrender
 
 # Computer Vision Auxiliary Scripts
 
 Set of auxiliary scripts for computer vision tasks.
```

### Comparing `cvutil-0.0.3/setup.py` & `cvutil-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     author_email='osemery@gmail.com',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
-        'License :: Other/Proprietary License',
+        'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Topic :: Scientific/Engineering :: Image Processing',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
-    keywords='datasets image audio processing',
+    keywords='datasets image video audio processing',
     packages=find_packages(exclude=['others', '*.others', 'others.*', '*.others.*']),
-    install_requires=['opencv-python', 'pyrender'],
-    python_requires='>=3.7',
+    install_requires=['opencv-python'],
+    python_requires='>=3.10',
     include_package_data=True,
 )
```

