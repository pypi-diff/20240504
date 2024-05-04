# Comparing `tmp/agentops-0.1.7.tar.gz` & `tmp/agentops-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentops-0.1.7.tar", last modified: Fri May  3 19:21:33 2024, max compression
+gzip compressed data, was "agentops-0.1.8.tar", last modified: Sat May  4 03:01:49 2024, max compression
```

## Comparing `agentops-0.1.7.tar` & `agentops-0.1.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:21:33.291933 agentops-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 19:21:28.000000 agentops-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-05-03 19:21:33.291933 agentops-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-03 19:21:28.000000 agentops-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:21:33.287933 agentops-0.1.7/agentops/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4857 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    14941 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/host_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/langchain_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/llm_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:21:33.291933 agentops-0.1.7/agentops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-05-03 19:21:33.000000 agentops-0.1.7/agentops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-03 19:21:33.000000 agentops-0.1.7/agentops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:21:33.000000 agentops-0.1.7/agentops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 19:21:33.000000 agentops-0.1.7/agentops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 19:21:33.000000 agentops-0.1.7/agentops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-03 19:21:28.000000 agentops-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:21:33.291933 agentops-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:21:33.287933 agentops-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-03 19:21:28.000000 agentops-0.1.7/tests/test_canary.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-03 19:21:28.000000 agentops-0.1.7/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-03 19:21:28.000000 agentops-0.1.7/tests/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-03 19:21:28.000000 agentops-0.1.7/tests/test_record_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-03 19:21:28.000000 agentops-0.1.7/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-03 19:21:28.000000 agentops-0.1.7/tests/test_teardown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:01:49.256699 agentops-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-04 03:01:44.000000 agentops-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-05-04 03:01:49.256699 agentops-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-04 03:01:44.000000 agentops-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:01:49.252699 agentops-0.1.8/agentops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4857 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15247 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/host_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/langchain_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/llm_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:01:49.256699 agentops-0.1.8/agentops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-05-04 03:01:49.000000 agentops-0.1.8/agentops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-04 03:01:49.000000 agentops-0.1.8/agentops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 03:01:49.000000 agentops-0.1.8/agentops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-04 03:01:49.000000 agentops-0.1.8/agentops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 03:01:49.000000 agentops-0.1.8/agentops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-04 03:01:44.000000 agentops-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 03:01:49.256699 agentops-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:01:49.256699 agentops-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-04 03:01:44.000000 agentops-0.1.8/tests/test_canary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-04 03:01:44.000000 agentops-0.1.8/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-04 03:01:44.000000 agentops-0.1.8/tests/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-04 03:01:44.000000 agentops-0.1.8/tests/test_record_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-04 03:01:44.000000 agentops-0.1.8/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-04 03:01:44.000000 agentops-0.1.8/tests/test_teardown.py
```

### Comparing `agentops-0.1.7/LICENSE` & `agentops-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/PKG-INFO` & `agentops-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.7 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.8 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
```

### Comparing `agentops-0.1.7/README.md` & `agentops-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/__init__.py` & `agentops-0.1.8/agentops/__init__.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/agent.py` & `agentops-0.1.8/agentops/agent.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/client.py` & `agentops-0.1.8/agentops/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,15 +73,16 @@
                            DeprecationWarning, stacklevel=2)
             instrument_llm_calls = instrument_llm_calls or override
 
         self._session = None
         self._worker = None
         self._tags_for_future_session = None
 
-        self._env_data_opt_out = os.getenv('AGENTOPS_ENV_DATA_OPT_OUT') and os.getenv('AGENTOPS_ENV_DATA_OPT_OUT').lower() == 'true'
+        self._env_data_opt_out = os.getenv('AGENTOPS_ENV_DATA_OPT_OUT') and os.getenv(
+            'AGENTOPS_ENV_DATA_OPT_OUT').lower() == 'true'
 
         try:
             self.config = Configuration(api_key=api_key,
                                         parent_key=parent_key,
                                         endpoint=endpoint,
                                         max_wait_time=max_wait_time,
                                         max_queue_size=max_queue_size)
@@ -132,27 +133,32 @@
     def record(self, event: Event | ErrorEvent):
         """
             Record an event with the AgentOps service.
 
             Args:
                 event (Event): The event to record.
         """
-        if not event.end_timestamp or event.init_timestamp == event.end_timestamp:
-            event.end_timestamp = get_ISO_time()
-        if self._session is not None and not self._session.has_ended:
+        if self._session is None or self._session.has_ended:
+            logger.warning("🖇 AgentOps: Cannot record event - no current session")
+            return
+
+        # Need to update end_timestamp for ErrorEvent so creating this event_local pointer
+        event_local = event.trigger_event if isinstance(event, ErrorEvent) else event
+        if event_local:  # ErrorEvent may not have a trigger_event set
+            if not event_local.end_timestamp or event_local.init_timestamp == event_local.end_timestamp:
+                event_local.end_timestamp = get_ISO_time()
+
             if isinstance(event, ErrorEvent):
-                if event.trigger_event:
-                    event.trigger_event_id = event.trigger_event.id
-                    event.trigger_event_type = event.trigger_event.event_type
-                    self._worker.add_event(event.trigger_event.__dict__)
-                    event.trigger_event = None  # removes trigger_event from serialization
-            self._worker.add_event(event.__dict__)
-        else:
-            logger.warning(
-                "🖇 AgentOps: Cannot record event - no current session")
+                # Extract trigger_event info from ErrorEvent and log trigger_event
+                event.trigger_event_id = event_local.id
+                event.trigger_event_type = event_local.event_type
+                self._worker.add_event(event_local.__dict__)
+                event.trigger_event = None  # removes trigger_event from serialization
+
+        self._worker.add_event(event.__dict__)
 
     def _record_event_sync(self, func, event_name, *args, **kwargs):
         init_time = get_ISO_time()
         func_args = inspect.signature(func).parameters
         arg_names = list(func_args.keys())
         # Get default values
         arg_values = {name: func_args[name].default
@@ -236,15 +242,16 @@
 
         if self._session is not None:
             return logger.warning("🖇 AgentOps: Cannot start session - session already started")
 
         if not config and not self.config:
             return logger.warning("🖇 AgentOps: Cannot start session - missing configuration")
 
-        self._session = Session(inherited_session_id or uuid4(), tags or self._tags_for_future_session, host_env=get_host_env(self._env_data_opt_out))
+        self._session = Session(inherited_session_id or uuid4(),
+                                tags or self._tags_for_future_session, host_env=get_host_env(self._env_data_opt_out))
         self._worker = Worker(config or self.config)
         start_session_result = self._worker.start_session(self._session)
         if not start_session_result:
             self._session = None
             return logger.warning("🖇 AgentOps: Cannot start session")
 
         logger.info('View info on this session at https://app.agentops.ai/drilldown?session_id={}'
```

### Comparing `agentops-0.1.7/agentops/config.py` & `agentops-0.1.8/agentops/config.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/decorators.py` & `agentops-0.1.8/agentops/decorators.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/enums.py` & `agentops-0.1.8/agentops/enums.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/event.py` & `agentops-0.1.8/agentops/event.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/helpers.py` & `agentops-0.1.8/agentops/helpers.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/host_env.py` & `agentops-0.1.8/agentops/host_env.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/http_client.py` & `agentops-0.1.8/agentops/http_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/langchain_callback_handler.py` & `agentops-0.1.8/agentops/langchain_callback_handler.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/llm_tracker.py` & `agentops-0.1.8/agentops/llm_tracker.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/meta_client.py` & `agentops-0.1.8/agentops/meta_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/session.py` & `agentops-0.1.8/agentops/session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops/worker.py` & `agentops-0.1.8/agentops/worker.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/agentops.egg-info/PKG-INFO` & `agentops-0.1.8/agentops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.7 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.8 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
```

### Comparing `agentops-0.1.7/agentops.egg-info/SOURCES.txt` & `agentops-0.1.8/agentops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/pyproject.toml` & `agentops-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "agentops"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Alex Reibman", email="areibman@gmail.com" },
   { name="Shawn Qiu", email="siyangqiu@gmail.com" },
   { name="Braelyn Boynton", email="bboynton97@gmail.com" },
   { name="Howard Gil", email="howardbgil@gmail.com" }
 ]
 description = "Python SDK for developing AI agent evals and observability"
```

### Comparing `agentops-0.1.7/tests/test_canary.py` & `agentops-0.1.8/tests/test_canary.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/tests/test_events.py` & `agentops-0.1.8/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/tests/test_patcher.py` & `agentops-0.1.8/tests/test_patcher.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/tests/test_record_function.py` & `agentops-0.1.8/tests/test_record_function.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/tests/test_session.py` & `agentops-0.1.8/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.7/tests/test_teardown.py` & `agentops-0.1.8/tests/test_teardown.py`

 * *Files identical despite different names*

