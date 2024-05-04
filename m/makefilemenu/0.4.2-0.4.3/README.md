# Comparing `tmp/makefilemenu-0.4.2.tar.gz` & `tmp/makefilemenu-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/makefilemenu-0.4.2.tar", last modified: Tue Aug 25 05:28:55 2020, max compression
+gzip compressed data, was "makefilemenu-0.4.3.tar", last modified: Sat May  4 07:11:14 2024, max compression
```

## Comparing `makefilemenu-0.4.2.tar` & `makefilemenu-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 kkto      (1000) kkto      (1000)        0 2020-08-25 05:28:55.000000 makefilemenu-0.4.2/
--rw-r--r--   0 kkto      (1000) kkto      (1000)     4323 2020-08-25 05:28:55.000000 makefilemenu-0.4.2/PKG-INFO
--rw-r--r--   0 kkto      (1000) kkto      (1000)     2830 2020-08-23 06:09:19.000000 makefilemenu-0.4.2/README.md
-drwxr-xr-x   0 kkto      (1000) kkto      (1000)        0 2020-08-25 05:28:55.000000 makefilemenu-0.4.2/makefilemenu/
--rw-r--r--   0 kkto      (1000) kkto      (1000)     7239 2020-08-23 10:58:45.000000 makefilemenu-0.4.2/makefilemenu/__init__.py
--rw-r--r--   0 kkto      (1000) kkto      (1000)     2766 2020-08-25 05:26:12.000000 makefilemenu-0.4.2/makefilemenu/__main__.py
-drwxr-xr-x   0 kkto      (1000) kkto      (1000)        0 2020-08-25 05:28:55.000000 makefilemenu-0.4.2/makefilemenu.egg-info/
--rw-r--r--   0 kkto      (1000) kkto      (1000)     4323 2020-08-25 05:28:55.000000 makefilemenu-0.4.2/makefilemenu.egg-info/PKG-INFO
--rw-r--r--   0 kkto      (1000) kkto      (1000)      286 2020-08-25 05:28:55.000000 makefilemenu-0.4.2/makefilemenu.egg-info/SOURCES.txt
--rw-r--r--   0 kkto      (1000) kkto      (1000)        1 2020-08-25 05:28:55.000000 makefilemenu-0.4.2/makefilemenu.egg-info/dependency_links.txt
--rw-r--r--   0 kkto      (1000) kkto      (1000)       61 2020-08-25 05:28:55.000000 makefilemenu-0.4.2/makefilemenu.egg-info/entry_points.txt
--rw-r--r--   0 kkto      (1000) kkto      (1000)       11 2020-08-25 05:28:55.000000 makefilemenu-0.4.2/makefilemenu.egg-info/requires.txt
--rw-r--r--   0 kkto      (1000) kkto      (1000)       13 2020-08-25 05:28:55.000000 makefilemenu-0.4.2/makefilemenu.egg-info/top_level.txt
--rw-r--r--   0 kkto      (1000) kkto      (1000)       38 2020-08-25 05:28:55.000000 makefilemenu-0.4.2/setup.cfg
--rw-r--r--   0 kkto      (1000) kkto      (1000)     1118 2020-08-25 05:28:40.000000 makefilemenu-0.4.2/setup.py
+drwxr-xr-x   0 kkto      (1000) kkto      (1000)        0 2024-05-04 07:11:14.229388 makefilemenu-0.4.3/
+-rw-r--r--   0 kkto      (1000) kkto      (1000)     1064 2020-06-12 12:07:44.000000 makefilemenu-0.4.3/LICENSE
+-rw-r--r--   0 kkto      (1000) kkto      (1000)     3505 2024-05-04 07:11:14.229388 makefilemenu-0.4.3/PKG-INFO
+-rw-r--r--   0 kkto      (1000) kkto      (1000)     2830 2020-08-23 06:09:19.000000 makefilemenu-0.4.3/README.md
+drwxr-xr-x   0 kkto      (1000) kkto      (1000)        0 2024-05-04 07:11:14.229388 makefilemenu-0.4.3/makefilemenu/
+-rw-r--r--   0 kkto      (1000) kkto      (1000)     7239 2020-08-23 10:58:45.000000 makefilemenu-0.4.3/makefilemenu/__init__.py
+-rw-r--r--   0 kkto      (1000) kkto      (1000)     2766 2020-08-25 05:26:12.000000 makefilemenu-0.4.3/makefilemenu/__main__.py
+drwxr-xr-x   0 kkto      (1000) kkto      (1000)        0 2024-05-04 07:11:14.229388 makefilemenu-0.4.3/makefilemenu.egg-info/
+-rw-r--r--   0 kkto      (1000) kkto      (1000)     3505 2024-05-04 07:11:14.000000 makefilemenu-0.4.3/makefilemenu.egg-info/PKG-INFO
+-rw-r--r--   0 kkto      (1000) kkto      (1000)      294 2024-05-04 07:11:14.000000 makefilemenu-0.4.3/makefilemenu.egg-info/SOURCES.txt
+-rw-r--r--   0 kkto      (1000) kkto      (1000)        1 2024-05-04 07:11:14.000000 makefilemenu-0.4.3/makefilemenu.egg-info/dependency_links.txt
+-rw-r--r--   0 kkto      (1000) kkto      (1000)       60 2024-05-04 07:11:14.000000 makefilemenu-0.4.3/makefilemenu.egg-info/entry_points.txt
+-rw-r--r--   0 kkto      (1000) kkto      (1000)       11 2024-05-04 07:11:14.000000 makefilemenu-0.4.3/makefilemenu.egg-info/requires.txt
+-rw-r--r--   0 kkto      (1000) kkto      (1000)       13 2024-05-04 07:11:14.000000 makefilemenu-0.4.3/makefilemenu.egg-info/top_level.txt
+-rw-r--r--   0 kkto      (1000) kkto      (1000)       38 2024-05-04 07:11:14.229388 makefilemenu-0.4.3/setup.cfg
+-rw-r--r--   0 kkto      (1000) kkto      (1000)     1118 2024-05-04 07:10:50.000000 makefilemenu-0.4.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `makefilemenu-0.4.2/PKG-INFO` & `makefilemenu-0.4.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,118 @@
 Metadata-Version: 2.1
 Name: makefilemenu
-Version: 0.4.2
+Version: 0.4.3
 Summary: Console menu for Makefiles
 Home-page: https://github.com/isaacto/makefilemenu
 Author: Isaac To
 Author-email: isaac.to@gmail.com
-License: UNKNOWN
-Description: # makefilemenu
-        
-        Provide a console menu interface for a Makefile.
-        
-        The canonical use of the system is to have a quick and stupid way to
-        document commands one would like to run, while at the same time making
-        it extremely easy to run, without memorizing anything.  Because I'm
-        (ab)using "make", it is also very easy to run a particular target from
-        the command line without using the menu system.
-        
-        Of course nothing stops you from using the tool for a more regular
-        Makefile.
-        
-        ## Description
-        
-        This is a very simple system to create a menu from the Makefile.  You
-        annotate your Makefile as follows:
-        
-            # menu title: My title
-        
-            # menu item: a
-            .PHONY: hello
-            hello:
-            	echo hello world
-        
-            # menu item: b
-            .PHONY: foo
-            foo:
-            	echo foo bar
-        
-            # menu comment: Section 2
-        
-            # menu item: c
-            .PHONY: world
-            world:
-            	echo 42
-        
-        In other words, just add "# menu title" in the file once, and "# menu
-        item: &lt;ch&gt;" to create a command from a make file target.  Then
-        running "makefilemenu Makefile" shows:
-        
-            ===== My title =====
-            a: hello  b: foo  q: quit
-            Section 2
-            c: world
-        
-            Choice:
-        
-        You can choose one of the commands, and the corresponding target is
-        made.  Note that a "quit" command is automatically added to quit the
-        program.  If you don't want it, you can use "--quit_cmd ''" to disable
-        it.  In such case, to exit, press Control-C or Control-D.
-        
-        Regular "make" usage is not interfered, so you can still say "make foo
-        hello" on the command line to make both targets.
-        
-        You can also add a few clauses to the Makefile, so that running
-        makefilemenu is the default target, and your file can be simply
-        executed:
-        
-            #!/usr/bin/env -S make -f
-            # -*- makefile -*-
-        
-            thisfile := $(lastword $(MAKEFILE_LIST))
-        
-            .PHONY: menu
-            menu:
-            	@makefilemenu $(thisfile)
-        
-        ## Variables
-        
-        Two types of variables may be set using `makefilemenu`: environment
-        variables and Makefile variables.  Environment variables are set using
-        `# menu envvar`, like this.
-        
-            # menu envvar var
-            # menu envvar d:var
-        
-        This adds an initially unset variable `var`, and a menu entry to set
-        the variable.  In the first case the menu entry is invoked by `var`,
-        in the second case it is by `d`.
-        
-        You can set the initial value of the variable to be `val` as follows:
-        
-            # menu envvar var=val
-            # menu envvar d:var=val
-        
-        In this case, if an empty value is set on the command line, it is
-        given an empty value (if there is no default value, an empty value
-        would unset the variable).
-        
-        After the environment variable is given a value, when a command is
-        invoked the make command is invoked with the environment variable set.
-        
-        You can replace `envvar` by `makevar` in the `# menu` directive above.
-        In this case, the environment variable is not used, but instead the
-        `make` command is invoked like:
-        
-            make var=val ...
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: ~=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# makefilemenu
+
+Provide a console menu interface for a Makefile.
+
+The canonical use of the system is to have a quick and stupid way to
+document commands one would like to run, while at the same time making
+it extremely easy to run, without memorizing anything.  Because I'm
+(ab)using "make", it is also very easy to run a particular target from
+the command line without using the menu system.
+
+Of course nothing stops you from using the tool for a more regular
+Makefile.
+
+## Description
+
+This is a very simple system to create a menu from the Makefile.  You
+annotate your Makefile as follows:
+
+    # menu title: My title
+
+    # menu item: a
+    .PHONY: hello
+    hello:
+    	echo hello world
+
+    # menu item: b
+    .PHONY: foo
+    foo:
+    	echo foo bar
+
+    # menu comment: Section 2
+
+    # menu item: c
+    .PHONY: world
+    world:
+    	echo 42
+
+In other words, just add "# menu title" in the file once, and "# menu
+item: &lt;ch&gt;" to create a command from a make file target.  Then
+running "makefilemenu Makefile" shows:
+
+    ===== My title =====
+    a: hello  b: foo  q: quit
+    Section 2
+    c: world
+
+    Choice:
+
+You can choose one of the commands, and the corresponding target is
+made.  Note that a "quit" command is automatically added to quit the
+program.  If you don't want it, you can use "--quit_cmd ''" to disable
+it.  In such case, to exit, press Control-C or Control-D.
+
+Regular "make" usage is not interfered, so you can still say "make foo
+hello" on the command line to make both targets.
+
+You can also add a few clauses to the Makefile, so that running
+makefilemenu is the default target, and your file can be simply
+executed:
+
+    #!/usr/bin/env -S make -f
+    # -*- makefile -*-
+
+    thisfile := $(lastword $(MAKEFILE_LIST))
+
+    .PHONY: menu
+    menu:
+    	@makefilemenu $(thisfile)
+
+## Variables
+
+Two types of variables may be set using `makefilemenu`: environment
+variables and Makefile variables.  Environment variables are set using
+`# menu envvar`, like this.
+
+    # menu envvar var
+    # menu envvar d:var
+
+This adds an initially unset variable `var`, and a menu entry to set
+the variable.  In the first case the menu entry is invoked by `var`,
+in the second case it is by `d`.
+
+You can set the initial value of the variable to be `val` as follows:
+
+    # menu envvar var=val
+    # menu envvar d:var=val
+
+In this case, if an empty value is set on the command line, it is
+given an empty value (if there is no default value, an empty value
+would unset the variable).
+
+After the environment variable is given a value, when a command is
+invoked the make command is invoked with the environment variable set.
+
+You can replace `envvar` by `makevar` in the `# menu` directive above.
+In this case, the environment variable is not used, but instead the
+`make` command is invoked like:
+
+    make var=val ...
```

### Comparing `makefilemenu-0.4.2/README.md` & `makefilemenu-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `makefilemenu-0.4.2/makefilemenu/__init__.py` & `makefilemenu-0.4.3/makefilemenu/__init__.py`

 * *Files identical despite different names*

### Comparing `makefilemenu-0.4.2/makefilemenu/__main__.py` & `makefilemenu-0.4.3/makefilemenu/__main__.py`

 * *Files identical despite different names*

### Comparing `makefilemenu-0.4.2/makefilemenu.egg-info/PKG-INFO` & `makefilemenu-0.4.3/makefilemenu.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,118 @@
 Metadata-Version: 2.1
 Name: makefilemenu
-Version: 0.4.2
+Version: 0.4.3
 Summary: Console menu for Makefiles
 Home-page: https://github.com/isaacto/makefilemenu
 Author: Isaac To
 Author-email: isaac.to@gmail.com
-License: UNKNOWN
-Description: # makefilemenu
-        
-        Provide a console menu interface for a Makefile.
-        
-        The canonical use of the system is to have a quick and stupid way to
-        document commands one would like to run, while at the same time making
-        it extremely easy to run, without memorizing anything.  Because I'm
-        (ab)using "make", it is also very easy to run a particular target from
-        the command line without using the menu system.
-        
-        Of course nothing stops you from using the tool for a more regular
-        Makefile.
-        
-        ## Description
-        
-        This is a very simple system to create a menu from the Makefile.  You
-        annotate your Makefile as follows:
-        
-            # menu title: My title
-        
-            # menu item: a
-            .PHONY: hello
-            hello:
-            	echo hello world
-        
-            # menu item: b
-            .PHONY: foo
-            foo:
-            	echo foo bar
-        
-            # menu comment: Section 2
-        
-            # menu item: c
-            .PHONY: world
-            world:
-            	echo 42
-        
-        In other words, just add "# menu title" in the file once, and "# menu
-        item: &lt;ch&gt;" to create a command from a make file target.  Then
-        running "makefilemenu Makefile" shows:
-        
-            ===== My title =====
-            a: hello  b: foo  q: quit
-            Section 2
-            c: world
-        
-            Choice:
-        
-        You can choose one of the commands, and the corresponding target is
-        made.  Note that a "quit" command is automatically added to quit the
-        program.  If you don't want it, you can use "--quit_cmd ''" to disable
-        it.  In such case, to exit, press Control-C or Control-D.
-        
-        Regular "make" usage is not interfered, so you can still say "make foo
-        hello" on the command line to make both targets.
-        
-        You can also add a few clauses to the Makefile, so that running
-        makefilemenu is the default target, and your file can be simply
-        executed:
-        
-            #!/usr/bin/env -S make -f
-            # -*- makefile -*-
-        
-            thisfile := $(lastword $(MAKEFILE_LIST))
-        
-            .PHONY: menu
-            menu:
-            	@makefilemenu $(thisfile)
-        
-        ## Variables
-        
-        Two types of variables may be set using `makefilemenu`: environment
-        variables and Makefile variables.  Environment variables are set using
-        `# menu envvar`, like this.
-        
-            # menu envvar var
-            # menu envvar d:var
-        
-        This adds an initially unset variable `var`, and a menu entry to set
-        the variable.  In the first case the menu entry is invoked by `var`,
-        in the second case it is by `d`.
-        
-        You can set the initial value of the variable to be `val` as follows:
-        
-            # menu envvar var=val
-            # menu envvar d:var=val
-        
-        In this case, if an empty value is set on the command line, it is
-        given an empty value (if there is no default value, an empty value
-        would unset the variable).
-        
-        After the environment variable is given a value, when a command is
-        invoked the make command is invoked with the environment variable set.
-        
-        You can replace `envvar` by `makevar` in the `# menu` directive above.
-        In this case, the environment variable is not used, but instead the
-        `make` command is invoked like:
-        
-            make var=val ...
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: ~=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# makefilemenu
+
+Provide a console menu interface for a Makefile.
+
+The canonical use of the system is to have a quick and stupid way to
+document commands one would like to run, while at the same time making
+it extremely easy to run, without memorizing anything.  Because I'm
+(ab)using "make", it is also very easy to run a particular target from
+the command line without using the menu system.
+
+Of course nothing stops you from using the tool for a more regular
+Makefile.
+
+## Description
+
+This is a very simple system to create a menu from the Makefile.  You
+annotate your Makefile as follows:
+
+    # menu title: My title
+
+    # menu item: a
+    .PHONY: hello
+    hello:
+    	echo hello world
+
+    # menu item: b
+    .PHONY: foo
+    foo:
+    	echo foo bar
+
+    # menu comment: Section 2
+
+    # menu item: c
+    .PHONY: world
+    world:
+    	echo 42
+
+In other words, just add "# menu title" in the file once, and "# menu
+item: &lt;ch&gt;" to create a command from a make file target.  Then
+running "makefilemenu Makefile" shows:
+
+    ===== My title =====
+    a: hello  b: foo  q: quit
+    Section 2
+    c: world
+
+    Choice:
+
+You can choose one of the commands, and the corresponding target is
+made.  Note that a "quit" command is automatically added to quit the
+program.  If you don't want it, you can use "--quit_cmd ''" to disable
+it.  In such case, to exit, press Control-C or Control-D.
+
+Regular "make" usage is not interfered, so you can still say "make foo
+hello" on the command line to make both targets.
+
+You can also add a few clauses to the Makefile, so that running
+makefilemenu is the default target, and your file can be simply
+executed:
+
+    #!/usr/bin/env -S make -f
+    # -*- makefile -*-
+
+    thisfile := $(lastword $(MAKEFILE_LIST))
+
+    .PHONY: menu
+    menu:
+    	@makefilemenu $(thisfile)
+
+## Variables
+
+Two types of variables may be set using `makefilemenu`: environment
+variables and Makefile variables.  Environment variables are set using
+`# menu envvar`, like this.
+
+    # menu envvar var
+    # menu envvar d:var
+
+This adds an initially unset variable `var`, and a menu entry to set
+the variable.  In the first case the menu entry is invoked by `var`,
+in the second case it is by `d`.
+
+You can set the initial value of the variable to be `val` as follows:
+
+    # menu envvar var=val
+    # menu envvar d:var=val
+
+In this case, if an empty value is set on the command line, it is
+given an empty value (if there is no default value, an empty value
+would unset the variable).
+
+After the environment variable is given a value, when a command is
+invoked the make command is invoked with the environment variable set.
+
+You can replace `envvar` by `makevar` in the `# menu` directive above.
+In this case, the environment variable is not used, but instead the
+`make` command is invoked like:
+
+    make var=val ...
```

### Comparing `makefilemenu-0.4.2/setup.py` & `makefilemenu-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='makefilemenu',
-    version='0.4.2',
+    version='0.4.3',
     python_requires='~=3.5',
     author='Isaac To',
     author_email='isaac.to@gmail.com',
     description='Console menu for Makefiles',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/isaacto/makefilemenu',
```

