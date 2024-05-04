# Comparing `tmp/bluetooth_adapters-0.8.0.tar.gz` & `tmp/bluetooth_adapters-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetooth_adapters-0.8.0.tar", max compression
+gzip compressed data, was "bluetooth_adapters-0.9.0.tar", max compression
```

## Comparing `bluetooth_adapters-0.8.0.tar` & `bluetooth_adapters-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11345 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/LICENSE
--rw-r--r--   0        0        0     3617 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/README.md
--rw-r--r--   0        0        0     2466 2022-11-16 15:39:47.877511 bluetooth_adapters-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1160 2022-11-16 15:39:47.821510 bluetooth_adapters-0.8.0/src/bluetooth_adapters/__init__.py
--rw-r--r--   0        0        0      718 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/src/bluetooth_adapters/adapters.py
--rw-r--r--   0        0        0      354 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/src/bluetooth_adapters/const.py
--rw-r--r--   0        0        0     5270 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/src/bluetooth_adapters/dbus.py
--rw-r--r--   0        0        0     1927 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/src/bluetooth_adapters/history.py
--rw-r--r--   0        0        0      437 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/src/bluetooth_adapters/models.py
--rw-r--r--   0        0        0        0 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/src/bluetooth_adapters/py.typed
--rw-r--r--   0        0        0      459 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/src/bluetooth_adapters/systems/__init__.py
--rw-r--r--   0        0        0     1850 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/src/bluetooth_adapters/systems/linux.py
--rw-r--r--   0        0        0      747 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/src/bluetooth_adapters/systems/macos.py
--rw-r--r--   0        0        0      793 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/src/bluetooth_adapters/systems/windows.py
--rw-r--r--   0        0        0      452 2022-11-16 15:39:46.861490 bluetooth_adapters-0.8.0/src/bluetooth_adapters/util.py
--rw-r--r--   0        0        0     4675 1970-01-01 00:00:00.000000 bluetooth_adapters-0.8.0/setup.py
--rw-r--r--   0        0        0     5089 1970-01-01 00:00:00.000000 bluetooth_adapters-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11345 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3617 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/README.md
+-rw-r--r--   0        0        0     2490 2022-11-27 03:30:08.242303 bluetooth_adapters-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1160 2022-11-27 03:30:08.198303 bluetooth_adapters-0.9.0/src/bluetooth_adapters/__init__.py
+-rw-r--r--   0        0        0      718 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/src/bluetooth_adapters/adapters.py
+-rw-r--r--   0        0        0      354 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/src/bluetooth_adapters/const.py
+-rw-r--r--   0        0        0     5270 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/src/bluetooth_adapters/dbus.py
+-rw-r--r--   0        0        0     1927 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/src/bluetooth_adapters/history.py
+-rw-r--r--   0        0        0      703 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/src/bluetooth_adapters/models.py
+-rw-r--r--   0        0        0        0 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/src/bluetooth_adapters/py.typed
+-rw-r--r--   0        0        0      459 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/src/bluetooth_adapters/systems/__init__.py
+-rw-r--r--   0        0        0     3181 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/src/bluetooth_adapters/systems/linux.py
+-rw-r--r--   0        0        0      907 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/src/bluetooth_adapters/systems/macos.py
+-rw-r--r--   0        0        0      959 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/src/bluetooth_adapters/systems/windows.py
+-rw-r--r--   0        0        0      452 2022-11-27 03:30:07.330293 bluetooth_adapters-0.9.0/src/bluetooth_adapters/util.py
+-rw-r--r--   0        0        0     4700 1970-01-01 00:00:00.000000 bluetooth_adapters-0.9.0/setup.py
+-rw-r--r--   0        0        0     5126 1970-01-01 00:00:00.000000 bluetooth_adapters-0.9.0/PKG-INFO
```

### Comparing `bluetooth_adapters-0.8.0/LICENSE` & `bluetooth_adapters-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth_adapters-0.8.0/README.md` & `bluetooth_adapters-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bluetooth_adapters-0.8.0/pyproject.toml` & `bluetooth_adapters-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluetooth-adapters"
-version = "0.8.0"
+version = "0.9.0"
 description = "Tools to enumerate and find Bluetooth Adapters"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bluetooth-adapters"
 documentation = "https://bluetooth-adapters.readthedocs.io"
 classifiers = [
@@ -28,14 +28,15 @@
 # Documentation Dependencies
 Sphinx = {version = "^5.0", optional = true}
 sphinx-rtd-theme = {version = "^1.0", optional = true}
 myst-parser = {version = "^0.18", optional = true}
 async-timeout = ">=4.0.2"
 dbus-fast = ">=1.21.0"
 bleak = ">=0.15.1"
+usb-devices = ">=0.4.0"
 
 [tool.poetry.extras]
 docs = [
     "myst-parser",
     "sphinx",
     "sphinx-rtd-theme",
 ]
```

### Comparing `bluetooth_adapters-0.8.0/src/bluetooth_adapters/__init__.py` & `bluetooth_adapters-0.9.0/src/bluetooth_adapters/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 
 from .adapters import BluetoothAdapters
 from .const import (
     DEFAULT_ADDRESS,
     MACOS_DEFAULT_BLUETOOTH_ADAPTER,
     UNIX_DEFAULT_BLUETOOTH_ADAPTER,
```

### Comparing `bluetooth_adapters-0.8.0/src/bluetooth_adapters/adapters.py` & `bluetooth_adapters-0.9.0/src/bluetooth_adapters/adapters.py`

 * *Files identical despite different names*

### Comparing `bluetooth_adapters-0.8.0/src/bluetooth_adapters/dbus.py` & `bluetooth_adapters-0.9.0/src/bluetooth_adapters/dbus.py`

 * *Files identical despite different names*

### Comparing `bluetooth_adapters-0.8.0/src/bluetooth_adapters/history.py` & `bluetooth_adapters-0.9.0/src/bluetooth_adapters/history.py`

 * *Files identical despite different names*

### Comparing `bluetooth_adapters-0.8.0/src/bluetooth_adapters/systems/macos.py` & `bluetooth_adapters-0.9.0/src/bluetooth_adapters/systems/macos.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,18 @@
     def adapters(self) -> dict[str, AdapterDetails]:
         """Get the adapter details."""
         return {
             MACOS_DEFAULT_BLUETOOTH_ADAPTER: AdapterDetails(
                 address=DEFAULT_ADDRESS,
                 sw_version=platform.release(),
                 passive_scan=False,
+                manufacturer="Apple",
+                product="Unknown MacOS Model",
+                vendor_id="Unknown",
+                product_id="Unknown",
             )
         }
 
     @property
     def default_adapter(self) -> str:
         """Get the default adapter."""
         return MACOS_DEFAULT_BLUETOOTH_ADAPTER
```

### Comparing `bluetooth_adapters-0.8.0/src/bluetooth_adapters/systems/windows.py` & `bluetooth_adapters-0.9.0/src/bluetooth_adapters/systems/windows.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     def adapters(self) -> dict[str, AdapterDetails]:
         """Get the adapter details."""
         return {
             WINDOWS_DEFAULT_BLUETOOTH_ADAPTER: AdapterDetails(
                 address=DEFAULT_ADDRESS,
                 sw_version=platform.release(),
                 passive_scan=False,
+                manufacturer="Microsoft",
+                product="Unknown Windows Model",
+                vendor_id="Unknown",
+                product_id="Unknown",
             )
         }
 
     @property
     def default_adapter(self) -> str:
         """Get the default adapter."""
         return WINDOWS_DEFAULT_BLUETOOTH_ADAPTER
```

### Comparing `bluetooth_adapters-0.8.0/setup.py` & `bluetooth_adapters-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 packages = \
 ['bluetooth_adapters', 'bluetooth_adapters.systems']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['async-timeout>=4.0.2', 'bleak>=0.15.1', 'dbus-fast>=1.21.0']
+['async-timeout>=4.0.2',
+ 'bleak>=0.15.1',
+ 'dbus-fast>=1.21.0',
+ 'usb-devices>=0.4.0']
 
 extras_require = \
 {'docs': ['Sphinx>=5.0,<6.0',
           'sphinx-rtd-theme>=1.0,<2.0',
           'myst-parser>=0.18,<0.19']}
 
 setup_kwargs = {
     'name': 'bluetooth-adapters',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Tools to enumerate and find Bluetooth Adapters',
     'long_description': '# Bluetooth Adapters\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/bluetooth-adapters/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bluetooth-devices/bluetooth-adapters/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://bluetooth-adapters.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/bluetooth-adapters.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/bluetooth-adapters">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/bluetooth-adapters.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/bluetooth-adapters/">\n    <img src="https://img.shields.io/pypi/v/bluetooth-adapters.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/bluetooth-adapters.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/bluetooth-adapters.svg?style=flat-square" alt="License">\n</p>\n\nTools to enumerate and find Bluetooth Adapters\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install bluetooth-adapters`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bluetooth-devices/bluetooth-adapters',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['bluetooth_adapters', 'bluetooth_adapters.systems']
 package_data = \ {'': ['*']} install_requires = \ ['async-timeout>=4.0.2',
-'bleak>=0.15.1', 'dbus-fast>=1.21.0'] extras_require = \ {'docs':
-['Sphinx>=5.0,<6.0', 'sphinx-rtd-theme>=1.0,<2.0', 'myst-parser>=0.18,<0.19']}
-setup_kwargs = { 'name': 'bluetooth-adapters', 'version': '0.8.0',
-'description': 'Tools to enumerate and find Bluetooth Adapters',
+'bleak>=0.15.1', 'dbus-fast>=1.21.0', 'usb-devices>=0.4.0'] extras_require = \
+{'docs': ['Sphinx>=5.0,<6.0', 'sphinx-rtd-theme>=1.0,<2.0', 'myst-
+parser>=0.18,<0.19']} setup_kwargs = { 'name': 'bluetooth-adapters', 'version':
+'0.9.0', 'description': 'Tools to enumerate and find Bluetooth Adapters',
 'long_description': '# Bluetooth Adapters\n\n
     \n _\_n_ _[_C_I_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_T_e_s_t_ _c_o_v_e_r_a_g_e
                                _p_e_r_c_e_n_t_a_g_e_]_\_n_ \n
 \n
            \n _\_n_ _[_P_o_e_t_r_y_]_\_n_ \n _\_n_ _[_b_l_a_c_k_]_\_n_ \n _\_n_ _[_p_r_e_-_c_o_m_m_i_t_]_\_n_ \n
 \n
       \n _\_n_ _[_P_y_P_I_ _V_e_r_s_i_o_n_]_\_n_ \n [Supported Python versions]\n [License]\n
```

### Comparing `bluetooth_adapters-0.8.0/PKG-INFO` & `bluetooth_adapters-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetooth-adapters
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tools to enumerate and find Bluetooth Adapters
 Home-page: https://github.com/bluetooth-devices/bluetooth-adapters
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -20,14 +20,15 @@
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=5.0,<6.0); extra == "docs"
 Requires-Dist: async-timeout (>=4.0.2)
 Requires-Dist: bleak (>=0.15.1)
 Requires-Dist: dbus-fast (>=1.21.0)
 Requires-Dist: myst-parser (>=0.18,<0.19); extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0); extra == "docs"
+Requires-Dist: usb-devices (>=0.4.0)
 Project-URL: Bug Tracker, https://github.com/bluetooth-devices/bluetooth-adapters/issues
 Project-URL: Changelog, https://github.com/bluetooth-devices/bluetooth-adapters/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://bluetooth-adapters.readthedocs.io
 Project-URL: Repository, https://github.com/bluetooth-devices/bluetooth-adapters
 Description-Content-Type: text/markdown
 
 # Bluetooth Adapters
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: bluetooth-adapters Version: 0.8.0 Summary: Tools to
+Metadata-Version: 2.1 Name: bluetooth-adapters Version: 0.9.0 Summary: Tools to
 enumerate and find Bluetooth Adapters Home-page: https://github.com/bluetooth-
 devices/bluetooth-adapters License: Apache Software License 2.0 Author: J. Nick
 Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Software
 Development :: Libraries Provides-Extra: docs Requires-Dist: Sphinx
 (>=5.0,<6.0); extra == "docs" Requires-Dist: async-timeout (>=4.0.2) Requires-
 Dist: bleak (>=0.15.1) Requires-Dist: dbus-fast (>=1.21.0) Requires-Dist: myst-
 parser (>=0.18,<0.19); extra == "docs" Requires-Dist: sphinx-rtd-theme
-(>=1.0,<2.0); extra == "docs" Project-URL: Bug Tracker, https://github.com/
-bluetooth-devices/bluetooth-adapters/issues Project-URL: Changelog, https://
-github.com/bluetooth-devices/bluetooth-adapters/blob/main/CHANGELOG.md Project-
-URL: Documentation, https://bluetooth-adapters.readthedocs.io Project-URL:
-Repository, https://github.com/bluetooth-devices/bluetooth-adapters
-Description-Content-Type: text/markdown # Bluetooth Adapters
+(>=1.0,<2.0); extra == "docs" Requires-Dist: usb-devices (>=0.4.0) Project-URL:
+Bug Tracker, https://github.com/bluetooth-devices/bluetooth-adapters/issues
+Project-URL: Changelog, https://github.com/bluetooth-devices/bluetooth-
+adapters/blob/main/CHANGELOG.md Project-URL: Documentation, https://bluetooth-
+adapters.readthedocs.io Project-URL: Repository, https://github.com/bluetooth-
+devices/bluetooth-adapters Description-Content-Type: text/markdown # Bluetooth
+Adapters
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 Tools to enumerate and find Bluetooth Adapters ## Installation Install this via
 pip (or your favourite package manager): `pip install bluetooth-adapters` ##
 Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
 allcontributors.org/docs/en/emoji-key)): This project follows the [all-
```

