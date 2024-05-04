# Comparing `tmp/bufferq-0.1.1.tar.gz` & `tmp/bufferq-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bufferq-0.1.1.tar", max compression
+gzip compressed data, was "bufferq-0.1.2.tar", max compression
```

## Comparing `bufferq-0.1.1.tar` & `bufferq-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    11369 2022-03-29 02:37:43.000000 bufferq-0.1.1/LICENSE
--rw-r--r--   0        0        0     5150 2022-07-23 19:24:30.000000 bufferq-0.1.1/README.md
--rw-r--r--   0        0        0     1129 2022-06-18 05:13:06.000000 bufferq-0.1.1/bufferq/__init__.py
--rw-r--r--   0        0        0    10070 2022-07-23 19:24:30.000000 bufferq-0.1.1/bufferq/async_queues.py
--rw-r--r--   0        0        0     1303 2022-07-23 19:24:30.000000 bufferq-0.1.1/bufferq/errors.py
--rw-r--r--   0        0        0    17518 2022-07-23 19:24:30.000000 bufferq-0.1.1/bufferq/queues.py
--rw-r--r--   0        0        0      178 2022-06-18 05:13:06.000000 bufferq-0.1.1/bufferq/util.py
--rw-r--r--   0        0        0      730 2022-07-23 19:24:30.000000 bufferq-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5922 2022-07-23 19:25:03.592757 bufferq-0.1.1/setup.py
--rw-r--r--   0        0        0     5946 2022-07-23 19:25:03.593733 bufferq-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11369 2022-03-29 02:37:43.000000 bufferq-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5150 2022-07-23 19:24:30.000000 bufferq-0.1.2/README.md
+-rw-r--r--   0        0        0     1389 2024-05-04 19:33:40.484376 bufferq-0.1.2/bufferq/__init__.py
+-rw-r--r--   0        0        0     3741 2024-05-04 19:33:40.484874 bufferq-0.1.2/bufferq/async_queues.py
+-rw-r--r--   0        0        0    20906 2024-05-04 19:33:40.485092 bufferq-0.1.2/bufferq/base.py
+-rw-r--r--   0        0        0     1303 2022-07-23 19:24:30.000000 bufferq-0.1.2/bufferq/errors.py
+-rw-r--r--   0        0        0     3649 2024-05-04 19:33:40.485375 bufferq-0.1.2/bufferq/queues.py
+-rw-r--r--   0        0        0      754 2024-05-04 19:33:40.486207 bufferq-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6048 1970-01-01 00:00:00.000000 bufferq-0.1.2/PKG-INFO
```

### Comparing `bufferq-0.1.1/LICENSE` & `bufferq-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bufferq-0.1.1/README.md` & `bufferq-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bufferq-0.1.1/bufferq/__init__.py` & `bufferq-0.1.2/bufferq/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,23 +11,33 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 try:
     import pkg_resources
 
-    __version__ = pkg_resources.get_distribution('bufferq').version
+    __version__ = pkg_resources.get_distribution("bufferq").version
 except Exception:
-    __version__ = 'unknown'
+    __version__ = "unknown"
 
 # Bring the following imports into scope.
-from bufferq.queues import (
-    QueueBase, Queue, PriorityQueue, LIFOQueue
-)
-from bufferq.errors import (
-    QueueError, QueueEmpty, QueueFull, QueueStopped
-)
+from bufferq.base import AbstractQueue, AsyncAbstractQueue
+from bufferq.queues import Queue, PriorityQueue, LIFOQueue
+from bufferq.errors import QueueError, QueueEmpty, QueueFull, QueueStopped
 
 # Bring the following Asynchronous queues into scope as well.
-from bufferq.async_queues import (
-    AsyncQueueBase, AsyncQueue, AsyncLIFOQueue, AsyncPriorityQueue
-)
+from bufferq.async_queues import AsyncQueue, AsyncLIFOQueue, AsyncPriorityQueue
+
+__all__ = [
+    "QueueError",
+    "QueueEmpty",
+    "QueueFull",
+    "QueueStopped",
+    "AbstractQueue",
+    "Queue",
+    "PriorityQueue",
+    "LIFOQueue",
+    "AsyncAbstractQueue",
+    "AsyncQueue",
+    "AsyncLIFOQueue",
+    "AsyncPriorityQueue",
+]
```

### Comparing `bufferq-0.1.1/bufferq/errors.py` & `bufferq-0.1.2/bufferq/errors.py`

 * *Files identical despite different names*

### Comparing `bufferq-0.1.1/PKG-INFO` & `bufferq-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: bufferq
-Version: 0.1.1
+Version: 0.1.2
 Summary: Queue Library with an improved interface.
 Home-page: https://github.com/eulersIDcrisis/bufferq
 License: Apache-2.0
 Author: Aaron Gibson
 Author-email: eulersidcrisis@yahoo.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Bug Tracker, https://github.com/eulersIDcrisis/bufferq/issues
 Project-URL: Repository, https://github.com/eulersIDcrisis/bufferq
 Description-Content-Type: text/markdown
 
 # bufferq
 
 Better Queue Interface for Python
```

