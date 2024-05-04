# Comparing `tmp/django-money-3.4.1.tar.gz` & `tmp/django_money-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-money-3.4.1.tar", last modified: Thu Nov 30 19:38:03 2023, max compression
+gzip compressed data, was "django_money-3.5.tar", last modified: Sat May  4 12:28:39 2024, max compression
```

## Comparing `django-money-3.4.1.tar` & `django_money-3.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.998169 django-money-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2023-11-30 19:37:55.000000 django-money-3.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-30 19:37:55.000000 django-money-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17464 2023-11-30 19:38:02.998169 django-money-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15705 2023-11-30 19:37:55.000000 django-money-3.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.994169 django-money-3.4.1/django_money.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17464 2023-11-30 19:38:02.000000 django-money-3.4.1/django_money.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-11-30 19:38:02.000000 django-money-3.4.1/django_money.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 19:38:02.000000 django-money-3.4.1/django_money.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-30 19:38:02.000000 django-money-3.4.1/django_money.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-30 19:38:02.000000 django-money-3.4.1/django_money.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.990168 django-money-3.4.1/djmoney/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.990168 django-money-3.4.1/djmoney/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.990168 django-money-3.4.1/djmoney/contrib/django_rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/django_rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/django_rest_framework/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.990168 django-money-3.4.1/djmoney/contrib/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.990168 django-money-3.4.1/djmoney/contrib/exchange/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/backends/fixer.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/backends/openexchangerates.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.990168 django-money-3.4.1/djmoney/contrib/exchange/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/management/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.990168 django-money-3.4.1/djmoney/contrib/exchange/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/management/commands/clear_rates.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/management/commands/update_rates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.990168 django-money-3.4.1/djmoney/contrib/exchange/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/contrib/exchange/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.990168 django-money-3.4.1/djmoney/forms/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.994169 django-money-3.4.1/djmoney/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13043 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/models/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/models/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/models/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/money.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/money.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.994169 django-money-3.4.1/djmoney/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/templatetags/djmoney.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-30 19:37:55.000000 django-money-3.4.1/djmoney/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-30 19:37:55.000000 django-money-3.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-11-30 19:38:02.998169 django-money-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2023-11-30 19:37:55.000000 django-money-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 19:38:02.994169 django-money-3.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-11-30 19:37:55.000000 django-money-3.4.1/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2023-11-30 19:37:55.000000 django-money-3.4.1/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2023-11-30 19:37:55.000000 django-money-3.4.1/tests/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    39496 2023-11-30 19:37:55.000000 django-money-3.4.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2023-11-30 19:37:55.000000 django-money-3.4.1/tests/test_money.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-11-30 19:37:55.000000 django-money-3.4.1/tests/test_reversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2023-11-30 19:37:55.000000 django-money-3.4.1/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-11-30 19:37:55.000000 django-money-3.4.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2023-11-30 19:37:55.000000 django-money-3.4.1/tests/test_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.882816 django_money-3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-04 12:28:30.000000 django_money-3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-04 12:28:30.000000 django_money-3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-05-04 12:28:39.882816 django_money-3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16571 2024-05-04 12:28:30.000000 django_money-3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.878816 django_money-3.5/django_money.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-05-04 12:28:39.000000 django_money-3.5/django_money.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-04 12:28:39.000000 django_money-3.5/django_money.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 12:28:39.000000 django_money-3.5/django_money.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 12:28:39.000000 django_money-3.5/django_money.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 12:28:39.000000 django_money-3.5/django_money.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.874816 django_money-3.5/djmoney/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.874816 django_money-3.5/djmoney/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.874816 django_money-3.5/djmoney/contrib/django_rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/django_rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/django_rest_framework/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.874816 django_money-3.5/djmoney/contrib/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.874816 django_money-3.5/djmoney/contrib/exchange/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/backends/fixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/backends/openexchangerates.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.874816 django_money-3.5/djmoney/contrib/exchange/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/management/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.874816 django_money-3.5/djmoney/contrib/exchange/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/management/commands/clear_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/management/commands/update_rates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.874816 django_money-3.5/djmoney/contrib/exchange/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/contrib/exchange/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.878816 django_money-3.5/djmoney/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.878816 django_money-3.5/djmoney/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/models/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/models/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/models/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/money.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/money.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.878816 django_money-3.5/djmoney/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/templatetags/djmoney.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-04 12:28:30.000000 django_money-3.5/djmoney/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-04 12:28:30.000000 django_money-3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-04 12:28:39.882816 django_money-3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-04 12:28:30.000000 django_money-3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:28:39.878816 django_money-3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-04 12:28:30.000000 django_money-3.5/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-04 12:28:30.000000 django_money-3.5/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-04 12:28:30.000000 django_money-3.5/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39497 2024-05-04 12:28:30.000000 django_money-3.5/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-04 12:28:30.000000 django_money-3.5/tests/test_money.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-04 12:28:30.000000 django_money-3.5/tests/test_reversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-04 12:28:30.000000 django_money-3.5/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-04 12:28:30.000000 django_money-3.5/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-04 12:28:30.000000 django_money-3.5/tests/test_tags.py
```

### Comparing `django-money-3.4.1/LICENSE.txt` & `django_money-3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/PKG-INFO` & `django_money-3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-money
-Version: 3.4.1
+Version: 3.5
 Summary: Adds support for using money and currency fields in django models and forms. Uses py-moneyed as the money implementation.
 Home-page: https://github.com/django-money/django-money
 Maintainer: Greg Reinbach
 Maintainer-email: greg@reinbach.com
 License: BSD
 Keywords: django,py-money,money
 Platform: Any
@@ -28,17 +28,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: setuptools
 Requires-Dist: Django>=2.2
 Requires-Dist: py-moneyed<3.1,>=2.0
 Provides-Extra: test
-Requires-Dist: pytest<7.0,>=3.1.0; extra == "test"
+Requires-Dist: pytest<8.3,>=8.2; extra == "test"
 Requires-Dist: pytest-django; extra == "test"
-Requires-Dist: pytest-pythonpath; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: mixer; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: django-stubs; extra == "test"
 Provides-Extra: exchange
 Requires-Dist: certifi; extra == "exchange"
 
@@ -180,14 +179,45 @@
 The ``balance`` field from the model above has the following validation:
 
 * All input values should be between 10 and 1500 despite on currency;
 * Norwegian Crowns amount (NOK) should be between 500 and 900;
 * Euros should be between 100 and 1000;
 * US Dollars should be between 50 and 500;
 
+Constructing form data
+----------------------
+
+The default ``ModelForm`` class will use a form field (``djmoney.forms.fields.MoneyField``) that is constructed of two separate fields for amount and currency.
+
+If you need to feed data directly to such a form (for instance if you are writing a test case), then you need to pass amount and currency like this:
+
+
+
+.. code:: python
+
+        # models.py
+        class Product(models.Model):
+            price = MoneyField(
+                max_digits=14,
+                decimal_places=2,
+                default_currency='EUR'
+            )
+
+        # forms.py
+        class ProductForm(ModelForm):
+            class Meta:
+                model = Product
+                fields = ["price"]
+
+        # tests.py
+
+        # construct the form in your test case
+        form = ProductForm({'price_0': 10, 'price_1': 'EUR'})
+
+
 Adding a new Currency
 ---------------------
 
 Currencies are listed on moneyed, and this modules use this to provide a
 choice list on the admin, also for validation.
 
 To add a new currency available on all the project, you can simply add
```

### Comparing `django-money-3.4.1/README.rst` & `django_money-3.5/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,45 @@
 The ``balance`` field from the model above has the following validation:
 
 * All input values should be between 10 and 1500 despite on currency;
 * Norwegian Crowns amount (NOK) should be between 500 and 900;
 * Euros should be between 100 and 1000;
 * US Dollars should be between 50 and 500;
 
+Constructing form data
+----------------------
+
+The default ``ModelForm`` class will use a form field (``djmoney.forms.fields.MoneyField``) that is constructed of two separate fields for amount and currency.
+
+If you need to feed data directly to such a form (for instance if you are writing a test case), then you need to pass amount and currency like this:
+
+
+
+.. code:: python
+
+        # models.py
+        class Product(models.Model):
+            price = MoneyField(
+                max_digits=14,
+                decimal_places=2,
+                default_currency='EUR'
+            )
+
+        # forms.py
+        class ProductForm(ModelForm):
+            class Meta:
+                model = Product
+                fields = ["price"]
+
+        # tests.py
+
+        # construct the form in your test case
+        form = ProductForm({'price_0': 10, 'price_1': 'EUR'})
+
+
 Adding a new Currency
 ---------------------
 
 Currencies are listed on moneyed, and this modules use this to provide a
 choice list on the admin, also for validation.
 
 To add a new currency available on all the project, you can simply add
```

### Comparing `django-money-3.4.1/django_money.egg-info/PKG-INFO` & `django_money-3.5/django_money.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-money
-Version: 3.4.1
+Version: 3.5
 Summary: Adds support for using money and currency fields in django models and forms. Uses py-moneyed as the money implementation.
 Home-page: https://github.com/django-money/django-money
 Maintainer: Greg Reinbach
 Maintainer-email: greg@reinbach.com
 License: BSD
 Keywords: django,py-money,money
 Platform: Any
@@ -28,17 +28,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: setuptools
 Requires-Dist: Django>=2.2
 Requires-Dist: py-moneyed<3.1,>=2.0
 Provides-Extra: test
-Requires-Dist: pytest<7.0,>=3.1.0; extra == "test"
+Requires-Dist: pytest<8.3,>=8.2; extra == "test"
 Requires-Dist: pytest-django; extra == "test"
-Requires-Dist: pytest-pythonpath; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: mixer; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: django-stubs; extra == "test"
 Provides-Extra: exchange
 Requires-Dist: certifi; extra == "exchange"
 
@@ -180,14 +179,45 @@
 The ``balance`` field from the model above has the following validation:
 
 * All input values should be between 10 and 1500 despite on currency;
 * Norwegian Crowns amount (NOK) should be between 500 and 900;
 * Euros should be between 100 and 1000;
 * US Dollars should be between 50 and 500;
 
+Constructing form data
+----------------------
+
+The default ``ModelForm`` class will use a form field (``djmoney.forms.fields.MoneyField``) that is constructed of two separate fields for amount and currency.
+
+If you need to feed data directly to such a form (for instance if you are writing a test case), then you need to pass amount and currency like this:
+
+
+
+.. code:: python
+
+        # models.py
+        class Product(models.Model):
+            price = MoneyField(
+                max_digits=14,
+                decimal_places=2,
+                default_currency='EUR'
+            )
+
+        # forms.py
+        class ProductForm(ModelForm):
+            class Meta:
+                model = Product
+                fields = ["price"]
+
+        # tests.py
+
+        # construct the form in your test case
+        form = ProductForm({'price_0': 10, 'price_1': 'EUR'})
+
+
 Adding a new Currency
 ---------------------
 
 Currencies are listed on moneyed, and this modules use this to provide a
 choice list on the admin, also for validation.
 
 To add a new currency available on all the project, you can simply add
```

### Comparing `django-money-3.4.1/django_money.egg-info/SOURCES.txt` & `django_money-3.5/django_money.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/_compat.py` & `django_money-3.5/djmoney/_compat.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/admin.py` & `django_money-3.5/djmoney/admin.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/contrib/django_rest_framework/fields.py` & `django_money-3.5/djmoney/contrib/django_rest_framework/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,16 +61,22 @@
                 return Money(amount, data.currency)
             except CurrencyDoesNotExist:
                 self.fail("invalid_currency", currency=data.currency)
 
         return super().to_internal_value(data)
 
     def get_value(self, data):
+        default_currency = None
+        if hasattr(self.parent, "Meta"):
+            model_meta = self.parent.Meta.model._meta
+            field = model_meta.get_field(self.field_name)
+            default_currency = field.default_currency
+
         amount = super().get_value(data)
-        currency = data.get(get_currency_field_name(self.field_name), self.default_currency)
+        currency = data.get(get_currency_field_name(self.field_name), self.default_currency or default_currency)
         if currency and amount is not None and not isinstance(amount, MONEY_CLASSES) and amount is not empty:
             return _PrimitiveMoney(amount=amount, currency=currency)
         return amount
 
 
 def register_money_field():
     ModelSerializer.serializer_field_mapping[ModelField] = MoneyField
```

### Comparing `django-money-3.4.1/djmoney/contrib/exchange/backends/base.py` & `django_money-3.5/djmoney/contrib/exchange/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/contrib/exchange/backends/fixer.py` & `django_money-3.5/djmoney/contrib/exchange/backends/fixer.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/contrib/exchange/backends/openexchangerates.py` & `django_money-3.5/djmoney/contrib/exchange/backends/openexchangerates.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/contrib/exchange/management/base.py` & `django_money-3.5/djmoney/contrib/exchange/management/base.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/contrib/exchange/management/commands/clear_rates.py` & `django_money-3.5/djmoney/contrib/exchange/management/commands/clear_rates.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/contrib/exchange/migrations/0001_initial.py` & `django_money-3.5/djmoney/contrib/exchange/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/contrib/exchange/models.py` & `django_money-3.5/djmoney/contrib/exchange/models.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/forms/fields.py` & `django_money-3.5/djmoney/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/forms/widgets.py` & `django_money-3.5/djmoney/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/models/fields.py` & `django_money-3.5/djmoney/models/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -251,15 +251,19 @@
         Default ``DecimalValidator`` doesn't work with ``Money`` instances.
         """
         return super(models.DecimalField, self).validators + [MoneyValidator(self.max_digits, self.decimal_places)]
 
     def contribute_to_class(self, cls, name):
         cls._meta.has_money_field = True
 
-        if not hasattr(self, "_currency_field") and not cls.__module__ == "__fake__":
+        # Note the discussion about whether or not the currency field should be added in migrations:
+        # https://github.com/django-money/django-money/issues/725
+        # https://github.com/django-money/django-money/pull/726
+        # https://github.com/django-money/django-money/issues/731
+        if not hasattr(self, "_currency_field"):
             self.add_currency_field(cls, name)
 
         super().contribute_to_class(cls, name)
 
         setattr(cls, self.name, self.money_descriptor_class(self))
 
     def add_currency_field(self, cls, name):
```

### Comparing `django-money-3.4.1/djmoney/models/managers.py` & `django_money-3.5/djmoney/models/managers.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/models/validators.py` & `django_money-3.5/djmoney/models/validators.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/money.py` & `django_money-3.5/djmoney/money.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/money.pyi` & `django_money-3.5/djmoney/money.pyi`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/serializers.py` & `django_money-3.5/djmoney/serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 if ignore:
                     continue
                 else:
                     raise
             money_fields = {}
             fields = {}
             field_names = {field.name for field in Model._meta.get_fields()}
-            for (field_name, field_value) in obj["fields"].items():
+            for field_name, field_value in obj["fields"].items():
                 if ignore and field_name not in field_names:
                     # skip fields no longer on model
                     continue
                 field = Model._meta.get_field(field_name)
                 if isinstance(field, MoneyField) and field_value is not None:
                     money_fields[field_name] = Money(
                         field_value, obj["fields"][get_currency_field_name(field_name, field)]
```

### Comparing `django-money-3.4.1/djmoney/settings.py` & `django_money-3.5/djmoney/settings.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/templatetags/djmoney.py` & `django_money-3.5/djmoney/templatetags/djmoney.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/djmoney/utils.py` & `django_money-3.5/djmoney/utils.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/setup.cfg` & `django_money-3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/setup.py` & `django_money-3.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,17 @@
 import codecs
 import os
 import re
-import sys
 
 from setuptools import find_packages, setup
-from setuptools.command.test import test as TestCommand
-
-
-class PyTest(TestCommand):
-    user_options = [("pytest-args=", "a", "Arguments to pass into py.test")]
-
-    def initialize_options(self):
-        TestCommand.initialize_options(self)
-        self.pytest_args = []
-
-    def finalize_options(self):
-        TestCommand.finalize_options(self)
-        self.test_args = []
-        self.test_suite = True
-
-    def run_tests(self):
-        import pytest
-
-        errno = pytest.main(self.pytest_args)
-        sys.exit(errno)
 
 
 test_requirements = [
-    # Quickfix for https://docs.pytest.org/en/7.1.x/deprecations.html#using-pytest-warns-none
-    "pytest>=3.1.0,<7.0",
+    "pytest>=8.2,<8.3",
     "pytest-django",
-    "pytest-pythonpath",
     "pytest-cov",
     "mixer",
     "mypy",
     "django-stubs",
 ]
 
 extras_requirements = {
@@ -90,9 +67,8 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     tests_require=test_requirements,
     extras_require=extras_requirements,
-    cmdclass={"test": PyTest},
 )
```

### Comparing `django-money-3.4.1/tests/test_admin.py` & `django_money-3.5/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/tests/test_form.py` & `django_money-3.5/tests/test_form.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Created on May 7, 2011
 
 @author: jake
 """
+
+import warnings
 from decimal import Decimal
 
 import pytest
 
 from djmoney import settings
 from djmoney.models.fields import MoneyField
 from djmoney.money import Money
@@ -118,17 +120,17 @@
     assert form.fields["money"].initial == [123, "PLN"]
 
 
 def test_no_deprecation_warning():
     """
     The library's code shouldn't generate any warnings itself. See #262.
     """
-    with pytest.warns(None) as warning:
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
         MoneyField(max_digits=10, decimal_places=2, currency_choices=(("USD", "USD"),)).formfield()
-    assert not warning
 
 
 class TestValidation:
     @pytest.mark.parametrize(
         "value, error",
         (
             (Money(50, "EUR"), "Ensure this value is greater than or equal to €100.00."),
```

### Comparing `django-money-3.4.1/tests/test_managers.py` & `django_money-3.5/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/tests/test_models.py` & `django_money-3.5/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Created on May 7, 2011
 
 @author: jake
 """
+
 import datetime
 from copy import copy
 from decimal import Decimal, InvalidOperation
 
 from django import VERSION
 from django.core.exceptions import ValidationError
 from django.db import IntegrityError, models
```

### Comparing `django-money-3.4.1/tests/test_money.py` & `django_money-3.5/tests/test_money.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/tests/test_reversion.py` & `django_money-3.5/tests/test_reversion.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/tests/test_serialization.py` & `django_money-3.5/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/tests/test_settings.py` & `django_money-3.5/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-money-3.4.1/tests/test_tags.py` & `django_money-3.5/tests/test_tags.py`

 * *Files identical despite different names*

