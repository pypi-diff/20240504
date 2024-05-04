# Comparing `tmp/pyprland-2.2.8.tar.gz` & `tmp/pyprland-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.2.8.tar", max compression
+gzip compressed data, was "pyprland-2.2.9.tar", max compression
```

## Comparing `pyprland-2.2.8.tar` & `pyprland-2.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.8/LICENSE
--rw-r--r--   0        0        0     4458 2024-04-14 21:04:51.031595 pyprland-2.2.8/README.md
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.8/pyprland/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.8/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.8/pyprland/adapters/colors.py
--rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.8/pyprland/adapters/menus.py
--rw-r--r--   0        0        0     1395 2024-04-08 20:00:16.866561 pyprland-2.2.8/pyprland/adapters/units.py
--rwxr-xr-x   0        0        0    16724 2024-04-16 20:54:29.573076 pyprland-2.2.8/pyprland/command.py
--rw-r--r--   0        0        0     7574 2024-04-16 20:17:47.161668 pyprland-2.2.8/pyprland/common.py
--rw-r--r--   0        0        0     7197 2024-04-12 17:07:08.504043 pyprland-2.2.8/pyprland/ipc.py
--rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.8/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.8/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1647 2024-04-15 15:21:49.122927 pyprland-2.2.8/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.8/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0     2018 2024-04-14 20:56:27.261784 pyprland-2.2.8/pyprland/plugins/gbar.py
--rw-r--r--   0        0        0     2589 2024-04-09 20:50:41.034540 pyprland-2.2.8/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.8/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.8/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.8/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0     8680 2024-04-13 18:26:06.759226 pyprland-2.2.8/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.8/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0     1770 2024-04-13 21:52:18.890816 pyprland-2.2.8/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0    26132 2024-04-14 20:57:42.622754 pyprland-2.2.8/pyprland/plugins/scratchpads/__init__.py
--rw-r--r--   0        0        0     2641 2024-04-12 17:24:50.007112 pyprland-2.2.8/pyprland/plugins/scratchpads/animations.py
--rw-r--r--   0        0        0     2106 2024-04-12 17:23:41.858277 pyprland-2.2.8/pyprland/plugins/scratchpads/helpers.py
--rw-r--r--   0        0        0     3436 2024-04-12 17:21:22.436949 pyprland-2.2.8/pyprland/plugins/scratchpads/lookup.py
--rw-r--r--   0        0        0     4136 2024-04-12 17:19:16.255742 pyprland-2.2.8/pyprland/plugins/scratchpads/objects.py
--rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.8/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     4161 2024-04-09 15:53:04.519223 pyprland-2.2.8/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     3983 2024-04-09 21:03:19.309538 pyprland-2.2.8/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.8/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.8/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     5335 2024-04-13 18:20:53.870052 pyprland-2.2.8/pyprland/plugins/wallpapers.py
--rw-r--r--   0        0        0     2559 2024-04-14 20:57:42.622754 pyprland-2.2.8/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0      725 2024-04-16 20:54:29.563076 pyprland-2.2.8/pyproject.toml
--rw-r--r--   0        0        0     4997 1970-01-01 00:00:00.000000 pyprland-2.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.9/LICENSE
+-rw-r--r--   0        0        0     4458 2024-04-14 21:04:51.031595 pyprland-2.2.9/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.9/pyprland/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.9/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.9/pyprland/adapters/colors.py
+-rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.9/pyprland/adapters/menus.py
+-rw-r--r--   0        0        0     1395 2024-04-08 20:00:16.866561 pyprland-2.2.9/pyprland/adapters/units.py
+-rwxr-xr-x   0        0        0    17129 2024-04-19 17:18:47.257998 pyprland-2.2.9/pyprland/command.py
+-rw-r--r--   0        0        0     7746 2024-04-19 16:25:06.663994 pyprland-2.2.9/pyprland/common.py
+-rw-r--r--   0        0        0     7233 2024-04-19 16:13:14.787837 pyprland-2.2.9/pyprland/ipc.py
+-rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.9/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.9/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1647 2024-04-19 16:13:14.787837 pyprland-2.2.9/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.9/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0     2018 2024-04-14 20:56:27.261784 pyprland-2.2.9/pyprland/plugins/gbar.py
+-rw-r--r--   0        0        0     2589 2024-04-09 20:50:41.034540 pyprland-2.2.9/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.9/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.9/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     1760 2024-04-19 16:13:14.787837 pyprland-2.2.9/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0     8680 2024-04-13 18:26:06.759226 pyprland-2.2.9/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.9/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0     2071 2024-04-19 16:25:06.663994 pyprland-2.2.9/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0    26354 2024-04-19 16:48:51.098660 pyprland-2.2.9/pyprland/plugins/scratchpads/__init__.py
+-rw-r--r--   0        0        0     2641 2024-04-12 17:24:50.007112 pyprland-2.2.9/pyprland/plugins/scratchpads/animations.py
+-rw-r--r--   0        0        0     2106 2024-04-12 17:23:41.858277 pyprland-2.2.9/pyprland/plugins/scratchpads/helpers.py
+-rw-r--r--   0        0        0     3436 2024-04-12 17:21:22.436949 pyprland-2.2.9/pyprland/plugins/scratchpads/lookup.py
+-rw-r--r--   0        0        0     4268 2024-04-19 16:46:31.746537 pyprland-2.2.9/pyprland/plugins/scratchpads/objects.py
+-rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.9/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     4161 2024-04-09 15:53:04.519223 pyprland-2.2.9/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     4062 2024-04-19 16:13:14.787837 pyprland-2.2.9/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.9/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.9/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     5335 2024-04-13 18:20:53.870052 pyprland-2.2.9/pyprland/plugins/wallpapers.py
+-rw-r--r--   0        0        0     2547 2024-04-19 16:13:14.787837 pyprland-2.2.9/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0      725 2024-04-19 17:18:47.247997 pyprland-2.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4997 1970-01-01 00:00:00.000000 pyprland-2.2.9/PKG-INFO
```

### Comparing `pyprland-2.2.8/LICENSE` & `pyprland-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/README.md` & `pyprland-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/adapters/menus.py` & `pyprland-2.2.9/pyprland/adapters/menus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/adapters/units.py` & `pyprland-2.2.9/pyprland/adapters/units.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/command.py` & `pyprland-2.2.9/pyprland/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,41 +70,42 @@
             fname = os.path.expandvars(os.path.expanduser(config_filename))
         else:
             if os.path.exists(OLD_CONFIG_FILE) and not os.path.exists(CONFIG_FILE):
                 self.log.warning("Consider changing your configuration to TOML format.")
             self.config.clear()
             fname = os.path.expanduser(CONFIG_FILE)
 
-        config = self.__load_config_file(fname)
+        try:
+            config = self.__load_config_file(fname)
+        except tomllib.TOMLDecodeError as e:
+            self.log.critical("Problem reading %s: %s", fname, e)
+            await notify_error(f"Pyprland failed to read config: {e}")
+            raise PyprError() from e
+        except FileNotFoundError as e:
+            self.log.critical("Unable to open %s: %s", fname, e)
+            await notify_error(f"Pyprland failed to read config: {e}")
+            raise PyprError() from e
 
         if not config_filename:
             for extra_config in list(config["pyprland"].get("include", [])):
                 merge(config, await self.__open_config(extra_config))
             self.config.update(config)
         return config
 
     def __load_config_file(self, fname):
         """Loads a configuration file and returns it as a dictionary"""
         config = {}
         if os.path.exists(fname):
             self.log.info("Loading %s", fname)
-            try:
-                with open(fname, "rb") as f:
-                    config = tomllib.load(f)
-            except FileNotFoundError as e:
-                self.log.critical("Problem reading %s: %s", fname, e)
-                raise PyprError() from e
+            with open(fname, "rb") as f:
+                config = tomllib.load(f)
         elif os.path.exists(os.path.expanduser(OLD_CONFIG_FILE)):
             self.log.info("Loading %s", OLD_CONFIG_FILE)
-            try:
-                with open(os.path.expanduser(OLD_CONFIG_FILE), encoding="utf-8") as f:
-                    config = json.loads(f.read())
-            except FileNotFoundError as e:
-                self.log.critical("Problem reading %s: %s", fname, e)
-                raise PyprError() from e
+            with open(os.path.expanduser(OLD_CONFIG_FILE), encoding="utf-8") as f:
+                config = json.loads(f.read())
         else:
             self.log.critical("Config file not found! Please create %s", fname)
             raise PyprError()
         return config
 
     async def _load_single_plugin(self, name, init) -> bool:
         "Load a single plugin, optionally calling `init`"
@@ -146,22 +147,25 @@
         for name in ["pyprland"] + self.config["pyprland"]["plugins"]:
             if name not in self.plugins:
                 if not await self._load_single_plugin(name, init):
                     continue
             if init:
                 try:
                     await self.plugins[name].load_config(self.config)
-                    await self.plugins[name].on_reload()
-                    self.plugins[name].log.info("configured")
+                    await asyncio.wait_for(self.plugins[name].on_reload(), timeout=5.0)
+                except asyncio.TimeoutError:
+                    self.plugins[name].log.info("timed out on reload")
                 except PyprError:
                     raise
                 except Exception as e:
                     await notify_info(f"Error initializing plugin {name}: {e}")
                     self.log.error("Error initializing plugin %s:", name, exc_info=True)
                     raise PyprError() from e
+                else:
+                    self.plugins[name].log.info("configured")
         if init_pyprland:
             plug = self.plugins["pyprland"]
             plug.set_commands(reload=self.load_config)  # type: ignore
 
     async def load_config(self, init=True):
         """loads the configuration (new plugins will be added & config updated)
 
@@ -286,15 +290,17 @@
                 task = await q.get()
                 if is_pyprland:
                     self.pyprland_mutex_event.clear()
             except RuntimeError as e:
                 self.log.error("Aborting [%s] loop: %s", name, e)
                 return
             try:
-                await task()
+                await asyncio.wait_for(task(), timeout=12.0)
+            except asyncio.TimeoutError:
+                self.log.error("Timeout running plugin %s::%s", name, task)
             except Exception as e:  # pylint: disable=W0718
                 self.log.error(
                     "Unhandled error running plugin %s::%s: %s", name, task, e
                 )
             if is_pyprland and q.empty():
                 self.pyprland_mutex_event.set()
 
@@ -355,15 +361,15 @@
     manager.log.debug("[ initialized ]".center(80, "="))
     try:
         await manager.run()
     except KeyboardInterrupt:
         print("Interrupted")
     except asyncio.CancelledError:
         manager.log.critical("cancelled")
-    finally:
+    else:
         events_writer.close()
         await events_writer.wait_closed()
         manager.server.close()
         await manager.server.wait_closed()
 
 
 def show_help(manager):
@@ -391,15 +397,15 @@
 
 
 async def run_client():
     "Runs the client (CLI)"
     manager = Pyprland()
 
     if sys.argv[1] == "version":
-        print("2.2.8")  # Automatically updated version
+        print("2.2.9")  # Automatically updated version
         return
 
     if sys.argv[1] == "edit":
         editor = os.environ.get("EDITOR", os.environ.get("VISUAL", "vi"))
         filename = os.path.expanduser(CONFIG_FILE)
         run_interactive_program(f'{editor} "{filename}"')
         sys.argv[1] = "reload"
```

### Comparing `pyprland-2.2.8/pyprland/common.py` & `pyprland-2.2.9/pyprland/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,22 +178,30 @@
     logger.propagate = False
     for handler in LogObjects.handlers:
         logger.addHandler(handler)
     logger.info('Logger "%s" initialized', name)
     return logger
 
 
+@dataclass(order=True)
+class VersionInfo:
+    major: int = 0
+    minor: int = 0
+    micro: int = 0
+
+
 @dataclass
 class SharedState:
     "Stores commonly requested properties"
     active_workspace: str = ""  # workspace name
     active_monitor: str = ""  # monitor name
     active_window: str = ""  # window address
     variables: dict = field(default_factory=dict)
     monitors: list[str] = field(default_factory=list)
+    hyprland_version: VersionInfo = field(default_factory=VersionInfo)
 
 
 state = SharedState()
 """
 Exposes most-commonly accessed attributes to avoid specific IPC requests
 - `active_monitor` monitor's name
 - `active_workspace` workspace's name
```

### Comparing `pyprland-2.2.8/pyprland/ipc.py` & `pyprland-2.2.9/pyprland/ipc.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,16 @@
         raise ConnectionResetError() from exc
 
     return wrapper
 
 
 cached_responses: dict[str, list[Any]] = {
     # <command name>: [expiration_date, payload, retention_time]
-    "monitors": [0, None, 0.1],
+    "monitors": [0, None, 0.3],
+    # "workspaces": [0, None, 0.1],
     # "clients": [0, None, 0.02],
 }
 
 
 @retry_on_reset
 async def hyprctlJSON(
     command: str, logger=None
```

### Comparing `pyprland-2.2.8/pyprland/plugins/expose.py` & `pyprland-2.2.9/pyprland/plugins/expose.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/fetch_client_menu.py` & `pyprland-2.2.9/pyprland/plugins/fetch_client_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/gbar.py` & `pyprland-2.2.9/pyprland/plugins/gbar.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/interface.py` & `pyprland-2.2.9/pyprland/plugins/interface.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/layout_center.py` & `pyprland-2.2.9/pyprland/plugins/layout_center.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/lost_windows.py` & `pyprland-2.2.9/pyprland/plugins/lost_windows.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/monitors.py` & `pyprland-2.2.9/pyprland/plugins/monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/monitors_v0.py` & `pyprland-2.2.9/pyprland/plugins/monitors_v0.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/pyprland.py` & `pyprland-2.2.9/pyprland/plugins/pyprland.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 " Not a real Plugin - provides some core features and some caching of commonly requested structures "
 from .interface import Plugin
-from ..common import state
+from ..common import state, VersionInfo
 
 
 class Extension(Plugin):
     "Internal built-in plugin allowing caching states and implementing special commands"
 
     async def init(self):
         "initializes the plugin"
         state.active_window = ""
+        version = (await self.hyprctlJSON("version"))["tag"]
+        try:
+            state.hyprland_version = VersionInfo(
+                *(int(i) for i in version[1:].split(".")[:3])
+            )
+        except Exception:
+            self.log.error("Fail to parse hyprctl version.")
+
         state.active_workspace = (await self.hyprctlJSON("activeworkspace"))["name"]
         monitors = await self.hyprctlJSON("monitors")
         state.monitors = [mon["name"] for mon in monitors]
         state.active_monitor = next(mon["name"] for mon in monitors if mon["focused"])
 
     async def event_monitoradded(self, name):
         "track monitor"
```

### Comparing `pyprland-2.2.8/pyprland/plugins/scratchpads/__init__.py` & `pyprland-2.2.9/pyprland/plugins/scratchpads/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,21 +527,27 @@
 
         await self._show_transition(item, monitor, was_alive)
         item.monitor = monitor["name"]
 
     async def _show_transition(self, item, monitor, was_alive):
         "perfoms the transition to visible state"
         animation_type = item.conf.get("animation", "").lower()
-        wrkspc = monitor["activeWorkspace"]["name"]
+        forbid_special = not item.conf.get("allow_special_workspace", True)
+        wrkspc = (
+            monitor["activeWorkspace"]["name"]
+            if forbid_special or not monitor["specialWorkspace"]["name"]
+            else monitor["specialWorkspace"]["name"]
+        )
+
         item.meta["last_shown"] = time.time()
         # Start the transition
         await self.hyprctl(
             [
                 f"moveworkspacetomonitor special:scratch_{item.uid} {monitor['name']}",
-                f"movetoworkspacesilent name:{wrkspc},address:{item.full_address}",
+                f"movetoworkspacesilent {wrkspc},address:{item.full_address}",
                 f"alterzorder top,address:{item.full_address}",
             ]
         )
         preserve_aspect = self.cast_bool(item.conf.get("preserve_aspect"))
         should_set_aspect = (
             not (preserve_aspect and was_alive) or item.monitor != state.active_monitor
         )  # not aspect preserving or it's newly spawned
```

### Comparing `pyprland-2.2.8/pyprland/plugins/scratchpads/animations.py` & `pyprland-2.2.9/pyprland/plugins/scratchpads/animations.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/scratchpads/helpers.py` & `pyprland-2.2.9/pyprland/plugins/scratchpads/helpers.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/scratchpads/lookup.py` & `pyprland-2.2.9/pyprland/plugins/scratchpads/lookup.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/scratchpads/objects.py` & `pyprland-2.2.9/pyprland/plugins/scratchpads/objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Callable, cast
 from collections import defaultdict
 
 from aiofiles import os as aios
 from aiofiles import open as aiopen
 
 from ...ipc import notify_error
-from ...common import CastBoolMixin
+from ...common import CastBoolMixin, VersionInfo, state
 from .helpers import OverridableConfig, get_match_fn
 
 
 class Scratch(CastBoolMixin):  # {{{
     "A scratchpad state including configuration & client state"
     log = logging.getLogger("scratch")
     get_client_props: Callable
@@ -35,14 +35,17 @@
             opts["match_by"] = "class"
         if self.cast_bool(opts.get("preserve_aspect")):
             opts["lazy"] = True
         if not opts.get("process_tracking", True):
             opts["lazy"] = True
             if "match_by" not in opts:
                 opts["match_by"] = "class"
+        if state.hyprland_version < VersionInfo(0, 39, 0):
+            opts["allow_special_workspace"] = False
+
         self.conf = opts
 
     async def initialize(self, ex):
         "Initialize the scratchpad"
         if self.meta["initialized"]:
             return
         self.meta["initialized"] = True
```

### Comparing `pyprland-2.2.8/pyprland/plugins/shift_monitors.py` & `pyprland-2.2.9/pyprland/plugins/shift_monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.2.9/pyprland/plugins/shortcuts_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/system_notifier.py` & `pyprland-2.2.9/pyprland/plugins/system_notifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,19 +56,22 @@
             assert (
                 props["parser"] in self.parsers
             ), f"{props['parser']} was not found in {self.parsers}"
             self.log.debug("Loaded source %s => %s", props["command"], props["parser"])
             self.tasks.append(asyncio.create_task(self.start_source(props)))
 
     async def exit(self):
-        "empty exit function"
+        "exit function"
         self.running = False
         for task in self.tasks:
             task.cancel()
-            await task
+            try:
+                await task
+            except asyncio.CancelledError:
+                pass
         for source in self.sources.values():
             if source.pid is not None:
                 source.kill()
         self.tasks[:] = []
 
     async def start_source(self, props):
         "Start a source loop"
```

### Comparing `pyprland-2.2.8/pyprland/plugins/toggle_dpms.py` & `pyprland-2.2.9/pyprland/plugins/toggle_dpms.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/toggle_special.py` & `pyprland-2.2.9/pyprland/plugins/toggle_special.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/wallpapers.py` & `pyprland-2.2.9/pyprland/plugins/wallpapers.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.8/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.2.9/pyprland/plugins/workspaces_follow_focus.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         )
         workspaces = [
             w["name"]
             for w in cast(list[dict], await self.hyprctlJSON("workspaces"))
             if w["id"] > 0
         ]
 
-        batch: list[str | list[str]] = []
+        batch: list[str] = []
         for n in workspaces:
             if n in busy_workspaces or n == workspace_name:
                 continue
             batch.append(f"moveworkspacetomonitor name:{n} {monitor_id}")
         await self.hyprctl(batch)
 
     async def run_change_workspace(self, direction: str):
```

### Comparing `pyprland-2.2.8/pyproject.toml` & `pyprland-2.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprland"
-version = "2.2.8"
+version = "2.2.9"
 description = "Hyperland plugin system - batteries included"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyprland"}]
 homepage = "https://github.com/hyprland-community/pyprland/"
```

### Comparing `pyprland-2.2.8/PKG-INFO` & `pyprland-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.2.8
+Version: 2.2.9
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

