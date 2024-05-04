# Comparing `tmp/faststream-0.5.3.tar.gz` & `tmp/faststream-0.5.4.tar.gz`

## Comparing `faststream-0.5.3.tar` & `faststream-0.5.4.tar`

### file list

```diff
@@ -1,322 +1,322 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.5.3/.codespell-whitelist.txt
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 faststream-0.5.3/.secrets.baseline
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.3/.semgrepignore
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.3/CITATION.cff
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.3/SECURITY.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/dependabot.yml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/workflows/check-broken-links-in-docs.yaml
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/workflows/dependency-review.yaml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.3/.github/workflows/update_release_notes.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e01_basic_consume.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e02_1_basic_publisher.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e02_2_basic_publisher.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e02_3_basic_publisher.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e03_miltiple_pubsub.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e04_msg_filter.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e05_rpc_request.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e06_manual_ack.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e07_ack_immediately.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e08_testing.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e09_testing_mocks.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e10_middlewares.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/e11_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/fastapi_integration/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/fastapi_integration/app.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/fastapi_integration/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/howto/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/howto/structlogs.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/kafka/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/kafka/ack_after_process.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/kafka/batch_consume.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/kafka/batch_publish_1.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/kafka/batch_publish_2.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/kafka/batch_publish_3.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/kafka/testing.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/nats/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/nats/e01_basic.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/nats/e02_basic_rpc.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/nats/e03_publisher.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/nats/e04_js_basic.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/nats/e05_basic_and_js.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/nats/e06_key_value.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/nats/e07_object_storage.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/nats/e08_wildcards.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/nats/e09_pull_sub.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/rabbit/__init__.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/rabbit/direct.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/rabbit/header.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/rabbit/stream.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/rabbit/topic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/redis/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/redis/channel_sub.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/redis/channel_sub_pattern.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/redis/list_sub.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/redis/list_sub_batch.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/redis/rpc.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/redis/stream_sub.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/redis/stream_sub_batch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/router/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/router/basic_consume.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/router/basic_publish.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/router/delay_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/serialization/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/serialization/avro/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/serialization/avro/avro.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/serialization/avro/person.avsc
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/serialization/avro/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/serialization/msgpack/__init__.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/serialization/msgpack/pack.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/serialization/msgpack/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/serialization/protobuf/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/serialization/protobuf/message.proto
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/serialization/protobuf/protobuf.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.3/examples/serialization/protobuf/requirements.txt
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/__about__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/__main__.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/_compat.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/annotations.py
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/app.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/constants.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/py.typed
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/security.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/types.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/__init__.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/abc.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/generate.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/message.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/proto.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/site.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/utils.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/channels.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/info.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/main.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/message.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/operations.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/security.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/servers.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/bindings/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/bindings/amqp.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/bindings/kafka.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/bindings/main.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/bindings/nats.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/bindings/redis.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/asyncapi/schema/bindings/sqs.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/__init__.py
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/acknowledgement_watcher.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/message.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/proto.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/router.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/schemas.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/types.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/core/__init__.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/core/abc.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/core/logging.py
--rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/core/usecase.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/fastapi/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/fastapi/context.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/fastapi/get_dependant.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/fastapi/route.py
--rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/fastapi/router.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/middlewares/__init__.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/middlewares/base.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/middlewares/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/publisher/__init__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/publisher/fake.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/publisher/proto.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/subscriber/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/subscriber/call_item.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/subscriber/proto.py
--rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/subscriber/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/wrapper/__init__.py
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/wrapper/call.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/broker/wrapper/proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/__init__.py
--rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/docs/__init__.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/docs/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/supervisors/utils.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/utils/__init__.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/utils/imports.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/utils/logs.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/cli/utils/parser.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/annotations.py
--rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/message.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/parser.py
--rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/security.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/testing.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/broker/__init__.py
--rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/broker/broker.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/broker/logging.py
--rw-r--r--   0        0        0    64951 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/broker/registrator.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/fastapi/__init__.py
--rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/publisher/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/publisher/asyncapi.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/publisher/producer.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/schemas/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/subscriber/__init__.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/confluent/subscriber/usecase.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/annotations.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/message.py
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/parser.py
--rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/security.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/testing.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/broker/__init__.py
--rw-r--r--   0        0        0    28966 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/broker/broker.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/broker/logging.py
--rw-r--r--   0        0        0    71638 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/broker/registrator.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/fastapi/__init__.py
--rw-r--r--   0        0        0   117854 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/publisher/__init__.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/publisher/asyncapi.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/publisher/producer.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/schemas/__init__.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/subscriber/__init__.py
--rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/kafka/subscriber/usecase.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/log/__init__.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/log/formatter.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/log/logging.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/annotations.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/helpers.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/message.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/parser.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/router.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/security.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/testing.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/broker/__init__.py
--rw-r--r--   0        0        0    27053 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/broker/broker.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/broker/logging.py
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/broker/registrator.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/fastapi/__init__.py
--rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/publisher/__init__.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/publisher/asyncapi.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/publisher/producer.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/publisher/usecase.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/schemas/__init__.py
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/schemas/js_stream.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/schemas/pull_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/subscriber/__init__.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/subscriber/asyncapi.py
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/nats/subscriber/usecase.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/__init__.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/annotations.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/message.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/parser.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/router.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/security.py
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/testing.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/types.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/broker/__init__.py
--rw-r--r--   0        0        0    19596 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/broker/broker.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/broker/logging.py
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/broker/registrator.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/fastapi/__init__.py
--rw-r--r--   0        0        0    30283 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/fastapi/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/publisher/__init__.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/publisher/asyncapi.py
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/publisher/producer.py
--rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/publisher/usecase.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/schemas/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/schemas/constants.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/schemas/exchange.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/schemas/proto.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/schemas/queue.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/schemas/reply.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/subscriber/__init__.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/subscriber/asyncapi.py
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/rabbit/subscriber/usecase.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/annotations.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/message.py
--rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/parser.py
--rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/router.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/security.py
--rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/broker/__init__.py
--rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/broker/broker.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/broker/logging.py
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/broker/registrator.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/fastapi/__init__.py
--rw-r--r--   0        0        0    27638 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/publisher/__init__.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/publisher/asyncapi.py
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/publisher/producer.py
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/publisher/usecase.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/schemas/__init__.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/schemas/list_sub.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/schemas/proto.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/schemas/pub_sub.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/schemas/stream_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/subscriber/__init__.py
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/subscriber/asyncapi.py
--rw-r--r--   0        0        0    21352 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/redis/subscriber/usecase.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/testing/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/testing/app.py
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/testing/broker.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/utils/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/utils/ast.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/utils/classes.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/utils/data.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/utils/functions.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/utils/no_cast.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/utils/path.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/utils/context/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/utils/context/builders.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/utils/context/repository.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.3/faststream/utils/context/types.py
--rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/build-docs-pre-commit.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/build-docs.sh
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/lint-pre-commit.sh
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/lint.sh
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/publish.sh
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/serve-docs.sh
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/set_variables.sh
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/start_test_env.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/static-analysis.sh
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/static-pre-commit.sh
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/stop_test_env.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.3/scripts/test.sh
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.3/.gitignore
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.3/LICENSE
--rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.3/README.md
--rw-r--r--   0        0        0    10330 2020-02-02 00:00:00.000000 faststream-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    22988 2020-02-02 00:00:00.000000 faststream-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.5.4/.codespell-whitelist.txt
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 faststream-0.5.4/.secrets.baseline
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.4/.semgrepignore
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.4/CITATION.cff
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.4/SECURITY.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/check-broken-links-in-docs.yaml
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/dependency-review.yaml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/update_release_notes.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e01_basic_consume.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e02_1_basic_publisher.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e02_2_basic_publisher.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e02_3_basic_publisher.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e03_miltiple_pubsub.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e04_msg_filter.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e05_rpc_request.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e06_manual_ack.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e07_ack_immediately.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e08_testing.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e09_testing_mocks.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e10_middlewares.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e11_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/fastapi_integration/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/fastapi_integration/app.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/fastapi_integration/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/howto/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/howto/structlogs.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/ack_after_process.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/batch_consume.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/batch_publish_1.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/batch_publish_2.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/batch_publish_3.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/testing.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/__init__.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e01_basic.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e02_basic_rpc.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e03_publisher.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e04_js_basic.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e05_basic_and_js.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e06_key_value.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e07_object_storage.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e08_wildcards.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e09_pull_sub.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/rabbit/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/rabbit/direct.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/rabbit/header.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/rabbit/stream.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/rabbit/topic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/channel_sub.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/channel_sub_pattern.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/list_sub.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/list_sub_batch.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/rpc.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/stream_sub.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/stream_sub_batch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/router/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/router/basic_consume.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/router/basic_publish.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/router/delay_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/avro/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/avro/avro.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/avro/person.avsc
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/avro/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/msgpack/__init__.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/msgpack/pack.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/msgpack/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/protobuf/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/protobuf/message.proto
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/protobuf/protobuf.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/protobuf/requirements.txt
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/__about__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/__main__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/_compat.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/annotations.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/app.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/constants.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/py.typed
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/security.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/types.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/__init__.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/abc.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/generate.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/message.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/proto.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/site.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/channels.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/info.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/main.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/message.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/operations.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/security.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/servers.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/amqp.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/kafka.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/main.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/nats.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/redis.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/sqs.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/__init__.py
+-rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/acknowledgement_watcher.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/message.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/proto.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/router.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/schemas.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/types.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/core/__init__.py
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/core/abc.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/core/logging.py
+-rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/core/usecase.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/fastapi/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/fastapi/context.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/fastapi/get_dependant.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/fastapi/route.py
+-rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/fastapi/router.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/middlewares/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/middlewares/base.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/middlewares/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/publisher/__init__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/publisher/fake.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/publisher/proto.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/subscriber/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/subscriber/call_item.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/subscriber/proto.py
+-rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/subscriber/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/wrapper/__init__.py
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/wrapper/call.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/wrapper/proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/__init__.py
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/docs/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/docs/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/utils/__init__.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/utils/imports.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/utils/logs.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/utils/parser.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/annotations.py
+-rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/message.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/parser.py
+-rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/security.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/testing.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/broker/__init__.py
+-rw-r--r--   0        0        0    18815 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/broker/broker.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/broker/logging.py
+-rw-r--r--   0        0        0    64951 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/broker/registrator.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/fastapi/__init__.py
+-rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/publisher/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/publisher/producer.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/subscriber/__init__.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/subscriber/usecase.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/annotations.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/message.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/parser.py
+-rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/security.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/testing.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/broker/__init__.py
+-rw-r--r--   0        0        0    28954 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/broker/broker.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/broker/logging.py
+-rw-r--r--   0        0        0    71638 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/broker/registrator.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/fastapi/__init__.py
+-rw-r--r--   0        0        0   117854 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/publisher/__init__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/publisher/producer.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/schemas/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/subscriber/__init__.py
+-rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/subscriber/usecase.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/log/__init__.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/log/formatter.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/log/logging.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/annotations.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/helpers.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/message.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/parser.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/router.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/security.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/testing.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/broker/__init__.py
+-rw-r--r--   0        0        0    27053 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/broker/broker.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/broker/logging.py
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/broker/registrator.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/fastapi/__init__.py
+-rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/publisher/__init__.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/publisher/asyncapi.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/publisher/producer.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/publisher/usecase.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/schemas/__init__.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/schemas/js_stream.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/schemas/pull_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/subscriber/__init__.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/subscriber/usecase.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/__init__.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/annotations.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/message.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/parser.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/router.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/security.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/testing.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/types.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/broker/__init__.py
+-rw-r--r--   0        0        0    19596 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/broker/broker.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/broker/logging.py
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/broker/registrator.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/fastapi/__init__.py
+-rw-r--r--   0        0        0    30283 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/fastapi/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/publisher/__init__.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/publisher/asyncapi.py
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/publisher/producer.py
+-rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/publisher/usecase.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/schemas/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/schemas/constants.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/schemas/exchange.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/schemas/proto.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/schemas/queue.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/schemas/reply.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/subscriber/__init__.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/subscriber/usecase.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/annotations.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/message.py
+-rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/parser.py
+-rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/router.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/security.py
+-rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/broker/__init__.py
+-rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/broker/broker.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/broker/logging.py
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/broker/registrator.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/fastapi/__init__.py
+-rw-r--r--   0        0        0    27638 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/publisher/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/publisher/asyncapi.py
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/publisher/producer.py
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/publisher/usecase.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/schemas/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/schemas/list_sub.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/schemas/proto.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/schemas/pub_sub.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/schemas/stream_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/subscriber/__init__.py
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    21352 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/subscriber/usecase.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/testing/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/testing/app.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/testing/broker.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/ast.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/classes.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/data.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/functions.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/no_cast.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/path.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/context/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/context/builders.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/context/repository.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/context/types.py
+-rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/build-docs-pre-commit.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/lint-pre-commit.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/lint.sh
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/publish.sh
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/serve-docs.sh
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/set_variables.sh
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/start_test_env.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/static-analysis.sh
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/static-pre-commit.sh
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/stop_test_env.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/test.sh
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.4/.gitignore
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.4/LICENSE
+-rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.4/README.md
+-rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 faststream-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0    22991 2020-02-02 00:00:00.000000 faststream-0.5.4/PKG-INFO
```

### Comparing `faststream-0.5.3/.pre-commit-config.yaml` & `faststream-0.5.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.secrets.baseline` & `faststream-0.5.4/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/CITATION.cff` & `faststream-0.5.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/CODE_OF_CONDUCT.md` & `faststream-0.5.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/CONTRIBUTING.md` & `faststream-0.5.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/SECURITY.md` & `faststream-0.5.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.github/PULL_REQUEST_TEMPLATE.md` & `faststream-0.5.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.github/dependabot.yml` & `faststream-0.5.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md` & `faststream-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md` & `faststream-0.5.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.github/workflows/check-broken-links-in-docs.yaml` & `faststream-0.5.4/.github/workflows/check-broken-links-in-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.github/workflows/codeql.yml` & `faststream-0.5.4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.github/workflows/dependency-review.yaml` & `faststream-0.5.4/.github/workflows/dependency-review.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.github/workflows/deploy-docs.yaml` & `faststream-0.5.4/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.github/workflows/publish_coverage.yml` & `faststream-0.5.4/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.github/workflows/publish_pypi.yml` & `faststream-0.5.4/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.github/workflows/test.yaml` & `faststream-0.5.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/.github/workflows/update_release_notes.yaml` & `faststream-0.5.4/.github/workflows/update_release_notes.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/e02_1_basic_publisher.py` & `faststream-0.5.4/examples/e02_1_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/e02_2_basic_publisher.py` & `faststream-0.5.4/examples/e02_2_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/e02_3_basic_publisher.py` & `faststream-0.5.4/examples/e02_3_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/e03_miltiple_pubsub.py` & `faststream-0.5.4/examples/e03_miltiple_pubsub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/e04_msg_filter.py` & `faststream-0.5.4/examples/e04_msg_filter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/e07_ack_immediately.py` & `faststream-0.5.4/examples/e07_ack_immediately.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/e09_testing_mocks.py` & `faststream-0.5.4/examples/e09_testing_mocks.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/e10_middlewares.py` & `faststream-0.5.4/examples/e10_middlewares.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/e11_settings.py` & `faststream-0.5.4/examples/e11_settings.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/fastapi_integration/testing.py` & `faststream-0.5.4/examples/fastapi_integration/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/howto/structlogs.py` & `faststream-0.5.4/examples/howto/structlogs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/kafka/testing.py` & `faststream-0.5.4/examples/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/nats/e03_publisher.py` & `faststream-0.5.4/examples/nats/e03_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/nats/e04_js_basic.py` & `faststream-0.5.4/examples/nats/e04_js_basic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/nats/e05_basic_and_js.py` & `faststream-0.5.4/examples/nats/e05_basic_and_js.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/nats/e06_key_value.py` & `faststream-0.5.4/examples/nats/e06_key_value.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/nats/e07_object_storage.py` & `faststream-0.5.4/examples/nats/e07_object_storage.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/rabbit/direct.py` & `faststream-0.5.4/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/rabbit/fanout.py` & `faststream-0.5.4/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/rabbit/header.py` & `faststream-0.5.4/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/rabbit/topic.py` & `faststream-0.5.4/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/redis/channel_sub_pattern.py` & `faststream-0.5.4/examples/redis/channel_sub_pattern.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/redis/rpc.py` & `faststream-0.5.4/examples/redis/rpc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/router/basic_publish.py` & `faststream-0.5.4/examples/router/basic_publish.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/serialization/avro/avro.py` & `faststream-0.5.4/examples/serialization/avro/avro.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/serialization/msgpack/pack.py` & `faststream-0.5.4/examples/serialization/msgpack/pack.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/examples/serialization/protobuf/protobuf.py` & `faststream-0.5.4/examples/serialization/protobuf/protobuf.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/__init__.py` & `faststream-0.5.4/faststream/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/_compat.py` & `faststream-0.5.4/faststream/_compat.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/app.py` & `faststream-0.5.4/faststream/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/exceptions.py` & `faststream-0.5.4/faststream/exceptions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/security.py` & `faststream-0.5.4/faststream/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/types.py` & `faststream-0.5.4/faststream/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/abc.py` & `faststream-0.5.4/faststream/asyncapi/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/generate.py` & `faststream-0.5.4/faststream/asyncapi/generate.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/message.py` & `faststream-0.5.4/faststream/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/proto.py` & `faststream-0.5.4/faststream/asyncapi/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/site.py` & `faststream-0.5.4/faststream/asyncapi/site.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/utils.py` & `faststream-0.5.4/faststream/asyncapi/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/__init__.py` & `faststream-0.5.4/faststream/asyncapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/channels.py` & `faststream-0.5.4/faststream/asyncapi/schema/channels.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/info.py` & `faststream-0.5.4/faststream/asyncapi/schema/info.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/main.py` & `faststream-0.5.4/faststream/asyncapi/schema/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/message.py` & `faststream-0.5.4/faststream/asyncapi/schema/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/operations.py` & `faststream-0.5.4/faststream/asyncapi/schema/operations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/security.py` & `faststream-0.5.4/faststream/asyncapi/schema/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/servers.py` & `faststream-0.5.4/faststream/asyncapi/schema/servers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/utils.py` & `faststream-0.5.4/faststream/asyncapi/schema/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/bindings/amqp.py` & `faststream-0.5.4/faststream/asyncapi/schema/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/bindings/kafka.py` & `faststream-0.5.4/faststream/asyncapi/schema/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/bindings/main.py` & `faststream-0.5.4/faststream/asyncapi/schema/bindings/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/bindings/nats.py` & `faststream-0.5.4/faststream/asyncapi/schema/bindings/nats.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/bindings/redis.py` & `faststream-0.5.4/faststream/asyncapi/schema/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/asyncapi/schema/bindings/sqs.py` & `faststream-0.5.4/faststream/asyncapi/schema/bindings/sqs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/acknowledgement_watcher.py` & `faststream-0.5.4/faststream/broker/acknowledgement_watcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -122,19 +122,21 @@
 class WatcherContext:
     """A class representing a context for a watcher."""
 
     def __init__(
         self,
         message: "StreamMessage[MsgType]",
         watcher: BaseWatcher,
+        logger: Optional["LoggerProto"] = None,
         **extra_options: Any,
     ) -> None:
         self.watcher = watcher
         self.message = message
         self.extra_options = extra_options
+        self.logger = logger
 
     async def __aenter__(self) -> None:
         self.watcher.add(self.message.message_id)
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
@@ -168,23 +170,49 @@
 
         else:
             await self.__nack()
 
         return not is_test_env()
 
     async def __ack(self) -> None:
-        await self.message.ack(**self.extra_options)
-        self.watcher.remove(self.message.message_id)
+        try:
+            await self.message.ack(**self.extra_options)
+        except Exception as er:
+            if self.logger is not None:
+                self.logger.log(
+                    logging.ERROR,
+                    er,
+                    exc_info=er
+                )
+        else:
+            self.watcher.remove(self.message.message_id)
 
     async def __nack(self) -> None:
-        await self.message.nack(**self.extra_options)
+        try:
+            await self.message.nack(**self.extra_options)
+        except Exception as er:
+            if self.logger is not None:
+                self.logger.log(
+                    logging.ERROR,
+                    er,
+                    exc_info=er
+                )
 
     async def __reject(self) -> None:
-        await self.message.reject(**self.extra_options)
-        self.watcher.remove(self.message.message_id)
+        try:
+            await self.message.reject(**self.extra_options)
+        except Exception as er:
+            if self.logger is not None:
+                self.logger.log(
+                    logging.ERROR,
+                    er,
+                    exc_info=er
+                )
+        else:
+            self.watcher.remove(self.message.message_id)
 
 
 def get_watcher(
     logger: Optional["LoggerProto"],
     try_number: Union[bool, int],
 ) -> BaseWatcher:
     """Get a watcher object based on the provided parameters.
```

### Comparing `faststream-0.5.3/faststream/broker/message.py` & `faststream-0.5.4/faststream/broker/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/router.py` & `faststream-0.5.4/faststream/broker/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/schemas.py` & `faststream-0.5.4/faststream/broker/schemas.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/types.py` & `faststream-0.5.4/faststream/broker/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/utils.py` & `faststream-0.5.4/faststream/broker/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     if no_ack:
         return fake_context
 
     else:
         return partial(
             WatcherContext,
             watcher=get_watcher(logger, retry),
+            logger=logger,
             **extra_options,
         )
 
 
 class MultiLock:
     """A class representing a multi lock."""
```

### Comparing `faststream-0.5.3/faststream/broker/core/abc.py` & `faststream-0.5.4/faststream/broker/core/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/core/logging.py` & `faststream-0.5.4/faststream/broker/core/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/core/usecase.py` & `faststream-0.5.4/faststream/broker/core/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/fastapi/context.py` & `faststream-0.5.4/faststream/broker/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/fastapi/get_dependant.py` & `faststream-0.5.4/faststream/broker/fastapi/get_dependant.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/fastapi/route.py` & `faststream-0.5.4/faststream/broker/fastapi/route.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/fastapi/router.py` & `faststream-0.5.4/faststream/broker/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/middlewares/base.py` & `faststream-0.5.4/faststream/broker/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/middlewares/logging.py` & `faststream-0.5.4/faststream/broker/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/publisher/fake.py` & `faststream-0.5.4/faststream/broker/publisher/fake.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/publisher/proto.py` & `faststream-0.5.4/faststream/broker/publisher/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/publisher/usecase.py` & `faststream-0.5.4/faststream/broker/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/subscriber/call_item.py` & `faststream-0.5.4/faststream/broker/subscriber/call_item.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/subscriber/proto.py` & `faststream-0.5.4/faststream/broker/subscriber/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/subscriber/usecase.py` & `faststream-0.5.4/faststream/broker/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/broker/wrapper/call.py` & `faststream-0.5.4/faststream/broker/wrapper/call.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-from functools import wraps
 from typing import (
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     Generic,
     Iterable,
@@ -182,21 +181,17 @@
         self._wrapped_call = f
         return dependent
 
 
 def _wrap_decode_message(
     func: Callable[..., Awaitable[T_HandlerReturn]],
     params_ln: int,
-) -> Callable[
-    ["StreamMessage[MsgType]"],
-    Awaitable[T_HandlerReturn],
-]:
+) -> Callable[["StreamMessage[MsgType]"], Awaitable[T_HandlerReturn]]:
     """Wraps a function to decode a message and pass it as an argument to the wrapped function."""
 
-    @wraps(func)
     async def decode_wrapper(message: "StreamMessage[MsgType]") -> T_HandlerReturn:
         """A wrapper function to decode and handle a message."""
         msg = message.decoded_body
 
         if params_ln > 1:
             if isinstance(msg, Mapping):
                 return await func(**msg)
```

### Comparing `faststream-0.5.3/faststream/broker/wrapper/proto.py` & `faststream-0.5.4/faststream/broker/wrapper/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/cli/main.py` & `faststream-0.5.4/faststream/cli/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/cli/docs/app.py` & `faststream-0.5.4/faststream/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/cli/supervisors/basereload.py` & `faststream-0.5.4/faststream/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/cli/supervisors/multiprocess.py` & `faststream-0.5.4/faststream/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/cli/supervisors/utils.py` & `faststream-0.5.4/faststream/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/cli/supervisors/watchfiles.py` & `faststream-0.5.4/faststream/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/cli/utils/imports.py` & `faststream-0.5.4/faststream/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/cli/utils/logs.py` & `faststream-0.5.4/faststream/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/cli/utils/parser.py` & `faststream-0.5.4/faststream/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/annotations.py` & `faststream-0.5.4/faststream/confluent/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/client.py` & `faststream-0.5.4/faststream/confluent/client.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/message.py` & `faststream-0.5.4/faststream/confluent/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/parser.py` & `faststream-0.5.4/faststream/confluent/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/router.py` & `faststream-0.5.4/faststream/confluent/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/security.py` & `faststream-0.5.4/faststream/confluent/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/testing.py` & `faststream-0.5.4/faststream/confluent/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/broker/broker.py` & `faststream-0.5.4/faststream/confluent/broker/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,23 +435,26 @@
     async def _connect(  # type: ignore[override]
         self,
         *,
         client_id: str,
         **kwargs: Any,
     ) -> ConsumerConnectionParams:
         security_params = parse_security(self.security)
+        kwargs.update(security_params)
+
         producer = AsyncConfluentProducer(
             **kwargs,
-            **security_params,
             client_id=client_id,
         )
+
         self._producer = AsyncConfluentFastProducer(
             producer=producer,
         )
-        return filter_by_dict(ConsumerConnectionParams, {**kwargs, **security_params})
+
+        return filter_by_dict(ConsumerConnectionParams, kwargs)
 
     async def start(self) -> None:
         await super().start()
 
         for handler in self._subscribers.values():
             self._log(
                 f"`{handler.call_name}` waiting for messages",
```

### Comparing `faststream-0.5.3/faststream/confluent/broker/logging.py` & `faststream-0.5.4/faststream/confluent/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/broker/registrator.py` & `faststream-0.5.4/faststream/confluent/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/fastapi/__init__.py` & `faststream-0.5.4/faststream/confluent/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/fastapi/fastapi.py` & `faststream-0.5.4/faststream/confluent/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/publisher/asyncapi.py` & `faststream-0.5.4/faststream/confluent/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/publisher/producer.py` & `faststream-0.5.4/faststream/confluent/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/publisher/usecase.py` & `faststream-0.5.4/faststream/confluent/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/schemas/params.py` & `faststream-0.5.4/faststream/confluent/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/subscriber/asyncapi.py` & `faststream-0.5.4/faststream/confluent/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/confluent/subscriber/usecase.py` & `faststream-0.5.4/faststream/confluent/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/annotations.py` & `faststream-0.5.4/faststream/kafka/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/message.py` & `faststream-0.5.4/faststream/kafka/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/parser.py` & `faststream-0.5.4/faststream/kafka/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/router.py` & `faststream-0.5.4/faststream/kafka/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/security.py` & `faststream-0.5.4/faststream/kafka/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/testing.py` & `faststream-0.5.4/faststream/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/broker/broker.py` & `faststream-0.5.4/faststream/kafka/broker/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,24 +577,27 @@
     async def _connect(  # type: ignore[override]
         self,
         *,
         client_id: str,
         **kwargs: Any,
     ) -> ConsumerConnectionParams:
         security_params = parse_security(self.security)
+        kwargs.update(security_params)
+
         producer = aiokafka.AIOKafkaProducer(
             **kwargs,
-            **security_params,
             client_id=client_id,
         )
+
         await producer.start()
         self._producer = AioKafkaFastProducer(
             producer=producer,
         )
-        return filter_by_dict(ConsumerConnectionParams, {**kwargs, **security_params})
+
+        return filter_by_dict(ConsumerConnectionParams, kwargs)
 
     async def start(self) -> None:
         """Connect broker to Kafka and startup all subscribers."""
         await super().start()
 
         for handler in self._subscribers.values():
             self._log(
```

### Comparing `faststream-0.5.3/faststream/kafka/broker/logging.py` & `faststream-0.5.4/faststream/kafka/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/broker/registrator.py` & `faststream-0.5.4/faststream/kafka/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/fastapi/__init__.py` & `faststream-0.5.4/faststream/kafka/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/fastapi/fastapi.py` & `faststream-0.5.4/faststream/kafka/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/publisher/asyncapi.py` & `faststream-0.5.4/faststream/kafka/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/publisher/producer.py` & `faststream-0.5.4/faststream/kafka/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/publisher/usecase.py` & `faststream-0.5.4/faststream/kafka/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/schemas/params.py` & `faststream-0.5.4/faststream/kafka/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/subscriber/asyncapi.py` & `faststream-0.5.4/faststream/kafka/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/kafka/subscriber/usecase.py` & `faststream-0.5.4/faststream/kafka/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/log/formatter.py` & `faststream-0.5.4/faststream/log/formatter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/log/logging.py` & `faststream-0.5.4/faststream/log/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/__init__.py` & `faststream-0.5.4/faststream/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/annotations.py` & `faststream-0.5.4/faststream/nats/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/helpers.py` & `faststream-0.5.4/faststream/nats/helpers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/message.py` & `faststream-0.5.4/faststream/nats/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/parser.py` & `faststream-0.5.4/faststream/nats/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/router.py` & `faststream-0.5.4/faststream/nats/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/security.py` & `faststream-0.5.4/faststream/nats/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/testing.py` & `faststream-0.5.4/faststream/nats/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from nats.aio.msg import Msg
 from typing_extensions import override
 
 from faststream.broker.message import encode_message, gen_cor_id
+from faststream.exceptions import WRONG_PUBLISH_ARGS
 from faststream.nats.broker import NatsBroker
 from faststream.nats.publisher.producer import NatsFastProducer
 from faststream.nats.schemas.js_stream import is_subject_match_wildcard
 from faststream.nats.subscriber.asyncapi import AsyncAPISubscriber
 from faststream.testing.broker import TestBroker, call_handler
 
 if TYPE_CHECKING:
@@ -67,14 +68,17 @@
         timeout: Optional[float] = None,
         stream: Optional[str] = None,
         *,
         rpc: bool = False,
         rpc_timeout: Optional[float] = None,
         raise_timeout: bool = False,
     ) -> Any:
+        if rpc and reply_to:
+            raise WRONG_PUBLISH_ARGS
+
         incoming = build_message(
             message=message,
             subject=subject,
             headers=headers,
             correlation_id=correlation_id,
             reply_to=reply_to,
         )
```

### Comparing `faststream-0.5.3/faststream/nats/broker/broker.py` & `faststream-0.5.4/faststream/nats/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/broker/logging.py` & `faststream-0.5.4/faststream/nats/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/broker/registrator.py` & `faststream-0.5.4/faststream/nats/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/fastapi/__init__.py` & `faststream-0.5.4/faststream/nats/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/fastapi/fastapi.py` & `faststream-0.5.4/faststream/nats/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/publisher/asyncapi.py` & `faststream-0.5.4/faststream/nats/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/publisher/producer.py` & `faststream-0.5.4/faststream/nats/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/publisher/usecase.py` & `faststream-0.5.4/faststream/nats/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/schemas/js_stream.py` & `faststream-0.5.4/faststream/nats/schemas/js_stream.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/schemas/pull_sub.py` & `faststream-0.5.4/faststream/nats/schemas/pull_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/subscriber/asyncapi.py` & `faststream-0.5.4/faststream/nats/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/nats/subscriber/usecase.py` & `faststream-0.5.4/faststream/nats/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/__init__.py` & `faststream-0.5.4/faststream/rabbit/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/annotations.py` & `faststream-0.5.4/faststream/rabbit/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/message.py` & `faststream-0.5.4/faststream/rabbit/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/parser.py` & `faststream-0.5.4/faststream/rabbit/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/router.py` & `faststream-0.5.4/faststream/rabbit/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/security.py` & `faststream-0.5.4/faststream/rabbit/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/testing.py` & `faststream-0.5.4/faststream/rabbit/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import aiormq
 from aio_pika.message import IncomingMessage
 from pamqp import commands as spec
 from pamqp.header import ContentHeader
 from typing_extensions import override
 
 from faststream.broker.message import gen_cor_id
+from faststream.exceptions import WRONG_PUBLISH_ARGS
 from faststream.rabbit.broker.broker import RabbitBroker
 from faststream.rabbit.parser import AioPikaParser
 from faststream.rabbit.publisher.asyncapi import AsyncAPIPublisher
 from faststream.rabbit.publisher.producer import AioPikaFastProducer
 from faststream.rabbit.schemas import (
     ExchangeType,
     RabbitExchange,
@@ -193,14 +194,17 @@
         message_type: Optional[str] = None,
         user_id: Optional[str] = None,
         app_id: Optional[str] = None,
     ) -> Optional[Any]:
         """Publish a message to a RabbitMQ queue or exchange."""
         exch = RabbitExchange.validate(exchange)
 
+        if rpc and reply_to:
+            raise WRONG_PUBLISH_ARGS
+
         incoming = build_message(
             message=message,
             exchange=exch,
             routing_key=routing_key,
             reply_to=reply_to,
             app_id=app_id,
             user_id=user_id,
```

### Comparing `faststream-0.5.3/faststream/rabbit/utils.py` & `faststream-0.5.4/faststream/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/broker/broker.py` & `faststream-0.5.4/faststream/rabbit/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/broker/logging.py` & `faststream-0.5.4/faststream/rabbit/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/broker/registrator.py` & `faststream-0.5.4/faststream/rabbit/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/fastapi/__init__.py` & `faststream-0.5.4/faststream/rabbit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/fastapi/router.py` & `faststream-0.5.4/faststream/rabbit/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/publisher/asyncapi.py` & `faststream-0.5.4/faststream/rabbit/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/publisher/producer.py` & `faststream-0.5.4/faststream/rabbit/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/publisher/usecase.py` & `faststream-0.5.4/faststream/rabbit/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/schemas/constants.py` & `faststream-0.5.4/faststream/rabbit/schemas/constants.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/schemas/exchange.py` & `faststream-0.5.4/faststream/rabbit/schemas/exchange.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/schemas/queue.py` & `faststream-0.5.4/faststream/rabbit/schemas/queue.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/schemas/reply.py` & `faststream-0.5.4/faststream/rabbit/schemas/reply.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/subscriber/asyncapi.py` & `faststream-0.5.4/faststream/rabbit/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/rabbit/subscriber/usecase.py` & `faststream-0.5.4/faststream/rabbit/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/__init__.py` & `faststream-0.5.4/faststream/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/annotations.py` & `faststream-0.5.4/faststream/redis/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/message.py` & `faststream-0.5.4/faststream/redis/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/parser.py` & `faststream-0.5.4/faststream/redis/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/router.py` & `faststream-0.5.4/faststream/redis/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/security.py` & `faststream-0.5.4/faststream/redis/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/testing.py` & `faststream-0.5.4/faststream/redis/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from typing import TYPE_CHECKING, Any, Optional, Sequence, Union
 
 from typing_extensions import override
 
 from faststream.broker.message import gen_cor_id
-from faststream.exceptions import SetupError
+from faststream.exceptions import WRONG_PUBLISH_ARGS, SetupError
 from faststream.redis.broker.broker import RedisBroker
 from faststream.redis.message import (
     BatchListMessage,
     BatchStreamMessage,
     DefaultListMessage,
     DefaultStreamMessage,
     PubSubMessage,
@@ -83,14 +83,17 @@
         headers: Optional["AnyDict"] = None,
         reply_to: str = "",
         correlation_id: Optional[str] = None,
         rpc: bool = False,
         rpc_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
     ) -> Optional[Any]:
+        if rpc and reply_to:
+            raise WRONG_PUBLISH_ARGS
+
         correlation_id = correlation_id or gen_cor_id()
 
         body = build_message(
             message=message,
             reply_to=reply_to,
             correlation_id=correlation_id,
             headers=headers,
```

### Comparing `faststream-0.5.3/faststream/redis/broker/broker.py` & `faststream-0.5.4/faststream/redis/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/broker/logging.py` & `faststream-0.5.4/faststream/redis/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/broker/registrator.py` & `faststream-0.5.4/faststream/redis/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/fastapi/__init__.py` & `faststream-0.5.4/faststream/redis/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/fastapi/fastapi.py` & `faststream-0.5.4/faststream/redis/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/publisher/asyncapi.py` & `faststream-0.5.4/faststream/redis/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/publisher/producer.py` & `faststream-0.5.4/faststream/redis/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/publisher/usecase.py` & `faststream-0.5.4/faststream/redis/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/schemas/list_sub.py` & `faststream-0.5.4/faststream/redis/schemas/list_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/schemas/proto.py` & `faststream-0.5.4/faststream/redis/schemas/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/schemas/pub_sub.py` & `faststream-0.5.4/faststream/redis/schemas/pub_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/schemas/stream_sub.py` & `faststream-0.5.4/faststream/redis/schemas/stream_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/subscriber/asyncapi.py` & `faststream-0.5.4/faststream/redis/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/redis/subscriber/usecase.py` & `faststream-0.5.4/faststream/redis/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/testing/app.py` & `faststream-0.5.4/faststream/testing/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/testing/broker.py` & `faststream-0.5.4/faststream/testing/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/utils/ast.py` & `faststream-0.5.4/faststream/utils/ast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/utils/classes.py` & `faststream-0.5.4/faststream/utils/classes.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/utils/data.py` & `faststream-0.5.4/faststream/utils/data.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/utils/functions.py` & `faststream-0.5.4/faststream/utils/functions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/utils/no_cast.py` & `faststream-0.5.4/faststream/utils/no_cast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/utils/path.py` & `faststream-0.5.4/faststream/utils/path.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/utils/context/builders.py` & `faststream-0.5.4/faststream/utils/context/builders.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/utils/context/repository.py` & `faststream-0.5.4/faststream/utils/context/repository.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/faststream/utils/context/types.py` & `faststream-0.5.4/faststream/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/scripts/build-docs-pre-commit.sh` & `faststream-0.5.4/scripts/build-docs-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/scripts/lint-pre-commit.sh` & `faststream-0.5.4/scripts/lint-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/scripts/set_variables.sh` & `faststream-0.5.4/scripts/set_variables.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/scripts/static-pre-commit.sh` & `faststream-0.5.4/scripts/static-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/LICENSE` & `faststream-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/README.md` & `faststream-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.3/pyproject.toml` & `faststream-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -74,51 +74,51 @@
 redis = ["redis>=5.0.0,<6.0.0"]
 
 # dev dependencies
 devdocs = [
     "mkdocs-material==9.5.18",
     "mkdocs-static-i18n==1.2.2",
     "mdx-include==1.4.2",
-    "mkdocstrings[python]==0.24.3",
+    "mkdocstrings[python]==0.25.0",
     "mkdocs-literate-nav==0.6.1",
     "mkdocs-git-revision-date-localized-plugin==1.2.4",
     "mike==2.0.0",                                      # versioning
     "mkdocs-minify-plugin==0.8.0",
     "mkdocs-macros-plugin==1.0.5",                      # includes with variables
     "mkdocs-glightbox==0.3.7",                          # img zoom
     "pillow",                                           # required for mkdocs-glightbo
     "cairosvg",                                         # required for mkdocs-glightbo
     "requests",                                         # using in CI, do not pin it
     "griffe-typingdoc==0.2.5",                          # Annotated[..., Doc("")] support
 ]
 
 types = [
     "faststream[rabbit,confluent,kafka,nats,redis]",
-    "mypy==1.9.0",
+    "mypy==1.10.0",
     # mypy extensions
     "types-PyYAML",
     "types-setuptools",
     "types-ujson",
     "types-redis",
     "types-Pygments",
     "types-docutils",
     "confluent-kafka-stubs; python_version >= '3.11'",
 ]
 
 lint = [
     "faststream[types]",
-    "ruff==0.4.1",
+    "ruff==0.4.2",
     "bandit==1.7.8",
-    "semgrep==1.69.0",
+    "semgrep==1.70.0",
     "codespell==2.2.6",
 ]
 
 test-core = [
     "coverage[toml]==7.4.4",
-    "pytest==8.1.1",
+    "pytest==8.2.0",
     "pytest-asyncio==0.23.6",
     "dirty-equals==0.7.1.post0",
 ]
 
 testing = [
     "faststream[test-core]",
     "fastapi==0.110.2",
```

### Comparing `faststream-0.5.3/PKG-INFO` & `faststream-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faststream
-Version: 0.5.3
+Version: 0.5.4
 Summary: FastStream: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://faststream.airt.ai/latest/
 Project-URL: Documentation, https://faststream.airt.ai/latest/getting-started/
 Project-URL: Tracker, https://github.com/airtai/FastStream/issues
 Project-URL: Source, https://github.com/airtai/FastStream
 Project-URL: Discord, https://discord.gg/qFm6aSqq59
 Author-email: airt <info@airt.ai>, Nikita Pastukhov <nikita@pastukhov-dev.ru>
@@ -64,28 +64,28 @@
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.4; extra == 'dev'
 Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'dev'
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'dev'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'dev'
 Requires-Dist: mkdocs-material==9.5.18; extra == 'dev'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'dev'
 Requires-Dist: mkdocs-static-i18n==1.2.2; extra == 'dev'
-Requires-Dist: mkdocstrings[python]==0.24.3; extra == 'dev'
-Requires-Dist: mypy==1.9.0; extra == 'dev'
+Requires-Dist: mkdocstrings[python]==0.25.0; extra == 'dev'
+Requires-Dist: mypy==1.10.0; extra == 'dev'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'dev'
 Requires-Dist: pillow; extra == 'dev'
 Requires-Dist: pre-commit==3.5.0; (python_version < '3.9') and extra == 'dev'
 Requires-Dist: pre-commit==3.7.0; (python_version >= '3.9') and extra == 'dev'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'dev'
 Requires-Dist: pytest-asyncio==0.23.6; extra == 'dev'
-Requires-Dist: pytest==8.1.1; extra == 'dev'
+Requires-Dist: pytest==8.2.0; extra == 'dev'
 Requires-Dist: pyyaml==6.0.1; extra == 'dev'
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'dev'
 Requires-Dist: requests; extra == 'dev'
-Requires-Dist: ruff==0.4.1; extra == 'dev'
-Requires-Dist: semgrep==1.69.0; extra == 'dev'
+Requires-Dist: ruff==0.4.2; extra == 'dev'
+Requires-Dist: semgrep==1.70.0; extra == 'dev'
 Requires-Dist: types-docutils; extra == 'dev'
 Requires-Dist: types-pygments; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Requires-Dist: types-redis; extra == 'dev'
 Requires-Dist: types-setuptools; extra == 'dev'
 Requires-Dist: types-ujson; extra == 'dev'
 Requires-Dist: watchfiles==0.21.0; extra == 'dev'
@@ -97,31 +97,31 @@
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.4; extra == 'devdocs'
 Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'devdocs'
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'devdocs'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'devdocs'
 Requires-Dist: mkdocs-material==9.5.18; extra == 'devdocs'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'devdocs'
 Requires-Dist: mkdocs-static-i18n==1.2.2; extra == 'devdocs'
-Requires-Dist: mkdocstrings[python]==0.24.3; extra == 'devdocs'
+Requires-Dist: mkdocstrings[python]==0.25.0; extra == 'devdocs'
 Requires-Dist: pillow; extra == 'devdocs'
 Requires-Dist: requests; extra == 'devdocs'
 Provides-Extra: kafka
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'kafka'
 Provides-Extra: lint
 Requires-Dist: aio-pika<10,>=9; extra == 'lint'
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'lint'
 Requires-Dist: bandit==1.7.8; extra == 'lint'
 Requires-Dist: codespell==2.2.6; extra == 'lint'
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'lint'
 Requires-Dist: confluent-kafka<3,>=2; extra == 'lint'
-Requires-Dist: mypy==1.9.0; extra == 'lint'
+Requires-Dist: mypy==1.10.0; extra == 'lint'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'lint'
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'lint'
-Requires-Dist: ruff==0.4.1; extra == 'lint'
-Requires-Dist: semgrep==1.69.0; extra == 'lint'
+Requires-Dist: ruff==0.4.2; extra == 'lint'
+Requires-Dist: semgrep==1.70.0; extra == 'lint'
 Requires-Dist: types-docutils; extra == 'lint'
 Requires-Dist: types-pygments; extra == 'lint'
 Requires-Dist: types-pyyaml; extra == 'lint'
 Requires-Dist: types-redis; extra == 'lint'
 Requires-Dist: types-setuptools; extra == 'lint'
 Requires-Dist: types-ujson; extra == 'lint'
 Provides-Extra: nats
@@ -130,32 +130,32 @@
 Requires-Dist: aio-pika<10,>=9; extra == 'rabbit'
 Provides-Extra: redis
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'redis'
 Provides-Extra: test-core
 Requires-Dist: coverage[toml]==7.4.4; extra == 'test-core'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'test-core'
 Requires-Dist: pytest-asyncio==0.23.6; extra == 'test-core'
-Requires-Dist: pytest==8.1.1; extra == 'test-core'
+Requires-Dist: pytest==8.2.0; extra == 'test-core'
 Provides-Extra: testing
 Requires-Dist: coverage[toml]==7.4.4; extra == 'testing'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'testing'
 Requires-Dist: email-validator==2.1.1; extra == 'testing'
 Requires-Dist: fastapi==0.110.2; extra == 'testing'
 Requires-Dist: httpx==0.27.0; extra == 'testing'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'testing'
 Requires-Dist: pytest-asyncio==0.23.6; extra == 'testing'
-Requires-Dist: pytest==8.1.1; extra == 'testing'
+Requires-Dist: pytest==8.2.0; extra == 'testing'
 Requires-Dist: pyyaml==6.0.1; extra == 'testing'
 Requires-Dist: watchfiles==0.21.0; extra == 'testing'
 Provides-Extra: types
 Requires-Dist: aio-pika<10,>=9; extra == 'types'
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'types'
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'types'
 Requires-Dist: confluent-kafka<3,>=2; extra == 'types'
-Requires-Dist: mypy==1.9.0; extra == 'types'
+Requires-Dist: mypy==1.10.0; extra == 'types'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'types'
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'types'
 Requires-Dist: types-docutils; extra == 'types'
 Requires-Dist: types-pygments; extra == 'types'
 Requires-Dist: types-pyyaml; extra == 'types'
 Requires-Dist: types-redis; extra == 'types'
 Requires-Dist: types-setuptools; extra == 'types'
```

