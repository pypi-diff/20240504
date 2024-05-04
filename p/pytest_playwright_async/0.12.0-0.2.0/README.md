# Comparing `tmp/pytest_playwright_async-0.12.0.tar.gz` & `tmp/pytest-playwright-async-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_playwright_async-0.12.0.tar", last modified: Sat May  4 17:01:31 2024, max compression
+gzip compressed data, was "pytest-playwright-async-0.2.0.tar", last modified: Mon Jul  3 12:21:20 2023, max compression
```

## Comparing `pytest_playwright_async-0.12.0.tar` & `pytest-playwright-async-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:31.216702 pytest_playwright_async-0.12.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-04 17:01:31.216702 pytest_playwright_async-0.12.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-04 17:01:18.000000 pytest_playwright_async-0.12.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-04 17:01:18.000000 pytest_playwright_async-0.12.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 17:01:31.216702 pytest_playwright_async-0.12.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:31.216702 pytest_playwright_async-0.12.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:31.216702 pytest_playwright_async-0.12.0/src/pytest_playwright_async/
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-05-04 17:01:18.000000 pytest_playwright_async-0.12.0/src/pytest_playwright_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 17:01:18.000000 pytest_playwright_async-0.12.0/src/pytest_playwright_async/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:31.216702 pytest_playwright_async-0.12.0/src/pytest_playwright_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-04 17:01:31.000000 pytest_playwright_async-0.12.0/src/pytest_playwright_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-04 17:01:31.000000 pytest_playwright_async-0.12.0/src/pytest_playwright_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:01:31.000000 pytest_playwright_async-0.12.0/src/pytest_playwright_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-04 17:01:31.000000 pytest_playwright_async-0.12.0/src/pytest_playwright_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-04 17:01:31.000000 pytest_playwright_async-0.12.0/src/pytest_playwright_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 17:01:31.000000 pytest_playwright_async-0.12.0/src/pytest_playwright_async.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:31.216702 pytest_playwright_async-0.12.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-04 17:01:18.000000 pytest_playwright_async-0.12.0/tests/test_playwright.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:21:20.764295 pytest-playwright-async-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-03 12:21:20.764295 pytest-playwright-async-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1288 2023-07-03 12:21:10.000000 pytest-playwright-async-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-07-03 12:21:10.000000 pytest-playwright-async-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 12:21:20.764295 pytest-playwright-async-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:21:20.760295 pytest-playwright-async-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:21:20.760295 pytest-playwright-async-0.2.0/src/pytest_playwright_async/
+-rw-r--r--   0 root         (0) root         (0)     5958 2023-07-03 12:21:10.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:21:20.764295 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-03 12:21:20.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      397 2023-07-03 12:21:20.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:21:20.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-03 12:21:20.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-03 12:21:20.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-03 12:21:20.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:21:20.764295 pytest-playwright-async-0.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     4759 2023-07-03 12:21:10.000000 pytest-playwright-async-0.2.0/tests/test_playwright.py
```

### Comparing `pytest_playwright_async-0.12.0/PKG-INFO` & `pytest-playwright-async-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1
-Name: pytest_playwright_async
-Version: 0.12.0
-Summary: ASYNC Pytest plugin for Playwright
-License: MIT
-Project-URL: Homepage, https://github.com/m9810223/playwright-async-pytest
-Project-URL: Source, https://github.com/m9810223/playwright-async-pytest
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: pytest-playwright<=0.4.4,>=0.3.3
-Requires-Dist: pytest-asyncio==0.20.3
-
-# Playwright Async Pytest -- ASYNC Pytest plugin for Playwright
-
-[![pypi](https://img.shields.io/pypi/v/pytest_playwright_async.svg)](https://pypi.python.org/pypi/pytest_playwright_async)
+# ASYNC Pytest plugin for Playwright [![PyPI](https://img.shields.io/pypi/v/pytest-playwright-async)](https://pypi.org/project/pytest-playwright-async/)
 
 There an official playwright plugin for pytest: [PyPI](https://pypi.org/project/pytest-playwright/) / [playwright-pytest](https://github.com/microsoft/playwright-pytest) / [intro](https://playwright.dev/python/docs/intro).
 But if you need an async version, here is it!
 
 ## Installation
 
 ```shell
```

### Comparing `pytest_playwright_async-0.12.0/pyproject.toml` & `pytest-playwright-async-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,58 @@
 [project]
-name = "pytest_playwright_async"
-version = "0.12.0"
-requires-python = ">=3.8"
+authors = [
+  {name = "m9810223", email = "m9810223@gmail.com"},
+]
 dependencies = [
-    "pytest-playwright>=0.3.3,<=0.4.4", # https://pypi.org/project/pytest-playwright/
-    "pytest-asyncio==0.20.3",           # https://github.com/microsoft/playwright-python/blob/main/local-requirements.txt
+  "pytest-playwright==0.3.3", # https://pypi.org/project/pytest-playwright/
+  "pytest-asyncio==0.20.3", # https://github.com/microsoft/playwright-python/blob/main/local-requirements.txt
 ]
 description = "ASYNC Pytest plugin for Playwright"
-license = { text = "MIT" }
+license = {text = "MIT"}
+name = "pytest-playwright-async"
 readme = "README.md"
-
-[project.entry-points.pytest11]
-playwright_async = "pytest_playwright_async"
+requires-python = ">=3.8"
+version = "0.2.0"
 
 [project.urls]
 Homepage = "https://github.com/m9810223/playwright-async-pytest"
 Source = "https://github.com/m9810223/playwright-async-pytest"
 
-[tool.pdm]
-distribution = true
+[tool.semantic_release]
+# https://python-semantic-release.readthedocs.io/en/latest/configuration.html
+build_command = "pip install pdm && pdm build"
+version_toml = "pyproject.toml:project.version"
+
+[project.entry-points.pytest11]
+playwright_async = "pytest_playwright_async"
 
 [tool.pdm.dev-dependencies]
-dev = ["pytest>=7.4.0", "ipython>=8.12.2", "nest-asyncio>=1.5.6"]
+dev = [
+  "pytest>=7.4.0",
+  "ipython>=8.12.2",
+  "nest-asyncio>=1.5.6",
+]
 
 [tool.pdm.scripts]
 test = "pytest"
 
-[tool.semantic_release]
-# https://python-semantic-release.readthedocs.io/en/latest/configuration.html
-version_toml = ["pyproject.toml:project.version"]
-version_variables = ["src/pytest_playwright_async/__version__.py:VERSION"]
-
-[tool.black]
-# https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html
-line-length = 100
-skip-string-normalization = true
+[tool.pytest.ini_options]
+addopts = "--exitfirst --failed-first -r fEsxXp --disable-warnings --showlocals --tb=short"
 
 [tool.ruff]
-line-length = 100
-fix = true
-show-fixes = true
-output-format = "full"
-
-[tool.ruff.lint]
 extend-select = [
-    "W", # pycodestyle Warning
-    "I", # isort
-    "N", # pep8-naming
-    "S", # flake8-bandit
-    # "PTH", # flake8-use-pathlib
-    "PGH", # pygrep-hooks
-    "TRY", # tryceratops
+  "W", # pycodestyle Warning
+  "I", # isort
+  "N", # pep8-naming
+  "S", # flake8-bandit
+  "PGH", # pygrep-hooks
+  "TRY", # tryceratops
 ]
 ignore = [
-    "S101", # Use of `assert` detected
+  "E501", # line-too-long
+  "S101", # Use of `assert` detected
 ]
 
-[tool.ruff.lint.isort]
+[tool.ruff.isort]
 # https://beta.ruff.rs/docs/settings/#isort
-lines-after-imports = 2
 force-single-line = true
-force-sort-within-sections = true
-known-local-folder = []
-
-[tool.mypy]
-ignore_missing_imports = true
-
-[tool.pytest.ini_options]
-addopts = "--exitfirst --failed-first -r fEsxXp --disable-warnings --showlocals --tb=short"
+lines-after-imports = 2
```

### Comparing `pytest_playwright_async-0.12.0/src/pytest_playwright_async/__init__.py` & `pytest-playwright-async-0.2.0/src/pytest_playwright_async/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 import sys
 import typing as t
 
+import pytest
+import pytest_asyncio
 from playwright.async_api import Browser
 from playwright.async_api import BrowserContext
 from playwright.async_api import BrowserType
 from playwright.async_api import Error
 from playwright.async_api import Page
 from playwright.async_api import Playwright
 from playwright.async_api import async_playwright
-import pytest
-import pytest_asyncio
 from pytest_playwright.pytest_playwright import VSCODE_PYTHON_EXTENSION_ID
 from pytest_playwright.pytest_playwright import _build_artifact_test_folder
 from pytest_playwright.pytest_playwright import _is_debugger_attached
 from pytest_playwright.pytest_playwright import artifacts_folder
 from pytest_playwright.pytest_playwright import slugify
 
 
@@ -116,15 +116,17 @@
     yield context
 
     # If request.node is missing rep_call, then some error happened during execution
     # that prevented teardown, but should still be counted as a failure
     failed = request.node.rep_call.failed if hasattr(request.node, 'rep_call') else True
 
     if capture_trace:
-        retain_trace = tracing_option == 'on' or (failed and tracing_option == 'retain-on-failure')
+        retain_trace = tracing_option == 'on' or (
+            failed and tracing_option == 'retain-on-failure'
+        )
         if retain_trace:
             trace_path = _build_artifact_test_folder(pytestconfig, request, 'trace.zip')
             await context.tracing.stop(path=trace_path)
         else:
             await context.tracing.stop()
 
     screenshot_option = pytestconfig.getoption('--screenshot')
@@ -141,22 +143,24 @@
                 await page.screenshot(timeout=5000, path=screenshot_path)
             except Error:
                 pass
 
     await context.close()
 
     video_option = pytestconfig.getoption('--video')
-    preserve_video = video_option == 'on' or (failed and video_option == 'retain-on-failure')
+    preserve_video = video_option == 'on' or (
+        failed and video_option == 'retain-on-failure'
+    )
     if preserve_video:
         for page in pages:
             video = page.video
             if not video:
                 continue
             try:
-                video_path = await video.path()
+                video_path = video.path()
                 file_name = os.path.basename(video_path)
                 await video.save_as(
                     path=_build_artifact_test_folder(pytestconfig, request, file_name)
                 )
             except Error:
                 # Silent catch empty videos.
                 pass
```

### Comparing `pytest_playwright_async-0.12.0/tests/test_playwright.py` & `pytest-playwright-async-0.2.0/tests/test_playwright.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,128 +1,136 @@
 import typing as t
 
+import pytest
 from playwright.async_api import Browser
 from playwright.async_api import BrowserContext
 from playwright.async_api import BrowserType
 from playwright.async_api import Page
 from playwright.async_api import Playwright
 from playwright.async_api import async_playwright
-import pytest
 
 
 URL = 'https://playwright.dev/'
 TITLE = 'Fast and reliable end-to-end testing for modern web apps | Playwright'
 
 
 @pytest.mark.asyncio
 async def test_async_playwright():
     async with async_playwright() as playwright:
         async with await playwright.chromium.launch() as browser:
             async with await browser.new_context() as context:
                 async with await context.new_page() as page:
-                    await page.goto(URL, wait_until='networkidle')
+                    await page.goto(URL)
                     assert await page.title() == TITLE
 
 
 @pytest.mark.asyncio
 async def test_my_app_is_working(  # https://playwright.dev/python/docs/test-runners#fixtures
     playwright_async: Playwright,
     browser_async: Browser,
     browser_name: str,
     browser_channel: t.Optional[str],
     context_async: BrowserContext,
     browser_context_args_async: dict,
     page_async: Page,
 ):
-    print(f"\n{playwright_async = }")
+    print(f'\n{playwright_async = }')
     assert type(playwright_async) == Playwright
 
-    print(f"\n{browser_async = }")
+    print(f'\n{browser_async = }')
     assert type(browser_async) == Browser
 
-    print(f"\n{browser_name = }")
+    print(f'\n{browser_name = }')
 
-    print(f"\n{browser_channel = }")
+    print(f'\n{browser_channel = }')
 
-    print(f"\n{context_async = }")
+    print(f'\n{context_async = }')
     assert type(context_async) == BrowserContext
 
-    print(f"\n{browser_context_args_async = }")
+    print(f'\n{browser_context_args_async = }')
 
-    print(f"\n{page_async = }")
+    print(f'\n{page_async = }')
     assert type(page_async) == Page
 
 
 @pytest.mark.asyncio
 async def test_browser_type_launch_args_async(browser_type_launch_args_async: t.Dict):
-    print(f"\n{browser_type_launch_args_async, type(browser_type_launch_args_async) = }")
+    print(
+        f'\n{browser_type_launch_args_async, type(browser_type_launch_args_async) = }'
+    )
     async with async_playwright() as playwright:
-        async with await playwright.chromium.launch(**browser_type_launch_args_async) as browser:
+        async with await playwright.chromium.launch(
+            **browser_type_launch_args_async
+        ) as browser:
             async with await browser.new_context() as context:
                 async with await context.new_page() as page:
-                    await page.goto(URL, wait_until='networkidle')
+                    await page.goto(URL)
                     assert await page.title() == TITLE
 
 
 @pytest.mark.asyncio
 async def test_browser_context_args_async(browser_context_args_async: t.Dict):
-    print(f"\n{browser_context_args_async, type(browser_context_args_async) = }")
+    print(f'\n{browser_context_args_async, type(browser_context_args_async) = }')
     async with async_playwright() as playwright:
         async with await playwright.chromium.launch() as browser:
-            async with await browser.new_context(**browser_context_args_async) as context:
+            async with await browser.new_context(
+                **browser_context_args_async
+            ) as context:
                 async with await context.new_page() as page:
-                    await page.goto(URL, wait_until='networkidle')
+                    await page.goto(URL)
                     assert await page.title() == TITLE
 
 
 @pytest.mark.asyncio
 async def test_playwright_async(playwright_async: Playwright):
-    print(f"\n{playwright_async, type(playwright_async) = }")
+    print(f'\n{playwright_async, type(playwright_async) = }')
     async with await playwright_async.chromium.launch() as browser:
         async with await browser.new_context() as context:
             async with await context.new_page() as page:
-                await page.goto(URL, wait_until='networkidle')
+                await page.goto(URL)
                 assert await page.title() == TITLE
 
 
 @pytest.mark.asyncio
 async def test_browser_type_async(browser_type_async: BrowserType):
-    print(f"\n{browser_type_async, type(browser_type_async) = }")
+    print(f'\n{browser_type_async, type(browser_type_async) = }')
     async with await browser_type_async.launch() as browser:
         async with await browser.new_context() as context:
             async with await context.new_page() as page:
-                await page.goto(URL, wait_until='networkidle')
+                await page.goto(URL)
                 assert await page.title() == TITLE
 
 
 @pytest.mark.asyncio
-async def test_launch_browser_async(launch_browser_async: t.Callable[..., t.Awaitable[Browser]]):
-    print(f"\n{launch_browser_async, type(launch_browser_async) = }")
+async def test_launch_browser_async(
+    launch_browser_async: t.Callable[..., t.Awaitable[Browser]]
+):
+    print(f'\n{launch_browser_async, type(launch_browser_async) = }')
     browser = await launch_browser_async()
     async with await browser.new_context() as context:
         async with await context.new_page() as page:
-            await page.goto(URL, wait_until='networkidle')
+            await page.goto(URL)
             assert await page.title() == TITLE
 
 
 @pytest.mark.asyncio
-async def test_browser_async(browser_async: Browser):
-    print(f"\n{browser_async, type(browser_async) = }")
+async def test_browser_async(browser_async):
+    print(f'\n{browser_async, type(browser_async) = }')
     async with await browser_async.new_context() as context:
         async with await context.new_page() as page:
-            await page.goto(URL, wait_until='networkidle')
+            await page.goto(URL)
             assert await page.title() == TITLE
 
 
 @pytest.mark.asyncio
-async def test_context_async(context_async: BrowserContext):
-    print(f"\n{context_async = }")
+async def test_context_async(context_async):
+    print(f'\n{context_async = }')
     async with await context_async.new_page() as page:
-        await page.goto(URL, wait_until='networkidle')
+        await page.goto(URL)
         assert await page.title() == TITLE
 
 
 @pytest.mark.asyncio
 async def test_page_async(page_async: Page):
-    print(f"\n{page_async = }")
-    await page_async.goto(URL, wait_until='networkidle')
+    print(f'\n{page_async = }')
+    await page_async.goto(URL)
     assert await page_async.title() == TITLE
```

