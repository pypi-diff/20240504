# Comparing `tmp/amazon-codewhisperer-jupyterlab-ext-2.0.0.tar.gz` & `tmp/amazon-codewhisperer-jupyterlab-ext-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-codewhisperer-jupyterlab-ext-2.0.0.tar", last modified: Tue Nov  7 21:32:47 2023, max compression
+gzip compressed data, was "amazon-codewhisperer-jupyterlab-ext-2.0.1.tar", last modified: Fri Dec  8 23:36:18 2023, max compression
```

## Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0.tar` & `amazon-codewhisperer-jupyterlab-ext-2.0.1.tar`

### file list

```diff
@@ -1,134 +1,142 @@
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.071473 amazon-codewhisperer-jupyterlab-ext-2.0.0/
--rw-r--r--   0 kumarnzt   (504) staff       (20)    11357 2023-10-10 20:51:22.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/LICENSE
--rw-r--r--   0 kumarnzt   (504) staff       (20)      103 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/NOTICE
--rw-r--r--   0 kumarnzt   (504) staff       (20)     5604 2023-11-07 21:32:47.071164 amazon-codewhisperer-jupyterlab-ext-2.0.0/PKG-INFO
--rw-r--r--   0 kumarnzt   (504) staff       (20)     4703 2023-11-07 04:22:49.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/README.md
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.945310 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     1039 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/__init__.py
--rw-r--r--   0 kumarnzt   (504) staff       (20)      443 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/_version.py
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.952452 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/auth/
--rw-r--r--   0 kumarnzt   (504) staff       (20)       98 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/auth/__init__.py
--rw-r--r--   0 kumarnzt   (504) staff       (20)     3422 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/auth/sso_auth_manager.py
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.953487 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/
--rw-r--r--   0 kumarnzt   (504) staff       (20)        0 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/__init__.py
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.983489 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/
--rw-r--r--   0 kumarnzt   (504) staff       (20)      281 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/__init__.py
--rw-r--r--   0 kumarnzt   (504) staff       (20)     1277 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/client_manager.py
--rw-r--r--   0 kumarnzt   (504) staff       (20)      794 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/iam_client_manager.py
--rw-r--r--   0 kumarnzt   (504) staff       (20)     1395 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/sso_client_manager.py
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.909762 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.908818 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.984200 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/
--rw-r--r--   0 kumarnzt   (504) staff       (20)    15547 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/service-2.json
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.909307 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.984899 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/
--rw-r--r--   0 kumarnzt   (504) staff       (20)    24832 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/service-2.json
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.910008 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.986055 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     4536 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/service-2.json
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.987290 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/telemetry/
--rw-r--r--   0 kumarnzt   (504) staff       (20)       72 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/telemetry/__init__.py
--rw-r--r--   0 kumarnzt   (504) staff       (20)     3653 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py
--rw-r--r--   0 kumarnzt   (504) staff       (20)     1879 2023-10-30 23:26:48.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/constants.py
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.988470 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/env/
--rw-r--r--   0 kumarnzt   (504) staff       (20)       64 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/env/__init__.py
--rw-r--r--   0 kumarnzt   (504) staff       (20)     2097 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/env/environment.py
--rw-r--r--   0 kumarnzt   (504) staff       (20)     7057 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/handlers.py
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.989036 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     5727 2023-11-07 21:32:43.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/package.json
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.929405 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.990241 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     2263 2023-11-07 21:32:41.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json
--rw-r--r--   0 kumarnzt   (504) staff       (20)     5585 2023-11-07 21:32:41.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.994028 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     6604 2023-11-07 21:32:43.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/571.2ac5bdb342624f52bccb.js
--rw-r--r--   0 kumarnzt   (504) staff       (20)    70257 2023-11-07 21:32:43.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/706.92fee206ef596946b068.js
--rw-r--r--   0 kumarnzt   (504) staff       (20)      368 2023-11-07 21:32:43.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/706.92fee206ef596946b068.js.LICENSE.txt
--rw-r--r--   0 kumarnzt   (504) staff       (20)     6544 2023-11-07 21:32:43.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/747.a6f42e6a863d7358a568.js
--rw-r--r--   0 kumarnzt   (504) staff       (20)     8339 2023-11-07 21:32:43.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.25e2176ddc0e279b9e44.js
--rw-r--r--   0 kumarnzt   (504) staff       (20)      178 2023-11-07 21:32:41.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/style.js
--rw-r--r--   0 kumarnzt   (504) staff       (20)     5075 2023-11-07 21:32:43.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json
--rw-r--r--   0 kumarnzt   (504) staff       (20)     2715 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/utils.py
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.995492 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/validator/
--rw-r--r--   0 kumarnzt   (504) staff       (20)       67 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/validator/__init__.py
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.996124 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/validator/schemas/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     1286 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json
--rw-r--r--   0 kumarnzt   (504) staff       (20)      782 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/validator/validator.py
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.950645 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext.egg-info/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     5604 2023-11-07 21:32:46.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO
--rw-r--r--   0 kumarnzt   (504) staff       (20)     4028 2023-11-07 21:32:46.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt
--rw-r--r--   0 kumarnzt   (504) staff       (20)        1 2023-11-07 21:32:46.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext.egg-info/dependency_links.txt
--rw-r--r--   0 kumarnzt   (504) staff       (20)        1 2023-10-06 21:32:52.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext.egg-info/not-zip-safe
--rw-r--r--   0 kumarnzt   (504) staff       (20)       36 2023-11-07 21:32:46.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext.egg-info/requires.txt
--rw-r--r--   0 kumarnzt   (504) staff       (20)       36 2023-11-07 21:32:46.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext.egg-info/top_level.txt
--rw-r--r--   0 kumarnzt   (504) staff       (20)      231 2023-10-10 18:39:10.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/install.json
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.930672 amazon-codewhisperer-jupyterlab-ext-2.0.0/jupyter-config/
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:46.996887 amazon-codewhisperer-jupyterlab-ext-2.0.0/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 kumarnzt   (504) staff       (20)      119 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/jupyter-config/jupyter_server_config.d/amazon_codewhisperer_jupyterlab_ext.json
--rw-r--r--   0 kumarnzt   (504) staff       (20)     5585 2023-11-07 03:43:05.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/package.json
--rw-r--r--   0 kumarnzt   (504) staff       (20)      675 2023-11-03 20:43:08.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/pyproject.toml
--rw-r--r--   0 kumarnzt   (504) staff       (20)       38 2023-11-07 21:32:47.071598 amazon-codewhisperer-jupyterlab-ext-2.0.0/setup.cfg
--rw-r--r--   0 kumarnzt   (504) staff       (20)     2931 2023-11-06 21:43:05.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/setup.py
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.001313 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.002068 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/__tests__/
--rw-r--r--   0 kumarnzt   (504) staff       (20)      109 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/__tests__/index.spec.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)     3183 2023-10-28 00:13:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/application.ts
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.002826 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/auth/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     9594 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/auth/authManager.tsx
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.004568 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/aws_vector_consolas_jupyter_lab3_extension/
--rw-r--r--   0 kumarnzt   (504) staff       (20)       28 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/aws_vector_consolas_jupyter_lab3_extension/__init__.py
--rw-r--r--   0 kumarnzt   (504) staff       (20)       58 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/aws_vector_consolas_jupyter_lab3_extension/py.typed
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.007268 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/client/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     1811 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/client/apiclient.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)    15283 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/client/codewhispererclient.d.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)     7900 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/client/codewhispereruserclient.d.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)     1225 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/handler.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)     2444 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/icons.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)    10530 2023-10-30 23:26:48.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/index.ts
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.007985 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/inline/
--rw-r--r--   0 kumarnzt   (504) staff       (20)    24845 2023-10-30 23:26:48.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/inline/inline.ts
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.008787 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/keybindings/
--rw-r--r--   0 kumarnzt   (504) staff       (20)      937 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/keybindings/keybindings.ts
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.009537 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/logging/
--rw-r--r--   0 kumarnzt   (504) staff       (20)      524 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/logging/logger.tsx
--rw-r--r--   0 kumarnzt   (504) staff       (20)      127 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/messages.ts
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.010100 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/notifications/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     3833 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/notifications/notifications.tsx
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.011959 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/recommendation/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     4733 2023-10-12 23:56:21.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/recommendation/extractor.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)    11212 2023-10-12 23:51:48.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/recommendation/recommendationStateHandler.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)    10893 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/recommendation/worker.ts
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.012667 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/referencetracker/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     3067 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/referencetracker/referencetracker.tsx
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.013483 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/statusbar/
--rw-r--r--   0 kumarnzt   (504) staff       (20)    18359 2023-10-28 00:13:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/statusbar/statusbarwidget.tsx
--rw-r--r--   0 kumarnzt   (504) staff       (20)       78 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/svg.d.ts
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.015611 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/telemetry/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     4333 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/telemetry/clienttelemetry.d.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)   150822 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/telemetry/telemetry.gen.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)     4381 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/telemetry/telemetry.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)      899 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/telemetry/telemetryClient.ts
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.017895 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/utils/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     3386 2023-10-28 00:13:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/utils/constants.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)      359 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/utils/licenseUtils.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)     1135 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/utils/models.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)      292 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/utils/stateKeys.ts
--rw-r--r--   0 kumarnzt   (504) staff       (20)     2974 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/src/utils/utils.ts
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.019437 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     2510 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/base.css
-drwxr-xr-x   0 kumarnzt   (504) staff       (20)        0 2023-11-07 21:32:47.070615 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/
--rw-r--r--   0 kumarnzt   (504) staff       (20)     3451 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/codewhisperer.svg
--rw-r--r--   0 kumarnzt   (504) staff       (20)      234 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/connected.svg
--rw-r--r--   0 kumarnzt   (504) staff       (20)      767 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/disconnected.svg
--rw-r--r--   0 kumarnzt   (504) staff       (20)      222 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/documentation.svg
--rw-r--r--   0 kumarnzt   (504) staff       (20)      234 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/loading.svg
--rw-r--r--   0 kumarnzt   (504) staff       (20)      746 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/log.svg
--rw-r--r--   0 kumarnzt   (504) staff       (20)      420 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/pause.svg
--rw-r--r--   0 kumarnzt   (504) staff       (20)      463 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/resume.svg
--rw-r--r--   0 kumarnzt   (504) staff       (20)      660 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/signout.svg
--rw-r--r--   0 kumarnzt   (504) staff       (20)      379 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/start.svg
--rw-r--r--   0 kumarnzt   (504) staff       (20)      599 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/visual-cue-arrow.svg
--rw-r--r--   0 kumarnzt   (504) staff       (20)       25 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/index.css
--rw-r--r--   0 kumarnzt   (504) staff       (20)       21 2023-10-06 21:27:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/style/index.js
--rw-r--r--   0 kumarnzt   (504) staff       (20)      656 2023-10-28 00:13:37.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/tsconfig.json
--rw-r--r--   0 kumarnzt   (504) staff       (20)       80 2023-10-10 21:39:58.000000 amazon-codewhisperer-jupyterlab-ext-2.0.0/tsconfig.test.json
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.345241 amazon-codewhisperer-jupyterlab-ext-2.0.1/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)    11357 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/LICENSE
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      527 2023-12-08 23:35:39.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/MANIFEST.in
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      103 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/NOTICE
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     5828 2023-12-08 23:36:18.344352 amazon-codewhisperer-jupyterlab-ext-2.0.1/PKG-INFO
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     4821 2023-12-08 09:51:30.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/README.md
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.228458 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     1005 2023-12-08 20:53:30.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/__init__.py
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.239543 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/auth/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       98 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/auth/__init__.py
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     4222 2023-12-08 10:41:09.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/auth/sso_auth_manager.py
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.240887 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)        0 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/__init__.py
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.245015 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      281 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/__init__.py
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     1675 2023-12-08 10:30:54.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/client_manager.py
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     1110 2023-12-08 10:33:06.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/iam_client_manager.py
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     1724 2023-12-08 10:34:38.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/sso_client_manager.py
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.194885 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.193251 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.246203 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)    15547 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/service-2.json
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.194270 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.247176 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)    24832 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/service-2.json
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.195703 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.249098 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     4536 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/service-2.json
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.250954 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/telemetry/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       72 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/telemetry/__init__.py
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     4422 2023-12-08 10:38:25.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     2069 2023-12-08 09:51:30.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/constants.py
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.253918 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/env/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       64 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/env/__init__.py
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     2647 2023-12-08 10:39:15.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/env/environment.py
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     7258 2023-12-08 10:25:53.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/handlers.py
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.255267 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     5727 2023-12-08 23:36:02.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/package.json
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.198898 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.257545 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     2263 2023-12-08 23:36:00.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     5585 2023-12-08 23:36:00.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.265111 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     6604 2023-12-08 23:36:02.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/571.2ac5bdb342624f52bccb.js
+-rw-r--r--   0 yuxqiang   (504) staff       (20)    70258 2023-12-08 23:36:02.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/706.cbd5c24bed652ef332fb.js
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      368 2023-12-08 23:36:02.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/706.cbd5c24bed652ef332fb.js.LICENSE.txt
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     6544 2023-12-08 23:36:02.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/747.a6f42e6a863d7358a568.js
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     8341 2023-12-08 23:36:02.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.210c5ddb098daa585d05.js
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      178 2023-12-08 23:36:00.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/style.js
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     5075 2023-12-08 23:36:02.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     3122 2023-12-08 09:51:30.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/utils.py
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.266618 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/validator/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       67 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/validator/__init__.py
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.267423 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/validator/schemas/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     1286 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      782 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/validator/validator.py
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.234990 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     5828 2023-12-08 23:36:17.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     4187 2023-12-08 23:36:18.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 yuxqiang   (504) staff       (20)        1 2023-12-08 23:36:17.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 yuxqiang   (504) staff       (20)        1 2023-12-08 21:10:47.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/not-zip-safe
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       48 2023-12-08 23:36:17.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/requires.txt
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       36 2023-12-08 23:36:17.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/top_level.txt
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      231 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/install.json
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.201184 amazon-codewhisperer-jupyterlab-ext-2.0.1/jupyter-config/
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.268229 amazon-codewhisperer-jupyterlab-ext-2.0.1/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      119 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/jupyter-config/jupyter_server_config.d/amazon_codewhisperer_jupyterlab_ext.json
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     5585 2023-12-08 09:56:34.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/package.json
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      675 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/pyproject.toml
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       38 2023-12-08 23:36:18.345413 amazon-codewhisperer-jupyterlab-ext-2.0.1/setup.cfg
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     2954 2023-12-08 21:10:12.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/setup.py
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.276636 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.278825 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/__tests__/
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.282924 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/__tests__/autotrigger/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     1844 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/__tests__/autotrigger/autotrigger.spec.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      109 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/__tests__/index.spec.ts
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.285360 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/__tests__/recommendation/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     5255 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/__tests__/recommendation/recommendationStateHandler.spec.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     3183 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/application.ts
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.286553 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/auth/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     9594 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/auth/authManager.tsx
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.287521 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/autotrigger/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     6602 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/autotrigger/autotrigger.ts
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.289532 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/aws_vector_consolas_jupyter_lab3_extension/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       28 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/aws_vector_consolas_jupyter_lab3_extension/__init__.py
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       58 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/aws_vector_consolas_jupyter_lab3_extension/py.typed
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.292448 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/client/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     1811 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/client/apiclient.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)    15283 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/client/codewhispererclient.d.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     7900 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/client/codewhispereruserclient.d.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     1225 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/handler.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     2444 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/icons.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)    10530 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/index.ts
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.296802 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/inline/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)    24845 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/inline/inline.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      885 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/inline/inlinePlugin.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     1514 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/inline/inlineWidget.ts
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.297758 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/keybindings/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      937 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/keybindings/keybindings.ts
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.301526 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/logging/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      524 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/logging/logger.tsx
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      127 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/messages.ts
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.302652 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/notifications/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     3833 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/notifications/notifications.tsx
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.306114 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/recommendation/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     4733 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/recommendation/extractor.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)    11212 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/recommendation/recommendationStateHandler.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)    10893 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/recommendation/worker.ts
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.307233 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/referencetracker/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     3067 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/referencetracker/referencetracker.tsx
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.308951 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/statusbar/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)    18359 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/statusbar/statusbarwidget.tsx
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       78 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/svg.d.ts
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.316040 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/telemetry/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     4333 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/telemetry/clienttelemetry.d.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)   150822 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/telemetry/telemetry.gen.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     4381 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/telemetry/telemetry.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      899 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/telemetry/telemetryClient.ts
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.321995 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/utils/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     3386 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/utils/constants.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      359 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/utils/licenseUtils.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     1135 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/utils/models.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      292 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/utils/stateKeys.ts
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     2974 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/src/utils/utils.ts
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.325810 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     2510 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/base.css
+drwxr-xr-x   0 yuxqiang   (504) staff       (20)        0 2023-12-08 23:36:18.342385 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/
+-rw-r--r--   0 yuxqiang   (504) staff       (20)     3451 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/codewhisperer.svg
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      234 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/connected.svg
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      767 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/disconnected.svg
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      222 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/documentation.svg
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      234 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/loading.svg
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      746 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/log.svg
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      420 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/pause.svg
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      463 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/resume.svg
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      660 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/signout.svg
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      379 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/start.svg
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      599 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/visual-cue-arrow.svg
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       25 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/index.css
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       21 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/style/index.js
+-rw-r--r--   0 yuxqiang   (504) staff       (20)      656 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/tsconfig.json
+-rw-r--r--   0 yuxqiang   (504) staff       (20)       80 2023-11-22 01:42:40.000000 amazon-codewhisperer-jupyterlab-ext-2.0.1/tsconfig.test.json
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/LICENSE` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/PKG-INFO` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-codewhisperer-jupyterlab-ext
-Version: 2.0.0
+Version: 2.0.1
 Summary: Amazon CodeWhisperer for JupyterLab
 Home-page: https://aws.amazon.com/codewhisperer/
 Author: Amazon CodeWhisperer
 Author-email: codewhisperer@amazon.com
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab4,Amazon CodeWhisperer,CodeWhisperer,Code,Whisperer
 Platform: Linux
@@ -18,14 +18,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Jupyter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: boto3
+Requires-Dist: botocore
+Requires-Dist: aiobotocore
+Requires-Dist: jupyterlab<5.0,>=4.0
 
 # Amazon CodeWhisperer for JupyterLab
 
 Amazon CodeWhisperer is an AI coding companion which provides developers with real-time code suggestions in JupyterLab. Individual developers can use CodeWhisperer for free in JupyterLab and AWS SageMaker Studio.
 
 ![Codewhisperer demo](https://docs.aws.amazon.com/images/codewhisperer/latest/userguide/images/codewhisperer-timestamp-record.png)
 
@@ -111,11 +115,13 @@
 
 * [CodeWhisperer User Guide](https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html)
 * [Setting up Amazon CodeWhisperer with JupyterLab](https://docs.aws.amazon.com/codewhisperer/latest/userguide/jupyterlab-setup.html)
 * [Setting up CodeWhisperer with Amazon SageMaker Studio](https://docs.aws.amazon.com/codewhisperer/latest/userguide/sagemaker-setup.html)
 
 ## Change Log
 
+2.0.1
+* Improved handling when Jupyter has no access to internet.
+* Migrated network call to be made asynchronously.
+
 2.0.0
 * Initial release - Adoption of JupyterLab 4
-
-
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/README.md` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,9 +86,13 @@
 
 * [CodeWhisperer User Guide](https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html)
 * [Setting up Amazon CodeWhisperer with JupyterLab](https://docs.aws.amazon.com/codewhisperer/latest/userguide/jupyterlab-setup.html)
 * [Setting up CodeWhisperer with Amazon SageMaker Studio](https://docs.aws.amazon.com/codewhisperer/latest/userguide/sagemaker-setup.html)
 
 ## Change Log
 
+2.0.1
+* Improved handling when Jupyter has no access to internet.
+* Migrated network call to be made asynchronously.
+
 2.0.0
 * Initial release - Adoption of JupyterLab 4
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/__init__.py` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 from pathlib import Path
 
 from .handlers import setup_handlers
-from ._version import __version__
 
 HERE = Path(__file__).parent.resolve()
 
 with (HERE / "labextension" / "package.json").open() as fid:
     data = json.load(fid)
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/sso_client_manager.py` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/sso_client_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from abc import ABC
-from botocore import UNSIGNED
-from botocore.client import Config
+from botocore import UNSIGNED, client
 from amazon_codewhisperer_jupyterlab_ext.client.codewhisperer.client_manager import CodeWhispererClientManager
 from amazon_codewhisperer_jupyterlab_ext.constants import (
     REQUEST_OPTOUT_HEADER_NAME,
     RTS_PROD_ENDPOINT,
     RTS_PROD_REGION,
     BEARER
 )
@@ -13,30 +12,39 @@
 class CodeWhispererSsoClientManager(CodeWhispererClientManager, ABC):
     _initialized = False
 
     def __init__(self):
         if self._initialized:
             return
         self._initialized = True
-
-        super().__init__()
         self._bearer_token = ""
         self._opt_out = False
-        self._client = self.session.client(
-            service_name=BEARER,
-            endpoint_url=RTS_PROD_ENDPOINT,
-            region_name=RTS_PROD_REGION,
-            config=Config(signature_version=UNSIGNED),
+        self.cfg = client.Config(
+            connect_timeout=self.CONNECT_TIMEOUT_IN_SEC,
+            read_timeout=self.READ_TIMEOUT_IN_SEC,
+            retries={"total_max_attempts": 2},
+            tcp_keepalive=True,
+            signature_version=UNSIGNED
         )
-
-        self._client.meta.events.register_first("before-sign.*.*", self._add_header)
+        super().__init__()
 
     def _add_header(self, request, **kwargs):
         request.headers.add_header("Authorization", "Bearer " + self._bearer_token)
         request.headers.add_header(REQUEST_OPTOUT_HEADER_NAME, f"{self._opt_out}")
 
-    def invoke_recommendations(self, request, opt_out):
+    def get_client(self):
+        return self.session.create_client(
+            service_name=BEARER,
+            endpoint_url=RTS_PROD_ENDPOINT,
+            region_name=RTS_PROD_REGION,
+            verify=False,
+            config=self.cfg
+        )
+
+    async def invoke_recommendations(self, request, opt_out):
         self._opt_out = opt_out
-        return self.get_client().generate_completions(**request)
+        async with self.get_client() as sso_client:
+            sso_client.meta.events.register_first("before-sign.*.*", self._add_header)
+            return await sso_client.generate_completions(**request)
 
     def set_bearer_token(self, token):
         self._bearer_token = token
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/service-2.json` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/service-2.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/service-2.json` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/service-2.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/service-2.json` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/service-2.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,107 @@
-import boto3
 import logging
+
+from aiobotocore.session import get_session
+from botocore import client
 from botocore.exceptions import ClientError
 from pathlib import Path
 from amazon_codewhisperer_jupyterlab_ext.constants import (
     PROD_COGNITO_POOL_ID,
     INVALID_TOKEN_EXCEPTION_MESSAGE,
     TELEMETRY_PROD_ENDPOINT,
     PostMetricsRequestConstants,
 )
 
 logging.basicConfig(format="%(levelname)s: %(message)s")
-session = boto3.Session()
 
 
 class ToolkitTelemetry:
+
+    READ_TIMEOUT_IN_SEC = 15
+    CONNECT_TIMEOUT_IN_SEC = 5
+    _credentials = None
+
     def __init__(self):
-        self.session = None
-    
-    def _setup_telemetry_client(self):
-        self.session = boto3.Session()
-        session_folder =  f"{Path(__file__).parent.parent}/service_models"
-        self.session._loader.search_paths.append(session_folder)
-        self.cognito_client = boto3.client("cognito-identity", region_name="us-east-1")
-        self.identity_id = self.cognito_client.get_id(
-            IdentityPoolId=PROD_COGNITO_POOL_ID
-        )["IdentityId"]
-        credentials = self.cognito_client.get_credentials_for_identity(
-            IdentityId=self.identity_id
-        )["Credentials"]
-        self.telemetry_client = self.session.client(
-            "telemetry",
+        self.identity_id = None
+        self.session = get_session()
+        self.cfg = client.Config(
+            connect_timeout=self.CONNECT_TIMEOUT_IN_SEC,
+            read_timeout=self.READ_TIMEOUT_IN_SEC,
+            retries={"total_max_attempts": 2},
+        )
+        session_folder = f"{Path(__file__).parent.parent}/service_models"
+        self.session.get_component('data_loader').search_paths.append(session_folder)
+
+    def _get_cognito_client(self):
+        return self.session.create_client(
+            service_name="cognito-identity",
+            region_name="us-east-1",
+            config=self.cfg,
+        )
+
+    def _get_telemetry_client(self):
+        return self.session.create_client(
+            service_name="telemetry",
             region_name="us-east-1",
             endpoint_url=TELEMETRY_PROD_ENDPOINT,
-            aws_access_key_id=credentials["AccessKeyId"],
-            aws_secret_access_key=credentials["SecretKey"],
-            aws_session_token=credentials["SessionToken"],
+            aws_access_key_id=self._credentials["AccessKeyId"],
+            aws_secret_access_key=self._credentials["SecretKey"],
+            aws_session_token=self._credentials["SessionToken"],
+            config=self.cfg,
         )
 
-        self.credential_expire_time = credentials["Expiration"]
+    async def _setup_credentials(self):
+        async with self._get_cognito_client() as cognito_client:
+            self.identity_id = (await cognito_client.get_id(
+                IdentityPoolId=PROD_COGNITO_POOL_ID
+            ))["IdentityId"]
+            self._credentials = (await cognito_client.get_credentials_for_identity(
+                IdentityId=self.identity_id
+            ))["Credentials"]
 
+        self.credential_expire_time = self._credentials["Expiration"]
 
-    def post_metrics(self, request, parent_product):
-        if self.session is None:
-            self._setup_telemetry_client()
-        logging.info(request["ClientID"])
-        logging.info(request["MetricData"][0]["EpochTimestamp"])
+    async def post_metrics(self, request, parent_product):
         try:
-            self.telemetry_client.post_metrics(
-                AWSProduct=request[PostMetricsRequestConstants.AWS_PRODUCT],
-                AWSProductVersion=request[
-                    PostMetricsRequestConstants.AWS_PRODUCT_VERSION
-                ],
-                ClientID=request[PostMetricsRequestConstants.CLIENT_ID],
-                MetricData=request[PostMetricsRequestConstants.METRIC_DATA],
-                ParentProduct=parent_product,
-            )
-        except ClientError as e:
-            if INVALID_TOKEN_EXCEPTION_MESSAGE in e.response["Error"]["Message"]:
-                logging.info("refreshing credentials")
-                self._refresh_credentials()
-                self.telemetry_client.post_metrics(
+            if not self._credentials:
+                await self._setup_credentials()
+            logging.info(request["ClientID"])
+            logging.info(request["MetricData"][0]["EpochTimestamp"])
+            async with self._get_telemetry_client() as telemetry_client:
+                await telemetry_client.post_metrics(
                     AWSProduct=request[PostMetricsRequestConstants.AWS_PRODUCT],
                     AWSProductVersion=request[
                         PostMetricsRequestConstants.AWS_PRODUCT_VERSION
                     ],
                     ClientID=request[PostMetricsRequestConstants.CLIENT_ID],
                     MetricData=request[PostMetricsRequestConstants.METRIC_DATA],
                     ParentProduct=parent_product,
                 )
+            logging.info("sent telemetry")
+        except ClientError as e:
+            if INVALID_TOKEN_EXCEPTION_MESSAGE in e.response["Error"]["Message"]:
+                logging.info("refreshing credentials")
+                await self._refresh_credentials()
+                async with self._get_telemetry_client() as telemetry_client:
+                    await telemetry_client.post_metrics(
+                        AWSProduct=request[PostMetricsRequestConstants.AWS_PRODUCT],
+                        AWSProductVersion=request[
+                            PostMetricsRequestConstants.AWS_PRODUCT_VERSION
+                        ],
+                        ClientID=request[PostMetricsRequestConstants.CLIENT_ID],
+                        MetricData=request[PostMetricsRequestConstants.METRIC_DATA],
+                        ParentProduct=parent_product,
+                    )
             else:
                 logging.error(e.response["Error"]["Message"])
                 return
+        except Exception as e:
+            logging.warning(f"Logging telemetry error and ignoring exception {e}", exc_info=True)
 
-        logging.info("sent telemetry")
-
-    def _refresh_credentials(self):
-        credentials = self.cognito_client.get_credentials_for_identity(
-            IdentityId=self.identity_id
-        )["Credentials"]
-        self.telemetry_client = self.session.client(
-            "telemetry",
-            region_name="us-east-1",
-            endpoint_url=TELEMETRY_PROD_ENDPOINT,
-            aws_access_key_id=credentials["AccessKeyId"],
-            aws_secret_access_key=credentials["SecretKey"],
-            aws_session_token=credentials["SessionToken"],
-        )
+    async def _refresh_credentials(self):
+        async with self._get_cognito_client() as cognito_client:
+            self._credentials = (await cognito_client.get_credentials_for_identity(
+                IdentityId=self.identity_id
+            ))["Credentials"]
 
-        ## TODO: can use expire time to refresh
+        # TODO: can use expire time to refresh
         # self.credential_expire_time = credentials["Expiration"]
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/constants.py` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CURRENT_VERSION = "2.0.0"
+CURRENT_VERSION = "2.0.1"
 CODEWHISPERER_PYPI_JSON_URL = "https://pypi.org/pypi/amazon-codewhisperer-jupyterlab-ext/json"
 
 TELEMETRY_PROD_ENDPOINT = "https://client-telemetry.us-east-1.amazonaws.com"
 PROD_COGNITO_POOL_ID = "us-east-1:820fd6d1-95c0-4ca4-bffb-3f01d32da842"
 
 INVALID_TOKEN_EXCEPTION_MESSAGE = "The security token included in the request is expired"
 RTS_PROD_ENDPOINT = "https://codewhisperer.us-east-1.amazonaws.com/"
@@ -24,14 +24,15 @@
 
 # TODO: add more mapping from a specific (error_code, error_message) combo to a user-friendly error message
 ERROR_CODE_TO_USER_MESSAGE_MAP = {
     'InvalidGrantException: Invalid grant provided': 'InvalidGrantException: Login failed. Try login again later.'
 }
 
 NEW_VERSION_USER_MESSAGE = "New version of Amazon CodeWhisperer -  v{} is available! Update now to enjoy the latest features and improvements."
+SAGEMAKER_CONNECT_ERROR = "Cannot connect to CodeWhisperer services, please make sure that the domain has internet access or a VPC Endpoint for AWS CodeWhisperer if using a VPCOnly domain."
 
 START_URL = "https://view.awsapps.com/start"
 SSO_OIDC = "sso-oidc"
 OIDC_BUILDER_ID_ENDPOINT = "https://oidc.us-east-1.amazonaws.com"
 OIDC_BUILDER_ID_REGION = "us-east-1"
 SCOPES = ["codewhisperer:completions"]
 CLIENT_NAME = "CodeWhisperer for JupyterLab"
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/env/environment.py` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/env/environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 import json
 import os
+
+import aiohttp
 import requests
+from aiohttp import ClientTimeout
 from packaging.version import Version
 from amazon_codewhisperer_jupyterlab_ext.constants import CURRENT_VERSION, CODEWHISPERER_PYPI_JSON_URL, \
     NEW_VERSION_USER_MESSAGE, CONSUMER_ENV_KEY, CONSUMER_ENV_VALUE_GLUE_STUDIO
 
 
 class Environment:
     SM_STUDIO = "SageMaker Studio"
     JUPYTER_OSS = "Jupyter OSS"
     GLUE_STUDIO_NOTEBOOK = "Glue Studio Notebook"
 
     @staticmethod
-    def get_update_notification():
+    async def get_update_notification():
         try:
             # Glue Studio environment doesn't want any update and update notification
-            if Environment.is_glue_studio():
+            if Environment.is_glue_studio() or Environment.is_sm_studio():
                 return "", ""
 
             # Get the URL from environment variable or fall back to default
             url = os.environ.get("JSON_URL", CODEWHISPERER_PYPI_JSON_URL)
 
             # Download the JSON data
-            response = requests.get(url)
-            response.raise_for_status()
-            data = response.json()
+            async with aiohttp.ClientSession() as session:
+                # Define the timeout duration (in seconds)
+                timeout_duration = 2  # Timeout after 2 seconds
+
+                # Create a ClientTimeout object
+                timeout = ClientTimeout(total=timeout_duration)
+
+                async with session.get(url, timeout=timeout) as response:
+                    response.raise_for_status()
+                    data = await response.json()
 
             # Get the latest version and launch date
             latest_version = data["info"]["version"]
 
             # Compare the current version with the latest version
             if Version(latest_version) > Version(CURRENT_VERSION):
                 return NEW_VERSION_USER_MESSAGE.format(latest_version), latest_version
@@ -53,7 +63,11 @@
             # Default to Builder ID / Jupyter OSS for all errors
             pass
         return env
 
     @staticmethod
     def is_glue_studio():
         return CONSUMER_ENV_KEY in os.environ and os.environ.get(CONSUMER_ENV_KEY) == CONSUMER_ENV_VALUE_GLUE_STUDIO
+
+    @staticmethod
+    def is_sm_studio():
+        return Environment.get_environment() == Environment.SM_STUDIO
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/handlers.py` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,77 +28,77 @@
         environment = Environment.get_environment()
         self.input_validator = InputValidator()
         self.codewhisperer_client = CodeWhispererIamClientManager() \
             if environment != Environment.JUPYTER_OSS \
             else CodeWhispererSsoClientManager()
 
     @tornado.web.authenticated
-    def post(self):
+    async def post(self):
         input_data = self.get_json_body()
         try:
             if not self.input_validator.is_valid_input("generate_recommendations", input_data):
                 self.set_status(400)
-                self.finish(json.dumps({'success': False,  'message': 'Invalid input data.'}))
+                await self.finish(json.dumps({'success': False,  'message': 'Invalid input data.'}))
                 return
             token = self.request.headers['Token']
             opt_out = self.request.headers['OptOut']
             if token is not None and isinstance(self.codewhisperer_client, CodeWhispererSsoClientManager):
                 self.codewhisperer_client.set_bearer_token(token)
-            resp = self.codewhisperer_client.generate_recommendations(input_data, opt_out == 'True')
-            self.finish(json.dumps(resp.__dict__))
+            resp = await self.codewhisperer_client.generate_recommendations(input_data, opt_out == 'True')
+            await self.finish(json.dumps(resp.__dict__))
         except Exception as e:
+            logging.warning(f"Unexpected error while generating recommendations: {e}", exc_info=True)
             return_server_error(self)
 
 
 class RegisterClientHandler(APIHandler, ABC):
     @tornado.web.authenticated
-    def get(self):
+    async def get(self):
         try:
-            resp = authManager.register_client()
-            self.finish(json.dumps(resp.__dict__))
+            resp = await authManager.register_client()
+            await self.finish(json.dumps(resp.__dict__))
         except Exception as e:
             return_server_error(self)
 
 
 class DeviceAuthorizationHandler(APIHandler, ABC):
     @tornado.web.authenticated
-    def post(self):
+    async def post(self):
         try:
             input_data = self.get_json_body()
-            resp = authManager.device_authorization(input_data)
-            self.finish(json.dumps(resp.__dict__))
+            resp = await authManager.device_authorization(input_data)
+            await self.finish(json.dumps(resp.__dict__))
         except Exception as e:
             return_server_error(self)
 
 
 class CreateTokenHandler(APIHandler, ABC):
     @tornado.web.authenticated
-    @tornado.gen.coroutine
-    def post(self):
+    async def post(self):
         try:
             input_data = self.get_json_body()
-            resp = yield authManager.create_token(
+            resp = await authManager.create_token(
                 input_data['clientRegistration'],
                 input_data['deviceAuthorizationResponse']
             )
             if resp is None:
-                self.finish(json.dumps(resp))
+                await self.finish(json.dumps(resp))
             else:
-                self.finish(json.dumps(resp.__dict__))
+                await self.finish(json.dumps(resp.__dict__))
         except Exception as e:
             return_server_error(self)
 
 
 class RefreshHandler(APIHandler, ABC):
     @tornado.web.authenticated
-    def post(self):
+    async def post(self):
         try:
             input_data = self.get_json_body()
-            resp = authManager.refresh(input_data['clientRegistration'], input_data['token'])
-            self.finish(json.dumps(resp.__dict__))
+            resp = await authManager.refresh(input_data['clientRegistration'], input_data['token'])
+            await self.finish(json.dumps(resp.__dict__))
         except Exception as e:
             return_server_error(self)
 
 
 class CancelLoginHandler(APIHandler, ABC):
     @tornado.web.authenticated
     def get(self):
@@ -112,25 +112,25 @@
 class PostMetricsHandler(APIHandler, ABC):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         environment = Environment.get_environment()
         self.parent_product = environment
 
     @tornado.web.authenticated
-    def post(self):
+    async def post(self):
         input_data = self.get_json_body()
         logging.info("input data: ", input_data)
-        toolkit_telemetry_api.post_metrics(input_data, self.parent_product)
+        await toolkit_telemetry_api.post_metrics(input_data, self.parent_product)
 
 
 class GetEnvironmentHandler(APIHandler, ABC):
     @tornado.web.authenticated
-    def get(self):
-        update_notification, latest_version = Environment.get_update_notification()
-        self.finish(json.dumps(ServiceResponse(
+    async def get(self):
+        update_notification, latest_version = await Environment.get_update_notification()
+        await self.finish(json.dumps(ServiceResponse(
             ServiceResponseStatus.SUCCESS,
             {
                 'environment': Environment.get_environment(),
                 'version_notification': update_notification,
                 'latest_version': latest_version
             },
             None,
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/package.json` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.210c5ddb098daa585d05.js'}}",*

 * * "'version'": "'2.0.1'"}*

```diff
@@ -87,15 +87,15 @@
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/aws",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.25e2176ddc0e279b9e44.js",
+            "load": "static/remoteEntry.210c5ddb098daa585d05.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "amazon_codewhisperer_jupyterlab_ext/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -151,9 +151,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "2.0.1"
 }
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.0.1'"}*

```diff
@@ -146,9 +146,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "2.0.1"
 }
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/571.2ac5bdb342624f52bccb.js` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/571.2ac5bdb342624f52bccb.js`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/706.92fee206ef596946b068.js` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/706.cbd5c24bed652ef332fb.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,27 +1,27 @@
-/*! For license information please see 706.92fee206ef596946b068.js.LICENSE.txt */
+/*! For license information please see 706.cbd5c24bed652ef332fb.js.LICENSE.txt */
 "use strict";
 (self.webpackChunkamazon_codewhisperer_jupyterlab_ext = self.webpackChunkamazon_codewhisperer_jupyterlab_ext || []).push([
     [706], {
         706: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => be
             });
-            var i = n(408),
-                o = n(261),
-                s = n(684),
-                r = n(7),
-                a = n(260),
-                c = n(987),
+            var i = n(122),
+                o = n(977),
+                s = n(190),
+                r = n(10),
+                a = n(667),
+                c = n(527),
                 l = n(930),
-                d = n(981),
-                h = n(60),
-                g = n(614),
-                u = n(788),
-                p = n(861),
+                d = n(499),
+                h = n(454),
+                g = n(749),
+                u = n(125),
+                p = n(308),
                 m = n(862),
                 w = n.n(m);
             class v {
                 static getInstance(e) {
                     return v.parentLogger || (v.parentLogger = w()({
                         level: "error",
                         transport: {
@@ -170,15 +170,15 @@
                 }
                 async logout() {
                     await oe(k), await oe(I), this.authStateChangedSignal.emit(j.UNAUTHENTICATED)
                 }
             }! function(e) {
                 e[e.AUTHENTICATED = 0] = "AUTHENTICATED", e[e.UNAUTHENTICATED = 1] = "UNAUTHENTICATED", e[e.AUTHENTICATION_IN_PROGRESS = 2] = "AUTHENTICATION_IN_PROGRESS"
             }(j || (j = {}));
-            var O = n(800);
+            var O = n(85);
             class D {}
             D.visualCueArrowIcon = new O.LabIcon({
                 name: "visual-cue-arrow",
                 svgstr: '<?xml version="1.0" encoding="utf-8"?>\n\x3c!-- Generator: Adobe Illustrator 27.4.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  --\x3e\n<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"\n\t viewBox="0 0 17 17" style="enable-background:new 0 0 17 17;" xml:space="preserve">\n<circle class="jp-icon2" fill="#424242" cx="8.5" cy="8.5" r="8.5"/>\n<g>\n\t<path class="jp-icon-accent1" fill="#FFFFFF" d="M8.5,5.3L10.1,7l0.7-0.7L8.5,3.9L6.2,6.2L6.9,7L8.5,5.3z M8.5,11.7L6.9,10l-0.7,0.7l2.3,2.4l2.3-2.4L10.1,10\n\t\tL8.5,11.7z"/>\n</g>\n</svg>\n'
             }), D.logoIcon = new O.LabIcon({
                 name: "codewhisperer:logo",
                 svgstr: '<svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">\n<g clip-path="url(#clip0_6759_310550)">\n<path class="jp-icon3" fill-rule="evenodd" clip-rule="evenodd" d="M8.03734 8.48493L8.54502 8.66249L7.42349 11.9234L6.91581 11.7458L8.03734 8.48493ZM6.47451 9.33695L5.64888 10.1768L6.45811 11.015L6.07271 11.3934L5.07965 10.3644C4.97752 10.2584 4.97833 10.0892 5.08153 9.98431L6.09287 8.95526L6.47451 9.33695ZM10.468 9.98431C10.5712 10.0892 10.572 10.2584 10.4699 10.3644L9.47627 11.3934L9.09114 11.015L9.90037 10.1768L9.07502 9.33695L9.45665 8.95526L10.468 9.98431ZM12.3966 11.0874L11.4699 11.5544C11.3791 11.6005 11.3216 11.6943 11.3216 11.7971V13.4122L9.13979 14.7665L8.09646 14.1655V12.764H7.55895V14.1655L6.51563 14.7665L4.33384 13.4122V11.7968C4.33384 11.694 4.27633 11.6002 4.18522 11.5544L3.25881 11.0871L3.25854 10.0315L3.25881 8.84683L4.22795 8.10188C4.2946 8.05065 4.33384 7.97095 4.33384 7.88637V6.38022L6.33179 5.20479L7.55895 5.89579V7.61339H8.09646V5.89579L9.32335 5.20479L11.3216 6.38022V7.88637C11.3216 7.97095 11.3605 8.05065 11.4272 8.10188L12.3966 8.84656L12.3969 10.0315L12.3966 11.0874ZM12.8282 8.49686L11.8591 7.75191V6.22461C11.8591 6.12838 11.8083 6.03919 11.7258 5.9904L9.46176 4.65855C9.37952 4.61003 9.27793 4.60921 9.19542 4.65584L7.82771 5.42627L6.45999 4.65584C6.37695 4.60948 6.27562 4.61003 6.19365 4.65855L3.92963 5.9904C3.84685 6.03919 3.79632 6.12838 3.79632 6.22461V7.75218L2.82691 8.49686C2.76026 8.54809 2.72129 8.62806 2.72129 8.71264L2.72102 10.0315L2.72129 11.2546C2.72129 11.3574 2.7788 11.4512 2.86964 11.4972L3.79632 11.9643V13.5637C3.79632 13.6578 3.84443 13.7451 3.92398 13.7944L6.36969 15.3128C6.45327 15.3643 6.55809 15.3662 6.64382 15.3171L7.82771 14.6351L9.01132 15.3171C9.05271 15.341 9.09867 15.3529 9.14462 15.3529C9.19354 15.3529 9.24218 15.3393 9.28572 15.3128L11.7312 13.7944C11.8107 13.7451 11.8591 13.6578 11.8591 13.5637V11.9646L12.7855 11.4972C12.8766 11.4514 12.9341 11.3576 12.9341 11.2549L12.9344 10.0315L12.9341 8.71237C12.9341 8.62779 12.8949 8.54809 12.8282 8.49686ZM5.14012 1.78504C5.14012 2.0095 4.95951 2.19167 4.73698 2.19167C4.51418 2.19167 4.33384 2.0095 4.33384 1.78504C4.33384 1.56031 4.51418 1.37841 4.73698 1.37841C4.95951 1.37841 5.14012 1.56031 5.14012 1.78504ZM3.79632 1.78504C3.79632 2.0095 3.61572 2.19167 3.39319 2.19167C3.17039 2.19167 2.99005 2.0095 2.99005 1.78504C2.99005 1.56031 3.17039 1.37841 3.39319 1.37841C3.61572 1.37841 3.79632 1.56031 3.79632 1.78504ZM2.45253 1.78504C2.45253 2.0095 2.27192 2.19167 2.04939 2.19167C1.82659 2.19167 1.64625 2.0095 1.64625 1.78504C1.64625 1.56031 1.82659 1.37841 2.04939 1.37841C2.27192 1.37841 2.45253 1.56031 2.45253 1.78504ZM0.839978 2.73384L0.841322 0.86145C0.841322 0.849522 0.855297 0.836239 0.875185 0.836239H14.7816C14.8015 0.836239 14.8154 0.849522 14.8154 0.86145V2.73384H0.839978ZM14.7816 0.294067H0.873842C0.559394 0.294067 0.302998 0.548346 0.30246 0.860908L0.294129 10.8404C0.29386 11.1516 0.548643 11.4064 0.863897 11.4086L1.91501 11.408V10.8664L0.873304 10.8667C0.853685 10.8667 0.839978 10.8534 0.839978 10.8415L0.846159 3.27601H14.8154V10.8385C14.8154 10.8534 14.7998 10.8661 14.7816 10.8661L13.7404 10.8664V11.4086L14.7816 11.4083C15.0966 11.4083 15.353 11.1527 15.353 10.8385V0.86145C15.353 0.548617 15.0966 0.294067 14.7816 0.294067Z" fill="#616161"/>\n</g>\n<defs>\n<clipPath id="clip0_6759_310550">\n<rect width="16" height="16" fill="white"/>\n</clipPath>\n</defs>\n</svg>\n'
@@ -424,15 +424,15 @@
                     }
                     return t ? "Empty" : "Discard"
                 }
             }
             H = z, B = {
                 value: void 0
             };
-            var $ = n(141);
+            var $ = n(143);
             const G = "CodeWhisperer Reference Logs";
             class J {
                 static createInstance(e) {
                     return J.instance || (J.instance = new J(e)), J.instance
                 }
                 static getInstance() {
                     return J.instance
@@ -1606,11 +1606,11 @@
                 },
                 be = Ie
         },
         123: e => {
             e.exports = JSON.parse('{"codewhisperer_status_widget_text_not_authenticated":"CodeWhisperer","codewhisperer_status_widget_text_auth_in_progress":"CodeWhisperer(Connecting...)","codewhisperer_status_widget_text_authenticated":"CodeWhisperer","codewhisperer_start":"Start CodeWhisperer","codewhisperer_cancel_login":"Cancel Login","codewhisperer_learn_more":"Learn More","codewhisperer_update_now":"Update Now","codewhisperer_documentation_open":"Documentation","codewhisperer_pause_auto_suggestion":"Pause Auto-Suggestions","codewhisperer_resume_auto_suggestion":"Resume Auto-Suggestions","codewhisperer_reference_log_open":"Open Code Reference Log","codewhisperer_sign_out":"Sign Out","codewhisperer_toggle_telemetry":"Share telemetry with AWS","codewhisperer_toggle_code_references":"Code with references","codewhisperer_key_shortcut_title":"SHORTCUTS","codewhisperer_key_shortcut_accept":"Accept","codewhisperer_key_shortcut_manual_trigger":"Manual Invoke","codewhisperer_key_shortcut_navigate":"Navigate","codewhisperer_key_shortcut_reject":"Reject","codewhisperer_expiry_notification_message":"CodeWhisperer connection expired. Reauthenticate with AWS Builder ID to use CodeWhisperer.","codewhisperer_expiry_notification_button_authenticate":"Authenticate","codewhisperer_expiry_notification_button_cancel":"Cancel","codewhisperer_copy_code_and_proceed_dialog_title":"Start CodeWhisperer with AWS Builder ID","codewhisperer_copy_code_and_proceed_dialog_button_yes":"Copy Code and Proceed","codewhisperer_copy_code_and_proceed_dialog_message_first_li":"To use CodeWhisperer, individual developers must sign in using AWS Builder ID. ","codewhisperer_copy_code_and_proceed_dialog_message_first_li_learn_more":"Learn More","codewhisperer_copy_code_and_proceed_dialog_message_second_li":"A login page will open on an external website: https://device.sso.us-east-1.amazonaws.com","codewhisperer_copy_code_and_proceed_dialog_message_third_li":"Provide this code to confirm the access request: ","codewhisperer_server_extension_not_enabled_message":"CodeWhisperer isn\'t enabled. Run `jupyter server extension enable amazon_codewhisperer_jupyterlab_ext`, then restart server & refresh browser.","codewhisperer_update_notification_skip_this_version":"Skip this version","codewhisperer_notification_show_full_message_button_title":"Expand"}')
         },
         147: e => {
-            e.exports = JSON.parse('{"name":"amazon-codewhisperer-jupyterlab-ext","version":"2.0.0","description":"Amazon CodeWhisperer for JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","codewhisperer","amazon-codewhisperer"],"homepage":"https://github.com/aws","bugs":{"url":"https://aws.amazon.com/codewhisperer/","email":"codewhisperer@amazon.com"},"license":"Apache 2.0","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"author":{"name":"Amazon CodeWhisperer","email":"codewhisperer@amazon.com"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,eot,js,gif,html,jpg,json,png,svg,woff2,ttf}","style/img/*.{svg}","schema/*.json","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","config":{"vars":{"builddir":"./build/lib/amazon-codewhisperer-jupyterlab-ext","jupyterCorePath":"./build-tools/jupyter-staging"}},"npm-pretty-much":{"https://w/?NpmPrettyMuch/UndeclaredTransitiveDependencies":true,"legacyPackageNameAlias":"amazon-codewhisperer-jupyterlab-ext","npm-pretty-much":{"allowUnsafeName":"open source extension"},"runTest":"always","runRelease":"always"},"scripts":{"build":"npm run clean && npm run build:lib && npm run build:labextension","postbuild":"mkdir -p $npm_package_config_vars_builddir && rsync package.json $npm_package_config_vars_builddir && rsync -a --exclude={‘*.spec.d.ts’,’*.spec.js’} lib $npm_package_config_vars_builddir && rsync -a style $npm_package_config_vars_builddir","build:all":"npm run build:lib && npm run build:labextension","build:labextension":"build-labextension --core-path $npm_package_config_vars_jupyterCorePath .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:prod":"npm run clean && npm run build:lib && npm run build:labextension","clean":"npm run clean:lib","clean:all":"npm run clean:lib && npm run clean:labextension","clean:labextension":"rimraf amazon_codewhisperer_jupyterlab_ext/labextension","clean:lib":"rimraf lib tsconfig.tsbuildinfo","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"npm run build","dev":"npm run clean && npm run build:lib && npm run build:labextension:dev","dist":"python setup.py sdist","release":"npm run build && npm run postbuild && npm run dist","watch":"run-p watch:src watch:labextension","watch:labextension":"jupyter labextension watch .","watch:src":"tsc -w","generateTelemetry":"node node_modules/@aws-toolkits/telemetry/lib/generateTelemetry.js --output=src/telemetry/telemetry.gen.ts","generateClients":"ts-node ./scripts/build/generateServiceClient.ts ","test":"jest --no-cache"},"dependencies":{"@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.1.6","@jupyterlab/codeeditor":"^4.0.6","@jupyterlab/codemirror":"^4.0.6","@jupyterlab/completer":"^4.0.6","@jupyterlab/fileeditor":"^4.0.6","@jupyterlab/launcher":"^4.0.6","@jupyterlab/logconsole":"^4.0.6","@jupyterlab/nbformat":"^4.0.6","@jupyterlab/notebook":"^4.0.6","@jupyterlab/outputarea":"^4.0.6","@jupyterlab/rendermime":"^4.0.6","@jupyter/ydoc":"~1.0","@jupyterlab/settingregistry":"^4.0.6","@jupyterlab/statedb":"^4.0.6","@jupyterlab/translation":"^4.0.6","@lumino/algorithm":"^2.0.0","@lumino/coreutils":"^2.0.0","@lumino/datagrid":"^2.0.1","@lumino/disposable":"^2.0.0","aws-sdk":"^2.1267.0","pino":"^8.11.0"},"devDependencies":{"@codemirror/view":"^6.0.0","@codemirror/state":"^6.0.0","@aws-toolkits/telemetry":"^1.0.120","@babel/core":"^7.21.5","@babel/preset-env":"^7.21.5","@jupyterlab/builder":"^4.0.0","@jupyterlab/testutils":"^4.0.0","@types/codemirror":"^5.60.7","@types/fs-extra":"^9.0.11","@types/jest":"^29.2.0","@types/json-schema":"^7.0.11","@types/node":"^16.0.0","@types/react":"18.2.25","@types/react-addons-linked-state-mixin":"^0.14.22","@typescript-eslint/eslint-plugin":"^5.62.0","@typescript-eslint/parser":"^5.62.0","css-loader":"^6.7.1","eslint":"^8.36.0","eslint-config-prettier":"^8.8.0","eslint-plugin-jsdoc":"^40.0.0","eslint-plugin-prettier":"^5.0.0","eslint-plugin-react":"^7.18.3","jest":"^29.2.0","jest-environment-jsdom":"^29.7.0","jest-fetch-mock":"^1.6.6","mkdirp":"^1.0.3","npm-run-all":"^4.1.5","pino-pretty":"10.0.0","prettier":"^3.0.0","rimraf":"^5.0.1","source-map-loader":"^1.0.2","style-loader":"^3.3.1","stylelint":"^15.10.1","stylelint-config-recommended":"^13.0.0","stylelint-config-standard":"^34.0.0","stylelint-csstree-validator":"^3.0.0","stylelint-prettier":"^4.0.0","ts-jest":"^29.0.0","typescript":"~5.0.2","yjs":"^13.5.40"},"sideEffects":["style/*.css","style/index.js"],"jupyterlab":{"extension":true,"schemaDir":"schema","outputDir":"amazon_codewhisperer_jupyterlab_ext/labextension"},"styleModule":"style/index.js"}')
+            e.exports = JSON.parse('{"name":"amazon-codewhisperer-jupyterlab-ext","version":"2.0.1","description":"Amazon CodeWhisperer for JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","codewhisperer","amazon-codewhisperer"],"homepage":"https://github.com/aws","bugs":{"url":"https://aws.amazon.com/codewhisperer/","email":"codewhisperer@amazon.com"},"license":"Apache 2.0","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"author":{"name":"Amazon CodeWhisperer","email":"codewhisperer@amazon.com"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,eot,js,gif,html,jpg,json,png,svg,woff2,ttf}","style/img/*.{svg}","schema/*.json","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","config":{"vars":{"builddir":"./build/lib/amazon-codewhisperer-jupyterlab-ext","jupyterCorePath":"./build-tools/jupyter-staging"}},"npm-pretty-much":{"https://w/?NpmPrettyMuch/UndeclaredTransitiveDependencies":true,"legacyPackageNameAlias":"amazon-codewhisperer-jupyterlab-ext","npm-pretty-much":{"allowUnsafeName":"open source extension"},"runTest":"always","runRelease":"always"},"scripts":{"build":"npm run clean && npm run build:lib && npm run build:labextension","postbuild":"mkdir -p $npm_package_config_vars_builddir && rsync package.json $npm_package_config_vars_builddir && rsync -a --exclude={‘*.spec.d.ts’,’*.spec.js’} lib $npm_package_config_vars_builddir && rsync -a style $npm_package_config_vars_builddir","build:all":"npm run build:lib && npm run build:labextension","build:labextension":"build-labextension --core-path $npm_package_config_vars_jupyterCorePath .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:prod":"npm run clean && npm run build:lib && npm run build:labextension","clean":"npm run clean:lib","clean:all":"npm run clean:lib && npm run clean:labextension","clean:labextension":"rimraf amazon_codewhisperer_jupyterlab_ext/labextension","clean:lib":"rimraf lib tsconfig.tsbuildinfo","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"npm run build","dev":"npm run clean && npm run build:lib && npm run build:labextension:dev","dist":"python setup.py sdist","release":"npm run build && npm run postbuild && npm run dist","watch":"run-p watch:src watch:labextension","watch:labextension":"jupyter labextension watch .","watch:src":"tsc -w","generateTelemetry":"node node_modules/@aws-toolkits/telemetry/lib/generateTelemetry.js --output=src/telemetry/telemetry.gen.ts","generateClients":"ts-node ./scripts/build/generateServiceClient.ts ","test":"jest --no-cache"},"dependencies":{"@jupyter/ydoc":"~1.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.1.6","@jupyterlab/codeeditor":"^4.0.6","@jupyterlab/codemirror":"^4.0.6","@jupyterlab/completer":"^4.0.6","@jupyterlab/fileeditor":"^4.0.6","@jupyterlab/launcher":"^4.0.6","@jupyterlab/logconsole":"^4.0.6","@jupyterlab/nbformat":"^4.0.6","@jupyterlab/notebook":"^4.0.6","@jupyterlab/outputarea":"^4.0.6","@jupyterlab/rendermime":"^4.0.6","@jupyterlab/settingregistry":"^4.0.6","@jupyterlab/statedb":"^4.0.6","@jupyterlab/translation":"^4.0.6","@lumino/algorithm":"^2.0.0","@lumino/coreutils":"^2.0.0","@lumino/datagrid":"^2.0.1","@lumino/disposable":"^2.0.0","aws-sdk":"^2.1267.0","pino":"^8.11.0"},"devDependencies":{"@aws-toolkits/telemetry":"^1.0.120","@babel/core":"^7.21.5","@babel/preset-env":"^7.21.5","@codemirror/state":"^6.0.0","@codemirror/view":"^6.0.0","@jupyterlab/builder":"^4.0.0","@jupyterlab/testutils":"^4.0.0","@types/codemirror":"^5.60.7","@types/fs-extra":"^9.0.11","@types/jest":"^29.2.0","@types/json-schema":"^7.0.11","@types/node":"^16.0.0","@types/react":"18.2.25","@types/react-addons-linked-state-mixin":"^0.14.22","@typescript-eslint/eslint-plugin":"^5.62.0","@typescript-eslint/parser":"^5.62.0","css-loader":"^6.7.1","eslint":"^8.36.0","eslint-config-prettier":"^8.8.0","eslint-plugin-jsdoc":"^40.0.0","eslint-plugin-prettier":"^5.0.0","eslint-plugin-react":"^7.18.3","jest":"^29.2.0","jest-environment-jsdom":"^29.7.0","jest-fetch-mock":"^1.6.6","mkdirp":"^1.0.3","npm-run-all":"^4.1.5","pino-pretty":"10.0.0","prettier":"^3.0.0","rimraf":"^5.0.1","source-map-loader":"^1.0.2","style-loader":"^3.3.1","stylelint":"^15.10.1","stylelint-config-recommended":"^13.0.0","stylelint-config-standard":"^34.0.0","stylelint-csstree-validator":"^3.0.0","stylelint-prettier":"^4.0.0","ts-jest":"^29.0.0","typescript":"~5.0.2","yjs":"^13.5.40"},"sideEffects":["style/*.css","style/index.js"],"jupyterlab":{"extension":true,"schemaDir":"schema","outputDir":"amazon_codewhisperer_jupyterlab_ext/labextension"},"styleModule":"style/index.js"}')
         }
     }
 ]);
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/747.a6f42e6a863d7358a568.js` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/747.a6f42e6a863d7358a568.js`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.25e2176ddc0e279b9e44.js` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.210c5ddb098daa585d05.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, o, a, n, i, u, l, d, s, f, p, c, h, v, b, m, y, g, j, w, S, x = {
-            864: (e, r, t) => {
+            658: (e, r, t) => {
                 var o = {
                         "./index": () => t.e(706).then((() => () => t(706))),
                         "./extension": () => t.e(706).then((() => () => t(706))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -44,19 +44,19 @@
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
         571: "2ac5bdb342624f52bccb",
-        706: "92fee206ef596946b068",
+        706: "cbd5c24bed652ef332fb",
         747: "a6f42e6a863d7358a568"
     } [e] + ".js?v=" + {
         571: "2ac5bdb342624f52bccb",
-        706: "92fee206ef596946b068",
+        706: "cbd5c24bed652ef332fb",
         747: "a6f42e6a863d7358a568"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -109,15 +109,15 @@
                         (!u || !u.loaded && (!o != !u.eager ? o : i > u.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!o
                         })
                     },
                     l = [];
-                return "default" === t && (u("amazon-codewhisperer-jupyterlab-ext", "2.0.0", (() => E.e(706).then((() => () => E(706))))), u("pino", "8.11.0", (() => E.e(571).then((() => () => E(571)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("amazon-codewhisperer-jupyterlab-ext", "2.0.1", (() => E.e(706).then((() => () => E(706))))), u("pino", "8.11.0", (() => E.e(571).then((() => () => E(571)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -225,37 +225,37 @@
     }, v = e => (e.loaded = 1, e.get()), m = (b = e => function(r, t, o, a) {
         var n = E.I(r);
         return n && n.then ? n.then(e.bind(e, r, E.S[r], t, o, a)) : e(r, E.S[r], t, o, a)
     })(((e, r, t, o) => (i(e, t), v(f(r, t, o) || h(r, e, t, o) || u(r, t))))), y = b(((e, r, t, o) => (i(e, t), s(r, 0, t, o)))), g = b(((e, r, t, o, a) => {
         var n = r && E.o(r, t) && f(r, t, o);
         return n ? v(n) : a()
     })), j = {}, w = {
-        7: () => y("default", "@jupyterlab/statedb", [1, 4, 0, 7]),
+        10: () => y("default", "@jupyterlab/statedb", [1, 4, 0, 9]),
         29: () => y("default", "react", [1, 18, 2, 0]),
         59: () => y("default", "@lumino/virtualdom", [1, 2, 0, 0]),
-        60: () => y("default", "@jupyterlab/codemirror", [1, 4, 0, 7]),
+        85: () => y("default", "@jupyterlab/ui-components", [1, 4, 0, 9]),
         120: () => y("default", "@lumino/commands", [1, 2, 0, 1]),
-        141: () => y("default", "@jupyterlab/logconsole", [1, 4, 0, 7]),
+        122: () => y("default", "@jupyterlab/notebook", [1, 4, 0, 9]),
+        125: () => y("default", "@jupyterlab/services", [1, 7, 0, 9]),
+        143: () => y("default", "@jupyterlab/logconsole", [1, 4, 0, 9]),
+        190: () => y("default", "@jupyterlab/settingregistry", [1, 4, 0, 9]),
         211: () => y("default", "@codemirror/view", [1, 6, 9, 6]),
-        260: () => y("default", "@jupyterlab/statusbar", [1, 4, 0, 7]),
-        261: () => y("default", "@jupyterlab/fileeditor", [1, 4, 0, 7]),
-        408: () => y("default", "@jupyterlab/notebook", [1, 4, 0, 7]),
-        614: () => y("default", "@jupyterlab/coreutils", [1, 6, 0, 7]),
-        684: () => y("default", "@jupyterlab/settingregistry", [1, 4, 0, 7]),
+        308: () => y("default", "@jupyterlab/apputils", [1, 4, 1, 9]),
+        454: () => y("default", "@jupyterlab/codemirror", [1, 4, 0, 9]),
+        499: () => y("default", "@jupyterlab/rendermime", [1, 4, 0, 9]),
+        527: () => m("default", "@jupyterlab/docregistry", [1, 4, 0, 9]),
+        667: () => y("default", "@jupyterlab/statusbar", [1, 4, 0, 9]),
+        749: () => y("default", "@jupyterlab/coreutils", [1, 6, 0, 9]),
         778: () => y("default", "@lumino/widgets", [1, 2, 0, 1]),
-        788: () => y("default", "@jupyterlab/services", [1, 7, 0, 7]),
-        800: () => y("default", "@jupyterlab/ui-components", [1, 4, 0, 7]),
-        861: () => y("default", "@jupyterlab/apputils", [1, 4, 1, 7]),
         862: () => g("default", "pino", [1, 8, 11, 0], (() => E.e(571).then((() => () => E(571))))),
         901: () => y("default", "@lumino/signaling", [1, 2, 0, 0]),
         930: () => y("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        981: () => y("default", "@jupyterlab/rendermime", [1, 4, 0, 7]),
-        987: () => m("default", "@jupyterlab/docregistry", [1, 4, 0, 7])
+        977: () => y("default", "@jupyterlab/fileeditor", [1, 4, 0, 9])
     }, S = {
-        706: [7, 29, 59, 60, 120, 141, 211, 260, 261, 408, 614, 684, 778, 788, 800, 861, 862, 901, 930, 981, 987]
+        706: [10, 29, 59, 85, 120, 122, 125, 143, 190, 211, 308, 454, 499, 527, 667, 749, 778, 862, 901, 930, 977]
     }, E.f.consumes = (e, r) => {
         E.o(S, e) && S[e].forEach((e => {
             if (E.o(j, e)) return r.push(j[e]);
             var t = r => {
                     j[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
                     }
@@ -302,10 +302,10 @@
                     u && u(E)
                 }
                 for (r && r(t); l < n.length; l++) a = n[l], E.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunkamazon_codewhisperer_jupyterlab_ext = self.webpackChunkamazon_codewhisperer_jupyterlab_ext || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
-    var _ = E(864);
+    var _ = E(658);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["amazon-codewhisperer-jupyterlab-ext"] = _
 })();
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/utils.py` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from datetime import datetime, timedelta
 
-from amazon_codewhisperer_jupyterlab_ext.constants import RESPONSE_SESSION_ID_HEADER_NAME, ERROR_CODE_TO_USER_MESSAGE_MAP
+from amazon_codewhisperer_jupyterlab_ext.constants import (
+    RESPONSE_SESSION_ID_HEADER_NAME,
+    ERROR_CODE_TO_USER_MESSAGE_MAP,
+    SAGEMAKER_CONNECT_ERROR,
+)
+from amazon_codewhisperer_jupyterlab_ext.env import Environment
 
 
 def time_from_now(time):
     now = datetime.utcnow()
     future = now + timedelta(seconds=time)
     return int(future.timestamp())
 
@@ -71,7 +76,15 @@
     return ServiceResponse(ServiceResponseStatus.ERROR, None, error_info, request_id, None)
 
 
 def generate_client_error_codewhisperer_service_response(e):
     request_id = e.response['ResponseMetadata']['RequestId']
     error_info = ServiceErrorInfo(e.response['Error']['Code'], e.response['message'])
     return ServiceResponse(ServiceResponseStatus.ERROR, None, error_info, request_id, None)
+
+
+def generate_connect_error_codewhisperer_service_response(e):
+    if Environment.is_sm_studio():
+        error_info = ServiceErrorInfo('ConnectTimeoutError', SAGEMAKER_CONNECT_ERROR)
+        return ServiceResponse(ServiceResponseStatus.ERROR, None, error_info, None, None)
+    else:
+        raise e
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext/validator/validator.py` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext/validator/validator.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-codewhisperer-jupyterlab-ext
-Version: 2.0.0
+Version: 2.0.1
 Summary: Amazon CodeWhisperer for JupyterLab
 Home-page: https://aws.amazon.com/codewhisperer/
 Author: Amazon CodeWhisperer
 Author-email: codewhisperer@amazon.com
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab4,Amazon CodeWhisperer,CodeWhisperer,Code,Whisperer
 Platform: Linux
@@ -18,14 +18,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Jupyter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: boto3
+Requires-Dist: botocore
+Requires-Dist: aiobotocore
+Requires-Dist: jupyterlab<5.0,>=4.0
 
 # Amazon CodeWhisperer for JupyterLab
 
 Amazon CodeWhisperer is an AI coding companion which provides developers with real-time code suggestions in JupyterLab. Individual developers can use CodeWhisperer for free in JupyterLab and AWS SageMaker Studio.
 
 ![Codewhisperer demo](https://docs.aws.amazon.com/images/codewhisperer/latest/userguide/images/codewhisperer-timestamp-record.png)
 
@@ -111,11 +115,13 @@
 
 * [CodeWhisperer User Guide](https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html)
 * [Setting up Amazon CodeWhisperer with JupyterLab](https://docs.aws.amazon.com/codewhisperer/latest/userguide/jupyterlab-setup.html)
 * [Setting up CodeWhisperer with Amazon SageMaker Studio](https://docs.aws.amazon.com/codewhisperer/latest/userguide/sagemaker-setup.html)
 
 ## Change Log
 
+2.0.1
+* Improved handling when Jupyter has no access to internet.
+* Migrated network call to be made asynchronously.
+
 2.0.0
 * Initial release - Adoption of JupyterLab 4
-
-
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 LICENSE
+MANIFEST.in
 NOTICE
 README.md
 install.json
 package.json
 pyproject.toml
 setup.py
 tsconfig.json
 tsconfig.test.json
 amazon_codewhisperer_jupyterlab_ext/__init__.py
-amazon_codewhisperer_jupyterlab_ext/_version.py
 amazon_codewhisperer_jupyterlab_ext/constants.py
 amazon_codewhisperer_jupyterlab_ext/handlers.py
 amazon_codewhisperer_jupyterlab_ext/utils.py
 amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO
 amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt
 amazon_codewhisperer_jupyterlab_ext.egg-info/dependency_links.txt
 amazon_codewhisperer_jupyterlab_ext.egg-info/not-zip-safe
@@ -32,38 +32,43 @@
 amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py
 amazon_codewhisperer_jupyterlab_ext/env/__init__.py
 amazon_codewhisperer_jupyterlab_ext/env/environment.py
 amazon_codewhisperer_jupyterlab_ext/labextension/package.json
 amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json
 amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig
 amazon_codewhisperer_jupyterlab_ext/labextension/static/571.2ac5bdb342624f52bccb.js
-amazon_codewhisperer_jupyterlab_ext/labextension/static/706.92fee206ef596946b068.js
-amazon_codewhisperer_jupyterlab_ext/labextension/static/706.92fee206ef596946b068.js.LICENSE.txt
+amazon_codewhisperer_jupyterlab_ext/labextension/static/706.cbd5c24bed652ef332fb.js
+amazon_codewhisperer_jupyterlab_ext/labextension/static/706.cbd5c24bed652ef332fb.js.LICENSE.txt
 amazon_codewhisperer_jupyterlab_ext/labextension/static/747.a6f42e6a863d7358a568.js
-amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.25e2176ddc0e279b9e44.js
+amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.210c5ddb098daa585d05.js
 amazon_codewhisperer_jupyterlab_ext/labextension/static/style.js
 amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json
 amazon_codewhisperer_jupyterlab_ext/validator/__init__.py
 amazon_codewhisperer_jupyterlab_ext/validator/validator.py
 amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json
 jupyter-config/jupyter_server_config.d/amazon_codewhisperer_jupyterlab_ext.json
 src/application.ts
 src/handler.ts
 src/icons.ts
 src/index.ts
 src/messages.ts
 src/svg.d.ts
 src/__tests__/index.spec.ts
+src/__tests__/autotrigger/autotrigger.spec.ts
+src/__tests__/recommendation/recommendationStateHandler.spec.ts
 src/auth/authManager.tsx
+src/autotrigger/autotrigger.ts
 src/aws_vector_consolas_jupyter_lab3_extension/__init__.py
 src/aws_vector_consolas_jupyter_lab3_extension/py.typed
 src/client/apiclient.ts
 src/client/codewhispererclient.d.ts
 src/client/codewhispereruserclient.d.ts
 src/inline/inline.ts
+src/inline/inlinePlugin.ts
+src/inline/inlineWidget.ts
 src/keybindings/keybindings.ts
 src/logging/logger.tsx
 src/notifications/notifications.tsx
 src/recommendation/extractor.ts
 src/recommendation/recommendationStateHandler.ts
 src/recommendation/worker.ts
 src/referencetracker/referencetracker.tsx
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/package.json` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.0.1'"}*

```diff
@@ -146,9 +146,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "2.0.1"
 }
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/pyproject.toml` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/setup.py` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     license=pkg_json["license"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
         "boto3",
         "botocore",
+        "aiobotocore",
         "jupyterlab>=4.0,<5.0"
     ],
     zip_safe=False,
     include_package_data=True,
     python_requires=">=3.6",
     platforms="Linux, Mac OS X, Windows",
     keywords=["Jupyter", "JupyterLab", "JupyterLab4", "Amazon CodeWhisperer", "CodeWhisperer", "Code", "Whisperer"],
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/application.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/application.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/auth/authManager.tsx` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/auth/authManager.tsx`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/client/apiclient.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/client/apiclient.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/client/codewhispererclient.d.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/client/codewhispererclient.d.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/client/codewhispereruserclient.d.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/client/codewhispereruserclient.d.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/handler.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/icons.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/icons.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/index.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/inline/inline.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/inline/inline.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/keybindings/keybindings.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/keybindings/keybindings.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/logging/logger.tsx` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/logging/logger.tsx`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/notifications/notifications.tsx` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/notifications/notifications.tsx`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/recommendation/extractor.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/recommendation/extractor.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/recommendation/recommendationStateHandler.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/recommendation/recommendationStateHandler.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/recommendation/worker.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/recommendation/worker.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/referencetracker/referencetracker.tsx` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/referencetracker/referencetracker.tsx`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/statusbar/statusbarwidget.tsx` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/statusbar/statusbarwidget.tsx`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/telemetry/clienttelemetry.d.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/telemetry/clienttelemetry.d.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/telemetry/telemetry.gen.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/telemetry/telemetry.gen.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/telemetry/telemetry.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/telemetry/telemetry.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/telemetry/telemetryClient.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/telemetry/telemetryClient.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/utils/constants.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/utils/constants.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/utils/models.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/utils/models.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/src/utils/utils.ts` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/src/utils/utils.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/style/base.css` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/style/base.css`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/codewhisperer.svg` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/codewhisperer.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/disconnected.svg` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/disconnected.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/log.svg` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/log.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/signout.svg` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/signout.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/style/img/visual-cue-arrow.svg` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/style/img/visual-cue-arrow.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-2.0.0/tsconfig.json` & `amazon-codewhisperer-jupyterlab-ext-2.0.1/tsconfig.json`

 * *Files identical despite different names*

