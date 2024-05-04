# Comparing `tmp/github-backup-0.8.0.tar.gz` & `tmp/github-backup-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/github-backup-0.8.0.tar", last modified: Sun Feb 14 21:04:56 2016, max compression
+gzip compressed data, was "dist/github-backup-0.9.0.tar", last modified: Tue Mar 29 17:23:47 2016, max compression
```

## Comparing `github-backup-0.8.0.tar` & `github-backup-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2016-02-14 21:04:56.000000 github-backup-0.8.0/
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2016-02-14 21:04:56.000000 github-backup-0.8.0/bin/
--rwxr-xr-x   0 jose       (501) staff       (20)    25355 2016-02-14 21:04:47.000000 github-backup-0.8.0/bin/github-backup
--rw-r--r--   0 jose       (501) wheel        (0)     4898 2016-02-14 21:04:54.000000 github-backup-0.8.0/CHANGES.rst
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2016-02-14 21:04:56.000000 github-backup-0.8.0/github_backup/
--rw-------   0 jose       (501) wheel        (0)       22 2016-02-14 21:04:54.000000 github-backup-0.8.0/github_backup/__init__.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2016-02-14 21:04:56.000000 github-backup-0.8.0/github_backup.egg-info/
--rw-r--r--   0 jose       (501) staff       (20)        1 2016-02-14 21:04:56.000000 github-backup-0.8.0/github_backup.egg-info/dependency_links.txt
--rw-r--r--   0 jose       (501) staff       (20)       46 2016-02-14 21:04:56.000000 github-backup-0.8.0/github_backup.egg-info/pbr.json
--rw-r--r--   0 jose       (501) staff       (20)     5967 2016-02-14 21:04:56.000000 github-backup-0.8.0/github_backup.egg-info/PKG-INFO
--rw-r--r--   0 jose       (501) staff       (20)      335 2016-02-14 21:04:56.000000 github-backup-0.8.0/github_backup.egg-info/SOURCES.txt
--rw-r--r--   0 jose       (501) staff       (20)       14 2016-02-14 21:04:56.000000 github-backup-0.8.0/github_backup.egg-info/top_level.txt
--rw-r--r--   0 jose       (501) staff       (20)        1 2015-02-20 17:41:35.000000 github-backup-0.8.0/github_backup.egg-info/zip-safe
--rw-r--r--   0 jose       (501) staff       (20)     1085 2015-02-20 17:40:36.000000 github-backup-0.8.0/LICENSE.txt
--rw-r--r--   0 jose       (501) staff       (20)       28 2015-02-20 17:40:36.000000 github-backup-0.8.0/MANIFEST.in
--rw-r--r--   0 jose       (501) staff       (20)     5967 2016-02-14 21:04:56.000000 github-backup-0.8.0/PKG-INFO
--rw-r--r--   0 jose       (501) staff       (20)     3660 2016-02-14 21:04:56.000000 github-backup-0.8.0/README
--rw-r--r--   0 jose       (501) wheel        (0)     3660 2016-02-14 21:04:54.000000 github-backup-0.8.0/README.rst
--rw-r--r--   0 jose       (501) staff       (20)        1 2015-02-20 17:40:36.000000 github-backup-0.8.0/requirements.txt
--rw-r--r--   0 jose       (501) staff       (20)       59 2016-02-14 21:04:56.000000 github-backup-0.8.0/setup.cfg
--rw-r--r--   0 jose       (501) staff       (20)     1456 2015-02-20 17:40:36.000000 github-backup-0.8.0/setup.py
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2016-03-29 17:23:47.000000 github-backup-0.9.0/
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2016-03-29 17:23:47.000000 github-backup-0.9.0/bin/
+-rwxr-xr-x   0 jose       (501) staff       (20)    26111 2016-03-29 17:23:31.000000 github-backup-0.9.0/bin/github-backup
+-rw-r--r--   0 jose       (501) wheel        (0)     5006 2016-03-29 17:23:45.000000 github-backup-0.9.0/CHANGES.rst
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2016-03-29 17:23:47.000000 github-backup-0.9.0/github_backup/
+-rw-------   0 jose       (501) wheel        (0)       22 2016-03-29 17:23:45.000000 github-backup-0.9.0/github_backup/__init__.py
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2016-03-29 17:23:47.000000 github-backup-0.9.0/github_backup.egg-info/
+-rw-r--r--   0 jose       (501) staff       (20)        1 2016-03-29 17:23:47.000000 github-backup-0.9.0/github_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 jose       (501) staff       (20)       46 2016-02-14 21:04:56.000000 github-backup-0.9.0/github_backup.egg-info/pbr.json
+-rw-r--r--   0 jose       (501) staff       (20)     5967 2016-03-29 17:23:47.000000 github-backup-0.9.0/github_backup.egg-info/PKG-INFO
+-rw-r--r--   0 jose       (501) staff       (20)      335 2016-03-29 17:23:47.000000 github-backup-0.9.0/github_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 jose       (501) staff       (20)       14 2016-03-29 17:23:47.000000 github-backup-0.9.0/github_backup.egg-info/top_level.txt
+-rw-r--r--   0 jose       (501) staff       (20)        1 2015-02-20 17:41:35.000000 github-backup-0.9.0/github_backup.egg-info/zip-safe
+-rw-r--r--   0 jose       (501) staff       (20)     1085 2015-02-20 17:40:36.000000 github-backup-0.9.0/LICENSE.txt
+-rw-r--r--   0 jose       (501) staff       (20)       28 2015-02-20 17:40:36.000000 github-backup-0.9.0/MANIFEST.in
+-rw-r--r--   0 jose       (501) staff       (20)     5967 2016-03-29 17:23:47.000000 github-backup-0.9.0/PKG-INFO
+-rw-r--r--   0 jose       (501) staff       (20)     3660 2016-03-29 17:23:47.000000 github-backup-0.9.0/README
+-rw-r--r--   0 jose       (501) wheel        (0)     3660 2016-03-29 17:23:45.000000 github-backup-0.9.0/README.rst
+-rw-r--r--   0 jose       (501) staff       (20)        1 2015-02-20 17:40:36.000000 github-backup-0.9.0/requirements.txt
+-rw-r--r--   0 jose       (501) staff       (20)       59 2016-03-29 17:23:47.000000 github-backup-0.9.0/setup.cfg
+-rw-r--r--   0 jose       (501) staff       (20)     1456 2015-02-20 17:40:36.000000 github-backup-0.9.0/setup.py
```

### Comparing `github-backup-0.8.0/bin/github-backup` & `github-backup-0.9.0/bin/github-backup`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import logging
 import os
 import re
 import select
 import subprocess
 import sys
 import time
+import urlparse
 import urllib
 import urllib2
 
 from github_backup import __version__
 
 FNULL = open(os.devnull, 'w')
 
@@ -91,14 +92,23 @@
             os.makedirs(path)
         except OSError as exc:  # Python >2.5
             if exc.errno == errno.EEXIST and os.path.isdir(path):
                 pass
             else:
                 raise
 
+def mask_password(url, secret='*****'):
+    parsed = urlparse.urlparse(url)
+
+    if not parsed.password:
+        return url
+    elif parsed.password == 'x-oauth-basic':
+        return url.replace(parsed.username, secret)
+
+    return url.replace(parsed.password, secret)
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Backup a github account',
                                      prog='Github Backup')
     parser.add_argument('user',
                         metavar='USER',
                         type=str,
@@ -217,46 +227,67 @@
                         help='Clone repositories using SSH instead of HTTPS')
     parser.add_argument('-v', '--version',
                         action='version',
                         version='%(prog)s ' + __version__)
     return parser.parse_args()
 
 
-def get_auth(args):
-    if args.token:
-        return base64.b64encode(args.token + ':' + 'x-oauth-basic')
+def get_auth(args, encode=True):
+    auth = None
 
-    if args.username:
+    if args.token:
+        auth = args.token + ':' + 'x-oauth-basic'
+    elif args.username:
         if not args.password:
             args.password = getpass.getpass()
-        return base64.b64encode(args.username + ':' + args.password)
-
-    if args.password:
+        auth = args.username + ':' + args.password
+    elif args.password:
         log_error('You must specify a username for basic auth')
 
-    return None
+    if not auth:
+        return None
+
+    if encode == False:
+        return auth
+
+    return base64.b64encode(auth)
 
 
 def get_github_api_host(args):
     if args.github_host:
         host = args.github_host + '/api/v3'
     else:
         host = 'api.github.com'
 
     return host
 
 
-def get_github_ssh_host(args):
+def get_github_host(args):
     if args.github_host:
         host = args.github_host
     else:
         host = 'github.com'
 
     return host
 
+def get_github_repo_url(args, repository):
+    if args.prefer_ssh:
+        return repository['ssh_url']
+
+    auth = get_auth(args, False)
+    if auth:
+        repo_url = 'https://{0}@{1}/{2}/{3}.git'.format(
+            auth,
+            get_github_host(args),
+            args.user,
+            repository['name'])
+    else:
+        repo_url = repository['clone_url']
+
+    return repo_url
 
 def retrieve_data(args, template, query_args=None, single_request=False):
     auth = get_auth(args)
     query_args = get_query_args(query_args)
     per_page = 100
     page = 0
     data = []
@@ -428,19 +459,15 @@
     log_info('Backing up repositories')
     repos_template = 'https://{0}/repos'.format(get_github_api_host(args))
 
     for repository in repositories:
         backup_cwd = os.path.join(output_directory, 'repositories')
         repo_cwd = os.path.join(backup_cwd, repository['name'])
         repo_dir = os.path.join(repo_cwd, 'repository')
-
-        if args.prefer_ssh:
-            repo_url = repository['ssh_url']
-        else:
-            repo_url = repository['clone_url']
+        repo_url = get_github_repo_url(args, repository)
 
         if args.include_repository or args.include_everything:
             fetch_repository(repository['name'],
                              repo_url,
                              repo_dir,
                              skip_existing=args.skip_existing)
 
@@ -622,33 +649,35 @@
 
 def fetch_repository(name, remote_url, local_dir, skip_existing=False):
     clone_exists = os.path.exists(os.path.join(local_dir, '.git'))
 
     if clone_exists and skip_existing:
         return
 
+    masked_remote_url = mask_password(remote_url)
+
     initalized = subprocess.call('git ls-remote ' + remote_url,
                                  stdout=FNULL,
                                  stderr=FNULL,
                                  shell=True)
     if initalized == 128:
-        log_info("Skipping {0} ({1}) since it's not initalized".format(name, remote_url))
+        log_info("Skipping {0} ({1}) since it's not initalized".format(name, masked_remote_url))
         return
 
     if clone_exists:
         log_info('Updating {0} in {1}'.format(name, local_dir))
         git_command = ['git', 'remote', 'rm', 'origin']
         logging_subprocess(git_command, None, cwd=local_dir)
         git_command = ['git', 'remote', 'add', 'origin', remote_url]
         logging_subprocess(git_command, None, cwd=local_dir)
         git_command = ['git', 'fetch', '--all', '--tags', '--prune']
         logging_subprocess(git_command, None, cwd=local_dir)
     else:
         log_info('Cloning {0} repository from {1} to {2}'.format(name,
-                                                                 remote_url,
+                                                                 masked_remote_url,
                                                                  local_dir))
         git_command = ['git', 'clone', remote_url, local_dir]
         logging_subprocess(git_command, None)
 
 
 def backup_account(args, output_directory):
     account_cwd = os.path.join(output_directory, 'account')
```

### Comparing `github-backup-0.8.0/CHANGES.rst` & `github-backup-0.9.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+0.9.0 (2016-03-29)
+------------------
+
+- Fix cloning private repos with basic auth or token. [Kazuki Suda]
+
 0.8.0 (2016-02-14)
 ------------------
 
 - Don't store issues which are actually pull requests. [Enrico Tröger]
 
   This prevents storing pull requests twice since the Github API returns
   pull requests also as issues. Those issues will be skipped but only if
```

### Comparing `github-backup-0.8.0/github_backup.egg-info/PKG-INFO` & `github-backup-0.9.0/github_backup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: github-backup
-Version: 0.8.0
+Version: 0.9.0
 Summary: backup a github user or organization
 Home-page: http://github.com/josegonzalez/python-github-backup
 Author: Jose Diaz-Gonzalez
 Author-email: github-backup@josediazgonzalez.com
 License: The MIT License (MIT)
 
 Copyright (c) 2013 Jose Diaz-Gonzalez
```

### Comparing `github-backup-0.8.0/LICENSE.txt` & `github-backup-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `github-backup-0.8.0/PKG-INFO` & `github-backup-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: github-backup
-Version: 0.8.0
+Version: 0.9.0
 Summary: backup a github user or organization
 Home-page: http://github.com/josegonzalez/python-github-backup
 Author: Jose Diaz-Gonzalez
 Author-email: github-backup@josediazgonzalez.com
 License: The MIT License (MIT)
 
 Copyright (c) 2013 Jose Diaz-Gonzalez
```

### Comparing `github-backup-0.8.0/README` & `github-backup-0.9.0/README`

 * *Files identical despite different names*

### Comparing `github-backup-0.8.0/README.rst` & `github-backup-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `github-backup-0.8.0/setup.py` & `github-backup-0.9.0/setup.py`

 * *Files identical despite different names*

