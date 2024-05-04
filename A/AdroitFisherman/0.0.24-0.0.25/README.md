# Comparing `tmp/AdroitFisherman-0.0.24.tar.gz` & `tmp/AdroitFisherman-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdroitFisherman-0.0.24.tar", last modified: Mon Apr 29 14:12:20 2024, max compression
+gzip compressed data, was "AdroitFisherman-0.0.25.tar", last modified: Sat May  4 05:59:24 2024, max compression
```

## Comparing `AdroitFisherman-0.0.24.tar` & `AdroitFisherman-0.0.25.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.817307 AdroitFisherman-0.0.24/
-drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.795366 AdroitFisherman-0.0.24/AdroitFisherman/
-drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.812321 AdroitFisherman-0.0.24/AdroitFisherman/Utilities/
--rw-rw-rw-   0        0        0      701 2024-04-29 14:10:00.000000 AdroitFisherman-0.0.24/AdroitFisherman/Utilities/SequentialList.py
--rw-rw-rw-   0        0        0      843 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.24/AdroitFisherman/Utilities/SingleLinkedList.py
--rw-rw-rw-   0        0        0       32 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.24/AdroitFisherman/Utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.813321 AdroitFisherman-0.0.24/AdroitFisherman/Utilities/__pycache__/
--rw-rw-rw-   0        0        0      161 2024-04-29 13:36:19.000000 AdroitFisherman-0.0.24/AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0        0 2024-04-29 04:35:09.000000 AdroitFisherman-0.0.24/AdroitFisherman/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.814317 AdroitFisherman-0.0.24/AdroitFisherman/__pycache__/
--rw-rw-rw-   0        0        0      166 2024-04-29 04:35:10.000000 AdroitFisherman-0.0.24/AdroitFisherman/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.816311 AdroitFisherman-0.0.24/AdroitFisherman/includes/
--rw-rw-rw-   0        0        0      720 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.24/AdroitFisherman/includes/SeqList.c
--rw-rw-rw-   0        0        0     5163 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.24/AdroitFisherman/includes/SeqList.h
--rw-rw-rw-   0        0        0     1103 2024-04-29 04:03:41.000000 AdroitFisherman-0.0.24/AdroitFisherman/includes/SingleLinkedList.c
--rw-rw-rw-   0        0        0     8070 2024-04-29 04:10:03.000000 AdroitFisherman-0.0.24/AdroitFisherman/includes/SingleLinkedList.h
-drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.807336 AdroitFisherman-0.0.24/AdroitFisherman.egg-info/
--rw-rw-rw-   0        0        0     3089 2024-04-29 14:12:20.000000 AdroitFisherman-0.0.24/AdroitFisherman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      705 2024-04-29 14:12:20.000000 AdroitFisherman-0.0.24/AdroitFisherman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 14:12:20.000000 AdroitFisherman-0.0.24/AdroitFisherman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 14:12:20.000000 AdroitFisherman-0.0.24/AdroitFisherman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      107 2024-04-25 11:08:16.000000 AdroitFisherman-0.0.24/MANIFEST.in
--rw-rw-rw-   0        0        0     3089 2024-04-29 14:12:20.817307 AdroitFisherman-0.0.24/PKG-INFO
--rw-rw-rw-   0        0        0     2417 2024-04-25 07:13:31.000000 AdroitFisherman-0.0.24/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 14:12:20.818306 AdroitFisherman-0.0.24/setup.cfg
--rw-rw-rw-   0        0        0     1174 2024-04-29 14:12:17.000000 AdroitFisherman-0.0.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.310963 AdroitFisherman-0.0.25/
+drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.295006 AdroitFisherman-0.0.25/AdroitFisherman/
+drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.305977 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/
+-rw-rw-rw-   0        0        0      701 2024-04-29 14:10:00.000000 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/SequentialList.py
+-rw-rw-rw-   0        0        0      843 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/SingleLinkedList.py
+-rw-rw-rw-   0        0        0      882 2024-05-04 05:30:33.000000 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py
+-rw-rw-rw-   0        0        0       32 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.306974 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/__pycache__/
+-rw-rw-rw-   0        0        0     1781 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc
+-rw-rw-rw-   0        0        0      202 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0        0 2024-04-29 04:35:09.000000 AdroitFisherman-0.0.25/AdroitFisherman/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.307971 AdroitFisherman-0.0.25/AdroitFisherman/__pycache__/
+-rw-rw-rw-   0        0        0      166 2024-04-29 04:35:10.000000 AdroitFisherman-0.0.25/AdroitFisherman/__pycache__/__init__.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.310963 AdroitFisherman-0.0.25/AdroitFisherman/includes/
+-rw-rw-rw-   0        0        0      720 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.25/AdroitFisherman/includes/SeqList.c
+-rw-rw-rw-   0        0        0     5147 2024-05-04 03:47:56.000000 AdroitFisherman-0.0.25/AdroitFisherman/includes/SeqList.h
+-rw-rw-rw-   0        0        0     1103 2024-04-29 04:03:41.000000 AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedList.c
+-rw-rw-rw-   0        0        0     8093 2024-05-04 03:47:56.000000 AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedList.h
+-rw-rw-rw-   0        0        0      883 2024-05-04 05:23:21.000000 AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
+-rw-rw-rw-   0        0        0     9086 2024-05-04 05:59:20.000000 AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h
+drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.300990 AdroitFisherman-0.0.25/AdroitFisherman.egg-info/
+-rw-rw-rw-   0        0        0     3192 2024-05-04 05:59:24.000000 AdroitFisherman-0.0.25/AdroitFisherman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2024-05-04 05:59:24.000000 AdroitFisherman-0.0.25/AdroitFisherman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 05:59:24.000000 AdroitFisherman-0.0.25/AdroitFisherman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-04 05:59:24.000000 AdroitFisherman-0.0.25/AdroitFisherman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      107 2024-04-25 11:08:16.000000 AdroitFisherman-0.0.25/MANIFEST.in
+-rw-rw-rw-   0        0        0     3192 2024-05-04 05:59:24.311961 AdroitFisherman-0.0.25/PKG-INFO
+-rw-rw-rw-   0        0        0     2417 2024-04-25 07:13:31.000000 AdroitFisherman-0.0.25/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 05:59:24.312958 AdroitFisherman-0.0.25/setup.cfg
+-rw-rw-rw-   0        0        0     1472 2024-05-04 05:23:21.000000 AdroitFisherman-0.0.25/setup.py
```

### Comparing `AdroitFisherman-0.0.24/AdroitFisherman/Utilities/SequentialList.py` & `AdroitFisherman-0.0.25/AdroitFisherman/Utilities/SequentialList.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.24/AdroitFisherman/Utilities/SingleLinkedList.py` & `AdroitFisherman-0.0.25/AdroitFisherman/Utilities/SingleLinkedList.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.24/AdroitFisherman/includes/SeqList.c` & `AdroitFisherman-0.0.25/AdroitFisherman/includes/SeqList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.24/AdroitFisherman/includes/SeqList.h` & `AdroitFisherman-0.0.25/AdroitFisherman/includes/SeqList.h`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 }
 static PyMemberDef SeqList_members[] = {
     {"elem",T_OBJECT,offsetof(SeqList,elem),0,""},
     {"length",T_INT,offsetof(SeqList,length),0,""},
     {"size",T_INT,offsetof(SeqList,size),0,""},
     {NULL}
 };
-static PyObject* InitList(SeqList* self, PyObject* args, PyObject* kwds)
+static PyObject* InitList(SeqList* self, PyObject* args)
 {
     int size;
     if (PyArg_ParseTuple(args, "i", &size) < 0)
     {
         Py_RETURN_FALSE;
     }
     else
```

### Comparing `AdroitFisherman-0.0.24/AdroitFisherman/includes/SingleLinkedList.c` & `AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.24/AdroitFisherman/includes/SingleLinkedList.h` & `AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedList.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #ifndef SINGLELINKEDLIST_INCLUDED
 #define SINGLELINKEDLIST_INCLUDED
 typedef PyObject* ElemType;
 typedef struct Node
 {
+    PyObject_HEAD
     ElemType elem;
     struct Node* next;
 }LNode;
 typedef struct {
+    PyObject_HEAD
     LNode* instance;
 }List;
 static void LNode_destroy(LNode* self)
 {
     Py_DECREF(self->elem);
     Py_DECREF(self->next);
     Py_TYPE(self)->tp_free(self);
 }
 static void List_destroy(List* self)
 {
     Py_DECREF(self->instance);
     Py_TYPE(self)->tp_free(self);
 }
-static PyObject* LNode_new(PyTypeObject* type,PyObject* args,PyObject* kwds)
+static PyObject* LNode_new(PyTypeObject* type,PyObject* args)
 {
     LNode* self;
     self = (LNode*)type->tp_alloc(type,0);
     if (self==NULL)
     {
         PyErr_SetString(PyExc_Exception, "list node object created failure!");
         return NULL;
```

### Comparing `AdroitFisherman-0.0.24/AdroitFisherman.egg-info/PKG-INFO` & `AdroitFisherman-0.0.25/AdroitFisherman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: AdroitFisherman
-Version: 0.0.24
+Version: 0.0.25
 Summary: This is a simple package about Data Structure packed by C/C++ language.
 Home-page: UNKNOWN
 Author: adroit_fisherman
 Author-email: 1295284735@qq.com
 License: UNKNOWN
 Platform: Windows
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 
 # 总览
 ## 安装
 ```
 pip install AdroitFisherman
```

### Comparing `AdroitFisherman-0.0.24/AdroitFisherman.egg-info/SOURCES.txt` & `AdroitFisherman-0.0.25/AdroitFisherman.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -5,16 +5,21 @@
 AdroitFisherman/__init__.py
 AdroitFisherman.egg-info/PKG-INFO
 AdroitFisherman.egg-info/SOURCES.txt
 AdroitFisherman.egg-info/dependency_links.txt
 AdroitFisherman.egg-info/top_level.txt
 AdroitFisherman/includes/SeqList.c
 AdroitFisherman/includes/SingleLinkedList.c
+AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
 AdroitFisherman/Utilities/SequentialList.py
 AdroitFisherman/Utilities/SingleLinkedList.py
+AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py
 AdroitFisherman/Utilities/__init__.py
+AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc
 AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
 AdroitFisherman/__pycache__/__init__.cpython-310.pyc
 AdroitFisherman/includes/SeqList.c
 AdroitFisherman/includes/SeqList.h
 AdroitFisherman/includes/SingleLinkedList.c
-AdroitFisherman/includes/SingleLinkedList.h
+AdroitFisherman/includes/SingleLinkedList.h
+AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
+AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h
```

### Comparing `AdroitFisherman-0.0.24/PKG-INFO` & `AdroitFisherman-0.0.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: AdroitFisherman
-Version: 0.0.24
+Version: 0.0.25
 Summary: This is a simple package about Data Structure packed by C/C++ language.
 Home-page: UNKNOWN
 Author: adroit_fisherman
 Author-email: 1295284735@qq.com
 License: UNKNOWN
 Platform: Windows
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 
 # 总览
 ## 安装
 ```
 pip install AdroitFisherman
```

### Comparing `AdroitFisherman-0.0.24/README.md` & `AdroitFisherman-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.24/setup.py` & `AdroitFisherman-0.0.25/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from setuptools import setup,Extension
 SeqList=Extension("AdroitFisherman.SequentialList",sources=['AdroitFisherman/includes/SeqList.c'])
 SingleLinkedList=Extension("AdroitFisherman.SingleLinkedList",sources=['AdroitFisherman/includes/SingleLinkedList.c'])
+SingleLinkedListWithoutHeadNode=Extension("AdroitFisherman.SingleLinkedListWithoutHeadNode",sources=['AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c'])
 read_me = open('README.md', 'r',encoding='utf-8')
 setup(
     name="AdroitFisherman",
-    version="0.0.24",
+    version="0.0.25",
     author="adroit_fisherman",
     author_email="1295284735@qq.com",
     platforms="Windows",
     description="This is a simple package about Data Structure packed by C/C++ language.",
     long_description_content_type="text/markdown",
     long_description=read_me.read(),
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Natural Language :: Chinese (Simplified)",
         "Operating System :: Microsoft :: Windows :: Windows 10",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Programming Language :: C++",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.9",
         "Topic :: Utilities"
     ],
     include_package_data=True,
     packages=['AdroitFisherman.Utilities'],
-    ext_modules=[SeqList,SingleLinkedList]
+    ext_modules=[SeqList,SingleLinkedList,SingleLinkedListWithoutHeadNode]
 )
 read_me.close()
```

