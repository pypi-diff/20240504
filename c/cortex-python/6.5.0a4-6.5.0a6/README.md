# Comparing `tmp/cortex_python-6.5.0a4.tar.gz` & `tmp/cortex_python-6.5.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_python-6.5.0a4.tar", max compression
+gzip compressed data, was "cortex_python-6.5.0a6.tar", max compression
```

## Comparing `cortex_python-6.5.0a4.tar` & `cortex_python-6.5.0a6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11368 2024-04-22 16:39:53.323130 cortex_python-6.5.0a4/LICENSE
--rw-r--r--   0        0        0     3889 2024-04-22 16:39:53.324130 cortex_python-6.5.0a4/README.md
--rw-r--r--   0        0        0      667 2024-04-22 16:39:53.324130 cortex_python-6.5.0a4/cortex/__init__.py
--rw-r--r--   0        0        0     1600 2024-04-22 16:39:53.324130 cortex_python-6.5.0a4/cortex/auth.py
--rw-r--r--   0        0        0     1989 2024-04-22 16:39:53.324130 cortex_python-6.5.0a4/cortex/camel.py
--rw-r--r--   0        0        0    27332 2024-04-22 16:39:53.324130 cortex_python-6.5.0a4/cortex/client.py
--rw-r--r--   0        0        0     3428 2024-04-22 16:39:53.324130 cortex_python-6.5.0a4/cortex/connection.py
--rw-r--r--   0        0        0      684 2024-04-22 16:39:53.324130 cortex_python-6.5.0a4/cortex/constant.py
--rw-r--r--   0        0        0     9669 2024-04-22 16:39:53.324130 cortex_python-6.5.0a4/cortex/content.py
--rw-r--r--   0        0        0     2532 2024-04-22 16:39:53.324130 cortex_python-6.5.0a4/cortex/env.py
--rw-r--r--   0        0        0     2477 2024-04-22 16:39:53.324130 cortex_python-6.5.0a4/cortex/exceptions.py
--rw-r--r--   0        0        0      675 2024-04-22 16:39:53.325130 cortex_python-6.5.0a4/cortex/experiment/__init__.py
--rw-r--r--   0        0        0     7794 2024-04-22 16:39:53.325130 cortex_python-6.5.0a4/cortex/experiment/local.py
--rw-r--r--   0        0        0    10717 2024-04-22 16:39:53.325130 cortex_python-6.5.0a4/cortex/experiment/model.py
--rw-r--r--   0        0        0    37474 2024-04-22 16:39:53.325130 cortex_python-6.5.0a4/cortex/experiment/remote.py
--rw-r--r--   0        0        0     3195 2024-04-22 16:39:53.325130 cortex_python-6.5.0a4/cortex/message.py
--rw-r--r--   0        0        0     2971 2024-04-22 16:39:53.325130 cortex_python-6.5.0a4/cortex/models.py
--rw-r--r--   0        0        0    10071 2024-04-22 16:39:53.325130 cortex_python-6.5.0a4/cortex/properties.py
--rw-r--r--   0        0        0     2517 2024-04-22 16:39:53.326130 cortex_python-6.5.0a4/cortex/secrets.py
--rw-r--r--   0        0        0    11766 2024-04-22 16:39:53.326130 cortex_python-6.5.0a4/cortex/serviceconnector.py
--rw-r--r--   0        0        0     4460 2024-04-22 16:39:53.326130 cortex_python-6.5.0a4/cortex/session.py
--rw-r--r--   0        0        0     8521 2024-04-22 16:39:53.326130 cortex_python-6.5.0a4/cortex/skill.py
--rw-r--r--   0        0        0     1347 2024-04-22 16:39:53.326130 cortex_python-6.5.0a4/cortex/timer.py
--rw-r--r--   0        0        0     1950 2024-04-22 16:39:53.326130 cortex_python-6.5.0a4/cortex/types.py
--rw-r--r--   0        0        0     9079 2024-04-22 16:39:53.326130 cortex_python-6.5.0a4/cortex/utils.py
--rw-r--r--   0        0        0     4410 2024-04-22 16:39:53.326130 cortex_python-6.5.0a4/cortex/viz.py
--rw-r--r--   0        0        0     1780 2024-04-22 16:44:08.955175 cortex_python-6.5.0a4/pyproject.toml
--rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 cortex_python-6.5.0a4/PKG-INFO
+-rw-r--r--   0        0        0    11368 2024-04-16 02:35:18.682957 cortex_python-6.5.0a6/LICENSE
+-rw-r--r--   0        0        0     4274 2024-05-03 04:33:14.451244 cortex_python-6.5.0a6/README.md
+-rw-r--r--   0        0        0      667 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/__init__.py
+-rw-r--r--   0        0        0     1600 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/auth.py
+-rw-r--r--   0        0        0     1989 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/camel.py
+-rw-r--r--   0        0        0    27332 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/client.py
+-rw-r--r--   0        0        0     3428 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/connection.py
+-rw-r--r--   0        0        0      684 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/constant.py
+-rw-r--r--   0        0        0     9669 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/content.py
+-rw-r--r--   0        0        0     2532 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/env.py
+-rw-r--r--   0        0        0     2477 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/exceptions.py
+-rw-r--r--   0        0        0      675 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/experiment/__init__.py
+-rw-r--r--   0        0        0     7794 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/experiment/local.py
+-rw-r--r--   0        0        0    10717 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/experiment/model.py
+-rw-r--r--   0        0        0    37474 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/experiment/remote.py
+-rw-r--r--   0        0        0     3195 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/message.py
+-rw-r--r--   0        0        0     3460 2024-05-03 13:56:51.034809 cortex_python-6.5.0a6/cortex/models.py
+-rw-r--r--   0        0        0    10071 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/properties.py
+-rw-r--r--   0        0        0     2517 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/secrets.py
+-rw-r--r--   0        0        0    11766 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/serviceconnector.py
+-rw-r--r--   0        0        0     4460 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/session.py
+-rw-r--r--   0        0        0     8521 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/skill.py
+-rw-r--r--   0        0        0     1347 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/timer.py
+-rw-r--r--   0        0        0     1950 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/types.py
+-rw-r--r--   0        0        0     9079 2024-04-16 02:35:18.685957 cortex_python-6.5.0a6/cortex/utils.py
+-rw-r--r--   0        0        0     4410 2024-04-16 02:35:18.685957 cortex_python-6.5.0a6/cortex/viz.py
+-rw-r--r--   0        0        0     2522 2024-05-03 21:59:50.142056 cortex_python-6.5.0a6/pyproject.toml
+-rw-r--r--   0        0        0     5823 1970-01-01 00:00:00.000000 cortex_python-6.5.0a6/PKG-INFO
```

### Comparing `cortex_python-6.5.0a4/LICENSE` & `cortex_python-6.5.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/README.md` & `cortex_python-6.5.0a6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,47 +3,46 @@
 The Cortex Python module provides an API client library to easily integrate with the Cortex Cognitive Platform. 
 Refer to the Cortex documentation for details on how to use the library: 
 
 - Developer guide: https://cognitivescale.github.io/cortex-fabric/
 - Cortex Python references: https://cognitivescale.github.io/cortex-python/master/
 
 ## Installation
+There are several installation options available: 
 
-To install: 
+* base library - for interacting with a Sensa cluster or developing skills 
 
 ```bash
 poetry add cortex-python
 ```
 
-or from source code:
-
+* model development - for feature and model developing within jupyter notebooks 
 ```bash
-git clone git@github.com:CognitiveScale/cortex-python.git
-cd cortex-python
-poetry install
+poetry add cortex-python[model_development]
 ```
 
-To install the optional components: 
-
-When developing models using jupyter within notebooks
-
+* model development extras - for developing model training and inference skills
 ```bash
-poetry install cortex-python[models_dev]
+poetry add cortex-python[model_runtime]
 ```
 
-When using model SDK using jupyter within notebooks
-
+* Certifai Evaluator plugin - this must be installed with on of the model* extras
+    **NOTE:** extra config needed to access the Sensa python repository
 ```bash
-poetry install cortex-python[models_dev]
+poetry config http-basic.sensa <USER> <TOKEN> 
+poetry add cortex-python[model_development,certifai]
 ```
 
-When using the library within Skills
-
+#### Install from source
 ```bash
-poetry install cortex-python[models_runtime]
+git clone git@github.com:CognitiveScale/cortex-python.git
+cd cortex-python
+# Needed for certifai components
+poetry config http-basic.sensa <USER> <TOKEN> 
+poetry install
 ```
 
 ## Development 
 
 ### Setup
 
 When developing, it's a best practice to work in a virtual environment. Create and activate a virtual environment:
```

### Comparing `cortex_python-6.5.0a4/cortex/__init__.py` & `cortex_python-6.5.0a6/cortex/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/auth.py` & `cortex_python-6.5.0a6/cortex/auth.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/camel.py` & `cortex_python-6.5.0a6/cortex/camel.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/client.py` & `cortex_python-6.5.0a6/cortex/client.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/connection.py` & `cortex_python-6.5.0a6/cortex/connection.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/constant.py` & `cortex_python-6.5.0a6/cortex/constant.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/content.py` & `cortex_python-6.5.0a6/cortex/content.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/env.py` & `cortex_python-6.5.0a6/cortex/env.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/exceptions.py` & `cortex_python-6.5.0a6/cortex/exceptions.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/experiment/__init__.py` & `cortex_python-6.5.0a6/cortex/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/experiment/local.py` & `cortex_python-6.5.0a6/cortex/experiment/local.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/experiment/model.py` & `cortex_python-6.5.0a6/cortex/experiment/model.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/experiment/remote.py` & `cortex_python-6.5.0a6/cortex/experiment/remote.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/message.py` & `cortex_python-6.5.0a6/cortex/message.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/models.py` & `cortex_python-6.5.0a6/cortex/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,27 +45,33 @@
 
     def _setup_model_client(self, verify_ssl_cert=True, ttl="2h"):
         # Generate a JWT, this call stores the JWT in `_serviceconnector.jwt` ( meh )
         token = generate_token(self._serviceconnector._config, verify_ssl_cert=verify_ssl_cert, validity=ttl)  # pylint: disable=protected-access
         mlflow.set_tracking_uri(self._serviceconnector.url)
         os.environ['MLFLOW_TRACKING_URI'] = self._serviceconnector.url
         os.environ['MLFLOW_TRACKING_TOKEN'] = token
+        # Following behavior from python requests https://requests.readthedocs.io/en/latest/user/advanced/#ssl-cert-verification
+        if verify_ssl_cert is False:
+            os.environ['MLFLOW_TRACKING_INSECURE_TLS'] = "true"
+        elif isinstance(verify_ssl_cert, str):
+            os.environ['CURL_CA_BUNDLE'] = verify_ssl_cert
+
         #  detect cortex client setting to avoid invalid SSL cert errors
-        # os.environ['MLFLOW_TRACKING_TOKEN']='true'
         # os.environ['MLFLOW_TRACKING_CLIENT_CERT_PATH']=
         # Need api to fetch serverside userid..
         # os.environ['MLFLOW_TRACKING_USERNAME']=_Client.???
 
-    def login(self, ttl: Optional[Union[str, int]] = '2h'):
+    def login(self, ttl: Optional[Union[str, int]] = '2h', verify_ssl_cert: Optional[Union[bool, str]]=True):
         """
         Configure connection settings for model registry.
         :param ttl: Time to live, DEFAULT: 2h
+        :param verify_ssl_cert: Boolean enable/disable SSL certificate or String with certificate filepath, DEFAULT: True
         """
         check_installed()
-        self._setup_model_client(ttl=ttl)
+        self._setup_model_client(ttl=ttl, verify_ssl_cert=verify_ssl_cert)
         print("Configuring connection for model registry")
 
     def create_experiment(self,
                           name: str,
                           tags: Optional[Dict[str, Any]] = None,
                           ) -> str:
         """
```

### Comparing `cortex_python-6.5.0a4/cortex/properties.py` & `cortex_python-6.5.0a6/cortex/properties.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/secrets.py` & `cortex_python-6.5.0a6/cortex/secrets.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/serviceconnector.py` & `cortex_python-6.5.0a6/cortex/serviceconnector.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/session.py` & `cortex_python-6.5.0a6/cortex/session.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/skill.py` & `cortex_python-6.5.0a6/cortex/skill.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/timer.py` & `cortex_python-6.5.0a6/cortex/timer.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/types.py` & `cortex_python-6.5.0a6/cortex/types.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/utils.py` & `cortex_python-6.5.0a6/cortex/utils.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/cortex/viz.py` & `cortex_python-6.5.0a6/cortex/viz.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a4/PKG-INFO` & `cortex_python-6.5.0a6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: cortex-python
-Version: 6.5.0a4
+Version: 6.5.0a6
 Summary: Python module for the Tecnotree Sensa Platform
 License: Apache-2.0
 Author: Tecnotree
 Author-email: support@tecnotree.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: certifai
 Provides-Extra: models-dev
 Provides-Extra: models-runtime
-Requires-Dist: cuid (>=0.4,<1)
-Requires-Dist: dill (>=0.3.6)
+Requires-Dist: certifai-evaluator-plugin (>=1.3.17,<2.0.0) ; extra == "certifai"
+Requires-Dist: cortex-certifai-common (>=1.3.17,<2.0.0)
+Requires-Dist: cortex_certifai_engine (>=1.3.17,<2.0.0)
+Requires-Dist: cortex_certifai_model_sdk (>=1.3.17,<2.0.0)
+Requires-Dist: cortex_certifai_scanner (>=1.3.17,<2.0.0)
+Requires-Dist: cuid (>=0.3,<0.4)
+Requires-Dist: dill (<=0.3.4)
 Requires-Dist: ipython (>=8.10,<9) ; extra == "models-dev"
 Requires-Dist: jinja2 (<4) ; extra == "models-dev"
 Requires-Dist: matplotlib (>3,<4) ; extra == "models-dev"
 Requires-Dist: mlflow (>1) ; extra == "models-dev" or extra == "models-runtime"
 Requires-Dist: pandas (<3) ; extra == "models-dev"
 Requires-Dist: pyjwt[crypto] (<3)
 Requires-Dist: python-dateutil (>=2.8.2,<3)
@@ -35,47 +40,46 @@
 The Cortex Python module provides an API client library to easily integrate with the Cortex Cognitive Platform. 
 Refer to the Cortex documentation for details on how to use the library: 
 
 - Developer guide: https://cognitivescale.github.io/cortex-fabric/
 - Cortex Python references: https://cognitivescale.github.io/cortex-python/master/
 
 ## Installation
+There are several installation options available: 
 
-To install: 
+* base library - for interacting with a Sensa cluster or developing skills 
 
 ```bash
 poetry add cortex-python
 ```
 
-or from source code:
-
+* model development - for feature and model developing within jupyter notebooks 
 ```bash
-git clone git@github.com:CognitiveScale/cortex-python.git
-cd cortex-python
-poetry install
+poetry add cortex-python[model_development]
 ```
 
-To install the optional components: 
-
-When developing models using jupyter within notebooks
-
+* model development extras - for developing model training and inference skills
 ```bash
-poetry install cortex-python[models_dev]
+poetry add cortex-python[model_runtime]
 ```
 
-When using model SDK using jupyter within notebooks
-
+* Certifai Evaluator plugin - this must be installed with on of the model* extras
+    **NOTE:** extra config needed to access the Sensa python repository
 ```bash
-poetry install cortex-python[models_dev]
+poetry config http-basic.sensa <USER> <TOKEN> 
+poetry add cortex-python[model_development,certifai]
 ```
 
-When using the library within Skills
-
+#### Install from source
 ```bash
-poetry install cortex-python[models_runtime]
+git clone git@github.com:CognitiveScale/cortex-python.git
+cd cortex-python
+# Needed for certifai components
+poetry config http-basic.sensa <USER> <TOKEN> 
+poetry install
 ```
 
 ## Development 
 
 ### Setup
 
 When developing, it's a best practice to work in a virtual environment. Create and activate a virtual environment:
```

