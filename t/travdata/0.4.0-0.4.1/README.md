# Comparing `tmp/travdata-0.4.0.tar.gz` & `tmp/travdata-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "travdata-0.4.0.tar", max compression
+gzip compressed data, was "travdata-0.4.1.tar", max compression
```

## Comparing `travdata-0.4.0.tar` & `travdata-0.4.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1095 2024-04-27 06:59:32.835359 travdata-0.4.0/LICENSE
--rw-r--r--   0        0        0     6682 2024-04-27 06:59:32.835359 travdata-0.4.0/README.rst
--rw-r--r--   0        0        0     1501 2024-04-27 06:59:32.847360 travdata-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       85 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/__init__.py
--rwxr-xr-x   0        0        0     1762 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cli.py
--rw-r--r--   0        0        0      247 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cliutil.py
--rw-r--r--   0        0        0        0 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cmds/__init__.py
--rw-r--r--   0        0        0     1995 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cmds/csvtoyaml.py
--rw-r--r--   0        0        0     6304 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cmds/extractcsvtables.py
--rw-r--r--   0        0        0     2617 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cmds/licenses.py
--rw-r--r--   0        0        0      693 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cmds/listbooks.py
--rw-r--r--   0        0        0    22253 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cmds/tradetable.py
--rw-r--r--   0        0        0      521 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/commontext.py
--rw-r--r--   0        0        0    11835 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/config/__init__.py
--rw-r--r--   0        0        0      152 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/config/cfgerror.py
--rw-r--r--   0        0        0     4223 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/config/cfgextract.py
--rw-r--r--   0        0        0      224 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/config/yamlreg.py
--rw-r--r--   0        0        0     1495 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/csvutil.py
--rw-r--r--   0        0        0     1046 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/dataclassutil.py
--rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/datatypes/__init__.py
--rw-r--r--   0        0        0     3914 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/datatypes/basic.py
--rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/datatypes/core/__init__.py
--rw-r--r--   0        0        0      685 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/datatypes/core/trade.py
--rw-r--r--   0        0        0     3156 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/datatypes/core/worldcreation.py
--rw-r--r--   0        0        0      483 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/datatypes/yamlcodec.py
--rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/extraction/__init__.py
--rw-r--r--   0        0        0     5188 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/extraction/bookextract.py
--rw-r--r--   0        0        0     2357 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/extraction/parseutil.py
--rw-r--r--   0        0        0     8545 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/extraction/tableextract.py
--rw-r--r--   0        0        0     4691 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/extraction/tabulautil.py
--rw-r--r--   0        0        0    11853 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/filesio.py
--rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/gui/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/gui/extraction/__init__.py
--rw-r--r--   0        0        0    19093 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/gui/extraction/cfgwin.py
--rw-r--r--   0        0        0     4948 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/gui/extraction/runnerwin.py
--rw-r--r--   0        0        0      872 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/gui/gui.py
--rw-r--r--   0        0        0     1829 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/gui/qtutil.py
--rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/py.typed
--rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/tableconverters/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/tableconverters/core/__init__.py
--rw-r--r--   0        0        0      550 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/tableconverters/core/registry.py
--rw-r--r--   0        0        0     2079 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/tableconverters/core/trade.py
--rw-r--r--   0        0        0     3802 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/tableconverters/core/worldcreation.py
--rw-r--r--   0        0        0     1093 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/tableconverters/registry.py
--rw-r--r--   0        0        0      171 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/travdatarelease.py
--rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/travellermap/__init__.py
--rw-r--r--   0        0        0     3686 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/travellermap/apiurls.py
--rw-r--r--   0        0        0     2397 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/travellermap/sectorparse.py
--rw-r--r--   0        0        0     4879 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/travellermap/world.py
--rw-r--r--   0        0        0     6679 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/yamlutil.py
--rw-r--r--   0        0        0     7647 1970-01-01 00:00:00.000000 travdata-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-04 07:31:05.273587 travdata-0.4.1/LICENSE
+-rw-r--r--   0        0        0     6682 2024-05-04 07:31:05.273587 travdata-0.4.1/README.rst
+-rw-r--r--   0        0        0     1529 2024-05-04 07:31:05.285587 travdata-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/cli/__init__.py
+-rwxr-xr-x   0        0        0     1762 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/cli/cli.py
+-rw-r--r--   0        0        0      247 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/cli/cliutil.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/cli/cmds/__init__.py
+-rw-r--r--   0        0        0     2014 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/cli/cmds/csvtoyaml.py
+-rw-r--r--   0        0        0     6124 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/cli/cmds/extractcsvtables.py
+-rw-r--r--   0        0        0     2617 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/cli/cmds/licenses.py
+-rw-r--r--   0        0        0      693 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/cli/cmds/listbooks.py
+-rw-r--r--   0        0        0    22253 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/cli/cmds/tradetable.py
+-rw-r--r--   0        0        0      521 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/commontext.py
+-rw-r--r--   0        0        0    11954 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/config/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/config/cfgerror.py
+-rw-r--r--   0        0        0     4223 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/config/cfgextract.py
+-rw-r--r--   0        0        0      224 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/config/yamlreg.py
+-rw-r--r--   0        0        0     1523 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/csvutil.py
+-rw-r--r--   0        0        0     1046 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/dataclassutil.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/datatypes/__init__.py
+-rw-r--r--   0        0        0     3914 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/datatypes/basic.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/datatypes/core/__init__.py
+-rw-r--r--   0        0        0      685 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/datatypes/core/trade.py
+-rw-r--r--   0        0        0     3156 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/datatypes/core/worldcreation.py
+-rw-r--r--   0        0        0      483 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/datatypes/yamlcodec.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/extraction/__init__.py
+-rw-r--r--   0        0        0     8249 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/extraction/bookextract.py
+-rw-r--r--   0        0        0     2357 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/extraction/parseutil.py
+-rw-r--r--   0        0        0     8631 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/extraction/tableextract.py
+-rw-r--r--   0        0        0     4807 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/extraction/tabulautil.py
+-rw-r--r--   0        0        0    15088 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/filesio.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/gui/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/gui/extraction/__init__.py
+-rw-r--r--   0        0        0    19595 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/gui/extraction/cfgwin.py
+-rw-r--r--   0        0        0     4948 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/gui/extraction/runnerwin.py
+-rw-r--r--   0        0        0      872 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/gui/gui.py
+-rw-r--r--   0        0        0     1829 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/gui/qtutil.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/py.typed
+-rw-r--r--   0        0        0        0 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/tableconverters/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/tableconverters/core/__init__.py
+-rw-r--r--   0        0        0      550 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/tableconverters/core/registry.py
+-rw-r--r--   0        0        0     2079 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/tableconverters/core/trade.py
+-rw-r--r--   0        0        0     3802 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/tableconverters/core/worldcreation.py
+-rw-r--r--   0        0        0     1093 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/tableconverters/registry.py
+-rw-r--r--   0        0        0      171 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/travdatarelease.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/travellermap/__init__.py
+-rw-r--r--   0        0        0     3686 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/travellermap/apiurls.py
+-rw-r--r--   0        0        0     2397 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/travellermap/sectorparse.py
+-rw-r--r--   0        0        0     4879 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/travellermap/world.py
+-rw-r--r--   0        0        0     6679 2024-05-04 07:31:05.285587 travdata-0.4.1/src/travdata/yamlutil.py
+-rw-r--r--   0        0        0     7647 1970-01-01 00:00:00.000000 travdata-0.4.1/PKG-INFO
```

### Comparing `travdata-0.4.0/LICENSE` & `travdata-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/README.rst` & `travdata-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/pyproject.toml` & `travdata-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "travdata"
-version = "0.4.0"
+version = "0.4.1"
 description = "Data utility code for Mongoose Traveller TTRPG."
 authors = ["John Beisley <johnbeisleyuk@gmail.com>"]
 keywords = ["traveller", "ttrpg"]
 license = "MIT"
 readme = "README.rst"  # rebuilt from README.adoc
 repository = "https://github.com/huin/travdata"
 packages = [
@@ -22,14 +22,15 @@
 black = "^24.3.0"
 mypy = "^1.9.0"
 pylint = "^3.1.0"
 pytest = "^8.0.2"
 testfixtures = "^8.0.0"
 trove-classifiers = "^2024.3.3"
 types-pyinstaller = "^6.5.0.20240311"
+pytest-subtests = "^0.12.1"
 
 [tool.poetry.group.dev.dependencies.pyinstaller]
 version = "^6.5.0"
 python = ">=3.11,<3.13"
 
 [tool.black]
 line-length = 100
```

### Comparing `travdata-0.4.0/src/travdata/cli/cli.py` & `travdata-0.4.1/src/travdata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/cli/cmds/csvtoyaml.py` & `travdata-0.4.1/src/travdata/cli/cmds/csvtoyaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
 
 def run(args: argparse.Namespace) -> None:
     """CLI entry point."""
     registry.load_all_converters()
 
     with (
-        filesio.DirReader.open(args.input_dir) as csv_reader,
-        filesio.DirWriter.create(args.output_dir) as yaml_writer,
+        filesio.DirReader.new_reader(args.input_dir) as csv_reader,
+        filesio.DirReadWriter.new_read_writer(args.output_dir) as yaml_writer,
     ):
         for conv_key, conv_fn in registry.CONVERTERS.converters.items():
             in_group_dir = pathlib.PurePath(conv_key.group_name)
             out_group_dir = pathlib.PurePath(conv_key.group_name)
             with (
                 csvutil.open_by_reader(
                     csv_reader,
```

### Comparing `travdata-0.4.0/src/travdata/cli/cmds/extractcsvtables.py` & `travdata-0.4.1/src/travdata/cli/cmds/extractcsvtables.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import pathlib
 import sys
 import textwrap
 from typing import Callable, Iterator
 
 from progress import bar as progress  # type: ignore[import-untyped]
 from travdata import config, filesio
-from travdata.cli import cliutil
 from travdata.extraction import bookextract, tabulautil
 
 
 def add_subparser(subparsers) -> None:
     """Adds a subcommand parser to ``subparsers``."""
     argparser: argparse.ArgumentParser = subparsers.add_parser(
         "extractcsvtables",
@@ -163,23 +162,21 @@
     try:
         yield on_progress
     finally:
         if progress_bar is not None:
             progress_bar.finish()
 
 
-def _create_writer(
+def _create_read_writer(
     args: argparse.Namespace,
-) -> contextlib.AbstractContextManager[filesio.Writer]:
+) -> contextlib.AbstractContextManager[filesio.ReadWriter]:
     output: pathlib.Path = args.output
     output_type: filesio.IOType = args.output_type
     output_type = output_type.resolve_auto(output)
-    if output_type == filesio.IOType.ZIP and args.overwrite_existing:
-        raise cliutil.UsageError("--overwrite-existing is incompatible with writing to a ZIP file")
-    return output_type.create(output)
+    return output_type.new_read_writer(output)
 
 
 def run(args: argparse.Namespace) -> int:
     """CLI entry point."""
 
     with_tags = frozenset(args.with_tag)
     without_tags = frozenset(args.without_tag)
@@ -189,15 +186,15 @@
             f"Tags have been specified for both inclusion and exclusion: {fmt_inter}.",
             file=sys.stderr,
         )
         return 1
 
     ext_cfg = bookextract.ExtractionConfig(
         cfg_reader_ctx=config.config_reader(args),
-        out_writer_ctx=_create_writer(args),
+        out_writer_ctx=_create_read_writer(args),
         input_pdf=args.input_pdf,
         book_id=args.book_name,
         overwrite_existing=args.overwrite_existing,
         with_tags=with_tags,
         without_tags=without_tags,
     )
```

### Comparing `travdata-0.4.0/src/travdata/cli/cmds/licenses.py` & `travdata-0.4.1/src/travdata/cli/cmds/licenses.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/cli/cmds/listbooks.py` & `travdata-0.4.1/src/travdata/cli/cmds/listbooks.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/cli/cmds/tradetable.py` & `travdata-0.4.1/src/travdata/cli/cmds/tradetable.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/commontext.py` & `travdata-0.4.1/src/travdata/commontext.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/config/__init__.py` & `travdata-0.4.1/src/travdata/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 class Book:
     """Top level information about a book."""
 
     id_: str
     name: str
     default_filename: str
     tags: set[str] = dataclasses.field(default_factory=set)
+    page_offset: int = 1
     _group: Optional[Group] = None
 
     def load_group(self, cfg_reader: filesio.Reader) -> Group:
         """Loads and returns the top-level group in the `Book`."""
         if self._group is None:
             self._group = load_book(cfg_reader, self.id_, self.tags)
         return self._group
@@ -167,14 +168,15 @@
 @dataclasses.dataclass
 @yamlreg.YAML.register_class
 class _YamlBook(yamlutil.YamlMappingMixin):
     yaml_tag: ClassVar = "!Book"
     name: str
     default_filename: str
     tags: set[str] = dataclasses.field(default_factory=set, metadata=yamlutil.SET_METADATA)
+    page_offset: int = 1
 
     @classmethod
     def yaml_create_empty(cls) -> Self:
         return cls(name="", default_filename="")
 
     def prepare(
         self,
@@ -182,20 +184,21 @@
     ) -> Book:
         """Creates a ``Book`` from self.
 
         :param cfg_reader: Reader for the configuration files.
         :param book_id: ID of the book within the parent _YamlConfig.
         :return: Prepared ``Book``.
         """
-        tags = self.tags | {f"book/{self.name}"}
+        tags = self.tags | {f"book/{book_id}"}
         return Book(
             id_=book_id,
             name=self.name,
             default_filename=self.default_filename,
             tags=tags,
+            page_offset=self.page_offset,
         )
 
 
 @dataclasses.dataclass
 @yamlreg.YAML.register_class
 class _YamlConfig(yamlutil.YamlMappingMixin):
     yaml_tag: ClassVar = "!Config"
@@ -269,15 +272,15 @@
     try:
         with cfg_reader.open_read(_VERSION_FILE) as f:
             return f.read().rstrip()
     except filesio.NotFoundError:
         return None
 
 
-def save_config_version(cfg_writer: filesio.Writer, version: str) -> None:
+def save_config_version(cfg_writer: filesio.ReadWriter, version: str) -> None:
     """Writes the configuration version to the ``cfg_writer``."""
     with cfg_writer.open_write(_VERSION_FILE) as f:
         f.write(version)
 
 
 def load_config(cfg_reader: filesio.Reader) -> Config:
     """Loads the configuration from the ``cfg_reader``."""
@@ -349,31 +352,31 @@
 
     :param args: Parsed arguments. This must have been generated from a parser
     that included the argument added by ``add_config_flag``.
     :return: Context manager for a configuration reader.
     """
     path: pathlib.Path = args.config
     output_type = filesio.IOType.AUTO.resolve_auto(path)
-    return output_type.open(path)
+    return output_type.new_reader(path)
 
 
 def create_config_zip(
     version: str,
     config_dir: pathlib.Path,
     config_zip: pathlib.Path,
 ) -> None:
     """Generates a config ZIP file.
 
     :param version: Version to write into the configuration.
     :param config_dir: Config directory to copy from.
     :param config_zip: Config ZIP file to create.
     """
     with (
-        filesio.DirReader.open(config_dir) as cfg_reader,
-        filesio.ZipWriter.create(config_zip) as cfg_writer,
+        filesio.DirReader.new_reader(config_dir) as cfg_reader,
+        filesio.ZipReadWriter.new_read_writer(config_zip) as cfg_writer,
     ):
         save_config_version(cfg_writer, version)
 
         for path in sorted(cfg_reader.iter_files()):
             with (
                 cfg_reader.open_read(path) as fr,
                 cfg_writer.open_write(path) as fw,
```

### Comparing `travdata-0.4.0/src/travdata/config/cfgextract.py` & `travdata-0.4.1/src/travdata/config/cfgextract.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/csvutil.py` & `travdata-0.4.1/src/travdata/csvutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,25 +29,25 @@
 
     :param path: Path to the file to read.
     :return: Opened file.
     """
     return path.open(mode="rt", encoding="utf-8", newline="")
 
 
-def open_by_writer(
-    writer: filesio.Writer,
+def open_by_read_writer(
+    read_writer: filesio.ReadWriter,
     path: pathlib.PurePath,
 ) -> contextlib.AbstractContextManager[IO[str]]:
     """Opens a file in a manner suitable for writing CSV data into.
 
-    :param writer: Writer to use.
+    :param read_writer: ReadWriter to use.
     :param path: Path to the file to write.
     :return: Opened file.
     """
-    return writer.open_write(path, newline="")
+    return read_writer.open_write(path, newline="")
 
 
 def open_write(
     path: pathlib.Path,
 ) -> contextlib.AbstractContextManager[IO[str]]:
     """Opens a file in a manner suitable for writing CSV data into.
```

### Comparing `travdata-0.4.0/src/travdata/dataclassutil.py` & `travdata-0.4.1/src/travdata/dataclassutil.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/datatypes/basic.py` & `travdata-0.4.1/src/travdata/datatypes/basic.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/datatypes/core/trade.py` & `travdata-0.4.1/src/travdata/datatypes/core/trade.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/datatypes/core/worldcreation.py` & `travdata-0.4.1/src/travdata/datatypes/core/worldcreation.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/extraction/parseutil.py` & `travdata-0.4.1/src/travdata/extraction/parseutil.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/extraction/tableextract.py` & `travdata-0.4.1/src/travdata/extraction/tableextract.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,63 +22,62 @@
     """
 
     def read_pdf_with_template(
         self,
         *,
         pdf_path: pathlib.Path,
         template_file: IO[str],
-    ) -> list[tabulautil.TabulaTable]:
+    ) -> tuple[set[int], list[tabulautil.TabulaTable]]:
         """Reads tables from a PDF file, using the named template file.
 
         :param pdf_path: Path to the PDF file.
         :param template_file: File-like reader for the Tabula template JSON
         file.
-        :return: List of extracted tables.
+        :return: Set of page numbers and list of extracted tables.
         """
         raise NotImplementedError
 
 
 class ConfigurationError(Exception):
     """Exception indication error in the given configuration."""
 
 
 def extract_table(
     cfg_reader: filesio.Reader,
     table: config.Table,
     pdf_path: pathlib.Path,
     table_reader: TableReader,
-) -> Iterator[list[str]]:
+) -> tuple[set[int], Iterator[list[str]]]:
     """Extracts a table from the PDF.
 
     :cfg_reader: Configuration file reader.
     :param table: Configuration of the table to extract. ``table.extraction``
     must not be None.
     :param pdf_path: Path to the PDF to extract from.
     :param tabula_reader: Used to read the table from the PDF.
-    :returns: Iterator over rows from the table.
+    :returns: Set of page numbers and iterator over rows from the table.
     :raises ValueError: ``table.extraction`` is None.
     """
     if table.extraction is None:
         raise ValueError(
             f"extract_table called with table with `None` extraction: {table=}",
         )
 
     with cfg_reader.open_read(table.tabula_template_path) as tmpl_file:
-        tabula_rows: Iterator[tabulautil.TabulaRow] = tabulautil.table_rows_concat(
-            table_reader.read_pdf_with_template(
-                pdf_path=pdf_path,
-                template_file=tmpl_file,
-            )
+        pages, tables = table_reader.read_pdf_with_template(
+            pdf_path=pdf_path,
+            template_file=tmpl_file,
         )
+        tabula_rows: Iterator[tabulautil.TabulaRow] = tabulautil.table_rows_concat(tables)
         rows = tabulautil.table_rows_text(tabula_rows)
 
         for transform_cfg in table.extraction.transforms:
             rows = _transform(transform_cfg, rows)
 
-        return _clean_rows(rows)
+        return pages, _clean_rows(rows)
 
 
 _Row: TypeAlias = list[str]
 _RowGroup: TypeAlias = list[_Row]
 
 
 def _transform(cfg: cfgextract.TableTransform, rows: Iterable[_Row]) -> Iterator[_Row]:
```

### Comparing `travdata-0.4.0/src/travdata/extraction/tabulautil.py` & `travdata-0.4.1/src/travdata/extraction/tabulautil.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,29 +89,32 @@
             self._needs_shutdown = False
 
     def read_pdf_with_template(
         self,
         *,
         pdf_path: pathlib.Path,
         template_file: IO[str],
-    ) -> list[TabulaTable]:
+    ) -> tuple[set[int], list[TabulaTable]]:
         """Reads table(s) from a PDF, based on the Tabula template.
 
         :param pdf_path: Path to PDF to read from.
         :param template_file: File-like reader for the Tabula template JSON
         file.
-        :return: Tables read from the PDF.
+        :return: Page numbers and tables read from the PDF.
         """
         self._needs_shutdown = not self._force_subprocess
 
         result: list[TabulaTable] = []
         template = cast(list[_TemplateEntry], json.load(template_file))
 
+        pages: set[int] = set()
+
         for entry in template:
             method = entry["extraction_method"]
+            pages.add(int(entry["page"]))
             result.extend(
                 cast(
                     list[TabulaTable],
                     self._read_pdf(
                         input_path=pdf_path,
                         pages=[entry["page"]],
                         multiple_tables=True,
@@ -120,15 +123,15 @@
                         stream=method == "stream",
                         guess=method == "guess",
                         lattice=method == "lattice",
                     ),
                 )
             )
 
-        return result
+        return pages, result
 
     def _read_pdf(self, **kwargs) -> list[TabulaTable]:
         return cast(
             list[TabulaTable],
             tabula.read_pdf(  # pyright: ignore[reportPrivateImportUsage]
                 java_options=["-Djava.awt.headless=true"], output_format="json", **kwargs
             ),
```

### Comparing `travdata-0.4.0/src/travdata/filesio.py` & `travdata-0.4.1/src/travdata/filesio.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 # pylint: disable=too-few-public-methods
 
 import contextlib
 import enum
 import io
 import os
 import pathlib
-from typing import IO, Iterator, Protocol, Self
+import shutil
+import tempfile
+from typing import IO, Iterator, Optional, Protocol, Self
 import zipfile
 
 
 _ENCODING = "utf-8"
 _NEWLINE = "\n"
 
 
@@ -57,49 +59,49 @@
             case IOType.DIR:
                 return 2
             case IOType.ZIP:
                 return 3
             case _:
                 raise ValueError(self)
 
-    def open(
+    def new_reader(
         self,
         path: pathlib.Path,
     ) -> contextlib.AbstractContextManager["Reader"]:
         """Creates a context manager for a ``Reader``.
 
         :param path: Path for the reader to read.
         :raises Error: If ``self`` is an unknown or unresolved value like
         ``AUTO``.
         :return: Context manager for a ``Reader``.
         """
         match self:
             case IOType.DIR:
-                return DirReader.open(path)
+                return DirReader.new_reader(path)
             case IOType.ZIP:
-                return ZipReader.open(path)
+                return ZipReader.new_reader(path)
             case _:
                 raise Error(f"cannot open output type {self} with a path")
 
-    def create(
+    def new_read_writer(
         self,
         path: pathlib.Path,
-    ) -> contextlib.AbstractContextManager["Writer"]:
-        """Creates a context manager for a ``Writer``.
+    ) -> contextlib.AbstractContextManager["ReadWriter"]:
+        """Creates a context manager for a ``ReadWriter``.
 
         :param path: Path for the writer to create.
         :raises Error: If ``self`` is an unknown or unresolved value like
         ``AUTO``.
-        :return: Context manager for a ``Writer``.
+        :return: Context manager for a ``ReadWriter``.
         """
         match self:
             case IOType.DIR:
-                return DirWriter.create(path)
+                return DirReadWriter.new_read_writer(path)
             case IOType.ZIP:
-                return ZipWriter.create(path)
+                return ZipReadWriter.new_read_writer(path)
             case _:
                 raise Error(f"cannot open output type {self} with a path")
 
     def resolve_auto(self, path: pathlib.Path) -> "IOType":
         """Returns a concrete IOType for the given filesystem ``path``.
 
         :param path: Filesystem path to aid resolution.
@@ -139,56 +141,58 @@
     def iter_files(self) -> Iterator[pathlib.PurePath]:
         """Iterates over all files that the reader has.
 
         :yield: Paths of individual files. The order is undefined.
         """
         ...
 
+    def exists(
+        self,
+        path: pathlib.PurePath,
+    ) -> bool:
+        """Return ``True`` if the file exists.
+
+        :param path: Path to the file.
+        :return: ``True`` if the file exists, otherwise ``False``.
+        """
+        ...
 
-class Writer(Protocol):
-    """Protocol for writing files to the collection."""
+
+class ReadWriter(Reader, Protocol):
+    """Protocol for reading and writing files in the collection."""
 
     def open_write(
         self,
         path: pathlib.PurePath,
         newline: str = _NEWLINE,
     ) -> contextlib.AbstractContextManager[IO[str]]:
         """Open a text file for writing.
 
         :param path: Path of the file to write.
         :param newline: Newline sequence to use.
         :return: Context-managed writable file-like object.
         """
         ...
 
-    def exists(
-        self,
-        path: pathlib.PurePath,
-    ) -> bool:
-        """Return ``True`` if the file exists.
-
-        :param path: Path to the file.
-        :return: ``True`` if the file exists, otherwise ``False``.
-        """
-        ...
-
 
-class DirReader(Reader):
-    """Reads files from a local filesystem directory."""
+class DirReader:
+    """Reads files in a local filesystem directory."""
 
     _dir_path: pathlib.Path
+    _created_dirs: set[pathlib.Path]
 
     def __init__(self, dir_path: pathlib.Path) -> None:
-        """Initialise the DirReader to read from the given directory."""
+        """Initialise the DirReadWriter to read/write in the given directory."""
         self._dir_path = dir_path
+        self._created_dirs = set()
 
     @classmethod
     @contextlib.contextmanager
-    def open(cls, dir_path: pathlib.Path) -> Iterator[Self]:
-        """Create a DirReader to read from the given directory."""
+    def new_reader(cls, dir_path: pathlib.Path) -> Iterator[Self]:
+        """Create a DirReader to read in the given directory."""
         yield cls(dir_path)
 
     @property
     def dir_path(self) -> pathlib.Path:
         """Returns the directory path."""
         return self._dir_path
 
@@ -208,65 +212,57 @@
     def iter_files(self) -> Iterator[pathlib.PurePath]:
         """Implements Reader.iter_files."""
         for root, _, files in os.walk(self._dir_path):
             for filename in files:
                 full_path = pathlib.PurePath(root) / filename
                 yield full_path.relative_to(self._dir_path)
 
+    def exists(
+        self,
+        path: pathlib.PurePath,
+    ) -> bool:
+        """Implements Reader.exists."""
+        return (self._dir_path / path).exists()
 
-class DirWriter(Writer):
-    """Writes files to a local filesystem directory."""
-
-    _dir_path: pathlib.Path
-    _created_dirs: set[pathlib.Path]
 
-    def __init__(self, dir_path: pathlib.Path) -> None:
-        """Initialise the DirWriter to write to the given directory."""
-        self._dir_path = dir_path
-        self._created_dirs = set()
+class DirReadWriter(DirReader):
+    """Reads and writes files in a local filesystem directory."""
 
     @classmethod
     @contextlib.contextmanager
-    def create(cls, dir_path: pathlib.Path) -> Iterator[Self]:
-        """Create a DirWriter to write to the given directory."""
+    def new_read_writer(cls, dir_path: pathlib.Path) -> Iterator[Self]:
+        """Create a DirReadWriter to read and write in the given directory."""
         yield cls(dir_path)
 
     def open_write(
         self,
         path: pathlib.PurePath,
         newline: str = _NEWLINE,
     ) -> contextlib.AbstractContextManager[IO[str]]:
-        """Implements Writer.open_write."""
+        """Implements ReadWriter.open_write."""
         full_path = self._dir_path / path
         parent_dir = full_path.parent
         if parent_dir not in self._created_dirs:
             parent_dir.mkdir(parents=True, exist_ok=True)
             self._created_dirs.add(parent_dir)
         return full_path.open("wt", encoding=_ENCODING, newline=newline)
 
-    def exists(
-        self,
-        path: pathlib.PurePath,
-    ) -> bool:
-        """Implements Writer.exists."""
-        return (self._dir_path / path).exists()
-
 
-class MemReader(Reader):
-    """Reads files from in-memory files."""
+class MemReader:
+    """Reads in-memory files."""
 
     _files: dict[pathlib.PurePath, str]
 
     def __init__(self, files: dict[pathlib.PurePath, str]) -> None:
         """Initialise the MemReader to read from the given files."""
         self._files = files
 
     @classmethod
     @contextlib.contextmanager
-    def open(cls, files: dict[pathlib.PurePath, str]) -> Iterator[Self]:
+    def new_reader(cls, files: dict[pathlib.PurePath, str]) -> Iterator[Self]:
         """Create a MemReader to read from the given files."""
         yield cls(files)
 
     @contextlib.contextmanager
     def open_read(
         self,
         path: pathlib.PurePath,
@@ -279,128 +275,221 @@
             raise NotFoundError(path) from exc
         yield io.StringIO(contents, newline=newline)
 
     def iter_files(self) -> Iterator[pathlib.PurePath]:
         """Implements Reader.iter_files."""
         return iter(self._files.keys())
 
+    def exists(
+        self,
+        path: pathlib.PurePath,
+    ) -> bool:
+        """Implements Reader.exists."""
+        return path in self._files
 
-class MemWriter(Writer):
-    """Writes files to in-memory files."""
 
-    _files: dict[pathlib.PurePath, str]
-
-    def __init__(self, files: dict[pathlib.PurePath, str]) -> None:
-        """Initialise the MemWriter to write to the given files."""
-        self._files = files
+class MemReadWriter(MemReader):
+    """Reads and writes in-memory files."""
 
     @classmethod
     @contextlib.contextmanager
-    def create(cls, files: dict[pathlib.PurePath, str]) -> Iterator[Self]:
-        """Create a MemReader to write to the given files."""
+    def new_read_writer(cls, files: dict[pathlib.PurePath, str]) -> Iterator[Self]:
+        """Create a MemReadWriter to read and write in the given files."""
         yield cls(files)
 
     @contextlib.contextmanager
     def open_write(
         self,
         path: pathlib.PurePath,
         newline: str = _NEWLINE,
     ) -> Iterator[IO[str]]:
-        """Implements Writer.open_write."""
+        """Implements ReadWriter.open_write."""
         f = io.StringIO(newline=newline)
         try:
             yield f
         finally:
             f.seek(0, io.SEEK_SET)
             self._files[path] = f.read()
 
-    def exists(
-        self,
-        path: pathlib.PurePath,
-    ) -> bool:
-        """Implements Writer.exists."""
-        return path in self._files
-
 
 class ZipReader(Reader):
     """Reads files from a ZIP file."""
 
-    _zip_file: zipfile.ZipFile
+    _zip_file: Optional[zipfile.ZipFile]
 
-    def __init__(self, zip_file: zipfile.ZipFile) -> None:
+    def __init__(self, zip_file: Optional[zipfile.ZipFile]) -> None:
         """Initialise the ZipReader to read from the opened ZIP file."""
         self._zip_file = zip_file
 
     @classmethod
     @contextlib.contextmanager
-    def open(cls, zip_path: pathlib.Path) -> Iterator[Self]:
-        """Create a ZipReader to write to the ZIP file at the path."""
-        zip_file = zipfile.ZipFile(zip_path, "r")
+    def new_reader(
+        cls,
+        zip_path: pathlib.Path,
+        ignore_not_exist: bool = False,
+    ) -> Iterator[Self]:
+        """Create a ZipReader to write to the ZIP file at the path.
+
+        :param zip_path: Path to the ZIP file to open for reading.
+        :param ignore_not_exist: If True, then ignore ``zip_path`` not existing
+        on the filesystem. If the ZIP file does not exist, then the produced
+        ``ZipReader`` will behave as if no files exist within it.
+        :raises NotFoundError: If ``zip_path`` does not exist, and
+        ``ignore_not_exist`` is False.
+        :returns: Context managed ZipReader.
+        """
+        try:
+            zip_file = zipfile.ZipFile(zip_path, "r")
+        except FileNotFoundError:
+            if not ignore_not_exist:
+                raise
+            zip_file = None
+
         try:
             yield cls(zip_file)
         finally:
-            zip_file.close()
+            if zip_file is not None:
+                zip_file.close()
 
     @contextlib.contextmanager
     def open_read(
         self,
         path: pathlib.PurePath,
         newline: str = _NEWLINE,
     ) -> Iterator[IO[str]]:
         """Implements Reader.open_read."""
+        if self._zip_file is None:
+            raise NotFoundError(path)
+
         try:
             f = self._zip_file.open(str(path), "r")
         except KeyError as exc:
             raise NotFoundError(path) from exc
         with f:
             yield io.TextIOWrapper(f, encoding=_ENCODING, newline=newline)
 
     def iter_files(self) -> Iterator[pathlib.PurePath]:
         """Implements Reader.iter_files."""
+        if self._zip_file is None:
+            return
+
         for info in self._zip_file.infolist():
             yield pathlib.PurePath(info.filename)
 
+    def exists(
+        self,
+        path: pathlib.PurePath,
+    ) -> bool:
+        """Implements Reader.exists."""
+        if self._zip_file is None:
+            return False
+
+        try:
+            self._zip_file.getinfo(str(path))
+        except KeyError:
+            return False
+        return True
 
-class ZipWriter(Writer):
-    """Writes files to a ZIP file."""
 
-    _zip_file: zipfile.ZipFile
+class ZipReadWriter:
+    """Reads and writes files in a ZIP file."""
 
-    def __init__(self, zip_file: zipfile.ZipFile) -> None:
-        """Initialise the ZipWriter to write to the opened ZIP file."""
-        self._zip_file = zip_file
+    # _zip_reader is a reader for existing files from an existing Zip file being
+    # updated, if one exists.
+    _zip_reader: ZipReader
+    # _read_writer is a staging area for new files.
+    _read_writer: ReadWriter
+
+    def __init__(self, zip_reader: ZipReader, read_writer: ReadWriter) -> None:
+        """Initialise the ZipReadWriter to write to the opened ZIP file."""
+        self._zip_reader = zip_reader
+        self._read_writer = read_writer
 
     @classmethod
     @contextlib.contextmanager
-    def create(cls, zip_path: pathlib.Path) -> Iterator[Self]:
-        """Create a ZipWriter to write to a new ZIP file at the path."""
-        zip_path.parent.mkdir(parents=True, exist_ok=True)
-        zip_file = zipfile.ZipFile(zip_path, "w")
-        try:
-            yield cls(zip_file)
-        finally:
-            zip_file.close()
+    def new_read_writer(cls, zip_path: pathlib.Path) -> Iterator[Self]:
+        """Create a ZipReadWriter to write to a new ZIP file at the path."""
+        with (
+            tempfile.TemporaryDirectory() as tmpdir,
+            ZipReader.new_reader(zip_path, ignore_not_exist=True) as zip_reader,
+            DirReadWriter.new_reader(pathlib.Path(tmpdir)) as read_writer,
+        ):
+            zrw = cls(zip_reader, read_writer)
+            yield zrw
+
+            if next(read_writer.iter_files(), None) is None:
+                # No files changed, so can leave the existing ZIP file as-is.
+                return
+
+            dest_dir = zip_path.parent
+            dest_dir.mkdir(parents=True, exist_ok=True)
+            new_zip_path = _copy_reader_into_zipfile(zrw, dest_dir)
+
+        shutil.move(new_zip_path, zip_path)
 
     @contextlib.contextmanager
-    def open_write(
+    def open_read(
         self,
         path: pathlib.PurePath,
         newline: str = _NEWLINE,
     ) -> Iterator[IO[str]]:
-        """Implements Writer.open_write."""
-        with self._zip_file.open(str(path), "w") as f:
-            fw = io.TextIOWrapper(f, encoding=_ENCODING, newline=newline)
-            try:
-                yield fw
-            finally:
-                fw.flush()
+        """Implements Reader.open_read."""
+        try:
+            with self._read_writer.open_read(path, newline) as r:
+                yield r
+        except NotFoundError:
+            with self._zip_reader.open_read(path, newline) as r:
+                yield r
+
+    def iter_files(self) -> Iterator[pathlib.PurePath]:
+        """Implements Reader.iter_files."""
+        seen: set[pathlib.PurePath] = set()
+        for path in self._read_writer.iter_files():
+            yield path
+            seen.add(path)
+        for path in self._zip_reader.iter_files():
+            if path not in seen:
+                yield path
 
     def exists(
         self,
         path: pathlib.PurePath,
     ) -> bool:
-        """Implements Writer.exists."""
-        try:
-            self._zip_file.getinfo(str(path))
-        except KeyError:
-            return False
-        return True
+        """Implements Reader.exists."""
+        return self._read_writer.exists(path) or self._zip_reader.exists(path)
+
+    @contextlib.contextmanager
+    def open_write(
+        self,
+        path: pathlib.PurePath,
+        newline: str = _NEWLINE,
+    ) -> Iterator[IO[str]]:
+        """Implements ReadWriter.open_write."""
+        with self._read_writer.open_write(path, newline) as w:
+            yield w
+
+
+def _copy_reader_into_zipfile(
+    reader: Reader,
+    dest_dir: pathlib.Path,
+) -> pathlib.Path:
+    # mkstemp creates a new uniquely named file, but does not delete when we're
+    # done with it, which works nicely to create the new ZIP file without
+    # overwriting any existing file.
+    zf_fd, zf_path_str = tempfile.mkstemp(suffix=".zip", dir=dest_dir)
+    with (
+        os.fdopen(zf_fd, mode="wb") as zf,
+        zipfile.ZipFile(zf, mode="w") as zw,
+    ):
+        for path in reader.iter_files():
+            with (
+                reader.open_read(path, newline="") as r,
+                zw.open(str(path), mode="w") as w,
+            ):
+                wb = io.TextIOWrapper(w, encoding=_ENCODING, newline="")
+                n = 0
+                while data := r.read(64 * 1024):
+                    wb.write(data)
+                    n += len(data)
+                wb.flush()
+
+    return pathlib.Path(zf_path_str)
```

### Comparing `travdata-0.4.0/src/travdata/gui/extraction/cfgwin.py` & `travdata-0.4.1/src/travdata/gui/extraction/cfgwin.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,29 +26,36 @@
 
 
 def _open_config_reader(
     config_type: filesio.IOType,
     config_path: pathlib.Path,
 ) -> contextlib.AbstractContextManager[filesio.Reader]:
     config_type = config_type.resolve_auto(config_path)
-    return config_type.open(config_path)
+    return config_type.new_reader(config_path)
+
+
+def _open_read_writer(
+    path: pathlib.Path,
+) -> contextlib.AbstractContextManager[filesio.ReadWriter]:
+    config_type = filesio.IOType.AUTO.resolve_auto(path)
+    return config_type.new_read_writer(path)
 
 
 @dataclasses.dataclass
 class _ExtractionConfigBuilder:  # pylint: disable=too-many-instance-attributes
     _cfg: Optional[config.Config] = dataclasses.field(default=None, init=False)
     _cfg_error: Optional[str] = dataclasses.field(default=None, init=False)
     _cfg_version: Optional[str] = dataclasses.field(default=None, init=False)
 
     # Remaining fields enable building a config.ExtractionConfig.
     _config_type: filesio.IOType = dataclasses.field(default=filesio.IOType.AUTO, init=False)
     _config_path: Optional[pathlib.Path] = dataclasses.field(default=None, init=False)
     input_pdf: Optional[pathlib.Path] = None
     book_id: Optional[str] = None
-    output_dir: Optional[pathlib.Path] = None
+    output_path: Optional[pathlib.Path] = None
 
     @property
     def cfg(self) -> Optional[config.Config]:
         """Returns the current configuration."""
         return self._cfg
 
     @property
@@ -139,38 +146,32 @@
 
         if self.input_pdf is not None:
             if not self.input_pdf.exists():
                 errors.input_pdf = f"{self.input_pdf} does not exist."
             elif not self.input_pdf.is_file():
                 errors.input_pdf = f"{self.input_pdf} is not a regular file."
 
-        if self.output_dir is not None:
-            if not self.output_dir.exists():
-                errors.output_dir = f"{self.output_dir} does not exist."
-            elif not self.output_dir.is_dir():
-                errors.output_dir = f"{self.output_dir} is not a directory."
-
         return errors
 
     def build(self) -> Optional[bookextract.ExtractionConfig]:
         """Builds the extraction configuration, if complete."""
         if self._cfg is None:
             return None
         if self._config_path is None:
             return None
         if self.input_pdf is None:
             return None
         if self.book_id is None:
             return None
-        if self.output_dir is None:
+        if self.output_path is None:
             return None
 
         return bookextract.ExtractionConfig(
             cfg_reader_ctx=_open_config_reader(self._config_type, self._config_path),
-            out_writer_ctx=filesio.DirWriter.create(self.output_dir),
+            out_writer_ctx=_open_read_writer(self.output_path),
             input_pdf=self.input_pdf,
             book_id=self.book_id,
             overwrite_existing=False,
             with_tags=frozenset(),
             without_tags=frozenset(),
         )
 
@@ -218,15 +219,15 @@
         self._extract_button.clicked.connect(self._run_extraction)
 
         outer_box = qtutil.make_group_vbox(
             "Extract tables from PDF",
             data_usage_text,
             self._init_select_config(),
             self._init_select_input_pdf(),
-            self._init_select_output_dir(),
+            self._init_select_output(),
             QtWidgets.QSpacerItem(
                 0,
                 0,
                 QtWidgets.QSizePolicy.Policy.MinimumExpanding,
                 QtWidgets.QSizePolicy.Policy.MinimumExpanding,
             ),
             self._extract_button,
@@ -286,62 +287,81 @@
         layout.addRow("Input PDF:", self._input_pdf_label)
         layout.addRow(self._input_pdf_error)
         qtutil.set_error_style(self._input_pdf_error)
         layout.addRow("Select book:", self._book_combo)
 
         return input_pdf_box
 
-    def _init_select_output_dir(self) -> QtWidgets.QWidget:
-        self._output_dir_label = QtWidgets.QLabel("")
-        self._output_dir_error = QtWidgets.QLabel("")
-        qtutil.set_error_style(self._output_dir_error)
-        self._output_dir_button = QtWidgets.QPushButton(
+    def _init_select_output(self) -> QtWidgets.QWidget:
+        self._output_path_label = QtWidgets.QLabel("")
+        self._output_path_error = QtWidgets.QLabel("")
+        qtutil.set_error_style(self._output_path_error)
+
+        self._output_path_button_dir = QtWidgets.QPushButton(self._folder_icon, "Select directory")
+        self._output_path_button_dir.clicked.connect(self._select_output_dir)
+        self._output_path_button_zip = QtWidgets.QPushButton(self._file_icon, "Select ZIP")
+        self._output_path_button_zip.clicked.connect(self._select_output_zip)
+        self._output_path_button = QtWidgets.QPushButton(
             self._folder_icon,
-            "Select output directory",
+            "Select output path",
         )
-        self._output_dir_button.clicked.connect(self._select_output_dir)
+        self._output_path_button.clicked.connect(self._select_output_dir)
 
-        output_dir_box = QtWidgets.QGroupBox("Output directory")
+        select_output_box = QtWidgets.QWidget()
+        layout = QtWidgets.QHBoxLayout(select_output_box)
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.addWidget(self._output_path_button_dir)
+        layout.addWidget(self._output_path_button_zip)
+        layout.addSpacerItem(
+            QtWidgets.QSpacerItem(
+                0,
+                0,
+                QtWidgets.QSizePolicy.Policy.MinimumExpanding,
+                QtWidgets.QSizePolicy.Policy.Minimum,
+            )
+        )
+
+        output_dir_box = QtWidgets.QGroupBox("Output")
         layout = QtWidgets.QFormLayout(output_dir_box)
-        layout.addRow("Select directory:", self._output_dir_button)
-        layout.addRow("Output directory:", self._output_dir_label)
-        layout.addRow(self._output_dir_error)
+        layout.addRow("Select output:", select_output_box)
+        layout.addRow("Output path:", self._output_path_label)
+        layout.addRow(self._output_path_error)
 
         return output_dir_box
 
     def showEvent(self, event: QtGui.QShowEvent) -> None:  # pylint: disable=invalid-name
         """Intercepts the window being shown."""
         self._refresh_from_state()
         return super().showEvent(event)
 
     def _refresh_from_state(self) -> None:
         """Update widgets from current self.state."""
         _bulk_enable(
             self._extract_builder.cfg is not None,
             self._input_pdf_button,
             self._book_combo,
-            self._output_dir_button,
+            self._output_path_button,
         )
         _update_path_label(self._config_path_label, self._extract_builder.config_path)
         if version := self._extract_builder.config_version:
             self._config_version_label.setText(f"Version: {version}")
         else:
             self._config_version_label.setText("Version: <unknown>")
 
         _update_path_label(self._input_pdf_label, self._extract_builder.input_pdf)
         if self._book_combo_dirty:
             _repopulate_book_combo(self._book_combo, self._extract_builder.cfg)
             self._book_combo_dirty = False
         _update_book_combo(self._book_combo, self._extract_builder.book_id)
-        _update_path_label(self._output_dir_label, self._extract_builder.output_dir)
+        _update_path_label(self._output_path_label, self._extract_builder.output_path)
 
         errors = self._extract_builder.build_errors()
         _update_error_label(self._config_path_error, errors.config_path)
         _update_error_label(self._input_pdf_error, errors.input_pdf)
-        _update_error_label(self._output_dir_error, errors.output_dir)
+        _update_error_label(self._output_path_error, errors.output_dir)
 
         self._extract = self._extract_builder.build()
         self._extract_button.setEnabled(self._extract is not None and self._runner is None)
 
     def _selected_config(self, config_path: pathlib.Path) -> None:
         self._book_combo_dirty = self._extract_builder.set_config_path(config_path)
         self._guess_book_combo()
@@ -411,29 +431,39 @@
     @QtCore.Slot()
     def _select_book(self, index: int) -> None:
         if self._book_combo_dirty:
             return
         self._extract_builder.book_id = self._book_combo.itemData(index)
         self._refresh_from_state()
 
+    def _selected_output(self, output_path: pathlib.Path) -> None:
+        self._extract_builder.output_path = output_path
+        self._refresh_from_state()
+
     @QtCore.Slot()
     def _select_output_dir(self) -> None:
-        def selected(path: pathlib.Path) -> None:
-            self._extract_builder.output_dir = path
-            self._refresh_from_state()
-
         _do_file_selection(
             parent=self,
             accept_mode=QtWidgets.QFileDialog.AcceptMode.AcceptSave,
             file_mode=QtWidgets.QFileDialog.FileMode.Directory,
-            selected_callback=selected,
+            selected_callback=self._selected_output,
             filter_="",
         )
 
     @QtCore.Slot()
+    def _select_output_zip(self) -> None:
+        _do_file_selection(
+            parent=self,
+            accept_mode=QtWidgets.QFileDialog.AcceptMode.AcceptSave,
+            file_mode=QtWidgets.QFileDialog.FileMode.AnyFile,
+            selected_callback=self._selected_output,
+            filter_="*.zip",
+        )
+
+    @QtCore.Slot()
     def _run_extraction(self) -> None:
         if self._extract is None:
             return
         if self._runner is not None:
             # Extraction already running.
             return
         self._runner = runnerwin.ExtractionRunnerWindow(
@@ -466,42 +496,22 @@
     dialog = QtWidgets.QFileDialog(parent=parent, filter=filter_)
     dialog.setAcceptMode(accept_mode)
     dialog.setFileMode(file_mode)
     dialog.fileSelected.connect(selected)
     dialog.show()
 
 
-def _update_checked(radio: QtWidgets.QRadioButton, state: bool) -> None:
-    if radio.isChecked() != state:
-        radio.setChecked(state)
-
-
 def _bulk_enable(
     enabled: bool,
     *widgets: QtWidgets.QWidget,
 ) -> None:
     for widget in widgets:
         widget.setEnabled(enabled)
 
 
-def _repopulate_io_type_combo(combo: QtWidgets.QComboBox) -> None:
-    combo.clear()
-    combo.addItem("Directory", filesio.IOType.DIR)
-    combo.addItem("ZIP file", filesio.IOType.ZIP)
-
-
-def _update_io_type_combo(combo: QtWidgets.QComboBox, io_type: filesio.IOType) -> None:
-    for i in range(combo.count()):
-        if io_type == combo.itemData(i):
-            combo.setCurrentIndex(i)
-            return
-    # Fall back to selecting the first item.
-    combo.setCurrentIndex(0)
-
-
 def _repopulate_book_combo(combo: QtWidgets.QComboBox, cfg: Optional[config.Config]) -> None:
     combo.clear()
     if cfg is None:
         return
     combo.addItem("<unselected>", None)
     for book_id, book in sorted(cfg.books.items(), key=lambda item: item[1].name):
         combo.addItem(book.name, book_id)
```

### Comparing `travdata-0.4.0/src/travdata/gui/extraction/runnerwin.py` & `travdata-0.4.1/src/travdata/gui/extraction/runnerwin.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/gui/gui.py` & `travdata-0.4.1/src/travdata/gui/gui.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/gui/qtutil.py` & `travdata-0.4.1/src/travdata/gui/qtutil.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/tableconverters/core/registry.py` & `travdata-0.4.1/src/travdata/tableconverters/core/registry.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/tableconverters/core/trade.py` & `travdata-0.4.1/src/travdata/tableconverters/core/trade.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/tableconverters/core/worldcreation.py` & `travdata-0.4.1/src/travdata/tableconverters/core/worldcreation.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/tableconverters/registry.py` & `travdata-0.4.1/src/travdata/tableconverters/registry.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/travellermap/apiurls.py` & `travdata-0.4.1/src/travdata/travellermap/apiurls.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/travellermap/sectorparse.py` & `travdata-0.4.1/src/travdata/travellermap/sectorparse.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/travellermap/world.py` & `travdata-0.4.1/src/travdata/travellermap/world.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/src/travdata/yamlutil.py` & `travdata-0.4.1/src/travdata/yamlutil.py`

 * *Files identical despite different names*

### Comparing `travdata-0.4.0/PKG-INFO` & `travdata-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: travdata
-Version: 0.4.0
+Version: 0.4.1
 Summary: Data utility code for Mongoose Traveller TTRPG.
 Home-page: https://github.com/huin/travdata
 License: MIT
 Keywords: traveller,ttrpg
 Author: John Beisley
 Author-email: johnbeisleyuk@gmail.com
 Requires-Python: >=3.11,<4.0
```

