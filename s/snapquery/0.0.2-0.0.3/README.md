# Comparing `tmp/snapquery-0.0.2.tar.gz` & `tmp/snapquery-0.0.3.tar.gz`

## Comparing `snapquery-0.0.2.tar` & `snapquery-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snapquery-0.0.2/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 snapquery-0.0.2/.pydevproject
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snapquery-0.0.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 snapquery-0.0.2/.github/workflows/upload-to-pypi.yml
--rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 snapquery-0.0.2/scripts/blackisort
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 snapquery-0.0.2/scripts/install
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snapquery-0.0.2/scripts/test
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snapquery-0.0.2/snapquery/__init__.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 snapquery-0.0.2/snapquery/snapquery_cmd.py
--rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 snapquery-0.0.2/snapquery/snapquery_core.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 snapquery-0.0.2/snapquery/snapquery_webserver.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 snapquery-0.0.2/snapquery/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snapquery-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snapquery-0.0.2/tests/test_endpoints.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 snapquery-0.0.2/tests/test_namedqueries.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 snapquery-0.0.2/tests/test_restful_api.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 snapquery-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snapquery-0.0.2/LICENSE
--rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 snapquery-0.0.2/README.md
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 snapquery-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 snapquery-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snapquery-0.0.3/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 snapquery-0.0.3/.pydevproject
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snapquery-0.0.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 snapquery-0.0.3/.github/workflows/upload-to-pypi.yml
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 snapquery-0.0.3/scripts/blackisort
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 snapquery-0.0.3/scripts/install
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snapquery-0.0.3/scripts/test
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snapquery-0.0.3/snapquery/__init__.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 snapquery-0.0.3/snapquery/snapquery_cmd.py
+-rw-r--r--   0        0        0    13540 2020-02-02 00:00:00.000000 snapquery-0.0.3/snapquery/snapquery_core.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 snapquery-0.0.3/snapquery/snapquery_view.py
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 snapquery-0.0.3/snapquery/snapquery_webserver.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 snapquery-0.0.3/snapquery/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snapquery-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snapquery-0.0.3/tests/test_endpoints.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 snapquery-0.0.3/tests/test_namedqueries.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 snapquery-0.0.3/tests/test_restful_api.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 snapquery-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snapquery-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 snapquery-0.0.3/README.md
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 snapquery-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 snapquery-0.0.3/PKG-INFO
```

### Comparing `snapquery-0.0.2/.github/workflows/build.yml` & `snapquery-0.0.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.2/.github/workflows/upload-to-pypi.yml` & `snapquery-0.0.3/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.2/snapquery/snapquery_cmd.py` & `snapquery-0.0.3/snapquery/snapquery_cmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,14 +38,20 @@
         )
         parser.add_argument(
             "-le",
             "--listEndpoints",
             action="store_true",
             help="show the list of available endpoints",
         )
+        parser.add_argument(
+            "--limit", type=int, default=None, help="set limit parameter of query"
+        )
+        parser.add_argument(
+            "--namespace", type=str, default="wikidata-examples", help="namespace to filter queries"
+        )
         parser.add_argument("-qn", "--queryName", help="run a named query")
         parser.add_argument("-f", "--format", type=Format, choices=list(Format))
         return parser
 
     def handle_args(self) -> bool:
         """
         handle the command line args
@@ -57,22 +63,22 @@
         if self.args.listEndpoints:
             # List endpoints
             for endpoint in endpoints.values():
                 print(endpoint)
             handled = True  # Operation handled
         elif self.args.queryName is not None:
             nqm = NamedQueryManager()
+            namespace=self.args.namespace
             name = self.args.queryName
             endpoint_name = self.args.endpointName
             r_format = self.args.format
-            sparql_query = nqm.get_sparql(name=name, endpoint_name=endpoint_name)
-            qlod = nqm.query(endpoint_name=endpoint_name, name=name)
-            query = Query(name=name, query=sparql_query, lang="sparql")
-            nqm.format_result(qlod, query, r_format, endpoint_name=endpoint_name)
-        return handled
+            limit=self.args.limit
+            formatted_result=nqm.formatted_query(name, namespace=namespace,endpoint_name=endpoint_name, r_format=r_format,limit=limit)
+            print(formatted_result)
+            return handled
 
 
 def main(argv: list = None):
     """
     main call
     """
     cmd = SnapQueryCmd(
```

### Comparing `snapquery-0.0.2/snapquery/snapquery_core.py` & `snapquery-0.0.3/snapquery/snapquery_core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 Created on 2024-05-03
 
 @author: wf
 """
 import json
+import re
 import os
 from dataclasses import field
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 from lodstorage.csv import CSV
 from lodstorage.query import Endpoint, EndpointManager, Format, Query
 from lodstorage.sparql import SPARQL
 from lodstorage.sql import SQLDB, EntityInfo
 from lodstorage.yamlable import lod_storable
+from ngwidgets.widgets import Link
 
 
 @lod_storable
 class NamedQuery:
     """
     A named query that encapsulates the details and SPARQL query for a specific purpose.
 
@@ -46,14 +48,45 @@
     def __post_init__(self):
         """
         Post-initialization processing to construct a unique identifier for the query
         based on its namespace and name.
         """
         self.query_id = f"{self.namespace}.{self.name}"
 
+    def as_link(self) -> str:
+        url = f"/query/{self.namespace}/{self.name}"
+        text = self.name
+        tooltip = "query details"
+        link = Link.create(url, text, tooltip)
+        return link
+
+    @classmethod
+    def from_record(cls, record: Dict) -> "NamedQuery":
+        """
+        Class method to instantiate NamedQuery from a dictionary record.
+        """
+        return cls(
+            namespace=record["namespace"],
+            name=record["name"],
+            title=record["title"],
+            description=record["description"],
+            sparql=record["sparql"],
+        )
+
+    def as_viewrecord(self) -> Dict:
+        """
+        Return a dictionary representing the NamedQuery with keys ordered as Name, Namespace, Title, Description.
+        """
+        return {
+            "name": self.as_link(),
+            "namespace": self.namespace,
+            "title": self.title,
+            "description": self.description,
+        }
+
 
 class NamedQueryManager:
     """
     Manages the storage, retrieval, and execution of named SPARQL queries.
     """
 
     def __init__(self, db_path: str = None, debug: bool = False):
@@ -68,15 +101,15 @@
             debug (bool): Stores the debug state.
             sql_db (SQLDB): An instance of SQLDB to manage the SQLite database interactions.
             endpoints (dict): A dictionary of SPARQL endpoints configured for use.
         """
         if db_path is None:
             db_path = NamedQueryManager.get_cache_path()
         self.debug = debug
-        self.sql_db = SQLDB(dbname=db_path,check_same_thread=False, debug=debug)
+        self.sql_db = SQLDB(dbname=db_path, check_same_thread=False, debug=debug)
         self.endpoints = EndpointManager.getEndpoints(lang="sparql")
 
     @classmethod
     def get_cache_path(cls) -> str:
         home = str(Path.home())
         cache_dir = f"{home}/.solutions/snapquery/storage"
         os.makedirs(cache_dir, exist_ok=True)
@@ -192,64 +225,102 @@
         return sparql_query
 
     def query(
         self,
         name: str,
         namespace: str = "wikidata-examples",
         endpoint_name: str = "wikidata",
+        limit:int=None
     ):
         """
         Execute a named SPARQL query using a specified endpoint and return the results.
 
         Args:
             name (str): The name of the named query to execute.
             namespace (str): The namespace of the named query, default is 'wikidata-examples'.
             endpoint_name (str): The name of the endpoint to send the SPARQL query to, default is 'wikidata'.
+            limit(int): the query limit (if any)
 
         Returns:
             Dict[str, Any]: The results of the SPARQL query in JSON format.
 
         Raises:
             ValueError: If no named query matches the given name and namespace.
             Exception: If the SPARQL query execution fails or the endpoint returns an error.
         """
         sparql_query = self.get_sparql(name, namespace, endpoint_name)
 
         if not endpoint_name in self.endpoints:
             msg = f"Invalid endpoint {endpoint_name}"
             ValueError(msg)
         endpoint = self.endpoints.get(endpoint_name)
+        self.query = Query(name=name, query=sparql_query, lang="sparql",limit=limit)
+ 
         sparql = SPARQL(endpoint.endpoint)
+        if limit: 
+            # @TODO - this is to naive for cases where there are 
+            # SPARQL elements hat have a "limit" in the name e.g. "height_limit"
+            if "limit" in sparql_query or "LIMIT" in sparql_query:
+                sparql_query = re.sub(
+                    r"(limit|LIMIT)\s+(\d+)", f"LIMIT {limit}", sparql_query
+                )
+            else:
+                sparql_query += f"\nLIMIT {limit}"
         lod = sparql.queryAsListOfDicts(sparql_query)
         return lod
+    
+    def formatted_query(self,
+        name: str,
+        namespace: str = "wikidata-examples",
+        endpoint_name: str = "wikidata",
+        r_format: Format = Format.html,
+        limit:int=None)->str:
+        """
+        Execute a named SPARQL query using a specified endpoint and return the results formatted .
+
+        Args:
+            name (str): The name of the named query to execute.
+            namespace (str): The namespace of the named query, default is 'wikidata-examples'.
+            endpoint_name (str): The name of the endpoint to send the SPARQL query to, default is 'wikidata'.
+            r_format: (Format): the format to result should be returned in
+            limit(int): the query limit (if any)
+        Returns:
+            str: The results of the SPARQL query in the given format.
+
+        Raises:
+            ValueError: If no named query matches the given name and namespace.
+            Exception: If the SPARQL query execution fails or the endpoint returns an error.
+        """
+        qlod = self.query(endpoint_name=endpoint_name, name=name,namespace=namespace,limit=limit)
+        formatted_result=self.format_result(qlod=qlod, query=self.query, r_format=r_format, endpoint_name=endpoint_name)
+        return formatted_result
 
     def format_result(
         self,
         qlod: List[Dict[str, Any]],
         query: Query,
-        r_format_str: str,
+        r_format: Format,
         endpoint_name: str = "wikidata",
     ) -> Optional[str]:
         """
         Formats the query results based on the specified format and prints them.
 
         Args:
             qlod (List[Dict[str, Any]]): The list of dictionaries that represent the query results.
             query (Query): The query object which contains details like the endpoint and the database.
-            r_format_str: The format in which to print the results.
+            r_format_str(Format): The format in which to print the results.
             endpoint_name (str): The name of the endpoint to be used, defaults to "wikidata".
 
         Returns:
             Optional[str]: The formatted string representation of the query results, or None if printed directly.
         """
         # Retrieve endpoint configuration using the provided endpoint name
         endpointConf = self.endpoints.get(endpoint_name, Endpoint.getDefault())
         query.tryItUrl = endpointConf.website
         query.database = endpointConf.database
-        r_format = Format[r_format_str] 
 
         if r_format == Format.csv:
             csv_output = CSV.toCSV(qlod)
             return csv_output
         elif r_format in [Format.latex, Format.github, Format.mediawiki, Format.html]:
             doc = query.documentQueryResult(
                 qlod, tablefmt=str(r_format), floatfmt=".0f"
```

### Comparing `snapquery-0.0.2/snapquery/snapquery_webserver.py` & `snapquery-0.0.3/snapquery/snapquery_webserver.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 Created on 2024-05-03
 @author: wf
 """
-from fastapi import Request, Header,HTTPException
-from fastapi.responses import HTMLResponse
-from lodstorage.query import Query
+from fastapi import HTTPException
+from fastapi.responses import HTMLResponse, PlainTextResponse
+from lodstorage.query import Query, Format
 from ngwidgets.input_webserver import InputWebserver, InputWebSolution, WebserverConfig
 from nicegui import app
 from nicegui.client import Client
 
 from snapquery.snapquery_core import NamedQueryManager
+from snapquery.snapquery_view import NamedQuerySearch
 from snapquery.version import Version
 
 
 class SnapQueryWebServer(InputWebserver):
     """
     server to supply named Queries
     """
@@ -35,58 +36,79 @@
         return server_config
 
     def __init__(self):
         """Constructs all the necessary attributes for the WebServer object."""
         InputWebserver.__init__(self, config=SnapQueryWebServer.get_config())
         self.nqm = NamedQueryManager.from_samples()
 
-        @app.get("/query/{namespace}/{name}", response_class=HTMLResponse)
-        def query(namespace: str, name: str):
+        @app.get("/sparql/{namespace}/{name}")
+        def sparql(namespace: str, name: str) -> PlainTextResponse:
+            """
+            Gets a SPARQL query by name within a specified namespace
+
+            Args:
+                namespace (str): The namespace identifying the group or category of the query.
+                name (str): The specific name of the query to be executed.
+
+            Returns:
+                HTMLResponse: The plain text SPARQL code
+
+            Raises:
+                HTTPException: If the query cannot be found or fails to execute.
+            """
+            endpoint_name = "wikidata"
+            sparql_query = self.nqm.get_sparql(name, namespace, endpoint_name)
+            return PlainTextResponse(sparql_query)
+
+        @app.get("/query/{namespace}/{name}")
+        def query(namespace: str, name: str) -> HTMLResponse:
             """
             Executes a SPARQL query by name within a specified namespace, formats the results, and returns them as an HTML response.
 
             Args:
                 namespace (str): The namespace identifying the group or category of the query.
                 name (str): The specific name of the query to be executed.
 
             Returns:
                 HTMLResponse: The HTML formatted response containing the results of the query execution.
 
             Raises:
                 HTTPException: If the query cannot be found or fails to execute.
             """
-            content=self.query(namespace,name)
+            content = self.query(namespace, name)
             if not content:
                 raise HTTPException(status_code=500, detail="Could not create result")
 
             # Return the content as an HTML response
             return HTMLResponse(content)
-        
-    def query(self,namespace:str,name:str):
+
+    def query(self, namespace: str, name: str):
+        """ """
         endpoint_name = "wikidata"
         # content negotiation
         # Determine response format by extension in the name or Accept header
-        if '.' in name:
-            r_format = name.split('.')[-1]
-            name = name[:name.rfind('.')]
+        if "." in name:
+            r_format_str = name.split(".")[-1]
+            name = name[: name.rfind(".")]
         else:
-            r_format = "html"
+            r_format_str = "html"
 
         # Retrieve the SPARQL query string using the namespace and name.
         try:
             sparql_query = self.nqm.get_sparql(name, namespace, endpoint_name)
             qlod = self.nqm.query(
                 name=name, namespace=namespace, endpoint_name=endpoint_name
             )
             query = Query(name=name, query=sparql_query, lang="sparql")
         except Exception as e:
             # Handling specific exceptions can be more detailed based on what nqm.get_sparql and nqm.query can raise
             raise HTTPException(status_code=404, detail=str(e))
 
         # Format the results and generate HTML content
+        r_format = Format[r_format_str]
         content = self.nqm.format_result(
             qlod, query, r_format, endpoint_name=endpoint_name
         )
         return content
 
 
 class SnapQuerySolution(InputWebSolution):
@@ -100,7 +122,31 @@
 
         Calls the constructor of the base solution
         Args:
             webserver (SnapQueryWebServer): The webserver instance associated with this context.
             client (Client): The client instance this context is associated with.
         """
         super().__init__(webserver, client)  # Call to the superclass constructor
+        self.nqm = self.webserver.nqm
+        self.endpoint_name = "wikidata"
+
+    def configure_settings(self):
+        """
+        add additional settings
+        """
+        self.add_select("default Endpoint", list(self.nqm.endpoints.keys())).bind_value(
+            self, "endpoint_name"
+        )
+
+    def setup_ui(self):
+        """
+        setup my user interface
+        """
+        self.search = NamedQuerySearch(self)
+
+    async def home(
+        self,
+    ):
+        """Generates the home page with a selection of examples and
+        svg display
+        """
+        await self.setup_content_div(self.setup_ui)
```

### Comparing `snapquery-0.0.2/snapquery/version.py` & `snapquery-0.0.3/snapquery/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """
     Version handling for nicepdf
     """
 
     name = "snapquery"
     version = snapquery.__version__
     date = "2024-05-03"
-    updated = "2024-05-03"
+    updated = "2024-05-04"
     description = "Introduce Named Queries and Named Query Middleware to wikidata"
 
     authors = "Wolfgang Fahl"
 
     doc_url = "https://wiki.bitplan.com/index.php/snapquery"
     chat_url = "https://github.com/WolfgangFahl/snapquery/discussions"
     cm_url = "https://github.com/WolfgangFahl/snapquery"
```

### Comparing `snapquery-0.0.2/tests/test_endpoints.py` & `snapquery-0.0.3/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.2/tests/test_namedqueries.py` & `snapquery-0.0.3/tests/test_namedqueries.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.2/tests/test_restful_api.py` & `snapquery-0.0.3/tests/test_restful_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 """
 Created on 2024-05-03
 
 @author: wf
 """
-from snapquery.snapquery_webserver import SnapQueryWebServer
-from snapquery.snapquery_cmd import SnapQueryCmd
 from ngwidgets.webserver_test import WebserverTest
 
+from snapquery.snapquery_cmd import SnapQueryCmd
+from snapquery.snapquery_webserver import SnapQueryWebServer
 
-class TestRestFullApi(WebserverTest):
+
+class TestRestFulApi(WebserverTest):
     """
     test endpoint handling according to https://github.com/WolfgangFahl/snapquery/issues/1
     """
+
     def setUp(self, debug=True, profile=True):
         server_class = SnapQueryWebServer
         cmd_class = SnapQueryCmd
         WebserverTest.setUp(self, server_class, cmd_class, debug=debug, profile=profile)
 
-   
     def testDemoWebserver(self):
         """
         test API docs access
         """
         # self.debug=True
         html = self.getHtml("/docs")
         self.assertTrue("Swagger" in html)
-        
+
+    def testSparqlApi(self):
+        """
+        test the plaintext SPARQL API
+        """
+        for example in ["cats", "horses"]:
+            path = f"/sparql/wikidata-examples/{example}"
+            sparql_query = self.getHtml(path)
+            if self.debug:
+                print(sparql_query)
+            self.assertTrue("SELECT" in sparql_query)
+
     def testQueryApi(self):
-        for r_format in ["mediawiki","github","latex","html"]:
-            path=f"/query/wikidata-examples/cats.{r_format}"
-            html=self.getHtml(path)
+        """
+        test the RESTFul Query API
+        """
+        for r_format in ["mediawiki", "github", "latex", "html"]:
+            path = f"/query/wikidata-examples/cats.{r_format}"
+            html = self.getHtml(path)
             if self.debug:
                 print(html)
```

### Comparing `snapquery-0.0.2/.gitignore` & `snapquery-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.2/LICENSE` & `snapquery-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.2/README.md` & `snapquery-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.2/pyproject.toml` & `snapquery-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.2/PKG-INFO` & `snapquery-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snapquery
-Version: 0.0.2
+Version: 0.0.3
 Summary: snapquery: Introduce Named Queries and Named Query Middleware to wikidata
 Project-URL: Home, https://github.com/WolfgangFahl/snapquery
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/snapquery
 Project-URL: Source, https://github.com/WolfgangFahl/snapquery
 Author-email: Wolfgang Fahl <wf@WolfgangFahl.com>
 Maintainer-email: Wolfgang Fahl <wf@WolfgangFahl.com>
 License: Apache-2.0
```

