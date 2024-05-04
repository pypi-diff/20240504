# Comparing `tmp/pybotters-1.1.0.tar.gz` & `tmp/pybotters-1.1.1.tar.gz`

## Comparing `pybotters-1.1.0.tar` & `pybotters-1.1.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pybotters-1.1.0/.readthedocs.yml
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 pybotters-1.1.0/README.md
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pybotters-1.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pybotters-1.1.0/.github/release.yml
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 pybotters-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pybotters-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pybotters-1.1.0/.vscode/extensions.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pybotters-1.1.0/.vscode/hatch_config.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pybotters-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/Makefile
--rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/advanced.rst
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/conf.py
--rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/contributing.rst
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/examples.rst
--rw-r--r--   0        0        0    16099 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/exchanges.rst
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/favicon.ico
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/index.rst
--rw-r--r--   0        0        0    52834 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/logo.png
--rw-r--r--   0        0        0    16737 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/logo_150.png
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/make.bat
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/reference.rst
--rw-r--r--   0        0        0    31649 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/user-guide.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pybotters-1.1.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/binance.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/bitbank.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/bitflyer.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/bitget.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/bybit.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/coincheck.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/gmocoin.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/kucoin.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/okx.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/phemex.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/datastore/requirements.txt
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pybotters-1.1.0/example/trading-bot/bitflyer.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/__version__.py
--rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/auth.py
--rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/client.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/request.py
--rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/store.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/typedefs.py
--rw-r--r--   0        0        0    25768 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/ws.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/__init__.py
--rw-r--r--   0        0        0    31433 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/binance.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/bitbank.py
--rw-r--r--   0        0        0    16374 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/bitflyer.py
--rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/bitget.py
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/bitmex.py
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/bybit.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/coincheck.py
--rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/gmocoin.py
--rw-r--r--   0        0        0    25200 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/kucoin.py
--rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/okx.py
--rw-r--r--   0        0        0    11654 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/phemex.py
--rw-r--r--   0        0        0    20486 2020-02-02 00:00:00.000000 pybotters-1.1.0/pybotters/models/legacy/gmocoin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0    43212 2020-02-02 00:00:00.000000 pybotters-1.1.0/tests/test_auth.py
--rw-r--r--   0        0        0     9230 2020-02-02 00:00:00.000000 pybotters-1.1.0/tests/test_client.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pybotters-1.1.0/tests/test_request.py
--rw-r--r--   0        0        0    16502 2020-02-02 00:00:00.000000 pybotters-1.1.0/tests/test_store.py
--rw-r--r--   0        0        0    45820 2020-02-02 00:00:00.000000 pybotters-1.1.0/tests/test_ws.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pybotters-1.1.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pybotters-1.1.0/LICENCE
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pybotters-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    11047 2020-02-02 00:00:00.000000 pybotters-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pybotters-1.1.1/.readthedocs.yml
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 pybotters-1.1.1/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pybotters-1.1.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pybotters-1.1.1/.github/release.yml
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 pybotters-1.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pybotters-1.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pybotters-1.1.1/.vscode/extensions.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pybotters-1.1.1/.vscode/hatch_config.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pybotters-1.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/advanced.rst
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/conf.py
+-rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/contributing.rst
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/examples.rst
+-rw-r--r--   0        0        0    16099 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/exchanges.rst
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/favicon.ico
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/index.rst
+-rw-r--r--   0        0        0    52834 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/logo.png
+-rw-r--r--   0        0        0    16737 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/logo_150.png
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/make.bat
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/reference.rst
+-rw-r--r--   0        0        0    31649 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/user-guide.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/binance.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/bitbank.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/bitflyer.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/bitget.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/bybit.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/coincheck.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/gmocoin.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/kucoin.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/okx.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/phemex.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/requirements.txt
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/trading-bot/bitflyer.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/__version__.py
+-rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/auth.py
+-rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/client.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/request.py
+-rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/store.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/typedefs.py
+-rw-r--r--   0        0        0    25835 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/ws.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/__init__.py
+-rw-r--r--   0        0        0    31433 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/binance.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/bitbank.py
+-rw-r--r--   0        0        0    16374 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/bitflyer.py
+-rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/bitget.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/bitmex.py
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/bybit.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/coincheck.py
+-rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/gmocoin.py
+-rw-r--r--   0        0        0    25200 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/kucoin.py
+-rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/okx.py
+-rw-r--r--   0        0        0    11654 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/phemex.py
+-rw-r--r--   0        0        0    20486 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/legacy/gmocoin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    43212 2020-02-02 00:00:00.000000 pybotters-1.1.1/tests/test_auth.py
+-rw-r--r--   0        0        0     9230 2020-02-02 00:00:00.000000 pybotters-1.1.1/tests/test_client.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pybotters-1.1.1/tests/test_request.py
+-rw-r--r--   0        0        0    16502 2020-02-02 00:00:00.000000 pybotters-1.1.1/tests/test_store.py
+-rw-r--r--   0        0        0    45941 2020-02-02 00:00:00.000000 pybotters-1.1.1/tests/test_ws.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pybotters-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pybotters-1.1.1/LICENCE
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pybotters-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11047 2020-02-02 00:00:00.000000 pybotters-1.1.1/PKG-INFO
```

### Comparing `pybotters-1.1.0/README.md` & `pybotters-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/.github/FUNDING.yml` & `pybotters-1.1.1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/.github/release.yml` & `pybotters-1.1.1/.github/release.yml`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/.github/workflows/ci.yml` & `pybotters-1.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/.github/workflows/publish.yml` & `pybotters-1.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/.vscode/settings.json` & `pybotters-1.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/Makefile` & `pybotters-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/advanced.rst` & `pybotters-1.1.1/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/conf.py` & `pybotters-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/contributing.rst` & `pybotters-1.1.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/examples.rst` & `pybotters-1.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/exchanges.rst` & `pybotters-1.1.1/docs/exchanges.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/favicon.ico` & `pybotters-1.1.1/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/index.rst` & `pybotters-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/logo.png` & `pybotters-1.1.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/logo_150.png` & `pybotters-1.1.1/docs/logo_150.png`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/make.bat` & `pybotters-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/reference.rst` & `pybotters-1.1.1/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/user-guide.rst` & `pybotters-1.1.1/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/_templates/autosummary/class.rst` & `pybotters-1.1.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/docs/_templates/autosummary/module.rst` & `pybotters-1.1.1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/example/datastore/binance.py` & `pybotters-1.1.1/example/datastore/binance.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/example/datastore/bitbank.py` & `pybotters-1.1.1/example/datastore/bitbank.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/example/datastore/bitflyer.py` & `pybotters-1.1.1/example/datastore/bitflyer.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/example/datastore/bitget.py` & `pybotters-1.1.1/example/datastore/bitget.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/example/datastore/bybit.py` & `pybotters-1.1.1/example/datastore/bybit.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/example/datastore/coincheck.py` & `pybotters-1.1.1/example/datastore/coincheck.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/example/datastore/gmocoin.py` & `pybotters-1.1.1/example/datastore/gmocoin.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/example/datastore/kucoin.py` & `pybotters-1.1.1/example/datastore/kucoin.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/example/datastore/okx.py` & `pybotters-1.1.1/example/datastore/okx.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/example/datastore/phemex.py` & `pybotters-1.1.1/example/datastore/phemex.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/example/trading-bot/bitflyer.py` & `pybotters-1.1.1/example/trading-bot/bitflyer.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/__init__.py` & `pybotters-1.1.1/pybotters/__init__.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/auth.py` & `pybotters-1.1.1/pybotters/auth.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/client.py` & `pybotters-1.1.1/pybotters/client.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/request.py` & `pybotters-1.1.1/pybotters/request.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/store.py` & `pybotters-1.1.1/pybotters/store.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/ws.py` & `pybotters-1.1.1/pybotters/ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         if msg.type == aiohttp.WSMsgType.TEXT:
             for hdlr in hdlr_str:
                 self._loop.call_soon(hdlr, msg.data, ws)
         elif msg.type == aiohttp.WSMsgType.BINARY:
             for hdlr in hdlr_bytes:
                 self._loop.call_soon(hdlr, msg.data, ws)
 
-        if hdlr_json:
+        if hdlr_json and msg.type in {aiohttp.WSMsgType.TEXT, aiohttp.WSMsgType.BINARY}:
             try:
                 data = msg.json()
             except json.JSONDecodeError as e:
                 if msg.data not in {"ping", "pong"}:
                     logger.warning(f"{pretty_modulename(e)}: {e} {e.doc}")
             else:
                 for hdlr in hdlr_json:
```

### Comparing `pybotters-1.1.0/pybotters/models/binance.py` & `pybotters-1.1.1/pybotters/models/binance.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/models/bitbank.py` & `pybotters-1.1.1/pybotters/models/bitbank.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/models/bitflyer.py` & `pybotters-1.1.1/pybotters/models/bitflyer.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/models/bitget.py` & `pybotters-1.1.1/pybotters/models/bitget.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/models/bitmex.py` & `pybotters-1.1.1/pybotters/models/bitmex.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/models/bybit.py` & `pybotters-1.1.1/pybotters/models/bybit.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/models/coincheck.py` & `pybotters-1.1.1/pybotters/models/coincheck.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/models/gmocoin.py` & `pybotters-1.1.1/pybotters/models/gmocoin.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/models/kucoin.py` & `pybotters-1.1.1/pybotters/models/kucoin.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/models/okx.py` & `pybotters-1.1.1/pybotters/models/okx.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/models/phemex.py` & `pybotters-1.1.1/pybotters/models/phemex.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pybotters/models/legacy/gmocoin.py` & `pybotters-1.1.1/pybotters/models/legacy/gmocoin.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/tests/test_auth.py` & `pybotters-1.1.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/tests/test_client.py` & `pybotters-1.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/tests/test_request.py` & `pybotters-1.1.1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/tests/test_store.py` & `pybotters-1.1.1/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/tests/test_ws.py` & `pybotters-1.1.1/tests/test_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,53 +394,57 @@
 
         async for msg in ws:
             if msg.type == aiohttp.WSMsgType.PING:
                 if call_count == 1:
                     pass
                 else:
                     await ws.pong(msg.data)
-                    await ws.send_str("pong")
+                    await ws.send_json({"data": "spam"})
             elif msg.type == aiohttp.WSMsgType.PONG:
                 continue
 
         await ws.close()
         return ws
 
     app = web.Application()
     app.add_routes([web.get("/ws", echo_json)])
 
     async with TestServer(app) as server:
         yield server
 
 
 @pytest.mark.asyncio
-async def test_websocketapp_ensure_open(test_ping_pong_server: TestServer):
+async def test_websocketapp_ensure_open_hdlr(
+    test_ping_pong_server: TestServer, caplog: pytest.LogCaptureFixture
+):
     wsq = pybotters.WebSocketQueue()
 
     async def message_ping_pong():
         async with pybotters.Client() as client:
             ws = await client.ws_connect(
                 f"ws://localhost:{test_ping_pong_server.port}/ws",
-                hdlr_str=wsq.onmessage,
+                hdlr_json=wsq.onmessage,
                 heartbeat=None,
                 autoping=True,
             )
             await ws.heartbeat(0.1)
             await ws.wait()
 
     wstask = asyncio.create_task(message_ping_pong())
     received_messages = [
         (await asyncio.wait_for(wsq.get(), timeout=5.0)),
     ]
     wstask.cancel()
     await asyncio.wait([wstask], timeout=5.0)
 
-    assert received_messages == ["pong"]
+    assert received_messages == [{"data": "spam"}]
     assert wstask.cancelled()
 
+    assert caplog.records == []  # No handler errors
+
 
 def test_heartbeathosts():
     assert hasattr(pybotters.ws.HeartbeatHosts, "items")
     assert isinstance(pybotters.ws.HeartbeatHosts.items, dict)
     for host, func in pybotters.ws.HeartbeatHosts.items.items():
         assert isinstance(host, str)
         assert callable(func)
```

### Comparing `pybotters-1.1.0/.gitignore` & `pybotters-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/LICENCE` & `pybotters-1.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/pyproject.toml` & `pybotters-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.0/PKG-INFO` & `pybotters-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pybotters
-Version: 1.1.0
+Version: 1.1.1
 Summary: An advanced API client for python crypto bot traders
 Project-URL: Documentation, https://pybotters.readthedocs.io/ja/stable/
 Project-URL: Repository, https://github.com/pybotters/pybotters
 Author-email: MtkN1 <51289448+MtkN1@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: aiohttp,crypto,exchange,trading
```

