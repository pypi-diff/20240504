# Comparing `tmp/rer.newsletterplugin.flask-0.1.0.tar.gz` & `tmp/rer.newsletterplugin.flask-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rer.newsletterplugin.flask-0.1.0.tar", last modified: Tue Jul 21 07:49:56 2020, max compression
+gzip compressed data, was "rer.newsletterplugin.flask-0.1.1.tar", last modified: Sat May  4 20:44:15 2024, max compression
```

## Comparing `rer.newsletterplugin.flask-0.1.0.tar` & `rer.newsletterplugin.flask-0.1.1.tar`

### file list

```diff
@@ -1,89 +1,91 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/
--rw-r--r--   0 cekk       (501) staff       (20)     4714 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)       27 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)       50 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/constraints_plone52.txt
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      105 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/constraints_plone51.txt
--rw-r--r--   0 cekk       (501) staff       (20)      102 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/MANIFEST.in
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/docs/
--rw-r--r--   0 cekk       (501) staff       (20)      101 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)     7913 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)    32560 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/docs/rer-logo.png
--rw-r--r--   0 cekk       (501) staff       (20)      586 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)     2703 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/setup.py
--rw-r--r--   0 cekk       (501) staff       (20)       62 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      666 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      321 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     1926 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/.gitlab-ci.yml
--rw-r--r--   0 cekk       (501) staff       (20)     2600 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1835 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/publiccode.yml
--rw-r--r--   0 cekk       (501) staff       (20)       89 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1213 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/.travis.yml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/
--rw-r--r--   0 cekk       (501) staff       (20)      806 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/interfaces.py
--rw-r--r--   0 cekk       (501) staff       (20)     1475 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/
--rw-r--r--   0 cekk       (501) staff       (20)     1599 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/update.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     2306 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.po
--rw-r--r--   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/__init__.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      515 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/update.sh
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     1819 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.po
--rw-r--r--   0 cekk       (501) staff       (20)      611 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1951 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/rer.newsletterplugin.flask.pot
--rw-r--r--   0 cekk       (501) staff       (20)      260 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/tests/
--rw-r--r--   0 cekk       (501) staff       (20)     2624 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/tests/test_setup.py
--rw-r--r--   0 cekk       (501) staff       (20)     5887 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/tests/test_send_to_queue.py
--rw-r--r--   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3362 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/tests/test_send_complete.py
--rw-r--r--   0 cekk       (501) staff       (20)     2603 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/tests/test_send_adapter.py
--rw-r--r--   0 cekk       (501) staff       (20)      215 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/adapter/
--rw-r--r--   0 cekk       (501) staff       (20)      446 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/adapter/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     7054 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/adapter/flask_adapter.py
--rw-r--r--   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/adapter/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      627 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/setuphandlers.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/browser/
--rw-r--r--   0 cekk       (501) staff       (20)      568 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      807 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/browser/sendmessageview.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/browser/templates/
--rw-r--r--   0 cekk       (501) staff       (20)     1366 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/browser/templates/sendmessageview.pt
--rw-r--r--   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/browser/templates/.gitkeep
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      105 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      118 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/profiles/default/rolemap.xml
--rw-r--r--   0 cekk       (501) staff       (20)      242 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/profiles/default/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      203 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      182 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/profiles/default/metadata.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      255 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/profiles/uninstall/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      136 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)     2626 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/services/
--rw-r--r--   0 cekk       (501) staff       (20)      199 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/services/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/services/send_complete/
--rw-r--r--   0 cekk       (501) staff       (20)     2444 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/services/send_complete/post.py
--rw-r--r--   0 cekk       (501) staff       (20)      350 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/services/send_complete/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/services/send_complete/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/services/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)       80 2020-07-21 07:49:55.000000 rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer.newsletterplugin.flask.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     4714 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer.newsletterplugin.flask.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)        1 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer.newsletterplugin.flask.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)       25 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer.newsletterplugin.flask.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)     2950 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer.newsletterplugin.flask.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)      151 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer.newsletterplugin.flask.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)      226 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer.newsletterplugin.flask.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)        4 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer.newsletterplugin.flask.egg-info/top_level.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2020-07-21 07:49:56.000000 rer.newsletterplugin.flask-0.1.0/src/rer.newsletterplugin.flask.egg-info/dependency_links.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.453294 rer.newsletterplugin.flask-0.1.1/
+-rw-r--r--   0 cekk       (501) staff       (20)     1926 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/.gitlab-ci.yml
+-rw-r--r--   0 cekk       (501) staff       (20)     1213 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/.travis.yml
+-rw-r--r--   0 cekk       (501) staff       (20)      171 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       62 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      666 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      102 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     4116 2024-05-04 20:44:15.453361 rer.newsletterplugin.flask-0.1.1/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2600 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/constraints_plone51.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/constraints_plone52.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.446434 rer.newsletterplugin.flask-0.1.1/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7913 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)      101 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    32560 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/docs/rer-logo.png
+-rw-r--r--   0 cekk       (501) staff       (20)     1835 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/publiccode.yml
+-rw-r--r--   0 cekk       (501) staff       (20)       50 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      321 2024-05-04 20:44:15.453689 rer.newsletterplugin.flask-0.1.1/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2831 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.442757 rer.newsletterplugin.flask-0.1.1/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.446594 rer.newsletterplugin.flask-0.1.1/src/rer/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.447884 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.448663 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/
+-rw-r--r--   0 cekk       (501) staff       (20)      215 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.449049 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/adapter/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/adapter/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      446 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/adapter/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     7054 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/adapter/flask_adapter.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.449433 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      568 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      807 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/sendmessageview.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.449689 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/templates/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/templates/.gitkeep
+-rw-r--r--   0 cekk       (501) staff       (20)     1366 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/templates/sendmessageview.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     1475 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      806 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.450333 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.443347 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.450616 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      458 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     1819 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.443473 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.450897 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1118 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     2306 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1951 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/rer.newsletterplugin.flask.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1599 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      515 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      260 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.443683 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.451575 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      203 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      182 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      242 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.451859 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      136 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      255 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/uninstall/registry.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.452119 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      199 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.452492 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/send_complete/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/send_complete/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      350 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/send_complete/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2444 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/send_complete/post.py
+-rw-r--r--   0 cekk       (501) staff       (20)      627 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2626 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.453157 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2603 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_send_adapter.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3362 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_send_complete.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5887 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_send_to_queue.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2624 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.447717 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     4116 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3118 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      131 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       25 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      226 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rer.newsletterplugin.flask-0.1.0/LICENSE.GPL` & `rer.newsletterplugin.flask-0.1.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/docs/conf.py` & `rer.newsletterplugin.flask-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/docs/rer-logo.png` & `rer.newsletterplugin.flask-0.1.1/docs/rer-logo.png`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/DEVELOP.rst` & `rer.newsletterplugin.flask-0.1.1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/setup.py` & `rer.newsletterplugin.flask-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,81 @@
 # -*- coding: utf-8 -*-
 """Installer for the rer.newsletterplugin.flask package."""
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-long_description = '\n\n'.join(
+long_description = "\n\n".join(
     [
-        open('README.rst').read(),
-        open('CONTRIBUTORS.rst').read(),
-        open('CHANGES.rst').read(),
+        open("README.rst").read(),
+        open("CONTRIBUTORS.rst").read(),
+        open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
-    name='rer.newsletterplugin.flask',
-    version='0.1.0',
+    name="rer.newsletterplugin.flask",
+    version="0.1.1",
     description="Add-on per Plone collegato a rer.newsletter per inviare le mail usando un servizio Flask",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
-    keywords='Python Plone',
-    author='RedTurtle',
-    author_email='sviluppo@redturtle.it',
-    url='https://github.com/collective/rer.newsletterplugin.flask',
+    keywords="Python Plone",
+    author="RedTurtle",
+    author_email="sviluppo@redturtle.it",
+    url="https://github.com/collective/rer.newsletterplugin.flask",
     project_urls={
-        'PyPI': 'https://pypi.python.org/pypi/rer.newsletterplugin.flask',
-        'Source': 'https://github.com/collective/rer.newsletterplugin.flask',
-        'Tracker': 'https://github.com/collective/rer.newsletterplugin.flask/issues',
+        "PyPI": "https://pypi.python.org/pypi/rer.newsletterplugin.flask",
+        "Source": "https://github.com/collective/rer.newsletterplugin.flask",
+        "Tracker": "https://github.com/collective/rer.newsletterplugin.flask/issues",
         # 'Documentation': 'https://rer.newsletterplugin.flask.readthedocs.io/en/latest/',
     },
-    license='GPL version 2',
-    packages=find_packages('src', exclude=['ez_setup']),
-    namespace_packages=['rer', 'rer.newsletterplugin'],
-    package_dir={'': 'src'},
+    license="GPL version 2",
+    packages=find_packages("src", exclude=["ez_setup"]),
+    namespace_packages=["rer", "rer.newsletterplugin"],
+    package_dir={"": "src"},
     include_package_data=True,
+    python_requires=">=3.7",
     zip_safe=False,
-    python_requires="==2.7, >=3.6",
     install_requires=[
-        'setuptools',
+        "setuptools",
         # -*- Extra requirements: -*-
-        'z3c.jbot',
-        'plone.api>=1.8.4',
-        'plone.restapi',
-        'plone.app.dexterity',
-        'rer.newsletter',
+        "z3c.jbot",
+        "plone.api>=1.8.4",
+        "plone.restapi",
+        "plone.app.dexterity",
+        "rer.newsletter",
     ],
     extras_require={
-        'test': [
-            'plone.app.testing',
+        "test": [
+            "plone.app.testing",
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
             # plone_coredev tests as of 2016-04-01.
-            'plone.testing>=5.0.0',
-            'plone.app.contenttypes',
-            'plone.app.robotframework[debug]',
-            'collective.MockMailHost',
-            'requests-mock',
+            "plone.testing>=5.0.0",
+            "plone.app.contenttypes",
+            "plone.app.robotframework[debug]",
+            "collective.MockMailHost",
+            "requests-mock",
         ]
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     [console_scripts]
     update_locale = rer.newsletterplugin.flask.locales.update:update_locale
```

### Comparing `rer.newsletterplugin.flask-0.1.0/LICENSE.rst` & `rer.newsletterplugin.flask-0.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/.gitlab-ci.yml` & `rer.newsletterplugin.flask-0.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/README.rst` & `rer.newsletterplugin.flask-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/publiccode.yml` & `rer.newsletterplugin.flask-0.1.1/publiccode.yml`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/.travis.yml` & `rer.newsletterplugin.flask-0.1.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/interfaces.py` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/interfaces.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/configure.zcml` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/update.py` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/update.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.po` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.po`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/update.sh` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/update.sh`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.po` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.po`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/README.rst` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/README.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/locales/rer.newsletterplugin.flask.pot` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/rer.newsletterplugin.flask.pot`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/tests/test_setup.py` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/tests/test_send_to_queue.py` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_send_to_queue.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/tests/test_send_complete.py` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_send_complete.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/tests/test_send_adapter.py` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_send_adapter.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/adapter/flask_adapter.py` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/adapter/flask_adapter.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/setuphandlers.py` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/browser/configure.zcml` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/browser/sendmessageview.py` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/sendmessageview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/browser/templates/sendmessageview.pt` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/templates/sendmessageview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/testing.py` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/testing.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer/newsletterplugin/flask/services/send_complete/post.py` & `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/send_complete/post.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.0/src/rer.newsletterplugin.flask.egg-info/SOURCES.txt` & `rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,17 @@
 src/rer/newsletterplugin/flask/browser/templates/.gitkeep
 src/rer/newsletterplugin/flask/browser/templates/sendmessageview.pt
 src/rer/newsletterplugin/flask/locales/README.rst
 src/rer/newsletterplugin/flask/locales/__init__.py
 src/rer/newsletterplugin/flask/locales/rer.newsletterplugin.flask.pot
 src/rer/newsletterplugin/flask/locales/update.py
 src/rer/newsletterplugin/flask/locales/update.sh
+src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.mo
 src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.po
+src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.mo
 src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.po
 src/rer/newsletterplugin/flask/profiles/default/browserlayer.xml
 src/rer/newsletterplugin/flask/profiles/default/catalog.xml
 src/rer/newsletterplugin/flask/profiles/default/metadata.xml
 src/rer/newsletterplugin/flask/profiles/default/registry.xml
 src/rer/newsletterplugin/flask/profiles/default/rolemap.xml
 src/rer/newsletterplugin/flask/profiles/uninstall/browserlayer.xml
```

