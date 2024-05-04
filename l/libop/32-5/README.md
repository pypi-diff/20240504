# Comparing `tmp/libop-32.tar.gz` & `tmp/libop-5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libop-32.tar", last modified: Sat May  4 20:54:58 2024, max compression
+gzip compressed data, was "libop-5.tar", last modified: Sun Dec 31 20:26:04 2023, max compression
```

## Comparing `libop-32.tar` & `libop-5.tar`

### file list

```diff
@@ -1,36 +1,51 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-04 20:54:58.927616 libop-32/
--rw-r--r--   0 bart      (1000) bart      (1001)     4021 2024-05-04 20:54:58.927616 libop-32/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     3487 2024-05-04 20:39:30.000000 libop-32/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-04 20:54:58.923617 libop-32/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     3804 2024-05-04 20:19:14.000000 libop-32/bin/op
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-04 20:54:58.923617 libop-32/libop.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     4021 2024-05-04 20:54:58.000000 libop-32/libop.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      507 2024-05-04 20:54:58.000000 libop-32/libop.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-04 20:54:58.000000 libop-32/libop.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        3 2024-05-04 20:54:58.000000 libop-32/libop.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-04 20:54:58.000000 libop-32/libop.egg-info/zip-safe
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-04 20:54:58.927616 libop-32/op/
--rw-r--r--   0 bart      (1000) bart      (1001)       72 2024-05-03 13:32:18.000000 libop-32/op/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      745 2024-05-04 17:39:21.000000 libop-32/op/brokers.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4339 2024-05-04 17:35:21.000000 libop-32/op/handler.py
--rw-r--r--   0 bart      (1000) bart      (1001)      470 2024-05-04 19:39:39.000000 libop-32/op/logging.py
--rw-r--r--   0 bart      (1000) bart      (1001)      774 2024-05-04 17:35:08.000000 libop-32/op/message.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-04 20:54:58.927616 libop-32/op/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)      335 2024-05-04 17:52:27.000000 libop-32/op/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      217 2024-05-04 16:28:20.000000 libop-32/op/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      378 2024-05-04 19:41:51.000000 libop-32/op/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)    18763 2024-05-04 17:42:03.000000 libop-32/op/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      677 2024-05-04 17:42:30.000000 libop-32/op/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)      385 2024-05-03 12:59:45.000000 libop-32/op/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1001)    10747 2024-05-04 17:43:05.000000 libop-32/op/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1107 2024-05-04 17:43:22.000000 libop-32/op/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)      990 2024-05-04 17:40:37.000000 libop-32/op/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5142 2024-05-04 17:43:44.000000 libop-32/op/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6308 2024-05-04 16:37:10.000000 libop-32/op/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1601 2024-05-04 17:39:09.000000 libop-32/op/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4050 2024-05-04 17:36:18.000000 libop-32/op/storage.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4177 2024-05-04 19:41:26.000000 libop-32/op/threads.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1299 2024-05-04 01:54:25.000000 libop-32/op/utility.py
--rw-r--r--   0 bart      (1000) bart      (1001)      828 2024-05-04 20:24:44.000000 libop-32/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-05-04 20:54:58.927616 libop-32/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)      164 2024-05-01 15:00:55.000000 libop-32/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-12-31 20:26:04.121652 libop-5/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1219 2023-12-31 20:26:04.121652 libop-5/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      684 2023-12-31 20:25:48.000000 libop-5/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-12-31 20:26:04.117653 libop-5/libop.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1219 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      719 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        3 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/zip-safe
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-12-31 20:26:04.117653 libop-5/op/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1159 2023-12-31 14:57:27.000000 libop-5/op/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      131 2023-12-31 14:57:27.000000 libop-5/op/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      796 2023-12-31 19:31:40.000000 libop-5/op/brokers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      597 2023-12-31 19:31:09.000000 libop-5/op/clients.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      557 2023-12-31 14:57:27.000000 libop-5/op/collect.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      741 2023-12-31 19:31:36.000000 libop-5/op/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      413 2023-12-31 14:57:27.000000 libop-5/op/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1551 2023-12-31 19:31:28.000000 libop-5/op/excepts.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1230 2023-12-31 20:17:14.000000 libop-5/op/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2089 2023-12-31 14:57:27.000000 libop-5/op/locates.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      969 2023-12-31 19:31:46.000000 libop-5/op/message.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-12-31 20:26:04.121652 libop-5/op/mods/
+-rw-r--r--   0 bart      (1000) bart      (1000)      553 2023-12-31 20:17:54.000000 libop-5/op/mods/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      200 2023-12-31 14:57:34.000000 libop-5/op/mods/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      134 2023-12-31 14:57:34.000000 libop-5/op/mods/dbg.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      473 2023-12-31 14:57:34.000000 libop-5/op/mods/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      718 2023-12-31 14:57:34.000000 libop-5/op/mods/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    16008 2023-12-31 15:00:03.000000 libop-5/op/mods/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      629 2023-12-31 14:57:34.000000 libop-5/op/mods/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3496 2023-12-31 14:57:34.000000 libop-5/op/mods/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    16920 2023-12-31 14:57:34.000000 libop-5/op/mods/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      189 2023-12-31 14:57:34.000000 libop-5/op/mods/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      624 2023-12-31 14:57:34.000000 libop-5/op/mods/mre.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      390 2023-12-31 14:57:34.000000 libop-5/op/mods/pwd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2349 2023-12-31 14:57:34.000000 libop-5/op/mods/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6982 2023-12-31 14:57:34.000000 libop-5/op/mods/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2638 2023-12-31 14:57:34.000000 libop-5/op/mods/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1025 2023-12-31 14:57:34.000000 libop-5/op/mods/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      984 2023-12-31 14:57:34.000000 libop-5/op/mods/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1920 2023-12-31 14:57:34.000000 libop-5/op/mods/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2817 2023-12-31 14:57:34.000000 libop-5/op/mods/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5766 2023-12-31 14:57:34.000000 libop-5/op/mods/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5608 2023-12-31 15:00:22.000000 libop-5/op/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6125 2023-12-31 14:57:27.000000 libop-5/op/parsers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4958 2023-12-31 20:22:00.000000 libop-5/op/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2709 2023-12-31 14:57:27.000000 libop-5/op/storage.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2437 2023-12-31 19:31:59.000000 libop-5/op/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1000)       62 2023-12-31 14:57:27.000000 libop-5/op/utility.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      899 2023-12-31 20:21:50.000000 libop-5/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-12-31 20:26:04.121652 libop-5/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2023-12-31 14:56:01.000000 libop-5/setup.py
```

### Comparing `libop-32/bin/op` & `libop-5/op/runtime.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,97 @@
-#!/usr/bin/env python3
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0413
+# pylint: disable=C,R,W0201,W0212,W0105,W0613,W0406,E0102,W0611,W0718,W0125,E0401
 
 
-"main"
+"runtime"
 
 
 import getpass
+import inspect
 import os
 import pwd
-import readline
 import sys
 import termios
 import time
+import _thread
 
 
-sys.path.insert(0, os.getcwd())
+from .clients import Client
+from .command import Command
+from .default import Default
+from .excepts import Error, debug
+from .message import Event
+from .objects import Object
+from .parsers import parse_command, spl
+from .storage import Storage, cdir
+from .threads import launch
+
+
+def __dir__():
+    return (
+        'Cfg',
+        'Console',
+        'cmnd',
+        'daemon',
+        'forever',
+        'main',
+        'privileges',
+        'scan',
+        'wrap',
+        'wrapped'
+    )
+
+
+__all__ = __dir__()
+
+
+Cfg         = Default()
+Cfg.mod     = "cmd,err,mod,mre,pwd,thr"
+Cfg.name    = "op"
+Cfg.version = "5"
+Cfg.wd      = os.path.expanduser(f"~/.{Cfg.name}")
+Cfg.pidfile = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
+Cfg.user    = getpass.getuser()
+Storage.wd  = Cfg.wd
 
 
-from op.message import Event
-from op.handler import Client, parse_cmd
-from op.storage import Workdir, skel
-from op.logging import debug, enable
-from op.objects import Default, cdir
-from op.runtime import broker, cmnd, dte, init, scan
-from op.threads import errors, setout
-
-
-from op import modules
-
-
-Cfg             = Default()
-Cfg.dis         = ""
-Cfg.mod         = "cmd,mod"
-Cfg.opts        = ""
-Cfg.name        = __file__.rsplit(os.sep, maxsplit=1)[-1]
-Cfg.version     = "32"
-Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
-Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
-
-
-Workdir.workdir = Cfg.wdr
+from . import mods as modules
 
 
 class Console(Client):
 
-    "Console"
-
-    def __init__(self):
-        Client.__init__(self)
-        broker.add(self)
-
     def announce(self, txt):
-        "disable announce."
+        pass
 
     def callback(self, evt):
-        "wait for callback."
         Client.callback(self, evt)
         evt.wait()
 
-    def poll(self):
-        "poll console and create event."
+    def poll(self) -> Event:
         evt = Event()
         evt.orig = object.__repr__(self)
         evt.txt = input("> ")
         evt.type = "command"
         return evt
 
-    def say(self, _channel, txt):
-        "print to console"
+    def say(self, channel, txt):
         txt = txt.encode('utf-8', 'replace').decode()
         print(txt)
 
 
+def cmnd(txt):
+    evn = Event()
+    evn.txt = txt
+    Command.handle(evn)
+    evn.wait()
+    return evn
+
+
 def daemon(pidfile, verbose=False):
-    "switch to background."
-    # pylint: disable=W0212
     pid = os.fork()
     if pid != 0:
         os._exit(0)
     os.setsid()
     pid2 = os.fork()
     if pid2 != 0:
         os._exit(0)
@@ -96,67 +107,101 @@
     if os.path.exists(pidfile):
         os.unlink(pidfile)
     cdir(os.path.dirname(pidfile))
     with open(pidfile, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
+def forever():
+    while 1:
+        try:
+            time.sleep(1.0)
+        except (KeyboardInterrupt, EOFError):
+            _thread.interrupt_main()
+
+
 def privileges(username):
-    "drop privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
-def wrap(func):
-    "restore console."
+def scan(pkg, modstr, initer=False, wait=True) -> []:
+    mds = []
+    for modname in spl(modstr):
+        module = getattr(pkg, modname, None)
+        if not module:
+            continue
+        for _key, cmd in inspect.getmembers(module, inspect.isfunction):
+            if 'event' in cmd.__code__.co_varnames:
+                Command.add(cmd)
+        for _key, clz in inspect.getmembers(module, inspect.isclass):
+            if not issubclass(clz, Object):
+                continue
+            Storage.add(clz)
+        if initer and "init" in dir(module):
+            module._thr = launch(module.init, name=f"init {modname}")
+            mds.append(module)
+    if wait and initer:
+        for mod in mds:
+            mod._thr.join()
+    return mds
+
+
+def main():
+    Storage.skel()
+    parse_command(Cfg, " ".join(sys.argv[1:]))
+    if "a" in Cfg.opts:
+        Cfg.mod = ",".join(modules.__dir__())
+    if "v" in Cfg.opts:
+        dte = time.ctime(time.time()).replace("  ", " ")
+        debug(f"{Cfg.name.upper()} started {Cfg.opts.upper()} started {dte}")
+    if "d" in Cfg.opts:
+        daemon(Cfg.pidfile)
+        moddir = os.path.join(Storage.wd, "mods")
+        if os.path.exists(moddir) and "m" in Cfg.opts:
+            sys.path.insert(0, os.path.dirname(moddir))
+            import mods
+            if "a" in Cfg.opts:
+                Cfg.mod += "," +  ",".join(mods.__dir__())
+            scan(mods, Cfg.mod, True)
+        privileges(Cfg.user)
+        scan(modules, Cfg.mod, True)
+        forever()
+        return
+    if os.path.exists("mods") and "m" in Cfg.opts:
+        import mods
+        if "a" in Cfg.opts:
+            Cfg.mod += "," +  ",".join(mods.__dir__())
+        scan(mods, Cfg.mod)
+    csl = Console()
+    if "c" in Cfg.opts:
+        scan(modules, Cfg.mod, True, True)
+        csl.start()
+        forever()
+    if Cfg.otxt:
+        scan(modules, Cfg.mod)
+        return cmnd(Cfg.otxt)
+
+
+def wrap(func) -> None:
     old2 = None
     try:
         old2 = termios.tcgetattr(sys.stdin.fileno())
     except termios.error:
         pass
     try:
         func()
     except (KeyboardInterrupt, EOFError):
         print("")
     finally:
         if old2:
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old2)
 
 
-def main():
-    "main"
-    parse_cmd(Cfg, " ".join(sys.argv[1:]))
-    skel()
-    if "a" in Cfg.opts:
-        Cfg.mod = ",".join(modules.__dir__())
-    setout(print)
-    if "v" in Cfg.opts:
-        enable(print)
-        debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} {Cfg.mod.upper()} started {dte}")
-    if "h" in Cfg.opts:
-        print(__doc__)
-    elif "d" in Cfg.opts:
-        Cfg.mod  = ",".join(modules.__dir__())
-        Cfg.user = getpass.getuser()
-        daemon(Cfg.pidfile, "v" in Cfg.opts)
-        scan(modules, Cfg.mod)
-        privileges(Cfg.user)
-        init(modules, Cfg.mod)
-        while 1:
-            time.sleep(1.0)
-    elif "c" in Cfg.opts:
-        scan(modules, Cfg.mod, Cfg.sets.dis)
-        init(modules, Cfg.mod, Cfg.sets.dis)
-        csl = Console()
-        csl.start()
-        while 1:
-            time.sleep(1.0)
-    elif Cfg.otxt:
-        scan(modules, Cfg.mod, Cfg.sets.dis)
-        cmnd(Cfg.otxt, print)
+def wrapped():
+    wrap(main)
+    Error.show()
 
 
 if __name__ == "__main__":
-    readline.redisplay()
-    wrap(main)
-    errors()
+    wrapped()
```

### Comparing `libop-32/op/modules/irc.py` & `libop-5/op/mods/irc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,47 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,R,E1101,W0105,W0718,W0612,E0611
 
 
 "internet relay chat"
 
 
-import base64
 import os
 import queue
 import socket
 import ssl
 import textwrap
 import threading
 import time
 import _thread
 
 
-from op.storage import last, sync, whitelist
-from op.message import Event
-from op.handler import Client, command
-from op.logging import Logging, debug
-from op.objects import Default, Object, edit, fmt, keys, values
-from op.runtime import broker
-from op.threads import later, launch
+from .. import Default, Object, edit, fmt, keys
+from .. import Client, Command, Error, Event
+from .. import byorig, debug, last, launch, write
 
 
-NAME    = __file__.split(os.sep)[-3]
-saylock = _thread.allocate_lock()
+Error.filter = ["PING", "PONG", "PRIVMSG"]
+
 
+NAME = "op"
 
-Logging.filter = ["PING", "PONG", "PRIVMSG"]
+
+saylock = _thread.allocate_lock()
 
 
 def init():
-    "initialize a irc bot."
     irc = IRC()
     irc.start()
     irc.events.joined.wait()
     return irc
 
 
-def shutdown():
-    "shutdown irc bot."
-    for bot in values(broker.objs):
-        if "irc" not in str(type(bot)).lower():
-            continue
-        debug(f"IRC stopping {repr(bot)}")
-        bot.state.pongcheck = True
-        bot.state.keeprunning = False
-        bot.events.connected.clear()
-        bot.stop()
-
-
-class Config(Default): # pylint: disable=R0902,R0903
-
-    "Config"
+class Config(Default):
 
     channel = f'#{NAME}'
     commands = True
     control = '!'
     edited = time.time()
     nick = NAME
     port = 6667
@@ -77,21 +61,16 @@
         self.nick = self.nick or Config.nick
         self.port = self.port or Config.port
         self.realname = self.realname or Config.realname
         self.server = self.server or Config.server
         self.username = self.username or Config.username
 
 
-whitelist(Config)
-
-
 class TextWrap(textwrap.TextWrapper):
 
-    "TextWrap"
-
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = False
         self.fix_sentence_endings = True
         self.replace_whitespace = True
         self.tabsize = 4
@@ -99,54 +78,46 @@
 
 
 wrapper = TextWrap()
 
 
 class Output():
 
-    "Output"
-
     cache = Object()
 
     def __init__(self):
         self.dostop = threading.Event()
         self.oqueue = queue.Queue()
 
     def dosay(self, channel, txt):
-        "overload this."
         raise NotImplementedError
 
     @staticmethod
     def extend(channel, txtlist):
-        "add list of txt to channel cache."
         if channel not in Output.cache:
             Output.cache[channel] = []
-        chanlist = getattr(Output.cache, channel)
-        chanlist.extend(txtlist)
+        Output.cache[channel].extend(txtlist)
 
     @staticmethod
     def gettxt(channel):
-        "return text from channel cache."
         txt = None
         try:
             che = getattr(Output.cache, channel, None)
             if che:
                 txt = che.pop(0)
         except (KeyError, IndexError):
             pass
         return txt
 
     def oput(self, channel, txt):
-        "put text to output queue."
-        if channel and channel not in dir(Output.cache):
+        if channel not in dir(Output.cache):
             setattr(Output.cache, channel, [])
         self.oqueue.put_nowait((channel, txt))
 
     def out(self):
-        "output loop."
         while not self.dostop.is_set():
             (channel, txt) = self.oqueue.get()
             if channel is None and txt is None:
                 break
             if self.dostop.is_set():
                 break
             txtlist = wrapper.wrap(txt)
@@ -161,39 +132,34 @@
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
     @staticmethod
     def size(chan):
-        "return size of channel cache."
         if chan in Output.cache:
-            return len(getattr(Output.cache, chan, []))
+            return len(Output.cache.get(chan, []))
         return 0
 
 
 class IRC(Client, Output):
 
-    "IRC"
-
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
-        self.channels = []
         self.events = Default()
         self.events.authed = threading.Event()
         self.events.connected = threading.Event()
         self.events.joined = threading.Event()
         self.events.ready = threading.Event()
+        self.channels = []
         self.sock = None
         self.state = Default()
-        self.state.dostop = False
-        self.state.error = ""
         self.state.keeprunning = False
         self.state.lastline = ""
         self.state.nrconnect = 0
         self.state.nrsend = 0
         self.zelf = ''
         self.register('903', cb_h903)
         self.register('904', cb_h903)
@@ -201,23 +167,20 @@
         self.register('CAP', cb_cap)
         self.register('ERROR', cb_error)
         self.register('LOG', cb_log)
         self.register('NOTICE', cb_notice)
         self.register('PRIVMSG', cb_privmsg)
         self.register('QUIT', cb_quit)
         self.register("366", cb_ready)
-        broker.add(self)
 
     def announce(self, txt):
-        "announce on all channels."
         for channel in self.channels:
             self.oput(channel, txt)
 
-    def docommand(self, cmd, *args):
-        "send command to server."
+    def command(self, cmd, *args):
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
                 self.raw(f'{cmd.upper()} {args[0]}')
             elif len(args) == 2:
                 txt = ' '.join(args[1:])
@@ -226,15 +189,14 @@
                 txt = ' '.join(args[2:])
                 self.raw("{cmd.upper()} {args[0]} {args[1]} :{txt}")
             if (time.time() - self.state.last) < 5.0:
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
-        "connect to server."
         self.state.nrconnect += 1
         self.events.connected.clear()
         if self.cfg.password:
             debug("using SASL")
             self.cfg.sasl = True
             self.cfg.port = "6697"
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
@@ -253,113 +215,101 @@
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
-        "send text directly on the socket."
         with saylock:
             self.raw(txt)
             time.sleep(2.0)
 
     def disconnect(self):
-        "disconnect from server."
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
-               ) as _ex:
+               ) as ex:
             pass
-        except Exception as ex: # pylint: disable=W0718
-            later(ex)
+        except Exception as ex:
+            Error.errors.append(ex)
 
     def doconnect(self, server, nck, port=6667):
-        "loop until connected."
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
                     OSError,
                     ConnectionResetError
                    ) as ex:
-                self.state.error = str(ex)
+                self.state.errors = str(ex)
                 debug(str(ex))
             debug(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def event(self, txt):
-        "create an event."
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
-            self.docommand('PONG', evt.txt or '')
+            self.command('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
         if cmd == '001':
             self.state.needconnect = False
             if self.cfg.servermodes:
-                self.docommand(f'MODE {self.cfg.nick} {self.cfg.servermodes}')
+                self.command(f'MODE {self.cfg.nick} {self.cfg.servermodes}')
             self.zelf = evt.args[-1]
         elif cmd == "376":
             self.joinall()
         elif cmd == '002':
             self.state.host = evt.args[2][:-1]
         elif cmd == '366':
-            self.state.error = ""
+            self.state.errors = []
             self.events.joined.set()
         elif cmd == '433':
-            self.state.error = txt
+            self.state.errors = txt
             nck = self.cfg.nick + '_'
-            self.docommand('NICK', nck)
+            self.command('NICK', nck)
         return evt
 
     def joinall(self):
-        "join all channels."
         for channel in self.channels:
-            self.docommand('JOIN', channel)
+            self.command('JOIN', channel)
 
     def keep(self):
-        "keep alive."
         while not self.stopped.is_set():
-            if self.state.stopkeep:
-                self.state.stopkeep = False
-                break
             self.events.connected.wait()
             self.events.authed.wait()
             self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
-            self.docommand('PING', self.cfg.server)
+            self.command('PING', self.cfg.server)
             if self.state.pongcheck:
                 debug("failed pongcheck, restarting")
                 self.state.pongcheck = False
                 self.state.keeprunning = False
                 self.events.connected.clear()
                 self.stop()
                 init()
                 break
 
     def logon(self, server, nck):
-        "log onto server,"
         self.events.connected.wait()
         self.events.authed.wait()
         self.direct(f'NICK {nck}')
         self.direct(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
-        "parse text into an event."
-        # pylint: disable=R0912,R0915
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
         debug(txt)
         obj = Event()
         obj.args = []
         obj.rawstr = rawstr
@@ -413,15 +363,14 @@
             obj.rest = " ".join(obj.args)
         obj.orig = object.__repr__(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
-        "poll for event."
         self.events.connected.wait()
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
@@ -429,27 +378,26 @@
                     OSError,
                     socket.timeout,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                later(ex)
+                Error.add(ex)
                 self.stop()
                 debug("handler stopped")
                 evt = self.event(str(ex))
                 return evt
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
     def raw(self, txt):
-        "send raw text."
         txt = txt.rstrip()
         debug(txt)
         txt = txt[:500]
         txt += '\r\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
@@ -457,214 +405,173 @@
             except (
                     OSError,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                later(ex)
+                Error.errors.append(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
-        "reconnect to server."
         debug(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
         self.events.connected.clear()
         self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
 
     def dosay(self, channel, txt):
-        "method for output cache."
         self.events.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
-        self.docommand('PRIVMSG', channel, txt)
+        self.command('PRIVMSG', channel, txt)
 
     def say(self, channel, txt):
-        "say text on channel."
         self.oput(channel, txt)
 
     def some(self):
-        "parse part of input text."
         self.events.connected.wait()
         if not self.sock:
             return
         inbytes = self.sock.recv(512)
         txt = str(inbytes, 'utf-8')
         if txt == '':
             raise ConnectionResetError
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
-        "start bot."
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.events.connected.clear()
         self.events.joined.clear()
         launch(Output.out, self)
-        launch(Client.start, self)
+        Client.start(self)
         launch(
                self.doconnect,
                self.cfg.server or "localhost",
                self.cfg.nick,
                int(self.cfg.port or '6667')
               )
         if not self.state.keeprunning:
             launch(self.keep)
 
     def stop(self):
-        "stop bot."
-        self.state.stopkeep = True
         self.disconnect()
         self.dostop.set()
         self.oput(None, None)
         Client.stop(self)
 
     def wait(self):
-        "wait for ready."
         self.events.ready.wait()
 
 
-def cb_auth(bot, evt):
-    "auth callback."
-    bot.docommand(f'AUTHENTICATE {bot.cfg.password}')
+def cb_auth(evt):
+    bot = byorig(evt.orig)
+    bot.command(f'AUTHENTICATE {bot.cfg.password}')
 
 
-def cb_cap(bot, evt):
-    "capabilities callback."
+def cb_cap(evt):
+    bot = byorig(evt.orig)
     if bot.cfg.password and 'ACK' in evt.arguments:
         bot.direct('AUTHENTICATE PLAIN')
     else:
         bot.direct('CAP REQ :sasl')
 
 
-def cb_error(bot, evt):
-    "error callback."
-    if not bot.state.nrerror:
-        bot.state.nrerror = 0
+def cb_error(evt):
+    bot = byorig(evt.orig)
     bot.state.nrerror += 1
-    bot.state.error = evt.txt
+    bot.state.errors.append(evt.txt)
     debug(evt.txt)
 
 
-def cb_h903(bot, evt):
-    "auth succeded callback."
+def cb_h903(evt):
+    bot = byorig(evt.orig)
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
-def cb_h904(bot, evt):
-    "auth succeded callback."
+def cb_h904(evt):
+    bot = byorig(evt.orig)
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
-def cb_kill(bot, evt):
-    "got killed callback."
+def cb_kill(evt):
+    pass
 
 
-def cb_log(bot, evt):
-    "log callback."
+def cb_log(evt):
+    pass
 
 
-def cb_ready(bot, evt):
-    "bot is ready callback."
-    bot.events.ready.set()
+def cb_ready(evt):
+    bot = byorig(evt.orig)
+    if bot:
+        bot.events.ready.set()
 
 
-def cb_001(bot, evt):
-    "first line received callback."
+def cb_001(evt):
+    bot = byorig(evt.orig)
     bot.logon()
 
 
-def cb_notice(bot, evt):
-    "notice callback."
+def cb_notice(evt):
+    bot = byorig(evt.orig)
     if evt.txt.startswith('VERSION'):
         txt = f'\001VERSION {NAME.upper()} 140 - {bot.cfg.username}\001'
-        bot.docommand('NOTICE', evt.channel, txt)
+        bot.command('NOTICE', evt.channel, txt)
 
 
-def cb_privmsg(bot, evt):
-    "privmsg callback."
+def cb_privmsg(evt):
+    bot = byorig(evt.orig)
     if not bot.cfg.commands:
         return
     if evt.txt:
         if evt.txt[0] in ['!',]:
             evt.txt = evt.txt[1:]
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
             evt.txt = evt.txt[len(bot.cfg.nick)+1:]
         else:
             return
         if evt.txt:
             evt.txt = evt.txt[0].lower() + evt.txt[1:]
         debug(f"command from {evt.origin}: {evt.txt}")
-        command(bot, evt)
+        Command.handle(evt)
 
 
-def cb_quit(bot, evt):
-    "quit callback."
+def cb_quit(evt):
+    bot = byorig(evt.orig)
     debug(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
+"commands"
+
+
 def cfg(event):
-    "configure command."
     config = Config()
     path = last(config)
     if not event.sets:
         event.reply(
                     fmt(
                         config,
                         keys(config),
                         skip='control,password,realname,sleep,username'.split(",")
                        )
                    )
     else:
         edit(config, event.sets)
-        sync(config, path)
+        write(config, path)
         event.reply('ok')
-
-
-def mre(event):
-    "show from output cache."
-    if not event.channel:
-        event.reply('channel is not set.')
-        return
-    bot = broker.get(event.orig)
-    if 'cache' not in dir(bot):
-        event.reply('bot is missing cache')
-        return
-    if event.channel not in bot.cache:
-        event.reply(f'no output in {event.channel} cache.')
-        return
-    for _x in range(3):
-        txt = bot.gettxt(event.channel)
-        if txt:
-            bot.say(event.channel, txt)
-    size = bot.size(event.channel)
-    event.reply(f'{size} more in cache')
-
-
-def pwd(event):
-    "create a base64 password."
-    if len(event.args) != 2:
-        event.reply('pwd <nick> <password>')
-        return
-    arg1 = event.args[0]
-    arg2 = event.args[1]
-    txt = f'\x00{arg1}\x00{arg2}'
-    enc = txt.encode('ascii')
-    base = base64.b64encode(enc)
-    dcd = base.decode('ascii')
-    event.reply(dcd)
```

### Comparing `libop-32/op/modules/tdo.py` & `libop-5/op/mods/tdo.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,56 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=R0903
+# pylint: disable=C0115,C0116,R0903,W0105,E0402,E0611
+
 
 "todo list"
 
 
 import time
 
 
-from ..storage import fntime, find, sync
-from ..objects import Object
-from ..utility import laps
+from .. import Object, fntime, find, laps, write
 
 
 class NoDate(Exception):
 
-    "no matching date"
+    pass
 
 
 class Todo(Object):
 
-    "Todo"
-
     def __init__(self):
         Object.__init__(self)
         self.txt = ''
 
 
 def dne(event):
-    "flag todo as done."
     if not event.args:
         event.reply("dne <txt>")
         return
     selector = {'txt': event.args[0]}
     nmr = 0
     for fnm, obj in find('todo', selector):
         nmr += 1
         obj.__deleted__ = True
-        sync(obj, fnm)
+        write(obj, fnm)
         event.reply('ok')
         break
     if not nmr:
         event.reply("nothing todo")
 
 
 def tdo(event):
-    "add todo."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('todo'):
             lap = laps(time.time()-fntime(fnm))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
             event.reply("no todo")
         return
     obj = Todo()
     obj.txt = event.rest
-    sync(obj)
+    write(obj)
     event.reply('ok')
```

### Comparing `libop-32/op/modules/thr.py` & `libop-5/op/mods/thr.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C0116,W0105,E0402,E0401,E0611
 
 
 "show running threads"
 
 
 import threading
 import time
 
 
-from ..objects import Object, update
-from ..utility import laps
+from .. import Object, laps, update
 
 
 STARTTIME = time.time()
 
 
 def thr(event):
-    "show running threads."
     result = []
     for thread in sorted(threading.enumerate(), key=lambda x: x.name):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, 'sleep', None):
```

### Comparing `libop-32/op/modules/tmr.py` & `libop-5/op/parsers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,R,W0718,W0702
 
 
-"timer"
+"parsing text"
 
 
 import datetime
+import os
 import re
 import time as ttime
 
 
-from ..storage import find, sync
-from ..message import Event
-from ..objects import update
-from ..runtime import broker
-from ..threads import Timer, launch
-from ..utility import laps
+from .default import Default
 
 
-def init():
-    "start timers."
-    for _fn, obj in find("timer"):
-        if "time" not in obj:
-            continue
-        diff = float(obj.time) - ttime.time()
-        if diff > 0:
-            bot = broker.first()
-            evt = Event()
-            update(evt, obj)
-            evt.orig = object.__repr__(bot)
-            timer = Timer(diff, evt.show)
-            launch(timer.start)
+def __dir__():
+    return (
+        'NoDate',
+        'fntime',
+        'get_day',
+        'get_hour',
+        'get_time',
+        'laps',
+        'parse_command',
+        'parse_time',
+        'spl',
+        'today',
+        'to_day'
+    )
+
 
+__all__ = __dir__()
 
-MONTHS = [
+
+bdmonths = [
     'Bo',
     'Jan',
     'Feb',
     'Mar',
     'Apr',
     'May',
     'Jun',
@@ -45,67 +47,69 @@
     'Sep',
     'Oct',
     'Nov',
     'Dec'
 ]
 
 
-FORMATS = [
+year_formats = [
     "%Y-%m-%d",
     "%d-%m-%Y",
     "%d-%m",
     "%m-%d",
 ]
 
 
 class NoDate(Exception):
 
-    "NoDate"
+    pass
 
 
 def extract_date(daystr):
-    "extract date from string."
-    res = None
-    for fmt in FORMATS:
+    for fmt in year_formats:
         try:
             res = ttime.mktime(ttime.strptime(daystr, fmt))
-            break
-        except ValueError:
+        except:
             res = None
-    return res
+        if res:
+            return res
+
+
+def fntime(daystr) -> float:
+    daystr = daystr.replace('_', ':')
+    datestr = ' '.join(daystr.split(os.sep)[-2:])
+    if '.' in datestr:
+        datestr, rest = datestr.rsplit('.', 1)
+    else:
+        rest = ''
+    timed = ttime.mktime(ttime.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
+    if rest:
+        timed += float('.' + rest)
+    return timed
 
 
 def get_day(daystr):
-    "return day from string."
-    day = None
-    month = None
-    yea = None
     try:
         ymdre = re.search(r'(\d+)-(\d+)-(\d+)', daystr)
-        if ymdre:
-            (day, month, yea) = ymdre.groups()
-    except ValueError:
+        (day, month, yea) = ymdre.groups()
+    except:
         try:
             ymre = re.search(r'(\d+)-(\d+)', daystr)
-            if ymre:
-                (day, month) = ymre.groups()
-                yea = ttime.strftime("%Y", ttime.localtime())
-        except Exception as ex: # pylint: disable=W0212
+            (day, month) = ymre.groups()
+            yea = ttime.strftime("%Y", ttime.localtime())
+        except Exception as ex:
             raise NoDate(daystr) from ex
-    if day:
-        day = int(day)
-        month = int(month)
-        yea = int(yea)
-        date = f"{day} {MONTHS[month]} {yea}"
-        return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
-    raise NoDate(daystr)
+    day = int(day)
+    month = int(month)
+    yea = int(yea)
+    date = "%s %s %s" % (day, bdmonths[month], yea)
+    return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
 
 
 def get_hour(daystr):
-    "return hour from string."
     try:
         hmsre = re.search(r'(\d+):(\d+):(\d+)', str(daystr))
         hours = 60 * 60 * (int(hmsre.group(1)))
         hoursmin = hours  + int(hmsre.group(2)) * 60
         hmsres = hoursmin + int(hmsre.group(3))
     except AttributeError:
         pass
@@ -119,27 +123,117 @@
         return 0
     except ValueError:
         return 0
     return hmsres
 
 
 def get_time(txt):
-    "parse full time string."
     try:
         target = get_day(txt)
     except NoDate:
         target = to_day(today())
     hour =  get_hour(txt)
     if hour:
         target += hour
     return target
 
 
+def laps(seconds, short=True) -> str:
+    txt = ""
+    nsec = float(seconds)
+    if nsec < 1:
+        return f"{nsec:.2f}s"
+    yea = 365*24*60*60
+    week = 7*24*60*60
+    nday = 24*60*60
+    hour = 60*60
+    minute = 60
+    yeas = int(nsec/yea)
+    nsec -= yeas*yea
+    weeks = int(nsec/week)
+    nsec -= weeks*week
+    nrdays = int(nsec/nday)
+    nsec -= nrdays*nday
+    hours = int(nsec/hour)
+    nsec -= hours*hour
+    minutes = int(nsec/minute)
+    nsec -= int(minute*minutes)
+    sec = int(nsec)
+    if yeas:
+        txt += f"{yeas}y"
+    if weeks:
+        nrdays += weeks * 7
+    if nrdays:
+        txt += f"{nrdays}d"
+    if short and txt:
+        return txt.strip()
+    if hours:
+        txt += f"{hours}h"
+    if minutes:
+        txt += f"{minutes}m"
+    if sec:
+        txt += f"{sec}s"
+    txt = txt.strip()
+    return txt
+
+
+def parse_command(obj, txt=None) -> None:
+    args = []
+    obj.args    = obj.args or []
+    obj.cmd     = obj.cmd or ""
+    obj.gets    = obj.gets or Default()
+    obj.hasmods = obj.hasmod or False
+    obj.index   = None
+    obj.mod     = obj.mod or ""
+    obj.opts    = obj.opts or ""
+    obj.result  = obj.reult or []
+    obj.sets    = obj.sets or Default()
+    obj.txt     = txt or obj.txt or ""
+    obj.otxt    = obj.txt
+    _nr = -1
+    for spli in obj.otxt.split():
+        if spli.startswith("-"):
+            try:
+                obj.index = int(spli[1:])
+            except ValueError:
+                obj.opts += spli[1:]
+            continue
+        if "==" in spli:
+            key, value = spli.split("==", maxsplit=1)
+            if key in obj.gets:
+                val = getattr(obj.gets, key)
+                value = val + "," + value
+            setattr(obj.gets, key, value)
+            continue
+        if "=" in spli:
+            key, value = spli.split("=", maxsplit=1)
+            if key == "mod":
+                obj.hasmods = True
+                if obj.mod:
+                    obj.mod += f",{value}"
+                else:
+                    obj.mod = value
+                continue
+            setattr(obj.sets, key, value)
+            continue
+        _nr += 1
+        if _nr == 0:
+            obj.cmd = spli
+            continue
+        args.append(spli)
+    if args:
+        obj.args = args
+        obj.txt  = obj.cmd or ""
+        obj.rest = " ".join(obj.args)
+        obj.txt  = obj.cmd + " " + obj.rest
+    else:
+        obj.txt = obj.cmd or ""
+
+
 def parse_time(txt):
-    "parse time from string."
     seconds = 0
     target = 0
     txt = str(txt)
     for word in txt.split():
         if word.startswith("+"):
             seconds = int(word[1:])
             return ttime.time() + seconds
@@ -153,75 +247,33 @@
             target = to_day(today())
         hour =  get_hour(txt)
         if hour:
             target += hour
     return target
 
 
+def spl(txt) -> []:
+    try:
+        res = txt.split(',')
+    except (TypeError, ValueError):
+        res = txt
+    return [x for x in res if x]
+
+
 def to_day(daystr):
-    "parse day from string."
     previous = ""
     line = ""
     daystr = str(daystr)
-    res = None
     for word in daystr.split():
         line = previous + " " + word
         previous = word
         try:
             res = extract_date(line.strip())
-            break
         except ValueError:
             res = None
+        if res:
+            return res
         line = ""
-    return res
 
 
 def today():
-    "return date."
     return str(datetime.datetime.today()).split()[0]
-
-
-def tmr(event):
-    "add a timer."
-    result = ""
-    if not event.rest:
-        nmr = 0
-        for _fn, obj in find('timer'):
-            lap = float(obj.time) - ttime.time()
-            if lap > 0:
-                event.reply(f'{nmr} {obj.txt} {laps(lap)}')
-                nmr += 1
-        return result
-    seconds = 0
-    line = ""
-    for word in event.args:
-        if word.startswith("+"):
-            try:
-                seconds = int(word[1:])
-            except (ValueError, IndexError):
-                event.reply(f"{seconds} is not an integer")
-                return result
-        else:
-            line += word + " "
-    if seconds:
-        target = ttime.time() + seconds
-    else:
-        try:
-            target = get_day(event.rest)
-        except NoDate:
-            target = to_day(today())
-        hour =  get_hour(event.rest)
-        if hour:
-            target += hour
-    if not target or ttime.time() > target:
-        event.reply("already passed given time.")
-        return result
-    event.time = target
-    diff = target - ttime.time()
-    event.reply("ok " +  laps(diff))
-    event.result = []
-    event.result.append(event.rest)
-    timer = Timer(diff, event.show, thrname=event.cmd)
-    update(timer, event)
-    sync(timer)
-    launch(timer.start)
-    return result
```

### Comparing `libop-32/op/objects.py` & `libop-5/op/objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,166 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=R0902,R0903,W0105
+# pylint: disable=C,R,E0603,E0402,W0401,W0614,W0611,W0622,W0105
 
 
-"clean namespace"
+"a clean namespace"
 
 
+import datetime
 import json
 import os
-import pathlib
-import _thread
+import sys
+import types
 
 
-lock = _thread.allocate_lock()
+def __dir__():
+    return (
+            'Object',
+            'construct',
+            'dump',
+            'dumps',
+            'edit',
+            'fmt',
+            'fqn',
+            'ident',
+            'items',
+            'keys',
+            'load',
+            'loads',
+            'name',
+            'update',
+            'values',
+           )
+
+
+__all__ = __dir__()
 
 
 class Object:
 
-    "Object"
 
     def __contains__(self, key):
         return key in dir(self)
 
     def __iter__(self):
         return iter(self.__dict__)
 
     def __len__(self):
         return len(self.__dict__)
 
+    def __repr__(self):
+        return dumps(self)
+
     def __str__(self):
         return str(self.__dict__)
 
 
-def construct(obj, *args, **kwargs):
-    "construct an object from provided arguments."
+"decoder"
+
+
+class ObjectDecoder(json.JSONDecoder):
+
+    def decode(self, s, _w=None):
+        val = json.JSONDecoder.decode(self, s)
+        if not val:
+            val = {}
+        return hook(val)
+
+    def raw_decode(self, s, idx=0):
+        return json.JSONDecoder.raw_decode(self, s, idx)
+
+
+def hook(objdict, typ=None) -> Object:
+    if typ:
+        obj = typ()
+    else:
+        obj = Object()
+    construct(obj, objdict)
+    return obj
+
+
+def load(fpt, *args, **kw) -> Object:
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.load(fpt, *args, **kw)
+
+
+def loads(string, *args, **kw) -> Object:
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.loads(string, *args, **kw)
+
+
+"encoder"
+
+
+class ObjectEncoder(json.JSONEncoder):
+
+    def default(self, o) -> str:
+        if isinstance(o, dict):
+            return o.items()
+        if isinstance(o, Object):
+            return vars(o)
+        if isinstance(o, list):
+            return iter(o)
+        if isinstance(
+                      o,
+                      (
+                       type(str),
+                       type(True),
+                       type(False),
+                       type(int),
+                       type(float)
+                      )
+                     ):
+            return o
+        try:
+            return json.JSONEncoder.default(self, o)
+        except TypeError:
+            return object.__repr__(o)
+
+    def encode(self, o) -> str:
+        return json.JSONEncoder.encode(self, o)
+
+    def iterencode(
+                   self,
+                   o,
+                   _one_shot=False
+                  ) -> str:
+        return json.JSONEncoder.iterencode(self, o, _one_shot)
+
+
+def dump(*args, **kw) -> None:
+    kw["cls"] = ObjectEncoder
+    return json.dump(*args, **kw)
+
+
+def dumps(*args, **kw) -> str:
+    kw["cls"] = ObjectEncoder
+    return json.dumps(*args, **kw)
+
+
+"methods"
+
+
+def construct(obj, *args, **kwargs) -> None:
     if args:
         val = args[0]
         if isinstance(val, zip):
             update(obj, dict(val))
         elif isinstance(val, dict):
             update(obj, val)
         elif isinstance(val, Object):
             update(obj, vars(val))
     if kwargs:
         update(obj, kwargs)
 
 
-def edit(obj, setter, skip=False):
-    "edit an object from provided dict/dict-like."
+def edit(obj, setter, skip=False) -> None:
     for key, val in items(setter):
         if skip and val == "":
             continue
         try:
             setattr(obj, key, int(val))
             continue
         except ValueError:
@@ -65,16 +174,15 @@
             setattr(obj, key, True)
         elif val in ["False", "false"]:
             setattr(obj, key, False)
         else:
             setattr(obj, key, val)
 
 
-def fmt(obj, args=None, skip=None, plain=False):
-    "format an object to a printable string."
+def fmt(obj, args=None, skip=None, plain=False) -> str:
     if args is None:
         args = keys(obj)
     if skip is None:
         skip = []
     txt = ""
     for key in args:
         if key.startswith("__"):
@@ -85,212 +193,60 @@
         if value is None:
             continue
         if plain:
             txt += f"{value} "
         elif isinstance(value, str) and len(value.split()) >= 2:
             txt += f'{key}="{value}" '
         else:
-            txt += f"{key}={value} "
+            txt += f'{key}={value} '
     return txt.strip()
 
 
-def fqn(obj):
-    "return full qualified name of an object."
+def fqn(obj) -> str:
     kin = str(type(obj)).split()[-1][1:-2]
     if kin == "type":
         kin = obj.__name__
     return kin
 
 
-def items(obj):
-    "return the items of an object."
+def ident(obj) -> str:
+    return os.path.join(
+                        fqn(obj),
+                        os.path.join(*str(datetime.datetime.now()).split())
+                       )
+
+def items(obj) -> []:
     if isinstance(obj, type({})):
         return obj.items()
     return obj.__dict__.items()
 
 
-def keys(obj):
-    "return keys of an object."
+def keys(obj) -> []:
     if isinstance(obj, type({})):
         return obj.keys()
     return list(obj.__dict__.keys())
 
 
-def read(obj, pth):
-    "read an object from file path."
-    with lock:
-        with open(pth, 'r', encoding='utf-8') as ofile:
-            update(obj, load(ofile))
-
-
-def search(obj, selector):
-    "check if object matches provided values."
-    res = False
-    if not selector:
-        return True
-    for key, value in items(selector):
-        val = getattr(obj, key, None)
-        if str(value).lower() in str(val).lower():
-            res = True
-        else:
-            res = False
-            break
-    return res
+def name(obj) -> str:
+    typ = type(obj)
+    if isinstance(typ, types.ModuleType):
+        return obj.__name__
+    if '__self__' in dir(obj):
+        return f'{obj.__self__.__class__.__name__}.{obj.__name__}'
+    if '__class__' in dir(obj) and '__name__' in dir(obj):
+        return f'{obj.__class__.__name__}.{obj.__name__}'
+    if '__class__' in dir(obj):
+        return f"{obj.__class__.__module__}.{obj.__class__.__name__}"
+    if '__name__' in dir(obj):
+        return f'{obj.__class__.__name__}.{obj.__name__}'
+    return None
 
 
-def update(obj, data, empty=True):
-    "update an object."
+def update(obj, data, empty=True) -> None:
     for key, value in items(data):
         if empty and not value:
             continue
         setattr(obj, key, value)
 
 
-def values(obj):
-    "return values of an object."
+def values(obj) -> []:
     return obj.__dict__.values()
-
-
-def write(obj, pth):
-    "write an object to disk."
-    with lock:
-        cdir(os.path.dirname(pth))
-        with open(pth, 'w', encoding='utf-8') as ofile:
-            dump(obj, ofile, indent=4)
-
-
-"default"
-
-
-class Default(Object):
-
-    "Default"
-
-    def __getattr__(self, key):
-        return self.__dict__.get(key, "")
-
-
-
-"decoder"
-
-
-class ObjectDecoder(json.JSONDecoder):
-
-    "ObjectDecoder"
-
-    def __init__(self, *args, **kwargs):
-        json.JSONDecoder.__init__(self, *args, **kwargs)
-
-    def decode(self, s, _w=None):
-        "decoding string to object."
-        val = json.JSONDecoder.decode(self, s)
-        if not val:
-            val = {}
-        return hook(val)
-
-    def raw_decode(self, s, idx=0):
-        "decode partial string to object."
-        return json.JSONDecoder.raw_decode(self, s, idx)
-
-
-def hook(objdict, typ=None):
-    "construct object from dict."
-    if typ:
-        obj = typ()
-    else:
-        obj = Object()
-    construct(obj, objdict)
-    return obj
-
-
-def load(fpt, *args, **kw):
-    "load object from file."
-    kw["cls"] = ObjectDecoder
-    kw["object_hook"] = hook
-    return json.load(fpt, *args, **kw)
-
-
-def loads(string, *args, **kw):
-    "load object from string."
-    kw["cls"] = ObjectDecoder
-    kw["object_hook"] = hook
-    return json.loads(string, *args, **kw)
-
-
-"encoder"
-
-
-class ObjectEncoder(json.JSONEncoder):
-
-    "ObjectEncoder"
-
-    def __init__(self, *args, **kwargs):
-        json.JSONEncoder.__init__(self, *args, **kwargs)
-
-    def default(self, o):
-        "return stringable value."
-        if isinstance(o, dict):
-            return o.items()
-        if isinstance(o, Object):
-            return vars(o)
-        if isinstance(o, list):
-            return iter(o)
-        if isinstance(o, (type(str), type(True), type(False), type(int), type(float))):
-            return o
-        try:
-            return json.JSONEncoder.default(self, o)
-        except TypeError:
-            return o.__dict__
-
-    def encode(self, o) -> str:
-        "encode object to string."
-        return json.JSONEncoder.encode(self, o)
-
-    def iterencode(self, o, _one_shot=False):
-        "loop over object to encode to string."
-        return json.JSONEncoder.iterencode(self, o, _one_shot)
-
-
-def dump(*args, **kw):
-    "dump object to file."
-    kw["cls"] = ObjectEncoder
-    return json.dump(*args, **kw)
-
-
-def dumps(*args, **kw):
-    "dump object to string."
-    kw["cls"] = ObjectEncoder
-    return json.dumps(*args, **kw)
-
-
-def cdir(pth):
-    "create directory."
-    if os.path.exists(pth):
-        return
-    pth = pathlib.Path(pth)
-    os.makedirs(pth, exist_ok=True)
-
-
-"interface"
-
-
-def __dir__():
-    return (
-        'Object',
-        'Default',
-        'construct',
-        'dump',
-        'dumps',
-        'edit',
-        'fmt',
-        'fqn',
-        'hook',
-        'items',
-        'keys',
-        'load',
-        'loads',
-        'read',
-        'search',
-        'update',
-        'values',
-        'write'
-    )
```

### Comparing `libop-32/pyproject.toml` & `libop-5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 [build-system]
 requires = [
     "setuptools>=43.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
+
 [project]
 name = "libop"
 description = "original programmer"
-version = "32"
+version = "5"
 authors = [
-    {name = "Bart Thate",email = "bthate@dds.nl"},
+    {name = "Bart Thate",email = "libbotx@gmail.com"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
     'License :: Public Domain',
     'Operating System :: Unix',
     'Programming Language :: Python',
     'Topic :: Utilities'
 ]
 
+
 [project.urls]
 "home" = "https://pypi.org/project/libop"
-"bugs" = "https://github.com/xobjectz/libop/issues"
-"source" = "https://github.com/xobjectz/libop"
+"bugs" = "https://github.com/botlibx/libop/issues"
+"source" = "https://github.com/botlibx/libop"
 
 
 [tool.setuptools]
-script-files = [
-    'bin/op',
-]
 packages = [
-    "op",
-    "op.modules"
+    'op',
+    'op.mods'
 ]
 zip-safe=true
 
 
 [tool.setuptools.data-files]
 "share/doc/libop" = [
-    "README.rst"
+    "README.rst",
 ]
+
+
+[tool.setuptools.exclude-package-data]
+"*" = [
+       "env*",
+       "html*",
+       "test*"
+      ]
```

