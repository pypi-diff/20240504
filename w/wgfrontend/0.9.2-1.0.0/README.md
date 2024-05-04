# Comparing `tmp/wgfrontend-0.9.2.tar.gz` & `tmp/wgfrontend-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgfrontend-0.9.2.tar", last modified: Sat Nov 20 20:57:45 2021, max compression
+gzip compressed data, was "wgfrontend-1.0.0.tar", last modified: Sat May  4 18:28:04 2024, max compression
```

## Comparing `wgfrontend-0.9.2.tar` & `wgfrontend-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-20 20:57:45.253668 wgfrontend-0.9.2/
--rwxrw-r--   0 root         (0) root         (0)    34523 2020-11-19 20:46:23.000000 wgfrontend-0.9.2/LICENSE
--rwxrw-r--   0 root         (0) root         (0)      107 2020-12-02 20:41:03.000000 wgfrontend-0.9.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6597 2021-11-20 20:57:45.253668 wgfrontend-0.9.2/PKG-INFO
--rwxrw-r--   0 root         (0) root         (0)     4420 2021-03-05 20:03:30.000000 wgfrontend-0.9.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2021-11-20 20:57:45.253668 wgfrontend-0.9.2/setup.cfg
--rwxrw-r--   0 root         (0) root         (0)     1878 2021-11-20 20:53:38.000000 wgfrontend-0.9.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-20 20:57:44.225648 wgfrontend-0.9.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-20 20:57:44.565655 wgfrontend-0.9.2/src/wgfrontend/
--rwxrw-r--   0 root         (0) root         (0)     1167 2020-12-02 20:27:35.000000 wgfrontend-0.9.2/src/wgfrontend/__init__.py
--rwxrw-r--   0 root         (0) root         (0)     5271 2021-02-26 20:35:18.000000 wgfrontend-0.9.2/src/wgfrontend/config.py
--rwxrw-r--   0 root         (0) root         (0)     5169 2020-07-21 20:06:25.000000 wgfrontend-0.9.2/src/wgfrontend/exechelper.py
--rwxrw-r--   0 root         (0) root         (0)     1154 2020-11-19 18:31:07.000000 wgfrontend-0.9.2/src/wgfrontend/pwdtools.py
--rwxrw-r--   0 root         (0) root         (0)    20710 2021-11-20 20:53:11.000000 wgfrontend-0.9.2/src/wgfrontend/setupenv.py
--rwxrw-r--   0 root         (0) root         (0)     2387 2021-02-18 20:41:47.000000 wgfrontend-0.9.2/src/wgfrontend/setupenv_alpine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-20 20:57:45.189667 wgfrontend-0.9.2/src/wgfrontend/templates/
--rwxrw-r--   0 root         (0) root         (0)      612 2020-11-26 20:15:36.000000 wgfrontend-0.9.2/src/wgfrontend/templates/base.html
--rwxrw-r--   0 root         (0) root         (0)     1360 2020-11-25 21:42:40.000000 wgfrontend-0.9.2/src/wgfrontend/templates/config.html
--rwxrw-r--   0 root         (0) root         (0)     1472 2020-11-26 21:11:48.000000 wgfrontend-0.9.2/src/wgfrontend/templates/edit.html
--rwxrw-r--   0 root         (0) root         (0)     1416 2020-11-26 21:25:52.000000 wgfrontend-0.9.2/src/wgfrontend/templates/index.html
--rwxrw-r--   0 root         (0) root         (0)     1082 2020-11-26 20:44:54.000000 wgfrontend-0.9.2/src/wgfrontend/templates/login.html
--rwxrw-r--   0 root         (0) root         (0)      388 2020-11-26 19:22:44.000000 wgfrontend-0.9.2/src/wgfrontend/templates/part_header.html
--rwxrw-r--   0 root         (0) root         (0)     6599 2021-02-25 20:19:15.000000 wgfrontend-0.9.2/src/wgfrontend/webapp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-20 20:57:44.229648 wgfrontend-0.9.2/src/wgfrontend/webroot/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-20 20:57:45.233668 wgfrontend-0.9.2/src/wgfrontend/webroot/static/
--rwxrw-r--   0 root         (0) root         (0)     2238 2020-11-05 17:19:52.000000 wgfrontend-0.9.2/src/wgfrontend/webroot/static/favicon.ico
--rwxrw-r--   0 root         (0) root         (0)     7720 2020-04-30 09:19:08.000000 wgfrontend-0.9.2/src/wgfrontend/webroot/static/logo.svg
--rwxrw-r--   0 root         (0) root         (0)     3004 2020-11-27 07:58:49.000000 wgfrontend-0.9.2/src/wgfrontend/webroot/static/styles.css
--rwxrw-r--   0 root         (0) root         (0)     6693 2020-12-06 11:34:45.000000 wgfrontend-0.9.2/src/wgfrontend/wgcfg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-20 20:57:44.821660 wgfrontend-0.9.2/src/wgfrontend.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6597 2021-11-20 20:57:43.000000 wgfrontend-0.9.2/src/wgfrontend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      829 2021-11-20 20:57:43.000000 wgfrontend-0.9.2/src/wgfrontend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-20 20:57:43.000000 wgfrontend-0.9.2/src/wgfrontend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      131 2021-11-20 20:57:43.000000 wgfrontend-0.9.2/src/wgfrontend.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       37 2021-11-20 20:57:43.000000 wgfrontend-0.9.2/src/wgfrontend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2021-11-20 20:57:43.000000 wgfrontend-0.9.2/src/wgfrontend.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 18:28:04.741059 wgfrontend-1.0.0/
+-rwxrw-r--   0 root         (0) root         (0)    34523 2020-11-19 20:46:23.000000 wgfrontend-1.0.0/LICENSE
+-rwxrw-r--   0 root         (0) root         (0)      107 2020-12-02 20:41:03.000000 wgfrontend-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5593 2024-05-04 18:28:04.741059 wgfrontend-1.0.0/PKG-INFO
+-rwxrw-r--   0 root         (0) root         (0)     4420 2021-03-05 20:03:30.000000 wgfrontend-1.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-04 18:28:04.745059 wgfrontend-1.0.0/setup.cfg
+-rwxrw-r--   0 root         (0) root         (0)     1845 2024-05-04 18:25:31.000000 wgfrontend-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 18:28:04.649060 wgfrontend-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 18:28:04.685060 wgfrontend-1.0.0/src/wgfrontend/
+-rwxrw-r--   0 root         (0) root         (0)     1167 2022-07-04 10:17:32.000000 wgfrontend-1.0.0/src/wgfrontend/__init__.py
+-rwxrw-r--   0 root         (0) root         (0)     5271 2021-02-26 20:35:18.000000 wgfrontend-1.0.0/src/wgfrontend/config.py
+-rwxrw-r--   0 root         (0) root         (0)     5169 2020-07-21 20:06:25.000000 wgfrontend-1.0.0/src/wgfrontend/exechelper.py
+-rwxrw-r--   0 root         (0) root         (0)     1154 2020-11-19 18:31:07.000000 wgfrontend-1.0.0/src/wgfrontend/pwdtools.py
+-rwxrw-r--   0 root         (0) root         (0)    20710 2021-11-20 20:53:11.000000 wgfrontend-1.0.0/src/wgfrontend/setupenv.py
+-rwxrw-r--   0 root         (0) root         (0)     2387 2021-02-18 20:41:47.000000 wgfrontend-1.0.0/src/wgfrontend/setupenv_alpine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 18:28:04.725059 wgfrontend-1.0.0/src/wgfrontend/templates/
+-rwxrw-r--   0 root         (0) root         (0)      612 2020-11-26 20:15:36.000000 wgfrontend-1.0.0/src/wgfrontend/templates/base.html
+-rwxrw-r--   0 root         (0) root         (0)     1360 2020-11-25 21:42:40.000000 wgfrontend-1.0.0/src/wgfrontend/templates/config.html
+-rwxrw-r--   0 root         (0) root         (0)     1472 2020-11-26 21:11:48.000000 wgfrontend-1.0.0/src/wgfrontend/templates/edit.html
+-rwxrw-r--   0 root         (0) root         (0)     1416 2020-11-26 21:25:52.000000 wgfrontend-1.0.0/src/wgfrontend/templates/index.html
+-rwxrw-r--   0 root         (0) root         (0)     1082 2020-11-26 20:44:54.000000 wgfrontend-1.0.0/src/wgfrontend/templates/login.html
+-rwxrw-r--   0 root         (0) root         (0)      388 2020-11-26 19:22:44.000000 wgfrontend-1.0.0/src/wgfrontend/templates/part_header.html
+-rwxrw-r--   0 root         (0) root         (0)     6687 2022-09-15 20:10:05.000000 wgfrontend-1.0.0/src/wgfrontend/webapp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 18:28:04.653060 wgfrontend-1.0.0/src/wgfrontend/webroot/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 18:28:04.737059 wgfrontend-1.0.0/src/wgfrontend/webroot/static/
+-rwxrw-r--   0 root         (0) root         (0)     2238 2020-11-05 17:19:52.000000 wgfrontend-1.0.0/src/wgfrontend/webroot/static/favicon.ico
+-rwxrw-r--   0 root         (0) root         (0)     7720 2020-04-30 09:19:08.000000 wgfrontend-1.0.0/src/wgfrontend/webroot/static/logo.svg
+-rwxrw-r--   0 root         (0) root         (0)     3011 2024-05-04 18:06:51.000000 wgfrontend-1.0.0/src/wgfrontend/webroot/static/styles.css
+-rwxrw-r--   0 root         (0) root         (0)     6693 2020-12-06 11:34:45.000000 wgfrontend-1.0.0/src/wgfrontend/wgcfg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 18:28:04.705060 wgfrontend-1.0.0/src/wgfrontend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5593 2024-05-04 18:28:04.000000 wgfrontend-1.0.0/src/wgfrontend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      829 2024-05-04 18:28:04.000000 wgfrontend-1.0.0/src/wgfrontend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-04 18:28:04.000000 wgfrontend-1.0.0/src/wgfrontend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-04 18:28:04.000000 wgfrontend-1.0.0/src/wgfrontend.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-05-04 18:28:04.000000 wgfrontend-1.0.0/src/wgfrontend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-04 18:28:04.000000 wgfrontend-1.0.0/src/wgfrontend.egg-info/top_level.txt
```

### Comparing `wgfrontend-0.9.2/LICENSE` & `wgfrontend-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/PKG-INFO` & `wgfrontend-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,161 +1,164 @@
 Metadata-Version: 2.1
 Name: wgfrontend
-Version: 0.9.2
+Version: 1.0.0
 Summary: web-based user interface for configuring WireGuard for roadwarriors
 Home-page: https://www.github.com/towalink/wgfrontend
 Author: The Towalink Project
 Author-email: pypi.wgfrontend@towalink.net
-License: UNKNOWN
 Project-URL: Project homepage, https://www.towalink.net
 Project-URL: Repository, https://www.github.com/towalink/wgfrontend
 Project-URL: Documentation, https://towalink.readthedocs.io
-Description: # wgfrontend
-        
-        A simple web frontend for configuring peers within a WireGuard configuration file to thus administer road warrior clients.
-        
-        There are already a lot of user interfaces for administering WireGuard configuration files available. However, many of them have a bunch of dependencies, require root privileges to operate, or are a hassle to set up. "wgfrontend" provides a user interface that can be easily installed by just installing a package from Python's package repository PyPi (i.e. using pip).
-        
-        This little tool is independent of the Towalink site connectivity solution (see https://towalink.readthedocs.io).
-        
-        ---
-        
-        ## Features
-        
-        - Web frontend for adding, modifying, and deleting WireGuard peers
-        - Config files for WireGuard peers can be downloaded
-        - Config files for WireGuard peers are shown as QR Code
-        - Assistant for initial set-up
-        - Web frontend has responsive design
-        - Web frontend does not run with root privileges
-        - Simple installation
-        
-        ---
-        
-        ## Installation
-        
-        Install using PyPi:
-        
-        ```shell
-        pip3 install wgfrontend
-        ```
-        
-        Note: In the case you get an error regarding the imaging library needed for generating QR Codes, try to install it via the operating system packages:
-        
-        ```shell
-        # For Alpine:
-        apk add py3-pillow
-        # For Debian:
-        apt install python3-pil
-        ```
-        
-        ---
-        
-        ## Quickstart
-        
-        After installing "wgfrontend" as shown above, just execute the tool with root permissions to get started:
-        
-        ```shell
-        wgfrontend
-        ```
-        
-        An interactive set-up assistant queries for the needed configuration data and sets up the environment.
-        Once everything is configured, "wgfrontend" drops root privileges and runs a small web server on port 8080 to serve the web frontend.
-        
-        ---
-        
-        ## Screenshots
-        
-        ![screenshot: show a client config](https://raw.githubusercontent.com/towalink/wgfrontend/main/screenshots/show.png "Show a client config")
-        
-        See additional screenshots in the "screenshots" folder.
-        
-        ---
-        
-        ## Details
-        
-        ### The wgfrontend configuration file
-        
-        The interactive set-up assistant creates a configuration file with the desired information. It is located at "/etc/wgfrontend/wgfrontend.conf".
-        
-        Here is an example:
-        
-        ```
-        ### Config file of the Towalink WireGuard Frontend ###
-        [general]
-        # The WireGuard config file to read and write
-        wg_configfile = /etc/wireguard/wg_rw.conf
-        
-        # The command to be executed when the WireGuard config has changed
-        on_change_command = "sudo /etc/init.d/wgfrontend_interface restart"
-        
-        # The interface to bind to for the web server
-        socket_host = 0.0.0.0
-        
-        # The port to bind to for the web server
-        socket_port = 8080
-        
-        # The system user to be used for the frontend
-        user = wgfrontend
-        
-        [users]
-        admin = dc524e423d9762830649d4d9e18f4b47a56c92f96646104dd06c71b26b54f732e8318d5b60a6b2b01b4f269407771496e879c9bf65ca9ef4f55a243ff358fc8dfea0bd9d30d766320857093eb95022822f71b098215f26f6d2644033d956bfdd
-        ```
-        
-        ### Add an additional frontend user
-        
-        Create a password hash using the following command:
-        
-        ```shell
-        wgfrontend-password
-        ```
-        
-        Using this, you can add another user to the [users] section in the wgfrontend configuration file.
-        
-        ### A note on security
-        
-        Don't expose the web frontend to the Internet without another layer of protection.
-        
-        The wgfrontend web server does not run with root permissions. That's a start and better than many other WireGuard frontends. But the web server user has the permission to write to a WireGuard configuration file. This file may reference scripts that are run with root permissions when wg-quick is run. In case of a vulnerability in wgfrontend, this can be abused for privilege escalation. Thus add an additional safeguard layer of protection.
-        
-        ---
-        
-        ## Reporting bugs
-        
-        In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
-        
-        ---
-        
-        ## Developers
-        
-        ### Clone repository
-        
-        Clone this repo to your local machine using `https://github.com/towalink/wgfrontend.git`
-        
-        Install the module temporarily to make it available in your Python installation:
-        ```shell
-        pip3 install -e <path to directory with setup.py>
-        ```
-        
-        ---
-        
-        ## License
-        
-        [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
-        
-        - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
-        - Copyright 2020 © <a href="https://github.com/towalink/wgfrontend" target="_blank">Dirk Henrici</a>.
-        - [WireGuard](https://www.wireguard.com/) is a registered trademark of Jason A. Donenfeld.
-        
 Keywords: Towalink VPN WireGuard frontend gui
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cherrypy
+Requires-Dist: jinja2
+Requires-Dist: qrcode[pil]
+Requires-Dist: wgconfig
+
+# wgfrontend
+
+A simple web frontend for configuring peers within a WireGuard configuration file to thus administer road warrior clients.
+
+There are already a lot of user interfaces for administering WireGuard configuration files available. However, many of them have a bunch of dependencies, require root privileges to operate, or are a hassle to set up. "wgfrontend" provides a user interface that can be easily installed by just installing a package from Python's package repository PyPi (i.e. using pip).
+
+This little tool is independent of the Towalink site connectivity solution (see https://towalink.readthedocs.io).
+
+---
+
+## Features
+
+- Web frontend for adding, modifying, and deleting WireGuard peers
+- Config files for WireGuard peers can be downloaded
+- Config files for WireGuard peers are shown as QR Code
+- Assistant for initial set-up
+- Web frontend has responsive design
+- Web frontend does not run with root privileges
+- Simple installation
+
+---
+
+## Installation
+
+Install using PyPi:
+
+```shell
+pip3 install wgfrontend
+```
+
+Note: In the case you get an error regarding the imaging library needed for generating QR Codes, try to install it via the operating system packages:
+
+```shell
+# For Alpine:
+apk add py3-pillow
+# For Debian:
+apt install python3-pil
+```
+
+---
+
+## Quickstart
+
+After installing "wgfrontend" as shown above, just execute the tool with root permissions to get started:
+
+```shell
+wgfrontend
+```
+
+An interactive set-up assistant queries for the needed configuration data and sets up the environment.
+Once everything is configured, "wgfrontend" drops root privileges and runs a small web server on port 8080 to serve the web frontend.
+
+---
+
+## Screenshots
+
+![screenshot: show a client config](https://raw.githubusercontent.com/towalink/wgfrontend/main/screenshots/show.png "Show a client config")
+
+See additional screenshots in the "screenshots" folder.
+
+---
+
+## Details
+
+### The wgfrontend configuration file
+
+The interactive set-up assistant creates a configuration file with the desired information. It is located at "/etc/wgfrontend/wgfrontend.conf".
+
+Here is an example:
+
+```
+### Config file of the Towalink WireGuard Frontend ###
+[general]
+# The WireGuard config file to read and write
+wg_configfile = /etc/wireguard/wg_rw.conf
+
+# The command to be executed when the WireGuard config has changed
+on_change_command = "sudo /etc/init.d/wgfrontend_interface restart"
+
+# The interface to bind to for the web server
+socket_host = 0.0.0.0
+
+# The port to bind to for the web server
+socket_port = 8080
+
+# The system user to be used for the frontend
+user = wgfrontend
+
+[users]
+admin = dc524e423d9762830649d4d9e18f4b47a56c92f96646104dd06c71b26b54f732e8318d5b60a6b2b01b4f269407771496e879c9bf65ca9ef4f55a243ff358fc8dfea0bd9d30d766320857093eb95022822f71b098215f26f6d2644033d956bfdd
+```
+
+### Add an additional frontend user
+
+Create a password hash using the following command:
+
+```shell
+wgfrontend-password
+```
+
+Using this, you can add another user to the [users] section in the wgfrontend configuration file.
+
+### A note on security
+
+Don't expose the web frontend to the Internet without another layer of protection.
+
+The wgfrontend web server does not run with root permissions. That's a start and better than many other WireGuard frontends. But the web server user has the permission to write to a WireGuard configuration file. This file may reference scripts that are run with root permissions when wg-quick is run. In case of a vulnerability in wgfrontend, this can be abused for privilege escalation. Thus add an additional safeguard layer of protection.
+
+---
+
+## Reporting bugs
+
+In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
+
+---
+
+## Developers
+
+### Clone repository
+
+Clone this repo to your local machine using `https://github.com/towalink/wgfrontend.git`
+
+Install the module temporarily to make it available in your Python installation:
+```shell
+pip3 install -e <path to directory with setup.py>
+```
+
+---
+
+## License
+
+[![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
+
+- **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
+- Copyright 2020 © <a href="https://github.com/towalink/wgfrontend" target="_blank">Dirk Henrici</a>.
+- [WireGuard](https://www.wireguard.com/) is a registered trademark of Jason A. Donenfeld.
```

### Comparing `wgfrontend-0.9.2/README.md` & `wgfrontend-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/setup.py` & `wgfrontend-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'wgfrontend',
-    'version': '0.9.2',
+    'version': '1.0.0',
     'author': 'The Towalink Project',
     'author_email': 'pypi.wgfrontend@towalink.net',
     'description': 'web-based user interface for configuring WireGuard for roadwarriors',
     'long_description': long_description,
     'long_description_content_type': 'text/markdown',
     'url': 'https://www.github.com/towalink/wgfrontend',
-    'packages': setuptools.find_packages('src'),
+    'packages': setuptools.find_namespace_packages('src'),
     'package_dir': {'': 'src'},
     'include_package_data': True,
     'install_requires': ['cherrypy',
                          'jinja2',
                          'qrcode[pil]',
                          'wgconfig'
                         ],
@@ -28,16 +28,15 @@
         wgfrontend-password=pwdtools:hash_password_interactively
     ''',
     'classifiers': [
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: POSIX :: Linux',
-        'Development Status :: 4 - Beta',
-        #'Development Status :: 5 - Production/Stable',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: System Administrators',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Telecommunications Industry',
         'Topic :: System :: Networking'
     ],
     'python_requires': '>=3.6',
     'keywords': 'Towalink VPN WireGuard frontend gui',
```

### Comparing `wgfrontend-0.9.2/src/wgfrontend/__init__.py` & `wgfrontend-1.0.0/src/wgfrontend/__init__.py`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/config.py` & `wgfrontend-1.0.0/src/wgfrontend/config.py`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/exechelper.py` & `wgfrontend-1.0.0/src/wgfrontend/exechelper.py`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/pwdtools.py` & `wgfrontend-1.0.0/src/wgfrontend/pwdtools.py`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/setupenv.py` & `wgfrontend-1.0.0/src/wgfrontend/setupenv.py`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/setupenv_alpine.py` & `wgfrontend-1.0.0/src/wgfrontend/setupenv_alpine.py`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/templates/base.html` & `wgfrontend-1.0.0/src/wgfrontend/templates/base.html`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/templates/config.html` & `wgfrontend-1.0.0/src/wgfrontend/templates/config.html`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/templates/edit.html` & `wgfrontend-1.0.0/src/wgfrontend/templates/edit.html`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/templates/index.html` & `wgfrontend-1.0.0/src/wgfrontend/templates/index.html`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/templates/login.html` & `wgfrontend-1.0.0/src/wgfrontend/templates/login.html`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/webapp.py` & `wgfrontend-1.0.0/src/wgfrontend/webapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,16 @@
     # Configure the web application
     app_conf = {
       'global': {
          'environment' : 'production'
        },
        '/': {
             'tools.sessions.on': True,
+            'tools.sessions.secure': True,
+            'tools.sessions.httponly': True,
             'tools.staticdir.root': os.path.join(script_path, 'webroot'),
             'tools.session_auth.on': True,
             'tools.session_auth.login_screen': app.login_screen,
             'tools.session_auth.check_username_and_password': app.check_username_and_password,
             },
         '/configs': {
             'tools.staticdir.on': True,
```

### Comparing `wgfrontend-0.9.2/src/wgfrontend/webroot/static/favicon.ico` & `wgfrontend-1.0.0/src/wgfrontend/webroot/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/webroot/static/logo.svg` & `wgfrontend-1.0.0/src/wgfrontend/webroot/static/logo.svg`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend/webroot/static/styles.css` & `wgfrontend-1.0.0/src/wgfrontend/webroot/static/styles.css`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 html {
   font: normal 16px sans-serif;
   background-color: #f3f3f3;
   color: #000;
 }
 
+body {
+  min-height: 100vh;
+  display: flex;
+  flex-direction: column;
+}
+
 a {
   text-decoration: none;
   color: inherit;
   cursor: pointer;
   opacity: 0.9;
 }
 
@@ -115,15 +121,15 @@
 .user {
   color: blue;
   font-size: 14px;
 }
 
 section {
   width: 100%;
-  display: flex;
+  flex: 1;
   padding: 10px 250px;
   background-color: #f3f3f3;
 }
 
 .content {
   width: 100%;
 }
@@ -165,32 +171,27 @@
   padding: 5px 5px;
 }
 
 .instructions {
   font-size: 14px;
 }
 
-
 @media screen and (max-width: 1000px) {
   .table, .table-row {
     display: block;
   }
   .table-cell {
     display: block;
   }
   .bordertop2{
     border-top: 0;
   }
 }
 
-
 footer {
-  position: fixed;
-  left: 0;
-  bottom: 0;
   width: 100%;
   background-color: #dddddd;
   color: blue;
   font-size: 12px;
   text-align: center;
   padding: 3px 5px;
 }
@@ -202,18 +203,18 @@
   section {
     padding: 10px 100px;
   }
 }
 
 @media screen and (max-width: 500px) {
   header {
-    flex-direction: column;        
+    flex-direction: column;
     padding: 10px 10px;
   }
   header h2 {
     margin-bottom: 15px;
   }
   section {
-    flex-direction: column;        
+    flex-direction: column;
     padding: 10px 10px;
   }
 }
```

### Comparing `wgfrontend-0.9.2/src/wgfrontend/wgcfg.py` & `wgfrontend-1.0.0/src/wgfrontend/wgcfg.py`

 * *Files identical despite different names*

### Comparing `wgfrontend-0.9.2/src/wgfrontend.egg-info/PKG-INFO` & `wgfrontend-1.0.0/src/wgfrontend.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,161 +1,164 @@
 Metadata-Version: 2.1
 Name: wgfrontend
-Version: 0.9.2
+Version: 1.0.0
 Summary: web-based user interface for configuring WireGuard for roadwarriors
 Home-page: https://www.github.com/towalink/wgfrontend
 Author: The Towalink Project
 Author-email: pypi.wgfrontend@towalink.net
-License: UNKNOWN
 Project-URL: Project homepage, https://www.towalink.net
 Project-URL: Repository, https://www.github.com/towalink/wgfrontend
 Project-URL: Documentation, https://towalink.readthedocs.io
-Description: # wgfrontend
-        
-        A simple web frontend for configuring peers within a WireGuard configuration file to thus administer road warrior clients.
-        
-        There are already a lot of user interfaces for administering WireGuard configuration files available. However, many of them have a bunch of dependencies, require root privileges to operate, or are a hassle to set up. "wgfrontend" provides a user interface that can be easily installed by just installing a package from Python's package repository PyPi (i.e. using pip).
-        
-        This little tool is independent of the Towalink site connectivity solution (see https://towalink.readthedocs.io).
-        
-        ---
-        
-        ## Features
-        
-        - Web frontend for adding, modifying, and deleting WireGuard peers
-        - Config files for WireGuard peers can be downloaded
-        - Config files for WireGuard peers are shown as QR Code
-        - Assistant for initial set-up
-        - Web frontend has responsive design
-        - Web frontend does not run with root privileges
-        - Simple installation
-        
-        ---
-        
-        ## Installation
-        
-        Install using PyPi:
-        
-        ```shell
-        pip3 install wgfrontend
-        ```
-        
-        Note: In the case you get an error regarding the imaging library needed for generating QR Codes, try to install it via the operating system packages:
-        
-        ```shell
-        # For Alpine:
-        apk add py3-pillow
-        # For Debian:
-        apt install python3-pil
-        ```
-        
-        ---
-        
-        ## Quickstart
-        
-        After installing "wgfrontend" as shown above, just execute the tool with root permissions to get started:
-        
-        ```shell
-        wgfrontend
-        ```
-        
-        An interactive set-up assistant queries for the needed configuration data and sets up the environment.
-        Once everything is configured, "wgfrontend" drops root privileges and runs a small web server on port 8080 to serve the web frontend.
-        
-        ---
-        
-        ## Screenshots
-        
-        ![screenshot: show a client config](https://raw.githubusercontent.com/towalink/wgfrontend/main/screenshots/show.png "Show a client config")
-        
-        See additional screenshots in the "screenshots" folder.
-        
-        ---
-        
-        ## Details
-        
-        ### The wgfrontend configuration file
-        
-        The interactive set-up assistant creates a configuration file with the desired information. It is located at "/etc/wgfrontend/wgfrontend.conf".
-        
-        Here is an example:
-        
-        ```
-        ### Config file of the Towalink WireGuard Frontend ###
-        [general]
-        # The WireGuard config file to read and write
-        wg_configfile = /etc/wireguard/wg_rw.conf
-        
-        # The command to be executed when the WireGuard config has changed
-        on_change_command = "sudo /etc/init.d/wgfrontend_interface restart"
-        
-        # The interface to bind to for the web server
-        socket_host = 0.0.0.0
-        
-        # The port to bind to for the web server
-        socket_port = 8080
-        
-        # The system user to be used for the frontend
-        user = wgfrontend
-        
-        [users]
-        admin = dc524e423d9762830649d4d9e18f4b47a56c92f96646104dd06c71b26b54f732e8318d5b60a6b2b01b4f269407771496e879c9bf65ca9ef4f55a243ff358fc8dfea0bd9d30d766320857093eb95022822f71b098215f26f6d2644033d956bfdd
-        ```
-        
-        ### Add an additional frontend user
-        
-        Create a password hash using the following command:
-        
-        ```shell
-        wgfrontend-password
-        ```
-        
-        Using this, you can add another user to the [users] section in the wgfrontend configuration file.
-        
-        ### A note on security
-        
-        Don't expose the web frontend to the Internet without another layer of protection.
-        
-        The wgfrontend web server does not run with root permissions. That's a start and better than many other WireGuard frontends. But the web server user has the permission to write to a WireGuard configuration file. This file may reference scripts that are run with root permissions when wg-quick is run. In case of a vulnerability in wgfrontend, this can be abused for privilege escalation. Thus add an additional safeguard layer of protection.
-        
-        ---
-        
-        ## Reporting bugs
-        
-        In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
-        
-        ---
-        
-        ## Developers
-        
-        ### Clone repository
-        
-        Clone this repo to your local machine using `https://github.com/towalink/wgfrontend.git`
-        
-        Install the module temporarily to make it available in your Python installation:
-        ```shell
-        pip3 install -e <path to directory with setup.py>
-        ```
-        
-        ---
-        
-        ## License
-        
-        [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
-        
-        - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
-        - Copyright 2020 © <a href="https://github.com/towalink/wgfrontend" target="_blank">Dirk Henrici</a>.
-        - [WireGuard](https://www.wireguard.com/) is a registered trademark of Jason A. Donenfeld.
-        
 Keywords: Towalink VPN WireGuard frontend gui
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cherrypy
+Requires-Dist: jinja2
+Requires-Dist: qrcode[pil]
+Requires-Dist: wgconfig
+
+# wgfrontend
+
+A simple web frontend for configuring peers within a WireGuard configuration file to thus administer road warrior clients.
+
+There are already a lot of user interfaces for administering WireGuard configuration files available. However, many of them have a bunch of dependencies, require root privileges to operate, or are a hassle to set up. "wgfrontend" provides a user interface that can be easily installed by just installing a package from Python's package repository PyPi (i.e. using pip).
+
+This little tool is independent of the Towalink site connectivity solution (see https://towalink.readthedocs.io).
+
+---
+
+## Features
+
+- Web frontend for adding, modifying, and deleting WireGuard peers
+- Config files for WireGuard peers can be downloaded
+- Config files for WireGuard peers are shown as QR Code
+- Assistant for initial set-up
+- Web frontend has responsive design
+- Web frontend does not run with root privileges
+- Simple installation
+
+---
+
+## Installation
+
+Install using PyPi:
+
+```shell
+pip3 install wgfrontend
+```
+
+Note: In the case you get an error regarding the imaging library needed for generating QR Codes, try to install it via the operating system packages:
+
+```shell
+# For Alpine:
+apk add py3-pillow
+# For Debian:
+apt install python3-pil
+```
+
+---
+
+## Quickstart
+
+After installing "wgfrontend" as shown above, just execute the tool with root permissions to get started:
+
+```shell
+wgfrontend
+```
+
+An interactive set-up assistant queries for the needed configuration data and sets up the environment.
+Once everything is configured, "wgfrontend" drops root privileges and runs a small web server on port 8080 to serve the web frontend.
+
+---
+
+## Screenshots
+
+![screenshot: show a client config](https://raw.githubusercontent.com/towalink/wgfrontend/main/screenshots/show.png "Show a client config")
+
+See additional screenshots in the "screenshots" folder.
+
+---
+
+## Details
+
+### The wgfrontend configuration file
+
+The interactive set-up assistant creates a configuration file with the desired information. It is located at "/etc/wgfrontend/wgfrontend.conf".
+
+Here is an example:
+
+```
+### Config file of the Towalink WireGuard Frontend ###
+[general]
+# The WireGuard config file to read and write
+wg_configfile = /etc/wireguard/wg_rw.conf
+
+# The command to be executed when the WireGuard config has changed
+on_change_command = "sudo /etc/init.d/wgfrontend_interface restart"
+
+# The interface to bind to for the web server
+socket_host = 0.0.0.0
+
+# The port to bind to for the web server
+socket_port = 8080
+
+# The system user to be used for the frontend
+user = wgfrontend
+
+[users]
+admin = dc524e423d9762830649d4d9e18f4b47a56c92f96646104dd06c71b26b54f732e8318d5b60a6b2b01b4f269407771496e879c9bf65ca9ef4f55a243ff358fc8dfea0bd9d30d766320857093eb95022822f71b098215f26f6d2644033d956bfdd
+```
+
+### Add an additional frontend user
+
+Create a password hash using the following command:
+
+```shell
+wgfrontend-password
+```
+
+Using this, you can add another user to the [users] section in the wgfrontend configuration file.
+
+### A note on security
+
+Don't expose the web frontend to the Internet without another layer of protection.
+
+The wgfrontend web server does not run with root permissions. That's a start and better than many other WireGuard frontends. But the web server user has the permission to write to a WireGuard configuration file. This file may reference scripts that are run with root permissions when wg-quick is run. In case of a vulnerability in wgfrontend, this can be abused for privilege escalation. Thus add an additional safeguard layer of protection.
+
+---
+
+## Reporting bugs
+
+In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
+
+---
+
+## Developers
+
+### Clone repository
+
+Clone this repo to your local machine using `https://github.com/towalink/wgfrontend.git`
+
+Install the module temporarily to make it available in your Python installation:
+```shell
+pip3 install -e <path to directory with setup.py>
+```
+
+---
+
+## License
+
+[![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
+
+- **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
+- Copyright 2020 © <a href="https://github.com/towalink/wgfrontend" target="_blank">Dirk Henrici</a>.
+- [WireGuard](https://www.wireguard.com/) is a registered trademark of Jason A. Donenfeld.
```

### Comparing `wgfrontend-0.9.2/src/wgfrontend.egg-info/SOURCES.txt` & `wgfrontend-1.0.0/src/wgfrontend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

