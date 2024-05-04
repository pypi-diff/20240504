# Comparing `tmp/spark_on_k8s-0.5.2.tar.gz` & `tmp/spark_on_k8s-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_on_k8s-0.5.2.tar", max compression
+gzip compressed data, was "spark_on_k8s-0.6.0rc1.tar", max compression
```

## Comparing `spark_on_k8s-0.5.2.tar` & `spark_on_k8s-0.6.0rc1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11357 2024-05-03 12:14:02.577140 spark_on_k8s-0.5.2/LICENSE
--rw-r--r--   0        0        0    11213 2024-05-03 12:14:02.577140 spark_on_k8s-0.5.2/README.md
--rw-r--r--   0        0        0     2366 2024-05-03 12:14:18.773167 spark_on_k8s-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       58 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/airflow/__init__.py
--rw-r--r--   0        0        0    15115 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/airflow/operators.py
--rw-r--r--   0        0        0     3114 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/airflow/triggers.py
--rw-r--r--   0        0        0     1190 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/__init__.py
--rw-r--r--   0        0        0     1744 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/app.py
--rw-r--r--   0        0        0     1472 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/apps.py
--rw-r--r--   0        0        0      728 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/configuration.py
--rw-r--r--   0        0        0     1305 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/main.py
--rw-r--r--   0        0        0     6750 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/__init__.py
--rw-r--r--   0        0        0      587 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/static/app_logs.css
--rw-r--r--   0        0        0      758 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/static/apps.css
--rw-r--r--   0        0        0     1416 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/templates/app_logs.html
--rw-r--r--   0        0        0     2953 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/templates/apps.html
--rw-r--r--   0        0        0      368 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/templates/error.html
--rw-r--r--   0        0        0      542 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/cli/__init__.py
--rw-r--r--   0        0        0     1621 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/cli/api.py
--rw-r--r--   0        0        0     6601 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/cli/app.py
--rw-r--r--   0        0        0      690 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/cli/apps.py
--rw-r--r--   0        0        0      553 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/cli/namespace.py
--rw-r--r--   0        0        0     8686 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/cli/options.py
--rw-r--r--   0        0        0    27728 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/client.py
--rw-r--r--   0        0        0        0 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/k8s/__init__.py
--rw-r--r--   0        0        0     3135 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/k8s/async_client.py
--rw-r--r--   0        0        0     2849 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/k8s/sync_client.py
--rw-r--r--   0        0        0        0 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/__init__.py
--rw-r--r--   0        0        0    19764 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/app_manager.py
--rw-r--r--   0        0        0     9617 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/async_app_manager.py
--rw-r--r--   0        0        0     4048 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/configuration.py
--rw-r--r--   0        0        0      488 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/logging_mixin.py
--rw-r--r--   0        0        0     3956 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/setup_namespace.py
--rw-r--r--   0        0        0      842 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/spark_app_status.py
--rw-r--r--   0        0        0      141 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/types.py
--rw-r--r--   0        0        0    13060 1970-01-01 00:00:00.000000 spark_on_k8s-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-04 14:15:07.228942 spark_on_k8s-0.6.0rc1/LICENSE
+-rw-r--r--   0        0        0    11213 2024-05-04 14:15:07.228942 spark_on_k8s-0.6.0rc1/README.md
+-rw-r--r--   0        0        0     2371 2024-05-04 14:15:21.952981 spark_on_k8s-0.6.0rc1/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/airflow/__init__.py
+-rw-r--r--   0        0        0    17061 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/airflow/operators.py
+-rw-r--r--   0        0        0     3114 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/airflow/triggers.py
+-rw-r--r--   0        0        0     1190 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/__init__.py
+-rw-r--r--   0        0        0     1744 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/app.py
+-rw-r--r--   0        0        0     1472 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/apps.py
+-rw-r--r--   0        0        0      728 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/configuration.py
+-rw-r--r--   0        0        0     1305 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/main.py
+-rw-r--r--   0        0        0     6750 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/__init__.py
+-rw-r--r--   0        0        0      587 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/static/app_logs.css
+-rw-r--r--   0        0        0      758 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/static/apps.css
+-rw-r--r--   0        0        0     1416 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/templates/app_logs.html
+-rw-r--r--   0        0        0     2953 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/templates/apps.html
+-rw-r--r--   0        0        0      368 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/templates/error.html
+-rw-r--r--   0        0        0      542 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/__init__.py
+-rw-r--r--   0        0        0     1621 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/api.py
+-rw-r--r--   0        0        0     6601 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/app.py
+-rw-r--r--   0        0        0      690 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/apps.py
+-rw-r--r--   0        0        0      553 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/namespace.py
+-rw-r--r--   0        0        0     8686 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/options.py
+-rw-r--r--   0        0        0    27728 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/client.py
+-rw-r--r--   0        0        0        0 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/k8s/__init__.py
+-rw-r--r--   0        0        0     3135 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/k8s/async_client.py
+-rw-r--r--   0        0        0     2849 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/k8s/sync_client.py
+-rw-r--r--   0        0        0        0 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/__init__.py
+-rw-r--r--   0        0        0    19764 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/app_manager.py
+-rw-r--r--   0        0        0     9617 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/async_app_manager.py
+-rw-r--r--   0        0        0     4048 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/configuration.py
+-rw-r--r--   0        0        0      488 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/logging_mixin.py
+-rw-r--r--   0        0        0     3956 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/setup_namespace.py
+-rw-r--r--   0        0        0      842 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/spark_app_status.py
+-rw-r--r--   0        0        0      141 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/types.py
+-rw-r--r--   0        0        0    13063 1970-01-01 00:00:00.000000 spark_on_k8s-0.6.0rc1/PKG-INFO
```

### Comparing `spark_on_k8s-0.5.2/LICENSE` & `spark_on_k8s-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/README.md` & `spark_on_k8s-0.6.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/pyproject.toml` & `spark_on_k8s-0.6.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spark-on-k8s"
-version = "0.5.2"
+version = "0.6.0-rc.1"
 description = "A Python package to submit and manage Apache Spark applications on Kubernetes."
 authors = ["Hussein Awala <hussein@awala.fr>"]
 readme = "README.md"
 repository = "https://github.com/hussein-awala/spark-on-k8s"
 keywords = ["spark", "kubernetes", "k8s", "spark-submit", "spark-on-k8s"]
 license = "Apache-2.0"
 packages = [{include = "spark_on_k8s"}]
```

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/airflow/operators.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/airflow/operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import contextlib
 from enum import Enum
 from typing import TYPE_CHECKING, Any
 
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from spark_on_k8s.airflow.triggers import SparkOnK8STrigger
 from spark_on_k8s.k8s.sync_client import KubernetesClientManager
@@ -12,14 +13,15 @@
     from typing import Literal
 
     import jinja2
     from kubernetes import client as k8s
 
     from airflow.utils.context import Context
     from spark_on_k8s.client import ExecutorInstances, PodResources
+    from spark_on_k8s.utils.app_manager import SparkAppManager
 
 
 class _AirflowKubernetesClientManager(KubernetesClientManager):
     """A Kubernetes client manager for Airflow."""
 
     def __init__(self, kubernetes_conn_id: str, **kwargs):
         super().__init__(**kwargs)
@@ -44,14 +46,16 @@
 
     Args:
         image (str): Spark application image.
         app_path (str): Path to the Spark application.
         namespace (str, optional): Kubernetes namespace. Defaults to "default".
         service_account (str, optional): Kubernetes service account. Defaults to "spark".
         app_name (str, optional): Spark application name. Defaults to None.
+        app_id_suffix: A suffix for the application ID, defaults to current timestamp in
+            the format %Y%m%d%H%M%S prefixed with a dash.
         spark_conf (dict[str, str], optional): Spark configuration. Defaults to None.
         class_name (str, optional): Spark application class name. Defaults to None.
         app_arguments (list[str], optional): Spark application arguments. Defaults to None.
         app_waiter (Literal["no_wait", "wait", "log"], optional): Spark application waiter.
             Defaults to "wait".
         image_pull_policy (Literal["Always", "Never", "IfNotPresent"], optional): Image pull policy.
             Defaults to "IfNotPresent".
@@ -74,22 +78,26 @@
             Defaults to 10.
         deferrable (bool, optional): Whether the operator is deferrable. Defaults to False.
         on_kill_action (Literal["keep", "delete", "kill"], optional): Action to take when the
             operator is killed. Defaults to "delete".
         **kwargs: Other keyword arguments for BaseOperator.
     """
 
+    _XCOM_DRIVER_POD_NAMESPACE = "driver_pod_namespace"
+    _XCOM_DRIVER_POD_NAME = "driver_pod_name"
+
     _driver_pod_name: str | None = None
 
     template_fields = (
         "image",
         "app_path",
         "namespace",
         "service_account",
         "app_name",
+        "app_id_suffix",
         "spark_conf",
         "class_name",
         "app_arguments",
         "app_waiter",
         "image_pull_policy",
         "driver_resources",
         "executor_resources",
@@ -102,14 +110,15 @@
         self,
         *,
         image: str,
         app_path: str,
         namespace: str = "default",
         service_account: str = "spark",
         app_name: str | None = None,
+        app_id_suffix: str = None,
         spark_conf: dict[str, str] | None = None,
         class_name: str | None = None,
         app_arguments: list[str] | None = None,
         app_waiter: Literal["no_wait", "wait", "log"] = "wait",
         image_pull_policy: Literal["Always", "Never", "IfNotPresent"] = "IfNotPresent",
         ui_reverse_proxy: bool = False,
         driver_resources: PodResources | None = None,
@@ -135,14 +144,15 @@
     ):
         super().__init__(**kwargs)
         self.image = image
         self.app_path = app_path
         self.namespace = namespace
         self.service_account = service_account
         self.app_name = app_name
+        self.app_id_suffix = app_id_suffix
         self.spark_conf = spark_conf
         self.class_name = class_name
         self.app_arguments = app_arguments
         self.app_waiter = app_waiter
         self.image_pull_policy = image_pull_policy
         self.ui_reverse_proxy = ui_reverse_proxy
         self.driver_resources = driver_resources
@@ -188,17 +198,38 @@
             if template_fields:
                 seen_oids.add(id(content))
                 self._do_render_template_fields(content, template_fields, context, jinja_env, seen_oids)
                 return
 
         super()._render_nested_template_fields(content, context, jinja_env, seen_oids)
 
-    def execute(self, context):
+    def _persist_pod_name(self, context: Context):
+        context["ti"].xcom_push(key=self._XCOM_DRIVER_POD_NAMESPACE, value=self.namespace)
+        context["ti"].xcom_push(key=self._XCOM_DRIVER_POD_NAME, value=self._driver_pod_name)
+
+    def _try_to_adopt_job(self, context: Context, spark_app_manager: SparkAppManager) -> bool:
+        from spark_on_k8s.utils.spark_app_status import SparkAppStatus
+
+        xcom_driver_namespace = context["ti"].xcom_pull(key=self._XCOM_DRIVER_POD_NAMESPACE)
+        if not xcom_driver_namespace or xcom_driver_namespace != self.namespace:
+            return False
+        xcom_driver_pod_name = context["ti"].xcom_pull(key=self._XCOM_DRIVER_POD_NAME)
+        if xcom_driver_pod_name:
+            with contextlib.suppress(Exception):
+                app_status = spark_app_manager.app_status(
+                    namespace=xcom_driver_namespace,
+                    pod_name=xcom_driver_pod_name,
+                )
+                if app_status == SparkAppStatus.Running:
+                    self._driver_pod_name = xcom_driver_pod_name
+                    return True
+        return False
+
+    def _submit_new_job(self, context: Context):
         from spark_on_k8s.client import ExecutorInstances, PodResources, SparkOnK8S
-        from spark_on_k8s.utils.app_manager import SparkAppManager
 
         # post-process template fields
         if self.driver_resources:
             self.driver_resources = PodResources(
                 cpu=int(self.driver_resources.cpu) if self.driver_resources.cpu is not None else None,
                 memory=int(self.driver_resources.memory)
                 if self.driver_resources.memory is not None
@@ -226,14 +257,17 @@
 
         k8s_client_manager = _AirflowKubernetesClientManager(
             kubernetes_conn_id=self.kubernetes_conn_id,
         )
         spark_client = SparkOnK8S(
             k8s_client_manager=k8s_client_manager,
         )
+        submit_app_kwargs = {}
+        if self.app_id_suffix:
+            submit_app_kwargs["app_id_suffix"] = lambda: self.app_id_suffix
         self._driver_pod_name = spark_client.submit_app(
             image=self.image,
             app_path=self.app_path,
             namespace=self.namespace,
             service_account=self.service_account,
             app_name=self.app_name,
             spark_conf=self.spark_conf,
@@ -253,33 +287,41 @@
             executor_node_selector=self.executor_node_selector,
             driver_labels=self.driver_labels,
             executor_labels=self.executor_labels,
             driver_annotations=self.driver_annotations,
             executor_annotations=self.executor_annotations,
             driver_tolerations=self.driver_tolerations,
             executor_pod_template_path=self.executor_pod_template_path,
+            **submit_app_kwargs,
+        )
+
+    def execute(self, context: Context):
+        from spark_on_k8s.utils.app_manager import SparkAppManager
+
+        k8s_client_manager = _AirflowKubernetesClientManager(
+            kubernetes_conn_id=self.kubernetes_conn_id,
         )
+        spark_app_manager = SparkAppManager(
+            k8s_client_manager=k8s_client_manager,
+        )
+        if not self._try_to_adopt_job(context, spark_app_manager):
+            self._submit_new_job(context)
+            self._persist_pod_name(context)
         if self.app_waiter == "no_wait":
             return
         if self.deferrable:
             self.defer(
                 trigger=SparkOnK8STrigger(
                     driver_pod_name=self._driver_pod_name,
                     namespace=self.namespace,
                     kubernetes_conn_id=self.kubernetes_conn_id,
                     poll_interval=self.poll_interval,
                 ),
                 method_name="execute_complete",
             )
-        k8s_client_manager = _AirflowKubernetesClientManager(
-            kubernetes_conn_id=self.kubernetes_conn_id,
-        )
-        spark_app_manager = SparkAppManager(
-            k8s_client_manager=k8s_client_manager,
-        )
         if self.app_waiter == "wait":
             spark_app_manager.wait_for_app(
                 namespace=self.namespace,
                 pod_name=self._driver_pod_name,
                 poll_interval=self.poll_interval,
             )
         elif self.app_waiter == "log":
```

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/airflow/triggers.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/airflow/triggers.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/api/__init__.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/api/app.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/app.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/api/apps.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/apps.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/api/configuration.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/configuration.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/api/main.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/main.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/__init__.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/static/app_logs.css` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/static/app_logs.css`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/static/apps.css` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/static/apps.css`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/templates/app_logs.html` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/templates/app_logs.html`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/templates/apps.html` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/templates/apps.html`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/cli/__init__.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/cli/api.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/api.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/cli/app.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/app.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/cli/apps.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/apps.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/cli/namespace.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/namespace.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/cli/options.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/options.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/client.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/k8s/async_client.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/k8s/async_client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/k8s/sync_client.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/k8s/sync_client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/utils/app_manager.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/app_manager.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/utils/async_app_manager.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/async_app_manager.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/utils/configuration.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/utils/setup_namespace.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/setup_namespace.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/spark_on_k8s/utils/spark_app_status.py` & `spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/spark_app_status.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.2/PKG-INFO` & `spark_on_k8s-0.6.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-on-k8s
-Version: 0.5.2
+Version: 0.6.0rc1
 Summary: A Python package to submit and manage Apache Spark applications on Kubernetes.
 Home-page: https://github.com/hussein-awala/spark-on-k8s
 License: Apache-2.0
 Keywords: spark,kubernetes,k8s,spark-submit,spark-on-k8s
 Author: Hussein Awala
 Author-email: hussein@awala.fr
 Requires-Python: >=3.8,<4.0
```

