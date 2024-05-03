# Comparing `tmp/py_gadzooks-0.2.5.tar.gz` & `tmp/py_gadzooks-0.2.7.tar.gz`

## Comparing `py_gadzooks-0.2.5.tar` & `py_gadzooks-0.2.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 py_gadzooks-0.2.5/gadzooks/__init__.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 py_gadzooks-0.2.5/gadzooks/build_docs.py
--rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 py_gadzooks-0.2.5/gadzooks/check_version.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 py_gadzooks-0.2.5/gadzooks/loc_summarize.py
--rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 py_gadzooks-0.2.5/gadzooks/main.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 py_gadzooks-0.2.5/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 py_gadzooks-0.2.5/LICENSE
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 py_gadzooks-0.2.5/README.md
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 py_gadzooks-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 py_gadzooks-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/gadzooks/__init__.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/gadzooks/build_docs.py
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/gadzooks/check_version.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/gadzooks/loc_summarize.py
+-rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/gadzooks/main.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/LICENSE
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/README.md
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/PKG-INFO
```

### Comparing `py_gadzooks-0.2.5/gadzooks/__init__.py` & `py_gadzooks-0.2.7/gadzooks/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from argparse import ArgumentParser, Namespace
 import sys
 from typing import ClassVar, Optional
 
 
-__version__ = '0.2.5'
+__version__ = '0.2.7'
 
 
 def error(msg: str) -> None:
     """Prints an error message and exits the program with return code 1."""
     print(f'ERROR: {msg}', file=sys.stderr)
     sys.exit(1)
```

### Comparing `py_gadzooks-0.2.5/gadzooks/build_docs.py` & `py_gadzooks-0.2.7/gadzooks/build_docs.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,63 +14,72 @@
     assert len(hashes) > 0
     arr = [0 for _ in hashes[0]]
     for h in hashes:
         for (i, b) in enumerate(arr):
             arr[i] = b ^ h[i]
     return binascii.hexlify(bytes(arr))
 
-def get_file_checksum(paths: Sequence[Path]) -> str:
+def get_file_checksum(paths: Sequence[Path], verbose: bool = False) -> str:
     """Computes the checksum of some files, returning it as a hex string."""
     print(f'computing checksum of {len(paths)} file(s)')
     cmd = ['sha1sum'] + list(map(str, paths))
     lines = subprocess.check_output(cmd, text=True).splitlines()
     hashes = []
     for line in lines:
         [content_hash, name] = line.split()
         name_hash = hashlib.sha1(name.encode()).hexdigest()
-    hashes += list(map(binascii.unhexlify, [name_hash, content_hash]))
+        hashes += list(map(binascii.unhexlify, [name_hash, content_hash]))
+        if verbose:
+            print(line)
     return xor_bytes(hashes).decode()
 
 
 class BuildDocs(Subcommand):
     """build project documentation"""
 
     @classmethod
     def configure_parser(cls, parser: ArgumentParser) -> None:
-        parser.add_argument('--src-docs', nargs='*', help='path(s) to input docs (will use checksum to decide whether to rebuild)')
+        parser.add_argument('--src-docs', nargs='+', required=True, help='path(s) to input docs (will use checksum to decide whether to rebuild)')
         parser.add_argument('--checksum-file', type=Path, default='.doc-checksum', help='checksum file')
         parser.add_argument('-f', '--force', action='store_true', help='force rebuild')
+        parser.add_argument('--check-only', action='store_true', help='only check whether input docs have changed (do not rebuild)')
+        parser.add_argument('-v', '--verbose', action='store_true', help='print out filenames and hashes')
 
     @classmethod
     def main(cls, args: Namespace, extra_args: Optional[list[str]] = None) -> None:
-        if not extra_args:
+        if not (args.check_only or extra_args):
             error('must provide: -- <BUILD_DOCS_COMMAND>')
         assert isinstance(extra_args, list)
+        paths: list[Path] = []
+        for path in args.src_docs:
+            path = Path(path)
+            if path.is_dir():
+                paths.extend([p for p in path.rglob('*') if p.is_file()])
+            else:
+                paths.append(path)
+        checksum = get_file_checksum(paths, verbose=args.verbose) if paths else None
+        msg = None
         if args.force:
-            rebuild = True
-            print('force rebuilding docs')
+            pass
+        elif args.checksum_file.exists():
+            with open(args.checksum_file) as f:
+                prev_checksum = f.read().strip()
+            if checksum == prev_checksum:
+                print(f'checksum matches {args.checksum_file} -- source docs are unchanged')
+                return
+            msg = 'source docs have changed'
         else:
-            paths: list[Path] = []
-            for path in args.src_docs:
-                path = Path(path)
-                if path.is_dir():
-                    paths.extend([p for p in path.rglob('*') if p.is_file()])
-                else:
-                    paths.append(path)
-            checksum = get_file_checksum(paths) if paths else None
-            rebuild = True
-            if args.checksum_file.exists():
-                with open(args.checksum_file) as f:
-                    prev_checksum = f.read().strip()
-                if checksum == prev_checksum:
-                    print(f'checksum matches {args.checksum_file} -- source docs are unchanged')
-                    rebuild = False
-                else:
-                    print('source docs have changed... rebuilding')
-            else:
-                print('no checksum file found... rebuilding')
-        if rebuild:
-            print(' '.join(extra_args))
-            subprocess.run(extra_args)
-            if checksum:
-                with open(args.checksum_file, 'w') as f:
-                    print(checksum, file=f)
+            msg = 'no checksum file found'
+        if args.check_only:
+            print(f'\033[1;33mWARNING: {msg}')
+            return
+        print(msg)
+        msg = 'rebuilding docs...'
+        if args.force:
+            msg = 'force ' + msg
+        print(msg)
+        print(' '.join(extra_args))
+        subprocess.run(extra_args)
+        if checksum:
+            with open(args.checksum_file, 'w') as f:
+                print(checksum, file=f)
+            print(f'saved checksum to {args.checksum_file}')
```

### Comparing `py_gadzooks-0.2.5/gadzooks/check_version.py` & `py_gadzooks-0.2.7/gadzooks/check_version.py`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.5/gadzooks/loc_summarize.py` & `py_gadzooks-0.2.7/gadzooks/loc_summarize.py`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.5/gadzooks/main.py` & `py_gadzooks-0.2.7/gadzooks/main.py`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.5/LICENSE` & `py_gadzooks-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.5/README.md` & `py_gadzooks-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.5/pyproject.toml` & `py_gadzooks-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.5/PKG-INFO` & `py_gadzooks-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: py-gadzooks
-Version: 0.2.5
+Version: 0.2.7
 Summary: A collection of code maintenance tools for Python projects, intended to be used within git hooks.
 Project-URL: Documentation, https://github.com/jeremander/gadzooks#readme
 Project-URL: Issues, https://github.com/jeremander/gadzooks/issues
 Project-URL: Source, https://github.com/jeremander/gadzooks
 Author-email: Jeremy Silver <jeremys@nessiness.com>
 License-Expression: MIT
 License-File: LICENSE
```

