# Comparing `tmp/aa_charlink-1.2.0.tar.gz` & `tmp/aa_charlink-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_charlink-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_charlink-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_charlink-1.2.0.tar` & `aa_charlink-1.2.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rwxr-xr-x   0        0        0    35149 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/LICENSE
--rwxr-xr-x   0        0        0     3945 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/README.md
--rwxr-xr-x   0        0        0      127 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/__init__.py
--rw-r--r--   0        0        0     2713 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/app_imports/__init__.py
--rw-r--r--   0        0        0     5216 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/app_imports/utils.py
--rwxr-xr-x   0        0        0      108 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/app_settings.py
--rwxr-xr-x   0        0        0      148 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/apps.py
--rwxr-xr-x   0        0        0      754 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/auth_hooks.py
--rwxr-xr-x   0        0        0      494 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/decorators.py
--rwxr-xr-x   0        0        0      652 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/forms.py
--rwxr-xr-x   0        0        0        0 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/__init__.py
--rw-r--r--   0        0        0     2882 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/afat.py
--rwxr-xr-x   0        0        0        0 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/allianceauth/__init__.py
--rwxr-xr-x   0        0        0     1777 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/allianceauth/corputils.py
--rw-r--r--   0        0        0     1788 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/corpstats.py
--rwxr-xr-x   0        0        0     4001 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/corptools.py
--rwxr-xr-x   0        0        0     2058 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/memberaudit.py
--rwxr-xr-x   0        0        0     1548 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/miningtaxes.py
--rwxr-xr-x   0        0        0     2600 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/moonmining.py
--rwxr-xr-x   0        0        0     1689 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/moonstuff.py
--rwxr-xr-x   0        0        0     3962 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/structures.py
--rw-r--r--   0        0        0      810 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/migrations/__init__.py
--rwxr-xr-x   0        0        0      435 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/models.py
--rw-r--r--   0        0        0       62 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/static/charlink/css/added-icons.css
--rw-r--r--   0        0        0     4306 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/app_audit.html
--rwxr-xr-x   0        0        0     4080 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/audit.html
--rw-r--r--   0        0        0      746 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/base.html
--rwxr-xr-x   0        0        0     6124 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/charlink.html
--rw-r--r--   0        0        0      532 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/dashboard_login.html
--rw-r--r--   0        0        0      903 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/menu-left.html
--rw-r--r--   0        0        0      431 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/menu-right.html
--rw-r--r--   0        0        0     2711 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/search.html
--rw-r--r--   0        0        0     3032 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/user_audit.html
--rw-r--r--   0        0        0        0 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templatetags/__init__.py
--rw-r--r--   0        0        0      516 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templatetags/charlink_versioned_static.py
--rw-r--r--   0        0        0      837 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templatetags/charlinkutils.py
--rw-r--r--   0        0        0        0 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/__init__.py
--rw-r--r--   0        0        0     3943 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_afat.py
--rw-r--r--   0        0        0     3060 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_allianceauth_corputils.py
--rw-r--r--   0        0        0     2980 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_corpstats.py
--rw-r--r--   0        0        0     3798 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_corptools.py
--rw-r--r--   0        0        0     3213 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_memberaudit.py
--rw-r--r--   0        0        0     2272 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_miningtaxes.py
--rw-r--r--   0        0        0     3710 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_moonmining.py
--rw-r--r--   0        0        0     2440 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_moonstuff.py
--rw-r--r--   0        0        0     5986 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_structures.py
--rw-r--r--   0        0        0     7861 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_app_imports.py
--rwxr-xr-x   0        0        0     1265 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1323 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_decorators.py
--rw-r--r--   0        0        0     1261 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_forms.py
--rw-r--r--   0        0        0     2241 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_templatetags.py
--rw-r--r--   0        0        0     5488 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_utils.py
--rw-r--r--   0        0        0    20489 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_views.py
--rwxr-xr-x   0        0        0      520 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/urls.py
--rw-r--r--   0        0        0     2703 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/utils.py
--rwxr-xr-x   0        0        0     8267 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/views.py
--rwxr-xr-x   0        0        0     1519 2024-04-15 20:22:47.872466 aa_charlink-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 aa_charlink-1.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/LICENSE
+-rwxr-xr-x   0        0        0     3945 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/README.md
+-rwxr-xr-x   0        0        0      127 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/charlink/__init__.py
+-rw-r--r--   0        0        0     3233 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/charlink/app_imports/__init__.py
+-rw-r--r--   0        0        0     5216 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/charlink/app_imports/utils.py
+-rwxr-xr-x   0        0        0      108 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/charlink/app_settings.py
+-rwxr-xr-x   0        0        0      148 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/charlink/apps.py
+-rwxr-xr-x   0        0        0      754 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/charlink/auth_hooks.py
+-rwxr-xr-x   0        0        0      494 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/charlink/decorators.py
+-rwxr-xr-x   0        0        0      652 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/charlink/forms.py
+-rwxr-xr-x   0        0        0        0 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/charlink/imports/__init__.py
+-rw-r--r--   0        0        0     2882 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/charlink/imports/afat.py
+-rwxr-xr-x   0        0        0        0 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/charlink/imports/allianceauth/__init__.py
+-rwxr-xr-x   0        0        0     1777 2024-05-04 09:14:36.454978 aa_charlink-1.2.1/charlink/imports/allianceauth/corputils.py
+-rw-r--r--   0        0        0     1788 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/imports/corpstats.py
+-rwxr-xr-x   0        0        0     4001 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/imports/corptools.py
+-rwxr-xr-x   0        0        0     2058 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/imports/memberaudit.py
+-rwxr-xr-x   0        0        0     1548 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/imports/miningtaxes.py
+-rwxr-xr-x   0        0        0     2600 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/imports/moonmining.py
+-rwxr-xr-x   0        0        0     1689 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/imports/moonstuff.py
+-rwxr-xr-x   0        0        0     3962 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/imports/structures.py
+-rw-r--r--   0        0        0      810 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/migrations/__init__.py
+-rwxr-xr-x   0        0        0      435 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/models.py
+-rw-r--r--   0        0        0       62 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/static/charlink/css/added-icons.css
+-rw-r--r--   0        0        0     4306 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/templates/charlink/app_audit.html
+-rwxr-xr-x   0        0        0     4080 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/templates/charlink/audit.html
+-rw-r--r--   0        0        0      746 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/templates/charlink/base.html
+-rwxr-xr-x   0        0        0     6124 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/templates/charlink/charlink.html
+-rw-r--r--   0        0        0      532 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/templates/charlink/dashboard_login.html
+-rw-r--r--   0        0        0      903 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/templates/charlink/menu-left.html
+-rw-r--r--   0        0        0      431 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/templates/charlink/menu-right.html
+-rw-r--r--   0        0        0     2711 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/templates/charlink/search.html
+-rw-r--r--   0        0        0     3032 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/templates/charlink/user_audit.html
+-rw-r--r--   0        0        0        0 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/templatetags/__init__.py
+-rw-r--r--   0        0        0      516 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/templatetags/charlink_versioned_static.py
+-rw-r--r--   0        0        0      837 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/templatetags/charlinkutils.py
+-rw-r--r--   0        0        0        0 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/imports/__init__.py
+-rw-r--r--   0        0        0     3943 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/imports/test_afat.py
+-rw-r--r--   0        0        0     3060 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/imports/test_allianceauth_corputils.py
+-rw-r--r--   0        0        0     2980 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/imports/test_corpstats.py
+-rw-r--r--   0        0        0     3798 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/imports/test_corptools.py
+-rw-r--r--   0        0        0     3213 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/imports/test_memberaudit.py
+-rw-r--r--   0        0        0     2272 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/imports/test_miningtaxes.py
+-rw-r--r--   0        0        0     3710 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/imports/test_moonmining.py
+-rw-r--r--   0        0        0     2440 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/imports/test_moonstuff.py
+-rw-r--r--   0        0        0     5986 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/imports/test_structures.py
+-rw-r--r--   0        0        0     8839 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/test_app_imports.py
+-rwxr-xr-x   0        0        0     1265 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1323 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/test_decorators.py
+-rw-r--r--   0        0        0     1261 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/test_forms.py
+-rw-r--r--   0        0        0     2241 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/test_templatetags.py
+-rw-r--r--   0        0        0     5488 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/test_utils.py
+-rw-r--r--   0        0        0    20489 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/tests/test_views.py
+-rwxr-xr-x   0        0        0      520 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/urls.py
+-rw-r--r--   0        0        0     2703 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/utils.py
+-rwxr-xr-x   0        0        0     8267 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/charlink/views.py
+-rwxr-xr-x   0        0        0     1519 2024-05-04 09:14:36.458978 aa_charlink-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 aa_charlink-1.2.1/PKG-INFO
```

### Comparing `aa_charlink-1.2.0/LICENSE` & `aa_charlink-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/README.md` & `aa_charlink-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/app_imports/__init__.py` & `aa_charlink-1.2.1/charlink/app_imports/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,14 +26,16 @@
             get_users_with_perms=lambda: User.objects.filter(
                 Exists(CharacterOwnership.objects.filter(user_id=OuterRef('pk')))
             ),
         )
     ])
 }
 
+_duplicated_apps = set()
+
 _imported = False
 
 
 def import_apps():
     global _imported
     if not _imported:
         # hooks
@@ -49,16 +51,23 @@
             except AssertionError:
                 logger.debug(f"Loading of {hook_mod} link via hook: failed to validate")
             except ModuleNotFoundError:
                 logger.debug(f"Loading of {hook_mod} link via hook: failed to import")
             except:
                 logger.debug(f"Loading of {hook_mod} link via hook: failed")
             else:
-                _supported_apps[app_import.app_label] = app_import
-                logger.debug(f"Loading of {hook_mod} link via hook: success")
+                if app_import.app_label in _supported_apps:
+                    _supported_apps.pop(app_import.app_label)
+                    _duplicated_apps.add(app_import.app_label)
+
+                if app_import.app_label in _duplicated_apps:
+                    logger.debug(f"Loading of {hook_mod} link via hook: failed, duplicate {app_import.app_label}")
+                else:
+                    _supported_apps[app_import.app_label] = app_import
+                    logger.debug(f"Loading of {hook_mod} link via hook: success")
 
         # defaults
         for app in settings.INSTALLED_APPS:
             if app != 'allianceauth' and app not in _supported_apps:
                 try:
                     module = import_module(f'charlink.imports.{app}')
                 except ModuleNotFoundError:
@@ -66,7 +75,14 @@
                 else:
                     _supported_apps[app] = module.app_import
                     logger.debug(f"Loading of {app} link: success")
 
         _imported = True
 
     return _supported_apps
+
+
+def get_duplicated_apps():
+    if not _imported:
+        import_apps()
+
+    return _duplicated_apps
```

### Comparing `aa_charlink-1.2.0/charlink/app_imports/utils.py` & `aa_charlink-1.2.1/charlink/app_imports/utils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/auth_hooks.py` & `aa_charlink-1.2.1/charlink/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/forms.py` & `aa_charlink-1.2.1/charlink/forms.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/imports/afat.py` & `aa_charlink-1.2.1/charlink/imports/afat.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/imports/allianceauth/corputils.py` & `aa_charlink-1.2.1/charlink/imports/allianceauth/corputils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/imports/corpstats.py` & `aa_charlink-1.2.1/charlink/imports/corpstats.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/imports/corptools.py` & `aa_charlink-1.2.1/charlink/imports/corptools.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/imports/memberaudit.py` & `aa_charlink-1.2.1/charlink/imports/memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/imports/miningtaxes.py` & `aa_charlink-1.2.1/charlink/imports/miningtaxes.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/imports/moonmining.py` & `aa_charlink-1.2.1/charlink/imports/moonmining.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/imports/moonstuff.py` & `aa_charlink-1.2.1/charlink/imports/moonstuff.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/imports/structures.py` & `aa_charlink-1.2.1/charlink/imports/structures.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/migrations/0001_initial.py` & `aa_charlink-1.2.1/charlink/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/templates/charlink/app_audit.html` & `aa_charlink-1.2.1/charlink/templates/charlink/app_audit.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/templates/charlink/audit.html` & `aa_charlink-1.2.1/charlink/templates/charlink/audit.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/templates/charlink/base.html` & `aa_charlink-1.2.1/charlink/templates/charlink/base.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/templates/charlink/charlink.html` & `aa_charlink-1.2.1/charlink/templates/charlink/charlink.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/templates/charlink/dashboard_login.html` & `aa_charlink-1.2.1/charlink/templates/charlink/dashboard_login.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/templates/charlink/menu-left.html` & `aa_charlink-1.2.1/charlink/templates/charlink/menu-left.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/templates/charlink/search.html` & `aa_charlink-1.2.1/charlink/templates/charlink/search.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/templates/charlink/user_audit.html` & `aa_charlink-1.2.1/charlink/templates/charlink/user_audit.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/templatetags/charlink_versioned_static.py` & `aa_charlink-1.2.1/charlink/templatetags/charlink_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/templatetags/charlinkutils.py` & `aa_charlink-1.2.1/charlink/templatetags/charlinkutils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/imports/test_afat.py` & `aa_charlink-1.2.1/charlink/tests/imports/test_afat.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/imports/test_allianceauth_corputils.py` & `aa_charlink-1.2.1/charlink/tests/imports/test_allianceauth_corputils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/imports/test_corpstats.py` & `aa_charlink-1.2.1/charlink/tests/imports/test_corpstats.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/imports/test_corptools.py` & `aa_charlink-1.2.1/charlink/tests/imports/test_corptools.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/imports/test_memberaudit.py` & `aa_charlink-1.2.1/charlink/tests/imports/test_memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/imports/test_miningtaxes.py` & `aa_charlink-1.2.1/charlink/tests/imports/test_miningtaxes.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/imports/test_moonmining.py` & `aa_charlink-1.2.1/charlink/tests/imports/test_moonmining.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/imports/test_moonstuff.py` & `aa_charlink-1.2.1/charlink/tests/imports/test_moonstuff.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/imports/test_structures.py` & `aa_charlink-1.2.1/charlink/tests/imports/test_structures.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/test_app_imports.py` & `aa_charlink-1.2.1/charlink/tests/test_app_imports.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from importlib import import_module
 from unittest.mock import patch
 
 from django.test import TestCase
 
 from app_utils.testdata_factories import UserMainFactory
 
-from charlink.app_imports import import_apps
+from charlink.app_imports import import_apps, get_duplicated_apps
 from charlink.imports.corptools import _corp_perms
 
+from ..app_imports import AppImport
+
 
 class TestImportApps(TestCase):
 
     @patch('charlink.app_imports.import_module', wraps=import_module)
     @patch('charlink.app_imports._imported', False)
+    @patch('charlink.app_imports._duplicated_apps', set())
+    @patch('charlink.app_imports._supported_apps', {
+        'allianceauth.authentication': AppImport('allianceauth.authentication', [])
+    })
     def test_not_imported(self, mock_import_module):
         imported_apps = import_apps()
         self.assertTrue(mock_import_module.called)
         self.assertIn('allianceauth.authentication', imported_apps)
         self.assertIn('allianceauth.corputils', imported_apps)
         self.assertIn('testauth.testapp', imported_apps)
         self.assertNotIn('fakeapp', imported_apps)
@@ -43,14 +49,29 @@
 
         add_char = import_apps()['allianceauth.authentication']
         self.assertIsNone(add_char.imports[0].add_character(None))
         self.assertTrue(add_char.imports[0].is_character_added(main_char))
         self.assertTrue(add_char.imports[0].check_permissions(user))
         self.assertEqual(add_char.imports[0].get_users_with_perms().count(), 1)
 
+    def test_ignore_duplicate_imports(self):
+        imported_apps = import_apps()
+        self.assertNotIn('testauth.testapp_duplicate', imported_apps)
+        self.assertSetEqual({'testauth.testapp_duplicate'}, get_duplicated_apps())
+
+    @patch('charlink.app_imports.import_module', wraps=import_module)
+    @patch('charlink.app_imports._imported', False)
+    @patch('charlink.app_imports._duplicated_apps', set())
+    @patch('charlink.app_imports._supported_apps', {
+        'allianceauth.authentication': AppImport('allianceauth.authentication', [])
+    })
+    def test_get_duplicated_apps_imports_apps(self, mock_import_module):
+        get_duplicated_apps()
+        self.assertTrue(mock_import_module.called)
+
 
 class TestLoginImport(TestCase):
 
     def test_get_query_id(self):
         login_import = import_apps()['allianceauth.authentication'].get('default')
         self.assertEqual(login_import.get_query_id(), 'allianceauth.authentication_default')
```

### Comparing `aa_charlink-1.2.0/charlink/tests/test_auth_hooks.py` & `aa_charlink-1.2.1/charlink/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/test_decorators.py` & `aa_charlink-1.2.1/charlink/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/test_forms.py` & `aa_charlink-1.2.1/charlink/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/test_templatetags.py` & `aa_charlink-1.2.1/charlink/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/test_utils.py` & `aa_charlink-1.2.1/charlink/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/tests/test_views.py` & `aa_charlink-1.2.1/charlink/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/urls.py` & `aa_charlink-1.2.1/charlink/urls.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/utils.py` & `aa_charlink-1.2.1/charlink/utils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/charlink/views.py` & `aa_charlink-1.2.1/charlink/views.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/pyproject.toml` & `aa_charlink-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.2.0/PKG-INFO` & `aa_charlink-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-charlink
-Version: 1.2.0
+Version: 1.2.1
 Summary: Character Linker for Alliance Auth
 Keywords: allianceauth,eveonline,allianceauth_charlink,charlink
 Author-email: Matteo Ghia <matteo.ghia@yahoo.it>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

