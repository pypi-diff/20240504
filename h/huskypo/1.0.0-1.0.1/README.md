# Comparing `tmp/huskypo-1.0.0.tar.gz` & `tmp/huskypo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huskypo-1.0.0.tar", last modified: Sat May  4 02:50:22 2024, max compression
+gzip compressed data, was "huskypo-1.0.1.tar", last modified: Sat May  4 03:07:34 2024, max compression
```

## Comparing `huskypo-1.0.0.tar` & `huskypo-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-04 02:50:22.208192 huskypo-1.0.0/
--rw-r--r--   0 johnny     (501) staff       (20)    11357 2024-05-04 02:14:43.000000 huskypo-1.0.0/LICENSE
--rw-r--r--   0 johnny     (501) staff       (20)     4876 2024-05-04 02:50:22.207940 huskypo-1.0.0/PKG-INFO
--rw-r--r--   0 johnny     (501) staff       (20)     3754 2024-05-04 02:14:43.000000 huskypo-1.0.0/README.md
-drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-04 02:50:22.202528 huskypo-1.0.0/huskypo/
--rw-r--r--   0 johnny     (501) staff       (20)      208 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/__init__.py
--rw-r--r--   0 johnny     (501) staff       (20)      373 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/by.py
--rw-r--r--   0 johnny     (501) staff       (20)      374 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/config.py
--rw-r--r--   0 johnny     (501) staff       (20)      358 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/decorator.py
--rw-r--r--   0 johnny     (501) staff       (20)     5575 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/ec_extension.py
--rw-r--r--   0 johnny     (501) staff       (20)    42884 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/element.py
--rw-r--r--   0 johnny     (501) staff       (20)    18527 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/elements.py
-drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-04 02:50:22.207364 huskypo-1.0.0/huskypo/example/
--rw-r--r--   0 johnny     (501) staff       (20)        0 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/example/__init__.py
--rw-r--r--   0 johnny     (501) staff       (20)     2375 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/example/my_page.py
--rw-r--r--   0 johnny     (501) staff       (20)     1084 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/example/test_my_test.py
--rw-r--r--   0 johnny     (501) staff       (20)      575 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/logconfig.py
--rw-r--r--   0 johnny     (501) staff       (20)     4984 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/logstack.py
--rw-r--r--   0 johnny     (501) staff       (20)    33392 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/page.py
--rw-r--r--   0 johnny     (501) staff       (20)      564 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/typing.py
--rw-r--r--   0 johnny     (501) staff       (20)       17 2024-05-04 02:14:43.000000 huskypo-1.0.0/huskypo/version.py
-drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-04 02:50:22.207574 huskypo-1.0.0/huskypo.egg-info/
--rw-r--r--   0 johnny     (501) staff       (20)     4876 2024-05-04 02:50:22.000000 huskypo-1.0.0/huskypo.egg-info/PKG-INFO
--rw-r--r--   0 johnny     (501) staff       (20)      527 2024-05-04 02:50:22.000000 huskypo-1.0.0/huskypo.egg-info/SOURCES.txt
--rw-r--r--   0 johnny     (501) staff       (20)        1 2024-05-04 02:50:22.000000 huskypo-1.0.0/huskypo.egg-info/dependency_links.txt
--rw-r--r--   0 johnny     (501) staff       (20)        1 2024-05-04 02:50:22.000000 huskypo-1.0.0/huskypo.egg-info/not-zip-safe
--rw-r--r--   0 johnny     (501) staff       (20)       28 2024-05-04 02:50:22.000000 huskypo-1.0.0/huskypo.egg-info/requires.txt
--rw-r--r--   0 johnny     (501) staff       (20)        8 2024-05-04 02:50:22.000000 huskypo-1.0.0/huskypo.egg-info/top_level.txt
--rw-r--r--   0 johnny     (501) staff       (20)       38 2024-05-04 02:50:22.208235 huskypo-1.0.0/setup.cfg
--rw-r--r--   0 johnny     (501) staff       (20)     1487 2024-05-04 02:14:43.000000 huskypo-1.0.0/setup.py
+drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-04 03:07:34.586078 huskypo-1.0.1/
+-rw-r--r--   0 johnny     (501) staff       (20)    11357 2024-05-04 02:14:43.000000 huskypo-1.0.1/LICENSE
+-rw-r--r--   0 johnny     (501) staff       (20)     4876 2024-05-04 03:07:34.585864 huskypo-1.0.1/PKG-INFO
+-rw-r--r--   0 johnny     (501) staff       (20)     3754 2024-05-04 02:14:43.000000 huskypo-1.0.1/README.md
+drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-04 03:07:34.580914 huskypo-1.0.1/huskypo/
+-rw-r--r--   0 johnny     (501) staff       (20)      208 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/__init__.py
+-rw-r--r--   0 johnny     (501) staff       (20)      373 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/by.py
+-rw-r--r--   0 johnny     (501) staff       (20)      374 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/config.py
+-rw-r--r--   0 johnny     (501) staff       (20)      358 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/decorator.py
+-rw-r--r--   0 johnny     (501) staff       (20)     5575 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/ec_extension.py
+-rw-r--r--   0 johnny     (501) staff       (20)    42884 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/element.py
+-rw-r--r--   0 johnny     (501) staff       (20)    18527 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/elements.py
+drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-04 03:07:34.585289 huskypo-1.0.1/huskypo/example/
+-rw-r--r--   0 johnny     (501) staff       (20)        0 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/example/__init__.py
+-rw-r--r--   0 johnny     (501) staff       (20)     2375 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/example/my_page.py
+-rw-r--r--   0 johnny     (501) staff       (20)     1084 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/example/test_my_test.py
+-rw-r--r--   0 johnny     (501) staff       (20)      575 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/logconfig.py
+-rw-r--r--   0 johnny     (501) staff       (20)     4984 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/logstack.py
+-rw-r--r--   0 johnny     (501) staff       (20)    33331 2024-05-04 03:05:42.000000 huskypo-1.0.1/huskypo/page.py
+-rw-r--r--   0 johnny     (501) staff       (20)      564 2024-05-04 02:14:43.000000 huskypo-1.0.1/huskypo/typing.py
+-rw-r--r--   0 johnny     (501) staff       (20)       18 2024-05-04 03:06:59.000000 huskypo-1.0.1/huskypo/version.py
+drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-04 03:07:34.585532 huskypo-1.0.1/huskypo.egg-info/
+-rw-r--r--   0 johnny     (501) staff       (20)     4876 2024-05-04 03:07:34.000000 huskypo-1.0.1/huskypo.egg-info/PKG-INFO
+-rw-r--r--   0 johnny     (501) staff       (20)      527 2024-05-04 03:07:34.000000 huskypo-1.0.1/huskypo.egg-info/SOURCES.txt
+-rw-r--r--   0 johnny     (501) staff       (20)        1 2024-05-04 03:07:34.000000 huskypo-1.0.1/huskypo.egg-info/dependency_links.txt
+-rw-r--r--   0 johnny     (501) staff       (20)        1 2024-05-04 02:50:22.000000 huskypo-1.0.1/huskypo.egg-info/not-zip-safe
+-rw-r--r--   0 johnny     (501) staff       (20)       28 2024-05-04 03:07:34.000000 huskypo-1.0.1/huskypo.egg-info/requires.txt
+-rw-r--r--   0 johnny     (501) staff       (20)        8 2024-05-04 03:07:34.000000 huskypo-1.0.1/huskypo.egg-info/top_level.txt
+-rw-r--r--   0 johnny     (501) staff       (20)       38 2024-05-04 03:07:34.586121 huskypo-1.0.1/setup.cfg
+-rw-r--r--   0 johnny     (501) staff       (20)     1487 2024-05-04 02:14:43.000000 huskypo-1.0.1/setup.py
```

### Comparing `huskypo-1.0.0/LICENSE` & `huskypo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `huskypo-1.0.0/PKG-INFO` & `huskypo-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huskypo
-Version: 1.0.0
+Version: 1.0.1
 Summary: UI Automation Page Objects design pattern.
 Home-page: https://github.com/uujohnnyuu/huskyPO
 Author: Johnny
 Author-email: johnny071531@gmail.com
 License: Apache 2.0
 Keywords: huskypo,page object,selenium,appium,automation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `huskypo-1.0.0/README.md` & `huskypo-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `huskypo-1.0.0/huskypo/ec_extension.py` & `huskypo-1.0.1/huskypo/ec_extension.py`

 * *Files identical despite different names*

### Comparing `huskypo-1.0.0/huskypo/element.py` & `huskypo-1.0.1/huskypo/element.py`

 * *Files identical despite different names*

### Comparing `huskypo-1.0.0/huskypo/elements.py` & `huskypo-1.0.1/huskypo/elements.py`

 * *Files identical despite different names*

### Comparing `huskypo-1.0.0/huskypo/example/my_page.py` & `huskypo-1.0.1/huskypo/example/my_page.py`

 * *Files identical despite different names*

### Comparing `huskypo-1.0.0/huskypo/example/test_my_test.py` & `huskypo-1.0.1/huskypo/example/test_my_test.py`

 * *Files identical despite different names*

### Comparing `huskypo-1.0.0/huskypo/logconfig.py` & `huskypo-1.0.1/huskypo/logconfig.py`

 * *Files identical despite different names*

### Comparing `huskypo-1.0.0/huskypo/logstack.py` & `huskypo-1.0.1/huskypo/logstack.py`

 * *Files identical despite different names*

### Comparing `huskypo-1.0.0/huskypo/page.py` & `huskypo-1.0.1/huskypo/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.common.alert import Alert
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.actions import interaction
 from selenium.webdriver.common.actions.action_builder import ActionBuilder
 from selenium.webdriver.common.actions.pointer_input import PointerInput
 from selenium.webdriver.common.print_page_options import PrintOptions
-from appium.webdriver.common.touch_action import TouchAction
 
 from huskypo import ec_extension as ecex
 from huskypo.config import Timeout
 from huskypo.by import SwipeAction as SA
 from huskypo.typing import AppiumWebDriver, AppiumWebElement
 from huskypo.typing import WebDriver, WebElement, WebDriverTuple
```

### Comparing `huskypo-1.0.0/huskypo/typing.py` & `huskypo-1.0.1/huskypo/typing.py`

 * *Files identical despite different names*

### Comparing `huskypo-1.0.0/huskypo.egg-info/PKG-INFO` & `huskypo-1.0.1/huskypo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huskypo
-Version: 1.0.0
+Version: 1.0.1
 Summary: UI Automation Page Objects design pattern.
 Home-page: https://github.com/uujohnnyuu/huskyPO
 Author: Johnny
 Author-email: johnny071531@gmail.com
 License: Apache 2.0
 Keywords: huskypo,page object,selenium,appium,automation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `huskypo-1.0.0/huskypo.egg-info/SOURCES.txt` & `huskypo-1.0.1/huskypo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huskypo-1.0.0/setup.py` & `huskypo-1.0.1/setup.py`

 * *Files identical despite different names*

