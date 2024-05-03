# Comparing `tmp/highlight_io-0.7.0.tar.gz` & `tmp/highlight_io-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlight_io-0.7.0.tar", max compression
+gzip compressed data, was "highlight_io-0.7.1.tar", max compression
```

## Comparing `highlight_io-0.7.0.tar` & `highlight_io-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1340 2024-04-16 19:50:41.352277 highlight_io-0.7.0/README.md
--rw-r--r--   0        0        0       64 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/__init__.py
--rw-r--r--   0        0        0      155 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/__init__.py
--rw-r--r--   0        0        0      717 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/aws.py
--rw-r--r--   0        0        0      740 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/azure.py
--rw-r--r--   0        0        0      516 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/boto.py
--rw-r--r--   0        0        0      541 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/boto3sqs.py
--rw-r--r--   0        0        0      530 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/celery.py
--rw-r--r--   0        0        0     1911 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/django.py
--rw-r--r--   0        0        0     2224 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/fastapi.py
--rw-r--r--   0        0        0     1688 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/flask.py
--rw-r--r--   0        0        0      747 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/gcp.py
--rw-r--r--   0        0        0      523 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/redis.py
--rw-r--r--   0        0        0      544 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/requests.py
--rw-r--r--   0        0        0     1072 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/serverless.py
--rw-r--r--   0        0        0      558 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/sqlalchemy.py
--rw-r--r--   0        0        0    19222 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/sdk.py
--rw-r--r--   0        0        0        0 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/utils/__init__.py
--rw-r--r--   0        0        0     1150 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/utils/lru_cache.py
--rw-r--r--   0        0        0     2674 2024-04-16 19:50:41.356277 highlight_io-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3903 1970-01-01 00:00:00.000000 highlight_io-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1340 2024-05-03 18:24:06.970538 highlight_io-0.7.1/README.md
+-rw-r--r--   0        0        0       80 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/__init__.py
+-rw-r--r--   0        0        0      155 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/__init__.py
+-rw-r--r--   0        0        0      717 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/aws.py
+-rw-r--r--   0        0        0      740 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/azure.py
+-rw-r--r--   0        0        0      516 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/boto.py
+-rw-r--r--   0        0        0      541 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/boto3sqs.py
+-rw-r--r--   0        0        0      530 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/celery.py
+-rw-r--r--   0        0        0     1911 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/django.py
+-rw-r--r--   0        0        0     2224 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/fastapi.py
+-rw-r--r--   0        0        0     1688 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/flask.py
+-rw-r--r--   0        0        0      747 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/gcp.py
+-rw-r--r--   0        0        0      523 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/redis.py
+-rw-r--r--   0        0        0      544 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/requests.py
+-rw-r--r--   0        0        0     1072 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/serverless.py
+-rw-r--r--   0        0        0      558 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/integrations/sqlalchemy.py
+-rw-r--r--   0        0        0    19416 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/sdk.py
+-rw-r--r--   0        0        0        0 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/utils/__init__.py
+-rw-r--r--   0        0        0     1150 2024-05-03 18:24:06.970538 highlight_io-0.7.1/highlight_io/utils/lru_cache.py
+-rw-r--r--   0        0        0     2674 2024-05-03 18:24:06.970538 highlight_io-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3903 1970-01-01 00:00:00.000000 highlight_io-0.7.1/PKG-INFO
```

### Comparing `highlight_io-0.7.0/README.md` & `highlight_io-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/aws.py` & `highlight_io-0.7.1/highlight_io/integrations/aws.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/azure.py` & `highlight_io-0.7.1/highlight_io/integrations/azure.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/boto.py` & `highlight_io-0.7.1/highlight_io/integrations/boto.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/boto3sqs.py` & `highlight_io-0.7.1/highlight_io/integrations/boto3sqs.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/celery.py` & `highlight_io-0.7.1/highlight_io/integrations/celery.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/django.py` & `highlight_io-0.7.1/highlight_io/integrations/django.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/fastapi.py` & `highlight_io-0.7.1/highlight_io/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/flask.py` & `highlight_io-0.7.1/highlight_io/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/gcp.py` & `highlight_io-0.7.1/highlight_io/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/redis.py` & `highlight_io-0.7.1/highlight_io/integrations/redis.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/requests.py` & `highlight_io-0.7.1/highlight_io/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/serverless.py` & `highlight_io-0.7.1/highlight_io/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/integrations/sqlalchemy.py` & `highlight_io-0.7.1/highlight_io/integrations/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/highlight_io/sdk.py` & `highlight_io-0.7.1/highlight_io/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 import http
 import json
 import logging
 import sys
 import traceback
 import typing
 
-from opentelemetry import trace, _logs
+from highlight_io.integrations import Integration
+from highlight_io.integrations.boto import BotoIntegration
+from highlight_io.integrations.boto3sqs import Boto3SQSIntegration
+from highlight_io.integrations.celery import CeleryIntegration
+from highlight_io.integrations.redis import RedisIntegration
+from highlight_io.integrations.requests import RequestsIntegration
+from highlight_io.integrations.sqlalchemy import SQLAlchemyIntegration
+from highlight_io.utils.lru_cache import LRUCache
+from opentelemetry import trace as otel_trace, _logs
 from opentelemetry._logs.severity import std_to_otel
 from opentelemetry.baggage import set_baggage, get_baggage
 from opentelemetry.context import Context, attach
 from opentelemetry.exporter.otlp.proto.http import Compression
 from opentelemetry.exporter.otlp.proto.http._log_exporter import OTLPLogExporter
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
@@ -22,23 +30,14 @@
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider, Span, SpanProcessor
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.semconv.resource import ResourceAttributes
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import INVALID_SPAN
 
-from highlight_io.integrations import Integration
-from highlight_io.integrations.boto import BotoIntegration
-from highlight_io.integrations.boto3sqs import Boto3SQSIntegration
-from highlight_io.integrations.celery import CeleryIntegration
-from highlight_io.integrations.redis import RedisIntegration
-from highlight_io.integrations.requests import RequestsIntegration
-from highlight_io.integrations.sqlalchemy import SQLAlchemyIntegration
-from highlight_io.utils.lru_cache import LRUCache
-
 DEFAULT_INTEGRATIONS = [
     BotoIntegration,
     Boto3SQSIntegration,
     CeleryIntegration,
     RedisIntegration,
     RequestsIntegration,
     SQLAlchemyIntegration,
@@ -63,23 +62,23 @@
             lg.warning("oh, no!")
         """
         self.highlight = highlight
         super(LogHandler, self).__init__(level=level)
 
     def emit(self, record: logging.LogRecord):
         ctx = contextlib.nullcontext
-        span = trace.get_current_span()
+        span = otel_trace.get_current_span()
 
         if span is None or not span.is_recording():
             ctx = self.highlight.trace
 
         with ctx():
             if self.filter(record):
                 self.highlight.log_hook(
-                    trace.get_current_span(), record, formatted=self.format(record)
+                    otel_trace.get_current_span(), record, formatted=self.format(record)
                 )
 
 
 class H(object):
     REQUEST_HEADER = "X-Highlight-Request"
     OTLP_HTTP = "https://otel.highlight.io:4318"
     _instance: "H" = None
@@ -210,16 +209,16 @@
             BatchSpanProcessor(
                 OTLPSpanExporter(
                     f"{self._otlp_endpoint}/v1/traces", compression=Compression.Gzip
                 ),
                 **kwargs,
             )
         )
-        trace.set_tracer_provider(self._trace_provider)
-        self.tracer = trace.get_tracer(__name__)
+        otel_trace.set_tracer_provider(self._trace_provider)
+        self.tracer = otel_trace.get_tracer(__name__)
 
         self._log_provider = LoggerProvider(
             resource=resource,
         )
         self._log_provider.add_log_record_processor(
             BatchLogRecordProcessor(
                 OTLPLogExporter(
@@ -323,15 +322,15 @@
 
 
         :param status_code: the http status code to report
         :param detail: the error status details
         :param attributes: additional metadata to attribute to this error.
         :return: None
         """
-        span = trace.get_current_span()
+        span = otel_trace.get_current_span()
         if not span:
             raise RuntimeError("H.record_http_error called without a span context")
 
         # try load json of the form `{"detail":"Item not found"}`
         try:
             body = json.loads(detail)
             if "detail" in body:
@@ -383,15 +382,15 @@
                     H.record_exception(e)
 
 
         :param e: the exception to record. the contents and stacktrace will be recorded.
         :param attributes: additional metadata to attribute to this error.
         :return: None
         """
-        span = trace.get_current_span()
+        span = otel_trace.get_current_span()
         if not span:
             raise RuntimeError("H.record_exception called without a span context")
         span.record_exception(e, attributes)
 
     @property
     def logging_handler(self) -> logging.Handler:
         """A logging handler implementing `logging.Handler` that allows plugging highlight_io
@@ -470,15 +469,15 @@
 
         LoggingInstrumentor().instrument(
             set_logging_format=True, log_hook=self.log_hook
         )
         otel_factory = logging.getLogRecordFactory()
 
         def factory(*args, **kwargs) -> LogRecord:
-            span = trace.get_current_span()
+            span = otel_trace.get_current_span()
             if span != INVALID_SPAN:
                 manager = contextlib.nullcontext(enter_result=span)
             else:
                 manager = self.trace()
 
             try:
                 with manager:
@@ -497,14 +496,22 @@
 
         :param trace_id: the trace id to lookup
         :return: a tuple of (session_id, request_id)
         """
         return self._context_map.get(trace_id, ("", ""))
 
 
+def trace(func):
+    def wrapper():
+        with H.get_instance().trace(span_name=func.__name__):
+            return func()
+
+    return wrapper
+
+
 def _build_resource(
     service_name: str,
     service_version: str,
     environment: str,
 ) -> Resource:
     attrs = {}
```

### Comparing `highlight_io-0.7.0/highlight_io/utils/lru_cache.py` & `highlight_io-0.7.1/highlight_io/utils/lru_cache.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.7.0/pyproject.toml` & `highlight_io-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highlight-io"
-version = "0.7.0"
+version = "0.7.1"
 description = "Session replay and error monitoring: stop guessing why bugs happen!"
 license = "Apache-2.0"
 authors = [
     "Vadim Korolik <vadim@highlight.io>",
     "Jay Khatri <jay@highlight.io>",
 ]
 readme = "README.md"
```

### Comparing `highlight_io-0.7.0/PKG-INFO` & `highlight_io-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highlight-io
-Version: 0.7.0
+Version: 0.7.1
 Summary: Session replay and error monitoring: stop guessing why bugs happen!
 Home-page: https://www.highlight.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Vadim Korolik
 Author-email: vadim@highlight.io
 Requires-Python: >=3.8,<4
```

