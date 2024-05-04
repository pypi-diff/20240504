# Comparing `tmp/iothpy-1.3.0.tar.gz` & `tmp/iothpy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iothpy-1.3.0.tar", last modified: Tue Mar 26 14:34:30 2024, max compression
+gzip compressed data, was "iothpy-1.3.1.tar", last modified: Sat May  4 06:39:01 2024, max compression
```

## Comparing `iothpy-1.3.0.tar` & `iothpy-1.3.1.tar`

### file list

```diff
@@ -1,26 +1,37 @@
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-03-26 14:34:30.426581 iothpy-1.3.0/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      954 2024-03-26 14:33:52.000000 iothpy-1.3.0/CMakeLists.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    26526 2024-03-26 14:33:52.000000 iothpy-1.3.0/LICENSE
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      145 2024-03-26 14:33:52.000000 iothpy-1.3.0/MANIFEST.in
--rw-r--r--   0 francesco  (1000) francesco  (1000)     6516 2024-03-26 14:34:30.426581 iothpy-1.3.0/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6180 2024-03-26 14:33:52.000000 iothpy-1.3.0/README.md
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-03-26 14:34:30.422581 iothpy-1.3.0/iothpy/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2717 2024-03-26 14:33:52.000000 iothpy-1.3.0/iothpy/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7268 2024-03-26 14:33:52.000000 iothpy-1.3.0/iothpy/iothpy.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    78783 2024-03-26 14:33:52.000000 iothpy-1.3.0/iothpy/iothpy_socket.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      983 2024-03-26 14:33:52.000000 iothpy-1.3.0/iothpy/iothpy_socket.h
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    35491 2024-03-26 14:33:52.000000 iothpy-1.3.0/iothpy/iothpy_stack.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      260 2024-03-26 14:33:52.000000 iothpy-1.3.0/iothpy/iothpy_stack.h
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    14359 2024-03-26 14:33:52.000000 iothpy-1.3.0/iothpy/msocket.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2411 2024-03-26 14:33:52.000000 iothpy-1.3.0/iothpy/override.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4400 2024-03-26 14:33:52.000000 iothpy-1.3.0/iothpy/stack.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2892 2024-03-26 14:33:52.000000 iothpy-1.3.0/iothpy/utils.c
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      680 2024-03-26 14:33:52.000000 iothpy-1.3.0/iothpy/utils.h
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-03-26 14:34:30.426581 iothpy-1.3.0/iothpy.egg-info/
--rw-r--r--   0 francesco  (1000) francesco  (1000)     6516 2024-03-26 14:34:30.000000 iothpy-1.3.0/iothpy.egg-info/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      396 2024-03-26 14:34:30.000000 iothpy-1.3.0/iothpy.egg-info/SOURCES.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2024-03-26 14:34:30.000000 iothpy-1.3.0/iothpy.egg-info/dependency_links.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        7 2024-03-26 14:34:30.000000 iothpy-1.3.0/iothpy.egg-info/top_level.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       75 2024-03-26 14:33:52.000000 iothpy-1.3.0/pyproject.toml
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2024-03-26 14:34:30.426581 iothpy-1.3.0/setup.cfg
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1592 2024-03-26 14:33:52.000000 iothpy-1.3.0/setup.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.797777 iothpy-1.3.1/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1068 2024-05-04 06:34:10.000000 iothpy-1.3.1/CMakeLists.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    26526 2024-03-26 14:33:52.000000 iothpy-1.3.1/LICENSE
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      145 2024-03-26 14:33:52.000000 iothpy-1.3.1/MANIFEST.in
+-rw-r--r--   0 francesco  (1000) francesco  (1000)     6516 2024-05-04 06:39:01.797777 iothpy-1.3.1/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     6180 2024-03-26 14:33:52.000000 iothpy-1.3.1/README.md
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.781777 iothpy-1.3.1/_skbuild/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.781777 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.781777 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.789777 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2779 2024-05-04 06:31:09.000000 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/__init__.py
+-rw-r--r--   0 francesco  (1000) francesco  (1000)    87544 2024-05-04 06:31:09.000000 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/_const_linkadd.cpython-312-x86_64-linux-gnu.so
+-rw-r--r--   0 francesco  (1000) francesco  (1000)   193896 2024-05-04 06:31:09.000000 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/_iothpy.cpython-312-x86_64-linux-gnu.so
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    14359 2024-05-04 06:31:09.000000 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/msocket.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2411 2024-05-04 06:31:09.000000 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/override.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4400 2024-05-04 06:31:09.000000 iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/stack.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.793777 iothpy-1.3.1/iothpy/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2779 2024-05-04 06:34:10.000000 iothpy-1.3.1/iothpy/__init__.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    30003 2024-05-04 06:34:10.000000 iothpy-1.3.1/iothpy/const_linkadd.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     7268 2024-05-04 06:34:10.000000 iothpy-1.3.1/iothpy/iothpy.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    78783 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/iothpy_socket.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      983 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/iothpy_socket.h
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    38819 2024-05-04 06:34:10.000000 iothpy-1.3.1/iothpy/iothpy_stack.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      260 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/iothpy_stack.h
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    14359 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/msocket.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2411 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/override.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4400 2024-04-04 11:20:54.000000 iothpy-1.3.1/iothpy/stack.py
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     2892 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/utils.c
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      680 2024-03-26 14:33:52.000000 iothpy-1.3.1/iothpy/utils.h
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-04 06:39:01.797777 iothpy-1.3.1/iothpy.egg-info/
+-rw-r--r--   0 francesco  (1000) francesco  (1000)     6516 2024-05-04 06:39:01.000000 iothpy-1.3.1/iothpy.egg-info/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      838 2024-05-04 06:39:01.000000 iothpy-1.3.1/iothpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2024-05-04 06:39:01.000000 iothpy-1.3.1/iothpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        7 2024-05-04 06:39:01.000000 iothpy-1.3.1/iothpy.egg-info/top_level.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       75 2024-03-26 14:33:52.000000 iothpy-1.3.1/pyproject.toml
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2024-05-04 06:39:01.797777 iothpy-1.3.1/setup.cfg
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1592 2024-05-04 06:34:10.000000 iothpy-1.3.1/setup.py
```

### Comparing `iothpy-1.3.0/CMakeLists.txt` & `iothpy-1.3.1/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -26,8 +26,11 @@
 endforeach(HEADER)
 
 # Target for python extension module
 add_library(_iothpy MODULE iothpy/iothpy.c iothpy/iothpy_socket.c iothpy/iothpy_stack.c iothpy/utils.c)
 target_link_libraries(_iothpy -lioth -liothconf -liothdns)
 python_extension_module(_iothpy)
 
-install(TARGETS _iothpy LIBRARY DESTINATION iothpy)
+add_library(_const_linkadd MODULE iothpy/const_linkadd.c)
+python_extension_module(_const_linkadd)
+
+install(TARGETS _iothpy _const_linkadd LIBRARY DESTINATION iothpy)
```

### Comparing `iothpy-1.3.0/LICENSE` & `iothpy-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.0/PKG-INFO` & `iothpy-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iothpy
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python library for internet of threads
 Home-page: https://github.com/ramenguy99/iothpy
 Author: Dario Mylonopoulos
 Author-email: dmylos@yahoo.it
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `iothpy-1.3.0/README.md` & `iothpy-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.0/iothpy/__init__.py` & `iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,16 +61,20 @@
 # Import symbols to expose them at package scope
 # so they can be accessed with iothpy.name
 #
 
 # Import the Stack type
 from iothpy.stack import Stack
 
+# Import constants for ioth_linkadd
+from ._const_linkadd import *
+
 # Import functions from the c module
-from iothpy._iothpy import getdefaulttimeout, setdefaulttimeout, CMSG_LEN, CMSG_SPACE, close, timeout
+from ._iothpy import getdefaulttimeout, setdefaulttimeout, CMSG_LEN, CMSG_SPACE, close, timeout
+
 
 # Import the function to override the built-in socket module
 from iothpy.override import override_socket_module
 
 # Import functions and constants from the builtin socket module 
 from socket import (
     # Convertion utils
```

### Comparing `iothpy-1.3.0/iothpy/iothpy.c` & `iothpy-1.3.1/iothpy/iothpy.c`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 #include <sys/wait.h>
 #include <netinet/in.h>
 #include <pthread.h>
 #include <arpa/inet.h>
 
 #include <ioth.h>
 
+
 PyDoc_STRVAR(iothpy_doc,
 "_iothpy c module\n\
 \n\
 This module defines the base classes MSocketBase and StackBase\n\
 used to interface with the ioth c api. \n\
 It also defines the functions needed to offer the same interface as\n\
 the built-in socket module\n\
@@ -238,10 +239,9 @@
     }
 
     /* Add a symbol for the socket type */
     Py_INCREF((PyObject *)&socket_type);
     if (PyModule_AddObject(module, "MSocketBase",
                            (PyObject *)&socket_type) != 0)
         return NULL;
-
     return module;
 }
```

### Comparing `iothpy-1.3.0/iothpy/iothpy_socket.c` & `iothpy-1.3.1/iothpy/iothpy_socket.c`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.0/iothpy/iothpy_socket.h` & `iothpy-1.3.1/iothpy/iothpy_socket.h`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.0/iothpy/iothpy_stack.c` & `iothpy-1.3.1/iothpy/iothpy_stack.c`

 * *Files 3% similar despite different names*

```diff
@@ -37,18 +37,23 @@
 #include <sys/types.h>
 #include <sys/wait.h>
 #include <netinet/in.h>
 #include <pthread.h>
 #include <arpa/inet.h>
 #include <errno.h>
 
+#include <ioth.h>
+
+
 #define IS_PATH(str) (strchr(str, '/') != NULL)
 #define NI_MAXHOST 1025
 #define NI_MAXSERV 32
 
+static char* stackName = NULL;
+
 static void 
 stack_dealloc(stack_object* self)
 {
     if(PyObject_CallFinalizerFromDealloc((PyObject*)self) < 0) {
         return;
     }
 
@@ -132,22 +137,36 @@
     const char** multi_url_buf = NULL;
 
     if(!PyArg_ParseTuple(args, "s|Oz", &stack_name, &vdeurl, &config_dns)){
         PyErr_SetFromErrno(PyExc_OSError);
         return -1;
     }
 
+    
+
     if(stack_dns_init(s, config_dns) < 0) {
         PyErr_SetFromErrno(PyExc_OSError);
         return -1;
     }
 
     if(vdeurl == Py_None){
         /*stack interface in configuration string */
         s->stack = ioth_newstackc(stack_name);
+
+        if(!s->stack) {
+            PyErr_SetFromErrno(PyExc_OSError);
+            return -1;
+        }
+
+        //get stack name
+        char* stackString = strstr(stack_name, "stack=\0");
+        if(stackString){
+            strtok(stackString, "=");
+            stackName = strtok(NULL, "=");
+        }
     }
     else{
         /* check if vde url is a string or a list of strings */
         if(PyUnicode_Check(vdeurl)){
             single_url_buf[0] = PyUnicode_AsUTF8(vdeurl);
             single_url_buf[1] = 0;
             urls = single_url_buf;
@@ -178,22 +197,23 @@
             multi_url_buf[len] = 0;
             urls = multi_url_buf;
         }
 
 
         s->stack = ioth_newstackv(stack_name, urls);
         free(multi_url_buf);
+        stackName = stack_name;
     }
 
     if(!s->stack) {
         PyErr_SetFromErrno(PyExc_OSError);
         return -1;
     }
 
-
+    
 
     return 0;
 }
 
 
 PyDoc_STRVAR(if_nameindex_doc, "if_nameindex()\n\
 \n\
@@ -581,42 +601,123 @@
     Py_RETURN_NONE;
 }
 
 PyDoc_STRVAR(iplink_add_doc, "iplink_add(ifindex, type, data, ifname)\n\
 \n\
 This function adds a new link of type type,  named  ifname.  The\n\
 value of data depends on the type of link and can be optional. \n\
+Data is a list of tuple (tag, tag_data). \n\
 A default interface name is assigned if ifname is missing.  The  link  is\n\
 created with a given index when ifindex is positive.\n\
 \n\
 iplink_add can return the (positive)  ifindex  of  the  newly\n\
 created  link  when  the  argument ifindex is -1 and the stack supports\n\
 this feature.");
 
 static PyObject*
 stack_iplink_add(stack_object *self, PyObject *args){
     char* ifname = NULL;
     unsigned int ifindex;
     char* type;
-    char* data = NULL;
+    PyObject* data = NULL;
+    int nifd = - 1;
+    int newifindex;
+    struct nl_iplink_data* ifd = NULL;
+
+    if(!self->stack) 
+    {
+        PyErr_SetString(PyExc_Exception, "Uninitialized stack");
+        return NULL;
+    }
+
+    if(strcmp(stackName, "vdestack") == 0){
+        PyErr_SetString(PyExc_Exception, "Operation not supported by vdestack");
+        return NULL;
+    }
+
+    /* Parse arguments */
+    if(!PyArg_ParseTuple(args, "is|Os:iplink_add", &ifindex, &type, &data, &ifname)) {
+        return NULL;
+    }
+
+    if(PyList_Check(data)){
+        nifd = (int)PyList_Size(data);
+        ifd = (struct nl_iplink_data*) malloc(sizeof(struct nl_iplink_data) * nifd);
+
+        for(int i = 0; i < nifd; i++) {
+            PyObject* cur_tuple = PyList_GetItem(data, i);
+            if(!PyTuple_Check(cur_tuple)){
+                PyErr_SetString(PyExc_ValueError, "Data in list must be tuples");
+                return NULL;
+            }
+
+            PyObject* tag = PyTuple_GetItem(cur_tuple, 0);
+            PyObject* dataptr = PyTuple_GetItem(cur_tuple, 1);
 
+            ifd[i] = (struct nl_iplink_data) {(int) PyLong_AsLong(tag), sizeof(PyLong_AsVoidPtr(dataptr)) + 1, (PyLong_AsVoidPtr(dataptr))};
+        }
+
+    } else if(PyTuple_Check(data)){
+        nifd = 1;
+        ifd = (struct nl_iplink_data*) malloc(sizeof(struct nl_iplink_data) * nifd);
+
+        PyObject* tag = PyTuple_GetItem(data, 0);
+        PyObject* dataptr = PyTuple_GetItem(data, 1);
+
+        ifd[0] = (struct nl_iplink_data) {(int) PyLong_AsLong(tag), sizeof(PyLong_AsVoidPtr(dataptr)) + 1, (PyLong_AsVoidPtr(dataptr))};
+
+    } else {
+        PyErr_SetString(PyExc_ValueError, "Data must be list or tuple");
+        return NULL;
+    }
+
+    if((newifindex = ioth_iplink_add(self->stack, ifname, ifindex, type, ifd,  nifd)) < 0) {
+        PyErr_SetString(PyExc_Exception, "failed to add link");
+        return NULL;
+    }
+
+    return PyLong_FromLong(newifindex);
+}
+
+PyDoc_STRVAR(iplink_add_vde_doc, "iplink_add_vde(ifindex, vnl, ifname)\n\
+\n\
+This function adds a new link of type vde,  named  ifname.  The\n\
+vnl is the name of virtual network locator. \n\
+A default interface name is assigned if ifname is missing.  The  link  is\n\
+created with a given index when ifindex is positive.\n\
+\n\
+iplink_add can return the (positive)  ifindex  of  the  newly\n\
+created  link  when  the  argument ifindex is -1 and the stack supports\n\
+this feature.\n\
+It's a simplified version of iplink_add to use for vde vnl.");
+
+static PyObject*
+stack_iplink_add_vde(stack_object *self, PyObject *args){
+    char* ifname = NULL;
+    int ifindex;
+    char* vnl = NULL;
     int newifindex;
 
     if(!self->stack) 
     {
         PyErr_SetString(PyExc_Exception, "Uninitialized stack");
         return NULL;
     }
 
+    if(strcmp(stackName, "vdestack") == 0){
+        PyErr_SetString(PyExc_Exception, "Operation not supported by vdestack");
+        return NULL;
+    }
+
     /* Parse arguments */
-    if(!PyArg_ParseTuple(args, "is|ss:iplink_add", &ifindex, &type, &data, &ifname)) {
+    if(!PyArg_ParseTuple(args, "is|s:iplink_add_vde", &ifindex, &vnl, &ifname)) {
         return NULL;
     }
 
-     if((newifindex = ioth_iplink_add(self->stack, ifname, ifindex, type, data)) < 0) {
+    if((newifindex = ioth_iplink_add(self->stack, ifname, ifindex, "vde", nl_iplink_strdata(IFLA_VDE_VNL, vnl))) < 0) {
         PyErr_SetString(PyExc_Exception, "failed to add link");
         return NULL;
     }
 
     return PyLong_FromLong(newifindex);
 }
 
@@ -1067,14 +1168,15 @@
     {"if_nameindex", (PyCFunction)stack_if_nameindex, METH_NOARGS, if_nameindex_doc},
     {"if_nametoindex", (PyCFunction)stack_if_nametoindex, METH_VARARGS, if_nametoindex_doc},
     {"if_indextoname", (PyCFunction)stack_if_indextoname, METH_O, if_indextoname_doc},
 
     /* Network interface configuration */
     {"linksetupdown", (PyCFunction)stack_linksetupdown, METH_VARARGS, linksetupdown_doc},
     {"iplink_add", (PyCFunction)stack_iplink_add, METH_VARARGS, iplink_add_doc},
+    {"iplink_add_vde", (PyCFunction)stack_iplink_add_vde, METH_VARARGS, iplink_add_vde_doc},
     {"iplink_del", (PyCFunction)stack_iplink_del, METH_VARARGS | METH_KEYWORDS, iplink_del_doc},
 
     {"linkgetaddr", (PyCFunction)stack_linkgetaddr, METH_VARARGS, linkgetaddr_doc},
     {"_linksetaddr", (PyCFunction)stack_linksetaddr, METH_VARARGS, linksetaddr_doc},
     {"linksetmtu",  (PyCFunction)stack_linksetmtu,  METH_VARARGS, linksetmtu_doc},
 
     {"ipaddr_add", (PyCFunction)stack_ipaddr_add, METH_VARARGS, ipaddr_add_doc},
```

### Comparing `iothpy-1.3.0/iothpy/msocket.py` & `iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/msocket.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.0/iothpy/override.py` & `iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/override.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.0/iothpy/stack.py` & `iothpy-1.3.1/_skbuild/linux-x86_64-3.12/cmake-install/iothpy/stack.py`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.0/iothpy/utils.c` & `iothpy-1.3.1/iothpy/utils.c`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.0/iothpy/utils.h` & `iothpy-1.3.1/iothpy/utils.h`

 * *Files identical despite different names*

### Comparing `iothpy-1.3.0/iothpy.egg-info/PKG-INFO` & `iothpy-1.3.1/iothpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iothpy
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python library for internet of threads
 Home-page: https://github.com/ramenguy99/iothpy
 Author: Dario Mylonopoulos
 Author-email: dmylos@yahoo.it
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `iothpy-1.3.0/setup.py` & `iothpy-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 long_description = ""
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup (
        #setuptools options
        name = 'iothpy',
-       version = '1.3.0',
+       version = '1.3.1',
        author = 'Dario Mylonopoulos',
        author_email = 'dmylos@yahoo.it',
        url = 'https://github.com/ramenguy99/iothpy',
        description = 'Python library for internet of threads',
        long_description = long_description,
        long_description_content_type="text/markdown",
        packages = ["iothpy"],
```

