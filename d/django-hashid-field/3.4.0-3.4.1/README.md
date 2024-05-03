# Comparing `tmp/django-hashid-field-3.4.0.tar.gz` & `tmp/django-hashid-field-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hashid-field-3.4.0.tar", last modified: Tue Jan  9 21:42:15 2024, max compression
+gzip compressed data, was "django-hashid-field-3.4.1.tar", last modified: Fri May  3 22:31:00 2024, max compression
```

## Comparing `django-hashid-field-3.4.0.tar` & `django-hashid-field-3.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-01-09 21:42:15.042187 django-hashid-field-3.4.0/
--rw-rw-r--   0 nate      (1000) nate      (1000)     1075 2020-01-14 22:19:25.000000 django-hashid-field-3.4.0/LICENSE
--rw-rw-r--   0 nate      (1000) nate      (1000)    23834 2024-01-09 21:42:15.042465 django-hashid-field-3.4.0/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)    22939 2024-01-09 21:28:37.000000 django-hashid-field-3.4.0/README.rst
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-01-09 21:42:15.032137 django-hashid-field-3.4.0/django_hashid_field.egg-info/
--rw-rw-r--   0 nate      (1000) nate      (1000)    23834 2024-01-09 21:42:14.000000 django-hashid-field-3.4.0/django_hashid_field.egg-info/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)      587 2024-01-09 21:42:15.000000 django-hashid-field-3.4.0/django_hashid_field.egg-info/SOURCES.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)        1 2024-01-09 21:42:14.000000 django-hashid-field-3.4.0/django_hashid_field.egg-info/dependency_links.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       28 2024-01-09 21:42:14.000000 django-hashid-field-3.4.0/django_hashid_field.egg-info/requires.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       13 2024-01-09 21:42:14.000000 django-hashid-field-3.4.0/django_hashid_field.egg-info/top_level.txt
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-01-09 21:42:15.037626 django-hashid-field-3.4.0/hashid_field/
--rw-rw-r--   0 nate      (1000) nate      (1000)      318 2024-01-09 21:27:41.000000 django-hashid-field-3.4.0/hashid_field/__init__.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      941 2022-12-12 18:34:03.000000 django-hashid-field-3.4.0/hashid_field/conf.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     1817 2022-12-12 18:34:03.000000 django-hashid-field-3.4.0/hashid_field/descriptor.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     9490 2022-12-12 18:34:03.000000 django-hashid-field-3.4.0/hashid_field/field.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     6757 2022-10-11 21:59:09.000000 django-hashid-field-3.4.0/hashid_field/hashid.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     7245 2023-09-05 23:28:51.000000 django-hashid-field-3.4.0/hashid_field/lookups.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     4085 2022-06-17 15:53:26.000000 django-hashid-field-3.4.0/hashid_field/rest.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      634 2022-02-11 22:48:16.000000 django-hashid-field-3.4.0/hashid_field/validators.py
--rw-rw-r--   0 nate      (1000) nate      (1000)       67 2024-01-09 21:42:15.042873 django-hashid-field-3.4.0/setup.cfg
--rw-rw-r--   0 nate      (1000) nate      (1000)     5105 2024-01-09 21:21:04.000000 django-hashid-field-3.4.0/setup.py
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-01-09 21:42:15.041684 django-hashid-field-3.4.0/tests/
--rw-r--r--   0 nate      (1000) nate      (1000)      620 2018-02-23 18:15:28.000000 django-hashid-field-3.4.0/tests/test_admin.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     3042 2022-12-12 18:34:03.000000 django-hashid-field-3.4.0/tests/test_descriptor.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     5895 2022-10-11 21:59:09.000000 django-hashid-field-3.4.0/tests/test_hashid.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    27471 2023-09-05 23:28:51.000000 django-hashid-field-3.4.0/tests/test_hashids_field.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     9295 2022-02-11 23:15:04.000000 django-hashid-field-3.4.0/tests/test_rest_framework.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     1145 2022-02-11 23:22:07.000000 django-hashid-field-3.4.0/tests/test_settings.py
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-03 22:31:00.433093 django-hashid-field-3.4.1/
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1075 2020-01-14 22:19:25.000000 django-hashid-field-3.4.1/LICENSE
+-rw-rw-r--   0 nate      (1000) nate      (1000)    26020 2024-05-03 22:31:00.433393 django-hashid-field-3.4.1/PKG-INFO
+-rw-rw-r--   0 nate      (1000) nate      (1000)    25125 2024-05-03 22:30:11.000000 django-hashid-field-3.4.1/README.rst
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-03 22:31:00.424502 django-hashid-field-3.4.1/django_hashid_field.egg-info/
+-rw-rw-r--   0 nate      (1000) nate      (1000)    26020 2024-05-03 22:31:00.000000 django-hashid-field-3.4.1/django_hashid_field.egg-info/PKG-INFO
+-rw-rw-r--   0 nate      (1000) nate      (1000)      587 2024-05-03 22:31:00.000000 django-hashid-field-3.4.1/django_hashid_field.egg-info/SOURCES.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)        1 2024-05-03 22:31:00.000000 django-hashid-field-3.4.1/django_hashid_field.egg-info/dependency_links.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)       28 2024-05-03 22:31:00.000000 django-hashid-field-3.4.1/django_hashid_field.egg-info/requires.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)       13 2024-05-03 22:31:00.000000 django-hashid-field-3.4.1/django_hashid_field.egg-info/top_level.txt
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-03 22:31:00.428907 django-hashid-field-3.4.1/hashid_field/
+-rw-rw-r--   0 nate      (1000) nate      (1000)      318 2024-05-03 21:59:46.000000 django-hashid-field-3.4.1/hashid_field/__init__.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)      941 2022-12-12 18:34:03.000000 django-hashid-field-3.4.1/hashid_field/conf.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1817 2022-12-12 18:34:03.000000 django-hashid-field-3.4.1/hashid_field/descriptor.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     9490 2022-12-12 18:34:03.000000 django-hashid-field-3.4.1/hashid_field/field.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     6757 2022-10-11 21:59:09.000000 django-hashid-field-3.4.1/hashid_field/hashid.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     7665 2024-01-29 22:18:47.000000 django-hashid-field-3.4.1/hashid_field/lookups.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     4085 2022-06-17 15:53:26.000000 django-hashid-field-3.4.1/hashid_field/rest.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)      634 2022-02-11 22:48:16.000000 django-hashid-field-3.4.1/hashid_field/validators.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)       67 2024-05-03 22:31:00.433812 django-hashid-field-3.4.1/setup.cfg
+-rw-rw-r--   0 nate      (1000) nate      (1000)     5105 2024-01-29 22:17:35.000000 django-hashid-field-3.4.1/setup.py
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-03 22:31:00.432574 django-hashid-field-3.4.1/tests/
+-rw-r--r--   0 nate      (1000) nate      (1000)      620 2018-02-23 18:15:28.000000 django-hashid-field-3.4.1/tests/test_admin.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     3042 2022-12-12 18:34:03.000000 django-hashid-field-3.4.1/tests/test_descriptor.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     5895 2022-10-11 21:59:09.000000 django-hashid-field-3.4.1/tests/test_hashid.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)    29161 2024-01-29 22:18:47.000000 django-hashid-field-3.4.1/tests/test_hashids_field.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     9295 2022-02-11 23:15:04.000000 django-hashid-field-3.4.1/tests/test_rest_framework.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1145 2022-02-11 23:22:07.000000 django-hashid-field-3.4.1/tests/test_settings.py
```

### Comparing `django-hashid-field-3.4.0/LICENSE` & `django-hashid-field-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/PKG-INFO` & `django-hashid-field-3.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hashid-field
-Version: 3.4.0
+Version: 3.4.1
 Summary: A Hashids obfuscated Django Model Field
 Home-page: https://github.com/nshafer/django-hashid-field
 Author: Nathan Shafer
 Author-email: nate-pypi@lotech.org
 License: MIT
 Keywords: django hashids hashid
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,16 +23,24 @@
 License-File: LICENSE
 
 .. image:: https://github.com/nshafer/django-hashid-field/actions/workflows/tests.yml/badge.svg?branch=master
     :target: https://github.com/nshafer/django-hashid-field/actions/workflows/tests.yml?query=branch%3Amaster
 .. image:: https://badge.fury.io/py/django-hashid-field.svg
     :target: https://badge.fury.io/py/django-hashid-field
 
+WARNING! This module is retired!
+================================
+
+**This library has been retired. It is no longer recommended for new projects. Existing projects do not require**
+**changes, but should consider migrating to a different library. See the**
+`RETIRED <https://github.com/nshafer/django-hashid-field/blob/master/RETIRED.md>`_
+**document for more information.**
+
 Django Hashid Field
-====================
+===================
 
 A custom Model Field that uses the `Hashids <http://hashids.org/>`_ `library <https://pypi.python.org/pypi/hashids/>`_
 to obfuscate an IntegerField or AutoField. It can be used in new models or dropped in place of an existing IntegerField,
 explicit AutoField, or an automatically generated AutoField.
 
 Features
 --------
@@ -226,14 +234,28 @@
     DEFAULT_AUTO_FIELD = 'hashid_field.HashidAutoField'
     DEFAULT_AUTO_FIELD = 'hashid_field.BigHashidAutoField'
 
 Care must be given, as this will alter ALL models in your project. Usually you would only set this in a new project.
 Also, since this changes the auto-generated field, only global settings will be used for that field. If you desire
 specific settings for different models, then using this setting is not advised.
 
+Django may configure the per-app `default_auto_field` when a new app is created. This will prevent the global setting
+from taking affect. If you are attempting to use the global setting, you should check your app configs in
+`project/app_name/apps.py` to ensure they don't interfere.
+
+.. code-block:: python
+
+    from django.apps import AppConfig
+
+
+    class ScheduleConfig(AppConfig):
+        default_auto_field = 'django.db.models.BigAutoField'
+        name = 'schedule'
+
+
 Global Settings
 ---------------
 
 HASHID_FIELD_SALT
 ~~~~~~~~~~~~~~~~~
 
 You can optionally set a global Salt to be used by all HashFields and HashidAutoFields in your project. Do not use the
@@ -413,21 +435,24 @@
 
 prefix
 ~~~~~~
 
 An optional string prefix that will be prepended to all generated hashids. Also affects validation, so only hashids
 that have this prefix will be considered correct.
 
+IMPORTANT: Do not end your prefix with an underscore, as this can cause issues with the Django admin. See Known Issues
+below.
+
 :Type:    String
 :Default: ""
 :Example:
     .. code-block:: python
 
         # Including the type of id in the id itself:
-        reference_id = HashidField(prefix="order_")
+        reference_id = HashidField(prefix="order-")
 
 allow_int_lookup
 ~~~~~~~~~~~~~~~~
 
 Local field override for default global on whether or not integer lookups for this field should be allowed.
 See HASHID_FIELD_ALLOW_INT_LOOKUP above.
 
@@ -632,18 +657,36 @@
 
 *Please Note*: This field will always serialize to an integer and thus will also de-serialize integers into valid
 objects, regardless of the `allow_int_lookup` setting.
 
 Known Issues
 ============
 
+'Hashid' object is not iterable
+-------------------------------
+
 With Django 5.0, attempting to filter on a field that is a ForeignKey to another model that uses a Hashid*Field as its
 primary key will result in an error such as "'Hashid' object is not iterable". The workaround is to specify the exact
 field of the related model to filter on. e.g. instead of `list_filter = ['author']` use `list_filter = ['author__name']`.
 
+Admin can't find objects with a prefix that ends in an underscore
+-----------------------------------------------------------------
+
+The Django admin has a `quote` and `unquote` function that attempts to encode non-alphanumeric characters in primary
+keys using the format of `_xx` where `xx` is the hex value of the character. This can be a problem if you are using
+a prefix that ends in an underscore, as there's a chance that your Hashid primary key will be something like,
+"user_3Ej8Kjm". The Django admin will attempt to `unquote` that to "user>j8Kjm" by swapping the "_3E" with a ">"
+character, but that isn't valid and so it can't find the object. It will throw an error like, "Admin Object with id
+'prefix<2345678' doesn't exist. Perhaps it was deleted?"
+
+The workaround is to not use a prefix that ends in an underscore. You can end it with a character right after the
+underscore that can't be used in hexidecimal, though, so it still looks right. e.g. `prefix="user_g"` so that the above
+example would actually be "user_g3Ej8Kjm", and "_3E" can't be matched. Or you can use any other character, such as
+a hyphen, .e.g `prefix="user-"`.
+
 Development
 ===========
 
 Here are some rough instructions on how to set up a dev environment to develop this module. Modify as needed. The
 sandbox is a django project that uses django-hashid-id, and is useful for developing features with.
 
 - ``git clone https://github.com/nshafer/django-hashid-field.git && cd django-hashid-field``
```

### Comparing `django-hashid-field-3.4.0/README.rst` & `django-hashid-field-3.4.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 .. image:: https://github.com/nshafer/django-hashid-field/actions/workflows/tests.yml/badge.svg?branch=master
     :target: https://github.com/nshafer/django-hashid-field/actions/workflows/tests.yml?query=branch%3Amaster
 .. image:: https://badge.fury.io/py/django-hashid-field.svg
     :target: https://badge.fury.io/py/django-hashid-field
 
+WARNING! This module is retired!
+================================
+
+**This library has been retired. It is no longer recommended for new projects. Existing projects do not require**
+**changes, but should consider migrating to a different library. See the**
+`RETIRED <https://github.com/nshafer/django-hashid-field/blob/master/RETIRED.md>`_
+**document for more information.**
+
 Django Hashid Field
-====================
+===================
 
 A custom Model Field that uses the `Hashids <http://hashids.org/>`_ `library <https://pypi.python.org/pypi/hashids/>`_
 to obfuscate an IntegerField or AutoField. It can be used in new models or dropped in place of an existing IntegerField,
 explicit AutoField, or an automatically generated AutoField.
 
 Features
 --------
@@ -202,14 +210,28 @@
     DEFAULT_AUTO_FIELD = 'hashid_field.HashidAutoField'
     DEFAULT_AUTO_FIELD = 'hashid_field.BigHashidAutoField'
 
 Care must be given, as this will alter ALL models in your project. Usually you would only set this in a new project.
 Also, since this changes the auto-generated field, only global settings will be used for that field. If you desire
 specific settings for different models, then using this setting is not advised.
 
+Django may configure the per-app `default_auto_field` when a new app is created. This will prevent the global setting
+from taking affect. If you are attempting to use the global setting, you should check your app configs in
+`project/app_name/apps.py` to ensure they don't interfere.
+
+.. code-block:: python
+
+    from django.apps import AppConfig
+
+
+    class ScheduleConfig(AppConfig):
+        default_auto_field = 'django.db.models.BigAutoField'
+        name = 'schedule'
+
+
 Global Settings
 ---------------
 
 HASHID_FIELD_SALT
 ~~~~~~~~~~~~~~~~~
 
 You can optionally set a global Salt to be used by all HashFields and HashidAutoFields in your project. Do not use the
@@ -389,21 +411,24 @@
 
 prefix
 ~~~~~~
 
 An optional string prefix that will be prepended to all generated hashids. Also affects validation, so only hashids
 that have this prefix will be considered correct.
 
+IMPORTANT: Do not end your prefix with an underscore, as this can cause issues with the Django admin. See Known Issues
+below.
+
 :Type:    String
 :Default: ""
 :Example:
     .. code-block:: python
 
         # Including the type of id in the id itself:
-        reference_id = HashidField(prefix="order_")
+        reference_id = HashidField(prefix="order-")
 
 allow_int_lookup
 ~~~~~~~~~~~~~~~~
 
 Local field override for default global on whether or not integer lookups for this field should be allowed.
 See HASHID_FIELD_ALLOW_INT_LOOKUP above.
 
@@ -608,18 +633,36 @@
 
 *Please Note*: This field will always serialize to an integer and thus will also de-serialize integers into valid
 objects, regardless of the `allow_int_lookup` setting.
 
 Known Issues
 ============
 
+'Hashid' object is not iterable
+-------------------------------
+
 With Django 5.0, attempting to filter on a field that is a ForeignKey to another model that uses a Hashid*Field as its
 primary key will result in an error such as "'Hashid' object is not iterable". The workaround is to specify the exact
 field of the related model to filter on. e.g. instead of `list_filter = ['author']` use `list_filter = ['author__name']`.
 
+Admin can't find objects with a prefix that ends in an underscore
+-----------------------------------------------------------------
+
+The Django admin has a `quote` and `unquote` function that attempts to encode non-alphanumeric characters in primary
+keys using the format of `_xx` where `xx` is the hex value of the character. This can be a problem if you are using
+a prefix that ends in an underscore, as there's a chance that your Hashid primary key will be something like,
+"user_3Ej8Kjm". The Django admin will attempt to `unquote` that to "user>j8Kjm" by swapping the "_3E" with a ">"
+character, but that isn't valid and so it can't find the object. It will throw an error like, "Admin Object with id
+'prefix<2345678' doesn't exist. Perhaps it was deleted?"
+
+The workaround is to not use a prefix that ends in an underscore. You can end it with a character right after the
+underscore that can't be used in hexidecimal, though, so it still looks right. e.g. `prefix="user_g"` so that the above
+example would actually be "user_g3Ej8Kjm", and "_3E" can't be matched. Or you can use any other character, such as
+a hyphen, .e.g `prefix="user-"`.
+
 Development
 ===========
 
 Here are some rough instructions on how to set up a dev environment to develop this module. Modify as needed. The
 sandbox is a django project that uses django-hashid-id, and is useful for developing features with.
 
 - ``git clone https://github.com/nshafer/django-hashid-field.git && cd django-hashid-field``
```

### Comparing `django-hashid-field-3.4.0/django_hashid_field.egg-info/PKG-INFO` & `django-hashid-field-3.4.1/django_hashid_field.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hashid-field
-Version: 3.4.0
+Version: 3.4.1
 Summary: A Hashids obfuscated Django Model Field
 Home-page: https://github.com/nshafer/django-hashid-field
 Author: Nathan Shafer
 Author-email: nate-pypi@lotech.org
 License: MIT
 Keywords: django hashids hashid
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,16 +23,24 @@
 License-File: LICENSE
 
 .. image:: https://github.com/nshafer/django-hashid-field/actions/workflows/tests.yml/badge.svg?branch=master
     :target: https://github.com/nshafer/django-hashid-field/actions/workflows/tests.yml?query=branch%3Amaster
 .. image:: https://badge.fury.io/py/django-hashid-field.svg
     :target: https://badge.fury.io/py/django-hashid-field
 
+WARNING! This module is retired!
+================================
+
+**This library has been retired. It is no longer recommended for new projects. Existing projects do not require**
+**changes, but should consider migrating to a different library. See the**
+`RETIRED <https://github.com/nshafer/django-hashid-field/blob/master/RETIRED.md>`_
+**document for more information.**
+
 Django Hashid Field
-====================
+===================
 
 A custom Model Field that uses the `Hashids <http://hashids.org/>`_ `library <https://pypi.python.org/pypi/hashids/>`_
 to obfuscate an IntegerField or AutoField. It can be used in new models or dropped in place of an existing IntegerField,
 explicit AutoField, or an automatically generated AutoField.
 
 Features
 --------
@@ -226,14 +234,28 @@
     DEFAULT_AUTO_FIELD = 'hashid_field.HashidAutoField'
     DEFAULT_AUTO_FIELD = 'hashid_field.BigHashidAutoField'
 
 Care must be given, as this will alter ALL models in your project. Usually you would only set this in a new project.
 Also, since this changes the auto-generated field, only global settings will be used for that field. If you desire
 specific settings for different models, then using this setting is not advised.
 
+Django may configure the per-app `default_auto_field` when a new app is created. This will prevent the global setting
+from taking affect. If you are attempting to use the global setting, you should check your app configs in
+`project/app_name/apps.py` to ensure they don't interfere.
+
+.. code-block:: python
+
+    from django.apps import AppConfig
+
+
+    class ScheduleConfig(AppConfig):
+        default_auto_field = 'django.db.models.BigAutoField'
+        name = 'schedule'
+
+
 Global Settings
 ---------------
 
 HASHID_FIELD_SALT
 ~~~~~~~~~~~~~~~~~
 
 You can optionally set a global Salt to be used by all HashFields and HashidAutoFields in your project. Do not use the
@@ -413,21 +435,24 @@
 
 prefix
 ~~~~~~
 
 An optional string prefix that will be prepended to all generated hashids. Also affects validation, so only hashids
 that have this prefix will be considered correct.
 
+IMPORTANT: Do not end your prefix with an underscore, as this can cause issues with the Django admin. See Known Issues
+below.
+
 :Type:    String
 :Default: ""
 :Example:
     .. code-block:: python
 
         # Including the type of id in the id itself:
-        reference_id = HashidField(prefix="order_")
+        reference_id = HashidField(prefix="order-")
 
 allow_int_lookup
 ~~~~~~~~~~~~~~~~
 
 Local field override for default global on whether or not integer lookups for this field should be allowed.
 See HASHID_FIELD_ALLOW_INT_LOOKUP above.
 
@@ -632,18 +657,36 @@
 
 *Please Note*: This field will always serialize to an integer and thus will also de-serialize integers into valid
 objects, regardless of the `allow_int_lookup` setting.
 
 Known Issues
 ============
 
+'Hashid' object is not iterable
+-------------------------------
+
 With Django 5.0, attempting to filter on a field that is a ForeignKey to another model that uses a Hashid*Field as its
 primary key will result in an error such as "'Hashid' object is not iterable". The workaround is to specify the exact
 field of the related model to filter on. e.g. instead of `list_filter = ['author']` use `list_filter = ['author__name']`.
 
+Admin can't find objects with a prefix that ends in an underscore
+-----------------------------------------------------------------
+
+The Django admin has a `quote` and `unquote` function that attempts to encode non-alphanumeric characters in primary
+keys using the format of `_xx` where `xx` is the hex value of the character. This can be a problem if you are using
+a prefix that ends in an underscore, as there's a chance that your Hashid primary key will be something like,
+"user_3Ej8Kjm". The Django admin will attempt to `unquote` that to "user>j8Kjm" by swapping the "_3E" with a ">"
+character, but that isn't valid and so it can't find the object. It will throw an error like, "Admin Object with id
+'prefix<2345678' doesn't exist. Perhaps it was deleted?"
+
+The workaround is to not use a prefix that ends in an underscore. You can end it with a character right after the
+underscore that can't be used in hexidecimal, though, so it still looks right. e.g. `prefix="user_g"` so that the above
+example would actually be "user_g3Ej8Kjm", and "_3E" can't be matched. Or you can use any other character, such as
+a hyphen, .e.g `prefix="user-"`.
+
 Development
 ===========
 
 Here are some rough instructions on how to set up a dev environment to develop this module. Modify as needed. The
 sandbox is a django project that uses django-hashid-id, and is useful for developing features with.
 
 - ``git clone https://github.com/nshafer/django-hashid-field.git && cd django-hashid-field``
```

### Comparing `django-hashid-field-3.4.0/django_hashid_field.egg-info/SOURCES.txt` & `django-hashid-field-3.4.1/django_hashid_field.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/hashid_field/conf.py` & `django-hashid-field-3.4.1/hashid_field/conf.py`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/hashid_field/descriptor.py` & `django-hashid-field-3.4.1/hashid_field/descriptor.py`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/hashid_field/field.py` & `django-hashid-field-3.4.1/hashid_field/field.py`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/hashid_field/hashid.py` & `django-hashid-field-3.4.1/hashid_field/hashid.py`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/hashid_field/lookups.py` & `django-hashid-field-3.4.1/hashid_field/lookups.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import itertools
 
+import django
 from django.db.models.lookups import Lookup, GreaterThan, GreaterThanOrEqual, LessThan, LessThanOrEqual
 from django.utils.datastructures import OrderedSet
 from django.core.exceptions import EmptyResultSet
 
 from .hashid import Hashid
 from .conf import settings
 
@@ -76,14 +77,15 @@
                     raise
                 raise EmptyResultSet
             return '%s', [lookup_id]
 
 
 class HashidExactLookup(HashidFieldGetDbPrepValueMixin, Lookup):
     prepare_rhs = False
+    lookup_name = 'exact'
 
     def as_sql(self, compiler, connection):
         lhs_sql, params = self.process_lhs(compiler, connection)
         rhs_sql, rhs_params = self.process_rhs(compiler, connection)
         params.extend(rhs_params)
         rhs_sql = self.get_rhs_op(connection, rhs_sql)
         return '%s %s' % (lhs_sql, rhs_sql), params
@@ -92,16 +94,25 @@
         return "= %s" % rhs
 
 
 class HashidIterableLookup(HashidExactLookup):
     # This is an amalgamation of Django's FieldGetDbPrepValueIterableMixin and In lookup to allow support of both
     # iterables (lists, tuples) and subqueries.
     get_db_prep_lookup_value_is_iterable = True
+    lookup_name = 'in'
 
     def get_prep_lookup(self):
+        from django.db.models.sql.query import Query  # avoid circular import
+        if isinstance(self.rhs, Query):
+            if django.VERSION > (4, 0):
+                self.rhs.clear_ordering(clear_default=True)
+            if not self.rhs.has_select_fields:
+                self.rhs.clear_select_clause()
+                self.rhs.add_fields(['pk'])
+
         if hasattr(self.rhs, 'resolve_expression'):
             return self.rhs
         prepared_values = []
         if hasattr(self.rhs, '_prepare'):
             # A subquery is like an iterable but its items shouldn't be
             # prepared independently.
             return self.rhs._prepare(self.lhs.output_field)
```

### Comparing `django-hashid-field-3.4.0/hashid_field/rest.py` & `django-hashid-field-3.4.1/hashid_field/rest.py`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/hashid_field/validators.py` & `django-hashid-field-3.4.1/hashid_field/validators.py`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/setup.py` & `django-hashid-field-3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/tests/test_admin.py` & `django-hashid-field-3.4.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/tests/test_descriptor.py` & `django-hashid-field-3.4.1/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/tests/test_hashid.py` & `django-hashid-field-3.4.1/tests/test_hashid.py`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/tests/test_hashids_field.py` & `django-hashid-field-3.4.1/tests/test_hashids_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.core import exceptions
 from django.core import validators as django_validators
 from django.core.management import call_command
+from django.db.models import Expression
 from django.shortcuts import get_object_or_404
 from django.test import TestCase, override_settings
 from io import StringIO
 
 from hashid_field import Hashid, HashidField
 from tests.forms import RecordForm, AlternateRecordForm
 from tests.models import Record, Artist, Track, RecordLabel
@@ -201,14 +202,22 @@
         a = Artist.objects.create(name="Artist A")
         b = Artist.objects.create(name="Artist B")
         c = Artist.objects.create(name="Artist C")
         queryset = Artist.objects.all()[:2]
         self.assertEqual(len(queryset), 2)
         self.assertEqual(len(Artist.objects.filter(id__in=queryset.values('id'))), 2)
 
+    def test_subquery_lookup_without_specified_values(self):
+        a = Artist.objects.create(name="Artist A")
+        b = Artist.objects.create(name="Artist B")
+        c = Artist.objects.create(name="Artist C")
+        queryset = Artist.objects.all()[:2]
+        self.assertEqual(len(queryset), 2)
+        self.assertEqual(len(Artist.objects.filter(id__in=queryset)), 2)
+
     def test_passthrough_lookups(self):
         # Test null lookups
         self.assertTrue(Record.objects.filter(alternate_id__isnull=True).exists())
         self.assertFalse(Record.objects.filter(alternate_id__isnull=False).exists())
 
         # Create some new objects to test with
         a = Artist.objects.create(name="Artist A")
@@ -249,14 +258,34 @@
         self.assertEqual(Artist.objects.filter(id__gt=a.id.id).count(), 2)
         self.assertEqual(Record.objects.filter(reference_id__gte=r1.reference_id.id).count(), 3)
         self.assertEqual(Artist.objects.filter(id__lt=999_999_999).count(), 3)
         self.assertEqual(Record.objects.filter(reference_id__lte=r3.reference_id.id).count(), 3)
         Artist._meta.get_field('id').allow_int_lookup = False
         Record._meta.get_field('reference_id').allow_int_lookup = False
 
+    def assert_lookup_name(self, model_field, lookup_val, expected_lookup_name):
+        # The below lookup is based on how django-filter FilterSet class implements `filter_for_field`
+        # using the utility `resolve_field` function.
+        lhs = Expression(model_field)
+        lookup = lhs.get_lookup(lookup_val)
+        self.assertEqual(lookup.lookup_name if lookup else None, expected_lookup_name)
+
+    def test_lookup_names(self):
+        # None will generally will use default behaviors. For example, in django-filter, if the lookup name cannot be
+        # determined the `DEFAULT_LOOKUP_EXPR` will be used.
+        self.assert_lookup_name(Artist._meta.get_field('id'), '', None)
+        self.assert_lookup_name(Artist._meta.get_field('id'), None, None)
+        # All other named types should match exactly.
+        self.assert_lookup_name(Artist._meta.get_field('id'), 'in', 'in')
+        self.assert_lookup_name(Artist._meta.get_field('id'), 'exact', 'exact')
+        self.assert_lookup_name(Artist._meta.get_field('id'), 'gt', 'gt')
+        self.assert_lookup_name(Artist._meta.get_field('id'), 'gte', 'gte')
+        self.assert_lookup_name(Artist._meta.get_field('id'), 'lt', 'lt')
+        self.assert_lookup_name(Artist._meta.get_field('id'), 'lte', 'lte')
+
     def test_int_lookup_with_made_entirely_of_numbers(self):
         # The integer id 428697 encodes to the hashids string "3557953" which looks like an integer.
         # Make sure we can still look up this record with ALLOW_INT_LOOKUPS off.
         r = Record.objects.create(reference_id=428697)
         a = Record.objects.get(reference_id=r.reference_id.hashid)
         self.assertEqual(r, a)
```

### Comparing `django-hashid-field-3.4.0/tests/test_rest_framework.py` & `django-hashid-field-3.4.1/tests/test_rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-hashid-field-3.4.0/tests/test_settings.py` & `django-hashid-field-3.4.1/tests/test_settings.py`

 * *Files identical despite different names*

