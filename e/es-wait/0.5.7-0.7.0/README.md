# Comparing `tmp/es_wait-0.5.7.tar.gz` & `tmp/es_wait-0.7.0.tar.gz`

## Comparing `es_wait-0.5.7.tar` & `es_wait-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.7/.coveragerc
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/__init__.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/_base.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/exceptions.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/exists.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/health.py
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/ilm.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/restore.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 es_wait-0.5.7/src/es_wait/task.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.7/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.7/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.7/README.md
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.7.0/.coveragerc
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 es_wait-0.7.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.7.0/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 es_wait-0.7.0/src/es_wait/_base.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.7.0/src/es_wait/exceptions.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 es_wait-0.7.0/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 es_wait-0.7.0/src/es_wait/health.py
+-rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 es_wait-0.7.0/src/es_wait/ilm.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 es_wait-0.7.0/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 es_wait-0.7.0/src/es_wait/restore.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 es_wait-0.7.0/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 es_wait-0.7.0/src/es_wait/task.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.7.0/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.7.0/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.7.0/README.md
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 es_wait-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.7.0/PKG-INFO
```

### Comparing `es_wait-0.5.7/src/es_wait/_base.py` & `es_wait-0.7.0/src/es_wait/_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,49 +9,70 @@
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
 logger = logging.getLogger('es_wait.Waiter')
 
 
 class Waiter:
-    """Class Definition"""
+    """Waiter Parent Class"""
 
     def __init__(
         self,
         client: 'Elasticsearch',
         pause: float = 9,  # The delay between checks
         timeout: float = -1,  # How long is too long
     ) -> None:
+        #: An :py:class:`Elasticsearch <elasticsearch.Elasticsearch>` client instance
         self.client = client
+        #: The delay between checks for completion
         self.pause = pause
+        #: The number of seconds before giving up. -1 means no timeout.
         self.timeout = timeout
         self.waitstr = 'for Waiter class to initialize'
 
     @property
     def now(self) -> datetime:
-        """Return the 'now' datetime"""
+        """
+        :getter: Returns the time 'now' in the UTC timezone
+        :type: datetime
+        """
         return datetime.now(timezone.utc)
 
     @property
     def check(self) -> bool:
-        """This will need to be redefined by each child class"""
+        """
+        This will be redefined by each child class
+
+        :getter: Returns if the check was complete
+        :type: bool
+        """
         return False
 
     def empty_check(self, name: str) -> None:
-        """Ensure that no empty values sneak through"""
+        """
+        Raise a :py:exc:`ValueError` if the instance attribute `name` is None. This
+        method literally just checks:
+
+          .. code-block:: python
+
+             if getattr(self, name) is None:
+
+        :param name: The name of an instance attribute.
+        """
         if getattr(self, name) is None:
             msg = f'Keyword arg {name} cannot be None'
             logger.critical(msg)
             raise ValueError(msg)
 
     def prettystr(self, *args, **kwargs) -> str:
         """
-        A (nearly) straight up wrapper for pprint.pformat, except that we provide our
-        own default values for 'indent' (2) and 'sort_dicts' (False). Primarily for
-        debug logging and showing more readable dictionaries.
+        A (nearly) straight up wrapper for :py:meth:`pprint.pformat()
+        <pprint.PrettyPrinter.pformat>`, except that we provide our own default values
+        for `indent` (`2`) and `sort_dicts` (`False`). Primarily for debug logging and
+        showing more readable dictionaries.
 
         'Return the formatted representation of object as a string. indent, width,
         depth, compact, sort_dicts and underscore_numbers are passed to the
         PrettyPrinter constructor as formatting parameters' (from pprint
         documentation).
         """
         defaults = [
@@ -65,19 +86,31 @@
         kw = {}
         for tup in defaults:
             key, default = tup
             kw[key] = kwargs[key] if key in kwargs else default
 
         return f"\n{pformat(*args, **kw)}"  # newline in front so it's always clean
 
-    def setup(self) -> None:
-        """Setup the waiter"""
+    def wait(self, frequency: int = 5) -> None:
+        """
+        This method is where the actual waiting occurs. Depending on what `frequency`
+        is set to, you should see `non-DEBUG` level logs no more than every `frequency`
+        seconds.
+
+        If :py:attr:`timeout` has been reached without :py:meth:`check` returning as
+        ``True``, then a :py:exc:`TimeoutError` will be raised.
 
-    def wait_for_it(self, frequency: int = 5) -> None:
-        """Do the actual waiting"""
+        If :py:meth:`check` returns ``False``, then the method will wait
+        :py:attr:`pause` seconds before calling :py:meth:`check` again.
+
+        Elapsed time will be logged every `frequency` seconds, when :py:meth:`check` is
+        ``True``, or when :py:attr:`timeout` is reached.
+
+        :param frequency: The number of seconds between log reports on progress.
+        """
         # Now with this mapped, we can perform the wait as indicated.
         start_time = self.now
         success = False
         logger.debug('Only logging every %s seconds', frequency)
         while True:
             elapsed = int((self.now - start_time).total_seconds())
             if elapsed == 0:
```

### Comparing `es_wait-0.5.7/src/es_wait/exists.py` & `es_wait-0.7.0/src/es_wait/exists.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,72 @@
-"""Entity Exists"""
+"""Entity Exists Waiter"""
 
 import typing as t
 import logging
 from ._base import Waiter
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
-logger = logging.getLogger('es_wait.Exists')
+logger = logging.getLogger(__name__)
 
-# pylint: disable=missing-docstring,too-many-arguments
+# pylint: disable=R0913
 
 
 class Exists(Waiter):
-    """Class Definition"""
+    """Wait for an entity to 'exist' according to Elasticsearch"""
 
     IDX_OR_DS = ['index', 'data_stream', 'datastream', 'idx', 'ds']
     TEMPLATE = ['index_template', 'template', 'tmpl']
     COMPONENT = ['component_template', 'component', 'comp']
 
     def __init__(
         self,
         client: 'Elasticsearch',
         pause: float = 1.5,
         timeout: float = 15,
         name: str = '',
-        kind: str = '',
+        kind: t.Literal[
+            'index',
+            'data_stream',
+            'index_template',
+            'template',
+            'component_template',
+            'component',
+        ] = '',
     ) -> None:
 
         super().__init__(client=client, pause=pause, timeout=timeout)
+        #: The entity name
         self.name = name
+        #: What kind of entity
         self.kind = kind
         self.empty_check('name')
         self.empty_check('kind')
         self.waitstr = f'for {self.kindmap} "{name}" to exist'
         logger.debug('Waiting %s...', self.waitstr)
 
     @property
     def check(self) -> bool:
         """
-        Check if the named entity exists, based on kind
+        Check if the named entity exists, based on :py:attr:`kind` and :py:attr:`name`.
+
+        For indices and data_streams, the call is :py:meth:`indices.exists()
+        <elasticsearch.client.IndicesClient.exists>`.
+
+        For index templates, the call is :py:meth:`indices.exists_index_template()
+        <elasticsearch.client.IndicesClient.exists_index_template>`.
+
+        For component templates, it is :py:meth:`cluster.exists_component_template()
+        <elasticsearch.client.ClusterClient.exists_component_template>`.
+
+        The return value is the result of whichever call is made.
+
+        :getter: Returns if the check was complete
+        :type: bool
         """
         doit = {
             'index or data_stream': {
                 'func': self.client.indices.exists,
                 'kwargs': {'index': self.name},
             },
             'index template': {
@@ -60,15 +83,18 @@
 
     @property
     def kindmap(
         self,
     ) -> t.Literal[
         'index or datastream', 'index template', 'component template', 'FAIL'
     ]:
-        """This is a little way to ensure many possibilities come down to one"""
+        """
+        This method helps map :py:attr:`kind` to the proper 'exists' API call, as well
+        as accurately log what we're checking in :py:meth:`wait` logging.
+        """
         if self.kind in self.IDX_OR_DS:
             return 'index or data_stream'
         if self.kind in self.TEMPLATE:
             return 'index template'
         if self.kind in self.COMPONENT:
             return 'component template'
         logger.error('%s is not an acceptable value for kind', self.kind)
```

### Comparing `es_wait-0.5.7/src/es_wait/ilm.py` & `es_wait-0.7.0/src/es_wait/ilm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""ILM Phase and Step Checks"""
+"""ILM Phase and Step Check Waiters"""
 
 import typing as t
 import logging
 from dotmap import DotMap
 from elasticsearch8.exceptions import NotFoundError
 from ._base import Waiter
 from .exceptions import IlmWaitError
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
-logger = logging.getLogger('es_wait.IndexLifecycle')
+logger = logging.getLogger(__name__)
 
 # pylint: disable=R0913
 
 
 class IndexLifecycle(Waiter):
     """ILM Step and Phase Parent Class"""
 
@@ -23,22 +23,23 @@
         client: 'Elasticsearch',
         pause: float = 1,
         timeout: float = -1,
         name: t.Union[str, None] = None,
     ) -> None:
 
         super().__init__(client=client, pause=pause, timeout=timeout)
+        #: The index name
         self.name = name
         self.empty_check('name')
 
     def get_explain_data(self) -> t.Union[t.Dict, None]:
         """
-        Calls `client.indices.`
-        :py:meth:`~.elasticsearch.client.IlmClient.explain_lifecycle` with an index
-        name and returns the resulting response.
+        This method calls :py:meth:`ilm.explain_lifecycle()
+        <elasticsearch.client.IlmClient.explain_lifecycle>` with :py:attr:`name` and
+        returns the resulting response.
         """
         try:
             resp = dict(self.client.ilm.explain_lifecycle(index=self.name))
             logger.debug('ILM Explain response: %s', self.prettystr(resp))
         except NotFoundError as exc:
             msg = (
                 f'Datastream/Index Name changed. {self.name} was not found. '
@@ -67,35 +68,39 @@
         self,
         client: 'Elasticsearch',
         pause: float = 1,
         timeout: float = -1,
         name: t.Union[str, None] = None,
         phase: t.Union[str, None] = None,
     ) -> None:
-        self.logger = logging.getLogger('es_wait.IlmPhase')
         super().__init__(client=client, pause=pause, timeout=timeout, name=name)
+        #: The target ILM phase
         self.phase = phase
         self.empty_check('phase')
         self.waitstr = (
             f'for "{self.name}" to complete ILM transition to phase "{self.phase}"'
         )
         logger.debug('Waiting %s...', self.waitstr)
 
     @property
     def check(self) -> bool:
         """
-        Check for ILM phase change completion.  It will return ``True`` if the expected
-        phase and the actually collected phase match.
+        Collect ILM explain data from :py:meth:`get_explain_data()`, and check for ILM
+        phase change completion.  It will return ``True`` if the expected phase and the
+        actually collected phase match.
 
-        Upstream callers need to try/catch any of KeyError (index name changed),
-        :py:exc:`~.elasticsearch.exceptions.NotFoundError`, and
+        Upstream callers need to try/catch any of :py:exc:`KeyError` (index name
+        changed), :py:exc:`NotFoundError <elasticsearch.exceptions.NotFoundError>`, and
         :py:exc:`~.es_wait.exceptions.IlmWaitError`.
 
         We cannot not be responsible for retrying with a changed name as it's not in
         our scope as a "waiter"
+
+        :getter: Returns if the check was complete
+        :type: bool
         """
         explain = DotMap(self.get_explain_data())
         return bool(explain.phase == self.phase)
 
 
 class IlmStep(IndexLifecycle):
     """
@@ -108,37 +113,40 @@
     def __init__(
         self,
         client: 'Elasticsearch',
         pause: float = 1,
         timeout: float = -1,
         name: t.Union[str, None] = None,
     ) -> None:
-        self.logger = logging.getLogger('es_wait.IlmStep')
         super().__init__(client=client, pause=pause, timeout=timeout, name=name)
         self.waitstr = f'for "{self.name}" to complete the current ILM step'
 
     @property
     def check(self) -> bool:
         """
-        Check for ILM step completion.  It will return ``True`` if the step and
-        action values are both ``complete``
+        Collect ILM explain data from :py:meth:`get_explain_data()`, and check for ILM
+        step completion.  It will return ``True`` if the step and action values are
+        both ``complete``
 
-        Upstream callers need to try/catch any of KeyError (index name changed),
-        :py:exc:`~.elasticsearch.exceptions.NotFoundError`, and
+        Upstream callers need to try/catch any of :py:exc:`KeyError` (index name
+        changed), :py:exc:`NotFoundError <elasticsearch.exceptions.NotFoundError>`, and
         :py:exc:`~.es_wait.exceptions.IlmWaitError`.
 
         We cannot not be responsible for retrying with a changed name as it's not in
         our scope as a "waiter"
+
+        :getter: Returns if the check was complete
+        :type: bool
         """
         explain = DotMap(action='no', step='no')  # Set defaults so the return works
         try:
             explain = DotMap(self.get_explain_data())
         except NotFoundError as err:
             if self.client.indices.exists(index=self.name):
                 msg = (
                     f'NotFoundError encountered. However, index {self.name} has been '
                     f'confirmed to exist, so we continue to retry...'
                 )
-                self.logger.debug(msg)
+                logger.debug(msg)
             else:
                 raise err
         return bool(explain.action == 'complete' and explain.step == 'complete')
```

### Comparing `es_wait-0.5.7/src/es_wait/relocate.py` & `es_wait-0.7.0/src/es_wait/relocate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,110 @@
-"""Relocate Check"""
+"""Index Relocation Waiter"""
 
 import typing as t
 import logging
 from ._base import Waiter
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
-logger = logging.getLogger('es_wait.Relocate')
+logger = logging.getLogger(__name__)
 
-# pylint: disable=missing-docstring,too-many-arguments
+# pylint: disable=R0913
 
 
 class Relocate(Waiter):
+    """Wait for an index to relocate"""
 
     def __init__(
         self,
         client: 'Elasticsearch',
         pause: float = 9,
         timeout: float = -1,
         name: str = None,
     ) -> None:
         super().__init__(client=client, pause=pause, timeout=timeout)
+        #: The index name
         self.name = name
         self.empty_check('name')
         self.waitstr = f'for index "{self.name}" to finish relocating'
         logger.debug('Waiting %s...', self.waitstr)
 
     @property
     def check(self) -> bool:
         """
-        This function calls `client.cluster.`
-        :py:meth:`~.elasticsearch.client.ClusterClient.state` with a given index to
-        check if all of the shards for that index are in the ``STARTED`` state. It will
-        return ``True`` if all primary and replica shards are in the ``STARTED`` state,
-        and it will return ``False`` if any shard is in a different state.
+        This method gets the value from property :py:meth:`finished_state` and returns
+        that value.
+
+        :getter: Returns if the check was complete
+        :type: bool
         """
         finished = self.finished_state
         if finished:
             logger.debug('Relocate Check for index: "%s" has passed.', self.name)
         return finished
 
     @property
     def finished_state(self) -> bool:
         """
         Return the boolean state of whether all shards in the index are 'STARTED'
 
-        The all() function returns True if all items in an iterable are true,
+        The :py:func:`all` function returns True if all items in an iterable are true,
         otherwise it returns False. We use it twice here, nested.
+
+        Gets this from property :py:meth:`routing_table`
+
+        :getter: Returns whether the shards are all ``STARTED``
+        :type: bool
         """
         return all(
             all(shard['state'] == "STARTED" for shard in shards)
             for shards in self.routing_table.values()
         )
 
     @property
     def routing_table(self) -> t.Dict:
+        """
+        This method calls :py:meth:`cluster.state()
+        <elasticsearch.client.ClusterClient.state>` to get the shard routing table. As
+        the cluster state API result can be quite large, it uses a ``filter_path`` to
+        drastically reduce the result size. This path is:
+
+          .. code-block:: python
+
+             f'routing_table.indices.{self.name}'
+
+        It will raise a :py:exc:`ValueError` on an exception to this API call.
+
+        It will then try to return
+
+          .. code-block:: python
+
+             return result['routing_table']['indices'][self.name]['shards']
+
+        And will raise a :py:exc:`KeyError` if one of those keys is not found.
+
+        :getter: Returns the shard routing table
+        :type: bool
+        """
         msg = f'Unable to get routing table data from cluster state for {self.name}'
-        # Using filter_path drastically reduces the result size
         fpath = f'routing_table.indices.{self.name}'
         try:
             result = self.client.cluster.state(index=self.name, filter_path=fpath)
             # {
             #     "routing_table": {
             #         "indices": {
             #         "SELF.NAME": {
             #             "shards": {
             #             "0": [
             #                   {
             #                    "state": "SHARD_STATE",
         except Exception as exc:
             logger.critical(msg)
             raise ValueError(msg) from exc
+
+        # Actually return the result
         try:
             return result['routing_table']['indices'][self.name]['shards']
         except KeyError as err:
             logger.critical(msg)
             raise KeyError(msg) from err
```

### Comparing `es_wait-0.5.7/src/es_wait/snapshot.py` & `es_wait-0.7.0/src/es_wait/snapshot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,114 @@
-"""Snapshot Check"""
+"""Snapshot Completion Waiter"""
 
 import typing as t
 import logging
 from ._base import Waiter
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
-logger = logging.getLogger('es_wait.Snapshot')
+logger = logging.getLogger(__name__)
 
-# pylint: disable=missing-docstring,too-many-arguments
+# pylint: disable=R0913
 
 
 class Snapshot(Waiter):
-    ACTIONS: t.Optional[str] = None
+    """Wait for a snapshot to complete"""
 
     def __init__(
         self,
         client: 'Elasticsearch',
         pause: float = 9,
         timeout: float = -1,
         snapshot: str = None,
         repository: str = None,
     ) -> None:
         super().__init__(client=client, pause=pause, timeout=timeout)
+        #: The snapshot name
         self.snapshot = snapshot
+        #: The repository name
         self.repository = repository
         self.empty_check('snapshot')
         self.empty_check('repository')
         self.waitstr = f'for snapshot "{self.snapshot}" to complete'
         logger.debug('Waiting %s...', self.waitstr)
 
     @property
     def check(self) -> bool:
         """
-        This function calls `client.snapshot.`
-        :py:meth:`~.elasticsearch.client.SnapshotClient.get` and tests to see whether
-        the snapshot is complete, and if so, with what status. It will log errors
-        according to the result. If the snapshot is still ``IN_PROGRESS``, it will
-        return ``False``. ``SUCCESS`` will be an ``INFO`` level message, ``PARTIAL``
-        nets a ``WARNING`` message, ``FAILED`` is an ``ERROR``, message, and all others
-        will be a ``WARNING`` level message.
+        Get the state of the snapshot from :py:meth:`snapstate` to determine if the
+        snapshot is complete, and if so, with what status.
+
+        If the state is ``IN_PROGRESS``, this method will return ``False``.
+
+        For all other states, it calls :py:meth:`log_completion` to log the final
+        result. It then returns ``True``.
+
+        :getter: Returns if the check was complete
+        :type: bool
         """
         state = self.snapstate['snapshots'][0]['state']
         retval = True
         if state == 'IN_PROGRESS':
             retval = False
         if retval:
             self.log_completion(state)
         return retval
 
     @property
     def snapstate(self) -> t.Dict:
+        """
+        This function calls
+        :py:meth:`snapshot.get() <elasticsearch.client.SnapshotClient.get>` to get the
+        current state of the snapshot.
+
+        :getter: Returns the state of the snapshot
+        :type: bool
+        """
         result = {}
         try:
             result = self.client.snapshot.get(
                 repository=self.repository, snapshot=self.snapshot
             )
         except Exception as err:
             raise ValueError(
                 f'Unable to obtain information for snapshot "{self.snapshot}" in '
                 f'repository "{self.repository}". Error: {self.prettystr(err)}'
             ) from err
         return result
 
     def log_completion(self, state: str) -> None:
+        """
+        Log completion based on ``state``
+
+        If the snapshot state is:
+
+        .. list-table:: Snapshot States & Logs
+           :widths: 15 15 70
+           :header-rows: 1
+
+           * - State
+             - Log Level
+             - Message
+           * - ``SUCCESS``
+             - ``INFO``
+             - Snapshot [`name`] successfully completed.
+           * - ``PARTIAL``
+             - ``WARNING``
+             - Snapshot [`name`] completed with state PARTIAL.
+           * - ``FAILED``
+             - ``ERROR``
+             - Snapshot [`name`] completed with state FAILED.
+           * - [`other`]
+             - ``WARNING``
+             - Snapshot [`name`] completed with state: [`other`]
+
+        :param state: The snapshot state
+        """
         if state == 'SUCCESS':
             logger.info('Snapshot %s successfully completed.', self.snapshot)
         elif state == 'PARTIAL':
             logger.warning('Snapshot %s completed with state PARTIAL.', self.snapshot)
         elif state == 'FAILED':
             logger.error('Snapshot %s completed with state FAILED.', self.snapshot)
         else:
```

### Comparing `es_wait-0.5.7/src/es_wait/task.py` & `es_wait-0.7.0/src/es_wait/task.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,117 @@
-"""Task Check"""
+"""Task Completion Waiter"""
 
 import typing as t
 import logging
 from time import localtime, strftime
 from dotmap import DotMap
 from ._base import Waiter
 
-# from .args import TaskArgs
-
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
-logger = logging.getLogger('es_wait.Task')
+logger = logging.getLogger(__name__)
 
-# pylint: disable=missing-docstring,too-many-arguments
+# pylint: disable=R0913
 
 
 class Task(Waiter):
-    ACTIONS = ['forcemerge', 'reindex', 'update_by_query']
+    """Wait for a task to complete"""
 
     def __init__(
         self,
         client: 'Elasticsearch',
         pause: float = 9,
         timeout: float = -1,
         action: t.Literal['forcemerge', 'reindex', 'update_by_query'] = None,
         task_id: str = None,
     ) -> None:
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.action = action
+        #: The task identification string
         self.task_id = task_id
         self.empty_check('action')
         self.empty_check('task_id')
+        #: The :py:meth:`tasks.get() <elasticsearch.client.TasksClient.get>` results
         self.task_data = None
+        #: The contents of :py:attr:`task_data['task'] <task_data>`
         self.task = None
         self.waitstr = f'for the "{self.action}" task to complete'
         logger.debug('Waiting %s...', self.waitstr)
 
     @property
     def check(self) -> bool:
         """
-        This function calls `client.tasks.`
-        :py:meth:`~.elasticsearch.client.TasksClient.get` with the provided
-        ``task_id``.  If the task data contains ``'completed': True``, then it will
-        return ``True``. If the task is not completed, it will log some information
-        about the task and return ``False``
+        This function calls :py:meth:`tasks.get()
+        <elasticsearch.client.TasksClient.get>` with the provided ``task_id`` and sets
+        the values for :py:attr:`task_data` and :py:attr:`task` as part of its
+        execution pipeline.
+
+        It then calls :py:meth:`reindex_check` to see if it is a reindex operation.
+
+        Finally, it returns whatever :py:meth:`task_complete` returns.
+
+        :getter: Returns if the check was complete
+        :type: bool
         """
-        # The properties for TaskArgs
+        # The properties for task_data
         # TASK_DATA
         # self.task_data.response = {}
         # self.task_data.completed = False
         # self.task_data.task = {} -> Becomes TASK
         # TASK
         # self.task.action = str
         # self.task.description = str
         # self.task.running_time_in_nanos = 0
 
         try:
-            # self.task_data = TaskArgs(
-            #     settings=self.client.tasks.get(task_id=self.task_id)
-            # )
             self.task_data = DotMap(self.client.tasks.get(task_id=self.task_id))
         except Exception as err:
             msg = (
                 f'Unable to obtain task information for task_id "{self.task_id}". '
                 f'Exception {self.prettystr(err)}'
             )
             raise ValueError(msg) from err
         self.task = self.task_data.task
         self.reindex_check()
         return self.task_complete
 
     def reindex_check(self) -> None:
+        """
+        Check to see if the task is a reindex operation. The task may be "complete" but
+        had one or more failures. Raise a :py:exc:`ValueError` exception if errors were
+        encountered.
+
+        Gets data from :py:attr:`task` and :py:attr:`task_data`.
+        """
         if self.task.action == 'indices:data/write/reindex':
-            logger.debug("It's a REINDEX task")
-            logger.debug('TASK_DATA: %s', self.prettystr(self.task_data.toDict()))
-            logger.debug(
-                'TASK_DATA keys: %s',
-                self.prettystr(list(self.task_data.toDict().keys())),
-            )
+            # logger.debug("It's a REINDEX task")
+            # logger.debug('TASK_DATA: %s', self.prettystr(self.task_data.toDict()))
+            # logger.debug(
+            #     'TASK_DATA keys: %s',
+            #     self.prettystr(list(self.task_data.toDict().keys())),
+            # )
             if self.task_data.response.failures:
                 if len(self.task_data.response.failures) > 0:
                     msg = (
                         f'Failures found in the {self.action} response: '
                         f'{self.prettystr(self.task_data.response["failures"])}'
                     )
                     raise ValueError(msg)
 
     @property
     def task_complete(self) -> bool:
+        """
+        Process :py:attr:`task` and :py:attr:`task_data` to see if the task has
+        completed, or is still running.
+
+        If :py:attr:`task_data` contains ``'completed': True``, then it will
+        return ``True``. If the task is not completed, it will log some information
+        about the task and return ``False``
+        """
         running_time = 0.000000001 * self.task.running_time_in_nanos
         logger.debug('Running time: %s seconds', running_time)
         if self.task_data.completed:
             completion_time = (running_time * 1000) + self.task['start_time_in_millis']
             time_string = strftime(
                 '%Y-%m-%dT%H:%M:%S', localtime(completion_time / 1000)
             )
```

### Comparing `es_wait-0.5.7/.gitignore` & `es_wait-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.7/LICENSE` & `es_wait-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.7/PKG-INFO` & `es_wait-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.5.7
+Version: 0.7.0
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```

