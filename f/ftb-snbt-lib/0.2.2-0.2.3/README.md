# Comparing `tmp/ftb-snbt-lib-0.2.2.tar.gz` & `tmp/ftb_snbt_lib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftb-snbt-lib-0.2.2.tar", last modified: Sun Apr  7 05:23:04 2024, max compression
+gzip compressed data, was "ftb_snbt_lib-0.2.3.tar", last modified: Sat May  4 16:51:57 2024, max compression
```

## Comparing `ftb-snbt-lib-0.2.2.tar` & `ftb_snbt_lib-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:23:04.720735 ftb-snbt-lib-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-07 05:23:04.720735 ftb-snbt-lib-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:23:04.716735 ftb-snbt-lib-0.2.2/ftb_snbt_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/parsetab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:23:04.720735 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33639 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/ctokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    42905 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/lex.py
--rw-r--r--   0 runner    (1001) docker     (127)   137736 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/yacc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/ygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:23:04.720735 ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-07 05:23:04.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-07 05:23:04.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 05:23:04.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 05:23:04.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-07 05:23:04.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 05:23:04.720735 ftb-snbt-lib-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:51:57.149058 ftb_snbt_lib-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-04 16:51:57.149058 ftb_snbt_lib-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:51:57.145058 ftb_snbt_lib-0.2.3/ftb_snbt_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/parsetab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:51:57.145058 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33639 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/ctokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42905 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137736 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/yacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/ygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:51:57.145058 ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-04 16:51:57.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-04 16:51:57.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:51:57.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 16:51:57.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 16:51:57.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 16:51:57.149058 ftb_snbt_lib-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/setup.py
```

### Comparing `ftb-snbt-lib-0.2.2/LICENSE` & `ftb_snbt_lib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.2/PKG-INFO` & `ftb_snbt_lib-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftb-snbt-lib
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python library to parse, edit, and save FTB snbt tag, which is a variant of the "vanilla" snbt tag.
 Author-email: peunsu <peunsu55@gmail.com>
 Project-URL: homepage, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: repository, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: documentation, https://github.com/peunsu/ftb-snbt-lib
 Keywords: minecraft,ftb,snbt,parser,library
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 License-File: LICENSE
 Requires-Dist: wheel
 
 # ftb-snbt-lib
 
 ![GitHub Release](https://img.shields.io/github/v/release/peunsu/ftb-snbt-lib?style=for-the-badge)
 
-A python library to parse, edit, and save FTB snbt tag.
+**A python library to parse, edit, and save FTB snbt tag.**
 
 The FTB snbt tag is a variant of the "vanilla" snbt tag. It has no commas at end of lines, different suffixes for numeric values, and no support for array data type.
 
 This is the example of the FTB snbt tag:
 ```python
 {
     some_tag: "some_value"
@@ -43,81 +43,85 @@
 ```bash
 $ pip install ftb-snbt-lib
 ```
 
 ## Getting Started
 * Import the library.
 ```python
->>> import ftb_snbt_lib
+>>> import ftb_snbt_lib as slib
 ```
 
 * ``load(fp)``: Load the ftb snbt tag from a file (``fp``).
 ```python
->>> some_snbt = ftb_snbt_lib.load(open("tests/some_file.snbt", "r", encoding="utf-8"))
+>>> some_snbt = slib.load(open("tests/some_file.snbt", "r", encoding="utf-8"))
 ```
 * The type of returned value is ``Compound``, a dictionary-like object.<br>
 The ``Compound`` is containing values with **[tag data types](#data-types)** provided by this library.
 ```python
 >>> type(some_snbt)
-<class 'ftb_snbt.tag.Compound'>
+<class 'ftb_snbt_lib.tag.Compound'>
 >>> print(some_snbt)
 Compound({'some_tag': String('some_value'), 'another_tag': Byte(1)})
 ```
 
 * ``dump(tag, fp)``: Dump the ftb snbt tag to a file (``fp``).
 ```python
->>> ftb_snbt_lib.dump(some_snbt, open("tests/some_file_copy.snbt", "w", encoding="utf-8"))
+>>> slib.dump(some_snbt, open("tests/some_file_copy.snbt", "w", encoding="utf-8"))
 ```
 
 * ``loads(s)``: Load the ftb snbt tag from a string ``s``.
 ```python
->>> another_snbt = ftb_snbt_lib.loads('''
+>>> another_snbt = slib.loads('''
 ... {
 ...     some_tag: "some_value"
 ...     another_tag: 1b
 ... }
 ... ''')
 ```
 
 * ``dumps(tag)``: Dump the ftb snbt tag to a string.
 ```python
->>> dumped_snbt = ftb_snbt_lib.dumps(another_snbt)
+>>> dumped_snbt = slib.dumps(another_snbt)
 >>> print(dumped_snbt)
 {
     some_tag: "some_value"
     another_tag: 1b
 }
 ```
 
 * Edit the snbt tag. As its type is ``Compound``, it can be edited like a dictionary.<br>
 The inserted or replace values should be any of **[tag data types](#data-types)** provided by this library.
 ```python
->>> another_snbt["some_tag"] = ftb_snbt_lib.String("another_value")
+>>> another_snbt["some_tag"] = slib.String("another_value")
 ```
 
 * When editing the ``List``, a list-like object, its elements must have **the same type**.<br>
 For instance, ``List[Byte(1), Byte(2), Byte(3)]`` must contain **only** the ``Byte`` type object, so the other types like ``Integer`` or ``String`` **cannot be added or replaced** in it.
 
+* When editing the ``Array``, a list-like object with **a fixed length**, its elements must have **the same type**, and that type must **match the element type defined in the array**.<br>
+For instance, ``IntArray`` with a length of 3 must contain **three** ``Integer`` type objects, so **adding new objects, removing existing objects, and replacing with other type objects are not allowed**.
+
 * Save the edited snbt tag to a json file.
 ```python
 >>> import json
 >>> json.dump(another_snbt, open("tests/test.json", "w", encoding="utf-8"), indent=4, ensure_ascii=False)
 ```
 
 ## Data Types
 | Type | Description | Format | Example |
 | - | - | - | - |
 | Byte | A signed 8-bit integer.<br>Range: ``-128`` ~ ``127`` | ``<number>b`` | ``12b``, ``-35b`` |
 | Short | A signed 16-bit integer.<br>Range: ``-32,768`` ~ ``32,767`` | ``<number>s`` | ``132s``, ``-243s`` |
 | Integer | A signed 32-bit integer.<br>Range: ``-2,147,483,647`` ~ ``2,147,483,647`` | ``<number>`` | ``12345`` |
 | Long | A signed 64-bit integer.<br>Range: ``9,223,372,036,854,775,808`` ~ ``9,223,372,036,854,775,807`` | ``<number>L`` | ``12345L`` |
-| Float | A 32-bit, single-precision floating-point number.<br>Range: ``-3.4E+38`` ~ ``+3.4E+38`` | ``<number>f`` | ``12.345f`` |
-| Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308`` | ``<number>d`` | ``12.345d`` |
+| Float | A 32-bit, single-precision floating-point number.<br>Range: ``-3.4E+38`` ~ ``+3.4E+38`` | ``<number>f`` | ``12.345f``, ``1.0E-6f`` |
+| Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308`` | ``<number>d`` | ``12.345d``, ``1.0E-6d`` |
 | Bool | A boolean data type.<br>``0`` for ``false``, ``1`` for ``true``. | ``false``, ``true`` | ``true`` |
 | String | A sequence of characters. | A string enclosed in **double quotes ``""``**.<br>Nested double quotes can be included within a string using a **escaping character ``\"``**. | `"Hello, World!"`,<br>`"Say \"Hello, World!\""` |
 | List | An ordered list of tags.<br>The tags must be of **the same type**, determined by the first tag in the list. | Unnamed tags enclosed in square brackets and delimited by **newline** characters (``\n``). | <pre>[<br>    3.2d<br>    1.4d<br>    ...<br>]</pre> |
-| Array | An ordered list of 8-bit(ByteArray), 32-bit(IntArray), 64-bit(LongArray) integers. | ``<array_prefix>;`` followed by an ordered list of tags enclosed in square brackets and delimited by **newline** characters (``\n``).<br>Valid array prefixes are ``B``(Byte), ``I``(Integer), and ``L``(Long). | <pre>[B;<br>    12b<br>    -35b<br>    ...<br>]</pre> |
+| Array | An ordered list of 8-bit(``ByteArray``), 32-bit(``IntArray``), 64-bit(``LongArray``) integers. | ``<array_prefix>;`` followed by an ordered list of tags enclosed in square brackets and delimited by **newline** characters (``\n``).<br>Valid array prefixes are ``B``(Byte), ``I``(Integer), and ``L``(Long). | <pre>[B;<br>    12b<br>    -35b<br>    ...<br>]</pre> |
 | Compound | An ordered list of attribute-value pairs.<br>Each tag can be of **any type**. | Named tags enclosed in curly braces and delimited by commas or **newline** characters (``\n``).<br>The key (tag name) can be unquoted if it contains only ``0-9``, ``A-Z``, ``a-z``, ``_``, ``-``, ``.``, and ``+``. Otherwise the key should be quoted, using the format of ``String`` type. | <pre>[<br>    tag1: "string"<br>    tag2: 12b<br>    \"quoted:tag\": 3.5d<br>    ...<br>]</pre> |
 
 ## References
 * [PLY - Python Lex-Yacc](https://github.com/dabeaz/ply) by [David Beazley](https://www.dabeaz.com)
 * [nbtlib](https://github.com/vberlier/nbtlib) by [vberlier](https://github.com/vberlier)
+* [NBT format - Minecraft Wiki (fandom)](https://minecraft.fandom.com/wiki/NBT_format)
```

### Comparing `ftb-snbt-lib-0.2.2/README.md` & `ftb_snbt_lib-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ftb-snbt-lib
 
 ![GitHub Release](https://img.shields.io/github/v/release/peunsu/ftb-snbt-lib?style=for-the-badge)
 
-A python library to parse, edit, and save FTB snbt tag.
+**A python library to parse, edit, and save FTB snbt tag.**
 
 The FTB snbt tag is a variant of the "vanilla" snbt tag. It has no commas at end of lines, different suffixes for numeric values, and no support for array data type.
 
 This is the example of the FTB snbt tag:
 ```python
 {
     some_tag: "some_value"
@@ -26,81 +26,85 @@
 ```bash
 $ pip install ftb-snbt-lib
 ```
 
 ## Getting Started
 * Import the library.
 ```python
->>> import ftb_snbt_lib
+>>> import ftb_snbt_lib as slib
 ```
 
 * ``load(fp)``: Load the ftb snbt tag from a file (``fp``).
 ```python
->>> some_snbt = ftb_snbt_lib.load(open("tests/some_file.snbt", "r", encoding="utf-8"))
+>>> some_snbt = slib.load(open("tests/some_file.snbt", "r", encoding="utf-8"))
 ```
 * The type of returned value is ``Compound``, a dictionary-like object.<br>
 The ``Compound`` is containing values with **[tag data types](#data-types)** provided by this library.
 ```python
 >>> type(some_snbt)
-<class 'ftb_snbt.tag.Compound'>
+<class 'ftb_snbt_lib.tag.Compound'>
 >>> print(some_snbt)
 Compound({'some_tag': String('some_value'), 'another_tag': Byte(1)})
 ```
 
 * ``dump(tag, fp)``: Dump the ftb snbt tag to a file (``fp``).
 ```python
->>> ftb_snbt_lib.dump(some_snbt, open("tests/some_file_copy.snbt", "w", encoding="utf-8"))
+>>> slib.dump(some_snbt, open("tests/some_file_copy.snbt", "w", encoding="utf-8"))
 ```
 
 * ``loads(s)``: Load the ftb snbt tag from a string ``s``.
 ```python
->>> another_snbt = ftb_snbt_lib.loads('''
+>>> another_snbt = slib.loads('''
 ... {
 ...     some_tag: "some_value"
 ...     another_tag: 1b
 ... }
 ... ''')
 ```
 
 * ``dumps(tag)``: Dump the ftb snbt tag to a string.
 ```python
->>> dumped_snbt = ftb_snbt_lib.dumps(another_snbt)
+>>> dumped_snbt = slib.dumps(another_snbt)
 >>> print(dumped_snbt)
 {
     some_tag: "some_value"
     another_tag: 1b
 }
 ```
 
 * Edit the snbt tag. As its type is ``Compound``, it can be edited like a dictionary.<br>
 The inserted or replace values should be any of **[tag data types](#data-types)** provided by this library.
 ```python
->>> another_snbt["some_tag"] = ftb_snbt_lib.String("another_value")
+>>> another_snbt["some_tag"] = slib.String("another_value")
 ```
 
 * When editing the ``List``, a list-like object, its elements must have **the same type**.<br>
 For instance, ``List[Byte(1), Byte(2), Byte(3)]`` must contain **only** the ``Byte`` type object, so the other types like ``Integer`` or ``String`` **cannot be added or replaced** in it.
 
+* When editing the ``Array``, a list-like object with **a fixed length**, its elements must have **the same type**, and that type must **match the element type defined in the array**.<br>
+For instance, ``IntArray`` with a length of 3 must contain **three** ``Integer`` type objects, so **adding new objects, removing existing objects, and replacing with other type objects are not allowed**.
+
 * Save the edited snbt tag to a json file.
 ```python
 >>> import json
 >>> json.dump(another_snbt, open("tests/test.json", "w", encoding="utf-8"), indent=4, ensure_ascii=False)
 ```
 
 ## Data Types
 | Type | Description | Format | Example |
 | - | - | - | - |
 | Byte | A signed 8-bit integer.<br>Range: ``-128`` ~ ``127`` | ``<number>b`` | ``12b``, ``-35b`` |
 | Short | A signed 16-bit integer.<br>Range: ``-32,768`` ~ ``32,767`` | ``<number>s`` | ``132s``, ``-243s`` |
 | Integer | A signed 32-bit integer.<br>Range: ``-2,147,483,647`` ~ ``2,147,483,647`` | ``<number>`` | ``12345`` |
 | Long | A signed 64-bit integer.<br>Range: ``9,223,372,036,854,775,808`` ~ ``9,223,372,036,854,775,807`` | ``<number>L`` | ``12345L`` |
-| Float | A 32-bit, single-precision floating-point number.<br>Range: ``-3.4E+38`` ~ ``+3.4E+38`` | ``<number>f`` | ``12.345f`` |
-| Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308`` | ``<number>d`` | ``12.345d`` |
+| Float | A 32-bit, single-precision floating-point number.<br>Range: ``-3.4E+38`` ~ ``+3.4E+38`` | ``<number>f`` | ``12.345f``, ``1.0E-6f`` |
+| Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308`` | ``<number>d`` | ``12.345d``, ``1.0E-6d`` |
 | Bool | A boolean data type.<br>``0`` for ``false``, ``1`` for ``true``. | ``false``, ``true`` | ``true`` |
 | String | A sequence of characters. | A string enclosed in **double quotes ``""``**.<br>Nested double quotes can be included within a string using a **escaping character ``\"``**. | `"Hello, World!"`,<br>`"Say \"Hello, World!\""` |
 | List | An ordered list of tags.<br>The tags must be of **the same type**, determined by the first tag in the list. | Unnamed tags enclosed in square brackets and delimited by **newline** characters (``\n``). | <pre>[<br>    3.2d<br>    1.4d<br>    ...<br>]</pre> |
-| Array | An ordered list of 8-bit(ByteArray), 32-bit(IntArray), 64-bit(LongArray) integers. | ``<array_prefix>;`` followed by an ordered list of tags enclosed in square brackets and delimited by **newline** characters (``\n``).<br>Valid array prefixes are ``B``(Byte), ``I``(Integer), and ``L``(Long). | <pre>[B;<br>    12b<br>    -35b<br>    ...<br>]</pre> |
+| Array | An ordered list of 8-bit(``ByteArray``), 32-bit(``IntArray``), 64-bit(``LongArray``) integers. | ``<array_prefix>;`` followed by an ordered list of tags enclosed in square brackets and delimited by **newline** characters (``\n``).<br>Valid array prefixes are ``B``(Byte), ``I``(Integer), and ``L``(Long). | <pre>[B;<br>    12b<br>    -35b<br>    ...<br>]</pre> |
 | Compound | An ordered list of attribute-value pairs.<br>Each tag can be of **any type**. | Named tags enclosed in curly braces and delimited by commas or **newline** characters (``\n``).<br>The key (tag name) can be unquoted if it contains only ``0-9``, ``A-Z``, ``a-z``, ``_``, ``-``, ``.``, and ``+``. Otherwise the key should be quoted, using the format of ``String`` type. | <pre>[<br>    tag1: "string"<br>    tag2: 12b<br>    \"quoted:tag\": 3.5d<br>    ...<br>]</pre> |
 
 ## References
 * [PLY - Python Lex-Yacc](https://github.com/dabeaz/ply) by [David Beazley](https://www.dabeaz.com)
-* [nbtlib](https://github.com/vberlier/nbtlib) by [vberlier](https://github.com/vberlier)
+* [nbtlib](https://github.com/vberlier/nbtlib) by [vberlier](https://github.com/vberlier)
+* [NBT format - Minecraft Wiki (fandom)](https://minecraft.fandom.com/wiki/NBT_format)
```

### Comparing `ftb-snbt-lib-0.2.2/ftb_snbt_lib/parse.py` & `ftb_snbt_lib-0.2.3/ftb_snbt_lib/parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,46 +79,46 @@
 def get_parser():
     """Get the FTB snbt parser object.
     
     The parser object is ``yacc`` parser object that can be used to parse FTB snbt strings.
     
     Example
     -------
-        >>> import ftb_snbt
-        >>> parser = ftb_snbt.get_parser()
+        >>> import ftb_snbt_lib as slib
+        >>> parser = slib.get_parser()
         >>> snbt = parser.parse('''
             {
                 some_tag: "some_value"
                 another_tag: 1b
             }
             ''')
         >>> print(snbt)
         Compound({'some_tag': String('some_value'), 'another_tag': Byte(1)})
     """
     return yacc.yacc()
 
 def loads(s: str) -> Compound:
     """Load an FTB snbt string and return the result as a Compound object.
     
-    The loaded SNBT object consists of custom types: ``Compound``, ``List``, ``Numeric``, ``Bool``, and ``String``.
+    The loaded SNBT object consists of custom types: ``Compound``, ``List``, ``Array``, ``Numeric``, ``Bool``, and ``String``.
     
     When modifying the loaded object, use the provided custom types to ensure that the object is valid.
 
     Args
     ----
         s (str): The FTB snbt string to parse.
 
     Returns
     -------
         Compound: The loaded FTB snbt Compound object.
         
     Example
     -------
-        >>> import ftb_snbt
-        >>> snbt = ftb_snbt.loads('''
+        >>> import ftb_snbt_lib as slib
+        >>> snbt = slib.loads('''
             {
                 some_tag: "some_value"
                 another_tag: 1b
             }
             ''')
         >>> print(snbt)
         Compound({'some_tag': String('some_value'), 'another_tag': Byte(1)})
@@ -126,28 +126,28 @@
     parser = get_parser()
     return parser.parse(s)
 
 def load(fp) -> Compound:
     """    
     Load an FTB snbt file and return the result as a Compound object.
     
-    The loaded SNBT object consists of custom types: ``Compound``, ``List``, ``Numeric``, ``Bool``, and ``String``.
+    The loaded SNBT object consists of custom types: ``Compound``, ``List``, ``Array``, ``Numeric``, ``Bool``, and ``String``.
     
     When modifying the loaded object, use the provided custom types to ensure that the object is valid.
 
     Args
     ----
         fp (``io.TextIOWrapper``): The FTB snbt file to parse (opened in reading text mode with a ``UTF-8`` encoding.)
 
     Returns
     -------
         Compound: The loaded FTB snbt Compound object.
         
     Example
     -------
-        >>> import ftb_snbt
-        >>> snbt = ftb_snbt.load(open("path/to/file/some_file.snbt", "r", encoding="utf-8"))
+        >>> import ftb_snbt_lib as slib
+        >>> snbt = slib.load(open("path/to/file/some_file.snbt", "r", encoding="utf-8"))
         >>> type(snbt)
-        <class 'ftb_snbt.tag.Compound'>
+        <class 'ftb_snbt_lib.tag.Compound'>
     """
     parser = get_parser()
     return parser.parse(fp.read())
```

### Comparing `ftb-snbt-lib-0.2.2/ftb_snbt_lib/parsetab.py` & `ftb_snbt_lib-0.2.3/ftb_snbt_lib/parsetab.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/cpp.py` & `ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/ctokens.py` & `ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/lex.py` & `ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/lex.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/yacc.py` & `ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/ygen.py` & `ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.2/ftb_snbt_lib/tag.py` & `ftb_snbt_lib-0.2.3/ftb_snbt_lib/tag.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.2/ftb_snbt_lib/token.py` & `ftb_snbt_lib-0.2.3/ftb_snbt_lib/token.py`

 * *Files 24% similar despite different names*

```diff
@@ -58,20 +58,20 @@
 
 def t_SHORT(t):
     r'\-?[0-9]+s'
     t.value = Short(t.value[:-1])
     return t
 
 def t_FLOAT(t):
-    r'\-?[0-9]+\.[0-9]+f'
+    r'\-?[0-9]+(?:\.[0-9]+)?(?:[eE][\+\-]?[0-9]+)?f'
     t.value = Float(t.value[:-1])
     return t
 
 def t_DOUBLE(t):
-    r'\-?[0-9]+\.[0-9]+d'
+    r'\-?[0-9]+(?:\.[0-9]+)?(?:[eE][\+\-]?[0-9]+)?d'
     t.value = Double(t.value[:-1])
     return t
 
 def t_LONG(t):
     r'\-?[0-9]+L'
     t.value = Long(t.value[:-1])
     return t
```

### Comparing `ftb-snbt-lib-0.2.2/ftb_snbt_lib/write.py` & `ftb_snbt_lib-0.2.3/ftb_snbt_lib/write.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 }
 
 def get_writer():
     """Get the FTB snbt writer object.
     
     Example
     -------
-        >>> import ftb_snbt
-        >>> writer = ftb_snbt.get_writer()
+        >>> import ftb_snbt_lib as slib
+        >>> writer = slib.get_writer()
         >>> snbt = Compound({
         ...     'some_tag': String('some_value'),
         ...     'another_tag': Byte(1)
         ... })
         >>> dumped_snbt = writer.write(snbt)
         >>> print(dumped_snbt)
         {
@@ -41,20 +41,20 @@
 
     Returns
     -------
         str: The dumped FTB snbt string.
         
     Example
     -------
-        >>> import ftb_snbt
+        >>> import ftb_snbt_lib as slib
         >>> snbt = Compound({
         ...     'some_tag': String('some_value'),
         ...     'another_tag': Byte(1)
         ... })
-        >>> dumped_snbt = ftb_snbt.dumps(snbt)
+        >>> dumped_snbt = slib.dumps(snbt)
         >>> print(dumped_snbt)
         {
             some_tag: "some_value"
             another_tag: 1b
         }
     """
     return get_writer().write(tag) + "\n"
@@ -65,20 +65,20 @@
     Args
     ----
         tag (Base): The FTB snbt tag to dump.
         fp (io.TextIOWrapper): The file to write the FTB snbt tag to (opened in writing text mode with a UTF-8 encoding.)
     
     Example
     -------
-        >>> import ftb_snbt
+        >>> import ftb_snbt_lib as slib
         >>> snbt = Compound({
         ...     'some_tag': String('some_value'),
         ...     'another_tag': Byte(1)
         ... })
-        >>> ftb_snbt.dump(snbt, open('some_file.snbt', 'w', encoding='utf-8'))
+        >>> slib.dump(snbt, open('some_file.snbt', 'w', encoding='utf-8'))
     """
     fp.write(dumps(tag))
 
 class Writer:
     def __init__(self):
         self.indentation = "\t"
```

### Comparing `ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/PKG-INFO` & `ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftb-snbt-lib
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python library to parse, edit, and save FTB snbt tag, which is a variant of the "vanilla" snbt tag.
 Author-email: peunsu <peunsu55@gmail.com>
 Project-URL: homepage, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: repository, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: documentation, https://github.com/peunsu/ftb-snbt-lib
 Keywords: minecraft,ftb,snbt,parser,library
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 License-File: LICENSE
 Requires-Dist: wheel
 
 # ftb-snbt-lib
 
 ![GitHub Release](https://img.shields.io/github/v/release/peunsu/ftb-snbt-lib?style=for-the-badge)
 
-A python library to parse, edit, and save FTB snbt tag.
+**A python library to parse, edit, and save FTB snbt tag.**
 
 The FTB snbt tag is a variant of the "vanilla" snbt tag. It has no commas at end of lines, different suffixes for numeric values, and no support for array data type.
 
 This is the example of the FTB snbt tag:
 ```python
 {
     some_tag: "some_value"
@@ -43,81 +43,85 @@
 ```bash
 $ pip install ftb-snbt-lib
 ```
 
 ## Getting Started
 * Import the library.
 ```python
->>> import ftb_snbt_lib
+>>> import ftb_snbt_lib as slib
 ```
 
 * ``load(fp)``: Load the ftb snbt tag from a file (``fp``).
 ```python
->>> some_snbt = ftb_snbt_lib.load(open("tests/some_file.snbt", "r", encoding="utf-8"))
+>>> some_snbt = slib.load(open("tests/some_file.snbt", "r", encoding="utf-8"))
 ```
 * The type of returned value is ``Compound``, a dictionary-like object.<br>
 The ``Compound`` is containing values with **[tag data types](#data-types)** provided by this library.
 ```python
 >>> type(some_snbt)
-<class 'ftb_snbt.tag.Compound'>
+<class 'ftb_snbt_lib.tag.Compound'>
 >>> print(some_snbt)
 Compound({'some_tag': String('some_value'), 'another_tag': Byte(1)})
 ```
 
 * ``dump(tag, fp)``: Dump the ftb snbt tag to a file (``fp``).
 ```python
->>> ftb_snbt_lib.dump(some_snbt, open("tests/some_file_copy.snbt", "w", encoding="utf-8"))
+>>> slib.dump(some_snbt, open("tests/some_file_copy.snbt", "w", encoding="utf-8"))
 ```
 
 * ``loads(s)``: Load the ftb snbt tag from a string ``s``.
 ```python
->>> another_snbt = ftb_snbt_lib.loads('''
+>>> another_snbt = slib.loads('''
 ... {
 ...     some_tag: "some_value"
 ...     another_tag: 1b
 ... }
 ... ''')
 ```
 
 * ``dumps(tag)``: Dump the ftb snbt tag to a string.
 ```python
->>> dumped_snbt = ftb_snbt_lib.dumps(another_snbt)
+>>> dumped_snbt = slib.dumps(another_snbt)
 >>> print(dumped_snbt)
 {
     some_tag: "some_value"
     another_tag: 1b
 }
 ```
 
 * Edit the snbt tag. As its type is ``Compound``, it can be edited like a dictionary.<br>
 The inserted or replace values should be any of **[tag data types](#data-types)** provided by this library.
 ```python
->>> another_snbt["some_tag"] = ftb_snbt_lib.String("another_value")
+>>> another_snbt["some_tag"] = slib.String("another_value")
 ```
 
 * When editing the ``List``, a list-like object, its elements must have **the same type**.<br>
 For instance, ``List[Byte(1), Byte(2), Byte(3)]`` must contain **only** the ``Byte`` type object, so the other types like ``Integer`` or ``String`` **cannot be added or replaced** in it.
 
+* When editing the ``Array``, a list-like object with **a fixed length**, its elements must have **the same type**, and that type must **match the element type defined in the array**.<br>
+For instance, ``IntArray`` with a length of 3 must contain **three** ``Integer`` type objects, so **adding new objects, removing existing objects, and replacing with other type objects are not allowed**.
+
 * Save the edited snbt tag to a json file.
 ```python
 >>> import json
 >>> json.dump(another_snbt, open("tests/test.json", "w", encoding="utf-8"), indent=4, ensure_ascii=False)
 ```
 
 ## Data Types
 | Type | Description | Format | Example |
 | - | - | - | - |
 | Byte | A signed 8-bit integer.<br>Range: ``-128`` ~ ``127`` | ``<number>b`` | ``12b``, ``-35b`` |
 | Short | A signed 16-bit integer.<br>Range: ``-32,768`` ~ ``32,767`` | ``<number>s`` | ``132s``, ``-243s`` |
 | Integer | A signed 32-bit integer.<br>Range: ``-2,147,483,647`` ~ ``2,147,483,647`` | ``<number>`` | ``12345`` |
 | Long | A signed 64-bit integer.<br>Range: ``9,223,372,036,854,775,808`` ~ ``9,223,372,036,854,775,807`` | ``<number>L`` | ``12345L`` |
-| Float | A 32-bit, single-precision floating-point number.<br>Range: ``-3.4E+38`` ~ ``+3.4E+38`` | ``<number>f`` | ``12.345f`` |
-| Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308`` | ``<number>d`` | ``12.345d`` |
+| Float | A 32-bit, single-precision floating-point number.<br>Range: ``-3.4E+38`` ~ ``+3.4E+38`` | ``<number>f`` | ``12.345f``, ``1.0E-6f`` |
+| Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308`` | ``<number>d`` | ``12.345d``, ``1.0E-6d`` |
 | Bool | A boolean data type.<br>``0`` for ``false``, ``1`` for ``true``. | ``false``, ``true`` | ``true`` |
 | String | A sequence of characters. | A string enclosed in **double quotes ``""``**.<br>Nested double quotes can be included within a string using a **escaping character ``\"``**. | `"Hello, World!"`,<br>`"Say \"Hello, World!\""` |
 | List | An ordered list of tags.<br>The tags must be of **the same type**, determined by the first tag in the list. | Unnamed tags enclosed in square brackets and delimited by **newline** characters (``\n``). | <pre>[<br>    3.2d<br>    1.4d<br>    ...<br>]</pre> |
-| Array | An ordered list of 8-bit(ByteArray), 32-bit(IntArray), 64-bit(LongArray) integers. | ``<array_prefix>;`` followed by an ordered list of tags enclosed in square brackets and delimited by **newline** characters (``\n``).<br>Valid array prefixes are ``B``(Byte), ``I``(Integer), and ``L``(Long). | <pre>[B;<br>    12b<br>    -35b<br>    ...<br>]</pre> |
+| Array | An ordered list of 8-bit(``ByteArray``), 32-bit(``IntArray``), 64-bit(``LongArray``) integers. | ``<array_prefix>;`` followed by an ordered list of tags enclosed in square brackets and delimited by **newline** characters (``\n``).<br>Valid array prefixes are ``B``(Byte), ``I``(Integer), and ``L``(Long). | <pre>[B;<br>    12b<br>    -35b<br>    ...<br>]</pre> |
 | Compound | An ordered list of attribute-value pairs.<br>Each tag can be of **any type**. | Named tags enclosed in curly braces and delimited by commas or **newline** characters (``\n``).<br>The key (tag name) can be unquoted if it contains only ``0-9``, ``A-Z``, ``a-z``, ``_``, ``-``, ``.``, and ``+``. Otherwise the key should be quoted, using the format of ``String`` type. | <pre>[<br>    tag1: "string"<br>    tag2: 12b<br>    \"quoted:tag\": 3.5d<br>    ...<br>]</pre> |
 
 ## References
 * [PLY - Python Lex-Yacc](https://github.com/dabeaz/ply) by [David Beazley](https://www.dabeaz.com)
 * [nbtlib](https://github.com/vberlier/nbtlib) by [vberlier](https://github.com/vberlier)
+* [NBT format - Minecraft Wiki (fandom)](https://minecraft.fandom.com/wiki/NBT_format)
```

### Comparing `ftb-snbt-lib-0.2.2/pyproject.toml` & `ftb_snbt_lib-0.2.3/pyproject.toml`

 * *Files identical despite different names*

