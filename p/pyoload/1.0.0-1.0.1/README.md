# Comparing `tmp/pyoload-1.0.0.tar.gz` & `tmp/pyoload-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoload-1.0.0.tar", last modified: Thu May  2 02:57:10 2024, max compression
+gzip compressed data, was "pyoload-1.0.1.tar", last modified: Sat May  4 00:49:18 2024, max compression
```

## Comparing `pyoload-1.0.0.tar` & `pyoload-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:57:10.233789 pyoload-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-02 02:57:08.000000 pyoload-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-02 02:57:10.233789 pyoload-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-02 02:57:08.000000 pyoload-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:57:10.229789 pyoload-1.0.0/pyoload/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-02 02:57:06.000000 pyoload-1.0.0/pyoload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:57:10.229789 pyoload-1.0.0/pyoload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-02 02:57:10.000000 pyoload-1.0.0/pyoload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-02 02:57:10.000000 pyoload-1.0.0/pyoload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 02:57:10.000000 pyoload-1.0.0/pyoload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-02 02:57:10.000000 pyoload-1.0.0/pyoload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 02:57:10.000000 pyoload-1.0.0/pyoload.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 02:57:10.233789 pyoload-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-02 02:57:06.000000 pyoload-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:57:10.229789 pyoload-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-02 02:57:06.000000 pyoload-1.0.0/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:49:18.786731 pyoload-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-04 00:49:16.000000 pyoload-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-04 00:49:18.786731 pyoload-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-04 00:49:16.000000 pyoload-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:49:18.782731 pyoload-1.0.1/pyoload/
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-04 00:49:14.000000 pyoload-1.0.1/pyoload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:49:18.782731 pyoload-1.0.1/pyoload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-04 00:49:18.000000 pyoload-1.0.1/pyoload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-04 00:49:18.000000 pyoload-1.0.1/pyoload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:49:18.000000 pyoload-1.0.1/pyoload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-04 00:49:18.000000 pyoload-1.0.1/pyoload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 00:49:18.000000 pyoload-1.0.1/pyoload.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 00:49:18.786731 pyoload-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-04 00:49:14.000000 pyoload-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:49:18.782731 pyoload-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-04 00:49:14.000000 pyoload-1.0.1/tests/test_placeholder.py
```

### Comparing `pyoload-1.0.0/LICENSE` & `pyoload-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoload-1.0.0/pyoload/__init__.py` & `pyoload-1.0.1/pyoload/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,54 +39,70 @@
     __repr__ = __str__
 
 
 def get_name(funcOrCls):
     return funcOrCls.__module__ + '.' + funcOrCls.__qualname__
 
 
-class TypeChecker:
+class Validator:
     def __init__(self, func):
         if not callable(func):
             raise TypeError(self.__class__.__init__.__qualname__)
         self.func = func
 
     def __call__(self, val):
         try:
             return self.func()
         except Exception as e:
             raise AnnotationError(
-                f'{type(e)} while using typechecker method: {get_name(self.func)}' +
+                f'{type(e)} while using validator method: {get_name(self.func)}' +
                 f'\n{e!s}',
             ) from e
 
 
 class Cast:
+    @staticmethod
+    def cast(val, type):
+        if issubclass(type, Union):
+            type = type.__args__
+        if isinstance(type, tuple):
+            for x in type:
+                try:
+                    return Cast.cast(val, x)
+                except Exception:
+                    pass
+            else:
+                raise CastingError()
+        return type(val) if not isinstance(val, type) else val
+
     def __init__(self, type):
         self.type = type
 
     def __call__(self, val):
         try:
-            return self.type(val)
+            return Cast.cast(self.type, val)
         except Exception as e:
             raise CastingError(
                 f'Exception while casting: {val!r} to {self.type}',
             ) from e
 
 
 def typeMatch(val, spec):
     if spec == Any or spec is None:
         return True
+    if isinstance(val, tuple):
+        return isinstance(val, tuple)
     if isinstance(spec, Values):
         return spec(val)
-    elif isinstance(spec, TypeChecker):
+    elif isinstance(spec, Validator):
         return spec(val)
     elif isinstance(spec, GenericAlias):
         if not isinstance(val, spec.__origin__):
             return False
-        sub = Union[*spec.__args__]
+        sub = spec.__args__
         for val in val:
             if not typeMatch(val, sub):
                 return False
         else:
             return True
     else:
         return isinstance(val, spec)
@@ -217,8 +233,8 @@
             )
         else:
             return setter(self, name, value)
     cls.__setattr__ = new_setter
     return cls
 
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
```

### Comparing `pyoload-1.0.0/setup.py` & `pyoload-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -66,13 +66,16 @@
         # 'Development Status :: 6 - Mature',
         # 'Development Status :: 7 - Inactive',
 
         'License :: OSI Approved :: MIT License',
 
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
 
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 )
```

