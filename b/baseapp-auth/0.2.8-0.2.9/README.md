# Comparing `tmp/baseapp-auth-0.2.8.tar.gz` & `tmp/baseapp-auth-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseapp-auth-0.2.8.tar", last modified: Tue Mar 12 00:08:03 2024, max compression
+gzip compressed data, was "baseapp-auth-0.2.9.tar", last modified: Wed Mar 13 12:15:26 2024, max compression
```

## Comparing `baseapp-auth-0.2.8.tar` & `baseapp-auth-0.2.9.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.248858 baseapp-auth-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-03-12 00:08:03.248858 baseapp-auth-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.232859 baseapp-auth-0.2.8/baseapp_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.232859 baseapp-auth-0.2.8/baseapp_auth/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/graphql/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/graphql/object_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/graphql/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/graphql/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.232859 baseapp-auth-0.2.8/baseapp_auth/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/migrations/0002_passwordvalidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/migrations/0003_superuserupdatelog.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/password_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/querysets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.232859 baseapp-auth-0.2.8/baseapp_auth/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.232859 baseapp-auth-0.2.8/baseapp_auth/rest_framework/change_email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/change_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/change_email/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/change_email/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.232859 baseapp-auth-0.2.8/baseapp_auth/rest_framework/forgot_password/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/forgot_password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/forgot_password/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/forgot_password/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.236858 baseapp-auth-0.2.8/baseapp_auth/rest_framework/jwt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/jwt/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/jwt/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/jwt/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.236858 baseapp-auth-0.2.8/baseapp_auth/rest_framework/login/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/login/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/login/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.236858 baseapp-auth-0.2.8/baseapp_auth/rest_framework/mfa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/mfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/mfa/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.236858 baseapp-auth-0.2.8/baseapp_auth/rest_framework/pre_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/pre_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/pre_auth/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/pre_auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.236858 baseapp-auth-0.2.8/baseapp_auth/rest_framework/register/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/register/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/register/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.236858 baseapp-auth-0.2.8/baseapp_auth/rest_framework/routers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/routers/account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.236858 baseapp-auth-0.2.8/baseapp_auth/rest_framework/urls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/urls/auth_authtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/urls/auth_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/urls/auth_mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/urls/auth_mfa_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/urls/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/urls/pre_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.240858 baseapp-auth-0.2.8/baseapp_auth/rest_framework/users/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/users/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/users/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/users/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/users/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/users/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/rest_framework/users/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.228859 baseapp-auth-0.2.8/baseapp_auth/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.228859 baseapp-auth-0.2.8/baseapp_auth/templates/users/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.240858 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/change-email-confirm-body.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/change-email-confirm-body.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/change-email-confirm-subject.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/change-email-verify-body.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/change-email-verify-body.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/change-email-verify-subject.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/new-superuser-notification-email.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/new-superuser-notification-email.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/password-expired-body.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/password-expired-body.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/password-expired-subject.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/password-reset-body.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/password-reset-body.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/password-reset-subject.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/remove-superuser-notification-email.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/remove-superuser-notification-email.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/welcome-body.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/welcome-body.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/welcome-subject.txt.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.244858 baseapp-auth-0.2.8/baseapp_auth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/fixtures_mfa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.244858 baseapp-auth-0.2.8/baseapp_auth/tests/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/graphql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/graphql/test_queries_me.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/graphql/test_queries_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.244858 baseapp-auth-0.2.8/baseapp_auth/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_change_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_forgot_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_migration_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_pre_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_users_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.244858 baseapp-auth-0.2.8/baseapp_auth/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/unit/test_celery_beat_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tests/unit/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.244858 baseapp-auth-0.2.8/baseapp_auth/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_auth/utils/referral_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.232859 baseapp-auth-0.2.8/baseapp_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-03-12 00:08:03.000000 baseapp-auth-0.2.8/baseapp_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-03-12 00:08:03.000000 baseapp-auth-0.2.8/baseapp_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 00:08:03.000000 baseapp-auth-0.2.8/baseapp_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-12 00:08:03.000000 baseapp-auth-0.2.8/baseapp_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-12 00:08:03.000000 baseapp-auth-0.2.8/baseapp_auth.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.248858 baseapp-auth-0.2.8/baseapp_referrals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_referrals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_referrals/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_referrals/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.248858 baseapp-auth-0.2.8/baseapp_referrals/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_referrals/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_referrals/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_referrals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_referrals/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.248858 baseapp-auth-0.2.8/baseapp_referrals/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_referrals/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_referrals/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.248858 baseapp-auth-0.2.8/baseapp_referrals/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_referrals/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_referrals/tests/unit/test_referrals_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/baseapp_referrals/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-12 00:08:03.248858 baseapp-auth-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:03.248858 baseapp-auth-0.2.8/testproject/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/testproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/testproject/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/testproject/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/testproject/settings_referrals.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/testproject/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/testproject/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-12 00:08:02.000000 baseapp-auth-0.2.8/testproject/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.020151 baseapp-auth-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-03-13 12:15:26.020151 baseapp-auth-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.004151 baseapp-auth-0.2.9/baseapp_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.004151 baseapp-auth-0.2.9/baseapp_auth/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/graphql/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/graphql/object_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/graphql/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/graphql/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.004151 baseapp-auth-0.2.9/baseapp_auth/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/migrations/0002_passwordvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/migrations/0003_superuserupdatelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/password_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/querysets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.004151 baseapp-auth-0.2.9/baseapp_auth/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.008151 baseapp-auth-0.2.9/baseapp_auth/rest_framework/change_email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/change_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/change_email/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/change_email/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.008151 baseapp-auth-0.2.9/baseapp_auth/rest_framework/forgot_password/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/forgot_password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/forgot_password/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/forgot_password/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.008151 baseapp-auth-0.2.9/baseapp_auth/rest_framework/jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/jwt/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/jwt/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/jwt/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.008151 baseapp-auth-0.2.9/baseapp_auth/rest_framework/login/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/login/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/login/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.008151 baseapp-auth-0.2.9/baseapp_auth/rest_framework/mfa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/mfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/mfa/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.008151 baseapp-auth-0.2.9/baseapp_auth/rest_framework/pre_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/pre_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/pre_auth/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/pre_auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.008151 baseapp-auth-0.2.9/baseapp_auth/rest_framework/register/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/register/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/register/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.008151 baseapp-auth-0.2.9/baseapp_auth/rest_framework/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/routers/account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.012151 baseapp-auth-0.2.9/baseapp_auth/rest_framework/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/urls/auth_authtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/urls/auth_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/urls/auth_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/urls/auth_mfa_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/urls/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/urls/pre_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.012151 baseapp-auth-0.2.9/baseapp_auth/rest_framework/users/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/users/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/users/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/users/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/users/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/users/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/rest_framework/users/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.000151 baseapp-auth-0.2.9/baseapp_auth/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.000151 baseapp-auth-0.2.9/baseapp_auth/templates/users/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.016151 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/change-email-confirm-body.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/change-email-confirm-body.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/change-email-confirm-subject.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/change-email-verify-body.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/change-email-verify-body.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/change-email-verify-subject.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/new-superuser-notification-email.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/new-superuser-notification-email.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/password-expired-body.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/password-expired-body.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/password-expired-subject.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/password-reset-body.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/password-reset-body.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/password-reset-subject.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/remove-superuser-notification-email.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/remove-superuser-notification-email.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/welcome-body.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/welcome-body.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/welcome-subject.txt.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.016151 baseapp-auth-0.2.9/baseapp_auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/fixtures_mfa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.016151 baseapp-auth-0.2.9/baseapp_auth/tests/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/graphql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/graphql/test_queries_me.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/graphql/test_queries_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.016151 baseapp-auth-0.2.9/baseapp_auth/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_change_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_forgot_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_migration_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_pre_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_users_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.016151 baseapp-auth-0.2.9/baseapp_auth/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/unit/test_celery_beat_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tests/unit/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.016151 baseapp-auth-0.2.9/baseapp_auth/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_auth/utils/referral_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.004151 baseapp-auth-0.2.9/baseapp_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-03-13 12:15:25.000000 baseapp-auth-0.2.9/baseapp_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-03-13 12:15:25.000000 baseapp-auth-0.2.9/baseapp_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 12:15:25.000000 baseapp-auth-0.2.9/baseapp_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-13 12:15:25.000000 baseapp-auth-0.2.9/baseapp_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-13 12:15:25.000000 baseapp-auth-0.2.9/baseapp_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.020151 baseapp-auth-0.2.9/baseapp_referrals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_referrals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_referrals/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_referrals/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.020151 baseapp-auth-0.2.9/baseapp_referrals/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_referrals/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_referrals/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_referrals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_referrals/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.020151 baseapp-auth-0.2.9/baseapp_referrals/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_referrals/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_referrals/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.020151 baseapp-auth-0.2.9/baseapp_referrals/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_referrals/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_referrals/tests/unit/test_referrals_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/baseapp_referrals/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-13 12:15:26.020151 baseapp-auth-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:26.020151 baseapp-auth-0.2.9/testproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/testproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/testproject/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/testproject/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/testproject/settings_referrals.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/testproject/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/testproject/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-13 12:15:24.000000 baseapp-auth-0.2.9/testproject/wsgi.py
```

### Comparing `baseapp-auth-0.2.8/PKG-INFO` & `baseapp-auth-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp-auth
-Version: 0.2.8
+Version: 0.2.9
 Summary: BaseApp Auth
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause  # Example license
 Description: # BaseApp Auth
```

### Comparing `baseapp-auth-0.2.8/README.md` & `baseapp-auth-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/admin.py` & `baseapp-auth-0.2.9/baseapp_auth/admin.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/apps.py` & `baseapp-auth-0.2.9/baseapp_auth/apps.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/emails.py` & `baseapp-auth-0.2.9/baseapp_auth/emails.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/forms.py` & `baseapp-auth-0.2.9/baseapp_auth/forms.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/graphql/filters.py` & `baseapp-auth-0.2.9/baseapp_auth/graphql/filters.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/graphql/object_types.py` & `baseapp-auth-0.2.9/baseapp_auth/graphql/object_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import graphene
-from baseapp_core.graphql import DjangoObjectType
+from avatar.templatetags.avatar_tags import avatar_url
+from baseapp_core.graphql import DjangoObjectType, File
 from django.apps import apps
 from django.contrib.auth import get_user_model
 from graphene import relay
 
 from .filters import UsersFilter
 from .permissions import PermissionsInterface
 
@@ -24,14 +25,16 @@
 
 
 class AbstractUserObjectType(object):
     is_authenticated = graphene.Boolean()
     full_name = graphene.String()
     short_name = graphene.String()
 
+    avatar = graphene.Field(File, width=graphene.Int(), height=graphene.Int())
+
     # Make them not required
     email = graphene.String()
     phone_number = graphene.String()
     is_superuser = graphene.Boolean()
     is_staff = graphene.Boolean()
     is_email_verified = graphene.Boolean()
     password_changed_date = graphene.DateTime()
@@ -61,14 +64,17 @@
             "comments",
             "reactions",
             "last_login",
         )
         interfaces = interfaces
         filterset_class = UsersFilter
 
+    def resolve_avatar(self, info, width, height):
+        return File(url=avatar_url(self, width, height))
+
     def resolve_metadata(self, info):
         return MetadataObjectType(
             meta_title=self.get_full_name(),
         )
 
     def resolve_is_authenticated(self, info):
         return info.context.user.is_authenticated and self.pk == info.context.user.pk
```

### Comparing `baseapp-auth-0.2.8/baseapp_auth/graphql/permissions.py` & `baseapp-auth-0.2.9/baseapp_auth/graphql/permissions.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/graphql/queries.py` & `baseapp-auth-0.2.9/baseapp_auth/graphql/queries.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/managers.py` & `baseapp-auth-0.2.9/baseapp_auth/managers.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/middleware.py` & `baseapp-auth-0.2.9/baseapp_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/migrations/0002_passwordvalidation.py` & `baseapp-auth-0.2.9/baseapp_auth/migrations/0002_passwordvalidation.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/migrations/0003_superuserupdatelog.py` & `baseapp-auth-0.2.9/baseapp_auth/migrations/0003_superuserupdatelog.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/models.py` & `baseapp-auth-0.2.9/baseapp_auth/models.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/password_validators.py` & `baseapp-auth-0.2.9/baseapp_auth/password_validators.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/permissions.py` & `baseapp-auth-0.2.9/baseapp_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/pipeline.py` & `baseapp-auth-0.2.9/baseapp_auth/pipeline.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/querysets.py` & `baseapp-auth-0.2.9/baseapp_auth/querysets.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/change_email/serializers.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/change_email/serializers.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/change_email/views.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/change_email/views.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/forgot_password/serializers.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/forgot_password/serializers.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/forgot_password/views.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/forgot_password/views.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/jwt/serializers.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/jwt/serializers.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/jwt/tokens.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/jwt/tokens.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/jwt/views.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/jwt/views.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/login/serializers.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/login/serializers.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/login/views.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/login/views.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/mfa/mixins.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/mfa/mixins.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/pre_auth/serializers.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/pre_auth/serializers.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/pre_auth/views.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/pre_auth/views.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/register/serializers.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/register/serializers.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/register/views.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/register/views.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/routers/account.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/routers/account.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/urls/auth_mfa.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/urls/auth_mfa.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/urls/mfa.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/urls/mfa.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/users/channels.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/users/channels.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/users/serializers.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/users/serializers.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/rest_framework/users/views.py` & `baseapp-auth-0.2.9/baseapp_auth/rest_framework/users/views.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/change-email-confirm-body.html.j2` & `baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/change-email-confirm-body.html.j2`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/change-email-verify-body.html.j2` & `baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/change-email-verify-body.html.j2`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/new-superuser-notification-email.html.j2` & `baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/new-superuser-notification-email.html.j2`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/password-expired-body.html.j2` & `baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/password-expired-body.html.j2`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/password-reset-body.html.j2` & `baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/password-reset-body.html.j2`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/remove-superuser-notification-email.html.j2` & `baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/remove-superuser-notification-email.html.j2`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/templates/users/emails/welcome-body.html.j2` & `baseapp-auth-0.2.9/baseapp_auth/templates/users/emails/welcome-body.html.j2`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/fixtures_mfa.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/fixtures_mfa.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/graphql/test_queries_me.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/graphql/test_queries_me.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/graphql/test_queries_user.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/graphql/test_queries_user.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/helpers.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_change_email.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_change_email.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_forgot_password.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_forgot_password.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_login.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_login.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_migration_health_check.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_migration_health_check.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_pagination.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_pagination.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_pre_auth.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_pre_auth.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_register.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_register.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_users.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_users.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/integration/test_users_channels.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/integration/test_users_channels.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/unit/test_celery_beat_health_check.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/unit/test_celery_beat_health_check.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tests/unit/test_users.py` & `baseapp-auth-0.2.9/baseapp_auth/tests/unit/test_users.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth/tokens.py` & `baseapp-auth-0.2.9/baseapp_auth/tokens.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_auth.egg-info/PKG-INFO` & `baseapp-auth-0.2.9/baseapp_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp-auth
-Version: 0.2.8
+Version: 0.2.9
 Summary: BaseApp Auth
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause  # Example license
 Description: # BaseApp Auth
```

### Comparing `baseapp-auth-0.2.8/baseapp_auth.egg-info/SOURCES.txt` & `baseapp-auth-0.2.9/baseapp_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_referrals/migrations/0001_initial.py` & `baseapp-auth-0.2.9/baseapp_referrals/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_referrals/models.py` & `baseapp-auth-0.2.9/baseapp_referrals/models.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_referrals/tests/unit/test_referrals_utils.py` & `baseapp-auth-0.2.9/baseapp_referrals/tests/unit/test_referrals_utils.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/baseapp_referrals/utils.py` & `baseapp-auth-0.2.9/baseapp_referrals/utils.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/setup.cfg` & `baseapp-auth-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = baseapp_auth
-version = 0.2.8
+version = 0.2.9
 description = BaseApp Auth
 long_description = file: README.md
 url = https://github.com/silverlogic/baseapp-backend
 author = The SilverLogic
 author_email = dev@tsl.io
 license = BSD-3-Clause  # Example license
```

### Comparing `baseapp-auth-0.2.8/testproject/settings.py` & `baseapp-auth-0.2.9/testproject/settings.py`

 * *Files identical despite different names*

### Comparing `baseapp-auth-0.2.8/testproject/urls.py` & `baseapp-auth-0.2.9/testproject/urls.py`

 * *Files identical despite different names*

