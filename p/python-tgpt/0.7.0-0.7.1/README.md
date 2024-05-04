# Comparing `tmp/python_tgpt-0.7.0.tar.gz` & `tmp/python_tgpt-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_tgpt-0.7.0.tar", last modified: Thu May  2 23:23:40 2024, max compression
+gzip compressed data, was "python_tgpt-0.7.1.tar", last modified: Sat May  4 10:22:59 2024, max compression
```

## Comparing `python_tgpt-0.7.0.tar` & `python_tgpt-0.7.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.090761 python_tgpt-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23449 2024-05-02 23:23:40.090761 python_tgpt-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-05-02 23:23:39.000000 python_tgpt-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 23:23:40.090761 python_tgpt-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.074760 python_tgpt-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17339 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/api/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/async_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/auto/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/auto/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    16877 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/auto/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/blackboxai/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/blackboxai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16048 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/blackboxai/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    85577 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gemini/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/gpt4all/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gpt4all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gpt4all/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gpt4free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gpt4free/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/gpt4free/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/groq/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/groq/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/imager/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/imager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/imager/imager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.078760 python_tgpt-0.7.0/src/pytgpt/koboldai/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/koboldai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/koboldai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/leo/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/leo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18641 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/leo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/llama2/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/llama2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/llama2/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19455 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/openai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/opengpt/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/opengpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/opengpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/perplexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/perplexity/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/phind/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/phind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/phind/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/poe/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/poe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/poe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    36065 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/webchatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/webchatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/webchatgpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.082760 python_tgpt-0.7.0/src/pytgpt/yepchat/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/yepchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/src/pytgpt/yepchat/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.086760 python_tgpt-0.7.0/src/python_tgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23449 2024-05-02 23:23:40.000000 python_tgpt-0.7.0/src/python_tgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-02 23:23:40.000000 python_tgpt-0.7.0/src/python_tgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:23:40.000000 python_tgpt-0.7.0/src/python_tgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 23:23:40.000000 python_tgpt-0.7.0/src/python_tgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-02 23:23:40.000000 python_tgpt-0.7.0/src/python_tgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 23:23:40.000000 python_tgpt-0.7.0/src/python_tgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:23:40.086760 python_tgpt-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_auto_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_blackboxai_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_gpt4free_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_imager.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_koboldai_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_leo_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_llama2_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_opengpt_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_phind_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_webchatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-02 23:23:07.000000 python_tgpt-0.7.0/tests/test_yepchat_tgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.882453 python_tgpt-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-05-04 10:22:59.882453 python_tgpt-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20671 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 10:22:59.882453 python_tgpt-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.866453 python_tgpt-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.866453 python_tgpt-0.7.1/src/pytgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.866453 python_tgpt-0.7.1/src/pytgpt/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17361 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/api/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/async_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.866453 python_tgpt-0.7.1/src/pytgpt/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/auto/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16877 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/auto/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.866453 python_tgpt-0.7.1/src/pytgpt/blackboxai/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/blackboxai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16048 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/blackboxai/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85577 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gemini/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/gpt4all/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gpt4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gpt4all/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gpt4free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gpt4free/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gpt4free/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/groq/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/imager/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/imager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/imager/imager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/koboldai/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/koboldai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/koboldai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/leo/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/leo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18641 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/leo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/llama2/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/llama2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/llama2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19455 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/openai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/opengpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/opengpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/opengpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.874453 python_tgpt-0.7.1/src/pytgpt/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/perplexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/perplexity/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.874453 python_tgpt-0.7.1/src/pytgpt/phind/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/phind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/phind/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.874453 python_tgpt-0.7.1/src/pytgpt/poe/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/poe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/poe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36065 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.874453 python_tgpt-0.7.1/src/pytgpt/webchatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/webchatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/webchatgpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.874453 python_tgpt-0.7.1/src/pytgpt/yepchat/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/yepchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/yepchat/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.878453 python_tgpt-0.7.1/src/python_tgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/src/python_tgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/src/python_tgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/src/python_tgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/src/python_tgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/src/python_tgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/src/python_tgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.878453 python_tgpt-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_auto_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_blackboxai_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_gpt4free_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_koboldai_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_leo_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_llama2_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_opengpt_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_phind_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_webchatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_yepchat_tgpt.py
```

### Comparing `python_tgpt-0.7.0/LICENSE` & `python_tgpt-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/PKG-INFO` & `python_tgpt-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.7.0
+Version: 0.7.1
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -71,20 +71,20 @@
 
 <!-- <h1 align="center"> python-tgpt </h1> -->
 <p align="center">
 <!--
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 -->
 <a href="https://github.com/Simatwa/python-tgpt/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
+<a href=""><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
 <a href="https://pypi.org/project/python-tgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/python-tgpt?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
-<a href="#"><img alt="Website status" src="https://img.shields.io/website?url=https://python-tgpt.onrender.com"/></a>
+<a href="https://python-tgpt.onrender.com"><img alt="Website status" src="https://img.shields.io/website?url=https://python-tgpt.onrender.com"/></a>
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml"><img alt="Python Package flow" src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml/badge.svg?branch=master"/></a>
-<a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
+<a href=""><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="https://pepy.tech/project/tgpt2"><img src="https://static.pepy.tech/personalized-badge/tgpt2?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <a href="https://pepy.tech/project/python-tgpt"><img src="https://static.pepy.tech/personalized-badge/python-tgpt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases/latest"><img src="https://img.shields.io/github/downloads/Simatwa/python-tgpt/total?label=Asset%20Downloads&color=success" alt="Downloads"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/v/release/Simatwa/python-tgpt?color=success&label=Release&logo=github" alt="Latest release"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/release-date/Simatwa/python-tgpt?label=Release date&logo=github" alt="release date"></img></a>
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com/Simatwa/python-tgpt"/></a>      
 <a href="https://wakatime.com/badge/github/Simatwa/tgpt2"><img src="https://wakatime.com/badge/github/Simatwa/tgpt2.svg" alt="wakatime"></a>
@@ -641,21 +641,21 @@
 ```
 or
 ```bash
 $ pytgpt interactive -ttm
 ```
 This flag instructs the system to audiolize the ai responses and then play them, enhancing the user experience by providing auditory feedback.
 
-Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt.
+Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt. However, `auto` as a provider does not work so well with streaming responses, so probably you would need to sacrifice performance for the sake of reliability.
 
 ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot)
 
 If you're not satisfied with the existing interfaces, [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed to enhance your experience by offering a wide range of functionalities. Whether you're interested in engaging in AI-driven conversations, creating images and audio from text, or exploring other innovative features, [pytgpt-bot is equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot)
 
-The bot is maintained as a separate project so you just have to execute a command get it installed :
+The bot is maintained as a separate project so you just have to execute a command to get it installed :
 
 ```
 $ pip install pytgpt-bot
 ```
 
 Usage : `pytgpt bot run <bot-api-token>`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.7.0 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.7.1 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -35,16 +35,16 @@
 Requires-Dist: gpt4all==2.2.0; extra == "all" Requires-Dist: click==8.1.3;
 extra == "all" Requires-Dist: rich==13.3.4; extra == "all" Requires-Dist:
 clipman==3.1.0; extra == "all" Requires-Dist: pyperclip==1.8.2; extra == "all"
 Requires-Dist: colorama==0.4.6; extra == "all" Requires-Dist: g4f>=0.3.0.8;
 extra == "all" Requires-Dist: python-dotenv==1.0.0; extra == "all" Requires-
 Dist: fastapi[all]==0.110.1; extra == "all"
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
-  _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_W_e_b_s_i_t_e_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]
-   _[_c_o_v_e_r_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]
+  _[_L_i_c_e_n_s_e_][Python version]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_W_e_b_s_i_t_e_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]
+   [coverage]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]
                  _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
      _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
 ```python >>> import pytgpt.phind as phind >>> bot = phind.PHIND() >>> bot.chat
 ('hello there') 'Hello! How can I assist you today?' ``` ```python from
 pytgpt.imager import Imager img = Imager() generated_images = img.generate
@@ -233,24 +233,26 @@
 flag or its shorthand `-ttm` when running your commands. For example: ```bash $
 pytgpt generate "Generate an ogre story" --talk-to-me ``` or ```bash $ pytgpt
 interactive -ttm ``` This flag instructs the system to audiolize the ai
 responses and then play them, enhancing the user experience by providing
 auditory feedback. Version **0.6.4** introduces another dynamic provider,
 `auto`, which denotes the working provider **overall**. This relieves you of
 the workload of manually checking a working provider each time you fire up
-pytgpt. ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot) If you're not
-satisfied with the existing interfaces, [pytgpt-bot](https://github.com/
+pytgpt. However, `auto` as a provider does not work so well with streaming
+responses, so probably you would need to sacrifice performance for the sake of
+reliability. ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot) If you're
+not satisfied with the existing interfaces, [pytgpt-bot](https://github.com/
 Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed
 to enhance your experience by offering a wide range of functionalities. Whether
 you're interested in engaging in AI-driven conversations, creating images and
 audio from text, or exploring other innovative features, [pytgpt-bot is
 equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot) The bot is
-maintained as a separate project so you just have to execute a command get it
-installed : ``` $ pip install pytgpt-bot ``` Usage : `pytgpt bot run ` Or you
-can simply interact with the one running now as [@pytgpt-bot](https://t.me/
+maintained as a separate project so you just have to execute a command to get
+it installed : ``` $ pip install pytgpt-bot ``` Usage : `pytgpt bot run ` Or
+you can simply interact with the one running now as [@pytgpt-bot](https://t.me/
 pytgpt_bot) For more usage info run `$ pytgpt --help` ``` Usage: pytgpt
 [OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the version and exit. -
 h, --help Show this message and exit. Commands: api FastAPI control endpoint
 awesome Perform CRUD operations on awesome-prompts bot Telegram bot interface
 control generate Generate a quick response with AI gpt4free Discover gpt4free
 models, providers etc imager Generate images with pollinations.ai interactive
 Chat with AI interactively (Default) utils Utility endpoint for pytgpt
```

### Comparing `python_tgpt-0.7.0/README.md` & `python_tgpt-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 <!-- <h1 align="center"> python-tgpt </h1> -->
 <p align="center">
 <!--
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 -->
 <a href="https://github.com/Simatwa/python-tgpt/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
+<a href=""><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
 <a href="https://pypi.org/project/python-tgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/python-tgpt?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
-<a href="#"><img alt="Website status" src="https://img.shields.io/website?url=https://python-tgpt.onrender.com"/></a>
+<a href="https://python-tgpt.onrender.com"><img alt="Website status" src="https://img.shields.io/website?url=https://python-tgpt.onrender.com"/></a>
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml"><img alt="Python Package flow" src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml/badge.svg?branch=master"/></a>
-<a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
+<a href=""><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="https://pepy.tech/project/tgpt2"><img src="https://static.pepy.tech/personalized-badge/tgpt2?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <a href="https://pepy.tech/project/python-tgpt"><img src="https://static.pepy.tech/personalized-badge/python-tgpt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases/latest"><img src="https://img.shields.io/github/downloads/Simatwa/python-tgpt/total?label=Asset%20Downloads&color=success" alt="Downloads"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/v/release/Simatwa/python-tgpt?color=success&label=Release&logo=github" alt="Latest release"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/release-date/Simatwa/python-tgpt?label=Release date&logo=github" alt="release date"></img></a>
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com/Simatwa/python-tgpt"/></a>      
 <a href="https://wakatime.com/badge/github/Simatwa/tgpt2"><img src="https://wakatime.com/badge/github/Simatwa/tgpt2.svg" alt="wakatime"></a>
@@ -574,21 +574,21 @@
 ```
 or
 ```bash
 $ pytgpt interactive -ttm
 ```
 This flag instructs the system to audiolize the ai responses and then play them, enhancing the user experience by providing auditory feedback.
 
-Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt.
+Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt. However, `auto` as a provider does not work so well with streaming responses, so probably you would need to sacrifice performance for the sake of reliability.
 
 ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot)
 
 If you're not satisfied with the existing interfaces, [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed to enhance your experience by offering a wide range of functionalities. Whether you're interested in engaging in AI-driven conversations, creating images and audio from text, or exploring other innovative features, [pytgpt-bot is equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot)
 
-The bot is maintained as a separate project so you just have to execute a command get it installed :
+The bot is maintained as a separate project so you just have to execute a command to get it installed :
 
 ```
 $ pip install pytgpt-bot
 ```
 
 Usage : `pytgpt bot run <bot-api-token>`
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
-  _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_W_e_b_s_i_t_e_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]
-   _[_c_o_v_e_r_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]
+  _[_L_i_c_e_n_s_e_][Python version]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_W_e_b_s_i_t_e_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]
+   [coverage]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]
                  _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
      _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
 ```python >>> import pytgpt.phind as phind >>> bot = phind.PHIND() >>> bot.chat
 ('hello there') 'Hello! How can I assist you today?' ``` ```python from
 pytgpt.imager import Imager img = Imager() generated_images = img.generate
@@ -193,24 +193,26 @@
 flag or its shorthand `-ttm` when running your commands. For example: ```bash $
 pytgpt generate "Generate an ogre story" --talk-to-me ``` or ```bash $ pytgpt
 interactive -ttm ``` This flag instructs the system to audiolize the ai
 responses and then play them, enhancing the user experience by providing
 auditory feedback. Version **0.6.4** introduces another dynamic provider,
 `auto`, which denotes the working provider **overall**. This relieves you of
 the workload of manually checking a working provider each time you fire up
-pytgpt. ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot) If you're not
-satisfied with the existing interfaces, [pytgpt-bot](https://github.com/
+pytgpt. However, `auto` as a provider does not work so well with streaming
+responses, so probably you would need to sacrifice performance for the sake of
+reliability. ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot) If you're
+not satisfied with the existing interfaces, [pytgpt-bot](https://github.com/
 Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed
 to enhance your experience by offering a wide range of functionalities. Whether
 you're interested in engaging in AI-driven conversations, creating images and
 audio from text, or exploring other innovative features, [pytgpt-bot is
 equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot) The bot is
-maintained as a separate project so you just have to execute a command get it
-installed : ``` $ pip install pytgpt-bot ``` Usage : `pytgpt bot run ` Or you
-can simply interact with the one running now as [@pytgpt-bot](https://t.me/
+maintained as a separate project so you just have to execute a command to get
+it installed : ``` $ pip install pytgpt-bot ``` Usage : `pytgpt bot run ` Or
+you can simply interact with the one running now as [@pytgpt-bot](https://t.me/
 pytgpt_bot) For more usage info run `$ pytgpt --help` ``` Usage: pytgpt
 [OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the version and exit. -
 h, --help Show this message and exit. Commands: api FastAPI control endpoint
 awesome Perform CRUD operations on awesome-prompts bot Telegram bot interface
 control generate Generate a quick response with AI gpt4free Discover gpt4free
 models, providers etc imager Generate images with pollinations.ai interactive
 Chat with AI interactively (Default) utils Utility endpoint for pytgpt
```

### Comparing `python_tgpt-0.7.0/setup.py` & `python_tgpt-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="python-tgpt",
-    version="0.7.0",
+    version="0.7.1",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Interact with AI without API key",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `python_tgpt-0.7.0/src/pytgpt/__init__.py` & `python_tgpt-0.7.1/src/pytgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/api/__init__.py` & `python_tgpt-0.7.1/src/pytgpt/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/api/utils.py` & `python_tgpt-0.7.1/src/pytgpt/api/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/api/v1.py` & `python_tgpt-0.7.1/src/pytgpt/api/v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,16 +289,16 @@
             "example": {
                 "url": "http://localhost:8000/static/audios/f9d4233f-9b78-4d87-bc27-5d2ab928f673.mp3",
             }
         }
     }
 
 
-def init_provider(payload: TextGenerationPayload) -> object:
-    return provider_map.get(payload.provider, AsyncAUTO)(
+async def init_provider(payload: TextGenerationPayload) -> object:
+    return provider_map.get(payload.provider, AsyncGPT4FREE)(
         is_conversation=False,  # payload.is_conversation,
         max_tokens=payload.max_tokens,
         timeout=payload.timeout,
         proxies=payload.proxy,
     )
 
 
@@ -328,29 +328,29 @@
     - `timeout` : Http request timeout.
     - `proxy` : Http request proxy.
 
     *Ensure `proxy` value is correct otherwise make it `null`*
 
     **NOTE** : Example values are modified for illustration purposes.
     """
-    provider_obj: AsyncGPT4FREE = init_provider(payload)
+    provider_obj: AsyncGPT4FREE = await init_provider(payload)
     ai_generated_text: str = await provider_obj.chat(payload.prompt)
     return ProviderResponse(
         provider=(
             provider_obj.provider_name
             if payload.provider == "auto"
             else payload.provider
         ),
         text=ai_generated_text,
         body=provider_obj.last_response if payload.whole else None,
     )
 
 
 async def generate_streaming_response(payload: TextGenerationPayload) -> Generator:
-    provider_obj = init_provider(payload)
+    provider_obj = await init_provider(payload)
     async_chat = await provider_obj.chat(payload.prompt, stream=True)
     async for text in async_chat:
         response = ProviderResponse(
             provider=(
                 provider_obj.provider_name
                 if payload.provider == "auto"
                 else payload.provider
@@ -478,15 +478,15 @@
 async def redirect_image_generation(prompt: str):
     """Redirect image generation request to [pollinations.ai](https://pollinations.ai)"""
     return RedirectResponse(
         f"https://image.pollinations.ai/prompt/{prompt}",
     )
 
 
-@app.post("/audio", name="text-to-audio")
+@app.post("/voice", name="text-to-voice")
 @api_exception_handler
 async def text_to_audio(
     payload: TextToAudioPayload, request: Request
 ) -> TextToAudioResponse:
     """Vocalize text
 
     - `message` : Text to be synthesised.
@@ -504,15 +504,15 @@
         proxies=payload.proxy,
         timeout=payload.timeout,
         save_to=Audio.cache_dir.joinpath(filename).as_posix(),
     )
     return TextToAudioResponse(url=f"{host}/static/audios/" + filename)
 
 
-@app.get("/audio", name="text-to-audio (bytes)")
+@app.get("/voice", name="text-to-voice (bytes)")
 @api_exception_handler
 async def text_to_audio_bytes(
     message: str,
     voice: str = "en-US-Wavenet-C",
     timeout: int = 30,
     proxy: Union[str, None] = None,
 ):
```

### Comparing `python_tgpt-0.7.0/src/pytgpt/async_providers.py` & `python_tgpt-0.7.1/src/pytgpt/async_providers.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/auto/main.py` & `python_tgpt-0.7.1/src/pytgpt/auto/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/base.py` & `python_tgpt-0.7.1/src/pytgpt/base.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/blackboxai/main.py` & `python_tgpt-0.7.1/src/pytgpt/blackboxai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/console.py` & `python_tgpt-0.7.1/src/pytgpt/console.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/gemini/main.py` & `python_tgpt-0.7.1/src/pytgpt/gemini/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/gpt4all/main.py` & `python_tgpt-0.7.1/src/pytgpt/gpt4all/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/gpt4free/main.py` & `python_tgpt-0.7.1/src/pytgpt/gpt4free/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/gpt4free/utils.py` & `python_tgpt-0.7.1/src/pytgpt/gpt4free/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/groq/main.py` & `python_tgpt-0.7.1/src/pytgpt/groq/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/imager/imager.py` & `python_tgpt-0.7.1/src/pytgpt/imager/imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/koboldai/main.py` & `python_tgpt-0.7.1/src/pytgpt/koboldai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/leo/main.py` & `python_tgpt-0.7.1/src/pytgpt/leo/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/llama2/main.py` & `python_tgpt-0.7.1/src/pytgpt/llama2/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/openai/main.py` & `python_tgpt-0.7.1/src/pytgpt/openai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/opengpt/main.py` & `python_tgpt-0.7.1/src/pytgpt/opengpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/perplexity/main.py` & `python_tgpt-0.7.1/src/pytgpt/perplexity/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/phind/main.py` & `python_tgpt-0.7.1/src/pytgpt/phind/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/poe/main.py` & `python_tgpt-0.7.1/src/pytgpt/poe/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/utils.py` & `python_tgpt-0.7.1/src/pytgpt/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/webchatgpt/main.py` & `python_tgpt-0.7.1/src/pytgpt/webchatgpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/pytgpt/yepchat/main.py` & `python_tgpt-0.7.1/src/pytgpt/yepchat/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/python_tgpt.egg-info/PKG-INFO` & `python_tgpt-0.7.1/src/python_tgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.7.0
+Version: 0.7.1
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -71,20 +71,20 @@
 
 <!-- <h1 align="center"> python-tgpt </h1> -->
 <p align="center">
 <!--
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 -->
 <a href="https://github.com/Simatwa/python-tgpt/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
+<a href=""><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
 <a href="https://pypi.org/project/python-tgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/python-tgpt?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
-<a href="#"><img alt="Website status" src="https://img.shields.io/website?url=https://python-tgpt.onrender.com"/></a>
+<a href="https://python-tgpt.onrender.com"><img alt="Website status" src="https://img.shields.io/website?url=https://python-tgpt.onrender.com"/></a>
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml"><img alt="Python Package flow" src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml/badge.svg?branch=master"/></a>
-<a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
+<a href=""><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="https://pepy.tech/project/tgpt2"><img src="https://static.pepy.tech/personalized-badge/tgpt2?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <a href="https://pepy.tech/project/python-tgpt"><img src="https://static.pepy.tech/personalized-badge/python-tgpt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases/latest"><img src="https://img.shields.io/github/downloads/Simatwa/python-tgpt/total?label=Asset%20Downloads&color=success" alt="Downloads"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/v/release/Simatwa/python-tgpt?color=success&label=Release&logo=github" alt="Latest release"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/release-date/Simatwa/python-tgpt?label=Release date&logo=github" alt="release date"></img></a>
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com/Simatwa/python-tgpt"/></a>      
 <a href="https://wakatime.com/badge/github/Simatwa/tgpt2"><img src="https://wakatime.com/badge/github/Simatwa/tgpt2.svg" alt="wakatime"></a>
@@ -641,21 +641,21 @@
 ```
 or
 ```bash
 $ pytgpt interactive -ttm
 ```
 This flag instructs the system to audiolize the ai responses and then play them, enhancing the user experience by providing auditory feedback.
 
-Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt.
+Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt. However, `auto` as a provider does not work so well with streaming responses, so probably you would need to sacrifice performance for the sake of reliability.
 
 ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot)
 
 If you're not satisfied with the existing interfaces, [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed to enhance your experience by offering a wide range of functionalities. Whether you're interested in engaging in AI-driven conversations, creating images and audio from text, or exploring other innovative features, [pytgpt-bot is equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot)
 
-The bot is maintained as a separate project so you just have to execute a command get it installed :
+The bot is maintained as a separate project so you just have to execute a command to get it installed :
 
 ```
 $ pip install pytgpt-bot
 ```
 
 Usage : `pytgpt bot run <bot-api-token>`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.7.0 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.7.1 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -35,16 +35,16 @@
 Requires-Dist: gpt4all==2.2.0; extra == "all" Requires-Dist: click==8.1.3;
 extra == "all" Requires-Dist: rich==13.3.4; extra == "all" Requires-Dist:
 clipman==3.1.0; extra == "all" Requires-Dist: pyperclip==1.8.2; extra == "all"
 Requires-Dist: colorama==0.4.6; extra == "all" Requires-Dist: g4f>=0.3.0.8;
 extra == "all" Requires-Dist: python-dotenv==1.0.0; extra == "all" Requires-
 Dist: fastapi[all]==0.110.1; extra == "all"
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
-  _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_W_e_b_s_i_t_e_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]
-   _[_c_o_v_e_r_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]
+  _[_L_i_c_e_n_s_e_][Python version]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_W_e_b_s_i_t_e_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]
+   [coverage]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]
                  _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
      _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
 ```python >>> import pytgpt.phind as phind >>> bot = phind.PHIND() >>> bot.chat
 ('hello there') 'Hello! How can I assist you today?' ``` ```python from
 pytgpt.imager import Imager img = Imager() generated_images = img.generate
@@ -233,24 +233,26 @@
 flag or its shorthand `-ttm` when running your commands. For example: ```bash $
 pytgpt generate "Generate an ogre story" --talk-to-me ``` or ```bash $ pytgpt
 interactive -ttm ``` This flag instructs the system to audiolize the ai
 responses and then play them, enhancing the user experience by providing
 auditory feedback. Version **0.6.4** introduces another dynamic provider,
 `auto`, which denotes the working provider **overall**. This relieves you of
 the workload of manually checking a working provider each time you fire up
-pytgpt. ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot) If you're not
-satisfied with the existing interfaces, [pytgpt-bot](https://github.com/
+pytgpt. However, `auto` as a provider does not work so well with streaming
+responses, so probably you would need to sacrifice performance for the sake of
+reliability. ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot) If you're
+not satisfied with the existing interfaces, [pytgpt-bot](https://github.com/
 Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed
 to enhance your experience by offering a wide range of functionalities. Whether
 you're interested in engaging in AI-driven conversations, creating images and
 audio from text, or exploring other innovative features, [pytgpt-bot is
 equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot) The bot is
-maintained as a separate project so you just have to execute a command get it
-installed : ``` $ pip install pytgpt-bot ``` Usage : `pytgpt bot run ` Or you
-can simply interact with the one running now as [@pytgpt-bot](https://t.me/
+maintained as a separate project so you just have to execute a command to get
+it installed : ``` $ pip install pytgpt-bot ``` Usage : `pytgpt bot run ` Or
+you can simply interact with the one running now as [@pytgpt-bot](https://t.me/
 pytgpt_bot) For more usage info run `$ pytgpt --help` ``` Usage: pytgpt
 [OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the version and exit. -
 h, --help Show this message and exit. Commands: api FastAPI control endpoint
 awesome Perform CRUD operations on awesome-prompts bot Telegram bot interface
 control generate Generate a quick response with AI gpt4free Discover gpt4free
 models, providers etc imager Generate images with pollinations.ai interactive
 Chat with AI interactively (Default) utils Utility endpoint for pytgpt
```

### Comparing `python_tgpt-0.7.0/src/python_tgpt.egg-info/SOURCES.txt` & `python_tgpt-0.7.1/src/python_tgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/src/python_tgpt.egg-info/requires.txt` & `python_tgpt-0.7.1/src/python_tgpt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/tests/test_api.py` & `python_tgpt-0.7.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/tests/test_imager.py` & `python_tgpt-0.7.1/tests/test_imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.0/tests/test_utils.py` & `python_tgpt-0.7.1/tests/test_utils.py`

 * *Files identical despite different names*

