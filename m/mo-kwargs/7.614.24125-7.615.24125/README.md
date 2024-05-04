# Comparing `tmp/mo_kwargs-7.614.24125.tar.gz` & `tmp/mo_kwargs-7.615.24125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_kwargs-7.614.24125.tar", last modified: Sat May  4 13:41:35 2024, max compression
+gzip compressed data, was "mo_kwargs-7.615.24125.tar", last modified: Sat May  4 15:32:41 2024, max compression
```

## Comparing `mo_kwargs-7.614.24125.tar` & `mo_kwargs-7.615.24125.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 13:41:35.432830 mo_kwargs-7.614.24125/
--rw-rw-rw-   0        0        0    16725 2019-11-12 21:32:58.000000 mo_kwargs-7.614.24125/LICENSE
--rw-rw-rw-   0        0        0     5808 2024-05-04 13:41:35.432830 mo_kwargs-7.614.24125/PKG-INFO
--rw-rw-rw-   0        0        0     4577 2024-03-02 20:11:20.000000 mo_kwargs-7.614.24125/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 13:41:35.422455 mo_kwargs-7.614.24125/mo_kwargs/
--rw-rw-rw-   0        0        0     7048 2024-04-30 01:56:56.000000 mo_kwargs-7.614.24125/mo_kwargs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 13:41:35.430746 mo_kwargs-7.614.24125/mo_kwargs.egg-info/
--rw-rw-rw-   0        0        0     5808 2024-05-04 13:41:35.000000 mo_kwargs-7.614.24125/mo_kwargs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2024-05-04 13:41:35.000000 mo_kwargs-7.614.24125/mo_kwargs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 13:41:35.000000 mo_kwargs-7.614.24125/mo_kwargs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-30 01:03:59.000000 mo_kwargs-7.614.24125/mo_kwargs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      122 2024-05-04 13:41:35.000000 mo_kwargs-7.614.24125/mo_kwargs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 13:41:35.000000 mo_kwargs-7.614.24125/mo_kwargs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 13:41:35.433984 mo_kwargs-7.614.24125/setup.cfg
--rw-rw-rw-   0        0        0     5806 2024-05-04 13:41:29.000000 mo_kwargs-7.614.24125/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:32:41.343264 mo_kwargs-7.615.24125/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 21:32:58.000000 mo_kwargs-7.615.24125/LICENSE
+-rw-rw-rw-   0        0        0     5808 2024-05-04 15:32:41.341838 mo_kwargs-7.615.24125/PKG-INFO
+-rw-rw-rw-   0        0        0     4577 2024-03-02 20:11:20.000000 mo_kwargs-7.615.24125/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 15:32:41.330313 mo_kwargs-7.615.24125/mo_kwargs/
+-rw-rw-rw-   0        0        0     7048 2024-04-30 01:56:56.000000 mo_kwargs-7.615.24125/mo_kwargs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:32:41.339838 mo_kwargs-7.615.24125/mo_kwargs.egg-info/
+-rw-rw-rw-   0        0        0     5808 2024-05-04 15:32:41.000000 mo_kwargs-7.615.24125/mo_kwargs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-05-04 15:32:41.000000 mo_kwargs-7.615.24125/mo_kwargs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 15:32:41.000000 mo_kwargs-7.615.24125/mo_kwargs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-30 01:03:59.000000 mo_kwargs-7.615.24125/mo_kwargs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      122 2024-05-04 15:32:41.000000 mo_kwargs-7.615.24125/mo_kwargs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 15:32:41.000000 mo_kwargs-7.615.24125/mo_kwargs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 15:32:41.343873 mo_kwargs-7.615.24125/setup.cfg
+-rw-rw-rw-   0        0        0     5806 2024-05-04 15:32:35.000000 mo_kwargs-7.615.24125/setup.py
```

### Comparing `mo_kwargs-7.614.24125/LICENSE` & `mo_kwargs-7.615.24125/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_kwargs-7.614.24125/PKG-INFO` & `mo_kwargs-7.615.24125/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-kwargs
-Version: 7.614.24125
+Version: 7.615.24125
 Summary: Object destructuring of function parameters for Python!
 Home-page: https://github.com/klahnakoski/mo-kwargs
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==10.614.24125
+Requires-Dist: mo-dots==10.615.24125
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.610.24119; extra == "tests"
 Requires-Dist: mo-times>=5.609.24119; extra == "tests"
 Requires-Dist: mo-json>=6.609.24119; extra == "tests"
 Requires-Dist: mo-threads>=6.610.24119; extra == "tests"
```

### Comparing `mo_kwargs-7.614.24125/README.md` & `mo_kwargs-7.615.24125/README.md`

 * *Files identical despite different names*

### Comparing `mo_kwargs-7.614.24125/mo_kwargs/__init__.py` & `mo_kwargs-7.615.24125/mo_kwargs/__init__.py`

 * *Files identical despite different names*

### Comparing `mo_kwargs-7.614.24125/mo_kwargs.egg-info/PKG-INFO` & `mo_kwargs-7.615.24125/mo_kwargs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-kwargs
-Version: 7.614.24125
+Version: 7.615.24125
 Summary: Object destructuring of function parameters for Python!
 Home-page: https://github.com/klahnakoski/mo-kwargs
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==10.614.24125
+Requires-Dist: mo-dots==10.615.24125
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.610.24119; extra == "tests"
 Requires-Dist: mo-times>=5.609.24119; extra == "tests"
 Requires-Dist: mo-json>=6.609.24119; extra == "tests"
 Requires-Dist: mo-threads>=6.610.24119; extra == "tests"
```

### Comparing `mo_kwargs-7.614.24125/setup.py` & `mo_kwargs-7.615.24125/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='Object destructuring of function parameters for Python!',
     extras_require={"tests":["mo-testing>=8.610.24119","mo-times>=5.609.24119","mo-json>=6.609.24119","mo-threads>=6.610.24119"]},
     include_package_data=True,
-    install_requires=["mo-dots==10.614.24125"],
+    install_requires=["mo-dots==10.615.24125"],
     license='MPL 2.0',
     long_description='\n# More KWARGS!\n\nObject destructuring of function parameters for Python!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-kwargs.svg)](https://pypi.org/project/mo-kwargs/)\n [![Build Status](https://github.com/klahnakoski/mo-kwargs/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-kwargs/actions/workflows/build.yml)\n [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-kwargs/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-kwargs?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-kwargs)](https://pepy.tech/project/mo-kwargs)\n\n\n## Motivation\n\nJavascript has [object destructuring](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment#object_destructuring), and it can be used for function parameters. This has a couple of benefts over Python\'s keyword arguments:\n\n* Extra caller parameters are ignored (eg `f({a, b, c})`)\n* Duplicate parameters are handled elegantly (eg `f({a, a})`) \n\nThe `mo-kwargs` library provides this functionality with the `@override` decorator, with additional benefits:\n \n * required parameters throw an error if missing, just like regular Python\n * all parameters, even ones not in the argument list, are passed in the optional `kwargs` parameter \n \nThe `@override` decorator adds a `kwargs` argument which can be passed a dict of call parameters; but unlike `**kwargs`, it will not raise duplicate key exceptions.\n\n## Provide default values\n\nWe decorate the `login()` function with `@override`. `username` is a required parameter, and `password` will default to `None`. \n\n        @override\n        def login(username, password=None):\n            pass\n\nDefine some `dicts` for use with our `kwargs` parameter:\n\n        creds = {"userame": "ekyle", "password": "password123"}\n        alt_creds = {"username": "klahnakoski"}\n\n\nThe simplest case is when we use `kwargs` with no overrides\n\n        login(kwargs=creds)\n        # SAME AS\n        login(**creds)\n        # SAME AS\n        login(username="ekyle", password="password123")\n\nYou may override any property in `kwargs`: In this case it is `password`\n\n        login(password="123", kwargs=creds)\n        # SAME AS\n        login(username="ekyle", password="123")\n\nThere is no problem with overriding everything in `kwargs`:\n\n        login(username="klahnakoski", password="asd213", kwargs=creds)\n        # SAME AS\n        login(username="klahnakoski", password="asd213")\n\nYou may continue to use `**kwargs`; which provides a way to overlay one parameter template (`creds`) with another (`alt_creds`)\n\n        login(kwargs=creds, **alt_creds)\n        # SAME AS\n        login(username="klahnakoski", password="password123")\n\n## Handle too many parameters\n\nSometimes your method parameters come from a configuration file, or some other outside source which is outside your control. There may be more parameters than your method is willing to accept.  \n\n        creds = {"username": "ekyle", "password": "password123", "port":9000}\n        def login(username, password=None):\n             print(kwargs.get("port"))\n\nWithout `mo-kwargs`, passing the `creds` dictionary directly to `login()` would raise a key error\n\n        >>> login(**creds)\n        Traceback (most recent call last):\n          File "<stdin>", line 1, in <module>\n        TypeError: login() got an unexpected keyword argument \'port\'\n            \nThe traditional solution is to pass the parameters explicitly:\n\n        login(username=creds.username, password=creds.password)\n\nbut that can get get tedious when done often, or the parameter list get long. `mo-kwargs` allows you to pass the whole dictionary to the `kwargs` parameter; only the parameters used by the method are used:\n\n        @override\n        def login(username, password=None):\n            pass\n         \n        login(kwargs=creds)\n        # SAME AS\n        login(username=creds.username, password=creds.password)\n\n## Package all parameters\n\nYour method can accept `kwargs` as a parameter. If it does, ensure it defaults to `None` so that it\'s not required.\n\n        @override\n        def login(username, password=None, kwargs=None):\n            print(kwargs.get("username"))\n            print(kwargs.get("port"))\n\n`kwargs` will always be a dict, possibly empty, with the full set of parameters. This is different from using `**kwargs` which contains only the remainder of the keyword parameters.\n\n        >>> creds = {"username": "ekyle", "password": "password123", "port":9000}\n        >>> login(**creds)\n        ekyle\n        9000\n',
     long_description_content_type='text/markdown',
     name='mo-kwargs',
     packages=["mo_kwargs"],
     url='https://github.com/klahnakoski/mo-kwargs',
-    version='7.614.24125',
+    version='7.615.24125',
     zip_safe=False
 )
```

