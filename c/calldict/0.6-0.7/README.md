# Comparing `tmp/calldict-0.6.tar.gz` & `tmp/calldict-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calldict-0.6.tar", last modified: Fri May 12 11:09:05 2023, max compression
+gzip compressed data, was "calldict-0.7.tar", last modified: Wed Sep 20 00:41:58 2023, max compression
```

## Comparing `calldict-0.6.tar` & `calldict-0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 11:09:05.395457 calldict-0.6/
--rw-rw-rw-   0        0        0      400 2023-05-12 11:09:05.395457 calldict-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-12 11:09:05.394450 calldict-0.6/calldict/
--rw-rw-rw-   0        0        0     7259 2023-05-12 11:02:06.305437 calldict-0.6/calldict/__init__.py
--rw-rw-rw-   0        0        0      545 2023-05-12 11:02:41.027828 calldict-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-20 00:41:58.294592 calldict-0.7/
+-rw-rw-rw-   0        0        0      400 2023-09-20 00:41:58.294592 calldict-0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-09-20 00:41:58.292593 calldict-0.7/calldict/
+-rw-rw-rw-   0        0        0     6963 2023-09-20 00:38:28.163728 calldict-0.7/calldict/__init__.py
+-rw-rw-rw-   0        0        0      545 2023-09-20 00:38:15.607893 calldict-0.7/setup.py
```

### Comparing `calldict-0.6/calldict/__init__.py` & `calldict-0.7/calldict/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -167,27 +167,23 @@
     else:
         return data
 
     # @todo make following parameter as integer to allow multilevel precessing
     if not data.get('evaluate', True):
         return dict((x, y) for x, y in data.items() if x != 'evaluate')
 
-    # Evaluate data in sub structure
+    # Evaluate call parameters
     data = data.copy()
-    data['args'] = [eval(v, shared_data=shared_data, memo=memo) for v in data.get('args', [])]
-    kwargs = data.get('kwargs', {})
-    if isinstance(kwargs, SharedValue):
-        data['kwargs'] = kwargs.resolve(shared_data)
-    else:
-        data['kwargs'] = dict([(k, eval(v, shared_data=shared_data, memo=memo))
-                               for k, v in kwargs.items()])
-    data['func'] = eval(data['func'], shared_data=shared_data, memo=memo)
+    for k, v in data.items():
+        if k in ['returns']:
+            continue
+        data[k] = eval(v, shared_data=shared_data, memo=memo)
 
     # Call itself
-    result = data['func'](*data['args'], **data['kwargs'])
+    result = data['func'](*data.get('args', []), **data.get('kwargs', {}))
 
     if isinstance(result, SharedValue):
         result = result.resolve(shared_data)
 
     if 'returns' in data:
         for v in data['returns'] if isinstance(data['returns'],
                                                list) else [data['returns']]:
```

### Comparing `calldict-0.6/setup.py` & `calldict-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='calldict',
     packages=['calldict'],
-    version='0.6',
+    version='0.7',
     description='Protocol to markup and evaluate functions in data structures',
     author='Konstantin Maslyuk',
     author_email='kostyamaslyuk@gmail.com',
     url='https://github.com/kalemas/calldict',
     download_url='https://github.com/kalemas/calldict/archive/master.zip',
     keywords=['dict', 'evaluation', 'yaml'],
     classifiers=[],
```

