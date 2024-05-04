# Comparing `tmp/FixRaidenBoss2-3.6.1.tar.gz` & `tmp/fixraidenboss2-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FixRaidenBoss2-3.6.1.tar", last modified: Mon Mar  4 02:34:21 2024, max compression
+gzip compressed data, was "fixraidenboss2-3.7.0.tar", last modified: Sat May  4 20:32:33 2024, max compression
```

## Comparing `FixRaidenBoss2-3.6.1.tar` & `fixraidenboss2-3.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 02:34:21.517536 FixRaidenBoss2-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-04 02:34:17.000000 FixRaidenBoss2-3.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-03-04 02:34:21.517536 FixRaidenBoss2-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-03-04 02:34:17.000000 FixRaidenBoss2-3.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-04 02:34:17.000000 FixRaidenBoss2-3.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 02:34:21.517536 FixRaidenBoss2-3.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 02:34:21.513536 FixRaidenBoss2-3.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 02:34:21.513536 FixRaidenBoss2-3.6.1/src/FixRaidenBoss2/
--rw-r--r--   0 runner    (1001) docker     (127)   142169 2024-03-04 02:34:17.000000 FixRaidenBoss2-3.6.1/src/FixRaidenBoss2/FixRaidenBoss2.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-04 02:34:17.000000 FixRaidenBoss2-3.6.1/src/FixRaidenBoss2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-04 02:34:17.000000 FixRaidenBoss2-3.6.1/src/FixRaidenBoss2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 02:34:21.517536 FixRaidenBoss2-3.6.1/src/FixRaidenBoss2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-03-04 02:34:21.000000 FixRaidenBoss2-3.6.1/src/FixRaidenBoss2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-04 02:34:21.000000 FixRaidenBoss2-3.6.1/src/FixRaidenBoss2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 02:34:21.000000 FixRaidenBoss2-3.6.1/src/FixRaidenBoss2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-04 02:34:21.000000 FixRaidenBoss2-3.6.1/src/FixRaidenBoss2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:32:33.104026 fixraidenboss2-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-04 20:32:29.000000 fixraidenboss2-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-04 20:32:33.104026 fixraidenboss2-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-05-04 20:32:29.000000 fixraidenboss2-3.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-04 20:32:29.000000 fixraidenboss2-3.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 20:32:33.104026 fixraidenboss2-3.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:32:33.100026 fixraidenboss2-3.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:32:33.100026 fixraidenboss2-3.7.0/src/FixRaidenBoss2/
+-rw-r--r--   0 runner    (1001) docker     (127)   177578 2024-05-04 20:32:29.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2/FixRaidenBoss2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-04 20:32:29.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-04 20:32:29.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:32:33.104026 fixraidenboss2-3.7.0/src/FixRaidenBoss2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-04 20:32:33.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-04 20:32:33.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 20:32:33.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 20:32:33.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2.egg-info/top_level.txt
```

### Comparing `FixRaidenBoss2-3.6.1/LICENSE` & `fixraidenboss2-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FixRaidenBoss2-3.6.1/pyproject.toml` & `fixraidenboss2-3.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FixRaidenBoss2"
-version = "3.6.1"
+version = "3.7.0"
 authors = [
   {name="nhok0169", email="qqqqaaaapppp0000@gmail.com"},
   {name="Albert Gold", email="AlexXianZhenYuAu@gmail.com"}
 ]
 description = "A script to fix Raiden Shogun Boss Phase 1 for all types of mods"
 readme = "README.md"
 classifiers = [
```

### Comparing `FixRaidenBoss2-3.6.1/src/FixRaidenBoss2/FixRaidenBoss2.py` & `fixraidenboss2-3.7.0/src/FixRaidenBoss2/FixRaidenBoss2.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,48 +7,36 @@
 
 
 import os
 import configparser
 import re
 import struct
 import traceback
-from typing import List, Callable, Optional, Union, Dict, Any, TypeVar, Hashable, Tuple, Set
-from collections import deque
+from typing import List, Callable, Optional, Union, Dict, Any, TypeVar, Hashable, Tuple, Set, DefaultDict
+from collections import deque, defaultdict, OrderedDict
+from functools import cmp_to_key
+from enum import Enum
 import argparse
 import ntpath
 
 
-VGRemap = {'0':'0','1':'1','2':'2','3':'3','4':'4','5':'5','6':'6','7':'7','8':'60','9':'61','10':'66','11':'67',
-             '12':'8','13':'9','14':'10','15':'11','16':'12','17':'13','18':'14','19':'15','20':'16','21':'17',
-             '22':'18','23':'19','24':'20','25':'21','26':'22','27':'23','28':'24','29':'25','30':'26','31':'27',
-             '32':'28','33':'29','34':'30','35':'31','36':'32','37':'33','38':'34','39':'35','40':'36','41':'37',
-             '42':'38','43':'39','44':'40','45':'41','46':'42','47':'94','48':'43','49':'44','50':'45','51':'46',
-             '52':'47','53':'48','54':'49','55':'50','56':'51','57':'52','58':'53','59':'54','60':'55','61':'56',
-             '62':'57','63':'58','64':'59','65':'114','66':'116','67':'115','68':'117','69':'74','70':'62','71':'64',
-             '72':'106','73':'108','74':'110','75':'75','76':'77','77':'79','78':'87','79':'89','80':'91','81':'95',
-             '82':'97','83':'99','84':'81','85':'83','86':'85','87':'68','88':'70','89':'72','90':'104','91':'112',
-             '92':'93','93':'63','94':'65','95':'107','96':'109','97':'111','98':'76','99':'78','100':'80','101':'88',
-             '102':'90','103':'92','104':'96','105':'98','106':'100','107':'82','108':'84','109':'86','110':'69',
-             '111':'71','112':'73','113':'105','114':'113','115':'101','116':'102','117':'103'}
-MaxVGIndex = 117
-
 # change our current working directory to this file, allowing users to run program
 #   by clicking on the script instead of running by CLI
 if __name__ == "__main__":
     os.chdir(os.path.dirname(os.path.abspath(__file__)))
 
 DefaultFileType = "file"
 DefaultPath = os.getcwd()
 CurrentDir = "."
 IniExt = ".ini"
 TxtExt = ".txt"
 BufExt = ".buf"
 IniExtLen = len(IniExt)
 MergedFile = f"merged{IniExt}"
-BackupFilePrefix = "DISABLED_RSFixBackup_"
+BackupFilePrefix = "DISABLED_BossFixBackup_"
 DuplicateFilePrefix = "DISABLED_RSDup_"
 LogFile = f"RSFixLog{TxtExt}"
 
 IniFileType = "*.ini file"
 BlendFileType = f"Blend{BufExt}"
 RemapBlendFile = f"Remap{BlendFileType}"
 IniFileEncoding = "utf-8"
@@ -56,21 +44,61 @@
 
 Deprecated = "DEPRECATED"
 
 DeleteBackupOpt = '--deleteBackup'
 FixOnlyOpt = '--fixOnly'
 RevertOpt = '--revert'
 AllOpt = '--all'
-argParser = argparse.ArgumentParser(description='Fixes Raiden Boss Phase 1 for all types of mods', formatter_class=argparse.MetavarTypeHelpFormatter)
-argParser.add_argument('-s', '--src', action='store', type=str, help="The path to the Raiden mod folder. If this option is not specified, then will use the current directory as the mod folder.")
+TypeOpt = "--types"
+
+
+# BossFixFormatter: Text formatting for the help page of the command 
+class BossFixFormatter(argparse.MetavarTypeHelpFormatter, argparse.RawTextHelpFormatter):
+    pass
+
+# ConfigParserDict: Dictionary used to only keep the value of the first instance of a key
+class ConfigParserDict(OrderedDict):
+    def __setitem__(self, key, value):
+        # All values updated into the dictionary of ConfigParser will first updated as a list of values, then
+        #    the list of values will be turned into a string
+        #
+        # eg. the 'value' argument for the __setitem__ method in the case a key has 2 duplicates
+        # >> value = ["val1"]           <----------- we only want this list
+        # >> value = ["val1", "", "val2"]
+        # >> value = ["val1", "", "val2", "", "val3"]
+        # >> value = "val1\nval2\nval3"
+        #
+        # Note:
+        #   For the case of duplicate keys, GIMI will only keep the value of the first valid instance of the key.
+        #       Since checking for correct syntax and semantics is out of the scope of this program, we only get 
+        #        the value of the first instance of the key
+        if (key in self and isinstance(self[key], list) and isinstance(value, list)):
+            return
+
+        super().__setitem__(key, value)
+
+argParser = argparse.ArgumentParser(description='Fixes Raiden Boss Phase 1 for all types of mods', formatter_class=BossFixFormatter)
+argParser.add_argument('-s', '--src', action='store', type=str, help="The starting path to run this fix. If this option is not specified, then will run the fix from the current directory.")
 argParser.add_argument('-d', DeleteBackupOpt, action='store_true', help=f'deletes backup copies of the original {IniExt} files')
 argParser.add_argument('-f', FixOnlyOpt, action='store_true', help='only fixes the mod without cleaning any previous runs of the script')
 argParser.add_argument('-r', RevertOpt, action='store_true', help='reverts back previous runs of the script')
-argParser.add_argument('-l', '--log', action='store_true', help=f'Logs the printed out log into a seperate {TxtExt} file')
-argParser.add_argument('-a', AllOpt, action='store_true', help=f'Parses all {IniFileType}s that the program encounters instead of only parsing {IniFileType}s that have the section [TextureOverrideRaidenShogunBlend]')
+argParser.add_argument('-l', '--log', action='store', type=str, help=f'The folder location to log the printed out text into a seperate {TxtExt} file. If this option is not specified, then will not log the printed out text.')
+argParser.add_argument('-a', AllOpt, action='store_true', help=f'Parses all {IniFileType}s that the program encounters. This option supersedes the {TypeOpt} option')
+argParser.add_argument('-n', '--defaultType', action='store', type=str, help=f'''The default mod type to use if the {IniFileType} belongs to some unknown mod
+If the {AllOpt} is set to True, then this argument will be 'raiden'.
+Otherwise, if this value is not specified, then any mods with unknown types will be skipped
+
+See below for the different names/aliases of the supported types of mods.''')
+argParser.add_argument('-t', TypeOpt, action='store', type=str, help=f'''Parses {IniFileType}s that the program encounters for only specific types of mods. If the {AllOpt} option has been specified, this option has no effect. 
+By default, if this option is not specified, will parse the {IniFileType}s for all the supported types of mods. 
+
+Please specify the types of mods using the the mod type's name or alias, then seperate each name/alias with a comma(,)
+eg. raiden,arlecchino,ayaya
+
+See below for the different names/aliases of the supported types of mods.''')
 
 T = TypeVar('T')
 Pattern = TypeVar('Pattern')
 TextIoWrapper = TypeVar('TextIoWrapper')
 
 
 class Error(Exception):
@@ -82,20 +110,14 @@
     message: :class:`str`
         the error message to print out
     """
 
     def __init__(self, message: str):
         super().__init__(f"ERROR: {message}")
 
-    def warn(self):
-        """
-        Retrieves the warning message for the exception
-        """
-        return str(self).replace("ERROR", "WARNING")
-
 
 class FileException(Error):
     """
     This Class inherits from :class:`Error`
 
     Exceptions relating to files
 
@@ -188,44 +210,99 @@
     def __init__(self, fileType: str = DefaultFileType, path: Optional[str] = None):
         path = FileService.getPath(path)
         message = f"Unable to find {fileType}. Ensure it is in the folder"
         self.fileType = fileType
         super().__init__(message, path = path)
 
 
+class RemapMissingBlendFile(FileException):
+    """
+    This Class inherits from :class:`FileException`
+
+    Exception when a RemapBlend.buf file is missing its corresponding Blend.buf file
+
+    Parameters
+    ----------
+    remapBlend: :class:`str`
+        The path to the RemapBlend.buf file
+    """
+
+    def __init__(self, remapBlend: str):
+        super().__init__(f"Missing the corresponding Blend.buf file for the RemapBlend.buf", path = remapBlend)
+
+
 class BlendFileNotRecognized(FileException):
     """
     This Class inherits from :class:`FileException`
 
     Exception when a Blend.buf file cannot be read
 
     Parameters
     ----------
     blendFile: :class:`str`
         The file path to the Blend.buf file
     """
     def __init__(self, blendFile: str):
         super().__init__(f"Blend file format not recognized for {os.path.basename(blendFile)}", path = os.path.dirname(blendFile))
 
+class BadBlendData(Error):
+    """
+    This Class inherits from :class:`Error`
+
+    Exception when certain bytes do not correspond to the format defined for a Blend.buf file
+    """
+
+    def __init__(self):
+        super().__init__(f"Bytes do not corresponding to the defined format for a Blend.buf file")
+
 
 class ConflictingOptions(Error):
     """
     This Class inherits from :class:`Error`
 
-    Exception when the script or :class:`RaidenBossFixService` is ran with options that cannot be used together
+    Exception when the script or :class:`BossFixService` is ran with options that cannot be used together
 
     Parameters
     ----------
     options: List[:class:`str`]
         The options that cannot be used together
     """
     def __init__(self, options: List[str]):
         optionsStr = ", ".join(options)
         super().__init__(f"The following options cannot be used toghether: {optionsStr}")
 
+class InvalidModType(Error):
+    """
+    This Class inherits from :class:`Error`
+
+    Exception when the type of mod specified to fix is not found
+
+    Parameters
+    ----------
+    type: :class:`str`
+        The name for the type of mod specified
+    """
+    def __init__(self, type: str):
+        super().__init__(f"Unable to find the type of mod by the search string, '{type}'")
+
+class NoModType(Error):
+    """
+    This Class inherits from :class:`Error`
+
+    Exception when trying to fix a mod of some unidentified mod type
+
+    Parameters
+    ----------
+    type: :class:`str`
+        The name for the type of mod specified 
+    """
+
+    def __init__(self):
+        super().__init__(f"No mod type specified when fixing the .ini file")
+
 
 class DictTools():
     """
     Tools for handling with Dictionaries
     """
 
     @classmethod
@@ -234,14 +311,17 @@
         Retrieves the first key in a dictionary
 
         Parameters
         ----------
         dict: Dict[Any, Any]
             The dictionary we are working with
 
+            .. note::
+                The dictionary must not be empty
+
         Returns
         -------
         Any
             The first key of the dictionary
         """
 
         return next(iter(dict))
@@ -262,88 +342,41 @@
             The first value of the dictionary
         """
 
         return dict[cls.getFirstKey(dict)]
     
     # combine(dst, src, combine_duplicate): Combines dictionaries to 'dst'
     @classmethod
-    def combine(cls, dst: Dict[Hashable, Any], src: Dict[Hashable, Any], combineDuplicate: Optional[Callable[[Any, Any], Any]] = None):
+    def combine(cls, dict1: Dict[Hashable, Any], dict2: Dict[Hashable, Any], combineDuplicate: Optional[Callable[[Any, Any], Any]] = None) -> Dict[Hashable, Any]:
         """
         Combines 2 dictionaries
 
         Parameters
         ----------
-        dst: Dict[Hashable, Any]
+        dict1: Dict[Hashable, Any]
             The destination of where we want the combined dictionaries to be stored
 
-        src: Dict[Hashable, Any]
+        dict2: Dict[Hashable, Any]
             The that we want to combine values with
 
         combineDuplicate: Optional[Callable[[Any, Any], Any]]
             Function for handling cases where there contains the same key in both dictionaries
 
-            If this value is set to ``None``, then will use the key from 'dst' :raw-html:`<br />` :raw-html:`<br />`
+            If this value is set to ``None``, then will use the key from 'dict2' :raw-html:`<br />` :raw-html:`<br />`
 
             **Default**: ``None``
         """
-
+        new_dict = {**dict1, **dict2}
         if (combineDuplicate is None):
-            dst.update(src)
-            return dst
-        
-        new_dict = {**dst, **src}
+            return new_dict
+
         for key, value in new_dict.items():
-            if key in dst and key in src:
-                new_dict[key] = combineDuplicate(value, src[key])
+            if key in dict1 and key in dict2:
+                new_dict[key] = combineDuplicate(value, dict1[key])
         return new_dict
-    
-
-class ListTools():
-    """
-    Tools for handling with lists
-    """
-
-    @classmethod
-    def to_dict(cls, lst: List[T], get_id: Callable[[T], Hashable]) -> Dict[Hashable, T]:
-        """
-        Turns a list into a dictionary
-
-        Parameters
-        ----------
-        lst: List[T]
-            The list that we want to turn into a dictionary
-
-        get_id: Callable[[T], Hashable]
-            The function for generating ids for the list
-
-        Returns
-        -------
-        Dict[Hashable, T]
-            The transformed dictionary from the list
-        """
-
-        return {get_id(e): e for e in lst}
-
-    @classmethod
-    def getDistinct(cls, lst: List[T]) -> List[T]:
-        """
-        Retrieves a list with distinct values
-
-        Parameters
-        ----------
-        lst: List[T]
-            The list that we are working with
-
-        Returns
-        -------
-        List[T]
-            A list where all values are distinct
-        """
-
-        return list(dict.fromkeys(lst))
 
 
 class FileService():
     """
     Tools for handling with files and folders :raw-html:`<br />` :raw-html:`<br />`
     """
 
@@ -395,54 +428,35 @@
             if (os.path.isfile(fullPath)):
                 files.append(fullPath)
             else:
                 dirs.append(fullPath)
 
         return [files, dirs]
 
-    @classmethod
-    def isFile(cls, path: str, file: str) -> bool:
-        """
-        Checks whether a file path is a file
-
-        Parameters
-        ----------
-        path: :class:`str`
-            The file path to the folder where the file is contained
-
-        file: :class:`str`
-            The name of the file
-
-        Returns
-        -------
-        :class:`bool`
-            Whether the combined file path is a file
-        """
-
-        fullPath = os.path.join(path, file)
-        return os.path.isfile(fullPath)
-
     # filters and partitions the files based on the different filters specified
     @classmethod
-    def getFiles(cls, path: Optional[str] = None, filters: List[Callable[[str], bool]] = [], files: Optional[List[str]] = None) -> Union[List[str], List[List[str]]]:
+    def getFiles(cls, path: Optional[str] = None, filters: Optional[List[Callable[[str], bool]]] = None, files: Optional[List[str]] = None) -> Union[List[str], List[List[str]]]:
         """
         Retrieves many different types of files within a folder
 
+        .. note::
+            Only retrieves files that are the direct children of the folder (will not retrieve files nested in a folder within the folder we are searching)
+
         Parameters
         ----------
         path: Optional[:class:`str`]
             The path to the target folder we are working with. If this value is set to ``None``, then will use the current directory of where this module is loaded
             :raw-html:`<br />` :raw-html:`<br />`
 
             **Default**: ``None``
 
-        filters: List[Callable[[:class:`str`], :class:`bool`]]
-            Different filter functions for each type of file we are trying to get :raw-html:`<br />` :raw-html:`<br />`
+        filters: Optional[List[Callable[[:class:`str`], :class:`bool`]]]
+            Different filter functions for each type of file we are trying to get. If this values is either ``None`` or ``[]``, then will default to a filter to get all the files :raw-html:`<br />` :raw-html:`<br />`
 
-            **Default**: []
+            **Default**: ``None``
 
         files: Optional[List[:class:`str`]]
             The files contained in the target folder
 
             If this value is set to ``None``, then the function will search for the files :raw-html:`<br />` :raw-html:`<br />`
 
             **Default**: ``None``
@@ -455,74 +469,65 @@
             If 'filters' only has 1 element, then the function returns List[:class:`str`]
             Otherwise, will return List[List[:class:`str`]]
         """
 
         path = cls.getPath(path)
         result = []
 
+        if (filters is None):
+            filters = []
+
         if (not filters):
             filters.append(lambda itemPath: True)
 
-        pathFilters = []
         filtersLen = len(filters)
-
         usePathFiles = False
         if (files is None):
             files = os.listdir(path)
             usePathFiles = True
 
         for i in range(filtersLen):
-            filter = filters[i]
             result.append([])
-
-            if (usePathFiles):
-                newFilter = lambda itemPath: filters[i](itemPath) and cls.isFile(path, itemPath)
-            else:
-                newFilter = filter
-
-            pathFilters.append(newFilter)
-
+        
         for itemPath in files:
             for filterInd in range(filtersLen):
                 pathFilter = filters[filterInd]
-                if (not pathFilter(itemPath)):
+                if (not pathFilter(itemPath) or (usePathFiles and not os.path.isfile(os.path.join(path, itemPath)))):
                     continue
-                
-                fullPath = itemPath
-                if (usePathFiles):
-                    fullPath = os.path.join(path, itemPath)
+
+                fullPath = os.path.join(path, itemPath)
 
                 result[filterInd].append(fullPath)
 
         if (filtersLen == 1):
             return result[0]
         
         return result
     
     # retrieves only a single file for each filetype specified by the filters
     @classmethod
-    def getSingleFiles(cls, path: Optional[str] = None, filters: Dict[str, Callable[[str], bool]] = {}, files: Optional[List[str]] = None, optional: bool = False) -> Union[Optional[str], List[str], List[Optional[str]]]:
+    def getSingleFiles(cls, path: Optional[str] = None, filters: Optional[Dict[str, Callable[[str], bool]]] = None, files: Optional[List[str]] = None, optional: bool = False) -> Union[Optional[str], List[str], List[Optional[str]]]:
         """
         Retrieves exactly 1 of each type of file in a folder
 
         Parameters
         ----------
         path: Optional[:class:`str`]
             The path to the target folder we are searching. :raw-html:`<br />` :raw-html:`<br />`
             
             If this value is set to ``None``, then will use the current directory of where this module is loaded :raw-html:`<br />` :raw-html:`<br />`
 
             **Default**: ``None``
 
-        filters: Dict[str, Callable[[:class:`str`], :class:`bool`]]
-            Different filter functions for each type of file we are trying to get.
+        filters: Optional[Dict[str, Callable[[:class:`str`], :class:`bool`]]]
+            Different filter functions for each type of file we are trying to get. If this value is ``None`` or ``{}``, then will default to use a filter to get all files
 
             The keys are the names for the file type :raw-html:`<br />` :raw-html:`<br />`
 
-            **Default**: {}
+            **Default**: ``None``
 
         files: Optional[List[:class:`str`]]
             The files contained in the target folder
 
             If this value is set to ``None``, then the function will search for the files :raw-html:`<br />` :raw-html:`<br />`
 
             **Default**: ``None``
@@ -552,14 +557,17 @@
 
             * If ``filters`` only contains 1 element and ``optional`` is ``False``, then will return :class:`str`
             * If ``filters`` contains more than 1 element and ``optional`` is ``False`, then will return List[:class:`str`]
             * If ``filters`` only contains 1 element and ``optional`` is ``True``, then will return Optional[:class:`str`]
             * Otherwise, returns List[Optional[:class:`str`]]
         """
         path = cls.getPath(path)
+        if (filters is None):
+            filters = {}
+
         if (not filters):
             filters[DefaultFileType] = lambda itemPath: True
         
         filesPerFileTypes = cls.getFiles(path = path, filters = list(filters.values()), files = files)
         filtersLen = len(filters)
 
         onlyOneFilter = filtersLen == 1
@@ -601,14 +609,16 @@
         ----------
         oldFile: :class:`str`
             file path to the target file we are working with
 
         newFile: :class:`str`
             new file path for the target file 
         """
+        if (oldFile == newFile):
+            return
 
         try:
             os.rename(oldFile, newFile)
         except FileExistsError:
             os.remove(newFile)
             os.rename(oldFile, newFile)
 
@@ -650,21 +660,21 @@
         ----------
         file: :class:`str`
             The file path to the file we are working with
 
         filePrefix: :class:`str`
             Prefix name we want to add in front of the file name :raw-html:`<br />` :raw-html:`<br />`
 
-            **Default**: "DISABLED_RSFixBackup\_"
+            **Default**: "DISABLED_BossFixBackup\_"
         """
 
         baseName = os.path.basename(file)
         baseName = FileService.changeExt(baseName, TxtExt)
 
-        backupFile = os.path.join(os.path.dirname(file), filePrefix) + baseName
+        backupFile = os.path.join(os.path.dirname(file), filePrefix + baseName)
         FileService.rename(file, backupFile)
 
     @classmethod
     def parseOSPath(cls, path: str):
         """
         Retrieves a normalized file path from a string
 
@@ -718,17 +728,16 @@
             The absolute path for the target file
         """
 
         relFolder = os.path.abspath(relFolder)
         result = dstPath
         if (not os.path.isabs(result)):
             result = os.path.join(relFolder, result)
-            result = cls.parseOSPath(result)
 
-        return result
+        return cls.parseOSPath(result)
     
     @classmethod
     def getRelPath(cls, path: str, start: str) -> str:
         """
         Tries to get the relative path of a file/folder relative to another folder, if possible.
 
         If it is not possible to get the relative path, will return back the original file path
@@ -756,15 +765,15 @@
         try:
             result = os.path.relpath(path, start)
 
         # if the path is in another mount than 'start'
         except ValueError:
             pass
 
-        return result
+        return cls.parseOSPath(result)
     
     # read(file, fileCode, postProcessor): Tries to read a file using different encodings
     @classmethod
     def read(cls, file: str, fileCode: str, postProcessor: Callable[[TextIoWrapper], Any]) -> Any:
         """
         Tries to read a file using different file encodings
 
@@ -786,28 +795,119 @@
 
         Returns
         -------
         Any
             The result after processing the file pointer of the opened file
         """
 
+        error = None
         for encoding in ReadEncodings:
             try:
                 with open(file, fileCode, encoding = encoding) as f:
                     return postProcessor(f)
-            except UnicodeDecodeError:
-                pass
+            except UnicodeDecodeError as e:
+                error = e
+
+        if (error is not None):
+            raise UnicodeDecodeError(f"Cannot decode the file using any of the following encodings: {ReadEncodings}")
 
     @classmethod
     def getPath(cls, path: Optional[str]) -> str:
         if (path is None):
             return DefaultPath
         return path
 
 
+
+class Heading():
+    """
+    Class for handling information about a heading for pretty printing
+
+    Examples
+    --------
+
+    .. code-block:: python
+        :linenos:
+        :emphasize-lines: 1,3
+
+        ======= Title: Fix Raiden Boss 2 =======
+        ...
+        ========================================
+
+    Parameters
+    ----------
+    title: :class:`str`
+        The title for the heading :raw-html:`<br />` :raw-html:`<br />`
+
+        **Default**: ""
+
+    sideLen: :class:`int`
+        The number of characters we want one side for the border of the opening heading to have :raw-html:`<br />` :raw-html:`<br />`
+
+        **Default**: 0
+
+    sideChar: :class:`str`
+        The type of character we want the border for the heading to have  :raw-html:`<br />` :raw-html:`<br />`
+
+        **Default**: "="
+
+    Attributes
+    ----------
+    title: :class:`str`
+        The title for the heading
+
+    sideLen: :class:`int`
+        The number of characters we want one side for the border of the opening heading to have
+
+    sideChar: :class:`str`
+        The type of character we want the border for the heading to have
+    """
+
+    def __init__(self, title: str = "", sideLen: int = 0, sideChar: str = "="):
+        self.title = title
+        self.sideLen = sideLen
+        self.sideChar = sideChar
+
+    def copy(self):
+        """
+        Makes a new copy of a heading
+
+        Returns
+        -------
+        :class:`Heading`
+            The new copy of the heading
+        """
+        return Heading(title = self.title, sideLen = self.sideLen, sideChar = self.sideChar)
+
+    def open(self) -> str:
+        """
+        Makes the opening heading (see line 1 of the example at :class:`Heading`)
+
+        Returns
+        -------
+        :class:`str`
+            The opening heading created
+        """
+
+        side = self.sideLen * self.sideChar
+        return f"{side} {self.title} {side}"
+
+    def close(self) -> str:
+        """
+        Makes the closing heading (see line 3 of the example at :class:`Heading`)
+
+        Returns
+        -------
+        :class:`str`
+            The closing heading created
+        """
+
+        return self.sideChar * (2 * (self.sideLen + 1) + len(self.title))
+
+
 class Logger():
     """
     Class for pretty printing output to display on the console
 
     Parameters
     ----------
     prefix: :class:`str`
@@ -823,51 +923,43 @@
     verbose: :class:`bool`
         Whether to print out output :raw-html:`<br />` :raw-html:`<br />`
 
         **Default**: ``True``
 
     Attributes
     ----------
-    _prefix: :class:`str`
-        line that is printed before any message is printed out
-
-    _headingTxtLen: :class:`int`
-        The number of characters used for the name of the opening heading
-
-    _headingSideLen: :class:`int`
-        The number of characters used to make side border of an opening/closing heading
-
-    _headingChar: :class:`str`
-        The character used to make the border of an opening/closing heading
-
     includePrefix: :class:`bool`
         Whether to include the prefix string when printing out a message
 
     verbose: :class:`bool`
         Whether to print out output
 
     logTxt: :class:`bool`
         Whether to log all the printed messages into a .txt file once the fix is done
 
+    _prefix: :class:`str`
+        line that is printed before any message is printed out
+
+    _headings: Deque[:class:`Heading`]
+        A stack of headings that have been opened (by calling :meth:`Heading.open`), but have not been closed yet (have not called :meth:`Heading.close` yet)
+
     _loggedTxt: :class:`str`
         The text that will be logged into a .txt file
     """
 
     DefaultHeadingSideLen = 2
     DefaultHeadingChar = "="
 
     def __init__(self, prefix: str = "", logTxt: bool = False, verbose: bool = True):
         self._prefix = prefix
-        self._headingTxtLen = 0
-        self._headingSideLen = 0
-        self._headingChar = ""
         self.includePrefix = True
         self.verbose = verbose
         self.logTxt = logTxt
         self._loggedTxt = ""
+        self._headings = deque()
         self._currentPrefixTxt = ""
 
         self._setDefaultHeadingAtts()
 
     @property
     def prefix(self):
         """
@@ -939,23 +1031,22 @@
 
         Parameters
         ----------
         message: :class:`str`
             The message we want to print out
         """
 
-        if (not self.verbose):
-            return
-
         if (self.includePrefix):
             message = self.getStr(message)
 
         self._addLogTxt(message)
-        self._currentPrefixTxt += message
-        print(message)
+        self._currentPrefixTxt += f"{message}\n"
+
+        if (self.verbose):
+            print(message)
 
     def split(self):
         """
         Prints out a new line
         """
 
         if (self._currentPrefixTxt):
@@ -973,41 +1064,40 @@
 
         Parameters
         ----------
         txt: :class:`str`
             The message we want to print out
 
         sideLen: :class:`int`
-            How many characters we want for the side border of the heading :raw-html:`<br />` :raw-html:`<br />`
+            How many characters we want for the side border of the heading :raw-html:`<br />`
+            (see line 1 of the example at :class:`Heading`) :raw-html:`<br />` :raw-html:`<br />`
 
             **Default**: 2
 
         headingChar: :class:`str`
-            The character used to print the side border of the heading :raw-html:`<br />` :raw-html:`<br />`
+            The type of character used to print the side border of the heading :raw-html:`<br />`
+            (see line 3 of the example at :class:`Heading`) :raw-html:`<br />` :raw-html:`<br />`
 
             **Default**: "="
         """
 
-        self._headingTxtLen = len(txt)
-        self._headingSideLen = sideLen
-        self._headingChar = headingChar
-        
-        side = headingChar * sideLen
-        self.log(f"{side} {txt} {side}")
+        heading = Heading(title = txt, sideLen = sideLen, sideChar = headingChar)
+        self._headings.append(heading)
+        self.log(heading.open())
 
     def closeHeading(self):
         """
-        Prints out a closing heading that corresponds to a previous opening heading printed
+        Prints out a closing heading that corresponds to a previous opening heading printed (see line 3 of the example at :class:`Heading`)
         """
 
-        side = self._headingChar * self._headingSideLen
-        mid = self._headingChar * (self._headingTxtLen + 2)
-        self.log(f"{side}{mid}{side}")
+        if (not self._headings):
+            return
 
-        self._setDefaultHeadingAtts()
+        heading = self._headings.pop()
+        self.log(heading.close())
 
     @classmethod
     def getBulletStr(self, txt: str) -> str:
         """
         Creates the string for an item in an unordered list
 
         Parameters
@@ -1105,71 +1195,31 @@
 
         Parameters
         ----------
         message: :class:`str`
             The message we want to print out
         """
 
-        self.space()
         prevVerbose = self.verbose
-        self.verbose = True
+        if (not self.logTxt):
+            self.verbose = True
 
-        self.box(message, "!!!!!!!!!!!!!!!!!!!!!!!!!!!!!")
         self.space()
-        self.verbose = prevVerbose
-
-    def note(self, message: str):
-        """
-        Prints an important note that the user should take note of
-
-        Parameters
-        ----------
-        message: :class:`str`
-            The message we want to print out
-        """
 
+        self.box(message, "!!!!!!!!!!!!!!!!!!!!!!!!!!!!!")
         self.space()
-        self.box(f"Note: {message}", "*****************************")
-
-    @classmethod
-    def getWarnStr(self, exception: Error) -> str:
-        """
-        Retrieves the string for a warning
-
-        Parameters
-        ----------
-        exception: :class:`Error`
-            The warning we want to handle
-
-        Returns
-        -------
-        :class:`str`
-            The warning string
-        """
-        
-        return f"{type(exception).__name__}: {exception.warn()}"
-    
-    def warn(self, exception: Error):
-        """
-        Prints a warning
-
-        Parameters
-        ----------
-        exception: :class:`Error`
-            The warning we want to handle
-        """
-        self.error(self.getWarnStr(exception))
+        self.verbose = prevVerbose
 
-    def handleException(self, exception: BaseException):
+    def handleException(self, exception: Exception):
         """
         Prints the message for an error
 
         Parameters
         ----------
-        exception: :class:`BaseException`
+        exception: :class:`Exception`
             The error we want to handle
         """
 
         message = f"\n{type(exception).__name__}: {exception}\n\n{traceback.format_exc()}"
         self.error(message)
 
     def input(self, desc: str) -> str:
@@ -1333,14 +1383,257 @@
 
         if (self.origBlendPaths is not None):
             for partIndex in self.origBlendPaths:
                 path = self.origBlendPaths[partIndex]
                 self.origFullPaths[partIndex] = FileService.absPathOfRelPath(path, iniFolderPath)
 
 
+class ModType():
+    """
+    Class for defining a generic type of mod
+
+    Parameters
+    ----------
+    name: :class:`str`
+        The default name for the type of mod
+
+    check: Union[:class:`str`, `Pattern`_, Callable[[:class:`str`], :class:`bool`]]
+        The specific check used to identify the .ini file belongs to the specific type of mod when checking arbitrary line in a .ini file :raw-html:`<br />` :raw-html:`<br />`
+
+        #. If this argument is a string, then will check if a line in the .ini file equals to this argument
+        #. If this argument is a regex pattern, then will check if a line in the .ini file matches this regex pattern
+        #. If this argument is a function, then will check if a line in the .ini file will make the function for this argument return `True`
+
+    bossHash: :class:`str`
+        The hash for the Vertex Group Blend of the boss
+
+    aliases: Optional[List[:class:`str`]]
+        Other alternative names for the type of mod :raw-html:`<br />` :raw-html:`<br />`
+
+        **Default**: ``None``
+
+    vgRemap: Optional[Dict[int, int]]
+        Maps the blend indices from the vertex group of the mod's blend to the blend indices for the vertex group of the boss :raw-html:`<br />`
+        If this value is ``None``, then the blend indices of the mod and the boss are one-to-one
+
+        The keys are the blend indices in the mod and the values are the blend indices in the boss :raw-html:`<br />` :raw-html:`<br />`
+
+        **Default**: ``None``
+
+    Attributes
+    ----------
+    name: :class:`str`
+        The default name for the type of mod
+
+    check: Union[:class:`str`, `Pattern`_, Callable[[:class:`str`], :class:`bool`]]
+        The specific check used to identify the .ini file belongs to the specific type of mod when checking arbitrary line in a .ini file
+
+    bossHash: :class:`str`
+        The hash for the Vertex Group Blend of the boss
+
+    aliases: Optional[List[:class:`str`]]
+        Other alternative names for the type of mod
+    """
+
+    def __init__(self, name: str, check: Union[str, Pattern, Callable[[str], bool]], bossHash:str, aliases: Optional[List[str]] = None, vgRemap: Optional[Dict[int, int]] = None ):
+        self.name = name
+        self.bossHash = bossHash
+
+        self.check = check
+        if (isinstance(check, str)):
+            self._check = lambda line: line == check
+        elif (callable(check)):
+            self._check = check
+        else:
+            self._check = lambda line: bool(check.search(line))
+        
+        if (aliases is None):
+            aliases = []
+        self.aliases = list(set(aliases))
+        
+        self._maxVgIndex = None
+        if (vgRemap is None):
+            vgRemap = {}
+        self.vgRemap = vgRemap
+
+    @property
+    def vgRemap(self) -> Dict[int, int]:
+        """
+        The mapping for remapping vertex group blend indices of the mod to the vertex group blend indices of the boss
+
+        :getter: Returns whether the .ini file has already been fixed
+        :setter: Sets a new mapping for remapping the indices
+        :type: Dict[:class:`int`, :class:`int`]
+        """
+
+        return self._vgRemap
+
+    @vgRemap.setter
+    def vgRemap(self, newVgRemap: Dict[int, int]):
+        self._vgRemap = newVgRemap
+        if (self._vgRemap):
+            self._maxVgIndex = max(list(self._vgRemap.keys()))
+        else:
+            self._maxVgIndex = None
+
+    @property
+    def maxVgIndex(self) -> Optional[int]:
+        """
+        The max vertex group blend index of the mod (key of the mapping) in :attr:`ModType.vgRemap`
+
+        :getter: Returns the following index
+        :type: Optional[:class:`int`]
+        """
+
+        return self._maxVgIndex
+
+    def isName(self, name: str) -> bool:
+        """
+        Determines whether a certain name matches with the names defined for this type of mod
+
+        Parameters
+        ----------
+        name: :class:`str`
+            The name being searched
+
+        Returns
+        -------
+        :class:`bool`
+            Whether the searched name matches with the names for this type of mod
+        """
+
+        name = name.lower()
+        if (self.name.lower() == name):
+            return True
+        
+        for alias in self.aliases:
+            if (alias.lower() == name):
+                return True
+
+        return False
+    
+    def isType(self, iniLine: str) -> bool:
+        """
+        Determines whether a line in the .ini file correponds with this mod type
+
+        Parameters
+        ----------
+        iniLine: :class:`str`
+            An arbitrary line in a .ini file
+
+        Returns
+        -------
+        :class:`bool`
+            Whether the line in the .ini file corresponds with this type of mod
+        """
+
+        return self._check(iniLine)
+    
+
+class ModTypes(Enum):
+    """
+    The supported types of mods that can be fixed
+
+    Attributes
+    ----------
+    Raiden: :class:`ModType`
+        **Raiden mods** :raw-html:`<br />`
+
+        Checks if the .ini file contains a section with the regex ``[TextureOverride.*(Raiden|Shogun).*Blend]``
+    """
+
+    Raiden = ModType("Raiden", re.compile(r"^\s*\[\s*TextureOverride.*(Raiden|Shogun)((?!RemapBlend).)*Blend.*\s*\]"), "fe5c0180",
+                     aliases = ["Ei", "RaidenEi", "Shogun", "RaidenShogun", "RaidenShotgun", "Shotgun", "CrydenShogun", "Cryden", "SmolEi"], 
+                     vgRemap = {0: 0, 1: 1, 2: 2, 3: 3, 4: 4, 5: 5, 6: 6, 7: 7, 8: 60, 9: 61, 10: 66, 11: 67,
+                                12: 8, 13: 9, 14: 10, 15: 11, 16: 12, 17: 13, 18: 14, 19: 15, 20: 16, 21: 17,
+                                22: 18, 23: 19, 24: 20, 25: 21, 26: 22, 27: 23, 28: 24, 29: 25, 30: 26, 31: 27,
+                                32: 28, 33: 29, 34: 30, 35: 31, 36: 32, 37: 33, 38: 34, 39: 35, 40: 36, 41: 37,
+                                42: 38, 43: 39, 44: 40, 45: 41, 46: 42, 47: 94, 48: 43, 49: 44, 50: 45, 51: 46,
+                                52: 47, 53: 48, 54: 49, 55: 50, 56: 51, 57: 52, 58: 53, 59: 54, 60: 55, 61: 56,
+                                62: 57, 63: 58, 64: 59, 65: 114, 66: 116, 67: 115, 68: 117, 69: 74, 70: 62, 71: 64,
+                                72: 106, 73: 108, 74: 110, 75: 75, 76: 77, 77: 79, 78: 87, 79: 89, 80: 91, 81: 95,
+                                82: 97, 83: 99, 84: 81, 85: 83, 86: 85, 87: 68, 88: 70, 89: 72, 90: 104, 91: 112,
+                                92: 93, 93: 63, 94: 65, 95: 107, 96: 109, 97: 111, 98: 76, 99: 78, 100: 80, 101: 88,
+                                102: 90, 103: 92, 104: 96, 105: 98, 106: 100, 107: 82, 108: 84, 109: 86, 110: 69,
+                                111: 71, 112: 73, 113: 105, 114: 113, 115: 101, 116: 102, 117: 103})
+    
+    @classmethod
+    def getAll(cls) -> Set[ModType]:
+        """
+        Retrieves a set of all the mod types available
+
+        Returns
+        -------
+        Set[:class:`ModType`]
+            All the available mod types
+        """
+
+        result = set()
+        for modTypeEnum in cls:
+            result.add(modTypeEnum.value)
+        return result
+    
+    @classmethod
+    def search(cls, name: str):
+        """
+        Searches a mod type based off the provided name
+
+        Parameters
+        ----------
+        name: :class:`str`
+            The name of the mod to search for
+
+        Returns
+        -------
+        Optional[:class:`ModType`]
+            The found mod type based off the provided name
+        """
+
+        result = None
+        for modTypeEnum in cls:
+            modType = modTypeEnum.value
+            if (modType.isName(name)):
+                result = modType
+                break
+        
+        return result
+    
+    @classmethod
+    def getHelpStr(cls) -> str:
+        result = ""
+        helpHeading = Heading("supported types of mods", 15)
+        result += f"{helpHeading.open()}\n\nThe names/aliases for the mod types are not case sensitive\n\n"
+
+        modTypeHelpTxt = []
+        for modTypeEnum in cls:
+            modType = modTypeEnum.value
+            modTypeHeading = Heading(modType.name, 8, "-")
+
+            currentHelpStr = f"{modTypeHeading.open()}"
+            currentHelpStr += f"\n\nname: {modType.name}"
+            
+            if (modType.aliases):
+                aliasStr = ", ".join(modType.aliases)
+                currentHelpStr += f"\naliases: {aliasStr}"
+
+            if (isinstance(modType.check, str)):
+                currentHelpStr += f"\ndescription: check if the .ini file contains the section named, '{modType.check}'"
+            elif (not callable(modType.check)):
+                currentHelpStr += f"\ndescription: check if the .ini file contains a section matching the regex, {modType.check.pattern}"
+
+            currentHelpStr += f"\n\n{modTypeHeading.close()}"
+            modTypeHelpTxt.append(currentHelpStr)
+
+        modTypeHelpTxt = "\n".join(modTypeHelpTxt)
+        result += f"{modTypeHelpTxt}\n\n{helpHeading.close()}"
+        return result
+
+argParser.epilog = ModTypes.getHelpStr()
+
+
 # IfTemplate: Data class for the if..else template of the .ini file
 class IfTemplate():
     """
     Data for storing information about a `section`_ in a .ini file
 
     :raw-html:`<br />`
 
@@ -1463,14 +1756,21 @@
 
             **Default**: ``None``
 
         postProcessor: Optional[Callable[[Union[:class:`str`, Dict[str, Any]]], Any]]
             A function that performs any post-processing on the found part that meets the required condition :raw-html:`<br />` :raw-html:`<br />`
         
             **Default**: ``None``
+
+        Returns
+        -------
+        Dict[:class:`int`, Any]
+            The filtered parts that meet the search condition :raw-html:`<br />` :raw-html:`<br />`
+
+            The keys are the index locations of the parts and the values are the found parts
         """
 
         result = {}
         if (pred is None):
             pred = lambda part: True
 
         if (postProcessor is None):
@@ -1514,41 +1814,38 @@
         The logger to print messages if necessary
 
     txt: :class:`str`
         Used as the text content of the .ini file if :attr:`IniFile.file` is set to ``None`` :raw-html:`<br />` :raw-html:`<br />`
 
         **Default**: ""
 
-    mustBeRaiden: :class:`bool`
-        Whether the .ini file has to be used for a Raiden mod :raw-html:`<br />` :raw-html:`<br />`
+    modTypes: Optional[Set[:class:`ModType`]]
+        The types of mods that the .ini file should belong to :raw-html:`<br />` :raw-html:`<br />`
 
-        **Default**: ``True``
+        **Default**: ``None``
+
+    defaultModType: Optional[:class:`ModType`]
+        The type of mod to use if the .ini file has an unidentified mod type :raw-html:`<br />` :raw-html:`<br />`
+        If this value is ``None``, then will skip the .ini file with an unidentified mod type :raw-html:`<br />` :raw-html:`<br />`
+
+        **Default**: ``None``
 
     Attributes
     ----------
     file: :class:`str`
         The file path to the .ini file
 
     _parser: `ConfigParser`_
         Parser used to parse very basic cases in a .ini file
 
-    _fileLines: List[:class:`str`]
-        The file lines read from the .ini file
-
-    _fileLinesRead: :class:`bool`
-        Whether the file for the .ini file has been read
-
-    _isRaidenFixed: :class:`bool`
-        Whether the .ini file has already been fixed
-
-    _isRaidenIni: :class:`bool`
-        Whether the .ini file is used for a Raiden mod
+    modTypes: Optional[Set[:class:`ModType`]]
+        The types of mods that the .ini file should belong to
 
-    mustBeRaiden: :class:`bool`
-        Whether the .ini file has to be used for a Raiden mod :raw-html:`<br />` :raw-html:`<br />`
+    defaultModType: Optional[:class:`ModType`]
+        The type of mod to use if the .ini file has an unidentified mod type
 
     _textureOverrideBlendRoot: Optional[:class:`str`]
         The name for the `section`_ containing the keywords: ``[.*TextureOverride.*Blend.*]``
 
     _sectionIfTemplates: Dict[:class:`str`, :class:`IfTemplate`]
         All the `sections`_ in the .ini file that can be parsed into an :class:`IfTemplate`
 
@@ -1622,62 +1919,69 @@
             
             .. code-block:: python
                 :linenos:
 
                 list(remapBlendModelsDict.values())
     """
 
+    ModTypeNameReplaceStr = "{{modTypeName}}"
+    ModTypeBossNameReplaceStr = "{{modTypeBossName}}"
+    Credit = f'\n; {ModTypeBossNameReplaceStr}fixed by NK#1321 if you used it for fix your {ModTypeNameReplaceStr}mods pls give credit for "Nhok0169"\n; Thank nguen#2011 SilentNightSound#7430 HazrateGolabi#1364 and Albert Gold#2696 for support'
 
-    Credit = f'\n; Raiden boss fixed by NK#1321 if you used it for fix your raiden pls give credit for "Nhok0169"\n; Thank nguen#2011 SilentNightSound#7430 HazrateGolabi#1364 and Albert Gold#2696 for support'
-
-    _fixHeader = "; --------------- Raiden Boss Fix -----------------"
-    _fixFooter = "; -------------------------------------------------"
+    _defaultHeading = Heading(".*Boss Fix", 15, "-")
 
     Hash = "hash"
     Vb1 = "vb1"
     Handling = "handling"
     Draw = "draw"
     Resource = "Resource"
     Blend = "Blend"
     Run = "run"
     RemapBlend = f"Remap{Blend}"
 
     # -- regex strings ---
 
-    _textureOverrideRaidenBlendPatternStr = r"\[\s*TextureOverride.*(Raiden|Shogun).*" + Blend + r"\s*\]"
-    _textureOverrideBlendPatternStr = r"\[\s*TextureOverride.*" + Blend + r".*\s*\]"
-    _fixedTextureOverrideBlendPatternStr = r"\[\s*TextureOverride.*" + RemapBlend + r"\s*\]"
+    _textureOverrideBlendPatternStr = r"^\s*\[\s*TextureOverride.*" + Blend + r".*\s*\]"
+    _fixedTextureOverrideBlendPatternStr = r"^\s*\[\s*TextureOverride.*" + RemapBlend + r".*\s*\]"
 
     # --------------------
     # -- regex objects ---
-    _sectionPattern = re.compile(r"\[.*\]")
-    _textureOverrideRaidenBlendPattern  = re.compile(_textureOverrideRaidenBlendPatternStr)
+    _sectionPattern = re.compile(r"^\s*\[.*\]")
     _textureOverrideBlendPattern = re.compile(_textureOverrideBlendPatternStr)
     _fixedTextureOverrideBlendPattern = re.compile(_fixedTextureOverrideBlendPatternStr)
-    _fixRemovalPattern = re.compile(f"{_fixHeader}(.|\n)*{_fixFooter}")
-    _removalPattern = re.compile(f"({_fixedTextureOverrideBlendPatternStr})|(\[.*" + RemapBlend + r".*\])")
+    _fixRemovalPattern = re.compile(f"; {_defaultHeading.open()}(.|\n)*; {_defaultHeading.close()[:-2]}(-)*")
+    _removalPattern = re.compile(f"^\s*\[.*" + RemapBlend + r".*\]")
 
     # -------------------
 
     _ifStructurePattern = re.compile(r"\s*(endif|if|else)")
 
-    def __init__(self, file: Optional[str] = None, logger: Optional[Logger] = None, txt: str = "", mustBeRaiden: bool = True):
+    def __init__(self, file: Optional[str] = None, logger: Optional[Logger] = None, txt: str = "", modTypes: Optional[Set[ModType]] = None, defaultModType: Optional[ModType] = None):
         super().__init__(logger = logger)
         self.file = file
-        self._parser = configparser.ConfigParser()
+        self._parser = configparser.ConfigParser(dict_type = ConfigParserDict, strict = False)
 
         self._fileLines = []
+        self._fileTxt = ""
         self._fileLinesRead = False
         self._setupFileLines(fileTxt = txt)
 
-        self._isRaidenFixed = False
-        self._isRaidenIni = False
-        self.mustBeRaiden = mustBeRaiden
+        self._isFixed = False
+        self._type = None
+        self._isModIni = False
+
+        if (modTypes is None):
+            modTypes = set()
+        self.defaultModType = defaultModType
+        self.modTypes = modTypes
+        self._heading = self._defaultHeading.copy()
+        self._heading.title = None
 
         self._textureOverrideBlendRoot: Optional[str] = None
+        self._textureOverrideBlendSectionName: Optional[str] = None
         self._sectionIfTemplates: Dict[str, IfTemplate] = {}
         self._resourceBlends: Dict[str, IfTemplate] = {}
 
         self._blendCommands: Dict[str, IfTemplate] = {}
         self._blendCommandsRemapNames: Dict[str, str] = {}
         self._blendCommandsTuples: List[Tuple[str, IfTemplate]] = []
 
@@ -1685,104 +1989,228 @@
         self._resourceCommandsRemapNames:Dict[str, str] = {}
         self._resourceCommandsTuples: List[Tuple[str, IfTemplate]] = []
 
         self.remapBlendModelsDict: Dict[str, RemapBlendModel] = {}
         self.remapBlendModels: List[RemapBlendModel] = []
 
     @property
-    def isRaidenFixed(self):
+    def isFixed(self) -> bool:
         """
         Whether the .ini file has already been fixed
 
         :getter: Returns whether the .ini file has already been fixed
         :type: :class:`bool`
         """
 
-        return self._isRaidenFixed
+        return self._isFixed
     
     @property
-    def isRaidenIni(self):
+    def type(self) -> Optional[ModType]:
+        """
+        The type of mod the .ini file belongs to
+
+        :getter: Returns the type of mod the .ini file belongs to
+        :type: Optional[:class:`ModType`]
         """
-        Whether the .ini file is a for a Raiden mod
 
-        :getter: Returns whether the .ini file is a for a Raiden mod
+        return self._type
+    
+    @property
+    def isModIni(self) -> bool:
+        """
+        Whether the .ini file belongs to a mod
+
+        :getter: Returns whether the .ini file belongs to a mod
         :type: :class:`bool`
         """
 
-        return self._isRaidenIni
+        return self._isModIni
+    
+    @property
+    def fileLinesRead(self) -> bool:
+        """
+        Whether the .ini file has been read
 
-    def clearRead(self):
+        :getter: Determines whether the .ini file has been read
+        :type: :class:`bool`
         """
-        Clears all the saved text read in from the .ini file
+
+        return self._fileLinesRead
+    
+    @property
+    def fileTxt(self) -> str:
         """
+        The text content of the .ini file
 
-        self._fileLines = []
-        self._fileLinesRead = False
-        self._isRaidenFixed = False
+        :getter: Returns the content of the .ini file
+        :setter: Reads the new value for both the text content of the .ini file and the text lines of the .ini file 
+        :type: :class:`str`
+        """
+
+        return self._fileTxt
+    
+    @fileTxt.setter
+    def fileTxt(self, newFileTxt: str):
+        self._fileTxt = newFileTxt
+
+        self._fileLines = self._fileTxt.split("\n")
+
+        if (self._fileTxt):
+            fileLinesLen = len(self._fileLines)
+            for i in range(fileLinesLen):
+                if (i < fileLinesLen - 1):
+                    self._fileLines[i] += "\n"
+        else:
+            self._fileLines = []
+
+        self._fileLinesRead = True
+        self._isFixed = False
+        self._textureOverrideBlendRoot = None
+        self._textureOverrideBlendSectionName = None
+
+    @property
+    def fileLines(self) -> List[str]:
+        """
+        The text lines of the .ini file :raw-html:`<br />` :raw-html:`<br />`
+
+        .. note::
+            For the setter, each line must end with a newline character (same behaviour as `readLines`_)
+
+        :getter: Returns the text lines of the .ini file
+        :setter: Reads the new value for both the text lines of the .ini file and the text content of the .ini file
+        :type: List[:class:`str`]
+        """
+
+        return self._fileLines
+    
+    @fileLines.setter
+    def fileLines(self, newFileLines: List[str]):
+        self._fileLines = newFileLines
+        self._fileTxt = "".join(self._fileLines)
+
+        self._fileLinesRead = True
+        self._isFixed = False
+        self._textureOverrideBlendRoot = None
+        self._textureOverrideBlendSectionName = None
+
+    def clearRead(self, eraseSourceTxt: bool = False):
+        """
+        Clears the saved text read in from the .ini file
+
+        .. note::
+            If :attr:`IniFile.file` is set to ``None``, then the default run of this function
+            with the argument ``eraseSourceTxt`` set to ``False`` will have no effect since the provided text from :attr:`IniFile._fileTxt` is the only source of data for the :class:`IniFile`
+
+            If you also want to clear the above source text data, then run this function with the ``eraseSourceTxt`` argument set to ``True``
+
+        Parameters
+        ----------
+        eraseSourceTxt: :class:`bool`
+            Whether to erase the only data source for this class if :attr:`IniFile.file` is set to ``None``, see the note above for more info :raw-html:`<br />` :raw-html:`<br />`
+
+            **Default**: ``False``
+        """
+
+        if (self.file is not None or eraseSourceTxt):
+            self._fileLines = []
+            self._fileTxt = ""
+            self._fileLinesRead = False
+
+            self._isFixed = False
+            self._textureOverrideBlendRoot = None
+            self._textureOverrideBlendSectionName = None
+
+    def clear(self, eraseSourceTxt: bool = False):
+        """
+        Clears all the saved data for the .ini file
+
+        .. note::
+            Please see the note at :meth:`IniFile.clearRead`
+
+        Parameters
+        ----------
+        eraseSourceTxt: :class:`bool`
+            Whether to erase the only data source for this class if :attr:`IniFile.file` is set to ``None``, see the note at :meth:`IniFile.clearRead` for more info :raw-html:`<br />` :raw-html:`<br />`
+
+            **Default**: ``False``
+        """
+
+        self.clearRead(eraseSourceTxt = eraseSourceTxt)
+        self._type = None
+        self._isModIni = False
+        self._heading = self._defaultHeading.copy()
+        self._heading.title = None
+
+        self._sectionIfTemplates = {}
+        self._resourceBlends = {}
+
+        self._blendCommands = {}
+        self._blendCommandsRemapNames = {}
+        self._blendCommandsTuples = []
+
+        self._resourceCommands = {}
+        self._resourceCommandsRemapNames = {}
+        self._resourceCommandsTuples = []
+
+        self.remapBlendModelsDict = {}
+        self.remapBlendModels = []
 
     def read(self) -> str:
         """
-        Reads the .ini file
+        Reads the .ini file :raw-html:`<br />` :raw-html:`<br />`
+
+        If :attr:`IniFile.file` is set to ``None``, then will read the existing value from :attr:`IniFile.fileTxt`
 
         Returns
         -------
         :class:`str`
             The text content of the .ini file
         """
 
-        result = ""
-        result = FileService.read(self.file, "r", lambda filePtr: filePtr.read())
-        return result
+        if (self.file is not None):
+            self.fileTxt = FileService.read(self.file, "r", lambda filePtr: filePtr.read())
+        return self._fileTxt
     
     def write(self) -> str:
         """
         Writes back into the .ini files based off the content in :attr:`IniFile._fileLines`
 
         Returns
         -------
         :class:`str`
             The text that is written to the .ini file
         """
 
-        txtToWrite = "".join(self._fileLines)
-
         if (self.file is None):
-            return txtToWrite
+            return self._fileTxt
 
         with open(self.file, "w", encoding = IniFileEncoding) as f:
-            f.write(txtToWrite)
+            f.write(self._fileTxt)
 
-        return txtToWrite
+        return self._fileTxt
 
     def _setupFileLines(self, fileTxt: str = ""):
-        if (self.file is not None):
-            return
-        
-        self._fileLines = fileTxt.split("\n")
-
-        fileLinesLen = len(self._fileLines)
-        for i in range(fileLinesLen):
-            if (i < fileLinesLen - 1):
-                self._fileLines[i] += "\n"
-
-        self._fileLinesRead = True
-
+        if (self.file is None):
+            self.fileTxt = fileTxt
+            self._fileLinesRead = True
 
-    def getFileLines(self) -> List[str]:
+    def readFileLines(self) -> List[str]:
         """
-        Reads each line in the .ini file
+        Reads each line in the .ini file :raw-html:`<br />` :raw-html:`<br />`
+
+        If :attr:`IniFile.file` is set to ``None``, then will read the existing value from :attr:`IniFile.fileLines`
 
         Returns
         -------
         List[:class:`str`]
-            All the lines of the .ini file
+            All the lines read from the .ini file
         """
 
-        self._fileLines = FileService.read(self.file, "r", lambda filePtr: filePtr.readlines())
-        self._fileLinesRead = True
+        if (self.file is not None):
+            self.fileLines = FileService.read(self.file, "r", lambda filePtr: filePtr.readlines())
         return self._fileLines
 
     def _readLines(func):
         """
         Decorator to read all the lines in the .ini file first before running a certain function
 
         All the file lines will be saved in :attr:`IniFile._fileLines`
@@ -1796,82 +2224,84 @@
             def printLines(self):
                 for line in self._fileLines:
                     print(f"LINE: {line}")
         """
 
         def readLinesWrapper(self, *args, **kwargs):
             if (not self._fileLinesRead):
-                self.getFileLines()
+                self.readFileLines()
             return func(self, *args, **kwargs)
         return readLinesWrapper
     
-    def checkRaidenIni(self, mustBeRaiden: Optional[bool] = None) -> bool:
+    def checkIsMod(self) -> bool:
         """
-        Reads the entire .ini file and checks whether the .ini file is a Raiden mod that needs to be fixed
+        Reads the entire .ini file and checks whether the .ini file belongs to a mod
 
         .. note::
-            If the .ini file has already been parsed (eg. calling :meth:`IniFile.checkRaidenIni` or :meth:`IniFile.parse`), then
-
-            you only need to read the :attr:`IniFile._isRaidenIni`
+            If the .ini file has already been parsed (eg. calling :meth:`IniFile.checkModType` or :meth:`IniFile.parse`), then
 
-        Parameters
-        ----------
-        mustBeRaiden: Optional[:class:`bool`]
-            Whether the .ini file being checked has to be a Raiden mod
+            you only need to read :meth:`IniFile.isModIni`
 
         Returns
         -------
         :class:`bool`
-            Whether the .ini file is a .ini file that needs to be fixed
+            Whether the .ini file is a .ini file that belongs to some mod
         """
-
-        postProcessor = lambda startInd, endInd, fileLines, sectionName, srcTxt: sectionName
-        textureOverridePattern = self._textureOverrideRaidenBlendPattern
-        if ((mustBeRaiden is not None and not mustBeRaiden) or (mustBeRaiden is None and not self.mustBeRaiden)):
-            textureOverridePattern = self._textureOverrideBlendPattern
-
-        textureOverrideBlendSections = self.getSectionOptions(textureOverridePattern , postProcessor = postProcessor)
-
-        self._isRaidenIni = bool(textureOverrideBlendSections)
-        if (self._isRaidenIni):
-            self._textureOverrideBlendRoot = DictTools.getFirstKey(textureOverrideBlendSections)
-
-        return self._isRaidenIni
+        
+        self.clearRead()
+        section = lambda line: False
+        self.getSectionOptions(section, postProcessor = lambda startInd, endInd, fileLines, sectionName, srcTxt: "")
+        return self._isModIni
     
-    def _checkRaidenIni(self, line: str):
+    def _checkModType(self, line: str):
         """
-        Checks if a line of text contains the keywords to identify whether the .ini file is a Raiden mod :raw-html:`<br />` :raw-html:`<br />`
+        Checks if a line of text contains the keywords to identify whether the .ini file belongs to the types of mods in :attr:`IniFile.modTypes` :raw-html:`<br />` :raw-html:`<br />`
 
-        * If :attr:`IniFile.mustBeRaiden` is ``True``, then will see if the line matches with the regex, ``[.*TextureOverride.*(Raiden|Shogun).*Blend.*]``
+        * If :attr:`IniFile.modTypes` is not empty, then will find the first :class:`ModType` that where the line makes :meth:`ModType.isType` return ``True``
         * Otherwise, will see if the line matches with the regex, ``[.*TextureOverride.*Blend.*]`` 
 
         Parameters
         ----------
         line: :class:`str`
             The text to check
         """
 
-        if (self._textureOverrideBlendRoot is None and 
-            ((self.mustBeRaiden and self._textureOverrideRaidenBlendPattern.match(line)) or 
-             (not self.mustBeRaiden and self._textureOverrideBlendPattern.match(line)))):
+        if (not self._isModIni and self.defaultModType is not None and self._textureOverrideBlendSectionName is None and 
+            self._textureOverrideBlendPattern.search(line)):
+            self._isModIni = True
+            self._textureOverrideBlendSectionName = self._getSectionName(line)
+
+        if (self._textureOverrideBlendRoot is not None):
+            return
+        
+        if (not self.modTypes and self._textureOverrideBlendPattern.search(line)):
             self._textureOverrideBlendRoot = self._getSectionName(line)
-            self._isRaidenIni = True
+            self._isModIni = True
+            return
+
+        for modType in self.modTypes:
+            if (modType.isType(line)):
+                self._textureOverrideBlendRoot = self._getSectionName(line)
+                self._type = modType
+                self._heading.title = None
+                self._isModIni = True
+                break
 
-    def _checkRaidenFixed(self, line: str):
+    def _checkFixed(self, line: str):
         """
         Checks if a line of text matches the regex, ``[.*TextureOverride.*RemapBlend.*]`` ,to identify whether the .ini file has been fixed
 
         Parameters
         ----------
         line: :class:`str`
             The line of text to check
         """
 
-        if (not self._isRaidenFixed and self._fixedTextureOverrideBlendPattern.match(line)):
-            self._isRaidenFixed = True
+        if (not self._isFixed and self._fixedTextureOverrideBlendPattern.search(line)):
+            self._isFixed = True
 
     def _parseSection(self, sectionName: str, srcTxt: str, save: Optional[Dict[str, Any]] = None) -> Optional[Dict[str, str]]:
         """
         Regularly parses the key-value pairs of a certain `section`_
 
         The function parses uses `ConfigParser`_ to parse the `section`_.
 
@@ -1895,38 +2325,48 @@
         Optional[Dict[:class:`str`, :class:`str`]]
             The result from parsing the `section`_
 
             .. note:: 
                 If `ConfigParser`_ is unable to parse the section, then ``None`` is returned
         """
 
+        result = None
         try:
             self._parser.read_string(srcTxt)
-        except:
-            return None
-
-        result = dict(self._parser[sectionName])
+            result = dict(self._parser[sectionName])
+        except Exception:
+            return result
 
         try:
             save[sectionName] = result
         except TypeError:
             pass
 
         return result
     
     def _getSectionName(self, line: str) -> str:
-        currentSectionName = line.strip().replace("]", "")
-        currentSectionName = currentSectionName.replace("[", "")
-        return currentSectionName
+        currentSectionName = line
+        rightPos = currentSectionName.rfind("]")
+        leftPos = currentSectionName.find("[")
+
+        if (rightPos > -1 and leftPos > -1):
+            currentSectionName = currentSectionName[leftPos + 1:rightPos]
+        elif (rightPos > -1):
+            currentSectionName = currentSectionName[:rightPos]
+        elif (leftPos > -1):
+            currentSectionName = currentSectionName[leftPos + 1:]
+
+        return currentSectionName.strip()
 
     # retrieves the key-value pairs of a section in the .ini file. Manually parsed the file since ConfigParser
     #   errors out on conditional statements in .ini file for mods. Could later inherit from the parser (RawConfigParser) 
     #   to custom deal with conditionals
     @_readLines
-    def getSectionOptions(self, section: Union[str, Pattern, Callable[[str], bool]], postProcessor: Optional[Callable[[int, int, List[str], str, str], Any]] = None) -> Dict[str, Any]:
+    def getSectionOptions(self, section: Union[str, Pattern, Callable[[str], bool]], postProcessor: Optional[Callable[[int, int, List[str], str, str], Any]] = None, 
+                          handleDuplicateFunc: Optional[Callable[[List[Any]], Any]] = None) -> Dict[str, Any]:
         """
         Reads the entire .ini file for a certain type of `section`_
 
         Parameters
         ----------
         section: Union[:class:`str`, `Pattern`_, Callable[[:class:`str`], :class:`bool`]]
             The type of section to find
@@ -1944,70 +2384,100 @@
             #. The ending line index of the `section`_ in the .ini file
             #. All the file lines read from the .ini file
             #. The name of the `section`_ found
             #. The entire text for the `section`_ :raw-html:`<br />` :raw-html:`<br />`
 
             **Default**: `None`
 
+        handleDuplicateFunc: Optional[Callable[List[Any], Any]]
+            Function to used to handle the case of multiple sections names :raw-html:`<br />` :raw-html:`<br />`
+
+            If this value is set to ``None``, will keep all sections with the same names
+
+            .. note::
+                For this case, GIMI only keeps the first instance of all sections with same names
+
+            :raw-html:`<br />`
+
+            **Default**: ``None``
+
         Returns
         -------
         Dict[:class:`str`, Any]
             The resultant `sections`_ found
 
-            The keys are the names of the `sections`_ found and the values are the content for the `section`_
+            The keys are the names of the `sections`_ found and the values are the content for the `section`_,
         """
 
         sectionFilter = None
         if (isinstance(section, str)):
             sectionFilter = lambda line: line == section
         elif callable(section):
             sectionFilter = section
         else:
-            sectionFilter = lambda line: section.match(line)
+            sectionFilter = lambda line: section.search(line)
 
         if (postProcessor is None):
             postProcessor = lambda startInd, endInd, fileLines, sectionName, srcTxt: self._parseSection(sectionName, srcTxt)
 
         result = {}
         currentSectionName = None
         currentSectionToParse = None
         currentSectionStartInd = -1
 
         fileLinesLen = len(self._fileLines)
 
         for i in range(fileLinesLen):
             line = self._fileLines[i]
-            self._checkRaidenFixed(line)
-            self._checkRaidenIni(line)
-
-            if (sectionFilter(line)):
-                currentSectionToParse = f"{line}"
-                currentSectionName = self._getSectionName(currentSectionToParse)
-                currentSectionStartInd = i
-                continue
-
-            if (currentSectionToParse is None):
-                continue
+            self._checkFixed(line)
+            self._checkModType(line)
 
-            if (line.strip() == ""):
+            # process the resultant section
+            if (currentSectionToParse is not None and self._sectionPattern.search(line)):
                 currentResult = postProcessor(currentSectionStartInd, i, self._fileLines, currentSectionName, currentSectionToParse)
                 if (currentResult is None):
                     continue
 
-                result[currentSectionName] = currentResult
+                # whether to keep sections with the same name
+                try:
+                    result[currentSectionName]
+                except KeyError:
+                    result[currentSectionName] = [currentResult]
+                else:
+                    result[currentSectionName].append(currentResult)
 
                 currentSectionToParse = None
                 currentSectionName = None
                 currentSectionStartInd = -1
-            else:
+
+            elif (currentSectionToParse is not None):
                 currentSectionToParse += f"{line}"
 
+            # keep track of the found section
+            if (sectionFilter(line)):
+                currentSectionToParse = f"{line}"
+                currentSectionName = self._getSectionName(currentSectionToParse)
+                currentSectionStartInd = i
+
         # get any remainder section
         if (currentSectionToParse is not None):
-            result[currentSectionName] = postProcessor(currentSectionStartInd, fileLinesLen, self._fileLines, currentSectionName, currentSectionToParse)
+            currentResult = postProcessor(currentSectionStartInd, fileLinesLen, self._fileLines, currentSectionName, currentSectionToParse)
+            try:
+                result[currentSectionName]
+            except:
+                result[currentSectionName] = [currentResult]
+            else:
+                result[currentSectionName].append(currentResult)
+
+        if (handleDuplicateFunc is None):
+            return result
+
+        # handle the duplicate sections with the same names
+        for sectionName in result:
+            result[sectionName] = handleDuplicateFunc(result[sectionName])
 
         return result
 
     def _removeSection(self, startInd: int, endInd: int, fileLines: List[str], sectionName: str, srcTxt: str) -> Tuple[int, int]:
         """
         Retrieves the starting line index and ending line index of where to remove a certain `section`_ from the read lines of the .ini file
 
@@ -2030,38 +2500,44 @@
 
         Returns
         -------
         Tuple[:class:`int`, :class:`int`]
             The starting line index and the ending line index of the `section`_ to remove
         """
 
-        if (endInd >= len(fileLines)):
-            return (startInd, endInd)
-        return (startInd, endInd + 1)
+        fileLinesLen = len(fileLines)
+        if (endInd > fileLinesLen):
+            endInd = fileLinesLen
+
+        if (startInd > fileLinesLen):
+            startInd = fileLinesLen
+
+        return (startInd, endInd)
     
     def removeSectionOptions(self, section: Union[str, Pattern, Callable[[str], bool]]):
         """
         Removes a certain type of `section`_ from the .ini file
 
         Parameters
         ----------
         section: Union[:class:`str`, `Pattern`_, Callable[[:class:`str`], :class:`bool`]]
             The type of `section`_ to remove
         """
 
         rangesToRemove = self.getSectionOptions(section, postProcessor = self._removeSection)
 
         for sectionName in rangesToRemove:
-            range = rangesToRemove[sectionName]
-            startInd = range[0]
-            endInd = range[1]
+            ranges = rangesToRemove[sectionName]
+            for range in ranges:
+                startInd = range[0]
+                endInd = range[1]
 
-            self._fileLines[startInd:endInd] =  [0] * (endInd - startInd)
+                self._fileLines[startInd:endInd] =  [0] * (endInd - startInd)
 
-        self._fileLines = list(filter(lambda line: line != 0, self._fileLines))
+        self.fileLines = list(filter(lambda line: line != 0, self._fileLines))
 
     def _processIfTemplate(self, startInd: int, endInd: int, fileLines: List[str], sectionName: str, srcTxt: str) -> IfTemplate:
         """
         Parses a `section`_ in the .ini file as an :class:`IfTemplate`
 
         .. note::
             See :class:`IfTemplate` to see how we define an 'IfTemplate'
@@ -2133,72 +2609,116 @@
         calledSubCommands = result.find(pred = lambda part: isinstance(part, dict) and self._isIfTemplateSubCommand(part), postProcessor = self._getIfTemplateSubCommand)
         result.calledSubCommands = calledSubCommands
 
         return result
                 
     
     @classmethod
-    def getMergedResourceIndex(cls, mergedResourceName: str) -> str:
+    def getMergedResourceIndex(cls, mergedResourceName: str) -> Optional[int]:
         """
         Retrieves the index number of a resource created by GIMI's ``genshin_merge_mods.py`` script
 
         Examples
         --------
         >>> IniFile.getMergedResourceIndex("ResourceCuteLittleEiBlend.8")
         8
 
+
+        >>> IniFile.getMergedResourceIndex("ResourceCuteLittleEiBlend.Score.-100")
+        -100
+
+
+        >>> IniFile.getMergedResourceIndex("ResourceCuteLittleEiBlend.UnitTests")
+        None
+
+
+        >>> IniFile.getMergedResourceIndex("ResourceCuteLittleEiBlend")
+        None
+
         Parameters
         ----------
         mergedResourceName: :class:`str`
             The name of the `section`_
 
         Returns
         -------
-        :class:`str`
-            The index for the resource `section`_
+        Optional[:class:`int`]
+            The index for the resource `section`_, if found and the index is an integer
         """
-        
-        return mergedResourceName.rsplit(".", 1)[-1]
+        result = None
+
+        try:
+            result = int(mergedResourceName.rsplit(".", 1)[-1])
+        except:
+            pass
+            
+        return result
     
-    def _getResourceSortKey(self, resourceTuple: Tuple[str, Any]) -> int:
+    def _compareResources(self, resourceTuple1: Tuple[str, Optional[int]], resourceTuple2: Tuple[str, Optional[int]]) -> int:
         """
-        Retrieves the index number of a resource created by GIMI's ``genshin_merge_mods.py`` script as an integer
+        Compare function used for sorting resources :raw-html:`<br />` :raw-html:`<br />`
 
-        .. note::
-            See :meth:`IniFile.getMergedResourceIndex` for more info
+        The order for sorting is the resources is:
+        
+        #. Resources that do are not suffixed by an index number
+        #. Resource that are suffixed by an index number (see :meth:`IniFile.getMergedResourceIndex` for more info)
 
         Parameters
         ----------
-        resourceTuple: Tuple[:class:`str`, Any]
-            The name of the resource section and its content
+        resourceTuple1: Tuple[:class:`str`, Optional[:class:`int`]]
+            Data for the first resource in the compare function, contains:
+
+            * Name of the resource
+            * The index for the resource
+
+        resourceTuple2: Tuple[:class:`str`, Optional[:class:`int`]]
+            Data for the second resource in the compare function, contains:
+
+            * Name of the resource
+            * The index for the resource
 
         Returns
         -------
         :class:`int`
-            The index for the resource section
+            The result for a typical compare function used in sorting
+
+            * returns -1 if ``resourceTuple1`` should come before ``resourceTuple2``
+            * returns 1 if ``resourceTuple1`` should come after ``resourceTuple2``
+            * returns 0 if ``resourceTuple1`` is equal to ``resourceTuple2`` 
         """
 
-        result = -1
-        try:
-            result = int(self.getMergedResourceIndex(resourceTuple[0]))
-        except:
-            pass
+        resourceKey1 = resourceTuple1[1]
+        resourceKey2 = resourceTuple2[1]
+        resource1MissingIndex = resourceKey1 is None
+        resource2MissingIndex = resourceKey2 is None
 
-        return result
+        if (resource1MissingIndex):
+            resourceKey1 = resourceTuple1[0]
+        
+        if (resource2MissingIndex):
+            resourceKey2 = resourceTuple2[0]
+
+        if ((resource1MissingIndex == resource2MissingIndex and resourceKey1 < resourceKey2) or (resource1MissingIndex and not resource2MissingIndex)):
+            return -1
+        elif ((resource1MissingIndex == resource2MissingIndex and resourceKey1 > resourceKey2) or (not resource1MissingIndex and resource2MissingIndex)):
+            return 1
+        
+        return 0
 
     # Disabling the OLD ini
     def disIni(self):
         """
         Disables the .ini file
 
         .. note::
             For more info, see :meth:`FileService.disableFile`
         """
 
-        FileService.disableFile(self.file)
+        if (self.file is not None):
+            FileService.disableFile(self.file)
 
     @classmethod
     def getFixedBlendFile(cls, blendFile: str) -> str:
         """
         Retrieves the file path for the fixed RemapBlend.buf file
 
         Parameters
@@ -2208,37 +2728,103 @@
 
         Returns
         -------
         :class:`str`
             The file path of the fixed RemapBlend.buf file
         """
 
-        blendFile = blendFile.rsplit(".", 1)[0]
         blendFolder = os.path.dirname(blendFile)
         blendBaseName = os.path.basename(blendFile)
+        blendBaseName = blendBaseName.rsplit(".", 1)[0]
         
         return os.path.join(blendFolder, f"{cls.getRemapName(blendBaseName)}.buf")
+    
+    def getFixModTypeName(self) -> Optional[str]:
+        """
+        Retrieves the name of the type of mod corresponding to the .ini file to be used for the comment of the fix
 
-    @classmethod
-    def getFixHeader(cls) -> str:
+        Returns
+        -------
+        Optional[:class:`str`]
+            The name for the type of mod corresponding to the .ini file
         """
-        Retrieves the header text used to identify a code section has been changed by this fix
-        in the .ini file        
+        if (self._type is None):
+            return None
+        return self._type.name.replace("\n", "").replace("\t", "")
+    
+    def getFixModTypeHeadingname(self):
+        """
+        Retrieves the name of the type of mod corresponding to the .ini file to be used in the header/footer divider comment of the fix
+
+        Returns
+        -------
+        Optional[:class:`str`]
+            The name for the type of mod to be displayed in the header/footer divider comment
+        """
+
+        modTypeName = self.getFixModTypeName()
+        if (modTypeName is None):
+            modTypeName = "GI"
+
+        if (modTypeName is not None and modTypeName):
+            modTypeName += " "
+
+        return modTypeName
+
+    def getFixHeader(self) -> str:
         """
+        Retrieves the header text used to identify a code section has been changed by this fix
+        in the .ini file
 
-        return cls._fixHeader
+        Returns
+        -------
+        :class:`str`
+            The header section comment to be used in the .ini file
+        """
+        
+        if (self._heading.title is None):
+            modTypeName = self.getFixModTypeHeadingname()
+            self._heading.title = f"{modTypeName}Boss Fix"
+        return f"; {self._heading.open()}"
     
-    @classmethod
-    def getFixFooter(cls) -> str:
+    def getFixFooter(self) -> str:
         """
         Retrieves the footer text used to identify a code section has been changed by this fix
-        in the .ini file  
+        in the .ini file
+
+        Returns
+        -------
+        :class:`str`
+            The footer section comment to be used in the .ini file
         """
 
-        return f"\n\n{cls._fixFooter}"
+        if (self._heading.title is None):
+            modTypeName = self.getFixModTypeHeadingname()
+            self._heading.title = f"{modTypeName}Boss Fix"
+        return f"\n\n; {self._heading.close()}"
+    
+    def getFixCredit(self) -> str:
+        """
+        Retrieves the credit text for the code generated in the .ini file
+
+        Returns
+        -------
+        :class:`str`
+            The credits to be displayed in the .ini file
+        """
+
+        modTypeName = self.getFixModTypeName()
+        if (modTypeName is None):
+            modTypeName = ""
+
+        if (modTypeName):
+            modTypeName += " "
+
+        bossModTypeName = f"{modTypeName}Boss "
+        return self.Credit.replace(self.ModTypeBossNameReplaceStr, bossModTypeName).replace(self.ModTypeNameReplaceStr, modTypeName)
 
     def _addFixBoilerPlate(func):
         """
         Decorator used to add the boilerplate code to identify a code section has been changed by this fix in the .ini file
 
         Examples
         --------
@@ -2248,15 +2834,15 @@
             @_addFixBoilerPlate
             def helloWorld(self) -> str:
                 return "Hello World"
         """
 
         def addFixBoilerPlateWrapper(self, *args, **kwargs):
             addFix = self.getFixHeader()
-            addFix += self.Credit
+            addFix += self.getFixCredit()
             addFix += func(self, *args, **kwargs)
             addFix += self.getFixFooter()
 
             return addFix
         return addFixBoilerPlateWrapper
     
     @classmethod
@@ -2265,38 +2851,43 @@
         Makes the name of a `section`_ to be used for the resource `sections`_ of a .ini file
 
         Examples
         --------
         >>> IniFile.getResourceName("CuteLittleEi")
         "ResourceCuteLittleEi"
 
+
+        >>> IniFile.getResourceName("ResourceCuteLittleEi")
+        "ResourceCuteLittleEi"
+
         Parameters
         ----------
         name: :class:`str`
             The name of the `section`_
 
         Returns
         -------
         :class:`str`
             The name of the `section`_ as a resource in a .ini file
         """
 
-        return f"{cls.Resource}{name}"
+        if (not name.startswith(cls.Resource)):
+            name = f"{cls.Resource}{name}"
+        return name
     
     @classmethod
     def removeResourceName(cls, name: str) -> str:
         """
         Removes the 'Resource' prefix from a section's name
 
         Examples
         --------
         >>> IniFile.removeResourceName("ResourceCuteLittleEi")
         "CuteLittleEi"
 
-        
 
         >>> IniFile.removeResourceName("LittleMissGanyu")
         "LittleMissGanyu"
 
         Parameters
         ----------
         name: :class:`str`
@@ -2316,29 +2907,31 @@
     @classmethod
     def getRemapName(cls, name: str) -> str:
         """
         Changes a `section`_ name to have the keyword 'RemapBlend' to identify that the `section`_
         is created by this fix
 
 
-        This function either replace the keyword 'Blend' with 'RemapBlend' or adds 'RemapBlend'
-
         Examples
         --------
         >>> IniFile.getRemapName("EiTriesToUseBlenderAndFails")
         "EiTriesToUseRemapBlenderAndFails"
 
 
         >>> IniFile.getRemapName("EiBlendsTheBlender")
         "EiBlendsTheRemapBlender"
     
 
         >>> IniFile.getRemapName("ResourceCuteLittleEi")
         "ResourceCuteLittleEiRemapBlend"
 
+
+        >>> IniFile.getRemapName("ResourceCuteLittleEiRemapRemapBlend")
+        "ResourceCuteLittleEiRemapRemapBlend"
+
         Parameters
         ----------
         name: :class:`str`
             The name of the `section`_
 
         Returns
         -------
@@ -2372,17 +2965,15 @@
         Returns
         -------
         :class:`str`
             The name of the section with the prefix 'Resource' and the keyword 'Remap' added
         """
 
         name = cls.getRemapName(name)
-        if (not name.startswith(cls.Resource)):
-            name = cls.getResourceName(name)
-
+        name = cls.getResourceName(name)
         return name
 
     def _isIfTemplateResource(self, ifTemplatePart: Dict[str, Any]) -> bool:
         """
         Whether the content for some part of a `section`_ contains the key 'vb1'
 
         Parameters
@@ -2464,15 +3055,15 @@
         Any
             The corresponding value for the key 'run'
         """
 
         return ifTemplatePart[self.Run]
     
     # fills the attributes for the sections related to the texture override blend
-    def fillTextureOverrideRemapBlend(self, sectionName: str, part: Dict[str, Any], partIndex: int, linePrefix: str, origSectionName: str) -> str:
+    def _fillTextureOverrideRemapBlend(self, sectionName: str, part: Dict[str, Any], partIndex: int, linePrefix: str, origSectionName: str) -> str:
         """
         Creates the **content part** of an :class:`IfTemplate` for the new sections created by this fix related to the ``[TextureOverride.*Blend.*]`` `sections`_
 
         .. note::
             For more info about an 'IfTemplate', see :class:`IfTemplate`
 
         Parameters
@@ -2505,16 +3096,24 @@
 
             # filling in the subcommand
             if (varName == self.Run):
                 subCommandStr = f"{self.Run} = {self._blendCommandsRemapNames[varValue]}"
                 addFix += f"{linePrefix}{subCommandStr}\n"
 
             # filling in the hash
-            if (varName == self.Hash):
-                addFix += f"{linePrefix}hash = fe5c0180\n"
+            elif (varName == self.Hash):
+                hash = ""
+                if (self._type is not None):
+                    hash = self._type.bossHash
+                elif (self.defaultModType is not None):
+                    hash = self.defaultModType.bossHash
+                else:
+                    raise NoModType()
+
+                addFix += f"{linePrefix}hash = {hash}\n"
 
             # filling in the vb1 resource
             elif (varName == self.Vb1):
                 blendName = self._getIfTemplateResourceName(part)
                 remapModel = self.remapBlendModelsDict[blendName]
                 fixStr = f'{self.Vb1} = {remapModel.fixedBlendName}'
                 addFix += f"{linePrefix}{fixStr}\n"
@@ -2528,15 +3127,15 @@
             elif (varName == self.Draw):
                 fixStr = f'{self.Draw} = {varValue}'
                 addFix += f"{linePrefix}{fixStr}\n"
 
         return addFix
     
     # fill the attributes for the sections related to the resources
-    def fillRemapResource(self, sectionName: str, part: Dict[str, Any], partIndex: int, linePrefix: str, origSectionName: str):
+    def _fillRemapResource(self, sectionName: str, part: Dict[str, Any], partIndex: int, linePrefix: str, origSectionName: str):
         """
         Creates the **content part** of an :class:`IfTemplate` for the new `sections`_ created by this fix related to the ``[Resource.*Blend.*]`` `sections`_
 
         .. note::
             For more info about an 'IfTemplate', see :class:`IfTemplate`
 
         Parameters
@@ -2569,23 +3168,23 @@
 
             # filling in the subcommand
             if (varName == self.Run):
                 subCommandStr = f"{self.Run} = {self._resourceCommandsRemapNames[varValue]}"
                 addFix += f"{linePrefix}{subCommandStr}\n"
 
             # add in the type of file
-            if (varName == "type"):
+            elif (varName == "type"):
                 addFix += f"{linePrefix}type = Buffer\n"
 
             # add in the stride for the file
-            if (varName == "stride"):
+            elif (varName == "stride"):
                 addFix += f"{linePrefix}stride = 32\n"
 
             # add in the file
-            if (varName == "filename"):
+            elif (varName == "filename"):
                 remapModel = self.remapBlendModelsDict[origSectionName]
                 fixedBlendFile = remapModel.fixedBlendPaths[partIndex]
                 addFix += f"{linePrefix}filename = {fixedBlendFile}\n"
 
         return addFix
     
     # fills the if..else template in the .ini for each section
@@ -2685,29 +3284,29 @@
             fix += "\n\n"
 
         # get the fix string for all the texture override blends
         for commandTuple in self._blendCommandsTuples:
             section = commandTuple[0]
             ifTemplate = commandTuple[1]
             commandName = self.getRemapName(section)
-            fix += self.fillIfTemplate(commandName, ifTemplate, self.fillTextureOverrideRemapBlend)
+            fix += self.fillIfTemplate(commandName, ifTemplate, self._fillTextureOverrideRemapBlend)
             fix += "\n"
 
         if (hasResources):
             fix += "\n"
 
         # get the fix string for the resources
         resourceCommandsLen = len(self._resourceCommandsTuples)
         for i in range(resourceCommandsLen):
             commandTuple = self._resourceCommandsTuples[i]
             section = commandTuple[0]
             ifTemplate = commandTuple[1]
 
             resourceName = self.getRemapName(section)
-            fix += self.fillIfTemplate(resourceName, ifTemplate, self.fillRemapResource, origSectionName = section)
+            fix += self.fillIfTemplate(resourceName, ifTemplate, self._fillRemapResource, origSectionName = section)
 
             if (i < resourceCommandsLen - 1):
                 fix += "\n"
 
         return fix
 
     @_readLines
@@ -2754,76 +3353,60 @@
             result = f"{original}\n{addition}"
 
         # writing the fixed file
         if (self.file is not None):
             with open(self.file, "w", encoding = IniFileEncoding) as f:
                 f.write(result)
 
-        self._isRaidenFixed = True
+        self._isFixed = True
         return result
 
     @_readLines
     def _removeScriptFix(self) -> str:
         """
         Removes the dedicated section of the code in the .ini file that this script has made  
 
         Returns
         -------
         :class:`str`
             The new text content of the .ini file
         """
 
-        fileTxt = "".join(self._fileLines)
-        fileTxt = re.sub(self._fixRemovalPattern, "", fileTxt)
-        fileTxt = fileTxt.strip()
-        
-        if (self.file is not None):
-            with open(self.file, "w", encoding = IniFileEncoding) as f:
-                f.write(fileTxt)
-
-            self.clearRead()
-        else:
-            self._fileLines = fileTxt.split("\n")
-            fileLinesLen = len(self._fileLines)
-
-            for i in range(fileLinesLen):
-                if (i < fileLinesLen - 1):
-                    self._fileLines[i] = f"{self._fileLines[i]}\n"
-
-            self._isRaidenFixed = False
+        self._fileTxt = re.sub(self._fixRemovalPattern, "", self._fileTxt)
+        self.fileTxt = self._fileTxt.strip()
 
-        return fileTxt
+        result = self.write()
+        self.clearRead()
+        self._isFixed = False
+        return result
 
     def _removeFix(self) -> str:
         """
         Removes any previous changes that were probably made by this script :raw-html:`<br />` :raw-html:`<br />`
 
         For the .ini file will remove:
 
-        #. All code surrounded by the *'---...--- Raiden Boss Fix ---...----'* header/footer
+        #. All code surrounded by the *'---...--- .* Boss Fix ---...----'* header/footer
         #. All `sections`_ containing the keywords ``RemapBlend``
 
         Returns
         -------
         :class:`str`
             The new text content of the .ini file with the changes removed
         """
 
         self._removeScriptFix()        
         if (not self._fileLinesRead):
-            self.getFileLines()
+            self.readFileLines()
 
         self.removeSectionOptions(self._removalPattern)
         result = self.write()
 
-        if (self.file is not None):
-            self.clearRead()
-        else:
-            self._isRaidenFixed = False
-
+        self.clearRead()
+        self._isFixed = False
         return result
 
     @_readLines
     def removeFix(self, keepBackups: bool = True, fixOnly: bool = False) -> str:
         """
         Removes any previous changes that were probably made by this script and creates backup copies of the .ini file
 
@@ -2852,15 +3435,15 @@
         """
         
         if (keepBackups and not fixOnly and self.file is not None):
             self.print("log", f"Creating Backup for {os.path.basename(self.file)}")
             self.disIni()
 
         if (fixOnly):
-            return "".join(self._fileLines)
+            return self._fileTxt
 
         if (self.file is not None):
             self.print("log", f"Removing any previous changes from this script in {os.path.basename(self.file)}")
 
         result = self._removeFix()
         return result
 
@@ -2878,15 +3461,15 @@
         """
 
         folderPath = CurrentDir
         if (self.file is not None):
             folderPath = os.path.dirname(self.file)
         
         for resourceKey in self._resourceCommands:
-            resourceIftemplate = self._sectionIfTemplates[resourceKey]
+            resourceIftemplate = self._resourceCommands[resourceKey]
             fixedBlendName = self.getRemapResourceName(resourceKey)
             origBlendPaths = {}
             fixedBlendPaths = {}
 
             partIndex = 0
             for part in resourceIftemplate:
                 if (isinstance(part,str)):
@@ -2940,15 +3523,15 @@
         Returns
         -------
         Optional[:class:`IfTemplate`]
             The corresponding :class:`IfTemplate` for the `section`_
         """
         try:
             ifTemplate = self._sectionIfTemplates[sectionName]
-        except BaseException as e:
+        except Exception as e:
             if (raiseException):
                 raise KeyError(f"The section by the name '{sectionName}' does not exist") from e
             else:
                 return None
         else:
             return ifTemplate
 
@@ -2983,17 +3566,14 @@
         for part in ifTemplate:
             if (isinstance(part, str)):
                 continue
 
             if (self._isIfTemplateResource(part)):
                 resource = self._getIfTemplateResourceName(part)
                 blendResources.add(resource)
-
-            if (not self._isIfTemplateSubCommand(part)):
-                continue
         
         # get all the unvisited subcommand sections to visit
         self._getSubCommands(ifTemplate, currentSubCommands, subCommands, subCommandLst)
 
         # get the blend resources from other subcommands
         for sectionName in currentSubCommands:
             self._getBlendResources(sectionName, blendResources, subCommands, subCommandLst)
@@ -3043,57 +3623,63 @@
         Raises
         ------
         :class:`KeyError`
             If a certain resource `section`_ is not found :raw-html:`<br />` :raw-html:`<br />`
             
             (either the name of the `section`_ is not found in the .ini file or the `section`_ was skipped due to some error when parsing the `section`_)
         """
+        self._blendCommands = {}
+        self._blendCommandsRemapNames = {}
+        self._resourceCommands = {}
+        self._resourceCommandsRemapNames = {}
+        self._blendCommandsTuples = []
+        self._resourceCommandsTuples = []
+
+        self._sectionIfTemplates = self.getSectionOptions(self._sectionPattern, postProcessor = self._processIfTemplate, handleDuplicateFunc = lambda duplicates: duplicates[0])
 
-        self._sectionIfTemplates = self.getSectionOptions(self._sectionPattern, postProcessor = self._processIfTemplate)
+        if (self.defaultModType is not None and self._textureOverrideBlendSectionName is not None and self._textureOverrideBlendRoot is None):
+            self._textureOverrideBlendRoot = self._textureOverrideBlendSectionName
 
         try:
             self._sectionIfTemplates[self._textureOverrideBlendRoot]
         except:
             return
 
-        self._isRaidenIni = True
         blendResources = set()
         subCommands = { self._textureOverrideBlendRoot }
         subCommandLst = [self._textureOverrideBlendRoot]
         resourceCommands = set()
         resourceCommandLst = []
 
         # keep track of all the needed blend dependencies
         self._getBlendResources(self._textureOverrideBlendRoot, blendResources, subCommands, subCommandLst)
 
         # read in all the needed dependencies
         for blend in blendResources:
             try:
                 self._resourceBlends[blend] = self._sectionIfTemplates[blend]
-            except BaseException as e:
+            except Exception as e:
                 raise KeyError(f"The resource by the name, '{blend}', does not exist") from e
             else:
                 resourceCommands.add(blend)
                 resourceCommandLst.append(blend)
 
         # sort the resources
-        resourceCommandLst.sort(key = lambda resourceName: self._getResourceSortKey((resourceName, None)))
+        resourceCommandLst = list(map(lambda resourceName: (resourceName, self.getMergedResourceIndex(resourceName)), resourceCommandLst))
+        resourceCommandLst.sort(key = cmp_to_key(self._compareResources))
+        resourceCommandLst = list(map(lambda resourceTuple: resourceTuple[0], resourceCommandLst))
 
         # keep track of all the subcommands that the resources call
         for blend in blendResources:
             self._getCommands(blend, resourceCommands, resourceCommandLst)
 
-        self._blendCommands = {}
-        self._blendCommandsRemapNames = {}
         for subCommand in subCommands:
             self._blendCommands[subCommand] = self._sectionIfTemplates[subCommand]
             self._blendCommandsRemapNames[subCommand] = self.getRemapName(subCommand)
 
-        self._resourceCommands = {}
-        self._resourceCommandsRemapNames = {}
         for subCommand in resourceCommands:
             self._resourceCommands[subCommand] = self._sectionIfTemplates[subCommand]
             self._resourceCommandsRemapNames[subCommand] = self.getRemapName(subCommand)
 
         self._blendCommandsTuples = list(map(lambda subCommand: (subCommand, self._blendCommands[subCommand]), subCommandLst))
         self._resourceCommandsTuples = list(map(lambda subCommand: (subCommand, self._resourceCommands[subCommand]), resourceCommandLst))   
 
@@ -3120,33 +3706,37 @@
         -------
         :class:`str`
             The new content of the .ini file which includes the fix
         """
 
         fix = ""
         fix += self.getFixStr(fix = fix)
-        return self.injectAddition(f"\n\n{fix}", beforeOriginal = False, keepBackup = keepBackup, fixOnly = fixOnly)
+        result = self.injectAddition(f"\n\n{fix}", beforeOriginal = False, keepBackup = keepBackup, fixOnly = fixOnly)
+        self._isFixed = True
+        return result
 
 
 class Mod(Model):
     """
     This Class inherits from :class:`Model`
 
     Used for handling a mod
 
     .. note::
         We define **a mod** based off the following criteria:
 
         * A folder that contains at least 1 .ini file
         * At least 1 of the .ini files in the folder contains:
 
-            * a section with the regex ``[.*TextureOverride.*(Raiden|Shogun).*]`` if :attr:`RaidenBossFixService.readAllInis` is set to ``False`` :raw-html:`<br />` **OR** :raw-html:`<br />`
-            * a section with the regex ``[.*TextureOverride.*Blend.*]`` if :attr:`RaidenBossFixService.readAllInis` is set to ``True`` or the script is ran with the ``--all`` flag
-
+            * a section with the regex ``[TextureOverride.*Blend]`` if :attr:`BossFixService.readAllInis` is set to ``True`` or the script is ran with the ``--all`` flag :raw-html:`<br />`  :raw-html:`<br />` **OR** :raw-html:`<br />` :raw-html:`<br />`
+            * a section that meets the criteria of one of the mod types defined :attr:`Mod._types` by running the mod types' :meth:`ModType.isType` function
 
+        :raw-html:`<br />`
+        See :class:`ModTypes` for some predefined types of mods
+        
     Parameters
     ----------
     path: Optional[:class:`str`]
         The file location to the mod folder. :raw-html:`<br />` :raw-html:`<br />`
         
         If this value is set to ``None``, then will use the current directory of where this module is loaded.
         :raw-html:`<br />` :raw-html:`<br />`
@@ -3161,49 +3751,72 @@
         **Default**: ``None``
 
     logger: Optional[:class:`Logger`]
         The logger used to pretty print messages :raw-html:`<br />` :raw-html:`<br />`
 
         **Default**: ``None``
 
+    types: Optional[Set[:class:`ModType`]]
+        The types of mods this mod should be. :raw-html:`<br />` :raw-html:`<br />` 
+        If this argument is empty or is ``None``, then all the .ini files in this mod will be parsed :raw-html:`<br />` :raw-html:`<br />`
+
+        **Default**: ``None``
+
+    defaultType: Optional[:class:`ModType`]
+        The type of mod to use if a mod has an unidentified type :raw-html:`<br />` :raw-html:`<br />`
+        If this argument is ``None``, then will skip the mod with an identified type :raw-html:`<br />` :raw-html:`<br />` 
+
+        **Default**: ``None``
+
     Attributes
     ----------
     path: Optional[:class:`str`]
         The file location to the mod folder
 
     _files: List[:class:`str`]
         The direct children files to the mod folder (does not include files located in a folder within the mod folder).
 
+    _types: Set[:class:`ModType`]
+        The types of mods this mod should be
+
+    _defaultType: Optional[:class:`ModType`]
+        The type of mod to use if a mod has an unidentified type
+
     logger: Optional[:class:`Logger`]
         The logger used to pretty print messages
 
     inis: List[:class:`str`]
         The .ini files found for the mod
 
     remapBlend: List[:class:`str`]
         The RemapBlend.buf files found for the mod
 
     backupInis: List[:class:`str`]
-        The DISABLED_RSFixBackup.txt files found for the mod
+        The DISABLED_BossFixBackup.txt files found for the mod
 
     backupDups: List[:class:`str`]
         The DISABLED_RSDup.txt files found for the mod
 
         .. warning::
             This attribute is now DEPRECATED. Now, the fix does not care whether there are duplicate .ini files or Blend.buf files
     """
-    def __init__(self, path: Optional[str] = None, files: Optional[List[str]] = None, logger: Optional[Logger] = None):
+    def __init__(self, path: Optional[str] = None, files: Optional[List[str]] = None, logger: Optional[Logger] = None, types: Optional[Set[ModType]] = None, defaultType: Optional[ModType] = None):
         super().__init__(logger = logger)
         self.path = FileService.getPath(path)
         self._files = files
+        if (types is None):
+            types = set()
+        self._types = types
+        self._defaultType = defaultType
+
+        self.inis = []
+        self.remapBlend = []
+        self.backupInis = []
         self._setupFiles()
 
-        self.inis, self.remapBlend, self.backupInis, self.backupDups = self.getOptionalFiles()
-        self.inis = list(map(lambda iniPath: IniFile(iniPath, logger = logger), self.inis))
-
     @property
     def files(self):
         """
         The direct children files to the mod folder (does not include files located in a folder within the mod folder).
 
         :getter: Returns the files to the mod
         :setter: Sets up the files for the mod
@@ -3221,14 +3834,17 @@
         """
         Searches the direct children files to the mod folder if :attr:`Mod.files` is set to ``None``        
         """
 
         if (self._files is None):
             self._files = FileService.getFiles(path = self.path)
 
+        self.inis, self.remapBlend, self.backupInis = self.getOptionalFiles()
+        self.inis = list(map(lambda iniPath: IniFile(iniPath, logger = self.logger, modTypes = self._types, defaultModType = self._defaultType), self.inis))
+
     @classmethod
     def isIni(cls, file: str) -> bool:
         """
         Determines whether the file is a .ini file which is the file used to control how a mod behaves
 
         Parameters
         ----------
@@ -3285,72 +3901,50 @@
         """
 
         return bool(file.endswith(BlendFileType) and not cls.isRemapBlend(file))
    
     @classmethod
     def isBackupIni(cls, file: str) -> bool:
         """
-        Determines whether the file is a DISABLED_RSFixBackup.txt file that is used to make
+        Determines whether the file is a DISABLED_BossFixBackup.txt file that is used to make
         backup copies of .ini files
 
         Parameters
         ----------
         file: :class:`str`
             The file path to check
 
         Returns
         -------
         :class:`bool`
-            Whether the passed in file is a DISABLED_RSFixBackup.txt file
-        """
-        
-        return BackupFilePrefix in file and file.endswith(TxtExt)
-    
-    @classmethod
-    def isBackupDupFile(cls, file: str) -> bool:
+            Whether the passed in file is a DISABLED_BossFixBackup.txt file
         """
-        .. warning::
-            This function is now DEPRECATED. Now, the fix does not care whether there are duplicate .ini files or Blend.buf files
 
-        Determines whether the file is a DISABLED_RSDup.txt file that is used to disable duplicate .ini files
-        or Blend.buf files
-
-        Parameters
-        ----------
-        file: :class:`str`
-            The file path to check
-
-        Returns
-        -------
-        :class:`bool`
-            Whether the passed in file is a DISABLED_RSDup.txt file
-        """
-                
-        return DuplicateFilePrefix in file and file.endswith(TxtExt)
+        fileBaseName = os.path.basename(file)
+        return fileBaseName.startswith(BackupFilePrefix) and file.endswith(TxtExt)
 
     def getOptionalFiles(self) -> List[Optional[str]]:
         """
         Retrieves a list of each type of files that are not mandatory for the mod
 
         Returns
         -------
-        [ List[:class:`str`], List[:class:`str`], List[:class:`str`], List[:class:`str`] ]
+        [ List[:class:`str`], List[:class:`str`], List[:class:`str`]]
             The resultant files found for the following file categories (listed in the same order as the return type):
 
             #. .ini files
             #. .RemapBlend.buf files
-            #. DISABLED_RSFixBackup.txt files
-            #. DISABLED_RSDup.txt files
+            #. DISABLED_BossFixBackup.txt files
 
             .. note::
-                See :meth:`Mod.isIni`, :meth:`Mod.isRemapBlend`, :meth:`Mod.isBackupIni` or :meth:`Mod.isBackupDupFile` for the specifics of each type of file
+                See :meth:`Mod.isIni`, :meth:`Mod.isRemapBlend`, :meth:`Mod.isBackupIni` for the specifics of each type of file
         """
 
         SingleFileFilters = {}
-        MultiFileFilters = [self.isIni, self.isRemapBlend, self.isBackupIni, self.isBackupDupFile]
+        MultiFileFilters = [self.isIni, self.isRemapBlend, self.isBackupIni]
 
         singleFiles = []
         if (SingleFileFilters):
             singleFiles = FileService.getSingleFiles(path = self.path, filters = SingleFileFilters, files = self._files, optional = True)
         multiFiles = FileService.getFiles(path = self.path, filters = MultiFileFilters, files = self._files)
 
         result = singleFiles
@@ -3358,83 +3952,141 @@
             result = [result]
 
         result += multiFiles
         return result
     
     def removeBackupInis(self):
         """
-        Removes all DISABLED_RSFixBackup.txt contained in the mod
+        Removes all DISABLED_BossFixBackup.txt contained in the mod
         """
 
         for file in self.backupInis:
             self.print("log", f"Removing the backup ini, {os.path.basename(file)}")
             os.remove(file)
 
-    def removeBackupDups(self):
-        """
-        Removes all DISABLED_RSDup.txt contained in the mod
-        """
-
-        for file in self.backupDups:
-            self.print("log", f"Removing the unused duplicate file, {os.path.basename(file)}")
-            os.remove(file)
-
-    def removeFix(self, fixedBlends: Set[str], fixedInis: Set[str], keepBackups: bool = True, fixOnly: bool = False):
+    def removeFix(self, fixedBlends: Set[str], fixedInis: Set[str], visitedRemapBlendsAtRemoval: Set[str], inisSkipped: Dict[str, Exception], keepBackups: bool = True, fixOnly: bool = False) -> List[Set[str]]:
         """
         Removes any previous changes done by this module's fix
 
         Parameters
         ----------
         fixedBlend: Set[:class:`str`]
             The file paths to the RemapBlend.buf files that we do not want to remove
 
         fixedInis: Set[:class:`str`]
             The file paths to the .ini files that we do not want to remove
 
+        visitedRemapBlendsAtRemoval: Set[:class:`str`]
+            The file paths to the RemapBlend.buf that have already been attempted to be removed
+
+        inisSkipped: Dict[:class:`str`, :class:`Exception`]
+            The file paths to the .ini files that are skipped due to errors
+
         keepBackups: :class:`bool`
-            Whether to create or keep DISABLED_RSFixBackup.txt files in the mod :raw-html:`<br />` :raw-html:`<br />`
+            Whether to create or keep DISABLED_BossFixBackup.txt files in the mod :raw-html:`<br />` :raw-html:`<br />`
 
             **Default**: ``True``
 
         fixOnly: :class:`bool`
             Whether to not undo any changes created in the .ini files :raw-html:`<br />` :raw-html:`<br />`
 
             **Default**: ``False``
-        """
 
-        filesRemoved = False
-        if (self.remapBlend is not None):
-            for remapBlend in self.remapBlend:
-                remapBlendFullPath = FileService.absPathOfRelPath(remapBlend, self.path)
-
-                # remove only remap blends that have not been recently created
-                if (remapBlendFullPath not in fixedBlends):
-                    self.print("log", f"Removing previous {RemapBlendFile} at {os.path.basename(remapBlend)}")
-                    os.remove(remapBlend)
+        Returns
+        -------
+        [Set[:class:`str`], Set[:class:`str`]]
+            The removed files that have their fix removed, where the types of files for the return value is based on the list below:
+
+            #. .ini files with their fix removed
+            #. RemapBlend.buf files that got deleted
+        """
 
-                    if (not filesRemoved):
-                        filesRemoved = True
+        removedRemapBlends = set()
+        undoedInis = set()
 
         for ini in self.inis:
-            iniFullPath = FileService.absPathOfRelPath(ini.file, self.path)
-            if (iniFullPath not in fixedInis and ini.isRaidenIni):
-                ini.removeFix(keepBackups = keepBackups, fixOnly = fixOnly)
+            remapBlendsRemoved = False
+            iniFilesUndoed = False
+            iniFullPath = None
+            iniHasErrors = False
+            if (ini.file is not None):
+                iniFullPath = FileService.absPathOfRelPath(ini.file, self.path)
+
+            # parse the .ini file even if we are only undoing fixes for the case where a Blend.buf file
+            #   forms a bridge with some disconnected folder subtree of a mod
+            # Also, we only want to remove the Blend.buf files connected to particular types of .ini files, 
+            #   instead of all the Blend.buf files in the folder
+            if (iniFullPath is None or (iniFullPath not in fixedInis and iniFullPath not in inisSkipped)):
+                try:
+                    ini.parse()
+                except Exception as e:
+                    inisSkipped[iniFullPath] = e
+                    iniHasErrors = True
+                    self.print("handleException", e)
+
+            # remove only the remap blends that have not been recently created
+            for blendModel in ini.remapBlendModels:
+                for partIndex in blendModel.fullPaths:
+                    remapBlendFullPath = blendModel.fullPaths[partIndex]
+
+                    if (remapBlendFullPath not in fixedBlends and remapBlendFullPath not in visitedRemapBlendsAtRemoval):
+                        try:
+                            os.remove(remapBlendFullPath)
+                        except FileNotFoundError as e:
+                            self.print("log", f"No Previous {RemapBlendFile} found at {remapBlendFullPath}")
+                        else:
+                            self.print("log", f"Removing previous {RemapBlendFile} at {remapBlendFullPath}")
+                            removedRemapBlends.add(remapBlendFullPath)
+
+                        visitedRemapBlendsAtRemoval.add(remapBlendFullPath)
+                        if (not remapBlendsRemoved):
+                            remapBlendsRemoved = True
+
+            if (remapBlendsRemoved):
+                self.print("space")
 
-                if (not filesRemoved):
-                    filesRemoved = True
+            if (iniHasErrors):
+                continue
 
-        if (filesRemoved):
-            self.print("space")
+            # remove the fix from the .ini files
+            if (iniFullPath is not None and iniFullPath not in fixedInis and iniFullPath not in inisSkipped and 
+                ini.isModIni and (not self._types or ini.type in self._types)):
+                try:
+                    ini.removeFix(keepBackups = keepBackups, fixOnly = fixOnly)
+                except Exception as e:
+                    inisSkipped[iniFullPath] = e
+                    iniHasErrors = True
+                    self.print("handleException", e)
+                    continue
+
+                undoedInis.add(iniFullPath)
+
+                if (not iniFilesUndoed):
+                    iniFilesUndoed = True
+
+            if (iniFilesUndoed):
+                self.print("space")
+
+        return [undoedInis, removedRemapBlends]
 
     # correcting the blend file
     @classmethod
-    def blendCorrection(self, blendFile: Union[str, bytes], fixedBlendFile: Optional[str] = None) -> Union[str, bytes]:
+    def blendCorrection(self, blendFile: Union[str, bytes], modType: ModType, fixedBlendFile: Optional[str] = None) -> Union[Optional[str], bytearray]:
         """
         Fixes a Blend.buf file
 
+        .. note::
+            We observe that a Blend.buf file is a binary file defined as:
+
+            * each line contains 32 bytes (256 bits)
+            * each line uses little-endian mode (MSB is to the right while LSB is to the left)
+            * the first 16 bytes of a line are for the blend weights, each weight is 4 bytes or 32 bits (4 weights/line)
+            * the last 16 bytes of a line are for the corresponding indices for the blend weights, each index is 4 bytes or 32 bits (4 indices/line)
+            * the blend weights are floating points while the blend indices are unsigned integers
+
         Parameters
         ----------
         blendFile: Union[:class:`str`, :class:`bytes`]
             The file path to the Blend.buf file to fix
 
         fixedBlendFile: Optional[:class:`str`]
             The file path for the fixed Blend.buf file :raw-html:`<br />` :raw-html:`<br />`
@@ -3442,110 +4094,177 @@
             **Default**: ``None``
 
         Raises
         ------
         :class:`BlendFileNotRecognized`
             If the original Blend.buf file provided by the parameter ``blendFile`` cannot be read
 
+        :class:`BadBlendData`
+            If the bytes passed into this function do not correspond to the format defined for a Blend.buf file
+
         Returns
         -------
-        Union[:class:`str`, :class:`bytes`]
-            If the argument ``fixedBlendFile`` is ``None``, then will return bytes for the fixed Blend.buf file :raw-html:`<br />` :raw-html:`<br />`
-            Otherwise will return the filename fo the fixed RemapBlend.buf file
+        Union[Optional[:class:`str`], :class:`bytearray`]
+            If the argument ``fixedBlendFile`` is ``None``, then will return an array of bytes for the fixed Blend.buf file :raw-html:`<br />` :raw-html:`<br />`
+            Otherwise will return the filename to the fixed RemapBlend.buf file if the provided Blend.buf file got corrected
         """
 
+        # if no correction is needed to be done
+        blendIsFile = isinstance(blendFile, str)
+        if (not modType.vgRemap and blendIsFile):
+            return None
+        elif (not modType.vgRemap):
+            return bytearray(blendFile)
+
         blendData = None
-        if (isinstance(blendFile, str)):
+        if (blendIsFile):
             with open(blendFile, "rb") as f:
                 blendData = f.read()
         else:
             blendData = blendFile
 
-        if len(blendData)%32 != 0:
-            raise BlendFileNotRecognized(blendFile)
+        if (len(blendData)%32 != 0):
+            if (blendIsFile):
+                raise BlendFileNotRecognized(blendFile)
+            else:
+                raise BadBlendData()
 
         result = bytearray()
         for i in range(0,len(blendData),32):
             blendweights = [struct.unpack("<f", blendData[i+4*j:i+4*(j+1)])[0] for j in range(4)]
             blendindices = [struct.unpack("<I", blendData[i+16+4*j:i+16+4*(j+1)])[0] for j in range(4)]
             outputweights = bytearray()
             outputindices = bytearray()
+
+            # replaces the blend index in the original mod with the corresponding blend index
+            #   for the boss
             for weight, index in zip(blendweights, blendindices):
-                if weight != 0 and index <= MaxVGIndex:
-                    index = int(VGRemap[str(index)])
+                if weight != 0 and index <= modType.maxVgIndex:
+                    index = int(modType.vgRemap[index])
                 outputweights += struct.pack("<f", weight)
                 outputindices += struct.pack("<I", index)
             result += outputweights
             result += outputindices
 
         if (fixedBlendFile is not None):
             with open(fixedBlendFile, "wb") as f:
                 f.write(result)
 
             return fixedBlendFile
 
         return result
     
-    def correctBlend(self, fixedRemapBlends: Dict[str, RemapBlendModel]):
+    def correctBlend(self, fixedRemapBlends: Dict[str, RemapBlendModel], skippedBlends: Dict[str, Exception]) -> List[Union[Set[str], Dict[str, Exception]]]:
         """
         Fixes all the Blend.buf files reference by the mod
 
         Requires all the .ini files in the mod to have ran their :meth:`IniFile.parse` function
 
         Parameters
         ----------
         fixedRemapBlends: Dict[:class:`str`, :class:`RemapBlendModel`]
-            All of the RemapBlend.buf files that have already been fixed.
-            :raw-html:`<br />`
-            :raw-html:`<br />`
+            All of the RemapBlend.buf files that have already been fixed. :raw-html:`<br />` :raw-html:`<br />`
+
             The keys are the absolute filepath to the fixed RemapBlend.buf file and the values contains the data related
             to the fixed RemapBlend.buf file
+
+        skippedBlends: Dict[:class:`str`, :class:`Exception`]
+            All of the RemapBlend.buf files that have already been skipped due to some error when trying to fix them :raw-html:`<br />` :raw-html:`<br />`
+
+            The keys are the absolute filepath to the RemapBlend.buf file that was attempted to be fixed and the values are the exception encountered
+
+        Returns
+        -------
+        [Set[:class:`str`], Dict[:class:`str`, :class:`Exception`]]
+            #. The absolute file paths of the RemapBlend.buf files that were fixed
+            #. The exceptions encountered when trying to fix some RemapBlend.buf files :raw-html:`<br />` :raw-html:`<br />`
+
+            The keys are absolute filepath to the RemapBlend.buf file and the values are the exception encountered
         """
 
-        blendsFound = 0
-        blendsSkipped = {}
-        blendsFixed = set()
+        currentBlendsSkipped = {}
+        currentBlendsFixed = set()
 
         for ini in self.inis:
             if (ini is None):
                 continue
 
             for model in ini.remapBlendModels:
+                modType = self._defaultType
+                if (ini.type is not None):
+                    modType = ini.type
+
                 for partIndex in model.fullPaths:
-                    fixedFullPath = model.fullPaths[partIndex]
-                    origFullPath = model.origFullPaths[partIndex]
                     blendFixed = True
+                    fixedFullPath = model.fullPaths[partIndex]
+
+                    try:
+                        origFullPath = model.origFullPaths[partIndex]
+                    except KeyError:
+                        self.print("log", f"Missing Original Blend file for the RemapBlend file at {fixedFullPath}")
+                        if (fixedFullPath not in skippedBlends):
+                            error = RemapMissingBlendFile(fixedFullPath)
+                            currentBlendsSkipped[fixedFullPath] = error
+                            skippedBlends[fixedFullPath] = error
+                        continue
 
+                    # check if the blend file has been fixed
                     try:
                         fixedRemapBlends[fixedFullPath]
                     except:
                         blendFixed = False
                     else:
                         self.print("log", f"Blend file has already been corrected at {fixedFullPath}")
 
-                    if (blendFixed):
+                    # check if the blend was already encountered and did not need to be fixed
+                    try:
+                        fixedRemapBlends[origFullPath]
+                    except KeyError:
+                        pass
+                    else:
+                        blendFixed = True
+
+                    # check if the blend file already had encountered an error
+                    fixedPathWasSkipped = bool(fixedFullPath in skippedBlends)
+                    if (fixedPathWasSkipped or origFullPath in skippedBlends):
+                        targetFullPath = fixedFullPath
+                        if (not fixedPathWasSkipped):
+                            targetFullPath = origFullPath
+
+                        self.print("log", f"Blend file has already previously encountered an error at {targetFullPath}")
+                        continue
+
+                    if (blendFixed or modType is None):
                         continue
                     
-                    blendsFound += 1
+                    correctedBlendPath = None
                     try:
-                        self.blendCorrection(origFullPath, fixedFullPath)
-                    except BaseException as e:
-                        blendsSkipped[fixedFullPath] = e 
+                        correctedBlendPath = self.blendCorrection(origFullPath, modType, fixedBlendFile = fixedFullPath)
+                    except Exception as e:
+                        currentBlendsSkipped[fixedFullPath] = e
+                        skippedBlends[fixedFullPath] = e
                         self.print("handleException", e)
                     else:
-                        self.print("log", f'Blend file correction done at {fixedFullPath}')
-                        blendsFixed.add(fixedFullPath)
-                        fixedRemapBlends[fixedFullPath] = model
+                        pathToAdd = ""
+                        if (correctedBlendPath is None):
+                            self.print("log", f"Blend file does not need to be corrected at {origFullPath}")
+                            pathToAdd = origFullPath
+                        else:
+                            self.print("log", f'Blend file correction done at {fixedFullPath}')
+                            pathToAdd = fixedFullPath
 
-        return [blendsFound, blendsFixed, blendsSkipped]
+                        currentBlendsFixed.add(pathToAdd)
+                        fixedRemapBlends[pathToAdd] = model
 
+        return [currentBlendsFixed, currentBlendsSkipped]
 
-class RaidenBossFixService():
+
+class BossFixService():
     """
-    The overall class for fixing the Raiden Shogun Boss for Raiden Shogun mods
+    The overall class for fixing bosses for particular mods
 
     Parameters
     ----------
     path: Optional[:class:`str`]
         The file location of where to run the fix. :raw-html:`<br />` :raw-html:`<br />`
 
         If this attribute is set to ``None``, then will run the fix from wherever this class is called :raw-html:`<br />` :raw-html:`<br />`
@@ -3578,33 +4297,49 @@
         **Default**: ``True``
 
     readAllInis: :class:`bool`
         Whether to read all the .ini files that the fix encounters :raw-html:`<br />` :raw-html:`<br />`
 
         **Default**: ``False``
 
-    log: :class:`bool`
-        Whether to log the run of the fix in a seperate text file :raw-html:`<br />` :raw-html:`<br />`
+    types: Optional[:class:`str`]
+        A string containing the names for all the types of mods to fix. Each type of mod is seperated using a comma (,)  :raw-html:`<br />` :raw-html:`<br />`
 
-        **Default**: ``False``
+        If this argument is the empty string or this argument is ``None``, then will fix all the types of mods supported by this fix :raw-html:`<br />` :raw-html:`<br />`
+
+        **Default**: ``None``
+
+    defaultType: Optional[:class:`str`]
+        The name for the type to use if a mod has an unidentified type :raw-html:`<br />` :raw-html:`<br />`
+
+        If this value is ``None``, then mods with unidentified types will be skipped :raw-html:`<br />` :raw-html:`<br />`
+
+        **Default**: ``None``
+
+    log: Optional[:class:`str`]
+        The folder location to log the run of the fix into a seperate text file :raw-html:`<br />` :raw-html:`<br />`
+
+        If this value is ``None``, then will not log the fix :raw-html:`<br />` :raw-html:`<br />`
+
+        **Default**: ``None``
 
     verbose: :class:`bool`
         Whether to print the progress for fixing mods :raw-html:`<br />` :raw-html:`<br />`
 
         **Default**: ``True``
 
     handleExceptions: :class:`bool`
         When an exception is caught, whether to silently stop running the fix :raw-html:`<br />` :raw-html:`<br />`
 
         **Default**: ``False``
 
     Attributes
     ----------
-    log: :class:`bool`
-        Whether to log the run of the fix in a seperate text file
+    log: Optional[:class:`str`]
+        The folder location to log the run of the fix into a seperate text file
 
     _loggerBasePrefix: :class:`str`
         The prefix string for the logger used when the fix returns back to the original directory that it started to run
 
     logger: :class:`Logger`
         The logger used to pretty print messages
 
@@ -3619,14 +4354,20 @@
 
     undoOnly: :class:`bool`
         Whether to only undo the fixes previously made by the fix
 
     readAllInis: :class:`bool`
         Whether to read all the .ini files that the fix encounters
 
+    types: Set[:class:`ModType`]
+        All the types of mods that will be fixed.
+
+    defaultType: Optional[:class:`ModType`]
+        The type to use if a mod has an unidentified type
+
     verbose: :class:`bool`
         Whether to print the progress for fixing mods
 
     handleExceptions: :class:`bool`
         When an exception is caught, whether to silently stop running the fix
 
     _logFile: :class:`str`
@@ -3634,70 +4375,81 @@
 
     _pathIsCWD: :class:`bool`
         Whether the filepath that the program runs from is the current directory where this module is loaded
 
     modsFixed: :class:`int`
         The number of mods that have been fixed
 
-    skippedMods: Dict[:class:`str`, :class:`BaseException`]
+    skippedMods: Dict[:class:`str`, :class:`Exception`]
         All the mods that have been skipped :raw-html:`<br />` :raw-html:`<br />`
 
         The keys are the absolute path to the mod folder and the values are the exception that caused the mod to be skipped
 
-    blendsFound: :class:`int`
-        The number of Blend.buf files found within the found mods
-
     blendsFixed: Set[:class:`str`]
         The absolute paths to all the Blend.buf files that have been fixed
 
-    skippedBlends: Dict[:class:`str`, Dict[:class:`str`, :class:`BaseException`]]
-        The Blend.buf files that got skipped :raw-html:`<br />` :raw-html:`<br />`
+    skippedBlendsByMods: DefaultDict[:class:`str`, Dict[:class:`str`, :class:`Exception`]]
+        The RemapBlend.buf files that got skipped :raw-html for each mod :raw-html:`<br />` :raw-html:`<br />`
 
         * The outer key is the absolute path to the mod folder
-        * The inner key is the absolute path to the Blend.buf file
-        * The value in the inner dictionary is the exception that caused the Blend.buf file to be skipped
+        * The inner key is the absolute path to the RemapBlend.buf file
+        * The value in the inner dictionary is the exception that caused the RemapBlend.buf file to be skipped
+
+    skippedBlends: Dict[:class:`str`, :class:`Exception`]
+        The RemapBlend.buf files that got skipped  :raw-html:`<br />` :raw-html:`<br />`
 
-    skippedBlendsCount: :class:`int`
-        The count for how many Blend.buf files got skipped
+        The keys are the absolute path to the RemapBlend.buf file and the values are the exception that caused the RemapBlend.buf file to be skipped
 
     inisFixed: Set[:class:`str`]
         The absolute paths to the fixed .ini files
 
-    inisSkipped: Dict[:class:`str`, :class:`BaseException`]
+    inisSkipped: Dict[:class:`str`, :class:`Exception`]
         The .ini files that got skipped :raw-html:`<br />` :raw-html:`<br />`
 
         The keys are the absolute file paths to the .ini files and the values are exceptions that caused the .ini file to be skipped
+
+    removedRemapBlends: Set[:class:`str`]
+        Previous RemapBlend.buf files that are removed
     """
 
     def __init__(self, path: Optional[str] = None, keepBackups: bool = True, fixOnly: bool = False, undoOnly: bool = False, 
-                 readAllInis: bool = False, log: bool = False, verbose: bool = True, handleExceptions: bool = False):
+                 readAllInis: bool = False, types: Optional[str] = None, defaultType: Optional[str] = None, log: Optional[str] = None, verbose: bool = True, handleExceptions: bool = False):
         self.log = log
         self._loggerBasePrefix = ""
         self.logger = Logger(logTxt = log, verbose = verbose)
         self._path = path
         self.keepBackups = keepBackups
         self.fixOnly = fixOnly
         self.undoOnly = undoOnly
         self.readAllInis = readAllInis
+        self.types = types
+        self.defaultType = defaultType
         self.verbose = verbose
         self.handleExceptions = handleExceptions
-        self._logFile = FileService.parseOSPath(ntpath.join(DefaultPath, LogFile))
         self._pathIsCwd = False
+        self.__errorsBeforeFix = None
 
         # certain statistics about the fix
         self.modsFixed = 0
-        self.skippedMods: Dict[str, BaseException] = {}
-        self.blendsFound = 0
+        self.skippedMods: Dict[str, Exception] = {}
         self.blendsFixed: Set[str] = set()
-        self.skippedBlends: Dict[str, Dict[str, BaseException]] = {}
-        self.skippedBlendsCount = 0
+        self.skippedBlendsByMods: DefaultDict[str, Dict[str, Exception]] = defaultdict(lambda: {})
+        self.skippedBlends: Dict[str, Exception] = {}
         self.inisFixed = set()
-        self.inisSkipped: Dict[str, BaseException] = {}
+        self.inisSkipped: Dict[str, Exception] = {}
+        self.removedRemapBlends: Set[str] = set()
+        self._visitedRemapBlendsAtRemoval: Set[str] = set()
 
         self._setupModPath()
+        self._setupModTypes()
+        self._setupDefaultModType()
+        self._setupLogPath()
+
+        if (self.__errorsBeforeFix is None):
+            self._printModsToFix()
 
     @property
     def pathIsCwd(self):
         """
         Whether the filepath that the program runs from is the current directory where this module is loaded
 
         :getter: Returns whether the filepath that the program runs from is the current directory of where the module is loaded
@@ -3715,33 +4467,124 @@
         :setter: Sets the path for where the fix runs
         :type: :class:`str`
         """
 
         return self._path
     
     @path.setter
-    def path(self, newPath: str):
+    def path(self, newPath: Optional[str]):
         self._path = newPath
         self._setupModPath()
+        self.clear()
+
+    def clear(self):
+        """
+        Clears up all the saved data
+        """
+
+        self.modsFixed = 0
         self.skippedMods = {}
+        self.blendsFixed = set()
+        self.skippedBlendsByMods = defaultdict(lambda: {})
+        self.skippedBlends = {}
+        self.inisFixed = set()
+        self.inisSkipped = {}
+        self.removedRemapBlends = set()
+        self._visitedRemapBlendsAtRemoval = set()
     
     def _setupModPath(self):
         """
         Sets the filepath of where the fix will run from
         """
 
         self._pathIsCwd = False
         if (self._path is None):
             self._path = DefaultPath
             self._pathIsCwd = True
             return
 
         self._path = FileService.parseOSPath(self._path)
-        self._path = os.path.abspath(self._path)
+        self._path = FileService.parseOSPath(os.path.abspath(self._path))
         self._pathIsCwd = (self._path == DefaultPath)
+
+    def _setupLogPath(self):
+        """
+        Sets the folder path for where the log file will be stored
+        """
+
+        if (self.log is not None):
+            self.log = FileService.parseOSPath(os.path.join(self.log, LogFile))
+
+    def _setupModTypes(self):
+        """
+        Sets the types of mods that will be fixed
+        """
+
+        if (isinstance(self.types, set)):
+            return
+
+        modTypes = set()
+        if (self.types is None or self.readAllInis):
+            modTypes = ModTypes.getAll()
+
+        # search for the types of mods to fix
+        else:
+            typesLst = self.types.split(",")
+
+            for typeStr in typesLst:
+                modType = ModTypes.search(typeStr)
+                modTypeFound = bool(modType is not None)
+
+                if (modTypeFound):
+                    modTypes.add(modType)
+                elif (self.__errorsBeforeFix is None):
+                    self.__errorsBeforeFix = InvalidModType(typeStr)
+                    return
+
+        self.types = modTypes
+
+    def _setupDefaultModType(self):
+        """
+        Sets the default mod type to be used for an unidentified mod
+        """
+
+        if (not self.readAllInis):
+            self.defaultType = None
+        elif (self.defaultType is None):
+            self.defaultType = ModTypes.Raiden.value
+            return
+
+        if (self.defaultType is None or isinstance(self.defaultType, ModType)):
+            return
+
+        self.defaultType = ModTypes.search(self.defaultType)
+
+        if (self.defaultType is None and self.__errorsBeforeFix is None):
+            self.__errorsBeforeFix = InvalidModType(self.defaultType)
+
+    def _printModsToFix(self):
+        """
+        Prints out the types of mods that will be fixed
+        """
+
+        self.logger.includePrefix = False
+
+        self.logger.openHeading("Types of Mods To Fix", 5)
+        self.logger.space()
+
+        if (not self.types):
+            self.logger.log("All mods")
+        else:
+            for type in self.types:
+                self.logger.bulletPoint(f"{type.name}")
+        
+        self.logger.space()
+        self.logger.closeHeading()
+        self.logger.split() 
+        self.logger.includePrefix = True
     
     # fixes an ini file in a mod
     def fixIni(self, ini: IniFile, mod: Mod, fixedRemapBlends: Dict[str, RemapBlendModel]) -> bool:
         """
         Fixes an individual .ini file for a particular mod
 
         .. note:: 
@@ -3761,45 +4604,49 @@
             :raw-html:`<br />`
             The keys are the absolute filepath to the fixed RemapBlend.buf file and the values contains the data related
             to the fixed RemapBlend.buf file
 
         Returns
         -------
         :class:`bool`
-            Whether the particular .ini file has been fixed
+            Whether the particular .ini file has just been fixed
         """
 
-        # check if the .ini is for a raiden mod
-        if (ini is None or not ini.isRaidenIni):
+        # check if the .ini is belongs to some mod
+        if (ini is None or not ini.isModIni):
             return False
 
-        # parse the .ini file even if we are only undoing fixes for the case where a Blend.buf file
-        #   forms a bridge with some disconnected folder subtree of a mod
         if (self.undoOnly):
-            ini.parse()
             return True
 
         fileBaseName = os.path.basename(ini.file)
+        iniFullPath = FileService.absPathOfRelPath(ini.file, mod.path)
+
+        if (iniFullPath in self.inisSkipped):
+            self.logger.log(f"the ini file, {fileBaseName}, has alreaedy encountered an error")
+            return False
+        
+        if (iniFullPath in self.inisFixed):
+            self.logger.log(f"the ini file, {fileBaseName}, is already fixed")
+            return False
 
         # parse the .ini file
         self.logger.log(f"Parsing {fileBaseName}...")
         ini.parse()
-        if (ini.isRaidenFixed):
+        if (ini.isFixed):
             self.logger.log(f"the ini file, {fileBaseName}, is already fixed")
             return False
 
         # fix the blends
         self.logger.log(f"Fixing the {BlendFileType} files for {fileBaseName}...")
-        currentBlendsFound, currentBlendsFixed, currentBlendsSkipped = mod.correctBlend(fixedRemapBlends = fixedRemapBlends)
-        self.blendsFound += currentBlendsFound
+        currentBlendsFixed, currentBlendsSkipped = mod.correctBlend(fixedRemapBlends = fixedRemapBlends, skippedBlends = self.skippedBlends)
         self.blendsFixed = self.blendsFixed.union(currentBlendsFixed)
 
         if (currentBlendsSkipped):
-            self.skippedBlends[mod.path] = currentBlendsSkipped
-        self.skippedBlendsCount += len(currentBlendsSkipped)
+            self.skippedBlendsByMods[mod.path] = DictTools.combine(self.skippedBlendsByMods[mod.path], currentBlendsSkipped)
 
         # writing the fixed file
         self.logger.log(f"Making the fixed ini file for {fileBaseName}")
         ini.fix(keepBackup = self.keepBackups, fixOnly = self.fixOnly)
 
         return True
 
@@ -3821,56 +4668,61 @@
             :raw-html:`<br />` :raw-html:`<br />`
             The keys are the absolute filepath to the fixed RemapBlend.buf files and the values contains the data related
             to the fixed RemapBlend.buf file
 
         Returns
         -------
         :class:`bool`
-            Whether the particular mod has been fixed
+            Whether the particular mod has just been fixed
         """
 
         # remove any backups
         if (not self.keepBackups):
             mod.removeBackupInis()
 
         for ini in mod.inis:
-            ini.checkRaidenIni(mustBeRaiden = not self.readAllInis)
+            ini.checkIsMod()
 
         # undo any previous fixes
         if (not self.fixOnly):
-            mod.removeFix(self.blendsFixed, self.inisFixed, keepBackups = self.keepBackups)
+            undoedInis, removedRemapBlends = mod.removeFix(self.blendsFixed, self.inisFixed, self._visitedRemapBlendsAtRemoval, self.inisSkipped, keepBackups = self.keepBackups, fixOnly = self.fixOnly)
+            self.removedRemapBlends = self.removedRemapBlends.union(removedRemapBlends)
 
         result = False
         firstIniException = None
         inisLen = len(mod.inis)
 
         for i in range(inisLen):
             ini = mod.inis[i]
+            iniFullPath = FileService.absPathOfRelPath(ini.file, mod.path)
             iniIsFixed = False
 
             try:
                 iniIsFixed = self.fixIni(ini, mod, fixedRemapBlends)
-            except BaseException as e:
+            except Exception as e:
                 self.logger.handleException(e)
-                self.inisSkipped[ini.file] = e 
+                self.inisSkipped[iniFullPath] = e 
 
                 if (firstIniException is None):
                     firstIniException = e
 
+            if (firstIniException is None and iniFullPath in self.inisSkipped):
+                firstIniException = self.inisSkipped[iniFullPath]
+
             result = (result or iniIsFixed)
 
             if (not iniIsFixed):
                 continue
             
             if (i < inisLen - 1):
                 self.logger.space()
-            iniFullPath = FileService.absPathOfRelPath(ini.file, mod.path)
+
             self.inisFixed.add(iniFullPath)
-        
-        if (firstIniException is not None):
+
+        if (not result and firstIniException is not None):
             self.skippedMods[mod.path] = firstIniException
 
         return result
     
     def addTips(self):
         """
         Prints out any useful tips for the user to know
@@ -3885,45 +4737,45 @@
             if (self.keepBackups):
                 self.logger.bulletPoint(f'Hate deleting the "{BackupFilePrefix}" {IniExt}/{TxtExt} files yourself after running this script? (cuz I know I do!) Run this script again (on CMD) using the {DeleteBackupOpt} option')
 
             if (not self.undoOnly):
                 self.logger.bulletPoint(f"Want to undo this script's fix? Run this script again (on CMD) using the {RevertOpt} option")
 
             if (not self.readAllInis):
-                self.logger.bulletPoint(f"Were your {IniFileType}s not read because it does not contain the section named [TextureOverrideRaidenShogunBlend]? Run this script again (on CMD) using the {AllOpt} option")
+                self.logger.bulletPoint(f"Were your {IniFileType}s not read? Run this script again (on CMD) using the {AllOpt} option")
 
             self.logger.space()
             self.logger.log("For more info on command options, run this script (on CMD) using the --help option")
             self.logger.closeHeading()
 
         self.logger.includePrefix = True
 
 
-    def reportSkippedAsset(self, assetName: str, assetDict: Dict[str, BaseException], warnStrFunc: Callable[[str], str]):
+    def reportSkippedAsset(self, assetName: str, assetDict: Dict[str, Exception], warnStrFunc: Callable[[str], str]):
         """
         Prints out the exception message for why a particular .ini file or Blend.buf file has been skipped
 
         Parameters
         ----------
         assetName: :class:`str`
             The name for the type of asset (files, folders, mods, etc...) that was skipped
 
-        assetDict: Dict[:class:`str`, :class:`BaseException`]
+        assetDict: Dict[:class:`str`, :class:`Exception`]
             Locations of where exceptions have occured for the particular asset :raw-html:`<br />` :raw-html:`<br />`
 
             The keys are the absolute folder paths to where the exception occured
 
         wantStrFunc: Callable[[:class:`str`], :class:`str`]
             Function for how we want to print out the warning for each exception :raw-html:`<br />` :raw-html:`<br />`
 
             Takes in the folder location of where the exception occured as a parameter
         """
 
         if (assetDict):
-            message = f"WARNING: The following {assetName} were skipped due to warnings (see log above):\n\n"
+            message = f"\nWARNING: The following {assetName} were skipped due to warnings (see log above):\n\n"
             for dir in assetDict:
                 message += warnStrFunc(dir)
 
             self.logger.error(message)
             self.logger.space()
 
     def warnSkippedBlends(self, modPath: str):
@@ -3932,87 +4784,97 @@
 
         Parameters
         ----------
         modPath: :class:`str`
             The absolute path to a particular folder
         """
 
-        relModPath = FileService.getRelPath(modPath, self._path)
-        message = f"Mod: {relModPath}\n"
-        blendWarnings = self.skippedBlends[modPath]
+        parentFolder = os.path.dirname(self._path)
+        relModPath = FileService.getRelPath(modPath, parentFolder)
+        modHeading = Heading(f"Mod: {relModPath}", 5)
+        message = f"{modHeading.open()}\n\n"
+        blendWarnings = self.skippedBlendsByMods[modPath]
         
         for blendPath in blendWarnings:
             relBlendPath = FileService.getRelPath(blendPath, self._path)
-            message += self.logger.getBulletStr(f"{relBlendPath} >>> {blendWarnings[blendPath]}\n")
+            message += self.logger.getBulletStr(f"{relBlendPath}:\n\t{Heading(type(blendWarnings[blendPath]).__name__, 3, '-').open()}\n\t{blendWarnings[blendPath]}\n\n")
         
-        message += "\n"
+        message += f"{modHeading.close()}\n"
         return message
 
     def reportSkippedMods(self):
         """
         Prints out all of the mods that were skipped due to exceptions
 
         .. note:: 
             For more info about how we define a 'mod', go to :class:`Mod`
         """
 
-        self.reportSkippedAsset("mods", self.skippedMods, lambda dir: self.logger.getBulletStr(f"{dir} >>> {self.skippedMods[dir]}\n"))
-        self.reportSkippedAsset(f"{IniFileType}s", self.inisSkipped, lambda file: self.logger.getBulletStr(f"{file} >>> {self.inisSkipped[file]}\n"))
-        self.reportSkippedAsset(f"{BlendFileType} files", self.skippedBlends, lambda dir: self.warnSkippedBlends(dir))
+        self.reportSkippedAsset("mods", self.skippedMods, lambda dir: self.logger.getBulletStr(f"{dir}:\n\t{Heading(type(self.skippedMods[dir]).__name__, 3, '-').open()}\n\t{self.skippedMods[dir]}\n\n"))
+        self.reportSkippedAsset(f"{IniFileType}s", self.inisSkipped, lambda file: self.logger.getBulletStr(f"{file}:\n\t{Heading(type(self.inisSkipped[file]).__name__, 3, '-').open()}\n\t{self.inisSkipped[file]}\n\n"))
+        self.reportSkippedAsset(f"{BlendFileType} files", self.skippedBlendsByMods, lambda dir: self.warnSkippedBlends(dir))
 
     def reportSummary(self):
         skippedMods = len(self.skippedMods)
         foundMods = self.modsFixed + skippedMods
         fixedBlends = len(self.blendsFixed)
-        skippedBlends = self.blendsFound - fixedBlends
+        skippedBlends = len(self.skippedBlends)
+        foundBlends = fixedBlends + skippedBlends
         fixedInis = len(self.inisFixed)
         skippedInis = len(self.inisSkipped)
         foundInis = fixedInis + skippedInis
+        removedRemapBlends = len(self.removedRemapBlends)
 
         self.logger.openHeading("Summary", sideLen = 10)
         self.logger.space()
         
         modFixMsg = ""
         blendFixMsg = ""
         iniFixMsg = ""
+        removedRemappedMsg = ""
         if (not self.undoOnly):
             modFixMsg = f"Out of {foundMods} found mods, fixed {self.modsFixed} mods and skipped {skippedMods} mods"
             iniFixMsg = f"Out of the {foundInis} {IniFileType}s within the found mods, fixed {fixedInis} {IniFileType}s and skipped {skippedInis} {IniFileType} files"
-            blendFixMsg = f"Out of the {self.blendsFound} {BlendFileType} files within the found mods, fixed {fixedBlends} {BlendFileType} files and skipped {skippedBlends} {BlendFileType} files"
+            blendFixMsg = f"Out of the {foundBlends} {BlendFileType} files within the found mods, fixed {fixedBlends} {BlendFileType} files and skipped {skippedBlends} {BlendFileType} files"
         else:
             modFixMsg = f"Out of {foundMods} found mods, remove fix from {self.modsFixed} mods and skipped {skippedMods} mods"
 
+        if (not self.fixOnly and removedRemapBlends > 0):
+            removedRemappedMsg = f"Removed {removedRemapBlends} old {RemapBlendFile} files"
+
+
         self.logger.bulletPoint(modFixMsg)
         if (iniFixMsg):
             self.logger.bulletPoint(iniFixMsg)
 
         if (blendFixMsg):
             self.logger.bulletPoint(blendFixMsg)
 
+        if (removedRemappedMsg):
+            self.logger.bulletPoint(removedRemappedMsg)
+
         self.logger.space()
         self.logger.closeHeading()
 
     def createLog(self):
         """
         Creates a log text file that contains all the text printed on the command line
         """
 
-        if (not self.log):
+        if (self.log is None):
             return
 
         self.logger.includePrefix = False
         self.logger.space()
 
-        self.logger.verbose = True
         self.logger.log(f"Creating log file, {LogFile}")
 
         self.logger.includePrefix = True
-        self.logger.verbose = self.verbose
 
-        with open(self._logFile, "w", encoding = IniFileEncoding) as f:
+        with open(self.log, "w", encoding = IniFileEncoding) as f:
             f.write(self.logger.loggedTxt)
 
     def createMod(self, path: Optional[str] = None, files: Optional[List[str]] = None) -> Mod:
         """
         Creates a mod
 
         .. note:: 
@@ -4033,29 +4895,32 @@
         Returns
         -------
         :class:`Mod`
             The mod that has been created
         """
 
         path = FileService.getPath(path)
-        mod = Mod(path = path, files = files, logger = self.logger)
+        mod = Mod(path = path, files = files, logger = self.logger, types = self.types, defaultType = self.defaultType)
         return mod
 
     def _fix(self):
         """
         The overall logic for fixing a bunch of mods
 
         For finding out which folders may contain mods, this function:
-            #. recursively searches all folders from where the :attr:`RaidenBossFixService.path` is located
+            #. recursively searches all folders from where the :attr:`BossFixService.path` is located
             #. for every .ini file in a valid mod and every Blend.buf file encountered that is encountered, recursively search all the folders from where the .ini file or Blend.buf file is located
 
         .. note:: 
             For more info about how we define a 'mod', go to :class:`Mod`
         """
 
+        if (self.__errorsBeforeFix is not None):
+            raise self.__errorsBeforeFix
+
         if (self.fixOnly and self.undoOnly):
             raise ConflictingOptions([FixOnlyOpt, RevertOpt])
 
         parentFolder = os.path.dirname(self._path)
         self._loggerBasePrefix = os.path.basename(self._path)
         self.logger.prefix = os.path.basename(DefaultPath)
 
@@ -4088,15 +4953,15 @@
                 visitingDirs.remove(path)
                 visitedDirs.add(path)
                 continue
 
             # fix the mod
             try:
                 fixedMod = self.fixMod(mod, fixedRemapBlends)
-            except BaseException as e:
+            except Exception as e:
                 self.logger.handleException(e)
                 if (mod.inis):
                     self.skippedMods[path] = e
 
             # get all the folders that could potentially be other mods
             modFiles, modDirs = FileService.getFilesAndDirs(path = path, recursive = True)
 
@@ -4134,22 +4999,22 @@
         Fixes a bunch of mods
 
         see :meth:`_fix` for more info
         """
         
         try:
             self._fix()
-        except BaseException as e:
+        except Exception as e:
             if (self.handleExceptions):
                 self.logger.handleException(e)
             else:
                 self.createLog()
                 raise e from e
         else:
-            noErrors = bool(not self.skippedMods and not self.skippedBlends)
+            noErrors = bool(not self.skippedMods and not self.skippedBlendsByMods)
 
             if (noErrors):
                 self.logger.space()
                 self.logger.log("ENJOY")
 
             self.logger.split()
 
@@ -4157,16 +5022,19 @@
                 self.addTips()
 
         self.createLog()
 
 
 def main():
     args = argParser.parse_args()
-    raidenBossFixService = RaidenBossFixService(path = args.src, keepBackups = not args.deleteBackup, fixOnly = args.fixOnly, 
-                                                undoOnly = args.revert, readAllInis = args.all, 
-                                                log = args.log, verbose = True, handleExceptions = True)
-    raidenBossFixService.fix()
-    raidenBossFixService.logger.waitExit()
+    readAllInis = args.all
+    defaultType = args.defaultType
+
+    bossFixService = BossFixService(path = args.src, keepBackups = not args.deleteBackup, fixOnly = args.fixOnly, 
+                                    undoOnly = args.revert, readAllInis = readAllInis, types = args.types, defaultType = defaultType,
+                                    log = args.log, verbose = True, handleExceptions = True)
+    bossFixService.fix()
+    bossFixService.logger.waitExit()
 
 # Main Driver Code
 if __name__ == "__main__":
     main()
```

### Comparing `FixRaidenBoss2-3.6.1/src/FixRaidenBoss2/__init__.py` & `fixraidenboss2-3.7.0/src/FixRaidenBoss2/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,3 +1,3 @@
-from .FixRaidenBoss2 import RaidenBossFixService, Mod, IniFile, FileService, Logger, RemapBlendModel, Model, IfTemplate, Error, FileException, MissingFileException, DuplicateFileException, BlendFileNotRecognized, ConflictingOptions, ListTools, DictTools
+from .FixRaidenBoss2 import BossFixService, Mod, IniFile, FileService, Logger, RemapBlendModel, Model, IfTemplate, Error, FileException, MissingFileException, DuplicateFileException, BlendFileNotRecognized, ConflictingOptions, DictTools, Heading, ModType, ModTypes, NoModType, BadBlendData, RemapMissingBlendFile, InvalidModType
 
-__all__ = ["RaidenBossFixService", "Mod", "IniFile", "FileService", "Logger", "RemapBlendModel", "Model", "IfTemplate", "Error", "FileException", "MissingFileException", "DuplicateFileException", "BlendFileNotRecognized", "ConflictingOptions", "ListTools", "DictTools"]
+__all__ = ["BossFixService", "Mod", "IniFile", "FileService", "Logger", "RemapBlendModel", "Model", "IfTemplate", "Error", "FileException", "MissingFileException", "DuplicateFileException", "BlendFileNotRecognized", "ConflictingOptions", "DictTools", "Heading", "ModType", "ModTypes", "NoModType", "BadBlendData", "RemapMissingBlendFile", "InvalidModType"]
```

