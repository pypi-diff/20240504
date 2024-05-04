# Comparing `tmp/exctrap-0.1.tar.gz` & `tmp/exctrap-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exctrap-0.1.tar", last modified: Tue Dec 28 08:20:06 2021, max compression
+gzip compressed data, was "exctrap-0.2.tar", last modified: Sat May  4 06:49:54 2024, max compression
```

## Comparing `exctrap-0.1.tar` & `exctrap-0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 kkto      (1000) kkto      (1000)        0 2021-12-28 08:20:06.000000 exctrap-0.1/
--rw-r--r--   0 kkto      (1000) kkto      (1000)     4113 2021-12-28 08:20:06.000000 exctrap-0.1/PKG-INFO
--rw-r--r--   0 kkto      (1000) kkto      (1000)     2915 2021-12-28 07:58:52.000000 exctrap-0.1/README.md
-drwxr-xr-x   0 kkto      (1000) kkto      (1000)        0 2021-12-28 08:20:06.000000 exctrap-0.1/exctrap/
--rw-r--r--   0 kkto      (1000) kkto      (1000)     3765 2021-12-28 07:58:52.000000 exctrap-0.1/exctrap/__init__.py
--rw-r--r--   0 kkto      (1000) kkto      (1000)        0 2021-12-28 07:53:46.000000 exctrap-0.1/exctrap/py.typed
-drwxr-xr-x   0 kkto      (1000) kkto      (1000)        0 2021-12-28 08:20:06.000000 exctrap-0.1/exctrap.egg-info/
--rw-r--r--   0 kkto      (1000) kkto      (1000)     4113 2021-12-28 08:20:06.000000 exctrap-0.1/exctrap.egg-info/PKG-INFO
--rw-r--r--   0 kkto      (1000) kkto      (1000)      179 2021-12-28 08:20:06.000000 exctrap-0.1/exctrap.egg-info/SOURCES.txt
--rw-r--r--   0 kkto      (1000) kkto      (1000)        1 2021-12-28 08:20:06.000000 exctrap-0.1/exctrap.egg-info/dependency_links.txt
--rw-r--r--   0 kkto      (1000) kkto      (1000)        8 2021-12-28 08:20:06.000000 exctrap-0.1/exctrap.egg-info/top_level.txt
--rw-r--r--   0 kkto      (1000) kkto      (1000)       38 2021-12-28 08:20:06.000000 exctrap-0.1/setup.cfg
--rw-r--r--   0 kkto      (1000) kkto      (1000)      907 2021-12-28 08:13:36.000000 exctrap-0.1/setup.py
+drwxr-xr-x   0 kkto      (1000) kkto      (1000)        0 2024-05-04 06:49:54.268381 exctrap-0.2/
+-rw-r--r--   0 kkto      (1000) kkto      (1000)     1065 2021-12-28 02:57:53.000000 exctrap-0.2/LICENSE
+-rw-r--r--   0 kkto      (1000) kkto      (1000)     3567 2024-05-04 06:49:54.268381 exctrap-0.2/PKG-INFO
+-rw-r--r--   0 kkto      (1000) kkto      (1000)     2915 2021-12-28 07:58:52.000000 exctrap-0.2/README.md
+drwxr-xr-x   0 kkto      (1000) kkto      (1000)        0 2024-05-04 06:49:54.268381 exctrap-0.2/exctrap/
+-rw-r--r--   0 kkto      (1000) kkto      (1000)     4184 2021-12-28 08:57:13.000000 exctrap-0.2/exctrap/__init__.py
+-rw-r--r--   0 kkto      (1000) kkto      (1000)        0 2021-12-28 07:53:46.000000 exctrap-0.2/exctrap/py.typed
+drwxr-xr-x   0 kkto      (1000) kkto      (1000)        0 2024-05-04 06:49:54.268381 exctrap-0.2/exctrap.egg-info/
+-rw-r--r--   0 kkto      (1000) kkto      (1000)     3567 2024-05-04 06:49:54.000000 exctrap-0.2/exctrap.egg-info/PKG-INFO
+-rw-r--r--   0 kkto      (1000) kkto      (1000)      187 2024-05-04 06:49:54.000000 exctrap-0.2/exctrap.egg-info/SOURCES.txt
+-rw-r--r--   0 kkto      (1000) kkto      (1000)        1 2024-05-04 06:49:54.000000 exctrap-0.2/exctrap.egg-info/dependency_links.txt
+-rw-r--r--   0 kkto      (1000) kkto      (1000)        8 2024-05-04 06:49:54.000000 exctrap-0.2/exctrap.egg-info/top_level.txt
+-rw-r--r--   0 kkto      (1000) kkto      (1000)       38 2024-05-04 06:49:54.268381 exctrap-0.2/setup.cfg
+-rw-r--r--   0 kkto      (1000) kkto      (1000)      907 2024-05-04 06:49:37.000000 exctrap-0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `exctrap-0.1/PKG-INFO` & `exctrap-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,85 +1,84 @@
 Metadata-Version: 2.1
 Name: exctrap
-Version: 0.1
+Version: 0.2
 Summary: Exception trap
 Home-page: https://github.com/isaacto/exctrap
 Author: Isaac To
 Author-email: isaac.to@gmail.com
-License: UNKNOWN
-Description: # exctrap: Trap exceptions for retry
-        
-        It is not uncommon to have Python code that requires exceptions to be
-        trapped, with the code triggering it retried, e.g., to handle
-        temporary network or host failures when fetching web resources.  There
-        are quite a few Python packages that provide this functionality.  Or
-        actually, two functionalities: (1) trapping the exception, and (2)
-        retrying the triggering code upon failure.
-        
-        Typically, they work in the level of function: the code that needs to
-        be retried is written as a function, and it is either wrapped within a
-        context manager or passed to a retry function so that the function is
-        invoked repeatedly until it succeeds or fail sufficiently many times.
-        In this way, the two functionalities are packed into one function or
-        context manager for the user.
-        
-        We take a slightly different approach: the two functionalities are
-        separated into two entities: a context manager that traps exception,
-        and a function that returns the context manager.  We argue that this
-        leads to neater code.
-        
-        ## Recipe
-        
-        This provides most of what we normally need.
-        
-            for etrapper in exctrap.trial():
-                with etrapper:
-                    # Do whatever that may fail.
-                # Will reach here whether or not an exception is raised.
-                # If you want to reraise the exception here, use etrapper.reraise().
-            # If retry fails, the last exception is reraised so this is not reached.
-        
-        ## Options
-        
-        The `trial()` function provides all the options.  These include:
-        
-          * `num_tries`: Maximum number of trials, if the code keeps raising
-            exceptions for this many tries the exception is reraised without
-            further retry.
-          * `retry_period`: Number of seconds to wait between tries (adjusted
-            by `period_noise`).
-          * `period_noise`: Add or subtract at most this fraction of the
-            `retry_period` to get the actual amount of seconds to sleep.
-          * `etypes`: Exception types to trap.  By default, trap all
-            exceptions derived from `Exception`.  This is passed to the
-            constructor of `ExcTrapper` when creating exception trappers.
-        
-        Note that this does not require any function to be created for the
-        code needs to be exception-proof.  Experience shows that code can be a
-        lot more neat as a result: the code can access the required variables
-        much more easily when it does not sit within a separate global
-        function or an inner function.
-        
-        ## Implementation
-        
-        The "etrapper" is the context manager which traps exceptions when
-        running under the "with" statement.  This is done simply by recording
-        exceptions in the trapper object, and returning True to swallow it, in
-        the `__exit__` function.  If needed, the exception can be asked to be
-        `reraised()`.
-        
-        The `trial()` function provides the retry logic and create exception
-        trappers.  Because the exception would be trapped in the trapper, all
-        trial needs to do is to check whether an exception is trapped, and
-        decide whether to retry or reraise.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# exctrap: Trap exceptions for retry
+
+It is not uncommon to have Python code that requires exceptions to be
+trapped, with the code triggering it retried, e.g., to handle
+temporary network or host failures when fetching web resources.  There
+are quite a few Python packages that provide this functionality.  Or
+actually, two functionalities: (1) trapping the exception, and (2)
+retrying the triggering code upon failure.
+
+Typically, they work in the level of function: the code that needs to
+be retried is written as a function, and it is either wrapped within a
+context manager or passed to a retry function so that the function is
+invoked repeatedly until it succeeds or fail sufficiently many times.
+In this way, the two functionalities are packed into one function or
+context manager for the user.
+
+We take a slightly different approach: the two functionalities are
+separated into two entities: a context manager that traps exception,
+and a function that returns the context manager.  We argue that this
+leads to neater code.
+
+## Recipe
+
+This provides most of what we normally need.
+
+    for etrapper in exctrap.trial():
+        with etrapper:
+            # Do whatever that may fail.
+        # Will reach here whether or not an exception is raised.
+        # If you want to reraise the exception here, use etrapper.reraise().
+    # If retry fails, the last exception is reraised so this is not reached.
+
+## Options
+
+The `trial()` function provides all the options.  These include:
+
+  * `num_tries`: Maximum number of trials, if the code keeps raising
+    exceptions for this many tries the exception is reraised without
+    further retry.
+  * `retry_period`: Number of seconds to wait between tries (adjusted
+    by `period_noise`).
+  * `period_noise`: Add or subtract at most this fraction of the
+    `retry_period` to get the actual amount of seconds to sleep.
+  * `etypes`: Exception types to trap.  By default, trap all
+    exceptions derived from `Exception`.  This is passed to the
+    constructor of `ExcTrapper` when creating exception trappers.
+
+Note that this does not require any function to be created for the
+code needs to be exception-proof.  Experience shows that code can be a
+lot more neat as a result: the code can access the required variables
+much more easily when it does not sit within a separate global
+function or an inner function.
+
+## Implementation
+
+The "etrapper" is the context manager which traps exceptions when
+running under the "with" statement.  This is done simply by recording
+exceptions in the trapper object, and returning True to swallow it, in
+the `__exit__` function.  If needed, the exception can be asked to be
+`reraised()`.
+
+The `trial()` function provides the retry logic and create exception
+trappers.  Because the exception would be trapped in the trapper, all
+trial needs to do is to check whether an exception is trapped, and
+decide whether to retry or reraise.
```

### Comparing `exctrap-0.1/README.md` & `exctrap-0.2/README.md`

 * *Files identical despite different names*

### Comparing `exctrap-0.1/exctrap/__init__.py` & `exctrap-0.2/exctrap/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,16 +73,17 @@
     def reraise(self) -> None:
         """Re-raise the stored exception, if any."""
         if self.exc:
             raise self.exc[0].with_traceback(self.exc[1])
 
 
 def trial(
-        num_tries: int = 3, retry_period: float = 3,
+        num_tries: int = 3, retry_period: float = 3, *,
         period_noise: float = 0.25,
+        backoff: int = 0, backoff_ratio: float = 2,
         etypes: typing.Tuple[typing.Type[BaseException], ...] = (Exception,)
 ) -> typing.Iterator[ExcTrapper]:
     """Retry logic
 
     Generator which yield exception trappers, and stops when no
     exception is trapped by it for an iteration.  Users are supposed
     to use "for" to iterate through the exception trappers, and have
@@ -99,19 +100,28 @@
 
         retry_period: Number of seconds to wait between tries, to be
             modified by period_noise.
 
         period_noise: Add or subtract at most this fraction of the
             retry_period to get the actual amount of seconds to sleep.
 
+        backoff: Change (normally, increase) retry_period this many
+            times from the second trial.  After that the retry_period
+            will stay the same as the last one.
+
+        backoff_ratio: When changing the retry_period, multiply by
+            this number.
+
         etypes: Exception types to trap.  Other exceptions are raised
             directly without attempts for retry.
     """
     for cnt in range(num_tries):
         if cnt:
+            if 1 < cnt < backoff + 2:
+                retry_period *= backoff_ratio
             rnum = random.uniform(1 - period_noise, 1 + period_noise)
             time.sleep(max(rnum * retry_period, 0))
         etrapper = ExcTrapper(etypes)
         yield etrapper
         if not etrapper.exc:
             return
     etrapper.reraise()
```

### Comparing `exctrap-0.1/exctrap.egg-info/PKG-INFO` & `exctrap-0.2/exctrap.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,85 +1,84 @@
 Metadata-Version: 2.1
 Name: exctrap
-Version: 0.1
+Version: 0.2
 Summary: Exception trap
 Home-page: https://github.com/isaacto/exctrap
 Author: Isaac To
 Author-email: isaac.to@gmail.com
-License: UNKNOWN
-Description: # exctrap: Trap exceptions for retry
-        
-        It is not uncommon to have Python code that requires exceptions to be
-        trapped, with the code triggering it retried, e.g., to handle
-        temporary network or host failures when fetching web resources.  There
-        are quite a few Python packages that provide this functionality.  Or
-        actually, two functionalities: (1) trapping the exception, and (2)
-        retrying the triggering code upon failure.
-        
-        Typically, they work in the level of function: the code that needs to
-        be retried is written as a function, and it is either wrapped within a
-        context manager or passed to a retry function so that the function is
-        invoked repeatedly until it succeeds or fail sufficiently many times.
-        In this way, the two functionalities are packed into one function or
-        context manager for the user.
-        
-        We take a slightly different approach: the two functionalities are
-        separated into two entities: a context manager that traps exception,
-        and a function that returns the context manager.  We argue that this
-        leads to neater code.
-        
-        ## Recipe
-        
-        This provides most of what we normally need.
-        
-            for etrapper in exctrap.trial():
-                with etrapper:
-                    # Do whatever that may fail.
-                # Will reach here whether or not an exception is raised.
-                # If you want to reraise the exception here, use etrapper.reraise().
-            # If retry fails, the last exception is reraised so this is not reached.
-        
-        ## Options
-        
-        The `trial()` function provides all the options.  These include:
-        
-          * `num_tries`: Maximum number of trials, if the code keeps raising
-            exceptions for this many tries the exception is reraised without
-            further retry.
-          * `retry_period`: Number of seconds to wait between tries (adjusted
-            by `period_noise`).
-          * `period_noise`: Add or subtract at most this fraction of the
-            `retry_period` to get the actual amount of seconds to sleep.
-          * `etypes`: Exception types to trap.  By default, trap all
-            exceptions derived from `Exception`.  This is passed to the
-            constructor of `ExcTrapper` when creating exception trappers.
-        
-        Note that this does not require any function to be created for the
-        code needs to be exception-proof.  Experience shows that code can be a
-        lot more neat as a result: the code can access the required variables
-        much more easily when it does not sit within a separate global
-        function or an inner function.
-        
-        ## Implementation
-        
-        The "etrapper" is the context manager which traps exceptions when
-        running under the "with" statement.  This is done simply by recording
-        exceptions in the trapper object, and returning True to swallow it, in
-        the `__exit__` function.  If needed, the exception can be asked to be
-        `reraised()`.
-        
-        The `trial()` function provides the retry logic and create exception
-        trappers.  Because the exception would be trapped in the trapper, all
-        trial needs to do is to check whether an exception is trapped, and
-        decide whether to retry or reraise.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# exctrap: Trap exceptions for retry
+
+It is not uncommon to have Python code that requires exceptions to be
+trapped, with the code triggering it retried, e.g., to handle
+temporary network or host failures when fetching web resources.  There
+are quite a few Python packages that provide this functionality.  Or
+actually, two functionalities: (1) trapping the exception, and (2)
+retrying the triggering code upon failure.
+
+Typically, they work in the level of function: the code that needs to
+be retried is written as a function, and it is either wrapped within a
+context manager or passed to a retry function so that the function is
+invoked repeatedly until it succeeds or fail sufficiently many times.
+In this way, the two functionalities are packed into one function or
+context manager for the user.
+
+We take a slightly different approach: the two functionalities are
+separated into two entities: a context manager that traps exception,
+and a function that returns the context manager.  We argue that this
+leads to neater code.
+
+## Recipe
+
+This provides most of what we normally need.
+
+    for etrapper in exctrap.trial():
+        with etrapper:
+            # Do whatever that may fail.
+        # Will reach here whether or not an exception is raised.
+        # If you want to reraise the exception here, use etrapper.reraise().
+    # If retry fails, the last exception is reraised so this is not reached.
+
+## Options
+
+The `trial()` function provides all the options.  These include:
+
+  * `num_tries`: Maximum number of trials, if the code keeps raising
+    exceptions for this many tries the exception is reraised without
+    further retry.
+  * `retry_period`: Number of seconds to wait between tries (adjusted
+    by `period_noise`).
+  * `period_noise`: Add or subtract at most this fraction of the
+    `retry_period` to get the actual amount of seconds to sleep.
+  * `etypes`: Exception types to trap.  By default, trap all
+    exceptions derived from `Exception`.  This is passed to the
+    constructor of `ExcTrapper` when creating exception trappers.
+
+Note that this does not require any function to be created for the
+code needs to be exception-proof.  Experience shows that code can be a
+lot more neat as a result: the code can access the required variables
+much more easily when it does not sit within a separate global
+function or an inner function.
+
+## Implementation
+
+The "etrapper" is the context manager which traps exceptions when
+running under the "with" statement.  This is done simply by recording
+exceptions in the trapper object, and returning True to swallow it, in
+the `__exit__` function.  If needed, the exception can be asked to be
+`reraised()`.
+
+The `trial()` function provides the retry logic and create exception
+trappers.  Because the exception would be trapped in the trapper, all
+trial needs to do is to check whether an exception is trapped, and
+decide whether to retry or reraise.
```

### Comparing `exctrap-0.1/setup.py` & `exctrap-0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='exctrap',
-    version='0.1',
+    version='0.2',
     python_requires='~=3.7',
     author='Isaac To',
     author_email='isaac.to@gmail.com',
     description='Exception trap',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/isaacto/exctrap',
```

