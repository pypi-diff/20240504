# Comparing `tmp/python_none_objects-1.1.8.tar.gz` & `tmp/python_none_objects-1.1.9.tar.gz`

## Comparing `python_none_objects-1.1.8.tar` & `python_none_objects-1.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/README_printable.md
--rwxr-xr-x   0        0        0     2468 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/build_and_checks.sh
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/wget_sha512.sh
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/src/python_none_objects/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/src/python_none_objects/py.typed
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/typing_test/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/COPYING.LESSER
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/README.md
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/pyproject.toml
--rw-r--r--   0        0        0    14879 2020-02-02 00:00:00.000000 python_none_objects-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 python_none_objects-1.1.9/README_printable.md
+-rwxr-xr-x   0        0        0     2467 2020-02-02 00:00:00.000000 python_none_objects-1.1.9/build_and_checks.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 python_none_objects-1.1.9/wget_sha512.sh
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 python_none_objects-1.1.9/src/python_none_objects/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_none_objects-1.1.9/src/python_none_objects/py.typed
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 python_none_objects-1.1.9/typing_test/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 python_none_objects-1.1.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_none_objects-1.1.9/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_none_objects-1.1.9/COPYING.LESSER
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 python_none_objects-1.1.9/README.md
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 python_none_objects-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0    14879 2020-02-02 00:00:00.000000 python_none_objects-1.1.9/PKG-INFO
```

### Comparing `python_none_objects-1.1.8/README_printable.md` & `python_none_objects-1.1.9/README_printable.md`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.8/build_and_checks.sh` & `python_none_objects-1.1.9/build_and_checks.sh`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # You should have received a copy of
 # the GNU Lesser General Public License
 # along with python-none-objects.
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
 pylint src/python_none_objects/
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

### Comparing `python_none_objects-1.1.8/wget_sha512.sh` & `python_none_objects-1.1.9/wget_sha512.sh`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.8/src/python_none_objects/__init__.py` & `python_none_objects-1.1.9/src/python_none_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.8/typing_test/__init__.py` & `python_none_objects-1.1.9/typing_test/__init__.py`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.8/COPYING` & `python_none_objects-1.1.9/COPYING`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.8/COPYING.LESSER` & `python_none_objects-1.1.9/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.8/README.md` & `python_none_objects-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.8/pyproject.toml` & `python_none_objects-1.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python-none-objects"
-version = "1.1.8"
+version = "1.1.9"
 description = """\
 Add more constant \"None\" objects to Python \
 to avoid boilerplate code\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
```

### Comparing `python_none_objects-1.1.8/PKG-INFO` & `python_none_objects-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-none-objects
-Version: 1.1.8
+Version: 1.1.9
 Summary: Add more constant "None" objects to Python to avoid boilerplate code
 Project-URL: Homepage, https://github.com/LLyaudet/python-none-objects
 Project-URL: Bug Tracker, https://github.com/LLyaudet/python-none-objects/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 Maintainer-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

