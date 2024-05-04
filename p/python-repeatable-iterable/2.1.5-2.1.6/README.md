# Comparing `tmp/python_repeatable_iterable-2.1.5.tar.gz` & `tmp/python_repeatable_iterable-2.1.6.tar.gz`

## Comparing `python_repeatable_iterable-2.1.5.tar` & `python_repeatable_iterable-2.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/CONTRIBUTORS.md
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/README_printable.md
--rwxr-xr-x   0        0        0     2503 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/build_and_checks.sh
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/wget_sha512.sh
--rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/src/python_repeatable_iterable/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/src/python_repeatable_iterable/py.typed
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/typing_test/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/COPYING.LESSER
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/README.md
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/pyproject.toml
--rw-r--r--   0        0        0    14586 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/README_printable.md
+-rwxr-xr-x   0        0        0     2502 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/build_and_checks.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/wget_sha512.sh
+-rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/src/python_repeatable_iterable/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/src/python_repeatable_iterable/py.typed
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/typing_test/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/COPYING.LESSER
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/README.md
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0    14586 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.6/PKG-INFO
```

### Comparing `python_repeatable_iterable-2.1.5/README_printable.md` & `python_repeatable_iterable-2.1.6/README_printable.md`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.5/build_and_checks.sh` & `python_repeatable_iterable-2.1.6/build_and_checks.sh`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # You should have received a copy of
 # the GNU Lesser General Public License
 # along with python-repeatable-iterable.
 # If not, see <http://www.gnu.org/licenses/>.
 #
 # ©Copyright 2023-2024 Laurent Lyaudet
 
+shopt -s globstar
 source ./wget_sha512.sh
 
 personal_github="https://raw.githubusercontent.com/LLyaudet/"
 
 echo "Building README.md"
 script="$personal_github""DevOrSysAdminScripts/main/build_readme.sh"
 correct_sha512="a7705592c14c7709f8762967f5c5d1c98d27b8ab97fe2aaa73302"
@@ -47,16 +48,14 @@
 echo "Running pylint"
 pylint src/python_repeatable_iterable/
 pylint typing_test/
 
 echo "Running mypy"
 mypy .
 
-shopt -s globstar
-
 echo "Analyzing too long lines"
 script="$personal_github"
 script+="DevOrSysAdminScripts/main/too_long_code_lines.sh"
 correct_sha512="eab26337506d6fabdea227c4b584391cc4a728e6b852be2232a7e"
 correct_sha512+="4d21261eb356df77257b0ea7152c9587ce89a963732fc644caf1"
 correct_sha512+="38c21ee51932e6fa6168bf9"
 wget_sha512 ./too_long_code_lines.sh "$script" "$correct_sha512"
```

### Comparing `python_repeatable_iterable-2.1.5/wget_sha512.sh` & `python_repeatable_iterable-2.1.6/wget_sha512.sh`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.5/src/python_repeatable_iterable/__init__.py` & `python_repeatable_iterable-2.1.6/src/python_repeatable_iterable/__init__.py`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.5/typing_test/__init__.py` & `python_repeatable_iterable-2.1.6/typing_test/__init__.py`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.5/COPYING` & `python_repeatable_iterable-2.1.6/COPYING`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.5/COPYING.LESSER` & `python_repeatable_iterable-2.1.6/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.5/README.md` & `python_repeatable_iterable-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.5/pyproject.toml` & `python_repeatable_iterable-2.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python-repeatable-iterable"
-version = "2.1.5"
+version = "2.1.6"
 description = """\
 Add a RepeatableIterable type and a function to obtain it\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
```

### Comparing `python_repeatable_iterable-2.1.5/PKG-INFO` & `python_repeatable_iterable-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-repeatable-iterable
-Version: 2.1.5
+Version: 2.1.6
 Summary: Add a RepeatableIterable type and a function to obtain it
 Project-URL: Homepage, https://github.com/LLyaudet/python-repeatable-iterable
 Project-URL: Bug Tracker, https://github.com/LLyaudet/python-repeatable-iterable/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 Maintainer-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

