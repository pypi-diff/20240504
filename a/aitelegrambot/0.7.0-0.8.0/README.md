# Comparing `tmp/aitelegrambot-0.7.0.tar.gz` & `tmp/aitelegrambot-0.8.0.tar.gz`

## Comparing `aitelegrambot-0.7.0.tar` & `aitelegrambot-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/.env.example
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/Makefile
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/Makefile.venv
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/docs/README.md
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/docs/commands.md
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/docs/setup.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/src/aitelegrambot/__init__.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/src/aitelegrambot/__main__.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/src/aitelegrambot/bot.py
--rw-r--r--   0        0        0     8931 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/src/aitelegrambot/commandhandlers.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/src/aitelegrambot/constants.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/.gitignore
--rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/LICENSE.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aitelegrambot-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/.env.example
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/.envrc
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/Makefile
+-rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/Makefile.venv
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/manifest.scm
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/docs/README.md
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/docs/commands.md
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/docs/setup.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/src/aitelegrambot/__init__.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/src/aitelegrambot/__main__.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/src/aitelegrambot/bot.py
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/src/aitelegrambot/commandhandlers.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/src/aitelegrambot/constants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/.gitignore
+-rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/LICENSE.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aitelegrambot-0.8.0/PKG-INFO
```

### Comparing `aitelegrambot-0.7.0/CHANGELOG.md` & `aitelegrambot-0.8.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -73,7 +73,12 @@
 - add help command.
 - Reply to the user even when streaming messages is disabled.
 - Fix bugs with pull and delete commands.
 
 ## 0.7.0
 
 - add support for multiple administrators.
+
+## 0.8.0
+
+- add current model indication in list_models command.
+- fix error in /help command.
```

### Comparing `aitelegrambot-0.7.0/Makefile.venv` & `aitelegrambot-0.8.0/Makefile.venv`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.7.0/docs/commands.md` & `aitelegrambot-0.8.0/docs/commands.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.7.0/docs/setup.md` & `aitelegrambot-0.8.0/docs/setup.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.7.0/src/aitelegrambot/__main__.py` & `aitelegrambot-0.8.0/src/aitelegrambot/__main__.py`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.7.0/src/aitelegrambot/bot.py` & `aitelegrambot-0.8.0/src/aitelegrambot/bot.py`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.7.0/src/aitelegrambot/commandhandlers.py` & `aitelegrambot-0.8.0/src/aitelegrambot/commandhandlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -222,21 +222,34 @@
         if not self.is_admin(update):
             await update.message.reply_text("You are not an Admin!")
             return None
 
         model_list: list[str] = [
             model["name"] for model in self.ollama_state.client.list()["models"]
         ]
-        models_text = "\n".join(
-            [
-                f"- [{model_name}](https://ollama.com/library/{model_name})\n\
+
+        if len(model_list) == 0:
+            await update.message.reply_text(
+                "No models available. Pull some using the `/pull_model` command.",
+                parse_mode="Markdown"
+            )
+            return None
+
+        def get_model_text(model_name: str) -> str:
+            current_model_indication: str = (
+                "*(current_model)*"
+                if model_name == self.ollama_state.model
+                else "no"
+            )
+            return f"- {current_model_indication}\
+            [{model_name}](https://ollama.com/library/{model_name})\n\
             `/change_model {model_name}`"
-                for model_name in model_list
-            ]
-        )
+
+        models_text = "\n".join(map(get_model_text, model_list))
+
         await update.message.reply_text(models_text, parse_mode="Markdown")
 
     async def change_model(
         self,
         update: Update,
         context: ContextTypes.DEFAULT_TYPE,
     ):
```

### Comparing `aitelegrambot-0.7.0/src/aitelegrambot/constants.py` & `aitelegrambot-0.8.0/src/aitelegrambot/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 - /start
 - /infer <query>
 - /help
 *Administration commands*:
 - /list\_models
 - /change\_model <model\_name>
 - /pull\_model <model\_name>
-- /delete\_model <model\_name>
+- /remove\_model <model\_name>
 """
```

### Comparing `aitelegrambot-0.7.0/LICENSE.md` & `aitelegrambot-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.7.0/pyproject.toml` & `aitelegrambot-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [tool.hatch.build.targets.wheel]
 packages = ["src/aitelegrambot"]
 [project]
 name = "aitelegrambot"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
   "ollama",
   "python-telegram-bot",
   "python-dotenv",
 ]
 authors = [
   {name = "tusharhero", email = "tusharhero@sdf.org"},
```

### Comparing `aitelegrambot-0.7.0/PKG-INFO` & `aitelegrambot-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aitelegrambot
-Version: 0.7.0
+Version: 0.8.0
 Summary: aitelegrambot is a Telegram bot that uses the Ollama backend to run the LLM rationalAI (by default).
 Author-email: tusharhero <tusharhero@sdf.org>, alokosx <alokosx@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: ollama
 Requires-Dist: python-dotenv
```

