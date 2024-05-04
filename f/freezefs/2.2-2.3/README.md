# Comparing `tmp/freezefs-2.2.tar.gz` & `tmp/freezefs-2.3.tar.gz`

## Comparing `freezefs-2.2.tar` & `freezefs-2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 freezefs-2.2/freezefs/__main__.py
--rw-r--r--   0        0        0    12119 2020-02-02 00:00:00.000000 freezefs-2.2/freezefs/archive.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 freezefs-2.2/freezefs/ffsextract.py
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 freezefs-2.2/freezefs/ffsmount.py
--rwxr-xr-x   0        0        0      198 2020-02-02 00:00:00.000000 freezefs-2.2/tests/cleantest (1).bat
--rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 freezefs-2.2/tests/runtest.bat
--rw-r--r--   0        0        0    19910 2020-02-02 00:00:00.000000 freezefs-2.2/tests/test.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 freezefs-2.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 freezefs-2.2/LICENSE
--rw-r--r--   0        0        0    15936 2020-02-02 00:00:00.000000 freezefs-2.2/README.md
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 freezefs-2.2/pyproject.toml
--rw-r--r--   0        0        0    17916 2020-02-02 00:00:00.000000 freezefs-2.2/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 freezefs-2.3/freezefs/__main__.py
+-rw-r--r--   0        0        0    12175 2020-02-02 00:00:00.000000 freezefs-2.3/freezefs/archive.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 freezefs-2.3/freezefs/ffsextract.py
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 freezefs-2.3/freezefs/ffsmount.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 freezefs-2.3/tests/cleantest.bat
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 freezefs-2.3/tests/runtest.bat
+-rw-r--r--   0        0        0    19910 2020-02-02 00:00:00.000000 freezefs-2.3/tests/test.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 freezefs-2.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 freezefs-2.3/LICENSE
+-rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 freezefs-2.3/README.md
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 freezefs-2.3/pyproject.toml
+-rw-r--r--   0        0        0    18740 2020-02-02 00:00:00.000000 freezefs-2.3/PKG-INFO
```

### Comparing `freezefs-2.2/freezefs/archive.py` & `freezefs-2.3/freezefs/archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,14 +200,15 @@
                         default="mount",
                         help="Action when importing output module. Default is mount.")
 
     parser.add_argument("--target", "-t", type=str,
                         dest="target",
                         help="For --on-import=mount: mount point."
                              " For --on-import=extract: destination folder."
+                             " Default: the infolder."
                              " Example: --target /myfiles. Must start with /")
                              
     parser.add_argument("--overwrite", "-ov", type=str,
                         dest="overwrite",
                         choices=["never", "always"],
                         default="never",
                         help="always: on extract, all files are overwritten. never: on extract, no file is overwritten, only new files are extracted. Default: never. ")
```

### Comparing `freezefs-2.2/freezefs/ffsextract.py` & `freezefs-2.3/freezefs/ffsextract.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,10 +93,10 @@
     module = __import__( module_name )
     if module_name != "__main__":
         del sys.modules[ module_name ]
     
     vp = _VerbosePrint( module_name, "extract", silent )
 
     vp.print( f"extracting files to {target}." )
-    _extract_all( module.direntries, target, overwrite, vp )
+    _extract_all( direntries, target, overwrite, vp )
             
     return
```

### Comparing `freezefs-2.2/freezefs/ffsmount.py` & `freezefs-2.3/freezefs/ffsmount.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         while ".." in parts:
             i = parts.index("..")
             if i > 1:
                 del parts[i]
                 del parts[i-1]
             else:
                 # Can't access /..
-                raise OSError( errno.EPERM )
+                self._raise_perm()
         # Solve ./file or /folder/./file
         while "." in parts:
             i = parts.index(".")
             del parts[i]
         filename = "".join( "/" + p for p in parts ).replace( "//", "/" )
         return filename
         
@@ -61,27 +61,30 @@
             # the root. Return folder direntry for the root.
             return None
         if filename in self.filedict:
             # Return the file directory entry (dir_entry)
             return self.filedict[filename]
         else:
             raise OSError( errno.ENOENT )
-
+    
+    def _raise_perm( self ):
+        raise OSError(errno.EPERM) # Very common here
+        
     def open( self, filename, mode, buffering=None ):
         # Validate mode before opening file
         for c in mode:
             # Modes may be "r"/"rt"/"tr" or "rb"/"br"
             if c not in "rbt":
                 raise OSError( errno.EINVAL )
             
         dir_entry = self._find_file( filename )
         if dir_entry is None: 
             # This is a folder or the root of this file system
             if filename == "/":
-                raise OSError( errno.EPERM )
+                self._raise_perm()
             raise OSError(errno.EISDIR)
             
         data = dir_entry[0] # data 
         if not dir_entry[1]: # compressed
             if "b" in mode:
                 return BytesIO( data )
             else:
@@ -146,28 +149,31 @@
         #sum_size = sum( d[2] for d in self.filedict.values() if d is not None )
         return (1,1,self.sum_size,  0,0,self.files_folders,  0,0,1, 255)
     
     def mount( self, readonly, x ):
         self.path = "/"
         
     def remove( self, filename ):
-        raise OSError( errno.EPERM )
+        self._raise_perm()
     
     def mkdir( self, *args ):
-        raise OSError( errno.EPERM )
+        self._raise_perm()
 
     def rename( self, oldfname, newfname ):
-        raise OSError( errno.EPERM )
+        self._raise_perm()
         
     def umount( self ):
         # No specific cleanup necessary on umount.
         pass
-
+    
+    # Added rmdir for completeness
+    def rmdir(self):
+        self._raise_perm()
+        
 def mount_fs( frozen_module_name, target, silent ):
-    module = __import__( frozen_module_name )
     
     if target is None:
         raise ValueError("No target specified")
 
     # Check target doesn't exist
     file_exists = False
     try:
@@ -177,9 +183,9 @@
         pass  
     if file_exists:
         raise OSError( errno.EEXIST )
     
     if not silent:
         print( f"mounting {__name__} at {target}." )
         
-    os.mount( VfsFrozen( module.direntries, module.sum_size, module.files_folders ), target, readonly=True )
+    os.mount( VfsFrozen( direntries, sum_size, files_folders ), target, readonly=True )
     return True
```

### Comparing `freezefs-2.2/tests/test.py` & `freezefs-2.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `freezefs-2.2/LICENSE` & `freezefs-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `freezefs-2.2/README.md` & `freezefs-2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 ## Purpose
 
 freezefs saves a file structure with subfolders and builds an self-extractable or self-mountable archive in a .py file, optionally with compression, to be frozen as bytecode or extracted.
 
 There are several ways to use freezefs:
 * Freeze the archive as frozen bytecode in a MicroPython image. Import the archive and it gets mounted as a read-only file system. The files continue to reside in the frozen image. 
 * Freeze the compressed archive as frozen bytecode in a MicroPython image. Import the archive once to extract the file structure to the flash file system. The purpose is to aid initial deployment of read/write files.
+
+These two options require RAM to import the archive:
 * Run a compressed .py archive with ```mpremote run```. The files get extracted to the microprocessor. This is a easy way to install many files at once, and it is quite fast.
 * Install a compressed .py archive with ```mpremote mip install``` and then import the file to extract all files. This aids in installing complete systems over-the-air (OTA). The file should be compiled with mpy-cross, to get all the gain from compression.
 
 Overall, it simplifies deploying text and binary files, such as MicroPython code, html pages, json data files, etc.
 
 
 ## Description
@@ -25,14 +27,15 @@
 ## Feedback
 Please report any problem or ask for support in the issues section. If it works for you, please star the repository.
 
 ## Installation
 
 Install the software with ```pip install freezefs```
 
+This installs the freezefs utility to be run on PC or MAC. The necessary MicroPython code is also installed on the PC or MAC and then automatically included in the output file.
 
 ## An example: freeze a files to a MicroPython image and mount file system
 Suppose you have the following folders, files and subfolders on your PC and want to freeze that together with your MicroPython programs in a MicroPython image:
 
 ```
 myfolder
     |
@@ -46,28 +49,27 @@
     |
     +---images
          |
          +---myimage.jpg
 ```
 The following command will archive the complete structure to the myfolder.py file:
 ```
-python -m freezefs  myfolder frozen_myfolder.py --target=/myfolder --on-import=mount
+python -m freezefs  myfolder frozen_myfolder.py 
 ```
-The frozen_myfolder.py will now contain all the files and folders, together with the code to mount this as a read only file system. To mount on the microcontroller, add this line to _boot.py, boot.py or main.py:
+The frozen_myfolder.py will now contain all the files and folders, together with the code to mount this as a read only file system. To mount on the microcontroller, add this line to  boot.py or main.py:
 ```
 import frozen_myfolder
 ```
 
-
-When booting up the microcontroller, and once ```import frozen_myfolder``` has been executed, the above file structure is automatically mounted (using ```os.mount()``` internally) at /myfolder, and the files and folders will appear under ```/myfolder``` on the microcontroller as read only files. The files are not copied to ```/myfolder```, but remain in the MicroPython image on flash. They now can be accessed with MicroPython statements such as ```open( "/myfolder/index.html", "r"), read(), readline(), open in "rb" or "r" mode, os.listdir("/myfolder")``` etc. If the import is in ```boot.py``` or ```_boot.py```, the files are also visible with ```mpremote ls```. The RAM overhead is low, and access speed is similar to regular flash files.
+When booting up the microcontroller, and once ```import frozen_myfolder``` has been executed, the above file structure is mounted (using ```os.mount()``` internally) at /myfolder, and the files and folders will appear under ```/myfolder``` on the microcontroller as read only files. The files are not copied to ```/myfolder```, but remain in the MicroPython image on flash. They now can be accessed with MicroPython statements such as ```open( "/myfolder/index.html", "r"), read(), readline(), open in "rb" or "r" mode, os.listdir("/myfolder")``` etc.  lsIf the import is in ```boot.py```, the files are also visible with ```mpremote ls```. The RAM overhead is low, and access speed is similar to regular flash files.
 
 ## Another example: create a self-extractable file archive
 Use:
 ```
-python -m freezefs  myfolder frozen_myfolder.py --target=/myfolder --on-import=extract --compress
+python -m freezefs  myfolder frozen_myfolder.py --on-import=extract --compress
 ```
 
 The frozen_myfolder.py will now contain all the files and folders compressed with zlib, together with the code to extract the files to the flash file system at ```/```. Optionally compile with ```mpy-cross frozen_myfolder.py``` to reduce file size. Have your code ```import frozen_myfolder```. This will decompress and extract (copy) the complete folder and subfolders to flash memory. On the next import, the files won't be overwritten (see ```--overwrite``` option).
 
 Importing or running the file, for example ```mpremote run frozen_myfolder``` will also extract all files. Since this is quite fast, this is aids deploying software.
 
 
@@ -95,15 +97,16 @@
   outfile               Path and name of output module. Must have .py extension.
 
 options:
   -h, --help            show this help message and exit
   --on-import {mount,extract}, -oi {mount,extract}
                         Action when importing output module. Default is mount.
   --target TARGET, -t TARGET
-                        For --on-import=mount: mount point. For --on-import=extract: destination folder.
+                        For --on-import=mount: mount point. For --on-import=extract: destination folder. 
+                        Default: the infolder.
                         Example: --target /myfiles. Must start with /
   --overwrite {never,always}, -ov {never,always}
                         always: on extract, all files are overwritten. never: on extract, no file is
                         overwritten, only new files are extracted. Default: never.
   --compress, --no-compress, -c
                         Compress files before writing to output .py. See python zlib compression. (default:
                         False)
@@ -114,63 +117,63 @@
   --silent, -s          Supress messages printed when mounting/copying files and while running this program.
 ```
 ### The infolder
 The input folder and subfolders contain the files to be archived in the output .py file. 
 
 
 ### The output .py file
-The outfile is overwritten with the MicroPython code with file contents (possibly compressed), file and folder names and the code to os.mount() or extract the files.
+The outfile is overwritten with the MicroPython code with file contents (possibly compressed), file and folder names and the code to mount the archive as file system or extract the files.
 
 
-### freezefs with --on-import mount (default)
+### freezefs with --on-import mount 
 
 With this option, the output .py module mounts its file system on import at the mount point (virtual folder) specified by --target as read-only files. 
 
-The purpose --on-import=mount option to enable mounting a file system frozen in bytecode in a MicroPython image. So the best use for this option is to put the .py output file or files into a manifest.py, generate the MicroPython image and load the image to a microcontroller. Add a import of the output .py file in the main.py or boot.py (or _boot.py) and the files get visible read only at the specified target.
+The purpose --on-import=mount option to enable mounting a file system frozen in bytecode in a MicroPython image. So the best use for this option is to put the .py output file or files into a manifest.py, generate the MicroPython image and load the image to a microcontroller. Add a import of the output .py file in the main.py or boot.py and the files get visible read only at the specified target.
 
 See section on RAM usage below for --on-import with --compress.
 
 
 ### freezefs with --on-import=extract
-This option is intended for use with --compress to deploy files to the regular flash file system.
+This option is intended for use with --compress to makme a self extractable .py file.
+
+To obtain maximum gain from compression, compile the .py with mpy-cross to a .mpy file.
 
 When importing or running this .py file on a MicroPython system, the file system gets decompressed and extracted.
 
 Also see --overwrite option.
 
-With the --on-import=extract option, the folder is not mounted but copied to the file system at
-
 ### --on-import=extract with --overwrite=never
 When extracting, each file that exists will be skipped. Only non-existing files will be extracted. Existing files will be never overwritten.
 
 
 
 ### --on-import=extract with --overwrite=always
 When extracting, existing files will be always overwritten.
 
 
 ### freezefs  --target
 For ```--on-import=mount``` this is the mount point on the file system of the microcontroller.
 
 For ```--on-import=export```, this is the destination folder on the file system of the microcontroller.
 
-Must start with /, i.e. must be a root folder. ```--target=/myfolder/subfolder```  is a valid target.
+Must start with /
 
-For ```--on-import=extract```, this can be ```--target=/``` to deploy files to the root folder, such as main.py.
+For ```--on-import=extract```, ```--target=/``` is used to deploy files to the root folder, such as main.py.
 
 If omitted, the last subfolder of the infolder is set as target, for example if the infolder is ```/myfolder/subfolder```, target will be set to ```/subfolder```.
 
 ### freezefs --compress
-This option compresses the files when packing them into the output .py files and decompresses them using deflate on the microcontroller.
+This option compresses the files when packing them into the output .py files and decompresses them using MicroPytnon ```deflate``` on the microcontroller.
 
 This option is best for use with --on-import=extract. It works with ```--on-import=mount```, but the RAM usage is high when opening text files with "r" mode. See section on RAM usage below.
 
 ### freezefs --compress, --wbits and --level options
 
- --wbits indicates the number of bytes used at any time for compressing (called the window size). The size of the window is 2\*\*WBITS, so --wbits=9 means windows size of 2\*\*9=512 bytes and --wbits=14 means 2\*\*14=16384 bytes. The higher the value, the better the compression, however, to decompress, up to 2\*\*WBITS bytes may needed on the microcontroller. 
+ --wbits indicates the number of bytes used at any time for compressing (called the window size). The size of the window is 2\*\*WBITS, so --wbits=9 means windows size of 2\*\*9=512 bytes and --wbits=14 means 2\*\*14=16384 bytes. The higher the value, the better the compression. However, to decompress, up to 2\*\*WBITS bytes may needed on the microcontroller. 
  
  --level goes from 0 (no compression) to 9 (highest compression). Level 9 is a bit slower to decompress.
  
  See Python docs for zlib and MicroPython docs for deflate for more details. 
  
 
 ### freezefs  --silent
@@ -178,20 +181,20 @@
 
 If an exception occurs during mount or extract, the exception will be raised independently of the --silent option.
 
 ## The frozen .py output file
 
 The output file of the freezefs  utility is a module with the frozen file system. This generated module contains consts with all the file data. MicroPython will access the file data directly in flash, if the .py file is frozen as bytecode in a MicroPython image. 
 
-The code for extract or mount is included in the file. When compiled to .mpy files, this code is about 1800 bytes for mount or 1300 bytes for extract.
+The code for extract or mount is included in the file. When compiled to .mpy files, the additional code amounts to about 1800 bytes for mount and 1300 bytes for extract.
 
 
 ### The mounted virtual file system
 
-freezefs implements a Virtual File System (VFS), included in the output file when using --on-import=mount
+freezefs implements a Virtual File System (VFS), with the driver included in the output file when using --on-import=mount
 
 The VFS implements ```os.mount```, ```os.umount```, ```os.chdir```, ```os.getcwd```, ```os.ilistdir```, ```os.listdir```, ```os.stat```, ```open```, ```close```, ```read```, ```readinto```, ```readline```, the iterator for reading lines and the decoding of UTF-8 format files to MicroPython strings.
 
 ```statvfs``` returns block size of 1. The file system size is the sum of all file sizes, without overhead. Mode flag is 1 (read only). The maximum file length is set to 255.
 
 ```open``` will only accept modes "r", "rt" and "rb". As usual, "r" will decode UTF-8 to strings, and "rb" will return bytes.
 
@@ -203,47 +206,52 @@
 
 If ```--compress``` was used, the files are decompressed on open while reading the stream. ```read()```, ```readinto()```, ```readline()```, ```readlines()``` are available. However, ```seek()``` and ```tell()``` are not available for compress. See also RAM usage below.
 
 ## RAM usage for --on-import=mount
 
 When frozen as bytecode in a MicroPython image, the RAM usage is low, about 1 kbyte.
 
-When using the --compress option, files opened with "r" (text mode) have to be decompressed in RAM, and the complete file gets loaded to RAM. This does not affect files opened with "rb" mode (binary mode), RAM usage is similar to opening a regular file system file.
+```---on-import=mount``` with ```--compress``` is  RAM intensive on the microcontroller. Files opened with "r" (text mode) have to be decompressed in RAM, and the complete file gets loaded to RAM. This does not affect files opened with "rb" mode (binary mode), RAM usage is similar to opening a regular file system file.
 
 When the .py file resides in the flash file system (as opposed to being frozen in the MicroPython image) the complete file is read to RAM, and it's now essentially a read only RAM disk. 
 
 ## RAM usage for --on-import=extract
 
 When frozen as bytecode in a MicroPython image, the RAM usage is very low while extracting. The buffer size to read/write is set at 256 bytes. 
 
 Compressed .py files will use up to 2\*\*WBITS bytes of RAM while decompressing. The --wbits option can be used to set this value if RAM is low. The higher the WBITS value, the better the compression.
 
-When extracting a .py archive residing in the flash file system (or on SD card), the .py file is best compiled with mpy-cross to a .mpy to have the best gain in size. The complete file will be loaded to RAM. To get that memory back once the extract is done, use ```__import__("module-name")```, without assigning the result of ```__import__``` to a variable. The extract driver will delete the itself from the ```sys.modules[]``` list, so the next garbage collection will free the memory.
-
+When extracting a .py archive residing in the flash file system (or on SD card), the .py file is best compiled with mpy-cross to a .mpy to have the best gain in size. The complete .py (or .mpy) file will be loaded to RAM. To get that memory back once the extract is done, use ```__import__("module-name")```, without assigning the result of ```__import__``` to a variable. The extract driver will delete the itself from the ```sys.modules[]``` list, so the next garbage collection will free the memory.
 
 ## Unit tests
 
 The /tests folder on github has unit tests.
 
 
 ## Dependencies
 
 These standard MicroPython libraries are needed: sys, os, io.BytesIO, io.StringIO, collections.OrderedDict and errno.  If --compress is used, deflate is needed. Deflate is present in MicroPython 1.20 or later.
 
 Python 3.10 or later must be installed on the PC. Probably earlier versions of Python will work too. pahtlib is used to be platform independent.
 
 The code is MicroPython/Python only, no C/C++ code. There are no processor or board specific dependencies.
 
-#  Changes fron version 1 
+# Restrictions
+
+While a freezefs filesystem is mounted, ```os.sync()``` may crash the microcontroller, raise a TypeError, or it may even appear to work. ```os.sync()``` cannot be used with freezefs.
+
+If you are using ```os.sync()``` and want to use freezefs, you may consider dropping ```os.sync()``` altogether. See MicroPython issue #11449 (https://github.com/micropython/micropython/issues/11449). On most architectures and filesystems (including ESP32, RP2040 and LittleFS2), ```os.sync()``` is a no-op (at lest for MicroPython up to version 1.23). Verify that for you case ```os.sync()``` really does something.
+
+#  Changes since version 1 
 Version number 2. If you are using version 1, please regenerate the output .py files with the new version of freezefs as they are incompatible.
 
 Added --compress and --overwrite switches. Drivers for extracting and mounting are now included in the compressed file, no need to install drivers. freezefs is now pip installable.
 
 ## Compatibility with MicroPython/Python versions
-Tested with MicroPython 1.20 and Python 3.10.7 and 3.11.4.
+Tested with MicroPython 1.20 to 1.22 and Python 3.10.7 and 3.11.4.
 
 ## Copyright and license
 Source code and documentation Copyright (c) 2023 Hermann Paul von Borries.
 
 This software and documentation is licensed according to the MIT license:
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `freezefs-2.2/pyproject.toml` & `freezefs-2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "freezefs"
-version = "2.2"
+version = "2.3"
 authors = [
   { name="Hermann von Borries", email="bixb922@gmail.com" }
 ]
 description = "freezefs - Create self-mounting or self-extracting compressed archives for MicroPython"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
@@ -23,11 +23,11 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: MicroPython",
     "Topic :: Desktop Environment :: File Managers"
  ]
 
 [project.urls]
-"Homepage" = "https://github.com/bixb922/freezeFS"
-"Bug Tracker" = "https://github.com/bixb922/freezeFS/issues"
+"Homepage" = "https://github.com/bixb922/freezefs"
+"Bug Tracker" = "https://github.com/bixb922/freezefs/issues"
 "Blog" = "https://solazyasueto.blogspot.com"
```

### Comparing `freezefs-2.2/PKG-INFO` & `freezefs-2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: freezefs
-Version: 2.2
+Version: 2.3
 Summary: freezefs - Create self-mounting or self-extracting compressed archives for MicroPython
-Project-URL: Homepage, https://github.com/bixb922/freezeFS
-Project-URL: Bug Tracker, https://github.com/bixb922/freezeFS/issues
+Project-URL: Homepage, https://github.com/bixb922/freezefs
+Project-URL: Bug Tracker, https://github.com/bixb922/freezefs/issues
 Project-URL: Blog, https://solazyasueto.blogspot.com
 Author-email: Hermann von Borries <bixb922@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 bixb922
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,14 +46,16 @@
 ## Purpose
 
 freezefs saves a file structure with subfolders and builds an self-extractable or self-mountable archive in a .py file, optionally with compression, to be frozen as bytecode or extracted.
 
 There are several ways to use freezefs:
 * Freeze the archive as frozen bytecode in a MicroPython image. Import the archive and it gets mounted as a read-only file system. The files continue to reside in the frozen image. 
 * Freeze the compressed archive as frozen bytecode in a MicroPython image. Import the archive once to extract the file structure to the flash file system. The purpose is to aid initial deployment of read/write files.
+
+These two options require RAM to import the archive:
 * Run a compressed .py archive with ```mpremote run```. The files get extracted to the microprocessor. This is a easy way to install many files at once, and it is quite fast.
 * Install a compressed .py archive with ```mpremote mip install``` and then import the file to extract all files. This aids in installing complete systems over-the-air (OTA). The file should be compiled with mpy-cross, to get all the gain from compression.
 
 Overall, it simplifies deploying text and binary files, such as MicroPython code, html pages, json data files, etc.
 
 
 ## Description
@@ -68,14 +70,15 @@
 ## Feedback
 Please report any problem or ask for support in the issues section. If it works for you, please star the repository.
 
 ## Installation
 
 Install the software with ```pip install freezefs```
 
+This installs the freezefs utility to be run on PC or MAC. The necessary MicroPython code is also installed on the PC or MAC and then automatically included in the output file.
 
 ## An example: freeze a files to a MicroPython image and mount file system
 Suppose you have the following folders, files and subfolders on your PC and want to freeze that together with your MicroPython programs in a MicroPython image:
 
 ```
 myfolder
     |
@@ -89,28 +92,27 @@
     |
     +---images
          |
          +---myimage.jpg
 ```
 The following command will archive the complete structure to the myfolder.py file:
 ```
-python -m freezefs  myfolder frozen_myfolder.py --target=/myfolder --on-import=mount
+python -m freezefs  myfolder frozen_myfolder.py 
 ```
-The frozen_myfolder.py will now contain all the files and folders, together with the code to mount this as a read only file system. To mount on the microcontroller, add this line to _boot.py, boot.py or main.py:
+The frozen_myfolder.py will now contain all the files and folders, together with the code to mount this as a read only file system. To mount on the microcontroller, add this line to  boot.py or main.py:
 ```
 import frozen_myfolder
 ```
 
-
-When booting up the microcontroller, and once ```import frozen_myfolder``` has been executed, the above file structure is automatically mounted (using ```os.mount()``` internally) at /myfolder, and the files and folders will appear under ```/myfolder``` on the microcontroller as read only files. The files are not copied to ```/myfolder```, but remain in the MicroPython image on flash. They now can be accessed with MicroPython statements such as ```open( "/myfolder/index.html", "r"), read(), readline(), open in "rb" or "r" mode, os.listdir("/myfolder")``` etc. If the import is in ```boot.py``` or ```_boot.py```, the files are also visible with ```mpremote ls```. The RAM overhead is low, and access speed is similar to regular flash files.
+When booting up the microcontroller, and once ```import frozen_myfolder``` has been executed, the above file structure is mounted (using ```os.mount()``` internally) at /myfolder, and the files and folders will appear under ```/myfolder``` on the microcontroller as read only files. The files are not copied to ```/myfolder```, but remain in the MicroPython image on flash. They now can be accessed with MicroPython statements such as ```open( "/myfolder/index.html", "r"), read(), readline(), open in "rb" or "r" mode, os.listdir("/myfolder")``` etc.  lsIf the import is in ```boot.py```, the files are also visible with ```mpremote ls```. The RAM overhead is low, and access speed is similar to regular flash files.
 
 ## Another example: create a self-extractable file archive
 Use:
 ```
-python -m freezefs  myfolder frozen_myfolder.py --target=/myfolder --on-import=extract --compress
+python -m freezefs  myfolder frozen_myfolder.py --on-import=extract --compress
 ```
 
 The frozen_myfolder.py will now contain all the files and folders compressed with zlib, together with the code to extract the files to the flash file system at ```/```. Optionally compile with ```mpy-cross frozen_myfolder.py``` to reduce file size. Have your code ```import frozen_myfolder```. This will decompress and extract (copy) the complete folder and subfolders to flash memory. On the next import, the files won't be overwritten (see ```--overwrite``` option).
 
 Importing or running the file, for example ```mpremote run frozen_myfolder``` will also extract all files. Since this is quite fast, this is aids deploying software.
 
 
@@ -138,15 +140,16 @@
   outfile               Path and name of output module. Must have .py extension.
 
 options:
   -h, --help            show this help message and exit
   --on-import {mount,extract}, -oi {mount,extract}
                         Action when importing output module. Default is mount.
   --target TARGET, -t TARGET
-                        For --on-import=mount: mount point. For --on-import=extract: destination folder.
+                        For --on-import=mount: mount point. For --on-import=extract: destination folder. 
+                        Default: the infolder.
                         Example: --target /myfiles. Must start with /
   --overwrite {never,always}, -ov {never,always}
                         always: on extract, all files are overwritten. never: on extract, no file is
                         overwritten, only new files are extracted. Default: never.
   --compress, --no-compress, -c
                         Compress files before writing to output .py. See python zlib compression. (default:
                         False)
@@ -157,63 +160,63 @@
   --silent, -s          Supress messages printed when mounting/copying files and while running this program.
 ```
 ### The infolder
 The input folder and subfolders contain the files to be archived in the output .py file. 
 
 
 ### The output .py file
-The outfile is overwritten with the MicroPython code with file contents (possibly compressed), file and folder names and the code to os.mount() or extract the files.
+The outfile is overwritten with the MicroPython code with file contents (possibly compressed), file and folder names and the code to mount the archive as file system or extract the files.
 
 
-### freezefs with --on-import mount (default)
+### freezefs with --on-import mount 
 
 With this option, the output .py module mounts its file system on import at the mount point (virtual folder) specified by --target as read-only files. 
 
-The purpose --on-import=mount option to enable mounting a file system frozen in bytecode in a MicroPython image. So the best use for this option is to put the .py output file or files into a manifest.py, generate the MicroPython image and load the image to a microcontroller. Add a import of the output .py file in the main.py or boot.py (or _boot.py) and the files get visible read only at the specified target.
+The purpose --on-import=mount option to enable mounting a file system frozen in bytecode in a MicroPython image. So the best use for this option is to put the .py output file or files into a manifest.py, generate the MicroPython image and load the image to a microcontroller. Add a import of the output .py file in the main.py or boot.py and the files get visible read only at the specified target.
 
 See section on RAM usage below for --on-import with --compress.
 
 
 ### freezefs with --on-import=extract
-This option is intended for use with --compress to deploy files to the regular flash file system.
+This option is intended for use with --compress to makme a self extractable .py file.
+
+To obtain maximum gain from compression, compile the .py with mpy-cross to a .mpy file.
 
 When importing or running this .py file on a MicroPython system, the file system gets decompressed and extracted.
 
 Also see --overwrite option.
 
-With the --on-import=extract option, the folder is not mounted but copied to the file system at
-
 ### --on-import=extract with --overwrite=never
 When extracting, each file that exists will be skipped. Only non-existing files will be extracted. Existing files will be never overwritten.
 
 
 
 ### --on-import=extract with --overwrite=always
 When extracting, existing files will be always overwritten.
 
 
 ### freezefs  --target
 For ```--on-import=mount``` this is the mount point on the file system of the microcontroller.
 
 For ```--on-import=export```, this is the destination folder on the file system of the microcontroller.
 
-Must start with /, i.e. must be a root folder. ```--target=/myfolder/subfolder```  is a valid target.
+Must start with /
 
-For ```--on-import=extract```, this can be ```--target=/``` to deploy files to the root folder, such as main.py.
+For ```--on-import=extract```, ```--target=/``` is used to deploy files to the root folder, such as main.py.
 
 If omitted, the last subfolder of the infolder is set as target, for example if the infolder is ```/myfolder/subfolder```, target will be set to ```/subfolder```.
 
 ### freezefs --compress
-This option compresses the files when packing them into the output .py files and decompresses them using deflate on the microcontroller.
+This option compresses the files when packing them into the output .py files and decompresses them using MicroPytnon ```deflate``` on the microcontroller.
 
 This option is best for use with --on-import=extract. It works with ```--on-import=mount```, but the RAM usage is high when opening text files with "r" mode. See section on RAM usage below.
 
 ### freezefs --compress, --wbits and --level options
 
- --wbits indicates the number of bytes used at any time for compressing (called the window size). The size of the window is 2\*\*WBITS, so --wbits=9 means windows size of 2\*\*9=512 bytes and --wbits=14 means 2\*\*14=16384 bytes. The higher the value, the better the compression, however, to decompress, up to 2\*\*WBITS bytes may needed on the microcontroller. 
+ --wbits indicates the number of bytes used at any time for compressing (called the window size). The size of the window is 2\*\*WBITS, so --wbits=9 means windows size of 2\*\*9=512 bytes and --wbits=14 means 2\*\*14=16384 bytes. The higher the value, the better the compression. However, to decompress, up to 2\*\*WBITS bytes may needed on the microcontroller. 
  
  --level goes from 0 (no compression) to 9 (highest compression). Level 9 is a bit slower to decompress.
  
  See Python docs for zlib and MicroPython docs for deflate for more details. 
  
 
 ### freezefs  --silent
@@ -221,20 +224,20 @@
 
 If an exception occurs during mount or extract, the exception will be raised independently of the --silent option.
 
 ## The frozen .py output file
 
 The output file of the freezefs  utility is a module with the frozen file system. This generated module contains consts with all the file data. MicroPython will access the file data directly in flash, if the .py file is frozen as bytecode in a MicroPython image. 
 
-The code for extract or mount is included in the file. When compiled to .mpy files, this code is about 1800 bytes for mount or 1300 bytes for extract.
+The code for extract or mount is included in the file. When compiled to .mpy files, the additional code amounts to about 1800 bytes for mount and 1300 bytes for extract.
 
 
 ### The mounted virtual file system
 
-freezefs implements a Virtual File System (VFS), included in the output file when using --on-import=mount
+freezefs implements a Virtual File System (VFS), with the driver included in the output file when using --on-import=mount
 
 The VFS implements ```os.mount```, ```os.umount```, ```os.chdir```, ```os.getcwd```, ```os.ilistdir```, ```os.listdir```, ```os.stat```, ```open```, ```close```, ```read```, ```readinto```, ```readline```, the iterator for reading lines and the decoding of UTF-8 format files to MicroPython strings.
 
 ```statvfs``` returns block size of 1. The file system size is the sum of all file sizes, without overhead. Mode flag is 1 (read only). The maximum file length is set to 255.
 
 ```open``` will only accept modes "r", "rt" and "rb". As usual, "r" will decode UTF-8 to strings, and "rb" will return bytes.
 
@@ -246,47 +249,52 @@
 
 If ```--compress``` was used, the files are decompressed on open while reading the stream. ```read()```, ```readinto()```, ```readline()```, ```readlines()``` are available. However, ```seek()``` and ```tell()``` are not available for compress. See also RAM usage below.
 
 ## RAM usage for --on-import=mount
 
 When frozen as bytecode in a MicroPython image, the RAM usage is low, about 1 kbyte.
 
-When using the --compress option, files opened with "r" (text mode) have to be decompressed in RAM, and the complete file gets loaded to RAM. This does not affect files opened with "rb" mode (binary mode), RAM usage is similar to opening a regular file system file.
+```---on-import=mount``` with ```--compress``` is  RAM intensive on the microcontroller. Files opened with "r" (text mode) have to be decompressed in RAM, and the complete file gets loaded to RAM. This does not affect files opened with "rb" mode (binary mode), RAM usage is similar to opening a regular file system file.
 
 When the .py file resides in the flash file system (as opposed to being frozen in the MicroPython image) the complete file is read to RAM, and it's now essentially a read only RAM disk. 
 
 ## RAM usage for --on-import=extract
 
 When frozen as bytecode in a MicroPython image, the RAM usage is very low while extracting. The buffer size to read/write is set at 256 bytes. 
 
 Compressed .py files will use up to 2\*\*WBITS bytes of RAM while decompressing. The --wbits option can be used to set this value if RAM is low. The higher the WBITS value, the better the compression.
 
-When extracting a .py archive residing in the flash file system (or on SD card), the .py file is best compiled with mpy-cross to a .mpy to have the best gain in size. The complete file will be loaded to RAM. To get that memory back once the extract is done, use ```__import__("module-name")```, without assigning the result of ```__import__``` to a variable. The extract driver will delete the itself from the ```sys.modules[]``` list, so the next garbage collection will free the memory.
-
+When extracting a .py archive residing in the flash file system (or on SD card), the .py file is best compiled with mpy-cross to a .mpy to have the best gain in size. The complete .py (or .mpy) file will be loaded to RAM. To get that memory back once the extract is done, use ```__import__("module-name")```, without assigning the result of ```__import__``` to a variable. The extract driver will delete the itself from the ```sys.modules[]``` list, so the next garbage collection will free the memory.
 
 ## Unit tests
 
 The /tests folder on github has unit tests.
 
 
 ## Dependencies
 
 These standard MicroPython libraries are needed: sys, os, io.BytesIO, io.StringIO, collections.OrderedDict and errno.  If --compress is used, deflate is needed. Deflate is present in MicroPython 1.20 or later.
 
 Python 3.10 or later must be installed on the PC. Probably earlier versions of Python will work too. pahtlib is used to be platform independent.
 
 The code is MicroPython/Python only, no C/C++ code. There are no processor or board specific dependencies.
 
-#  Changes fron version 1 
+# Restrictions
+
+While a freezefs filesystem is mounted, ```os.sync()``` may crash the microcontroller, raise a TypeError, or it may even appear to work. ```os.sync()``` cannot be used with freezefs.
+
+If you are using ```os.sync()``` and want to use freezefs, you may consider dropping ```os.sync()``` altogether. See MicroPython issue #11449 (https://github.com/micropython/micropython/issues/11449). On most architectures and filesystems (including ESP32, RP2040 and LittleFS2), ```os.sync()``` is a no-op (at lest for MicroPython up to version 1.23). Verify that for you case ```os.sync()``` really does something.
+
+#  Changes since version 1 
 Version number 2. If you are using version 1, please regenerate the output .py files with the new version of freezefs as they are incompatible.
 
 Added --compress and --overwrite switches. Drivers for extracting and mounting are now included in the compressed file, no need to install drivers. freezefs is now pip installable.
 
 ## Compatibility with MicroPython/Python versions
-Tested with MicroPython 1.20 and Python 3.10.7 and 3.11.4.
+Tested with MicroPython 1.20 to 1.22 and Python 3.10.7 and 3.11.4.
 
 ## Copyright and license
 Source code and documentation Copyright (c) 2023 Hermann Paul von Borries.
 
 This software and documentation is licensed according to the MIT license:
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

