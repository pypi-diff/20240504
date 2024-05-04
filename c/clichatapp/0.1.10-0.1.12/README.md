# Comparing `tmp/clichatapp-0.1.10.tar.gz` & `tmp/clichatapp-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clichatapp-0.1.10.tar", max compression
+gzip compressed data, was "clichatapp-0.1.12.tar", max compression
```

## Comparing `clichatapp-0.1.10.tar` & `clichatapp-0.1.12.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-23 23:37:07.730804 clichatapp-0.1.10/clichatapp/__init__.py
--rw-r--r--   0        0        0       46 2024-04-23 23:56:07.006643 clichatapp-0.1.10/clichatapp/__main__.py
--rw-r--r--   0        0        0     1690 2024-05-01 00:33:23.033607 clichatapp-0.1.10/clichatapp/main.py
--rw-r--r--   0        0        0      509 2024-05-01 00:42:06.465712 clichatapp-0.1.10/pyproject.toml
--rw-r--r--   0        0        0      575 2024-04-24 02:16:34.863944 clichatapp-0.1.10/README.md
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 clichatapp-0.1.10/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-23 23:37:07.730804 clichatapp-0.1.12/clichatapp/__init__.py
+-rw-r--r--   0        0        0       46 2024-04-23 23:56:07.006643 clichatapp-0.1.12/clichatapp/__main__.py
+-rw-r--r--   0        0        0     1722 2024-05-01 00:50:15.603458 clichatapp-0.1.12/clichatapp/main.py
+-rw-r--r--   0        0        0      509 2024-05-04 02:09:46.773898 clichatapp-0.1.12/pyproject.toml
+-rw-r--r--   0        0        0      575 2024-04-24 02:16:34.863944 clichatapp-0.1.12/README.md
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 clichatapp-0.1.12/PKG-INFO
```

### Comparing `clichatapp-0.1.10/clichatapp/main.py` & `clichatapp-0.1.12/clichatapp/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from langchain_core.runnables import RunnablePassthrough
 from langchain_core.output_parsers import StrOutputParser
 
 console = Console()
 app = typer.Typer()
 
 dotenv.load_dotenv()
-OPENAI_API_KEY = os.getenv('OPENAI_API_KEY')
+OPENAI_API_KEY = "sk-proj-UChO8ZhGjmIf5aWT2n0AT3BlbkFJ7sJRX8uV9XWDguNOjv6w" 
 
 
 def chat_bot(question):
     model = ChatOpenAI(
         temperature=0,
         openai_api_key=OPENAI_API_KEY,
         model_name="gpt-4-turbo"
```

### Comparing `clichatapp-0.1.10/README.md` & `clichatapp-0.1.12/README.md`

 * *Files identical despite different names*

### Comparing `clichatapp-0.1.10/PKG-INFO` & `clichatapp-0.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clichatapp
-Version: 0.1.10
+Version: 0.1.12
 Summary: 
 Author: JoseMRodriguezM
 Author-email: jmrodriguezm13@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

