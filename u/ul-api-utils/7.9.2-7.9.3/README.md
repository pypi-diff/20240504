# Comparing `tmp/ul-api-utils-7.9.2.tar.gz` & `tmp/ul-api-utils-7.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-api-utils-7.9.2.tar", last modified: Mon Apr 22 12:43:14 2024, max compression
+gzip compressed data, was "ul-api-utils-7.9.3.tar", last modified: Wed Apr 24 06:16:03 2024, max compression
```

## Comparing `ul-api-utils-7.9.2.tar` & `ul-api-utils-7.9.3.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.356728 ul-api-utils-7.9.2/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2022-02-08 08:28:45.000000 ul-api-utils-7.9.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13527 2024-04-22 12:43:14.356728 ul-api-utils-7.9.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12938 2023-04-11 10:27:02.000000 ul-api-utils-7.9.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.184721 ul-api-utils-7.9.2/example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/example/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1018 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/example/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2024-02-19 15:49:36.000000 ul-api-utils-7.9.2/example/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.184721 ul-api-utils-7.9.2/example/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/example/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-09-19 08:28:56.000000 ul-api-utils-7.9.2/example/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1329 2022-08-15 22:48:45.000000 ul-api-utils-7.9.2/example/pure_flask_example.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-08-15 22:48:45.000000 ul-api-utils-7.9.2/example/rate_limit_load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.184721 ul-api-utils-7.9.2/example/routes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/example/routes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13316 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/example/routes/api_some.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.184721 ul-api-utils-7.9.2/example/workers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/example/workers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/example/workers/worker.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 12:43:14.356728 ul-api-utils-7.9.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2951 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.212722 ul-api-utils-7.9.2/ul_api_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.220723 ul-api-utils-7.9.2/ul_api_utils/access/
--rw-rw-rw-   0 root         (0) root         (0)     4526 2023-09-19 08:28:56.000000 ul-api-utils-7.9.2/ul_api_utils/access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.224722 ul-api-utils-7.9.2/ul_api_utils/api_resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/api_resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3279 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/api_resource/api_request.py
--rw-rw-rw-   0 root         (0) root         (0)    17766 2024-03-28 13:39:52.000000 ul-api-utils-7.9.2/ul_api_utils/api_resource/api_resource.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/api_resource/api_resource_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2024-03-28 13:39:52.000000 ul-api-utils-7.9.2/ul_api_utils/api_resource/api_resource_error_handling.py
--rw-rw-rw-   0 root         (0) root         (0)    18224 2024-03-28 13:39:52.000000 ul-api-utils-7.9.2/ul_api_utils/api_resource/api_resource_fn_typing.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/api_resource/api_resource_type.py
--rw-rw-rw-   0 root         (0) root         (0)     9676 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/api_resource/api_response.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/api_resource/api_response_db.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/api_resource/api_response_payload_alias.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-06-28 12:08:16.000000 ul-api-utils-7.9.2/ul_api_utils/api_resource/db_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/api_resource/signature_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.236723 ul-api-utils-7.9.2/ul_api_utils/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8453 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/commands/cmd_enc_keys.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-11-17 09:49:11.000000 ul-api-utils-7.9.2/ul_api_utils/commands/cmd_gen_api_user_token.py
--rw-rw-rw-   0 root         (0) root         (0)     4549 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/commands/cmd_gen_new_api_user.py
--rw-rw-rw-   0 root         (0) root         (0)     9617 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/commands/cmd_generate_api_docs.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/commands/cmd_start.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/commands/cmd_worker_start.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.248724 ul-api-utils-7.9.2/ul_api_utils/commands/start/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/commands/start/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/commands/start/gunicorn.conf.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/commands/start/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.276725 ul-api-utils-7.9.2/ul_api_utils/conf/
--rw-rw-rw-   0 root         (0) root         (0)   999747 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/conf/ul-debugger-main.js
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/conf/ul-debugger-ui.js
--rw-rw-rw-   0 root         (0) root         (0)     3232 2023-11-17 09:49:11.000000 ul-api-utils-7.9.2/ul_api_utils/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2024-02-12 08:21:41.000000 ul-api-utils-7.9.2/ul_api_utils/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.284725 ul-api-utils-7.9.2/ul_api_utils/debug/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/debug/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/debug/debugger.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/debug/malloc.py
--rw-rw-rw-   0 root         (0) root         (0)    14591 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/debug/stat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.284725 ul-api-utils-7.9.2/ul_api_utils/encrypt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/encrypt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/encrypt/encrypt_decrypt_abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     2356 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py
--rw-rw-rw-   0 root         (0) root         (0)     8137 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.284725 ul-api-utils-7.9.2/ul_api_utils/internal_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/internal_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.288725 ul-api-utils-7.9.2/ul_api_utils/internal_api/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/internal_api/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/internal_api/__tests__/internal_api.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/internal_api/__tests__/internal_api_content_type.py
--rw-rw-rw-   0 root         (0) root         (0)    14067 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/internal_api/internal_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/internal_api/internal_api_check_context.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/internal_api/internal_api_error.py
--rw-rw-rw-   0 root         (0) root         (0)    11583 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/internal_api/internal_api_response.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-02-19 10:35:07.000000 ul-api-utils-7.9.2/ul_api_utils/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.288725 ul-api-utils-7.9.2/ul_api_utils/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.288725 ul-api-utils-7.9.2/ul_api_utils/modules/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/modules/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10719 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
--rw-rw-rw-   0 root         (0) root         (0)    25660 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/modules/api_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)     2389 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/modules/api_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15112 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/modules/api_sdk_jwt.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/modules/intermediate_state.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/modules/worker_context.py
--rw-rw-rw-   0 root         (0) root         (0)     4654 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/modules/worker_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/modules/worker_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.296725 ul-api-utils-7.9.2/ul_api_utils/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7516 2024-03-28 13:39:52.000000 ul-api-utils-7.9.2/ul_api_utils/resources/caching.py
--rw-rw-rw-   0 root         (0) root         (0)     5094 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/resources/debugger_scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.300726 ul-api-utils-7.9.2/ul_api_utils/resources/health_check/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/resources/health_check/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/resources/health_check/const.py
--rw-rw-rw-   0 root         (0) root         (0)    18449 2023-09-19 09:52:18.000000 ul-api-utils-7.9.2/ul_api_utils/resources/health_check/health_check.py
--rw-rw-rw-   0 root         (0) root         (0)     2572 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/resources/health_check/health_check_template.py
--rw-rw-rw-   0 root         (0) root         (0)     4199 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/resources/health_check/resource.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/resources/not_implemented.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/resources/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     3358 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/resources/rate_limitter.py
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/resources/sockets.py
--rw-rw-rw-   0 root         (0) root         (0)     5359 2024-02-19 10:35:07.000000 ul-api-utils-7.9.2/ul_api_utils/resources/swagger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.300726 ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.300726 ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/custom_fields/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/custom_fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-03-28 13:39:52.000000 ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/custom_fields/custom_checkbox_select.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.300726 ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/custom_widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/custom_widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3777 2024-03-28 13:39:52.000000 ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/custom_widgets/custom_select_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-03-28 13:39:52.000000 ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/custom_widgets/custom_text_input_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/uni_form.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/sentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.332727 ul-api-utils-7.9.2/ul_api_utils/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.332727 ul-api-utils-7.9.2/ul_api_utils/utils/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/utils/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/__tests__/api_path_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2487 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/__tests__/unwrap_typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/api_encoding.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/api_format.py
--rw-rw-rw-   0 root         (0) root         (0)     2020 2024-02-12 08:21:41.000000 ul-api-utils-7.9.2/ul_api_utils/utils/api_method.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/api_pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/api_path_version.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/api_request_info.py
--rw-rw-rw-   0 root         (0) root         (0)     5021 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/avro.py
--rw-rw-rw-   0 root         (0) root         (0)     1556 2023-11-17 09:49:11.000000 ul-api-utils-7.9.2/ul_api_utils/utils/broker_topics_message_count.py
--rw-rw-rw-   0 root         (0) root         (0)      670 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/cached_per_request.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/colors.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/decode_base64.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/deprecated.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2023-09-19 08:28:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.336727 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.336727 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/specifiers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/specifiers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py
--rw-rw-rw-   0 root         (0) root         (0)    28944 2024-02-19 10:35:07.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.352728 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-08-15 07:34:58.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/schema_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/imports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.352728 ul-api-utils-7.9.2/ul_api_utils/utils/jinja/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/utils/jinja/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/jinja/t_url_for.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/jinja/to_pretty_json.py
--rw-rw-rw-   0 root         (0) root         (0)     4140 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/utils/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/load_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-28 12:08:16.000000 ul-api-utils-7.9.2/ul_api_utils/utils/token_check.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/token_check_through_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/unwrap_typing.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/utils/uuid_converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.352728 ul-api-utils-7.9.2/ul_api_utils/validators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/validators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.352728 ul-api-utils-7.9.2/ul_api_utils/validators/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 12:43:13.000000 ul-api-utils-7.9.2/ul_api_utils/validators/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/validators/__tests__/test_custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4023 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/validators/custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/validators/validate_empty_object.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-22 12:49:56.000000 ul-api-utils-7.9.2/ul_api_utils/validators/validate_uuid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:43:14.220723 ul-api-utils-7.9.2/ul_api_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13527 2024-04-22 12:43:14.000000 ul-api-utils-7.9.2/ul_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6050 2024-04-22 12:43:14.000000 ul-api-utils-7.9.2/ul_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 12:43:14.000000 ul-api-utils-7.9.2/ul_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-22 12:43:14.000000 ul-api-utils-7.9.2/ul_api_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      586 2024-04-22 12:43:14.000000 ul-api-utils-7.9.2/ul_api_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-22 12:43:14.000000 ul-api-utils-7.9.2/ul_api_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.292246 ul-api-utils-7.9.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2022-02-10 15:47:01.000000 ul-api-utils-7.9.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13527 2024-04-24 06:16:03.292246 ul-api-utils-7.9.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12938 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.176242 ul-api-utils-7.9.3/example/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/example/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1018 2024-04-24 06:16:01.000000 ul-api-utils-7.9.3/example/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-02-22 01:08:42.000000 ul-api-utils-7.9.3/example/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.180242 ul-api-utils-7.9.3/example/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/example/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-09-19 09:46:34.000000 ul-api-utils-7.9.3/example/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2022-08-11 17:53:18.000000 ul-api-utils-7.9.3/example/pure_flask_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-08-11 08:41:19.000000 ul-api-utils-7.9.3/example/rate_limit_load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.180242 ul-api-utils-7.9.3/example/routes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/example/routes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13316 2024-04-24 06:16:01.000000 ul-api-utils-7.9.3/example/routes/api_some.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.180242 ul-api-utils-7.9.3/example/workers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/example/workers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/example/workers/worker.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 06:16:03.292246 ul-api-utils-7.9.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2024-04-24 06:16:01.000000 ul-api-utils-7.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.188242 ul-api-utils-7.9.3/ul_api_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.188242 ul-api-utils-7.9.3/ul_api_utils/access/
+-rw-rw-rw-   0 root         (0) root         (0)     4526 2023-09-19 09:46:34.000000 ul-api-utils-7.9.3/ul_api_utils/access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.196243 ul-api-utils-7.9.3/ul_api_utils/api_resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/api_resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/api_resource/api_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    17766 2024-04-10 06:59:01.000000 ul-api-utils-7.9.3/ul_api_utils/api_resource/api_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/api_resource/api_resource_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2024-04-10 06:59:01.000000 ul-api-utils-7.9.3/ul_api_utils/api_resource/api_resource_error_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)    18224 2024-04-10 06:59:01.000000 ul-api-utils-7.9.3/ul_api_utils/api_resource/api_resource_fn_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/api_resource/api_resource_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/api_resource/api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/api_resource/api_response_db.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/api_resource/api_response_payload_alias.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-08-09 09:33:13.000000 ul-api-utils-7.9.3/ul_api_utils/api_resource/db_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/api_resource/signature_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.196243 ul-api-utils-7.9.3/ul_api_utils/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8453 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/commands/cmd_enc_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2024-02-22 01:08:42.000000 ul-api-utils-7.9.3/ul_api_utils/commands/cmd_gen_api_user_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/commands/cmd_gen_new_api_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     9617 2024-04-24 06:16:01.000000 ul-api-utils-7.9.3/ul_api_utils/commands/cmd_generate_api_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-10 06:59:01.000000 ul-api-utils-7.9.3/ul_api_utils/commands/cmd_start.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/commands/cmd_worker_start.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.200243 ul-api-utils-7.9.3/ul_api_utils/commands/start/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/commands/start/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/commands/start/gunicorn.conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/commands/start/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.216243 ul-api-utils-7.9.3/ul_api_utils/conf/
+-rw-rw-rw-   0 root         (0) root         (0)   999747 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/conf/ul-debugger-main.js
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/conf/ul-debugger-ui.js
+-rw-rw-rw-   0 root         (0) root         (0)     3487 2024-04-24 06:16:01.000000 ul-api-utils-7.9.3/ul_api_utils/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-02-22 01:08:42.000000 ul-api-utils-7.9.3/ul_api_utils/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.228244 ul-api-utils-7.9.3/ul_api_utils/debug/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/debug/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/debug/debugger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/debug/malloc.py
+-rw-rw-rw-   0 root         (0) root         (0)    14591 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/debug/stat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.228244 ul-api-utils-7.9.3/ul_api_utils/encrypt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/encrypt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/encrypt/encrypt_decrypt_abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py
+-rw-rw-rw-   0 root         (0) root         (0)     8137 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.232244 ul-api-utils-7.9.3/ul_api_utils/internal_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/internal_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.232244 ul-api-utils-7.9.3/ul_api_utils/internal_api/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/internal_api/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/internal_api/__tests__/internal_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/internal_api/__tests__/internal_api_content_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    14067 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/internal_api/internal_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/internal_api/internal_api_check_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/internal_api/internal_api_error.py
+-rw-rw-rw-   0 root         (0) root         (0)    11583 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/internal_api/internal_api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-02-22 01:08:42.000000 ul-api-utils-7.9.3/ul_api_utils/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.232244 ul-api-utils-7.9.3/ul_api_utils/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.232244 ul-api-utils-7.9.3/ul_api_utils/modules/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/modules/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10719 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)    25660 2024-04-24 06:16:01.000000 ul-api-utils-7.9.3/ul_api_utils/modules/api_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2389 2024-04-10 06:59:01.000000 ul-api-utils-7.9.3/ul_api_utils/modules/api_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15112 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/modules/api_sdk_jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/modules/intermediate_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/modules/worker_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2024-04-24 06:16:01.000000 ul-api-utils-7.9.3/ul_api_utils/modules/worker_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/modules/worker_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.236244 ul-api-utils-7.9.3/ul_api_utils/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7516 2024-04-10 06:59:01.000000 ul-api-utils-7.9.3/ul_api_utils/resources/caching.py
+-rw-rw-rw-   0 root         (0) root         (0)     5094 2024-04-24 06:16:01.000000 ul-api-utils-7.9.3/ul_api_utils/resources/debugger_scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.244244 ul-api-utils-7.9.3/ul_api_utils/resources/health_check/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/resources/health_check/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/resources/health_check/const.py
+-rw-rw-rw-   0 root         (0) root         (0)    18449 2023-10-12 09:08:28.000000 ul-api-utils-7.9.3/ul_api_utils/resources/health_check/health_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     2572 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/resources/health_check/health_check_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     4199 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/resources/health_check/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/resources/not_implemented.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/resources/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3358 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/resources/rate_limitter.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-10 06:59:01.000000 ul-api-utils-7.9.3/ul_api_utils/resources/sockets.py
+-rw-rw-rw-   0 root         (0) root         (0)     5391 2024-04-24 06:16:01.000000 ul-api-utils-7.9.3/ul_api_utils/resources/swagger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.244244 ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.244244 ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/custom_fields/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/custom_fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-02-28 09:55:22.000000 ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/custom_fields/custom_checkbox_select.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.256245 ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/custom_widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/custom_widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3777 2024-02-28 09:55:22.000000 ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/custom_widgets/custom_select_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-02-28 09:55:22.000000 ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/custom_widgets/custom_text_input_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2024-04-24 06:16:01.000000 ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/uni_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/sentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.272246 ul-api-utils-7.9.3/ul_api_utils/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.272246 ul-api-utils-7.9.3/ul_api_utils/utils/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/utils/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/__tests__/api_path_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/__tests__/unwrap_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/api_encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/api_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2024-02-22 01:08:42.000000 ul-api-utils-7.9.3/ul_api_utils/utils/api_method.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/api_pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/api_path_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/api_request_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     5021 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/avro.py
+-rw-rw-rw-   0 root         (0) root         (0)     1556 2024-02-22 01:08:42.000000 ul-api-utils-7.9.3/ul_api_utils/utils/broker_topics_message_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      670 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/cached_per_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/decode_base64.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/deprecated.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2023-09-19 09:46:34.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.272246 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.288246 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/specifiers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/specifiers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    28944 2024-02-22 01:08:42.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.292246 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-08-09 09:33:13.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/schema_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/imports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.292246 ul-api-utils-7.9.3/ul_api_utils/utils/jinja/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/utils/jinja/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/jinja/t_url_for.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/jinja/to_pretty_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     4140 2024-04-24 06:16:01.000000 ul-api-utils-7.9.3/ul_api_utils/utils/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/load_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-08-09 09:33:13.000000 ul-api-utils-7.9.3/ul_api_utils/utils/token_check.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/token_check_through_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/unwrap_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/utils/uuid_converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.292246 ul-api-utils-7.9.3/ul_api_utils/validators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/validators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.292246 ul-api-utils-7.9.3/ul_api_utils/validators/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils/validators/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/validators/__tests__/test_custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     4023 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/validators/custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/validators/validate_empty_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-22 11:20:51.000000 ul-api-utils-7.9.3/ul_api_utils/validators/validate_uuid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:16:03.188242 ul-api-utils-7.9.3/ul_api_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13527 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6050 2024-04-24 06:16:03.000000 ul-api-utils-7.9.3/ul_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      586 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-24 06:16:02.000000 ul-api-utils-7.9.3/ul_api_utils.egg-info/top_level.txt
```

### Comparing `ul-api-utils-7.9.2/LICENSE` & `ul-api-utils-7.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/PKG-INFO` & `ul-api-utils-7.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-api-utils
-Version: 7.9.2
+Version: 7.9.3
 Summary: Python api utils
 Author: Unic-lab
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-api-utils-7.9.2/README.md` & `ul-api-utils-7.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/example/conf.py` & `ul-api-utils-7.9.3/example/conf.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/example/pure_flask_example.py` & `ul-api-utils-7.9.3/example/pure_flask_example.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/example/routes/api_some.py` & `ul-api-utils-7.9.3/example/routes/api_some.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/example/workers/worker.py` & `ul-api-utils-7.9.3/example/workers/worker.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/setup.py` & `ul-api-utils-7.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-api-utils',
-    version='7.9.2',
+    version='7.9.3',
     description='Python api utils',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='',
     packages=find_packages(),
     package_data={
```

### Comparing `ul-api-utils-7.9.2/ul_api_utils/access/__init__.py` & `ul-api-utils-7.9.3/ul_api_utils/access/__init__.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/api_resource/api_request.py` & `ul-api-utils-7.9.3/ul_api_utils/api_resource/api_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/api_resource/api_resource.py` & `ul-api-utils-7.9.3/ul_api_utils/api_resource/api_resource.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/api_resource/api_resource_config.py` & `ul-api-utils-7.9.3/ul_api_utils/api_resource/api_resource_config.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/api_resource/api_resource_error_handling.py` & `ul-api-utils-7.9.3/ul_api_utils/api_resource/api_resource_error_handling.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/api_resource/api_resource_fn_typing.py` & `ul-api-utils-7.9.3/ul_api_utils/api_resource/api_resource_fn_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/api_resource/api_response.py` & `ul-api-utils-7.9.3/ul_api_utils/api_resource/api_response.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/api_resource/api_response_db.py` & `ul-api-utils-7.9.3/ul_api_utils/api_resource/api_response_db.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/api_resource/api_response_payload_alias.py` & `ul-api-utils-7.9.3/ul_api_utils/api_resource/api_response_payload_alias.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/api_resource/signature_check.py` & `ul-api-utils-7.9.3/ul_api_utils/api_resource/signature_check.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/commands/cmd_enc_keys.py` & `ul-api-utils-7.9.3/ul_api_utils/commands/cmd_enc_keys.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/commands/cmd_gen_api_user_token.py` & `ul-api-utils-7.9.3/ul_api_utils/commands/cmd_gen_api_user_token.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/commands/cmd_gen_new_api_user.py` & `ul-api-utils-7.9.3/ul_api_utils/commands/cmd_gen_new_api_user.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/commands/cmd_generate_api_docs.py` & `ul-api-utils-7.9.3/ul_api_utils/commands/cmd_generate_api_docs.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/commands/cmd_start.py` & `ul-api-utils-7.9.3/ul_api_utils/commands/cmd_start.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/commands/cmd_worker_start.py` & `ul-api-utils-7.9.3/ul_api_utils/commands/cmd_worker_start.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/commands/start/wsgi.py` & `ul-api-utils-7.9.3/ul_api_utils/commands/start/wsgi.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/conf/ul-debugger-main.js` & `ul-api-utils-7.9.3/ul_api_utils/conf/ul-debugger-main.js`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/conf/ul-debugger-ui.js` & `ul-api-utils-7.9.3/ul_api_utils/conf/ul-debugger-ui.js`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/conf.py` & `ul-api-utils-7.9.3/ul_api_utils/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 from datetime import datetime
 from typing import Optional
 
 from ul_py_tool.utils.colors import NC, FG_BLUE
 
-from ul_api_utils.const import APPLICATION_ENV__LOCAL
+from ul_api_utils.const import APPLICATION_ENV__LOCAL, API_PATH__SWAGGER, API_PATH__SWAGGER_SPEC
 from ul_api_utils.utils.decode_base64 import decode_base64_to_string
 from ul_api_utils.utils.flags import Flagged
 
 APPLICATION_START_DT = datetime.fromisoformat(os.environ.get('APPLICATION_START_DT', datetime.now().isoformat()))
 APPLICATION_DEBUGGER_PIN = os.environ.get('APPLICATION_DEBUGGER_PIN', '1232344321')
 assert len(APPLICATION_DEBUGGER_PIN) > 0
 APPLICATION_GUNICORN_WORKERS = os.environ.get('APPLICATION_GUNICORN_WORKERS', '')
@@ -54,14 +54,17 @@
 assert APPLICATION_LOG_LEVEL in _LOG_MAP
 
 APPLICATION_SENTRY_DSN = os.environ.get('APPLICATION_SENTRY_DSN', '')
 APPLICATION_SENTRY_ENABLED_FLASK = os.environ.get('APPLICATION_SENTRY_FLASK', '1') == '1'
 
 APPLICATION_F = Flagged(os.environ.get('APPLICATION_F', ''))
 
+APPLICATION_SWAGGER_SPECIFICATION_PATH = os.environ.get('APPLICATION_SWAGGER_SPECIFICATION_PATH', API_PATH__SWAGGER_SPEC)
+APPLICATION_SWAGGER_PATH = os.environ.get('APPLICATION_SWAGGER_PATH', API_PATH__SWAGGER)
+
 logging.basicConfig(
     handlers=[logging.StreamHandler(sys.stdout)],
     level=_LOG_MAP[APPLICATION_LOG_LEVEL],
     format=APPLICATION_LOG_FORMAT,
 )
 
 logging.getLogger('').setLevel(_LOG_MAP[APPLICATION_LOG_LEVEL])
```

### Comparing `ul-api-utils-7.9.2/ul_api_utils/const.py` & `ul-api-utils-7.9.3/ul_api_utils/const.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/debug/debugger.py` & `ul-api-utils-7.9.3/ul_api_utils/debug/debugger.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/debug/malloc.py` & `ul-api-utils-7.9.3/ul_api_utils/debug/malloc.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/debug/stat.py` & `ul-api-utils-7.9.3/ul_api_utils/debug/stat.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py` & `ul-api-utils-7.9.3/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/errors.py` & `ul-api-utils-7.9.3/ul_api_utils/errors.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/internal_api/__tests__/internal_api.py` & `ul-api-utils-7.9.3/ul_api_utils/internal_api/__tests__/internal_api.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/internal_api/__tests__/internal_api_content_type.py` & `ul-api-utils-7.9.3/ul_api_utils/internal_api/__tests__/internal_api_content_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/internal_api/internal_api.py` & `ul-api-utils-7.9.3/ul_api_utils/internal_api/internal_api.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/internal_api/internal_api_check_context.py` & `ul-api-utils-7.9.3/ul_api_utils/internal_api/internal_api_check_context.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/internal_api/internal_api_response.py` & `ul-api-utils-7.9.3/ul_api_utils/internal_api/internal_api_response.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/main.py` & `ul-api-utils-7.9.3/ul_api_utils/main.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py` & `ul-api-utils-7.9.3/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/modules/api_sdk.py` & `ul-api-utils-7.9.3/ul_api_utils/modules/api_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/modules/api_sdk_config.py` & `ul-api-utils-7.9.3/ul_api_utils/modules/api_sdk_config.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/modules/api_sdk_jwt.py` & `ul-api-utils-7.9.3/ul_api_utils/modules/api_sdk_jwt.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/modules/intermediate_state.py` & `ul-api-utils-7.9.3/ul_api_utils/modules/intermediate_state.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/modules/worker_context.py` & `ul-api-utils-7.9.3/ul_api_utils/modules/worker_context.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/modules/worker_sdk.py` & `ul-api-utils-7.9.3/ul_api_utils/modules/worker_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/resources/caching.py` & `ul-api-utils-7.9.3/ul_api_utils/resources/caching.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/resources/debugger_scripts.py` & `ul-api-utils-7.9.3/ul_api_utils/resources/debugger_scripts.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/resources/health_check/health_check.py` & `ul-api-utils-7.9.3/ul_api_utils/resources/health_check/health_check.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/resources/health_check/health_check_template.py` & `ul-api-utils-7.9.3/ul_api_utils/resources/health_check/health_check_template.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/resources/health_check/resource.py` & `ul-api-utils-7.9.3/ul_api_utils/resources/health_check/resource.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/resources/not_implemented.py` & `ul-api-utils-7.9.3/ul_api_utils/resources/not_implemented.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/resources/permissions.py` & `ul-api-utils-7.9.3/ul_api_utils/resources/permissions.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/resources/rate_limitter.py` & `ul-api-utils-7.9.3/ul_api_utils/resources/rate_limitter.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/resources/swagger.py` & `ul-api-utils-7.9.3/ul_api_utils/resources/swagger.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 
 from ul_api_utils.access import GLOBAL_PERMISSION__PUBLIC, PermissionDefinition
 from ul_api_utils.api_resource.api_resource import ApiResource
 from ul_api_utils.api_resource.api_resource_config import ApiResourceConfig
 from ul_api_utils.api_resource.api_resource_fn_typing import ApiResourceFnTyping
 from ul_api_utils.api_resource.api_resource_type import ApiResourceType
 from ul_api_utils.api_resource.api_response import EmptyJsonApiResponse, ApiResponse
-from ul_api_utils.conf import APPLICATION_TMP, APPLICATION_DIR, APPLICATION_F
-from ul_api_utils.const import API_PATH__SWAGGER_SPEC, API_PATH__SWAGGER
+from ul_api_utils.conf import APPLICATION_TMP, APPLICATION_DIR, APPLICATION_F, APPLICATION_SWAGGER_PATH, APPLICATION_SWAGGER_SPECIFICATION_PATH
 from ul_api_utils.debug.debugger import Debugger, AJAX_INTERSEPTOR
 from ul_api_utils.utils.api_method import ApiMethod
 from ul_api_utils.utils.api_path_version import ApiPathVersion
 from ul_api_utils.utils.flask_swagger_generator.specifiers.swagger_three_specifier import SwaggerThreeSpecifier
 from ul_api_utils.utils.flask_swagger_generator.utils.security_type import SecurityType
 
 if TYPE_CHECKING:
@@ -41,31 +40,31 @@
     flask_app = sdk._flask_app
     swagger_open_api_cache_file = os.path.join(APPLICATION_TMP, f"swagger-{SLUG_REPLACE_RE.sub('_', flask_app.import_name).lower()}-{int(time.time())}.yml")
 
     from flask_swagger_ui import get_swaggerui_blueprint  # type: ignore
 
     bp = get_swaggerui_blueprint(
         blueprint_name='swagger_ui',
-        base_url=ApiPathVersion.NO_VERSION.compile_path(API_PATH__SWAGGER, api_route_path_prefix),
-        api_url=ApiPathVersion.NO_VERSION.compile_path(API_PATH__SWAGGER_SPEC, api_route_path_prefix),
+        base_url=ApiPathVersion.NO_VERSION.compile_path(APPLICATION_SWAGGER_PATH, api_route_path_prefix),
+        api_url=ApiPathVersion.NO_VERSION.compile_path(APPLICATION_SWAGGER_SPECIFICATION_PATH, api_route_path_prefix),
     )
 
     @bp.after_request
     def after_request(response: Response) -> Response:
         d = Debugger(flask_app.import_name, sdk._debugger_enabled_with_pin(), ApiMethod(request.method), request.url)
         if isinstance(response.response, list) and b'<!DOCTYPE html>' in response.response[0]:
             resp = response.get_data(as_text=True)
             resp = resp.replace('</body>', f'{d.render_html(response.status_code)}</body>')
             resp = resp.replace('<head>', f'<head>{AJAX_INTERSEPTOR}')
             response.set_data(resp)
         return response
 
     flask_app.register_blueprint(bp)
 
-    @sdk.rest_api('GET', API_PATH__SWAGGER_SPEC, v=ApiPathVersion.NO_VERSION, access=GLOBAL_PERMISSION__PUBLIC, config=ApiResourceConfig(swagger_disabled=True))
+    @sdk.rest_api('GET', APPLICATION_SWAGGER_SPECIFICATION_PATH, v=ApiPathVersion.NO_VERSION, access=GLOBAL_PERMISSION__PUBLIC, config=ApiResourceConfig(swagger_disabled=True))
     def swagger_specification(api_resource: ApiResource) -> EmptyJsonApiResponse:
         try:
             if not os.path.exists(swagger_open_api_cache_file):
                 with open(swagger_open_api_cache_file, 'wt') as f:
                     specifier = SwaggerThreeSpecifier()
                     _index_endpoints(specifier, [r for r in resources if APPLICATION_F.has_or_unset(r.access.flags)])
                     specifier.set_application_name('API')
```

### Comparing `ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/custom_widgets/custom_select_widget.py` & `ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/custom_widgets/custom_select_widget.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/custom_widgets/custom_text_input_widget.py` & `ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/custom_widgets/custom_text_input_widget.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/resources/web_forms/uni_form.py` & `ul-api-utils-7.9.3/ul_api_utils/resources/web_forms/uni_form.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/sentry.py` & `ul-api-utils-7.9.3/ul_api_utils/sentry.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/__tests__/api_path_version.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/__tests__/api_path_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/__tests__/unwrap_typing.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/__tests__/unwrap_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/api_encoding.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/api_encoding.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/api_format.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/api_format.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/api_method.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/api_method.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/api_pagination.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/api_pagination.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/api_path_version.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/api_path_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/avro.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/avro.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/broker_topics_message_count.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/broker_topics_message_count.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/cached_per_request.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/cached_per_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/colors.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/deprecated.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/flags.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/flags.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/json_encoder.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/load_modules.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/load_modules.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/token_check_through_request.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/token_check_through_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/unwrap_typing.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/unwrap_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/utils/uuid_converter.py` & `ul-api-utils-7.9.3/ul_api_utils/utils/uuid_converter.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/validators/__tests__/test_custom_fields.py` & `ul-api-utils-7.9.3/ul_api_utils/validators/__tests__/test_custom_fields.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils/validators/custom_fields.py` & `ul-api-utils-7.9.3/ul_api_utils/validators/custom_fields.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils.egg-info/PKG-INFO` & `ul-api-utils-7.9.3/ul_api_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-api-utils
-Version: 7.9.2
+Version: 7.9.3
 Summary: Python api utils
 Author: Unic-lab
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-api-utils-7.9.2/ul_api_utils.egg-info/SOURCES.txt` & `ul-api-utils-7.9.3/ul_api_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.9.2/ul_api_utils.egg-info/requires.txt` & `ul-api-utils-7.9.3/ul_api_utils.egg-info/requires.txt`

 * *Files identical despite different names*

