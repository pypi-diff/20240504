# Comparing `tmp/safe_ds_stubgen-0.2.0.tar.gz` & `tmp/safe_ds_stubgen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_ds_stubgen-0.2.0.tar", max compression
+gzip compressed data, was "safe_ds_stubgen-0.3.0.tar", max compression
```

## Comparing `safe_ds_stubgen-0.2.0.tar` & `safe_ds_stubgen-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1069 2024-03-29 13:15:02.929458 safe_ds_stubgen-0.2.0/LICENSE
--rw-r--r--   0        0        0     2407 2024-03-29 13:15:02.929458 safe_ds_stubgen-0.2.0/docs/README.md
--rw-r--r--   0        0        0      997 2024-03-29 13:15:47.077465 safe_ds_stubgen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       66 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/__init__.py
--rw-r--r--   0        0        0     1361 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/__init__.py
--rw-r--r--   0        0        0    12355 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_api.py
--rw-r--r--   0        0        0    50157 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_ast_visitor.py
--rw-r--r--   0        0        0     4423 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_ast_walker.py
--rw-r--r--   0        0        0     6324 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_get_api.py
--rw-r--r--   0        0        0     4781 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_mypy_helpers.py
--rw-r--r--   0        0        0      739 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_package_metadata.py
--rw-r--r--   0        0        0    19823 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_types.py
--rw-r--r--   0        0        0      138 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/cli/__init__.py
--rw-r--r--   0        0        0     2993 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/cli/_cli.py
--rw-r--r--   0        0        0      915 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/__init__.py
--rw-r--r--   0        0        0     1339 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_abstract_docstring_parser.py
--rw-r--r--   0        0        0      865 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_create_docstring_parser.py
--rw-r--r--   0        0        0     1131 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_docstring.py
--rw-r--r--   0        0        0      514 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_docstring_style.py
--rw-r--r--   0        0        0     4928 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_epydoc_parser.py
--rw-r--r--   0        0        0     5697 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_googledoc_parser.py
--rw-r--r--   0        0        0     1544 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_helpers.py
--rw-r--r--   0        0        0     9115 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_numpydoc_parser.py
--rw-r--r--   0        0        0     1807 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_plaintext_docstring_parser.py
--rw-r--r--   0        0        0     5700 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_restdoc_parser.py
--rw-r--r--   0        0        0      449 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/main.py
--rw-r--r--   0        0        0      170 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/stubs_generator/__init__.py
--rw-r--r--   0        0        0    43649 2024-03-29 13:15:02.933458 safe_ds_stubgen-0.2.0/src/safeds_stubgen/stubs_generator/_generate_stubs.py
--rw-r--r--   0        0        0     3173 1970-01-01 00:00:00.000000 safe_ds_stubgen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-04 15:36:11.860738 safe_ds_stubgen-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2301 2024-05-04 15:36:11.860738 safe_ds_stubgen-0.3.0/docs/README.md
+-rw-r--r--   0        0        0      994 2024-05-04 15:36:30.828800 safe_ds_stubgen-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      136 2024-05-04 15:36:11.864739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-04 15:36:11.864739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/_helpers.py
+-rw-r--r--   0        0        0     1488 2024-05-04 15:36:11.864739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/__init__.py
+-rw-r--r--   0        0        0    12312 2024-05-04 15:36:11.864739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_api.py
+-rw-r--r--   0        0        0    54930 2024-05-04 15:36:11.864739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_ast_visitor.py
+-rw-r--r--   0        0        0     4460 2024-05-04 15:36:11.864739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_ast_walker.py
+-rw-r--r--   0        0        0     7182 2024-05-04 15:36:11.864739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_get_api.py
+-rw-r--r--   0        0        0     4731 2024-05-04 15:36:11.864739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_mypy_helpers.py
+-rw-r--r--   0        0        0      430 2024-05-04 15:36:11.864739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_package_metadata.py
+-rw-r--r--   0        0        0    22827 2024-05-04 15:36:11.864739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_types.py
+-rw-r--r--   0        0        0      138 2024-05-04 15:36:11.864739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/cli/__init__.py
+-rw-r--r--   0        0        0     3063 2024-05-04 15:36:11.864739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/cli/_cli.py
+-rw-r--r--   0        0        0      748 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/__init__.py
+-rw-r--r--   0        0        0     1204 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/_abstract_docstring_parser.py
+-rw-r--r--   0        0        0      898 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/_create_docstring_parser.py
+-rw-r--r--   0        0        0     1196 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/_docstring.py
+-rw-r--r--   0        0        0    19058 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/_docstring_parser.py
+-rw-r--r--   0        0        0      492 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/_docstring_style.py
+-rw-r--r--   0        0        0      974 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/_helpers.py
+-rw-r--r--   0        0        0     1666 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/_plaintext_docstring_parser.py
+-rw-r--r--   0        0        0      449 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/main.py
+-rw-r--r--   0        0        0      369 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/stubs_generator/__init__.py
+-rw-r--r--   0        0        0     6366 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/stubs_generator/_generate_stubs.py
+-rw-r--r--   0        0        0     3884 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/stubs_generator/_helper.py
+-rw-r--r--   0        0        0    44852 2024-05-04 15:36:11.868739 safe_ds_stubgen-0.3.0/src/safeds_stubgen/stubs_generator/_stub_string_generator.py
+-rw-r--r--   0        0        0     3057 1970-01-01 00:00:00.000000 safe_ds_stubgen-0.3.0/PKG-INFO
```

### Comparing `safe_ds_stubgen-0.2.0/LICENSE` & `safe_ds_stubgen-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_ds_stubgen-0.2.0/docs/README.md` & `safe_ds_stubgen-0.3.0/docs/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Stub Generator
 
 [![PyPI](https://img.shields.io/pypi/v/safe-ds-stubgen)](https://pypi.org/project/safe-ds-stubgen)
 [![Main](https://github.com/Safe-DS/Stub-Generator/actions/workflows/main.yml/badge.svg)](https://github.com/Safe-DS/Stub-Generator/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/Safe-DS/Stub-Generator/branch/main/graph/badge.svg?token=UyCUY59HKM)](https://codecov.io/gh/Safe-DS/Stub-Generator)
 [![Documentation Status](https://readthedocs.org/projects/safe-ds-stub-generator/badge/?version=stable)](https://stubgen.safeds.com)
 
-Automated generation of [Safe-DS stubs](https://dsl.safeds.com/en/stable/language/stub-language/) for Python libraries.
+Automated generation of [Safe-DS stubs](https://dsl.safeds.com/en/stable/stub-language/) for Python libraries.
 
 ## Installation
 
 Get the latest version from [PyPI](https://pypi.org/project/safe-ds-stubgen):
 
 ```shell
 pip install safe-ds-stubgen
@@ -25,15 +25,15 @@
 Analyze Python code.
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         show info messages
   -p PACKAGE, --package PACKAGE
                         The name of the package.
-  -s SRC, --src SRC     Directory containing the Python code of the package. If this is omitted, we try to locate the package with the given name in the current Python interpreter.
+  -s SRC, --src SRC     Source directory containing the Python code of the package.
   -o OUT, --out OUT     Output directory.
   --docstyle {PLAINTEXT,EPYDOC,GOOGLE,NUMPYDOC,REST}
                         The docstring style.
   -tr, --testrun        Set this flag if files in /test or /tests directories should be included.
   -nc, --naming_convert
                         Set this flag if the name identifiers should be converted to Safe-DS standard (UpperCamelCase for classes and camelCase for everything else).
 ```
```

### Comparing `safe_ds_stubgen-0.2.0/pyproject.toml` & `safe_ds_stubgen-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "safe-ds-stubgen"
-version = "0.2.0"
+version = "0.3.0"
 description = "Generation of Safe-DS stubs for Python libraries."
 authors = ["Lars Reimann <mail@larsreimann.com>"]
 license = "MIT"
 readme = "docs/README.md"
 repository = "https://github.com/Safe-DS/Stub-Generator"
 documentation = "https://stubgen.readthedocs.io"
 keywords = ["data-science", "machine-learning", "dsl"]
@@ -14,19 +14,19 @@
 
 [tool.poetry.scripts]
 safe-ds-stubgen = "safeds_stubgen.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 mypy = "^1.6.1"
-docstring-parser = "^0.15"
+griffe = ">=0.42,<0.45"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.3,<9.0.0"
-pytest-cov = "^4.0.0"
+pytest-cov = ">=4,<6"
 syrupy = "^4.6.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-glightbox = "^0.3.1"
 mkdocs-material = "^9.4.7"
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/__init__.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,31 +12,34 @@
     Parameter,
     ParameterAssignment,
     QualifiedImport,
     Result,
     VarianceKind,
     WildcardImport,
 )
+from ._ast_visitor import result_name_generator
 from ._get_api import get_api
 from ._mypy_helpers import get_classdef_definitions, get_funcdef_definitions, get_mypyfile_definitions
-from ._package_metadata import distribution, distribution_version, package_root
+from ._package_metadata import distribution, distribution_version
 from ._types import (
     AbstractType,
     BoundaryType,
     CallableType,
     DictType,
     EnumType,
     FinalType,
     ListType,
     LiteralType,
+    NamedSequenceType,
     NamedType,
     SetType,
     TupleType,
     TypeVarType,
     UnionType,
+    UnknownType,
 )
 
 __all__ = [
     "AbstractType",
     "API",
     "Attribute",
     "BoundaryType",
@@ -52,20 +55,22 @@
     "get_api",
     "get_classdef_definitions",
     "get_funcdef_definitions",
     "get_mypyfile_definitions",
     "ListType",
     "LiteralType",
     "Module",
+    "NamedSequenceType",
     "NamedType",
-    "package_root",
     "Parameter",
     "ParameterAssignment",
     "QualifiedImport",
     "Result",
+    "result_name_generator",
     "SetType",
     "TupleType",
     "TypeVarType",
     "UnionType",
+    "UnknownType",
     "VarianceKind",
     "WildcardImport",
 ]
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_api.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def ensure_file_exists(file: Path) -> None:
     """
     Create a file and all parent directories if they don't exist already.
 
     Parameters
     ----------
-    file: Path
+    file:
         The file path.
     """
     file.parent.mkdir(parents=True, exist_ok=True)
     file.touch(exist_ok=True)
 
 
 class API:
@@ -44,15 +44,14 @@
         self.classes: dict[str, Class] = {}
         self.functions: dict[str, Function] = {}
         self.results: dict[str, Result] = {}
         self.enums: dict[str, Enum] = {}
         self.enum_instances: dict[str, EnumInstance] = {}
         self.attributes_: dict[str, Attribute] = {}
         self.parameters_: dict[str, Parameter] = {}
-
         self.reexport_map: dict[str, set[Module]] = defaultdict(set)
 
     def add_module(self, module: Module) -> None:
         self.modules[module.id] = module
 
     def add_class(self, class_: Class) -> None:
         self.classes[class_.id] = class_
@@ -238,14 +237,15 @@
     id: str
     name: str
     docstring: FunctionDocstring
     is_public: bool
     is_static: bool
     is_class_method: bool
     is_property: bool
+    result_docstrings: list[ResultDocstring]
     type_var_types: list[TypeVarType] = field(default_factory=list)
     results: list[Result] = field(default_factory=list)
     reexported_by: list[Module] = field(default_factory=list)
     parameters: list[Parameter] = field(default_factory=list)
 
     def to_dict(self) -> dict[str, Any]:
         return {
@@ -335,21 +335,19 @@
 
 
 @dataclass(frozen=True)
 class Result:
     id: str
     name: str
     type: AbstractType | None
-    docstring: ResultDocstring
 
     def to_dict(self) -> dict[str, Any]:
         return {
             "id": self.id,
             "name": self.name,
-            "docstring": self.docstring.to_dict(),
             "type": self.type.to_dict() if self.type is not None else None,
         }
 
 
 @dataclass
 class Enum:
     id: str
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_ast_visitor.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_ast_visitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
+import logging
 from copy import deepcopy
 from types import NoneType
 from typing import TYPE_CHECKING
 
 import mypy.nodes as mp_nodes
 import mypy.types as mp_types
 
 import safeds_stubgen.api_analyzer._types as sds_types
+from safeds_stubgen import is_internal
+from safeds_stubgen.docstring_parsing import ResultDocstring
 
 from ._api import (
     API,
     Attribute,
     Class,
     Enum,
     EnumInstance,
@@ -33,16 +36,18 @@
     has_correct_type_of_any,
     mypy_expression_to_python_value,
     mypy_expression_to_sds_type,
     mypy_variance_parser,
 )
 
 if TYPE_CHECKING:
+    from collections.abc import Generator
+
     from safeds_stubgen.api_analyzer._types import AbstractType
-    from safeds_stubgen.docstring_parsing import AbstractDocstringParser, ResultDocstring
+    from safeds_stubgen.docstring_parsing import AbstractDocstringParser
 
 
 class MyPyAstVisitor:
     def __init__(self, docstring_parser: AbstractDocstringParser, api: API, aliases: dict[str, set[str]]) -> None:
         self.docstring_parser: AbstractDocstringParser = docstring_parser
         self.api: API = api
         self.__declaration_stack: list[Module | Class | Function | Enum | list[Attribute | EnumInstance]] = []
@@ -59,15 +64,15 @@
         wildcard_imports: list[WildcardImport] = []
         docstring = ""
 
         # We don't need to check functions, classes and assignments, since the ast walker will already check them
         child_definitions = [
             _definition
             for _definition in get_mypyfile_definitions(node)
-            if _definition.__class__.__name__ not in ["FuncDef", "Decorator", "ClassDef", "AssignmentStmt"]
+            if _definition.__class__.__name__ not in {"FuncDef", "Decorator", "ClassDef", "AssignmentStmt"}
         ]
 
         # Imports
         for import_ in node.imports:
             if isinstance(import_, mp_nodes.Import):
                 for import_name, import_alias in import_.ids:
                     qualified_imports.append(
@@ -120,16 +125,15 @@
         module = self.__declaration_stack.pop()
         if not isinstance(module, Module):  # pragma: no cover
             raise AssertionError("Imbalanced push/pop on stack")  # noqa: TRY004
 
         self.api.add_module(module)
 
     def enter_classdef(self, node: mp_nodes.ClassDef) -> None:
-        name = node.name
-        id_ = self._create_id_from_stack(name)
+        id_ = self._create_id_from_stack(node.name)
 
         # Get docstring
         docstring = self.docstring_parser.get_class_documentation(node)
 
         # Variance
         # Special base classes like Generic[...] get moved to "removed_base_type_expr" during semantic analysis of mypy
         generic_exprs = []
@@ -193,30 +197,32 @@
                 if superclass_name in self.aliases:
                     _, superclass_alias_qname = self._find_alias(superclass_name)
                     superclass_qname = superclass_alias_qname if superclass_alias_qname else superclass_qname
 
                 superclasses.append(superclass_qname)
 
         # Get reexported data
-        reexported_by = self._get_reexported_by(name)
+        reexported_by = self._get_reexported_by(node.fullname)
+        # Sort for snapshot tests
+        reexported_by.sort(key=lambda x: x.id)
 
         # Get constructor docstring
         definitions = get_classdef_definitions(node)
         constructor_fulldocstring = ""
         for definition in definitions:
             if isinstance(definition, mp_nodes.FuncDef) and definition.name == "__init__":
                 constructor_docstring = self.docstring_parser.get_function_documentation(definition)
                 constructor_fulldocstring = constructor_docstring.full_docstring
 
         # Remember class, so we can later add methods
         class_ = Class(
             id=id_,
-            name=name,
+            name=node.name,
             superclasses=superclasses,
-            is_public=self._is_public(node.name, name),
+            is_public=self._is_public(node.name, node.fullname),
             docstring=docstring,
             reexported_by=reexported_by,
             constructor_fulldocstring=constructor_fulldocstring,
             inherits_from_exception=inherits_from_exception,
             type_parameters=type_parameters,
         )
         self.__declaration_stack.append(class_)
@@ -252,33 +258,37 @@
             arguments = self._parse_parameter_data(node, function_id)
 
             if self.type_var_types:
                 type_var_types = list(self.type_var_types)
                 # Sort for the snapshot tests
                 type_var_types.sort(key=lambda x: x.name)
 
-        # Create results
-        results = self._parse_results(node, function_id)
+        # Create results and result docstrings
+        result_docstrings = self.docstring_parser.get_result_documentation(node.fullname)
+        results = self._parse_results(node, function_id, result_docstrings)
 
         # Get reexported data
-        reexported_by = self._get_reexported_by(name)
+        reexported_by = self._get_reexported_by(node.fullname)
+        # Sort for snapshot tests
+        reexported_by.sort(key=lambda x: x.id)
 
         # Create and add Function to stack
         function = Function(
             id=function_id,
             name=name,
             docstring=docstring,
             is_public=is_public,
             is_static=is_static,
             is_class_method=node.is_class,
             is_property=node.is_property,
             results=results,
             reexported_by=reexported_by,
             parameters=arguments,
             type_var_types=type_var_types,
+            result_docstrings=result_docstrings,
         )
         self.__declaration_stack.append(function)
 
     def leave_funcdef(self, _: mp_nodes.FuncDef) -> None:
         function = self.__declaration_stack.pop()
         if not isinstance(function, Function):  # pragma: no cover
             raise AssertionError("Imbalanced push/pop on stack")  # noqa: TRY004
@@ -396,66 +406,102 @@
                 else:  # pragma: no cover
                     raise TypeError("Unexpected value type for assignments")
 
     # ############################## Utilities ############################## #
 
     # #### Result utilities
 
-    def _parse_results(self, node: mp_nodes.FuncDef, function_id: str) -> list[Result]:
+    def _parse_results(
+        self,
+        node: mp_nodes.FuncDef,
+        function_id: str,
+        result_docstrings: list[ResultDocstring],
+    ) -> list[Result]:
         # __init__ functions aren't supposed to have returns, so we can ignore them
         if node.name == "__init__":
             return []
 
         # Get type
         ret_type: sds_types.AbstractType | None = None
         type_is_inferred = False
         if hasattr(node, "type"):
             node_type = node.type
             if node_type is not None and hasattr(node_type, "ret_type"):
                 node_ret_type = node_type.ret_type
 
-                if not isinstance(node_ret_type, mp_types.NoneType):
-                    if isinstance(node_ret_type, mp_types.AnyType) and not has_correct_type_of_any(
-                        node_ret_type.type_of_any,
+                if isinstance(node_ret_type, mp_types.NoneType):
+                    ret_type = sds_types.NamedType(name="None", qname="builtins.None")
+                else:
+                    unanalyzed_ret_type = getattr(node.unanalyzed_type, "ret_type", None)
+
+                    if (
+                        (
+                            not unanalyzed_ret_type
+                            or getattr(unanalyzed_ret_type, "literal_value", "") is None
+                            or isinstance(unanalyzed_ret_type, mp_types.AnyType)
+                        )
+                        and isinstance(node_ret_type, mp_types.AnyType)
+                        and not has_correct_type_of_any(node_ret_type.type_of_any)
                     ):
                         # In this case, the "Any" type was given because it was not explicitly annotated.
                         # Therefor we have to try to infer the type.
                         ret_type = self._infer_type_from_return_stmts(node)
                         type_is_inferred = ret_type is not None
                     else:
                         # Otherwise, we can parse the type normally
-                        unanalyzed_ret_type = getattr(node.unanalyzed_type, "ret_type", None)
                         ret_type = self.mypy_type_to_abstract_type(node_ret_type, unanalyzed_ret_type)
             else:
                 # Infer type
                 ret_type = self._infer_type_from_return_stmts(node)
                 type_is_inferred = ret_type is not None
 
         if ret_type is None:
             return []
 
-        result_docstring = self.docstring_parser.get_result_documentation(node)
-
         if type_is_inferred and isinstance(ret_type, sds_types.TupleType):
-            return self._create_inferred_results(ret_type, result_docstring, function_id)
+            return self._create_inferred_results(ret_type, result_docstrings, function_id)
 
         # If we got a TupleType, we can iterate it for the results, but if we got a NamedType, we have just one result
         return_results = ret_type.types if isinstance(ret_type, sds_types.TupleType) else [ret_type]
-        return [
-            Result(
-                id=f"{function_id}/result_{i + 1}",
-                type=type_,
-                name=f"result_{i + 1}",
-                docstring=result_docstring,
-            )
-            for i, type_ in enumerate(return_results)
-        ]
+
+        # Create Result objects and try to find a matching docstring name
+        all_results = []
+        name_generator = result_name_generator()
+
+        if len(return_results) == 1 == len(result_docstrings):
+            result_name = result_docstrings[0].name or next(name_generator)
+            all_results = [
+                Result(
+                    id=f"{function_id}/{result_name}",
+                    type=return_results[0],
+                    name=f"{result_name}",
+                ),
+            ]
+        else:
+            for type_ in return_results:
+                result_docstring = ResultDocstring()
+                for docstring in result_docstrings:
+                    if hash(docstring.type) == hash(type_):
+                        result_docstring = docstring
+                        break
+
+                result_name = result_docstring.name or next(name_generator)
+
+                all_results.append(
+                    Result(
+                        id=f"{function_id}/{result_name}",
+                        type=type_,
+                        name=f"{result_name}",
+                    ),
+                )
+
+        return all_results
 
     @staticmethod
-    def _infer_type_from_return_stmts(func_node: mp_nodes.FuncDef) -> sds_types.NamedType | sds_types.TupleType | None:
+    def _infer_type_from_return_stmts(func_node: mp_nodes.FuncDef) -> sds_types.TupleType | None:
         # To infer the type, we iterate through all return statements we find in the function
         func_defn = get_funcdef_definitions(func_node)
         return_stmts = find_return_stmts_recursive(func_defn)
         if return_stmts:
             types = set()
             for return_stmt in return_stmts:
                 if return_stmt.expr is None:  # pragma: no cover
@@ -468,91 +514,132 @@
                             if conditional_branch is None:  # pragma: no cover
                                 continue
 
                             if not isinstance(conditional_branch, mp_nodes.CallExpr | mp_nodes.MemberExpr):
                                 type_ = mypy_expression_to_sds_type(conditional_branch)
                                 if isinstance(type_, sds_types.NamedType | sds_types.TupleType):
                                     types.add(type_)
+                    elif hasattr(return_stmt.expr, "node") and getattr(return_stmt.expr.node, "is_self", False):
+                        # The result type is an instance of the parent class
+                        expr_type = return_stmt.expr.node.type.type
+                        types.add(sds_types.NamedType(name=expr_type.name, qname=expr_type.fullname))
                     else:
                         type_ = mypy_expression_to_sds_type(return_stmt.expr)
                         if isinstance(type_, sds_types.NamedType | sds_types.TupleType):
                             types.add(type_)
 
             # We have to sort the list for the snapshot tests
             return_stmt_types = list(types)
             return_stmt_types.sort(
                 key=lambda x: (x.name if isinstance(x, sds_types.NamedType) else str(len(x.types))),
             )
 
-            if len(return_stmt_types) == 1:
-                return return_stmt_types[0]
-            elif len(return_stmt_types) >= 2:
-                return sds_types.TupleType(types=return_stmt_types)
+            return sds_types.TupleType(types=return_stmt_types)
         return None
 
     @staticmethod
     def _create_inferred_results(
         results: sds_types.TupleType,
-        result_docstring: ResultDocstring,
+        docstrings: list[ResultDocstring],
         function_id: str,
     ) -> list[Result]:
         """Create Result objects with inferred results.
 
         If we inferred the result types, we have to create a two-dimensional array for the results since tuples are
         considered as multiple results, but other return types have to be grouped as one union. For example, if a
         function has the following returns "return 42" and "return True, 1.2" we would have to group the integer and
         boolean as "result_1: Union[int, bool]" and the float number as "result_2: Union[float, None]".
 
         Paramters
         ---------
-        ret_type : sds_types.TupleType
+        ret_type:
             An object representing a tuple with all inferred types.
-        result_docstring : ResultDocstring
+        result_docstring:
             The docstring of the function to which the results belong to.
-        function_id : str
+        function_id:
             The function ID.
 
         Returns
         -------
-        list[Result]
+        results:
             A list of Results objects representing the possible results of a funtion.
         """
-        result_array: list[list] = []
+        result_array: list[list[AbstractType]] = []
+        longest_inner_list = 1
         for type_ in results.types:
             if isinstance(type_, sds_types.NamedType):
                 if result_array:
                     result_array[0].append(type_)
                 else:
                     result_array.append([type_])
             elif isinstance(type_, sds_types.TupleType):
                 for i, type__ in enumerate(type_.types):
                     if len(result_array) > i:
-                        result_array[i].append(type__)
+                        if type__ not in result_array[i]:
+                            result_array[i].append(type__)
+
+                            if len(result_array[i]) > longest_inner_list:
+                                longest_inner_list = len(result_array[i])
                     else:
                         result_array.append([type__])
             else:  # pragma: no cover
                 raise TypeError(f"Expected NamedType or TupleType, received {type(type_)}")
 
-        inferred_results = []
-        for i, result_list in enumerate(result_array):
-            result_count = len(result_list)
-            if result_count == 1:
-                result_type = result_list[0]
-            else:
-                result_type = sds_types.UnionType(result_list)
+        # If there are any arrays longer than others, these "others" are optional types and can be None
+        none_element = sds_types.NamedType(name="None", qname="builtins.None")
+        for array in result_array:
+            if len(array) < longest_inner_list and none_element not in array:
+                array.append(none_element)
 
-            name = f"result_{i + 1}"
-            inferred_results.append(
+        # Create Result objects
+        name_generator = result_name_generator()
+        inferred_results = []
+        if 1 == len(result_array) == len(result_array[0]) == len(docstrings):
+            result_name = docstrings[0].name or next(name_generator)
+            inferred_results = [
                 Result(
-                    id=f"{function_id}/{name}",
-                    type=result_type,
-                    name=name,
-                    docstring=result_docstring,
+                    id=f"{function_id}/{result_name}",
+                    type=result_array[0][0],
+                    name=result_name,
                 ),
-            )
+            ]
+        else:
+            for result_list in result_array:
+                result_count = len(result_list)
+                if result_count == 1:
+                    result_type = result_list[0]
+                else:
+                    result_type = sds_types.UnionType(result_list)
+
+                # Search for matching docstrings for each result for the name
+                result_docstring = ResultDocstring()
+                if docstrings:
+                    if isinstance(result_type, sds_types.UnionType):
+                        possible_type: sds_types.AbstractType | None
+                        if len(docstrings) > 1:
+                            docstring_types = [docstring.type for docstring in docstrings if docstring.type is not None]
+                            possible_type = sds_types.UnionType(types=docstring_types)
+                        else:
+                            possible_type = docstrings[0].type
+                        if possible_type == result_type:
+                            result_docstring = docstrings[0]
+                    else:
+                        for docstring in docstrings:
+                            if hash(docstring.type) == hash(result_type):
+                                result_docstring = docstring
+                                break
+
+                result_name = result_docstring.name or next(name_generator)
+                inferred_results.append(
+                    Result(
+                        id=f"{function_id}/{result_name}",
+                        type=result_type,
+                        name=result_name,
+                    ),
+                )
 
         return inferred_results
 
     # #### Attribute utilities
 
     def _parse_attributes(
         self,
@@ -666,15 +753,15 @@
             type_ = self.mypy_type_to_abstract_type(attribute_type, unanalyzed_type)
 
         # Get docstring
         parent = self.__declaration_stack[-1]
         if isinstance(parent, Function) and parent.name == "__init__":
             parent = self.__declaration_stack[-2]
         assert isinstance(parent, Class)
-        docstring = self.docstring_parser.get_attribute_documentation(parent, name)
+        docstring = self.docstring_parser.get_attribute_documentation(parent.id, name)
 
         # Remove __init__ for attribute ids
         id_ = self._create_id_from_stack(name).replace("__init__/", "")
 
         return Attribute(
             id=id_,
             name=name,
@@ -723,18 +810,17 @@
 
             arg_name = argument.variable.name
             arg_kind = get_argument_kind(argument)
 
             # Create parameter docstring
             parent = self.__declaration_stack[-1]
             docstring = self.docstring_parser.get_parameter_documentation(
-                function_node=node,
+                function_qname=node.fullname,
                 parameter_name=arg_name,
-                parameter_assigned_by=arg_kind,
-                parent_class=parent if isinstance(parent, Class) else None,
+                parent_class_qname=parent.id if isinstance(parent, Class) else "",
             )
 
             if isinstance(default_value, type):  # pragma: no cover
                 raise TypeError("default_value has the unexpected type 'type'.")
 
             # Create parameter object
             arguments.append(
@@ -779,45 +865,45 @@
                     raise TypeError("Default value got an unsupported value.")
 
                 default_is_none = default_value is None
         return default_value, default_is_none
 
     # #### Reexport utilities
 
-    def _get_reexported_by(self, name: str) -> list[Module]:
-        # Get the uppermost module and the path to the current node
-        parents = []
-        parent = None
-        i = 1
-        while not isinstance(parent, Module):
-            parent = self.__declaration_stack[-i]
-            if isinstance(parent, list):  # pragma: no cover
-                continue
-            parents.append(parent.name)
-            i += 1
-        path = [*list(reversed(parents)), name]
+    def _get_reexported_by(self, qname: str) -> list[Module]:
+        path = qname.split(".")
 
         # Check if there is a reexport entry for each item in the path to the current module
         reexported_by = set()
         for i in range(len(path)):
-            reexport_name = ".".join(path[: i + 1])
-            if reexport_name in self.api.reexport_map:
-                for mod in self.api.reexport_map[reexport_name]:
+            reexport_name_forward = ".".join(path[: i + 1])
+            if reexport_name_forward in self.api.reexport_map:
+                for mod in self.api.reexport_map[reexport_name_forward]:
+                    reexported_by.add(mod)
+
+            reexport_name_backward = ".".join(path[-i - 1 :])
+            if reexport_name_backward in self.api.reexport_map:
+                for mod in self.api.reexport_map[reexport_name_backward]:
+                    reexported_by.add(mod)
+
+            reexport_name_backward_whitelist = f"{'.'.join(path[-2 - i:-1])}.*"
+            if reexport_name_backward_whitelist in self.api.reexport_map:
+                for mod in self.api.reexport_map[reexport_name_backward_whitelist]:
                     reexported_by.add(mod)
 
         return list(reexported_by)
 
     def _add_reexports(self, module: Module) -> None:
         for qualified_import in module.qualified_imports:
             name = qualified_import.qualified_name
             self.api.reexport_map[name].add(module)
 
         for wildcard_import in module.wildcard_imports:
             name = wildcard_import.module_name
-            self.api.reexport_map[name].add(module)
+            self.api.reexport_map[f"{name}.*"].add(module)
 
     # #### Misc. utilities
     def mypy_type_to_abstract_type(
         self,
         mypy_type: mp_types.Instance | mp_types.ProperType | mp_types.Type,
         unanalyzed_type: mp_types.Type | None = None,
     ) -> AbstractType:
@@ -840,45 +926,56 @@
                     and isinstance(type_args[0], mp_types.AnyType)
                     and not has_correct_type_of_any(type_args[0].type_of_any)
                 ):
                     # This case happens if we have a list or set with multiple arguments like "list[str, int]" which is
                     # not allowed. In this case mypy interprets the type as "list[Any]", but we want the real types
                     # of the list arguments, which we cant get through the "unanalyzed_type" attribute
                     return self.mypy_type_to_abstract_type(unanalyzed_type)
+        elif isinstance(unanalyzed_type, mp_types.TupleType):
+            return sds_types.TupleType(types=[self.mypy_type_to_abstract_type(item) for item in unanalyzed_type.items])
 
         # Iterable mypy types
         if isinstance(mypy_type, mp_types.TupleType):
             return sds_types.TupleType(types=[self.mypy_type_to_abstract_type(item) for item in mypy_type.items])
         elif isinstance(mypy_type, mp_types.UnionType):
             return sds_types.UnionType(types=[self.mypy_type_to_abstract_type(item) for item in mypy_type.items])
 
         # Special Cases
         elif isinstance(mypy_type, mp_types.TypeVarType):
             upper_bound = mypy_type.upper_bound
             type_ = None
             if upper_bound.__str__() != "builtins.object":
                 type_ = self.mypy_type_to_abstract_type(upper_bound)
 
+                if mypy_type.name == "Self":
+                    # Special case, where the method returns an instance of its class
+                    return type_
+
             type_var = sds_types.TypeVarType(name=mypy_type.name, upper_bound=type_)
             self.type_var_types.add(type_var)
             return type_var
         elif isinstance(mypy_type, mp_types.CallableType):
             return sds_types.CallableType(
                 parameter_types=[self.mypy_type_to_abstract_type(arg_type) for arg_type in mypy_type.arg_types],
                 return_type=self.mypy_type_to_abstract_type(mypy_type.ret_type),
             )
         elif isinstance(mypy_type, mp_types.AnyType):
             if mypy_type.type_of_any == mp_types.TypeOfAny.from_unimported_type:
                 # If the Any type is generated b/c of from_unimported_type, then we can parse the type
                 # from the import information
                 missing_import_name = mypy_type.missing_import_name.split(".")[-1]  # type: ignore[union-attr]
                 name, qname = self._find_alias(missing_import_name)
+
+                if not qname:  # pragma: no cover
+                    logging.warning("Could not parse a type, added unknown type instead.")
+                    return sds_types.UnknownType()
+
                 return sds_types.NamedType(name=name, qname=qname)
             else:
-                return sds_types.NamedType(name="Any", qname="builtins.Any")
+                return sds_types.NamedType(name="Any", qname="typing.Any")
         elif isinstance(mypy_type, mp_types.NoneType):
             return sds_types.NamedType(name="None", qname="builtins.None")
         elif isinstance(mypy_type, mp_types.LiteralType):
             return sds_types.LiteralType(literals=[mypy_type.value])
         elif isinstance(mypy_type, mp_types.UnboundType):
             if mypy_type.name in {"list", "set"}:
                 return {
@@ -901,14 +998,19 @@
                 for module_class in module.classes:
                     if module_class.name == mypy_type.name:
                         qname = module_class.id.replace("/", ".")
                         return sds_types.NamedType(name=module_class.name, qname=qname)
 
                 # if not, we check if it's an alias
                 name, qname = self._find_alias(mypy_type.name)
+
+                if not qname:  # pragma: no cover
+                    logging.warning("Could not parse a type, added unknown type instead.")
+                    return sds_types.UnknownType()
+
                 return sds_types.NamedType(name=name, qname=qname)
 
         # Builtins
         elif isinstance(mypy_type, mp_types.Instance):
             type_name = mypy_type.type.name
             if type_name in {"int", "str", "bool", "float"}:
                 return sds_types.NamedType(name=type_name, qname=mypy_type.type.fullname)
@@ -930,63 +1032,53 @@
 
             elif type_name in {"dict", "Mapping"}:
                 return sds_types.DictType(
                     key_type=self.mypy_type_to_abstract_type(mypy_type.args[0]),
                     value_type=self.mypy_type_to_abstract_type(mypy_type.args[1]),
                 )
             else:
+                if mypy_type.args:
+                    types = [self.mypy_type_to_abstract_type(arg) for arg in mypy_type.args]
+                    return sds_types.NamedSequenceType(name=type_name, qname=mypy_type.type.fullname, types=types)
                 return sds_types.NamedType(name=type_name, qname=mypy_type.type.fullname)
-        raise ValueError("Unexpected type.")  # pragma: no cover
+
+        logging.warning("Could not parse a type, added unknown type instead.")  # pragma: no cover
+        return sds_types.UnknownType()  # pragma: no cover
 
     def _find_alias(self, type_name: str) -> tuple[str, str]:
         module = self.__declaration_stack[0]
 
         # At this point, the first item of the stack can only ever be a module
         if not isinstance(module, Module):  # pragma: no cover
             raise TypeError(f"Expected module, got {type(module)}.")
 
-        name = ""
-        qname = ""
-        qualified_imports = module.qualified_imports
-        import_aliases = [qimport.alias for qimport in qualified_imports]
+        # First we check if it can be found in the imports
+        name, qname = self._search_alias_in_qualified_imports(module.qualified_imports, type_name)
+        if name and qname:
+            return name, qname
 
         if type_name in self.aliases:
             qnames: set = self.aliases[type_name]
             if len(qnames) == 1:
-                # We have to check if this is an alias from an import
-                import_name, import_qname = self._search_alias_in_qualified_imports(qualified_imports, type_name)
-
                 # We need a deepcopy since qnames is a pointer to the set in the alias dict
-                qname = import_qname if import_qname else deepcopy(qnames).pop()
-                name = import_name if import_name else qname.split(".")[-1]
-            elif type_name in import_aliases:
-                # We check if the type was imported
-                qimport_name, qimport_qname = self._search_alias_in_qualified_imports(qualified_imports, type_name)
-
-                if qimport_qname:
-                    qname = qimport_qname
-                    name = qimport_name
+                qname = deepcopy(qnames).pop()
+                name = qname.split(".")[-1]
             else:
                 # In this case some types where defined in multiple modules with the same names.
                 for alias_qname in qnames:
                     # We check if the type was defined in the same module
                     type_path = ".".join(alias_qname.split(".")[0:-1])
                     name = alias_qname.split(".")[-1]
 
                     if self.mypy_file is None:  # pragma: no cover
                         raise TypeError("Expected mypy_file (module information), got None.")
 
-                    if type_path == self.mypy_file.fullname:
+                    if self.mypy_file.fullname in type_path:
                         qname = alias_qname
                         break
-        else:
-            name, qname = self._search_alias_in_qualified_imports(qualified_imports, type_name)
-
-        if not qname:  # pragma: no cover
-            raise ValueError(f"It was not possible to find out where the alias {type_name} was defined.")
 
         return name, qname
 
     @staticmethod
     def _search_alias_in_qualified_imports(
         qualified_imports: list[QualifiedImport],
         alias_name: str,
@@ -1028,20 +1120,20 @@
         """Create an ID for a new object using previous objects of the stack.
 
         Creates an ID by connecting the previous objects of the __declaration_stack stack and the new objects name,
         which is on the highest level.
 
         Paramters
         ---------
-        name : str
+        name:
             The name of the new object which lies on the highest level.
 
         Returns
         -------
-        str
+        id:
             ID of the object
         """
         segments = [
             it.id if isinstance(it, Module) else it.name  # Special case, to get the module path info the id
             for it in self.__declaration_stack
             if not isinstance(it, list)  # Check for the linter, on runtime can never be list type
         ]
@@ -1058,25 +1150,30 @@
     def _check_publicity_in_reexports(self, name: str, qname: str, parent: Module | Class) -> bool | None:
         not_internal = not is_internal(name)
         module_qname = getattr(self.mypy_file, "fullname", "")
         module_name = getattr(self.mypy_file, "name", "")
         package_id = "/".join(module_qname.split(".")[:-1])
 
         for reexported_key in self.api.reexport_map:
-            module_is_reexported = reexported_key in {module_name, module_qname}
+            module_is_reexported = reexported_key in {
+                module_name,
+                module_qname,
+                f"{module_name}.*",
+                f"{module_qname}.*",
+            }
 
             # Check if the function/class/module is reexported
             if reexported_key.endswith(name) or module_is_reexported:
 
                 # Iterate through all sources (__init__.py files) where it was reexported
                 for reexport_source in self.api.reexport_map[reexported_key]:
 
                     # We have to check if it's the correct reexport with the ID
                     is_from_same_package = reexport_source.id == package_id
-                    is_from_another_package = reexported_key in {qname, module_qname}
+                    is_from_another_package = reexported_key.rstrip(".*") in {qname, module_qname}
                     if not is_from_same_package and not is_from_another_package:
                         continue
 
                     # If the whole module was reexported we have to check if the name or alias is intern
                     if module_is_reexported:
 
                         # Check the wildcard imports of the source
@@ -1123,9 +1220,12 @@
                                 # If a specific func / class was reexported check
                                 #   1. If it has an alias and if it's alias is internal
                                 #   2. Else if it has no alias and is not internal
                                 return True
         return None
 
 
-def is_internal(name: str) -> bool:
-    return name.startswith("_")
+def result_name_generator() -> Generator:
+    """Generate a name for callable type parameters starting from 'a' until 'zz'."""
+    while True:
+        for x in range(1, 1000):
+            yield f"result_{x}"
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_ast_walker.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_ast_walker.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,45 +37,36 @@
 
         if node in visited_nodes:  # pragma: no cover
             raise AssertionError("Node visited twice")
         visited_nodes.add(node)
 
         self.__enter(node)
 
-        definitions: list = []
+        # Search nodes for more child nodes. Skip other not specified types, since we either get them through the
+        # ast_visitor, some other way or don't need to parse them at all
+        child_nodes = []
         if isinstance(node, MypyFile):
             definitions = get_mypyfile_definitions(node)
+            child_nodes = [
+                _def for _def in definitions if _def.__class__.__name__ in {"FuncDef", "ClassDef", "Decorator"}
+            ]
         elif isinstance(node, ClassDef):
             definitions = get_classdef_definitions(node)
-        elif isinstance(node, FuncDef):
+            child_nodes = [
+                _def
+                for _def in definitions
+                if _def.__class__.__name__ in {"AssignmentStmt", "FuncDef", "ClassDef", "Decorator"}
+            ]
+        elif isinstance(node, FuncDef) and node.name == "__init__":
             definitions = get_funcdef_definitions(node)
-
-        # Skip other types, since we either get them through the ast_visitor, some other way or
-        # don't need to parse them
-        child_nodes = [
-            _def
-            for _def in definitions
-            if _def.__class__.__name__
-            in {
-                "AssignmentStmt",
-                "FuncDef",
-                "ClassDef",
-                "Decorator",
-            }
-        ]
+            child_nodes = [_def for _def in definitions if _def.__class__.__name__ == "AssignmentStmt"]
 
         for child_node in child_nodes:
-            # Ignore global variables and function attributes if the function is an __init__
-            if isinstance(child_node, AssignmentStmt):
-                if isinstance(node, MypyFile):
-                    continue
-                if isinstance(node, FuncDef) and node.name != "__init__":
-                    continue
-
-            if isinstance(child_node, FuncDef) and isinstance(node, FuncDef):
+            # The '__mypy-replace' name is a mypy placeholer which we don't want to parse.
+            if getattr(child_node, "name", "") == "__mypy-replace":  # pragma: no cover
                 continue
 
             self.__walk(child_node, visited_nodes)
         self.__leave(node)
 
     def __enter(self, node: MypyFile | ClassDef | FuncDef | AssignmentStmt) -> None:
         method = self.__get_callbacks(node)[0]
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_get_api.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_get_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,41 +10,38 @@
 from mypy import types as mypy_types
 
 from safeds_stubgen.docstring_parsing import DocstringStyle, create_docstring_parser
 
 from ._api import API
 from ._ast_visitor import MyPyAstVisitor
 from ._ast_walker import ASTWalker
-from ._package_metadata import distribution, distribution_version, package_root
+from ._package_metadata import distribution, distribution_version
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
 def get_api(
-    package_name: str,
-    root: Path | None = None,
+    root: Path,
     docstring_style: DocstringStyle = DocstringStyle.PLAINTEXT,
     is_test_run: bool = False,
 ) -> API:
-    # Check root
-    if root is None:
-        root = package_root(package_name)
+    init_roots = _get_nearest_init_dirs(root)
+    if len(init_roots) == 1:
+        root = init_roots[0]
+
+    logging.info("Started gathering the raw package data with Mypy.")
 
     walkable_files = []
     package_paths = []
     for file_path in root.glob(pattern="./**/*.py"):
-        logging.info(
-            "Working on file {posix_path}",
-            extra={"posix_path": str(file_path)},
-        )
-
         # Check if the current path is a test directory
-        if not is_test_run and ("test" in file_path.parts or "tests" in file_path.parts):
-            logging.info("Skipping test file")
+        if not is_test_run and ("test" in file_path.parts or "tests" in file_path.parts or "docs" in file_path.parts):
+            log_msg = f"Skipping test file in {file_path}"
+            logging.info(log_msg)
             continue
 
         # Check if the current file is an init file
         if file_path.parts[-1] == "__init__.py":
             # if a directory contains an __init__.py file it's a package
             package_paths.append(
                 str(file_path.parent),
@@ -52,35 +49,57 @@
             continue
 
         walkable_files.append(str(file_path))
 
     if not walkable_files:
         raise ValueError("No files found to analyse.")
 
+    # Package name
+    package_name = root.stem
+
     # Get distribution data
-    dist = distribution(package_name) or ""
-    dist_version = distribution_version(dist) or ""
+    dist = distribution(package_name=package_name) or ""
+    dist_version = distribution_version(dist=dist) or ""
 
     # Get mypy ast and aliases
-    build_result = _get_mypy_build(walkable_files)
-    mypy_asts = _get_mypy_asts(build_result, walkable_files, package_paths)
-    aliases = _get_aliases(build_result.types, package_name)
+    build_result = _get_mypy_build(files=walkable_files)
+    mypy_asts = _get_mypy_asts(build_result=build_result, files=walkable_files, package_paths=package_paths)
+    aliases = _get_aliases(result_types=build_result.types, package_name=package_name)
 
     # Setup api walker
-    api = API(dist, package_name, dist_version)
-    docstring_parser = create_docstring_parser(docstring_style)
-    callable_visitor = MyPyAstVisitor(docstring_parser, api, aliases)
-    walker = ASTWalker(callable_visitor)
+    api = API(distribution=dist, package=package_name, version=dist_version)
+    docstring_parser = create_docstring_parser(style=docstring_style, package_path=root)
+    callable_visitor = MyPyAstVisitor(docstring_parser=docstring_parser, api=api, aliases=aliases)
+    walker = ASTWalker(handler=callable_visitor)
 
     for tree in mypy_asts:
-        walker.walk(tree)
+        walker.walk(tree=tree)
 
     return callable_visitor.api
 
 
+def _get_nearest_init_dirs(root: Path) -> list[Path]:
+    all_inits = list(root.glob("./**/__init__.py"))
+    shortest_init_paths = []
+    shortest_len = -1
+    for init in all_inits:
+        path_len = len(init.parts)
+        if shortest_len == -1:
+            shortest_len = path_len
+            shortest_init_paths.append(init.parent)
+        elif path_len <= shortest_len:  # pragma: no cover
+            if path_len == shortest_len:
+                shortest_init_paths.append(init.parent)
+            else:
+                shortest_len = path_len
+                shortest_init_paths = [init.parent]
+
+    return shortest_init_paths
+
+
 def _get_mypy_build(files: list[str]) -> mypy_build.BuildResult:
     """Build a mypy checker and return the build result."""
     mypyfiles, opt = mypy_main.process_options(files)
 
     # Disable the memory optimization of freeing ASTs when possible
     opt.preserve_asts = True
     # Only check parts of the code that have changed since the last check
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_mypy_helpers.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_mypy_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,14 @@
             raise ValueError("Mypy variance parser received an illegal parameter value.")
 
 
 def has_correct_type_of_any(type_of_any: int) -> bool:
     # In Mypy AnyType can be set as type because of different reasons (see TypeOfAny class-documentation)
     return type_of_any in {
         mp_types.TypeOfAny.explicit,
-        mp_types.TypeOfAny.from_omitted_generics,
         mp_types.TypeOfAny.from_another_any,
         mp_types.TypeOfAny.from_unimported_type,
     }
 
 
 def mypy_expression_to_sds_type(expr: mp_nodes.Expression) -> sds_types.AbstractType:
     if isinstance(expr, mp_nodes.NameExpr):
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/_types.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from __future__ import annotations
 
 import re
 from abc import ABCMeta, abstractmethod
+from collections import Counter
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any, ClassVar
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
 
 class AbstractType(metaclass=ABCMeta):
     @classmethod
     def from_dict(cls, d: dict[str, Any]) -> AbstractType:
         match d["kind"]:
+            case UnknownType.__name__:
+                return UnknownType.from_dict(d)
             case NamedType.__name__:
                 return NamedType.from_dict(d)
+            case NamedSequenceType.__name__:
+                return NamedSequenceType.from_dict(d)
             case EnumType.__name__:
                 return EnumType.from_dict(d)
             case BoundaryType.__name__:
                 return BoundaryType.from_dict(d)
             case ListType.__name__:
                 return ListType.from_dict(d)
             case DictType.__name__:
@@ -41,14 +46,29 @@
                 raise ValueError(f"Cannot parse {d['kind']} value.")
 
     @abstractmethod
     def to_dict(self) -> dict[str, Any]: ...
 
 
 @dataclass(frozen=True)
+class UnknownType(AbstractType):
+    @classmethod
+    def from_dict(cls, _: dict[str, Any]) -> UnknownType:
+        return UnknownType()
+
+    def to_dict(self) -> dict[str, str]:
+        return {"kind": self.__class__.__name__}
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, UnknownType):  # pragma: no cover
+            return NotImplemented
+        return True
+
+
+@dataclass(frozen=True)
 class NamedType(AbstractType):
     name: str
     qname: str
 
     @classmethod
     def from_dict(cls, d: dict[str, Any]) -> NamedType:
         return NamedType(d["name"], d["qname"])
@@ -62,14 +82,46 @@
         return self.name == other.name and self.qname == other.qname
 
     def __hash__(self) -> int:
         return hash((self.name, self.qname))
 
 
 @dataclass(frozen=True)
+class NamedSequenceType(AbstractType):
+    name: str
+    qname: str
+    types: Sequence[AbstractType]
+
+    @classmethod
+    def from_dict(cls, d: dict[str, Any]) -> NamedSequenceType:
+        types = []
+        for element in d["types"]:
+            type_ = AbstractType.from_dict(element)
+            if type_ is not None:
+                types.append(type_)
+        return NamedSequenceType(name=d["name"], qname=d["qname"], types=types)
+
+    def to_dict(self) -> dict[str, Any]:
+        return {
+            "kind": self.__class__.__name__,
+            "name": self.name,
+            "qname": self.qname,
+            "types": [t.to_dict() for t in self.types],
+        }
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, NamedSequenceType):  # pragma: no cover
+            return NotImplemented
+        return Counter(self.types) == Counter(other.types) and self.name == other.name and self.qname == other.qname
+
+    def __hash__(self) -> int:
+        return hash(frozenset([self.name, self.qname, *self.types]))
+
+
+@dataclass(frozen=True)
 class EnumType(AbstractType):
     values: frozenset[str] = field(default_factory=frozenset)
     full_match: str = field(default="", compare=False)
 
     @classmethod
     def from_dict(cls, d: dict[str, Any]) -> EnumType:
         return EnumType(d["values"])
@@ -240,14 +292,19 @@
             type_list.append(t.to_dict())
 
         return {"kind": self.__class__.__name__, "types": type_list}
 
     def __hash__(self) -> int:
         return hash(frozenset(self.types))
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, UnionType):  # pragma: no cover
+            return NotImplemented
+        return Counter(self.types) == Counter(other.types)
+
 
 @dataclass(frozen=True)
 class ListType(AbstractType):
     types: Sequence[AbstractType]
 
     @classmethod
     def from_dict(cls, d: dict[str, Any]) -> ListType:
@@ -259,14 +316,19 @@
         return ListType(types)
 
     def to_dict(self) -> dict[str, Any]:
         type_list = [t.to_dict() for t in self.types]
 
         return {"kind": self.__class__.__name__, "types": type_list}
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, ListType):  # pragma: no cover
+            return NotImplemented
+        return Counter(self.types) == Counter(other.types)
+
     def __hash__(self) -> int:
         return hash(frozenset(self.types))
 
 
 @dataclass(frozen=True)
 class DictType(AbstractType):
     key_type: AbstractType
@@ -305,14 +367,19 @@
     def to_dict(self) -> dict[str, Any]:
         return {
             "kind": self.__class__.__name__,
             "parameter_types": [t.to_dict() for t in self.parameter_types],
             "return_type": self.return_type.to_dict(),
         }
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, CallableType):  # pragma: no cover
+            return NotImplemented
+        return Counter(self.parameter_types) == Counter(other.parameter_types) and self.return_type == other.return_type
+
     def __hash__(self) -> int:
         return hash(frozenset([*self.parameter_types, self.return_type]))
 
 
 @dataclass(frozen=True)
 class SetType(AbstractType):
     types: Sequence[AbstractType]
@@ -328,14 +395,19 @@
 
     def to_dict(self) -> dict[str, Any]:
         return {
             "kind": self.__class__.__name__,
             "types": [t.to_dict() for t in self.types],
         }
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, SetType):  # pragma: no cover
+            return NotImplemented
+        return Counter(self.types) == Counter(other.types)
+
     def __hash__(self) -> int:
         return hash(frozenset(self.types))
 
 
 @dataclass(frozen=True)
 class LiteralType(AbstractType):
     literals: list[str | int | float | bool]
@@ -343,14 +415,19 @@
     @classmethod
     def from_dict(cls, d: dict[str, Any]) -> LiteralType:
         return LiteralType(d["literals"])
 
     def to_dict(self) -> dict[str, Any]:
         return {"kind": self.__class__.__name__, "literals": self.literals}
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, LiteralType):  # pragma: no cover
+            return NotImplemented
+        return Counter(self.literals) == Counter(other.literals)
+
     def __hash__(self) -> int:
         return hash(frozenset(self.literals))
 
 
 @dataclass(frozen=True)
 class FinalType(AbstractType):
     type_: AbstractType
@@ -380,14 +457,19 @@
         return TupleType(types)
 
     def to_dict(self) -> dict[str, Any]:
         type_list = [t.to_dict() for t in self.types]
 
         return {"kind": self.__class__.__name__, "types": type_list}
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, TupleType):  # pragma: no cover
+            return NotImplemented
+        return Counter(self.types) == Counter(other.types)
+
     def __hash__(self) -> int:
         return hash(frozenset(self.types))
 
 
 @dataclass(frozen=True)
 class TypeVarType(AbstractType):
     name: str
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/api_analyzer/cli/_cli.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/api_analyzer/cli/_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,50 +2,40 @@
 
 import argparse
 import logging
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from safeds_stubgen.api_analyzer import get_api
-from safeds_stubgen.stubs_generator import generate_stubs
+from safeds_stubgen.stubs_generator import StubsStringGenerator, create_stub_files, generate_stub_data
 
 if TYPE_CHECKING:
     from safeds_stubgen.docstring_parsing import DocstringStyle
 
 
 def cli() -> None:
     args = _get_args()
     if args.verbose:
         logging.basicConfig(level=logging.INFO)
 
-    _run_api_command(args.package, args.src, args.out, args.docstyle, args.testrun, args.naming_convert)
+    _run_stub_generator(args.src.resolve(), args.out.resolve(), args.docstyle, args.testrun, args.naming_convert)
 
 
 def _get_args() -> argparse.Namespace:
     from safeds_stubgen.docstring_parsing import DocstringStyle
 
     parser = argparse.ArgumentParser(description="Analyze Python code.")
 
     parser.add_argument("-v", "--verbose", help="show info messages", action="store_true")
     parser.add_argument(
-        "-p",
-        "--package",
-        help="The name of the package.",
-        type=str,
-        required=True,
-    )
-    parser.add_argument(
         "-s",
         "--src",
-        help=(
-            "Directory containing the Python code of the package. If this is omitted, we try to locate the package "
-            "with the given name in the current Python interpreter."
-        ),
+        help="Source directory containing the Python code of the package.",
         type=Path,
-        required=False,
+        required=True,
         default=None,
     )
     parser.add_argument("-o", "--out", help="Output directory.", type=Path, required=True)
     parser.add_argument(
         "--docstyle",
         help="The docstring style.",
         type=DocstringStyle.from_string,
@@ -70,34 +60,37 @@
         required=False,
         action="store_true",
     )
 
     return parser.parse_args()
 
 
-def _run_api_command(
-    package: str,
+def _run_stub_generator(
     src_dir_path: Path,
     out_dir_path: Path,
     docstring_style: DocstringStyle,
     is_test_run: bool,
     convert_identifiers: bool,
 ) -> None:
     """
-    List the API of a package.
+    Create API data of a package and Safe-DS stub files.
 
     Parameters
     ----------
-    package : str
-        The name of the package.
-    out_dir_path : Path
+    out_dir_path:
         The path to the output directory.
-    docstring_style : DocstringStyle
+    docstring_style:
         The style of docstrings that used in the library.
-    is_test_run : bool
+    is_test_run:
         Set True if files in test directories should be parsed too.
     """
-    api = get_api(package, src_dir_path, docstring_style, is_test_run)
-    out_file_api = out_dir_path.joinpath(f"{package}__api.json")
+    # Generate the API data
+    api = get_api(root=src_dir_path, docstring_style=docstring_style, is_test_run=is_test_run)
+    # Create an API file
+    out_file_api = out_dir_path.joinpath(f"{src_dir_path.stem}__api.json")
     api.to_json_file(out_file_api)
 
-    generate_stubs(api, out_dir_path, convert_identifiers)
+    # Generate the stub data
+    stubs_generator = StubsStringGenerator(api=api, convert_identifiers=convert_identifiers)
+    stub_data = generate_stub_data(stubs_generator=stubs_generator, out_path=out_dir_path)
+    # Create the stub files
+    create_stub_files(stubs_generator=stubs_generator, stubs_data=stub_data, out_path=out_dir_path)
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/__init__.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/_create_docstring_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-"""Parsing docstrings into a common format."""
+from __future__ import annotations
 
-from ._abstract_docstring_parser import AbstractDocstringParser
-from ._create_docstring_parser import create_docstring_parser
-from ._docstring import AttributeDocstring, ClassDocstring, FunctionDocstring, ParameterDocstring, ResultDocstring
+from typing import TYPE_CHECKING
+
+from griffe.enumerations import Parser
+
+from ._docstring_parser import DocstringParser
 from ._docstring_style import DocstringStyle
-from ._epydoc_parser import EpydocParser
-from ._googledoc_parser import GoogleDocParser
-from ._numpydoc_parser import NumpyDocParser
 from ._plaintext_docstring_parser import PlaintextDocstringParser
-from ._restdoc_parser import RestDocParser
 
-__all__ = [
-    "AbstractDocstringParser",
-    "AttributeDocstring",
-    "ClassDocstring",
-    "create_docstring_parser",
-    "DocstringStyle",
-    "EpydocParser",
-    "FunctionDocstring",
-    "GoogleDocParser",
-    "NumpyDocParser",
-    "ParameterDocstring",
-    "PlaintextDocstringParser",
-    "RestDocParser",
-    "ResultDocstring",
-]
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from ._abstract_docstring_parser import AbstractDocstringParser
+
+
+def create_docstring_parser(style: DocstringStyle, package_path: Path) -> AbstractDocstringParser:
+    if style == DocstringStyle.GOOGLE:
+        return DocstringParser(parser=Parser.google, package_path=package_path)
+    elif style == DocstringStyle.NUMPYDOC:
+        return DocstringParser(parser=Parser.numpy, package_path=package_path)
+    elif style == DocstringStyle.REST:
+        return DocstringParser(parser=Parser.sphinx, package_path=package_path)
+    else:
+        return PlaintextDocstringParser()
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_abstract_docstring_parser.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/_abstract_docstring_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from mypy import nodes
 
-    from safeds_stubgen.api_analyzer import Class, ParameterAssignment
-
     from ._docstring import (
         AttributeDocstring,
         ClassDocstring,
         FunctionDocstring,
         ParameterDocstring,
         ResultDocstring,
     )
@@ -25,25 +23,24 @@
     @abstractmethod
     def get_function_documentation(self, function_node: nodes.FuncDef) -> FunctionDocstring:
         pass  # pragma: no cover
 
     @abstractmethod
     def get_parameter_documentation(
         self,
-        function_node: nodes.FuncDef,
+        function_qname: str,
         parameter_name: str,
-        parameter_assigned_by: ParameterAssignment,
-        parent_class: Class | None,
+        parent_class_qname: str,
     ) -> ParameterDocstring:
         pass  # pragma: no cover
 
     @abstractmethod
     def get_attribute_documentation(
         self,
-        parent_class: Class,
+        parent_class_qname: str,
         attribute_name: str,
     ) -> AttributeDocstring:
         pass  # pragma: no cover
 
     @abstractmethod
-    def get_result_documentation(self, function_node: nodes.FuncDef) -> ResultDocstring:
+    def get_result_documentation(self, function_qname: str) -> list[ResultDocstring]:
         pass  # pragma: no cover
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_create_docstring_parser.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
+"""Parsing docstrings into a common format."""
 
+from ._abstract_docstring_parser import AbstractDocstringParser
+from ._create_docstring_parser import create_docstring_parser
+from ._docstring import (
+    AttributeDocstring,
+    ClassDocstring,
+    FunctionDocstring,
+    ParameterDocstring,
+    ResultDocstring,
+)
+from ._docstring_parser import DocstringParser
 from ._docstring_style import DocstringStyle
-from ._epydoc_parser import EpydocParser
-from ._googledoc_parser import GoogleDocParser
-from ._numpydoc_parser import NumpyDocParser
 from ._plaintext_docstring_parser import PlaintextDocstringParser
-from ._restdoc_parser import RestDocParser
-
-if TYPE_CHECKING:
-    from ._abstract_docstring_parser import AbstractDocstringParser
-
 
-def create_docstring_parser(style: DocstringStyle) -> AbstractDocstringParser:
-    if style == DocstringStyle.EPYDOC:
-        return EpydocParser()
-    elif style == DocstringStyle.GOOGLE:
-        return GoogleDocParser()
-    elif style == DocstringStyle.NUMPYDOC:
-        return NumpyDocParser()
-    elif style == DocstringStyle.REST:
-        return RestDocParser()
-    else:
-        return PlaintextDocstringParser()
+__all__ = [
+    "AbstractDocstringParser",
+    "AttributeDocstring",
+    "ClassDocstring",
+    "create_docstring_parser",
+    "DocstringParser",
+    "DocstringStyle",
+    "FunctionDocstring",
+    "ParameterDocstring",
+    "PlaintextDocstringParser",
+    "ResultDocstring",
+]
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_helpers.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/_helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from __future__ import annotations
 
 import inspect
-from typing import TYPE_CHECKING
 
 from mypy import nodes
 
-if TYPE_CHECKING:
-    from docstring_parser import Docstring
-
 
 def get_full_docstring(declaration: nodes.ClassDef | nodes.FuncDef) -> str:
     """
     Return the full docstring of the given declaration.
 
     If no docstring is available, an empty string is returned. Indentation is cleaned up.
     """
@@ -26,23 +22,7 @@
 
     full_docstring = ""
     for definition in definitions:
         if isinstance(definition, nodes.ExpressionStmt) and isinstance(definition.expr, nodes.StrExpr):
             full_docstring = definition.expr.value
 
     return inspect.cleandoc(full_docstring)
-
-
-def get_description(docstring_obj: Docstring) -> str:
-    """
-    Return the concatenated short and long description of the given docstring object.
-
-    If these parts are blank, an empty string is returned.
-    """
-    summary: str = docstring_obj.short_description or ""
-    extended_summary: str = docstring_obj.long_description or ""
-
-    result = ""
-    result += summary.rstrip()
-    result += "\n\n"
-    result += extended_summary.rstrip()
-    return result.strip()
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/docstring_parsing/_plaintext_docstring_parser.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/docstring_parsing/_plaintext_docstring_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from ._abstract_docstring_parser import AbstractDocstringParser
-from ._docstring import AttributeDocstring, ClassDocstring, FunctionDocstring, ParameterDocstring, ResultDocstring
+from ._docstring import (
+    AttributeDocstring,
+    ClassDocstring,
+    FunctionDocstring,
+    ParameterDocstring,
+    ResultDocstring,
+)
 from ._helpers import get_full_docstring
 
 if TYPE_CHECKING:
     from mypy import nodes
 
-    from safeds_stubgen.api_analyzer import Class, ParameterAssignment
-
 
 class PlaintextDocstringParser(AbstractDocstringParser):
     """Parses documentation in any format. Should not be used if there is another parser for the specific format."""
 
     def get_class_documentation(self, class_node: nodes.ClassDef) -> ClassDocstring:
         docstring = get_full_docstring(class_node)
 
@@ -29,26 +33,25 @@
         return FunctionDocstring(
             description=docstring,
             full_docstring=docstring,
         )
 
     def get_parameter_documentation(
         self,
-        function_node: nodes.FuncDef,  # noqa: ARG002
+        function_qname: str,  # noqa: ARG002
         parameter_name: str,  # noqa: ARG002
-        parameter_assigned_by: ParameterAssignment,  # noqa: ARG002
-        parent_class: Class | None,  # noqa: ARG002
+        parent_class_qname: str,  # noqa: ARG002
     ) -> ParameterDocstring:
         return ParameterDocstring()
 
     def get_attribute_documentation(
         self,
-        parent_class: Class,  # noqa: ARG002
+        parent_class_qname: str,  # noqa: ARG002
         attribute_name: str,  # noqa: ARG002
     ) -> AttributeDocstring:
         return AttributeDocstring()
 
     def get_result_documentation(
         self,
-        function_node: nodes.FuncDef,  # noqa: ARG002
-    ) -> ResultDocstring:
-        return ResultDocstring()
+        function_qname: str,  # noqa: ARG002
+    ) -> list[ResultDocstring]:
+        return []
```

### Comparing `safe_ds_stubgen-0.2.0/src/safeds_stubgen/stubs_generator/_generate_stubs.py` & `safe_ds_stubgen-0.3.0/src/safeds_stubgen/stubs_generator/_stub_string_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,222 +1,165 @@
 from __future__ import annotations
 
-from enum import IntEnum
+import logging
+from collections import defaultdict
 from pathlib import Path
+from types import NoneType
 from typing import TYPE_CHECKING
 
+from safeds_stubgen import is_internal
 from safeds_stubgen.api_analyzer import (
     API,
     Attribute,
     Class,
     Enum,
     Function,
     Module,
     Parameter,
     ParameterAssignment,
     Result,
     UnionType,
     VarianceKind,
+    result_name_generator,
 )
+from safeds_stubgen.docstring_parsing import AttributeDocstring
 
-if TYPE_CHECKING:
-    from collections.abc import Generator
-
-    from safeds_stubgen.docstring_parsing import AttributeDocstring, ClassDocstring, FunctionDocstring
-
-
-class NamingConvention(IntEnum):
-    PYTHON = 1
-    SAFE_DS = 2
-
-
-def generate_stubs(api: API, out_path: Path, convert_identifiers: bool) -> None:
-    """Generate Safe-DS stubs.
-
-    Generates stub files from an API object and writes them to the out_path path.
-
-    Parameters
-    ----------
-    api
-        The API object from which the stubs
-    out_path
-        The path in which the stub files should be created. If no such path exists this function creates the directory
-        files.
-    convert_identifiers
-        Set this True if the identifiers should be converted to Safe-DS standard (UpperCamelCase for classes and
-        camelCase for everything else).
-    """
-    naming_convention = NamingConvention.SAFE_DS if convert_identifiers else NamingConvention.PYTHON
-    stubs_generator = StubsStringGenerator(api, naming_convention)
-    stubs_data = _generate_stubs_data(api, out_path, stubs_generator)
-    _generate_stubs_files(stubs_data, out_path, stubs_generator, naming_convention)
-
-
-def _generate_stubs_data(
-    api: API,
-    out_path: Path,
-    stubs_generator: StubsStringGenerator,
-) -> list[tuple[Path, str, str]]:
-    stubs_data: list[tuple[Path, str, str]] = []
-    for module in api.modules.values():
-        if module.name == "__init__":
-            continue
-
-        module_text = stubs_generator(module)
-
-        # Each text block we create ends with "\n", therefore, if there is only the package information
-        # the file would look like this: "package path.to.myPackage\n" or this:
-        # '@PythonModule("path.to.my_package")\npackage path.to.myPackage\n'. With the split we check if the module
-        # has enough information, if not, we won't create it.
-        _module_text = module_text
-        if _module_text.startswith("/**"):
-            # Remove docstring
-            _module_text = "*/\n".join(_module_text.split("*/\n\n")[1:])
-        splitted_text = _module_text.split("\n")
-        if len(splitted_text) <= 2 or (len(splitted_text) == 3 and splitted_text[1].startswith("package ")):
-            continue
-
-        module_dir = Path(out_path / module.id)
-        stubs_data.append((module_dir, module.name, module_text))
-    return stubs_data
-
-
-def _generate_stubs_files(
-    stubs_data: list[tuple[Path, str, str]],
-    out_path: Path,
-    stubs_generator: StubsStringGenerator,
-    naming_convention: NamingConvention,
-) -> None:
-    for module_dir, module_name, module_text in stubs_data:
-        # Create module dir
-        module_dir.mkdir(parents=True, exist_ok=True)
-
-        # Create and open module file
-        file_path = Path(module_dir / f"{module_name}.sdsstub")
-        Path(file_path).touch()
-
-        with file_path.open("w") as f:
-            f.write(module_text)
-
-    created_module_paths: set[str] = set()
-    classes_outside_package = list(stubs_generator.classes_outside_package)
-    classes_outside_package.sort()
-    for class_ in classes_outside_package:
-        created_module_paths = _create_outside_package_class(class_, out_path, naming_convention, created_module_paths)
-
-
-def _create_outside_package_class(
-    class_path: str,
-    out_path: Path,
-    naming_convention: NamingConvention,
-    created_module_paths: set[str],
-) -> set[str]:
-    path_parts = class_path.split(".")
-    class_name = path_parts.pop(-1)
-    module_name = path_parts[-1]
-    module_path = "/".join(path_parts)
-
-    first_creation = False
-    if module_path not in created_module_paths:
-        created_module_paths.add(module_path)
-        first_creation = True
-
-    module_dir = Path(out_path / module_path)
-    module_dir.mkdir(parents=True, exist_ok=True)
-
-    file_path = Path(module_dir / f"{module_name}.sdsstub")
-    if Path.exists(file_path) and not first_creation:
-        with file_path.open("a") as f:
-            f.write(_create_outside_package_class_text(class_name, naming_convention))
-    else:
-        with file_path.open("w") as f:
-            module_text = ""
-
-            # package name & annotation
-            python_module_path = ".".join(path_parts)
-            module_path_camel_case = _convert_name_to_convention(python_module_path, naming_convention)
-            module_name_info = ""
-            if python_module_path != module_path_camel_case:
-                module_text += f'@PythonModule("{python_module_path}")\n'
-            module_text += f"{module_name_info}package {module_path_camel_case}\n"
-
-            module_text += _create_outside_package_class_text(class_name, naming_convention)
-
-            f.write(module_text)
-
-    return created_module_paths
-
-
-def _create_outside_package_class_text(class_name: str, naming_convention: NamingConvention) -> str:
-    # to camel case
-    camel_case_name = _convert_name_to_convention(class_name, naming_convention, is_class_name=True)
-
-    # add name annotation
-    class_annotation = ""
-    if class_name != camel_case_name:
-        class_annotation = f"\n{_create_name_annotation(class_name)}"
-
-    # check for identifiers
-    safe_class_name = _replace_if_safeds_keyword(camel_case_name)
+from ._helper import (
+    INDENTATION,
+    NamingConvention,
+    _convert_name_to_convention,
+    _create_name_annotation,
+    _get_shortest_public_reexport,
+    _replace_if_safeds_keyword,
+)
 
-    return f"{class_annotation}\nclass {safe_class_name}\n"
+if TYPE_CHECKING:
+    from safeds_stubgen.docstring_parsing import ClassDocstring, FunctionDocstring
 
 
 class StubsStringGenerator:
     """Generate Safe-DS stub strings.
 
     Generates stub string for Safe-DS. Each part has its own method, but it all starts with the create_module_string
     method.
     """
 
-    def __init__(self, api: API, naming_convention: NamingConvention) -> None:
+    def __init__(self, api: API, convert_identifiers: bool) -> None:
+        self.module_id: str = ""
+        self.class_generics: list = []
+        self.module_imports: set[str] = set()
+
         self.api = api
-        self.naming_convention = naming_convention
+        self.naming_convention = NamingConvention.SAFE_DS if convert_identifiers else NamingConvention.PYTHON
         self.classes_outside_package: set[str] = set()
+        self.reexport_modules: dict[str, list[Class | Function]] = defaultdict(list)
+
+    def __call__(self, module: Module) -> tuple[str, str]:
+        self.module_id = module.id
+        self.class_generics = []
+        self.module_imports = set()
 
-    def __call__(self, module: Module) -> str:
-        self.module_imports: set[str] = set()
         self._current_todo_msgs: set[str] = set()
-        self.module = module
-        self.class_generics: list = []
-        return self._create_module_string()
+        return self._create_module_string(module)
+
+    def create_reexport_module_strings(self, out_path: Path) -> list[tuple[Path, str, str, bool]]:
+        module_data = []
+        for module_id in self.reexport_modules:
+            elements: list[Class | Function] = self.reexport_modules[module_id]
+
+            # We sort for the snapshot tests
+            elements.sort(key=lambda x: x.name)
+
+            for element in elements:
+                # Reset the objects that we normally would reset in the __call__
+                self.module_imports = set()
+                self.class_generics = []
+
+                module_name = element.name
+                self.module_id = f"{module_id}/{module_name}"
+
+                # Create module header
+                package_info = ".".join(self.module_id.split("/")[:-1])
+                package_info_camel_case = _convert_name_to_convention(package_info, self.naming_convention)
+                module_name_info = ""
+                if package_info != package_info_camel_case:
+                    module_name_info = f'@PythonModule("{package_info}")\n'
+                module_header = f"{module_name_info}package {package_info_camel_case}\n"
+
+                # Create body text
+                if isinstance(element, Class):
+                    module_text = f"\n{self._create_class_string(class_=element, in_reexport_module=True)}\n"
+                elif isinstance(element, Function):
+                    module_text = f"\n{self._create_function_string(function=element, in_reexport_module=True)}\n"
+                else:  # pragma: no cover
+                    msg = f"Could not create a module for {element.id}. Unsupported type {type(element)}."
+                    logging.warning(msg)
+                    continue
+
+                # Create imports
+                #  We have to create them last, since we have to check all used types in this module first
+                module_header += self._create_imports_string()
+                module_text = module_header + module_text
+                module_data.append((Path(out_path / self.module_id), module_name, module_text, True))
+
+        return module_data
+
+    def _create_module_string(self, module: Module) -> tuple[str, str]:
+        module_text = ""
 
-    def _create_module_string(self) -> str:
         # Create package info
-        package_info = self._get_shortest_public_reexport()
+        package_info, _ = _get_shortest_public_reexport(
+            reexport_map=self.api.reexport_map,
+            name=module.name,
+            qname="",
+            is_module=True,
+        )
+
+        in_reexport_module = bool(package_info)
+
+        if not package_info:
+            package_info = ".".join(module.id.split("/"))
+
         package_info_camel_case = _convert_name_to_convention(package_info, self.naming_convention)
         module_name_info = ""
-        module_text = ""
         if package_info != package_info_camel_case:
             module_name_info = f'@PythonModule("{package_info}")\n'
         module_header = f"{module_name_info}package {package_info_camel_case}\n"
 
         # Create docstring
-        docstring = self._create_sds_docstring_description(self.module.docstring, "")
+        docstring = self._create_sds_docstring_description(module.docstring, "")
         if docstring:
             docstring += "\n"
 
         # Create global functions and properties
-        for function in self.module.global_functions:
+        for function in module.global_functions:
             if function.is_public:
-                module_text += f"\n{self._create_function_string(function, is_method=False)}\n"
+                function_string = self._create_function_string(
+                    function=function,
+                    is_method=False,
+                    in_reexport_module=in_reexport_module,
+                )
+                if function_string:
+                    module_text += f"\n{function_string}\n"
 
         # Create classes, class attr. & class methods
-        for class_ in self.module.classes:
+        for class_ in module.classes:
             if class_.is_public and not class_.inherits_from_exception:
-                module_text += f"\n{self._create_class_string(class_)}\n"
+                class_string = self._create_class_string(class_=class_, in_reexport_module=in_reexport_module)
+                if class_string:
+                    module_text += f"\n{class_string}\n"
 
         # Create enums & enum instances
-        for enum in self.module.enums:
+        for enum in module.enums:
             module_text += f"\n{self._create_enum_string(enum)}\n"
 
         # Create imports - We have to create them last, since we have to check all used types in this module first
         module_header += self._create_imports_string()
 
-        return docstring + module_header + module_text
+        return f"{docstring}{module_header}{module_text}", package_info
 
     def _create_imports_string(self) -> str:
         if not self.module_imports:
             return ""
 
         import_strings = []
 
@@ -235,16 +178,20 @@
 
         # We have to sort for the snapshot tests
         import_strings.sort()
 
         import_string = "\n".join(import_strings)
         return f"\n{import_string}\n"
 
-    def _create_class_string(self, class_: Class, class_indentation: str = "") -> str:
-        inner_indentations = class_indentation + "\t"
+    def _create_class_string(self, class_: Class, class_indentation: str = "", in_reexport_module: bool = False) -> str:
+        if not in_reexport_module and self._has_node_shorter_reexport(node=class_):
+            return ""
+
+        # Set indentation
+        inner_indentations = class_indentation + INDENTATION
 
         # Constructor parameter
         if class_.is_abstract:
             # Abstract classes have no constructor
             constructor_info = ""
         else:
             constructor = class_.constructor
@@ -334,24 +281,29 @@
         )
 
         # Attributes
         class_text = self._create_class_attribute_string(class_.attributes, inner_indentations)
 
         # Inner classes
         for inner_class in class_.classes:
-            class_text += f"\n{self._create_class_string(inner_class, inner_indentations)}\n"
+            class_string = self._create_class_string(
+                class_=inner_class,
+                class_indentation=inner_indentations,
+                in_reexport_module=in_reexport_module,
+            )
+            class_text += f"\n{class_string}\n"
 
         # Superclass methods, if the superclass is an internal class
         class_text += superclass_methods_text
 
         # Methods
         class_text += self._create_class_method_string(class_.methods, inner_indentations)
 
         # Docstring
-        docstring = self._create_sds_docstring(class_.docstring, "", node=class_)
+        docstring = self._create_sds_docstring(class_.docstring, class_indentation, node=class_)
 
         # If the does not have a body, we just return the docstring and signature line
         if not class_text:
             return docstring + class_signature
 
         # Close class
         class_text += f"{class_indentation}}}"
@@ -372,15 +324,15 @@
                 continue
             elif method.is_property:
                 class_property_methods.append(
                     self._create_property_function_string(method, inner_indentations),
                 )
             else:
                 class_methods.append(
-                    self._create_function_string(method, inner_indentations, is_method=True),
+                    self._create_function_string(function=method, indentations=inner_indentations, is_method=True),
                 )
 
         method_text = ""
         if class_property_methods:
             properties = "\n".join(class_property_methods)
             method_text += f"\n{properties}\n"
 
@@ -435,16 +387,25 @@
 
         attribute_text = ""
         if class_attributes:
             attribute_infos = "\n".join(class_attributes)
             attribute_text += f"\n{attribute_infos}\n"
         return attribute_text
 
-    def _create_function_string(self, function: Function, indentations: str = "", is_method: bool = False) -> str:
+    def _create_function_string(
+        self,
+        function: Function,
+        indentations: str = "",
+        is_method: bool = False,
+        in_reexport_module: bool = False,
+    ) -> str:
         """Create a function string for Safe-DS stubs."""
+        if not is_method and not in_reexport_module and self._has_node_shorter_reexport(node=function):
+            return ""
+
         # Check if static or class method
         is_static = function.is_static
         is_class_method = function.is_class_method
 
         static = ""
         if is_class_method or is_static:
             static = "static "
@@ -536,14 +497,18 @@
     def _create_result_string(self, function_results: list[Result]) -> str:
         results: list[str] = []
         for result in function_results:
             if result.type is None:  # pragma: no cover
                 continue
 
             result_type = result.type.to_dict()
+
+            if result_type["kind"] == "NamedType" and result_type["qname"] == "builtins.None":
+                return ""
+
             ret_type = self._create_type_string(result_type)
             type_string = f": {ret_type}" if ret_type else ""
             result_name = _convert_name_to_convention(result.name, self.naming_convention)
             result_name = _replace_if_safeds_keyword(result_name)
             if type_string:
                 results.append(
                     f"{result_name}{type_string}",
@@ -630,15 +595,15 @@
             camel_case_name = _replace_if_safeds_keyword(camel_case_name)
 
             # Create string and append to the list
             parameters_data.append(
                 f"{name_annotation}{camel_case_name}{type_string}{param_value}",
             )
 
-        inner_indentations = indentations + "\t"
+        inner_indentations = indentations + INDENTATION
         if parameters_data:
             inner_param_data = f",\n{inner_indentations}".join(parameters_data)
             return f"\n{inner_indentations}{inner_param_data}\n{indentations}"
         return ""
 
     def _create_enum_string(self, enum_data: Enum) -> str:
         # Docstring
@@ -661,15 +626,15 @@
                 annotation = ""
                 if camel_case_name != name:
                     annotation = f"{_create_name_annotation(name)} "
 
                 # Check if the name is a Safe-DS keyword and escape it
                 camel_case_name = _replace_if_safeds_keyword(camel_case_name)
 
-                enum_text += f"\t{annotation}{camel_case_name}\n"
+                enum_text += f"{INDENTATION}{annotation}{camel_case_name}\n"
             return f"{enum_signature} {{{enum_text}}}"
 
         return enum_signature
 
     def _create_type_string(self, type_data: dict | None) -> str:
         """Create a SafeDS stubs type string."""
         if type_data is None:
@@ -689,91 +654,130 @@
                 case "float":
                     return "Float"
                 case "None":
                     return none_type_name
                 case _:
                     self._add_to_imports(type_data["qname"])
 
-                    # inner classes that are private should not be used as types, therefore we add a todo
+                    # inner classes that are private should not be used as types, therefore we add a TOD0
                     if name[0] == "_" and type_data["qname"] not in self.module_imports:
                         self._current_todo_msgs.add("internal class as type")
 
                     return name
         elif kind == "FinalType":
             return self._create_type_string(type_data["type"])
         elif kind == "CallableType":
-            name_generator = _callable_type_name_generator()
-
             params = [
-                f"{next(name_generator)}: {self._create_type_string(parameter_type)}"
-                for parameter_type in type_data["parameter_types"]
+                (
+                    f"{_convert_name_to_convention('param_' + str(i + 1), self.naming_convention)}: "
+                    f"{self._create_type_string(parameter_type)}"
+                )
+                for i, parameter_type in enumerate(type_data["parameter_types"])
             ]
 
             return_type = type_data["return_type"]
             if return_type["kind"] == "TupleType":
                 return_types = [
-                    f"{next(name_generator)}: {self._create_type_string(type_)}" for type_ in return_type["types"]
+                    (
+                        f"{_convert_name_to_convention('result_' + str(i+1), self.naming_convention)}: "
+                        f"{self._create_type_string(type_)}"
+                    )
+                    for i, type_ in enumerate(return_type["types"])
                 ]
                 return_type_string = f"({', '.join(return_types)})"
+            elif return_type["kind"] == "NamedType" and return_type["name"] == "None":
+                return f"({', '.join(params)}) -> ()"
             else:
-                return_type_string = f"{next(name_generator)}: {self._create_type_string(return_type)}"
+                result_name = _convert_name_to_convention("result_1", self.naming_convention)
+                return_type_string = f"{result_name}: {self._create_type_string(return_type)}"
 
             return f"({', '.join(params)}) -> {return_type_string}"
-        elif kind in {"SetType", "ListType"}:
+        elif kind in {"SetType", "ListType", "NamedSequenceType"}:
             types = [self._create_type_string(type_) for type_ in type_data["types"]]
 
             # Cut out the "Type" in the kind name
             name = kind[0:-4]
 
             if name == "Set":
                 self._current_todo_msgs.add("no set support")
+            elif name == "NamedSequence":
+                name = type_data["name"]
 
             if types:
-                if len(types) >= 2:
+                if len(types) >= 2 and name in {"Set", "List"}:
                     self._current_todo_msgs.add(name)
                 return f"{name}<{', '.join(types)}>"
             return f"{name}<Any>"
+        elif kind == "UnknownType":  # pragma: no cover
+            self._current_todo_msgs.add("unknown")
+            return "unknown"
         elif kind == "UnionType":
             # In Mypy LiteralTypes are getting seperated into unions of LiteralTypes,
             # and we have to join them for the stubs.
             literal_data = []
             other_type_data = []
+            has_named_type = False
             for type_information in type_data["types"]:
                 if type_information["kind"] == "LiteralType":
                     literal_data.append(type_information)
                 else:
                     other_type_data.append(type_information)
 
+                if type_information["kind"] in {"NamedType", "TupleType", "ListType", "SetType", "DictType"} and not (
+                    type_information["kind"] == "NamedType" and type_information["qname"] == "builtins.None"
+                ):
+                    has_named_type = True
+
             if len(literal_data) >= 2:
                 all_literals = [literal_type for literal in literal_data for literal_type in literal["literals"]]
 
                 # We overwrite the old types of the union with the joined literal types
                 type_data["types"] = other_type_data
-                type_data["types"].append({
-                    "kind": "LiteralType",
-                    "literals": all_literals,
-                })
+                type_data["types"].append(
+                    {
+                        "kind": "LiteralType",
+                        "literals": all_literals,
+                    },
+                )
+
+            if len(type_data["types"]) == 2 and literal_data:
+                # If we have a LiteralType and a None we combine them to a "Literal[..., null]"
+                has_none = (type_data["types"][0]["kind"] == "NamedType" and type_data["types"][0]["kind"]) or (
+                    type_data["types"][1]["kind"] == "NamedType" and type_data["types"][1]["kind"]
+                )
+                if has_none:
+                    _types = type_data["types"]
+                    literal_type_data = _types[0] if _types[0]["kind"] == "LiteralType" else _types[1]
+
+                    literal_type_data["literals"].append(None)
+                    return self._create_type_string(literal_type_data)
 
             # Union items have to be unique, therefore we use sets. But the types set has to be a sorted list, since
             # otherwise the snapshot tests would fail b/c element order in sets is non-deterministic.
             types = list({self._create_type_string(type_) for type_ in type_data["types"]})
             types.sort()
 
             if types:
-                if len(types) == 2 and none_type_name in types:
+                if len(types) == 2 and none_type_name in types and has_named_type:
                     # if None is at least one of the two possible types, we can remove the None and just return the
-                    # other type with a question mark
+                    # other type with a question mark. But only named types (class/enum/enum variant) support the ?
+                    # syntax for nullability in Safe-DS, therefore we handle callable types here.
                     if types[0] == none_type_name:
                         return f"{types[1]}?"
                     return f"{types[0]}?"
 
                 # If the union contains only one type, return the type instead of creating a union
                 elif len(types) == 1:
                     return types[0]
 
+                if none_type_name in types and types[-1] != none_type_name:
+                    # Make sure Nones are always at the end of Unions
+                    types.pop(types.index(none_type_name))
+                    types.append(none_type_name)
+
                 return f"union<{', '.join(types)}>"
             return ""
         elif kind == "TupleType":
             self._current_todo_msgs.add("no tuple support")
             types = [self._create_type_string(type_) for type_ in type_data["types"]]
 
             return f"Tuple<{', '.join(types)}>"
@@ -787,14 +791,16 @@
                 if isinstance(literal_type, str):
                     types.append(f'"{literal_type}"')
                 elif isinstance(literal_type, bool):
                     if literal_type:
                         types.append("true")
                     else:
                         types.append("false")
+                elif isinstance(literal_type, NoneType):
+                    types.append("null")
                 else:
                     types.append(f"{literal_type}")
             return f"literal<{', '.join(types)}>"
         elif kind == "TypeVarType":
             name = _convert_name_to_convention(type_data["name"], self.naming_convention)
             return _replace_if_safeds_keyword(name)
 
@@ -816,48 +822,192 @@
                 superclass_methods_text += self._create_internal_class_methods_string(
                     superclass_superclass,
                     inner_indentations,
                 )
 
         return superclass_methods_text
 
+    def _create_sds_docstring_description(self, description: str, indentations: str) -> str:
+        if not description:
+            return ""
+
+        full_docstring = self._create_docstring_description_part(description, indentations)
+        return f"{indentations}/**\n{indentations} * {full_docstring}{indentations} */\n"
+
+    def _create_sds_docstring(
+        self,
+        docstring: ClassDocstring | FunctionDocstring | AttributeDocstring,
+        indentations: str,
+        node: Class | Function | None = None,
+    ) -> str:
+        full_docstring = ""
+
+        # Description
+        if docstring.description:
+            full_docstring = f"{indentations} * "
+            full_docstring += self._create_docstring_description_part(docstring.description, indentations)
+
+        # Parameters
+        full_parameter_docstring = ""
+        if node is not None:
+            parameters = []
+            if isinstance(node, Class):
+                if node.constructor is not None:
+                    parameters = node.constructor.parameters
+            else:
+                parameters = node.parameters
+
+            if parameters:
+                parameter_docstrings = []
+                for parameter in parameters:
+                    param_desc = parameter.docstring.description
+                    if not param_desc:
+                        continue
+
+                    param_desc = self._create_docstring_description_part(param_desc, indentations)
+
+                    parameter_name = _convert_name_to_convention(parameter.name, self.naming_convention)
+                    parameter_docstrings.append(f"{indentations} * @param {parameter_name} {param_desc}")
+
+                full_parameter_docstring = "".join(parameter_docstrings)
+
+                if full_parameter_docstring and full_docstring:
+                    full_parameter_docstring = f"{indentations} *\n{full_parameter_docstring}"
+        full_docstring += full_parameter_docstring
+
+        # Results
+        full_result_docstring = ""
+        if isinstance(node, Function):
+            name_generator = result_name_generator()
+
+            for result_docstring in node.result_docstrings:
+                result_desc = result_docstring.description
+                if result_desc:
+                    result_desc = f"\n{indentations} * ".join(result_desc.split("\n"))
+
+                    result_name = result_docstring.name if result_docstring.name else next(name_generator)
+                    result_name = _convert_name_to_convention(result_name, self.naming_convention)
+
+                    full_result_docstring += f"{indentations} * @result {result_name} {result_desc}\n"
+
+            if full_result_docstring and full_docstring:
+                full_result_docstring = f"{indentations} *\n{full_result_docstring}"
+        full_docstring += full_result_docstring
+
+        # Example
+        example = ""
+        if not isinstance(docstring, AttributeDocstring) and docstring.example:
+            example = f"{indentations} * @example\n{indentations} * pipeline example {{\n"
+            for example_part in docstring.example.split("\n"):
+                if example_part.startswith(">>>"):
+                    example += f"{indentations} *     {example_part.replace('>>>', '//')}\n"
+                elif example_part.startswith("..."):
+                    example += f"{indentations} *     {example_part.replace('...', '//')}\n"
+            example += f"{indentations} * }}\n"
+        if full_docstring and example:
+            full_docstring += f"{indentations} *\n"
+        full_docstring += example
+
+        # Open and close the docstring
+        if full_docstring:
+            full_docstring = f"{indentations}/**\n{full_docstring}{indentations} */\n"
+
+        return full_docstring
+
     # ############################### Utilities ############################### #
 
-    def _add_to_imports(self, qname: str) -> None:
+    def _has_node_shorter_reexport(self, node: Class | Function) -> bool:
+        # Check if this node is beeing reexported from a shorter path. If it is, we create it there, not in this module
+        shortest_reexport_module_id = self.module_id
+        shortest_reexport_module: Module | None = None
+        for reexport_module in node.reexported_by:
+            if len(reexport_module.id.split("/")) < len(shortest_reexport_module_id.split("/")):
+                shortest_reexport_module_id = reexport_module.id
+                shortest_reexport_module = reexport_module
+
+        if shortest_reexport_module_id != self.module_id and shortest_reexport_module is not None:
+            # Get alias
+            alias = None
+            for qualified_import in shortest_reexport_module.qualified_imports:
+                if qualified_import.qualified_name.endswith(node.name):
+                    alias = qualified_import.alias
+
+            if alias:
+                node.name = alias
+
+            self.reexport_modules[shortest_reexport_module_id].append(node)
+            return True
+        return False
+
+    def _is_path_connected_to_class(self, path: str, class_path: str) -> bool:
+        if class_path.endswith(path):
+            return True
+
+        name = path.split("/")[-1]
+        class_name = class_path.split("/")[-1]
+        for reexport in self.api.reexport_map:
+            if reexport.endswith(name):
+                for module in self.api.reexport_map[reexport]:
+                    # Added "no cover" since I can't recreate this in the tests
+                    if (
+                        path.startswith(module.id)
+                        and class_path.startswith(module.id)
+                        and path.lstrip(module.id).lstrip("/") == name == class_name
+                    ):  # pragma: no cover
+                        return True
+
+        return False
+
+    def _add_to_imports(self, import_qname: str) -> None:
         """Check if the qname of a type is defined in the current module, if not, create an import for it.
 
         Paramters
         ---------
-        qname
+        qname:
             The qualified name of a module/class/etc.
         """
-        if qname == "":  # pragma: no cover
+        if import_qname == "":  # pragma: no cover
             raise ValueError("Type has no import source.")
 
-        qname_parts = qname.split(".")
-        if qname_parts[0] == "builtins" and len(qname_parts) == 2:
+        qname_parts = import_qname.split(".")
+        if (qname_parts[0] == "builtins" and len(qname_parts) == 2) or import_qname == "typing.Any":
             return
 
-        module_id = self.module.id.replace("/", ".")
-        if module_id not in qname:
+        module_id = self.module_id.replace("/", ".")
+        if module_id not in import_qname:
             # We need the full path for an import from the same package, but we sometimes don't get enough information,
             # therefore we have to search for the class and get its id
-            qname_path = qname.replace(".", "/")
+            import_qname_path = import_qname.replace(".", "/")
             in_package = False
-            for class_ in self.api.classes:
-                if class_.endswith(qname_path):
-                    qname = class_.replace("/", ".")
-                    qname = _convert_name_to_convention(qname, self.naming_convention)
+            qname = ""
+            for class_id in self.api.classes:
+                if self._is_path_connected_to_class(import_qname_path, class_id):
+                    qname = class_id.replace("/", ".")
+
+                    name = qname.split(".")[-1]
+                    shortest_qname, _ = _get_shortest_public_reexport(
+                        reexport_map=self.api.reexport_map,
+                        name=name,
+                        qname=qname,
+                        is_module=False,
+                    )
+
+                    if shortest_qname:
+                        qname = f"{shortest_qname}.{name}"
+
                     in_package = True
                     break
 
+            qname = qname or import_qname
+
             if not in_package:
                 self.classes_outside_package.add(qname)
 
-            self.module_imports.add(qname)
+            if qname.replace(".", "/") != self.module_id:
+                self.module_imports.add(qname)
 
     def _create_todo_msg(self, indentations: str) -> str:
         if not self._current_todo_msgs:
             return ""
 
         todo_msgs = [
             "// TODO "
@@ -871,236 +1021,45 @@
                 "multiple_inheritance": "Safe-DS does not support multiple inheritance.",
                 "variadic": "Safe-DS does not support variadic parameters.",
                 "class_method": "Safe-DS does not support class methods.",
                 "param without type": "Some parameter have no type information.",
                 "attr without type": "Attribute has no type information.",
                 "result without type": "Result type information missing.",
                 "internal class as type": "An internal class must not be used as a type in a public class.",
+                "unknown": "Unknown type - Type could not be parsed.",
             }[msg]
             for msg in self._current_todo_msgs
         ]
         todo_msgs.sort()
 
         # Empty the message list
         self._current_todo_msgs = set()
 
         return indentations + f"\n{indentations}".join(todo_msgs) + "\n"
 
     def _get_class_in_module(self, class_name: str) -> Class:
-        if f"{self.module.id}/{class_name}" in self.api.classes:
-            return self.api.classes[f"{self.module.id}/{class_name}"]
+        if f"{self.module_id}/{class_name}" in self.api.classes:
+            return self.api.classes[f"{self.module_id}/{class_name}"]
 
         # If the class is a nested class
         for class_ in self.api.classes:
-            if class_.startswith(self.module.id) and class_.endswith(class_name):
+            if class_.startswith(self.module_id) and class_.endswith(class_name):
                 return self.api.classes[class_]
 
-        raise LookupError(f"Expected finding class '{class_name}' in module '{self.module.id}'.")  # pragma: no cover
-
-    def _get_shortest_public_reexport(self) -> str:
-        module_qname = self.module.id.replace("/", ".")
-        module_name = self.module.name
-        reexports = self.api.reexport_map
-
-        def _module_name_check(name: str, string: str) -> bool:
-            return (
-                string == name
-                or (f".{name}" in string and (string.endswith(f".{name}") or f"{name}." in string))
-                or (f"{name}." in string and (string.startswith(f"{name}.") or f".{name}" in string))
-            )
-
-        keys = [reexport_key for reexport_key in reexports if _module_name_check(module_name, reexport_key)]
-
-        module_ids = set()
-        for key in keys:
-            for module in reexports[key]:
-                added_module_id = False
-
-                for qualified_import in module.qualified_imports:
-                    if _module_name_check(module_name, qualified_import.qualified_name):
-                        module_ids.add(module.id)
-                        added_module_id = True
-                        break
-
-                if added_module_id:
-                    continue
-
-                for wildcard_import in module.wildcard_imports:
-                    if _module_name_check(module_name, wildcard_import.module_name):
-                        module_ids.add(module.id)
-                        break
-
-        # Adjust all ids
-        fixed_module_ids_parts = [module_id.split("/") for module_id in module_ids]
-
-        shortest_id = None
-        for fixed_module_id_parts in fixed_module_ids_parts:
-            if shortest_id is None or len(fixed_module_id_parts) < len(shortest_id):
-                shortest_id = fixed_module_id_parts
-
-                if len(shortest_id) == 1:
-                    break
-
-        if shortest_id is None:
-            return module_qname
-        return ".".join(shortest_id)
+        raise LookupError(f"Expected finding class '{class_name}' in module '{self.module_id}'.")  # pragma: no cover
 
     @staticmethod
-    def _create_sds_docstring_description(description: str, indentations: str) -> str:
-        if not description:
-            return ""
-
+    def _create_docstring_description_part(description: str, indentations: str) -> str:
         description = description.rstrip("\n")
         description = description.lstrip("\n")
-        description = description.replace("\n", f"\n{indentations} * ")
-        return f"{indentations}/**\n{indentations} * {description}\n{indentations} */\n"
+        splitted_docstring = description.split("\n")
 
-    def _create_sds_docstring(
-        self,
-        docstring: ClassDocstring | FunctionDocstring | AttributeDocstring,
-        indentations: str,
-        node: Class | Function | None = None,
-    ) -> str:
         full_docstring = ""
-
-        # Description
-        if docstring.description:
-            docstring_description = docstring.description.rstrip("\n")
-            docstring_description = docstring_description.lstrip("\n")
-            docstring_description = docstring_description.replace("\n", f"\n{indentations} * ")
-            full_docstring += f"{indentations} * {docstring_description}\n"
-
-        # Parameters
-        full_parameter_docstring = ""
-        if node is not None:
-            parameters = []
-            if isinstance(node, Class):
-                if node.constructor is not None:
-                    parameters = node.constructor.parameters
+        for i, docstring_part in enumerate(splitted_docstring):
+            if i == 0:
+                full_docstring = f"{docstring_part}"
+            elif docstring_part:
+                full_docstring += f"\n{indentations} * {docstring_part}"
             else:
-                parameters = node.parameters
-
-            if parameters:
-                parameter_docstrings = []
-                for parameter in parameters:
-                    param_desc = parameter.docstring.description
-                    if not param_desc:
-                        continue
-
-                    param_desc = f"\n{indentations} * ".join(param_desc.split("\n"))
-
-                    parameter_name = _convert_name_to_convention(parameter.name, self.naming_convention)
-                    parameter_docstrings.append(f"{indentations} * @param {parameter_name} {param_desc}\n")
-
-                full_parameter_docstring = "".join(parameter_docstrings)
-
-                if full_parameter_docstring and full_docstring:
-                    full_parameter_docstring = f"{indentations} *\n{full_parameter_docstring}"
-        full_docstring += full_parameter_docstring
-
-        # Results
-        full_result_docstring = ""
-        if isinstance(node, Function):
-            result_docstrings = []
-            for result in node.results:
-                result_desc = result.docstring.description
-                if not result_desc:
-                    continue
-
-                result_desc = f"\n{indentations} * ".join(result_desc.split("\n"))
-
-                result_name = _convert_name_to_convention(result.name, self.naming_convention)
-                result_docstrings.append(f"{indentations} * @result {result_name} {result_desc}\n")
-
-            full_result_docstring = "".join(result_docstrings)
-
-            if full_result_docstring and full_docstring:
-                full_result_docstring = f"{indentations} *\n{full_result_docstring}"
-        full_docstring += full_result_docstring
-
-        # Open and close the docstring
-        if full_docstring:
-            full_docstring = f"{indentations}/**\n{full_docstring}{indentations} */\n"
-
-        return full_docstring
-
-
-def _callable_type_name_generator() -> Generator:
-    """Generate a name for callable type parameters starting from 'a' until 'zz'."""
-    while True:
-        for x in range(1, 1000):
-            yield f"param{x}"
-
-
-def _create_name_annotation(name: str) -> str:
-    return f'@PythonName("{name}")'
-
-
-def _replace_if_safeds_keyword(keyword: str) -> str:
-    if keyword in {
-        "as",
-        "from",
-        "import",
-        "literal",
-        "union",
-        "where",
-        "yield",
-        "false",
-        "null",
-        "true",
-        "annotation",
-        "attr",
-        "class",
-        "enum",
-        "fun",
-        "package",
-        "pipeline",
-        "schema",
-        "segment",
-        "val",
-        "const",
-        "in",
-        "internal",
-        "out",
-        "private",
-        "static",
-        "and",
-        "not",
-        "or",
-        "sub",
-        "super",
-        "_",
-    }:
-        return f"`{keyword}`"
-    return keyword
-
-
-def is_internal(name: str) -> bool:
-    return name.startswith("_")
-
-
-def _convert_name_to_convention(
-    name: str,
-    naming_convention: NamingConvention,
-    is_class_name: bool = False,
-) -> str:
-    if name == "_" or naming_convention == NamingConvention.PYTHON:
-        return name
-
-    # Count underscores in front and behind the name
-    underscore_count_start = len(name) - len(name.lstrip("_"))
-    underscore_count_end = len(name) - len(name.rstrip("_"))
-
-    if underscore_count_end == 0:
-        cleaned_name = name[underscore_count_start:]
-    else:
-        cleaned_name = name[underscore_count_start:-underscore_count_end]
-
-    # Remove underscores and join in camelCase
-    name_parts = cleaned_name.split("_")
-
-    # UpperCamelCase for class names
-    if is_class_name:
-        return "".join(part[0].upper() + part[1:] for part in name_parts if part)
+                full_docstring += f"\n{indentations} *"
 
-    # Normal camelCase for everything else
-    return name_parts[0] + "".join(part[0].upper() + part[1:] for part in name_parts[1:] if part)
+        return full_docstring + "\n"
```

### Comparing `safe_ds_stubgen-0.2.0/PKG-INFO` & `safe_ds_stubgen-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: safe-ds-stubgen
-Version: 0.2.0
+Version: 0.3.0
 Summary: Generation of Safe-DS stubs for Python libraries.
 Home-page: https://github.com/Safe-DS/Stub-Generator
 License: MIT
 Keywords: data-science,machine-learning,dsl
 Author: Lars Reimann
 Author-email: mail@larsreimann.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: docstring-parser (>=0.15,<0.16)
+Requires-Dist: griffe (>=0.42,<0.45)
 Requires-Dist: mypy (>=1.6.1,<2.0.0)
 Project-URL: Documentation, https://stubgen.readthedocs.io
 Project-URL: Repository, https://github.com/Safe-DS/Stub-Generator
 Description-Content-Type: text/markdown
 
 # Stub Generator
 
 [![PyPI](https://img.shields.io/pypi/v/safe-ds-stubgen)](https://pypi.org/project/safe-ds-stubgen)
 [![Main](https://github.com/Safe-DS/Stub-Generator/actions/workflows/main.yml/badge.svg)](https://github.com/Safe-DS/Stub-Generator/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/Safe-DS/Stub-Generator/branch/main/graph/badge.svg?token=UyCUY59HKM)](https://codecov.io/gh/Safe-DS/Stub-Generator)
 [![Documentation Status](https://readthedocs.org/projects/safe-ds-stub-generator/badge/?version=stable)](https://stubgen.safeds.com)
 
-Automated generation of [Safe-DS stubs](https://dsl.safeds.com/en/stable/language/stub-language/) for Python libraries.
+Automated generation of [Safe-DS stubs](https://dsl.safeds.com/en/stable/stub-language/) for Python libraries.
 
 ## Installation
 
 Get the latest version from [PyPI](https://pypi.org/project/safe-ds-stubgen):
 
 ```shell
 pip install safe-ds-stubgen
@@ -45,15 +45,15 @@
 Analyze Python code.
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         show info messages
   -p PACKAGE, --package PACKAGE
                         The name of the package.
-  -s SRC, --src SRC     Directory containing the Python code of the package. If this is omitted, we try to locate the package with the given name in the current Python interpreter.
+  -s SRC, --src SRC     Source directory containing the Python code of the package.
   -o OUT, --out OUT     Output directory.
   --docstyle {PLAINTEXT,EPYDOC,GOOGLE,NUMPYDOC,REST}
                         The docstring style.
   -tr, --testrun        Set this flag if files in /test or /tests directories should be included.
   -nc, --naming_convert
                         Set this flag if the name identifiers should be converted to Safe-DS standard (UpperCamelCase for classes and camelCase for everything else).
 ```
```

