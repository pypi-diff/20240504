# Comparing `tmp/re-ircbot-1.7.0.tar.gz` & `tmp/re_ircbot-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re-ircbot-1.7.0.tar", last modified: Sat Aug 12 00:06:56 2023, max compression
+gzip compressed data, was "re_ircbot-2.0.0.dev0.tar", last modified: Sat May  4 15:04:21 2024, max compression
```

## Comparing `re-ircbot-1.7.0.tar` & `re_ircbot-2.0.0.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-12 00:06:56.188473 re-ircbot-1.7.0/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-12 00:06:56.188473 re-ircbot-1.7.0/IrcBot/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-12 00:06:49.000000 re-ircbot-1.7.0/IrcBot/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    54162 2023-08-12 00:06:49.000000 re-ircbot-1.7.0/IrcBot/bot.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5408 2023-08-12 00:06:49.000000 re-ircbot-1.7.0/IrcBot/dcc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1658 2023-08-12 00:06:49.000000 re-ircbot-1.7.0/IrcBot/message.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1902 2023-08-12 00:06:49.000000 re-ircbot-1.7.0/IrcBot/shortestPrefix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11315 2023-08-12 00:06:49.000000 re-ircbot-1.7.0/IrcBot/sqlitedb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16449 2023-08-12 00:06:49.000000 re-ircbot-1.7.0/IrcBot/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-08-12 00:06:49.000000 re-ircbot-1.7.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14056 2023-08-12 00:06:56.188473 re-ircbot-1.7.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2023-08-12 00:06:49.000000 re-ircbot-1.7.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-12 00:06:56.188473 re-ircbot-1.7.0/re_ircbot.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14056 2023-08-12 00:06:56.000000 re-ircbot-1.7.0/re_ircbot.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      315 2023-08-12 00:06:56.000000 re-ircbot-1.7.0/re_ircbot.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-12 00:06:56.000000 re-ircbot-1.7.0/re_ircbot.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2023-08-12 00:06:56.000000 re-ircbot-1.7.0/re_ircbot.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2023-08-12 00:06:56.000000 re-ircbot-1.7.0/re_ircbot.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-12 00:06:56.188473 re-ircbot-1.7.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1858 2023-08-12 00:06:49.000000 re-ircbot-1.7.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 15:04:21.306030 re_ircbot-2.0.0.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14058 2024-05-04 15:04:21.306030 re_ircbot-2.0.0.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 15:04:21.306030 re_ircbot-2.0.0.dev0/ircbot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    54469 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/dcc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1658 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/message.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/shortest_prefix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/sqlitedb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16430 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 15:04:21.306030 re_ircbot-2.0.0.dev0/re_ircbot.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14058 2024-05-04 15:04:21.000000 re_ircbot-2.0.0.dev0/re_ircbot.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      319 2024-05-04 15:04:21.000000 re_ircbot-2.0.0.dev0/re_ircbot.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-04 15:04:21.000000 re_ircbot-2.0.0.dev0/re_ircbot.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-05-04 15:04:21.000000 re_ircbot-2.0.0.dev0/re_ircbot.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-04 15:04:21.000000 re_ircbot-2.0.0.dev0/re_ircbot.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-04 15:04:21.306030 re_ircbot-2.0.0.dev0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/setup.py
```

### Comparing `re-ircbot-1.7.0/IrcBot/bot.py` & `re_ircbot-2.0.0.dev0/ircbot/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 #                                                                       #
 #########################################################################
 #  Depends on: `pip3 install -r requirements.txt`                       #
 #                                                                       #
 #########################################################################
 
 
+import asyncio
 import inspect
 import random
 import re
 import socket
 from copy import copy, deepcopy
 from functools import partial
 from math import ceil
 from pathlib import Path
+from typing import Awaitable, Callable, TypeAlias
 
-import trio
-import trio_asyncio
 from cachetools import TTLCache
 
-from IrcBot import dcc, utils
-from IrcBot.message import Message, RawMessage, ReplyIntent
-from IrcBot.sqlitedb import DB
-from IrcBot.utils import debug, log, logger
+from ircbot import dcc, utils
+from ircbot.message import Message, RawMessage, ReplyIntent
+from ircbot.sqlitedb import DB
+from ircbot.utils import debug, log, logger
 
 Message = Message
 ReplyIntent = ReplyIntent
 RawMessage = RawMessage
 
 BUFFSIZE = 2048
 MAX_MESSAGE_LEN = 410
@@ -103,26 +103,26 @@
             if not (k.startswith("_") or k in ["esc", "COLORS", "colors", "getcolors", "random"])
         ]
 
     def __str__(self):
         return self.str
 
 
-class dbOperation(object):
+class DBOperation(object):
     ADD = 1
     UPDATE = 0
     REMOVE = -1
 
     def __init__(self, data={}, id={}, op=UPDATE):
         self.data = data
         self.id = id
         self.op = op
 
 
-class tempData(object):
+class TempData(object):
     def __init__(self):
         """Initializes a temporary data object that can be retrieved from the
         same user and channel."""
         self.data = {}
 
     def push(self, msg, data):
         """Stores any data for the current nick and channel.
@@ -143,15 +143,15 @@
         """Returns data for user channel of the given message.
 
         :param msg: Message object
         """
         return self.data[(msg.channel, msg.sender_nick)]
 
 
-class persistentData(object):
+class PersistentData(object):
     def __init__(self, filename, name, keys):
         """__init__.
 
         :param name: Name of the table
         :param keys: List of strings. Names for each column
         :param blockDB: If true the database connection will be kept open. This can increase performance but you will have to shut down the bot in case you want to edit the database file manually.
 
@@ -167,104 +167,145 @@
         self.fetch()
 
     def initDB(self, filename):
         self.db = DB(filename, self.name, self.keys, self.blockDB)
 
     def fetch(self):
         """fetches the list of dicts/items with ids."""
-        self.data = self.db.getAllWithId()
+        self.data = self.db.get_all_with_id()
         return self.data
 
     def push(self, items):
         """push. Add new items to the table.
 
         :param items: list or single dict.
         """
         if type(items) == list:
             for item in items:
                 self.push(item)
         else:
-            self._queue.append(dbOperation(data=items, op=dbOperation.ADD))
+            self._queue.append(DBOperation(data=items, op=DBOperation.ADD))
 
     def pop(self, id):
         """Removes the row based on the id. (You can see with self.data)
 
         :param id: int
         """
         assert type(id) == int, "id needs to be an int!"
-        self._queue.append(dbOperation(id=id, op=dbOperation.REMOVE))
+        self._queue.append(DBOperation(id=id, op=DBOperation.REMOVE))
 
     def update(self, id, item):
         """update.
 
         :param id: id of item to update, change.
         :param item: New item to replace with. This dict doesn't need to have all keys/columns, just the ones to be changed.
         """
         assert type(item) == dict, "item must be either list or dict"
         assert type(id) == int, "id needs to be an int!"
-        self._queue.append(dbOperation(id=id, data=item, op=dbOperation.UPDATE))
+        self._queue.append(DBOperation(id=id, data=item, op=DBOperation.UPDATE))
 
     def clear(self):
         """Clear all the proposed modifications."""
         self._queue = []
 
 
-class IrcBot(object):
-    """IrcBot."""
+class TCPStream:
+    def __init__(self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
+        self.reader = reader
+        self.writer = writer
+
+    async def send_all(self, data: bytes):
+        self.writer.write(data)
+        await self.writer.drain()
+
+    async def recv(self, n: int = 2048) -> bytes:
+        return await self.reader.read(n)
+
+    async def aclose(self):
+        self.writer.close()
+        await self.writer.wait_closed()
+
+    def close(self):
+        self.writer.close()
+
+
+class IrcBot:
+    AsyncCallback = Callable[["IrcBot"], Awaitable[None]]
+    Sendable: TypeAlias = str | Message | Color | list[str | Message | Color]
+
+    nick: str
+    password: str
+    server_password: str | None
+    username: str
+    host: str
+    port: int
+    channels: list[str] | str
+    use_sasl: bool
+    use_ssl: bool
+    tables: list[PersistentData]
+    delay: int
+    accept_join_from: list[str]
+    custom_handlers: dict
+    strip_messages: bool
+    dcc_ports: list[int]
+    dcc_host: str | None
+    dcc_announce_host: str | None
+    middleware: list[Callable]
+    _dcc_busy_ports: dict
+    connected: bool
+    server_channels: dict
+    channel_names: dict
+    replyIntents: dict
+    ping_delay: int
+    is_running_with_callback: bool
+    async_callback: AsyncCallback | None
+    retry_connecting: bool
+    message_queue: asyncio.Queue[str]
+    db_operation_queue: asyncio.Queue[PersistentData]
+    stream: TCPStream
 
     def __init__(
         self,
-        host,
-        port=6667,
-        nick="bot",
-        channels=None,
-        username=None,
-        password="",
-        server_password="",
-        use_sasl=False,
-        use_ssl=False,
-        delay=False,
-        accept_join_from=None,
-        tables=None,
-        custom_handlers=None,
-        strip_messages=True,
-        dcc_ports=None,
-        dcc_host=False,
-        dcc_announce_host=None,
+        host: str,
+        port: int = 6667,
+        nick: str = "bot",
+        channels: list[str] | str | None = None,
+        username: str | None = None,
+        password: str = "",
+        server_password: str = "",
+        use_sasl: bool = False,
+        use_ssl: bool = False,
+        delay: int = 0,
+        accept_join_from: list[str] | None = None,
+        tables: list[PersistentData] | None = None,
+        custom_handlers: dict | None = None,
+        strip_messages: bool = True,
+        dcc_ports: list[int] | None = None,
+        dcc_host: str | None = None,
+        dcc_announce_host: str | None = None,
     ):
         """Creates a bot instance joining to the channel if specified.
 
         :param host: str. Server hostname. ex: "irc.freenode.org"
-        :param port: int. Server port. default 6665
+        :param port: int. Server port.
         :param nick: str. Bot nickname. If this is set but username is not set then this will be used as the username for authentication if password is set.
-        :param channel: List of strings of channels to join or string for a single channel. You can leave this empty can call .join manually.
-        :param username: str. Username for authentication.
+        :param channels: list[str] or None. List of strings of channels to join or string for a single channel. You can leave this empty can call .join manually.
+        :param username: str or None. Username for authentication.
         :param password: str. Password for authentication.
         :param server_password: str. Authenticate with the server.
         :param use_sasl: bool. Use sasl autentication. (Still not working. Don't use this!)
         :param delay: int. Delay after nickserv authentication
-        :param accept_join_from: str. Who to accept invite command from ([])
-        :param tables: List of persistentData to be registered on the bot.
+        :param accept_join_from: list[str] or None. Who to accept invite command from ([])
+        :param tables: list[persistentData] or None. List of persistentData to be registered on the bot.
         :param strip_messages: bool. Should messages be stripped (for *_with_message decorators)
-        :param custom_handlers:{type: function, ...} Dict with function values to be called to handle custom server messages. Possible types (keys) are:
-            type             kwargs
-            'privmsg' -> {'nick', 'channel', 'text'}
-            'ping' -> {'ping'}
-            'names' -> {'channel', 'names'}
-            'channel' -> {'channel', 'channeldescription'}
-            'join' -> {'nick', 'channel'}
-            'quit' -> {'nick', 'text'}
-            'part' -> {'nick', 'channel'}
-            'dccsend' -> {'nick', 'filename', 'ip', 'port', 'size', 'token'}
-        :param dcc_ports: list of ports numbers to use for dcc
-        :param dcc_host: ip address to bind to for passive dcc file receiving and dcc send.
-        :param dcc_announce_host: ip address to announce for passive dcc file receiving and dcc send.
-        type: str ip or None to bind to the wildcard address. Default will try to guess (LAN IP)
+        :param custom_handlers: dict or None. Custom handlers to be added to the bot.
+        :param dcc_ports: list[int] or None. List of ports numbers to use for dcc
+        :param dcc_host: str or None. ip address to bind to for passive dcc file receiving and dcc send. type: str ip or None to bind to the wildcard address. Default will try to guess (LAN IP)
+        :param dcc_announce_host: str or None. ip address to announce for passive dcc file receiving and dcc send.
         """
-
         if channels is None:
             channels = []
         if accept_join_from is None:
             accept_join_from = []
         if tables is None:
             tables = []
         if custom_handlers is None:
@@ -273,15 +314,15 @@
             dcc_ports = list(range(4990, 5000))
         if dcc_announce_host is None:
             dcc_announce_host = dcc_host
 
         self.nick = nick
         self.password = password
         self.server_password = server_password
-        self.username = username
+        self.username = username or self.nick
         self.host = host
         self.port = port
         self.channels = channels
         self.use_sasl = use_sasl
         self.use_ssl = use_ssl
         self.tables = tables
         self.delay = delay
@@ -306,249 +347,228 @@
         self.connected = False
         self.server_channels = {}
         self.channel_names = {}
 
         if utils.arg_commands_with_message:
             new_commands = deepcopy(utils._defined_command_dict)
             new_commands.update(utils.arg_commands_with_message)
-            utils.setCommands(new_commands, prefix=utils.command_prefix)
+            utils.set_commands(new_commands, prefix=utils.command_prefix)
 
-        (
-            self.send_message_channel,
-            self.receive_message_channel,
-            self.send_db_operation_channel,
-            self.receive_db_operation_channel,
-        ) = [None] * 4
+        self.message_queue = asyncio.Queue()
+        self.db_operation_queue = asyncio.Queue()
         self.replyIntents = {}
 
         self.ping_delay = 30  # seconds
 
         self.is_running_with_callback = False
         self.async_callback = None
         self.retry_connecting = False
-        self.nursery = None
-
-        if not self.username:
-            self.username = self.nick
 
     async def hot_reload(self):
         """Reload the handlers."""
         utils._hot_reload()
         self.custom_handlers.update(utils.custom_handlers)
         if utils.arg_commands_with_message:
             new_commands = deepcopy(utils._defined_command_dict)
             new_commands.update(utils.arg_commands_with_message)
-            utils.setCommands(new_commands, prefix=utils.command_prefix)
+            utils.set_commands(new_commands, prefix=utils.command_prefix)
 
-    async def _mainloop(self, async_callback=None):
-        self.is_running_with_callback = True if async_callback else None
+    async def _mainloop(self, async_callback: AsyncCallback):
+        self.is_running_with_callback = bool(async_callback)
         self.async_callback = async_callback
         while True:
-            (
-                self.send_message_channel,
-                self.receive_message_channel,
-            ) = trio.open_memory_channel(0)
-            (
-                self.send_db_operation_channel,
-                self.receive_db_operation_channel,
-            ) = trio.open_memory_channel(0)
             try:
-                async with trio.open_nursery() as nursery:
-                    self.nursery = await nursery.start(self._main_task)
+                await self._main_task()
             except (BotConnectionError, socket.gaierror):
-                log(f"Attempting to reconnect in {self.ping_delay}...")
-                await trio.sleep(self.ping_delay)
+                log(f"Attempting to reconnect in {self.ping_delay / 2}...")
+                await asyncio.sleep(self.ping_delay / 2)
 
-    async def _main_task(self, task_status=trio.TASK_STATUS_IGNORED):
-        async with trio.open_nursery() as nursery:
-            with trio.CancelScope() as scope:
-                task_status.started(scope)
-                if self.async_callback is None:
-                    self.nursery = nursery.start_soon(self.connect)
-                else:
-                    self.nursery = nursery.start_soon(self.start_with_callback)
+    async def _main_task(self):
+        if self.async_callback is None:
+            await self.connect()
+        else:
+            await self.start_with_callback()
 
-    def runWithCallback(self, async_callback):
+    def run_with_callback(self, async_callback: AsyncCallback):
         """starts the bot with an async callback.
 
         Useful if you want to use bot.send without user interaction.
         param: async_callback: async function to be called.
         """
-        trio_asyncio.run(self._mainloop, async_callback)
+        asyncio.run(self._mainloop(async_callback))
 
     async def start_with_callback(self):
-        async with trio.open_nursery() as nursery:
-            nursery.start_soon(self.connect)
-            nursery.start_soon(self._wait_and_async_cb_task)
+        await asyncio.gather(self.connect(), self._wait_and_async_cb_task())
 
     async def _wait_and_async_cb_task(self):
         while not self.connected:
-            await trio.sleep(1)
-        await self.async_callback(self)
+            await asyncio.sleep(1)
+        if self.async_callback:
+            await self.async_callback(self)
 
     def add_middleware(self, method):
         """Adds a middleware to run before every command.
 
         :param method callable: Async method that will receive the this bot instance and the incoming message object for every command handling event. If this methods doesn't return True, then the callback execution stops.
         """
         self.middleware.append(method)
 
-    def run(self, async_callback=None):
+    def run(self, async_callback: AsyncCallback):
         """Simply starts the bot.
 
         param: async_callback: async function to be called.
         """
-        trio_asyncio.run(self._mainloop, async_callback)
+        asyncio.run(self._mainloop(async_callback))
 
     async def sleep(self, time):
         """Waits for time.
 
         Asynchronous wrapper for trip.sleep
         """
-        await trio.sleep(time)
+        await asyncio.sleep(time)
 
-    async def ping_confirmation(self, s):
+    async def ping_confirmation(self, stream: TCPStream):
         MAX = 10
         c = 0
         log("AWAITING PING CONFIRMATION.....")
-        async for data in s:
+        while True:
+            data = await stream.recv()
             data = data.decode("utf-8")
             for msg in data.split("\r\n"):
                 debug("RECV --------- " + msg)
                 if c > MAX:
                     return
                 if "001 " + self.nick + " :" in msg:
                     return
                 if data.find("PING") != -1 and len(data.split(":")) >= 2:
                     msg = str("PONG :" + data.split(":")[-1])
                     debug("Registration pong: ", msg)
-                    await s.send_all(msg.encode())
+                    await stream.send_all(msg.encode())
                     return
                 c += 1
 
     async def connect(self):
         remote_ip = socket.gethostbyname(self.host)
         log("ip of irc server is:", remote_ip)
         if self.use_ssl:
             log("Using SSL connection")
             import ssl
-
-            ssl_context = ssl.SSLContext()
-            s = await trio.open_ssl_over_tcp_stream(
-                remote_ip, self.port, https_compatible=True, ssl_context=ssl_context
-            )
+            ssl_context = ssl.create_default_context()
+            ssl_context.check_hostname = False
+            ssl_context.verify_mode = ssl.CERT_NONE
+            reader, writer = await asyncio.open_connection(remote_ip, self.port, ssl=ssl_context)
         else:
-            s = await trio.open_tcp_stream(remote_ip, self.port)
+            reader, writer = await asyncio.open_connection(remote_ip, self.port)
+
         log("connected to: ", self.host, self.port)
+        stream = TCPStream(reader, writer)
 
-        async with s:
-            if self.use_sasl:
-                await s.send_all(("CAP REQ :sasl").encode())
+        if self.use_sasl:
+            # TODO: Implement SASL
+            await stream.send_all(("CAP REQ :sasl").encode())
 
-            if self.server_password:
-                pw_cr = ("PASS " + self.server_password + "\r\n").encode()
-                await s.send_all(pw_cr)
+        if self.server_password:
+            pw_cr = ("PASS " + self.server_password + "\r\n").encode()
+            await stream.send_all(pw_cr)
 
-            nick_cr = ("NICK " + self.nick + "\r\n").encode()
-            await s.send_all(nick_cr)
+        nick_cr = ("NICK " + self.nick + "\r\n").encode()
+        await stream.send_all(nick_cr)
 
-            usernam_cr = ("USER " + " ".join([self.username] * 3) + " :" + self.nick + " \r\n").encode()
-            await s.send_all(usernam_cr)
+        usernam_cr = ("USER " + " ".join([self.username] * 3) + " :" + self.nick + " \r\n").encode()
+        await stream.send_all(usernam_cr)
 
-            ping_confirmed = False
-            try:
-                with trio.fail_after(5):
-                    await self.ping_confirmation(s)
-                    ping_confirmed = True
-                    log("SUBMITTING PING COOKIE CONFIRMATION")
-            except trio.TooSlowError:
-                log("NO PING CONFIRMATION!!!!!")
-
-            if self.password:
-                log("IDENTIFYING")
-                auth_cr = ("PRIVMSG NickServ :IDENTIFY " + self.password + "\r\n").encode()
-                await s.send_all(auth_cr)
-
-            if self.delay:
-                await trio.sleep(self.delay)
-            if self.use_sasl:
-                import base64
-
-                await s.send_all(("AUTHENTICATE PLAIN").encode())
-                sep = "\x00"
-                b = base64.b64encode((self.nick + sep + self.nick + sep + self.password).encode("utf8")).decode("utf8")
-                data = s.recv(4096).decode("utf-8")
-                log("Server SAYS: ", data)
-                await s.send_all(("AUTHENTICATE " + b).encode())
-                log("PERFORMING SASL PLAIN AUTH....")
-                data = s.recv(4096).decode("utf-8")
-                log("Server SAYS: ", data)
-                data = s.recv(4096).decode("utf-8")
-                log("Server SAYS: ", data)
-                await s.send_all(("CAP END").encode())
-
-            self.s = s
-            if type(self.channels) == list:
-                for c in self.channels:
-                    await self.join(c)
-            else:
-                await self.join(self.channels)
-                self.channels = [self.channels]
+        try:
+            async with asyncio.timeout(5):
+                await self.ping_confirmation(stream)
+                log("SUBMITTING PING COOKIE CONFIRMATION")
+        except asyncio.TimeoutError:
+            log("NO PING CONFIRMATION!!!!!")
+
+        if self.password:
+            log("IDENTIFYING")
+            auth_cr = ("PRIVMSG NickServ :IDENTIFY " + self.password + "\r\n").encode()
+            await stream.send_all(auth_cr)
+
+        if self.delay:
+            await asyncio.sleep(self.delay)
+        if self.use_sasl:
+            import base64
+
+            await stream.send_all(("AUTHENTICATE PLAIN").encode())
+            sep = "\x00"
+            b = base64.b64encode((self.nick + sep + self.nick + sep + self.password).encode("utf8")).decode("utf8")
+            data = (await stream.recv(4096)).decode("utf-8")
+            log("Server SAYS: ", data)
+            await stream.send_all(("AUTHENTICATE " + b).encode())
+            log("PERFORMING SASL PLAIN AUTH....")
+            data = (await stream.recv(4096)).decode("utf-8")
+            log("Server SAYS: ", data)
+            data = (await stream.recv(4096)).decode("utf-8")
+            log("Server SAYS: ", data)
+            await stream.send_all(("CAP END").encode())
+
+        self.stream = stream
+        if isinstance(self.channels, list):
+            for c in self.channels:
+                await self.join(c)
+        elif isinstance(self.channels, str):
+            await self.join(self.channels)
+            self.channels = [self.channels]
+        else:
+            raise ValueError("Channels must be a list or a string")
 
-            self.connected = True
-            async with trio.open_nursery() as nursery:
-                log("Listening for messages...")
-                nursery.start_soon(self.run_bot_loop, s)
-                nursery.start_soon(self.message_task_loop)
-                if self.tables:
-                    nursery.start_soon(self.db_operation_loop)
-                nursery.start_soon(self.check_reconnect)
+        self.connected = True
+
+        log("Listening for messages...")
+        tasks = [self.run_bot_loop(stream), self.message_task_loop(), self.check_reconnect()]
+        if self.tables:
+            tasks.append(self.db_operation_loop())
+        await asyncio.gather(*tasks)
 
     async def check_reconnect(self):
         await self.sleep(self.ping_delay)
         while True:
             if not self.connected:
                 break
             self.connected = False
             await self.send_raw(f"PING {self.host}\r\n")
             await self.sleep(self.ping_delay)
         log("Disconnected!! Attempting to reconnect...")
-        await self.s.aclose()
+        await self.stream.aclose()
         raise BotConnectionError("Bot Disconnected: No ping response from server")
-        # self.nursery.cancel()
 
     async def send_raw(self, data: str):
         """send_raw. Sends a string to the irc server.
 
         :param data:
         :type data: str
         """
         if not data.endswith("\r\n"):
             data += "\r\n"
         await self._enqueue_message(data)
 
-    async def join(self, channel):
+    async def join(self, channel: str):
         """joins a channel.
 
         :param channel: str. Channel name. Include the '#', eg. "#lobby"
         """
         log("Joining", channel)
-        await self.s.send_all(("JOIN " + channel + " \r\n").encode())  # chanel
+        await self.stream.send_all(("JOIN " + channel + " \r\n").encode())  # chanel
 
     async def list_channels(self):
         """list_channels of the irc server.
 
         They will be available as a list of strings under:
         bot.server_channels
         """
         await self._send_data("LIST")
         await self.sleep(1)
         return self.server_channels
 
-    async def list_names(self, channel):
+    async def list_names(self, channel: str):
         """Lists users nicks in channel.
 
         Also check bot.channel_names for a non sanitized version(like starting with ~ & % @ + for operators, moderators, etc; if you want to detect them)
 
         :param channel:str channel name
         """
         # await self._send_data(f"NAMES {channel}")
@@ -560,110 +580,116 @@
             "@",
             "+",
         ]
         names = self.channel_names[channel]
         names = [name[1:] if any([name.startswith(s) for s in special_symbols]) else name for name in names]
         return names
 
-    async def send_message(self, message, channel=None):
+    async def send_message(self, message: Sendable, channel: str | list[str] | None = None):
         """Sends a text message. The message will be enqueued and sent whenever
         the messaging loop arrives on it.
 
         :param message: Can be a str, a list of str or a IrcBot.Message object.
         :param channel: Can be a str or a list of str. By default it is all channels the bot constructor receives. Instead of the channel name you can pass in a user nickname to send a private message.
         """
         if channel is None:
             channel = self.channels
 
-        if type(channel) == list and type(message) != Message:
+        if isinstance(channel, list):
             for chan in channel:
                 await self._send_message(message, chan)
         else:
             await self._send_message(message, channel)
 
-    async def _send_message(self, message, channel):
-        if type(message) == str:
+    async def _send_message(self, message: Sendable, channel: str):
+        if isinstance(message, str):
             message = message.replace("\n", "    ")
             message = message.replace("\r", "")
             await self._enqueue_message((str("PRIVMSG " + channel) + " :" + message + " \r\n"))
-        elif type(message) == Color:
+        elif isinstance(message, Color):
             await self._send_message(message.str, channel)
-        elif type(message) == list:
+        elif isinstance(message, list):
             for msg in message:
                 await self._send_message(msg, channel)
-        elif type(message) == Message:
+        elif isinstance(message, Message):
             await self._send_message(message.message, message.channel)
+        else:
+            raise ValueError("Message must be a str, a list of str, a Message object or a Color object")
 
     async def message_task_loop(self):
-        async with self.receive_message_channel:
-            async for msg in self.receive_message_channel:
+        while True:
+            try:
+                msg = await self.message_queue.get()
                 await self._send_data(msg)
+                self.message_queue.task_done()
+            except asyncio.QueueEmpty:
+                break
 
     async def _enqueue_message(self, message):
-        await self.send_message_channel.send(message)
+        await self.message_queue.put(message)
 
     async def _send_data(self, data):
-        s = self.s
         debug("Sending: ", f"{data=}")
-        await trio.sleep(0)
-        await s.send_all(data.encode())
+        await self.stream.send_all(data.encode())
 
     async def check_tables(self):
         debug("Checking tables")
         for table in self.tables:
             if table._queue:
-                table_copy = persistentData(table.filename, table.name, table.keys)
+                table_copy = PersistentData(table.filename, table.name, table.keys)
                 table_copy._queue = table._queue
                 await self._enqueue_db_tsk(table_copy)
             debug("qeue", table._queue)
             table.clear()
 
     def fetch_tables(self):
         debug("Fetching tables")
         for table in self.tables:
             table.fetch()
 
-    async def _enqueue_db_tsk(self, table):
+    async def _enqueue_db_tsk(self, table: PersistentData):
         debug("db task", str(table._queue))
-        await self.send_db_operation_channel.send(table)
+        await self.db_operation_queue.put(table)
 
     async def db_operation_loop(self):
-        async with self.receive_db_operation_channel:
-            async for table in self.receive_db_operation_channel:
+        while True:
+            try:
+                table = await self.db_operation_queue.get()
                 for op in table._queue:
-                    if op.op == dbOperation.ADD:
-                        table.db.newData(op.data)
-                    if op.op == dbOperation.REMOVE:
-                        table.db.deleteData(op.id)
-                    if op.op == dbOperation.UPDATE:
+                    if op.op == DBOperation.ADD:
+                        table.db.new_data(op.data)
+                    if op.op == DBOperation.REMOVE:
+                        table.db.delete_data(op.id)
+                    if op.op == DBOperation.UPDATE:
                         table.db.update(op.id, op.data)
+                self.db_operation_queue.task_done()
+            except asyncio.QueueEmpty:
+                break
 
-    async def run_bot_loop(self, s):
+    async def run_bot_loop(self, stream: TCPStream):
         """Starts main bot loop waiting for messages."""
-        async with trio.open_nursery() as nursery:
-            async with self.send_message_channel, self.send_db_operation_channel:
-                async for data in s:
-                    try:
-                        data = data.decode("utf-8")
-                    except UnicodeDecodeError:
-                        pass
-                    debug(
-                        "\n>>>> DECODED DATA FROM SERVER: \n",
-                        60 * "-",
-                        "\n",
-                        f"{data=}\n",
-                        60 * "-",
-                        "\n",
-                    )
-                    self.fetch_tables()
-                    for msg in data.split("\r\n"):
-                        nursery.start_soon(self.data_handler, s, msg)
+        while True:
+            data = await stream.recv()
+            try:
+                data = data.decode("utf-8")
+            except UnicodeDecodeError:
+                continue
+            debug(
+                "\n>>>> DECODED DATA FROM SERVER: \n",
+                60 * "-",
+                "\n",
+                f"{data=}\n",
+                60 * "-",
+                "\n",
+            )
+            self.fetch_tables()
+            await asyncio.gather(*[self.data_handler(data) for data in data.split("\r\n")])
 
     async def process_result(self, result, channel, sender_nick, is_private):
-        if type(result) == ReplyIntent:
+        if isinstance(result, ReplyIntent):
             if result.message:
                 await self.send_message(result.message, sender_nick if is_private else channel)
                 if type(result.message) == Message:
                     if result.message.channel not in self.replyIntents:
                         self.replyIntents[result.message.channel] = {}
                     debug("Saving message intent")
                     self.replyIntents[result.message.channel][result.message.sender_nick] = result
@@ -909,15 +935,15 @@
 
     def jls_extract_def(self, wait_for):
         return wait_for
 
     async def wait_for(
         self,
         type: str,
-        from_nick: str = None,
+        from_nick: str | None = None,
         timeout: int = 0,
         cache_ttl: int = 0,
         filter_func=None,
     ) -> dict:
         """Will wait for a response of type check custom handler types from
         nick. Will return the message dict.
 
@@ -957,43 +983,42 @@
         self._awaiting_messages[key][idx]["message"] = {}
         self._awaiting_messages[key][idx]["filter_func"] = filter_func
         self._awaiting_messages[key][idx]["type"] = type
         self._awaiting_messages[key][idx]["timeout"] = timeout
         self._awaiting_messages[key][idx]["nick"] = from_nick
         self._awaiting_messages[key][idx]["cache_ttl"] = cache_ttl
         self._awaiting_messages[key][idx]["use_cache"] = use_cache
-        send_stream, receive_stream = trio.open_memory_channel(0)
-        self._awaiting_messages[key][idx]["send_stream"] = send_stream
+        wait_for_queue = asyncio.Queue()
+        self._awaiting_messages[key][idx]["send_stream"] = wait_for_queue
 
         async def await_message():
-            async for msg in receive_stream:
-                break
-            await send_stream.aclose()
-            await receive_stream.aclose()
+            msg = await wait_for_queue.get()
             self._awaiting_messages[key][idx]["message"] = msg
             if use_cache and "cache" not in self._awaiting_messages[key]:
                 self._awaiting_messages[key]["cache"] = msg
+            wait_for_queue.task_done()
+            self._awaiting_messages[key][idx]["send_stream"] = None
 
         if timeout and timeout > 0:
-            with trio.move_on_after(timeout):
+            async with asyncio.timeout(timeout):
                 await await_message()
         else:
             await await_message()
 
         msg = self._awaiting_messages.get(key)
         if msg:
             msg = msg.get(idx)
         else:
             return {}
         if not use_cache:
             self._awaiting_messages[key].pop(idx)
         return msg["message"] if msg else {}
 
     # MAIN DATA RECEIVING HANDLER
-    async def data_handler(self, s, data):
+    async def data_handler(self, data: str):
         nick = self.nick
         host = self.host
         self.connected = True
 
         try:
             if utils._hot_reload_if_changed():
                 await self.hot_reload()
@@ -1058,15 +1083,15 @@
             r"^:(.*)!.*NOTICE (\S+) :(\S+) (.*)$": lambda g: {
                 "type": "notice",
                 "nick": g.group(1),
                 "channel": g.group(2),
                 "notice": g.group(3),
                 "text": g.group(4),
             },
-            r"^\s*PING \s*" + self.nick + r"\s*$": lambda g: {"type": "ping", "ping": self.nick},
+            r"^\s*PING \s*" + self.nick + r"\s*$": lambda _: {"type": "ping", "ping": self.nick},
             r"^:\S+\s+PONG\s+\S+\s+:(\S+).*$": lambda g: {"type": "pong", "nick": g[1]},
             r"^:\S* 353 "
             + self.nick
             + r" = (\S+) :(.*)\s*$": lambda g: {
                 "type": "names",
                 "channel": g.group(1),
                 "names": g.group(2).split(),
@@ -1151,17 +1176,19 @@
                         if callable(filter_func) and not filter_func(message):
                             continue
                     except Exception as e:
                         log(f"ATTENTION! Error in wait_for -> your {filter_func=} failed with {str(e)}")
                         continue
                     debug(f"Found match for awaiting message {idx=} {self._awaiting_messages[akey][idx]=}")
                     debug(f"{message=}")
-                    try:
-                        await self._awaiting_messages[akey][idx]["send_stream"].send(message)
-                    except trio.ClosedResourceError:
+
+                    queue = self._awaiting_messages[akey][idx]["send_stream"]
+                    if queue is not None:
+                        await queue.put(message)
+                    else:
                         continue
                     if not use_cache:
                         return
 
             if message["type"] == "dccreject":
                 items = self._dcc_busy_ports.items()
                 free_ports = []
@@ -1297,15 +1324,14 @@
                         break
                     for reg in cmd:
                         m = re.match(reg, msg)
                         if m:
                             if cmd in utils.regex_commands:
                                 if is_private and not utils.regex_commands_accept_pm[i]:
                                     continue
-                                await trio.sleep(0)
                                 _message = Message(channel, sender_nick, msg, is_private)
                                 result = await self._call_cb(cmd[reg], _message, m)
                             if result:
                                 await self.process_result(result, channel, sender_nick, is_private)
                                 matched = True
                             if utils.single_match:
                                 matched = True
@@ -1326,30 +1352,28 @@
                         m = re.match(reg, msg)  # , flags=re.IGNORECASE)
                         if m:
                             if cmd in utils.regex_commands_with_message:
                                 if is_private and not utils.regex_commands_with_message_accept_pm[i]:
                                     continue
                                 debug("sending to", sender_nick)
                                 if utils.regex_commands_with_message_pass_data[i]:
-                                    await trio.sleep(0)
                                     _message = Message(
                                         channel,
                                         sender_nick,
                                         msg,
                                         is_private,
                                         strip=self.strip_messages,
                                     )
                                     result = await self._call_cb(
                                         cmd[reg],
                                         _message,
                                         m,
                                         _message,
                                     )
                                 else:
-                                    await trio.sleep(0)
                                     _message = Message(
                                         channel,
                                         sender_nick,
                                         msg,
                                         is_private,
                                         strip=self.strip_messages,
                                     )
@@ -1371,16 +1395,15 @@
                     for word in msg.split(" "):
                         if len(word) < 6:
                             continue
                         result = None
                         word = word.strip()
                         if word[-1] in [" ", "?", ",", ";", ":", "\\"]:
                             word = word[:-1]
-                        if utils.validateUrl(word):
-                            await trio.sleep(0)
+                        if utils.validate_url(word):
                             debug("Checking url: " + str(word))
                             _message = Message(channel, sender_nick, msg, is_private)
                             result = await self._call_cb(utils.url_commands[-1], _message, word)
                         if result:
                             await self.send_message(result, channel)
 
             await self.check_tables()
@@ -1397,14 +1420,14 @@
                     return
         if inspect.iscoroutinefunction(cb):
             return await cb(self, *args, **kwargs)
         return cb(*args, **kwargs)
 
     def __del__(self):
         try:
-            self.s.close()
+            self.stream.close()
         except:
             pass
 
     def close(self):
         """Stops the bot and loop if running."""
         self.__del__()
```

### Comparing `re-ircbot-1.7.0/IrcBot/dcc.py` & `re_ircbot-2.0.0.dev0/ircbot/dcc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Simple dcc related functions
 import socket
 import struct
 from enum import Enum
 
-from IrcBot.utils import debug, log
+from ircbot.utils import debug, log
 
 BUFFSIZE = 2048
 
 
 class DccServer(Enum):
     SEND = 0
     GET = 1
@@ -79,17 +79,15 @@
         """
         self.nick = nick
         self.filename = filename
         self.ip = ip
         self.port = port
         self.size = size
         self.token = token
-        self.is_passive = (
-            self.token is not None
-        )  # and self.port == 0 or self.ip == "1.1.1.1" ?
+        self.is_passive = self.token is not None  # and self.port == 0 or self.ip == "1.1.1.1" ?
         self.download_progress = 0
 
     def to_message(self):
         return {
             "nick": self.nick,
             "filename": self.filename,
             "ip": self.ip,
```

### Comparing `re-ircbot-1.7.0/IrcBot/message.py` & `re_ircbot-2.0.0.dev0/ircbot/message.py`

 * *Files identical despite different names*

### Comparing `re-ircbot-1.7.0/IrcBot/shortestPrefix.py` & `re_ircbot-2.0.0.dev0/ircbot/shortest_prefix.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import itertools
 
+
 # A class to store a Trie node
 class TrieNode:
     def __init__(self):
         # each node stores a dictionary to its child nodes
         self.child = {}
 
         # keep track of the total number of times the current node is visited
@@ -24,48 +25,53 @@
         curr.child[c].freq += 1
 
         # go to the next node
         curr = curr.child[c]
 
 
 # Function to recursively traverse the Trie in a preorder fashion and
-def shortestPrefix(root, word_so_far):
+def shortest_prefix(root, word_so_far):
     if root is None:
         return ""
 
     # print `word_so_far` if the current Trie node is visited only once
     if root.freq == 1:
         return word_so_far
 
     # recur for all child nodes
     r = []
     for k, v in root.child.items():
-        r.append(shortestPrefix(v, word_so_far + k))
+        r.append(shortest_prefix(v, word_so_far + k))
     return r
 
 
 # Find the shortest unique prefix for every word in a given array
-def findShortestPrefix(words):
+def find_shortest_prefix(words):
 
     # construct a Trie from the given items
     root = TrieNode()
     for s in words:
         insert(root, s)
 
     # Recursively traverse the Trie in a preorder fashion to list all prefixes
-    r = shortestPrefix(root, "")
+    r = shortest_prefix(root, "")
     R = list(itertools.chain(*r))
     while any([isinstance(elm, list) for elm in R]):
         R = list(itertools.chain(*R))
 
     # DIRT FIX HERE
     reordered = {}
     for r in R:
+        w = None
         for w in words:
             if w.startswith(r):
                 reordered[w] = r
                 break
-        words.remove(w)
+        if w is not None:
+            words.remove(w)
     return reordered
 
+
 if __name__ == "__main__":
-    print(findShortestPrefix(['board', 'move', 'colors', 'undo', 'hint', 'score', 'label', 'start', 'accept', 'help']))
+    print(
+        find_shortest_prefix(["board", "move", "colors", "undo", "hint", "score", "label", "start", "accept", "help"])
+    )
```

### Comparing `re-ircbot-1.7.0/IrcBot/sqlitedb.py` & `re_ircbot-2.0.0.dev0/ircbot/sqlitedb.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,317 +10,295 @@
 #  Depends on: sqlite module, basically all python std.                 #
 #                                                                       #
 #########################################################################
 
 import sqlite3
 from copy import copy
 from pathlib import Path
+from typing import Any
 
 
 class DB:
-    def __init__(self, dbFilePath, tableName, rowLabels, keepOpen=False):
-        """dbFilePath: str. Path for the file to save the sqtile db on.
-        tableName: str. Name of the table to use.
-        rowLabels: list. Strings with the data keys to store, columns of the table.
-        keepOpen: bool. If set to True you will have to manually call connect and close.
+    def __init__(self, db_file_path: str, table_name: str, row_labels: list[str], keep_open: bool) -> None:
+        """Initialize the DB object.
+
+        :param db_file_path: str. Path for the file to save the SQLite DB.
+        :param table_name: str. Name of the table to use.
+        :param row_labels: list[str]. Strings with the data keys to store, columns of the table.
+        :param keep_open: bool. If set to True, manually call connect and close.
         """
-        self.filepath = dbFilePath
-        self.tableName = tableName
-        self.rowLabels = rowLabels
-        self.keepOpen = keepOpen
-        self.checkIfExistsIfNotCreate()
+        self.filepath = db_file_path
+        self.table_name = table_name
+        self.row_labels = row_labels
+        self.keep_open = keep_open
+        self._check_if_exists_if_not_create()
 
-    def toDict(self, data):
-        """toDict. Returns a dict.
+    def to_dict(self, data):
+        """Convert a row to a dictionary.
 
-        :param data: list which represents a full row to convert to a dict with the respective kes defined in rowLabels
+        :param data: list representing a full row to convert to a dict with the respective keys defined in row_labels.
         """
-        return {n: data[i] for i, n in enumerate(self.rowLabels)}
+        return {n: data[i] for i, n in enumerate(self.row_labels)}
 
-    def toDictWithId(self, data):
-        """toDictWithId. Returns a dict with the "id" field.
+    def to_dict_with_id(self, data: list[Any]) -> dict[str, Any]:
+        """Convert a row to a dictionary with the "id" field.
 
-        :param data: list which represents a full row to convert to a dict with the respective kes defined in rowLabels
+        :param data: list representing a full row to convert to a dict with the respective keys defined in row_labels.
         """
-        return {n: data[i] for i, n in enumerate(["id"] + self.rowLabels)}
+        return {n: data[i] for i, n in enumerate(["id"] + self.row_labels)}
 
-    def toList(self, data):
-        """toList. Converts a dict to a row list in the other defined by
-        rowLabels.
+    def to_list(self, data: dict[str, Any]) -> list[Any]:
+        """Convert a dictionary to a row list as defined by row_labels.
 
         :param data: dict.
         """
-        return [data[n] if n in data.keys() else "" for n in self.rowLabels]
+        return [data[n] if n in data.keys() else "" for n in self.row_labels]
 
-    def checkIfExistsIfNotCreate(self):
-        self.connect()
+    def _check_if_exists_if_not_create(self):
+        self._connect()
         try:
-            self.cursor.execute("SELECT * FROM " + self.tableName)
+            self.cursor.execute("SELECT * FROM " + self.table_name)
             col_name_list = [tuple[0] for tuple in self.cursor.description]
             col_name_list.remove("id")
         except:
             col_name_list = []
-        self.close()
-        if not sorted(col_name_list) == sorted(self.rowLabels):
-            self.deleteTable()
+        self._close()
+        if not sorted(col_name_list) == sorted(self.row_labels):
+            self.delete_table()
             self._connect()
             self.cursor.execute(
                 "CREATE TABLE IF NOT EXISTS "
-                + self.tableName
+                + self.table_name
                 + " (id INTEGER primary key AUTOINCREMENT,"
-                + str(self.rowLabels)[1:-1]
+                + str(self.row_labels)[1:-1]
                 + ")"
             )
-            self.close()
+            self._close()
 
     def connect(self):
         self.connection = sqlite3.connect(self.filepath)
         self.cursor = self.connection.cursor()
         self.connected = True
 
     def _connect(self):
-        if self.keepOpen:
+        if self.keep_open:
             return
         self.connect()
 
     def close(self):
         self.connection.commit()
         self.connection.close()
         self.connected = False
 
     def _close(self):
-        if self.keepOpen:
+        if self.keep_open:
             return
         self.close()
 
-    def _saveData(self, data_):
-        data_ = self.toList(data_)
+    def _save_data(self, data_: dict[str, Any]):
+        rows = self.to_list(data_)
         self.cursor.execute(
             "INSERT INTO "
-            + self.tableName
+            + self.table_name
             + " ("
-            + str(self.rowLabels)[1:-1]
+            + str(self.row_labels)[1:-1]
             + ")VALUES ("
-            + (len(self.rowLabels) * "?,")[:-1]
+            + (len(self.row_labels) * "?,")[:-1]
             + ")",
-            data_,
+            rows,
         )
 
-    def newData(self, data_):
-        # assert len(data_)==len(self.rowLabels), "ERRO: O data_ deve ter o tamanho " + str(len(self.rowLabels))
+    def new_data(self, data_: dict[str, Any]) -> int:
         self._connect()
-        self._saveData(data_)
+        self._save_data(data_)
         id = copy(self.cursor.lastrowid)
         self._close()
+        if id is None:
+            raise BaseException("Error saving data!")
         return id
 
-    def saveDataList(self, lista):
+    def save_data_list(self, lista: list[dict[str, Any]]):
         self._connect()
-        [self._saveData(data_) for data_ in lista]
+        [self._save_data(data_) for data_ in lista]
         self._close()
 
-    def _getData(self, id):
-        return self.toDict(
-            list(
-                list(
-                    self.cursor.execute(
-                        "SELECT * FROM " + self.tableName + " WHERE id = ?", (id,)
-                    )
-                )[0]
-            )[1:]
+    def _get_data(self, id: int) -> dict[str, Any]:
+        return self.to_dict(
+            list(list(self.cursor.execute("SELECT * FROM " +
+                 self.table_name + " WHERE id = ?", (id,)))[0])[1:]
         )
 
-    def getData(self, id):
+    def get_data(self, id: int) -> dict[str, Any]:
         self._connect()
-        data_ = self._getData(id)
+        data_ = self._get_data(id)
         self._close()
         return data_
 
-    def getDataWithId(self, id):
+    def get_data_with_id(self, id: int) -> dict[str, Any]:
         self._connect()
-        data_ = self._getData(id)
+        data_ = self._get_data(id)
         self._close()
         data_.update({"id": id})
         return data_
 
-    def getAll(self):
+    def get_all(self):
         self._connect()
-        data_s = [
-            self.toDict(row[1:])
-            for row in self.cursor.execute("SELECT * FROM " + self.tableName)
-        ]
+        data_s = [self.to_dict(row[1:]) for row in self.cursor.execute(
+            "SELECT * FROM " + self.table_name)]
         self._close()
         return data_s
 
-    def getAllWithId(self):
+    def get_all_with_id(self):
         self._connect()
-        data_s = [
-            self.toDictWithId(row)
-            for row in self.cursor.execute("SELECT * FROM " + self.tableName)
-        ]
+        data_s = [self.to_dict_with_id(row) for row in self.cursor.execute(
+            "SELECT * FROM " + self.table_name)]
         self._close()
         return data_s
 
-    def _getByKey(self, key: str, value: any):
-        if key not in self.rowLabels:
+    def _get_by_key(self, key: str, value: Any):
+        if key not in self.row_labels:
             raise BaseException("Invalid Key!")
         self._connect()
-        # self.connection.set_trace_callback(print)
         cursor = self.cursor.execute(
-            "SELECT * FROM " + self.tableName + " WHERE " + key + " = ?",
-            (value,),
-        )
-        # self.connection.set_trace_callback(None)
+            "SELECT * FROM " + self.table_name + " WHERE " + key + " = ?", (value,))
         data = cursor.fetchone()
         self._close()
         return data
 
-    def getByKey(self, key: str, value: any):
-        data = self._getByKey(key, value)
-        return self.toDict(list(data)[1:]) if data else None
-
-    def getByKeyWithId(self, key: str, value: any):
-        data = self._getByKey(key, value)
-        return self.toDictWithId(data) if data else None
+    def get_by_key(self, key: str, value: Any):
+        data = self._get_by_key(key, value)
+        return self.to_dict(list(data)[1:]) if data else None
+
+    def get_by_key_with_id(self, key: str, value: Any):
+        data = self._get_by_key(key, value)
+        return self.to_dict_with_id(data) if data else None
 
-    def findData(self, key, nome):
+    def find_data(self, key: str, name: Any):
         func = str
         try:
-            float(nome)
+            float(name)
             func = float
         except:
             pass
         self._connect()
-        if type(nome) == str:
-            key = key
-            idList = [
-                [list(data_)[0], self.toDict(list(data_)[1:])[key]]
-                for data_ in list(
-                    self.cursor.execute("SELECT * FROM " + self.tableName)
-                )
-                if nome.lower() in str(self.toDict(list(data_)[1:])[key]).lower()
+        if isinstance(name, str):
+            id_list = [
+                [list(data_)[0], self.to_dict(list(data_)[1:])[key]]
+                for data_ in list(self.cursor.execute("SELECT * FROM " + self.table_name))
+                if name.lower() in str(self.to_dict(list(data_)[1:])[key]).lower()
             ]
         else:
-            idList = [
-                [list(data_)[0], self.toDict(list(data_)[1:])[key]]
-                for data_ in list(
-                    self.cursor.execute("SELECT * FROM " + self.tableName)
-                )
-                if str(nome) == str(self.toDict(list(data_)[1:])[key])
+            id_list = [
+                [list(data_)[0], self.to_dict(list(data_)[1:])[key]]
+                for data_ in list(self.cursor.execute("SELECT * FROM " + self.table_name))
+                if str(name) == str(self.to_dict(list(data_)[1:])[key])
             ]
         self._close()
         try:
-            return [x[0] for x in sorted(idList, key=lambda x: func(x[1]))]
-        except ValueError as e:
-            return [x[0] for x in sorted(idList, key=lambda x: str(x[1]))]
+            return [x[0] for x in sorted(id_list, key=lambda x: func(x[1]))]
+        except ValueError:
+            return [x[0] for x in sorted(id_list, key=lambda x: str(x[1]))]
 
-    def findExactMatchFromKey(self, key, nome):
+    def find_exact_match_from_key(self, key, nome):
         func = str
         try:
             float(nome)
             func = float
         except:
             pass
         self._connect()
-        if type(nome) == str:
-            key = key
-            idList = [
-                [list(data_)[0], self.toDict(list(data_)[1:])[key]]
-                for data_ in list(
-                    self.cursor.execute("SELECT * FROM " + self.tableName)
-                )
-                if nome.lower() == str(self.toDict(list(data_)[1:])[key]).lower()
+        if isinstance(nome, str):
+            id_list = [
+                [list(data_)[0], self.to_dict(list(data_)[1:])[key]]
+                for data_ in list(self.cursor.execute("SELECT * FROM " + self.table_name))
+                if nome.lower() == str(self.to_dict(list(data_)[1:])[key]).lower()
             ]
         else:
-            idList = [
-                [list(data_)[0], self.toDict(list(data_)[1:])[key]]
-                for data_ in list(
-                    self.cursor.execute("SELECT * FROM " + self.tableName)
-                )
-                if str(nome) == str(self.toDict(list(data_)[1:])[key])
+            id_list = [
+                [list(data_)[0], self.to_dict(list(data_)[1:])[key]]
+                for data_ in list(self.cursor.execute("SELECT * FROM " + self.table_name))
+                if str(nome) == str(self.to_dict(list(data_)[1:])[key])
             ]
         self._close()
         try:
-            return [x[0] for x in sorted(idList, key=lambda x: func(x[1]))]
-        except ValueError as e:
-            return [x[0] for x in sorted(idList, key=lambda x: str(x[1]))]
-
-    def getDataListByIdList(self, listaDeIds):
-        return [self.getData(id) for id in listaDeIds]
-
-    def getDataListByIdListWithId(self, listaDeIds):
-        return [self.getDataWithId(id) for id in listaDeIds]
-
-    def findDataByKey(self, key, nome):
-        return sorted(
-            self.getDataListByIdList(self.findData(key, nome)), key=lambda x: x[key]
-        )
-
-    def findGreaterThan(self, key, valor):
-        assert type(valor) == int or type(valor) == float, "Entre com valores numéricos"
-        self._connect()
-        idList = [
-            [list(data_)[0], self.toDict(list(data_)[1:])[key]]
-            for data_ in list(self.cursor.execute("SELECT * FROM " + self.tableName))
-            if float(valor) <= float(self.toDict(list(data_)[1:])[key])
+            return [x[0] for x in sorted(id_list, key=lambda x: func(x[1]))]
+        except ValueError:
+            return [x[0] for x in sorted(id_list, key=lambda x: str(x[1]))]
+
+    def get_data_list_by_id_list(self, id_list: list[int]) -> list[dict[str, Any]]:
+        return [self.get_data(id) for id in id_list]
+
+    def get_data_list_by_id_list_with_id(self, id_list: list[int]) -> list[dict[str, Any]]:
+        return [self.get_data_with_id(id) for id in id_list]
+
+    def find_data_by_key(self, key: str, name: Any):
+        return sorted(self.get_data_list_by_id_list(self.find_data(key, name)), key=lambda x: x[key])
+
+    def find_greater_than(self, key: str, value: Any):
+        assert isinstance(value, int) or isinstance(
+            value, float), "Enter numeric values"
+        self._connect()
+        id_list = [
+            [list(data_)[0], self.to_dict(list(data_)[1:])[key]]
+            for data_ in list(self.cursor.execute("SELECT * FROM " + self.table_name))
+            if float(value) <= float(self.to_dict(list(data_)[1:])[key])
         ]
         self._close()
-        return [x[0] for x in sorted(idList, key=lambda x: x[1])]
+        return [x[0] for x in sorted(id_list, key=lambda x: x[1])]
 
-    def findLessThan(self, key, valor):
-        assert type(valor) == int or type(valor) == float, "Entre com valores numéricos"
-        self._connect()
-        idList = [
-            [list(data_)[0], self.toDict(list(data_)[1:])[key]]
-            for data_ in list(self.cursor.execute("SELECT * FROM " + self.tableName))
-            if float(valor) >= float(self.toDict(list(data_)[1:])[key])
+    def find_less_than(self, key, value):
+        assert isinstance(value, int) or isinstance(
+            value, float), "Enter numeric values"
+        self._connect()
+        id_list = [
+            [list(data_)[0], self.to_dict(list(data_)[1:])[key]]
+            for data_ in list(self.cursor.execute("SELECT * FROM " + self.table_name))
+            if float(value) >= float(self.to_dict(list(data_)[1:])[key])
         ]
         self._close()
-        return [x[0] for x in sorted(idList, key=lambda x: x[1])]
+        return [x[0] for x in sorted(id_list, key=lambda x: x[1])]
 
-    def findDataBiggerThan(self, key, valor):
+    def find_data_bigger_than(self, key: str, value: Any):
         return sorted(
-            self.getDataListByIdList(self.findGreaterThan(key, valor)),
+            self.get_data_list_by_id_list(self.find_greater_than(key, value)),
             key=lambda x: x[key],
         )
 
-    def findDataLessThan(self, key, valor):
+    def find_data_less_than(self, key: str, value: Any):
         return sorted(
-            self.getDataListByIdList(self.findLessThan(key, valor)),
+            self.get_data_list_by_id_list(self.find_less_than(key, value)),
             key=lambda x: x[key],
         )
 
-    def deleteData(self, id):
+    def delete_data(self, id: int):
         self._connect()
-        id = str(id)
-        self.cursor.execute("DELETE FROM " + self.tableName + " WHERE ID = ?", (id,))
+        id_str = str(id)
+        self.cursor.execute(
+            "DELETE FROM " + self.table_name + " WHERE ID = ?", (id_str,))
         self._close()
 
-    def update(self, id, data_):
-        """updates given id to new dict.
+    def update(self, id: int, data_: dict[str, Any]):
+        """Update given id with new dict.
 
-        :param id: id to modify
-        :param data_: data dict that can only contain fields to update
+        :param id: id to modify.
+        :param data_: data dict that can only contain fields to update.
         """
-        d = self.getData(id)
+        d = self.get_data(id)
         d.update(data_)
-        d = self.toList(d)
+        d = self.to_list(d)
         self._connect()
         self.cursor.execute(
-            "UPDATE "
-            + self.tableName
-            + " SET "
-            + " = ?,".join(self.rowLabels)
-            + "= ? WHERE id= ?",
+            "UPDATE " + self.table_name + " SET " +
+            " = ?,".join(self.row_labels) + "= ? WHERE id= ?",
             (d + [id]),
         )
         self._close()
 
-    def deleteTable(self):
-        """Deletes the table."""
+    def delete_table(self):
+        """Delete the table."""
         self._connect()
-        self.cursor.execute("DROP TABLE IF EXISTS " + self.tableName)
+        self.cursor.execute("DROP TABLE IF EXISTS " + self.table_name)
         self._close()
 
-    def deleteAll(self):
-        """Deletes the db file."""
+    def delete_all(self):
+        """Delete the DB file."""
         Path(self.filepath).unlink()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `re-ircbot-1.7.0/IrcBot/utils.py` & `re_ircbot-2.0.0.dev0/ircbot/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 import importlib.util
 import inspect
 import logging
 import os
 import re
 import sys
 from functools import wraps
-from typing import Callable, TypeVar
 
 has_validators = False
 try:
     import validators
 
     has_validators = True
 except:
     pass
 
-from .message import Message
-from .shortestPrefix import findShortestPrefix
+from ircbot.message import Message
+from ircbot.shortest_prefix import find_shortest_prefix
 
 logger = None
 
 parse_order = False
 
 # COMMAND DECORATORS
 regex_commands = []
@@ -187,15 +186,15 @@
 )
 
 arg_commands_with_message = {}
 
 simplify_arg_commands = True
 
 
-def setSimplifyCommands(simplify):
+def set_simplify_commands(simplify):
     global simplify_arg_commands
     simplify_arg_commands = simplify
 
 
 def arg_command(
     command,
     help="",
@@ -241,51 +240,51 @@
 help_msg = {}
 help_msg_bottom = []
 commands_help = {}
 help_menu_separator = "\n"
 help_on_private = False
 
 
-def setHelpMenuSeparator(sep: str):
+def set_help_menu_separator(sep: str):
     """Sets the separator string between the help commands. If can contain a
     '\n'.
 
     :param sep: separator
     :type sep: str
     """
     global help_menu_separator
     help_menu_separator = sep
 
 
-def setHelpOnPrivate(is_private):
+def set_help_on_private(is_private):
     """Defines if the help messages should be sent as private messages. This is
     useful to avoide flooding if the bots has many commands.
 
     :param is_private: if true they will be private (default False: display on the current channel)
     """
     global help_on_private
     help_on_private = is_private
 
 
-def setHelpHeader(txt: str):
+def set_help_header(txt: str):
     """Adds some text to the help message before the command descriptions.
 
     :param txt: Text to display before command descriptions
     :type txt: str
     """
     global help_msg_header
     if isinstance(txt, str):
         help_msg_header = [txt]
     elif isinstance(txt, list):
         help_msg_header = txt
     else:
         raise BaseException("You must pass wither a list of strings or a string")
 
 
-def setHelpBottom(txt: str):
+def set_help_bottom(txt: str):
     """Adds some text to the help message after the command descriptions.
 
     :param txt: Text to display after command descriptions
     :type txt: str
     """
     global help_msg_bottom
     if isinstance(txt, str):
@@ -306,15 +305,15 @@
         + opt_close * len(org[len(pref) :])
     )
 
 
 _defined_command_dict = {}
 
 
-def setCommands(command_dict: dict, simplify=None, prefix="!"):
+def set_commands(command_dict: dict, simplify=None, prefix="!"):
     """Defines commands for the bot from existing functions
     param: command_dict: Takes a dictionary of "command names": function's to call creating the commands for each of them.
     param: simplify: Uses shortest prefixes for each command. If True the shortest differentiatable prefixes for the commands will work. Like if there is start and stop, !sta will call start and !sto will call stop. Instead of passing a function  directly you can pass in a dict like:
     {"function": cb, "acccept_pms": True, "pass_data": True, "help": "This command starts the bot", "command_help": "Detailed help for this command in particular"}
     if needed. The help parameter if passed will define the 'help' command.
     """
     global command_prefix, help_msg, commands_help
@@ -331,15 +330,15 @@
             return True
         if isinstance(command_dict[c], dict) and "simplify" not in command_dict[c]:
             return not simplify
         if isinstance(command_dict[c], dict) and "simplify" in command_dict[c]:
             return not command_dict[c]["simplify"]
         return False
 
-    _commands = findShortestPrefix([c for c in command_dict.keys() if not not_regex(c)])
+    _commands = find_shortest_prefix([c for c in command_dict.keys() if not not_regex(c)])
     min_commands = []
     exclude_list = [c for c in command_dict.keys() if not_regex(c)]
     for cmd in command_dict:
         if cmd in exclude_list:
             min_commands.append(cmd)
         else:
             min_commands.append(_commands[cmd])
@@ -375,15 +374,15 @@
             re_command(expression)(cb)
         else:
             logging.error("You passed a wrong data type on setCommands for command: %s", cmd)
             sys.exit(1)
 
     _defined_command_dict = command_dict
     if help_msg or commands_help:
-        _commands = findShortestPrefix([c for c in command_dict.keys() if not not_regex(c)] + ["help"])
+        _commands = find_shortest_prefix([c for c in command_dict.keys() if not not_regex(c)] + ["help"])
 
         def help_menu(args, message):
             channel = message.channel
             if help_on_private:
                 channel = message.sender_nick
 
             if args[1] in commands_help:
@@ -404,54 +403,51 @@
                         + help_menu_separator.join(help_msg.values())
                         + help_menu_separator.join(help_msg_bottom)
                     )
 
         re_command(_reg_word("help", _commands["help"]))(help_menu)
 
 
-def setPrefix(prefix):
+def set_prefix(prefix):
     """setPrefix. Sets the prefix for arg commands.
 
     :param prefix: str prefix for commands
     """
     global command_prefix
     command_prefix = prefix
 
 
-def setSingleMatch(singleMatch: bool):
+def set_single_match(singleMatch: bool):
     """Defines if there will be only one command handler called. If false all regex and arg_commands will be matched against the user input.
     :param singleMatch: If true there will be only one match per command. Defaults to False (all matches will be called)
     :type singleMatch: bool
     """
     global single_match
     single_match = singleMatch
 
 
-def setParseOrderTopBottom(top_bottom: bool = True):
+def set_parser_order(top_bottom: bool = True):
     """setParseOrder.
 
     :param top_bottom: bool -> if True then first defined regex expressions will overwrite last ones. Default is False
     """
     global parse_order
     parse_order = top_bottom
 
 
-def setMaxArguments(n):
+def set_max_arguments(n):
     """setMaxArguments.
 
     :param n: number of arguments for callbacks in arg_command decorator
     """
     global _command_max_arguments
     _command_max_arguments = n
 
 
-# LOGGING SETUP
-
-
-def setLogging(level, logfile=None):
+def set_loglevel(level, logfile=None):
     """Sets the loggins level of the logging module.
 
     :param level: int. level, (logging.DEBUG, logging.INFO, etc...)
     :param logfile: str. Path for file or empty for none.
     """
     global logger
     logging.basicConfig(
@@ -460,15 +456,15 @@
         format="%(asctime)s::%(levelname)s -> %(message)s",
         datefmt="%I:%M:%S %p",
     )
     logger = logging.getLogger()
     logger.setLevel(level)
 
 
-setLogging(logging.DEBUG)
+set_loglevel(logging.DEBUG)
 
 
 def log(*args, level=logging.INFO):
     msg = " ".join([str(a) for a in list(args)])
     if type(level) == int:
         logger.log(level, msg)
     elif type(level) == str:
@@ -482,15 +478,15 @@
 
 def warning(*args, level=logging.WARNING):
     msg = " ".join([str(a) for a in list(args)])
     logger.log(level, msg)
 
 
 # Extras
-def validateUrl(url):
+def validate_url(url):
     if has_validators:
         return validators.url(url)
     else:
         log("You do not have the validators module installed! run `pip install validators` to use this functionality")
 
 
 def m2list(args):
```

### Comparing `re-ircbot-1.7.0/LICENSE` & `re_ircbot-2.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `re-ircbot-1.7.0/PKG-INFO` & `re_ircbot-2.0.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 1.7.0
+Version: 2.0.0.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet
-Requires-Python: >=3.4
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cachetools==5.3.0
 
 [![Pypi](https://badge.fury.io/py/re-ircbot.svg)](https://pypi.org/project/re-ircbot/)
 [![Chat with me on irc](https://img.shields.io/badge/-IRC-gray?logo=gitter)](https://mangle.ga/irc)
 
 # re-ircbot, a simple irc bot library
 
 This is a simple irc bot library that uses trio for async callback processing and allows you to
@@ -329,9 +328,7 @@
 For version 2.0:
 
 1. [ ] SASL AUTHENTICATION
 2. [x] Handle weird character's on input (Colors, fonts, underlines, glyphs etc)
 3. [ ] Convert utils to an actual class that can be used as a context
 4. [x] Dcc file transfer
 
-
-
```

### Comparing `re-ircbot-1.7.0/README.md` & `re_ircbot-2.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `re-ircbot-1.7.0/re_ircbot.egg-info/PKG-INFO` & `re_ircbot-2.0.0.dev0/re_ircbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 1.7.0
+Version: 2.0.0.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet
-Requires-Python: >=3.4
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cachetools==5.3.0
 
 [![Pypi](https://badge.fury.io/py/re-ircbot.svg)](https://pypi.org/project/re-ircbot/)
 [![Chat with me on irc](https://img.shields.io/badge/-IRC-gray?logo=gitter)](https://mangle.ga/irc)
 
 # re-ircbot, a simple irc bot library
 
 This is a simple irc bot library that uses trio for async callback processing and allows you to
@@ -329,9 +328,7 @@
 For version 2.0:
 
 1. [ ] SASL AUTHENTICATION
 2. [x] Handle weird character's on input (Colors, fonts, underlines, glyphs etc)
 3. [ ] Convert utils to an actual class that can be used as a context
 4. [x] Dcc file transfer
 
-
-
```

### Comparing `re-ircbot-1.7.0/setup.py` & `re_ircbot-2.0.0.dev0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 import re
-import setuptools
 import subprocess
 
-VERSION = "1.6.5",
-BRANCH = "main"
+import setuptools
+
+VERSION = "2.0.0-dev"
+BRANCH = "v2"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+
 def requirements():
     """Build the requirements list for this project"""
     requirements_list = []
 
-    with open('requirements.txt') as requirements:
+    with open("requirements.txt") as requirements:
         for install in requirements:
             requirements_list.append(install.strip())
     return requirements_list
 
+
 def exec(cmd):
     """Execute a command and return the output"""
     return subprocess.check_output(cmd, stderr=subprocess.STDOUT, shell=True).decode().strip()
 
+
 def git_version_tag():
     """Get the current git version tag"""
     branch = exec("git rev-parse --abbrev-ref HEAD")
-    version = re.match(r"^v[0-9]+(\.[0-9]+)*$", exec("git describe --tags --abbrev=0"))
+    version = re.match(r"^v[0-9]+(\.[0-9]+)*.*$", exec("git describe --tags --abbrev=0"))
     if branch == BRANCH and version:
         return version[0][1:]
     else:
         return VERSION
 
+
 requirements = requirements()
 
-VERSION = git_version_tag()
+# VERSION = git_version_tag()
 print(f"BUILDING Version: {VERSION}")
 
 setuptools.setup(
     name="re-ircbot",
     version=VERSION,
     author="Matheus Fillipe",
     author_email="mattf@tilde.club",
@@ -51,9 +56,9 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Communications :: Chat",
         "Topic :: Internet",
     ],
-    python_requires=">=3.4",
+    python_requires=">=3.10",
 )
```

