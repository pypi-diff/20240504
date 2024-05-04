# Comparing `tmp/scrutinydebugger-0.1.0.tar.gz` & `tmp/scrutinydebugger-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrutinydebugger-0.1.0.tar", last modified: Sun Mar 31 23:47:33 2024, max compression
+gzip compressed data, was "scrutinydebugger-0.2.0.tar", last modified: Sat May  4 13:41:43 2024, max compression
```

## Comparing `scrutinydebugger-0.1.0.tar` & `scrutinydebugger-0.2.0.tar`

### file list

```diff
@@ -1,140 +1,145 @@
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:33.000341 scrutinydebugger-0.1.0/
--rw-rw-r--   0 py        (1000) py        (1000)     1073 2024-03-25 03:09:50.000000 scrutinydebugger-0.1.0/LICENSE
--rw-r--r--   0 py        (1000) py        (1000)      887 2024-03-31 23:47:33.000341 scrutinydebugger-0.1.0/PKG-INFO
--rw-rw-r--   0 py        (1000) py        (1000)      815 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/README.md
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.980341 scrutinydebugger-0.1.0/scrutiny/
--rw-rw-r--   0 py        (1000) py        (1000)      188 2024-03-31 23:46:59.000000 scrutinydebugger-0.1.0/scrutiny/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)      453 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/__main__.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.980341 scrutinydebugger-0.1.0/scrutiny/cli/
--rw-rw-r--   0 py        (1000) py        (1000)       39 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     5078 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/cli.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.980341 scrutinydebugger-0.1.0/scrutiny/cli/commands/
--rw-rw-r--   0 py        (1000) py        (1000)     1577 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     5166 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/add_alias.py
--rw-rw-r--   0 py        (1000) py        (1000)     1323 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/base_command.py
--rw-rw-r--   0 py        (1000) py        (1000)     2774 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/datalog_info.py
--rw-rw-r--   0 py        (1000) py        (1000)     1359 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/delete_datalog.py
--rw-rw-r--   0 py        (1000) py        (1000)     1944 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/elf2varmap.py
--rw-rw-r--   0 py        (1000) py        (1000)     1621 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/export_datalog.py
--rw-rw-r--   0 py        (1000) py        (1000)     1974 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/get_firmware_id.py
--rw-rw-r--   0 py        (1000) py        (1000)     1249 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/install_sfd.py
--rw-rw-r--   0 py        (1000) py        (1000)     2024 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/launch_server.py
--rw-rw-r--   0 py        (1000) py        (1000)     5569 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/list_datalog.py
--rw-rw-r--   0 py        (1000) py        (1000)     3746 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/list_sfd.py
--rw-rw-r--   0 py        (1000) py        (1000)     2719 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/make_metadata.py
--rw-rw-r--   0 py        (1000) py        (1000)     1472 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/make_sfd.py
--rw-rw-r--   0 py        (1000) py        (1000)     3654 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/runtest.py
--rw-rw-r--   0 py        (1000) py        (1000)     1801 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/tag_firmware_id.py
--rw-rw-r--   0 py        (1000) py        (1000)     1241 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/cli/commands/uninstall_sfd.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.984341 scrutinydebugger-0.1.0/scrutiny/core/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     7065 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/alias.py
--rw-rw-r--   0 py        (1000) py        (1000)     5963 2024-03-26 02:00:31.000000 scrutinydebugger-0.1.0/scrutiny/core/basic_types.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.984341 scrutinydebugger-0.1.0/scrutiny/core/bintools/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/bintools/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1924 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/bintools/demangler.py
--rw-rw-r--   0 py        (1000) py        (1000)    26802 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/bintools/elf_dwarf_var_extractor.py
--rw-rw-r--   0 py        (1000) py        (1000)      223 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/bintools/elftools_stubs.py
--rw-rw-r--   0 py        (1000) py        (1000)      532 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/bintools/elftools_stubs.pyi
--rw-rw-r--   0 py        (1000) py        (1000)      755 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/bintools/get_var_memrange.py
--rw-rw-r--   0 py        (1000) py        (1000)     5385 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/codecs.py
--rw-rw-r--   0 py        (1000) py        (1000)     7523 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/datalogging.py
--rw-rw-r--   0 py        (1000) py        (1000)    10600 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/firmware_description.py
--rw-rw-r--   0 py        (1000) py        (1000)      402 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/firmware_id.py
--rw-rw-r--   0 py        (1000) py        (1000)     3653 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/firmware_parser.py
--rw-rw-r--   0 py        (1000) py        (1000)    14113 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/memory_content.py
--rw-rw-r--   0 py        (1000) py        (1000)     6809 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/sfd_storage.py
--rw-rw-r--   0 py        (1000) py        (1000)      787 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/typehints.py
--rw-rw-r--   0 py        (1000) py        (1000)     2811 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/validation.py
--rw-rw-r--   0 py        (1000) py        (1000)    13242 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/variable.py
--rw-rw-r--   0 py        (1000) py        (1000)    10651 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/core/varmap.py
--rw-rw-r--   0 py        (1000) py        (1000)      290 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/exceptions.py
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-27 04:12:19.000000 scrutinydebugger-0.1.0/scrutiny/py.typed
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.988341 scrutinydebugger-0.1.0/scrutiny/sdk/
--rw-rw-r--   0 py        (1000) py        (1000)      350 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/sdk/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    35224 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/sdk/_api_parser.py
--rw-rw-r--   0 py        (1000) py        (1000)    72780 2024-03-27 04:12:19.000000 scrutinydebugger-0.1.0/scrutiny/sdk/client.py
--rw-rw-r--   0 py        (1000) py        (1000)    23041 2024-03-27 04:12:19.000000 scrutinydebugger-0.1.0/scrutiny/sdk/datalogging.py
--rw-rw-r--   0 py        (1000) py        (1000)    13027 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/sdk/definitions.py
--rw-rw-r--   0 py        (1000) py        (1000)     1539 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/sdk/exceptions.py
--rw-rw-r--   0 py        (1000) py        (1000)     9981 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/sdk/watchable_handle.py
--rw-rw-r--   0 py        (1000) py        (1000)     3707 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/sdk/write_request.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.988341 scrutinydebugger-0.1.0/scrutiny/server/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     8039 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/active_sfd_handler.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.988341 scrutinydebugger-0.1.0/scrutiny/server/api/
--rw-rw-r--   0 py        (1000) py        (1000)    79375 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/api/API.py
--rw-rw-r--   0 py        (1000) py        (1000)       64 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/api/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1203 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/api/abstract_client_handler.py
--rw-rw-r--   0 py        (1000) py        (1000)     5976 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/api/dummy_client_handler.py
--rw-rw-r--   0 py        (1000) py        (1000)    11174 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/api/typing.py
--rw-rw-r--   0 py        (1000) py        (1000)     2868 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/api/value_streamer.py
--rw-rw-r--   0 py        (1000) py        (1000)     4652 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/api/websocket_client_handler.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.988341 scrutinydebugger-0.1.0/scrutiny/server/datalogging/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/datalogging/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    28543 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/datalogging/datalogging_manager.py
--rw-rw-r--   0 py        (1000) py        (1000)    22438 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/datalogging/datalogging_storage.py
--rw-rw-r--   0 py        (1000) py        (1000)     2294 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/datalogging/datalogging_utilities.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.992341 scrutinydebugger-0.1.0/scrutiny/server/datalogging/definitions/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/datalogging/definitions/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     2771 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/datalogging/definitions/api.py
--rw-rw-r--   0 py        (1000) py        (1000)    11122 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/datalogging/definitions/device.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.992341 scrutinydebugger-0.1.0/scrutiny/server/datastore/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/datastore/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    14837 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/datastore/datastore.py
--rw-rw-r--   0 py        (1000) py        (1000)    16643 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/datastore/datastore_entry.py
--rw-rw-r--   0 py        (1000) py        (1000)      716 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/datastore/entry_type.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.992341 scrutinydebugger-0.1.0/scrutiny/server/device/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    48034 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/device_handler.py
--rw-rw-r--   0 py        (1000) py        (1000)     5021 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/device_info.py
--rw-rw-r--   0 py        (1000) py        (1000)    50160 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/emulated_device.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.992341 scrutinydebugger-0.1.0/scrutiny/server/device/links/
--rw-rw-r--   0 py        (1000) py        (1000)       94 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/links/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1946 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/links/abstract_link.py
--rw-rw-r--   0 py        (1000) py        (1000)     5921 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/links/dummy_link.py
--rw-rw-r--   0 py        (1000) py        (1000)     6997 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/links/serial_link.py
--rw-rw-r--   0 py        (1000) py        (1000)     5386 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/links/udp_link.py
--rw-rw-r--   0 py        (1000) py        (1000)     9056 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/request_dispatcher.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.992341 scrutinydebugger-0.1.0/scrutiny/server/device/submodules/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/submodules/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    37665 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/submodules/datalogging_poller.py
--rw-rw-r--   0 py        (1000) py        (1000)     6325 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/submodules/device_searcher.py
--rw-rw-r--   0 py        (1000) py        (1000)     6513 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/submodules/heartbeat_generator.py
--rw-rw-r--   0 py        (1000) py        (1000)    28019 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/submodules/info_poller.py
--rw-rw-r--   0 py        (1000) py        (1000)    30808 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/submodules/memory_reader.py
--rw-rw-r--   0 py        (1000) py        (1000)    25434 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/submodules/memory_writer.py
--rw-rw-r--   0 py        (1000) py        (1000)     6047 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/device/submodules/session_initializer.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.996341 scrutinydebugger-0.1.0/scrutiny/server/protocol/
--rw-rw-r--   0 py        (1000) py        (1000)      191 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    15732 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/comm_handler.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.996341 scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/
--rw-rw-r--   0 py        (1000) py        (1000)      360 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1639 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/base_command.py
--rw-rw-r--   0 py        (1000) py        (1000)     1084 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/comm_control.py
--rw-rw-r--   0 py        (1000) py        (1000)     1439 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/datalog_control.py
--rw-rw-r--   0 py        (1000) py        (1000)      517 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/dummy_command.py
--rw-rw-r--   0 py        (1000) py        (1000)     1738 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/get_info.py
--rw-rw-r--   0 py        (1000) py        (1000)     1448 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/memory_control.py
--rw-rw-r--   0 py        (1000) py        (1000)      481 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/user_command.py
--rw-rw-r--   0 py        (1000) py        (1000)      622 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/crc32.py
--rw-rw-r--   0 py        (1000) py        (1000)      790 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/exceptions.py
--rw-rw-r--   0 py        (1000) py        (1000)    61575 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/protocol.py
--rw-rw-r--   0 py        (1000) py        (1000)     4218 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/request.py
--rw-rw-r--   0 py        (1000) py        (1000)     4315 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/response.py
--rw-rw-r--   0 py        (1000) py        (1000)     6527 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/protocol/typing.py
--rw-rw-r--   0 py        (1000) py        (1000)     5311 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/server/server.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:32.996341 scrutinydebugger-0.1.0/scrutiny/tools/
--rw-rw-r--   0 py        (1000) py        (1000)      101 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/tools/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     4733 2024-03-27 04:12:19.000000 scrutinydebugger-0.1.0/scrutiny/tools/synchronous_websocket_server.py
--rw-rw-r--   0 py        (1000) py        (1000)     5426 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/tools/throttler.py
--rw-rw-r--   0 py        (1000) py        (1000)     1277 2024-03-25 02:32:28.000000 scrutinydebugger-0.1.0/scrutiny/tools/timer.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-03-31 23:47:33.000341 scrutinydebugger-0.1.0/scrutinydebugger.egg-info/
--rw-r--r--   0 py        (1000) py        (1000)      887 2024-03-31 23:47:32.000000 scrutinydebugger-0.1.0/scrutinydebugger.egg-info/PKG-INFO
--rw-rw-r--   0 py        (1000) py        (1000)     4418 2024-03-31 23:47:32.000000 scrutinydebugger-0.1.0/scrutinydebugger.egg-info/SOURCES.txt
--rw-rw-r--   0 py        (1000) py        (1000)        1 2024-03-31 23:47:32.000000 scrutinydebugger-0.1.0/scrutinydebugger.egg-info/dependency_links.txt
--rw-rw-r--   0 py        (1000) py        (1000)       52 2024-03-31 23:47:32.000000 scrutinydebugger-0.1.0/scrutinydebugger.egg-info/entry_points.txt
--rw-rw-r--   0 py        (1000) py        (1000)      222 2024-03-31 23:47:32.000000 scrutinydebugger-0.1.0/scrutinydebugger.egg-info/requires.txt
--rw-rw-r--   0 py        (1000) py        (1000)        9 2024-03-31 23:47:32.000000 scrutinydebugger-0.1.0/scrutinydebugger.egg-info/top_level.txt
--rw-rw-r--   0 py        (1000) py        (1000)       38 2024-03-31 23:47:33.000341 scrutinydebugger-0.1.0/setup.cfg
--rw-rw-r--   0 py        (1000) py        (1000)     1403 2024-03-27 04:12:19.000000 scrutinydebugger-0.1.0/setup.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.279700 scrutinydebugger-0.2.0/
+-rw-rw-r--   0 py        (1000) py        (1000)     1073 2024-03-25 03:09:50.000000 scrutinydebugger-0.2.0/LICENSE
+-rw-r--r--   0 py        (1000) py        (1000)      887 2024-05-04 13:41:43.279700 scrutinydebugger-0.2.0/PKG-INFO
+-rw-rw-r--   0 py        (1000) py        (1000)      596 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/README.md
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.259700 scrutinydebugger-0.2.0/scrutiny/
+-rw-rw-r--   0 py        (1000) py        (1000)      188 2024-05-04 13:40:52.000000 scrutinydebugger-0.2.0/scrutiny/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)      453 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/__main__.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.259700 scrutinydebugger-0.2.0/scrutiny/cli/
+-rw-rw-r--   0 py        (1000) py        (1000)       39 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/cli/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5089 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/cli.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.263700 scrutinydebugger-0.2.0/scrutiny/cli/commands/
+-rw-rw-r--   0 py        (1000) py        (1000)     1577 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5166 2024-04-15 02:52:23.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/add_alias.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1431 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/base_command.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2774 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/datalog_info.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1481 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/delete_datalog.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2148 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/elf2varmap.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1699 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/export_datalog.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2082 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/get_firmware_id.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1314 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/install_sfd.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2024 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/launch_server.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5569 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/list_datalog.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3746 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/list_sfd.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2880 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/make_metadata.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1641 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/make_sfd.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3618 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/runtest.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1970 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/tag_firmware_id.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1498 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/uninstall_sfd.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.263700 scrutinydebugger-0.2.0/scrutiny/core/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/core/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     7134 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/core/alias.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5938 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/core/basic_types.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.263700 scrutinydebugger-0.2.0/scrutiny/core/bintools/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/core/bintools/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1924 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/bintools/demangler.py
+-rw-rw-r--   0 py        (1000) py        (1000)    31787 2024-05-03 19:11:00.000000 scrutinydebugger-0.2.0/scrutiny/core/bintools/elf_dwarf_var_extractor.py
+-rw-rw-r--   0 py        (1000) py        (1000)      223 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/bintools/elftools_stubs.py
+-rw-rw-r--   0 py        (1000) py        (1000)      547 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/core/bintools/elftools_stubs.pyi
+-rw-rw-r--   0 py        (1000) py        (1000)      755 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/bintools/get_var_memrange.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5385 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/codecs.py
+-rw-rw-r--   0 py        (1000) py        (1000)     7670 2024-04-21 14:05:12.000000 scrutinydebugger-0.2.0/scrutiny/core/datalogging.py
+-rw-rw-r--   0 py        (1000) py        (1000)    10600 2024-04-21 03:45:36.000000 scrutinydebugger-0.2.0/scrutiny/core/firmware_description.py
+-rw-rw-r--   0 py        (1000) py        (1000)      402 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/firmware_id.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3653 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/firmware_parser.py
+-rw-rw-r--   0 py        (1000) py        (1000)    14117 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/core/memory_content.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6939 2024-04-15 02:52:23.000000 scrutinydebugger-0.2.0/scrutiny/core/sfd_storage.py
+-rw-rw-r--   0 py        (1000) py        (1000)      787 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/typehints.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3000 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/core/validation.py
+-rw-rw-r--   0 py        (1000) py        (1000)    13755 2024-05-03 19:11:00.000000 scrutinydebugger-0.2.0/scrutiny/core/variable.py
+-rw-rw-r--   0 py        (1000) py        (1000)    10690 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/core/varmap.py
+-rw-rw-r--   0 py        (1000) py        (1000)      290 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/exceptions.py
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-27 04:12:19.000000 scrutinydebugger-0.2.0/scrutiny/py.typed
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.267700 scrutinydebugger-0.2.0/scrutiny/sdk/
+-rw-rw-r--   0 py        (1000) py        (1000)      350 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/sdk/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    35478 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/sdk/_api_parser.py
+-rw-rw-r--   0 py        (1000) py        (1000)    73474 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/sdk/client.py
+-rw-rw-r--   0 py        (1000) py        (1000)    23098 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/sdk/datalogging.py
+-rw-rw-r--   0 py        (1000) py        (1000)    13027 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/sdk/definitions.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1539 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/sdk/exceptions.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.267700 scrutinydebugger-0.2.0/scrutiny/sdk/listeners/
+-rw-rw-r--   0 py        (1000) py        (1000)    11930 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/sdk/listeners/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1365 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/sdk/listeners/buffered_reader_listener.py
+-rw-rw-r--   0 py        (1000) py        (1000)    10506 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/sdk/listeners/csv_file_listener.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2127 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/sdk/listeners/text_stream_listener.py
+-rw-rw-r--   0 py        (1000) py        (1000)     9981 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/sdk/watchable_handle.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3707 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/sdk/write_request.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.267700 scrutinydebugger-0.2.0/scrutiny/server/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     8039 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/active_sfd_handler.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.267700 scrutinydebugger-0.2.0/scrutiny/server/api/
+-rw-rw-r--   0 py        (1000) py        (1000)    79420 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/api/API.py
+-rw-rw-r--   0 py        (1000) py        (1000)       64 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/api/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1203 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/api/abstract_client_handler.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5976 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/api/dummy_client_handler.py
+-rw-rw-r--   0 py        (1000) py        (1000)    11185 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/api/typing.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2868 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/api/value_streamer.py
+-rw-rw-r--   0 py        (1000) py        (1000)     4652 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/api/websocket_client_handler.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.267700 scrutinydebugger-0.2.0/scrutiny/server/datalogging/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    29373 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/datalogging_manager.py
+-rw-rw-r--   0 py        (1000) py        (1000)    22438 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/datalogging_storage.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2294 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/datalogging_utilities.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.271700 scrutinydebugger-0.2.0/scrutiny/server/datalogging/definitions/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/definitions/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2771 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/definitions/api.py
+-rw-rw-r--   0 py        (1000) py        (1000)    11122 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/definitions/device.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.271700 scrutinydebugger-0.2.0/scrutiny/server/datastore/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/datastore/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    14837 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/datastore/datastore.py
+-rw-rw-r--   0 py        (1000) py        (1000)    17593 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/datastore/datastore_entry.py
+-rw-rw-r--   0 py        (1000) py        (1000)      716 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/datastore/entry_type.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.271700 scrutinydebugger-0.2.0/scrutiny/server/device/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/device/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    48107 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/device/device_handler.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5021 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/device_info.py
+-rw-rw-r--   0 py        (1000) py        (1000)    50160 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/emulated_device.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.271700 scrutinydebugger-0.2.0/scrutiny/server/device/links/
+-rw-rw-r--   0 py        (1000) py        (1000)       94 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/device/links/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1946 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/links/abstract_link.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5921 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/links/dummy_link.py
+-rw-rw-r--   0 py        (1000) py        (1000)     7384 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/device/links/serial_link.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5386 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/links/udp_link.py
+-rw-rw-r--   0 py        (1000) py        (1000)     9056 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/request_dispatcher.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.271700 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    37665 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/datalogging_poller.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6350 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/device_searcher.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6341 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/heartbeat_generator.py
+-rw-rw-r--   0 py        (1000) py        (1000)    28019 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/info_poller.py
+-rw-rw-r--   0 py        (1000) py        (1000)    30897 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/memory_reader.py
+-rw-rw-r--   0 py        (1000) py        (1000)    25434 2024-04-19 01:49:41.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/memory_writer.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6047 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/session_initializer.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.275700 scrutinydebugger-0.2.0/scrutiny/server/protocol/
+-rw-rw-r--   0 py        (1000) py        (1000)      191 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    15748 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/comm_handler.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.275700 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/
+-rw-rw-r--   0 py        (1000) py        (1000)      360 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1639 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/base_command.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1084 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/comm_control.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1439 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/datalog_control.py
+-rw-rw-r--   0 py        (1000) py        (1000)      517 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/dummy_command.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1738 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/get_info.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1448 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/memory_control.py
+-rw-rw-r--   0 py        (1000) py        (1000)      481 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/user_command.py
+-rw-rw-r--   0 py        (1000) py        (1000)      622 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/crc32.py
+-rw-rw-r--   0 py        (1000) py        (1000)      790 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/exceptions.py
+-rw-rw-r--   0 py        (1000) py        (1000)    61707 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/protocol.py
+-rw-rw-r--   0 py        (1000) py        (1000)     4218 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/request.py
+-rw-rw-r--   0 py        (1000) py        (1000)     4315 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/response.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6527 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/typing.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5269 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/server.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.275700 scrutinydebugger-0.2.0/scrutiny/tools/
+-rw-rw-r--   0 py        (1000) py        (1000)      101 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/tools/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     4733 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/tools/synchronous_websocket_server.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5442 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/tools/throttler.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1287 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/tools/timer.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.275700 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/
+-rw-r--r--   0 py        (1000) py        (1000)      887 2024-05-04 13:41:43.000000 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/PKG-INFO
+-rw-rw-r--   0 py        (1000) py        (1000)     4595 2024-05-04 13:41:43.000000 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/SOURCES.txt
+-rw-rw-r--   0 py        (1000) py        (1000)        1 2024-05-04 13:41:43.000000 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/dependency_links.txt
+-rw-rw-r--   0 py        (1000) py        (1000)       52 2024-05-04 13:41:43.000000 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/entry_points.txt
+-rw-rw-r--   0 py        (1000) py        (1000)      222 2024-05-04 13:41:43.000000 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/requires.txt
+-rw-rw-r--   0 py        (1000) py        (1000)        9 2024-05-04 13:41:43.000000 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/top_level.txt
+-rw-rw-r--   0 py        (1000) py        (1000)       38 2024-05-04 13:41:43.279700 scrutinydebugger-0.2.0/setup.cfg
+-rw-rw-r--   0 py        (1000) py        (1000)     1403 2024-03-27 04:12:19.000000 scrutinydebugger-0.2.0/setup.py
```

### Comparing `scrutinydebugger-0.1.0/LICENSE` & `scrutinydebugger-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/PKG-INFO` & `scrutinydebugger-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrutinydebugger
-Version: 0.1.0
+Version: 0.2.0
 Summary: Scrutiny debugger Python framework
 Home-page: https://github.com/scrutinydebugger/scrutiny-python
 Author: Pier-Yves Lessard
 License: MIT
 Requires-Python: >3.8
 License-File: LICENSE
 Requires-Dist: appdirs>=1.4.4
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/cli.py` & `scrutinydebugger-0.2.0/scrutiny/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,16 @@
 
         error = None
         try:
             logging_level_str = cargs.loglevel if cargs.loglevel else self.default_log_level
             logging_level = getattr(logging, logging_level_str.upper())
             format_string = ""
             if logging_level == logging.DEBUG:
-                format_string += "%(relativeCreated)s "    
-            format_string += '[%(levelname)s] %(message)s'
+                format_string += "%(relativeCreated)d "    
+            format_string += '[%(levelname)s] <%(name)s> %(message)s'
             logging.basicConfig(level=logging_level, filename=cargs.logfile, format=format_string)
             if cargs.disable_loggers is not None:
                 for logger_name in cargs.disable_loggers.split(','):
                     logging.getLogger(logger_name).disabled = True
 
             for cmd in self.command_list:
                 if cmd.get_name() == cargs.command:
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/__init__.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/add_alias.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/add_alias.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     parser: argparse.ArgumentParser
 
     def __init__(self, args: List[str], requested_log_level: Optional[str] = None):
         self.logger = logging.getLogger('CLI')
         self.args = args
         self.parser = argparse.ArgumentParser(prog=self.get_prog())
         self.parser.add_argument(
-            'destination', help='Where to add the alias. Can be an SFD file, a folder of a in making SFD file or a firmware ID to alter an already installed SFD file.')
+            'destination', help='Where to add the alias. Can be an SFD file, a folder of a in-making SFD file or a firmware ID to alter an already installed SFD file.')
         self.parser.add_argument('--file', help='The input alias file in .json format')
 
         self.parser.add_argument('--fullpath', help='The alias fullpath')
         self.parser.add_argument('--target', help='The target of the alias')
         self.parser.add_argument('--gain', help='The gain to apply when reading the alias')
         self.parser.add_argument('--offset', help='The offset to apply when reading the alias')
         self.parser.add_argument('--min', help='The minimum value for this alias')
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/base_command.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/base_command.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #   - License : MIT - See LICENSE file.
 #   - Project :  Scrutiny Debugger (github.com/scrutinydebugger/scrutiny-python)
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
 from abc import ABC, abstractmethod
 from typing import List, Optional
-
+import logging
 
 class BaseCommand(ABC):
     _cmd_name_: str
     _brief_: str
     _group_: str
 
     @classmethod
@@ -43,7 +43,10 @@
     def run(self) -> Optional[int]:
         """Executes a command"""
         pass
 
     @abstractmethod
     def __init__(self, args: List[str], requested_log_level: Optional[str] = None):
         pass
+
+    def getLogger(self) -> logging.Logger:
+        return logging.getLogger(self._cmd_name_)
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/datalog_info.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/datalog_info.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/delete_datalog.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/delete_datalog.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,13 +27,15 @@
 
     def run(self) -> Optional[int]:
         from scrutiny.server.datalogging.datalogging_storage import DataloggingStorage
 
         args = self.parser.parse_args(self.args)
         if args.all:
             DataloggingStorage.clear_all()
+            self.getLogger().info("All datalogs deleted")
         elif args.id:
             DataloggingStorage.initialize()
             DataloggingStorage.delete(args.id)
+            self.getLogger().info(f"Datalog {args.id} deleted")
         else:
             raise ValueError("An acquisition ID must be provided or --all")
         return 0
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/elf2varmap.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/elf2varmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     def __init__(self, args: List[str], requested_log_level: Optional[str] = None):
         self.args = args
         self.parser = argparse.ArgumentParser(prog=self.get_prog())
         self.parser.add_argument('file', help='The ELF file to read')
         self.parser.add_argument('--cppfilt', default=None, help='The path to the c++filt used demangler when parsing a binary produced by GCC')
         self.parser.add_argument('--output', default=None, help='The varmap output file. Will go to STDOUT if not set')
+        self.parser.add_argument('--indent', default=4, type=int, help='Number of spaces for JSON indentation')
 
     def run(self) -> Optional[int]:
         from scrutiny.core.bintools.elf_dwarf_var_extractor import ElfDwarfVarExtractor
 
         args = self.parser.parse_args(self.args)
         extractor = ElfDwarfVarExtractor(args.file, cppfilt=args.cppfilt)
         varmap = extractor.get_varmap()
@@ -44,10 +45,11 @@
                 output_file = os.path.join(args.output, 'varmap.json')
             else:
                 output_file = args.output
 
             if os.path.isfile(output_file):
                 logging.warning('File %s already exist. Overwritting' % output_file)
 
-            varmap.write(output_file)
+            varmap.write(output_file, indent=args.indent)
+            self.getLogger().info(f"Varmap file {output_file} written")
 
         return 0
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/export_datalog.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/export_datalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,9 +38,10 @@
         if not self.parsed_args.csv:
             raise ValueError("At least one  export method must be specified")
 
         acquisition = DataloggingStorage.read(reference_id=self.parsed_args.reference_id)
 
         if self.parsed_args.csv:
             acquisition.to_csv(self.parsed_args.csv)
+            self.getLogger().info(f"CSV file {self.parsed_args.csv} written")
 
         return 0
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/get_firmware_id.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/get_firmware_id.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,9 +51,10 @@
             parser.throw_no_tag_error()
 
         if output_file is None:
             print(parser.get_firmware_id_ascii(), flush=True, end='')
         else:
             with open(output_file, 'w') as f:
                 f.write(parser.get_firmware_id_ascii())
+            self.getLogger().info(f"Firmware ID {parser.get_firmware_id_ascii()} written to {output_file}")
 
         return 0
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/install_sfd.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/install_sfd.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,9 +26,10 @@
         self.parser.add_argument('file', help='Scrutiny Firmware Description (SFD) file to be installed')
 
     def run(self) -> Optional[int]:
         from scrutiny.core.sfd_storage import SFDStorage
 
         args = self.parser.parse_args(self.args)
         SFDStorage.install(args.file)
+        self.getLogger().info(f"SFD file {args.file} installed")
 
         return 0
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/launch_server.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/launch_server.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/list_datalog.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/list_datalog.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/list_sfd.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/list_sfd.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/make_metadata.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/make_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import argparse
 from .base_command import BaseCommand
 import json
 import os
 import datetime
 import platform
 from typing import Optional, List
+import logging
 
 
 class MakeMetadata(BaseCommand):
     _cmd_name_ = 'make-metadata'
     _brief_ = 'Generate a .json file containing the metadata used inside a SFD (Scrutiny Firmware Description)'
     _group_ = 'Build Toolchain'
 
@@ -48,14 +49,15 @@
             output_file = os.path.join(args.output, self.DEFAULT_NAME)
         else:
             output_file = args.output
 
         try:
             scrutiny_version = scrutiny.__version__
         except Exception:
+            self.getLogger().warning("Could not find the scrutiny version")
             scrutiny_version = '0.0.0'
 
         metadata: MetadataType = {
             'project_name': args.project_name,
             'author': args.author,
             'version': args.version,
             'generation_info': {
@@ -64,9 +66,10 @@
                 'scrutiny_version': scrutiny_version,
                 'system_type': platform.system()
             }
         }
 
         with open(output_file, 'w') as f:
             f.write(json.dumps(metadata, indent=4))
+        self.getLogger().info(f"Metadata file {output_file} written")
 
         return 0
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/make_sfd.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/make_sfd.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #   - Project :  Scrutiny Debugger (github.com/scrutinydebugger/scrutiny-python)
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
 import argparse
 from .base_command import BaseCommand
 from typing import Optional, List
+import logging
 
 
 class MakeSFD(BaseCommand):
     _cmd_name_ = 'make-sfd'
     _brief_ = 'Generates a SFD file (Scrutiny Firmware Description) from a given folder containing the required files.'
     _group_ = 'Build Toolchain'
 
@@ -20,20 +21,22 @@
     parser: argparse.ArgumentParser
 
     def __init__(self, args: List[str], requested_log_level: Optional[str] = None):
         self.args = args
         self.parser = argparse.ArgumentParser(prog=self.get_prog())
         self.parser.add_argument('folder', help='Folder containing the firmware description files.')
         self.parser.add_argument('output', help='Destination file')
-        self.parser.add_argument('--install', action="store_true", help='Install the firmware info file after making it')
+        self.parser.add_argument('--install', action="store_true", default=False, help='Install the firmware info file after making it')
 
     def run(self) -> Optional[int]:
-        from scrutiny.core.firmware_description import FirmwareDescription
-        from scrutiny.core.sfd_storage import SFDStorage
+        from scrutiny.core.firmware_description import FirmwareDescription        
         args = self.parser.parse_args(self.args)
         sfd = FirmwareDescription(args.folder)
         sfd.write(args.output)
+        self.getLogger().info(f"SFD File {args.output} written")
 
         if args.install:
+            from scrutiny.core.sfd_storage import SFDStorage
             SFDStorage.install(args.output)
+            self.getLogger().info(f"{args.output} installed")
 
         return 0
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/runtest.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/runtest.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,18 +54,18 @@
         format_string += '[%(levelname)s] <%(name)s> %(message)s'
         logging.getLogger().handlers[0].setFormatter(logging.Formatter(format_string))
         logging.getLogger().setLevel(logging_level)
 
         import test  # load the test module.
         if not hasattr(test, '__scrutiny__'):   # Make sure this is Scrutiny Test folder (in case we run from install dir)
             if args.root is None:
-                logging.getLogger(self._cmd_name_).critical(
+                self.getLogger().critical(
                     'No scrutiny unit tests available in %s. Consider passing a test folder with --root if you run the tests from an installed module' % test_root)
             else:
-                logging.getLogger(self._cmd_name_).critical('No unit tests available in %s' % test_root)
+                self.getLogger().critical('No unit tests available in %s' % test_root)
         else:
             try:
                 loader = unittest.TestLoader()
                 if args.module is None:
                     suite = loader.discover(test_root)
                 else:
                     suite = loader.loadTestsFromName(args.module)
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/tag_firmware_id.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/tag_firmware_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,9 +43,11 @@
                 raise Exception('Output file is required')
 
         parser = FirmwareParser(src)
         if not parser.has_placeholder():
             parser.throw_no_tag_error()
 
         parser.write_tagged(args.dst)   # inplace if None
+        binname = args.dst if args.dst is not None else src
+        self.getLogger().info(f"Binary {binname} tagged with firmware ID: {parser.get_firmware_id_ascii()}")
 
         return 0
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/cli/commands/uninstall_sfd.py` & `scrutinydebugger-0.2.0/scrutiny/cli/commands/uninstall_sfd.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,10 +25,15 @@
         self.parser = argparse.ArgumentParser(prog=self.get_prog())
         self.parser.add_argument('firmwareid', help='Firmware ID of the Scrutiny Firmware Info')
         self.parser.add_argument('--quiet', action="store_true", help='Do not report error if not installed')
 
     def run(self) -> Optional[int]:
         from scrutiny.core.sfd_storage import SFDStorage
         args = self.parser.parse_args(self.args)
-        SFDStorage.uninstall(args.firmwareid, ignore_not_exist=args.quiet)
+        is_installed = SFDStorage.is_installed(args.firmwareid)
+        if is_installed:
+            SFDStorage.uninstall(args.firmwareid, ignore_not_exist=args.quiet)
+            self.getLogger().info(f"SFD {args.firmwareid} uninstalled")
+        else:
+            self.getLogger().info(f"SFD {args.firmwareid} was not installed")
 
         return 0
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/alias.py` & `scrutinydebugger-0.2.0/scrutiny/core/alias.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,19 +150,20 @@
 
     def get_gain(self) -> float:
         return self.gain if self.gain is not None else 1.0
 
     def get_offset(self) -> float:
         return self.offset if self.offset is not None else 0.0
 
-    def compute_user_to_device(self, value: Union[int, float, bool]) -> Union[int, float, bool]:
+    def compute_user_to_device(self, value: Union[int, float, bool], apply_saturation:bool=True) -> Union[int, float, bool]:
         """Transform the value received from the user before writing it to the device. Applies min, max, gain, offset"""
         if isinstance(value, int) or isinstance(value, float):
-            value = min(value, self.get_max())
-            value = max(value, self.get_min())
+            if apply_saturation:
+                value = min(value, self.get_max())
+                value = max(value, self.get_min())
             value -= self.get_offset()
             value /= self.get_gain()
         return value
 
     def compute_device_to_user(self, value: Union[int, float, bool]) -> Union[int, float, bool]:
         """Converts to value read from the device into a value that can be shown to the user. Applies gain and offset"""
         if isinstance(value, int) or isinstance(value, float):
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/basic_types.py` & `scrutinydebugger-0.2.0/scrutiny/core/basic_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     'DataTypeSize',
     'EmbeddedDataType',
     'RuntimePublishedValue',
     'MemoryRegion'
 ]
 
 from enum import Enum
-from typing import Union
 from dataclasses import dataclass
 from scrutiny.core import validation
 
 
 @dataclass(frozen=True)
 class MemoryRegion:
     """(Immutable struct)
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/bintools/demangler.py` & `scrutinydebugger-0.2.0/scrutiny/core/bintools/demangler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/bintools/elf_dwarf_var_extractor.py` & `scrutinydebugger-0.2.0/scrutiny/core/bintools/elf_dwarf_var_extractor.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,32 +7,62 @@
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
 __all__ = ['ElfDwarfVarExtractor']
 
 from elftools.elf.elffile import ELFFile
 import os
-from enum import Enum
+from enum import Enum, auto
 from .demangler import GccDemangler
 import logging
+import traceback
+import inspect
+from dataclasses import dataclass
+from inspect import currentframe
 
 from scrutiny.core.varmap import VarMap
 from scrutiny.core.basic_types import *
 from scrutiny.core.variable import *
 from scrutiny.exceptions import EnvionmentNotSetUpException
+from scrutiny.core.bintools import elftools_stubs
 
-from typing import Optional, List, Dict, Any, Union, cast, Iterable, Callable, Set, Tuple, TYPE_CHECKING
+from typing import Optional, List, Dict, Any, Union, cast, Iterable, Callable, Set, Tuple, TYPE_CHECKING, Tuple
 
-from scrutiny.core.bintools import elftools_stubs
 
 
+def get_linenumber() -> int:
+    cf = currentframe()
+    if cf is None:
+        return -1
+    if cf.f_back is None:
+        return -1
+    if cf.f_back.f_lineno is None:
+        return -1
+
+    return int(cf.f_back.f_lineno)
+
+class TypeOfVar(Enum):
+    BaseType=auto()
+    Struct=auto()
+    Class=auto()
+    Union=auto()
+    Pointer=auto()
+    Array=auto()
+
+@dataclass
+class TypeDescriptor:
+    type: TypeOfVar
+    enum_die:Optional[ "elftools_stubs.Die"]
+    type_die: "elftools_stubs.Die"
+
 class ElfParsingError(Exception):
     pass
 
 
+
 class CuName:
     """
     Handles a compile unit name. Useful to build a unique name as small as possible.
     """
     _class_internal_id = 0
     PATH_JOIN_CHAR = '_'
 
@@ -41,25 +71,27 @@
     filename: str
     display_name: str
     segments: List[str]
 
     def __init__(self, cu: "elftools_stubs.CompileUnit", fullpath: str) -> None:
         self.cu = cu
         self.fullpath = os.path.normpath(fullpath)
-        self.filename = os.path.basename(fullpath)
+        self.filename = os.path.basename(self.fullpath)
         self.display_name = self.filename
         self.segments = os.path.split(self.fullpath)[0].split(os.sep)
 
     def get_display_name(self) -> str:
         return self.display_name.replace('/', '-')
 
     def get_fullpath(self) -> str:
         return self.fullpath
 
     def go_up(self) -> None:
+        """Add a the closest directory name to the display name.
+        /aaa/bbb/ccc, ddd -->  /aaa/bbb, ccc_ddd"""
         if len(self.segments) > 0:
             last_dir = self.segments.pop()
             if last_dir == '':
                 raise ElfParsingError('Cannot go up')
             self.display_name = self.PATH_JOIN_CHAR.join([last_dir, self.display_name])
         else:
             raise ElfParsingError('Cannot go up')
@@ -72,15 +104,16 @@
                 return candidate
             i += 1
 
 
 class ElfDwarfVarExtractor:
     defaults_names = {
         'DW_TAG_structure_type': '<struct>',
-        'DW_TAG_enumeration_type': '<enum>'
+        'DW_TAG_enumeration_type': '<enum>',
+        'DW_TAG_union_type': '<union>'
     }
 
     STATIC = 'static'
     GLOBAL = 'global'
     MAX_CU_DISPLAY_NAME_LENGTH = 40
     DW_OP_ADDR = 3
 
@@ -120,18 +153,37 @@
         self.die2vartype_map = {}
         self.cu_name_map = {}   # maps a CompileUnit object to it's unique display name
         self.enum_die_map = {}
         self.struct_die_map = {}
         self.endianness = Endianness.Little
         self.cppfilt = cppfilt
         self.logger = logging.getLogger(self.__class__.__name__)
+        
+        self.logger.handlers
+        self.initial_stack_depth= len(inspect.stack())
 
         if filename is not None:
             self.load_from_elf_file(filename)
 
+    def make_name_for_log(self, die: "elftools_stubs.Die") -> str:
+        name=''
+        try:
+            name = self.get_name(die, nolog=True)
+        except:
+            pass
+        return f'{die.tag} <{die.offset:x}> "{name}"'
+
+    def log_debug_process_die(self, die: "elftools_stubs.Die") -> None:
+        if self.logger.isEnabledFor(logging.DEBUG):
+            stack_depth = len(inspect.stack()) - self.initial_stack_depth-1
+            stack_depth = max(stack_depth, 1)
+            funcname = inspect.stack()[1][3]
+            pad = '|  ' * (stack_depth - 1) + '|--'
+            self.logger.debug(f"{pad}{funcname}({self.make_name_for_log(die)})")
+
     def get_varmap(self) -> VarMap:
         return self.varmap
 
     # Builds a dictionary that maps a CompuleUnit object to a unique displayable name
     def make_cu_name_map(self, dwarfinfo: "elftools_stubs.ELFFile") -> None:
 
         fullpath_cu_tuple_list = []
@@ -139,17 +191,17 @@
         cu: "elftools_stubs.CompileUnit"
         for cu in dwarfinfo.iter_CUs():
             topdie: "elftools_stubs.Die" = cu.get_top_DIE()
             if topdie.tag != 'DW_TAG_compile_unit':
                 raise ElfParsingError('Top die should be a compile unit')
 
             comp_dir = None
-            name = self.get_name(topdie)
+            name = self.get_name(topdie, 'unnamed_cu')
             if 'DW_AT_comp_dir' in topdie.attributes:
-                comp_dir = topdie.attributes['DW_AT_comp_dir'].value.decode('ascii')
+                comp_dir = topdie.attributes['DW_AT_comp_dir'].value.decode('utf8')
                 fullpath = os.path.join(comp_dir, name)
             else:
                 fullpath = os.path.abspath(name)
 
             if fullpath in fullpath_set:
                 raise RuntimeError('Duplicate compile unit name')
             fullpath_set.add(fullpath)
@@ -205,29 +257,33 @@
             displayname_cu_tuple_list.append((displayname, displayname_map[displayname][0].cu))
         return displayname_cu_tuple_list
 
     def get_cu_name(self, die: "elftools_stubs.Die") -> str:
         return self.cu_name_map[die.cu]
 
     def get_die_at_spec(self, die: "elftools_stubs.Die") -> "elftools_stubs.Die":
+        self.log_debug_process_die(die)
         refaddr = cast(int, die.attributes['DW_AT_specification'].value) + die.cu.cu_offset
         return die.dwarfinfo.get_DIE_from_refaddr(refaddr)
 
-    def get_name(self, die: "elftools_stubs.Die", default: Optional[str] = None) -> str:
+    def get_name(self, die: "elftools_stubs.Die", default: Optional[str] = None, nolog:bool=False) -> str:
+        if not nolog:
+            self.log_debug_process_die(die)
         if 'DW_AT_name' in die.attributes:
             return cast(str, die.attributes['DW_AT_name'].value.decode('ascii'))
         else:
             if default is not None:
                 return default
             elif die.tag in self.defaults_names:
                 return self.defaults_names[die.tag]
             else:
                 raise ElfParsingError('Cannot get a name for this die. %s' % die)
 
     def get_linkage_name(self, die: "elftools_stubs.Die") -> str:
+        self.log_debug_process_die(die)
         return self.demangler.demangle(die.attributes['DW_AT_linkage_name'].value.decode('ascii'))
 
     # Tells if the die is accessible from outside the compile unit. If it is, it's global, otherwise it's static.
 
     def is_external(self, die: "elftools_stubs.Die") -> bool:
         try:
             return cast(bool, die.attributes['DW_AT_external'].value)
@@ -320,158 +376,180 @@
             self.make_cu_name_map(self.dwarfinfo)
             args = [self.cppfilt] if self.cppfilt is not None else []
             self.demangler = GccDemangler(*args)  # todo : adapt according to compile unit producer
 
             if not self.demangler.can_run():
                 raise EnvionmentNotSetUpException("Demangler cannot be used. %s" % self.demangler.get_error())
 
+            self.initial_stack_depth = len(inspect.stack())
+            
             for cu in self.dwarfinfo.iter_CUs():
                 die = cu.get_top_DIE()
-                self.extract_var_recursive(die)
+                self.extract_var_recursive(die) # Recursion start point
 
-    # Process each die recursively and call the right handler based on the die Tag
     def extract_var_recursive(self, die: "elftools_stubs.Die") -> None:
-        process_fn: Dict[str, Callable[["elftools_stubs.Die"], None]] = {
-            'DW_TAG_base_type': self.die_process_base_type,
-            'DW_TAG_variable': self.die_process_variable,
-            'DW_TAG_enumeration_type': self.die_process_enum,
-            'DW_TAG_enumerator': self.die_process_enum_val
-        }
+        # Finds all "variable" tags and create an entry in the varmap.
+        # Types / structures / enums are discovered as we go. We only take
+        # definitions that are used by a variables, the rest will be ignored.
 
-        if die.tag in process_fn:
-            process_fn[die.tag](die)
+        self.log_debug_process_die(die)
 
-        for child in die.iter_children():
-            self.extract_var_recursive(child)
+        if die.tag == 'DW_TAG_variable':
+            self.die_process_variable(die)  
 
+        for child in die.iter_children():
+            try:
+                self.extract_var_recursive(child)
+            except Exception as e:
+                self.logger.error(f"Failed to extract var under {child}. {e}")
+                self.logger.debug(traceback.format_exc()) 
+    
     def get_typename_from_die(self, die: "elftools_stubs.Die") -> str:
         return cast(bytes, die.attributes['DW_AT_name'].value).decode('ascii')
-
+    
     # Process die of type "base type". Register the type in the global index and maps it to a known type.
     def die_process_base_type(self, die: "elftools_stubs.Die") -> None:
+        self.log_debug_process_die(die)
         name = self.get_typename_from_die(die)
         encoding = self.DwarfEncoding(cast(int, die.attributes['DW_AT_encoding'].value))
         bytesize = cast(int, die.attributes['DW_AT_byte_size'].value)
         basetype = self.get_core_base_type(encoding, bytesize)
+        self.logger.debug(f"Registering base type: {name} as {basetype.name}")
         self.varmap.register_base_type(name, basetype)
 
         self.die2typeid_map[die] = self.varmap.get_type_id(name)
         self.die2vartype_map[die] = basetype
 
     def die_process_enum(self, die: "elftools_stubs.Die") -> None:
+        self.log_debug_process_die(die)
         name = self.get_name(die)
         if die not in self.enum_die_map:
-            self.enum_die_map[die] = VariableEnum(name)
-
-    def die_process_enum_val(self, die: "elftools_stubs.Die") -> None:
-        parent_enum = die.get_parent()
-        assert parent_enum is not None
-        if parent_enum not in self.enum_die_map:
-            raise ElfParsingError('Encountered an enumerator die with a parent not in enum map')
+            enum = VariableEnum(name)
 
-        name = self.get_name(die)
-        if 'DW_AT_const_value' in die.attributes:
-            value = cast(int, die.attributes['DW_AT_const_value'].value)
-            self.enum_die_map[parent_enum].add_value(name=name, value=value)
-        else:
-            self.logger.error('Enumerator without value')
+            for child in die.iter_children():
+                if child.tag != 'DW_TAG_enumerator':
+                    continue
+
+                name = self.get_name(child)
+                if 'DW_AT_const_value' in child.attributes:
+                    value = cast(int, child.attributes['DW_AT_const_value'].value)
+                    enum.add_value(name=name, value=value)
+                else:
+                    self.logger.error('Enumerator without value')
 
-    # Todo: the fucntions below could probably merge in one "type analyzer" function
+            self.enum_die_map[die] = enum
 
-    def extract_enum(self, die: "elftools_stubs.Die") -> Optional[VariableEnum]:
-        prevdie = die
-        while True:
-            refaddr = cast(int, prevdie.attributes['DW_AT_type'].value) + prevdie.cu.cu_offset
-            nextdie = prevdie.dwarfinfo.get_DIE_from_refaddr(refaddr)
-            if nextdie.tag == 'DW_TAG_base_type':
-                return None
-            elif nextdie.tag == 'DW_TAG_enumeration_type':
-                self.die_process_enum(nextdie)
-                return self.enum_die_map[nextdie]
-            else:
-                prevdie = nextdie
 
     def extract_basetype_die(self, die: "elftools_stubs.Die") -> "elftools_stubs.Die":
+        self.log_debug_process_die(die)
+        basetype_die = self.get_first_parent_of_type(die, 'DW_TAG_base_type')
+        if basetype_die is None:
+            raise ElfParsingError("Given die does not resolve to a base type")
+        return basetype_die
+    
+    def get_first_parent_of_type(self, die: "elftools_stubs.Die", tags:Union[str, List[str]] ) -> Optional["elftools_stubs.Die"]:
+        self.log_debug_process_die(die)
+        if isinstance(tags, str):
+            tags = [tags]
         prevdie = die
         while True:
+            if 'DW_AT_type' not in prevdie.attributes:
+                return None
             refaddr = cast(int, prevdie.attributes['DW_AT_type'].value) + prevdie.cu.cu_offset
             nextdie = prevdie.dwarfinfo.get_DIE_from_refaddr(refaddr)
-            if nextdie.tag == 'DW_TAG_base_type':
+            if nextdie.tag in tags:
                 return nextdie
             else:
                 prevdie = nextdie
 
-    def is_type_struct_or_class(self, die: "elftools_stubs.Die") -> bool:
+    def get_type_of_var(self, die: "elftools_stubs.Die") -> TypeDescriptor:
+        """Go up the hiearchy to find the die that represent the type of the variable. """
+        self.log_debug_process_die(die)
         prevdie = die
+        enum:Optional["elftools_stubs.Die"] = None
         while True:
             refaddr = prevdie.attributes['DW_AT_type'].value + prevdie.cu.cu_offset
             nextdie = prevdie.dwarfinfo.get_DIE_from_refaddr(refaddr)
-
-            if nextdie.tag in ['DW_TAG_structure_type', 'DW_TAG_class_type']:
-                return True
+            if nextdie.tag =='DW_TAG_structure_type':
+                return TypeDescriptor(TypeOfVar.Struct, enum, nextdie)
+            elif nextdie.tag == 'DW_TAG_class_type':
+                return TypeDescriptor(TypeOfVar.Class, enum, nextdie)
+            elif nextdie.tag == 'DW_TAG_array_type':
+                return TypeDescriptor(TypeOfVar.Array, enum, nextdie)
             elif nextdie.tag == 'DW_TAG_base_type':
-                return False
-
-            else:
-                prevdie = nextdie
+                return TypeDescriptor(TypeOfVar.BaseType, enum, nextdie)
+            elif nextdie.tag == 'DW_TAG_pointer_type':
+                return TypeDescriptor(TypeOfVar.Pointer, enum, nextdie)
+            elif nextdie.tag == 'DW_TAG_union_type':
+                return TypeDescriptor(TypeOfVar.Union, enum, nextdie)
+            elif nextdie.tag == 'DW_TAG_enumeration_type':
+                enum = nextdie  # Should resolve to a basetype on next iteration.
 
-    def get_struct_or_class_type(self, die: "elftools_stubs.Die") -> "elftools_stubs.Die":
-        prevdie = die
-        while True:
-            refaddr = prevdie.attributes['DW_AT_type'].value + prevdie.cu.cu_offset
-            nextdie = prevdie.dwarfinfo.get_DIE_from_refaddr(refaddr)
-            if nextdie.tag in ['DW_TAG_structure_type', 'DW_TAG_class_type']:
-                return nextdie
-            elif nextdie.tag == 'DW_TAG_base_type':
-                raise ElfParsingError('Not a structure type')
-            else:
-                prevdie = nextdie
+            prevdie = nextdie
 
     # When we encounter a struct die, we make a definition that we keep global,
     # this definition includes all submember with their respective offset.
     # each time we will encounter a instance of this struct, we will generate a variable for each sub member
 
-    def die_process_struct(self, die: "elftools_stubs.Die") -> None:
+    def die_process_struct_or_class(self, die: "elftools_stubs.Die") -> None:
+        self.log_debug_process_die(die)
+
         if die not in self.struct_die_map:
             self.struct_die_map[die] = self.get_struct_or_class_def(die)
 
+
     # Go down the hierarchy to get the whole struct def in a recursive way
     def get_struct_or_class_def(self, die: "elftools_stubs.Die") -> Struct:
+        self.log_debug_process_die(die)
         if die.tag not in ['DW_TAG_structure_type', 'DW_TAG_class_type']:
             raise ValueError('DIE must be a structure or a class type')
 
         struct = Struct(self.get_name(die))
 
         for child in die.iter_children():
-            if child.tag in ['DW_TAG_structure_type', 'DW_TAG_class_type']:
-                self.die_process_struct(child)
-            elif child.tag == 'DW_TAG_member':
+            if child.tag == 'DW_TAG_member':
                 member = self.get_member_from_die(child)
                 if member is not None:
                     struct.add_member(member)
-            elif child.tag == 'DW_TAG_subprogram':
-                pass  # TODO : There's a lot of stuff underneath this.
-            else:
-                raise NotImplementedError('DIE below structure type is expected to be a member or a struct.')  # In case this happens..
+            elif child.tag == 'DW_TAG_inheritance':
+                offset = 0
+                if 'DW_AT_data_member_location' in child.attributes:
+                    offset = child.attributes['DW_AT_data_member_location'].value
+                refaddr = child.attributes['DW_AT_type'].value + child.cu.cu_offset
+                typedie = child.dwarfinfo.get_DIE_from_refaddr(refaddr)
+                if typedie.tag not in ['DW_TAG_structure_type', 'DW_TAG_class_type']:
+                    self.logger.warning(f"Line {get_linenumber()}: Inheritance to a type die {self.make_name_for_log(typedie)}. Not supported yet")
+                    continue
+                self.die_process_struct_or_class(typedie)
+                parent_struct = self.struct_die_map[typedie]
+                struct.inherit(parent_struct, offset=offset)
 
         return struct
 
     # Read a member die and generate a Struct.Member that we will later on use to register a variable.
     # The struct.Member object contains everything we need to map a
     def get_member_from_die(self, die: "elftools_stubs.Die") -> Optional[Struct.Member]:
+        self.log_debug_process_die(die)
         name = self.get_name(die)
-        if self.is_type_struct_or_class(die):
-            struct_die = self.get_struct_or_class_type(die)
-            substruct = self.get_struct_or_class_def(struct_die)  # recursion
+        type_desc = self.get_type_of_var(die)
+        enum:Optional[VariableEnum] = None
+        if type_desc.type in (TypeOfVar.Struct, TypeOfVar.Class):
+            substruct = self.get_struct_or_class_def(type_desc.type_die)  # recursion
             typename = None
-        else:
-            basetype_die = self.extract_basetype_die(die)
-            self.die_process_base_type(basetype_die)    # Just in case it is unknown yet
-            typename = self.get_typename_from_die(basetype_die)
+        elif type_desc.type == TypeOfVar.BaseType:
+            self.die_process_base_type(type_desc.type_die)    # Just in case it is unknown yet
+            if type_desc.enum_die is not None:
+                self.die_process_enum(type_desc.enum_die)
+                enum = self.enum_die_map[type_desc.enum_die]
+            typename = self.get_typename_from_die(type_desc.type_die)
             substruct = None
+        else:
+            self.logger.warning(f"Line {get_linenumber()}: Found a member with a type die {self.make_name_for_log(type_desc.type_die)} (type={type_desc.type.name}). Not supported yet")
+            return None
+
 
         # We are looking at a forward declared member.
         if 'DW_AT_declaration' in die.attributes and die.attributes['DW_AT_declaration'].value == True:
             return None
 
         byte_offset = die.attributes['DW_AT_data_member_location'].value
 
@@ -497,120 +575,150 @@
         return Struct.Member(
             name=name,
             is_substruct=True if substruct is not None else False,
             original_type_name=typename,
             byte_offset=byte_offset,
             bitoffset=bitoffset,
             bitsize=bitsize,
-            substruct=substruct
+            substruct=substruct,
+            enum=enum
+            
         )
 
     # We have an instance of a struct. Use the location and go down the structure recursively
     # using the members offsets to find the final address that we will apply to the output var
-    def register_struct_var(self, die: "elftools_stubs.Die", location: VariableLocation) -> None:
+    def register_struct_var(self, die: "elftools_stubs.Die", type_die:"elftools_stubs.Die", location: VariableLocation) -> None:
         path_segments = self.make_varpath(die)
         path_segments.append(self.get_name(die))
-        struct_die = self.get_struct_or_class_type(die)
-        struct = self.struct_die_map[struct_die]
+        struct = self.struct_die_map[type_die]
         startpoint = Struct.Member(struct.name, is_substruct=True, bitoffset=None, bitsize=None, substruct=struct)
 
         # Start the recursion
         self.register_member_as_var_recursive(path_segments, startpoint, location, offset=0)
 
     # Recursive function to dig into a structure and register all possible variables.
-    def register_member_as_var_recursive(self, path_segments: List[str], member: Struct.Member, location: VariableLocation, offset: int) -> None:
+    def register_member_as_var_recursive(self, path_segments: List[str], member: Struct.Member, base_location: VariableLocation, offset: int) -> None:
         if member.is_substruct:
             assert member.substruct is not None
             struct = member.substruct
             for name, submember in struct.members.items():
                 new_path_segments = path_segments.copy()
+                location = base_location.copy()
                 if submember.is_substruct:
                     assert submember.byte_offset is not None
                     new_path_segments.append(name)
-                    location = location.copy()  # When we go ina substruct, the member byte_offset is reset to 0
                     location.add_offset(submember.byte_offset)
 
                 elif submember.byte_offset is not None:
                     offset = submember.byte_offset
 
                 self.register_member_as_var_recursive(new_path_segments, submember, location, offset)
         else:
-            location = location.copy()
+            location = base_location.copy()
             assert member.byte_offset is not None
             assert member.original_type_name is not None
             location.add_offset(member.byte_offset)
 
+            if self.logger.isEnabledFor(logging.DEBUG):
+                fullpath = '/'.join(path_segments + [member.name])
+                self.logger.debug(f"Registering {fullpath}")
             self.varmap.add_variable(
                 path_segments=path_segments,
                 name=member.name,
                 original_type_name=member.original_type_name,
                 location=location,
                 bitoffset=member.bitoffset,
                 bitsize=member.bitsize,
-                # enum                = member.enum # TODO
+                enum = member.enum
             )
 
-            # context.varmap.append(varentry)
-
-    # Try to extract a location from a die.
-
+    def register_variable(self, 
+                          name:str, 
+                          path_segments:List[str], 
+                          location:VariableLocation, 
+                          original_type_name:str, 
+                          enum:Optional[VariableEnum] 
+                          ) -> None:
+        """Adds a variable to the varmap.
+        
+            :param name: Name of the variable
+            :param path_segments: List of str representing each level of display tree
+            :param location: The address of the variable
+            :param original_type_name: The name of the underlying type. Must be a name coming from the binary. Will resolve to an EmbeddedDataType
+            :param enum: Optional enum to associate with the type
+        """
+        if self.logger.isEnabledFor(logging.DEBUG):
+            fullpath = '/'.join(path_segments + [name])
+            self.logger.debug(f"Registering {fullpath}")
+        self.varmap.add_variable(
+            path_segments=path_segments,
+            name=name,
+            location=location,
+            original_type_name=original_type_name,
+            enum=enum
+        )
+    
     def get_location(self, die: "elftools_stubs.Die") -> Optional[VariableLocation]:
+        """Try t extract the location from a die. Returns ``None`` if not available"""
         if 'DW_AT_location' in die.attributes:
             dieloc = (die.attributes['DW_AT_location'].value)
 
             if not isinstance(dieloc, list):
-                self.logger.warning('die location is not a list')
                 return None
 
             if len(dieloc) < 1:
-                self.logger.warning('die location is too small')
                 return None
 
             if dieloc[0] != self.DW_OP_ADDR:
-                self.logger.warning('die location must be an absolute address')
                 return None
 
             if len(dieloc) < 2:
-                self.logger.warning('die location is too small')
+                self.logger.warning(f'die location is too small: {dieloc}')
                 return None
 
             return VariableLocation.from_bytes(dieloc[1:], self.endianness)
         return None
 
-    # Process a variable die.
-    # Register a variable from it.
     def die_process_variable(self, die: "elftools_stubs.Die", location: Optional[VariableLocation] = None) -> None:
+        """Process a variable die and insert a variable in the varmap object if it has an absolute address"""
         if location is None:
             location = self.get_location(die)
 
         if 'DW_AT_specification' in die.attributes:
             vardie = self.get_die_at_spec(die)
-            self.die_process_variable(vardie, location)
+            self.die_process_variable(vardie, location) # Recursion
 
         else:
             if location is not None:
-                if self.is_type_struct_or_class(die):
-                    struct_die = self.get_struct_or_class_type(die)
-                    self.die_process_struct(struct_die)
-                    self.register_struct_var(die, location)
-                else:
+                type_desc = self.get_type_of_var(die)
+
+                if type_desc.type in (TypeOfVar.Struct, TypeOfVar.Class):   # TODO: Union
+                    self.die_process_struct_or_class(type_desc.type_die)
+                    self.register_struct_var(die, type_desc.type_die, location)
+                elif type_desc.type == TypeOfVar.BaseType:
                     path_segments = self.make_varpath(die)
                     name = self.get_name(die)
-                    basetype_die = self.extract_basetype_die(die)
-                    enum_obj = self.extract_enum(die)
-                    self.die_process_base_type(basetype_die)
-                    self.varmap.add_variable(
-                        path_segments=path_segments,
+                    self.die_process_base_type(type_desc.type_die)
+                    enum:Optional[VariableEnum] = None
+                    if type_desc.enum_die is not None:
+                        self.die_process_enum(type_desc.enum_die)
+                        enum = self.enum_die_map[type_desc.enum_die]
+                   
+                    self.register_variable(
                         name=name,
+                        path_segments=path_segments,
                         location=location,
-                        original_type_name=self.get_typename_from_die(basetype_die),
-                        enum=enum_obj
+                        original_type_name=self.get_typename_from_die(type_desc.type_die),
+                        enum=enum
                     )
+                else:
+                    self.logger.warning(f"Line {get_linenumber()}: Found a variable with a type die {self.make_name_for_log(type_desc.type_die)} (type={type_desc.type.name}). Not supported yet")
 
     def get_varpath_from_hierarchy(self, die: "elftools_stubs.Die") -> List[str]:
+        """Go up in the DWARF hierarchy and make a path segment for each level"""
         segments: List[str] = []
         parent = die.get_parent()
         while parent is not None:
             if parent.tag == 'DW_TAG_compile_unit':
                 break
 
             try:
@@ -625,26 +733,28 @@
 
             if name is not None:
                 segments.insert(0, name)
             parent = parent.get_parent()
         return segments
 
     def get_varpath_from_linkage_name(self, die: "elftools_stubs.Die") -> List[str]:
+        """Generate path segments by parsing the linkage name. Relies on the ability to demangle"""
         mangled = die.attributes['DW_AT_linkage_name'].value.decode('ascii')
         demangled = self.demangler.demangle(mangled)
         segments = demangled.split('::')
         try:
             name = self.get_name(die)
             if segments[-1] == name:
                 segments.pop()
         except Exception:
             pass
         return segments
 
     def make_varpath(self, die: "elftools_stubs.Die") -> List[str]:
+        """Generate the display path for a die, either from the hierarchy or the linkage name"""
         if 'DW_AT_linkage_name' in die.attributes:
             segments = self.get_varpath_from_linkage_name(die)
         else:
             segments = self.get_varpath_from_hierarchy(die)
 
         if self.is_external(die):
             segments.insert(0, self.GLOBAL)
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/bintools/elftools_stubs.pyi` & `scrutinydebugger-0.2.0/scrutiny/core/bintools/elftools_stubs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 class Die:
     tag: str
     cu: "CompileUnit"
     attributes: Dict[str, Attribute]
     dwarfinfo: DwarfInfo
+    offset:int
 
     def iter_children(self) -> Iterable["Die"]: pass
     def get_parent(self) -> Optional["Die"]: pass
 
 
 class CompileUnit:
     cu_offset: int
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/bintools/get_var_memrange.py` & `scrutinydebugger-0.2.0/scrutiny/core/bintools/get_var_memrange.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/codecs.py` & `scrutinydebugger-0.2.0/scrutiny/core/codecs.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/datalogging.py` & `scrutinydebugger-0.2.0/scrutiny/core/datalogging.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     'DataSeriesWithAxis',
     'DataloggingAcquisition'
 ]
 
 
 @dataclass(frozen=True)
 class AxisDefinition:
-    """Represent an axis"""
+    """(Immutable struct) Represent an axis"""
+
     name: str
     """The name of the axis. Used for display"""
     axis_id: int
     """A unique ID used to identify the axis"""
 
 
 class DataSeries:
@@ -74,14 +75,16 @@
 
     def __len__(self) -> int:
         return len(self.data)
 
 
 @dataclass(frozen=True)
 class DataSeriesWithAxis:
+    """(Immutable struct) Dataseries tied to an axis definition"""
+
     series: DataSeries
     """The dataseries containing the acquisition data"""
 
     axis: AxisDefinition
     """The Y-Axis to which the dataseries is bound to"""
 
 
@@ -200,14 +203,14 @@
         for i in range(len(self.xdata.data)):
             trigger_val = []
             if self.trigger_index is not None:
                 trigger_val = [0 if i < self.trigger_index else 1]
             writer.writerow([self.xdata.data[i]] + [ydata.series.data[i] for ydata in self.ydata] + trigger_val)
 
     def to_csv(self, filename: str) -> None:
-        """Export a DataloggingAcquisition content to a csv file
+        """Export a :class:`DataloggingAcquisition<scrutiny.core.datalogging.DataloggingAcquisition>` content to a csv file
 
         :param filename: The file to write to
         """
         with open(filename, 'w', encoding='utf8', newline='') as f:
             writer = csv.writer(f, delimiter=',', quotechar='"', quoting=csv.QUOTE_MINIMAL)
             self.write_csv(writer)
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/firmware_description.py` & `scrutinydebugger-0.2.0/scrutiny/core/firmware_description.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/firmware_parser.py` & `scrutinydebugger-0.2.0/scrutiny/core/firmware_parser.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/memory_content.py` & `scrutinydebugger-0.2.0/scrutiny/core/memory_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         if size < 0:
             raise ValueError('Cannot read a negative size')
 
         if offset < 0:
             raise IndexError('Offset cannot be negative %d' % offset)
 
         if offset + size > self.size:
-            raise IndexError('Index out of range %d to %d' % (offset, offset + size))
+            raise IndexError('Index out of range 0x%x to 0x%x' % (offset, offset + size))
 
         if self.has_data:
             assert self.internal_data is not None
             data_out = data_out = self.internal_data[offset:offset + size]
             if isinstance(data_out, int):
                 data_out = bytearray([data_out])
         else:
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/sfd_storage.py` & `scrutinydebugger-0.2.0/scrutiny/core/sfd_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,30 +48,31 @@
             raise ValueError('Firmware ID must be a string')
 
         return firmwareid.lower().strip()
 
     def __init__(self, folder: str) -> None:
         self.folder = folder
         self.temporary_dir = None
-        os.makedirs(self.folder, exist_ok=True)
-
+    
     def use_temp_folder(self) -> TempStorageWithAutoRestore:
         """Require the storage manager to switch to a temporary directory. Used for unit testing"""
         self.temporary_dir = tempfile.TemporaryDirectory()
         return TempStorageWithAutoRestore(self)
 
     def restore_storage(self) -> None:
         """Require the storage manager to work on the real directory and not a temporary directory"""
         self.temporary_dir = None
 
-    def get_storage_dir(self) -> str:
+    def get_storage_dir(self, create:bool=False) -> str:
         """Ge the actual storage directory"""
         if self.temporary_dir is not None:
             return self.temporary_dir.name
 
+        if create:
+            os.makedirs(self.folder, exist_ok=True)
         return self.folder
 
     def install(self, filename: str, ignore_exist: bool = False) -> FirmwareDescription:
         """Install a Scrutiny Firmware Description file (SFD) from a filename into the global storage. 
         Once installed, it can be loaded when communication starts with a device that identify
         itself with an ID that matches this SFD"""
         if not os.path.isfile(filename):
@@ -82,28 +83,28 @@
         return sfd
 
     def install_sfd(self, sfd: FirmwareDescription, ignore_exist: bool = False) -> None:
         """Install a Scrutiny Firmware Description (SFD) object into the global storage. 
         Once isntalled, it can be loaded when communication starts with a device that identify
         itself with an ID that matches this SFD"""
         firmware_id_ascii = self.clean_firmware_id(sfd.get_firmware_id_ascii())
-        output_file = os.path.join(self.get_storage_dir(), firmware_id_ascii)
+        output_file = os.path.join(self.get_storage_dir(create=True), firmware_id_ascii)
 
         if os.path.isfile(output_file) and ignore_exist == False:
             logging.warning('A Scrutiny Firmware Description file with the same firmware ID was already installed. Overwriting.')
 
         sfd.write(output_file)  # Write the Firmware Description file in storage folder with firmware ID as name
 
     def uninstall(self, firmwareid: str, ignore_not_exist: bool = False) -> None:
         """Remove a Scrutiny Firmware Description (SFD) with given ID from the global storage"""
         firmwareid = self.clean_firmware_id(firmwareid)
         if not self.is_valid_firmware_id(firmwareid):
             raise ValueError('Invalid firmware ID')
 
-        target_file = os.path.join(self.get_storage_dir(), firmwareid)
+        target_file = os.path.join(self.get_storage_dir(create=True), firmwareid)
 
         if os.path.isfile(target_file):
             os.remove(target_file)
         else:
             if not ignore_not_exist:
                 raise ValueError('SFD file with firmware ID %s not found' % (firmwareid))
 
@@ -136,17 +137,18 @@
         firmwareid = self.clean_firmware_id(firmwareid)
         filename = os.path.join(storage, firmwareid)
         return FirmwareDescription.read_metadata_from_sfd_file(filename)
 
     def list(self) -> List[str]:
         """Returns a list of firmware ID installed in the global storage"""
         thelist = []
-        for filename in os.listdir(self.get_storage_dir()):   # file name is firmware ID
-            if os.path.isfile(os.path.join(self.get_storage_dir(), filename)) and self.is_valid_firmware_id(filename):
-                thelist.append(filename)
+        if os.path.isdir(self.get_storage_dir()):
+            for filename in os.listdir(self.get_storage_dir()):   # file name is firmware ID
+                if os.path.isfile(os.path.join(self.get_storage_dir(), filename)) and self.is_valid_firmware_id(filename):
+                    thelist.append(filename)
         return thelist
 
     @classmethod
     def is_valid_firmware_id(cls, firmware_id: str) -> bool:
         """Returns True if the given string respect the expected format for a firmware ID"""
         retval = False
         try:
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/typehints.py` & `scrutinydebugger-0.2.0/scrutiny/core/typehints.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/validation.py` & `scrutinydebugger-0.2.0/scrutiny/core/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,7 +68,13 @@
     return val
 
 
 def assert_float_range_if_not_none(val: Optional[float], name: str, minval: Optional[float] = None, maxval: Optional[float] = None) -> Optional[float]:
     if val is None:
         return None
     return assert_float_range(val, name, minval, maxval)
+
+def assert_is_iterable(val:Any, name:str) -> None:
+    try:
+        iter(val)
+    except TypeError:
+        raise ValueError(f"{name} is not iterable. Got type: {val.__class__.__name__}")
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/variable.py` & `scrutinydebugger-0.2.0/scrutiny/core/variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     'Variable'
 ]
 
 import struct
 from scrutiny.core.basic_types import Endianness, EmbeddedDataType
 from scrutiny.core.codecs import Codecs, Encodable, UIntCodec
 from typing import Dict, Union, List, Literal, Optional, TypedDict, Any, Tuple
-
+from copy import deepcopy
 
 MASK_MAP: Dict[int, int] = {}
 for i in range(64):
     v = 0
     for j in range(i):
         v |= (1 << j)
         MASK_MAP[i] = v
@@ -149,22 +149,24 @@
         name: str
         is_substruct: bool
         original_type_name: Optional[str]
         bitoffset: Optional[int]
         byte_offset: Optional[int]
         bitsize: Optional[int]
         substruct: Optional['Struct']
+        enum:Optional['VariableEnum']
 
         def __init__(self, name: str,
                      is_substruct: bool = False,
                      original_type_name: Optional[str] = None,
                      byte_offset: Optional[int] = None,
                      bitoffset: Optional[int] = None,
                      bitsize: Optional[int] = None,
-                     substruct: Optional['Struct'] = None
+                     substruct: Optional['Struct'] = None,
+                     enum:Optional['VariableEnum'] = None
                      ):
 
             if not is_substruct:
                 if original_type_name is None:
                     raise ValueError('A typename must be given for non-struct member')
 
             if bitoffset is not None:
@@ -192,14 +194,15 @@
             self.name = name
             self.is_substruct = is_substruct
             self.original_type_name = original_type_name
             self.bitoffset = bitoffset
             self.byte_offset = byte_offset
             self.bitsize = bitsize
             self.substruct = substruct
+            self.enum = enum
 
     name: str
     members: Dict[str, "Struct.Member"]
 
     def __init__(self, name: str) -> None:
         self.name = name
         self.members = {}
@@ -209,14 +212,22 @@
         if member.name in self.members:
             raise KeyError('Duplicate member %s' % member.name)
 
         if not isinstance(member, Struct.Member):
             raise ValueError('Node must be a Struct.Member')
 
         self.members[member.name] = member
+    
+    def inherit(self, other:"Struct", offset:int=0) -> None:
+        for member in other.members.values():
+            member2 = deepcopy(member)
+            if member2.byte_offset is None:
+                raise RuntimeError("Expect byte_offset to be set to handle inheritance")
+            member2.byte_offset += offset
+            self.add_member(member)
 
 
 class Variable:
     """
     One of the most basic type of data (with RPV and Alias).
     Represent a variable in memory. It has a name, location and type.
     It supports bitfields and variable endianness.
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/core/varmap.py` & `scrutinydebugger-0.2.0/scrutiny/core/varmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,33 +112,33 @@
         if endianness not in [Endianness.Little, Endianness.Big]:
             raise ValueError('Invalid endianness %s' % endianness)
         self.endianness = endianness
 
     def get_endianness(self) -> Endianness:
         return self.endianness
 
-    def write(self, filename: str) -> None:
+    def write(self, filename: str, indent:int=4) -> None:
         with open(filename, 'w') as f:
-            f.write(self.get_json())
+            f.write(self.get_json(indent))
 
-    def get_json(self) -> str:
+    def get_json(self, indent:int=4) -> str:
         if self.endianness == Endianness.Little:
             endianness_str = 'little'
         elif self.endianness == Endianness.Big:
             endianness_str = 'big'
         else:
             raise Exception('Unknown endianness')
 
         content = {
             'endianness': endianness_str,
             'type_map': self.typemap,
             'variables': self.variables,
             'enums': self.enums,
         }
-        return json.dumps(content, indent=4)
+        return json.dumps(content, indent=indent)
 
     def validate(self) -> None:
         pass
 
     def validate_json(self, content: Dict[str, Any]) -> None:
         required_fields = {
             'endianness',
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/sdk/_api_parser.py` & `scrutinydebugger-0.2.0/scrutiny/sdk/_api_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -713,30 +713,35 @@
         _check_response_dict(cmd, sig, 'axis_id', int)
         _check_response_dict(cmd, sig, 'logged_element', str)
         _check_response_dict(cmd, sig, 'name', str)
         _check_response_dict(cmd, sig, 'data', list)
 
         yaxis_data: Optional[List[float]] = None
         try:
-            yaxis_data = [float(x) for x in sig['data']]
+            yaxis_data = [float(x) for x in sig['data']]    # Convert to float for inf or nan
         except Exception:
             raise sdk.exceptions.BadResponseError(f'Dataseries {sig["name"]} data is not all numerical')
         assert yaxis_data is not None
 
         if sig['axis_id'] not in axis_map:
             raise sdk.exceptions.BadResponseError(f'Dataseries {sig["name"]} refer to a non-existent Y-Axis')
         ds = sdk.datalogging.DataSeries(
             data=yaxis_data,
             name=sig['name'],
             logged_element=sig['logged_element']
         )
         acquisition.add_data(ds, axis=axis_map[sig['axis_id']])
 
+    try:
+        xaxis_data = [ float(f) for f in response['xdata']['data'] ]    # Convert to float for inf or nan
+    except Exception:
+        raise sdk.exceptions.BadResponseError(f'X-Axis Dataseries data is not all numerical')
+
     xdata = sdk.datalogging.DataSeries(
-        data=response['xdata']['data'],
+        data=xaxis_data,
         name=response['xdata']['name'],
         logged_element=response['xdata']['logged_element']
     )
 
     acquisition.set_xdata(xdata)
     try:
         acquisition.set_trigger_index(response['trigger_index'])
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/sdk/client.py` & `scrutinydebugger-0.2.0/scrutiny/sdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import scrutiny.sdk
 import scrutiny.sdk.datalogging
 from scrutiny.core import validation
 sdk = scrutiny.sdk
 from scrutiny.sdk import _api_parser as api_parser
 from scrutiny.sdk.definitions import *
 from scrutiny.sdk.watchable_handle import WatchableHandle
+from scrutiny.sdk import listeners
 from scrutiny.core.basic_types import *
 from scrutiny.tools.timer import Timer
 from scrutiny.sdk.write_request import WriteRequest
 from scrutiny.server.api import typing as api_typing
 from scrutiny.server.api import API
 
 import logging
@@ -213,14 +214,16 @@
     _watchable_path_to_id_map: Dict[str, str]   # A dict that maps the watchables from display path to their server id
     _server_info: Optional[ServerInfo]  # The actual server internal state given by inform_server_status
 
     _active_batch_context: Optional[BatchWriteContext]  # The active write batch. All writes are appended to it if not None
     _last_device_session_id: Optional[str]  # The last device session ID observed. Used to detect disconnection/reconnection
     _last_sfd_firmware_id: Optional[str]    # The last loaded SFD seen. Used to detect change in SFD
 
+    _listeners:List[listeners.BaseListener]   # List of registered listeners
+
     def __enter__(self) -> "ScrutinyClient":
         return self
 
     def __exit__(self, exc_type: Optional[Type[BaseException]], exc_val: Optional[BaseException], exc_tb: Optional[types.TracebackType]) -> Literal[False]:
         self.disconnect()
         return False
 
@@ -269,14 +272,15 @@
         self._watchable_storage = {}
         self._watchable_path_to_id_map = {}
         self._callback_storage = {}
         self._last_device_session_id = None
         self._last_sfd_firmware_id = None
 
         self._active_batch_context = None
+        self._listeners=[]
 
     def _start_worker_thread(self) -> None:
         self._threading_events.stop_worker_thread.clear()
         self._threading_events.disconnect.clear()
         started_event = threading.Event()
         self._worker_thread = threading.Thread(target=self._worker_thread_task, args=[started_event], daemon=True)
         self._worker_thread.start()
@@ -345,27 +349,32 @@
         with self._main_lock:
             self._server_info = info
             self._threading_events.server_status_updated.set()
 
     def _wt_process_msg_watchable_update(self, msg: api_typing.S2C.WatchableUpdate, reqid: Optional[int]) -> None:
         updates = api_parser.parse_watchable_update(msg)
 
+        updated_watchables:List[WatchableHandle] = []
         for update in updates:
             with self._main_lock:
                 watchable: Optional[WatchableHandle] = None
                 if update.server_id in self._watchable_storage:
                     watchable = self._watchable_storage[update.server_id]
 
             if watchable is None:
                 self._logger.error(f"Got watchable update for unknown watchable {update.server_id}")
                 continue
             else:
                 self._logger.debug(f"Updating value of {update.server_id} ({watchable.name})")
 
             watchable._update_value(update.value)
+            updated_watchables.append(watchable)
+        
+        for listener in self._listeners:
+            listener._broadcast_update(updated_watchables)
 
     def _wt_process_msg_inform_write_completion(self, msg: api_typing.S2C.WriteCompletion, reqid: Optional[int]) -> None:
         completion = api_parser.parse_write_completion(msg)
 
         if completion.request_token not in self._pending_api_batch_writes:
             return   # Maybe triggered by another client. Silently ignore.
 
@@ -837,15 +846,15 @@
             if incomplete_count > 0:
                 raise sdk.exceptions.TimeoutException(
                     f"Incomplete batch write. {incomplete_count} write requests not completed in {batch.timeout} sec. ")
 
     # === User API ====
 
     def connect(self, hostname: str, port: int, wait_status: bool = True, **kwargs: Dict[str, Any]) -> "ScrutinyClient":
-        """Connect to a Scrutiny server through a websocket. Extra kwargs are passed down to `websockets.sync.client.connect()`
+        """Connect to a Scrutiny server through a websocket. Extra kwargs are passed down to ``websockets.sync.client.connect()``
 
         :param hostname: The hostname or ip address of the server
         :param port: The listening port of the server
         :param wait_status: Wait for a server status update after the websocket connection is established. Ensure that a value is available when calling :meth:`get_server_status()<get_server_status>`
 
         :raise ConnectionError: In case of failure
         """
@@ -1557,14 +1566,22 @@
             if not self._server_state == ServerState.Connected:
                 raise sdk.exceptions.ConnectionError(f"Disconnected from server")
             info = self._server_info
         if info is None:
             raise sdk.exceptions.InvalidValueError("Server status is not available")
         return info
 
+    def register_listener(self, listener:listeners.BaseListener) -> None:
+        """Register a new listener. The client will notify it each time a new value update is received from the server
+        
+        :param listener: The listener to register
+        """
+        with self._main_lock:
+            self._listeners.append(listener)
+
     @property
     def name(self) -> str:
         return '' if self._name is None else self.name
 
     @property
     def server_state(self) -> ServerState:
         """The server communication state"""
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/sdk/datalogging.py` & `scrutinydebugger-0.2.0/scrutiny/sdk/datalogging.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,17 +217,18 @@
         self._next_axis_id = 0
         self._trigger_operands = []
         self._signals = []
         self._axes = {}
 
     def add_axis(self, name: str) -> AxisDefinition:
         """Adds a Y axis to the acquisition.
+        
         :param name: The name of the axis, for display purpose. 
 
-        :return: An `AxisDefinition` object that can be assigned to a signal when calling :meth:`add_signal()<scrutiny.sdk.datalogging.DataloggingConfig.add_signal>`
+        :return: An :class:`AxisDefinition<scrutiny.sdk.datalogging.AxisDefinition>` object that can be assigned to a signal when calling :meth:`add_signal()<scrutiny.sdk.datalogging.DataloggingConfig.add_signal>`
         """
         validation.assert_type(name, 'name', str)
         axis = AxisDefinition(axis_id=self._next_axis_id, name=name)
         self._next_axis_id += 1
         self._axes[axis.axis_id] = axis
         return axis
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/sdk/definitions.py` & `scrutinydebugger-0.2.0/scrutiny/sdk/definitions.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/sdk/exceptions.py` & `scrutinydebugger-0.2.0/scrutiny/sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/sdk/watchable_handle.py` & `scrutinydebugger-0.2.0/scrutiny/sdk/watchable_handle.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/sdk/write_request.py` & `scrutinydebugger-0.2.0/scrutiny/sdk/write_request.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/active_sfd_handler.py` & `scrutinydebugger-0.2.0/scrutiny/server/active_sfd_handler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/api/API.py` & `scrutinydebugger-0.2.0/scrutiny/server/api/API.py`

 * *Files 0% similar despite different names*

```diff
@@ -1499,15 +1499,15 @@
         if err:
             raise InvalidRequestException(req, "Failed to read acquisition. %s" % (str(err)))
 
         def dataseries_to_api_signal_data(ds: core_datalogging.DataSeries) -> api_typing.DataloggingSignalData:
             signal: api_typing.DataloggingSignalData = {
                 'name': ds.name,
                 'logged_element': ds.logged_element,
-                'data': ds.get_data()
+                'data': [f if math.isfinite(f) else str(f) for f in ds.get_data()]
             }
             return signal
 
         def dataseries_to_api_signal_data_with_axis(ds: core_datalogging.DataSeries, axis_id: int) -> api_typing.DataloggingSignalDataWithAxis:
             signal: api_typing.DataloggingSignalDataWithAxis = cast(api_typing.DataloggingSignalDataWithAxis, dataseries_to_api_signal_data(ds))
             signal['axis_id'] = axis_id
             return signal
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/api/abstract_client_handler.py` & `scrutinydebugger-0.2.0/scrutiny/server/api/abstract_client_handler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/api/dummy_client_handler.py` & `scrutinydebugger-0.2.0/scrutiny/server/api/dummy_client_handler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/api/typing.py` & `scrutinydebugger-0.2.0/scrutiny/server/api/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     timestamp: float
     firmware_id: str
     firmware_metadata: Optional[SFDMetadata]
 
 
 class DataloggingSignalData(TypedDict):
     name: str
-    data: List[float]
+    data: List[Union[float,str]]
     logged_element: str
 
 
 class DataloggingSignalDataWithAxis(DataloggingSignalData):
     axis_id: int
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/api/value_streamer.py` & `scrutinydebugger-0.2.0/scrutiny/server/api/value_streamer.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/api/websocket_client_handler.py` & `scrutinydebugger-0.2.0/scrutiny/server/api/websocket_client_handler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/datalogging/datalogging_manager.py` & `scrutinydebugger-0.2.0/scrutiny/server/datalogging/datalogging_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -200,16 +200,16 @@
                 else:
                     raise ValueError('Impossible X-Axis type')
 
                 if len(xaxis) != nb_points:
                     raise ValueError("Failed to find a matching xaxis dataseries")
 
                 acquisition.set_xdata(xaxis)
-                # -1 because index is 0 based.   -1 because we have the number of points AFTER the trigger, excluding the trigger.  So total of -2
-                trigger_index = max(0, min(metadata.number_of_points - metadata.points_after_trigger, metadata.number_of_points - 2))
+                # -1 because we are 0 based. min(a,b)-1 = min(a-1, b-1)
+                trigger_index = max(0, min(metadata.number_of_points - metadata.points_after_trigger, metadata.number_of_points) - 1 )
                 acquisition.set_trigger_index(trigger_index)
                 DataloggingStorage.save(acquisition)
             else:
                 # acquisition will be None here
                 self.logger.info("Failed to acquire acquisition. " + str(detail_msg))
         except Exception as e:
             acquisition = None  # Checked later to call the callback
@@ -353,24 +353,39 @@
 
         self.previous_state = self.state
         self.state = next_state
 
     @classmethod
     def api_trigger_condition_to_device_trigger_condition(cls, api_cond: api_datalogging.TriggerCondition) -> device_datalogging.TriggerCondition:
         """Converts a TriggerCondition in the API format to the device format"""
+        scaling_operand:Optional[api_datalogging.TriggerConditionOperand] = None
         device_operands: List[device_datalogging.Operand] = []
+
+        for api_operand in api_cond.operands:
+            if isinstance(api_operand.value, DatastoreAliasEntry):
+                if api_operand.value.has_value_modifier():
+                    if scaling_operand is None:
+                        scaling_operand = api_operand
+            
+
         for api_operand in api_cond.operands:
             if api_operand.type == api_datalogging.TriggerConditionOperandType.LITERAL:
                 if not isinstance(api_operand.value, (int, float)):
                     raise ValueError("Literal operands must be int or float")
-                device_operands.append(device_datalogging.LiteralOperand(api_operand.value))
+                value = api_operand.value
+                if scaling_operand is not None:
+                    assert isinstance(scaling_operand.value, DatastoreAliasEntry)
+                    value = scaling_operand.value.compute_user_to_device(value, apply_saturation=False) # Scale the literal to math the alias user value.
+                device_operands.append(device_datalogging.LiteralOperand(value))
+            
             elif api_operand.type == api_datalogging.TriggerConditionOperandType.WATCHABLE:
                 if not isinstance(api_operand.value, DatastoreEntry):
                     raise ValueError("Watchable operand must have a datastore entry as value")
-
+                if scaling_operand is not None and scaling_operand is not api_operand:
+                    raise ValueError("Cannot compare an alias with a value modifier with anything else than a literal.")
                 device_operands.append(cls.make_device_operand_from_watchable(api_operand.value))
             else:
                 raise ValueError("Unsupported operand type %s" % str(api_operand.type))
 
         device_cond = device_datalogging.TriggerCondition(api_cond.condition_id, *device_operands)
 
         return device_cond
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/datalogging/datalogging_storage.py` & `scrutinydebugger-0.2.0/scrutiny/server/datalogging/datalogging_storage.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/datalogging/datalogging_utilities.py` & `scrutinydebugger-0.2.0/scrutiny/server/datalogging/datalogging_utilities.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/datalogging/definitions/api.py` & `scrutinydebugger-0.2.0/scrutiny/server/datalogging/definitions/api.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/datalogging/definitions/device.py` & `scrutinydebugger-0.2.0/scrutiny/server/datalogging/definitions/device.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/datastore/datastore.py` & `scrutinydebugger-0.2.0/scrutiny/server/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/datastore/datastore_entry.py` & `scrutinydebugger-0.2.0/scrutiny/server/datastore/datastore_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,14 +362,32 @@
         raise NotImplementedError('Cannot set value on a Alias variable')
 
     def set_value_internal(self, value: Union[int, float, bool]) -> None:
         """Set the value of this alias object."""
         # These function are meant to be used internally to make the alias mechanism work. Not to be used by a user.
         new_value = self.aliasdef.compute_device_to_user(value)
         DatastoreEntry.set_value(self, new_value)
+    
+    def compute_device_to_user(self, value:Union[int, float, bool]) -> Union[int, float, bool]:
+        """Transform a value from the device side to the user side applying the alias configuration"""
+        return self.aliasdef.compute_device_to_user(value)
+    
+    def compute_user_to_device(self, value:Union[int, float, bool], apply_saturation:bool=True) -> Union[int, float, bool]:
+        """Transform a value from the user side to the device side applying the alias configuration"""
+        return self.aliasdef.compute_user_to_device(value, apply_saturation)
+    
+    def has_value_modifier(self) -> bool:
+        """Tells if the alias is configured to modify the value for the user"""
+        val = False
+        val = val or self.aliasdef.gain is not None 
+        val = val or self.aliasdef.offset is not None 
+        val = val or self.aliasdef.max is not None 
+        val = val or self.aliasdef.min is not None
+        return val
+
 
 
 class DatastoreRPVEntry(DatastoreEntry):
     """A datastore entry that represents a Runtime Published Value"""
 
     rpv: RuntimePublishedValue
     codec: BaseCodec
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/datastore/entry_type.py` & `scrutinydebugger-0.2.0/scrutiny/server/datastore/entry_type.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/device_handler.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/device_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'DeviceAcquisitionRequestCompletionCallback'
 ]
 
 import copy
 import logging
 import binascii
 import time
-from enum import Enum
+from enum import Enum, auto
 import traceback
 from uuid import uuid4
 import math
 from scrutiny.server.datastore.datastore_entry import DatastoreRPVEntry, EntryType
 import scrutiny.server.datalogging.definitions.device as device_datalogging
 from scrutiny.server.protocol import *
 import scrutiny.server.protocol.typing as protocol_typing
@@ -179,23 +179,23 @@
         DISCONNECTED = 0
         CONNECTING = 1
         CONNECTED_NOT_READY = 2
         CONNECTED_READY = 3
 
     class FsmState(Enum):
         """The Device Handler State Machine states"""
-        INIT = 0
-        WAIT_COMM_LINK = 1
-        WAIT_CLEAN_STATE = 2
-        DISCOVERING = 3
-        CONNECTING = 4
-        POLLING_INFO = 5
-        WAIT_DATALOGGING_READY = 6
-        READY = 7
-        DISCONNECTING = 8
+        INIT = auto()
+        WAIT_COMM_LINK = auto()
+        WAIT_CLEAN_STATE = auto()
+        DISCOVERING = auto()
+        CONNECTING = auto()
+        POLLING_INFO = auto()
+        WAIT_DATALOGGING_READY = auto()
+        READY = auto()
+        DISCONNECTING = auto()
 
     class OperatingMode(Enum):
         """Tells the main function of the device handler. Modes different from Normal are meant for unit tests"""
         Normal = 0
         Test_CheckThrottling = 1
 
     def __init__(self, config: DeviceHandlerConfig, datastore: Datastore):
@@ -232,15 +232,15 @@
         self.comm_handler = CommHandler(cast(Dict[str, Any], self.config))
         self.comm_handler_open_restart_timer = Timer(1.0)
 
         self.heartbeat_generator.set_interval(max(0.5, self.config['heartbeat_timeout'] * 0.75))
         self.comm_broken = False
         self.device_id = None
         self.operating_mode = self.OperatingMode.Normal
-        self.wait_clean_state_timestamp = time.time()
+        self.wait_clean_state_timestamp = time.monotonic()
         self.active_request_record = None
         self.device_state_changed_callbacks = []
         self.expect_no_timeout = False  # Unit tests will set this to True
 
         if 'link_type' in self.config and 'link_config' in self.config:
             self.configure_comm(self.config['link_type'], self.config['link_config'])
 
@@ -595,34 +595,34 @@
         state_entry: bool = True if self.fsm_state != self.last_fsm_state else False
         next_state: "DeviceHandler.FsmState" = self.fsm_state
         if self.fsm_state == self.FsmState.INIT:
             self.reset_comm()
             next_state = self.FsmState.WAIT_COMM_LINK
 
         elif self.fsm_state == self.FsmState.WAIT_COMM_LINK:
-            if self.comm_handler.is_open():
+            if self.comm_handler.is_operational():
                 next_state = self.FsmState.WAIT_CLEAN_STATE
 
         elif self.fsm_state == self.FsmState.WAIT_CLEAN_STATE:
             if state_entry:
-                self.wait_clean_state_timestamp = time.time()
+                self.wait_clean_state_timestamp = time.monotonic()
 
             fully_stopped = True
             fully_stopped = fully_stopped and self.device_searcher.fully_stopped()
             fully_stopped = fully_stopped and self.heartbeat_generator.fully_stopped()
             fully_stopped = fully_stopped and self.info_poller.fully_stopped()
             fully_stopped = fully_stopped and self.datalogging_poller.fully_stopped()
             fully_stopped = fully_stopped and self.session_initializer.fully_stopped()
             fully_stopped = fully_stopped and self.memory_reader.fully_stopped()
             fully_stopped = fully_stopped and self.memory_writer.fully_stopped()
 
             if fully_stopped:
                 next_state = self.FsmState.DISCOVERING
 
-            if time.time() - self.wait_clean_state_timestamp > self.WAIT_CLEAN_STATE_TIMEOUT:
+            if time.monotonic() - self.wait_clean_state_timestamp > self.WAIT_CLEAN_STATE_TIMEOUT:
                 if not self.device_searcher.fully_stopped():
                     self.logger.error("Device searcher is not stopping. Forcefully resetting.")
                     self.device_searcher.reset()
 
                 if not self.heartbeat_generator.fully_stopped():
                     self.logger.error("Heartbeat Generator is not stopping. Forcefully resetting.")
                     self.heartbeat_generator.reset()
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/device_info.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/device_info.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/emulated_device.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/emulated_device.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/links/abstract_link.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/links/abstract_link.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/links/dummy_link.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/links/dummy_link.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/links/serial_link.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/links/serial_link.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,36 +8,40 @@
 
 import logging
 
 from .abstract_link import AbstractLink, LinkConfig
 
 from typing import Optional, Dict, TypedDict, cast, Union
 import serial   # type: ignore
+import time
 
 
 class SerialConfig(TypedDict):
     """
     Config given the the SerialLink object.
     Can be set through the API or config file with JSON format
     """
     portname: str
     baudrate: int
     stopbits: str
     databits: int
     parity: str
+    start_delay:float
+
 
 
 class SerialLink(AbstractLink):
     """
     Communication channel to talk with a device through a serial link
     Based on pyserial module
     """
     logger: logging.Logger
     config: SerialConfig
     _initialized: bool
+    _init_timestamp:float
 
     port: Optional[serial.Serial]
 
     STR_TO_PARITY: Dict[str, str] = {
         'none': serial.PARITY_NONE,
         'even': serial.PARITY_EVEN,
         'odd': serial.PARITY_ODD,
@@ -98,50 +102,63 @@
         return cls(config)
 
     def __init__(self, config: LinkConfig):
         self.port = None
         self.validate_config(config)
         self._initialized = False
         self.logger = logging.getLogger(self.__class__.__name__)
+        self._init_timestamp = time.monotonic()
 
         self.config = cast(SerialConfig, {
             'portname': config['portname'],
             'baudrate': config['baudrate'],
-            'stopbits': config['stopbits'] if 'stopbits' in config else "1",
-            'databits': config['databits'] if 'databits' in config else 8,
-            'parity': config['parity'] if 'parity' in config else 'none',
+            'stopbits': config.get('stopbits', '1'),
+            'databits': config.get('databits', 8),
+            'parity': config.get('parity', 'none'),
+            'start_delay' : config.get('start_delay', 0)
         })
 
     def get_config(self) -> LinkConfig:
         return cast(LinkConfig, self.config)
 
     def initialize(self) -> None:
         """ Called by the device Handler when initiating communication. Should reset the channel to a working state"""
         portname = str(self.config['portname'])
         baudrate = int(self.config['baudrate'])
         stopbits = self.get_stop_bits(self.config['stopbits'])
         databits = self.get_data_bits(self.config['databits'])
         parity = self.get_parity(self.config['parity'])
 
-        self.port = serial.Serial(portname, baudrate, timeout=0, parity=parity, bytesize=databits, stopbits=stopbits, xonxoff=False)
+        self.port = serial.Serial(
+            port=portname, 
+            baudrate=baudrate, 
+            timeout=0, 
+            parity=parity, 
+            bytesize=databits, 
+            stopbits=stopbits, 
+            xonxoff=False, 
+            rtscts=True, 
+            dsrdtr=False
+            )
         self.port.reset_input_buffer()      # Clear pending data
         self.port.reset_output_buffer()     # Clear pending data
         self._initialized = True
+        self._init_timestamp = time.monotonic()
 
     def destroy(self) -> None:
         """ Put the comm channel to a resource-free non-working state"""
         if self.port is not None:
             self.port.close()
         self._initialized = False
 
     def operational(self) -> bool:
         """ Tells if this comm channel is in proper state to be functional"""
         if self.port is None:
             return False
-        return self.port.isOpen() and self._initialized
+        return self.port.isOpen() and self.initialized()
 
     def read(self) -> Optional[bytes]:
         """ Reads bytes Non-Blocking from the comm channel. None if no data available"""
         data: Optional[bytes] = None
         if self.operational():
             assert self.port is not None    # For mypy
             try:
@@ -163,15 +180,15 @@
                 self.port.flush()
             except Exception as e:
                 self.logger.debug("Cannot write data. " + str(e))
                 self.port.close()
 
     def initialized(self) -> bool:
         """ Tells if initialize() has been called"""
-        return self._initialized
+        return self._initialized and time.monotonic()-self._init_timestamp > self.config['start_delay']
 
     def process(self) -> None:
         pass
 
     @staticmethod
     def validate_config(config: LinkConfig) -> None:
         """Raises an exception if the configuration is not adequate"""
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/links/udp_link.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/links/udp_link.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/request_dispatcher.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/request_dispatcher.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/submodules/datalogging_poller.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/datalogging_poller.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/submodules/device_searcher.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/device_searcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         """Indicates that this submodule is stopped and has no pending state"""
         return self.started == False
 
     def reset(self) -> None:
         """ Restart the search from the beginning"""
         self.pending = False
         self.last_request_timestamp = None
-        self.found_device_timestamp = time.time()
+        self.found_device_timestamp = time.monotonic()
         self.started = False
         self.found_device = None
 
     def device_found(self) -> bool:
         """Tells if a device was found"""
         return self.found_device is not None
 
@@ -96,38 +96,38 @@
     def process(self) -> None:
         """To be called periodically"""
         if not self.started:
             self.reset()
             return
 
         # Timeout
-        if time.time() - self.found_device_timestamp > self.DEVICE_GONE_DELAY:
+        if time.monotonic() - self.found_device_timestamp > self.DEVICE_GONE_DELAY:
             self.found_device = None
 
         if self.pending == False:
-            if self.last_request_timestamp is None or (time.time() - self.last_request_timestamp > self.DISCOVER_INTERVAL):
+            if self.last_request_timestamp is None or (time.monotonic() - self.last_request_timestamp > self.DISCOVER_INTERVAL):
                 self.logger.debug('Registering a Discover request')
                 self.dispatcher.register_request(
                     request=self.protocol.comm_discover(),
                     success_callback=SuccessCallback(self.success_callback),
                     failure_callback=FailureCallback(self.failure_callback),
                     priority=self.priority
                 )
                 self.pending = True
-                self.last_request_timestamp = time.time()
+                self.last_request_timestamp = time.monotonic()
 
     def success_callback(self, request: Request, response: Response, params: Any = None) -> None:
         # Called by the dispatcher when a request is completed and succeeded
         self.logger.debug("Success callback. Request=%s. Response Code=%s, Params=%s" % (request, response.code, params))
 
         if self.started:
             if response.code == ResponseCode.OK:
                 try:
                     response_data = cast(protocol_typing.Response.CommControl.Discover, self.protocol.parse_response(response))
-                    self.found_device_timestamp = time.time()
+                    self.found_device_timestamp = time.monotonic()
                     self.found_device = response_data
                 except Exception as e:
                     self.logger.error('Discover request got a response with invalid data.')
                     self.logger.debug(traceback.format_exc())
                     self.found_device = None
             else:
                 self.logger.error('Discover request got Nacked. %s' % response.code)
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/submodules/heartbeat_generator.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/heartbeat_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def __init__(self, protocol: Protocol, dispatcher: RequestDispatcher, priority: int):
         self.logger = logging.getLogger(self.__class__.__name__)
         self.dispatcher = dispatcher
         self.protocol = protocol
         self.session_id = None
         self.last_heartbeat_request = None
-        self.last_heartbeat_timestamp = time.time()
+        self.last_heartbeat_timestamp = time.monotonic()
         self.challenge = 0
         self.interval = 3
         self.priority = priority
         self.reset()
 
     def set_interval(self, interval: float) -> None:
         """Set the interval of time at which to send heartbeat"""
@@ -54,15 +54,15 @@
     def set_session_id(self, session_id: int) -> None:
         """Sets the session ID to use for heartbeat request"""
         self.session_id = session_id
 
     def start(self) -> None:
         """Enable the heartbeat generator."""
         self.started = True
-        self.last_heartbeat_timestamp = time.time()
+        self.last_heartbeat_timestamp = time.monotonic()
 
     def stop(self) -> None:
         """Disable the heartbeat generator. Will stop sending request and FSM will go idle"""
         self.logger.debug('Stop requested')
         self.started = False
 
     def fully_stopped(self) -> bool:
@@ -71,50 +71,46 @@
 
     def reset(self) -> None:
         """Put the heartbeat generator in its startup state"""
         self.pending = False
         self.started = False
         self.session_id = None
 
-    def last_valid_heartbeat_timestamp(self) -> Optional[float]:
-        """Returns the timestamp of the last heartbeat that completed successfully"""
-        return self.last_heartbeat_timestamp
-
     def process(self) -> None:
         """To be called periodically"""
         if not self.started:
             self.reset()
             return
 
         # If no request is being waited and we have a session ID assigned
         if self.pending == False and self.session_id is not None:
-            if self.last_heartbeat_request is None or (time.time() - self.last_heartbeat_request > self.interval):
+            if self.last_heartbeat_request is None or (time.monotonic() - self.last_heartbeat_request > self.interval):
                 self.logger.debug('Registering a Heartbeat request')
                 self.dispatcher.register_request(
                     request=self.protocol.comm_heartbeat(session_id=self.session_id, challenge=self.challenge),
                     success_callback=SuccessCallback(self.success_callback),
                     failure_callback=FailureCallback(self.failure_callback),
                     priority=self.priority
                 )
                 self.pending = True
-                self.last_heartbeat_request = time.time()
+                self.last_heartbeat_request = time.monotonic()
 
     def success_callback(self, request: Request, response: Response, params: Any = None) -> None:
         """ Called by the dispatcher when a request is completed and succeeded"""
         self.logger.debug("Success callback. Request=%s. Response Code=%s, Params=%s" % (request, response.code, params))
 
         expected_challenge_response = self.protocol.heartbeat_expected_challenge_response(self.challenge)
         if self.started:
             if response.code == ResponseCode.OK:
                 try:
                     response_data = cast(protocol_typing.Response.CommControl.Heartbeat, self.protocol.parse_response(response))
 
                     if response_data['session_id'] == self.session_id:
                         if response_data['challenge_response'] == expected_challenge_response:  # Make sure the device is not sending a buffered response
-                            self.last_heartbeat_timestamp = time.time()  # This is the indicator that the device is alive
+                            self.last_heartbeat_timestamp = time.monotonic()  # This is the indicator that the device is alive
                         else:
                             self.logger.error('Heartbeat challenge response is not good. Got %s, expected %s' %
                                               (response_data['challenge_response'], expected_challenge_response))
                     else:
                         self.logger.error('Heartbeat session ID echo not good. Got %s, expected %s' % (response_data['session_id'], self.session_id))
                 except Exception:
                     self.logger.error('Heartbeat response data is invalid')
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/submodules/info_poller.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/info_poller.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/submodules/memory_reader.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/memory_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,15 +507,16 @@
                     response_data = cast(protocol_typing.Response.MemoryControl.Read, self.protocol.parse_response(response))
                     try:
                         temp_memory = MemoryContent()
                         for block in response_data['read_blocks']:
                             temp_memory.write(block['address'], block['data'])
 
                         for entry in self.entries_in_pending_read_var_request:
-                            raw_data = temp_memory.read(entry.get_address(), entry.get_size())
+                            block_addr = self.protocol.get_truncated_address(entry.get_address())
+                            raw_data = temp_memory.read(block_addr, entry.get_size())
                             entry.set_value_from_data(raw_data)
                             self.entries_in_pending_read_var_request = []
                     except Exception as e:
                         self.logger.critical('Error while writing datastore. %s' % str(e))
                         self.logger.debug(traceback.format_exc())
                 except Exception:
                     self.logger.error('Response for ReadMemory read request is malformed and must be discarded.')
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/submodules/memory_writer.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/memory_writer.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/device/submodules/session_initializer.py` & `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/session_initializer.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/comm_handler.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/comm_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         """Get the target bitrate for throttling. None if disabled"""
         return self.throttler.get_bitrate() if self.throttler.is_enabled() else None
 
     def reset_bitrate_monitor(self) -> None:
         """Reset data size counters"""
         self.rx_bitcount = 0
         self.tx_bitcount = 0
-        self.bitcount_time = time.time()
+        self.bitcount_time = time.perf_counter()
 
     def get_link(self) -> Optional[AbstractLink]:
         """Return the Link object used to talk with the device."""
         return self.link
 
     def get_link_type(self) -> str:
         """Return the link type as a string. This type is the same used by the server configuration"""
@@ -356,9 +356,9 @@
     def reset(self) -> None:
         """Put back the CommHandler to its startup state"""
         self.reset_rx()
         self.clear_timeout()
 
     def get_average_bitrate(self) -> float:
         """Get the measured average bitrate since last counter reset"""
-        dt = time.time() - self.bitcount_time
+        dt = time.perf_counter() - self.bitcount_time
         return float(self.rx_bitcount + self.tx_bitcount) / float(dt)
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/base_command.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/comm_control.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/comm_control.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/datalog_control.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/datalog_control.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/dummy_command.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/dummy_command.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/get_info.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/get_info.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/commands/memory_control.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/memory_control.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/crc32.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/crc32.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/exceptions.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/protocol.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
             return self.nbits
 
         def get_pack_char(self) -> str:
             return self.pack_char
 
         def get_address_mask(self) -> int:
             return self.mask
+        
 
         def encode_address(self, address: int) -> bytes:
             address &= self.get_address_mask()
             return pack('>%s' % self.get_pack_char(), address)
 
         def decode_address(self, buff: bytes) -> int:
             return cast(int, unpack('>%s' % self.get_pack_char(), buff[0:self.get_address_size_bytes()])[0])
@@ -89,14 +90,17 @@
 
     def get_address_size_bytes(self) -> int:
         return self.address_format.get_address_size_bytes()
 
     def get_address_size_bits(self) -> int:
         return self.address_format.get_address_size_bits()
 
+    def get_truncated_address(self, address:int) -> int:
+        return address & self.address_format.get_address_mask() 
+
     def set_version(self, major: int, minor: int) -> None:
         if not isinstance(major, int) or not isinstance(minor, int):
             raise ValueError('Version major and minor number must be a valid integer.')
 
         if major == 999 and minor == 123:
             pass  # Special version for unit test
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/request.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/request.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/response.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/response.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/protocol/typing.py` & `scrutinydebugger-0.2.0/scrutiny/server/protocol/typing.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/server/server.py` & `scrutinydebugger-0.2.0/scrutiny/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,30 +25,30 @@
 
 
 class ServerConfig(TypedDict, total=False):
     """The server configuration definition loadable from json"""
     name: str
     autoload_sfd: bool
     debug: bool
-    device_config: DeviceHandlerConfig
-    api_config: APIConfig
+    device: DeviceHandlerConfig
+    api: APIConfig
 
 
 DEFAULT_CONFIG: ServerConfig = {
     'name': 'Scrutiny Server (Default config)',
     'autoload_sfd': True,
     'debug': False,    # Requires ipdb. Module must be installed with [dev] extras
-    'api_config': {
+    'api': {
         'client_interface_type': 'websocket',
         'client_interface_config': {
             'host': 'localhost',
             'port': 8765
         }
     },
-    'device_config': {
+    'device': {
         'response_timeout': 1.0,
         'link_type': 'none',
         'link_config': {
         }
     }
 }
 
@@ -81,19 +81,19 @@
             elif isinstance(input_config, dict):
                 self.config.update(input_config)
 
         self.validate_config()
         self.server_name = '<Unnamed>' if 'name' not in self.config else self.config['name']
 
         self.datastore = Datastore()
-        self.device_handler = DeviceHandler(self.config['device_config'], self.datastore)
+        self.device_handler = DeviceHandler(self.config['device'], self.datastore)
         self.datalogging_manager = DataloggingManager(self.datastore, self.device_handler)
         self.sfd_handler = ActiveSFDHandler(device_handler=self.device_handler, datastore=self.datastore, autoload=self.config['autoload_sfd'])
         self.api = API(
-            self.config['api_config'],
+            self.config['api'],
             datastore=self.datastore,
             device_handler=self.device_handler,
             sfd_handler=self.sfd_handler,
             datalogging_manager=self.datalogging_manager,
             enable_debug=self.config['debug'])
 
     def validate_config(self) -> None:
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/tools/synchronous_websocket_server.py` & `scrutinydebugger-0.2.0/scrutiny/tools/synchronous_websocket_server.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.1.0/scrutiny/tools/throttler.py` & `scrutinydebugger-0.2.0/scrutiny/tools/throttler.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,26 +65,26 @@
 
     def get_bitrate(self) -> float:
         """Return the target average bitrate"""
         return self.mean_bitrate
 
     def reset(self) -> None:
         """ Sets the throttler to its initial state"""
-        self.last_process_timestamp = time.time()
+        self.last_process_timestamp = time.perf_counter()
         self.estimated_bitrate_slow = 0
         self.estimated_bitrate_fast = 0
         self.consumed_since_last_estimation = 0
 
     def process(self) -> None:
         """To be called periodically as fast as possible."""
         if not self.enabled:
             self.reset()
             return
 
-        t = time.time()
+        t = time.perf_counter()
         dt = t - self.last_process_timestamp
         if dt > self.bitrate_estimation_window:
             # We need to update the filters, e.g. our estimation of the bitrate
             # The time delta (dT) is variable because of thread resolution. We need to recompute the
             # filters weights every time
             instant_bitrate = self.consumed_since_last_estimation / dt  # Filters inputs
```

### Comparing `scrutinydebugger-0.1.0/scrutiny/tools/timer.py` & `scrutinydebugger-0.2.0/scrutiny/tools/timer.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 
     def set_timeout(self, timeout: float) -> None:
         self.timeout = timeout
 
     def start(self, timeout: Optional[float] = None) -> None:
         if timeout is not None:
             self.set_timeout(timeout)
-        self.start_time = time.time()
+        self.start_time = time.monotonic()
 
     def stop(self) -> None:
         self.start_time = None
 
     def elapsed(self) -> float:
         if self.start_time is not None:
-            return time.time() - self.start_time
+            return time.monotonic() - self.start_time
         else:
             return 0
 
     def is_timed_out(self) -> bool:
         if self.is_stopped() or self.timeout is None:
             return False
         else:
```

### Comparing `scrutinydebugger-0.1.0/scrutinydebugger.egg-info/PKG-INFO` & `scrutinydebugger-0.2.0/scrutinydebugger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrutinydebugger
-Version: 0.1.0
+Version: 0.2.0
 Summary: Scrutiny debugger Python framework
 Home-page: https://github.com/scrutinydebugger/scrutiny-python
 Author: Pier-Yves Lessard
 License: MIT
 Requires-Python: >3.8
 License-File: LICENSE
 Requires-Dist: appdirs>=1.4.4
```

### Comparing `scrutinydebugger-0.1.0/scrutinydebugger.egg-info/SOURCES.txt` & `scrutinydebugger-0.2.0/scrutinydebugger.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 scrutiny/sdk/_api_parser.py
 scrutiny/sdk/client.py
 scrutiny/sdk/datalogging.py
 scrutiny/sdk/definitions.py
 scrutiny/sdk/exceptions.py
 scrutiny/sdk/watchable_handle.py
 scrutiny/sdk/write_request.py
+scrutiny/sdk/listeners/__init__.py
+scrutiny/sdk/listeners/buffered_reader_listener.py
+scrutiny/sdk/listeners/csv_file_listener.py
+scrutiny/sdk/listeners/text_stream_listener.py
 scrutiny/server/__init__.py
 scrutiny/server/active_sfd_handler.py
 scrutiny/server/server.py
 scrutiny/server/api/API.py
 scrutiny/server/api/__init__.py
 scrutiny/server/api/abstract_client_handler.py
 scrutiny/server/api/dummy_client_handler.py
```

### Comparing `scrutinydebugger-0.1.0/setup.py` & `scrutinydebugger-0.2.0/setup.py`

 * *Files identical despite different names*

