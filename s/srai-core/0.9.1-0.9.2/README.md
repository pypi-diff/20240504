# Comparing `tmp/srai-core-0.9.1.tar.gz` & `tmp/srai-core-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-core-0.9.1.tar", last modified: Sun Sep 10 08:52:42 2023, max compression
+gzip compressed data, was "srai-core-0.9.2.tar", last modified: Sun Sep 10 09:10:47 2023, max compression
```

## Comparing `srai-core-0.9.1.tar` & `srai-core-0.9.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-09-10 08:52:42.417935 srai-core-0.9.1/
--rw-rw-rw-   0        0        0     1092 2023-07-15 07:11:37.000000 srai-core-0.9.1/LICENSE.txt
--rw-rw-rw-   0        0        0       24 2023-07-15 08:05:50.000000 srai-core-0.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0      767 2023-09-10 08:52:42.417935 srai-core-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-07-15 07:11:37.000000 srai-core-0.9.1/README.md
--rw-rw-rw-   0        0        0       76 2023-09-10 08:06:19.000000 srai-core-0.9.1/requirements.txt
--rw-rw-rw-   0        0        0      129 2023-09-10 08:52:42.417935 srai-core-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1894 2023-09-10 08:11:09.000000 srai-core-0.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-10 08:52:42.377806 srai-core-0.9.1/srai_core/
--rw-rw-rw-   0        0        0      130 2023-09-10 08:11:04.000000 srai-core-0.9.1/srai_core/__init__.py
--rw-rw-rw-   0        0        0      213 2023-09-04 07:11:22.000000 srai-core-0.9.1/srai_core/base_command_handler.py
--rw-rw-rw-   0        0        0      593 2023-09-07 10:45:53.000000 srai-core-0.9.1/srai_core/command_handler_ssh.py
--rw-rw-rw-   0        0        0      326 2023-09-04 07:15:23.000000 srai-core-0.9.1/srai_core/command_handler_subprocess.py
--rw-rw-rw-   0        0        0      538 2023-07-16 08:31:22.000000 srai-core-0.9.1/srai_core/file_store.py
--rw-rw-rw-   0        0        0      499 2023-07-16 09:04:42.000000 srai-core-0.9.1/srai_core/file_store_disk.py
--rw-rw-rw-   0        0        0     1296 2023-07-16 09:07:55.000000 srai-core-0.9.1/srai_core/jsondict_store.py
-drwxrwxrwx   0        0        0        0 2023-09-10 08:52:42.417935 srai-core-0.9.1/srai_core/script/
--rw-rw-rw-   0        0        0        0 2023-07-15 06:16:01.000000 srai-core-0.9.1/srai_core/script/__init__.py
--rw-rw-rw-   0        0        0      270 2023-09-04 07:15:31.000000 srai-core-0.9.1/srai_core/script/build_docker.py
--rw-rw-rw-   0        0        0      803 2023-09-04 09:00:52.000000 srai-core-0.9.1/srai_core/script/build_docker_remote_ssh.py
--rw-rw-rw-   0        0        0      148 2023-09-04 08:41:07.000000 srai-core-0.9.1/srai_core/script/create_repository.py
--rw-rw-rw-   0        0        0     1094 2023-09-04 07:42:22.000000 srai-core-0.9.1/srai_core/script/deploy_docker_local.py
--rw-rw-rw-   0        0        0     1766 2023-09-02 09:11:23.000000 srai-core-0.9.1/srai_core/script/deploy_docker_remote_ssh.py
--rw-rw-rw-   0        0        0      430 2023-09-10 08:09:22.000000 srai-core-0.9.1/srai_core/script/list_commands.py
--rw-rw-rw-   0        0        0      829 2023-09-04 08:41:58.000000 srai-core-0.9.1/srai_core/script/list_containers_ssh.py
--rw-rw-rw-   0        0        0      355 2023-09-10 08:02:05.000000 srai-core-0.9.1/srai_core/script/list_images.py
--rw-rw-rw-   0        0        0      462 2023-09-04 07:44:25.000000 srai-core-0.9.1/srai_core/script/release_code_public.py
--rw-rw-rw-   0        0        0      351 2023-09-04 08:30:54.000000 srai-core-0.9.1/srai_core/script/release_docker_aws_local.py
--rw-rw-rw-   0        0        0     1132 2023-09-07 11:24:58.000000 srai-core-0.9.1/srai_core/script/release_docker_aws_ssh.py
--rw-rw-rw-   0        0        0     8805 2023-09-10 08:10:52.000000 srai-core-0.9.1/srai_core/tools_docker.py
--rw-rw-rw-   0        0        0     1562 2023-09-07 12:07:42.000000 srai-core-0.9.1/srai_core/tools_env.py
-drwxrwxrwx   0        0        0        0 2023-09-10 08:52:42.402169 srai-core-0.9.1/srai_core.egg-info/
--rw-rw-rw-   0        0        0      767 2023-09-10 08:52:42.000000 srai-core-0.9.1/srai_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      991 2023-09-10 08:52:42.000000 srai-core-0.9.1/srai_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-10 08:52:42.000000 srai-core-0.9.1/srai_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      500 2023-09-10 08:52:42.000000 srai-core-0.9.1/srai_core.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       72 2023-09-10 08:52:42.000000 srai-core-0.9.1/srai_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-09-10 08:52:42.000000 srai-core-0.9.1/srai_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-09-10 09:10:47.240432 srai-core-0.9.2/
+-rw-rw-rw-   0        0        0     1092 2023-07-15 07:11:37.000000 srai-core-0.9.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       24 2023-07-15 08:05:50.000000 srai-core-0.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      767 2023-09-10 09:10:47.240432 srai-core-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-07-15 07:11:37.000000 srai-core-0.9.2/README.md
+-rw-rw-rw-   0        0        0       76 2023-09-10 08:06:19.000000 srai-core-0.9.2/requirements.txt
+-rw-rw-rw-   0        0        0      129 2023-09-10 09:10:47.243586 srai-core-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1894 2023-09-10 09:10:42.000000 srai-core-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-10 09:10:47.206329 srai-core-0.9.2/srai_core/
+-rw-rw-rw-   0        0        0      130 2023-09-10 09:10:33.000000 srai-core-0.9.2/srai_core/__init__.py
+-rw-rw-rw-   0        0        0      213 2023-09-04 07:11:22.000000 srai-core-0.9.2/srai_core/base_command_handler.py
+-rw-rw-rw-   0        0        0      593 2023-09-07 10:45:53.000000 srai-core-0.9.2/srai_core/command_handler_ssh.py
+-rw-rw-rw-   0        0        0      326 2023-09-04 07:15:23.000000 srai-core-0.9.2/srai_core/command_handler_subprocess.py
+-rw-rw-rw-   0        0        0      538 2023-07-16 08:31:22.000000 srai-core-0.9.2/srai_core/file_store.py
+-rw-rw-rw-   0        0        0      499 2023-07-16 09:04:42.000000 srai-core-0.9.2/srai_core/file_store_disk.py
+-rw-rw-rw-   0        0        0     1296 2023-07-16 09:07:55.000000 srai-core-0.9.2/srai_core/jsondict_store.py
+drwxrwxrwx   0        0        0        0 2023-09-10 09:10:47.240432 srai-core-0.9.2/srai_core/script/
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:16:01.000000 srai-core-0.9.2/srai_core/script/__init__.py
+-rw-rw-rw-   0        0        0      270 2023-09-04 07:15:31.000000 srai-core-0.9.2/srai_core/script/build_docker.py
+-rw-rw-rw-   0        0        0      803 2023-09-04 09:00:52.000000 srai-core-0.9.2/srai_core/script/build_docker_remote_ssh.py
+-rw-rw-rw-   0        0        0      148 2023-09-04 08:41:07.000000 srai-core-0.9.2/srai_core/script/create_repository.py
+-rw-rw-rw-   0        0        0     1094 2023-09-04 07:42:22.000000 srai-core-0.9.2/srai_core/script/deploy_docker_local.py
+-rw-rw-rw-   0        0        0     1766 2023-09-02 09:11:23.000000 srai-core-0.9.2/srai_core/script/deploy_docker_remote_ssh.py
+-rw-rw-rw-   0        0        0      430 2023-09-10 08:09:22.000000 srai-core-0.9.2/srai_core/script/list_commands.py
+-rw-rw-rw-   0        0        0      829 2023-09-04 08:41:58.000000 srai-core-0.9.2/srai_core/script/list_containers_ssh.py
+-rw-rw-rw-   0        0        0      355 2023-09-10 08:02:05.000000 srai-core-0.9.2/srai_core/script/list_images.py
+-rw-rw-rw-   0        0        0      462 2023-09-04 07:44:25.000000 srai-core-0.9.2/srai_core/script/release_code_public.py
+-rw-rw-rw-   0        0        0      366 2023-09-10 09:08:09.000000 srai-core-0.9.2/srai_core/script/release_docker_aws_local.py
+-rw-rw-rw-   0        0        0     1132 2023-09-07 11:24:58.000000 srai-core-0.9.2/srai_core/script/release_docker_aws_ssh.py
+-rw-rw-rw-   0        0        0     8805 2023-09-10 08:10:52.000000 srai-core-0.9.2/srai_core/tools_docker.py
+-rw-rw-rw-   0        0        0     1562 2023-09-07 12:07:42.000000 srai-core-0.9.2/srai_core/tools_env.py
+drwxrwxrwx   0        0        0        0 2023-09-10 09:10:47.222364 srai-core-0.9.2/srai_core.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-09-10 09:10:47.000000 srai-core-0.9.2/srai_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      991 2023-09-10 09:10:47.000000 srai-core-0.9.2/srai_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-09-10 09:10:47.000000 srai-core-0.9.2/srai_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      500 2023-09-10 09:10:47.000000 srai-core-0.9.2/srai_core.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       72 2023-09-10 09:10:47.000000 srai-core-0.9.2/srai_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-09-10 09:10:47.000000 srai-core-0.9.2/srai_core.egg-info/top_level.txt
```

### Comparing `srai-core-0.9.1/LICENSE.txt` & `srai-core-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srai-core-0.9.1/PKG-INFO` & `srai-core-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srai-core
-Version: 0.9.1
+Version: 0.9.2
 Summary: A library core functions used in other SRAI libraries.
 Home-page: https://github.com/southriverai/srai-core
 Download-URL: https://github.com/southriverai/srai-core/archive/v_01.tar.gz
 Author: Jaap Oosterbroek
 Author-email: jaap.oosterbroek@southriverai.com
 License: MIT
 Keywords: SRAI,TOOLS
```

### Comparing `srai-core-0.9.1/setup.py` & `srai-core-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="srai-core",
     packages=find_packages(),
-    version="0.9.1",  # TODO manual....
+    version="0.9.2",  # TODO manual....
     license="MIT",
     package_data={},
     python_requires=">=3.5",
     install_requires=requirements,
     author="Jaap Oosterbroek",
     author_email="jaap.oosterbroek@southriverai.com",
     description="A library core functions used in other SRAI libraries.",
```

### Comparing `srai-core-0.9.1/srai_core/command_handler_ssh.py` & `srai-core-0.9.2/srai_core/command_handler_ssh.py`

 * *Files identical despite different names*

### Comparing `srai-core-0.9.1/srai_core/file_store.py` & `srai-core-0.9.2/srai_core/file_store.py`

 * *Files identical despite different names*

### Comparing `srai-core-0.9.1/srai_core/jsondict_store.py` & `srai-core-0.9.2/srai_core/jsondict_store.py`

 * *Files identical despite different names*

### Comparing `srai-core-0.9.1/srai_core/script/build_docker_remote_ssh.py` & `srai-core-0.9.2/srai_core/script/build_docker_remote_ssh.py`

 * *Files identical despite different names*

### Comparing `srai-core-0.9.1/srai_core/script/deploy_docker_local.py` & `srai-core-0.9.2/srai_core/script/deploy_docker_local.py`

 * *Files identical despite different names*

### Comparing `srai-core-0.9.1/srai_core/script/deploy_docker_remote_ssh.py` & `srai-core-0.9.2/srai_core/script/deploy_docker_remote_ssh.py`

 * *Files identical despite different names*

### Comparing `srai-core-0.9.1/srai_core/script/list_containers_ssh.py` & `srai-core-0.9.2/srai_core/script/list_containers_ssh.py`

 * *Files identical despite different names*

### Comparing `srai-core-0.9.1/srai_core/script/release_docker_aws_ssh.py` & `srai-core-0.9.2/srai_core/script/release_docker_aws_ssh.py`

 * *Files identical despite different names*

### Comparing `srai-core-0.9.1/srai_core/tools_docker.py` & `srai-core-0.9.2/srai_core/tools_docker.py`

 * *Files identical despite different names*

### Comparing `srai-core-0.9.1/srai_core/tools_env.py` & `srai-core-0.9.2/srai_core/tools_env.py`

 * *Files identical despite different names*

### Comparing `srai-core-0.9.1/srai_core.egg-info/PKG-INFO` & `srai-core-0.9.2/srai_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srai-core
-Version: 0.9.1
+Version: 0.9.2
 Summary: A library core functions used in other SRAI libraries.
 Home-page: https://github.com/southriverai/srai-core
 Download-URL: https://github.com/southriverai/srai-core/archive/v_01.tar.gz
 Author: Jaap Oosterbroek
 Author-email: jaap.oosterbroek@southriverai.com
 License: MIT
 Keywords: SRAI,TOOLS
```

### Comparing `srai-core-0.9.1/srai_core.egg-info/SOURCES.txt` & `srai-core-0.9.2/srai_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

