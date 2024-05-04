# Comparing `tmp/django-admin-extra-buttons-1.5.7.tar.gz` & `tmp/django_admin_extra_buttons-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-extra-buttons-1.5.7.tar", last modified: Tue Nov 28 13:11:22 2023, max compression
+gzip compressed data, was "django_admin_extra_buttons-1.5.8.tar", last modified: Sat May  4 05:57:35 2024, max compression
```

## Comparing `django-admin-extra-buttons-1.5.7.tar` & `django_admin_extra_buttons-1.5.8.tar`

### file list

```diff
@@ -1,102 +1,2611 @@
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.589930 django-admin-extra-buttons-1.5.7/
--rw-r--r--   0 sax        (501) staff       (20)      836 2023-11-28 13:11:14.000000 django-admin-extra-buttons-1.5.7/CHANGES
--rw-r--r--   0 sax        (501) staff       (20)     1164 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/LICENSE
--rw-r--r--   0 sax        (501) staff       (20)      285 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/MANIFEST.in
--rw-r--r--   0 sax        (501) staff       (20)     4945 2023-11-28 13:11:22.590087 django-admin-extra-buttons-1.5.7/PKG-INFO
--rw-r--r--   0 sax        (501) staff       (20)     3833 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/README.md
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.566544 django-admin-extra-buttons-1.5.7/docs/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.568809 django-admin-extra-buttons-1.5.7/docs/api/
--rw-r--r--   0 sax        (501) staff       (20)     3974 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/api/button.md
--rw-r--r--   0 sax        (501) staff       (20)     2484 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/api/choice.md
--rw-r--r--   0 sax        (501) staff       (20)      505 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/api/handlers.md
--rw-r--r--   0 sax        (501) staff       (20)     1995 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/api/link.md
--rw-r--r--   0 sax        (501) staff       (20)     1075 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/api/mixin.md
--rw-r--r--   0 sax        (501) staff       (20)        0 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/api/utils.md
--rw-r--r--   0 sax        (501) staff       (20)      896 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/api/view.md
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.569068 django-admin-extra-buttons-1.5.7/docs/css/
--rw-r--r--   0 sax        (501) staff       (20)      973 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/css/extra.css
--rw-r--r--   0 sax        (501) staff       (20)     1340 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/howto.md
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.569644 django-admin-extra-buttons-1.5.7/docs/images/
--rw-r--r--   0 sax        (501) staff       (20)    28164 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/images/buttons.png
--rw-r--r--   0 sax        (501) staff       (20)   167645 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/images/screenshot.png
--rw-r--r--   0 sax        (501) staff       (20)       16 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/index.md
--rw-r--r--   0 sax        (501) staff       (20)       69 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/requirements.txt
--rw-r--r--   0 sax        (501) staff       (20)      249 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/docs/to_gif.sh
--rw-r--r--   0 sax        (501) staff       (20)     1451 2022-02-19 20:21:39.000000 django-admin-extra-buttons-1.5.7/docs/~index.md
--rw-r--r--   0 sax        (501) staff       (20)      766 2023-11-28 13:11:22.590674 django-admin-extra-buttons-1.5.7/setup.cfg
--rwxr-xr-x   0 sax        (501) staff       (20)     2812 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/setup.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.561587 django-admin-extra-buttons-1.5.7/src/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.573296 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/
--rw-r--r--   0 sax        (501) staff       (20)       87 2023-11-28 13:11:14.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)      133 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/api.py
--rw-r--r--   0 sax        (501) staff       (20)       94 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/apps.py
--rw-r--r--   0 sax        (501) staff       (20)     6285 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/buttons.py
--rw-r--r--   0 sax        (501) staff       (20)      818 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/decorators.py
--rw-r--r--   0 sax        (501) staff       (20)     6065 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/handlers.py
--rw-r--r--   0 sax        (501) staff       (20)     6364 2023-11-28 13:11:14.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/mixins.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.575048 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/static/
--rw-r--r--   0 sax        (501) staff       (20)      389 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/static/admin_extra_buttons.css
--rw-r--r--   0 sax        (501) staff       (20)      216 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/static/admin_extra_buttons.css.map
--rw-r--r--   0 sax        (501) staff       (20)      957 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/static/admin_extra_buttons.js
--rw-r--r--   0 sax        (501) staff       (20)      671 2023-11-28 13:09:54.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/static/admin_extra_buttons.min.js
--rw-r--r--   0 sax        (501) staff       (20)      478 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/static/admin_extra_buttons.scss
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.560971 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.576427 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/
--rw-r--r--   0 sax        (501) staff       (20)     1228 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/action_page.html
--rw-r--r--   0 sax        (501) staff       (20)      350 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/change_form.html
--rw-r--r--   0 sax        (501) staff       (20)      279 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/change_list.html
--rw-r--r--   0 sax        (501) staff       (20)      990 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/confirm.html
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.578511 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/includes/
--rw-r--r--   0 sax        (501) staff       (20)      226 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/includes/action_buttons.html
--rw-r--r--   0 sax        (501) staff       (20)      178 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/includes/attrs.html
--rw-r--r--   0 sax        (501) staff       (20)      289 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/includes/button.html
--rw-r--r--   0 sax        (501) staff       (20)      253 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/includes/change_form_buttons.html
--rw-r--r--   0 sax        (501) staff       (20)      247 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/includes/change_list_buttons.html
--rw-r--r--   0 sax        (501) staff       (20)      520 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/includes/choice.html
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.579073 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templatetags/
--rw-r--r--   0 sax        (501) staff       (20)        0 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templatetags/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)      779 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templatetags/extra_buttons.py
--rw-r--r--   0 sax        (501) staff       (20)     3825 2023-11-28 13:11:14.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/utils.py
--rw-r--r--   0 sax        (501) staff       (20)     4159 2022-02-18 06:02:55.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/~button.p_
--rw-r--r--   0 sax        (501) staff       (20)      503 2022-02-18 06:02:55.000000 django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/~config.p_
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.581013 django-admin-extra-buttons-1.5.7/src/django_admin_extra_buttons.egg-info/
--rw-r--r--   0 sax        (501) staff       (20)     4945 2023-11-28 13:11:22.000000 django-admin-extra-buttons-1.5.7/src/django_admin_extra_buttons.egg-info/PKG-INFO
--rw-r--r--   0 sax        (501) staff       (20)     2893 2023-11-28 13:11:22.000000 django-admin-extra-buttons-1.5.7/src/django_admin_extra_buttons.egg-info/SOURCES.txt
--rw-r--r--   0 sax        (501) staff       (20)        1 2023-11-28 13:11:22.000000 django-admin-extra-buttons-1.5.7/src/django_admin_extra_buttons.egg-info/dependency_links.txt
--rw-r--r--   0 sax        (501) staff       (20)      293 2023-11-28 13:11:22.000000 django-admin-extra-buttons-1.5.7/src/django_admin_extra_buttons.egg-info/requires.txt
--rw-r--r--   0 sax        (501) staff       (20)       20 2023-11-28 13:11:22.000000 django-admin-extra-buttons-1.5.7/src/django_admin_extra_buttons.egg-info/top_level.txt
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.586139 django-admin-extra-buttons-1.5.7/tests/
--rw-r--r--   0 sax        (501) staff       (20)      625 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/.coveragerc
--rw-r--r--   0 sax        (501) staff       (20)   163840 2022-09-15 21:09:17.000000 django-admin-extra-buttons-1.5.7/tests/.db.sqlite
--rw-r--r--   0 sax        (501) staff       (20)     1195 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/conftest.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.562061 django-admin-extra-buttons-1.5.7/tests/demoapp/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.588303 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/
--rw-r--r--   0 sax        (501) staff       (20)        0 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)     6282 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/admin.py
--rw-r--r--   0 sax        (501) staff       (20)      626 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/backends.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.589231 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/migrations/
--rw-r--r--   0 sax        (501) staff       (20)     1385 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/migrations/0001_initial.py
--rw-r--r--   0 sax        (501) staff       (20)     1353 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/migrations/0002_demomodel5_alter_demomodel1_options_and_more.py
--rw-r--r--   0 sax        (501) staff       (20)        0 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/migrations/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)     1209 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/models.py
--rw-r--r--   0 sax        (501) staff       (20)     1670 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/settings.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.562647 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/templates/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.589453 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/templates/admin_extra_buttons/
--rw-r--r--   0 sax        (501) staff       (20)      376 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/templates/admin_extra_buttons/upload.html
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-11-28 13:11:22.589711 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/templates/demo/
--rw-r--r--   0 sax        (501) staff       (20)       53 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/templates/demo/test22.html
--rw-r--r--   0 sax        (501) staff       (20)     1725 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/upload.py
--rw-r--r--   0 sax        (501) staff       (20)      237 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/demoapp/demo/urls.py
--rwxr-xr-x   0 sax        (501) staff       (20)      335 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/manage.py
--rw-r--r--   0 sax        (501) staff       (20)      195 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/test_admin.py
--rw-r--r--   0 sax        (501) staff       (20)     3505 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/test_buttons.py
--rw-r--r--   0 sax        (501) staff       (20)      456 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/test_checks.py
--rw-r--r--   0 sax        (501) staff       (20)     1089 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/test_choices.py
--rw-r--r--   0 sax        (501) staff       (20)     1060 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/test_confirm.py
--rw-r--r--   0 sax        (501) staff       (20)      827 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/test_links.py
--rw-r--r--   0 sax        (501) staff       (20)      786 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/test_mixin.py
--rw-r--r--   0 sax        (501) staff       (20)      534 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/test_templatetags.py
--rw-r--r--   0 sax        (501) staff       (20)      688 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/test_upload.py
--rw-r--r--   0 sax        (501) staff       (20)     1200 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/test_utils.py
--rw-r--r--   0 sax        (501) staff       (20)     1397 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tests/test_views.py
--rw-r--r--   0 sax        (501) staff       (20)     1135 2023-11-28 13:09:39.000000 django-admin-extra-buttons-1.5.7/tox.ini
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.421798 django_admin_extra_buttons-1.5.8/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.116073 django_admin_extra_buttons-1.5.8/.tox/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.048577 django_admin_extra_buttons-1.5.8/.tox/.pkg/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.048629 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.048682 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.050185 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.132710 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.049634 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.133030 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.133148 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.133274 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.133386 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.133490 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.133598 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.133722 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.133820 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.133916 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.134011 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.134110 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.134226 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.134537 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      286 2024-05-04 05:20:16.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.049760 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.050119 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.134653 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.049926 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/jaraco/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.135034 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/jaraco/functools/
+-rw-r--r--   0 sax        (501) staff       (20)     3982 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/jaraco/functools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/jaraco/functools/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.136533 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    21044 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     4436 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.136785 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.136898 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.050233 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.050641 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.137002 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.137107 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.050455 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/jaraco/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.137417 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/jaraco/functools/
+-rw-r--r--   0 sax        (501) staff       (20)     3982 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/jaraco/functools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/jaraco/functools/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.138307 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    14977 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     3551 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.138450 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.138555 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:20:17.000000 django_admin_extra_buttons-1.5.8/.tox/.pkg/lib/python3.12/site-packages/setuptools/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.050762 django_admin_extra_buttons-1.5.8/.tox/.tox/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.050810 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.050859 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.051159 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.138704 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:26.000000 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.138805 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:26.000000 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.138899 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:01:26.000000 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.139147 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:27.000000 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.139253 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.051275 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.139357 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:26.000000 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:26.000000 django_admin_extra_buttons-1.5.8/.tox/.tox/lib/python3.9/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.051395 django_admin_extra_buttons-1.5.8/.tox/d22-py310/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.051445 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.051494 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.052548 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.139459 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:29.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.139557 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:28.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.139670 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:28.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.139767 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:29.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.139871 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:28.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.139969 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:27.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.140067 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:29.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.140164 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-09-08 07:30:46.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.140440 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:28.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.140535 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.052231 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.140635 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:28.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:28.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.140730 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:27.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.140823 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:29.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.140916 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:30.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.141004 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:32:27.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.141098 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-09-08 07:32:27.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py310/lib/python3.10/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.052672 django_admin_extra_buttons-1.5.8/.tox/d22-py36/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.052726 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.052775 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.053485 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.141398 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:41.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.141492 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:38.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.141589 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:37.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.141683 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:38.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.141784 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:38.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.141874 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:37.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.141973 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:01:38.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.142258 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.053362 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.142353 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:37.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:37.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.142444 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:37.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.142537 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:38.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py36/lib/python3.6/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.053599 django_admin_extra_buttons-1.5.8/.tox/d22-py37/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.053646 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.053696 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.054698 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.142634 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:45.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.142730 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:43.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.142824 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:41.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.142914 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:42.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.143004 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:42.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.143099 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:41.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.143192 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:43.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.143290 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:41.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.143380 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:01:43.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.143617 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:45.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.143723 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.054451 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.143828 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:41.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:41.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.143923 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:41.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.144019 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:43.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.144116 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:41.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.144222 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-02-18 06:01:43.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py37/lib/python3.7/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.054821 django_admin_extra_buttons-1.5.8/.tox/d22-py38/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.054870 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.054917 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.055900 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.144557 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:37.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.144650 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:34.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.144746 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:32.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.144836 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:33.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.144932 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:34.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.145027 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:34.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.145120 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:32.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.145223 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:01:34.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.145511 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:37.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.145619 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.055649 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.145718 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:32.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:32.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.145817 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:32.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.145918 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:34.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.146015 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:32.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.146122 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-02-18 06:01:34.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py38/lib/python3.8/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.056018 django_admin_extra_buttons-1.5.8/.tox/d22-py39/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.056065 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.056114 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.057146 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.146389 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:37.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.146487 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:36.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.146582 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:36.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.146681 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:37.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.146778 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:36.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.146868 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:34.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.146963 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:36.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.147054 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-09-08 07:29:15.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.147307 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:36.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.147405 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.056835 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.147516 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:35.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:35.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.147617 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:35.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.147708 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:37.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.147804 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:38.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.147902 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:30:35.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.147995 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-09-08 07:30:34.000000 django_admin_extra_buttons-1.5.8/.tox/d22-py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.057267 django_admin_extra_buttons-1.5.8/.tox/d30-py36/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.057316 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.057364 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.058170 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.148293 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:40.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.148387 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:37.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.148482 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:38.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.148581 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:37.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.148678 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:38.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.148772 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:38.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.148871 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:37.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.148964 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:02:38.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.149231 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.058040 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.149329 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:37.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:37.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.149423 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:37.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.149531 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:38.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py36/lib/python3.6/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.058288 django_admin_extra_buttons-1.5.8/.tox/d30-py37/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.058336 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.058387 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.059202 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.149630 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:29.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.149736 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:25.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.149833 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:26.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.149922 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:25.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.150018 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:26.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.150118 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:25.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.150220 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:02:26.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.150450 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.059054 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.150559 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:25.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:25.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.150658 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:25.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.150773 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:26.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py37/lib/python3.7/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.059322 django_admin_extra_buttons-1.5.8/.tox/d30-py38/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.059375 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.059433 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.060180 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.150889 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:36.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.151002 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:33.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.151118 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:34.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.151220 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:34.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.151332 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:33.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.151461 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:02:34.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.151744 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.060037 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.151862 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:33.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:33.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.151978 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:33.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.152087 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:34.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py38/lib/python3.8/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.060306 django_admin_extra_buttons-1.5.8/.tox/d30-py39/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.060360 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.060413 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.061139 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.152202 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:33.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.152313 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:29.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.152438 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:30.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.152566 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:30.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.152678 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:29.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.152787 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:02:30.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.153090 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.061000 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.153212 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:29.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:29.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.153324 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:29.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.153447 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:30.000000 django_admin_extra_buttons-1.5.8/.tox/d30-py39/lib/python3.9/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.061263 django_admin_extra_buttons-1.5.8/.tox/d31-py36/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.061327 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.061385 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.062278 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.153571 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:06.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.153687 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:02.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.153798 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:03.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.153917 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:03.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.154030 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:03.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.154139 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:04.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.154250 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:02.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.154354 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:02:03.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.154667 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.062136 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.154792 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:02.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:02.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.154911 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:02.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.155030 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:03.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py36/lib/python3.6/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.062424 django_admin_extra_buttons-1.5.8/.tox/d31-py37/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.062482 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.062546 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.064389 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.155148 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:25.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.155257 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:20.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.155379 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:22.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.155487 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:20.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.155593 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:21.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.155698 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:21.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.155818 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:20.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.155920 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:22.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.156029 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:20.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.156138 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:02:22.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.156390 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:25.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.156487 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.063963 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.156595 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:20.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:20.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.156687 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:20.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.156779 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:22.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.156879 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:20.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.156978 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-02-18 06:02:22.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py37/lib/python3.7/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.064587 django_admin_extra_buttons-1.5.8/.tox/d31-py38/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.064670 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.064753 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.066541 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.157238 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:12.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.157331 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:06.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.157423 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:08.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.157522 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:06.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.157636 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:08.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.157755 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:08.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.157882 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:09.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.158005 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:06.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.158124 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:02:08.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.158399 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:13.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.158517 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.066129 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.158627 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:06.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:06.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.158732 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:07.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.158831 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:09.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.158924 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:07.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.159018 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-02-18 06:02:08.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py38/lib/python3.8/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.066730 django_admin_extra_buttons-1.5.8/.tox/d31-py39/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.066808 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.066891 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.068591 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.159232 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:19.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.159334 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:13.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.159427 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:15.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.159526 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:13.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.159618 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:14.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.159712 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:14.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.159803 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:15.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.159950 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:13.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.160057 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:02:15.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.160328 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:19.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.160429 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.068174 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.160525 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:13.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:13.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.160622 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:13.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.160717 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:15.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.160830 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:02:13.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.160929 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-02-18 06:02:15.000000 django_admin_extra_buttons-1.5.8/.tox/d31-py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.068781 django_admin_extra_buttons-1.5.8/.tox/d32-py311/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.068855 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.068925 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.073445 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.161143 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.161241 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:15.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.163739 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)    16976 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attr/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      399 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attr/_cmp.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      469 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attr/_typing_compat.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      209 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attr/_version_info.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      406 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attr/converters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      539 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attr/exceptions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      225 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attr/filters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attr/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      567 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attr/setters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2580 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attr/validators.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.164013 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)     2168 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attrs/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.164123 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.164468 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 sax        (501) staff       (20)       72 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/coverage/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     1171 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/coverage/tracer.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.164681 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/cssselect/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/cssselect/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.166491 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)   134880 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/faker/proxy.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.166588 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.166683 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.166775 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.166872 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.071626 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.167123 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.167232 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.167344 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.167446 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.167541 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.167636 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.167728 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.167823 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.167921 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.168013 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.168122 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.168218 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.168459 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      286 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.071812 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.072152 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.168569 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.170076 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    20105 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     4056 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.170320 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.170415 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.170513 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.170605 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pluggy/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pluggy/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.170940 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 sax        (501) staff       (20)      535 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pyproject_api/_backend.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.171034 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.171126 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.072811 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.073242 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.171227 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.171320 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.172038 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    14977 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     3551 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.172258 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.172352 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:20:14.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.172577 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:29.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.172669 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:30.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py311/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.073595 django_admin_extra_buttons-1.5.8/.tox/d32-py312/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.073666 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.073730 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.076464 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.172765 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:45.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.172857 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:39.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.175146 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)    16976 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attr/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      399 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attr/_cmp.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      469 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attr/_typing_compat.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      209 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attr/_version_info.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      406 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attr/converters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      539 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attr/exceptions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      225 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attr/filters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attr/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      567 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attr/setters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2580 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attr/validators.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.175399 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)     2168 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attrs/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.175491 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.175847 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/coverage/
+-rw-r--r--   0 sax        (501) staff       (20)       72 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/coverage/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     1171 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/coverage/tracer.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.176072 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/cssselect/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/cssselect/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.177024 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)   134880 2024-05-04 05:21:45.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/faker/proxy.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:45.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.177125 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.177215 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.177310 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.177400 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.075929 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.177656 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.177748 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.177838 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.177928 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.178024 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.178117 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.178209 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.178302 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.178398 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.178502 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.178593 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.178689 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.178950 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      286 2024-05-04 05:21:38.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.179046 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.179136 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pluggy/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pluggy/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.179484 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pyproject_api/
+-rw-r--r--   0 sax        (501) staff       (20)      535 2024-05-04 05:21:45.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pyproject_api/_backend.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:45.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.179576 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:45.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.179667 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:45.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.179758 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:44.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.179849 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/tox/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:45.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py312/lib/python3.12/site-packages/tox/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.076599 django_admin_extra_buttons-1.5.8/.tox/d32-py37/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.076654 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.076714 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.078254 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.179945 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:26.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.180040 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:20.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.180129 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:22.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.180216 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:20.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.180308 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:21.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.180399 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:21.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.180493 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:20.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.180583 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:22.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.180675 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:20.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.180766 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:01:22.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.181034 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:26.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.181124 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.077894 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.181216 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:20.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:20.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.181309 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:20.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.181398 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:22.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.181491 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:20.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.181590 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-02-18 06:01:22.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py37/lib/python3.7/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.078420 django_admin_extra_buttons-1.5.8/.tox/d32-py38/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.078497 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.078561 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.079938 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.181849 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:32.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.181952 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:27.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.182048 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:29.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.182143 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:27.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.182232 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:28.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.182333 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:29.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.182422 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:29.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.182513 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:27.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.182605 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:01:29.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.182868 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:32.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.182957 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.079645 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.183056 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:27.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:27.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.183144 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:27.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.183232 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:29.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.183324 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:27.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.183414 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-02-18 06:01:29.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py38/lib/python3.8/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.080099 django_admin_extra_buttons-1.5.8/.tox/d32-py39/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.080168 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.080231 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.084016 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.183657 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.183748 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:04.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.186345 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)    16976 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attr/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      399 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attr/_cmp.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      469 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attr/_typing_compat.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      209 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attr/_version_info.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      406 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attr/converters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      539 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attr/exceptions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      225 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attr/filters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attr/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      567 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attr/setters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2580 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attr/validators.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.186640 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)     2168 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attrs/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.186748 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.187156 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/coverage/
+-rw-r--r--   0 sax        (501) staff       (20)       72 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/coverage/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     1171 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/coverage/tracer.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.187424 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/cssselect/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/cssselect/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.187534 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/exceptiongroup/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.188258 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)   134880 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/faker/proxy.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.188370 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.188471 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.188583 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.188694 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.082350 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.188979 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.189095 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.189207 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.189320 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.189427 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.189539 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.189651 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.189763 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.189875 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.189990 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.190106 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.190219 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.190521 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      286 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.082477 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.082777 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.190640 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.192012 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    20105 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     4056 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.192163 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.192257 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.192350 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.192442 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pluggy/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pluggy/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.192784 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pyproject_api/
+-rw-r--r--   0 sax        (501) staff       (20)      535 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pyproject_api/_backend.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.192878 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.192969 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.083275 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.083704 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.193070 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.193179 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.193905 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    14977 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     3551 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.194119 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.194216 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:14:03.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/setuptools/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.194468 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:01.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.194560 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:15:01.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.194784 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/tox/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:02.000000 django_admin_extra_buttons-1.5.8/.tox/d32-py39/lib/python3.9/site-packages/tox/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.084192 django_admin_extra_buttons-1.5.8/.tox/d40-py310/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.084262 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.084333 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.086031 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.194883 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:08.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.194985 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:56.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.195081 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:07.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.195172 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:07.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.195265 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:08.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.195354 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:07.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.195445 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:06.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.195539 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:08.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.195628 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-09-08 07:33:55.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.195877 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:07.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.195967 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.085542 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.196067 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:07.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:07.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.196160 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:06.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.196251 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:08.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.196339 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:09.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.196436 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:06.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.196530 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-09-08 07:34:06.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py310/lib/python3.10/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.086211 django_admin_extra_buttons-1.5.8/.tox/d40-py37/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.086281 django_admin_extra_buttons-1.5.8/.tox/d40-py37/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.086362 django_admin_extra_buttons-1.5.8/.tox/d40-py37/lib/python3.7/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.086430 django_admin_extra_buttons-1.5.8/.tox/d40-py37/lib/python3.7/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.196843 django_admin_extra_buttons-1.5.8/.tox/d40-py37/lib/python3.7/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:01:57.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py37/lib/python3.7/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.086604 django_admin_extra_buttons-1.5.8/.tox/d40-py38/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.086683 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.086760 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.088529 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.197085 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:57.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.197201 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:52.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.197302 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:53.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.197403 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:52.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.087312 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/backports/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.197496 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/backports/zoneinfo/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:53.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/backports/zoneinfo/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.197593 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:53.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.197683 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:53.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.197781 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:54.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.197880 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:52.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.197974 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-18 06:01:53.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.198248 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:57.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.198351 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.088165 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.198444 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:52.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:52.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.198544 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:52.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.198636 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:54.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.198726 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-18 06:01:52.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.198821 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-02-18 06:01:53.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py38/lib/python3.8/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.088698 django_admin_extra_buttons-1.5.8/.tox/d40-py39/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.088755 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.088813 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.090073 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.199104 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:45.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.199203 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:32.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.199299 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:45.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.199396 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:45.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.199487 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:46.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.199587 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:45.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.199682 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:43.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.199776 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:45.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.199864 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-09-08 07:33:31.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.200363 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:44.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.200454 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.089723 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.200553 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:44.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:44.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.200643 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:43.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.200741 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:45.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.200846 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:47.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.200942 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:33:43.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.201038 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-09-08 07:33:43.000000 django_admin_extra_buttons-1.5.8/.tox/d40-py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.090214 django_admin_extra_buttons-1.5.8/.tox/d41-py310/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.090272 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.090321 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.091555 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.201403 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:16.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.201497 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:54.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.201589 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:15.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.201684 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:15.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.201784 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:16.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.201882 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:15.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.201976 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:14.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.202065 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:15.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.202153 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-09-08 07:34:48.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.202402 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:15.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.202501 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.091203 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.202595 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:15.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:15.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.202690 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:14.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.202783 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:16.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.202876 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:17.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.202970 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:35:14.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.203063 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-09-08 07:35:14.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py310/lib/python3.10/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.091681 django_admin_extra_buttons-1.5.8/.tox/d41-py39/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.091740 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.091791 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.093016 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.203320 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:37.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.203415 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:21.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.203508 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:36.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.203597 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:36.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.203690 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:37.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.203789 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:36.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.203885 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:34.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.203981 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:37.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.204074 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-09-08 07:34:19.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.204512 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:36.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.204619 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.092650 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.204735 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:36.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:36.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.204847 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:35.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.204954 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:37.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.205066 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:39.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.205175 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-09-08 07:34:35.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.205289 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-09-08 07:34:35.000000 django_admin_extra_buttons-1.5.8/.tox/d41-py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.093160 django_admin_extra_buttons-1.5.8/.tox/d42-py311/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.093222 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.093278 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.096755 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.205668 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.205769 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:54.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.208094 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)    16976 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attr/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      399 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attr/_cmp.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      469 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attr/_typing_compat.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      209 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attr/_version_info.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      406 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attr/converters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      539 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attr/exceptions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      225 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attr/filters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attr/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      567 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attr/setters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2580 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attr/validators.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.208386 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)     2168 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attrs/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.208484 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:58.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.208813 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 sax        (501) staff       (20)       72 2024-05-04 05:21:58.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/coverage/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     1171 2024-05-04 05:21:58.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/coverage/tracer.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.209037 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/cssselect/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:58.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/cssselect/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.210276 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)   134880 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/faker/proxy.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.210370 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:58.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.210471 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:58.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.210564 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:58.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.210657 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.095317 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.210907 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.211004 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.211102 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.211192 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.211294 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.211388 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.211486 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.211585 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.211679 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.211780 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.211872 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.211973 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.212245 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      286 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.095476 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.095751 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.212342 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.213525 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    20105 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     4056 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.213655 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.213759 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.213852 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:58.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.213942 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pluggy/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:58.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pluggy/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.214290 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 sax        (501) staff       (20)      535 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pyproject_api/_backend.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.214381 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.214469 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.096263 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.096611 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.214572 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.214673 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.215391 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    14977 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     3551 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.215595 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.215690 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:21:53.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.215934 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:58.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.216028 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:21:59.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py311/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.096896 django_admin_extra_buttons-1.5.8/.tox/d42-py312/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.096961 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.097016 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.099445 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.216134 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.216232 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:07.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.218523 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)    16976 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attr/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      399 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attr/_cmp.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      469 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attr/_typing_compat.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      209 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attr/_version_info.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      406 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attr/converters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      539 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attr/exceptions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      225 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attr/filters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attr/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      567 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attr/setters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2580 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attr/validators.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.218792 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)     2168 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attrs/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.218889 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.219252 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/coverage/
+-rw-r--r--   0 sax        (501) staff       (20)       72 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/coverage/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     1171 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/coverage/tracer.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.219489 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/cssselect/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/cssselect/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.220685 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)   134880 2024-05-04 05:22:12.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/faker/proxy.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:12.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.220780 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.220873 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.220966 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.221066 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.098918 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.221449 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.221543 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.221634 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.221726 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.221816 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.221918 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.222011 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.222105 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.222195 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.222298 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.222399 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.222513 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.222994 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      286 2024-05-04 05:22:05.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.223110 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.223222 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pluggy/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pluggy/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.223623 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pyproject_api/
+-rw-r--r--   0 sax        (501) staff       (20)      535 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pyproject_api/_backend.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.223737 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.223837 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:12.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.223945 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:10.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.224053 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/tox/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:11.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py312/lib/python3.12/site-packages/tox/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.099593 django_admin_extra_buttons-1.5.8/.tox/d42-py39/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.099652 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.099710 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.103917 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.224164 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.224274 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:38.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.226523 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)    16976 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attr/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      399 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attr/_cmp.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      469 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attr/_typing_compat.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      209 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attr/_version_info.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      406 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attr/converters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      539 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attr/exceptions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      225 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attr/filters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attr/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      567 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attr/setters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2580 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attr/validators.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.226804 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)     2168 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attrs/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.226897 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.227241 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/coverage/
+-rw-r--r--   0 sax        (501) staff       (20)       72 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/coverage/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     1171 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/coverage/tracer.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.227501 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/cssselect/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/cssselect/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.227606 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/exceptiongroup/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.228968 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)   134880 2024-05-04 05:15:43.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/faker/proxy.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:43.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.229064 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.229156 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.229244 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.229335 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.101832 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.229573 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.229665 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.229755 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.229845 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.229936 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.230029 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.230124 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.230216 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.230313 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.230408 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.230506 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.230597 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.230851 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      286 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.102030 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.102383 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.230949 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.231967 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    20105 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     4056 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.232097 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.232188 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.232287 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.232378 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pluggy/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pluggy/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.232720 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pyproject_api/
+-rw-r--r--   0 sax        (501) staff       (20)      535 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pyproject_api/_backend.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.232817 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.232910 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.103059 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.103601 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.233011 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.233102 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.233848 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    14977 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     3551 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.234073 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.234168 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:15:37.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/setuptools/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.234434 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:41.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.234523 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:15:41.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.234753 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/tox/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:15:42.000000 django_admin_extra_buttons-1.5.8/.tox/d42-py39/lib/python3.9/site-packages/tox/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.104110 django_admin_extra_buttons-1.5.8/.tox/d50-py311/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.104205 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.104283 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.109214 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.234847 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.234944 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:21.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.237088 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)    16976 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attr/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      399 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attr/_cmp.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      469 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attr/_typing_compat.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      209 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attr/_version_info.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      406 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attr/converters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      539 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attr/exceptions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      225 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attr/filters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attr/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      567 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attr/setters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2580 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attr/validators.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.237354 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)     2168 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attrs/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.237443 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.237778 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 sax        (501) staff       (20)       72 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/coverage/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     1171 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/coverage/tracer.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.238005 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/cssselect/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/cssselect/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.239189 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)   134880 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/faker/proxy.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.239291 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.239380 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.239478 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.239567 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.107051 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.239820 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.239912 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.240012 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.240108 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.240202 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.240303 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.240396 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.240498 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.240597 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.240695 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.240789 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.240879 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.241143 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      286 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.107278 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.107714 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.241243 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.242500 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    20105 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     4056 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.242634 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.242728 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.242817 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.242906 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pluggy/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:24.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pluggy/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.243267 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 sax        (501) staff       (20)      535 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pyproject_api/_backend.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.243369 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.243459 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.108470 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.108975 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.243552 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.243646 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.244384 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    14977 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     3551 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.244620 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.244719 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:22:20.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/setuptools/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.244945 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:24.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.245040 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:25.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py311/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.109425 django_admin_extra_buttons-1.5.8/.tox/d50-py312/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.109501 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.109577 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.112830 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.245132 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.245224 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:35.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.247203 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)    16976 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attr/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      399 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attr/_cmp.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      469 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attr/_typing_compat.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      209 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attr/_version_info.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      406 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attr/converters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      539 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attr/exceptions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      225 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attr/filters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attr/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      567 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attr/setters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2580 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attr/validators.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.247464 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)     2168 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attrs/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.247563 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.247920 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/coverage/
+-rw-r--r--   0 sax        (501) staff       (20)       72 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/coverage/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     1171 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/coverage/tracer.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.248151 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/cssselect/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/cssselect/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.248969 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)   134880 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/faker/proxy.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.249070 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.249158 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.249262 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.249354 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.112230 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.249638 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.249734 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.249826 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.249918 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.250015 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.250115 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.250206 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.250298 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.250390 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.250490 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.250587 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.250681 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.250950 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      286 2024-05-04 05:22:34.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.251049 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.251139 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pluggy/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pluggy/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.251497 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pyproject_api/
+-rw-r--r--   0 sax        (501) staff       (20)      535 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pyproject_api/_backend.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.251594 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.251689 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.251779 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:38.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.251876 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/tox/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:22:39.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py312/lib/python3.12/site-packages/tox/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.113018 django_admin_extra_buttons-1.5.8/.tox/d50-py39/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.113094 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.113166 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.114830 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.251981 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.114305 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.252249 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.252341 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.252441 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.252536 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.252631 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.252725 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.252815 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.252910 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.253004 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.253099 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.253194 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.253286 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.253549 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      286 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.114449 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.114749 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.253645 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.254702 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    20105 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     4056 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.254928 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.255023 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.114894 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.115277 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.255121 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.255215 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.255919 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    14977 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     3551 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.256140 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.256233 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 05:16:12.000000 django_admin_extra_buttons-1.5.8/.tox/d50-py39/lib/python3.9/site-packages/setuptools/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.115421 django_admin_extra_buttons-1.5.8/.tox/docs/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.115484 django_admin_extra_buttons-1.5.8/.tox/docs/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.115547 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.115993 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.256509 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/click/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-20 12:53:29.000000 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/click/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.256619 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-20 12:53:29.000000 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.256727 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/jinja2/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-20 12:53:29.000000 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/jinja2/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.256836 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/markupsafe/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-20 12:53:28.000000 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.256940 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-20 12:53:29.000000 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.257043 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-20 12:53:17.000000 django_admin_extra_buttons-1.5.8/.tox/docs/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.116131 django_admin_extra_buttons-1.5.8/.tox/package/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.116193 django_admin_extra_buttons-1.5.8/.tox/package/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.116254 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.117912 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.257326 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:28.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.257416 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:28.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/attr/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.257516 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:28.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.257620 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/build/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:18.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/build/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.257726 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/charset_normalizer/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:18.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.257822 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:28.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.257911 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:28.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.258010 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:18.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.258104 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:18.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.258202 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:26.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.258295 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/keyring/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:18.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/keyring/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.258385 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:28.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.258485 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 sax        (501) staff       (20)      286 2022-02-19 09:57:12.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.258685 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:27.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.258778 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/py/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.117530 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.258868 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:27.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:27.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/py/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.258956 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:28.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.259044 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:30.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.259136 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:26.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.259232 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2022-02-19 09:57:26.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.259523 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/twine/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-19 09:57:18.000000 django_admin_extra_buttons-1.5.8/.tox/package/lib/python3.9/site-packages/twine/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.118067 django_admin_extra_buttons-1.5.8/.venv/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.118130 django_admin_extra_buttons-1.5.8/.venv/lib/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.118191 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.128991 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.259640 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/_pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/_pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.259752 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/asgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/asgiref/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.262202 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attr/
+-rw-r--r--   0 sax        (501) staff       (20)    16976 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attr/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      399 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attr/_cmp.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      469 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attr/_typing_compat.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      209 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attr/_version_info.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      406 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attr/converters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      539 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attr/exceptions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      225 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attr/filters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attr/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      567 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attr/setters.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2580 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attr/validators.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.262500 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attrs/
+-rw-r--r--   0 sax        (501) staff       (20)     2168 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attrs/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/attrs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.262609 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/babel/
+-rw-r--r--   0 sax        (501) staff       (20)       59 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/babel/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.262845 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/build/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:42.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/build/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.262956 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/certifi/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/certifi/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.263065 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.263177 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/charset_normalizer/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.263285 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/click/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/click/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.263666 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/coverage/
+-rw-r--r--   0 sax        (501) staff       (20)       72 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/coverage/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     1171 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/coverage/tracer.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.263901 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/cssselect/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/cssselect/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.263991 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/faker/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:56.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/faker/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.264085 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/filelock/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/filelock/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.264176 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.264270 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/iniconfig/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.264375 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/isort/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.119521 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/isort/_vendored/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.264479 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/isort/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.264764 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/jinja2/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:41.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/jinja2/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.265108 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/markupsafe/
+-rw-r--r--   0 sax        (501) staff       (20)      229 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/markupsafe/_speedups.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.265212 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mkdocs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:56.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mkdocs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.265321 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/
+-rw-r--r--   0 sax        (501) staff       (20)       64 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.124362 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.321774 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/
+-rw-r--r--   0 sax        (501) staff       (20)      915 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/__future__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       63 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/__main__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    15576 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_ast.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2651 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_bisect.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       64 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_bootlocale.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6961 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_codecs.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2479 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_collections_abc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      356 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_compat_pickle.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      816 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_compression.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2499 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_csv.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     8139 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_ctypes.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    15379 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_curses.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    13802 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_decimal.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1252 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_dummy_thread.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5087 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_dummy_threading.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      337 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_heapq.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1121 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_imp.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1452 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_json.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2264 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_locale.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1264 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_lsprof.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      722 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_markupbase.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3260 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_msi.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6044 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_operator.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1865 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_osx_support.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      931 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_posixsubprocess.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      397 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_py_abc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      895 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_pydecimal.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      408 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_random.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      518 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_sitebuiltins.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    21634 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_socket.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2902 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_stat.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2005 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_thread.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      516 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_threading_local.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3976 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_tkinter.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      548 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_tracemalloc.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.322714 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_typeshed/
+-rw-r--r--   0 sax        (501) staff       (20)    11408 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_typeshed/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1636 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_typeshed/dbapi.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1637 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_typeshed/wsgi.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      499 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_typeshed/xml.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1562 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_warnings.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1428 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_weakref.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2361 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_weakrefset.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     9390 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/_winapi.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2023 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/abc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3354 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/aifc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      123 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/antigravity.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    22493 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/argparse.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4058 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/array.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    11480 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ast.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      787 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asynchat.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.331546 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/
+-rw-r--r--   0 sax        (501) staff       (20)     1181 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    17849 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/base_events.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      719 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/base_futures.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2680 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/base_subprocess.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      404 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/base_tasks.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      568 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/constants.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1031 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/coroutines.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    22233 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/events.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1099 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/exceptions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      887 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/format_helpers.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2329 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/futures.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4288 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/locks.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       39 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/log.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      215 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/mixins.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2532 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/proactor_events.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1631 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/protocols.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1544 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/queues.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1141 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/runners.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      223 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/selector_events.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6356 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/sslproto.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      341 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/staggered.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5807 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/streams.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     9237 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/subprocess.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      794 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/taskgroups.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    18566 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/tasks.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      266 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/threads.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      653 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/timeouts.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2040 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/transports.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4644 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/trsock.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     8856 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/unix_events.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4070 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/windows_events.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1941 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncio/windows_utils.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3670 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/asyncore.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      392 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/atexit.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2085 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/audioop.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2188 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/base64.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4641 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/bdb.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1526 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/binascii.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1279 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/binhex.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       67 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/bisect.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    81291 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/builtins.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4872 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/bz2.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1298 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/cProfile.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     7327 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/calendar.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3700 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/cgi.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1394 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/cgitb.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      614 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/chunk.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1175 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/cmath.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1725 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/cmd.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1481 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/code.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    11812 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/codecs.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      466 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/codeop.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.331871 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/collections/
+-rw-r--r--   0 sax        (501) staff       (20)    23112 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/collections/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       79 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/collections/abc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      648 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/colorsys.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3441 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/compileall.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.332005 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/concurrent/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/concurrent/__init__.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.332628 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/concurrent/futures/
+-rw-r--r--   0 sax        (501) staff       (20)      818 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/concurrent/futures/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4593 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/concurrent/futures/_base.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     7977 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/concurrent/futures/process.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2326 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/concurrent/futures/thread.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    12657 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/configparser.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     8930 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/contextlib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2163 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/contextvars.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      350 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/copy.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      983 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/copyreg.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      383 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/crypt.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4323 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/csv.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.333504 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ctypes/
+-rw-r--r--   0 sax        (501) staff       (20)     6646 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ctypes/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      757 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ctypes/_endian.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      129 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ctypes/util.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6341 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ctypes/wintypes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.334456 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/curses/
+-rw-r--r--   0 sax        (501) staff       (20)      653 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/curses/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1127 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/curses/ascii.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       40 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/curses/has_key.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      816 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/curses/panel.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      443 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/curses/textpad.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     9326 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/dataclasses.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    10818 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/datetime.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.335053 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/dbm/
+-rw-r--r--   0 sax        (501) staff       (20)     1787 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/dbm/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1287 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/dbm/dumb.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1663 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/dbm/gnu.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1449 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/dbm/ndbm.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      117 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/decimal.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4557 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/difflib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4646 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/dis.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.339439 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/
+-rw-r--r--   0 sax        (501) staff       (20)      351 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      545 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/archive_util.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       78 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/bcppcompiler.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6346 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/ccompiler.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2896 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/cmd.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.343162 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      540 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/bdist.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      450 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_dumb.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1494 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_msi.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_packager.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1104 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_rpm.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      639 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_wininst.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      711 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/build.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      668 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/build_clib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1293 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/build_ext.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1442 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/build_py.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      574 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/build_scripts.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1092 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/check.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      377 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/clean.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2679 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/config.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1689 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/install.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      436 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/install_data.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      490 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/install_egg_info.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      387 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/install_headers.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      598 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/install_lib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      426 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/install_scripts.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      570 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/register.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1118 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/sdist.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      462 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/command/upload.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      497 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/config.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1849 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/core.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      534 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/cygwinccompiler.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       19 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/debug.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      224 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/dep_util.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      510 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/dir_util.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5879 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/dist.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      852 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/errors.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1236 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/extension.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1162 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/fancy_getopt.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      429 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/file_util.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2175 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/filelist.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      843 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/log.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       78 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/msvccompiler.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      187 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/spawn.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1113 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/sysconfig.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      682 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/text_file.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       79 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/unixccompiler.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1550 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/util.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1308 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/distutils/version.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     7401 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/doctest.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       79 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/dummy_threading.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.346874 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/
+-rw-r--r--   0 sax        (501) staff       (20)     1054 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    11135 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/_header_value_parser.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1971 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/_policybase.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      559 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/base64mime.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1274 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/charset.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      480 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      293 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/encoders.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1533 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/errors.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      956 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/feedparser.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1175 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/generator.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1265 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/header.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6129 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/headerregistry.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      648 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/iterators.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     8423 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/message.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.348574 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/mime/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/mime/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      498 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/mime/application.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      482 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/mime/audio.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      271 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/mime/base.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      482 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/mime/image.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      294 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/mime/message.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      485 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/mime/multipart.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      108 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/mime/nonmultipart.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      293 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/mime/text.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1328 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/parser.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1390 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/policy.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      835 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/quoprimime.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2578 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/email/utils.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.349270 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/encodings/
+-rw-r--r--   0 sax        (501) staff       (20)      309 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/encodings/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      896 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/encodings/utf_8.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1059 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/encodings/utf_8_sig.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.349706 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ensurepip/
+-rw-r--r--   0 sax        (501) staff       (20)      264 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ensurepip/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    11274 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/enum.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3957 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/errno.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      644 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/faulthandler.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3796 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/fcntl.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1936 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/filecmp.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     7161 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/fileinput.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      339 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/fnmatch.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3711 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/formatter.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5092 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/fractions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6535 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ftplib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     8281 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/functools.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1200 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/gc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1924 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/genericpath.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      439 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/getopt.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      227 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/getpass.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6121 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/gettext.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1421 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/glob.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      914 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/graphlib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      702 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/grp.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4861 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/gzip.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5036 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/hashlib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      760 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/heapq.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1343 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/hmac.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.350340 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/html/
+-rw-r--r--   0 sax        (501) staff       (20)      157 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/html/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      182 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/html/entities.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1714 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/html/parser.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.351457 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/http/
+-rw-r--r--   0 sax        (501) staff       (20)     2674 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/http/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     8396 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/http/client.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6688 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/http/cookiejar.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2312 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/http/cookies.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3471 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/http/server.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     7857 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/imaplib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      507 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/imghdr.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2383 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/imp.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.353168 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/
+-rw-r--r--   0 sax        (501) staff       (20)      849 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      609 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/_abc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6887 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/abc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     7004 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/machinery.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.353724 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/metadata/
+-rw-r--r--   0 sax        (501) staff       (20)     9284 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2010 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2584 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/readers.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.354309 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/resources/
+-rw-r--r--   0 sax        (501) staff       (20)     1678 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/resources/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      476 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/resources/abc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      398 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/resources/readers.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2200 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/resources/simple.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      354 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/simple.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1826 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/importlib/util.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    20241 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/inspect.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     9705 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/io.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     7328 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ipaddress.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    11055 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/itertools.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.354826 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/json/
+-rw-r--r--   0 sax        (501) staff       (20)     2061 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/json/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1117 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/json/decoder.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1195 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/json/encoder.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       24 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/json/tool.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      565 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/keyword.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.355817 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      860 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/btm_matcher.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1692 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixer_base.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.368703 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      215 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_apply.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      245 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_asserts.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      240 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_basestring.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      224 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_buffer.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      424 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_dict.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      415 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_except.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      214 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_exec.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      218 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_execfile.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      445 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_exitfunc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      280 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_filter.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      227 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_funcattrs.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      216 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_future.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      225 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_getcwdu.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      216 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_has_key.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      438 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_idioms.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      507 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_import.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      639 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_imports.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      117 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_imports2.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      269 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_input.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      252 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_intern.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      228 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_isinstance.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      245 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_itertools.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      230 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_itertools_imports.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      240 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_long.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      274 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_map.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      587 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_metaclass.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      250 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_methodattrs.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      217 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_ne.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      518 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_next.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      225 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_nonzero.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      226 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_numliterals.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      312 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_operator.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      223 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_paren.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      334 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_print.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      215 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_raise.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      226 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_raw_input.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      264 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_reduce.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      252 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_reload.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      486 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_renames.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      214 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_repr.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      224 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_set_literal.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      223 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_standarderror.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      250 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_sys_exc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      223 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_throw.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      505 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_tuple_params.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      215 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_types.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      468 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_unicode.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      542 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_urllib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      304 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_ws_comma.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      726 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_xrange.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      228 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_xreadlines.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      274 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/fixes/fix_zip.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1532 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/main.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.370464 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/
+-rw-r--r--   0 sax        (501) staff       (20)      287 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1067 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/driver.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      682 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/grammar.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      151 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/literals.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1133 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/parse.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2206 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/pgen.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      958 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/token.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1972 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/tokenize.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2253 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/pygram.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4118 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/pytree.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3946 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lib2to3/refactor.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      958 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/linecache.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4341 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/locale.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.371619 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/logging/
+-rw-r--r--   0 sax        (501) staff       (20)    19986 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/logging/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5742 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/logging/config.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     9607 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/logging/handlers.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5344 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/lzma.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    10459 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/mailbox.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      388 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/mailcap.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      839 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/marshal.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4838 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/math.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1672 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/mimetypes.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4003 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/mmap.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3294 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/modulefinder.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.372560 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/msilib/
+-rw-r--r--   0 sax        (501) staff       (20)     5853 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/msilib/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2141 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/msilib/schema.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      362 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/msilib/sequence.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      170 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/msilib/text.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1166 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/msvcrt.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.377750 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/
+-rw-r--r--   0 sax        (501) staff       (20)     3132 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2969 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/connection.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     7821 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/context.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.378013 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/
+-rw-r--r--   0 sax        (501) staff       (20)     1935 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1282 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/connection.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1058 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/forkserver.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1046 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/heap.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     8899 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/managers.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3888 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/pool.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      724 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/popen_fork.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      353 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/popen_forkserver.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      524 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/popen_spawn_posix.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      738 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/popen_spawn_win32.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1177 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/process.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1487 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/queues.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3135 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/reduction.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      420 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/resource_sharer.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      609 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/resource_tracker.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1389 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/shared_memory.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4200 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/sharedctypes.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      861 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/spawn.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2122 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/synchronize.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2810 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/multiprocessing/util.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      745 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/netrc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      293 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/nis.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4490 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/nntplib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3273 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/nt.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2873 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ntpath.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       76 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/nturl2path.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     7370 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/numbers.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1272 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/opcode.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1644 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/operator.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    10527 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/optparse.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.378675 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/os/
+-rw-r--r--   0 sax        (501) staff       (20)    40258 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/os/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      186 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/os/path.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3589 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ossaudiodev.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1017 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/parser.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     9022 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pathlib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     7549 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pdb.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5727 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pickle.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3813 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pickletools.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      502 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pipes.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1914 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pkgutil.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1660 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/platform.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3724 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/plistlib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2487 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/poplib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    12107 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/posix.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4643 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/posixpath.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2984 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pprint.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1401 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/profile.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2804 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pstats.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      697 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pty.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      905 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pwd.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      897 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/py_compile.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2284 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pyclbr.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    10881 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pydoc.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.379001 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pydoc_data/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pydoc_data/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       23 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pydoc_data/topics.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.379660 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pyexpat/
+-rw-r--r--   0 sax        (501) staff       (20)     3549 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pyexpat/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1477 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pyexpat/errors.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      205 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/pyexpat/model.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2290 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/queue.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      635 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/quopri.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5012 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/random.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    11314 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/re.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1875 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/readline.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1986 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/reprlib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2804 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/resource.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      322 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/rlcompleter.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      811 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/runpy.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1333 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sched.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      624 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/secrets.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4544 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/select.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2782 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/selectors.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1892 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/shelve.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2206 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/shlex.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6892 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/shutil.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5404 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/signal.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1358 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/site.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2998 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/smtpd.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6724 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/smtplib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      353 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sndhdr.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    29277 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/socket.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6732 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/socketserver.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1153 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/spwd.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.380104 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sqlite3/
+-rw-r--r--   0 sax        (501) staff       (20)       29 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sqlite3/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    19822 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sqlite3/dbapi2.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      332 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sre_compile.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3986 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sre_constants.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3790 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sre_parse.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    19244 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/ssl.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       20 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/stat.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4803 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/statistics.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3108 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/string.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      910 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/stringprep.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1271 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/struct.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    90809 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/subprocess.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2937 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sunau.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1467 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/symbol.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2146 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/symtable.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.381141 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sys/
+-rw-r--r--   0 sax        (501) staff       (20)    12402 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sys/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1492 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sys/_monitoring.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1569 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/sysconfig.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1347 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/syslog.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      514 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tabnanny.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    14357 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tarfile.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2862 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/telnetlib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    16453 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tempfile.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5168 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/termios.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3233 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/textwrap.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       25 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/this.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5932 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/threading.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3682 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/time.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1240 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/timeit.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.384636 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/
+-rw-r--r--   0 sax        (501) staff       (20)   137438 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      654 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/colorchooser.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      398 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/commondialog.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1875 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/constants.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      401 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/dialog.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      786 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/dnd.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5203 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/filedialog.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4344 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/font.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1321 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/messagebox.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      302 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/scrolledtext.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1596 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/simpledialog.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    14405 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/tix.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    45734 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tkinter/ttk.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2494 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/token.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4268 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tokenize.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      376 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tomllib.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3448 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/trace.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     9056 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/traceback.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4575 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tracemalloc.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      822 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/tty.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    22749 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/turtle.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    20405 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/types.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    33870 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/typing.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    15184 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/typing_extensions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2575 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unicodedata.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.387555 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/
+-rw-r--r--   0 sax        (501) staff       (20)     1813 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      912 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/_log.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      738 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/async_case.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    14662 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/case.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2181 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/loader.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2430 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/main.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    14562 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/mock.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2029 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/result.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2506 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/runner.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      488 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      983 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1009 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/unittest/util.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.389634 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/urllib/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      816 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/urllib/error.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6532 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    18009 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/urllib/request.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1635 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/urllib/response.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      683 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/urllib/robotparser.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      431 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/uu.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2677 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/uuid.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.389887 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/venv/
+-rw-r--r--   0 sax        (501) staff       (20)     2665 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/venv/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3682 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/warnings.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3240 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/wave.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6350 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/weakref.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2563 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/webbrowser.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     5494 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/winreg.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      956 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/winsound.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.391304 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/wsgiref/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/wsgiref/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3068 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/wsgiref/handlers.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1036 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/wsgiref/headers.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1398 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/wsgiref/simple_server.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1260 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/wsgiref/types.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      995 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/wsgiref/util.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1737 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/wsgiref/validate.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2368 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xdrlib.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.391536 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/
+-rw-r--r--   0 sax        (501) staff       (20)       35 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/__init__.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.393019 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/dom/
+-rw-r--r--   0 sax        (501) staff       (20)      457 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/dom/NodeFilter.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1889 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/dom/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      418 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/dom/domreg.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4847 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/dom/expatbuilder.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      678 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/dom/minicompat.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    15066 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/dom/minidom.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3453 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/dom/pulldom.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     4199 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/dom/xmlbuilder.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.393893 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/etree/
+-rw-r--r--   0 sax        (501) staff       (20)      983 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/etree/ElementInclude.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1636 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/etree/ElementPath.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    12618 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/etree/ElementTree.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/etree/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       36 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/etree/cElementTree.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.394036 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/parsers/
+-rw-r--r--   0 sax        (501) staff       (20)       39 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/parsers/__init__.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.395161 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/
+-rw-r--r--   0 sax        (501) staff       (20)       22 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       29 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/errors.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       28 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/model.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.395859 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/sax/
+-rw-r--r--   0 sax        (501) staff       (20)     1148 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/sax/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      755 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/sax/_exceptions.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2102 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/sax/handler.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3187 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/sax/saxutils.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3829 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xml/sax/xmlreader.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.396347 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xmlrpc/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xmlrpc/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    11757 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xmlrpc/client.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     6065 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xmlrpc/server.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      423 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/xxlimited.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      553 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/zipapp.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.396846 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/zipfile/
+-rw-r--r--   0 sax        (501) staff       (20)    10211 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/zipfile/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     3640 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/zipfile/_path.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1349 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/zipimport.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1777 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/zlib.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.396980 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/zoneinfo/
+-rw-r--r--   0 sax        (501) staff       (20)     1517 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stdlib/zoneinfo/__init__.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.124481 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stubs/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.397200 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stubs/mypy-extensions/
+-rw-r--r--   0 sax        (501) staff       (20)     8892 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypy/typeshed/stubs/mypy-extensions/mypy_extensions.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.124720 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypyc/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.124806 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypyc/test-data/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.397512 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypyc/test-data/fixtures/
+-rw-r--r--   0 sax        (501) staff       (20)     4969 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/mypyc/test-data/fixtures/typing-full.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.397957 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/nh3/
+-rw-r--r--   0 sax        (501) staff       (20)      789 2024-05-04 04:26:37.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/nh3/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:37.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/nh3/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.398055 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.398147 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pathspec/
+-rw-r--r--   0 sax        (501) staff       (20)       68 2024-04-13 16:16:52.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pathspec/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.398409 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.126629 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.398619 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.398720 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.398816 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.398909 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.399014 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.399115 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.399215 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.399310 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.399407 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.399508 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.399605 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.399702 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.399946 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      286 2024-05-04 04:26:39.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pip/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.400037 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/piptools/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:42.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/piptools/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.126915 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.127426 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.400129 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.127153 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/jaraco/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.400463 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/jaraco/functools/
+-rw-r--r--   0 sax        (501) staff       (20)     3982 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/jaraco/functools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/jaraco/functools/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.401411 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    21044 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     4436 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.401646 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.401738 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.401829 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/platformdirs/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:52.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.401919 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pluggy/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:52.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pluggy/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.402307 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pyproject_api/
+-rw-r--r--   0 sax        (501) staff       (20)      535 2024-04-13 16:16:54.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pyproject_api/_backend.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:54.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.402413 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pyproject_hooks/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pyproject_hooks/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.402516 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pytest/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:53.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pytest/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.402612 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pytest_django/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:56.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/pytest_django/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.402710 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/readme_renderer/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:40.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.128187 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.128655 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.402814 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.402914 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.128454 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/jaraco/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.403258 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/jaraco/functools/
+-rw-r--r--   0 sax        (501) staff       (20)     3982 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/jaraco/functools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/jaraco/functools/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.404071 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 sax        (501) staff       (20)       43 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)    14977 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)     3551 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.404206 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.404303 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 sax        (501) staff       (20)       26 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/setuptools/_vendor/tomli/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.404528 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/soupsieve/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:51.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/soupsieve/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.404617 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/sphinx/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:26:42.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/sphinx/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.404711 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/tox/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:55.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/tox/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.404801 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/urllib3/
+-rw-r--r--   0 sax        (501) staff       (20)       93 2024-05-04 04:26:38.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/urllib3/py.typed
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.405047 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/watchdog/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-04-13 16:16:51.000000 django_admin_extra_buttons-1.5.8/.venv/lib/python3.12/site-packages/watchdog/py.typed
+-rw-r--r--   0 sax        (501) staff       (20)      899 2024-05-04 05:48:04.000000 django_admin_extra_buttons-1.5.8/CHANGES
+-rw-r--r--   0 sax        (501) staff       (20)     1164 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/LICENSE
+-rw-r--r--   0 sax        (501) staff       (20)      329 2024-05-04 05:09:08.000000 django_admin_extra_buttons-1.5.8/MANIFEST.in
+-rw-r--r--   0 sax        (501) staff       (20)     6149 2024-05-04 05:57:35.421728 django_admin_extra_buttons-1.5.8/PKG-INFO
+-rw-r--r--   0 sax        (501) staff       (20)     3897 2024-05-04 05:09:08.000000 django_admin_extra_buttons-1.5.8/README.md
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.405995 django_admin_extra_buttons-1.5.8/docs/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.407319 django_admin_extra_buttons-1.5.8/docs/api/
+-rw-r--r--   0 sax        (501) staff       (20)     3975 2024-05-04 05:09:08.000000 django_admin_extra_buttons-1.5.8/docs/api/button.md
+-rw-r--r--   0 sax        (501) staff       (20)     2484 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/api/choice.md
+-rw-r--r--   0 sax        (501) staff       (20)      505 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/api/handlers.md
+-rw-r--r--   0 sax        (501) staff       (20)     1995 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/api/link.md
+-rw-r--r--   0 sax        (501) staff       (20)     1075 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/api/mixin.md
+-rw-r--r--   0 sax        (501) staff       (20)        0 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/api/utils.md
+-rw-r--r--   0 sax        (501) staff       (20)      896 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/api/view.md
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.407452 django_admin_extra_buttons-1.5.8/docs/css/
+-rw-r--r--   0 sax        (501) staff       (20)      973 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/css/extra.css
+-rw-r--r--   0 sax        (501) staff       (20)     1340 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/howto.md
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.408439 django_admin_extra_buttons-1.5.8/docs/images/
+-rw-r--r--   0 sax        (501) staff       (20)    28164 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/images/buttons.png
+-rw-r--r--   0 sax        (501) staff       (20)   167645 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/images/screenshot.png
+-rw-r--r--   0 sax        (501) staff       (20)       16 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/index.md
+-rw-r--r--   0 sax        (501) staff       (20)       69 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/requirements.txt
+-rw-r--r--   0 sax        (501) staff       (20)      249 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/docs/to_gif.sh
+-rw-r--r--   0 sax        (501) staff       (20)     1451 2022-02-19 20:21:39.000000 django_admin_extra_buttons-1.5.8/docs/~index.md
+-rw-r--r--   0 sax        (501) staff       (20)      766 2024-05-04 05:57:35.422070 django_admin_extra_buttons-1.5.8/setup.cfg
+-rwxr-xr-x   0 sax        (501) staff       (20)     2835 2024-05-04 05:09:08.000000 django_admin_extra_buttons-1.5.8/setup.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.129799 django_admin_extra_buttons-1.5.8/src/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.410987 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/
+-rw-r--r--   0 sax        (501) staff       (20)       87 2024-05-04 05:48:32.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)      133 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/api.py
+-rw-r--r--   0 sax        (501) staff       (20)       94 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/apps.py
+-rw-r--r--   0 sax        (501) staff       (20)     6319 2024-05-04 05:09:08.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/buttons.py
+-rw-r--r--   0 sax        (501) staff       (20)      818 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/decorators.py
+-rw-r--r--   0 sax        (501) staff       (20)     6065 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/handlers.py
+-rw-r--r--   0 sax        (501) staff       (20)     6383 2024-05-04 05:09:08.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/mixins.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.411682 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/static/
+-rw-r--r--   0 sax        (501) staff       (20)      389 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/static/admin_extra_buttons.css
+-rw-r--r--   0 sax        (501) staff       (20)      216 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/static/admin_extra_buttons.css.map
+-rw-r--r--   0 sax        (501) staff       (20)      957 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/static/admin_extra_buttons.js
+-rw-r--r--   0 sax        (501) staff       (20)      671 2023-11-28 13:09:54.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/static/admin_extra_buttons.min.js
+-rw-r--r--   0 sax        (501) staff       (20)      478 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/static/admin_extra_buttons.scss
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.129598 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.412201 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/
+-rw-r--r--   0 sax        (501) staff       (20)     1228 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/action_page.html
+-rw-r--r--   0 sax        (501) staff       (20)      350 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/change_form.html
+-rw-r--r--   0 sax        (501) staff       (20)      279 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/change_list.html
+-rw-r--r--   0 sax        (501) staff       (20)      990 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/confirm.html
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.412992 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/includes/
+-rw-r--r--   0 sax        (501) staff       (20)      226 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/includes/action_buttons.html
+-rw-r--r--   0 sax        (501) staff       (20)      178 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/includes/attrs.html
+-rw-r--r--   0 sax        (501) staff       (20)      289 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/includes/button.html
+-rw-r--r--   0 sax        (501) staff       (20)      253 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/includes/change_form_buttons.html
+-rw-r--r--   0 sax        (501) staff       (20)      247 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/includes/change_list_buttons.html
+-rw-r--r--   0 sax        (501) staff       (20)      520 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/includes/choice.html
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.413212 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templatetags/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templatetags/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)      779 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templatetags/extra_buttons.py
+-rw-r--r--   0 sax        (501) staff       (20)     3825 2023-11-28 13:11:14.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/utils.py
+-rw-r--r--   0 sax        (501) staff       (20)     4159 2022-02-18 06:02:55.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/~button.p_
+-rw-r--r--   0 sax        (501) staff       (20)      503 2022-02-18 06:02:55.000000 django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/~config.p_
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.420471 django_admin_extra_buttons-1.5.8/src/django_admin_extra_buttons.egg-info/
+-rw-r--r--   0 sax        (501) staff       (20)     6149 2024-05-04 05:57:19.000000 django_admin_extra_buttons-1.5.8/src/django_admin_extra_buttons.egg-info/PKG-INFO
+-rw-r--r--   0 sax        (501) staff       (20)   106731 2024-05-04 05:57:35.000000 django_admin_extra_buttons-1.5.8/src/django_admin_extra_buttons.egg-info/SOURCES.txt
+-rw-r--r--   0 sax        (501) staff       (20)        1 2024-05-04 05:57:19.000000 django_admin_extra_buttons-1.5.8/src/django_admin_extra_buttons.egg-info/dependency_links.txt
+-rw-r--r--   0 sax        (501) staff       (20)      282 2024-05-04 05:57:19.000000 django_admin_extra_buttons-1.5.8/src/django_admin_extra_buttons.egg-info/requires.txt
+-rw-r--r--   0 sax        (501) staff       (20)       20 2024-05-04 05:57:19.000000 django_admin_extra_buttons-1.5.8/src/django_admin_extra_buttons.egg-info/top_level.txt
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.129922 django_admin_extra_buttons-1.5.8/stubs/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.415286 django_admin_extra_buttons-1.5.8/stubs/admin_extra_buttons/
+-rw-r--r--   0 sax        (501) staff       (20)       40 2024-05-04 04:58:16.000000 django_admin_extra_buttons-1.5.8/stubs/admin_extra_buttons/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      180 2024-05-04 04:58:16.000000 django_admin_extra_buttons-1.5.8/stubs/admin_extra_buttons/api.pyi
+-rw-r--r--   0 sax        (501) staff       (20)       74 2024-05-04 04:58:16.000000 django_admin_extra_buttons-1.5.8/stubs/admin_extra_buttons/apps.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1854 2024-05-04 04:58:16.000000 django_admin_extra_buttons-1.5.8/stubs/admin_extra_buttons/buttons.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      242 2024-05-04 04:58:16.000000 django_admin_extra_buttons-1.5.8/stubs/admin_extra_buttons/decorators.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     2206 2024-05-04 04:58:16.000000 django_admin_extra_buttons-1.5.8/stubs/admin_extra_buttons/handlers.pyi
+-rw-r--r--   0 sax        (501) staff       (20)     1425 2024-05-04 04:58:16.000000 django_admin_extra_buttons-1.5.8/stubs/admin_extra_buttons/mixins.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.415534 django_admin_extra_buttons-1.5.8/stubs/admin_extra_buttons/templatetags/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2024-05-04 04:58:16.000000 django_admin_extra_buttons-1.5.8/stubs/admin_extra_buttons/templatetags/__init__.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      252 2024-05-04 04:58:16.000000 django_admin_extra_buttons-1.5.8/stubs/admin_extra_buttons/templatetags/extra_buttons.pyi
+-rw-r--r--   0 sax        (501) staff       (20)      555 2024-05-04 04:58:16.000000 django_admin_extra_buttons-1.5.8/stubs/admin_extra_buttons/utils.pyi
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.418563 django_admin_extra_buttons-1.5.8/tests/
+-rw-r--r--   0 sax        (501) staff       (20)      625 2024-04-09 00:27:35.000000 django_admin_extra_buttons-1.5.8/tests/.coveragerc
+-rw-r--r--   0 sax        (501) staff       (20)   163840 2024-04-09 00:27:35.000000 django_admin_extra_buttons-1.5.8/tests/.db.sqlite
+-rw-r--r--   0 sax        (501) staff       (20)     1195 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/conftest.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.130186 django_admin_extra_buttons-1.5.8/tests/demoapp/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.419644 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)     6282 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/admin.py
+-rw-r--r--   0 sax        (501) staff       (20)      626 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/backends.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.420041 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/migrations/
+-rw-r--r--   0 sax        (501) staff       (20)     1385 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/migrations/0001_initial.py
+-rw-r--r--   0 sax        (501) staff       (20)     1353 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/migrations/0002_demomodel5_alter_demomodel1_options_and_more.py
+-rw-r--r--   0 sax        (501) staff       (20)        0 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/migrations/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)     1209 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/models.py
+-rw-r--r--   0 sax        (501) staff       (20)     1670 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/settings.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.130470 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/templates/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.420150 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/templates/admin_extra_buttons/
+-rw-r--r--   0 sax        (501) staff       (20)      376 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/templates/admin_extra_buttons/upload.html
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2024-05-04 05:57:35.420279 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/templates/demo/
+-rw-r--r--   0 sax        (501) staff       (20)       53 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/templates/demo/test22.html
+-rw-r--r--   0 sax        (501) staff       (20)     1725 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/upload.py
+-rw-r--r--   0 sax        (501) staff       (20)      237 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/demoapp/demo/urls.py
+-rwxr-xr-x   0 sax        (501) staff       (20)      335 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/manage.py
+-rw-r--r--   0 sax        (501) staff       (20)      195 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/test_admin.py
+-rw-r--r--   0 sax        (501) staff       (20)     3505 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/test_buttons.py
+-rw-r--r--   0 sax        (501) staff       (20)      456 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/test_checks.py
+-rw-r--r--   0 sax        (501) staff       (20)     1089 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/test_choices.py
+-rw-r--r--   0 sax        (501) staff       (20)     1060 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/test_confirm.py
+-rw-r--r--   0 sax        (501) staff       (20)      827 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/test_links.py
+-rw-r--r--   0 sax        (501) staff       (20)      786 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/test_mixin.py
+-rw-r--r--   0 sax        (501) staff       (20)      534 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/test_templatetags.py
+-rw-r--r--   0 sax        (501) staff       (20)      688 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/test_upload.py
+-rw-r--r--   0 sax        (501) staff       (20)     1200 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/test_utils.py
+-rw-r--r--   0 sax        (501) staff       (20)     1397 2023-11-28 13:09:39.000000 django_admin_extra_buttons-1.5.8/tests/test_views.py
+-rw-r--r--   0 sax        (501) staff       (20)     1158 2024-05-04 05:20:10.000000 django_admin_extra_buttons-1.5.8/tox.ini
```

### Comparing `django-admin-extra-buttons-1.5.7/CHANGES` & `django_admin_extra_buttons-1.5.8/CHANGES`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+1.5.8
+-----
+* add common css class
+* fixes permissions check
+
+
 1.5.7
 -----
 * BUG FIX: fixes check() implementation
 * Allow any HttpResponse as return value
 
 
 1.5.6
```

### Comparing `django-admin-extra-buttons-1.5.7/LICENSE` & `django_admin_extra_buttons-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/PKG-INFO` & `django_admin_extra_buttons-1.5.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,8 @@
-Metadata-Version: 2.1
-Name: django-admin-extra-buttons
-Version: 1.5.7
-Summary: Django mixin to easily add buttons to any ModelAdmin
-Home-page: https://github.com/saxix/django-admin-extra-buttons
-Download-URL: https://pypi.python.org/pypi/django-admin-extra-buttons
-License: UNKNOWN
-Platform: linux
-Classifier: Environment :: Web Environment
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Developers
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
-django-admin-extra-buttons
+ django-admin-extra-buttons
 ==========================
 
 
 [![Pypi](https://badge.fury.io/py/django-admin-extra-buttons.svg)](https://badge.fury.io/py/django-admin-extra-buttons)
 [![coverage](https://codecov.io/github/saxix/django-admin-extra-buttons/coverage.svg?branch=develop)](https://codecov.io/github/saxix/django-admin-extra-buttons?branch=develop)
 [![Test](https://github.com/saxix/django-admin-extra-buttons/actions/workflows/test.yml/badge.svg)](https://github.com/saxix/django-admin-extra-buttons/actions/workflows/test.yml)
 [![Docs](https://github.com/saxix/django-admin-extra-buttons/actions/workflows/docs.yml/badge.svg)](https://github.com/saxix/django-admin-extra-buttons/actions/workflows/docs.yml)
@@ -72,34 +44,36 @@
 from admin_extra_buttons.api import ExtraButtonsMixin, button, confirm_action, link, view
 from admin_extra_buttons.utils import HttpResponseRedirectToReferrer
 from django.http import HttpResponse, JsonResponse
 from django.contrib import admin
 from django.views.decorators.clickjacking import xframe_options_sameorigin
 from django.views.decorators.csrf import csrf_exempt
 
+
 class MyModelModelAdmin(ExtraButtonsMixin, admin.ModelAdmin):
 
     @button(permission='demo.add_demomodel1',
+            visible=lambda self: self.context["request"].user.is_superuser,
             change_form=True,
             html_attrs={'style': 'background-color:#88FF88;color:black'})
     def refresh(self, request):
         self.message_user(request, 'refresh called')
         # Optional: returns HttpResponse
         return HttpResponseRedirectToReferrer(request)
-    
+
     @button(html_attrs={'style': 'background-color:#DC6C6C;color:black'})
     def confirm(self, request):
         def _action(request):
             pass
 
         return confirm_action(self, request, _action, "Confirm action",
-                          "Successfully executed", )
+                              "Successfully executed", )
 
-    @link(href=None, 
-          change_list=False, 
+    @link(href=None,
+          change_list=False,
           html_attrs={'target': '_new', 'style': 'background-color:var(--button-bg)'})
     def search_on_google(self, button):
         original = button.context['original']
         button.label = f"Search '{original.name}' on Google"
         button.href = f"https://www.google.com/?q={original.name}"
 
     @view()
@@ -111,20 +85,18 @@
         return HttpResponse("Basic Authentication allowed")
 
     @view(decorators=[csrf_exempt, xframe_options_sameorigin])
     def preview(self, request):
         if request.method == "POST":
             return HttpResponse("POST")
         return HttpResponse("GET")
-            
+
 
 ```
 
 #### Project Links
 
 
 - Code: https://github.com/saxix/django-admin-extra-buttons
 - Documentation: https://saxix.github.io/django-admin-extra-buttons/
 - Issue Tracker: https://github.com/saxix/django-admin-extra-buttons/issues
 - Download Package: https://pypi.org/project/django-admin-extra-buttons/
-
-
```

### Comparing `django-admin-extra-buttons-1.5.7/docs/api/button.md` & `django_admin_extra_buttons-1.5.8/docs/api/button.md`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         
         @button(permission=lambda request, obj: request.user.is_superuser)
         def delete_all(self, request):
             pass
 
         @button(permission='app.delete_mymodel)
         def mark(self, request, pk):
-            obj = self.get_object(request.pk)
+            obj = self.get_object(request, pk)
             obj.mark = True
             obj.save()
 
 
 ### Fully featured
 Buttons with custom permission, one for `change_list` and other for `change_form`
```

### Comparing `django-admin-extra-buttons-1.5.7/docs/api/choice.md` & `django_admin_extra_buttons-1.5.8/docs/api/choice.md`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/docs/api/link.md` & `django_admin_extra_buttons-1.5.8/docs/api/link.md`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/docs/api/mixin.md` & `django_admin_extra_buttons-1.5.8/docs/api/mixin.md`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/docs/api/view.md` & `django_admin_extra_buttons-1.5.8/docs/api/view.md`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/docs/css/extra.css` & `django_admin_extra_buttons-1.5.8/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/docs/howto.md` & `django_admin_extra_buttons-1.5.8/docs/howto.md`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/docs/images/buttons.png` & `django_admin_extra_buttons-1.5.8/docs/images/buttons.png`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/docs/images/screenshot.png` & `django_admin_extra_buttons-1.5.8/docs/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/docs/~index.md` & `django_admin_extra_buttons-1.5.8/docs/~index.md`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/setup.cfg` & `django_admin_extra_buttons-1.5.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 known_future_library = future,pies
 known_first_party = admin_extra_buttons
 multi_line_output = 0
 balanced_wrapping = true
 sections = FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
 
 [metadata]
-license-file = LICENSE
+license_file = LICENSE
 
 [wheel]
 universal = 1
 
 [devpi:upload]
 formats = bdist_wheel,sdist.tgz
```

### Comparing `django-admin-extra-buttons-1.5.7/setup.py` & `django_admin_extra_buttons-1.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
                 ]
 dev_require = ['autopep8',
                'bump2version',
                'check-manifest',
                'django',
                'pip-tools',
                'flake8',
+               'mypy',
                'pep8',
                'readme',
                'sphinx',
                'wheel',
                'isort',
                ]
```

### Comparing `django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/buttons.py` & `django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/buttons.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     @property
     def html_attrs(self):
         attrs = self.config.get('html_attrs', {})
         if 'id' not in attrs:
             attrs['id'] = f'btn-{self.handler.func.__name__}'
 
         css_class = attrs.get("class", "")
-
+        css_class += " aeb-button"
         if self.disable_on_click and "aeb-disable-on-click" not in css_class:
             css_class += " aeb-disable-on-click"
         if self.disable_on_edit and "aeb-disable_on_edit" not in css_class:
             css_class += " aeb-disable_on_edit"
 
         css_class = css_class.replace("disabled", "")
         if self.enabled:
```

### Comparing `django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/decorators.py` & `django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/decorators.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/handlers.py` & `django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/handlers.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/mixins.py` & `django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,36 +93,37 @@
             pass
         return errors
 
     def get_common_context(self, request, pk=None, **kwargs):
         opts = self.model._meta
         app_label = opts.app_label
         self.object = None
+        if pk:
+            self.object = self.get_object(request, pk)
 
         context = {
             **self.admin_site.each_context(request),
             **kwargs,
             'opts': opts,
             'add': False,
             'change': True,
             'save_as': False,
+            "original": self.object,
             'extra_buttons': self.extra_button_handlers,
-            'has_delete_permission': self.has_delete_permission(request, pk),
             'has_editable_inline_admin_formsets': False,
-            'has_view_permission': self.has_view_permission(request, pk),
-            'has_change_permission': self.has_change_permission(request, pk),
+            'has_delete_permission': self.has_delete_permission(request, self.object),
+            'has_view_permission': self.has_view_permission(request, self.object),
+            'has_change_permission': self.has_change_permission(request, self.object),
             'has_add_permission': self.has_add_permission(request),
             'app_label': app_label,
             'adminform': DummyAdminform(model_admin=self),
         }
         context.setdefault('title', '')
         context.update(**kwargs)
-        if pk:
-            self.object = self.get_object(request, pk)
-            context['original'] = self.object
+
         return context
 
     def get_extra_urls(self) -> list:
         self.extra_button_handlers = {}
         handlers = {}
         extra_urls = []
         opts = self.model._meta
```

### Comparing `django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/static/admin_extra_buttons.js` & `django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/static/admin_extra_buttons.js`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/static/admin_extra_buttons.min.js` & `django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/static/admin_extra_buttons.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/action_page.html` & `django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/action_page.html`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/confirm.html` & `django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/confirm.html`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templates/admin_extra_buttons/includes/choice.html` & `django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templates/admin_extra_buttons/includes/choice.html`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/templatetags/extra_buttons.py` & `django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/templatetags/extra_buttons.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/utils.py` & `django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/src/admin_extra_buttons/~button.p_` & `django_admin_extra_buttons-1.5.8/src/admin_extra_buttons/~button.p_`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/.coveragerc` & `django_admin_extra_buttons-1.5.8/tests/.coveragerc`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/.db.sqlite` & `django_admin_extra_buttons-1.5.8/tests/.db.sqlite`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/conftest.py` & `django_admin_extra_buttons-1.5.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/demoapp/demo/admin.py` & `django_admin_extra_buttons-1.5.8/tests/demoapp/demo/admin.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/demoapp/demo/backends.py` & `django_admin_extra_buttons-1.5.8/tests/demoapp/demo/backends.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/demoapp/demo/migrations/0001_initial.py` & `django_admin_extra_buttons-1.5.8/tests/demoapp/demo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/demoapp/demo/migrations/0002_demomodel5_alter_demomodel1_options_and_more.py` & `django_admin_extra_buttons-1.5.8/tests/demoapp/demo/migrations/0002_demomodel5_alter_demomodel1_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/demoapp/demo/models.py` & `django_admin_extra_buttons-1.5.8/tests/demoapp/demo/models.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/demoapp/demo/settings.py` & `django_admin_extra_buttons-1.5.8/tests/demoapp/demo/settings.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/demoapp/demo/upload.py` & `django_admin_extra_buttons-1.5.8/tests/demoapp/demo/upload.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/test_buttons.py` & `django_admin_extra_buttons-1.5.8/tests/test_buttons.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/test_choices.py` & `django_admin_extra_buttons-1.5.8/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/test_confirm.py` & `django_admin_extra_buttons-1.5.8/tests/test_confirm.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/test_links.py` & `django_admin_extra_buttons-1.5.8/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/test_mixin.py` & `django_admin_extra_buttons-1.5.8/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/test_templatetags.py` & `django_admin_extra_buttons-1.5.8/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/test_upload.py` & `django_admin_extra_buttons-1.5.8/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/test_utils.py` & `django_admin_extra_buttons-1.5.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tests/test_views.py` & `django_admin_extra_buttons-1.5.8/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-admin-extra-buttons-1.5.7/tox.ini` & `django_admin_extra_buttons-1.5.8/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = d{32,42}-py{39,310,311}
+envlist = d{32,42,50}-py{311,312}
 
 [pytest]
 pythonpath=./tests/demoapp/
 django_find_project = false
 DJANGO_SETTINGS_MODULE=demo.settings
 norecursedirs = .tox docs ./tests/demoapp/
 python_files=tests/test_*.py
@@ -26,14 +26,15 @@
     PYTHONDONTWRITEBYTECODE=true
     DISPLAY=:0.0
 
 extras = test
 deps=
     d32: django==3.2.*
     d42: django==4.0.*
+    d50: django==5.0.*
     dev: git+git://github.com/django/django.git#egg=django
 
 commands =
     py.test tests --create-db {posargs}
 
 
 [testenv:package]
```

