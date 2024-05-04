# Comparing `tmp/sts_lib-0.30.2.tar.gz` & `tmp/sts_lib-0.30.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.30.2.tar", last modified: Thu May  2 12:17:42 2024, max compression
+gzip compressed data, was "sts_lib-0.30.3.tar", last modified: Sat May  4 08:50:47 2024, max compression
```

## Comparing `sts_lib-0.30.2.tar` & `sts_lib-0.30.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 12:17:42.772128 sts_lib-0.30.2/
--rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.30.2/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.30.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6916 2024-05-02 12:17:42.772128 sts_lib-0.30.2/PKG-INFO
--rw-rw-rw-   0        0        0     5463 2024-04-29 19:01:51.000000 sts_lib-0.30.2/README.md
--rw-rw-rw-   0        0        0     1728 2024-05-02 12:17:42.772128 sts_lib-0.30.2/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.30.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:17:42.718969 sts_lib-0.30.2/sts/
--rw-rw-rw-   0        0        0    52950 2024-05-02 12:17:18.000000 sts_lib-0.30.2/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.30.2/sts/__main__.py
--rw-rw-rw-   0        0        0     7551 2024-05-02 11:33:58.000000 sts_lib-0.30.2/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:17:42.718969 sts_lib-0.30.2/sts/data/
-drwxrwxrwx   0        0        0        0 2024-05-02 12:17:42.739964 sts_lib-0.30.2/sts/data/config/
--rw-rw-rw-   0        0        0      915 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      608 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      346 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      410 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      419 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      267 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      417 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      607 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      247 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      261 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      267 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      245 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      606 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      670 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      344 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-05-02 12:17:42.757108 sts_lib-0.30.2/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    22659 2024-05-02 11:55:17.000000 sts_lib-0.30.2/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-05-02 12:17:42.757108 sts_lib-0.30.2/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2024-05-02 12:17:13.000000 sts_lib-0.30.2/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 12:17:42.766109 sts_lib-0.30.2/sts_lib.egg-info/
--rw-rw-rw-   0        0        0     6916 2024-05-02 12:17:42.000000 sts_lib-0.30.2/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-05-02 12:17:42.000000 sts_lib-0.30.2/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 12:17:42.000000 sts_lib-0.30.2/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-02 12:17:42.000000 sts_lib-0.30.2/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      202 2024-05-02 12:17:42.000000 sts_lib-0.30.2/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-02 12:17:42.000000 sts_lib-0.30.2/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.553971 sts_lib-0.30.3/
+-rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.30.3/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.30.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6916 2024-05-04 08:50:47.553971 sts_lib-0.30.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5463 2024-04-29 19:01:51.000000 sts_lib-0.30.3/README.md
+-rw-rw-rw-   0        0        0     1728 2024-05-04 08:50:47.553971 sts_lib-0.30.3/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.30.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.422407 sts_lib-0.30.3/sts/
+-rw-rw-rw-   0        0        0    52916 2024-05-04 08:48:31.000000 sts_lib-0.30.3/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.30.3/sts/__main__.py
+-rw-rw-rw-   0        0        0     7551 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.422407 sts_lib-0.30.3/sts/data/
+drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.438030 sts_lib-0.30.3/sts/data/config/
+-rw-rw-rw-   0        0        0      915 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      608 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      346 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      410 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      419 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      267 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      417 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      607 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      247 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      261 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      267 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      245 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      606 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      670 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      344 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.475845 sts_lib-0.30.3/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-05-02 13:01:51.000000 sts_lib-0.30.3/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    22659 2024-05-04 08:41:18.000000 sts_lib-0.30.3/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.507097 sts_lib-0.30.3/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.538335 sts_lib-0.30.3/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0     6916 2024-05-04 08:50:47.000000 sts_lib-0.30.3/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-05-04 08:50:47.000000 sts_lib-0.30.3/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 08:50:47.000000 sts_lib-0.30.3/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-04 08:50:47.000000 sts_lib-0.30.3/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-05-04 08:50:47.000000 sts_lib-0.30.3/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-04 08:50:47.000000 sts_lib-0.30.3/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.30.2/LICENSE` & `sts_lib-0.30.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/PKG-INFO` & `sts_lib-0.30.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.30.2
+Version: 0.30.3
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.30.2/README.md` & `sts_lib-0.30.3/README.md`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/setup.cfg` & `sts_lib-0.30.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/__init__.py` & `sts_lib-0.30.3/sts/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.30.2'
+__version__ = '0.30.3'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 StsConvExclude = namedtuple('StsConvExclude', ['text'])
 
 
 class StreamList(list):
@@ -228,15 +228,15 @@
         """Implementation of len(self).
         """
         return len(self._dict)
 
     def __iter__(self):
         """Implementation of iter(self).
         """
-        yield from self._dict
+        return iter(self._dict)
 
     def __eq__(self, other):
         """Implementation of "==" operator.
         """
         if not isinstance(other, (dict, StsDict)):
             return False
 
@@ -780,16 +780,16 @@
     NOTE: The internal data format is different from base StsDict.
     """
     def __getitem__(self, key):
         """Implementation of self[key].
         """
         trie = self._dict
         try:
-            for k in self._split(key):
-                trie = trie[k]
+            for comp in Unicode.split(key):
+                trie = trie[comp]
             return trie['']
         except KeyError:
             raise KeyError(key)
 
     def __contains__(self, item):
         """Implementation of "item in self".
         """
@@ -804,93 +804,93 @@
         """Implementation of len(self).
         """
         return sum(1 for _ in self)
 
     def __iter__(self):
         """Implementation of iter(self).
         """
-        yield from self.keys()
+        return self.keys()
 
     def __delitem__(self, key):
         """Implementation of del self[key].
         """
         trie = self._dict
         try:
-            for k in self._split(key):
-                trie = trie[k]
+            for comp in Unicode.split(key):
+                trie = trie[comp]
             del trie['']
         except KeyError:
             raise KeyError(key)
 
     def keys(self):
         """Get a generator of keys.
         """
-        def recurse(trie):
-            for key in trie:
-                if key == '':
-                    yield ''.join(keystack)
+        trie = self._dict
+        stack = [('', trie, iter(trie))]
+        while stack:
+            key, trie, it = stack[-1]
+            for comp in it:
+                if comp == '':
+                    yield key
                 else:
-                    keystack.append(key)
-                    triestack.append(trie[key])
-                    yield from recurse(triestack[-1])
-            keystack.pop()
-            triestack.pop()
-
-        keystack = ['']
-        triestack = [self._dict]
-        yield from recurse(triestack[-1])
+                    trie = trie[comp]
+                    stack.append((key + comp, trie, iter(trie)))
+                    break
+            else:
+                stack.pop()
 
     def values(self):
         """Get a generator of values.
         """
-        def recurse(trie):
-            for key in trie:
-                if key == '':
-                    yield trie[key]
+        trie = self._dict
+        stack = [(trie, iter(trie))]
+        while stack:
+            trie, it = stack[-1]
+            for comp in it:
+                if comp == '':
+                    yield trie[comp]
                 else:
-                    triestack.append(trie[key])
-                    yield from recurse(triestack[-1])
-            triestack.pop()
-
-        triestack = [self._dict]
-        yield from recurse(triestack[-1])
+                    trie = trie[comp]
+                    stack.append((trie, iter(trie)))
+                    break
+            else:
+                stack.pop()
 
     def items(self):
         """Get a generator of key-values pairs.
         """
-        def recurse(trie):
-            for key in trie:
-                if key == '':
-                    yield ''.join(keystack), trie[key]
+        trie = self._dict
+        stack = [('', trie, iter(trie))]
+        while stack:
+            key, trie, it = stack[-1]
+            for comp in it:
+                if comp == '':
+                    yield key, trie[comp]
                 else:
-                    keystack.append(key)
-                    triestack.append(trie[key])
-                    yield from recurse(triestack[-1])
-            keystack.pop()
-            triestack.pop()
-
-        keystack = ['']
-        triestack = [self._dict]
-        yield from recurse(triestack[-1])
+                    trie = trie[comp]
+                    stack.append((key + comp, trie, iter(trie)))
+                    break
+            else:
+                stack.pop()
 
     def add(self, key, values, skip_check=False):
         """Add a key-values pair to this dictionary.
 
         Args:
             values: a string or a list of strings.
             skip_check: True to skip checking duplicated values.
         """
-        values = [values] if isinstance(values, str) else values
+        values = (values,) if isinstance(values, str) else values
 
-        current = self._dict
-        for composite in Unicode.split(key):
-            current = current.setdefault(composite, {})
+        trie = self._dict
+        for comp in Unicode.split(key):
+            trie = trie.setdefault(comp, {})
 
-        list_ = current.setdefault('', [])
-        list_ += values if skip_check else [x for x in values if x not in list_]
+        list_ = trie.setdefault('', [])
+        list_ += values if skip_check else (x for x in values if x not in list_)
         return self
 
     def match(self, parts, pos, maxpos=math.inf):
         """Match a unicode composite at pos.
 
         Args:
             parts: a string or iterable parts to be matched.
```

### Comparing `sts_lib-0.30.2/sts/cli.py` & `sts_lib-0.30.3/sts/cli.py`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/config/_default.json` & `sts_lib-0.30.3/sts/data/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/config/hk2s.json` & `sts_lib-0.30.3/sts/data/config/hk2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/config/s2twp.json` & `sts_lib-0.30.3/sts/data/config/s2twp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/config/tw2s.json` & `sts_lib-0.30.3/sts/data/config/tw2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/config/tw2sp.json` & `sts_lib-0.30.3/sts/data/config/tw2sp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.30.3/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.30.3/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.30.3/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.30.3/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.30.3/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.30.3/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.30.3/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.30.3/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.30.3/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.30.3/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.30.3/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.30.3/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/htmlpage.tpl.html` & `sts_lib-0.30.3/sts/data/htmlpage.tpl.html`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/scheme/st_multi.txt` & `sts_lib-0.30.3/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts/data/scheme/variant.txt` & `sts_lib-0.30.3/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.2/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.30.3/sts_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.30.2
+Version: 0.30.3
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.30.2/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.30.3/sts_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

