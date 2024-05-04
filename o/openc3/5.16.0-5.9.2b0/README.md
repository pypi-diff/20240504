# Comparing `tmp/openc3-5.16.0.tar.gz` & `tmp/openc3-5.9.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openc3-5.16.0.tar", last modified: Sat May  4 03:13:09 2024, max compression
+gzip compressed data, was "openc3-5.9.2b0.tar", last modified: Fri Aug  4 17:12:46 2023, max compression
```

## Comparing `openc3-5.16.0.tar` & `openc3-5.9.2b0.tar`

### file list

```diff
@@ -1,346 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.804258 openc3-5.16.0/
--rw-r--r--   0 runner    (1001) docker     (127)    37778 2024-05-04 03:12:39.000000 openc3-5.16.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-04 03:12:39.000000 openc3-5.16.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-04 03:13:09.804258 openc3-5.16.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-04 03:12:39.000000 openc3-5.16.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.756258 openc3-5.16.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-04 03:12:39.000000 openc3-5.16.0/examples/cosmos_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-04 03:12:39.000000 openc3-5.16.0/examples/cosmos_web_socket_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-04 03:12:39.000000 openc3-5.16.0/examples/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-04 03:12:39.000000 openc3-5.16.0/examples/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.760258 openc3-5.16.0/openc3/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-04 03:13:04.000000 openc3-5.16.0/openc3/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.760258 openc3-5.16.0/openc3/accessors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/accessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/accessors/accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    48459 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/accessors/binary_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/accessors/cbor_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/accessors/html_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/accessors/json_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/accessors/xml_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.760258 openc3-5.16.0/openc3/api/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/api/authorized_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23935 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/api/cmd_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/api/config_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/api/interface_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18236 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/api/limits_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/api/router_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/api/settings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/api/stash_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/api/target_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23234 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/api/tlm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.760258 openc3-5.16.0/openc3/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/config/config_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.764258 openc3-5.16.0/openc3/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/generic_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/packet_time_formatted_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/packet_time_seconds_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/polynomial_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/processor_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/received_count_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/received_time_formatted_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/received_time_seconds_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/segmented_polynomial_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/unix_time_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/unix_time_formatted_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/conversions/unix_time_seconds_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.764258 openc3-5.16.0/openc3/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20981 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.768258 openc3-5.16.0/openc3/interfaces/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/protocols/burst_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/protocols/cobs_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/protocols/crc_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/protocols/fixed_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/protocols/ignore_packet_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/protocols/length_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/protocols/preidentified_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/protocols/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/protocols/slip_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/protocols/template_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/protocols/terminated_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/simulated_target_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/stream_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/tcpip_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/tcpip_server_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/interfaces/udp_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.768258 openc3-5.16.0/openc3/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/io/io_multiplexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/io/json_api_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/io/json_drb_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/io/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/io/stderr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/io/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/io/udp_sockets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.768258 openc3-5.16.0/openc3/logs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/logs/log_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/logs/stream_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/logs/stream_log_pair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.768258 openc3-5.16.0/openc3/microservices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/microservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/microservices/decom_microservice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/microservices/interface_decom_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    36903 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/microservices/interface_microservice.py
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/microservices/microservice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/microservices/router_microservice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.772258 openc3-5.16.0/openc3/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17546 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/cvt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/interface_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/interface_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/metric_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/microservice_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/microservice_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/reducer_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/router_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/router_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/secret_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/setting_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/stash_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/models/tool_config_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.772258 openc3-5.16.0/openc3/packets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14028 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/limits_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    52019 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/packet.py
--rw-r--r--   0 runner    (1001) docker     (127)    34943 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/packet_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27405 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/packet_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/packet_item_limits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.776258 openc3-5.16.0/openc3/packets/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/parsers/format_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/parsers/limits_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/parsers/limits_response_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/parsers/packet_item_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/parsers/packet_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/parsers/processor_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/parsers/state_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22492 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/structure_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    17624 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/packets/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.776258 openc3-5.16.0/openc3/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/processors/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/processors/statistics_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/processors/watermark_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.780258 openc3-5.16.0/openc3/script/
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38077 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/api_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/cosmos_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/screen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/server_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/stream_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)    19793 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/suite_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/suite_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18365 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/script/web_socket_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.780258 openc3-5.16.0/openc3/streams/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/streams/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/streams/tcpip_client_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/streams/tcpip_socket_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/streams/web_socket_client_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.780258 openc3-5.16.0/openc3/system/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/system/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     8812 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/system/target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.780258 openc3-5.16.0/openc3/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.780258 openc3-5.16.0/openc3/tools/test_runner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/tools/test_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/tools/test_runner/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/top_level.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.780258 openc3-5.16.0/openc3/topics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/topics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/topics/command_decom_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/topics/command_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/topics/decom_interface_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/topics/interface_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/topics/limits_event_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/topics/router_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/topics/telemetry_decom_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/topics/telemetry_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/topics/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.784258 openc3-5.16.0/openc3/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/aws_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/bucket_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/crc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/kubernetes_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/local_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    21733 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/local_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/message_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/redis_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/simulated_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/sleeper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/store_queued.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/target_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/target_file_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-04 03:12:39.000000 openc3-5.16.0/openc3/utilities/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.804258 openc3-5.16.0/openc3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-04 03:13:09.000000 openc3-5.16.0/openc3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-05-04 03:13:09.000000 openc3-5.16.0/openc3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 03:13:09.000000 openc3-5.16.0/openc3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 03:13:09.000000 openc3-5.16.0/openc3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-04 03:13:09.804258 openc3-5.16.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-04 03:12:39.000000 openc3-5.16.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.788258 openc3-5.16.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.788258 openc3-5.16.0/test/accessors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/accessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43330 2024-05-04 03:12:39.000000 openc3-5.16.0/test/accessors/test_binary_accessor_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    96495 2024-05-04 03:12:39.000000 openc3-5.16.0/test/accessors/test_binary_accessor_write.py
--rw-r--r--   0 runner    (1001) docker     (127)    20312 2024-05-04 03:12:39.000000 openc3-5.16.0/test/accessors/test_cbor_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-05-04 03:12:39.000000 openc3-5.16.0/test/accessors/test_html_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19760 2024-05-04 03:12:39.000000 openc3-5.16.0/test/accessors/test_json_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-04 03:12:39.000000 openc3-5.16.0/test/accessors/test_xml_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.788258 openc3-5.16.0/test/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33638 2024-05-04 03:12:39.000000 openc3-5.16.0/test/api/test_cmd_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-04 03:12:39.000000 openc3-5.16.0/test/api/test_config_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-05-04 03:12:39.000000 openc3-5.16.0/test/api/test_interface_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21026 2024-05-04 03:12:39.000000 openc3-5.16.0/test/api/test_limits_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-04 03:12:39.000000 openc3-5.16.0/test/api/test_router_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-04 03:12:39.000000 openc3-5.16.0/test/api/test_settings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-04 03:12:39.000000 openc3-5.16.0/test/api/test_stash_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-04 03:12:39.000000 openc3-5.16.0/test/api/test_target_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46966 2024-05-04 03:12:39.000000 openc3-5.16.0/test/api/test_tlm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.788258 openc3-5.16.0/test/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22721 2024-05-04 03:12:39.000000 openc3-5.16.0/test/config/test_config_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.792258 openc3-5.16.0/test/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/test_generic_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/test_packet_time_formatted_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/test_packet_time_seconds_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/test_polynomial_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/test_processor_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/test_received_count_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/test_received_time_formatted_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/test_received_time_seconds_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/test_segmented_polynomial_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/test_unix_time_formatted_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-04 03:12:39.000000 openc3-5.16.0/test/conversions/test_unix_time_seconds_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.792258 openc3-5.16.0/test/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.796258 openc3-5.16.0/test/interfaces/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/protocols/test_burst_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/protocols/test_cobs_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    35019 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/protocols/test_crc_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/protocols/test_fixed_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    11567 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/protocols/test_ignore_packet_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    28662 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/protocols/test_length_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/protocols/test_preidentified_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    11933 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/protocols/test_slip_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    23894 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/protocols/test_template_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/protocols/test_terminated_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/sim_tgt_inst.py
--rw-r--r--   0 runner    (1001) docker     (127)    27943 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/test_simulated_target_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/test_stream_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/test_tcpip_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/test_tcpip_server_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-04 03:12:39.000000 openc3-5.16.0/test/interfaces/test_udp_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.796258 openc3-5.16.0/test/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-04 03:12:39.000000 openc3-5.16.0/test/io/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-04 03:12:39.000000 openc3-5.16.0/test/io/test_udp_sockets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.796258 openc3-5.16.0/test/logs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-04 03:12:39.000000 openc3-5.16.0/test/logs/test_stream_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.796258 openc3-5.16.0/test/microservices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/microservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18809 2024-05-04 03:12:39.000000 openc3-5.16.0/test/microservices/test_interface_microservice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-04 03:12:39.000000 openc3-5.16.0/test/microservices/test_microservice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.800258 openc3-5.16.0/test/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27329 2024-05-04 03:12:39.000000 openc3-5.16.0/test/models/test_cvt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-05-04 03:12:39.000000 openc3-5.16.0/test/models/test_interface_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-04 03:12:39.000000 openc3-5.16.0/test/models/test_interface_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-04 03:12:39.000000 openc3-5.16.0/test/models/test_microservice_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-04 03:12:39.000000 openc3-5.16.0/test/models/test_microservice_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-04 03:12:39.000000 openc3-5.16.0/test/models/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-04 03:12:39.000000 openc3-5.16.0/test/models/test_router_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-04 03:12:39.000000 openc3-5.16.0/test/models/test_tool_config_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.800258 openc3-5.16.0/test/packets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.800258 openc3-5.16.0/test/packets/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/parsers/test_format_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14849 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/parsers/test_limits_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/parsers/test_limits_response_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    21248 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/parsers/test_packet_item_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/parsers/test_packet_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/parsers/test_processor_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/parsers/test_state_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    74976 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/test_packet.py
--rw-r--r--   0 runner    (1001) docker     (127)    52616 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/test_packet_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    26498 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/test_packet_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    26874 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    11084 2024-05-04 03:12:39.000000 openc3-5.16.0/test/packets/test_structure_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.800258 openc3-5.16.0/test/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-04 03:12:39.000000 openc3-5.16.0/test/processors/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-04 03:12:39.000000 openc3-5.16.0/test/processors/test_statistics_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-04 03:12:39.000000 openc3-5.16.0/test/processors/test_watermark_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.804258 openc3-5.16.0/test/script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38738 2024-05-04 03:12:39.000000 openc3-5.16.0/test/script/test_api_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-04 03:12:39.000000 openc3-5.16.0/test/script/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-04 03:12:39.000000 openc3-5.16.0/test/script/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-04 03:12:39.000000 openc3-5.16.0/test/script/test_telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.804258 openc3-5.16.0/test/streams/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-04 03:12:39.000000 openc3-5.16.0/test/streams/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-04 03:12:39.000000 openc3-5.16.0/test/streams/test_tcpip_client_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-04 03:12:39.000000 openc3-5.16.0/test/streams/test_tcpip_socket_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-04 03:12:39.000000 openc3-5.16.0/test/test_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-04 03:12:39.000000 openc3-5.16.0/test/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-04 03:12:39.000000 openc3-5.16.0/test/test_json_rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-04 03:12:39.000000 openc3-5.16.0/test/test_json_rpc_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-04 03:12:39.000000 openc3-5.16.0/test/test_json_rpc_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.804258 openc3-5.16.0/test/topics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/topics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-04 03:12:39.000000 openc3-5.16.0/test/topics/test_limits_event_topic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:13:09.804258 openc3-5.16.0/test/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:12:39.000000 openc3-5.16.0/test/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-04 03:12:39.000000 openc3-5.16.0/test/utilities/test_crc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-04 03:12:39.000000 openc3-5.16.0/test/utilities/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-04 03:12:39.000000 openc3-5.16.0/test/utilities/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-04 03:12:39.000000 openc3-5.16.0/test/utilities/test_target_file_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-04 03:12:39.000000 openc3-5.16.0/test/utilities/test_time.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.398862 openc3-5.9.2b0/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    37778 2023-07-27 22:17:09.000000 openc3-5.9.2b0/LICENSE.txt
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      105 2023-07-27 22:17:09.000000 openc3-5.9.2b0/MANIFEST.in
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2574 2023-08-04 17:12:46.398959 openc3-5.9.2b0/PKG-INFO
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1863 2023-07-27 22:17:09.000000 openc3-5.9.2b0/README.md
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.370315 openc3-5.9.2b0/examples/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2000 2023-07-27 22:17:09.000000 openc3-5.9.2b0/examples/cosmos_v5_enterprise_example.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1958 2023-07-27 22:17:09.000000 openc3-5.9.2b0/examples/cosmos_v5_example.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2345 2023-07-27 22:17:09.000000 openc3-5.9.2b0/examples/cosmos_v5_stream_example.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      247 2023-07-27 22:17:09.000000 openc3-5.9.2b0/examples/test.txt
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.371092 openc3-5.9.2b0/openc3/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      198 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      579 2023-08-04 14:20:46.000000 openc3-5.9.2b0/openc3/__version__.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.372671 openc3-5.9.2b0/openc3/accessors/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-31 15:36:25.000000 openc3-5.9.2b0/openc3/accessors/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2248 2023-08-01 16:42:30.000000 openc3-5.9.2b0/openc3/accessors/accessor.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    47372 2023-08-04 14:01:26.000000 openc3-5.9.2b0/openc3/accessors/binary_accessor.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.374922 openc3-5.9.2b0/openc3/api/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      795 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/api/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      764 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/api/authorized_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    19507 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/api/cmd_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     6215 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/api/interface_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1928 2023-08-04 13:58:29.000000 openc3-5.9.2b0/openc3/api/stash_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    20397 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/api/tlm_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     5827 2023-08-04 01:56:57.000000 openc3-5.9.2b0/openc3/environment.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.376877 openc3-5.9.2b0/openc3/io/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/io/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2062 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/io/io_multiplexer.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     7318 2023-08-04 03:14:31.000000 openc3-5.9.2b0/openc3/io/json_api_object.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     6037 2023-08-04 03:07:34.000000 openc3-5.9.2b0/openc3/io/json_drb_object.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    10670 2023-08-01 16:42:30.000000 openc3-5.9.2b0/openc3/io/json_rpc.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1109 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/io/stderr.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1110 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/io/stdout.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.378193 openc3-5.9.2b0/openc3/models/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/models/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    12403 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/models/cvt_model.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1920 2023-08-01 23:35:45.000000 openc3-5.9.2b0/openc3/models/interface_model.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     6015 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/models/model.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3237 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/models/reducer_model.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1698 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/models/stash_model.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4134 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/models/target_model.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.381046 openc3-5.9.2b0/openc3/packets/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/packets/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    12363 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/packets/commands.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     7710 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/packets/limits.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3467 2023-07-31 15:36:25.000000 openc3-5.9.2b0/openc3/packets/packet.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    25953 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/packets/packet_config.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.381422 openc3-5.9.2b0/openc3/packets/parsers/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/packets/parsers/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4264 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/packets/parsers/packet_parser.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    23560 2023-08-04 03:14:31.000000 openc3-5.9.2b0/openc3/packets/structure.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    15419 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/packets/structure_item.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    17940 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/packets/telemetry.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.386409 openc3-5.9.2b0/openc3/script/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1735 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    37372 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/api_shared.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     7123 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/script/authorization.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     9796 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/commands.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     9444 2023-08-02 00:19:22.000000 openc3-5.9.2b0/openc3/script/cosmos_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1677 2023-08-01 23:37:42.000000 openc3-5.9.2b0/openc3/script/decorators.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      799 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/script/exceptions.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1470 2023-08-02 00:19:40.000000 openc3-5.9.2b0/openc3/script/internal_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1350 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/limits.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4492 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/metadata.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4396 2023-08-02 03:25:30.000000 openc3-5.9.2b0/openc3/script/screen.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3648 2023-08-04 02:39:26.000000 openc3-5.9.2b0/openc3/script/server_proxy.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     6556 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/storage.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     7417 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/script/stream.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4432 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/script/stream_shared.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    18113 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/suite.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     5272 2023-08-01 23:41:45.000000 openc3-5.9.2b0/openc3/script/suite_results.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    10614 2023-08-02 00:20:56.000000 openc3-5.9.2b0/openc3/script/suite_runner.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3194 2023-08-02 00:21:33.000000 openc3-5.9.2b0/openc3/script/telemetry.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.387311 openc3-5.9.2b0/openc3/stream_api/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/stream_api/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1565 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/stream_api/base_client.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4588 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/stream_api/data_extractor_client.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3030 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/stream_api/log_message_client.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.389507 openc3-5.9.2b0/openc3/system/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/system/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     5056 2023-08-01 23:42:17.000000 openc3-5.9.2b0/openc3/system/system.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     8505 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/system/target.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3716 2023-08-01 17:27:18.000000 openc3-5.9.2b0/openc3/top_level.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.390802 openc3-5.9.2b0/openc3/topics/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/topics/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3517 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/topics/command_decom_topic.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3894 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/topics/command_topic.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2695 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/topics/decom_interface_topic.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1532 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/topics/interface_topic.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1586 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/topics/topic.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.394107 openc3-5.9.2b0/openc3/utilities/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/utilities/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     5990 2023-08-04 03:15:28.000000 openc3-5.9.2b0/openc3/utilities/authentication.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1497 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/utilities/authorization.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     8776 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/utilities/aws_bucket.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3898 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/utilities/bucket.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4672 2023-08-01 20:44:09.000000 openc3-5.9.2b0/openc3/utilities/bucket_utilities.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1342 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/utilities/connection_pool.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     8481 2023-08-01 23:44:42.000000 openc3-5.9.2b0/openc3/utilities/extract.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      746 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/utilities/local_bucket.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1032 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/utilities/local_mode.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4951 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/utilities/logger.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3889 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/utilities/message_log.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1545 2023-08-01 23:19:42.000000 openc3-5.9.2b0/openc3/utilities/script_shared.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1608 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/utilities/sleeper.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     8345 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/utilities/store.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1697 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/utilities/target_file.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.371958 openc3-5.9.2b0/openc3.egg-info/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2574 2023-08-04 17:12:46.000000 openc3-5.9.2b0/openc3.egg-info/PKG-INFO
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3119 2023-08-04 17:12:46.000000 openc3-5.9.2b0/openc3.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        1 2023-08-04 17:12:46.000000 openc3-5.9.2b0/openc3.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanmelt   (501) staff       (20)       12 2023-08-04 17:12:46.000000 openc3-5.9.2b0/openc3.egg-info/top_level.txt
+-rw-r--r--   0 ryanmelt   (501) staff       (20)       67 2023-08-04 17:12:46.399243 openc3-5.9.2b0/setup.cfg
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3834 2023-08-04 17:06:36.000000 openc3-5.9.2b0/setup.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.395294 openc3-5.9.2b0/test/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/test/__init__.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.396639 openc3-5.9.2b0/test/accessors/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-31 15:36:25.000000 openc3-5.9.2b0/test/accessors/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    42817 2023-08-04 03:14:31.000000 openc3-5.9.2b0/test/accessors/test_binary_accessor_read.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)   101175 2023-08-04 03:14:31.000000 openc3-5.9.2b0/test/accessors/test_binary_accessor_write.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.397925 openc3-5.9.2b0/test/api/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-31 15:36:25.000000 openc3-5.9.2b0/test/api/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     6472 2023-08-02 22:48:03.000000 openc3-5.9.2b0/test/api/test_cmd_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2395 2023-08-02 22:48:03.000000 openc3-5.9.2b0/test/api/test_tlm_api.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.398437 openc3-5.9.2b0/test/config/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/test/config/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    22765 2023-07-31 15:36:25.000000 openc3-5.9.2b0/test/config/test_config_parser.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2654 2023-07-27 22:17:09.000000 openc3-5.9.2b0/test/test_authorization.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1329 2023-07-27 22:17:09.000000 openc3-5.9.2b0/test/test_helper.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      959 2023-08-01 16:42:30.000000 openc3-5.9.2b0/test/test_json_rpc_error.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2278 2023-08-01 16:42:30.000000 openc3-5.9.2b0/test/test_json_rpc_request.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2858 2023-08-01 16:42:30.000000 openc3-5.9.2b0/test/test_json_rpc_response.py
```

### Comparing `openc3-5.16.0/LICENSE.txt` & `openc3-5.9.2b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openc3-5.16.0/PKG-INFO` & `openc3-5.9.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openc3
-Version: 5.16.0
+Version: 5.9.2b0
 Summary: Python Support for OpenC3 COSMOS v5
 Home-page: https://github.com/OpenC3/cosmos
 Author: Ryan Melton
 Author-email: ryan@openc3.com
 License: AGPLv3, Nonstandard
 Keywords: openc3 cosmos
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openc3-5.16.0/README.md` & `openc3-5.9.2b0/README.md`

 * *Files identical despite different names*

### Comparing `openc3-5.16.0/examples/cosmos_example.py` & `openc3-5.9.2b0/examples/cosmos_v5_enterprise_example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,69 @@
 import os
+import sys
 
 # See openc3/docs/environment.md for environment documentation
-# These VALUES are required for COSMOS Enterprise
-# os.environ["OPENC3_API_USER"] = "operator"
-# os.environ["OPENC3_API_PASSWORD"] = "operator"
-# This value is the only one required for COSMOS Open Source
-os.environ["OPENC3_API_PASSWORD"] = "password"
 
+os.environ["OPENC3_API_USER"] = "operator"
+os.environ["OPENC3_API_PASSWORD"] = "operator"
 os.environ["OPENC3_LOG_LEVEL"] = "INFO"
 os.environ["OPENC3_API_SCHEMA"] = "http"
 os.environ["OPENC3_API_HOSTNAME"] = "127.0.0.1"
 os.environ["OPENC3_API_PORT"] = "2900"
-# This import must be after the os.environ settings
+
 from openc3.script import *
 
-# telemetry.py
+print(cosmos_status())
+print(cosmos_health())
+
+# ~ # telemetry.py
 print(tlm("INST HEALTH_STATUS TEMP1"))
 print(tlm_raw("INST HEALTH_STATUS TEMP1"))
 print(tlm_formatted("INST HEALTH_STATUS TEMP1"))
 print(tlm_with_units("INST HEALTH_STATUS TEMP1"))
+print(tlm_variable("INST HEALTH_STATUS TEMP1", "RAW"))
 print(set_tlm("INST HEALTH_STATUS TEMP1 = 5"))
 print(get_tlm_packet("INST", "HEALTH_STATUS"))
 print(
     get_tlm_values(
         [
             "INST__HEALTH_STATUS__TEMP1__CONVERTED",
             "INST__HEALTH_STATUS__TEMP2__CONVERTED",
         ]
     )
 )
-print(get_target_names())
+print(get_target_list())
 print(get_target("INST"))
 print(get_tlm_buffer("INST", "HEALTH_STATUS"))
 
 id_ = subscribe_packets([["INST", "HEALTH_STATUS"]])
 print(id_)
 
+sys.exit(1)
+
+FILE_PATH = os.path.dirname(os.path.abspath(__file__))
 # commands.py
 cmd("INST ABORT")
 cmd_no_range_check("INST COLLECT with TYPE NORMAL, TEMP 50.0")
 cmd_no_hazardous_check("INST CLEAR")
 cmd_no_checks("INST COLLECT with TYPE SPECIAL, TEMP 50.0")
 cmd_raw("INST COLLECT with TYPE 0, TEMP 10.0")
 cmd_raw_no_range_check("INST COLLECT with TYPE 0, TEMP 50.0")
 cmd_raw_no_hazardous_check("INST CLEAR")
 cmd_raw_no_checks("INST COLLECT with TYPE 1, TEMP 50.0")
 send_raw("EXAMPLE_INT", "\x00\x00\x00\x00")
-get_cmd_hazardous("INST CLEAR")
-get_cmd_value("INST COLLECT TEMP")
+send_raw_file("EXAMPLE_INT", os.path.join(FILE_PATH, "test.txt"))
+get_cmd_list("INST")
+get_cmd_param_list("INST", "COLLECT")
+get_cmd_hazardous("INST", "CLEAR")
+get_cmd_value("INST", "COLLECT", "TEMP")
 get_cmd_time()
-get_cmd_buffer("INST COLLECT")
+get_cmd_buffer("INST", "COLLECT")
 cmd_no_range_check("INST COLLECT with TYPE NORMAL, TEMP 50.0")
+
+
+# timeline_api.py
+print(cosmos_timelines())
+
+update_scope("UPDATE")
+
+shutdown()
```

### Comparing `openc3-5.16.0/openc3/__version__.py` & `openc3-5.9.2b0/openc3/__version__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Lesser General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 __title__ = "openc3"
 __description__ = "Python Support for OpenC3 COSMOS v5"
 __url__ = "https://github.com/OpenC3/cosmos"
-__version__ = "5.16.0"
+__version__ = "5.9.2-beta0"
```

### Comparing `openc3-5.16.0/openc3/accessors/binary_accessor.py` & `openc3-5.9.2b0/openc3/accessors/binary_accessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -101,15 +103,15 @@
             f"{len(buffer)} byte buffer insufficient to {read_write} {data_type} at bit_offset {given_bit_offset} with bit_size {given_bit_size}"
         )
 
     # Valid endianess
     ENDIANNESS = ["BIG_ENDIAN", "LITTLE_ENDIAN"]
 
     @classmethod
-    def class_read_item(cls, item, buffer):
+    def read_item(cls, item, buffer):
         if item.data_type == "DERIVED":
             return None
         if item.array_size:
             return cls.read_array(
                 item.bit_offset,
                 item.bit_size,
                 item.data_type,
@@ -119,15 +121,15 @@
             )
         else:
             return cls.read(
                 item.bit_offset, item.bit_size, item.data_type, buffer, item.endianness
             )
 
     @classmethod
-    def class_write_item(cls, item, value, buffer):
+    def write_item(cls, item, value, buffer):
         if item.data_type == "DERIVED":
             return None
         if item.array_size:
             return cls.write_array(
                 value,
                 item.bit_offset,
                 item.bit_size,
@@ -188,25 +190,18 @@
         if data_type in ["STRING", "BLOCK"]:
             #######################################
             # Handle 'STRING' and 'BLOCK' data types
             #######################################
 
             if cls.byte_aligned(bit_offset):
                 if data_type == "STRING":
+                    buffer = buffer[lower_bound : (upper_bound + 1)]
                     try:
-                        buffer = buffer[lower_bound : (upper_bound + 1)]
-                        try:
-                            return buffer[: buffer.index(b"\00")].decode(
-                                encoding="utf-8"
-                            )
-                        except ValueError:
-                            return buffer.decode(encoding="utf-8")
-                    # If this 'STRING' contains binary buffer.decode will fail
-                    # Instead of blowing up return the original buffer
-                    except UnicodeDecodeError:
+                        return buffer[: buffer.index(b"\00")]
+                    except ValueError:
                         return buffer
                 else:  # BLOCK
                     return buffer[lower_bound : upper_bound + 1]
 
             else:
                 raise AttributeError(
                     f"bit_offset {given_bit_offset} is not byte aligned for data_type {data_type}"
@@ -352,18 +347,15 @@
 
         if (data_type == "STRING") or (data_type == "BLOCK"):
             #######################################
             # Handle 'STRING' and 'BLOCK' data types
             #######################################
 
             if cls.byte_aligned(bit_offset):
-                if data_type == "STRING" and type(value) == str:
-                    temp = value.encode(encoding="utf-8")
-                else:
-                    temp = value
+                temp = value
                 if given_bit_size <= 0:
                     end_bytes = -math.floor(given_bit_size / 8)
                     old_upper_bound = len(buffer) - 1 - end_bytes
                     # Lower bound + end_bytes can never be more than 1 byte outside of the given buffer
                     if (lower_bound + end_bytes) > len(buffer):
                         cls.raise_buffer_error(
                             "write", buffer, data_type, given_bit_offset, given_bit_size
@@ -392,18 +384,14 @@
                         buffer[upper_bound + 1 : upper_bound + 1 + end_bytes] = buffer[
                             old_upper_bound + 1 : old_upper_bound + 1 + end_bytes
                         ]
 
                 else:  # given_bit_size > 0
                     byte_size = math.floor(bit_size / 8)
                     if len(value) < byte_size:
-                        if type(value) is str:
-                            ba = bytearray()
-                            ba.extend(value.encode(encoding="utf-8"))
-                            value = ba
                         # Pad the requested size with zeros
                         temp = value.ljust(byte_size, b"\00")
                     elif len(value) > byte_size:
                         if overflow == "TRUNCATE":
                             # Resize the value to fit the field
                             temp = value[0:byte_size]
                         else:
@@ -524,15 +512,15 @@
             value = float(value)
 
             if cls.byte_aligned(bit_offset):
                 if bit_size in [32, 64]:
                     const = getattr(BinaryAccessor, f"STRUCT_{data_type}_{bit_size}")
                     endian = getattr(BinaryAccessor, f"STRUCT_{endianness}")
                     format = "%s%s" % (endian, const)
-                    buffer[lower_bound : upper_bound + 1] = struct.pack(
+                    buffer[lower_bound:upper_bound] = struct.pack(
                         format,
                         value,
                     )
                 else:
                     raise AttributeError(
                         f"bit_size is {given_bit_size} but must be 32 or 64 for data_type {data_type}"
                     )
@@ -948,19 +936,14 @@
                 f"too many values {len(values)} for given array_size {given_array_size} and bit_size {given_bit_size}"
             )
 
         # Check overflow type
         if overflow not in BinaryAccessor.OVERFLOW_TYPES:
             raise AttributeError(f"unknown overflow type {overflow}")
 
-        # Expand the values by appending 0
-        if len(values) < num_writes:
-            for _ in range(0, (num_writes - len(values))):
-                values.append(0)
-
         match data_type:
             case "STRING" | "BLOCK":
                 #######################################
                 # Handle 'STRING' and 'BLOCK' data types
                 #######################################
 
                 if byte_aligned:
@@ -1153,34 +1136,23 @@
     # @param data_type [Symbol] {DATA_TYPES}
     # @param overflow [Symbol] {OVERFLOW_TYPES}
     # @return [Array[Integer]] Potentially modified values
     @classmethod
     def check_overflow_array(
         cls, values, min_value, max_value, hex_max_value, bit_size, data_type, overflow
     ):
-        for index, value in enumerate(values):
-            values[index] = cls.check_overflow(
-                value,
-                min_value,
-                max_value,
-                hex_max_value,
-                bit_size,
-                data_type,
-                overflow,
-            )
+        if overflow != "TRUNCATE":
+            for index, value in enumerate(values):
+                values[index] = cls.check_overflow(
+                    value,
+                    min_value,
+                    max_value,
+                    hex_max_value,
+                    bit_size,
+                    data_type,
+                    overflow,
+                )
         return values
 
-    def enforce_encoding(self):
-        return "ASCII-8BIT"
-
-    def enforce_length(self):
-        return True
-
-    def enforce_short_buffer_allowed(self):
-        return False
-
-    def enforce_derived_write_conversion(self, item):
-        return True
-
 
 # Store the host endianness so that it only has to be determined once
 BinaryAccessor.HOST_ENDIANNESS = BinaryAccessor.get_host_endianness()
```

### Comparing `openc3-5.16.0/openc3/accessors/html_accessor.py` & `openc3-5.9.2b0/openc3/api/authorized_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -10,19 +12,11 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-from openc3.accessors.xml_accessor import XmlAccessor
-import lxml.html as HTML
-
-
-class HtmlAccessor(XmlAccessor):
-    @classmethod
-    def buffer_to_doc(cls, buffer):
-        return HTML.fromstring(buffer)
+OPENC3_AUTHORIZE = True
 
-    @classmethod
-    def doc_to_buffer(cls, doc):
-        return HTML.tostring(doc)
+# TODO: Import everything somehow?
+# from .tlm_api import *
```

### Comparing `openc3-5.16.0/openc3/accessors/json_accessor.py` & `openc3-5.9.2b0/openc3/accessors/accessor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -10,64 +12,57 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-import json
-from jsonpath_ng import parse
-from .accessor import Accessor
 
+class Accessor:
+    def read_item(item, buffer):
+        raise Exception("Must be defined by subclass")
 
-class JsonAccessor(Accessor):
-    @classmethod
-    def class_read_item(cls, item, buffer):
-        if item.data_type == "DERIVED":
-            return None
-        if type(buffer) is bytearray:
-            buffer = json.loads(buffer.decode())
-        result = parse(item.key).find(buffer)
-        return cls.convert_to_type(result[0].value, item)
+    def write_item(item, value, buffer):
+        raise Exception("Must be defined by subclass")
 
     @classmethod
-    def class_write_item(cls, item, value, buffer):
-        if item.data_type == "DERIVED":
-            return None
-        if type(buffer) is bytearray:
-            decoded = json.loads(buffer.decode())
-        else:
-            decoded = buffer
-
-        value = cls.convert_to_type(value, item)
-        result = parse(item.key).update(decoded, value)
-
-        if type(buffer) is bytearray:
-            buffer[0:] = bytearray(json.dumps(result), encoding="utf-8")
+    def read_items(cls, items, buffer):
+        result = {}
+        for item in items:
+            result[item.name] = cls.read_item(item, buffer)
+        return result
 
     @classmethod
-    def class_read_items(cls, items, buffer):
-        if type(buffer) is bytearray:
-            buffer = json.loads(buffer.decode())
-        return super().class_read_items(items, buffer)
+    def write_items(cls, items, values, buffer):
+        for index, item in enumerate(items):
+            cls.write_item(item, values[index], buffer)
+        return buffer
 
     @classmethod
-    def class_write_items(cls, items, values, buffer):
-        if type(buffer) is bytearray:
-            decoded = json.loads(buffer.decode())
-        else:
-            decoded = buffer
-        super().class_write_items(items, values, decoded)
-        if type(buffer) is bytearray:
-            buffer[0:] = bytearray(json.dumps(decoded), encoding="utf-8")
-
-    def enforce_encoding(self):
-        return None
+    def convert_to_type(cls, value, item):
+        data_type = item.data_type
+        if (data_type == "STRING") or (data_type == "BLOCK"):
+            #######################################
+            # Handle :STRING and :BLOCK data types
+            #######################################
+            value = str(value)
+
+        elif (data_type == "INT") or (data_type == "UINT"):
+            ###################################
+            # Handle :INT data type
+            ###################################
+            value = int(value)
+
+        elif data_type == "FLOAT":
+            ##########################
+            # Handle :FLOAT data type
+            ##########################
+            value = float(value)
 
-    def enforce_length(self):
-        return False
+        else:
+            ############################
+            # Handle Unknown data types
+            ############################
 
-    def enforce_short_buffer_allowed(self):
-        return True
+            raise AttributeError(f"data_type {data_type} is not recognized")
 
-    def enforce_derived_write_conversion(self, item):
-        return True
+        return value
```

### Comparing `openc3-5.16.0/openc3/api/authorized_api.py` & `openc3-5.9.2b0/openc3/utilities/local_bucket.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
-
+#
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-OPENC3_AUTHORIZE = True
+from openc3.utilities.aws_bucket import AwsBucket
 
-# TODO: Import everything somehow?
-# from .tlm_api import *
+class LocalBucket(AwsBucket):
+    pass
```

### Comparing `openc3-5.16.0/openc3/api/cmd_api.py` & `openc3-5.9.2b0/openc3/api/cmd_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Copyright 2024 OpenC3, Inc.
+#!/usr/bin/env python3
+
+# Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addums as found in the LICENSE.txt
 #
@@ -10,22 +12,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-from contextlib import contextmanager
 from openc3.api import WHITELIST
 from openc3.api.interface_api import get_interface
-from openc3.top_level import DisabledError
 from openc3.environment import OPENC3_SCOPE
 from openc3.utilities.authorization import authorize
 from openc3.utilities.logger import Logger
-from openc3.utilities.string import simple_formatted
 from openc3.models.target_model import TargetModel
 from openc3.utilities.extract import *
 from openc3.topics.topic import Topic
 from openc3.topics.command_topic import CommandTopic
 from openc3.topics.interface_topic import InterfaceTopic
 from openc3.topics.decom_interface_topic import DecomInterfaceTopic
 from openc3.topics.command_decom_topic import CommandDecomTopic
@@ -38,27 +37,20 @@
         "cmd_no_range_check",
         "cmd_no_hazardous_check",
         "cmd_no_checks",
         "cmd_raw",
         "cmd_raw_no_range_check",
         "cmd_raw_no_hazardous_check",
         "cmd_raw_no_checks",
-        "build_cmd",
-        "build_command",  # DEPRECATED
-        "enable_cmd",
-        "disable_cmd",
+        "build_command",
         "send_raw",
-        "get_all_cmds",
-        "get_all_commands",  # DEPRECATED
-        "get_all_cmd_names",
-        "get_all_command_names",  # DEPRECATED
-        "get_cmd",
-        "get_command",  # DEPRECATED
-        "get_param",
-        "get_parameter",  # DEPRECATED
+        "get_all_commands",
+        "get_all_command_names",
+        "get_command",
+        "get_parameter",
         "get_cmd_buffer",
         "get_cmd_hazardous",
         "get_cmd_value",
         "get_cmd_time",
         "get_cmd_cnt",
         "get_cmd_cnts",
     ]
@@ -70,104 +62,109 @@
 #
 # Accepts two different calling styles:
 #   cmd("TGT CMD with PARAM1 val, PARAM2 val")
 #   cmd('TGT','CMD',{'PARAM1':val,'PARAM2':val})
 #
 # Favor the first syntax where possible as it is more succinct.
 def cmd(*args, **kwargs):
-    return _cmd_implementation(
+    return cmd_implementation(
         "cmd", *args, range_check=True, hazardous_check=True, raw=False, **kwargs
     )
 
 
 def cmd_raw(*args, **kwargs):
-    return _cmd_implementation(
+    return cmd_implementation(
         "cmd_raw", *args, range_check=True, hazardous_check=True, raw=True, **kwargs
     )
 
 
 # S a command packet to a target without performing any value range
 # checks on the parameters. Useful for testing to allow sing command
 # parameters outside the allowable range as defined in the configuration.
 def cmd_no_range_check(*args, **kwargs):
-    return _cmd_implementation(
+    return cmd_implementation(
         "cmd_no_range_check",
         *args,
         range_check=False,
         hazardous_check=True,
         raw=False,
         **kwargs,
     )
 
 
 def cmd_raw_no_range_check(*args, **kwargs):
-    return _cmd_implementation(
+    return cmd_implementation(
         "cmd_raw_no_range_check",
         *args,
         range_check=False,
         hazardous_check=True,
         raw=True,
         **kwargs,
     )
 
 
 # S a command packet to a target without performing any hazardous checks
 # both on the command itself and its parameters. Useful in scripts to
 # prevent popping up warnings to the user.
 def cmd_no_hazardous_check(*args, **kwargs):
-    return _cmd_implementation(
+    return cmd_implementation(
         "cmd_no_hazardous_check",
         *args,
         range_check=True,
         hazardous_check=False,
         raw=False,
         **kwargs,
     )
 
 
 def cmd_raw_no_hazardous_check(*args, **kwargs):
-    return _cmd_implementation(
+    return cmd_implementation(
         "cmd_raw_no_hazardous_check",
         *args,
         range_check=True,
         hazardous_check=False,
         raw=True,
         **kwargs,
     )
 
 
 # S a command packet to a target without performing any value range
 # checks or hazardous checks both on the command itself and its parameters.
 def cmd_no_checks(*args, **kwargs):
-    return _cmd_implementation(
+    return cmd_implementation(
         "cmd_no_checks",
         *args,
         range_check=False,
         hazardous_check=False,
         raw=False,
         **kwargs,
     )
 
 
 def cmd_raw_no_checks(*args, **kwargs):
-    return _cmd_implementation(
+    return cmd_implementation(
         "cmd_raw_no_checks",
         *args,
         range_check=False,
         hazardous_check=False,
         raw=True,
         **kwargs,
     )
 
 
 # Build a command binary
-def build_cmd(*args, range_check=True, raw=False, scope=OPENC3_SCOPE):
+def build_command(
+    self, *args, range_check=True, raw=False, scope=OPENC3_SCOPE, **kwargs
+):
+    self.extract_string_kwargs_to_args(args, kwargs)
     match len(args):
         case 1:
-            target_name, cmd_name, cmd_params = extract_fields_from_cmd_text(args[0])
+            target_name, cmd_name, cmd_params = self.extract_fields_from_cmd_text(
+                args[0]
+            )
         case 2 | 3:
             target_name = args[0]
             cmd_name = args[1]
             if len(args) == 2:
                 cmd_params = {}
             else:
                 cmd_params = args[2]
@@ -176,50 +173,19 @@
             raise RuntimeError(
                 f"ERROR: Invalid number of arguments ({len(args)}) passed to build_command()"
             )
     target_name = target_name.upper()
     cmd_name = cmd_name.upper()
     cmd_params = {k.upper(): v for k, v in cmd_params.items()}
     authorize(permission="cmd_info", target_name=target_name, scope=scope)
-    return DecomInterfaceTopic.build_cmd(
+    DecomInterfaceTopic.build_cmd(
         target_name, cmd_name, cmd_params, range_check, raw, scope
     )
 
 
-# build_command is DEPRECATED
-build_command = build_cmd
-
-
-# Helper method for disable_cmd / enable_cmd
-@contextmanager
-def _get_and_set_cmd(method, *args, scope=OPENC3_SCOPE):
-    target_name, command_name = _extract_target_command_names(method, *args)
-    authorize(
-        permission="admin",
-        target_name=target_name,
-        packet_name=command_name,
-        scope=scope,
-    )
-    command = TargetModel.packet(target_name, command_name, type="CMD", scope=scope)
-    yield command
-    TargetModel.set_packet(target_name, command_name, command, type="CMD", scope=scope)
-
-
-# @since 5.15.1
-def enable_cmd(*args, scope=OPENC3_SCOPE):
-    with _get_and_set_cmd("enable_cmd", *args, scope=scope) as command:
-        command.pop("disabled", None)
-
-
-# @since 5.15.1
-def disable_cmd(*args, scope=OPENC3_SCOPE):
-    with _get_and_set_cmd("disable_cmd", *args, scope=scope) as command:
-        command["disabled"] = True
-
-
 # Send a raw binary string to the specified interface.
 #
 # @param interface_name [String] The interface to s the raw binary
 # @param data [String] The raw binary data
 def send_raw(interface_name, data, scope=OPENC3_SCOPE):
     interface_name = interface_name.upper()
     authorize(permission="cmd_raw", interface_name=interface_name, scope=scope)
@@ -230,204 +196,170 @@
 
 
 # Returns the raw buffer from the most recent specified command packet.
 #
 # @param target_name [String] Target name of the command
 # @param command_name [String] Packet name of the command
 # @return [Hash] command hash with last command buffer
-def get_cmd_buffer(*args, scope=OPENC3_SCOPE):
-    target_name, command_name = _extract_target_command_names("get_cmd_buffer", *args)
+def get_cmd_buffer(target_name, command_name, scope=OPENC3_SCOPE):
+    target_name = target_name.upper()
+    command_name = command_name.upper()
     authorize(
         permission="cmd_info",
         target_name=target_name,
         packet_name=command_name,
         scope=scope,
     )
     TargetModel.packet(target_name, command_name, type="CMD", scope=scope)
     topic = f"{scope}__COMMAND__{{{target_name}}}__{command_name}"
     msg_id, msg_hash = Topic.get_newest_message(topic)
     if msg_id:
-        # Decode the keys for user convenience
-        return {k.decode(): v for (k, v) in msg_hash.items()}
+        # TODO: Python equivalent of .b?
+        # msg_hash["buffer"] = msg_hash["buffer"].b
+        return msg_hash
     return None
 
 
 # Returns an array of all the commands as a hash
 # @param target_name [String] Name of the target
 # @return [Array<Hash>] Array of all commands as a hash
-def get_all_cmds(target_name, scope=OPENC3_SCOPE):
+def get_all_commands(target_name, scope=OPENC3_SCOPE):
     target_name = target_name.upper()
     authorize(permission="cmd_info", target_name=target_name, scope=scope)
-    return TargetModel.packets(target_name, type="CMD", scope=scope)
-
-
-# get_all_commands is DEPRECATED
-get_all_commands = get_all_cmds
+    TargetModel.packets(target_name, type="CMD", scope=scope)
 
 
 # Returns an array of all the command packet names
 # @param target_name [String] Name of the target
 # @return [Array<String>] Array of all command packet names
-def get_all_cmd_names(target_name, hidden=False, scope=OPENC3_SCOPE):
-    try:
-        packets = get_all_cmds(target_name, scope=scope)
-    except RuntimeError:
-        packets = []
-    names = []
-    for packet in packets:
-        if hidden:
-            names.append(packet["packet_name"])
-        else:
-            if "hidden" not in packet:
-                names.append(packet["packet_name"])
-    return names
-
-
-# get_all_command_names is DEPRECATED
-get_all_command_names = get_all_cmd_names
+def get_all_command_names(target_name, scope=OPENC3_SCOPE):
+    target_name = target_name.upper()
+    authorize(permission="cmd_info", target_name=target_name, scope=scope)
+    TargetModel.packet_names(target_name, type="CMD", scope=scope)
 
 
 # Returns a hash of the given command
-def get_cmd(*args, scope=OPENC3_SCOPE):
-    target_name, command_name = _extract_target_command_names("get_cmd", *args)
+# @param target_name [String] Name of the target
+# @param command_name [String] Name of the packet
+# @return [Hash] Command as a hash
+def get_command(target_name, command_name, scope=OPENC3_SCOPE):
+    target_name = target_name.upper()
+    command_name = command_name.upper()
     authorize(permission="cmd_info", target_name=target_name, scope=scope)
-    return TargetModel.packet(target_name, command_name, type="CMD", scope=scope)
-
-
-# get_command is DEPRECATED
-get_command = get_cmd
+    TargetModel.packet(target_name, command_name, type="CMD", scope=scope)
 
 
 # Returns a hash of the given command parameter
 # @param target_name [String] Name of the target
 # @param command_name [String] Name of the packet
 # @param parameter_name [String] Name of the parameter
 # @return [Hash] Command parameter as a hash
-def get_param(*args, scope=OPENC3_SCOPE):
-    target_name, command_name, parameter_name = _extract_target_command_parameter_names(
-        "get_param", *args
-    )
+def get_parameter(target_name, command_name, parameter_name, scope=OPENC3_SCOPE):
+    target_name = target_name.upper()
+    command_name = command_name.upper()
+    parameter_name = parameter_name.upper()
     authorize(
         permission="cmd_info",
         target_name=target_name,
         packet_name=command_name,
         scope=scope,
     )
-    return TargetModel.packet_item(
+    TargetModel.packet_item(
         target_name, command_name, parameter_name, type="CMD", scope=scope
     )
 
 
-# get_parameter is DEPRECATED
-get_parameter = get_param
-
-
 # Returns whether the specified command is hazardous
 #
 # Accepts two different calling styles:
 #   get_cmd_hazardous("TGT CMD with PARAM1 val, PARAM2 val")
 #   get_cmd_hazardous('TGT','CMD',{'PARAM1'=>val,'PARAM2'=>val})
 #
 # @param args [String|Array<String>] See the description for calling style
 # @return [Boolean] Whether the command is hazardous
-def get_cmd_hazardous(*args, scope=OPENC3_SCOPE):
+def get_cmd_hazardous(self, *args, scope=OPENC3_SCOPE, **kwargs):
+    self.extract_string_kwargs_to_args(args, kwargs)
     match len(args):
         case 1:
             target_name, command_name, parameters = extract_fields_from_cmd_text(
                 args[0]
             )
-            target_name = target_name.upper()
-            command_name = command_name.upper()
-            parameters = {k.upper(): v for k, v in parameters.items()}
         case 2 | 3:
-            target_name = args[0].upper()
-            command_name = args[1].upper()
+            target_name = args[0]
+            command_name = args[1]
             if len(args) == 2:
                 parameters = {}
             else:
                 parameters = args[2]
 
         case _:
             # Invalid number of arguments
             raise RuntimeError(
                 f"ERROR: Invalid number of arguments ({len(args)}) passed to get_cmd_hazardous()"
             )
 
+    target_name = target_name.upper()
+    command_name = command_name.upper()
+    parameters = {k.upper(): v for k, v in parameters.items()}
+
     authorize(
         permission="cmd_info",
         target_name=target_name,
         packet_name=command_name,
         scope=scope,
     )
     packet = TargetModel.packet(target_name, command_name, type="CMD", scope=scope)
-    if packet.get("hazardous") is not None:
+    if packet["hazardous"]:
         return True
 
     for item in packet["items"]:
         if item["name"] not in parameters and "states" not in item:
             continue
 
         # States are an array of the name followed by a hash of 'value' and sometimes 'hazardous'
-        for name, hash in item["states"].items():
+        for name, hash in item["states"]:
             parameter_name = parameters[item["name"]]
             # Remove quotes from string parameters
             if type(parameter_name) == str:
-                parameter_name = parameter_name.replace('"', "").replace("'", "")
+                parameter_name = parameter_name.gsub('"', "").gsub("'", "")
             # To be hazardous the state must be marked hazardous
             # Check if either the state name or value matches the param passed
-            if hash.get("hazardous") is not None and (
+            if hash["hazardous"] and (
                 name == parameter_name or hash["value"] == parameter_name
             ):
                 return True
     return False
 
 
 # Returns a value from the specified command
+#
+# @param target_name [String] Target name of the command
+# @param command_name [String] Packet name of the command
+# @param parameter_name [String] Parameter name in the command
+# @param value_type [Symbol] How the values should be converted. Must be
+#   one of {Packet::VALUE_TYPES}
+# @return [Varies] value
 def get_cmd_value(
-    *args,
-    type="CONVERTED",
+    target_name,
+    command_name,
+    parameter_name,
+    value_type="CONVERTED",
     scope=OPENC3_SCOPE,
 ):
-    target_name = None
-    command_name = None
-    parameter_name = None
-    match len(args):
-        case 1:
-            try:
-                target_name, command_name, parameter_name = args[0].upper().split()
-            except ValueError:
-                # Do nothing because we catch it below
-                pass
-        case 3:
-            target_name = args[0].upper()
-            command_name = args[1].upper()
-            parameter_name = args[2].upper()
-        case 4:
-            target_name = args[0].upper()
-            command_name = args[1].upper()
-            parameter_name = args[2].upper()
-            type = args[3].upper()
-        case _:
-            # Invalid number of arguments
-            raise RuntimeError(
-                f"ERROR: Invalid number of arguments ({len(args)}) passed to get_cmd_value()"
-            )
-    if target_name is None or command_name is None:
-        raise RuntimeError(
-            f'ERROR: Target name, command name and parameter name required. Usage: get_cmd_value("TGT CMD PARAM") or {method_name}("TGT", "CMD", "PARAM")'
-        )
-
+    target_name = target_name.upper()
+    command_name = command_name.upper()
+    parameter_name = parameter_name.upper()
     authorize(
         permission="cmd_info",
         target_name=target_name,
         packet_name=command_name,
         scope=scope,
     )
-    return CommandDecomTopic.get_cmd_item(
-        target_name, command_name, parameter_name, type=type, scope=scope
+    CommandDecomTopic.get_cmd_item(
+        target_name, command_name, parameter_name, type=value_type, scope=scope
     )
 
 
 # Returns the time the most recent command was sent
 #
 # @param target_name [String] Target name of the command. If not given then
 #    the most recent time from all commands will be returned
@@ -447,31 +379,24 @@
         time = CommandDecomTopic.get_cmd_item(
             target_name,
             command_name,
             "RECEIVED_TIMESECONDS",
             type="CONVERTED",
             scope=scope,
         )
-        if time is None:
-            time = 0
-        return (
-            target_name,
-            command_name,
-            int(time),
-            int((time - int(time)) * 1_000_000),
-        )
+        return [target_name, command_name, int(time), (time - int(time)) * 1_000_000]
     else:
         if not target_name:
             targets = TargetModel.names(scope=scope)
         else:
             targets = [target_name.upper()]
 
-        time = 0
-        command_name = None
         for target_name in targets:
+            time = 0
+            command_name = None
             for packet in TargetModel.packets(target_name, type="CMD", scope=scope):
                 cur_time = CommandDecomTopic.get_cmd_item(
                     target_name,
                     packet["packet_name"],
                     "RECEIVED_TIMESECONDS",
                     type="CONVERTED",
                     scope=scope,
@@ -479,125 +404,84 @@
                 if not cur_time:
                     continue
 
                 if cur_time > time:
                     time = cur_time
                     command_name = packet["packet_name"]
 
-        if not command_name:
-            target_name = None
-        return (
-            target_name,
-            command_name,
-            int(time),
-            int((time - int(time)) * 1_000_000),
-        )
+            if not command_name:
+                target_name = None
+            return [
+                target_name,
+                command_name,
+                int(time),
+                (time.to_f - int(time)) * 1_000_000,
+            ]
 
 
 # Get the transmit count for a command packet
 #
 # @param target_name [String] Target name of the command
 # @param command_name [String] Packet name of the command
 # @return [Numeric] Transmit count for the command
-def get_cmd_cnt(*args, scope=OPENC3_SCOPE):
-    target_name, command_name = _extract_target_command_names("get_cmd_cnt", *args)
+def get_cmd_cnt(target_name, command_name, scope=OPENC3_SCOPE):
+    target_name = target_name.upper()
+    command_name = command_name.upper()
     authorize(
         permission="system",
         target_name=target_name,
         packet_name=command_name,
         scope=scope,
     )
     TargetModel.packet(target_name, command_name, type="CMD", scope=scope)
-    return Topic.get_cnt(f"{scope}__COMMAND__{{{target_name}}}__{command_name}")
+    Topic.get_cnt(f"{scope}__COMMAND__{{{target_name}}}__{command_name}")
 
 
 # Get the transmit counts for command packets
 #
 # @param target_commands [Array<Array<String, String>>] Array of arrays containing target_name, packet_name
 # @return [Numeric] Transmit count for the command
 def get_cmd_cnts(target_commands, scope=OPENC3_SCOPE):
     authorize(permission="system", scope=scope)
-    if type(target_commands) is list and type(target_commands[0] is list):
-        counts = []
-        for target_name, command_name in target_commands:
-            target_name = target_name.upper()
-            command_name = command_name.upper()
-            counts.append(
-                Topic.get_cnt(f"{scope}__COMMAND__{{{target_name}}}__{command_name}")
-            )
-        return counts
-    else:
-        raise RuntimeError(
-            "get_cmd_cnts takes a dict of dicts containing target, packet_name, e.g. [['INST', 'COLLECT'], ['INST', 'ABORT']]"
-        )
+    counts = []
+    for target_name, command_name in target_commands:
+        target_name = target_name.upper()
+        command_name = command_name.upper()
+        counts << Topic.get_cnt(f"{scope}__COMMAND__{{{target_name}}}__{command_name}")
+    return counts
 
 
-def _extract_target_command_names(method_name, *args):
-    target_name = None
-    command_name = None
-    match len(args):
-        case 1:
-            try:
-                target_name, command_name = args[0].upper().split()
-            except ValueError:
-                # Do nothing because we catch it below
-                pass
-        case 2:
-            target_name = args[0].upper()
-            command_name = args[1].upper()
-        case _:
-            # Invalid number of arguments
-            raise RuntimeError(
-                f"ERROR: Invalid number of arguments ({len(args)}) passed to {method_name}()"
-            )
-    if target_name is None or command_name is None:
-        raise RuntimeError(
-            f'ERROR: Target name and command name required. Usage: {method_name}("TGT CMD") or {method_name}("TGT", "CMD")'
-        )
-    return (target_name, command_name)
+###########################################################################
+# PRIVATE implementation details
+###########################################################################
 
 
-def _extract_target_command_parameter_names(method_name, *args):
-    target_name = None
-    command_name = None
-    parameter_name = None
-    match len(args):
-        case 1:
-            try:
-                target_name, command_name, parameter_name = args[0].upper().split()
-            except ValueError:
-                # Do nothing because we catch it below
-                pass
-        case 3:
-            target_name = args[0].upper()
-            command_name = args[1].upper()
-            parameter_name = args[2].upper()
-        case _:
-            # Invalid number of arguments
-            raise RuntimeError(
-                f"ERROR: Invalid number of arguments ({len(args)}) passed to {method_name}()"
-            )
-    if target_name is None or command_name is None:
-        raise RuntimeError(
-            f'ERROR: Target name, command name and parameter name required. Usage: {method_name}("TGT CMD PARAM") or {method_name}("TGT", "CMD", "PARAM")'
-        )
-    return (target_name, command_name, parameter_name)
-
-
-def _cmd_implementation(
+def cmd_implementation(
     method_name,
     *args,
     range_check,
     hazardous_check,
     raw,
+    timeout=None,
+    log_message=None,
+    scope=OPENC3_SCOPE,
     **kwargs,
 ):
-    scope = OPENC3_SCOPE
-    if kwargs.get("scope"):
-        scope = kwargs["scope"]
+    # extract_string_kwargs_to_args(args, kwargs)
+    if log_message not in [None, True, False]:
+        raise RuntimeError(
+            f"Invalid log_message parameter: {log_message}. Must be True or False."
+        )
+    if timeout is not None:
+        try:
+            float(timeout)
+        except ValueError:
+            raise RuntimeError(
+                f"Invalid timeout parameter: {timeout}. Must be numeric."
+            )
 
     match len(args):
         case 1:
             target_name, cmd_name, cmd_params = extract_fields_from_cmd_text(args[0])
         case 2 | 3:
             target_name = args[0]
             cmd_name = args[1]
@@ -614,104 +498,85 @@
     target_name = target_name.upper()
     cmd_name = cmd_name.upper()
     cmd_params = {k.upper(): v for k, v in cmd_params.items()}
     authorize(
         permission="cmd", target_name=target_name, packet_name=cmd_name, scope=scope
     )
     packet = TargetModel.packet(target_name, cmd_name, type="CMD", scope=scope)
-    if packet.get("disabled", False):
-        error = DisabledError()
-        error.target_name = target_name
-        error.cmd_name = cmd_name
-        raise error
 
     command = {
         "target_name": target_name,
         "cmd_name": cmd_name,
         "cmd_params": cmd_params,
         "range_check": str(range_check),
         "hazardous_check": str(hazardous_check),
         "raw": str(raw),
     }
-
-    timeout = None
-    if kwargs.get("timeout") is not None:
-        try:
-            timeout = float(kwargs["timeout"])
-        except ValueError:
-            raise RuntimeError(
-                f"Invalid timeout parameter: {timeout}. Must be numeric."
-            )
-
-    # Determine if we should log this command
-    log_message = True  # Default is True
-    # If the packet has the DISABLE_MESSAGES keyword then no messages
-    if packet.get("messages_disabled"):
-        log_message = False
-    else:
+    if log_message is None:  # This means the default was used, no argument was passed
+        log_message = True  # Default is True
+        # If the packet has the DISABLE_MESSAGES keyword then no messages by default
+        if packet.get("messages_disabled"):
+            log_message = False
         # Check if any of the parameters have DISABLE_MESSAGES
         for key, value in cmd_params.items():
             found = None
             for item in packet["items"]:
                 if item["name"] == key:
                     found = item
                     break
             if (
                 found
-                and "states" in found
-                and value in found["states"]
+                and found["states"]
+                and found["states"][value]
                 and found["states"][value].get("messages_disabled")
             ):
                 log_message = False
-    # If they explicitly set the log_message kwarg then that overrides the above
-    if kwargs.get("log_message") is not None:
-        if kwargs["log_message"] not in [True, False]:
-            raise RuntimeError(
-                f"Invalid log_message parameter: {log_message}. Must be True or False."
-            )
-        log_message = kwargs["log_message"]
     if log_message:
         Logger.info(
-            _cmd_log_string(method_name, target_name, cmd_name, cmd_params, packet),
+            build_cmd_output_string(target_name, cmd_name, cmd_params, packet, raw),
             scope,
         )
     return CommandTopic.send_command(command, timeout, scope)
 
 
-def _cmd_log_string(method_name, target_name, cmd_name, cmd_params, packet):
-    output_string = f'{method_name}("'
+def build_cmd_output_string(target_name, cmd_name, cmd_params, packet, raw):
+    if raw:
+        output_string = 'cmd_raw("'
+    else:
+        output_string = 'cmd("'
     output_string += target_name + " " + cmd_name
     if not cmd_params:
         output_string += '")'
     else:
         params = []
         for key, value in cmd_params.items():
             if key in Packet.RESERVED_ITEM_NAMES:
                 continue
 
         found = False
         for item in packet["items"]:
             if item["name"] == key:
                 found = item
                 break
-        if found and "data_type" in found:
+        if found:
             item_type = found["data_type"]
         else:
             item_type = None
 
-        if isinstance(value, str):
+        if type(value) == str:
+            value = value.dup
             if item_type == "BLOCK" or item_type == "STRING":
-                if not value.isascii():
-                    value = "0x" + simple_formatted(value)
+                if value.isascii():
+                    value = "0x" + value.simple_formatted
                 else:
-                    value = f"'{str(value)}'"
+                    value = str(value)
             else:
                 value = convert_to_value(value)
             if len(value) > 256:
-                value = value[:256] + "...'"
+                value = value[:255] + "...'"
             value = value.replace('"', "'")
-        elif isinstance(value, list):
-            value = f"[{', '.join(str(i) for i in value)}]"
+        elif type(value) == list:
+            value = f"[{', '.join(value)}]"
         params.append(f"{key} {value}")
         params = ", ".join(params)
         output_string += " with " + params + '")'
     return output_string
```

### Comparing `openc3-5.16.0/openc3/api/interface_api.py` & `openc3-5.9.2b0/openc3/api/interface_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addums as found in the LICENSE.txt
@@ -14,17 +16,21 @@
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 from openc3.api import WHITELIST
 from openc3.environment import OPENC3_SCOPE
 from openc3.utilities.authorization import authorize
 from openc3.models.interface_model import InterfaceModel
-from openc3.models.interface_status_model import InterfaceStatusModel
-from openc3.topics.interface_topic import InterfaceTopic
-from openc3.utilities.logger import Logger
+
+# from openc3.utilities.logger import Logger
+
+# require 'openc3/models/interface_model'
+# require 'openc3/models/interface_status_model'
+# require 'openc3/topics/interface_topic'
+
 
 WHITELIST.extend(
     [
         "get_interface",
         "get_interface_names",
         "connect_interface",
         "disconnect_interface",
@@ -44,133 +50,106 @@
 # @param interface_name [String] Interface name
 # @return [Hash] Hash of all the interface information
 def get_interface(interface_name, scope=OPENC3_SCOPE):
     authorize(permission="system", interface_name=interface_name, scope=scope)
     interface = InterfaceModel.get(name=interface_name, scope=scope)
     if not interface:
         raise RuntimeError(f"Interface '{interface_name}' does not exist")
-    return interface | InterfaceStatusModel.get(name=interface_name, scope=scope)
+    return interface
+    # interface.merge(InterfaceStatusModel.get(name=interface_name, scope=scope))
 
 
 # @return [Array<String>] All the interface names
 def get_interface_names(scope=OPENC3_SCOPE):
     authorize(permission="system", scope=scope)
-    return InterfaceModel.names(scope=scope)
-
-
-# Connects an interface and starts its telemetry gathering thread
-#
-# @param interface_name [String] The name of the interface
-# @param interface_params [Array] Optional parameters to pass to the interface
-def connect_interface(interface_name, *interface_params, scope=OPENC3_SCOPE):
-    authorize(permission="system_set", interface_name=interface_name, scope=scope)
-    InterfaceTopic.connect_interface(interface_name, *interface_params, scope=scope)
-
-
-# Disconnects from an interface and kills its telemetry gathering thread
-#
-# @param interface_name [String] The name of the interface
-def disconnect_interface(interface_name, scope=OPENC3_SCOPE):
-    authorize(permission="system_set", interface_name=interface_name, scope=scope)
-    InterfaceTopic.disconnect_interface(interface_name, scope=scope)
+    InterfaceModel.names(scope=scope)
 
 
-# Starts raw logging for an interface
-#
-# @param interface_name [String] The name of the interface
-def start_raw_logging_interface(interface_name="ALL", scope=OPENC3_SCOPE):
-    authorize(permission="system_set", interface_name=interface_name, scope=scope)
-    if interface_name == "ALL":
-        for interface_name in get_interface_names():
-            InterfaceTopic.start_raw_logging(interface_name, scope=scope)
-    else:
-        InterfaceTopic.start_raw_logging(interface_name, scope=scope)
-
-
-# Stop raw logging for an interface
-#
-# @param interface_name [String] The name of the interface
-def stop_raw_logging_interface(interface_name="ALL", scope=OPENC3_SCOPE):
-    authorize(permission="system_set", interface_name=interface_name, scope=scope)
-    if interface_name == "ALL":
-        for interface_name in get_interface_names():
-            InterfaceTopic.stop_raw_logging(interface_name, scope=scope)
-    else:
-        InterfaceTopic.stop_raw_logging(interface_name, scope=scope)
-
-
-# Get information about all interfaces
-#
-# @return [Array<Array<String, Numeric, Numeric, Numeric, Numeric, Numeric,
-#   Numeric, Numeric>>] Array of Arrays containing \[name, state, num clients,
-#   TX queue size, RX queue size, TX bytes, RX bytes, Command count,
-#   Telemetry count] for all interfaces
-def get_all_interface_info(scope=OPENC3_SCOPE):
-    authorize(permission="system", scope=scope)
-    info = []
-    for int_name, int in InterfaceStatusModel.all(scope=scope).items():
-        info.append(
-            [
-                int["name"],
-                int["state"],
-                int["clients"],
-                int["txsize"],
-                int["rxsize"],
-                int["txbytes"],
-                int["rxbytes"],
-                int["txcnt"],
-                int["rxcnt"],
-            ]
-        )
-    #   info.sort! { |a, b| a[0] <: b[0] }
-    return info
-
-
-# Associates a target and all its commands and telemetry with a particular
-# interface. All the commands will go out over and telemetry be received
-# from that interface.
-#
-# @param target_name [String/Array] The name of the target(s)
-# @param interface_name (see #connect_interface)
-def map_target_to_interface(
-    target_name,
-    interface_name,
-    cmd_only=False,
-    tlm_only=False,
-    unmap_old=True,
-    scope=OPENC3_SCOPE,
-):
-    authorize(permission="system_set", interface_name=interface_name, scope=scope)
-    new_interface = InterfaceModel.get_model(name=interface_name, scope=scope)
-    if type(target_name) is list:
-        target_names = target_name
-    else:
-        target_names = [target_name]
-    for name in target_names:
-        new_interface.map_target(
-            name, cmd_only=cmd_only, tlm_only=tlm_only, unmap_old=unmap_old
-        )
-        Logger.info(f"Target {name} mapped to Interface {interface_name}", scope=scope)
-
-
-def interface_cmd(interface_name, cmd_name, *cmd_params, scope=OPENC3_SCOPE):
-    authorize(permission="system_set", interface_name=interface_name, scope=scope)
-    InterfaceTopic.interface_cmd(interface_name, cmd_name, *cmd_params, scope=scope)
-
-
-def interface_protocol_cmd(
-    interface_name,
-    cmd_name,
-    *cmd_params,
-    read_write="READ_WRITE",
-    index=-1,
-    scope=OPENC3_SCOPE,
-):
-    authorize(permission="system_set", interface_name=interface_name, scope=scope)
-    InterfaceTopic.protocol_cmd(
-        interface_name,
-        cmd_name,
-        *cmd_params,
-        read_write=read_write,
-        index=index,
-        scope=scope,
-    )
+# # Connects an interface and starts its telemetry gathering thread
+# #
+# # @param interface_name [String] The name of the interface
+# # @param interface_params [Array] Optional parameters to pass to the interface
+# def connect_interface(interface_name, *interface_params, scope=OPENC3_SCOPE):
+#   authorize(permission: 'system_set', interface_name: interface_name, scope: scope)
+#   InterfaceTopic.connect_interface(interface_name, *interface_params, scope: scope)
+
+
+# # Disconnects from an interface and kills its telemetry gathering thread
+# #
+# # @param interface_name [String] The name of the interface
+# def disconnect_interface(interface_name, scope=OPENC3_SCOPE):
+#   authorize(permission: 'system_set', interface_name: interface_name, scope: scope)
+#   InterfaceTopic.disconnect_interface(interface_name, scope: scope)
+
+
+# # Starts raw logging for an interface
+# #
+# # @param interface_name [String] The name of the interface
+# def start_raw_logging_interface(interface_name = 'ALL', scope=OPENC3_SCOPE):
+#   authorize(permission: 'system_set', interface_name: interface_name, scope: scope)
+#   if interface_name == 'ALL'
+#     get_interface_names().each do |interface_name|
+#       InterfaceTopic.start_raw_logging(interface_name, scope: scope)
+
+#   else
+#     InterfaceTopic.start_raw_logging(interface_name, scope: scope)
+
+
+# # Stop raw logging for an interface
+# #
+# # @param interface_name [String] The name of the interface
+# def stop_raw_logging_interface(interface_name = 'ALL', scope=OPENC3_SCOPE):
+#   authorize(permission: 'system_set', interface_name: interface_name, scope: scope)
+#   if interface_name == 'ALL'
+#     get_interface_names().each do |interface_name|
+#       InterfaceTopic.stop_raw_logging(interface_name, scope: scope)
+
+#   else
+#     InterfaceTopic.stop_raw_logging(interface_name, scope: scope)
+
+
+# # Get information about all interfaces
+# #
+# # @return [Array<Array<String, Numeric, Numeric, Numeric, Numeric, Numeric,
+# #   Numeric, Numeric>>] Array of Arrays containing \[name, state, num clients,
+# #   TX queue size, RX queue size, TX bytes, RX bytes, Command count,
+# #   Telemetry count] for all interfaces
+# def get_all_interface_info(scope=OPENC3_SCOPE):
+#   authorize(permission: 'system', scope: scope)
+#   info = []
+#   InterfaceStatusModel.all(scope: scope).each do |int_name, int|
+#     info << [int['name'], int['state'], int['clients'], int['txsize'], int['rxsize'],
+#              int['txbytes'], int['rxbytes'], int['txcnt'], int['rxcnt']]
+
+#   info.sort! { |a, b| a[0] <=> b[0] }
+#   info
+
+
+# # Associates a target and all its commands and telemetry with a particular
+# # interface. All the commands will go out over and telemetry be received
+# # from that interface.
+# #
+# # @param target_name [String/Array] The name of the target(s)
+# # @param interface_name (see #connect_interface)
+# def map_target_to_interface(target_name, interface_name, cmd_only: false, tlm_only: false, unmap_old: true, scope=OPENC3_SCOPE):
+#   authorize(permission: 'system_set', interface_name: interface_name, scope: scope)
+#   new_interface = InterfaceModel.get_model(name: interface_name, scope: scope)
+#   if Array === target_name
+#     target_names = target_name
+#   else
+#     target_names = [target_name]
+
+#   target_names.each do |name|
+#     new_interface.map_target(name, cmd_only: cmd_only, tlm_only: tlm_only, unmap_old: unmap_old)
+#     Logger.info("Target #{name} mapped to Interface #{interface_name}", scope: scope)
+
+#   nil
+
+
+# def interface_cmd(interface_name, cmd_name, *cmd_params, scope=OPENC3_SCOPE):
+#   authorize(permission: 'system_set', interface_name: interface_name, scope: scope)
+#   InterfaceTopic.interface_cmd(interface_name, cmd_name, *cmd_params, scope: scope)
+
+
+# def interface_protocol_cmd(interface_name, cmd_name, *cmd_params, read_write: :READ_WRITE, index: -1, scope=OPENC3_SCOPE):
+#   authorize(permission: 'system_set', interface_name: interface_name, scope: scope)
+#   InterfaceTopic.protocol_cmd(interface_name, cmd_name, *cmd_params, read_write: read_write, index: index, scope: scope)
```

### Comparing `openc3-5.16.0/openc3/api/stash_api.py` & `openc3-5.9.2b0/openc3/api/stash_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 OpenC3, Inc
+# Copyright 2022 OpenC3, Inc
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 #
@@ -21,38 +21,40 @@
 from openc3.models.stash_model import StashModel
 
 WHITELIST.extend(["stash_set", "stash_get", "stash_all", "stash_keys", "stash_delete"])
 
 
 def stash_set(key, value, scope=OPENC3_SCOPE):
     authorize(permission="script_run", scope=scope)
-    return StashModel.set({"name": key, "value": json.dumps(value)}, scope=scope)
+    return StashModel.set(
+        {"name": key, "value": json.dumps(value.as_json())}, scope=scope
+    )
 
 
 def stash_get(key, scope=OPENC3_SCOPE):
     authorize(permission="script_view", scope=scope)
     result = StashModel.get(name=key, scope=scope)
     if result:
         return json.loads(result["value"])
     else:
         return None
 
 
 def stash_all(scope=OPENC3_SCOPE):
     authorize(permission="script_view", scope=scope)
     all = StashModel.all(scope=scope)
-    for key, hash in all.items():
+    for key, hash in all:
         all[key] = json.loads(hash["value"])
     return all
 
 
 def stash_keys(scope=OPENC3_SCOPE):
     authorize(permission="script_view", scope=scope)
     return StashModel.names(scope=scope)
 
 
 def stash_delete(key, scope=OPENC3_SCOPE):
     authorize(permission="script_run", scope=scope)
     model = StashModel.get_model(name=key, scope=scope)
     if model:
-        model.destroy()
+        model.destroy
     return model
```

### Comparing `openc3-5.16.0/openc3/api/tlm_api.py` & `openc3-5.9.2b0/openc3/api/tlm_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -10,49 +12,42 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-import json
 from openc3.api import WHITELIST
 from openc3.environment import OPENC3_SCOPE
 from openc3.utilities.authorization import authorize
 from openc3.topics.topic import Topic
 from openc3.topics.interface_topic import InterfaceTopic
 from openc3.topics.decom_interface_topic import DecomInterfaceTopic
 from openc3.models.cvt_model import CvtModel
 from openc3.models.target_model import TargetModel
 from openc3.models.interface_model import InterfaceModel
 from openc3.utilities.extract import *
 
 WHITELIST.extend(
     [
         "tlm",
-        "tlm_raw",
-        "tlm_formatted",
-        "tlm_with_units",
         "set_tlm",
         "inject_tlm",
         "override_tlm",
         "get_overrides",
         "normalize_tlm",
         "get_tlm_buffer",
         "get_tlm_packet",
         "get_tlm_values",
-        "get_all_tlm",
-        "get_all_telemetry",  # DEPRECATED
-        "get_all_tlm_names",
-        "get_all_telemetry_names",  # DEPRECATED
-        "get_tlm",
-        "get_telemetry",  # DEPRECATED
+        "get_all_telemetry",
+        "get_all_telemetry_names",
+        "get_telemetry",
         "get_item",
-        "subscribe_packets",
-        "get_packets",
+        # 'subscribe_packets',
+        # 'get_packets',
         "get_tlm_cnt",
         "get_tlm_cnts",
         "get_packet_derived_items",
     ]
 )
 
 
@@ -63,36 +58,20 @@
 #   tlm('TGT','PKT','ITEM')
 #
 # Favor the first syntax where possible as it is more succinct.
 #
 # @param args [String|Array<String>] See the description for calling style
 # @param type [Symbol] Telemetry type, :RAW, :CONVERTED (default), :FORMATTED, or :WITH_UNITS
 # @return [Object] The telemetry value formatted as requested
-def tlm(*args, type="CONVERTED", cache_timeout=0.1, scope=OPENC3_SCOPE):
-    target_name, packet_name, item_name = _tlm_process_args(
-        args, "tlm", cache_timeout=cache_timeout, scope=scope
-    )
+def tlm(*args, type="CONVERTED", scope=OPENC3_SCOPE):
+    target_name, packet_name, item_name = _tlm_process_args(args, "tlm", scope=scope)
     authorize(
         permission="tlm", target_name=target_name, packet_name=packet_name, scope=scope
     )
-    return CvtModel.get_item(
-        target_name, packet_name, item_name, type, cache_timeout, scope
-    )
-
-
-def tlm_raw(*args, cache_timeout=0.1, scope=OPENC3_SCOPE):
-    return tlm(*args, type="RAW", cache_timeout=cache_timeout, scope=scope)
-
-
-def tlm_formatted(*args, cache_timeout=0.1, scope=OPENC3_SCOPE):
-    return tlm(*args, type="FORMATTED", cache_timeout=cache_timeout, scope=scope)
-
-
-def tlm_with_units(*args, cache_timeout=0.1, scope=OPENC3_SCOPE):
-    return tlm(*args, type="WITH_UNITS", cache_timeout=cache_timeout, scope=scope)
+    return CvtModel.get_item(target_name, packet_name, item_name, type, scope)
 
 
 # Set a telemetry item in the current value table.
 #
 # Note: If this is done while OpenC3 is currently receiving telemetry,
 # this value could get overwritten at any time. Thus this capability is
 # best used for testing or for telemetry items that are not received
@@ -104,23 +83,25 @@
 #
 # Favor the first syntax where possible as it is more succinct.
 #
 # @param args [String|Array<String>] See the description for calling style
 # @param type [Symbol] Telemetry type, :RAW, :CONVERTED (default), :FORMATTED, or :WITH_UNITS
 def set_tlm(*args, type="CONVERTED", scope=OPENC3_SCOPE):
     target_name, packet_name, item_name, value = _set_tlm_process_args(
-        args, "set_tlm", scope
+        args, "set_tlm", scope=scope
     )
     authorize(
         permission="tlm_set",
         target_name=target_name,
         packet_name=packet_name,
         scope=scope,
     )
-    CvtModel.set_item(target_name, packet_name, item_name, value, type, scope)
+    CvtModel.set_item(
+        target_name, packet_name, item_name, value, type=type, scope=scope
+    )
 
 
 # Injects a packet into the system as if it was received from an interface
 #
 # @param target_name [String] Target name of the packet
 # @param packet_name [String] Packet name of the packet
 # @param item_hash [Hash] Hash of item_name and value for each item you want to change from the current value table
@@ -138,24 +119,22 @@
     packet_name = packet_name.upper()
     if type not in CvtModel.VALUE_TYPES:
         raise RuntimeError(f"Unknown type '{type}' for {target_name} {packet_name}")
 
     if item_hash:
         item_hash = {k.upper(): v for k, v in item_hash.items()}
         # Check that the items exist ... exceptions are raised if not
-        TargetModel.packet_items(
-            target_name, packet_name, item_hash.keys(), scope=scope
-        )
+        TargetModel.packet_items(target_name, packet_name, item_hash.keys, scope=scope)
     else:
         # Check that the packet exists ... exceptions are raised if not
         TargetModel.packet(target_name, packet_name, scope=scope)
 
     # See if this target has a tlm interface
     interface_name = None
-    for _, interface in InterfaceModel.all(scope).items():
+    for _, interface in InterfaceModel.all(scope):
         if target_name in interface["tlm_target_names"]:
             interface_name = interface["name"]
             break
 
     # Use an interface microservice if it exists, other use the decom microservice
     if interface_name:
         InterfaceTopic.inject_tlm(
@@ -179,15 +158,15 @@
 #
 # @param args The args must either be a string followed by a value or
 #   three strings followed by a value (see the calling style in the
 #   description).
 # @param type [Symbol] Telemetry type, :ALL (default), :RAW, :CONVERTED, :FORMATTED, :WITH_UNITS
 def override_tlm(*args, type="ALL", scope=OPENC3_SCOPE):
     target_name, packet_name, item_name, value = _set_tlm_process_args(
-        args, "override_tlm", scope
+        args, "override_tlm", scope=scope
     )
     authorize(
         permission="tlm_set",
         target_name=target_name,
         packet_name=packet_name,
         scope=scope,
     )
@@ -195,15 +174,15 @@
         target_name, packet_name, item_name, value, type=type, scope=scope
     )
 
 
 # Get the list of CVT overrides
 def get_overrides(scope=OPENC3_SCOPE):
     authorize(permission="tlm", scope=scope)
-    return CvtModel.overrides(scope=scope)
+    CvtModel.overrides(scope=scope)
 
 
 # Normalize a telemetry item in a packet to its default behavior. Called
 # after override_tlm to restore standard processing.
 #
 # Accepts two different calling styles:
 #   normalize_tlm("TGT PKT ITEM")
@@ -229,244 +208,206 @@
 
 
 # Returns the raw buffer for a telemetry packet.
 #
 # @param target_name [String] Name of the target
 # @param packet_name [String] Name of the packet
 # @return [Hash] telemetry hash with last telemetry buffer
-def get_tlm_buffer(*args, scope=OPENC3_SCOPE):
-    target_name, packet_name = _extract_target_packet_names("get_tlm_buffer", *args)
+def get_tlm_buffer(target_name, packet_name, scope=OPENC3_SCOPE):
+    target_name = target_name.upper()
+    packet_name = packet_name.upper()
     authorize(
         permission="tlm", target_name=target_name, packet_name=packet_name, scope=scope
     )
     TargetModel.packet(target_name, packet_name, scope=scope)
     topic = f"{scope}__TELEMETRY__{{{target_name}}}__{packet_name}"
     msg_id, msg_hash = Topic.get_newest_message(topic)
     if msg_id:
-        # Decode the keys for user convenience
-        return {k.decode(): v for (k, v) in msg_hash.items()}
+        # TODO: Python equivalent of .b
+        # msg_hash['buffer'] = msg_hash['buffer'].b
+        return msg_hash
     return None
 
 
 # Returns all the values (along with their limits state) for a packet.
 #
 # @param target_name [String] Name of the target
 # @param packet_name [String] Name of the packet
 # @param stale_time [Integer] Time in seconds from Time.now that packet will be marked stale
 # @param type [Symbol] Types returned, :RAW, :CONVERTED (default), :FORMATTED, or :WITH_UNITS
 # @return [Array<String, Object, Symbol|None>] Returns an Array consisting
 #   of [item name, item value, item limits state] where the item limits
 #   state can be one of {OpenC3::Limits::LIMITS_STATES}
-def get_tlm_packet(*args, stale_time=30, type="CONVERTED", scope=OPENC3_SCOPE):
-    target_name, packet_name = _extract_target_packet_names("get_tlm_packet", *args)
+def get_tlm_packet(
+    self, target_name, packet_name, stale_time=30, type="CONVERTED", scope=OPENC3_SCOPE
+):
+    target_name = target_name.upper()
+    packet_name = packet_name.upper()
     authorize(
         permission="tlm", target_name=target_name, packet_name=packet_name, scope=scope
     )
     packet = TargetModel.packet(target_name, packet_name, scope=scope)
     t = _validate_tlm_type(type)
-    if t is None:
+    if not t:
         raise AttributeError(f"Unknown type '{type}' for {target_name} {packet_name}")
-    cvt_items = [
-        [target_name, packet_name, item["name"].upper(), type]
-        for item in packet["items"]
-    ]
-    # This returns an array of arrays containin the value and the limits state:
-    # [[0, None], [0, 'RED_LOW'], ... ]
+    items = {item["name"].upper() for item in packet["items"]}
+    cvt_items = {f"{target_name}__{packet_name}__{item}__{type}" for item in items}
     current_values = CvtModel.get_tlm_values(
         cvt_items, stale_time=stale_time, scope=scope
     )
-    result = []
-    # Combine the values with the item name
-    for index, item in enumerate(current_values):
-        result.append([cvt_items[index][2], item[0], item[1]])
-    return result
+    return {[item, values[0], values[1]] for item, values in current_values}
 
 
 # Returns all the item values (along with their limits state). The items
 # can be from any target and packet and thus must be fully qualified with
 # their target and packet names.
 #
 # @param items [Array<String>] Array of items consisting of 'tgt__pkt__item__type'
 # @param stale_time [Integer] Time in seconds from Time.now that data will be marked stale
 # @return [Array<Object, Symbol>]
 #   Array consisting of the item value and limits state
 #   given as symbols such as :RED, :YELLOW, :STALE
-def get_tlm_values(items, stale_time=30, cache_timeout=0.1, scope=OPENC3_SCOPE):
-    if type(items) != list or len(items) == 0 or type(items[0]) != str:
+def get_tlm_values(items, stale_time=30, scope=OPENC3_SCOPE):
+    if type(items) != list or type(items[0]) != str:
         raise AttributeError(
             "items must be array of strings: ['TGT__PKT__ITEM__TYPE', ...]"
         )
-    packets = []
-    cvt_items = []
-    for item in items:
-        try:
-            target_name, packet_name, item_name, value_type = item.upper().split("__")
-        except ValueError:
+    for index, item in enumerate(items):
+        target_name, packet_name, item_name, value_type = item.split("__")
+        if not target_name or not packet_name or not item_name or not value_type:
             raise AttributeError("items must be formatted as TGT__PKT__ITEM__TYPE")
+        target_name = target_name.upper()
+        packet_name = packet_name.upper()
+        item_name = item_name.upper()
+        value_type = value_type.upper()
         if packet_name == "LATEST":
-            packet_name = CvtModel.determine_latest_packet_for_item(
-                target_name, item_name, cache_timeout, scope
-            )
+            _, packet_name, _ = _tlm_process_args(
+                [target_name, packet_name, item_name], "get_tlm_values", scope=scope
+            )  # Figure out which packet is LATEST
         # Change packet_name in case of LATEST and ensure upcase
-        cvt_items.append([target_name, packet_name, item_name, value_type])
-        packets.append([target_name, packet_name])
-    # Make the array of arrays unique
-    packets = [list(x) for x in set(tuple(x) for x in packets)]
-    for name in packets:
+        items[index] = f"{target_name}__{packet_name}__{item_name}__{value_type}"
         authorize(
             permission="tlm",
-            target_name=name[0],
-            packet_name=name[1],
+            target_name=target_name,
+            packet_name=packet_name,
             scope=scope,
         )
-    return CvtModel.get_tlm_values(cvt_items, stale_time, cache_timeout, scope)
+    return CvtModel.get_tlm_values(items, stale_time=stale_time, scope=scope)
 
 
 # Returns an array of all the telemetry packet hashes
 #
 # @param target_name [String] Name of the target
 # @return [Array<Hash>] Array of all telemetry packet hashes
-def get_all_tlm(target_name, scope=OPENC3_SCOPE):
+def get_all_telemetry(target_name, scope=OPENC3_SCOPE):
     target_name = target_name.upper()
     authorize(permission="tlm", target_name=target_name, scope=scope)
     return TargetModel.packets(target_name, type="TLM", scope=scope)
 
 
-# get_all_telemetry is DEPRECATED
-get_all_telemetry = get_all_tlm
-
-
 # Returns an array of all the telemetry packet names
 #
 # @param target_name [String] Name of the target
 # @return [Array<String>] Array of all telemetry packet names
-def get_all_tlm_names(target_name, hidden=False, scope=OPENC3_SCOPE):
-    try:
-        packets = get_all_tlm(target_name, scope=scope)
-    except RuntimeError:
-        packets = []
-    names = []
-    for packet in packets:
-        if hidden:
-            names.append(packet["packet_name"])
-        else:
-            if "hidden" not in packet:
-                names.append(packet["packet_name"])
-    return names
-
-
-# get_all_telemetry_names is DEPRECATED
-get_all_telemetry_names = get_all_tlm_names
+def get_all_telemetry_names(target_name, scope=OPENC3_SCOPE):
+    target_name = target_name.upper()
+    authorize(permission="cmd_info", target_name=target_name, scope=scope)
+    return TargetModel.packet_names(target_name, type="TLM", scope=scope)
 
 
 # Returns a telemetry packet hash
 #
 # @param target_name [String] Name of the target
 # @param packet_name [String] Name of the packet
 # @return [Hash] Telemetry packet hash
-def get_tlm(*args, scope=OPENC3_SCOPE):
-    target_name, packet_name = _extract_target_packet_names("get_tlm", *args)
+def get_telemetry(target_name, packet_name, scope=OPENC3_SCOPE):
+    target_name = target_name.upper()
+    packet_name = packet_name.upper()
     authorize(
         permission="tlm", target_name=target_name, packet_name=packet_name, scope=scope
     )
     return TargetModel.packet(target_name, packet_name, scope=scope)
 
 
-# get_telemetry is DEPRECATED
-get_telemetry = get_tlm
-
-
 # Returns a telemetry packet item hash
 #
 # @param target_name [String] Name of the target
 # @param packet_name [String] Name of the packet
 # @param item_name [String] Name of the packet
 # @return [Hash] Telemetry packet item hash
-def get_item(*args, scope=OPENC3_SCOPE):
-    target_name, packet_name, item_name = _extract_target_packet_item_names(
-        "get_item", *args
-    )
+def get_item(target_name, packet_name, item_name, scope=OPENC3_SCOPE):
+    target_name = target_name.upper()
+    packet_name = packet_name.upper()
+    item_name = item_name.upper()
     authorize(
         permission="tlm", target_name=target_name, packet_name=packet_name, scope=scope
     )
     return TargetModel.packet_item(target_name, packet_name, item_name, scope=scope)
 
 
-# 2x double underscore since __ is reserved
-SUBSCRIPTION_DELIMITER = "____"
-
-
-# Subscribe to a list of packets. An ID is returned which is passed to
-# get_packets(id) to return packets.
-#
-# @param packets [Array<Array<String, String>>] Array of arrays consisting of target name, packet name
-# @return [String] ID which should be passed to get_packets
-def subscribe_packets(packets, scope=OPENC3_SCOPE):
-    if type(packets) is not list or type(packets[0]) is not list:
-        raise RuntimeError("packets must be nested array: [['TGT','PKT'],...]")
-
-    result = {}
-    for target_name, packet_name in packets:
-        target_name = target_name.upper()
-        packet_name = packet_name.upper()
-        authorize(
-            permission="tlm",
-            target_name=target_name,
-            packet_name=packet_name,
-            scope=scope,
-        )
-        topic = f"{scope}__DECOM__{{{target_name}}}__{packet_name}"
-        id, _ = Topic.get_newest_message(topic)
+# # 2x double underscore since __ is reserved
+# SUBSCRIPTION_DELIMITER = '____'
 
-        if id:
-            result[topic] = id
-        else:
-            result[topic] = "0-0"
-    mylist = []
-    for k, v in result.items():
-        mylist += [k, v]
-    return SUBSCRIPTION_DELIMITER.join(mylist)
-
-
-# Get packets based on ID returned from subscribe_packet.
-# @param id [String] ID returned from subscribe_packets or last call to get_packets
-# @param count [Integer] Maximum number of packets to return from EACH packet stream
-# @return [Array<String, Array<Hash>] Array of the ID and array of all packets found
-def get_packets(id, count=1000, scope=OPENC3_SCOPE):
-    authorize(permission="tlm", scope=scope)
-    # Split the list of topic, ID values and turn it into a hash for easy updates
-    items = id.split(SUBSCRIPTION_DELIMITER)
-    # Convert it back into a dict to create a lookup
-    lookup = dict(zip(items[::2], items[1::2]))
-    packets = []
-    for topic, _, msg_hash, _ in Topic.read_topics(
-        lookup.keys(), list(lookup.values()), None, count
-    ):
-        # # Return the original ID and and empty array if we didn't get anything
-        # for topic, data in xread:
-        # for id, msg_hash in data:
-        lookup[topic] = id  # save the new ID
-        # decode the binary string keys and values to strings
-        msg_hash = {k.decode(): v.decode() for (k, v) in msg_hash.items()}
-        json_hash = json.loads(msg_hash["json_data"])
-        msg_hash.pop("json_data")
-        packets.append(msg_hash | json_hash)
-    mylist = []
-    for k, v in lookup.items():
-        mylist += [k, v]
-    return (SUBSCRIPTION_DELIMITER.join(mylist), packets)
+# # Subscribe to a list of packets. An ID is returned which is passed to
+# # get_packets(id) to return packets.
+# #
+# # @param packets [Array<Array<String, String>>] Array of arrays consisting of target name, packet name
+# # @return [String] ID which should be passed to get_packets
+# def subscribe_packets(packets, scope=OPENC3_SCOPE)
+#   if !packets.is_a?(Array) || !packets[0].is_a?(Array)
+#     raise ArgumentError, "packets must be nested array: [['TGT','PKT'],...]"
+#   end
+
+#   result = {}
+#   packets.each do |target_name, packet_name|
+#     target_name = target_name.upper()
+#     packet_name = packet_name.upper()
+#     authorize(permission='tlm', target_name= target_name, packet_name= packet_name, scope=scope)
+#     topic = "#{scope}__DECOM__{#{target_name}}__#{packet_name}"
+#     id, _ = Topic.get_newest_message(topic)
+#     result[topic] = id ? id : '0-0'
+#   end
+#   result.to_a.join(SUBSCRIPTION_DELIMITER)
+# end
+# # Alias the singular as well since that matches COSMOS 4
+# alias subscribe_packet subscribe_packets
+
+# # Get packets based on ID returned from subscribe_packet.
+# # @param id [String] ID returned from subscribe_packets or last call to get_packets
+# # @param block [Integer] Unused - Blocking must be implemented at the client
+# # @param count [Integer] Maximum number of packets to return from EACH packet stream
+# # @return [Array<String, Array<Hash>] Array of the ID and array of all packets found
+# def get_packets(id, block: None, count: 1000, scope=OPENC3_SCOPE)
+#   authorize(permission='tlm', scope=scope)
+#   # Split the list of topic, ID values and turn it into a hash for easy updates
+#   lookup = Hash[*id.split(SUBSCRIPTION_DELIMITER)]
+#   xread = Topic.read_topics(lookup.keys, lookup.values, None, count) # Always don't block
+#   # Return the original ID and and empty array if we didn't get anything
+#   packets = []
+#   return [id, packets] if xread.empty?
+#   xread.each do |topic, data|
+#     data.each do |id, msg_hash|
+#       lookup[topic] = id # save the new ID
+#       json_hash = JSON.parse(msg_hash['json_data'], :allow_nan => true, :create_additions => true)
+#       msg_hash.delete('json_data')
+#       packets << msg_hash.merge(json_hash)
+#     end
+#   end
+#   return lookup.to_a.join(SUBSCRIPTION_DELIMITER), packets
+# end
 
 
 # Get the receive count for a telemetry packet
 #
 # @param target_name [String] Name of the target
 # @param packet_name [String] Name of the packet
 # @return [Numeric] Receive count for the telemetry packet
-def get_tlm_cnt(*args, scope=OPENC3_SCOPE):
-    target_name, packet_name = _extract_target_packet_names("get_tlm_cnt", *args)
+def get_tlm_cnt(target_name, packet_name, scope=OPENC3_SCOPE):
+    target_name = target_name.upper()
+    packet_name = packet_name.upper()
     authorize(
         permission="system",
         target_name=target_name,
         packet_name=packet_name,
         scope=scope,
     )
     TargetModel.packet(target_name, packet_name, scope=scope)
@@ -479,103 +420,47 @@
 # @return [Numeric] Transmit count for the command
 def get_tlm_cnts(target_packets, scope=OPENC3_SCOPE):
     authorize(permission="system", scope=scope)
     counts = []
     for target_name, packet_name in target_packets:
         target_name = target_name.upper()
         packet_name = packet_name.upper()
-        counts.append(
-            Topic.get_cnt(f"{scope}__TELEMETRY__{{{target_name}}}__{packet_name}")
-        )
+        counts << Topic.get_cnt(f"{scope}__TELEMETRY__{{{target_name}}}__{packet_name}")
     return counts
 
 
 # Get the list of derived telemetry items for a packet
 #
 # @param target_name [String] Target name
 # @param packet_name [String] Packet name
 # @return [Array<String>] All of the ignored telemetry items for a packet.
-def get_packet_derived_items(*args, scope=OPENC3_SCOPE):
-    target_name, packet_name = _extract_target_packet_names(
-        "get_packet_derived_items", *args
-    )
+def get_packet_derived_items(target_name, packet_name, scope=OPENC3_SCOPE):
+    target_name = target_name.upper()
+    packet_name = packet_name.upper()
     authorize(
         permission="tlm", target_name=target_name, packet_name=packet_name, scope=scope
     )
     packet = TargetModel.packet(target_name, packet_name, scope=scope)
     return [item["name"] for item in packet["items"] if item["data_type"] == "DERIVED"]
 
 
-def _extract_target_packet_names(method_name, *args):
-    target_name = None
-    packet_name = None
-    match len(args):
-        case 1:
-            try:
-                target_name, packet_name = args[0].upper().split()
-            except ValueError:
-                # We get ValueError if passing not enough parameters
-                # The check below for None handles this case
-                pass
-        case 2:
-            target_name = args[0].upper()
-            packet_name = args[1].upper()
-        case _:
-            # Invalid number of arguments
-            raise RuntimeError(
-                f"ERROR: Invalid number of arguments ({len(args)}) passed to {method_name}()"
-            )
-    if target_name is None or packet_name is None:
-        raise RuntimeError(
-            f'ERROR: Both target name and packet name required. Usage: {method_name}("TGT PKT") or {method_name}("TGT", "PKT")'
-        )
-    return (target_name, packet_name)
-
-
-def _extract_target_packet_item_names(method_name, *args):
-    target_name = None
-    packet_name = None
-    item_name = None
-    match len(args):
-        case 1:
-            try:
-                target_name, packet_name, item_name = args[0].upper().split()
-            except ValueError:  # Thrown when not enough items given
-                # Do nothing because below error will catch this
-                pass
-        case 3:
-            target_name = args[0].upper()
-            packet_name = args[1].upper()
-            item_name = args[2].upper()
-        case _:
-            # Invalid number of arguments
-            raise RuntimeError(
-                f"ERROR: Invalid number of arguments ({len(args)}) passed to {method_name}()"
-            )
-    if target_name is None or packet_name is None or item_name is None:
-        raise RuntimeError(
-            f'ERROR: Target name, packet name and item name required. Usage: {method_name}("TGT PKT ITEM") or {method_name}("TGT", "PKT", "ITEM")'
-        )
-    return (target_name, packet_name, item_name)
-
-
 def _validate_tlm_type(type):
     match type:
         case "RAW":
             return ""
         case "CONVERTED":
             return "C"
         case "FORMATTED":
             return "F"
         case "WITH_UNITS":
             return "U"
     return None
 
 
-def _tlm_process_args(args, method_name, cache_timeout=0.1, scope=OPENC3_SCOPE):
+def _tlm_process_args(args, method_name, scope=OPENC3_SCOPE):
     match (len(args)):
         case 1:
             target_name, packet_name, item_name = extract_fields_from_tlm_text(args[0])
         case 3:
             target_name = args[0]
             packet_name = args[1]
             item_name = args[2]
@@ -584,21 +469,35 @@
             raise RuntimeError(
                 f"ERROR: Invalid number of arguments ({len(args)}) passed to {method_name}()"
             )
     target_name = target_name.upper()
     packet_name = packet_name.upper()
     item_name = item_name.upper()
     if packet_name == "LATEST":
-        packet_name = CvtModel.determine_latest_packet_for_item(
-            target_name, item_name, cache_timeout, scope
-        )
+        latest = -1
+        for packet in TargetModel.packets(target_name, scope=scope):
+            found = None
+            for item in packet["items"]:
+                if item["name"] == item_name:
+                    found = item
+                    break
+            if found:
+                hash = CvtModel.get(target_name, packet["packet_name"], scope)
+                if hash["PACKET_TIMESECONDS"] and hash["PACKET_TIMESECONDS"] > latest:
+                    latest = hash["PACKET_TIMESECONDS"]
+                    packet_name = packet["packet_name"]
+        if latest == -1:
+            raise RuntimeError(
+                f"Item '{target_name} LATEST {item_name}' does not exist"
+            )
     else:
+        pass
         # Determine if this item exists, it will raise appropriate errors if not
         TargetModel.packet_item(target_name, packet_name, item_name, scope=scope)
-    return target_name, packet_name, item_name
+    return [target_name, packet_name, item_name]
 
 
 def _set_tlm_process_args(args, method_name, scope=OPENC3_SCOPE):
     match len(args):
         case 1:
             (
                 target_name,
@@ -618,8 +517,8 @@
             )
     target_name = target_name.upper()
     packet_name = packet_name.upper()
     item_name = item_name.upper()
     # Determine if this item exists, it will raise appropriate errors if not
     TargetModel.packet_item(target_name, packet_name, item_name, scope=scope)
 
-    return target_name, packet_name, item_name, value
+    return [target_name, packet_name, item_name, value]
```

### Comparing `openc3-5.16.0/openc3/conversions/packet_time_formatted_conversion.py` & `openc3-5.9.2b0/openc3/io/stderr.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
-# attribution addums as found in the LICENSE.txt
+# attribution addendums as found in the LICENSE.txt
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
-
+#
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
+from openc3.io.io_multiplexer import IoMultiplexer
 
-from openc3.conversions.conversion import Conversion
-from openc3.utilities.time import formatted
-
+# Adds STDOUT to the multiplexed streams
+class Stderr(IoMultiplexer):
+    my_instance = None
 
-# Converts the packet received time object into a formatted string.
-class PacketTimeFormattedConversion(Conversion):
-    # Initializes converted_type to 'STRING' and converted_bit_size to 0
     def __init__(self):
         super().__init__()
-        self.converted_type = "STRING"
-        self.converted_bit_size = 0
+        self.streams.append(self.STDERR)
+        Stderr.my_instance = self
 
-    # self.param (see Conversion#call)
-    # self.return [String] Formatted packet time
-    def call(self, value, packet, buffer):
-        packet_time = packet.packet_time
-        if packet_time:
-            return formatted(packet_time)
-        else:
-            return "No Packet Time"
+    # @return [Stdout] Returns a single instance of Stdout
+    @classmethod
+    def instance(cls):
+        if not cls.my_instance:
+            cls()
+        return cls.my_instance
```

### Comparing `openc3-5.16.0/openc3/conversions/received_count_conversion.py` & `openc3-5.9.2b0/openc3/io/stdout.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-# Copyright 2023 OpenC3, Inc.
+# Copyright 2023, OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
-# attribution addums as found in the LICENSE.txt
+# attribution addendums as found in the LICENSE.txt
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
-
+#
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
+from openc3.io.io_multiplexer import IoMultiplexer
 
-from openc3.conversions.conversion import Conversion
-
+# Adds STDOUT to the multiplexed streams
+class Stdout(IoMultiplexer):
+    my_instance = None
 
-# Converts the packet received count as a derived telemetry item
-class ReceivedCountConversion(Conversion):
-    # Initializes converted_type to 'UINT' and converted_bit_size to 32
     def __init__(self):
         super().__init__()
-        self.converted_type = "UINT"
-        self.converted_bit_size = 32
+        self.streams.append(self.STDOUT)
+        Stdout.my_instance = self
 
-    # self.param (see Conversion#call)
-    # self.return [Integer] packet.received_count
-    def call(self, value, packet, buffer):
-        return packet.received_count
+    # @return [Stdout] Returns a single instance of Stdout
+    @classmethod
+    def instance(cls):
+        if not cls.my_instance:
+            cls()
+        return cls.my_instance
```

### Comparing `openc3-5.16.0/openc3/conversions/received_time_seconds_conversion.py` & `openc3-5.9.2b0/test/test_helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,42 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
-# attribution addums as found in the LICENSE.txt
+# attribution addendums as found in the LICENSE.txt
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-
-from openc3.conversions.conversion import Conversion
-
-
-# Converts the packet received time into floating point seconds.
-class ReceivedTimeSecondsConversion(Conversion):
-    # Initializes converted_type to 'FLOAT' and converted_bit_size to 64
-    def __init__(self):
-        super().__init__()
-        self.converted_type = "FLOAT"
-        self.converted_bit_size = 64
-
-    # self.param (see Conversion#call)
-    # self.return [Float] Packet received time in seconds
-    def call(self, value, packet, buffer):
-        if packet.received_time is not None:
-            return packet.received_time.timestamp()
-        else:
-            return 0.0
+import io
+import sys
+import fakeredis
+from unittest.mock import *
+from openc3.utilities.logger import Logger
+
+
+def mock_redis(self):
+    redis = fakeredis.FakeRedis(server=fakeredis.FakeServer(), version=7)
+    patcher = patch("redis.Redis", return_value=redis)
+    self.mock_redis = patcher.start()
+    self.addCleanup(patcher.stop)
+    return redis
+
+
+def capture_io():
+    stdout = sys.stdout
+    capturedOutput = io.StringIO()  # Create StringIO object
+    sys.stdout = capturedOutput  #  and redirect stdout.
+    Logger.stdout = True
+    Logger.level = Logger.INFO
+    yield capturedOutput
+    Logger.level = Logger.FATAL
+    sys.stdout = stdout
```

### Comparing `openc3-5.16.0/openc3/environment.py` & `openc3-5.9.2b0/openc3/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,27 +35,25 @@
 _openc3_redis_port = "OPENC3_REDIS_PORT"
 _openc3_redis_username = "OPENC3_REDIS_USERNAME"
 _openc3_redis_password = "OPENC3_REDIS_PASSWORD"
 _openc3_redis_ephemeral_hostname = "OPENC3_REDIS_EPHEMERAL_HOSTNAME"
 _openc3_redis_ephemeral_port = "OPENC3_REDIS_EPHEMERAL_PORT"
 _openc3_cloud = "OPENC3_CLOUD"
 _aws_region = "AWS_REGION"
-_openc3_aws_arn_prefix = "OPENC3_AWS_ARN_PREFIX"
 _openc3_bucket_url = "OPENC3_BUCKET_URL"
 _openc3_bucket_username = "OPENC3_BUCKET_USERNAME"
 _openc3_bucket_password = "OPENC3_BUCKET_PASSWORD"
+_openc3_service_password = "OPENC3_SERVICE_PASSWORD"
 _openc3_devel = "OPENC3_DEVEL"
 _openc3_full_backtrace = "OPENC3_FULL_BACKTRACE"
 _openc3_config_bucket = "OPENC3_CONFIG_BUCKET"
 _openc3_logs_bucket = "OPENC3_LOGS_BUCKET"
 _openc3_tools_bucket = "OPENC3_TOOLS_BUCKET"
 _openc3_local_mode = "OPENC3_LOCAL_MODE"
 _openc3_local_mode_path = "OPENC3_LOCAL_MODE_PATH"
-_openc3_no_bucket_policy = "OPENC3_NO_BUCKET_POLICY"
-_openc3_log_stderr = "OPENC3_LOG_STDERR"
 
 # The following variables are only used with Enterprise Edition
 _openc3_api_user = "OPENC3_API_USER"
 _openc3_api_client = "OPENC3_API_CLIENT"
 _openc3_api_token = "OPENC3_API_TOKEN"
 _openc3_keycloak_realm = "OPENC3_KEYCLOAK_REALM"
 _openc3_keycloak_url = "OPENC3_KEYCLOAK_URL"
@@ -81,43 +79,41 @@
 except TypeError:
     OPENC3_SCRIPT_API_PORT = 2902
 try:
     OPENC3_SCRIPT_API_TIMEOUT = float(os.environ.get(_openc3_script_api_timeout))
 except TypeError:
     OPENC3_SCRIPT_API_TIMEOUT = 5.0
 
-OPENC3_REDIS_HOSTNAME = os.environ.get(_openc3_redis_hostname, "openc3-redis")
+OPENC3_REDIS_HOSTNAME = os.environ.get(_openc3_redis_hostname, "127.0.0.1")
 try:
     OPENC3_REDIS_PORT = int(os.environ.get(_openc3_redis_port))
 except TypeError:
     OPENC3_REDIS_PORT = 6379
 OPENC3_REDIS_USERNAME = os.environ.get(_openc3_redis_username)
 OPENC3_REDIS_PASSWORD = os.environ.get(_openc3_redis_password)
 OPENC3_REDIS_EPHEMERAL_HOSTNAME = os.environ.get(
-    _openc3_redis_ephemeral_hostname, "openc3-redis-ephemeral"
+    _openc3_redis_ephemeral_hostname, "127.0.0.1"
 )
 try:
     OPENC3_REDIS_EPHEMERAL_PORT = int(os.environ.get(_openc3_redis_ephemeral_port))
 except TypeError:
-    OPENC3_REDIS_EPHEMERAL_PORT = 6380
-OPENC3_CLOUD = os.environ.get(_openc3_cloud, "local")
+    OPENC3_REDIS_EPHEMERAL_PORT = 6379
+OPENC3_CLOUD = os.environ.get(_openc3_cloud)
 AWS_REGION = os.environ.get(_aws_region)
-OPENC3_AWS_ARN_PREFIX = os.environ.get(_openc3_aws_arn_prefix, "arn:aws")
 OPENC3_BUCKET_URL = os.environ.get(_openc3_bucket_url)
 OPENC3_BUCKET_USERNAME = os.environ.get(_openc3_bucket_username)
 OPENC3_BUCKET_PASSWORD = os.environ.get(_openc3_bucket_password)
+OPENC3_SERVICE_PASSWORD = os.environ.get(_openc3_service_password)
 OPENC3_DEVEL = os.environ.get(_openc3_devel)
 OPENC3_FULL_BACKTRACE = os.environ.get(_openc3_full_backtrace)
 OPENC3_CONFIG_BUCKET = os.environ.get(_openc3_config_bucket)
 OPENC3_LOGS_BUCKET = os.environ.get(_openc3_logs_bucket)
 OPENC3_TOOLS_BUCKET = os.environ.get(_openc3_tools_bucket)
 OPENC3_LOCAL_MODE = os.environ.get(_openc3_local_mode)
 OPENC3_LOCAL_MODE_PATH = os.environ.get(_openc3_local_mode_path)
-OPENC3_NO_BUCKET_POLICY = os.environ.get(_openc3_no_bucket_policy)
-OPENC3_LOG_STDERR = os.environ.get(_openc3_log_stderr)
 
 OPENC3_SCOPE = os.environ.get(_openc3_scope, "DEFAULT")
 OPENC3_API_PASSWORD = os.environ.get(_openc3_api_password)
 OPENC3_LOG_LEVEL = os.environ.get(_openc3_log_level, "INFO")
 OPENC3_NO_STORE = os.environ.get(_openc3_no_store)
 OPENC3_API_USER = os.environ.get(_openc3_api_user)
 OPENC3_API_CLIENT = os.environ.get(_openc3_api_client, "api")
```

### Comparing `openc3-5.16.0/openc3/io/io_multiplexer.py` & `openc3-5.9.2b0/openc3/io/io_multiplexer.py`

 * *Files identical despite different names*

### Comparing `openc3-5.16.0/openc3/io/json_api_object.py` & `openc3-5.9.2b0/openc3/io/json_api_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -61,15 +63,15 @@
             self.authentication = self.generate_auth()
         self.timeout = timeout
         self.shutdown = False
 
     # generate the auth object
     def generate_auth(self):
         if OPENC3_API_TOKEN is None and OPENC3_API_USER is None:
-            if OPENC3_API_PASSWORD:
+            if OPENC3_API_PASSWORD or OPENC3_SERVICE_PASSWORD:
                 return OpenC3Authentication()
             else:
                 return None
         else:
             return OpenC3KeycloakAuthentication(OPENC3_KEYCLOAK_URL)
 
     # Forwards all method calls to the remote service.
```

### Comparing `openc3-5.16.0/openc3/io/json_drb_object.py` & `openc3-5.9.2b0/openc3/io/json_drb_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Copyright 2024 OpenC3, Inc.
+#!/usr/bin/env python3
+
+# Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 #
@@ -18,15 +20,15 @@
 from openc3.io.json_api_object import JsonApiObject, JsonApiError
 from .json_rpc import (
     JsonRpcRequest,
     JsonRpcResponse,
     JsonRpcSuccessResponse,
     JsonRpcErrorResponse,
 )
-from openc3.top_level import HazardousError, DisabledError  # noqa: F401
+from openc3.top_level import HazardousError  # Needed for error_class lookup
 
 
 class JsonDrbUnknownError(Exception):
     pass
 
 
 # The Ruby side implements from_hash directly on Exception but Python says:
@@ -39,15 +41,15 @@
     def from_hash(cls, hash):
         # Hash contains class, message, backtrace, and instance_variables
         error_class = None
         try:
             error_class = globals()[hash["class"]]
         except KeyError:
             error_class = RuntimeError
-            if "message" not in hash and "class" in hash:
+            if not "message" in hash and "class" in hash:
                 hash["message"] = hash["class"]
         error = None
         if error_class == RuntimeError and "message" in hash:
             error = error_class(hash["message"])
         else:
             error = error_class()
         if "instance_variables" in hash:
```

### Comparing `openc3-5.16.0/openc3/io/json_rpc.py` & `openc3-5.9.2b0/openc3/io/json_rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -298,15 +300,15 @@
         try:
             json_class = object_["json_class"]
             raw = object_["raw"]
             if json_class == "Float":
                 if raw == "Infinity":
                     return float("inf")
                 elif raw == "-Infinity":
-                    return float("-inf")
+                    return -float("inf")
                 elif raw == "NaN":
                     return float("nan")
                 return raw
             return bytearray(raw)
         except Exception:
             for key, value in object_.items():
                 object_[key] = convert_json_class(value)
@@ -320,18 +322,15 @@
         return object_
     else:
         return object_
 
 
 def _convert_bytearray_to_string_raw(object_):
     if isinstance(object_, (bytes, bytearray)):
-        try:
-            return object_.decode()
-        except UnicodeDecodeError:
-            return {"json_class": "String", "raw": [byte for byte in object_]}
+        return object_.decode("latin-1")
     if isinstance(object_, dict):
         for key, value in object_.items():
             object_[key] = _convert_bytearray_to_string_raw(value)
         return object_
     if isinstance(object_, (tuple, list)):
         object_ = list(object_)
         index = 0
```

### Comparing `openc3-5.16.0/openc3/io/stdout.py` & `openc3-5.9.2b0/openc3/utilities/local_mode.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023, OpenC3, Inc.
+# Copyright 2022 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 #
@@ -10,29 +10,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-from openc3.io.io_multiplexer import IoMultiplexer
+from openc3.environment import OPENC3_LOCAL_MODE_PATH
 
 
-# Adds STDOUT to the multiplexed streams
-class Stdout(IoMultiplexer):
-    my_instance = None
+class LocalMode:
+    LOCAL_MODE_PATH = OPENC3_LOCAL_MODE_PATH or "/plugins"
 
-    def __init__(self):
-        super().__init__()
-        self.streams.append(self.STDOUT)
-        Stdout.my_instance = self
-
-    # @return [Stdout] Returns a single instance of Stdout
     @classmethod
-    def instance(cls):
-        if not Stdout.my_instance:
-            cls()
-        return Stdout.my_instance
-
-    @property
-    def encoding(self):
-        return self.STDOUT.encoding
+    def open_local_file(cls, path, scope):
+        try:
+            full_path = f"{cls.LOCAL_MODE_PATH}/{scope}/targets_modified/{path}"
+            return open(full_path, "rb")
+        except OSError:
+            return None
```

### Comparing `openc3-5.16.0/openc3/models/microservice_status_model.py` & `openc3-5.9.2b0/openc3/models/stash_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,51 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
-# attribution addendums as found in the LICENSE.txt
+# attribution addums as found in the LICENSE.txt
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 from openc3.models.model import Model
+from openc3.environment import OPENC3_SCOPE
 
 
-class MicroserviceStatusModel(Model):
-    PRIMARY_KEY = "openc3_microservice_status"
+class StashModel(Model):
+    PRIMARY_KEY = "openc3__stash"
 
     # NOTE: The following three class methods are used by the ModelController
     # and are reimplemented to enable various Model class methods to work
     @classmethod
-    def get(cls, name, scope=None):
-        return super().get(f"{scope}__{MicroserviceStatusModel.PRIMARY_KEY}", name=name)
+    def get(cls, name, scope=OPENC3_SCOPE):
+        super().get(f"{scope}__{StashModel.PRIMARY_KEY}", name=name)
 
     @classmethod
-    def names(cls, scope=None):
-        return super().names(f"{scope}__{MicroserviceStatusModel.PRIMARY_KEY}")
+    def names(cls, scope=OPENC3_SCOPE):
+        super().names(f"{scope}__{StashModel.PRIMARY_KEY}")
 
     @classmethod
-    def all(cls, scope=None):
-        return super().all(f"{scope}__{MicroserviceStatusModel.PRIMARY_KEY}")
+    def all(cls, scope=OPENC3_SCOPE):
+        super().all(f"{scope}__{StashModel.PRIMARY_KEY}")
+
+    # END NOTE
 
-    def __init__(
-        self,
-        name,
-        state=None,
-        count=0,
-        error=None,
-        custom=None,
-        updated_at=None,
-        plugin=None,
-        scope=None,
-    ):
-        super().__init__(
-            f"{scope}__{MicroserviceStatusModel.PRIMARY_KEY}",
-            name=name,
-            updated_at=updated_at,
-            plugin=plugin,
-            scope=scope,
-        )
-        self.state = state
-        self.count = count
-        self.error = error
-        self.custom = custom
+    def __init__(self, name, value, scope=OPENC3_SCOPE):
+        super.__init__(f"{scope}__{StashModel.PRIMARY_KEY}", name=name, scope=scope)
+        self.value = value
 
+    # self.return [Hash] JSON encoding of this model
     def as_json(self):
-        json = {
+        return {
             "name": self.name,
-            "state": self.state,
-            "count": self.count,
-            "plugin": self.plugin,
-            "updated_at": self.updated_at,
+            "value": self.value.as_json(),
         }
-        if self.error is not None:
-            json["error"] = repr(self.error)
-        if self.custom is not None:
-            json["custom"] = self.custom.as_json()
-        return json
```

### Comparing `openc3-5.16.0/openc3/models/model.py` & `openc3-5.9.2b0/openc3/models/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,148 +12,157 @@
 # GNU Affero General Public License for more details.
 
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import json
 import time
-from typing import Optional
+from openc3.utilities.store import Store
 
-from openc3.utilities.store import Store, EphemeralStore
-from openc3.utilities.store_queued import StoreQueued, EphemeralStoreQueued
+# require 'openc3/config/config_parser'
 
+# attr_accessor :name
+# attr_accessor :updated_at
+# attr_accessor :plugin
+# attr_accessor :scope
 
-class Model:
-    @classmethod
-    def store(cls):
-        return Store
-
-    @classmethod
-    def store_queued(cls):
-        return StoreQueued
 
+class Model:
     # NOTE: The following three methods must be reimplemented by Model subclasses
     # without primary_key to support other class methods.
 
     @classmethod
-    def get(cls, primary_key: str, name: str):
+    def get(primary_key, name):
         """@return [Hash|nil] Hash of this model or nil if name not found under primary_key"""
-        json_data = cls.store().hget(primary_key, name)
-        return json.loads(json_data) if json_data else None
+        json_data = Store.hget(primary_key, name)
+        if json_data:
+            return json.loads(json)
+        else:
+            return None
 
     @classmethod
-    def names(cls, primary_key: str):
+    def names(primary_key):
         """@return [Array<String>] All the names stored under the primary key"""
-        keys = cls.store().hkeys(primary_key)
-        keys.sort()
-        return [key.decode() for key in keys]
+        Store.hkeys(primary_key).sort()
 
     @classmethod
-    def all(cls, primary_key: str):
+    def all(primary_key):
         """@return [Array<Hash>] All the models (as Hash objects) stored under the primary key"""
-        base = cls.store().hgetall(primary_key)
-        # decode the binary string keys to strings
-        hash_ = {k.decode(): v for (k, v) in base.items()}
-        for key, value in hash_.items():
-            hash_[key] = json.loads(value)
-        return hash_
+        hash = Store.hgetall(primary_key)
+        for key, value in hash.items():
+            hash[key] = json.loads(value)
+        return hash
 
     # END NOTE
 
-    # Sets (updates) the redis hash of this model
-    @classmethod
-    def set(cls, json_data: dict, scope: str, queued: bool = False):
-        json_data["scope"] = scope
-        cls(**json_data).create(force=True, queued=queued)
-
-    # @return [Model] Model generated from the passed JSON
-    @classmethod
-    def from_json(cls, json_data: str | dict, scope: str):
-        if type(json_data) is str:
-            json_data = json.loads(json_data)
-        if json_data is None:
-            raise RuntimeError("json data is nil")
-        json_data["scope"] = scope
-        return cls(**json_data)
-
-    # Calls self.get and then from_json to turn the Hash configuration into a Ruby Model object.
-    # @return [Object|nil] Model object or nil if name not found under primary_key
-    @classmethod
-    def get_model(cls, name: str, scope: str):
-        json_data = cls.get(name, scope)
-        return cls.from_json(json_data, scope) if json_data else None
-
-    # NOTE: get_all_models not implemented as it is currently
-    # unused by any python models
+    #     # Loops over all items and returns objects that match a key value pair
+    #     def self.filter(key, value, scope:, substr: false)
+    #       filtered = {}
+    #       results = all(scope: scope)
+    #       results.each do |name, result|
+    #         if result[key] == value || (substr && result[key].include?(value))
+    #           filtered[name] = result
+    #         end
+    #       end
+    #       return filtered
+    #     end
 
-    # NOTE: find_all_by_plugin, handle_config not implemented as it is
-    # only needed by plugin_model which is Ruby only
+    # Sets (updates) the redis hash of this model
+    def set(cls, json, scope):
+        json[scope] = scope
+        cls()(**json).create(force=True)
+
+    #     # @return [Model] Model generated from the passed JSON
+    #     def self.from_json(json, scope:)
+    #       json = JSON.parse(json, :allow_nan => true, :create_additions => true) if String === json
+    #       raise "json data is nil" if json.nil?
+    #       json[:scope] = scope
+    #       self.new(**json.transform_keys(&:to_sym), scope: scope)
+    #     end
+
+    #     # Calls self.get and then from_json to turn the Hash configuration into a Ruby Model object.
+    #     # @return [Object|nil] Model object or nil if name not found under primary_key
+    #     def self.get_model(name:, scope:)
+    #       json = get(name: name, scope: scope)
+    #       if json
+    #         return from_json(json, scope: scope)
+    #       else
+    #         return nil
+    #       end
+    #     end
+
+    #     # @return [Array<Object>] All the models (as Model objects) stored under the primary key
+    #     def self.get_all_models(scope:)
+    #       models = {}
+    #       all(scope: scope).each { |name, json| models[name] = from_json(json, scope: scope) }
+    #       models
+    #     end
+
+    #     # @return [Array<Object>] All the models (as Model objects) stored under the primary key
+    #     #   which have the plugin attribute
+    #     def self.find_all_by_plugin(plugin:, scope:)
+    #       result = {}
+    #       models = get_all_models(scope: scope)
+    #       models.each do |name, model|
+    #         result[name] = model if model.plugin == plugin
+    #       end
+    #       result
+    #     end
+
+    #     def self.handle_config(parser, keyword, parameters)
+    #       raise "must be implemented by subclass"
+    #     end
 
     # Store the primary key and keyword arguments
-    def __init__(self, primary_key: str, **kw_args):
-        self.primary_key: str = primary_key
-        self.name: Optional[str] = kw_args.get("name")
-        self.updated_at: Optional[float] = kw_args.get("updated_at")
-        self.plugin: Optional[str] = kw_args.get("plugin")
-        self.scope: Optional[str] = kw_args.get("scope")
-        self.destroyed: bool = False
+    def __init__(self, primary_key, **kw_args):
+        self.primary_key = primary_key
+        self.name = kw_args["name"]
+        self.updated_at = kw_args["updated_at"]
+        self.plugin = kw_args["plugin"]
+        self.scope = kw_args["scope"]
+        self.destroyed = False
 
     # Update the Redis hash at primary_key and set the field "name"
     # to the JSON generated via calling as_json
-    def create(self, update=False, force=False, queued=False):
+    def create(self, update=False, force=False):
         if not force:
-            existing = self.store().hget(self.primary_key, self.name)
+            existing = Store.hget(self.primary_key, self.name)
             if existing and not update:
                 raise RuntimeError(
                     f"{self.primary_key}:{self.name} already exists at create"
                 )
             if not existing and update:
                 raise RuntimeError(
                     f"{self.primary_key}:{self.name} doesn't exist at update"
                 )
         self.updated_at = time.time() * 1_000_000_000
-
-        if queued:
-            write_store = self.store_queued()
-        else:
-            write_store = self.store()
-
-        write_store.hset(self.primary_key, self.name, json.dumps(self.as_json()))
+        Store.hset(self.primary_key, self.name, json.dumps(self.as_json()))
 
     # Alias for create(update: true)
-    def update(self, force=False, queued=True):
-        self.create(update=True, force=force, queued=queued)
+    def update(self):
+        self.create(update=True)
 
-    # Deploy the model into the OpenC3 system. Subclasses must implement this
-    # and typically create MicroserviceModels to implement.
-    def deploy(self, gem_path: str, variables: str):
-        raise NotImplementedError("must be implemented by subclass")
+    #     # Deploy the model into the OpenC3 system. Subclasses must implement this
+    #     # and typically create MicroserviceModels to implement.
+    #     def deploy(gem_path, variables)
+    #       raise "must be implemented by subclass"
+    #     end
 
     # Undo the actions of deploy and remove the model from OpenC3.
     # Subclasses must implement this as by default it is a noop.
     def undeploy(self):
         pass
 
     # Delete the model from the Store
     def destroy(self):
         self.destroyed = True
         self.undeploy()
-        self.store().hdel(self.primary_key, self.name)
+        Store.hdel(self.primary_key, self.name)
 
     # @return [Hash] JSON encoding of this model
     def as_json(self):
         return {
             "name": self.name,
             "updated_at": self.updated_at,
             "plugin": self.plugin,
             "scope": self.scope,
         }
-
-
-class EphemeralModel(Model):
-    @classmethod
-    def store(cls):
-        return EphemeralStore
-
-    @classmethod
-    def store_queued(cls):
-        return EphemeralStoreQueued
```

### Comparing `openc3-5.16.0/openc3/models/reducer_model.py` & `openc3-5.9.2b0/openc3/models/reducer_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,45 +14,44 @@
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import os
 import re
 from openc3.utilities.store import Store
 
-
 # Tracks the files which are being stored in buckets for data reduction purposes.
 # Files are stored in a Redis set by spliting their filenames and storing in
 # a set named SCOPE__TARGET__reducer__TYPE, e.g. DEFAULT__INST__reducer__decom
 # Where TYPE can be 'decom', 'minute', or 'hour'. 'day' is not necessary because
 # day is the final reduction state. As files are reduced they are removed from
 # the set. Thus the sets contain the active set of files to be reduced.
 class ReducerModel:
-    DECOM_BIN_GZ = re.compile(r"__decom\.bin.gz$")
-    REDUCED_MINUTE_BIN_GZ = re.compile(r"__reduced_minute\.bin.gz$")
-    REDUCED_HOUR_BIN_GZ = re.compile(r"__reduced_hour\.bin.gz$")
+    DECOM_BIN_GZ = re.compile("__decom\.bin.gz$")
+    REDUCED_MINUTE_BIN_GZ = re.compile("__reduced_minute\.bin.gz$")
+    REDUCED_HOUR_BIN_GZ = re.compile("__reduced_hour\.bin.gz$")
 
     @classmethod
     def add_file(cls, bucket_key):
         # Only reduce tlm files
-        bucket_key_split = bucket_key.split("/")
-        if bucket_key_split[2] == "tlm":
+        bucket_key_split = bucket_key.split('/')
+        if bucket_key_split[2] == 'tlm':
             # bucket_key is formatted like STARTTIME__ENDTIME__SCOPE__TARGET__PACKET__TYPE.bin
             # e.g. 20211229191610578229500__20211229192610563836500__DEFAULT__INST__HEALTH_STATUS__rt__decom.bin
-            _, _, scope, target, _ = os.path.basename(bucket_key).split("__")
+            _, _, scope, target, _ = os.path.basename(bucket_key).split('__')
             if cls.DECOM_BIN_GZ.match(bucket_key):
                 return Store.sadd(f"{scope}__{target}__reducer__decom", bucket_key)
             elif cls.REDUCED_MINUTE_BIN_GZ.match(bucket_key):
                 return Store.sadd(f"{scope}__{target}__reducer__minute", bucket_key)
             elif cls.REDUCED_HOUR_BIN_GZ.match(bucket_key):
                 return Store.sadd(f"{scope}__{target}__reducer__hour", bucket_key)
             # No else clause because add_file is called with raw files which are ignored
 
     @classmethod
     def rm_file(cls, bucket_key):
-        _, _, scope, target, _ = bucket_key.split("__")
+        _, _, scope, target, _ = bucket_key.split('__')
         if cls.DECOM_BIN_GZ.match(bucket_key):
             return Store.srem(f"{scope}__{target}__reducer__decom", bucket_key)
         elif cls.REDUCED_MINUTE_BIN_GZ.match(bucket_key):
             return Store.srem(f"{scope}__{target}__reducer__minute", bucket_key)
         elif cls.REDUCED_HOUR_BIN_GZ.match(bucket_key):
             return Store.srem(f"{scope}__{target}__reducer__hour", bucket_key)
         else:
```

### Comparing `openc3-5.16.0/openc3/models/router_model.py` & `openc3-5.9.2b0/openc3/script/exceptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -10,12 +12,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-from openc3.models.interface_model import InterfaceModel
+
+class CheckError(Exception):
+    pass
+
+
+class StopScript(Exception):
+    pass
 
 
-class RouterModel(InterfaceModel):
+class SkipScript(Exception):
     pass
```

### Comparing `openc3-5.16.0/openc3/packets/commands.py` & `openc3-5.9.2b0/openc3/packets/commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addums as found in the LICENSE.txt
@@ -10,19 +12,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-from datetime import datetime, timezone
-from openc3.packets.packet import Packet
-from openc3.utilities.string import simple_formatted
-from openc3.utilities.extract import convert_to_value
-
 
 class Commands:
     """Commands uses PacketConfig to parse the command and telemetry
     configuration files. It contains all the knowledge of which command packets
     exist in the system and how to access them. This class is the API layer
     which other classes use to access commands.
 
@@ -32,299 +29,304 @@
     Packet or PacketItem objects. While there are some overlapping methods between
     the two, these are separate interfaces into the system."""
 
     LATEST_PACKET_NAME = "LATEST"
 
     # @param config [PacketConfig] Packet configuration to use to access the
     #  commands
-    def __init__(self, config, system):
+    def __init__(self, config):
         self.config = config
-        self.system = system
 
     # (see PacketConfig#warnings)
     def warnings(self):
         return self.config.warnings
 
     # @return [Array<String>] The command target names (excluding UNKNOWN)
     def target_names(self):
-        result = list(self.config.commands.keys())
-        if "UNKNOWN" in result:
-            result.remove("UNKNOWN")
+        result = self.config.commands.keys().sort()
+        result.delete("UNKNOWN")
         return result
 
     # @param target_name [String] The target name
     # @return [Hash<packet_name=>Packet>] Hash of the command packets for the given
     #   target name keyed by the packet name
     def packets(self, target_name):
         target_packets = self.config.commands.get(target_name.upper(), None)
-        if target_packets is None:
-            raise RuntimeError(f"Command target '{target_name.upper()}' does not exist")
+        if not target_packets:
+            raise Exception(f"Command target '{target_name.upper()}' does not exist")
         return target_packets
 
     # @param target_name [String] The target name
     # @param packet_name [String] The packet name. Must be a defined packet name
     #   and not 'LATEST'.
     # @return [Packet] The command packet for the given target and packet name
     def packet(self, target_name, packet_name):
         target_packets = self.packets(target_name)
         packet = target_packets.get(packet_name.upper(), None)
-        if packet is None:
-            raise RuntimeError(
+        if not packet:
+            raise Exception(
                 f"Command packet '{target_name.upper()} {packet_name.upper()}' does not exist"
             )
         return packet
 
     # @param target_name (see #packet)
     # @param packet_name (see #packet)
     # @return [Array<PacketItem>] The command parameters for the given target and packet name
     def params(self, target_name, packet_name):
         return self.packet(target_name, packet_name).sorted_items
 
-    # Identifies an unknown buffer of data as a defined command and sets the
-    # commands's data to the given buffer. Identifying a command uses the fields
-    # marked as ID_PARAMETER to identify if the buffer passed represents the
-    # command defined. Incorrectly sized buffers are still processed but an
-    # error is logged.
-    #
-    # Note: Subsequent requests for the command (using packet) will return
-    # an uninitialized copy of the command. Thus you must use the return value
-    # of this method.
-    #
-    # @param (see #identify_tlm!)
-    # @return (see #identify_tlm!)
-    def identify(self, packet_data, target_names=None):
-        identified_packet = None
-
-        if not target_names:
-            target_names = self.target_names()
-
-        for target_name in target_names:
-            target_name = str(target_name).upper()
-            target_packets = None
-            try:
-                target_packets = self.packets(target_name)
-            except RuntimeError:
-                # No commands for this target
-                continue
-
-            target = self.system.targets.get(target_name)
-            if target and target.cmd_unique_id_mode:
-                # Iterate through the packets and see if any represent the buffer
-                for _, packet in target_packets.items():
-                    if packet.identify(packet_data):
-                        identified_packet = packet
-                        break
-            else:
-                # Do a hash lookup to quickly identify the packet
-                if len(target_packets) > 0:
-                    packet = next(iter(target_packets.values()))
-                    key = packet.read_id_values(packet_data)
-                    hash = self.config.cmd_id_value_hash[target_name]
-                    identified_packet = hash.get(str(key))
-                    if identified_packet is None:
-                        identified_packet = hash.get("CATCHALL")
-
-            if identified_packet is not None:
-                identified_packet.received_count += 1
-                identified_packet = identified_packet.clone()
-                identified_packet.received_time = None
-                identified_packet.stored = False
-                identified_packet.extra = None
-                identified_packet.buffer = packet_data
-                break
-
-        return identified_packet
-
-    # Returns a copy of the specified command packet with the parameters
-    # initialzed to the given params values.
-    #
-    # @param target_name (see #packet)
-    # @param packet_name (see #packet)
-    # @param params [Hash<param_name=>param_value>] Parameter items to override
-    #   in the given command.
-    # @param range_checking [Boolean] Whether to perform range checking on the
-    #   passed in parameters.
-    # @param raw [Boolean] Indicates whether or not to run conversions on command parameters
-    # @param check_required_params [Boolean] Indicates whether or not to check
-    #   that the required command parameters are present
-    def build_cmd(
-        self,
-        target_name,
-        packet_name,
-        params={},
-        range_checking=True,
-        raw=False,
-        check_required_params=True,
-    ):
-        target_upcase = target_name.upper()
-        packet_upcase = packet_name.upper()
-
-        # Lookup the command and create a light weight copy
-        pkt = self.packet(target_upcase, packet_upcase)
-        pkt.received_count += 1
-        command = pkt.clone()
-
-        # Restore the command's buffer to a zeroed string of defined length
-        # This will undo any side effects from earlier commands that may have altered the size
-        # of the buffer
-        command.buffer = bytearray(b"\x00" * command.defined_length)
-
-        # Set time, parameters, and restore defaults
-        command.received_time = datetime.now(timezone.utc)
-        command.stored = False
-        command.extra = None
-        command.given_values = params
-        command.restore_defaults(command.buffer_no_copy(), list(params.keys()))
-        command.raw = raw
-
-        given_item_names = self._set_parameters(command, params, range_checking)
-        if check_required_params:
-            self._check_required_params(command, given_item_names)
-
-        return command
-
-    # Formatted version of a command
-    def format(self, packet, ignored_parameters=[]):
-        if packet.raw:
-            items = packet.read_all("RAW")
-            raw = True
-        else:
-            items = packet.read_all("FORMATTED")
-            raw = False
-        items = [item for item in items if item[0] not in ignored_parameters]
-        return self.build_cmd_output_string(
-            packet.target_name, packet.packet_name, items, raw
-        )
-
-    def build_cmd_output_string(self, target_name, cmd_name, cmd_params, raw=False):
-        if raw:
-            output_string = 'cmd_raw("'
-        else:
-            output_string = 'cmd("'
-        if not target_name:
-            target_name = "UNKNOWN"
-        if not cmd_name:
-            cmd_name = "UNKNOWN"
-        output_string += target_name + " " + cmd_name
-        if cmd_params is None or len(cmd_params) == 0:
-            output_string += '")'
-        else:
-            # TODO: Try except around this?
-            command_items = self.packet(target_name, cmd_name).items
-
-            params = []
-            for key, value in cmd_params:
-                if key in Packet.RESERVED_ITEM_NAMES:
-                    continue
-
-                try:
-                    item_type = command_items[key].data_type
-                except KeyError:
-                    item_type = None
-
-                if isinstance(value, str):
-                    if item_type == "BLOCK" or item_type == "STRING":
-                        if not value.isascii():
-                            value = "0x" + simple_formatted(value)
-                        else:
-                            value = f"'{str(value)}'"
-                    else:
-                        value = str(convert_to_value(value))
-                    if len(value) > 256:
-                        value = value[:256] + "...'"
-                    value = value.replace('"', "'")
-                elif isinstance(value, list):
-                    value = f"[{', '.join(str(i) for i in value)}]"
-                params.append(f"{key} {value}")
-            params = (", ").join(params)
-            output_string += " with " + params + '")'
-        return output_string
-
-    # Returns whether the given command is hazardous. Commands are hazardous
-    # if they are marked hazardous overall or if any of their hardardous states
-    # are set. Thus any given parameter values are first applied to the command
-    # and then checked for hazardous states.
-    #
-    # @param command [Packet] The command to check for hazardous
-    def cmd_pkt_hazardous(self, command):
-        if command.hazardous:
-            return (True, command.hazardous_description)
-
-        # Check each item for hazardous states
-        for item_name, item_def in command.items.items():
-            if item_def.hazardous:
-                state_name = command.read(item_name)
-                # Nominally the command.read will return a valid state_name
-                # If it doesn't, the if check will fail and we'll fall through to
-                # the bottom where we return [false, nil] which means this
-                # command is not hazardous.
-                if item_def.hazardous.get(state_name) is not None:
-                    return (True, item_def.hazardous[state_name])
-
-        return (False, None)
-
-    # Returns whether the given command is hazardous. Commands are hazardous
-    # if they are marked hazardous overall or if any of their hardardous states
-    # are set. Thus any given parameter values are first applied to the command
-    # and then checked for hazardous states.
-    #
-    # @param target_name (see #packet)
-    # @param packet_name (see #packet)
-    # @param params (see #build_cmd)
-    def cmd_hazardous(self, target_name, packet_name, params={}):
-        # Build a command without range checking, perform conversions, and don't
-        # check required parameters since we're not actually using the command.
-        return self.cmd_pkt_hazardous(
-            self.build_cmd(target_name, packet_name, params, False, False, False)
-        )
-
-    def clear_counters(self):
-        for target_name, target_packets in self.config.commands.items():
-            for packet_name, packet in target_packets.items():
-                packet.received_count = 0
-
-    def all(self):
-        return self.config.commands
-
-    def _set_parameters(self, command, params, range_checking):
-        given_item_names = []
-        for item_name, value in params.items():
-            item_upcase = item_name.upper()
-            item = command.get_item(item_upcase)
-            range_check_value = value
-
-            # Convert from state to value if possible
-            if (
-                item.states is not None
-                and item.states.get(str(value).upper()) is not None
-            ):
-                range_check_value = item.states[value.upper()]
-
-            if range_checking:
-                minimum = item.minimum
-                maximum = item.maximum
-                if minimum is not None and maximum is not None:
-                    # Perform Range Check on command parameter
-                    if range_check_value < minimum or range_check_value > maximum:
-                        if type(range_check_value) is str:
-                            range_check_value = f"'{range_check_value}'"
-                        raise RuntimeError(
-                            f"Command parameter '{command.target_name} {command.packet_name} {item_upcase}' = {range_check_value} not in valid range of {minimum} to {maximum}"
-                        )
-
-            # Update parameter in command
-            if command.raw:
-                command.write(item_upcase, value, "RAW")
-            else:
-                command.write(item_upcase, value, "CONVERTED")
-            given_item_names.append(item_upcase)
-
-        return given_item_names
-
-    def _check_required_params(self, command, given_item_names):
-        # Script Runner could call this command with only some parameters
-        # so make sure any required parameters were actually passed in.
-        for item_name, item_def in command.items.items():
-            if item_def.required and item_name not in given_item_names:
-                raise RuntimeError(
-                    f"Required command parameter '{command.target_name} {command.packet_name} {item_name}' not given"
-                )
+
+#   # Identifies an unknown buffer of data as a defined command and sets the
+#   # commands's data to the given buffer. Identifying a command uses the fields
+#   # marked as ID_PARAMETER to identify if the buffer passed represents the
+#   # command defined. Incorrectly sized buffers are still processed but an
+#   # error is logged.
+#   #
+#   # Note: Subsequent requests for the command (using packet) will return
+#   # an uninitialized copy of the command. Thus you must use the return value
+#   # of this method.
+#   #
+#   # @param (see #identify_tlm!)
+#   # @return (see #identify_tlm!)
+#   def identify(packet_data, target_names = nil)
+#     identified_packet = nil
+
+#     target_names = target_names() unless target_names
+
+#     target_names.each do |target_name|
+#       target_name = target_name.to_s.upcase
+#       target_packets = nil
+#       begin
+#         target_packets = packets(target_name)
+#       rescue RuntimeError
+#         # No commands for this target
+#         next
+
+
+#       target = System.targets[target_name]
+#       if target and target.cmd_unique_id_mode
+#         # Iterate through the packets and see if any represent the buffer
+#         target_packets.each do |packet_name, packet|
+#           if packet.identify?(packet_data)
+#             identified_packet = packet
+#             break
+
+
+#       else
+#         # Do a hash lookup to quickly identify the packet
+#         if target_packets.length > 0
+#           packet = target_packets.first[1]
+#           key = packet.read_id_values(packet_data)
+#           hash = self.config.cmd_id_value_hash[target_name]
+#           identified_packet = hash[key]
+#           identified_packet = hash['CATCHALL'.freeze] unless identified_packet
+
+
+#       if identified_packet
+#         identified_packet.received_count += 1
+#         identified_packet = identified_packet.clone
+#         identified_packet.received_time = nil
+#         identified_packet.stored = false
+#         identified_packet.extra = nil
+#         identified_packet.buffer = packet_data
+#         break
+
+
+#     return identified_packet
+
+
+#   # Returns a copy of the specified command packet with the parameters
+#   # initialzed to the given params values.
+#   #
+#   # @param target_name (see #packet)
+#   # @param packet_name (see #packet)
+#   # @param params [Hash<param_name=>param_value>] Parameter items to override
+#   #   in the given command.
+#   # @param range_checking [Boolean] Whether to perform range checking on the
+#   #   passed in parameters.
+#   # @param raw [Boolean] Indicates whether or not to run conversions on command parameters
+#   # @param check_required_params [Boolean] Indicates whether or not to check
+#   #   that the required command parameters are present
+#   def build_cmd(target_name, packet_name, params = {}, range_checking = true, raw = false, check_required_params = true)
+#     target_upcase = target_name.to_s.upcase
+#     packet_upcase = packet_name.to_s.upcase
+
+#     # Lookup the command and create a light weight copy
+#     pkt = packet(target_upcase, packet_upcase)
+#     pkt.received_count += 1
+#     command = pkt.clone
+
+#     # Restore the command's buffer to a zeroed string of defined length
+#     # This will undo any side effects from earlier commands that may have altered the size
+#     # of the buffer
+#     command.buffer = "\x00" * command.defined_length
+
+#     # Set time, parameters, and restore defaults
+#     command.received_time = Time.now.sys
+#     command.stored = false
+#     command.extra = nil
+#     command.given_values = params
+#     command.restore_defaults(command.buffer(false), params.keys)
+#     command.raw = raw
+
+#     given_item_names = set_parameters(command, params, range_checking)
+#     check_required_params(command, given_item_names) if check_required_params
+
+#     return command
+
+
+#   # Formatted version of a command
+#   def format(packet, ignored_parameters = [])
+#     if packet.raw
+#       items = packet.read_all(:RAW)
+#       raw = true
+#     else
+#       items = packet.read_all(:FORMATTED)
+#       raw = false
+
+#     items.delete_if { |item_name, item_value| ignored_parameters.include?(item_name) }
+#     return build_cmd_output_string(packet.target_name, packet.packet_name, items, raw)
+
+
+#   def build_cmd_output_string(target_name, cmd_name, cmd_params, raw = false)
+#     if raw
+#       output_string = 'cmd_raw("'
+#     else
+#       output_string = 'cmd("'
+
+#     target_name = 'UNKNOWN' unless target_name
+#     cmd_name = 'UNKNOWN' unless cmd_name
+#     output_string << target_name + ' ' + cmd_name
+#     if cmd_params.nil? or cmd_params.empty?
+#       output_string << '")'
+#     else
+#       begin
+#         command_items = packet(target_name, cmd_name).items
+#       rescue
+
+
+#       params = []
+#       cmd_params.each do |key, value|
+#         next if Packet::RESERVED_ITEM_NAMES.include?(key)
+
+#         begin
+#           item_type = command_items[key].data_type
+#         rescue
+#           item_type = nil
+
+
+#         if value.is_a?(String)
+#           value = value.dup
+#           if item_type == :BLOCK or item_type == :STRING
+#             if !value.is_printable?
+#               value = "0x" + value.simple_formatted
+#             else
+#               value = value.inspect
+
+#           else
+#             value = value.convert_to_value.to_s
+
+#           if value.length > 256
+#             value = value[0..255] + "...'"
+
+#           value.tr!('"', "'")
+#         elsif value.is_a?(Array)
+#           value = "[{value.join(", ")}]"
+
+#         params << "{key} {value}"
+
+#       params = params.join(", ")
+#       output_string << ' with ' + params + '")'
+
+#     return output_string
+
+
+#   # Returns whether the given command is hazardous. Commands are hazardous
+#   # if they are marked hazardous overall or if any of their hardardous states
+#   # are set. Thus any given parameter values are first applied to the command
+#   # and then checked for hazardous states.
+#   #
+#   # @param command [Packet] The command to check for hazardous
+#   def cmd_pkt_hazardous?(command)
+#     return [true, command.hazardous_description] if command.hazardous
+
+#     # Check each item for hazardous states
+#     item_defs = command.items
+#     item_defs.each do |item_name, item_def|
+#       if item_def.hazardous
+#         state_name = command.read(item_name)
+#         # Nominally the command.read will return a valid state_name
+#         # If it doesn't, the if check will fail and we'll fall through to
+#         # the bottom where we return [false, nil] which means this
+#         # command is not hazardous.
+#         return [true, item_def.hazardous[state_name]] if item_def.hazardous[state_name]
+
+
+#     return [false, nil]
+
+
+#   # Returns whether the given command is hazardous. Commands are hazardous
+#   # if they are marked hazardous overall or if any of their hardardous states
+#   # are set. Thus any given parameter values are first applied to the command
+#   # and then checked for hazardous states.
+#   #
+#   # @param target_name (see #packet)
+#   # @param packet_name (see #packet)
+#   # @param params (see #build_cmd)
+#   def cmd_hazardous?(target_name, packet_name, params = {})
+#     # Build a command without range checking, perform conversions, and don't
+#     # check required parameters since we're not actually using the command.
+#     cmd_pkt_hazardous?(build_cmd(target_name, packet_name, params, false, false, false))
+
+
+#   def clear_counters
+#     self.config.commands.each do |target_name, target_packets|
+#       target_packets.each do |packet_name, packet|
+#         packet.received_count = 0
+
+
+#   def all
+#     self.config.commands
+
+
+#   protected
+
+#   def set_parameters(command, params, range_checking)
+#     given_item_names = []
+#     params.each do |item_name, value|
+#       item_upcase = item_name.to_s.upcase
+#       item = command.get_item(item_upcase)
+#       range_check_value = value
+
+#       # Convert from state to value if possible
+#       if item.states and item.states[value.to_s.upcase]
+#         range_check_value = item.states[value.to_s.upcase]
+
+
+#       if range_checking
+#         range = item.range
+#         if range
+#           # Perform Range Check on command parameter
+#           if not range.include?(range_check_value)
+#             range_check_value = "'{range_check_value}'" if String === range_check_value
+#             raise "Command parameter '{command.target_name} {command.packet_name} {item_upcase}' = {range_check_value} not in valid range of {range.first} to {range.last}"
+
+
+#       # Update parameter in command
+#       if command.raw
+#         command.write(item_upcase, value, :RAW)
+#       else
+#         command.write(item_upcase, value, :CONVERTED)
+
+
+#       given_item_names << item_upcase
+
+#     given_item_names
+
+
+#   def check_required_params(command, given_item_names)
+#     # Script Runner could call this command with only some parameters
+#     # so make sure any required parameters were actually passed in.
+#     item_defs = command.items
+#     item_defs.each do |item_name, item_def|
+#       if item_def.required and not given_item_names.include? item_name
+#         raise "Required command parameter '{command.target_name} {command.packet_name} {item_name}' not given"
```

### Comparing `openc3-5.16.0/openc3/packets/limits.py` & `openc3-5.9.2b0/openc3/packets/limits.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -22,17 +24,16 @@
     setting and checking individual limit items as well as manipulating limits groups.
     """
 
     LATEST_PACKET_NAME = "LATEST"
 
     # @param config [PacketConfig] Packet configuration to use to access the
     #  limits
-    def __init__(self, config, system):
+    def __init__(self, config):
         self.config = config
-        self.system = system
 
     # (see PacketConfig#warnings)
     def warnings(self):
         return self.config.warnings
 
     # (see PacketConfig#limits_sets)
     def sets(self):
@@ -46,156 +47,138 @@
                 items += packet.out_of_limits()
         return items
 
     # @return [Hash(String, Array)] The defined limits groups
     def groups(self):
         return self.config.limits_groups
 
-    # Checks whether the limits are enabled for the specified item
-    #
-    # @param target_name [String] The target name
-    # @param packet_name [String] The packet name. Must be a defined packet name and not 'LATEST'.
-    # @param item_name [String] The item name
-    def enabled(self, target_name, packet_name, item_name):
-        return (
-            self._get_packet(target_name, packet_name)
-            .get_item(item_name)
-            .limits.enabled
-        )
-
-    # Enables limit checking for the specified item
-    #
-    # @param (see #enabled?)
-    def enable(self, target_name, packet_name, item_name):
-        self._get_packet(target_name, packet_name).enable_limits(item_name)
-
-    # Disables limit checking for the specified item
-    #
-    # @param (see #enabled?)
-    def disable(self, target_name, packet_name, item_name):
-        self._get_packet(target_name, packet_name).disable_limits(item_name)
-
-    # Get the limits for a telemetry item
-    #
-    # @param target_name [String] Target Name
-    # @param packet_name [String] Packet Name
-    # @param item_name [String] Item Name
-    # @param limits_set [String or Symbol or nil] Desired Limits set.  nil = current limits set
-    # @return [Array<limits_set, persistence, enabled, red_low, yellow_low, red_high, yellow_high, green_low (optional), green_high (optional)] Limits information
-    def get(self, target_name, packet_name, item_name, limits_set=None):
-        limits = self._get_packet(target_name, packet_name).get_item(item_name).limits
-        if limits.values:
-            if limits_set:
-                limits_set = str(limits_set).upper()
-            else:
-                limits_set = self.system.limits_set
-            limits_for_set = limits.values.get(limits_set)
-            if limits_for_set is not None:
-                return [
-                    limits_set,
-                    limits.persistence_setting,
-                    limits.enabled,
-                    limits_for_set[0],
-                    limits_for_set[1],
-                    limits_for_set[2],
-                    limits_for_set[3],
-                    limits_for_set[4],
-                    limits_for_set[5],
-                ]
-            else:
-                return [None, None, None, None, None, None, None, None, None]
-        else:
-            return [None, None, None, None, None, None, None, None, None]
-
-    # Set the limits for a telemetry item
-    #
-    # @param target_name [String] Target Name
-    # @param packet_name [String] Packet Name
-    # @param item_name [String] Item Name
-    # @param red_low [Float] Red Low Limit
-    # @param yellow_low [Float] Yellow Low Limit
-    # @param yellow_high [Float] Yellow High Limit
-    # @param red_high [Float] Red High Limit
-    # @param green_low [Float] Green Low Limit
-    # @param green_high [Float] Green High Limit
-    # @param limits_set [String or Symbol or nil] Desired Limits set.  nil = current limits set, recommend using :CUSTOM
-    # @param persistence [Integer] The number of samples the value must be out of limits before detecting a limits change. nil = Leave unchanged
-    # @param enabled [Boolean] If limits monitoring is enabled for this item
-    # @return [Array<limits_set, persistence, enabled, red_low, yellow_low, red_high, yellow_high, green_low (optional), green_high (optional)] Limits information
-    def set(
-        self,
-        target_name,
-        packet_name,
-        item_name,
-        red_low,
-        yellow_low,
-        yellow_high,
-        red_high,
-        green_low=None,
-        green_high=None,
-        limits_set="CUSTOM",
-        persistence=None,
-        enabled=True,
-    ):
-        packet = self._get_packet(target_name, packet_name)
-        item = packet.get_item(item_name)
-        limits = item.limits
-        if limits_set:
-            limits_set = str(limits_set).upper()
-        else:
-            limits_set = self.system.limits_set
-        if limits.values is None:
-            if limits_set == "DEFAULT":
-                limits.values = {"DEFAULT": []}
-            else:
-                raise RuntimeError(
-                    f"DEFAULT limits must be defined for {target_name} {packet_name} {item_name} before setting limits set {limits_set}"
-                )
-        limits_for_set = limits.values.get(limits_set)
-        if limits_for_set is None:
-            limits.values[limits_set] = []
-            limits_for_set = limits.values[limits_set]
-        while len(limits_for_set) < 6:
-            limits_for_set.append(None)
-        limits_for_set[0] = float(red_low)
-        limits_for_set[1] = float(yellow_low)
-        limits_for_set[2] = float(yellow_high)
-        limits_for_set[3] = float(red_high)
-        if green_low and green_high:
-            limits_for_set[4] = float(green_low)
-            limits_for_set[5] = float(green_high)
-        if enabled is not None:
-            limits.enabled = enabled
-        if persistence is not None:
-            limits.persistence_setting = int(persistence)
-        packet.update_limits_items_cache(item)
-        if limits_set not in self.config.limits_sets:
-            self.config.limits_sets.append(limits_set)
-        return [
-            limits_set,
-            limits.persistence_setting,
-            limits.enabled,
-            limits_for_set[0],
-            limits_for_set[1],
-            limits_for_set[2],
-            limits_for_set[3],
-            limits_for_set[4],
-            limits_for_set[5],
-        ]
-
-    def _get_packet(self, target_name, packet_name):
-        if packet_name.upper() == Limits.LATEST_PACKET_NAME:
-            raise RuntimeError("LATEST packet not valid")
-
-        packets = self.config.telemetry.get(target_name.upper())
-        if packets is None:
-            raise RuntimeError(
-                f"Telemetry target '{target_name.upper()}' does not exist"
-            )
-
-        packet = packets.get(packet_name.upper())
-        if packet is None:
-            raise RuntimeError(
-                f"Telemetry packet '{target_name.upper()} { packet_name.upper()}' does not exist"
-            )
 
-        return packet
+#     # Checks whether the limits are enabled for the specified item
+#     #
+#     # @param target_name [String] The target name
+#     # @param packet_name [String] The packet name. Must be a defined packet name and not 'LATEST'.
+#     # @param item_name [String] The item name
+#     def enabled?(target_name, packet_name, item_name)
+#       get_packet(target_name, packet_name).get_item(item_name).limits.enabled
+#     end
+
+#     # Enables limit checking for the specified item
+#     #
+#     # @param (see #enabled?)
+#     def enable(target_name, packet_name, item_name)
+#       get_packet(target_name, packet_name).enable_limits(item_name)
+#     end
+
+#     # Disables limit checking for the specified item
+#     #
+#     # @param (see #enabled?)
+#     def disable(target_name, packet_name, item_name)
+#       get_packet(target_name, packet_name).disable_limits(item_name)
+#     end
+
+#     # Get the limits for a telemetry item
+#     #
+#     # @param target_name [String] Target Name
+#     # @param packet_name [String] Packet Name
+#     # @param item_name [String] Item Name
+#     # @param limits_set [String or Symbol or nil] Desired Limits set.  nil = current limits set
+#     # @return [Array<limits_set, persistence, enabled, red_low, yellow_low, red_high, yellow_high, green_low (optional), green_high (optional)] Limits information
+#     def get(target_name, packet_name, item_name, limits_set = nil)
+#       limits = get_packet(target_name, packet_name).get_item(item_name).limits
+#       if limits.values
+#         if limits_set
+#           limits_set = limits_set.to_s.upcase.intern
+#         else
+#           limits_set = System.limits_set
+#         end
+#         limits_for_set = limits.values[limits_set]
+#         if limits_for_set
+#           return [limits_set, limits.persistence_setting, limits.enabled, limits_for_set[0], limits_for_set[1], limits_for_set[2], limits_for_set[3], limits_for_set[4], limits_for_set[5]]
+#         else
+#           return [nil, nil, nil, nil, nil, nil, nil, nil, nil]
+#         end
+#       else
+#         return [nil, nil, nil, nil, nil, nil, nil, nil, nil]
+#       end
+#     end
+
+#     # Set the limits for a telemetry item
+#     #
+#     # @param target_name [String] Target Name
+#     # @param packet_name [String] Packet Name
+#     # @param item_name [String] Item Name
+#     # @param red_low [Float] Red Low Limit
+#     # @param yellow_low [Float] Yellow Low Limit
+#     # @param yellow_high [Float] Yellow High Limit
+#     # @param red_high [Float] Red High Limit
+#     # @param green_low [Float] Green Low Limit
+#     # @param green_high [Float] Green High Limit
+#     # @param limits_set [String or Symbol or nil] Desired Limits set.  nil = current limits set, recommend using :CUSTOM
+#     # @param persistence [Integer] The number of samples the value must be out of limits before detecting a limits change. nil = Leave unchanged
+#     # @param enabled [Boolean] If limits monitoring is enabled for this item
+#     # @return [Array<limits_set, persistence, enabled, red_low, yellow_low, red_high, yellow_high, green_low (optional), green_high (optional)] Limits information
+#     def set(target_name, packet_name, item_name, red_low, yellow_low, yellow_high, red_high, green_low = nil, green_high = nil, limits_set = :CUSTOM, persistence = nil, enabled = true)
+#       packet = get_packet(target_name, packet_name)
+#       item = packet.get_item(item_name)
+#       limits = item.limits
+#       if limits_set
+#         limits_set = limits_set.to_s.upcase.intern
+#       else
+#         limits_set = System.limits_set
+#       end
+#       if !limits.values
+#         if limits_set == :DEFAULT
+#           limits.values = { :DEFAULT => [] }
+#         else
+#           raise "DEFAULT limits must be defined for #{target_name} #{packet_name} #{item_name} before setting limits set #{limits_set}"
+#         end
+#       end
+#       limits_for_set = limits.values[limits_set]
+#       unless limits_for_set
+#         limits.values[limits_set] = []
+#         limits_for_set = limits.values[limits_set]
+#       end
+#       limits_for_set[0] = red_low.to_f
+#       limits_for_set[1] = yellow_low.to_f
+#       limits_for_set[2] = yellow_high.to_f
+#       limits_for_set[3] = red_high.to_f
+#       limits_for_set.delete_at(5) if limits_for_set[5]
+#       limits_for_set.delete_at(4) if limits_for_set[4]
+#       if green_low && green_high
+#         limits_for_set[4] = green_low.to_f
+#         limits_for_set[5] = green_high.to_f
+#       end
+#       limits.enabled = enabled if not enabled.nil?
+#       limits.persistence_setting = Integer(persistence) if persistence
+#       packet.update_limits_items_cache(item)
+#       @config.limits_sets << limits_set
+#       @config.limits_sets.uniq!
+#       return [limits_set, limits.persistence_setting, limits.enabled, limits_for_set[0], limits_for_set[1], limits_for_set[2], limits_for_set[3], limits_for_set[4], limits_for_set[5]]
+#     end
+
+#     protected
+
+#     def get_packet(target_name, packet_name)
+#       raise "LATEST packet not valid" if packet_name.upcase == LATEST_PACKET_NAME
+
+#       packets = @config.telemetry[target_name.to_s.upcase]
+#       raise "Telemetry target '#{target_name.to_s.upcase}' does not exist" unless packets
+
+#       packet = packets[packet_name.to_s.upcase]
+#       raise "Telemetry packet '#{target_name.to_s.upcase} #{packet_name.to_s.upcase}' does not exist" unless packet
+
+#       return packet
+#     end
+
+#     def includes_item?(ignored_items, target_name, packet_name, item_name)
+#       ignored_items.each do |array_target_name, array_packet_name, array_item_name|
+#         if (array_target_name == target_name) &&
+#            (array_packet_name == packet_name) &&
+#            # If the item name is nil we're ignoring an entire packet
+#            (array_item_name == item_name || array_item_name.nil?)
+#           return true
+#         end
+#       end
+#       return false
+#     end
+#   end
+# end
```

### Comparing `openc3-5.16.0/openc3/packets/packet_config.py` & `openc3-5.9.2b0/openc3/packets/packet_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Copyright 2024 OpenC3, Inc.
+#!/usr/bin/env python3
+
+# Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 #
@@ -14,33 +16,14 @@
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import os
 from openc3.config.config_parser import ConfigParser
 from openc3.packets.packet import Packet
 from openc3.packets.parsers.packet_parser import PacketParser
-from openc3.packets.parsers.packet_item_parser import PacketItemParser
-from openc3.packets.parsers.state_parser import StateParser
-from openc3.packets.parsers.limits_parser import LimitsParser
-from openc3.packets.parsers.limits_response_parser import LimitsResponseParser
-from openc3.packets.parsers.format_string_parser import FormatStringParser
-from openc3.packets.parsers.processor_parser import ProcessorParser
-from openc3.conversions.generic_conversion import GenericConversion
-from openc3.conversions.polynomial_conversion import PolynomialConversion
-from openc3.conversions.segmented_polynomial_conversion import (
-    SegmentedPolynomialConversion,
-)
-from openc3.utilities.extract import convert_to_value
-from openc3.utilities.logger import Logger
-from openc3.utilities.string import (
-    filename_to_module,
-    filename_to_class_name,
-    class_name_to_filename,
-)
-from openc3.top_level import get_class_from_module
 
 
 class PacketConfig:
     COMMAND = "Command"
     TELEMETRY = "Telemetry"
 
     def __init__(self):
@@ -88,189 +71,154 @@
 
         self.converted_type = None
         self.converted_bit_size = None
         self.proc_text = ""
         self.building_generic_conversion = False
 
         process_target_name = process_target_name.upper()
-        parser = ConfigParser("https://docs.openc3.com/docs")
+        parser = ConfigParser("https://openc3.com/docs/v5")
         setattr(parser, "target_name", process_target_name)
         for keyword, params in parser.parse_file(filename):
-            if self.building_generic_conversion:
-                match keyword:
-                    # Complete a generic conversion
-                    case "GENERIC_READ_CONVERSION_END" | "GENERIC_WRITE_CONVERSION_END":
-                        parser.verify_num_parameters(0, 0, keyword)
-                        if "READ" in keyword:
-                            self.current_item.read_conversion = GenericConversion(
-                                self.proc_text,
-                                self.converted_type,
-                                self.converted_bit_size,
-                            )
-                        if "WRITE" in keyword:
-                            self.current_item.write_conversion = GenericConversion(
-                                self.proc_text,
-                                self.converted_type,
-                                self.converted_bit_size,
-                            )
-                        self.building_generic_conversion = False
-                    # Add the current config.line to the conversion being built
-                    case _:
-                        self.proc_text += parser.line + "\n"
-
-            else:  # not building generic conversion
-                match keyword:
-                    # Start a new packet
-                    case "COMMAND":
-                        self.finish_packet()
-                        self.current_packet = PacketParser.parse_command(
-                            parser, process_target_name, self.commands, self.warnings
-                        )
-                        self.current_cmd_or_tlm = PacketConfig.COMMAND
+            match keyword:
+                # Start a new packet
+                case "COMMAND":
+                    self.finish_packet()
+                    self.current_packet = PacketParser.parse_command(
+                        parser, process_target_name, self.commands, self.warnings
+                    )
+                    self.current_cmd_or_tlm = PacketConfig.COMMAND
 
-                    case "TELEMETRY":
-                        self.finish_packet()
-                        self.current_packet = PacketParser.parse_telemetry(
-                            parser,
-                            process_target_name,
-                            self.telemetry,
-                            self.latest_data,
-                            self.warnings,
-                        )
-                        self.current_cmd_or_tlm = PacketConfig.TELEMETRY
+                case "TELEMETRY":
+                    self.finish_packet()
+                    self.current_packet = PacketParser.parse_telemetry(
+                        parser,
+                        process_target_name,
+                        self.telemetry,
+                        self.latest_data,
+                        self.warnings,
+                    )
+                    self.current_cmd_or_tlm = PacketConfig.TELEMETRY
+
+                # Select an existing packet for editing
+                case "SELECT_COMMAND" | "SELECT_TELEMETRY":
+                    usage = f"{keyword} <TARGET NAME> <PACKET NAME>"
+                    self.finish_packet()
+                    parser.verify_num_parameters(2, 2, usage)
+                    target_name = process_target_name
+                    if target_name == "SYSTEM":
+                        target_name = params[0].upper()
+                    packet_name = params[1].upper()
 
-                    # Select an existing packet for editing
-                    case "SELECT_COMMAND" | "SELECT_TELEMETRY":
-                        usage = f"{keyword} <TARGET NAME> <PACKET NAME>"
-                        self.finish_packet()
-                        parser.verify_num_parameters(2, 2, usage)
-                        target_name = process_target_name
-                        if target_name == "SYSTEM":
-                            target_name = params[0].upper()
-                        packet_name = params[1].upper()
-
-                        self.current_packet = None
-                        if "COMMAND" in keyword:
-                            self.current_cmd_or_tlm = PacketConfig.COMMAND
-                            if self.commands.get(target_name):
-                                self.current_packet = self.commands[target_name][
-                                    packet_name
-                                ]
-                        else:
-                            self.current_cmd_or_tlm = PacketConfig.TELEMETRY
-                            if self.telemetry.get(target_name):
-                                self.current_packet = self.telemetry[target_name][
-                                    packet_name
-                                ]
-
-                        if not self.current_packet:
-                            raise parser.error("Packet not found", usage)
-
-                    # Start the creation of a new limits group
-                    case "LIMITS_GROUP":
-                        usage = "LIMITS_GROUP <GROUP NAME>"
-                        parser.verify_num_parameters(1, 1, usage)
-                        self.current_limits_group = params[0].upper()
-                        if self.current_limits_group not in self.limits_groups:
-                            self.limits_groups[self.current_limits_group] = []
-
-                    # Add a telemetry item to the limits group
-                    case "LIMITS_GROUP_ITEM":
-                        usage = (
-                            "LIMITS_GROUP_ITEM <TARGET NAME> <PACKET NAME> <ITEM NAME>"
+                    self.current_packet = None
+                    if "COMMAND" in keyword:
+                        self.current_cmd_or_tlm = PacketConfig.COMMAND
+                        if self.commands[target_name]:
+                            self.current_packet = self.commands[target_name][
+                                packet_name
+                            ]
+                    else:
+                        self.current_cmd_or_tlm = PacketConfig.TELEMETRY
+                        if self.telemetry[target_name]:
+                            self.current_packet = self.telemetry[target_name][
+                                packet_name
+                            ]
+
+                    if not self.current_packet:
+                        raise parser.error("Packet not found", usage)
+
+                # Start the creation of a new limits group
+                case "LIMITS_GROUP":
+                    usage = "LIMITS_GROUP <GROUP NAME>"
+                    parser.verify_num_parameters(1, 1, usage)
+                    self.current_limits_group = params[0].upper()
+                    if self.current_limits_group not in self.limits_groups:
+                        self.limits_groups[self.current_limits_group] = []
+
+                # Add a telemetry item to the limits group
+                case "LIMITS_GROUP_ITEM":
+                    usage = "LIMITS_GROUP_ITEM <TARGET NAME> <PACKET NAME> <ITEM NAME>"
+                    parser.verify_num_parameters(3, 3, usage)
+                    if self.current_limits_group:
+                        self.limits_groups[self.current_limits_group].append(
+                            [params[0].upper(), params[1].upper(), params[2].upper()]
                         )
-                        parser.verify_num_parameters(3, 3, usage)
-                        if self.current_limits_group:
-                            self.limits_groups[self.current_limits_group].append(
-                                [
-                                    params[0].upper(),
-                                    params[1].upper(),
-                                    params[2].upper(),
-                                ]
-                            )
-
-                    #######################################################################
-                    # All the following keywords must have a current packet defined
-                    #######################################################################
-                    case (
-                        "SELECT_ITEM"
-                        | "SELECT_PARAMETER"
-                        | "DELETE_ITEM"
-                        | "DELETE_PARAMETER"
-                        | "ITEM"
-                        | "PARAMETER"
-                        | "ID_ITEM"
-                        | "ID_PARAMETER"
-                        | "ARRAY_ITEM"
-                        | "ARRAY_PARAMETER"
-                        | "APPEND_ITEM"
-                        | "APPEND_PARAMETER"
-                        | "APPEND_ID_ITEM"
-                        | "APPEND_ID_PARAMETER"
-                        | "APPEND_ARRAY_ITEM"
-                        | "APPEND_ARRAY_PARAMETER"
-                        | "ALLOW_SHORT"
-                        | "HAZARDOUS"
-                        | "PROCESSOR"
-                        | "META"
-                        | "DISABLE_MESSAGES"
-                        | "HIDDEN"
-                        | "DISABLED"
-                        | "ACCESSOR"
-                        | "TEMPLATE"
-                        | "TEMPLATE_FILE"
-                        | "RESPONSE"
-                        | "ERROR_RESPONSE"
-                        | "SCREEN"
-                        | "RELATED_ITEM"
-                        | "IGNORE_OVERLAP"
-                    ):
-                        if not self.current_packet:
-                            raise parser.error(f"No current packet for {keyword}")
-                        self.process_current_packet(parser, keyword, params)
-
-                    #######################################################################
-                    # All the following keywords must have a current item defined
-                    #######################################################################
-                    case (
-                        "STATE"
-                        | "READ_CONVERSION"
-                        | "WRITE_CONVERSION"
-                        | "POLY_READ_CONVERSION"
-                        | "POLY_WRITE_CONVERSION"
-                        | "SEG_POLY_READ_CONVERSION"
-                        | "SEG_POLY_WRITE_CONVERSION"
-                        | "GENERIC_READ_CONVERSION_START"
-                        | "GENERIC_WRITE_CONVERSION_START"
-                        | "REQUIRED"
-                        | "LIMITS"
-                        | "LIMITS_RESPONSE"
-                        | "UNITS"
-                        | "FORMAT_STRING"
-                        | "DESCRIPTION"
-                        | "MINIMUM_VALUE"
-                        | "MAXIMUM_VALUE"
-                        | "DEFAULT_VALUE"
-                        | "OVERFLOW"
-                        | "OVERLAP"
-                        | "KEY"
-                    ):
-                        if not self.current_item:
-                            raise parser.error(f"No current item for {keyword}")
-                        self.process_current_item(parser, keyword, params)
-
-                    case _:
-                        # blank config.lines will have a None keyword and should not raise an exception
-                        if keyword:
-                            raise parser.error(f"Unknown keyword '{keyword}'")
+
+                #######################################################################
+                # All the following keywords must have a current packet defined
+                #######################################################################
+                case (
+                    "SELECT_ITEM"
+                    | "SELECT_PARAMETER"
+                    | "DELETE_ITEM"
+                    | "DELETE_PARAMETER"
+                    | "ITEM"
+                    | "PARAMETER"
+                    | "ID_ITEM"
+                    | "ID_PARAMETER"
+                    | "ARRAY_ITEM"
+                    | "ARRAY_PARAMETER"
+                    | "APPEND_ITEM"
+                    | "APPEND_PARAMETER"
+                    | "APPEND_ID_ITEM"
+                    | "APPEND_ID_PARAMETER"
+                    | "APPEND_ARRAY_ITEM"
+                    | "APPEND_ARRAY_PARAMETER"
+                    | "ALLOW_SHORT"
+                    | "HAZARDOUS"
+                    | "PROCESSOR"
+                    | "META"
+                    | "DISABLE_MESSAGES"
+                    | "HIDDEN"
+                    | "DISABLED"
+                    | "ACCESSOR"
+                    | "TEMPLATE"
+                    | "TEMPLATE_FILE"
+                ):
+                    if not self.current_packet:
+                        raise parser.error(f"No current packet for {keyword}")
+                    self.process_current_packet(parser, keyword, params)
+
+                #######################################################################
+                # All the following keywords must have a current item defined
+                #######################################################################
+                case (
+                    "STATE"
+                    | "READ_CONVERSION"
+                    | "WRITE_CONVERSION"
+                    | "POLY_READ_CONVERSION"
+                    | "POLY_WRITE_CONVERSION"
+                    | "SEG_POLY_READ_CONVERSION"
+                    | "SEG_POLY_WRITE_CONVERSION"
+                    | "GENERIC_READ_CONVERSION_START"
+                    | "GENERIC_WRITE_CONVERSION_START"
+                    | "REQUIRED"
+                    | "LIMITS"
+                    | "LIMITS_RESPONSE"
+                    | "UNITS"
+                    | "FORMAT_STRING"
+                    | "DESCRIPTION"
+                    | "MINIMUM_VALUE"
+                    | "MAXIMUM_VALUE"
+                    | "DEFAULT_VALUE"
+                    | "OVERFLOW"
+                    | "OVERLAP"
+                    | "KEY"
+                ):
+                    if not self.current_item:
+                        raise parser.error(f"No current item for {keyword}")
+                    self.process_current_item(parser, keyword, params)
+
+                case _:
+                    # blank config.lines will have a None keyword and should not raise an exception
+                    if keyword:
+                        raise parser.error(f"Unknown keyword '{keyword}'")
 
         # Complete the last defined packet
         self.finish_packet()
 
-    # TODO: Used in xtce conversion
     # # Convert the PacketConfig back to OpenC3 configuration files for each target
     # def to_config(output_dir)
     #   FileUtils.mkdir_p(output_dir)
 
     #   self.telemetry.each do |target_name, packets|
     #     next if target_name == 'UNKNOWN'
 
@@ -298,15 +246,15 @@
 
     #     packets.each do |packet_name, packet|
     #       File.open(filename, 'a') do |file|
     #         file.puts packet.to_config(:COMMAND)
     #         file.puts ""
 
     #   # Put limits groups into SYSTEM target
-    #   if len(self.limits_groups) > 0
+    #   if self.limits_groups.length > 0
     #     FileUtils.mkdir_p(File.join(output_dir, 'SYSTEM', 'cmd_tlm'))
     #     filename = File.join(output_dir, 'SYSTEM', 'cmd_tlm', 'limits_groups.txt')
     #     File.open(filename, 'w') do |file|
     #       self.limits_groups.each do |limits_group_name, limits_group_items|
     #         file.puts "LIMITS_GROUP {limits_group_name.quote_if_necessary}"
     #         limits_group_items.each do |target_name, packet_name, item_name|
     #           file.puts "  LIMITS_GROUP_ITEM {target_name.quote_if_necessary} {packet_name.quote_if_necessary} {item_name.quote_if_necessary}"
@@ -314,451 +262,328 @@
     #         file.puts ""
 
     #  # def to_config
 
     # def to_xtce(output_dir)
     #   XtceConverter.convert(self.commands, self.telemetry, output_dir)
 
-    # Add current packet into hash if it exists
-    def finish_packet(self):
-        self.finish_item()
-        if self.current_packet:
-            warnings = self.current_packet.check_bit_offsets()
-            if len(warnings) > 0:
-                self.warnings += warnings
-            if self.current_cmd_or_tlm == PacketConfig.COMMAND:
-                PacketParser.check_item_data_types(self.current_packet)
-                self.commands[self.current_packet.target_name][
-                    self.current_packet.packet_name
-                ] = self.current_packet
-                hash = self.cmd_id_value_hash.get(self.current_packet.target_name)
-                if not hash:
-                    hash = {}
-                self.cmd_id_value_hash[self.current_packet.target_name] = hash
-                self.update_id_value_hash(hash)
-            else:
-                self.telemetry[self.current_packet.target_name][
-                    self.current_packet.packet_name
-                ] = self.current_packet
-                hash = self.tlm_id_value_hash.get(self.current_packet.target_name)
-                if not hash:
-                    hash = {}
-                self.tlm_id_value_hash[self.current_packet.target_name] = hash
-                self.update_id_value_hash(hash)
-
-            self.current_packet = None
-            self.current_item = None
-
-    def update_id_value_hash(self, hash):
-        if self.current_packet.id_items and len(self.current_packet.id_items) > 0:
-            key = []
-            for item in self.current_packet.id_items:
-                key.append(item.id_value)
-
-            hash[repr(key)] = self.current_packet
-        else:
-            hash["CATCHALL"] = self.current_packet
-
-    def reset_processing_variables(self):
-        self.current_cmd_or_tlm = None
-        self.current_packet = None
-        self.current_item = None
-        self.current_limits_group = None
-
-    def process_current_packet(self, parser, keyword, params):
-        match keyword:
-            # Select or delete an item in the current packet
-            case (
-                "SELECT_PARAMETER" | "SELECT_ITEM" | "DELETE_PARAMETER" | "DELETE_ITEM"
-            ):
-                if (self.current_cmd_or_tlm == PacketConfig.COMMAND) and (
-                    keyword.split("_")[1] == "ITEM"
-                ):
-                    raise parser.error(f"{keyword} only applies to telemetry packets")
-                if (self.current_cmd_or_tlm == PacketConfig.TELEMETRY) and (
-                    keyword.split("_")[1] == "PARAMETER"
-                ):
-                    raise parser.error(f"{keyword} only applies to command packets")
-
-                usage = f"{keyword} <{keyword.split('_')[1]} NAME>"
-                self.finish_item()
-                parser.verify_num_parameters(1, 1, usage)
-                try:
-                    if "SELECT" in keyword:
-                        self.current_item = self.current_packet.get_item(params[0])
-                    else:  # DELETE
-                        self.current_packet.delete_item(params[0])
-                except (
-                    AttributeError
-                ):  # Rescue the default execption to provide a nicer error message
-                    raise parser.error(
-                        f"{params[0]} not found in {self.current_cmd_or_tlm.lower()} packet {self.current_packet.target_name} {self.current_packet.packet_name}",
-                        usage,
-                    )
-
-            # Start a new telemetry item in the current packet
-            case (
-                "ITEM"
-                | "PARAMETER"
-                | "ID_ITEM"
-                | "ID_PARAMETER"
-                | "ARRAY_ITEM"
-                | "ARRAY_PARAMETER"
-                | "APPEND_ITEM"
-                | "APPEND_PARAMETER"
-                | "APPEND_ID_ITEM"
-                | "APPEND_ID_PARAMETER"
-                | "APPEND_ARRAY_ITEM"
-                | "APPEND_ARRAY_PARAMETER"
-            ):
-                self.start_item(parser)
-
-            # Allow this packet to be received with less data than the defined length
-            # without generating a warning.
-            case "ALLOW_SHORT":
-                self.current_packet.short_buffer_allowed = True
-
-            # Mark the current command as hazardous
-            case "HAZARDOUS":
-                usage = "HAZARDOUS <HAZARDOUS DESCRIPTION (Optional)>"
-                parser.verify_num_parameters(0, 1, usage)
-                self.current_packet.hazardous = True
-                if len(params) == 1:
-                    self.current_packet.hazardous_description = params[0]
-
-            # Define a processor class that will be called once case a packet is received
-            case "PROCESSOR":
-                ProcessorParser.parse(
-                    parser, self.current_packet, self.current_cmd_or_tlm
-                )
-
-            case "DISABLE_MESSAGES":
-                usage = keyword
-                parser.verify_num_parameters(0, 0, usage)
-                self.current_packet.messages_disabled = True
-
-            # Store user defined metadata for the packet or a packet item
-            case "META":
-                usage = "META <META NAME> <META VALUES (optional)>"
-                parser.verify_num_parameters(1, None, usage)
-                if len(params) > 1:
-                    meta_values = params[1:]
-                else:
-                    meta_values = []
-                for index, value in enumerate(meta_values):
-                    if type(value) is str:
-                        meta_values[index] = value
-                if self.current_item:
-                    # Item META
-                    self.current_item.meta[params[0].upper()] = meta_values
-                else:
-                    # Packet META
-                    self.current_packet.meta[params[0].upper()] = meta_values
-
-            case "HIDDEN":
-                usage = keyword
-                parser.verify_num_parameters(0, 0, usage)
-                self.current_packet.hidden = True
-
-            case "DISABLED":
-                usage = keyword
-                parser.verify_num_parameters(0, 0, usage)
-                self.current_packet.hidden = True
-                self.current_packet.disabled = True
-
-            case "ACCESSOR":
-                usage = f"{keyword} <Accessor class name>"
-                parser.verify_num_parameters(1, None, usage)
-                try:
-                    filename = class_name_to_filename(params[0])
-                    klass = get_class_from_module(
-                        f"openc3.accessors.{filename}", params[0]
-                    )
-                    if len(params) > 1:
-                        self.current_packet.accessor = klass(
-                            self.current_packet, *params[1:]
-                        )
-                    else:
-                        self.current_packet.accessor = klass(self.current_packet)
-                except ModuleNotFoundError as error:
-                    raise parser.error(error)
-
-            case "TEMPLATE":
-                usage = f"{keyword} <Template string>"
-                parser.verify_num_parameters(1, 1, usage)
-                self.current_packet.template = params[0]
-
-            case "TEMPLATE_FILE":
-                usage = f"{keyword} <Template file path>"
-                parser.verify_num_parameters(1, 1, usage)
-
-                try:
-                    self.current_packet.template = parser.read_file(params[0])
-                except RuntimeError as error:
-                    raise parser.error(error)
-
-            case "RESPONSE":
-                usage = f"{keyword} <Target Name> <Packet Name>"
-                parser.verify_num_parameters(2, 2, usage)
-                if self.current_cmd_or_tlm == PacketConfig.TELEMETRY:
-                    raise parser.error(f"{keyword} only applies to command packets")
-                self.current_packet.response = [params[0].upper(), params[1].upper()]
-
-            case "ERROR_RESPONSE":
-                usage = f"{keyword} <Target Name> <Packet Name>"
-                parser.verify_num_parameters(2, 2, usage)
-                if self.current_cmd_or_tlm == PacketConfig.TELEMETRY:
-                    raise parser.error(f"{keyword} only applies to command packets")
-                self.current_packet.error_response = [
-                    params[0].upper(),
-                    params[1].upper(),
-                ]
-
-            case "SCREEN":
-                usage = f"{keyword} <Target Name> <Screen Name>"
-                parser.verify_num_parameters(2, 2, usage)
-                if self.current_cmd_or_tlm == PacketConfig.TELEMETRY:
-                    raise parser.error(f"{keyword} only applies to command packets")
-                self.current_packet.screen = [params[0].upper(), params[1].upper()]
-
-            case "RELATED_ITEM":
-                usage = f"{keyword} <Target Name> <Packet Name> <Item Name>"
-                parser.verify_num_parameters(3, 3, usage)
-                if self.current_cmd_or_tlm == PacketConfig.TELEMETRY:
-                    raise parser.error(f"{keyword} only applies to command packets")
-                if not self.current_packet.related_items:
-                    self.current_packet.related_items = []
-                self.current_packet.related_items.append(
-                    [params[0].upper(), params[1].upper(), params[2].upper()]
-                )
-
-            case "IGNORE_OVERLAP":
-                usage = f"{keyword}"
-                parser.verify_num_parameters(0, 0, usage)
-                self.current_packet.ignore_overlap = True
-
-    def process_current_item(self, parser, keyword, params):
-        match keyword:
-            # Add a state to the current telemety item
-            case "STATE":
-                StateParser.parse(
-                    parser,
-                    self.current_packet,
-                    self.current_cmd_or_tlm,
-                    self.current_item,
-                    self.warnings,
-                )
-
-            # Apply a conversion to the current item after it is read to or
-            # written from the packet
-            case "READ_CONVERSION" | "WRITE_CONVERSION":
-                usage = f"{keyword} <conversion class filename> <custom parameters> ..."
-                parser.verify_num_parameters(1, None, usage)
-                try:
-                    klass = get_class_from_module(
-                        filename_to_module(params[0]),
-                        filename_to_class_name(params[0]),
-                    )
-                    conversion = klass(*params[1:])
-                    if "READ" in keyword:
-                        self.current_item.read_conversion = conversion
-                    else:
-                        self.current_item.write_conversion = conversion
-                    # if klass != ProcessorConversion and (conversion.converted_type.None? or conversion.converted_bit_size.None?):
-                    #     msg = f"Read Conversion {params[0]} on item {self.current_item.name} does not specify converted type or bit size"
-                    #     self.warnings.append(msg)
-                    #     Logger.warn(self.warnings[-1])
-                except Exception as error:
-                    raise parser.error(error)
-
-            # Apply a polynomial conversion to the current item
-            case "POLY_READ_CONVERSION" | "POLY_WRITE_CONVERSION":
-                usage = f"{keyword} <C0> <C1> <C2> ..."
-                parser.verify_num_parameters(1, None, usage)
-                if "READ" in keyword:
-                    self.current_item.read_conversion = PolynomialConversion(*params)
-                else:
-                    self.current_item.write_conversion = PolynomialConversion(*params)
-
-            # Apply a segmented polynomial conversion to the current item
-            # after it is read from the telemetry packet
-            case "SEG_POLY_READ_CONVERSION":
-                usage = "SEG_POLY_READ_CONVERSION <Lower Bound> <C0> <C1> <C2> ..."
-                parser.verify_num_parameters(2, None, usage)
-                if (
-                    self.current_item.read_conversion is None
-                    or self.current_item.read_conversion.__class__
-                    != SegmentedPolynomialConversion
-                ):
-                    self.current_item.read_conversion = SegmentedPolynomialConversion()
-                self.current_item.read_conversion.add_segment(
-                    float(params[0]), *params[1:]
-                )
-
-            # Apply a segmented polynomial conversion to the current item
-            # before it is written to the telemetry packet
-            case "SEG_POLY_WRITE_CONVERSION":
-                usage = "SEG_POLY_WRITE_CONVERSION <Lower Bound> <C0> <C1> <C2> ..."
-                parser.verify_num_parameters(2, None, usage)
-                if (
-                    self.current_item.write_conversion is None
-                    or self.current_item.write_conversion.__class__
-                    != SegmentedPolynomialConversion
-                ):
-                    self.current_item.write_conversion = SegmentedPolynomialConversion()
-                self.current_item.write_conversion.add_segment(
-                    float(params[0]), *params[1:]
-                )
-
-            # Start the definition of a generic conversion.
-            # All config.lines following this config.line are considered part
-            # of the conversion until an end of conversion marker is found
-            case "GENERIC_READ_CONVERSION_START" | "GENERIC_WRITE_CONVERSION_START":
-                usage = f"{keyword} <Converted Type (optional)> <Converted Bit Size (optional)>"
-                parser.verify_num_parameters(0, 2, usage)
-                self.proc_text = ""
-                self.building_generic_conversion = True
-                self.converted_type = None
-                self.converted_bit_size = None
-                if len(params) == 2:
-                    self.converted_type = params[0].upper()
-                    if self.converted_type not in [
-                        "INT",
-                        "UINT",
-                        "FLOAT",
-                        "STRING",
-                        "BLOCK",
-                    ]:
-                        raise parser.error(
-                            f"Invalid converted_type: {self.converted_type}."
-                        )
-                    self.converted_bit_size = int(params[1])
-                if self.converted_type is None or self.converted_bit_size is None:
-                    msg = f"Generic Conversion on item {self.current_item.name} does not specify converted type or bit size"
-                    self.warnings.append(msg)
-                    Logger.warn(self.warnings[-1])
-
-            # Define a set of limits for the current telemetry item
-            case "LIMITS":
-                self.limits_sets.append(
-                    LimitsParser.parse(
-                        parser,
-                        self.current_packet,
-                        self.current_cmd_or_tlm,
-                        self.current_item,
-                        self.warnings,
-                    )
-                )
-                self.limits_sets = list(set(self.limits_sets))
-
-            # Define a response class that will be called case the limits state of the:
-            # current item changes.
-            case "LIMITS_RESPONSE":
-                LimitsResponseParser.parse(
-                    parser, self.current_item, self.current_cmd_or_tlm
-                )
-
-            # Define a printf style formatting string for the current telemetry item
-            case "FORMAT_STRING":
-                FormatStringParser.parse(parser, self.current_item)
-
-            # Define the units of the current telemetry item
-            case "UNITS":
-                usage = "UNITS <FULL UNITS NAME> <ABBREVIATED UNITS NAME>"
-                parser.verify_num_parameters(2, 2, usage)
-                self.current_item.units_full = params[0]
-                self.current_item.units = params[1]
-
-            # Update the description for the current telemetry item
-            case "DESCRIPTION":
-                usage = "DESCRIPTION <DESCRIPTION>"
-                parser.verify_num_parameters(1, 1, usage)
-                self.current_item.description = params[0]
-
-            # Mark the current command parameter as required.
-            # This means it must be given a value and not just use its default.
-            case "REQUIRED":
-                usage = "REQUIRED"
-                parser.verify_num_parameters(0, 0, usage)
-                if self.current_cmd_or_tlm == PacketConfig.COMMAND:
-                    self.current_item.required = True
-                else:
-                    raise parser.error(f"{keyword} only applies to command parameters")
-
-            # Update the mimimum value for the current command parameter
-            case "MINIMUM_VALUE":
-                if self.current_cmd_or_tlm == PacketConfig.TELEMETRY:
-                    raise parser.error(f"{keyword} only applies to command parameters")
-
-                usage = "MINIMUM_VALUE <MINIMUM VALUE>"
-                parser.verify_num_parameters(1, 1, usage)
-                min = ConfigParser.handle_defined_constants(
-                    convert_to_value(params[0]),
-                    self.current_item.data_type,
-                    self.current_item.bit_size,
-                )
-                self.current_item.minimum = min
-
-            # Update the maximum value for the current command parameter
-            case "MAXIMUM_VALUE":
-                if self.current_cmd_or_tlm == PacketConfig.TELEMETRY:
-                    raise parser.error(f"{keyword} only applies to command parameters")
-
-                usage = "MAXIMUM_VALUE <MAXIMUM VALUE>"
-                parser.verify_num_parameters(1, 1, usage)
-                max = ConfigParser.handle_defined_constants(
-                    convert_to_value(params[0]),
-                    self.current_item.data_type,
-                    self.current_item.bit_size,
-                )
-                self.current_item.maximum = max
-
-            # Update the default value for the current command parameter
-            case "DEFAULT_VALUE":
-                if self.current_cmd_or_tlm == PacketConfig.TELEMETRY:
-                    raise parser.error(f"{keyword} only applies to command parameters")
-
-                usage = "DEFAULT_VALUE <DEFAULT VALUE>"
-                parser.verify_num_parameters(1, 1, usage)
-                if (self.current_item.data_type == "STRING") or (
-                    self.current_item.data_type == "BLOCK"
-                ):
-                    self.current_item.default = params[0]
-                else:
-                    self.current_item.default = ConfigParser.handle_defined_constants(
-                        convert_to_value(params[0]),
-                        self.current_item.data_type,
-                        self.current_item.bit_size,
-                    )
+    # # Add current packet into hash if it exists
+    # def finish_packet
+    #   finish_item()
+    #   if self.current_packet
+    #     self.warnings += self.current_packet.check_bit_offsets
+    #     if self.current_cmd_or_tlm == COMMAND
+    #       PacketParser.check_item_data_types(self.current_packet)
+    #       self.commands[self.current_packet.target_name][self.current_packet.packet_name] = self.current_packet
+    #       hash = self.cmd_id_value_hash[self.current_packet.target_name]
+    #       hash = {} unless hash
+    #       self.cmd_id_value_hash[self.current_packet.target_name] = hash
+    #       update_id_value_hash(hash)
+    #     else
+    #       self.telemetry[self.current_packet.target_name][self.current_packet.packet_name] = self.current_packet
+    #       hash = self.tlm_id_value_hash[self.current_packet.target_name]
+    #       hash = {} unless hash
+    #       self.tlm_id_value_hash[self.current_packet.target_name] = hash
+    #       update_id_value_hash(hash)
+
+    #     self.current_packet = None
+    #     self.current_item = None
+
+    # protected
+
+    # def update_id_value_hash(hash)
+    #   if self.current_packet.id_items.length > 0
+    #     key = []
+    #     self.current_packet.id_items.each do |item|
+    #       key << item.id_value
+
+    #     hash[key] = self.current_packet
+    #   else
+    #     hash['CATCHALL'.freeze] = self.current_packet
+
+    # def reset_processing_variables
+    #   self.current_cmd_or_tlm = None
+    #   self.current_packet = None
+    #   self.current_item = None
+    #   self.current_limits_group = None
+
+    # def process_current_packet(parser, keyword, params)
+    #   case keyword
+
+    #   # Select or delete an item in the current packet
+    #   when 'SELECT_PARAMETER', 'SELECT_ITEM', 'DELETE_PARAMETER', 'DELETE_ITEM'
+    #     if (self.current_cmd_or_tlm == COMMAND) && (keyword.split('_')[1] == 'ITEM')
+    #       raise parser.error("{keyword} only applies to telemetry packets")
+
+    #     if (self.current_cmd_or_tlm == TELEMETRY) && (keyword.split('_')[1] == 'PARAMETER')
+    #       raise parser.error("{keyword} only applies to command packets")
+
+    #     usage = "{keyword} <{keyword.split('_')[1]} NAME>"
+    #     finish_item()
+    #     parser.verify_num_parameters(1, 1, usage)
+    #     begin
+    #       if keyword.include?("SELECT")
+    #         self.current_item = self.current_packet.get_item(params[0])
+    #       else # DELETE
+    #         self.current_packet.delete_item(params[0])
+
+    #     rescue # Rescue the default execption to provide a nicer error message
+    #       raise parser.error("{params[0]} not found in {self.current_cmd_or_tlm.downcase} packet {self.current_packet.target_name} {self.current_packet.packet_name}", usage)
+
+    #   # Start a new telemetry item in the current packet
+    #   when 'ITEM', 'PARAMETER', 'ID_ITEM', 'ID_PARAMETER', 'ARRAY_ITEM', 'ARRAY_PARAMETER',\
+    #       'APPEND_ITEM', 'APPEND_PARAMETER', 'APPEND_ID_ITEM', 'APPEND_ID_PARAMETER',\
+    #       'APPEND_ARRAY_ITEM', 'APPEND_ARRAY_PARAMETER'
+    #     start_item(parser)
+
+    #   # Allow this packet to be received with less data than the defined length
+    #   # without generating a warning.
+    #   when 'ALLOW_SHORT'
+    #     self.current_packet.short_buffer_allowed = True
+
+    #   # Mark the current command as hazardous
+    #   when 'HAZARDOUS'
+    #     usage = "HAZARDOUS <HAZARDOUS DESCRIPTION (Optional)>"
+    #     parser.verify_num_parameters(0, 1, usage)
+    #     self.current_packet.hazardous = True
+    #     self.current_packet.hazardous_description = params[0] if params[0]
+
+    #   # Define a processor class that will be called once when a packet is received
+    #   when 'PROCESSOR'
+    #     ProcessorParser.parse(parser, self.current_packet, self.current_cmd_or_tlm)
+
+    #   when 'DISABLE_MESSAGES'
+    #     usage = "{keyword}"
+    #     parser.verify_num_parameters(0, 0, usage)
+    #     self.current_packet.messages_disabled = True
+
+    #   # Store user defined metadata for the packet or a packet item
+    #   when 'META'
+    #     usage = "META <META NAME> <META VALUES (optional)>"
+    #     parser.verify_num_parameters(1, None, usage)
+    #     if params.length > 1
+    #       meta_values = params[1..-1]
+    #     else
+    #       meta_values = []
+
+    #     meta_values.each_with_index do |value, index|
+    #       if String === value
+    #         meta_values[index] = value.to_utf8
+
+    #     if self.current_item
+    #       # Item META
+    #       self.current_item.meta[params[0].upper()] = meta_values
+    #     else
+    #       # Packet META
+    #       self.current_packet.meta[params[0].upper()] = meta_values
+
+    #   when 'HIDDEN'
+    #     usage = "{keyword}"
+    #     parser.verify_num_parameters(0, 0, usage)
+    #     self.current_packet.hidden = True
+
+    #   when 'DISABLED'
+    #     usage = "{keyword}"
+    #     parser.verify_num_parameters(0, 0, usage)
+    #     self.current_packet.hidden = True
+    #     self.current_packet.disabled = True
+    #   when 'ACCESSOR'
+    #     usage = "{keyword} <Accessor class name>"
+    #     parser.verify_num_parameters(1, 1, usage)
+    #     begin
+    #       klass = OpenC3.require_class(params[0])
+    #       self.current_packet.accessor = klass
+    #     rescue Exception => err
+    #       raise parser.error(err)
+
+    #   when 'TEMPLATE'
+    #     usage = "{keyword} <Template string>"
+    #     parser.verify_num_parameters(1, 1, usage)
+    #     self.current_packet.template = params[0]
+
+    #   when 'TEMPLATE_FILE'
+    #     usage = "{keyword} <Template file path>"
+    #     parser.verify_num_parameters(1, 1, usage)
 
-            # Update the overflow type for the current command parameter
-            case "OVERFLOW":
-                usage = "OVERFLOW <OVERFLOW VALUE - ERROR, ERROR_ALLOW_HEX, TRUNCATE, or SATURATE>"
-                parser.verify_num_parameters(1, 1, usage)
-                self.current_item.overflow = params[0].upper()
-
-            case "OVERLAP":
-                parser.verify_num_parameters(0, 0, "OVERLAP")
-                self.current_item.overlap = True
-
-            case "KEY":
-                parser.verify_num_parameters(1, 1, "KEY <key or path into data>")
-                self.current_item.key = params[0]
-
-    def start_item(self, parser):
-        self.finish_item()
-        self.current_item = PacketItemParser.parse(
-            parser, self.current_packet, self.current_cmd_or_tlm, self.warnings
-        )
+    #     begin
+    #       self.current_packet.template = parser.read_file(params[0])
+    #     rescue Exception => err
+    #       raise parser.error(err)
+
+    # def process_current_item(parser, keyword, params)
+    #   case keyword
+
+    #   # Add a state to the current telemety item
+    #   when 'STATE'
+    #     StateParser.parse(parser, self.current_packet, self.current_cmd_or_tlm, self.current_item, self.warnings)
+
+    #   # Apply a conversion to the current item after it is read to or
+    #   # written from the packet
+    #   when 'READ_CONVERSION', 'WRITE_CONVERSION'
+    #     usage = "{keyword} <conversion class filename> <custom parameters> ..."
+    #     parser.verify_num_parameters(1, None, usage)
+    #     begin
+    #       klass = OpenC3.require_class(params[0])
+    #       conversion = klass.new(*params[1..(params.length - 1)])
+    #       self.current_item.public_send("{keyword.downcase}=".to_sym, conversion)
+    #       if klass != ProcessorConversion and (conversion.converted_type.None? or conversion.converted_bit_size.None?)
+    #         msg = "Read Conversion {params[0]} on item {self.current_item.name} does not specify converted type or bit size"
+    #         self.warnings << msg
+    #         Logger.instance.warn self.warnings[-1]
+
+    #     rescue Exception => err
+    #       raise parser.error(err)
+
+    #   # Apply a polynomial conversion to the current item
+    #   when 'POLY_READ_CONVERSION', 'POLY_WRITE_CONVERSION'
+    #     usage = "{keyword} <C0> <C1> <C2> ..."
+    #     parser.verify_num_parameters(1, None, usage)
+    #     self.current_item.read_conversion = PolynomialConversion.new(*params) if keyword.include? "READ"
+    #     self.current_item.write_conversion = PolynomialConversion.new(*params) if keyword.include? "WRITE"
+
+    #   # Apply a segmented polynomial conversion to the current item
+    #   # after it is read from the telemetry packet
+    #   when 'SEG_POLY_READ_CONVERSION'
+    #     usage = "SEG_POLY_READ_CONVERSION <Lower Bound> <C0> <C1> <C2> ..."
+    #     parser.verify_num_parameters(2, None, usage)
+    #     if !(self.current_item.read_conversion &&
+    #          SegmentedPolynomialConversion === self.current_item.read_conversion)
+    #       self.current_item.read_conversion = SegmentedPolynomialConversion.new
+
+    #     self.current_item.read_conversion.add_segment(params[0].to_f, *params[1..-1])
+
+    #   # Apply a segmented polynomial conversion to the current item
+    #   # before it is written to the telemetry packet
+    #   when 'SEG_POLY_WRITE_CONVERSION'
+    #     usage = "SEG_POLY_WRITE_CONVERSION <Lower Bound> <C0> <C1> <C2> ..."
+    #     parser.verify_num_parameters(2, None, usage)
+    #     if !(self.current_item.write_conversion &&
+    #          SegmentedPolynomialConversion === self.current_item.write_conversion)
+    #       self.current_item.write_conversion = SegmentedPolynomialConversion.new
+
+    #     self.current_item.write_conversion.add_segment(params[0].to_f, *params[1..-1])
+
+    #   # Start the definition of a generic conversion.
+    #   # All config.lines following this config.line are considered part
+    #   # of the conversion until an  of conversion marker is found
+    #   when 'GENERIC_READ_CONVERSION_START', 'GENERIC_WRITE_CONVERSION_START'
+    #     usage = "{keyword} <Converted Type (optional)> <Converted Bit Size (optional)>"
+    #     parser.verify_num_parameters(0, 2, usage)
+    #     self.proc_text = ''
+    #     self.building_generic_conversion = True
+    #     self.converted_type = None
+    #     self.converted_bit_size = None
+    #     if params[0]
+    #       self.converted_type = params[0].upper().intern
+    #       raise parser.error("Invalid converted_type: {self.converted_type}.") unless [:INT, :UINT, :FLOAT, :STRING, :BLOCK, :RUBY_TIME].include? self.converted_type
+
+    #     self.converted_bit_size = Integer(params[1]) if params[1]
+    #     if self.converted_type.None? or self.converted_bit_size.None?
+    #       msg = "Generic Conversion on item {self.current_item.name} does not specify converted type or bit size"
+    #       self.warnings << msg
+    #       Logger.instance.warn self.warnings[-1]
+
+    #   # Define a set of limits for the current telemetry item
+    #   when 'LIMITS'
+    #     self.limits_sets << LimitsParser.parse(parser, self.current_packet, self.current_cmd_or_tlm, self.current_item, self.warnings)
+    #     self.limits_sets.uniq!
+
+    #   # Define a response class that will be called when the limits state of the
+    #   # current item changes.
+    #   when 'LIMITS_RESPONSE'
+    #     LimitsResponseParser.parse(parser, self.current_item, self.current_cmd_or_tlm)
+
+    #   # Define a printf style formatting string for the current telemetry item
+    #   when 'FORMAT_STRING'
+    #     FormatStringParser.parse(parser, self.current_item)
+
+    #   # Define the units of the current telemetry item
+    #   when 'UNITS'
+    #     usage = "UNITS <FULL UNITS NAME> <ABBREVIATED UNITS NAME>"
+    #     parser.verify_num_parameters(2, 2, usage)
+    #     self.current_item.units_full = params[0]
+    #     self.current_item.units = params[1]
+
+    #   # Update the description for the current telemetry item
+    #   when 'DESCRIPTION'
+    #     usage = "DESCRIPTION <DESCRIPTION>"
+    #     parser.verify_num_parameters(1, 1, usage)
+    #     self.current_item.description = params[0]
+
+    #   # Mark the current command parameter as required.
+    #   # This means it must be given a value and not just use its default.
+    #   when 'REQUIRED'
+    #     usage = "REQUIRED"
+    #     parser.verify_num_parameters(0, 0, usage)
+    #     if self.current_cmd_or_tlm == COMMAND
+    #       self.current_item.required = True
+    #     else
+    #       raise parser.error("{keyword} only applies to command parameters")
+
+    #   # Update the mimimum value for the current command parameter
+    #   when 'MINIMUM_VALUE'
+    #     if self.current_cmd_or_tlm == TELEMETRY
+    #       raise parser.error("{keyword} only applies to command parameters")
+
+    #     usage = "MINIMUM_VALUE <MINIMUM VALUE>"
+    #     parser.verify_num_parameters(1, 1, usage)
+    #     min = ConfigParser.handle_defined_constants(
+    #       params[0].convert_to_value, self.current_item.data_type, self.current_item.bit_size
+    #     )
+    #     self.current_item.range = Range.new(min, self.current_item.range.)
+
+    #   # Update the maximum value for the current command parameter
+    #   when 'MAXIMUM_VALUE'
+    #     if self.current_cmd_or_tlm == TELEMETRY
+    #       raise parser.error("{keyword} only applies to command parameters")
+
+    #     usage = "MAXIMUM_VALUE <MAXIMUM VALUE>"
+    #     parser.verify_num_parameters(1, 1, usage)
+    #     max = ConfigParser.handle_defined_constants(
+    #       params[0].convert_to_value, self.current_item.data_type, self.current_item.bit_size
+    #     )
+    #     self.current_item.range = Range.new(self.current_item.range.begin, max)
+
+    #   # Update the default value for the current command parameter
+    #   when 'DEFAULT_VALUE'
+    #     if self.current_cmd_or_tlm == TELEMETRY
+    #       raise parser.error("{keyword} only applies to command parameters")
+
+    #     usage = "DEFAULT_VALUE <DEFAULT VALUE>"
+    #     parser.verify_num_parameters(1, 1, usage)
+    #     if (self.current_item.data_type == :STRING) ||
+    #        (self.current_item.data_type == :BLOCK)
+    #       self.current_item.default = params[0]
+    #     else
+    #       self.current_item.default = ConfigParser.handle_defined_constants(
+    #         params[0].convert_to_value, self.current_item.data_type, self.current_item.bit_size
+    #       )
+
+    #   # Update the overflow type for the current command parameter
+    #   when 'OVERFLOW'
+    #     usage = "OVERFLOW <OVERFLOW VALUE - ERROR, ERROR_ALLOW_HEX, TRUNCATE, or SATURATE>"
+    #     parser.verify_num_parameters(1, 1, usage)
+    #     self.current_item.overflow = params[0].upper().intern
+
+    #   when 'OVERLAP'
+    #     parser.verify_num_parameters(0, 0, 'OVERLAP')
+    #     self.current_item.overlap = True
+
+    #   when 'KEY'
+    #     parser.verify_num_parameters(1, 1, 'KEY <key or path into data>')
+    #     self.current_item.key = params[0]
+
+    # def start_item(parser)
+    #   finish_item()
+    #   self.current_item = PacketItemParser.parse(parser, self.current_packet, self.current_cmd_or_tlm, self.warnings)
+
+    # # Finish updating packet item
+    # def finish_item
+    #   if self.current_item
+    #     self.current_packet.set_item(self.current_item)
+    #     if self.current_cmd_or_tlm == TELEMETRY
+    #       target_latest_data = self.latest_data[self.current_packet.target_name]
+    #       target_latest_data[self.current_item.name] ||= []
+    #       latest_data_packets = target_latest_data[self.current_item.name]
+    #       latest_data_packets << self.current_packet unless latest_data_packets.include?(self.current_packet)
 
-    # Finish updating packet item
-    def finish_item(self):
-        if self.current_item:
-            self.current_packet.set_item(self.current_item)
-            if self.current_cmd_or_tlm == PacketConfig.TELEMETRY:
-                target_latest_data = self.latest_data[self.current_packet.target_name]
-                if not target_latest_data.get(self.current_item.name):
-                    target_latest_data[self.current_item.name] = []
-                latest_data_packets = target_latest_data[self.current_item.name]
-                if self.current_packet not in latest_data_packets:
-                    latest_data_packets.append(self.current_packet)
-            self.current_item = None
+    #     self.current_item = None
```

### Comparing `openc3-5.16.0/openc3/packets/parsers/packet_parser.py` & `openc3-5.9.2b0/openc3/packets/parsers/packet_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -17,61 +19,61 @@
 from openc3.packets.packet import Packet
 from openc3.utilities.logger import Logger
 
 
 class PacketParser:
     @classmethod
     def parse_command(cls, parser, target_name, commands, warnings):
-        parser = PacketParser(parser)
+        parser = PacketParser.new(parser)
         parser.verify_parameters()
-        return parser.create_command(target_name, commands, warnings)
+        parser.create_command(target_name, commands, warnings)
 
     @classmethod
     def parse_telemetry(cls, parser, target_name, telemetry, latest_data, warnings):
-        parser = PacketParser(parser)
+        parser = PacketParser.new(parser)
         parser.verify_parameters()
-        return parser.create_telemetry(target_name, telemetry, latest_data, warnings)
+        parser.create_telemetry(target_name, telemetry, latest_data, warnings)
 
     @classmethod
     def check_item_data_types(cls, packet):
         try:
             for item in packet.sorted_items:
                 item.check_default_and_range_data_types()
 
-        except AttributeError as error:
+        except Exception as error:
             # Add the target name and packet name to the error message so the user
             # can debug where the error occurred
-            raise AttributeError(
-                f"{packet.target_name} {packet.packet_name} {error}"
+            raise Exception(
+                f"{packet.target_name} {packet.packet_name} {repr(error)}"
             ) from error
 
     @classmethod
     def _check_for_duplicate(cls, type, list, packet):
         msg = None
-        if list.get(packet.target_name):
-            if list[packet.target_name].get(packet.packet_name):
+        if list[packet.target_name]:
+            if list[packet.target_name][packet.packet_name]:
                 msg = f"{type} Packet {packet.target_name} {packet.packet_name} redefined."
                 Logger.warn(msg)
         return msg
 
     @classmethod
     def _finish_create_command(cls, packet, commands, warnings):
         warning = PacketParser._check_for_duplicate("Command", commands, packet)
         if warning:
-            warnings.append(warning)
+            warnings += warning
         packet.define_reserved_items()
         if not commands.get(packet.target_name):
             commands[packet.target_name] = {}
         return packet
 
     @classmethod
     def _finish_create_telemetry(cls, packet, telemetry, latest_data, warnings):
         warning = PacketParser._check_for_duplicate("Telemetry", telemetry, packet)
         if warning:
-            warnings.append(warning)
+            warnings += warning
         packet.define_reserved_items()
 
         if not telemetry.get(packet.target_name):
             telemetry[packet.target_name] = {}
             latest_data[packet.target_name] = {}
         return packet
 
@@ -81,31 +83,26 @@
     def verify_parameters(self):
         self.usage = f"{self.parser.keyword} <TARGET NAME> <PACKET NAME> <ENDIANNESS: BIG_ENDIAN/LITTLE_ENDIAN> <DESCRIPTION (Optional)>"
         self.parser.verify_num_parameters(3, 4, self.usage)
         self.parser.verify_parameter_naming(2)  # Packet name is the 2nd parameter
 
     def create_command(self, target_name, commands, warnings):
         packet = self._create_packet(target_name)
-        return PacketParser._finish_create_command(packet, commands, warnings)
+        PacketParser._finish_create_command(packet, commands, warnings)
 
     def create_telemetry(self, target_name, telemetry, latest_data, warnings):
         packet = self._create_packet(target_name)
-        return PacketParser._finish_create_telemetry(
-            packet, telemetry, latest_data, warnings
-        )
+        PacketParser._finish_create_telemetry(packet, telemetry, latest_data, warnings)
 
     def _create_packet(self, target_name):
         params = self.parser.parameters
         if target_name == "SYSTEM":
             target_name = params[0].upper()
         packet_name = params[1].upper()
         endianness = params[2].upper()
-        # description is optional
-        description = None
-        if len(params) > 3:
-            description = params[3]
+        description = params[3]
         if endianness != "BIG_ENDIAN" and endianness != "LITTLE_ENDIAN":
             raise self.parser.error(
                 f"Invalid endianness {params[2]}. Must be BIG_ENDIAN or LITTLE_ENDIAN.",
                 self.usage,
             )
         return Packet(target_name, packet_name, endianness, description)
```

### Comparing `openc3-5.16.0/openc3/packets/structure.py` & `openc3-5.9.2b0/openc3/packets/structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -15,70 +17,97 @@
 # if purchased from OpenC3, Inc.
 
 import copy
 import threading
 from contextlib import contextmanager
 from openc3.accessors.binary_accessor import BinaryAccessor
 from openc3.packets.structure_item import StructureItem
-from openc3.utilities.string import formatted
 
 
 class Structure:
     """Maintains knowledge of a raw binary structure. Uses structure_item to
     create individual structure items which are read and written by
     binary_accessor."""
 
+    # # self.return [Symbol] Default endianness for items in the structure. One of
+    # #   {BinaryAccessor::ENDIANNESS}
+    # attr_reader :default_endianness
+
+    # # self.return [Hash] Items that make up the structure.
+    # #   Hash key is the item's name in uppercase
+    # attr_reader :items
+
+    # # self.return [Array] Items sorted by bit_offset.
+    # attr_reader :sorted_items
+
+    # # self.return [Integer] Defined length in bytes (not bits) of the structure
+    # attr_reader :defined_length
+
+    # # self.return [Integer] Defined length in bits of the structure
+    # attr_reader :defined_length_bits
+
+    # # self.return [Boolean] Flag indicating if the structure contains any variably
+    # #   sized items or not.
+    # attr_reader :fixed_size
+
+    # # self.return [Boolean] Flag indicating if giving a buffer with less than
+    # #   required data size is allowed.
+    # attr_accessor :short_buffer_allowed
+
+    # # self.return [Accessor] Class used to access raw data of structure from buffer
+    # attr_reader :accessor
+
+    # Used to force encoding
+    ASCII_8BIT_STRING = "ASCII-8BIT"
+
     # String providing a single 0 byte
     ZERO_STRING = b"\00"
 
     def __init__(
         self,
         default_endianness=BinaryAccessor.HOST_ENDIANNESS,
         buffer=None,
         item_class=StructureItem,
     ):
         if (default_endianness == "BIG_ENDIAN") or (
             default_endianness == "LITTLE_ENDIAN"
         ):
             self.default_endianness = default_endianness
-            if buffer is not None and not isinstance(
-                buffer, (bytes, bytearray)
-            ):  # type(buffer) != str:
+            if buffer is not None and type(buffer) != str:
                 raise TypeError(
-                    f"wrong argument type {buffer.__class__.__name__} (expected bytes)"
+                    f"wrong argument type {buffer.__class__.__name__} (expected String)"
                 )
-            if buffer is None:
-                self._buffer = None
-            else:
-                self._buffer = bytearray(buffer)  # TODO: Do we need to force encoding?
+            self._buffer = buffer  # .force_encoding(Structure.ASCII_8BIT_STRING)
             self.item_class = item_class
             self.items = {}
             self.sorted_items = []
             self.defined_length = 0
             self.defined_length_bits = 0
             self.pos_bit_size = 0
             self.neg_bit_size = 0
             self.fixed_size = True
             self.short_buffer_allowed = False
             self.mutex = None
-            self.accessor = BinaryAccessor()
+            self.accessor = BinaryAccessor
         else:
             raise AttributeError(
                 f"Unknown endianness '{default_endianness}', must be 'BIG_ENDIAN' or 'LITTLE_ENDIAN'"
             )
 
     # Read an item in the structure
     #
     # self.param item [StructureItem] Instance of StructureItem or one of its subclasses
     # self.param value_type [Symbol] Not used. Subclasses should overload this
     #   parameter to check whether to perform conversions on the item.
     # self.param buffer [String] The binary buffer to read the item from
     # self.return Value based on the item definition. This could be a string, integer,
     #   float, or array of values.
     def read_item(self, item, value_type="RAW", buffer=None):
+        if item.data_type == "DERIVED":
+            return None
         if not buffer:
             buffer = self._buffer
         if not buffer:
             buffer = self.allocate_buffer_if_needed()
         return self.accessor.read_item(item, buffer)
 
     # Get the length of the buffer used by the structure
@@ -105,17 +134,15 @@
 
     # Configure the accessor for this packet
     #
     # self.param accessor [Accessor] The class to use as an accessor
     @accessor.setter
     def accessor(self, accessor):
         self.__accessor = accessor
-        # isinstance can fail if the class is reloaded because the class becomes a new class
-        # so direcly check the class name which is basically equivalent
-        if self.__accessor.enforce_short_buffer_allowed():
+        if self.__accessor != BinaryAccessor:
             self.short_buffer_allowed = True
 
     # Read a list of items in the structure
     #
     # self.param items [StructureItem] Array of StructureItem or one of its subclasses
     # self.param value_type [Symbol] Not used. Subclasses should overload this
     #   parameter to check whether to perform conversions on the item.
@@ -181,15 +208,15 @@
     ):
         if not endianness:
             endianness = self.default_endianness
         # Create the item
         item = self.item_class(
             name, bit_offset, bit_size, data_type, endianness, array_size, overflow
         )
-        return self.define(item)
+        self.define(item)
 
     # Adds the given item to the items hash. It also resizes the buffer to
     # accomodate the new item.
     #
     # self.param item [StructureItem] The structure item to add
     # self.return [StrutureItem] The struture item defined
     def define(self, item):
@@ -257,14 +284,15 @@
             self.defined_length = int(self.defined_length_bits / 8)
             if self.defined_length_bits % 8 != 0:
                 self.defined_length += 1
 
         # Resize the buffer if necessary
         if self.buffer:
             self.resize_buffer()
+
         return item
 
     # Define an item at the end of the structure. This creates a new instance of the
     # item_class as given in the constructor and adds it to the items hash. It
     # also resizes the buffer to accomodate the new item.
     #
     # self.param name (see #define_item)
@@ -375,15 +403,15 @@
     #   parameter to check whether to perform conversions on the item.
     # self.param buffer [String] The binary buffer to write the values to
     def write_items(self, items, values, value_type="RAW", buffer=None):
         if not buffer:
             buffer = self._buffer
         if not buffer:
             buffer = self.allocate_buffer_if_needed()
-        self.accessor.write_items(items, values, buffer)
+        return self.accessor.write_items(items, values, buffer)
 
     # Read an item in the structure by name
     #
     # self.param name [String] Name of an item to read
     # self.param value_type [Symbol] Not used. Subclasses should overload this
     #   parameter to check whether to perform conversions on the item.
     # self.param buffer [String] The binary buffer to read the item from
@@ -447,30 +475,30 @@
                     item.data_type == "BLOCK"
                     and value_type != "RAW"
                     and hasattr(item, "read_conversion")
                 ):
                     string += f"{indent_string}{item.name}: {self.read_item(item, value_type, buffer)}\n"
                 else:
                     value = self.read_item(item, value_type, buffer)
-                    if isinstance(value, (str, bytes, bytearray)):
+                    if type(value) == str:
                         string += f"{indent_string}{item.name}:\n"
-                        string += formatted(value, 1, 16, " ", indent + 2)
+                        string += value  # .formatted(1, 16, " ", indent + 2)
                     else:
                         string += f"{indent_string}{item.name}: {value}\n"
 
         return string
 
     # Get the buffer used by the structure. The current buffer is copied and
     # thus modifications to the returned buffer will have no effect on the
     # structure items.
     #
     # self.param copy [TrueClass/FalseClass] Whether to copy the buffer
     # self.return [String] Data buffer backing the structure
     @property
-    def buffer(self):
+    def buffer(self, copy=True):
         return self.allocate_buffer_if_needed()[:]
 
     def buffer_no_copy(self):
         return self.allocate_buffer_if_needed()
 
     # Set the buffer to be used by the structure. The buffer is copied and thus
     # further modifications to the buffer have no effect on the structure
@@ -484,18 +512,31 @@
 
     # Make a light weight clone of this structure. This only creates a new buffer
     # of data. The defined structure items are the same.
     #
     # self.return [Structure] A copy of the current structure with a new underlying
     #   buffer of data
     def clone(self):
-        struct = copy.copy(self)
-        struct._buffer = self.buffer  # Makes a copy
-        struct.accessor.packet = struct
-        return struct
+        return copy.deepcopy(self)
+
+    # Enable the ability to read and write item values as if they were methods
+    # to the class
+    def __getattr__(self, func):
+        # Prevent recursion in deepcopy
+        if func in ["__deepcopy__", "__setstate__"]:
+            raise AttributeError()
+
+        def method(*args, **kwargs):
+            return getattr(self, func)(*args, **kwargs)
+
+        return method
+
+    # TODO:
+    # def __setattr__(self, func, value):
+    #     return setattr(self, func, value)
 
     MUTEX = threading.Lock()
 
     def setup_mutex(self):
         if self.mutex:
             return
         with Structure.MUTEX:
@@ -524,26 +565,25 @@
         else:
             got_mutex = self.mutex.acquire(False)
             if got_mutex:
                 try:
                     yield
                 finally:
                     self.mutex.release()
-            else:  # if self.mutex_allow_reads == threading.get_ident()
+            elif self.mutex_allow_reads == threading.get_ident():
                 yield
 
     def internal_buffer_equals(self, buffer):
         if not isinstance(buffer, (bytes, bytearray)):
             raise AttributeError(
                 f"Buffer class is {buffer.__class__.__name__} but must be bytearray"
             )
 
-        self._buffer = bytearray(buffer[:])
+        self._buffer = buffer[:]
         # self.buffer.force_encoding('ASCII-8BIT'.freeze)
-        if self.accessor.enforce_length():
-            if len(self._buffer) != self.defined_length:
-                if len(self._buffer) < self.defined_length:
-                    self.resize_buffer()
-                    if not self.short_buffer_allowed:
-                        raise AttributeError("Buffer length less than defined length")
-                elif self.fixed_size and self.defined_length != 0:
-                    raise AttributeError("Buffer length greater than defined length")
+        if len(self._buffer) != self.defined_length:
+            if len(self._buffer) < self.defined_length:
+                self.resize_buffer()
+                if not self.short_buffer_allowed:
+                    raise AttributeError("Buffer length less than defined length")
+            elif self.fixed_size and self.defined_length != 0:
+                raise AttributeError("Buffer length greater than defined length")
```

### Comparing `openc3-5.16.0/openc3/packets/structure_item.py` & `openc3-5.9.2b0/openc3/packets/structure_item.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -22,14 +24,60 @@
 @total_ordering
 class StructureItem:
     create_index = 0
 
     # Valid data types adds DERIVED to those defined by BinaryAccessor
     DATA_TYPES = BinaryAccessor.DATA_TYPES + ["DERIVED"]
 
+    #     # Name is used by higher level classes to access the StructureItem.
+    #     # self.return [String] Name of the item
+    #     attr_reader :name
+
+    #     # Key is used to access into nested structures during decom if applicable
+    #     attr_reader :key
+
+    #     # Indicates where in the binary buffer the StructureItem exists.
+    #     # self.return [Integer] 0 based bit offset
+    #     attr_reader :bit_offset
+
+    #     # The number of bits which represent this StructureItem in the binary buffer.
+    #     # self.return [Integer] Size in bits
+    #     attr_reader :bit_size
+
+    #     # The data type is what kind of data this StructureItem
+    #     # represents when extracted from the binary buffer. 'INT' and 'UINT' are
+    #     # turned into Integers (Ruby Fixnum). 'FLOAT' are turned into floating point
+    #     # numbers (Ruby Float). 'STRING' is turned into an ASCII string (Ruby
+    #     # String). 'BLOCK' is turned into a binary buffer (Ruby String). 'DERIVED' is
+    #     # interpreted by the subclass and can result in any type.
+    #     # self.return [Symbol] {DATA_TYPES}
+    #     attr_reader :data_type
+
+    #     # Used to interpret how to read the item from the binary data buffer.
+    #     # self.return [Symbol] {BinaryAccessor::ENDIANNESS}
+    #     attr_reader :endianness
+
+    #     # The total number of bits in the binary buffer that create the array.
+    #     # The array size can be set to None to indicate the StructureItem is
+    #     # not represented as an array. For example, if the bit_size is 8 bits,
+    #     # an array_size of 16 would result in two 8 bit items.
+    #     # self.return [Integer, None] Array size of the item in bits
+    #     attr_reader :array_size
+
+    #     # How to handle overflow for 'INT', 'UINT', 'STRING', and 'BLOCK' data types
+    #     # Note: Has no meaning for 'FLOAT' data types
+    #     # self.return [Symbol] {BinaryAccessor::OVERFLOW_TYPES}
+    #     attr_reader :overflow
+
+    #     # self.return [Boolean] Whether this structure item can overlap another item in the same packet
+    #     attr_accessor :overlap
+
+    #     # A large buffer size in bits (1 Megabyte)
+    #     LARGE_BUFFER_SIZE_BITS = 1024 * 1024 * 8
+
     # Create a StructureItem by setting all the attributes. It
     # calls all the setter routines to do the attribute verification and then
     # verifies the overall integrity.
     #
     # self.param name [String] The item name
     # self.param bit_offset [Integer] Offset to the item starting at 0
     # self.param bit_size [Integer] Size of the items in bits
@@ -181,17 +229,15 @@
     @property
     def data_type(self):
         return self.__data_type
 
     @data_type.setter
     def data_type(self, data_type):
         if type(data_type) != str:
-            raise AttributeError(
-                f"{self.name}: data_type must be a str but {data_type} is a {type(data_type).__name__}"
-            )
+            raise AttributeError(f"{self.name}: data_type must be a String")
         if data_type not in StructureItem.DATA_TYPES:
             raise AttributeError(
                 f"{self.name}: unknown data_type: {data_type} - Must be 'INT', 'UINT', 'FLOAT', 'STRING', 'BLOCK', or 'DERIVED'"
             )
 
         self.__data_type = data_type
         if self.structure_item_constructed:
```

### Comparing `openc3-5.16.0/openc3/packets/telemetry.py` & `openc3-5.9.2b0/openc3/packets/telemetry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Copyright 2024 OpenC3, Inc.
+#!/usr/bin/env python3
+
+# Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 #
@@ -27,27 +29,25 @@
     Packet or PacketItem objects. While there are some overlapping methods between
     the two, these are separate interfaces into the system."""
 
     LATEST_PACKET_NAME = "LATEST"
 
     # @param config [PacketConfig] Packet configuration to use to access the
     #  telemetry
-    def __init__(self, config, system):
-        self.system = system
+    def __init__(self, config):
         self.config = config
 
     # (see PacketConfig#warnings)
     def warnings(self):
         return self.config.warnings
 
     # @return [Array<String>] The command target names (excluding UNKNOWN)
     def target_names(self):
-        result = self.config.telemetry.keys()
+        result = self.config.telemetry.keys().sort()
         result.delete("UNKNOWN")
-        result.sort()
         return result
 
     # @param target_name [String] The target name
     # @return [Hash<packet_name=>Packet>] Hash of the telemetry packets for the given
     #   target name keyed by the packet name
     def packets(self, target_name):
         upcase_target_name = target_name.upper()
@@ -66,331 +66,368 @@
     def packet(self, target_name, packet_name):
         target_packets = self.packets(target_name)
         upcase_packet_name = packet_name.upper()
         packet = target_packets.get(upcase_packet_name, None)
         if not packet:
             upcase_target_name = target_name.upper()
             raise RuntimeError(
-                f"Telemetry packet '{upcase_target_name} {upcase_packet_name}' does not exist"
+                f"Telemetry packet '#{upcase_target_name} #{upcase_packet_name}' does not exist"
             )
         return packet
 
-    # # @param target_name (see #packet)
-    # # @param packet_name [String] The packet name. 'LATEST' can also be given
-    # #   to specify the last received (or defined if no packets have been
-    # #   received) packet within the given target that contains the
-    # #   item_name.
-    # # @param item_name [String] The item name
-    # # @return [Packet, PacketItem] The packet and the packet item
-    # def packet_and_item(target_name, packet_name, item_name):
-    #     upcase_packet_name = str(packet_name).upper()
-    #     if upcase_packet_name == "LATEST":
+    #   # @param target_name (see #packet)
+    #   # @param packet_name [String] The packet name. 'LATEST' can also be given
+    #   #   to specify the last received (or defined if no packets have been
+    #   #   received) packet within the given target that contains the
+    #   #   item_name.
+    #   # @param item_name [String] The item name
+    #   # @return [Packet, PacketItem] The packet and the packet item
+    #   def packet_and_item(target_name, packet_name, item_name)
+    #     upcase_packet_name = packet_name.to_s.upcase
+    #     if upcase_packet_name == "LATEST".freeze
     #       return_packet = newest_packet(target_name, item_name)
-    #     else:
+    #     else
     #       return_packet = packet(target_name, packet_name)
+    #     end
     #     item = return_packet.get_item(item_name)
     #     return [return_packet, item]
+    #   end
 
-    # # Return a telemetry value from a packet.
-    # #
-    # # @param target_name (see #packet_and_item)
-    # # @param packet_name (see #packet_and_item)
-    # # @param item_name (see #packet_and_item)
-    # # @param value_type [Symbol] How to convert the item before returning.
-    # #   Must be one of {Packet::VALUE_TYPES}
-    # # @return The value. :FORMATTED and :WITH_UNITS values are always returned
-    # #   as Strings. :RAW values will match their data_type. :CONVERTED values
-    # #   can be any type.
-    # def value(target_name, packet_name, item_name, value_type = 'CONVERTED'):
+    #   # Return a telemetry value from a packet.
+    #   #
+    #   # @param target_name (see #packet_and_item)
+    #   # @param packet_name (see #packet_and_item)
+    #   # @param item_name (see #packet_and_item)
+    #   # @param value_type [Symbol] How to convert the item before returning.
+    #   #   Must be one of {Packet::VALUE_TYPES}
+    #   # @return The value. :FORMATTED and :WITH_UNITS values are always returned
+    #   #   as Strings. :RAW values will match their data_type. :CONVERTED values
+    #   #   can be any type.
+    #   def value(target_name, packet_name, item_name, value_type = :CONVERTED)
     #     packet, _ = packet_and_item(target_name, packet_name, item_name) # Handles LATEST
     #     return packet.read(item_name, value_type)
+    #   end
 
-    # # Reads the specified list of items and returns their values and limits
-    # # state.
-    # #
-    # # @param item_array [Array<Array(String String String)>] An array
-    # #   consisting of [target name, packet name, item name]
-    # # @param value_types [Symbol|Array<Symbol>] How to convert the items before
-    # #   returning. A single symbol of {Packet::VALUE_TYPES}
-    # #   can be passed which will convert all items the same way. Or
-    # #   an array of symbols can be passed to control how each item is
-    # #   converted.
-    # # @return [Array, Array, Array] The first array contains the item values and the
-    # #   second their limits state, and the third their limits settings which includes
-    # #   the red, yellow, and green (if given) limits values.
-    # def values_and_limits_states(item_array, value_types = 'CONVERTED'):
+    #   # Reads the specified list of items and returns their values and limits
+    #   # state.
+    #   #
+    #   # @param item_array [Array<Array(String String String)>] An array
+    #   #   consisting of [target name, packet name, item name]
+    #   # @param value_types [Symbol|Array<Symbol>] How to convert the items before
+    #   #   returning. A single symbol of {Packet::VALUE_TYPES}
+    #   #   can be passed which will convert all items the same way. Or
+    #   #   an array of symbols can be passed to control how each item is
+    #   #   converted.
+    #   # @return [Array, Array, Array] The first array contains the item values and the
+    #   #   second their limits state, and the third their limits settings which includes
+    #   #   the red, yellow, and green (if given) limits values.
+    #   def values_and_limits_states(item_array, value_types = :CONVERTED)
     #     items = []
 
     #     # Verify item_array is a nested array
-    #     raise AttributeError(f"item_array must be a nested array consisting of [[tgt,pkt,item],[tgt,pkt,item],...]") if not Array === item_array[0]
+    #     raise AttributeError("item_array must be a nested array consisting of [[tgt,pkt,item],[tgt,pkt,item],...]") unless Array === item_array[0]
 
     #     states = []
     #     settings = []
-    #     limits_set = System.limits_set()
+    #     limits_set = System.limits_set
 
-    #     if (Array === value_types) and len(item_array) != len(value_types):
-    #         raise AttributeError(f"Passed {len(item_array)} items but only {len(value_types)} value types")
+    #     raise AttributeError("Passed #{item_array.length} items but only #{value_types.length} value types") if (Array === value_types) and item_array.length != value_types.length
 
-    #     value_type = value_types if not Array === value_types
-    #     len(item_array).times do |index|
+    #     value_type = value_types.intern unless Array === value_types
+    #     item_array.length.times do |index|
     #       entry = item_array[index]
     #       target_name = entry[0]
     #       packet_name = entry[1]
     #       item_name = entry[2]
-    #       if Array === value_types:
-    #           value_type = value_types[index]
+    #       value_type = value_types[index].intern if Array === value_types
 
     #       packet, item = packet_and_item(target_name, packet_name, item_name) # Handles LATEST
-    #       items.append(packet.read(item_name, value_type))
+    #       items << packet.read(item_name, value_type)
     #       limits = item.limits
-    #       states.append(limits.state)
+    #       states << limits.state
     #       limits_values = limits.values
-    #       if limits_values:
+    #       if limits_values
     #         limits_settings = limits_values[limits_set]
-    #       else:
-    #         limits_settings = None
-    #       settings.append(limits_settings)
+    #       else
+    #         limits_settings = nil
+    #       end
+    #       settings << limits_settings
+    #     end
 
     #     return [items, states, settings]
+    #   end
+    # end
 
     # # @param target_name (see #packet)
     # # @param packet_name (see #packet)
     # # @return [Array<PacketItem>] The telemetry items for the given target and packet name
-    # def items(target_name, packet_name):
+    # def items(target_name, packet_name)
     #   return packet(target_name, packet_name).sorted_items
+    # end
 
     # # @param target_name (see #packet)
     # # @param packet_name (see #packet) The packet name.  LATEST is supported.
     # # @return [Array<PacketItem>] The telemetry item names for the given target and packet name
-    # def item_names(target_name, packet_name):
-    #   if LATEST_PACKET_NAME.casecmp(packet_name).zero?:
-    #     target_upmatch = str(target_name).upper():
-    #     target_latest_data = self.config.latest_data[target_upcase]
-    #     raise "Telemetry Target '{target_upcase}' does not exist" if not target_latest_data
+    # def item_names(target_name, packet_name)
+    #   if LATEST_PACKET_NAME.casecmp(packet_name).zero?
+    #     target_upcase = target_name.to_s.upcase
+    #     target_latest_data = @config.latest_data[target_upcase]
+    #     raise "Telemetry Target '#{target_upcase}' does not exist" unless target_latest_data
 
     #     item_names = target_latest_data.keys
-    #   else:
+    #   else
     #     tlm_packet = packet(target_name, packet_name)
     #     item_names = []
-    #     tlm_packet.sorted_items.each { |item| item_names.append(item.name })
+    #     tlm_packet.sorted_items.each { |item| item_names << item.name }
+    #   end
     #   item_names
+    # end
 
     # # Set a telemetry value in a packet.
     # #
     # # @param target_name (see #packet_and_item)
     # # @param packet_name (see #packet_and_item)
     # # @param item_name (see #packet_and_item)
     # # @param value The value to set in the packet
     # # @param value_type (see #tlm)
-    # def set_value(target_name, packet_name, item_name, value, value_type = 'CONVERTED'):
+    # def set_value(target_name, packet_name, item_name, value, value_type = :CONVERTED)
     #   packet, _ = packet_and_item(target_name, packet_name, item_name)
     #   packet.write(item_name, value, value_type)
+    # end
 
     # # @param target_name (see #packet_and_item)
     # # @param item_name (see #packet_and_item)
     # # @return [Array<Packet>] The latest (most recently arrived) packets with
     # #   the specified target and item.
-    # def latest_packets(target_name, item_name):
-    #   target_upmatch = str(target_name).upper():
-    #   item_upmatch = str(item_name).upper():
-    #   target_latest_data = self.config.latest_data[target_upcase]
-    #   raise "Telemetry target '{target_upcase}' does not exist" if not target_latest_data
+    # def latest_packets(target_name, item_name)
+    #   target_upcase = target_name.to_s.upcase
+    #   item_upcase = item_name.to_s.upcase
+    #   target_latest_data = @config.latest_data[target_upcase]
+    #   raise "Telemetry target '#{target_upcase}' does not exist" unless target_latest_data
 
-    #   packets = self.config.latest_data[target_upcase][item_upcase]
-    #   raise "Telemetry item '{target_upcase} {LATEST_PACKET_NAME} {item_upcase}' does not exist" if not packets
+    #   packets = @config.latest_data[target_upcase][item_upcase]
+    #   raise "Telemetry item '#{target_upcase} #{LATEST_PACKET_NAME} #{item_upcase}' does not exist" unless packets
 
     #   return packets
+    # end
 
     # # @param target_name (see #packet_and_item)
     # # @param item_name (see #packet_and_item)
     # # @return [Packet] The packet with the most recent timestamp that contains
     # #   the specified target and item.
-    # def newest_packet(target_name, item_name):
+    # def newest_packet(target_name, item_name)
     #   # Handle LATEST_PACKET_NAME - Lookup packets for this target/item
     #   packets = latest_packets(target_name, item_name)
 
     #   # Find packet with newest timestamp
-    #   newest_packet = None
-    #   newest_received_time = None
-    #    for packet in packets:
+    #   newest_packet = nil
+    #   newest_received_time = nil
+    #   packets.each do |packet|
     #     received_time = packet.received_time
-    #     if newest_received_time:
+    #     if newest_received_time
     #       # See if the received time from this packet is newer.
     #       # Having the >= makes this method return the last defined packet
     #       # whether the timestamps are both nil or both equal.
-    #       if received_time and received_time >= newest_received_time:
+    #       if received_time and received_time >= newest_received_time
     #         newest_packet = packet
     #         newest_received_time = newest_packet.received_time
-    #     else:
+    #       end
+    #     else
     #       # No received time yet so take this packet
     #       newest_packet = packet
     #       newest_received_time = newest_packet.received_time
+    #     end
+    #   end
     #   return newest_packet
+    # end
+
+    # # Identifies an unknown buffer of data as a defined packet and sets the
+    # # packet's data to the given buffer. Identifying a packet uses the fields
+    # # marked as ID_ITEM to identify if the buffer passed represents the
+    # # packet defined. Incorrectly sized buffers are still processed but an
+    # # error is logged.
+    # #
+    # # Note: This affects all subsequent requests for the packet (for example
+    # # using packet) which is why the method is marked with a bang!
+    # #
+    # # @param packet_data [String] The binary packet data buffer
+    # # @param target_names [Array<String>] List of target names to limit the search. The
+    # #   default value of nil means to search all known targets.
+    # # @return [Packet] The identified packet with its data set to the given
+    # #   packet_data buffer. Returns nil if no packet could be identified.
+    # def identify!(packet_data, target_names = nil)
+    #   identified_packet = identify(packet_data, target_names)
+    #   identified_packet.buffer = packet_data if identified_packet
+    #   return identified_packet
+    # end
 
-    # Identifies an unknown buffer of data as a defined packet and sets the
-    # packet's data to the given buffer. Identifying a packet uses the fields
-    # marked as ID_ITEM to identify if the buffer passed represents the
-    # packet defined. Incorrectly sized buffers are still processed but an
-    # error is logged.
-    #
-    # Note: This affects all subsequent requests for the packet (for example
-    # using packet)
-    #
-    # @param packet_data [String] The binary packet data buffer
-    # @param target_names [Array<String>] List of target names to limit the search. The
-    #   default value of nil means to search all known targets.
-    # @return [Packet] The identified packet with its data set to the given
-    #   packet_data buffer. Returns nil if no packet could be identified.
-    def identify_and_set_buffer(self, packet_data, target_names=None):
-        identified_packet = self.identify(packet_data, target_names)
-        if identified_packet:
-            identified_packet.buffer = packet_data
-        return identified_packet
-
-    # Finds a packet from the Current Value Table that matches the given data
-    # and returns it.  Does not fill the packets buffer.  Use identify! to update the CVT.
-    #
-    # @param packet_data [String] The binary packet data buffer
-    # @param target_names [Array<String>] List of target names to limit the search. The
-    #   default value of nil means to search all known targets.
-    # @return [Packet] The identified packet, Returns nil if no packet could be identified.
-    def identify(self, packet_data, target_names=None):
-        if target_names is None:
-            target_names = self.target_names()
-
-        for target_name in target_names:
-            target_name = str(target_name).upper()
-
-            target_packets = None
-            try:
-                target_packets = self.packets(target_name)
-            except RuntimeError:
-                # No telemetry for this target
-                continue
-
-            target = self.system.targets[target_name]
-            if target and target.tlm_unique_id_mode:
-                # Iterate through the packets and see if any represent the buffer
-                for _, packet in target_packets:
-                    if packet.identify(packet_data):
-                        return packet
-            else:
-                # Do a hash lookup to quickly identify the packet
-                if len(target_packets) > 0:
-                    packet = next(iter(target_packets.values()))
-                    key = packet.read_id_values(packet_data)
-                    hash = self.config.tlm_id_value_hash[target_name]
-                    identified_packet = hash.get(repr(key))
-                    if identified_packet is None:
-                        identified_packet = hash.get("CATCHALL")
-                    if identified_packet is not None:
-                        return identified_packet
-
-        return None
-
-    def identify_and_define_packet(self, packet, target_names=None):
-        if not packet.identified():
-            identified_packet = self.identify(packet.buffer_no_copy(), target_names)
-            if not identified_packet:
-                return None
-
-            identified_packet = identified_packet.clone()
-            identified_packet.buffer = packet.buffer
-            identified_packet.received_time = packet.received_time
-            identified_packet.stored = packet.stored
-            identified_packet.extra = packet.extra
-            return identified_packet
-
-        if not packet.defined():
-            try:
-                identified_packet = self.packet(packet.target_name, packet.packet_name)
-            except RuntimeError:
-                return None
-            identified_packet = identified_packet.clone()
-            identified_packet.buffer = packet.buffer
-            identified_packet.received_time = packet.received_time
-            identified_packet.stored = packet.stored
-            identified_packet.extra = packet.extra
-            return identified_packet
+    # # Finds a packet from the Current Value Table that matches the given data
+    # # and returns it.  Does not fill the packets buffer.  Use identify! to update the CVT.
+    # #
+    # # @param packet_data [String] The binary packet data buffer
+    # # @param target_names [Array<String>] List of target names to limit the search. The
+    # #   default value of nil means to search all known targets.
+    # # @return [Packet] The identified packet, Returns nil if no packet could be identified.
+    # def identify(packet_data, target_names = nil)
+    #   target_names = target_names() unless target_names
+
+    #   target_names.each do |target_name|
+    #     target_name = target_name.to_s.upcase
+
+    #     target_packets = nil
+    #     begin
+    #       target_packets = packets(target_name)
+    #       # puts target_packets.length
+    #     rescue RuntimeError
+    #       # No telemetry for this target
+    #       next
+    #     end
+
+    #     target = System.targets[target_name]
+    #     if target and target.tlm_unique_id_mode
+    #       # Iterate through the packets and see if any represent the buffer
+    #       target_packets.each do |packet_name, packet|
+    #         return packet if packet.identify?(packet_data)
+    #       end
+    #     else
+    #       # Do a hash lookup to quickly identify the packet
+    #       if target_packets.length > 0
+    #         packet = target_packets.first[1]
+    #         key = packet.read_id_values(packet_data)
+    #         hash = @config.tlm_id_value_hash[target_name]
+    #         identified_packet = hash[key]
+    #         identified_packet = hash['CATCHALL'.freeze] unless identified_packet
+    #         return identified_packet if identified_packet
+    #       end
+    #     end
+    #   end
+
+    #   return nil
+    # end
+
+    # def identify_and_define_packet(packet, target_names = nil)
+    #   if !packet.identified?
+    #     identified_packet = identify(packet.buffer(false), target_names)
+    #     return nil unless identified_packet
+
+    #     identified_packet = identified_packet.clone
+    #     identified_packet.buffer = packet.buffer
+    #     identified_packet.received_time = packet.received_time
+    #     identified_packet.stored = packet.stored
+    #     identified_packet.extra = packet.extra
+    #     return identified_packet
+    #   end
+
+    #   if !packet.defined?
+    #     begin
+    #       identified_packet = self.packet(packet.target_name, packet.packet_name)
+    #     rescue RuntimeError
+    #       return nil
+    #     end
+    #     identified_packet = identified_packet.clone
+    #     identified_packet.buffer = packet.buffer
+    #     identified_packet.received_time = packet.received_time
+    #     identified_packet.stored = packet.stored
+    #     identified_packet.extra = packet.extra
+    #     return identified_packet
+    #   end
 
-        return packet
+    #   return packet
+    # end
 
-    # Updates the specified packet with the given packet data. Raises an error
-    # if the packet could not be found.
-    #
-    # Note: This affects all subsequent requests for the packet
-    #
-    # @param target_name (see #packet)
-    # @param packet_name (see #packet)
-    # @param packet_data (see #identify_tlm!)
-    # @return [Packet] The packet with its data set to the given packet_data
-    #   buffer.
-    def update(self, target_name, packet_name, packet_data):
-        identified_packet = self.packet(target_name, packet_name)
-        identified_packet.buffer = packet_data
-        return identified_packet
-
-    # Assigns a limits change callback to all telemetry packets
-    #
-    # @param limits_change_callback
-    def set_limits_change_callback(self, limits_change_callback):
-        for _, packets in self.config.telemetry.items():
-            for _, packet in packets.items():
-                packet.limits_change_callback = limits_change_callback
+    # # Updates the specified packet with the given packet data. Raises an error
+    # # if the packet could not be found.
+    # #
+    # # Note: This affects all subsequent requests for the packet which is why
+    # # the method is marked with a bang!
+    # #
+    # # @param target_name (see #packet)
+    # # @param packet_name (see #packet)
+    # # @param packet_data (see #identify_tlm!)
+    # # @return [Packet] The packet with its data set to the given packet_data
+    # #   buffer.
+    # def update!(target_name, packet_name, packet_data)
+    #   identified_packet = packet(target_name, packet_name)
+    #   identified_packet.buffer = packet_data
+    #   return identified_packet
+    # end
+
+    # # Assigns a limits change callback to all telemetry packets
+    # #
+    # # @param limits_change_callback
+    # def limits_change_callback=(limits_change_callback)
+    #   @config.telemetry.each do |target_name, packets|
+    #     packets.each do |packet_name, packet|
+    #       packet.limits_change_callback = limits_change_callback
+    #     end
+    #   end
+    # end
 
     # # Clears the received_count value on every packet in every target
-    # def clear_counters:
-    #    for target_name, target_packets in self.config.telemetry:
-    #      for packet_name, packet in target_packets:
+    # def clear_counters
+    #   @config.telemetry.each do |target_name, target_packets|
+    #     target_packets.each do |packet_name, packet|
     #       packet.received_count = 0
+    #     end
+    #   end
+    # end
 
     # # Resets metadata on every packet in every target
-    # def reset:
-    #    for target_name, target_packets in self.config.telemetry:
-    #      for packet_name, packet in target_packets:
+    # def reset
+    #   @config.telemetry.each do |target_name, target_packets|
+    #     target_packets.each do |packet_name, packet|
     #       packet.reset
+    #     end
+    #   end
+    # end
 
     # # Returns the first non-hidden packet
-    # def first_non_hidden:
-    #    for target_name, target_packets in self.config.telemetry:
-    #     if target_name == 'UNKNOWN':
-    #         next
-
-    #      for packet_name, packet in target_packets:
-    #       return packet if not packet.hidden
-    #   None
+    # def first_non_hidden
+    #   @config.telemetry.each do |target_name, target_packets|
+    #     next if target_name == 'UNKNOWN'
+
+    #     target_packets.each do |packet_name, packet|
+    #       return packet unless packet.hidden
+    #     end
+    #   end
+    #   nil
+    # end
 
     # # Returns an array with a "TARGET_NAME PACKET_NAME ITEM_NAME" string for every item in the system
-    # def all_item_strings(include_hidden = False, splash = None):
+    # def all_item_strings(include_hidden = false, splash = nil)
     #   strings = []
     #   tnames = target_names()
-    #   total = len(tnames) float()
+    #   total = tnames.length.to_f
     #   tnames.each_with_index do |target_name, index|
-    #     if splash:
-    #       splash.message = "Processing {target_name} telemetry"
+    #     if splash
+    #       splash.message = "Processing #{target_name} telemetry"
     #       splash.progress = index / total
+    #     end
 
     #     # Note: System only has declared target structures but telemetry may have more
     #     system_target = System.targets[target_name]
-    #     if system_target:
+    #     if system_target
     #       ignored_items = system_target.ignored_items
-    #     else:
+    #     else
     #       ignored_items = []
+    #     end
 
-    #      for packet_name, packet in packets(target_name):
+    #     packets(target_name).each do |packet_name, packet|
     #       # We don't audit against hidden or disabled packets
-    #       if !include_hidden and (packet.hidden or packet.disabled):
-    #           next
+    #       next if !include_hidden and (packet.hidden || packet.disabled)
 
     #       packet.items.each_key do |item_name|
     #         # Skip ignored items
-    #         if !include_hidden and ignored_items.include? item_name:
-    #             next
+    #         next if !include_hidden and ignored_items.include? item_name
 
-    #         strings.append("{target_name} {packet_name} {item_name}")
-    #   return strings
+    #         strings << "#{target_name} #{packet_name} #{item_name}"
+    #       end
+    #     end
+    #   end
+    #   strings
+    # end
 
     # @return [Hash{String=>Hash{String=>Packet}}] Hash of all the telemetry
     #   packets keyed by the target name. The value is another hash keyed by the
     #   packet name returning the packet.
     def all(self):
         return self.config.telemetry
```

### Comparing `openc3-5.16.0/openc3/script/api_shared.py` & `openc3-5.9.2b0/openc3/script/api_shared.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,42 @@
+#!/usr/bin/env python3
+
 # Copyright 2022 Ball Aerospace & Technologies Corp.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 
 # Modified by OpenC3, Inc.
-# All changes Copyright 2023, OpenC3, Inc.
+# All changes Copyright 2022, OpenC3, Inc.
 # All Rights Reserved
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import sys
 import time
-from contextlib import contextmanager
+
 import openc3.script
+from openc3.utilities.script_shared import openc3_script_sleep
+from .telemetry import *
 from .exceptions import CheckError
-from openc3.utilities.extract import (
-    extract_fields_from_check_text,
-    extract_fields_from_tlm_text,
-)
-from openc3.environment import OPENC3_SCOPE
+from openc3.utilities.logger import Logger
+from openc3.utilities.extract import *
+from openc3.environment import *
 
 DEFAULT_TLM_POLLING_RATE = 0.25
 
-# NOTE: The formatting applied throughout uses :.Xf meaning X decimal points
-# This allows extremely small wait times to simply be displayed 0.000.
-# Without the 'f' :.X means display X significant figures
-
 
 def check(*args, type="CONVERTED", scope="DEFAULT"):
     """Check the converted value of a telmetry item against a condition
     Always print the value of the telemetry item to STDOUT
     If the condition check fails, raise an error
     Supports two signatures:
     check(target_name, packet_name, item_name, comparison_to_eval)
@@ -85,25 +83,24 @@
 
 
 def check_exception(method_name, *args, **kwargs):
     """Executes the passed method and expects an exception to be raised.
     Raises a CheckError if an Exception is not raised.
     Usage: check_exception(method_name, method_params}"""
     try:
-        method = method_name
-        orig_kwargs = kwargs.copy()
-        if "scope" not in kwargs:
+        orig_kwargs = kwargs.clone
+        if not kwargs["scope"]:
             kwargs["scope"] = OPENC3_SCOPE
         getattr(sys.modules[__name__], method_name)(*args, **kwargs)
         method = f"{method_name}({', '.join(args)}"
         if orig_kwargs:
             method += f", {orig_kwargs}"
         method += ")"
     except Exception as error:
-        print(f"CHECK: {method} raised {repr(error)}")
+        Logger.info(f"CHECK: {method} raised {repr(error)}")
     else:
         raise CheckError(f"{method} should have raised an exception but did not.")
 
 
 def check_tolerance(*args, type="CONVERTED", scope=OPENC3_SCOPE):
     """Check the converted value of a telmetry item against an expected value with a tolerance
     Always print the value of the telemetry item to STDOUT
@@ -132,56 +129,62 @@
         )
 
         message = ""
         all_checks_ok = True
         for i in range(len(value)):
             range_bottom = expected_value[i] - tolerance[i]
             range_top = expected_value[i] + tolerance[i]
-            check_str = f"CHECK: {_upcase(target_name, packet_name, item_name)}[{i}]"
-            range_str = f"range {_frange(range_bottom)} to {_frange(range_top)} with value == {value[i]}"
+            check_str = "CHECK: {:s}[{:d}]".format(
+                _upcase(target_name, packet_name, item_name), i
+            )
+            range_str = "range {:g} to {:g} with value == {:g}".format(
+                range_bottom, range_top, value[i]
+            )
             if value[i] >= range_bottom and value[i] <= range_top:
-                message += f"{check_str} was within {range_str}\n"
+                message += f"{check_str} was within #{range_str}\n"
             else:
                 message += f"{check_str} failed to be within {range_str}\n"
                 all_checks_ok = False
 
         if all_checks_ok:
-            print(message)
+            Logger.info(message)
         else:
             if openc3.script.DISCONNECT:
-                print(f"ERROR: {message}")
+                Logger.error(message)
             else:
                 raise CheckError(message)
     else:
         range_bottom = expected_value - tolerance
         range_top = expected_value + tolerance
-        check_str = f"CHECK: {_upcase(target_name, packet_name, item_name)}"
-        range_str = f"range {_frange(range_bottom)} to {_frange(range_top)} with value == {value}"
+        check_str = "CHECK: {:s}".format(_upcase(target_name, packet_name, item_name))
+        range_str = "range {:g} to {:g} with value == {:g}".format(
+            range_bottom, range_top, value
+        )
         if value >= range_bottom and value <= range_top:
-            print(f"{check_str} was within {range_str}")
+            Logger.info(f"{check_str} was within {range_str}")
         else:
             message = f"{check_str} failed to be within {range_str}"
             if openc3.script.DISCONNECT:
-                print(f"ERROR: {message}")
+                Logger.error(message)
             else:
                 raise CheckError(message)
 
 
 def check_expression(exp_to_eval, locals=None):
     """Check to see if an expression is true without waiting.  If the expression
     is not true, the script will pause."""
-    success = _openc3_script_wait_expression(
+    success = _openc3_script_wait_implementation_expression(
         exp_to_eval, 0, DEFAULT_TLM_POLLING_RATE, locals
     )
     if success:
-        print(f"CHECK: {exp_to_eval} is TRUE")
+        Logger.info(f"CHECK: {exp_to_eval} is TRUE")
     else:
         message = f"CHECK: {exp_to_eval} is FALSE"
         if openc3.script.DISCONNECT:
-            print(f"ERROR: {message}")
+            Logger.error(message)
         else:
             raise CheckError(message)
 
 
 def wait(*args, type="CONVERTED", quiet=False, scope=OPENC3_SCOPE):
     """Wait on an expression to be true.  On a timeout, the script will continue.
     Supports multiple signatures:
@@ -194,47 +197,45 @@
     match len(args):
         # wait() # indefinitely until they click Go
         case 0:
             start_time = time.time()
             openc3_script_sleep()
             time_diff = time.time() - start_time
             if not quiet:
-                print(f"WAIT: Indefinite for actual time of {time_diff:.3f} seconds")
-            return time_diff
+                Logger.info(f"WAIT: Indefinite for actual time of {time_diff} seconds")
 
         # wait(5) # absolute wait time
         case 1:
             try:
                 value = float(args[0])
             except ValueError:
                 raise RuntimeError("Non-numeric wait time specified")
 
             start_time = time.time()
             openc3_script_sleep(value)
             time_diff = time.time() - start_time
             if not quiet:
-                print(
-                    f"WAIT: {value} seconds with actual time of {time_diff:.3f} seconds"
+                Logger.info(
+                    f"WAIT: {value} seconds with actual time of {time_diff} seconds"
                 )
-            return time_diff
 
         # wait('target_name packet_name item_name > 1', timeout, polling_rate) # polling_rate is optional
         case 2 | 3:
             (
                 target_name,
                 packet_name,
                 item_name,
                 comparison_to_eval,
             ) = extract_fields_from_check_text(args[0])
             timeout = args[1]
             if len(args) == 3:
                 polling_rate = args[2]
             else:
                 polling_rate = DEFAULT_TLM_POLLING_RATE
-            return _execute_wait(
+            _execute_wait(
                 target_name,
                 packet_name,
                 item_name,
                 type,
                 comparison_to_eval,
                 timeout,
                 polling_rate,
@@ -249,15 +250,15 @@
             item_name = args[2]
             comparison_to_eval = args[3]
             timeout = args[4]
             if len(args) == 6:
                 polling_rate = args[5]
             else:
                 polling_rate = DEFAULT_TLM_POLLING_RATE
-            return _execute_wait(
+            _execute_wait(
                 target_name,
                 packet_name,
                 item_name,
                 type,
                 comparison_to_eval,
                 timeout,
                 polling_rate,
@@ -265,14 +266,15 @@
                 scope,
             )
         case _:
             # Invalid number of arguments
             raise RuntimeError(
                 f"ERROR: Invalid number of arguments ({len(args)}) passed to wait()"
             )
+    return time_diff
 
 
 def wait_tolerance(*args, type="CONVERTED", quiet=False, scope=OPENC3_SCOPE):
     """Wait on an expression to be true.  On a timeout, the script will continue.
     Supports multiple signatures:
     wait_tolerance('target_name packet_name item_name', expected_value, tolerance, timeout, polling_rate)
     wait_tolerance('target_name', 'packet_name', 'item_name', expected_value, tolerance, timeout, polling_rate)
@@ -293,15 +295,15 @@
     value = getattr(openc3.script.API_SERVER, "tlm")(
         target_name, packet_name, item_name, type=type, scope=scope
     )
     if isinstance(value, list):
         expected_value, tolerance = _array_tolerance_process_args(
             len(value), expected_value, tolerance, "wait_tolerance"
         )
-        success, value = _openc3_script_wait_array_tolerance(
+        success, value = _openc3_script_wait_implementation_array_tolerance(
             len(value),
             target_name,
             packet_name,
             item_name,
             type,
             expected_value,
             tolerance,
@@ -310,69 +312,81 @@
         )
         time_diff = time.time() - start_time
 
         message = ""
         for i in range(0, len(value)):
             range_bottom = expected_value[i] - tolerance[i]
             range_top = expected_value[i] + tolerance[i]
-            check_str = f"WAIT: {_upcase(target_name, packet_name, item_name)}[{i}]"
-            range_str = f"range {_frange(range_bottom)} to {_frange(range_top)} with value == {value[i]} after waiting {time_diff:.3f} seconds"
+            check_str = "WAIT: {:s}[{:d}]".format(
+                _upcase(target_name, packet_name, item_name), i
+            )
+            range_str = "range {:g} to {:g} with value == {:g} after waiting {:g} seconds".format(
+                range_bottom, range_top, value[i], time_diff
+            )
             if value[i] >= range_bottom and value[i] <= range_top:
-                message += f"{check_str} was within {range_str}\n"
+                message += f"{check_str} was within #{range_str}\n"
             else:
                 message += f"{check_str} failed to be within {range_str}\n"
 
         if not quiet:
             if success:
-                print(message)
+                Logger.info(message)
             else:
-                print(f"WARN: {message}")
+                Logger.warn(message)
     else:
-        success, value = _openc3_script_wait_tolerance(
+        success, value = _openc3_script_wait_implementation_tolerance(
             target_name,
             packet_name,
             item_name,
             type,
             expected_value,
             tolerance,
             timeout,
             polling_rate,
         )
         time_diff = time.time() - start_time
         range_bottom = expected_value - tolerance
         range_top = expected_value + tolerance
-        wait_str = f"WAIT: {_upcase(target_name, packet_name, item_name)}"
-        range_str = f"range {_frange(range_bottom)} to {_frange(range_top)} with value == {value} after waiting {time_diff:.3f} seconds"
+        wait_str = "WAIT: {:s}".format(_upcase(target_name, packet_name, item_name))
+        range_str = (
+            "range {:g} to {:g} with value == {:g} after waiting {:g} seconds".format(
+                range_bottom, range_top, value, time_diff
+            )
+        )
         if not quiet:
             if success:
-                print(f"{wait_str} was within {range_str}")
+                Logger.info(f"{wait_str} was within {range_str}")
             else:
-                print(f"WARN: {wait_str} failed to be within {range_str}")
-    return success
+                Logger.warn(f"{wait_str} failed to be within {range_str}")
+    return time_diff
 
 
 def wait_expression(
     exp_to_eval,
     timeout,
     polling_rate=DEFAULT_TLM_POLLING_RATE,
     locals=None,
     quiet=False,
 ):
     """Wait on a custom expression to be true"""
     start_time = time.time()
-    success = _openc3_script_wait_expression(exp_to_eval, timeout, polling_rate, locals)
+    success = _openc3_script_wait_implementation_expression(
+        exp_to_eval, timeout, polling_rate, locals
+    )
     time_diff = time.time() - start_time
     if not quiet:
         if success:
-            print(f"WAIT: {exp_to_eval} is TRUE after waiting {time_diff:.3f} seconds")
+            Logger.info(
+                f"WAIT: {exp_to_eval} is TRUE after waiting {time_diff} seconds"
+            )
         else:
-            print(
-                f"WARN: WAIT: {exp_to_eval} is FALSE after waiting {time_diff:.3f} seconds"
+            Logger.warn(
+                f"WAIT: {exp_to_eval} is FALSE after waiting {time_diff} seconds"
             )
-    return success
+    return time_diff
 
 
 def wait_check(*args, type="CONVERTED", scope=OPENC3_SCOPE):
     """Wait for the converted value of a telmetry item against a condition or for a timeout
     and then check against the condition
     Supports two signatures:
     wait_check(target_name, packet_name, item_name, comparison_to_eval, timeout, polling_rate)
@@ -383,48 +397,46 @@
         packet_name,
         item_name,
         comparison_to_eval,
         timeout,
         polling_rate,
     ) = _wait_check_process_args(args)
     start_time = time.time()
-    success, value = _openc3_script_wait_value(
+    success, value = openc3_script_wait_implementation(
         target_name,
         packet_name,
         item_name,
         type,
         comparison_to_eval,
         timeout,
         polling_rate,
     )
-    if isinstance(value, str):
-        value = f"'{value}'"  # Show user the check against a quoted string
     time_diff = time.time() - start_time
-    check_str = f"CHECK: {_upcase(target_name, packet_name, item_name)}"
-    if comparison_to_eval:
-        check_str += f" {comparison_to_eval}"
-    with_value_str = f"with value == {value} after waiting {time_diff:.3f} seconds"
+    check_str = "CHECK: {:s} {:s}".format(
+        _upcase(target_name, packet_name, item_name), comparison_to_eval
+    )
+    with_value_str = f"with value == {str(value)} after waiting {time_diff} seconds"
     if success:
-        print(f"{check_str} success {with_value_str}")
+        Logger.info(f"{check_str} success {with_value_str}")
     else:
         message = f"{check_str} failed {with_value_str}"
         if openc3.script.DISCONNECT:
-            print(f"ERROR: {message}")
+            Logger.error(message)
         else:
             raise CheckError(message)
     return time_diff
 
 
 def wait_check_tolerance(*args, type="CONVERTED", scope=OPENC3_SCOPE):
     """Wait for the value of a telmetry item to be within a tolerance of a value
     and then check against the condition.
     Supports two signatures:
-    wait_check_tolerance('target_name packet_name item_name', expected_value, tolerance, timeout, polling_rate)
+    wait_tolerance('target_name packet_name item_name', expected_value, tolerance, timeout, polling_rate)
     or
-    wait_check_tolerance('target_name', 'packet_name', 'item_name', expected_value, tolerance, timeout, polling_rate)
+    wait_tolerance('target_name', 'packet_name', 'item_name', expected_value, tolerance, timeout, polling_rate)
     """
     if type not in ["RAW", "CONVERTED"]:
         raise RuntimeError(f"Invalid type '{type}' for wait_check_tolerance")
 
     (
         target_name,
         packet_name,
@@ -438,15 +450,15 @@
     value = getattr(openc3.script.API_SERVER, "tlm")(
         target_name, packet_name, item_name, type=type, scope=scope
     )
     if isinstance(value, list):
         expected_value, tolerance = _array_tolerance_process_args(
             len(value), expected_value, tolerance, "wait_check_tolerance"
         )
-        success, value = _openc3_script_wait_array_tolerance(
+        success, value = _openc3_script_wait_implementation_array_tolerance(
             len(value),
             target_name,
             packet_name,
             item_name,
             type,
             expected_value,
             tolerance,
@@ -455,115 +467,120 @@
         )
         time_diff = time.time() - start_time
 
         message = ""
         for i in range(0, len(value)):
             range_bottom = expected_value[i] - tolerance[i]
             range_top = expected_value[i] + tolerance[i]
-            check_str = f"CHECK: {_upcase(target_name, packet_name, item_name)}[{i}]"
-            range_str = f"range {_frange(range_bottom)} to {_frange(range_top)} with value == {value[i]} after waiting {time_diff:.3f} seconds"
+            check_str = "WAIT: {:s}[{:d}]".format(
+                _upcase(target_name, packet_name, item_name), i
+            )
+            range_str = "range {:g} to {:g} with value == {:g} after waiting {:g} seconds".format(
+                range_bottom, range_top, value[i], time_diff
+            )
             if value[i] >= range_bottom and value[i] <= range_top:
-                message += f"{check_str} was within {range_str}\n"
+                message += f"{check_str} was within #{range_str}\n"
             else:
                 message += f"{check_str} failed to be within {range_str}\n"
 
         if success:
-            print(message)
+            Logger.info(message)
         else:
             if openc3.script.DISCONNECT:
-                print(f"ERROR: {message}")
+                Logger.error(message)
             else:
                 raise CheckError(message)
     else:
-        success, value = _openc3_script_wait_tolerance(
+        success, value = _openc3_script_wait_implementation_tolerance(
             target_name,
             packet_name,
             item_name,
             type,
             expected_value,
             tolerance,
             timeout,
             polling_rate,
             scope,
         )
         time_diff = time.time() - start_time
         range_bottom = expected_value - tolerance
         range_top = expected_value + tolerance
-        check_str = f"CHECK: {_upcase(target_name, packet_name, item_name)}"
-        range_str = f"range {_frange(range_bottom)} to {_frange(range_top)} with value == {value} after waiting {time_diff:.3f} seconds"
+        check_str = "CHECK: {:s}".format(_upcase(target_name, packet_name, item_name))
+        range_str = (
+            "range {:g} to {:g} with value == {:g} after waiting {:g} seconds".format(
+                range_bottom, range_top, value, time_diff
+            )
+        )
         if success:
-            print(f"{check_str} was within {range_str}")
+            Logger.info(f"{check_str} was within {range_str}")
         else:
             message = f"{check_str} failed to be within {range_str}"
             if openc3.script.DISCONNECT:
-                print(f"ERROR: {message}")
+                Logger.error(message)
             else:
                 raise CheckError(message)
     return time_diff
 
 
 def wait_check_expression(
     exp_to_eval, timeout, polling_rate=DEFAULT_TLM_POLLING_RATE, context=None
 ):
     """Wait on an expression to be true.  On a timeout, the script will pause"""
     start_time = time.time()
-    success = _openc3_script_wait_expression(
+    success = _openc3_script_wait_implementation_expression(
         exp_to_eval, timeout, polling_rate, context
     )
     time_diff = time.time() - start_time
     if success:
-        print(f"CHECK: {exp_to_eval} is TRUE after waiting {time_diff:.3f} seconds")
+        Logger.info(f"CHECK: {exp_to_eval} is TRUE after waiting {time_diff} seconds")
     else:
-        message = f"CHECK: {exp_to_eval} is FALSE after waiting {time_diff:.3f} seconds"
+        message = f"CHECK: {exp_to_eval} is FALSE after waiting {time_diff} seconds"
         if openc3.script.DISCONNECT:
-            print(f"ERROR: {message}")
+            Logger.error(message)
         else:
             raise CheckError(message)
     return time_diff
 
 
 def wait_packet(
     target_name,
     packet_name,
     num_packets,
     timeout,
     polling_rate=DEFAULT_TLM_POLLING_RATE,
     quiet=False,
     scope=OPENC3_SCOPE,
 ):
-    success, _ = _wait_packet(
+    return _wait_packet(
         False,
         target_name,
         packet_name,
         num_packets,
         timeout,
         polling_rate,
         quiet,
         scope,
     )
-    return success
 
 
 def wait_check_packet(
     target_name,
     packet_name,
     num_packets,
     timeout,
     polling_rate=DEFAULT_TLM_POLLING_RATE,
     quiet=False,
     scope=OPENC3_SCOPE,
 ):
     """Wait for a telemetry packet to be received a certain number of times or timeout and raise an error"""
-    _, time_diff = _wait_packet(
+    return _wait_packet(
         True, target_name, packet_name, num_packets, timeout, polling_rate, quiet, scope
     )
-    return time_diff
 
 
-@contextmanager
 def disable_instrumentation():
     if openc3.script.RUNNING_SCRIPT:
         openc3.script.RUNNING_SCRIPT.instance.use_instrumentation = False
         try:
             yield
         finally:
             openc3.script.RUNNING_SCRIPT.instance.use_instrumentation = True
@@ -599,15 +616,15 @@
 
     # TODO:
     # def start(procedure_name)
     #   cached = false
     #   begin
     #     Kernel::load(procedure_name)
     #   rescue LoadError => error
-    #     raise LoadError, f"Error loading -- {procedure_name}\n{error.message}"
+    #     raise LoadError, "Error loading -- #{procedure_name}\n#{error.message}"
     #   end
     #   # Return whether we had to load and instrument this file, i.e. it was not cached
     #   !cached
     # end
 
     # # Require an additional ruby file
     # def load_utility(procedure_name)
@@ -634,24 +651,19 @@
 
 
 ###########################################################################
 # Private implementation details
 ###########################################################################
 
 
-def openc3_script_sleep(sleep_time=None):
-    if sleep_time:
-        time.sleep(float(sleep_time))
-    else:
-        input("Press any key to continue...")
-
-
 def _upcase(target_name, packet_name, item_name):
     """Creates a string with the parameters upcased"""
-    return f"{target_name.upper()} {packet_name.upper()} {item_name.upper()}"
+    return "{:s} {:s} {:s}".format(
+        target_name.upper(), packet_name.upper(), item_name.upper()
+    )
 
 
 def _check(*args, type="CONVERTED", scope=OPENC3_SCOPE):
     """Implementation of the various check commands. It yields back to the
     caller to allow the return of the value through various telemetry calls.
     This method should not be called directly by application code."""
     target_name, packet_name, item_name, comparison_to_eval = _check_process_args(
@@ -661,46 +673,43 @@
         target_name, packet_name, item_name, type=type, scope=scope
     )
     if comparison_to_eval:
         return _check_eval(
             target_name, packet_name, item_name, comparison_to_eval, value
         )
     else:
-        print(f"CHECK: {_upcase(target_name, packet_name, item_name)} == {value}")
+        Logger.info(
+            "CHECK: %s == %s", _upcase(target_name, packet_name, item_name), str(value)
+        )
 
 
 def _check_process_args(args, method_name):
     match len(args):
         case 1:
             (
                 target_name,
                 packet_name,
                 item_name,
                 comparison_to_eval,
             ) = extract_fields_from_check_text(args[0])
-        case 3:
-            target_name = args[0]
-            packet_name = args[1]
-            item_name = args[2]
-            comparison_to_eval = None
         case 4:
             target_name = args[0]
             packet_name = args[1]
             item_name = args[2]
             comparison_to_eval = args[3]
         case _:
             # Invalid number of arguments
             raise RuntimeError(
                 f"ERROR: Invalid number of arguments ({len(args)}) passed to {method_name}()"
             )
-    if comparison_to_eval and not comparison_to_eval.isascii():
+    if not comparison_to_eval.isascii():
         raise RuntimeError(
-            f"ERROR: Invalid comparison to non-ascii value: {comparison_to_eval}"
+            f"Invalid comparison to non-ascii value: {comparison_to_eval}"
         )
-    return target_name, packet_name, item_name, comparison_to_eval
+    return [target_name, packet_name, item_name, comparison_to_eval]
 
 
 def _check_tolerance_process_args(args):
     length = len(args)
     if length == 3:
         target_name, packet_name, item_name = extract_fields_from_tlm_text(args[0])
         expected_value = args[1]
@@ -718,15 +727,15 @@
         else:
             tolerance = abs(args[4])
     else:
         # Invalid number of arguments
         raise RuntimeError(
             f"ERROR: Invalid number of arguments ({length}) passed to check_tolerance()"
         )
-    return target_name, packet_name, item_name, expected_value, tolerance
+    return [target_name, packet_name, item_name, expected_value, tolerance]
 
 
 def _wait_packet(
     check,
     target_name,
     packet_name,
     num_packets,
@@ -740,18 +749,18 @@
         type = "CHECK"
     else:
         type = "WAIT"
     initial_count = getattr(openc3.script.API_SERVER, "tlm")(
         target_name, packet_name, "RECEIVED_COUNT", scope=scope
     )
     # If the packet has not been received the initial_count could be None
-    if initial_count is None:
+    if not initial_count:
         initial_count = 0
     start_time = time.time()
-    success, value = _openc3_script_wait_value(
+    success, value = openc3_script_wait_implementation(
         target_name,
         packet_name,
         "RECEIVED_COUNT",
         "CONVERTED",
         f">= {initial_count + num_packets}",
         timeout,
         polling_rate,
@@ -759,64 +768,76 @@
     )
     # If the packet has not been received the value could be None
     if not value:
         value = 0
     time_diff = time.time() - start_time
     if success:
         if not quiet:
-            print(
-                f"{type}: {target_name.upper()} {packet_name.upper()} received {value - initial_count} times after waiting {time_diff:.3f} seconds"
+            Logger.info(
+                "{:s}: {:s} {:s} received {:d} times after waiting {:g} seconds".format(
+                    type,
+                    target_name.upper(),
+                    packet_name.upper(),
+                    value - initial_count,
+                    time_diff,
+                )
             )
     else:
-        message = f"{type}: {target_name.upper()} {packet_name.upper()} expected to be received {num_packets} times but only received {value - initial_count} times after waiting {time_diff:.3f} seconds"
+        message = "{:s}: {:s} {:s} expected to be received {:d} times but only received {:d} times after waiting {:g} seconds".format(
+            type,
+            target_name.upper(),
+            packet_name.upper(),
+            num_packets,
+            value - initial_count,
+            time_diff,
+        )
         if check:
             if openc3.script.DISCONNECT:
-                print(f"ERROR: {message}")
+                Logger.error(message)
             else:
                 raise CheckError(message)
         elif not quiet:
-            print(f"WARN: {message}")
-    return success, time_diff
+            Logger.warn(message)
+    return time_diff
 
 
 def _execute_wait(
     target_name,
     packet_name,
     item_name,
     value_type,
     comparison_to_eval,
     timeout,
     polling_rate,
     quiet,
     scope,
 ):
     start_time = time.time()
-    success, value = _openc3_script_wait_value(
+    success, value = openc3_script_wait_implementation(
         target_name,
         packet_name,
         item_name,
         value_type,
         comparison_to_eval,
         timeout,
         polling_rate,
         scope,
     )
     if type(value) == str:
         value = f"'{value}'"  # Show user the check against a quoted string
     time_diff = time.time() - start_time
-    wait_str = (
-        f"WAIT: {_upcase(target_name, packet_name, item_name)} {comparison_to_eval}"
+    wait_str = "WAIT: {:s} {:s}".format(
+        _upcase(target_name, packet_name, item_name), comparison_to_eval
     )
-    value_str = f"with value == {value} after waiting {time_diff:.3f} seconds"
+    value_str = f"with value == {value} after waiting {time_diff} seconds"
     if not quiet:
         if success:
-            print(f"{wait_str} success {value_str}")
+            Logger.info(f"{wait_str} success {value_str}")
         else:
-            print(f"WARN: {wait_str} failed {value_str}")
-    return success
+            Logger.warn(f"{wait_str} failed {value_str}")
 
 
 def _wait_tolerance_process_args(args, function_name):
     length = len(args)
     if length == 4 or length == 5:
         target_name, packet_name, item_name = extract_fields_from_tlm_text(args[0])
         expected_value = args[1]
@@ -842,25 +863,27 @@
         if length == 7:
             polling_rate = args[6]
         else:
             polling_rate = DEFAULT_TLM_POLLING_RATE
     else:
         # Invalid number of arguments
         raise RuntimeError(
-            f"ERROR: Invalid number of arguments ({length}) passed to {function_name}()"
+            "ERROR: Invalid number of arguments ({:d}) passed to {:s}()".format(
+                length, function_name
+            )
         )
-    return (
+    return [
         target_name,
         packet_name,
         item_name,
         expected_value,
         tolerance,
         timeout,
         polling_rate,
-    )
+    ]
 
 
 def _array_tolerance_process_args(array_size, expected_value, tolerance, function_name):
     """
     When testing an array with a tolerance, the expected value and tolerance
     can both be supplied as either an array or a single value.  If a single
     value is passed in, that value will be used for all array elements.
@@ -875,15 +898,15 @@
     if isinstance(tolerance, list):
         if array_size != len(tolerance):
             raise RuntimeError(
                 f"ERROR: Invalid array size for tolerance passed to {function_name}()"
             )
     else:
         tolerance = [tolerance] * array_size
-    return expected_value, tolerance
+    return [expected_value, tolerance]
 
 
 def _wait_check_process_args(args):
     length = len(args)
     if length == 2 or length == 3:
         (
             target_name,
@@ -907,52 +930,47 @@
         else:
             polling_rate = DEFAULT_TLM_POLLING_RATE
     else:
         # Invalid number of arguments
         raise RuntimeError(
             f"ERROR: Invalid number of arguments ({len(args)}) passed to wait_check()"
         )
-    return (
+    return [
         target_name,
         packet_name,
         item_name,
         comparison_to_eval,
         timeout,
         polling_rate,
-    )
+    ]
 
 
-def _openc3_script_wait(
+def _openc3_script_wait_implementation(
     target_name,
     packet_name,
     item_name,
     value_type,
     timeout,
     polling_rate,
     exp_to_eval,
     scope,
 ):
     value = None
     end_time = time.time() + timeout
-    if exp_to_eval and not exp_to_eval.isascii():
-        raise RuntimeError("ERROR: Invalid comparison to non-ascii value")
+    if not exp_to_eval.isascii():
+        raise RuntimeError("Invalid comparison to non-ascii value")
 
     try:
         while True:
             work_start = time.time()
             value = getattr(openc3.script.API_SERVER, "tlm")(
                 target_name, packet_name, item_name, type=value_type, scope=scope
             )
-            try:
-                if eval(exp_to_eval):
-                    return True, value
-            # We get TypeError when trying to eval None >= 0 (for example)
-            # In this case we just continue and see if eventually we get a good value from tlm()
-            except TypeError:
-                pass
+            if eval(exp_to_eval):
+                return [True, value]
             if time.time() >= end_time:
                 break
 
             delta = time.time() - work_start
             sleep_time = polling_rate - delta
             end_delta = end_time - time.time()
             if end_delta < sleep_time:
@@ -961,115 +979,120 @@
                 sleep_time = 0
             canceled = openc3_script_sleep(sleep_time)
 
             if canceled:
                 value = getattr(openc3.script.API_SERVER, "tlm")(
                     target_name, packet_name, item_name, type=value_type, scope=scope
                 )
-                try:
-                    if eval(exp_to_eval):
-                        return True, value
-                    else:
-                        return False, value
-                # We get TypeError when trying to eval None >= 0 (for example)
-                except TypeError:
-                    return False, value
+                if eval(exp_to_eval):
+                    return [True, value]
+                else:
+                    return [False, value]
 
     except NameError as error:
         parts = error.args[0].split("'")
         new_error = NameError(
             f"Uninitialized constant {parts[1]}. Did you mean '{parts[1]}' as a string?"
         )
         raise new_error from error
 
-    return False, value
+    return [False, value]
 
 
 # Wait for a converted telemetry item to pass a comparison
-def _openc3_script_wait_value(
+def openc3_script_wait_implementation(
     target_name,
     packet_name,
     item_name,
     value_type,
     comparison_to_eval,
     timeout,
     polling_rate=DEFAULT_TLM_POLLING_RATE,
     scope=OPENC3_SCOPE,
 ):
     if comparison_to_eval:
         exp_to_eval = "value " + comparison_to_eval
     else:
         exp_to_eval = None
-    return _openc3_script_wait(
+    return _openc3_script_wait_implementation(
         target_name,
         packet_name,
         item_name,
         value_type,
         timeout,
         polling_rate,
         exp_to_eval,
         scope,
     )
 
 
-def _openc3_script_wait_tolerance(
+def _openc3_script_wait_implementation_tolerance(
     target_name,
     packet_name,
     item_name,
     value_type,
     expected_value,
     tolerance,
     timeout,
     polling_rate=DEFAULT_TLM_POLLING_RATE,
     scope=OPENC3_SCOPE,
 ):
-    exp_to_eval = f"(value >= ({expected_value} - {abs(tolerance)}) and value <= ({expected_value} + {abs(tolerance)}))"
-    return _openc3_script_wait(
+    exp_to_eval = "(value >= ({:g} - {:g}) and value <= ({:g} + {:g}))".format(
+        expected_value, abs(tolerance), expected_value, abs(tolerance)
+    )
+    return _openc3_script_wait_implementation(
         target_name,
         packet_name,
         item_name,
         value_type,
         timeout,
         polling_rate,
         exp_to_eval,
         scope,
     )
 
 
-def _openc3_script_wait_array_tolerance(
+def _openc3_script_wait_implementation_array_tolerance(
     array_size,
     target_name,
     packet_name,
     item_name,
     value_type,
     expected_value,
     tolerance,
     timeout,
     polling_rate=DEFAULT_TLM_POLLING_RATE,
     scope=OPENC3_SCOPE,
 ):
     statements = []
     for i in range(array_size):
         statements.append(
-            f"(value[{i}] >= ({expected_value[i]} - {abs(tolerance[i])}) and value[{i}] <= ({expected_value[i]} + {abs(tolerance[i])}))"
+            "(value >= ({:g} - {:g}) and value <= ({:g} + {:g}))".format(
+                expected_value[i],
+                abs(tolerance[i]),
+                expected_value[i],
+                abs(tolerance[i]),
+            )
         )
     exp_to_eval = " and ".join(statements)
-    return _openc3_script_wait(
+    return _openc3_script_wait_implementation(
         target_name,
         packet_name,
         item_name,
         value_type,
         timeout,
         polling_rate,
         exp_to_eval,
         scope,
     )
 
 
-def _openc3_script_wait_expression(exp_to_eval, timeout, polling_rate, locals=None):
+def _openc3_script_wait_implementation_expression(
+    exp_to_eval, timeout, polling_rate, locals=None
+):
     """Wait on an expression to be true."""
     end_time = time.time() + timeout
     if not exp_to_eval.isascii():
         raise RuntimeError(f"Invalid comparison to non-ascii value: {exp_to_eval}")
 
     try:
         while True:
@@ -1101,50 +1124,32 @@
         raise new_error from error
 
     return None
 
 
 def _check_eval(target_name, packet_name, item_name, comparison_to_eval, value):
     string = "value " + comparison_to_eval
-    check_str = (
-        f"CHECK: {_upcase(target_name, packet_name, item_name)} {comparison_to_eval}"
+    check_str = "CHECK: {:s} {:s}".format(
+        _upcase(target_name, packet_name, item_name), comparison_to_eval
     )
     # Show user the check against a quoted string
     # Note: We have to preserve the original 'value' variable because we're going to eval against it
     if isinstance(value, str):
         value_str = f"'{value}'"
     else:
         value_str = value
     with_value = f"with value == {value_str}"
     try:
         if eval(string):
-            print(f"{check_str} success {with_value}")
+            Logger.info(f"{check_str} success {with_value}")
         else:
             message = f"{check_str} failed {with_value}"
             if openc3.script.DISCONNECT:
-                print(f"ERROR: {message}")
+                Logger.error(message)
             else:
                 raise CheckError(message)
     except NameError as error:
         parts = error.args[0].split("'")
         new_error = NameError(
             f"Uninitialized constant {parts[1]}. Did you mean '{parts[1]}' as a string?"
         )
         raise new_error from error
-
-
-def _frange(value):
-    if isinstance(value, float):
-        # Display at most 6 significant figures on a range value
-        # This truncates float values like 1.6500000000000001 to simply 1.65
-        return f"{value:.6}"
-    else:
-        return value
-
-
-# Interesting formatter to a specific number of significant digits:
-# https://stackoverflow.com/questions/3410976/how-to-round-a-number-to-significant-figures-in-python?rq=3
-# def format(value, sigfigs=9):
-#     if isinstance(value, float):
-#         return "{:.{p}g}".format(float("{:.{p}g}".format(value, p=sigfigs)), p=sigfigs)
-#     else:
-#         return value
```

### Comparing `openc3-5.16.0/openc3/script/authorization.py` & `openc3-5.9.2b0/openc3/script/authorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2022 Ball Aerospace & Technologies Corp.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
```

### Comparing `openc3-5.16.0/openc3/script/commands.py` & `openc3-5.9.2b0/openc3/script/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -10,23 +12,140 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-from datetime import datetime
 import openc3.script
 from openc3.environment import OPENC3_SCOPE
 from openc3.top_level import HazardousError
+from openc3.utilities.logger import Logger
 from openc3.utilities.extract import *
+
 from openc3.packets.packet import Packet
 
 
+# Format the command like it appears in a script
+def _cmd_string(target_name, cmd_name, cmd_params, raw):
+    output_string = ""
+    if openc3.script.DISCONNECT:
+        output_string += "openc3.script.DISCONNECT: "
+    if raw:
+        output_string += 'cmd_raw("'
+    else:
+        output_string += 'cmd("'
+    output_string += target_name + " " + cmd_name
+    if not cmd_params:
+        output_string += '")'
+    else:
+        params = []
+        for key, value in cmd_params.items():
+            if key in Packet.RESERVED_ITEM_NAMES:
+                continue
+            if type(value) == str:
+                value = convert_to_value(value)
+                if len(value) > 256:
+                    value = value[:255] + "...'"
+                if not value.isascii():
+                    value = "BINARY"
+                value = value.replace('"', "'")
+            elif type(value) == list:
+                value = f"[{', '.join(value)}]"
+            params.append(f"{key} {value}")
+        params = ", ".join(params)
+        output_string += " with " + params + '")'
+    return output_string
+
+
+def _log_cmd(target_name, cmd_name, cmd_params, raw, no_range, no_hazardous):
+    """Log any warnings about disabling checks and log the command itself
+    NOTE: This is a helper method and should not be called directly"""
+    if no_range:
+        Logger.warn(
+            f"Command {target_name} {cmd_name} being sent ignoring range checks"
+        )
+    if no_hazardous:
+        Logger.warn(
+            f"Command {target_name} {cmd_name} being sent ignoring hazardous warnings"
+        )
+    Logger.info(_cmd_string(target_name, cmd_name, cmd_params, raw))
+
+
+def _cmd_disconnect(cmd, raw, no_range, no_hazardous, *args, scope):
+    match len(args):
+        case 1:
+            target_name, cmd_name, cmd_params = extract_fields_from_cmd_text(args[0])
+        case 2 | 3:
+            target_name = args[0]
+            cmd_name = args[1]
+            if len(args) == 2:
+                cmd_params = {}
+            else:
+                cmd_params = args[2]
+        case _:
+            # Invalid number of arguments
+            raise RuntimeError(
+                f"ERROR: Invalid number of arguments ({len(args)}) passed to {cmd}()"
+            )
+
+    # Get the command and validate the parameters
+    command = openc3.script.API_SERVER.get_command(target_name, cmd_name, scope=scope)
+    if cmd_params:
+        for param_name in cmd_params.keys():
+            found = False
+            if "items" in command:
+                for item in command["items"]:
+                    if item["name"] == param_name:
+                        found = item
+                        break
+            if not found:
+                raise RuntimeError(
+                    f"Packet item '{target_name} {cmd_name} {param_name}' does not exist"
+                )
+    _log_cmd(target_name, cmd_name, cmd_params, raw, no_range, no_hazardous)
+
+
+def _cmd(cmd, cmd_no_hazardous, *args, scope=OPENC3_SCOPE, timeout=None):
+    """Send the command and log the results
+    # This method signature has to include the keyword params present in cmd_api.py cmd_implementation()
+    NOTE: This is a helper method and should not be called directly"""
+    print(f"_cmd:{cmd} args:{args} scope:{scope} timeout:{timeout}")
+
+    raw = "raw" in cmd
+    no_range = "no_range" in cmd or "no_checks" in cmd
+    no_hazardous = "no_hazardous" in cmd or "no_checks" in cmd
+
+    if openc3.script.DISCONNECT:
+        _cmd_disconnect(cmd, raw, no_range, no_hazardous, *args, scope=scope)
+    else:
+        try:
+            print(f"command:{cmd} args:{args}")
+            target_name, cmd_name, cmd_params = getattr(openc3.script.API_SERVER, cmd)(
+                *args, timeout=timeout, scope=scope
+            )
+            _log_cmd(target_name, cmd_name, cmd_params, raw, no_range, no_hazardous)
+        except HazardousError as error:
+            # Need to reimport here to pick up changes from running_script
+            from openc3.utilities.script_shared import prompt_for_hazardous
+
+            ok_to_proceed = prompt_for_hazardous(
+                error.target_name,
+                error.cmd_name,
+                error.hazardous_description,
+            )
+            if ok_to_proceed:
+                target_name, cmd_name, cmd_params = getattr(
+                    openc3.script.API_SERVER, cmd_no_hazardous
+                )(*args, scope=scope, timeout=timeout)
+                _log_cmd(target_name, cmd_name, cmd_params, raw, no_range, no_hazardous)
+
+
 def cmd(*args, **kwargs):
+    print(f"CMD args:{args} kwargs:{kwargs}")
     """Send a command to the specified target
     Usage:
       cmd(target_name, cmd_name, cmd_params = {})
     or
       cmd('target_name cmd_name with cmd_param1 value1, cmd_param2 value2')
     """
     return _cmd("cmd", "cmd_no_hazardous_check", *args, **kwargs)
@@ -98,160 +217,43 @@
       cmd_raw_no_checks(target_name, cmd_name, cmd_params = {})
     or
       cmd_raw_no_checks('target_name cmd_name with cmd_param1 value1, cmd_param2 value2')
     """
     return _cmd("cmd_raw_no_checks", None, *args, **kwargs)
 
 
-def build_cmd(*args, **kwargs):
+def build_command(*args, **kwargs):
     """Builds a command binary
     Accepts two different calling styles:
     build_command("TGT CMD with PARAM1 val, PARAM2 val")
     build_command('TGT','CMD',{'PARAM1'=>val,'PARAM2'=>val})"""
     extract_string_kwargs_to_args(args, kwargs)
-    return getattr(openc3.script.API_SERVER, "build_cmd")(*args)
-
-
-# build_command is DEPRECATED
-build_command = build_cmd
+    return getattr(openc3.script.API_SERVER, "build_command")(*args)
 
 
 def get_cmd_hazardous(*args, **kwargs):
     """Returns whether a command is hazardous (true or false)"""
     extract_string_kwargs_to_args(args, kwargs)
     return getattr(openc3.script.API_SERVER, "get_cmd_hazardous")(*args)
 
 
+def send_raw_file(interface_name, filename, scope=OPENC3_SCOPE):
+    """Sends raw data through an interface from a file"""
+    with open(filename, "rb") as file:
+        data = file.read()
+    return getattr(openc3.script.API_SERVER, "send_raw")(
+        interface_name, data, scope=scope
+    )
+
+
 # Returns the time the most recent command was sent
 def get_cmd_time(target_name=None, command_name=None, scope=OPENC3_SCOPE):
     results = getattr(openc3.script.API_SERVER, "get_cmd_time")(
         target_name, command_name, scope=scope
     )
-    results = list(results)
-    if results[2] and results[3]:
-        results[2] = datetime.fromtimestamp(results[2] + results[3] / 1000000)
+    if type(results) == list:
+        if results[2] and results[3]:
+            pass
+            # TODO: Python Time.at equivalent?
+            # results[2] = Time.at(results[2], results[3]).sys
         results.pop(3)
     return results
-
-
-# Format the command like it appears in a script
-def _cmd_string(target_name, cmd_name, cmd_params, raw):
-    output_string = ""
-    if openc3.script.DISCONNECT:
-        output_string += "openc3.script.DISCONNECT: "
-    if raw:
-        output_string += 'cmd_raw("'
-    else:
-        output_string += 'cmd("'
-    output_string += target_name + " " + cmd_name
-    if not cmd_params:
-        output_string += '")'
-    else:
-        params = []
-        for key, value in cmd_params.items():
-            if key in Packet.RESERVED_ITEM_NAMES:
-                continue
-            if type(value) == str:
-                value = convert_to_value(value)
-                if len(value) > 256:
-                    value = value[:255] + "...'"
-                if not value.isascii():
-                    value = "BINARY"
-                value = value.replace('"', "'")
-            elif type(value) == list:
-                value = str(value)
-            params.append(f"{key} {value}")
-        params = ", ".join(params)
-        output_string += " with " + params + '")'
-    return output_string
-
-
-def _log_cmd(target_name, cmd_name, cmd_params, raw, no_range, no_hazardous):
-    """Log any warnings about disabling checks and log the command itself
-    NOTE: This is a helper method and should not be called directly"""
-    if no_range:
-        print(
-            f"WARN: Command {target_name} {cmd_name} being sent ignoring range checks"
-        )
-    if no_hazardous:
-        print(
-            f"WARN: Command {target_name} {cmd_name} being sent ignoring hazardous warnings"
-        )
-    print(_cmd_string(target_name, cmd_name, cmd_params, raw))
-
-
-def _cmd_disconnect(cmd, raw, no_range, no_hazardous, *args, scope):
-    match len(args):
-        case 1:
-            target_name, cmd_name, cmd_params = extract_fields_from_cmd_text(args[0])
-        case 2 | 3:
-            target_name = args[0]
-            cmd_name = args[1]
-            if len(args) == 2:
-                cmd_params = {}
-            else:
-                cmd_params = args[2]
-        case _:
-            # Invalid number of arguments
-            raise RuntimeError(
-                f"ERROR: Invalid number of arguments ({len(args)}) passed to {cmd}()"
-            )
-
-    # Get the command and validate the parameters
-    command = openc3.script.API_SERVER.get_cmd(target_name, cmd_name, scope=scope)
-    if cmd_params:
-        for param_name in cmd_params.keys():
-            found = False
-            if "items" in command:
-                for item in command["items"]:
-                    if item["name"] == param_name:
-                        found = item
-                        break
-            if not found:
-                raise RuntimeError(
-                    f"Packet item '{target_name} {cmd_name} {param_name}' does not exist"
-                )
-    _log_cmd(target_name, cmd_name, cmd_params, raw, no_range, no_hazardous)
-
-
-def _cmd(
-    cmd,
-    cmd_no_hazardous,
-    *args,
-    timeout=None,
-    log_message=None,
-    scope=OPENC3_SCOPE,
-):
-    """Send the command and log the results
-    # This method signature has to include the keyword params present in cmd_api.py cmd_implementation()
-    NOTE: This is a helper method and should not be called directly"""
-
-    raw = "raw" in cmd
-    no_range = "no_range" in cmd or "no_checks" in cmd
-    no_hazardous = "no_hazardous" in cmd or "no_checks" in cmd
-
-    if openc3.script.DISCONNECT:
-        _cmd_disconnect(cmd, raw, no_range, no_hazardous, *args, scope=scope)
-    else:
-        try:
-            target_name, cmd_name, cmd_params = getattr(openc3.script.API_SERVER, cmd)(
-                *args, timeout=timeout, log_message=log_message, scope=scope
-            )
-            if log_message is None or log_message:
-                _log_cmd(target_name, cmd_name, cmd_params, raw, no_range, no_hazardous)
-        except HazardousError as error:
-            # Need to reimport here to pick up changes from running_script
-            from openc3.script import prompt_for_hazardous
-
-            ok_to_proceed = prompt_for_hazardous(
-                error.target_name,
-                error.cmd_name,
-                error.hazardous_description,
-            )
-            if ok_to_proceed:
-                target_name, cmd_name, cmd_params = getattr(
-                    openc3.script.API_SERVER, cmd_no_hazardous
-                )(*args, scope=scope, timeout=timeout)
-                if log_message is None or log_message:
-                    _log_cmd(
-                        target_name, cmd_name, cmd_params, raw, no_range, no_hazardous
-                    )
```

### Comparing `openc3-5.16.0/openc3/script/decorators.py` & `openc3-5.9.2b0/openc3/script/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,36 @@
+#!/usr/bin/env python3
+# vim: tabstop=8 expandtab shiftwidth=4 softtabstop=4
+# -*- coding: latin-1 -*-
+"""
+decorators.py
+"""
+
 # Copyright 2022 Ball Aerospace & Technologies Corp.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Lesser General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 
 # Modified by OpenC3, Inc.
-# All changes Copyright 2023, OpenC3, Inc.
+# All changes Copyright 2022, OpenC3, Inc.
 # All Rights Reserved
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import functools
 import requests
+import logging
+
+from openc3.__version__ import __title__
+
+logger = logging.getLogger(__title__)
 
 
 def request_wrapper(func):
     @functools.wraps(func)
     def _request(*args, **kwargs):
         try:
             value = func(*args, **kwargs)
```

### Comparing `openc3-5.16.0/openc3/script/exceptions.py` & `openc3-5.9.2b0/openc3/api/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,24 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
-#
+
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
+WHITELIST = []
 
-class CheckError(Exception):
-    pass
-
-
-class StopScript(Exception):
-    pass
-
-
-class SkipScript(Exception):
-    pass
+from .cmd_api import *
+from .tlm_api import *
+from .interface_api import *
+from .stash_api import *
```

### Comparing `openc3-5.16.0/openc3/script/limits.py` & `openc3-5.9.2b0/openc3/script/limits.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -10,28 +12,28 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-from openc3.script import DISCONNECT
-from openc3.script import API_SERVER as API_SERVER
 
 LIMITS_METHODS = [
     "enable_limits",
     "disable_limits",
     "set_limits",
     "enable_limits_group",
     "disable_limits_group",
     "set_limits_set",
 ]
 
 # Define all the modification methods such that we can disconnect them
 for method in LIMITS_METHODS:
     code = [f"def {method}(*args, **kwargs):"]
-    if DISCONNECT:
-        code.append(f"        print('DISCONNECT: {method}(args) ignored')")
-    else:
-        code.append(f"        return getattr(API_SERVER, '{method}')(*args, **kwargs)")
+    code.append("    if openc3.script.DISCONNECT:")
+    code.append(f"        Logger.info('DISCONNECT: {method}(args) ignored')")
+    code.append("    else:")
+    code.append(
+        f"        return getattr(openc3.script.API_SERVER, '{method}')(*args, **kwargs)"
+    )
     function = compile("\n".join(code), "<string>", "exec")
     exec(function, globals())
```

### Comparing `openc3-5.16.0/openc3/script/metadata.py` & `openc3-5.9.2b0/openc3/script/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python3
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -58,15 +61,15 @@
 # @param metadata [Hash<Symbol, Variable>] A hash of metadata
 # @param start [Integer] Metadata time value as integer seconds from epoch
 # @param color [String] Events color to show on Calendar tool, if None will be blue
 # @return The result of the method call.
 def metadata_set(metadata, start=None, color=None, scope=OPENC3_SCOPE):
     if type(metadata) != dict:
         raise RuntimeError(
-            f"metadata must be a dict: {metadata} is a {metadata.__class__.__name__}"
+            f"metadata must be a Hash: {metadata} is a {metadata.__class__.__name__}"
         )
 
     if not color:
         color = "#003784"
     data = {"color": color, "metadata": metadata}
     if start:
         data["start"] = time.asctime(time.gmtime(start))
@@ -92,15 +95,15 @@
 # @return The result of the method call.
 def metadata_update(metadata, start=None, color=None, scope=OPENC3_SCOPE):
     if type(metadata) != dict:
         raise RuntimeError(
             f"metadata must be a Hash: {metadata} is a {metadata.__class__.__name__}"
         )
 
-    if start is None:  # No start so grab latest
+    if not start:  # No start so grab latest
         existing = metadata_get()
         start = existing["start"]
         if not color:
             color = existing["color"]
         metadata = existing["metadata"] | metadata
     else:
         if not color:
```

### Comparing `openc3-5.16.0/openc3/script/screen.py` & `openc3-5.9.2b0/openc3/script/screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
```

### Comparing `openc3-5.16.0/openc3/script/server_proxy.py` & `openc3-5.9.2b0/openc3/script/server_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -36,16 +38,16 @@
 
     def generate_timeout(self):
         """pull openc3-cosmos-cmd-tlm-api timeout from environment variables"""
         return float(OPENC3_API_TIMEOUT)
 
     # generate the auth object
     def generate_auth(self):
-        if OPENC3_API_TOKEN is None and OPENC3_API_USER is None:
-            if OPENC3_API_PASSWORD:
+        if OPENC3_API_TOKEN == None and OPENC3_API_USER == None:
+            if OPENC3_API_PASSWORD or OPENC3_SERVICE_PASSWORD:
                 return OpenC3Authentication()
             else:
                 return None
         else:
             return OpenC3KeycloakAuthentication(OPENC3_KEYCLOAK_URL)
 
     # Create a JsonDRbObject connection to the API server
@@ -63,24 +65,25 @@
                 kwargs["scope"] = OPENC3_SCOPE
             match func:
                 case "shutdown":
                     return self.json_drb.shutdown()
                 case "request":
                     return self.json_drb.request(*args, **kwargs)
                 case _:
-                    disconnect = kwargs.pop("disconnect", None)
                     if openc3.script.DISCONNECT:
+                        result = None
+                        disconnect = kwargs.pop("disconnect", None)
+                        # The only commands allowed through in disconnect mode are read-only
+                        # Thus we allow the get, list, tlm and limits_enabled and subscribe methods
+                        if re.compile(
+                            r"get_\w*|list_\w*|^tlm|limits_enabled|subscribe"
+                        ).match(func):
+                            result = getattr(self.json_drb, func)(*args, **kwargs)
+                        # If they overrode the return value using the disconnect keyword then return that
                         if disconnect:
                             return disconnect
                         else:
-                            # The only commands allowed through in disconnect mode are read-only
-                            # Thus we allow the get, list, tlm and limits_enabled and subscribe methods
-                            if re.compile(
-                                r"\w*_get$|^get_\w*|\w*_list$|^list_\w*|^tlm|^limits_enabled$|^subscribe$"
-                            ).match(func):
-                                return getattr(self.json_drb, func)(*args, **kwargs)
-                            else:
-                                return None
+                            return result
                     else:
                         return getattr(self.json_drb, func)(*args, **kwargs)
 
         return method
```

### Comparing `openc3-5.16.0/openc3/script/storage.py` & `openc3-5.9.2b0/openc3/script/storage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Copyright 2024 OpenC3, Inc.
+#!/usr/bin/env python3
+
+# Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 #
@@ -12,39 +14,39 @@
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import os
 import json
-import tempfile
 import requests
 from openc3.utilities.extract import *
 import openc3.script
 from openc3.environment import OPENC3_SCOPE
+from openc3.utilities.logger import Logger
 from openc3.utilities.local_mode import LocalMode
 
 OPENC3_CLOUD = os.environ.get("OPENC3_CLOUD") or "local"
 
 
 # Delete a file on a target
 #
 # @param [String] Path to a file in a target directory
 def delete_target_file(path, scope=OPENC3_SCOPE):
     try:
         # Only delete from the targets_modified
         delete_path = f"{scope}/targets_modified/{path}"
         endpoint = f"/openc3-api/storage/delete/{delete_path}"
-        print(f"Deleting {delete_path}")
+        Logger.info(f"Deleting {delete_path}")
         # Pass the name of the ENV variable name where we pull the actual bucket name
         response = openc3.script.API_SERVER.request(
             "delete", endpoint, query={"bucket": "OPENC3_CONFIG_BUCKET"}, scope=scope
         )
-        if not response or response.status_code != 200:
-            raise Exception(f"Failed to delete {delete_path}")
+        if not response or response.status != 200:
+            raise Exception("Failed to delete {delete_path}")
     except Exception as error:
         raise Exception(f"Failed deleting {path} due to {repr(error)}") from error
     return None
 
 
 # Get a handle to write a target file
 #
@@ -52,150 +54,127 @@
 # @param io_or_string [Io or String] IO object
 def put_target_file(path, io_or_string, scope=OPENC3_SCOPE):
     if ".." in path:
         raise Exception(f"Disallowed path modifier '..' found in {path}")
 
     upload_path = f"{scope}/targets_modified/{path}"
 
-    if os.getenv("OPENC3_LOCAL_MODE") and openc3.script.OPENC3_IN_CLUSTER:
+    if os.environ["OPENC3_LOCAL_MODE"] and openc3.script.OPENC3_IN_CLUSTER:
         LocalMode.put_target_file(upload_path, io_or_string, scope=scope)
-        if hasattr(io_or_string, "read"):  # not str or bytes
-            io_or_string.seek(0)
+        # TODO: Python respond_to?
+        # if io_or_string.respond_to?(:rewind):
+        #   io_or_string.rewind
 
     endpoint = f"/openc3-api/storage/upload/{upload_path}"
     result = _get_presigned_request(endpoint, scope=scope)
-    print(f"Writing {upload_path}")
+    Logger.info(f"Writing {upload_path}")
 
     # Try to put the file
     try:
         uri = _get_uri(result["url"])
         with requests.Session() as s:
-            if hasattr(io_or_string, "read"):
-                # TODO: Better way to get io size?
-                io_or_string.seek(0, 2)  # Jump to end
-                length = io_or_string.tell()
-                io_or_string.seek(0)
-                io_or_string = io_or_string.read()
-            else:  # str or bytes
-                length = len(io_or_string)
             result = s.put(
                 uri,
                 data=io_or_string,
-                headers={"Content-Length": str(length)},
+                headers={"Content-Length": str(len(io_or_string))},
             )
             return result.content
+            # Net::HTTP.start(uri.host, uri.port) do
+            # request = Net::HTTP::Put.new(uri, {'Content-Length' => io_or_string.length.to_s})
+            # if String === io_or_string
+            #   request.body = io_or_string
+            # else
+            #   request.body_stream = io_or_string
+
+            # Net::HTTP.start(uri.host, uri.port, use_ssl: uri.scheme == 'https') do |http|
+            #   http.request(request) do |response|
+            #     response.value() # Raises an HTTP error if the response is not 2xx (success)
+            #     return response
     except Exception as error:
         raise Exception(
             f"Failed to write {upload_path} due to {repr(error)}"
         ) from error
 
 
 # Get a handle to access a target file
 #
 # @param path [String] Path to a file in a target directory, e.g. "INST/procedures/test.rb"
 # @param original [Boolean] Whether to get the original or modified file
 # @return [File|None]
 def get_target_file(path, original=False, scope=OPENC3_SCOPE):
     part = "targets"
-    if original is False:
+    if not original:
         part += "_modified"
     # Loop to allow redo when switching from modified to original
-    while True:
+    while 1:
         try:
-            if part == "targets_modified" and os.getenv("OPENC3_LOCAL_MODE"):
+            if part == "targets_modified" and os.environ["OPENC3_LOCAL_MODE"]:
                 local_file = LocalMode.open_local_file(path, scope=scope)
                 if local_file:
-                    print(f"Reading local {scope}/{part}/{path}")
-                    file = tempfile.NamedTemporaryFile(mode="w+b")
+                    Logger.info(f"Reading local {scope}/{path}")
+                    file = open(path, "wb")
                     file.write(local_file.read())
-                    file.seek(0)  # Rewind so the file is ready to read
+                    file.close()
                     return file
-            return _get_storage_file(f"{part}/{path}", scope=scope)
+            return _get_storage_file("{part}/{path}", scope=scope)
         except Exception as error:
             if part == "targets_modified":
                 part = "targets"
                 # redo
             else:
                 raise error
 
 
-def get_download_url(path, scope=OPENC3_SCOPE):
-    targets = "targets_modified"  # First try targets_modified
-    response = openc3.script.API_SERVER.request(
-        "get",
-        f"/openc3-api/storage/exists/{scope}/{targets}/{path}",
-        query={"bucket": "OPENC3_CONFIG_BUCKET"},
-        scope=scope,
-    )
-
-    if response.status_code != 200:
-        targets = "targets"  # Next try targets
-        response = openc3.script.API_SERVER.request(
-            "get",
-            f"/openc3-api/storage/exists/{scope}/{targets}/{path}",
-            query={"bucket": "OPENC3_CONFIG_BUCKET"},
-            scope=scope,
-        )
-        if response.status_code != 200:
-            raise RuntimeError(f"File not found: {path} in scope: {scope}")
-    endpoint = f"/openc3-api/storage/download/{scope}/{targets}/{path}"
-    # external must be true because we're using this URL from the frontend
-    result = _get_presigned_request(endpoint, external=True, scope=scope)
-    return result["url"]
-
+# download_file(path_or_file) is implemented by running_script to download a file
 
 # These are helper methods ... should not be used directly
 
 
 def _get_storage_file(path, scope=OPENC3_SCOPE):
     # Create Tempfile to store data
-    file = tempfile.NamedTemporaryFile(mode="w+b")
+    file = open(path, "wb")
 
     endpoint = f"/openc3-api/storage/download/{scope}/{path}"
     result = _get_presigned_request(endpoint, scope=scope)
-    print(f"Reading {scope}/{path}")
+    Logger.info(f"Reading {scope}/{path}")
 
     # Try to get the file
     uri = _get_uri(result["url"])
-    response = requests.get(uri)
-    if response.status_code == 404:
-        raise RuntimeError(f"File not found: {scope}/{path}")
-    file.write(response.content)
-    file.seek(0)
+    with requests.Session() as s:
+        response = s.get(uri)
+        for chunk in response.iter_content:
+            file.write(chunk)
+    file.close()
     return file
 
 
 def _get_uri(url):
     if openc3.script.OPENC3_IN_CLUSTER:
         match OPENC3_CLOUD:
             case "local":
-                bucket_url = os.environ.get(
-                    "OPENC3_BUCKET_URL", "http://openc3-minio:9000"
-                )
-                return f"{bucket_url}{url}"
+                return f"http://openc3-minio:9000{url}"
             case "aws":
-                return f"https://s3.{os.getenv('AWS_REGION')}.amazonaws.com{url}"
+                return f"https://s3.{os.environ['AWS_REGION']}.amazonaws.com{url}"
             case "gcp":
                 return f"https://storage.googleapis.com{url}"
             # when 'azure'
             case _:
                 raise Exception(f"Unknown cloud {OPENC3_CLOUD}")
     else:
-        return f"{openc3.script.API_SERVER.generate_url()}{url}"
+        return f"{openc3.script.API_SERVER.generate_url}url"
 
 
-def _get_presigned_request(endpoint, external=None, scope=OPENC3_SCOPE):
-    if external or not openc3.script.OPENC3_IN_CLUSTER:
-        response = openc3.script.API_SERVER.request(
-            "get", endpoint, query={"bucket": "OPENC3_CONFIG_BUCKET"}, scope=scope
-        )
-    else:
+def _get_presigned_request(endpoint, scope=OPENC3_SCOPE):
+    if openc3.script.OPENC3_IN_CLUSTER:
         response = openc3.script.API_SERVER.request(
             "get",
             endpoint,
             query={"bucket": "OPENC3_CONFIG_BUCKET", "internal": True},
             scope=scope,
         )
-
-    if not response or response.status_code != 201:
+    else:
+        response = openc3.script.API_SERVER.request(
+            "get", endpoint, query={"bucket": "OPENC3_CONFIG_BUCKET"}, scope=scope
+        )
+    if not response or response.status != 201:
         raise Exception(f"Failed to get presigned URL for {endpoint}")
-    return json.loads(response.text)
+    return json.loads(response.body)
```

### Comparing `openc3-5.16.0/openc3/script/stream.py` & `openc3-5.9.2b0/openc3/script/stream.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+#!/usr/bin/env python3
+# vim: tabstop=8 expandtab shiftwidth=4 softtabstop=4
+# -*- coding: latin-1 -*-
+"""
+stream.py
+"""
+
 # Copyright 2022 Ball Aerospace & Technologies Corp.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Lesser General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 
 # Modified by OpenC3, Inc.
-# All changes Copyright 2023, OpenC3, Inc.
+# All changes Copyright 2022, OpenC3, Inc.
 # All Rights Reserved
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import asyncio
 import json
@@ -56,15 +63,15 @@
         self.auth = generate_auth() if auth is None else auth
         self._tasks = {}
         self._events = {}
         self._queues = {}
         self._loop = asyncio.new_event_loop()
         self._stop_event = asyncio.Event()
 
-        if schema == "http":
+        if (schema == "http"):
             self._url = f"ws://{hostname}:{port}"
         else:
             self._url = f"wss://{hostname}:{port}"
 
     def run(self):
         """
         Should be called from the thread.start() method.
@@ -146,18 +153,15 @@
         Parameters:
             endpoint (str): example: /openc3-api/cable
             sub_msg (dict): json based message to send
             callback (callable): method/function to call with data
         """
         url = f"{self._url}{endpoint}"
         try:
-            ws = await websockets.connect(
-                f"{url}?scope={OPENC3_SCOPE}&authorization={self.auth.get()}",
-                loop=self._loop,
-            )
+            ws = await websockets.connect(f"{url}?scope={OPENC3_SCOPE}&authorization={self.auth.get()}", loop=self._loop)
             await self._welcome(ws)
             await self._confirm(ws, sub_msg)
             await self._handle(endpoint, ws, callback)
             await ws.close()
         except asyncio.CancelledError:
             logging.info(f"{endpoint} has been canceled")
         except CosmosAsyncStop:
```

### Comparing `openc3-5.16.0/openc3/script/stream_shared.py` & `openc3-5.9.2b0/openc3/script/stream_shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+#!/usr/bin/env python3
+# vim: tabstop=8 expandtab shiftwidth=4 softtabstop=4
+# -*- coding: latin-1 -*-
+"""
+stream_api.py
+"""
+
 # Copyright 2022 Ball Aerospace & Technologies Corp.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Lesser General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 
 # Modified by OpenC3, Inc.
-# All changes Copyright 2023, OpenC3, Inc.
+# All changes Copyright 2022, OpenC3, Inc.
 # All Rights Reserved
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import json
```

### Comparing `openc3-5.16.0/openc3/script/suite.py` & `openc3-5.9.2b0/openc3/script/suite.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -16,74 +18,76 @@
 
 import sys
 import copy
 import re
 from io import StringIO
 from openc3.script.exceptions import StopScript, SkipScript
 import openc3.script
-from openc3.io.stdout import Stdout
-from openc3.io.stderr import Stderr
 
 
 class Suite:
     """Base class for Script Runner suites. OpenC3 Suites inherit from Suite
     and can implement setup and teardown methods. Script groups are added via add_group(Group)
     and individual scripts added via add_script(Group, script_method)."""
 
     def scripts(self):
-        if not hasattr(self, "_scripts"):
-            self._scripts = {}
-        return self._scripts
+        if not self.scripts:
+            self.scripts = {}
+        return self.scripts
 
     def plans(self):
-        if not hasattr(self, "_plans"):
-            self._plans = []
-        return self._plans
+        if not self.plans:
+            self.plans = []
+        return self.plans
 
     ###########################################################################
     # START PUBLIC API
     ###########################################################################
 
     # Explictly avoid creating an initialize method which forces users to call super()
 
     # Add a group to the suite
     def add_group(self, group_class):
+        self.scripts()
+        self.plans()
         if not group_class.__class__ == type:
-            raise RuntimeError("add_group must be given Class not String in Python")
-        if not self.scripts().get(group_class, None):
-            self.scripts()[group_class] = group_class()
-        self.plans().append(["GROUP", group_class, None])
+            group_class = globals()[group_class]
+        if not self.scripts.get(group_class, None):
+            self.scripts[group_class] = group_class()
+        self.plans.append(["GROUP", group_class, None])
 
     # Add a script to the suite
     def add_script(self, group_class, script):
+        self.scripts()
+        self.plans()
         if not group_class.__class__ == type:
-            raise RuntimeError("add_script must be given Class not String in Python")
-        if not self.scripts().get(group_class, None):
-            self.scripts()[group_class] = group_class()
-        self.plans().append(["SCRIPT", group_class, script])
+            group_class = globals()[group_class]
+        if not self.scripts.get(group_class, None):
+            self.scripts[group_class] = group_class()
+        self.plans.append(["SCRIPT", group_class, script])
 
     # Add a group setup to the suite
     def add_group_setup(self, group_class):
+        self.scripts()
+        self.plans()
         if not group_class.__class__ == type:
-            raise RuntimeError(
-                "add_group_setup must be given Class not String in Python"
-            )
-        if not self.scripts().get(group_class, None):
-            self.scripts()[group_class] = group_class()
-        self.plans().append(["GROUP_SETUP", group_class, None])
+            group_class = globals()[group_class]
+        if not self.scripts.get(group_class, None):
+            self.scripts[group_class] = group_class()
+        self.plans.append(["GROUP_SETUP", group_class, None])
 
     # Add a group teardown to the suite
     def add_group_teardown(self, group_class):
+        self.scripts()
+        self.plans()
         if not group_class.__class__ == type:
-            raise RuntimeError(
-                "add_group_teardown must be given Class not String in Python"
-            )
-        if not self.scripts().get(group_class, None):
-            self.scripts()[group_class] = group_class()
-        self.plans().append(["GROUP_TEARDOWN", group_class, None])
+            group_class = globals()[group_class]
+        if not self.scripts.get(group_class, None):
+            self.scripts[group_class] = group_class()
+        self.plans.append(["GROUP_TEARDOWN", group_class, None])
 
     ###########################################################################
     # END PUBLIC API
     ###########################################################################
 
     def __eq__(self, other):
         return self.name == other.name
@@ -94,90 +98,85 @@
             return self.__class__.__name__
         else:
             return "UnassignedSuite"
 
     # Returns the number of scripts in the suite including setup and teardown methods
     def get_num_scripts(self):
         num_scripts = 0
-        for type, group_class, _ in self.plans():
+        for type, group_class, _ in self.plans:
             if type == "GROUP":
                 num_scripts += group_class.get_num_scripts()
             else:
                 num_scripts += 1
 
         if hasattr(self, "setup"):
             num_scripts += 1
         if hasattr(self, "teardown"):
             num_scripts += 1
         return num_scripts
 
     # Run all the scripts
     def run(self):
         ScriptResult.suite = self.name()
-        ScriptStatus.instance().total = self.get_num_scripts()
+        ScriptStatus.instance.total = self.get_num_scripts()
         results = []
 
         # Setup the suite
         result = self.run_setup(True)
         if result:
             results.append(result)
-            yield result
-            if result.stopped:
-                raise StopScript
+        yield result
+        if result.stopped:
+            raise StopScript
 
         # Run each script
         for type, group_class, script in self.plans():
             match type:
                 case "GROUP":
-                    for result in self.run_group(group_class, True):
-                        results.append(result)
-                        yield result
-                        if result.stopped:
-                            raise StopScript
+                    results.append(self.run_group(group_class, True))
                 case "SCRIPT":
                     result = self.run_script(group_class, script, True)
                     results.append(result)
                     yield result
                     if (
                         result.exceptions and group_class.abort_on_exception
                     ) or result.stopped:
                         raise StopScript
                 case "GROUP_SETUP":
                     result = self.run_group_setup(group_class, True)
                     if result:
                         results.append(result)
-                        yield result
-                        if (
-                            result.exceptions and group_class.abort_on_exception
-                        ) or result.stopped:
-                            raise StopScript
+                    yield result
+                    if (
+                        result.exceptions and group_class.abort_on_exception
+                    ) or result.stopped:
+                        raise StopScript
 
                 case "GROUP_TEARDOWN":
                     result = self.run_group_teardown(group_class, True)
                     if result:
                         results.append(result)
-                        yield result
-                        if (
-                            result.exceptions and group_class.abort_on_exception
-                        ) or result.stopped:
-                            raise StopScript
+                    yield result
+                    if (
+                        result.exceptions and group_class.abort_on_exception
+                    ) or result.stopped:
+                        raise StopScript
 
         # Teardown the suite
         result = self.run_teardown(True)
         if result:
             results.append(result)
-            yield result
-            if result.stopped:
-                raise StopScript
+        yield result
+        if result.stopped:
+            raise StopScript
         ScriptResult.suite = None
         return results
 
     # Run a specific group
     def run_group(self, group_class, internal=False):
-        results = []
         if not internal:
             ScriptResult.suite = self.name()
 
         # Determine if this group_class is in the plan and the number of scripts associated with this group_class
         in_plan = False
         num_scripts = 0
         for plan_type, plan_group_class, plan_script in self.plans():
@@ -189,23 +188,20 @@
                 or (plan_type == "GROUP_TEARDOWN" and group_class == plan_group_class)
                 or (plan_script and group_class == plan_group_class)
             ):
                 num_scripts += 1
 
         if in_plan:
             if not internal:
-                ScriptStatus.instance().total = group_class.get_num_scripts()
-            for result in self.scripts()[group_class].run():
-                results.append(result)
-                yield result
-                if result.stopped:
-                    raise StopScript
+                ScriptStatus.instance.total = group_class.get_num_scripts()
+            results = self.scripts[group_class].run()
         else:
+            results = []
             if not internal:
-                ScriptStatus.instance().total = num_scripts
+                ScriptStatus.instance.total = num_scripts
 
             # Run each setup, teardown, or script associated with this group_class in the order
             # defined in the plan
             for plan_type, plan_group_class, plan_script in self.plans():
                 if plan_group_class == group_class:
                     match plan_type:
                         case "SCRIPT":
@@ -214,82 +210,80 @@
                             )
                             results.append(result)
                             yield result
                         case "GROUP_SETUP":
                             result = self.run_group_setup(plan_group_class, True)
                             if result:
                                 results.append(result)
-                                yield result
+                            yield result
 
                         case "GROUP_TEARDOWN":
                             result = self.run_group_teardown(plan_group_class, True)
                             if result:
                                 results.append(result)
-                                yield result
+                            yield result
         if not internal:
             ScriptResult.suite = None
         return results
 
     # Run a specific script
     def run_script(self, group_class, script, internal=False):
         if not internal:
             ScriptResult.suite = self.name()
         if not internal:
-            ScriptStatus.instance().total = 1
-        result = self.scripts()[group_class].run_script(script)
+            ScriptStatus.instance.total = 1
+        result = self.scripts[group_class].run_script(script)
         if not internal:
             ScriptResult.suite = None
         return result
 
     def run_setup(self, internal=False):
         if not internal:
             ScriptResult.suite = self.name()
         result = None
-        if "setup" in dir(self) and len(self.scripts()) > 0:
+        if "setup" in self.__class__ and self.scripts.length > 0:
             if not internal:
-                ScriptStatus.instance().total = 1
-            ScriptStatus.instance().status = f"{self.__class__.__name__} : setup"
-            # Get the first group
-            result = next(iter(self.scripts().values())).run_method(self, "setup")
+                ScriptStatus.instance.total = 1
+            ScriptStatus.instance.status = f"{self.__class__.__name__} : setup"
+            result = self.scripts[self.scripts.keys[0]].run_method(self, "setup")
 
         if not internal:
             ScriptResult.suite = None
         return result
 
     def run_teardown(self, internal=False):
         if not internal:
             ScriptResult.suite = self.name()
         result = None
-        if "teardown" in dir(self) and len(self.scripts()) > 0:
+        if "teardown" in self.__class__ and self.scripts.length > 0:
             if not internal:
-                ScriptStatus.instance().total = 1
-            ScriptStatus.instance().status = f"{self.__class__} : teardown"
-            # Get the first group
-            result = next(iter(self.scripts().values())).run_method(self, "teardown")
+                ScriptStatus.instance.total = 1
+            ScriptStatus.instance.status = f"{self.__class__} : teardown"
+            result = self.scripts[self.scripts.keys[0]].run_method(self, "teardown")
 
         if not internal:
             ScriptResult.suite = None
         return result
 
     def run_group_setup(self, group_class, internal=False):
         if not internal:
             ScriptResult.suite = self.name()
         if not internal:
-            ScriptStatus.instance().total = 1
-        result = self.scripts()[group_class].run_setup()
+            ScriptStatus.instance.total = 1
+        result = self.scripts[group_class].run_setup()
         if not internal:
             ScriptResult.suite = None
         return result
 
     def run_group_teardown(self, group_class, internal=False):
         if not internal:
             ScriptResult.suite = self.name()
         if not internal:
-            ScriptStatus.instance().total = 1
-        result = self.scripts()[group_class].run_teardown()
+            ScriptStatus.instance.total = 1
+        result = self.scripts[group_class].run_teardown()
         if not internal:
             ScriptResult.suite = None
         return result
 
 
 class Group:
     """Base class for a group. All OpenC3 Script Runner scripts should inherit Group
@@ -300,24 +294,19 @@
     current_result = None
 
     # Explictly avoid creating an initialize method which forces users to call super()
 
     @classmethod
     def scripts(cls):
         # Find all the script methods
-        result = [
+        return [
             func
             for func in dir(cls)
-            if callable(getattr(cls, func))
-            and re.search(r"^test|^script|op_", func)
-            and func != "scripts"
-            and func != "test_cases"
-        ]
-        result.sort()
-        return result
+            if callable(getattr(cls, func)) and re.search(r"^test|^script|op_", func)
+        ].sort()
 
     # Name of the script group
     def name(self):
         if self.__class__ != Group:
             return self.__class__.__name__
         else:
             return "UnnamedGroup"
@@ -326,167 +315,142 @@
     def run(self):
         results = []
 
         # Setup the script group
         result = self.run_setup()
         if result:
             results.append(result)
-            yield result
-            if (results[-1].exceptions and Group.abort_on_exception) or results[
-                -1
-            ].stopped:
-                raise StopScript
+        yield result
+        if (results[-1].exceptions and Group.abort_on_exception) or results[-1].stopped:
+            raise StopScript
 
         # Run all the scripts
         for method_name in self.__class__.scripts():
-            results.append(self.run_script(method_name))
+            results << self.run_script(method_name)
             yield results[-1]
             if (results[-1].exceptions and Group.abort_on_exception) or results[
                 -1
             ].stopped:
                 raise StopScript
 
         # Teardown the script group
         result = self.run_teardown()
         if result:
             results.append(result)
-            yield result
-            if (results[-1].exceptions and Group.abort_on_exception) or results[
-                -1
-            ].stopped:
-                raise StopScript
+        yield result
+        if (results[-1].exceptions and Group.abort_on_exception) or results[-1].stopped:
+            raise StopScript
         return results
 
     # Run a specific script method
     def run_script(self, method_name):
-        ScriptStatus.instance().status = f"{self.__class__.__name__} : {method_name}"
-        return self.run_method(self, method_name)
+        ScriptStatus.instance.status = f"{self.__class__.__name__} : {method_name}"
+        self.run_method(self, method_name)
 
     def run_method(self, object, method_name):
         result = ScriptResult()
         Group.current_result = result
 
         # Verify script method exists
         if hasattr(object.__class__, method_name):
-            if hasattr(self, "output_io"):
-                self.output_io = self.output_io or StringIO("")
-            else:
-                self.output_io = StringIO("")
-
+            self.output_io = self.output_io or StringIO("")
             # Capture STDOUT and STDERR
-            sys.stdout = Stdout.instance()
-            sys.stderr = Stderr.instance()
             sys.stdout.add_stream(self.output_io)
             sys.stderr.add_stream(self.output_io)
 
             result.group = object.__class__.__name__
             result.script = method_name
             try:
-                method = getattr(object, method_name)
-                method()
+                object.public_send(method_name)
                 result.result = "PASS"
 
                 if (
-                    openc3.script.RUNNING_SCRIPT
+                    openc3.script.RUNNING_SCRIPT.instance
                     and openc3.script.RUNNING_SCRIPT.instance.exceptions
                 ):
                     result.exceptions = openc3.script.RUNNING_SCRIPT.instance.exceptions
                     result.result = "FAIL"
                     openc3.script.RUNNING_SCRIPT.instance.exceptions = None
 
             except Exception as error:
                 # Check that the error belongs to the StopScript inheritance chain
-                if issubclass(error.__class__, StopScript):
+                if issubclass(error, StopScript):
                     result.stopped = True
                     result.result = "STOP"
                 # Check that the error belongs to the SkipScript inheritance chain
-                if issubclass(error.__class__, SkipScript):
+                elif issubclass(error, SkipScript):
                     result.result = "SKIP"
-                    if hasattr(error, "message"):
-                        result.message = result.message or ""
-                        result.message += error.message + "\n"
+                    result.message = result.message or ""
+                    result.message += error.message + "\n"
                 else:
-                    if not issubclass(error.__class__, StopScript) and (
-                        not openc3.script.RUNNING_SCRIPT
-                        or not openc3.script.RUNNING_SCRIPT.instance
+                    if (
+                        not openc3.script.RUNNING_SCRIPT.instance
                         or not openc3.script.RUNNING_SCRIPT.instance.exceptions
                         or error not in openc3.script.RUNNING_SCRIPT.instance.exceptions
                     ):
                         result.exceptions = result.exceptions or []
                         result.exceptions.append(error)
+                        print("*** Exception in Control Statement:")
+                        print(repr(error))
                     if (
-                        openc3.script.RUNNING_SCRIPT
-                        and openc3.script.RUNNING_SCRIPT.instance
+                        openc3.script.RUNNING_SCRIPT.instance
                         and openc3.script.RUNNING_SCRIPT.instance.exceptions
                     ):
                         result.exceptions = result.exceptions or []
-                        result.exceptions.extend(
+                        result.exceptions.append(
                             openc3.script.RUNNING_SCRIPT.instance.exceptions
                         )
                         openc3.script.RUNNING_SCRIPT.instance.exceptions = None
                 if result.exceptions:
                     result.result = "FAIL"
             finally:
-                result.output = self.output_io.getvalue()
-                self.output_io.truncate(0)
-                self.output_io.seek(0)
+                result.output = self.output_io.string
+                self.output_io.string = ""
                 sys.stdout.remove_stream(self.output_io)
                 sys.stdout.remove_stream(self.output_io)
 
                 match result.result:
                     case "FAIL":
-                        ScriptStatus.instance().fail_count += 1
+                        ScriptStatus.instance.fail_count += 1
                     case "SKIP":
-                        ScriptStatus.instance().skip_count += 1
+                        ScriptStatus.instance.skip_count += 1
                     case "PASS":
-                        ScriptStatus.instance().pass_count += 1
+                        ScriptStatus.instance.pass_count += 1
         else:
             Group.current_result = None
             raise Exception(f"Unknown method {method_name} for {object.__class__}")
         Group.current_result = None
         return result
 
     def run_setup(self):
-        result = None
-        if "setup" in dir(self):
-            ScriptStatus.instance().status = f"{self.__class__} : setup"
-            result = self.run_script("setup")
-        return result
+        if "setup" in self.__class__:
+            ScriptStatus.instance.status = f"{self.__class__} : setup"
+        return self.run_script("setup")
 
     def run_teardown(self):
-        result = None
-        if "teardown" in dir(self):
-            ScriptStatus.instance().status = f"{self.__class__} : teardown"
-            result = self.run_script("teardown")
-        return result
+        if "teardown" in self.__class__:
+            ScriptStatus.instance.status = f"{self.__class__} : teardown"
+        return self.run_script("teardown")
 
     @classmethod
     def get_num_scripts(cls):
         num_scripts = 0
-        if "setup" in dir(cls):
+        if "setup" in cls:
             num_scripts += 1
-        if "teardown" in dir(cls):
+        if "teardown" in cls:
             num_scripts += 1
         num_scripts += len(cls.scripts())
         return num_scripts
 
     @classmethod
     def puts(cls, string):
-        print(string, file=sys.stdout)
+        sys.stdout.print(string)
         if Group.current_result:
             Group.current_result.message = Group.current_result.message or ""
-            Group.current_result.message += string.rstrip("\n")
-            Group.current_result.message += "\n"
-
-    @classmethod
-    def print(cls, string):
-        print(string, file=sys.stdout)
-        if Group.current_result:
-            Group.current_result.message = Group.current_result.message or ""
-            Group.current_result.message += string.rstrip("\n")
+            Group.current_result.message += string.chomp
             Group.current_result.message += "\n"
 
     @classmethod
     def current_suite(cls):
         if Group.current_result:
             return Group.current_result.suite
         else:
@@ -514,30 +478,29 @@
     def __init__(self):
         self.status = ""
         self.pass_count = 0
         self.skip_count = 0
         self.fail_count = 0
         self.total = 1
 
-    @classmethod
     def instance(cls):
         if ScriptStatus.instance_obj:
             return ScriptStatus.instance_obj
-        ScriptStatus.instance_obj = cls()
+        ScriptStatus.instance_obj = cls.__init__()
         return ScriptStatus.instance_obj
 
 
 # Helper class to collect script result information
 class ScriptResult:
     suite = None
 
     def __init__(self):
         self.suite = None
         if ScriptResult.suite:
-            ScriptResult.suite = copy.deepcopy(ScriptResult.suite)
+            self.suite = copy.deepcopy(ScriptResult.suite)
         self.group = None
         self.script = None
         self.output = None
         self.exceptions = None
         self.stopped = False
         self.result = "SKIP"
         self.message = None
```

### Comparing `openc3-5.16.0/openc3/script/suite_results.py` & `openc3-5.9.2b0/openc3/script/suite_results.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Copyright 2024 OpenC3, Inc.
+#!/usr/bin/env python3
+
+# Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 #
@@ -12,25 +14,23 @@
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import re
 import time
-from datetime import datetime, timezone
+from datetime import datetime
 from openc3.utilities.extract import remove_quotes
-import traceback
 
 
 class SuiteResults:
     metadata = None
-    context = None
 
     def __init__(self):
-        self._report = None
+        self.report = None
         self.context = None
         self.start_time = None
         self.stop_time = None
         self.results = None
         self.settings = None
         self.metadata = None
 
@@ -41,27 +41,27 @@
         test_class=None,
         test_case=None,
         settings=None,
     ):
         self.results = []
         self.start_time = time.time()
         self.settings = settings
-        self._report = []
+        self.report = []
 
         if test_case:
-            # Executing a script
-            self.context = f"{test_suite_class.__name__}:{test_class.__name__}:{test_case} {test_type}"
-        elif test_class:
-            # Executing a group
+            # Executing a single test case
             self.context = (
-                f"{test_suite_class.__name__}:{test_class.__name__} {test_type}"
+                f"{test_suite_class.name()}:{test_class.name()}:{test_case} {test_type}"
             )
+        elif test_class:
+            # Executing an entire test
+            self.context = f"{test_suite_class.name()}:{test_class.name()} {test_type}"
         else:
-            # Executing a suite
-            self.context = f"{test_suite_class.__name__} {test_type}"
+            # Executing a test suite
+            self.context = f"{test_suite_class.name()} {test_type}"
         self.header()
 
     # process_result can handle an array of OpenC3TestResult objects
     # or a single OpenC3TestResult object
     def process_result(self, results):
         # If we were passed an array we concat it to the results global
         if type(results) == list:
@@ -71,62 +71,62 @@
             self.results.append(results)
             results = [results]
 
         # Process all the results (may be just one)
         for result in results:
             self.puts(f"{result.group}:{result.script}:{result.result}")
             if result.message:
-                for line in result.message.split("\n"):
+                for line in result.message:
                     if re.search(r"\x00-\x08\x0B-\x0C\x0E-\x1F\x7F-\xFF", line):
-                        line = line.rstrip("\n")
-                        line = remove_quotes(repr(line))
-                    self._report.append("  " + line.strip())
+                        line = line.rstrip()
+                        line = remove_quotes(line)
+                    self.report += "  " + line.rstrip()
 
             if result.exceptions:
-                self._report.append("  Exceptions:")
+                self.report += "  Exceptions:"
                 for index, error in enumerate(result.exceptions):
-                    self._report.extend(traceback.format_exception(error))
+                    self.report += repr(error)
                     # for line in repr(error):
                     #   next if /in run_text/.match?(line)
                     #   next if /running_script.rb/.match?(line)
                     #   next if line&.match?(openc3_lib)
 
                     #   if /[\x00-\x08\x0B-\x0C\x0E-\x1F\x7F-\xFF]/.match?(line)
                     #     line.chomp!
                     #     line = line.inspect.remove_quotes
 
-                    #   self._report += '    ' + line.rstrip()
+                    #   self.report += '    ' + line.rstrip()
                     # if index != (result.exceptions.length - 1):
-                    #   self._report += ''
+                    #   self.report += ''
 
     def complete(self):
         self.stop_time = time.time()
         self.footer()
 
     def report(self):
-        return "\n".join(self._report)
+        return "\n".join(self.report)
 
     def header(self):
-        self._report.append("--- Script Report ---")
+        self.report += "--- Script Report ---"
         if self.settings:
-            self._report.append("")
-            self._report.append("Settings:")
-            for setting_name, setting_value in self.settings.items():
-                self._report.append(f"{setting_name} = {setting_value}")
+            self.report += ""
+            self.report += "Settings:"
+            for setting_name, setting_value in self.settings:
+                self.report += f"{setting_name} = {setting_value}"
 
-        self._report.append("")
-        self._report.append("Results:")
+        self.report += ""
+        self.report += "Results:"
         self.puts(f"Executing {self.context}")
 
     def footer(self):
         self.puts(f"Completed {self.context}")
 
-        self._report.append("")
-        self._report.append("--- Test Summary ---")
-        self._report.append("")
+        self.report += ""
+        self.report += "--- Test Summary ---"
+        self.report += ""
 
         pass_count = 0
         skip_count = 0
         fail_count = 0
         stopped = False
         for result in self.results:
             if result.result == "PASS":
@@ -135,26 +135,22 @@
                 skip_count += 1
             elif result.result == "FAIL":
                 fail_count += 1
             if result.stopped:
                 stopped = True
 
         run_time = self.stop_time - self.start_time
-        self._report.append(f"Run Time: {run_time}")
-        self._report.append(f"Total Tests: {len(self.results)}")
-        self._report.append(f"Pass: {pass_count}")
-        self._report.append(f"Skip: {skip_count}")
-        self._report.append(f"Fail: {fail_count}")
-        self._report.append("")
+        self.report += f"Run Time: {run_time}"
+        self.report += f"Total Tests: {len(self.results)}"
+        self.report += f"Pass: {pass_count}"
+        self.report += f"Skip: {skip_count}"
+        self.report += f"Fail: {fail_count}"
+        self.report += ""
         if stopped:
-            self._report.append("*** Test was stopped prematurely ***")
-            self._report.append("")
+            self.report += "*** Test was stopped prematurely ***"
+            self.report += ""
 
     def write(self, string):
-        # Can't use isoformat because it appends "+00:00" instead of "Z"
-        self._report.append(
-            datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%S.%fZ") + ": " + string
-        )
-
-    # Define a few aliases
-    puts = write
-    print = write
+        self.report += datetime.now().isoformat(" ") + ": " + string
+
+    def puts(self, string):
+        self.report += datetime.now().isoformat(" ") + ": " + string
```

### Comparing `openc3-5.16.0/openc3/script/suite_runner.py` & `openc3-5.9.2b0/openc3/script/suite_runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -11,18 +13,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 from .suite import Suite, Group, ScriptStatus
-from openc3.tools.test_runner.test import TestSuite, Test
 from .suite_results import SuiteResults
 from openc3.script.exceptions import StopScript
-import inspect
 
 
 class UnassignedSuite(Suite):
     """Placeholder for all Groups discovered without assigned Suites"""
 
     pass
 
@@ -43,15 +43,15 @@
                     group_class,
                     script,
                     SuiteRunner.settings,
                 )
                 while True:
                     yield (suite)
                     if not SuiteRunner.settings["Loop"] or (
-                        ScriptStatus.instance().fail_count > 0
+                        ScriptStatus.instance.fail_count > 0
                         and SuiteRunner.settings["Break Loop On Error"]
                     ):
                         break
                 break
 
     @classmethod
     def start(cls, suite_class, group_class=None, script=None):
@@ -64,15 +64,15 @@
                     raise StopScript
             elif group_class:
                 for result in suite.run_group(group_class):
                     SuiteRunner.suite_results.process_result(result)
                     if result.stopped:
                         raise StopScript
             else:
-                for result in suite.run():
+                for result in suite.run:
                     SuiteRunner.suite_results.process_result(result)
                     if result.stopped:
                         raise StopScript
 
     @classmethod
     def setup(cls, suite_class, group_class=None):
         for suite in cls.execute("Manual Setup", suite_class, group_class):
@@ -95,169 +95,160 @@
                 result = suite.run_teardown
 
             if result:
                 SuiteRunner.suite_results.process_result(result)
                 if result.stopped:
                     raise StopScript
 
+    # # Convert the OpenStruct structure to a simple hash
+    # # TODO: Maybe just use hashes right from the beginning?
+    # def self.open_struct_to_hash(object)
+    #   hash = object.to_h
+    #   hash.each do |key1, val1|
+    #     if val1.is_a?(Hash)
+    #       val1.each do |key2, val2|
+    #         if val2.is_a?(OpenStruct)
+    #           hash[key1][key2] = val2.to_h
+
+    #   hash
+
     # Build list of Suites and Groups
     @classmethod
-    def build_suites(cls, from_module=None, from_globals=None):
+    def build_suites(cls):
         SuiteRunner.suites = []
         suites = {}
         groups = []
-
-        if from_module:
-            for attr_name in dir(from_module):
-                object = getattr(from_module, attr_name)
-                if not inspect.isclass(object):
-                    continue
-
-                # If we inherit from Suite
-                if (
-                    issubclass(object, Suite)
-                    and object != Suite
-                    and object != TestSuite
-                ):
-                    SuiteRunner.suites.insert(0, object())
-
-                # If we inherit from Group
-                if issubclass(object, Group) and object != Group and object != Test:
-                    groups.append(object)
-
-        if from_globals:
-            for object in from_globals.values():
-                if not inspect.isclass(object):
-                    continue
-
-                # If we inherit from Suite
-                if (
-                    issubclass(object, Suite)
-                    and object != Suite
-                    and object != TestSuite
-                ):
-                    SuiteRunner.suites.insert(0, object())
-
-                # If we inherit from Group
-                if issubclass(object, Group) and object != Group and object != Test:
-                    groups.append(object)
+        # TODO: This is only the current namespace where Ruby was everything
+        # How do we get all the objects?
+        for object in globals():
+            # If we inherit from Suite
+            if isinstance(object, Suite):
+                # Ensure they didn't override name for some reason
+                if hasattr(object, "name"):
+                    raise AttributeError(
+                        f"{object} redefined the 'name' method. Delete the 'name' method and try again."
+                    )
+
+                # ObjectSpace.each_object appears to yield objects in the reverse
+                # order that they were parsed by the interpreter so push each
+                # Suite object to the front of the array to order as encountered
+                SuiteRunner.suites.insert(0, object())
+
+            # If we inherit from Group
+            if isinstance(object, Group):
+                # Ensure they didn't override self.name for some reason
+                if hasattr(object, "name"):
+                    raise AttributeError(
+                        f"{object} redefined the 'self.name' method. Delete the 'self.name' method and try again."
+                    )
+                groups << object
 
         # Raise error if no suites or groups
         if len(SuiteRunner.suites) == 0 or len(groups) == 0:
             return "No Suite or no Group classes found"
 
         # Remove assigned Groups from the array of groups
         for suite in SuiteRunner.suites:
             if suite.__class__ == UnassignedSuite:
                 continue
             groups_to_delete = []
             for group in groups:
-                if group in suite.scripts():
+                if suite.scripts[group]:
                     groups_to_delete.append(group)
             for group in groups_to_delete:
-                groups.remove(group)
+                groups.delete(group)
 
         if len(groups) == 0:
             # If there are no unassigned group we simply remove the UnassignedSuite
             SuiteRunner.suites = [
                 suite
                 for suite in SuiteRunner.suites
                 if suite.__class__ != UnassignedSuite
             ]
         else:
             # unassigned groups should be added to the UnassignedSuite
-            unassigned_suite = UnassignedSuite()
+            unassigned_suite = [
+                suite
+                for suite in SuiteRunner.suites
+                if suite.__class__ == UnassignedSuite
+            ]
             for group in groups:
                 unassigned_suite.add_group(group)
 
         for suite in SuiteRunner.suites:
             cur_suite = {"setup": False, "teardown": False, "groups": {}}
-            if "setup" in dir(suite):
-                cur_suite["setup"] = True
-            if "teardown" in dir(suite):
-                cur_suite["teardown"] = True
+            if "setup" in suite.__class__:
+                cur_suite.setup = True
+            if "teardown" in suite.__class__:
+                cur_suite.teardown = True
 
             for type, group_class, script in suite.plans():
                 match type:
                     case "GROUP":
-                        if not cur_suite["groups"].get(group_class.__name__):
-                            cur_suite["groups"][group_class.__name__] = {
+                        if not cur_suite.groups.get(group_class.name):
+                            cur_suite.groups[group_class.name] = {
                                 "setup": False,
                                 "teardown": False,
                                 "scripts": [],
                             }
-                        cur_suite["groups"][group_class.__name__]["scripts"].extend(
-                            group_class.scripts()
-                        )
-                        # Make uniq!
-                        temp = set(cur_suite["groups"][group_class.__name__]["scripts"])
-                        cur_suite["groups"][group_class.__name__]["scripts"] = list(
-                            temp
+                        cur_suite.groups[group_class.name].scripts.append(
+                            group_class.scripts
                         )
-                        cur_suite["groups"][group_class.__name__]["scripts"].sort()
-                        if "setup" in dir(group_class):
-                            cur_suite["groups"][group_class.__name__]["setup"] = True
-                        if "teardown" in dir(group_class):
-                            cur_suite["groups"][group_class.__name__]["teardown"] = True
+                        # cur_suite.groups[group_class.name].scripts.uniq!
+                        if "setup" in group_class:
+                            cur_suite.groups[group_class.name].setup = True
+                        if "teardown" in group_class:
+                            cur_suite.groups[group_class.name].teardown = True
                     case "SCRIPT":
-                        if not cur_suite["groups"].get(group_class.__name__):
-                            cur_suite["groups"][group_class.__name__] = {
+                        if not cur_suite.groups.get(group_class.name):
+                            cur_suite.groups[group_class.name] = {
                                 "setup": False,
                                 "teardown": False,
                                 "scripts": [],
                             }
                         # Explicitly check for this method and raise an error if it does not exist
-                        if script in dir(group_class):
-                            cur_suite["groups"][group_class.__name__]["scripts"].append(
-                                script
-                            )
-                            # Make uniq!
-                            temp = set(
-                                cur_suite["groups"][group_class.__name__]["scripts"]
-                            )
-                            cur_suite["groups"][group_class.__name__]["scripts"] = list(
-                                temp
-                            )
-                            cur_suite["groups"][group_class.__name__]["scripts"].sort()
+                        if script in group_class:
+                            cur_suite.groups[group_class.name].scripts.append(script)
+                            # cur_suite.groups[group_class.name].scripts.uniq!
                         else:
                             raise Exception(
                                 f"{group_class} does not have a {script} method defined."
                             )
 
-                        if "setup" in dir(group_class):
-                            cur_suite["groups"][group_class.__name__]["setup"] = True
-                        if "teardown" in dir(group_class):
-                            cur_suite["groups"][group_class.__name__]["teardown"] = True
+                        if "setup" in group_class:
+                            cur_suite.groups[group_class.name].setup = True
+                        if "teardown" in group_class:
+                            cur_suite.groups[group_class.name].teardown = True
                     case "GROUP_SETUP":
-                        if not cur_suite["groups"].get(group_class.__name__):
-                            cur_suite["groups"][group_class.__name__] = {
+                        if not cur_suite.groups.get(group_class.name):
+                            cur_suite.groups[group_class.name] = {
                                 "setup": False,
                                 "teardown": False,
                                 "scripts": [],
                             }
                         # Explicitly check for the setup method and raise an error if it does not exist
-                        if "setup" in dir(group_class):
-                            cur_suite["groups"][group_class.__name__]["setup"] = True
+                        if "setup" in group_class:
+                            cur_suite.groups[group_class.name].setup = True
                         else:
                             raise Exception(
                                 f"{group_class} does not have a setup method defined."
                             )
 
                     case "GROUP_TEARDOWN":
-                        if not cur_suite["groups"].get(group_class.__name__):
-                            cur_suite["groups"][group_class.__name__] = {
+                        if not cur_suite.groups.get(group_class.name):
+                            cur_suite.groups[group_class.name] = {
                                 "setup": False,
                                 "teardown": False,
                                 "scripts": [],
                             }
                         # Explicitly check for the teardown method and raise an error if it does not exist
-                        if "teardown" in dir(group_class):
-                            cur_suite["groups"][group_class.__name__]["teardown"] = True
+                        if "teardown" in group_class:
+                            cur_suite.groups[group_class.name].teardown = True
                         else:
                             raise Exception(
                                 f"{group_class} does not have a teardown method defined."
                             )
 
             if not suite.name == "CustomSuite":
-                suites[suite.name()] = cur_suite
+                suites[suite.name] = cur_suite
 
         return suites
```

### Comparing `openc3-5.16.0/openc3/system/system.py` & `openc3-5.9.2b0/openc3/system/system.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,56 +12,50 @@
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import os
 import zipfile
-import traceback
 from threading import Lock
 from openc3.environment import OPENC3_SCOPE, OPENC3_CONFIG_BUCKET
 from openc3.top_level import add_to_search_path
 from openc3.utilities.bucket import Bucket
 from openc3.utilities.logger import Logger
-from openc3.utilities.store import Store
 from openc3.config.config_parser import ConfigParser
 from openc3.packets.packet_config import PacketConfig
 from openc3.packets.commands import Commands
 from openc3.packets.telemetry import Telemetry
 from openc3.packets.limits import Limits
 from .target import Target
 
 
 class System:
-    # Declare the System class variables ... they are set in __init__
-    targets = {}
-    packet_config = None
-    commands = None
-    telemetry = None
-    limits = None
+    # instance_attr_reader :targets
+    # instance_attr_reader :packet_config
+    # instance_attr_reader :commands
+    # instance_attr_reader :telemetry
+    # instance_attr_reader :limits
 
     # Variable that holds the singleton instance
     instance_obj = None
 
     # Mutex used to ensure that only one instance of System is created
     instance_mutex = Lock()
 
+    # The current limits set
+    limits_set = None
+
     # @return [Symbol] The current limits_set of the system returned from Redis
-    @classmethod
-    def limits_set(cls, scope=OPENC3_SCOPE):
-        # This line is basically the same code as limits_event_topic.py
-        # but we can't import it because it imports system.py and that
-        # creates a circular reference
-        sets = Store.hgetall(f"{scope}__limits_sets")
-        try:
-            return list(sets.keys())[list(sets.values()).index(b"true")].decode()
-        except ValueError:
-            return "DEFAULT"
+    def limits_set(cls):
+        # TODO: Implement LimitsEventTopic
+        # if not System.limits_set:
+        #   System.limits_set = LimitsEventTopic.current_set(scope=OPENC3_SCOPE)
+        return System.limits_set
 
-    @classmethod
     def setup_targets(cls, target_names, base_dir, scope=OPENC3_SCOPE):
         if not System.instance_obj:
             os.makedirs(f"{base_dir}/targets", exist_ok=True)
             bucket = Bucket.getClient()
             for target_name in target_names:
                 # Retrieve bucket/targets/target_name/target_id.zip
                 zip_path = f"{base_dir}/targets/{target_name}_current.zip"
@@ -69,58 +63,59 @@
                     f"{scope}/target_archives/{target_name}/{target_name}_current.zip"
                 )
                 Logger.info(f"Retrieving {bucket_key} from targets bucket")
                 bucket.get_object(
                     bucket=OPENC3_CONFIG_BUCKET, key=bucket_key, path=zip_path
                 )
                 with zipfile.ZipFile(zip_path) as zip_file:
-                    zip_file.extractall(f"{base_dir}/targets")
+                    for entry in zip_file.namelist():
+                        path = f"{base_dir}/targets/{entry}"
+                        os.makedirs(path, exist_ok=True)
+                        zip_file.extract(entry, path)
             # Build System from targets
-            System.instance(target_names, f"{base_dir}/targets")
+            System.instance(target_names, "#{base_dir}/targets")
 
     # Get the singleton instance of System
     #
     # @param target_names [Array of target_names]
     # @param target_config_dir Directory where target config folders are
     # @return [System] The System singleton
-    @classmethod
     def instance(cls, target_names=None, target_config_dir=None):
         if System.instance_obj:
             return System.instance_obj
         if not target_names and not target_config_dir:
             raise Exception("System.instance parameters are required on first call")
 
         with System.instance_mutex:
-            System.instance_obj = cls(target_names, target_config_dir)
+            System.instance_obj = cls.__init__(target_names, target_config_dir)
             return System.instance_obj
 
     # Create a new System object.
     #
     # @param target_names [Array of target names]
     # @param target_config_dir Directory where target config folders are
-    def __init__(self, target_names, target_config_dir):
+    def initialize(self, target_names, target_config_dir):
         add_to_search_path(target_config_dir, True)
-        System.targets = {}
-        System.packet_config = PacketConfig()
-        System.commands = Commands(System.packet_config, System)
-        System.telemetry = Telemetry(System.packet_config, System)
-        System.limits = Limits(System.packet_config, System)
+        self.targets = {}
+        self.packet_config = PacketConfig()
+        self.commands = Commands(self.packet_config)
+        self.telemetry = Telemetry(self.packet_config)
+        self.limits = Limits(self.packet_config)
         for target_name in target_names:
             self.add_target(target_name, target_config_dir)
 
     def add_target(self, target_name, target_config_dir):
         parser = ConfigParser()
         folder_name = f"{target_config_dir}/{target_name}"
         if not os.path.exists(folder_name):
             raise parser.error(f"Target folder must exist '{folder_name}'.")
 
         target = Target(target_name, target_config_dir)
-        System.targets[target.name] = target
+        self.targets[target.name] = target
         errors = []  # Store all errors processing the cmd_tlm files
         try:
             for cmd_tlm_file in target.cmd_tlm_files:
                 self.packet_config.process_file(cmd_tlm_file, target.name)
         except Exception as error:
-            trace = "".join(traceback.TracebackException.from_exception(error).format())
-            errors.append(f"Error processing {target_name}:\n{trace}")
+            errors.append(f"Error processing {cmd_tlm_file}:\n{error}")
         if len(errors) != 0:
             raise Exception("\n".join(errors))
```

### Comparing `openc3-5.16.0/openc3/system/target.py` & `openc3-5.9.2b0/openc3/system/target.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 OpenC3, Inc.
+# Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addums as found in the LICENSE.txt
 #
@@ -11,15 +11,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import os
-import glob
 from openc3.top_level import add_to_search_path
 from openc3.utilities.logger import Logger
 from openc3.config.config_parser import ConfigParser
 
 
 class Target:
     """Target encapsulates the information about a OpenC3 target. Targets are
@@ -27,15 +26,14 @@
     which define their access."""
 
     def __init__(self, target_name, path, gem_path=None):
         """Creates a new target by processing the target.txt file in the directory
         given by the path joined with the target_name. Records all the command
         and telemetry definition files found in the targets cmd_tlm directory.
         System uses this list and processes them using PacketConfig."""
-        self.language = "python"
         self.requires = []
         self.ignored_parameters = []
         self.ignored_items = []
         self.cmd_tlm_files = []
         self.interface = None
         self.routers = []
         self.cmd_cnt = 0
@@ -44,34 +42,30 @@
         self.tlm_unique_id_mode = False
         self.name = target_name.upper()
         self.get_target_dir(path, gem_path)
         self.process_target_config_file()
 
         # If target.txt didn't specify specific cmd/tlm files then add everything
         if len(self.cmd_tlm_files) == 0:
-            self.add_all_cmd_tlm()
+            self.cmd_tlm_files = self.add_all_cmd_tlm()
         else:
-            self.add_cmd_tlm_partials()
+            self.cmd_tlm_files = self.add_cmd_tlm_partials()
 
     # Parses the target configuration file
     #
     # self.param filename [String] The target configuration file to parse
     def process_file(self, filename):
-        Logger.info(f"Processing python target definition in file '{filename}'")
-        parser = ConfigParser("https://docs.openc3.com/docs/configuration/target")
+        Logger.info(f"Processing target definition in file '{filename}'")
+        parser = ConfigParser("https://openc3.com/docs/v5/target")
         for keyword, parameters in parser.parse_file(filename):
             match keyword:
-                case "LANGUAGE":
-                    usage = f"{keyword} <ruby | python>"
-                    parser.verify_num_parameters(1, 1, usage)
-                    self.language = parameters[0].lower()
                 case "REQUIRE":
                     usage = f"{keyword} <FILENAME>"
                     parser.verify_num_parameters(1, 1, usage)
-                    filename = f"{self.dir}/lib/{parameters[0]}"
+                    filename = f"{self.dir}/lib{parameters[0]}"
                     # TODO:
                     # try:
                     #     # Require absolute path to file in target lib folder. Prevents name
                     #     # conflicts at the require step
                     #     # OpenC3.require_file(filename, False)
 
                     # except LoadError:
@@ -93,23 +87,23 @@
                     #     test_filename = os.path.join(search_path, filename).gsub("\\", "/")
                     #     if os.path.exists(test_filename)
                     #         filename = test_filename
                     #         break
                     # self.requires << filename
 
                 case "IGNORE_PARAMETER" | "IGNORE_ITEM":
-                    usage = f"{keyword} <{keyword.split('_')[1]} NAME>"
+                    usage = "{keyword} <{keyword.split('_')[1]} NAME>"
                     parser.verify_num_parameters(1, 1, usage)
                     if "PARAMETER" in keyword:
-                        self.ignored_parameters.append(parameters[0].upper())
+                        self.ignored_parameters << parameters[0].upcase
                     if "ITEM" in keyword:
-                        self.ignored_items.append(parameters[0].upper())
+                        self.ignored_items << parameters[0].upcase
 
                 case "COMMANDS" | "TELEMETRY":
-                    usage = f"{keyword} <FILENAME>"
+                    usage = "{keyword} <FILENAME>"
                     parser.verify_num_parameters(1, 1, usage)
                     filename = f"{self.dir}/cmd_tlm/{parameters[0]}"
                     if not os.path.exists(filename):
                         raise parser.error(f"{filename} not found")
                     self.cmd_tlm_files.append(filename)
 
                 case "CMD_UNIQUE_ID_MODE":
@@ -129,15 +123,21 @@
 
     def as_json(self):
         config = {}
         config["name"] = self.name
         config["requires"] = self.requires
         config["ignored_parameters"] = self.ignored_parameters
         config["ignored_items"] = self.ignored_items
+        # config['auto_screen_substitute'] = True if self.auto_screen_substitute
         config["cmd_tlm_files"] = self.cmd_tlm_files
+        # config['filename'] = self.filename
+        # config['interface'] = self.interface.name if self.interface
+        # config['dir'] = self.dir
+        # config['cmd_cnt'] = self.cmd_cnt
+        # config['tlm_cnt'] = self.tlm_cnt
         if self.cmd_unique_id_mode:
             config["cmd_unique_id_mode"] = True
         if self.tlm_unique_id_mode:
             config["tlm_unique_id_mode"] = True
         config["id"] = self.id
         return config
 
@@ -145,14 +145,15 @@
     # search path if it exists
     def get_target_dir(self, path, gem_path):
         if gem_path:
             self.dir = gem_path
         else:
             self.dir = os.path.join(path, self.name)
 
+        #   self.dir.gsub!("\\", '/')
         lib_dir = os.path.join(self.dir, "lib")
         if os.path.exists(lib_dir):
             add_to_search_path(lib_dir, False)
         proc_dir = os.path.join(self.dir, "procedures")
         if os.path.exists(proc_dir):
             add_to_search_path(proc_dir, False)
 
@@ -167,38 +168,28 @@
         id_filename = os.path.join(self.dir, "target_id.txt")
         if os.path.exists(id_filename):
             with open(id_filename) as f:
                 self.id = f.read().strip()
         else:
             self.id = None
 
-    # Automatically add all command and telemetry definitions to the list
-    def add_all_cmd_tlm(self):
-        cmd_tlm_files = []
-        if os.path.exists(os.path.join(self.dir, "cmd_tlm")):
-            # Grab All *.txt files in the cmd_tlm folder and subfolders
-            for filename in glob.glob(
-                os.path.join(self.dir, "cmd_tlm", "**", "*.txt"), recursive=True
-            ):
-                if os.path.isfile(filename):
-                    cmd_tlm_files.append(filename)
-            # Grab All *.xtce files in the cmd_tlm folder and subfolders
-            for filename in glob.glob(
-                os.path.join(self.dir, "cmd_tlm", "**", "*.xtce"), recursive=True
-            ):
-                if os.isfile(filename):
-                    cmd_tlm_files.append(filename)
-        cmd_tlm_files.sort()
-        self.cmd_tlm_files = cmd_tlm_files
-
-    # Make sure all partials are included in the cmd_tlm list for the hashing sum calculation
-    def add_cmd_tlm_partials(self):
-        partial_files = []
-        if os.path.isfile(os.path.join(self.dir, "cmd_tlm")):
-            # Grab all _*.txt files in the cmd_tlm folder and subfolders
-            os.path.join(self.dir, "cmd_tlm", "**", "_*.txt")
-            for filename in glob.glob(
-                os.path.join(self.dir, "cmd_tlm", "**", "_*.txt"), recursive=True
-            ):
-                partial_files.append(filename)
-        partial_files.sort()
-        self.cmd_tlm_files = list(dict.fromkeys(self.cmd_tlm_files + partial_files))
+    # # Automatically add all command and telemetry definitions to the list
+    # def add_all_cmd_tlm(self):
+    #   cmd_tlm_files = []
+    #   if os.path.exists(os.path.join(self.dir, 'cmd_tlm')):
+    #     # Grab All *.txt files in the cmd_tlm folder and subfolders
+    #     Dir[os.path.join(self.dir, 'cmd_tlm', '**', '*.txt')].each do |filename|
+    #       cmd_tlm_files << filename
+
+    #     # Grab All *.xtce files in the cmd_tlm folder and subfolders
+    #     Dir[os.path.join(self.dir, 'cmd_tlm', '**', '*.xtce')].each do |filename|
+    #       cmd_tlm_files << filename
+    #   return cmd_tlm_files.sort()
+
+    # # Make sure all partials are included in the cmd_tlm list for the hashing sum calculation
+    # def add_cmd_tlm_partials(self):
+    #   partial_files = []
+    #   if os.path.exists(os.path.join(self.dir, 'cmd_tlm')):
+    #     # Grab all _*.txt files in the cmd_tlm folder and subfolders
+    #     Dir[os.path.join(self.dir, 'cmd_tlm', '**', '_*.txt')].each do |filename|
+    #       partial_files << filename
+    #   return list(set(self.cmd_tlm_files.concat(partial_files.sort())))
```

### Comparing `openc3-5.16.0/openc3/topics/command_decom_topic.py` & `openc3-5.9.2b0/openc3/topics/command_decom_topic.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,46 +12,43 @@
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import json
 from openc3.topics.topic import Topic
-from openc3.utilities.store_queued import EphemeralStoreQueued
 from openc3.environment import OPENC3_SCOPE
-from openc3.utilities.json import JsonEncoder
-from openc3.utilities.time import to_nsec_from_epoch
 
 
 class CommandDecomTopic(Topic):
     @classmethod
     def topics(cls, scope):
-        Topic.topics("DECOMCMD", scope)
+        Topic.topics(scope, "DECOMCMD")
 
     @classmethod
     def write_packet(cls, packet, scope):
         topic = f"{scope}__DECOMCMD__{{{packet.target_name}}}__{packet.packet_name}"
         msg_hash = {
-            "time": to_nsec_from_epoch(packet.packet_time),
+            "time": packet.packet_time.to_nsec_from_epoch,
             "target_name": packet.target_name,
             "packet_name": packet.packet_name,
             "stored": str(packet.stored),
             "received_count": packet.received_count,
         }
         json_hash = {}
         for item in packet.sorted_items:
             json_hash[item.name] = packet.read_item(item, "RAW")
             if item.write_conversion or item.states:
                 json_hash[item.name + "__C"] = packet.read_item(item, "CONVERTED")
             if item.format_string:
                 json_hash[item.name + "__F"] = packet.read_item(item, "FORMATTED")
             if item.units:
                 json_hash[item.name + "__U"] = packet.read_item(item, "WITH_UNITS")
-        msg_hash["json_data"] = json.dumps(json_hash, cls=JsonEncoder)
-        EphemeralStoreQueued.write_topic(topic, msg_hash)
+        msg_hash["json_data"] = json.dumps(json_hash)
+        Topic.write_topic(topic, msg_hash)
 
     @classmethod
     def get_cmd_item(
         cls, target_name, packet_name, param_name, type="WITH_UNITS", scope=OPENC3_SCOPE
     ):
         msg_id, msg_hash = Topic.get_newest_message(
             f"{scope}__DECOMCMD__{{{target_name}}}__{packet_name}"
@@ -61,26 +58,27 @@
             # Do we still calculate from msg_hash['time'] or use the times directly?
             #
             # if param_name == 'RECEIVED_TIMESECONDS' || param_name == 'PACKET_TIMESECONDS'
             #   Time.from_nsec_from_epoch(msg_hash['time'].to_i).to_f
             # elsif param_name == 'RECEIVED_TIMEFORMATTED' || param_name == 'PACKET_TIMEFORMATTED'
             #   Time.from_nsec_from_epoch(msg_hash['time'].to_i).formatted
             if param_name == "RECEIVED_COUNT":
-                return int(msg_hash[b"received_count"])
+                return int(msg_hash["received_count"])
             else:
-                hash = json.loads(msg_hash[b"json_data"])
+                json = msg_hash["json_data"]
+                hash = json.loads(json)
                 # Start from the most complex down to the basic raw value
-                value = hash.get(f"{param_name}__U")
-                if value is not None and type == "WITH_UNITS":
+                value = hash[f"{param_name}__U"]
+                if value and type == "WITH_UNITS":
                     return value
 
-                value = hash.get(f"{param_name}__F")
-                if value is not None and (type == "WITH_UNITS" or type == "FORMATTED"):
+                value = hash[f"{param_name}__F"]
+                if value and (type == "WITH_UNITS" or type == "FORMATTED"):
                     return value
 
-                value = hash.get(f"{param_name}__C")
-                if value is not None and (
+                value = hash[f"{param_name}__C"]
+                if value and (
                     type == "WITH_UNITS" or type == "FORMATTED" or type == "CONVERTED"
                 ):
                     return value
 
                 return hash[param_name]
```

### Comparing `openc3-5.16.0/openc3/topics/command_topic.py` & `openc3-5.9.2b0/openc3/topics/command_topic.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,78 +13,76 @@
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import time
 import json
 from openc3.topics.topic import Topic
-from openc3.utilities.store_queued import EphemeralStoreQueued
 from openc3.top_level import HazardousError
-from openc3.utilities.time import to_nsec_from_epoch
-from openc3.utilities.json import JsonEncoder
 
 
 class CommandTopic(Topic):
-    COMMAND_ACK_TIMEOUT_S = 5
+    COMMAND_ACK_TIMEOUT_S = 0.1  # TODO 5
 
     @classmethod
     def write_packet(cls, packet, scope):
-        topic = f"{scope}__COMMAND__{{{packet.target_name}}}__{packet.packet_name}"
+        topic = f"{scope}__COMMAND__{{packet.target_name}}__{packet.packet_name}"
         msg_hash = {
-            "time": to_nsec_from_epoch(packet.packet_time),
-            "received_time": to_nsec_from_epoch(packet.received_time),
+            "time": packet.packet_time.to_nsec_from_epoch,
+            "received_time": packet.received_time.to_nsec_from_epoch,
             "target_name": packet.target_name,
             "packet_name": packet.packet_name,
             "received_count": packet.received_count,
             "stored": str(packet.stored),
-            "buffer": bytes(packet.buffer_no_copy()),
+            "buffer": packet.buffer(False),
         }
-        EphemeralStoreQueued.write_topic(topic, msg_hash)
+        Topic.write_topic(topic, msg_hash)
 
     @classmethod
     def send_command(cls, command, timeout, scope):
+        print(f"send_command:{command}")
         if timeout is None:
             timeout = cls.COMMAND_ACK_TIMEOUT_S
         ack_topic = f"{{{scope}__ACKCMD}}TARGET__{command['target_name']}"
         Topic.update_topic_offsets([ack_topic])
         # Save the existing cmd_params Hash and JSON generate before writing to the topic
         cmd_params = command["cmd_params"]
-        command["cmd_params"] = json.dumps(command["cmd_params"], cls=JsonEncoder)
+        command["cmd_params"] = json.dumps(command["cmd_params"])
         cmd_id = Topic.write_topic(
             f"{{{scope}__CMD}}TARGET__{command['target_name']}",
             command,
             "*",
             100,
         )
         start_time = time.time()
         while (time.time() - start_time) < timeout:
             for _, _, msg_hash, _ in Topic.read_topics([ack_topic]):
-                if msg_hash[b"id"] == cmd_id:
-                    result = msg_hash[b"result"].decode()
-                    if result == "SUCCESS":
-                        return command["target_name"], command["cmd_name"], cmd_params
+                if msg_hash["id"] == cmd_id:
+                    if msg_hash["result"] == "SUCCESS":
+                        return [command["target_name"], command["cmd_name"], cmd_params]
                     # Check for HazardousError which is a special case
-                    elif "HazardousError" in result:
+                    elif "HazardousError" in msg_hash["result"]:
                         cls.raise_hazardous_error(
                             msg_hash,
                             command["target_name"],
                             command["cmd_name"],
                             cmd_params,
                         )
                     else:
-                        raise RuntimeError(result)
+                        raise msg_hash["result"]
         raise RuntimeError(f"Timeout of {timeout}s waiting for cmd ack")
 
     ###########################################################################
     # PRIVATE implementation details
     ###########################################################################
 
     @classmethod
-    def raise_hazardous_error(cls, msg_hash, target_name, cmd_name, cmd_params):
-        _, description, formatted = msg_hash[b"result"].decode().split("\n")
+    def raise_hazardous_error(msg_hash, target_name, cmd_name, cmd_params):
+        print(f"raise_hazardous_error hash:{msg_hash}")
+        _, description, formatted = msg_hash["result"].split("\n")
         # Create and populate a new HazardousError and raise it up
         # The _cmd method in script/commands.rb rescues this and calls prompt_for_hazardous
         error = HazardousError()
         error.target_name = target_name
         error.cmd_name = cmd_name
         error.cmd_params = cmd_params
         error.hazardous_description = description
```

### Comparing `openc3-5.16.0/openc3/topics/decom_interface_topic.py` & `openc3-5.9.2b0/openc3/topics/decom_interface_topic.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import json
 import time
 from openc3.topics.topic import Topic
 from openc3.environment import OPENC3_SCOPE
-from openc3.utilities.json import JsonEncoder, JsonDecoder
 
 
 class DecomInterfaceTopic(Topic):
     @classmethod
     def build_cmd(
         cls, target_name, cmd_name, cmd_params, range_check, raw, scope=OPENC3_SCOPE
     ):
@@ -32,35 +31,29 @@
         data["cmd_params"] = cmd_params
         data["range_check"] = range_check
         data["raw"] = raw
         # DecomMicroservice is listening to the DECOMINTERFACE topic and is responsible
         # for actually building the command. This was deliberate to allow this to work
         # with or without an interface.
         decom_id = Topic.write_topic(
-            f"{scope}__DECOMINTERFACE__{{{target_name}}}",
-            {"build_cmd": json.dumps(data, cls=JsonEncoder)},
+            f"#{scope}__DECOMINTERFACE__{{{target_name}}}",
+            {"build_cmd": json.dumps(data)},
             "*",
             100,
         )
         timeout = 5  # Arbitrary 5s timeout
         ack_topic = f"{{{scope}__ACKCMD}}TARGET__{target_name}"
         start_time = time.time()
         while (time.time() - start_time) < timeout:
-            for topic, msg_id, msg_hash, redis in Topic.read_topics([ack_topic]):
-                if msg_hash[b"id"] == decom_id:
-                    if msg_hash[b"result"] == b"SUCCESS":
-                        msg_hash = {
-                            k.decode(): v.decode() for (k, v) in msg_hash.items()
-                        }
-                        msg_hash["buffer"] = json.loads(
-                            msg_hash["buffer"], cls=JsonDecoder
-                        )
+            for _, _, msg_hash, _ in Topic.read_topics([ack_topic]):
+                if msg_hash["id"] == decom_id:
+                    if msg_hash["result"] == "SUCCESS":
                         return msg_hash
                     else:
-                        raise RuntimeError(msg_hash[b"message"])
+                        raise msg_hash["message"]
         raise RuntimeError(
             f"Timeout of {timeout}s waiting for cmd ack. Does target '{target_name}' exist?"
         )
 
     @classmethod
     def inject_tlm(
         cls,
```

### Comparing `openc3-5.16.0/openc3/topics/telemetry_topic.py` & `openc3-5.9.2b0/openc3/utilities/target_file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
-# attribution addums as found in the LICENSE.txt
+# attribution addendums as found in the LICENSE.txt
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-import json
-from openc3.topics.topic import Topic
-from openc3.utilities.store_queued import EphemeralStoreQueued
-from openc3.utilities.time import to_nsec_from_epoch
+from openc3.environment import OPENC3_LOCAL_MODE, OPENC3_CONFIG_BUCKET
+from openc3.utilities.local_mode import LocalMode
+from openc3.utilities.bucket import Bucket
 
 
-class TelemetryTopic(Topic):
+class TargetFile:
     @classmethod
-    def write_packet(cls, packet, scope, queued=False):
-        msg_hash = {
-            "time": to_nsec_from_epoch(packet.packet_time),
-            "received_time": to_nsec_from_epoch(packet.received_time),
-            "stored": str(packet.stored),
-            "target_name": packet.target_name,
-            "packet_name": packet.packet_name,
-            "received_count": packet.received_count,
-            "buffer": bytes(packet.buffer_no_copy()),
-        }
-        if packet.extra:
-            msg_hash["extra"] = json.dumps(packet.extra.as_json())
-        if queued:
-            EphemeralStoreQueued.write_topic(
-                f"{scope}__TELEMETRY__{{{packet.target_name}}}__{packet.packet_name}",
-                msg_hash,
+    def body(cls, scope, name):
+        name = name.split("*")[0]  # Split '*' that indicates modified
+        # First try opening a potentially modified version by looking for the modified target
+        if OPENC3_LOCAL_MODE:
+            local_file = LocalMode.open_local_file(name, scope=scope)
+            if local_file:
+                return local_file.read()
+
+        bucket = Bucket.getClient()
+        resp = bucket.get_object(
+            bucket=OPENC3_CONFIG_BUCKET, key=f"{scope}/targets_modified/{name}"
+        )
+        print(resp)
+        if not resp:
+            # Now try the original
+            resp = bucket.get_object(
+                bucket=OPENC3_CONFIG_BUCKET, key=f"{scope}/targets/{name}"
             )
+        if resp and resp["Body"]:
+            return resp["Body"].read()
         else:
-            Topic.write_topic(
-                f"{scope}__TELEMETRY__{{{packet.target_name}}}__{packet.packet_name}",
-                msg_hash,
-            )
+            return None
```

### Comparing `openc3-5.16.0/openc3/topics/topic.py` & `openc3-5.9.2b0/openc3/topics/topic.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 class Topic(metaclass=TopicMeta):
     @classmethod
     def clear_topics(cls, topics, maxlen=0):
         for topic in topics:
             EphemeralStore.xtrim(topic, maxlen)
 
     @classmethod
-    def topics(cls, key, scope):
+    def topics(cls, scope, key):
         return sorted(
             set(
                 list(
-                    EphemeralStore.scan_iter(
+                    EphemeralStore.scan_each(
                         match=f"{scope}__{key}__*", type="stream", count=100
                     )
                 )
             )
         )
 
     @classmethod
     def get_cnt(cls, topic):
         _, packet = EphemeralStore.get_newest_message(topic)
         if packet:
-            return int(packet[b"received_count"])
+            return int(packet["received_count"])
         else:
             return 0
```

### Comparing `openc3-5.16.0/openc3/utilities/authentication.py` & `openc3-5.9.2b0/openc3/utilities/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -29,18 +31,18 @@
 class OpenC3AuthenticationRetryableError(OpenC3AuthenticationError):
     pass
 
 
 # OpenC3 base / open source authentication code
 class OpenC3Authentication:
     def __init__(self):
-        self._token = OPENC3_API_PASSWORD
+        self._token = OPENC3_API_PASSWORD or OPENC3_SERVICE_PASSWORD
         if not self._token:
             raise OpenC3AuthenticationError(
-                "Authentication requires environment variable OPENC3_API_PASSWORD"
+                "Authentication requires environment variables OPENC3_API_PASSWORD or OPENC3_SERVICE_PASSWORD"
             )
 
     def token(self):
         return self._token
 
 
 # OpenC3 enterprise Keycloak authentication code
@@ -71,15 +73,15 @@
         self.http = Session()
 
     # Load the token from the environment
     def token(self):
         with self.auth_mutex:
             self.log = [None, None]
             current_time = time.time()
-            if self._token is None:
+            if self._token == None:
                 self._make_token(current_time)
             elif self.refresh_expires_at < current_time:
                 self._make_token(current_time)
             elif self.expires_at < current_time:
                 self._refresh_token(current_time)
         return f"Bearer {self._token}"
 
@@ -99,15 +101,15 @@
             # Username and password
             data = f"username={OPENC3_API_USER}&password={OPENC3_API_PASSWORD}&client_id={client_id}&grant_type=password&scope=openid"
             headers = {
                 "Content-Type": "application/x-www-form-urlencoded",
                 "User-Agent": OPENC3_USER_AGENT,
             }
             oath = self._make_request(headers, data)
-            self._token = oath["access_token"]
+            self_token = oath["access_token"]
             self.refresh_token = oath["refresh_token"]
             self.expires_at = (
                 current_time + oath["expires_in"] - self.REFRESH_OFFSET_SECONDS
             )
             self.refresh_expires_at = (
                 current_time + oath["refresh_expires_in"] - self.REFRESH_OFFSET_SECONDS
             )
@@ -144,17 +146,17 @@
             "url": url,
             "data": data,
             "headers": headers,
         }
         self.log[0] = f"Request: {request_kwargs}"
         # print(self.log[0])
         resp = self.http.post(**request_kwargs)
-        self.log[1] = (
-            f"response status: {resp.status_code} header: {resp.headers} body: {resp.text}"
-        )
+        self.log[
+            1
+        ] = f"response status: #{resp.status_code} header: #{resp.headers} body: #{resp.text}"
         # print(self.log[1])
         if resp.status_code >= 200 and resp.status_code <= 299:
             return json.loads(resp.text)
         elif resp.status_code >= 500 and resp.status_code <= 599:
             raise OpenC3AuthenticationRetryableError(
                 f"authentication request retryable {self.log[0]} ::: {self.log[1]}"
             )
```

### Comparing `openc3-5.16.0/openc3/utilities/authorization.py` & `openc3-5.9.2b0/openc3/utilities/authorization.py`

 * *Files identical despite different names*

### Comparing `openc3-5.16.0/openc3/utilities/aws_bucket.py` & `openc3-5.9.2b0/openc3/utilities/aws_bucket.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import boto3
 from botocore.config import Config
 from botocore.exceptions import ClientError, WaiterError
 from openc3.utilities.bucket import Bucket
 from openc3.environment import *
 import time
 
-aws_arn = OPENC3_AWS_ARN_PREFIX
 s3_config = Config(s3={"addressing_style": "path"})
 if OPENC3_BUCKET_URL:
     s3_endpoint_url = OPENC3_BUCKET_URL
 elif OPENC3_DEVEL:
     s3_endpoint_url = "http://127.0.0.1:9000"
 else:
     s3_endpoint_url = "http://openc3-minio:9000"
@@ -41,16 +40,14 @@
     s3_session = boto3.session.Session(region_name=AWS_REGION)
 
 
 class AwsBucket(Bucket):
     CREATE_CHECK_COUNT = 100  # 10 seconds
 
     def __init__(self):
-        # Check whether the session is a real Session or a MockS3
-        # print(f"\nAwsBucket INIT session:{s3_session}\n")
         self.client = s3_session.client(
             "s3", endpoint_url=s3_endpoint_url, config=s3_config
         )
 
     def create(self, bucket):
         if not self.exist(bucket):
             self.client.create_bucket(Bucket=bucket)
@@ -59,62 +56,59 @@
                 time.sleep(0.1)
                 count += 1
                 if self.exist(bucket) or count > self.CREATE_CHECK_COUNT:
                     break
         return bucket
 
     def ensure_public(self, bucket):
-        if OPENC3_NO_BUCKET_POLICY is None:
-            policy = """{
+        policy = """{
   "Version": "2012-10-17",
   "Statement": [
     {
       "Action": [
         "s3:GetBucketLocation",
         "s3:ListBucket"
       ],
       "Effect": "Allow",
       "Principal": {
         "AWS": [
           "*"
         ]
       },
       "Resource": ["""
-            policy = policy + f'\n        "{aws_arn}:s3:::{bucket}"'
-            policy = (
-                policy
-                + """
+        policy = policy + f'\n        "arn:aws:s3:::{bucket}"'
+        policy = (
+            policy
+            + """
       ],
       "Sid": ""
     },
     {
       "Action": [
         "s3:GetObject"
       ],
       "Effect": "Allow",
       "Principal": {
         "AWS": [
           "*"
         ]
       },
       "Resource": ["""
-            )
-            policy = policy + f'\n        "{aws_arn}:s3:::{bucket}/*"'
-            policy = (
-                policy
-                + """
+        )
+        policy = policy + f'\n        "arn:aws:s3:::{bucket}/*"'
+        policy = (
+            policy
+            + """
       ],
       "Sid": ""
     }
   ]
 }"""
-            )
-            self.client.put_bucket_policy(
-                Bucket=bucket, Policy=policy, ChecksumAlgorithm="SHA256"
-            )
+        )
+        self.client.put_bucket_policy(Bucket=bucket, Policy=policy)
 
     def exist(self, bucket):
         try:
             self.client.head_bucket(Bucket=bucket)
             return True
         except ClientError:
             return False
@@ -140,16 +134,15 @@
         try:
             result = []
             kw_args = {"Bucket": bucket, "MaxKeys": max_request}
             if prefix:
                 kw_args["Prefix"] = prefix
             while True:
                 resp = self.client.list_objects_v2(**kw_args)
-                if "Contents" in resp:
-                    result = result + resp["Contents"]
+                result = result + resp["Contents"]
                 if len(result) >= max_total:
                     break
                 if not resp["IsTruncated"]:
                     break
                 kw_args["ContinuationToken"] = resp["NextContinuationToken"]
             # Array  of objects with key and size methods
             return result
@@ -176,30 +169,30 @@
 
             while True:
                 resp = self.client.list_objects_v2(**kw_args)
                 if "CommonPrefixes" in resp:
                     for item in resp["CommonPrefixes"]:
                         # If path was DEFAULT/targets_modified/ then the
                         # results look like DEFAULT/targets_modified/INST/
-                        dirs.append(item["Prefix"].split("/")[-2])
+                        dirs.append(item["Prefix"].split("/")[-1])
                 if only_directories:
                     result = dirs
                 else:
                     if "Contents" in resp:
                         for aws_item in resp["Contents"]:
                             item = {}
                             item["name"] = aws_item["Key"].split("/")[-1]
                             item["modified"] = aws_item["LastModified"]
                             item["size"] = aws_item["Size"]
                             if metadata:
                                 item["metadata"] = self.head_object(
                                     bucket=bucket, key=aws_item["Key"]
                                 )
                             files.append(item)
-                    result = (dirs, files)
+                    result = [dirs, files]
                 if not resp["IsTruncated"]:
                     break
                 kw_args["ContinuationToken"] = resp["NextContinuationToken"]
             return result
         except ClientError:
             raise Bucket.NotFound(f"Bucket '{bucket}' does not exist.")
 
@@ -210,47 +203,33 @@
         except ClientError:
             raise Bucket.NotFound(f"Object '{bucket}/{key}' does not exist.")
 
     # put_object fires off the request to store but does not confirm
     def put_object(
         self, bucket, key, body, content_type=None, cache_control=None, metadata=None
     ):
-        kw_args = {
-            "Bucket": bucket,
-            "Key": key,
-            "Body": body,
-            "ChecksumAlgorithm": "SHA256",
-        }
+        kw_args = {"Bucket": bucket, "Key": key, "Body": body}
         if content_type:
             kw_args["ContentType"] = content_type
         if cache_control:
             kw_args["CacheControl"] = cache_control
         if metadata:
             kw_args["Metadata"] = metadata
         return self.client.put_object(**kw_args)
 
     # @returns [Boolean] Whether the file exists
-    def check_object(self, bucket, key, retries=True):
-        if retries:
-            try:
-                s3_object_exists_waiter = self.client.get_waiter("object_exists")
-                s3_object_exists_waiter.wait(
-                    Bucket=bucket,
-                    Key=key,
-                    WaiterConfig={"Delay": 0.1, "MaxAttempts": 30},
-                )
-                return True
-            except WaiterError:
-                return False
-        else:
-            try:
-                self.head_object(bucket, key)
-                return True
-            except Bucket.NotFound:
-                return False
+    def check_object(self, bucket, key):
+        try:
+            s3_object_exists_waiter = self.client.get_waiter("object_exists")
+            s3_object_exists_waiter.wait(
+                Bucket=bucket, Key=key, WaiterConfig={"Delay": 0.1, "MaxAttempts": 30}
+            )
+            return True
+        except WaiterError:
+            return False
 
     def delete_object(self, bucket, key):
         self.client.delete_object(Bucket=bucket, Key=key)
 
     def delete_objects(self, bucket, keys):
         def method(key):
             return {"Key": key}
```

### Comparing `openc3-5.16.0/openc3/utilities/bucket.py` & `openc3-5.9.2b0/openc3/utilities/bucket.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,24 +27,17 @@
 
     @classmethod
     def getClient(cls):
         if not OPENC3_CLOUD:
             raise RuntimeError("OPENC3_CLOUD environment variable is required")
         # Base is AwsBucket which works with MINIO, Enterprise implements additional
         bucket_class = OPENC3_CLOUD.capitalize() + "Bucket"
-        my_module = None
-        try:
-            my_module = importlib.import_module(
-                "." + OPENC3_CLOUD.lower() + "_bucket", "openc3.utilities"
-            )
-        # If the file doesn't exist try the Enterprise module
-        except ModuleNotFoundError:
-            my_module = importlib.import_module(
-                "." + OPENC3_CLOUD.lower() + "_bucket", "openc3-enterprise.utilities"
-            )
+        my_module = importlib.import_module(
+            "." + OPENC3_CLOUD.lower() + "_bucket", "openc3.utilities"
+        )
         return getattr(my_module, bucket_class)()
 
     def create(self, bucket):
         raise NotImplementedError(
             f"{self.__class__.__name__} has not implemented method '{inspect.currentframe().f_code.co_name}'"
         )
 
@@ -81,15 +74,15 @@
     def put_object(
         self, bucket, key, body, content_type=None, cache_control=None, metadata=None
     ):
         raise NotImplementedError(
             f"{self.__class__.__name__} has not implemented method '{inspect.currentframe().f_code.co_name}'"
         )
 
-    def check_object(self, bucket, key, retries=True):
+    def check_object(self, bucket, key):
         raise NotImplementedError(
             f"{self.__class__.__name__} has not implemented method '{inspect.currentframe().f_code.co_name}'"
         )
 
     def delete_object(self, bucket, key):
         raise NotImplementedError(
             f"{self.__class__.__name__} has not implemented method '{inspect.currentframe().f_code.co_name}'"
```

### Comparing `openc3-5.16.0/openc3/utilities/bucket_utilities.py` & `openc3-5.9.2b0/openc3/utilities/bucket_utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,53 +11,51 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 from openc3.utilities.bucket import Bucket
-
-# from openc3.utilities.target_file import TargetFile
+from openc3.utilities.target_file import TargetFile
 from openc3.utilities.logger import Logger
 from openc3.models.reducer_model import ReducerModel
-from openc3.environment import OPENC3_LOGS_BUCKET
+from openc3.environment import OPENC3_SCOPE, OPENC3_LOGS_BUCKET
 import zlib
 import os
 import time
 import threading
 
 
 class BucketUtilities:
     FILE_TIMESTAMP_FORMAT = "%Y%m%d%H%M%S%N"
     DIRECTORY_TIMESTAMP_FORMAT = "%Y%m%d"
 
-    # TODO: This is never called
-    # @classmethod
-    # def bucket_load(cls, *args, scope=OPENC3_SCOPE):
-    #     if not scope:
-    #         scope = OPENC3_SCOPE
-    #     path = args[0]
-
-    #     # Only support TARGET files
-    #     if path[0] == "/" or str(path.split("/")[0]).upper() != path.split("/")[0]:
-    #         raise ImportError(f"only relative TARGET files are allowed -- {path}")
-    #     extension = os.path.splitext(path)[1]
-    #     if not extension or extension == "":
-    #         path = path + ".py"
-
-    #     # Retrieve the text of the script from S3
-    #     text = TargetFile.body(scope, path)
-    #     if not text:
-    #         raise ImportError(f"Bucket file {path} not found for scope {scope}")
+    @classmethod
+    def bucket_load(cls, *args, scope=OPENC3_SCOPE):
+        if not scope:
+            scope = OPENC3_SCOPE
+        path = args[0]
+
+        # Only support TARGET files
+        if path[0] == "/" or str(path.split("/")[0]).upper() != path.split("/")[0]:
+            raise ImportError(f"only relative TARGET files are allowed -- {path}")
+        extension = os.path.splitext(path)[1]
+        if not extension or extension == "":
+            path = path + ".py"
+
+        # Retrieve the text of the script from S3
+        text = TargetFile.body(scope, path)
+        if not text:
+            raise ImportError(f"Bucket file {path} not found for scope {scope}")
 
-    #     # Execute the script directly without instrumentation because we are doing require/load
-    #     exec(text.decode())
+        # Execute the script directly without instrumentation because we are doing require/load
+        exec(text)
 
-    #     # Successful load/require returns true
-    #     return True
+        # Successful load/require returns true
+        return True
 
     @classmethod
     def move_log_file_to_bucket_thread(cls, filename, bucket_key, metadata={}):
         try:
             client = Bucket.getClient()
 
             orig_filename = None
@@ -98,17 +96,15 @@
             os.remove(filename)
         except Exception as err:
             Logger.error(f"Error saving log file to bucket: {filename}\n{str(err)}")
 
     @classmethod
     def move_log_file_to_bucket(cls, filename, bucket_key, metadata={}):
         thread = threading.Thread(
-            target=cls.move_log_file_to_bucket_thread,
-            args=[filename, bucket_key, metadata],
-            daemon=True,
+            target=cls.move_log_file_to_bucket, args=[filename, bucket_key, metadata]
         )
         thread.start()
         return thread
 
     @classmethod
     def compress_file(cls, filename, chunk_size=50_000_000):
         zipped = f"{filename}.gz"
```

### Comparing `openc3-5.16.0/openc3/utilities/connection_pool.py` & `openc3-5.9.2b0/openc3/utilities/connection_pool.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,32 +14,28 @@
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 from contextlib import contextmanager
 from queue import SimpleQueue
 from threading import Lock
 
-
 class ConnectionPool:
     def __init__(self, ctor, pool_size):
         self.ctor = ctor
         self.count = 0
         self.pool_size = pool_size
         self.pool = SimpleQueue()
         self.lock = Lock()
-        self.pipelines = {}
 
     @contextmanager
     def get(self):
         item = None
         with self.lock:
             if not self.pool.empty():
                 item = self.pool.get(False)
             elif self.count < self.pool_size:
                 item = self.ctor()
                 self.count += 1
             else:
                 item = self.pool.get()
-        try:
-            yield item
-        finally:
-            self.pool.put(item)
+        yield item
+        self.pool.put(item)
```

### Comparing `openc3-5.16.0/openc3/utilities/extract.py` & `openc3-5.9.2b0/openc3/utilities/extract.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+#!/usr/bin/env python3
+# vim: tabstop=8 expandtab shiftwidth=4 softtabstop=4
+# -*- coding: latin-1 -*-
+"""
+extract.py
+"""
+
 # Copyright 2022 Ball Aerospace & Technologies Corp.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Lesser General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 
 # Modified by OpenC3, Inc.
-# All changes Copyright 2023, OpenC3, Inc.
+# All changes Copyright 2022, OpenC3, Inc.
 # All Rights Reserved
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import re
 
@@ -99,16 +106,16 @@
             # Floating Point in normal or scientific notation
             return_value = float(string)
         elif is_int(string):
             # Integer
             return_value = int(string)
         elif is_hex(string):
             # Hex
-            return_value = int(string, 0)
-        elif is_array(string):
+            return_value = int(string)
+        elif isinstance(string, list):
             # Array
             return_value = eval(string)
     except Exception:
         # Something went wrong so just return the string as is
         pass
     return return_value
 
@@ -117,18 +124,14 @@
     """Converts the String representing a hexadecimal number (i.e. "0xABCD")
     to a binary String with the same data (i.e "\xAB\xCD")
     @return [String] Binary byte string"""
 
     # Remove leading 0x or 0X
     if string[:2] == "0x" or string[:2] == "0X":
         string = string[2:]
-    # fromhex only works with an even number of characters to prepend
-    # a zero in case we get something like '0xA' or '0xABC'
-    if len(string) % 2 == 1:
-        string = f"0{string}"
 
     return bytearray.fromhex(string)
 
 
 def add_cmd_parameter(keyword, value, cmd_params):
     quotes_removed = remove_quotes(value)
     if value == quotes_removed:
@@ -190,50 +193,51 @@
             if value:
                 add_cmd_parameter(keyword, value, cmd_params)
             else:
                 raise RuntimeError(
                     "Missing value for last command parameter: {:s}".format(text)
                 )
 
-    return target_name, cmd_name, cmd_params
+    return [target_name, cmd_name, cmd_params]
 
 
 def extract_fields_from_tlm_text(text):
     split_string = text.split(" ")
     if len(split_string) != 3:
         raise RuntimeError(
             f"ERROR: Telemetry Item must be specified as 'TargetName PacketName ItemName' : {text}"
         )
     target_name = split_string[0]
     packet_name = split_string[1]
     item_name = split_string[2]
-    return target_name, packet_name, item_name
+    return [target_name, packet_name, item_name]
 
 
 def extract_fields_from_set_tlm_text(text):
     error_msg = f"ERROR: Set Telemetry Item must be specified as 'TargetName PacketName ItemName = Value' : {text}"
     # We have to handle these cases:
     # set_tlm("TGT PKT ITEM='new item'")
     # set_tlm("TGT PKT ITEM = 'new item'")
     # set_tlm("TGT PKT ITEM= 'new item'")
     # set_tlm("TGT PKT ITEM ='new item'")
-    initial_split = text.split("=")
-    if len(initial_split) < 2 or not initial_split[1].strip():
+    split_string = text.split("=")
+    if len(split_string) < 2 or not split_string[1].strip():
         raise RuntimeError(error_msg)
-    parts = initial_split[0].strip().split(" ") + [initial_split[1].strip()]
-
-    if len(parts) != 4:  # Ensure tgt,pkt,item,value
+    split_string = (
+        split_string[0].strip().split(" ") + "=".join(split_string[1:]).strip()
+    )
+    if len(split_string) != 4:  # Ensure tgt,pkt,item,value
         raise RuntimeError(error_msg)
-    target_name = parts[0]
-    packet_name = parts[1]
-    item_name = parts[2]
-    value = convert_to_value(parts[3])
+    target_name = split_string[0]
+    packet_name = split_string[1]
+    item_name = split_string[2]
+    value = convert_to_value(split_string[3].strip())
     if isinstance(value, str):
         value = remove_quotes(value)
-    return target_name, packet_name, item_name, value
+    return [target_name, packet_name, item_name, value]
 
 
 def extract_fields_from_check_text(text):
     split_string = text.split(" ")
     if len(split_string) < 3:
         raise RuntimeError(f"ERROR: Check improperly specified: {text}")
     target_name = split_string[0]
@@ -246,8 +250,8 @@
         raise RuntimeError(f"ERROR: Check improperly specified: {text}")
 
     # TODO: Ruby version has additional code to split on regex spaces
     comparison_to_eval = " ".join(split_string[3:])
     if split_string[3] == "=":
         raise RuntimeError(f"ERROR: Use '==' instead of '=': {text}")
 
-    return target_name, packet_name, item_name, comparison_to_eval
+    return [target_name, packet_name, item_name, comparison_to_eval]
```

### Comparing `openc3-5.16.0/openc3/utilities/logger.py` & `openc3-5.9.2b0/openc3/utilities/logger.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,228 +11,118 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import socket
+import time
 import sys
 import json
-from datetime import datetime, timezone
+from datetime import datetime
 from threading import Lock
 from openc3.environment import *
-from openc3.utilities.store_queued import EphemeralStoreQueued
-
-# Logger class, class attribute list
-CLASS_ATTRS = [
-    "instance",
-    "instance_mutex",
-    "my_instance",
-    "scope",
-    "__dict__",
-    "DEBUG",
-    "INFO",
-    "WARN",
-    "ERROR",
-    "FATAL",
-    "DEBUG_LEVEL",
-    "INFO_LEVEL",
-    "WARN_LEVEL",
-    "ERROR_LEVEL",
-    "FATAL_LEVEL",
-    "LOG",
-    "NOTIFICATION",
-    "ALERT",
-]
-
-
-# Logger class, instance attribute list
-INSTANCE_ATTRS = [
-    "stdout",
-    "level",
-    "detail_string",
-    "container_name",
-    "microservice_name",
-    "no_store",
-]
-
+from openc3.topics.topic import Topic
 
 class LoggerMeta(type):
     def __getattribute__(cls, func):
-        if func in CLASS_ATTRS:
+        if func == 'instance' or func == 'instance_mutex' or func == 'my_instance':
             return super().__getattribute__(func)
-
-        if func in INSTANCE_ATTRS:
-            return getattr(cls.instance(), func)
-
         def method(*args, **kw_args):
             return getattr(cls.instance(), func)(*args, **kw_args)
-
         return method
 
-    def __setattr__(cls, func, value):
-        if func in INSTANCE_ATTRS:
-            return setattr(cls.instance(), func, value)
-
-        if func in CLASS_ATTRS:
-            return super().__setattr__(func, value)
-
-        raise AttributeError(f"Unknown attribute {func}")
-
-
 # Supports different levels of logging and only writes if the level
 # is exceeded.
 class Logger(metaclass=LoggerMeta):
     instance_mutex = Lock()
     my_instance = None
-    scope = OPENC3_SCOPE
 
     DEBUG = 0
     INFO = 1
     WARN = 2
     ERROR = 3
     FATAL = 4
 
-    DEBUG_LEVEL = "DEBUG"
-    INFO_LEVEL = "INFO"
-    WARN_LEVEL = "WARN"
-    ERROR_LEVEL = "ERROR"
-    FATAL_LEVEL = "FATAL"
-
-    LOG = "log"
-    NOTIFICATION = "notification"
-    ALERT = "alert"
+    DEBUG_SEVERITY_STRING = 'DEBUG'
+    INFO_SEVERITY_STRING = 'INFO'
+    WARN_SEVERITY_STRING = 'WARN'
+    ERROR_SEVERITY_STRING = 'ERROR'
+    FATAL_SEVERITY_STRING = 'FATAL'
 
     # @param level [Integer] The initial logging level
-    def __init__(self, level=INFO):
+    def __init__(self, level = INFO):
         self.stdout = True
         self.level = level
+        self.scope = OPENC3_SCOPE
         self.detail_string = None
         self.container_name = socket.gethostname()
         self.microservice_name = None
-        if OPENC3_NO_STORE:
-            self.no_store = True
-        else:
-            self.no_store = False
+        self.no_store = OPENC3_NO_STORE
 
     # Get the singleton instance
     @classmethod
-    def instance(cls, level=INFO):
+    def instance(cls, level = INFO):
         if cls.my_instance:
             return cls.my_instance
 
         with cls.instance_mutex:
             cls.my_instance = cls(level)
             return cls.my_instance
 
     # @param message [String] The message to print if the log level is at or
     #   below the method name log level.
     # @param block [Proc] Block to call which should return a string to append
     #   to the log message
-    def debug(self, message=None, scope=None, user=None, type=LOG, url=None):
+    def debug(self, message = None, scope = None, user = None):
         scope = scope or self.scope
         if self.level <= self.DEBUG:
-            self.log_message(
-                self.DEBUG_LEVEL,
-                message,
-                scope=scope,
-                user=user,
-                type=type,
-                url=url,
-            )
+            self.log_message(self.DEBUG_SEVERITY_STRING, message, scope = scope, user = user)
 
     # (see #debug)
-    def info(self, message=None, scope=None, user=None, type=LOG, url=None):
+    def info(self, message = None, scope = None, user = None):
         scope = scope or self.scope
         if self.level <= self.INFO:
-            self.log_message(
-                self.INFO_LEVEL,
-                message,
-                scope=scope,
-                user=user,
-                type=type,
-                url=url,
-            )
+            self.log_message(self.INFO_SEVERITY_STRING, message, scope = scope, user = user)
 
     # (see #debug)
-    def warn(self, message=None, scope=None, user=None, type=LOG, url=None):
+    def warn(self, message = None, scope = None, user = None):
         scope = scope or self.scope
         if self.level <= self.WARN:
-            self.log_message(
-                self.WARN_LEVEL,
-                message,
-                scope=scope,
-                user=user,
-                type=type,
-                url=url,
-            )
+            self.log_message(self.WARN_SEVERITY_STRING, message, scope = scope, user = user)
 
     # (see #debug)
-    def error(self, message=None, scope=None, user=None, type=LOG, url=None):
+    def error(self, message = None, scope = None, user = None):
         scope = scope or self.scope
         if self.level <= self.ERROR:
-            self.log_message(
-                self.ERROR_LEVEL,
-                message,
-                scope=scope,
-                user=user,
-                type=type,
-                url=url,
-            )
+            self.log_message(self.ERROR_SEVERITY_STRING, message, scope = scope, user = user)
 
     # (see #debug)
-    def fatal(self, message=None, scope=None, user=None, type=LOG, url=None):
+    def fatal(self, message = None, scope = None, user = None):
         scope = scope or self.scope
         if self.level <= self.FATAL:
-            self.log_message(
-                self.FATAL_LEVEL,
-                message,
-                scope=scope,
-                user=user,
-                type=type,
-                url=url,
-            )
+            self.log_message(self.FATAL_SEVERITY_STRING, message, scope = scope, user = user)
 
-    def log_message(self, log_level, message, scope, user, type, url):
+    def log_message(self, severity_string, message, scope, user):
         with self.instance_mutex:
-            now_time = datetime.now(timezone.utc)
-            data = {
-                "time": now_time.timestamp() * 1000000000,
-                # Can't use isoformat because it appends "+00:00" instead of "Z"
-                "@timestamp": now_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ"),
-                "level": log_level,
-            }
+            data = { 'time': time.time() * 1000000000, '@timestamp': datetime.now().isoformat(), 'severity': severity_string }
             if self.microservice_name:
-                data["microservice_name"] = self.microservice_name
+                data['microservice_name'] = self.microservice_name
             if self.detail_string:
-                data["detail"] = self.detail_string
-            # EE: If a user is passed, put its name. Don't include user data if no user was passed.
-            if user:
-                data["user"] = user
-            data["container_name"] = self.container_name
-            data["message"] = message
-            data["type"] = type
-            if url:
-                data["url"] = url
+                data['detail'] = self.detail_string
+            if user: # EE: If a user is passed, put its name ('Unknown' if it doesn't have a name). Don't include user data if no user was passed
+                if 'username' in user:
+                    data['user'] = user['username']
+                else:
+                    data['user'] = 'Unknown'
+            data['container_name'] = self.container_name
+            data['log'] = message
             if self.stdout:
-                match log_level:
-                    case "WARN" | "ERROR" | "FATAL":
-                        if OPENC3_LOG_STDERR:
-                            print(json.dumps(data), file=sys.stderr)
-                            sys.stderr.flush()
-                        else:
-                            print(json.dumps(data), file=sys.stdout)
-                            sys.stdout.flush()
-                    case _:
-                        print(json.dumps(data), file=sys.stdout)
-                        sys.stdout.flush()
-            if self.no_store is False:
-                if scope is not None:
-                    EphemeralStoreQueued.write_topic(
-                        f"{scope}__openc3_log_messages", data
-                    )
+                print(json.dumps(data))
+                sys.stdout.flush
+            if not self.no_store:
+                if scope:
+                    Topic.write_topic(f"{scope}__openc3_log_messages", data)
                 else:
                     # The base openc3_log_messages doesn't have an associated logger
                     # so it must be limited to prevent unbounded stream growth
-                    EphemeralStoreQueued.write_topic(
-                        "NOSCOPE__openc3_log_messages", data
-                    )
+                    Topic.write_topic("openc3_log_messages", data, '*', 1000)
```

### Comparing `openc3-5.16.0/openc3/utilities/message_log.py` & `openc3-5.9.2b0/openc3/utilities/message_log.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,103 +12,90 @@
 # GNU Affero General Public License for more details.
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import os
 import time
-from datetime import datetime, timezone
+from datetime import datetime
 from threading import Lock
 from openc3.utilities.bucket_utilities import BucketUtilities
 from openc3.utilities.logger import Logger
 from openc3.environment import OPENC3_SCOPE
 
-
 # Handles writing message logs to a file
 class MessageLog:
-    @classmethod
-    def build_timestamped_filename(cls, tags=None, extension=".txt", time=None):
-        if time is None:
-            time = datetime.now(timezone.utc)
-        timestamp = time.strftime("%Y_%m_%d_%H_%M_%S")
-        tags = tags or []
-        tags = [i for i in tags if i is not None]  # Remove Nones
-        combined_tags = "_".join(tags)
-        filename = None
-        if len(combined_tags) > 0:
-            filename = timestamp + "_" + combined_tags + extension
-        else:
-            filename = timestamp + extension
-        return filename
-
-    # @param tool_name [String] The name of the tool creating the message log.
-    #   This will be inserted into the message log filename to help identify it.
-    # @param log_dir [String] The filesystem path to store the message log file.
-    # @param tags [Array<String>] Array of strings to put into the filename
-    def __init__(self, tool_name, log_dir, tags=["messages"], scope=OPENC3_SCOPE):
-        self.remote_log_directory = f"{scope}/tool_logs/{tool_name}/"
-        self.tags = [tool_name] + tags
-        self.log_dir = log_dir
-        self.filename = ""
-        self.file = None
-        self.start_day = None
-        self.mutex = Lock()
-
-    # Ensures the log file is opened and ready to write. It then writes the
-    # message to the log and flushes it to force the write.
-    #
-    # @param message [String] Message to write to the log
-    def write(self, message, flush=False):
-        with self.mutex:
-            if (
-                self.file is None
-                or self.file.closed
-                or not os.path.exists(self.filename)
-            ):
-                self.start(False)
-
-            self.file.write(message)
-            if flush:
-                self.file.flush()
-
-    # Closes the message log and marks it read only
-    def stop(self, take_mutex=True, metadata={}):
-        if take_mutex:
-            self.mutex.acquire()
-        if self.file and not self.file.closed:
-            self.file.close()
-            os.chmod(self.filename, 0o444)
-            bucket_key = os.path.join(
-                self.remote_log_directory,
-                self.start_day,
-                os.path.basename(self.filename),
-            )
-            try:
-                thread = BucketUtilities.move_log_file_to_bucket(
-                    self.filename, bucket_key, metadata=metadata
-                )
-                thread.join()
-            except Exception as e:
-                Logger.error(str(e))
-
-        if take_mutex:
-            self.mutex.release()
-
-    # Creates a new message log and sets the filename
-    def start(self, take_mutex=True):
-        if take_mutex:
-            self.mutex.acquire()
-        # Prevent starting files too fast
-        while True:
-            if os.path.exists(
-                os.path.join(self.log_dir, self.build_timestamped_filename(self.tags))
-            ):
-                time.sleep(0.1)
-            else:
-                break
-        self.stop(False)
-        timed_filename = self.build_timestamped_filename(self.tags)
-        self.start_day = timed_filename[0:10].replace("_", "")  # YYYYMMDD
-        self.filename = os.path.join(self.log_dir, timed_filename)
-        self.file = open(self.filename, "a")
-        if take_mutex:
-            self.mutex.release()
+  @classmethod
+  def build_timestamped_filename(cls, tags = None, extension = '.txt', time = None):
+    if time is None:
+        time = datetime.now()
+    timestamp = time.strftime('%Y_%m_%d_%H_%M_%S')
+    tags = tags or []
+    tags = [i for i in tags if i is not None] # Remove Nones
+    combined_tags = "_".join(tags)
+    filename = None
+    if len(combined_tags) > 0:
+        filename = timestamp + "_" + combined_tags + extension
+    else:
+        filename = timestamp + extension
+    return filename
+
+  # @param tool_name [String] The name of the tool creating the message log.
+  #   This will be inserted into the message log filename to help identify it.
+  # @param log_dir [String] The filesystem path to store the message log file.
+  # @param tags [Array<String>] Array of strings to put into the filename
+  def __init__(self, tool_name, log_dir, tags = ['messages'], scope = OPENC3_SCOPE):
+      self.remote_log_directory = f"{scope}/tool_logs/{tool_name}/"
+      self.tags = [tool_name] + tags
+      self.log_dir = log_dir
+      self.filename = ''
+      self.file = None
+      self.start_day = None
+      self.mutex = Lock()
+
+  # Ensures the log file is opened and ready to write. It then writes the
+  # message to the log and flushes it to force the write.
+  #
+  # @param message [String] Message to write to the log
+  def write(self, message, flush = False):
+      with self.mutex:
+          if self.file is None or self.file.closed or not os.path.exists(self.filename):
+            self.start(False)
+
+          self.file.write(message)
+          if flush:
+              self.file.flush()
+
+  # Closes the message log and marks it read only
+  def stop(self, take_mutex = True, metadata = {}):
+      if take_mutex:
+          self.mutex.acquire()
+      if self.file and not self.file.closed:
+          self.file.close()
+          os.chmod(self.filename, 0o444)
+          bucket_key = os.path.join(self.remote_log_directory, self.start_day, os.path.basename(self.filename))
+          try:
+              thread = BucketUtilities.move_log_file_to_bucket(self.filename, bucket_key, metadata = metadata)
+              thread.join
+          except Exception as e:
+              Logger.error(str(e))
+
+      if take_mutex:
+          self.mutex.release()
+
+  # Creates a new message log and sets the filename
+  def start(self, take_mutex = True):
+      if take_mutex:
+          self.mutex.acquire()
+      # Prevent starting files too fast
+      while True:
+          if os.path.exists(os.path.join(self.log_dir, self.build_timestamped_filename(self.tags))):
+              time.sleep(0.1)
+          else:
+              break
+      self.stop(False)
+      timed_filename = self.build_timestamped_filename(self.tags)
+      self.start_day = timed_filename[0:10].replace("_", "") # YYYYMMDD
+      self.filename = os.path.join(self.log_dir, timed_filename)
+      self.file = open(self.filename, 'a')
+      if take_mutex:
+          self.mutex.release()
```

### Comparing `openc3-5.16.0/openc3/utilities/sleeper.py` & `openc3-5.9.2b0/openc3/utilities/sleeper.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,38 +13,32 @@
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import os
 import selectors
 
-
 # Allows for a breakable sleep implementation using the self-pipe trick
 # See http://www.sitepoint.com/the-self-pipe-trick-explained/
 class Sleeper:
-    def __init__(self):
-        self.pipe_reader, self.pipe_writer = os.pipe()
-        self.selector = selectors.DefaultSelector()
-        self.selector.register(self.pipe_reader, selectors.EVENT_READ)
-        self.canceled = False
+  def __init__(self):
+      self.pipe_reader, self.pipe_writer = os.pipe()
+      self.selector = selectors.DefaultSelector()
+      self.selector.register(self.pipe_reader, selectors.EVENT_READ)
+      self.canceled = False
 
-    # Breakable version of sleep
-    # @param seconds Number of seconds to sleep
-    # @return true if the sleep was broken by someone calling cancel
-    #   otherwise returns false
-    def sleep(self, seconds):
-        list = self.selector.select(timeout=seconds)
-        if list and list[0]:
-            try:
-                os.close(self.pipe_reader)
-            except Exception:
-                pass
-            return True
-        else:
-            return False
+  # Breakable version of sleep
+  # @param seconds Number of seconds to sleep
+  # @return true if the sleep was broken by someone calling cancel
+  #   otherwise returns false
+  def sleep(self, seconds):
+      list = self.selector.select(timeout = seconds)
+      if list and list[0]:
+          return True
+      else:
+          return False
 
-    # Break sleeping - Once canceled a sleeper cannot be used again
-    def cancel(self):
-        if not self.canceled:
-            self.canceled = True
-            os.write(self.pipe_writer, bytes(".", encoding="ascii"))
-            os.close(self.pipe_writer)
+  # Break sleeping - Once canceled a sleeper cannot be used again
+  def cancel(self):
+      if not self.canceled:
+          self.canceled = True
+          os.write(self.pipe_writer, bytes('.', encoding="ascii"))
```

### Comparing `openc3-5.16.0/openc3/utilities/store.py` & `openc3-5.9.2b0/openc3/utilities/store.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 OpenC3, Inc.
+# Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
 #
@@ -13,64 +13,23 @@
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 import redis
 from redis.exceptions import TimeoutError
 from openc3.utilities.connection_pool import ConnectionPool
-from contextlib import contextmanager
 import threading
 from openc3.environment import *
 
 if OPENC3_REDIS_CLUSTER:
     openc3_redis_cluster = True
 else:
     openc3_redis_cluster = False
 
 
-class StoreConnectionPool(ConnectionPool):
-    @contextmanager
-    def pipelined(self):
-        if openc3_redis_cluster:
-            yield  # TODO: Update keys to support pipelining in cluster
-        else:
-            with self.get() as redis:
-                pipeline = redis.pipeline(transaction=False)
-                thread_id = threading.get_native_id()
-                self.pipelines[thread_id] = pipeline
-                try:
-                    yield
-                finally:
-                    pipeline.execute()
-                    self.pipelines[thread_id] = None
-
-    @contextmanager
-    def get(self):
-        thread_id = threading.get_native_id()
-        if thread_id not in self.pipelines:
-            self.pipelines[thread_id] = None
-        pipeline = self.pipelines[thread_id]
-        if pipeline:
-            yield pipeline
-        else:
-            item = None
-            with self.lock:
-                if not self.pool.empty():
-                    item = self.pool.get(False)
-                elif self.count < self.pool_size:
-                    item = self.ctor()
-                    self.count += 1
-                else:
-                    item = self.pool.get()
-            try:
-                yield item
-            finally:
-                self.pool.put(item)
-
-
 class StoreMeta(type):
     def __getattribute__(cls, func):
         if func == "instance" or func == "instance_mutex" or func == "my_instance":
             return super().__getattribute__(func)
 
         def method(*args, **kw_args):
             return getattr(cls.instance(), func)(*args, **kw_args)
@@ -103,29 +62,26 @@
                 return getattr(redis, func)(*args, **kwargs)
 
             return method
 
     def __init__(self, pool_size=10):
         self.redis_host = OPENC3_REDIS_HOSTNAME
         self.redis_port = OPENC3_REDIS_PORT
-        self.redis_pool = StoreConnectionPool(self.build_redis, pool_size)
+        self.redis_pool = ConnectionPool(self.build_redis, pool_size)
         self.topic_offsets = {}
-        self.pipelines = {}
 
     if not openc3_redis_cluster:
 
         def build_redis(self):
-            # NOTE: We can't use decode_response because it tries to decode the binary
-            # packet buffer which does not work. Thus strings come back as bytes like
-            # b"target_name" and we decode them using b"target_name".decode()
             return redis.Redis(
                 host=self.redis_host,
                 port=self.redis_port,
                 username=OPENC3_REDIS_USERNAME,
                 password=OPENC3_REDIS_PASSWORD,
+                decode_responses=True,
             )
 
     ###########################################################################
     # Stream APIs
     ###########################################################################
 
     def get_oldest_message(self, topic):
@@ -139,25 +95,23 @@
     def get_newest_message(self, topic):
         with self.redis_pool.get() as redis:
             # Default in xrevrange is range end '+', start '-' which means get all
             # elements from higher ID to lower ID and since we're limiting to 1
             # we get the last element. See https://redis.io/commands/xrevrange.
             result = redis.xrevrange(topic, count=1)
             if result and len(result) > 0:
-                first = list(result[0])
-                first[0] = first[0].decode()
-                return first
+                return result[0]
             else:
-                return (None, None)
+                return None
 
     def get_last_offset(self, topic):
         with self.redis_pool.get() as redis:
             result = redis.xrevrange(topic, count=1)
             if result and result[0] and result[0][0]:
-                return result[0][0].decode()
+                return result[0][0]
             else:
                 return "0-0"
 
     def update_topic_offsets(self, topics):
         offsets = []
         for topic in topics:
             # Normally we will just be grabbing the topic offset
@@ -182,36 +136,34 @@
             if len(topics) == 0:
                 return {}
             thread_id = threading.get_native_id()
             if thread_id not in self.topic_offsets:
                 self.topic_offsets[thread_id] = {}
             topic_offsets = self.topic_offsets[thread_id]
             try:
+                # Logger.debug "read_topics: #{topics}, #{offsets} pool:#{@redis_pool}"
                 with self.redis_pool.get() as redis:
                     if not offsets:
                         offsets = self.update_topic_offsets(topics)
                     streams = {}
                     index = 0
                     for topic in topics:
                         streams[topic] = offsets[index]
                         index += 1
                     result = redis.xread(streams, block=timeout_ms, count=count)
                     if result and len(result) > 0:
                         for topic, messages in result:
                             for msg_id, msg_hash in messages:
-                                if type(topic) is bytes:
-                                    topic = topic.decode()
-                                if type(msg_id) is bytes:
-                                    msg_id = msg_id.decode()
                                 topic_offsets[topic] = msg_id
                                 yield topic, msg_id, msg_hash, redis
                     return result
             except TimeoutError:
-                # Should return an empty hash not array - xread returns a hash
-                return {}
+                return (
+                    {}
+                )  # Should return an empty hash not array - xread returns a hash
 
     # Add new entry to the redis stream.
     # > https://www.rubydoc.info/github/redis/redis-rb/Redis:xadd
     #
     # @example Without options
     #   store.write_topic('MANGO__TOPIC', {'message' => 'something'})
     # @example With options
@@ -252,15 +204,11 @@
         with self.redis_pool.get() as redis:
             return redis.xtrim(
                 name=topic, minid=minid, approximate=approximate, limit=limit
             )
 
 
 class EphemeralStore(Store):
-    # Variable that holds the singleton instance
-    my_instance = None
-
     def __init__(self, pool_size=10):
         super().__init__(pool_size)
         self.redis_host = OPENC3_REDIS_EPHEMERAL_HOSTNAME
         self.redis_port = OPENC3_REDIS_EPHEMERAL_PORT
-        self.redis_pool = StoreConnectionPool(self.build_redis, pool_size)
```

### Comparing `openc3-5.16.0/openc3.egg-info/PKG-INFO` & `openc3-5.9.2b0/openc3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openc3
-Version: 5.16.0
+Version: 5.9.2b0
 Summary: Python Support for OpenC3 COSMOS v5
 Home-page: https://github.com/OpenC3/cosmos
 Author: Ryan Melton
 Author-email: ryan@openc3.com
 License: AGPLv3, Nonstandard
 Keywords: openc3 cosmos
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openc3-5.16.0/setup.py` & `openc3-5.9.2b0/setup.py`

 * *Files identical despite different names*

### Comparing `openc3-5.16.0/test/accessors/test_binary_accessor_read.py` & `openc3-5.9.2b0/test/accessors/test_binary_accessor_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -20,18 +22,22 @@
 from openc3.accessors.binary_accessor import BinaryAccessor
 
 
 class TestBinaryAccessorRead(unittest.TestCase):
     def setUp(self):
         self.data = b"\x80\x81\x82\x83\x84\x85\x86\x87\x00\x09\x0A\x0B\x0C\x0D\x0E\x0F"
 
+    # def test_get_host_endianness(self):
+    #     endianness = BinaryAccessor.get_host_endianness()
+    #     print(f"Host endianness:{endianness}")
+
     def test_complains_about_unknown_data_types(self):
         self.assertRaisesRegex(
             AttributeError,
-            "data_type BLOB is not recognized",
+            f"data_type BLOB is not recognized",
             BinaryAccessor.read,
             0,
             32,
             "BLOB",
             self.data,
             "BIG_ENDIAN",
         )
@@ -89,72 +95,57 @@
 
     def test_complains_about_negative_or_zero_bit_sizes_with_data_types_other_than_string_and_block(
         self,
     ):
         self.assertRaisesRegex(
             AttributeError,
             # TODO: WHat's up with this not matching
-            "bit_size -8 must be positive for data types other than 'STRING' and 'BLOCK'",
+            f"bit_size -8 must be positive for data types other than 'STRING' and 'BLOCK'",
             BinaryAccessor.read,
             0,
             -8,
             "INT",
             self.data,
             "BIG_ENDIAN",
         )
         self.assertRaisesRegex(
             AttributeError,
             # TODO: WHat's up with this not matching
-            "bit_size -8 must be positive for data types other than 'STRING' and 'BLOCK'",
+            f"bit_size -8 must be positive for data types other than 'STRING' and 'BLOCK'",
             BinaryAccessor.read,
             0,
             -8,
             "UINT",
             self.data,
             "BIG_ENDIAN",
         )
         self.assertRaisesRegex(
             AttributeError,
             # TODO: WHat's up with this not matching
-            "bit_size -8 must be positive for data types other than 'STRING' and 'BLOCK'",
+            f"bit_size -8 must be positive for data types other than 'STRING' and 'BLOCK'",
             BinaryAccessor.read,
             0,
             -8,
             "FLOAT",
             self.data,
             "BIG_ENDIAN",
         )
 
-    def test_reads_ascii_strings(self):
-        self.data = "DEADBEEF".encode()
-        self.assertEqual(
-            BinaryAccessor.read(
-                0,
-                64,
-                "STRING",
-                self.data,
-                "BIG_ENDIAN",
-            ),
-            "DEADBEEF",
-        )
-
     def test_reads_aligned_strings(self):
-        # Make the data ASCII
-        self.data = b"\x40\x41\x42\x43\x44\x45\x46\x47\x00\x59\x5A\x5B\x5C\x5D\x5E\x5F"
-        for bit_offset in range(0, len(self.data) * 8, 8):
+        for bit_offset in range(0, len(self.data) - 1, 8):
             if (bit_offset / 8) <= 7:
                 self.assertEqual(
                     BinaryAccessor.read(
                         bit_offset,
                         (len(self.data) * 8) - bit_offset,
                         "STRING",
                         self.data,
                         "BIG_ENDIAN",
                     ),
-                    self.data[int(bit_offset / 8) : 8].decode(encoding="ascii"),
+                    self.data[int(bit_offset / 8) : 8],
                 )
             elif (bit_offset / 8) == 8:
                 self.assertEqual(
                     BinaryAccessor.read(
                         bit_offset,
                         (len(self.data) * 8) - bit_offset,
                         "STRING",
@@ -168,41 +159,40 @@
                     BinaryAccessor.read(
                         bit_offset,
                         (len(self.data) * 8) - bit_offset,
                         "STRING",
                         self.data,
                         "BIG_ENDIAN",
                     ),
-                    self.data[int(bit_offset / 8) :].decode(encoding="ascii"),
+                    self.data[(bit_offset / 8) :],
                 )
 
     def test_reads_variable_length_strings_with_a_zero_and_negative_bit_size(self):
-        self.data = b"\x40\x41\x42\x43\x44\x45\x46\x47\x00\x59\x5A\x5B\x5C\x5D\x5E\x5F"
         for bit_size in range(0, -len(self.data) * 8, -8):
             if (bit_size / 8) >= -8:
                 self.assertEqual(
                     BinaryAccessor.read(0, bit_size, "STRING", self.data, "BIG_ENDIAN"),
-                    self.data[0:8].decode(),
+                    self.data[0:8],
                 )
             else:
                 self.assertEqual(
                     BinaryAccessor.read(0, bit_size, "STRING", self.data, "BIG_ENDIAN"),
-                    self.data[0 : int(bit_size / 8)].decode(),
+                    self.data[0 : int(bit_size / 8)],
                 )
 
     def test_reads_strings_with_negative_bit_offsets(self):
         self.assertEqual(
             BinaryAccessor.read(-16, 16, "STRING", self.data, "BIG_ENDIAN"),
-            self.data[-2:].decode(),
+            self.data[-2:],
         )
 
     def test_complains_about_unaligned_strings(self):
         self.assertRaisesRegex(
             AttributeError,
-            "bit_offset 1 is not byte aligned for data_type STRING",
+            f"bit_offset 1 is not byte aligned for data_type STRING",
             BinaryAccessor.read,
             1,
             32,
             "STRING",
             self.data,
             "BIG_ENDIAN",
         )
@@ -232,27 +222,27 @@
             BinaryAccessor.read(-16, 16, "BLOCK", self.data, "BIG_ENDIAN"),
             self.data[-2:],
         )
 
     def test_complains_about_unaligned_blocks(self):
         self.assertRaisesRegex(
             AttributeError,
-            "bit_offset 7 is not byte aligned for data_type BLOCK",
+            f"bit_offset 7 is not byte aligned for data_type BLOCK",
             BinaryAccessor.read,
             7,
             16,
             "BLOCK",
             self.data,
             "BIG_ENDIAN",
         )
 
     def test_complains_if_read_exceeds_the_size_of_the_buffer(self):
         self.assertRaisesRegex(
             AttributeError,
-            "16 byte buffer insufficient to read STRING at bit_offset 8 with bit_size 800",
+            f"16 byte buffer insufficient to read STRING at bit_offset 8 with bit_size 800",
             BinaryAccessor.read,
             8,
             800,
             "STRING",
             self.data,
             "BIG_ENDIAN",
         )
@@ -554,27 +544,27 @@
             BinaryAccessor.read(64, 64, "FLOAT", self.data, "BIG_ENDIAN"),
             expected_array[1],
         )
 
     def test_complains_about_unaligned_floats(self):
         self.assertRaisesRegex(
             AttributeError,
-            "bit_offset 17 is not byte aligned for data_type FLOAT",
+            f"bit_offset 17 is not byte aligned for data_type FLOAT",
             BinaryAccessor.read,
             17,
             32,
             "FLOAT",
             self.data,
             "BIG_ENDIAN",
         )
 
     def test_complains_about_mis_sized_floats(self):
         self.assertRaisesRegex(
             AttributeError,
-            "bit_size is 33 but must be 32 or 64 for data_type FLOAT",
+            f"bit_size is 33 but must be 32 or 64 for data_type FLOAT",
             BinaryAccessor.read,
             0,
             33,
             "FLOAT",
             self.data,
             "BIG_ENDIAN",
         )
@@ -583,15 +573,15 @@
 class TestBinaryAccessorReadLittleEndian(unittest.TestCase):
     def setUp(self):
         self.data = b"\x80\x81\x82\x83\x84\x85\x86\x87\x00\x09\x0A\x0B\x0C\x0D\x0E\x0F"
 
     def test_complains_about_ill_defined_little_endian_bitfields(self):
         self.assertRaisesRegex(
             AttributeError,
-            "LITTLE_ENDIAN bitfield with bit_offset 3 and bit_size 7 is invalid",
+            f"LITTLE_ENDIAN bitfield with bit_offset 3 and bit_size 7 is invalid",
             BinaryAccessor.read,
             3,
             7,
             "UINT",
             self.data,
             "LITTLE_ENDIAN",
         )
@@ -865,59 +855,61 @@
             BinaryAccessor.read(64, 64, "FLOAT", self.data, "LITTLE_ENDIAN"),
             expected_array[1],
         )
 
     def test_complains_about_unaligned_floats(self):
         self.assertRaisesRegex(
             AttributeError,
-            "bit_offset 1 is not byte aligned for data_type FLOAT",
+            f"bit_offset 1 is not byte aligned for data_type FLOAT",
             BinaryAccessor.read,
             1,
             32,
             "FLOAT",
             self.data,
             "LITTLE_ENDIAN",
         )
 
     def test_complains_about_mis_sized_floats(self):
         self.assertRaisesRegex(
             AttributeError,
-            "bit_size is 65 but must be 32 or 64 for data_type FLOAT",
+            f"bit_size is 65 but must be 32 or 64 for data_type FLOAT",
             BinaryAccessor.read,
             0,
             65,
             "FLOAT",
             self.data,
             "LITTLE_ENDIAN",
         )
 
 
 class TestBinaryAccessorReadArrayLE(unittest.TestCase):
     def setUp(self):
         self.data = b"\x80\x81\x82\x83\x84\x85\x86\x87\x00\x09\x0A\x0B\x0C\x0D\x0E\x0F"
 
     def test_complains_with_unknown_data_type(self):
-        with self.assertRaisesRegex(AttributeError, "data_type BLAH is not recognized"):
+        with self.assertRaisesRegex(
+            AttributeError, f"data_type BLAH is not recognized"
+        ):
             BinaryAccessor.read_array(0, 8, "BLAH", 0, self.data, "LITTLE_ENDIAN")
 
     def test_complains_about_negative_bit_sizes(self):
         with self.assertRaisesRegex(
-            AttributeError, "bit_size -8 must be positive for arrays"
+            AttributeError, f"bit_size -8 must be positive for arrays"
         ):
             BinaryAccessor.read_array(
                 0, -8, "UINT", len(self.data) * 8, self.data, "LITTLE_ENDIAN"
             )
 
     def test_reads_the_given_array_size_amount_of_items(self):
         self.assertEqual(
             BinaryAccessor.read_array(0, 8, "UINT", 32, self.data, "LITTLE_ENDIAN"),
-            list(self.data[0:4]),
+            self.data[0:4],
         )
 
-    def test_reads_the_given_array_size_amount_of_items2(self):
+    def test_reads_the_given_array_size_amount_of_items(self):
         self.assertEqual(
             BinaryAccessor.read_array(32, 8, "UINT", 32, self.data, "LITTLE_ENDIAN"),
             list(self.data[4:8]),
         )
 
     def test_reads_the_total_buffer_given_array_size_eql_buffer_size(self):
         data = [(x & ~(1 << 7)) - (x & (1 << 7)) for x in self.data]
@@ -926,15 +918,15 @@
                 0, 8, "INT", len(self.data) * 8, self.data, "LITTLE_ENDIAN"
             ),
             data,
         )
 
     def test_complains_with_an_array_size_not_a_multiple_of_bit_size(self):
         with self.assertRaisesRegex(
-            AttributeError, "array_size 10 not a multiple of bit_size 8"
+            AttributeError, f"array_size 10 not a multiple of bit_size 8"
         ):
             BinaryAccessor.read_array(0, 8, "UINT", 10, self.data, "LITTLE_ENDIAN")
 
     def test_reads_as_many_items_as_possible_with_a_zero_array_size(self):
         self.assertEqual(
             BinaryAccessor.read_array(0, 8, "UINT", 0, self.data, "LITTLE_ENDIAN"),
             list(self.data),
@@ -1010,35 +1002,33 @@
             r"negative or zero array_size \(-8\) cannot be given with negative bit_offset \(-32\)",
         ):
             BinaryAccessor.read_array(-32, 8, "UINT", -8, self.data, "LITTLE_ENDIAN")
 
     def test_complains_about_accessing_data_from_a_buffer_which_is_too_small(self):
         with self.assertRaisesRegex(
             AttributeError,
-            "16 byte buffer insufficient to read STRING at bit_offset 0 with bit_size 256",
+            f"16 byte buffer insufficient to read STRING at bit_offset 0 with bit_size 256",
         ):
             BinaryAccessor.read_array(0, 256, "STRING", 256, self.data, "LITTLE_ENDIAN")
 
     def test_returns_an_empty_array_when_passed_a_zero_length_buffer(self):
         self.assertEqual(
             BinaryAccessor.read_array(0, 8, "UINT", 32, b"", "LITTLE_ENDIAN"), []
         )
 
     def test_complains_about_unaligned_strings(self):
         with self.assertRaisesRegex(
-            AttributeError, "bit_offset 1 is not byte aligned for data_type STRING"
+            AttributeError, f"bit_offset 1 is not byte aligned for data_type STRING"
         ):
             BinaryAccessor.read_array(1, 32, "STRING", 32, self.data, "LITTLE_ENDIAN")
 
     def test_reads_a_single_string_item(self):
-        # Make the data ASCII
-        self.data = b"\x40\x41\x42\x43\x44\x45\x46\x47\x00\x59\x5A\x5B\x5C\x5D\x5E\x5F"
         self.assertEqual(
             BinaryAccessor.read_array(0, 128, "STRING", 0, self.data, "LITTLE_ENDIAN"),
-            [self.data[0:8].decode()],
+            [self.data[0:8]],
         )
 
     def test_reads_a_single_block_item(self):
         self.assertEqual(
             BinaryAccessor.read_array(0, 128, "BLOCK", 0, self.data, "LITTLE_ENDIAN"),
             [self.data],
         )
@@ -1058,15 +1048,15 @@
             BinaryAccessor.read_array(0, 1, "INT", 2, self.data, "LITTLE_ENDIAN"),
             expected[0:2],
         )
 
     def test_complains_about_little_endian_bit_fields_greater_than_1_bit(self):
         with self.assertRaisesRegex(
             AttributeError,
-            "read_array does not support little endian bit fields with bit_size greater than 1-bit",
+            f"read_array does not support little endian bit fields with bit_size greater than 1-bit",
         ):
             BinaryAccessor.read_array(8, 7, "UINT", 21, self.data, "LITTLE_ENDIAN")
 
     def test_reads_16_bit_uint_items(self):
         data = [0x8180, 0x8382, 0x8584, 0x8786, 0x0900, 0x0B0A, 0x0D0C, 0x0F0E]
         self.assertEqual(
             BinaryAccessor.read_array(0, 16, "UINT", 0, self.data, "LITTLE_ENDIAN"),
@@ -1122,21 +1112,21 @@
             0, 64, "FLOAT", 0, self.data, "LITTLE_ENDIAN"
         )
         for index, val in enumerate(actual):
             self.assertAlmostEqual(val, expected_array[index])
 
     def test_complains_about_unaligned_floats(self):
         with self.assertRaisesRegex(
-            AttributeError, "bit_offset 1 is not byte aligned for data_type FLOAT"
+            AttributeError, f"bit_offset 1 is not byte aligned for data_type FLOAT"
         ):
             BinaryAccessor.read_array(1, 32, "FLOAT", 32, self.data, "LITTLE_ENDIAN")
 
     def test_complains_about_mis_sized_floats(self):
         with self.assertRaisesRegex(
-            AttributeError, "bit_size is 65 but must be 32 or 64 for data_type FLOAT"
+            AttributeError, f"bit_size is 65 but must be 32 or 64 for data_type FLOAT"
         ):
             BinaryAccessor.read_array(0, 65, "FLOAT", 65, self.data, "LITTLE_ENDIAN")
 
 
 class TestBinaryAccessorReadArrayBE(unittest.TestCase):
     def setUp(self):
         self.data = b"\x80\x81\x82\x83\x84\x85\x86\x87\x00\x09\x0A\x0B\x0C\x0D\x0E\x0F"
```

### Comparing `openc3-5.16.0/test/accessors/test_binary_accessor_write.py` & `openc3-5.9.2b0/test/accessors/test_binary_accessor_write.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
@@ -10,15 +12,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
-import math
 import struct
 import unittest
 from unittest.mock import *
 from test.test_helper import *
 from openc3.accessors.binary_accessor import BinaryAccessor
 
 
@@ -30,15 +31,15 @@
         self.baseline_data = bytearray(
             b"\x80\x81\x82\x83\x84\x85\x86\x87\x00\x09\x0A\x0B\x0C\x0D\x0E\x0F"
         )
 
     def test_complains_about_unknown_data_types(self):
         self.assertRaisesRegex(
             AttributeError,
-            "data_type BLOB is not recognized",
+            f"data_type BLOB is not recognized",
             BinaryAccessor.write,
             0,
             0,
             32,
             "BLOB",
             self.data,
             "BIG_ENDIAN",
@@ -398,26 +399,14 @@
             "STRING",
             self.data,
             "BIG_ENDIAN",
             "ERROR",
         )
         self.assertEqual(self.data, b"\x00\x00\x00\x00\x00\x00\x00\x00")
 
-    def test_writes_a_string_with_zero_bit_size(self):
-        BinaryAccessor.write(
-            "This is a test",
-            0,
-            0,
-            "STRING",
-            self.data,
-            "BIG_ENDIAN",
-            "ERROR",
-        )
-        self.assertEqual(self.data, b"This is a test")
-
     def test_writes_a_shorter_block_with_zero_bit_size(self):
         BinaryAccessor.write(
             b"\x00\x00\x00\x00\x00\x00\x00\x00",
             0,
             0,
             "BLOCK",
             self.data,
@@ -816,34 +805,14 @@
         )
         self.assertAlmostEqual(
             BinaryAccessor.read(96, 32, "FLOAT", self.data, "BIG_ENDIAN"),
             expected_array[3],
             31,
         )
 
-    def test_writes_simple_floats(self):
-        data_len = len(self.data)
-        BinaryAccessor.write(5.5, 0, 32, "FLOAT", self.data, "BIG_ENDIAN", "ERROR")
-        self.assertEqual(
-            5.5, BinaryAccessor.read(0, 32, "FLOAT", self.data, "BIG_ENDIAN")
-        )
-        self.assertEqual(data_len, len(self.data))  # buffer shouldn't grow
-        BinaryAccessor.write(
-            float("nan"), 0, 32, "FLOAT", self.data, "BIG_ENDIAN", "ERROR"
-        )
-        nan = BinaryAccessor.read(0, 32, "FLOAT", self.data, "BIG_ENDIAN")
-        self.assertTrue(math.isnan(nan))
-        self.assertEqual(data_len, len(self.data))  # buffer shouldn't grow
-        BinaryAccessor.write(
-            float("inf"), 0, 32, "FLOAT", self.data, "BIG_ENDIAN", "ERROR"
-        )
-        inf = BinaryAccessor.read(0, 32, "FLOAT", self.data, "BIG_ENDIAN")
-        self.assertTrue(math.isinf(inf))
-        self.assertEqual(data_len, len(self.data))  # buffer shouldn't grow
-
     def test_writes_37_bit_unsigned_integers(self):
         BinaryAccessor.write(
             0x8182838485 >> 3, 8, 37, "UINT", self.data, "BIG_ENDIAN", "ERROR"
         )
         BinaryAccessor.write(
             0x00090A0B0C, 67, 37, "UINT", self.data, "BIG_ENDIAN", "ERROR"
         )
@@ -1012,29 +981,29 @@
             "BIG_ENDIAN",
             "ERROR",
         )
 
     def test_complains_about_unaligned_floats(self):
         self.assertRaisesRegex(
             AttributeError,
-            "bit_offset 17 is not byte aligned for data_type FLOAT",
+            f"bit_offset 17 is not byte aligned for data_type FLOAT",
             BinaryAccessor.write,
             0.0,
             17,
             32,
             "FLOAT",
             self.data,
             "BIG_ENDIAN",
             "ERROR",
         )
 
     def test_complains_about_mis_sized_floats(self):
         self.assertRaisesRegex(
             AttributeError,
-            "bit_size is 33 but must be 32 or 64 for data_type FLOAT",
+            f"bit_size is 33 but must be 32 or 64 for data_type FLOAT",
             BinaryAccessor.write,
             0.0,
             0,
             33,
             "FLOAT",
             self.data,
             "BIG_ENDIAN",
@@ -1050,15 +1019,15 @@
         self.baseline_data = bytearray(
             b"\x80\x81\x82\x83\x84\x85\x86\x87\x00\x09\x0A\x0B\x0C\x0D\x0E\x0F"
         )
 
     def test_complains_about_ill_defined_little_endian_bitfields(self):
         self.assertRaisesRegex(
             AttributeError,
-            "LITTLE_ENDIAN bitfield with bit_offset 3 and bit_size 7 is invalid",
+            f"LITTLE_ENDIAN bitfield with bit_offset 3 and bit_size 7 is invalid",
             BinaryAccessor.write,
             0x1,
             3,
             7,
             "UINT",
             self.data,
             "LITTLE_ENDIAN",
@@ -1404,32 +1373,32 @@
         )
         self.assertAlmostEqual(
             BinaryAccessor.read(64, 64, "FLOAT", self.data, "LITTLE_ENDIAN"),
             expected_array[1],
             236,
         )
 
-    def test_le_complains_about_unaligned_floats(self):
+    def test_complains_about_unaligned_floats(self):
         self.assertRaisesRegex(
             AttributeError,
-            "bit_offset 1 is not byte aligned for data_type FLOAT",
+            f"bit_offset 1 is not byte aligned for data_type FLOAT",
             BinaryAccessor.write,
             0.0,
             1,
             32,
             "FLOAT",
             self.data,
             "LITTLE_ENDIAN",
             "ERROR",
         )
 
     def test_complains_about_mis_sized_floats(self):
         self.assertRaisesRegex(
             AttributeError,
-            "bit_size is 65 but must be 32 or 64 for data_type FLOAT",
+            f"bit_size is 65 but must be 32 or 64 for data_type FLOAT",
             BinaryAccessor.write,
             0.0,
             0,
             65,
             "FLOAT",
             self.data,
             "LITTLE_ENDIAN",
@@ -1442,15 +1411,15 @@
         self.data = bytearray(
             b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
         )
 
     def test_handles_invalid_overflow_types(self):
         self.assertRaisesRegex(
             AttributeError,
-            "unknown overflow type OTHER",
+            f"unknown overflow type OTHER",
             BinaryAccessor.write,
             b"abcde",
             0,
             32,
             "STRING",
             self.data,
             "BIG_ENDIAN",
@@ -1609,21 +1578,25 @@
             b"\x80\x81\x82\x83\x84\x85\x86\x87\x00\x09\x0A\x0B\x0C\x0D\x0E\x0F"
         )
         self.baseline_data_array = []
         for i in range(len(self.baseline_data)):
             self.baseline_data_array.append(self.baseline_data[i])
 
     def test_complains_about_value_other_than_array(self):
-        with self.assertRaisesRegex(AttributeError, "values must be a list but is str"):
+        with self.assertRaisesRegex(
+            AttributeError, f"values must be a list but is str"
+        ):
             BinaryAccessor.write_array(
                 "", 0, 32, "STRING", 0, self.data, "BIG_ENDIAN", "ERROR"
             )
 
     def test_complains_about_unknown_data_types(self):
-        with self.assertRaisesRegex(AttributeError, "data_type BLOB is not recognized"):
+        with self.assertRaisesRegex(
+            AttributeError, f"data_type BLOB is not recognized"
+        ):
             BinaryAccessor.write_array(
                 [0], 0, 32, "BLOB", 0, self.data, "BIG_ENDIAN", "ERROR"
             )
 
     def test_complains_about_bit_offsets_before_the_beginning_of_the_buffer(self):
         with self.assertRaisesRegex(
             AttributeError,
@@ -1651,21 +1624,21 @@
             "BIG_ENDIAN",
             "ERROR",
         )
         self.assertEqual(self.data, self.baseline_data)
 
     def test_complains_about_a_negative_or_zero_bit_size(self):
         with self.assertRaisesRegex(
-            AttributeError, "bit_size 0 must be positive for arrays"
+            AttributeError, f"bit_size 0 must be positive for arrays"
         ):
             BinaryAccessor.write_array(
                 [""], 0, 0, "STRING", 0, self.data, "BIG_ENDIAN", "ERROR"
             )
         with self.assertRaisesRegex(
-            AttributeError, "bit_size -8 must be positive for arrays"
+            AttributeError, f"bit_size -8 must be positive for arrays"
         ):
             BinaryAccessor.write_array(
                 [""], 0, -8, "STRING", 0, self.data, "BIG_ENDIAN", "ERROR"
             )
 
     def test_writes_aligned_strings_with_fixed_array_size(self):
         data = self.data[:]
@@ -1705,15 +1678,15 @@
             "BIG_ENDIAN",
             "ERROR",
         )
         self.assertEqual(self.data, (b"\x00" * 14) + self.baseline_data[14:16])
 
     def test_complains_about_unaligned_strings(self):
         with self.assertRaisesRegex(
-            AttributeError, "bit_offset 1 is not byte aligned for data_type STRING"
+            AttributeError, f"bit_offset 1 is not byte aligned for data_type STRING"
         ):
             BinaryAccessor.write_array(
                 [], 1, 32, "STRING", 32, self.data, "BIG_ENDIAN", "ERROR"
             )
 
     def test_complains_if_pass_more_values_than_the_given_array_size_can_hold(self):
         with self.assertRaisesRegex(
@@ -1790,23 +1763,23 @@
             "BIG_ENDIAN",
             "ERROR",
         )
         self.assertEqual(self.data, (b"\x00" * 12) + self.baseline_data[0:4])
 
     def test_complains_with_a_pos_array_size_not_a_multiple_of_bit_size(self):
         with self.assertRaisesRegex(
-            AttributeError, "array_size 10 not a multiple of bit_size 8"
+            AttributeError, f"array_size 10 not a multiple of bit_size 8"
         ):
             BinaryAccessor.write_array(
                 [1, 2], 0, 8, "UINT", 10, self.data, "BIG_ENDIAN", "ERROR"
             )
 
     def test_complains_with_a_neg_array_size_not_a_multiple_of_bit_size(self):
         with self.assertRaisesRegex(
-            AttributeError, "array_size -10 not a multiple of bit_size 8"
+            AttributeError, f"array_size -10 not a multiple of bit_size 8"
         ):
             BinaryAccessor.write_array(
                 [1, 2], 0, 8, "UINT", -10, self.data, "BIG_ENDIAN", "ERROR"
             )
 
     def test_excludes_the_remaining_bits_if_array_size_is_negative(self):
         data = self.data[:]
@@ -1922,15 +1895,15 @@
             "ERROR",
         )
         self.assertEqual(
             self.data,
             b"\x01\x02\x00\x00\x01\x02\x00\x00\x01\x02\x00\x00\x01\x02\x00\x00",
         )
 
-    def test_writes_a_shorter_block_and_zero_fill_to_the_given_bit_size(self):
+    def test_writes_a_shorter_string_and_zero_fill_to_the_given_bit_size(self):
         self.data = bytearray(
             b"\x80\x81\x82\x83\x84\x85\x86\x87\x00\x09\x0A\x0B\x0C\x0D\x0E\x0F"
         )
         BinaryAccessor.write_array(
             [b"\x01\x02", b"\x01\x02", b"\x01\x02", b"\x01\x02"],
             0,
             32,
@@ -1943,15 +1916,15 @@
         self.assertEqual(
             self.data,
             b"\x01\x02\x00\x00\x01\x02\x00\x00\x01\x02\x00\x00\x01\x02\x00\x00",
         )
 
     def test_complains_about_unaligned_blocks(self):
         with self.assertRaisesRegex(
-            AttributeError, "bit_offset 7 is not byte aligned for data_type BLOCK"
+            AttributeError, f"bit_offset 7 is not byte aligned for data_type BLOCK"
         ):
             BinaryAccessor.write_array(
                 self.baseline_data_array[0:2],
                 7,
                 16,
                 "BLOCK",
                 32,
@@ -1959,15 +1932,15 @@
                 "BIG_ENDIAN",
                 "ERROR",
             )
 
     def test_complains_if_write_exceeds_the_size_of_the_buffer(self):
         with self.assertRaisesRegex(
             AttributeError,
-            "16 byte buffer insufficient to write STRING at bit_offset 8 with bit_size 800",
+            f"16 byte buffer insufficient to write STRING at bit_offset 8 with bit_size 800",
         ):
             BinaryAccessor.write_array(
                 [], 8, 800, "STRING", 800, self.data, "BIG_ENDIAN", "ERROR"
             )
 
     def test_writes_aligned_8_bit_unsigned_integers(self):
         BinaryAccessor.write_array(
@@ -1991,17 +1964,17 @@
             0,
             self.data,
             "BIG_ENDIAN",
             "ERROR",
         )
         self.assertEqual(self.data, b"\x00\x01\x02\x03\x04\x05\xFF\x7F")
 
-    def test_complains_about_unaligned_strings_bin(self):
+    def test_complains_about_unaligned_strings(self):
         with self.assertRaisesRegex(
-            AttributeError, "bit_offset 1 is not byte aligned for data_type STRING"
+            AttributeError, f"bit_offset 1 is not byte aligned for data_type STRING"
         ):
             BinaryAccessor.write_array(
                 [b"X"], 1, 32, "STRING", 32, self.data, "BIG_ENDIAN", "ERROR"
             )
 
     def test_writes_string_items(self):
         BinaryAccessor.write_array(
@@ -2255,23 +2228,23 @@
         )
         self.assertAlmostEqual(
             BinaryAccessor.read(64, 64, "FLOAT", self.data, "BIG_ENDIAN"), data[1]
         )
 
     def test_complains_about_unaligned_floats(self):
         with self.assertRaisesRegex(
-            AttributeError, "bit_offset 17 is not byte aligned for data_type FLOAT"
+            AttributeError, f"bit_offset 17 is not byte aligned for data_type FLOAT"
         ):
             BinaryAccessor.write_array(
                 [0.0], 17, 32, "FLOAT", 32, self.data, "BIG_ENDIAN", "ERROR"
             )
 
     def test_complains_about_mis_sized_floats(self):
         with self.assertRaisesRegex(
-            AttributeError, "bit_size is 33 but must be 32 or 64 for data_type FLOAT"
+            AttributeError, f"bit_size is 33 but must be 32 or 64 for data_type FLOAT"
         ):
             BinaryAccessor.write_array(
                 [0.0], 0, 33, "FLOAT", 33, self.data, "BIG_ENDIAN", "ERROR"
             )
 
 
 class TestBinaryAccessorWriteArrayLittleEndian(unittest.TestCase):
@@ -2303,15 +2276,15 @@
             [1, 0, 1], 8, 1, "INT", 0, self.data, "LITTLE_ENDIAN", "ERROR"
         )
         self.assertEqual(self.data, b"\x00\xA0")
 
     def test_complains_about_little_endian_bit_fields_greater_than_1_bit(self):
         with self.assertRaisesRegex(
             AttributeError,
-            "write_array does not support little endian bit fields with bit_size greater than 1-bit",
+            f"write_array does not support little endian bit fields with bit_size greater than 1-bit",
         ):
             BinaryAccessor.write_array(
                 [0x40, 0x60, 0x50],
                 8,
                 7,
                 "UINT",
                 21,
@@ -2403,23 +2376,23 @@
             BinaryAccessor.read(64, 64, "FLOAT", self.data, "LITTLE_ENDIAN"),
             data[1],
             236,
         )
 
     def test_complains_about_unaligned_floats(self):
         with self.assertRaisesRegex(
-            AttributeError, "bit_offset 1 is not byte aligned for data_type FLOAT"
+            AttributeError, f"bit_offset 1 is not byte aligned for data_type FLOAT"
         ):
             BinaryAccessor.write_array(
                 [0.0], 1, 32, "FLOAT", 32, self.data, "LITTLE_ENDIAN", "ERROR"
             )
 
     def test_complains_about_mis_sized_floats(self):
         with self.assertRaisesRegex(
-            AttributeError, "bit_size is 65 but must be 32 or 64 for data_type FLOAT"
+            AttributeError, f"bit_size is 65 but must be 32 or 64 for data_type FLOAT"
         ):
             BinaryAccessor.write_array(
                 [0.0], 0, 65, "FLOAT", 65, self.data, "LITTLE_ENDIAN", "ERROR"
             )
 
 
 class TestBinaryAccessorWriteOverflow(unittest.TestCase):
@@ -2427,24 +2400,24 @@
         self.data = bytearray(
             b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
         )
 
     def test_prevents_overflow_of_string(self):
         with self.assertRaisesRegex(
             AttributeError,
-            "value of 5 bytes does not fit into 4 bytes for data_type STRING",
+            f"value of 5 bytes does not fit into 4 bytes for data_type STRING",
         ):
             BinaryAccessor.write_array(
                 ["abcde"], 0, 32, "STRING", 32, self.data, "BIG_ENDIAN", "ERROR"
             )
 
     def test_prevents_overflow_of_block(self):
         with self.assertRaisesRegex(
             AttributeError,
-            "value of 5 bytes does not fit into 4 bytes for data_type BLOCK",
+            f"value of 5 bytes does not fit into 4 bytes for data_type BLOCK",
         ):
             BinaryAccessor.write_array(
                 ["abcde"], 0, 32, "BLOCK", 32, self.data, "BIG_ENDIAN", "ERROR"
             )
 
     def test_prevents_overflow_of_8_bit_int(self):
         bit_size = 8
@@ -2634,96 +2607,150 @@
 
     def test_truncates_block(self):
         BinaryAccessor.write_array(
             [b"abcde"], 0, 32, "BLOCK", 32, self.data, "BIG_ENDIAN", "TRUNCATE"
         )
         self.assertEqual(self.data[0:5], b"abcd\x00")
 
-    def test_truncates_ints(self):
-        for bit_size in [3, 5, 8, 16, 32, 64]:
-            data_type = "INT"
-            value = 2 ** (bit_size - 1)
-            truncated_value = -value
-            BinaryAccessor.write_array(
-                [value],
-                0,
-                bit_size,
-                data_type,
-                bit_size,
-                self.data,
-                "BIG_ENDIAN",
-                "TRUNCATE",
-            )
-            self.assertEqual(
-                BinaryAccessor.read(0, bit_size, data_type, self.data, "BIG_ENDIAN"),
-                truncated_value,
-            )
-
-    def test_truncates_uints(self):
-        for bit_size in [3, 5, 8, 16, 32, 64]:
-            data_type = "INT"
-            value = 2**bit_size + 1
-            truncated_value = 1
-            BinaryAccessor.write_array(
-                [value],
-                0,
-                bit_size,
-                data_type,
-                bit_size,
-                self.data,
-                "BIG_ENDIAN",
-                "TRUNCATE",
-            )
-            self.assertEqual(
-                BinaryAccessor.read(0, bit_size, data_type, self.data, "BIG_ENDIAN"),
-                truncated_value,
-            )
-
-    def test_saturates_ints(self):
-        for bit_size in [3, 5, 8, 16, 32, 64]:
-            data_type = "INT"
-            value = 2 ** (bit_size - 1)
-            saturated_value = value - 1
-            BinaryAccessor.write_array(
-                [value],
-                0,
-                bit_size,
-                data_type,
-                bit_size,
-                self.data,
-                "BIG_ENDIAN",
-                "SATURATE",
-            )
-            self.assertEqual(
-                BinaryAccessor.read(0, bit_size, data_type, self.data, "BIG_ENDIAN"),
-                saturated_value,
-            )
+    # def test_truncates_ints(self):
+    #     for bit_size in [3, 5, 8, 16, 32, 64]:
+    #         data_type = "INT"
+    #         value = 2 ** (bit_size - 1)
+    #         truncated_value = -value
+    #         BinaryAccessor.write_array(
+    #             [value],
+    #             0,
+    #             bit_size,
+    #             data_type,
+    #             bit_size,
+    #             self.data,
+    #             "BIG_ENDIAN",
+    #             "TRUNCATE",
+    #         )
+    #         self.assertEqual(
+    #             BinaryAccessor.read(0, bit_size, data_type, self.data, "BIG_ENDIAN"),
+    #             truncated_value,
+    #         )
 
-    def test_saturates_uints(self):
-        for bit_size in [3, 5, 8, 16, 32, 64]:
-            data_type = "UINT"
-            value = 2**bit_size
-            saturated_value = value - 1
-            BinaryAccessor.write_array(
-                [value],
-                0,
-                bit_size,
-                data_type,
-                bit_size,
-                self.data,
-                "BIG_ENDIAN",
-                "SATURATE",
-            )
-            self.assertEqual(
-                BinaryAccessor.read(0, bit_size, data_type, self.data, "BIG_ENDIAN"),
-                saturated_value,
-            )
+    # def test_truncates_8_bit_int(self):
+    #     bit_size = 8
+    #     data_type = "INT"
+    #     value = 2 ** (bit_size - 1)
+    #     truncated_value = -value
+    #     BinaryAccessor.write_array(
+    #         [value],
+    #         0,
+    #         bit_size,
+    #         data_type,
+    #         bit_size,
+    #         self.data,
+    #         "BIG_ENDIAN",
+    #         "TRUNCATE",
+    #     )
+    #     self.assertEqual(
+    #         BinaryAccessor.read(0, bit_size, data_type, self.data, "BIG_ENDIAN"),
+    #         truncated_value,
+    #     )
 
+    # def test_truncates_16_bit_int(self):
+    #       bit_size = 16; data_type = 'INT'; value = 2**(bit_size - 1); truncated_value = -value
+    #       BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+    #       self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+    # def test_truncates_32_bit_int(self):
+    #       bit_size = 32; data_type = 'INT'; value = 2**(bit_size - 1); truncated_value = -value
+    #       BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+    #       self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+    # def test_truncates_64_bit_int(self):
+    #       bit_size = 64; data_type = 'INT'; value = 2**(bit_size - 1); truncated_value = -value
+    #       BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+    #       self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+
+#     def test_truncates_3_bit_int(self):
+#           bit_size = 3; data_type = 'INT'; value = 2**(bit_size - 1); truncated_value = -value
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+#     def test_truncates_8_bit_uint(self):
+#           bit_size = 8; data_type = 'UINT'; value = 2**bit_size + 1; truncated_value = 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+#     def test_truncates_16_bit_uint(self):
+#           bit_size = 16; data_type = 'UINT'; value = 2**bit_size + 1; truncated_value = 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+#     def test_truncates_32_bit_uint(self):
+#           bit_size = 32; data_type = 'UINT'; value = 2**bit_size + 1; truncated_value = 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+#     def test_truncates_64_bit_uint(self):
+#           bit_size = 64; data_type = 'UINT'; value = 2**bit_size + 1; truncated_value = 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+#     def test_truncates_3_bit_uint(self):
+#           bit_size = 3; data_type = 'UINT'; value = 2**bit_size + 1; truncated_value = 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+#     def test_saturates_8_bit_int(self):
+#           bit_size = 8; data_type = 'INT'; value = 2**(bit_size - 1); saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_16_bit_int(self):
+#           bit_size = 16; data_type = 'INT'; value = 2**(bit_size - 1); saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_32_bit_int(self):
+#           bit_size = 32; data_type = 'INT'; value = 2**(bit_size - 1); saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_64_bit_int(self):
+#           bit_size = 64; data_type = 'INT'; value = 2**(bit_size - 1); saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_3_bit_int(self):
+#           bit_size = 3; data_type = 'INT'; value = 2**(bit_size - 1); saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_8_bit_uint(self):
+#           bit_size = 8; data_type = 'UINT'; value = 2**bit_size; saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_16_bit_uint(self):
+#           bit_size = 16; data_type = 'UINT'; value = 2**bit_size; saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_32_bit_uint(self):
+#           bit_size = 32; data_type = 'UINT'; value = 2**bit_size; saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_64_bit_uint(self):
+#           bit_size = 64; data_type = 'UINT'; value = 2**bit_size; saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_3_bit_uint(self):
+#           bit_size = 3; data_type = 'UINT'; value = 2**bit_size; saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
 
-# TODO: Do we need these?
 #     def test_allows_hex_value_entry_of_8_bit_int(self):
 #           bit_size = 8; data_type = 'INT'; value = 2**bit_size - 1; allowed_value = -1
 #           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'ERROR_ALLOW_HEX')
 #           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), allowed_value)
 
 #     def test_allows_hex_value_entry_of_16_bit_int(self):
 #           bit_size = 16; data_type = 'INT'; value = 2**bit_size - 1; allowed_value = -1
```

### Comparing `openc3-5.16.0/test/config/test_config_parser.py` & `openc3-5.9.2b0/test/config/test_config_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addums as found in the LICENSE.txt
@@ -10,14 +12,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
+import json
 import unittest
 import tempfile
 from unittest.mock import *
 from test.test_helper import *
 from openc3.config.config_parser import ConfigParser
 
 
@@ -340,15 +343,15 @@
         tf.writelines(line)
         tf.seek(0)
 
         for keyword, params in self.cp.parse_file(tf.name):
             self.assertEqual(keyword, "KEYWORD")
             self.assertRaisesRegex(
                 ConfigParser.Error,
-                "Too many parameters for KEYWORD",
+                f"Too many parameters for KEYWORD",
                 self.cp.verify_num_parameters,
                 1,
                 1,
             )
         tf.close()
 
     def test_verifies_parameters_do_not_have_bad_characters(self):
@@ -356,33 +359,33 @@
         line = "KEYWORD BAD1_ BAD__2 'BAD 3' }BAD_4"
         tf.writelines(line)
         tf.seek(0)
 
         for keyword, params in self.cp.parse_file(tf.name):
             self.assertRaisesRegex(
                 ConfigParser.Error,
-                "cannot end with an underscore",
+                f"cannot end with an underscore",
                 self.cp.verify_parameter_naming,
                 1,
             )
             self.assertRaisesRegex(
                 ConfigParser.Error,
-                "cannot contain a double underscore",
+                f"cannot contain a double underscore",
                 self.cp.verify_parameter_naming,
                 2,
             )
             self.assertRaisesRegex(
                 ConfigParser.Error,
-                "cannot contain a space",
+                f"cannot contain a space",
                 self.cp.verify_parameter_naming,
                 3,
             )
             self.assertRaisesRegex(
                 ConfigParser.Error,
-                "cannot start with a close bracket",
+                f"cannot start with a close bracket",
                 self.cp.verify_parameter_naming,
                 4,
             )
         tf.close()
 
     def test_returns_an_error(self):
         tf = tempfile.NamedTemporaryFile(mode="w+t")
@@ -536,31 +539,31 @@
             ConfigParser.handle_defined_constants("POS_INFINITY"), float("inf")
         )
         self.assertEqual(
             ConfigParser.handle_defined_constants("NEG_INFINITY"), float("-inf")
         )
         self.assertRaisesRegex(
             AttributeError,
-            "Invalid bit size 16 for FLOAT type.",
+            f"Invalid bit size 16 for FLOAT type.",
             ConfigParser.handle_defined_constants,
             "MIN",
             "FLOAT",
             16,
         )
 
     def test_complains_about_undefined_strings(self):
         self.assertRaisesRegex(
             AttributeError,
-            "Could not convert constant: TRUE",
+            f"Could not convert constant: TRUE",
             ConfigParser.handle_defined_constants,
             "TRUE",
         )
         self.assertRaisesRegex(
             AttributeError,
-            "Invalid data type BLAH when calculating range.",
+            f"Invalid data type BLAH when calculating range.",
             ConfigParser.handle_defined_constants,
             "MIN",
             "BLAH",
             16,
         )
 
     def test_passes_through_numbers(self):
```

### Comparing `openc3-5.16.0/test/test_json_rpc_response.py` & `openc3-5.9.2b0/test/test_json_rpc_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Copyright 2023 OpenC3, Inc.
 # All Rights Reserved.
 #
 # This program is free software; you can modify and/or redistribute it
 # under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation; version 3 with
 # attribution addendums as found in the LICENSE.txt
```

