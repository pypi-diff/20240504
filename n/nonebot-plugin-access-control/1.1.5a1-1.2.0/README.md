# Comparing `tmp/nonebot_plugin_access_control-1.1.5a1.tar.gz` & `tmp/nonebot_plugin_access_control-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_access_control-1.1.5a1.tar", max compression
+gzip compressed data, was "nonebot_plugin_access_control-1.2.0.tar", max compression
```

## Comparing `nonebot_plugin_access_control-1.1.5a1.tar` & `nonebot_plugin_access_control-1.2.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-1.1.5a1/LICENSE
--rw-r--r--   0        0        0     2291 2023-11-26 15:11:05.494035 nonebot_plugin_access_control-1.1.5a1/pyproject.toml
--rw-r--r--   0        0        0    15268 2023-11-23 15:59:00.851323 nonebot_plugin_access_control-1.1.5a1/README.MD
--rw-r--r--   0        0        0     1056 2023-11-24 04:52:35.739565 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/__init__.py
--rw-r--r--   0        0        0     4123 2023-11-04 10:37:53.894431 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/alc.py
--rw-r--r--   0        0        0      967 2023-11-04 10:37:53.898431 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/config.py
--rw-r--r--   0        0        0      734 2023-11-04 10:37:53.921431 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/datastore/__init__.py
--rw-r--r--   0        0        0     2171 2023-11-04 10:38:04.974811 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/datastore/migrations/6fbda6d1d8ee_.py
--rw-r--r--   0        0        0     3727 2023-11-04 10:38:05.013808 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/datastore/migrations/875c4dd8c271_.py
--rw-r--r--   0        0        0     4673 2023-11-24 04:52:35.740565 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/handler/__init__.py
--rw-r--r--   0        0        0      248 2023-11-04 10:37:53.936450 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/handler/help_handler.py
--rw-r--r--   0        0        0     4035 2023-11-24 04:52:35.740565 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/handler/limit_handler.py
--rw-r--r--   0        0        0     3158 2023-11-24 04:52:35.741565 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/handler/permission_handler.py
--rw-r--r--   0        0        0      511 2023-11-23 15:59:00.858055 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/handler/service_handler.py
--rw-r--r--   0        0        0      591 2023-11-24 04:52:35.741565 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/handler/subject_handler.py
--rw-r--r--   0        0        0        0 2023-11-03 14:53:21.082579 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/handler/utils/__init__.py
--rw-r--r--   0        0        0      282 2023-11-24 04:52:35.742565 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/handler/utils/env.py
--rw-r--r--   0        0        0      569 2023-11-24 04:52:35.743565 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/handler/utils/permission.py
--rw-r--r--   0        0        0     1014 2023-11-03 14:53:21.083579 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/matcher.py
--rw-r--r--   0        0        0     5798 2023-11-26 15:11:05.499036 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/orm_migrations/96ced46e72e9_data_migrate.py
--rw-r--r--   0        0        0     3420 2023-11-24 04:38:49.395556 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/orm_migrations/9bb3231cf9aa_init_db.py
--rw-r--r--   0        0        0        0 2023-11-23 15:59:00.860056 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/__init__.py
--rw-r--r--   0        0        0        0 2023-11-23 15:59:00.860056 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/orm/__init__.py
--rw-r--r--   0        0        0      396 2023-11-23 15:59:00.860056 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/orm/permission.py
--rw-r--r--   0        0        0     1690 2023-11-23 15:59:00.861061 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/orm/rate_limit.py
--rw-r--r--   0        0        0      114 2023-11-23 15:59:00.861061 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/permission/__init__.py
--rw-r--r--   0        0        0     2924 2023-11-24 04:52:35.743565 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/permission/impl.py
--rw-r--r--   0        0        0      797 2023-11-23 15:59:00.862060 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/permission/interface.py
--rw-r--r--   0        0        0      112 2023-11-23 15:59:00.862060 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/rate_limit/__init__.py
--rw-r--r--   0        0        0     3784 2023-11-24 04:52:35.744565 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/rate_limit/impl.py
--rw-r--r--   0        0        0      972 2023-11-23 15:59:00.863059 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/rate_limit/interface.py
--rw-r--r--   0        0        0      693 2023-11-23 15:59:00.863059 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/rate_limit_token/__init__.py
--rw-r--r--   0        0        0     4516 2023-11-24 04:52:35.745568 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/rate_limit_token/datastore.py
--rw-r--r--   0        0        0     3037 2023-11-24 04:52:35.745568 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/rate_limit_token/inmemory.py
--rw-r--r--   0        0        0      607 2023-11-23 15:59:00.864059 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/rate_limit_token/interface.py
--rw-r--r--   0        0        0      802 2023-11-24 04:52:35.746923 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/utils.py
--rw-r--r--   0        0        0     1071 2023-11-04 10:37:54.008454 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/script/__init__.py
--rw-r--r--   0        0        0       29 2023-11-23 15:59:00.865059 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/service/__init__.py
--rw-r--r--   0        0        0       31 2023-11-23 15:59:00.866059 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/service/_impl/__init__.py
--rw-r--r--   0        0        0     1482 2023-11-24 04:52:35.747431 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/service/_impl/factory.py
--rw-r--r--   0        0        0     5151 2023-11-26 12:45:40.038082 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/service/_impl/patcher.py
--rw-r--r--   0        0        0     6420 2023-11-24 04:52:35.748439 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/service/_impl/permission.py
--rw-r--r--   0        0        0     8442 2023-11-24 04:52:35.748439 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/service/_impl/rate_limit.py
--rw-r--r--   0        0        0       33 2023-11-23 15:59:00.868059 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/subject/__init__.py
--rw-r--r--   0        0        0      884 2023-11-24 04:52:35.749439 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/subject/extractor/__init__.py
--rw-r--r--   0        0        0        0 2023-11-23 15:59:00.868059 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/subject/extractor/builtin/__init__.py
--rw-r--r--   0        0        0     1193 2023-11-24 04:52:35.750439 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/subject/extractor/builtin/kaiheila.py
--rw-r--r--   0        0        0     1432 2023-11-24 04:52:35.750439 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/subject/extractor/builtin/onebot_v11.py
--rw-r--r--   0        0        0     3193 2023-11-24 04:52:35.751439 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/subject/extractor/builtin/qqguild.py
--rw-r--r--   0        0        0     4094 2023-11-24 04:52:35.752439 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/subject/extractor/builtin/session.py
--rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/utils/__init__.py
--rw-r--r--   0        0        0     1007 2023-11-04 10:37:54.168450 nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/utils/tree.py
--rw-r--r--   0        0        0    16153 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-1.1.5a1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-04 09:00:54.647271 nonebot_plugin_access_control-1.2.0/LICENSE
+-rw-r--r--   0        0        0    14909 2024-05-04 09:00:54.647271 nonebot_plugin_access_control-1.2.0/README.MD
+-rw-r--r--   0        0        0     2184 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1022 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/__init__.py
+-rw-r--r--   0        0        0     4014 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/alc.py
+-rw-r--r--   0        0        0      972 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/config.py
+-rw-r--r--   0        0        0      704 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/datastore/__init__.py
+-rw-r--r--   0        0        0     2103 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/datastore/migrations/6fbda6d1d8ee_.py
+-rw-r--r--   0        0        0     3629 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/datastore/migrations/875c4dd8c271_.py
+-rw-r--r--   0        0        0     4491 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/__init__.py
+-rw-r--r--   0        0        0      238 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/help_handler.py
+-rw-r--r--   0        0        0     3938 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/limit_handler.py
+-rw-r--r--   0        0        0     3111 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/permission_handler.py
+-rw-r--r--   0        0        0      496 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/service_handler.py
+-rw-r--r--   0        0        0      572 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/subject_handler.py
+-rw-r--r--   0        0        0        0 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/utils/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/utils/env.py
+-rw-r--r--   0        0        0     3066 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/utils/errors.py
+-rw-r--r--   0        0        0      550 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/utils/permission.py
+-rw-r--r--   0        0        0      973 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/matcher.py
+-rw-r--r--   0        0        0     5640 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/orm_migrations/96ced46e72e9_data_migrate.py
+-rw-r--r--   0        0        0     3331 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/orm_migrations/9bb3231cf9aa_init_db.py
+-rw-r--r--   0        0        0        0 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/orm/__init__.py
+-rw-r--r--   0        0        0      385 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/orm/permission.py
+-rw-r--r--   0        0        0     1640 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/orm/rate_limit.py
+-rw-r--r--   0        0        0      110 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/permission/__init__.py
+-rw-r--r--   0        0        0     2847 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/permission/impl.py
+-rw-r--r--   0        0        0      774 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/permission/interface.py
+-rw-r--r--   0        0        0      108 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/rate_limit/__init__.py
+-rw-r--r--   0        0        0     3726 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/rate_limit/impl.py
+-rw-r--r--   0        0        0      943 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/rate_limit/interface.py
+-rw-r--r--   0        0        0      673 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/rate_limit_token/__init__.py
+-rw-r--r--   0        0        0     4385 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/rate_limit_token/datastore.py
+-rw-r--r--   0        0        0     2938 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/rate_limit_token/inmemory.py
+-rw-r--r--   0        0        0      551 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/rate_limit_token/interface.py
+-rw-r--r--   0        0        0      777 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/utils.py
+-rw-r--r--   0        0        0     1028 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/script/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/service/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/service/_impl/__init__.py
+-rw-r--r--   0        0        0     1445 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/service/_impl/factory.py
+-rw-r--r--   0        0        0     5012 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/service/_impl/patcher.py
+-rw-r--r--   0        0        0     6244 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/service/_impl/permission.py
+-rw-r--r--   0        0        0     8212 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/service/_impl/rate_limit.py
+-rw-r--r--   0        0        0       32 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/subject/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/subject/extractor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/subject/extractor/builtin/__init__.py
+-rw-r--r--   0        0        0     1157 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/subject/extractor/builtin/kaiheila.py
+-rw-r--r--   0        0        0     1391 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/subject/extractor/builtin/onebot_v11.py
+-rw-r--r--   0        0        0     3112 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/subject/extractor/builtin/qqguild.py
+-rw-r--r--   0        0        0     3978 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/subject/extractor/builtin/session.py
+-rw-r--r--   0        0        0        0 2024-05-04 09:00:54.651271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/utils/__init__.py
+-rw-r--r--   0        0        0      974 2024-05-04 09:00:54.655271 nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/utils/tree.py
+-rw-r--r--   0        0        0    16204 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-1.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/pyproject.toml` & `nonebot_plugin_access_control-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-[tool.poetry]
-name = "nonebot-plugin-access-control"
-version = "1.1.5a1"
-description = ""
-authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
-license = "MIT"
-readme = "README.MD"
-repository = "https://github.com/bot-ssttkkl/nonebot-plugin-access-control"
-packages = [
-    { include = "nonebot_plugin_access_control", from = "src" }
-]
-
-[tool.poetry.dependencies]
-python = "^3.9"
-nonebot2 = "^2.1.0"
-nonebot-plugin-access-control-api = "^1.1.2"
-nonebot-plugin-apscheduler = ">=0.3.0"
-nonebot-plugin-session = "^0.2.0"
-nonebot-plugin-orm = ">=0.5.0, <1.0.0"
-arclet-alconna = "^1.7.24"
-shortuuid = "^1.0.11"
-pytimeparser = "^0.2.0"
-ssttkkl-nonebot-utils = ">=0.1.17"
-
-nb-cli = { version = ">=1.2.0", optional = true }
-
-nonebot-plugin-datastore = { version = ">=1.0.0", optional = true }
-
-[tool.poetry.group.dev.dependencies]
-ruff = "^0.0.275"
-isort = "^5.10.1"
-black = "^23.1.0"
-pre-commit = "^3.1.0"
-
-setuptools = "^68.1.2"
-nb-cli = "^1.2.5"
-nonebot-plugin-orm = {extras = ["default"], version = "^0.5.0"}
-
-nonebot2 = {extras = ["fastapi"], version = "^2.1.2"}
-nonebot-adapter-onebot = "*"
-nonebot-adapter-kaiheila = "*"
-nonebot-adapter-qqguild = "*"
-nonebot-adapter-telegram = "*"
-nonebot-adapter-console = "*"
-nonebot-adapter-feishu = "*"
-
-nonebug = "^0.3.5"
-pytest = "^7.4.3"
-pytest-asyncio = "^0.21.1"
-pytest-cov = "^4.1.0"
-
-
-[tool.black]
-line-length = 88
-target-version = ["py39", "py310", "py311", "py312"]
-include = '\.pyi?$'
-extend-exclude = '''
-'''
-
-[tool.isort]
-profile = "black"
-line_length = 88
-length_sort = true
-skip_gitignore = true
-force_sort_within_sections = true
-extra_standard_library = ["typing_extensions"]
-
-[tool.ruff]
-select = ["E", "W", "F", "UP", "C", "T", "PYI", "PT", "Q"]
-ignore = ["C901", "E402", "F403", "T201"]
-
-line-length = 160
-target-version = "py39"
-
-[tool.ruff.flake8-pytest-style]
-fixture-parentheses = false
-mark-parentheses = false
-
-[tool.poetry.extras]
-cli = ["nb-cli"]
-migrate = ["nonebot-plugin-datastore"]
-
-[tool.poetry.plugins.nb_scripts]
-accctrl = "nonebot_plugin_access_control.script:install"
-
-[tool.nonebot]
-plugins = ["nonebot_plugin_access_control"]
-plugin_dirs = []
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "nonebot-plugin-access-control"
+version = "1.2.0"
+description = ""
+authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
+license = "MIT"
+readme = "README.MD"
+repository = "https://github.com/bot-ssttkkl/nonebot-plugin-access-control"
+packages = [
+    { include = "nonebot_plugin_access_control", from = "src" }
+]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+nonebot2 = ">=2.2.0, <3.0.0"
+nonebot-plugin-access-control-api = "^1.2.0"
+nonebot-plugin-apscheduler = ">=0.3.0"
+nonebot-plugin-session = "^0.3.0"
+nonebot-plugin-orm = ">=0.7.0, <1.0.0"
+arclet-alconna = "^1.7.24"
+shortuuid = "^1.0.11"
+pytimeparser = "^0.2.0"
+pydantic-settings = "^2.2.1"
+
+nb-cli = { version = ">=1.2.0", optional = true }
+
+nonebot-plugin-datastore = { version = ">=1.0.0", optional = true }
+
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.0.275"
+isort = "^5.10.1"
+black = "^23.1.0"
+pre-commit = "^3.1.0"
+
+setuptools = "^68.1.2"
+nb-cli = "*"
+nonebot-plugin-orm = { extras = ["default"], version = "*" }
+
+nonebot2 = { extras = ["fastapi"], version = "*" }
+nonebot-adapter-onebot = "*"
+nonebot-adapter-kaiheila = "*"
+nonebot-adapter-qq = "*"
+nonebot-adapter-telegram = "*"
+nonebot-adapter-console = "*"
+nonebot-adapter-feishu = "*"
+
+nonebug = "^0.3.5"
+pytest = "^7.4.3"
+pytest-asyncio = "^0.21.1"
+pytest-cov = "^4.1.0"
+
+
+[tool.black]
+line-length = 88
+target-version = ["py39", "py310", "py311", "py312"]
+include = '\.pyi?$'
+extend-exclude = '''
+'''
+
+[tool.isort]
+profile = "black"
+line_length = 88
+length_sort = true
+skip_gitignore = true
+force_sort_within_sections = true
+extra_standard_library = ["typing_extensions"]
+
+[tool.ruff]
+select = ["E", "W", "F", "UP", "C", "T", "PYI", "PT", "Q"]
+ignore = ["C901", "E402", "F403", "T201"]
+
+line-length = 160
+target-version = "py39"
+
+[tool.ruff.flake8-pytest-style]
+fixture-parentheses = false
+mark-parentheses = false
+
+[tool.poetry.extras]
+cli = ["nb-cli"]
+migrate = ["nonebot-plugin-datastore"]
+
+[tool.poetry.plugins.nb_scripts]
+accctrl = "nonebot_plugin_access_control.script:install"
+
+[tool.nonebot]
+plugins = ["nonebot_plugin_access_control"]
+plugin_dirs = []
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/README.MD` & `nonebot_plugin_access_control-1.2.0/README.MD`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,359 +1,359 @@
-<!-- markdownlint-disable MD033 MD036 MD041 -->
-
-<p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
-</p>
-
-<div align="center">
-
-nonebot-plugin-access-control
-============
-
-_✨ Nonebot 权限控制插件 ✨_
-
-</div>
-
-
-<p align="center">
-  <a href="https://raw.githubusercontent.com/ssttkkl/nonebot-plugin-access-control/master/LICENSE">
-    <img src="https://img.shields.io/github/license/ssttkkl/nonebot-plugin-access-control.svg" alt="license">
-  </a>
-  <a href="https://pypi.python.org/pypi/nonebot-plugin-access-control">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-access-control.svg" alt="pypi">
-  </a>
-  <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
-</p>
-
-## 特点
-
-- 功能
-    - [x] 支持针对用户/群组的权限开关
-    - [x] 支持限制同一用户在一定时间内的指令调用次数
-    - [x] 对未适配插件提供**插件级别**的控制支持
-- 插件适配
-    - [x] 支持**功能级别**的细粒度控制
-    - [x] 支持对权限开关等事件进行订阅
-- 拓展
-    - [x] 支持开发者拓展定义新的主体
-- CLI插件
-    - [x] 支持通过控制台中执行`nb accctrl`进入权限控制台
-
-## 使用
-
-### 主体
-
-#### 概念
-
-当我们对用户进行权限控制时，我们想要的是针对拥有某种同样身份的所有用户进行配置，而不是对每一个具体用户分别配置。因此，我们引入主体的概念。
-**主体（Subject）代表了拥有某种同样身份的用户的集合，也是设置权限的基本单位。**
-当我们说用户具有某个主体，也就是说用户在该主体所代表的集合内。换句话说，主体就是一个用户所具有的身份。
-
-一个用户通常拥有多个主体。举个例子：QQ上群组G的用户U发送了一条消息，该用户同时具有“用户U”、“群组G成员”、“QQ用户”、“Bot用户”这几个主体。同时QQ上群组G的用户V也发送了一条消息，该用户该用户同时具有“用户V”、“群组G成员”、“QQ用户”、“Bot用户”这几个主体。
-
-当设置权限时，我们直接针对一个主体进行设置。当鉴权时，我们对用户的所有主体**按优先级从高到低的顺序**
-，逐一检查是否设置了权限。一旦检查到某个主体设置了权限，就以该主体设置的权限作为该用户的权限。
-
-回到上面的例子，假设我们对主体”群组G“禁用服务，但是对主体”用户V“启用服务。则用户U在群组G内将无法使用服务，但是用户V在群组G内可以使用。
-
-在插件使用中，我们用一个字符串表示主体，例如`qq:12345678`表示QQ用户12345678、`qq:g87654321`表示QQ群组87654321。
-
-我们约定：`all`表示所有用户、`superuser`表示超级用户、`<平台名>`表示所有此平台的用户、`<协议名>`
-表示所有此协议的用户、所有与平台相关的主体均以`<平台名>:`开头、所有与协议相关的主体均以`<协议名>:`开头。
-
-插件依赖[nonebot-plugin-session](https://github.com/noneplugin/nonebot-plugin-session)提取事件的主体，各适配器的主体定义如下：
-
-- [OneBot V11](docs/onebot_v11.md)
-- [OneBot V12](docs/onebot_v12.md)
-- [Kaiheila](docs/kaiheila.md)
-- [QQ Guild](docs/qqguild.md)
-- Telegram：未测试，参考OneBot V12的定义
-
-### 服务
-
-**服务（Service）为一组能够进行权限控制的功能的集合。** 服务可以拥有子服务，通过树形结构组织服务，统一管理权限。
-
-整个NoneBot是一个名为nonebot的服务，为树形结构的根节点，其直接子节点为所有插件。
-
-一个插件是一个服务（PluginService），其父节点为nonebot。当插件未进行适配时，该插件只具有这一个PluginService。对插件进行适配，则需要从插件的PluginService创建SubService，为插件的Matcher等功能入口应用SubService。（参考下文插件适配章节）
-
-（为防止意外发生，nonebot_plugin_access_control本身不可以进行权限开关）
-
-当某主体需要检查某服务是否可用时，将从该服务开始检查是否为该主体配置了权限，若未配置则检查其父服务，以此类推直到检查到根节点nonebot。
-
-换句话说，当鉴权时，我们逐一对用户的所有主体**按优先级从高到低的顺序**，**按服务的节点深度从深到浅的顺序**
-检查该服务及其所有祖先节点配置的权限。因此，在节点深度较浅的服务配置的高优先级的主体配置，也会覆盖在节点深度较深的服务配置的低优先级的主体配置。
-
-通过指令可查看所有服务及子服务层级：
-
-- `/ac service ls`：列出所有服务与子服务层级
-- `/ac service ls --srv <服务>`：列出服务的子服务层级
-
-其中`<服务>`的格式如下：
-
-- `nonebot`：对整个NoneBot进行开关
-- `<插件名>`：对整个插件进行开关
-- `<插件名>.<子服务名>.<子服务名>.....<子服务名>`：对插件内的某个子服务进行开关（需参照下文对插件进行配置）
-
-### 鉴权
-
-通过指令可实现权限开关：
-
-- `/ac permission allow --sbj <主体> --srv <服务>`：为主体启用服务
-- `/ac permission deny --sbj <主体> --srv <服务>`：为主体禁用服务
-- `/ac permission rm --sbj <主体> --srv <服务>`：为主体删除服务权限配置
-- `/ac permission ls`：列出所有已配置的权限
-- `/ac permission ls --sbj <主体>`：列出主体已配置的服务权限
-- `/ac permission ls --srv <服务>`：列出服务已配置的主体权限
-- `/ac permission ls --sbj <主体> --srv <服务>`：列出主体与服务已配置的权限
-
-其中`<服务>`的格式同上
-
-### 限流
-
-插件还提供了限流的功能（限制同一用户在一定时间内的指令调用次数）。
-
-限流规则同样是针对服务及主体的。与鉴权不同的是，限流规则是串联的。应用在一个用户拥有的所有主体的限流规则，与应用在一个服务及其所有祖先服务的限流规则，会同时对用户产生限制。
-
-举个例子，如果我们设置了”主体`all`每天最多调用100次`nonebot`服务“，”主体`qq:g87654321`
-每分钟最多调用5次`nonebot_plugin_pixivbot`服务“。一位拥有`qq:12345678`、`qq:g87654321`、`qq`、`all`
-这四个主体的用户尝试调用`nonebot_plugin_pixivbot.xxx`服务时，将同时受到以上两条规则的限制。
-
-如果我不希望这样的串联，该怎么办？通过为规则设置”覆写“属性，可以覆盖掉所有优先级低于该规则的规则。规则的优先级比较规则如下：
-
-- 若主体优先级不一致，按照主体优先级
-- 否则，按照服务的父子关系，父服务优先级低于子服务
-
-通过指令可对限流规则进行操作：
-
-- `/ac limit add --sbj <主体> --srv <服务> --limit <次数> --span <时间间隔> [--overwrite]`
-  ：为主体与服务添加限流规则（`--overwrite`：为规则设置”覆写“属性）
-- `/ac limit rm <规则ID>`：删除限流规则
-- `/ac limit ls`：列出所有已配置的限流规则
-- `/ac limit ls --sbj <主体>`：列出主体已配置的限流规则
-- `/ac limit ls --srv <服务>`：列出服务已配置的限流规则
-- `/ac limit ls --sbj <主体> --srv <服务>`：列出主体与服务已配置的限流规则
-- `/ac limit reset`：重置限流计数
-
-其中`<服务>`的格式同上
-
-### 指令一览
-
-进行控制的指令为`/ac`，仅超级用户可用。（通过在配置文件中设置`SUPERUSERS`变量可设置超级用户）
-
-（注意：0.3.0版本对指令进行了一次大的更改）
-
-- 帮助
-    - `/ac help`：显示此帮助
-- 权限控制
-    - `/ac permission allow --sbj <主体> --srv <服务>`：为主体启用服务
-    - `/ac permission deny --sbj <主体> --srv <服务>`：为主体禁用服务
-    - `/ac permission rm --sbj <主体> --srv <服务>`：为主体删除服务权限配置
-    - `/ac permission ls`：列出所有已配置的权限
-    - `/ac permission ls --sbj <主体>`：列出主体已配置的服务权限
-    - `/ac permission ls --srv <服务>`：列出服务已配置的主体权限
-    - `/ac permission ls --sbj <主体> --srv <服务>`：列出主体与服务已配置的权限
-- 流量限制
-    - `/ac limit add --sbj <主体> --srv <服务> --limit <次数> --span <时间间隔> [--overwrite]`：为主体与服务添加限流规则
-    - `/ac limit rm <规则ID>`：删除限流规则
-    - `/ac limit ls`：列出所有已配置的限流规则
-    - `/ac limit ls --sbj <主体>`：列出主体已配置的限流规则
-    - `/ac limit ls --srv <服务>`：列出服务已配置的限流规则
-    - `/ac limit ls --sbj <主体> --srv <服务>`：列出主体与服务已配置的限流规则
-    - `/ac limit reset`：重置限流计数
-- 服务查看
-    - `/ac service ls`：列出所有服务与子服务层级
-    - `/ac service ls --srv <服务>`：列出服务的子服务层级
-- 主体测试
-    - `/ac subject`：列出消息发送者的所有主体
-
-其中`<服务>`的格式如下：
-
-- `nonebot`：对整个NoneBot进行开关
-- `<插件名>`：对整个插件进行开关
-- `<插件名>.<子服务名>.<子服务名>.....<子服务名>`：对插件内的某个子服务进行开关（需参照下文对插件进行配置）
-
-### 示例
-
-首先编辑配置文件，打开对未适配插件的支持：
-
-```
-ACCESS_CONTROL_AUTO_PATCH_ENABLED=true
-```
-
-假设bot加载了内置插件echo
-
-```python
-nonebot.load_builtin_plugins("echo")
-```
-
-#### 鉴权
-
-执行下面的指令后，QQ用户12345678将无法调用指令`/echo`
-
-```
-/ac permission deny --sbj qq:12345678 --srv echo
-```
-
-执行下面的指令后，QQ用户12345678将无法调用所有指令
-
-```
-/ac permission deny --sbj all --srv nonebot
-```
-
-执行下面的指令后，QQ群组87654321的所有用户（QQ用户12345678除外）将无法调用指令`/echo`
-
-```
-/ac permission allow --sbj qq:12345678 --srv echo
-/ac permission deny --sbj qq:g87654321 --srv echo
-```
-
-执行下面的指令后，所有用户将无法调用指令`/echo`
-
-```
-/ac permission deny --sbj all --srv echo
-```
-
-#### 限流
-
-执行下面的指令后，所有用户每天只能调用100次任意指令，且每分钟只能调用三次指令`/echo`
-
-```
-/ac limit add --sbj all --srv nonebot --span 1d --limit 100
-/ac limit add --sbj all --srv echo --span 1m --limit 3
-```
-
-执行下面的指令后，QQ群组87654321的所有用户（QQ用户12345678除外）每分钟只能调用三次指令`/echo`
-
-（QQ用户12345678每分钟能够调用114514次指令`/echo`）
-
-```
-/ac limit add --sbj qq:g87654321 --srv echo --span 1m --limit 3
-/ac limit add --sbj qq:12345678 --srv echo --span 1m --limit 114514 --overwrite
-```
-
-## 插件适配
-
-参考 [https://github.com/ssttkkl/nonebot-plugin-access-control-api/blob/v1.1.0/README.MD]
-
-## CLI支持
-
-可以通过控制台中执行`nb accctrl`进入权限控制台，使用方式与`/ac`指令类似。
-
-## 配置项
-
-### 数据库配置
-
-参考 https://github.com/nonebot/plugin-orm#%E9%85%8D%E7%BD%AE%E9%A1%B9
-
-### access_control_default_permission
-
-未设置权限时的默认行为
-
-可选值：`allow`, `deny`
-
-默认值：`allow`
-
-### access_control_auto_patch_enabled
-
-是否启用对未适配插件的权限控制
-
-类型：`bool`
-
-默认值：`False`
-
-### access_control_auto_patch_ignore
-
-对指定的未适配插件将不启用权限控制
-
-类型：`List[str]`
-
-默认值：`[]`
-
-### access_control_reply_on_permission_denied_enabled
-
-因无权限而拒绝执行时，是否向用户回复消息
-
-类型：`bool`
-
-默认值：`False`
-
-### access_control_reply_on_permission_denied
-
-因无权限而拒绝执行时向用户回复的消息
-
-类型：`str`
-
-默认值：`"你没有权限执行该指令"`
-
-### access_control_reply_on_rate_limited_enabled
-
-因到达最大次数而拒绝执行时，是否向用户回复消息
-
-类型：`bool`
-
-默认值：`False`
-
-### access_control_reply_on_rate_limited
-
-因到达最大次数而拒绝执行时向用户回复的消息
-
-类型：`str`
-
-### access_control_rate_limit_token_storage
-
-限流计数使用的存储方式，支持内存存储（inmemory）与数据库存储（datastore）。
-
-内存存储会在重启后重置限流计数，数据库存储则不会。同时数据库存储还能够实现多个NoneBot实例共享限流计数，适用于分布式Bot应用。
-
-在性能上，内存存储优于数据库存储。默认使用的是内存存储。
-
-可选值：`inmemory`, `datastore`
-
-默认值：`inmemory`
-
-## Q&A
-
-### **本插件与[nonebot_plugin_rauthman](https://github.com/Lancercmd/nonebot_plugin_rauthman)
-
-和[nonebot-plugin-manager](https://github.com/nonepkg/nonebot-plugin-manager)等其他权限管理插件有什么差别？**
-
-[nonebot_plugin_rauthman](https://github.com/Lancercmd/nonebot_plugin_rauthman)
-支持功能级别的细粒度权限控制，但是需要插件进行适配，对于未适配插件不起作用。[nonebot-plugin-manager](https://github.com/nonepkg/nonebot-plugin-manager)
-则实现了非侵入式的权限控制。
-
-本插件主要受这两个插件的启发，结合了这两个插件的优点。既支持非侵入式应用到原有插件，也支持对插件进行适配以获得更多feature。同时提供事件订阅机制，以便插件开发者更灵活处理权限。
-
-同时，上述两款插件均只支持OneBot V11协议，而本插件设计之初就考虑到了除OneBot V11以外的协议，具有更强的可扩展性。
-
-## 在线乞讨
-
-<details><summary>点击请我打两把maimai</summary>
-
-![](https://github.com/ssttkkl/ssttkkl/blob/main/afdian-ssttkkl.jfif)
-
-</details>
-
-## LICENSE
-
-> MIT License
->
-> Copyright (c) 2022 ssttkkl
->
-> Permission is hereby granted, free of charge, to any person obtaining a copy
-> of this software and associated documentation files (the "Software"), to deal
-> in the Software without restriction, including without limitation the rights
-> to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-> copies of the Software, and to permit persons to whom the Software is
-> furnished to do so, subject to the following conditions:
->
-> The above copyright notice and this permission notice shall be included in all
-> copies or substantial portions of the Software.
->
-> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-> SOFTWARE.
-> 
+<!-- markdownlint-disable MD033 MD036 MD041 -->
+
+<p align="center">
+  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+</p>
+
+<div align="center">
+
+nonebot-plugin-access-control
+============
+
+_✨ Nonebot 权限控制插件 ✨_
+
+</div>
+
+
+<p align="center">
+  <a href="https://raw.githubusercontent.com/ssttkkl/nonebot-plugin-access-control/master/LICENSE">
+    <img src="https://img.shields.io/github/license/ssttkkl/nonebot-plugin-access-control.svg" alt="license">
+  </a>
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-access-control">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-access-control.svg" alt="pypi">
+  </a>
+  <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+</p>
+
+## 特点
+
+- 功能
+    - [x] 支持针对用户/群组的权限开关
+    - [x] 支持限制同一用户在一定时间内的指令调用次数
+    - [x] 对未适配插件提供**插件级别**的控制支持
+- 插件适配
+    - [x] 支持**功能级别**的细粒度控制
+    - [x] 支持对权限开关等事件进行订阅
+- 拓展
+    - [x] 支持开发者拓展定义新的主体
+- CLI插件
+    - [x] 支持通过控制台中执行`nb accctrl`进入权限控制台
+
+## 使用
+
+### 主体
+
+#### 概念
+
+当我们对用户进行权限控制时，我们想要的是针对拥有某种同样身份的所有用户进行配置，而不是对每一个具体用户分别配置。因此，我们引入主体的概念。
+**主体（Subject）代表了拥有某种同样身份的用户的集合，也是设置权限的基本单位。**
+当我们说用户具有某个主体，也就是说用户在该主体所代表的集合内。换句话说，主体就是一个用户所具有的身份。
+
+一个用户通常拥有多个主体。举个例子：QQ上群组G的用户U发送了一条消息，该用户同时具有“用户U”、“群组G成员”、“QQ用户”、“Bot用户”这几个主体。同时QQ上群组G的用户V也发送了一条消息，该用户该用户同时具有“用户V”、“群组G成员”、“QQ用户”、“Bot用户”这几个主体。
+
+当设置权限时，我们直接针对一个主体进行设置。当鉴权时，我们对用户的所有主体**按优先级从高到低的顺序**
+，逐一检查是否设置了权限。一旦检查到某个主体设置了权限，就以该主体设置的权限作为该用户的权限。
+
+回到上面的例子，假设我们对主体”群组G“禁用服务，但是对主体”用户V“启用服务。则用户U在群组G内将无法使用服务，但是用户V在群组G内可以使用。
+
+在插件使用中，我们用一个字符串表示主体，例如`qq:12345678`表示QQ用户12345678、`qq:g87654321`表示QQ群组87654321。
+
+我们约定：`all`表示所有用户、`superuser`表示超级用户、`<平台名>`表示所有此平台的用户、`<协议名>`
+表示所有此协议的用户、所有与平台相关的主体均以`<平台名>:`开头、所有与协议相关的主体均以`<协议名>:`开头。
+
+插件依赖[nonebot-plugin-session](https://github.com/noneplugin/nonebot-plugin-session)提取事件的主体，各适配器的主体定义如下：
+
+- [OneBot V11](docs/onebot_v11.md)
+- [OneBot V12](docs/onebot_v12.md)
+- [Kaiheila](docs/kaiheila.md)
+- [QQ Guild](docs/qqguild.md)
+- Telegram：未测试，参考OneBot V12的定义
+
+### 服务
+
+**服务（Service）为一组能够进行权限控制的功能的集合。** 服务可以拥有子服务，通过树形结构组织服务，统一管理权限。
+
+整个NoneBot是一个名为nonebot的服务，为树形结构的根节点，其直接子节点为所有插件。
+
+一个插件是一个服务（PluginService），其父节点为nonebot。当插件未进行适配时，该插件只具有这一个PluginService。对插件进行适配，则需要从插件的PluginService创建SubService，为插件的Matcher等功能入口应用SubService。（参考下文插件适配章节）
+
+（为防止意外发生，nonebot_plugin_access_control本身不可以进行权限开关）
+
+当某主体需要检查某服务是否可用时，将从该服务开始检查是否为该主体配置了权限，若未配置则检查其父服务，以此类推直到检查到根节点nonebot。
+
+换句话说，当鉴权时，我们逐一对用户的所有主体**按优先级从高到低的顺序**，**按服务的节点深度从深到浅的顺序**
+检查该服务及其所有祖先节点配置的权限。因此，在节点深度较浅的服务配置的高优先级的主体配置，也会覆盖在节点深度较深的服务配置的低优先级的主体配置。
+
+通过指令可查看所有服务及子服务层级：
+
+- `/ac service ls`：列出所有服务与子服务层级
+- `/ac service ls --srv <服务>`：列出服务的子服务层级
+
+其中`<服务>`的格式如下：
+
+- `nonebot`：对整个NoneBot进行开关
+- `<插件名>`：对整个插件进行开关
+- `<插件名>.<子服务名>.<子服务名>.....<子服务名>`：对插件内的某个子服务进行开关（需参照下文对插件进行配置）
+
+### 鉴权
+
+通过指令可实现权限开关：
+
+- `/ac permission allow --sbj <主体> --srv <服务>`：为主体启用服务
+- `/ac permission deny --sbj <主体> --srv <服务>`：为主体禁用服务
+- `/ac permission rm --sbj <主体> --srv <服务>`：为主体删除服务权限配置
+- `/ac permission ls`：列出所有已配置的权限
+- `/ac permission ls --sbj <主体>`：列出主体已配置的服务权限
+- `/ac permission ls --srv <服务>`：列出服务已配置的主体权限
+- `/ac permission ls --sbj <主体> --srv <服务>`：列出主体与服务已配置的权限
+
+其中`<服务>`的格式同上
+
+### 限流
+
+插件还提供了限流的功能（限制同一用户在一定时间内的指令调用次数）。
+
+限流规则同样是针对服务及主体的。与鉴权不同的是，限流规则是串联的。应用在一个用户拥有的所有主体的限流规则，与应用在一个服务及其所有祖先服务的限流规则，会同时对用户产生限制。
+
+举个例子，如果我们设置了”主体`all`每天最多调用100次`nonebot`服务“，”主体`qq:g87654321`
+每分钟最多调用5次`nonebot_plugin_pixivbot`服务“。一位拥有`qq:12345678`、`qq:g87654321`、`qq`、`all`
+这四个主体的用户尝试调用`nonebot_plugin_pixivbot.xxx`服务时，将同时受到以上两条规则的限制。
+
+如果我不希望这样的串联，该怎么办？通过为规则设置”覆写“属性，可以覆盖掉所有优先级低于该规则的规则。规则的优先级比较规则如下：
+
+- 若主体优先级不一致，按照主体优先级
+- 否则，按照服务的父子关系，父服务优先级低于子服务
+
+通过指令可对限流规则进行操作：
+
+- `/ac limit add --sbj <主体> --srv <服务> --limit <次数> --span <时间间隔> [--overwrite]`
+  ：为主体与服务添加限流规则（`--overwrite`：为规则设置”覆写“属性）
+- `/ac limit rm <规则ID>`：删除限流规则
+- `/ac limit ls`：列出所有已配置的限流规则
+- `/ac limit ls --sbj <主体>`：列出主体已配置的限流规则
+- `/ac limit ls --srv <服务>`：列出服务已配置的限流规则
+- `/ac limit ls --sbj <主体> --srv <服务>`：列出主体与服务已配置的限流规则
+- `/ac limit reset`：重置限流计数
+
+其中`<服务>`的格式同上
+
+### 指令一览
+
+进行控制的指令为`/ac`，仅超级用户可用。（通过在配置文件中设置`SUPERUSERS`变量可设置超级用户）
+
+（注意：0.3.0版本对指令进行了一次大的更改）
+
+- 帮助
+    - `/ac help`：显示此帮助
+- 权限控制
+    - `/ac permission allow --sbj <主体> --srv <服务>`：为主体启用服务
+    - `/ac permission deny --sbj <主体> --srv <服务>`：为主体禁用服务
+    - `/ac permission rm --sbj <主体> --srv <服务>`：为主体删除服务权限配置
+    - `/ac permission ls`：列出所有已配置的权限
+    - `/ac permission ls --sbj <主体>`：列出主体已配置的服务权限
+    - `/ac permission ls --srv <服务>`：列出服务已配置的主体权限
+    - `/ac permission ls --sbj <主体> --srv <服务>`：列出主体与服务已配置的权限
+- 流量限制
+    - `/ac limit add --sbj <主体> --srv <服务> --limit <次数> --span <时间间隔> [--overwrite]`：为主体与服务添加限流规则
+    - `/ac limit rm <规则ID>`：删除限流规则
+    - `/ac limit ls`：列出所有已配置的限流规则
+    - `/ac limit ls --sbj <主体>`：列出主体已配置的限流规则
+    - `/ac limit ls --srv <服务>`：列出服务已配置的限流规则
+    - `/ac limit ls --sbj <主体> --srv <服务>`：列出主体与服务已配置的限流规则
+    - `/ac limit reset`：重置限流计数
+- 服务查看
+    - `/ac service ls`：列出所有服务与子服务层级
+    - `/ac service ls --srv <服务>`：列出服务的子服务层级
+- 主体测试
+    - `/ac subject`：列出消息发送者的所有主体
+
+其中`<服务>`的格式如下：
+
+- `nonebot`：对整个NoneBot进行开关
+- `<插件名>`：对整个插件进行开关
+- `<插件名>.<子服务名>.<子服务名>.....<子服务名>`：对插件内的某个子服务进行开关（需参照下文对插件进行配置）
+
+### 示例
+
+首先编辑配置文件，打开对未适配插件的支持：
+
+```
+ACCESS_CONTROL_AUTO_PATCH_ENABLED=true
+```
+
+假设bot加载了内置插件echo
+
+```python
+nonebot.load_builtin_plugins("echo")
+```
+
+#### 鉴权
+
+执行下面的指令后，QQ用户12345678将无法调用指令`/echo`
+
+```
+/ac permission deny --sbj qq:12345678 --srv echo
+```
+
+执行下面的指令后，QQ用户12345678将无法调用所有指令
+
+```
+/ac permission deny --sbj all --srv nonebot
+```
+
+执行下面的指令后，QQ群组87654321的所有用户（QQ用户12345678除外）将无法调用指令`/echo`
+
+```
+/ac permission allow --sbj qq:12345678 --srv echo
+/ac permission deny --sbj qq:g87654321 --srv echo
+```
+
+执行下面的指令后，所有用户将无法调用指令`/echo`
+
+```
+/ac permission deny --sbj all --srv echo
+```
+
+#### 限流
+
+执行下面的指令后，所有用户每天只能调用100次任意指令，且每分钟只能调用三次指令`/echo`
+
+```
+/ac limit add --sbj all --srv nonebot --span 1d --limit 100
+/ac limit add --sbj all --srv echo --span 1m --limit 3
+```
+
+执行下面的指令后，QQ群组87654321的所有用户（QQ用户12345678除外）每分钟只能调用三次指令`/echo`
+
+（QQ用户12345678每分钟能够调用114514次指令`/echo`）
+
+```
+/ac limit add --sbj qq:g87654321 --srv echo --span 1m --limit 3
+/ac limit add --sbj qq:12345678 --srv echo --span 1m --limit 114514 --overwrite
+```
+
+## 插件适配
+
+参考 [https://github.com/ssttkkl/nonebot-plugin-access-control-api/blob/v1.1.0/README.MD]
+
+## CLI支持
+
+可以通过控制台中执行`nb accctrl`进入权限控制台，使用方式与`/ac`指令类似。
+
+## 配置项
+
+### 数据库配置
+
+参考 https://github.com/nonebot/plugin-orm#%E9%85%8D%E7%BD%AE%E9%A1%B9
+
+### access_control_default_permission
+
+未设置权限时的默认行为
+
+可选值：`allow`, `deny`
+
+默认值：`allow`
+
+### access_control_auto_patch_enabled
+
+是否启用对未适配插件的权限控制
+
+类型：`bool`
+
+默认值：`False`
+
+### access_control_auto_patch_ignore
+
+对指定的未适配插件将不启用权限控制
+
+类型：`List[str]`
+
+默认值：`[]`
+
+### access_control_reply_on_permission_denied_enabled
+
+因无权限而拒绝执行时，是否向用户回复消息
+
+类型：`bool`
+
+默认值：`False`
+
+### access_control_reply_on_permission_denied
+
+因无权限而拒绝执行时向用户回复的消息
+
+类型：`str`
+
+默认值：`"你没有权限执行该指令"`
+
+### access_control_reply_on_rate_limited_enabled
+
+因到达最大次数而拒绝执行时，是否向用户回复消息
+
+类型：`bool`
+
+默认值：`False`
+
+### access_control_reply_on_rate_limited
+
+因到达最大次数而拒绝执行时向用户回复的消息
+
+类型：`str`
+
+### access_control_rate_limit_token_storage
+
+限流计数使用的存储方式，支持内存存储（inmemory）与数据库存储（datastore）。
+
+内存存储会在重启后重置限流计数，数据库存储则不会。同时数据库存储还能够实现多个NoneBot实例共享限流计数，适用于分布式Bot应用。
+
+在性能上，内存存储优于数据库存储。默认使用的是内存存储。
+
+可选值：`inmemory`, `datastore`
+
+默认值：`inmemory`
+
+## Q&A
+
+### **本插件与[nonebot_plugin_rauthman](https://github.com/Lancercmd/nonebot_plugin_rauthman)
+
+和[nonebot-plugin-manager](https://github.com/nonepkg/nonebot-plugin-manager)等其他权限管理插件有什么差别？**
+
+[nonebot_plugin_rauthman](https://github.com/Lancercmd/nonebot_plugin_rauthman)
+支持功能级别的细粒度权限控制，但是需要插件进行适配，对于未适配插件不起作用。[nonebot-plugin-manager](https://github.com/nonepkg/nonebot-plugin-manager)
+则实现了非侵入式的权限控制。
+
+本插件主要受这两个插件的启发，结合了这两个插件的优点。既支持非侵入式应用到原有插件，也支持对插件进行适配以获得更多feature。同时提供事件订阅机制，以便插件开发者更灵活处理权限。
+
+同时，上述两款插件均只支持OneBot V11协议，而本插件设计之初就考虑到了除OneBot V11以外的协议，具有更强的可扩展性。
+
+## 在线乞讨
+
+<details><summary>点击请我打两把maimai</summary>
+
+![](https://github.com/ssttkkl/ssttkkl/blob/main/afdian-ssttkkl.jfif)
+
+</details>
+
+## LICENSE
+
+> MIT License
+>
+> Copyright (c) 2022 ssttkkl
+>
+> Permission is hereby granted, free of charge, to any person obtaining a copy
+> of this software and associated documentation files (the "Software"), to deal
+> in the Software without restriction, including without limitation the rights
+> to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+> copies of the Software, and to permit persons to whom the Software is
+> furnished to do so, subject to the following conditions:
+>
+> The above copyright notice and this permission notice shall be included in all
+> copies or substantial portions of the Software.
+>
+> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+> SOFTWARE.
+>
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/__init__.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-"""
-nonebot-plugin-access-control
-
-@Author         : ssttkkl
-@License        : MIT
-@GitHub         : https://github.com/bot-ssttkkl/nonebot-plugin-access-control
-"""
-from nonebot import require
-
-require("nonebot_plugin_access_control_api")
-require("nonebot_plugin_apscheduler")
-require("nonebot_plugin_session")
-require("nonebot_plugin_orm")
-
-from nonebot.plugin import PluginMetadata, inherit_supported_adapters
-
-from .alc import help_ac
-from .config import Config
-from . import orm_migrations
-
-__plugin_meta__ = PluginMetadata(
-    name="权限控制",
-    description="对功能进行权限控制以及调用次数限制",
-    usage=help_ac(),
-    type="application",
-    homepage="https://github.com/bot-ssttkkl/nonebot-plugin-access-control",
-    config=Config,
-    supported_adapters=inherit_supported_adapters("nonebot_plugin_session"),
-    extra={"orm_version_location": orm_migrations},
-)
-
-from . import matcher  # noqa
-from . import service  # noqa
-from . import subject  # noqa
-from . import datastore  # noqa
+"""
+nonebot-plugin-access-control
+
+@Author         : ssttkkl
+@License        : MIT
+@GitHub         : https://github.com/bot-ssttkkl/nonebot-plugin-access-control
+"""
+
+from nonebot import require
+
+require("nonebot_plugin_access_control_api")
+require("nonebot_plugin_apscheduler")
+require("nonebot_plugin_session")
+require("nonebot_plugin_orm")
+
+from nonebot.plugin import PluginMetadata, inherit_supported_adapters
+
+from .alc import help_ac
+from .config import Config
+from . import orm_migrations
+
+__plugin_meta__ = PluginMetadata(
+    name="权限控制",
+    description="对功能进行权限控制以及调用次数限制",
+    usage=help_ac(),
+    type="application",
+    homepage="https://github.com/bot-ssttkkl/nonebot-plugin-access-control",
+    config=Config,
+    supported_adapters=inherit_supported_adapters("nonebot_plugin_session"),
+    extra={"orm_version_location": orm_migrations},
+)
+
+from . import matcher  # noqa
+from . import service  # noqa
+from . import subject  # noqa
+from . import datastore  # noqa
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/config.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from typing import Literal, Optional
-
-from nonebot import get_driver
-from pydantic import Field, BaseSettings
-
-
-class Config(BaseSettings):
-    access_control_default_permission: Literal["allow", "deny"] = "allow"
-
-    access_control_rate_limit_token_storage: Literal[
-        "datastore", "inmemory"
-    ] = "inmemory"
-
-    access_control_auto_patch_enabled: bool = False
-    access_control_auto_patch_ignore: list[str] = Field(default_factory=list)
-
-    access_control_reply_on_permission_denied_enabled: bool = False
-    access_control_reply_on_permission_denied: str = "你没有权限执行该指令"
-    access_control_reply_on_rate_limited_enabled: bool = True
-    access_control_reply_on_rate_limited: Optional[str]
-
-    class Config:
-        extra = "ignore"
-
-
-_conf: Optional[Config] = None
-
-
-def conf() -> Config:
-    global _conf
-    if _conf is None:
-        _conf = Config(**get_driver().config.dict())
-    return _conf
+from typing import Literal, Optional
+
+from pydantic import Field
+from nonebot import get_driver
+from pydantic_settings import BaseSettings
+
+
+class Config(BaseSettings):
+    access_control_default_permission: Literal["allow", "deny"] = "allow"
+
+    access_control_rate_limit_token_storage: Literal["datastore", "inmemory"] = (
+        "inmemory"
+    )
+
+    access_control_auto_patch_enabled: bool = False
+    access_control_auto_patch_ignore: list[str] = Field(default_factory=list)
+
+    access_control_reply_on_permission_denied_enabled: bool = False
+    access_control_reply_on_permission_denied: str = "你没有权限执行该指令"
+    access_control_reply_on_rate_limited_enabled: bool = True
+    access_control_reply_on_rate_limited: Optional[str] = None
+
+    class Config:
+        extra = "ignore"
+
+
+_conf: Optional[Config] = None
+
+
+def conf() -> Config:
+    global _conf
+    if _conf is None:
+        _conf = Config(**get_driver().config.dict())
+    return _conf
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/datastore/__init__.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/datastore/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-"""
-用于将datastore数据库迁移到最新版本后再进行数据迁移
-"""
-
-from pathlib import Path
-
-from nonebot import require
-from pkg_resources import DistributionNotFound, get_distribution
-
-
-def _prepare():
-    try:
-        get_distribution("nonebot_plugin_datastore")
-    except DistributionNotFound:
-        return
-
-    require("nonebot_plugin_datastore")
-
-    from nonebot_plugin_datastore import get_plugin_data
-
-    plugin_data = get_plugin_data("nonebot_plugin_access_control")
-
-    migrations_dir = Path(__file__).parent / "migrations"
-    plugin_data.set_migration_dir(migrations_dir)
-
-    # 保证将插件加入datastore的待迁移列表
-    plugin_data.Model  # noqa
-
-
-_prepare()
+"""
+用于将datastore数据库迁移到最新版本后再进行数据迁移
+"""
+
+from pathlib import Path
+
+from nonebot import require
+from pkg_resources import DistributionNotFound, get_distribution
+
+
+def _prepare():
+    try:
+        get_distribution("nonebot_plugin_datastore")
+    except DistributionNotFound:
+        return
+
+    require("nonebot_plugin_datastore")
+
+    from nonebot_plugin_datastore import get_plugin_data
+
+    plugin_data = get_plugin_data("nonebot_plugin_access_control")
+
+    migrations_dir = Path(__file__).parent / "migrations"
+    plugin_data.set_migration_dir(migrations_dir)
+
+    # 保证将插件加入datastore的待迁移列表
+    plugin_data.Model  # noqa
+
+
+_prepare()
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/datastore/migrations/875c4dd8c271_.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/orm_migrations/9bb3231cf9aa_init_db.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,91 @@
-"""empty message
-
-Revision ID: 875c4dd8c271
-Revises:
-Create Date: 2023-03-11 22:32:32.995987
-
-"""
-import sqlalchemy as sa
-from alembic import op
-
-# revision identifiers, used by Alembic.
-from sqlalchemy import Inspector
-
-revision = "875c4dd8c271"
-down_revision = None
-branch_labels = None
-depends_on = None
-
-
-def upgrade() -> None:
-    conn = op.get_bind()
-    inspector = Inspector.from_engine(conn.engine)
-    tables = inspector.get_table_names()
-
-    # ### commands auto generated by Alembic - please adjust! ###
-    if "nonebot_plugin_access_control_permission" not in tables:
-        op.create_table(
-            "nonebot_plugin_access_control_permission",
-            sa.Column("subject", sa.String(), nullable=False),
-            sa.Column("service", sa.String(), nullable=False),
-            sa.Column("allow", sa.Boolean(), nullable=False),
-            sa.PrimaryKeyConstraint("subject", "service"),
-        )
-
-    if "nonebot_plugin_access_control_rate_limit_rule" not in tables:
-        op.create_table(
-            "nonebot_plugin_access_control_rate_limit_rule",
-            sa.Column("id", sa.String(), nullable=False),
-            sa.Column("subject", sa.String(), nullable=False),
-            sa.Column("service", sa.String(), nullable=False),
-            sa.Column("time_span", sa.Integer(), nullable=False),
-            sa.Column("limit", sa.Integer(), nullable=False),
-            sa.Column("overwrite", sa.Boolean(), nullable=False),
-            sa.PrimaryKeyConstraint("id"),
-        )
-        with op.batch_alter_table(
-            "nonebot_plugin_access_control_rate_limit_rule", schema=None
-        ) as batch_op:
-            batch_op.create_index(
-                "ix_nonebot_plugin_access_control_rate_limit_rule_subject_service",
-                ["subject", "service"],
-                unique=False,
-            )
-
-    if "nonebot_plugin_access_control_rate_limit_token" not in tables:
-        op.create_table(
-            "nonebot_plugin_access_control_rate_limit_token",
-            sa.Column("id", sa.Integer(), nullable=False),
-            sa.Column("rule_id", sa.String(), nullable=False),
-            sa.Column("user", sa.String(), nullable=False),
-            sa.Column("acquire_time", sa.DateTime(), nullable=False),
-            sa.ForeignKeyConstraint(
-                ["rule_id"],
-                ["nonebot_plugin_access_control_rate_limit_rule.id"],
-            ),
-            sa.PrimaryKeyConstraint("id"),
-        )
-        with op.batch_alter_table(
-            "nonebot_plugin_access_control_rate_limit_token", schema=None
-        ) as batch_op:
-            batch_op.create_index(
-                batch_op.f("ix_nonebot_plugin_access_control_rate_limit_token_rule_id"),
-                ["rule_id"],
-                unique=False,
-            )
-
-    # ### end Alembic commands ###
-
-
-def downgrade() -> None:
-    # ### commands auto generated by Alembic - please adjust! ###
-    with op.batch_alter_table(
-        "nonebot_plugin_access_control_rate_limit_token", schema=None
-    ) as batch_op:
-        batch_op.drop_index(
-            batch_op.f("ix_nonebot_plugin_access_control_rate_limit_token_rule_id")
-        )
-
-    op.drop_table("nonebot_plugin_access_control_rate_limit_token")
-    with op.batch_alter_table(
-        "nonebot_plugin_access_control_rate_limit_rule", schema=None
-    ) as batch_op:
-        batch_op.drop_index(
-            "ix_nonebot_plugin_access_control_rate_limit_rule_subject_service"
-        )
-
-    op.drop_table("nonebot_plugin_access_control_rate_limit_rule")
-    op.drop_table("nonebot_plugin_access_control_permission")
-    # ### end Alembic commands ###
+"""init_db
+
+修订 ID: 9bb3231cf9aa
+父修订:
+创建时间: 2023-10-10 21:21:15.574058
+
+"""
+
+from __future__ import annotations
+
+from collections.abc import Sequence
+
+import sqlalchemy as sa
+from alembic import op
+
+revision: str = "9bb3231cf9aa"
+down_revision: str | Sequence[str] | None = None
+branch_labels: str | Sequence[str] | None = ("nonebot_plugin_access_control",)
+depends_on: str | Sequence[str] | None = None
+
+
+def upgrade(name: str = "") -> None:
+    if name:
+        return
+    # ### commands auto generated by Alembic - please adjust! ###
+    op.create_table(
+        "accctrl_permission",
+        sa.Column("subject", sa.String(), nullable=False),
+        sa.Column("service", sa.String(), nullable=False),
+        sa.Column("allow", sa.Boolean(), nullable=False),
+        sa.PrimaryKeyConstraint(
+            "subject", "service", name=op.f("pk_accctrl_permission")
+        ),
+    )
+    op.create_table(
+        "accctrl_rate_limit_rule",
+        sa.Column("id", sa.String(), nullable=False),
+        sa.Column("subject", sa.String(), nullable=False),
+        sa.Column("service", sa.String(), nullable=False),
+        sa.Column("time_span", sa.Integer(), nullable=False),
+        sa.Column("limit", sa.Integer(), nullable=False),
+        sa.Column("overwrite", sa.Boolean(), nullable=False),
+        sa.PrimaryKeyConstraint("id", name=op.f("pk_accctrl_rate_limit_rule")),
+    )
+    with op.batch_alter_table("accctrl_rate_limit_rule", schema=None) as batch_op:
+        batch_op.create_index(
+            "ix_accctrl_rate_limit_rule_subject_service",
+            ["subject", "service"],
+            unique=False,
+        )
+
+    op.create_table(
+        "accctrl_rate_limit_token",
+        sa.Column("id", sa.Integer(), nullable=False),
+        sa.Column("rule_id", sa.String(), nullable=False),
+        sa.Column("user", sa.String(), nullable=False),
+        sa.Column("acquire_time", sa.DateTime(), nullable=False),
+        sa.Column("expire_time", sa.DateTime(), nullable=False),
+        sa.ForeignKeyConstraint(
+            ["rule_id"],
+            ["accctrl_rate_limit_rule.id"],
+            name=op.f("fk_accctrl_rate_limit_token_rule_id_accctrl_rate_limit_rule"),
+        ),
+        sa.PrimaryKeyConstraint("id", name=op.f("pk_accctrl_rate_limit_token")),
+    )
+    with op.batch_alter_table("accctrl_rate_limit_token", schema=None) as batch_op:
+        batch_op.create_index(
+            "ix_accctrl_rate_limit_token_expire_time", ["expire_time"], unique=False
+        )
+        batch_op.create_index(
+            "ix_accctrl_rate_limit_token_rule_id", ["rule_id"], unique=False
+        )
+
+    # ### end Alembic commands ###
+
+
+def downgrade(name: str = "") -> None:
+    if name:
+        return
+    # ### commands auto generated by Alembic - please adjust! ###
+    with op.batch_alter_table("accctrl_rate_limit_token", schema=None) as batch_op:
+        batch_op.drop_index("ix_accctrl_rate_limit_token_rule_id")
+        batch_op.drop_index("ix_accctrl_rate_limit_token_expire_time")
+
+    op.drop_table("accctrl_rate_limit_token")
+    with op.batch_alter_table("accctrl_rate_limit_rule", schema=None) as batch_op:
+        batch_op.drop_index("ix_accctrl_rate_limit_rule_subject_service")
+
+    op.drop_table("accctrl_rate_limit_rule")
+    op.drop_table("accctrl_permission")
+    # ### end Alembic commands ###
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/handler/limit_handler.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/limit_handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,119 +1,121 @@
-from typing import TextIO, Optional
-
-import pytimeparser
-from nonebot_plugin_access_control_api.service import Service
-from nonebot_plugin_access_control_api.models.rate_limit import RateLimitRule
-from nonebot_plugin_access_control_api.service.methods import (
-    get_service_by_qualified_name,
-)
-from nonebot_plugin_access_control_api.errors import (
-    AccessControlQueryError,
-    AccessControlBadRequestError,
-)
-
-from ..repository.utils import use_ac_session
-from .utils.permission import require_superuser_or_script
-
-
-def _map_rule(f: TextIO, rule: RateLimitRule, service_name: Optional[str]):
-    f.write(
-        f"[{rule.id}] 服务 '{rule.service.qualified_name}' "
-        f"限制主体 '{rule.subject}' "
-        f"每 {int(rule.time_span.total_seconds())} 秒钟"
-        f"最多调用 {rule.limit} 次 "
-    )
-    if rule.overwrite:
-        f.write(" (覆写)")
-    if service_name is not None and rule.service.qualified_name != service_name:
-        f.write(f" (继承自服务 '{rule.service.qualified_name}')")
-
-
-@require_superuser_or_script
-async def add(
-    f: TextIO,
-    service_name: Optional[str],
-    subject: Optional[str],
-    limit: Optional[int],
-    time_span: Optional[str],
-    overwrite: Optional[bool],
-):
-    if not subject or not service_name:
-        raise AccessControlBadRequestError("请指定服务名（--service）与主体（--subject）")
-    elif not time_span:
-        raise AccessControlBadRequestError("请指定限制时间段（--span）")
-    elif not limit:
-        raise AccessControlBadRequestError("请指定限制次数（--limit）")
-    elif limit <= 0:
-        raise AccessControlBadRequestError("限制次数（--limit）必须大于0")
-
-    try:
-        parsed_time_span = pytimeparser.parse(time_span)
-    except ValueError:
-        raise AccessControlBadRequestError("给定的限制时间段（--span）不合法")
-
-    async with use_ac_session():
-        service = get_service_by_qualified_name(service_name)
-        if service is None:
-            raise AccessControlQueryError(f"找不到服务 {service_name}")
-
-        rule = await service.add_rate_limit_rule(
-            subject, parsed_time_span, limit, overwrite or False
-        )
-    _map_rule(f, rule, service_name)
-
-
-@require_superuser_or_script
-async def rm(
-    f: TextIO,
-    rule_id: Optional[str],
-):
-    if not rule_id:
-        raise AccessControlBadRequestError("请指定限流规则ID")
-
-    async with use_ac_session():
-        ok = await Service.remove_rate_limit_rule(rule_id)
-    if ok:
-        f.write("删除成功")
-    else:
-        raise AccessControlQueryError("删除失败，未找到该限流规则")
-
-
-@require_superuser_or_script
-async def ls(f: TextIO, service_name: Optional[str], subject: Optional[str]):
-    async with use_ac_session():
-        if not service_name and not subject:
-            rules = [x async for x in Service.get_all_rate_limit_rules()]
-        elif not service_name:
-            rules = [
-                x async for x in Service.get_all_rate_limit_rules_by_subject(subject)
-            ]
-        else:
-            service = get_service_by_qualified_name(
-                service_name, raise_on_not_exists=True
-            )
-
-            if not subject:
-                rules = [x async for x in service.get_rate_limit_rules()]
-            else:
-                rules = [
-                    x async for x in service.get_rate_limit_rules_by_subject(subject)
-                ]
-
-    if len(rules) != 0:
-        # 按照服务全称、subject排序
-        rules = sorted(rules, key=lambda x: (x.service.qualified_name, x.subject, x.id))
-
-        for rule in rules:
-            _map_rule(f, rule, service_name)
-            f.write("\n")
-    else:
-        f.write("无")
-
-
-@require_superuser_or_script
-async def reset(
-    f: TextIO,
-):
-    async with use_ac_session():
-        await Service.clear_rate_limit_tokens()
-    f.write("成功")
+from typing import TextIO, Optional
+
+import pytimeparser
+from nonebot_plugin_access_control_api.service import Service
+from nonebot_plugin_access_control_api.models.rate_limit import RateLimitRule
+from nonebot_plugin_access_control_api.service.methods import (
+    get_service_by_qualified_name,
+)
+from nonebot_plugin_access_control_api.errors import (
+    AccessControlQueryError,
+    AccessControlBadRequestError,
+)
+
+from ..repository.utils import use_ac_session
+from .utils.permission import require_superuser_or_script
+
+
+def _map_rule(f: TextIO, rule: RateLimitRule, service_name: Optional[str]):
+    f.write(
+        f"[{rule.id}] 服务 '{rule.service.qualified_name}' "
+        f"限制主体 '{rule.subject}' "
+        f"每 {int(rule.time_span.total_seconds())} 秒钟"
+        f"最多调用 {rule.limit} 次 "
+    )
+    if rule.overwrite:
+        f.write(" (覆写)")
+    if service_name is not None and rule.service.qualified_name != service_name:
+        f.write(f" (继承自服务 '{rule.service.qualified_name}')")
+
+
+@require_superuser_or_script
+async def add(
+    f: TextIO,
+    service_name: Optional[str],
+    subject: Optional[str],
+    limit: Optional[int],
+    time_span: Optional[str],
+    overwrite: Optional[bool],
+):
+    if not subject or not service_name:
+        raise AccessControlBadRequestError(
+            "请指定服务名（--service）与主体（--subject）"
+        )
+    elif not time_span:
+        raise AccessControlBadRequestError("请指定限制时间段（--span）")
+    elif not limit:
+        raise AccessControlBadRequestError("请指定限制次数（--limit）")
+    elif limit <= 0:
+        raise AccessControlBadRequestError("限制次数（--limit）必须大于0")
+
+    try:
+        parsed_time_span = pytimeparser.parse(time_span)
+    except ValueError:
+        raise AccessControlBadRequestError("给定的限制时间段（--span）不合法")
+
+    async with use_ac_session():
+        service = get_service_by_qualified_name(service_name)
+        if service is None:
+            raise AccessControlQueryError(f"找不到服务 {service_name}")
+
+        rule = await service.add_rate_limit_rule(
+            subject, parsed_time_span, limit, overwrite or False
+        )
+    _map_rule(f, rule, service_name)
+
+
+@require_superuser_or_script
+async def rm(
+    f: TextIO,
+    rule_id: Optional[str],
+):
+    if not rule_id:
+        raise AccessControlBadRequestError("请指定限流规则ID")
+
+    async with use_ac_session():
+        ok = await Service.remove_rate_limit_rule(rule_id)
+    if ok:
+        f.write("删除成功")
+    else:
+        raise AccessControlQueryError("删除失败，未找到该限流规则")
+
+
+@require_superuser_or_script
+async def ls(f: TextIO, service_name: Optional[str], subject: Optional[str]):
+    async with use_ac_session():
+        if not service_name and not subject:
+            rules = [x async for x in Service.get_all_rate_limit_rules()]
+        elif not service_name:
+            rules = [
+                x async for x in Service.get_all_rate_limit_rules_by_subject(subject)
+            ]
+        else:
+            service = get_service_by_qualified_name(
+                service_name, raise_on_not_exists=True
+            )
+
+            if not subject:
+                rules = [x async for x in service.get_rate_limit_rules()]
+            else:
+                rules = [
+                    x async for x in service.get_rate_limit_rules_by_subject(subject)
+                ]
+
+    if len(rules) != 0:
+        # 按照服务全称、subject排序
+        rules = sorted(rules, key=lambda x: (x.service.qualified_name, x.subject, x.id))
+
+        for rule in rules:
+            _map_rule(f, rule, service_name)
+            f.write("\n")
+    else:
+        f.write("无")
+
+
+@require_superuser_or_script
+async def reset(
+    f: TextIO,
+):
+    async with use_ac_session():
+        await Service.clear_rate_limit_tokens()
+    f.write("成功")
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/handler/subject_handler.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/subject_handler.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import TextIO
-
-from nonebot.internal.matcher import current_bot, current_event
-from nonebot_plugin_access_control_api.subject import extract_subjects
-from nonebot_plugin_access_control_api.errors import AccessControlBadRequestError
-
-from .utils.env import ac_get_env
-
-
-async def subject(f: TextIO):
-    if ac_get_env() != "nonebot":
-        raise AccessControlBadRequestError("该指令仅限聊天中使用")
-
-    bot = current_bot.get()
-    event = current_event.get()
-
-    for sbj in extract_subjects(bot, event):
-        f.write(sbj)
-        f.write("\n")
+from typing import TextIO
+
+from nonebot.internal.matcher import current_bot, current_event
+from nonebot_plugin_access_control_api.subject import extract_subjects
+from nonebot_plugin_access_control_api.errors import AccessControlBadRequestError
+
+from .utils.env import ac_get_env
+
+
+async def subject(f: TextIO):
+    if ac_get_env() != "nonebot":
+        raise AccessControlBadRequestError("该指令仅限聊天中使用")
+
+    bot = current_bot.get()
+    event = current_event.get()
+
+    for sbj in extract_subjects(bot, event):
+        f.write(sbj)
+        f.write("\n")
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/handler/utils/permission.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/handler/utils/permission.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from functools import wraps
-
-from nonebot.permission import SUPERUSER
-from nonebot.internal.matcher import current_bot, current_event
-from nonebot_plugin_access_control_api.errors import PermissionDeniedError
-
-from .env import ac_get_env
-
-
-def require_superuser_or_script(f):
-    @wraps(f)
-    async def wrapper(*args, **kwargs):
-        if ac_get_env() != "script":
-            if not await SUPERUSER(current_bot.get(), current_event.get()):
-                raise PermissionDeniedError()
-
-        return await f(*args, **kwargs)
-
-    return wrapper
+from functools import wraps
+
+from nonebot.permission import SUPERUSER
+from nonebot.internal.matcher import current_bot, current_event
+from nonebot_plugin_access_control_api.errors import PermissionDeniedError
+
+from .env import ac_get_env
+
+
+def require_superuser_or_script(f):
+    @wraps(f)
+    async def wrapper(*args, **kwargs):
+        if ac_get_env() != "script":
+            if not await SUPERUSER(current_bot.get(), current_event.get()):
+                raise PermissionDeniedError()
+
+        return await f(*args, **kwargs)
+
+    return wrapper
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/orm_migrations/96ced46e72e9_data_migrate.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/orm_migrations/96ced46e72e9_data_migrate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,151 +1,152 @@
-"""data_migrate
-
-修订 ID: 96ced46e72e9
-父修订: 9bb3231cf9aa
-创建时间: 2023-10-11 21:07:26.511220
-
-"""
-from __future__ import annotations
-
-from collections.abc import Sequence
-
-import sqlalchemy as sa
-from sqlalchemy import inspect
-from alembic.op import run_async
-from nonebot import logger, require
-from pkg_resources import DistributionNotFound, get_distribution
-from sqlalchemy.ext.asyncio import AsyncSession, AsyncConnection
-
-revision: str = "96ced46e72e9"
-down_revision: str | Sequence[str] | None = "9bb3231cf9aa"
-branch_labels: str | Sequence[str] | None = None
-depends_on: str | Sequence[str] | None = None
-
-
-async def data_migrate(conn: AsyncConnection):
-    require("nonebot_plugin_datastore")
-
-    from nonebot_plugin_datastore.db import get_engine
-
-    # nonebot_plugin_access_control_permission
-    async with AsyncConnection(get_engine()) as ds_conn:
-        async with AsyncSession(ds_conn) as ds_sess:
-            if not await ds_conn.run_sync(
-                lambda conn: inspect(conn).has_table(
-                    "nonebot_plugin_access_control_alembic_version"
-                )
-            ):
-                return
-
-            result = (
-                await ds_sess.execute(
-                    sa.text(
-                        "SELECT version_num "
-                        "FROM nonebot_plugin_access_control_alembic_version"
-                    )
-                )
-            ).scalar_one_or_none()
-            if result != "6fbda6d1d8ee":
-                raise RuntimeError(
-                    "请先执行 nb datastore upgrade "
-                    "--name nonebot_plugin_access_control "
-                    "将旧数据库迁移到最新版本"
-                )
-
-            result = await ds_sess.stream(
-                sa.text(
-                    "SELECT subject, service, allow "
-                    "FROM nonebot_plugin_access_control_permission;"
-                )
-            )
-            async for row in result:
-                subject, service, allow = row
-                await conn.execute(
-                    sa.text(
-                        "INSERT INTO accctrl_permission (subject, service, allow) "
-                        "VALUES (:subject, :service, :allow);"
-                    ),
-                    [{"subject": subject, "service": service, "allow": allow}],
-                )
-                logger.debug(
-                    f"从表 nonebot_plugin_access_control_permission 迁移数据："
-                    f"subject={subject} service={service} allow={allow}"
-                )
-
-            # nonebot_plugin_access_control_rate_limit_rule
-            result = await ds_sess.stream(
-                sa.text(
-                    "SELECT id, subject, service, time_span, \"limit\", overwrite "
-                    "FROM nonebot_plugin_access_control_rate_limit_rule;"
-                )
-            )
-            async for row in result:
-                id, subject, service, time_span, limit, overwrite = row
-                await conn.execute(
-                    sa.text(
-                        "INSERT INTO accctrl_rate_limit_rule (id, subject, service, time_span, \"limit\", overwrite) "
-                        "VALUES (:id, :subject, :service, :time_span, :limit, :overwrite);"
-                    ),
-                    [
-                        {
-                            "id": id,
-                            "subject": subject,
-                            "service": service,
-                            "time_span": time_span,
-                            "limit": limit,
-                            "overwrite": overwrite,
-                        }
-                    ],
-                )
-                logger.debug(
-                    f"从表 nonebot_plugin_access_control_rate_limit_rule 迁移数据："
-                    f"id={id} subject={subject} service={service} "
-                    f"time_span={time_span} limit={limit} overwrite={overwrite}"
-                )
-
-            # nonebot_plugin_access_control_rate_limit_token
-            result = await ds_sess.stream(
-                sa.text(
-                    "SELECT id, rule_id, \"user\", acquire_time, expire_time "
-                    "FROM nonebot_plugin_access_control_rate_limit_token;"
-                )
-            )
-            async for row in result:
-                id, rule_id, user, acquire_time, expire_time = row
-                await conn.execute(
-                    sa.text(
-                        "INSERT INTO accctrl_rate_limit_rule (id, rule_id, \"user\", acquire_time, expire_time) "
-                        "VALUES (:id, :rule_id, :user, :acquire_time, :expire_time);"
-                    ),
-                    [
-                        {
-                            "id": id,
-                            "rule_id": rule_id,
-                            "user": user,
-                            "acquire_time": acquire_time,
-                            "expire_time": expire_time,
-                        }
-                    ],
-                )
-                logger.debug(
-                    f"从表 nonebot_plugin_access_control_rate_limit_token 迁移数据："
-                    f"id={id} rule_id={rule_id} user={user} "
-                    f"acquire_time={acquire_time} expire_time={expire_time}"
-                )
-
-
-def upgrade(name: str = "") -> None:
-    if name:
-        return
-    try:
-        get_distribution("nonebot_plugin_datastore")
-    except DistributionNotFound:
-        return
-
-    logger.info("正在从 datastore 迁移数据……")
-    run_async(data_migrate)
-
-
-def downgrade(name: str = "") -> None:
-    # do nothing
-    pass
+"""data_migrate
+
+修订 ID: 96ced46e72e9
+父修订: 9bb3231cf9aa
+创建时间: 2023-10-11 21:07:26.511220
+
+"""
+
+from __future__ import annotations
+
+from collections.abc import Sequence
+
+import sqlalchemy as sa
+from sqlalchemy import inspect
+from alembic.op import run_async
+from nonebot import logger, require
+from pkg_resources import DistributionNotFound, get_distribution
+from sqlalchemy.ext.asyncio import AsyncSession, AsyncConnection
+
+revision: str = "96ced46e72e9"
+down_revision: str | Sequence[str] | None = "9bb3231cf9aa"
+branch_labels: str | Sequence[str] | None = None
+depends_on: str | Sequence[str] | None = None
+
+
+async def data_migrate(conn: AsyncConnection):
+    require("nonebot_plugin_datastore")
+
+    from nonebot_plugin_datastore.db import get_engine
+
+    # nonebot_plugin_access_control_permission
+    async with AsyncConnection(get_engine()) as ds_conn:
+        async with AsyncSession(ds_conn) as ds_sess:
+            if not await ds_conn.run_sync(
+                lambda conn: inspect(conn).has_table(
+                    "nonebot_plugin_access_control_alembic_version"
+                )
+            ):
+                return
+
+            result = (
+                await ds_sess.execute(
+                    sa.text(
+                        "SELECT version_num "
+                        "FROM nonebot_plugin_access_control_alembic_version"
+                    )
+                )
+            ).scalar_one_or_none()
+            if result != "6fbda6d1d8ee":
+                raise RuntimeError(
+                    "请先执行 nb datastore upgrade "
+                    "--name nonebot_plugin_access_control "
+                    "将旧数据库迁移到最新版本"
+                )
+
+            result = await ds_sess.stream(
+                sa.text(
+                    "SELECT subject, service, allow "
+                    "FROM nonebot_plugin_access_control_permission;"
+                )
+            )
+            async for row in result:
+                subject, service, allow = row
+                await conn.execute(
+                    sa.text(
+                        "INSERT INTO accctrl_permission (subject, service, allow) "
+                        "VALUES (:subject, :service, :allow);"
+                    ),
+                    [{"subject": subject, "service": service, "allow": allow}],
+                )
+                logger.debug(
+                    f"从表 nonebot_plugin_access_control_permission 迁移数据："
+                    f"subject={subject} service={service} allow={allow}"
+                )
+
+            # nonebot_plugin_access_control_rate_limit_rule
+            result = await ds_sess.stream(
+                sa.text(
+                    'SELECT id, subject, service, time_span, "limit", overwrite '
+                    "FROM nonebot_plugin_access_control_rate_limit_rule;"
+                )
+            )
+            async for row in result:
+                id, subject, service, time_span, limit, overwrite = row
+                await conn.execute(
+                    sa.text(
+                        'INSERT INTO accctrl_rate_limit_rule (id, subject, service, time_span, "limit", overwrite) '
+                        "VALUES (:id, :subject, :service, :time_span, :limit, :overwrite);"
+                    ),
+                    [
+                        {
+                            "id": id,
+                            "subject": subject,
+                            "service": service,
+                            "time_span": time_span,
+                            "limit": limit,
+                            "overwrite": overwrite,
+                        }
+                    ],
+                )
+                logger.debug(
+                    f"从表 nonebot_plugin_access_control_rate_limit_rule 迁移数据："
+                    f"id={id} subject={subject} service={service} "
+                    f"time_span={time_span} limit={limit} overwrite={overwrite}"
+                )
+
+            # nonebot_plugin_access_control_rate_limit_token
+            result = await ds_sess.stream(
+                sa.text(
+                    'SELECT id, rule_id, "user", acquire_time, expire_time '
+                    "FROM nonebot_plugin_access_control_rate_limit_token;"
+                )
+            )
+            async for row in result:
+                id, rule_id, user, acquire_time, expire_time = row
+                await conn.execute(
+                    sa.text(
+                        'INSERT INTO accctrl_rate_limit_rule (id, rule_id, "user", acquire_time, expire_time) '
+                        "VALUES (:id, :rule_id, :user, :acquire_time, :expire_time);"
+                    ),
+                    [
+                        {
+                            "id": id,
+                            "rule_id": rule_id,
+                            "user": user,
+                            "acquire_time": acquire_time,
+                            "expire_time": expire_time,
+                        }
+                    ],
+                )
+                logger.debug(
+                    f"从表 nonebot_plugin_access_control_rate_limit_token 迁移数据："
+                    f"id={id} rule_id={rule_id} user={user} "
+                    f"acquire_time={acquire_time} expire_time={expire_time}"
+                )
+
+
+def upgrade(name: str = "") -> None:
+    if name:
+        return
+    try:
+        get_distribution("nonebot_plugin_datastore")
+    except DistributionNotFound:
+        return
+
+    logger.info("正在从 datastore 迁移数据……")
+    run_async(data_migrate)
+
+
+def downgrade(name: str = "") -> None:
+    # do nothing
+    pass
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/orm/rate_limit.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/orm/rate_limit.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from datetime import datetime
-
-from shortuuid import ShortUUID
-from nonebot_plugin_orm import Model
-from sqlalchemy import Index, ForeignKey
-from sqlalchemy.orm import Mapped, MappedAsDataclass, relationship, mapped_column
-
-_shortuuid = ShortUUID(alphabet="23456789abcdefghijkmnopqrstuvwxyz")
-
-
-def _gen_id():
-    return _shortuuid.random(length=5)
-
-
-class RateLimitRuleOrm(MappedAsDataclass, Model):
-    __tablename__ = "accctrl_rate_limit_rule"
-    __table_args__ = (
-        Index("ix_accctrl_rate_limit_rule_subject_service", "subject", "service"),
-        {"extend_existing": True},
-    )
-
-    id: Mapped[str] = mapped_column(
-        init=False, primary_key=True, default_factory=_gen_id
-    )
-    subject: Mapped[str]
-    service: Mapped[str]
-    time_span: Mapped[int]  # 单位：秒
-    limit: Mapped[int]
-    overwrite: Mapped[bool]
-
-    tokens: Mapped[list["RateLimitTokenOrm"]] = relationship(
-        init=False, back_populates="rule", cascade="delete"
-    )
-
-
-class RateLimitTokenOrm(MappedAsDataclass, Model):
-    __tablename__ = "accctrl_rate_limit_token"
-    __table_args__ = (
-        Index("ix_accctrl_rate_limit_token_rule_id", "rule_id"),
-        Index("ix_accctrl_rate_limit_token_expire_time", "expire_time"),
-        {"extend_existing": True},
-    )
-
-    id: Mapped[int] = mapped_column(init=False, primary_key=True)
-    rule_id: Mapped[str] = mapped_column(ForeignKey("accctrl_rate_limit_rule.id"))
-    user: Mapped[str]
-    acquire_time: Mapped[datetime] = mapped_column()
-    expire_time: Mapped[datetime] = mapped_column()
-
-    rule: Mapped[RateLimitRuleOrm] = relationship(init=False, back_populates="tokens")
+from datetime import datetime
+
+from shortuuid import ShortUUID
+from nonebot_plugin_orm import Model
+from sqlalchemy import Index, ForeignKey
+from sqlalchemy.orm import Mapped, MappedAsDataclass, relationship, mapped_column
+
+_shortuuid = ShortUUID(alphabet="23456789abcdefghijkmnopqrstuvwxyz")
+
+
+def _gen_id():
+    return _shortuuid.random(length=5)
+
+
+class RateLimitRuleOrm(MappedAsDataclass, Model):
+    __tablename__ = "accctrl_rate_limit_rule"
+    __table_args__ = (
+        Index("ix_accctrl_rate_limit_rule_subject_service", "subject", "service"),
+        {"extend_existing": True},
+    )
+
+    id: Mapped[str] = mapped_column(
+        init=False, primary_key=True, default_factory=_gen_id
+    )
+    subject: Mapped[str]
+    service: Mapped[str]
+    time_span: Mapped[int]  # 单位：秒
+    limit: Mapped[int]
+    overwrite: Mapped[bool]
+
+    tokens: Mapped[list["RateLimitTokenOrm"]] = relationship(
+        init=False, back_populates="rule", cascade="delete"
+    )
+
+
+class RateLimitTokenOrm(MappedAsDataclass, Model):
+    __tablename__ = "accctrl_rate_limit_token"
+    __table_args__ = (
+        Index("ix_accctrl_rate_limit_token_rule_id", "rule_id"),
+        Index("ix_accctrl_rate_limit_token_expire_time", "expire_time"),
+        {"extend_existing": True},
+    )
+
+    id: Mapped[int] = mapped_column(init=False, primary_key=True)
+    rule_id: Mapped[str] = mapped_column(ForeignKey("accctrl_rate_limit_rule.id"))
+    user: Mapped[str]
+    acquire_time: Mapped[datetime] = mapped_column()
+    expire_time: Mapped[datetime] = mapped_column()
+
+    rule: Mapped[RateLimitRuleOrm] = relationship(init=False, back_populates="tokens")
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/permission/impl.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/permission/impl.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from typing import Optional
-from collections.abc import AsyncGenerator
-
-from sqlalchemy import select
-from nonebot_plugin_access_control_api.context import context
-from nonebot_plugin_access_control_api.service.interface import IService
-from nonebot_plugin_access_control_api.models.permission import Permission
-from nonebot_plugin_access_control_api.service.interface.nonebot_service import (
-    INoneBotService,
-)
-
-from ..utils import use_ac_session
-from ..orm.permission import PermissionOrm
-from .interface import IPermissionRepository
-
-
-@context.bind_singleton_to(IPermissionRepository)
-class PermissionRepository(IPermissionRepository):
-    async def get_permissions(
-        self, service: Optional[IService], subject: Optional[str]
-    ) -> AsyncGenerator[Permission, None]:
-        async with use_ac_session() as session:
-            stmt = select(PermissionOrm)
-            if service is not None:
-                stmt = stmt.where(PermissionOrm.service == service.qualified_name)
-            if subject is not None:
-                stmt = stmt.where(PermissionOrm.subject == subject)
-
-            async for x in await session.stream_scalars(stmt):
-                s = service
-                if s is None:
-                    s = context.require(INoneBotService).get_service_by_qualified_name(
-                        x.service
-                    )
-                if s is not None:
-                    yield Permission(s, x.subject, x.allow)
-
-    async def set_permission(
-        self, service: Optional[IService], subject: str, allow: bool
-    ) -> bool:
-        async with use_ac_session() as sess:
-            stmt = select(PermissionOrm).where(
-                PermissionOrm.service == service.qualified_name,
-                PermissionOrm.subject == subject,
-            )
-            p = (await sess.execute(stmt)).scalar_one_or_none()
-            if p is None:
-                p = PermissionOrm(
-                    service=service.qualified_name, subject=subject, allow=allow
-                )
-                sess.add(p)
-                old_allow = None
-            else:
-                old_allow = p.allow
-                p.allow = allow
-
-            if old_allow != allow:
-                await sess.commit()
-                return True
-            else:
-                return False
-
-    async def remove_permission(
-        self, service: Optional[IService], subject: str
-    ) -> bool:
-        async with use_ac_session() as sess:
-            stmt = select(PermissionOrm).where(
-                PermissionOrm.service == service.qualified_name,
-                PermissionOrm.subject == subject,
-            )
-            p = (await sess.execute(stmt)).scalar_one_or_none()
-            if p is None:
-                return False
-
-            await sess.delete(p)
-            await sess.commit()
-            return True
+from typing import Optional
+from collections.abc import AsyncGenerator
+
+from sqlalchemy import select
+from nonebot_plugin_access_control_api.context import context
+from nonebot_plugin_access_control_api.service.interface import IService
+from nonebot_plugin_access_control_api.models.permission import Permission
+from nonebot_plugin_access_control_api.service.interface.nonebot_service import (
+    INoneBotService,
+)
+
+from ..utils import use_ac_session
+from ..orm.permission import PermissionOrm
+from .interface import IPermissionRepository
+
+
+@context.bind_singleton_to(IPermissionRepository)
+class PermissionRepository(IPermissionRepository):
+    async def get_permissions(
+        self, service: Optional[IService], subject: Optional[str]
+    ) -> AsyncGenerator[Permission, None]:
+        async with use_ac_session() as session:
+            stmt = select(PermissionOrm)
+            if service is not None:
+                stmt = stmt.where(PermissionOrm.service == service.qualified_name)
+            if subject is not None:
+                stmt = stmt.where(PermissionOrm.subject == subject)
+
+            async for x in await session.stream_scalars(stmt):
+                s = service
+                if s is None:
+                    s = context.require(INoneBotService).get_service_by_qualified_name(
+                        x.service
+                    )
+                if s is not None:
+                    yield Permission(s, x.subject, x.allow)
+
+    async def set_permission(
+        self, service: Optional[IService], subject: str, allow: bool
+    ) -> bool:
+        async with use_ac_session() as sess:
+            stmt = select(PermissionOrm).where(
+                PermissionOrm.service == service.qualified_name,
+                PermissionOrm.subject == subject,
+            )
+            p = (await sess.execute(stmt)).scalar_one_or_none()
+            if p is None:
+                p = PermissionOrm(
+                    service=service.qualified_name, subject=subject, allow=allow
+                )
+                sess.add(p)
+                old_allow = None
+            else:
+                old_allow = p.allow
+                p.allow = allow
+
+            if old_allow != allow:
+                await sess.commit()
+                return True
+            else:
+                return False
+
+    async def remove_permission(
+        self, service: Optional[IService], subject: str
+    ) -> bool:
+        async with use_ac_session() as sess:
+            stmt = select(PermissionOrm).where(
+                PermissionOrm.service == service.qualified_name,
+                PermissionOrm.subject == subject,
+            )
+            p = (await sess.execute(stmt)).scalar_one_or_none()
+            if p is None:
+                return False
+
+            await sess.delete(p)
+            await sess.commit()
+            return True
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/permission/interface.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/permission/interface.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Optional, Protocol
-from collections.abc import AsyncGenerator
-
-from nonebot_plugin_access_control_api.service.interface import IService
-from nonebot_plugin_access_control_api.models.permission import Permission
-
-
-class IPermissionRepository(Protocol):
-    async def get_permissions(
-        self, service: Optional[IService], subject: Optional[str]
-    ) -> AsyncGenerator[Permission, None]:
-        raise NotImplementedError()
-        yield Permission()  # noqa
-
-    async def set_permission(
-        self, service: Optional[IService], subject: str, allow: bool
-    ) -> bool:
-        raise NotImplementedError()
-
-    async def remove_permission(
-        self, service: Optional[IService], subject: str
-    ) -> bool:
-        raise NotImplementedError()
+from typing import Optional, Protocol
+from collections.abc import AsyncGenerator
+
+from nonebot_plugin_access_control_api.service.interface import IService
+from nonebot_plugin_access_control_api.models.permission import Permission
+
+
+class IPermissionRepository(Protocol):
+    async def get_permissions(
+        self, service: Optional[IService], subject: Optional[str]
+    ) -> AsyncGenerator[Permission, None]:
+        raise NotImplementedError()
+        yield Permission()  # noqa
+
+    async def set_permission(
+        self, service: Optional[IService], subject: str, allow: bool
+    ) -> bool:
+        raise NotImplementedError()
+
+    async def remove_permission(
+        self, service: Optional[IService], subject: str
+    ) -> bool:
+        raise NotImplementedError()
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/rate_limit/impl.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/rate_limit/impl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,106 @@
-from typing import Optional
-from datetime import timedelta
-from collections.abc import AsyncGenerator
-
-from sqlalchemy import func, select
-from nonebot_plugin_access_control_api.context import context
-from nonebot_plugin_access_control_api.service.interface import IService
-from nonebot_plugin_access_control_api.errors import AccessControlQueryError
-from nonebot_plugin_access_control_api.models.rate_limit import RateLimitRule
-from nonebot_plugin_access_control_api.service.interface.nonebot_service import (
-    INoneBotService,
-)
-
-from ..utils import use_ac_session
-from .interface import IRateLimitRepository
-from ..orm.rate_limit import RateLimitRuleOrm
-
-
-@context.bind_singleton_to(IRateLimitRepository)
-class RateLimitRepository(IRateLimitRepository):
-    async def get_rules_by_subject(
-        self, service: Optional[IService], subject: Optional[str]
-    ) -> AsyncGenerator[RateLimitRuleOrm, None]:
-        async with use_ac_session() as session:
-            stmt = select(RateLimitRuleOrm)
-            if service is not None:
-                stmt = stmt.where(RateLimitRuleOrm.service == service.qualified_name)
-            if subject is not None:
-                stmt = stmt.where(RateLimitRuleOrm.subject == subject)
-
-            async for x in await session.stream_scalars(stmt):
-                s = service
-                if s is None:
-                    s = context.require(INoneBotService).get_service_by_qualified_name(
-                        x.service
-                    )
-                if s is not None:
-                    yield RateLimitRule(
-                        x.id,
-                        s,
-                        x.subject,
-                        timedelta(seconds=x.time_span),
-                        x.limit,
-                        x.overwrite,
-                    )
-
-    async def add_rate_limit_rule(
-        self,
-        service: IService,
-        subject: str,
-        time_span: timedelta,
-        limit: int,
-        overwrite: bool = False,
-    ) -> RateLimitRule:
-        async with use_ac_session() as sess:
-            if overwrite:
-                stmt = select(func.count()).where(
-                    RateLimitRuleOrm.subject == subject,
-                    RateLimitRuleOrm.service == service.qualified_name,
-                )
-                cnt = (await sess.execute(stmt)).scalar_one()
-
-                if cnt > 0:
-                    raise AccessControlQueryError("已存在对该实体与服务的限流规则，不允许再添加覆写规则")
-
-            orm = RateLimitRuleOrm(
-                subject=subject,
-                service=service.qualified_name,
-                time_span=int(time_span.total_seconds()),
-                limit=limit,
-                overwrite=overwrite,
-            )
-            sess.add(orm)
-            await sess.commit()
-
-            await sess.refresh(orm)
-
-            rule = RateLimitRule(orm.id, service, subject, time_span, limit, overwrite)
-
-            return rule
-
-    async def remove_rate_limit_rule(self, rule_id: str) -> Optional[RateLimitRule]:
-        async with use_ac_session() as sess:
-            orm = await sess.get(RateLimitRuleOrm, rule_id)
-            if orm is None:
-                return None
-
-            await sess.delete(orm)
-            await sess.commit()
-
-            service = context.require(INoneBotService).get_service_by_qualified_name(
-                orm.service
-            )
-
-            rule = RateLimitRule(
-                orm.id,
-                service,
-                orm.subject,
-                timedelta(seconds=orm.time_span),
-                orm.limit,
-                orm.overwrite,
-            )
-
-            return rule
+from typing import Optional
+from datetime import timedelta
+from collections.abc import AsyncGenerator
+
+from sqlalchemy import func, select
+from nonebot_plugin_access_control_api.context import context
+from nonebot_plugin_access_control_api.service.interface import IService
+from nonebot_plugin_access_control_api.errors import AccessControlQueryError
+from nonebot_plugin_access_control_api.models.rate_limit import RateLimitRule
+from nonebot_plugin_access_control_api.service.interface.nonebot_service import (
+    INoneBotService,
+)
+
+from ..utils import use_ac_session
+from .interface import IRateLimitRepository
+from ..orm.rate_limit import RateLimitRuleOrm
+
+
+@context.bind_singleton_to(IRateLimitRepository)
+class RateLimitRepository(IRateLimitRepository):
+    async def get_rules_by_subject(
+        self, service: Optional[IService], subject: Optional[str]
+    ) -> AsyncGenerator[RateLimitRuleOrm, None]:
+        async with use_ac_session() as session:
+            stmt = select(RateLimitRuleOrm)
+            if service is not None:
+                stmt = stmt.where(RateLimitRuleOrm.service == service.qualified_name)
+            if subject is not None:
+                stmt = stmt.where(RateLimitRuleOrm.subject == subject)
+
+            async for x in await session.stream_scalars(stmt):
+                s = service
+                if s is None:
+                    s = context.require(INoneBotService).get_service_by_qualified_name(
+                        x.service
+                    )
+                if s is not None:
+                    yield RateLimitRule(
+                        x.id,
+                        s,
+                        x.subject,
+                        timedelta(seconds=x.time_span),
+                        x.limit,
+                        x.overwrite,
+                    )
+
+    async def add_rate_limit_rule(
+        self,
+        service: IService,
+        subject: str,
+        time_span: timedelta,
+        limit: int,
+        overwrite: bool = False,
+    ) -> RateLimitRule:
+        async with use_ac_session() as sess:
+            if overwrite:
+                stmt = select(func.count()).where(
+                    RateLimitRuleOrm.subject == subject,
+                    RateLimitRuleOrm.service == service.qualified_name,
+                )
+                cnt = (await sess.execute(stmt)).scalar_one()
+
+                if cnt > 0:
+                    raise AccessControlQueryError(
+                        "已存在对该实体与服务的限流规则，不允许再添加覆写规则"
+                    )
+
+            orm = RateLimitRuleOrm(
+                subject=subject,
+                service=service.qualified_name,
+                time_span=int(time_span.total_seconds()),
+                limit=limit,
+                overwrite=overwrite,
+            )
+            sess.add(orm)
+            await sess.commit()
+
+            await sess.refresh(orm)
+
+            rule = RateLimitRule(orm.id, service, subject, time_span, limit, overwrite)
+
+            return rule
+
+    async def remove_rate_limit_rule(self, rule_id: str) -> Optional[RateLimitRule]:
+        async with use_ac_session() as sess:
+            orm = await sess.get(RateLimitRuleOrm, rule_id)
+            if orm is None:
+                return None
+
+            await sess.delete(orm)
+            await sess.commit()
+
+            service = context.require(INoneBotService).get_service_by_qualified_name(
+                orm.service
+            )
+
+            rule = RateLimitRule(
+                orm.id,
+                service,
+                orm.subject,
+                timedelta(seconds=orm.time_span),
+                orm.limit,
+                orm.overwrite,
+            )
+
+            return rule
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/rate_limit/interface.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/rate_limit/interface.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from datetime import timedelta
-from typing import Optional, Protocol
-from collections.abc import AsyncGenerator
-
-from nonebot_plugin_access_control_api.service.interface import IService
-from nonebot_plugin_access_control_api.models.rate_limit import RateLimitRule
-
-from ..orm.rate_limit import RateLimitRuleOrm
-
-
-class IRateLimitRepository(Protocol):
-    async def get_rules_by_subject(
-        self, service: Optional[IService], subject: Optional[str]
-    ) -> AsyncGenerator[RateLimitRuleOrm, None]:
-        raise NotImplementedError()
-        yield RateLimitRuleOrm()  # noqa
-
-    async def add_rate_limit_rule(
-        self,
-        service: IService,
-        subject: str,
-        time_span: timedelta,
-        limit: int,
-        overwrite: bool = False,
-    ) -> RateLimitRule:
-        raise NotImplementedError()
-
-    async def remove_rate_limit_rule(self, rule_id: str) -> Optional[RateLimitRule]:
-        raise NotImplementedError()
+from datetime import timedelta
+from typing import Optional, Protocol
+from collections.abc import AsyncGenerator
+
+from nonebot_plugin_access_control_api.service.interface import IService
+from nonebot_plugin_access_control_api.models.rate_limit import RateLimitRule
+
+from ..orm.rate_limit import RateLimitRuleOrm
+
+
+class IRateLimitRepository(Protocol):
+    async def get_rules_by_subject(
+        self, service: Optional[IService], subject: Optional[str]
+    ) -> AsyncGenerator[RateLimitRuleOrm, None]:
+        raise NotImplementedError()
+        yield RateLimitRuleOrm()  # noqa
+
+    async def add_rate_limit_rule(
+        self,
+        service: IService,
+        subject: str,
+        time_span: timedelta,
+        limit: int,
+        overwrite: bool = False,
+    ) -> RateLimitRule:
+        raise NotImplementedError()
+
+    async def remove_rate_limit_rule(self, rule_id: str) -> Optional[RateLimitRule]:
+        raise NotImplementedError()
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/rate_limit_token/__init__.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/rate_limit_token/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from nonebot import logger
-
-from ...config import conf
-from .interface import IRateLimitTokenRepository
-
-if conf().access_control_rate_limit_token_storage == "datastore":
-    from . import datastore  # noqa
-
-    logger.opt(colors=True).info("use <y>datastore</y> rate_limit_token storage")
-elif conf().access_control_rate_limit_token_storage == "inmemory":
-    from . import inmemory  # noqa
-
-    logger.opt(colors=True).info("use <y>inmemory</y> rate_limit_token storage")
-else:
-    raise RuntimeError(
-        f"invalid access_control_rate_limit_token_storage: "
-        f"{conf().access_control_rate_limit_token_storage}"
-    )
-
-__all__ = ("IRateLimitTokenRepository",)
+from nonebot import logger
+
+from ...config import conf
+from .interface import IRateLimitTokenRepository
+
+if conf().access_control_rate_limit_token_storage == "datastore":
+    from . import datastore  # noqa
+
+    logger.opt(colors=True).info("use <y>datastore</y> rate_limit_token storage")
+elif conf().access_control_rate_limit_token_storage == "inmemory":
+    from . import inmemory  # noqa
+
+    logger.opt(colors=True).info("use <y>inmemory</y> rate_limit_token storage")
+else:
+    raise RuntimeError(
+        f"invalid access_control_rate_limit_token_storage: "
+        f"{conf().access_control_rate_limit_token_storage}"
+    )
+
+__all__ = ("IRateLimitTokenRepository",)
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/rate_limit_token/datastore.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/rate_limit_token/datastore.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-from nonebot import require
-from nonebot_plugin_access_control_api.context import context
-
-require("nonebot_plugin_apscheduler")
-
-from typing import Optional
-from datetime import datetime
-
-from loguru import logger
-from sqlalchemy import func, delete, select
-from nonebot_plugin_apscheduler import scheduler
-from apscheduler.triggers.interval import IntervalTrigger
-from nonebot_plugin_access_control_api.models.rate_limit import (
-    RateLimitRule,
-    RateLimitSingleToken,
-)
-
-from ..utils import use_ac_session
-from .interface import IRateLimitTokenRepository
-from ..orm.rate_limit import RateLimitRuleOrm, RateLimitTokenOrm
-
-
-@context.bind_singleton_to(IRateLimitTokenRepository)
-class DataStoreTokenRepository(IRateLimitTokenRepository):
-    def __init__(self):
-        scheduler.add_job(
-            self.delete_outdated_tokens,
-            IntervalTrigger(minutes=1),
-            id="delete_outdated_tokens_inmemory",
-        )
-
-    async def get_first_expire_token(
-        self, rule: RateLimitRule, user: str
-    ) -> Optional[RateLimitSingleToken]:
-        now = datetime.utcnow()
-
-        async with use_ac_session() as sess:
-            stmt = (
-                select(func.min(RateLimitTokenOrm.expire_time))
-                .select_from(RateLimitTokenOrm)
-                .where(RateLimitTokenOrm.expire_time > now)
-                .scalar_subquery()
-            )
-            stmt = (
-                select(RateLimitTokenOrm)
-                .where(RateLimitTokenOrm.expire_time == stmt)
-                .limit(1)
-            )
-            res = (await sess.execute(stmt)).scalar_one_or_none()
-
-            if res is None:
-                return None
-            else:
-                return RateLimitSingleToken(
-                    res.id,
-                    res.rule_id,
-                    res.user,
-                    res.acquire_time,
-                    res.acquire_time + rule.time_span,
-                )
-
-    async def acquire_token(
-        self, rule: RateLimitRule, user: str
-    ) -> Optional[RateLimitSingleToken]:
-        now = datetime.utcnow()
-
-        async with use_ac_session() as sess:
-            stmt = select(func.count()).where(
-                RateLimitTokenOrm.rule_id == rule.id,
-                RateLimitTokenOrm.user == user,
-                RateLimitTokenOrm.expire_time > now,
-            )
-            cnt = (await sess.execute(stmt)).scalar_one()
-
-            if cnt >= rule.limit:
-                return None
-
-            acquire_time = datetime.utcnow()
-            expire_time = acquire_time + rule.time_span
-
-            x = RateLimitTokenOrm(
-                rule_id=rule.id,
-                user=user,
-                acquire_time=acquire_time,
-                expire_time=expire_time,
-            )
-            sess.add(x)
-            await sess.commit()
-
-            await sess.refresh(x)
-
-            return RateLimitSingleToken(
-                x.id, x.rule_id, x.user, acquire_time, expire_time
-            )
-
-    async def retire_token(self, token: RateLimitSingleToken):
-        async with use_ac_session() as sess:
-            stmt = delete(RateLimitTokenOrm).where(RateLimitTokenOrm.id == token.id)
-            await sess.execute(stmt)
-            await sess.commit()
-
-    async def delete_outdated_tokens(self):
-        async with use_ac_session() as session:
-            now = datetime.utcnow()
-            stmts = []
-            async for rule in await session.stream_scalars(select(RateLimitRuleOrm)):
-                stmt = (
-                    delete(RateLimitTokenOrm)
-                    .where(
-                        RateLimitTokenOrm.rule_id == rule.id,
-                        RateLimitTokenOrm.expire_time <= now,
-                    )
-                    .execution_options(synchronize_session=False)
-                )
-                stmts.append(stmt)
-
-            rowcount = 0
-            for stmt in stmts:
-                result = await session.execute(stmt)
-                rowcount += result.rowcount
-
-            await session.commit()
-
-            logger.debug(f"deleted {rowcount} outdated rate limit token(s)")
-
-    async def clear_token(self):
-        async with use_ac_session() as sess:
-            stmt = delete(RateLimitTokenOrm)
-            result = await sess.execute(stmt)
-            await sess.commit()
-            logger.debug(f"deleted {result.rowcount} rate limit token(s)")
+from nonebot import require
+from nonebot_plugin_access_control_api.context import context
+
+require("nonebot_plugin_apscheduler")
+
+from typing import Optional
+from datetime import datetime
+
+from loguru import logger
+from sqlalchemy import func, delete, select
+from nonebot_plugin_apscheduler import scheduler
+from apscheduler.triggers.interval import IntervalTrigger
+from nonebot_plugin_access_control_api.models.rate_limit import (
+    RateLimitRule,
+    RateLimitSingleToken,
+)
+
+from ..utils import use_ac_session
+from .interface import IRateLimitTokenRepository
+from ..orm.rate_limit import RateLimitRuleOrm, RateLimitTokenOrm
+
+
+@context.bind_singleton_to(IRateLimitTokenRepository)
+class DataStoreTokenRepository(IRateLimitTokenRepository):
+    def __init__(self):
+        scheduler.add_job(
+            self.delete_outdated_tokens,
+            IntervalTrigger(minutes=1),
+            id="delete_outdated_tokens_inmemory",
+        )
+
+    async def get_first_expire_token(
+        self, rule: RateLimitRule, user: str
+    ) -> Optional[RateLimitSingleToken]:
+        now = datetime.utcnow()
+
+        async with use_ac_session() as sess:
+            stmt = (
+                select(func.min(RateLimitTokenOrm.expire_time))
+                .select_from(RateLimitTokenOrm)
+                .where(RateLimitTokenOrm.expire_time > now)
+                .scalar_subquery()
+            )
+            stmt = (
+                select(RateLimitTokenOrm)
+                .where(RateLimitTokenOrm.expire_time == stmt)
+                .limit(1)
+            )
+            res = (await sess.execute(stmt)).scalar_one_or_none()
+
+            if res is None:
+                return None
+            else:
+                return RateLimitSingleToken(
+                    res.id,
+                    res.rule_id,
+                    res.user,
+                    res.acquire_time,
+                    res.acquire_time + rule.time_span,
+                )
+
+    async def acquire_token(
+        self, rule: RateLimitRule, user: str
+    ) -> Optional[RateLimitSingleToken]:
+        now = datetime.utcnow()
+
+        async with use_ac_session() as sess:
+            stmt = select(func.count()).where(
+                RateLimitTokenOrm.rule_id == rule.id,
+                RateLimitTokenOrm.user == user,
+                RateLimitTokenOrm.expire_time > now,
+            )
+            cnt = (await sess.execute(stmt)).scalar_one()
+
+            if cnt >= rule.limit:
+                return None
+
+            acquire_time = datetime.utcnow()
+            expire_time = acquire_time + rule.time_span
+
+            x = RateLimitTokenOrm(
+                rule_id=rule.id,
+                user=user,
+                acquire_time=acquire_time,
+                expire_time=expire_time,
+            )
+            sess.add(x)
+            await sess.commit()
+
+            await sess.refresh(x)
+
+            return RateLimitSingleToken(
+                x.id, x.rule_id, x.user, acquire_time, expire_time
+            )
+
+    async def retire_token(self, token: RateLimitSingleToken):
+        async with use_ac_session() as sess:
+            stmt = delete(RateLimitTokenOrm).where(RateLimitTokenOrm.id == token.id)
+            await sess.execute(stmt)
+            await sess.commit()
+
+    async def delete_outdated_tokens(self):
+        async with use_ac_session() as session:
+            now = datetime.utcnow()
+            stmts = []
+            async for rule in await session.stream_scalars(select(RateLimitRuleOrm)):
+                stmt = (
+                    delete(RateLimitTokenOrm)
+                    .where(
+                        RateLimitTokenOrm.rule_id == rule.id,
+                        RateLimitTokenOrm.expire_time <= now,
+                    )
+                    .execution_options(synchronize_session=False)
+                )
+                stmts.append(stmt)
+
+            rowcount = 0
+            for stmt in stmts:
+                result = await session.execute(stmt)
+                rowcount += result.rowcount
+
+            await session.commit()
+
+            logger.debug(f"deleted {rowcount} outdated rate limit token(s)")
+
+    async def clear_token(self):
+        async with use_ac_session() as sess:
+            stmt = delete(RateLimitTokenOrm)
+            result = await sess.execute(stmt)
+            await sess.commit()
+            logger.debug(f"deleted {result.rowcount} rate limit token(s)")
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/rate_limit_token/inmemory.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/rate_limit_token/inmemory.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from nonebot import require
-from nonebot_plugin_access_control_api.context import context
-
-require("nonebot_plugin_apscheduler")
-
-from datetime import datetime
-from typing import Optional, NamedTuple
-
-from nonebot_plugin_apscheduler import scheduler
-from apscheduler.triggers.interval import IntervalTrigger
-from nonebot_plugin_access_control_api.models.rate_limit import (
-    RateLimitRule,
-    RateLimitSingleToken,
-)
-
-from .interface import IRateLimitTokenRepository
-
-
-class StorageKey(NamedTuple):
-    rule_id: str
-    user: str
-
-
-def _handle_expired(
-    tokens: tuple[RateLimitSingleToken, ...]
-) -> tuple[RateLimitSingleToken, ...]:
-    now = datetime.utcnow()
-    return tuple(filter(lambda x: x.expire_time > now, tokens))
-
-
-@context.bind_singleton_to(IRateLimitTokenRepository)
-class InmemoryTokenRepository(IRateLimitTokenRepository):
-    def __init__(self):
-        self.id_cnt = 0
-        self.data: dict[StorageKey, tuple[RateLimitSingleToken, ...]] = {}
-
-        scheduler.add_job(
-            self.delete_outdated_tokens,
-            IntervalTrigger(minutes=1),
-            id="delete_outdated_tokens_inmemory",
-        )
-
-    def next_id(self) -> int:
-        self.id_cnt += 1
-        return self.id_cnt
-
-    async def get_first_expire_token(
-        self, rule: RateLimitRule, user: str
-    ) -> Optional[RateLimitSingleToken]:
-        key = StorageKey(rule.id, user)
-        tokens = _handle_expired(self.data.get(key) or ())
-        self.data[key] = tokens
-
-        with_min_expire_time = None
-        for x in tokens:
-            if (
-                with_min_expire_time is None
-                or x.expire_time < with_min_expire_time.expire_time
-            ):
-                with_min_expire_time = x
-        return with_min_expire_time
-
-    async def acquire_token(
-        self, rule: RateLimitRule, user: str
-    ) -> Optional[RateLimitSingleToken]:
-        key = StorageKey(rule.id, user)
-        tokens = _handle_expired(self.data.get(key) or ())
-        self.data[key] = tokens
-
-        if len(tokens) >= rule.limit:
-            return None
-
-        acquire_time = datetime.utcnow()
-        expire_time = acquire_time + rule.time_span
-
-        token = RateLimitSingleToken(
-            self.next_id(), rule.id, user, acquire_time, expire_time
-        )
-        self.data[key] = (*tokens, token)
-        return token
-
-    async def retire_token(self, token: RateLimitSingleToken):
-        key = StorageKey(token.rule_id, token.user)
-        tokens = _handle_expired(self.data.get(key) or ())
-        self.data[key] = tuple(filter(lambda x: x.id != token.id, tokens))
-
-    async def delete_outdated_tokens(self):
-        del_keys = set()
-
-        for k in self.data:
-            self.data[k] = _handle_expired(self.data[k])
-            if len(self.data[k]) == 0:
-                del_keys.add(k)
-
-        for k in del_keys:
-            del self.data[k]
-
-    async def clear_token(self):
-        self.data = {}
+from nonebot import require
+from nonebot_plugin_access_control_api.context import context
+
+require("nonebot_plugin_apscheduler")
+
+from datetime import datetime
+from typing import Optional, NamedTuple
+
+from nonebot_plugin_apscheduler import scheduler
+from apscheduler.triggers.interval import IntervalTrigger
+from nonebot_plugin_access_control_api.models.rate_limit import (
+    RateLimitRule,
+    RateLimitSingleToken,
+)
+
+from .interface import IRateLimitTokenRepository
+
+
+class StorageKey(NamedTuple):
+    rule_id: str
+    user: str
+
+
+def _handle_expired(
+    tokens: tuple[RateLimitSingleToken, ...]
+) -> tuple[RateLimitSingleToken, ...]:
+    now = datetime.utcnow()
+    return tuple(filter(lambda x: x.expire_time > now, tokens))
+
+
+@context.bind_singleton_to(IRateLimitTokenRepository)
+class InmemoryTokenRepository(IRateLimitTokenRepository):
+    def __init__(self):
+        self.id_cnt = 0
+        self.data: dict[StorageKey, tuple[RateLimitSingleToken, ...]] = {}
+
+        scheduler.add_job(
+            self.delete_outdated_tokens,
+            IntervalTrigger(minutes=1),
+            id="delete_outdated_tokens_inmemory",
+        )
+
+    def next_id(self) -> int:
+        self.id_cnt += 1
+        return self.id_cnt
+
+    async def get_first_expire_token(
+        self, rule: RateLimitRule, user: str
+    ) -> Optional[RateLimitSingleToken]:
+        key = StorageKey(rule.id, user)
+        tokens = _handle_expired(self.data.get(key) or ())
+        self.data[key] = tokens
+
+        with_min_expire_time = None
+        for x in tokens:
+            if (
+                with_min_expire_time is None
+                or x.expire_time < with_min_expire_time.expire_time
+            ):
+                with_min_expire_time = x
+        return with_min_expire_time
+
+    async def acquire_token(
+        self, rule: RateLimitRule, user: str
+    ) -> Optional[RateLimitSingleToken]:
+        key = StorageKey(rule.id, user)
+        tokens = _handle_expired(self.data.get(key) or ())
+        self.data[key] = tokens
+
+        if len(tokens) >= rule.limit:
+            return None
+
+        acquire_time = datetime.utcnow()
+        expire_time = acquire_time + rule.time_span
+
+        token = RateLimitSingleToken(
+            self.next_id(), rule.id, user, acquire_time, expire_time
+        )
+        self.data[key] = (*tokens, token)
+        return token
+
+    async def retire_token(self, token: RateLimitSingleToken):
+        key = StorageKey(token.rule_id, token.user)
+        tokens = _handle_expired(self.data.get(key) or ())
+        self.data[key] = tuple(filter(lambda x: x.id != token.id, tokens))
+
+    async def delete_outdated_tokens(self):
+        del_keys = set()
+
+        for k in self.data:
+            self.data[k] = _handle_expired(self.data[k])
+            if len(self.data[k]) == 0:
+                del_keys.add(k)
+
+        for k in del_keys:
+            del self.data[k]
+
+    async def clear_token(self):
+        self.data = {}
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/repository/utils.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/repository/utils.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import contextvars
-from contextlib import AbstractAsyncContextManager, asynccontextmanager
-
-from nonebot import logger
-from nonebot_plugin_orm import get_session
-from sqlalchemy.ext.asyncio import AsyncSession
-
-_ac_current_session = contextvars.ContextVar("ac_current_session")
-
-
-@asynccontextmanager
-async def use_ac_session() -> AbstractAsyncContextManager[AsyncSession]:
-    try:
-        yield _ac_current_session.get()
-    except LookupError:
-        session = get_session()
-        logger.trace("sqlalchemy session was created")
-        token = _ac_current_session.set(session)
-
-        try:
-            yield session
-        finally:
-            await session.close()
-            logger.trace("sqlalchemy session was closed")
-            _ac_current_session.reset(token)
+import contextvars
+from contextlib import AbstractAsyncContextManager, asynccontextmanager
+
+from nonebot import logger
+from nonebot_plugin_orm import get_session
+from sqlalchemy.ext.asyncio import AsyncSession
+
+_ac_current_session = contextvars.ContextVar("ac_current_session")
+
+
+@asynccontextmanager
+async def use_ac_session() -> AbstractAsyncContextManager[AsyncSession]:
+    try:
+        yield _ac_current_session.get()
+    except LookupError:
+        session = get_session()
+        logger.trace("sqlalchemy session was created")
+        token = _ac_current_session.set(session)
+
+        try:
+            yield session
+        finally:
+            await session.close()
+            logger.trace("sqlalchemy session was closed")
+            _ac_current_session.reset(token)
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/service/_impl/factory.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/service/_impl/factory.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from nonebot_plugin_access_control_api.context import context
-from nonebot_plugin_access_control_api.service.interface import IService
-from nonebot_plugin_access_control_api.service.interface.patcher import IServicePatcher
-from nonebot_plugin_access_control_api.service.interface.rate_limit import (
-    IServiceRateLimit,
-)
-from nonebot_plugin_access_control_api.service.interface.permission import (
-    IServicePermission,
-)
-from nonebot_plugin_access_control_api.service.interface.factory import (
-    IServiceComponentFactory,
-)
-
-from .patcher import ServicePatcherImpl
-from .rate_limit import ServiceRateLimitImpl
-from .permission import ServicePermissionImpl
-
-
-@context.bind_singleton_to(IServiceComponentFactory)
-class ServiceComponentFactory(IServiceComponentFactory):
-    def create_patcher_impl(self, service: IService) -> IServicePatcher:
-        return ServicePatcherImpl(service)
-
-    def typeof_patcher_impl(self) -> type[IServicePatcher]:
-        return ServicePatcherImpl
-
-    def create_permission_impl(self, service: IService) -> IServicePermission:
-        return ServicePermissionImpl(service)
-
-    def typeof_permission_impl(self) -> type[IServicePermission]:
-        return ServicePermissionImpl
-
-    def create_rate_limit_impl(self, service: IService) -> IServiceRateLimit:
-        return ServiceRateLimitImpl(service)
-
-    def typeof_rate_limit_impl(self) -> type[IServiceRateLimit]:
-        return ServiceRateLimitImpl
+from nonebot_plugin_access_control_api.context import context
+from nonebot_plugin_access_control_api.service.interface import IService
+from nonebot_plugin_access_control_api.service.interface.patcher import IServicePatcher
+from nonebot_plugin_access_control_api.service.interface.rate_limit import (
+    IServiceRateLimit,
+)
+from nonebot_plugin_access_control_api.service.interface.permission import (
+    IServicePermission,
+)
+from nonebot_plugin_access_control_api.service.interface.factory import (
+    IServiceComponentFactory,
+)
+
+from .patcher import ServicePatcherImpl
+from .rate_limit import ServiceRateLimitImpl
+from .permission import ServicePermissionImpl
+
+
+@context.bind_singleton_to(IServiceComponentFactory)
+class ServiceComponentFactory(IServiceComponentFactory):
+    def create_patcher_impl(self, service: IService) -> IServicePatcher:
+        return ServicePatcherImpl(service)
+
+    def typeof_patcher_impl(self) -> type[IServicePatcher]:
+        return ServicePatcherImpl
+
+    def create_permission_impl(self, service: IService) -> IServicePermission:
+        return ServicePermissionImpl(service)
+
+    def typeof_permission_impl(self) -> type[IServicePermission]:
+        return ServicePermissionImpl
+
+    def create_rate_limit_impl(self, service: IService) -> IServiceRateLimit:
+        return ServiceRateLimitImpl(service)
+
+    def typeof_rate_limit_impl(self) -> type[IServiceRateLimit]:
+        return ServiceRateLimitImpl
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/service/_impl/patcher.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/service/_impl/patcher.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-from functools import wraps
-from datetime import datetime
-
-from nonebot.internal.adapter import Event
-from nonebot.message import run_preprocessor
-from nonebot.exception import IgnoredException
-from nonebot import Bot, logger, get_driver, get_loaded_plugins
-from nonebot_plugin_access_control_api.service.interface import IService
-from nonebot_plugin_access_control_api.service import get_nonebot_service
-from nonebot_plugin_access_control_api.models.rate_limit import AcquireTokenResult
-from nonebot_plugin_access_control_api.service.interface.patcher import IServicePatcher
-from nonebot_plugin_access_control_api.service.contextvars import (
-    current_rate_limit_token,
-)
-from nonebot_plugin_access_control_api.errors import (
-    RateLimitedError,
-    PermissionDeniedError,
-)
-from nonebot.internal.matcher import (
-    Matcher,
-    current_bot,
-    current_event,
-    current_matcher,
-)
-
-from ...config import conf
-from ...repository.utils import use_ac_session
-
-
-class ServicePatcherImpl(IServicePatcher):
-    _matcher_service_mapping: dict[type[Matcher], IService] = {}
-
-    def __init__(self, service: IService):
-        self.service = service
-
-    @classmethod
-    async def handle_permission_denied(cls, matcher: Matcher):
-        if conf().access_control_reply_on_permission_denied_enabled:
-            await matcher.send(conf().access_control_reply_on_permission_denied)
-
-    @classmethod
-    async def handle_rate_limited(cls, matcher: Matcher, result: AcquireTokenResult):
-        if conf().access_control_reply_on_rate_limited_enabled:
-            msg = conf().access_control_reply_on_rate_limited
-            if msg is None:
-                now = datetime.utcnow()
-                available_time = result.available_time
-                msg = (
-                    "使用太频繁了，请稍后再试。"
-                    f"下次可用时间：{available_time.timestamp() - now.timestamp():.0f}秒后"
-                )
-            await matcher.send(msg)
-
-    def patch_matcher(self, matcher: type[Matcher]) -> type[Matcher]:
-        self._matcher_service_mapping[matcher] = self.service
-        logger.debug(f"patched {matcher}  (with service {self.service.qualified_name})")
-        return matcher
-
-    def patch_handler(self, retire_on_throw: bool = False):
-        def decorator(func):
-            @wraps(func)
-            async def wrapped_func(*args, **kwargs):
-                bot = current_bot.get()
-                event = current_event.get()
-                matcher = current_matcher.get()
-
-                async with use_ac_session():
-                    if not await self.service.check(
-                        bot, event, acquire_rate_limit_token=False
-                    ):
-                        await self.handle_permission_denied(matcher)
-                        return
-
-                    result = await self.service.acquire_token_for_rate_limit_receiving_result(
-                        bot, event
-                    )
-
-                if not result.success:
-                    await self.handle_rate_limited(matcher, result)
-                    return
-
-                t = current_rate_limit_token.set(result.token)
-                try:
-                    return await func(*args, **kwargs)
-                except BaseException as e:
-                    if retire_on_throw:
-                        await result.token.retire()
-                    raise e
-                finally:
-                    current_rate_limit_token.reset(t)
-
-            return wrapped_func
-
-        return decorator
-
-
-@run_preprocessor
-async def check(bot: Bot, event: Event, matcher: Matcher):
-    service = ServicePatcherImpl._matcher_service_mapping.get(type(matcher), None)
-    if service is None:
-        return
-
-    try:
-        async with use_ac_session():
-            await service.check(bot, event, throw_on_fail=True)
-    except PermissionDeniedError:
-        await ServicePatcherImpl.handle_permission_denied(matcher)
-        raise IgnoredException("permission denied (by nonebot_plugin_access_control)")
-    except RateLimitedError as e:
-        await ServicePatcherImpl.handle_rate_limited(matcher, e.result)
-        raise IgnoredException("rate limited (by nonebot_plugin_access_control)")
-
-
-def _auto_patch():
-    nonebot_service = get_nonebot_service()
-
-    patched_plugins = []
-
-    for plugin in get_loaded_plugins():
-        if (
-            plugin.name == "nonebot_plugin_access_control"
-            or plugin.name in conf().access_control_auto_patch_ignore
-        ):
-            continue
-
-        service = nonebot_service.get_or_create_plugin_service(plugin.name)
-        if service.auto_created:
-            for matcher in plugin.matcher:
-                service.patch_matcher(matcher)
-            patched_plugins.append(plugin)
-
-    logger.opt(colors=True).success(
-        "auto patched plugin(s): "
-        + ", ".join([f"<y>{p.name}</y>" for p in patched_plugins])
-    )
-
-
-if conf().access_control_auto_patch_enabled:
-    get_driver().on_startup(_auto_patch)
+from functools import wraps
+from datetime import datetime
+
+from nonebot.internal.adapter import Event
+from nonebot.message import run_preprocessor
+from nonebot.exception import IgnoredException
+from nonebot import Bot, logger, get_driver, get_loaded_plugins
+from nonebot_plugin_access_control_api.service.interface import IService
+from nonebot_plugin_access_control_api.service import get_nonebot_service
+from nonebot_plugin_access_control_api.models.rate_limit import AcquireTokenResult
+from nonebot_plugin_access_control_api.service.interface.patcher import IServicePatcher
+from nonebot_plugin_access_control_api.service.contextvars import (
+    current_rate_limit_token,
+)
+from nonebot_plugin_access_control_api.errors import (
+    RateLimitedError,
+    PermissionDeniedError,
+)
+from nonebot.internal.matcher import (
+    Matcher,
+    current_bot,
+    current_event,
+    current_matcher,
+)
+
+from ...config import conf
+from ...repository.utils import use_ac_session
+
+
+class ServicePatcherImpl(IServicePatcher):
+    _matcher_service_mapping: dict[type[Matcher], IService] = {}
+
+    def __init__(self, service: IService):
+        self.service = service
+
+    @classmethod
+    async def handle_permission_denied(cls, matcher: Matcher):
+        if conf().access_control_reply_on_permission_denied_enabled:
+            await matcher.send(conf().access_control_reply_on_permission_denied)
+
+    @classmethod
+    async def handle_rate_limited(cls, matcher: Matcher, result: AcquireTokenResult):
+        if conf().access_control_reply_on_rate_limited_enabled:
+            msg = conf().access_control_reply_on_rate_limited
+            if msg is None:
+                now = datetime.utcnow()
+                available_time = result.available_time
+                msg = (
+                    "使用太频繁了，请稍后再试。"
+                    f"下次可用时间：{available_time.timestamp() - now.timestamp():.0f}秒后"
+                )
+            await matcher.send(msg)
+
+    def patch_matcher(self, matcher: type[Matcher]) -> type[Matcher]:
+        self._matcher_service_mapping[matcher] = self.service
+        logger.debug(f"patched {matcher}  (with service {self.service.qualified_name})")
+        return matcher
+
+    def patch_handler(self, retire_on_throw: bool = False):
+        def decorator(func):
+            @wraps(func)
+            async def wrapped_func(*args, **kwargs):
+                bot = current_bot.get()
+                event = current_event.get()
+                matcher = current_matcher.get()
+
+                async with use_ac_session():
+                    if not await self.service.check(
+                        bot, event, acquire_rate_limit_token=False
+                    ):
+                        await self.handle_permission_denied(matcher)
+                        return
+
+                    result = await self.service.acquire_token_for_rate_limit_receiving_result(
+                        bot, event
+                    )
+
+                if not result.success:
+                    await self.handle_rate_limited(matcher, result)
+                    return
+
+                t = current_rate_limit_token.set(result.token)
+                try:
+                    return await func(*args, **kwargs)
+                except BaseException as e:
+                    if retire_on_throw:
+                        await result.token.retire()
+                    raise e
+                finally:
+                    current_rate_limit_token.reset(t)
+
+            return wrapped_func
+
+        return decorator
+
+
+@run_preprocessor
+async def check(bot: Bot, event: Event, matcher: Matcher):
+    service = ServicePatcherImpl._matcher_service_mapping.get(type(matcher), None)
+    if service is None:
+        return
+
+    try:
+        async with use_ac_session():
+            await service.check(bot, event, throw_on_fail=True)
+    except PermissionDeniedError:
+        await ServicePatcherImpl.handle_permission_denied(matcher)
+        raise IgnoredException("permission denied (by nonebot_plugin_access_control)")
+    except RateLimitedError as e:
+        await ServicePatcherImpl.handle_rate_limited(matcher, e.result)
+        raise IgnoredException("rate limited (by nonebot_plugin_access_control)")
+
+
+def _auto_patch():
+    nonebot_service = get_nonebot_service()
+
+    patched_plugins = []
+
+    for plugin in get_loaded_plugins():
+        if (
+            plugin.name == "nonebot_plugin_access_control"
+            or plugin.name in conf().access_control_auto_patch_ignore
+        ):
+            continue
+
+        service = nonebot_service.get_or_create_plugin_service(plugin.name)
+        if service.auto_created:
+            for matcher in plugin.matcher:
+                service.patch_matcher(matcher)
+            patched_plugins.append(plugin)
+
+    logger.opt(colors=True).success(
+        "auto patched plugin(s): "
+        + ", ".join([f"<y>{p.name}</y>" for p in patched_plugins])
+    )
+
+
+if conf().access_control_auto_patch_enabled:
+    get_driver().on_startup(_auto_patch)
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/service/_impl/rate_limit.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/service/_impl/rate_limit.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-from typing import Optional
-from datetime import timedelta
-from collections.abc import Collection, AsyncGenerator
-
-from nonebot import logger
-from nonebot_plugin_access_control_api.context import context
-from nonebot_plugin_access_control_api.service.interface import IService
-from nonebot_plugin_access_control_api.service.interface.rate_limit import (
-    IServiceRateLimit,
-)
-from nonebot_plugin_access_control_api.event_bus import (
-    EventType,
-    T_Listener,
-    on_event,
-    fire_event,
-)
-from nonebot_plugin_access_control_api.models.rate_limit import (
-    RateLimitRule,
-    IRateLimitToken,
-    AcquireTokenResult,
-    RateLimitSingleToken,
-)
-
-from ...repository.utils import use_ac_session
-from ...repository.rate_limit import IRateLimitRepository
-from ...repository.rate_limit_token import IRateLimitTokenRepository
-
-
-class RateLimitTokenImpl(IRateLimitToken):
-    def __init__(
-        self, tokens: Collection[RateLimitSingleToken], service: "ServiceRateLimitImpl"
-    ):
-        self.tokens = tokens
-        self.service = service
-
-    async def retire(self):
-        async with use_ac_session():
-            for t in self.tokens:
-                await self.service._retire_token(t)
-
-
-class ServiceRateLimitImpl(IServiceRateLimit):
-    repo = context.require(IRateLimitRepository)
-    token_repo = context.require(IRateLimitTokenRepository)
-
-    def __init__(self, service: IService):
-        self.service = service
-
-    def on_add_rate_limit_rule(self, func: Optional[T_Listener] = None):
-        return on_event(
-            EventType.service_add_rate_limit_rule,
-            lambda service: service == self.service,
-            func,
-        )
-
-    def on_remove_rate_limit_rule(self, func: Optional[T_Listener] = None):
-        return on_event(
-            EventType.service_remove_rate_limit_rule,
-            lambda service: service == self.service,
-            func,
-        )
-
-    @classmethod
-    async def _get_rules_by_subject(
-        cls, service: Optional[IService], subject: Optional[str]
-    ) -> AsyncGenerator[RateLimitRule, None]:
-        async for x in cls.repo.get_rules_by_subject(service, subject):
-            yield x
-
-    async def get_rate_limit_rules_by_subject(
-        self, *subject: str, trace: bool = True
-    ) -> AsyncGenerator[RateLimitRule, None]:
-        async with use_ac_session():
-            for sub in subject:
-                if trace:
-                    for node in self.service.trace():
-                        async for p in self._get_rules_by_subject(node, sub):
-                            yield p
-                            if p.overwrite:
-                                return
-                else:
-                    async for p in self._get_rules_by_subject(self.service, sub):
-                        yield p
-                        if p.overwrite:
-                            return
-
-    async def get_rate_limit_rules(
-        self, *, trace: bool = True
-    ) -> AsyncGenerator[RateLimitRule, None]:
-        async with use_ac_session():
-            if trace:
-                for node in self.service.trace():
-                    async for p in self._get_rules_by_subject(node, None):
-                        yield p
-            else:
-                async for p in self._get_rules_by_subject(self.service, None):
-                    yield p
-
-    @classmethod
-    async def get_all_rate_limit_rules_by_subject(
-        cls, *subject: str
-    ) -> AsyncGenerator[RateLimitRule, None]:
-        async with use_ac_session():
-            for sub in subject:
-                async for x in cls._get_rules_by_subject(None, sub):
-                    yield x
-
-    @classmethod
-    async def get_all_rate_limit_rules(cls) -> AsyncGenerator[RateLimitRule, None]:
-        async with use_ac_session():
-            async for x in cls._get_rules_by_subject(None, None):
-                yield x
-
-    @staticmethod
-    async def _fire_service_add_rate_limit_rule(rule: RateLimitRule):
-        for node in rule.service.travel():
-            await fire_event(
-                EventType.service_add_rate_limit_rule, {"service": node, "rule": rule}
-            )
-
-    @staticmethod
-    async def _fire_service_remove_rate_limit_rule(rule: RateLimitRule):
-        for node in rule.service.travel():
-            await fire_event(
-                EventType.service_remove_rate_limit_rule,
-                {"service": node, "rule": rule},
-            )
-
-    async def add_rate_limit_rule(
-        self, subject: str, time_span: timedelta, limit: int, overwrite: bool = False
-    ) -> RateLimitRule:
-        async with use_ac_session():
-            rule = await self.repo.add_rate_limit_rule(
-                self.service, subject, time_span, limit, overwrite
-            )
-            await self._fire_service_add_rate_limit_rule(rule)
-            return rule
-
-    @classmethod
-    async def remove_rate_limit_rule(cls, rule_id: str) -> bool:
-        async with use_ac_session():
-            rule = await cls.repo.remove_rate_limit_rule(rule_id)
-            if rule is not None:
-                await cls._fire_service_remove_rate_limit_rule(rule)
-                return True
-            else:
-                return False
-
-    @classmethod
-    async def _get_first_expire_token(
-        cls, rule: RateLimitRule, user: str
-    ) -> Optional[RateLimitSingleToken]:
-        return await cls.token_repo.get_first_expire_token(rule, user)
-
-    @classmethod
-    async def _acquire_token(
-        cls, rule: RateLimitRule, user: str
-    ) -> Optional[RateLimitSingleToken]:
-        x = await cls.token_repo.acquire_token(rule, user)
-        if x is not None:
-            logger.trace(
-                f"[rate limit] token {x.id} acquired "
-                f"for rule {x.rule_id} by user {x.user} "
-                f"(service: {rule.service})"
-            )
-        return x
-
-    @classmethod
-    async def _retire_token(cls, token: RateLimitSingleToken):
-        await cls.token_repo.retire_token(token)
-        logger.trace(
-            f"[rate limit] token {token.id} retired for "
-            f"rule {token.rule_id} by user {token.user}"
-        )
-
-    async def acquire_token_for_rate_limit_by_subjects_receiving_result(
-        self, *subject: str
-    ) -> AcquireTokenResult:
-        async with use_ac_session():
-            assert len(subject) > 0, "require at least one subject"
-            user = subject[0]
-
-            tokens = []
-            violating_rules = []
-
-            # 先获取所有rule，再对每个rule获取token
-            rules = [x async for x in self.get_rate_limit_rules_by_subject(*subject)]
-            for rule in rules:
-                token = await self._acquire_token(rule, user)
-                if token is not None:
-                    tokens.append(token)
-                else:
-                    logger.debug(
-                        f"[rate limit] limit reached for rule {rule.id} "
-                        f"(service: {rule.service}, subject: {rule.subject})"
-                    )
-                    violating_rules.append(rule)
-
-                if rule.overwrite:
-                    break
-
-            success = len(violating_rules) == 0
-            if not success:
-                for t in tokens:
-                    await self._retire_token(t)
-
-                first_expire_token = None
-                for rule in violating_rules:
-                    _first_expire_token = await self._get_first_expire_token(rule, user)
-                    if (
-                        first_expire_token is None
-                        or _first_expire_token.expire_time
-                        < first_expire_token.expire_time
-                    ):
-                        first_expire_token = _first_expire_token
-
-                return AcquireTokenResult(
-                    success=False,
-                    violating=violating_rules,
-                    available_time=first_expire_token.expire_time,
-                )
-            else:
-                return AcquireTokenResult(
-                    success=True, token=RateLimitTokenImpl(tokens, self)
-                )
-
-    @classmethod
-    async def clear_rate_limit_tokens(cls):
-        async with use_ac_session():
-            await cls.token_repo.clear_token()
+from typing import Optional
+from datetime import timedelta
+from collections.abc import Collection, AsyncGenerator
+
+from nonebot import logger
+from nonebot_plugin_access_control_api.context import context
+from nonebot_plugin_access_control_api.service.interface import IService
+from nonebot_plugin_access_control_api.service.interface.rate_limit import (
+    IServiceRateLimit,
+)
+from nonebot_plugin_access_control_api.event_bus import (
+    EventType,
+    T_Listener,
+    on_event,
+    fire_event,
+)
+from nonebot_plugin_access_control_api.models.rate_limit import (
+    RateLimitRule,
+    IRateLimitToken,
+    AcquireTokenResult,
+    RateLimitSingleToken,
+)
+
+from ...repository.utils import use_ac_session
+from ...repository.rate_limit import IRateLimitRepository
+from ...repository.rate_limit_token import IRateLimitTokenRepository
+
+
+class RateLimitTokenImpl(IRateLimitToken):
+    def __init__(
+        self, tokens: Collection[RateLimitSingleToken], service: "ServiceRateLimitImpl"
+    ):
+        self.tokens = tokens
+        self.service = service
+
+    async def retire(self):
+        async with use_ac_session():
+            for t in self.tokens:
+                await self.service._retire_token(t)
+
+
+class ServiceRateLimitImpl(IServiceRateLimit):
+    repo = context.require(IRateLimitRepository)
+    token_repo = context.require(IRateLimitTokenRepository)
+
+    def __init__(self, service: IService):
+        self.service = service
+
+    def on_add_rate_limit_rule(self, func: Optional[T_Listener] = None):
+        return on_event(
+            EventType.service_add_rate_limit_rule,
+            lambda service: service == self.service,
+            func,
+        )
+
+    def on_remove_rate_limit_rule(self, func: Optional[T_Listener] = None):
+        return on_event(
+            EventType.service_remove_rate_limit_rule,
+            lambda service: service == self.service,
+            func,
+        )
+
+    @classmethod
+    async def _get_rules_by_subject(
+        cls, service: Optional[IService], subject: Optional[str]
+    ) -> AsyncGenerator[RateLimitRule, None]:
+        async for x in cls.repo.get_rules_by_subject(service, subject):
+            yield x
+
+    async def get_rate_limit_rules_by_subject(
+        self, *subject: str, trace: bool = True
+    ) -> AsyncGenerator[RateLimitRule, None]:
+        async with use_ac_session():
+            for sub in subject:
+                if trace:
+                    for node in self.service.trace():
+                        async for p in self._get_rules_by_subject(node, sub):
+                            yield p
+                            if p.overwrite:
+                                return
+                else:
+                    async for p in self._get_rules_by_subject(self.service, sub):
+                        yield p
+                        if p.overwrite:
+                            return
+
+    async def get_rate_limit_rules(
+        self, *, trace: bool = True
+    ) -> AsyncGenerator[RateLimitRule, None]:
+        async with use_ac_session():
+            if trace:
+                for node in self.service.trace():
+                    async for p in self._get_rules_by_subject(node, None):
+                        yield p
+            else:
+                async for p in self._get_rules_by_subject(self.service, None):
+                    yield p
+
+    @classmethod
+    async def get_all_rate_limit_rules_by_subject(
+        cls, *subject: str
+    ) -> AsyncGenerator[RateLimitRule, None]:
+        async with use_ac_session():
+            for sub in subject:
+                async for x in cls._get_rules_by_subject(None, sub):
+                    yield x
+
+    @classmethod
+    async def get_all_rate_limit_rules(cls) -> AsyncGenerator[RateLimitRule, None]:
+        async with use_ac_session():
+            async for x in cls._get_rules_by_subject(None, None):
+                yield x
+
+    @staticmethod
+    async def _fire_service_add_rate_limit_rule(rule: RateLimitRule):
+        for node in rule.service.travel():
+            await fire_event(
+                EventType.service_add_rate_limit_rule, {"service": node, "rule": rule}
+            )
+
+    @staticmethod
+    async def _fire_service_remove_rate_limit_rule(rule: RateLimitRule):
+        for node in rule.service.travel():
+            await fire_event(
+                EventType.service_remove_rate_limit_rule,
+                {"service": node, "rule": rule},
+            )
+
+    async def add_rate_limit_rule(
+        self, subject: str, time_span: timedelta, limit: int, overwrite: bool = False
+    ) -> RateLimitRule:
+        async with use_ac_session():
+            rule = await self.repo.add_rate_limit_rule(
+                self.service, subject, time_span, limit, overwrite
+            )
+            await self._fire_service_add_rate_limit_rule(rule)
+            return rule
+
+    @classmethod
+    async def remove_rate_limit_rule(cls, rule_id: str) -> bool:
+        async with use_ac_session():
+            rule = await cls.repo.remove_rate_limit_rule(rule_id)
+            if rule is not None:
+                await cls._fire_service_remove_rate_limit_rule(rule)
+                return True
+            else:
+                return False
+
+    @classmethod
+    async def _get_first_expire_token(
+        cls, rule: RateLimitRule, user: str
+    ) -> Optional[RateLimitSingleToken]:
+        return await cls.token_repo.get_first_expire_token(rule, user)
+
+    @classmethod
+    async def _acquire_token(
+        cls, rule: RateLimitRule, user: str
+    ) -> Optional[RateLimitSingleToken]:
+        x = await cls.token_repo.acquire_token(rule, user)
+        if x is not None:
+            logger.trace(
+                f"[rate limit] token {x.id} acquired "
+                f"for rule {x.rule_id} by user {x.user} "
+                f"(service: {rule.service})"
+            )
+        return x
+
+    @classmethod
+    async def _retire_token(cls, token: RateLimitSingleToken):
+        await cls.token_repo.retire_token(token)
+        logger.trace(
+            f"[rate limit] token {token.id} retired for "
+            f"rule {token.rule_id} by user {token.user}"
+        )
+
+    async def acquire_token_for_rate_limit_by_subjects_receiving_result(
+        self, *subject: str
+    ) -> AcquireTokenResult:
+        async with use_ac_session():
+            assert len(subject) > 0, "require at least one subject"
+            user = subject[0]
+
+            tokens = []
+            violating_rules = []
+
+            # 先获取所有rule，再对每个rule获取token
+            rules = [x async for x in self.get_rate_limit_rules_by_subject(*subject)]
+            for rule in rules:
+                token = await self._acquire_token(rule, user)
+                if token is not None:
+                    tokens.append(token)
+                else:
+                    logger.debug(
+                        f"[rate limit] limit reached for rule {rule.id} "
+                        f"(service: {rule.service}, subject: {rule.subject})"
+                    )
+                    violating_rules.append(rule)
+
+                if rule.overwrite:
+                    break
+
+            success = len(violating_rules) == 0
+            if not success:
+                for t in tokens:
+                    await self._retire_token(t)
+
+                first_expire_token = None
+                for rule in violating_rules:
+                    _first_expire_token = await self._get_first_expire_token(rule, user)
+                    if (
+                        first_expire_token is None
+                        or _first_expire_token.expire_time
+                        < first_expire_token.expire_time
+                    ):
+                        first_expire_token = _first_expire_token
+
+                return AcquireTokenResult(
+                    success=False,
+                    violating=violating_rules,
+                    available_time=first_expire_token.expire_time,
+                )
+            else:
+                return AcquireTokenResult(
+                    success=True, token=RateLimitTokenImpl(tokens, self)
+                )
+
+    @classmethod
+    async def clear_rate_limit_tokens(cls):
+        async with use_ac_session():
+            await cls.token_repo.clear_token()
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/subject/extractor/__init__.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/subject/extractor/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from collections.abc import Sequence
-
-from nonebot import logger
-from nonebot_plugin_session import Session
-from nonebot_plugin_access_control_api.subject.extractor import extractor_chain
-
-from .builtin.qqguild import extract_qqguild_role
-from .builtin.kaiheila import extract_kaiheila_role
-from .builtin.onebot_v11 import extract_onebot_v11_group_role
-from .builtin.session import extract_by_session, extract_from_session
-
-extractor_chain.add_first(
-    extract_by_session,
-    extract_onebot_v11_group_role,
-    extract_qqguild_role,
-    extract_kaiheila_role,
-)
-logger.debug("added default subject extractors")
-
-
-def extract_subjects_from_session(session: Session) -> Sequence[str]:
-    sbj = [x.content for x in extract_from_session(session)]
-    logger.debug("subjects: " + ", ".join(sbj))
-    return sbj
-
-
-__all__ = ("extract_subjects_from_session",)
+from collections.abc import Sequence
+
+from nonebot import logger
+from nonebot_plugin_session import Session
+from nonebot_plugin_access_control_api.subject.extractor import extractor_chain
+
+from .builtin.qqguild import extract_qqguild_role
+from .builtin.kaiheila import extract_kaiheila_role
+from .builtin.onebot_v11 import extract_onebot_v11_group_role
+from .builtin.session import extract_by_session, extract_from_session
+
+extractor_chain.add_first(
+    extract_by_session,
+    extract_onebot_v11_group_role,
+    extract_qqguild_role,
+    extract_kaiheila_role,
+)
+logger.debug("added default subject extractors")
+
+
+def extract_subjects_from_session(session: Session) -> Sequence[str]:
+    sbj = [x.content for x in extract_from_session(session)]
+    logger.debug("subjects: " + ", ".join(sbj))
+    return sbj
+
+
+__all__ = ("extract_subjects_from_session",)
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/subject/extractor/builtin/kaiheila.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/subject/extractor/builtin/kaiheila.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from typing import TYPE_CHECKING, Optional
-
-from nonebot import Bot
-from nonebot.internal.adapter import Event
-from nonebot_plugin_access_control_api.subject.model import SubjectModel
-from nonebot_plugin_access_control_api.subject.manager import SubjectManager
-
-if TYPE_CHECKING:
-    from nonebot.adapters.kaiheila.event import User
-    from nonebot.adapters.kaiheila.event import Event as KaiheilaEvent
-
-OFFER_BY = "nonebot_plugin_access_control"
-
-
-def extract_kaiheila_role(bot: Bot, event: Event, manager: SubjectManager):
-    if bot.type != "Kaiheila":
-        return
-
-    event: KaiheilaEvent
-
-    guild_id: Optional[str] = event.extra.guild_id
-    getattr(event, "group_id", None) or getattr(event.extra.body, "channel_id", None)
-    author: Optional["User"] = event.extra.author
-
-    if author is not None:
-        li = []
-
-        for role in sorted(author.roles):
-            li.append(
-                SubjectModel(
-                    f"kaiheila:g{guild_id}.role_{role}", OFFER_BY, "kaiheila:guild.role"
-                )
-            )
-
-        # 添加在platform:guild:channel之前
-        manager.insert_before("platform:guild:channel", *li)
+from typing import TYPE_CHECKING, Optional
+
+from nonebot import Bot
+from nonebot.internal.adapter import Event
+from nonebot_plugin_access_control_api.subject.model import SubjectModel
+from nonebot_plugin_access_control_api.subject.manager import SubjectManager
+
+if TYPE_CHECKING:
+    from nonebot.adapters.kaiheila.event import User
+    from nonebot.adapters.kaiheila.event import Event as KaiheilaEvent
+
+OFFER_BY = "nonebot_plugin_access_control"
+
+
+def extract_kaiheila_role(bot: Bot, event: Event, manager: SubjectManager):
+    if bot.type != "Kaiheila":
+        return
+
+    event: KaiheilaEvent
+
+    guild_id: Optional[str] = event.extra.guild_id
+    getattr(event, "group_id", None) or getattr(event.extra.body, "channel_id", None)
+    author: Optional["User"] = event.extra.author
+
+    if author is not None:
+        li = []
+
+        for role in sorted(author.roles):
+            li.append(
+                SubjectModel(
+                    f"kaiheila:g{guild_id}.role_{role}", OFFER_BY, "kaiheila:guild.role"
+                )
+            )
+
+        # 添加在platform:guild:channel之前
+        manager.insert_before("platform:guild:channel", *li)
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/subject/extractor/builtin/qqguild.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/subject/extractor/builtin/qqguild.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from typing import TYPE_CHECKING, Optional
-
-from nonebot import Bot
-from nonebot.internal.adapter import Event
-from nonebot_plugin_access_control_api.subject.model import SubjectModel
-from nonebot_plugin_access_control_api.subject.manager import SubjectManager
-
-if TYPE_CHECKING:
-    from nonebot.adapters.qqguild.event import Member
-
-OFFER_BY = "nonebot_plugin_access_control"
-
-PRESET_ROLES = {2: "guild_admin", 4: "guild_owner", 5: "channel_admin"}
-
-PRESET_ROLE_PRIORITY = (4, 2, 5)
-
-
-def extract_qqguild_role(bot: Bot, event: Event, manager: SubjectManager):
-    if bot.type != "QQ Guild":
-        return
-
-    is_direct_msg = getattr(event, "src_guild_id", None) is not None
-    if is_direct_msg:
-        return
-
-    guild_id: Optional[str] = getattr(event, "guild_id", None)
-    channel_id: Optional[str] = getattr(event, "channel_id", None)
-    member: Optional["Member"] = getattr(event, "member", None)
-
-    if member is not None:
-        li = []
-
-        for actual_role in sorted(member.roles):
-            if actual_role in PRESET_ROLES:
-                # 我们默认优先级高的预置角色（例如服务器主）
-                # 继承优先级低的（例如频道管理员）
-                priority = PRESET_ROLE_PRIORITY.index(actual_role)
-                for i in range(priority, len(PRESET_ROLE_PRIORITY)):
-                    role = PRESET_ROLE_PRIORITY[i]
-
-                    if role == 5:  # 频道管理员
-                        li.append(
-                            SubjectModel(
-                                f"qqguild:g{guild_id}:c{channel_id}.{PRESET_ROLES[role]}",
-                                OFFER_BY,
-                                f"qqguild:guild:channel.{PRESET_ROLES[role]}",
-                            )
-                        )
-                        li.append(
-                            SubjectModel(
-                                f"qqguild:c{channel_id}.{PRESET_ROLES[role]}",
-                                OFFER_BY,
-                                f"qqguild:channel:{PRESET_ROLES[role]}",
-                            )
-                        )
-                    else:
-                        li.append(
-                            SubjectModel(
-                                f"qqguild:g{guild_id}.{PRESET_ROLES[role]}",
-                                OFFER_BY,
-                                f"qqguild:guild.{PRESET_ROLES[role]}",
-                            )
-                        )
-                    li.append(
-                        SubjectModel(
-                            f"qqguild:{PRESET_ROLES[role]}",
-                            OFFER_BY,
-                            f"qqguild:{PRESET_ROLES[role]}",
-                        )
-                    )
-            else:
-                li.append(
-                    SubjectModel(
-                        f"qqguild:g{guild_id}.role_{actual_role}",
-                        OFFER_BY,
-                        "qqguild:guild.role",
-                    )
-                )
-
-        # 添加在platform:guild:channel之前
-        manager.insert_before("platform:guild:channel", *li)
+from typing import TYPE_CHECKING, Optional
+
+from nonebot import Bot
+from nonebot.internal.adapter import Event
+from nonebot_plugin_access_control_api.subject.model import SubjectModel
+from nonebot_plugin_access_control_api.subject.manager import SubjectManager
+
+if TYPE_CHECKING:
+    from nonebot.adapters.qqguild.event import Member
+
+OFFER_BY = "nonebot_plugin_access_control"
+
+PRESET_ROLES = {2: "guild_admin", 4: "guild_owner", 5: "channel_admin"}
+
+PRESET_ROLE_PRIORITY = (4, 2, 5)
+
+
+def extract_qqguild_role(bot: Bot, event: Event, manager: SubjectManager):
+    if bot.type != "QQ Guild":
+        return
+
+    is_direct_msg = getattr(event, "src_guild_id", None) is not None
+    if is_direct_msg:
+        return
+
+    guild_id: Optional[str] = getattr(event, "guild_id", None)
+    channel_id: Optional[str] = getattr(event, "channel_id", None)
+    member: Optional["Member"] = getattr(event, "member", None)
+
+    if member is not None:
+        li = []
+
+        for actual_role in sorted(member.roles):
+            if actual_role in PRESET_ROLES:
+                # 我们默认优先级高的预置角色（例如服务器主）
+                # 继承优先级低的（例如频道管理员）
+                priority = PRESET_ROLE_PRIORITY.index(actual_role)
+                for i in range(priority, len(PRESET_ROLE_PRIORITY)):
+                    role = PRESET_ROLE_PRIORITY[i]
+
+                    if role == 5:  # 频道管理员
+                        li.append(
+                            SubjectModel(
+                                f"qqguild:g{guild_id}:c{channel_id}.{PRESET_ROLES[role]}",
+                                OFFER_BY,
+                                f"qqguild:guild:channel.{PRESET_ROLES[role]}",
+                            )
+                        )
+                        li.append(
+                            SubjectModel(
+                                f"qqguild:c{channel_id}.{PRESET_ROLES[role]}",
+                                OFFER_BY,
+                                f"qqguild:channel:{PRESET_ROLES[role]}",
+                            )
+                        )
+                    else:
+                        li.append(
+                            SubjectModel(
+                                f"qqguild:g{guild_id}.{PRESET_ROLES[role]}",
+                                OFFER_BY,
+                                f"qqguild:guild.{PRESET_ROLES[role]}",
+                            )
+                        )
+                    li.append(
+                        SubjectModel(
+                            f"qqguild:{PRESET_ROLES[role]}",
+                            OFFER_BY,
+                            f"qqguild:{PRESET_ROLES[role]}",
+                        )
+                    )
+            else:
+                li.append(
+                    SubjectModel(
+                        f"qqguild:g{guild_id}.role_{actual_role}",
+                        OFFER_BY,
+                        "qqguild:guild.role",
+                    )
+                )
+
+        # 添加在platform:guild:channel之前
+        manager.insert_before("platform:guild:channel", *li)
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/src/nonebot_plugin_access_control/subject/extractor/builtin/session.py` & `nonebot_plugin_access_control-1.2.0/src/nonebot_plugin_access_control/subject/extractor/builtin/session.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-from collections.abc import Sequence
-
-from nonebot import Bot
-from nonebot.internal.adapter import Event
-from nonebot_plugin_access_control_api.subject.model import SubjectModel
-from nonebot_plugin_session import Session, SessionLevel, extract_session
-from nonebot_plugin_access_control_api.utils.superuser import is_superuser
-from nonebot_plugin_access_control_api.subject.manager import SubjectManager
-
-OFFER_BY = "nonebot_plugin_access_control"
-
-
-def _append_subject(
-    li: list[SubjectModel],
-    content_body: str,
-    content_prefix: Sequence[str],
-    tag: Sequence[str],
-):
-    for i in range(min(len(content_prefix), len(tag))):
-        li.append(SubjectModel(f"{content_prefix[i]}{content_body}", OFFER_BY, tag[i]))
-
-
-def extract_from_session(session: Session) -> Sequence[SubjectModel]:
-    if session.bot_type == "OneBot V11" or session.bot_type == "OneBot V12":
-        prefix = [session.platform, "onebot"]
-    else:
-        prefix = [session.platform]
-
-    li: list[SubjectModel] = []
-
-    if session.level == SessionLevel.LEVEL3:
-        user_id = session.id1
-        channel_id = session.id2
-        guild_id = session.id3
-
-        _append_subject(
-            li,
-            f":g{guild_id}:c{channel_id}:{user_id}",
-            prefix,
-            ["platform:guild:channel:user", "onebot:guild:channel:user"],
-        )
-        _append_subject(
-            li,
-            f":c{channel_id}:{user_id}",
-            prefix,
-            ["platform:channel:user", "onebot:channel:user"],
-        )
-        _append_subject(
-            li,
-            f":g{guild_id}:{user_id}",
-            prefix,
-            ["platform:guild:user", "onebot:guild:user"],
-        )
-        _append_subject(li, f":{user_id}", prefix, ["platform:user", "onebot:user"])
-
-        if is_superuser(user_id, session.bot_type):
-            li.append(SubjectModel("superuser", OFFER_BY, "superuser"))
-
-        _append_subject(
-            li,
-            f":g{guild_id}:c{channel_id}",
-            prefix,
-            ["platform:guild:channel", "onebot:guild:channel"],
-        )
-        _append_subject(
-            li, f":c{channel_id}", prefix, ["platform:channel", "onebot:channel"]
-        )
-        _append_subject(li, f":g{guild_id}", prefix, ["platform:guild", "onebot:guild"])
-
-        _append_subject(
-            li, ":channel", prefix, ["platform:chat_type", "onebot:chat_type"]
-        )
-        li.append(SubjectModel("channel", OFFER_BY, "chat_type"))
-    elif session.level == SessionLevel.LEVEL2:
-        user_id = session.id1
-        group_id = session.id2
-
-        _append_subject(
-            li,
-            f":g{group_id}:{user_id}",
-            prefix,
-            ["platform:group:user", "onebot:group:user"],
-        )
-        _append_subject(li, f":{user_id}", prefix, ["platform:user", "onebot:user"])
-
-        if is_superuser(user_id, session.bot_type):
-            li.append(SubjectModel("superuser", OFFER_BY, "superuser"))
-
-        _append_subject(li, f":g{group_id}", prefix, ["platform:group", "onebot:group"])
-        _append_subject(
-            li, ":group", prefix, ["platform:chat_type", "onebot:chat_type"]
-        )
-        li.append(SubjectModel("group", OFFER_BY, "chat_type"))
-    elif session.level == SessionLevel.LEVEL1:
-        user_id = session.id1
-
-        _append_subject(li, f":{user_id}", prefix, ["platform:user", "onebot:user"])
-
-        if is_superuser(user_id, session.bot_type):
-            li.append(SubjectModel("superuser", OFFER_BY, "superuser"))
-
-        _append_subject(
-            li, ":private", prefix, ["platform:chat_type", "onebot:chat_type"]
-        )
-        li.append(SubjectModel("private", OFFER_BY, "chat_type"))
-
-    _append_subject(li, "", prefix, ["platform", "onebot"])
-
-    li.append(SubjectModel("all", OFFER_BY, "all"))
-
-    return li
-
-
-def extract_by_session(bot: Bot, event: Event, manager: SubjectManager):
-    session = extract_session(bot, event)
-    manager.append(*extract_from_session(session))
+from collections.abc import Sequence
+
+from nonebot import Bot
+from nonebot.internal.adapter import Event
+from nonebot_plugin_access_control_api.subject.model import SubjectModel
+from nonebot_plugin_session import Session, SessionLevel, extract_session
+from nonebot_plugin_access_control_api.utils.superuser import is_superuser
+from nonebot_plugin_access_control_api.subject.manager import SubjectManager
+
+OFFER_BY = "nonebot_plugin_access_control"
+
+
+def _append_subject(
+    li: list[SubjectModel],
+    content_body: str,
+    content_prefix: Sequence[str],
+    tag: Sequence[str],
+):
+    for i in range(min(len(content_prefix), len(tag))):
+        li.append(SubjectModel(f"{content_prefix[i]}{content_body}", OFFER_BY, tag[i]))
+
+
+def extract_from_session(session: Session) -> Sequence[SubjectModel]:
+    if session.bot_type == "OneBot V11" or session.bot_type == "OneBot V12":
+        prefix = [session.platform, "onebot"]
+    else:
+        prefix = [session.platform]
+
+    li: list[SubjectModel] = []
+
+    if session.level == SessionLevel.LEVEL3:
+        user_id = session.id1
+        channel_id = session.id2
+        guild_id = session.id3
+
+        _append_subject(
+            li,
+            f":g{guild_id}:c{channel_id}:{user_id}",
+            prefix,
+            ["platform:guild:channel:user", "onebot:guild:channel:user"],
+        )
+        _append_subject(
+            li,
+            f":c{channel_id}:{user_id}",
+            prefix,
+            ["platform:channel:user", "onebot:channel:user"],
+        )
+        _append_subject(
+            li,
+            f":g{guild_id}:{user_id}",
+            prefix,
+            ["platform:guild:user", "onebot:guild:user"],
+        )
+        _append_subject(li, f":{user_id}", prefix, ["platform:user", "onebot:user"])
+
+        if is_superuser(user_id, session.bot_type):
+            li.append(SubjectModel("superuser", OFFER_BY, "superuser"))
+
+        _append_subject(
+            li,
+            f":g{guild_id}:c{channel_id}",
+            prefix,
+            ["platform:guild:channel", "onebot:guild:channel"],
+        )
+        _append_subject(
+            li, f":c{channel_id}", prefix, ["platform:channel", "onebot:channel"]
+        )
+        _append_subject(li, f":g{guild_id}", prefix, ["platform:guild", "onebot:guild"])
+
+        _append_subject(
+            li, ":channel", prefix, ["platform:chat_type", "onebot:chat_type"]
+        )
+        li.append(SubjectModel("channel", OFFER_BY, "chat_type"))
+    elif session.level == SessionLevel.LEVEL2:
+        user_id = session.id1
+        group_id = session.id2
+
+        _append_subject(
+            li,
+            f":g{group_id}:{user_id}",
+            prefix,
+            ["platform:group:user", "onebot:group:user"],
+        )
+        _append_subject(li, f":{user_id}", prefix, ["platform:user", "onebot:user"])
+
+        if is_superuser(user_id, session.bot_type):
+            li.append(SubjectModel("superuser", OFFER_BY, "superuser"))
+
+        _append_subject(li, f":g{group_id}", prefix, ["platform:group", "onebot:group"])
+        _append_subject(
+            li, ":group", prefix, ["platform:chat_type", "onebot:chat_type"]
+        )
+        li.append(SubjectModel("group", OFFER_BY, "chat_type"))
+    elif session.level == SessionLevel.LEVEL1:
+        user_id = session.id1
+
+        _append_subject(li, f":{user_id}", prefix, ["platform:user", "onebot:user"])
+
+        if is_superuser(user_id, session.bot_type):
+            li.append(SubjectModel("superuser", OFFER_BY, "superuser"))
+
+        _append_subject(
+            li, ":private", prefix, ["platform:chat_type", "onebot:chat_type"]
+        )
+        li.append(SubjectModel("private", OFFER_BY, "chat_type"))
+
+    _append_subject(li, "", prefix, ["platform", "onebot"])
+
+    li.append(SubjectModel("all", OFFER_BY, "all"))
+
+    return li
+
+
+def extract_by_session(bot: Bot, event: Event, manager: SubjectManager):
+    session = extract_session(bot, event)
+    manager.append(*extract_from_session(session))
```

### Comparing `nonebot_plugin_access_control-1.1.5a1/PKG-INFO` & `nonebot_plugin_access_control-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-access-control
-Version: 1.1.5a1
+Version: 1.2.0
 Summary: 
 Home-page: https://github.com/bot-ssttkkl/nonebot-plugin-access-control
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: cli
 Provides-Extra: migrate
 Requires-Dist: arclet-alconna (>=1.7.24,<2.0.0)
 Requires-Dist: nb-cli (>=1.2.0) ; extra == "cli"
-Requires-Dist: nonebot-plugin-access-control-api (>=1.1.2,<2.0.0)
+Requires-Dist: nonebot-plugin-access-control-api (>=1.2.0,<2.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0)
 Requires-Dist: nonebot-plugin-datastore (>=1.0.0) ; extra == "migrate"
-Requires-Dist: nonebot-plugin-orm (>=0.5.0,<1.0.0)
-Requires-Dist: nonebot-plugin-session (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot2 (>=2.1.0,<3.0.0)
+Requires-Dist: nonebot-plugin-orm (>=0.7.0,<1.0.0)
+Requires-Dist: nonebot-plugin-session (>=0.3.0,<0.4.0)
+Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pytimeparser (>=0.2.0,<0.3.0)
 Requires-Dist: shortuuid (>=1.0.11,<2.0.0)
-Requires-Dist: ssttkkl-nonebot-utils (>=0.1.17)
 Project-URL: Repository, https://github.com/bot-ssttkkl/nonebot-plugin-access-control
 Description-Content-Type: text/plain
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 1.1.5a1
+Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 1.2.0
 Summary: Home-page: https://github.com/bot-ssttkkl/nonebot-plugin-access-
 control License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Provides-Extra: cli
-Provides-Extra: migrate Requires-Dist: arclet-alconna (>=1.7.24,<2.0.0)
-Requires-Dist: nb-cli (>=1.2.0) ; extra == "cli" Requires-Dist: nonebot-plugin-
-access-control-api (>=1.1.2,<2.0.0) Requires-Dist: nonebot-plugin-apscheduler
-(>=0.3.0) Requires-Dist: nonebot-plugin-datastore (>=1.0.0) ; extra ==
-"migrate" Requires-Dist: nonebot-plugin-orm (>=0.5.0,<1.0.0) Requires-Dist:
-nonebot-plugin-session (>=0.2.0,<0.3.0) Requires-Dist: nonebot2
-(>=2.1.0,<3.0.0) Requires-Dist: pytimeparser (>=0.2.0,<0.3.0) Requires-Dist:
-shortuuid (>=1.0.11,<2.0.0) Requires-Dist: ssttkkl-nonebot-utils (>=0.1.17)
-Project-URL: Repository, https://github.com/bot-ssttkkl/nonebot-plugin-access-
-control Description-Content-Type: text/plain
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Provides-Extra: cli Provides-Extra: migrate
+Requires-Dist: arclet-alconna (>=1.7.24,<2.0.0) Requires-Dist: nb-cli (>=1.2.0)
+; extra == "cli" Requires-Dist: nonebot-plugin-access-control-api
+(>=1.2.0,<2.0.0) Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0) Requires-
+Dist: nonebot-plugin-datastore (>=1.0.0) ; extra == "migrate" Requires-Dist:
+nonebot-plugin-orm (>=0.7.0,<1.0.0) Requires-Dist: nonebot-plugin-session
+(>=0.3.0,<0.4.0) Requires-Dist: nonebot2 (>=2.2.0,<3.0.0) Requires-Dist:
+pydantic-settings (>=2.2.1,<3.0.0) Requires-Dist: pytimeparser (>=0.2.0,<0.3.0)
+Requires-Dist: shortuuid (>=1.0.11,<2.0.0) Project-URL: Repository, https://
+github.com/bot-ssttkkl/nonebot-plugin-access-control Description-Content-Type:
+text/plain
                                    _[_n_o_n_e_b_o_t_]
 nonebot-plugin-access-control ============ _â¨ Nonebot æéæ§å¶æä»¶ â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ç¹ç¹ - åè½ - [x] æ¯æéå¯¹ç¨æ·/ç¾¤ç»çæéå¼å³ - [x]
 æ¯æéå¶åä¸ç¨æ·å¨ä¸å®æ¶é´åçæä»¤è°ç¨æ¬¡æ° - [x]
 å¯¹æªééæä»¶æä¾**æä»¶çº§å«**çæ§å¶æ¯æ - æä»¶éé - [x]
 æ¯æ**åè½çº§å«**çç»ç²åº¦æ§å¶ - [x]
```

