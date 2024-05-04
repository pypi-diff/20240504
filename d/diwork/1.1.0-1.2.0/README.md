# Comparing `tmp/diwork-1.1.0.tar.gz` & `tmp/diwork-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diwork-1.1.0.tar", last modified: Sat May  4 10:02:21 2024, max compression
+gzip compressed data, was "diwork-1.2.0.tar", last modified: Sat May  4 11:41:51 2024, max compression
```

## Comparing `diwork-1.1.0.tar` & `diwork-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 10:02:21.072634 diwork-1.1.0/
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2023-02-10 11:11:21.000000 diwork-1.1.0/LICENSE
--rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-04 10:02:21.071634 diwork-1.1.0/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      211 2024-05-04 08:36:38.000000 diwork-1.1.0/README.md
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 10:02:21.069634 diwork-1.1.0/diwork/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      343 2024-05-04 08:22:40.000000 diwork-1.1.0/diwork/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      115 2024-05-04 08:01:22.000000 diwork-1.1.0/diwork/__main__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)       47 2024-05-04 08:33:46.000000 diwork-1.1.0/diwork/__version__.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 10:02:21.071634 diwork-1.1.0/diwork/diwork_mains/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      734 2024-05-04 08:48:21.000000 diwork-1.1.0/diwork/diwork_mains/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5734 2023-05-08 08:27:25.000000 diwork-1.1.0/diwork/diwork_mains/diwork_archive.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5032 2024-05-04 08:53:21.000000 diwork-1.1.0/diwork/diwork_mains/diwork_clone.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     7521 2023-03-17 19:19:40.000000 diwork-1.1.0/diwork/diwork_mains/diwork_diff.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     4099 2024-05-04 10:01:13.000000 diwork-1.1.0/diwork/diwork_mains/diwork_diffclone.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     3241 2023-02-18 08:20:12.000000 diwork-1.1.0/diwork/diwork_mains/diwork_difx.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     9181 2023-04-11 08:18:44.000000 diwork-1.1.0/diwork/diwork_mains/diwork_exec.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5170 2023-03-23 06:31:31.000000 diwork-1.1.0/diwork/diwork_mains/diwork_hash.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      582 2023-02-18 08:13:38.000000 diwork-1.1.0/diwork/diwork_mains/diwork_help.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     2900 2023-03-09 08:12:58.000000 diwork-1.1.0/diwork/diwork_mains/diwork_repeats.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     9064 2023-03-09 21:18:05.000000 diwork-1.1.0/diwork/diwork_mains/diwork_sshclone.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 10:02:21.071634 diwork-1.1.0/diwork/diwork_ways/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      571 2024-05-04 09:30:24.000000 diwork-1.1.0/diwork/diwork_ways/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      982 2023-02-17 14:44:34.000000 diwork-1.1.0/diwork/diwork_ways/diwork_parse.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)    10791 2024-05-04 09:52:54.000000 diwork-1.1.0/diwork/diwork_ways/diwork_sup.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1390 2024-05-04 09:37:47.000000 diwork-1.1.0/diwork/main.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 10:02:21.071634 diwork-1.1.0/diwork.egg-info/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-04 10:02:21.000000 diwork-1.1.0/diwork.egg-info/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      795 2024-05-04 10:02:21.000000 diwork-1.1.0/diwork.egg-info/SOURCES.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-05-04 10:02:21.000000 diwork-1.1.0/diwork.egg-info/dependency_links.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       44 2024-05-04 10:02:21.000000 diwork-1.1.0/diwork.egg-info/entry_points.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       14 2024-05-04 10:02:21.000000 diwork-1.1.0/diwork.egg-info/requires.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        7 2024-05-04 10:02:21.000000 diwork-1.1.0/diwork.egg-info/top_level.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       81 2024-05-04 07:49:04.000000 diwork-1.1.0/pyproject.toml
--rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-05-04 10:02:21.072634 diwork-1.1.0/setup.cfg
--rw-r--r--   0 the220th  (1000) the220th  (1000)      997 2024-05-04 08:57:56.000000 diwork-1.1.0/setup.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 11:41:51.233725 diwork-1.2.0/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2023-02-10 11:11:21.000000 diwork-1.2.0/LICENSE
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-04 11:41:51.233725 diwork-1.2.0/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      211 2024-05-04 08:36:38.000000 diwork-1.2.0/README.md
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 11:41:51.230726 diwork-1.2.0/diwork/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      343 2024-05-04 08:22:40.000000 diwork-1.2.0/diwork/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      115 2024-05-04 08:01:22.000000 diwork-1.2.0/diwork/__main__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       47 2024-05-04 10:36:20.000000 diwork-1.2.0/diwork/__version__.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 11:41:51.232725 diwork-1.2.0/diwork/diwork_mains/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      734 2024-05-04 08:48:21.000000 diwork-1.2.0/diwork/diwork_mains/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5693 2024-05-04 10:26:10.000000 diwork-1.2.0/diwork/diwork_mains/diwork_archive.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5116 2024-05-04 10:48:42.000000 diwork-1.2.0/diwork/diwork_mains/diwork_clone.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     7521 2023-03-17 19:19:40.000000 diwork-1.2.0/diwork/diwork_mains/diwork_diff.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5755 2024-05-04 11:39:18.000000 diwork-1.2.0/diwork/diwork_mains/diwork_diffclone.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     3241 2023-02-18 08:20:12.000000 diwork-1.2.0/diwork/diwork_mains/diwork_difx.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     9181 2023-04-11 08:18:44.000000 diwork-1.2.0/diwork/diwork_mains/diwork_exec.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5174 2024-05-04 10:36:42.000000 diwork-1.2.0/diwork/diwork_mains/diwork_hash.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      582 2023-02-18 08:13:38.000000 diwork-1.2.0/diwork/diwork_mains/diwork_help.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     2900 2023-03-09 08:12:58.000000 diwork-1.2.0/diwork/diwork_mains/diwork_repeats.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     9064 2023-03-09 21:18:05.000000 diwork-1.2.0/diwork/diwork_mains/diwork_sshclone.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 11:41:51.232725 diwork-1.2.0/diwork/diwork_ways/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      583 2024-05-04 10:44:35.000000 diwork-1.2.0/diwork/diwork_ways/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1033 2024-05-04 10:29:33.000000 diwork-1.2.0/diwork/diwork_ways/diwork_parse.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)    10915 2024-05-04 11:35:31.000000 diwork-1.2.0/diwork/diwork_ways/diwork_sup.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1390 2024-05-04 10:12:20.000000 diwork-1.2.0/diwork/main.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 11:41:51.233725 diwork-1.2.0/diwork.egg-info/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-04 11:41:51.000000 diwork-1.2.0/diwork.egg-info/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      795 2024-05-04 11:41:51.000000 diwork-1.2.0/diwork.egg-info/SOURCES.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-05-04 11:41:51.000000 diwork-1.2.0/diwork.egg-info/dependency_links.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       44 2024-05-04 11:41:51.000000 diwork-1.2.0/diwork.egg-info/entry_points.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       14 2024-05-04 11:41:51.000000 diwork-1.2.0/diwork.egg-info/requires.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        7 2024-05-04 11:41:51.000000 diwork-1.2.0/diwork.egg-info/top_level.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       81 2024-05-04 07:49:04.000000 diwork-1.2.0/pyproject.toml
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-05-04 11:41:51.233725 diwork-1.2.0/setup.cfg
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      997 2024-05-04 08:57:56.000000 diwork-1.2.0/setup.py
```

### Comparing `diwork-1.1.0/LICENSE` & `diwork-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diwork-1.1.0/diwork/diwork_mains/__init__.py` & `diwork-1.2.0/diwork/diwork_mains/__init__.py`

 * *Files identical despite different names*

### Comparing `diwork-1.1.0/diwork/diwork_mains/diwork_archive.py` & `diwork-1.2.0/diwork/diwork_mains/diwork_archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,18 @@
                 pout(f"{cur_iter} ({gi}/{gN}) Hash \"{hash_i}\" have file \"{file_i}\" ({get_nice_size(size_i)}). ")
             else:
                 pout(f"({gi}/{gN}) Hash \"{hash_i}\" have file \"{file_i}\" ({get_nice_size(size_i)}). ")
             zfd.write(file_i, f"{folder_path_name}/{file_rel_i}")
         d["folder_hash"] = hash_files = get_hash_of_hashes(sorted(d["hashes"].values()))
         d["folder_size"] = sum(d["sizes"].values())
         d["date"] = get_time_str()
-        d["hash_mode"] = Global.hash_mode
         d["legacy_version"] = legacy_version # if calculating hash will be changed or changed other things, this needed change too (increment)
         zfd.writestr("archive_info.json", json.dumps(d).encode("utf-8"))
     
-    return (errors, ) # TODO: errors
+    return (errors, )  # TODO: errors
 
 def process_if_zip_exists(zip_path: str) -> int:
     """ 0=override,    1=skip """
     while(True):
         pout(f"File \"{zip_path}\" already exists. Override this?")
         pout("Type \"yes\" in capital letter to override or \"no\" to skip. \n> ", endl=False)
         user_in = input()
```

### Comparing `diwork-1.1.0/diwork/diwork_mains/diwork_clone.py` & `diwork-1.2.0/diwork/diwork_mains/diwork_clone.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 def main_clone(args: list):
     parser = argparse.ArgumentParser(prog = "diwork clone",
         description="This module will clone all the contents of {folder_src} to {folder_dest}. As a result, {folder_src} and {folder_dest} will be completely identical.")
     parser.add_argument("folder_src", type=str, nargs=1,
                        help="Path to source directory")
     parser.add_argument("folder_dest", type=str, nargs=1,
                        help="Path to destination directory")
-    parser.add_argument("--symlink_mode", type=int, choices=[0,1,2], default=2, required=False,
-                       help="What to do with links: 0 - ignor, 1 - consider link content, 2 - use the file where the link refers to. Default 2.")
+    # parser.add_argument("--symlink_mode", type=int, choices=[0,1,2], default=2, required=False,
+    #                    help="What to do with links: 0 - ignor, 1 - consider link content, 2 - use the file where the link refers to. Default 2.")
     parser.add_argument("--copy_mode", type=int, choices=[0,1], default=0, required=False,
                        help="How to copy files: 0 - python shutil, 1 - system cp (copy). Default 0.")
     parser = common_init_parser(parser)
     args = parser.parse_args(args)
     common_init_parse(args)
     
     folder1 = args.folder_src[0]
@@ -106,17 +106,19 @@
             else:
                 pout(f"Failed successfully. symlink_mode={symlink_mode}, cannot understand it. ")
                 exit()
         else:
             pout(f"({gi}/{N}) Copying \"{file_i_rel}\"... ")
             cp(file_i_1, file_i_2, copy_mode)
     if(copy_mode == 0):
-        os.sync()
+        if sys.platform != "win32":
+            os.sync()
     elif(copy_mode == 1):
-        exe("sync")
+        if sys.platform != "win32":
+            exe("sync")
     else:
         pass
 
     if(len(err_out) != 0):
         pout(f"\n===============\nSome troubles happened:")
         for err_i in err_out:
             pout(f"\t{err_i}")
```

### Comparing `diwork-1.1.0/diwork/diwork_mains/diwork_diff.py` & `diwork-1.2.0/diwork/diwork_mains/diwork_diff.py`

 * *Files identical despite different names*

### Comparing `diwork-1.1.0/diwork/diwork_mains/diwork_diffclone.py` & `diwork-1.2.0/diwork/diwork_mains/diwork_diffclone.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,45 +18,47 @@
     for file_i in tqdm(files):
         file_i_rel = os.path.relpath(file_i, dir_path)
         d[file_i_rel] = get_hash_file(file_i)
     return d
 
 
 def main_diffclone(args: list):
+    platform = sys.platform
     parser = argparse.ArgumentParser(prog = "diwork diffclone",
         description="This module will clone all the contents of {folder_src} to {folder_dest}, but only files, which does not already contains in {folder_dest}. "
                     "Old files will be renamed if needed.")
     parser.add_argument("folder_src", type=str, nargs=1,
                        help="Path to source directory")
     parser.add_argument("folder_dest", type=str, nargs=1,
                        help="Path to destination directory")
+    parser.add_argument("--check_hash", default=False, action='store_true',
+                       help="Check hashes of files from {folder_dest}")
     # TODO: symlinks
-    # parser.add_argument("--symlink_mode", type=int, choices=[0, 1, 2], default=2, required=False,
-    #                    help="What to do with links: 0 - ignor, 1 - consider link content, 2 - use the file where the link refers to. Default 2.")
     parser = common_init_parser(parser)
     args = parser.parse_args(args)
     common_init_parse(args)
 
     folder1 = args.folder_src[0]
     folder2 = args.folder_dest[0]
     err_out = []
+    check_hash = args.check_hash
     folder1_abs = os.path.abspath(folder1)
     folder2_abs = os.path.abspath(folder2)
     if not is_folder(folder1_abs):
         pout(f"\"{folder1_abs}\" is not folder. ")
         exit()
     if not is_folder(folder2_abs):
         pout(f"\"{folder2_abs}\" is not folder. ")
         exit()
 
     if folder1_abs in folder2_abs:
-        pout(f"Directory \"{folder1_abs}\" contains directory \"{folder2_abs}\". Exiting...")
+        pout(f"Directory \"{folder1_abs}\" contains directory \"{folder2_abs}\". ")
         input("Enter to continue...")
     if folder2_abs in folder1_abs:
-        pout(f"Directory \"{folder2_abs}\" contains directory \"{folder1_abs}\". Exiting...")
+        pout(f"Directory \"{folder2_abs}\" contains directory \"{folder1_abs}\". ")
         input("Enter to continue...")
 
     pout(f"Calculating hash tree of directory \"{folder1_abs}\"...")
     d1 = calc_hash_dict_of_dir(folder1_abs)
 
     pout("Diffclonning...")
     # 3 варианта:
@@ -71,32 +73,73 @@
         dir_i_2 = os.path.join(folder2_abs, dir_i_rel)
         if not os.path.exists(dir_i_2):
             mkdir(dir_i_2, p=True)
 
     files1, files2 = getFilesList(folder1_abs), getFilesList(folder2_abs)
     for file1_i in tqdm(files1):
         try:
+            if os.path.islink(file1_i):
+                if Global.symlink_mode == 0:
+                    continue
+                if Global.symlink_mode == 1:
+                    # TODO: symlink rewrite original file
+                    pass
+
             file1_i_rel = str(os.path.relpath(file1_i, folder1_abs))
             file2_i = os.path.join(folder2_abs, file1_i_rel)
             if not os.path.isfile(file2_i):  # case 1
-                shutil.copy(file1_i, file2_i)
-                os.sync()
+                if copy_file(file1_i, file2_i) in [False, None]:
+                    err_out.append(f"Cannot copy \"{file1_i}\" to \"{file2_i}\". ")
             else:
                 file2_i_hash = get_hash_file(file2_i)
                 if d1[file1_i_rel] == file2_i_hash:  # case 2
                     pass  # ничего не делаем
                 else:  # case 3
                     file2_i_time = get_time_file(file2_i)
                     os.rename(file2_i, f"{file2_i}---{file2_i_time}.bak")
-                    shutil.copy(file1_i, file2_i)
-                    os.sync()
+                    if copy_file(file1_i, file2_i) in [False, None]:
+                        err_out.append(f"Cannot copy \"{file1_i}\" to \"{file2_i}\". ")
         except Exception as e:
             pout(str(e))
             err_out.append(f"\"{file1_i}\"")
 
+    if platform != "win32":
+        os.sync()
     if len(err_out) != 0:
         pout(f"\n===============\nSome troubles happened:")
         for err_i in err_out:
             pout(f"\t{err_i}")
         pout(f"===============")
 
+    IF_OK = True
+    if check_hash:
+        err_out = []
+        pout("Checking...")
+        for file1_i in tqdm(files1):
+            try:
+                if os.path.islink(file1_i):
+                    if Global.symlink_mode == 0:
+                        continue
+                file1_i_rel = str(os.path.relpath(file1_i, folder1_abs))
+                file2_i = os.path.join(folder2_abs, file1_i_rel)
+                file2_i_hash = get_hash_file(file2_i)
+                if d1[file1_i_rel] != file2_i_hash:
+                    buffS = (
+                        f"HASHES OF FILES DOES NOT MATCH: "
+                        f"\"{d1[file1_i_rel]}\" of \"{file1_i}\" and "
+                        f"\"{file2_i_hash}\" of \"{file2_i}\""
+                             )
+                    pout(buffS)
+                    err_out.append(buffS)
+                    IF_OK = False
+            except Exception as e:
+                IF_OK = False
+                pout(str(e))
+                err_out.append(f"\"{file1_i}\"")
+    if len(err_out) != 0:
+        pout(f"\n===============\nSome troubles happened:")
+        for err_i in err_out:
+            pout(f"\t{err_i}")
+        pout(f"===============")
+    if not IF_OK:
+        pout("Hashes does NOT match, diffclone failed!!!")
     pout("=============== Done! ===============")
```

### Comparing `diwork-1.1.0/diwork/diwork_mains/diwork_difx.py` & `diwork-1.2.0/diwork/diwork_mains/diwork_difx.py`

 * *Files identical despite different names*

### Comparing `diwork-1.1.0/diwork/diwork_mains/diwork_exec.py` & `diwork-1.2.0/diwork/diwork_mains/diwork_exec.py`

 * *Files identical despite different names*

### Comparing `diwork-1.1.0/diwork/diwork_mains/diwork_hash.py` & `diwork-1.2.0/diwork/diwork_mains/diwork_hash.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
     parser = argparse.ArgumentParser(prog = "diwork hash",
         description="Calculate hash of directory(s)")
     parser.add_argument("folders_paths", type=str, nargs="+",
                        help="Paths to directories whose hash will be calculated")
     parser.add_argument("--exclude", type=str, nargs="+", default=None, action="append",
                        help="Do not take these files or directories into consideration when calculating the hash")
-    parser.add_argument("--symlink_mode", type=int, choices=[0,1,2], default=2, required=False,
-                       help="What to do with links: 0 - ignor, 1 - consider link content, 2 - use the file where the link refers to. Default 2.")
+    # parser.add_argument("--symlink_mode", type=int, choices=[0,1,2], default=2, required=False,
+    #                    help="What to do with links: 0 - ignor, 1 - consider link content, 2 - use the file where the link refers to. Default 2.")
     parser.add_argument("--hierarchy", default=False, action='store_true',
                        help="If True, then the file hierarchy will be considered when calculating the hash. Default False")
     parser = common_init_parser(parser)
     args = parser.parse_args(args)
     common_init_parse(args)
 
     folders = args.folders_paths
```

### Comparing `diwork-1.1.0/diwork/diwork_mains/diwork_help.py` & `diwork-1.2.0/diwork/diwork_mains/diwork_help.py`

 * *Files identical despite different names*

### Comparing `diwork-1.1.0/diwork/diwork_mains/diwork_repeats.py` & `diwork-1.2.0/diwork/diwork_mains/diwork_repeats.py`

 * *Files identical despite different names*

### Comparing `diwork-1.1.0/diwork/diwork_mains/diwork_sshclone.py` & `diwork-1.2.0/diwork/diwork_mains/diwork_sshclone.py`

 * *Files identical despite different names*

### Comparing `diwork-1.1.0/diwork/diwork_ways/__init__.py` & `diwork-1.2.0/diwork/diwork_ways/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 from .diwork_sup import *
 
 from .diwork_parse import common_init_parser, common_init_parse
 
 __all__ = [
     "Global", "getFilesList", "getDirsList", "is_folder", "is_file", "is_exists", "is_folder_empty", "rel_path", "rm_folder_content", 
     "check_files_exists_or_exit", "pout", "write2File_str", "mkdir", "get_link_unwinding", "get_nice_size", "get_time_str", "get_time_file",
-    "get_hash_file", "get_hash_str", "get_hash_of_hashes", 
+    "copy_file", "get_hash_file", "get_hash_str", "get_hash_of_hashes",
     "exclude_files", "delete_all_if_dir_not_empty", "exe",
     "common_init_parser", "common_init_parse"
 ]
```

### Comparing `diwork-1.1.0/diwork/diwork_ways/diwork_parse.py` & `diwork-1.2.0/diwork/diwork_ways/diwork_parse.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 def common_init_parser(parser: "ArgumentParser") -> "ArgumentParser":
     # https://docs.python.org/3/library/argparse.html
     # https://stackoverflow.com/questions/20063/whats-the-best-way-to-parse-command-line-arguments
 
     parser.add_argument("--dublicate_out_to_file", type=str, default=None, required=False,
                        help="Duplicate program output to file")
 
-    parser.add_argument("--hash_mode", type=int, choices=[0,1,2], default=1, required=False,
-                       help="Hash mode: 0 is sha256sum, 1 is hashlib.sha256, 2 is sha512sum. Default 1.")
-
     parser.add_argument("--version", action="version", version=f"diwork {Global.version}",
                        help="Check version of diwork")
 
+    parser.add_argument("--symlink_mode", type=int, choices=[0, 1, 2], default=2, required=False,
+                       help="What to do with links: 0 - ignor, 1 - consider link content, 2 - use the file where the link refers to. Default 2.")
     return parser
 
 def common_init_parse(args: "ArgumentParser.parse_args") -> None:
     Global.outfile = args.dublicate_out_to_file
-    Global.hash_mode = args.hash_mode
+    Global.symlink_mode = args.symlink_mode
```

### Comparing `diwork-1.1.0/diwork/diwork_ways/diwork_sup.py` & `diwork-1.2.0/diwork/diwork_ways/diwork_sup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,164 +1,188 @@
 # -*- coding: utf-8 -*-
 
 import os
 import sys
 import subprocess
 import hashlib
 import datetime
+import shutil
 
 class Global():
     version = None
     outfile = None
-    hash_mode = 1 # 0 is sha256sum, 1 is hashlib.sha256, 2 is sha512sum
+    symlink_mode = None
     
 
-
 def getFilesList(dirPath: str) -> list:
     return [os.path.join(path, name) for path, subdirs, files in os.walk(dirPath) for name in files]
 
+
 def getDirsList(dirPath: str) -> list:
     dirs = [os.path.join(path, name) for path, subdirs, files in os.walk(dirPath) for name in subdirs]
     return list(set(dirs))
 
+
 # return False, if folder_path not exists or folder_path is not folder
 def is_folder(folder_path: str) -> bool:
     return os.path.isdir(folder_path)
 
+
 # return False, if file_path not exists or file_path is not file
 def is_file(file_path: str) -> bool:
     return os.path.isfile(file_path)
 
+
 # return False, if file_path not exists
 def is_exists(file_path: str) -> bool:
     return os.path.exists(file_path)
 
+
 def check_files_exists_or_exit(files: list) -> None:
     F = False
     for file_i in files:
         if(is_exists(file_i) == False):
             pout(f"File \"{file_i}\" does not exists. ")
             F = True
     if(F == True):
         exit()
 
+
 def is_folder_empty(folder_path: str) -> bool:
     if(len(os.listdir(folder_path)) == 0):
         return True
     else:
         return False
 
+
 def rel_path(file_path: str, folder_path: str) -> str:
     return os.path.relpath(file_path, folder_path)
 
+
 def rm_folder_content(folder_path: str, root_dir_too: bool = False, does_not_exists_is_ok = False):
     """Удаляет всё содержимое папки. Саму папку не трогает, если root_dir_too == False"""
     if(does_not_exists_is_ok == True and is_folder(folder_path) == False):
         return
     for root, dirs, files in os.walk(folder_path, topdown=False):
         for file_i in files:
             os.remove(os.path.join(root, file_i))
         for dir in dirs:
             os.rmdir(os.path.join(root, dir))
     if(root_dir_too == True):
         os.rmdir(folder_path)
 
+
 def pout(msg : str, endl = True):
     if(endl == False):
         pout_low(msg)
     else:
         pout_low(msg + "\n")
 
+
 def pout_low(msg: str):
     print(msg, end="")
     if(Global.outfile != None):
         with open(Global.outfile, "a", encoding="utf-8") as fd:
             fd.write(msg)
             fd.flush()
 
+
 def write2File_str(fileName : str, s : str) -> None:
     with open(fileName, 'w', encoding="utf-8") as temp:
         temp.write(s)
         temp.flush()
 
+
 def mkdir(path: str, p: bool = True):
     os.makedirs(path, exist_ok=True)
 
-def get_link_unwinding(link_path: str) -> str:
+
+def get_link_unwinding(link_path: str) -> str or None:
     """Вернёт конечный файл, на который (рекурсивно) ссылаются сылки. """
     if(os.path.exists(link_path) == False):
         return None
     elif(os.path.islink(link_path) == False):
         return link_path
     else:
         linkto = os.readlink(link_path)
         if(os.path.islink(linkto) == False):
             return linkto
         else:
             return get_link_unwinding(linkto)
 
+
 def get_nice_size(size_bytes: int) -> str:
     if(size_bytes < 1024):
         return f"{size_bytes} B"
     elif(size_bytes < 1024*1024):
         return f"{size_bytes // 1024} KB"
     elif(size_bytes < 1024*1024*1024):
         return f"{size_bytes // (1024*1024)} MB"
     elif(size_bytes < 1024*1024*1024*1024):
         return f"{size_bytes // (1024*1024*1024)} GB"
     else:
         return f"{size_bytes // (1024*1024*1024*1024)} TB"
 
+
 def get_time_str() -> str:
     # time_str = datetime.datetime.now().strftime("[%y.%m.%d %H:%M:%S.%f]")
     time_str = datetime.datetime.now().strftime("%y.%m.%d %H:%M:%S")
     return time_str
 
+
 def get_time_file(file_path: str) -> str:
     dt_m = datetime.datetime.fromtimestamp(os.path.getmtime(file_path))
     return dt_m.strftime("%d.%m.%Y_%H-%M-%S")
 
-def get_hash_file(file_path: str) -> str:
-    if(Global.hash_mode == 1):
-        buff_BLOCKSIZE = 65536 # 64 kB
-        sha = hashlib.sha256()
-        with open(file_path, "rb") as temp:
+
+def copy_file(src: str, dest: str) -> bool or None:
+    if os.path.islink(src):
+        if Global.symlink_mode == 0:
+            return None
+        elif Global.symlink_mode == 1:
+            linkto = os.readlink(src)
+            os.symlink(linkto, dest)
+            return True
+        elif Global.symlink_mode == 2:
+            file_path = get_link_unwinding(src)
+            if file_path is None:
+                return False
+        else:
+            raise Exception(f"Failed successfully: copy_file with {src}->{dest}")
+
+    shutil.copy(src, dest)
+    return True
+
+
+def get_hash_file(file_path: str) -> str or None:
+    if os.path.islink(file_path):
+        if Global.symlink_mode == 0:
+            return None
+        elif Global.symlink_mode == 1:
+            return get_hash_str(os.readlink(file_path))
+        elif Global.symlink_mode == 2:
+            file_path = get_link_unwinding(file_path)
+            if file_path is None:
+                return None
+        else:
+            raise Exception(f"Failed successfully: get_hash_file with {file_path}")
+
+    buff_BLOCKSIZE = 65536  # 64 kB
+    sha = hashlib.sha256()
+    with open(file_path, "rb") as temp:
+        file_buffer = temp.read(buff_BLOCKSIZE)
+        while len(file_buffer) > 0:
+            sha.update(file_buffer)
             file_buffer = temp.read(buff_BLOCKSIZE)
-            while len(file_buffer) > 0:
-                sha.update(file_buffer)
-                file_buffer = temp.read(buff_BLOCKSIZE)
-        return sha.hexdigest()
-    else:
-        if(Global.hash_mode == 0):
-            shaxxxsum = "sha256sum"
-        elif(Global.hash_mode == 2):
-            shaxxxsum = "sha512sum"
-        exe_res = exe(f"{shaxxxsum} \"{file_path}\"")
-        if(exe_res[1] != ""):
-            pout(f"Error with {shaxxxsum}: ")
-            pout(f"\"{exe_res[1]}\"")
-            exit()
-        res = exe_res[0]
-        return res[:res.find(" ")]
+    return sha.hexdigest()
+
 
 def get_hash_str(s: str):
-    if(Global.hash_mode == 1):
-        return hashlib.sha256( s.encode("utf-8") ).hexdigest()
-    else:
-        if(Global.hash_mode == 0):
-            shaxxxsum = "sha256sum"
-        elif(Global.hash_mode == 2):
-            shaxxxsum = "sha512sum"
-        exe_res = exe(f"{shaxxxsum}", stdin_msg=s)
-        if(exe_res[1] != ""):
-            pout(f"Error with {shaxxxsum}: ")
-            pout(f"\"{exe_res[1]}\"")
-            exit()
-        res = exe_res[0]
-        return res[:res.find(" ")]
+    return hashlib.sha256( s.encode("utf-8") ).hexdigest()
+
 
 def get_hash_of_hashes(hashes: list) -> str:
 
     # IF CHANGE, then change make_archive_one_folder in diwork_archive.py (its legacy_version)
 
     # from io import StringIO
     # o = StringIO()
@@ -194,14 +218,15 @@
             for ex_file_i in exclude_files:
                 if ex_file_i in file_i:
                     F = False
             if(F == True):
                 res.append(file_i) 
     return res
 
+
 def delete_all_if_dir_not_empty(dir_path: str):
     if(is_folder_empty(dir_path) == False):
         pout(f"Folder \"{dir_path}\" is not empty. ")
         pout(f"===============\n\t All files in \"{dir_path}\" will be removed before continue. \n===============")
         pout("Continue? Type \"yes\" in capital letter to continue or \"no\" to exit. \n> ", endl=False)
         
         while(True):
@@ -217,22 +242,24 @@
         rm_folder_content(dir_path)
         if(is_folder_empty(dir_path) == True):
             pout(f"All files from folder \"{dir_path}\" removed. This folder is empty now.")
         else:
             pout(f"Cannot clean folder \"{dir_path}\"! Exiting ")
             exit()
 
+
 def get_dirs_needed_for_files(files: list) -> list:
     dirs = set()
     for file_i in files:
         dir_i = os.path.dirname(file_i)
         dirs.add(dir_i)
     dirs = sorted(list(dirs))
     return dirs
 
+
 def exe_lowout(command: str, debug: bool = True, std_out_pipe: bool = False, std_err_pipe: bool = False) -> tuple:
     '''
     Аргумент command - команда для выполнения в терминале. Например: "ls -lai ."
     Возвращает кортеж, где элементы:
         0 - строка stdout or None if std_out_pipe == False
         1 - строка stderr or None if std_err_pipe == False
         2 - returncode
@@ -258,14 +285,15 @@
         else:
             process = subprocess.Popen(command, shell=True)
             out = None
             err = None
     errcode = process.returncode
     return (out, err, errcode)
 
+
 def exe(command: str, debug: bool = True, std_out_fd = subprocess.PIPE, std_err_fd = subprocess.PIPE, stdin_msg: str = None) -> tuple:
     '''
     Аргумент command - команда для выполнения в терминале. Например: "ls -lai ."
     if(std_out_fd or std_err_fd) == subprocess.DEVNULL   |=>    No output enywhere
     if(std_out_fd or std_err_fd) == subprocess.PIPE      |=>    All output to return
     if(std_out_fd or std_err_fd) == open(path, "w")      |=>    All output to file path
     Возвращает кортеж, где элементы:
@@ -288,8 +316,8 @@
     else:
         proc = subprocess.run(command, shell=True, stdout=std_out_fd, stderr=std_err_fd, input=stdin_msg.encode("utf-8"))
     
     #return (proc.stdout.decode("utf-8"), proc.stderr.decode("utf-8"))
 
     res_stdout = proc.stdout.decode("utf-8") if proc.stdout != None else None
     res_errout = proc.stderr.decode("utf-8") if proc.stderr != None else None
-    return (res_stdout, res_errout, proc.returncode)
+    return (res_stdout, res_errout, proc.returncode)
```

### Comparing `diwork-1.1.0/diwork/main.py` & `diwork-1.2.0/diwork/main.py`

 * *Files identical despite different names*

### Comparing `diwork-1.1.0/diwork.egg-info/SOURCES.txt` & `diwork-1.2.0/diwork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diwork-1.1.0/setup.py` & `diwork-1.2.0/setup.py`

 * *Files identical despite different names*

