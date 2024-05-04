# Comparing `tmp/agentic_security-0.1.3.tar.gz` & `tmp/agentic_security-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentic_security-0.1.3.tar", max compression
+gzip compressed data, was "agentic_security-0.1.4.tar", max compression
```

## Comparing `agentic_security-0.1.3.tar` & `agentic_security-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11367 2024-04-27 14:28:28.279193 agentic_security-0.1.3/LICENSE
--rw-r--r--   0        0        0     9192 2024-04-27 14:28:28.279193 agentic_security-0.1.3/Readme.md
--rw-r--r--   0        0        0       64 2024-04-27 14:28:28.279193 agentic_security-0.1.3/agentic_security/__init__.py
--rw-r--r--   0        0        0      560 2024-04-27 14:28:28.279193 agentic_security-0.1.3/agentic_security/__main__.py
--rw-r--r--   0        0        0     8903 2024-04-27 14:28:28.279193 agentic_security-0.1.3/agentic_security/agent.py
--rw-r--r--   0        0        0     3833 2024-04-27 14:28:28.279193 agentic_security-0.1.3/agentic_security/app.py
--rw-r--r--   0        0        0     2900 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/http_spec.py
--rw-r--r--   0        0        0     2265 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/lib.py
--rw-r--r--   0        0        0        0 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/probe_actor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/probe_actor/__main__.py
--rw-r--r--   0        0        0     3355 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/probe_actor/fuzzer.py
--rw-r--r--   0        0        0     1209 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/probe_actor/refusal.py
--rw-r--r--   0        0        0      458 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/probe_actor/test_refusal.py
--rw-r--r--   0        0        0     3889 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/probe_data/__init__.py
--rw-r--r--   0        0        0     9183 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/probe_data/data.py
--rw-r--r--   0        0        0        0 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/probe_data/modules/__init__.py
--rw-r--r--   0        0        0     6593 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/probe_data/modules/adaptive_attacks.py
--rw-r--r--   0        0        0     2446 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/probe_data/modules/test_adaptive_attacks.py
--rw-r--r--   0        0        0     2645 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/probe_data/stenography_fn.py
--rw-r--r--   0        0        0      725 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/probe_data/test_data.py
--rw-r--r--   0        0        0     2365 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/report_chart.py
--rw-r--r--   0        0        0    26899 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/static/index.html
--rw-r--r--   0        0        0      656 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/test_lib.py
--rw-r--r--   0        0        0     1961 2024-04-27 14:28:28.283193 agentic_security-0.1.3/agentic_security/test_spec.py
--rw-r--r--   0        0        0     1340 2024-04-27 14:28:28.283193 agentic_security-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    10577 1970-01-01 00:00:00.000000 agentic_security-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11367 2024-05-04 09:49:34.419064 agentic_security-0.1.4/LICENSE
+-rw-r--r--   0        0        0     9128 2024-05-04 09:49:34.419064 agentic_security-0.1.4/Readme.md
+-rw-r--r--   0        0        0       64 2024-05-04 09:49:34.419064 agentic_security-0.1.4/agentic_security/__init__.py
+-rw-r--r--   0        0        0      595 2024-05-04 09:49:34.419064 agentic_security-0.1.4/agentic_security/__main__.py
+-rw-r--r--   0        0        0     8903 2024-05-04 09:49:34.419064 agentic_security-0.1.4/agentic_security/agent.py
+-rw-r--r--   0        0        0     5365 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/app.py
+-rw-r--r--   0        0        0     2900 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/http_spec.py
+-rw-r--r--   0        0        0     2265 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/lib.py
+-rw-r--r--   0        0        0        0 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_actor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_actor/__main__.py
+-rw-r--r--   0        0        0     3720 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_actor/fuzzer.py
+-rw-r--r--   0        0        0     1209 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_actor/refusal.py
+-rw-r--r--   0        0        0      458 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_actor/test_refusal.py
+-rw-r--r--   0        0        0     4325 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/__init__.py
+-rw-r--r--   0        0        0     9314 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/data.py
+-rw-r--r--   0        0        0        0 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/modules/__init__.py
+-rw-r--r--   0        0        0     6593 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/modules/adaptive_attacks.py
+-rw-r--r--   0        0        0     1910 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/modules/garak_tool.py
+-rw-r--r--   0        0        0     2446 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/modules/test_adaptive_attacks.py
+-rw-r--r--   0        0        0     2645 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/stenography_fn.py
+-rw-r--r--   0        0        0      725 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/test_data.py
+-rw-r--r--   0        0        0     2365 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/report_chart.py
+-rw-r--r--   0        0        0    27290 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/static/index.html
+-rw-r--r--   0        0        0      657 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/test_lib.py
+-rw-r--r--   0        0        0     1961 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/test_spec.py
+-rw-r--r--   0        0        0     1349 2024-05-04 09:49:34.423064 agentic_security-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    10514 1970-01-01 00:00:00.000000 agentic_security-0.1.4/PKG-INFO
```

### Comparing `agentic_security-0.1.3/LICENSE` & `agentic_security-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.3/Readme.md` & `agentic_security-0.1.4/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 <p align="center">
 
 <h1 align="center">Agentic Security</h1>
 
 <p align="center">
-    The open-source Agentic LLM Vulnerability Scanner .
-    <br />
-    <a href="#features"><strong>Learn more »</strong></a>
+    The open-source Agentic LLM Vulnerability Scanner
     <br />
     <br />
 
 <p>
 <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/msoedov/agentic_security" />
 <img alt="GitHub Last Commit" src="https://img.shields.io/github/last-commit/msoedov/agentic_security" />
 <img alt="" src="https://img.shields.io/github/repo-size/msoedov/agentic_security" />
@@ -20,15 +18,15 @@
 </p>
   </p>
 </p>
 
 ## Features
 
 - Customizable Rule Sets or Agent based attacks🛠️
-- Comprehansive fuzzing for any LLMs 🧪
+- Comprehensive fuzzing for any LLMs 🧪
 - LLM API integration and stress testing 🛠️
 - Wide range of fuzzing and attack techniques 🌀
 
 Note: Please be aware that Agentic Security is designed as a safety scanner tool and not a foolproof solution. It cannot guarantee complete protection against all possible threats.
 
 ## About the Project 🧙
 
@@ -113,15 +111,15 @@
 Authorization: Bearer XXXXX
 Content-Type: application/json
 
 {
     "prompt": "<<PROMPT>>"
 }
 """
-result = AgenticSecurity.scan(spec)
+result = AgenticSecurity.scan(llmSpec=spec)
 
 # module: failure rate
 # {"Local CSV": 79.65116279069767, "llm-adaptive-attacks": 20.0}
 exit(max(r.values()) > 20)
 ```
 
 ```
```

### Comparing `agentic_security-0.1.3/agentic_security/__main__.py` & `agentic_security-0.1.4/agentic_security/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 from agentic_security.app import app
 
 
 class T:
     def server(self, port=8718, host="0.0.0.0"):
         sys.path.append(os.path.dirname("."))
-        config = uvicorn.Config(app, port=port, host=host, log_level="info")
+        config = uvicorn.Config(
+            app, port=port, host=host, log_level="info", reload=True
+        )
         server = uvicorn.Server(config)
         server.run()
         return
 
     def headless(self):
         sys.path.append(os.path.dirname("."))
```

### Comparing `agentic_security-0.1.3/agentic_security/agent.py` & `agentic_security-0.1.4/agentic_security/agent.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.3/agentic_security/app.py` & `agentic_security-0.1.4/agentic_security/app.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import random
 import sys
+from asyncio import Event, Queue
 from datetime import datetime
 from pathlib import Path
 
 from fastapi import BackgroundTasks, FastAPI, HTTPException, Response
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import FileResponse, StreamingResponse
 from loguru import logger
@@ -35,14 +36,17 @@
     CORSMiddleware,
     allow_origins=origins,
     allow_credentials=True,
     allow_methods=["*"],  # Allows all methods
     allow_headers=["*"],  # Allows all headers
 )
 
+tools_inbox = Queue()
+FEATURE_PROXY = False
+
 
 @app.get("/")
 async def root():
     agentic_security_path = Path(__file__).parent
     return FileResponse(f"{agentic_security_path}/static/index.html")
 
 
@@ -84,14 +88,15 @@
     request_factory = LLMSpec.from_string(scan_parameters.llmSpec)
 
     async def _gen():
         async for scan_result in fuzzer.perform_scan(
             request_factory=request_factory,
             max_budget=scan_parameters.maxBudget,
             datasets=scan_parameters.datasets,
+            tools_inbox=tools_inbox,
         ):
             yield scan_result + "\n"  # Adding a newline for separation
 
     return _gen()
 
 
 @app.post("/scan")
@@ -145,7 +150,59 @@
     table: list[dict]
 
 
 @app.post("/plot.jpeg", response_class=Response)
 async def get_plot(table: Table):
     buf = plot_security_report(table.table)
     return StreamingResponse(buf, media_type="image/jpeg")
+
+
+class Message(BaseModel):
+    role: str
+    content: str
+
+
+class CompletionRequest(BaseModel):
+    model: str
+    messages: list[Message]
+    temperature: float
+    top_p: float
+    n: int
+    stop: list[str]
+    max_tokens: int
+    presence_penalty: float
+    frequency_penalty: float
+
+
+# OpenAI proxy endpoint
+@app.post("/proxy/chat/completions")
+async def proxy_completions(request: CompletionRequest):
+    refuse = random.random() < 0.2
+    message = random.choice(REFUSAL_MARKS) if refuse else "This is a test!"
+    prompt_content = " ".join(
+        [msg.content for msg in request.messages if msg.role == "user"]
+    )
+    message = prompt_content + " " + message
+    ready = Event()
+    ref = dict(message=message, reply="", ready=ready)
+    tools_inbox.put_nowait(ref)
+    if FEATURE_PROXY:
+        # Proxy to agent
+        await ready.wait()
+        reply = ref["reply"]
+        return reply
+    # Simulate a completion response
+    return {
+        "id": "chatcmpl-abc123",
+        "object": "chat.completion",
+        "created": 1677858242,
+        "model": "gpt-3.5-turbo-0613",
+        "usage": {"prompt_tokens": 13, "completion_tokens": 7, "total_tokens": 20},
+        "choices": [
+            {
+                "message": {"role": "assistant", "content": message},
+                "logprobs": None,
+                "finish_reason": "stop",
+                "index": 0,
+            }
+        ],
+    }
```

### Comparing `agentic_security-0.1.3/agentic_security/http_spec.py` & `agentic_security-0.1.4/agentic_security/http_spec.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.3/agentic_security/lib.py` & `agentic_security-0.1.4/agentic_security/lib.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import asyncio
 import json
 
 import colorama
 import tqdm.asyncio
+from tabulate import tabulate
+
 from agentic_security.app import Scan, streaming_response_generator
 from agentic_security.probe_data import REGISTRY
-from tabulate import tabulate
 
 RESET = colorama.Style.RESET_ALL
 BRIGHT = colorama.Style.BRIGHT
 RED = colorama.Fore.RED
 GREEN = colorama.Fore.GREEN
 
 
@@ -21,15 +22,14 @@
 {
     "prompt": "<<PROMPT>>"
 }
 """
 
 
 class AgenticSecurity:
-
     @classmethod
     async def async_scan(
         self, llmSpec: str, maxBudget: int, datasets: list[dict], max_th: float
     ):
         gen = streaming_response_generator(
             Scan(llmSpec=llmSpec, maxBudget=maxBudget, datasets=datasets)
         )
```

### Comparing `agentic_security-0.1.3/agentic_security/probe_actor/fuzzer.py` & `agentic_security-0.1.4/agentic_security/probe_actor/fuzzer.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,38 +26,53 @@
             cost=0,
             progress=0,
             failureRate=0,
             status=True,
         ).model_dump_json()
 
 
-async def perform_scan(request_factory, max_budget: int, datasets: list[dict] = []):
+async def prompt_iter(prompts):
+    if isinstance(prompts, list):
+        for p in prompts:
+            yield p
+        return
+    async for p in prompts:
+        yield p
+
+
+async def perform_scan(
+    request_factory, max_budget: int, datasets: list[dict] = [], tools_inbox=None
+):
     yield ScanResult.status_msg("Loading datasets...")
     if IS_VERCEL:
         yield ScanResult.status_msg(
             "Vercel deployment detected. Streaming messages are not supported by serverless, plz run it locally."
         )
         return
     prompt_modules = prepare_prompts(
         dataset_names=[m["dataset_name"] for m in datasets if m["selected"]],
         budget=max_budget,
+        tools_inbox=tools_inbox,
     )
     yield ScanResult.status_msg("Datasets loaded. Starting scan...")
 
     errors = []
     refusals = []
-    size = sum(len(m.prompts) for m in prompt_modules)
+    size = sum(len(m.prompts) for m in prompt_modules if not m.lazy)
     step = 0
     for mi, module in enumerate(prompt_modules):
         tokens = 0
         module_failures = 0
-        logger.info(f"Scanning {module.dataset_name} {len(module.prompts)}")
-        for i, prompt in enumerate(module.prompts):
+        size = 0 if module.lazy else len(module.prompts)
+        logger.info(f"Scanning {module.dataset_name} {size}")
+        i = 0
+        async for prompt in prompt_iter(module.prompts):
+            i += 1
             step += 1
-            progress = 100 * (step) / size
+            progress = 100 * (step) / size if size else 0
 
             # Naive token count
             tokens += len(prompt.split())
             try:
                 r = await request_factory.fn(prompt=prompt)
             except httpx.RequestError as e:
                 logger.error(f"Request error: {e}")
@@ -82,20 +97,21 @@
                         r.status_code,
                         r.text,
                     )
                 )
                 module_failures += 1
             # Naive token count for llm response
             tokens += len(r.text.split())
+            total = size if size else i
             yield ScanResult(
                 module=module.dataset_name,
                 tokens=round(tokens / 1000, 1),
                 cost=round(tokens * 1.5 / 1000_000, 2),
                 progress=round(progress, 2),
-                failureRate=100 * module_failures / max(len(module.prompts), 1),
+                failureRate=100 * module_failures / max(total, 1),
             ).model_dump_json()
     yield ScanResult.status_msg("Done.")
     import pandas as pd
 
     df = pd.DataFrame(
         errors + refusals, columns=["module", "prompt", "status_code", "content"]
     )
```

### Comparing `agentic_security-0.1.3/agentic_security/probe_actor/refusal.py` & `agentic_security-0.1.4/agentic_security/probe_actor/refusal.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.3/agentic_security/probe_data/__init__.py` & `agentic_security-0.1.4/agentic_security/probe_data/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,56 +84,70 @@
     {
         "dataset_name": "Agentic Security",
         "num_prompts": 0,
         "tokens": 0,
         "approx_cost": 0.0,
         "source": "Local dataset",
         "selected": True,
-        "dynamic": False,
+        "dynamic": True,
         "url": "",
     },
     {
         "dataset_name": "Malwaregen",
         "num_prompts": 0,
         "tokens": 0,
         "approx_cost": 0.0,
         "source": "Local dataset",
         "selected": False,
+        "dynamic": True,
         "url": "",
     },
     {
         "dataset_name": "Hallucination",
         "num_prompts": 0,
         "tokens": 0,
         "approx_cost": 0.0,
         "source": "Local dataset",
         "selected": False,
+        "dynamic": True,
         "url": "",
     },
     {
         "dataset_name": "DataLeak",
         "num_prompts": 0,
         "tokens": 0,
         "approx_cost": 0.0,
         "source": "Local dataset",
         "selected": False,
+        "dynamic": True,
         "url": "",
     },
     {
         "dataset_name": "llm-adaptive-attacks",
         "num_prompts": 0,
         "tokens": 0,
         "approx_cost": 0.0,
-        "source": "Github: tml-epfl/llm-adaptive-attacks",
+        "source": "Github: tml-epfl/llm-adaptive-attacks#0.0.1",
         "selected": False,
+        "dynamic": True,
         "url": "https://github.com/tml-epfl/llm-adaptive-attacks",
     },
     {
+        "dataset_name": "Garak",
+        "num_prompts": 0,
+        "tokens": 0,
+        "approx_cost": 0.0,
+        "source": "Github: https://github.com/leondz/garak#v0.9.0.1",
+        "selected": False,
+        "url": "https://github.com/leondz/garak2",
+        "dynamic": True,
+    },
+    {
         "dataset_name": "Custom CSV",
         "num_prompts": len(load_local_csv().prompts),
         "tokens": load_local_csv().tokens,
         "approx_cost": 0.0,
-        "source": "Local file dataset",
+        "source": f"Local file dataset: {load_local_csv().metadata['src']}",
         "selected": len(load_local_csv().prompts),
         "url": "",
     },
 ]
```

### Comparing `agentic_security-0.1.3/agentic_security/probe_data/data.py` & `agentic_security-0.1.4/agentic_security/probe_data/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 from functools import lru_cache
 
 import pandas as pd
 from loguru import logger
 
 from agentic_security.probe_data import stenography_fn
-from agentic_security.probe_data.modules import adaptive_attacks
+from agentic_security.probe_data.modules import adaptive_attacks, garak_tool
 
 IS_VERCEL = os.getenv("IS_VERCEL", "f") == "t"
 
 if not IS_VERCEL:
     from cache_to_disk import cache_to_disk
 else:
     # Read only fs in vercel, just mock no-op decorator
@@ -28,14 +28,15 @@
 @dataclass
 class ProbeDataset:
     dataset_name: str
     metadata: dict
     prompts: list[str]
     tokens: int
     approx_cost: float
+    lazy: bool = False
 
     def metadata_summary(self):
         return {
             "dataset_name": self.dataset_name,
             "num_prompts": len(self.prompts),
             "tokens": self.tokens,
             "approx_cost": self.approx_cost,
@@ -164,18 +165,15 @@
         metadata={},
         prompts=ds,
         tokens=count_words_in_list(ds),
         approx_cost=0.0,
     )
 
 
-def prepare_prompts(
-    dataset_names,
-    budget,
-):
+def prepare_prompts(dataset_names, budget, tools_inbox=None):
     # ## Datasets used and cleaned:
     # markush1/LLM-Jailbreak-Classifier
     # 1. Open-Orca/OpenOrca
     # 2. ShawnMenz/DAN_jailbreak
     # 3. EddyLuo/JailBreakV_28K
     # 4. https://raw.githubusercontent.com/verazuo/jailbreak_llms/main/data/jailbreak_prompts.csv
 
@@ -199,44 +197,33 @@
                 logger.error(f"Error loading {dataset_name}: {e}")
 
     dynamic_datasets = {
         "Steganography": lambda: Stenography(group),
         "llm-adaptive-attacks": lambda: dataset_from_iterator(
             "llm-adaptive-attacks", adaptive_attacks.Module(group).apply()
         ),
+        "Garak": lambda: dataset_from_iterator(
+            "Garak",
+            garak_tool.Module(group, tools_inbox=tools_inbox).apply(),
+            lazy=True,
+        ),
         "GPT fuzzer": lambda: [],
     }
 
     dynamic_groups = []
     for dataset_name in dataset_names:
         if dataset_name in dynamic_datasets:
             logger.info(f"Loading {dataset_name}")
             ds = dynamic_datasets[dataset_name]()
 
             for g in ds:
                 dynamic_groups.append(g)
     return group + dynamic_groups
 
 
-class MutationFn:
-    def __init__(self, mutation_fn):
-        self.mutation_fn = mutation_fn
-        self.mutation_fn_name = mutation_fn.__name__
-        self.input = ""
-        self.output = ""
-
-    def __call__(self, prompt):
-        self.input = prompt
-        self.output = self.mutation_fn(prompt)
-        return self.output
-
-    def __str__(self):
-        return f"{self.mutation_fn_name}({self.input}) => {self.output}"
-
-
 class Stenography:
     fn_library = {
         "rot5": stenography_fn.rot5,
         "rot13": stenography_fn.rot13,
         "base64": stenography_fn.base64_encode,
         "mirror": stenography_fn.mirror_words,
         "random_case": stenography_fn.randomize_letter_case,
@@ -277,38 +264,48 @@
 def load_local_csv() -> ProbeDataset:
     csv_files = [f for f in os.listdir(".") if f.endswith(".csv")]
     logger.info(f"Found {len(csv_files)} CSV files")
     logger.info(f"CSV files: {csv_files}")
     prompt_list = []
 
     for file in csv_files:
-        df = pd.read_csv(file)
+        try:
+            df = pd.read_csv(file)
+        except Exception as e:
+            logger.error(f"Error reading {file}: {e}")
+            continue
         # Check if 'prompt' column exists
         if "prompt" in df.columns:
             prompt_list.extend(df["prompt"].tolist())
-
+        else:
+            logger.warning(f"File {file} does not contain a 'prompt' column")
     return ProbeDataset(
         dataset_name="Local CSV",
-        metadata={},
+        metadata={"src": str(csv_files)},
         prompts=prompt_list,
         tokens=count_words_in_list(prompt_list),
         approx_cost=0.0,
     )
 
 
-def dataset_from_iterator(name: str, iterator) -> list:
+def dataset_from_iterator(name: str, iterator, lazy=False) -> list:
     """Convert an iterator into a list of prompts and create a ProbeDataset
     object.
 
     Args:
         name (str): The name of the dataset.
         iterator (iterator): An iterator that generates prompts.
 
     Returns:
         list: A list containing a single ProbeDataset object.
     """
-    prompts = list(iterator)
-    tokens = count_words_in_list(prompts)
+    prompts = list(iterator) if not lazy else iterator
+    tokens = count_words_in_list(prompts) if not lazy else 0
     dataset = ProbeDataset(
-        dataset_name=name, metadata={}, prompts=prompts, tokens=tokens, approx_cost=0.0
+        dataset_name=name,
+        metadata={},
+        prompts=prompts,
+        tokens=tokens,
+        approx_cost=0.0,
+        lazy=lazy,
     )
     return [dataset]
```

### Comparing `agentic_security-0.1.3/agentic_security/probe_data/modules/adaptive_attacks.py` & `agentic_security-0.1.4/agentic_security/probe_data/modules/adaptive_attacks.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.3/agentic_security/probe_data/modules/test_adaptive_attacks.py` & `agentic_security-0.1.4/agentic_security/probe_data/modules/test_adaptive_attacks.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.3/agentic_security/probe_data/stenography_fn.py` & `agentic_security-0.1.4/agentic_security/probe_data/stenography_fn.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.3/agentic_security/probe_data/test_data.py` & `agentic_security-0.1.4/agentic_security/probe_data/test_data.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.3/agentic_security/report_chart.py` & `agentic_security-0.1.4/agentic_security/report_chart.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.3/agentic_security/static/index.html` & `agentic_security-0.1.4/agentic_security/static/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             <p class="text-sm text-muted-foreground text-center ">Input the API
               LLM spec
               and specify the maximum budget in tokens.</p>
           </div>
           <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
             <div class="flex flex-col space-y-4">
               <div class="text-lg font-semibold">Select a config</div>
-              <div class="grid grid-cols-1 md:grid-cols-4 gap-4">
+              <div class="grid grid-cols-1 md:grid-cols-5 gap-4">
                 <div v-for="(config, index) in configs" :key="index"
                   @click="selectConfig(index)"
                   class="border-2 rounded-lg p-4 flex flex-col items-start transition-all hover:shadow-md"
                   :class="{'border-earth-1': selectedConfig === index, 'border-gray-300': selectedConfig !== index}">
                   <div class="flex items-center justify-between w-full">
                     <div class="font-medium"
                       :class="{'text-earth-1': selectedConfig === index, 'text-gray-800': selectedConfig !== index}">
@@ -401,14 +401,26 @@
 
 {
     "model_id": "codellama-34b",
     "system_prompt": "You are helpful and concise coding assistant",
     "user_prompt": "<<PROMPT>>"
 }
 `,
+        `POST https://api.together.xyz/v1/chat/completions
+Authorization: Bearer $TOGETHER_API_KEY
+Content-Type: application/json
+
+{
+    "model": "mistralai/Mixtral-8x7B-Instruct-v0.1",
+    "messages": [
+        {"role": "system", "content": "You are an expert travel guide"},
+        {"role": "user", "content": "<<PROMPT>>"}
+    ]
+}
+`,
       ]
       var app = new Vue({
         el: '#vue-app',
         data: {
           progressWidth: '0%',
           modelSpec: LLM_SPECS[0],
           budget: 50,
@@ -423,14 +435,15 @@
           reportImageUrl: '',
           selectedConfig: 0,
           configs: [
             { name: 'Custom API', prompts: 40000, customInstructions: 'Requires api spec' },
             { name: 'Open AI', prompts: 24000 },
             { name: 'Replicate', prompts: 40000 },
             { name: 'Groq', prompts: 40000 },
+            { name: 'Together.ai', prompts: 40000 },
           ],
           dataConfig: [],
         },
         mounted: function() {
           console.log('Vue app mounted');
           this.adjustHeight({ target: document.getElementById('llm-spec') });
           // this.startScan();
```

### Comparing `agentic_security-0.1.3/agentic_security/test_lib.py` & `agentic_security-0.1.4/agentic_security/test_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from agentic_security.lib import REGISTRY, AgenticSecurity
 from inline_snapshot import snapshot
 
+from agentic_security.lib import REGISTRY, AgenticSecurity
+
 SAMPLE_SPEC = """
 POST http://0.0.0.0:8718/v1/self-probe
 Authorization: Bearer XXXXX
 Content-Type: application/json
 
 {
     "prompt": "<<PROMPT>>"
```

### Comparing `agentic_security-0.1.3/agentic_security/test_spec.py` & `agentic_security-0.1.4/agentic_security/test_spec.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.3/pyproject.toml` & `agentic_security-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentic_security"
-version = "0.1.3"
+version = "0.1.4"
 description = "Agentic LLM vulnerability scanner"
 authors = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 maintainers = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 repository = "https://github.com/msoedov/agentic_security"
 license = "MIT"
 readme = "Readme.md"
 keywords = [
@@ -22,23 +22,23 @@
 
 
 [tool.poetry.scripts]
 agentic_security = "agentic_security.__main__:entrypoint"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-fastapi = ">=0.109.1,<0.111.0"
+fastapi = ">=0.109.1,<0.112.0"
 uvicorn = ">=0.23.2,<0.30.0"
 fire = "^0.5.0"
 loguru = "^0.7.2"
 httpx = ">=0.25.1,<0.28.0"
 cache-to-disk = "^2.0.0"
 pandas = ">=1.4,<3.0"
 datasets = "^1.14.0"
-tabulate = "^0.8.9"
+tabulate = ">=0.8.9,<0.10.0"
 colorama = "^0.4.4"
 matplotlib = "^3.4.3"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.10.1,<25.0.0"
 mypy = "^1.6.1"
 httpx = ">=0.25.1,<0.28.0"
```

### Comparing `agentic_security-0.1.3/PKG-INFO` & `agentic_security-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentic_security
-Version: 0.1.3
+Version: 0.1.4
 Summary: Agentic LLM vulnerability scanner
 Home-page: https://github.com/msoedov/agentic_security
 License: MIT
 Keywords: LLM vulnerability scanner,llm security,llm adversarial attacks,prompt injection,prompt leakage,prompt injection attacks,prompt leakage prevention,llm vulnerabilities,owasp-llm-top-10
 Author: Alexander Miasoiedov
 Author-email: msoedov@gmail.com
 Maintainer: Alexander Miasoiedov
@@ -15,33 +15,31 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cache-to-disk (>=2.0.0,<3.0.0)
 Requires-Dist: colorama (>=0.4.4,<0.5.0)
 Requires-Dist: datasets (>=1.14.0,<2.0.0)
-Requires-Dist: fastapi (>=0.109.1,<0.111.0)
+Requires-Dist: fastapi (>=0.109.1,<0.112.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: httpx (>=0.25.1,<0.28.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
 Requires-Dist: pandas (>=1.4,<3.0)
-Requires-Dist: tabulate (>=0.8.9,<0.9.0)
+Requires-Dist: tabulate (>=0.8.9,<0.10.0)
 Requires-Dist: uvicorn (>=0.23.2,<0.30.0)
 Project-URL: Repository, https://github.com/msoedov/agentic_security
 Description-Content-Type: text/markdown
 
 <p align="center">
 
 <h1 align="center">Agentic Security</h1>
 
 <p align="center">
-    The open-source Agentic LLM Vulnerability Scanner .
-    <br />
-    <a href="#features"><strong>Learn more »</strong></a>
+    The open-source Agentic LLM Vulnerability Scanner
     <br />
     <br />
 
 <p>
 <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/msoedov/agentic_security" />
 <img alt="GitHub Last Commit" src="https://img.shields.io/github/last-commit/msoedov/agentic_security" />
 <img alt="" src="https://img.shields.io/github/repo-size/msoedov/agentic_security" />
@@ -52,15 +50,15 @@
 </p>
   </p>
 </p>
 
 ## Features
 
 - Customizable Rule Sets or Agent based attacks🛠️
-- Comprehansive fuzzing for any LLMs 🧪
+- Comprehensive fuzzing for any LLMs 🧪
 - LLM API integration and stress testing 🛠️
 - Wide range of fuzzing and attack techniques 🌀
 
 Note: Please be aware that Agentic Security is designed as a safety scanner tool and not a foolproof solution. It cannot guarantee complete protection against all possible threats.
 
 ## About the Project 🧙
 
@@ -145,15 +143,15 @@
 Authorization: Bearer XXXXX
 Content-Type: application/json
 
 {
     "prompt": "<<PROMPT>>"
 }
 """
-result = AgenticSecurity.scan(spec)
+result = AgenticSecurity.scan(llmSpec=spec)
 
 # module: failure rate
 # {"Local CSV": 79.65116279069767, "llm-adaptive-attacks": 20.0}
 exit(max(r.values()) > 20)
 ```
 
 ```
```

